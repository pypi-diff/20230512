# Comparing `tmp/uoy-assessment-uploader-0.3.0.tar.gz` & `tmp/uoy-assessment-uploader-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uoy-assessment-uploader-0.3.0.tar", last modified: Mon May  8 15:54:42 2023, max compression
+gzip compressed data, was "uoy-assessment-uploader-0.4.0.tar", last modified: Fri May 12 20:03:35 2023, max compression
```

## Comparing `uoy-assessment-uploader-0.3.0.tar` & `uoy-assessment-uploader-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    32422 2023-05-08 15:54:31.863871 uoy-assessment-uploader-0.3.0/LICENSE
--rw-r--r--   0        0        0     1369 2023-05-08 15:54:31.867871 uoy-assessment-uploader-0.3.0/README.md
--rw-r--r--   0        0        0      741 2023-05-08 15:54:31.867871 uoy-assessment-uploader-0.3.0/pyproject.toml
--rwxr-xr-x   0        0        0     6783 2023-05-08 15:54:31.867871 uoy-assessment-uploader-0.3.0/uoy_assessment_uploader/__init__.py
--rw-r--r--   0        0        0       27 2023-05-08 15:54:31.867871 uoy-assessment-uploader-0.3.0/uoy_assessment_uploader/__main__.py
--rw-r--r--   0        0        0     1551 2023-05-08 15:54:31.867871 uoy-assessment-uploader-0.3.0/uoy_assessment_uploader/selenium.py
--rw-r--r--   0        0        0     2006 1970-01-01 00:00:00.000000 uoy-assessment-uploader-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    32422 2023-05-12 20:03:22.969493 uoy-assessment-uploader-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1369 2023-05-12 20:03:22.969493 uoy-assessment-uploader-0.4.0/README.md
+-rw-r--r--   0        0        0      768 2023-05-12 20:03:22.969493 uoy-assessment-uploader-0.4.0/pyproject.toml
+-rwxr-xr-x   0        0        0     7942 2023-05-12 20:03:22.973493 uoy-assessment-uploader-0.4.0/uoy_assessment_uploader/__init__.py
+-rw-r--r--   0        0        0       27 2023-05-12 20:03:22.973493 uoy-assessment-uploader-0.4.0/uoy_assessment_uploader/__main__.py
+-rw-r--r--   0        0        0     1551 2023-05-12 20:03:22.973493 uoy-assessment-uploader-0.4.0/uoy_assessment_uploader/selenium.py
+-rw-r--r--   0        0        0     2040 1970-01-01 00:00:00.000000 uoy-assessment-uploader-0.4.0/PKG-INFO
```

### Comparing `uoy-assessment-uploader-0.3.0/LICENSE` & `uoy-assessment-uploader-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uoy-assessment-uploader-0.3.0/README.md` & `uoy-assessment-uploader-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `uoy-assessment-uploader-0.3.0/pyproject.toml` & `uoy-assessment-uploader-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     "Environment :: Console",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Natural Language :: English",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "selenium ~= 4.9.0",
-    "webdriver-manager ~= 3.8.6"
+    "webdriver-manager ~= 3.8.6",
+    "keyring ~= 23.13.1",
 ]
 dynamic = ["version", "description"]
 
 [project.urls]
 Home = "https://github.com/joelsgp/uoy-assessment-uploader"
 
 [project.scripts]
```

### Comparing `uoy-assessment-uploader-0.3.0/uoy_assessment_uploader/__init__.py` & `uoy-assessment-uploader-0.4.0/uoy_assessment_uploader/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 """Tool for automating submitting assessments to the University of York Computer Science department."""
 
 import getpass
 import hashlib
 import sys
 from argparse import ArgumentParser
 from pathlib import Path
-from typing import Optional
+from typing import Optional, Sequence
 
+import keyring
 from selenium import webdriver
 from selenium.webdriver.chrome.service import Service as ChromeService
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.support import expected_conditions as ec
 from selenium.webdriver.support.wait import WebDriverWait
 from webdriver_manager.chrome import ChromeDriverManager
 
 from .selenium import enter_exam_number, load_cookies, login, save_cookies, upload
 
 
-__version__ = "0.3.0"
+# todo: re-implement with saml auth and requests, as alternative to selenium
 
+
+__version__ = "0.4.0"
+
+# used for service_name in keyring
+NAME = "uoy-assessment-uploader"
 # timeout for selenium waits, in seconds
 TIMEOUT = 10
 
 DEFAULT_ARG_FILE = "exam.zip"
 DEFAULT_ARG_COOKIE_FILE = ".cookies.json"
 
 URL_SUBMIT_BASE = "https://teaching.cs.york.ac.uk/student"
@@ -59,14 +65,19 @@
     )
     # options
     parser.add_argument(
         "--dry-run",
         action="store_true",
         help="Log in but don't actually upload the file.",
     )
+    parser.add_argument(
+        "--use-keyring",
+        action="store_true",
+        help="Use the keyring service for storing and retrieving password and exam number. keyring must be installed.",
+    )
     # selenium cookies
     parser.add_argument(
         "--cookie-file",
         type=Path,
         default=DEFAULT_ARG_COOKIE_FILE,
         help="default: '%(default)s'",
     )
@@ -89,66 +100,90 @@
         help="Hide the browser window. Full auto.",
     )
 
     return parser
 
 
 class Args:
-    username: str
-    password: str
-    exam_number: str
+    username: Optional[str]
+    password: Optional[str]
+    exam_number: Optional[str]
     submit_url: str
     file: Path
     dry_run: bool
+    use_keyring: bool
     cookie_file: Path
     save_cookies: bool
     delete_cookies: bool
     headless: bool
 
 
-def ensure_details(
-    current: str, prompt: Optional[str] = None, hide: bool = False
+def parse_args(argv: Sequence[str] = None) -> Args:
+    parser = get_parser()
+    args = Args()
+    parser.parse_args(argv, namespace=args)
+    return args
+
+
+def ensure_username(username: Optional[str]) -> str:
+    if username is None:
+        username = input("Username: ")
+    return username
+
+
+def ensure_password(
+    password: Optional[str], username: str, which: str, use_keyring: bool
 ) -> str:
-    if current is not None:
-        return current
+    service_name = f"{NAME}-{which}"
+    # get password
+    if password is None and use_keyring:
+        password = keyring.get_password(service_name, username)
+    if password is None:
+        prompt = f"{which}: "
+        password = getpass.getpass(prompt)
+    # save password to keyring
+    if use_keyring:
+        keyring.set_password(service_name, username, password)
 
-    if hide:
-        current = getpass.getpass()
-    else:
-        current = input(prompt)
-    return current
+    return password
 
 
-def do(
+def run_selenium(
     driver: WebDriver,
     submit_url: str,
     username: Optional[str],
     password: Optional[str],
     exam_number: Optional[str],
     file_name: str,
     dry_run: bool,
+    use_keyring: bool,
 ):
     wait = WebDriverWait(driver, TIMEOUT)
 
     # breaks loop on submit
     while True:
         driver.get(submit_url)
         # username/password login page
         if driver.current_url == URL_LOGIN:
             print("Logging in..")
-            username = ensure_details(username, "Enter username: ")
-            password = ensure_details(password, hide=True)
+            username = ensure_username(username)
+            password = ensure_password(
+                password, username, which="Password", use_keyring=use_keyring
+            )
             login(driver, username, password)
             wait.until(
                 ec.any_of(ec.url_to_be(URL_EXAM_NUMBER), ec.url_to_be(submit_url))
             )
         # exam number login page
         elif driver.current_url == URL_EXAM_NUMBER:
             print("Entering exam number..")
-            exam_number = ensure_details(exam_number, "Enter exam number: ")
+            username = ensure_username(username)
+            exam_number = ensure_password(
+                exam_number, username, which="Exam number", use_keyring=use_keyring
+            )
             enter_exam_number(driver, exam_number)
             wait.until(ec.url_to_be(submit_url))
         # logged in, upload page
         elif driver.current_url == submit_url:
             print("Uploading file...")
             upload(driver, file_name, dry_run)
             if dry_run:
@@ -170,18 +205,15 @@
     submit_url = submit_url.removeprefix(base).strip("/")
     submit_url = f"{base}/{submit_url}"
     return submit_url
 
 
 def main():
     # load arguments
-    parser = get_parser()
-    args = Args()
-    parser.parse_args(namespace=args)
-
+    args = parse_args()
     # verify arguments
     submit_url = resolve_submit_url(args.submit_url)
     # check zip to be uploaded exists
     if not args.file.is_file():
         print(f"File doesn't exist '{args.file}'.")
         sys.exit(1)
     print(f"Found file '{args.file}'.")
@@ -208,22 +240,23 @@
         # load cookies
         if args.delete_cookies:
             args.cookie_file.unlink(missing_ok=True)
         elif args.save_cookies:
             load_cookies(driver, args.cookie_file)
 
         # run
-        do(
+        run_selenium(
             driver=driver,
             submit_url=submit_url,
             username=args.username,
             password=args.password,
             exam_number=args.exam_number,
             file_name=file_name,
             dry_run=args.dry_run,
+            use_keyring=args.use_keyring,
         )
 
         # save cookies
         if args.save_cookies:
             print("Saving cookies.")
             save_cookies(driver, args.cookie_file)
```

### Comparing `uoy-assessment-uploader-0.3.0/uoy_assessment_uploader/selenium.py` & `uoy-assessment-uploader-0.4.0/uoy_assessment_uploader/selenium.py`

 * *Files identical despite different names*

### Comparing `uoy-assessment-uploader-0.3.0/PKG-INFO` & `uoy-assessment-uploader-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: uoy-assessment-uploader
-Version: 0.3.0
+Version: 0.4.0
 Summary: Tool for automating submitting assessments to the University of York Computer Science department.
 Author-email: jmcb <joelsgp@protonmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Requires-Dist: selenium ~= 4.9.0
 Requires-Dist: webdriver-manager ~= 3.8.6
+Requires-Dist: keyring ~= 23.13.1
 Project-URL: Home, https://github.com/joelsgp/uoy-assessment-uploader
 
 # uoy_assessment_uploader
 
 ## Install
 1. When you have Python and Pip ready, it's as easy as:
    ```shell
```


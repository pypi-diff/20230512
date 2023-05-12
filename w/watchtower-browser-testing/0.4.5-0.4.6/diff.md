# Comparing `tmp/watchtower_browser_testing-0.4.5.tar.gz` & `tmp/watchtower_browser_testing-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.4.5.tar", last modified: Mon May  1 13:55:29 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.4.6.tar", last modified: Fri May 12 10:58:46 2023, max compression
```

## Comparing `watchtower_browser_testing-0.4.5.tar` & `watchtower_browser_testing-0.4.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 13:55:29.471115 watchtower_browser_testing-0.4.5/
--rw-rw-rw-   0        0        0      310 2023-05-01 13:55:29.471115 watchtower_browser_testing-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.4.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 13:55:29.471115 watchtower_browser_testing-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1135 2023-04-17 17:34:58.000000 watchtower_browser_testing-0.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 13:55:29.459109 watchtower_browser_testing-0.4.5/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.4.5/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      945 2023-04-18 07:07:32.000000 watchtower_browser_testing-0.4.5/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.4.5/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.4.5/watchtower_browser_testing/helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-01 13:55:29.469716 watchtower_browser_testing-0.4.5/watchtower_browser_testing/templates/
--rw-rw-rw-   0        0        0     6195 2023-04-25 13:45:16.000000 watchtower_browser_testing-0.4.5/watchtower_browser_testing/templates/measurement_plan.html
--rw-rw-rw-   0        0        0    17363 2023-05-01 13:54:03.000000 watchtower_browser_testing-0.4.5/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     7743 2023-04-17 17:27:01.000000 watchtower_browser_testing-0.4.5/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0       21 2023-05-01 13:55:27.000000 watchtower_browser_testing-0.4.5/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-05-01 13:55:29.465128 watchtower_browser_testing-0.4.5/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-05-01 13:55:29.000000 watchtower_browser_testing-0.4.5/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      609 2023-05-01 13:55:29.000000 watchtower_browser_testing-0.4.5/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 13:55:29.000000 watchtower_browser_testing-0.4.5/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-05-01 13:55:29.000000 watchtower_browser_testing-0.4.5/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-05-01 13:55:29.000000 watchtower_browser_testing-0.4.5/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 10:58:46.138528 watchtower_browser_testing-0.4.6/
+-rw-rw-rw-   0        0        0      310 2023-05-12 10:58:46.138528 watchtower_browser_testing-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.4.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-12 10:58:46.138528 watchtower_browser_testing-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1135 2023-04-17 17:34:58.000000 watchtower_browser_testing-0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:58:46.122903 watchtower_browser_testing-0.4.6/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      945 2023-04-18 07:07:32.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing/helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:58:46.138528 watchtower_browser_testing-0.4.6/watchtower_browser_testing/templates/
+-rw-rw-rw-   0        0        0     6195 2023-04-25 13:45:16.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing/templates/measurement_plan.html
+-rw-rw-rw-   0        0        0    17927 2023-05-02 09:55:35.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     7743 2023-04-17 17:27:01.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0       21 2023-05-12 10:58:03.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:58:46.138528 watchtower_browser_testing-0.4.6/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-05-12 10:58:45.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2023-05-12 10:58:45.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 10:58:45.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-05-12 10:58:45.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-05-12 10:58:45.000000 watchtower_browser_testing-0.4.6/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.4.5/setup.py` & `watchtower_browser_testing-0.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.5/watchtower_browser_testing/config.py` & `watchtower_browser_testing-0.4.6/watchtower_browser_testing/config.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.5/watchtower_browser_testing/helpers.py` & `watchtower_browser_testing-0.4.6/watchtower_browser_testing/helpers.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.5/watchtower_browser_testing/templates/measurement_plan.html` & `watchtower_browser_testing-0.4.6/watchtower_browser_testing/templates/measurement_plan.html`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.5/watchtower_browser_testing/testsuite.py` & `watchtower_browser_testing-0.4.6/watchtower_browser_testing/testsuite.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import importlib.util
 import inspect
 import sys
 import types
 import functools
 import json
 import datetime
+import webbrowser
 
 from playwright.sync_api import sync_playwright
 from marko.ext.gfm import gfm as markdown
 import jinja2
 import pytz
 import tzlocal
 
@@ -465,14 +466,30 @@
 
         test_results = test_results or {}
 
         return self.render_html(title=title,
                                 content=content,
                                 test_results=test_results)
 
+    def view_in_browser(self,
+                        title='Measurement plan',
+                        test_results=None,
+                        temp_file_path='temp.html'):
+
+        if not os.path.isabs(temp_file_path):
+            temp_file_path = os.path.abspath(os.path.join(os.getcwd(), temp_file_path))
+
+        html = self.html_report(title=title, test_results=test_results)
+        with open(temp_file_path, 'w') as f:
+            f.write(html)
+
+        webbrowser.open('file://' + os.path.realpath(temp_file_path))
+
+
+
     @classmethod
     def render_html(cls,
                     title,
                     content,
                     test_results,
                     run_tests_token=None):
```

### Comparing `watchtower_browser_testing-0.4.5/watchtower_browser_testing/tracking_validation.py` & `watchtower_browser_testing-0.4.6/watchtower_browser_testing/tracking_validation.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.5/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.4.6/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/enochecker_test-0.7.1.tar.gz` & `tmp/enochecker_test-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enochecker_test-0.7.1.tar", last modified: Wed Apr 27 18:46:39 2022, max compression
+gzip compressed data, was "enochecker_test-0.8.0.tar", last modified: Fri May 12 18:28:12 2023, max compression
```

## Comparing `enochecker_test-0.7.1.tar` & `enochecker_test-0.8.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 18:46:39.499496 enochecker_test-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-04-27 18:46:22.000000 enochecker_test-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-04-27 18:46:22.000000 enochecker_test-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-04-27 18:46:39.499496 enochecker_test-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-04-27 18:46:22.000000 enochecker_test-0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-04-27 18:46:22.000000 enochecker_test-0.7.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 18:46:39.495496 enochecker_test-0.7.1/enochecker_test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-27 18:46:22.000000 enochecker_test-0.7.1/enochecker_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-04-27 18:46:22.000000 enochecker_test-0.7.1/enochecker_test/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      500 2022-04-27 18:46:22.000000 enochecker_test-0.7.1/enochecker_test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2639 2022-04-27 18:46:22.000000 enochecker_test-0.7.1/enochecker_test/main.py
--rw-r--r--   0 runner    (1001) docker     (121)    16839 2022-04-27 18:46:22.000000 enochecker_test-0.7.1/enochecker_test/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 18:46:39.499496 enochecker_test-0.7.1/enochecker_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-04-27 18:46:38.000000 enochecker_test-0.7.1/enochecker_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-04-27 18:46:39.000000 enochecker_test-0.7.1/enochecker_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-27 18:46:38.000000 enochecker_test-0.7.1/enochecker_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-04-27 18:46:39.000000 enochecker_test-0.7.1/enochecker_test.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-27 18:46:37.000000 enochecker_test-0.7.1/enochecker_test.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-04-27 18:46:39.000000 enochecker_test-0.7.1/enochecker_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-04-27 18:46:39.000000 enochecker_test-0.7.1/enochecker_test.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-04-27 18:46:22.000000 enochecker_test-0.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-27 18:46:39.499496 enochecker_test-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-04-27 18:46:22.000000 enochecker_test-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:28:12.633022 enochecker_test-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-12 18:28:01.000000 enochecker_test-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-12 18:28:01.000000 enochecker_test-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-12 18:28:12.633022 enochecker_test-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-12 18:28:01.000000 enochecker_test-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-12 18:28:01.000000 enochecker_test-0.8.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:28:12.629022 enochecker_test-0.8.0/enochecker_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:28:01.000000 enochecker_test-0.8.0/enochecker_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-12 18:28:01.000000 enochecker_test-0.8.0/enochecker_test/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-12 18:28:01.000000 enochecker_test-0.8.0/enochecker_test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-12 18:28:01.000000 enochecker_test-0.8.0/enochecker_test/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-05-12 18:28:01.000000 enochecker_test-0.8.0/enochecker_test/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:28:12.633022 enochecker_test-0.8.0/enochecker_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-12 18:28:12.000000 enochecker_test-0.8.0/enochecker_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-12 18:28:12.000000 enochecker_test-0.8.0/enochecker_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 18:28:12.000000 enochecker_test-0.8.0/enochecker_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-12 18:28:12.000000 enochecker_test-0.8.0/enochecker_test.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 18:28:12.000000 enochecker_test-0.8.0/enochecker_test.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-12 18:28:12.000000 enochecker_test-0.8.0/enochecker_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-12 18:28:12.000000 enochecker_test-0.8.0/enochecker_test.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-12 18:28:01.000000 enochecker_test-0.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 18:28:12.633022 enochecker_test-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-12 18:28:01.000000 enochecker_test-0.8.0/setup.py
```

### Comparing `enochecker_test-0.7.1/LICENSE` & `enochecker_test-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `enochecker_test-0.7.1/PKG-INFO` & `enochecker_test-0.8.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: enochecker_test
-Version: 0.7.1
+Version: 0.8.0
 Summary: Library to help testing checker scripts based on enochecker
 Home-page: https://github.com/enowars/enochecker_test
 Author: ldruschk
 Author-email: ldruschk@posteo.de
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # enochecker_test [![PyPI version](https://badge.fury.io/py/enochecker-test.svg)](https://pypi.org/project/enochecker-test) [![Build Status](https://github.com/enowars/enochecker_test/actions/workflows/pythonapp.yml/badge.svg?branch=main)](https://github.com/enowars/enochecker_test/actions/workflows/pythonapp.yml) ![Lines of code](https://tokei.rs/b1/github/enowars/enochecker_test)
 Automatically test services/checker using the enochecker API
 
-
+# Usage
+`enochecker_test` can be used to run tests against a checker, optionally you can specify wich tests to run e.g. `enochecker_test test_getflag[0] test_exploit_per_exploit_id` will run only the first `getflag` test and all `exploit_per_exploit_id` tests.
```

### Comparing `enochecker_test-0.7.1/enochecker_test/main.py` & `enochecker_test-0.8.0/enochecker_test/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from typing import cast
 
 import jsons
 import pytest
 import requests
 from enochecker_core import CheckerInfoMessage
 from requests.adapters import HTTPAdapter
-from requests.packages.urllib3.util.retry import Retry
+from urllib3.util.retry import Retry
 
 
-def run_tests(host, port, service_address):
+def run_tests(host, port, service_address, test_methods):
     s = requests.Session()
     retry_strategy = Retry(
         total=5,
         backoff_factor=1,
     )
     s.mount("http://", HTTPAdapter(max_retries=retry_strategy))
     r = s.get(f"http://{host}:{port}/service")
@@ -30,30 +30,35 @@
         info.service_name,
         info.flag_variants,
         info.noise_variants,
         info.havoc_variants,
         info.exploit_variants,
     )
 
-    sys.exit(
-        pytest.main(
-            [
-                f"--checker-address={host}",
-                f"--checker-port={port}",
-                f"--service-address={service_address}",
-                f"--flag-variants={info.flag_variants}",
-                f"--noise-variants={info.noise_variants}",
-                f"--havoc-variants={info.havoc_variants}",
-                f"--exploit-variants={info.exploit_variants}",
-                "--durations=0",
-                "-v",
-                os.path.join(os.path.dirname(__file__), "tests.py"),
-            ]
-        )
-    )
+    test_args = [
+        f"--checker-address={host}",
+        f"--checker-port={port}",
+        f"--service-address={service_address}",
+        f"--flag-variants={info.flag_variants}",
+        f"--noise-variants={info.noise_variants}",
+        f"--havoc-variants={info.havoc_variants}",
+        f"--exploit-variants={info.exploit_variants}",
+        "--durations=0",
+        "-v",
+    ]
+
+    if test_methods is None or len(test_methods) == 0:
+        test_args.append(os.path.join(os.path.dirname(__file__), "tests.py"))
+    else:
+        for method in test_methods:
+            test_args.append(
+                os.path.join(os.path.dirname(__file__), "tests.py") + "::" + method
+            )
+
+    sys.exit(pytest.main(test_args))
 
 
 def main():
     if not os.getenv("ENOCHECKER_TEST_CHECKER_ADDRESS"):
         raise Exception(
             "Missing enochecker address, please set the ENOCHECKER_TEST_CHECKER_ADDRESS environment variable"
         )
@@ -70,8 +75,8 @@
     try:
         port_str = os.getenv("ENOCHECKER_TEST_CHECKER_PORT")
         port = int(cast(str, port_str))
     except ValueError:
         raise Exception("Invalid number in ENOCHECKER_TEST_PORT")
 
     logging.basicConfig(level=logging.INFO)
-    run_tests(host, port, _service_address)
+    run_tests(host, port, _service_address, sys.argv[2:])
```

### Comparing `enochecker_test-0.7.1/enochecker_test/tests.py` & `enochecker_test-0.8.0/enochecker_test/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,17 @@
         data=msg,
         headers={"content-type": "application/json"},
         timeout=REQUEST_TIMEOUT,
     )
     result_message: CheckerResultMessage = jsons.loads(
         r.content, CheckerResultMessage, key_transformer=jsons.KEY_TRANSFORMER_SNAKECASE
     )
-    assert CheckerTaskResult(result_message.result) == expected_result
+    assert (
+        CheckerTaskResult(result_message.result) == expected_result
+    ), f"\nMessage: {result_message.message}\n"
     return result_message.attack_info
 
 
 def _test_getflag(
     flag,
     round_id,
     flag_id,
@@ -203,15 +205,17 @@
         headers={"content-type": "application/json"},
         timeout=REQUEST_TIMEOUT,
     )
     assert r.status_code == 200
     result_message: CheckerResultMessage = jsons.loads(
         r.content, CheckerResultMessage, key_transformer=jsons.KEY_TRANSFORMER_SNAKECASE
     )
-    assert CheckerTaskResult(result_message.result) == expected_result
+    assert (
+        CheckerTaskResult(result_message.result) == expected_result
+    ), f"\nMessage: {result_message.message}\n"
 
 
 def _test_putnoise(
     round_id,
     noise_id,
     service_address,
     checker_url,
@@ -234,15 +238,17 @@
         headers={"content-type": "application/json"},
         timeout=REQUEST_TIMEOUT,
     )
     assert r.status_code == 200
     result_message: CheckerResultMessage = jsons.loads(
         r.content, CheckerResultMessage, key_transformer=jsons.KEY_TRANSFORMER_SNAKECASE
     )
-    assert CheckerTaskResult(result_message.result) == expected_result
+    assert (
+        CheckerTaskResult(result_message.result) == expected_result
+    ), f"\nMessage: {result_message.message}\n"
 
 
 def _test_getnoise(
     round_id,
     noise_id,
     service_address,
     checker_url,
@@ -265,15 +271,17 @@
         headers={"content-type": "application/json"},
         timeout=REQUEST_TIMEOUT,
     )
     assert r.status_code == 200
     result_message: CheckerResultMessage = jsons.loads(
         r.content, CheckerResultMessage, key_transformer=jsons.KEY_TRANSFORMER_SNAKECASE
     )
-    assert CheckerTaskResult(result_message.result) == expected_result
+    assert (
+        CheckerTaskResult(result_message.result) == expected_result
+    ), f"\nMessage: {result_message.message}\n"
 
 
 def _test_havoc(
     round_id,
     havoc_id,
     service_address,
     checker_url,
@@ -296,15 +304,17 @@
         headers={"content-type": "application/json"},
         timeout=REQUEST_TIMEOUT,
     )
     assert r.status_code == 200
     result_message: CheckerResultMessage = jsons.loads(
         r.content, CheckerResultMessage, key_transformer=jsons.KEY_TRANSFORMER_SNAKECASE
     )
-    assert CheckerTaskResult(result_message.result) == expected_result
+    assert (
+        CheckerTaskResult(result_message.result) == expected_result
+    ), f"\nMessage: {result_message.message}\n"
 
 
 def _test_exploit(
     flag_regex,
     flag_hash,
     attack_info,
     round_id,
@@ -333,15 +343,17 @@
         headers={"content-type": "application/json"},
         timeout=REQUEST_TIMEOUT,
     )
     assert r.status_code == 200
     result_message: CheckerResultMessage = jsons.loads(
         r.content, CheckerResultMessage, key_transformer=jsons.KEY_TRANSFORMER_SNAKECASE
     )
-    assert CheckerTaskResult(result_message.result) == expected_result
+    assert (
+        CheckerTaskResult(result_message.result) == expected_result
+    ), f"\nMessage: {result_message.message}\n"
     return result_message.flag
 
 
 def test_putflag(round_id, flag_id, service_address, checker_url):
     flag = generate_dummyflag()
     _test_putflag(flag, round_id, flag_id, service_address, checker_url)
```

### Comparing `enochecker_test-0.7.1/enochecker_test.egg-info/PKG-INFO` & `enochecker_test-0.8.0/enochecker_test.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: enochecker-test
-Version: 0.7.1
+Version: 0.8.0
 Summary: Library to help testing checker scripts based on enochecker
 Home-page: https://github.com/enowars/enochecker_test
 Author: ldruschk
 Author-email: ldruschk@posteo.de
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # enochecker_test [![PyPI version](https://badge.fury.io/py/enochecker-test.svg)](https://pypi.org/project/enochecker-test) [![Build Status](https://github.com/enowars/enochecker_test/actions/workflows/pythonapp.yml/badge.svg?branch=main)](https://github.com/enowars/enochecker_test/actions/workflows/pythonapp.yml) ![Lines of code](https://tokei.rs/b1/github/enowars/enochecker_test)
 Automatically test services/checker using the enochecker API
 
-
+# Usage
+`enochecker_test` can be used to run tests against a checker, optionally you can specify wich tests to run e.g. `enochecker_test test_getflag[0] test_exploit_per_exploit_id` will run only the first `getflag` test and all `exploit_per_exploit_id` tests.
```

### Comparing `enochecker_test-0.7.1/setup.py` & `enochecker_test-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="enochecker_test",
-    version="0.7.1",
+    version="0.8.0",
     author="ldruschk",
     author_email="ldruschk@posteo.de",
     description="Library to help testing checker scripts based on enochecker",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/enowars/enochecker_test",
     packages=setuptools.find_packages(),
@@ -28,15 +28,15 @@
         #   5 - Production/Stable
         "Development Status :: 3 - Alpha",
         # Indicate who your project is intended for
         # 'Intended Audience :: Developers',
         "License :: OSI Approved :: MIT License",
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     zip_safe=False,  # This might be needed for reqirements.txt
-    python_requires=">=3.7",
+    python_requires=">=3.8",
 )
```


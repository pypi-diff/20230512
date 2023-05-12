# Comparing `tmp/volttron_lib_base_historian-0.2.1rc0.tar.gz` & `tmp/volttron_lib_base_historian-0.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_lib_base_historian-0.2.1rc0.tar", max compression
+gzip compressed data, was "volttron_lib_base_historian-0.2.1rc1.tar", max compression
```

## Comparing `volttron_lib_base_historian-0.2.1rc0.tar` & `volttron_lib_base_historian-0.2.1rc1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    11928 2023-05-12 16:44:30.056341 volttron_lib_base_historian-0.2.1rc0/LICENSE
--rw-r--r--   0        0        0     2871 2023-05-12 16:45:34.346987 volttron_lib_base_historian-0.2.1rc0/README.md
--rw-r--r--   0        0        0     1278 2023-05-12 16:45:39.171173 volttron_lib_base_historian-0.2.1rc0/pyproject.toml
--rw-r--r--   0        0        0     1250 2023-05-12 16:44:30.060341 volttron_lib_base_historian-0.2.1rc0/src/historian/base/__init__.py
--rw-r--r--   0        0        0    96502 2023-05-12 16:44:30.060341 volttron_lib_base_historian-0.2.1rc0/src/historian/base/base_historian.py
--rw-r--r--   0        0        0        0 2023-05-12 16:44:30.060341 volttron_lib_base_historian-0.2.1rc0/tests/historian/testing/__init__.py
--rw-r--r--   0        0        0    20260 2023-05-12 16:45:34.346987 volttron_lib_base_historian-0.2.1rc0/tests/historian/testing/integration_test_interface.py
--rw-r--r--   0        0        0     3627 1970-01-01 00:00:00.000000 volttron_lib_base_historian-0.2.1rc0/PKG-INFO
+-rw-r--r--   0        0        0    11928 2023-05-12 16:46:01.868830 volttron_lib_base_historian-0.2.1rc1/LICENSE
+-rw-r--r--   0        0        0     2871 2023-05-12 16:46:01.868830 volttron_lib_base_historian-0.2.1rc1/README.md
+-rw-r--r--   0        0        0     1278 2023-05-12 16:47:18.737439 volttron_lib_base_historian-0.2.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     1250 2023-05-12 16:46:01.872830 volttron_lib_base_historian-0.2.1rc1/src/historian/base/__init__.py
+-rw-r--r--   0        0        0    96502 2023-05-12 16:46:01.872830 volttron_lib_base_historian-0.2.1rc1/src/historian/base/base_historian.py
+-rw-r--r--   0        0        0        0 2023-05-12 16:46:01.872830 volttron_lib_base_historian-0.2.1rc1/tests/historian/testing/__init__.py
+-rw-r--r--   0        0        0    20260 2023-05-12 16:46:01.872830 volttron_lib_base_historian-0.2.1rc1/tests/historian/testing/integration_test_interface.py
+-rw-r--r--   0        0        0     3862 1970-01-01 00:00:00.000000 volttron_lib_base_historian-0.2.1rc1/setup.py
+-rw-r--r--   0        0        0     3627 1970-01-01 00:00:00.000000 volttron_lib_base_historian-0.2.1rc1/PKG-INFO
```

### Comparing `volttron_lib_base_historian-0.2.1rc0/LICENSE` & `volttron_lib_base_historian-0.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_lib_base_historian-0.2.1rc0/README.md` & `volttron_lib_base_historian-0.2.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `volttron_lib_base_historian-0.2.1rc0/pyproject.toml` & `volttron_lib_base_historian-0.2.1rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "volttron-lib-base-historian"
-version = "0.2.1rc0"
+version = "0.2.1rc1"
 description = "A base library with extension points for using with the VOLTTRON platform."
 authors = ["VOLTTRON Team <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/eclipse-volttron/volttron-lib-base-historian"
 homepage = "https://github.com/eclipse-volttron/volttron-lib-base-historian"
 keywords = []
```

### Comparing `volttron_lib_base_historian-0.2.1rc0/src/historian/base/__init__.py` & `volttron_lib_base_historian-0.2.1rc1/src/historian/base/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_base_historian-0.2.1rc0/src/historian/base/base_historian.py` & `volttron_lib_base_historian-0.2.1rc1/src/historian/base/base_historian.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_base_historian-0.2.1rc0/tests/historian/testing/integration_test_interface.py` & `volttron_lib_base_historian-0.2.1rc1/tests/historian/testing/integration_test_interface.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_base_historian-0.2.1rc0/PKG-INFO` & `volttron_lib_base_historian-0.2.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-lib-base-historian
-Version: 0.2.1rc0
+Version: 0.2.1rc1
 Summary: A base library with extension points for using with the VOLTTRON platform.
 Home-page: https://github.com/eclipse-volttron/volttron-lib-base-historian
 License: Apache-2.0
 Author: VOLTTRON Team
 Author-email: volttron@pnnl.gov
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```


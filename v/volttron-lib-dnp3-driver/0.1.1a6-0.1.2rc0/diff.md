# Comparing `tmp/volttron_lib_dnp3_driver-0.1.1a6.tar.gz` & `tmp/volttron_lib_dnp3_driver-0.1.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_lib_dnp3_driver-0.1.1a6.tar", max compression
+gzip compressed data, was "volttron_lib_dnp3_driver-0.1.2rc0.tar", max compression
```

## Comparing `volttron_lib_dnp3_driver-0.1.1a6.tar` & `volttron_lib_dnp3_driver-0.1.2rc0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11928 2023-05-12 18:44:09.421295 volttron_lib_dnp3_driver-0.1.1a6/LICENSE
--rw-r--r--   0        0        0    21060 2023-05-12 18:44:09.421295 volttron_lib_dnp3_driver-0.1.1a6/README.md
--rw-r--r--   0        0        0     1588 2023-05-12 18:45:03.525768 volttron_lib_dnp3_driver-0.1.1a6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-12 18:44:09.421295 volttron_lib_dnp3_driver-0.1.1a6/src/volttron/driver/interfaces/dnp3/__init__.py
--rw-r--r--   0        0        0     9189 2023-05-12 18:44:09.421295 volttron_lib_dnp3_driver-0.1.1a6/src/volttron/driver/interfaces/dnp3/dnp3.py
--rw-r--r--   0        0        0    22079 1970-01-01 00:00:00.000000 volttron_lib_dnp3_driver-0.1.1a6/PKG-INFO
+-rw-r--r--   0        0        0    11928 2023-05-12 18:53:14.658853 volttron_lib_dnp3_driver-0.1.2rc0/LICENSE
+-rw-r--r--   0        0        0    21060 2023-05-12 18:54:17.103300 volttron_lib_dnp3_driver-0.1.2rc0/README.md
+-rw-r--r--   0        0        0     1615 2023-05-12 18:57:42.568559 volttron_lib_dnp3_driver-0.1.2rc0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-12 18:53:14.658853 volttron_lib_dnp3_driver-0.1.2rc0/src/volttron/driver/interfaces/dnp3/__init__.py
+-rw-r--r--   0        0        0     9189 2023-05-12 18:54:17.103300 volttron_lib_dnp3_driver-0.1.2rc0/src/volttron/driver/interfaces/dnp3/dnp3.py
+-rw-r--r--   0        0        0    22080 1970-01-01 00:00:00.000000 volttron_lib_dnp3_driver-0.1.2rc0/PKG-INFO
```

### Comparing `volttron_lib_dnp3_driver-0.1.1a6/LICENSE` & `volttron_lib_dnp3_driver-0.1.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_lib_dnp3_driver-0.1.1a6/README.md` & `volttron_lib_dnp3_driver-0.1.2rc0/README.md`

 * *Files identical despite different names*

### Comparing `volttron_lib_dnp3_driver-0.1.1a6/pyproject.toml` & `volttron_lib_dnp3_driver-0.1.2rc0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "volttron-lib-dnp3-driver"
-version = "0.1.1a6"
+version = "0.1.2rc0"
 description = "A minimal implementation of a driver for the VOLTTRON platform."
 authors = ["VOLTTRON Team <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/eclipse-volttron/volttron-lib-dnp3-driver"
 homepage = "https://github.com/eclipse-volttron/volttron-lib-dnp3-driver"
 keywords = []
@@ -38,14 +38,15 @@
 mock = "^4.0.3"
 pre-commit = "^2.17.0"
 yapf = "^0.32.0"
 toml = "^0.10.2"
 mypy = "^0.942"
 coverage = "^6.3.2"
 isort = "^5.10.1"
+pytest-timeout = "^2.1.0"
 
 [tool.poetry.group.documentation.dependencies]
 Sphinx = "^4.5.0"
 sphinx-rtd-theme = "^1.0.0"
 
 [tool.yapf]
 based_on_style = "pep8"
```

### Comparing `volttron_lib_dnp3_driver-0.1.1a6/src/volttron/driver/interfaces/dnp3/dnp3.py` & `volttron_lib_dnp3_driver-0.1.2rc0/src/volttron/driver/interfaces/dnp3/dnp3.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_dnp3_driver-0.1.1a6/PKG-INFO` & `volttron_lib_dnp3_driver-0.1.2rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-lib-dnp3-driver
-Version: 0.1.1a6
+Version: 0.1.2rc0
 Summary: A minimal implementation of a driver for the VOLTTRON platform.
 Home-page: https://github.com/eclipse-volttron/volttron-lib-dnp3-driver
 License: Apache-2.0
 Author: VOLTTRON Team
 Author-email: volttron@pnnl.gov
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: volttron-lib-dnp3-driver Version: 0.1.1a6 Summary:
+Metadata-Version: 2.1 Name: volttron-lib-dnp3-driver Version: 0.1.2rc0 Summary:
 A minimal implementation of a driver for the VOLTTRON platform. Home-page:
 https://github.com/eclipse-volttron/volttron-lib-dnp3-driver License: Apache-
 2.0 Author: VOLTTRON Team Author-email: volttron@pnnl.gov Requires-Python:
 >=3.10,<4.0 Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: Other
 Audience Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Programming Language ::
```


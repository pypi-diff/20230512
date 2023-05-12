# Comparing `tmp/volttron_lib_dnp3_driver-0.1.1a5.tar.gz` & `tmp/volttron_lib_dnp3_driver-0.1.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_lib_dnp3_driver-0.1.1a5.tar", max compression
+gzip compressed data, was "volttron_lib_dnp3_driver-0.1.1a6.tar", max compression
```

## Comparing `volttron_lib_dnp3_driver-0.1.1a5.tar` & `volttron_lib_dnp3_driver-0.1.1a6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11928 2023-05-11 17:10:28.016525 volttron_lib_dnp3_driver-0.1.1a5/LICENSE
--rw-r--r--   0        0        0    21060 2023-05-11 17:10:28.016525 volttron_lib_dnp3_driver-0.1.1a5/README.md
--rw-r--r--   0        0        0     1579 2023-05-11 17:11:13.220621 volttron_lib_dnp3_driver-0.1.1a5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-11 17:10:28.016525 volttron_lib_dnp3_driver-0.1.1a5/src/volttron/driver/interfaces/dnp3/__init__.py
--rw-r--r--   0        0        0     9189 2023-05-11 17:10:28.016525 volttron_lib_dnp3_driver-0.1.1a5/src/volttron/driver/interfaces/dnp3/dnp3.py
--rw-r--r--   0        0        0    22079 1970-01-01 00:00:00.000000 volttron_lib_dnp3_driver-0.1.1a5/PKG-INFO
+-rw-r--r--   0        0        0    11928 2023-05-12 18:44:09.421295 volttron_lib_dnp3_driver-0.1.1a6/LICENSE
+-rw-r--r--   0        0        0    21060 2023-05-12 18:44:09.421295 volttron_lib_dnp3_driver-0.1.1a6/README.md
+-rw-r--r--   0        0        0     1588 2023-05-12 18:45:03.525768 volttron_lib_dnp3_driver-0.1.1a6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-12 18:44:09.421295 volttron_lib_dnp3_driver-0.1.1a6/src/volttron/driver/interfaces/dnp3/__init__.py
+-rw-r--r--   0        0        0     9189 2023-05-12 18:44:09.421295 volttron_lib_dnp3_driver-0.1.1a6/src/volttron/driver/interfaces/dnp3/dnp3.py
+-rw-r--r--   0        0        0    22079 1970-01-01 00:00:00.000000 volttron_lib_dnp3_driver-0.1.1a6/PKG-INFO
```

### Comparing `volttron_lib_dnp3_driver-0.1.1a5/LICENSE` & `volttron_lib_dnp3_driver-0.1.1a6/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_lib_dnp3_driver-0.1.1a5/README.md` & `volttron_lib_dnp3_driver-0.1.1a6/README.md`

 * *Files identical despite different names*

### Comparing `volttron_lib_dnp3_driver-0.1.1a5/pyproject.toml` & `volttron_lib_dnp3_driver-0.1.1a6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "volttron-lib-dnp3-driver"
-version = "0.1.1a5"
+version = "0.1.1a6"
 description = "A minimal implementation of a driver for the VOLTTRON platform."
 authors = ["VOLTTRON Team <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/eclipse-volttron/volttron-lib-dnp3-driver"
 homepage = "https://github.com/eclipse-volttron/volttron-lib-dnp3-driver"
 keywords = []
@@ -24,15 +24,15 @@
     "Intended Audience :: Other Audience",
     "License :: OSI Approved :: Apache Software License"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 volttron-lib-base-driver = "^0.2.0rc0"
-dnp3-python = "^0.2.3b2"
+dnp3-python = ">=0.2.3b3, <0.3.0"
 
 [tool.poetry.group.dev.dependencies]
 volttron-testing = "^0.4.0rc0"
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
 pytest-env = ">0"
 mock = "^4.0.3"
```

### Comparing `volttron_lib_dnp3_driver-0.1.1a5/src/volttron/driver/interfaces/dnp3/dnp3.py` & `volttron_lib_dnp3_driver-0.1.1a6/src/volttron/driver/interfaces/dnp3/dnp3.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_dnp3_driver-0.1.1a5/PKG-INFO` & `volttron_lib_dnp3_driver-0.1.1a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-lib-dnp3-driver
-Version: 0.1.1a5
+Version: 0.1.1a6
 Summary: A minimal implementation of a driver for the VOLTTRON platform.
 Home-page: https://github.com/eclipse-volttron/volttron-lib-dnp3-driver
 License: Apache-2.0
 Author: VOLTTRON Team
 Author-email: volttron@pnnl.gov
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
@@ -12,15 +12,15 @@
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Dist: dnp3-python (>=0.2.3b2,<0.3.0)
+Requires-Dist: dnp3-python (>=0.2.3b3,<0.3.0)
 Requires-Dist: volttron-lib-base-driver (>=0.2.0rc0,<0.3.0)
 Project-URL: Repository, https://github.com/eclipse-volttron/volttron-lib-dnp3-driver
 Description-Content-Type: text/markdown
 
 # volttron-lib-dnp3-driver
 
 [![Eclipse VOLTTRON™](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/)
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: volttron-lib-dnp3-driver Version: 0.1.1a5 Summary:
+Metadata-Version: 2.1 Name: volttron-lib-dnp3-driver Version: 0.1.1a6 Summary:
 A minimal implementation of a driver for the VOLTTRON platform. Home-page:
 https://github.com/eclipse-volttron/volttron-lib-dnp3-driver License: Apache-
 2.0 Author: VOLTTRON Team Author-email: volttron@pnnl.gov Requires-Python:
 >=3.10,<4.0 Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: Other
 Audience Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3 :: Only Requires-Dist: dnp3-python (>=0.2.3b2,<0.3.0) Requires-
+Python :: 3 :: Only Requires-Dist: dnp3-python (>=0.2.3b3,<0.3.0) Requires-
 Dist: volttron-lib-base-driver (>=0.2.0rc0,<0.3.0) Project-URL: Repository,
 https://github.com/eclipse-volttron/volttron-lib-dnp3-driver Description-
 Content-Type: text/markdown # volttron-lib-dnp3-driver [![Eclipse VOLTTRONâ¢]
 (https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://
 volttron.readthedocs.io/en/latest/) ![Python 3.10](https://img.shields.io/
 badge/python-3.10-blue.svg) ![Python 3.11](https://img.shields.io/badge/python-
 3.11-blue.svg) [![Pytests](https://github.com/eclipse-volttron/volttron-lib-
```


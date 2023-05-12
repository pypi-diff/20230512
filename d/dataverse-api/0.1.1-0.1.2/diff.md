# Comparing `tmp/dataverse_api-0.1.1.tar.gz` & `tmp/dataverse_api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataverse_api-0.1.1.tar", max compression
+gzip compressed data, was "dataverse_api-0.1.2.tar", max compression
```

## Comparing `dataverse_api-0.1.1.tar` & `dataverse_api-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       61 2023-05-12 18:28:06.104392 dataverse_api-0.1.1/dataverse_api/__init__.py
--rw-r--r--   0        0        0    17764 2023-05-12 18:40:36.006430 dataverse_api-0.1.1/dataverse_api/dataverse.py
--rw-r--r--   0        0        0     2428 2023-05-12 18:33:21.684230 dataverse_api-0.1.1/dataverse_api/schema.py
--rw-r--r--   0        0        0     2180 2023-05-12 18:01:04.757130 dataverse_api-0.1.1/dataverse_api/utils.py
--rw-r--r--   0        0        0     1093 2023-05-12 18:09:25.896155 dataverse_api-0.1.1/LICENSE
--rw-r--r--   0        0        0      619 2023-05-12 18:42:39.687748 dataverse_api-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2952 2023-05-12 18:12:08.221665 dataverse_api-0.1.1/README.md
--rw-r--r--   0        0        0     3471 1970-01-01 00:00:00.000000 dataverse_api-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-05-12 18:28:06.104392 dataverse_api-0.1.2/dataverse_api/__init__.py
+-rw-r--r--   0        0        0    17764 2023-05-12 18:40:36.006430 dataverse_api-0.1.2/dataverse_api/dataverse.py
+-rw-r--r--   0        0        0     2428 2023-05-12 18:33:21.684230 dataverse_api-0.1.2/dataverse_api/schema.py
+-rw-r--r--   0        0        0     2180 2023-05-12 18:01:04.757130 dataverse_api-0.1.2/dataverse_api/utils.py
+-rw-r--r--   0        0        0     1093 2023-05-12 18:09:25.896155 dataverse_api-0.1.2/LICENSE
+-rw-r--r--   0        0        0      660 2023-05-12 19:23:48.043242 dataverse_api-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2941 2023-05-12 19:21:52.771293 dataverse_api-0.1.2/README.md
+-rw-r--r--   0        0        0     3460 1970-01-01 00:00:00.000000 dataverse_api-0.1.2/PKG-INFO
```

### Comparing `dataverse_api-0.1.1/dataverse_api/dataverse.py` & `dataverse_api-0.1.2/dataverse_api/dataverse.py`

 * *Files identical despite different names*

### Comparing `dataverse_api-0.1.1/dataverse_api/schema.py` & `dataverse_api-0.1.2/dataverse_api/schema.py`

 * *Files identical despite different names*

### Comparing `dataverse_api-0.1.1/dataverse_api/utils.py` & `dataverse_api-0.1.2/dataverse_api/utils.py`

 * *Files identical despite different names*

### Comparing `dataverse_api-0.1.1/LICENSE` & `dataverse_api-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dataverse_api-0.1.1/pyproject.toml` & `dataverse_api-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataverse-api"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Marcus Risanger <69350948+MarcusRisanger@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 msal = "^1.22.0"
@@ -16,14 +16,16 @@
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 ipykernel = "^6.22.0"
 python-dotenv = "^1.0.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 pre-commit = "^3.3.1"
+coverage = "^7.2.5"
+pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
-profile = 'black'
+profile = 'black'
```

### Comparing `dataverse_api-0.1.1/README.md` & `dataverse_api-0.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 `dataverse-api`
 ================================
 [![Build Status](https://github.com/MarcusRisanger/dataverse-api/workflows/release/badge.svg)](https://github.com/MarcusRisanger/dataverse-api/actions)
-<!-- [![codecov](https://codecov.io/gh/THREE60-Energy/rushmore-tools/branch/main/graph/badge.svg)](https://codecov.io/gh/THREE60-Energy/rushmore-tools) -->
+[![codecov](https://codecov.io/gh/MarcusRisanger/Dataverse-API/branch/main/graph/badge.svg)](https://codecov.io/gh/MarcusRisanger/Dataverse-API)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 The `dataverse-api` package is an abstraction layer developed for allowing simple interaction with Microsoft Dataverse Web API.
 
 Overview
 ================================
 The main goal of this project was to allow for simple upserts and inserts of data into Dataverse tables using simple and ubiquitous data structures, with use of batch requests to avoid frequent hits on the REST API. It is based on Python 3.9 to be compatible with current Python runtimes in Azure Functions.
```

### Comparing `dataverse_api-0.1.1/PKG-INFO` & `dataverse_api-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverse-api
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Marcus Risanger
 Author-email: 69350948+MarcusRisanger@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -15,15 +15,15 @@
 Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 
 `dataverse-api`
 ================================
 [![Build Status](https://github.com/MarcusRisanger/dataverse-api/workflows/release/badge.svg)](https://github.com/MarcusRisanger/dataverse-api/actions)
-<!-- [![codecov](https://codecov.io/gh/THREE60-Energy/rushmore-tools/branch/main/graph/badge.svg)](https://codecov.io/gh/THREE60-Energy/rushmore-tools) -->
+[![codecov](https://codecov.io/gh/MarcusRisanger/Dataverse-API/branch/main/graph/badge.svg)](https://codecov.io/gh/MarcusRisanger/Dataverse-API)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 The `dataverse-api` package is an abstraction layer developed for allowing simple interaction with Microsoft Dataverse Web API.
 
 Overview
 ================================
 The main goal of this project was to allow for simple upserts and inserts of data into Dataverse tables using simple and ubiquitous data structures, with use of batch requests to avoid frequent hits on the REST API. It is based on Python 3.9 to be compatible with current Python runtimes in Azure Functions.
```


# Comparing `tmp/dataverse_api-0.1.0.tar.gz` & `tmp/dataverse_api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataverse_api-0.1.0.tar", max compression
+gzip compressed data, was "dataverse_api-0.1.1.tar", max compression
```

## Comparing `dataverse_api-0.1.0.tar` & `dataverse_api-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       61 2023-05-12 18:28:06.104392 dataverse_api-0.1.0/dataverse_api/__init__.py
--rw-r--r--   0        0        0    17764 2023-05-12 18:01:34.745439 dataverse_api-0.1.0/dataverse_api/dataverse.py
--rw-r--r--   0        0        0     2433 2023-05-12 15:08:30.445229 dataverse_api-0.1.0/dataverse_api/schema.py
--rw-r--r--   0        0        0     2180 2023-05-12 18:01:04.757130 dataverse_api-0.1.0/dataverse_api/utils.py
--rw-r--r--   0        0        0     1093 2023-05-12 18:09:25.896155 dataverse_api-0.1.0/LICENSE
--rw-r--r--   0        0        0      585 2023-05-12 18:29:58.894000 dataverse_api-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2952 2023-05-12 18:12:08.221665 dataverse_api-0.1.0/README.md
--rw-r--r--   0        0        0     3471 1970-01-01 00:00:00.000000 dataverse_api-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-05-12 18:28:06.104392 dataverse_api-0.1.1/dataverse_api/__init__.py
+-rw-r--r--   0        0        0    17764 2023-05-12 18:40:36.006430 dataverse_api-0.1.1/dataverse_api/dataverse.py
+-rw-r--r--   0        0        0     2428 2023-05-12 18:33:21.684230 dataverse_api-0.1.1/dataverse_api/schema.py
+-rw-r--r--   0        0        0     2180 2023-05-12 18:01:04.757130 dataverse_api-0.1.1/dataverse_api/utils.py
+-rw-r--r--   0        0        0     1093 2023-05-12 18:09:25.896155 dataverse_api-0.1.1/LICENSE
+-rw-r--r--   0        0        0      619 2023-05-12 18:42:39.687748 dataverse_api-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2952 2023-05-12 18:12:08.221665 dataverse_api-0.1.1/README.md
+-rw-r--r--   0        0        0     3471 1970-01-01 00:00:00.000000 dataverse_api-0.1.1/PKG-INFO
```

### Comparing `dataverse_api-0.1.0/dataverse_api/dataverse.py` & `dataverse_api-0.1.1/dataverse_api/dataverse.py`

 * *Files identical despite different names*

### Comparing `dataverse_api-0.1.0/dataverse_api/schema.py` & `dataverse_api-0.1.1/dataverse_api/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import xml.etree.ElementTree as ET
 from dataclasses import dataclass
-from typing import Any, Dict, List, Set
+from typing import Dict, List, Set
 from urllib.parse import urljoin
 
 import requests
 from msal_requests_auth.auth import ClientCredentialAuth
 
 from dataverse_api.utils import DataverseError
```

### Comparing `dataverse_api-0.1.0/dataverse_api/utils.py` & `dataverse_api-0.1.1/dataverse_api/utils.py`

 * *Files identical despite different names*

### Comparing `dataverse_api-0.1.0/LICENSE` & `dataverse_api-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dataverse_api-0.1.0/pyproject.toml` & `dataverse_api-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataverse-api"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Marcus Risanger <69350948+MarcusRisanger@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 msal = "^1.22.0"
@@ -20,7 +20,10 @@
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 pre-commit = "^3.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.isort]
+profile = 'black'
```

### Comparing `dataverse_api-0.1.0/README.md` & `dataverse_api-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dataverse_api-0.1.0/PKG-INFO` & `dataverse_api-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverse-api
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Marcus Risanger
 Author-email: 69350948+MarcusRisanger@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


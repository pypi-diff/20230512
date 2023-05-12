# Comparing `tmp/virtool_core-4.8.0.tar.gz` & `tmp/virtool_core-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virtool_core-4.8.0.tar", max compression
+gzip compressed data, was "virtool_core-4.9.0.tar", max compression
```

## Comparing `virtool_core-4.8.0.tar` & `virtool_core-4.9.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1077 2023-03-21 21:09:43.161680 virtool_core-4.8.0/LICENSE
--rw-r--r--   0        0        0     2074 2023-03-21 21:09:43.161680 virtool_core-4.8.0/README.md
--rw-r--r--   0        0        0     1017 2023-03-21 21:09:56.481871 virtool_core-4.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/__init__.py
--rw-r--r--   0        0        0     7013 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/bio.py
--rw-r--r--   0        0        0       79 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/errors.py
--rw-r--r--   0        0        0      608 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/logging.py
--rw-r--r--   0        0        0      384 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/models/__init__.py
--rw-r--r--   0        0        0     1194 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/models/account.py
--rw-r--r--   0        0        0      438 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/models/administrator.py
--rw-r--r--   0        0        0     1425 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/models/analysis.py
--rw-r--r--   0        0        0      176 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/models/auth.py
--rw-r--r--   0        0        0      264 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/models/basemodel.py
--rw-r--r--   0        0        0      417 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/models/blast.py
--rw-r--r--   0        0        0     1452 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/models/enums.py
--rw-r--r--   0        0        0      565 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/models/genbank.py
--rw-r--r--   0        0        0      960 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/models/group.py
--rw-r--r--   0        0        0     1607 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/models/history.py
--rw-r--r--   0        0        0     1638 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/models/hmm.py
--rw-r--r--   0        0        0     1173 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/models/index.py
--rw-r--r--   0        0        0      359 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/models/instancemessage.py
--rw-r--r--   0        0        0     1363 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/models/job.py
--rw-r--r--   0        0        0      389 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/models/label.py
--rw-r--r--   0        0        0     1909 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/models/otu.py
--rw-r--r--   0        0        0     1105 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/models/project.py
--rw-r--r--   0        0        0     2550 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/models/reference.py
--rw-r--r--   0        0        0     4334 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/models/roles.py
--rw-r--r--   0        0        0     1896 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/models/samples.py
--rw-r--r--   0        0        0      179 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/models/searchresult.py
--rw-r--r--   0        0        0      435 2023-03-21 21:09:43.369683 virtool_core-4.8.0/virtool_core/models/session.py
--rw-r--r--   0        0        0      481 2023-03-21 21:09:43.373683 virtool_core-4.8.0/virtool_core/models/settings.py
--rw-r--r--   0        0        0     1412 2023-03-21 21:09:43.373683 virtool_core-4.8.0/virtool_core/models/subtraction.py
--rw-r--r--   0        0        0      451 2023-03-21 21:09:43.373683 virtool_core-4.8.0/virtool_core/models/task.py
--rw-r--r--   0        0        0      656 2023-03-21 21:09:43.373683 virtool_core-4.8.0/virtool_core/models/upload.py
--rw-r--r--   0        0        0      924 2023-03-21 21:09:43.373683 virtool_core-4.8.0/virtool_core/models/user.py
--rw-r--r--   0        0        0      881 2023-03-21 21:09:43.373683 virtool_core-4.8.0/virtool_core/models/validators.py
--rw-r--r--   0        0        0     1895 2023-03-21 21:09:43.373683 virtool_core-4.8.0/virtool_core/mongo.py
--rw-r--r--   0        0        0     3285 2023-03-21 21:09:43.373683 virtool_core-4.8.0/virtool_core/redis.py
--rw-r--r--   0        0        0     9637 2023-03-21 21:09:43.373683 virtool_core-4.8.0/virtool_core/utils.py
--rw-r--r--   0        0        0     3201 1970-01-01 00:00:00.000000 virtool_core-4.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-03-21 21:13:58.305268 virtool_core-4.9.0/LICENSE
+-rw-r--r--   0        0        0     2074 2023-03-21 21:13:58.305268 virtool_core-4.9.0/README.md
+-rw-r--r--   0        0        0     1017 2023-03-21 21:14:09.597967 virtool_core-4.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-21 21:13:58.513280 virtool_core-4.9.0/virtool_core/__init__.py
+-rw-r--r--   0        0        0     7013 2023-03-21 21:13:58.513280 virtool_core-4.9.0/virtool_core/bio.py
+-rw-r--r--   0        0        0       79 2023-03-21 21:13:58.513280 virtool_core-4.9.0/virtool_core/errors.py
+-rw-r--r--   0        0        0      608 2023-03-21 21:13:58.513280 virtool_core-4.9.0/virtool_core/logging.py
+-rw-r--r--   0        0        0      384 2023-03-21 21:13:58.513280 virtool_core-4.9.0/virtool_core/models/__init__.py
+-rw-r--r--   0        0        0     1194 2023-03-21 21:13:58.513280 virtool_core-4.9.0/virtool_core/models/account.py
+-rw-r--r--   0        0        0      438 2023-03-21 21:13:58.513280 virtool_core-4.9.0/virtool_core/models/administrator.py
+-rw-r--r--   0        0        0     1425 2023-03-21 21:13:58.513280 virtool_core-4.9.0/virtool_core/models/analysis.py
+-rw-r--r--   0        0        0      176 2023-03-21 21:13:58.513280 virtool_core-4.9.0/virtool_core/models/auth.py
+-rw-r--r--   0        0        0      264 2023-03-21 21:13:58.513280 virtool_core-4.9.0/virtool_core/models/basemodel.py
+-rw-r--r--   0        0        0      417 2023-03-21 21:13:58.513280 virtool_core-4.9.0/virtool_core/models/blast.py
+-rw-r--r--   0        0        0     1452 2023-03-21 21:13:58.513280 virtool_core-4.9.0/virtool_core/models/enums.py
+-rw-r--r--   0        0        0      565 2023-03-21 21:13:58.513280 virtool_core-4.9.0/virtool_core/models/genbank.py
+-rw-r--r--   0        0        0      960 2023-03-21 21:13:58.513280 virtool_core-4.9.0/virtool_core/models/group.py
+-rw-r--r--   0        0        0     1607 2023-03-21 21:13:58.517281 virtool_core-4.9.0/virtool_core/models/history.py
+-rw-r--r--   0        0        0     1638 2023-03-21 21:13:58.517281 virtool_core-4.9.0/virtool_core/models/hmm.py
+-rw-r--r--   0        0        0     1173 2023-03-21 21:13:58.517281 virtool_core-4.9.0/virtool_core/models/index.py
+-rw-r--r--   0        0        0      359 2023-03-21 21:13:58.517281 virtool_core-4.9.0/virtool_core/models/instancemessage.py
+-rw-r--r--   0        0        0     1363 2023-03-21 21:13:58.517281 virtool_core-4.9.0/virtool_core/models/job.py
+-rw-r--r--   0        0        0      389 2023-03-21 21:13:58.517281 virtool_core-4.9.0/virtool_core/models/label.py
+-rw-r--r--   0        0        0     1909 2023-03-21 21:13:58.517281 virtool_core-4.9.0/virtool_core/models/otu.py
+-rw-r--r--   0        0        0     1105 2023-03-21 21:13:58.517281 virtool_core-4.9.0/virtool_core/models/project.py
+-rw-r--r--   0        0        0     2550 2023-03-21 21:13:58.517281 virtool_core-4.9.0/virtool_core/models/reference.py
+-rw-r--r--   0        0        0     4334 2023-03-21 21:13:58.517281 virtool_core-4.9.0/virtool_core/models/roles.py
+-rw-r--r--   0        0        0     1973 2023-03-21 21:13:58.517281 virtool_core-4.9.0/virtool_core/models/samples.py
+-rw-r--r--   0        0        0      179 2023-03-21 21:13:58.517281 virtool_core-4.9.0/virtool_core/models/searchresult.py
+-rw-r--r--   0        0        0      435 2023-03-21 21:13:58.517281 virtool_core-4.9.0/virtool_core/models/session.py
+-rw-r--r--   0        0        0      481 2023-03-21 21:13:58.517281 virtool_core-4.9.0/virtool_core/models/settings.py
+-rw-r--r--   0        0        0     1412 2023-03-21 21:13:58.517281 virtool_core-4.9.0/virtool_core/models/subtraction.py
+-rw-r--r--   0        0        0      451 2023-03-21 21:13:58.517281 virtool_core-4.9.0/virtool_core/models/task.py
+-rw-r--r--   0        0        0      656 2023-03-21 21:13:58.517281 virtool_core-4.9.0/virtool_core/models/upload.py
+-rw-r--r--   0        0        0      924 2023-03-21 21:13:58.517281 virtool_core-4.9.0/virtool_core/models/user.py
+-rw-r--r--   0        0        0      881 2023-03-21 21:13:58.517281 virtool_core-4.9.0/virtool_core/models/validators.py
+-rw-r--r--   0        0        0     1895 2023-03-21 21:13:58.517281 virtool_core-4.9.0/virtool_core/mongo.py
+-rw-r--r--   0        0        0     3285 2023-03-21 21:13:58.517281 virtool_core-4.9.0/virtool_core/redis.py
+-rw-r--r--   0        0        0     9637 2023-03-21 21:13:58.517281 virtool_core-4.9.0/virtool_core/utils.py
+-rw-r--r--   0        0        0     3201 1970-01-01 00:00:00.000000 virtool_core-4.9.0/PKG-INFO
```

### Comparing `virtool_core-4.8.0/LICENSE` & `virtool_core-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `virtool_core-4.8.0/README.md` & `virtool_core-4.9.0/README.md`

 * *Files identical despite different names*

### Comparing `virtool_core-4.8.0/pyproject.toml` & `virtool_core-4.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "virtool-core"
-version = "4.8.0"
+version = "4.9.0"
 description = "Core utilities for Virtool."
 authors = ["Ian Boyes", "Blake Smith"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/virtool/virtool-core"
 classifiers = [
     "Topic :: Software Development :: Libraries",
```

### Comparing `virtool_core-4.8.0/virtool_core/bio.py` & `virtool_core-4.9.0/virtool_core/bio.py`

 * *Files identical despite different names*

### Comparing `virtool_core-4.8.0/virtool_core/logging.py` & `virtool_core-4.9.0/virtool_core/logging.py`

 * *Files identical despite different names*

### Comparing `virtool_core-4.8.0/virtool_core/models/account.py` & `virtool_core-4.9.0/virtool_core/models/account.py`

 * *Files identical despite different names*

### Comparing `virtool_core-4.8.0/virtool_core/models/analysis.py` & `virtool_core-4.9.0/virtool_core/models/analysis.py`

 * *Files identical despite different names*

### Comparing `virtool_core-4.8.0/virtool_core/models/enums.py` & `virtool_core-4.9.0/virtool_core/models/enums.py`

 * *Files identical despite different names*

### Comparing `virtool_core-4.8.0/virtool_core/models/genbank.py` & `virtool_core-4.9.0/virtool_core/models/genbank.py`

 * *Files identical despite different names*

### Comparing `virtool_core-4.8.0/virtool_core/models/group.py` & `virtool_core-4.9.0/virtool_core/models/group.py`

 * *Files identical despite different names*

### Comparing `virtool_core-4.8.0/virtool_core/models/history.py` & `virtool_core-4.9.0/virtool_core/models/history.py`

 * *Files identical despite different names*

### Comparing `virtool_core-4.8.0/virtool_core/models/hmm.py` & `virtool_core-4.9.0/virtool_core/models/hmm.py`

 * *Files identical despite different names*

### Comparing `virtool_core-4.8.0/virtool_core/models/index.py` & `virtool_core-4.9.0/virtool_core/models/index.py`

 * *Files identical despite different names*

### Comparing `virtool_core-4.8.0/virtool_core/models/job.py` & `virtool_core-4.9.0/virtool_core/models/job.py`

 * *Files identical despite different names*

### Comparing `virtool_core-4.8.0/virtool_core/models/otu.py` & `virtool_core-4.9.0/virtool_core/models/otu.py`

 * *Files identical despite different names*

### Comparing `virtool_core-4.8.0/virtool_core/models/project.py` & `virtool_core-4.9.0/virtool_core/models/project.py`

 * *Files identical despite different names*

### Comparing `virtool_core-4.8.0/virtool_core/models/reference.py` & `virtool_core-4.9.0/virtool_core/models/reference.py`

 * *Files identical despite different names*

### Comparing `virtool_core-4.8.0/virtool_core/models/roles.py` & `virtool_core-4.9.0/virtool_core/models/roles.py`

 * *Files identical despite different names*

### Comparing `virtool_core-4.8.0/virtool_core/models/samples.py` & `virtool_core-4.9.0/virtool_core/models/samples.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from datetime import datetime
 from typing import List, Union, TYPE_CHECKING, Optional
 
 from virtool_core.models.basemodel import BaseModel
 from virtool_core.models.enums import LibraryType
+from virtool_core.models.job import JobMinimal
 from virtool_core.models.label import LabelNested
 from virtool_core.models.searchresult import SearchResult
 from virtool_core.models.upload import Upload
 from virtool_core.models.user import UserNested
 
 if TYPE_CHECKING:
     from virtool_core.models.subtraction import SubtractionNested
@@ -22,14 +23,15 @@
     name: str
 
 
 class SampleMinimal(SampleNested):
     created_at: datetime
     host: str
     isolate: str
+    job: Optional[JobMinimal]
     labels: List[LabelNested]
     library_type: LibraryType
     notes: str
     nuvs: Union[bool, str]
     pathoscope: Union[bool, str]
     ready: bool
     user: UserNested
```

### Comparing `virtool_core-4.8.0/virtool_core/models/subtraction.py` & `virtool_core-4.9.0/virtool_core/models/subtraction.py`

 * *Files identical despite different names*

### Comparing `virtool_core-4.8.0/virtool_core/models/upload.py` & `virtool_core-4.9.0/virtool_core/models/upload.py`

 * *Files identical despite different names*

### Comparing `virtool_core-4.8.0/virtool_core/models/user.py` & `virtool_core-4.9.0/virtool_core/models/user.py`

 * *Files identical despite different names*

### Comparing `virtool_core-4.8.0/virtool_core/models/validators.py` & `virtool_core-4.9.0/virtool_core/models/validators.py`

 * *Files identical despite different names*

### Comparing `virtool_core-4.8.0/virtool_core/mongo.py` & `virtool_core-4.9.0/virtool_core/mongo.py`

 * *Files identical despite different names*

### Comparing `virtool_core-4.8.0/virtool_core/redis.py` & `virtool_core-4.9.0/virtool_core/redis.py`

 * *Files identical despite different names*

### Comparing `virtool_core-4.8.0/virtool_core/utils.py` & `virtool_core-4.9.0/virtool_core/utils.py`

 * *Files identical despite different names*

### Comparing `virtool_core-4.8.0/PKG-INFO` & `virtool_core-4.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virtool-core
-Version: 4.8.0
+Version: 4.9.0
 Summary: Core utilities for Virtool.
 Home-page: https://github.com/virtool/virtool-core
 License: MIT
 Author: Ian Boyes
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


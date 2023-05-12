# Comparing `tmp/steadfast-1.0.0.tar.gz` & `tmp/steadfast-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steadfast-1.0.0.tar", last modified: Wed May 10 15:59:54 2023, max compression
+gzip compressed data, was "steadfast-1.0.1.tar", last modified: Fri May 12 16:38:10 2023, max compression
```

## Comparing `steadfast-1.0.0.tar` & `steadfast-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-10 15:59:54.488788 steadfast-1.0.0/
--rw-r--r--   0 work       (505) staff       (20)       19 2022-03-13 22:55:00.000000 steadfast-1.0.0/AUTHORS.txt
--rw-r--r--   0 work       (505) staff       (20)     1525 2023-05-10 12:24:52.000000 steadfast-1.0.0/LICENSE.txt
--rw-r--r--   0 work       (505) staff       (20)       38 2022-11-21 19:45:36.000000 steadfast-1.0.0/MANIFEST.in
--rw-r--r--   0 work       (505) staff       (20)      871 2023-05-10 15:59:54.488935 steadfast-1.0.0/PKG-INFO
--rw-r--r--   0 work       (505) staff       (20)      216 2023-05-10 15:59:49.000000 steadfast-1.0.0/README.md
--rw-r--r--   0 work       (505) staff       (20)      100 2021-02-16 17:38:13.000000 steadfast-1.0.0/pyproject.toml
--rw-r--r--   0 work       (505) staff       (20)      802 2023-05-10 15:59:54.490122 steadfast-1.0.0/setup.cfg
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-10 15:59:54.332134 steadfast-1.0.0/src/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-10 15:59:54.486944 steadfast-1.0.0/src/steadfast/
--rw-r--r--   0 work       (505) staff       (20)      263 2021-07-23 17:34:38.000000 steadfast-1.0.0/src/steadfast/__init__.py
--rw-r--r--   0 work       (505) staff       (20)    17873 2022-10-31 12:11:03.000000 steadfast-1.0.0/src/steadfast/archive.py
--rw-r--r--   0 work       (505) staff       (20)     1773 2021-07-18 17:44:45.000000 steadfast-1.0.0/src/steadfast/common.py
--rw-r--r--   0 work       (505) staff       (20)     6204 2021-07-24 09:21:30.000000 steadfast-1.0.0/src/steadfast/core.py
--rw-r--r--   0 work       (505) staff       (20)     3987 2021-08-09 10:21:09.000000 steadfast-1.0.0/src/steadfast/decorators.py
--rw-r--r--   0 work       (505) staff       (20)     2366 2021-08-07 20:11:03.000000 steadfast-1.0.0/src/steadfast/identifiers.py
--rw-r--r--   0 work       (505) staff       (20)     7135 2021-07-25 22:15:59.000000 steadfast-1.0.0/src/steadfast/inspect.py
--rw-r--r--   0 work       (505) staff       (20)    18730 2022-11-07 13:53:06.000000 steadfast-1.0.0/src/steadfast/operators.py
--rw-r--r--   0 work       (505) staff       (20)     1503 2020-10-01 08:37:37.000000 steadfast-1.0.0/src/steadfast/priority_queue.py
--rw-r--r--   0 work       (505) staff       (20)      650 2021-07-14 15:28:38.000000 steadfast-1.0.0/src/steadfast/test_core.py
--rw-r--r--   0 work       (505) staff       (20)     4047 2022-11-07 13:52:24.000000 steadfast-1.0.0/src/steadfast/test_example.py
--rw-r--r--   0 work       (505) staff       (20)     2456 2021-07-19 16:04:11.000000 steadfast-1.0.0/src/steadfast/toposort.py
--rw-r--r--   0 work       (505) staff       (20)     2065 2021-08-09 09:47:11.000000 steadfast-1.0.0/src/steadfast/types.py
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-10 15:59:54.488536 steadfast-1.0.0/src/steadfast.egg-info/
--rw-r--r--   0 work       (505) staff       (20)      871 2023-05-10 15:59:54.000000 steadfast-1.0.0/src/steadfast.egg-info/PKG-INFO
--rw-r--r--   0 work       (505) staff       (20)      598 2023-05-10 15:59:54.000000 steadfast-1.0.0/src/steadfast.egg-info/SOURCES.txt
--rw-r--r--   0 work       (505) staff       (20)        1 2023-05-10 15:59:54.000000 steadfast-1.0.0/src/steadfast.egg-info/dependency_links.txt
--rw-r--r--   0 work       (505) staff       (20)        1 2023-05-10 15:59:54.000000 steadfast-1.0.0/src/steadfast.egg-info/not-zip-safe
--rw-r--r--   0 work       (505) staff       (20)       10 2023-05-10 15:59:54.000000 steadfast-1.0.0/src/steadfast.egg-info/top_level.txt
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:38:10.045484 steadfast-1.0.1/
+-rw-r--r--   0 work       (505) staff       (20)       19 2022-03-13 22:55:00.000000 steadfast-1.0.1/AUTHORS.txt
+-rw-r--r--   0 work       (505) staff       (20)     1525 2023-05-10 12:24:52.000000 steadfast-1.0.1/LICENSE.txt
+-rw-r--r--   0 work       (505) staff       (20)       38 2022-11-21 19:45:36.000000 steadfast-1.0.1/MANIFEST.in
+-rw-r--r--   0 work       (505) staff       (20)      871 2023-05-12 16:38:10.045688 steadfast-1.0.1/PKG-INFO
+-rw-r--r--   0 work       (505) staff       (20)      216 2023-05-10 15:59:49.000000 steadfast-1.0.1/README.md
+-rw-r--r--   0 work       (505) staff       (20)      100 2021-02-16 17:38:13.000000 steadfast-1.0.1/pyproject.toml
+-rw-r--r--   0 work       (505) staff       (20)      802 2023-05-12 16:38:10.047665 steadfast-1.0.1/setup.cfg
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:38:09.882697 steadfast-1.0.1/src/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:38:10.035198 steadfast-1.0.1/src/steadfast/
+-rw-r--r--   0 work       (505) staff       (20)      263 2021-07-23 17:34:38.000000 steadfast-1.0.1/src/steadfast/__init__.py
+-rw-r--r--   0 work       (505) staff       (20)    17873 2022-10-31 12:11:03.000000 steadfast-1.0.1/src/steadfast/archive.py
+-rw-r--r--   0 work       (505) staff       (20)     1773 2021-07-18 17:44:45.000000 steadfast-1.0.1/src/steadfast/common.py
+-rw-r--r--   0 work       (505) staff       (20)     6204 2021-07-24 09:21:30.000000 steadfast-1.0.1/src/steadfast/core.py
+-rw-r--r--   0 work       (505) staff       (20)     3987 2021-08-09 10:21:09.000000 steadfast-1.0.1/src/steadfast/decorators.py
+-rw-r--r--   0 work       (505) staff       (20)     2366 2021-08-07 20:11:03.000000 steadfast-1.0.1/src/steadfast/identifiers.py
+-rw-r--r--   0 work       (505) staff       (20)     7135 2021-07-25 22:15:59.000000 steadfast-1.0.1/src/steadfast/inspect.py
+-rw-r--r--   0 work       (505) staff       (20)    18734 2023-05-12 14:36:17.000000 steadfast-1.0.1/src/steadfast/operators.py
+-rw-r--r--   0 work       (505) staff       (20)     1503 2020-10-01 08:37:37.000000 steadfast-1.0.1/src/steadfast/priority_queue.py
+-rw-r--r--   0 work       (505) staff       (20)      650 2021-07-14 15:28:38.000000 steadfast-1.0.1/src/steadfast/test_core.py
+-rw-r--r--   0 work       (505) staff       (20)     4047 2022-11-07 13:52:24.000000 steadfast-1.0.1/src/steadfast/test_example.py
+-rw-r--r--   0 work       (505) staff       (20)     2456 2021-07-19 16:04:11.000000 steadfast-1.0.1/src/steadfast/toposort.py
+-rw-r--r--   0 work       (505) staff       (20)     2065 2021-08-09 09:47:11.000000 steadfast-1.0.1/src/steadfast/types.py
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:38:10.045033 steadfast-1.0.1/src/steadfast.egg-info/
+-rw-r--r--   0 work       (505) staff       (20)      871 2023-05-12 16:38:09.000000 steadfast-1.0.1/src/steadfast.egg-info/PKG-INFO
+-rw-r--r--   0 work       (505) staff       (20)      598 2023-05-12 16:38:09.000000 steadfast-1.0.1/src/steadfast.egg-info/SOURCES.txt
+-rw-r--r--   0 work       (505) staff       (20)        1 2023-05-12 16:38:09.000000 steadfast-1.0.1/src/steadfast.egg-info/dependency_links.txt
+-rw-r--r--   0 work       (505) staff       (20)        1 2023-05-12 16:38:09.000000 steadfast-1.0.1/src/steadfast.egg-info/not-zip-safe
+-rw-r--r--   0 work       (505) staff       (20)       10 2023-05-12 16:38:09.000000 steadfast-1.0.1/src/steadfast.egg-info/top_level.txt
```

### Comparing `steadfast-1.0.0/LICENSE.txt` & `steadfast-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `steadfast-1.0.0/PKG-INFO` & `steadfast-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steadfast
-Version: 1.0.0
+Version: 1.0.1
 Summary: Utilities for object serialization.
 Home-page: https://github.com/high-dimensional/steadfast
 Author: High Dimensional Neurology Group, UCL
 Author-email: pypi@highdimensional.net
 License: BSD-3-Clause
 Platform: any
 Classifier: Framework :: Django
```

### Comparing `steadfast-1.0.0/setup.cfg` & `steadfast-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = steadfast
-version = 1.0.0
+version = 1.0.1
 url = https://github.com/high-dimensional/steadfast
 author = High Dimensional Neurology Group, UCL
 author_email = pypi@highdimensional.net
 description = Utilities for object serialization.
 long_description = file:README.md
 long_description_content_type = text/markdown
 license = BSD-3-Clause
```

### Comparing `steadfast-1.0.0/src/steadfast/archive.py` & `steadfast-1.0.1/src/steadfast/archive.py`

 * *Files identical despite different names*

### Comparing `steadfast-1.0.0/src/steadfast/common.py` & `steadfast-1.0.1/src/steadfast/common.py`

 * *Files identical despite different names*

### Comparing `steadfast-1.0.0/src/steadfast/core.py` & `steadfast-1.0.1/src/steadfast/core.py`

 * *Files identical despite different names*

### Comparing `steadfast-1.0.0/src/steadfast/decorators.py` & `steadfast-1.0.1/src/steadfast/decorators.py`

 * *Files identical despite different names*

### Comparing `steadfast-1.0.0/src/steadfast/identifiers.py` & `steadfast-1.0.1/src/steadfast/identifiers.py`

 * *Files identical despite different names*

### Comparing `steadfast-1.0.0/src/steadfast/inspect.py` & `steadfast-1.0.1/src/steadfast/inspect.py`

 * *Files identical despite different names*

### Comparing `steadfast-1.0.0/src/steadfast/operators.py` & `steadfast-1.0.1/src/steadfast/operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 import typing as tp
 from types import SimpleNamespace, GeneratorType
-from collections import Iterator
+from collections.abc import Iterator
 
 from .core import *
 from .common import *
 
 # from .types import TypeRegistry
 # from .identifiers import dot_identifier_for_type
```

### Comparing `steadfast-1.0.0/src/steadfast/priority_queue.py` & `steadfast-1.0.1/src/steadfast/priority_queue.py`

 * *Files identical despite different names*

### Comparing `steadfast-1.0.0/src/steadfast/test_core.py` & `steadfast-1.0.1/src/steadfast/test_core.py`

 * *Files identical despite different names*

### Comparing `steadfast-1.0.0/src/steadfast/test_example.py` & `steadfast-1.0.1/src/steadfast/test_example.py`

 * *Files identical despite different names*

### Comparing `steadfast-1.0.0/src/steadfast/toposort.py` & `steadfast-1.0.1/src/steadfast/toposort.py`

 * *Files identical despite different names*

### Comparing `steadfast-1.0.0/src/steadfast/types.py` & `steadfast-1.0.1/src/steadfast/types.py`

 * *Files identical despite different names*

### Comparing `steadfast-1.0.0/src/steadfast.egg-info/PKG-INFO` & `steadfast-1.0.1/src/steadfast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steadfast
-Version: 1.0.0
+Version: 1.0.1
 Summary: Utilities for object serialization.
 Home-page: https://github.com/high-dimensional/steadfast
 Author: High Dimensional Neurology Group, UCL
 Author-email: pypi@highdimensional.net
 License: BSD-3-Clause
 Platform: any
 Classifier: Framework :: Django
```

### Comparing `steadfast-1.0.0/src/steadfast.egg-info/SOURCES.txt` & `steadfast-1.0.1/src/steadfast.egg-info/SOURCES.txt`

 * *Files identical despite different names*


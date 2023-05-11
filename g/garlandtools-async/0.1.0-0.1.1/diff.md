# Comparing `tmp/garlandtools_async-0.1.0.tar.gz` & `tmp/garlandtools_async-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garlandtools_async-0.1.0.tar", max compression
+gzip compressed data, was "garlandtools_async-0.1.1.tar", max compression
```

## Comparing `garlandtools_async-0.1.0.tar` & `garlandtools_async-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1069 2023-05-11 19:45:32.808905 garlandtools_async-0.1.0/LICENSE
--rw-r--r--   0        0        0      571 2023-05-11 19:45:32.808905 garlandtools_async-0.1.0/README.md
--rw-r--r--   0        0        0       62 2023-05-11 19:45:32.808905 garlandtools_async-0.1.0/garlandtools/__init__.py
--rw-r--r--   0        0        0     1722 2023-05-11 19:45:32.808905 garlandtools_async-0.1.0/garlandtools/client.py
--rw-r--r--   0        0        0      112 2023-05-11 19:45:32.808905 garlandtools_async-0.1.0/garlandtools/models/__init__.py
--rw-r--r--   0        0        0      152 2023-05-11 19:45:32.808905 garlandtools_async-0.1.0/garlandtools/models/lang.py
--rw-r--r--   0        0        0       66 2023-05-11 19:45:32.808905 garlandtools_async-0.1.0/garlandtools/models/partials/__init__.py
--rw-r--r--   0        0        0      588 2023-05-11 19:45:32.808905 garlandtools_async-0.1.0/garlandtools/models/partials/item_partial.py
--rw-r--r--   0        0        0      309 2023-05-11 19:45:32.808905 garlandtools_async-0.1.0/garlandtools/models/partials/partial.py
--rw-r--r--   0        0        0      328 2023-05-11 19:45:32.808905 garlandtools_async-0.1.0/garlandtools/models/type.py
--rw-r--r--   0        0        0      593 2023-05-11 19:45:32.808905 garlandtools_async-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 garlandtools_async-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 22:05:50.630530 garlandtools_async-0.1.1/LICENSE
+-rw-r--r--   0        0        0      571 2023-05-11 22:05:50.630530 garlandtools_async-0.1.1/README.md
+-rw-r--r--   0        0        0       62 2023-05-11 22:05:50.630530 garlandtools_async-0.1.1/garlandtools/__init__.py
+-rw-r--r--   0        0        0     1722 2023-05-11 22:05:50.630530 garlandtools_async-0.1.1/garlandtools/client.py
+-rw-r--r--   0        0        0      112 2023-05-11 22:05:50.630530 garlandtools_async-0.1.1/garlandtools/models/__init__.py
+-rw-r--r--   0        0        0      152 2023-05-11 22:05:50.630530 garlandtools_async-0.1.1/garlandtools/models/lang.py
+-rw-r--r--   0        0        0       66 2023-05-11 22:05:50.630530 garlandtools_async-0.1.1/garlandtools/models/partials/__init__.py
+-rw-r--r--   0        0        0      588 2023-05-11 22:05:50.630530 garlandtools_async-0.1.1/garlandtools/models/partials/item_partial.py
+-rw-r--r--   0        0        0      309 2023-05-11 22:05:50.630530 garlandtools_async-0.1.1/garlandtools/models/partials/partial.py
+-rw-r--r--   0        0        0      328 2023-05-11 22:05:50.630530 garlandtools_async-0.1.1/garlandtools/models/type.py
+-rw-r--r--   0        0        0      593 2023-05-11 22:05:50.630530 garlandtools_async-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 garlandtools_async-0.1.1/PKG-INFO
```

### Comparing `garlandtools_async-0.1.0/LICENSE` & `garlandtools_async-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `garlandtools_async-0.1.0/README.md` & `garlandtools_async-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `garlandtools_async-0.1.0/garlandtools/client.py` & `garlandtools_async-0.1.1/garlandtools/client.py`

 * *Files identical despite different names*

### Comparing `garlandtools_async-0.1.0/garlandtools/models/partials/item_partial.py` & `garlandtools_async-0.1.1/garlandtools/models/partials/item_partial.py`

 * *Files identical despite different names*

### Comparing `garlandtools_async-0.1.0/pyproject.toml` & `garlandtools_async-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "garlandtools-async"
-version = "0.1.0"
+version = "0.1.1"
 description = "A async python wrapper for the https://garlandtools.org/ API"
 authors = ["Abigail Howe <abby@abigailhowe.org>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "garlandtools"}]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 aiohttp = "^3.8.4"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.3.1"
 isort = "^5.12.0"
 mypy = "^1.2.0"
```

### Comparing `garlandtools_async-0.1.0/PKG-INFO` & `garlandtools_async-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: garlandtools-async
-Version: 0.1.0
+Version: 0.1.1
 Summary: A async python wrapper for the https://garlandtools.org/ API
 License: MIT
 Author: Abigail Howe
 Author-email: abby@abigailhowe.org
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Description-Content-Type: text/markdown
 
 # garlandtools-py
 
 Work in progress project to provide a async wrapper around the Garland Tools API as detailed here:
```


# Comparing `tmp/boxfs-0.1.1.tar.gz` & `tmp/boxfs-0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boxfs-0.1.1.tar", max compression
+gzip compressed data, was "boxfs-0.1a1.tar", max compression
```

## Comparing `boxfs-0.1.1.tar` & `boxfs-0.1a1.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1109 2023-05-11 19:02:55.323065 boxfs-0.1.1/LICENSE
--rw-r--r--   0        0        0     1535 2023-05-12 16:03:42.396238 boxfs-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1920 2023-05-12 15:59:55.694514 boxfs-0.1.1/README.md
--rw-r--r--   0        0        0       34 2023-05-12 15:59:55.744647 boxfs-0.1.1/src/boxfs/__init__.py
--rw-r--r--   0        0        0    17437 2023-05-12 15:59:55.765537 boxfs-0.1.1/src/boxfs/boxfs.py
--rw-r--r--   0        0        0     2781 1970-01-01 00:00:00.000000 boxfs-0.1.1/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 boxfs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1109 2023-05-11 19:02:55.323065 boxfs-0.1a1/LICENSE
+-rw-r--r--   0        0        0     1105 2023-05-12 15:02:00.753230 boxfs-0.1a1/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-05-12 13:46:02.149383 boxfs-0.1a1/src/boxfs/__init__.py
+-rw-r--r--   0        0        0    17437 2023-05-12 14:00:34.245785 boxfs-0.1a1/src/boxfs/boxfs.py
+-rw-r--r--   0        0        0      807 1970-01-01 00:00:00.000000 boxfs-0.1a1/setup.py
+-rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 boxfs-0.1a1/PKG-INFO
```

### Comparing `boxfs-0.1.1/LICENSE` & `boxfs-0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `boxfs-0.1.1/pyproject.toml` & `boxfs-0.1a1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -2,35 +2,22 @@
 requires = ["poetry_core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [project]
 name = "boxfs"
 dynamic = ["version"]
 
-
 [tool.poetry]
 name = "boxfs"
-version = "0.1.1"
-description = "Implementation of fsspec for Box file storage"
+version = "0.1-alpha1"
+description = "Box File System"
 authors = ["Thomas Hunter <boxfs.tehunter@gmail.com>"]
 packages = [
     { include = "boxfs", from = "src" }
 ]
-readme = "README.md"
-license = "MIT"
-repository = "https://github.com/IBM/boxfs"
-keywords = ["file-storage", "fsspec", "file-system", "box"]
-classifiers = [
-    "Development Status :: 2 - Pre-Alpha",
-    "Topic :: Database",
-    "Topic :: Office/Business",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "Topic :: System :: Filesystems",
-    "Topic :: Utilities",
-]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 boxsdk = {version = "^3.7", extras = ["jwt"]}
 fsspec = ">=2023.4"
 # universal-pathlib = "^0.0.23"
 # TEMP: Temporary fix for boxsdk dependency conflict as of 5/8/2023
```

### Comparing `boxfs-0.1.1/src/boxfs/boxfs.py` & `boxfs-0.1a1/src/boxfs/boxfs.py`

 * *Files identical despite different names*


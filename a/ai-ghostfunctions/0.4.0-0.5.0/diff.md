# Comparing `tmp/ai_ghostfunctions-0.4.0.tar.gz` & `tmp/ai_ghostfunctions-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_ghostfunctions-0.4.0.tar", max compression
+gzip compressed data, was "ai_ghostfunctions-0.5.0.tar", max compression
```

## Comparing `ai_ghostfunctions-0.4.0.tar` & `ai_ghostfunctions-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-05-04 22:43:14.564348 ai_ghostfunctions-0.4.0/LICENSE
--rw-r--r--   0        0        0     4451 2023-05-04 22:43:14.568348 ai_ghostfunctions-0.4.0/README.md
--rw-r--r--   0        0        0     1828 2023-05-04 22:43:30.620375 ai_ghostfunctions-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      162 2023-05-04 22:43:14.568348 ai_ghostfunctions-0.4.0/src/ai_ghostfunctions/__init__.py
--rw-r--r--   0        0        0     6689 2023-05-04 22:43:14.568348 ai_ghostfunctions-0.4.0/src/ai_ghostfunctions/ghostfunctions.py
--rw-r--r--   0        0        0      231 2023-05-04 22:43:14.568348 ai_ghostfunctions-0.4.0/src/ai_ghostfunctions/keywords.py
--rw-r--r--   0        0        0        0 2023-05-04 22:43:14.568348 ai_ghostfunctions-0.4.0/src/ai_ghostfunctions/py.typed
--rw-r--r--   0        0        0      343 2023-05-04 22:43:14.568348 ai_ghostfunctions-0.4.0/src/ai_ghostfunctions/types.py
--rw-r--r--   0        0        0     5377 1970-01-01 00:00:00.000000 ai_ghostfunctions-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-12 21:41:24.666035 ai_ghostfunctions-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4451 2023-05-12 21:41:24.666035 ai_ghostfunctions-0.5.0/README.md
+-rw-r--r--   0        0        0     1828 2023-05-12 21:41:38.270156 ai_ghostfunctions-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      162 2023-05-12 21:41:24.670035 ai_ghostfunctions-0.5.0/src/ai_ghostfunctions/__init__.py
+-rw-r--r--   0        0        0     8200 2023-05-12 21:41:24.670035 ai_ghostfunctions-0.5.0/src/ai_ghostfunctions/ghostfunctions.py
+-rw-r--r--   0        0        0      231 2023-05-12 21:41:24.670035 ai_ghostfunctions-0.5.0/src/ai_ghostfunctions/keywords.py
+-rw-r--r--   0        0        0        0 2023-05-12 21:41:24.670035 ai_ghostfunctions-0.5.0/src/ai_ghostfunctions/py.typed
+-rw-r--r--   0        0        0      343 2023-05-12 21:41:24.670035 ai_ghostfunctions-0.5.0/src/ai_ghostfunctions/types.py
+-rw-r--r--   0        0        0     5377 1970-01-01 00:00:00.000000 ai_ghostfunctions-0.5.0/PKG-INFO
```

### Comparing `ai_ghostfunctions-0.4.0/LICENSE` & `ai_ghostfunctions-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_ghostfunctions-0.4.0/README.md` & `ai_ghostfunctions-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ai_ghostfunctions-0.4.0/pyproject.toml` & `ai_ghostfunctions-0.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai-ghostfunctions"
-version = "0.4.0"
+version = "0.5.0"
 description = "AI Ghostfunctions"
 authors = ["Brian M. Ritz <brianmritz@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bmritz/ai-ghostfunctions"
 repository = "https://github.com/bmritz/ai-ghostfunctions"
 documentation = "https://ai-ghostfunctions.readthedocs.io"
```

### Comparing `ai_ghostfunctions-0.4.0/PKG-INFO` & `ai_ghostfunctions-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-ghostfunctions
-Version: 0.4.0
+Version: 0.5.0
 Summary: AI Ghostfunctions
 Home-page: https://github.com/bmritz/ai-ghostfunctions
 License: MIT
 Author: Brian M. Ritz
 Author-email: brianmritz@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```


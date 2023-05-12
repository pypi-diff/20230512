# Comparing `tmp/ld2410-1.1.tar.gz` & `tmp/ld2410-1.1.1.tar.gz`

## Comparing `ld2410-1.1.tar` & `ld2410-1.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 ld2410-1.1/example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ld2410-1.1/LD2410/LICENSE
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ld2410-1.1/LD2410/__init__.py
--rw-r--r--   0        0        0    13123 2020-02-02 00:00:00.000000 ld2410-1.1/LD2410/ld2410.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 ld2410-1.1/LD2410/ld2410_consts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ld2410-1.1/LD2410/setup.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 ld2410-1.1/LICENSE
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 ld2410-1.1/README.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 ld2410-1.1/pyproject.toml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 ld2410-1.1/PKG-INFO
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 ld2410-1.1.1/example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ld2410-1.1.1/LD2410/LICENSE
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ld2410-1.1.1/LD2410/__init__.py
+-rw-r--r--   0        0        0    13123 2020-02-02 00:00:00.000000 ld2410-1.1.1/LD2410/ld2410.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 ld2410-1.1.1/LD2410/ld2410_consts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ld2410-1.1.1/LD2410/setup.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 ld2410-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 ld2410-1.1.1/README.md
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 ld2410-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 ld2410-1.1.1/PKG-INFO
```

### Comparing `ld2410-1.1/example.py` & `ld2410-1.1.1/example.py`

 * *Files identical despite different names*

### Comparing `ld2410-1.1/LD2410/ld2410.py` & `ld2410-1.1.1/LD2410/ld2410.py`

 * *Files identical despite different names*

### Comparing `ld2410-1.1/LD2410/ld2410_consts.py` & `ld2410-1.1.1/LD2410/ld2410_consts.py`

 * *Files identical despite different names*

### Comparing `ld2410-1.1/LICENSE` & `ld2410-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ld2410-1.1/pyproject.toml` & `ld2410-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "LD2410"
-version = "1.1"
+version = "1.1.1"
 authors = [
   { name="Vi Jun Sean Yong", email="vjsyong@connect.ust.hk" },
 ]
 description = "A python interface for the HiLink LD2410 presence detection module"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```


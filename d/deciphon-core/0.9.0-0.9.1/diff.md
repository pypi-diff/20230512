# Comparing `tmp/deciphon_core-0.9.0.tar.gz` & `tmp/deciphon_core-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deciphon_core-0.9.0.tar", max compression
+gzip compressed data, was "deciphon_core-0.9.1.tar", max compression
```

## Comparing `deciphon_core-0.9.0.tar` & `deciphon_core-0.9.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1069 2023-03-08 14:04:58.431591 deciphon_core-0.9.0/LICENSE
--rw-r--r--   0        0        0       65 2023-03-08 14:04:58.431591 deciphon_core-0.9.0/README.md
--rw-r--r--   0        0        0     3845 2023-03-08 14:04:58.431591 deciphon_core-0.9.0/build_ext.py
--rw-r--r--   0        0        0        0 2023-03-08 14:04:58.431591 deciphon_core-0.9.0/deciphon_core/__init__.py
--rw-r--r--   0        0        0     1401 2023-03-08 14:04:58.431591 deciphon_core-0.9.0/deciphon_core/cseq.py
--rw-r--r--   0        0        0      694 2023-03-08 14:04:58.431591 deciphon_core-0.9.0/deciphon_core/dbfile.py
--rw-r--r--   0        0        0      257 2023-03-08 14:04:58.431591 deciphon_core-0.9.0/deciphon_core/error.py
--rw-r--r--   0        0        0       91 2023-03-08 14:04:58.431591 deciphon_core-0.9.0/deciphon_core/filepath.py
--rw-r--r--   0        0        0     1515 2023-03-08 14:04:58.431591 deciphon_core-0.9.0/deciphon_core/h3result.py
--rw-r--r--   0        0        0      659 2023-03-08 14:04:58.431591 deciphon_core-0.9.0/deciphon_core/hmmfile.py
--rw-r--r--   0        0        0     1759 2023-03-08 14:04:58.431591 deciphon_core-0.9.0/deciphon_core/interface.h
--rw-r--r--   0        0        0     1852 2023-03-08 14:04:58.431591 deciphon_core-0.9.0/deciphon_core/press.py
--rw-r--r--   0        0        0     3042 2023-03-08 14:04:58.431591 deciphon_core-0.9.0/deciphon_core/scan.py
--rw-r--r--   0        0        0      303 2023-03-08 14:04:58.431591 deciphon_core-0.9.0/deciphon_core/seq.py
--rw-r--r--   0        0        0     1014 2023-03-08 14:04:58.431591 deciphon_core-0.9.0/deciphon_core/snapfile.py
--rw-r--r--   0        0        0      891 2023-03-08 14:04:58.431591 deciphon_core-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 deciphon_core-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-08 15:03:34.008876 deciphon_core-0.9.1/LICENSE
+-rw-r--r--   0        0        0       65 2023-03-08 15:03:34.008876 deciphon_core-0.9.1/README.md
+-rw-r--r--   0        0        0     3845 2023-03-08 15:03:34.008876 deciphon_core-0.9.1/build_ext.py
+-rw-r--r--   0        0        0        0 2023-03-08 15:03:34.008876 deciphon_core-0.9.1/deciphon_core/__init__.py
+-rw-r--r--   0        0        0     1401 2023-03-08 15:03:34.008876 deciphon_core-0.9.1/deciphon_core/cseq.py
+-rw-r--r--   0        0        0      694 2023-03-08 15:03:34.008876 deciphon_core-0.9.1/deciphon_core/dbfile.py
+-rw-r--r--   0        0        0      257 2023-03-08 15:03:34.008876 deciphon_core-0.9.1/deciphon_core/error.py
+-rw-r--r--   0        0        0       91 2023-03-08 15:03:34.008876 deciphon_core-0.9.1/deciphon_core/filepath.py
+-rw-r--r--   0        0        0     1515 2023-03-08 15:03:34.008876 deciphon_core-0.9.1/deciphon_core/h3result.py
+-rw-r--r--   0        0        0      659 2023-03-08 15:03:34.008876 deciphon_core-0.9.1/deciphon_core/hmmfile.py
+-rw-r--r--   0        0        0     1759 2023-03-08 15:03:34.008876 deciphon_core-0.9.1/deciphon_core/interface.h
+-rw-r--r--   0        0        0     1852 2023-03-08 15:03:34.008876 deciphon_core-0.9.1/deciphon_core/press.py
+-rw-r--r--   0        0        0     3042 2023-03-08 15:03:34.008876 deciphon_core-0.9.1/deciphon_core/scan.py
+-rw-r--r--   0        0        0      303 2023-03-08 15:03:34.008876 deciphon_core-0.9.1/deciphon_core/seq.py
+-rw-r--r--   0        0        0     1014 2023-03-08 15:03:34.008876 deciphon_core-0.9.1/deciphon_core/snapfile.py
+-rw-r--r--   0        0        0      891 2023-03-08 15:03:34.008876 deciphon_core-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 deciphon_core-0.9.1/PKG-INFO
```

### Comparing `deciphon_core-0.9.0/LICENSE` & `deciphon_core-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deciphon_core-0.9.0/build_ext.py` & `deciphon_core-0.9.1/build_ext.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     Ext("horta", "logaddexp", "2.1.14", CMAKE_OPTS),
     Ext("horta", "elapsed", "3.1.2", CMAKE_OPTS),
     Ext("EBI-Metagenomics", "lip", "0.5.0", CMAKE_OPTS),
     Ext("EBI-Metagenomics", "hmr", "0.6.0", CMAKE_OPTS),
     Ext("EBI-Metagenomics", "imm", "2.2.1", CMAKE_OPTS + CPM_OPTS),
     Ext("nanomsg", "nng", "1.5.2", CMAKE_OPTS + NNG_OPTS),
     Ext("EBI-Metagenomics", "h3c", "0.10.5", CMAKE_OPTS + CPM_OPTS),
-    Ext("EBI-Metagenomics", "deciphon", "0.6.0", CMAKE_OPTS + CPM_OPTS),
+    Ext("EBI-Metagenomics", "deciphon", "0.6.1", CMAKE_OPTS + CPM_OPTS),
 ]
 
 
 def rm(folder: Path, pattern: str):
     for filename in folder.glob(pattern):
         filename.unlink()
```

### Comparing `deciphon_core-0.9.0/deciphon_core/cseq.py` & `deciphon_core-0.9.1/deciphon_core/cseq.py`

 * *Files identical despite different names*

### Comparing `deciphon_core-0.9.0/deciphon_core/dbfile.py` & `deciphon_core-0.9.1/deciphon_core/dbfile.py`

 * *Files identical despite different names*

### Comparing `deciphon_core-0.9.0/deciphon_core/h3result.py` & `deciphon_core-0.9.1/deciphon_core/h3result.py`

 * *Files identical despite different names*

### Comparing `deciphon_core-0.9.0/deciphon_core/hmmfile.py` & `deciphon_core-0.9.1/deciphon_core/hmmfile.py`

 * *Files identical despite different names*

### Comparing `deciphon_core-0.9.0/deciphon_core/interface.h` & `deciphon_core-0.9.1/deciphon_core/interface.h`

 * *Files identical despite different names*

### Comparing `deciphon_core-0.9.0/deciphon_core/press.py` & `deciphon_core-0.9.1/deciphon_core/press.py`

 * *Files identical despite different names*

### Comparing `deciphon_core-0.9.0/deciphon_core/scan.py` & `deciphon_core-0.9.1/deciphon_core/scan.py`

 * *Files identical despite different names*

### Comparing `deciphon_core-0.9.0/deciphon_core/snapfile.py` & `deciphon_core-0.9.1/deciphon_core/snapfile.py`

 * *Files identical despite different names*

### Comparing `deciphon_core-0.9.0/pyproject.toml` & `deciphon_core-0.9.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deciphon-core"
-version = "0.9.0"
+version = "0.9.1"
 description = "Python package for biding the C implementation"
 authors = ["Danilo Horta <danilo.horta@pm.me>"]
 license = "MIT"
 readme = "README.md"
 include = [
   { path = "deciphon_core/*.so", format = "wheel" },
   { path = "deciphon_core/*.pyd", format = "wheel" },
```

### Comparing `deciphon_core-0.9.0/PKG-INFO` & `deciphon_core-0.9.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deciphon-core
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python package for biding the C implementation
 License: MIT
 Author: Danilo Horta
 Author-email: danilo.horta@pm.me
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


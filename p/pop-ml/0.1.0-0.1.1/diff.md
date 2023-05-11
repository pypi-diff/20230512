# Comparing `tmp/pop-ml-0.1.0.tar.gz` & `tmp/pop-ml-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop-ml-0.1.0.tar", last modified: Wed May 10 03:47:39 2023, max compression
+gzip compressed data, was "pop-ml-0.1.1.tar", last modified: Thu May 11 23:46:11 2023, max compression
```

## Comparing `pop-ml-0.1.0.tar` & `pop-ml-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 03:47:39.076100 pop-ml-0.1.0/
--rw-r--r--   0 root         (0) root         (0)    11342 2023-05-10 03:47:24.000000 pop-ml-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5835 2023-05-10 03:47:39.076100 pop-ml-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4828 2023-05-10 03:47:24.000000 pop-ml-0.1.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 03:47:39.076100 pop-ml-0.1.0/pop_ml.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5835 2023-05-10 03:47:39.000000 pop-ml-0.1.0/pop_ml.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      219 2023-05-10 03:47:39.000000 pop-ml-0.1.0/pop_ml.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 03:47:39.000000 pop-ml-0.1.0/pop_ml.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-05-10 03:47:39.000000 pop-ml-0.1.0/pop_ml.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-10 03:47:39.000000 pop-ml-0.1.0/pop_ml.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 03:47:39.000000 pop-ml-0.1.0/pop_ml.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-10 03:47:39.076100 pop-ml-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2987 2023-05-10 03:47:24.000000 pop-ml-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 23:46:11.622382 pop-ml-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)    11342 2023-05-11 23:45:56.000000 pop-ml-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5835 2023-05-11 23:46:11.622382 pop-ml-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4828 2023-05-11 23:45:56.000000 pop-ml-0.1.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 23:46:11.622382 pop-ml-0.1.1/pop_ml/
+-rw-r--r--   0 root         (0) root         (0)     1287 2023-05-11 23:45:56.000000 pop-ml-0.1.1/pop_ml/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 23:46:11.622382 pop-ml-0.1.1/pop_ml/ml/
+-rw-r--r--   0 root         (0) root         (0)      823 2023-05-11 23:45:56.000000 pop-ml-0.1.1/pop_ml/ml/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-05-11 23:45:56.000000 pop-ml-0.1.1/pop_ml/ml/init.py
+-rw-r--r--   0 root         (0) root         (0)     3889 2023-05-11 23:45:56.000000 pop-ml-0.1.1/pop_ml/ml/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-05-11 23:45:56.000000 pop-ml-0.1.1/pop_ml/scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 23:46:11.622382 pop-ml-0.1.1/pop_ml/token/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 23:46:11.622382 pop-ml-0.1.1/pop_ml/token/contracts/
+-rw-r--r--   0 root         (0) root         (0)      277 2023-05-11 23:45:56.000000 pop-ml-0.1.1/pop_ml/token/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-05-11 23:45:56.000000 pop-ml-0.1.1/pop_ml/token/init.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-11 23:45:56.000000 pop-ml-0.1.1/pop_ml/token/python_keywords.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-11 23:46:11.000000 pop-ml-0.1.1/pop_ml/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 23:46:11.622382 pop-ml-0.1.1/pop_ml.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5835 2023-05-11 23:46:11.000000 pop-ml-0.1.1/pop_ml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      416 2023-05-11 23:46:11.000000 pop-ml-0.1.1/pop_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 23:46:11.000000 pop-ml-0.1.1/pop_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-11 23:46:11.000000 pop-ml-0.1.1/pop_ml.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-11 23:46:11.000000 pop-ml-0.1.1/pop_ml.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-11 23:46:11.000000 pop-ml-0.1.1/pop_ml.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-11 23:46:11.622382 pop-ml-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2983 2023-05-11 23:45:56.000000 pop-ml-0.1.1/setup.py
```

### Comparing `pop-ml-0.1.0/LICENSE` & `pop-ml-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pop-ml-0.1.0/PKG-INFO` & `pop-ml-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-ml
-Version: 0.1.0
+Version: 0.1.1
 Summary: Machine learning library for pop projects
 Home-page: https://gitlab.com/vmware/pop/pop-ml
 Author: VMWare, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `pop-ml-0.1.0/README.rst` & `pop-ml-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `pop-ml-0.1.0/pop_ml.egg-info/PKG-INFO` & `pop-ml-0.1.1/pop_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-ml
-Version: 0.1.0
+Version: 0.1.1
 Summary: Machine learning library for pop projects
 Home-page: https://gitlab.com/vmware/pop/pop-ml
 Author: VMWare, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `pop-ml-0.1.0/setup.py` & `pop-ml-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 import os
 import pathlib
 import shutil
 
 from setuptools import Command
 from setuptools import setup
 
-NAME = "pop-ml"
+NAME = "pop_ml"
 DESC = "Machine learning library for pop projects"
 
 # Version info -- read without importing
 _locals = {}
-with pathlib.Path("pop_ml", "version.py").open() as fp:
+with pathlib.Path(NAME, "version.py").open() as fp:
     exec(fp.read(), None, _locals)
 VERSION = _locals["version"]
 SETUP_DIRNAME = os.path.dirname(__file__)
 if not SETUP_DIRNAME:
     SETUP_DIRNAME = os.getcwd()
 
 with open("README.rst", encoding="utf-8") as f:
```


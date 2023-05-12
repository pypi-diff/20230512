# Comparing `tmp/homeduino-0.0.5.8.tar.gz` & `tmp/homeduino-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeduino-0.0.5.8.tar", last modified: Thu May 11 16:46:52 2023, max compression
+gzip compressed data, was "homeduino-0.0.6.tar", last modified: Fri May 12 15:02:50 2023, max compression
```

## Comparing `homeduino-0.0.5.8.tar` & `homeduino-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:46:52.451246 homeduino-0.0.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-05-11 16:46:32.000000 homeduino-0.0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-11 16:46:52.451246 homeduino-0.0.5.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:46:52.451246 homeduino-0.0.5.8/homeduino/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-11 16:46:32.000000 homeduino-0.0.5.8/homeduino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-11 16:46:32.000000 homeduino-0.0.5.8/homeduino/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-05-11 16:46:32.000000 homeduino-0.0.5.8/homeduino/homeduino.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:46:52.451246 homeduino-0.0.5.8/homeduino.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-11 16:46:52.000000 homeduino-0.0.5.8/homeduino.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-11 16:46:52.000000 homeduino-0.0.5.8/homeduino.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:46:52.000000 homeduino-0.0.5.8/homeduino.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-11 16:46:52.000000 homeduino-0.0.5.8/homeduino.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 16:46:52.000000 homeduino-0.0.5.8/homeduino.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-11 16:46:32.000000 homeduino-0.0.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 16:46:52.451246 homeduino-0.0.5.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:02:50.867834 homeduino-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-05-12 15:02:35.000000 homeduino-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-12 15:02:50.867834 homeduino-0.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:02:50.863834 homeduino-0.0.6/homeduino/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-12 15:02:35.000000 homeduino-0.0.6/homeduino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-12 15:02:35.000000 homeduino-0.0.6/homeduino/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-05-12 15:02:35.000000 homeduino-0.0.6/homeduino/homeduino.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:02:50.867834 homeduino-0.0.6/homeduino.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-12 15:02:50.000000 homeduino-0.0.6/homeduino.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-12 15:02:50.000000 homeduino-0.0.6/homeduino.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:02:50.000000 homeduino-0.0.6/homeduino.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-12 15:02:50.000000 homeduino-0.0.6/homeduino.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-12 15:02:50.000000 homeduino-0.0.6/homeduino.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-12 15:02:35.000000 homeduino-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 15:02:50.867834 homeduino-0.0.6/setup.cfg
```

### Comparing `homeduino-0.0.5.8/LICENSE` & `homeduino-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `homeduino-0.0.5.8/PKG-INFO` & `homeduino-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeduino
-Version: 0.0.5.8
+Version: 0.0.6
 Summary: Homeduino library
 Author: Rogier van Staveren
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rrooggiieerr/homeduino.py
 Project-URL: Bug Tracker, https://github.com/rrooggiieerr/homeduino.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `homeduino-0.0.5.8/homeduino/__main__.py` & `homeduino-0.0.6/homeduino/__main__.py`

 * *Files identical despite different names*

### Comparing `homeduino-0.0.5.8/homeduino/homeduino.py` & `homeduino-0.0.6/homeduino/homeduino.py`

 * *Files identical despite different names*

### Comparing `homeduino-0.0.5.8/homeduino.egg-info/PKG-INFO` & `homeduino-0.0.6/homeduino.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeduino
-Version: 0.0.5.8
+Version: 0.0.6
 Summary: Homeduino library
 Author: Rogier van Staveren
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rrooggiieerr/homeduino.py
 Project-URL: Bug Tracker, https://github.com/rrooggiieerr/homeduino.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `homeduino-0.0.5.8/pyproject.toml` & `homeduino-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "homeduino"
-version = "0.0.5.8"
+version = "0.0.6"
 license = {text = "Apache-2.0"}
 authors = [
     { name="Rogier van Staveren" }
 ]
 description = "Homeduino library"
 readme = "README.md"
 requires-python = ">=3.7"
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "pyserial-asyncio==0.6",
-    "rfcontrolpy>=0.0.2"
+    "rfcontrolpy>=0.0.3"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/rrooggiieerr/homeduino.py"
 "Bug Tracker" = "https://github.com/rrooggiieerr/homeduino.py/issues"
 
 [tool.black]
```


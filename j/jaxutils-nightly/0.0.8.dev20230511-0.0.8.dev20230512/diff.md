# Comparing `tmp/jaxutils-nightly-0.0.8.dev20230511.tar.gz` & `tmp/jaxutils-nightly-0.0.8.dev20230512.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20230511.tar", last modified: Thu May 11 00:06:43 2023, max compression
+gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20230512.tar", last modified: Fri May 12 00:06:33 2023, max compression
```

## Comparing `jaxutils-nightly-0.0.8.dev20230511.tar` & `jaxutils-nightly-0.0.8.dev20230512.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 00:06:43.653096 jaxutils-nightly-0.0.8.dev20230511/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4448 2023-05-11 00:06:43.653096 jaxutils-nightly-0.0.8.dev20230511/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2894 2023-05-11 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230511/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 00:06:43.657096 jaxutils-nightly-0.0.8.dev20230511/jaxutils/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2023-05-11 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230511/jaxutils/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2023-05-11 00:06:43.657096 jaxutils-nightly-0.0.8.dev20230511/jaxutils/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2023-05-11 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230511/jaxutils/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2023-05-11 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230511/jaxutils/data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2023-05-11 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230511/jaxutils/dict.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2023-05-11 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230511/jaxutils/parameters.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2023-05-11 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230511/jaxutils/pytree.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 00:06:43.653096 jaxutils-nightly-0.0.8.dev20230511/jaxutils_nightly.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4448 2023-05-11 00:06:43.000000 jaxutils-nightly-0.0.8.dev20230511/jaxutils_nightly.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2023-05-11 00:06:43.000000 jaxutils-nightly-0.0.8.dev20230511/jaxutils_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-11 00:06:43.000000 jaxutils-nightly-0.0.8.dev20230511/jaxutils_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-05-11 00:06:43.000000 jaxutils-nightly-0.0.8.dev20230511/jaxutils_nightly.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-05-11 00:06:43.000000 jaxutils-nightly-0.0.8.dev20230511/jaxutils_nightly.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2023-05-11 00:06:43.657096 jaxutils-nightly-0.0.8.dev20230511/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2023-05-11 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230511/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2023-05-11 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230511/versioneer.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-12 00:06:33.310334 jaxutils-nightly-0.0.8.dev20230512/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-05-12 00:06:33.310334 jaxutils-nightly-0.0.8.dev20230512/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3004 2023-05-12 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230512/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-12 00:06:33.314334 jaxutils-nightly-0.0.8.dev20230512/jaxutils/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2023-05-12 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230512/jaxutils/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2023-05-12 00:06:33.314334 jaxutils-nightly-0.0.8.dev20230512/jaxutils/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2023-05-12 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230512/jaxutils/config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2023-05-12 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230512/jaxutils/data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2023-05-12 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230512/jaxutils/dict.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2023-05-12 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230512/jaxutils/parameters.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2023-05-12 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230512/jaxutils/pytree.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-12 00:06:33.310334 jaxutils-nightly-0.0.8.dev20230512/jaxutils_nightly.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-05-12 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230512/jaxutils_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2023-05-12 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230512/jaxutils_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-12 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230512/jaxutils_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-05-12 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230512/jaxutils_nightly.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-05-12 00:06:33.000000 jaxutils-nightly-0.0.8.dev20230512/jaxutils_nightly.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2023-05-12 00:06:33.310334 jaxutils-nightly-0.0.8.dev20230512/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2023-05-12 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230512/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2023-05-12 00:06:26.000000 jaxutils-nightly-0.0.8.dev20230512/versioneer.py
```

### Comparing `jaxutils-nightly-0.0.8.dev20230511/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20230512/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20230511
+Version: 0.0.8.dev20230512
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
-Description: # [JaxUtils](https://github.com/JaxGaussianProcesses/JaxUtils)
+Description: ----
+        This project has now been incorporated into [GPJax](https://github.com/JaxGaussianProcesses/GPJax).
+        ----
+        # [JaxUtils](https://github.com/JaxGaussianProcesses/JaxUtils)
         
         [![CircleCI](https://dl.circleci.com/status-badge/img/gh/JaxGaussianProcesses/JaxUtils/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/JaxGaussianProcesses/JaxUtils/tree/master)
         
         `JaxUtils` provides utility functions for the [`JaxGaussianProcesses`]() ecosystem.</h2>
         
         # Contents
```

### Comparing `jaxutils-nightly-0.0.8.dev20230511/README.md` & `jaxutils-nightly-0.0.8.dev20230512/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+----
+This project has now been incorporated into [GPJax](https://github.com/JaxGaussianProcesses/GPJax).
+----
 # [JaxUtils](https://github.com/JaxGaussianProcesses/JaxUtils)
 
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/JaxGaussianProcesses/JaxUtils/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/JaxGaussianProcesses/JaxUtils/tree/master)
 
 `JaxUtils` provides utility functions for the [`JaxGaussianProcesses`]() ecosystem.</h2>
 
 # Contents
```

### Comparing `jaxutils-nightly-0.0.8.dev20230511/jaxutils/__init__.py` & `jaxutils-nightly-0.0.8.dev20230512/jaxutils/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230511/jaxutils/config.py` & `jaxutils-nightly-0.0.8.dev20230512/jaxutils/config.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230511/jaxutils/data.py` & `jaxutils-nightly-0.0.8.dev20230512/jaxutils/data.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230511/jaxutils/dict.py` & `jaxutils-nightly-0.0.8.dev20230512/jaxutils/dict.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230511/jaxutils/parameters.py` & `jaxutils-nightly-0.0.8.dev20230512/jaxutils/parameters.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230511/jaxutils/pytree.py` & `jaxutils-nightly-0.0.8.dev20230512/jaxutils/pytree.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230511/jaxutils_nightly.egg-info/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20230512/jaxutils_nightly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20230511
+Version: 0.0.8.dev20230512
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
-Description: # [JaxUtils](https://github.com/JaxGaussianProcesses/JaxUtils)
+Description: ----
+        This project has now been incorporated into [GPJax](https://github.com/JaxGaussianProcesses/GPJax).
+        ----
+        # [JaxUtils](https://github.com/JaxGaussianProcesses/JaxUtils)
         
         [![CircleCI](https://dl.circleci.com/status-badge/img/gh/JaxGaussianProcesses/JaxUtils/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/JaxGaussianProcesses/JaxUtils/tree/master)
         
         `JaxUtils` provides utility functions for the [`JaxGaussianProcesses`]() ecosystem.</h2>
         
         # Contents
```

### Comparing `jaxutils-nightly-0.0.8.dev20230511/setup.py` & `jaxutils-nightly-0.0.8.dev20230512/setup.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230511/versioneer.py` & `jaxutils-nightly-0.0.8.dev20230512/versioneer.py`

 * *Files identical despite different names*


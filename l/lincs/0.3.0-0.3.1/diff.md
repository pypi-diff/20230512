# Comparing `tmp/lincs-0.3.0.tar.gz` & `tmp/lincs-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lincs-0.3.0.tar", last modified: Thu May 11 17:39:46 2023, max compression
+gzip compressed data, was "lincs-0.3.1.tar", last modified: Fri May 12 08:54:07 2023, max compression
```

## Comparing `lincs-0.3.0.tar` & `lincs-0.3.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-11 17:39:46.074369 lincs-0.3.0/
--rw-r--r--   0 user      (1002) user      (1002)      102 2023-05-11 16:35:31.000000 lincs-0.3.0/MANIFEST.in
--rw-r--r--   0 user      (1002) user      (1002)    16795 2023-05-11 17:39:46.074369 lincs-0.3.0/PKG-INFO
--rw-rw-r--   0 user      (1002) user      (1002)    16088 2023-05-11 17:35:39.000000 lincs-0.3.0/README.md
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-11 17:39:46.070369 lincs-0.3.0/lincs/
--rw-rw-r--   0 user      (1002) user      (1002)      762 2023-05-11 16:48:08.000000 lincs-0.3.0/lincs/__init__.py
--rw-r--r--   0 user      (1002) user      (1002)      136 2023-05-04 08:59:02.000000 lincs-0.3.0/lincs/__main__.py
--rw-rw-r--   0 user      (1002) user      (1002)    21943 2023-05-11 17:15:21.000000 lincs-0.3.0/lincs/command_line_interface.py
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-11 17:39:46.074369 lincs-0.3.0/lincs/liblincs/
--rw-rw-r--   0 user      (1002) user      (1002)     1566 2023-05-09 14:37:35.000000 lincs-0.3.0/lincs/liblincs/classification.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     9942 2023-05-08 05:22:27.000000 lincs-0.3.0/lincs/liblincs/generation.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     6492 2023-05-11 13:04:24.000000 lincs-0.3.0/lincs/liblincs/io.cpp
--rw-rw-r--   0 user      (1002) user      (1002)    26434 2023-05-11 17:02:54.000000 lincs-0.3.0/lincs/liblincs/learning.cpp
--rw-rw-r--   0 user      (1002) user      (1002)    15089 2023-05-11 16:48:00.000000 lincs-0.3.0/lincs/liblincs/liblincs_module.cpp
--rw-rw-r--   0 user      (1002) user      (1002)    11471 2023-05-11 17:01:21.000000 lincs-0.3.0/lincs/liblincs/lincs.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     2928 2023-05-11 13:04:24.000000 lincs-0.3.0/lincs/liblincs/median-and-max.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      741 2023-05-11 13:04:24.000000 lincs-0.3.0/lincs/liblincs/randomness-utils.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1391 2023-05-11 13:04:24.000000 lincs-0.3.0/lincs/liblincs/randomness-utils.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    10384 2023-05-11 16:48:16.000000 lincs-0.3.0/lincs/liblincs_module_tests.py
--rw-rw-r--   0 user      (1002) user      (1002)      759 2023-05-11 17:16:10.000000 lincs-0.3.0/lincs/visualization.py
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-11 17:39:46.070369 lincs-0.3.0/lincs.egg-info/
--rw-r--r--   0 user      (1002) user      (1002)    16795 2023-05-11 17:39:46.000000 lincs-0.3.0/lincs.egg-info/PKG-INFO
--rw-r--r--   0 user      (1002) user      (1002)      625 2023-05-11 17:39:46.000000 lincs-0.3.0/lincs.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1002) user      (1002)        1 2023-05-11 17:39:46.000000 lincs-0.3.0/lincs.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1002) user      (1002)       60 2023-05-11 17:39:46.000000 lincs-0.3.0/lincs.egg-info/entry_points.txt
--rw-r--r--   0 user      (1002) user      (1002)       27 2023-05-11 17:39:46.000000 lincs-0.3.0/lincs.egg-info/requires.txt
--rw-r--r--   0 user      (1002) user      (1002)       15 2023-05-11 17:39:46.000000 lincs-0.3.0/lincs.egg-info/top_level.txt
--rw-r--r--   0 user      (1002) user      (1002)       27 2023-05-05 13:01:57.000000 lincs-0.3.0/requirements.txt
--rw-r--r--   0 user      (1002) user      (1002)       38 2023-05-11 17:39:46.074369 lincs-0.3.0/setup.cfg
--rw-rw-r--   0 user      (1002) user      (1002)     2439 2023-05-11 17:38:48.000000 lincs-0.3.0/setup.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 08:54:07.058991 lincs-0.3.1/
+-rw-rw-r--   0 user      (1002) user      (1002)       70 2023-05-12 08:52:07.000000 lincs-0.3.1/MANIFEST.in
+-rw-r--r--   0 user      (1002) user      (1002)    16795 2023-05-12 08:54:07.058991 lincs-0.3.1/PKG-INFO
+-rw-rw-r--   0 user      (1002) user      (1002)    16088 2023-05-11 17:35:39.000000 lincs-0.3.1/README.md
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 08:54:07.058991 lincs-0.3.1/lincs/
+-rw-rw-r--   0 user      (1002) user      (1002)      762 2023-05-11 16:48:08.000000 lincs-0.3.1/lincs/__init__.py
+-rw-r--r--   0 user      (1002) user      (1002)      136 2023-05-04 08:59:02.000000 lincs-0.3.1/lincs/__main__.py
+-rw-rw-r--   0 user      (1002) user      (1002)    21943 2023-05-11 17:15:21.000000 lincs-0.3.1/lincs/command_line_interface.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 08:54:07.058991 lincs-0.3.1/lincs/liblincs/
+-rw-rw-r--   0 user      (1002) user      (1002)     1566 2023-05-12 08:51:21.000000 lincs-0.3.1/lincs/liblincs/classification.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     9942 2023-05-12 08:51:21.000000 lincs-0.3.1/lincs/liblincs/generation.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     6492 2023-05-12 08:51:21.000000 lincs-0.3.1/lincs/liblincs/io.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)    26434 2023-05-12 08:51:21.000000 lincs-0.3.1/lincs/liblincs/learning.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)    15089 2023-05-12 08:51:21.000000 lincs-0.3.1/lincs/liblincs/liblincs_module.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)    11471 2023-05-12 08:51:21.000000 lincs-0.3.1/lincs/liblincs/lincs.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     2928 2023-05-12 08:51:14.000000 lincs-0.3.1/lincs/liblincs/median-and-max.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      609 2023-05-12 08:51:14.000000 lincs-0.3.1/lincs/liblincs/median-and-max.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)      741 2023-05-12 08:51:14.000000 lincs-0.3.1/lincs/liblincs/randomness-utils.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1391 2023-05-12 08:51:21.000000 lincs-0.3.1/lincs/liblincs/randomness-utils.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    10384 2023-05-11 16:48:16.000000 lincs-0.3.1/lincs/liblincs_module_tests.py
+-rw-rw-r--   0 user      (1002) user      (1002)      759 2023-05-11 17:16:10.000000 lincs-0.3.1/lincs/visualization.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 08:54:07.058991 lincs-0.3.1/lincs.egg-info/
+-rw-r--r--   0 user      (1002) user      (1002)    16795 2023-05-12 08:54:07.000000 lincs-0.3.1/lincs.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1002) user      (1002)      659 2023-05-12 08:54:07.000000 lincs-0.3.1/lincs.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1002) user      (1002)        1 2023-05-12 08:54:07.000000 lincs-0.3.1/lincs.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1002) user      (1002)       60 2023-05-12 08:54:07.000000 lincs-0.3.1/lincs.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1002) user      (1002)       27 2023-05-12 08:54:07.000000 lincs-0.3.1/lincs.egg-info/requires.txt
+-rw-r--r--   0 user      (1002) user      (1002)       15 2023-05-12 08:54:07.000000 lincs-0.3.1/lincs.egg-info/top_level.txt
+-rw-r--r--   0 user      (1002) user      (1002)       27 2023-05-05 13:01:57.000000 lincs-0.3.1/requirements.txt
+-rw-r--r--   0 user      (1002) user      (1002)       38 2023-05-12 08:54:07.058991 lincs-0.3.1/setup.cfg
+-rw-rw-r--   0 user      (1002) user      (1002)     2200 2023-05-12 08:53:31.000000 lincs-0.3.1/setup.py
```

### Comparing `lincs-0.3.0/PKG-INFO` & `lincs-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincs
-Version: 0.3.0
+Version: 0.3.1
 Summary: MCDA algorithms
 Home-page: https://github.com/jacquev6/lincs
 Author: Vincent Jacques
 Author-email: vincent@vincent-jacques.net
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -267,15 +267,15 @@
 <!-- STOP -->
 <!-- EXTEND command-line-example/run.sh --><!--
     cp model.png ../../..
 --><!-- STOP -->
 
 It should output something like:
 
-![Model visualization](https://github.com/jacquev6/lincs/raw/v0.3.0/model.png)
+![Model visualization](https://github.com/jacquev6/lincs/raw/v0.3.1/model.png)
 
 And finally generate a set of classified alternatives (@todo Link to concepts and file formats):
 
 <!-- EXTEND command-line-example/run.sh -->
     lincs generate classified-alternatives domain.yml model.yml 1000 --output-classified-alternatives learning-set.csv
 <!-- APPEND-TO-LAST-LINE --random-seed 42 -->
 <!-- STOP -->
@@ -302,15 +302,15 @@
 <!-- STOP -->
 <!-- EXTEND command-line-example/run.sh --><!--
     cp alternatives.png ../../..
 --><!-- STOP -->
 
 It should output something like:
 
-![Alternatives visualization](https://github.com/jacquev6/lincs/raw/v0.3.0/alternatives.png)
+![Alternatives visualization](https://github.com/jacquev6/lincs/raw/v0.3.1/alternatives.png)
 
 @todo Improve how this graph looks:
 
 - display categories as stacked solid colors
 - display alternatives in a color that matches their assigned category
 - remove the legend, place names (categories and alternatives) directly on the graph
```

### Comparing `lincs-0.3.0/README.md` & `lincs-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `lincs-0.3.0/lincs/__init__.py` & `lincs-0.3.1/lincs/__init__.py`

 * *Files identical despite different names*

### Comparing `lincs-0.3.0/lincs/command_line_interface.py` & `lincs-0.3.1/lincs/command_line_interface.py`

 * *Files identical despite different names*

### Comparing `lincs-0.3.0/lincs/liblincs/classification.cpp` & `lincs-0.3.1/lincs/liblincs/classification.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.0/lincs/liblincs/generation.cpp` & `lincs-0.3.1/lincs/liblincs/generation.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.0/lincs/liblincs/io.cpp` & `lincs-0.3.1/lincs/liblincs/io.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.0/lincs/liblincs/learning.cpp` & `lincs-0.3.1/lincs/liblincs/learning.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.0/lincs/liblincs/liblincs_module.cpp` & `lincs-0.3.1/lincs/liblincs/liblincs_module.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.0/lincs/liblincs/lincs.hpp` & `lincs-0.3.1/lincs/liblincs/lincs.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.0/lincs/liblincs/median-and-max.cpp` & `lincs-0.3.1/lincs/liblincs/median-and-max.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.0/lincs/liblincs/randomness-utils.cpp` & `lincs-0.3.1/lincs/liblincs/randomness-utils.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.0/lincs/liblincs/randomness-utils.hpp` & `lincs-0.3.1/lincs/liblincs/randomness-utils.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.0/lincs/liblincs_module_tests.py` & `lincs-0.3.1/lincs/liblincs_module_tests.py`

 * *Files identical despite different names*

### Comparing `lincs-0.3.0/lincs/visualization.py` & `lincs-0.3.1/lincs/visualization.py`

 * *Files identical despite different names*

### Comparing `lincs-0.3.0/lincs.egg-info/PKG-INFO` & `lincs-0.3.1/lincs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincs
-Version: 0.3.0
+Version: 0.3.1
 Summary: MCDA algorithms
 Home-page: https://github.com/jacquev6/lincs
 Author: Vincent Jacques
 Author-email: vincent@vincent-jacques.net
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -267,15 +267,15 @@
 <!-- STOP -->
 <!-- EXTEND command-line-example/run.sh --><!--
     cp model.png ../../..
 --><!-- STOP -->
 
 It should output something like:
 
-![Model visualization](https://github.com/jacquev6/lincs/raw/v0.3.0/model.png)
+![Model visualization](https://github.com/jacquev6/lincs/raw/v0.3.1/model.png)
 
 And finally generate a set of classified alternatives (@todo Link to concepts and file formats):
 
 <!-- EXTEND command-line-example/run.sh -->
     lincs generate classified-alternatives domain.yml model.yml 1000 --output-classified-alternatives learning-set.csv
 <!-- APPEND-TO-LAST-LINE --random-seed 42 -->
 <!-- STOP -->
@@ -302,15 +302,15 @@
 <!-- STOP -->
 <!-- EXTEND command-line-example/run.sh --><!--
     cp alternatives.png ../../..
 --><!-- STOP -->
 
 It should output something like:
 
-![Alternatives visualization](https://github.com/jacquev6/lincs/raw/v0.3.0/alternatives.png)
+![Alternatives visualization](https://github.com/jacquev6/lincs/raw/v0.3.1/alternatives.png)
 
 @todo Improve how this graph looks:
 
 - display categories as stacked solid colors
 - display alternatives in a color that matches their assigned category
 - remove the legend, place names (categories and alternatives) directly on the graph
```

### Comparing `lincs-0.3.0/lincs.egg-info/SOURCES.txt` & `lincs-0.3.1/lincs.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -16,9 +16,10 @@
 lincs/liblincs/classification.cpp
 lincs/liblincs/generation.cpp
 lincs/liblincs/io.cpp
 lincs/liblincs/learning.cpp
 lincs/liblincs/liblincs_module.cpp
 lincs/liblincs/lincs.hpp
 lincs/liblincs/median-and-max.cpp
+lincs/liblincs/median-and-max.hpp
 lincs/liblincs/randomness-utils.cpp
 lincs/liblincs/randomness-utils.hpp
```

### Comparing `lincs-0.3.0/setup.py` & `lincs-0.3.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import glob
 import setuptools
 
 
-version = "0.3.0"
+version = "0.3.1"
 
 with open("README.md") as f:
     long_description = f.read()
 for image in ["model", "alternatives"]:
     long_description = long_description.replace(f"]({image}.png)", f"](https://github.com/jacquev6/lincs/raw/v{version}/{image}.png)")
 
 with open("requirements.txt") as f:
@@ -14,23 +15,15 @@
 
 # @todo Consider using scikit-build:
 # it should make it easier to compile CUDA code using nvcc and to run C++ unit tests during build.
 # Note that pybind11 comes with an example of building using scikit-build.
 # (see also https://www.benjack.io/hybrid-python/c-packages-revisited/)
 liblincs = setuptools.Extension(
     "liblincs",
-    sources=[
-        "lincs/liblincs/liblincs_module.cpp",
-        "lincs/liblincs/classification.cpp",
-        "lincs/liblincs/generation.cpp",
-        "lincs/liblincs/io.cpp",
-        "lincs/liblincs/learning.cpp",
-        "lincs/liblincs/median-and-max.cpp",
-        "lincs/liblincs/randomness-utils.cpp",
-    ],
+    sources=glob.glob("lincs/liblincs/**/*.cpp", recursive=True),
     libraries=[
         "boost_python310",
         "ortools",
         "python3.10",  # Make the Python module usable as a C++ shared library without -lpython3.10 (still linked, but implicitly)
         "yaml-cpp",
     ],
     define_macros=[("DOCTEST_CONFIG_DISABLE", None)],
```


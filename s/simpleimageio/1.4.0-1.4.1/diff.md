# Comparing `tmp/simpleimageio-1.4.0.tar.gz` & `tmp/simpleimageio-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleimageio-1.4.0.tar", last modified: Thu May 11 10:57:38 2023, max compression
+gzip compressed data, was "simpleimageio-1.4.1.tar", last modified: Fri May 12 15:26:15 2023, max compression
```

## Comparing `simpleimageio-1.4.0.tar` & `simpleimageio-1.4.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:57:38.078467 simpleimageio-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:57:38.074467 simpleimageio-1.4.0/Core/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:57:38.074467 simpleimageio-1.4.0/Core/External/
--rw-r--r--   0 runner    (1001) docker     (123)   114725 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/External/fpng.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/External/fpng.h
--rw-r--r--   0 runner    (1001) docker     (123)   319839 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/External/miniz.c
--rw-r--r--   0 runner    (1001) docker     (123)    69441 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/External/miniz.h
--rw-r--r--   0 runner    (1001) docker     (123)   273149 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/External/stb_image.h
--rw-r--r--   0 runner    (1001) docker     (123)    69564 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/External/stb_image_write.h
--rw-r--r--   0 runner    (1001) docker     (123)   163059 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/External/tiny_dng_loader.h
--rw-r--r--   0 runner    (1001) docker     (123)    38477 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/External/tiny_dng_writer.h
--rw-r--r--   0 runner    (1001) docker     (123)   269883 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/External/tinyexr.h
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/error_metrics.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11082 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/filter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/image.h
--rw-r--r--   0 runner    (1001) docker     (123)    34881 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/imageio.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/manipulation.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/tonemapping.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/Core/vec3.h
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-05-11 10:57:38.078467 simpleimageio-1.4.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:57:38.070467 simpleimageio-1.4.0/PyWrapper/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:57:38.074467 simpleimageio-1.4.0/PyWrapper/simpleimageio/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/PyWrapper/simpleimageio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/PyWrapper/simpleimageio/corelib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/PyWrapper/simpleimageio/error_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/PyWrapper/simpleimageio/flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/PyWrapper/simpleimageio/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/PyWrapper/simpleimageio/manip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/PyWrapper/simpleimageio/tev.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/PyWrapper/simpleimageio/tonemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 10:57:38.078467 simpleimageio-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-11 10:57:29.000000 simpleimageio-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:57:38.078467 simpleimageio-1.4.0/simpleimageio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-05-11 10:57:38.000000 simpleimageio-1.4.0/simpleimageio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-11 10:57:38.000000 simpleimageio-1.4.0/simpleimageio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 10:57:38.000000 simpleimageio-1.4.0/simpleimageio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 10:57:38.000000 simpleimageio-1.4.0/simpleimageio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-11 10:57:38.000000 simpleimageio-1.4.0/simpleimageio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:26:15.948130 simpleimageio-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-12 15:25:46.000000 simpleimageio-1.4.1/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:26:15.940130 simpleimageio-1.4.1/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-12 15:25:46.000000 simpleimageio-1.4.1/Core/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:26:15.944130 simpleimageio-1.4.1/Core/External/
+-rw-r--r--   0 runner    (1001) docker     (123)   114725 2023-05-12 15:25:46.000000 simpleimageio-1.4.1/Core/External/fpng.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-05-12 15:25:46.000000 simpleimageio-1.4.1/Core/External/fpng.h
+-rw-r--r--   0 runner    (1001) docker     (123)   319839 2023-05-12 15:25:46.000000 simpleimageio-1.4.1/Core/External/miniz.c
+-rw-r--r--   0 runner    (1001) docker     (123)    69441 2023-05-12 15:25:46.000000 simpleimageio-1.4.1/Core/External/miniz.h
+-rw-r--r--   0 runner    (1001) docker     (123)   273149 2023-05-12 15:25:46.000000 simpleimageio-1.4.1/Core/External/stb_image.h
+-rw-r--r--   0 runner    (1001) docker     (123)    69564 2023-05-12 15:25:46.000000 simpleimageio-1.4.1/Core/External/stb_image_write.h
+-rw-r--r--   0 runner    (1001) docker     (123)   163059 2023-05-12 15:25:46.000000 simpleimageio-1.4.1/Core/External/tiny_dng_loader.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38477 2023-05-12 15:25:46.000000 simpleimageio-1.4.1/Core/External/tiny_dng_writer.h
+-rw-r--r--   0 runner    (1001) docker     (123)   269883 2023-05-12 15:25:46.000000 simpleimageio-1.4.1/Core/External/tinyexr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-05-12 15:25:46.000000 simpleimageio-1.4.1/Core/error_metrics.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11082 2023-05-12 15:25:46.000000 simpleimageio-1.4.1/Core/filter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-12 15:25:46.000000 simpleimageio-1.4.1/Core/image.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34881 2023-05-12 15:25:46.000000 simpleimageio-1.4.1/Core/imageio.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-12 15:25:46.000000 simpleimageio-1.4.1/Core/manipulation.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-12 15:25:46.000000 simpleimageio-1.4.1/Core/tonemapping.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-12 15:25:46.000000 simpleimageio-1.4.1/Core/vec3.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-12 15:25:46.000000 simpleimageio-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-12 15:25:46.000000 simpleimageio-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-05-12 15:26:15.948130 simpleimageio-1.4.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:26:15.936130 simpleimageio-1.4.1/PyWrapper/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:26:15.948130 simpleimageio-1.4.1/PyWrapper/simpleimageio/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-12 15:25:47.000000 simpleimageio-1.4.1/PyWrapper/simpleimageio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-12 15:25:47.000000 simpleimageio-1.4.1/PyWrapper/simpleimageio/corelib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-12 15:25:47.000000 simpleimageio-1.4.1/PyWrapper/simpleimageio/error_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-12 15:25:47.000000 simpleimageio-1.4.1/PyWrapper/simpleimageio/flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)   207155 2023-05-12 15:26:03.000000 simpleimageio-1.4.1/PyWrapper/simpleimageio/flipbook.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-05-12 15:25:47.000000 simpleimageio-1.4.1/PyWrapper/simpleimageio/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-12 15:25:47.000000 simpleimageio-1.4.1/PyWrapper/simpleimageio/manip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-12 15:25:47.000000 simpleimageio-1.4.1/PyWrapper/simpleimageio/tev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-12 15:25:47.000000 simpleimageio-1.4.1/PyWrapper/simpleimageio/tonemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-05-12 15:25:47.000000 simpleimageio-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-12 15:25:47.000000 simpleimageio-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 15:26:15.948130 simpleimageio-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-12 15:25:47.000000 simpleimageio-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:26:15.948130 simpleimageio-1.4.1/simpleimageio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-05-12 15:26:15.000000 simpleimageio-1.4.1/simpleimageio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-12 15:26:15.000000 simpleimageio-1.4.1/simpleimageio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:26:15.000000 simpleimageio-1.4.1/simpleimageio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-12 15:26:15.000000 simpleimageio-1.4.1/simpleimageio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-12 15:26:15.000000 simpleimageio-1.4.1/simpleimageio.egg-info/top_level.txt
```

### Comparing `simpleimageio-1.4.0/Core/CMakeLists.txt` & `simpleimageio-1.4.1/Core/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.4.0/Core/External/fpng.cpp` & `simpleimageio-1.4.1/Core/External/fpng.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.4.0/Core/External/fpng.h` & `simpleimageio-1.4.1/Core/External/fpng.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.4.0/Core/External/miniz.c` & `simpleimageio-1.4.1/Core/External/miniz.c`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.4.0/Core/External/miniz.h` & `simpleimageio-1.4.1/Core/External/miniz.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.4.0/Core/External/stb_image.h` & `simpleimageio-1.4.1/Core/External/stb_image.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.4.0/Core/External/stb_image_write.h` & `simpleimageio-1.4.1/Core/External/stb_image_write.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.4.0/Core/External/tiny_dng_loader.h` & `simpleimageio-1.4.1/Core/External/tiny_dng_loader.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.4.0/Core/External/tiny_dng_writer.h` & `simpleimageio-1.4.1/Core/External/tiny_dng_writer.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.4.0/Core/External/tinyexr.h` & `simpleimageio-1.4.1/Core/External/tinyexr.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.4.0/Core/error_metrics.cpp` & `simpleimageio-1.4.1/Core/error_metrics.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.4.0/Core/filter.cpp` & `simpleimageio-1.4.1/Core/filter.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.4.0/Core/image.h` & `simpleimageio-1.4.1/Core/image.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.4.0/Core/imageio.cpp` & `simpleimageio-1.4.1/Core/imageio.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.4.0/Core/manipulation.cpp` & `simpleimageio-1.4.1/Core/manipulation.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.4.0/Core/tonemapping.cpp` & `simpleimageio-1.4.1/Core/tonemapping.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.4.0/Core/vec3.h` & `simpleimageio-1.4.1/Core/vec3.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.4.0/LICENSE` & `simpleimageio-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.4.0/PKG-INFO` & `simpleimageio-1.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleimageio
-Version: 1.4.0
+Version: 1.4.1
 Summary: A very simple Python wrapper to read and write various HDR and LDR image file formats.
 Home-page: https://github.com/pgrit/SimpleImageIO
 Author: Pascal Grittmann
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -154,29 +154,35 @@
 
 Note that, currently, Open Image Denoise is included in binary from. The `Denoiser` class can therefore not be used on platforms other than x86-64 Windows, Linux, or macOS. Attempting to use it on other platforms will cause a `DllNotFound` exception.
 
 Then, you should be able to follow the steps above and proceed as usual.
 
 ### Building the Python wrapper
 
-Simply running:
+The simplest route is to run the build script
 
 ```
-python -m build
+pwsh ./make.ps1
 ```
 
-will automatically fetch an adequate version of CMake, compile the shared library, and build
-the Python package.
-You can then simply install the result via:
+which builds and installs the Python lib with pip, using whatever `python` executable is currently in the path.
 
+If you need manual control, e.g., specific Python version, here are the required steps:
 ```
-pip install ./dist/simpleimageio-*.whl
+cd ./FlipViewer
+npm install
+npm run build
+cd ..
+cp ./FlipViewer/dist/flipbook.js PyWrapper/simpleimageio/flipbook.js
+
+python -m build
+python -m pip install ./dist/simpleimageio-*.whl
 ```
 
-Where the * has to be substituted by the version number and the compiler and platform identifier (use auto-complete).
+The first commands build, bundle, and pack the frontend code. Then, we build the Python package itself and install it via pip. The `*` must be substituted by the correct version number and runtime identifier.
 
 The tests can be run via:
 
 ```
 cd PyTest
 python -m unittest
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: simpleimageio Version: 1.4.0 Summary: A very simple
+Metadata-Version: 2.1 Name: simpleimageio Version: 1.4.1 Summary: A very simple
 Python wrapper to read and write various HDR and LDR image file formats. Home-
 page: https://github.com/pgrit/SimpleImageIO Author: Pascal Grittmann
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE ![Build](https://github.com/pgrit/SimpleImageIO/workflows/Build/
 badge.svg) [https://buildstats.info/nuget/SimpleImageIO] # Simple Image IO A
@@ -104,13 +104,17 @@
 to the .csproj file. You can find the right RID for your platform here: [https:
 //docs.microsoft.com/en-us/dotnet/core/rid-catalog](https://docs.microsoft.com/
 en-us/dotnet/core/rid-catalog). Note that, currently, Open Image Denoise is
 included in binary from. The `Denoiser` class can therefore not be used on
 platforms other than x86-64 Windows, Linux, or macOS. Attempting to use it on
 other platforms will cause a `DllNotFound` exception. Then, you should be able
 to follow the steps above and proceed as usual. ### Building the Python wrapper
-Simply running: ``` python -m build ``` will automatically fetch an adequate
-version of CMake, compile the shared library, and build the Python package. You
-can then simply install the result via: ``` pip install ./dist/simpleimageio-
-*.whl ``` Where the * has to be substituted by the version number and the
-compiler and platform identifier (use auto-complete). The tests can be run via:
-``` cd PyTest python -m unittest ```
+The simplest route is to run the build script ``` pwsh ./make.ps1 ``` which
+builds and installs the Python lib with pip, using whatever `python` executable
+is currently in the path. If you need manual control, e.g., specific Python
+version, here are the required steps: ``` cd ./FlipViewer npm install npm run
+build cd .. cp ./FlipViewer/dist/flipbook.js PyWrapper/simpleimageio/
+flipbook.js python -m build python -m pip install ./dist/simpleimageio-*.whl
+``` The first commands build, bundle, and pack the frontend code. Then, we
+build the Python package itself and install it via pip. The `*` must be
+substituted by the correct version number and runtime identifier. The tests can
+be run via: ``` cd PyTest python -m unittest ```
```

### Comparing `simpleimageio-1.4.0/PyWrapper/simpleimageio/corelib.py` & `simpleimageio-1.4.1/PyWrapper/simpleimageio/corelib.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.4.0/PyWrapper/simpleimageio/error_metrics.py` & `simpleimageio-1.4.1/PyWrapper/simpleimageio/error_metrics.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.4.0/PyWrapper/simpleimageio/flip.py` & `simpleimageio-1.4.1/PyWrapper/simpleimageio/flip.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.4.0/PyWrapper/simpleimageio/image.py` & `simpleimageio-1.4.1/PyWrapper/simpleimageio/image.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.4.0/PyWrapper/simpleimageio/manip.py` & `simpleimageio-1.4.1/PyWrapper/simpleimageio/manip.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.4.0/PyWrapper/simpleimageio/tev.py` & `simpleimageio-1.4.1/PyWrapper/simpleimageio/tev.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.4.0/PyWrapper/simpleimageio/tonemap.py` & `simpleimageio-1.4.1/PyWrapper/simpleimageio/tonemap.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.4.0/README.md` & `simpleimageio-1.4.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -141,29 +141,35 @@
 
 Note that, currently, Open Image Denoise is included in binary from. The `Denoiser` class can therefore not be used on platforms other than x86-64 Windows, Linux, or macOS. Attempting to use it on other platforms will cause a `DllNotFound` exception.
 
 Then, you should be able to follow the steps above and proceed as usual.
 
 ### Building the Python wrapper
 
-Simply running:
+The simplest route is to run the build script
 
 ```
-python -m build
+pwsh ./make.ps1
 ```
 
-will automatically fetch an adequate version of CMake, compile the shared library, and build
-the Python package.
-You can then simply install the result via:
+which builds and installs the Python lib with pip, using whatever `python` executable is currently in the path.
 
+If you need manual control, e.g., specific Python version, here are the required steps:
 ```
-pip install ./dist/simpleimageio-*.whl
+cd ./FlipViewer
+npm install
+npm run build
+cd ..
+cp ./FlipViewer/dist/flipbook.js PyWrapper/simpleimageio/flipbook.js
+
+python -m build
+python -m pip install ./dist/simpleimageio-*.whl
 ```
 
-Where the * has to be substituted by the version number and the compiler and platform identifier (use auto-complete).
+The first commands build, bundle, and pack the frontend code. Then, we build the Python package itself and install it via pip. The `*` must be substituted by the correct version number and runtime identifier.
 
 The tests can be run via:
 
 ```
 cd PyTest
 python -m unittest
 ```
```

#### html2text {}

```diff
@@ -98,13 +98,17 @@
 to the .csproj file. You can find the right RID for your platform here: [https:
 //docs.microsoft.com/en-us/dotnet/core/rid-catalog](https://docs.microsoft.com/
 en-us/dotnet/core/rid-catalog). Note that, currently, Open Image Denoise is
 included in binary from. The `Denoiser` class can therefore not be used on
 platforms other than x86-64 Windows, Linux, or macOS. Attempting to use it on
 other platforms will cause a `DllNotFound` exception. Then, you should be able
 to follow the steps above and proceed as usual. ### Building the Python wrapper
-Simply running: ``` python -m build ``` will automatically fetch an adequate
-version of CMake, compile the shared library, and build the Python package. You
-can then simply install the result via: ``` pip install ./dist/simpleimageio-
-*.whl ``` Where the * has to be substituted by the version number and the
-compiler and platform identifier (use auto-complete). The tests can be run via:
-``` cd PyTest python -m unittest ```
+The simplest route is to run the build script ``` pwsh ./make.ps1 ``` which
+builds and installs the Python lib with pip, using whatever `python` executable
+is currently in the path. If you need manual control, e.g., specific Python
+version, here are the required steps: ``` cd ./FlipViewer npm install npm run
+build cd .. cp ./FlipViewer/dist/flipbook.js PyWrapper/simpleimageio/
+flipbook.js python -m build python -m pip install ./dist/simpleimageio-*.whl
+``` The first commands build, bundle, and pack the frontend code. Then, we
+build the Python package itself and install it via pip. The `*` must be
+substituted by the correct version number and runtime identifier. The tests can
+be run via: ``` cd PyTest python -m unittest ```
```

### Comparing `simpleimageio-1.4.0/setup.py` & `simpleimageio-1.4.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,16 @@
         extdir = pathlib.Path(self.get_ext_fullpath(ext.name))
         extdir.mkdir(parents=True, exist_ok=True)
 
         # Configure CMake arguments
         config = 'Release'
         cmake_args = [
             '-DPYLIB=' + str(extdir.parent.absolute()), # destination for the shared library
-            '-DCMAKE_BUILD_TYPE=' + config
+            '-DCMAKE_BUILD_TYPE=' + config,
+            '-DCMAKE_OSX_DEPLOYMENT_TARGET=10.15'
         ]
         build_args = [ '--config', config ]
 
         # Run CMake and build (automatically copies the .dll / .so / .dylib file)
         os.chdir(str(build_temp))
         self.spawn(['cmake', str(cwd)] + cmake_args)
         if not self.dry_run:
@@ -45,15 +46,15 @@
         os.chdir(str(cwd))
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='simpleimageio',
-    version='1.4.0',
+    version='1.4.1',
     author='Pascal Grittmann',
     url='https://github.com/pgrit/SimpleImageIO',
 
     description='A very simple Python wrapper to read and write various HDR and LDR image file formats.',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `simpleimageio-1.4.0/simpleimageio.egg-info/PKG-INFO` & `simpleimageio-1.4.1/simpleimageio.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleimageio
-Version: 1.4.0
+Version: 1.4.1
 Summary: A very simple Python wrapper to read and write various HDR and LDR image file formats.
 Home-page: https://github.com/pgrit/SimpleImageIO
 Author: Pascal Grittmann
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -154,29 +154,35 @@
 
 Note that, currently, Open Image Denoise is included in binary from. The `Denoiser` class can therefore not be used on platforms other than x86-64 Windows, Linux, or macOS. Attempting to use it on other platforms will cause a `DllNotFound` exception.
 
 Then, you should be able to follow the steps above and proceed as usual.
 
 ### Building the Python wrapper
 
-Simply running:
+The simplest route is to run the build script
 
 ```
-python -m build
+pwsh ./make.ps1
 ```
 
-will automatically fetch an adequate version of CMake, compile the shared library, and build
-the Python package.
-You can then simply install the result via:
+which builds and installs the Python lib with pip, using whatever `python` executable is currently in the path.
 
+If you need manual control, e.g., specific Python version, here are the required steps:
 ```
-pip install ./dist/simpleimageio-*.whl
+cd ./FlipViewer
+npm install
+npm run build
+cd ..
+cp ./FlipViewer/dist/flipbook.js PyWrapper/simpleimageio/flipbook.js
+
+python -m build
+python -m pip install ./dist/simpleimageio-*.whl
 ```
 
-Where the * has to be substituted by the version number and the compiler and platform identifier (use auto-complete).
+The first commands build, bundle, and pack the frontend code. Then, we build the Python package itself and install it via pip. The `*` must be substituted by the correct version number and runtime identifier.
 
 The tests can be run via:
 
 ```
 cd PyTest
 python -m unittest
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: simpleimageio Version: 1.4.0 Summary: A very simple
+Metadata-Version: 2.1 Name: simpleimageio Version: 1.4.1 Summary: A very simple
 Python wrapper to read and write various HDR and LDR image file formats. Home-
 page: https://github.com/pgrit/SimpleImageIO Author: Pascal Grittmann
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE ![Build](https://github.com/pgrit/SimpleImageIO/workflows/Build/
 badge.svg) [https://buildstats.info/nuget/SimpleImageIO] # Simple Image IO A
@@ -104,13 +104,17 @@
 to the .csproj file. You can find the right RID for your platform here: [https:
 //docs.microsoft.com/en-us/dotnet/core/rid-catalog](https://docs.microsoft.com/
 en-us/dotnet/core/rid-catalog). Note that, currently, Open Image Denoise is
 included in binary from. The `Denoiser` class can therefore not be used on
 platforms other than x86-64 Windows, Linux, or macOS. Attempting to use it on
 other platforms will cause a `DllNotFound` exception. Then, you should be able
 to follow the steps above and proceed as usual. ### Building the Python wrapper
-Simply running: ``` python -m build ``` will automatically fetch an adequate
-version of CMake, compile the shared library, and build the Python package. You
-can then simply install the result via: ``` pip install ./dist/simpleimageio-
-*.whl ``` Where the * has to be substituted by the version number and the
-compiler and platform identifier (use auto-complete). The tests can be run via:
-``` cd PyTest python -m unittest ```
+The simplest route is to run the build script ``` pwsh ./make.ps1 ``` which
+builds and installs the Python lib with pip, using whatever `python` executable
+is currently in the path. If you need manual control, e.g., specific Python
+version, here are the required steps: ``` cd ./FlipViewer npm install npm run
+build cd .. cp ./FlipViewer/dist/flipbook.js PyWrapper/simpleimageio/
+flipbook.js python -m build python -m pip install ./dist/simpleimageio-*.whl
+``` The first commands build, bundle, and pack the frontend code. Then, we
+build the Python package itself and install it via pip. The `*` must be
+substituted by the correct version number and runtime identifier. The tests can
+be run via: ``` cd PyTest python -m unittest ```
```

### Comparing `simpleimageio-1.4.0/simpleimageio.egg-info/SOURCES.txt` & `simpleimageio-1.4.1/simpleimageio.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 Core/External/tiny_dng_loader.h
 Core/External/tiny_dng_writer.h
 Core/External/tinyexr.h
 PyWrapper/simpleimageio/__init__.py
 PyWrapper/simpleimageio/corelib.py
 PyWrapper/simpleimageio/error_metrics.py
 PyWrapper/simpleimageio/flip.py
+PyWrapper/simpleimageio/flipbook.js
 PyWrapper/simpleimageio/image.py
 PyWrapper/simpleimageio/manip.py
 PyWrapper/simpleimageio/tev.py
 PyWrapper/simpleimageio/tonemap.py
 simpleimageio.egg-info/PKG-INFO
 simpleimageio.egg-info/SOURCES.txt
 simpleimageio.egg-info/dependency_links.txt
```


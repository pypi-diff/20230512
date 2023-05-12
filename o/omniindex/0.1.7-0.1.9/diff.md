# Comparing `tmp/omniindex-0.1.7.tar.gz` & `tmp/omniindex-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniindex-0.1.7.tar", last modified: Wed Mar 29 10:25:27 2023, max compression
+gzip compressed data, was "omniindex-0.1.9.tar", last modified: Thu Mar 30 11:40:52 2023, max compression
```

## Comparing `omniindex-0.1.7.tar` & `omniindex-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 10:25:27.982641 omniindex-0.1.7/
--rw-rw-rw-   0        0        0     1089 2023-03-27 07:05:59.000000 omniindex-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     1813 2023-03-29 10:25:27.981642 omniindex-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1035 2023-03-29 09:47:31.000000 omniindex-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-03-29 10:25:27.956644 omniindex-0.1.7/omniindex/
--rw-rw-rw-   0        0        0       41 2023-03-28 14:55:49.000000 omniindex-0.1.7/omniindex/__init__.py
--rw-rw-rw-   0        0        0     5220 2023-03-29 10:07:16.000000 omniindex-0.1.7/omniindex/api.py
-drwxrwxrwx   0        0        0        0 2023-03-29 10:25:27.974644 omniindex-0.1.7/omniindex.egg-info/
--rw-rw-rw-   0        0        0     1813 2023-03-29 10:25:27.000000 omniindex-0.1.7/omniindex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-03-29 10:25:27.000000 omniindex-0.1.7/omniindex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 10:25:27.000000 omniindex-0.1.7/omniindex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-03-29 10:25:27.000000 omniindex-0.1.7/omniindex.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-03-29 10:25:27.000000 omniindex-0.1.7/omniindex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-29 10:25:27.983645 omniindex-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1222 2023-03-29 10:23:23.000000 omniindex-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-29 10:25:27.979642 omniindex-0.1.7/tests/
--rw-rw-rw-   0        0        0        0 2023-03-28 14:55:49.000000 omniindex-0.1.7/tests/__init__.py
--rw-rw-rw-   0        0        0     2854 2023-03-29 09:58:20.000000 omniindex-0.1.7/tests/omni_api_test.py
+drwxrwxrwx   0        0        0        0 2023-03-30 11:40:52.841394 omniindex-0.1.9/
+-rw-rw-rw-   0        0        0     1089 2023-03-27 07:05:59.000000 omniindex-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     1953 2023-03-30 11:40:52.840392 omniindex-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1175 2023-03-29 16:30:01.000000 omniindex-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-30 11:40:52.796398 omniindex-0.1.9/omniindex/
+-rw-rw-rw-   0        0        0       41 2023-03-28 14:55:49.000000 omniindex-0.1.9/omniindex/__init__.py
+-rw-rw-rw-   0        0        0     8111 2023-03-30 10:45:17.000000 omniindex-0.1.9/omniindex/api.py
+drwxrwxrwx   0        0        0        0 2023-03-30 11:40:52.832393 omniindex-0.1.9/omniindex.egg-info/
+-rw-rw-rw-   0        0        0     1953 2023-03-30 11:40:52.000000 omniindex-0.1.9/omniindex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-03-30 11:40:52.000000 omniindex-0.1.9/omniindex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-30 11:40:52.000000 omniindex-0.1.9/omniindex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-03-30 11:40:52.000000 omniindex-0.1.9/omniindex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-03-30 11:40:52.000000 omniindex-0.1.9/omniindex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-30 11:40:52.842395 omniindex-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1222 2023-03-30 11:34:29.000000 omniindex-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-30 11:40:52.837393 omniindex-0.1.9/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-28 14:55:49.000000 omniindex-0.1.9/tests/__init__.py
+-rw-rw-rw-   0        0        0     5607 2023-03-30 10:39:53.000000 omniindex-0.1.9/tests/omni_api_test.py
```

### Comparing `omniindex-0.1.7/LICENSE` & `omniindex-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `omniindex-0.1.7/README.md` & `omniindex-0.1.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ## Project description
 
 # OmniIndex Python Library
 
 The OmniIndex Python library provides convenient access to the OmniIndex API from applications written in the Python language. It includes a pre-defined set of classes for API resources that initialize themselves dynamically from API responses which makes it compatible with a wide range of versions of the OmniIndex API.
 
-You can find usage examples for the OmniIndex Python library in our [API reference](https://omniindex.readthedocs.io/)
+You can find usage examples for the OmniIndex Python library in our [Python Library reference](https://omniindex.readthedocs.io/) which includes code samples etc
+For just the [API reference](https://app.swaggerhub.com/apis-docs/OmniIndexAPI/OmniIndex/1.0.0)
 
 ## Installation
 
 You don't need this source code unless you want to modify the package. If you just want to use the package, just run:
 
 ```bash
 pip install --upgrade omniindex
```

### Comparing `omniindex-0.1.7/setup.py` & `omniindex-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from os import path
 
 # The directory containing this file
 HERE = path.abspath(path.dirname(__file__))
 
 setup(
     name="omniindex",
-    version="0.1.7",
+    version="0.1.9",
     packages=find_packages(),
     install_requires=[
         "requests",
     ],
     include_package_data=True,
     author="James Stanbridge",
     author_email="james@omniindex.io",
```


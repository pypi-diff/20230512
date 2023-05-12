# Comparing `tmp/pythoncoloringspkgV2-1.0.0.tar.gz` & `tmp/pythoncoloringspkgV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythoncoloringspkgV2-1.0.0.tar", last modified: Fri May 12 18:08:42 2023, max compression
+gzip compressed data, was "pythoncoloringspkgV2-1.1.0.tar", last modified: Fri May 12 18:10:47 2023, max compression
```

## Comparing `pythoncoloringspkgV2-1.0.0.tar` & `pythoncoloringspkgV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 18:08:42.221026 pythoncoloringspkgV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      353 2023-05-12 18:08:42.221026 pythoncoloringspkgV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 18:08:42.221026 pythoncoloringspkgV2-1.0.0/pythoncoloringspkgV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-12 18:08:41.000000 pythoncoloringspkgV2-1.0.0/pythoncoloringspkgV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 18:08:42.221026 pythoncoloringspkgV2-1.0.0/pythoncoloringspkgV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      353 2023-05-12 18:08:42.000000 pythoncoloringspkgV2-1.0.0/pythoncoloringspkgV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      217 2023-05-12 18:08:42.000000 pythoncoloringspkgV2-1.0.0/pythoncoloringspkgV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 18:08:42.000000 pythoncoloringspkgV2-1.0.0/pythoncoloringspkgV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-12 18:08:42.000000 pythoncoloringspkgV2-1.0.0/pythoncoloringspkgV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 18:08:42.221026 pythoncoloringspkgV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      566 2023-05-12 18:08:41.000000 pythoncoloringspkgV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 18:10:47.663670 pythoncoloringspkgV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-05-12 18:10:47.663670 pythoncoloringspkgV2-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 18:10:47.663670 pythoncoloringspkgV2-1.1.0/pythoncoloringspkgV2/
+-rw-r--r--   0 root         (0) root         (0)    97161 2023-05-12 18:10:47.000000 pythoncoloringspkgV2-1.1.0/pythoncoloringspkgV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 18:10:47.663670 pythoncoloringspkgV2-1.1.0/pythoncoloringspkgV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-05-12 18:10:47.000000 pythoncoloringspkgV2-1.1.0/pythoncoloringspkgV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      217 2023-05-12 18:10:47.000000 pythoncoloringspkgV2-1.1.0/pythoncoloringspkgV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 18:10:47.000000 pythoncoloringspkgV2-1.1.0/pythoncoloringspkgV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-12 18:10:47.000000 pythoncoloringspkgV2-1.1.0/pythoncoloringspkgV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 18:10:47.663670 pythoncoloringspkgV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      566 2023-05-12 18:10:47.000000 pythoncoloringspkgV2-1.1.0/setup.py
```

### Comparing `pythoncoloringspkgV2-1.0.0/setup.py` & `pythoncoloringspkgV2-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pythoncoloringspkgV2",
     version=VERSION,
```


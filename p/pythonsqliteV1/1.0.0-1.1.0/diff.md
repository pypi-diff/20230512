# Comparing `tmp/pythonsqliteV1-1.0.0.tar.gz` & `tmp/pythonsqliteV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonsqliteV1-1.0.0.tar", last modified: Fri May 12 19:40:58 2023, max compression
+gzip compressed data, was "pythonsqliteV1-1.1.0.tar", last modified: Fri May 12 19:43:03 2023, max compression
```

## Comparing `pythonsqliteV1-1.0.0.tar` & `pythonsqliteV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:40:58.191889 pythonsqliteV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      347 2023-05-12 19:40:58.191889 pythonsqliteV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:40:58.191889 pythonsqliteV1-1.0.0/pythonsqliteV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-12 19:40:57.000000 pythonsqliteV1-1.0.0/pythonsqliteV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:40:58.191889 pythonsqliteV1-1.0.0/pythonsqliteV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      347 2023-05-12 19:40:58.000000 pythonsqliteV1-1.0.0/pythonsqliteV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      187 2023-05-12 19:40:58.000000 pythonsqliteV1-1.0.0/pythonsqliteV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 19:40:58.000000 pythonsqliteV1-1.0.0/pythonsqliteV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-12 19:40:58.000000 pythonsqliteV1-1.0.0/pythonsqliteV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 19:40:58.191889 pythonsqliteV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      560 2023-05-12 19:40:57.000000 pythonsqliteV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:43:03.082436 pythonsqliteV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-05-12 19:43:03.082436 pythonsqliteV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:43:03.082436 pythonsqliteV1-1.1.0/pythonsqliteV1/
+-rw-r--r--   0 root         (0) root         (0)    97161 2023-05-12 19:43:02.000000 pythonsqliteV1-1.1.0/pythonsqliteV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:43:03.082436 pythonsqliteV1-1.1.0/pythonsqliteV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-05-12 19:43:03.000000 pythonsqliteV1-1.1.0/pythonsqliteV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      187 2023-05-12 19:43:03.000000 pythonsqliteV1-1.1.0/pythonsqliteV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 19:43:03.000000 pythonsqliteV1-1.1.0/pythonsqliteV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-12 19:43:03.000000 pythonsqliteV1-1.1.0/pythonsqliteV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 19:43:03.082436 pythonsqliteV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      560 2023-05-12 19:43:02.000000 pythonsqliteV1-1.1.0/setup.py
```

### Comparing `pythonsqliteV1-1.0.0/setup.py` & `pythonsqliteV1-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pythonsqliteV1",
     version=VERSION,
```


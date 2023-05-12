# Comparing `tmp/syscoloringaddons-1.0.0.tar.gz` & `tmp/syscoloringaddons-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syscoloringaddons-1.0.0.tar", last modified: Fri May 12 18:26:13 2023, max compression
+gzip compressed data, was "syscoloringaddons-1.1.0.tar", last modified: Fri May 12 18:28:20 2023, max compression
```

## Comparing `syscoloringaddons-1.0.0.tar` & `syscoloringaddons-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 18:26:13.398186 syscoloringaddons-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      350 2023-05-12 18:26:13.398186 syscoloringaddons-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 18:26:13.398186 syscoloringaddons-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      563 2023-05-12 18:26:13.000000 syscoloringaddons-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 18:26:13.398186 syscoloringaddons-1.0.0/syscoloringaddons/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-12 18:26:13.000000 syscoloringaddons-1.0.0/syscoloringaddons/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 18:26:13.398186 syscoloringaddons-1.0.0/syscoloringaddons.egg-info/
--rw-r--r--   0 root         (0) root         (0)      350 2023-05-12 18:26:13.000000 syscoloringaddons-1.0.0/syscoloringaddons.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      202 2023-05-12 18:26:13.000000 syscoloringaddons-1.0.0/syscoloringaddons.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 18:26:13.000000 syscoloringaddons-1.0.0/syscoloringaddons.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-12 18:26:13.000000 syscoloringaddons-1.0.0/syscoloringaddons.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 18:28:20.312864 syscoloringaddons-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-05-12 18:28:20.312864 syscoloringaddons-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 18:28:20.312864 syscoloringaddons-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      563 2023-05-12 18:28:20.000000 syscoloringaddons-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 18:28:20.312864 syscoloringaddons-1.1.0/syscoloringaddons/
+-rw-r--r--   0 root         (0) root         (0)    97161 2023-05-12 18:28:20.000000 syscoloringaddons-1.1.0/syscoloringaddons/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 18:28:20.312864 syscoloringaddons-1.1.0/syscoloringaddons.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-05-12 18:28:20.000000 syscoloringaddons-1.1.0/syscoloringaddons.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      202 2023-05-12 18:28:20.000000 syscoloringaddons-1.1.0/syscoloringaddons.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 18:28:20.000000 syscoloringaddons-1.1.0/syscoloringaddons.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-12 18:28:20.000000 syscoloringaddons-1.1.0/syscoloringaddons.egg-info/top_level.txt
```

### Comparing `syscoloringaddons-1.0.0/setup.py` & `syscoloringaddons-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="syscoloringaddons",
     version=VERSION,
```


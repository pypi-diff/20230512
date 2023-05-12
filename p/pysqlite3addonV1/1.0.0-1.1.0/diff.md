# Comparing `tmp/pysqlite3addonV1-1.0.0.tar.gz` & `tmp/pysqlite3addonV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysqlite3addonV1-1.0.0.tar", last modified: Fri May 12 21:23:27 2023, max compression
+gzip compressed data, was "pysqlite3addonV1-1.1.0.tar", last modified: Fri May 12 21:25:32 2023, max compression
```

## Comparing `pysqlite3addonV1-1.0.0.tar` & `pysqlite3addonV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:23:27.558711 pysqlite3addonV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      349 2023-05-12 21:23:27.558711 pysqlite3addonV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:23:27.558711 pysqlite3addonV1-1.0.0/pysqlite3addonV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-12 21:23:27.000000 pysqlite3addonV1-1.0.0/pysqlite3addonV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:23:27.558711 pysqlite3addonV1-1.0.0/pysqlite3addonV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      349 2023-05-12 21:23:27.000000 pysqlite3addonV1-1.0.0/pysqlite3addonV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-12 21:23:27.000000 pysqlite3addonV1-1.0.0/pysqlite3addonV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 21:23:27.000000 pysqlite3addonV1-1.0.0/pysqlite3addonV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-12 21:23:27.000000 pysqlite3addonV1-1.0.0/pysqlite3addonV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 21:23:27.558711 pysqlite3addonV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      562 2023-05-12 21:23:27.000000 pysqlite3addonV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:25:32.513614 pysqlite3addonV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-05-12 21:25:32.513614 pysqlite3addonV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:25:32.513614 pysqlite3addonV1-1.1.0/pysqlite3addonV1/
+-rw-r--r--   0 root         (0) root         (0)    97161 2023-05-12 21:25:32.000000 pysqlite3addonV1-1.1.0/pysqlite3addonV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:25:32.513614 pysqlite3addonV1-1.1.0/pysqlite3addonV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-05-12 21:25:32.000000 pysqlite3addonV1-1.1.0/pysqlite3addonV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      197 2023-05-12 21:25:32.000000 pysqlite3addonV1-1.1.0/pysqlite3addonV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 21:25:32.000000 pysqlite3addonV1-1.1.0/pysqlite3addonV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-12 21:25:32.000000 pysqlite3addonV1-1.1.0/pysqlite3addonV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 21:25:32.513614 pysqlite3addonV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      562 2023-05-12 21:25:32.000000 pysqlite3addonV1-1.1.0/setup.py
```

### Comparing `pysqlite3addonV1-1.0.0/setup.py` & `pysqlite3addonV1-1.1.0/setup.py`

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
     name="pysqlite3addonV1",
     version=VERSION,
```


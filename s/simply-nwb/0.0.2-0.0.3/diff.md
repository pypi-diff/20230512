# Comparing `tmp/simply_nwb-0.0.2.tar.gz` & `tmp/simply_nwb-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simply_nwb-0.0.2.tar", last modified: Fri May 12 16:25:41 2023, max compression
+gzip compressed data, was "simply_nwb-0.0.3.tar", last modified: Fri May 12 16:34:26 2023, max compression
```

## Comparing `simply_nwb-0.0.2.tar` & `simply_nwb-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 16:25:41.722238 simply_nwb-0.0.2/
--rw-rw-rw-   0        0        0      494 2023-05-12 16:25:41.721245 simply_nwb-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-05-10 16:56:33.000000 simply_nwb-0.0.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-05-12 16:25:41.722238 simply_nwb-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      762 2023-05-12 16:04:18.000000 simply_nwb-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-12 16:25:41.707481 simply_nwb-0.0.2/simply_nwb/
--rw-rw-rw-   0        0        0       35 2023-05-10 18:53:16.000000 simply_nwb-0.0.2/simply_nwb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 16:25:41.715460 simply_nwb-0.0.2/simply_nwb/acquisition/
--rw-rw-rw-   0        0        0        0 2023-05-11 17:12:45.000000 simply_nwb-0.0.2/simply_nwb/acquisition/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 16:25:41.718452 simply_nwb-0.0.2/simply_nwb/acquisition/tools/
--rw-rw-rw-   0        0        0       50 2023-05-10 20:47:41.000000 simply_nwb-0.0.2/simply_nwb/acquisition/tools/__init__.py
--rw-rw-rw-   0        0        0     2971 2023-05-10 17:46:16.000000 simply_nwb-0.0.2/simply_nwb/acquisition/tools/blackrock.py
--rw-rw-rw-   0        0        0     3831 2023-05-11 16:28:17.000000 simply_nwb-0.0.2/simply_nwb/acquisition/tools/p_erg.py
--rw-rw-rw-   0        0        0      436 2023-05-12 15:44:54.000000 simply_nwb-0.0.2/simply_nwb/nwb_inspect_script.py
--rw-rw-rw-   0        0        0    11191 2023-05-12 15:49:58.000000 simply_nwb-0.0.2/simply_nwb/simple_nwb.py
--rw-rw-rw-   0        0        0     3774 2023-05-12 15:53:16.000000 simply_nwb-0.0.2/simply_nwb/testing.py
-drwxrwxrwx   0        0        0        0 2023-05-12 16:25:41.720446 simply_nwb-0.0.2/simply_nwb/transforms/
--rw-rw-rw-   0        0        0        0 2023-05-10 16:49:20.000000 simply_nwb-0.0.2/simply_nwb/transforms/__init__.py
--rw-rw-rw-   0        0        0     2026 2023-05-12 15:44:54.000000 simply_nwb-0.0.2/simply_nwb/util.py
-drwxrwxrwx   0        0        0        0 2023-05-12 16:25:41.714462 simply_nwb-0.0.2/simply_nwb.egg-info/
--rw-rw-rw-   0        0        0      494 2023-05-12 16:25:41.000000 simply_nwb-0.0.2/simply_nwb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-05-12 16:25:41.000000 simply_nwb-0.0.2/simply_nwb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 16:25:41.000000 simply_nwb-0.0.2/simply_nwb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-05-12 16:25:41.000000 simply_nwb-0.0.2/simply_nwb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-12 16:25:41.000000 simply_nwb-0.0.2/simply_nwb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 16:34:26.801905 simply_nwb-0.0.3/
+-rw-rw-rw-   0        0        0      494 2023-05-12 16:34:26.800908 simply_nwb-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-05-10 16:56:33.000000 simply_nwb-0.0.3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-05-12 16:34:26.801905 simply_nwb-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      762 2023-05-12 16:26:57.000000 simply_nwb-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 16:34:26.788162 simply_nwb-0.0.3/simply_nwb/
+-rw-rw-rw-   0        0        0       35 2023-05-10 18:53:16.000000 simply_nwb-0.0.3/simply_nwb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 16:34:26.794921 simply_nwb-0.0.3/simply_nwb/acquisition/
+-rw-rw-rw-   0        0        0        0 2023-05-11 17:12:45.000000 simply_nwb-0.0.3/simply_nwb/acquisition/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 16:34:26.798910 simply_nwb-0.0.3/simply_nwb/acquisition/tools/
+-rw-rw-rw-   0        0        0       50 2023-05-10 20:47:41.000000 simply_nwb-0.0.3/simply_nwb/acquisition/tools/__init__.py
+-rw-rw-rw-   0        0        0     2971 2023-05-10 17:46:16.000000 simply_nwb-0.0.3/simply_nwb/acquisition/tools/blackrock.py
+-rw-rw-rw-   0        0        0     3831 2023-05-11 16:28:17.000000 simply_nwb-0.0.3/simply_nwb/acquisition/tools/p_erg.py
+-rw-rw-rw-   0        0        0      436 2023-05-12 15:44:54.000000 simply_nwb-0.0.3/simply_nwb/nwb_inspect_script.py
+-rw-rw-rw-   0        0        0    11191 2023-05-12 15:49:58.000000 simply_nwb-0.0.3/simply_nwb/simple_nwb.py
+-rw-rw-rw-   0        0        0     3774 2023-05-12 15:53:16.000000 simply_nwb-0.0.3/simply_nwb/testing.py
+drwxrwxrwx   0        0        0        0 2023-05-12 16:34:26.799914 simply_nwb-0.0.3/simply_nwb/transforms/
+-rw-rw-rw-   0        0        0        0 2023-05-10 16:49:20.000000 simply_nwb-0.0.3/simply_nwb/transforms/__init__.py
+-rw-rw-rw-   0        0        0     2026 2023-05-12 15:44:54.000000 simply_nwb-0.0.3/simply_nwb/util.py
+drwxrwxrwx   0        0        0        0 2023-05-12 16:34:26.793923 simply_nwb-0.0.3/simply_nwb.egg-info/
+-rw-rw-rw-   0        0        0      494 2023-05-12 16:34:26.000000 simply_nwb-0.0.3/simply_nwb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-05-12 16:34:26.000000 simply_nwb-0.0.3/simply_nwb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 16:34:26.000000 simply_nwb-0.0.3/simply_nwb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-05-12 16:34:26.000000 simply_nwb-0.0.3/simply_nwb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-12 16:34:26.000000 simply_nwb-0.0.3/simply_nwb.egg-info/top_level.txt
```

### Comparing `simply_nwb-0.0.2/setup.py` & `simply_nwb-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 
 
 def parse_requirements(requirement_file):
     with open(requirement_file) as fi:
         return fi.readlines()
```

### Comparing `simply_nwb-0.0.2/simply_nwb/acquisition/tools/blackrock.py` & `simply_nwb-0.0.3/simply_nwb/acquisition/tools/blackrock.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.2/simply_nwb/acquisition/tools/p_erg.py` & `simply_nwb-0.0.3/simply_nwb/acquisition/tools/p_erg.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.2/simply_nwb/simple_nwb.py` & `simply_nwb-0.0.3/simply_nwb/simple_nwb.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.2/simply_nwb/testing.py` & `simply_nwb-0.0.3/simply_nwb/testing.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.2/simply_nwb/util.py` & `simply_nwb-0.0.3/simply_nwb/util.py`

 * *Files identical despite different names*


# Comparing `tmp/soda-core-vertica-3.0.34.tar.gz` & `tmp/soda-core-vertica-3.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-vertica-3.0.34.tar", last modified: Wed May 10 12:23:41 2023, max compression
+gzip compressed data, was "soda-core-vertica-3.0.36.tar", last modified: Thu May 11 22:59:47 2023, max compression
```

## Comparing `soda-core-vertica-3.0.34.tar` & `soda-core-vertica-3.0.36.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:23:41.975212 soda-core-vertica-3.0.34/
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-05-10 12:23:41.975212 soda-core-vertica-3.0.34/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-10 12:23:41.975212 soda-core-vertica-3.0.34/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      597 2023-05-10 12:22:20.000000 soda-core-vertica-3.0.34/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:23:41.975212 soda-core-vertica-3.0.34/soda/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:23:41.975212 soda-core-vertica-3.0.34/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)     7672 2023-05-10 12:22:20.000000 soda-core-vertica-3.0.34/soda/data_sources/vertica_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:23:41.975212 soda-core-vertica-3.0.34/soda_core_vertica.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-05-10 12:23:41.000000 soda-core-vertica-3.0.34/soda_core_vertica.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-10 12:23:41.000000 soda-core-vertica-3.0.34/soda_core_vertica.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 12:23:41.000000 soda-core-vertica-3.0.34/soda_core_vertica.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-10 12:23:41.000000 soda-core-vertica-3.0.34/soda_core_vertica.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-10 12:23:41.000000 soda-core-vertica-3.0.34/soda_core_vertica.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:23:41.975212 soda-core-vertica-3.0.34/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-10 12:22:20.000000 soda-core-vertica-3.0.34/tests/test_vertica.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:59:47.848021 soda-core-vertica-3.0.36/
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-05-11 22:59:47.848021 soda-core-vertica-3.0.36/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 22:59:47.848021 soda-core-vertica-3.0.36/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      597 2023-05-11 22:53:33.000000 soda-core-vertica-3.0.36/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:59:47.848021 soda-core-vertica-3.0.36/soda/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:59:47.848021 soda-core-vertica-3.0.36/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     7672 2023-05-11 22:53:33.000000 soda-core-vertica-3.0.36/soda/data_sources/vertica_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:59:47.848021 soda-core-vertica-3.0.36/soda_core_vertica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-05-11 22:59:47.000000 soda-core-vertica-3.0.36/soda_core_vertica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-11 22:59:47.000000 soda-core-vertica-3.0.36/soda_core_vertica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 22:59:47.000000 soda-core-vertica-3.0.36/soda_core_vertica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-11 22:59:47.000000 soda-core-vertica-3.0.36/soda_core_vertica.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-11 22:59:47.000000 soda-core-vertica-3.0.36/soda_core_vertica.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:59:47.848021 soda-core-vertica-3.0.36/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-11 22:53:33.000000 soda-core-vertica-3.0.36/tests/test_vertica.py
```

### Comparing `soda-core-vertica-3.0.34/setup.py` & `soda-core-vertica-3.0.36/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda Core requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-vertica"
-package_version = "3.0.34"
+package_version = "3.0.36"
 description = "Soda Core Vertica Package"
 
 requires = [f"soda-core=={package_version}", "vertica-python>=1.0.3, <2.0"]
 
 setup(
     name=package_name,
     version=package_version,
```

### Comparing `soda-core-vertica-3.0.34/soda/data_sources/vertica_data_source.py` & `soda-core-vertica-3.0.36/soda/data_sources/vertica_data_source.py`

 * *Files identical despite different names*

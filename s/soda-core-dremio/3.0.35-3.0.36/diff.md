# Comparing `tmp/soda-core-dremio-3.0.35.tar.gz` & `tmp/soda-core-dremio-3.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-dremio-3.0.35.tar", last modified: Thu May 11 22:10:09 2023, max compression
+gzip compressed data, was "soda-core-dremio-3.0.36.tar", last modified: Thu May 11 22:58:28 2023, max compression
```

## Comparing `soda-core-dremio-3.0.35.tar` & `soda-core-dremio-3.0.36.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:10:09.805009 soda-core-dremio-3.0.35/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-11 22:10:09.805009 soda-core-dremio-3.0.35/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 22:10:09.805009 soda-core-dremio-3.0.35/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-05-11 22:09:20.000000 soda-core-dremio-3.0.35/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:10:09.805009 soda-core-dremio-3.0.35/soda/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:10:09.805009 soda-core-dremio-3.0.35/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)     5458 2023-05-11 22:09:20.000000 soda-core-dremio-3.0.35/soda/data_sources/dremio_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:10:09.805009 soda-core-dremio-3.0.35/soda_core_dremio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-11 22:10:09.000000 soda-core-dremio-3.0.35/soda_core_dremio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-11 22:10:09.000000 soda-core-dremio-3.0.35/soda_core_dremio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 22:10:09.000000 soda-core-dremio-3.0.35/soda_core_dremio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-11 22:10:09.000000 soda-core-dremio-3.0.35/soda_core_dremio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-11 22:10:09.000000 soda-core-dremio-3.0.35/soda_core_dremio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:10:09.805009 soda-core-dremio-3.0.35/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-05-11 22:09:20.000000 soda-core-dremio-3.0.35/tests/test_dremio.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:58:28.811525 soda-core-dremio-3.0.36/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-11 22:58:28.811525 soda-core-dremio-3.0.36/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 22:58:28.811525 soda-core-dremio-3.0.36/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-05-11 22:53:33.000000 soda-core-dremio-3.0.36/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:58:28.811525 soda-core-dremio-3.0.36/soda/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:58:28.811525 soda-core-dremio-3.0.36/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     5458 2023-05-11 22:53:33.000000 soda-core-dremio-3.0.36/soda/data_sources/dremio_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:58:28.811525 soda-core-dremio-3.0.36/soda_core_dremio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-11 22:58:28.000000 soda-core-dremio-3.0.36/soda_core_dremio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-11 22:58:28.000000 soda-core-dremio-3.0.36/soda_core_dremio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 22:58:28.000000 soda-core-dremio-3.0.36/soda_core_dremio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-11 22:58:28.000000 soda-core-dremio-3.0.36/soda_core_dremio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-11 22:58:28.000000 soda-core-dremio-3.0.36/soda_core_dremio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:58:28.811525 soda-core-dremio-3.0.36/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-05-11 22:53:33.000000 soda-core-dremio-3.0.36/tests/test_dremio.py
```

### Comparing `soda-core-dremio-3.0.35/setup.py` & `soda-core-dremio-3.0.36/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda Core requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-dremio"
-package_version = "3.0.35"
+package_version = "3.0.36"
 description = "Soda Core Dremio Package"
 
 requires = [f"soda-core=={package_version}", "pyodbc", "pyarrow"]
 
 setup(
     name=package_name,
     version=package_version,
```

### Comparing `soda-core-dremio-3.0.35/soda/data_sources/dremio_data_source.py` & `soda-core-dremio-3.0.36/soda/data_sources/dremio_data_source.py`

 * *Files identical despite different names*


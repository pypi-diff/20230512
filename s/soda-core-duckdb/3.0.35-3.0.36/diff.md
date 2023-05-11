# Comparing `tmp/soda-core-duckdb-3.0.35.tar.gz` & `tmp/soda-core-duckdb-3.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-duckdb-3.0.35.tar", last modified: Thu May 11 22:10:16 2023, max compression
+gzip compressed data, was "soda-core-duckdb-3.0.36.tar", last modified: Thu May 11 22:58:32 2023, max compression
```

## Comparing `soda-core-duckdb-3.0.35.tar` & `soda-core-duckdb-3.0.36.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:10:16.589103 soda-core-duckdb-3.0.35/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-11 22:10:16.589103 soda-core-duckdb-3.0.35/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 22:10:16.589103 soda-core-duckdb-3.0.35/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-05-11 22:09:20.000000 soda-core-duckdb-3.0.35/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:10:16.585103 soda-core-duckdb-3.0.35/soda/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:10:16.585103 soda-core-duckdb-3.0.35/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)     5496 2023-05-11 22:09:20.000000 soda-core-duckdb-3.0.35/soda/data_sources/duckdb_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:10:16.585103 soda-core-duckdb-3.0.35/soda_core_duckdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-11 22:10:16.000000 soda-core-duckdb-3.0.35/soda_core_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-11 22:10:16.000000 soda-core-duckdb-3.0.35/soda_core_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 22:10:16.000000 soda-core-duckdb-3.0.35/soda_core_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-11 22:10:16.000000 soda-core-duckdb-3.0.35/soda_core_duckdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-11 22:10:16.000000 soda-core-duckdb-3.0.35/soda_core_duckdb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:10:16.585103 soda-core-duckdb-3.0.35/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      690 2023-05-11 22:09:20.000000 soda-core-duckdb-3.0.35/tests/test_duckdb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:58:32.591741 soda-core-duckdb-3.0.36/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-11 22:58:32.591741 soda-core-duckdb-3.0.36/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 22:58:32.591741 soda-core-duckdb-3.0.36/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-05-11 22:53:33.000000 soda-core-duckdb-3.0.36/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:58:32.591741 soda-core-duckdb-3.0.36/soda/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:58:32.591741 soda-core-duckdb-3.0.36/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     5496 2023-05-11 22:53:33.000000 soda-core-duckdb-3.0.36/soda/data_sources/duckdb_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:58:32.591741 soda-core-duckdb-3.0.36/soda_core_duckdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-11 22:58:32.000000 soda-core-duckdb-3.0.36/soda_core_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-11 22:58:32.000000 soda-core-duckdb-3.0.36/soda_core_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 22:58:32.000000 soda-core-duckdb-3.0.36/soda_core_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-11 22:58:32.000000 soda-core-duckdb-3.0.36/soda_core_duckdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-11 22:58:32.000000 soda-core-duckdb-3.0.36/soda_core_duckdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:58:32.591741 soda-core-duckdb-3.0.36/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      690 2023-05-11 22:53:33.000000 soda-core-duckdb-3.0.36/tests/test_duckdb.py
```

### Comparing `soda-core-duckdb-3.0.35/setup.py` & `soda-core-duckdb-3.0.36/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda Core requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-duckdb"
-package_version = "3.0.35"
+package_version = "3.0.36"
 description = "Soda Core Duckdb Package"
 
 requires = [f"soda-core=={package_version}", "duckdb==0.6.1"]
 
 setup(
     name=package_name,
     version=package_version,
```

### Comparing `soda-core-duckdb-3.0.35/soda/data_sources/duckdb_data_source.py` & `soda-core-duckdb-3.0.36/soda/data_sources/duckdb_data_source.py`

 * *Files identical despite different names*

### Comparing `soda-core-duckdb-3.0.35/tests/test_duckdb.py` & `soda-core-duckdb-3.0.36/tests/test_duckdb.py`

 * *Files identical despite different names*


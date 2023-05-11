# Comparing `tmp/soda-core-oracle-3.0.35.tar.gz` & `tmp/soda-core-oracle-3.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-oracle-3.0.35.tar", last modified: Thu May 11 22:11:26 2023, max compression
+gzip compressed data, was "soda-core-oracle-3.0.36.tar", last modified: Thu May 11 22:59:00 2023, max compression
```

## Comparing `soda-core-oracle-3.0.35.tar` & `soda-core-oracle-3.0.36.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:11:26.450020 soda-core-oracle-3.0.35/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-11 22:11:26.450020 soda-core-oracle-3.0.35/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 22:11:26.450020 soda-core-oracle-3.0.35/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-05-11 22:09:20.000000 soda-core-oracle-3.0.35/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:11:26.450020 soda-core-oracle-3.0.35/soda/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:11:26.450020 soda-core-oracle-3.0.35/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)     9209 2023-05-11 22:09:20.000000 soda-core-oracle-3.0.35/soda/data_sources/oracle_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:11:26.450020 soda-core-oracle-3.0.35/soda_core_oracle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-11 22:11:26.000000 soda-core-oracle-3.0.35/soda_core_oracle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-11 22:11:26.000000 soda-core-oracle-3.0.35/soda_core_oracle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 22:11:26.000000 soda-core-oracle-3.0.35/soda_core_oracle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-11 22:11:26.000000 soda-core-oracle-3.0.35/soda_core_oracle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-11 22:11:26.000000 soda-core-oracle-3.0.35/soda_core_oracle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:59:00.225320 soda-core-oracle-3.0.36/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-11 22:59:00.225320 soda-core-oracle-3.0.36/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 22:59:00.225320 soda-core-oracle-3.0.36/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-05-11 22:53:33.000000 soda-core-oracle-3.0.36/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:59:00.225320 soda-core-oracle-3.0.36/soda/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:59:00.225320 soda-core-oracle-3.0.36/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     9209 2023-05-11 22:53:33.000000 soda-core-oracle-3.0.36/soda/data_sources/oracle_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 22:59:00.225320 soda-core-oracle-3.0.36/soda_core_oracle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-11 22:59:00.000000 soda-core-oracle-3.0.36/soda_core_oracle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-11 22:59:00.000000 soda-core-oracle-3.0.36/soda_core_oracle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 22:59:00.000000 soda-core-oracle-3.0.36/soda_core_oracle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-11 22:59:00.000000 soda-core-oracle-3.0.36/soda_core_oracle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-11 22:59:00.000000 soda-core-oracle-3.0.36/soda_core_oracle.egg-info/top_level.txt
```

### Comparing `soda-core-oracle-3.0.35/setup.py` & `soda-core-oracle-3.0.36/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda Core requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-oracle"
-package_version = "3.0.35"
+package_version = "3.0.36"
 # TODO Add proper description
 description = "Soda Core Oracle Package"
 
 requires = [f"soda-core=={package_version}", "oracledb==1.1.1"]
 # TODO Fix the params
 setup(
     name=package_name,
```

### Comparing `soda-core-oracle-3.0.35/soda/data_sources/oracle_data_source.py` & `soda-core-oracle-3.0.36/soda/data_sources/oracle_data_source.py`

 * *Files identical despite different names*


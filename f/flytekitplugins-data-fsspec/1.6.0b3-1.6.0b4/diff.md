# Comparing `tmp/flytekitplugins-data-fsspec-1.6.0b3.tar.gz` & `tmp/flytekitplugins-data-fsspec-1.6.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-data-fsspec-1.6.0b3.tar", last modified: Mon May  8 20:18:39 2023, max compression
+gzip compressed data, was "flytekitplugins-data-fsspec-1.6.0b4.tar", last modified: Tue May  9 00:42:32 2023, max compression
```

## Comparing `flytekitplugins-data-fsspec-1.6.0b3.tar` & `flytekitplugins-data-fsspec-1.6.0b4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:39.460879 flytekitplugins-data-fsspec-1.6.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-08 20:18:39.460879 flytekitplugins-data-fsspec-1.6.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-08 20:18:20.000000 flytekitplugins-data-fsspec-1.6.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:39.460879 flytekitplugins-data-fsspec-1.6.0b3/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:39.460879 flytekitplugins-data-fsspec-1.6.0b3/flytekitplugins/fsspec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:20.000000 flytekitplugins-data-fsspec-1.6.0b3/flytekitplugins/fsspec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:39.460879 flytekitplugins-data-fsspec-1.6.0b3/flytekitplugins_data_fsspec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-08 20:18:39.000000 flytekitplugins-data-fsspec-1.6.0b3/flytekitplugins_data_fsspec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-08 20:18:39.000000 flytekitplugins-data-fsspec-1.6.0b3/flytekitplugins_data_fsspec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:18:39.000000 flytekitplugins-data-fsspec-1.6.0b3/flytekitplugins_data_fsspec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:39.000000 flytekitplugins-data-fsspec-1.6.0b3/flytekitplugins_data_fsspec.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 20:18:39.000000 flytekitplugins-data-fsspec-1.6.0b3/flytekitplugins_data_fsspec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:39.000000 flytekitplugins-data-fsspec-1.6.0b3/flytekitplugins_data_fsspec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:18:39.460879 flytekitplugins-data-fsspec-1.6.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-08 20:18:37.000000 flytekitplugins-data-fsspec-1.6.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:32.524757 flytekitplugins-data-fsspec-1.6.0b4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-09 00:42:32.524757 flytekitplugins-data-fsspec-1.6.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-09 00:42:14.000000 flytekitplugins-data-fsspec-1.6.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:32.520757 flytekitplugins-data-fsspec-1.6.0b4/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:32.520757 flytekitplugins-data-fsspec-1.6.0b4/flytekitplugins/fsspec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:14.000000 flytekitplugins-data-fsspec-1.6.0b4/flytekitplugins/fsspec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:32.524757 flytekitplugins-data-fsspec-1.6.0b4/flytekitplugins_data_fsspec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-09 00:42:32.000000 flytekitplugins-data-fsspec-1.6.0b4/flytekitplugins_data_fsspec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-09 00:42:32.000000 flytekitplugins-data-fsspec-1.6.0b4/flytekitplugins_data_fsspec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:42:32.000000 flytekitplugins-data-fsspec-1.6.0b4/flytekitplugins_data_fsspec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:32.000000 flytekitplugins-data-fsspec-1.6.0b4/flytekitplugins_data_fsspec.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-09 00:42:32.000000 flytekitplugins-data-fsspec-1.6.0b4/flytekitplugins_data_fsspec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:32.000000 flytekitplugins-data-fsspec-1.6.0b4/flytekitplugins_data_fsspec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 00:42:32.524757 flytekitplugins-data-fsspec-1.6.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-09 00:42:30.000000 flytekitplugins-data-fsspec-1.6.0b4/setup.py
```

### Comparing `flytekitplugins-data-fsspec-1.6.0b3/PKG-INFO` & `flytekitplugins-data-fsspec-1.6.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-data-fsspec
-Version: 1.6.0b3
+Version: 1.6.0b4
 Summary: This is a deprecated plugin as of flytekit 1.5
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-data-fsspec
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-data-fsspec-1.6.0b3/flytekitplugins_data_fsspec.egg-info/PKG-INFO` & `flytekitplugins-data-fsspec-1.6.0b4/flytekitplugins_data_fsspec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-data-fsspec
-Version: 1.6.0b3
+Version: 1.6.0b4
 Summary: This is a deprecated plugin as of flytekit 1.5
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-data-fsspec
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-data-fsspec-1.6.0b3/setup.py` & `flytekitplugins-data-fsspec-1.6.0b4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "fsspec"
 
 microlib_name = f"flytekitplugins-data-{PLUGIN_NAME}"
 
 plugin_requires = []
 
-__version__ = "1.6.0b3"
+__version__ = "1.6.0b4"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This is a deprecated plugin as of flytekit 1.5",
```


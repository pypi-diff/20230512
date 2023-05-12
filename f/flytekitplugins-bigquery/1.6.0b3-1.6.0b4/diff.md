# Comparing `tmp/flytekitplugins-bigquery-1.6.0b3.tar.gz` & `tmp/flytekitplugins-bigquery-1.6.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-bigquery-1.6.0b3.tar", last modified: Mon May  8 20:18:38 2023, max compression
+gzip compressed data, was "flytekitplugins-bigquery-1.6.0b4.tar", last modified: Tue May  9 00:42:31 2023, max compression
```

## Comparing `flytekitplugins-bigquery-1.6.0b3.tar` & `flytekitplugins-bigquery-1.6.0b4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:38.752881 flytekitplugins-bigquery-1.6.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-08 20:18:38.752881 flytekitplugins-bigquery-1.6.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-08 20:18:20.000000 flytekitplugins-bigquery-1.6.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:38.752881 flytekitplugins-bigquery-1.6.0b3/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:38.752881 flytekitplugins-bigquery-1.6.0b3/flytekitplugins/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-08 20:18:20.000000 flytekitplugins-bigquery-1.6.0b3/flytekitplugins/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-05-08 20:18:20.000000 flytekitplugins-bigquery-1.6.0b3/flytekitplugins/bigquery/backend_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-05-08 20:18:20.000000 flytekitplugins-bigquery-1.6.0b3/flytekitplugins/bigquery/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:38.752881 flytekitplugins-bigquery-1.6.0b3/flytekitplugins_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-08 20:18:38.000000 flytekitplugins-bigquery-1.6.0b3/flytekitplugins_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-08 20:18:38.000000 flytekitplugins-bigquery-1.6.0b3/flytekitplugins_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:18:38.000000 flytekitplugins-bigquery-1.6.0b3/flytekitplugins_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-08 20:18:38.000000 flytekitplugins-bigquery-1.6.0b3/flytekitplugins_bigquery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:38.000000 flytekitplugins-bigquery-1.6.0b3/flytekitplugins_bigquery.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-08 20:18:38.000000 flytekitplugins-bigquery-1.6.0b3/flytekitplugins_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:38.000000 flytekitplugins-bigquery-1.6.0b3/flytekitplugins_bigquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:18:38.752881 flytekitplugins-bigquery-1.6.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-08 20:18:37.000000 flytekitplugins-bigquery-1.6.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:31.812755 flytekitplugins-bigquery-1.6.0b4/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-09 00:42:31.812755 flytekitplugins-bigquery-1.6.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-09 00:42:14.000000 flytekitplugins-bigquery-1.6.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:31.808755 flytekitplugins-bigquery-1.6.0b4/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:31.808755 flytekitplugins-bigquery-1.6.0b4/flytekitplugins/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-09 00:42:14.000000 flytekitplugins-bigquery-1.6.0b4/flytekitplugins/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-05-09 00:42:14.000000 flytekitplugins-bigquery-1.6.0b4/flytekitplugins/bigquery/backend_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-05-09 00:42:14.000000 flytekitplugins-bigquery-1.6.0b4/flytekitplugins/bigquery/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:31.812755 flytekitplugins-bigquery-1.6.0b4/flytekitplugins_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-09 00:42:31.000000 flytekitplugins-bigquery-1.6.0b4/flytekitplugins_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-09 00:42:31.000000 flytekitplugins-bigquery-1.6.0b4/flytekitplugins_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:42:31.000000 flytekitplugins-bigquery-1.6.0b4/flytekitplugins_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 00:42:31.000000 flytekitplugins-bigquery-1.6.0b4/flytekitplugins_bigquery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:31.000000 flytekitplugins-bigquery-1.6.0b4/flytekitplugins_bigquery.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 00:42:31.000000 flytekitplugins-bigquery-1.6.0b4/flytekitplugins_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:31.000000 flytekitplugins-bigquery-1.6.0b4/flytekitplugins_bigquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 00:42:31.812755 flytekitplugins-bigquery-1.6.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-09 00:42:30.000000 flytekitplugins-bigquery-1.6.0b4/setup.py
```

### Comparing `flytekitplugins-bigquery-1.6.0b3/PKG-INFO` & `flytekitplugins-bigquery-1.6.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-bigquery
-Version: 1.6.0b3
+Version: 1.6.0b4
 Summary: This package holds the Bigquery plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-bigquery-1.6.0b3/README.md` & `flytekitplugins-bigquery-1.6.0b4/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-bigquery-1.6.0b3/flytekitplugins/bigquery/backend_plugin.py` & `flytekitplugins-bigquery-1.6.0b4/flytekitplugins/bigquery/backend_plugin.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-bigquery-1.6.0b3/flytekitplugins/bigquery/task.py` & `flytekitplugins-bigquery-1.6.0b4/flytekitplugins/bigquery/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-bigquery-1.6.0b3/flytekitplugins_bigquery.egg-info/PKG-INFO` & `flytekitplugins-bigquery-1.6.0b4/flytekitplugins_bigquery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-bigquery
-Version: 1.6.0b3
+Version: 1.6.0b4
 Summary: This package holds the Bigquery plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-bigquery-1.6.0b3/setup.py` & `flytekitplugins-bigquery-1.6.0b4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "bigquery"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "google-cloud-bigquery"]
 
-__version__ = "1.6.0b3"
+__version__ = "1.6.0b4"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the Bigquery plugins for flytekit",
```


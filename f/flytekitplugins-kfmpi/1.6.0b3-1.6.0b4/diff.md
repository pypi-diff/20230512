# Comparing `tmp/flytekitplugins-kfmpi-1.6.0b3.tar.gz` & `tmp/flytekitplugins-kfmpi-1.6.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-kfmpi-1.6.0b3.tar", last modified: Mon May  8 20:18:42 2023, max compression
+gzip compressed data, was "flytekitplugins-kfmpi-1.6.0b4.tar", last modified: Tue May  9 00:42:36 2023, max compression
```

## Comparing `flytekitplugins-kfmpi-1.6.0b3.tar` & `flytekitplugins-kfmpi-1.6.0b4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:42.984868 flytekitplugins-kfmpi-1.6.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-08 20:18:42.984868 flytekitplugins-kfmpi-1.6.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-08 20:18:20.000000 flytekitplugins-kfmpi-1.6.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:42.984868 flytekitplugins-kfmpi-1.6.0b3/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:42.984868 flytekitplugins-kfmpi-1.6.0b3/flytekitplugins/kfmpi/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-08 20:18:20.000000 flytekitplugins-kfmpi-1.6.0b3/flytekitplugins/kfmpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-05-08 20:18:20.000000 flytekitplugins-kfmpi-1.6.0b3/flytekitplugins/kfmpi/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:42.984868 flytekitplugins-kfmpi-1.6.0b3/flytekitplugins_kfmpi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-08 20:18:42.000000 flytekitplugins-kfmpi-1.6.0b3/flytekitplugins_kfmpi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-08 20:18:42.000000 flytekitplugins-kfmpi-1.6.0b3/flytekitplugins_kfmpi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:18:42.000000 flytekitplugins-kfmpi-1.6.0b3/flytekitplugins_kfmpi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:42.000000 flytekitplugins-kfmpi-1.6.0b3/flytekitplugins_kfmpi.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-08 20:18:42.000000 flytekitplugins-kfmpi-1.6.0b3/flytekitplugins_kfmpi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:42.000000 flytekitplugins-kfmpi-1.6.0b3/flytekitplugins_kfmpi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:18:42.984868 flytekitplugins-kfmpi-1.6.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-08 20:18:37.000000 flytekitplugins-kfmpi-1.6.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:36.072767 flytekitplugins-kfmpi-1.6.0b4/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-09 00:42:36.068767 flytekitplugins-kfmpi-1.6.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-09 00:42:15.000000 flytekitplugins-kfmpi-1.6.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:36.068767 flytekitplugins-kfmpi-1.6.0b4/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:36.068767 flytekitplugins-kfmpi-1.6.0b4/flytekitplugins/kfmpi/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-09 00:42:15.000000 flytekitplugins-kfmpi-1.6.0b4/flytekitplugins/kfmpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-05-09 00:42:15.000000 flytekitplugins-kfmpi-1.6.0b4/flytekitplugins/kfmpi/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:36.068767 flytekitplugins-kfmpi-1.6.0b4/flytekitplugins_kfmpi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-09 00:42:36.000000 flytekitplugins-kfmpi-1.6.0b4/flytekitplugins_kfmpi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-09 00:42:36.000000 flytekitplugins-kfmpi-1.6.0b4/flytekitplugins_kfmpi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:42:36.000000 flytekitplugins-kfmpi-1.6.0b4/flytekitplugins_kfmpi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:36.000000 flytekitplugins-kfmpi-1.6.0b4/flytekitplugins_kfmpi.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-09 00:42:36.000000 flytekitplugins-kfmpi-1.6.0b4/flytekitplugins_kfmpi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:36.000000 flytekitplugins-kfmpi-1.6.0b4/flytekitplugins_kfmpi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 00:42:36.072767 flytekitplugins-kfmpi-1.6.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-09 00:42:30.000000 flytekitplugins-kfmpi-1.6.0b4/setup.py
```

### Comparing `flytekitplugins-kfmpi-1.6.0b3/PKG-INFO` & `flytekitplugins-kfmpi-1.6.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfmpi
-Version: 1.6.0b3
+Version: 1.6.0b4
 Summary: K8s based MPI plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfmpi-1.6.0b3/flytekitplugins/kfmpi/task.py` & `flytekitplugins-kfmpi-1.6.0b4/flytekitplugins/kfmpi/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-kfmpi-1.6.0b3/flytekitplugins_kfmpi.egg-info/PKG-INFO` & `flytekitplugins-kfmpi-1.6.0b4/flytekitplugins_kfmpi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfmpi
-Version: 1.6.0b3
+Version: 1.6.0b4
 Summary: K8s based MPI plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfmpi-1.6.0b3/setup.py` & `flytekitplugins-kfmpi-1.6.0b4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "kfmpi"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "flyteidl>=0.21.4"]
 
-__version__ = "1.6.0b3"
+__version__ = "1.6.0b4"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="K8s based MPI plugin for flytekit",
```


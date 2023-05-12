# Comparing `tmp/flytekitplugins-kftensorflow-1.6.0b3.tar.gz` & `tmp/flytekitplugins-kftensorflow-1.6.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-kftensorflow-1.6.0b3.tar", last modified: Mon May  8 20:18:43 2023, max compression
+gzip compressed data, was "flytekitplugins-kftensorflow-1.6.0b4.tar", last modified: Tue May  9 00:42:36 2023, max compression
```

## Comparing `flytekitplugins-kftensorflow-1.6.0b3.tar` & `flytekitplugins-kftensorflow-1.6.0b4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:43.696866 flytekitplugins-kftensorflow-1.6.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-08 20:18:43.696866 flytekitplugins-kftensorflow-1.6.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-08 20:18:20.000000 flytekitplugins-kftensorflow-1.6.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:43.696866 flytekitplugins-kftensorflow-1.6.0b3/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:43.696866 flytekitplugins-kftensorflow-1.6.0b3/flytekitplugins/kftensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-08 20:18:20.000000 flytekitplugins-kftensorflow-1.6.0b3/flytekitplugins/kftensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-08 20:18:20.000000 flytekitplugins-kftensorflow-1.6.0b3/flytekitplugins/kftensorflow/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-08 20:18:20.000000 flytekitplugins-kftensorflow-1.6.0b3/flytekitplugins/kftensorflow/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:43.696866 flytekitplugins-kftensorflow-1.6.0b3/flytekitplugins_kftensorflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-08 20:18:43.000000 flytekitplugins-kftensorflow-1.6.0b3/flytekitplugins_kftensorflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-08 20:18:43.000000 flytekitplugins-kftensorflow-1.6.0b3/flytekitplugins_kftensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:18:43.000000 flytekitplugins-kftensorflow-1.6.0b3/flytekitplugins_kftensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:43.000000 flytekitplugins-kftensorflow-1.6.0b3/flytekitplugins_kftensorflow.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 20:18:43.000000 flytekitplugins-kftensorflow-1.6.0b3/flytekitplugins_kftensorflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:43.000000 flytekitplugins-kftensorflow-1.6.0b3/flytekitplugins_kftensorflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:18:43.696866 flytekitplugins-kftensorflow-1.6.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-08 20:18:37.000000 flytekitplugins-kftensorflow-1.6.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:36.768768 flytekitplugins-kftensorflow-1.6.0b4/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-09 00:42:36.768768 flytekitplugins-kftensorflow-1.6.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-09 00:42:15.000000 flytekitplugins-kftensorflow-1.6.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:36.764768 flytekitplugins-kftensorflow-1.6.0b4/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:36.768768 flytekitplugins-kftensorflow-1.6.0b4/flytekitplugins/kftensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-09 00:42:15.000000 flytekitplugins-kftensorflow-1.6.0b4/flytekitplugins/kftensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-09 00:42:15.000000 flytekitplugins-kftensorflow-1.6.0b4/flytekitplugins/kftensorflow/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-09 00:42:15.000000 flytekitplugins-kftensorflow-1.6.0b4/flytekitplugins/kftensorflow/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:36.768768 flytekitplugins-kftensorflow-1.6.0b4/flytekitplugins_kftensorflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-09 00:42:36.000000 flytekitplugins-kftensorflow-1.6.0b4/flytekitplugins_kftensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-09 00:42:36.000000 flytekitplugins-kftensorflow-1.6.0b4/flytekitplugins_kftensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:42:36.000000 flytekitplugins-kftensorflow-1.6.0b4/flytekitplugins_kftensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:36.000000 flytekitplugins-kftensorflow-1.6.0b4/flytekitplugins_kftensorflow.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 00:42:36.000000 flytekitplugins-kftensorflow-1.6.0b4/flytekitplugins_kftensorflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:36.000000 flytekitplugins-kftensorflow-1.6.0b4/flytekitplugins_kftensorflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 00:42:36.768768 flytekitplugins-kftensorflow-1.6.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-09 00:42:30.000000 flytekitplugins-kftensorflow-1.6.0b4/setup.py
```

### Comparing `flytekitplugins-kftensorflow-1.6.0b3/PKG-INFO` & `flytekitplugins-kftensorflow-1.6.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kftensorflow
-Version: 1.6.0b3
+Version: 1.6.0b4
 Summary: K8s based Tensorflow plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kftensorflow-1.6.0b3/flytekitplugins/kftensorflow/models.py` & `flytekitplugins-kftensorflow-1.6.0b4/flytekitplugins/kftensorflow/models.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-kftensorflow-1.6.0b3/flytekitplugins/kftensorflow/task.py` & `flytekitplugins-kftensorflow-1.6.0b4/flytekitplugins/kftensorflow/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-kftensorflow-1.6.0b3/flytekitplugins_kftensorflow.egg-info/PKG-INFO` & `flytekitplugins-kftensorflow-1.6.0b4/flytekitplugins_kftensorflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kftensorflow
-Version: 1.6.0b3
+Version: 1.6.0b4
 Summary: K8s based Tensorflow plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kftensorflow-1.6.0b3/setup.py` & `flytekitplugins-kftensorflow-1.6.0b4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 PLUGIN_NAME = "kftensorflow"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 # TODO: Requirements are missing, add them back in later.
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0"]
 
-__version__ = "1.6.0b3"
+__version__ = "1.6.0b4"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="K8s based Tensorflow plugin for flytekit",
```


# Comparing `tmp/flytekitplugins-kfpytorch-1.6.0b3.tar.gz` & `tmp/flytekitplugins-kfpytorch-1.6.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-kfpytorch-1.6.0b3.tar", last modified: Mon May  8 20:18:43 2023, max compression
+gzip compressed data, was "flytekitplugins-kfpytorch-1.6.0b4.tar", last modified: Tue May  9 00:42:36 2023, max compression
```

## Comparing `flytekitplugins-kfpytorch-1.6.0b3.tar` & `flytekitplugins-kfpytorch-1.6.0b4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:43.344867 flytekitplugins-kfpytorch-1.6.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-08 20:18:43.344867 flytekitplugins-kfpytorch-1.6.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-08 20:18:20.000000 flytekitplugins-kfpytorch-1.6.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:43.344867 flytekitplugins-kfpytorch-1.6.0b3/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:43.344867 flytekitplugins-kfpytorch-1.6.0b3/flytekitplugins/kfpytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-08 20:18:20.000000 flytekitplugins-kfpytorch-1.6.0b3/flytekitplugins/kfpytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-05-08 20:18:20.000000 flytekitplugins-kfpytorch-1.6.0b3/flytekitplugins/kfpytorch/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:43.344867 flytekitplugins-kfpytorch-1.6.0b3/flytekitplugins_kfpytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-08 20:18:43.000000 flytekitplugins-kfpytorch-1.6.0b3/flytekitplugins_kfpytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-08 20:18:43.000000 flytekitplugins-kfpytorch-1.6.0b3/flytekitplugins_kfpytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:18:43.000000 flytekitplugins-kfpytorch-1.6.0b3/flytekitplugins_kfpytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:43.000000 flytekitplugins-kfpytorch-1.6.0b3/flytekitplugins_kfpytorch.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-08 20:18:43.000000 flytekitplugins-kfpytorch-1.6.0b3/flytekitplugins_kfpytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:43.000000 flytekitplugins-kfpytorch-1.6.0b3/flytekitplugins_kfpytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:18:43.344867 flytekitplugins-kfpytorch-1.6.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-08 20:18:37.000000 flytekitplugins-kfpytorch-1.6.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:36.420768 flytekitplugins-kfpytorch-1.6.0b4/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-09 00:42:36.420768 flytekitplugins-kfpytorch-1.6.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-09 00:42:15.000000 flytekitplugins-kfpytorch-1.6.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:36.420768 flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:36.420768 flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins/kfpytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-09 00:42:15.000000 flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins/kfpytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-05-09 00:42:15.000000 flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins/kfpytorch/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:36.420768 flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins_kfpytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-09 00:42:36.000000 flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins_kfpytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-09 00:42:36.000000 flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins_kfpytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:42:36.000000 flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins_kfpytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:36.000000 flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins_kfpytorch.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-09 00:42:36.000000 flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins_kfpytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:36.000000 flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins_kfpytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 00:42:36.420768 flytekitplugins-kfpytorch-1.6.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-09 00:42:30.000000 flytekitplugins-kfpytorch-1.6.0b4/setup.py
```

### Comparing `flytekitplugins-kfpytorch-1.6.0b3/PKG-INFO` & `flytekitplugins-kfpytorch-1.6.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfpytorch
-Version: 1.6.0b3
+Version: 1.6.0b4
 Summary: K8s based Pytorch plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfpytorch-1.6.0b3/README.md` & `flytekitplugins-kfpytorch-1.6.0b4/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-kfpytorch-1.6.0b3/flytekitplugins/kfpytorch/task.py` & `flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins/kfpytorch/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-kfpytorch-1.6.0b3/flytekitplugins_kfpytorch.egg-info/PKG-INFO` & `flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins_kfpytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfpytorch
-Version: 1.6.0b3
+Version: 1.6.0b4
 Summary: K8s based Pytorch plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfpytorch-1.6.0b3/setup.py` & `flytekitplugins-kfpytorch-1.6.0b4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "kfpytorch"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["cloudpickle", "flytekit>=1.3.0,<2.0.0", "flyteidl>=1.3.19"]
 
-__version__ = "1.6.0b3"
+__version__ = "1.6.0b4"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="K8s based Pytorch plugin for Flytekit",
```


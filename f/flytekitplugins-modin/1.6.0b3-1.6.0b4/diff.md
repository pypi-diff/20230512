# Comparing `tmp/flytekitplugins-modin-1.6.0b3.tar.gz` & `tmp/flytekitplugins-modin-1.6.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-modin-1.6.0b3.tar", last modified: Mon May  8 20:18:44 2023, max compression
+gzip compressed data, was "flytekitplugins-modin-1.6.0b4.tar", last modified: Tue May  9 00:42:37 2023, max compression
```

## Comparing `flytekitplugins-modin-1.6.0b3.tar` & `flytekitplugins-modin-1.6.0b4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:44.404863 flytekitplugins-modin-1.6.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-08 20:18:44.404863 flytekitplugins-modin-1.6.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-08 20:18:20.000000 flytekitplugins-modin-1.6.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:44.400863 flytekitplugins-modin-1.6.0b3/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:44.400863 flytekitplugins-modin-1.6.0b3/flytekitplugins/modin/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-08 20:18:20.000000 flytekitplugins-modin-1.6.0b3/flytekitplugins/modin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-08 20:18:20.000000 flytekitplugins-modin-1.6.0b3/flytekitplugins/modin/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:44.404863 flytekitplugins-modin-1.6.0b3/flytekitplugins_modin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-08 20:18:44.000000 flytekitplugins-modin-1.6.0b3/flytekitplugins_modin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-08 20:18:44.000000 flytekitplugins-modin-1.6.0b3/flytekitplugins_modin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:18:44.000000 flytekitplugins-modin-1.6.0b3/flytekitplugins_modin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:44.000000 flytekitplugins-modin-1.6.0b3/flytekitplugins_modin.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-08 20:18:44.000000 flytekitplugins-modin-1.6.0b3/flytekitplugins_modin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:44.000000 flytekitplugins-modin-1.6.0b3/flytekitplugins_modin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:18:44.404863 flytekitplugins-modin-1.6.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-08 20:18:37.000000 flytekitplugins-modin-1.6.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:37.476770 flytekitplugins-modin-1.6.0b4/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-09 00:42:37.476770 flytekitplugins-modin-1.6.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-09 00:42:15.000000 flytekitplugins-modin-1.6.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:37.476770 flytekitplugins-modin-1.6.0b4/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:37.476770 flytekitplugins-modin-1.6.0b4/flytekitplugins/modin/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-09 00:42:15.000000 flytekitplugins-modin-1.6.0b4/flytekitplugins/modin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-09 00:42:15.000000 flytekitplugins-modin-1.6.0b4/flytekitplugins/modin/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:37.476770 flytekitplugins-modin-1.6.0b4/flytekitplugins_modin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-09 00:42:37.000000 flytekitplugins-modin-1.6.0b4/flytekitplugins_modin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-09 00:42:37.000000 flytekitplugins-modin-1.6.0b4/flytekitplugins_modin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:42:37.000000 flytekitplugins-modin-1.6.0b4/flytekitplugins_modin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:37.000000 flytekitplugins-modin-1.6.0b4/flytekitplugins_modin.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-09 00:42:37.000000 flytekitplugins-modin-1.6.0b4/flytekitplugins_modin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:37.000000 flytekitplugins-modin-1.6.0b4/flytekitplugins_modin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 00:42:37.476770 flytekitplugins-modin-1.6.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-09 00:42:30.000000 flytekitplugins-modin-1.6.0b4/setup.py
```

### Comparing `flytekitplugins-modin-1.6.0b3/PKG-INFO` & `flytekitplugins-modin-1.6.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-modin
-Version: 1.6.0b3
+Version: 1.6.0b4
 Summary: Modin plugin for flytekit
 Author: Intel
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `flytekitplugins-modin-1.6.0b3/README.md` & `flytekitplugins-modin-1.6.0b4/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-modin-1.6.0b3/flytekitplugins/modin/schema.py` & `flytekitplugins-modin-1.6.0b4/flytekitplugins/modin/schema.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-modin-1.6.0b3/flytekitplugins_modin.egg-info/PKG-INFO` & `flytekitplugins-modin-1.6.0b4/flytekitplugins_modin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-modin
-Version: 1.6.0b3
+Version: 1.6.0b4
 Summary: Modin plugin for flytekit
 Author: Intel
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `flytekitplugins-modin-1.6.0b3/setup.py` & `flytekitplugins-modin-1.6.0b4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 plugin_requires = [
     "flytekit<1.3.0b2,<2.0.0",
     "modin>=0.13.0",
     "fsspec",
     "ray",
 ]
 
-__version__ = "1.6.0b3"
+__version__ = "1.6.0b4"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="Intel",
     description="Modin plugin for flytekit",
     namespace_packages=["flytekitplugins"],
```


# Comparing `tmp/flytekitplugins-papermill-1.6.0b3.tar.gz` & `tmp/flytekitplugins-papermill-1.6.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-papermill-1.6.0b3.tar", last modified: Mon May  8 20:18:45 2023, max compression
+gzip compressed data, was "flytekitplugins-papermill-1.6.0b4.tar", last modified: Tue May  9 00:42:38 2023, max compression
```

## Comparing `flytekitplugins-papermill-1.6.0b3.tar` & `flytekitplugins-papermill-1.6.0b4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:45.812858 flytekitplugins-papermill-1.6.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-08 20:18:45.812858 flytekitplugins-papermill-1.6.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-08 20:18:20.000000 flytekitplugins-papermill-1.6.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:45.808858 flytekitplugins-papermill-1.6.0b3/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:45.812858 flytekitplugins-papermill-1.6.0b3/flytekitplugins/papermill/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-08 20:18:20.000000 flytekitplugins-papermill-1.6.0b3/flytekitplugins/papermill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12932 2023-05-08 20:18:20.000000 flytekitplugins-papermill-1.6.0b3/flytekitplugins/papermill/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:45.812858 flytekitplugins-papermill-1.6.0b3/flytekitplugins_papermill.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-08 20:18:45.000000 flytekitplugins-papermill-1.6.0b3/flytekitplugins_papermill.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-08 20:18:45.000000 flytekitplugins-papermill-1.6.0b3/flytekitplugins_papermill.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:18:45.000000 flytekitplugins-papermill-1.6.0b3/flytekitplugins_papermill.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:45.000000 flytekitplugins-papermill-1.6.0b3/flytekitplugins_papermill.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-08 20:18:45.000000 flytekitplugins-papermill-1.6.0b3/flytekitplugins_papermill.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:45.000000 flytekitplugins-papermill-1.6.0b3/flytekitplugins_papermill.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:18:45.812858 flytekitplugins-papermill-1.6.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-08 20:18:37.000000 flytekitplugins-papermill-1.6.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:38.888773 flytekitplugins-papermill-1.6.0b4/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-09 00:42:38.888773 flytekitplugins-papermill-1.6.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-09 00:42:15.000000 flytekitplugins-papermill-1.6.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:38.888773 flytekitplugins-papermill-1.6.0b4/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:38.888773 flytekitplugins-papermill-1.6.0b4/flytekitplugins/papermill/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-09 00:42:15.000000 flytekitplugins-papermill-1.6.0b4/flytekitplugins/papermill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12932 2023-05-09 00:42:15.000000 flytekitplugins-papermill-1.6.0b4/flytekitplugins/papermill/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:38.888773 flytekitplugins-papermill-1.6.0b4/flytekitplugins_papermill.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-09 00:42:38.000000 flytekitplugins-papermill-1.6.0b4/flytekitplugins_papermill.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-09 00:42:38.000000 flytekitplugins-papermill-1.6.0b4/flytekitplugins_papermill.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:42:38.000000 flytekitplugins-papermill-1.6.0b4/flytekitplugins_papermill.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:38.000000 flytekitplugins-papermill-1.6.0b4/flytekitplugins_papermill.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-09 00:42:38.000000 flytekitplugins-papermill-1.6.0b4/flytekitplugins_papermill.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:38.000000 flytekitplugins-papermill-1.6.0b4/flytekitplugins_papermill.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 00:42:38.888773 flytekitplugins-papermill-1.6.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-09 00:42:30.000000 flytekitplugins-papermill-1.6.0b4/setup.py
```

### Comparing `flytekitplugins-papermill-1.6.0b3/PKG-INFO` & `flytekitplugins-papermill-1.6.0b4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-papermill
-Version: 1.6.0b3
+Version: 1.6.0b4
 Summary: This is the flytekit papermill plugin
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-papermill-1.6.0b3/README.md` & `flytekitplugins-papermill-1.6.0b4/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-papermill-1.6.0b3/flytekitplugins/papermill/task.py` & `flytekitplugins-papermill-1.6.0b4/flytekitplugins/papermill/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-papermill-1.6.0b3/flytekitplugins_papermill.egg-info/PKG-INFO` & `flytekitplugins-papermill-1.6.0b4/flytekitplugins_papermill.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-papermill
-Version: 1.6.0b3
+Version: 1.6.0b4
 Summary: This is the flytekit papermill plugin
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-papermill-1.6.0b3/setup.py` & `flytekitplugins-papermill-1.6.0b4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 plugin_requires = [
     "flytekit>=1.3.0b2,<2.0.0",
     "papermill>=1.2.0",
     "nbconvert>=6.0.7",
     "ipykernel>=5.0.0",
 ]
 
-__version__ = "1.6.0b3"
+__version__ = "1.6.0b4"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This is the flytekit papermill plugin",
```


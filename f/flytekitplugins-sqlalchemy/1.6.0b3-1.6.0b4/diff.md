# Comparing `tmp/flytekitplugins-sqlalchemy-1.6.0b3.tar.gz` & `tmp/flytekitplugins-sqlalchemy-1.6.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-sqlalchemy-1.6.0b3.tar", last modified: Mon May  8 20:18:47 2023, max compression
+gzip compressed data, was "flytekitplugins-sqlalchemy-1.6.0b4.tar", last modified: Tue May  9 00:42:40 2023, max compression
```

## Comparing `flytekitplugins-sqlalchemy-1.6.0b3.tar` & `flytekitplugins-sqlalchemy-1.6.0b4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:47.580853 flytekitplugins-sqlalchemy-1.6.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-08 20:18:47.576853 flytekitplugins-sqlalchemy-1.6.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-08 20:18:20.000000 flytekitplugins-sqlalchemy-1.6.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:47.576853 flytekitplugins-sqlalchemy-1.6.0b3/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:47.576853 flytekitplugins-sqlalchemy-1.6.0b3/flytekitplugins/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-08 20:18:20.000000 flytekitplugins-sqlalchemy-1.6.0b3/flytekitplugins/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-05-08 20:18:20.000000 flytekitplugins-sqlalchemy-1.6.0b3/flytekitplugins/sqlalchemy/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:47.576853 flytekitplugins-sqlalchemy-1.6.0b3/flytekitplugins_sqlalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-08 20:18:47.000000 flytekitplugins-sqlalchemy-1.6.0b3/flytekitplugins_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-08 20:18:47.000000 flytekitplugins-sqlalchemy-1.6.0b3/flytekitplugins_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:18:47.000000 flytekitplugins-sqlalchemy-1.6.0b3/flytekitplugins_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:47.000000 flytekitplugins-sqlalchemy-1.6.0b3/flytekitplugins_sqlalchemy.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 20:18:47.000000 flytekitplugins-sqlalchemy-1.6.0b3/flytekitplugins_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:47.000000 flytekitplugins-sqlalchemy-1.6.0b3/flytekitplugins_sqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:18:47.580853 flytekitplugins-sqlalchemy-1.6.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-08 20:18:37.000000 flytekitplugins-sqlalchemy-1.6.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:40.672777 flytekitplugins-sqlalchemy-1.6.0b4/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-09 00:42:40.672777 flytekitplugins-sqlalchemy-1.6.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-09 00:42:15.000000 flytekitplugins-sqlalchemy-1.6.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:40.668777 flytekitplugins-sqlalchemy-1.6.0b4/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:40.668777 flytekitplugins-sqlalchemy-1.6.0b4/flytekitplugins/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-09 00:42:15.000000 flytekitplugins-sqlalchemy-1.6.0b4/flytekitplugins/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-05-09 00:42:15.000000 flytekitplugins-sqlalchemy-1.6.0b4/flytekitplugins/sqlalchemy/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:40.668777 flytekitplugins-sqlalchemy-1.6.0b4/flytekitplugins_sqlalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-09 00:42:40.000000 flytekitplugins-sqlalchemy-1.6.0b4/flytekitplugins_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-09 00:42:40.000000 flytekitplugins-sqlalchemy-1.6.0b4/flytekitplugins_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:42:40.000000 flytekitplugins-sqlalchemy-1.6.0b4/flytekitplugins_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:40.000000 flytekitplugins-sqlalchemy-1.6.0b4/flytekitplugins_sqlalchemy.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-09 00:42:40.000000 flytekitplugins-sqlalchemy-1.6.0b4/flytekitplugins_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:40.000000 flytekitplugins-sqlalchemy-1.6.0b4/flytekitplugins_sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 00:42:40.672777 flytekitplugins-sqlalchemy-1.6.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-09 00:42:30.000000 flytekitplugins-sqlalchemy-1.6.0b4/setup.py
```

### Comparing `flytekitplugins-sqlalchemy-1.6.0b3/PKG-INFO` & `flytekitplugins-sqlalchemy-1.6.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-sqlalchemy
-Version: 1.6.0b3
+Version: 1.6.0b4
 Summary: SQLAlchemy plugin for flytekit
 Author: dolthub
 Author-email: max@dolthub.com
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-sqlalchemy-1.6.0b3/README.md` & `flytekitplugins-sqlalchemy-1.6.0b4/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-sqlalchemy-1.6.0b3/flytekitplugins/sqlalchemy/task.py` & `flytekitplugins-sqlalchemy-1.6.0b4/flytekitplugins/sqlalchemy/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-sqlalchemy-1.6.0b3/flytekitplugins_sqlalchemy.egg-info/PKG-INFO` & `flytekitplugins-sqlalchemy-1.6.0b4/flytekitplugins_sqlalchemy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-sqlalchemy
-Version: 1.6.0b3
+Version: 1.6.0b4
 Summary: SQLAlchemy plugin for flytekit
 Author: dolthub
 Author-email: max@dolthub.com
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-sqlalchemy-1.6.0b3/setup.py` & `flytekitplugins-sqlalchemy-1.6.0b4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "sqlalchemy"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "sqlalchemy>=1.4.7"]
 
-__version__ = "1.6.0b3"
+__version__ = "1.6.0b4"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="dolthub",
     author_email="max@dolthub.com",
     description="SQLAlchemy plugin for flytekit",
```


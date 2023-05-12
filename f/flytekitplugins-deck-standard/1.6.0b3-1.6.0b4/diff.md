# Comparing `tmp/flytekitplugins-deck-standard-1.6.0b3.tar.gz` & `tmp/flytekitplugins-deck-standard-1.6.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-deck-standard-1.6.0b3.tar", last modified: Mon May  8 20:18:40 2023, max compression
+gzip compressed data, was "flytekitplugins-deck-standard-1.6.0b4.tar", last modified: Tue May  9 00:42:33 2023, max compression
```

## Comparing `flytekitplugins-deck-standard-1.6.0b3.tar` & `flytekitplugins-deck-standard-1.6.0b4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:40.172877 flytekitplugins-deck-standard-1.6.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-08 20:18:40.168877 flytekitplugins-deck-standard-1.6.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-08 20:18:20.000000 flytekitplugins-deck-standard-1.6.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:40.168877 flytekitplugins-deck-standard-1.6.0b3/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:40.168877 flytekitplugins-deck-standard-1.6.0b3/flytekitplugins/deck/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-08 20:18:20.000000 flytekitplugins-deck-standard-1.6.0b3/flytekitplugins/deck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-08 20:18:20.000000 flytekitplugins-deck-standard-1.6.0b3/flytekitplugins/deck/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:40.168877 flytekitplugins-deck-standard-1.6.0b3/flytekitplugins_deck_standard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-08 20:18:40.000000 flytekitplugins-deck-standard-1.6.0b3/flytekitplugins_deck_standard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-08 20:18:40.000000 flytekitplugins-deck-standard-1.6.0b3/flytekitplugins_deck_standard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:18:40.000000 flytekitplugins-deck-standard-1.6.0b3/flytekitplugins_deck_standard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-08 20:18:40.000000 flytekitplugins-deck-standard-1.6.0b3/flytekitplugins_deck_standard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:40.000000 flytekitplugins-deck-standard-1.6.0b3/flytekitplugins_deck_standard.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-08 20:18:40.000000 flytekitplugins-deck-standard-1.6.0b3/flytekitplugins_deck_standard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:40.000000 flytekitplugins-deck-standard-1.6.0b3/flytekitplugins_deck_standard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:18:40.172877 flytekitplugins-deck-standard-1.6.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-08 20:18:37.000000 flytekitplugins-deck-standard-1.6.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:33.236759 flytekitplugins-deck-standard-1.6.0b4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-09 00:42:33.236759 flytekitplugins-deck-standard-1.6.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-09 00:42:14.000000 flytekitplugins-deck-standard-1.6.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:33.232759 flytekitplugins-deck-standard-1.6.0b4/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:33.232759 flytekitplugins-deck-standard-1.6.0b4/flytekitplugins/deck/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-09 00:42:14.000000 flytekitplugins-deck-standard-1.6.0b4/flytekitplugins/deck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-09 00:42:14.000000 flytekitplugins-deck-standard-1.6.0b4/flytekitplugins/deck/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:33.236759 flytekitplugins-deck-standard-1.6.0b4/flytekitplugins_deck_standard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-09 00:42:33.000000 flytekitplugins-deck-standard-1.6.0b4/flytekitplugins_deck_standard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-09 00:42:33.000000 flytekitplugins-deck-standard-1.6.0b4/flytekitplugins_deck_standard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:42:33.000000 flytekitplugins-deck-standard-1.6.0b4/flytekitplugins_deck_standard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 00:42:33.000000 flytekitplugins-deck-standard-1.6.0b4/flytekitplugins_deck_standard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:33.000000 flytekitplugins-deck-standard-1.6.0b4/flytekitplugins_deck_standard.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-09 00:42:33.000000 flytekitplugins-deck-standard-1.6.0b4/flytekitplugins_deck_standard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:33.000000 flytekitplugins-deck-standard-1.6.0b4/flytekitplugins_deck_standard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 00:42:33.236759 flytekitplugins-deck-standard-1.6.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-09 00:42:30.000000 flytekitplugins-deck-standard-1.6.0b4/setup.py
```

### Comparing `flytekitplugins-deck-standard-1.6.0b3/PKG-INFO` & `flytekitplugins-deck-standard-1.6.0b4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-deck-standard
-Version: 1.6.0b3
+Version: 1.6.0b4
 Summary: This Plugin provides more renderers to improve task visibility
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-data-fsspec
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-deck-standard-1.6.0b3/flytekitplugins/deck/renderer.py` & `flytekitplugins-deck-standard-1.6.0b4/flytekitplugins/deck/renderer.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-deck-standard-1.6.0b3/flytekitplugins_deck_standard.egg-info/PKG-INFO` & `flytekitplugins-deck-standard-1.6.0b4/flytekitplugins_deck_standard.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-deck-standard
-Version: 1.6.0b3
+Version: 1.6.0b4
 Summary: This Plugin provides more renderers to improve task visibility
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-data-fsspec
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-deck-standard-1.6.0b3/setup.py` & `flytekitplugins-deck-standard-1.6.0b4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "deck"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}-standard"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "markdown", "plotly", "ydata-profiling", "ipywidgets"]
 
-__version__ = "1.6.0b3"
+__version__ = "1.6.0b4"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This Plugin provides more renderers to improve task visibility",
```


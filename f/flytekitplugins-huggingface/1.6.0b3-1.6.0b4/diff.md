# Comparing `tmp/flytekitplugins-huggingface-1.6.0b3.tar.gz` & `tmp/flytekitplugins-huggingface-1.6.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-huggingface-1.6.0b3.tar", last modified: Mon May  8 20:18:42 2023, max compression
+gzip compressed data, was "flytekitplugins-huggingface-1.6.0b4.tar", last modified: Tue May  9 00:42:35 2023, max compression
```

## Comparing `flytekitplugins-huggingface-1.6.0b3.tar` & `flytekitplugins-huggingface-1.6.0b4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:42.280871 flytekitplugins-huggingface-1.6.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-08 20:18:42.280871 flytekitplugins-huggingface-1.6.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-08 20:18:20.000000 flytekitplugins-huggingface-1.6.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:42.280871 flytekitplugins-huggingface-1.6.0b3/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:42.280871 flytekitplugins-huggingface-1.6.0b3/flytekitplugins/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-08 20:18:20.000000 flytekitplugins-huggingface-1.6.0b3/flytekitplugins/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-08 20:18:20.000000 flytekitplugins-huggingface-1.6.0b3/flytekitplugins/huggingface/sd_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:18:42.280871 flytekitplugins-huggingface-1.6.0b3/flytekitplugins_huggingface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-08 20:18:42.000000 flytekitplugins-huggingface-1.6.0b3/flytekitplugins_huggingface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-08 20:18:42.000000 flytekitplugins-huggingface-1.6.0b3/flytekitplugins_huggingface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:18:42.000000 flytekitplugins-huggingface-1.6.0b3/flytekitplugins_huggingface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-08 20:18:42.000000 flytekitplugins-huggingface-1.6.0b3/flytekitplugins_huggingface.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:42.000000 flytekitplugins-huggingface-1.6.0b3/flytekitplugins_huggingface.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-08 20:18:42.000000 flytekitplugins-huggingface-1.6.0b3/flytekitplugins_huggingface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 20:18:42.000000 flytekitplugins-huggingface-1.6.0b3/flytekitplugins_huggingface.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:18:42.280871 flytekitplugins-huggingface-1.6.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-08 20:18:37.000000 flytekitplugins-huggingface-1.6.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:35.356765 flytekitplugins-huggingface-1.6.0b4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-09 00:42:35.356765 flytekitplugins-huggingface-1.6.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-09 00:42:15.000000 flytekitplugins-huggingface-1.6.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:35.356765 flytekitplugins-huggingface-1.6.0b4/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:35.356765 flytekitplugins-huggingface-1.6.0b4/flytekitplugins/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-09 00:42:15.000000 flytekitplugins-huggingface-1.6.0b4/flytekitplugins/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-09 00:42:15.000000 flytekitplugins-huggingface-1.6.0b4/flytekitplugins/huggingface/sd_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:35.356765 flytekitplugins-huggingface-1.6.0b4/flytekitplugins_huggingface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-09 00:42:35.000000 flytekitplugins-huggingface-1.6.0b4/flytekitplugins_huggingface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-09 00:42:35.000000 flytekitplugins-huggingface-1.6.0b4/flytekitplugins_huggingface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:42:35.000000 flytekitplugins-huggingface-1.6.0b4/flytekitplugins_huggingface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-09 00:42:35.000000 flytekitplugins-huggingface-1.6.0b4/flytekitplugins_huggingface.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:35.000000 flytekitplugins-huggingface-1.6.0b4/flytekitplugins_huggingface.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-09 00:42:35.000000 flytekitplugins-huggingface-1.6.0b4/flytekitplugins_huggingface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:35.000000 flytekitplugins-huggingface-1.6.0b4/flytekitplugins_huggingface.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 00:42:35.356765 flytekitplugins-huggingface-1.6.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-09 00:42:30.000000 flytekitplugins-huggingface-1.6.0b4/setup.py
```

### Comparing `flytekitplugins-huggingface-1.6.0b3/PKG-INFO` & `flytekitplugins-huggingface-1.6.0b4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-huggingface
-Version: 1.6.0b3
+Version: 1.6.0b4
 Summary: Hugging Face plugin for flytekit
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-huggingface
 Author: Evan Sadler
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-huggingface-1.6.0b3/README.md` & `flytekitplugins-huggingface-1.6.0b4/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-huggingface-1.6.0b3/flytekitplugins/huggingface/sd_transformers.py` & `flytekitplugins-huggingface-1.6.0b4/flytekitplugins/huggingface/sd_transformers.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-huggingface-1.6.0b3/flytekitplugins_huggingface.egg-info/PKG-INFO` & `flytekitplugins-huggingface-1.6.0b4/flytekitplugins_huggingface.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-huggingface
-Version: 1.6.0b3
+Version: 1.6.0b4
 Summary: Hugging Face plugin for flytekit
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-huggingface
 Author: Evan Sadler
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-huggingface-1.6.0b3/setup.py` & `flytekitplugins-huggingface-1.6.0b4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = [
     "flytekit>=1.3.0b2,<2.0.0",
     "datasets>=2.4.0",
 ]
 
-__version__ = "1.6.0b3"
+__version__ = "1.6.0b4"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="Evan Sadler",
     description="Hugging Face plugin for flytekit",
     url="https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-huggingface",
```


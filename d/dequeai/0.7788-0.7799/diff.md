# Comparing `tmp/dequeai-0.7788.tar.gz` & `tmp/dequeai-0.7799.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.7788.tar", last modified: Fri May 12 16:21:26 2023, max compression
+gzip compressed data, was "dequeai-0.7799.tar", last modified: Fri May 12 17:11:23 2023, max compression
```

## Comparing `dequeai-0.7788.tar` & `dequeai-0.7799.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:21:26.621949 dequeai-0.7788/
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-12 16:21:26.621949 dequeai-0.7788/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:21:26.621949 dequeai-0.7788/dequeai/
--rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.7788/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.7788/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.7788/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.7788/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-04-26 15:26:45.000000 dequeai-0.7788/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    29818 2023-05-12 16:20:46.000000 dequeai-0.7788/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.7788/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.7788/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.7788/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.7788/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:21:26.621949 dequeai-0.7788/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-12 16:21:26.000000 dequeai-0.7788/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-05-12 16:21:26.000000 dequeai-0.7788/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 16:21:26.000000 dequeai-0.7788/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-05-12 16:21:26.000000 dequeai-0.7788/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-12 16:21:26.000000 dequeai-0.7788/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 16:21:26.621949 dequeai-0.7788/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      584 2023-05-12 16:21:12.000000 dequeai-0.7788/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:23.299770 dequeai-0.7799/
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-12 17:11:23.299770 dequeai-0.7799/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:23.299770 dequeai-0.7799/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.7799/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.7799/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.7799/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.7799/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-04-26 15:26:45.000000 dequeai-0.7799/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    30272 2023-05-12 17:10:56.000000 dequeai-0.7799/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.7799/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.7799/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.7799/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.7799/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:23.299770 dequeai-0.7799/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-12 17:11:22.000000 dequeai-0.7799/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-05-12 17:11:23.000000 dequeai-0.7799/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 17:11:22.000000 dequeai-0.7799/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-05-12 17:11:23.000000 dequeai-0.7799/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-12 17:11:23.000000 dequeai-0.7799/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 17:11:23.299770 dequeai-0.7799/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      584 2023-05-12 17:11:09.000000 dequeai-0.7799/setup.py
```

### Comparing `dequeai-0.7788/dequeai/datatypes.py` & `dequeai-0.7799/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.7788/dequeai/dequeai.py` & `dequeai-0.7799/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.7788/dequeai/dequeai_run.py` & `dequeai-0.7799/dequeai/dequeai_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -380,29 +380,38 @@
                 http_response = requests.get(url=res["url"])
                 file_name = os.path.basename(artifact['artifact_uri'])
                 with open(file_name, "wb") as f:
                     f.write(http_response.content)
                 print(f"Downloaded artifact '{file_name}'")
 
     def _validate_data(self, data):
+        new_data = {}
         for key, value in data.items():
             if key is None:
-
                 raise ValueError("Key cannot be None")
 
-            if type(value) is dict:
-                self._validate_data(value)
+            if isinstance(value, dict):
+                new_data[key] = self._validate_data(value)
             else:
-                if type(value) in [Audio, BoundingBox2D, Histogram, Table,
-                                   Image] or type(value) in types.__builtins__.values():
-                    pass
+                if isinstance(value, (Audio, BoundingBox2D, Histogram, Table, Image)) or \
+                        type(value) in types.__builtins__.values():
+                    new_data[key] = value
+                elif isinstance(value, np.generic):  # Check if the value is a numpy type
+                    new_data[key] = self._convert_numpy_to_python(value)  # Convert numpy to Python scalar
                 else:
                     raise ValueError(
                         "Invalid type in dictionary. Allowed values include builtin types and Deque data types " + str(
                             type(value)) + " " + str(value.__class__.__module__))
+        return new_data
+
+    def _convert_numpy_to_python(self, val):
+        if np.isscalar(val) and isinstance(val, np.generic):
+            return np.asscalar(val)
+        else:
+            return val
 
     def _validate_hyperparams(self, hyperparams):
         for key, value in hyperparams.items():
             if type(value) in types.__builtins__.values():
                 pass
             else:
                 raise ValueError(
```

### Comparing `dequeai-0.7788/dequeai/parsing_service.py` & `dequeai-0.7799/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.7788/dequeai/rest_connect.py` & `dequeai-0.7799/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.7788/dequeai/util.py` & `dequeai-0.7799/dequeai/util.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.7788/setup.py` & `dequeai-0.7799/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, Extension
 
 
 setup(
     name='dequeai',
-    version='0.000007788',
+    version='0.000007799',
     description='Python Experiment Tracking Package for Deque AI DLOps Platform',
     author="The Deque AI Team",
     author_email='team@deque.app',
     packages=["dequeai"],
     url='https://dequeapp-deque.gitbook.io/deque-docs/getting-started/dequeai-experiment-tracking',
     keywords='deque client for experiment tracking, sweep and other deep learning tooling',
     install_requires=[
```


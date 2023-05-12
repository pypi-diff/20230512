# Comparing `tmp/dequeai-0.777.tar.gz` & `tmp/dequeai-0.7777.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.777.tar", last modified: Tue May  9 21:04:03 2023, max compression
+gzip compressed data, was "dequeai-0.7777.tar", last modified: Fri May 12 00:16:36 2023, max compression
```

## Comparing `dequeai-0.777.tar` & `dequeai-0.7777.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 21:04:03.484665 dequeai-0.777/
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-09 21:04:03.484665 dequeai-0.777/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 21:04:03.484665 dequeai-0.777/dequeai/
--rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.777/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.777/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.777/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.777/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-04-26 15:26:45.000000 dequeai-0.777/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    29696 2023-05-09 21:03:50.000000 dequeai-0.777/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.777/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.777/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.777/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.777/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 21:04:03.484665 dequeai-0.777/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-09 21:04:03.000000 dequeai-0.777/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-05-09 21:04:03.000000 dequeai-0.777/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 21:04:03.000000 dequeai-0.777/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-05-09 21:04:03.000000 dequeai-0.777/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-09 21:04:03.000000 dequeai-0.777/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 21:04:03.484665 dequeai-0.777/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      583 2023-05-09 21:03:51.000000 dequeai-0.777/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 00:16:36.041879 dequeai-0.7777/
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-12 00:16:36.041879 dequeai-0.7777/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 00:16:36.041879 dequeai-0.7777/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.7777/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.7777/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.7777/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.7777/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-04-26 15:26:45.000000 dequeai-0.7777/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    29701 2023-05-12 00:16:21.000000 dequeai-0.7777/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.7777/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.7777/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.7777/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.7777/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 00:16:36.041879 dequeai-0.7777/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-12 00:16:35.000000 dequeai-0.7777/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-05-12 00:16:36.000000 dequeai-0.7777/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 00:16:35.000000 dequeai-0.7777/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-05-12 00:16:35.000000 dequeai-0.7777/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-12 00:16:35.000000 dequeai-0.7777/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 00:16:36.041879 dequeai-0.7777/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      584 2023-05-12 00:16:21.000000 dequeai-0.7777/setup.py
```

### Comparing `dequeai-0.777/dequeai/datatypes.py` & `dequeai-0.7777/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.777/dequeai/dequeai.py` & `dequeai-0.7777/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.777/dequeai/dequeai_run.py` & `dequeai-0.7777/dequeai/dequeai_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,15 @@
         gpu_count = len(gpu_list)
 
         for i in range(gpu_count):
             gpu = gpu_list[i]
             gpu_free_memory = gpu.memoryFree
             current_gpu_load = 100 * gpu.load
             total_gpu_memory = gpu.memoryTotal
-            metadata["GPU"][i] = {
+            metadata["GPU"][str(i)] = {
                 "name": gpu.name,
                 "memory": {"total": total_gpu_memory, "free": gpu_free_memory},
                 "utilization": current_gpu_load
             }
 
         metadata.update({"CPU": {"utilization": psutil.cpu_percent(interval=1)}})
```

### Comparing `dequeai-0.777/dequeai/parsing_service.py` & `dequeai-0.7777/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.777/dequeai/rest_connect.py` & `dequeai-0.7777/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.777/dequeai/util.py` & `dequeai-0.7777/dequeai/util.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.777/setup.py` & `dequeai-0.7777/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, Extension
 
 
 setup(
     name='dequeai',
-    version='0.00000777',
+    version='0.000007777',
     description='Python Experiment Tracking Package for Deque AI DLOps Platform',
     author="The Deque AI Team",
     author_email='team@deque.app',
     packages=["dequeai"],
     url='https://dequeapp-deque.gitbook.io/deque-docs/getting-started/dequeai-experiment-tracking',
     keywords='deque client for experiment tracking, sweep and other deep learning tooling',
     install_requires=[
```


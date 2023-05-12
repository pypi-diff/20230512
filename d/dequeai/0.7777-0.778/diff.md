# Comparing `tmp/dequeai-0.7777.tar.gz` & `tmp/dequeai-0.778.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.7777.tar", last modified: Fri May 12 00:16:36 2023, max compression
+gzip compressed data, was "dequeai-0.778.tar", last modified: Fri May 12 14:29:48 2023, max compression
```

## Comparing `dequeai-0.7777.tar` & `dequeai-0.778.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 00:16:36.041879 dequeai-0.7777/
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-12 00:16:36.041879 dequeai-0.7777/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 00:16:36.041879 dequeai-0.7777/dequeai/
--rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.7777/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.7777/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.7777/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.7777/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-04-26 15:26:45.000000 dequeai-0.7777/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    29701 2023-05-12 00:16:21.000000 dequeai-0.7777/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.7777/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.7777/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.7777/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.7777/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 00:16:36.041879 dequeai-0.7777/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-12 00:16:35.000000 dequeai-0.7777/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-05-12 00:16:36.000000 dequeai-0.7777/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 00:16:35.000000 dequeai-0.7777/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-05-12 00:16:35.000000 dequeai-0.7777/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-12 00:16:35.000000 dequeai-0.7777/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 00:16:36.041879 dequeai-0.7777/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      584 2023-05-12 00:16:21.000000 dequeai-0.7777/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:29:48.718798 dequeai-0.778/
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-12 14:29:48.718798 dequeai-0.778/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:29:48.718798 dequeai-0.778/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.778/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.778/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.778/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.778/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-04-26 15:26:45.000000 dequeai-0.778/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    29698 2023-05-12 14:29:29.000000 dequeai-0.778/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.778/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.778/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.778/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.778/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:29:48.718798 dequeai-0.778/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-12 14:29:48.000000 dequeai-0.778/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-05-12 14:29:48.000000 dequeai-0.778/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 14:29:48.000000 dequeai-0.778/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-05-12 14:29:48.000000 dequeai-0.778/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-12 14:29:48.000000 dequeai-0.778/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 14:29:48.718798 dequeai-0.778/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      583 2023-05-12 14:29:29.000000 dequeai-0.778/setup.py
```

### Comparing `dequeai-0.7777/dequeai/datatypes.py` & `dequeai-0.778/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.7777/dequeai/dequeai.py` & `dequeai-0.778/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.7777/dequeai/dequeai_run.py` & `dequeai-0.778/dequeai/dequeai_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,15 +327,15 @@
                 else:
                     # TODO: for google we need a different way to save data
                     object_text = f.read()
                     headers = {'Content-type': "application/octet-stream"}
                     http_response = requests.put(url=res['url'], data=object_text, headers=headers)
                 print(http_response)
             req_data = {"user_name": self.user_name, "destination_path": dest_path, "artifact_type": artifact_type,
-                        "project_name": self._project_name, "run_id": self._run_id, "artifact_uris": [dest_path]}
+                        "project_name": self._project_name, "run_id": self._run_id, "artifact_uri": dest_path}
             resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/artifact/metadata/create/",
                                  json=req_data)
             res = resp.json()
             print(res)
 
     def register_artifacts(self, latest=True, label=None, tags=None):
         if not self._model_logged:
```

### Comparing `dequeai-0.7777/dequeai/parsing_service.py` & `dequeai-0.778/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.7777/dequeai/rest_connect.py` & `dequeai-0.778/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.7777/dequeai/util.py` & `dequeai-0.778/dequeai/util.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.7777/setup.py` & `dequeai-0.778/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, Extension
 
 
 setup(
     name='dequeai',
-    version='0.000007777',
+    version='0.00000778',
     description='Python Experiment Tracking Package for Deque AI DLOps Platform',
     author="The Deque AI Team",
     author_email='team@deque.app',
     packages=["dequeai"],
     url='https://dequeapp-deque.gitbook.io/deque-docs/getting-started/dequeai-experiment-tracking',
     keywords='deque client for experiment tracking, sweep and other deep learning tooling',
     install_requires=[
```


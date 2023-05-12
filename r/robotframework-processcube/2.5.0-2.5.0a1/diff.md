# Comparing `tmp/robotframework-processcube-2.5.0.tar.gz` & `tmp/robotframework-processcube-2.5.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-processcube-2.5.0.tar", last modified: Fri May 12 06:50:49 2023, max compression
+gzip compressed data, was "robotframework-processcube-2.5.0a1.tar", last modified: Fri May 12 07:30:22 2023, max compression
```

## Comparing `robotframework-processcube-2.5.0.tar` & `robotframework-processcube-2.5.0a1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:50:49.622843 robotframework-processcube-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    15967 2023-05-12 06:50:49.622843 robotframework-processcube-2.5.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:50:49.618843 robotframework-processcube-2.5.0/ProcessCubeLibrary/
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-12 06:50:37.000000 robotframework-processcube-2.5.0/ProcessCubeLibrary/ProcessCubeLibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-12 06:50:37.000000 robotframework-processcube-2.5.0/ProcessCubeLibrary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-12 06:50:37.000000 robotframework-processcube-2.5.0/ProcessCubeLibrary/docker_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:50:49.622843 robotframework-processcube-2.5.0/ProcessCubeLibrary/keywords/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-12 06:50:37.000000 robotframework-processcube-2.5.0/ProcessCubeLibrary/keywords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-12 06:50:37.000000 robotframework-processcube-2.5.0/ProcessCubeLibrary/keywords/_fields_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-12 06:50:37.000000 robotframework-processcube-2.5.0/ProcessCubeLibrary/keywords/_retry_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-12 06:50:37.000000 robotframework-processcube-2.5.0/ProcessCubeLibrary/keywords/deploy_keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-12 06:50:37.000000 robotframework-processcube-2.5.0/ProcessCubeLibrary/keywords/empty_task_keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-12 06:50:37.000000 robotframework-processcube-2.5.0/ProcessCubeLibrary/keywords/engine_keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-12 06:50:37.000000 robotframework-processcube-2.5.0/ProcessCubeLibrary/keywords/external_task_keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-12 06:50:37.000000 robotframework-processcube-2.5.0/ProcessCubeLibrary/keywords/manual_task_keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-12 06:50:37.000000 robotframework-processcube-2.5.0/ProcessCubeLibrary/keywords/process_instance_keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-12 06:50:37.000000 robotframework-processcube-2.5.0/ProcessCubeLibrary/keywords/send_keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-12 06:50:37.000000 robotframework-processcube-2.5.0/ProcessCubeLibrary/keywords/start_keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-12 06:50:37.000000 robotframework-processcube-2.5.0/ProcessCubeLibrary/keywords/user_task_keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)    15231 2023-05-12 06:50:37.000000 robotframework-processcube-2.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:50:49.622843 robotframework-processcube-2.5.0/robotframework_processcube.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15967 2023-05-12 06:50:49.000000 robotframework-processcube-2.5.0/robotframework_processcube.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-12 06:50:49.000000 robotframework-processcube-2.5.0/robotframework_processcube.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 06:50:49.000000 robotframework-processcube-2.5.0/robotframework_processcube.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-12 06:50:49.000000 robotframework-processcube-2.5.0/robotframework_processcube.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-12 06:50:49.000000 robotframework-processcube-2.5.0/robotframework_processcube.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 06:50:49.622843 robotframework-processcube-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-12 06:50:49.000000 robotframework-processcube-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:30:22.257002 robotframework-processcube-2.5.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    15969 2023-05-12 07:30:22.257002 robotframework-processcube-2.5.0a1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:30:22.253002 robotframework-processcube-2.5.0a1/ProcessCubeLibrary/
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-12 07:30:09.000000 robotframework-processcube-2.5.0a1/ProcessCubeLibrary/ProcessCubeLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-12 07:30:09.000000 robotframework-processcube-2.5.0a1/ProcessCubeLibrary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-12 07:30:09.000000 robotframework-processcube-2.5.0a1/ProcessCubeLibrary/docker_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:30:22.257002 robotframework-processcube-2.5.0a1/ProcessCubeLibrary/keywords/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-12 07:30:09.000000 robotframework-processcube-2.5.0a1/ProcessCubeLibrary/keywords/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-12 07:30:09.000000 robotframework-processcube-2.5.0a1/ProcessCubeLibrary/keywords/_fields_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-12 07:30:09.000000 robotframework-processcube-2.5.0a1/ProcessCubeLibrary/keywords/_retry_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-12 07:30:09.000000 robotframework-processcube-2.5.0a1/ProcessCubeLibrary/keywords/deploy_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-12 07:30:09.000000 robotframework-processcube-2.5.0a1/ProcessCubeLibrary/keywords/empty_task_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-12 07:30:09.000000 robotframework-processcube-2.5.0a1/ProcessCubeLibrary/keywords/engine_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-12 07:30:09.000000 robotframework-processcube-2.5.0a1/ProcessCubeLibrary/keywords/external_task_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-12 07:30:09.000000 robotframework-processcube-2.5.0a1/ProcessCubeLibrary/keywords/manual_task_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-12 07:30:09.000000 robotframework-processcube-2.5.0a1/ProcessCubeLibrary/keywords/process_instance_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-12 07:30:09.000000 robotframework-processcube-2.5.0a1/ProcessCubeLibrary/keywords/send_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-12 07:30:09.000000 robotframework-processcube-2.5.0a1/ProcessCubeLibrary/keywords/start_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-12 07:30:09.000000 robotframework-processcube-2.5.0a1/ProcessCubeLibrary/keywords/user_task_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15231 2023-05-12 07:30:09.000000 robotframework-processcube-2.5.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:30:22.257002 robotframework-processcube-2.5.0a1/robotframework_processcube.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15969 2023-05-12 07:30:22.000000 robotframework-processcube-2.5.0a1/robotframework_processcube.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-12 07:30:22.000000 robotframework-processcube-2.5.0a1/robotframework_processcube.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 07:30:22.000000 robotframework-processcube-2.5.0a1/robotframework_processcube.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-12 07:30:22.000000 robotframework-processcube-2.5.0a1/robotframework_processcube.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-12 07:30:22.000000 robotframework-processcube-2.5.0a1/robotframework_processcube.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 07:30:22.257002 robotframework-processcube-2.5.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-12 07:30:21.000000 robotframework-processcube-2.5.0a1/setup.py
```

### Comparing `robotframework-processcube-2.5.0/PKG-INFO` & `robotframework-processcube-2.5.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-processcube
-Version: 2.5.0
+Version: 2.5.0a1
 Summary: Robot Framework Keywords for processcube workflow engine.
 Home-page: https://github.com/atlas-engine-contrib/robotframework-processcube
 Author: 5Minds IT-Solutions GmbH & Co. KG
 Author-email: processcube@5minds.de
 License: MIT Licence
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `robotframework-processcube-2.5.0/ProcessCubeLibrary/ProcessCubeLibrary.py` & `robotframework-processcube-2.5.0a1/ProcessCubeLibrary/ProcessCubeLibrary.py`

 * *Files identical despite different names*

### Comparing `robotframework-processcube-2.5.0/ProcessCubeLibrary/docker_handler.py` & `robotframework-processcube-2.5.0a1/ProcessCubeLibrary/docker_handler.py`

 * *Files identical despite different names*

### Comparing `robotframework-processcube-2.5.0/ProcessCubeLibrary/keywords/_retry_helper.py` & `robotframework-processcube-2.5.0a1/ProcessCubeLibrary/keywords/_retry_helper.py`

 * *Files identical despite different names*

### Comparing `robotframework-processcube-2.5.0/ProcessCubeLibrary/keywords/deploy_keyword.py` & `robotframework-processcube-2.5.0a1/ProcessCubeLibrary/keywords/deploy_keyword.py`

 * *Files identical despite different names*

### Comparing `robotframework-processcube-2.5.0/ProcessCubeLibrary/keywords/empty_task_keyword.py` & `robotframework-processcube-2.5.0a1/ProcessCubeLibrary/keywords/empty_task_keyword.py`

 * *Files identical despite different names*

### Comparing `robotframework-processcube-2.5.0/ProcessCubeLibrary/keywords/external_task_keyword.py` & `robotframework-processcube-2.5.0a1/ProcessCubeLibrary/keywords/external_task_keyword.py`

 * *Files identical despite different names*

### Comparing `robotframework-processcube-2.5.0/ProcessCubeLibrary/keywords/manual_task_keyword.py` & `robotframework-processcube-2.5.0a1/ProcessCubeLibrary/keywords/manual_task_keyword.py`

 * *Files identical despite different names*

### Comparing `robotframework-processcube-2.5.0/ProcessCubeLibrary/keywords/process_instance_keyword.py` & `robotframework-processcube-2.5.0a1/ProcessCubeLibrary/keywords/process_instance_keyword.py`

 * *Files identical despite different names*

### Comparing `robotframework-processcube-2.5.0/ProcessCubeLibrary/keywords/send_keyword.py` & `robotframework-processcube-2.5.0a1/ProcessCubeLibrary/keywords/send_keyword.py`

 * *Files identical despite different names*

### Comparing `robotframework-processcube-2.5.0/ProcessCubeLibrary/keywords/start_keyword.py` & `robotframework-processcube-2.5.0a1/ProcessCubeLibrary/keywords/start_keyword.py`

 * *Files identical despite different names*

### Comparing `robotframework-processcube-2.5.0/ProcessCubeLibrary/keywords/user_task_keyword.py` & `robotframework-processcube-2.5.0a1/ProcessCubeLibrary/keywords/user_task_keyword.py`

 * *Files identical despite different names*

### Comparing `robotframework-processcube-2.5.0/README.md` & `robotframework-processcube-2.5.0a1/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-processcube-2.5.0/robotframework_processcube.egg-info/PKG-INFO` & `robotframework-processcube-2.5.0a1/robotframework_processcube.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-processcube
-Version: 2.5.0
+Version: 2.5.0a1
 Summary: Robot Framework Keywords for processcube workflow engine.
 Home-page: https://github.com/atlas-engine-contrib/robotframework-processcube
 Author: 5Minds IT-Solutions GmbH & Co. KG
 Author-email: processcube@5minds.de
 License: MIT Licence
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `robotframework-processcube-2.5.0/robotframework_processcube.egg-info/SOURCES.txt` & `robotframework-processcube-2.5.0a1/robotframework_processcube.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-processcube-2.5.0/setup.py` & `robotframework-processcube-2.5.0a1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 name = "5Minds IT-Solutions GmbH & Co. KG"
 
 setuptools.setup(
     name="robotframework-processcube",
-    version=setuptools.sic('2.5.0'),
+    version=setuptools.sic('2.5.0-alpha.1'),
     description="Robot Framework Keywords for processcube workflow engine.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author=name,
     author_email="processcube@5minds.de",
     url="https://github.com/atlas-engine-contrib/robotframework-processcube",
     packages=setuptools.find_packages(),
```


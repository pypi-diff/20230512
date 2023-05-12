# Comparing `tmp/rayasdk-1.1.0.dev1.tar.gz` & `tmp/rayasdk-1.1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rayasdk-1.1.0.dev1.tar", last modified: Wed May 10 18:26:23 2023, max compression
+gzip compressed data, was "rayasdk-1.1.0.dev2.tar", last modified: Fri May 12 17:02:31 2023, max compression
```

## Comparing `rayasdk-1.1.0.dev1.tar` & `rayasdk-1.1.0.dev2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 santiagour  (1000) santiagour  (1000)        0 2023-05-10 18:26:23.968736 rayasdk-1.1.0.dev1/
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      357 2023-05-10 18:26:23.968736 rayasdk-1.1.0.dev1/PKG-INFO
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)        0 2023-05-10 14:16:37.000000 rayasdk-1.1.0.dev1/README.md
-drwxrwxr-x   0 santiagour  (1000) santiagour  (1000)        0 2023-05-10 18:26:23.968736 rayasdk-1.1.0.dev1/rayasdk/
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      546 2023-05-10 14:28:01.000000 rayasdk-1.1.0.dev1/rayasdk/__init__.py
--rwxrwxr-x   0 santiagour  (1000) santiagour  (1000)     4888 2023-05-10 18:21:31.000000 rayasdk-1.1.0.dev1/rayasdk/__main__.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     5150 2023-05-10 16:24:09.000000 rayasdk-1.1.0.dev1/rayasdk/connect.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     6158 2023-05-10 17:43:43.000000 rayasdk-1.1.0.dev1/rayasdk/constants.py
-drwxrwxr-x   0 santiagour  (1000) santiagour  (1000)        0 2023-05-10 18:26:23.968736 rayasdk-1.1.0.dev1/rayasdk/container_handlers/
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)        0 2023-05-04 20:26:47.000000 rayasdk-1.1.0.dev1/rayasdk/container_handlers/__init__.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     3868 2023-05-10 17:43:57.000000 rayasdk-1.1.0.dev1/rayasdk/container_handlers/docker_handler.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     9834 2023-05-10 16:24:09.000000 rayasdk-1.1.0.dev1/rayasdk/container_handlers/vcs.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     2568 2023-05-10 14:28:01.000000 rayasdk-1.1.0.dev1/rayasdk/initializer.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     1342 2023-05-10 14:28:01.000000 rayasdk-1.1.0.dev1/rayasdk/killer.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     1346 2023-05-10 14:28:01.000000 rayasdk-1.1.0.dev1/rayasdk/logger.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      819 2023-05-10 14:28:01.000000 rayasdk-1.1.0.dev1/rayasdk/messages.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     6011 2023-05-10 18:11:03.000000 rayasdk-1.1.0.dev1/rayasdk/runner.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     4396 2023-05-10 16:24:09.000000 rayasdk-1.1.0.dev1/rayasdk/scanner.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     1767 2023-05-10 16:24:09.000000 rayasdk-1.1.0.dev1/rayasdk/simulator.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     2667 2023-05-10 16:38:58.000000 rayasdk-1.1.0.dev1/rayasdk/sshKeyGen.py
-drwxrwxr-x   0 santiagour  (1000) santiagour  (1000)        0 2023-05-10 18:26:23.968736 rayasdk-1.1.0.dev1/rayasdk/template/
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      244 2023-05-04 20:26:47.000000 rayasdk-1.1.0.dev1/rayasdk/template/__main__.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      551 2023-05-10 14:28:01.000000 rayasdk-1.1.0.dev1/rayasdk/template/app.py
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      399 2023-05-10 14:16:37.000000 rayasdk-1.1.0.dev1/rayasdk/template/launch.json
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      108 2023-05-04 20:26:47.000000 rayasdk-1.1.0.dev1/rayasdk/template/manifest.json
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     3113 2023-05-10 18:21:04.000000 rayasdk-1.1.0.dev1/rayasdk/utils.py
-drwxrwxr-x   0 santiagour  (1000) santiagour  (1000)        0 2023-05-10 18:26:23.968736 rayasdk-1.1.0.dev1/rayasdk.egg-info/
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      357 2023-05-10 18:26:23.000000 rayasdk-1.1.0.dev1/rayasdk.egg-info/PKG-INFO
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      702 2023-05-10 18:26:23.000000 rayasdk-1.1.0.dev1/rayasdk.egg-info/SOURCES.txt
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)        1 2023-05-10 18:26:23.000000 rayasdk-1.1.0.dev1/rayasdk.egg-info/dependency_links.txt
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)       51 2023-05-10 18:26:23.000000 rayasdk-1.1.0.dev1/rayasdk.egg-info/entry_points.txt
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      103 2023-05-10 18:26:23.000000 rayasdk-1.1.0.dev1/rayasdk.egg-info/requires.txt
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)        8 2023-05-10 18:26:23.000000 rayasdk-1.1.0.dev1/rayasdk.egg-info/top_level.txt
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)       79 2023-05-10 18:26:23.968736 rayasdk-1.1.0.dev1/setup.cfg
--rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     1002 2023-05-10 18:24:53.000000 rayasdk-1.1.0.dev1/setup.py
+drwxrwxr-x   0 santiagour  (1000) santiagour  (1000)        0 2023-05-12 17:02:31.632375 rayasdk-1.1.0.dev2/
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     6569 2023-05-12 17:02:31.632375 rayasdk-1.1.0.dev2/PKG-INFO
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     6219 2023-05-12 15:27:54.000000 rayasdk-1.1.0.dev2/README.md
+drwxrwxr-x   0 santiagour  (1000) santiagour  (1000)        0 2023-05-12 17:02:31.632375 rayasdk-1.1.0.dev2/rayasdk/
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      546 2023-05-10 14:28:01.000000 rayasdk-1.1.0.dev2/rayasdk/__init__.py
+-rwxrwxr-x   0 santiagour  (1000) santiagour  (1000)     4888 2023-05-10 18:21:31.000000 rayasdk-1.1.0.dev2/rayasdk/__main__.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     5150 2023-05-10 16:24:09.000000 rayasdk-1.1.0.dev2/rayasdk/connect.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     6202 2023-05-12 15:57:49.000000 rayasdk-1.1.0.dev2/rayasdk/constants.py
+drwxrwxr-x   0 santiagour  (1000) santiagour  (1000)        0 2023-05-12 17:02:31.632375 rayasdk-1.1.0.dev2/rayasdk/container_handlers/
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)        0 2023-05-04 20:26:47.000000 rayasdk-1.1.0.dev2/rayasdk/container_handlers/__init__.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     5576 2023-05-12 16:35:40.000000 rayasdk-1.1.0.dev2/rayasdk/container_handlers/docker_handler.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     9930 2023-05-12 17:01:05.000000 rayasdk-1.1.0.dev2/rayasdk/container_handlers/vcs.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     2568 2023-05-10 14:28:01.000000 rayasdk-1.1.0.dev2/rayasdk/initializer.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     1342 2023-05-10 14:28:01.000000 rayasdk-1.1.0.dev2/rayasdk/killer.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     1346 2023-05-10 14:28:01.000000 rayasdk-1.1.0.dev2/rayasdk/logger.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      819 2023-05-10 14:28:01.000000 rayasdk-1.1.0.dev2/rayasdk/messages.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     5993 2023-05-12 15:27:54.000000 rayasdk-1.1.0.dev2/rayasdk/runner.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     4396 2023-05-10 16:24:09.000000 rayasdk-1.1.0.dev2/rayasdk/scanner.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     1749 2023-05-12 15:27:54.000000 rayasdk-1.1.0.dev2/rayasdk/simulator.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     2667 2023-05-10 16:38:58.000000 rayasdk-1.1.0.dev2/rayasdk/sshKeyGen.py
+drwxrwxr-x   0 santiagour  (1000) santiagour  (1000)        0 2023-05-12 17:02:31.632375 rayasdk-1.1.0.dev2/rayasdk/template/
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      244 2023-05-04 20:26:47.000000 rayasdk-1.1.0.dev2/rayasdk/template/__main__.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      551 2023-05-10 14:28:01.000000 rayasdk-1.1.0.dev2/rayasdk/template/app.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      399 2023-05-10 14:16:37.000000 rayasdk-1.1.0.dev2/rayasdk/template/launch.json
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      108 2023-05-04 20:26:47.000000 rayasdk-1.1.0.dev2/rayasdk/template/manifest.json
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     3123 2023-05-12 15:27:59.000000 rayasdk-1.1.0.dev2/rayasdk/utils.py
+drwxrwxr-x   0 santiagour  (1000) santiagour  (1000)        0 2023-05-12 17:02:31.632375 rayasdk-1.1.0.dev2/rayasdk.egg-info/
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     6569 2023-05-12 17:02:31.000000 rayasdk-1.1.0.dev2/rayasdk.egg-info/PKG-INFO
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      702 2023-05-12 17:02:31.000000 rayasdk-1.1.0.dev2/rayasdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)        1 2023-05-12 17:02:31.000000 rayasdk-1.1.0.dev2/rayasdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)       51 2023-05-12 17:02:31.000000 rayasdk-1.1.0.dev2/rayasdk.egg-info/entry_points.txt
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      103 2023-05-12 17:02:31.000000 rayasdk-1.1.0.dev2/rayasdk.egg-info/requires.txt
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)        8 2023-05-12 17:02:31.000000 rayasdk-1.1.0.dev2/rayasdk.egg-info/top_level.txt
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)       79 2023-05-12 17:02:31.632375 rayasdk-1.1.0.dev2/setup.cfg
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      934 2023-05-12 17:02:21.000000 rayasdk-1.1.0.dev2/setup.py
```

### Comparing `rayasdk-1.1.0.dev1/rayasdk/__init__.py` & `rayasdk-1.1.0.dev2/rayasdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev1/rayasdk/__main__.py` & `rayasdk-1.1.0.dev2/rayasdk/__main__.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev1/rayasdk/connect.py` & `rayasdk-1.1.0.dev2/rayasdk/connect.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev1/rayasdk/constants.py` & `rayasdk-1.1.0.dev2/rayasdk/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright 2020 Unlimited Robotics
 import re
 import tempfile
 import platform
 import subprocess
 from pathlib import Path
 
-RAYAENV_DOCKER_VERSION_DEFAULT = '1.0.8'
-GARYSIM_VERSION_DEFAULT = '1.0.4'
+RAYAENV_DOCKER_VERSION_DEFAULT = '0.0.0'
+GARYSIM_VERSION_DEFAULT = '0.0.0'
 GARYSIM_VERSION = GARYSIM_VERSION_DEFAULT
 RAYAENV_DOCKER_VERSION = RAYAENV_DOCKER_VERSION_DEFAULT
 
 # Json SCAN Keys
 JSON_SCAN_ID = 'ROBOT_ID'
 JSON_SCAN_IP = 'ROBOT_IP'
 JSON_SCAN_SERIAL = 'ROBOT_SERIAL'
@@ -81,14 +81,15 @@
 EXECSETTINGS_PATH = CURRENT_PATH / EXECSETTINGS_FILE
 CONNECTION_SETTINGS_PATH = UR_HOME / CONNECTION_SETTINGS_FILE
 
 # Docker Environment
 RAYAENV_DOCKER_UR_ROOT = SIMS_HOME / 'ur_root'
 RAYAENV_DOCKER_UR_ROOT_REPO = 'git clone --branch garyunity git@github.com:Unlimited-Robotics/raya_root_folder_templates.git'
 RAYAENV_DOCKER_IMGNAME = 'raya_os'
+RAYAENV_DOCKER_IMGNAME_DEV = 'raya_sim_dev'
 RAYAENV_DOCKER_IMG_VERSION_NAME = 'sim'
 RAYAENV_DOCKER_IMG_VERSION_GPU = 'sim_gpu'
 
 
 def check_if_gpu():
     global RAYAENV_DOCKER_IMAGE_NAME
     return_code = subprocess.call(
```

### Comparing `rayasdk-1.1.0.dev1/rayasdk/container_handlers/vcs.py` & `rayasdk-1.1.0.dev2/rayasdk/container_handlers/vcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 
 
 def check_versions():
     vcs = URVCS()
     # If there is a major/minor version let the user know
     if not vcs.full_updated() or not vcs.minor_updated():
         log_warning('RayaOS is not up to date. To update run "rayasdk update"')
-        return False
-    # If there is a patch update available, ask the user if they want to update
+    # If there is a patch update available, update
     if not vcs.patch_updated():
         for cpm in RAYA_OS_COMPONENTS:
             if not vcs.patch_updated(cpm):
                 log_info(f'Updating {cpm}')
                 if not vcs.update_patch(cpm):
                     log_error(f'Could not update {cpm}')
                     return False
@@ -112,14 +111,15 @@
                 update_constants()
                 return True
         except:
             log_error('Error updating the constants file')
             return False
 
     def __update_sdk_packages(self):
+        return True
         try:
             pip_process = subprocess.Popen('pip install --upgrade rayasdk',
                                            shell=True,
                                            stdin=subprocess.PIPE,
                                            stdout=subprocess.PIPE,
                                            stderr=subprocess.PIPE)
             output, err = pip_process.communicate()
@@ -142,33 +142,35 @@
 
     def update_full(self):
 
         # update SDK
         if self.__get_latest_version('SDK') != self.__local_version('SDK'):
             if not self.__update_sdk_packages():
                 return False
-            log_info('Simulator updated successfully')
+            self.__update_constants_file('SDK')
+            log_warning('SDK updated successfully')
 
         # Update Unity
-        if self.__get_latest_version('Unity') != self.__local_version('Unity'):
+        if self.__get_latest_version('Unity') != self.__local_version(
+                'Unity') or not os.path.exists(f'{SIM_BINARY}'):
             response = requests.request("GET", VCS_URL)
             if not download_simulator(response=response.json()):
                 return False
+            self.__update_constants_file('Unity')
             log_warning('Simulator updated successfully')
 
         # Update Docker
         if self.__get_latest_version('Docker') != self.__local_version(
-                'Docker'):
+                'Docker') or not check_image():
             version = self.__get_latest_version('Docker')
             if not download_raya_image(version):
                 return False
+            self.__update_constants_file('Docker')
             log_warning('Raya_OS updated successfully')
 
-        for component in RAYA_OS_COMPONENTS:
-            self.__update_constants_file(component)
         return True
 
     def minor_updated(self, component=None):
         '''Function to check if the latest version is a minor version'''
         if component:
             local = self.__local_version(component)
             latest = self.__get_latest_version(component)
```

### Comparing `rayasdk-1.1.0.dev1/rayasdk/initializer.py` & `rayasdk-1.1.0.dev2/rayasdk/initializer.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev1/rayasdk/killer.py` & `rayasdk-1.1.0.dev2/rayasdk/killer.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev1/rayasdk/logger.py` & `rayasdk-1.1.0.dev2/rayasdk/logger.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev1/rayasdk/messages.py` & `rayasdk-1.1.0.dev2/rayasdk/messages.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev1/rayasdk/runner.py` & `rayasdk-1.1.0.dev2/rayasdk/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
     def init_parser(self, subparser):
         self.parser = subparser.add_parser(
             type(self).COMMAND,
             add_help=False,
             help="connect current raya project to a robot or simulator.")
         self.parser.add_argument(
-            '-d',
             '--debug',
             help='runs applications in debug mode',
             action="store_true",
         )
 
     def run(self, args, unknownargs):
         self.args = args
```

### Comparing `rayasdk-1.1.0.dev1/rayasdk/scanner.py` & `rayasdk-1.1.0.dev2/rayasdk/scanner.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev1/rayasdk/simulator.py` & `rayasdk-1.1.0.dev2/rayasdk/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     def __init__(self):
         pass
 
     def init_parser(self, subparser):
         self.parser = subparser.add_parser(type(self).COMMAND,
                                            help="run the simulator bridge.")
         self.parser.add_argument(
-            '-d',
             '--debug',
             help='Runs only the unity simulation for dev on the container',
             action="store_true")
 
     def run(self, args, unknownargs):
         self.args = args
         self.unknownargs = unknownargs
```

### Comparing `rayasdk-1.1.0.dev1/rayasdk/sshKeyGen.py` & `rayasdk-1.1.0.dev2/rayasdk/sshKeyGen.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev1/rayasdk/template/app.py` & `rayasdk-1.1.0.dev2/rayasdk/template/app.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev1/rayasdk/utils.py` & `rayasdk-1.1.0.dev2/rayasdk/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,9 +98,10 @@
 
 def open_connection_file():
     try:
         with open(CONNECTION_SETTINGS_PATH, 'r', encoding='utf-8') as f:
             connection_settings = json.load(f)
         return connection_settings
     except OSError:
-        raise Exception((f'the file "{CONNECTION_SETTINGS_FILE}" was not found, '
-                'run \'rayasdk connect\''))
+        raise Exception(
+            (f'the file "{CONNECTION_SETTINGS_FILE}" was not found, '
+             'run \'rayasdk connect\''))
```

### Comparing `rayasdk-1.1.0.dev1/rayasdk.egg-info/SOURCES.txt` & `rayasdk-1.1.0.dev2/rayasdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rayasdk-1.1.0.dev1/setup.py` & `rayasdk-1.1.0.dev2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 from setuptools import setup, find_packages
 
-
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='rayasdk',
     packages=find_packages(),
-    version='1.1.0.dev1',
+    version='1.1.0.dev2',
     license='MIT',
     description='Raya SDK - Unlimited Robotics Software Development Kit',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Unlimited Robotics',
     author_email='camilo@unlimited-robotics.com',
     url='',
     python_requires=">=3.8",
-    download_url = '',
-    package_data={'':['./template/*']},
-    keywords = ['robotics', 'unlimited-robotics', 'gary'],
+    download_url='',
+    package_data={'': ['./template/*']},
+    keywords=['robotics', 'unlimited-robotics', 'gary'],
     install_requires=[
-        'tabulate',
-        'importlib_metadata',
-        'tqdm',
-        'docker',
-        'progressbar',
-        'simple_file_checksum', 
-        'gsutil',
-        'zeroconf',
-        'raya',
-        'paramiko'
+        'tabulate', 'importlib_metadata', 'tqdm', 'docker', 'progressbar',
+        'simple_file_checksum', 'gsutil', 'zeroconf', 'raya', 'paramiko'
     ],
     entry_points={
         'console_scripts': [
             'rayasdk = rayasdk.__main__:main',
         ],
     },
-)
+)
```


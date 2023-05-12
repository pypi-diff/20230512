# Comparing `tmp/connpy-3.2.3.tar.gz` & `tmp/connpy-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connpy-3.2.3.tar", last modified: Fri May 12 15:06:29 2023, max compression
+gzip compressed data, was "connpy-3.2.4.tar", last modified: Fri May 12 21:32:13 2023, max compression
```

## Comparing `connpy-3.2.3.tar` & `connpy-3.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:06:29.679170 connpy-3.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-12 15:06:18.000000 connpy-3.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-12 15:06:29.679170 connpy-3.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-05-12 15:06:18.000000 connpy-3.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:06:29.679170 connpy-3.2.3/connpy/
--rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-05-12 15:06:18.000000 connpy-3.2.3/connpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-12 15:06:18.000000 connpy-3.2.3/connpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 15:06:18.000000 connpy-3.2.3/connpy/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20394 2023-05-12 15:06:18.000000 connpy-3.2.3/connpy/ai.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5102 2023-05-12 15:06:18.000000 connpy-3.2.3/connpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-12 15:06:18.000000 connpy-3.2.3/connpy/completion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15540 2023-05-12 15:06:18.000000 connpy-3.2.3/connpy/configfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    50300 2023-05-12 15:06:18.000000 connpy-3.2.3/connpy/connapp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28719 2023-05-12 15:06:18.000000 connpy-3.2.3/connpy/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:06:29.679170 connpy-3.2.3/connpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-12 15:06:29.000000 connpy-3.2.3/connpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-12 15:06:29.000000 connpy-3.2.3/connpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:06:29.000000 connpy-3.2.3/connpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-12 15:06:29.000000 connpy-3.2.3/connpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-12 15:06:29.000000 connpy-3.2.3/connpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 15:06:29.000000 connpy-3.2.3/connpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-12 15:06:29.679170 connpy-3.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 15:06:18.000000 connpy-3.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:32:13.237972 connpy-3.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-12 21:31:58.000000 connpy-3.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-12 21:32:13.237972 connpy-3.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-05-12 21:31:58.000000 connpy-3.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:32:13.237972 connpy-3.2.4/connpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-05-12 21:31:58.000000 connpy-3.2.4/connpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-12 21:31:58.000000 connpy-3.2.4/connpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 21:31:58.000000 connpy-3.2.4/connpy/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20694 2023-05-12 21:31:58.000000 connpy-3.2.4/connpy/ai.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5102 2023-05-12 21:31:58.000000 connpy-3.2.4/connpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-12 21:31:58.000000 connpy-3.2.4/connpy/completion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15540 2023-05-12 21:31:58.000000 connpy-3.2.4/connpy/configfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50300 2023-05-12 21:31:58.000000 connpy-3.2.4/connpy/connapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28719 2023-05-12 21:31:58.000000 connpy-3.2.4/connpy/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:32:13.237972 connpy-3.2.4/connpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-12 21:32:13.000000 connpy-3.2.4/connpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-12 21:32:13.000000 connpy-3.2.4/connpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 21:32:13.000000 connpy-3.2.4/connpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-12 21:32:13.000000 connpy-3.2.4/connpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-12 21:32:13.000000 connpy-3.2.4/connpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 21:32:13.000000 connpy-3.2.4/connpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-12 21:32:13.237972 connpy-3.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 21:31:58.000000 connpy-3.2.4/setup.py
```

### Comparing `connpy-3.2.3/LICENSE` & `connpy-3.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `connpy-3.2.3/PKG-INFO` & `connpy-3.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.2.3
+Version: 3.2.4
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
```

### Comparing `connpy-3.2.3/README.md` & `connpy-3.2.4/README.md`

 * *Files identical despite different names*

### Comparing `connpy-3.2.3/connpy/__init__.py` & `connpy-3.2.4/connpy/__init__.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.3/connpy/ai.py` & `connpy-3.2.4/connpy/ai.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,27 +91,29 @@
                 Filter: {{filter}}
                 Expected: {{expected}}
                 Response: {{response}}
     """ 
         self.__prompt["original_user"] = "Get the IP addresses of loopback0 for all routers from w2az1 and e1.*(prod|dev) and check if they have the ip 192.168.1.1"
         self.__prompt["original_assistant"] = "app_related: True\nType: Command\nFilter: ['w2az1', 'e1.*(prod|dev)']\nExpected: 192.168.1.1"
         self.__prompt["command_system"] = """
-    For each device listed below, provide the command(s) needed to perform the specified action, depending on the device OS (e.g., Cisco IOSXR router, Linux server). Always format your response as a Python list (e.g., ['command1', 'command2']). 
+        For each device listed below, provide the command(s) needed to perform the specified action, depending on the device OS (e.g., Cisco IOSXR router, Linux server). Always format your response as a Python list (e.g., ['command1', 'command2']). 
 
-    Note that the application knows how to connect to devices via SSH, so you only need to provide the command(s) to run after connecting. 
+        It's very important to note: If a user has provided a specific command to be run, you should include that command exactly as provided, even if it's not recognized or understood. No alterations should be made to the user-provided commands under any circumstances. 
 
-    If the commands needed are not for the specific OS type, just send an empty list (e.g., []).
+        The application knows how to connect to devices via SSH, so you only need to provide the command(s) to run after connecting. 
 
-    It is crucial to always include the device name provided in your response, even when there is only one device.
+        If the commands needed are not for the specific OS type, just send an empty list (e.g., []). 
 
-    your response has to be always like this:
-        node1: ["command1", "command2"]
-        node2: ["command1", "command2", "command3"]
-        node1@folder: ["command1"]
-        Node4@subfolder@folder: []
+        It is crucial to always include the device name provided in your response, even when there is only one device.
+
+        Your response has to be always like this:
+            node1: ["command1", "command2"]
+            node2: ["command1", "command2", "command3"]
+            node1@folder: ["command1"]
+            Node4@subfolder@folder: []
     """
         self.__prompt["command_user"]= """
     input: show me the full configuration for all this devices:
 
     Devices:
     router1: cisco ios
     """
```

### Comparing `connpy-3.2.3/connpy/api.py` & `connpy-3.2.4/connpy/api.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.3/connpy/completion.py` & `connpy-3.2.4/connpy/completion.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.3/connpy/configfile.py` & `connpy-3.2.4/connpy/configfile.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.3/connpy/connapp.py` & `connpy-3.2.4/connpy/connapp.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.3/connpy/core.py` & `connpy-3.2.4/connpy/core.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.3/connpy.egg-info/PKG-INFO` & `connpy-3.2.4/connpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.2.3
+Version: 3.2.4
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
```

### Comparing `connpy-3.2.3/setup.cfg` & `connpy-3.2.4/setup.cfg`

 * *Files identical despite different names*


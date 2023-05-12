# Comparing `tmp/pybuilder-integration-87.tar.gz` & `tmp/pybuilder-integration-88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybuilder-integration-87.tar", last modified: Wed Mar  1 16:45:46 2023, max compression
+gzip compressed data, was "pybuilder-integration-88.tar", last modified: Fri May 12 17:54:17 2023, max compression
```

## Comparing `pybuilder-integration-87.tar` & `pybuilder-integration-88.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 16:45:46.585518 pybuilder-integration-87/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-01 16:45:46.585518 pybuilder-integration-87/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 16:45:46.585518 pybuilder-integration-87/pybuilder_integration/
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-03-01 16:45:16.000000 pybuilder-integration-87/pybuilder_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-03-01 16:45:16.000000 pybuilder-integration-87/pybuilder_integration/artifact_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-03-01 16:45:16.000000 pybuilder-integration-87/pybuilder_integration/cloudwatchlogs_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-03-01 16:45:16.000000 pybuilder-integration-87/pybuilder_integration/directory_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-03-01 16:45:16.000000 pybuilder-integration-87/pybuilder_integration/exec_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-01 16:45:16.000000 pybuilder-integration-87/pybuilder_integration/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-03-01 16:45:16.000000 pybuilder-integration-87/pybuilder_integration/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-03-01 16:45:16.000000 pybuilder-integration-87/pybuilder_integration/tool_utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 16:45:46.585518 pybuilder-integration-87/pybuilder_integration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-01 16:45:46.000000 pybuilder-integration-87/pybuilder_integration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-01 16:45:46.000000 pybuilder-integration-87/pybuilder_integration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 16:45:46.000000 pybuilder-integration-87/pybuilder_integration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 16:45:46.000000 pybuilder-integration-87/pybuilder_integration.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-01 16:45:46.000000 pybuilder-integration-87/pybuilder_integration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-01 16:45:46.000000 pybuilder-integration-87/pybuilder_integration.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 16:45:46.000000 pybuilder-integration-87/pybuilder_integration.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 16:45:46.585518 pybuilder-integration-87/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1682 2023-03-01 16:45:44.000000 pybuilder-integration-87/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:17.092278 pybuilder-integration-88/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-12 17:54:17.092278 pybuilder-integration-88/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:17.092278 pybuilder-integration-88/pybuilder_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-12 17:53:39.000000 pybuilder-integration-88/pybuilder_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-05-12 17:53:39.000000 pybuilder-integration-88/pybuilder_integration/artifact_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-12 17:53:39.000000 pybuilder-integration-88/pybuilder_integration/cloudwatchlogs_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-12 17:53:39.000000 pybuilder-integration-88/pybuilder_integration/directory_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-12 17:53:39.000000 pybuilder-integration-88/pybuilder_integration/exec_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-12 17:53:39.000000 pybuilder-integration-88/pybuilder_integration/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-05-12 17:53:39.000000 pybuilder-integration-88/pybuilder_integration/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-12 17:53:39.000000 pybuilder-integration-88/pybuilder_integration/tool_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:54:17.092278 pybuilder-integration-88/pybuilder_integration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-12 17:54:17.000000 pybuilder-integration-88/pybuilder_integration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-12 17:54:17.000000 pybuilder-integration-88/pybuilder_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:54:17.000000 pybuilder-integration-88/pybuilder_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:54:17.000000 pybuilder-integration-88/pybuilder_integration.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-12 17:54:17.000000 pybuilder-integration-88/pybuilder_integration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-12 17:54:17.000000 pybuilder-integration-88/pybuilder_integration.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:54:17.000000 pybuilder-integration-88/pybuilder_integration.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 17:54:17.092278 pybuilder-integration-88/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1682 2023-05-12 17:54:15.000000 pybuilder-integration-88/setup.py
```

### Comparing `pybuilder-integration-87/PKG-INFO` & `pybuilder-integration-88/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybuilder-integration
-Version: 87
+Version: 88
 Summary: A pybuilder plugin that runs integration tests (Tavern & Cypress) against a target.
 Home-page: https://github.com/rspitler/pybuilder-integration
 Author: 
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: Apache 2.0
```

### Comparing `pybuilder-integration-87/pybuilder_integration/__init__.py` & `pybuilder-integration-88/pybuilder_integration/__init__.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-87/pybuilder_integration/artifact_manager.py` & `pybuilder-integration-88/pybuilder_integration/artifact_manager.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-87/pybuilder_integration/cloudwatchlogs_utility.py` & `pybuilder-integration-88/pybuilder_integration/cloudwatchlogs_utility.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-87/pybuilder_integration/directory_utility.py` & `pybuilder-integration-88/pybuilder_integration/directory_utility.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-87/pybuilder_integration/exec_utility.py` & `pybuilder-integration-88/pybuilder_integration/exec_utility.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-87/pybuilder_integration/properties.py` & `pybuilder-integration-88/pybuilder_integration/properties.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-87/pybuilder_integration/tasks.py` & `pybuilder-integration-88/pybuilder_integration/tasks.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-87/pybuilder_integration/tool_utility.py` & `pybuilder-integration-88/pybuilder_integration/tool_utility.py`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-87/pybuilder_integration.egg-info/PKG-INFO` & `pybuilder-integration-88/pybuilder_integration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybuilder-integration
-Version: 87
+Version: 88
 Summary: A pybuilder plugin that runs integration tests (Tavern & Cypress) against a target.
 Home-page: https://github.com/rspitler/pybuilder-integration
 Author: 
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: Apache 2.0
```

### Comparing `pybuilder-integration-87/pybuilder_integration.egg-info/SOURCES.txt` & `pybuilder-integration-88/pybuilder_integration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybuilder-integration-87/setup.py` & `pybuilder-integration-88/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         _install.run(self)
 
         self.post_install_script()
 
 if __name__ == '__main__':
     setup(
         name = 'pybuilder-integration',
-        version = '87',
+        version = '88',
         description = 'A pybuilder plugin that runs integration tests (Tavern & Cypress) against a target.',
         long_description = 'A pybuilder plugin that runs integration tests against a target.  This is intended to be a broader scope than unit-tests encompassing dependant functionality.',
         long_description_content_type = None,
         classifiers = [
             'Development Status :: 3 - Alpha',
             'Programming Language :: Python'
         ],
```


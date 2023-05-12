# Comparing `tmp/autotraders-0.1.4.tar.gz` & `tmp/autotraders-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-0.1.4.tar", last modified: Fri May 12 17:32:04 2023, max compression
+gzip compressed data, was "autotraders-0.1.5.tar", last modified: Fri May 12 17:33:13 2023, max compression
```

## Comparing `autotraders-0.1.4.tar` & `autotraders-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:32:04.393057 autotraders-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-12 17:31:47.000000 autotraders-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-12 17:32:04.393057 autotraders-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-12 17:31:47.000000 autotraders-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:32:04.393057 autotraders-0.1.4/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:31:47.000000 autotraders-0.1.4/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-12 17:31:47.000000 autotraders-0.1.4/autotraders/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-12 17:31:47.000000 autotraders-0.1.4/autotraders/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-12 17:31:47.000000 autotraders-0.1.4/autotraders/ships.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-12 17:31:47.000000 autotraders-0.1.4/autotraders/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-12 17:31:47.000000 autotraders-0.1.4/autotraders/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:32:04.393057 autotraders-0.1.4/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-12 17:32:04.000000 autotraders-0.1.4/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-12 17:32:04.000000 autotraders-0.1.4/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:32:04.000000 autotraders-0.1.4/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-12 17:32:04.000000 autotraders-0.1.4/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-12 17:31:47.000000 autotraders-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 17:32:04.393057 autotraders-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:33:13.556688 autotraders-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-12 17:33:01.000000 autotraders-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-12 17:33:13.556688 autotraders-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-12 17:33:01.000000 autotraders-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:33:13.552688 autotraders-0.1.5/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:33:01.000000 autotraders-0.1.5/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-12 17:33:01.000000 autotraders-0.1.5/autotraders/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-12 17:33:01.000000 autotraders-0.1.5/autotraders/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-12 17:33:01.000000 autotraders-0.1.5/autotraders/ships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-12 17:33:01.000000 autotraders-0.1.5/autotraders/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-12 17:33:01.000000 autotraders-0.1.5/autotraders/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:33:13.556688 autotraders-0.1.5/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-12 17:33:13.000000 autotraders-0.1.5/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-12 17:33:13.000000 autotraders-0.1.5/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:33:13.000000 autotraders-0.1.5/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-12 17:33:13.000000 autotraders-0.1.5/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-12 17:33:01.000000 autotraders-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 17:33:13.556688 autotraders-0.1.5/setup.cfg
```

### Comparing `autotraders-0.1.4/LICENSE` & `autotraders-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-0.1.4/PKG-INFO` & `autotraders-0.1.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 0.1.4
+Version: 0.1.5
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://github.com/arihant2math/autotraders
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `autotraders-0.1.4/README.md` & `autotraders-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-0.1.4/autotraders/agent.py` & `autotraders-0.1.5/autotraders/agent.py`

 * *Files identical despite different names*

### Comparing `autotraders-0.1.4/autotraders/contract.py` & `autotraders-0.1.5/autotraders/contract.py`

 * *Files identical despite different names*

### Comparing `autotraders-0.1.4/autotraders/ships.py` & `autotraders-0.1.5/autotraders/ships.py`

 * *Files identical despite different names*

### Comparing `autotraders-0.1.4/autotraders/system.py` & `autotraders-0.1.5/autotraders/system.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from autotraders import Waypoint
+from autotraders.waypoint import Waypoint
 
 
 class System:
     def __init__(self, symbol, session, update=True):
         self.session = session
         self.symbol = symbol
         self.waypoints = []
```

### Comparing `autotraders-0.1.4/autotraders/waypoint.py` & `autotraders-0.1.5/autotraders/waypoint.py`

 * *Files identical despite different names*

### Comparing `autotraders-0.1.4/autotraders.egg-info/PKG-INFO` & `autotraders-0.1.5/autotraders.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 0.1.4
+Version: 0.1.5
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://github.com/arihant2math/autotraders
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `autotraders-0.1.4/pyproject.toml` & `autotraders-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "autotraders"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```


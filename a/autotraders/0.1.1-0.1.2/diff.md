# Comparing `tmp/autotraders-0.1.1.tar.gz` & `tmp/autotraders-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-0.1.1.tar", last modified: Fri May 12 17:19:46 2023, max compression
+gzip compressed data, was "autotraders-0.1.2.tar", last modified: Fri May 12 17:25:27 2023, max compression
```

## Comparing `autotraders-0.1.1.tar` & `autotraders-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:19:46.946435 autotraders-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-12 17:19:34.000000 autotraders-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-12 17:19:46.946435 autotraders-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-12 17:19:34.000000 autotraders-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:19:46.946435 autotraders-0.1.1/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-12 17:19:34.000000 autotraders-0.1.1/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-12 17:19:34.000000 autotraders-0.1.1/autotraders/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-12 17:19:34.000000 autotraders-0.1.1/autotraders/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-12 17:19:34.000000 autotraders-0.1.1/autotraders/ships.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-12 17:19:34.000000 autotraders-0.1.1/autotraders/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-12 17:19:34.000000 autotraders-0.1.1/autotraders/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:19:46.946435 autotraders-0.1.1/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-12 17:19:46.000000 autotraders-0.1.1/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-12 17:19:46.000000 autotraders-0.1.1/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:19:46.000000 autotraders-0.1.1/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-12 17:19:46.000000 autotraders-0.1.1/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-12 17:19:34.000000 autotraders-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 17:19:46.946435 autotraders-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:25:27.276875 autotraders-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-12 17:25:14.000000 autotraders-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-12 17:25:27.276875 autotraders-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-12 17:25:14.000000 autotraders-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:25:27.276875 autotraders-0.1.2/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-12 17:25:14.000000 autotraders-0.1.2/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-12 17:25:14.000000 autotraders-0.1.2/autotraders/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-12 17:25:14.000000 autotraders-0.1.2/autotraders/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-12 17:25:14.000000 autotraders-0.1.2/autotraders/ships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-12 17:25:14.000000 autotraders-0.1.2/autotraders/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-12 17:25:14.000000 autotraders-0.1.2/autotraders/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:25:27.276875 autotraders-0.1.2/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-12 17:25:27.000000 autotraders-0.1.2/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-12 17:25:27.000000 autotraders-0.1.2/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:25:27.000000 autotraders-0.1.2/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-12 17:25:27.000000 autotraders-0.1.2/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-12 17:25:14.000000 autotraders-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 17:25:27.276875 autotraders-0.1.2/setup.cfg
```

### Comparing `autotraders-0.1.1/LICENSE` & `autotraders-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-0.1.1/PKG-INFO` & `autotraders-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 0.1.1
+Version: 0.1.2
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://github.com/arihant2math/autotraders
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -38,10 +38,10 @@
 
 ```python
 from autotraders.ships import Ship
 # create a session here
 ship = Ship("SYMBOL-Here", session) # This makes an API request
 ship.dock()
 ship.refuel()
-ship.orbit()
+ship.orbit() # All these functions make API calls (one each), but the line below doesn't
 print(ship.fuel.current + "/" + ship.fuel.total)
 ```
```

### Comparing `autotraders-0.1.1/README.md` & `autotraders-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -24,10 +24,10 @@
 
 ```python
 from autotraders.ships import Ship
 # create a session here
 ship = Ship("SYMBOL-Here", session) # This makes an API request
 ship.dock()
 ship.refuel()
-ship.orbit()
+ship.orbit() # All these functions make API calls (one each), but the line below doesn't
 print(ship.fuel.current + "/" + ship.fuel.total)
 ```
```

### Comparing `autotraders-0.1.1/autotraders/agent.py` & `autotraders-0.1.2/autotraders/agent.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from sdk.contract import Contract
-from sdk.ships import Ship, get_all_ships
-
-from autotraders.autotraders.contract import get_all_contracts
+from autotraders.ships import get_all_ships
+from contract import get_all_contracts
 
 
 class Agent:
-    def __init__(self, session):
+    def __init__(self, session, update=True):
         self.session = session
-        self.update()
+        if update:
+            self.update()
 
-    def update(self):
-        r = self.session.get("https://api.spacetraders.io/v2/my/agent")
-        j = r.json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
-        self.account_id = j["data"]["accountId"]
-        self.symbol = j["data"]["symbol"]
-        self.headquarters = j["data"]["headquarters"]
-        self.credits = j["data"]["credits"]
+    def update(self, data=None):
+        if data is None:
+            r = self.session.get("https://api.spacetraders.io/v2/my/agent")
+            j = r.json()
+            if "error" in j:
+                raise IOError(j["error"]["message"])
+            data = j["data"]
+        self.account_id = data["accountId"]
+        self.symbol = data["symbol"]
+        self.headquarters = data["headquarters"]
+        self.credits = data["credits"]
         self.ships = get_all_ships(self.session)
         self.contracts = get_all_contracts(self.session)
```

### Comparing `autotraders-0.1.1/autotraders/contract.py` & `autotraders-0.1.2/autotraders/contract.py`

 * *Files identical despite different names*

### Comparing `autotraders-0.1.1/autotraders/ships.py` & `autotraders-0.1.2/autotraders/ships.py`

 * *Files identical despite different names*

### Comparing `autotraders-0.1.1/autotraders/system.py` & `autotraders-0.1.2/autotraders/system.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sdk.waypoint import Waypoint
+from autotraders import Waypoint
 
 
 class System:
     def __init__(self, symbol, session, update=True):
         self.session = session
         self.symbol = symbol
         self.waypoints = []
```

### Comparing `autotraders-0.1.1/autotraders/waypoint.py` & `autotraders-0.1.2/autotraders/waypoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             self.faction = None
         self.traits = []
         if "traits" in data:
             for trait in data["traits"]:
                 self.traits.append(Trait(trait))
 
 
-def get_waypoints(system, session):
+def get_all_waypoints(system, session):
     r = session.get("https://api.spacetraders.io/v2/systems/" + system + "/waypoints")
     data = r.json()["data"]
     waypoints = []
     for w in data:
         waypoint = Waypoint(w["symbol"], session, False)
         waypoint.update(w)
         waypoints.append(waypoint)
```

### Comparing `autotraders-0.1.1/autotraders.egg-info/PKG-INFO` & `autotraders-0.1.2/autotraders.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 0.1.1
+Version: 0.1.2
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://github.com/arihant2math/autotraders
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -38,10 +38,10 @@
 
 ```python
 from autotraders.ships import Ship
 # create a session here
 ship = Ship("SYMBOL-Here", session) # This makes an API request
 ship.dock()
 ship.refuel()
-ship.orbit()
+ship.orbit() # All these functions make API calls (one each), but the line below doesn't
 print(ship.fuel.current + "/" + ship.fuel.total)
 ```
```

### Comparing `autotraders-0.1.1/pyproject.toml` & `autotraders-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "autotraders"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```


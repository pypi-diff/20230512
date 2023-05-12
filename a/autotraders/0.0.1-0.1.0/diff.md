# Comparing `tmp/autotraders-0.0.1.tar.gz` & `tmp/autotraders-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-0.0.1.tar", last modified: Fri May 12 07:21:27 2023, max compression
+gzip compressed data, was "autotraders-0.1.0.tar", last modified: Fri May 12 17:09:23 2023, max compression
```

## Comparing `autotraders-0.0.1.tar` & `autotraders-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 07:21:27.154316 autotraders-0.0.1/
--rw-rw-rw-   0        0        0     1065 2023-05-12 07:05:08.000000 autotraders-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      550 2023-05-12 07:21:27.154316 autotraders-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-05-12 07:20:50.000000 autotraders-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 07:21:27.146287 autotraders-0.0.1/autotraders/
--rw-rw-rw-   0        0        0      107 2023-05-12 07:20:11.000000 autotraders-0.0.1/autotraders/__init__.py
--rw-rw-rw-   0        0        0      919 2023-05-12 06:55:06.000000 autotraders-0.0.1/autotraders/agent.py
--rw-rw-rw-   0        0        0      887 2023-05-12 01:51:19.000000 autotraders-0.0.1/autotraders/contract.py
--rw-rw-rw-   0        0        0     5201 2023-05-12 06:55:06.000000 autotraders-0.0.1/autotraders/ships.py
--rw-rw-rw-   0        0        0     1116 2023-05-12 04:43:37.000000 autotraders-0.0.1/autotraders/system.py
--rw-rw-rw-   0        0        0     1473 2023-05-11 23:17:22.000000 autotraders-0.0.1/autotraders/waypoint.py
-drwxrwxrwx   0        0        0        0 2023-05-12 07:21:27.152287 autotraders-0.0.1/autotraders.egg-info/
--rw-rw-rw-   0        0        0      550 2023-05-12 07:21:27.000000 autotraders-0.0.1/autotraders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-05-12 07:21:27.000000 autotraders-0.0.1/autotraders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 07:21:27.000000 autotraders-0.0.1/autotraders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-12 07:21:27.000000 autotraders-0.0.1/autotraders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      620 2023-05-12 07:20:49.000000 autotraders-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 07:21:27.154316 autotraders-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-12 17:09:23.132120 autotraders-0.1.0/
+-rw-rw-rw-   0        0        0     1065 2023-05-12 07:05:08.000000 autotraders-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1286 2023-05-12 17:09:23.131121 autotraders-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      752 2023-05-12 17:08:26.000000 autotraders-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 17:09:23.110120 autotraders-0.1.0/autotraders/
+-rw-rw-rw-   0        0        0      107 2023-05-12 07:20:11.000000 autotraders-0.1.0/autotraders/__init__.py
+-rw-rw-rw-   0        0        0      746 2023-05-12 17:05:59.000000 autotraders-0.1.0/autotraders/agent.py
+-rw-rw-rw-   0        0        0     1813 2023-05-12 17:05:59.000000 autotraders-0.1.0/autotraders/contract.py
+-rw-rw-rw-   0        0        0     5202 2023-05-12 17:03:46.000000 autotraders-0.1.0/autotraders/ships.py
+-rw-rw-rw-   0        0        0     1116 2023-05-12 04:43:37.000000 autotraders-0.1.0/autotraders/system.py
+-rw-rw-rw-   0        0        0     1473 2023-05-11 23:17:22.000000 autotraders-0.1.0/autotraders/waypoint.py
+drwxrwxrwx   0        0        0        0 2023-05-12 17:09:23.129121 autotraders-0.1.0/autotraders.egg-info/
+-rw-rw-rw-   0        0        0     1286 2023-05-12 17:09:23.000000 autotraders-0.1.0/autotraders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-05-12 17:09:23.000000 autotraders-0.1.0/autotraders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 17:09:23.000000 autotraders-0.1.0/autotraders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-12 17:09:23.000000 autotraders-0.1.0/autotraders.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      618 2023-05-12 17:08:00.000000 autotraders-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-12 17:09:23.132120 autotraders-0.1.0/setup.cfg
```

### Comparing `autotraders-0.0.1/LICENSE` & `autotraders-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-0.0.1/autotraders/agent.py` & `autotraders-0.1.0/autotraders/agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from sdk.contract import Contract
 from sdk.ships import Ship, get_all_ships
 
+from autotraders.autotraders.contract import get_all_contracts
+
 
 class Agent:
     def __init__(self, session):
         self.session = session
         self.update()
 
     def update(self):
@@ -13,14 +15,8 @@
         if "error" in j:
             raise IOError(j["error"]["message"])
         self.account_id = j["data"]["accountId"]
         self.symbol = j["data"]["symbol"]
         self.headquarters = j["data"]["headquarters"]
         self.credits = j["data"]["credits"]
         self.ships = get_all_ships(self.session)
-        r = self.session.get("https://api.spacetraders.io/v2/my/contracts")
-        j = r.json()
-        self.contracts = []
-        for contract in j["data"]:
-            c = Contract(contract["id"], self.session, False)
-            c.update(contract)
-            self.contracts.append(c)
+        self.contracts = get_all_contracts(self.session)
```

### Comparing `autotraders-0.0.1/autotraders/contract.py` & `autotraders-0.1.0/autotraders/contract.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,7 +15,33 @@
         self.fulfilled = data["fulfilled"]
         self.deadline = data["terms"]["deadline"]
 
     def accept(self):
         j = self.session.post("https://api.spacetraders.io/v2/my/contracts/" + self.contract_id + "/accept").json()
         if "error" in j:
             raise IOError(j["error"]["message"])
+
+    def deliver(self, symbol, cargo_symbol, amount):
+        j = self.session.post("https://api.spacetraders.io/v2/my/contracts/" + self.contract_id + "/deliver", data={
+            "shipSymbol": symbol,
+            "tradeSymbol": cargo_symbol,
+            "units": amount
+        }).json()
+        if "error" in j:
+            raise IOError(j["error"]["message"])
+        self.update()
+
+    def fulfill(self):
+        j = self.session.post("https://api.spacetraders.io/v2/my/contracts/" + self.contract_id + "/fulfill").json()
+        if "error" in j:
+            raise IOError(j["error"]["message"])
+
+
+def get_all_contracts(session):
+    r = session.get("https://api.spacetraders.io/v2/my/contracts")
+    j = r.json()
+    contracts = []
+    for contract in j["data"]:
+        c = Contract(contract["id"], session, False)
+        c.update(contract)
+        contracts.append(c)
+    return contracts
```

### Comparing `autotraders-0.0.1/autotraders/ships.py` & `autotraders-0.1.0/autotraders/ships.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,15 +68,14 @@
     def move(self, waypoint):
         r = self.session.post("https://api.spacetraders.io/v2/my/ships/" + self.symbol + "/navigate", data={
             "waypointSymbol": waypoint
         })
         j = r.json()
         if "error" in j:
             raise IOError(j["error"]["message"])
-        print(j)
         self.update()
 
     def dock(self):
         r = self.session.post("https://api.spacetraders.io/v2/my/ships/" + self.symbol + "/dock")
         j = r.json()
         if "error" in j:
             raise IOError(j["error"]["message"])
@@ -122,24 +121,25 @@
             "symbol": cargo_symbol,
             "units": quantity
         }).json()
         if "error" in j:
             raise IOError(j["error"]["message"])
         self.update()
 
-    def deliver(self, contract_id, cargo_symbol, amount):
-        j = self.session.post("https://api.spacetraders.io/v2/my/contracts/" + contract_id + "/deliver", data={
-            "shipSymbol": self.symbol,
+    def transfer(self, destination: str, cargo_symbol: str, quantity: int):
+        j = self.session.post("https://api.spacetraders.io/v2/my/ships/" + self.symbol + "/transfer", data={
             "tradeSymbol": cargo_symbol,
-            "units": amount
+            "units": quantity,
+            "shipSymbol": destination
         }).json()
         if "error" in j:
             raise IOError(j["error"]["message"])
         self.update()
 
+
 def get_all_ships(session):
     r = session.get("https://api.spacetraders.io/v2/my/ships")
     j = r.json()
     if "error" in j:
         raise IOError(j["error"]["message"])
     ships = []
     for ship in j["data"]:
```

### Comparing `autotraders-0.0.1/autotraders/system.py` & `autotraders-0.1.0/autotraders/system.py`

 * *Files identical despite different names*

### Comparing `autotraders-0.0.1/autotraders/waypoint.py` & `autotraders-0.1.0/autotraders/waypoint.py`

 * *Files identical despite different names*

### Comparing `autotraders-0.0.1/pyproject.toml` & `autotraders-0.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "autotraders"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 
 [project.urls]
-"Homepage" = "https://github.com/arihant2math/spacetraders"
-"Bug Tracker" = "https://github.com/arihant2math/spacetraders/issues"
+"Homepage" = "https://github.com/arihant2math/autotraders"
+"Bug Tracker" = "https://github.com/arihant2math/autotraders/issues"
```


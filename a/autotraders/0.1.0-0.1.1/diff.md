# Comparing `tmp/autotraders-0.1.0.tar.gz` & `tmp/autotraders-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-0.1.0.tar", last modified: Fri May 12 17:09:23 2023, max compression
+gzip compressed data, was "autotraders-0.1.1.tar", last modified: Fri May 12 17:19:46 2023, max compression
```

## Comparing `autotraders-0.1.0.tar` & `autotraders-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 17:09:23.132120 autotraders-0.1.0/
--rw-rw-rw-   0        0        0     1065 2023-05-12 07:05:08.000000 autotraders-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1286 2023-05-12 17:09:23.131121 autotraders-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      752 2023-05-12 17:08:26.000000 autotraders-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 17:09:23.110120 autotraders-0.1.0/autotraders/
--rw-rw-rw-   0        0        0      107 2023-05-12 07:20:11.000000 autotraders-0.1.0/autotraders/__init__.py
--rw-rw-rw-   0        0        0      746 2023-05-12 17:05:59.000000 autotraders-0.1.0/autotraders/agent.py
--rw-rw-rw-   0        0        0     1813 2023-05-12 17:05:59.000000 autotraders-0.1.0/autotraders/contract.py
--rw-rw-rw-   0        0        0     5202 2023-05-12 17:03:46.000000 autotraders-0.1.0/autotraders/ships.py
--rw-rw-rw-   0        0        0     1116 2023-05-12 04:43:37.000000 autotraders-0.1.0/autotraders/system.py
--rw-rw-rw-   0        0        0     1473 2023-05-11 23:17:22.000000 autotraders-0.1.0/autotraders/waypoint.py
-drwxrwxrwx   0        0        0        0 2023-05-12 17:09:23.129121 autotraders-0.1.0/autotraders.egg-info/
--rw-rw-rw-   0        0        0     1286 2023-05-12 17:09:23.000000 autotraders-0.1.0/autotraders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-05-12 17:09:23.000000 autotraders-0.1.0/autotraders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 17:09:23.000000 autotraders-0.1.0/autotraders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-12 17:09:23.000000 autotraders-0.1.0/autotraders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      618 2023-05-12 17:08:00.000000 autotraders-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 17:09:23.132120 autotraders-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:19:46.946435 autotraders-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-12 17:19:34.000000 autotraders-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-12 17:19:46.946435 autotraders-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-12 17:19:34.000000 autotraders-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:19:46.946435 autotraders-0.1.1/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-12 17:19:34.000000 autotraders-0.1.1/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-12 17:19:34.000000 autotraders-0.1.1/autotraders/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-12 17:19:34.000000 autotraders-0.1.1/autotraders/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-12 17:19:34.000000 autotraders-0.1.1/autotraders/ships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-12 17:19:34.000000 autotraders-0.1.1/autotraders/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-12 17:19:34.000000 autotraders-0.1.1/autotraders/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:19:46.946435 autotraders-0.1.1/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-12 17:19:46.000000 autotraders-0.1.1/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-12 17:19:46.000000 autotraders-0.1.1/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:19:46.000000 autotraders-0.1.1/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-12 17:19:46.000000 autotraders-0.1.1/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-12 17:19:34.000000 autotraders-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 17:19:46.946435 autotraders-0.1.1/setup.cfg
```

### Comparing `autotraders-0.1.0/LICENSE` & `autotraders-0.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2023 ASHWIN NAREN
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Copyright 2023 ASHWIN NAREN
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `autotraders-0.1.0/PKG-INFO` & `autotraders-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-Metadata-Version: 2.1
-Name: autotraders
-Version: 0.1.0
-Summary: A powerful spacetraders API
-Author-email: Ashwin Naren <arihant2math@gmail.com>
-Project-URL: Homepage, https://github.com/arihant2math/autotraders
-Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Autotraders
-A spacetraders API focused on automation and ease of use
-## Usage
-First you need a client, which can be generated 
-```python
-import requests
-
-
-class BearerAuth(requests.auth.AuthBase):
-    def __init__(self, token):
-        self.token = token
-
-    def __call__(self, r):
-        r.headers["authorization"] = "Bearer " + self.token
-        return r
-
-token = TOKEN_HERE
-s = requests.Session()
-s.auth = BearerAuth(token)
-```
-And now you're all set to use they actual API.
-
-## Ships
-
-```python
-from autotraders.ships import Ship
-# create a session here
-ship = Ship("SYMBOL-Here", session) # This makes an API request
-ship.dock()
-ship.refuel()
-ship.orbit()
-print(ship.fuel.current + "/" + ship.fuel.total)
-```
+Metadata-Version: 2.1
+Name: autotraders
+Version: 0.1.1
+Summary: A powerful spacetraders API
+Author-email: Ashwin Naren <arihant2math@gmail.com>
+Project-URL: Homepage, https://github.com/arihant2math/autotraders
+Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Autotraders
+A spacetraders API focused on automation and ease of use
+## Usage
+First you need a client, which can be generated 
+```python
+import requests
+
+
+class BearerAuth(requests.auth.AuthBase):
+    def __init__(self, token):
+        self.token = token
+
+    def __call__(self, r):
+        r.headers["authorization"] = "Bearer " + self.token
+        return r
+
+token = TOKEN_HERE
+s = requests.Session()
+s.auth = BearerAuth(token)
+```
+And now you're all set to use they actual API.
+
+## Ships
+
+```python
+from autotraders.ships import Ship
+# create a session here
+ship = Ship("SYMBOL-Here", session) # This makes an API request
+ship.dock()
+ship.refuel()
+ship.orbit()
+print(ship.fuel.current + "/" + ship.fuel.total)
+```
```

### Comparing `autotraders-0.1.0/README.md` & `autotraders-0.1.1/README.md`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# Autotraders
-A spacetraders API focused on automation and ease of use
-## Usage
-First you need a client, which can be generated 
-```python
-import requests
-
-
-class BearerAuth(requests.auth.AuthBase):
-    def __init__(self, token):
-        self.token = token
-
-    def __call__(self, r):
-        r.headers["authorization"] = "Bearer " + self.token
-        return r
-
-token = TOKEN_HERE
-s = requests.Session()
-s.auth = BearerAuth(token)
-```
-And now you're all set to use they actual API.
-
-## Ships
-
-```python
-from autotraders.ships import Ship
-# create a session here
-ship = Ship("SYMBOL-Here", session) # This makes an API request
-ship.dock()
-ship.refuel()
-ship.orbit()
-print(ship.fuel.current + "/" + ship.fuel.total)
-```
+# Autotraders
+A spacetraders API focused on automation and ease of use
+## Usage
+First you need a client, which can be generated 
+```python
+import requests
+
+
+class BearerAuth(requests.auth.AuthBase):
+    def __init__(self, token):
+        self.token = token
+
+    def __call__(self, r):
+        r.headers["authorization"] = "Bearer " + self.token
+        return r
+
+token = TOKEN_HERE
+s = requests.Session()
+s.auth = BearerAuth(token)
+```
+And now you're all set to use they actual API.
+
+## Ships
+
+```python
+from autotraders.ships import Ship
+# create a session here
+ship = Ship("SYMBOL-Here", session) # This makes an API request
+ship.dock()
+ship.refuel()
+ship.orbit()
+print(ship.fuel.current + "/" + ship.fuel.total)
+```
```

### Comparing `autotraders-0.1.0/autotraders/agent.py` & `autotraders-0.1.1/autotraders/agent.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from sdk.contract import Contract
-from sdk.ships import Ship, get_all_ships
-
-from autotraders.autotraders.contract import get_all_contracts
-
-
-class Agent:
-    def __init__(self, session):
-        self.session = session
-        self.update()
-
-    def update(self):
-        r = self.session.get("https://api.spacetraders.io/v2/my/agent")
-        j = r.json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
-        self.account_id = j["data"]["accountId"]
-        self.symbol = j["data"]["symbol"]
-        self.headquarters = j["data"]["headquarters"]
-        self.credits = j["data"]["credits"]
-        self.ships = get_all_ships(self.session)
-        self.contracts = get_all_contracts(self.session)
+from sdk.contract import Contract
+from sdk.ships import Ship, get_all_ships
+
+from autotraders.autotraders.contract import get_all_contracts
+
+
+class Agent:
+    def __init__(self, session):
+        self.session = session
+        self.update()
+
+    def update(self):
+        r = self.session.get("https://api.spacetraders.io/v2/my/agent")
+        j = r.json()
+        if "error" in j:
+            raise IOError(j["error"]["message"])
+        self.account_id = j["data"]["accountId"]
+        self.symbol = j["data"]["symbol"]
+        self.headquarters = j["data"]["headquarters"]
+        self.credits = j["data"]["credits"]
+        self.ships = get_all_ships(self.session)
+        self.contracts = get_all_contracts(self.session)
```

### Comparing `autotraders-0.1.0/autotraders/contract.py` & `autotraders-0.1.1/autotraders/contract.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,58 @@
-class Contract:
-    def __init__(self, contract_id, session, update=True):
-        self.contract_id = contract_id
-        self.session = session
-        if update:
-            self.update()
-
-    def update(self, data=None):
-        if data is None:
-            r = self.session.get("https://api.spacetraders.io/v2/my/contracts/" + self.contract_id)
-            data = r.json()["data"]
-        self.on_accepted = data["terms"]["payment"]["onAccepted"]
-        self.on_fulfilled = data["terms"]["payment"]["onFulfilled"]
-        self.accepted = data["accepted"]
-        self.fulfilled = data["fulfilled"]
-        self.deadline = data["terms"]["deadline"]
-
-    def accept(self):
-        j = self.session.post("https://api.spacetraders.io/v2/my/contracts/" + self.contract_id + "/accept").json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
-
-    def deliver(self, symbol, cargo_symbol, amount):
-        j = self.session.post("https://api.spacetraders.io/v2/my/contracts/" + self.contract_id + "/deliver", data={
-            "shipSymbol": symbol,
-            "tradeSymbol": cargo_symbol,
-            "units": amount
-        }).json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
-        self.update()
-
-    def fulfill(self):
-        j = self.session.post("https://api.spacetraders.io/v2/my/contracts/" + self.contract_id + "/fulfill").json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
-
-
-def get_all_contracts(session):
-    r = session.get("https://api.spacetraders.io/v2/my/contracts")
-    j = r.json()
-    contracts = []
-    for contract in j["data"]:
-        c = Contract(contract["id"], session, False)
-        c.update(contract)
-        contracts.append(c)
-    return contracts
+class Contract:
+    def __init__(self, contract_id, session, update=True):
+        self.contract_id = contract_id
+        self.session = session
+        if update:
+            self.update()
+
+    def update(self, data=None):
+        if data is None:
+            r = self.session.get(
+                "https://api.spacetraders.io/v2/my/contracts/" + self.contract_id
+            )
+            data = r.json()["data"]
+        self.on_accepted = data["terms"]["payment"]["onAccepted"]
+        self.on_fulfilled = data["terms"]["payment"]["onFulfilled"]
+        self.accepted = data["accepted"]
+        self.fulfilled = data["fulfilled"]
+        self.deadline = data["terms"]["deadline"]
+
+    def accept(self):
+        j = self.session.post(
+            "https://api.spacetraders.io/v2/my/contracts/"
+            + self.contract_id
+            + "/accept"
+        ).json()
+        if "error" in j:
+            raise IOError(j["error"]["message"])
+
+    def deliver(self, symbol, cargo_symbol, amount):
+        j = self.session.post(
+            "https://api.spacetraders.io/v2/my/contracts/"
+            + self.contract_id
+            + "/deliver",
+            data={"shipSymbol": symbol, "tradeSymbol": cargo_symbol, "units": amount},
+        ).json()
+        if "error" in j:
+            raise IOError(j["error"]["message"])
+        self.update()
+
+    def fulfill(self):
+        j = self.session.post(
+            "https://api.spacetraders.io/v2/my/contracts/"
+            + self.contract_id
+            + "/fulfill"
+        ).json()
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

### Comparing `autotraders-0.1.0/autotraders/waypoint.py` & `autotraders-0.1.1/autotraders/waypoint.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,50 @@
-class Trait:
-    def __init__(self, data):
-        self.symbol = data["symbol"]
-        self.name = data["name"]
-        self.description = data["description"]
-
-
-    def __str__(self):
-        return self.name
-
-class Waypoint:
-    def __init__(self, symbol, session, update=True):
-        self.session = session
-        self.symbol = symbol
-        if update:
-            self.update()
-
-    def update(self, data=None):
-        if data is None:
-            split = self.symbol.split("-")
-            system_symbol = split[0] + "-" + split[1]
-            waypoint_symbol = self.symbol
-            data = self.session.get("https://api.spacetraders.io/v2/systems/" + system_symbol + "/waypoints/" + waypoint_symbol).json()["data"]
-        self.waypoint_type = data["type"]
-        self.x = data["x"]
-        self.y = data["y"]
-        if "faction" in data:
-            self.faction = data["faction"]["symbol"]
-        else:
-            self.faction = None
-        self.traits = []
-        if "traits" in data:
-            for trait in data["traits"]:
-                self.traits.append(Trait(trait))
-
-
-def get_waypoints(system, session):
-    r = session.get("https://api.spacetraders.io/v2/systems/" + system + "/waypoints")
-    data = r.json()["data"]
-    waypoints = []
-    for w in data:
-        waypoint = Waypoint(w["symbol"], session, False)
-        waypoint.update(w)
-        waypoints.append(waypoint)
-    return waypoints
+class Trait:
+    def __init__(self, data):
+        self.symbol = data["symbol"]
+        self.name = data["name"]
+        self.description = data["description"]
+
+    def __str__(self):
+        return self.name
+
+
+class Waypoint:
+    def __init__(self, symbol, session, update=True):
+        self.session = session
+        self.symbol = symbol
+        if update:
+            self.update()
+
+    def update(self, data=None):
+        if data is None:
+            split = self.symbol.split("-")
+            system_symbol = split[0] + "-" + split[1]
+            waypoint_symbol = self.symbol
+            data = self.session.get(
+                "https://api.spacetraders.io/v2/systems/"
+                + system_symbol
+                + "/waypoints/"
+                + waypoint_symbol
+            ).json()["data"]
+        self.waypoint_type = data["type"]
+        self.x = data["x"]
+        self.y = data["y"]
+        if "faction" in data:
+            self.faction = data["faction"]["symbol"]
+        else:
+            self.faction = None
+        self.traits = []
+        if "traits" in data:
+            for trait in data["traits"]:
+                self.traits.append(Trait(trait))
+
+
+def get_waypoints(system, session):
+    r = session.get("https://api.spacetraders.io/v2/systems/" + system + "/waypoints")
+    data = r.json()["data"]
+    waypoints = []
+    for w in data:
+        waypoint = Waypoint(w["symbol"], session, False)
+        waypoint.update(w)
+        waypoints.append(waypoint)
+    return waypoints
```

### Comparing `autotraders-0.1.0/autotraders.egg-info/PKG-INFO` & `autotraders-0.1.1/autotraders.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-Metadata-Version: 2.1
-Name: autotraders
-Version: 0.1.0
-Summary: A powerful spacetraders API
-Author-email: Ashwin Naren <arihant2math@gmail.com>
-Project-URL: Homepage, https://github.com/arihant2math/autotraders
-Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Autotraders
-A spacetraders API focused on automation and ease of use
-## Usage
-First you need a client, which can be generated 
-```python
-import requests
-
-
-class BearerAuth(requests.auth.AuthBase):
-    def __init__(self, token):
-        self.token = token
-
-    def __call__(self, r):
-        r.headers["authorization"] = "Bearer " + self.token
-        return r
-
-token = TOKEN_HERE
-s = requests.Session()
-s.auth = BearerAuth(token)
-```
-And now you're all set to use they actual API.
-
-## Ships
-
-```python
-from autotraders.ships import Ship
-# create a session here
-ship = Ship("SYMBOL-Here", session) # This makes an API request
-ship.dock()
-ship.refuel()
-ship.orbit()
-print(ship.fuel.current + "/" + ship.fuel.total)
-```
+Metadata-Version: 2.1
+Name: autotraders
+Version: 0.1.1
+Summary: A powerful spacetraders API
+Author-email: Ashwin Naren <arihant2math@gmail.com>
+Project-URL: Homepage, https://github.com/arihant2math/autotraders
+Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Autotraders
+A spacetraders API focused on automation and ease of use
+## Usage
+First you need a client, which can be generated 
+```python
+import requests
+
+
+class BearerAuth(requests.auth.AuthBase):
+    def __init__(self, token):
+        self.token = token
+
+    def __call__(self, r):
+        r.headers["authorization"] = "Bearer " + self.token
+        return r
+
+token = TOKEN_HERE
+s = requests.Session()
+s.auth = BearerAuth(token)
+```
+And now you're all set to use they actual API.
+
+## Ships
+
+```python
+from autotraders.ships import Ship
+# create a session here
+ship = Ship("SYMBOL-Here", session) # This makes an API request
+ship.dock()
+ship.refuel()
+ship.orbit()
+print(ship.fuel.current + "/" + ship.fuel.total)
+```
```


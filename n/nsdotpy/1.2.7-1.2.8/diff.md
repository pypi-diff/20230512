# Comparing `tmp/nsdotpy-1.2.7.tar.gz` & `tmp/nsdotpy-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsdotpy-1.2.7.tar", max compression
+gzip compressed data, was "nsdotpy-1.2.8.tar", max compression
```

## Comparing `nsdotpy-1.2.7.tar` & `nsdotpy-1.2.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34354 2023-05-09 23:52:00.967120 nsdotpy-1.2.7/LICENSE.md
--rw-r--r--   0        0        0     2436 2023-05-09 23:52:00.967120 nsdotpy-1.2.7/README.md
--rw-r--r--   0        0        0      790 2023-05-09 23:52:00.979121 nsdotpy-1.2.7/nsdotpy/__init__.py
--rw-r--r--   0        0        0    40841 2023-05-09 23:52:00.979121 nsdotpy-1.2.7/nsdotpy/session.py
--rw-r--r--   0        0        0     4963 2023-05-09 23:52:00.979121 nsdotpy-1.2.7/nsdotpy/valid.py
--rw-r--r--   0        0        0      703 2023-05-09 23:52:00.979121 nsdotpy-1.2.7/pyproject.toml
--rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 nsdotpy-1.2.7/PKG-INFO
+-rw-r--r--   0        0        0    34354 2023-05-12 03:19:53.212307 nsdotpy-1.2.8/LICENSE.md
+-rw-r--r--   0        0        0     2436 2023-05-12 03:19:53.212307 nsdotpy-1.2.8/README.md
+-rw-r--r--   0        0        0      790 2023-05-12 03:19:53.224307 nsdotpy-1.2.8/nsdotpy/__init__.py
+-rw-r--r--   0        0        0    41448 2023-05-12 03:19:53.224307 nsdotpy-1.2.8/nsdotpy/session.py
+-rw-r--r--   0        0        0     4963 2023-05-12 03:19:53.224307 nsdotpy-1.2.8/nsdotpy/valid.py
+-rw-r--r--   0        0        0      703 2023-05-12 03:19:53.224307 nsdotpy-1.2.8/pyproject.toml
+-rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 nsdotpy-1.2.8/PKG-INFO
```

### Comparing `nsdotpy-1.2.7/LICENSE.md` & `nsdotpy-1.2.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.2.7/README.md` & `nsdotpy-1.2.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 `pip install nsdotpy`
 
 ## Simple Example
 
 ```python
 
 from nsdotpy.session import NSSession
-session = NSSession("NSDotPy Example," "1.0.0", "Script Author's nation", "Script User's nation")
+session = NSSession("NSDotPy Example", "1.0.0", "Script Author's nation", "Script User's nation")
 
 if session.login("User Nation", "Password"):  # logs in and checks if login was successful
     session.move_to_region("Lily")  # only moves if you successfully logged in
 ```
 
 ## TODO:
```

### Comparing `nsdotpy-1.2.7/nsdotpy/__init__.py` & `nsdotpy-1.2.8/nsdotpy/__init__.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.2.7/nsdotpy/session.py` & `nsdotpy-1.2.8/nsdotpy/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             script_version (str): Version number of your script
             script_author (str): Author of your script
             script_user (str): Nation name of the user running your script
             keybind (str, optional): Keybind to count as a user click. Defaults to "space".
             link_to_src (str, optional): Link to the source code of your script.
             logger (logging.Logger | None, optional): Logger to use. Will create its own with name "NSDotPy" if none is specified. Defaults to None.
         """
-        self.VERSION = "1.2.7"
+        self.VERSION = "1.2.8"
         # Initialize logger
         if not logger:
             self._init_logger()
         else:
             self.logger = logger
         # Attach the tendo singleton to the session object so it can
         # only be run once at a time, avoiding simultaneity issues
@@ -1067,10 +1067,29 @@
         url = "https://www.nationstates.net/template-overall=none/page=deck"
 
         data = {"edit": "1", "collection_name": name, "delete_collection": "1"}
         response = self.request(url, data)
 
         return "Created collection!" in response.text
 
+    def can_nation_be_founded(self, name: str):
+        """Checks if a nation can be founded
+
+        Args:
+            name (str): The name of the nation you want to check
+
+        Returns:
+            bool: Whether the nation can be founded or not
+        """
+        self.logger.info(f"Checking {name} in boneyard")
+        url = "https://www.nationstates.net/template-overall=none/page=boneyard"
+
+        data = {"nation": name, "submit": "1"}
+        response = self.request(url, data)
+
+        return (
+            "Available! This name may be used to found a new nation." in response.text
+        )
+
 
 if __name__ == "__main__":
     print("this is a module/library, not a script")
```

### Comparing `nsdotpy-1.2.7/nsdotpy/valid.py` & `nsdotpy-1.2.8/nsdotpy/valid.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.2.7/pyproject.toml` & `nsdotpy-1.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsdotpy"
-version = "1.2.7"
+version = "1.2.8"
 description = "A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use."
 authors = ["audrey <audreyreal@proton.me>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/sw33ze/NSDotPy"
 
 [tool.poetry.dependencies]
```

### Comparing `nsdotpy-1.2.7/PKG-INFO` & `nsdotpy-1.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsdotpy
-Version: 1.2.7
+Version: 1.2.8
 Summary: A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use.
 Home-page: https://github.com/sw33ze/NSDotPy
 License: AGPL-3.0-or-later
 Author: audrey
 Author-email: audreyreal@proton.me
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -27,15 +27,15 @@
 `pip install nsdotpy`
 
 ## Simple Example
 
 ```python
 
 from nsdotpy.session import NSSession
-session = NSSession("NSDotPy Example," "1.0.0", "Script Author's nation", "Script User's nation")
+session = NSSession("NSDotPy Example", "1.0.0", "Script Author's nation", "Script User's nation")
 
 if session.login("User Nation", "Password"):  # logs in and checks if login was successful
     session.move_to_region("Lily")  # only moves if you successfully logged in
 ```
 
 ## TODO:
```


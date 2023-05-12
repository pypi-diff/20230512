# Comparing `tmp/audiconnectpy-1.3.4.tar.gz` & `tmp/audiconnectpy-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-1.3.4.tar", last modified: Sat May  6 10:03:31 2023, max compression
+gzip compressed data, was "audiconnectpy-1.3.5.tar", last modified: Fri May 12 17:47:01 2023, max compression
```

## Comparing `audiconnectpy-1.3.4.tar` & `audiconnectpy-1.3.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:03:31.802897 audiconnectpy-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-06 10:03:18.000000 audiconnectpy-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-06 10:03:18.000000 audiconnectpy-1.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-06 10:03:31.802897 audiconnectpy-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-06 10:03:18.000000 audiconnectpy-1.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:03:31.802897 audiconnectpy-1.3.4/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-06 10:03:18.000000 audiconnectpy-1.3.4/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-06 10:03:18.000000 audiconnectpy-1.3.4/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22631 2023-05-06 10:03:18.000000 audiconnectpy-1.3.4/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-06 10:03:18.000000 audiconnectpy-1.3.4/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-06 10:03:18.000000 audiconnectpy-1.3.4/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27807 2023-05-06 10:03:18.000000 audiconnectpy-1.3.4/audiconnectpy/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30454 2023-05-06 10:03:18.000000 audiconnectpy-1.3.4/audiconnectpy/services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:03:31.802897 audiconnectpy-1.3.4/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-06 10:03:31.000000 audiconnectpy-1.3.4/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-06 10:03:31.000000 audiconnectpy-1.3.4/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 10:03:31.000000 audiconnectpy-1.3.4/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 10:03:31.000000 audiconnectpy-1.3.4/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-06 10:03:31.000000 audiconnectpy-1.3.4/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-06 10:03:18.000000 audiconnectpy-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 10:03:31.802897 audiconnectpy-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-06 10:03:29.000000 audiconnectpy-1.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:03:31.802897 audiconnectpy-1.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-06 10:03:18.000000 audiconnectpy-1.3.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:47:01.536051 audiconnectpy-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-12 17:46:48.000000 audiconnectpy-1.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-12 17:46:48.000000 audiconnectpy-1.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-12 17:47:01.536051 audiconnectpy-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-12 17:46:48.000000 audiconnectpy-1.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:47:01.536051 audiconnectpy-1.3.5/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-12 17:46:48.000000 audiconnectpy-1.3.5/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-12 17:46:48.000000 audiconnectpy-1.3.5/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22631 2023-05-12 17:46:48.000000 audiconnectpy-1.3.5/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-12 17:46:48.000000 audiconnectpy-1.3.5/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-12 17:46:48.000000 audiconnectpy-1.3.5/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27959 2023-05-12 17:46:48.000000 audiconnectpy-1.3.5/audiconnectpy/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30454 2023-05-12 17:46:48.000000 audiconnectpy-1.3.5/audiconnectpy/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:47:01.536051 audiconnectpy-1.3.5/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-12 17:47:01.000000 audiconnectpy-1.3.5/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-12 17:47:01.000000 audiconnectpy-1.3.5/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:47:01.000000 audiconnectpy-1.3.5/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 17:47:01.000000 audiconnectpy-1.3.5/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-12 17:47:01.000000 audiconnectpy-1.3.5/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-12 17:46:48.000000 audiconnectpy-1.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 17:47:01.536051 audiconnectpy-1.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-12 17:46:59.000000 audiconnectpy-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:47:01.536051 audiconnectpy-1.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-12 17:46:48.000000 audiconnectpy-1.3.5/tests/__init__.py
```

### Comparing `audiconnectpy-1.3.4/LICENSE` & `audiconnectpy-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.4/PKG-INFO` & `audiconnectpy-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.3.4
+Version: 1.3.5
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.3.4/README.md` & `audiconnectpy-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.4/audiconnectpy/api.py` & `audiconnectpy-1.3.5/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.4/audiconnectpy/auth.py` & `audiconnectpy-1.3.5/audiconnectpy/auth.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.4/audiconnectpy/helpers.py` & `audiconnectpy-1.3.5/audiconnectpy/helpers.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.4/audiconnectpy/models.py` & `audiconnectpy-1.3.5/audiconnectpy/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -428,26 +428,30 @@
         """Supported status."""
         return self.data.getr("findCarResponse.Position") is not None
 
     @property
     def attributes(self) -> dict[str, Any]:
         """Attributes properties."""
         attrs = {}
-        if coordinate := self.data.getr("findCarResponse.Position.carCoordinate"):
+        if isinstance(self.data, ExtendedDict) and (
+            coordinate := self.data.getr("findCarResponse.Position.carCoordinate")
+        ):
             timestamp = self.data.getr("findCarResponse.Position.timestampCarSentUTC")
             attrs = {
                 "position": {
                     "latitude": coordinate["latitude"] / 1000000,
                     "longitude": coordinate["longitude"] / 1000000,
                     "timestamp": timestamp,
                     "parktime": self.data.getr(
                         "findCarResponse.parkingTimeUTC", timestamp
                     ),
                 }
             }
+        else:
+            _LOGGER.warning("Position format is incorrect %s", self.data)
         return attrs
 
 
 @dataclass
 class TripDataResponse:
     """Trip class."""
```

### Comparing `audiconnectpy-1.3.4/audiconnectpy/services.py` & `audiconnectpy-1.3.5/audiconnectpy/services.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.4/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-1.3.5/audiconnectpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.3.4
+Version: 1.3.5
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.3.4/pyproject.toml` & `audiconnectpy-1.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.4/setup.py` & `audiconnectpy-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="audiconnectpy",
-    version="1.3.4",
+    version="1.3.5",
     packages=find_packages(),
     author="cyr-ius",
     author_email="cyr-ius@ipocus.net",
     description="Provides asynchronous authentication and access to Audi Connect",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp>=3.8.1", "beautifulsoup4>=4.11.2"],
```


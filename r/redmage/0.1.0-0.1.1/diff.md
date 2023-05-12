# Comparing `tmp/redmage-0.1.0.tar.gz` & `tmp/redmage-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redmage-0.1.0.tar", max compression
+gzip compressed data, was "redmage-0.1.1.tar", max compression
```

## Comparing `redmage-0.1.0.tar` & `redmage-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.1.0/LICENSE
--rw-r--r--   0        0        0    14351 2023-05-12 14:17:31.917169 redmage-0.1.0/README.md
--rw-r--r--   0        0        0      660 2023-05-12 14:55:28.760619 redmage-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      333 2023-05-12 13:48:08.901451 redmage-0.1.0/redmage/__init__.py
--rw-r--r--   0        0        0     6689 2023-05-12 14:38:21.207931 redmage-0.1.0/redmage/components.py
--rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.1.0/redmage/convertors.py
--rw-r--r--   0        0        0     7186 2023-05-12 14:51:43.484701 redmage-0.1.0/redmage/core.py
--rw-r--r--   0        0        0     9605 2023-04-30 17:34:15.446362 redmage-0.1.0/redmage/elements.py
--rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.1.0/redmage/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.1.0/redmage/py.typed
--rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.1.0/redmage/targets.py
--rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.1.0/redmage/triggers.py
--rw-r--r--   0        0        0     1314 2023-05-01 00:53:46.268926 redmage-0.1.0/redmage/types.py
--rw-r--r--   0        0        0      558 2023-04-30 18:18:23.887821 redmage-0.1.0/redmage/utils.py
--rw-r--r--   0        0        0    15052 1970-01-01 00:00:00.000000 redmage-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-30 18:42:13.320074 redmage-0.1.1/LICENSE
+-rw-r--r--   0        0        0    14351 2023-05-12 14:17:31.917169 redmage-0.1.1/README.md
+-rw-r--r--   0        0        0      660 2023-05-12 15:01:02.142626 redmage-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      333 2023-05-12 13:48:08.901451 redmage-0.1.1/redmage/__init__.py
+-rw-r--r--   0        0        0     6689 2023-05-12 14:38:21.207931 redmage-0.1.1/redmage/components.py
+-rw-r--r--   0        0        0      611 2023-04-30 17:51:09.398688 redmage-0.1.1/redmage/convertors.py
+-rw-r--r--   0        0        0     7141 2023-05-12 15:00:48.077628 redmage-0.1.1/redmage/core.py
+-rw-r--r--   0        0        0     9605 2023-04-30 17:34:15.446362 redmage-0.1.1/redmage/elements.py
+-rw-r--r--   0        0        0       40 2023-04-30 16:16:17.636906 redmage-0.1.1/redmage/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:02:07.108573 redmage-0.1.1/redmage/py.typed
+-rw-r--r--   0        0        0     1582 2023-04-29 14:59:56.659250 redmage-0.1.1/redmage/targets.py
+-rw-r--r--   0        0        0     2187 2023-04-30 16:49:07.664173 redmage-0.1.1/redmage/triggers.py
+-rw-r--r--   0        0        0     1314 2023-05-01 00:53:46.268926 redmage-0.1.1/redmage/types.py
+-rw-r--r--   0        0        0      558 2023-04-30 18:18:23.887821 redmage-0.1.1/redmage/utils.py
+-rw-r--r--   0        0        0    15052 1970-01-01 00:00:00.000000 redmage-0.1.1/PKG-INFO
```

### Comparing `redmage-0.1.0/LICENSE` & `redmage-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `redmage-0.1.0/README.md` & `redmage-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `redmage-0.1.0/pyproject.toml` & `redmage-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redmage"
-version = "0.1.0"
+version = "0.1.1"
 description = "A component based library for building htmx powered applications."
 authors = ["Scott Russell <me@scottrussell.net>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `redmage-0.1.0/redmage/components.py` & `redmage-0.1.1/redmage/components.py`

 * *Files identical despite different names*

### Comparing `redmage-0.1.0/redmage/convertors.py` & `redmage-0.1.1/redmage/convertors.py`

 * *Files identical despite different names*

### Comparing `redmage-0.1.0/redmage/core.py` & `redmage-0.1.1/redmage/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,14 @@
         return target_method
 
     def _register_routes(
         self, cls: ComponentClass, routes: Tuple[str]
     ) -> ComponentClass:
         for route in routes:
             logger.debug(route)
-            print(route)
             self.routes.append(
                 Route(
                     route,
                     self._get_explicit_route_function(cls),
                     methods=[
                         HTTPMethod.GET,
                     ],
@@ -184,15 +183,14 @@
     def _register_target(
         self, cls: ComponentClass, method: Tuple[str, FunctionType]
     ) -> None:
         method_name, method_fn = method
         path = cls.get_base_path()
         path += cls.get_target_path(method_name)
         logger.debug(path)
-        print(path)
         route_function = self._get_route_function(cls, method_name, method_fn)
 
         self.routes.append(
             Route(
                 path,
                 route_function,
                 name=method_name,
```

### Comparing `redmage-0.1.0/redmage/elements.py` & `redmage-0.1.1/redmage/elements.py`

 * *Files identical despite different names*

### Comparing `redmage-0.1.0/redmage/targets.py` & `redmage-0.1.1/redmage/targets.py`

 * *Files identical despite different names*

### Comparing `redmage-0.1.0/redmage/triggers.py` & `redmage-0.1.1/redmage/triggers.py`

 * *Files identical despite different names*

### Comparing `redmage-0.1.0/redmage/types.py` & `redmage-0.1.1/redmage/types.py`

 * *Files identical despite different names*

### Comparing `redmage-0.1.0/redmage/utils.py` & `redmage-0.1.1/redmage/utils.py`

 * *Files identical despite different names*

### Comparing `redmage-0.1.0/PKG-INFO` & `redmage-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redmage
-Version: 0.1.0
+Version: 0.1.1
 Summary: A component based library for building htmx powered applications.
 License: MIT
 Author: Scott Russell
 Author-email: me@scottrussell.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


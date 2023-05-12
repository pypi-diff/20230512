# Comparing `tmp/confik-1.0.1.tar.gz` & `tmp/confik-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confik-1.0.1.tar", last modified: Fri May 12 06:46:33 2023, max compression
+gzip compressed data, was "confik-1.0.2.tar", last modified: Fri May 12 06:58:34 2023, max compression
```

## Comparing `confik-1.0.1.tar` & `confik-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-12 06:46:33.925893 confik-1.0.1/
--rw-r--r--   0 leondaz    (501) staff       (20)      197 2023-05-12 06:46:33.925759 confik-1.0.1/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)      133 2023-05-12 06:07:05.000000 confik-1.0.1/README.md
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-12 06:46:33.924748 confik-1.0.1/confik/
--rw-r--r--   0 leondaz    (501) staff       (20)      828 2023-05-12 06:34:12.000000 confik-1.0.1/confik/__init__.py
--rw-r--r--   0 leondaz    (501) staff       (20)       78 2023-05-12 03:19:53.000000 confik-1.0.1/confik/exceptions.py
--rw-r--r--   0 leondaz    (501) staff       (20)     2213 2023-05-12 06:45:46.000000 confik-1.0.1/confik/parsers.py
--rw-r--r--   0 leondaz    (501) staff       (20)      904 2023-05-12 06:45:46.000000 confik-1.0.1/confik/proxies.py
--rw-r--r--   0 leondaz    (501) staff       (20)      286 2023-05-12 05:54:36.000000 confik-1.0.1/confik/utils.py
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-12 06:46:33.925210 confik-1.0.1/confik.egg-info/
--rw-r--r--   0 leondaz    (501) staff       (20)      197 2023-05-12 06:46:33.000000 confik-1.0.1/confik.egg-info/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)      319 2023-05-12 06:46:33.000000 confik-1.0.1/confik.egg-info/SOURCES.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-12 06:46:33.000000 confik-1.0.1/confik.egg-info/dependency_links.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        7 2023-05-12 06:46:33.000000 confik-1.0.1/confik.egg-info/top_level.txt
--rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-12 06:46:33.925934 confik-1.0.1/setup.cfg
--rw-r--r--   0 leondaz    (501) staff       (20)      277 2023-05-12 06:46:25.000000 confik-1.0.1/setup.py
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-12 06:46:33.925579 confik-1.0.1/tests/
--rw-r--r--   0 leondaz    (501) staff       (20)      308 2023-05-12 06:07:05.000000 confik-1.0.1/tests/test_confik_parser.py
--rw-r--r--   0 leondaz    (501) staff       (20)     1482 2023-05-12 06:07:05.000000 confik-1.0.1/tests/test_read_environment_variables.py
--rw-r--r--   0 leondaz    (501) staff       (20)      164 2023-05-12 05:54:17.000000 confik-1.0.1/tests/test_utils.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-12 06:58:34.685003 confik-1.0.2/
+-rw-r--r--   0 leondaz    (501) staff       (20)      197 2023-05-12 06:58:34.684871 confik-1.0.2/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)      133 2023-05-12 06:07:05.000000 confik-1.0.2/README.md
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-12 06:58:34.683304 confik-1.0.2/confik/
+-rw-r--r--   0 leondaz    (501) staff       (20)      828 2023-05-12 06:34:12.000000 confik-1.0.2/confik/__init__.py
+-rw-r--r--   0 leondaz    (501) staff       (20)       78 2023-05-12 03:19:53.000000 confik-1.0.2/confik/exceptions.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     2213 2023-05-12 06:45:46.000000 confik-1.0.2/confik/parsers.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     1265 2023-05-12 06:56:06.000000 confik-1.0.2/confik/proxies.py
+-rw-r--r--   0 leondaz    (501) staff       (20)      286 2023-05-12 05:54:36.000000 confik-1.0.2/confik/utils.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-12 06:58:34.683979 confik-1.0.2/confik.egg-info/
+-rw-r--r--   0 leondaz    (501) staff       (20)      197 2023-05-12 06:58:34.000000 confik-1.0.2/confik.egg-info/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)      319 2023-05-12 06:58:34.000000 confik-1.0.2/confik.egg-info/SOURCES.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-12 06:58:34.000000 confik-1.0.2/confik.egg-info/dependency_links.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        7 2023-05-12 06:58:34.000000 confik-1.0.2/confik.egg-info/top_level.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-12 06:58:34.685043 confik-1.0.2/setup.cfg
+-rw-r--r--   0 leondaz    (501) staff       (20)      277 2023-05-12 06:58:33.000000 confik-1.0.2/setup.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-12 06:58:34.684583 confik-1.0.2/tests/
+-rw-r--r--   0 leondaz    (501) staff       (20)      308 2023-05-12 06:07:05.000000 confik-1.0.2/tests/test_confik_parser.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     1482 2023-05-12 06:07:05.000000 confik-1.0.2/tests/test_read_environment_variables.py
+-rw-r--r--   0 leondaz    (501) staff       (20)      164 2023-05-12 05:54:17.000000 confik-1.0.2/tests/test_utils.py
```

### Comparing `confik-1.0.1/confik/__init__.py` & `confik-1.0.2/confik/__init__.py`

 * *Files identical despite different names*

### Comparing `confik-1.0.1/confik/parsers.py` & `confik-1.0.2/confik/parsers.py`

 * *Files identical despite different names*

### Comparing `confik-1.0.1/confik/proxies.py` & `confik-1.0.2/confik/proxies.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,50 @@
 import contextlib
 import os
 from pathlib import Path
 
 
-class EnvMappingProxy:
-    def __init__(self, path=Path("."), *args, **kwargs):
-        assert isinstance(path, (str, Path)), "unsupported path type {t}".format(
-            t=type(path)
-        )
+class MapConfigToMappingProxy:
+    def get_mapping(self, path):
+        """
+        Should return a mapping from the path given
+        :param path: str
+        :return: Mapping
+        """
+        raise NotImplementedError
 
-        environ = os.environ.copy()
 
-        if isinstance(path, str):
-            path = Path(path)
-
-        if path.suffix != ".env":
-            path = path / ".env"
+class EnvMappingProxy(MapConfigToMappingProxy):
+    def get_mapping(self, path):
+        mapping = {}
 
         with contextlib.suppress(FileNotFoundError):
             with open(path, "r") as f:
                 for line in f.readlines():
                     entry = line.strip().split("=")
 
                     if len(entry) == 1:
                         entry.append("")
 
                     name, value = entry
-                    environ[name] = value.replace('"', "")
+                    mapping[name] = value.replace('"', "")
+
+        return mapping
+
+    def __init__(self, path=Path("."), *args, **kwargs):
+        assert isinstance(path, (str, Path)), "unsupported path type {t}".format(
+            t=type(path)
+        )
+
+        if isinstance(path, str):
+            path = Path(path)
+
+        if path.suffix != ".env":
+            path = path / ".env"
 
-        self.environ = environ
+        self.environ = {
+            **os.environ,
+            **self.get_mapping(path),
+        }
 
     def get(self, key, default):
         return self.environ.get(key, default)
```

### Comparing `confik-1.0.1/tests/test_read_environment_variables.py` & `confik-1.0.2/tests/test_read_environment_variables.py`

 * *Files identical despite different names*


# Comparing `tmp/confik-1.0.0.tar.gz` & `tmp/confik-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confik-1.0.0.tar", last modified: Fri May 12 06:34:46 2023, max compression
+gzip compressed data, was "confik-1.0.1.tar", last modified: Fri May 12 06:46:33 2023, max compression
```

## Comparing `confik-1.0.0.tar` & `confik-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-12 06:34:46.826832 confik-1.0.0/
--rw-r--r--   0 leondaz    (501) staff       (20)      197 2023-05-12 06:34:46.826692 confik-1.0.0/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)      133 2023-05-12 06:07:05.000000 confik-1.0.0/README.md
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-12 06:34:46.825619 confik-1.0.0/confik/
--rw-r--r--   0 leondaz    (501) staff       (20)      828 2023-05-12 06:34:12.000000 confik-1.0.0/confik/__init__.py
--rw-r--r--   0 leondaz    (501) staff       (20)       78 2023-05-12 03:19:53.000000 confik-1.0.0/confik/exceptions.py
--rw-r--r--   0 leondaz    (501) staff       (20)     2221 2023-05-12 06:14:31.000000 confik-1.0.0/confik/parsers.py
--rw-r--r--   0 leondaz    (501) staff       (20)      809 2023-05-12 05:54:36.000000 confik-1.0.0/confik/proxies.py
--rw-r--r--   0 leondaz    (501) staff       (20)      286 2023-05-12 05:54:36.000000 confik-1.0.0/confik/utils.py
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-12 06:34:46.826086 confik-1.0.0/confik.egg-info/
--rw-r--r--   0 leondaz    (501) staff       (20)      197 2023-05-12 06:34:46.000000 confik-1.0.0/confik.egg-info/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)      319 2023-05-12 06:34:46.000000 confik-1.0.0/confik.egg-info/SOURCES.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-12 06:34:46.000000 confik-1.0.0/confik.egg-info/dependency_links.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        7 2023-05-12 06:34:46.000000 confik-1.0.0/confik.egg-info/top_level.txt
--rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-12 06:34:46.826872 confik-1.0.0/setup.cfg
--rw-r--r--   0 leondaz    (501) staff       (20)      277 2023-05-12 05:54:36.000000 confik-1.0.0/setup.py
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-12 06:34:46.826500 confik-1.0.0/tests/
--rw-r--r--   0 leondaz    (501) staff       (20)      308 2023-05-12 06:07:05.000000 confik-1.0.0/tests/test_confik_parser.py
--rw-r--r--   0 leondaz    (501) staff       (20)     1482 2023-05-12 06:07:05.000000 confik-1.0.0/tests/test_read_environment_variables.py
--rw-r--r--   0 leondaz    (501) staff       (20)      164 2023-05-12 05:54:17.000000 confik-1.0.0/tests/test_utils.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-12 06:46:33.925893 confik-1.0.1/
+-rw-r--r--   0 leondaz    (501) staff       (20)      197 2023-05-12 06:46:33.925759 confik-1.0.1/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)      133 2023-05-12 06:07:05.000000 confik-1.0.1/README.md
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-12 06:46:33.924748 confik-1.0.1/confik/
+-rw-r--r--   0 leondaz    (501) staff       (20)      828 2023-05-12 06:34:12.000000 confik-1.0.1/confik/__init__.py
+-rw-r--r--   0 leondaz    (501) staff       (20)       78 2023-05-12 03:19:53.000000 confik-1.0.1/confik/exceptions.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     2213 2023-05-12 06:45:46.000000 confik-1.0.1/confik/parsers.py
+-rw-r--r--   0 leondaz    (501) staff       (20)      904 2023-05-12 06:45:46.000000 confik-1.0.1/confik/proxies.py
+-rw-r--r--   0 leondaz    (501) staff       (20)      286 2023-05-12 05:54:36.000000 confik-1.0.1/confik/utils.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-12 06:46:33.925210 confik-1.0.1/confik.egg-info/
+-rw-r--r--   0 leondaz    (501) staff       (20)      197 2023-05-12 06:46:33.000000 confik-1.0.1/confik.egg-info/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)      319 2023-05-12 06:46:33.000000 confik-1.0.1/confik.egg-info/SOURCES.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-12 06:46:33.000000 confik-1.0.1/confik.egg-info/dependency_links.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        7 2023-05-12 06:46:33.000000 confik-1.0.1/confik.egg-info/top_level.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-12 06:46:33.925934 confik-1.0.1/setup.cfg
+-rw-r--r--   0 leondaz    (501) staff       (20)      277 2023-05-12 06:46:25.000000 confik-1.0.1/setup.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-12 06:46:33.925579 confik-1.0.1/tests/
+-rw-r--r--   0 leondaz    (501) staff       (20)      308 2023-05-12 06:07:05.000000 confik-1.0.1/tests/test_confik_parser.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     1482 2023-05-12 06:07:05.000000 confik-1.0.1/tests/test_read_environment_variables.py
+-rw-r--r--   0 leondaz    (501) staff       (20)      164 2023-05-12 05:54:17.000000 confik-1.0.1/tests/test_utils.py
```

### Comparing `confik-1.0.0/confik/__init__.py` & `confik-1.0.1/confik/__init__.py`

 * *Files identical despite different names*

### Comparing `confik-1.0.0/confik/parsers.py` & `confik-1.0.1/confik/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections.abc import Callable, Iterable
 
 from confik.exceptions import ConfikError
-from confik.proxies import EnvFileMappingProxy
+from confik.proxies import EnvMappingProxy
 
 
 class ConfikParser:
-    proxy_class = EnvFileMappingProxy
+    proxy_class = EnvMappingProxy
 
     def __init__(self, path=".", *args, **kwargs):
         self.source = self.proxy_class(*args, path=path, **kwargs)
 
     def validate_params(
         self,
         key,
```

### Comparing `confik-1.0.0/confik/proxies.py` & `confik-1.0.1/confik/proxies.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,34 @@
+import contextlib
 import os
 from pathlib import Path
 
 
-class EnvFileMappingProxy:
+class EnvMappingProxy:
     def __init__(self, path=Path("."), *args, **kwargs):
         assert isinstance(path, (str, Path)), "unsupported path type {t}".format(
             t=type(path)
         )
 
         environ = os.environ.copy()
 
         if isinstance(path, str):
             path = Path(path)
 
         if path.suffix != ".env":
             path = path / ".env"
 
-        with open(path, "r") as f:
-            for line in f.readlines():
-                entry = line.strip().split("=")
+        with contextlib.suppress(FileNotFoundError):
+            with open(path, "r") as f:
+                for line in f.readlines():
+                    entry = line.strip().split("=")
 
-                if len(entry) == 1:
-                    entry.append("")
+                    if len(entry) == 1:
+                        entry.append("")
 
-                name, value = entry
-                environ[name] = value.replace('"', "")
+                    name, value = entry
+                    environ[name] = value.replace('"', "")
 
         self.environ = environ
 
     def get(self, key, default):
         return self.environ.get(key, default)
```

### Comparing `confik-1.0.0/tests/test_read_environment_variables.py` & `confik-1.0.1/tests/test_read_environment_variables.py`

 * *Files identical despite different names*


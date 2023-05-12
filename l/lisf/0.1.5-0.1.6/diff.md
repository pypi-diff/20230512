# Comparing `tmp/lisf-0.1.5.tar.gz` & `tmp/lisf-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lisf-0.1.5.tar", max compression
+gzip compressed data, was "lisf-0.1.6.tar", max compression
```

## Comparing `lisf-0.1.5.tar` & `lisf-0.1.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2972 2023-05-12 07:22:57.306192 lisf-0.1.5/lisf.py
--rw-r--r--   0        0        0      405 2023-05-12 07:23:08.978456 lisf-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 lisf-0.1.5/setup.py
--rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 lisf-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     2973 2023-05-12 07:26:32.095069 lisf-0.1.6/lisf.py
+-rw-r--r--   0        0        0      405 2023-05-12 07:26:50.663493 lisf-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 lisf-0.1.6/setup.py
+-rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 lisf-0.1.6/PKG-INFO
```

### Comparing `lisf-0.1.5/lisf.py` & `lisf-0.1.6/lisf.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     def set(self, key, value):
         self._cache[key] = value
         return value
 
     def alias(self, src, dst):
         loader = self._lazy_loaders.get(src, nothing)
         if loader is not nothing:
-            self._lazy_loaders(dst, loader)
+            self._lazy_loaders[dst] = loader
         value = self._cache.get(src, nothing)
         if value is not nothing:
             self._cache[dst] = value
 
     def pop(self, key, default=None):
         result = self._cache.pop(key, default)
         return result
```


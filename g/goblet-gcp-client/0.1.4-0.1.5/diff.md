# Comparing `tmp/goblet_gcp_client-0.1.4.tar.gz` & `tmp/goblet_gcp_client-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goblet_gcp_client-0.1.4.tar", last modified: Mon May  8 18:51:34 2023, max compression
+gzip compressed data, was "goblet_gcp_client-0.1.5.tar", last modified: Fri May 12 13:03:49 2023, max compression
```

## Comparing `goblet_gcp_client-0.1.4.tar` & `goblet_gcp_client-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-05-08 18:51:34.002220 goblet_gcp_client-0.1.4/
--rw-r--r--   0 austen.novis   (502) staff       (20)    11357 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.4/LICENSE
--rw-r--r--   0 austen.novis   (502) staff       (20)     4794 2023-05-08 18:51:34.002073 goblet_gcp_client-0.1.4/PKG-INFO
--rw-r--r--   0 austen.novis   (502) staff       (20)     3984 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.4/README.md
-drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-05-08 18:51:34.001061 goblet_gcp_client-0.1.4/goblet_gcp_client/
--rw-r--r--   0 austen.novis   (502) staff       (20)      200 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.4/goblet_gcp_client/__init__.py
--rw-r--r--   0 austen.novis   (502) staff       (20)       64 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.4/goblet_gcp_client/__version__.py
--rw-r--r--   0 austen.novis   (502) staff       (20)     6335 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.4/goblet_gcp_client/client.py
--rw-r--r--   0 austen.novis   (502) staff       (20)     6033 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.4/goblet_gcp_client/http_files.py
-drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-05-08 18:51:34.001835 goblet_gcp_client-0.1.4/goblet_gcp_client.egg-info/
--rw-r--r--   0 austen.novis   (502) staff       (20)     4794 2023-05-08 18:51:33.000000 goblet_gcp_client-0.1.4/goblet_gcp_client.egg-info/PKG-INFO
--rw-r--r--   0 austen.novis   (502) staff       (20)      353 2023-05-08 18:51:33.000000 goblet_gcp_client-0.1.4/goblet_gcp_client.egg-info/SOURCES.txt
--rw-r--r--   0 austen.novis   (502) staff       (20)        1 2023-05-08 18:51:33.000000 goblet_gcp_client-0.1.4/goblet_gcp_client.egg-info/dependency_links.txt
--rw-r--r--   0 austen.novis   (502) staff       (20)       25 2023-05-08 18:51:33.000000 goblet_gcp_client-0.1.4/goblet_gcp_client.egg-info/requires.txt
--rw-r--r--   0 austen.novis   (502) staff       (20)       18 2023-05-08 18:51:33.000000 goblet_gcp_client-0.1.4/goblet_gcp_client.egg-info/top_level.txt
--rw-r--r--   0 austen.novis   (502) staff       (20)       38 2023-05-08 18:51:34.002276 goblet_gcp_client-0.1.4/setup.cfg
--rw-r--r--   0 austen.novis   (502) staff       (20)     3382 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.4/setup.py
+drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-05-12 13:03:49.082708 goblet_gcp_client-0.1.5/
+-rw-r--r--   0 austen.novis   (502) staff       (20)    11357 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.5/LICENSE
+-rw-r--r--   0 austen.novis   (502) staff       (20)     4794 2023-05-12 13:03:49.082533 goblet_gcp_client-0.1.5/PKG-INFO
+-rw-r--r--   0 austen.novis   (502) staff       (20)     3984 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.5/README.md
+drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-05-12 13:03:49.081419 goblet_gcp_client-0.1.5/goblet_gcp_client/
+-rw-r--r--   0 austen.novis   (502) staff       (20)      200 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.5/goblet_gcp_client/__init__.py
+-rw-r--r--   0 austen.novis   (502) staff       (20)       64 2023-05-12 13:03:39.000000 goblet_gcp_client-0.1.5/goblet_gcp_client/__version__.py
+-rw-r--r--   0 austen.novis   (502) staff       (20)     6335 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.5/goblet_gcp_client/client.py
+-rw-r--r--   0 austen.novis   (502) staff       (20)     6149 2023-05-12 13:03:39.000000 goblet_gcp_client-0.1.5/goblet_gcp_client/http_files.py
+drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-05-12 13:03:49.082261 goblet_gcp_client-0.1.5/goblet_gcp_client.egg-info/
+-rw-r--r--   0 austen.novis   (502) staff       (20)     4794 2023-05-12 13:03:49.000000 goblet_gcp_client-0.1.5/goblet_gcp_client.egg-info/PKG-INFO
+-rw-r--r--   0 austen.novis   (502) staff       (20)      353 2023-05-12 13:03:49.000000 goblet_gcp_client-0.1.5/goblet_gcp_client.egg-info/SOURCES.txt
+-rw-r--r--   0 austen.novis   (502) staff       (20)        1 2023-05-12 13:03:49.000000 goblet_gcp_client-0.1.5/goblet_gcp_client.egg-info/dependency_links.txt
+-rw-r--r--   0 austen.novis   (502) staff       (20)       25 2023-05-12 13:03:49.000000 goblet_gcp_client-0.1.5/goblet_gcp_client.egg-info/requires.txt
+-rw-r--r--   0 austen.novis   (502) staff       (20)       18 2023-05-12 13:03:49.000000 goblet_gcp_client-0.1.5/goblet_gcp_client.egg-info/top_level.txt
+-rw-r--r--   0 austen.novis   (502) staff       (20)       38 2023-05-12 13:03:49.082760 goblet_gcp_client-0.1.5/setup.cfg
+-rw-r--r--   0 austen.novis   (502) staff       (20)     3382 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.5/setup.py
```

### Comparing `goblet_gcp_client-0.1.4/LICENSE` & `goblet_gcp_client-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `goblet_gcp_client-0.1.4/PKG-INFO` & `goblet_gcp_client-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goblet_gcp_client
-Version: 0.1.4
+Version: 0.1.5
 Summary: GCP Client and GCP integration testing helpers
 Home-page: https://github.com/goblet/goblet_gcp_client
 Author: Austen
 Author-email: austen.novis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `goblet_gcp_client-0.1.4/README.md` & `goblet_gcp_client-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `goblet_gcp_client-0.1.4/goblet_gcp_client/client.py` & `goblet_gcp_client-0.1.5/goblet_gcp_client/client.py`

 * *Files identical despite different names*

### Comparing `goblet_gcp_client-0.1.4/goblet_gcp_client/http_files.py` & `goblet_gcp_client-0.1.5/goblet_gcp_client/http_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,16 @@
         fopen = open
         if fpath.endswith(".bz2"):
             if fpath in self._cache:
                 return self._cache[fpath]
             fopen = bz2.BZ2File
         with fopen(fpath, "rb") as fh:
             data = json.load(fh)
+            if data["body"].get("error"):
+                data["headers"]["status"] = data["body"]["error"]["code"]
             response = Response(data["headers"])
             serialized = json.dumps(data["body"]).encode("utf8")
             if fpath.endswith("bz2"):
                 self._cache[fpath] = response, serialized
             return response, serialized
```

### Comparing `goblet_gcp_client-0.1.4/goblet_gcp_client.egg-info/PKG-INFO` & `goblet_gcp_client-0.1.5/goblet_gcp_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goblet-gcp-client
-Version: 0.1.4
+Version: 0.1.5
 Summary: GCP Client and GCP integration testing helpers
 Home-page: https://github.com/goblet/goblet_gcp_client
 Author: Austen
 Author-email: austen.novis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `goblet_gcp_client-0.1.4/setup.py` & `goblet_gcp_client-0.1.5/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/ango-1.0.0.tar.gz` & `tmp/ango-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ango-1.0.0.tar", last modified: Fri May 12 08:45:39 2023, max compression
+gzip compressed data, was "ango-1.0.1.tar", last modified: Fri May 12 14:51:53 2023, max compression
```

## Comparing `ango-1.0.0.tar` & `ango-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-12 08:45:39.347913 ango-1.0.0/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-12 08:45:39.347913 ango-1.0.0/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 ango-1.0.0/README.md
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-12 08:45:39.347913 ango-1.0.0/ango/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.0/ango/__init__.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-12 08:45:39.347913 ango-1.0.0/ango/models/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.0/ango/models/__init__.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-03-08 06:39:17.000000 ango-1.0.0/ango/models/enums.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5421 2023-01-23 13:16:24.000000 ango-1.0.0/ango/models/label_category.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-02-08 11:40:21.000000 ango-1.0.0/ango/plugin_logger.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5319 2023-04-05 12:21:08.000000 ango-1.0.0/ango/plugins.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)    13920 2023-05-12 08:45:18.000000 ango-1.0.0/ango/sdk.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-12 08:45:39.347913 ango-1.0.0/ango.egg-info/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-12 08:45:39.000000 ango-1.0.0/ango.egg-info/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      299 2023-05-12 08:45:39.000000 ango-1.0.0/ango.egg-info/SOURCES.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-05-12 08:45:39.000000 ango-1.0.0/ango.egg-info/dependency_links.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      130 2023-05-12 08:45:39.000000 ango-1.0.0/ango.egg-info/requires.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        5 2023-05-12 08:45:39.000000 ango-1.0.0/ango.egg-info/top_level.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-05-12 08:45:39.347913 ango-1.0.0/setup.cfg
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      864 2023-05-05 06:29:37.000000 ango-1.0.0/setup.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-12 14:51:53.025334 ango-1.0.1/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-12 14:51:53.025334 ango-1.0.1/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 ango-1.0.1/README.md
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-12 14:51:53.025334 ango-1.0.1/ango/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.1/ango/__init__.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-12 14:51:53.025334 ango-1.0.1/ango/models/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.1/ango/models/__init__.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-03-08 06:39:17.000000 ango-1.0.1/ango/models/enums.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5421 2023-01-23 13:16:24.000000 ango-1.0.1/ango/models/label_category.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-02-08 11:40:21.000000 ango-1.0.1/ango/plugin_logger.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5319 2023-04-05 12:21:08.000000 ango-1.0.1/ango/plugins.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)    13957 2023-05-12 14:51:41.000000 ango-1.0.1/ango/sdk.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-12 14:51:53.025334 ango-1.0.1/ango.egg-info/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-12 14:51:52.000000 ango-1.0.1/ango.egg-info/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      299 2023-05-12 14:51:53.000000 ango-1.0.1/ango.egg-info/SOURCES.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-05-12 14:51:52.000000 ango-1.0.1/ango.egg-info/dependency_links.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      130 2023-05-12 14:51:52.000000 ango-1.0.1/ango.egg-info/requires.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        5 2023-05-12 14:51:53.000000 ango-1.0.1/ango.egg-info/top_level.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-05-12 14:51:53.025334 ango-1.0.1/setup.cfg
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      864 2023-05-12 14:51:50.000000 ango-1.0.1/setup.py
```

### Comparing `ango-1.0.0/PKG-INFO` & `ango-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ango
-Version: 1.0.0
+Version: 1.0.1
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: ango,ango-hub,ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ango-1.0.0/README.md` & `ango-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ango-1.0.0/ango/models/label_category.py` & `ango-1.0.1/ango/models/label_category.py`

 * *Files identical despite different names*

### Comparing `ango-1.0.0/ango/plugin_logger.py` & `ango-1.0.1/ango/plugin_logger.py`

 * *Files identical despite different names*

### Comparing `ango-1.0.0/ango/plugins.py` & `ango-1.0.1/ango/plugins.py`

 * *Files identical despite different names*

### Comparing `ango-1.0.0/ango/sdk.py` & `ango-1.0.1/ango/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 class SDK:
 
     def __init__(self, api_key, host="https://imeritapi.ango.ai"):
         self.api_key = api_key
         self.host = host
         self.session = requests.Session()
-        if host == 'https://api.ango.ai':
+        if host == 'https://api.ango.ai' or host == 'https://apibeta.ango.ai':
             logging.getLogger().error("Please downgrade your version to < 1.0.0")
         logging.getLogger().warning("Your host is %s" % host)
 
     def list_projects(self, page=1, limit=10):
         url = "%s/v2/listProjects?page=%s&limit=%s" % (self.host, page, limit)
 
         payload = {}
```

### Comparing `ango-1.0.0/ango.egg-info/PKG-INFO` & `ango-1.0.1/ango.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ango
-Version: 1.0.0
+Version: 1.0.1
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: ango,ango-hub,ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ango-1.0.0/setup.py` & `ango-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="ango",
-    version="1.0.0",
+    version="1.0.1",
     author="Faruk Karakaya",
     author_email="<faruk@ango.ai>",
     description="Ango-Hub SDK",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```


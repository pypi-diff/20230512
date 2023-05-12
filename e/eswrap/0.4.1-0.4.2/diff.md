# Comparing `tmp/eswrap-0.4.1.tar.gz` & `tmp/eswrap-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eswrap-0.4.1.tar", last modified: Fri May 12 06:15:04 2023, max compression
+gzip compressed data, was "eswrap-0.4.2.tar", last modified: Fri May 12 08:57:34 2023, max compression
```

## Comparing `eswrap-0.4.1.tar` & `eswrap-0.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:15:04.396215 eswrap-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-12 06:15:04.396215 eswrap-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-12 06:14:50.000000 eswrap-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:15:04.396215 eswrap-0.4.1/eswrap/
--rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-05-12 06:14:50.000000 eswrap-0.4.1/eswrap/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-12 06:15:04.000000 eswrap-0.4.1/eswrap/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-12 06:14:50.000000 eswrap-0.4.1/eswrap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:15:04.396215 eswrap-0.4.1/eswrap/common/
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-12 06:14:50.000000 eswrap-0.4.1/eswrap/common/EsHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 06:14:50.000000 eswrap-0.4.1/eswrap/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-12 06:14:50.000000 eswrap-0.4.1/eswrap/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 06:15:04.396215 eswrap-0.4.1/eswrap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-12 06:15:04.000000 eswrap-0.4.1/eswrap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-12 06:15:04.000000 eswrap-0.4.1/eswrap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 06:15:04.000000 eswrap-0.4.1/eswrap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-12 06:15:04.000000 eswrap-0.4.1/eswrap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 06:15:04.000000 eswrap-0.4.1/eswrap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 06:15:04.396215 eswrap-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-12 06:14:50.000000 eswrap-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:57:34.905730 eswrap-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-12 08:57:34.905730 eswrap-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-12 08:57:10.000000 eswrap-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:57:34.905730 eswrap-0.4.2/eswrap/
+-rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-05-12 08:57:10.000000 eswrap-0.4.2/eswrap/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-12 08:57:34.000000 eswrap-0.4.2/eswrap/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-12 08:57:10.000000 eswrap-0.4.2/eswrap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:57:34.905730 eswrap-0.4.2/eswrap/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-12 08:57:10.000000 eswrap-0.4.2/eswrap/common/EsHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 08:57:10.000000 eswrap-0.4.2/eswrap/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-12 08:57:10.000000 eswrap-0.4.2/eswrap/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:57:34.905730 eswrap-0.4.2/eswrap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-12 08:57:34.000000 eswrap-0.4.2/eswrap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-12 08:57:34.000000 eswrap-0.4.2/eswrap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 08:57:34.000000 eswrap-0.4.2/eswrap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-12 08:57:34.000000 eswrap-0.4.2/eswrap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 08:57:34.000000 eswrap-0.4.2/eswrap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 08:57:34.905730 eswrap-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-12 08:57:10.000000 eswrap-0.4.2/setup.py
```

### Comparing `eswrap-0.4.1/PKG-INFO` & `eswrap-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eswrap
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python wrapper for simple elasticsearch queries
 Home-page: 
 Author: Paul Tikken
 Author-email: paul.tikken@gmail.com
 License: GNU General Public License v3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `eswrap-0.4.1/eswrap/LICENSE` & `eswrap-0.4.2/eswrap/LICENSE`

 * *Files identical despite different names*

### Comparing `eswrap-0.4.1/eswrap/__init__.py` & `eswrap-0.4.2/eswrap/__init__.py`

 * *Files identical despite different names*

### Comparing `eswrap-0.4.1/eswrap/common/EsHandler.py` & `eswrap-0.4.2/eswrap/common/EsHandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,22 @@
 
         if isinstance(results, str):
             self.data_queue = None
             return
 
         try:
             if len(results["hits"]["hits"]) > 0:
-                self.data_queue = [x["_source"] for x in results["hits"]["hits"]]
+                ret_list = []
+                for x in results["hits"]["hits"]:
+                    val_dict = x["_source"]
+                    val_dict.update({"_id": x["_id"]})
+                    ret_list.append(val_dict)
+
+                self.data_queue = ret_list
+                # self.data_queue = [x["_source"] for x in results["hits"]["hits"]]
         except Exception:
             self.data_queue = results
 
     def limit(self, value: int):
         """
         Method to limit the amount of returned data; default is set to 10
```

### Comparing `eswrap-0.4.1/eswrap/main.py` & `eswrap-0.4.2/eswrap/main.py`

 * *Files identical despite different names*

### Comparing `eswrap-0.4.1/eswrap.egg-info/PKG-INFO` & `eswrap-0.4.2/eswrap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eswrap
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python wrapper for simple elasticsearch queries
 Home-page: 
 Author: Paul Tikken
 Author-email: paul.tikken@gmail.com
 License: GNU General Public License v3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `eswrap-0.4.1/setup.py` & `eswrap-0.4.2/setup.py`

 * *Files identical despite different names*


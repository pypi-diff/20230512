# Comparing `tmp/eswrap-0.4.3.tar.gz` & `tmp/eswrap-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eswrap-0.4.3.tar", last modified: Fri May 12 10:46:54 2023, max compression
+gzip compressed data, was "eswrap-0.4.4.tar", last modified: Fri May 12 11:36:05 2023, max compression
```

## Comparing `eswrap-0.4.3.tar` & `eswrap-0.4.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:46:54.974686 eswrap-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-12 10:46:54.974686 eswrap-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-12 10:46:40.000000 eswrap-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:46:54.970687 eswrap-0.4.3/eswrap/
--rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-05-12 10:46:40.000000 eswrap-0.4.3/eswrap/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-12 10:46:54.000000 eswrap-0.4.3/eswrap/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-12 10:46:40.000000 eswrap-0.4.3/eswrap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:46:54.970687 eswrap-0.4.3/eswrap/common/
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-05-12 10:46:40.000000 eswrap-0.4.3/eswrap/common/EsHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 10:46:40.000000 eswrap-0.4.3/eswrap/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-12 10:46:40.000000 eswrap-0.4.3/eswrap/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:46:54.970687 eswrap-0.4.3/eswrap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-12 10:46:54.000000 eswrap-0.4.3/eswrap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-12 10:46:54.000000 eswrap-0.4.3/eswrap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:46:54.000000 eswrap-0.4.3/eswrap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-12 10:46:54.000000 eswrap-0.4.3/eswrap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 10:46:54.000000 eswrap-0.4.3/eswrap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 10:46:54.974686 eswrap-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-12 10:46:40.000000 eswrap-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:36:05.716565 eswrap-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-12 11:36:05.716565 eswrap-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-12 11:35:48.000000 eswrap-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:36:05.716565 eswrap-0.4.4/eswrap/
+-rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-05-12 11:35:48.000000 eswrap-0.4.4/eswrap/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-12 11:36:05.000000 eswrap-0.4.4/eswrap/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-12 11:35:48.000000 eswrap-0.4.4/eswrap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:36:05.716565 eswrap-0.4.4/eswrap/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-12 11:35:48.000000 eswrap-0.4.4/eswrap/common/EsHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:35:48.000000 eswrap-0.4.4/eswrap/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-12 11:35:48.000000 eswrap-0.4.4/eswrap/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:36:05.716565 eswrap-0.4.4/eswrap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-12 11:36:05.000000 eswrap-0.4.4/eswrap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-12 11:36:05.000000 eswrap-0.4.4/eswrap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 11:36:05.000000 eswrap-0.4.4/eswrap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-12 11:36:05.000000 eswrap-0.4.4/eswrap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 11:36:05.000000 eswrap-0.4.4/eswrap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 11:36:05.716565 eswrap-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-12 11:35:48.000000 eswrap-0.4.4/setup.py
```

### Comparing `eswrap-0.4.3/PKG-INFO` & `eswrap-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eswrap
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python wrapper for simple elasticsearch queries
 Home-page: 
 Author: Paul Tikken
 Author-email: paul.tikken@gmail.com
 License: GNU General Public License v3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `eswrap-0.4.3/eswrap/LICENSE` & `eswrap-0.4.4/eswrap/LICENSE`

 * *Files identical despite different names*

### Comparing `eswrap-0.4.3/eswrap/__init__.py` & `eswrap-0.4.4/eswrap/__init__.py`

 * *Files identical despite different names*

### Comparing `eswrap-0.4.3/eswrap/common/EsHandler.py` & `eswrap-0.4.4/eswrap/common/EsHandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,16 @@
         """ """
         if filter is None:
             data = {"query": {"match_all": {}}}
         else:
             if "regexp" in kwargs:
                 if kwargs["regexp"]:
                     data = {"query": {"regexp": filter}}
+                    # popping this value; elasticsearch does not recognize this value
+                    kwargs.pop("regexp")
                 else:
                     data = {"query": {"match": filter}}
             else:
                 data = {"query": {"match": filter}}
 
         return self.es_connection.count(index=self.index, body=data, **kwargs)["count"]
 
@@ -79,15 +81,15 @@
     def __init__(
         self,
         es_handler: EsHandler,
         filter: dict = None,
         limit: int = 10,
         skip: int = None,
         sort: tuple = None,
-            **kwargs
+        **kwargs
     ):
         """
         Create a new CveSearchApi object.
 
         :param es_handler: EsHandler object
         :type es_handler: EsHandler
         """
```

### Comparing `eswrap-0.4.3/eswrap/main.py` & `eswrap-0.4.4/eswrap/main.py`

 * *Files identical despite different names*

### Comparing `eswrap-0.4.3/eswrap.egg-info/PKG-INFO` & `eswrap-0.4.4/eswrap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eswrap
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python wrapper for simple elasticsearch queries
 Home-page: 
 Author: Paul Tikken
 Author-email: paul.tikken@gmail.com
 License: GNU General Public License v3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `eswrap-0.4.3/setup.py` & `eswrap-0.4.4/setup.py`

 * *Files identical despite different names*


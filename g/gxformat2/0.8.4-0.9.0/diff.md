# Comparing `tmp/gxformat2-0.8.4.tar.gz` & `tmp/gxformat2-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gxformat2-0.8.4.tar", last modified: Mon Jun 24 19:13:30 2019, max compression
+gzip compressed data, was "dist/gxformat2-0.9.0.tar", last modified: Mon Jul  8 12:46:01 2019, max compression
```

## Comparing `gxformat2-0.8.4.tar` & `gxformat2-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 john       (502) staff       (20)        0 2019-06-24 19:13:30.000000 gxformat2-0.8.4/
-drwxr-xr-x   0 john       (502) staff       (20)        0 2019-06-24 19:13:30.000000 gxformat2-0.8.4/gxformat2/
--rw-r--r--   0 john       (502) staff       (20)      690 2019-06-24 19:13:28.000000 gxformat2-0.8.4/gxformat2/__init__.py
--rw-r--r--   0 john       (502) staff       (20)     1292 2018-10-08 19:13:45.000000 gxformat2-0.8.4/gxformat2/_yaml.py
--rw-r--r--   0 john       (502) staff       (20)    23790 2019-05-23 16:54:30.000000 gxformat2-0.8.4/gxformat2/converter.py
--rw-r--r--   0 john       (502) staff       (20)     8920 2019-06-24 19:12:34.000000 gxformat2-0.8.4/gxformat2/export.py
--rw-r--r--   0 john       (502) staff       (20)     2684 2018-10-10 13:09:05.000000 gxformat2-0.8.4/gxformat2/interface.py
--rw-r--r--   0 john       (502) staff       (20)     2165 2018-10-10 12:59:53.000000 gxformat2-0.8.4/gxformat2/main.py
-drwxr-xr-x   0 john       (502) staff       (20)        0 2019-06-24 19:13:30.000000 gxformat2-0.8.4/gxformat2.egg-info/
--rw-r--r--   0 john       (502) staff       (20)        1 2019-06-24 19:13:29.000000 gxformat2-0.8.4/gxformat2.egg-info/dependency_links.txt
--rw-r--r--   0 john       (502) staff       (20)        1 2019-06-24 19:13:29.000000 gxformat2-0.8.4/gxformat2.egg-info/entry_points.txt
--rw-r--r--   0 john       (502) staff       (20)        1 2019-06-24 19:13:29.000000 gxformat2-0.8.4/gxformat2.egg-info/not-zip-safe
--rw-r--r--   0 john       (502) staff       (20)     6126 2019-06-24 19:13:29.000000 gxformat2-0.8.4/gxformat2.egg-info/PKG-INFO
--rw-r--r--   0 john       (502) staff       (20)       27 2019-06-24 19:13:29.000000 gxformat2-0.8.4/gxformat2.egg-info/requires.txt
--rw-r--r--   0 john       (502) staff       (20)      418 2019-06-24 19:13:29.000000 gxformat2-0.8.4/gxformat2.egg-info/SOURCES.txt
--rw-r--r--   0 john       (502) staff       (20)       10 2019-06-24 19:13:29.000000 gxformat2-0.8.4/gxformat2.egg-info/top_level.txt
--rw-r--r--   0 john       (502) staff       (20)     2693 2019-06-24 19:13:28.000000 gxformat2-0.8.4/HISTORY.rst
--rw-r--r--   0 john       (502) staff       (20)    11158 2018-02-22 03:55:43.000000 gxformat2-0.8.4/LICENSE
--rw-r--r--   0 john       (502) staff       (20)       23 2018-02-22 03:55:43.000000 gxformat2-0.8.4/MANIFEST.in
--rw-r--r--   0 john       (502) staff       (20)     6126 2019-06-24 19:13:30.000000 gxformat2-0.8.4/PKG-INFO
--rw-r--r--   0 john       (502) staff       (20)     1346 2018-02-22 03:55:43.000000 gxformat2-0.8.4/README.rst
--rw-r--r--   0 john       (502) staff       (20)      308 2019-06-24 19:13:30.000000 gxformat2-0.8.4/setup.cfg
--rw-r--r--   0 john       (502) staff       (20)     2498 2018-10-02 02:51:15.000000 gxformat2-0.8.4/setup.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-07-08 12:46:01.000000 gxformat2-0.9.0/
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-07-08 12:46:01.000000 gxformat2-0.9.0/gxformat2/
+-rw-r--r--   0 john       (502) staff       (20)      690 2019-07-08 12:46:00.000000 gxformat2-0.9.0/gxformat2/__init__.py
+-rw-r--r--   0 john       (502) staff       (20)     1292 2018-10-08 19:13:45.000000 gxformat2-0.9.0/gxformat2/_yaml.py
+-rw-r--r--   0 john       (502) staff       (20)    23801 2019-07-08 12:45:17.000000 gxformat2-0.9.0/gxformat2/converter.py
+-rw-r--r--   0 john       (502) staff       (20)     8920 2019-06-24 19:12:34.000000 gxformat2-0.9.0/gxformat2/export.py
+-rw-r--r--   0 john       (502) staff       (20)     2684 2018-10-10 13:09:05.000000 gxformat2-0.9.0/gxformat2/interface.py
+-rw-r--r--   0 john       (502) staff       (20)     2165 2018-10-10 12:59:53.000000 gxformat2-0.9.0/gxformat2/main.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2019-07-08 12:46:01.000000 gxformat2-0.9.0/gxformat2.egg-info/
+-rw-r--r--   0 john       (502) staff       (20)        1 2019-07-08 12:46:01.000000 gxformat2-0.9.0/gxformat2.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (502) staff       (20)        1 2019-07-08 12:46:01.000000 gxformat2-0.9.0/gxformat2.egg-info/entry_points.txt
+-rw-r--r--   0 john       (502) staff       (20)        1 2019-07-08 12:46:01.000000 gxformat2-0.9.0/gxformat2.egg-info/not-zip-safe
+-rw-r--r--   0 john       (502) staff       (20)     6280 2019-07-08 12:46:01.000000 gxformat2-0.9.0/gxformat2.egg-info/PKG-INFO
+-rw-r--r--   0 john       (502) staff       (20)       27 2019-07-08 12:46:00.000000 gxformat2-0.9.0/gxformat2.egg-info/requires.txt
+-rw-r--r--   0 john       (502) staff       (20)      418 2019-07-08 12:46:01.000000 gxformat2-0.9.0/gxformat2.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (502) staff       (20)       10 2019-07-08 12:46:01.000000 gxformat2-0.9.0/gxformat2.egg-info/top_level.txt
+-rw-r--r--   0 john       (502) staff       (20)     2799 2019-07-08 12:46:00.000000 gxformat2-0.9.0/HISTORY.rst
+-rw-r--r--   0 john       (502) staff       (20)    11158 2018-02-22 03:55:43.000000 gxformat2-0.9.0/LICENSE
+-rw-r--r--   0 john       (502) staff       (20)       23 2018-02-22 03:55:43.000000 gxformat2-0.9.0/MANIFEST.in
+-rw-r--r--   0 john       (502) staff       (20)     6280 2019-07-08 12:46:01.000000 gxformat2-0.9.0/PKG-INFO
+-rw-r--r--   0 john       (502) staff       (20)     1346 2018-02-22 03:55:43.000000 gxformat2-0.9.0/README.rst
+-rw-r--r--   0 john       (502) staff       (20)      308 2019-07-08 12:46:01.000000 gxformat2-0.9.0/setup.cfg
+-rw-r--r--   0 john       (502) staff       (20)     2498 2018-10-02 02:51:15.000000 gxformat2-0.9.0/setup.py
```

### Comparing `gxformat2-0.8.4/gxformat2/__init__.py` & `gxformat2-0.9.0/gxformat2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """The public interface or entry point for the Format 2 workflow code."""
 
-__version__ = '0.8.4'
+__version__ = '0.9.0'
 
 PROJECT_NAME = "gxformat2"
 PROJECT_OWNER = PROJECT_USERAME = "jmchilton"
 PROJECT_AUTHOR = 'Galaxy Project and Community'
 PROJECT_EMAIL = 'jmchilton@gmail.com'
 PROJECT_URL = "https://github.com/jmchilton/gxformat2"
```

### Comparing `gxformat2-0.8.4/gxformat2/_yaml.py` & `gxformat2-0.9.0/gxformat2/_yaml.py`

 * *Files identical despite different names*

### Comparing `gxformat2-0.8.4/gxformat2/converter.py` & `gxformat2-0.9.0/gxformat2/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,15 +330,15 @@
     _ensure_defaults(step_inputs, {
         "name": name,
         "description": "",
     })
     tool_state = {
         "name": name
     }
-    for attrib in ["collection_type", "parameter_type", "optional"]:
+    for attrib in ["collection_type", "parameter_type", "optional", "default"]:
         if attrib in step:
             tool_state[attrib] = step[attrib]
 
     _populate_tool_state(step, tool_state)
 
 
 def transform_pause(context, step, default_name="Pause for dataset review"):
```

### Comparing `gxformat2-0.8.4/gxformat2/export.py` & `gxformat2-0.9.0/gxformat2/export.py`

 * *Files identical despite different names*

### Comparing `gxformat2-0.8.4/gxformat2/interface.py` & `gxformat2-0.9.0/gxformat2/interface.py`

 * *Files identical despite different names*

### Comparing `gxformat2-0.8.4/gxformat2/main.py` & `gxformat2-0.9.0/gxformat2/main.py`

 * *Files identical despite different names*

### Comparing `gxformat2-0.8.4/gxformat2.egg-info/PKG-INFO` & `gxformat2-0.9.0/gxformat2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: gxformat2
-Version: 0.8.4
+Version: 0.9.0
 Summary: Galaxy Workflow Format 2 Descriptions
 Home-page: https://github.com/jmchilton/gxformat2
 Author: Galaxy Project and Community
 Author-email: jmchilton@gmail.com
 License: AFL
 Description-Content-Type: UNKNOWN
 Description: 
@@ -47,14 +47,20 @@
         
         History
         -------
         
         .. to_doc
         
         ---------------------
+        0.9.0 (2019-07-08)
+        ---------------------
+        
+        * Implement default values in gxformat2.
+        
+        ---------------------
         0.8.4 (2019-06-24)
         ---------------------
         
         * Fix output IDs of 0.    
         
         ---------------------
         0.8.3 (2019-05-23)
```

### Comparing `gxformat2-0.8.4/HISTORY.rst` & `gxformat2-0.9.0/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 
 History
 -------
 
 .. to_doc
 
 ---------------------
+0.9.0 (2019-07-08)
+---------------------
+
+* Implement default values in gxformat2.
+
+---------------------
 0.8.4 (2019-06-24)
 ---------------------
 
 * Fix output IDs of 0.    
 
 ---------------------
 0.8.3 (2019-05-23)
```

### Comparing `gxformat2-0.8.4/LICENSE` & `gxformat2-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gxformat2-0.8.4/PKG-INFO` & `gxformat2-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: gxformat2
-Version: 0.8.4
+Version: 0.9.0
 Summary: Galaxy Workflow Format 2 Descriptions
 Home-page: https://github.com/jmchilton/gxformat2
 Author: Galaxy Project and Community
 Author-email: jmchilton@gmail.com
 License: AFL
 Description-Content-Type: UNKNOWN
 Description: 
@@ -47,14 +47,20 @@
         
         History
         -------
         
         .. to_doc
         
         ---------------------
+        0.9.0 (2019-07-08)
+        ---------------------
+        
+        * Implement default values in gxformat2.
+        
+        ---------------------
         0.8.4 (2019-06-24)
         ---------------------
         
         * Fix output IDs of 0.    
         
         ---------------------
         0.8.3 (2019-05-23)
```

### Comparing `gxformat2-0.8.4/README.rst` & `gxformat2-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `gxformat2-0.8.4/setup.py` & `gxformat2-0.9.0/setup.py`

 * *Files identical despite different names*


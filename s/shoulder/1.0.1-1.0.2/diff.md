# Comparing `tmp/shoulder-1.0.1.tar.gz` & `tmp/shoulder-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shoulder-1.0.1.tar", max compression
+gzip compressed data, was "shoulder-1.0.2.tar", max compression
```

## Comparing `shoulder-1.0.1.tar` & `shoulder-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1097 2023-05-12 01:39:37.059210 shoulder-1.0.1/LICENSE.md
--rw-r--r--   0        0        0     1765 2023-05-12 01:44:36.173649 shoulder-1.0.1/README.md
--rw-r--r--   0        0        0      879 2023-05-12 01:46:29.126572 shoulder-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      109 2023-05-12 01:39:37.059210 shoulder-1.0.1/src/shoulder/__init__.py
--rw-r--r--   0        0        0     1293 2023-05-12 01:39:37.059210 shoulder-1.0.1/src/shoulder/base.py
--rw-r--r--   0        0        0     2766 2023-05-12 01:39:37.059210 shoulder-1.0.1/src/shoulder/bone.py
--rw-r--r--   0        0        0        0 2023-05-12 01:39:37.059210 shoulder-1.0.1/src/shoulder/glenoid/__init__.py
--rw-r--r--   0        0        0        1 2023-05-12 01:39:37.059210 shoulder-1.0.1/src/shoulder/humerus/__init__.py
--rw-r--r--   0        0        0    18070 2023-05-12 01:39:37.059210 shoulder-1.0.1/src/shoulder/humerus/anatomic_neck.py
--rw-r--r--   0        0        0     3297 2023-05-12 01:39:37.059210 shoulder-1.0.1/src/shoulder/humerus/angles.py
--rw-r--r--   0        0        0    12438 2023-05-12 01:39:37.059210 shoulder-1.0.1/src/shoulder/humerus/bicipital_groove.py
--rw-r--r--   0        0        0     6714 2023-05-12 01:39:37.059210 shoulder-1.0.1/src/shoulder/humerus/canal.py
--rw-r--r--   0        0        0     5277 2023-05-12 01:39:37.059210 shoulder-1.0.1/src/shoulder/humerus/epicondyle.py
--rw-r--r--   0        0        0     7252 2023-05-12 01:39:37.059210 shoulder-1.0.1/src/shoulder/humerus/mesh.py
--rw-r--r--   0        0        0     2803 2023-05-12 01:39:37.059210 shoulder-1.0.1/src/shoulder/plotting.py
--rw-r--r--   0        0        0     6681 2023-05-12 01:39:37.059210 shoulder-1.0.1/src/shoulder/utils.py
--rw-r--r--   0        0        0     2762 1970-01-01 00:00:00.000000 shoulder-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-05-12 01:39:37.059210 shoulder-1.0.2/LICENSE.md
+-rw-r--r--   0        0        0     1829 2023-05-12 02:04:38.546625 shoulder-1.0.2/README.md
+-rw-r--r--   0        0        0      879 2023-05-12 02:05:36.618969 shoulder-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/__init__.py
+-rw-r--r--   0        0        0     1293 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/base.py
+-rw-r--r--   0        0        0     2766 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/bone.py
+-rw-r--r--   0        0        0        0 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/glenoid/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/humerus/__init__.py
+-rw-r--r--   0        0        0    18070 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/humerus/anatomic_neck.py
+-rw-r--r--   0        0        0     3297 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/humerus/angles.py
+-rw-r--r--   0        0        0    12438 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/humerus/bicipital_groove.py
+-rw-r--r--   0        0        0     6714 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/humerus/canal.py
+-rw-r--r--   0        0        0     5277 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/humerus/epicondyle.py
+-rw-r--r--   0        0        0     7252 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/humerus/mesh.py
+-rw-r--r--   0        0        0     2803 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/plotting.py
+-rw-r--r--   0        0        0     6681 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/utils.py
+-rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 shoulder-1.0.2/PKG-INFO
```

### Comparing `shoulder-1.0.1/LICENSE.md` & `shoulder-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.1/README.md` & `shoulder-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     # construct plot from above humeral bone with landmarks and coordinate system
     plot = shoulder.Plot(hum)
     plot.figure.show()
 
 The output of the plot will appear as shown below with landmarks included and transformed from the original CT coordinate system to a coordainte system defined by the canal and transepicondylar axis.
 
-![Plot of Example code above](images/plot.png)
+![Plot of Example code above](https://raw.githubusercontent.com/gregspangenberg/shoulder/main/images/plot.png)
 
 
 ## Contributing 
 Clone the repo, open the cloned folder containing the poetry.lock file, then install the development dependencies using poetry. 
 ```
 poetry install --with dev
 ```
```

### Comparing `shoulder-1.0.1/pyproject.toml` & `shoulder-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shoulder"
-version = "1.0.1"
+version = "1.0.2"
 description = "patient specific anatomic coordinate system generation for shoulder bones"
 authors = ["Gregory W Spangenberg <gspangen@westerneng.ca>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gregspangenberg/shoulder"
 
 [tool.poetry.dependencies]
```

### Comparing `shoulder-1.0.1/src/shoulder/base.py` & `shoulder-1.0.2/src/shoulder/base.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.1/src/shoulder/bone.py` & `shoulder-1.0.2/src/shoulder/bone.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.1/src/shoulder/humerus/anatomic_neck.py` & `shoulder-1.0.2/src/shoulder/humerus/anatomic_neck.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.1/src/shoulder/humerus/angles.py` & `shoulder-1.0.2/src/shoulder/humerus/angles.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.1/src/shoulder/humerus/bicipital_groove.py` & `shoulder-1.0.2/src/shoulder/humerus/bicipital_groove.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.1/src/shoulder/humerus/canal.py` & `shoulder-1.0.2/src/shoulder/humerus/canal.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.1/src/shoulder/humerus/epicondyle.py` & `shoulder-1.0.2/src/shoulder/humerus/epicondyle.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.1/src/shoulder/humerus/mesh.py` & `shoulder-1.0.2/src/shoulder/humerus/mesh.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.1/src/shoulder/plotting.py` & `shoulder-1.0.2/src/shoulder/plotting.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.1/src/shoulder/utils.py` & `shoulder-1.0.2/src/shoulder/utils.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.1/PKG-INFO` & `shoulder-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shoulder
-Version: 1.0.1
+Version: 1.0.2
 Summary: patient specific anatomic coordinate system generation for shoulder bones
 Home-page: https://github.com/gregspangenberg/shoulder
 License: MIT
 Author: Gregory W Spangenberg
 Author-email: gspangen@westerneng.ca
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -61,15 +61,15 @@
 
     # construct plot from above humeral bone with landmarks and coordinate system
     plot = shoulder.Plot(hum)
     plot.figure.show()
 
 The output of the plot will appear as shown below with landmarks included and transformed from the original CT coordinate system to a coordainte system defined by the canal and transepicondylar axis.
 
-![Plot of Example code above](images/plot.png)
+![Plot of Example code above](https://raw.githubusercontent.com/gregspangenberg/shoulder/main/images/plot.png)
 
 
 ## Contributing 
 Clone the repo, open the cloned folder containing the poetry.lock file, then install the development dependencies using poetry. 
 ```
 poetry install --with dev
 ```
```


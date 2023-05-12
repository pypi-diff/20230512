# Comparing `tmp/shoulder-1.0.4.tar.gz` & `tmp/shoulder-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shoulder-1.0.4.tar", max compression
+gzip compressed data, was "shoulder-1.0.5.tar", max compression
```

## Comparing `shoulder-1.0.4.tar` & `shoulder-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1097 2023-05-12 01:39:37.059210 shoulder-1.0.4/LICENSE.md
--rw-r--r--   0        0        0     1829 2023-05-12 02:04:38.546625 shoulder-1.0.4/README.md
--rw-r--r--   0        0        0      879 2023-05-12 20:22:51.805316 shoulder-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      109 2023-05-12 01:39:37.059210 shoulder-1.0.4/src/shoulder/__init__.py
--rw-r--r--   0        0        0     1293 2023-05-12 01:39:37.059210 shoulder-1.0.4/src/shoulder/base.py
--rw-r--r--   0        0        0     2718 2023-05-12 18:56:43.185059 shoulder-1.0.4/src/shoulder/bone.py
--rw-r--r--   0        0        0        0 2023-05-12 01:39:37.059210 shoulder-1.0.4/src/shoulder/glenoid/__init__.py
--rw-r--r--   0        0        0        1 2023-05-12 01:39:37.059210 shoulder-1.0.4/src/shoulder/humerus/__init__.py
--rw-r--r--   0        0        0    18092 2023-05-12 18:56:15.052822 shoulder-1.0.4/src/shoulder/humerus/anatomic_neck.py
--rw-r--r--   0        0        0     3297 2023-05-12 01:39:37.059210 shoulder-1.0.4/src/shoulder/humerus/angles.py
--rw-r--r--   0        0        0    11404 2023-05-12 18:05:39.879225 shoulder-1.0.4/src/shoulder/humerus/bicipital_groove.py
--rw-r--r--   0        0        0     6756 2023-05-12 18:50:36.369783 shoulder-1.0.4/src/shoulder/humerus/canal.py
--rw-r--r--   0        0        0     5267 2023-05-12 18:56:35.104991 shoulder-1.0.4/src/shoulder/humerus/epicondyle.py
--rw-r--r--   0        0        0     7262 2023-05-12 04:24:24.053927 shoulder-1.0.4/src/shoulder/humerus/mesh.py
--rw-r--r--   0        0        0     2803 2023-05-12 01:39:37.059210 shoulder-1.0.4/src/shoulder/plotting.py
--rw-r--r--   0        0        0     6681 2023-05-12 01:39:37.059210 shoulder-1.0.4/src/shoulder/utils.py
--rw-r--r--   0        0        0     2877 1970-01-01 00:00:00.000000 shoulder-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-05-12 01:39:37.059210 shoulder-1.0.5/LICENSE.md
+-rw-r--r--   0        0        0     1829 2023-05-12 02:04:38.546625 shoulder-1.0.5/README.md
+-rw-r--r--   0        0        0      879 2023-05-12 20:31:12.545279 shoulder-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-05-12 01:39:37.059210 shoulder-1.0.5/src/shoulder/__init__.py
+-rw-r--r--   0        0        0     1293 2023-05-12 01:39:37.059210 shoulder-1.0.5/src/shoulder/base.py
+-rw-r--r--   0        0        0     2718 2023-05-12 18:56:43.185059 shoulder-1.0.5/src/shoulder/bone.py
+-rw-r--r--   0        0        0        0 2023-05-12 01:39:37.059210 shoulder-1.0.5/src/shoulder/glenoid/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-12 01:39:37.059210 shoulder-1.0.5/src/shoulder/humerus/__init__.py
+-rw-r--r--   0        0        0    18093 2023-05-12 20:29:51.032233 shoulder-1.0.5/src/shoulder/humerus/anatomic_neck.py
+-rw-r--r--   0        0        0     3297 2023-05-12 01:39:37.059210 shoulder-1.0.5/src/shoulder/humerus/angles.py
+-rw-r--r--   0        0        0    11404 2023-05-12 18:05:39.879225 shoulder-1.0.5/src/shoulder/humerus/bicipital_groove.py
+-rw-r--r--   0        0        0     6756 2023-05-12 18:50:36.369783 shoulder-1.0.5/src/shoulder/humerus/canal.py
+-rw-r--r--   0        0        0     5267 2023-05-12 18:56:35.104991 shoulder-1.0.5/src/shoulder/humerus/epicondyle.py
+-rw-r--r--   0        0        0     7262 2023-05-12 04:24:24.053927 shoulder-1.0.5/src/shoulder/humerus/mesh.py
+-rw-r--r--   0        0        0     2803 2023-05-12 01:39:37.059210 shoulder-1.0.5/src/shoulder/plotting.py
+-rw-r--r--   0        0        0     6681 2023-05-12 01:39:37.059210 shoulder-1.0.5/src/shoulder/utils.py
+-rw-r--r--   0        0        0     2877 1970-01-01 00:00:00.000000 shoulder-1.0.5/PKG-INFO
```

### Comparing `shoulder-1.0.4/LICENSE.md` & `shoulder-1.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.4/README.md` & `shoulder-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.4/pyproject.toml` & `shoulder-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shoulder"
-version = "1.0.4"
+version = "1.0.5"
 description = "patient specific anatomic coordinate system generation for shoulder bones"
 authors = ["Gregory W Spangenberg <gspangen@westerneng.ca>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gregspangenberg/shoulder"
 
 [tool.poetry.dependencies]
```

### Comparing `shoulder-1.0.4/src/shoulder/base.py` & `shoulder-1.0.5/src/shoulder/base.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.4/src/shoulder/bone.py` & `shoulder-1.0.5/src/shoulder/bone.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.4/src/shoulder/humerus/anatomic_neck.py` & `shoulder-1.0.5/src/shoulder/humerus/anatomic_neck.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             circle_threshold = 0.3
             sup_inf_num = 16
             med_lat_num = 8
 
             articular_pt, hc_mnr_axis, medial_epicondyle_pt = self.__seed(
                 self._mesh_oriented,
                 50,
-                utils.transform_pts(self.transepi_axis, self._transform),
+                utils.transform_pts(self._transepi_axis, self._transform),
             )
             # Slice along the head central minor axis
             # find which endpoint of hc_mnr_axis is closer to the medial_epicondyle_pt,
             # that side contins the greater tuberosity
             gt_side_pt, non_gt_side_pt = utils.closest_pt(
                 medial_epicondyle_pt[:, :-1], hc_mnr_axis[:, :-1], return_other_pts=True
             )  # z removed from inputs
```

### Comparing `shoulder-1.0.4/src/shoulder/humerus/angles.py` & `shoulder-1.0.5/src/shoulder/humerus/angles.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.4/src/shoulder/humerus/bicipital_groove.py` & `shoulder-1.0.5/src/shoulder/humerus/bicipital_groove.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.4/src/shoulder/humerus/canal.py` & `shoulder-1.0.5/src/shoulder/humerus/canal.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.4/src/shoulder/humerus/epicondyle.py` & `shoulder-1.0.5/src/shoulder/humerus/epicondyle.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.4/src/shoulder/humerus/mesh.py` & `shoulder-1.0.5/src/shoulder/humerus/mesh.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.4/src/shoulder/plotting.py` & `shoulder-1.0.5/src/shoulder/plotting.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.4/src/shoulder/utils.py` & `shoulder-1.0.5/src/shoulder/utils.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.4/PKG-INFO` & `shoulder-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shoulder
-Version: 1.0.4
+Version: 1.0.5
 Summary: patient specific anatomic coordinate system generation for shoulder bones
 Home-page: https://github.com/gregspangenberg/shoulder
 License: MIT
 Author: Gregory W Spangenberg
 Author-email: gspangen@westerneng.ca
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
```


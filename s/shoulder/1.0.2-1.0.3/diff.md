# Comparing `tmp/shoulder-1.0.2.tar.gz` & `tmp/shoulder-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shoulder-1.0.2.tar", max compression
+gzip compressed data, was "shoulder-1.0.3.tar", max compression
```

## Comparing `shoulder-1.0.2.tar` & `shoulder-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1097 2023-05-12 01:39:37.059210 shoulder-1.0.2/LICENSE.md
--rw-r--r--   0        0        0     1829 2023-05-12 02:04:38.546625 shoulder-1.0.2/README.md
--rw-r--r--   0        0        0      879 2023-05-12 02:05:36.618969 shoulder-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      109 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/__init__.py
--rw-r--r--   0        0        0     1293 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/base.py
--rw-r--r--   0        0        0     2766 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/bone.py
--rw-r--r--   0        0        0        0 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/glenoid/__init__.py
--rw-r--r--   0        0        0        1 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/humerus/__init__.py
--rw-r--r--   0        0        0    18070 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/humerus/anatomic_neck.py
--rw-r--r--   0        0        0     3297 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/humerus/angles.py
--rw-r--r--   0        0        0    12438 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/humerus/bicipital_groove.py
--rw-r--r--   0        0        0     6714 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/humerus/canal.py
--rw-r--r--   0        0        0     5277 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/humerus/epicondyle.py
--rw-r--r--   0        0        0     7252 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/humerus/mesh.py
--rw-r--r--   0        0        0     2803 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/plotting.py
--rw-r--r--   0        0        0     6681 2023-05-12 01:39:37.059210 shoulder-1.0.2/src/shoulder/utils.py
--rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 shoulder-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-05-12 01:39:37.059210 shoulder-1.0.3/LICENSE.md
+-rw-r--r--   0        0        0     1829 2023-05-12 02:04:38.546625 shoulder-1.0.3/README.md
+-rw-r--r--   0        0        0      879 2023-05-12 04:44:19.778765 shoulder-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-05-12 01:39:37.059210 shoulder-1.0.3/src/shoulder/__init__.py
+-rw-r--r--   0        0        0     1293 2023-05-12 01:39:37.059210 shoulder-1.0.3/src/shoulder/base.py
+-rw-r--r--   0        0        0     2766 2023-05-12 01:39:37.059210 shoulder-1.0.3/src/shoulder/bone.py
+-rw-r--r--   0        0        0        0 2023-05-12 01:39:37.059210 shoulder-1.0.3/src/shoulder/glenoid/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-12 01:39:37.059210 shoulder-1.0.3/src/shoulder/humerus/__init__.py
+-rw-r--r--   0        0        0    18080 2023-05-12 04:40:25.125002 shoulder-1.0.3/src/shoulder/humerus/anatomic_neck.py
+-rw-r--r--   0        0        0     3297 2023-05-12 01:39:37.059210 shoulder-1.0.3/src/shoulder/humerus/angles.py
+-rw-r--r--   0        0        0    12458 2023-05-12 04:25:10.430258 shoulder-1.0.3/src/shoulder/humerus/bicipital_groove.py
+-rw-r--r--   0        0        0     6756 2023-05-12 04:24:05.845798 shoulder-1.0.3/src/shoulder/humerus/canal.py
+-rw-r--r--   0        0        0     5287 2023-05-12 04:15:16.322134 shoulder-1.0.3/src/shoulder/humerus/epicondyle.py
+-rw-r--r--   0        0        0     7262 2023-05-12 04:24:24.053927 shoulder-1.0.3/src/shoulder/humerus/mesh.py
+-rw-r--r--   0        0        0     2803 2023-05-12 01:39:37.059210 shoulder-1.0.3/src/shoulder/plotting.py
+-rw-r--r--   0        0        0     6681 2023-05-12 01:39:37.059210 shoulder-1.0.3/src/shoulder/utils.py
+-rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 shoulder-1.0.3/PKG-INFO
```

### Comparing `shoulder-1.0.2/LICENSE.md` & `shoulder-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.2/README.md` & `shoulder-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.2/pyproject.toml` & `shoulder-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shoulder"
-version = "1.0.2"
+version = "1.0.3"
 description = "patient specific anatomic coordinate system generation for shoulder bones"
 authors = ["Gregory W Spangenberg <gspangen@westerneng.ca>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gregspangenberg/shoulder"
 
 [tool.poetry.dependencies]
```

### Comparing `shoulder-1.0.2/src/shoulder/base.py` & `shoulder-1.0.3/src/shoulder/base.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.2/src/shoulder/bone.py` & `shoulder-1.0.3/src/shoulder/bone.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.2/src/shoulder/humerus/anatomic_neck.py` & `shoulder-1.0.3/src/shoulder/humerus/anatomic_neck.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
                 mesh.bounds[:, -1] <= 0, -1
             ]  # bone in negative space, bone past the centerline midpoint
 
             distal_cutoff = 0.85 * total_length + neg_length
             proximal_cutoff = 0.99 * total_length + neg_length
 
             # spacing of cuts
-            cuts = np.linspace(distal_cutoff, proximal_cutoff, num=num_slice)
+            cuts = np.linspace(distal_cutoff, proximal_cutoff, num=num_slice).flatten()
 
             for cut in cuts:
                 try:
                     path = mesh.section(
                         plane_origin=[0, 0, cut], plane_normal=[0, 0, 1]
                     )
                     slice, to_3d = path.to_planar()
```

### Comparing `shoulder-1.0.2/src/shoulder/humerus/angles.py` & `shoulder-1.0.3/src/shoulder/humerus/angles.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.2/src/shoulder/humerus/bicipital_groove.py` & `shoulder-1.0.3/src/shoulder/humerus/bicipital_groove.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     def axis(self, slice_num=35, interp_num=250):
         if self._axis is None:
             # slice_num  must use odd soo add 1 if even
             if (slice_num % 2) == 0:
                 slice_num += 1
 
             z_max = np.max(self._mesh_oriented_uobb.bounds[:, -1])
-            zs = np.linspace(0.92 * z_max, 0.75 * z_max, num=slice_num)
+            zs = np.linspace(0.92 * z_max, 0.75 * z_max, num=slice_num).flatten()
 
             pts = np.zeros((interp_num, 2, slice_num))
             pts_r = np.zeros((interp_num, 2, slice_num))
             pts_r_sp = np.zeros((interp_num, 2, slice_num))
             weights = np.zeros((interp_num, 2, slice_num))
             to_3Ds = np.zeros((4, 4, slice_num))
 
@@ -49,15 +49,15 @@
                 _pts = _resample_polygon(_pts, interp_num)
 
                 pol = _cart2pol(_pts)
 
                 f = scipy.interpolate.interp1d(pol[:, 0], pol[:, 1])
                 theta_spaced = np.linspace(
                     np.min(pol[:, 0]), np.max(pol[:, 0]), (interp_num)
-                )
+                ).flatten()
                 r_spaced = f(theta_spaced)
 
                 pol_spaced = np.c_[theta_spaced, r_spaced]
 
                 xy = _pol2cart(pol_spaced)
 
                 # if a cavity is present do not count that as a weight
```

### Comparing `shoulder-1.0.2/src/shoulder/humerus/canal.py` & `shoulder-1.0.3/src/shoulder/humerus/canal.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,17 @@
                 y_length / 2
             )  # pct of total y-length then subtract to return center to 0
             proximal_cutoff = cutoff_pcts[1] * y_length - (y_length / 2)
             # length between cutoff pts
             cutoff_length = abs(proximal_cutoff - distal_cutoff)
 
             # spacing of cuts
-            cuts = np.linspace(distal_cutoff, proximal_cutoff, num=num_centroids)
+            cuts = np.linspace(
+                distal_cutoff, proximal_cutoff, num=num_centroids
+            ).flatten()
 
             centroids = []  # record data
             for cut in cuts:
                 slice = msh_o.section(plane_origin=[0, 0, cut], plane_normal=[0, 0, 1])
                 centroids.append(np.array(slice.centroid).reshape(1, 3))
 
             centroids = np.concatenate(centroids, axis=0)
```

### Comparing `shoulder-1.0.2/src/shoulder/humerus/epicondyle.py` & `shoulder-1.0.3/src/shoulder/humerus/epicondyle.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,18 @@
                 msh_o.bounds[:, -1] >= 0, -1
             ]  # bone in positive space, bone before the centerline midpoint
 
             proximal_cutoff = -0.8 * total_length + pos_length
             distal_cutoff = -0.99 * total_length + pos_length
 
             # spacing of cuts
-            cuts = np.linspace(proximal_cutoff, distal_cutoff, num=num_slices)
+            cuts = np.linspace(proximal_cutoff, distal_cutoff, num=num_slices).flatten()
 
             dist = []
+
             for cut in cuts:
                 try:
                     path = msh_o.section(
                         plane_origin=[0, 0, cut], plane_normal=[0, 0, 1]
                     )
                     slice, to_3d = path.to_planar()
                 except:
@@ -51,15 +52,14 @@
                 polygon = slice.polygons_closed[0]
 
                 # create rotated bounding box
                 majr_dist = utils.major_axis_dist(
                     polygon.minimum_rotated_rectangle
                 )  # maximize this distance
                 dist.append(majr_dist)
-
             idx_max_dist = dist.index(max(dist))
             max_dist_cut = cuts[idx_max_dist]
 
             return max_dist_cut
 
         if self._axis is None:
             # find z distance where medial lateral distance is longest
```

### Comparing `shoulder-1.0.2/src/shoulder/humerus/mesh.py` & `shoulder-1.0.3/src/shoulder/humerus/mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
 
         # find largest area along z axis
         inset_factor = 0.99  # percent shrink z of first slice
         # evenly space z intervals
         num_zs = 100
         z_intervals = np.linspace(
             z_limits[0] * inset_factor, z_limits[1] * inset_factor, num_zs
-        )
+        ).flatten()
         z_area = []
         for z in z_intervals:
             slice = _mesh.section(plane_origin=[0, 0, z], plane_normal=[0, 0, 1])
             slice, to_3d = slice.to_planar()
             z_area.append(slice.area)
 
         # the middle of humeral head has the largest area for proximal humerus
```

### Comparing `shoulder-1.0.2/src/shoulder/plotting.py` & `shoulder-1.0.3/src/shoulder/plotting.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.2/src/shoulder/utils.py` & `shoulder-1.0.3/src/shoulder/utils.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.2/PKG-INFO` & `shoulder-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shoulder
-Version: 1.0.2
+Version: 1.0.3
 Summary: patient specific anatomic coordinate system generation for shoulder bones
 Home-page: https://github.com/gregspangenberg/shoulder
 License: MIT
 Author: Gregory W Spangenberg
 Author-email: gspangen@westerneng.ca
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
```


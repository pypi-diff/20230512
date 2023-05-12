# Comparing `tmp/shoulder-1.0.3.tar.gz` & `tmp/shoulder-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shoulder-1.0.3.tar", max compression
+gzip compressed data, was "shoulder-1.0.4.tar", max compression
```

## Comparing `shoulder-1.0.3.tar` & `shoulder-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1097 2023-05-12 01:39:37.059210 shoulder-1.0.3/LICENSE.md
--rw-r--r--   0        0        0     1829 2023-05-12 02:04:38.546625 shoulder-1.0.3/README.md
--rw-r--r--   0        0        0      879 2023-05-12 04:44:19.778765 shoulder-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      109 2023-05-12 01:39:37.059210 shoulder-1.0.3/src/shoulder/__init__.py
--rw-r--r--   0        0        0     1293 2023-05-12 01:39:37.059210 shoulder-1.0.3/src/shoulder/base.py
--rw-r--r--   0        0        0     2766 2023-05-12 01:39:37.059210 shoulder-1.0.3/src/shoulder/bone.py
--rw-r--r--   0        0        0        0 2023-05-12 01:39:37.059210 shoulder-1.0.3/src/shoulder/glenoid/__init__.py
--rw-r--r--   0        0        0        1 2023-05-12 01:39:37.059210 shoulder-1.0.3/src/shoulder/humerus/__init__.py
--rw-r--r--   0        0        0    18080 2023-05-12 04:40:25.125002 shoulder-1.0.3/src/shoulder/humerus/anatomic_neck.py
--rw-r--r--   0        0        0     3297 2023-05-12 01:39:37.059210 shoulder-1.0.3/src/shoulder/humerus/angles.py
--rw-r--r--   0        0        0    12458 2023-05-12 04:25:10.430258 shoulder-1.0.3/src/shoulder/humerus/bicipital_groove.py
--rw-r--r--   0        0        0     6756 2023-05-12 04:24:05.845798 shoulder-1.0.3/src/shoulder/humerus/canal.py
--rw-r--r--   0        0        0     5287 2023-05-12 04:15:16.322134 shoulder-1.0.3/src/shoulder/humerus/epicondyle.py
--rw-r--r--   0        0        0     7262 2023-05-12 04:24:24.053927 shoulder-1.0.3/src/shoulder/humerus/mesh.py
--rw-r--r--   0        0        0     2803 2023-05-12 01:39:37.059210 shoulder-1.0.3/src/shoulder/plotting.py
--rw-r--r--   0        0        0     6681 2023-05-12 01:39:37.059210 shoulder-1.0.3/src/shoulder/utils.py
--rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 shoulder-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-05-12 01:39:37.059210 shoulder-1.0.4/LICENSE.md
+-rw-r--r--   0        0        0     1829 2023-05-12 02:04:38.546625 shoulder-1.0.4/README.md
+-rw-r--r--   0        0        0      879 2023-05-12 20:22:51.805316 shoulder-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-05-12 01:39:37.059210 shoulder-1.0.4/src/shoulder/__init__.py
+-rw-r--r--   0        0        0     1293 2023-05-12 01:39:37.059210 shoulder-1.0.4/src/shoulder/base.py
+-rw-r--r--   0        0        0     2718 2023-05-12 18:56:43.185059 shoulder-1.0.4/src/shoulder/bone.py
+-rw-r--r--   0        0        0        0 2023-05-12 01:39:37.059210 shoulder-1.0.4/src/shoulder/glenoid/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-12 01:39:37.059210 shoulder-1.0.4/src/shoulder/humerus/__init__.py
+-rw-r--r--   0        0        0    18092 2023-05-12 18:56:15.052822 shoulder-1.0.4/src/shoulder/humerus/anatomic_neck.py
+-rw-r--r--   0        0        0     3297 2023-05-12 01:39:37.059210 shoulder-1.0.4/src/shoulder/humerus/angles.py
+-rw-r--r--   0        0        0    11404 2023-05-12 18:05:39.879225 shoulder-1.0.4/src/shoulder/humerus/bicipital_groove.py
+-rw-r--r--   0        0        0     6756 2023-05-12 18:50:36.369783 shoulder-1.0.4/src/shoulder/humerus/canal.py
+-rw-r--r--   0        0        0     5267 2023-05-12 18:56:35.104991 shoulder-1.0.4/src/shoulder/humerus/epicondyle.py
+-rw-r--r--   0        0        0     7262 2023-05-12 04:24:24.053927 shoulder-1.0.4/src/shoulder/humerus/mesh.py
+-rw-r--r--   0        0        0     2803 2023-05-12 01:39:37.059210 shoulder-1.0.4/src/shoulder/plotting.py
+-rw-r--r--   0        0        0     6681 2023-05-12 01:39:37.059210 shoulder-1.0.4/src/shoulder/utils.py
+-rw-r--r--   0        0        0     2877 1970-01-01 00:00:00.000000 shoulder-1.0.4/PKG-INFO
```

### Comparing `shoulder-1.0.3/LICENSE.md` & `shoulder-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.3/README.md` & `shoulder-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.3/pyproject.toml` & `shoulder-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "shoulder"
-version = "1.0.3"
+version = "1.0.4"
 description = "patient specific anatomic coordinate system generation for shoulder bones"
 authors = ["Gregory W Spangenberg <gspangen@westerneng.ca>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gregspangenberg/shoulder"
 
 [tool.poetry.dependencies]
-python = ">=3.10, <3.11"
+python = ">=3.10, <3.12"
 trimesh = "^3.14.1"
 scipy = "^1.9.1"
 networkx = "^2.8.6"
 Shapely = "^1.8.4"
 Rtree = "^1.0.0"
 plotly = "^5.10.0"
 scikit-spatial = "^6.5.0"
```

### Comparing `shoulder-1.0.3/src/shoulder/base.py` & `shoulder-1.0.4/src/shoulder/base.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.3/src/shoulder/bone.py` & `shoulder-1.0.4/src/shoulder/bone.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,16 @@
 class Humerus(Bone):
     def __init__(self, stl_file):
         self.stl_file = stl_file
         self.transform = np.identity(4)
         msh = mesh.FullObb(stl_file)
 
         self.canal = canal.Canal(msh)
-        self.trans_epiconylar = epicondyle.TransEpicondylar(msh, self.canal)
-        self.anatomic_neck = anatomic_neck.AnatomicNeck(
-            msh, self.canal, self.trans_epiconylar
-        )
+        self.trans_epiconylar = epicondyle.TransEpicondylar(msh)
+        self.anatomic_neck = anatomic_neck.AnatomicNeck(msh, self.trans_epiconylar)
         self.bicipital_groove = bicipital_groove.DeepGroove(msh)
 
     def apply_csys_canal_transepiconylar(self) -> np.ndarray:
         self.transform = construct_csys(self.canal._axis, self.trans_epiconylar._axis)
         self._update_landmark_data(self.transform)
         return self.transform
```

### Comparing `shoulder-1.0.3/src/shoulder/humerus/anatomic_neck.py` & `shoulder-1.0.4/src/shoulder/humerus/anatomic_neck.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,84 +13,84 @@
 from scipy.spatial import KDTree
 from itertools import islice, cycle
 import sklearn.cluster
 import trimesh
 
 
 class AnatomicNeck(Landmark):
-    def __init__(
-        self, obb: mesh.Obb, canal: canal.Canal, transepi: epicondyle.TransEpicondylar
-    ):
+    def __init__(self, obb: mesh.Obb, transepi: epicondyle.TransEpicondylar):
         self._mesh_oriented = obb.mesh
         self._transform = obb.transform
         self._transepi = transepi
         self._axis_ct = None
         self._axis = None
         self._points_ct = None
         self._points = None
         self._control_points_ct = None
         self._control_points = None
 
     @property
-    def transepi_axis(self):
+    def _transepi_axis(self):
         return self._transepi._axis_ct
 
     # needs implimentation
     def plane(self):
         if self._axis is None:
             circle_threshold = 0.3
             sup_inf_num = 16
             med_lat_num = 8
 
-            articular_pt, hc_mnr_axis, medial_epicondyle_pt = self.seed(
+            articular_pt, hc_mnr_axis, medial_epicondyle_pt = self.__seed(
                 self._mesh_oriented,
                 50,
                 utils.transform_pts(self.transepi_axis, self._transform),
             )
             # Slice along the head central minor axis
             # find which endpoint of hc_mnr_axis is closer to the medial_epicondyle_pt,
             # that side contins the greater tuberosity
             gt_side_pt, non_gt_side_pt = utils.closest_pt(
                 medial_epicondyle_pt[:, :-1], hc_mnr_axis[:, :-1], return_other_pts=True
             )  # z removed from inputs
             gt_side_pt = np.c_[gt_side_pt, hc_mnr_axis[0, -1]]  # add z back in
             non_gt_side_pt = np.c_[non_gt_side_pt, hc_mnr_axis[0, -1]]
 
-            hc_mnr_line, hc_mnr_length = self._midpoint_line(gt_side_pt, non_gt_side_pt)
+            hc_mnr_line, hc_mnr_length = self.__midpoint_line(
+                gt_side_pt, non_gt_side_pt
+            )
             # generate points along the middle 1/3 of the axis
             hc_mnr_axis_cut_locs = np.linspace(
                 hc_mnr_line.to_point(t=-hc_mnr_length / 6),  # - away from GT
                 hc_mnr_line.to_point(t=hc_mnr_length / 12),  # towards GT
                 sup_inf_num,
             )  # loc of cuts, which way is positive and which is negative, i am unsure
             # find endpoints of where circle stops on each slice
             seed_pt = articular_pt.copy()
             seed_pt[:, -1] += (
                 hc_mnr_length / 6
             )  # add extra z-height to offset the low z starting seed
-            hc_mnr_end_pts = self._rolling_circle_slices(
+            hc_mnr_end_pts = self.__rolling_circle_slices(
                 self._mesh_oriented,
                 seed_pt,
                 hc_mnr_axis_cut_locs,
                 hc_mnr_line.direction,
                 circle_threshold,
             )
             # seperate into distal and proximal pts, and return filtered end points
-            inf_pts, sup_pts = self._inf_sup_articular(hc_mnr_end_pts, hc_mnr_axis)
+            inf_pts, sup_pts = self.__inf_sup_articular(hc_mnr_end_pts, hc_mnr_axis)
 
             # slice along a line between the mean of inferior and superior endpoints
             inf_mean = np.mean(inf_pts, axis=0).reshape(-1, 3)
             sup_mean = np.mean(sup_pts, axis=0).reshape(-1, 3)
-            inf_sup_line, inf_sup_len = self._midpoint_line(inf_mean, sup_mean)
+            inf_sup_line, inf_sup_len = self.__midpoint_line(inf_mean, sup_mean)
             inf_sup_cut_locs = np.linspace(
                 inf_sup_line.to_point(t=-inf_sup_len / 6),
                 inf_sup_line.to_point(t=inf_sup_len / 6),
                 med_lat_num,
             )
-            med_lat_pts = self._rolling_circle_slices(
+            med_lat_pts = self.__rolling_circle_slices(
                 self._mesh_oriented,
                 seed_pt,
                 inf_sup_cut_locs,
                 inf_sup_line.direction,
                 circle_threshold,
             )
             # med_pts, lat_pts = med_lat_articular(med_lat_pts, inf_pts, sup_pts)
@@ -160,15 +160,15 @@
                     mode="markers",
                     name="Anatomic Neck Plane Control Points",
                 ),
             ]
 
             return plot
 
-    def seed(self, mesh, slice_num, transepi):
+    def __seed(self, mesh, slice_num, transepi):
         # transepi must be  in same csys as mesh
 
         def head_direction(polygon, hc_maj_axis_pts):
             """finds which pt of the head central axis corresponds to the aritcular surface
             and returns the row the point is in the array
             """
             bound = polygon.minimum_rotated_rectangle
@@ -254,15 +254,15 @@
         medial_epicondyle = utils.closest_pt(
             articular_pt[:, :-1], transepi[:, :-1]  # removed z from inputs
         )
         medial_epicondyle = np.c_[medial_epicondyle, transepi[0, -1]]  # add z back in
 
         return seed, min_axis_pts, medial_epicondyle
 
-    def _rolling_circle_fit(self, pts, seed_pt, threshold):
+    def __rolling_circle_fit(self, pts, seed_pt, threshold):
         # find which point is closest to seed point (articular_point)
         kdtree = KDTree(pts)
         d, i = kdtree.query(
             seed_pt
         )  # returns distance and loction in index of closest point
 
         r_pts = np.roll(
@@ -320,26 +320,26 @@
                             len(fit_pts) - 1,
                         ]  # location in array of final stop points for each direction
                         break
         fit_pts = np.vstack(fit_pts)  # convert list of (1,3) to array of (n,3)
 
         return fit_pts[skip_i]
 
-    def _midpoint_line(self, pt0, pt1):
+    def __midpoint_line(self, pt0, pt1):
         pt0 = pt0.flatten()
         pt1 = pt1.flatten()
         midpoint = np.mean(np.vstack([pt0, pt1]), axis=0)
         dir = skspatial.objects.Line.from_points(pt0, pt1).direction
         length = skspatial.objects.Point(pt0).distance_point(pt1)
         dir = dir / length  # create unit vector
         midpoint_line = skspatial.objects.Line(midpoint, dir)
 
         return midpoint_line, length
 
-    def _rolling_circle_slices(self, mesh, seed_pt, locs, dir, thresh):
+    def __rolling_circle_slices(self, mesh, seed_pt, locs, dir, thresh):
         def multislice(mesh, cut_increments, normal):
             for cut in cut_increments:
                 try:
                     path = mesh.section(plane_origin=cut, plane_normal=normal)
                     slice, to_3d = path.to_planar(normal=normal)
 
                     if len(slice.polygons_closed) > 1:  # if more than 1 poly
@@ -375,23 +375,23 @@
             pts = np.asarray(polygon.exterior.xy).T  # extract points [nx3] matrix
             seed_pt_alt = utils.transform_pts(
                 seed_pt, utils.inv_transform(to_3d)
             )  # project into plane space
             seed_pt_alt = seed_pt_alt[:, :-1]  # remove out of plane direction for now
 
             # find circular portion of trace with rolling least squares circle
-            circle_end_pts = self._rolling_circle_fit(pts, seed_pt_alt, thresh)
+            circle_end_pts = self.__rolling_circle_fit(pts, seed_pt_alt, thresh)
             circle_end_pts = utils.z_zero_col(circle_end_pts)
 
             circle_end_pts = utils.transform_pts(circle_end_pts, to_3d)
             end_pts.append(circle_end_pts)
 
         return np.vstack(end_pts)
 
-    def _distal_proximal_zs_articular(self, end_pts):
+    def __distal_proximal_zs_articular(self, end_pts):
         # the end points alternate back and forth so seperate them out
         _, labels, _ = sklearn.cluster.k_means(end_pts, 2)
         pts0 = end_pts[np.where(labels == 0)]
         pts1 = end_pts[np.where(labels == 1)]
 
         # filter out nonsense at weird z elevations, now that they have both been seperated
         pts0 = utils.z_score_filter(pts0, -1, 2)
@@ -408,15 +408,15 @@
             distal_z = pts1_mean
         else:
             proximal_z = pts1_mean
             distal_z = pts0_mean
 
         return filt_pts, distal_z, proximal_z
 
-    def _inf_sup_articular(self, end_pts, minor_axis):
+    def __inf_sup_articular(self, end_pts, minor_axis):
         # the end points alternate back and forth so seperate them out
         _, labels, _ = sklearn.cluster.k_means(end_pts, 2)
         pts0 = end_pts[np.where(labels == 0)]
         pts1 = end_pts[np.where(labels == 1)]
 
         # filter out nonsense at weird z elevations, now that they have both been seperated
         pts0 = utils.z_score_filter(pts0, -1, 2)
```

### Comparing `shoulder-1.0.3/src/shoulder/humerus/angles.py` & `shoulder-1.0.4/src/shoulder/humerus/angles.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.3/src/shoulder/humerus/bicipital_groove.py` & `shoulder-1.0.4/src/shoulder/humerus/bicipital_groove.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,165 +2,141 @@
 from shoulder.base import Landmark
 
 
 import numpy as np
 import scipy.signal
 import skspatial.objects
 import plotly.graph_objects as go
+import matplotlib.pyplot as plt
 
 
 class DeepGroove(Landmark):
     def __init__(self, obb):
         self._mesh_oriented_uobb = obb.mesh
         self._transform_uobb = obb.transform
         self._points_ct = None
         self._points = None
         self._axis_ct = None
         self._axis = None
 
-    def axis(self, slice_num=35, interp_num=250):
+    def axis(self, cutoff_pcts=[0.75, 0.92], slice_num=35, interp_num=250):
         if self._axis is None:
             # slice_num  must use odd soo add 1 if even
             if (slice_num % 2) == 0:
                 slice_num += 1
 
+            # find z interval to calculate bicipital groove upon
+            cutoff_pcts.sort()
             z_max = np.max(self._mesh_oriented_uobb.bounds[:, -1])
-            zs = np.linspace(0.92 * z_max, 0.75 * z_max, num=slice_num).flatten()
+            zs = np.linspace(
+                cutoff_pcts[1] * z_max, cutoff_pcts[0] * z_max, num=slice_num
+            ).flatten()
 
-            pts = np.zeros((interp_num, 2, slice_num))
-            pts_r = np.zeros((interp_num, 2, slice_num))
-            pts_r_sp = np.zeros((interp_num, 2, slice_num))
+            xy = np.zeros((interp_num, 2, slice_num))
+            polar = np.zeros((interp_num, 2, slice_num))
             weights = np.zeros((interp_num, 2, slice_num))
             to_3Ds = np.zeros((4, 4, slice_num))
 
             for i, z in enumerate(zs):
+                # grab the polygon of the slice
                 origin = [0, 0, z]
                 normal = [0, 0, 1]
                 path = self._mesh_oriented_uobb.section(
                     plane_origin=origin, plane_normal=normal
                 )
-
                 slice, to_3D = path.to_planar(normal=normal)
+                # keep only largest polygon
                 big_poly = slice.polygons_closed[
                     np.argmax([p.area for p in slice.polygons_closed])
                 ]
 
                 # resample cartesion coordinates to create evenly spaced points
                 _pts = np.asarray(big_poly.exterior.xy).T
                 _pts = _resample_polygon(_pts, interp_num)
 
-                pol = _cart2pol(_pts)
-
-                f = scipy.interpolate.interp1d(pol[:, 0], pol[:, 1])
-                theta_spaced = np.linspace(
-                    np.min(pol[:, 0]), np.max(pol[:, 0]), (interp_num)
-                ).flatten()
-                r_spaced = f(theta_spaced)
-
-                pol_spaced = np.c_[theta_spaced, r_spaced]
-
-                xy = _pol2cart(pol_spaced)
+                # convert to polar and ensure even degree spacing
+                _pol = _cart2pol(_pts)
 
                 # if a cavity is present do not count that as a weight
                 theta_diff = (
-                    np.diff(pol[:, 0], prepend=-10) < 0
+                    np.diff(_pol[:, 0], prepend=-10) < 0
                 )  # prepend -10 so first difference is positive
                 cav = _true_propogate(theta_diff)  # all cavities are True
                 cav = np.array(cav, dtype=np.int32)  # make all true 1
                 cav = cav ^ (
                     cav & 1 == cav
                 )  # flip all 0s to 1s, since we want to preserve everythin but cavities
                 cav_weight = np.c_[cav, cav]
 
                 # log data
-                pts[:, :, i] = xy
-                pts_r[:, :, i] = pol
-                pts_r_sp[:, :, i] = pol_spaced
+                xy[:, :, i] = _pts
+                polar[:, :, i] = _pol
                 weights[:, :, i] = cav_weight
                 to_3Ds[:, :, i] = to_3D
 
             # make each radial slice stationary
-            pts_r_0 = pts_r.copy()
-            pts_r_0[:, 1, :] = np.apply_along_axis(
-                lambda x: x - np.mean(x), axis=0, arr=pts_r[:, 1, :]
+            polar_0 = polar.copy()
+            polar_0[:, 1, :] = np.apply_along_axis(
+                lambda x: x - np.mean(x), axis=0, arr=polar[:, 1, :]
             )
 
-            # calulcate mean across each slice
-            mean_pts_r_0 = np.mean(pts_r_0, axis=2)
-            deg = np.rad2deg(mean_pts_r_0[:, 0])
-            radius = mean_pts_r_0[:, 1]
-            # calculate weighted mean that has cavity weight as 0
-            w_mean_pts_r_0 = np.average(pts_r_0, axis=2, weights=weights)
-            deg_w = np.rad2deg(w_mean_pts_r_0[:, 0])
-            radius_w = w_mean_pts_r_0[:, 1]
-            radius_w = scipy.signal.savgol_filter(
-                radius_w, 10, 1
-            )  # weights create jagged edges
+            # calculate weighted mean across slices where cavities have a weight of 0
+            polar_avg_0 = np.average(polar_0, axis=2, weights=weights)
+            deg = np.rad2deg(polar_avg_0[:, 0])
+            radius = polar_avg_0[:, 1]
+            # weights create jagged edges
+            radius = scipy.signal.savgol_filter(radius, 10, 1)
 
             # calulate derivatives
             dd_radius = _derivative_smooth_ends(radius, 2, 10, 2)
-            dd_radius_w = _derivative_smooth_ends(radius_w, 2, 10, 2)
 
-            # find peaks in derivative, and keep 3 largest
-            m_peaks, m_peaks_prop = scipy.signal.find_peaks(
+            peaks, _prop = scipy.signal.find_peaks(
                 dd_radius, height=0, distance=interp_num / 360 * 25
             )
-            m_peaks = m_peaks[np.argpartition(m_peaks_prop["peak_heights"], -3)[-3:]]
-            wm_peaks, wm_peaks_prop = scipy.signal.find_peaks(
-                dd_radius_w, height=0, distance=interp_num / 360 * 25
-            )
-            wm_peaks = wm_peaks[
-                np.argpartition(wm_peaks_prop["peak_heights"], -3)[-3:]
+            peaks = peaks[
+                np.argpartition(_prop["peak_heights"], -3)[-3:]
             ]  # top 3 largest
 
             # find the peaks that are not near the furthest point
             # the furthest point is on the articular surface so any peaks neighbouring there
             # would not be the biciptal groove
-            deg_far = deg_w[np.argmax(radius_w)]
-            wm_peaks = sorted(wm_peaks)
-            deg_w_peaks = deg_w[wm_peaks]
-            filt_vals = np.r_[deg_w_peaks, deg_far]
-            deg_w_shft = np.r_[
-                deg_w[wm_peaks[0] :], deg_w[: wm_peaks[0]], deg_w[wm_peaks[0]]
-            ]
-            filt = [x for x in deg_w_shft if x in filt_vals]
+            peaks.sort()
+            deg_rmax = deg[np.argmax(radius)]
+            deg_peaks = deg[peaks]
+            filt_vals = np.r_[deg_peaks, deg_rmax]
+            deg_shft = np.r_[deg[peaks[0] :], deg[: peaks[0]], deg[peaks[0]]]
+            filt = [x for x in deg_shft if x in filt_vals]
             non_bg_peaks = (
-                filt[filt.index(deg_far) - 1],
-                filt[filt.index(deg_far) + 1],
+                filt[filt.index(deg_rmax) - 1],
+                filt[filt.index(deg_rmax) + 1],
             )
-            bg_peak = list(set(deg_w_peaks) - set(non_bg_peaks))[0]
-
-            # print(bg_peak)
+            bg_peak = list(set(deg_peaks) - set(non_bg_peaks))[0]
 
             # get local minima by specifying serach window for
             # search up to 15 degrees away on each side
-            deg_idx_var = int(round(360 / interp_num) * 15)
-            bg_locals = np.zeros((1, 2, len(zs)))
-            bg_xy = np.zeros((1, 2, len(zs)))
+            deg_variance = int(round(360 / interp_num) * 15)
             bg_xyz = np.zeros((1, 3, len(zs)))
             for i, z in enumerate(zs):
                 bg_idx_near = _find_nearest_idx(
-                    pts_r_0[:, 0, i].flatten(), np.deg2rad(bg_peak)
+                    polar_0[:, 0, i].flatten(), np.deg2rad(bg_peak)
                 )
-                bg_range = pts_r_0[
-                    (bg_idx_near - deg_idx_var) : (bg_idx_near + deg_idx_var), :, i
+                bg_range = polar_0[
+                    (bg_idx_near - deg_variance) : (bg_idx_near + deg_variance), :, i
                 ]
                 bg_local_i = np.argmin(bg_range[:, 1])
-                bg_local = bg_range[bg_local_i, :]
-                bg_locals[:, :, i] = bg_local
+
                 # transform back to radial coordinates
-                bg_i = bg_local_i + bg_idx_near - deg_idx_var  # put back in context
-                _bg_xy = _pol2cart(pts_r[bg_i, :, i].reshape(1, 2))
-                bg_xy[:, :, i] = _bg_xy
+                bg_i = bg_local_i + (bg_idx_near - deg_variance)  # put back in context
+                _bg_xy = _pol2cart(polar[bg_i, :, i].reshape(1, 2))
 
                 # i think to_3D is perhaps fully broken, doesn't seem to work
                 bg_xyz[:, :, i] = utils.transform_pts(np.c_[_bg_xy, 0], to_3Ds[:, :, i])
 
             bg_xyz = bg_xyz.transpose(2, 1, 0).reshape(-1, 3)
-            print(bg_xyz.shape)
+
             # transform back
             bg_xyz = utils.transform_pts(
                 bg_xyz, utils.inv_transform(self._transform_uobb)
             )
 
             # construct an estimate of the bicipital groove axis from the bg_xyz pts
             line_ends = _fit_line(bg_xyz)
```

### Comparing `shoulder-1.0.3/src/shoulder/humerus/canal.py` & `shoulder-1.0.4/src/shoulder/humerus/canal.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.3/src/shoulder/humerus/epicondyle.py` & `shoulder-1.0.4/src/shoulder/humerus/epicondyle.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import plotly.graph_objects as go
 import shapely
 import numpy as np
 import itertools
 
 
 class TransEpicondylar(Landmark):
-    def __init__(self, obb: mesh.FullObb, canal: canal.Canal):
+    def __init__(self, obb: mesh.FullObb):
         self._mesh_oriented = obb.mesh
         self._transform = obb.transform
         self._axis_ct = None
         self._axis = None
 
     def axis(self, num_slices: int = 50):
         def medial_lateral_dist_multislice(msh_o, num_slices: int):
```

### Comparing `shoulder-1.0.3/src/shoulder/humerus/mesh.py` & `shoulder-1.0.4/src/shoulder/humerus/mesh.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.3/src/shoulder/plotting.py` & `shoulder-1.0.4/src/shoulder/plotting.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.3/src/shoulder/utils.py` & `shoulder-1.0.4/src/shoulder/utils.py`

 * *Files identical despite different names*

### Comparing `shoulder-1.0.3/PKG-INFO` & `shoulder-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: shoulder
-Version: 1.0.3
+Version: 1.0.4
 Summary: patient specific anatomic coordinate system generation for shoulder bones
 Home-page: https://github.com/gregspangenberg/shoulder
 License: MIT
 Author: Gregory W Spangenberg
 Author-email: gspangen@westerneng.ca
-Requires-Python: >=3.10,<3.11
+Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Rtree (>=1.0.0,<2.0.0)
 Requires-Dist: Shapely (>=1.8.4,<2.0.0)
 Requires-Dist: circle-fit (>=0.1.3,<0.2.0)
 Requires-Dist: networkx (>=2.8.6,<3.0.0)
 Requires-Dist: numpy-stl (>=2.17.1,<3.0.0)
 Requires-Dist: pandas (>=1.4.4,<2.0.0)
 Requires-Dist: plotly (>=5.10.0,<6.0.0)
```


# Comparing `tmp/Pulse3D-0.33.3.tar.gz` & `tmp/Pulse3D-0.33.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pulse3D-0.33.3.tar", last modified: Mon May  8 21:56:35 2023, max compression
+gzip compressed data, was "Pulse3D-0.33.4.tar", last modified: Thu May 11 22:58:29 2023, max compression
```

## Comparing `Pulse3D-0.33.3.tar` & `Pulse3D-0.33.4.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:56:35.911337 Pulse3D-0.33.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-08 21:56:35.911337 Pulse3D-0.33.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:56:35.907337 Pulse3D-0.33.3/mantarray-magnet-finding/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-08 21:55:17.000000 Pulse3D-0.33.3/mantarray-magnet-finding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:56:35.907337 Pulse3D-0.33.3/mantarray-magnet-finding/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:56:35.911337 Pulse3D-0.33.3/mantarray-magnet-finding/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-08 21:55:17.000000 Pulse3D-0.33.3/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-08 21:55:17.000000 Pulse3D-0.33.3/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-05-08 21:55:17.000000 Pulse3D-0.33.3/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-08 21:55:17.000000 Pulse3D-0.33.3/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-08 21:56:35.915337 Pulse3D-0.33.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:56:35.907337 Pulse3D-0.33.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:56:35.911337 Pulse3D-0.33.3/src/Pulse3D.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-08 21:56:35.000000 Pulse3D-0.33.3/src/Pulse3D.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-08 21:56:35.000000 Pulse3D-0.33.3/src/Pulse3D.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 21:56:18.000000 Pulse3D-0.33.3/src/Pulse3D.egg-info/not-zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:56:35.911337 Pulse3D-0.33.3/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-08 21:55:52.000000 Pulse3D-0.33.3/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-08 21:55:52.000000 Pulse3D-0.33.3/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-05-08 21:55:52.000000 Pulse3D-0.33.3/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-08 21:55:52.000000 Pulse3D-0.33.3/src/mantarray_magnet_finding/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:56:35.911337 Pulse3D-0.33.3/src/pulse3D/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/compression_cy.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    18124 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    46415 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    34854 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/nb_peak_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/peak_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    33482 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/plate_recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/stimulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:58:29.858380 Pulse3D-0.33.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-11 22:58:29.858380 Pulse3D-0.33.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:58:29.854380 Pulse3D-0.33.4/mantarray-magnet-finding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-11 22:57:22.000000 Pulse3D-0.33.4/mantarray-magnet-finding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:58:29.854380 Pulse3D-0.33.4/mantarray-magnet-finding/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:58:29.854380 Pulse3D-0.33.4/mantarray-magnet-finding/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 22:57:22.000000 Pulse3D-0.33.4/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-11 22:57:22.000000 Pulse3D-0.33.4/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-11 22:57:22.000000 Pulse3D-0.33.4/mantarray-magnet-finding/src/mantarray_magnet_finding/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-05-11 22:57:22.000000 Pulse3D-0.33.4/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-11 22:57:22.000000 Pulse3D-0.33.4/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-11 22:58:29.858380 Pulse3D-0.33.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:58:29.854380 Pulse3D-0.33.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:58:29.854380 Pulse3D-0.33.4/src/Pulse3D.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-11 22:58:29.000000 Pulse3D-0.33.4/src/Pulse3D.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-11 22:58:29.000000 Pulse3D-0.33.4/src/Pulse3D.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 22:58:14.000000 Pulse3D-0.33.4/src/Pulse3D.egg-info/not-zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:58:29.854380 Pulse3D-0.33.4/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 22:57:52.000000 Pulse3D-0.33.4/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-11 22:57:52.000000 Pulse3D-0.33.4/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-11 22:57:52.000000 Pulse3D-0.33.4/src/mantarray_magnet_finding/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-05-11 22:57:52.000000 Pulse3D-0.33.4/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-11 22:57:52.000000 Pulse3D-0.33.4/src/mantarray_magnet_finding/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:58:29.854380 Pulse3D-0.33.4/src/pulse3D/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/compression_cy.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    18124 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46466 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34854 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/nb_peak_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/peak_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33716 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/plate_recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/stimulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-11 22:57:19.000000 Pulse3D-0.33.4/src/pulse3D/utils.py
```

### Comparing `Pulse3D-0.33.3/LICENSE` & `Pulse3D-0.33.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.3/PKG-INFO` & `Pulse3D-0.33.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.33.3
+Version: 0.33.4
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
```

### Comparing `Pulse3D-0.33.3/mantarray-magnet-finding/setup.py` & `Pulse3D-0.33.4/mantarray-magnet-finding/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """Setup configuration."""
 from setuptools import find_packages
 from setuptools import setup
 
 
 setup(
     name="mantarray_magnet_finding",
-    version="0.5.0",
+    version="0.5.1",
     description="Magnet Finding",
     url="https://github.com/CuriBio/mantarray-magnet-finding",
     author="Curi Bio",
     author_email="contact@curibio.com",
     license="MIT",
     packages=find_packages("src"),
     package_dir={"": "src"},
```

### Comparing `Pulse3D-0.33.3/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.33.4/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from .constants import GUESS_INCR
 from .constants import NUM_ACTIVE_WELLS
 from .constants import NUM_AXES
 from .constants import NUM_CHANNELS
 from .constants import NUM_SENSORS
 from .constants import WELLS_PER_COL
+from .exceptions import UnableToConvergeError
 
 ADJACENT_WELL_DISTANCE_MM = 19.5
 
 # machine epsilon for float64, calibrated for 2-point derivative calculation
 EPS_ADJ = np.finfo(np.float64).eps ** 0.5
 
 DEFAULT_INITIAL_GUESS_VALUES = immutabledict(
@@ -132,17 +133,15 @@
                     np.arange(0, NUM_AXES * len(f1), 3) + axis, magnet + NUM_ACTIVE_WELLS * param_idx
                 ] = (np.transpose(f1 - f0) / DIPOLE_MODEL_FACTOR / dx0[magnet + param_idx * NUM_ACTIVE_WELLS])
     return jacobian
 
 
 @njit(fastmath=True)  # type: ignore
 def objective_function(
-    pos: NDArray[(1, Any), float],
-    b_meas: NDArray[(1, Any), float],
-    manta: NDArray[MANTA_SHAPE, float],
+    pos: NDArray[(1, Any), float], b_meas: NDArray[(1, Any), float], manta: NDArray[MANTA_SHAPE, float]
 ) -> NDArray[
     (Any,), float
 ]:  # pragma: no cover  # Tanner (1/9/22): codecov cannot cover functions compiled with numba
     """Cost function."""
     xpos, ypos, zpos, theta, phi, remn = pos.reshape(NUM_PARAMS, NUM_ACTIVE_WELLS)
 
     fields = np.zeros((NUM_SENSORS * NUM_ACTIVE_WELLS, NUM_AXES))
@@ -224,55 +223,60 @@
         [
             initial_guess_values["Y"] + ADJACENT_WELL_DISTANCE_MM * (well_idx % WELLS_PER_COL)
             for well_idx in active_wells
         ]
     )
     for param in list(initial_guess_values.keys())[2:]:
         prev_guess.extend([initial_guess_values[param]] * NUM_ACTIVE_WELLS)
+
     params = tuple(initial_guess_values.keys())
     estimations = {param: np.zeros((data.shape[-1], NUM_ACTIVE_WELLS)) for param in params}
 
     # Tanner (12/8/21): should probably add some sort of logging eventually
     # Kevin (12/1/21): Run the algorithm on each time index. The algorithm uses its previous outputs as its initial guess for all datapoints but the first one
-
-    for incr in range(
-        0, 10
-    ):  # change x position guess incrementally, uniformly for all wells until the algorithm converges properly
+    optimal_initial_guess_found = False
+    # change x position guess incrementally, uniformly for all wells until the algorithm converges properly
+    for _ in range(0, 10):
         b_meas = data[:, 0]
+        # increment previous guess
         prev_guess = prev_guess + np.append(
             np.ones(NUM_ACTIVE_WELLS) * -GUESS_INCR, np.zeros((NUM_PARAMS - 1) * NUM_ACTIVE_WELLS)
-        )  # increment previous guess  # increment previous guess
+        )
 
         res = least_squares(
             objective_function,
             prev_guess,
             args=(b_meas, manta_xyz),
             method="lm",
             ftol=1e-1,
             verbose=0,
             jac=compute_jacobian,
         )
-        optimality = res.optimality
 
-        if optimality < 1e-5:
-            for data_idx in range(0, data.shape[-1]):
-                b_meas = data[:, data_idx]
-
-                res = least_squares(
-                    objective_function,
-                    prev_guess,
-                    args=(b_meas, manta_xyz),
-                    method="lm",
-                    ftol=1e-1,
-                    verbose=0,
-                    jac=compute_jacobian,
-                )
-
-                # Tanner (12/2/21): set the start of all subsequent loops as the estimation from the first loop
-                prev_guess = np.array(res.x)  # type: ignore
-
-                outputs = np.asarray(res.x).reshape(NUM_PARAMS, NUM_ACTIVE_WELLS)
-                for i, param in enumerate(params):
-                    estimations[param][data_idx, :] = outputs[i]
+        if optimal_initial_guess_found := res.optimality < 1e-5:
             break
 
+    # Luci (05/10/23) raise exception if no guess is found. Will be caught and displayed to user.
+    if not optimal_initial_guess_found:
+        raise UnableToConvergeError()
+
+    for data_idx in range(0, data.shape[-1]):
+        b_meas = data[:, data_idx]
+
+        res = least_squares(
+            objective_function,
+            prev_guess,
+            args=(b_meas, manta_xyz),
+            method="lm",
+            ftol=1e-1,
+            verbose=0,
+            jac=compute_jacobian,
+        )
+
+        # Tanner (12/2/21): set the start of all subsequent loops as the estimation from the first loop
+        prev_guess = np.array(res.x)  # type: ignore
+
+        outputs = np.asarray(res.x).reshape(NUM_PARAMS, NUM_ACTIVE_WELLS)
+        for i, param in enumerate(params):
+            estimations[param][data_idx, :] = outputs[i]
+
     return estimations
```

### Comparing `Pulse3D-0.33.3/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.33.4/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.3/setup.py` & `Pulse3D-0.33.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 extensions = [Extension("pulse3D.compression_cy", [os.path.join("src", "pulse3D", "compression_cy") + ext])]
 if USE_CYTHON:
     # cythonizing compression_cy.pyx with kwarg annotate=True will help when optimizing the code by enabling generation of the html annotation file
     extensions = cythonize(extensions, annotate=False)
 
 setup(
     name="Pulse3D",
-    version="0.33.3",
+    version="0.33.4",
     description="Pulse3D Analysis Platform",
     url="https://github.com/CuriBio/Pulse3D",
     project_urls={"Documentation": "https://pulse3D.readthedocs.io/en/latest/"},
     author="Curi Bio",
     author_email="contact@curibio.com",
     license="MIT",
     package_dir={"": "src"},
```

### Comparing `Pulse3D-0.33.3/src/Pulse3D.egg-info/PKG-INFO` & `Pulse3D-0.33.4/src/Pulse3D.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.33.3
+Version: 0.33.4
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
```

### Comparing `Pulse3D-0.33.3/src/Pulse3D.egg-info/SOURCES.txt` & `Pulse3D-0.33.4/src/Pulse3D.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 LICENSE
 setup.cfg
 setup.py
 mantarray-magnet-finding/setup.py
 mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
 mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
+mantarray-magnet-finding/src/mantarray_magnet_finding/exceptions.py
 mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
 mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
 src/Pulse3D.egg-info/PKG-INFO
 src/Pulse3D.egg-info/not-zip-safe
 src/mantarray_magnet_finding/__init__.py
 src/mantarray_magnet_finding/constants.py
+src/mantarray_magnet_finding/exceptions.py
 src/mantarray_magnet_finding/magnet_finding.py
 src/mantarray_magnet_finding/utils.py
 src/pulse3D/__init__.py
 src/pulse3D/compression_cy.pyx
 src/pulse3D/constants.py
 src/pulse3D/excel_writer.py
 src/pulse3D/exceptions.py
```

### Comparing `Pulse3D-0.33.3/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.33.4/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from .constants import GUESS_INCR
 from .constants import NUM_ACTIVE_WELLS
 from .constants import NUM_AXES
 from .constants import NUM_CHANNELS
 from .constants import NUM_SENSORS
 from .constants import WELLS_PER_COL
+from .exceptions import UnableToConvergeError
 
 ADJACENT_WELL_DISTANCE_MM = 19.5
 
 # machine epsilon for float64, calibrated for 2-point derivative calculation
 EPS_ADJ = np.finfo(np.float64).eps ** 0.5
 
 DEFAULT_INITIAL_GUESS_VALUES = immutabledict(
@@ -132,17 +133,15 @@
                     np.arange(0, NUM_AXES * len(f1), 3) + axis, magnet + NUM_ACTIVE_WELLS * param_idx
                 ] = (np.transpose(f1 - f0) / DIPOLE_MODEL_FACTOR / dx0[magnet + param_idx * NUM_ACTIVE_WELLS])
     return jacobian
 
 
 @njit(fastmath=True)  # type: ignore
 def objective_function(
-    pos: NDArray[(1, Any), float],
-    b_meas: NDArray[(1, Any), float],
-    manta: NDArray[MANTA_SHAPE, float],
+    pos: NDArray[(1, Any), float], b_meas: NDArray[(1, Any), float], manta: NDArray[MANTA_SHAPE, float]
 ) -> NDArray[
     (Any,), float
 ]:  # pragma: no cover  # Tanner (1/9/22): codecov cannot cover functions compiled with numba
     """Cost function."""
     xpos, ypos, zpos, theta, phi, remn = pos.reshape(NUM_PARAMS, NUM_ACTIVE_WELLS)
 
     fields = np.zeros((NUM_SENSORS * NUM_ACTIVE_WELLS, NUM_AXES))
@@ -224,55 +223,60 @@
         [
             initial_guess_values["Y"] + ADJACENT_WELL_DISTANCE_MM * (well_idx % WELLS_PER_COL)
             for well_idx in active_wells
         ]
     )
     for param in list(initial_guess_values.keys())[2:]:
         prev_guess.extend([initial_guess_values[param]] * NUM_ACTIVE_WELLS)
+
     params = tuple(initial_guess_values.keys())
     estimations = {param: np.zeros((data.shape[-1], NUM_ACTIVE_WELLS)) for param in params}
 
     # Tanner (12/8/21): should probably add some sort of logging eventually
     # Kevin (12/1/21): Run the algorithm on each time index. The algorithm uses its previous outputs as its initial guess for all datapoints but the first one
-
-    for incr in range(
-        0, 10
-    ):  # change x position guess incrementally, uniformly for all wells until the algorithm converges properly
+    optimal_initial_guess_found = False
+    # change x position guess incrementally, uniformly for all wells until the algorithm converges properly
+    for _ in range(0, 10):
         b_meas = data[:, 0]
+        # increment previous guess
         prev_guess = prev_guess + np.append(
             np.ones(NUM_ACTIVE_WELLS) * -GUESS_INCR, np.zeros((NUM_PARAMS - 1) * NUM_ACTIVE_WELLS)
-        )  # increment previous guess  # increment previous guess
+        )
 
         res = least_squares(
             objective_function,
             prev_guess,
             args=(b_meas, manta_xyz),
             method="lm",
             ftol=1e-1,
             verbose=0,
             jac=compute_jacobian,
         )
-        optimality = res.optimality
 
-        if optimality < 1e-5:
-            for data_idx in range(0, data.shape[-1]):
-                b_meas = data[:, data_idx]
-
-                res = least_squares(
-                    objective_function,
-                    prev_guess,
-                    args=(b_meas, manta_xyz),
-                    method="lm",
-                    ftol=1e-1,
-                    verbose=0,
-                    jac=compute_jacobian,
-                )
-
-                # Tanner (12/2/21): set the start of all subsequent loops as the estimation from the first loop
-                prev_guess = np.array(res.x)  # type: ignore
-
-                outputs = np.asarray(res.x).reshape(NUM_PARAMS, NUM_ACTIVE_WELLS)
-                for i, param in enumerate(params):
-                    estimations[param][data_idx, :] = outputs[i]
+        if optimal_initial_guess_found := res.optimality < 1e-5:
             break
 
+    # Luci (05/10/23) raise exception if no guess is found. Will be caught and displayed to user.
+    if not optimal_initial_guess_found:
+        raise UnableToConvergeError()
+
+    for data_idx in range(0, data.shape[-1]):
+        b_meas = data[:, data_idx]
+
+        res = least_squares(
+            objective_function,
+            prev_guess,
+            args=(b_meas, manta_xyz),
+            method="lm",
+            ftol=1e-1,
+            verbose=0,
+            jac=compute_jacobian,
+        )
+
+        # Tanner (12/2/21): set the start of all subsequent loops as the estimation from the first loop
+        prev_guess = np.array(res.x)  # type: ignore
+
+        outputs = np.asarray(res.x).reshape(NUM_PARAMS, NUM_ACTIVE_WELLS)
+        for i, param in enumerate(params):
+            estimations[param][data_idx, :] = outputs[i]
+
     return estimations
```

### Comparing `Pulse3D-0.33.3/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.33.4/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.3/src/pulse3D/compression_cy.pyx` & `Pulse3D-0.33.4/src/pulse3D/compression_cy.pyx`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.3/src/pulse3D/constants.py` & `Pulse3D-0.33.4/src/pulse3D/constants.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.3/src/pulse3D/excel_writer.py` & `Pulse3D-0.33.4/src/pulse3D/excel_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,14 +96,15 @@
         "values": f"='continuous-waveforms'!${stim_session_col}$2:${stim_session_col}${upper_x_bound_cell}",
         "line": {"color": "#d1d128"},
     }
     y_axis_params: Dict[str, Any] = {"name": f"Stimulator Output ({charge_unit})", **y_axis_bounds}
 
     if format == "overlayed":
         series_params["y2_axis"] = 1
+        series_params["line"]["transparency"] = 70
     else:
         y_axis_params["major_gridlines"] = {"visible": 0}
 
     for chart in charts:
         chart.add_series(series_params)
         (chart.set_y2_axis if format == "overlayed" else chart.set_y_axis)(y_axis_params)
         chart.show_blanks_as("span")
```

### Comparing `Pulse3D-0.33.3/src/pulse3D/exceptions.py` & `Pulse3D-0.33.4/src/pulse3D/exceptions.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.3/src/pulse3D/magnet_finding.py` & `Pulse3D-0.33.4/src/pulse3D/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.3/src/pulse3D/metrics.py` & `Pulse3D-0.33.4/src/pulse3D/metrics.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.3/src/pulse3D/nb_peak_detection.py` & `Pulse3D-0.33.4/src/pulse3D/nb_peak_detection.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.3/src/pulse3D/peak_detection.py` & `Pulse3D-0.33.4/src/pulse3D/peak_detection.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.3/src/pulse3D/plate_recording.py` & `Pulse3D-0.33.4/src/pulse3D/plate_recording.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from typing import List
 from typing import Optional
 from typing import Union
 import uuid
 import zipfile
 
 import h5py
+from mantarray_magnet_finding.exceptions import UnableToConvergeError
 from mantarray_magnet_finding.utils import calculate_magnetic_flux_density_from_memsic
 from nptyping import NDArray
 import numpy as np
 from openpyxl import load_workbook
 from openpyxl.worksheet.worksheet import Worksheet
 import pandas as pd
 from scipy import interpolate
@@ -436,19 +437,23 @@
         # load 'calibration' data
         baseline_data = format_well_file_data(calibration_recordings)
         baseline_data_mt = calculate_magnetic_flux_density_from_memsic(baseline_data)
 
         # create baseline data array
         baseline_data_mt = np.mean(baseline_data_mt[:, -BASELINE_MEAN_NUM_DATA_POINTS:], axis=1)
 
-        # pass data into magnet finding alg
-        log.info("Estimating magnet positions")
-        estimated_magnet_positions = find_magnet_positions(
-            plate_data_array_mt, baseline_data_mt, initial_magnet_finding_params
-        )
+        try:
+            # pass data into magnet finding alg
+            log.info("Estimating magnet positions")
+            estimated_magnet_positions = find_magnet_positions(
+                plate_data_array_mt, baseline_data_mt, initial_magnet_finding_params
+            )
+        except UnableToConvergeError:
+            log.exception("Unable to converge due to bad quality of data")
+            raise
 
         flip_data = self.wells[0].version >= VersionInfo.parse("1.1.0")
 
         # create displacement and force arrays for each WellFile
         log.info("Create diplacement and force data for each well")
         for well_idx, well_file in enumerate(self):
             x = estimated_magnet_positions["X"][:, well_idx]
```

### Comparing `Pulse3D-0.33.3/src/pulse3D/plotting.py` & `Pulse3D-0.33.4/src/pulse3D/plotting.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.3/src/pulse3D/stimulation.py` & `Pulse3D-0.33.4/src/pulse3D/stimulation.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.3/src/pulse3D/transforms.py` & `Pulse3D-0.33.4/src/pulse3D/transforms.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.3/src/pulse3D/utils.py` & `Pulse3D-0.33.4/src/pulse3D/utils.py`

 * *Files identical despite different names*


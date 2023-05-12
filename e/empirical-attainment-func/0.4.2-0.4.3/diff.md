# Comparing `tmp/empirical_attainment_func-0.4.2-py3-none-any.whl.zip` & `tmp/empirical_attainment_func-0.4.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 14146 bytes, number of entries: 9
--rw-rw-r--  2.0 unx      545 b- defN 23-May-11 23:37 eaf/__init__.py
+Zip file size: 14214 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx      545 b- defN 23-May-12 00:52 eaf/__init__.py
 -rw-rw-r--  2.0 unx     7680 b- defN 23-May-11 16:37 eaf/eaf.py
--rw-rw-r--  2.0 unx    22805 b- defN 23-May-11 23:37 eaf/plot_surface.py
+-rw-rw-r--  2.0 unx    23119 b- defN 23-May-12 00:51 eaf/plot_surface.py
 -rw-rw-r--  2.0 unx     7055 b- defN 23-May-11 16:29 eaf/utils.py
--rw-rw-r--  2.0 unx    10760 b- defN 23-May-11 23:41 empirical_attainment_func-0.4.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx      432 b- defN 23-May-11 23:41 empirical_attainment_func-0.4.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-11 23:41 empirical_attainment_func-0.4.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        4 b- defN 23-May-11 23:41 empirical_attainment_func-0.4.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      759 b- defN 23-May-11 23:41 empirical_attainment_func-0.4.2.dist-info/RECORD
-9 files, 50132 bytes uncompressed, 12830 bytes compressed:  74.4%
+-rw-rw-r--  2.0 unx    10760 b- defN 23-May-12 03:03 empirical_attainment_func-0.4.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      432 b- defN 23-May-12 03:03 empirical_attainment_func-0.4.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-12 03:03 empirical_attainment_func-0.4.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        4 b- defN 23-May-12 03:03 empirical_attainment_func-0.4.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      759 b- defN 23-May-12 03:03 empirical_attainment_func-0.4.3.dist-info/RECORD
+9 files, 50446 bytes uncompressed, 12898 bytes compressed:  74.4%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: eaf/plot_surface.py
 Comment: 
 
 Filename: eaf/utils.py
 Comment: 
 
-Filename: empirical_attainment_func-0.4.2.dist-info/LICENSE
+Filename: empirical_attainment_func-0.4.3.dist-info/LICENSE
 Comment: 
 
-Filename: empirical_attainment_func-0.4.2.dist-info/METADATA
+Filename: empirical_attainment_func-0.4.3.dist-info/METADATA
 Comment: 
 
-Filename: empirical_attainment_func-0.4.2.dist-info/WHEEL
+Filename: empirical_attainment_func-0.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: empirical_attainment_func-0.4.2.dist-info/top_level.txt
+Filename: empirical_attainment_func-0.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: empirical_attainment_func-0.4.2.dist-info/RECORD
+Filename: empirical_attainment_func-0.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## eaf/__init__.py

```diff
@@ -1,13 +1,13 @@
 from eaf.eaf import get_empirical_attainment_surface
 from eaf.plot_surface import EmpiricalAttainmentFuncPlot
 from eaf.utils import pareto_front_to_surface
 
 
-__version__ = "0.4.2"
+__version__ = "0.4.3"
 __copyright__ = "Copyright (C) 2023 Shuhei Watanabe"
 __licence__ = "Apache-2.0 License"
 __author__ = "Shuhei Watanabe"
 __author_email__ = "shuhei.watanabe.utokyo@gmail.com"
 __url__ = "https://github.com/nabenabe0928/empirical-attainment-func"
```

## eaf/plot_surface.py

```diff
@@ -453,14 +453,20 @@
         ref_point, _costs_array = self._transform_ref_point_and_costs_array(costs_array)
         (n_runs, n_observations, _) = _costs_array.shape
         hvs = np.zeros((n_runs, n_observations))
         for i in range(n_observations):
             hvs[:, i] = _compute_hypervolume2d(costs_array=_costs_array[:, : i + 1], ref_point=ref_point)
 
         if normalize:
+            if self._true_pareto_sols is None:
+                raise AttributeError(
+                    "true_pareto_sols is not provided at the instantiation, but it is required to "
+                    "call `plot_hypervolume2d_with_band` with normalize=True. Consider using normalize=False"
+                )
+
             max_hv = self._compute_true_pareto_surface_hypervolume2d()
             hvs /= max_hv
 
         T = np.arange(n_observations) + 1
         m, s = np.mean(hvs, axis=0), np.std(hvs, axis=0) / np.sqrt(n_observations)
 
         marker_kwargs, kwargs = _extract_marker_kwargs(**kwargs)
```

## Comparing `empirical_attainment_func-0.4.2.dist-info/LICENSE` & `empirical_attainment_func-0.4.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `empirical_attainment_func-0.4.2.dist-info/RECORD` & `empirical_attainment_func-0.4.3.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-eaf/__init__.py,sha256=kFmEJKMEfGcWe5dDdehEWuL30MqMABIisV7fCbyHmDU,545
+eaf/__init__.py,sha256=D-CViBk2remCyjg_OO8yRXG1QljTO7p2AyMV3Fkxbok,545
 eaf/eaf.py,sha256=emGAMIg8LpK9iGtr82of4wzmPC5VDNSH1Hy98R0ToPg,7680
-eaf/plot_surface.py,sha256=orWoG0kEY5zgoohb8vgLJYweOfVb7ZT5jUHkLMwtonk,22805
+eaf/plot_surface.py,sha256=najzyrwAx0R0hjA2TpGEtLSwd2DKhCw3zeGJ_8pfaW8,23119
 eaf/utils.py,sha256=Net_dWEFZQ60hiy48kem557HFGt_l1CDZv6n2RSGRz8,7055
-empirical_attainment_func-0.4.2.dist-info/LICENSE,sha256=ac88kY3zZoCX1A9T_SZaKlkrNbdqKqwlqOVSgpAb-yg,10760
-empirical_attainment_func-0.4.2.dist-info/METADATA,sha256=tZsQwDFQfvYMiZKqCPfaEkcz3I8c57Zc-05UdNhynIw,432
-empirical_attainment_func-0.4.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-empirical_attainment_func-0.4.2.dist-info/top_level.txt,sha256=RB8SxfRWdmUVxvWEHyO5JYAwhi_tMl6QkEd0MxPCR04,4
-empirical_attainment_func-0.4.2.dist-info/RECORD,,
+empirical_attainment_func-0.4.3.dist-info/LICENSE,sha256=ac88kY3zZoCX1A9T_SZaKlkrNbdqKqwlqOVSgpAb-yg,10760
+empirical_attainment_func-0.4.3.dist-info/METADATA,sha256=FFkTctHkSIYOELMkGsVE2SP5J5MV-q0hOrc8pk_sQNk,432
+empirical_attainment_func-0.4.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+empirical_attainment_func-0.4.3.dist-info/top_level.txt,sha256=RB8SxfRWdmUVxvWEHyO5JYAwhi_tMl6QkEd0MxPCR04,4
+empirical_attainment_func-0.4.3.dist-info/RECORD,,
```


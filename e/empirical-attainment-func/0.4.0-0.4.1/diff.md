# Comparing `tmp/empirical_attainment_func-0.4.0-py3-none-any.whl.zip` & `tmp/empirical_attainment_func-0.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 13804 bytes, number of entries: 9
--rw-rw-r--  2.0 unx      545 b- defN 23-May-11 16:44 eaf/__init__.py
+Zip file size: 14088 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx      545 b- defN 23-May-11 23:19 eaf/__init__.py
 -rw-rw-r--  2.0 unx     7680 b- defN 23-May-11 16:37 eaf/eaf.py
--rw-rw-r--  2.0 unx    19195 b- defN 23-May-11 16:41 eaf/plot_surface.py
+-rw-rw-r--  2.0 unx    21689 b- defN 23-May-11 23:18 eaf/plot_surface.py
 -rw-rw-r--  2.0 unx     7055 b- defN 23-May-11 16:29 eaf/utils.py
--rw-rw-r--  2.0 unx    10760 b- defN 23-May-11 16:45 empirical_attainment_func-0.4.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx      432 b- defN 23-May-11 16:45 empirical_attainment_func-0.4.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-11 16:45 empirical_attainment_func-0.4.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        4 b- defN 23-May-11 16:45 empirical_attainment_func-0.4.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      759 b- defN 23-May-11 16:45 empirical_attainment_func-0.4.0.dist-info/RECORD
-9 files, 46522 bytes uncompressed, 12488 bytes compressed:  73.2%
+-rw-rw-r--  2.0 unx    10760 b- defN 23-May-11 23:19 empirical_attainment_func-0.4.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      432 b- defN 23-May-11 23:19 empirical_attainment_func-0.4.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-11 23:19 empirical_attainment_func-0.4.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        4 b- defN 23-May-11 23:19 empirical_attainment_func-0.4.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      759 b- defN 23-May-11 23:19 empirical_attainment_func-0.4.1.dist-info/RECORD
+9 files, 49016 bytes uncompressed, 12772 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: eaf/plot_surface.py
 Comment: 
 
 Filename: eaf/utils.py
 Comment: 
 
-Filename: empirical_attainment_func-0.4.0.dist-info/LICENSE
+Filename: empirical_attainment_func-0.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: empirical_attainment_func-0.4.0.dist-info/METADATA
+Filename: empirical_attainment_func-0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: empirical_attainment_func-0.4.0.dist-info/WHEEL
+Filename: empirical_attainment_func-0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: empirical_attainment_func-0.4.0.dist-info/top_level.txt
+Filename: empirical_attainment_func-0.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: empirical_attainment_func-0.4.0.dist-info/RECORD
+Filename: empirical_attainment_func-0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## eaf/__init__.py

```diff
@@ -1,13 +1,13 @@
 from eaf.eaf import get_empirical_attainment_surface
 from eaf.plot_surface import EmpiricalAttainmentFuncPlot
 from eaf.utils import pareto_front_to_surface
 
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 __copyright__ = "Copyright (C) 2023 Shuhei Watanabe"
 __licence__ = "Apache-2.0 License"
 __author__ = "Shuhei Watanabe"
 __author_email__ = "shuhei.watanabe.utokyo@gmail.com"
 __url__ = "https://github.com/nabenabe0928/empirical-attainment-func"
```

## eaf/plot_surface.py

```diff
@@ -46,26 +46,28 @@
             For example, if you would like to plot the first objective in the log scale,
             you need to feed log_scale=[0].
             In principle, log_scale changes the minimum value of the axes
             from -np.inf to a small positive value.
         x_min, x_max, y_min, y_max (float):
             The lower/upper bounds for each objective if available.
             It is used to fix the value ranges of each objective in plots.
+        ref_point (Optional[np.ndarray]):
+            The reference point to be used for the visualization of hypervolume plots.
     """
 
     def __init__(
         self,
         true_pareto_sols: Optional[np.ndarray] = None,
         larger_is_better_objectives: Optional[List[int]] = None,
         log_scale: Optional[List[int]] = None,
         x_min: float = np.inf,
         x_max: float = -np.inf,
         y_min: float = np.inf,
         y_max: float = -np.inf,
-        ref_point: np.ndarray = None,
+        ref_point: Optional[np.ndarray] = None,
     ):
         self.step_dir = _step_direction(larger_is_better_objectives)
         self.larger_is_better_objectives = (
             larger_is_better_objectives if larger_is_better_objectives is not None else []
         )
         self._ref_point = ref_point.copy().astype(np.float64) if ref_point is not None else None
         self.log_scale = log_scale if log_scale is not None else []
@@ -122,19 +124,25 @@
         Args:
             ax (plt.Axes):
                 The subplots axes.
             surf (np.ndarray):
                 The vertices of the empirical attainment surface.
                 The shape must be (X.size, 2).
             color (str):
-                The color of the plot
+                The color of the plot.
             label (str):
                 The label of the plot.
+            linestyle (Optional[str]):
+                The linestyle of the plot.
+            marker (Optional[str]):
+                The marker of the plot.
+            transform (bool):
+                Whether automatically transforming based on (x_min, x_max) and (y_min, y_max).
             kwargs:
-                The kwargs for scatter.
+                The kwargs for ax.plot.
         """
         if len(surf.shape) != 2 or surf.shape[1] != 2:
             raise ValueError(f"The shape of surf must be (n_points, 2), but got {surf.shape}")
 
         _surf = surf.copy()
         if transform:
             _surf = self._transform_surface_list(surfs_list=[_surf])[0]
@@ -154,25 +162,30 @@
         color: str,
         label: str,
         linestyle: Optional[str] = None,
         marker: Optional[str] = None,
         **kwargs: Any,
     ) -> Any:
         """
-        Plot multiple surfaces.
+        Plot the true pareto front surface.
+        The true pareto front must be provided when instantiating this class.
 
         Args:
             ax (plt.Axes):
                 The subplots axes.
             color (str):
-                The color of the plot
+                The color of the plot.
             label (str):
                 The label of the plot.
+            linestyle (Optional[str]):
+                The linestyle of the plot.
+            marker (Optional[str]):
+                The marker of the plot.
             kwargs:
-                The kwargs for scatter.
+                The kwargs for ax.plot.
         """
         if self._true_pareto_sols is None:
             raise AttributeError("true_pareto_sols is not provided at the instantiation")
 
         true_pareto_surf = pareto_front_to_surface(
             self._true_pareto_sols.copy(),
             x_min=self.x_min,
@@ -212,16 +225,20 @@
                 The vertices of the empirical attainment surfaces for each plot.
                 Each element should have the shape of (X.size, 2).
                 If this is an array, then the shape must be (n_surf, X.size, 2).
             colors (List[str]):
                 The colors of each plot
             labels (List[str]):
                 The labels of each plot.
+            linestyles (Optional[List[str]]):
+                The linestyles of each plot.
+            markers (Optional[List[str]]):
+                The markers of each plot.
             kwargs:
-                The kwargs for scatter.
+                The kwargs for ax.plot.
         """
         lines: List[Any] = []
         _surfs = deepcopy(surfs)
         _surfs = self._transform_surface_list(_surfs)
 
         n_surfs = len(_surfs)
         linestyles = linestyles if linestyles is not None else [None] * n_surfs
@@ -258,16 +275,22 @@
                 The vertices of the empirical attainment surfaces for each level.
                 If surf[i, j, 1] takes np.inf, this is not actually on the surface.
                 The shape is (3, X.size, 2).
             color (str):
                 The color of the plot
             label (str):
                 The label of the plot.
+            linestyle (Optional[str]):
+                The linestyle of the plot.
+            marker (Optional[str]):
+                The marker of the plot.
+            transform (bool):
+                Whether automatically transforming based on (x_min, x_max) and (y_min, y_max).
             kwargs:
-                The kwargs for scatter.
+                The kwargs for ax.plot.
         """
         if surfs.shape[0] != 3:
             raise ValueError(f"plot_surface_with_band requires three levels, but got only {surfs.shape[0]} levels")
 
         _surfs = deepcopy(surfs)
         if transform:
             _surfs = self._transform_surface_list(surfs_list=_surfs)
@@ -298,29 +321,33 @@
         colors: List[str],
         labels: List[str],
         linestyles: Optional[List[Optional[str]]] = None,
         markers: Optional[List[Optional[str]]] = None,
         **kwargs: Any,
     ) -> List[Any]:
         """
-        Plot multiple surfaces.
+        Plot multiple surfaces with a band.
 
         Args:
             ax (plt.Axes):
                 The subplots axes.
             surfs_list (Union[np.ndarray, List[np.ndarray]]):
                 The vertices of the empirical attainment surfaces for each plot.
                 Each element should have the shape of (3, X.size, 2).
                 If this is an array, then the shape must be (n_surf, 3, X.size, 2).
             colors (List[str]):
-                The colors of each plot
+                The colors of each plot.
             labels (List[str]):
                 The labels of each plot.
+            linestyles (Optional[List[str]]):
+                The linestyles of each plot.
+            markers (Optional[List[str]]):
+                The markers of each plot.
             kwargs:
-                The kwargs for scatter.
+                The kwargs for ax.plot.
         """
         lines: List[Any] = []
         _surfs_list = deepcopy(surfs_list)
         _surfs_list = self._transform_surface_list(_surfs_list)
 
         n_surfs = len(_surfs_list)
         linestyles = linestyles if linestyles is not None else [None] * n_surfs
@@ -369,20 +396,31 @@
         Args:
             ax (plt.Axes):
                 The subplots axes.
             costs_array (np.ndarray):
                 The costs obtained in the observations.
                 The shape must be (n_independent_runs, n_samples, n_obj).
                 For now, we only support n_obj == 2.
-            colors (str):
-                The color of the plot
+            color (str):
+                The color of the plot.
             label (str):
                 The label of the plot.
+            linestyle (Optional[str]):
+                The linestyle of the plot.
+            marker (Optional[str]):
+                The marker of the plot.
+            log (bool):
+                Whether to use the log scale in the y-axis of the plot.
+            axis_label (bool):
+                Whether to add the default axis labels or not.
+            normalize (bool):
+                Whether to normalize the hypervolume or not.
+                If True, the y-axis is scaled into [0, 1].
             kwargs:
-                The kwargs for scatter.
+                The kwargs for ax.plot.
         """
         if len(costs_array.shape) != 3 or costs_array.shape[-1] != 2:
             raise ValueError(
                 f"The shape of costs_array must be (n_independent_runs, n_points, 2), but got {costs_array.shape}"
             )
         if self._ref_point is None:
             raise AttributeError("ref_point must be provided for plot_hypervolume2d_with_band")
@@ -439,17 +477,28 @@
             ax (plt.Axes):
                 The subplots axes.
             costs_array (np.ndarray):
                 The costs obtained in the observations.
                 The shape must be (n_curves, n_independent_runs, n_samples, n_obj).
                 For now, we only support n_obj == 2.
             colors (List[str]):
-                The colors of each plot
+                The colors of each plot.
             labels (List[str]):
                 The labels of each plot.
+            linestyles (Optional[List[str]]):
+                The linestyles of each plot.
+            markers (Optional[List[str]]):
+                The markers of each plot.
+            log (bool):
+                Whether to use the log scale in the y-axis of the plot.
+            axis_label (bool):
+                Whether to add the default axis labels or not.
+            normalize (bool):
+                Whether to normalize the hypervolume or not.
+                If True, the y-axis is scaled into [0, 1].
             kwargs:
                 The kwargs for scatter.
         """
         if len(costs_array.shape) != 4 or costs_array.shape[-1] != 2:
             raise ValueError(
                 "The shape of costs_array must be (n_curves, n_independent_runs, n_points, 2),"
                 f" but got {costs_array.shape}"
@@ -501,19 +550,23 @@
         Args:
             ax (plt.Axes):
                 The subplots axes.
             n_observations (int):
                 How many samples happened in each experiment.
                 We need this value to set xlim.
             color (str):
-                The color of the plot
+                The color of the plot.
             label (str):
                 The label of the plot.
+            linestyle (Optional[str]):
+                The linestyle of the plot.
+            marker (Optional[str]):
+                The marker of the plot.
             kwargs:
-                The kwargs for scatter.
+                The kwargs for ax.plot.
         """
 
         if normalize:
             hv = 1.0
         else:
             hv = self._compute_true_pareto_surface_hypervolume2d()
```

## Comparing `empirical_attainment_func-0.4.0.dist-info/LICENSE` & `empirical_attainment_func-0.4.1.dist-info/LICENSE`

 * *Files identical despite different names*


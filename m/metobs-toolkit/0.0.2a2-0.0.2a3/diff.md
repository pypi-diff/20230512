# Comparing `tmp/metobs_toolkit-0.0.2a2.tar.gz` & `tmp/metobs_toolkit-0.0.2a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metobs_toolkit-0.0.2a2.tar", max compression
+gzip compressed data, was "metobs_toolkit-0.0.2a3.tar", max compression
```

## Comparing `metobs_toolkit-0.0.2a2.tar` & `metobs_toolkit-0.0.2a3.tar`

### file list

```diff
@@ -1,40 +1,58 @@
--rw-r--r--   0        0        0     1074 2022-09-22 07:29:20.660989 metobs_toolkit-0.0.2a2/LICENSE
--rw-r--r--   0        0        0      403 2023-05-10 06:57:22.583568 metobs_toolkit-0.0.2a2/README.md
--rw-r--r--   0        0        0     2438 2023-05-10 12:42:06.812133 metobs_toolkit-0.0.2a2/metobs_toolkit/__init__.py
--rw-r--r--   0        0        0    19751 2023-05-10 07:27:19.656930 metobs_toolkit-0.0.2a2/metobs_toolkit/analysis.py
--rw-r--r--   0        0        0     2566 2023-05-10 06:57:22.695567 metobs_toolkit-0.0.2a2/metobs_toolkit/convertors.py
--rw-r--r--   0        0        0    12056 2023-05-10 07:27:19.656930 metobs_toolkit-0.0.2a2/metobs_toolkit/data_import.py
--rw-r--r--   0        0        0     2378 2023-05-10 06:57:22.695567 metobs_toolkit-0.0.2a2/metobs_toolkit/data_templates/db_templates.py
--rw-r--r--   0        0        0     1701 2023-05-10 07:27:19.656930 metobs_toolkit-0.0.2a2/metobs_toolkit/data_templates/import_templates.py
--rw-r--r--   0        0        0      931 2023-05-10 06:57:22.695567 metobs_toolkit-0.0.2a2/metobs_toolkit/data_templates/template_defaults/default_template.csv
--rwxr-xr-x   0        0        0  9062298 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/datafiles/demo_datafile.csv
--rw-r--r--   0        0        0     2306 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/datafiles/demo_metadatafile.csv
--rw-r--r--   0        0        0      931 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/datafiles/demo_templatefile.csv
--rw-r--r--   0        0        0    68547 2023-05-10 11:47:22.343657 metobs_toolkit-0.0.2a2/metobs_toolkit/dataset.py
--rw-r--r--   0        0        0    17115 2023-05-10 11:47:22.343657 metobs_toolkit-0.0.2a2/metobs_toolkit/dataset_settings_updater.py
--rw-r--r--   0        0        0    11623 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/df_helpers.py
--rw-r--r--   0        0        0    22073 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/gap.py
--rw-r--r--   0        0        0    15267 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/gap_filling.py
--rw-r--r--   0        0        0      673 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a2/metobs_toolkit/geometry_functions.py
--rw-r--r--   0        0        0    18129 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/landcover_functions.py
--rw-r--r--   0        0        0     7973 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/missingobs.py
--rw-r--r--   0        0        0     4723 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a2/metobs_toolkit/modeldata.py
--rw-r--r--   0        0        0    20492 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/plotting_functions.py
--rw-r--r--   0        0        0     1847 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/printing.py
--rw-r--r--   0        0        0    22903 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a2/metobs_toolkit/qc_checks.py
--rw-r--r--   0        0        0     4159 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a2/metobs_toolkit/qc_statistics.py
--rw-r--r--   0        0        0    14146 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/settings.py
--rw-r--r--   0        0        0       73 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/app_print_settings.json
--rw-r--r--   0        0        0      237 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/dataset_resolution_settings.json
--rw-r--r--   0        0        0     4509 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/default_formats_settings.py
--rw-r--r--   0        0        0     1831 2023-05-10 07:27:19.692932 metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/gaps_and_missing_settings.py
--rw-r--r--   0        0        0     3880 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/gee_settings.py
--rw-r--r--   0        0        0     2851 2023-05-10 11:47:22.347657 metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/qc_settings.py
--rw-r--r--   0        0        0      132 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/server_login.json
--rw-r--r--   0        0        0  8385556 2023-05-10 06:57:22.787565 metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shp
--rw-r--r--   0        0        0     2108 2023-05-10 06:57:22.787565 metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shx
--rw-r--r--   0        0        0      916 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/station.py
--rw-r--r--   0        0        0        0 2023-05-10 12:30:33.435807 metobs_toolkit-0.0.2a2/metobs_toolkit/test.py
--rw-r--r--   0        0        0     2441 2023-05-10 06:57:22.787565 metobs_toolkit-0.0.2a2/metobs_toolkit/writing_files.py
--rw-r--r--   0        0        0      835 2023-05-10 12:42:06.732132 metobs_toolkit-0.0.2a2/pyproject.toml
--rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 metobs_toolkit-0.0.2a2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2022-09-22 07:29:20.660989 metobs_toolkit-0.0.2a3/LICENSE
+-rw-r--r--   0        0        0      403 2023-05-10 06:57:22.583568 metobs_toolkit-0.0.2a3/README.md
+-rw-r--r--   0        0        0      222 2023-05-12 09:54:13.697462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/cache/custom_template.csv
+-rw-r--r--   0        0        0      485 2023-05-12 09:54:13.697462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/cache/custom_template_Ian.csv
+-rw-r--r--   0        0        0      295 2023-05-12 09:54:13.697462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/cache/vlindersmall_template.csv
+-rw-r--r--   0        0        0      160 2023-05-12 09:54:13.697462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/cache/wow_template.csv
+-rw-r--r--   0        0        0     1426 2023-05-12 09:54:13.697462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/data_func.py
+-rw-r--r--   0        0        0      825 2023-05-12 09:54:13.697462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/errors.py
+-rw-r--r--   0        0        0     4857 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/extra_windows.py
+-rw-r--r--   0        0        0     3369 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/fig_window.ui
+-rw-r--r--   0        0        0     2320 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/figuremodel.py
+-rw-r--r--   0        0        0     2029 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/json_save_func.py
+-rw-r--r--   0        0        0    10955 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/main.py
+-rw-r--r--   0        0        0     1435 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/merge_overview.ui
+-rw-r--r--   0        0        0     2367 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/pandasmodel.py
+-rw-r--r--   0        0        0     2288 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/path_handler.py
+-rw-r--r--   0        0        0      283 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/save_gui_vals.json
+-rw-r--r--   0        0        0    46735 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/templ_build.ui
+-rw-r--r--   0        0        0    11554 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/template_func.py
+-rw-r--r--   0        0        0     7330 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/GUI/tlk_scripts.py
+-rw-r--r--   0        0        0     2503 2023-05-12 10:11:37.762628 metobs_toolkit-0.0.2a3/metobs_toolkit/__init__.py
+-rw-r--r--   0        0        0    19751 2023-05-12 09:54:16.821478 metobs_toolkit-0.0.2a3/metobs_toolkit/analysis.py
+-rw-r--r--   0        0        0     2566 2023-05-10 06:57:22.695567 metobs_toolkit-0.0.2a3/metobs_toolkit/convertors.py
+-rw-r--r--   0        0        0    12056 2023-05-12 09:54:16.821478 metobs_toolkit-0.0.2a3/metobs_toolkit/data_import.py
+-rw-r--r--   0        0        0     2378 2023-05-10 06:57:22.695567 metobs_toolkit-0.0.2a3/metobs_toolkit/data_templates/db_templates.py
+-rw-r--r--   0        0        0     1701 2023-05-12 09:54:16.821478 metobs_toolkit-0.0.2a3/metobs_toolkit/data_templates/import_templates.py
+-rw-r--r--   0        0        0      931 2023-05-10 06:57:22.695567 metobs_toolkit-0.0.2a3/metobs_toolkit/data_templates/template_defaults/default_template.csv
+-rwxr-xr-x   0        0        0  9062298 2023-05-12 09:54:16.849478 metobs_toolkit-0.0.2a3/metobs_toolkit/datafiles/demo_datafile.csv
+-rw-r--r--   0        0        0     2306 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/datafiles/demo_metadatafile.csv
+-rw-r--r--   0        0        0      931 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/datafiles/demo_templatefile.csv
+-rw-r--r--   0        0        0    68582 2023-05-12 09:54:16.881478 metobs_toolkit-0.0.2a3/metobs_toolkit/dataset.py
+-rw-r--r--   0        0        0    17115 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/dataset_settings_updater.py
+-rw-r--r--   0        0        0    11623 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/df_helpers.py
+-rw-r--r--   0        0        0    22073 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/gap.py
+-rw-r--r--   0        0        0    15267 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/gap_filling.py
+-rw-r--r--   0        0        0      673 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a3/metobs_toolkit/geometry_functions.py
+-rw-r--r--   0        0        0      222 2023-05-12 09:54:13.701462 metobs_toolkit-0.0.2a3/metobs_toolkit/gui_launcher.py
+-rw-r--r--   0        0        0    18129 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/landcover_functions.py
+-rw-r--r--   0        0        0     7973 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/missingobs.py
+-rw-r--r--   0        0        0     4723 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a3/metobs_toolkit/modeldata.py
+-rw-r--r--   0        0        0    20497 2023-05-12 09:54:16.877478 metobs_toolkit-0.0.2a3/metobs_toolkit/plotting_functions.py
+-rw-r--r--   0        0        0     1847 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/printing.py
+-rw-r--r--   0        0        0    22903 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a3/metobs_toolkit/qc_checks.py
+-rw-r--r--   0        0        0     4159 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a3/metobs_toolkit/qc_statistics.py
+-rw-r--r--   0        0        0    14146 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/settings.py
+-rw-r--r--   0        0        0       73 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/app_print_settings.json
+-rw-r--r--   0        0        0      237 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/dataset_resolution_settings.json
+-rw-r--r--   0        0        0     4509 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/default_formats_settings.py
+-rw-r--r--   0        0        0     1831 2023-05-12 09:54:16.873478 metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/gaps_and_missing_settings.py
+-rw-r--r--   0        0        0     3880 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/gee_settings.py
+-rw-r--r--   0        0        0     2851 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/qc_settings.py
+-rw-r--r--   0        0        0      132 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/server_login.json
+-rw-r--r--   0        0        0  8385556 2023-05-10 06:57:22.787565 metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shp
+-rw-r--r--   0        0        0     2108 2023-05-10 06:57:22.787565 metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shx
+-rw-r--r--   0        0        0      916 2023-05-12 09:54:16.853478 metobs_toolkit-0.0.2a3/metobs_toolkit/station.py
+-rw-r--r--   0        0        0     2441 2023-05-10 06:57:22.787565 metobs_toolkit-0.0.2a3/metobs_toolkit/writing_files.py
+-rw-r--r--   0        0        0      853 2023-05-12 10:11:37.682628 metobs_toolkit-0.0.2a3/pyproject.toml
+-rw-r--r--   0        0        0     1495 1970-01-01 00:00:00.000000 metobs_toolkit-0.0.2a3/PKG-INFO
```

### Comparing `metobs_toolkit-0.0.2a2/LICENSE` & `metobs_toolkit-0.0.2a3/LICENSE`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/__init__.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,19 +63,22 @@
 # Import classes and function to be used by the user
 # =============================================================================
 
 from metobs_toolkit.dataset import Dataset
 from metobs_toolkit.station import Station
 from metobs_toolkit.modeldata import Modeldata
 
+# import GUI
+from metobs_toolkit.gui_launcher import launch_gui
+
 # =============================================================================
 # Import extenders
 # =============================================================================
 from metobs_toolkit.dataset_settings_updater import Dataset
 
 # =============================================================================
 # Version
 # =============================================================================
 
 # DO not change this manually!
-__version__ = "0.0.2a2"
+__version__ = "0.0.2a3"
```

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/analysis.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/analysis.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/convertors.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/convertors.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/data_import.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/data_import.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/data_templates/db_templates.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/data_templates/db_templates.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/data_templates/import_templates.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/data_templates/import_templates.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/data_templates/template_defaults/default_template.csv` & `metobs_toolkit-0.0.2a3/metobs_toolkit/data_templates/template_defaults/default_template.csv`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/datafiles/demo_datafile.csv` & `metobs_toolkit-0.0.2a3/metobs_toolkit/datafiles/demo_datafile.csv`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/datafiles/demo_metadatafile.csv` & `metobs_toolkit-0.0.2a3/metobs_toolkit/datafiles/demo_metadatafile.csv`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/datafiles/demo_templatefile.csv` & `metobs_toolkit-0.0.2a3/metobs_toolkit/datafiles/demo_templatefile.csv`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/dataset.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,14 +232,15 @@
         obstype="temp",
         colorby="name",
         starttime=None,
         endtime=None,
         title=None,
         legend=True,
         show_outliers=True,
+        ax=None
     ):
         """
         This function creates a timeseries plot for the dataset. The variable observation type
         is plotted for all stationnames from a starttime to an endtime.
 
 
          All styling attributes are extracted from the Settings.
@@ -332,14 +333,15 @@
             ylabel=self.data_template[obstype]["orig_name"],
             colorby=colorby,
             show_legend=legend,
             show_outliers=show_outliers,
             plot_settings=self.settings.app["plot_settings"],
             gap_settings=self.settings.gap,
             qc_info_settings=self.settings.qc["qc_checks_info"],
+            ax=ax,
         )
 
         return ax
 
     def make_geo_plot(
         self,
         obstype="temp",
```

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/dataset_settings_updater.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/dataset_settings_updater.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/df_helpers.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/df_helpers.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/gap.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/gap.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/gap_filling.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/gap_filling.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/geometry_functions.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/geometry_functions.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/landcover_functions.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/landcover_functions.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/missingobs.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/missingobs.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/modeldata.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/modeldata.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/plotting_functions.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/plotting_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,19 +250,21 @@
     ylabel,
     colorby,
     show_legend,
     show_outliers,
     plot_settings,
     gap_settings,
     qc_info_settings,
+    ax=None
 ):
-    # plot_settings = plot_settings['time_series']
 
-    # init figure
-    fig, ax = plt.subplots(figsize=plot_settings["time_series"]["figsize"])
+    if isinstance(ax, type(None)):
+        # init figure
+        fig, ax = plt.subplots(figsize=plot_settings["time_series"]["figsize"])
+
 
     # subbset and cleanup data
 
     mergedf = mergedf[~mergedf.index.duplicated()]
     init_idx = mergedf.index
 
     if not show_outliers:
```

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/printing.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/printing.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/qc_checks.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/qc_checks.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/qc_statistics.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/qc_statistics.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/settings.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/settings.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/default_formats_settings.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/default_formats_settings.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/gaps_and_missing_settings.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/gaps_and_missing_settings.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/gee_settings.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/gee_settings.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/qc_settings.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/qc_settings.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shp` & `metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shp`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shx` & `metobs_toolkit-0.0.2a3/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shx`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/station.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/station.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/metobs_toolkit/writing_files.py` & `metobs_toolkit-0.0.2a3/metobs_toolkit/writing_files.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a2/pyproject.toml` & `metobs_toolkit-0.0.2a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MetObs-toolkit"
-version = "0.0.2a2"
+version = "0.0.2a3"
 description = "A Meteorological observations toolkit for scientists"
 authors = ["Thomas Vergauwen <thomas.vergauwen@meteo.be>"]
 maintainers = ["Thomas Vergauwen <thomas.vergauwen@meteo.be>"]
 license = "LICENSE"
 readme = "README.md"
 documentation = "https://python-poetry.org/docs/"
 packages = [{include = "metobs_toolkit"}]
@@ -17,14 +17,15 @@
 matplotlib = "^3.0.0"
 mysql-connector-python = "^8.0.6"
 geopandas = "^0.9.0"
 pyproj = "~3.4"
 #rasterstats = "^0.16.0"
 mapclassify = "^2.4.0"
 earthengine-api = "^0.1.340"
+PyQt5 = "^5.15.0"
 
 
 
 [tool.poetry.group.dev.dependencies]
 poetry = "^1.3.2"
 
 [build-system]
```

### Comparing `metobs_toolkit-0.0.2a2/PKG-INFO` & `metobs_toolkit-0.0.2a3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: metobs-toolkit
-Version: 0.0.2a2
+Version: 0.0.2a3
 Summary: A Meteorological observations toolkit for scientists
 License: LICENSE
 Keywords: meteorology,observations,urban climate
 Author: Thomas Vergauwen
 Author-email: thomas.vergauwen@meteo.be
 Maintainer: Thomas Vergauwen
 Maintainer-email: thomas.vergauwen@meteo.be
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyQt5 (>=5.15.0,<6.0.0)
 Requires-Dist: earthengine-api (>=0.1.340,<0.2.0)
 Requires-Dist: geopandas (>=0.9.0,<0.10.0)
 Requires-Dist: mapclassify (>=2.4.0,<3.0.0)
 Requires-Dist: matplotlib (>=3.0.0,<4.0.0)
 Requires-Dist: mysql-connector-python (>=8.0.6,<9.0.0)
 Requires-Dist: numpy (>=1.17.3,<2.0.0)
 Requires-Dist: pandas (>=1.3.0,<2.0.0)
```


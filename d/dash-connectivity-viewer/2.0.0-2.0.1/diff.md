# Comparing `tmp/dash-connectivity-viewer-2.0.0.tar.gz` & `tmp/dash-connectivity-viewer-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash-connectivity-viewer-2.0.0.tar", last modified: Tue May  9 18:49:15 2023, max compression
+gzip compressed data, was "dash-connectivity-viewer-2.0.1.tar", last modified: Fri May 12 20:25:16 2023, max compression
```

## Comparing `dash-connectivity-viewer-2.0.0.tar` & `dash-connectivity-viewer-2.0.1.tar`

### file list

```diff
@@ -1,55 +1,51 @@
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-09 18:49:15.861546 dash-connectivity-viewer-2.0.0/
--rw-r--r--   0 caseysm    (501) staff       (20)       71 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.0/MANIFEST.in
--rw-r--r--   0 caseysm    (501) staff       (20)      499 2023-05-09 18:49:15.861328 dash-connectivity-viewer-2.0.0/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)      216 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.0/README.md
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-09 18:49:15.847099 dash-connectivity-viewer-2.0.0/app/
--rw-r--r--   0 caseysm    (501) staff       (20)     2204 2023-04-13 17:47:51.000000 dash-connectivity-viewer-2.0.0/app/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)     2648 2023-04-13 17:47:51.000000 dash-connectivity-viewer-2.0.0/app/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)      323 2023-04-13 17:47:51.000000 dash-connectivity-viewer-2.0.0/app/reset_auth.py
--rw-r--r--   0 caseysm    (501) staff       (20)      736 2023-04-13 17:47:51.000000 dash-connectivity-viewer-2.0.0/app/webapp.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-09 18:49:15.847323 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/
--rw-r--r--   0 caseysm    (501) staff       (20)       22 2023-05-09 18:48:23.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/__init__.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-09 18:49:15.852882 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_connectivity/
--rw-r--r--   0 caseysm    (501) staff       (20)      568 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_connectivity/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    24414 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_connectivity/callbacks.py
--rw-r--r--   0 caseysm    (501) staff       (20)     5453 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_connectivity/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3461 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py
--rw-r--r--   0 caseysm    (501) staff       (20)     6156 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py
--rw-r--r--   0 caseysm    (501) staff       (20)       82 2023-03-18 18:57:32.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_connectivity/external_stylesheets.py
--rw-r--r--   0 caseysm    (501) staff       (20)    20418 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_connectivity/layout.py
--rw-r--r--   0 caseysm    (501) staff       (20)     4439 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-09 18:49:15.854204 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_table/
--rw-r--r--   0 caseysm    (501) staff       (20)      711 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_table/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    14456 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_table/callbacks.py
--rw-r--r--   0 caseysm    (501) staff       (20)     1347 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_table/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)      210 2023-02-08 23:15:09.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_table/ct_utils.py
--rw-r--r--   0 caseysm    (501) staff       (20)    14861 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_table/layout.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-09 18:49:15.858246 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/common/
--rw-r--r--   0 caseysm    (501) staff       (20)       17 2023-04-13 06:43:13.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/common/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)     5184 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/common/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)     2914 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/common/dash_url_helper.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-09 18:49:15.858936 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/common/data/
--rw-r--r--   0 caseysm    (501) staff       (20)      144 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/common/data/height_bounds_v1.npy
--rw-r--r--   0 caseysm    (501) staff       (20)      168 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/common/data/layer_bounds_v1.npy
--rw-r--r--   0 caseysm    (501) staff       (20)    10103 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/common/dataframe_utilities.py
--rw-r--r--   0 caseysm    (501) staff       (20)      294 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/common/external_stylesheets.py
--rw-r--r--   0 caseysm    (501) staff       (20)    13477 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/common/link_utilities.py
--rw-r--r--   0 caseysm    (501) staff       (20)     4043 2023-04-25 19:19:28.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/common/lookup_utilities.py
--rw-r--r--   0 caseysm    (501) staff       (20)    11384 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/common/neuron_data_base.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3756 2023-04-25 19:21:22.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/common/schema_utils.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3950 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/common/table_lookup.py
--rw-r--r--   0 caseysm    (501) staff       (20)      762 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/common/transform_utils.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-09 18:49:15.860834 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/connectivity_table/
--rw-r--r--   0 caseysm    (501) staff       (20)      591 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/connectivity_table/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    13817 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/connectivity_table/callbacks.py
--rw-r--r--   0 caseysm    (501) staff       (20)      523 2023-02-08 23:15:09.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/connectivity_table/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)     9093 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/connectivity_table/layout.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-09 18:49:15.848337 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer.egg-info/
--rw-r--r--   0 caseysm    (501) staff       (20)      499 2023-05-09 18:49:15.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer.egg-info/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)     2040 2023-05-09 18:49:15.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-05-09 18:49:15.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 caseysm    (501) staff       (20)     1114 2023-05-09 18:49:15.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer.egg-info/requires.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       29 2023-05-09 18:49:15.000000 dash-connectivity-viewer-2.0.0/dash_connectivity_viewer.egg-info/top_level.txt
--rw-r--r--   0 caseysm    (501) staff       (20)     3240 2023-05-02 20:56:04.000000 dash-connectivity-viewer-2.0.0/requirements.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-05-09 18:49:15.861617 dash-connectivity-viewer-2.0.0/setup.cfg
--rw-r--r--   0 caseysm    (501) staff       (20)     1153 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.0/setup.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-12 20:25:16.638161 dash-connectivity-viewer-2.0.1/
+-rw-r--r--   0 caseysm    (501) staff       (20)     1842 2023-05-09 18:49:42.000000 dash-connectivity-viewer-2.0.1/LICENSE.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       71 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.1/MANIFEST.in
+-rw-r--r--   0 caseysm    (501) staff       (20)      525 2023-05-12 20:25:16.637827 dash-connectivity-viewer-2.0.1/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)      216 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.1/README.md
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-12 20:25:16.603821 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/
+-rw-r--r--   0 caseysm    (501) staff       (20)       22 2023-05-12 20:25:00.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/__init__.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-12 20:25:16.618488 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_connectivity/
+-rw-r--r--   0 caseysm    (501) staff       (20)      568 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_connectivity/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    24414 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_connectivity/callbacks.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     5453 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_connectivity/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3461 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     6156 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py
+-rw-r--r--   0 caseysm    (501) staff       (20)       82 2023-03-18 18:57:32.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_connectivity/external_stylesheets.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    20418 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_connectivity/layout.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     4439 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-12 20:25:16.623044 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_table/
+-rw-r--r--   0 caseysm    (501) staff       (20)      711 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_table/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    14456 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_table/callbacks.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     1347 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_table/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      210 2023-02-08 23:15:09.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_table/ct_utils.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    14861 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_table/layout.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-12 20:25:16.631924 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/common/
+-rw-r--r--   0 caseysm    (501) staff       (20)       17 2023-04-13 06:43:13.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/common/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     5184 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/common/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     2914 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/common/dash_url_helper.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-12 20:25:16.633696 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/common/data/
+-rw-r--r--   0 caseysm    (501) staff       (20)      144 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/common/data/height_bounds_v1.npy
+-rw-r--r--   0 caseysm    (501) staff       (20)      168 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/common/data/layer_bounds_v1.npy
+-rw-r--r--   0 caseysm    (501) staff       (20)    10103 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/common/dataframe_utilities.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      294 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/common/external_stylesheets.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    13477 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/common/link_utilities.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     4043 2023-04-25 19:19:28.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/common/lookup_utilities.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    11384 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/common/neuron_data_base.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3756 2023-04-25 19:21:22.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/common/schema_utils.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3950 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/common/table_lookup.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      762 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/common/transform_utils.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-12 20:25:16.637204 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/connectivity_table/
+-rw-r--r--   0 caseysm    (501) staff       (20)      591 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/connectivity_table/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    13817 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/connectivity_table/callbacks.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      523 2023-02-08 23:15:09.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/connectivity_table/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     9093 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/connectivity_table/layout.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-05-12 20:25:16.607485 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer.egg-info/
+-rw-r--r--   0 caseysm    (501) staff       (20)      525 2023-05-12 20:25:16.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)     1990 2023-05-12 20:25:16.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-05-12 20:25:16.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)      168 2023-05-12 20:25:16.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer.egg-info/requires.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       25 2023-05-12 20:25:16.000000 dash-connectivity-viewer-2.0.1/dash_connectivity_viewer.egg-info/top_level.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)      167 2023-05-12 20:23:49.000000 dash-connectivity-viewer-2.0.1/requirements.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-05-12 20:25:16.638274 dash-connectivity-viewer-2.0.1/setup.cfg
+-rw-r--r--   0 caseysm    (501) staff       (20)     1153 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.0.1/setup.py
```

### Comparing `dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_connectivity/__init__.py` & `dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_connectivity/__init__.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_connectivity/callbacks.py` & `dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_connectivity/callbacks.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_connectivity/config.py` & `dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_connectivity/config.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py` & `dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py` & `dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_connectivity/layout.py` & `dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_connectivity/layout.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py` & `dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_table/__init__.py` & `dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_table/__init__.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_table/callbacks.py` & `dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_table/callbacks.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_table/config.py` & `dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_table/config.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/cell_type_table/layout.py` & `dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/cell_type_table/layout.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/common/config.py` & `dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/common/config.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/common/dash_url_helper.py` & `dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/common/dash_url_helper.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/common/dataframe_utilities.py` & `dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/common/dataframe_utilities.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/common/link_utilities.py` & `dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/common/link_utilities.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/common/lookup_utilities.py` & `dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/common/lookup_utilities.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/common/neuron_data_base.py` & `dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/common/neuron_data_base.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/common/schema_utils.py` & `dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/common/schema_utils.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/common/table_lookup.py` & `dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/common/table_lookup.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/common/transform_utils.py` & `dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/common/transform_utils.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/connectivity_table/__init__.py` & `dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/connectivity_table/__init__.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/connectivity_table/callbacks.py` & `dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/connectivity_table/callbacks.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/connectivity_table/config.py` & `dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/connectivity_table/config.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.0/dash_connectivity_viewer/connectivity_table/layout.py` & `dash-connectivity-viewer-2.0.1/dash_connectivity_viewer/connectivity_table/layout.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.0.0/dash_connectivity_viewer.egg-info/SOURCES.txt` & `dash-connectivity-viewer-2.0.1/dash_connectivity_viewer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,12 @@
+LICENSE.txt
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
-app/__init__.py
-app/config.py
-app/reset_auth.py
-app/webapp.py
 dash_connectivity_viewer/__init__.py
 dash_connectivity_viewer.egg-info/PKG-INFO
 dash_connectivity_viewer.egg-info/SOURCES.txt
 dash_connectivity_viewer.egg-info/dependency_links.txt
 dash_connectivity_viewer.egg-info/requires.txt
 dash_connectivity_viewer.egg-info/top_level.txt
 dash_connectivity_viewer/cell_type_connectivity/__init__.py
```

### Comparing `dash-connectivity-viewer-2.0.0/setup.py` & `dash-connectivity-viewer-2.0.1/setup.py`

 * *Files identical despite different names*


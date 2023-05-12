# Comparing `tmp/spatial_summarize_within-0.1.2.tar.gz` & `tmp/spatial_summarize_within-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatial_summarize_within-0.1.2.tar", last modified: Mon May  8 23:09:43 2023, max compression
+gzip compressed data, was "spatial_summarize_within-0.2.1.tar", last modified: Fri May 12 04:21:11 2023, max compression
```

## Comparing `spatial_summarize_within-0.1.2.tar` & `spatial_summarize_within-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-08 23:09:43.592262 spatial_summarize_within-0.1.2/
--rw-r--r--   0 Kenne      (501) staff       (20)     1076 2023-05-06 22:57:53.000000 spatial_summarize_within-0.1.2/LICENSE
--rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-05-08 23:09:43.592158 spatial_summarize_within-0.1.2/PKG-INFO
--rw-r--r--   0 Kenne      (501) staff       (20)     2188 2023-05-06 22:57:53.000000 spatial_summarize_within-0.1.2/README.md
--rw-r--r--   0 Kenne      (501) staff       (20)       38 2023-05-08 23:09:43.592296 spatial_summarize_within-0.1.2/setup.cfg
--rw-r--r--   0 Kenne      (501) staff       (20)      252 2023-05-08 23:08:58.000000 spatial_summarize_within-0.1.2/setup.py
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-08 23:09:43.591436 spatial_summarize_within-0.1.2/spatial_summarize_within/
--rw-r--r--   0 Kenne      (501) staff       (20)       46 2023-05-06 23:00:41.000000 spatial_summarize_within-0.1.2/spatial_summarize_within/__init__.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2294 2023-05-08 23:09:21.000000 spatial_summarize_within-0.1.2/spatial_summarize_within/summarize_within.py
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-08 23:09:43.592010 spatial_summarize_within-0.1.2/spatial_summarize_within.egg-info/
--rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-05-08 23:09:43.000000 spatial_summarize_within-0.1.2/spatial_summarize_within.egg-info/PKG-INFO
--rw-r--r--   0 Kenne      (501) staff       (20)      347 2023-05-08 23:09:43.000000 spatial_summarize_within-0.1.2/spatial_summarize_within.egg-info/SOURCES.txt
--rw-r--r--   0 Kenne      (501) staff       (20)        1 2023-05-08 23:09:43.000000 spatial_summarize_within-0.1.2/spatial_summarize_within.egg-info/dependency_links.txt
--rw-r--r--   0 Kenne      (501) staff       (20)       37 2023-05-08 23:09:43.000000 spatial_summarize_within-0.1.2/spatial_summarize_within.egg-info/requires.txt
--rw-r--r--   0 Kenne      (501) staff       (20)       25 2023-05-08 23:09:43.000000 spatial_summarize_within-0.1.2/spatial_summarize_within.egg-info/top_level.txt
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-12 04:21:11.234774 spatial_summarize_within-0.2.1/
+-rw-r--r--   0 Kenne      (501) staff       (20)     1076 2023-05-06 22:57:53.000000 spatial_summarize_within-0.2.1/LICENSE
+-rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-05-12 04:21:11.234638 spatial_summarize_within-0.2.1/PKG-INFO
+-rw-r--r--   0 Kenne      (501) staff       (20)     2170 2023-05-08 23:11:41.000000 spatial_summarize_within-0.2.1/README.md
+-rw-r--r--   0 Kenne      (501) staff       (20)       38 2023-05-12 04:21:11.234817 spatial_summarize_within-0.2.1/setup.cfg
+-rw-r--r--   0 Kenne      (501) staff       (20)      329 2023-05-12 04:20:35.000000 spatial_summarize_within-0.2.1/setup.py
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-12 04:21:11.233705 spatial_summarize_within-0.2.1/spatial_summarize_within/
+-rw-r--r--   0 Kenne      (501) staff       (20)      141 2023-05-12 03:23:32.000000 spatial_summarize_within-0.2.1/spatial_summarize_within/__init__.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2348 2023-05-12 03:51:40.000000 spatial_summarize_within-0.2.1/spatial_summarize_within/max_within.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2346 2023-05-12 03:35:04.000000 spatial_summarize_within-0.2.1/spatial_summarize_within/mean_within.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2348 2023-05-12 03:53:18.000000 spatial_summarize_within-0.2.1/spatial_summarize_within/min_within.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2329 2023-05-12 03:35:04.000000 spatial_summarize_within-0.2.1/spatial_summarize_within/sum_within.py
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-12 04:21:11.234322 spatial_summarize_within-0.2.1/spatial_summarize_within.egg-info/
+-rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-05-12 04:21:11.000000 spatial_summarize_within-0.2.1/spatial_summarize_within.egg-info/PKG-INFO
+-rw-r--r--   0 Kenne      (501) staff       (20)      459 2023-05-12 04:21:11.000000 spatial_summarize_within-0.2.1/spatial_summarize_within.egg-info/SOURCES.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)        1 2023-05-12 04:21:11.000000 spatial_summarize_within-0.2.1/spatial_summarize_within.egg-info/dependency_links.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)       37 2023-05-12 04:21:11.000000 spatial_summarize_within-0.2.1/spatial_summarize_within.egg-info/requires.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)       25 2023-05-12 04:21:11.000000 spatial_summarize_within-0.2.1/spatial_summarize_within.egg-info/top_level.txt
```

### Comparing `spatial_summarize_within-0.1.2/LICENSE` & `spatial_summarize_within-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spatial_summarize_within-0.1.2/README.md` & `spatial_summarize_within-0.2.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 ## Installation
 
 You can install Spatial Summarize Within using pip:
 
 ```bash
 pip install spatial_summarize_within
 ```
-Geo Summarizer has the following dependencies, which will be installed automatically:
+Spatial Summarize Within has the following dependencies, which will be installed automatically:
 
 geopandas
 pandas
 shapely
 mapclassifier
 
 # Usage
 To use Spatial Summarize Within you'll first need to import the summarize_within function:
-from spatial_summarize_within.summarize_within import summarize_within
+```
+from spatial_summarize_within import summarize_within
+```
 
 Next, call the summarize_within function with your input and overlay shapefiles, the columns you want to sum, and the key to group the results by:
 ```
 input_shapefile = gpd.read_file("path/to/your/input_shapefile.shp")
 overlay_shapefile = gpd.read_file("path/to/your/overlay_shapefile.shp")
 
 result = summarize_within(
@@ -36,32 +38,32 @@
     ],
     key_to_group_by="your_group_by_key"
 )
 ```
 The result variable will contain a GeoDataFrame with the summarized data.
 
 # Example
-In this example, we will summarize population data within an input shapefile using an overlay shapefile.
+In this example, we will aggregate population data within census tracts by county.
 
 ```
-from spatial_summarize_within.summarize_within import summarize_within
+from spatial_summarize_within import summarize_within
 import geopandas as gpd
 
 # Load input and overlay shapefiles
-input_shapefile = gpd.read_file("path/to/your/input_shapefile.shp")
-overlay_shapefile = gpd.read_file("path/to/your/overlay_shapefile.shp")
+CENSUS_TRACTS_SHAPEFILE = gpd.read_file("path/to/your/input_shapefile.shp")
+COUNTIES_SHAPEFILE = gpd.read_file("path/to/your/overlay_shapefile.shp")
 
 # Call the summarize_within function
 result = summarize_within(
-    input_shapefile=input_shapefile,
-    overlay_shapefile=overlay_shapefile,
+    input_shapefile=CENSUS_TRACTS_SHAPEFILE,
+    overlay_shapefile=COUNTIES_SHAPEFILE,
     columns_to_sum=[
         "total_population",
         "urban_population",
         "rural_population",
     ],
-    key_to_group_by="region_id"
+    key_to_group_by="county_name"
 )
 
 # Save the result to a new shapefile
 result.to_file("path/to/your/output_shapefile.shp")
 ```
```

### Comparing `spatial_summarize_within-0.1.2/spatial_summarize_within/summarize_within.py` & `spatial_summarize_within-0.2.1/spatial_summarize_within/sum_within.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,47 +4,47 @@
 from shapely import wkt
 import shapely.ops
 from shapely.geometry import Polygon, MultiPolygon, shape, Point
 import geopandas as gpd
 import mapclassify
 
 # Function
-def summarize_within(input_shapefile, overlay_shapefile, columns_to_sum, key_to_group_by):
+def sum_within(input_shapefile, input_summary_features, columns, key):
     # Read input and overlay shapefiles
-    input = input_shapefile
-    overlay = overlay_shapefile
+    input_shapefile = input_shapefile
+    input_summary_features = input_summary_features
 
     # Add area column to input geodataframe
-    input["area"] = input.geometry.area
+    input_summary_features["area"] = input_summary_features.geometry.area
     # Create an empty geodataframe to store the results
     result_gdf = gpd.GeoDataFrame()
 
     # Loop through each polygon in the overlay geodataframe
-    for index, row in overlay.iterrows():
+    for index, row in input_shapefile.iterrows():
         # Create a temporary geodataframe with just the current overlay polygon
-        temp_overlay = gpd.GeoDataFrame([row], columns=overlay.columns)
+        temp_overlay = gpd.GeoDataFrame([row], columns=input_shapefile.columns)
         # set crs
         temp_overlay = temp_overlay.set_crs("EPSG:3395")
         # Intersect the input geodataframe with the current overlay polygon
         temp_intersect = gpd.overlay(input, temp_overlay, how='intersection')
-        # Calculate the area of each polygon in the intersect geodataframe
+        # Calculate the area of each polygon in intersect dataframe
         temp_intersect["intersect_area"] = temp_intersect.area
         # Calculate the percentage overlap of each polygon in the input geodataframe with the current overlay polygon
         temp_intersect["overlap_pct"] = temp_intersect["intersect_area"] / temp_intersect["area"]
         # Calculate the weighted sum
-        columns = columns_to_sum
+        columns = columns
         for column in columns:
             temp_intersect[column] = (temp_intersect[column] * temp_intersect["overlap_pct"]).round(0)
         # Keep only the relevant columns in the temp_intersect dataframe
-        temp_intersect = temp_intersect[[key_to_group_by] + columns + ['intersect_area', 'overlap_pct']]
+        temp_intersect = temp_intersect[[key] + columns + ['intersect_area', 'overlap_pct']]
         # Group the results
-        temp_result = temp_intersect.groupby(key_to_group_by).sum(numeric_only=True).reset_index()
+        temp_result = temp_intersect.groupby(key).sum(numeric_only=True).reset_index()
         # Append the results to the result gdf
         result_gdf = pd.concat([result_gdf, temp_result], ignore_index=True)
 
     # Merge the result with the overlay geodataframe
-    result_gdf = overlay.merge(result_gdf, on=key_to_group_by)
+    result_gdf = input_shapefile.merge(result_gdf, on=key)
 
     # Remove the added area column from input geodataframe
-    input = input.drop("area", axis=1)
+    input_summary_features = input.drop("area", axis=1)
 
     return result_gdf
```


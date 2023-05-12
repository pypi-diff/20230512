# Comparing `tmp/tight_loops-0.2.4.tar.gz` & `tmp/tight_loops-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tight_loops-0.2.4.tar", last modified: Mon May  8 17:41:32 2023, max compression
+gzip compressed data, was "tight_loops-0.3.0.tar", last modified: Fri May 12 15:13:31 2023, max compression
```

## Comparing `tight_loops-0.2.4.tar` & `tight_loops-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:41:32.849717 tight_loops-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-08 17:41:16.000000 tight_loops-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-08 17:41:16.000000 tight_loops-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-08 17:41:32.849717 tight_loops-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-08 17:41:16.000000 tight_loops-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-08 17:41:16.000000 tight_loops-0.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 17:41:32.853717 tight_loops-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-08 17:41:16.000000 tight_loops-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:41:32.849717 tight_loops-0.2.4/tight_loops/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-08 17:41:16.000000 tight_loops-0.2.4/tight_loops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-08 17:41:16.000000 tight_loops-0.2.4/tight_loops/folium_loops.py
--rw-r--r--   0 runner    (1001) docker     (123)    10878 2023-05-08 17:41:16.000000 tight_loops-0.2.4/tight_loops/tight_loops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:41:32.849717 tight_loops-0.2.4/tight_loops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-08 17:41:32.000000 tight_loops-0.2.4/tight_loops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-08 17:41:32.000000 tight_loops-0.2.4/tight_loops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 17:41:32.000000 tight_loops-0.2.4/tight_loops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 17:41:32.000000 tight_loops-0.2.4/tight_loops.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 17:41:32.000000 tight_loops-0.2.4/tight_loops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-08 17:41:32.000000 tight_loops-0.2.4/tight_loops.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:13:31.507151 tight_loops-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-12 15:13:19.000000 tight_loops-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-12 15:13:19.000000 tight_loops-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-12 15:13:31.507151 tight_loops-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-12 15:13:19.000000 tight_loops-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-12 15:13:19.000000 tight_loops-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-12 15:13:31.507151 tight_loops-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-12 15:13:19.000000 tight_loops-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:13:31.507151 tight_loops-0.3.0/tight_loops/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-12 15:13:19.000000 tight_loops-0.3.0/tight_loops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-12 15:13:19.000000 tight_loops-0.3.0/tight_loops/folium_loops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13907 2023-05-12 15:13:19.000000 tight_loops-0.3.0/tight_loops/tight_loops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:13:31.507151 tight_loops-0.3.0/tight_loops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-12 15:13:31.000000 tight_loops-0.3.0/tight_loops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-12 15:13:31.000000 tight_loops-0.3.0/tight_loops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-12 15:13:31.000000 tight_loops-0.3.0/tight_loops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:13:31.000000 tight_loops-0.3.0/tight_loops.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-12 15:13:31.000000 tight_loops-0.3.0/tight_loops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-12 15:13:31.000000 tight_loops-0.3.0/tight_loops.egg-info/top_level.txt
```

### Comparing `tight_loops-0.2.4/LICENSE` & `tight_loops-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tight_loops-0.2.4/PKG-INFO` & `tight_loops-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tight_loops
-Version: 0.2.4
+Version: 0.3.0
 Summary: This is a demo python package for UTK GEOG510
 Home-page: https://github.com/wnelso18/tight_loops
 Author: Will Nelson
 Author-email: wnelso18@vols.utk.edu
 License: MIT license
 Keywords: tight_loops
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `tight_loops-0.2.4/README.md` & `tight_loops-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tight_loops-0.2.4/setup.py` & `tight_loops-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='tight_loops',
     name='tight_loops',
     packages=find_packages(include=['tight_loops', 'tight_loops.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/wnelso18/tight_loops',
-    version='0.2.4',
+    version='0.3.0',
     zip_safe=False,
 )
```

### Comparing `tight_loops-0.2.4/tight_loops/folium_loops.py` & `tight_loops-0.3.0/tight_loops/folium_loops.py`

 * *Files identical despite different names*

### Comparing `tight_loops-0.2.4/tight_loops/tight_loops.py` & `tight_loops-0.3.0/tight_loops/tight_loops.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Main module."""
 
 import random
 import ipyleaflet
 import ipywidgets as widgets
 from ipyleaflet import WidgetControl
+import whitebox as wbt
 
 class Map(ipyleaflet.Map):
     def __init__(self, center=(0,0), zoom=2, **kwargs) -> None:
 
         if "scroll_wheel_zoom" not in kwargs:
             kwargs["scroll_wheel_zoom"] = True
         super().__init__(center=center, zoom=zoom, **kwargs)
@@ -316,21 +317,108 @@
                 tool = grid[i, j]
                 tool.on_click(tool_click)
 
         toolbar_ctrl = ipyleaflet.WidgetControl(widget=toolbar, position=position)
 
         self.add_control(toolbar_ctrl)
 
+from osgeo import gdal, ogr, osr
+import os
+
+def contour_tif(input_file, output_file="new_contours/output_contours.shp", contourInterval=200.0, contourBase=0.0, fixedLevelCount=[], useNoData=False, noDataValue=0, idField=0, elevField=1):
+
+    """
+    This function creates contour lines from a DEM file. The function uses the GDAL library to open the DEM file and
+    extract the elevation values. The function then uses the GDAL library to create a vector file containing the
+    contour lines. The function uses the OGR library to create the vector file and add the contour lines to it.
+
+    :param input_file: The input DEM file.
+    :param output_file: The output vector file containing the contour lines.
+    :param interval: The contour interval.
+    :param base: The base contour.
+    :param fixedLevels: A list of fixed contour levels.
+    :param useNoData: A boolean value indicating whether to use the NoData value.
+    :param useZ: A boolean value indicating whether to use the Z value.
+    :param idField: The field number for the ID field.
+    :param elevField: The field number for the elevation field.
+    """
+
+    # Open the DEM file using the GDAL library
+    input_file = 'Smokies_DEM.tif'
+    ds = gdal.Open(input_file)
+
+    # Get the geotransform information from the DEM
+    transform = ds.GetGeoTransform()
+
+    # Define the output file format and options
+    driver = ogr.GetDriverByName('ESRI Shapefile')
+    output_file = output_file
+    output_dir = os.path.dirname(output_file)
+    if not os.path.exists(output_dir):
+        os.makedirs(output_dir)
+    output_ds = driver.CreateDataSource(output_file)
+
+    # Create the output layer and add a field for elevation values
+    contour_layer = output_ds.CreateLayer('contours', srs=osr.SpatialReference().CloneGeogCS())
+    contour_field = ogr.FieldDefn('elev', ogr.OFTReal)
+    contour_layer.CreateField(contour_field)
+
+
+    band = ds.GetRasterBand(1)
+    gdal.ContourGenerate(
+        band, 
+        contourInterval=contourInterval, 
+        contourBase=contourBase, 
+        fixedLevelCount=fixedLevelCount, 
+        useNoData=useNoData, 
+        noDataValue=noDataValue,
+        dstLayer=contour_layer, 
+        idField=idField, 
+        elevField=elevField
+        )
+    
+
+# ContourGenerate(Band 
+# srcBand, 
+# double contourInterval, 
+# double contourBase, 
+# int fixedLevelCount, 
+# int useNoData, 
+# double noDataValue, 
+# Layer dstLayer, 
+# int idField, 
+# int elevField, 
+# GDALProgressFunc callback=0, 
+# void * callback_data=None) 
+
+
+
+    # Clean up the resources
+    ds = None
+    output_ds = None
+
+
 
 
 
 
 
 
+    # def contour_lines(self, i, output="contour_lines", interval=10.0, base=0.0, smooth=9, tolerance=10.0, callback=None):
 
+    #     wbt.WhiteboxTools.contours_from_raster(
+    #         i, 
+    #         output=output, 
+    #         interval=interval,
+    #         base=base, 
+    #         smooth=smooth, 
+    #         tolerance=tolerance,
+    #         callback=callback
+    #     )
 
+    #     self.add_shp(output)
 
 
 
 # def generate_random_string(length=15):
 #     """Generates a random string."""
 #     return ''.join([random.choice('abcdefghijklmnopqrstuvwxyz') for _ in range(length)])
```

### Comparing `tight_loops-0.2.4/tight_loops.egg-info/PKG-INFO` & `tight_loops-0.3.0/tight_loops.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tight-loops
-Version: 0.2.4
+Version: 0.3.0
 Summary: This is a demo python package for UTK GEOG510
 Home-page: https://github.com/wnelso18/tight_loops
 Author: Will Nelson
 Author-email: wnelso18@vols.utk.edu
 License: MIT license
 Keywords: tight_loops
 Classifier: Development Status :: 2 - Pre-Alpha
```


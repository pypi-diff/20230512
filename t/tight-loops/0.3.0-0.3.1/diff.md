# Comparing `tmp/tight_loops-0.3.0.tar.gz` & `tmp/tight_loops-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tight_loops-0.3.0.tar", last modified: Fri May 12 15:13:31 2023, max compression
+gzip compressed data, was "tight_loops-0.3.1.tar", last modified: Fri May 12 16:18:39 2023, max compression
```

## Comparing `tight_loops-0.3.0.tar` & `tight_loops-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:13:31.507151 tight_loops-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-12 15:13:19.000000 tight_loops-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-12 15:13:19.000000 tight_loops-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-12 15:13:31.507151 tight_loops-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-12 15:13:19.000000 tight_loops-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-12 15:13:19.000000 tight_loops-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-12 15:13:31.507151 tight_loops-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-12 15:13:19.000000 tight_loops-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:13:31.507151 tight_loops-0.3.0/tight_loops/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-12 15:13:19.000000 tight_loops-0.3.0/tight_loops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-12 15:13:19.000000 tight_loops-0.3.0/tight_loops/folium_loops.py
--rw-r--r--   0 runner    (1001) docker     (123)    13907 2023-05-12 15:13:19.000000 tight_loops-0.3.0/tight_loops/tight_loops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:13:31.507151 tight_loops-0.3.0/tight_loops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-12 15:13:31.000000 tight_loops-0.3.0/tight_loops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-12 15:13:31.000000 tight_loops-0.3.0/tight_loops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-12 15:13:31.000000 tight_loops-0.3.0/tight_loops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:13:31.000000 tight_loops-0.3.0/tight_loops.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-12 15:13:31.000000 tight_loops-0.3.0/tight_loops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-12 15:13:31.000000 tight_loops-0.3.0/tight_loops.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:18:39.756499 tight_loops-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-12 16:18:26.000000 tight_loops-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-12 16:18:26.000000 tight_loops-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-12 16:18:39.756499 tight_loops-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-12 16:18:26.000000 tight_loops-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-12 16:18:26.000000 tight_loops-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-12 16:18:39.756499 tight_loops-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-12 16:18:26.000000 tight_loops-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:18:39.752499 tight_loops-0.3.1/tight_loops/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-12 16:18:26.000000 tight_loops-0.3.1/tight_loops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-12 16:18:26.000000 tight_loops-0.3.1/tight_loops/folium_loops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-05-12 16:18:26.000000 tight_loops-0.3.1/tight_loops/tight_loops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:18:39.756499 tight_loops-0.3.1/tight_loops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-12 16:18:39.000000 tight_loops-0.3.1/tight_loops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-12 16:18:39.000000 tight_loops-0.3.1/tight_loops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-12 16:18:39.000000 tight_loops-0.3.1/tight_loops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 16:18:39.000000 tight_loops-0.3.1/tight_loops.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-12 16:18:39.000000 tight_loops-0.3.1/tight_loops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-12 16:18:39.000000 tight_loops-0.3.1/tight_loops.egg-info/top_level.txt
```

### Comparing `tight_loops-0.3.0/LICENSE` & `tight_loops-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tight_loops-0.3.0/PKG-INFO` & `tight_loops-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tight_loops
-Version: 0.3.0
+Version: 0.3.1
 Summary: This is a demo python package for UTK GEOG510
 Home-page: https://github.com/wnelso18/tight_loops
 Author: Will Nelson
 Author-email: wnelso18@vols.utk.edu
 License: MIT license
 Keywords: tight_loops
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `tight_loops-0.3.0/README.md` & `tight_loops-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tight_loops-0.3.0/setup.py` & `tight_loops-0.3.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='tight_loops',
     name='tight_loops',
     packages=find_packages(include=['tight_loops', 'tight_loops.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/wnelso18/tight_loops',
-    version='0.3.0',
+    version='0.3.1',
     zip_safe=False,
 )
```

### Comparing `tight_loops-0.3.0/tight_loops/folium_loops.py` & `tight_loops-0.3.1/tight_loops/folium_loops.py`

 * *Files identical despite different names*

### Comparing `tight_loops-0.3.0/tight_loops/tight_loops.py` & `tight_loops-0.3.1/tight_loops/tight_loops.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Main module."""
 
 import random
 import ipyleaflet
 import ipywidgets as widgets
 from ipyleaflet import WidgetControl
-import whitebox as wbt
 
 class Map(ipyleaflet.Map):
     def __init__(self, center=(0,0), zoom=2, **kwargs) -> None:
 
         if "scroll_wheel_zoom" not in kwargs:
             kwargs["scroll_wheel_zoom"] = True
         super().__init__(center=center, zoom=zoom, **kwargs)
@@ -114,43 +113,64 @@
                 attribution = basemap.attribution
                 self.add_tile_layer(url, name=basemap.name, attribution=attribution, **kwargs)
             except:
                 raise ValueError("Invalid basemap name.")
             
     def add_geojson(self, data, **kwargs):
         """Adds a GeoJSON layer to the map."""
-
-        isinstance(data, str)
         import json
-        with open(data, "r") as f:
-            data = json.load(f)
+
+        if isinstance(data, str):
+        
+            with open(data, "r") as f:
+                data = json.load(f)
+
+        elif not isinstance(data, dict):
+            raise ValueError("data must be a GeoJSON dictionary or a GeoJSON file path.")
 
         geojson = ipyleaflet.GeoJSON(data=data, **kwargs)
         self.add_layer(geojson)
-        return geojson
     
-    def add_shp(self, data, **kwargs):
-        """Adds a Shapefile layer to the map."""
+    # def add_shp(self, data, **kwargs):
+    #     """Adds a Shapefile layer to the map."""
+    #     import geopandas as gpd
+    #     import json
+    #     gdf = gpd.read_file(data)
+    #     data = json.loads(gdf.to_json())
+    #     geojson = ipyleaflet.GeoJSON(data=data, **kwargs)
+    #     self.add_layer(geojson)
+
+    def add_shp(self, data, name='Shapefile', **kwargs):
+        """Adds a Shapefile layer to the map.
+
+        Args:
+            data (str): The path to the Shapefile.
+        """
         import geopandas as gpd
-        import json
+
         gdf = gpd.read_file(data)
-        data = json.loads(gdf.to_json())
-        geojson = ipyleaflet.GeoJSON(data=data, **kwargs)
-        self.add_layer(geojson)
-        return geojson
+        
+        if gdf.crs.to_epsg() != 4326:
+            
+            gdf = gdf.to_crs(epsg=4326)
+            geojson = gdf.__geo_interface__
+        
+        else:
+            geojson = gdf.__geo_interface__
+
+        self.add_geojson(geojson, name=name, **kwargs)
     
     def add_vector(self, data, **kwargs):
         """Adds a vector layer to the map."""
         import geopandas as gpd
         import json
         gdf = gpd.read_file(data)
         data = json.loads(gdf.to_json())
         geojson = ipyleaflet.GeoJSON(data=data, **kwargs)
         self.add_layer(geojson)
-        return geojson
     
     def add_raster(self, url, name='Raster', fit_bounds=True, **kwargs):
         """Adds a raster layer to the map.
 
             Args:
                 url (str): The URL of the raster.
                 name (str): The name of the raster.
@@ -180,19 +200,19 @@
 
         self.add_tile_layer(url=tile, name=name, attribution="raster", **kwargs)
 
         if fit_bounds:
             bbox = [[bounds[1], bounds[0]], [bounds[3], bounds[2]]]
             self.fit_bounds(bbox)
 
-    def add_local_raster(self, filename, name='Local Raster', **kwargs):
-        try:
-            import localtilesserver
-        except ImportError:
-            raise ImportError("Please install localtilesserver: pip install localtilesserver")
+    # def add_local_raster(self, filename, name='Local Raster', **kwargs):
+    #     try:
+    #         import localtilesserver
+    #     except ImportError:
+    #         raise ImportError("Please install localtilesserver: pip install localtilesserver")
         
     def opacity_slider(self, value=0.1, min=0, max=1, position="bottomright"):
         """Adds an opacity slider to the map.
         
         Args:   
             value (float): The initial value of the slider.
             min (float): The minimum value of the slider.
@@ -281,14 +301,15 @@
 
 
 
         output = widgets.Output()
         output_ctrl = WidgetControl(widget=output, position="bottomright")
         self.add_control(output_ctrl)
 
+
         basemap = widgets.Dropdown(
 
             options = ["Satellite", "Roadmap"],
             value = None,
             description = "Basemap",
             style = {"description_width": "initial"},
             layout=widgets.Layout(width="250px")
@@ -317,108 +338,134 @@
                 tool = grid[i, j]
                 tool.on_click(tool_click)
 
         toolbar_ctrl = ipyleaflet.WidgetControl(widget=toolbar, position=position)
 
         self.add_control(toolbar_ctrl)
 
-from osgeo import gdal, ogr, osr
-import os
-
-def contour_tif(input_file, output_file="new_contours/output_contours.shp", contourInterval=200.0, contourBase=0.0, fixedLevelCount=[], useNoData=False, noDataValue=0, idField=0, elevField=1):
-
-    """
-    This function creates contour lines from a DEM file. The function uses the GDAL library to open the DEM file and
-    extract the elevation values. The function then uses the GDAL library to create a vector file containing the
-    contour lines. The function uses the OGR library to create the vector file and add the contour lines to it.
-
-    :param input_file: The input DEM file.
-    :param output_file: The output vector file containing the contour lines.
-    :param interval: The contour interval.
-    :param base: The base contour.
-    :param fixedLevels: A list of fixed contour levels.
-    :param useNoData: A boolean value indicating whether to use the NoData value.
-    :param useZ: A boolean value indicating whether to use the Z value.
-    :param idField: The field number for the ID field.
-    :param elevField: The field number for the elevation field.
-    """
-
-    # Open the DEM file using the GDAL library
-    input_file = 'Smokies_DEM.tif'
-    ds = gdal.Open(input_file)
-
-    # Get the geotransform information from the DEM
-    transform = ds.GetGeoTransform()
-
-    # Define the output file format and options
-    driver = ogr.GetDriverByName('ESRI Shapefile')
-    output_file = output_file
-    output_dir = os.path.dirname(output_file)
-    if not os.path.exists(output_dir):
-        os.makedirs(output_dir)
-    output_ds = driver.CreateDataSource(output_file)
-
-    # Create the output layer and add a field for elevation values
-    contour_layer = output_ds.CreateLayer('contours', srs=osr.SpatialReference().CloneGeogCS())
-    contour_field = ogr.FieldDefn('elev', ogr.OFTReal)
-    contour_layer.CreateField(contour_field)
-
-
-    band = ds.GetRasterBand(1)
-    gdal.ContourGenerate(
-        band, 
-        contourInterval=contourInterval, 
-        contourBase=contourBase, 
-        fixedLevelCount=fixedLevelCount, 
-        useNoData=useNoData, 
-        noDataValue=noDataValue,
-        dstLayer=contour_layer, 
-        idField=idField, 
-        elevField=elevField
-        )
-    
-
-# ContourGenerate(Band 
-# srcBand, 
-# double contourInterval, 
-# double contourBase, 
-# int fixedLevelCount, 
-# int useNoData, 
-# double noDataValue, 
-# Layer dstLayer, 
-# int idField, 
-# int elevField, 
-# GDALProgressFunc callback=0, 
-# void * callback_data=None) 
-
-
-
-    # Clean up the resources
-    ds = None
-    output_ds = None
-
-
-
-
-
-
-
+    def csv_to_shp(self, data, output):
+        import pandas as pd
+        import geopandas as gpd
+        from shapely.geometry import Point
 
-    # def contour_lines(self, i, output="contour_lines", interval=10.0, base=0.0, smooth=9, tolerance=10.0, callback=None):
+        df = pd.read_csv(data)
 
-    #     wbt.WhiteboxTools.contours_from_raster(
-    #         i, 
-    #         output=output, 
-    #         interval=interval,
-    #         base=base, 
-    #         smooth=smooth, 
-    #         tolerance=tolerance,
-    #         callback=callback
-    #     )
+        geometry = [Point(xy) for xy in zip(df.longitude, df.latitude)]
+        gdf = gpd.GeoDataFrame(df, geometry=geometry)
+        gdf = gdf.set_crs(epsg=4326)
+        gdf.to_file(output, driver='ESRI Shapefile')
 
-    #     self.add_shp(output)
+        self.add_shp(output)
+    
 
+    def grouping_points(self, data):
+        import pandas as pd
+        from ipyleaflet import Marker, MarkerCluster
+        import ipywidgets as widgets
+
+        df = pd.read_csv(data)
+
+        markers = []
+
+        for index, row in df.iterrows():
+            name = row['name']
+            latitude = row['latitude']
+            longitude = row['longitude']
+            marker = Marker(location=(latitude, longitude))
+
+            popup_content = widgets.HTML()
+            popup_content.value = f"<b>Name:</b> {name}<br><b>Latitude:</b> {latitude}<br><b>Longitude:</b> {longitude}"
+            marker.popup = popup_content
+
+            markers.append(marker)
+
+
+        marker_cluster = MarkerCluster()
+
+        marker_cluster = MarkerCluster(markers=markers)
+
+        self.add_layer(marker_cluster)
+
+def contour_tif_box(
+    i,
+    output,
+    interval=200,
+    base=0,
+    smooth=9,
+    tolerance=10,
+    ):
+
+    import os
+    import whitebox
+
+    wbt = whitebox.WhiteboxTools()
+
+    i = os.path.abspath(i)
+    output = os.path.abspath(output)
+
+    wbt.contours_from_raster(i=i, output=output, interval=interval, base=base, smooth=smooth, tolerance=tolerance)
+
+# ----------------------------------------------------------------GDAL Contour Function----------------------------------------------------------------
+# from osgeo import gdal, ogr, osr
+# import os
+
+# def contour_tif(input_file, output_file="new_contours/output_contours.shp", contourInterval=200.0, contourBase=0.0, fixedLevelCount=[], useNoData=False, noDataValue=0, idField=0, elevField=1):
+
+#     """
+#     This function creates contour lines from a DEM file. The function uses the GDAL library to open the DEM file and
+#     extract the elevation values. The function then uses the GDAL library to create a vector file containing the
+#     contour lines. The function uses the OGR library to create the vector file and add the contour lines to it.
+
+#     :param input_file: The input DEM file.
+#     :param output_file: The output vector file containing the contour lines.
+#     :param interval: The contour interval.
+#     :param base: The base contour.
+#     :param fixedLevels: A list of fixed contour levels.
+#     :param useNoData: A boolean value indicating whether to use the NoData value.
+#     :param useZ: A boolean value indicating whether to use the Z value.
+#     :param idField: The field number for the ID field.
+#     :param elevField: The field number for the elevation field.
+#     """
+
+#     # Open the DEM file using the GDAL library
+#     input_file = 'Smokies_DEM.tif'
+#     ds = gdal.Open(input_file)
+
+#     # Get the geotransform information from the DEM
+#     transform = ds.GetGeoTransform()
+
+#     # Define the output file format and options
+#     driver = ogr.GetDriverByName('ESRI Shapefile')
+#     output_file = output_file
+#     output_dir = os.path.dirname(output_file)
+#     if not os.path.exists(output_dir):
+#         os.makedirs(output_dir)
+#     output_ds = driver.CreateDataSource(output_file)
+
+#     # Create the output layer and add a field for elevation values
+#     contour_layer = output_ds.CreateLayer('contours', srs=osr.SpatialReference().CloneGeogCS())
+#     contour_field = ogr.FieldDefn('elev', ogr.OFTReal)
+#     contour_layer.CreateField(contour_field)
+
+
+#     band = ds.GetRasterBand(1)
+#     gdal.ContourGenerate(
+#         band, 
+#         contourInterval=contourInterval, 
+#         contourBase=contourBase, 
+#         fixedLevelCount=fixedLevelCount, 
+#         useNoData=useNoData, 
+#         noDataValue=noDataValue,
+#         dstLayer=contour_layer, 
+#         idField=idField, 
+#         elevField=elevField
+#         )
+    
+#     # Clean up the resources
+#     ds = None
+#     output_ds = None
 
+    
 
-# def generate_random_string(length=15):
-#     """Generates a random string."""
-#     return ''.join([random.choice('abcdefghijklmnopqrstuvwxyz') for _ in range(length)])
+def generate_random_string(length=15):
+    """Generates a random string."""
+    return ''.join([random.choice('abcdefghijklmnopqrstuvwxyz') for _ in range(length)])
```

### Comparing `tight_loops-0.3.0/tight_loops.egg-info/PKG-INFO` & `tight_loops-0.3.1/tight_loops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tight-loops
-Version: 0.3.0
+Version: 0.3.1
 Summary: This is a demo python package for UTK GEOG510
 Home-page: https://github.com/wnelso18/tight_loops
 Author: Will Nelson
 Author-email: wnelso18@vols.utk.edu
 License: MIT license
 Keywords: tight_loops
 Classifier: Development Status :: 2 - Pre-Alpha
```


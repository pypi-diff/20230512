# Comparing `tmp/zensvi-0.0.1.tar.gz` & `tmp/zensvi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zensvi-0.0.1.tar", max compression
+gzip compressed data, was "zensvi-0.0.2.tar", max compression
```

## Comparing `zensvi-0.0.1.tar` & `zensvi-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.0.1/LICENSE
--rwxr-xr-x   0        0        0      669 2023-05-10 08:45:06.029273 zensvi-0.0.1/README.md
--rwxr-xr-x   0        0        0      678 2023-05-10 08:49:00.788856 zensvi-0.0.1/pyproject.toml
--rwxr-xr-x   0        0        0      131 2023-05-10 08:45:06.034573 zensvi-0.0.1/src/zensvi/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-10 08:45:06.034772 zensvi-0.0.1/src/zensvi/cv/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-10 08:45:06.034938 zensvi-0.0.1/src/zensvi/cv/segmentation/__init__.py
--rwxr-xr-x   0        0        0    38123 2023-05-10 08:45:06.035269 zensvi-0.0.1/src/zensvi/cv/segmentation/segmentation.py
--rwxr-xr-x   0        0        0       55 2023-05-10 08:45:06.035499 zensvi-0.0.1/src/zensvi/download/__init__.py
--rwxr-xr-x   0        0        0    11935 2023-05-10 08:45:06.036064 zensvi-0.0.1/src/zensvi/download/streetview_downloader.py
--rwxr-xr-x   0        0        0   316244 2023-05-10 08:45:06.037620 zensvi-0.0.1/src/zensvi/download/utils/UserAgent.csv
--rwxr-xr-x   0        0        0        0 2023-05-10 08:45:06.037726 zensvi-0.0.1/src/zensvi/download/utils/__init__.py
--rwxr-xr-x   0        0        0     7531 2023-05-10 08:45:06.037969 zensvi-0.0.1/src/zensvi/download/utils/geoprocess.py
--rwxr-xr-x   0        0        0     1730 2023-05-10 08:45:06.038142 zensvi-0.0.1/src/zensvi/download/utils/get_pids.py
--rwxr-xr-x   0        0        0      956 2023-05-10 08:45:06.038300 zensvi-0.0.1/src/zensvi/download/utils/helpers.py
--rwxr-xr-x   0        0        0     7161 2023-05-10 08:45:06.038542 zensvi-0.0.1/src/zensvi/download/utils/imtool.py
--rwxr-xr-x   0        0        0       30 2023-05-10 08:45:06.038720 zensvi-0.0.1/src/zensvi/transform/__init__.py
--rwxr-xr-x   0        0        0     6500 2023-05-10 08:45:06.038914 zensvi-0.0.1/src/zensvi/transform/transform_image.py
--rwxr-xr-x   0        0        0        0 2023-05-10 08:45:06.038961 zensvi-0.0.1/src/zensvi/zensvi.py
--rw-r--r--   0        0        0     1753 1970-01-01 00:00:00.000000 zensvi-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.0.2/LICENSE
+-rwxr-xr-x   0        0        0      669 2023-05-10 08:45:06.029273 zensvi-0.0.2/README.md
+-rwxr-xr-x   0        0        0      678 2023-05-12 09:34:11.694669 zensvi-0.0.2/pyproject.toml
+-rwxr-xr-x   0        0        0      131 2023-05-10 08:45:06.034573 zensvi-0.0.2/src/zensvi/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-10 08:45:06.034772 zensvi-0.0.2/src/zensvi/cv/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-10 08:45:06.034938 zensvi-0.0.2/src/zensvi/cv/segmentation/__init__.py
+-rwxr-xr-x   0        0        0    38123 2023-05-10 08:45:06.035269 zensvi-0.0.2/src/zensvi/cv/segmentation/segmentation.py
+-rwxr-xr-x   0        0        0       55 2023-05-10 08:45:06.035499 zensvi-0.0.2/src/zensvi/download/__init__.py
+-rwxr-xr-x   0        0        0    12210 2023-05-12 09:26:45.990826 zensvi-0.0.2/src/zensvi/download/streetview_downloader.py
+-rwxr-xr-x   0        0        0   316244 2023-05-10 08:45:06.037620 zensvi-0.0.2/src/zensvi/download/utils/UserAgent.csv
+-rwxr-xr-x   0        0        0        0 2023-05-10 08:45:06.037726 zensvi-0.0.2/src/zensvi/download/utils/__init__.py
+-rwxr-xr-x   0        0        0     7705 2023-05-12 09:26:45.991456 zensvi-0.0.2/src/zensvi/download/utils/geoprocess.py
+-rwxr-xr-x   0        0        0     1730 2023-05-10 08:45:06.038142 zensvi-0.0.2/src/zensvi/download/utils/get_pids.py
+-rwxr-xr-x   0        0        0      956 2023-05-10 08:45:06.038300 zensvi-0.0.2/src/zensvi/download/utils/helpers.py
+-rwxr-xr-x   0        0        0     7161 2023-05-11 09:20:45.913523 zensvi-0.0.2/src/zensvi/download/utils/imtool.py
+-rwxr-xr-x   0        0        0       30 2023-05-10 08:45:06.038720 zensvi-0.0.2/src/zensvi/transform/__init__.py
+-rwxr-xr-x   0        0        0     6500 2023-05-10 08:45:06.038914 zensvi-0.0.2/src/zensvi/transform/transform_image.py
+-rwxr-xr-x   0        0        0        0 2023-05-10 08:45:06.038961 zensvi-0.0.2/src/zensvi/zensvi.py
+-rw-r--r--   0        0        0     1753 1970-01-01 00:00:00.000000 zensvi-0.0.2/PKG-INFO
```

### Comparing `zensvi-0.0.1/LICENSE` & `zensvi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zensvi-0.0.1/README.md` & `zensvi-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `zensvi-0.0.1/pyproject.toml` & `zensvi-0.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zensvi"
-version = "0.0.1"
+version = "0.0.2"
 description = "This package handles downloading, cleaning, analyzing street view imagery in one-stop and zen manner."
 authors = ["koito19960406"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -12,15 +12,15 @@
 geopandas = "^0.9.0"
 geopy = "^2.2.0"
 numpy = "^1.21.2"
 opencv_python = "^4.5.3"
 osmnx = "^1.1.1"
 pandas = "^1.3.3"
 requests = "^2.30.0"
-setuptools = "^58.0.4"
+setuptools = "^67.7.2"
 Shapely = "^1.7.1"
 torch = "^2.0.0"
 tqdm = "^4.62.2"
 transformers = "^4.10.2"
 scipy = "^1.7.1"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `zensvi-0.0.1/src/zensvi/cv/segmentation/segmentation.py` & `zensvi-0.0.2/src/zensvi/cv/segmentation/segmentation.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.0.1/src/zensvi/download/streetview_downloader.py` & `zensvi-0.0.2/src/zensvi/download/streetview_downloader.py`

 * *Files 14% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         user_agent_file = pkg_resources.resource_filename('zensvi.download.utils', 'UserAgent.csv')
         UA = []
         with open(user_agent_file, 'r') as f:
             for line in f:
                 ua = {"user_agent": line.strip()}
                 UA.append(ua)
         return UA
-
+    
     def _read_pids(self, path_pid):
         pid_df = pd.read_csv(path_pid)
         # get unique pids as a list
         pids = pid_df.iloc[:,0].unique().tolist()
         return pids
 
     def _check_already(self, all_panoids):
@@ -133,138 +133,145 @@
                     month = date.split("-")[1]
                 except Exception:
                     year = None
                     month = None
                 return {"year": year, "month": month}
             return {"year": None, "month": None}    
 
-        def worker(index, row):
-            panoid = row['panoid']
+        def worker(row):
+            panoid = row.panoid
             year_month = get_year_month(panoid)
-            return index, year_month
+            return row.Index, year_month
         
         with ThreadPoolExecutor() as executor:
-            futures = {executor.submit(worker, i, row): i for i, row in tqdm(df.iterrows(), total = len(df), desc="Preparing to augment metadata")}
+            futures = {executor.submit(worker, row): row.Index for row in tqdm(df.itertuples(), total = len(df), desc="Preparing to augment metadata")}
             for future in tqdm(as_completed(futures), total=len(futures), desc="Augmenting timestamp metadata"):
                 row_index, year_month = future.result()
                 df.at[row_index, 'year'] = year_month['year']
                 df.at[row_index, 'month'] = year_month['month']
         return df
                     
-    def _get_pids_from_csv(self, input_df, closest=False, disp=False):
+    def _get_pids_from_csv(self, df, id_columns, closest=False, disp=False):
         def get_street_view_info(longitude, latitude):
             results = panoids(latitude, longitude, closest=closest, disp=disp)
             return results
 
         def worker(row):
-            input_longitude = row['longitude']
-            input_latitude = row['latitude']
-            return (input_longitude, input_latitude), get_street_view_info(input_longitude, input_latitude)
+            input_longitude = row.longitude
+            input_latitude = row.latitude
+            return {column: getattr(row, column) for column in id_columns}, (input_longitude, input_latitude), get_street_view_info(input_longitude, input_latitude)
 
         results = []
 
         with ThreadPoolExecutor() as executor:
-            futures = {executor.submit(worker, row): (row['longitude'], row['latitude']) for _, row in tqdm(input_df.iterrows(), total = len(input_df), desc="Preparing to get pids")}
+            futures = {executor.submit(worker, row): row for row in tqdm(df.itertuples(), total=len(df), desc="Preparing to get pids")}
             for future in tqdm(as_completed(futures), total=len(futures), desc="Getting pids"):
-                (input_longitude, input_latitude), row_results = future.result()
+                id_dict, (input_longitude, input_latitude), row_results = future.result()
                 for result in row_results:
                     result['input_longitude'] = input_longitude
                     result['input_latitude'] = input_latitude
+                    result.update(id_dict)
                     results.append(result)
 
         results_df = pd.DataFrame(results)
         return results_df
 
     
-    def _get_pids_from_gdf(self, gdf, closest=False, disp=False):  
-        def get_street_view_info(longitude, latitude):
-            results = panoids(latitude, longitude, closest=closest, disp=disp)
-            return results
-
-        def worker(row):
-            input_longitude = row['longitude']
-            input_latitude = row['latitude']
-            results = get_street_view_info(input_longitude, input_latitude)
-            return (input_longitude, input_latitude), results
-
+    def _get_pids_from_gdf(self, gdf, id_columns, closest=False, disp=False):  
         # read shapefile
-        gp = GeoProcessor(gdf, distance=self.distance, grid=self.grid, grid_size=self.grid_size)
+        gp = GeoProcessor(gdf, distance=self.distance, grid=self.grid, grid_size=self.grid_size, id_columns = id_columns)
         df = gp.get_lat_lon()
-        results = []
 
-        with ThreadPoolExecutor() as executor:
-            futures = {executor.submit(worker, row): (row['longitude'], row['latitude']) for _, row in tqdm(df.iterrows(), total=len(df), desc="Preparing to get pids")}
-            for future in tqdm(as_completed(futures), total=len(futures), desc="Getting pids"):
-                (input_longitude, input_latitude), row_results = future.result()
-                for result in row_results:
-                    result['input_longitude'] = input_longitude
-                    result['input_latitude'] = input_latitude
-                    results.append(result)
-
-        results_df = pd.DataFrame(results)
+        # Use _get_pids_from_csv to get pids from df
+        results_df = self._get_pids_from_csv(df, id_columns, closest=closest, disp=disp)
 
         # Check if lat and lon are within input polygons
         polygons = gpd.GeoSeries([geom for geom in gdf['geometry'] if geom.type in ['Polygon', 'MultiPolygon']])
 
         # Convert lat, lon to Points and create a GeoSeries
         points = gpd.GeoSeries([Point(lon, lat) for lon, lat in zip(results_df['lon'], results_df['lat'])])
 
+        # Create a GeoDataFrame with the points and an index column
+        points_gdf = gpd.GeoDataFrame(geometry=points, crs=gdf.crs)
+        points_gdf['index'] = range(len(points_gdf))
+
+        # Create a spatial index on the polygons GeoSeries
+        polygons_sindex = polygons.sindex
+
+        # Function to check whether a point is within any polygon
+        def is_within_polygon(point):
+            possible_matches_index = list(polygons_sindex.intersection(point.bounds))
+            possible_matches = polygons.iloc[possible_matches_index]
+            precise_matches = possible_matches.contains(point)
+            return precise_matches.any()
+
         # Add progress bar for within_polygon calculation
-        tqdm.pandas(total=len(points), desc="Checking points within polygons")
-        within_polygon = points.progress_apply(lambda point: polygons.contains(point).any())
+        with tqdm(total=len(points), desc="Checking points within polygons") as pbar:
+            within_polygon = []
+            for point in points_gdf['geometry']:
+                within_polygon.append(is_within_polygon(point))
+                pbar.update()
 
         results_df['within_polygon'] = within_polygon
 
         # Return only those points within polygons
         results_within_polygons_df = results_df[results_df['within_polygon']]
         # Drop the 'within_polygon' column
         results_within_polygons_df = results_within_polygons_df.drop(columns='within_polygon')
         return results_within_polygons_df
-    
-    def get_pids(self, path_pid, lat = None, lon = None, input_csv_file = "", input_shp_file = "", buffer = 0, closest=False, disp=False, augment_metadata=False):
+
+    def get_pids(self, path_pid, lat = None, lon = None, input_csv_file = "", input_shp_file = "", id_columns=None, buffer = 0, closest=False, disp=False, augment_metadata=False):
+        if id_columns is not None:
+            if isinstance(id_columns, str):
+                id_columns = [id_columns.lower()]
+            elif isinstance(id_columns, list):
+                id_columns = [column.lower() for column in id_columns]
+        else:
+            id_columns = []
         if lat != None and lon != None:
             pid = panoids(lat, lon, closest=closest, disp=disp)
         elif input_csv_file != "":
             df = pd.read_csv(input_csv_file)
             df = standardize_column_names(df)
             if buffer > 0:
                 gdf = gpd.GeoDataFrame(df, geometry=gpd.points_from_xy(df.longitude, df.latitude), crs='EPSG:4326')
                 gdf = create_buffer_gdf(gdf, buffer)
-                pid = self._get_pids_from_gdf(gdf, closest=closest, disp=disp)
+                pid = self._get_pids_from_gdf(gdf, id_columns, closest=False, disp=False)
             else:
-                pid = self._get_pids_from_csv(df, closest=closest, disp=disp)
+                pid = self._get_pids_from_csv(df, id_columns, closest=False, disp=False)
         elif input_shp_file != "":
             gdf = gpd.read_file(input_shp_file)
             if buffer > 0:
                 gdf = create_buffer_gdf(gdf, buffer)
-            pid = self._get_pids_from_gdf(gdf, closest=closest, disp=disp)
+            pid = self._get_pids_from_gdf(gdf, id_columns, closest=False, disp=False)
         else:
             raise ValueError("Please input the lat and lon, csv file, or shapefile.")
         # save the pids
         pid_df = pd.DataFrame(pid)
         pid_df = pid_df.drop_duplicates(subset='panoid')
         if augment_metadata & (self.gsv_api_key != None):
             pid_df = self._augment_metadata(pid_df)
         elif augment_metadata & (self.gsv_api_key == None):
             raise ValueError("Please set the gsv api key by calling the gsv_api_key method.")
         pid_df.to_csv(path_pid, index=False)
         print("The panorama IDs have been saved to {}".format(path_pid))
     
     def download_gsv(self, dir_output, path_pid = None, zoom=2, h_tiles=4, v_tiles=2, cropped=False, full=True, 
-                lat=None, lon=None, input_csv_file="", input_shp_file = "", buffer = 0, closest=False, disp=False, augment_metadata=False):
+                lat=None, lon=None, input_csv_file="", input_shp_file = "", id_columns=None, buffer = 0, closest=False, disp=False, augment_metadata=False):
         # set dir_output as attribute and create the directory
         self.dir_output = dir_output
         Path(dir_output).mkdir(parents=True, exist_ok=True)
         
-        # If path_pid is None, call get_pids function first
+        # call get_pids function first if path_pid is None
         if path_pid is None:
             print("Getting pids...")
             path_pid = os.path.join(self.dir_output, "pids.csv")
             self.get_pids(path_pid, lat=lat, lon=lon,
-                        input_csv_file=input_csv_file, input_shp_file = input_shp_file, buffer = buffer, closest=closest, disp=disp, augment_metadata=augment_metadata)
+                        input_csv_file=input_csv_file, input_shp_file = input_shp_file, id_columns=id_columns, buffer = buffer, closest=closest, disp=disp, augment_metadata=augment_metadata)
+
 
         # Horizontal Google Street View tiles
         # zoom 3: (8, 4); zoom 5: (26, 13) zoom 2: (4, 2) zoom 1: (2, 1);4:(8,16)
         # zoom = 2
         # h_tiles = 4  # 26
         # v_tiles = 2  # 13
         # cropped = False
```

### Comparing `zensvi-0.0.1/src/zensvi/download/utils/UserAgent.csv` & `zensvi-0.0.2/src/zensvi/download/utils/UserAgent.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.0.1/src/zensvi/download/utils/geoprocess.py` & `zensvi-0.0.2/src/zensvi/download/utils/geoprocess.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,30 +4,32 @@
 import pandas as pd
 from shapely.geometry import Point
 from tqdm.auto import tqdm
 tqdm.pandas()
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor, as_completed
 import numpy as np
 from pyproj import Transformer
+import networkx
 
 class GeoProcessor:
-    def __init__(self, gdf, distance=1, grid = False, grid_size = 20):
+    def __init__(self, gdf, distance=1, grid = False, grid_size = 20, id_columns=[]):
         self.gdf = gdf
         self.distance = distance
         self.processing_functions = {
             'Point': self.process_point,
             'MultiPoint': self.process_multipoint,
             'LineString': self.process_linestring,
             'MultiLineString': self.process_multilinestring,
             'Polygon': self.process_polygon,
             'MultiPolygon': self.process_multipolygon
         }
         self.grid = grid
         self.grid_size = grid_size
         self.utm_crs = None
+        self.id_columns = id_columns
 
     def get_lat_lon(self):
         self.gdf['feature_type'] = self.gdf['geometry'].apply(lambda x: x.geom_type)
         gdf_list = []
 
         for feature_type, func in self.processing_functions.items():
             sub_gdf = self.gdf[self.gdf['feature_type'] == feature_type]
@@ -39,15 +41,15 @@
         result_gdf = pd.concat(gdf_list)
         return result_gdf
 
     # Define other processing functions (process_point, process_multipoint, etc.) as class methods here
     def process_point(self, gdf):
         gdf['longitude'] = gdf.geometry.x
         gdf['latitude'] = gdf.geometry.y
-        return gdf[['longitude', 'latitude']]
+        return gdf[self.id_columns + ['longitude', 'latitude']]
 
     def process_multipoint(self, gdf):
         # Explode the multipoint into individual points
         gdf = gdf.explode('geometry').reset_index(drop=True)
 
         # Call process_point on the exploded GeoDataFrame
         return self.process_point(gdf)
@@ -58,16 +60,16 @@
         self.utm_crs = gdf_utm.crs
 
         # Use osmnx.utils_geo.interpolate_points function to interpolate points along LineStrings
         gdf_utm['sample_points'] = gdf_utm['geometry'].progress_apply(lambda geom: list(ox.utils_geo.interpolate_points(geom, dist=self.distance)), desc="Interpolating Points")
         gdf_utm = gdf_utm.explode('sample_points').reset_index(drop=True)
 
         # Convert the UTM points to latitude and longitude
-        gdf_utm['longitude'], gdf_utm['latitude'] = zip(*self.utm_to_lat_lon(gdf_utm['sample_points'].apply(lambda p: (p.x, p.y)).tolist(), self.utm_crs))
-        return gdf_utm[['longitude', 'latitude']]
+        gdf['longitude'], gdf['latitude'] = zip(*self.utm_to_lat_lon(gdf_utm['sample_points'].apply(lambda p: (p.x, p.y)).tolist(), self.utm_crs))
+        return gdf[self.id_columns + ['longitude', 'latitude']]
 
     def process_multilinestring(self, gdf):
         # Explode the multilinestring into individual linestrings
         gdf = gdf.explode('geometry').reset_index(drop=True)
 
         # Call process_linestring on the exploded GeoDataFrame
         return self.process_linestring(gdf)
@@ -120,45 +122,46 @@
     def utm_to_lat_lon(self, utm_points, utm_crs):
         transformer = Transformer.from_crs(utm_crs, "EPSG:4326", always_xy=True)
         lat_lon_points = [transformer.transform(x, y) for x, y in tqdm(utm_points, desc="Converting UTM to Lat/Lon")]
         return lat_lon_points
 
     def process_polygon(self, gdf):
         with ProcessPoolExecutor() as executor:
-            # Store tuples of (Future, geom) in the futures list
-            futures = []
+            # Use a dictionary to map futures to geoms
+            future_to_geom = {}
+
             for geom in tqdm(gdf.geometry, desc="Preparing Polygons"):
                 if self.grid == False:
                     future = executor.submit(self.get_street_points, geom)
                 else:
                     future = executor.submit(self.create_point_grid, geom, self.grid_size)
-                futures.append((future, geom))
+                future_to_geom[future] = geom
 
             results = []
-            for future in tqdm(as_completed([f[0] for f in futures]), total=len(gdf), desc="Processing Polygons"):
+            for future in tqdm(as_completed(future_to_geom.keys()), total=len(gdf), desc="Processing Polygons"):
                 # Retrieve the corresponding geom for each future
-                geom = next(geom for f, geom in futures if f == future)
+                geom = future_to_geom[future]
                 try:
                     result = future.result()
                     results.append(result)
-                except ValueError:
-                    tqdm.write("Found no graph nodes within the polygon, switching to grid creation.")
+                except (ValueError, networkx.exception.NetworkXPointlessConcept):
+                    tqdm.write("Found no graph nodes within the polygon or connectivity is undefined for the null graph, switching to grid creation.")
                     future = executor.submit(self.create_point_grid, geom, self.grid_size)
                     result = future.result()
                     results.append(result)
 
             gdf['street_points'] = [result[0] for result in results]
             self.utm_crs = results[0][1]
 
         gdf = gdf.explode('street_points').reset_index(drop=True)
 
         # Convert the UTM points to latitude and longitude
         gdf['longitude'], gdf['latitude'] = zip(*self.utm_to_lat_lon(gdf['street_points'].tolist(), self.utm_crs))
 
-        return gdf[['longitude', 'latitude']]
+        return gdf[self.id_columns + ['longitude', 'latitude']]
 
     def process_multipolygon(self, gdf):
         # Explode the multipolygon into individual polygons
         gdf = gdf.explode('geometry').reset_index(drop=True)
 
         # Call process_polygon on the exploded GeoDataFrame
         return self.process_polygon(gdf)
```

### Comparing `zensvi-0.0.1/src/zensvi/download/utils/get_pids.py` & `zensvi-0.0.2/src/zensvi/download/utils/get_pids.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.0.1/src/zensvi/download/utils/helpers.py` & `zensvi-0.0.2/src/zensvi/download/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.0.1/src/zensvi/download/utils/imtool.py` & `zensvi-0.0.2/src/zensvi/download/utils/imtool.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.0.1/src/zensvi/transform/transform_image.py` & `zensvi-0.0.2/src/zensvi/transform/transform_image.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.0.1/PKG-INFO` & `zensvi-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zensvi
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package handles downloading, cleaning, analyzing street view imagery in one-stop and zen manner.
 License: MIT
 Author: koito19960406
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -16,15 +16,15 @@
 Requires-Dist: geopy (>=2.2.0,<3.0.0)
 Requires-Dist: numpy (>=1.21.2,<2.0.0)
 Requires-Dist: opencv_python (>=4.5.3,<5.0.0)
 Requires-Dist: osmnx (>=1.1.1,<2.0.0)
 Requires-Dist: pandas (>=1.3.3,<2.0.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: scipy (>=1.7.1,<2.0.0)
-Requires-Dist: setuptools (>=58.0.4,<59.0.0)
+Requires-Dist: setuptools (>=67.7.2,<68.0.0)
 Requires-Dist: torch (>=2.0.0,<3.0.0)
 Requires-Dist: tqdm (>=4.62.2,<5.0.0)
 Requires-Dist: transformers (>=4.10.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # ZenSVI
```


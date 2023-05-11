# Comparing `tmp/sliderule-3.2.0.tar.gz` & `tmp/sliderule-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliderule-3.2.0.tar", last modified: Mon May  8 12:42:08 2023, max compression
+gzip compressed data, was "sliderule-3.3.0.tar", last modified: Thu May 11 23:51:59 2023, max compression
```

## Comparing `sliderule-3.2.0.tar` & `sliderule-3.3.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:42:08.882824 sliderule-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-05-08 12:41:56.000000 sliderule-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-05-08 12:41:56.000000 sliderule-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-05-08 12:42:08.882824 sliderule-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-05-08 12:41:56.000000 sliderule-3.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-05-08 12:41:56.000000 sliderule-3.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-08 12:42:08.882824 sliderule-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-05-08 12:41:56.000000 sliderule-3.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:42:08.878824 sliderule-3.2.0/sliderule/
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-05-08 12:41:56.000000 sliderule-3.2.0/sliderule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3406 2023-05-08 12:41:56.000000 sliderule-3.2.0/sliderule/arcticdem.py
--rw-r--r--   0 runner    (1001) docker     (122)    24752 2023-05-08 12:41:56.000000 sliderule-3.2.0/sliderule/earthdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18906 2023-05-08 12:41:56.000000 sliderule-3.2.0/sliderule/gedi.py
--rw-r--r--   0 runner    (1001) docker     (122)     9833 2023-05-08 12:41:56.000000 sliderule-3.2.0/sliderule/h5.py
--rw-r--r--   0 runner    (1001) docker     (122)    36209 2023-05-08 12:41:56.000000 sliderule-3.2.0/sliderule/icesat2.py
--rw-r--r--   0 runner    (1001) docker     (122)    38844 2023-05-08 12:41:56.000000 sliderule-3.2.0/sliderule/io.py
--rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-05-08 12:41:56.000000 sliderule-3.2.0/sliderule/ipxapi.py
--rw-r--r--   0 runner    (1001) docker     (122)    85029 2023-05-08 12:41:56.000000 sliderule-3.2.0/sliderule/ipysliderule.py
--rw-r--r--   0 runner    (1001) docker     (122)    44386 2023-05-08 12:41:56.000000 sliderule-3.2.0/sliderule/sliderule.py
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-05-08 12:41:56.000000 sliderule-3.2.0/sliderule/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:42:08.878824 sliderule-3.2.0/sliderule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-05-08 12:42:08.000000 sliderule-3.2.0/sliderule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      950 2023-05-08 12:42:08.000000 sliderule-3.2.0/sliderule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 12:42:08.000000 sliderule-3.2.0/sliderule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-08 12:42:08.000000 sliderule-3.2.0/sliderule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-08 12:42:08.000000 sliderule-3.2.0/sliderule.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:42:08.882824 sliderule-3.2.0/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/big_query.py
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/build_arctic_dem_mosaics_index.py
--rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/build_arctic_dem_mosaics_vrt_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/build_arctic_dem_strips_vrt.py
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/extract_h5_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/icepyx_region.py
--rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/lpdaac_download.py
--rw-r--r--   0 runner    (1001) docker     (122)     6618 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/monitor.py
--rw-r--r--   0 runner    (1001) docker     (122)      922 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/query_cmr.py
--rw-r--r--   0 runner    (1001) docker     (122)      677 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/query_elevations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/query_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/query_photons.py
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/query_stac.py
--rw-r--r--   0 runner    (1001) docker     (122)      612 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/query_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/region_of_interest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/results_to_s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/stac.py
--rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/stream_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/tail_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-05-08 12:41:56.000000 sliderule-3.2.0/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-08 12:41:56.000000 sliderule-3.2.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 23:51:59.088946 sliderule-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-05-11 23:51:48.000000 sliderule-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-05-11 23:51:48.000000 sliderule-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-05-11 23:51:59.088946 sliderule-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-05-11 23:51:48.000000 sliderule-3.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-05-11 23:51:48.000000 sliderule-3.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 23:51:59.088946 sliderule-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-05-11 23:51:48.000000 sliderule-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 23:51:59.084946 sliderule-3.3.0/sliderule/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-05-11 23:51:48.000000 sliderule-3.3.0/sliderule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3406 2023-05-11 23:51:48.000000 sliderule-3.3.0/sliderule/arcticdem.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24752 2023-05-11 23:51:48.000000 sliderule-3.3.0/sliderule/earthdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17509 2023-05-11 23:51:48.000000 sliderule-3.3.0/sliderule/gedi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9833 2023-05-11 23:51:48.000000 sliderule-3.3.0/sliderule/h5.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34861 2023-05-11 23:51:48.000000 sliderule-3.3.0/sliderule/icesat2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38844 2023-05-11 23:51:48.000000 sliderule-3.3.0/sliderule/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-05-11 23:51:48.000000 sliderule-3.3.0/sliderule/ipxapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    85029 2023-05-11 23:51:48.000000 sliderule-3.3.0/sliderule/ipysliderule.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6249 2023-05-11 23:51:48.000000 sliderule-3.3.0/sliderule/raster.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45777 2023-05-11 23:51:48.000000 sliderule-3.3.0/sliderule/sliderule.py
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-05-11 23:51:48.000000 sliderule-3.3.0/sliderule/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 23:51:59.084946 sliderule-3.3.0/sliderule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-05-11 23:51:59.000000 sliderule-3.3.0/sliderule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      970 2023-05-11 23:51:59.000000 sliderule-3.3.0/sliderule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 23:51:59.000000 sliderule-3.3.0/sliderule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-11 23:51:59.000000 sliderule-3.3.0/sliderule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-11 23:51:59.000000 sliderule-3.3.0/sliderule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 23:51:59.088946 sliderule-3.3.0/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/big_query.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/build_arctic_dem_mosaics_index.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/build_arctic_dem_mosaics_vrt_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/build_arctic_dem_strips_vrt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/extract_h5_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/icepyx_region.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/lpdaac_download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6618 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      922 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/query_cmr.py
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/query_elevations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/query_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/query_photons.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/query_stac.py
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/query_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/region_of_interest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/results_to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/stac.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/stream_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/tail_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-05-11 23:51:48.000000 sliderule-3.3.0/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-11 23:51:48.000000 sliderule-3.3.0/version.txt
```

### Comparing `sliderule-3.2.0/LICENSE` & `sliderule-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/PKG-INFO` & `sliderule-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 3.2.0
+Version: 3.3.0
 Summary: Python client for interacting with sliderule server
 Home-page: https://github.com/ICESat2-SlideRule/sliderule-python/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sliderule-3.2.0/README.md` & `sliderule-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/setup.py` & `sliderule-3.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/sliderule/arcticdem.py` & `sliderule-3.3.0/sliderule/arcticdem.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/sliderule/earthdata.py` & `sliderule-3.3.0/sliderule/earthdata.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/sliderule/gedi.py` & `sliderule-3.3.0/sliderule/gedi.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,60 +56,14 @@
 ALL_BEAMS = -1
 
 ###############################################################################
 # LOCAL FUNCTIONS
 ###############################################################################
 
 #
-#  Dictionary to GeoDataFrame
-#
-def __todataframe(columns, time_key="time", lon_key="longitude", lat_key="latitude", **kwargs):
-
-    # Latch Start Time
-    tstart = time.perf_counter()
-
-    # Set Default Keyword Arguments
-    kwargs['index_key'] = "time"
-    kwargs['crs'] = sliderule.EPSG_MERCATOR
-
-    # Check Empty Columns
-    if len(columns) <= 0:
-        return sliderule.emptyframe(**kwargs)
-
-    # Generate Time Column
-    columns['time'] = columns[time_key].astype('datetime64[ns]')
-
-    # Generate Geometry Column
-    geometry = geopandas.points_from_xy(columns[lon_key], columns[lat_key])
-    del columns[lon_key]
-    del columns[lat_key]
-
-    # Create Pandas DataFrame object
-    if type(columns) == dict:
-        df = geopandas.pd.DataFrame(columns)
-    else:
-        df = columns
-
-    # Build GeoDataFrame (default geometry is crs=EPSG_MERCATOR)
-    gdf = geopandas.GeoDataFrame(df, geometry=geometry, crs=kwargs['crs'])
-
-    # Set index (default is Timestamp), can add `verify_integrity=True` to check for duplicates
-    # Can do this during DataFrame creation, but this allows input argument for desired column
-    gdf.set_index(kwargs['index_key'], inplace=True)
-
-    # Sort values for reproducible output despite async processing
-    gdf.sort_index(inplace=True)
-
-    # Update Profile
-    profiles[__todataframe.__name__] = time.perf_counter() - tstart
-
-    # Return GeoDataFrame
-    return gdf
-
-#
 # Flatten Batches
 #
 def __flattenbatches(rsps, rectype, batch_column, parm, keep_id):
 
     # Latch Start Time
     tstart_flatten = time.perf_counter()
 
@@ -178,15 +132,15 @@
                     for field in columns:
                         columns[field][cnt] = batch[field]
                     cnt += 1
     else:
         logger.debug("No response returned")
 
     # Build Initial GeoDataFrame
-    gdf = __todataframe(columns)
+    gdf = sliderule.todataframe(columns)
 
     # Merge Ancillary Fields
     tstart_merge = time.perf_counter()
     for field_set in field_dictionary:
         df = geopandas.pd.DataFrame(field_dictionary[field_set])
         gdf = geopandas.pd.merge(gdf, df, how='left', on='shot_number').set_axis(gdf.index)
     profiles["merge"] = time.perf_counter() - tstart_merge
@@ -235,15 +189,15 @@
     if kwargs['return_metadata']:
         resources,metadata = earthdata.cmr(short_name=dataset, **kwargs)
     else:
         resources = earthdata.cmr(short_name=dataset, **kwargs)
 
     # Check Resources are Under Limit
     if(len(resources) > earthdata.max_requested_resources):
-        raise sliderule.FatalError('Exceeded maximum requested granules: {} (current max is {})\nConsider using icesat2.set_max_resources to set a higher limit.'.format(len(resources), max_requested_resources))
+        raise sliderule.FatalError('Exceeded maximum requested granules: {} (current max is {})\nConsider using icesat2.set_max_resources to set a higher limit.'.format(len(resources), earthdata.max_requested_resources))
     else:
         logger.info("Identified %d resources to process", len(resources))
 
     # Update Profile
     profiles[__query_resources.__name__] = time.perf_counter() - tstart
 
     # Return Resources
```

### Comparing `sliderule-3.2.0/sliderule/h5.py` & `sliderule-3.3.0/sliderule/h5.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/sliderule/icesat2.py` & `sliderule-3.3.0/sliderule/icesat2.py`

 * *Files 4% similar despite different names*

```diff
@@ -133,60 +133,14 @@
             elif pair == RIGHT_PAIR:
                 return 1
 
     # unknown spot
     return 0
 
 #
-#  Dictionary to GeoDataFrame
-#
-def __todataframe(columns, time_key="time", lon_key="lon", lat_key="lat", **kwargs):
-
-    # Latch Start Time
-    tstart = time.perf_counter()
-
-    # Set Default Keyword Arguments
-    kwargs['index_key'] = "time"
-    kwargs['crs'] = sliderule.EPSG_MERCATOR
-
-    # Check Empty Columns
-    if len(columns) <= 0:
-        return sliderule.emptyframe(**kwargs)
-
-    # Generate Time Column
-    columns['time'] = columns[time_key].astype('datetime64[ns]')
-
-    # Generate Geometry Column
-    geometry = geopandas.points_from_xy(columns[lon_key], columns[lat_key])
-    del columns[lon_key]
-    del columns[lat_key]
-
-    # Create Pandas DataFrame object
-    if type(columns) == dict:
-        df = geopandas.pd.DataFrame(columns)
-    else:
-        df = columns
-
-    # Build GeoDataFrame (default geometry is crs=EPSG_MERCATOR)
-    gdf = geopandas.GeoDataFrame(df, geometry=geometry, crs=kwargs['crs'])
-
-    # Set index (default is Timestamp), can add `verify_integrity=True` to check for duplicates
-    # Can do this during DataFrame creation, but this allows input argument for desired column
-    gdf.set_index(kwargs['index_key'], inplace=True)
-
-    # Sort values for reproducible output despite async processing
-    gdf.sort_index(inplace=True)
-
-    # Update Profile
-    profiles[__todataframe.__name__] = time.perf_counter() - tstart
-
-    # Return GeoDataFrame
-    return gdf
-
-#
 # Flatten Batches
 #
 def __flattenbatches(rsps, rectype, batch_column, parm, keep_id):
 
     # Latch Start Time
     tstart_flatten = time.perf_counter()
 
@@ -282,15 +236,15 @@
                     for field in columns:
                         columns[field][cnt] = batch[field]
                     cnt += 1
     else:
         logger.debug("No response returned")
 
     # Build Initial GeoDataFrame
-    gdf = __todataframe(columns)
+    gdf = sliderule.todataframe(columns, lon_key='lon', lat_key='lat')
 
     # Merge Ancillary Fields
     tstart_merge = time.perf_counter()
     for field_set in field_dictionary:
         df = geopandas.pd.DataFrame(field_dictionary[field_set])
         gdf = geopandas.pd.merge(gdf, df, how='left', on='extent_id').set_axis(gdf.index)
     profiles["merge"] = time.perf_counter() - tstart_merge
@@ -356,15 +310,15 @@
     if kwargs['return_metadata']:
         resources,metadata = earthdata.cmr(short_name='ATL03', version=version, **kwargs)
     else:
         resources = earthdata.cmr(short_name='ATL03', version=version, **kwargs)
 
     # Check Resources are Under Limit
     if(len(resources) > earthdata.max_requested_resources):
-        raise sliderule.FatalError('Exceeded maximum requested granules: {} (current max is {})\nConsider using cmr.set_max_resources to set a higher limit.'.format(len(resources), max_requested_resources))
+        raise sliderule.FatalError('Exceeded maximum requested granules: {} (current max is {})\nConsider using cmr.set_max_resources to set a higher limit.'.format(len(resources), earthdata.max_requested_resources))
     else:
         logger.info("Identified %d resources to process", len(resources))
 
     # Update Profile
     profiles[__query_resources.__name__] = time.perf_counter() - tstart
 
     # Return Resources
@@ -695,15 +649,15 @@
                     if "extent_id" in columns and not keep_id:
                         del columns["extent_id"]
 
                     # Capture Time to Flatten
                     profiles["flatten"] = time.perf_counter() - tstart_flatten
 
                     # Create DataFrame
-                    gdf = __todataframe(columns, lat_key="latitude", lon_key="longitude")
+                    gdf = sliderule.todataframe(columns, lat_key="latitude", lon_key="longitude")
 
                     # Calculate Spot Column
                     gdf['spot'] = gdf.apply(lambda row: __calcspot(row["sc_orient"], row["track"], row["pair"]), axis=1)
 
                     # Return Response
                     profiles[atl03sp.__name__] = time.perf_counter() - tstart
                     return gdf
```

### Comparing `sliderule-3.2.0/sliderule/io.py` & `sliderule-3.3.0/sliderule/io.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/sliderule/ipxapi.py` & `sliderule-3.3.0/sliderule/ipxapi.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/sliderule/ipysliderule.py` & `sliderule-3.3.0/sliderule/ipysliderule.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/sliderule/sliderule.py` & `sliderule-3.3.0/sliderule/sliderule.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 ps_access_token = None
 ps_token_exp = None
 
 MAX_PS_CLUSTER_WAIT_SECS = 600
 
 verbose = False
 
-request_timeout = (10, 60) # (connection, read) in seconds
+request_timeout = (10, 120) # (connection, read) in seconds
 
 logger = logging.getLogger(__name__)
 
 clustering_enabled = False
 try:
     from sklearn.cluster import KMeans
     clustering_enabled = True
@@ -537,14 +537,59 @@
     datatype = basictypes[codedtype2str[dtype]]["nptype"]
     num_elements = int(size / numpy.dtype(datatype).itemsize)
     slicesize = num_elements * numpy.dtype(datatype).itemsize # truncates partial bytes
     values = numpy.frombuffer(raw[:slicesize], dtype=datatype, count=num_elements)
 
     return values
 
+#
+#  Dictionary to GeoDataFrame
+#
+def todataframe(columns, time_key="time", lon_key="longitude", lat_key="latitude", **kwargs):
+
+    # Latch Start Time
+    tstart = time.perf_counter()
+
+    # Set Default Keyword Arguments
+    kwargs['index_key'] = "time"
+    kwargs['crs'] = EPSG_MERCATOR
+
+    # Check Empty Columns
+    if len(columns) <= 0:
+        return emptyframe(**kwargs)
+
+    # Generate Time Column
+    columns['time'] = columns[time_key].astype('datetime64[ns]')
+
+    # Generate Geometry Column
+    geometry = geopandas.points_from_xy(columns[lon_key], columns[lat_key])
+    del columns[lon_key]
+    del columns[lat_key]
+
+    # Create Pandas DataFrame object
+    if type(columns) == dict:
+        df = geopandas.pd.DataFrame(columns)
+    else:
+        df = columns
+
+    # Build GeoDataFrame (default geometry is crs=EPSG_MERCATOR)
+    gdf = geopandas.GeoDataFrame(df, geometry=geometry, crs=kwargs['crs'])
+
+    # Set index (default is Timestamp), can add `verify_integrity=True` to check for duplicates
+    # Can do this during DataFrame creation, but this allows input argument for desired column
+    gdf.set_index(kwargs['index_key'], inplace=True)
+
+    # Sort values for reproducible output despite async processing
+    gdf.sort_index(inplace=True)
+
+    # Update Profile
+    profiles[todataframe.__name__] = time.perf_counter() - tstart
+
+    # Return GeoDataFrame
+    return gdf
 
 ###############################################################################
 # APIs
 ###############################################################################
 
 #
 #  Initialize
```

### Comparing `sliderule-3.2.0/sliderule.egg-info/PKG-INFO` & `sliderule-3.3.0/sliderule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 3.2.0
+Version: 3.3.0
 Summary: Python client for interacting with sliderule server
 Home-page: https://github.com/ICESat2-SlideRule/sliderule-python/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sliderule-3.2.0/sliderule.egg-info/SOURCES.txt` & `sliderule-3.3.0/sliderule.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 sliderule/earthdata.py
 sliderule/gedi.py
 sliderule/h5.py
 sliderule/icesat2.py
 sliderule/io.py
 sliderule/ipxapi.py
 sliderule/ipysliderule.py
+sliderule/raster.py
 sliderule/sliderule.py
 sliderule/version.py
 sliderule.egg-info/PKG-INFO
 sliderule.egg-info/SOURCES.txt
 sliderule.egg-info/dependency_links.txt
 sliderule.egg-info/requires.txt
 sliderule.egg-info/top_level.txt
```

### Comparing `sliderule-3.2.0/utils/big_query.py` & `sliderule-3.3.0/utils/big_query.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/utils/build_arctic_dem_mosaics_index.py` & `sliderule-3.3.0/utils/build_arctic_dem_mosaics_index.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/utils/build_arctic_dem_mosaics_vrt_list.py` & `sliderule-3.3.0/utils/build_arctic_dem_mosaics_vrt_list.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/utils/build_arctic_dem_strips_vrt.py` & `sliderule-3.3.0/utils/build_arctic_dem_strips_vrt.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/utils/extract_h5_dataset.py` & `sliderule-3.3.0/utils/extract_h5_dataset.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/utils/icepyx_region.py` & `sliderule-3.3.0/utils/icepyx_region.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/utils/lpdaac_download.py` & `sliderule-3.3.0/utils/lpdaac_download.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/utils/monitor.py` & `sliderule-3.3.0/utils/monitor.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/utils/query_cmr.py` & `sliderule-3.3.0/utils/query_cmr.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/utils/query_elevations.py` & `sliderule-3.3.0/utils/query_elevations.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/utils/query_metrics.py` & `sliderule-3.3.0/utils/query_metrics.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/utils/query_photons.py` & `sliderule-3.3.0/utils/query_photons.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/utils/query_stac.py` & `sliderule-3.3.0/utils/query_stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/utils/query_version.py` & `sliderule-3.3.0/utils/query_version.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/utils/region_of_interest.py` & `sliderule-3.3.0/utils/region_of_interest.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/utils/results_to_s3.py` & `sliderule-3.3.0/utils/results_to_s3.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/utils/stac.py` & `sliderule-3.3.0/utils/stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/utils/stream_events.py` & `sliderule-3.3.0/utils/stream_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/utils/tail_events.py` & `sliderule-3.3.0/utils/tail_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.2.0/utils/utils.py` & `sliderule-3.3.0/utils/utils.py`

 * *Files identical despite different names*


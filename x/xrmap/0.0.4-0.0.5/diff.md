# Comparing `tmp/xrmap-0.0.4.tar.gz` & `tmp/xrmap-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrmap-0.0.4.tar", last modified: Fri Apr 28 08:23:15 2023, max compression
+gzip compressed data, was "xrmap-0.0.5.tar", last modified: Fri May 12 07:37:11 2023, max compression
```

## Comparing `xrmap-0.0.4.tar` & `xrmap-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-28 08:23:15.533902 xrmap-0.0.4/
--rw-r--r--   0 javier     (501) staff       (20)      939 2023-04-28 08:23:15.534581 xrmap-0.0.4/PKG-INFO
--rw-r--r--   0 javier     (501) staff       (20)     1066 2023-04-28 08:23:15.538452 xrmap-0.0.4/setup.cfg
--rw-r--r--   0 javier     (501) staff       (20)      102 2023-04-26 13:39:17.000000 xrmap-0.0.4/setup.py
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-28 08:23:15.522502 xrmap-0.0.4/xarray_map/
--rw-r--r--   0 javier     (501) staff       (20)      112 2023-04-26 13:19:23.000000 xrmap-0.0.4/xarray_map/__init__.py
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-28 08:23:15.522814 xrmap-0.0.4/xarray_map/kmz/
--rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-26 11:34:33.000000 xrmap-0.0.4/xarray_map/kmz/__init__.py
--rw-r--r--   0 javier     (501) staff       (20)     1306 2023-04-26 13:46:32.000000 xrmap-0.0.4/xarray_map/plot_folium.py
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-28 08:23:15.533224 xrmap-0.0.4/xrmap.egg-info/
--rw-r--r--   0 javier     (501) staff       (20)      939 2023-04-28 08:23:15.000000 xrmap-0.0.4/xrmap.egg-info/PKG-INFO
--rw-r--r--   0 javier     (501) staff       (20)      266 2023-04-28 08:23:15.000000 xrmap-0.0.4/xrmap.egg-info/SOURCES.txt
--rw-r--r--   0 javier     (501) staff       (20)        1 2023-04-28 08:23:15.000000 xrmap-0.0.4/xrmap.egg-info/dependency_links.txt
--rw-r--r--   0 javier     (501) staff       (20)        1 2023-04-28 08:20:56.000000 xrmap-0.0.4/xrmap.egg-info/not-zip-safe
--rw-r--r--   0 javier     (501) staff       (20)       31 2023-04-28 08:23:15.000000 xrmap-0.0.4/xrmap.egg-info/requires.txt
--rw-r--r--   0 javier     (501) staff       (20)       11 2023-04-28 08:23:15.000000 xrmap-0.0.4/xrmap.egg-info/top_level.txt
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-05-12 07:37:11.631015 xrmap-0.0.5/
+-rw-r--r--   0 javier     (501) staff       (20)      939 2023-05-12 07:37:11.631158 xrmap-0.0.5/PKG-INFO
+-rw-r--r--   0 javier     (501) staff       (20)     1066 2023-05-12 07:37:11.632674 xrmap-0.0.5/setup.cfg
+-rw-r--r--   0 javier     (501) staff       (20)      102 2023-04-26 13:39:17.000000 xrmap-0.0.5/setup.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-05-12 07:37:11.625753 xrmap-0.0.5/xarray_map/
+-rw-r--r--   0 javier     (501) staff       (20)      112 2023-04-26 13:19:23.000000 xrmap-0.0.5/xarray_map/__init__.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-05-12 07:37:11.626511 xrmap-0.0.5/xarray_map/kmz/
+-rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-26 11:34:33.000000 xrmap-0.0.5/xarray_map/kmz/__init__.py
+-rw-r--r--   0 javier     (501) staff       (20)     1404 2023-05-12 07:36:47.000000 xrmap-0.0.5/xarray_map/plot_folium.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-05-12 07:37:11.630617 xrmap-0.0.5/xrmap.egg-info/
+-rw-r--r--   0 javier     (501) staff       (20)      939 2023-05-12 07:37:11.000000 xrmap-0.0.5/xrmap.egg-info/PKG-INFO
+-rw-r--r--   0 javier     (501) staff       (20)      266 2023-05-12 07:37:11.000000 xrmap-0.0.5/xrmap.egg-info/SOURCES.txt
+-rw-r--r--   0 javier     (501) staff       (20)        1 2023-05-12 07:37:11.000000 xrmap-0.0.5/xrmap.egg-info/dependency_links.txt
+-rw-r--r--   0 javier     (501) staff       (20)        1 2023-04-28 08:20:56.000000 xrmap-0.0.5/xrmap.egg-info/not-zip-safe
+-rw-r--r--   0 javier     (501) staff       (20)       31 2023-05-12 07:37:11.000000 xrmap-0.0.5/xrmap.egg-info/requires.txt
+-rw-r--r--   0 javier     (501) staff       (20)       11 2023-05-12 07:37:11.000000 xrmap-0.0.5/xrmap.egg-info/top_level.txt
```

### Comparing `xrmap-0.0.4/PKG-INFO` & `xrmap-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xrmap
-Version: 0.0.4
+Version: 0.0.5
 Summary: Plot xarrays lat-lon datasets using folium
 Home-page: https://github.com/javiergvaldecasas/xarray-map
 Author: Javier García-Valdecasas
 Author-email: garciavaldecasas@oritiayboreas.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `xrmap-0.0.4/setup.cfg` & `xrmap-0.0.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = xrmap
-version = 0.0.4
+version = 0.0.5
 author = Javier García-Valdecasas
 author_email = garciavaldecasas@oritiayboreas.com
 license = Apache-2.0
 description = Plot xarrays lat-lon datasets using folium
 long_description_content_type = text/x-rst
 long_description = Plot xarrays lat-lon datasets using folium
 url = https://github.com/javiergvaldecasas/xarray-map
```

### Comparing `xrmap-0.0.4/xarray_map/plot_folium.py` & `xrmap-0.0.5/xarray_map/plot_folium.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 import folium
 import matplotlib.pyplot as plt
 
 
 def plot_folium(self, m: folium.Map, colormap: str = 'viridis',
-                opacity: float = 0.6, vmax: float = None, vmin: float = None):
+                opacity: float = 0.6, vmax: float = None, vmin: float = None,
+                x=None, y=None):
     """
 
     :param self:
     :param m:
     :param colormap:
     :param opacity:
     :param vmax:
@@ -18,16 +19,18 @@
     if vmax is None:
         vmax = self.values[:].max()
     if vmin is None:
         vmin = self.values[:].min()
 
     values = np.flipud(self.values[:].astype(float))
     values = (values - vmin) / (vmax - vmin)
-
-    if 'latitude' in self.dims and 'longitude' in self.dims:
+    if x is not None:
+        latitude = x
+        longitude = y
+    elif 'latitude' in self.dims and 'longitude' in self.dims:
         latitude = self.latitude
         longitude = self.longitude
     elif 'lat' in self.dims:
         latitude = self.lat
         longitude = self.lon
     else:
         raise ValueError('dimensions: latitude or lat ')
```

### Comparing `xrmap-0.0.4/xrmap.egg-info/PKG-INFO` & `xrmap-0.0.5/xrmap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xrmap
-Version: 0.0.4
+Version: 0.0.5
 Summary: Plot xarrays lat-lon datasets using folium
 Home-page: https://github.com/javiergvaldecasas/xarray-map
 Author: Javier García-Valdecasas
 Author-email: garciavaldecasas@oritiayboreas.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```


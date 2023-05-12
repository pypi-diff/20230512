# Comparing `tmp/xdatasets-0.2.6.tar.gz` & `tmp/xdatasets-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdatasets-0.2.6.tar", last modified: Tue May  9 16:35:56 2023, max compression
+gzip compressed data, was "xdatasets-0.2.7.tar", last modified: Fri May 12 02:27:58 2023, max compression
```

## Comparing `xdatasets-0.2.6.tar` & `xdatasets-0.2.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:35:56.370160 xdatasets-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-09 16:35:49.000000 xdatasets-0.2.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-09 16:35:49.000000 xdatasets-0.2.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-09 16:35:49.000000 xdatasets-0.2.6/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-09 16:35:49.000000 xdatasets-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-09 16:35:49.000000 xdatasets-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-09 16:35:56.370160 xdatasets-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-09 16:35:49.000000 xdatasets-0.2.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-09 16:35:56.370160 xdatasets-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-09 16:35:49.000000 xdatasets-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:35:56.370160 xdatasets-0.2.6/xdatasets/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-09 16:35:49.000000 xdatasets-0.2.6/xdatasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-05-09 16:35:49.000000 xdatasets-0.2.6/xdatasets/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-09 16:35:49.000000 xdatasets-0.2.6/xdatasets/scripting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-09 16:35:49.000000 xdatasets-0.2.6/xdatasets/spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-09 16:35:49.000000 xdatasets-0.2.6/xdatasets/temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-09 16:35:49.000000 xdatasets-0.2.6/xdatasets/tutorial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-09 16:35:49.000000 xdatasets-0.2.6/xdatasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-09 16:35:49.000000 xdatasets-0.2.6/xdatasets/validations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-05-09 16:35:49.000000 xdatasets-0.2.6/xdatasets/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:35:56.370160 xdatasets-0.2.6/xdatasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-09 16:35:56.000000 xdatasets-0.2.6/xdatasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-09 16:35:56.000000 xdatasets-0.2.6/xdatasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:35:56.000000 xdatasets-0.2.6/xdatasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:35:56.000000 xdatasets-0.2.6/xdatasets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-09 16:35:56.000000 xdatasets-0.2.6/xdatasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 16:35:56.000000 xdatasets-0.2.6/xdatasets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:27:58.765426 xdatasets-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-12 02:27:50.000000 xdatasets-0.2.7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-12 02:27:50.000000 xdatasets-0.2.7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-12 02:27:50.000000 xdatasets-0.2.7/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-12 02:27:50.000000 xdatasets-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-12 02:27:50.000000 xdatasets-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-12 02:27:58.765426 xdatasets-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-12 02:27:50.000000 xdatasets-0.2.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-12 02:27:58.769427 xdatasets-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-12 02:27:51.000000 xdatasets-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:27:58.765426 xdatasets-0.2.7/xdatasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-12 02:27:51.000000 xdatasets-0.2.7/xdatasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-05-12 02:27:51.000000 xdatasets-0.2.7/xdatasets/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-12 02:27:51.000000 xdatasets-0.2.7/xdatasets/scripting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-12 02:27:51.000000 xdatasets-0.2.7/xdatasets/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-12 02:27:51.000000 xdatasets-0.2.7/xdatasets/temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-12 02:27:51.000000 xdatasets-0.2.7/xdatasets/tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-12 02:27:51.000000 xdatasets-0.2.7/xdatasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-12 02:27:51.000000 xdatasets-0.2.7/xdatasets/validations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-05-12 02:27:51.000000 xdatasets-0.2.7/xdatasets/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:27:58.765426 xdatasets-0.2.7/xdatasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-12 02:27:58.000000 xdatasets-0.2.7/xdatasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-12 02:27:58.000000 xdatasets-0.2.7/xdatasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 02:27:58.000000 xdatasets-0.2.7/xdatasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 02:27:58.000000 xdatasets-0.2.7/xdatasets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-12 02:27:58.000000 xdatasets-0.2.7/xdatasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-12 02:27:58.000000 xdatasets-0.2.7/xdatasets.egg-info/top_level.txt
```

### Comparing `xdatasets-0.2.6/CONTRIBUTING.rst` & `xdatasets-0.2.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.6/LICENSE` & `xdatasets-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.6/PKG-INFO` & `xdatasets-0.2.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdatasets
-Version: 0.2.6
+Version: 0.2.7
 Summary: Easy acess to earth observation datasets with xarray.
 Home-page: https://github.com/hydrologie/xdatasets'
 Author: Sebastien Langlois
 Author-email: sebastien.langlois62@gmail.com
 License: MIT license
 Keywords: xdatasets hydrology meteorology climate climatology netcdf gridded analysis
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `xdatasets-0.2.6/README.rst` & `xdatasets-0.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.6/setup.py` & `xdatasets-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,10 +72,10 @@
     long_description_content_type="text/x-rst",
     include_package_data=True,
     keywords=KEYWORDS,
     name=NAME,
     packages=find_packages(),
     extras_require={"dev": dev_requirements},
     url=URL,
-    version='0.2.6',
+    version='0.2.7',
     zip_safe=False,
 )
```

### Comparing `xdatasets-0.2.6/xdatasets/core.py` & `xdatasets-0.2.7/xdatasets/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import xarray as xr
 import hvplot.xarray
 import hvplot.pandas
 
 from .validations import _validate_space_params
 from .workflows import climate_request, hydrometric_request, user_provided_dataset
 from .scripting import LOGGING_CONFIG
+from .utils import cache_catalog
 
 logging.config.dictConfig(LOGGING_CONFIG)
 logger = logging.getLogger(__name__)
 
 url_path = 'https://raw.githubusercontent.com/hydrocloudservices/catalogs/main/catalogs/main.yaml'
 
 
@@ -106,14 +107,16 @@
     def __init__(self,
                  datasets: Union[str, List[str], Dict[str, Union[str, List[str]]]],
                  space: Dict[str, Union[str, List[str]]] = dict(),
                  time: Dict[str, Union[str, List[str]]] = dict(),
                  catalog_path: str = url_path
                  )-> None:
 
+        catalog_path = cache_catalog(catalog_path)
+
         self.catalog = intake.open_catalog(catalog_path)
         self.datasets = datasets
         self.space = self._resolve_space_params(**space)
         self.time = self._resolve_time_params(**time)
         
         self.load_query(datasets=self.datasets,
                         space=self.space,
```

### Comparing `xdatasets-0.2.6/xdatasets/scripting.py` & `xdatasets-0.2.7/xdatasets/scripting.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.6/xdatasets/spatial.py` & `xdatasets-0.2.7/xdatasets/spatial.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.6/xdatasets/temporal.py` & `xdatasets-0.2.7/xdatasets/temporal.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.6/xdatasets/tutorial.py` & `xdatasets-0.2.7/xdatasets/tutorial.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.6/xdatasets/validations.py` & `xdatasets-0.2.7/xdatasets/validations.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.6/xdatasets/workflows.py` & `xdatasets-0.2.7/xdatasets/workflows.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.6/xdatasets.egg-info/PKG-INFO` & `xdatasets-0.2.7/xdatasets.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdatasets
-Version: 0.2.6
+Version: 0.2.7
 Summary: Easy acess to earth observation datasets with xarray.
 Home-page: https://github.com/hydrologie/xdatasets'
 Author: Sebastien Langlois
 Author-email: sebastien.langlois62@gmail.com
 License: MIT license
 Keywords: xdatasets hydrology meteorology climate climatology netcdf gridded analysis
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `xdatasets-0.2.6/xdatasets.egg-info/requires.txt` & `xdatasets-0.2.7/xdatasets.egg-info/requires.txt`

 * *Files identical despite different names*


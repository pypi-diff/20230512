# Comparing `tmp/atmoswing-toolbox-1.3.4.tar.gz` & `tmp/atmoswing-toolbox-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atmoswing-toolbox-1.3.4.tar", last modified: Fri May 12 09:05:46 2023, max compression
+gzip compressed data, was "atmoswing-toolbox-1.3.5.tar", last modified: Fri May 12 09:30:54 2023, max compression
```

## Comparing `atmoswing-toolbox-1.3.4.tar` & `atmoswing-toolbox-1.3.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:05:46.403482 atmoswing-toolbox-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-12 09:05:35.000000 atmoswing-toolbox-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-12 09:05:35.000000 atmoswing-toolbox-1.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-12 09:05:46.403482 atmoswing-toolbox-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-12 09:05:35.000000 atmoswing-toolbox-1.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:05:46.399482 atmoswing-toolbox-1.3.4/atmoswing_toolbox/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:05:46.403482 atmoswing-toolbox-1.3.4/atmoswing_toolbox/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-12 09:05:35.000000 atmoswing-toolbox-1.3.4/atmoswing_toolbox/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-12 09:05:35.000000 atmoswing-toolbox-1.3.4/atmoswing_toolbox/datasets/generic_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-05-12 09:05:35.000000 atmoswing-toolbox-1.3.4/atmoswing_toolbox/datasets/grib_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-12 09:05:35.000000 atmoswing-toolbox-1.3.4/atmoswing_toolbox/datasets/netcdf_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-12 09:05:35.000000 atmoswing-toolbox-1.3.4/atmoswing_toolbox/datasets/predictor_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:05:46.403482 atmoswing-toolbox-1.3.4/atmoswing_toolbox/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-12 09:05:35.000000 atmoswing-toolbox-1.3.4/atmoswing_toolbox/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-05-12 09:05:35.000000 atmoswing-toolbox-1.3.4/atmoswing_toolbox/parsers/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)    12088 2023-05-12 09:05:35.000000 atmoswing-toolbox-1.3.4/atmoswing_toolbox/parsers/optimized_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:05:46.403482 atmoswing-toolbox-1.3.4/atmoswing_toolbox/plots/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-12 09:05:35.000000 atmoswing-toolbox-1.3.4/atmoswing_toolbox/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-05-12 09:05:35.000000 atmoswing-toolbox-1.3.4/atmoswing_toolbox/plots/forecast_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    24128 2023-05-12 09:05:35.000000 atmoswing-toolbox-1.3.4/atmoswing_toolbox/plots/gas_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-05-12 09:05:35.000000 atmoswing-toolbox-1.3.4/atmoswing_toolbox/plots/montecarlo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:05:46.403482 atmoswing-toolbox-1.3.4/atmoswing_toolbox/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-12 09:05:35.000000 atmoswing-toolbox-1.3.4/atmoswing_toolbox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-12 09:05:35.000000 atmoswing-toolbox-1.3.4/atmoswing_toolbox/utils/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-12 09:05:35.000000 atmoswing-toolbox-1.3.4/atmoswing_toolbox/utils/compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-12 09:05:35.000000 atmoswing-toolbox-1.3.4/atmoswing_toolbox/utils/mjd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:05:46.403482 atmoswing-toolbox-1.3.4/atmoswing_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-12 09:05:46.000000 atmoswing-toolbox-1.3.4/atmoswing_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-12 09:05:46.000000 atmoswing-toolbox-1.3.4/atmoswing_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 09:05:46.000000 atmoswing-toolbox-1.3.4/atmoswing_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 09:05:46.000000 atmoswing-toolbox-1.3.4/atmoswing_toolbox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-12 09:05:46.000000 atmoswing-toolbox-1.3.4/atmoswing_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-12 09:05:46.000000 atmoswing-toolbox-1.3.4/atmoswing_toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-12 09:05:35.000000 atmoswing-toolbox-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 09:05:46.403482 atmoswing-toolbox-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-12 09:05:35.000000 atmoswing-toolbox-1.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:05:46.403482 atmoswing-toolbox-1.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-12 09:05:35.000000 atmoswing-toolbox-1.3.4/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:30:54.252681 atmoswing-toolbox-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-12 09:30:41.000000 atmoswing-toolbox-1.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-12 09:30:41.000000 atmoswing-toolbox-1.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-12 09:30:54.252681 atmoswing-toolbox-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-12 09:30:41.000000 atmoswing-toolbox-1.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:30:54.248681 atmoswing-toolbox-1.3.5/atmoswing_toolbox/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:30:54.248681 atmoswing-toolbox-1.3.5/atmoswing_toolbox/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-12 09:30:41.000000 atmoswing-toolbox-1.3.5/atmoswing_toolbox/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-12 09:30:41.000000 atmoswing-toolbox-1.3.5/atmoswing_toolbox/datasets/generic_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-05-12 09:30:41.000000 atmoswing-toolbox-1.3.5/atmoswing_toolbox/datasets/grib_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-12 09:30:41.000000 atmoswing-toolbox-1.3.5/atmoswing_toolbox/datasets/netcdf_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-12 09:30:41.000000 atmoswing-toolbox-1.3.5/atmoswing_toolbox/datasets/predictor_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:30:54.252681 atmoswing-toolbox-1.3.5/atmoswing_toolbox/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-12 09:30:41.000000 atmoswing-toolbox-1.3.5/atmoswing_toolbox/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-05-12 09:30:41.000000 atmoswing-toolbox-1.3.5/atmoswing_toolbox/parsers/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12088 2023-05-12 09:30:41.000000 atmoswing-toolbox-1.3.5/atmoswing_toolbox/parsers/optimized_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:30:54.252681 atmoswing-toolbox-1.3.5/atmoswing_toolbox/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-12 09:30:41.000000 atmoswing-toolbox-1.3.5/atmoswing_toolbox/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-05-12 09:30:41.000000 atmoswing-toolbox-1.3.5/atmoswing_toolbox/plots/forecast_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24128 2023-05-12 09:30:41.000000 atmoswing-toolbox-1.3.5/atmoswing_toolbox/plots/gas_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-05-12 09:30:41.000000 atmoswing-toolbox-1.3.5/atmoswing_toolbox/plots/montecarlo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:30:54.252681 atmoswing-toolbox-1.3.5/atmoswing_toolbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-12 09:30:41.000000 atmoswing-toolbox-1.3.5/atmoswing_toolbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-12 09:30:41.000000 atmoswing-toolbox-1.3.5/atmoswing_toolbox/utils/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-12 09:30:41.000000 atmoswing-toolbox-1.3.5/atmoswing_toolbox/utils/compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-12 09:30:41.000000 atmoswing-toolbox-1.3.5/atmoswing_toolbox/utils/mjd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:30:54.248681 atmoswing-toolbox-1.3.5/atmoswing_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-12 09:30:54.000000 atmoswing-toolbox-1.3.5/atmoswing_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-12 09:30:54.000000 atmoswing-toolbox-1.3.5/atmoswing_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 09:30:54.000000 atmoswing-toolbox-1.3.5/atmoswing_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 09:30:54.000000 atmoswing-toolbox-1.3.5/atmoswing_toolbox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-12 09:30:54.000000 atmoswing-toolbox-1.3.5/atmoswing_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-12 09:30:54.000000 atmoswing-toolbox-1.3.5/atmoswing_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-12 09:30:41.000000 atmoswing-toolbox-1.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 09:30:54.252681 atmoswing-toolbox-1.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-12 09:30:41.000000 atmoswing-toolbox-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:30:54.252681 atmoswing-toolbox-1.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-12 09:30:41.000000 atmoswing-toolbox-1.3.5/tests/test_init.py
```

### Comparing `atmoswing-toolbox-1.3.4/LICENSE` & `atmoswing-toolbox-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `atmoswing-toolbox-1.3.4/PKG-INFO` & `atmoswing-toolbox-1.3.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atmoswing-toolbox
-Version: 1.3.4
+Version: 1.3.5
 Summary: Python tools for AtmoSwing
 Author: Pascal Horton
 Author-email: pascal.horton@giub.unibe
 License: MIT
 Project-URL: Source Code, https://github.com/atmoswing/atmoswing-python-toolbox
 Project-URL: Bug Tracker, https://github.com/atmoswing/atmoswing-python-toolbox/issues
 Classifier: Programming Language :: Python
```

### Comparing `atmoswing-toolbox-1.3.4/atmoswing_toolbox/datasets/generic_dataset.py` & `atmoswing-toolbox-1.3.5/atmoswing_toolbox/datasets/generic_dataset.py`

 * *Files identical despite different names*

### Comparing `atmoswing-toolbox-1.3.4/atmoswing_toolbox/datasets/grib_dataset.py` & `atmoswing-toolbox-1.3.5/atmoswing_toolbox/datasets/grib_dataset.py`

 * *Files identical despite different names*

### Comparing `atmoswing-toolbox-1.3.4/atmoswing_toolbox/datasets/netcdf_dataset.py` & `atmoswing-toolbox-1.3.5/atmoswing_toolbox/datasets/netcdf_dataset.py`

 * *Files identical despite different names*

### Comparing `atmoswing-toolbox-1.3.4/atmoswing_toolbox/datasets/predictor_dataset.py` & `atmoswing-toolbox-1.3.5/atmoswing_toolbox/datasets/predictor_dataset.py`

 * *Files identical despite different names*

### Comparing `atmoswing-toolbox-1.3.4/atmoswing_toolbox/parsers/forecast.py` & `atmoswing-toolbox-1.3.5/atmoswing_toolbox/parsers/forecast.py`

 * *Files identical despite different names*

### Comparing `atmoswing-toolbox-1.3.4/atmoswing_toolbox/parsers/optimized_parameters.py` & `atmoswing-toolbox-1.3.5/atmoswing_toolbox/parsers/optimized_parameters.py`

 * *Files identical despite different names*

### Comparing `atmoswing-toolbox-1.3.4/atmoswing_toolbox/plots/forecast_timeseries.py` & `atmoswing-toolbox-1.3.5/atmoswing_toolbox/plots/forecast_timeseries.py`

 * *Files identical despite different names*

### Comparing `atmoswing-toolbox-1.3.4/atmoswing_toolbox/plots/gas_variables.py` & `atmoswing-toolbox-1.3.5/atmoswing_toolbox/plots/gas_variables.py`

 * *Files identical despite different names*

### Comparing `atmoswing-toolbox-1.3.4/atmoswing_toolbox/plots/montecarlo.py` & `atmoswing-toolbox-1.3.5/atmoswing_toolbox/plots/montecarlo.py`

 * *Files identical despite different names*

### Comparing `atmoswing-toolbox-1.3.4/atmoswing_toolbox/utils/cleanup.py` & `atmoswing-toolbox-1.3.5/atmoswing_toolbox/utils/cleanup.py`

 * *Files identical despite different names*

### Comparing `atmoswing-toolbox-1.3.4/atmoswing_toolbox/utils/compress.py` & `atmoswing-toolbox-1.3.5/atmoswing_toolbox/utils/compress.py`

 * *Files identical despite different names*

### Comparing `atmoswing-toolbox-1.3.4/atmoswing_toolbox/utils/mjd.py` & `atmoswing-toolbox-1.3.5/atmoswing_toolbox/utils/mjd.py`

 * *Files identical despite different names*

### Comparing `atmoswing-toolbox-1.3.4/atmoswing_toolbox.egg-info/PKG-INFO` & `atmoswing-toolbox-1.3.5/atmoswing_toolbox.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atmoswing-toolbox
-Version: 1.3.4
+Version: 1.3.5
 Summary: Python tools for AtmoSwing
 Author: Pascal Horton
 Author-email: pascal.horton@giub.unibe
 License: MIT
 Project-URL: Source Code, https://github.com/atmoswing/atmoswing-python-toolbox
 Project-URL: Bug Tracker, https://github.com/atmoswing/atmoswing-python-toolbox/issues
 Classifier: Programming Language :: Python
```

### Comparing `atmoswing-toolbox-1.3.4/atmoswing_toolbox.egg-info/SOURCES.txt` & `atmoswing-toolbox-1.3.5/atmoswing_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atmoswing-toolbox-1.3.4/setup.py` & `atmoswing-toolbox-1.3.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name="atmoswing-toolbox",
-    version="1.3.4",
+    version="1.3.5",
     author="Pascal Horton",
     author_email="pascal.horton@giub.unibe",
     description="Python tools for AtmoSwing",
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=['atmoswing_toolbox', 'atmoswing_toolbox.datasets',
               'atmoswing_toolbox.parsers', 'atmoswing_toolbox.plots',
```


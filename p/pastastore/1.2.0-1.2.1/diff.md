# Comparing `tmp/pastastore-1.2.0.tar.gz` & `tmp/pastastore-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pastastore-1.2.0.tar", last modified: Fri May  5 14:06:23 2023, max compression
+gzip compressed data, was "pastastore-1.2.1.tar", last modified: Fri May 12 13:03:39 2023, max compression
```

## Comparing `pastastore-1.2.0.tar` & `pastastore-1.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:06:23.297315 pastastore-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-05 14:06:07.000000 pastastore-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-05 14:06:23.293315 pastastore-1.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:06:23.293315 pastastore-1.2.0/pastastore/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-05 14:06:07.000000 pastastore-1.2.0/pastastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62394 2023-05-05 14:06:07.000000 pastastore-1.2.0/pastastore/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    28727 2023-05-05 14:06:07.000000 pastastore-1.2.0/pastastore/connectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-05-05 14:06:07.000000 pastastore-1.2.0/pastastore/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    41622 2023-05-05 14:06:07.000000 pastastore-1.2.0/pastastore/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    34111 2023-05-05 14:06:07.000000 pastastore-1.2.0/pastastore/store.py
--rw-r--r--   0 runner    (1001) docker     (123)    31168 2023-05-05 14:06:07.000000 pastastore-1.2.0/pastastore/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-05 14:06:07.000000 pastastore-1.2.0/pastastore/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    29490 2023-05-05 14:06:07.000000 pastastore-1.2.0/pastastore/yaml_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:06:23.293315 pastastore-1.2.0/pastastore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-05 14:06:23.000000 pastastore-1.2.0/pastastore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-05 14:06:23.000000 pastastore-1.2.0/pastastore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:06:23.000000 pastastore-1.2.0/pastastore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-05 14:06:23.000000 pastastore-1.2.0/pastastore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 14:06:23.000000 pastastore-1.2.0/pastastore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-05 14:06:07.000000 pastastore-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-05 14:06:07.000000 pastastore-1.2.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 14:06:23.297315 pastastore-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:06:23.293315 pastastore-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-05 14:06:07.000000 pastastore-1.2.0/tests/test_001_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-05-05 14:06:07.000000 pastastore-1.2.0/tests/test_002_connectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-05-05 14:06:07.000000 pastastore-1.2.0/tests/test_003_pastastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-05 14:06:07.000000 pastastore-1.2.0/tests/test_004_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-05 14:06:07.000000 pastastore-1.2.0/tests/test_005_maps_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-05-05 14:06:07.000000 pastastore-1.2.0/tests/test_006_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:03:39.086528 pastastore-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-12 13:03:20.000000 pastastore-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-05-12 13:03:39.086528 pastastore-1.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:03:39.086528 pastastore-1.2.1/pastastore/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-12 13:03:20.000000 pastastore-1.2.1/pastastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62290 2023-05-12 13:03:20.000000 pastastore-1.2.1/pastastore/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28727 2023-05-12 13:03:20.000000 pastastore-1.2.1/pastastore/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-05-12 13:03:20.000000 pastastore-1.2.1/pastastore/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41622 2023-05-12 13:03:20.000000 pastastore-1.2.1/pastastore/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34126 2023-05-12 13:03:20.000000 pastastore-1.2.1/pastastore/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31203 2023-05-12 13:03:20.000000 pastastore-1.2.1/pastastore/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-12 13:03:20.000000 pastastore-1.2.1/pastastore/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29490 2023-05-12 13:03:20.000000 pastastore-1.2.1/pastastore/yaml_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:03:39.086528 pastastore-1.2.1/pastastore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-05-12 13:03:39.000000 pastastore-1.2.1/pastastore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-12 13:03:39.000000 pastastore-1.2.1/pastastore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 13:03:39.000000 pastastore-1.2.1/pastastore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-12 13:03:39.000000 pastastore-1.2.1/pastastore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-12 13:03:39.000000 pastastore-1.2.1/pastastore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-12 13:03:20.000000 pastastore-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-12 13:03:20.000000 pastastore-1.2.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 13:03:39.086528 pastastore-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:03:39.086528 pastastore-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-12 13:03:20.000000 pastastore-1.2.1/tests/test_001_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-05-12 13:03:20.000000 pastastore-1.2.1/tests/test_002_connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-05-12 13:03:20.000000 pastastore-1.2.1/tests/test_003_pastastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-12 13:03:20.000000 pastastore-1.2.1/tests/test_004_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-12 13:03:20.000000 pastastore-1.2.1/tests/test_005_maps_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-05-12 13:03:20.000000 pastastore-1.2.1/tests/test_006_benchmark.py
```

### Comparing `pastastore-1.2.0/LICENSE` & `pastastore-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pastastore-1.2.0/PKG-INFO` & `pastastore-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pastastore
-Version: 1.2.0
+Version: 1.2.1
 Summary: Tools for managing Pastas time series models.
 Author: D.A. Brakenhoff
 Maintainer-email: "D.A. Brakenhoff" <d.brakenhoff@artesia-water.nl>, "R. Calje" <r.calje@artesia-water.nl>, "M.A. Vonk" <m.vonk@artesia-water.nl>
 License: The MIT License (MIT)
         
         Copyright (c) 2020 D.A. Brakenhoff
         
@@ -40,14 +40,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: lint
 Provides-Extra: optional
 Provides-Extra: test
```

### Comparing `pastastore-1.2.0/pastastore/base.py` & `pastastore-1.2.1/pastastore/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,14 @@
             name of the library
 
         Returns
         -------
         lib : Any
             handle to the library
         """
-        pass
 
     @abstractmethod
     def _add_item(
         self,
         libname: str,
         item: Union[FrameorSeriesUnion, Dict],
         name: str,
@@ -90,15 +89,14 @@
         item : FrameorSeriesUnion or dict
             item to add
         name : str
             name of the item
         metadata : dict, optional
             dictionary containing metadata, by default None
         """
-        pass
 
     @abstractmethod
     def _get_item(self, libname: str, name: str) -> Union[FrameorSeriesUnion, Dict]:
         """Internal method to get item (series or pastas.Models).
 
         Must be overriden by subclass.
 
@@ -110,30 +108,28 @@
             name of item
 
         Returns
         -------
         item : FrameorSeriesUnion or dict
             item (time series or pastas.Model)
         """
-        pass
 
     @abstractmethod
     def _del_item(self, libname: str, name: str) -> None:
         """Internal method to delete items (series or models).
 
         Must be overriden by subclass.
 
         Parameters
         ----------
         libname : str
             name of library to delete item from
         name : str
             name of item to delete
         """
-        pass
 
     @abstractmethod
     def _get_metadata(self, libname: str, name: str) -> Dict:
         """Internal method to get metadata.
 
         Must be overriden by subclass.
 
@@ -145,39 +141,35 @@
             name of the item
 
         Returns
         -------
         metadata : dict
             dictionary containing metadata
         """
-        pass
 
     @abstractproperty
     def oseries_names(self):
         """List of oseries names.
 
         Property must be overriden by subclass.
         """
-        pass
 
     @abstractproperty
     def stresses_names(self):
         """List of stresses names.
 
         Property must be overriden by subclass.
         """
-        pass
 
     @abstractproperty
     def model_names(self):
         """List of model names.
 
         Property must be overriden by subclass.
         """
-        pass
 
     def set_check_model_series_values(self, b: bool):
         """Turn CHECK_MODEL_SERIES_VALUES option on (True) or off (False).
 
         The default option is on (it is highly recommended to keep it that
         way). When turned on, the model time series
         (ml.oseries._series_original, and stressmodel.stress._series_original)
```

### Comparing `pastastore-1.2.0/pastastore/connectors.py` & `pastastore-1.2.1/pastastore/connectors.py`

 * *Files identical despite different names*

### Comparing `pastastore-1.2.0/pastastore/datasets.py` & `pastastore-1.2.1/pastastore/datasets.py`

 * *Files identical despite different names*

### Comparing `pastastore-1.2.0/pastastore/plotting.py` & `pastastore-1.2.1/pastastore/plotting.py`

 * *Files identical despite different names*

### Comparing `pastastore-1.2.0/pastastore/store.py` & `pastastore-1.2.1/pastastore/store.py`

 * *Files 0% similar despite different names*

```diff
@@ -978,14 +978,14 @@
             for sm in iml["stressmodels"].values():
                 class_key = "stressmodel" if PASFILE_LEQ_022 else "class"
                 if sm[class_key] == "RechargeModel":
                     pnam = sm["prec"]["name"]
                     enam = sm["evap"]["name"]
                     structure.loc[mlnam, pnam] = 1
                     structure.loc[mlnam, enam] = 1
-                else:
+                elif "stress" in sm:
                     for s in sm["stress"]:
                         structure.loc[mlnam, s["name"]] = 1
         if dropna:
             return structure.dropna(how="all", axis=1)
         else:
             return structure
```

### Comparing `pastastore-1.2.0/pastastore/util.py` & `pastastore-1.2.1/pastastore/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -741,15 +741,16 @@
                             gain_std = np.nan
                             check_gain_passed = pd.NA
                         elif np.isnan(gain_std):
                             check_gain_passed = pd.NA
                         else:
                             check_gain_passed = np.abs(gain) > 2 * gain_std
                         checks.loc[
-                            f"gain > 2*std: {sm_name}-{iw:02g} ({sm.distances.index[iw]})"
+                            f"gain > 2*std: {sm_name}-{iw:02g} ({sm.distances.index[iw]})",
+                            :,
                         ] = (
                             gain,
                             2 * gain_std,
                             "(unit head)/(unit well stress)",
                             check_gain_passed,
                         )
                 else:
@@ -759,15 +760,15 @@
                         gain_std = np.nan
                         check_gain_passed = pd.NA
                     elif np.isnan(gain_std):
                         check_gain_passed = pd.NA
                     else:
                         check_gain_passed = np.abs(gain) > 2 * gain_std
                     check_gain_passed = np.abs(gain) > 2 * gain_std
-                    checks.loc[f"gain > 2*std: {sm_name}"] = (
+                    checks.loc[f"gain > 2*std: {sm_name}", :] = (
                         gain,
                         2 * gain_std,
                         "(unit head)/(unit well stress)",
                         check_gain_passed,
                     )
 
         # Check 5 - Parameter Bounds
```

### Comparing `pastastore-1.2.0/pastastore/yaml_interface.py` & `pastastore-1.2.1/pastastore/yaml_interface.py`

 * *Files identical despite different names*

### Comparing `pastastore-1.2.0/pastastore.egg-info/PKG-INFO` & `pastastore-1.2.1/pastastore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pastastore
-Version: 1.2.0
+Version: 1.2.1
 Summary: Tools for managing Pastas time series models.
 Author: D.A. Brakenhoff
 Maintainer-email: "D.A. Brakenhoff" <d.brakenhoff@artesia-water.nl>, "R. Calje" <r.calje@artesia-water.nl>, "M.A. Vonk" <m.vonk@artesia-water.nl>
 License: The MIT License (MIT)
         
         Copyright (c) 2020 D.A. Brakenhoff
         
@@ -40,14 +40,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: lint
 Provides-Extra: optional
 Provides-Extra: test
```

### Comparing `pastastore-1.2.0/pastastore.egg-info/SOURCES.txt` & `pastastore-1.2.1/pastastore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pastastore-1.2.0/pyproject.toml` & `pastastore-1.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     "Operating System :: MacOS",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Scientific/Engineering :: Hydrology",
 ]
 
 [project.urls]
 homepage = "https://github.com/pastas/pastastore"
 repository = "https://github.com/pastas/pastastore"
@@ -57,17 +58,15 @@
     "pytest-benchmark",
     "codacy-coverage",
 ]
 pystore = ["fsspec>=0.3.3", "python-snappy", "dask[dataframe]"]
 arctic = [
     "arctic", # will not work as releases not uploaded to PyPI
 ]
-arcticdb = [
-    "arcticdb",
-]
+arcticdb = ["arcticdb"]
 docs = [
     "pastastore[optional]",
     "sphinx_rtd_theme",
     "Ipython",
     "ipykernel",
     "nbsphinx",
     "nbsphinx_link",
```

### Comparing `pastastore-1.2.0/readme.md` & `pastastore-1.2.1/readme.md`

 * *Files identical despite different names*

### Comparing `pastastore-1.2.0/tests/test_002_connectors.py` & `pastastore-1.2.1/tests/test_002_connectors.py`

 * *Files identical despite different names*

### Comparing `pastastore-1.2.0/tests/test_003_pastastore.py` & `pastastore-1.2.1/tests/test_003_pastastore.py`

 * *Files identical despite different names*

### Comparing `pastastore-1.2.0/tests/test_004_yaml.py` & `pastastore-1.2.1/tests/test_004_yaml.py`

 * *Files identical despite different names*

### Comparing `pastastore-1.2.0/tests/test_005_maps_plots.py` & `pastastore-1.2.1/tests/test_005_maps_plots.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     ax = pstore.plots.cumulative_hist()
     plt.close(ax.figure)
 
 
 # %% maps
 
 
+@pytest.mark.bgmap
 def test_map_oseries_w_bgmap(pstore):
     ax = pstore.maps.oseries()
     # only test bgmap once for pas
     if pstore.type == "pas":
         pstore.maps.add_background_map(ax)
     plt.close(ax.figure)
```

### Comparing `pastastore-1.2.0/tests/test_006_benchmark.py` & `pastastore-1.2.1/tests/test_006_benchmark.py`

 * *Files identical despite different names*


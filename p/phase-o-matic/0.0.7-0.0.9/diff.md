# Comparing `tmp/phase-o-matic-0.0.7.tar.gz` & `tmp/phase-o-matic-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phase-o-matic-0.0.7.tar", last modified: Thu May 11 20:19:49 2023, max compression
+gzip compressed data, was "phase-o-matic-0.0.9.tar", last modified: Fri May 12 19:44:01 2023, max compression
```

## Comparing `phase-o-matic-0.0.7.tar` & `phase-o-matic-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:19:49.179319 phase-o-matic-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-11 20:19:31.000000 phase-o-matic-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-11 20:19:49.179319 phase-o-matic-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-11 20:19:31.000000 phase-o-matic-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:19:49.179319 phase-o-matic-0.0.7/phase_o_matic/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 20:19:31.000000 phase-o-matic-0.0.7/phase_o_matic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-11 20:19:31.000000 phase-o-matic-0.0.7/phase_o_matic/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-05-11 20:19:31.000000 phase-o-matic-0.0.7/phase_o_matic/phase_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-05-11 20:19:31.000000 phase-o-matic-0.0.7/phase_o_matic/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-11 20:19:31.000000 phase-o-matic-0.0.7/phase_o_matic/presto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-11 20:19:31.000000 phase-o-matic-0.0.7/phase_o_matic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:19:49.179319 phase-o-matic-0.0.7/phase_o_matic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-11 20:19:49.000000 phase-o-matic-0.0.7/phase_o_matic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-11 20:19:49.000000 phase-o-matic-0.0.7/phase_o_matic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:19:49.000000 phase-o-matic-0.0.7/phase_o_matic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 20:19:49.000000 phase-o-matic-0.0.7/phase_o_matic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 20:19:49.000000 phase-o-matic-0.0.7/phase_o_matic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-11 20:19:31.000000 phase-o-matic-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 20:19:49.179319 phase-o-matic-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-11 20:19:31.000000 phase-o-matic-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:19:49.179319 phase-o-matic-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-11 20:19:31.000000 phase-o-matic-0.0.7/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-11 20:19:31.000000 phase-o-matic-0.0.7/tests/test_preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:44:01.706304 phase-o-matic-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-12 19:43:42.000000 phase-o-matic-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-05-12 19:44:01.706304 phase-o-matic-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-12 19:43:42.000000 phase-o-matic-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:44:01.706304 phase-o-matic-0.0.9/phase_o_matic/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 19:43:42.000000 phase-o-matic-0.0.9/phase_o_matic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-12 19:43:42.000000 phase-o-matic-0.0.9/phase_o_matic/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-05-12 19:43:42.000000 phase-o-matic-0.0.9/phase_o_matic/phase_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-05-12 19:43:42.000000 phase-o-matic-0.0.9/phase_o_matic/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-12 19:43:42.000000 phase-o-matic-0.0.9/phase_o_matic/presto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-12 19:43:42.000000 phase-o-matic-0.0.9/phase_o_matic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:44:01.706304 phase-o-matic-0.0.9/phase_o_matic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-05-12 19:44:01.000000 phase-o-matic-0.0.9/phase_o_matic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-12 19:44:01.000000 phase-o-matic-0.0.9/phase_o_matic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 19:44:01.000000 phase-o-matic-0.0.9/phase_o_matic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 19:44:01.000000 phase-o-matic-0.0.9/phase_o_matic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-12 19:44:01.000000 phase-o-matic-0.0.9/phase_o_matic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-12 19:43:42.000000 phase-o-matic-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 19:44:01.706304 phase-o-matic-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-12 19:43:43.000000 phase-o-matic-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:44:01.706304 phase-o-matic-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-05-12 19:43:42.000000 phase-o-matic-0.0.9/tests/test_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-12 19:43:42.000000 phase-o-matic-0.0.9/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-05-12 19:43:42.000000 phase-o-matic-0.0.9/tests/test_preprocess.py
```

### Comparing `phase-o-matic-0.0.7/LICENSE` & `phase-o-matic-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `phase-o-matic-0.0.7/PKG-INFO` & `phase-o-matic-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phase-o-matic
-Version: 0.0.7
+Version: 0.0.9
 Summary: InSAR Atmospheric Delay Corrections with ERA5.
 Home-page: https://github.com/ZachKeskinen/phase-o-matic
 Author: Zach Keskinen
 Author-email: zachkeskinen@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -14,18 +14,19 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # phase-o-matic
+[![PIP](https://img.shields.io/badge/pip-0.0.8-purple)](https://img.shields.io/badge/pip-0.0.8-purple)
+[![LICENSE](https://img.shields.io/badge/license-MIT-orange)](https://img.shields.io/badge/license-MIT-orange)
+[![DOI](https://zenodo.org/badge/636333382.svg)](https://zenodo.org/badge/latestdoi/636333382) 
 
-[![DOI](https://zenodo.org/badge/636333382.svg)](https://zenodo.org/badge/latestdoi/636333382)
-
-Python package for calculating Interferometric Synthetic Aperture Radar phase delays from ERA5 atmospheric models. Utilizes xarray to easily download, processes, and add phase delays to netcdfs of InSAR Phase. 
+Python package for calculating Interferometric Synthetic Aperture Radar phase delays from ERA5 atmospheric models. Utilizes xarray to easily download, processes, and add phase delays to netcdfs of InSAR Phase.
 
 Useful publications for this repo:
  - Doin, M.-P., Lasserre, C., Peltzer, G., Cavalié, O., and Doubre, C.: Corrections of stratified tropospheric delays in SAR interferometry: Validation with global atmospheric models, J Appl Geophys, 69, 35–50, https://doi.org/10.1016/j.jappgeo.2009.03.010, 2009.
 
  - Jolivet, R., Agram, P. S., Lin, N. Y., Simons, M., Doin, M., Peltzer, G., and Li, Z.: Improving InSAR geodesy using Global Atmospheric Models, J Geophys Res Solid Earth, 119, 2324–2341, https://doi.org/10.1002/2013jb010588, 2014.
 
  - Hu, Z. and Mallorquí, J. J.: An Accurate Method to Correct Atmospheric Phase Delay for InSAR with the ERA5 Global Atmospheric Model, Remote Sens-basel, 11, 1969, https://doi.org/10.3390/rs11171969, 2019.
@@ -34,15 +35,14 @@
 
 <img src="https://github.com/ZachKeskinen/phase-o-matic/blob/main/images/pyaps_phaseo_compare.png">
 
 ## Installation
 
 ### Pip installation
 ```bash
-# not implemented yet. Please just add the home directory of this repo to your path
 pip install phase_o_matic
 ```
 
 ### ERA5 Data Registration
 
 [ERA5](https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-single-levels) is atmospheric data distributed by the Copernicus Climate Change Service. You must register for an account and save the provided locally where you are downloading.
 
@@ -68,34 +68,31 @@
 This example usage is also available in `notebooks/usage.ipynb`
 
 ```python
 import sys
 import xarray as xr
 import matplotlib.pyplot as plt
 
-# this relative path assumes you are in the notebooks directory
-sys.path.append('..')
 from phase_o_matic import presto_phase_delay
 
 # this relative path assumes you are in the notebooks directory
-# the dem_datset is a netcdf that should have a 'dem' variable and an
-# incidence angle data variable 'inc' in radians
-dem_dataset = xr.open_dataset('../pyAPS_data/pyaps_geom.nc')
+dem = xr.open_dataset('../pyAPS_data/pyaps_geom.nc')['dem']
+inc = xr.open_dataset('../pyAPS_data/pyaps_geom.nc')['inc']
 
 work_dir = '../pyAPS_data/example'
 
-t1 = presto_phase_delay(date = '2020-01-03', geometry = dem_dataset, work_dir = work_dir, wavelength = 0.238403545)
-t2 = presto_phase_delay(date = '2020-01-10', geometry = dem_dataset, work_dir = work_dir, wavelength = 0.238403545)
+t1 = presto_phase_delay(date = '2020-01-03', dem = dem, inc = inc, work_dir = work_dir, wavelength = 0.238403545)
+t2 = presto_phase_delay(date = '2020-01-10', dem = dem, inc = inc, work_dir = work_dir, wavelength = 0.238403545)
 
 delay_change = t2.isel(time = 0)['delay'] - t1.isel(time = 0)['delay']
 
 fig, axes = plt.subplots(1, 2, figsize = (12, 9))
 delay_change.plot(ax = axes[0], vmax = 0, vmin = -4)
-dem_dataset['dem'].plot(ax = axes[1], vmin = 0, vmax = 2000)
-plt.show()
+dem.plot(ax = axes[1], vmin = 0, vmax = 2000)
+plt.savefig('../images/usage.png')
 ```
 
 ## Citations
 
 If you end up using the ERA5 data please cite this repo:
 
 Keskinen, Z. (2023) Phase-o-matic: InSAR atmospheric delay calculations, https://github.com/ZachKeskinen/phase-o-matic/. DOI: 10.5281/zenodo.7926686
```

### Comparing `phase-o-matic-0.0.7/README.md` & `phase-o-matic-0.0.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # phase-o-matic
+[![PIP](https://img.shields.io/badge/pip-0.0.8-purple)](https://img.shields.io/badge/pip-0.0.8-purple)
+[![LICENSE](https://img.shields.io/badge/license-MIT-orange)](https://img.shields.io/badge/license-MIT-orange)
+[![DOI](https://zenodo.org/badge/636333382.svg)](https://zenodo.org/badge/latestdoi/636333382) 
 
-[![DOI](https://zenodo.org/badge/636333382.svg)](https://zenodo.org/badge/latestdoi/636333382)
-
-Python package for calculating Interferometric Synthetic Aperture Radar phase delays from ERA5 atmospheric models. Utilizes xarray to easily download, processes, and add phase delays to netcdfs of InSAR Phase. 
+Python package for calculating Interferometric Synthetic Aperture Radar phase delays from ERA5 atmospheric models. Utilizes xarray to easily download, processes, and add phase delays to netcdfs of InSAR Phase.
 
 Useful publications for this repo:
  - Doin, M.-P., Lasserre, C., Peltzer, G., Cavalié, O., and Doubre, C.: Corrections of stratified tropospheric delays in SAR interferometry: Validation with global atmospheric models, J Appl Geophys, 69, 35–50, https://doi.org/10.1016/j.jappgeo.2009.03.010, 2009.
 
  - Jolivet, R., Agram, P. S., Lin, N. Y., Simons, M., Doin, M., Peltzer, G., and Li, Z.: Improving InSAR geodesy using Global Atmospheric Models, J Geophys Res Solid Earth, 119, 2324–2341, https://doi.org/10.1002/2013jb010588, 2014.
 
  - Hu, Z. and Mallorquí, J. J.: An Accurate Method to Correct Atmospheric Phase Delay for InSAR with the ERA5 Global Atmospheric Model, Remote Sens-basel, 11, 1969, https://doi.org/10.3390/rs11171969, 2019.
@@ -15,15 +16,14 @@
 
 <img src="https://github.com/ZachKeskinen/phase-o-matic/blob/main/images/pyaps_phaseo_compare.png">
 
 ## Installation
 
 ### Pip installation
 ```bash
-# not implemented yet. Please just add the home directory of this repo to your path
 pip install phase_o_matic
 ```
 
 ### ERA5 Data Registration
 
 [ERA5](https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-single-levels) is atmospheric data distributed by the Copernicus Climate Change Service. You must register for an account and save the provided locally where you are downloading.
 
@@ -49,34 +49,31 @@
 This example usage is also available in `notebooks/usage.ipynb`
 
 ```python
 import sys
 import xarray as xr
 import matplotlib.pyplot as plt
 
-# this relative path assumes you are in the notebooks directory
-sys.path.append('..')
 from phase_o_matic import presto_phase_delay
 
 # this relative path assumes you are in the notebooks directory
-# the dem_datset is a netcdf that should have a 'dem' variable and an
-# incidence angle data variable 'inc' in radians
-dem_dataset = xr.open_dataset('../pyAPS_data/pyaps_geom.nc')
+dem = xr.open_dataset('../pyAPS_data/pyaps_geom.nc')['dem']
+inc = xr.open_dataset('../pyAPS_data/pyaps_geom.nc')['inc']
 
 work_dir = '../pyAPS_data/example'
 
-t1 = presto_phase_delay(date = '2020-01-03', geometry = dem_dataset, work_dir = work_dir, wavelength = 0.238403545)
-t2 = presto_phase_delay(date = '2020-01-10', geometry = dem_dataset, work_dir = work_dir, wavelength = 0.238403545)
+t1 = presto_phase_delay(date = '2020-01-03', dem = dem, inc = inc, work_dir = work_dir, wavelength = 0.238403545)
+t2 = presto_phase_delay(date = '2020-01-10', dem = dem, inc = inc, work_dir = work_dir, wavelength = 0.238403545)
 
 delay_change = t2.isel(time = 0)['delay'] - t1.isel(time = 0)['delay']
 
 fig, axes = plt.subplots(1, 2, figsize = (12, 9))
 delay_change.plot(ax = axes[0], vmax = 0, vmin = -4)
-dem_dataset['dem'].plot(ax = axes[1], vmin = 0, vmax = 2000)
-plt.show()
+dem.plot(ax = axes[1], vmin = 0, vmax = 2000)
+plt.savefig('../images/usage.png')
 ```
 
 ## Citations
 
 If you end up using the ERA5 data please cite this repo:
 
 Keskinen, Z. (2023) Phase-o-matic: InSAR atmospheric delay calculations, https://github.com/ZachKeskinen/phase-o-matic/. DOI: 10.5281/zenodo.7926686
```

### Comparing `phase-o-matic-0.0.7/phase_o_matic/download.py` & `phase-o-matic-0.0.9/phase_o_matic/download.py`

 * *Files identical despite different names*

### Comparing `phase-o-matic-0.0.7/phase_o_matic/phase_delay.py` & `phase-o-matic-0.0.9/phase_o_matic/phase_delay.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import numpy as np
 import xarray as xr
 from scipy import integrate
 
+from typing import Union
+
 def calculate_dry_refractivity(dataset: xr.Dataset) -> xr.Dataset:
     """
     Calculate dry/hydro-static refractivity from air pressure, vapor pressure, and temperature
     Following Jolivet et al (2011, 2014).
     
     Args:
     dataset: xarray dataset with air_pressure, vapor_pressure, and temperature
 
     Returns:
     dataset: xarray dataset with dry refractivity added
     """
 
-    assert dataset['air_pressure'].attrs['units'] == 'pascals'
-    assert dataset['temperature'].attrs['units'] == 'K'
+    if 'units' in dataset['air_pressure'].attrs:
+        assert dataset['air_pressure'].attrs['units'] == 'pascals'
+    if 'units' in dataset['temperature'].attrs:
+        assert dataset['temperature'].attrs['units'] == 'K'
     
     # constant for dry refractivity
     k1 = 0.776 # K / Pa
     Rd = 287.05 # j / kg K
     g = 9.81 # m / s
 
     if np.all(np.diff(dataset.height, 1) < 0):
@@ -40,16 +44,18 @@
     Args:
     dataset: xarray dataset with air_pressure, vapor_pressure, and temperature
 
     Returns:
     dataset: xarray dataset with wet refractivity added
     """
 
-    assert dataset['vapor_pressure'].attrs['units'] == 'pascals'
-    assert dataset['temperature'].attrs['units'] == 'K'
+    if 'units' in dataset['vapor_pressure'].attrs:
+        assert dataset['vapor_pressure'].attrs['units'] == 'pascals'
+    if 'units' in dataset['temperature'].attrs:
+        assert dataset['temperature'].attrs['units'] == 'K'
 
     if not np.all(np.diff(dataset.height, 1) > 0):
         # reverse heights so we integrate from satellite to ground (high -> low)
         dataset = dataset.reindex(height=list(reversed(dataset.height)))
 
     # constants for wet refractivity
     k1 = 0.776 # K / Pa
@@ -104,42 +110,60 @@
     # calculate refractivity index from water vapor
     dataset = calculate_wet_refractivity(dataset)
     # combine wet and dry refractivity
     dataset['N'] = dataset['N_dry'] + dataset['N_wet']
 
     return dataset
 
-def get_delay(dataset: xr.Dataset, geometry: xr.Dataset, wavelength: float = 4*np.pi) -> xr.Dataset:
+def get_delay(dataset: xr.Dataset, dem: xr.DataArray, inc: Union[xr.DataArray, float], wavelength: float = 4*np.pi) -> xr.Dataset:
     """
     Get delay in m (default) or radians (if wavelength provided) for each height
     https://github.com/insarlab/PyAPS/blob/244552cdfcf4e1a55de5f1439be4f08eb45872ec/src/pyaps3/objects.py#L213
 
     Args:
     ds: xarray dataset of atmosphere with refractive indexes calculated
     geometry: xarray dataset of elevations (var_name = 'dem'), incidence angles in radians (var_name = 'inc')
         and coords for "y" and "x".
     wavelength: either default 4 * pi (returns meters of delay) or radar wavelength in meters (returns radians)
 
     Returns:
     delay: cos calculated phase delay for each weather station data point interpolated to each meter of DEM
     """
 
-    assert 'N' in dataset.data_vars
-    assert 'dem' in geometry.data_vars
-    assert 'inc' in geometry.data_vars
+    assert wavelength > 0, "Can not have negative wavelength"
+
+    assert 'N' in dataset.data_vars, "Must have refractivity index calculated to interpolate to DEM"
+
+    if isinstance(inc, xr.DataArray):
+
+        assert inc.mean() < 2*np.pi, f'Incidence mean over 2 pi. Check if you are inc in radians'
 
-    if geometry['inc'].mean() > 10: print(f'Incidence mean over 10. Check if you are inc in radians')
+        # check to see if incidence angle and DEM are aligned and align them if not
+        try:
+            xr.align(dem, inc, join='exact')
+        except ValueError:
+            inc = inc.interp_like(dem)
+
+            # check if we got rid of all the values due to no overlap
+            assert inc.isnull().sum() != dem.size, "No overlap between incidence angle and dem"
+
+    else:
+        assert inc < 2*np.pi, f'Incidence mean over 2 pi. Check if you are inc in radians'
+    
+    # check if atmospheric values cover the dem
+    assert dataset.height.min() <= dem.min()
+    assert dataset.height.max() >= dem.max()
 
     # interpolate heights to each meter from the lowest point of the dem to the highest from our current spacing
-    dataset = dataset.interp(height = np.round(np.arange(geometry['dem'].min() - 2, geometry['dem'].max() + 2)), method = 'linear')
+    dataset = dataset.interp(height = np.round(np.arange(dem.min() - 2, dem.max() + 2)), method = 'linear')
 
     # interpolate across the dem's lats, longs, and elevations to find the surface delay
-    dataset = dataset.interp(latitude = geometry.y, longitude = geometry.x, height = geometry['dem'])
+    dataset = dataset.interp(latitude = dem.latitude, longitude = dem.longitude, height = dem)
 
     # add phase delay data_variable
-    dataset['delay'] = dataset['N']*np.pi*4.0/(wavelength*geometry['inc'])
+    dataset['delay'] = dataset['N']*np.pi*4.0/(wavelength*np.cos(inc))
 
     # make sure we have coordinates in the right order for plotting
-    dataset = dataset.transpose('time','y','x')
+    dataset = dataset.transpose('time','latitude','longitude')
 
     return dataset
```

### Comparing `phase-o-matic-0.0.7/phase_o_matic/preprocess.py` & `phase-o-matic-0.0.9/phase_o_matic/preprocess.py`

 * *Files identical despite different names*

### Comparing `phase-o-matic-0.0.7/phase_o_matic.egg-info/PKG-INFO` & `phase-o-matic-0.0.9/phase_o_matic.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phase-o-matic
-Version: 0.0.7
+Version: 0.0.9
 Summary: InSAR Atmospheric Delay Corrections with ERA5.
 Home-page: https://github.com/ZachKeskinen/phase-o-matic
 Author: Zach Keskinen
 Author-email: zachkeskinen@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -14,18 +14,19 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # phase-o-matic
+[![PIP](https://img.shields.io/badge/pip-0.0.8-purple)](https://img.shields.io/badge/pip-0.0.8-purple)
+[![LICENSE](https://img.shields.io/badge/license-MIT-orange)](https://img.shields.io/badge/license-MIT-orange)
+[![DOI](https://zenodo.org/badge/636333382.svg)](https://zenodo.org/badge/latestdoi/636333382) 
 
-[![DOI](https://zenodo.org/badge/636333382.svg)](https://zenodo.org/badge/latestdoi/636333382)
-
-Python package for calculating Interferometric Synthetic Aperture Radar phase delays from ERA5 atmospheric models. Utilizes xarray to easily download, processes, and add phase delays to netcdfs of InSAR Phase. 
+Python package for calculating Interferometric Synthetic Aperture Radar phase delays from ERA5 atmospheric models. Utilizes xarray to easily download, processes, and add phase delays to netcdfs of InSAR Phase.
 
 Useful publications for this repo:
  - Doin, M.-P., Lasserre, C., Peltzer, G., Cavalié, O., and Doubre, C.: Corrections of stratified tropospheric delays in SAR interferometry: Validation with global atmospheric models, J Appl Geophys, 69, 35–50, https://doi.org/10.1016/j.jappgeo.2009.03.010, 2009.
 
  - Jolivet, R., Agram, P. S., Lin, N. Y., Simons, M., Doin, M., Peltzer, G., and Li, Z.: Improving InSAR geodesy using Global Atmospheric Models, J Geophys Res Solid Earth, 119, 2324–2341, https://doi.org/10.1002/2013jb010588, 2014.
 
  - Hu, Z. and Mallorquí, J. J.: An Accurate Method to Correct Atmospheric Phase Delay for InSAR with the ERA5 Global Atmospheric Model, Remote Sens-basel, 11, 1969, https://doi.org/10.3390/rs11171969, 2019.
@@ -34,15 +35,14 @@
 
 <img src="https://github.com/ZachKeskinen/phase-o-matic/blob/main/images/pyaps_phaseo_compare.png">
 
 ## Installation
 
 ### Pip installation
 ```bash
-# not implemented yet. Please just add the home directory of this repo to your path
 pip install phase_o_matic
 ```
 
 ### ERA5 Data Registration
 
 [ERA5](https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-single-levels) is atmospheric data distributed by the Copernicus Climate Change Service. You must register for an account and save the provided locally where you are downloading.
 
@@ -68,34 +68,31 @@
 This example usage is also available in `notebooks/usage.ipynb`
 
 ```python
 import sys
 import xarray as xr
 import matplotlib.pyplot as plt
 
-# this relative path assumes you are in the notebooks directory
-sys.path.append('..')
 from phase_o_matic import presto_phase_delay
 
 # this relative path assumes you are in the notebooks directory
-# the dem_datset is a netcdf that should have a 'dem' variable and an
-# incidence angle data variable 'inc' in radians
-dem_dataset = xr.open_dataset('../pyAPS_data/pyaps_geom.nc')
+dem = xr.open_dataset('../pyAPS_data/pyaps_geom.nc')['dem']
+inc = xr.open_dataset('../pyAPS_data/pyaps_geom.nc')['inc']
 
 work_dir = '../pyAPS_data/example'
 
-t1 = presto_phase_delay(date = '2020-01-03', geometry = dem_dataset, work_dir = work_dir, wavelength = 0.238403545)
-t2 = presto_phase_delay(date = '2020-01-10', geometry = dem_dataset, work_dir = work_dir, wavelength = 0.238403545)
+t1 = presto_phase_delay(date = '2020-01-03', dem = dem, inc = inc, work_dir = work_dir, wavelength = 0.238403545)
+t2 = presto_phase_delay(date = '2020-01-10', dem = dem, inc = inc, work_dir = work_dir, wavelength = 0.238403545)
 
 delay_change = t2.isel(time = 0)['delay'] - t1.isel(time = 0)['delay']
 
 fig, axes = plt.subplots(1, 2, figsize = (12, 9))
 delay_change.plot(ax = axes[0], vmax = 0, vmin = -4)
-dem_dataset['dem'].plot(ax = axes[1], vmin = 0, vmax = 2000)
-plt.show()
+dem.plot(ax = axes[1], vmin = 0, vmax = 2000)
+plt.savefig('../images/usage.png')
 ```
 
 ## Citations
 
 If you end up using the ERA5 data please cite this repo:
 
 Keskinen, Z. (2023) Phase-o-matic: InSAR atmospheric delay calculations, https://github.com/ZachKeskinen/phase-o-matic/. DOI: 10.5281/zenodo.7926686
```

### Comparing `phase-o-matic-0.0.7/setup.py` & `phase-o-matic-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
         sys.exit()
 
 
 # Where the magic happens:
 setup(
     name=NAME,
-    version='0.0.7',
+    version='0.0.9',
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
```

### Comparing `phase-o-matic-0.0.7/tests/test_download.py` & `phase-o-matic-0.0.9/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `phase-o-matic-0.0.7/tests/test_preprocess.py` & `phase-o-matic-0.0.9/tests/test_preprocess.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 sys.path.append('./')
 sys.path.append('../')
 from phase_o_matic.preprocess import convert_pressure_to_pascals, get_vapor_partial_pressure,\
     interpolate_to_heights, geopotential_to_geopotential_heights, check_start_end
 
 class TestPreprocess(unittest.TestCase):
     """
-    Test functionality of downloading ERA5 model data
+    Test functionality of preprocessing datasets
     """
 
     levels = ['1','2','3','5','7','10','20','30','50', '70','100','125',\
         '150','175','200','225', '250','300','350','400','450','500','550','600','650',\
         '700','750','775','800','825', '850','875','900','925','950','975','1000']
     levels = np.array(levels).astype('int32')
     lats = np.linspace(43, 45, 10).astype('float32')
@@ -37,15 +37,15 @@
             "time" : (["time"], [pd.to_datetime('2020-01-04T09:00')], {'long_name' :'time'}),
         },
         attrs={'Conventions' :'CF-1.6', 'history' :'2023-05-04 17:03:14 GMT by grib_'}
     )
 
     def test_pascal_convert(self, test_ds = test_ds):
         """
-        Test downloading era5 data
+        Test converting to pascals from bars
         """
         original = test_ds.copy(deep = True)
         ds = convert_pressure_to_pascals(test_ds)
 
         self.assertEqual(ds['level'].units, 'pascals')
 
         assert_allclose(ds['level'], original['level']*100)
@@ -54,29 +54,45 @@
         ds = convert_pressure_to_pascals(ds)
 
         assert_allclose(ds['level'], original['level']*100)
         self.assertEqual(ds['level'].units, 'pascals')
     
     def test_vapor_pressure_calc(self, test_ds = test_ds):
         """
-        Tests for succesful calculation of vapour partial pressure
+        Test for succesful calculation of vapour partial pressure
         from specific humidity
         """
         original = test_ds.copy(deep = True)
         ds = get_vapor_partial_pressure(test_ds)
 
         self.assertTrue('vpr' in ds.data_vars)
 
         alpha = 461.495/287.05
         correct_vpr = original['q'] * original['level'] * alpha / (1 + (alpha - 1) * original['q'])
         assert_allclose(ds['vpr'], correct_vpr)
 
         ds['q'] = ds['q'].assign_attrs(standard_name = 'relative_humidity')
     
+    def test_geopotential_to_geopotential_heights(self, test_ds = test_ds):
+        """
+        Test for conversions between geopotential to geopotential heights
+        """
+        test_ds = convert_pressure_to_pascals(test_ds)
+        original = test_ds['z'].copy()
+        test_ds = geopotential_to_geopotential_heights(test_ds)
+
+        self.assertTrue('gph' in test_ds.data_vars)
+
+        assert_allclose(original/9.81, test_ds['gph'])
+
     def test_interpolate_to_heights(self, test_ds = test_ds):
+        """
+        Test for interpolating from pressure levels as coordinate and geopotential 
+        height as data variable to geopotential heights as indexing coordinate.
+        """
         test_ds = convert_pressure_to_pascals(test_ds)
         test_ds = geopotential_to_geopotential_heights(test_ds)
         test_ds['vpr'] = xr.DataArray(np.random.random((10, 10, 37, 1)),\
                                     coords = [test_ds.longitude, test_ds.latitude, test_ds.level, test_ds.time],\
                                     dims = ['longitude', 'latitude', 'level', 'time'])
 
         original = test_ds.copy()
```


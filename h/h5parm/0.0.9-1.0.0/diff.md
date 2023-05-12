# Comparing `tmp/h5parm-0.0.9.tar.gz` & `tmp/h5parm-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/h5parm-0.0.9.tar", last modified: Mon May 30 22:59:32 2022, max compression
+gzip compressed data, was "h5parm-1.0.0.tar", last modified: Fri May 12 09:49:08 2023, max compression
```

## Comparing `h5parm-0.0.9.tar` & `h5parm-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2022-05-30 22:59:32.620300 h5parm-0.0.9/
--rw-rw-r--   0 albert    (1000) albert    (1000)    11357 2021-06-02 01:08:45.000000 h5parm-0.0.9/LICENSE
--rw-rw-r--   0 albert    (1000) albert    (1000)     1385 2022-05-30 22:59:32.620300 h5parm-0.0.9/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)      903 2022-05-21 17:50:27.000000 h5parm-0.0.9/README.md
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2022-05-30 22:59:32.616300 h5parm-0.0.9/h5parm/
--rw-rw-r--   0 albert    (1000) albert    (1000)      141 2021-06-02 01:08:45.000000 h5parm-0.0.9/h5parm/__init__.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2022-05-30 22:59:32.620300 h5parm-0.0.9/h5parm/arrays/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2021-06-02 01:08:45.000000 h5parm-0.0.9/h5parm/arrays/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)   134014 2022-05-21 17:50:27.000000 h5parm-0.0.9/h5parm/arrays/dsa2000.W.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)     2455 2021-06-02 01:08:45.000000 h5parm-0.0.9/h5parm/arrays/gmrtPos.cfg
--rw-rw-r--   0 albert    (1000) albert    (1000)     6649 2021-06-02 01:08:45.000000 h5parm-0.0.9/h5parm/arrays/lofar.antenna.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)     2844 2021-06-02 01:08:45.000000 h5parm-0.0.9/h5parm/arrays/lofar.hba.antenna.cfg
--rw-rw-r--   0 albert    (1000) albert    (1000)    33202 2021-06-02 01:08:45.000000 h5parm-0.0.9/h5parm/datapack.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2271 2021-06-02 01:08:45.000000 h5parm-0.0.9/h5parm/maintenance.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    12882 2022-05-30 22:59:05.000000 h5parm-0.0.9/h5parm/utils.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2022-05-30 22:59:32.616300 h5parm-0.0.9/h5parm.egg-info/
--rw-rw-r--   0 albert    (1000) albert    (1000)     1385 2022-05-30 22:59:32.000000 h5parm-0.0.9/h5parm.egg-info/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)      396 2022-05-30 22:59:32.000000 h5parm-0.0.9/h5parm.egg-info/SOURCES.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2022-05-30 22:59:32.000000 h5parm-0.0.9/h5parm.egg-info/dependency_links.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        7 2022-05-30 22:59:32.000000 h5parm-0.0.9/h5parm.egg-info/top_level.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)       38 2022-05-30 22:59:32.620300 h5parm-0.0.9/setup.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)     1201 2022-05-30 22:59:15.000000 h5parm-0.0.9/setup.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-12 09:49:08.020055 h5parm-1.0.0/
+-rw-rw-r--   0 albert    (1000) albert    (1000)    11357 2021-06-02 01:08:45.000000 h5parm-1.0.0/LICENSE
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1348 2023-05-12 09:49:08.020055 h5parm-1.0.0/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)      903 2022-05-21 17:50:27.000000 h5parm-1.0.0/README.md
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-12 09:49:08.020055 h5parm-1.0.0/h5parm/
+-rw-rw-r--   0 albert    (1000) albert    (1000)      141 2021-06-02 01:08:45.000000 h5parm-1.0.0/h5parm/__init__.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-12 09:49:08.020055 h5parm-1.0.0/h5parm/arrays/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2021-06-02 01:08:45.000000 h5parm-1.0.0/h5parm/arrays/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)   134014 2022-05-21 17:50:27.000000 h5parm-1.0.0/h5parm/arrays/dsa2000.W.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)     2455 2021-06-02 01:08:45.000000 h5parm-1.0.0/h5parm/arrays/gmrtPos.cfg
+-rw-rw-r--   0 albert    (1000) albert    (1000)     6649 2021-06-02 01:08:45.000000 h5parm-1.0.0/h5parm/arrays/lofar.antenna.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)     2844 2021-06-02 01:08:45.000000 h5parm-1.0.0/h5parm/arrays/lofar.hba.antenna.cfg
+-rw-rw-r--   0 albert    (1000) albert    (1000)    33202 2021-06-02 01:08:45.000000 h5parm-1.0.0/h5parm/datapack.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2271 2021-06-02 01:08:45.000000 h5parm-1.0.0/h5parm/maintenance.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    13380 2023-05-12 09:46:44.000000 h5parm-1.0.0/h5parm/utils.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-05-12 09:49:08.020055 h5parm-1.0.0/h5parm.egg-info/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1348 2023-05-12 09:49:07.000000 h5parm-1.0.0/h5parm.egg-info/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)      396 2023-05-12 09:49:07.000000 h5parm-1.0.0/h5parm.egg-info/SOURCES.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-05-12 09:49:07.000000 h5parm-1.0.0/h5parm.egg-info/dependency_links.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        7 2023-05-12 09:49:07.000000 h5parm-1.0.0/h5parm.egg-info/top_level.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-05-12 09:49:08.020055 h5parm-1.0.0/setup.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)     1135 2023-05-12 09:46:44.000000 h5parm-1.0.0/setup.py
```

### Comparing `h5parm-0.0.9/LICENSE` & `h5parm-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `h5parm-0.0.9/PKG-INFO` & `h5parm-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: h5parm
-Version: 0.0.9
+Version: 1.0.0
 Summary: H5Parm data pack interface
 Home-page: https://github.com/joshuaalbert/h5parm
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -34,9 +32,7 @@
 patch_names, directions = datapack.get_directions(axes['dir'])
 antenna_labels, antennas = datapack.get_antennas(axes['ant'])
 timestamp, times = datapack.get_antennas(axes['time'])
 freq_labels, freqs = datapack.get_freqs(axes['freq'])
 pol_labels, pols = datapack.get_pols(axes['pol'])
 ```
 In general the first element returned by all `get_*` methods are string labels, and the second is a dimensionful `astropy` object, e.g. `ICRS` object, `Time` object etc.
-
-
```

### Comparing `h5parm-0.0.9/README.md` & `h5parm-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `h5parm-0.0.9/h5parm/arrays/dsa2000.W.cfg` & `h5parm-1.0.0/h5parm/arrays/dsa2000.W.cfg`

 * *Files identical despite different names*

### Comparing `h5parm-0.0.9/h5parm/arrays/gmrtPos.cfg` & `h5parm-1.0.0/h5parm/arrays/gmrtPos.cfg`

 * *Files identical despite different names*

### Comparing `h5parm-0.0.9/h5parm/arrays/lofar.antenna.cfg` & `h5parm-1.0.0/h5parm/arrays/lofar.antenna.cfg`

 * *Files identical despite different names*

### Comparing `h5parm-0.0.9/h5parm/arrays/lofar.hba.antenna.cfg` & `h5parm-1.0.0/h5parm/arrays/lofar.hba.antenna.cfg`

 * *Files identical despite different names*

### Comparing `h5parm-0.0.9/h5parm/datapack.py` & `h5parm-1.0.0/h5parm/datapack.py`

 * *Files identical despite different names*

### Comparing `h5parm-0.0.9/h5parm/maintenance.py` & `h5parm-1.0.0/h5parm/maintenance.py`

 * *Files identical despite different names*

### Comparing `h5parm-0.0.9/h5parm/utils.py` & `h5parm-1.0.0/h5parm/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import numpy as np
 import logging
 
+import numpy as np
+
 logger = logging.getLogger(__name__)
 import os
 from h5parm.datapack import DataPack
 import astropy.time as at
 import astropy.coordinates as ac
 import astropy.units as au
 
@@ -16,48 +17,53 @@
         phi:
 
     Returns: wrapped phi
     """
     return (phi + np.pi) % (2 * np.pi) - np.pi
 
 
-def create_empty_datapack(Nd, Nf, Nt, pols=None,
+def create_empty_datapack(Nd: int | None, Nf, Nt, pols=None,
                           field_of_view_diameter=4.,
                           start_time=None,
                           time_resolution=30.,
                           min_freq=122.,
                           max_freq=166.,
                           array_file=None,
                           phase_tracking=None,
+                          directions: ac.ICRS | None = None,
                           save_name='test_datapack.h5',
                           clobber=False,
                           seed=None) -> DataPack:
     """
     Creates an empty datapack with phase, amplitude and DTEC.
 
     Args:
-        Nd: number of directions
+        Nd: number of directions or None (needs directions given)
         Nf: number of frequencies
         Nt: number of times
         pols: polarisations, ['XX', ...]
         array_file: array file else Lofar HBA is used
         phase_tracking: tuple (RA, DEC) in degrees in ICRS frame
         field_of_view_diameter: FoV diameter in degrees
         start_time: start time in modified Julian days (mjs/86400)
         time_resolution: time step in seconds.
         min_freq: minimum frequency in MHz
         max_freq: maximum frequency in MHz
+        sky_model_bbs: optional sky model to use,
         save_name: where to save the H5parm.
         clobber: Whether to overwrite.
         seed: Numpy seed int
 
     Returns:
         DataPack
     """
-
+    if Nd is None:
+        if directions is None:
+            raise ValueError("Need Nd or directions given.")
+        Nd = len(directions)
     logger.info("=== Creating empty datapack ===")
     if seed is not None:
         np.random.seed(seed)
     save_name = os.path.abspath(save_name)
     if os.path.isfile(save_name) and clobber:
         os.unlink(save_name)
 
@@ -85,15 +91,18 @@
         up = phase_tracking.transform_to(altaz)
         if up.alt.deg < 0.:
             logger.warning("Phase tracking center below horizon at start of observation.")
         else:
             logger.info(f"Phase tracking altitude: {up.alt.deg} degrees")
         logger.info(f"Phase tracking RA: {phase_tracking.ra.deg} deg, DEC {phase_tracking.dec.deg} deg")
         phase_tracking = (phase_tracking.ra.rad, phase_tracking.dec.rad)
-        directions = get_uniform_directions_on_S2(Nd, phase_tracking, field_of_view_diameter)
+        if directions is None:
+            directions = get_uniform_directions_on_S2(Nd, phase_tracking, field_of_view_diameter)
+        if isinstance(directions, ac.ICRS):
+            directions = np.stack([directions.ra.rad, directions.dec.rad], axis=1)  # Nd, 2
         datapack.set_directions(None, directions)
         patch_names, _ = datapack.directions
         antenna_labels, _ = datapack.antennas
         _, antennas = datapack.get_antennas(antenna_labels)
         antennas = antennas.cartesian.xyz.to(au.km).value.T
         Na = antennas.shape[0]
 
@@ -109,28 +118,28 @@
                             pol=pols)
         datapack.add_soltab('amplitude000', values=amp, ant=antenna_labels, dir=patch_names, time=times, freq=freqs,
                             pol=pols)
         datapack.add_soltab('tec000', values=dtecs, ant=antenna_labels, dir=patch_names, time=times, pol=pols)
         return datapack
 
 
-def get_uniform_directions_on_S2(Nd, phase_tracking, field_of_view_diameter, source_in_centre:bool=True):
+def get_uniform_directions_on_S2(Nd, phase_tracking, field_of_view_diameter, source_in_centre: bool = True):
     """
     Get uniform directions on the sphere constrained to a given angular separation.
 
     Args:
         Nd:
         phase_tracking: tuple RA,DEC in radians
         field_of_view_diameter: field of view in degrees
 
     Returns:
         [Nd, 2] array of ra,dec in radians
     """
-    ra = phase_tracking[0]# * np.pi / 180.
-    dec = phase_tracking[1]# * np.pi / 180.
+    ra = phase_tracking[0]  # * np.pi / 180.
+    dec = phase_tracking[1]  # * np.pi / 180.
 
     def dec_to_phi(dec):
         return 0.5 * np.pi - dec
 
     phi = dec_to_phi(dec)
     unit_phase_tracking = np.asarray([np.cos(ra) * np.sin(phi), np.sin(ra) * np.sin(phi), np.cos(phi)])
     if source_in_centre:
@@ -281,16 +290,16 @@
         if to_solset not in datapack.solsets:
             datapack.add_solset(to_solset,
                                 array_file=DataPack.lofar_array_hba,
                                 directions=np.stack([directions.ra.to(au.rad).value,
                                                      directions.dec.to(au.rad).value], axis=1),
                                 patch_names=patch_names)
         for soltab in to_soltab:
-#             if not soltab.endswith("000"):
-#                 raise ValueError("By Losoto convention soltabs should end in XXX or similar. We only support XXX=000.")
+            #             if not soltab.endswith("000"):
+            #                 raise ValueError("By Losoto convention soltabs should end in XXX or similar. We only support XXX=000.")
             if 'tec' in soltab:
                 datapack.add_soltab(soltab, weightDtype='f16', time=times.mjd * 86400., pol=pol_labels,
                                     ant=antenna_labels,
                                     dir=patch_names)
             if 'clock' in soltab:
                 datapack.add_soltab(soltab, weightDtype='f16', time=times.mjd * 86400., pol=pol_labels,
                                     ant=antenna_labels, dir=patch_names)
```

### Comparing `h5parm-0.0.9/h5parm.egg-info/PKG-INFO` & `h5parm-1.0.0/h5parm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: h5parm
-Version: 0.0.9
+Version: 1.0.0
 Summary: H5Parm data pack interface
 Home-page: https://github.com/joshuaalbert/h5parm
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -34,9 +32,7 @@
 patch_names, directions = datapack.get_directions(axes['dir'])
 antenna_labels, antennas = datapack.get_antennas(axes['ant'])
 timestamp, times = datapack.get_antennas(axes['time'])
 freq_labels, freqs = datapack.get_freqs(axes['freq'])
 pol_labels, pols = datapack.get_pols(axes['pol'])
 ```
 In general the first element returned by all `get_*` methods are string labels, and the second is a dimensionful `astropy` object, e.g. `ICRS` object, `Time` object etc.
-
-
```

### Comparing `h5parm-0.0.9/setup.py` & `h5parm-1.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 from setuptools import find_packages
 
-__maximum_numpy_version__ = '1.19.0'
 __minimum_tables_version__ = '3.6.1'
 __minimum_astropy_version__ = '4.0.0'
 
-setup_requires = ['numpy<' + __maximum_numpy_version__,
+setup_requires = ['numpy',
                   'tables>=' + __minimum_tables_version__,
                   'astropy>=' + __minimum_astropy_version__]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='h5parm',
-      version='0.0.9',
+      version='1.0.0',
       description='H5Parm data pack interface',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/joshuaalbert/h5parm",
       author='Joshua G. Albert',
       author_email='albert@strw.leidenuniv.nl',
       setup_requires=setup_requires,
```


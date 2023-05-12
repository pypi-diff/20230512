# Comparing `tmp/pfsspy-1.1.2.tar.gz` & `tmp/pfsspy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfsspy-1.1.2.tar", last modified: Fri Aug 26 14:18:09 2022, max compression
+gzip compressed data, was "pfsspy-1.2.0.tar", last modified: Fri May 12 11:36:48 2023, max compression
```

## Comparing `pfsspy-1.1.2.tar` & `pfsspy-1.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 14:18:09.420414 pfsspy-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)    35288 2022-08-26 14:17:49.000000 pfsspy-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-08-26 14:17:49.000000 pfsspy-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2169 2022-08-26 14:18:09.420414 pfsspy-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-08-26 14:17:49.000000 pfsspy-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 14:18:09.420414 pfsspy-1.1.2/pfsspy/
--rw-r--r--   0 runner    (1001) docker     (121)      971 2022-08-26 14:17:49.000000 pfsspy-1.1.2/pfsspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-08-26 14:18:09.420414 pfsspy-1.1.2/pfsspy/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     4423 2022-08-26 14:17:49.000000 pfsspy-1.1.2/pfsspy/analytic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-08-26 14:17:49.000000 pfsspy-1.1.2/pfsspy/coords.py
--rw-r--r--   0 runner    (1001) docker     (121)     8115 2022-08-26 14:17:49.000000 pfsspy-1.1.2/pfsspy/fieldline.py
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-08-26 14:17:49.000000 pfsspy-1.1.2/pfsspy/grid.py
--rw-r--r--   0 runner    (1001) docker     (121)     2036 2022-08-26 14:17:49.000000 pfsspy-1.1.2/pfsspy/input.py
--rw-r--r--   0 runner    (1001) docker     (121)     5564 2022-08-26 14:17:49.000000 pfsspy-1.1.2/pfsspy/interpolator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2960 2022-08-26 14:17:49.000000 pfsspy-1.1.2/pfsspy/map.py
--rw-r--r--   0 runner    (1001) docker     (121)    18423 2022-08-26 14:17:49.000000 pfsspy-1.1.2/pfsspy/output.py
--rw-r--r--   0 runner    (1001) docker     (121)     4918 2022-08-26 14:17:49.000000 pfsspy-1.1.2/pfsspy/pfss.py
--rw-r--r--   0 runner    (1001) docker     (121)      864 2022-08-26 14:17:49.000000 pfsspy-1.1.2/pfsspy/sample_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     7460 2022-08-26 14:17:49.000000 pfsspy-1.1.2/pfsspy/tracing.py
--rw-r--r--   0 runner    (1001) docker     (121)    12816 2022-08-26 14:17:49.000000 pfsspy-1.1.2/pfsspy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 14:18:09.420414 pfsspy-1.1.2/pfsspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2169 2022-08-26 14:18:09.000000 pfsspy-1.1.2/pfsspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-08-26 14:18:09.000000 pfsspy-1.1.2/pfsspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 14:18:09.000000 pfsspy-1.1.2/pfsspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 14:18:09.000000 pfsspy-1.1.2/pfsspy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-08-26 14:18:09.000000 pfsspy-1.1.2/pfsspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-26 14:18:09.000000 pfsspy-1.1.2/pfsspy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2293 2022-08-26 14:18:09.420414 pfsspy-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-08-26 14:17:49.000000 pfsspy-1.1.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    68614 2022-08-26 14:17:49.000000 pfsspy-1.1.2/versioneer.py
+drwxr-xr-x   0 dstansby   (501) staff       (20)        0 2023-05-12 11:36:48.132924 pfsspy-1.2.0/
+-rw-r--r--   0 dstansby   (501) staff       (20)    35288 2022-02-25 17:41:32.000000 pfsspy-1.2.0/LICENSE
+-rw-r--r--   0 dstansby   (501) staff       (20)       49 2022-02-25 17:41:32.000000 pfsspy-1.2.0/MANIFEST.in
+-rw-r--r--   0 dstansby   (501) staff       (20)     2172 2023-05-12 11:36:48.132981 pfsspy-1.2.0/PKG-INFO
+-rw-r--r--   0 dstansby   (501) staff       (20)     1137 2022-02-25 17:41:32.000000 pfsspy-1.2.0/README.md
+drwxr-xr-x   0 dstansby   (501) staff       (20)        0 2023-05-12 11:36:48.133576 pfsspy-1.2.0/pfsspy/
+-rw-r--r--   0 dstansby   (501) staff       (20)      971 2023-05-12 10:44:39.000000 pfsspy-1.2.0/pfsspy/__init__.py
+-rw-r--r--   0 dstansby   (501) staff       (20)      497 2023-05-12 11:36:48.133605 pfsspy-1.2.0/pfsspy/_version.py
+-rw-r--r--   0 dstansby   (501) staff       (20)     4423 2023-05-12 10:44:39.000000 pfsspy-1.2.0/pfsspy/analytic.py
+-rw-r--r--   0 dstansby   (501) staff       (20)     1130 2022-02-25 17:41:32.000000 pfsspy-1.2.0/pfsspy/coords.py
+-rw-r--r--   0 dstansby   (501) staff       (20)     8115 2023-05-12 10:44:39.000000 pfsspy-1.2.0/pfsspy/fieldline.py
+-rw-r--r--   0 dstansby   (501) staff       (20)     2606 2023-05-12 10:44:39.000000 pfsspy-1.2.0/pfsspy/grid.py
+-rw-r--r--   0 dstansby   (501) staff       (20)     2036 2023-05-12 10:44:39.000000 pfsspy-1.2.0/pfsspy/input.py
+-rw-r--r--   0 dstansby   (501) staff       (20)     5564 2023-05-12 10:44:39.000000 pfsspy-1.2.0/pfsspy/interpolator.py
+-rw-r--r--   0 dstansby   (501) staff       (20)     2960 2023-05-12 10:44:39.000000 pfsspy-1.2.0/pfsspy/map.py
+-rw-r--r--   0 dstansby   (501) staff       (20)    18425 2023-05-12 10:44:39.000000 pfsspy-1.2.0/pfsspy/output.py
+-rw-r--r--   0 dstansby   (501) staff       (20)     4918 2023-05-12 10:44:39.000000 pfsspy-1.2.0/pfsspy/pfss.py
+-rw-r--r--   0 dstansby   (501) staff       (20)      864 2023-05-12 10:44:39.000000 pfsspy-1.2.0/pfsspy/sample_data.py
+-rw-r--r--   0 dstansby   (501) staff       (20)     7460 2023-05-12 10:44:39.000000 pfsspy-1.2.0/pfsspy/tracing.py
+-rw-r--r--   0 dstansby   (501) staff       (20)    13144 2023-05-12 10:44:39.000000 pfsspy-1.2.0/pfsspy/utils.py
+drwxr-xr-x   0 dstansby   (501) staff       (20)        0 2023-05-12 11:36:48.132814 pfsspy-1.2.0/pfsspy.egg-info/
+-rw-r--r--   0 dstansby   (501) staff       (20)     2172 2023-05-12 11:36:48.000000 pfsspy-1.2.0/pfsspy.egg-info/PKG-INFO
+-rw-r--r--   0 dstansby   (501) staff       (20)      490 2023-05-12 11:36:48.000000 pfsspy-1.2.0/pfsspy.egg-info/SOURCES.txt
+-rw-r--r--   0 dstansby   (501) staff       (20)        1 2023-05-12 11:36:48.000000 pfsspy-1.2.0/pfsspy.egg-info/dependency_links.txt
+-rw-r--r--   0 dstansby   (501) staff       (20)        1 2023-05-12 11:36:47.000000 pfsspy-1.2.0/pfsspy.egg-info/not-zip-safe
+-rw-r--r--   0 dstansby   (501) staff       (20)      325 2023-05-12 11:36:48.000000 pfsspy-1.2.0/pfsspy.egg-info/requires.txt
+-rw-r--r--   0 dstansby   (501) staff       (20)        7 2023-05-12 11:36:48.000000 pfsspy-1.2.0/pfsspy.egg-info/top_level.txt
+-rw-r--r--   0 dstansby   (501) staff       (20)     2291 2023-05-12 11:36:48.133451 pfsspy-1.2.0/setup.cfg
+-rw-r--r--   0 dstansby   (501) staff       (20)      240 2023-05-12 11:22:16.000000 pfsspy-1.2.0/setup.py
+-rw-r--r--   0 dstansby   (501) staff       (20)    68614 2023-05-12 10:44:39.000000 pfsspy-1.2.0/versioneer.py
```

### Comparing `pfsspy-1.1.2/LICENSE` & `pfsspy-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pfsspy-1.1.2/PKG-INFO` & `pfsspy-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: pfsspy
-Version: 1.1.2
+Version: 1.2.0
 Summary: "Potential field source surface modelling"
 Home-page: https://pfsspy.readthedocs.io/en/stable/
 Author: David Stansby
 Author-email: dstansby@gmail.com
 License: GPLv3
 Keywords: solar physics,solar,science,sun
 Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides: pfsspy
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: performance
 Provides-Extra: analytic
 License-File: LICENSE
```

### Comparing `pfsspy-1.1.2/README.md` & `pfsspy-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pfsspy-1.1.2/pfsspy/__init__.py` & `pfsspy-1.2.0/pfsspy/__init__.py`

 * *Files identical despite different names*

### Comparing `pfsspy-1.1.2/pfsspy/analytic.py` & `pfsspy-1.2.0/pfsspy/analytic.py`

 * *Files identical despite different names*

### Comparing `pfsspy-1.1.2/pfsspy/coords.py` & `pfsspy-1.2.0/pfsspy/coords.py`

 * *Files identical despite different names*

### Comparing `pfsspy-1.1.2/pfsspy/fieldline.py` & `pfsspy-1.2.0/pfsspy/fieldline.py`

 * *Files identical despite different names*

### Comparing `pfsspy-1.1.2/pfsspy/grid.py` & `pfsspy-1.2.0/pfsspy/grid.py`

 * *Files identical despite different names*

### Comparing `pfsspy-1.1.2/pfsspy/input.py` & `pfsspy-1.2.0/pfsspy/input.py`

 * *Files identical despite different names*

### Comparing `pfsspy-1.1.2/pfsspy/interpolator.py` & `pfsspy-1.2.0/pfsspy/interpolator.py`

 * *Files identical despite different names*

### Comparing `pfsspy-1.1.2/pfsspy/map.py` & `pfsspy-1.2.0/pfsspy/map.py`

 * *Files identical despite different names*

### Comparing `pfsspy-1.1.2/pfsspy/output.py` & `pfsspy-1.2.0/pfsspy/output.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,19 +424,19 @@
 
     def get_bvec(self, coords, out_type="spherical"):
         """
         Interpolate magnetic vectors at arbitrary coordinates.
 
         Parameters
         ----------
-        coords : `astropy.SkyCoord`
+        coords : `astropy.coordinates.SkyCoord`
             An arbitary point or set of points (length N >= 1) in the PFSS
             model domain (1Rs < r < Rss).
 
-        out_type : str, optional
+        out_type : str
             Takes values 'spherical' (default) or 'cartesian' and specifies
             whether the output vector is in spherical coordinates
             (B_r, B_theta, B_phi) or cartesian (B_x, B_y, B_z).
 
         Returns
         -------
         bvec : astropy.units.Quantity
```

### Comparing `pfsspy-1.1.2/pfsspy/pfss.py` & `pfsspy-1.2.0/pfsspy/pfss.py`

 * *Files identical despite different names*

### Comparing `pfsspy-1.1.2/pfsspy/sample_data.py` & `pfsspy-1.2.0/pfsspy/sample_data.py`

 * *Files identical despite different names*

### Comparing `pfsspy-1.1.2/pfsspy/tracing.py` & `pfsspy-1.2.0/pfsspy/tracing.py`

 * *Files identical despite different names*

### Comparing `pfsspy-1.1.2/pfsspy/utils.py` & `pfsspy-1.2.0/pfsspy/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,38 +84,43 @@
 
     data_header_pairs = [(map_slice, header)
                          for map_slice in adapt_fits[0].data]
     adaptMapSequence = sunpy.map.Map(data_header_pairs, sequence=True)
     return adaptMapSequence
 
 
-def carr_cea_wcs_header(dtime, shape):
+@u.quantity_input
+def carr_cea_wcs_header(dtime, shape, *, map_center_longitude=0*u.deg):
     """
     Create a Carrington WCS header for a Cylindrical Equal Area (CEA)
     projection. See [1]_ for information on how this is constructed.
 
     Parameters
     ----------
     dtime : datetime, None
         Datetime to associate with the map.
     shape : tuple
         Map shape. The first entry should be number of points in longitude, the
         second in latitude.
+    map_center_longitude : astropy.units.Quantity
+        Change the world coordinate longitude of the central image pixel to allow
+        for different roll angles of the Carrington map. Default to 0 deg. Must
+        be supplied with units of `astropy.units.deg`
 
     References
     ----------
     .. [1] W. T. Thompson, "Coordinate systems for solar image data",
        https://doi.org/10.1051/0004-6361:20054262
     """
     # If datetime is None, put in a dummy value here to make
     # make_fitswcs_header happy, then strip it out at the end
     obstime = dtime or astropy.time.Time('2000-1-1')
 
     frame_out = coord.SkyCoord(
-        0 * u.deg, 0 * u.deg, const.R_sun, obstime=obstime,
+        map_center_longitude, 0 * u.deg, const.R_sun, obstime=obstime,
         frame="heliographic_carrington", observer='self')
     # Construct header
     header = sunpy.map.make_fitswcs_header(
         [shape[1], shape[0]], frame_out,
         scale=[360 / shape[0],
                180 / shape[1]] * u.deg / u.pix,
         reference_pixel=[(shape[0] / 2) - 0.5,
```

### Comparing `pfsspy-1.1.2/pfsspy.egg-info/PKG-INFO` & `pfsspy-1.2.0/pfsspy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: pfsspy
-Version: 1.1.2
+Version: 1.2.0
 Summary: "Potential field source surface modelling"
 Home-page: https://pfsspy.readthedocs.io/en/stable/
 Author: David Stansby
 Author-email: dstansby@gmail.com
 License: GPLv3
 Keywords: solar physics,solar,science,sun
 Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides: pfsspy
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: performance
 Provides-Extra: analytic
 License-File: LICENSE
```

### Comparing `pfsspy-1.1.2/setup.cfg` & `pfsspy-1.2.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -3,44 +3,43 @@
 provides = pfsspy
 description = "Potential field source surface modelling"
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = David Stansby
 author_email = dstansby@gmail.com
 license = GPLv3
-license_file = LICENSE
 url = https://pfsspy.readthedocs.io/en/stable/
 edit_on_github = True
 github_project = dstansby/pfsspy
 platform = any
 keywords = solar physics, solar, science, sun
 classifiers = 
-	Development Status :: 4 - Beta
+	Development Status :: 6 - Mature
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering :: Physics
 
 [options]
 zip_safe = False
-python_requires = >=3.8
+python_requires = >=3.9
 packages = pfsspy
 include_package_data = True
 install_requires = 
 	astropy>=5.0
 	numpy
 	scikit-image
 	scipy
-	sunpy[map]>=3,!=3.1.0
+	sunpy[map]>=4
 
 [options.extras_require]
 docs = 
 	graphviz
 	importlib_metadata
 	pillow
 	reproject
@@ -49,15 +48,15 @@
 	sphinx-gallery
 	sphinx_rtd_theme
 	streamtracer
 	sunpy[net,map]
 	sympy
 test = 
 	numpy
-	parfive<2
+	parfive
 	pytest
 	pytest-cov
 	reproject
 	streamtracer
 	sympy
 performance = 
 	numba
@@ -77,14 +76,15 @@
 filterwarnings = 
 	error
 	ignore:numpy.ufunc size changed:RuntimeWarning
 	ignore:numpy.ndarray size changed, may indicate binary incompatibility:RuntimeWarning
 	ignore:Missing metadata for observer
 	ignore:unclosed <socket
 	ignore:unclosed transport
+	ignore:unclosed event loop
 	ignore:'datfix' made the change
 	ignore:The distutils package is deprecated
 	ignore:The distutils.sysconfig module is deprecated
 markers = 
 	remote_data
 
 [isort]
```

### Comparing `pfsspy-1.1.2/versioneer.py` & `pfsspy-1.2.0/versioneer.py`

 * *Files identical despite different names*


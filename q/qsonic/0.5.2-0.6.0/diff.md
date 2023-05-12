# Comparing `tmp/qsonic-0.5.2.tar.gz` & `tmp/qsonic-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsonic-0.5.2.tar", last modified: Sat Apr  1 01:30:22 2023, max compression
+gzip compressed data, was "qsonic-0.6.0.tar", last modified: Fri May 12 19:16:25 2023, max compression
```

## Comparing `qsonic-0.5.2.tar` & `qsonic-0.6.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:30:22.732282 qsonic-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-01 01:30:08.000000 qsonic-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-01 01:30:22.732282 qsonic-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-01 01:30:08.000000 qsonic-0.5.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:30:22.728282 qsonic-0.5.2/py/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:30:22.728282 qsonic-0.5.2/py/qsonic/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-01 01:30:08.000000 qsonic-0.5.2/py/qsonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-04-01 01:30:08.000000 qsonic-0.5.2/py/qsonic/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    13224 2023-04-01 01:30:08.000000 qsonic-0.5.2/py/qsonic/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    13526 2023-04-01 01:30:08.000000 qsonic-0.5.2/py/qsonic/masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-04-01 01:30:08.000000 qsonic-0.5.2/py/qsonic/mathtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-01 01:30:08.000000 qsonic-0.5.2/py/qsonic/mpi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    48382 2023-04-01 01:30:08.000000 qsonic-0.5.2/py/qsonic/picca_continuum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:30:22.732282 qsonic-0.5.2/py/qsonic/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-04-01 01:30:08.000000 qsonic-0.5.2/py/qsonic/scripts/qsonic_calib.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-04-01 01:30:08.000000 qsonic-0.5.2/py/qsonic/scripts/qsonic_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)    22558 2023-04-01 01:30:08.000000 qsonic-0.5.2/py/qsonic/spectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:30:22.732282 qsonic-0.5.2/py/qsonic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-01 01:30:22.000000 qsonic-0.5.2/py/qsonic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-01 01:30:22.000000 qsonic-0.5.2/py/qsonic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 01:30:22.000000 qsonic-0.5.2/py/qsonic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-01 01:30:22.000000 qsonic-0.5.2/py/qsonic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-01 01:30:22.000000 qsonic-0.5.2/py/qsonic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-01 01:30:22.000000 qsonic-0.5.2/py/qsonic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-01 01:30:08.000000 qsonic-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-01 01:30:08.000000 qsonic-0.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-01 01:30:22.732282 qsonic-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 01:30:08.000000 qsonic-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:30:22.732282 qsonic-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-04-01 01:30:08.000000 qsonic-0.5.2/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-04-01 01:30:08.000000 qsonic-0.5.2/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-01 01:30:08.000000 qsonic-0.5.2/tests/test_masks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-01 01:30:08.000000 qsonic-0.5.2/tests/test_mathtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-01 01:30:08.000000 qsonic-0.5.2/tests/test_mpi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-04-01 01:30:08.000000 qsonic-0.5.2/tests/test_picca_continuum.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-01 01:30:08.000000 qsonic-0.5.2/tests/test_qsonic_calib.py
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-04-01 01:30:08.000000 qsonic-0.5.2/tests/test_spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:16:25.790731 qsonic-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-12 19:16:07.000000 qsonic-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-12 19:16:25.790731 qsonic-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-12 19:16:07.000000 qsonic-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:16:25.786731 qsonic-0.6.0/py/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:16:25.786731 qsonic-0.6.0/py/qsonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-12 19:16:07.000000 qsonic-0.6.0/py/qsonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-12 19:16:07.000000 qsonic-0.6.0/py/qsonic/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-05-12 19:16:07.000000 qsonic-0.6.0/py/qsonic/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-05-12 19:16:07.000000 qsonic-0.6.0/py/qsonic/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-05-12 19:16:07.000000 qsonic-0.6.0/py/qsonic/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17279 2023-05-12 19:16:07.000000 qsonic-0.6.0/py/qsonic/mathtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-12 19:16:07.000000 qsonic-0.6.0/py/qsonic/mpi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49789 2023-05-12 19:16:07.000000 qsonic-0.6.0/py/qsonic/picca_continuum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:16:25.790731 qsonic-0.6.0/py/qsonic/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-05-12 19:16:07.000000 qsonic-0.6.0/py/qsonic/scripts/qsonic_calib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-05-12 19:16:07.000000 qsonic-0.6.0/py/qsonic/scripts/qsonic_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25437 2023-05-12 19:16:07.000000 qsonic-0.6.0/py/qsonic/spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:16:25.790731 qsonic-0.6.0/py/qsonic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-12 19:16:25.000000 qsonic-0.6.0/py/qsonic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-12 19:16:25.000000 qsonic-0.6.0/py/qsonic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 19:16:25.000000 qsonic-0.6.0/py/qsonic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-12 19:16:25.000000 qsonic-0.6.0/py/qsonic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-12 19:16:25.000000 qsonic-0.6.0/py/qsonic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 19:16:25.000000 qsonic-0.6.0/py/qsonic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-12 19:16:07.000000 qsonic-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-12 19:16:07.000000 qsonic-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-12 19:16:25.790731 qsonic-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 19:16:07.000000 qsonic-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:16:25.790731 qsonic-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-12 19:16:07.000000 qsonic-0.6.0/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-05-12 19:16:07.000000 qsonic-0.6.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-12 19:16:07.000000 qsonic-0.6.0/tests/test_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-12 19:16:07.000000 qsonic-0.6.0/tests/test_mathtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-12 19:16:07.000000 qsonic-0.6.0/tests/test_mpi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-05-12 19:16:07.000000 qsonic-0.6.0/tests/test_picca_continuum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-12 19:16:07.000000 qsonic-0.6.0/tests/test_qsonic_calib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-12 19:16:07.000000 qsonic-0.6.0/tests/test_spectrum.py
```

### Comparing `qsonic-0.5.2/LICENSE` & `qsonic-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qsonic-0.5.2/PKG-INFO` & `qsonic-0.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsonic
-Version: 0.5.2
+Version: 0.6.0
 Summary: Quasar continuum fitter for DESI
 Author: Naim Goksel Karacayli
 Author-email: ngokselk@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/p-slash/qsonic/issues
 Project-URL: Documentation, http://qsonic.readthedocs.io/
 Project-URL: Source, https://github.com/p-slash/qsonic
@@ -34,15 +34,16 @@
 **QSOnic** is an MPI-parallelized, highly optimized quasar continuum fitting package for DESI built on the same algorithm as `picca <https://github.com/igmhub/picca>`_, but *faster*. It also provides an efficient API to read DESI quasar spectra.
 
 The key differences
 -------------------
 - Coadding of spectrograph arms is optional and performed after continuum fitting.
 - Continuum is multiplied by a fiducial mean flux when provided.
 - You can pass fiducial var_lss (column ``VAR``) and mean flux (column ``MEANFLUX``) for observed wavelength ``LAMBDA`` in ``STATS`` extention of a FITS file. Wavelength should be linearly and equally spaced. This is the same format as rawio output from picca.
-- If no fiducial is passed, we fit only for var_lss (no eta fitting currently).
-- Internal weights for continuum fitting and coadding are based on smoothed ``IVAR``, but output ``WEIGHT`` is **not** smoothed.
+- If no fiducial is passed, we fit only for var_lss (no eta fitting by default). Eta fitting can be enabled, but is not recommended for Lya forest.
+- Internal weights for continuum fitting and coadding are based on smoothed ``IVAR``, and output ``WEIGHT`` is based on this smoothed ivar. This smoothing can be turned off.
 - Chi2 information as well as best fits are saved in continuum_chi2_catalog.fits. Chi2 is calculated using smooth ivar and var_lss, and does not subtract sum of ln(weights).
 
 Similarities
 ------------
 + Delta files are the same. `CONT` column is mean flux times continuum even when fiducial mean flux is passed.
 + ``MEANSNR`` in header file and chi2 catalog is average of flux times square root of positive ivar values. Header values are per arm, but catalog values are the average over all arms.
++ Eta fitting does not rescale ``IVAR`` output. Pipeline noise will be modified with explicit calibration option.
```

### Comparing `qsonic-0.5.2/README.rst` & `qsonic-0.6.0/py/qsonic.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: qsonic
+Version: 0.6.0
+Summary: Quasar continuum fitter for DESI
+Author: Naim Goksel Karacayli
+Author-email: ngokselk@gmail.com
+License: MIT
+Project-URL: Bug Reports, https://github.com/p-slash/qsonic/issues
+Project-URL: Documentation, http://qsonic.readthedocs.io/
+Project-URL: Source, https://github.com/p-slash/qsonic
+Requires-Python: >=3.7
+Provides-Extra: dev
+Provides-Extra: doc
+Provides-Extra: pub
+License-File: LICENSE
+
 ======
 QSOnic
 ======
 
 *Lightining-fast continuum fitting*
 
 .. image:: https://img.shields.io/pypi/v/qsonic?color=blue
@@ -18,15 +34,16 @@
 **QSOnic** is an MPI-parallelized, highly optimized quasar continuum fitting package for DESI built on the same algorithm as `picca <https://github.com/igmhub/picca>`_, but *faster*. It also provides an efficient API to read DESI quasar spectra.
 
 The key differences
 -------------------
 - Coadding of spectrograph arms is optional and performed after continuum fitting.
 - Continuum is multiplied by a fiducial mean flux when provided.
 - You can pass fiducial var_lss (column ``VAR``) and mean flux (column ``MEANFLUX``) for observed wavelength ``LAMBDA`` in ``STATS`` extention of a FITS file. Wavelength should be linearly and equally spaced. This is the same format as rawio output from picca.
-- If no fiducial is passed, we fit only for var_lss (no eta fitting currently).
-- Internal weights for continuum fitting and coadding are based on smoothed ``IVAR``, but output ``WEIGHT`` is **not** smoothed.
+- If no fiducial is passed, we fit only for var_lss (no eta fitting by default). Eta fitting can be enabled, but is not recommended for Lya forest.
+- Internal weights for continuum fitting and coadding are based on smoothed ``IVAR``, and output ``WEIGHT`` is based on this smoothed ivar. This smoothing can be turned off.
 - Chi2 information as well as best fits are saved in continuum_chi2_catalog.fits. Chi2 is calculated using smooth ivar and var_lss, and does not subtract sum of ln(weights).
 
 Similarities
 ------------
 + Delta files are the same. `CONT` column is mean flux times continuum even when fiducial mean flux is passed.
 + ``MEANSNR`` in header file and chi2 catalog is average of flux times square root of positive ivar values. Header values are per arm, but catalog values are the average over all arms.
++ Eta fitting does not rescale ``IVAR`` output. Pipeline noise will be modified with explicit calibration option.
```

### Comparing `qsonic-0.5.2/py/qsonic/catalog.py` & `qsonic-0.6.0/py/qsonic/catalog.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.5.2/py/qsonic/io.py` & `qsonic-0.6.0/py/qsonic/io.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,25 +52,23 @@
     outgroup.add_argument(
         "--outdir", '-o',
         help="Output directory to save deltas.")
     outgroup.add_argument(
         "--coadd-arms", action="store_true",
         help="Coadds arms when saving.")
     outgroup.add_argument(
-        "--save-smooth-weights", action="store_true",
-        help="Save smoothed weights instead.")
-    outgroup.add_argument(
         "--save-by-hpx", action="store_true",
         help="Save by healpix. If not, saves by MPI rank.")
     return parser
 
 
 def read_spectra_onehealpix(
         catalog_hpx, input_dir, arms_to_keep, mock_analysis, skip_resomat,
-        program="dark"):
+        program="dark"
+):
     """ Returns a list of Spectrum objects for a given catalog of a single
     healpix.
 
     Arguments
     ---------
     catalog_hpx: :external+numpy:py:class:`ndarray <numpy.ndarray>`
         Catalog of quasars in a single healpix. If for data 'SURVEY' column
@@ -79,15 +77,15 @@
         Input directory
     arms_to_keep: list(str)
         Must only contain B, R and Z
     mock_analysis: bool
         Reads for mock data if true.
     skip_resomat: bool
         If true, do not read resomat.
-    program: str
+    program: str, default: "dark"
         Always use dark program.
 
     Returns
     ---------
     spectra_list: list(Spectrum)
 
     Raises
@@ -130,14 +128,65 @@
                     cat_by_survey, data
                 )
             )
 
     return spectra_list
 
 
+def read_resolution_matrices_onehealpix_data(
+        catalog_hpx, input_dir, spectra_list, program="dark"
+):
+    """ Returns a list of Spectrum objects for a given catalog of a single
+    healpix.
+
+    Arguments
+    ---------
+    catalog_hpx: :external+numpy:py:class:`ndarray <numpy.ndarray>`
+        Catalog of quasars in a single healpix. If for data 'SURVEY' column
+        must be present and sorted.
+    input_dir: str
+        Input directory
+    spectra_list: list(Spectrum)
+        List of spectra to read resolution matrix
+    program: str, default: "dark"
+        Always use dark program.
+
+    Returns
+    ---------
+    spectra_list: list(Spectrum)
+
+    Raises
+    ---------
+    RuntimeWarning
+        If number of quasars in the healpix file does not match the catalog.
+    """
+    # assert (catalog_hpx.size == len(spectra_list))
+
+    unique_surveys, s2 = np.unique(
+        catalog_hpx['SURVEY'], return_index=True)
+    survey_split_cat = np.split(catalog_hpx, s2[1:])
+    s2 = np.append(s2, len(spectra_list))
+
+    arms_to_keep = spectra_list[0].wave.keys()
+
+    for ii, cat_by_survey in enumerate(survey_split_cat):
+        survey = cat_by_survey['SURVEY'][0]
+        pixnum = cat_by_survey['HPXPIXEL'][0]
+        targetids_by_survey = cat_by_survey['TARGETID']
+
+        fspec = (f"{input_dir}/{survey}/{program}/{pixnum//100}/"
+                 f"{pixnum}/coadd-{survey}-{program}-{pixnum}.fits")
+
+        i1, i2 = s2[ii], s2[ii + 1]
+        spectra_list[i1:i2] = _read_onehealpix_file_onlyreso(
+            targetids_by_survey, fspec, arms_to_keep, spectra_list[i1:i2])
+
+    return spectra_list
+
+
 def read_deltas(fname):
     """ Returns a list of all Delta objects in a file.
 
     Arguments
     ---------
     fname: str
         FITS file name
@@ -159,34 +208,29 @@
 
     fitsfile.close()
 
     return deltas_list
 
 
 def save_deltas(
-        spectra_list, outdir, varlss_interp,
-        save_by_hpx=False, mpi_rank=None, use_ivar_sm=False
+        spectra_list, outdir, save_by_hpx=False, mpi_rank=None
 ):
     """ Saves given list of spectra as deltas. NO coaddition of arms.
     Each arm is saved separately. Only valid spectra are saved.
 
     Arguments
     ---------
     spectra_list: list(Spectrum)
         Continuum fitted spectra objects. All must be valid!
     outdir: str
         Output directory. Does not save if empty of None
-    varlss_interp: Interpolator
-        Interpolator for LSS variance
     save_by_hpx: bool, default: False
         Saves by healpix if True. Has priority over mpi_rank
     mpi_rank: int, default: None
         Rank of the MPI process. Save by `mpi_rank` if passed.
-    use_ivar_sm: bool, default: False
-        Use :attr:`Spectrum.forestivar_sm` in weights instead.
 
     Raises
     ---------
     QsonicException
         If both `mpi_rank` and `save_by_hpx` is None/False.
     QsonicException
         If blinding is not set.
@@ -210,15 +254,15 @@
         raise QsonicException("Blinding is not set. Cannot save delta.")
 
     for healpix, hp_specs in zip(unique_pix, split_spectra):
         results = fitsio.FITS(
             f"{outdir}/delta-{healpix}.fits", 'rw', clobber=True)
 
         for spec in qsonic.spectrum.valid_spectra(hp_specs):
-            spec.write(results, varlss_interp, use_ivar_sm)
+            spec.write(results)
 
         results.close()
 
 
 def _read_resoimage(imhdu, quasar_indices, nwave):
     # Reading into sorted order is faster
     # Since the output catalog is already sorted, we place them in order
@@ -244,15 +288,16 @@
 #     ndims = imhdu.get_info()['ndims']
 #     if ndims == 2:
 #         return np.vstack([imhdu[int(idx), :] for idx in quasar_indices])
 #     return np.vstack([imhdu[int(idx), :, :] for idx in quasar_indices])
 
 
 def _read_onehealpix_file(
-        targetids_by_survey, fspec, arms_to_keep, skip_resomat):
+        targetids_by_survey, fspec, arms_to_keep, skip_resomat
+):
     """ Common function to read a single fits file.
 
     Arguments
     ---------
     targetids_by_survey: :external+numpy:py:class:`ndarray <numpy.ndarray>`
         Targetids_by_survey (used to be catalog). If data, split by survey and
         contains only one survey.
@@ -286,16 +331,14 @@
     if (common_targetids.size != targetids_by_survey.size):
         warnings.warn(
             f"Error reading {fspec}. "
             "Number of quasars in healpix does not match the catalog "
             f"catalog:{targetids_by_survey.size} vs "
             f"healpix:{common_targetids.size}!", RuntimeWarning)
 
-    fbrmap = fbrmap[idx_fbr]
-
     data = {
         'wave': {},
         'flux': {},
         'ivar': {},
         'mask': {},
         'reso': {}
     }
@@ -319,16 +362,76 @@
             fitsfile[f'{arm}_RESOLUTION'], idx_fbr, nwave)
 
     fitsfile.close()
 
     return data, idx_cat
 
 
+def _read_onehealpix_file_onlyreso(
+        targetids_by_survey, fspec, arms_to_keep, spectra_list
+):
+    """ Function to read forest region resolution matrix for data. Note reading
+    resolution matrix is already fast for mocks.
+
+    Arguments
+    ---------
+    targetids_by_survey: :external+numpy:py:class:`ndarray <numpy.ndarray>`
+        Targetids_by_survey (used to be catalog). If data, split by survey and
+        contains only one survey.
+    fspec: str
+        Filename to open.
+    arms_to_keep: list(str)
+        Must only contain B, R and Z.
+    spectra_list: list(Spectrum)
+        List of spectra that forest region is set. Modified in place and also
+        returned.
+
+    Returns
+    ---------
+    spectra_list: list(Spectrum)
+        List of spectra where forestreso is set.
+
+    Raises
+    ---------
+    RuntimeWarning
+        If number of quasars in the healpix file does not match the catalog.
+    """
+    fitsfile = fitsio.FITS(fspec)
+
+    fbrmap = fitsfile['FIBERMAP'].read(columns='TARGETID')
+    common_targetids, idx_fbr, idx_cat = np.intersect1d(
+        fbrmap, targetids_by_survey, assume_unique=True, return_indices=True)
+    if (common_targetids.size != targetids_by_survey.size):
+        warnings.warn(
+            f"Error reading {fspec}. "
+            "Number of quasars in healpix does not match the catalog "
+            f"catalog:{targetids_by_survey.size} vs "
+            f"healpix:{common_targetids.size}!", RuntimeWarning)
+
+    for arm in arms_to_keep:
+        imhdu = fitsfile[f'{arm}_RESOLUTION']
+
+        for jj, spec in zip(idx_fbr, spectra_list):
+            # assert (common_targetids[jj] == spec.targetid)
+
+            if arm not in spec.forestwave.keys():
+                continue
+
+            f1 = spec._f1[arm]
+            f2 = spec._f2[arm]
+            spec._forestreso[arm] = imhdu[int(jj), :, f1:f2][0]
+
+    fitsfile.close()
+
+    return spectra_list
+
+
 def read_onehealpix_file_data(
-        cat_by_survey, input_dir, arms_to_keep, skip_resomat, program="dark"):
+        cat_by_survey, input_dir, arms_to_keep, skip_resomat, program="dark"
+):
     """ Read a single fits file for data.
 
     Arguments
     ---------
     cat_by_survey: :external+numpy:py:class:`ndarray <numpy.ndarray>`
         Catalog for a single survey and healpix. Ordered by TARGETID.
     input_dir: str
@@ -359,15 +462,16 @@
     data, idx_cat = _read_onehealpix_file(
         cat_by_survey['TARGETID'], fspec, arms_to_keep, skip_resomat)
 
     return data, idx_cat
 
 
 def read_onehealpix_file_mock(
-        catalog_hpx, input_dir, arms_to_keep, skip_resomat, nside=16):
+        catalog_hpx, input_dir, arms_to_keep, skip_resomat, nside=16
+):
     """ Read a single FITS file for mocks.
 
     Arguments
     ---------
     catalog_hpx: :external+numpy:py:class:`ndarray <numpy.ndarray>`
         Catalog for a single healpix. Ordered by TARGETID.
     input_dir: str
```

### Comparing `qsonic-0.5.2/py/qsonic/masks.py` & `qsonic-0.6.0/py/qsonic/masks.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 from astropy.io.ascii import read as asread
 import numpy as np
 from numpy.lib.recfunctions import rename_fields
 import fitsio
 
 from qsonic import QsonicException
+from qsonic.mpi_utils import mpi_fnc_bcast
+
 
 LIGHT_SPEED = 299792.458
 """float: Speed of light in km/s."""
 sqrt_pi = 1.77245385091
 """float: Square root of pi."""
 sqrt_2 = 1.41421356237
 """float: Square root of 2."""
@@ -52,27 +54,28 @@
 
     Parameters
     ----------
     fname: str
         Filename to read by `astropy.io.ascii`. Must have four columns ordered
         as type, minimum wavelength, maximum wavelength and frame (must be 'RF'
         or 'OBS').
+    comm: None or MPI.COMM_WORLD, default: None
+    mpi_rank: int, default: 0
     """
     column_names = ('type', 'wave_min', 'wave_max', 'frame')
     """tuple: Assumed ordering of columns in the text file."""
 
-    def __init__(self, fname):
-        try:
-            mask = asread(fname, names=SkyMask.column_names)
-
-            self.mask_rest_frame = mask[mask['frame'] == 'RF']
-            self.mask_obs_frame = mask[mask['frame'] == 'OBS']
-        except Exception as e:
-            raise QsonicException(
-                f"Error loading SkyMask from mask file {fname}.") from e
+    def __init__(self, fname, comm=None, mpi_rank=0):
+        mask = mpi_fnc_bcast(
+            asread, comm, mpi_rank,
+            f"Error loading SkyMask from mask file {fname}.",
+            fname, names=SkyMask.column_names)
+
+        self.mask_rest_frame = mask[mask['frame'] == 'RF']
+        self.mask_obs_frame = mask[mask['frame'] == 'OBS']
 
     def apply(self, spec):
         """ Apply the mask by setting **only** ``spec.forestivar`` to zero.
 
         Arguments
         ----------
         spec: Spectrum
@@ -381,15 +384,17 @@
         fts = fitsio.FITS(fname)
 
         fts_colnames = set(fts["DLACAT"].get_colnames())
         z_colname = fts_colnames.intersection(DLAMask.accepted_zcolnames)
 
         if not z_colname:
             fts.close()
-            return None
+            raise ValueError(
+                "DLA mask error::Z colname has to be one of "
+                f"{', '.join(DLAMask.accepted_zcolnames)}")
 
         z_colname = z_colname.pop()
         columns_list = ["TARGETID", z_colname, "NHI"]
         catalog = fts['DLACAT'].read(columns=columns_list)
 
         if z_colname != 'Z_DLA':
             catalog = rename_fields(catalog, {z_colname: 'Z_DLA'})
@@ -397,27 +402,20 @@
         fts.close()
 
         return catalog
 
     def __init__(
             self, fname, local_targetids=None, comm=None, mpi_rank=0,
             dla_mask_limit=0.8):
-        catalog = None
         self.dla_mask_limit = dla_mask_limit
 
-        if mpi_rank == 0:
-            catalog = DLAMask._read_catalog(fname)
-
-        if comm is not None:
-            catalog = comm.bcast(catalog)
-
-        if catalog is None:
-            raise ValueError(
-                "DLA mask error::Z colname has to be one of "
-                f"{', '.join(DLAMask.accepted_zcolnames)}")
+        catalog = mpi_fnc_bcast(
+            DLAMask._read_catalog, comm, mpi_rank,
+            f"Error loading DLAMask from file {fname}.",
+            fname)
 
         if local_targetids is not None:
             w = np.isin(catalog['TARGETID'], local_targetids)
             catalog = catalog[w]
         catalog.sort(order='TARGETID')
 
         # Group DLA catalog into targetids
```

### Comparing `qsonic-0.5.2/py/qsonic/mathtools.py` & `qsonic-0.6.0/py/qsonic/mathtools.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,89 @@
 """Mathematical utility objects and functions."""
 import numpy as np
 from numba import njit
 
 from qsonic import QsonicException
 
 
+def _zero_function(x):
+    return 0
+
+
+def _one_function(x):
+    return 1
+
+
 @njit("f8[:](f8[:], f8, f8, f8[:])")
-def _fast_eval_interp1d(x, xp0, dxp, fp):
+def _fast_eval_interp1d_lin(x, xp0, dxp, fp):
+    """JIT fast linear interpolation."""
     xx = (x - xp0) / dxp
     idx = np.clip(xx, 0, fp.size - 1 - 1e-8).astype(np.int_)
 
     d_idx = xx - idx
     y1, y2 = fp[idx], fp[idx + 1]
 
     return y1 * (1 - d_idx) + y2 * d_idx
 
 
+@njit("f8[:](f8[:], f8, f8, f8[:], f8[:])")
+def _fast_eval_interp1d_cubic(x, xp0, dxp, fp, y2p):
+    """JIT fast cubic spline."""
+    xx = (x - xp0) / dxp
+    idx = np.clip(xx, 0, fp.size - 1 - 1e-8).astype(np.int_)
+
+    d_idx = xx - idx
+    a, b = 1 - d_idx, d_idx
+    y1, y2 = fp[idx], fp[idx + 1]
+    ypp1, ypp2 = y2p[idx], y2p[idx + 1]
+
+    r1 = a * y1 + b * y2
+    r2 = ((a + 1) * ypp1 + (b + 1) * ypp2) * (-a * b * dxp**2 / 6.)
+
+    return r1 + r2
+
+
+@njit("f8[:](f8[:], f8)")
+def _spline_cubic(fp, dxp):
+    """ Constructs the second derivative array.
+
+    As coded in Numerical Recipes in C Chaper 3.3, but specialized for equally
+    spaced input data.
+
+    Arguments
+    ---------
+    fp: ndarray
+        1D data points array to interpolate.
+    dxp: float
+        Spacing of x points.
+
+    Returns
+    -------
+    y2p: ndarray
+        Second derivative array. Same size as ``fp``.
+    """
+    y2p = np.empty(fp.size)
+    u = np.empty(fp.size - 1)
+    u[0] = 0
+    y2p[0] = y2p[-1] = 0
+
+    sig = 0.5
+
+    for ii in range(1, fp.size - 1):
+        p = sig * y2p[ii - 1] + 2.
+        y2p[ii] = (sig - 1) / p
+        u[ii] = (fp[ii + 1] + fp[ii - 1] - 2 * fp[ii]) / dxp
+        u[ii] = (3 * u[ii] / dxp - sig * u[ii - 1]) / p
+
+    for ii in range(fp.size - 2, 0, -1):
+        y2p[ii] = y2p[ii] * y2p[ii + 1] + u[ii]
+
+    return y2p
+
+
 @njit("f8[:](f8[:], f8[:])")
 def mypoly1d(coef, x):
     """ My simple power series polynomial calculator.
 
     Arguments
     ---------
     coef: :external+numpy:py:class:`ndarray <numpy.ndarray>`
@@ -34,14 +98,60 @@
     """
     results = np.zeros_like(x)
     for i, a in enumerate(coef):
         results += a * x**i
     return results
 
 
+@njit("f8[:, :, :](f8[:], f8[:], f8[:, :, :])")
+def block_covariance_of_square(mean, var, cov):
+    """ Return the block covariance of x^2, i.e.
+    :math:`<x_i^2 x_j^2> - <x_i^2><x_j^2>`. Compatible with ``blockdim``
+    argument of :meth:`SubsampleCov.get_mean_n_cov`.
+
+    .. math::
+
+        Cov[x_i^2, x_j^2] &= Var[x_i] Var[x_j] + Cov(x_i, x_j)^2 \\\\
+        &+ 2 Cov(x_i, x_j) E[x_i] E[x_j] \\\\
+        &+  Var[x_i] E[x_j]^2 + Var[x_j] E[x_i]^2
+
+    Arguments
+    ---------
+    mean: :external+numpy:py:class:`ndarray <numpy.ndarray>`
+        1D array mean values.
+    var: :external+numpy:py:class:`ndarray <numpy.ndarray>`
+        1D array variance values.
+    cov: :external+numpy:py:class:`ndarray <numpy.ndarray>`
+        3D array covariance. Shape is ``(nblock, ndata, ndata)``.
+
+    Returns
+    -------
+    new_cov: :external+numpy:py:class:`ndarray <numpy.ndarray>`
+        3D array propagated covariance.
+    """
+    nblock = cov.shape[0]
+    ndata = cov.shape[1]
+    new_cov = np.empty_like(cov)
+
+    for jj in range(nblock):
+        i1 = jj * ndata
+        i2 = i1 + ndata
+        v = var[i1:i2]
+        m = mean[i1:i2]
+
+        np.outer(v, v, out=new_cov[jj])
+        new_cov[jj] += cov[jj]**2
+        new_cov[jj] += 2 * cov[jj] * np.outer(m, m)
+
+        C1 = np.outer(v, m**2)
+        new_cov[jj] += C1 + C1.T
+
+    return new_cov
+
+
 def fft_gaussian_smooth(x, sigma_pix=20, mode='edge'):
     """ My Gaussian smoother using FFTs. Input array is padded with edge
     values at the boundary by default. Pad size is ``3*sigma_pix``.
 
     Arguments
     ---------
     x: :external+numpy:py:class:`ndarray <numpy.ndarray>`
@@ -110,48 +220,103 @@
     error[w2] = err_org
     ivar2 = 1 / error**2
     ivar2[~w1] = 0
 
     return ivar2
 
 
-class Fast1DInterpolator():
+class FastLinear1DInterp():
     """Fast interpolator class for equally spaced data. Out of domain points
     are linearly extrapolated without producing any warnings or errors.
 
+    Uses :func:`_fast_eval_interp1d_lin`.
+
     Example::
 
-        one_interp = Fast1DInterpolator(0., 1., np.ones(3))
+        one_interp = FastLinear1DInterp(0., 1., np.ones(3))
         one_interp(5) # = 1
 
     Parameters
     ----------
     xp0: float
         Initial x point for interpolation data.
-    dxp0: float
+    dxp: float
         Spacing of x points.
     fp: :external+numpy:py:class:`ndarray <numpy.ndarray>`
         Function calculated at interpolation points.
+    copy: bool, default: False
+        Copy input data, specifically fp.
     ep: :external+numpy:py:class:`ndarray <numpy.ndarray>`, optional
         Error on fp points. Not used! Bookkeeping purposes only.
+    """
+
+    def __init__(self, xp0, dxp, fp, copy=False, ep=None):
+        self.xp0 = float(xp0)
+        self.dxp = float(dxp)
+        if copy:
+            self.fp = fp.copy()
+        else:
+            self.fp = fp
+        self.ep = ep
+
+    def __call__(self, x):
+        return _fast_eval_interp1d_lin(x, self.xp0, self.dxp, self.fp)
+
+    def reset(self, fp, copy=False, ep=None):
+        if copy:
+            self.fp = fp.copy()
+        else:
+            self.fp = fp
+
+        self.ep = ep
+
+
+class FastCubic1DInterp():
+    """ Fast cubic spline for equally spaced data. Out of domain points
+    are linearly extrapolated without producing any warnings or errors.
+
+    Uses :func:`_spline_cubic` and :func:`_fast_eval_interp1d_cubic`.
+
+    Parameters
+    ----------
+    xp0: float
+        Initial x point for interpolation data.
+    dxp: float
+        Spacing of x points.
+    fp: :external+numpy:py:class:`ndarray <numpy.ndarray>`
+        Function calculated at interpolation points.
     copy: bool, default: False
         Copy input data, specifically fp.
+    ep: :external+numpy:py:class:`ndarray <numpy.ndarray>`, optional
+        Error on fp points. Not used! Bookkeeping purposes only.
     """
 
     def __init__(self, xp0, dxp, fp, copy=False, ep=None):
         self.xp0 = float(xp0)
         self.dxp = float(dxp)
         if copy:
             self.fp = fp.copy()
         else:
             self.fp = fp
+        self._y2p = _spline_cubic(fp, dxp)
         self.ep = ep
 
     def __call__(self, x):
-        return _fast_eval_interp1d(x, self.xp0, self.dxp, self.fp)
+        return _fast_eval_interp1d_cubic(
+            x, self.xp0, self.dxp, self.fp, self._y2p)
+
+    def reset(self, fp, copy=False, ep=None):
+        if copy:
+            self.fp = fp.copy()
+        else:
+            self.fp = fp
+
+        self.ep = ep
+
+        self._y2p = _spline_cubic(fp, self.dxp)
 
 
 class SubsampleCov():
     """Utility class to store all subsamples with weights and calculate
     the delete-one Jackknife covariance matrix.
 
     Usage::
@@ -168,48 +333,49 @@
 
             You cannot call :meth:`add_measurement` after calling
             :meth:`get_mean`, :meth:`get_mean_n_cov`,
             or :meth:`get_mean_n_var`.
 
     Parameters
     ----------
-    ndata: int
-        Size of the data vector.
+    ndata: int or tuple(int)
+        Size or shape of the data vector. If tuple, it should be
+        ``(nset, size1d)``. For example, 3 quantities share the same
+        weights, data vector shape should pass ``ndata=(3, size1d)``.
     nsamples: int
-        Number of samples.
+        Number of samples. You can add more measurements then this.
     istart: int, default: 0
         Start index for the subsampling array
 
     Attributes
     ----------
-    ndata: int or tuple(int)
-        Size or shape of the data vector. If 3 quantities share the same
-        weights, data vector shape should be (3, size1d).
-    nsamples: int
-        Number of samples. You can more measurements then this.
+    _istart: int
+        Sampler initial index.
     _isample: int
         Sample counter. Wraps around nsamples
     _is_normalized: bool
         If the weights are normalized. Keeps track if :func:`_normalize` is
         called.
     all_measurements: :external+numpy:py:class:`ndarray <numpy.ndarray>`
-        2D array of zeros of shape ``(nsamples, ndata)``.
+        3D array of shape ``(nsamples, nset, ndata)``.
     all_weights: :external+numpy:py:class:`ndarray <numpy.ndarray>`
-        2D array of zeros of shape ``(nsamples, ndata)``.
+        3D array of shape ``(nsamples, nset, ndata)``.
     mean: :class:`ndarray <numpy.ndarray>` or None
-        Mean. 1D array of size ``ndata``
-    covariance: :class:`ndarray <numpy.ndarray>` or None
-        Covariance. 2D array of shape ``(ndata, ndata)``
+        Mean. 2D array of shape ``(nset, ndata)``
     variance: :class:`ndarray <numpy.ndarray>` or None
-        Variance. 1D array of size ``ndata``
+        Variance. 2D array of shape ``(nset, ndata)``
+    covariance: list(:class:`ndarray <numpy.ndarray>`) or None
+        Covariance. 2D arrays of shape ``(ndata, ndata)`` or 3D arrays of
+        shape ``(nblock, blockdim, blockdim)``.
     """
 
     def __init__(self, ndata, nsamples, istart=0):
         self.nsamples = nsamples
-        self._isample = istart % nsamples
+        self._istart = istart % nsamples
+        self._isample = self._istart
 
         if isinstance(ndata, int):
             newshape = (nsamples, 1, ndata)
             self.ndata = ndata
         elif isinstance(ndata, tuple):
             newshape = (nsamples, ndata[0], ndata[1])
             self.ndata = ndata[1]
@@ -311,46 +477,67 @@
             bias_jack = (self.nsamples - 1) * (mean_jack - mean_xvec)
             mean_xvec -= bias_jack
 
         xdiff = jack_i - mean_jack
 
         return mean_xvec, xdiff
 
-    def get_mean_n_cov(self, bias_correct=False):
+    def _get_block_covariance(self, x, blockdim):
+        nblock = self.ndata // blockdim
+        cov = np.empty((nblock, blockdim, blockdim), dtype=np.float_)
+        for kk in range(nblock):
+            y = x[:, kk * blockdim:(kk + 1) * blockdim]
+            cov[kk] = (y.T @ y) * (self.nsamples - 1) / self.nsamples
+
+        return cov
+
+    def get_mean_n_cov(self, indices=None, blockdim=None, bias_correct=False):
         """ Get the mean and covariance of the mean using delete-one Jackknife.
 
         Also sets :attr:`mean` and :attr:`covariance`.
 
         .. warning::
 
             You cannot call :meth:`add_measurement` after calling this unless
             you :meth:`reset`.
 
         Arguments
         ---------
+        indices: list(int), default: None
+            Data set indices to estimate the covariance.
+        blockdim: int, default: None
+            Calculate covariance by this block size instead of the full space.
         bias_correct: bool, default: False
             Jackknife bias correction term for the mean.
 
         Returns
         -------
         mean: :class:`ndarray <numpy.ndarray>`
             Mean.
-        cov: :class:`ndarray <numpy.ndarray>`
-            Covariance of the mean. 2D array
+        cov: list(:class:`ndarray <numpy.ndarray>`)
+            Covariances of the mean.
         """
         mean_xvec = self.get_mean()
         self.mean, xdiff = self._get_xdiff(mean_xvec, bias_correct)
 
-        covshape = (self.all_measurements.shape[1], self.ndata, self.ndata)
-        self.covariance = np.empty(covshape)
-        for jj in range(self.all_measurements.shape[1]):
+        if indices is None:
+            indices = range(self.all_measurements.shape[1])
+
+        if blockdim is not None:
+            assert (self.ndata % blockdim == 0)
+
+        self.covariance = [None] * self.all_measurements.shape[1]
+        for jj in indices:
             x = xdiff[:, jj, :]
-            self.covariance[jj] = (
-                np.dot(x.T, x) * (self.nsamples - 1) / self.nsamples
-            )
+
+            if blockdim is None:
+                cov = (x.T @ x) * (self.nsamples - 1) / self.nsamples
+            else:
+                cov = self._get_block_covariance(x, blockdim)
+            self.covariance[jj] = cov
 
         return self.mean, self.covariance
 
     def get_mean_n_var(self, bias_correct=False):
         """ Get the mean and variance of themean (i.e. diagonal of the
         covariance) using delete-one Jackknife.
 
@@ -376,16 +563,16 @@
 
         self.variance = (
             np.sum(xdiff**2, axis=0) * (self.nsamples - 1) / self.nsamples
         )
 
         return self.mean, self.variance
 
-    def reset(self, istart=0):
-        self._isample = istart % self.nsamples
+    def reset(self):
+        self._isample = self._istart
 
         self.all_measurements *= 0
         self.all_weights *= 0
         self._is_normalized = False
 
         self.mean = None
         self.covariance = None
```

### Comparing `qsonic-0.5.2/py/qsonic/mpi_utils.py` & `qsonic-0.6.0/py/qsonic/mpi_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -112,15 +112,16 @@
         If any error occur while doing ``fnc``.
     """
     result = _INVALID_VALUE
     if (mpi_rank == 0 or comm is None):
         try:
             result = fnc(*args, **kwargs)
         except Exception as e:
-            logging_mpi(f"{fnc.__module__}.{fnc.__name__}: {e}", 0, "error")
+            logging.exception(e)
+            logging.error(f"Error in {fnc.__module__}.{fnc.__name__}.")
             result = _INVALID_VALUE
 
     if comm is not None:
         result = comm.bcast(result)
 
     if result is _INVALID_VALUE:
         raise QsonicException(err_msg)
```

### Comparing `qsonic-0.5.2/py/qsonic/picca_continuum.py` & `qsonic-0.6.0/py/qsonic/picca_continuum.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,20 @@
 from scipy.interpolate import UnivariateSpline
 from scipy.special import legendre
 
 from mpi4py import MPI
 
 from qsonic import QsonicException
 from qsonic.spectrum import valid_spectra
-from qsonic.mpi_utils import logging_mpi, warn_mpi, MPISaver
-from qsonic.mathtools import mypoly1d, Fast1DInterpolator, SubsampleCov
+from qsonic.mpi_utils import logging_mpi, warn_mpi, mpi_fnc_bcast, MPISaver
+from qsonic.mathtools import (
+    mypoly1d, block_covariance_of_square,
+    FastLinear1DInterp, FastCubic1DInterp,
+    SubsampleCov
+)
 
 
 def add_picca_continuum_parser(parser=None):
     """ Adds PiccaContinuumFitter related arguments to parser. These
     arguments are grouped under 'Continuum fitting options'. All of them
     come with defaults, none are required.
 
@@ -45,24 +49,23 @@
         "--fiducial-meanflux", help="Fiducial mean flux FITS file.")
     cont_group.add_argument(
         "--fiducial-varlss", help="Fiducial var_lss FITS file.")
     cont_group.add_argument(
         "--cont-order", type=int, default=1,
         help="Order of continuum fitting polynomial.")
     cont_group.add_argument(
-        "--fit-eta", action="store_true",
-        help="NOT IMPLEMENTED: Fit for noise calibration (eta).")
+        "--var-fit-eta", action="store_true",
+        help="Fit for noise calibration (eta).")
+    cont_group.add_argument(
+        "--var-use-cov", action="store_true",
+        help="Use covariance in varlss-eta fitting.")
     cont_group.add_argument(
         "--normalize-stacked-flux", action="store_true",
         help="NOT IMPLEMENTED: Force stacked flux to be one at the end.")
     cont_group.add_argument(
-        "--error-method-vardelta", default="regJack",
-        choices=VarLSSFitter.accepted_vardelta_error_methods,
-        help="Error estimation method for var_delta.")
-    cont_group.add_argument(
         "--minimizer", default="iminuit", choices=["iminuit", "l_bfgs_b"],
         help="Minimizer to fit the continuum.")
 
     return parser
 
 
 class PiccaContinuumFitter():
@@ -88,116 +91,102 @@
     ----------
     nbins: int
         Number of bins for the mean continuum in the rest frame.
     rfwave: :external+numpy:py:class:`ndarray <numpy.ndarray>`
         Rest-frame wavelength centers for the mean continuum.
     _denom: float
         Denominator for the slope term in the continuum model.
-    meancont_interp: Fast1DInterpolator
-        Fast linear interpolator object for the mean continuum.
+    meancont_interp: FastCubic1DInterp
+        Fast cubic spline object for the mean continuum.
     minimizer: function
         Function that points to one of the minimizer options.
     comm: MPI.COMM_WORLD
         MPI comm object to reduce, broadcast etc.
     mpi_rank: int
         Rank of the MPI process.
-    meanflux_interp: Fast1DInterpolator
+    meanflux_interp: FastLinear1DInterp
         Interpolator for mean flux. If fiducial is not set, this equals to 1.
-    flux_stacker: FluxStacker (disabled)
+    flux_stacker: FluxStacker
         Stacks flux. Set up with 8 A wavelength bin size.
     varlss_fitter: VarLSSFitter or None
         None if fiducials are set for var_lss.
-    varlss_interp: Fast1DInterpolator
-        Interpolator for var_lss.
+    varlss_interp: FastLinear1DInterp or FastCubic1DInterp
+        Cubic spline for var_lss if fitting. Linear if from file.
+    eta_interp: FastCubic1DInterp
+        Interpolator for eta. Returns one if fiducial var_lss is set.
     niterations: int
         Number of iterations from `args.no_iterations`.
     cont_order: int
         Order of continuum polynomial from `args.cont_order`.
     outdir: str or None
         Directory to save catalogs. If None or empty, does not save.
+    fit_eta: bool
+        True if fitting eta and fiducial var_lss is not set.
     """
 
     def _get_fiducial_interp(self, fname, col2read):
         """ Return an interpolator for mean flux or var_lss.
 
         FITS file must have a 'STATS' extention, which must have 'LAMBDA',
         'MEANFLUX' and 'VAR' columns. This is the same format as raw_io output
         from picca. 'LAMBDA' must be linearly and equally spaced.
-        This function sets up ``col2read`` as Fast1DInterpolator object.
+        This function sets up ``col2read`` as FastLinear1DInterp object.
 
         Arguments
         ---------
         fname: str
             Filename of the FITS file.
         col2read: str
             Should be 'MEANFLUX' or 'VAR'.
 
         Returns
         -------
-        Fast1DInterpolator
+        FastLinear1DInterp
 
         Raises
         ------
         QsonicException
             If 'LAMBDA' is not equally spaced or ``col2read`` is not in the
             file.
         """
-        if self.mpi_rank == 0:
+        def _read(fname, col2read):
             with fitsio.FITS(fname) as fts:
                 data = fts['STATS'].read()
 
             waves = data['LAMBDA']
             waves_0 = waves[0]
             dwave = waves[1] - waves[0]
             nsize = waves.size
 
             if not np.allclose(np.diff(waves), dwave):
-                # Set nsize to 0, later will be used to diagnose and exit
-                # for uneven wavelength array.
-                nsize = 0
-            elif col2read not in data.dtype.names:
-                nsize = -1
-            else:
-                data = np.array(data[col2read], dtype='d')
-        else:
-            waves_0 = 0.
-            dwave = 0.
-            nsize = 0
-
-        nsize, waves_0, dwave = self.comm.bcast([nsize, waves_0, dwave])
-
-        if nsize == 0:
-            raise QsonicException(
-                "Failed to construct fiducial mean flux or varlss from "
-                f"{fname}::LAMBDA is not equally spaced.")
-
-        if nsize == -1:
-            raise QsonicException(
-                "Failed to construct fiducial mean flux or varlss from "
-                f"{fname}::{col2read} is not in file.")
-
-        if self.mpi_rank != 0:
-            data = np.empty(nsize, dtype='d')
-
-        self.comm.Bcast([data, MPI.DOUBLE])
-
-        return Fast1DInterpolator(waves_0, dwave, data, ep=np.zeros(nsize))
+                raise Exception(
+                    "Failed to construct fiducial mean flux or varlss from "
+                    f"{fname}::LAMBDA is not equally spaced.")
+
+            data = np.array(data[col2read], dtype='d')
+
+            return FastLinear1DInterp(waves_0, dwave, data, ep=np.zeros(nsize))
+
+        return mpi_fnc_bcast(
+            _read, self.comm, self.mpi_rank,
+            f"Failed to construct fiducial mean flux or varlss from {fname}.",
+            fname, col2read)
 
     def __init__(self, args):
         # We first decide how many bins will approximately satisfy
         # rest-frame wavelength spacing. Then we create wavelength edges, and
         # transform these edges into centers
         self.nbins = int(round(
             (args.forest_w2 - args.forest_w1) / args.rfdwave))
         edges, self.dwrf = np.linspace(
             args.forest_w1, args.forest_w2, self.nbins + 1, retstep=True)
         self.rfwave = (edges[1:] + edges[:-1]) / 2
         self._denom = np.log(self.rfwave[-1] / self.rfwave[0])
 
-        self.meancont_interp = Fast1DInterpolator(
+        self.meancont_interp = FastCubic1DInterp(
             self.rfwave[0], self.dwrf, np.ones(self.nbins),
             ep=np.zeros(self.nbins))
 
         if args.minimizer == "iminuit":
             self.minimizer = self._iminuit_minimizer
         elif args.minimizer == "l_bfgs_b":
             self.minimizer = self._scipy_l_bfgs_b_minimizer
@@ -208,37 +197,42 @@
         self.comm = MPI.COMM_WORLD
         self.mpi_rank = self.comm.Get_rank()
 
         if args.fiducial_meanflux:
             self.meanflux_interp = self._get_fiducial_interp(
                 args.fiducial_meanflux, 'MEANFLUX')
         else:
-            self.meanflux_interp = Fast1DInterpolator(
+            self.meanflux_interp = FastLinear1DInterp(
                 args.wave1, args.wave2 - args.wave1, np.ones(3))
 
-        # self.flux_stacker = FluxStacker(
-        #     args.wave1, args.wave2, 8., comm=self.comm)
+        self.flux_stacker = FluxStacker(
+            args.wave1, args.wave2, 8., comm=self.comm)
 
         if args.fiducial_varlss:
             self.varlss_fitter = None
             self.varlss_interp = self._get_fiducial_interp(
                 args.fiducial_varlss, 'VAR')
         else:
             self.varlss_fitter = VarLSSFitter(
-                args.wave1, args.wave2,
-                error_method=args.error_method_vardelta,
+                args.wave1, args.wave2, use_cov=args.var_use_cov,
                 comm=self.comm)
-            self.varlss_interp = Fast1DInterpolator(
+            self.varlss_interp = FastCubic1DInterp(
                 self.varlss_fitter.waveobs[0], self.varlss_fitter.dwobs,
                 0.1 * np.ones(self.varlss_fitter.nwbins),
                 ep=np.zeros(self.varlss_fitter.nwbins))
 
+        self.eta_interp = FastCubic1DInterp(
+            self.varlss_interp.xp0, self.varlss_interp.dxp,
+            np.ones_like(self.varlss_interp.fp),
+            ep=np.zeros_like(self.varlss_interp.fp))
+
         self.niterations = args.no_iterations
         self.cont_order = args.cont_order
         self.outdir = args.outdir
+        self.fit_eta = args.var_fit_eta
 
     def _continuum_costfn(self, x, wave, flux, ivar_sm, z_qso):
         """ Cost function to minimize for each quasar.
 
         This is a modified chi2 where amplitude is also part of minimization.
         Cost of each arm is simply added to the total cost.
 
@@ -266,15 +260,16 @@
             cont_est = self.get_continuum_model(x, wave_arm / (1 + z_qso))
             # no_neg = np.sum(cont_est<0)
             # penalty = wave_arm.size * no_neg**2
 
             cont_est *= self.meanflux_interp(wave_arm)
 
             var_lss = self.varlss_interp(wave_arm) * cont_est**2
-            weight = ivar_sm[arm] / (1 + ivar_sm[arm] * var_lss)
+            eta = self.eta_interp(wave_arm)
+            weight = ivar_sm[arm] / (eta + ivar_sm[arm] * var_lss)
             w = weight > 0
 
             cost += np.dot(
                 weight, (flux[arm] - cont_est)**2
             ) - np.log(weight[w]).sum()  # + penalty
 
         return cost
@@ -379,34 +374,29 @@
             return a0 / n0
 
         result = self.minimizer(spec, get_a0())
         spec.cont_params['valid'] = result['valid']
 
         if spec.cont_params['valid']:
             spec.cont_params['cont'] = {}
-            chi2 = 0
             for arm, wave_arm in spec.forestwave.items():
                 cont_est = self.get_continuum_model(
                     result['x'], wave_arm / (1 + spec.z_qso))
 
                 if any(cont_est < 0):
                     spec.cont_params['valid'] = False
                     break
 
                 cont_est *= self.meanflux_interp(wave_arm)
                 # cont_est *= self.flux_stacker(wave_arm)
                 spec.cont_params['cont'][arm] = cont_est
-                var_lss = self.varlss_interp(wave_arm) * cont_est**2
-                weight = 1. / (1 + spec.forestivar_sm[arm] * var_lss)
-                weight *= spec.forestivar_sm[arm]
 
-                chi2 += np.dot(weight, (spec.forestflux[arm] - cont_est)**2)
-
-            # We can further eliminate spectra based chi2
-            spec.cont_params['chi2'] = chi2
+        spec.set_forest_weight(self.varlss_interp, self.eta_interp)
+        # We can further eliminate spectra based chi2
+        spec.calc_continuum_chi2()
 
         if spec.cont_params['valid']:
             spec.cont_params['x'] = result['x']
             spec.cont_params['xcov'] = result['xcov']
         else:
             spec.cont_params['cont'] = None
             spec.cont_params['chi2'] = -1
@@ -508,39 +498,36 @@
         has_converged: bool
             True if all continuum updates on every point are less than 0.33
             times the error estimates.
         """
         norm_flux = np.zeros(self.nbins)
         std_flux = np.empty(self.nbins)
         counts = np.zeros(self.nbins)
-        # self.flux_stacker.reset()
+        self.flux_stacker.reset()
 
         for spec in valid_spectra(spectra_list):
             for arm, wave_arm in spec.forestwave.items():
                 wave_rf_arm = wave_arm / (1 + spec.z_qso)
                 bin_idx = (
                     (wave_rf_arm - self.rfwave[0]) / self.dwrf + 0.5
                 ).astype(int)
 
                 cont = spec.cont_params['cont'][arm]
                 flux = spec.forestflux[arm] / cont
+                weight = spec.forestweight[arm] * cont**2
                 # Deconvolve resolution matrix ?
 
-                var_lss = self.varlss_interp(wave_arm)
-                weight = spec.forestivar_sm[arm] * cont**2
-                weight = weight / (1 + weight * var_lss)
-
                 norm_flux += np.bincount(
                     bin_idx, weights=flux * weight, minlength=self.nbins)
                 counts += np.bincount(
                     bin_idx, weights=weight, minlength=self.nbins)
 
-                # self.flux_stacker.add(wave_arm, flux, weight)
+                self.flux_stacker.add(wave_arm, flux, weight)
 
-        # self.flux_stacker.calculate()
+        self.flux_stacker.calculate()
         self.comm.Allreduce(MPI.IN_PLACE, norm_flux)
         self.comm.Allreduce(MPI.IN_PLACE, counts)
         w = counts > 0
 
         if w.sum() != self.nbins:
             warn_mpi(
                 "Extrapolating empty bins in the mean continuum.",
@@ -559,38 +546,37 @@
         # remove tilt and higher orders and normalize
         new_meancont, mean_ = self._project_normalize_meancont(new_meancont)
 
         norm_flux = new_meancont / self.meancont_interp.fp - 1
         std_flux /= mean_
 
         if not noupdate:
-            self.meancont_interp.fp = new_meancont
-            self.meancont_interp.ep = std_flux
+            self.meancont_interp.reset(new_meancont, ep=std_flux)
 
         all_pt_test = np.all(np.abs(norm_flux) < 0.33 * std_flux)
         chi2_change = np.sum((norm_flux / std_flux)**2) / self.nbins
         has_converged = (chi2_change < 1e-3) | all_pt_test
 
         if self.mpi_rank != 0:
             return has_converged
 
         text = ("Continuum updates\n" "rfwave\t| update\t| error\n")
 
-        sl = np.s_[::max(1, int(self.nbins / 10))]
+        sl = np.s_[::max(1, self.nbins // 10)]
         for w, n, e in zip(self.rfwave[sl], norm_flux[sl], std_flux[sl]):
-            text += f"{w:7.2f}\t| {n:7.2e}\t| pm {e:7.2e}\n"
+            text += f"{w:7.2f}\t| {n:7.2e}\t| +- {e:7.2e}\n"
 
         text += f"Change in chi2: {chi2_change*100:.4e}%"
         logging_mpi(text, 0)
 
         return has_converged
 
-    def update_var_lss(self, spectra_list, noupdate):
-        """ Fit and update var_lss. See :class:`VarLSSFitter` for fitting
-        details.
+    def update_var_lss_eta(self, spectra_list, noupdate):
+        """ Fit and update var_lss and eta if enabled. See
+        :class:`VarLSSFitter` for fitting details.
 
         Arguments
         ---------
         spectra_list: list(Spectrum)
             Spectrum objects to fit.
         noupdate: bool
             Does not update `self.varlss_interp.fp` if True (last iteration).
@@ -605,29 +591,46 @@
                 cont = spec.cont_params['cont'][arm]
                 delta = spec.forestflux[arm] / cont - 1
                 ivar = spec.forestivar[arm] * cont**2
 
                 self.varlss_fitter.add(wave_arm, delta, ivar)
 
         # Else, fit for var_lss
-        logging_mpi("Fitting var_lss", self.mpi_rank)
-        y, ep = self.varlss_fitter.fit(
-            self.varlss_interp.fp)
-        if not noupdate:
-            self.varlss_interp.fp = y
-            self.varlss_interp.ep = ep
+        if self.fit_eta:
+            text = "Fitting var_lss and eta"
+            initial_guess = np.vstack(
+                (self.varlss_interp.fp, self.eta_interp.fp)).T
+        else:
+            text = "Fitting var_lss"
+            initial_guess = self.varlss_interp.fp
+
+        logging_mpi(text, self.mpi_rank)
+        y, ep = self.varlss_fitter.fit(initial_guess)
+
+        if not noupdate and not self.fit_eta:
+            self.varlss_interp.reset(y, ep=ep)
+        if not noupdate and self.fit_eta:
+            self.varlss_interp.reset(y[:, 0], ep=ep[:, 0])
+            self.eta_interp.reset(y[:, 1], ep=ep[:, 1])
 
         if self.mpi_rank != 0:
             return
 
-        sl = np.s_[::max(1, int(y.size / 10))]
+        step = max(1, self.varlss_fitter.nwbins // 10)
         text = ("------------------------------\n"
-                "wave\t| var_lss\t| error\n")
-        for w, v, e in zip(self.varlss_fitter.waveobs[sl], y[sl], ep[sl]):
-            text += f"{w:7.2f}\t| {v:7.2e} \t| {e:7.2e}\n"
+                "wave\t| var_lss +-  error \t|   eta   +-  error \n")
+
+        for i in range(0, self.varlss_fitter.nwbins, step):
+            w = self.varlss_fitter.waveobs[i]
+            v = self.varlss_interp.fp[i]
+            ve = self.varlss_interp.ep[i]
+            n = self.eta_interp.fp[i]
+            ne = self.eta_interp.ep[i]
+            text += \
+                f"{w:7.2f}\t| {v:7.2e} +- {ve:7.2e}\t| {n:7.2e} +- {ne:7.2e}\n"
         text += "------------------------------"
         logging_mpi(text, 0)
 
     def iterate(self, spectra_list):
         """Main function to fit continua and iterate.
 
         Consists of three major steps: initializing, fitting, updating global
@@ -662,67 +665,69 @@
             spec.cont_params['xcov'] = np.eye(self.cont_order + 1)
             spec.cont_params['dof'] = spec.get_real_size()
 
         fname = f"{self.outdir}/attributes.fits" if self.outdir else ""
         fattr = MPISaver(fname, self.mpi_rank)
 
         for it in range(self.niterations):
+            is_last_it = it == self.niterations - 1
             logging_mpi(
                 f"Fitting iteration {it+1}/{self.niterations}", self.mpi_rank)
 
-            self.save(fattr, it + 1)
+            self.save(fattr, f"-{it + 1}")
 
             # Fit all continua one by one
             self.fit_continua(spectra_list)
             # Stack all spectra in each process
             # Broadcast and recalculate global functions
-            has_converged = self.update_mean_cont(
-                spectra_list, it == self.niterations - 1)
+            has_converged = self.update_mean_cont(spectra_list, is_last_it)
 
-            self.update_var_lss(spectra_list, it == self.niterations - 1)
+            self.update_var_lss_eta(spectra_list, is_last_it)
 
             if has_converged:
                 logging_mpi("Iteration has converged.", self.mpi_rank)
                 break
 
         if not has_converged:
             warn_mpi("Iteration has NOT converged.", self.mpi_rank)
 
+        self.save(fattr)
+        self.varlss_fitter.write(fattr)
         fattr.close()
         logging_mpi("All continua are fit.", self.mpi_rank)
 
-        self.save_contchi2_catalog(spectra_list)
-
-    def save(self, fattr, it):
+    def save(self, fattr, suff=''):
         """Save mean continuum and var_lss (if fitting) to a fits file.
 
         Arguments
         ---------
         fattr: MPISaver
             File handler to save only on master node.
-        it: int
-            Current iteration number.
+        suff: str
+            Suffix for the current iteration number.
         """
         fattr.write(
             [self.rfwave, self.meancont_interp.fp, self.meancont_interp.ep],
             names=['lambda_rf', 'mean_cont', 'e_mean_cont'],
-            extname=f'CONT-{it}')
+            extname=f'CONT{suff}')
 
-        # fattr.write(
-        #     [self.flux_stacker.waveobs, self.flux_stacker.stacked_flux],
-        #     names=['lambda', 'stacked_flux'],
-        #     extname=f'STACKED_FLUX-{it}')
+        fattr.write(
+            [self.flux_stacker.waveobs, self.flux_stacker.stacked_flux],
+            names=['lambda', 'stacked_flux'],
+            extname=f'STACKED_FLUX{suff}')
 
         if self.varlss_fitter is None:
             return
 
         fattr.write(
-            [self.varlss_fitter.waveobs, self.varlss_interp.fp,
-             self.varlss_interp.ep],
-            names=['lambda', 'var_lss', 'e_var_lss'], extname=f'VAR_FUNC-{it}')
+            [self.varlss_fitter.waveobs,
+             self.varlss_interp.fp, self.varlss_interp.ep,
+             self.eta_interp.fp, self.eta_interp.ep],
+            names=['lambda', 'var_lss', 'e_var_lss', 'eta', 'e_eta'],
+            extname=f'VAR_FUNC{suff}')
 
     def save_contchi2_catalog(self, spectra_list):
         """Save chi2 catalog if ``self.outdir`` is set. All values are gathered
         and saved on the master node.
 
         Arguments
         ---------
@@ -733,29 +738,35 @@
             return
 
         logging_mpi("Saving continuum chi2 catalog.", self.mpi_rank)
         corder = self.cont_order + 1
 
         dtype = np.dtype([
             ('TARGETID', 'int64'), ('Z', 'f4'), ('HPXPIXEL', 'i8'),
-            ('MPI_RANK', 'i4'), ('MEANSNR', 'f4'), ('RSNR', 'f4'),
+            ('ARMS', 'U5'), ('MEANSNR', 'f4', 3), ('RSNR', 'f4'),
+            ('MPI_RANK', 'i4'),
             ('CONT_valid', bool), ('CONT_chi2', 'f4'), ('CONT_dof', 'i4'),
             ('CONT_x', 'f4', corder),
             ('CONT_xcov', 'f4', corder**2)
         ])
         local_catalog = np.empty(len(spectra_list), dtype=dtype)
 
         for i, spec in enumerate(spectra_list):
+            mean_snrs = np.zeros(3)
+            _x = list(spec.mean_snr.values())
+            mean_snrs[:len(_x)] = _x
+
             row = local_catalog[i]
             row['TARGETID'] = spec.targetid
             row['Z'] = spec.z_qso
             row['HPXPIXEL'] = spec.catrow['HPXPIXEL']
-            row['MPI_RANK'] = self.mpi_rank
-            row['MEANSNR'] = spec.mean_snr()
+            row['ARMS'] = ",".join(spec.mean_snr.keys())
+            row['MEANSNR'] = mean_snrs
             row['RSNR'] = spec.rsnr
+            row['MPI_RANK'] = self.mpi_rank
             for lbl in ['valid', 'x', 'chi2', 'dof']:
                 row[f'CONT_{lbl}'] = spec.cont_params[lbl]
             row['CONT_xcov'] = spec.cont_params['xcov'].ravel()
 
         all_catalogs = self.comm.gather(local_catalog)
         if self.mpi_rank == 0:
             all_catalog = np.concatenate(all_catalogs)
@@ -814,30 +825,28 @@
         120 A wavelength spacing.
     var1: float, default: 1e-4
         Lower variance edge.
     var2: float, default: 20
         Upper variance edge.
     nvarbins: int, default: 100
         Number of variance bins.
-    nsubsamples: int, default: 100
-        Number of subsamples for the Jackknife covariance.
-    error_method: str, default: regJack
-        Error estimation methods for var_delta. Must be one of
-        :attr:`accepted_vardelta_error_methods`.
+    nsubsamples: int, default: None
+        Number of subsamples for the Jackknife covariance. Auto determined by
+        number of bins (``nvarbins^2``) if None.
+    use_cov: bool, default: False
+        Use the Jackknife covariance when fitting.
     comm: MPI.COMM_WORLD or None, default: None
         MPI comm object to allreduce if enabled.
 
     Attributes
     ----------
     waveobs: :external+numpy:py:class:`ndarray <numpy.ndarray>`
         Wavelength centers in the observed frame.
     ivar_edges: :external+numpy:py:class:`ndarray <numpy.ndarray>`
         Inverse variance edges.
-    var_centers: :external+numpy:py:class:`ndarray <numpy.ndarray>`
-        Variance centers in **descending** order.
     minlength: int
         Minimum size of the combined bin count array. It includes underflow and
         overflow bins for both wavelength and variance bins.
     wvalid_bins: :external+numpy:py:class:`ndarray <numpy.ndarray>`
         Bool array slicer to get non-overflow bins of 1D arrays.
     subsampler: SubsampleCov
         Subsampler object that stores mean_delta in axis=0, var_delta in axis=1
@@ -847,25 +856,23 @@
     mpi_rank: int
         Rank of the MPI process if ``comm!=None``. Zero otherwise.
     """
     min_no_pix = 500
     """int: Minimum number of pixels a bin must have to be valid."""
     min_no_qso = 50
     """int: Minimum number of quasars a bin must have to be valid."""
-    accepted_vardelta_error_methods = ["gauss", "regJack"]
-    """list(str): Accepted error estimation methods for var_delta."""
 
     @staticmethod
     def variance_function(var_pipe, var_lss, eta=1):
         """Variance model to be fit.
 
         .. math::
 
-            \sigma^2_\mathrm{obs} = \eta \sigma^2_\mathrm{pipe} +
-            \sigma^2_\mathrm{LSS}
+            \\sigma^2_\\mathrm{obs} = \\eta \\sigma^2_\\mathrm{pipe} +
+            \\sigma^2_\\mathrm{LSS}
 
         Arguments
         ---------
         var_pipe: :external+numpy:py:class:`ndarray <numpy.ndarray>`
             Pipeline variance.
         var_lss: :external+numpy:py:class:`ndarray <numpy.ndarray>`
             Large-scale structure variance.
@@ -878,27 +885,22 @@
             Expected variance of deltas.
         """
         return eta * var_pipe + var_lss
 
     def __init__(
             self, w1obs, w2obs, nwbins=None,
             var1=1e-4, var2=20., nvarbins=100,
-            nsubsamples=100, error_method="regJack",
-            comm=None
+            nsubsamples=None, use_cov=False, comm=None
     ):
-        assert set(
-            VarLSSFitter.accepted_vardelta_error_methods
-        ).intersection([error_method])
-
         if nwbins is None:
             nwbins = int(round((w2obs - w1obs) / 120.))
 
         self.nwbins = nwbins
         self.nvarbins = nvarbins
-        self.error_method = error_method
+        self.use_cov = use_cov
         self.comm = comm
 
         # Set up wavelength and inverse variance bins
         wave_edges, self.dwobs = np.linspace(
             w1obs, w2obs, nwbins + 1, retstep=True)
         self.waveobs = (wave_edges[1:] + wave_edges[:-1]) / 2
         self.ivar_edges = np.logspace(
@@ -917,27 +919,32 @@
         self._num_pixels = np.zeros(self.minlength, dtype=int)
         self._num_qso = np.zeros(self.minlength, dtype=int)
 
         # If ran with MPI, save mpi_rank first
         # Then shift each container to remove possibly over adding to 0th bin.
         if comm is not None:
             self.mpi_rank = comm.Get_rank()
+            mpi_size = comm.Get_size()
         else:
             self.mpi_rank = 0
+            mpi_size = 1
 
+        if nsubsamples is None:
+            nsubsamples = self.nvarbins**2
+        istart = (self.mpi_rank * nsubsamples) // mpi_size
         # Axis 0 is mean
         # Axis 1 is var_delta
         # Axis 2 is var2_delta
         # Axis 3 is var_centers
         self.subsampler = SubsampleCov(
-            (4, self.minlength), nsubsamples, self.mpi_rank)
+            (4, self.minlength), nsubsamples, istart)
 
     def reset(self):
         """Reset delta and num arrays to zero."""
-        self.subsampler.reset(self.mpi_rank)
+        self.subsampler.reset()
         self._num_pixels *= 0
         self._num_qso *= 0
 
     def add(self, wave, delta, ivar):
         """Add statistics of a single spectrum. Updates delta and num arrays.
 
         Assumes no spectra has ``wave < w1obs`` or ``wave > w2obs``.
@@ -969,34 +976,65 @@
         ])
         self.subsampler.add_measurement(xvec, npix)
 
         npix[npix > 0] = 1
         self._num_qso += npix
 
     def _allreduce(self):
-        """Sums statistics from all MPI process, and calculates mean, variance
-        and error on the variance.
+        """ Sums statistics from all MPI process in place."""
+        if self.comm is None:
+            return
 
-        It also calculates the delete-one Jackknife variance of var_delta over
-        ``nsubsamples``.
-        """
-        if self.comm is not None:
-            self.subsampler.allreduce(self.comm, MPI.IN_PLACE)
+        self.subsampler.allreduce(self.comm, MPI.IN_PLACE)
+
+        self.comm.Allreduce(MPI.IN_PLACE, self._num_pixels)
+        self.comm.Allreduce(MPI.IN_PLACE, self._num_qso)
 
-            self.comm.Allreduce(MPI.IN_PLACE, self._num_pixels)
-            self.comm.Allreduce(MPI.IN_PLACE, self._num_qso)
+    def _calc_subsampler_stats(self):
+        """ Calculates mean, variance and error on the variance.
 
+        It also calculates the delete-one Jackknife variance over
+        ``nsubsamples``.
+        The variance on var_delta is updated with the variance on the mean
+        estimates, then it is regularized by calculated var2_delta
+        (Gaussian estimates), where if Jackknife variance is smaller than
+        the Gaussian estimate, it is replaced by the Gaussian estimate.
+
+        Covariance is calculated if :attr:`use_cov` is set to True in init.
+        Covariance of mean_delta^2 is propagated using the formula in
+        :func:`qsonic.mathtools.block_covariance_of_square`.
+        """
         self.subsampler.get_mean_n_var()
+        if self.use_cov:
+            self.subsampler.get_mean_n_cov(
+                indices=[0, 1], blockdim=self.nvarbins + 2)
 
-        self.subsampler.mean[1] -= self.subsampler.mean[0]**2
+        m2 = self.subsampler.mean[0]**2
+        self.subsampler.mean[1] -= m2
         self.subsampler.mean[2] -= self.subsampler.mean[1]**2
 
         w = self._num_pixels > 0
         self.subsampler.mean[2, w] /= self._num_pixels[w]
 
+        # Update variance / covariance
+        if self.use_cov:
+            self.subsampler.covariance[1] += block_covariance_of_square(
+                self.subsampler.mean[0],
+                self.subsampler.variance[0],
+                self.subsampler.covariance[0])
+        else:
+            self.subsampler.variance[1] += 4 * m2 * self.subsampler.variance[0]
+            self.subsampler.variance[1] += 2 * self.subsampler.variance[0]**2
+            # Regularized jackknife errors
+            self.subsampler.variance[1] = np.where(
+                self.subsampler.variance[1] > self.subsampler.mean[2],
+                self.subsampler.variance[1],
+                self.subsampler.mean[2]
+            )
+
     def _smooth_fit_results(self, fit_results, std_results):
         w = fit_results > 0
 
         # Smooth new estimates
         if fit_results.ndim == 1:
             spl = UnivariateSpline(
                 self.waveobs[w], fit_results[w], w=1 / std_results[w])
@@ -1011,91 +1049,40 @@
                 self.waveobs[w], fit_results[w, 1], w=1 / std_results[w, 1])
 
             fit_results[:, 0] = spl1(self.waveobs)
             fit_results[:, 1] = spl2(self.waveobs)
 
         return fit_results
 
-    def get_var_delta_error(self, method=None):
-        """ Calculate the error (sigma) on var_delta using a given method.
-
-        - ``method="gauss"``:
-            Observed var2_delta using delta**4 statistics are used as has been
-            done before.
-
-        - ``method="regJack"``:
-            The variance on var_delta is first calculated by delete-one
-            Jackknife
-            over ``nsubsamples``. This is regularized by calculated var2_delta
-            (Gaussian estimates), where if Jackknife variance is smaller than
-            the Gaussian estimate, it is replaced by the Gaussian estimate.
-
-        Arguments
-        ---------
-        method: str, default: None
-            Method to estimate error on var_delta
-
-        Returns
-        ---------
-        error_estimates: :external+numpy:py:class:`ndarray <numpy.ndarray>`
-            Error (sigma) on var_delta
-
-        Raises
-        ------
-        ValueError
-            If method is not one of :attr:`accepted_vardelta_error_methods`.
-        """
-        if method is None:
-            method = self.error_method
-
-        if method == "gauss":
-            error_estimates = np.sqrt(self.subsampler.mean[2])
-
-        elif method == "regJack":
-            # Regularized jackknife errors
-            error_estimates = np.where(
-                self.subsampler.variance[1] > self.subsampler.mean[2],
-                self.subsampler.variance[1],
-                self.subsampler.mean[2]
-            )
-
-            error_estimates = np.sqrt(error_estimates)
-        else:
-            raise ValueError(f"Unkown error method {method}.")
-
-        return error_estimates[self.wvalid_bins]
-
     def _fit_array_shape_assert(self, arr):
         assert (arr.ndim == 1 or arr.ndim == 2)
         assert (arr.shape[0] == self.nwbins)
         if arr.ndim == 2:
             assert (arr.shape[1] == 2)
 
-    def fit(self, initial_guess, method=None, smooth=True):
+    def fit(self, initial_guess, smooth=True):
         """ Syncronize all MPI processes and fit for ``var_lss`` and ``eta``.
 
         Second axis always contains ``eta`` values. Example::
 
             var_lss = initial_guess[:, 0]
             eta = initial_guess[:, 1]
 
         This implemented using :func:`scipy.optimize.curve_fit` with
-        ``sqrt(var2_delta_subs)`` as absolute errors. Domain is bounded to
-        ``(0, 2)``. These fits are then smoothed via
+        :attr:`e_var_delta` or :attr:`cov_var_delta` as absolute errors. Domain
+        is bounded to ``(0, 2)``. These fits are then smoothed via
         :external+scipy:py:class:`scipy.interpolate.UnivariateSpline`
         using weights from ``curve_fit``,
         while missing values or failed wavelength bins are extrapolated.
 
         Arguments
         ---------
         initial_guess: :external+numpy:py:class:`ndarray <numpy.ndarray>`
             Initial guess for var_lss and eta. If 1D array, eta is fixed to
             one. If 2D, its shape must be ``(nwbins, 2)``.
-        method: str, default: None
-            Error estimation method
         smooth: bool, default: True
             Smooth results using UnivariateSpline.
 
         Returns
         ---------
         fit_results: :external+numpy:py:class:`ndarray <numpy.ndarray>`
             Smoothed fit results at observed wavelengths where missing values
@@ -1104,44 +1091,54 @@
             axis if ``initial_guess`` is 2D ndarray.
         std_results: :external+numpy:py:class:`ndarray <numpy.ndarray>`
             Error on ``var_lss`` from sqrt of ``curve_fit`` output. Same
             behavior as ``fit_results``.
         """
         self._fit_array_shape_assert(initial_guess)
         self._allreduce()
+        self._calc_subsampler_stats()
 
         nfails = 0
         fit_results = np.zeros_like(initial_guess)
         std_results = np.zeros_like(initial_guess)
 
-        error_estimates = self.get_var_delta_error(method)
         w_gtr_min = ((self.num_pixels > VarLSSFitter.min_no_pix)
                      & (self.num_qso > VarLSSFitter.min_no_qso))
 
+        if self.use_cov:
+            err_base = self.cov_var_delta
+        else:
+            err_base = self.e_var_delta
+
         for iwave in range(self.nwbins):
             i1 = iwave * self.nvarbins
             i2 = i1 + self.nvarbins
             wave_slice = np.s_[i1:i2]
             w = w_gtr_min[wave_slice]
 
             if w.sum() == 0:
                 nfails += 1
                 warn_mpi(
                     "Not enough statistics for VarLSSFitter at"
                     f" wave_obs: {self.waveobs[iwave]:.2f}.",
                     self.mpi_rank)
                 continue
 
+            if self.use_cov:
+                err2use = err_base[iwave][:, w][w, :]
+            else:
+                err2use = err_base[wave_slice][w]
+
             try:
                 pfit, pcov = curve_fit(
                     VarLSSFitter.variance_function,
                     self.var_centers[wave_slice][w],
                     self.var_delta[wave_slice][w],
                     p0=initial_guess[iwave],
-                    sigma=error_estimates[wave_slice][w],
+                    sigma=err2use,
                     absolute_sigma=True,
                     check_finite=True,
                     bounds=(0, 2)
                 )
             except Exception as e:
                 nfails += 1
                 warn_mpi(
@@ -1149,44 +1146,42 @@
                     f"{self.waveobs[iwave]:.2f}. "
                     f"Reason: {e}. Extrapolating.",
                     self.mpi_rank)
             else:
                 fit_results[iwave] = pfit
                 std_results[iwave] = np.sqrt(np.diag(pcov))
 
-        # Smooth new estimates
-        if smooth:
-            fit_results = self._smooth_fit_results(fit_results, std_results)
+        invalid_ratio = nfails / fit_results.shape[0]
+        if invalid_ratio > 0.4:
+            raise QsonicException(
+                "VarLSSFitter failed at more than 40% points.")
 
         if nfails > 0:
             warn_mpi(
                 f"VarLSSFitter failed and extrapolated at {nfails} points.",
                 self.mpi_rank)
 
+        # Smooth new estimates
+        if smooth:
+            fit_results = self._smooth_fit_results(fit_results, std_results)
+
         return fit_results, std_results
 
-    def save(self, fname, min_snr=0, max_snr=100):
-        """Save variance statistics to FITS file.
+    def write(self, mpi_saver, min_snr=0, max_snr=100):
+        """ Write variance statistics to FITS file in 'VAR_STATS' extention.
 
         Arguments
         ---------
-        fname: str
-            Filename to be written. It is always overwritten.
+        mpi_saver: MPISaver
+            MPI FITS file handler.
         min_snr: float, default: 0
             Minimum SNR in this sample to be written into header.
         max_snr: float, default: 100
-            Maximum SNR in this sampleto be written into header.
-
-        Returns
-        -------
-        mpi_saver: MPISaver
-            To save additional data or to close manually.
+            Maximum SNR in this sample to be written into header.
         """
-        mpi_saver = MPISaver(fname, self.mpi_rank)
-
         hdr_dict = {
             'MINNPIX': VarLSSFitter.min_no_pix,
             'MINNQSO': VarLSSFitter.min_no_qso,
             'MINSNR': min_snr,
             'MAXSNR': max_snr,
             'WAVE1': self.waveobs[0],
             'WAVE2': self.waveobs[-1],
@@ -1195,25 +1190,29 @@
             'IVAR2': self.ivar_edges[-1],
             'NVARBINS': self.nvarbins
         }
 
         data_to_write = [
             np.repeat(self.waveobs, self.nvarbins),
             self.var_centers, self.e_var_centers,
-            self.mean_delta, self.var_delta,
-            self.subsampler.variance[1][self.wvalid_bins], self.var2_delta,
-            self.num_pixels, self.num_qso]
-        names = ['wave', 'var_pipe', 'e_var_pipe', 'mean_delta', 'var_delta',
-                 'varjack_delta', 'var2_delta', 'num_pixels', 'num_qso']
+            self.var_delta, self.e_var_delta,
+            self.mean_delta, self.var2_delta, self.num_pixels, self.num_qso]
+
+        names = ['wave', 'var_pipe', 'e_var_pipe', 'var_delta', 'e_var_delta',
+                 'mean_delta', 'var2_delta', 'num_pixels', 'num_qso']
+
+        if self.use_cov:
+            cov_data = self.cov_var_delta.reshape(
+                self.nwbins * self.nvarbins, self.nvarbins)
+            data_to_write.append(cov_data)
+            names.append("cov_var_delta")
 
         mpi_saver.write(
             data_to_write, names=names, extname="VAR_STATS", header=hdr_dict)
 
-        return mpi_saver
-
     @property
     def num_pixels(self):
         """:external+numpy:py:class:`ndarray <numpy.ndarray>`:
         Number of pixels in bins."""
         return self._num_pixels[self.wvalid_bins]
 
     @property
@@ -1230,23 +1229,45 @@
     @property
     def var_delta(self):
         """:external+numpy:py:class:`ndarray <numpy.ndarray>`:
         Variance delta."""
         return self.subsampler.mean[1][self.wvalid_bins]
 
     @property
+    def e_var_delta(self):
+        """:external+numpy:py:class:`ndarray <numpy.ndarray>`:
+        Error on variance delta using delete-one Jackknife. The error of
+        :attr:`mean_delta` is propagated, then regularized using
+        :attr:`var2_delta`. See source code of :meth:`_calc_subsampler_stats`.
+        """
+        return np.sqrt(self.subsampler.variance[1][self.wvalid_bins])
+
+    @property
+    def cov_var_delta(self):
+        """:external+numpy:py:class:`ndarray <numpy.ndarray>`:
+        3D array of shape ``(nwbins, nvarbins, nvarbins)`` for the covariance
+        on variance delta using delete-one Jackknife. The covariance
+        of :attr:`mean_delta` is propagated. See
+        :func:`qsonic.mathtools.block_covariance_of_square` for details.
+        None if :attr:`use_cov` is False."""
+        if not self.use_cov:
+            return None
+        cov = self.subsampler.covariance[1]
+        return cov[1:-1, 1:-1, 1:-1]
+
+    @property
     def var2_delta(self):
         """:external+numpy:py:class:`ndarray <numpy.ndarray>`:
         Variance delta^2."""
         return self.subsampler.mean[2][self.wvalid_bins]
 
     @property
     def var_centers(self):
         """:external+numpy:py:class:`ndarray <numpy.ndarray>`:
-        Mean variance for the bin centers."""
+        Mean variance for the bin centers in **descending** order."""
         return self.subsampler.mean[3][self.wvalid_bins]
 
     @property
     def e_var_centers(self):
         """:external+numpy:py:class:`ndarray <numpy.ndarray>`:
         Error on the mean variance for the bin centers."""
         return np.sqrt(self.subsampler.variance[3][self.wvalid_bins])
@@ -1274,30 +1295,30 @@
     ----------
     waveobs: :external+numpy:py:class:`ndarray <numpy.ndarray>`
         Wavelength centers in the observed frame.
     nwbins: int
         Number of wavelength bins
     dwobs: float
         Wavelength spacing. Usually same as observed grid.
-    _interp: Fast1DInterpolator
+    _interp: FastLinear1DInterp
         Interpolator. Saves stacked_flux in fp and weights in ep.
     comm: MPI.COMM_WORLD or None, default: None
         MPI comm object to allreduce if enabled.
     """
 
     def __init__(self, w1obs, w2obs, dwobs, comm=None):
         # Set up wavelength and inverse variance bins
-        self.nwbins = int((w2obs - w1obs) / dwobs)
+        self.nwbins = int(round((w2obs - w1obs) / dwobs))
         wave_edges, self.dwobs = np.linspace(
             w1obs, w2obs, self.nwbins + 1, retstep=True)
         self.waveobs = (wave_edges[1:] + wave_edges[:-1]) / 2
 
         self.comm = comm
 
-        self._interp = Fast1DInterpolator(
+        self._interp = FastLinear1DInterp(
             self.waveobs[0], self.dwobs,
             np.ones(self.nwbins), ep=np.zeros(self.nwbins))
 
     def __call__(self, wave):
         return self._interp(wave)
 
     def add(self, wave, flux, weight):
```

### Comparing `qsonic-0.5.2/py/qsonic/scripts/qsonic_calib.py` & `qsonic-0.6.0/py/qsonic/scripts/qsonic_calib.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import numpy as np
 
 from qsonic import QsonicException
 import qsonic.catalog
 import qsonic.io
 from qsonic.masks import BALMask
-from qsonic.mpi_utils import logging_mpi, mpi_parse, mpi_fnc_bcast
+from qsonic.mpi_utils import logging_mpi, mpi_parse, mpi_fnc_bcast, MPISaver
 from qsonic.picca_continuum import VarLSSFitter
 from qsonic.spectrum import add_wave_region_parser
 
 
 def get_parser(add_help=True):
     """Constructs the parser needed for the script.
 
@@ -57,27 +57,32 @@
     iogroup.add_argument(
         "--remove-targetid-list",
         help="Text file with TARGETIDs to exclude from analysis.")
 
     vargroup = parser.add_argument_group(
         'Variance fitting parameters')
     vargroup.add_argument(
-        "--nvarbins", help="Number of variance bins (logarithmically spaced)",
+        "--nvarbins", help="Number of variance bins (logarithmically spaced).",
         default=100, type=int)
     vargroup.add_argument(
+        "--var-use-cov", action="store_true",
+        help="Use covariance in varlss-eta fitting.")
+    vargroup.add_argument(
         "--nwbins", default=None, type=int,
         help="Number of wavelength bins. None creates bins with 120 A spacing")
     vargroup.add_argument(
-        "--var1", help="Lower variance bin", default=1e-5, type=float)
+        "--var1", help="Lower variance bin.", default=1e-4, type=float)
     vargroup.add_argument(
-        "--var2", help="Upper variance bin", default=2., type=float)
+        "--var2", help="Upper variance bin.", default=20., type=float)
     vargroup.add_argument(
-        "--min-snr", help="Minimum SNR of the forest", default=0, type=float)
+        "--min-snr", help="Minimum SNR of the forest.",
+        default=0, type=float)
     vargroup.add_argument(
-        "--max-snr", help="Maximum SNR of the forest", default=100, type=float)
+        "--max-snr", help="Maximum SNR of the forest.",
+        default=100, type=float)
 
     parser = add_wave_region_parser(parser)
 
     return parser
 
 
 def mpi_set_targetid_list_to_remove(args, comm=None, mpi_rank=0):
@@ -203,15 +208,15 @@
     args = mpi_parse(get_parser(), comm, mpi_rank)
     if mpi_rank == 0:
         os_makedirs(args.outdir, exist_ok=True)
 
     varfitter = VarLSSFitter(
         args.wave1, args.wave2, args.nwbins,
         args.var1, args.var2, args.nvarbins,
-        nsubsamples=100, comm=comm)
+        use_cov=args.var_use_cov, comm=comm)
 
     ids_to_remove = mpi_set_targetid_list_to_remove(args, comm, mpi_rank)
 
     def _is_kept(delta):
         return (
             (delta.targetid not in ids_to_remove)
             and (delta.mean_snr > args.min_snr)
@@ -230,29 +235,30 @@
     fit_results[:, 0] = 0.1
     fit_results, std_results = varfitter.fit(fit_results)
 
     # Save variance stats to file
     logging_mpi("Saving variance stats to files", mpi_rank)
     suffix = f"snr{args.min_snr:.1f}-{args.max_snr:.1f}"
     tmpfilename = f"{args.outdir}/{args.fbase}-{suffix}-variance-stats.fits"
-    mpi_saver = varfitter.save(tmpfilename)
+    mpi_saver = MPISaver(tmpfilename, mpi_rank)
+    varfitter.write(mpi_saver, args.min_snr, args.max_snr)
     logging_mpi(f"Variance stats saved in {tmpfilename}.", mpi_rank)
 
     # Save fits results as well
     mpi_saver.write([
-        varfitter.waveobs, fit_results[:, 0], fit_results[:, 1],
-        std_results[:, 0], std_results[:, 1]],
-        names=["wave", "var_lss", "eta", "e_var_lss", "e_eta"],
+        varfitter.waveobs, fit_results[:, 0], std_results[:, 0],
+        fit_results[:, 1], std_results[:, 1]],
+        names=['lambda', 'var_lss', 'e_var_lss', 'eta', 'e_eta'],
         extname="VAR_FUNC"
     )
 
     waveobs, stacked_flux = mpi_stack_fluxes(args, comm, deltas_list)
     mpi_saver.write(
         [waveobs, stacked_flux],
-        names=["wave", "stacked_flux"],
+        names=["lambda", "stacked_flux"],
         extname="STACKED_FLUX")
 
     mpi_saver.close()
 
 
 def main():
     from mpi4py import MPI
```

### Comparing `qsonic-0.5.2/py/qsonic/scripts/qsonic_fit.py` & `qsonic-0.6.0/py/qsonic/scripts/qsonic_fit.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import time
 
 from os import makedirs as os_makedirs
 
 import numpy as np
 
 from qsonic import QsonicException
+import qsonic.calibration
 import qsonic.catalog
 import qsonic.io
 import qsonic.spectrum
 import qsonic.masks
 from qsonic.mpi_utils import logging_mpi, mpi_parse
 from qsonic.picca_continuum import (
     PiccaContinuumFitter, add_picca_continuum_parser)
@@ -29,14 +30,15 @@
     parser: argparse.ArgumentParser
     """
     parser = argparse.ArgumentParser(
         add_help=add_help,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 
     parser = qsonic.io.add_io_parser(parser)
+    parser = qsonic.calibration.add_calibration_parser(parser)
 
     analysis_group = parser.add_argument_group('Analysis options')
     analysis_group.add_argument(
         "--smoothing-scale", default=16., type=float,
         help="Smoothing scale for pipeline noise in A.")
     analysis_group.add_argument(
         "--min-rsnr", type=float, default=0.,
@@ -75,41 +77,67 @@
     ---------
     spectra_list: list(Spectrum)
         Spectrum objects for the local MPI rank.
     """
     start_time = time.time()
     logging_mpi("Reading spectra.", mpi_rank)
 
+    # skip_resomat = args.skip_resomat or not args.mock_analysis
+    skip_resomat = args.skip_resomat
+
     spectra_list = []
     # Each process reads its own list
     for cat in local_queue:
         local_specs = qsonic.io.read_spectra_onehealpix(
-            cat, args.input_dir, args.arms,
-            args.mock_analysis, args.skip_resomat
-        )
+            cat, args.input_dir, args.arms, args.mock_analysis, skip_resomat)
+
         for spec in local_specs:
             spec.set_forest_region(
-                args.wave1, args.wave2,
-                args.forest_w1, args.forest_w2
-            )
+                args.wave1, args.wave2, args.forest_w1, args.forest_w2)
 
             if not args.keep_nonforest_pixels:
                 spec.remove_nonforest_pixels()
 
         spectra_list.extend(
             [spec for spec in local_specs if spec.rsnr > args.min_rsnr])
 
+        # if args.skip_resomat:
+        #     continue
+
+        # w = np.array(
+        #     [spec.rsnr > args.min_rsnr for spec in local_specs], dtype=bool)
+        # nspec = w.sum()
+
+        # # Read resolution matrix hopefully faster
+        # spectra_list[-nspec:] = \
+        #     qsonic.io.read_resolution_matrices_onehealpix_data(
+        #         cat[w], args.input_dir, spectra_list[-nspec:])
+
     nspec_all = comm.reduce(len(spectra_list))
     etime = (time.time() - start_time) / 60  # min
     logging_mpi(
         f"All {nspec_all} spectra are read in {etime:.1f} mins.", mpi_rank)
 
     return spectra_list
 
 
+def mpi_noise_flux_calibrate(spectra_list, args, comm, mpi_rank):
+    if args.noise_calibration:
+        logging_mpi("Applying noise calibration.", mpi_rank)
+        ncal = qsonic.calibration.NoiseCalibrator(
+            args.noise_calibration, comm, mpi_rank)
+        ncal.apply(spectra_list)
+
+    if args.flux_calibration:
+        logging_mpi("Applying flux calibration.", mpi_rank)
+        fcal = qsonic.calibration.FluxCalibrator(
+            args.flux_calibration, comm, mpi_rank)
+        fcal.apply(spectra_list)
+
+
 def mpi_read_masks(local_queue, args, comm, mpi_rank):
     """ Read and set masking objects. Broadcast from the master process if
     necessary. See :mod:`qsonic.masks` for
     :class:`SkyMask <qsonic.masks.SkyMask>`,
     :class:`BALMask <qsonic.masks.BALMask>` and
     :class:`DLAMask <qsonic.masks.DLAMask>`.
 
@@ -227,14 +255,16 @@
 
     # Read masks before data
     maskers = mpi_read_masks(local_queue, args, comm, mpi_rank)
 
     spectra_list = mpi_read_spectra_local_queue(
         local_queue, args, comm, mpi_rank)
 
+    mpi_noise_flux_calibrate(spectra_list, args, comm, mpi_rank)
+
     apply_masks(maskers, spectra_list, mpi_rank)
 
     # remove from sample if no pixels is small
     spectra_list = remove_short_spectra(
         spectra_list, args.forest_w1, args.forest_w2, args.skip, mpi_rank)
 
     # Create smoothed ivar as intermediate variable
@@ -252,33 +282,36 @@
 
     # Fit continua
     # Stack all spectra in each process
     # Broadcast and recalculate global functions
     # Iterate
     qcfit.iterate(spectra_list)
 
-    # Keep only valid spectra
-    spectra_list = list(qsonic.spectrum.valid_spectra(spectra_list))
     if args.coadd_arms:
         logging_mpi("Coadding arms.", mpi_rank)
-        for spec in spectra_list:
-            spec.coadd_arms_forest(qcfit.varlss_interp)
+        for spec in qsonic.spectrum.valid_spectra(spectra_list):
+            spec.coadd_arms_forest(qcfit.varlss_interp, qcfit.eta_interp)
+
+    qcfit.save_contchi2_catalog(spectra_list)
+
+    # Keep only valid spectra
+    spectra_list = list(qsonic.spectrum.valid_spectra(spectra_list))
 
     # Final cleaning. Especially important if not coadding arms.
     for spec in spectra_list:
         spec.drop_short_arms(args.forest_w1, args.forest_w2, args.skip)
 
     etime = (time.time() - start_time) / 60  # min
     logging_mpi(f"Continuum fitting and tweaking took {etime:.1f} mins.",
                 mpi_rank)
 
     # Save deltas
     logging_mpi("Saving deltas.", mpi_rank)
     qsonic.io.save_deltas(
-        spectra_list, args.outdir, qcfit.varlss_interp,
+        spectra_list, args.outdir,
         save_by_hpx=args.save_by_hpx, mpi_rank=mpi_rank)
 
 
 def main():
     start_time = time.time()
 
     from mpi4py import MPI
```

### Comparing `qsonic-0.5.2/py/qsonic/spectrum.py` & `qsonic-0.6.0/py/qsonic/spectrum.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 
 import numpy as np
 
 from qsonic import QsonicException
-from qsonic.mathtools import get_smooth_ivar
+from qsonic.mathtools import _zero_function, _one_function, get_smooth_ivar
 
 
 def add_wave_region_parser(parser=None):
     """ Adds wavelength analysis related arguments to parser. These
     arguments are grouped under 'Wavelength analysis region'. All of them
     come with defaults, none are required.
 
@@ -79,20 +79,21 @@
         Index to access in flux, ivar, mask and reso that corresponds to the
         quasar in `catrow`.
 
     Attributes
     ----------
     rsnr: float
         Average SNR above Lya. Calculated in set_forest_region.
+    mean_snr: dict(float)
+        Mean signal-to-noise ratio in the forest.
     _f1, _f2: dict(int)
         Forest indices. Set up using `set_forest_region` method. Then use
         property functions to access forest wave, flux, ivar instead.
     cont_params: dict
         Continuum parameters. Initial estimates are constructed.
-
     """
     WAVE_LYA_A = 1215.67
     """float: Lya wavelength in A."""
     _wave = None
     """dict(:external+numpy:py:class:`ndarray <numpy.ndarray>`): Common
     wavelength grid for **all** Spectra."""
     _dwave = None
@@ -163,22 +164,26 @@
         self.catrow = catrow
         Spectrum._set_wave(wave)
 
         self.flux = {}
         self.ivar = {}
         self.reso = {}
 
-        self.rsnr = 0
+        self.rsnr = None
+        self.mean_snr = None
         self._f1 = {}
         self._f2 = {}
         self._forestwave = {}
         self._forestflux = {}
         self._forestivar = {}
         self._forestivar_sm = {}
         self._forestreso = {}
+        self._forestweight = {}
+
+        self._smoothing_scale = 0
 
         for arm, wave_arm in self.wave.items():
             self._f1[arm], self._f2[arm] = 0, wave_arm.size
             self.flux[arm] = flux[arm][idx]
             self.ivar[arm] = ivar[arm][idx]
             w = (mask[arm][idx] != 0) | np.isnan(self.flux[arm])\
                 | np.isnan(self.ivar[arm])
@@ -197,39 +202,70 @@
         self.cont_params['valid'] = False
         self.cont_params['x'] = np.array([1., 0.])
         self.cont_params['xcov'] = np.eye(2)
         self.cont_params['chi2'] = -1.
         self.cont_params['dof'] = 0
         self.cont_params['cont'] = {}
 
+        self._set_rsnr()
+
+    def _set_rsnr(self):
+        """Calculates and sets SNR above Lya."""
+        self.rsnr = 0
+        rsnr_weight = 1e-6
+
+        for arm, wave_arm in self.wave.items():
+            # Calculate SNR above Lya
+            ii1 = np.searchsorted(
+                wave_arm, (1 + self.z_qso) * Spectrum.WAVE_LYA_A)
+            weight = np.sqrt(self.ivar[arm][ii1:])
+            self.rsnr += np.dot(self.flux[arm][ii1:], weight)
+            rsnr_weight += np.sum(weight > 0)
+
+        self.rsnr /= rsnr_weight
+
+    def _set_forest_related_parameters(self):
+        """Calculates the mean SNR in the forest region and an initial guess
+        for the continuum amplitude."""
+        self.cont_params['x'][0] = 0
+        cont_params_weight = 1e-6
+
+        self.mean_snr = {}
+
+        for arm, ivar_arm in self.forestivar.items():
+            flux_arm = self.forestflux[arm]
+            w = flux_arm > 0
+
+            self.cont_params['x'][0] += np.dot(flux_arm[w], ivar_arm[w])
+            cont_params_weight += np.sum(ivar_arm[w])
+
+            self.mean_snr[arm] = 0
+            armpix = np.sum(ivar_arm > 0)
+            if armpix == 0:
+                continue
+
+            self.mean_snr[arm] = np.dot(np.sqrt(ivar_arm), flux_arm) / armpix
+
+        self.cont_params['x'][0] /= cont_params_weight
+
     def set_forest_region(self, w1, w2, lya1, lya2):
-        """ Sets slices for the forest region. Also calculates
-        average SNR above Lya
+        """ Sets slices for the forest region. Also calculates the mean SNR in
+        the forest and an initial guess for the continuum amplitude.
 
         Arguments
         ---------
         w1, w2: float
             Observed wavelength range
         lya1, lya2: float
             Rest-frame wavelength for the forest
         """
         l1 = max(w1, (1 + self.z_qso) * lya1)
         l2 = min(w2, (1 + self.z_qso) * lya2)
-        rsnr_weight = 1e-6
 
-        a0 = 1e-6
-        n0 = 1e-6
         for arm, wave_arm in self.wave.items():
-            # Calculate SNR above Lya
-            ii1 = np.searchsorted(
-                wave_arm, (1 + self.z_qso) * Spectrum.WAVE_LYA_A)
-            weight = np.sqrt(self.ivar[arm][ii1:])
-            self.rsnr += np.dot(self.flux[arm][ii1:], weight)
-            rsnr_weight += np.sum(weight > 0)
-
             # Slice to forest limits
             ii1, ii2 = np.searchsorted(wave_arm, [l1, l2])
             real_size_arm = np.sum(self.ivar[arm][ii1:ii2] > 0)
             if real_size_arm == 0:
                 continue
 
             self._f1[arm], self._f2[arm] = ii1, ii2
@@ -237,23 +273,17 @@
             # Does this create a view or copy array?
             self._forestwave[arm] = wave_arm[ii1:ii2]
             self._forestflux[arm] = self.flux[arm][ii1:ii2]
             self._forestivar[arm] = self.ivar[arm][ii1:ii2]
             if self.reso:
                 self._forestreso[arm] = self.reso[arm][:, ii1:ii2]
 
-            # np.shares_memory(self.forestflux, self.flux)
-            w = self.forestflux[arm] > 0
-
-            a0 += np.dot(self.forestflux[arm][w], self.forestivar[arm][w])
-            n0 += np.sum(self.forestivar[arm][w])
-
-        self.rsnr /= rsnr_weight
-        self.cont_params['x'][0] = a0 / n0
         self._forestivar_sm = self._forestivar
+        self._forestweight = self._forestivar
+        self._set_forest_related_parameters()
 
     def drop_short_arms(self, lya1=0, lya2=0, skip_ratio=0):
         """Arms that have less than ``skip_ratio`` pixels are removed from
         forest dictionary.
 
         Arguments
         ---------
@@ -268,14 +298,15 @@
                       if np.sum(ivar > 0) < npixels_expected]
         for arm in short_arms:
             self._forestwave.pop(arm, None)
             self._forestflux.pop(arm, None)
             self._forestivar.pop(arm, None)
             self._forestreso.pop(arm, None)
             self._forestivar_sm.pop(arm, None)
+            self._forestweight.pop(arm, None)
             self.cont_params['cont'].pop(arm, None)
 
     def remove_nonforest_pixels(self):
         """ Remove non-forest pixels from storage.
 
         This equates `flux` to `forestflux` etc, but `wave` is not modified,
         since it is a static variable. Good practive is to loop using, e.g.,
@@ -299,81 +330,155 @@
         return size
 
     def is_long(self, dforest_wave, skip_ratio):
         npixels = (1 + self.z_qso) * dforest_wave / self.dwave
         return self.get_real_size() > skip_ratio * npixels
 
     def set_smooth_ivar(self, smoothing_size=16.):
-        """ Set `forestivar_sm` to smoothed inverse variance. Before this call
-        `forestivar_sm` points to `forestivar`.
+        """ Set :attr:`forestivar_sm` to smoothed inverse variance. Before this
+        call :attr:`forestivar_sm` points to :attr:`forestivar`. If
+        ``smoothing_size <= 0``, smoothing is undone such that ivar_sm
+        points to ivar.
+
+
+        ``smoothing_size`` is saved to a private :attr:`_smoothing_scale`
+        variable for future use.
 
         Arguments
         ---------
-        smoothing_size: float, default: 16.
+        smoothing_size: float, default: 16
             Gaussian smoothing spread in A.
         """
         self._forestivar_sm = {}
+        if smoothing_size <= 0:
+            self._smoothing_scale = 0
+            self._forestivar_sm = self._forestivar
+            return
+
+        self._smoothing_scale = smoothing_size
         sigma_pix = smoothing_size / self.dwave
         for arm, ivar_arm in self.forestivar.items():
             self._forestivar_sm[arm] = get_smooth_ivar(ivar_arm, sigma_pix)
 
+    def set_forest_weight(
+            self,
+            varlss_interp=_zero_function,
+            eta_interp=_one_function
+    ):
+        """ Sets :attr:`forestweight` for a given var_lss and eta correction.
+        Always uses :attr:`forestivar_sm`, which is not actually smoothed if
+        :meth:`set_smooth_ivar` is not called.
+
+        .. math::
+
+            w = i / (\\eta + i \\sigma^2_\\mathrm{LSS} C^2),
+
+        where i is IVAR and C is the continuum.
+
+        Arguments
+        ---------
+        varlss_interp: Callable[[ndarray], ndarray], default: 0
+            LSS variance interpolator.
+        eta_interp: Callable[[ndarray], ndarray], default: 1
+            eta interpolator.
+        """
+        self._forestweight = {}
+        if not self.cont_params['valid'] or not self.cont_params['cont']:
+            return
+
+        for arm, wave_arm in self.forestwave.items():
+            cont_est = self.cont_params['cont'][arm]
+            var_lss = varlss_interp(wave_arm) * cont_est**2
+            eta = eta_interp(wave_arm)
+            ivar_arm = self.forestivar_sm[arm]
+            self._forestweight[arm] = ivar_arm / (eta + ivar_arm * var_lss)
+
+    def calc_continuum_chi2(self):
+        """ Calculate the chi2 of the continuum fitting. This is just a sum
+        of weight * (flux - cont)^2.
+
+        Returns
+        -------
+        chi2: float
+        """
+        if not self.cont_params['valid'] or not self.cont_params['cont']:
+            self.cont_params['chi2'] = -1
+            return -1
+
+        chi2 = 0
+        for arm, wave_arm in self.forestwave.items():
+            cont_est = self.cont_params['cont'][arm]
+            weight = self.forestweight[arm]
+            flux = self.forestflux[arm]
+            chi2 += np.dot(weight, (flux - cont_est)**2)
+
+        self.cont_params['chi2'] = chi2
+
+        return chi2
+
     def _coadd_arms_reso(self, nwaves, idxes):
-        """Coadd resolution matrix with equal weights."""
+        """Coadd resolution matrix"""
         max_ndia = np.max([reso.shape[0] for reso in self.forestreso.values()])
         coadd_reso = np.zeros((max_ndia, nwaves))
         creso_norm = np.zeros(nwaves)
 
         for arm, reso_arm in self.forestreso.items():
+            weight = self.forestweight[arm].copy()
+            weight[weight == 0] = 1e-8
+
             reso_arm = self.forestreso[arm]
             ddia = max_ndia - reso_arm.shape[0]
             if ddia > 0:
                 reso_arm = np.pad(reso_arm, ((ddia, ddia), (0, 0)))
 
-            coadd_reso[:, idxes[arm]] += reso_arm
-            creso_norm[idxes[arm]] += 1
+            coadd_reso[:, idxes[arm]] += weight * reso_arm
+            creso_norm[idxes[arm]] += weight
 
         coadd_reso /= creso_norm
         self._forestreso = {'brz': coadd_reso}
 
-    def coadd_arms_forest(self, varlss_interp):
-        """ Coadds different arms using smoothed pipeline ivar and var_lss.
-        Resolution matrix is equally weighted!
+    def coadd_arms_forest(
+            self,
+            varlss_interp=_zero_function,
+            eta_interp=_one_function
+    ):
+        """ Coadds different arms using :attr:`forestweight`. Interpolators are
+        needed to reset :attr:`forestweight`.
 
-        Replaces `forest` variables and ``cont_params['cont']`` with a
+        Replaces ``forest`` variables and ``cont_params['cont']`` with a
         dictionary that has a single arm ``brz`` as key to access coadded data.
 
         Arguments
         ---------
-        varlss_interp: Fast1DInterpolator or any other interpolator.
-            LSS variance interpolator.
+        varlss_interp: Callable[[ndarray], ndarray], default: 0
+            LSS variance interpolator or function.
+        eta_interp: Callable[[ndarray], ndarray], default: 1
+            eta interpolator or function.
         """
         if not self.cont_params['valid'] or not self.cont_params['cont']:
             raise QsonicException("Continuum needed for coadding.")
 
         min_wave = np.min([wave[0] for wave in self.forestwave.values()])
         max_wave = np.max([wave[-1] for wave in self.forestwave.values()])
 
-        nwaves = int((max_wave - min_wave) / self.dwave + 0.5) + 1
+        nwaves = int((max_wave - min_wave) / self.dwave + 0.1) + 1
         coadd_wave = np.arange(nwaves) * self.dwave + min_wave
         coadd_flux = np.zeros(nwaves)
         coadd_ivar = np.zeros(nwaves)
         coadd_cont = np.empty(nwaves)
         coadd_norm = np.zeros(nwaves)
 
         idxes = {}
         for arm, wave_arm in self.forestwave.items():
-            idx = ((wave_arm - min_wave) / self.dwave + 0.5).astype(int)
+            idx = ((wave_arm - min_wave) / self.dwave + 0.1).astype(int)
             idxes[arm] = idx
 
-            var_lss = varlss_interp(wave_arm)
-            var_lss *= self.cont_params['cont'][arm]**2
-            ivar2 = self.forestivar_sm[arm]
-            weight = ivar2 / (1 + ivar2 * var_lss)
+            weight = self.forestweight[arm]
 
-            var = np.zeros_like(ivar2)
+            var = np.zeros_like(weight)
             w = self.forestivar[arm] > 0
             var[w] = 1 / self.forestivar[arm][w]
 
             coadd_flux[idx] += weight * self.forestflux[arm]
             coadd_ivar[idx] += weight**2 * var
             coadd_norm[idx] += weight
 
@@ -385,52 +490,46 @@
         coadd_ivar[w] = coadd_norm[w]**2 / coadd_ivar[w]
 
         self._forestwave = {'brz': coadd_wave}
         self._forestflux = {'brz': coadd_flux}
         self._forestivar = {'brz': coadd_ivar}
         self.cont_params['cont'] = {'brz': coadd_cont}
 
-        if self.reso:
-            self._coadd_arms_reso(nwaves, idxes)
+        self.set_smooth_ivar(self._smoothing_scale)
+        self._forestweight = {}
+        self.set_forest_weight(varlss_interp, eta_interp)
+
+        mean_snr = np.dot(
+            np.sqrt(coadd_ivar), coadd_flux) / np.sum(coadd_ivar > 0)
+        self.mean_snr = {'brz': mean_snr}
 
-    def mean_snr(self):
-        """float: Mean signal-to-noise ratio in the forest."""
-        snr = 0
-        npix = 1e-6
-        for arm, ivar_arm in self.forestivar.items():
-            w = ivar_arm > 0
-            armpix = np.sum(w)
-            if armpix == 0:
-                continue
-
-            snr += np.dot(np.sqrt(ivar_arm), self.forestflux[arm])
-            npix += armpix
-        return snr / npix
+        if self.forestreso:
+            self._coadd_arms_reso(nwaves, idxes)
 
     def mean_resolution(self, arm, weight=None):
         """ Returns the weighted mean Gaussian sigma of the spectrograph
         resolution.
 
         Arguments
         ---------
         arm: str
             Arm.
         weight: None or ndarray, default: None
-            Weights. If ``None``, forestivar_sm is used.
+            Weights. If ``None``, :attr:`forestweight` is used.
 
         Returns
         -------
         mean_reso: float or None
             Gaussian sigma. None if forestreso is not set.
         """
         if not self.forestreso:
             return None
 
         if weight is None:
-            weight = self.forestivar_sm[arm]
+            weight = self.forestweight[arm]
 
         total_weight = np.sum(weight)
         reso = np.dot(self.forestreso[arm], weight) / total_weight
         lambda_eff = np.dot(self.forestwave[arm], weight) / total_weight
 
         central_idx = reso.argmax()
         off_idx = np.array([-2, -1, 1, 2], dtype=int)
@@ -440,68 +539,55 @@
         norm = np.sum(w2)
         new_ratios = np.zeros_like(ratios)
         new_ratios[w2] = 1. / np.sqrt(ratios[w2])
 
         rms_in_pixel = np.abs(off_idx).dot(new_ratios) / np.sqrt(2.) / norm
         return rms_in_pixel * 3e5 * self.dwave / lambda_eff
 
-    def write(self, fts_file, varlss_interp, use_ivar_sm=False):
+    def write(self, fts_file):
         """Writes each arm to FITS file separately.
 
         Writes 'LAMBDA', 'DELTA', 'IVAR', 'WEIGHT', 'CONT' columns and
         'RESOMAT' column if resolution matrix is present to extention name
         ``targetid-arm``. FITS file must be initialized before.
-        Each arm has its own `MEANSNR`. "WEIGHT" in the file do not use
-        smoothed inverse variance by default, which can be changed by
-        ``use_ivar_sm=True``.
+        Each arm has its own `MEANSNR`.
 
         Arguments
         ---------
         fts_file: FITS file
             The file handler, not filename.
-        varlss_interp: Fast1DInterpolator or any other interpolator.
-            LSS variance interpolator.
-        use_ivar_sm: bool, default: False
-            Use :attr:`forestivar_sm` in weights instead.
         """
         hdr_dict = {
             'LOS_ID': self.targetid,
             'TARGETID': self.targetid,
             'RA': np.radians(self.ra),
             'DEC': np.radians(self.dec),
             'Z': self.z_qso,
             'BLINDING': Spectrum._blinding,
             'WAVE_SOLUTION': "lin",
             'MEANSNR': 0.,
             'RSNR': self.rsnr,
             'DELTA_LAMBDA': self.dwave,
-            'SMWEIGHT': use_ivar_sm,
+            'SMSCALE': self._smoothing_scale
         }
 
         for arm, wave_arm in self.forestwave.items():
-            armpix = np.sum(self.forestivar[arm] > 0)
-            if armpix == 0:
+            if self.mean_snr[arm] == 0:
                 continue
 
-            hdr_dict['MEANSNR'] = np.dot(
-                np.sqrt(self.forestivar[arm]),
-                self.forestflux[arm]
-            ) / armpix
+            hdr_dict['MEANSNR'] = self.mean_snr[arm]
 
             cont_est = self.cont_params['cont'][arm]
             delta = self.forestflux[arm] / cont_est - 1
             ivar = self.forestivar[arm] * cont_est**2
-            var_lss = varlss_interp(wave_arm)
-            ivar_w = (
-                self.forestivar_sm[arm] * cont_est**2 if use_ivar_sm else ivar)
-            weight = ivar_w / (1 + ivar_w * var_lss)
+            weight = self.forestweight[arm] * cont_est**2
 
             cols = [wave_arm, delta, ivar, weight, cont_est]
             if self.forestreso:
-                hdr_dict['MEANRESO'] = self.mean_resolution(arm, weight)
+                hdr_dict['MEANRESO'] = self.mean_resolution(arm)
                 cols.append(self.forestreso[arm].T.astype('f8'))
 
             fts_file.write(
                 cols, names=Spectrum._fits_colnames, header=hdr_dict,
                 extname=f"{self.targetid}-{arm}")
 
     @property
@@ -564,14 +650,20 @@
         smoothed inverse variance field.
 
         Initially equal to :attr:`.forestivar`. Smoothed if
         :meth:`.set_smooth_ivar` is called."""
         return self._forestivar_sm
 
     @property
+    def forestweight(self):
+        """dict(:external+numpy:py:class:`ndarray <numpy.ndarray>`): Forest
+        weight field. Initially equal to :attr:`.forestivar`."""
+        return self._forestweight
+
+    @property
     def forestreso(self):
         """dict(:external+numpy:py:class:`ndarray <numpy.ndarray>`): Resolution
         matrix in the forest."""
         return self._forestreso
 
 
 class Delta():
```

### Comparing `qsonic-0.5.2/py/qsonic.egg-info/SOURCES.txt` & `qsonic-0.6.0/py/qsonic.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.rst
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 py/qsonic/__init__.py
+py/qsonic/calibration.py
 py/qsonic/catalog.py
 py/qsonic/io.py
 py/qsonic/masks.py
 py/qsonic/mathtools.py
 py/qsonic/mpi_utils.py
 py/qsonic/picca_continuum.py
 py/qsonic/spectrum.py
```

### Comparing `qsonic-0.5.2/setup.cfg` & `qsonic-0.6.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.5.2
+current_version = 0.6.0
 commit = True
 tag = True
 
 [bumpversion:file:py/qsonic/__init__.py]
 search = __version__ = '{current_version}'
 replace = __version__ = '{new_version}'
```

### Comparing `qsonic-0.5.2/tests/test_catalog.py` & `qsonic-0.6.0/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.5.2/tests/test_io.py` & `qsonic-0.6.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.5.2/tests/test_masks.py` & `qsonic-0.6.0/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.5.2/tests/test_mathtools.py` & `qsonic-0.6.0/tests/test_mathtools.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 import pytest
 
 import numpy as np
-from scipy.interpolate import interp1d
+from scipy.interpolate import interp1d, CubicSpline
 import numpy.testing as npt
 
 import qsonic.mathtools
 
 
 class TestMathtools(object):
-    def test_Fast1DInterpolator(self):
+    def test_FastLinear1DInterp(self):
         xin, dxp = np.linspace(320., 550., 300, retstep=True)
         fp = np.power(xin / 100. - 4., 3)
 
-        fast_interp = qsonic.mathtools.Fast1DInterpolator(xin[0], dxp, fp)
+        fast_interp = qsonic.mathtools.FastLinear1DInterp(xin[0], dxp, fp)
         xarr = np.linspace(310., 560., 100)
         yarr = fast_interp(xarr)
 
         ytrue = interp1d(xin, fp, fill_value='extrapolate')(xarr)
 
         npt.assert_allclose(yarr, ytrue)
 
+    def test_FastCubic1DInterp(self):
+        xin, dxp = np.linspace(320., 550., 300, retstep=True)
+        fp = np.power(xin / 100. - 4., 3)
+
+        fast_interp = qsonic.mathtools.FastCubic1DInterp(xin[0], dxp, fp)
+        xarr = np.linspace(310., 560., 100)
+        yarr = fast_interp(xarr)
+
+        ytrue = CubicSpline(xin, fp, bc_type='natural', extrapolate=True)(xarr)
+
+        npt.assert_allclose(yarr, ytrue)
+
     def test_mypoly1d(self):
         coefs = np.array([5.5, 1.5, 0.7])
         xarr = np.linspace(-2, 2, 100)
         yarr = qsonic.mathtools.mypoly1d(coefs, xarr)
 
         ytrue = np.poly1d(coefs[::-1])(xarr)
 
@@ -54,15 +66,15 @@
 
         for r in randoms:
             subsampler.add_measurement(r, 1)
 
         mean, cov = subsampler.get_mean_n_cov()
 
         npt.assert_allclose(mean, true_mean)
-        npt.assert_almost_equal(cov[0, 0], var_on_mean, decimal=4)
+        npt.assert_almost_equal(cov[0][0], var_on_mean, decimal=4)
 
     def test_SubsampleCov_shape(self):
         subsampler = qsonic.mathtools.SubsampleCov((3, 10), 20)
         randoms = np.random.default_rng().normal(size=(100, 3, 10))
         randoms[:, 1, :] += 1
         randoms[:, 2, :] += 2
 
@@ -75,15 +87,24 @@
 
         mean, var = subsampler.get_mean_n_var()
         npt.assert_allclose(mean, true_mean)
         npt.assert_equal(mean.shape, var.shape)
 
         mean, cov = subsampler.get_mean_n_cov()
         npt.assert_allclose(mean, true_mean)
-        npt.assert_equal(cov.shape, (3, 10, 10))
+        assert (len(cov) == 3)
+        for jj in range(3):
+            npt.assert_equal(cov[jj].shape, (10, 10))
+
+        mean, cov = subsampler.get_mean_n_cov(indices=[0, 1], blockdim=5)
+        npt.assert_allclose(mean, true_mean)
+        assert (len(cov) == 3)
+        for jj in range(2):
+            npt.assert_equal(cov[jj].shape, (2, 5, 5))
+        assert cov[2] is None
 
     def test_SubsampleCov_reset(self):
         subsampler = qsonic.mathtools.SubsampleCov((3, 10), 20)
         subsampler.reset()
 
         npt.assert_equal(subsampler.all_measurements.shape, (20, 3, 10))
         npt.assert_equal(subsampler.all_weights.shape, (20, 1, 10))
```

### Comparing `qsonic-0.5.2/tests/test_mpi_utils.py` & `qsonic-0.6.0/tests/test_mpi_utils.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.5.2/tests/test_picca_continuum.py` & `qsonic-0.6.0/tests/test_picca_continuum.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,15 +214,15 @@
         varlss_fitter.add(
             data['wave']['R'], data['flux']['R'][0], data['ivar']['R'][0])
         expected_numqso[[11, 16]] = 2
         expected_numqso[21] = 1
         npt.assert_equal(varlss_fitter._num_qso, expected_numqso)
 
         expected_size = 3 * nwbins
-        varlss_fitter._allreduce()
+        varlss_fitter._calc_subsampler_stats()
         npt.assert_equal(varlss_fitter.wvalid_bins.sum(), expected_size)
         npt.assert_equal(varlss_fitter.mean_delta.size, expected_size)
 
     def test_fit(self):
         varlss_fitter = VarLSSFitter(
             3600, 4800, nwbins=1, var1=1e-5, var2=2.)
```

### Comparing `qsonic-0.5.2/tests/test_qsonic_calib.py` & `qsonic-0.6.0/tests/test_qsonic_calib.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.5.2/tests/test_spectrum.py` & `qsonic-0.6.0/tests/test_spectrum.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import copy
 import pytest
 
 import numpy as np
 import numpy.testing as npt
 
 import qsonic.spectrum
-from qsonic.mathtools import Fast1DInterpolator
+from qsonic.mathtools import FastLinear1DInterp
 
 
 class TestSpecParsers(object):
     def test_add_wave_region_parser(self):
         parser = argparse.ArgumentParser()
 
         qsonic.spectrum.add_wave_region_parser(parser)
@@ -45,15 +45,15 @@
         spectra_list = qsonic.spectrum.generate_spectra_list_from_data(
             cat_by_survey, data)
 
         spec = spectra_list[0]
         spec.set_forest_region(3600., 6000., 1050., 1180.)
 
         npt.assert_almost_equal(spec.rsnr, 2.1)
-        npt.assert_almost_equal(spec.mean_snr(), 2.1)
+        npt.assert_almost_equal(spec.mean_snr['B'], 2.1)
         npt.assert_almost_equal(spec.cont_params['x'], [2.1, 0.])
         npt.assert_allclose(spec.forestflux['B'], 2.1)
         npt.assert_allclose(spec.forestivar['B'], spec.forestivar_sm['B'])
         assert ('R' not in spec.forestflux.keys())
         assert (not spec.forestreso)
 
     def test_drop_short_arms(self, setup_data):
@@ -104,39 +104,41 @@
 
     def test_coadd_arms_forest(self, setup_data):
         cat_by_survey, _, data = setup_data(1)
         spectra_list = qsonic.spectrum.generate_spectra_list_from_data(
             cat_by_survey, data)
 
         # var_lss zero
-        varlss_interp = Fast1DInterpolator(0, 1, np.zeros(3))
+        varlss_interp = FastLinear1DInterp(0, 1, np.zeros(3))
         spec = copy.deepcopy(spectra_list[0])
         spec.set_forest_region(3600., 6000., 1050., 1300.)
         spec.cont_params['valid'] = True
         spec.cont_params['cont'] = {
             arm: np.ones_like(farm) for arm, farm in spec.forestflux.items()
         }
+        spec.set_forest_weight(varlss_interp)
         spec.coadd_arms_forest(varlss_interp)
 
         assert ('brz' in spec.forestflux.keys())
         npt.assert_almost_equal(spec.forestflux['brz'], 2.1)
         npt.assert_almost_equal(spec.cont_params['cont']['brz'], 1.)
         w = (spec.forestwave['brz'] < data['wave']['R'][0])\
             | (spec.forestwave['brz'] > data['wave']['B'][-1])
         npt.assert_almost_equal(spec.forestivar['brz'][w], 1)
         npt.assert_almost_equal(spec.forestivar['brz'][~w], 2)
 
         # var_lss non-zero
-        varlss_interp = Fast1DInterpolator(0, 1, 0.5 * np.ones(3))
+        varlss_interp = FastLinear1DInterp(0, 1, 0.5 * np.ones(3))
         spec = copy.deepcopy(spectra_list[0])
         spec.set_forest_region(3600., 6000., 1050., 1300.)
         spec.cont_params['valid'] = True
         spec.cont_params['cont'] = {
             arm: np.ones_like(farm) for arm, farm in spec.forestflux.items()
         }
+        spec.set_forest_weight(varlss_interp)
         spec.coadd_arms_forest(varlss_interp)
 
         assert ('brz' in spec.forestflux.keys())
         npt.assert_almost_equal(spec.forestflux['brz'], 2.1)
         npt.assert_almost_equal(spec.cont_params['cont']['brz'], 1.)
         w = (spec.forestwave['brz'] < data['wave']['R'][0])\
             | (spec.forestwave['brz'] > data['wave']['B'][-1])
```


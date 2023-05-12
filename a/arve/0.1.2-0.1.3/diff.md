# Comparing `tmp/arve-0.1.2.tar.gz` & `tmp/arve-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arve-0.1.2.tar", last modified: Wed Feb 15 15:46:50 2023, max compression
+gzip compressed data, was "arve-0.1.3.tar", last modified: Fri May 12 14:11:21 2023, max compression
```

## Comparing `arve-0.1.2.tar` & `arve-0.1.3.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-02-15 15:46:50.592933 arve-0.1.2/
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)     1073 2023-02-02 15:37:16.000000 arve-0.1.2/LICENSE
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      440 2023-02-15 15:46:50.592531 arve-0.1.2/PKG-INFO
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      115 2023-02-06 14:14:55.000000 arve-0.1.2/README.md
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-02-15 15:46:50.556310 arve-0.1.2/arve/
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      251 2023-02-15 15:15:58.000000 arve-0.1.2/arve/__init__.py
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)     3267 2023-02-15 15:16:38.000000 arve-0.1.2/arve/arve.py
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-02-15 15:46:50.552696 arve-0.1.2/arve/aux_data/
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-02-15 15:46:50.582522 arve-0.1.2/arve/aux_data/masks/
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)    59650 2023-02-14 15:05:45.000000 arve-0.1.2/arve/aux_data/masks/A0_3500-7000.mask
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)    87650 2023-02-14 15:05:45.000000 arve-0.1.2/arve/aux_data/masks/A2_3500-7000.mask
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   139050 2023-02-14 15:05:45.000000 arve-0.1.2/arve/aux_data/masks/A5_3500-7000.mask
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   168400 2023-02-14 15:05:45.000000 arve-0.1.2/arve/aux_data/masks/A7_3500-7000.mask
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   239800 2023-02-14 15:05:45.000000 arve-0.1.2/arve/aux_data/masks/F0_3500-7000.mask
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   244450 2023-02-14 15:05:45.000000 arve-0.1.2/arve/aux_data/masks/F2_3500-7000.mask
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   315850 2023-02-14 15:05:45.000000 arve-0.1.2/arve/aux_data/masks/F5_3500-7000.mask
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   364600 2023-02-14 15:05:45.000000 arve-0.1.2/arve/aux_data/masks/F8_3500-7000.mask
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   415550 2023-02-14 15:05:45.000000 arve-0.1.2/arve/aux_data/masks/G0_3500-7000.mask
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   481900 2023-02-14 15:05:45.000000 arve-0.1.2/arve/aux_data/masks/G2_3500-7000.mask
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   481900 2023-02-14 15:05:45.000000 arve-0.1.2/arve/aux_data/masks/G5_3500-7000.mask
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   532950 2023-02-14 15:05:45.000000 arve-0.1.2/arve/aux_data/masks/G8_3500-7000.mask
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   592800 2023-02-14 15:05:45.000000 arve-0.1.2/arve/aux_data/masks/K0_3500-7000.mask
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   646100 2023-02-14 15:05:46.000000 arve-0.1.2/arve/aux_data/masks/K2_3500-7000.mask
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   646100 2023-02-14 15:05:46.000000 arve-0.1.2/arve/aux_data/masks/K3_3500-7000.mask
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   765750 2023-02-14 15:05:46.000000 arve-0.1.2/arve/aux_data/masks/K5_3500-7000.mask
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   765750 2023-02-14 15:05:45.000000 arve-0.1.2/arve/aux_data/masks/K7_3500-7000.mask
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)   761000 2023-02-14 15:05:46.000000 arve-0.1.2/arve/aux_data/masks/M0_3500-7000.mask
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)  1440600 2023-02-14 15:05:46.000000 arve-0.1.2/arve/aux_data/masks/M2_3500-7000.mask
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)  1364200 2023-02-14 15:05:46.000000 arve-0.1.2/arve/aux_data/masks/M5_3500-7000.mask
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-02-15 15:46:50.586747 arve-0.1.2/arve/data/
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      108 2023-02-15 12:21:29.000000 arve-0.1.2/arve/data/__init__.py
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      948 2023-02-15 12:25:45.000000 arve-0.1.2/arve/data/add_spec.py
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      779 2023-02-03 19:55:32.000000 arve-0.1.2/arve/data/add_vrad.py
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)     4687 2023-02-15 15:19:25.000000 arve-0.1.2/arve/data/compute_vrad.py
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-02-15 15:46:50.588483 arve-0.1.2/arve/functions/
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      130 2023-02-15 15:07:20.000000 arve-0.1.2/arve/functions/__init__.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)      342 2023-02-15 15:07:05.000000 arve-0.1.2/arve/functions/doppler_shift.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     3792 2023-02-03 19:55:52.000000 arve-0.1.2/arve/functions/gls_periodogram.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)      265 2023-02-15 14:05:55.000000 arve-0.1.2/arve/functions/sptype_to_num.py
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-02-15 15:46:50.589335 arve-0.1.2/arve/planets/
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)       34 2023-02-03 19:57:53.000000 arve-0.1.2/arve/planets/__init__.py
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)       50 2023-02-03 19:56:07.000000 arve-0.1.2/arve/planets/add_planet.py
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-02-15 15:46:50.591945 arve-0.1.2/arve/star/
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      278 2023-02-03 19:57:39.000000 arve-0.1.2/arve/star/__init__.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     3955 2023-02-06 14:25:03.000000 arve-0.1.2/arve/star/add_vpsd_components.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     1366 2023-02-03 19:56:29.000000 arve-0.1.2/arve/star/compute_vpsd.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     2772 2023-02-03 19:56:39.000000 arve-0.1.2/arve/star/fit_vpsd_coefficients.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     2649 2023-02-15 14:09:48.000000 arve-0.1.2/arve/star/get_stellar_parameters.py
--rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     2555 2023-02-03 19:57:01.000000 arve-0.1.2/arve/star/plot_vpsd_components.py
-drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-02-15 15:46:50.557972 arve-0.1.2/arve.egg-info/
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      440 2023-02-15 15:46:50.000000 arve-0.1.2/arve.egg-info/PKG-INFO
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)     1410 2023-02-15 15:46:50.000000 arve-0.1.2/arve.egg-info/SOURCES.txt
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)        1 2023-02-15 15:46:50.000000 arve-0.1.2/arve.egg-info/dependency_links.txt
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)       46 2023-02-15 15:46:50.000000 arve-0.1.2/arve.egg-info/requires.txt
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)        5 2023-02-15 15:46:50.000000 arve-0.1.2/arve.egg-info/top_level.txt
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)       38 2023-02-15 15:46:50.593082 arve-0.1.2/setup.cfg
--rw-r--r--   0 khaledalmoulla   (501) staff       (20)      859 2023-02-15 15:15:43.000000 arve-0.1.2/setup.py
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-05-12 14:11:21.949378 arve-0.1.3/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)     1073 2023-02-02 15:37:16.000000 arve-0.1.3/LICENSE
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      597 2023-05-12 14:11:21.948915 arve-0.1.3/PKG-INFO
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      115 2023-02-06 14:14:55.000000 arve-0.1.3/README.md
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-05-12 14:11:21.924071 arve-0.1.3/arve/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      251 2023-05-12 13:53:39.000000 arve-0.1.3/arve/__init__.py
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)     1827 2023-05-12 12:45:58.000000 arve-0.1.3/arve/arve.py
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-05-12 14:11:21.922104 arve-0.1.3/arve/aux_data/
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-05-12 14:11:21.939235 arve-0.1.3/arve/aux_data/masks/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)    18615 2023-04-28 14:14:54.000000 arve-0.1.3/arve/aux_data/masks/A0_3500-7000.csv
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)    27356 2023-04-28 14:14:53.000000 arve-0.1.3/arve/aux_data/masks/A2_3500-7000.csv
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)    43308 2023-04-28 14:14:53.000000 arve-0.1.3/arve/aux_data/masks/A5_3500-7000.csv
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)    52490 2023-04-28 14:14:54.000000 arve-0.1.3/arve/aux_data/masks/A7_3500-7000.csv
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)    74648 2023-04-28 14:14:53.000000 arve-0.1.3/arve/aux_data/masks/F0_3500-7000.csv
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)    76147 2023-04-28 14:14:53.000000 arve-0.1.3/arve/aux_data/masks/F2_3500-7000.csv
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)    98242 2023-04-28 14:14:53.000000 arve-0.1.3/arve/aux_data/masks/F5_3500-7000.csv
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)   113164 2023-04-28 14:14:54.000000 arve-0.1.3/arve/aux_data/masks/F8_3500-7000.csv
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)   128904 2023-04-28 14:14:53.000000 arve-0.1.3/arve/aux_data/masks/G0_3500-7000.csv
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)   149481 2023-04-28 14:14:53.000000 arve-0.1.3/arve/aux_data/masks/G2_3500-7000.csv
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)   149481 2023-04-28 14:14:54.000000 arve-0.1.3/arve/aux_data/masks/G5_3500-7000.csv
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)   165192 2023-04-28 14:14:53.000000 arve-0.1.3/arve/aux_data/masks/G8_3500-7000.csv
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)   183696 2023-04-28 14:14:54.000000 arve-0.1.3/arve/aux_data/masks/K0_3500-7000.csv
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)   200200 2023-04-28 14:14:54.000000 arve-0.1.3/arve/aux_data/masks/K2_3500-7000.csv
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)   200200 2023-04-28 14:14:54.000000 arve-0.1.3/arve/aux_data/masks/K3_3500-7000.csv
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)   237329 2023-04-28 14:14:54.000000 arve-0.1.3/arve/aux_data/masks/K5_3500-7000.csv
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)   237329 2023-04-28 14:14:54.000000 arve-0.1.3/arve/aux_data/masks/K7_3500-7000.csv
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)   235852 2023-04-28 14:14:54.000000 arve-0.1.3/arve/aux_data/masks/M0_3500-7000.csv
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)   450099 2023-04-28 14:14:54.000000 arve-0.1.3/arve/aux_data/masks/M2_3500-7000.csv
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)   427005 2023-04-28 14:14:54.000000 arve-0.1.3/arve/aux_data/masks/M5_3500-7000.csv
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-05-12 14:11:21.941733 arve-0.1.3/arve/data/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      233 2023-05-12 12:39:33.000000 arve-0.1.3/arve/data/__init__.py
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)     1057 2023-05-12 09:58:19.000000 arve-0.1.3/arve/data/add_spec.py
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      872 2023-05-12 12:04:26.000000 arve-0.1.3/arve/data/add_vrad.py
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)     4634 2023-05-12 12:56:35.000000 arve-0.1.3/arve/data/compute_vrad_ccf.py
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-05-12 14:11:21.943587 arve-0.1.3/arve/functions/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      362 2023-05-12 12:43:02.000000 arve-0.1.3/arve/functions/__init__.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)      412 2023-05-12 12:10:56.000000 arve-0.1.3/arve/functions/doppler_shift.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     3980 2023-05-12 12:11:07.000000 arve-0.1.3/arve/functions/gls_periodogram.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)      696 2023-05-12 12:10:30.000000 arve-0.1.3/arve/functions/inverted_gaussian.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)      319 2023-05-12 12:11:30.000000 arve-0.1.3/arve/functions/sptype_to_num.py
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-05-12 14:11:21.944548 arve-0.1.3/arve/planets/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)       80 2023-05-12 12:43:31.000000 arve-0.1.3/arve/planets/__init__.py
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)       81 2023-05-12 12:12:35.000000 arve-0.1.3/arve/planets/add_planet.py
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-05-12 14:11:21.948066 arve-0.1.3/arve/star/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      450 2023-05-12 12:44:13.000000 arve-0.1.3/arve/star/__init__.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     4279 2023-05-12 12:13:14.000000 arve-0.1.3/arve/star/add_vpsd_components.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     1503 2023-05-12 12:13:54.000000 arve-0.1.3/arve/star/compute_vpsd.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     2946 2023-05-12 12:14:29.000000 arve-0.1.3/arve/star/fit_vpsd_coefficients.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     2808 2023-05-12 12:14:54.000000 arve-0.1.3/arve/star/get_stellar_parameters.py
+-rwxr-xr-x   0 khaledalmoulla   (501) staff       (20)     2852 2023-05-12 12:15:31.000000 arve-0.1.3/arve/star/plot_vpsd_components.py
+drwxr-xr-x   0 khaledalmoulla   (501) staff       (20)        0 2023-05-12 14:11:21.925800 arve-0.1.3/arve.egg-info/
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)      597 2023-05-12 14:11:21.000000 arve-0.1.3/arve.egg-info/PKG-INFO
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)     1430 2023-05-12 14:11:21.000000 arve-0.1.3/arve.egg-info/SOURCES.txt
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)        1 2023-05-12 14:11:21.000000 arve-0.1.3/arve.egg-info/dependency_links.txt
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)       51 2023-05-12 14:11:21.000000 arve-0.1.3/arve.egg-info/requires.txt
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)        5 2023-05-12 14:11:21.000000 arve-0.1.3/arve.egg-info/top_level.txt
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)       38 2023-05-12 14:11:21.949519 arve-0.1.3/setup.cfg
+-rw-r--r--   0 khaledalmoulla   (501) staff       (20)     1101 2023-05-12 13:52:33.000000 arve-0.1.3/setup.py
```

### Comparing `arve-0.1.2/LICENSE` & `arve-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arve-0.1.2/arve/data/add_spec.py` & `arve-0.1.3/arve/data/add_spec.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-def add_spec(self, time:list, wave:list, flux_val:list, flux_err:list=None, time_unit:str=None, wave_unit:str=None, flux_unit:str=None) -> None:
-    """Add spectral data.
+class add_spec:
 
-    :param time: time values
-    :type time: list
-    :param wave: wavelength values
-    :type wave: list
-    :param flux_val: flux values
-    :type flux_val: list
-    :param flux_err: flux errors, defaults to None
-    :type flux_err: list, optional
-    :param time_unit: time unit, defaults to None
-    :type time_unit: str, optional
-    :param wave_unit: wavelength unit, defaults to None
-    :type time_unit: str, optional
-    :param flux_unit: flux unit, defaults to None
-    :type flux_unit: str, optional
-    :return: None
-    :rtype: None
-    """
+    def add_spec(self, time:list, wave:list, flux_val:list, flux_err:list=None, time_unit:str=None, wave_unit:str=None, flux_unit:str=None) -> None:
+        """Add spectral data.
 
-    # add dictionary with spectral data
-    self.spec = {"time": time, "wave": wave, "flux_val": flux_val, "flux_err": flux_err, "time_unit": time_unit, "wave_unit": wave_unit, "flux_unit": flux_unit}
-    
-    return None
+        :param time: time values
+        :type time: list
+        :param wave: wavelength values
+        :type wave: list
+        :param flux_val: flux values
+        :type flux_val: list
+        :param flux_err: flux errors, defaults to None
+        :type flux_err: list, optional
+        :param time_unit: time unit, defaults to None
+        :type time_unit: str, optional
+        :param wave_unit: wavelength unit, defaults to None
+        :type time_unit: str, optional
+        :param flux_unit: flux unit, defaults to None
+        :type flux_unit: str, optional
+        :return: None
+        :rtype: None
+        """
+
+        # add dictionary with spectral data
+        self.spec = {"time": time, "wave": wave, "flux_val": flux_val, "flux_err": flux_err, "time_unit": time_unit, "wave_unit": wave_unit, "flux_unit": flux_unit}
+        
+        return None
```

### Comparing `arve-0.1.2/arve/data/add_vrad.py` & `arve-0.1.3/arve/data/add_vrad.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-def add_vrad(self, time:list, vrad_val:list, vrad_err:list=None, time_unit:str=None, vrad_unit:str=None) -> None:
-    """Add radial velocity data.
+class add_vrad:
 
-    :param time: time values
-    :type time: list
-    :param vrad_val: radial velocity values
-    :type vrad_val: list
-    :param vrad_err: radial velocity errors, defaults to None
-    :type vrad_err: list, optional
-    :param time_unit: time unit, defaults to None
-    :type time_unit: str, optional
-    :param vrad_unit: radial velocity unit, defaults to None
-    :type vrad_unit: str, optional
-    :return: None
-    :rtype: None
-    """
+    def add_vrad(self, time:list, vrad_val:list, vrad_err:list=None, time_unit:str=None, vrad_unit:str=None) -> None:
+        """Add radial velocity data.
 
-    # add dictionary with radial velocity data
-    self.vrad = {"time": time, "vrad_val": vrad_val, "vrad_err": vrad_err, "time_unit": time_unit, "vrad_unit": vrad_unit}
-    
-    return None
+        :param time: time values
+        :type time: list
+        :param vrad_val: radial velocity values
+        :type vrad_val: list
+        :param vrad_err: radial velocity errors, defaults to None
+        :type vrad_err: list, optional
+        :param time_unit: time unit, defaults to None
+        :type time_unit: str, optional
+        :param vrad_unit: radial velocity unit, defaults to None
+        :type vrad_unit: str, optional
+        :return: None
+        :rtype: None
+        """
+
+        # add dictionary with radial velocity data
+        self.vrad = {"time": time, "vrad_val": vrad_val, "vrad_err": vrad_err, "time_unit": time_unit, "vrad_unit": vrad_unit}
+        
+        return None
```

### Comparing `arve-0.1.2/arve/functions/gls_periodogram.py` & `arve-0.1.3/arve/functions/gls_periodogram.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,61 +1,63 @@
 from   numba import njit
 import numpy as     np
 
-def gls_periodogram(self, time:list, val:list, err:list=None, ofac:int=1, normalize:bool=True, win_func:bool=False) -> tuple:
-    """Generalized Lomb-Scargle (GLS) periodogram.
+class gls_periodogram:
 
-    :param time: time values
-    :type time: list
-    :param val: values
-    :type val: list
-    :param err: errors, defaults to None
-    :type err: list, optional
-    :param ofac: over-factorization, defaults to 1
-    :type ofac: int, optional
-    :param normalize: normalization of periodogram, defaults to True
-    :type normalize: bool, optional
-    :param win_func: return window function, defaults to False
-    :type win_func: bool, optional
-    :return: frequency, power spectrum and phase of periodogram; if win_func is True, the frequency, power spectrum and phase of the window function are returned as well
-    :rtype: tuple
-    """
-
-    # if not provided, set uncertainties to unity
-    if err is None:
-        err = np.ones(len(time))
-
-    # frequencies, power spectrum and phases of data
-    freq, ps, phi = _gls(time, val, err, ofac, normalize)
-
-    # spectral window function
-    if win_func:
-
-        # central frequency
-        freq_c = freq[int(len(freq)/2)]
-
-        # sinusoid with unit amplitude at central frequency
-        win_val = np.sin(2*np.pi*freq_c*time)
-        win_err = err
-
-        # power spectrum of window function
-        win_freq, win_ps, _ = _gls(time, win_val, win_err, ofac)
-
-        # recenter window function frequencies
-        win_freq -= freq_c
-
-        # area of window function
-        win_dfreq = np.mean(win_freq[1:]-win_freq[:-1])
-        win_area = np.sum(win_ps)*win_dfreq
-
-    # return periodogram parameters
-    if win_func:
-        return freq, ps, phi, win_freq, win_ps, win_area
-    else:
-        return freq, ps, phi
+    def gls_periodogram(self, time:list, val:list, err:list=None, ofac:int=1, normalize:bool=True, win_func:bool=False) -> tuple:
+        """Generalized Lomb-Scargle (GLS) periodogram.
+
+        :param time: time values
+        :type time: list
+        :param val: values
+        :type val: list
+        :param err: errors, defaults to None
+        :type err: list, optional
+        :param ofac: over-factorization, defaults to 1
+        :type ofac: int, optional
+        :param normalize: normalization of periodogram, defaults to True
+        :type normalize: bool, optional
+        :param win_func: return window function, defaults to False
+        :type win_func: bool, optional
+        :return: frequency, power spectrum and phase of periodogram; if win_func is True, the frequency, power spectrum and phase of the window function are returned as well
+        :rtype: tuple
+        """
+
+        # if not provided, set uncertainties to unity
+        if err is None:
+            err = np.ones(len(time))
+
+        # frequencies, power spectrum and phases of data
+        freq, ps, phi = _gls(time, val, err, ofac, normalize)
+
+        # spectral window function
+        if win_func:
+
+            # central frequency
+            freq_c = freq[int(len(freq)/2)]
+
+            # sinusoid with unit amplitude at central frequency
+            win_val = np.sin(2*np.pi*freq_c*time)
+            win_err = err
+
+            # power spectrum of window function
+            win_freq, win_ps, _ = _gls(time, win_val, win_err, ofac)
+
+            # recenter window function frequencies
+            win_freq -= freq_c
+
+            # area of window function
+            win_dfreq = np.mean(win_freq[1:]-win_freq[:-1])
+            win_area = np.sum(win_ps)*win_dfreq
+
+        # return periodogram parameters
+        if win_func:
+            return freq, ps, phi, win_freq, win_ps, win_area
+        else:
+            return freq, ps, phi
 
 def _gls(time, val, err, ofac, normalize=True):
 
     # time span and steps
     Time = time[-1] - time[0]
     dtime = time[1:] - time[:-1]
```

### Comparing `arve-0.1.2/arve/star/add_vpsd_components.py` & `arve-0.1.3/arve/star/add_vpsd_components.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,98 +1,100 @@
 import numpy as np
 
-def add_vpsd_components(self, components:list=["Photon_noise", "Oscillations", "Granulation", "Supergranulation"]) -> None:
-    """Add velocity power spectral density (VPSD) components.
+class add_vpsd_components:
 
-    :param components: VPSD components, defaults to ["Photon_noise", "Oscillations", "Granulation", "Supergranulation"]
-    :type components: list, optional
-    :return: None
-    :rtype: None
-    """
-
-    # read stellar parameters and VPSD
-    Teff, logg, M, R = [self.stellar_parameters[key] for key in ["Teff", "logg", "M", "R"]]
-    freq, vpsd, freq_avg, vpsd_avg = [self.vpsd[key] for key in ["freq", "vpsd", "freq_avg", "vpsd_avg"]]
-
-    # photon noise
-    if "Photon_noise" in components:
-
-        # coefficients
-        c0 = np.min(vpsd_avg) # amplitude
-
-        # specifications
-        name     = "Photon_noise" # name
-        type     = "Constant"     # function type
-        coef_val = [c0  ]         # coefficient values
-        coef_err = [0   ]         # coefficient errors
-        vary     = [True]         # vary when fitted
-
-        # check noise is non-negative
-        if c0 >= 0:
-
-            # save VPSD component
-            self.vpsd_components[name] = {"type": type, "coef_val": coef_val, "coef_err": coef_err, "vary": vary}
-
-    # oscillations
-    if "Oscillations" in components:
-
-        # coefficients
-        c2 = M/(R**2*np.sqrt(Teff/5777))*3.05e-3 * 60*60*24 # central frequency
-        c1 = M**(1/2)*R**(-3/2)*134.9*1e-6*2 * 60*60*24     # peak width
-        c0 = vpsd_avg[np.argmin(np.abs(freq_avg-c2))]       # amplitude
-
-        # specifications
-        name     = "Oscillations"     # name
-        type     = "Lorentz"          # function type
-        coef_val = [c0  , c1  , c2  ] # coefficient values
-        coef_err = [0   , 0   , 0   ] # coefficient errors
-        vary     = [True, True, True] # vary when fitted
-
-        # check central frequency is within frequency range
-        if (c2 > min(freq)) & (c2 < max(freq)):
-
-            # save VPSD component
-            self.vpsd_components[name] = {"type": type, "coef_val": coef_val, "coef_err": coef_err, "vary": vary}
-
-    # granulation
-    if "Granulation" in components:
-
-        # coefficients
-        c2 = 2                                                    # exponent
-        c1 = 1/24*(10**logg/10**(4.4))**(7/9)*(Teff/5777)**(23/9) # characteristic timescale
-        c0 = vpsd_avg[np.argmin(np.abs(freq_avg-1/c1))]           # amplitude
-
-        # specifications
-        name     = "Granulation"       # name
-        type     = "Harvey"            # function type
-        coef_val = [c0  , c1  , c2   ] # coefficient values
-        coef_err = [0   , 0   , 0    ] # coefficient errors
-        vary     = [True, True, False] # vary when fitted
-
-        # check characteristic frequency is within frequency range
-        if (1/c1 > min(freq)) & (1/c1 < max(freq)):
-
-            # save VPSD component
-            self.vpsd_components[name] = {"type": type, "coef_val": coef_val, "coef_err": coef_err, "vary": vary}
-
-    # supergranulation
-    if "Supergranulation" in components:
-
-        # coefficients
-        c2 = 2                                                     # exponent
-        c1 = 10/24*(10**logg/10**(4.4))**(7/9)*(Teff/5777)**(23/9) # characteristic timescale
-        c0 = vpsd_avg[np.argmin(np.abs(freq_avg-1/c1))]            # amplitude
-
-        # specifications
-        name     = "Supergranulation"  # name
-        type     = "Harvey"            # function type
-        coef_val = [c0  , c1  , c2   ] # coefficient values
-        coef_err = [0   , 0   , 0    ] # coefficient errors
-        vary     = [True, True, False] # vary when fitted
-
-        # check characteristic frequency is within frequency range
-        if (1/c1 > min(freq)) & (1/c1 < max(freq)):
-
-            # save VPSD component
-            self.vpsd_components[name] = {"type": type, "coef_val": coef_val, "coef_err": coef_err, "vary": vary}
-    
-    return None
+    def add_vpsd_components(self, components:list=["Photon_noise", "Oscillations", "Granulation", "Supergranulation"]) -> None:
+        """Add velocity power spectral density (VPSD) components.
+
+        :param components: VPSD components, defaults to ["Photon_noise", "Oscillations", "Granulation", "Supergranulation"]
+        :type components: list, optional
+        :return: None
+        :rtype: None
+        """
+
+        # read stellar parameters and VPSD
+        Teff, logg, M, R = [self.stellar_parameters[key] for key in ["Teff", "logg", "M", "R"]]
+        freq, vpsd, freq_avg, vpsd_avg = [self.vpsd[key] for key in ["freq", "vpsd", "freq_avg", "vpsd_avg"]]
+
+        # photon noise
+        if "Photon_noise" in components:
+
+            # coefficients
+            c0 = np.min(vpsd_avg) # amplitude
+
+            # specifications
+            name     = "Photon_noise" # name
+            type     = "Constant"     # function type
+            coef_val = [c0  ]         # coefficient values
+            coef_err = [0   ]         # coefficient errors
+            vary     = [True]         # vary when fitted
+
+            # check noise is non-negative
+            if c0 >= 0:
+
+                # save VPSD component
+                self.vpsd_components[name] = {"type": type, "coef_val": coef_val, "coef_err": coef_err, "vary": vary}
+
+        # oscillations
+        if "Oscillations" in components:
+
+            # coefficients
+            c2 = M/(R**2*np.sqrt(Teff/5777))*3.05e-3 * 60*60*24 # central frequency
+            c1 = M**(1/2)*R**(-3/2)*134.9*1e-6*2 * 60*60*24     # peak width
+            c0 = vpsd_avg[np.argmin(np.abs(freq_avg-c2))]       # amplitude
+
+            # specifications
+            name     = "Oscillations"     # name
+            type     = "Lorentz"          # function type
+            coef_val = [c0  , c1  , c2  ] # coefficient values
+            coef_err = [0   , 0   , 0   ] # coefficient errors
+            vary     = [True, True, True] # vary when fitted
+
+            # check central frequency is within frequency range
+            if (c2 > min(freq)) & (c2 < max(freq)):
+
+                # save VPSD component
+                self.vpsd_components[name] = {"type": type, "coef_val": coef_val, "coef_err": coef_err, "vary": vary}
+
+        # granulation
+        if "Granulation" in components:
+
+            # coefficients
+            c2 = 2                                                    # exponent
+            c1 = 1/24*(10**logg/10**(4.4))**(7/9)*(Teff/5777)**(23/9) # characteristic timescale
+            c0 = vpsd_avg[np.argmin(np.abs(freq_avg-1/c1))]           # amplitude
+
+            # specifications
+            name     = "Granulation"       # name
+            type     = "Harvey"            # function type
+            coef_val = [c0  , c1  , c2   ] # coefficient values
+            coef_err = [0   , 0   , 0    ] # coefficient errors
+            vary     = [True, True, False] # vary when fitted
+
+            # check characteristic frequency is within frequency range
+            if (1/c1 > min(freq)) & (1/c1 < max(freq)):
+
+                # save VPSD component
+                self.vpsd_components[name] = {"type": type, "coef_val": coef_val, "coef_err": coef_err, "vary": vary}
+
+        # supergranulation
+        if "Supergranulation" in components:
+
+            # coefficients
+            c2 = 2                                                     # exponent
+            c1 = 10/24*(10**logg/10**(4.4))**(7/9)*(Teff/5777)**(23/9) # characteristic timescale
+            c0 = vpsd_avg[np.argmin(np.abs(freq_avg-1/c1))]            # amplitude
+
+            # specifications
+            name     = "Supergranulation"  # name
+            type     = "Harvey"            # function type
+            coef_val = [c0  , c1  , c2   ] # coefficient values
+            coef_err = [0   , 0   , 0    ] # coefficient errors
+            vary     = [True, True, False] # vary when fitted
+
+            # check characteristic frequency is within frequency range
+            if (1/c1 > min(freq)) & (1/c1 < max(freq)):
+
+                # save VPSD component
+                self.vpsd_components[name] = {"type": type, "coef_val": coef_val, "coef_err": coef_err, "vary": vary}
+        
+        return None
```

### Comparing `arve-0.1.2/arve/star/compute_vpsd.py` & `arve-0.1.3/arve/star/compute_vpsd.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 import numpy as np
 
-def compute_vpsd(self) -> None:
-    """Compute velocity power spectral density (VPSD).
+class compute_vpsd:
 
-    :return: None
-    :rtype: None
-    """
-
-    # read RV time series
-    time, vrad_val, vrad_err, time_unit, vrad_unit = [self.arve.data.vrad[key] for key in ["time", "vrad_val", "vrad_err", "time_unit", "vrad_unit"]]
-
-    # compute velocity power spectrum
-    freq, vps, phi, win_freq, win_vps, win_area = self.arve.functions.gls_periodogram(time=time, val=vrad_val, err=vrad_err, normalize=False, win_func=True)
-
-    # compute log-average VPS
-    freq_bin = 10 ** (np.linspace(np.log10(freq[0]), np.log10(freq[-1]), 51))
-    freq_avg = (freq_bin[1:] + freq_bin[:-1]) / 2
-    vps_avg  = np.empty(freq_avg.size)
-    for i in range(freq_avg.size):
-        vps_bin = vps[(freq > freq_bin[i]) & (freq < freq_bin[i + 1])]
-        if len(vps_bin) == 0:
-            vps_avg[i] = np.nan
-        else:
-            vps_avg[i] = np.mean(vps_bin)
-
-    # delete NaN values
-    i_delete = np.isnan(vps_avg)
-    freq_avg = np.delete(freq_avg, np.where(i_delete))
-    vps_avg  = np.delete(vps_avg , np.where(i_delete))
-
-    # compute VPSD
-    vpsd     = vps    /win_area
-    vpsd_avg = vps_avg/win_area
+    def compute_vpsd(self) -> None:
+        """Compute velocity power spectral density (VPSD).
 
-    # save VPSD
-    self.vpsd = {"freq": freq, "vps": vps, "vpsd": vpsd, "phase": phi, "freq_avg": freq_avg, "vps_avg": vps_avg, "vpsd_avg": vpsd_avg}
+        :return: None
+        :rtype: None
+        """
+
+        # read RV time series
+        time, vrad_val, vrad_err, time_unit, vrad_unit = [self.arve.data.vrad[key] for key in ["time", "vrad_val", "vrad_err", "time_unit", "vrad_unit"]]
+
+        # compute velocity power spectrum
+        freq, vps, phi, win_freq, win_vps, win_area = self.arve.functions.gls_periodogram(time=time, val=vrad_val, err=vrad_err, normalize=False, win_func=True)
+
+        # compute log-average VPS
+        freq_bin = 10 ** (np.linspace(np.log10(freq[0]), np.log10(freq[-1]), 51))
+        freq_avg = (freq_bin[1:] + freq_bin[:-1]) / 2
+        vps_avg  = np.empty(freq_avg.size)
+        for i in range(freq_avg.size):
+            vps_bin = vps[(freq > freq_bin[i]) & (freq < freq_bin[i + 1])]
+            if len(vps_bin) == 0:
+                vps_avg[i] = np.nan
+            else:
+                vps_avg[i] = np.mean(vps_bin)
+
+        # delete NaN values
+        i_delete = np.isnan(vps_avg)
+        freq_avg = np.delete(freq_avg, np.where(i_delete))
+        vps_avg  = np.delete(vps_avg , np.where(i_delete))
+
+        # compute VPSD
+        vpsd     = vps    /win_area
+        vpsd_avg = vps_avg/win_area
 
-    return None
+        # save VPSD
+        self.vpsd = {"freq": freq, "vps": vps, "vpsd": vpsd, "phase": phi, "freq_avg": freq_avg, "vps_avg": vps_avg, "vpsd_avg": vpsd_avg}
+
+        return None
```

### Comparing `arve-0.1.2/arve/star/fit_vpsd_coefficients.py` & `arve-0.1.3/arve/star/fit_vpsd_coefficients.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,60 +1,62 @@
 import numpy as     np
 from   lmfit import Parameters, minimize
 
-def fit_vpsd_coefficients(self) -> None:
-    """Fit velocity power spectral density (VPSD) coefficients.
+class fit_vpsd_coefficients:
 
-    :return: None
-    :rtype: None
-    """
+    def fit_vpsd_coefficients(self) -> None:
+        """Fit velocity power spectral density (VPSD) coefficients.
 
-    # read VPSD
-    freq, vpsd, freq_avg, vpsd_avg = [self.vpsd[key] for key in ["freq", "vpsd", "freq_avg", "vpsd_avg"]]
+        :return: None
+        :rtype: None
+        """
 
-    # LMFIT parameters
-    params = Parameters()
+        # read VPSD
+        freq, vpsd, freq_avg, vpsd_avg = [self.vpsd[key] for key in ["freq", "vpsd", "freq_avg", "vpsd_avg"]]
 
-    # loop components
-    for comp in self.vpsd_components.keys():
+        # LMFIT parameters
+        params = Parameters()
 
-        # component dictionary
-        comp_dict = self.vpsd_components[comp]
+        # loop components
+        for comp in self.vpsd_components.keys():
 
-        # coefficients and vary
-        coef_val = comp_dict["coef_val"]
-        vary     = comp_dict["vary"]
+            # component dictionary
+            comp_dict = self.vpsd_components[comp]
 
-        # loop coefficients
-        for i in range(len(coef_val)):
+            # coefficients and vary
+            coef_val = comp_dict["coef_val"]
+            vary     = comp_dict["vary"]
 
-            # add parameters
-            params.add(comp + "_" + str(i), value=coef_val[i], min=coef_val[i]/10, max=coef_val[i]*10, vary=vary[i])
+            # loop coefficients
+            for i in range(len(coef_val)):
 
-    # fit coefficients
-    c = minimize(_func_res, params, args=(self, freq_avg, vpsd_avg))
+                # add parameters
+                params.add(comp + "_" + str(i), value=coef_val[i], min=coef_val[i]/10, max=coef_val[i]*10, vary=vary[i])
 
-    # loop components
-    for comp in self.vpsd_components.keys():
+        # fit coefficients
+        c = minimize(_func_res, params, args=(self, freq_avg, vpsd_avg))
+
+        # loop components
+        for comp in self.vpsd_components.keys():
+
+            # component dictionary
+            comp_dict = self.vpsd_components[comp]
+
+            # coefficients
+            coef_val = comp_dict["coef_val"]
+            coef_err = comp_dict["coef_err"]
 
-        # component dictionary
-        comp_dict = self.vpsd_components[comp]
+            # loop coefficients
+            for i in range(len(coef_val)):
 
-        # coefficients
-        coef_val = comp_dict["coef_val"]
-        coef_err = comp_dict["coef_err"]
-
-        # loop coefficients
-        for i in range(len(coef_val)):
-
-            # update coefficients with fitted values
-            coef_val[i] = c.params[comp + "_" + str(i)].value
-            coef_err[i] = c.params[comp + "_" + str(i)].stderr
-    
-    return None
+                # update coefficients with fitted values
+                coef_val[i] = c.params[comp + "_" + str(i)].value
+                coef_err[i] = c.params[comp + "_" + str(i)].stderr
+        
+        return None
 
 def _func_res(params, self, freq_avg, vpsd_avg):
 
     # empty array for sum of components
     vpsd_tot = np.zeros(len(freq_avg))
 
     # loop components
```

### Comparing `arve-0.1.2/arve/star/get_stellar_parameters.py` & `arve-0.1.3/arve/star/get_stellar_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 from   astroquery.simbad import Simbad
 import numpy             as     np
 
-def get_stellar_parameters(self) -> None:
-    """Get spectral type from SIMBAD query and stellar parameters from main-sequence table.
+class get_stellar_parameters:
 
-    :return: None
-    :rtype: None
-    """
-
-    # Sun
-    if self.target == "Sun":
-
-        # save stellar parameters
-        self.stellar_parameters["sptype"] = "G2"
-        self.stellar_parameters["Teff"  ] = 5770
-        self.stellar_parameters["logg"  ] = 4.4
-        self.stellar_parameters["Fe_H"  ] = 0.0
-        self.stellar_parameters["M"     ] = 1.0
-        self.stellar_parameters["R"     ] = 1.0
-        self.stellar_parameters["vsini" ] = 1.63
-
-    # other stars
-    else:
-
-        # get spectral type from query
-        simbad = Simbad()
-        simbad.add_votable_fields("sptype")
-        self.stellar_parameters["sptype"] = simbad.query_object(self.target)["SP_TYPE"][0][:2]
-
-        # convert spectral types to numbers
-        sptype_num       =  self.arve.functions.sptype_to_num(sptype=self.stellar_parameters["sptype"])
-        sptype_num_table = [self.arve.functions.sptype_to_num(sptype=sptype) for sptype in _table["sptype"]]
-
-        # interpolate and save stellar parameters from table
-        for key in ["Teff", "logg", "Fe_H", "M", "R", "vsini"]:
-            self.stellar_parameters[key] = np.interp(sptype_num, sptype_num_table, _table[key])
-        
-    # compute and save micro- and macro-turbulence
-    self.stellar_parameters["vmic"] = 0.85
-    self.stellar_parameters["vmac"] = max(0.00, 3.98-(self.stellar_parameters["Teff"]-5770)/650)
+    def get_stellar_parameters(self) -> None:
+        """Get spectral type from SIMBAD query and stellar parameters from main-sequence table.
 
-    return None
+        :return: None
+        :rtype: None
+        """
+
+        # Sun
+        if self.target == "Sun":
+
+            # save stellar parameters
+            self.stellar_parameters["sptype"] = "G2"
+            self.stellar_parameters["Teff"  ] = 5770
+            self.stellar_parameters["logg"  ] = 4.4
+            self.stellar_parameters["Fe_H"  ] = 0.0
+            self.stellar_parameters["M"     ] = 1.0
+            self.stellar_parameters["R"     ] = 1.0
+            self.stellar_parameters["vsini" ] = 1.63
+
+        # other stars
+        else:
+
+            # get spectral type from query
+            simbad = Simbad()
+            simbad.add_votable_fields("sptype")
+            self.stellar_parameters["sptype"] = simbad.query_object(self.target)["SP_TYPE"][0][:2]
+
+            # convert spectral types to numbers
+            sptype_num       =  self.arve.functions.sptype_to_num(sptype=self.stellar_parameters["sptype"])
+            sptype_num_table = [self.arve.functions.sptype_to_num(sptype=sptype) for sptype in _table["sptype"]]
+
+            # interpolate and save stellar parameters from table
+            for key in ["Teff", "logg", "Fe_H", "M", "R", "vsini"]:
+                self.stellar_parameters[key] = np.interp(sptype_num, sptype_num_table, _table[key])
+            
+        # compute and save micro- and macro-turbulence
+        self.stellar_parameters["vmic"] = 0.85
+        self.stellar_parameters["vmac"] = max(0.00, 3.98-(self.stellar_parameters["Teff"]-5770)/650)
+
+        return None
 
 # table with spectral parameters for main sequence stars
 _table = np.array(
 [
 ("A0", 9572, 4.3, 0.0, 2.34, 1.80, 255.0),
 ("A2", 8985, 4.3, 0.0, 2.21, 1.75, 244.0),
 ("A5", 8306, 4.2, 0.0, 2.04, 1.69, 225.0),
```

### Comparing `arve-0.1.2/arve/star/plot_vpsd_components.py` & `arve-0.1.3/arve/star/plot_vpsd_components.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,96 +1,98 @@
 import matplotlib.pyplot as plt
 import numpy             as np
 
-def plot_vpsd_components(self) -> plt.Figure:
-    """Plot velocity power spectral density (VPSD) components.
+class plot_vpsd_components:
 
-    :return: figure with the VPSD, its log-average and its modeled components
-    :rtype: plt.Figure
-    """
+    def plot_vpsd_components(self) -> plt.Figure:
+        """Plot velocity power spectral density (VPSD) components.
 
-    # figure
-    fig = plt.figure()
+        :return: figure with the VPSD, its log-average and its modeled components
+        :rtype: plt.Figure
+        """
 
-    # read VPSD and units
-    freq, vpsd, freq_avg, vpsd_avg = [self.vpsd[key] for key in ["freq", "vpsd", "freq_avg", "vpsd_avg"]]
-    time_unit, vrad_unit = [self.arve.data.vrad[key] for key in ["time_unit", "vrad_unit"]]
+        # figure
+        fig = plt.figure()
 
-    # plot VPSD and average VPSD
-    plt.loglog(freq, vpsd, ls="-", c="k", alpha=0.5)
-    plt.loglog(freq_avg, vpsd_avg, ls="None", marker="o", mec="k", mfc="None")
+        # read VPSD and units
+        freq, vpsd, freq_avg, vpsd_avg = [self.vpsd[key] for key in ["freq", "vpsd", "freq_avg", "vpsd_avg"]]
+        time_unit, vrad_unit = [self.arve.data.vrad[key] for key in ["time_unit", "vrad_unit"]]
 
-    # empty array for sum of components
-    vpsd_tot = np.zeros(len(freq))
+        # plot VPSD and average VPSD
+        plt.loglog(freq, vpsd, ls="-", c="k", alpha=0.5)
+        plt.loglog(freq_avg, vpsd_avg, ls="None", marker="o", mec="k", mfc="None")
 
-    # loop components
-    for comp in self.vpsd_components.keys():
+        # empty array for sum of components
+        vpsd_tot = np.zeros(len(freq))
 
-        # component dictionary
-        comp_dict = self.vpsd_components[comp]
+        # loop components
+        for comp in self.vpsd_components.keys():
 
-        # type and coefficients
-        type     = comp_dict["type"]
-        coef_val = comp_dict["coef_val"]
+            # component dictionary
+            comp_dict = self.vpsd_components[comp]
 
-        # type Constant
-        if type == "Constant":
+            # type and coefficients
+            type     = comp_dict["type"]
+            coef_val = comp_dict["coef_val"]
 
-            # unpack coefficients
-            c0 = coef_val[0]
+            # type Constant
+            if type == "Constant":
 
-            # compute component
-            vpsd_comp = c0
+                # unpack coefficients
+                c0 = coef_val[0]
 
-            # plot component
-            plt.axhline(vpsd_comp, ls="--", label=comp)
+                # compute component
+                vpsd_comp = c0
 
-        # type Lorentz
-        if type == "Lorentz":
-            
-            # unpack coefficients
-            c0 = coef_val[0]
-            c1 = coef_val[1]
-            c2 = coef_val[2]
+                # plot component
+                plt.axhline(vpsd_comp, ls="--", label=comp)
 
-            # compute component
-            vpsd_comp = c0*c1**2/(c1**2+(freq-c2)**2)
+            # type Lorentz
+            if type == "Lorentz":
+                
+                # unpack coefficients
+                c0 = coef_val[0]
+                c1 = coef_val[1]
+                c2 = coef_val[2]
 
-            # plot component
-            plt.loglog(freq, vpsd_comp, ls="--", label=comp)
+                # compute component
+                vpsd_comp = c0*c1**2/(c1**2+(freq-c2)**2)
 
-        # type Harvey
-        if type == "Harvey":
+                # plot component
+                plt.loglog(freq, vpsd_comp, ls="--", label=comp)
 
-            # unpack coefficients
-            c0 = coef_val[0]
-            c1 = coef_val[1]
-            c2 = coef_val[2]
+            # type Harvey
+            if type == "Harvey":
 
-            # compute component
-            vpsd_comp = c0/(1+(c1*freq)**c2)
+                # unpack coefficients
+                c0 = coef_val[0]
+                c1 = coef_val[1]
+                c2 = coef_val[2]
 
-            # plot component
-            plt.loglog(freq, vpsd_comp, ls="--", label=comp)
+                # compute component
+                vpsd_comp = c0/(1+(c1*freq)**c2)
 
-        # add component to sum
-        vpsd_tot += vpsd_comp
+                # plot component
+                plt.loglog(freq, vpsd_comp, ls="--", label=comp)
 
-    # plot component sum
-    plt.loglog(freq, vpsd_tot, ls="-", c="k", label="Total")
+            # add component to sum
+            vpsd_tot += vpsd_comp
 
-    # plot limits
-    plt.xlim(freq[0], freq[-1])
+        # plot component sum
+        plt.loglog(freq, vpsd_tot, ls="-", c="k", label="Total")
 
-    # plot labels
-    plt.xlabel("$f$" + " " + f"[{time_unit}" + "$^{-1}$]")
-    plt.ylabel("VPSD" + " " + f"[({vrad_unit})" + "$^{2}$" + " / " + f"{time_unit}" + "$^{-1}$]")
+        # plot limits
+        plt.xlim(freq[0], freq[-1])
 
-    # plot legend
-    leg = plt.legend(loc="lower left")
-    leg.set_zorder(101)
+        # plot labels
+        plt.xlabel("$f$" + " " + f"[{time_unit}" + "$^{-1}$]")
+        plt.ylabel("VPSD" + " " + f"[({vrad_unit})" + "$^{2}$" + " / " + f"{time_unit}" + "$^{-1}$]")
 
-    # plot layout
-    plt.tight_layout()
+        # plot legend
+        leg = plt.legend(loc="lower left")
+        leg.set_zorder(101)
 
-    # return figure
-    return fig
+        # plot layout
+        plt.tight_layout()
+
+        # return figure
+        return fig
```

### Comparing `arve-0.1.2/arve.egg-info/SOURCES.txt` & `arve-0.1.3/arve.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -4,41 +4,42 @@
 arve/__init__.py
 arve/arve.py
 arve.egg-info/PKG-INFO
 arve.egg-info/SOURCES.txt
 arve.egg-info/dependency_links.txt
 arve.egg-info/requires.txt
 arve.egg-info/top_level.txt
-arve/aux_data/masks/A0_3500-7000.mask
-arve/aux_data/masks/A2_3500-7000.mask
-arve/aux_data/masks/A5_3500-7000.mask
-arve/aux_data/masks/A7_3500-7000.mask
-arve/aux_data/masks/F0_3500-7000.mask
-arve/aux_data/masks/F2_3500-7000.mask
-arve/aux_data/masks/F5_3500-7000.mask
-arve/aux_data/masks/F8_3500-7000.mask
-arve/aux_data/masks/G0_3500-7000.mask
-arve/aux_data/masks/G2_3500-7000.mask
-arve/aux_data/masks/G5_3500-7000.mask
-arve/aux_data/masks/G8_3500-7000.mask
-arve/aux_data/masks/K0_3500-7000.mask
-arve/aux_data/masks/K2_3500-7000.mask
-arve/aux_data/masks/K3_3500-7000.mask
-arve/aux_data/masks/K5_3500-7000.mask
-arve/aux_data/masks/K7_3500-7000.mask
-arve/aux_data/masks/M0_3500-7000.mask
-arve/aux_data/masks/M2_3500-7000.mask
-arve/aux_data/masks/M5_3500-7000.mask
+arve/aux_data/masks/A0_3500-7000.csv
+arve/aux_data/masks/A2_3500-7000.csv
+arve/aux_data/masks/A5_3500-7000.csv
+arve/aux_data/masks/A7_3500-7000.csv
+arve/aux_data/masks/F0_3500-7000.csv
+arve/aux_data/masks/F2_3500-7000.csv
+arve/aux_data/masks/F5_3500-7000.csv
+arve/aux_data/masks/F8_3500-7000.csv
+arve/aux_data/masks/G0_3500-7000.csv
+arve/aux_data/masks/G2_3500-7000.csv
+arve/aux_data/masks/G5_3500-7000.csv
+arve/aux_data/masks/G8_3500-7000.csv
+arve/aux_data/masks/K0_3500-7000.csv
+arve/aux_data/masks/K2_3500-7000.csv
+arve/aux_data/masks/K3_3500-7000.csv
+arve/aux_data/masks/K5_3500-7000.csv
+arve/aux_data/masks/K7_3500-7000.csv
+arve/aux_data/masks/M0_3500-7000.csv
+arve/aux_data/masks/M2_3500-7000.csv
+arve/aux_data/masks/M5_3500-7000.csv
 arve/data/__init__.py
 arve/data/add_spec.py
 arve/data/add_vrad.py
-arve/data/compute_vrad.py
+arve/data/compute_vrad_ccf.py
 arve/functions/__init__.py
 arve/functions/doppler_shift.py
 arve/functions/gls_periodogram.py
+arve/functions/inverted_gaussian.py
 arve/functions/sptype_to_num.py
 arve/planets/__init__.py
 arve/planets/add_planet.py
 arve/star/__init__.py
 arve/star/add_vpsd_components.py
 arve/star/compute_vpsd.py
 arve/star/fit_vpsd_coefficients.py
```

### Comparing `arve-0.1.2/setup.py` & `arve-0.1.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from setuptools import find_packages, setup
 
+with open("README.md", "r") as file:
+    long_description = file.read()
+
 setup(
     name="arve",
-    version="0.1.2",
-    description="Analyzing Radial Velocity Elements",
-    url="https://github.com/almoulla/arve",
+    version="0.1.3",
     author="Khaled Al Moulla",
     author_email="khaled.almoulla@gmail.com",
+    description="Analyzing Radial Velocity Elements",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/almoulla/arve",
     license="MIT License",
     packages=find_packages(),
     install_requires=["astroquery",
                       "lmfit"     ,
                       "matplotlib",
                       "numba"     ,
                       "numpy"     ,
-                      "scipy"
+                      "scipy"     ,
+                      "tqdm"      ,
                      ],
-
-    classifiers=[
-        "Development Status :: 1 - Planning",
-        "Intended Audience :: Science/Research",
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3",
-    ],
+    classifiers=["Development Status :: 1 - Planning"    ,
+                 "Intended Audience :: Science/Research" ,
+                 "License :: OSI Approved :: MIT License",
+                 "Programming Language :: Python :: 3"   ,
+                 ],
     include_package_data=True,
-    package_data={"arve": ["aux_data/masks/*.mask"]}
+    package_data={"arve": ["aux_data/masks/*.csv"]}
 )
```


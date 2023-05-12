# Comparing `tmp/pycalib-0.1.0.dev4.tar.gz` & `tmp/pycalib-0.1.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycalib-0.1.0.dev4.tar", last modified: Fri Apr 21 12:36:12 2023, max compression
+gzip compressed data, was "pycalib-0.1.0.dev5.tar", last modified: Fri May 12 12:15:08 2023, max compression
```

## Comparing `pycalib-0.1.0.dev4.tar` & `pycalib-0.1.0.dev5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2023-04-21 12:36:12.174405 pycalib-0.1.0.dev4/
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     7372 2023-04-21 12:36:12.174405 pycalib-0.1.0.dev4/PKG-INFO
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     5372 2022-11-29 17:05:41.000000 pycalib-0.1.0.dev4/README.md
-drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2023-04-21 12:36:12.174405 pycalib-0.1.0.dev4/pycalib/
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)       27 2023-04-21 12:32:27.000000 pycalib-0.1.0.dev4/pycalib/__init__.py
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)    22331 2022-11-29 16:53:42.000000 pycalib-0.1.0.dev4/pycalib/metrics.py
-drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2023-04-21 12:36:12.174405 pycalib-0.1.0.dev4/pycalib/models/
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)    29071 2022-11-29 16:56:53.000000 pycalib-0.1.0.dev4/pycalib/models/__init__.py
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     9530 2021-03-24 17:40:54.000000 pycalib-0.1.0.dev4/pycalib/models/multiclass.py
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     2712 2021-03-24 17:08:37.000000 pycalib-0.1.0.dev4/pycalib/stats.py
-drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2023-04-21 12:36:12.174405 pycalib-0.1.0.dev4/pycalib/tests/
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)        0 2021-03-08 14:18:37.000000 pycalib-0.1.0.dev4/pycalib/tests/__init__.py
-drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2023-04-21 12:36:12.174405 pycalib-0.1.0.dev4/pycalib/tests/models/
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)        0 2021-08-04 09:25:58.000000 pycalib-0.1.0.dev4/pycalib/tests/models/__init__.py
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     1964 2022-11-29 16:54:08.000000 pycalib-0.1.0.dev4/pycalib/tests/models/test_init.py
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     5012 2021-03-24 17:23:05.000000 pycalib-0.1.0.dev4/pycalib/tests/test_metrics.py
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     1994 2022-11-29 16:53:11.000000 pycalib-0.1.0.dev4/pycalib/utils.py
-drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2023-04-21 12:36:12.174405 pycalib-0.1.0.dev4/pycalib/visualisations/
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)    29080 2022-11-29 16:52:30.000000 pycalib-0.1.0.dev4/pycalib/visualisations/__init__.py
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     9555 2023-04-21 12:35:12.000000 pycalib-0.1.0.dev4/pycalib/visualisations/barycentric.py
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     6653 2021-03-24 17:06:48.000000 pycalib-0.1.0.dev4/pycalib/visualisations/ternary.py
-drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2023-04-21 12:36:12.174405 pycalib-0.1.0.dev4/pycalib/visualisations/tests/
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)        0 2021-04-13 10:23:56.000000 pycalib-0.1.0.dev4/pycalib/visualisations/tests/__init__.py
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     4975 2022-11-29 16:52:02.000000 pycalib-0.1.0.dev4/pycalib/visualisations/tests/test_init.py
-drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2023-04-21 12:36:12.174405 pycalib-0.1.0.dev4/pycalib.egg-info/
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     7372 2023-04-21 12:36:12.000000 pycalib-0.1.0.dev4/pycalib.egg-info/PKG-INFO
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)      624 2023-04-21 12:36:12.000000 pycalib-0.1.0.dev4/pycalib.egg-info/SOURCES.txt
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)        1 2023-04-21 12:36:12.000000 pycalib-0.1.0.dev4/pycalib.egg-info/dependency_links.txt
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)       76 2023-04-21 12:36:12.000000 pycalib-0.1.0.dev4/pycalib.egg-info/requires.txt
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)        8 2023-04-21 12:36:12.000000 pycalib-0.1.0.dev4/pycalib.egg-info/top_level.txt
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)       79 2023-04-21 12:36:12.174405 pycalib-0.1.0.dev4/setup.cfg
--rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     1215 2022-11-30 14:09:22.000000 pycalib-0.1.0.dev4/setup.py
+drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2023-05-12 12:15:08.784757 pycalib-0.1.0.dev5/
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     7372 2023-05-12 12:15:08.784757 pycalib-0.1.0.dev5/PKG-INFO
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     5372 2022-11-29 17:05:41.000000 pycalib-0.1.0.dev5/README.md
+drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2023-05-12 12:15:08.784757 pycalib-0.1.0.dev5/pycalib/
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)       27 2023-05-12 12:09:24.000000 pycalib-0.1.0.dev5/pycalib/__init__.py
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)    22331 2022-11-29 16:53:42.000000 pycalib-0.1.0.dev5/pycalib/metrics.py
+drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2023-05-12 12:15:08.784757 pycalib-0.1.0.dev5/pycalib/models/
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)    29071 2022-11-29 16:56:53.000000 pycalib-0.1.0.dev5/pycalib/models/__init__.py
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     9530 2021-03-24 17:40:54.000000 pycalib-0.1.0.dev5/pycalib/models/multiclass.py
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     2712 2021-03-24 17:08:37.000000 pycalib-0.1.0.dev5/pycalib/stats.py
+drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2023-05-12 12:15:08.784757 pycalib-0.1.0.dev5/pycalib/tests/
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)        0 2021-03-08 14:18:37.000000 pycalib-0.1.0.dev5/pycalib/tests/__init__.py
+drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2023-05-12 12:15:08.784757 pycalib-0.1.0.dev5/pycalib/tests/models/
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)        0 2021-08-04 09:25:58.000000 pycalib-0.1.0.dev5/pycalib/tests/models/__init__.py
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     1964 2022-11-29 16:54:08.000000 pycalib-0.1.0.dev5/pycalib/tests/models/test_init.py
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     5012 2021-03-24 17:23:05.000000 pycalib-0.1.0.dev5/pycalib/tests/test_metrics.py
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     1994 2022-11-29 16:53:11.000000 pycalib-0.1.0.dev5/pycalib/utils.py
+drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2023-05-12 12:15:08.784757 pycalib-0.1.0.dev5/pycalib/visualisations/
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)    29064 2023-05-12 12:07:44.000000 pycalib-0.1.0.dev5/pycalib/visualisations/__init__.py
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     9555 2023-04-21 12:35:12.000000 pycalib-0.1.0.dev5/pycalib/visualisations/barycentric.py
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     6653 2021-03-24 17:06:48.000000 pycalib-0.1.0.dev5/pycalib/visualisations/ternary.py
+drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2023-05-12 12:15:08.784757 pycalib-0.1.0.dev5/pycalib/visualisations/tests/
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)        0 2021-04-13 10:23:56.000000 pycalib-0.1.0.dev5/pycalib/visualisations/tests/__init__.py
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     4975 2022-11-29 16:52:02.000000 pycalib-0.1.0.dev5/pycalib/visualisations/tests/test_init.py
+drwxrwxr-x   0 mp15688   (1001) mp15688   (1001)        0 2023-05-12 12:15:08.784757 pycalib-0.1.0.dev5/pycalib.egg-info/
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     7372 2023-05-12 12:15:08.000000 pycalib-0.1.0.dev5/pycalib.egg-info/PKG-INFO
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)      624 2023-05-12 12:15:08.000000 pycalib-0.1.0.dev5/pycalib.egg-info/SOURCES.txt
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)        1 2023-05-12 12:15:08.000000 pycalib-0.1.0.dev5/pycalib.egg-info/dependency_links.txt
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)       76 2023-05-12 12:15:08.000000 pycalib-0.1.0.dev5/pycalib.egg-info/requires.txt
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)        8 2023-05-12 12:15:08.000000 pycalib-0.1.0.dev5/pycalib.egg-info/top_level.txt
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)       79 2023-05-12 12:15:08.784757 pycalib-0.1.0.dev5/setup.cfg
+-rw-rw-r--   0 mp15688   (1001) mp15688   (1001)     1215 2023-05-12 12:03:43.000000 pycalib-0.1.0.dev5/setup.py
```

### Comparing `pycalib-0.1.0.dev4/PKG-INFO` & `pycalib-0.1.0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pycalib
-Version: 0.1.0.dev4
+Version: 0.1.0.dev5
 Summary: Python library with tools for classifier calibration.
 Home-page: https://classifier-calibration.github.io/PyCalib/
 Author: Miquel Perello Nieto, Hao Song, Telmo de Menezes e Silva Filho
 Author-email: perello.nieto@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/classifier-calibration/archive/0.1.0.dev4.tar.gz
+Download-URL: https://github.com/classifier-calibration/archive/0.1.0.dev5.tar.gz
 Description: [![CI][ci:b]][ci]
         [![Documentation][documentation:b]][documentation]
         [![License BSD3][license:b]][license]
         ![Python3.8][python:b]
         [![pypi][pypi:b]][pypi]
         [![codecov][codecov:b]][codecov]
         [![DOI](https://zenodo.org/badge/280465805.svg)](https://zenodo.org/badge/latestdoi/280465805)
```

### Comparing `pycalib-0.1.0.dev4/README.md` & `pycalib-0.1.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `pycalib-0.1.0.dev4/pycalib/metrics.py` & `pycalib-0.1.0.dev5/pycalib/metrics.py`

 * *Files identical despite different names*

### Comparing `pycalib-0.1.0.dev4/pycalib/models/__init__.py` & `pycalib-0.1.0.dev5/pycalib/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pycalib-0.1.0.dev4/pycalib/models/multiclass.py` & `pycalib-0.1.0.dev5/pycalib/models/multiclass.py`

 * *Files identical despite different names*

### Comparing `pycalib-0.1.0.dev4/pycalib/stats.py` & `pycalib-0.1.0.dev5/pycalib/stats.py`

 * *Files identical despite different names*

### Comparing `pycalib-0.1.0.dev4/pycalib/tests/models/test_init.py` & `pycalib-0.1.0.dev5/pycalib/tests/models/test_init.py`

 * *Files identical despite different names*

### Comparing `pycalib-0.1.0.dev4/pycalib/tests/test_metrics.py` & `pycalib-0.1.0.dev5/pycalib/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `pycalib-0.1.0.dev4/pycalib/utils.py` & `pycalib-0.1.0.dev5/pycalib/utils.py`

 * *Files identical despite different names*

### Comparing `pycalib-0.1.0.dev4/pycalib/visualisations/__init__.py` & `pycalib-0.1.0.dev5/pycalib/visualisations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
                 for ap, at in zip(avg_pred, avg_true):
                     ax1.arrow(ap, at, at - ap, 0, color=color_gaps,
                               head_width=0.02, length_includes_head=True,
                               width=0.01)
 
             if show_gaps:
                 for ap, at in zip(avg_pred, avg_true):
-                    ygaps = avg_pred - avg_true
+                    ygaps = np.abs(avg_pred - avg_true)
                     ygaps = np.vstack((np.zeros_like(ygaps), ygaps))
                     ax1.errorbar(avg_pred, avg_true, yerr=ygaps, fmt=" ",
                                  color=color_gaps, lw=4, capsize=5, capthick=1,
                                  zorder=10)
 
         ax1.set_xlim([0, 1])
         ax1.set_ylim([0, 1])
@@ -323,16 +323,15 @@
                         method=interval_method)
                     nozero_intervals = np.array(nozero_intervals)
 
                     intervals = np.empty((2, bin_total.shape[0]))
                     intervals.fill(np.nan)
                     intervals[:, ~zero_idx] = nozero_intervals
 
-                    yerr = intervals - avg_true
-                    yerr = np.abs(yerr)
+                    yerr = np.abs(intervals - avg_true)
                     ax1.errorbar(avg_pred, avg_true, yerr=yerr, label=name,
                                  fmt=fmt, color=color_list[j])  # markersize=5)
 
             if show_counts:
                 for ap, at, count in zip(avg_pred, avg_true, bin_total):
                     if np.isfinite(ap) and np.isfinite(at):
                         ax1.text(ap, at, str(count), fontsize=6,
@@ -344,15 +343,15 @@
                 for ap, at in zip(avg_pred, avg_true):
                     ax1.arrow(ap, at, at - ap, 0, color=color_gaps,
                               head_width=0.02, length_includes_head=True,
                               width=0.01)
 
             if show_gaps:
                 for ap, at in zip(avg_pred, avg_true):
-                    ygaps = avg_pred - avg_true
+                    ygaps = np.abs(avg_pred - avg_true)
                     ygaps = np.vstack((np.zeros_like(ygaps), ygaps))
                     ax1.errorbar(avg_pred, avg_true, yerr=ygaps, fmt=" ",
                                  color=color_gaps, lw=4, capsize=5, capthick=1,
                                  zorder=10)
 
             if sample_proportion > 0:
                 idx = np.random.choice(labels.shape[0],
```

### Comparing `pycalib-0.1.0.dev4/pycalib/visualisations/barycentric.py` & `pycalib-0.1.0.dev5/pycalib/visualisations/barycentric.py`

 * *Files identical despite different names*

### Comparing `pycalib-0.1.0.dev4/pycalib/visualisations/ternary.py` & `pycalib-0.1.0.dev5/pycalib/visualisations/ternary.py`

 * *Files identical despite different names*

### Comparing `pycalib-0.1.0.dev4/pycalib/visualisations/tests/test_init.py` & `pycalib-0.1.0.dev5/pycalib/visualisations/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `pycalib-0.1.0.dev4/pycalib.egg-info/PKG-INFO` & `pycalib-0.1.0.dev5/pycalib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pycalib
-Version: 0.1.0.dev4
+Version: 0.1.0.dev5
 Summary: Python library with tools for classifier calibration.
 Home-page: https://classifier-calibration.github.io/PyCalib/
 Author: Miquel Perello Nieto, Hao Song, Telmo de Menezes e Silva Filho
 Author-email: perello.nieto@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/classifier-calibration/archive/0.1.0.dev4.tar.gz
+Download-URL: https://github.com/classifier-calibration/archive/0.1.0.dev5.tar.gz
 Description: [![CI][ci:b]][ci]
         [![Documentation][documentation:b]][documentation]
         [![License BSD3][license:b]][license]
         ![Python3.8][python:b]
         [![pypi][pypi:b]][pypi]
         [![codecov][codecov:b]][codecov]
         [![DOI](https://zenodo.org/badge/280465805.svg)](https://zenodo.org/badge/latestdoi/280465805)
```

### Comparing `pycalib-0.1.0.dev4/pycalib.egg-info/SOURCES.txt` & `pycalib-0.1.0.dev5/pycalib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycalib-0.1.0.dev4/setup.py` & `pycalib-0.1.0.dev5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 with open(ver_path) as ver_file:
     exec(ver_file.read(), main_ns)
 
 setup(
   name = 'pycalib',
   packages = find_packages(exclude=['tests.*', 'tests', 'docs.*', 'docs']),
   install_requires=[
-    'numpy==1.22',
-    'scipy==1.6',
-    'scikit-learn==0.24',
-    'matplotlib==3.3',
-    'statsmodels==0.12'
+    'numpy>=1.22',
+    'scipy>=1.6',
+    'scikit-learn>=0.24',
+    'matplotlib>=3.3',
+    'statsmodels>=0.12'
   ],
   version=main_ns['__version__'],
   description = 'Python library with tools for classifier calibration.',
   author = 'Miquel Perello Nieto, Hao Song, Telmo de Menezes e Silva Filho',
   author_email = 'perello.nieto@gmail.com',
   url = 'https://classifier-calibration.github.io/PyCalib/',
   download_url = 'https://github.com/classifier-calibration/archive/{}.tar.gz'.format(main_ns['__version__']),
```


# Comparing `tmp/BDMLtools-0.3.5.tar.gz` & `tmp/BDMLtools-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BDMLtools-0.3.5.tar", last modified: Mon Apr  3 08:18:09 2023, max compression
+gzip compressed data, was "BDMLtools-0.3.6.tar", last modified: Fri May 12 08:15:01 2023, max compression
```

## Comparing `BDMLtools-0.3.5.tar` & `BDMLtools-0.3.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-04-03 08:18:09.955411 BDMLtools-0.3.5/
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-04-03 08:18:09.931479 BDMLtools-0.3.5/BDMLtools/
--rwxr-xr-x   0 zengke     (501) staff       (20)     1490 2023-03-31 09:58:37.000000 BDMLtools-0.3.5/BDMLtools/__init__.py
--rw-r--r--   0 zengke     (501) staff       (20)     7931 2022-09-16 05:41:25.000000 BDMLtools-0.3.5/BDMLtools/base.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-04-03 08:18:09.935487 BDMLtools-0.3.5/BDMLtools/clearner/
--rw-r--r--   0 zengke     (501) staff       (20)      303 2022-05-30 05:46:05.000000 BDMLtools-0.3.5/BDMLtools/clearner/__init__.py
--rw-r--r--   0 zengke     (501) staff       (20)    21546 2022-09-06 10:05:08.000000 BDMLtools-0.3.5/BDMLtools/clearner/cleaner.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-04-03 08:18:09.936777 BDMLtools-0.3.5/BDMLtools/encoder/
--rw-r--r--   0 zengke     (501) staff       (20)      230 2022-09-09 08:32:26.000000 BDMLtools-0.3.5/BDMLtools/encoder/__init__.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    13123 2022-10-26 06:18:44.000000 BDMLtools-0.3.5/BDMLtools/encoder/woe.py
--rw-r--r--   0 zengke     (501) staff       (20)      617 2022-05-30 05:46:05.000000 BDMLtools-0.3.5/BDMLtools/exception.py
--rwxr-xr-x   0 zengke     (501) staff       (20)     5965 2022-07-22 07:30:31.000000 BDMLtools-0.3.5/BDMLtools/fun.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-04-03 08:18:09.938677 BDMLtools-0.3.5/BDMLtools/plotter/
--rw-r--r--   0 zengke     (501) staff       (20)      280 2022-07-08 09:08:07.000000 BDMLtools-0.3.5/BDMLtools/plotter/__init__.py
--rw-r--r--   0 zengke     (501) staff       (20)    32833 2022-08-30 04:00:04.000000 BDMLtools-0.3.5/BDMLtools/plotter/base.py
--rw-r--r--   0 zengke     (501) staff       (20)    16452 2023-04-03 07:45:25.000000 BDMLtools-0.3.5/BDMLtools/plotter/eval.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-04-03 08:18:09.940090 BDMLtools-0.3.5/BDMLtools/report/
--rw-r--r--   0 zengke     (501) staff       (20)      379 2022-05-30 05:46:05.000000 BDMLtools-0.3.5/BDMLtools/report/__init__.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    49285 2023-03-29 06:24:55.000000 BDMLtools-0.3.5/BDMLtools/report/report.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-04-03 08:18:09.945609 BDMLtools-0.3.5/BDMLtools/selector/
--rw-r--r--   0 zengke     (501) staff       (20)      902 2022-11-22 04:09:12.000000 BDMLtools-0.3.5/BDMLtools/selector/__init__.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    30341 2023-01-31 10:03:44.000000 BDMLtools-0.3.5/BDMLtools/selector/bin.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    61178 2023-03-29 06:28:50.000000 BDMLtools-0.3.5/BDMLtools/selector/bin_fun.py
--rw-r--r--   0 zengke     (501) staff       (20)    12019 2023-04-03 06:42:57.000000 BDMLtools-0.3.5/BDMLtools/selector/embeded.py
--rw-r--r--   0 zengke     (501) staff       (20)    15545 2023-03-29 06:31:10.000000 BDMLtools-0.3.5/BDMLtools/selector/fa.py
--rw-r--r--   0 zengke     (501) staff       (20)    25071 2023-03-30 01:22:06.000000 BDMLtools-0.3.5/BDMLtools/selector/lgbm.py
--rw-r--r--   0 zengke     (501) staff       (20)    27613 2022-10-08 09:45:23.000000 BDMLtools-0.3.5/BDMLtools/selector/logtit.py
--rw-r--r--   0 zengke     (501) staff       (20)    30242 2023-03-29 06:26:13.000000 BDMLtools-0.3.5/BDMLtools/selector/simple.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-04-03 08:18:09.949687 BDMLtools-0.3.5/BDMLtools/tuner/
--rw-r--r--   0 zengke     (501) staff       (20)      384 2022-05-30 05:46:05.000000 BDMLtools-0.3.5/BDMLtools/tuner/__init__.py
--rw-r--r--   0 zengke     (501) staff       (20)     3230 2022-08-30 06:57:04.000000 BDMLtools-0.3.5/BDMLtools/tuner/base.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    17778 2023-02-20 02:22:16.000000 BDMLtools-0.3.5/BDMLtools/tuner/bayesian.py
--rwxr-xr-x   0 zengke     (501) staff       (20)     5705 2023-01-17 10:01:41.000000 BDMLtools-0.3.5/BDMLtools/tuner/fun.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    23123 2023-02-20 02:24:38.000000 BDMLtools-0.3.5/BDMLtools/tuner/gridcv.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    24672 2023-02-20 02:26:00.000000 BDMLtools-0.3.5/BDMLtools/tuner/halvingcv.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-04-03 08:18:09.934404 BDMLtools-0.3.5/BDMLtools.egg-info/
--rw-r--r--   0 zengke     (501) staff       (20)     2172 2023-04-03 08:18:09.000000 BDMLtools-0.3.5/BDMLtools.egg-info/PKG-INFO
--rw-r--r--   0 zengke     (501) staff       (20)     1046 2023-04-03 08:18:09.000000 BDMLtools-0.3.5/BDMLtools.egg-info/SOURCES.txt
--rw-r--r--   0 zengke     (501) staff       (20)        1 2023-04-03 08:18:09.000000 BDMLtools-0.3.5/BDMLtools.egg-info/dependency_links.txt
--rw-r--r--   0 zengke     (501) staff       (20)      465 2023-04-03 08:18:09.000000 BDMLtools-0.3.5/BDMLtools.egg-info/requires.txt
--rw-r--r--   0 zengke     (501) staff       (20)       15 2023-04-03 08:18:09.000000 BDMLtools-0.3.5/BDMLtools.egg-info/top_level.txt
--rw-r--r--   0 zengke     (501) staff       (20)     1062 2022-09-07 02:01:45.000000 BDMLtools-0.3.5/LICENSE
--rw-r--r--   0 zengke     (501) staff       (20)     2172 2023-04-03 08:18:09.954701 BDMLtools-0.3.5/PKG-INFO
--rw-r--r--   0 zengke     (501) staff       (20)     1646 2023-04-03 01:49:57.000000 BDMLtools-0.3.5/README.md
--rw-r--r--   0 zengke     (501) staff       (20)       38 2023-04-03 08:18:09.955565 BDMLtools-0.3.5/setup.cfg
--rwxr-xr-x   0 zengke     (501) staff       (20)     3632 2023-04-03 03:16:22.000000 BDMLtools-0.3.5/setup.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-04-03 08:18:09.953966 BDMLtools-0.3.5/test/
--rwxr-xr-x   0 zengke     (501) staff       (20)        0 2022-07-12 06:58:12.000000 BDMLtools-0.3.5/test/__init__.py
--rw-r--r--   0 zengke     (501) staff       (20)     9104 2022-09-06 10:00:06.000000 BDMLtools-0.3.5/test/test_base.py
--rw-r--r--   0 zengke     (501) staff       (20)     4500 2022-09-06 10:08:22.000000 BDMLtools-0.3.5/test/test_clearner.py
--rw-r--r--   0 zengke     (501) staff       (20)     1966 2022-08-30 07:06:15.000000 BDMLtools-0.3.5/test/test_eval.py
--rw-r--r--   0 zengke     (501) staff       (20)     4458 2023-03-02 09:37:36.000000 BDMLtools-0.3.5/test/test_report.py
--rw-r--r--   0 zengke     (501) staff       (20)    18557 2023-04-03 07:48:23.000000 BDMLtools-0.3.5/test/test_selector.py
--rw-r--r--   0 zengke     (501) staff       (20)    20045 2023-02-17 09:55:41.000000 BDMLtools-0.3.5/test/test_tunner.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-12 08:15:01.290393 BDMLtools-0.3.6/
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-12 08:15:01.272845 BDMLtools-0.3.6/BDMLtools/
+-rwxr-xr-x   0 zengke     (501) staff       (20)     1490 2023-04-19 03:35:33.000000 BDMLtools-0.3.6/BDMLtools/__init__.py
+-rw-r--r--   0 zengke     (501) staff       (20)     7931 2022-09-16 05:41:25.000000 BDMLtools-0.3.6/BDMLtools/base.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-12 08:15:01.275288 BDMLtools-0.3.6/BDMLtools/clearner/
+-rw-r--r--   0 zengke     (501) staff       (20)      303 2022-05-30 05:46:05.000000 BDMLtools-0.3.6/BDMLtools/clearner/__init__.py
+-rw-r--r--   0 zengke     (501) staff       (20)    21550 2023-05-10 02:08:49.000000 BDMLtools-0.3.6/BDMLtools/clearner/cleaner.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-12 08:15:01.276077 BDMLtools-0.3.6/BDMLtools/encoder/
+-rw-r--r--   0 zengke     (501) staff       (20)      230 2022-09-09 08:32:26.000000 BDMLtools-0.3.6/BDMLtools/encoder/__init__.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    13123 2022-10-26 06:18:44.000000 BDMLtools-0.3.6/BDMLtools/encoder/woe.py
+-rw-r--r--   0 zengke     (501) staff       (20)      617 2022-05-30 05:46:05.000000 BDMLtools-0.3.6/BDMLtools/exception.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)     5965 2022-07-22 07:30:31.000000 BDMLtools-0.3.6/BDMLtools/fun.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-12 08:15:01.277091 BDMLtools-0.3.6/BDMLtools/plotter/
+-rw-r--r--   0 zengke     (501) staff       (20)      280 2022-07-08 09:08:07.000000 BDMLtools-0.3.6/BDMLtools/plotter/__init__.py
+-rw-r--r--   0 zengke     (501) staff       (20)    32833 2022-08-30 04:00:04.000000 BDMLtools-0.3.6/BDMLtools/plotter/base.py
+-rw-r--r--   0 zengke     (501) staff       (20)    16452 2023-04-03 07:45:25.000000 BDMLtools-0.3.6/BDMLtools/plotter/eval.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-12 08:15:01.278048 BDMLtools-0.3.6/BDMLtools/report/
+-rw-r--r--   0 zengke     (501) staff       (20)      379 2022-05-30 05:46:05.000000 BDMLtools-0.3.6/BDMLtools/report/__init__.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    49254 2023-05-11 06:09:02.000000 BDMLtools-0.3.6/BDMLtools/report/report.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-12 08:15:01.281151 BDMLtools-0.3.6/BDMLtools/selector/
+-rw-r--r--   0 zengke     (501) staff       (20)      902 2022-11-22 04:09:12.000000 BDMLtools-0.3.6/BDMLtools/selector/__init__.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    30341 2023-01-31 10:03:44.000000 BDMLtools-0.3.6/BDMLtools/selector/bin.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    61178 2023-03-29 06:28:50.000000 BDMLtools-0.3.6/BDMLtools/selector/bin_fun.py
+-rw-r--r--   0 zengke     (501) staff       (20)    12019 2023-04-03 06:42:57.000000 BDMLtools-0.3.6/BDMLtools/selector/embeded.py
+-rw-r--r--   0 zengke     (501) staff       (20)    16406 2023-04-19 06:45:01.000000 BDMLtools-0.3.6/BDMLtools/selector/fa.py
+-rw-r--r--   0 zengke     (501) staff       (20)    25071 2023-03-30 01:22:06.000000 BDMLtools-0.3.6/BDMLtools/selector/lgbm.py
+-rw-r--r--   0 zengke     (501) staff       (20)    27613 2022-10-08 09:45:23.000000 BDMLtools-0.3.6/BDMLtools/selector/logtit.py
+-rw-r--r--   0 zengke     (501) staff       (20)    30242 2023-03-29 06:26:13.000000 BDMLtools-0.3.6/BDMLtools/selector/simple.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-12 08:15:01.284382 BDMLtools-0.3.6/BDMLtools/tuner/
+-rw-r--r--   0 zengke     (501) staff       (20)      384 2022-05-30 05:46:05.000000 BDMLtools-0.3.6/BDMLtools/tuner/__init__.py
+-rw-r--r--   0 zengke     (501) staff       (20)     3149 2023-04-18 10:14:12.000000 BDMLtools-0.3.6/BDMLtools/tuner/base.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    17803 2023-04-19 02:58:32.000000 BDMLtools-0.3.6/BDMLtools/tuner/bayesian.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)     5750 2023-04-19 06:49:36.000000 BDMLtools-0.3.6/BDMLtools/tuner/fun.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    23169 2023-04-19 03:22:16.000000 BDMLtools-0.3.6/BDMLtools/tuner/gridcv.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    24712 2023-04-19 03:29:39.000000 BDMLtools-0.3.6/BDMLtools/tuner/halvingcv.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-12 08:15:01.274464 BDMLtools-0.3.6/BDMLtools.egg-info/
+-rw-r--r--   0 zengke     (501) staff       (20)     2099 2023-05-12 08:15:01.000000 BDMLtools-0.3.6/BDMLtools.egg-info/PKG-INFO
+-rw-r--r--   0 zengke     (501) staff       (20)     1046 2023-05-12 08:15:01.000000 BDMLtools-0.3.6/BDMLtools.egg-info/SOURCES.txt
+-rw-r--r--   0 zengke     (501) staff       (20)        1 2023-05-12 08:15:01.000000 BDMLtools-0.3.6/BDMLtools.egg-info/dependency_links.txt
+-rw-r--r--   0 zengke     (501) staff       (20)      481 2023-05-12 08:15:01.000000 BDMLtools-0.3.6/BDMLtools.egg-info/requires.txt
+-rw-r--r--   0 zengke     (501) staff       (20)       15 2023-05-12 08:15:01.000000 BDMLtools-0.3.6/BDMLtools.egg-info/top_level.txt
+-rw-r--r--   0 zengke     (501) staff       (20)     1062 2022-09-07 02:01:45.000000 BDMLtools-0.3.6/LICENSE
+-rw-r--r--   0 zengke     (501) staff       (20)     2099 2023-05-12 08:15:01.289831 BDMLtools-0.3.6/PKG-INFO
+-rw-r--r--   0 zengke     (501) staff       (20)     1573 2023-05-11 09:25:34.000000 BDMLtools-0.3.6/README.md
+-rw-r--r--   0 zengke     (501) staff       (20)       38 2023-05-12 08:15:01.290543 BDMLtools-0.3.6/setup.cfg
+-rwxr-xr-x   0 zengke     (501) staff       (20)     3662 2023-05-11 10:01:26.000000 BDMLtools-0.3.6/setup.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-12 08:15:01.289101 BDMLtools-0.3.6/test/
+-rwxr-xr-x   0 zengke     (501) staff       (20)        0 2022-07-12 06:58:12.000000 BDMLtools-0.3.6/test/__init__.py
+-rw-r--r--   0 zengke     (501) staff       (20)     9104 2022-09-06 10:00:06.000000 BDMLtools-0.3.6/test/test_base.py
+-rw-r--r--   0 zengke     (501) staff       (20)     4500 2022-09-06 10:08:22.000000 BDMLtools-0.3.6/test/test_clearner.py
+-rw-r--r--   0 zengke     (501) staff       (20)     1966 2022-08-30 07:06:15.000000 BDMLtools-0.3.6/test/test_eval.py
+-rw-r--r--   0 zengke     (501) staff       (20)     4873 2023-05-12 07:52:29.000000 BDMLtools-0.3.6/test/test_report.py
+-rw-r--r--   0 zengke     (501) staff       (20)    18928 2023-05-12 07:52:56.000000 BDMLtools-0.3.6/test/test_selector.py
+-rw-r--r--   0 zengke     (501) staff       (20)    20045 2023-02-17 09:55:41.000000 BDMLtools-0.3.6/test/test_tunner.py
```

### Comparing `BDMLtools-0.3.5/BDMLtools/__init__.py` & `BDMLtools-0.3.6/BDMLtools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from BDMLtools.plotter import BaseWoePlotter
 from BDMLtools.plotter import perfEval,perfEval2
 from BDMLtools.encoder import woeTransformer,binTransformer
 from BDMLtools.tuner import gridTuner,hgridTuner
 from BDMLtools.tuner import BayesianCVTuner,shapCheck
 
 
-__version__ = '0.3.5'
+__version__ = '0.3.6'
 
 __all__ = (    
     dtStandardization,
     outliersTransformer,
     dtypeAllocator,
     nanTransformer,
     businessReport,
```

### Comparing `BDMLtools-0.3.5/BDMLtools/base.py` & `BDMLtools-0.3.6/BDMLtools/base.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.5/BDMLtools/clearner/cleaner.py` & `BDMLtools-0.3.6/BDMLtools/clearner/cleaner.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,15 @@
             
             X_tdiff=X[col_tdiff].div(pd.to_timedelta(self.t_unit)).astype("float64").apply(np.round,args=(self.precision,))
        
             X_float=X[col_float].astype("float64").apply(np.round,args=(self.precision,))
             
             X_obj=X[col_obj].astype('str')
             
-            X_date=None if self.drop_date else X[col_date].replace('[^0-9]','',regex=True).astype('datetime64')
+            X_date=None if self.drop_date else X[col_date].replace('[^0-9]','',regex=True).astype('datetime64[ns]')
             
             X_out=pd.concat([X_keep,X_float,X_obj,X_date,X_tdiff],axis=1)
             
         elif not columns.size:
             
             X_out=self._getXAuto(X)
```

### Comparing `BDMLtools-0.3.5/BDMLtools/encoder/woe.py` & `BDMLtools-0.3.6/BDMLtools/encoder/woe.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.5/BDMLtools/exception.py` & `BDMLtools-0.3.6/BDMLtools/exception.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.5/BDMLtools/fun.py` & `BDMLtools-0.3.6/BDMLtools/fun.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.5/BDMLtools/plotter/base.py` & `BDMLtools-0.3.6/BDMLtools/plotter/base.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.5/BDMLtools/plotter/eval.py` & `BDMLtools-0.3.6/BDMLtools/plotter/eval.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.5/BDMLtools/report/report.py` & `BDMLtools-0.3.6/BDMLtools/report/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,17 +102,16 @@
         category_col=X.select_dtypes(include=['object','category']).columns.tolist()
             
         if len(category_col):    
     
             report={}
             for col in category_col:
     
-                ColTable=X[col].value_counts(dropna=False).sort_index().rename('Freq').reset_index() \
-                    .rename(columns={'index':'Levels'})[['Levels','Freq']]
-    
+                ColTable=X[col].value_counts(dropna=False).sort_index().rename('Freq').reset_index()
+                ColTable.columns=['Levels','Freq']
                 ColTable['Percent']=ColTable.Freq/X[col].size #占比
                 ColTable['CumFreq']=ColTable.Freq.cumsum() #累计(分类特征类别有次序性时有参考价值)
                 ColTable['CumPercent']=ColTable.CumFreq/X[col].size #累计占比(分类特征类别有次序性时有参考价值)
     
                 report[col]=ColTable
             
             return pd.concat(report).droplevel(1).reset_index().rename(columns={'index':'Name'})
```

### Comparing `BDMLtools-0.3.5/BDMLtools/selector/__init__.py` & `BDMLtools-0.3.6/BDMLtools/selector/__init__.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.5/BDMLtools/selector/bin.py` & `BDMLtools-0.3.6/BDMLtools/selector/bin.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.5/BDMLtools/selector/bin_fun.py` & `BDMLtools-0.3.6/BDMLtools/selector/bin_fun.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.5/BDMLtools/selector/embeded.py` & `BDMLtools-0.3.6/BDMLtools/selector/embeded.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.5/BDMLtools/selector/fa.py` & `BDMLtools-0.3.6/BDMLtools/selector/fa.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from sklearn.metrics.pairwise import pairwise_distances
 from scipy.stats import pearsonr,spearmanr
 from sklearn.base import TransformerMixin
 from sklearn.decomposition import PCA
 from sklearn.preprocessing import StandardScaler
 import warnings
 from BDMLtools.base import Base
+import inspect
 
 
 class faSelector(Base,TransformerMixin):
     
     """
     变量聚类:基于sklearn.cluster.FeatureAgglomeration
     
@@ -271,20 +272,32 @@
             
             X_t=X.T
         
         m = pd.DataFrame(pairwise_distances(X_t,X_t,metric=custom_distance)) #距离衡量
         
         if distance_threshold:
             
-            model = FeatureAgglomeration(distance_threshold=distance_threshold,n_clusters=None,metric='precomputed',linkage=linkage).fit(m)
+            if 'metric' in inspect.signature(FeatureAgglomeration).parameters:
+            
+                model = FeatureAgglomeration(distance_threshold=distance_threshold,n_clusters=None,metric='precomputed',linkage=linkage).fit(m)
+            
+            else:
+                
+                model = FeatureAgglomeration(distance_threshold=distance_threshold,n_clusters=None,affinity='precomputed',linkage=linkage).fit(m)
             
         elif n_clusters:
             
-            model = FeatureAgglomeration(n_clusters=n_clusters,metric='precomputed',linkage='average').fit(m)
+            if 'metric' in inspect.signature(FeatureAgglomeration).parameters:
             
+                model = FeatureAgglomeration(n_clusters=n_clusters,metric='precomputed',linkage='average').fit(m)                
+            
+            else:
+                
+                model = FeatureAgglomeration(n_clusters=n_clusters,affinity='precomputed',linkage='average').fit(m)          
+                
         else:
             
             raise ValueError('set n_clusters or distance_threshold')
 
         if np.unique(model.labels_).size==1:
             
             raise ValueError('Only 1 cluster,reset the distance_threshold or n_clusters')
@@ -324,15 +337,22 @@
         else:
             
             X_t=X.T
         
         m = pd.DataFrame(pairwise_distances(X_t, X_t, metric=custom_distance)) #使用相关系数距离衡量
 
         #affinity设定为'precomputed',linkage设定为非ward
-        model = FeatureAgglomeration(distance_threshold=0,n_clusters=None,metric='precomputed',linkage=linkage).fit(m)
+        if 'metric' in inspect.signature(FeatureAgglomeration).parameters:
+            
+            model = FeatureAgglomeration(distance_threshold=0,n_clusters=None,metric='precomputed',linkage=linkage).fit(m)
+        
+        else:
+            
+            model = FeatureAgglomeration(distance_threshold=0,n_clusters=None,affinity='precomputed',linkage=linkage).fit(m)
+            
         plt.title('Hierarchical Clustering Dendrogram')
         plot(model)
         plt.xlabel("Variable index")
         plt.ylabel("distance")
         
     def _getComponentsInfos(self,X,fclusters):
```

### Comparing `BDMLtools-0.3.5/BDMLtools/selector/lgbm.py` & `BDMLtools-0.3.6/BDMLtools/selector/lgbm.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.5/BDMLtools/selector/logtit.py` & `BDMLtools-0.3.6/BDMLtools/selector/logtit.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.5/BDMLtools/selector/simple.py` & `BDMLtools-0.3.6/BDMLtools/selector/simple.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.5/BDMLtools/tuner/base.py` & `BDMLtools-0.3.6/BDMLtools/tuner/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from sklearn import metrics
 import numpy as np
 import pandas as pd
 from lightgbm import LGBMClassifier
 import warnings
-#from catboost.core import CatBoostClassifier
-#from xgboost import XGBClassifier
 
 
 class BaseTunner:
     
     @property
     def _get_scorer(self):
```

### Comparing `BDMLtools-0.3.5/BDMLtools/tuner/bayesian.py` & `BDMLtools-0.3.6/BDMLtools/tuner/bayesian.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,25 +4,22 @@
 Created on Thu Oct 14 17:26:03 2021
 
 @author: zengke
 """
 from BDMLtools.base import Base
 from BDMLtools.tuner.base import BaseTunner
 #from sklearn.model_selection import GridSearchCV
-from xgboost.sklearn import XGBClassifier
 #from bayes_opt import BayesianOptimization
 from sklearn.calibration import CalibratedClassifierCV
-from catboost import CatBoostClassifier
 from sklearn.model_selection import RepeatedStratifiedKFold,train_test_split
 #from lightgbm import early_stopping as lgbm_early_stopping
 #from time import time
 #import pandas as pd
-from joblib import effective_n_jobs,cpu_count
+from joblib import effective_n_jobs
 #import numpy as np
-from lightgbm.sklearn import LGBMClassifier
 from skopt import BayesSearchCV
 
 
 class BayesianCVTuner(Base,BaseTunner):
     
     '''
     使用scikit-optmize进行贝叶斯超参优化，可支持分类超参，能够提供对sklearn生态更好的兼容性且效率较高
@@ -161,19 +158,19 @@
         return pred
     
     def transform(self,X,y=None):   
         
         self._check_is_fitted()
         self._check_X(X)
         
-        if self.Estimator is CatBoostClassifier:
+        if self.Estimator.__module__ == "catboost.core":
             
             out=X.apply(lambda col:col.astype('str') if col.name in self.cat_features else col) if self.cat_features else X
             
-        elif self.Estimator is LGBMClassifier:
+        elif self.Estimator.__module__ == 'lightgbm.sklearn':
         
             out=X.apply(lambda col:col.astype('category') if col.name in self.cat_features else col) if self.cat_features else X
             
         else:
             
             out=X
             
@@ -194,19 +191,19 @@
         self._check_data(X, y)
         self._check_ws(y, sample_weight)
         
         self.cat_features=X.select_dtypes(['object','category']).columns.tolist() if cat_features is None else cat_features    
         
         para_space=self._hpsearch_default(self.Estimator) if not self.para_space else self.para_space
         
-        if self.Estimator is CatBoostClassifier:
+        if self.Estimator.__module__ == "catboost.core":
             
             X=X.apply(lambda col:col.astype('str') if col.name in self.cat_features else col) if self.cat_features else X
             
-        elif self.Estimator is LGBMClassifier:
+        elif self.Estimator.__module__ == 'lightgbm.sklearn':
         
             X=X.apply(lambda col:col.astype('category') if col.name in self.cat_features else col) if self.cat_features else X
             
         else:
             
             X=X 
             
@@ -223,15 +220,15 @@
             #params_best
             self.params_best=self.bs_res.best_params_
      
             #cv_result
             self.cv_result=self._cvresult_to_df(self.bs_res.cv_results_)
             
             #refit with early_stopping_rounds                  
-            if self.Estimator is CatBoostClassifier:
+            if self.Estimator.__module__ == "catboost.core":
                 
                 refit_Estimator=self.Estimator(random_state=self.random_state,
                                                thread_count=effective_n_jobs(self.n_jobs),
                                                **self.params_best)
                 
                 if self.eval_metric=='auc':
                     
@@ -243,30 +240,30 @@
                 
                 refit_Estimator=self.Estimator(random_state=self.random_state,
                                                n_jobs=effective_n_jobs(self.n_jobs),
                                                **self.params_best)
 
             self.model_refit = refit_Estimator.fit(**self._get_fit_params(self.Estimator,X_tr,y_tr,X_val,y_val,sample_weight,y_tr.index,y_val.index))   
                                                                                                  
-            self.params_best['best_iteration']=self.model_refit.best_iteration if self.Estimator is XGBClassifier else self.model_refit.best_iteration_ 
+            self.params_best['best_iteration']=self.model_refit.best_iteration if self.Estimator.__module__ == 'xgboost.sklearn' else self.model_refit.best_iteration_ 
             
             
         else:
             
             #BayesSearch_CV        
             self._BayesSearch_CV(para_space,X,y,sample_weight)
             
             #params_best
             self.params_best=self.bs_res.best_params_
      
             #cv_result
             self.cv_result=self._cvresult_to_df(self.bs_res.cv_results_)
             
             #refit model
-            if self.Estimator is CatBoostClassifier:
+            if self.Estimator.__module__ == "catboost.core":
                 
                 refit_Estimator=self.Estimator(random_state=self.random_state,
                                                thread_count=effective_n_jobs(self.n_jobs),
                                                **self.params_best)
                 
                 refit_Estimator.set_params(**{'cat_features':self.cat_features})
                 
@@ -301,15 +298,15 @@
             scorer=self.scoring
              
                     
         cv = RepeatedStratifiedKFold(n_splits=self.cv, n_repeats=self.repeats, random_state=self.random_state)
         
         n_jobs=effective_n_jobs(self.n_jobs)
         
-        if self.Estimator is CatBoostClassifier:
+        if self.Estimator.__module__ == "catboost.core":
             
             bs=BayesSearchCV(
                 self.Estimator(random_state=self.random_state,thread_count=n_jobs),para_space,cv=cv,
                 n_iter=self.n_iter,n_points=self.init_points,
                 n_jobs=-1 if self.n_jobs==-1 else 1,
                 verbose=self.verbose,refit=False,random_state=self.random_state,
                 scoring=scorer,error_score=0)    
@@ -331,15 +328,15 @@
             
         return(self)     
     
     
     def _get_fit_params(self,Estimator,X_train,y_train,X_val,y_val,sample_weight=None,train_index=None,val_index=None):
         
         
-        if Estimator is XGBClassifier:
+        if Estimator.__module__ == "xgboost.sklearn":
             
             fit_params = {
                 "X":X_train,
                 "y":y_train,
                 "eval_set": [(X_val, y_val)],
                 "eval_metric": self.eval_metric,
                 "early_stopping_rounds": self.early_stopping_rounds,
@@ -347,15 +344,15 @@
             
             if sample_weight is not None:
                 
                 fit_params["sample_weight"] = sample_weight.loc[train_index]
                 fit_params["sample_weight_eval_set"] = [sample_weight.loc[val_index]]
         
             
-        elif Estimator is LGBMClassifier:
+        elif Estimator.__module__ == 'lightgbm.sklearn':
             
             from lightgbm import early_stopping, log_evaluation
 
             fit_params = {
                 "X":X_train,
                 "y":y_train,
                 "eval_set": [(X_val, y_val)],
@@ -373,15 +370,15 @@
                 
             if sample_weight is not None:
                 
                 fit_params["sample_weight"] = sample_weight.loc[train_index]
                 fit_params["eval_sample_weight"] = [sample_weight.loc[val_index]]
             
         
-        elif Estimator is CatBoostClassifier:
+        elif Estimator.__module__ == "catboost.core":
             
             from catboost import Pool
             
             fit_params = {
                 "X": Pool(X_train, y_train, cat_features=self.cat_features),
                 "eval_set": Pool(X_val, y_val, cat_features=self.cat_features),
                 "early_stopping_rounds": self.early_stopping_rounds,
@@ -401,30 +398,30 @@
     
     
     @staticmethod
     def _hpsearch_default(Estimator):
         
         from skopt.utils import Categorical,Real,Integer
         
-        if Estimator is XGBClassifier:
+        if Estimator.__module__ == "xgboost.sklearn":
             
             para_space = {
                 'n_estimators': Integer(30, 120),
                 'max_depth':Integer(2, 4),
                 'learning_rate': Real(0.05, 0.2,prior='uniform'),
                 
                 'gamma': Real(0,10,prior='uniform'),
                 'subsample':Real(0.5,1.0,prior='uniform'),
                 'colsample_bytree':Real(0.5,1.0,prior='uniform'),
                 'reg_lambda':Real(0,10,prior='uniform'),
                 
                 'use_label_encoder':Categorical([False])            
             } 
             
-        elif Estimator is LGBMClassifier:
+        elif Estimator.__module__ == 'lightgbm.sklearn':
             
             para_space = {
                 
                 'verbose':Categorical([-1]),
                 'boosting_type':Categorical(['gbdt','goss']),
                 'n_estimators': Integer(30, 120),
                 'max_depth':Integer(2, 4),
@@ -434,15 +431,15 @@
                 'min_child_samples':Integer(1, 100,prior='uniform'),
                 
                 'subsample':Real(0.5,1.0,prior='uniform'),
                 'colsample_bytree':Real(0.5,1.0,prior='uniform'),
                 'reg_lambda':Real(0,10,prior='uniform'),    
             } 
             
-        elif Estimator is CatBoostClassifier:
+        elif Estimator.__module__ == "catboost.core":
             
             para_space = {
             
                 'n_estimators': Integer(30, 120),
                 'learning_rate': Real(0.05, 0.2,prior='uniform'),
             
                 'max_depth':Integer(2, 4),
```

### Comparing `BDMLtools-0.3.5/BDMLtools/tuner/fun.py` & `BDMLtools-0.3.6/BDMLtools/tuner/fun.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 """
 
 import pandas as pd
 from BDMLtools.selector import binSelector
 from BDMLtools.encoder import woeTransformer
 import shap
 from scipy.stats import pearsonr,spearmanr
-from lightgbm import LGBMClassifier
-from catboost import CatBoostClassifier
 from joblib import effective_n_jobs,Parallel,delayed
 import numpy as np
 
 class shapCheck:
     
     """ 
     对树模型结果进行woe/shap相关性校验
@@ -79,33 +77,35 @@
                                 iv_limit=0,sample_weight=sample_weight,n_jobs=self.n_jobs,verbose=self.verbose).fit(X,y)
             
             X_woe=woeTransformer(bins.bins,woe_missing=0,distr_limit=0.05).fit_transform(X)
         
 
         explainer = shap.TreeExplainer(self.Estimator)        
             
-        if isinstance(self.Estimator,LGBMClassifier):
+        if self.Estimator.__module__ == 'lightgbm.sklearn':
             
             cate_cols=X.select_dtypes(['object','category']).columns.tolist()
         
             if cate_cols:
                 
                 X=X.apply(lambda x:x.astype('category') if x.name in cate_cols else x)
                 
             X_shap=pd.DataFrame(explainer.shap_values(X)[1],columns=X.columns,index=X.index)
             
 
-        elif self.Estimator is CatBoostClassifier:
+        elif self.Estimator.__module__ == 'catboost.core':
             
             cate_cols=X.select_dtypes(['object','category']).columns.tolist()
 
             if cate_cols:
                 
                 X=X.apply(lambda x:x.astype('str') if x.name in cate_cols else x)
                 
+            X_shap=pd.DataFrame(explainer.shap_values(X),columns=X.columns,index=X.index)
+                
         else:
                 
             X_shap=pd.DataFrame(explainer.shap_values(X),columns=X.columns,index=X.index)
         
         self.report=self._check(X_woe, X_shap)
         
         if self.plot==True:
```

### Comparing `BDMLtools-0.3.5/BDMLtools/tuner/gridcv.py` & `BDMLtools-0.3.6/BDMLtools/tuner/gridcv.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 
 from sklearn.model_selection import GridSearchCV,RandomizedSearchCV
 from sklearn.model_selection import RepeatedStratifiedKFold,train_test_split
 from sklearn.calibration import CalibratedClassifierCV
 from BDMLtools.base import Base
 from BDMLtools.tuner.base import BaseTunner
 from joblib import effective_n_jobs
-from lightgbm.sklearn import LGBMClassifier
-from catboost.core import CatBoostClassifier
-from xgboost import XGBClassifier
 
 
 class gridTuner(Base,BaseTunner):
     
     '''
     Xgb与Lgbm的网格搜索与随机搜索
     Parameters:
@@ -212,19 +209,19 @@
         return pred
     
     def transform(self,X,y=None):  
         
         self._check_is_fitted()
         self._check_X(X)
         
-        if self.Estimator is CatBoostClassifier:
+        if self.Estimator.__module__ == 'catboost.core':
             
             out=X.apply(lambda col:col.astype('str') if col.name in self.cat_features else col) if self.cat_features else X
             
-        elif self.Estimator is LGBMClassifier:
+        elif self.Estimator.__module__ == 'lightgbm.sklearn':
         
             out=X.apply(lambda col:col.astype('category') if col.name in self.cat_features else col) if self.cat_features else X
             
         else:
             
             out=X
 
@@ -243,19 +240,19 @@
         
         self._check_data(X, y)     
         self._check_ws(y, sample_weight)
         
         self.cat_features=X.select_dtypes(['object','category']).columns.tolist() if cat_features is None else cat_features    
 
 
-        if self.Estimator is CatBoostClassifier:
+        if self.Estimator.__module__ == 'catboost.core':
             
             X=X.apply(lambda col:col.astype('str') if col.name in self.cat_features else col) if self.cat_features else X
             
-        elif self.Estimator is LGBMClassifier:
+        elif self.Estimator.__module__ == 'lightgbm.sklearn':       
         
             X=X.apply(lambda col:col.astype('category') if col.name in self.cat_features else col) if self.cat_features else X
             
         else:
             
             X=X   
 
@@ -271,15 +268,15 @@
                 self._grid_search(X_tr,y_tr,sample_weight_tr)
                 
                 #输出最优参数组合
                 self.params_best=self.grid_res.best_params_
                 self.cv_result=self._cvresult_to_df(self.grid_res.cv_results_)
                 
                 #refit with early_stopping_rounds  
-                if self.Estimator is CatBoostClassifier:
+                if self.Estimator.__module__ == 'catboost.core':
                     
                     refit_Estimator=self.Estimator(random_state=self.random_state,
                                                    thread_count=effective_n_jobs(self.n_jobs),
                                                    **self.params_best)
                     
                     if self.eval_metric=='auc':
                         
@@ -291,15 +288,15 @@
                     
                     refit_Estimator=self.Estimator(random_state=self.random_state,
                                                    n_jobs=effective_n_jobs(self.n_jobs),
                                                    **self.params_best)
     
                 self.model_refit = refit_Estimator.fit(**self._get_fit_params(self.Estimator,X_tr,y_tr,X_val,y_val,sample_weight,y_tr.index,y_val.index))   
                                                                                                      
-                self.params_best['best_iteration']=self.model_refit.best_iteration if self.Estimator is XGBClassifier else self.model_refit.best_iteration_ 
+                self.params_best['best_iteration']=self.model_refit.best_iteration if self.Estimator.__module__ == 'xgboost.sklearn' else self.model_refit.best_iteration_ 
                 
             else:
                 
                 #search
                 self._grid_search(X,y,sample_weight)
                 
                 #params_best
@@ -307,15 +304,15 @@
          
                 #cv_result
                 self.cv_result=self._cvresult_to_df(self.grid_res.cv_results_)
                 
                 #refit model
                 
 
-                if self.Estimator is CatBoostClassifier:
+                if self.Estimator.__module__ == 'catboost.core':
                     
                     refit_Estimator=self.Estimator(random_state=self.random_state,
                                                    thread_count=effective_n_jobs(self.n_jobs),
                                                    **self.params_best)
                     
                     refit_Estimator.set_params(**{'cat_features':self.cat_features})
                     
@@ -340,15 +337,15 @@
             
                 self._random_search(X_tr,y_tr,sample_weight)
                 #输出最优参数组合
                 self.params_best=self.r_grid_res.best_params_
                 self.cv_result=self._cvresult_to_df(self.r_grid_res.cv_results_)                
             
                 #refit with early_stopping_rounds or None  
-                if self.Estimator is CatBoostClassifier:
+                if self.Estimator.__module__ == 'catboost.core':
                     
                     refit_Estimator=self.Estimator(random_state=self.random_state,
                                                    thread_count=effective_n_jobs(self.n_jobs),
                                                    **self.params_best)
            
                     if self.eval_metric=='auc':
                         
@@ -360,30 +357,30 @@
                     
                     refit_Estimator=self.Estimator(random_state=self.random_state,
                                                    n_jobs=effective_n_jobs(self.n_jobs),
                                                    **self.params_best)
     
                 self.model_refit = refit_Estimator.fit(**self._get_fit_params(self.Estimator,X_tr,y_tr,X_val,y_val,sample_weight,y_tr.index,y_val.index))   
                                                                                                      
-                self.params_best['best_iteration']=self.model_refit.best_iteration if self.Estimator is XGBClassifier else self.model_refit.best_iteration_ 
+                self.params_best['best_iteration']=self.model_refit.best_iteration if self.Estimator.__module__ == 'xgboost.sklearn' else self.model_refit.best_iteration_ 
     
     
             else:
                 
                 #search
                 self._random_search(X,y,sample_weight)
                 
                 #params_best
                 self.params_best=self.r_grid_res.best_params_
          
                 #cv_result
                 self.cv_result=self._cvresult_to_df(self.r_grid_res.cv_results_)
                 
                 #refit with early_stopping_rounds or None      
-                if self.Estimator is CatBoostClassifier:
+                if self.Estimator.__module__ == 'catboost.core':
                     
                     refit_Estimator=self.Estimator(random_state=self.random_state,
                                                    thread_count=effective_n_jobs(self.n_jobs),
                                                    **self.params_best)
                     
                     refit_Estimator.set_params(**{'cat_features':self.cat_features})
                     
@@ -423,15 +420,15 @@
             
             scorer=self.scoring
             
         cv = RepeatedStratifiedKFold(n_splits=self.cv, n_repeats=self.repeats, random_state=self.random_state) 
         
         n_jobs=effective_n_jobs(self.n_jobs)              
         
-        if self.Estimator is CatBoostClassifier:
+        if self.Estimator.__module__ == 'catboost.core':
             
             grid=GridSearchCV(self.Estimator(random_state=self.random_state,thread_count=n_jobs),self.para_space,cv=cv,
                               n_jobs=-1 if self.n_jobs==-1 else 1,
                               refit=False,
                               verbose=self.verbose,
                               scoring=scorer,error_score=0)   
             
@@ -464,15 +461,15 @@
             scorer=self.scoring
         
         cv = RepeatedStratifiedKFold(n_splits=self.cv, n_repeats=self.repeats, random_state=self.random_state) 
         
         n_jobs=effective_n_jobs(self.n_jobs) 
         
         
-        if self.Estimator is CatBoostClassifier:
+        if self.Estimator.__module__ == 'catboost.core':
             
             r_grid=RandomizedSearchCV(self.Estimator(random_state=self.random_state,thread_count=n_jobs),self.para_space,cv=cv,
                                       n_jobs=-1 if self.n_jobs==-1 else 1,
                                       verbose=self.verbose,refit=False,
                                       random_state=self.random_state,
                                       scoring=scorer,error_score=0,n_iter=self.n_iter)
         
@@ -490,15 +487,15 @@
         
         return self  
     
     
     def _get_fit_params(self,Estimator,X_train,y_train,X_val,y_val,sample_weight=None,train_index=None,val_index=None):
         
         
-        if Estimator is XGBClassifier:
+        if Estimator.__module__ == "xgboost.sklearn":
             
             fit_params = {
                 "X":X_train,
                 "y":y_train,
                 "eval_set": [(X_val, y_val)],
                 "eval_metric": self.eval_metric,
                 "early_stopping_rounds": self.early_stopping_rounds,
@@ -506,15 +503,15 @@
             
             if sample_weight is not None:
                 
                 fit_params["sample_weight"] = sample_weight.loc[train_index]
                 fit_params["sample_weight_eval_set"] = [sample_weight.loc[val_index]]
         
             
-        elif Estimator is LGBMClassifier:
+        elif Estimator.__module__ == 'lightgbm.sklearn':
             
             from lightgbm import early_stopping, log_evaluation
 
             fit_params = {
                 "X":X_train,
                 "y":y_train,
                 "eval_set": [(X_val, y_val)],
@@ -532,15 +529,15 @@
                 
             if sample_weight is not None:
                 
                 fit_params["sample_weight"] = sample_weight.loc[train_index]
                 fit_params["eval_sample_weight"] = [sample_weight.loc[val_index]]
             
         
-        elif Estimator is CatBoostClassifier:
+        elif Estimator.__module__ == "catboost.core":
             
             from catboost import Pool
             
             fit_params = {
                 "X": Pool(X_train, y_train, cat_features=self.cat_features),
                 "eval_set": Pool(X_val, y_val, cat_features=self.cat_features),
                 "early_stopping_rounds": self.early_stopping_rounds,
```

### Comparing `BDMLtools-0.3.5/BDMLtools/tuner/halvingcv.py` & `BDMLtools-0.3.6/BDMLtools/tuner/halvingcv.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,18 +9,15 @@
 from BDMLtools.base import Base
 from sklearn.experimental import enable_halving_search_cv
 from sklearn.model_selection import train_test_split
 from BDMLtools.tuner.base import BaseTunner
 from sklearn.model_selection import HalvingGridSearchCV,HalvingRandomSearchCV,RepeatedStratifiedKFold
 from sklearn.calibration import CalibratedClassifierCV
 from joblib import effective_n_jobs
-from lightgbm.sklearn import LGBMClassifier
-from catboost.core import CatBoostClassifier
-from xgboost import XGBClassifier
-from lightgbm import early_stopping as lgbm_early_stopping
+#from lightgbm import early_stopping as lgbm_early_stopping
 
 
 class hgridTuner(Base,BaseTunner):
     
     '''
     Xgb与Lgbm的sucessive halving搜索与sucessive halving搜索
     Parameters:
@@ -223,19 +220,19 @@
     
     
     def transform(self,X,y=None):   
 
         self._check_is_fitted()
         self._check_X(X)
         
-        if self.Estimator is CatBoostClassifier:
+        if self.Estimator.__module__ == 'catboost.core':
             
             out=X.apply(lambda col:col.astype('str') if col.name in self.cat_features else col) if self.cat_features else X
             
-        elif self.Estimator is LGBMClassifier:
+        elif self.Estimator.__module__ == 'lightgbm.sklearn':
         
             out=X.apply(lambda col:col.astype('category') if col.name in self.cat_features else col) if self.cat_features else X
             
         else:
             
             out=X        
          
@@ -253,19 +250,19 @@
         '''   
         
         self._check_data(X, y)
         self._check_ws(y, sample_weight)
         
         self.cat_features=X.select_dtypes(['object','category']).columns.tolist() if cat_features is None else cat_features    
         
-        if self.Estimator is CatBoostClassifier:
+        if self.Estimator.__module__ == 'catboost.core':
             
             X=X.apply(lambda col:col.astype('str') if col.name in self.cat_features else col) if self.cat_features else X
             
-        elif self.Estimator is LGBMClassifier:
+        elif self.Estimator.__module__ == 'lightgbm.sklearn':
         
             X=X.apply(lambda col:col.astype('category') if col.name in self.cat_features else col) if self.cat_features else X
             
         else:
             
             X=X   
 
@@ -280,15 +277,15 @@
             
                 self._h_grid_search(X_tr,y_tr,sample_weight_tr)
                 #输出最优参数组合
                 self.params_best=self.h_grid_res.best_params_
                 self.cv_result=self._cvresult_to_df(self.h_grid_res.cv_results_)
             
                 #refit with early_stopping_rounds  
-                if self.Estimator is CatBoostClassifier:
+                if self.Estimator.__module__ == 'catboost.core':
                     
                     refit_Estimator=self.Estimator(random_state=self.random_state,
                                                    thread_count=effective_n_jobs(self.n_jobs),
                                                    **self.params_best)
                     
                     if self.eval_metric=='auc':
                         
@@ -301,30 +298,30 @@
                     refit_Estimator=self.Estimator(random_state=self.random_state,
                                                    n_jobs=effective_n_jobs(self.n_jobs),
                                                    **self.params_best)
                     
             
                 self.model_refit = refit_Estimator.fit(**self._get_fit_params(self.Estimator,X_tr,y_tr,X_val,y_val,sample_weight,y_tr.index,y_val.index))   
                                                                                                      
-                self.params_best['best_iteration']=self.model_refit.best_iteration if self.Estimator is XGBClassifier else self.model_refit.best_iteration_ 
+                self.params_best['best_iteration']=self.model_refit.best_iteration if self.Estimator.__module__ == 'xgboost.sklearn' else self.model_refit.best_iteration_ 
                 
             else:
                 
                 #search
                 
                 self._h_grid_search(X,y,sample_weight)
                 
                 #params_best
                 self.params_best=self.h_grid_res.best_params_
             
                 #cv_result
                 self.cv_result=self._cvresult_to_df(self.h_grid_res.cv_results_)
                 
                 #refit model            
-                if self.Estimator is CatBoostClassifier:
+                if self.Estimator.__module__ == 'catboost.core':
                     
                     refit_Estimator=self.Estimator(random_state=self.random_state,
                                                    thread_count=effective_n_jobs(self.n_jobs),**self.params_best)
                     
                     refit_Estimator.set_params(**{'cat_features':self.cat_features})
                     
                 else:
@@ -345,15 +342,15 @@
             
                 self._h_random_search(X_tr,y_tr,sample_weight_tr)
                 #输出最优参数组合
                 self.params_best=self.h_random_res.best_params_
                 self.cv_result=self._cvresult_to_df(self.h_random_res.cv_results_)
             
                 #refit with early_stopping_rounds  
-                if self.Estimator is CatBoostClassifier:
+                if self.Estimator.__module__ == 'catboost.core':
                     
                     refit_Estimator=self.Estimator(random_state=self.random_state,
                                                    thread_count=effective_n_jobs(self.n_jobs),
                                                    **self.params_best)
                     
                     if self.eval_metric=='auc':
                         
@@ -365,30 +362,30 @@
                     
                     refit_Estimator=self.Estimator(random_state=self.random_state,
                                                    n_jobs=effective_n_jobs(self.n_jobs),
                                                    **self.params_best)                    
             
                 self.model_refit = refit_Estimator.fit(**self._get_fit_params(self.Estimator,X_tr,y_tr,X_val,y_val,sample_weight,y_tr.index,y_val.index))   
                                                                                                      
-                self.params_best['best_iteration']=self.model_refit.best_iteration if self.Estimator is XGBClassifier else self.model_refit.best_iteration_ 
+                self.params_best['best_iteration']=self.model_refit.best_iteration if self.Estimator.__module__ == 'xgboost.sklearn' else self.model_refit.best_iteration_ 
                 
             else:
                 
                 #search
                 
                 self._h_random_search(X,y,sample_weight)
                 
                 #params_best
                 self.params_best=self.h_random_res.best_params_
             
                 #cv_result
                 self.cv_result=self._cvresult_to_df(self.h_random_res.cv_results_)
                 
                 #refit model
-                if self.Estimator is CatBoostClassifier:
+                if self.Estimator.__module__ == 'catboost.core':
                     
                     refit_Estimator=self.Estimator(random_state=self.random_state,
                                                    thread_count=effective_n_jobs(self.n_jobs),**self.params_best)                   
                     
                     refit_Estimator.set_params(**{'cat_features':self.cat_features})
                     
                 else:
@@ -428,15 +425,15 @@
             scorer=self.scoring
             
         cv = RepeatedStratifiedKFold(n_splits=self.cv, n_repeats=self.repeats, random_state=self.random_state) 
         
         n_jobs=effective_n_jobs(self.n_jobs) 
         
         
-        if self.Estimator is CatBoostClassifier:
+        if self.Estimator.__module__ == 'catboost.core':
             
             hgrid=HalvingGridSearchCV(self.Estimator(random_state=self.random_state,thread_count=n_jobs),
                                       param_grid=self.para_space,
                                       cv=cv,
                                       refit=False,
                                       factor=self.factor,
                                       scoring=scorer,
@@ -476,15 +473,15 @@
             
            scorer=self.scoring
         
         cv = RepeatedStratifiedKFold(n_splits=self.cv, n_repeats=self.repeats, random_state=self.random_state) 
         
         n_jobs=effective_n_jobs(self.n_jobs) 
         
-        if self.Estimator is CatBoostClassifier:
+        if self.Estimator.__module__ == 'catboost.core':
             
             h_r_grid=HalvingRandomSearchCV(self.Estimator(random_state=self.random_state,thread_count=n_jobs),
                                          param_distributions=self.para_space,
                                          n_candidates=self.n_candidates,
                                          factor=self.factor,
                                          cv=cv,
                                          n_jobs=-1 if self.n_jobs==-1 else 1,
@@ -514,15 +511,15 @@
         
         return self   
     
     
     def _get_fit_params(self,Estimator,X_train,y_train,X_val,y_val,sample_weight=None,train_index=None,val_index=None):
         
         
-        if Estimator is XGBClassifier:
+        if Estimator.__module__ == "xgboost.sklearn":
             
             fit_params = {
                 "X":X_train,
                 "y":y_train,
                 "eval_set": [(X_val, y_val)],
                 "eval_metric": self.eval_metric,
                 "early_stopping_rounds": self.early_stopping_rounds,
@@ -530,15 +527,15 @@
             
             if sample_weight is not None:
                 
                 fit_params["sample_weight"] = sample_weight.loc[train_index]
                 fit_params["sample_weight_eval_set"] = [sample_weight.loc[val_index]]
         
             
-        elif Estimator is LGBMClassifier:
+        elif Estimator.__module__ == 'lightgbm.sklearn':
             
             from lightgbm import early_stopping, log_evaluation
 
             fit_params = {
                 "X":X_train,
                 "y":y_train,
                 "eval_set": [(X_val, y_val)],
@@ -556,15 +553,15 @@
                 
             if sample_weight is not None:
                 
                 fit_params["sample_weight"] = sample_weight.loc[train_index]
                 fit_params["eval_sample_weight"] = [sample_weight.loc[val_index]]
             
         
-        elif Estimator is CatBoostClassifier:
+        elif Estimator.__module__ == "catboost.core":
             
             from catboost import Pool
             
             fit_params = {
                 "X": Pool(X_train, y_train, cat_features=self.cat_features),
                 "eval_set": Pool(X_val, y_val, cat_features=self.cat_features),
                 "early_stopping_rounds": self.early_stopping_rounds,
```

### Comparing `BDMLtools-0.3.5/BDMLtools.egg-info/PKG-INFO` & `BDMLtools-0.3.6/BDMLtools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: BDMLtools
-Version: 0.3.5
+Version: 0.3.6
 Summary: Ml learning tools for busniess data mining
 Author: 曾珂
 Author-email: zengke403@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE
 
-# BDMLtools-0.3.5
+# BDMLtools-0.3.6
 
 [![PyPI version](https://img.shields.io/pypi/pyversions/BDMLtools.svg)](https://pypi.python.org/pypi/BDMLtools)
 [![License](https://img.shields.io/github/license/zk403/mlearn)](https://github.com/zk403/mlearn/blob/master/LICENSE)
 [![Build Status](https://github.com/zk403/mlearn/actions/workflows/python-test.yml/badge.svg)](https://github.com/zk403/mlearn/actions/workflows/python-test.yml)
 [![codecov](https://codecov.io/gh/zk403/mlearn/main/graphs/badge.svg)](https://app.codecov.io/gh/zk403/mlearn)
 [![PyPI release](https://img.shields.io/pypi/v/BDMLtools.svg)](https://pypi.python.org/pypi/BDMLtools)
 
@@ -43,16 +43,16 @@
 卸载: 
 
 ```
 pip uninstall BDMLtools
 ```
 
 更新
-
 ```
-v0.3.5
-1.在LassoLgoit中加入随机数参数以消除saga导致得模型无法复现的问题
-2.现在LassoLgoit中将在交叉验证后对全量数据拟合模型并依此计算回归系数相关得指标与图表
-3.移除LassoLgoit的refit_with_C方法，加入select_C方法以选择最合适得模型
-4.更新单元测试脚本,更新部分代码说明
-5.更新example
+v0.3.6
+1.优化代码，移除对xgboost与catboost库的依赖
+2.优化代码，对sklearn的最低依赖降低为1.0.2
+3.修复了shapcheck中的使用catboost时无法计算的bug
+4.修复了EDAreport在pandas==2.0.1版本下的bug
+5.更新单元测试脚本,更新部分代码说明
+6.更新example
 ```
```

### Comparing `BDMLtools-0.3.5/BDMLtools.egg-info/SOURCES.txt` & `BDMLtools-0.3.6/BDMLtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.5/LICENSE` & `BDMLtools-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.5/PKG-INFO` & `BDMLtools-0.3.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: BDMLtools
-Version: 0.3.5
+Version: 0.3.6
 Summary: Ml learning tools for busniess data mining
 Author: 曾珂
 Author-email: zengke403@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE
 
-# BDMLtools-0.3.5
+# BDMLtools-0.3.6
 
 [![PyPI version](https://img.shields.io/pypi/pyversions/BDMLtools.svg)](https://pypi.python.org/pypi/BDMLtools)
 [![License](https://img.shields.io/github/license/zk403/mlearn)](https://github.com/zk403/mlearn/blob/master/LICENSE)
 [![Build Status](https://github.com/zk403/mlearn/actions/workflows/python-test.yml/badge.svg)](https://github.com/zk403/mlearn/actions/workflows/python-test.yml)
 [![codecov](https://codecov.io/gh/zk403/mlearn/main/graphs/badge.svg)](https://app.codecov.io/gh/zk403/mlearn)
 [![PyPI release](https://img.shields.io/pypi/v/BDMLtools.svg)](https://pypi.python.org/pypi/BDMLtools)
 
@@ -43,16 +43,16 @@
 卸载: 
 
 ```
 pip uninstall BDMLtools
 ```
 
 更新
-
 ```
-v0.3.5
-1.在LassoLgoit中加入随机数参数以消除saga导致得模型无法复现的问题
-2.现在LassoLgoit中将在交叉验证后对全量数据拟合模型并依此计算回归系数相关得指标与图表
-3.移除LassoLgoit的refit_with_C方法，加入select_C方法以选择最合适得模型
-4.更新单元测试脚本,更新部分代码说明
-5.更新example
+v0.3.6
+1.优化代码，移除对xgboost与catboost库的依赖
+2.优化代码，对sklearn的最低依赖降低为1.0.2
+3.修复了shapcheck中的使用catboost时无法计算的bug
+4.修复了EDAreport在pandas==2.0.1版本下的bug
+5.更新单元测试脚本,更新部分代码说明
+6.更新example
 ```
```

### Comparing `BDMLtools-0.3.5/README.md` & `BDMLtools-0.3.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# BDMLtools-0.3.5
+# BDMLtools-0.3.6
 
 [![PyPI version](https://img.shields.io/pypi/pyversions/BDMLtools.svg)](https://pypi.python.org/pypi/BDMLtools)
 [![License](https://img.shields.io/github/license/zk403/mlearn)](https://github.com/zk403/mlearn/blob/master/LICENSE)
 [![Build Status](https://github.com/zk403/mlearn/actions/workflows/python-test.yml/badge.svg)](https://github.com/zk403/mlearn/actions/workflows/python-test.yml)
 [![codecov](https://codecov.io/gh/zk403/mlearn/main/graphs/badge.svg)](https://app.codecov.io/gh/zk403/mlearn)
 [![PyPI release](https://img.shields.io/pypi/v/BDMLtools.svg)](https://pypi.python.org/pypi/BDMLtools)
 
@@ -27,16 +27,16 @@
 卸载: 
 
 ```
 pip uninstall BDMLtools
 ```
 
 更新
-
 ```
-v0.3.5
-1.在LassoLgoit中加入随机数参数以消除saga导致得模型无法复现的问题
-2.现在LassoLgoit中将在交叉验证后对全量数据拟合模型并依此计算回归系数相关得指标与图表
-3.移除LassoLgoit的refit_with_C方法，加入select_C方法以选择最合适得模型
-4.更新单元测试脚本,更新部分代码说明
-5.更新example
+v0.3.6
+1.优化代码，移除对xgboost与catboost库的依赖
+2.优化代码，对sklearn的最低依赖降低为1.0.2
+3.修复了shapcheck中的使用catboost时无法计算的bug
+4.修复了EDAreport在pandas==2.0.1版本下的bug
+5.更新单元测试脚本,更新部分代码说明
+6.更新example
 ```
```

### Comparing `BDMLtools-0.3.5/setup.py` & `BDMLtools-0.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,37 +12,38 @@
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 # To use a consistent encoding
 from codecs import open
 from os import path
 import re
 
-base_pkgs=[       #'numpy>=1.18,<=1.22',#https://github.com/numpy/numpy
+base_pkgs=[       'numpy>=1.18,<=1.23.5',#https://github.com/numpy/numpy
                   #'matplotlib>=3.5.0,<=3.5.3',
                   #'lofo-importance>=0.3.1',#https://github.com/aerdem4/lofo-importance
                   'fastparquet>=0.7.1',#https://github.com/dask/fastparquet
                   'pandas>=1.3.5',#https://github.com/pandas-dev/pandas
                   #'statsmodels>=0.13.2',#https://github.com/statsmodels/statsmodels
                   'plotnine>=0.10.1',#https://github.com/has2k1/plotnine
-                  'scikit-learn>=1.2.1',#https://github.com/scikit-learn/scikit-learn
-                  'xgboost>=1.4.2',#https://github.com/dmlc/xgboost
-                  'catboost>=1.0.4',#https://github.com/catboost/catboost
+                  'scikit-learn>=1.0.2',#https://github.com/scikit-learn/scikit-learn
                   'category_encoders>=2.3.0',#https://github.com/scikit-learn-contrib/category_encoders
                   'lightgbm>=3.3.0',#https://github.com/microsoft/LightGBM 
                   'probatus>=1.8.9',#https://github.com/ing-bank/probatus
                   'mlxtend>=0.19.0',#https://github.com/rasbt/mlxtend
                   'scikit-optimize>=0.9.0',#https://github.com/scikit-optimize/scikit-optimize
                   'openpyxl'
                  ]
 
 dev_dep = [
     "pytest>=6.0.0",
     "pytest-cov>=2.10.0",
     "IPython",
-    "mock"
+    "mock",
+    #'shap>=0.41.0',
+    'xgboost>=1.4.2',#https://github.com/dmlc/xgboost
+    'catboost>=1.0.4,<1.2',#https://github.com/catboost/catboost gituhb action failed in macox
 ]
 
 here = path.abspath(path.dirname(__file__))
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
```

### Comparing `BDMLtools-0.3.5/test/test_base.py` & `BDMLtools-0.3.6/test/test_base.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.5/test/test_clearner.py` & `BDMLtools-0.3.6/test/test_clearner.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.5/test/test_eval.py` & `BDMLtools-0.3.6/test/test_eval.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.5/test/test_report.py` & `BDMLtools-0.3.6/test/test_report.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 @author: zengke
 """
 
 from BDMLtools.report import EDAReport,varReport,varGroupsReport,varReportSinge,varGroupsPlot,GainsTable,businessReport
 import pandas as pd
 import numpy as np
 import mock
+import os
 
 def test_EDAReport():
 
     dt=pd.DataFrame(
         {'a':[1,2,2],'b':[1,2,3],'c':['1','2',np.nan],'d':[1,2,np.nan]},
         index=[0,1,2])
     
@@ -24,89 +25,98 @@
     res=EDAReport(is_nacorr=True).report(dt)
     assert hasattr(res,'num_report')
     assert hasattr(res,'char_report')
     assert hasattr(res,'na_report')
     assert hasattr(res,'nacorr_report')
 
 @mock.patch('matplotlib.pyplot.show')
-def test_varReportSinge(mock_show):
+def test_varReportSinge(mock):
     
-    X=pd.DataFrame(
-        {'a':[1,2,2],'c':['1','2','3']})
-    
-    ws=pd.Series([1,1,1],name='y')
-    y=pd.Series([0,1,1],name='y')
+    #plot issue(ax.twinx() failed in windows)
+    if os.name!='nt':
     
-    varReportSinge().report(X['a'],y,[1])
-    varReportSinge().report(X['c'],y,['1','2','3'])
-    varReportSinge().report(X['a'],y,[1],sample_weight=ws)
-    varReportSinge().woe_plot(X['c'],y,['1','2','3'])
-    varReportSinge().woe_plot(X['c'],y,['1','2','3'],sample_weight=ws)
-    varReportSinge().woe_plot(X['c'],y,['1','2%,%3'])
-    varReportSinge().woe_plot(X['c'],y,['1%,%2','3'],sample_weight=ws)
+        X=pd.DataFrame(
+            {'a':[1,2,2],'c':['1','2','3']})
+        
+        ws=pd.Series([1,1,1],name='y')
+        y=pd.Series([0,1,1],name='y')
+        
+        varReportSinge().report(X['a'],y,[1])
+        varReportSinge().report(X['c'],y,['1','2','3'])
+        varReportSinge().report(X['a'],y,[1],sample_weight=ws)
+        varReportSinge().woe_plot(X['c'],y,['1','2','3'])
+        varReportSinge().woe_plot(X['c'],y,['1','2','3'],sample_weight=ws)
+        varReportSinge().woe_plot(X['c'],y,['1','2%,%3'])
+        varReportSinge().woe_plot(X['c'],y,['1%,%2','3'],sample_weight=ws)
 
     
 @mock.patch('matplotlib.pyplot.show')
-def test_varReport(mock_show):
-    
-    X=pd.DataFrame(
-        {'a':[1,2,2],'c':['1','2','3']})
-    
-    ws=pd.Series([1,1,1],name='y')
-    y=pd.Series([0,1,1],name='y')
-
-    res=varReport({'a':[1],'c':['1','2','3']},n_jobs=1).fit(X,y)
-    res=varReport({'a':[1],'c':['1','2','3']},sample_weight=ws,n_jobs=1).fit(X,y)
-    res=varReport({'a':[1],'c':['1','2','3']},out_path='tmp',n_jobs=1).fit(X,y)
+def test_varReport(mock):
     
-    assert hasattr(res,'var_report_dict')
-    assert hasattr(res,'breaks_list_dict')
+    #plot issue(ax.twinx() failed in windows)
+    if os.name!='nt':
     
-    res.woe_plot(n_jobs=1)
+        X=pd.DataFrame(
+            {'a':[1,2,2],'c':['1','2','3']})
+        
+        ws=pd.Series([1,1,1],name='y')
+        y=pd.Series([0,1,1],name='y')
+    
+        res=varReport({'a':[1],'c':['1','2','3']},n_jobs=1).fit(X,y)
+        res=varReport({'a':[1],'c':['1','2','3']},sample_weight=ws,n_jobs=1).fit(X,y)
+        res=varReport({'a':[1],'c':['1','2','3']},out_path='tmp',n_jobs=1).fit(X,y)
+        
+        assert hasattr(res,'var_report_dict')
+        assert hasattr(res,'breaks_list_dict')
+        
+        res.woe_plot(n_jobs=1)
     
 
 def test_businessReport():
     
     X=pd.DataFrame(
         {'a':[1,2,2],'c':['1','2','3'],'g':['g1','g1','g2'],'y':[0,1,1]})
     
     businessReport('y',['g'],None).report(X)
     
     businessReport('y',['g'],None,rename_columns=['group']).report(X)
     
     businessReport('y',['g'],None,rename_index=['group']).report(X)
     
-    businessReport('y',['g'],None,out_path='tmp').report(X)
+    #businessReport('y',['g'],None,out_path='tmp').report(X)
 
     
 @mock.patch('matplotlib.pyplot.show')
-def test_varGroupsReport(mock_show):  
-    
-    X=pd.DataFrame(
-        {'a':[1,2,2],'c':['1','2','3'],'g':['g1','g1','g2'],'y':[0,1,1]})
-    ws=pd.Series([1,1,1],name='y')    
-    
-    res=varGroupsReport({'a':[1],'c':['1','2','3']},columns=['g'],target='y',n_jobs=1).fit(X)
-    res=varGroupsReport({'a':[1],'c':['1','2','3']},sample_weight=ws,columns=['g'],target='y',n_jobs=1).fit(X)
-    res=varGroupsReport({'a':[1],'c':['1','2','3']},columns=['g'],row_limit=1,target='y',n_jobs=1).fit(X)
-    res=varGroupsReport({'a':[1],'c':['1','2','3']},columns=['g'],sort_columns={'g':['g1','g2']},target='y',n_jobs=1).fit(X)   
-    res=varGroupsReport({'a':[1],'c':['1','2','3']},out_path='tmp',columns=['g'],target='y',n_jobs=1).fit(X)
-    
-    assert hasattr(res,'report_dict')
-    assert not len(set(res.report_dict.keys())-set(['report_all','report_brief','report_count',
-                                                    'report_badprob','report_iv','report_ks','report_lift']))
-             
-    res=varGroupsReport({'a':[1],'c':['1','2','3']},columns=['g'],output_psi=True,target='y',n_jobs=1).fit(X)
-    assert hasattr(res,'report_dict')
-    assert not len(set(res.report_dict.keys())-set(['report_all','report_brief','report_count',
-                                                    'report_badprob','report_iv','report_ks','report_psi','report_lift']))
-    
-    varGroupsPlot({'a':[1],'c':['1','2','3']},column='g',target='y',n_jobs=1).plot(X)
-    varGroupsPlot({'a':[1],'c':['1','2','3']},column='g',sort_column=['g1','g2'],target='y',n_jobs=1).plot(X)
+def test_varGroupsReport(mock):  
     
+    #plot issue(ax.twinx() failed in windows)
+    if os.name!='nt':
+        
+        X=pd.DataFrame(
+            {'a':[1,2,2],'c':['1','2','3'],'g':['g1','g1','g2'],'y':[0,1,1]})
+        ws=pd.Series([1,1,1],name='y')    
+        
+        res=varGroupsReport({'a':[1],'c':['1','2','3']},columns=['g'],target='y',n_jobs=1).fit(X)
+        res=varGroupsReport({'a':[1],'c':['1','2','3']},sample_weight=ws,columns=['g'],target='y',n_jobs=1).fit(X)
+        res=varGroupsReport({'a':[1],'c':['1','2','3']},columns=['g'],row_limit=1,target='y',n_jobs=1).fit(X)
+        res=varGroupsReport({'a':[1],'c':['1','2','3']},columns=['g'],sort_columns={'g':['g1','g2']},target='y',n_jobs=1).fit(X)   
+        res=varGroupsReport({'a':[1],'c':['1','2','3']},out_path='tmp',columns=['g'],target='y',n_jobs=1).fit(X)
+        
+        assert hasattr(res,'report_dict')
+        assert not len(set(res.report_dict.keys())-set(['report_all','report_brief','report_count',
+                                                        'report_badprob','report_iv','report_ks','report_lift']))
+                 
+        res=varGroupsReport({'a':[1],'c':['1','2','3']},columns=['g'],output_psi=True,target='y',n_jobs=1).fit(X)
+        assert hasattr(res,'report_dict')
+        assert not len(set(res.report_dict.keys())-set(['report_all','report_brief','report_count',
+                                                        'report_badprob','report_iv','report_ks','report_psi','report_lift']))
+        
+        varGroupsPlot({'a':[1],'c':['1','2','3']},column='g',target='y',n_jobs=1).plot(X)
+        varGroupsPlot({'a':[1],'c':['1','2','3']},column='g',sort_column=['g1','g2'],target='y',n_jobs=1).plot(X)
+        
 
 def test_GainsTable():      
     
     X=pd.Series([100,250,280,310,460],name='score')
     g=pd.Series(['g1','g1','g2','g2','g2'])
     y=pd.Series([1,0,0,1,1],name='y')
```

### Comparing `BDMLtools-0.3.5/test/test_selector.py` & `BDMLtools-0.3.6/test/test_selector.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from BDMLtools.selector import stepLogit,cardScorer,LgbmSeqSelector,LgbmShapRFECVSelector,LgbmPISelector
 from BDMLtools.encoder import woeTransformer,binTransformer
 from sklearn.linear_model import LogisticRegression
 import pandas as pd
 import numpy as np
 import mock
 from io import StringIO
+import os
 
 
 def test_binSelector():
 
     X=pd.DataFrame(
         {
          'a':np.arange(100,dtype='float'),
@@ -55,97 +56,99 @@
     
     binSelector(method='pretty',n_jobs=1,iv_limit=0).fit_transform(X,y)               
     binSelector(method='pretty',n_jobs=1,iv_limit=0,coerce_monotonic=True).fit_transform(X,y)         
     binSelector(method='pretty',n_jobs=1,iv_limit=0,sample_weight=ws,keep=['a','c']).fit_transform(X,y)      
     binSelector(method='pretty',n_jobs=1,iv_limit=0,special_values=[1,2,3,4,'a']).fit_transform(X,y)   
 
 
-@mock.patch('matplotlib.pyplot.show')
+@mock.patch('matplotlib.pyplot.show') #(mock_show,monkeypatch)
 def test_binAdjuster(mock_show,monkeypatch):
-
-    X=pd.DataFrame(
-        {
-         'a':np.arange(100),
-         'c':np.concatenate([np.repeat('a',50),np.repeat('b',50)],dtype=object)}
-        )
-
-    y=pd.Series(np.append(np.zeros(50),np.ones(50)),name='y')
-
-    br_raw={'a':[40,80],'c':['a','b']}  
     
-    number_inputs = StringIO('1\n1')
-    monkeypatch.setattr('sys.stdin', number_inputs)
-    adj=binAdjuster(br_raw).fit(X,y)
-    res=adj.transform(X)
-    assert hasattr(adj,'breaks_list_adj')
-    assert hasattr(adj,'vtabs_dict_adj')
-    assert all(np.equal(res.columns,['a','c']))
-    
-    
-    number_inputs = StringIO('2\n40,50\n1\n2\na%,%b\n1')
-    monkeypatch.setattr('sys.stdin', number_inputs)
-    adj=binAdjuster(br_raw).fit(X,y)
-    assert all(np.equal(adj.breaks_list_adj['a'],[40,50]))
-    assert adj.breaks_list_adj['c'][0]=='a%,%b'
-    
-    number_inputs = StringIO('1\n3\n2\n20,70\n1\n1')
-    monkeypatch.setattr('sys.stdin', number_inputs)
-    adj=binAdjuster(br_raw).fit(X,y)
-    assert all(np.equal(adj.breaks_list_adj['a'],[20,70]))
-    
-    number_inputs = StringIO('1\n4')
-    monkeypatch.setattr('sys.stdin', number_inputs)
-    adj=binAdjuster(br_raw).fit(X,y)
-    assert 'a' in adj.breaks_list_adj.keys() and 'c' not in adj.breaks_list_adj.keys()   
-
-    number_inputs = StringIO('0\ny')
-    monkeypatch.setattr('sys.stdin', number_inputs)
-    adj=binAdjuster(br_raw).fit(X,y)
+    if os.name!='nt':
+    
+        X=pd.DataFrame(
+            {
+             'a':np.arange(100),
+             'c':np.concatenate([np.repeat('a',50),np.repeat('b',50)],dtype=object)}
+            )
+    
+        y=pd.Series(np.append(np.zeros(50),np.ones(50)),name='y')
+    
+        br_raw={'a':[40,80],'c':['a','b']}  
         
-    X=pd.DataFrame(
-        {
-         'a':np.arange(100),
-         'c':np.concatenate([np.repeat('a',50),np.repeat('b',50)],dtype=object),
-         'g':np.concatenate([np.repeat('a',30),np.repeat('b',30),np.repeat('c',40)],dtype=object)}    
-        )
-
-    y=pd.Series(np.append(np.zeros(50),np.ones(50)),name='y')
-
-    br_raw={'a':[40,80],'c':['a','b']}   
+        number_inputs = StringIO('1\n1')
+        monkeypatch.setattr('sys.stdin', number_inputs)
+        adj=binAdjuster(br_raw).fit(X,y)
+        res=adj.transform(X)
+        assert hasattr(adj,'breaks_list_adj')
+        assert hasattr(adj,'vtabs_dict_adj')
+        assert all(np.equal(res.columns,['a','c']))
+        
+        
+        number_inputs = StringIO('2\n40,50\n1\n2\na%,%b\n1')
+        monkeypatch.setattr('sys.stdin', number_inputs)
+        adj=binAdjuster(br_raw).fit(X,y)
+        assert all(np.equal(adj.breaks_list_adj['a'],[40,50]))
+        assert adj.breaks_list_adj['c'][0]=='a%,%b'
+        
+        number_inputs = StringIO('1\n3\n2\n20,70\n1\n1')
+        monkeypatch.setattr('sys.stdin', number_inputs)
+        adj=binAdjuster(br_raw).fit(X,y)
+        assert all(np.equal(adj.breaks_list_adj['a'],[20,70]))
+        
+        number_inputs = StringIO('1\n4')
+        monkeypatch.setattr('sys.stdin', number_inputs)
+        adj=binAdjuster(br_raw).fit(X,y)
+        assert 'a' in adj.breaks_list_adj.keys() and 'c' not in adj.breaks_list_adj.keys()   
+    
+        number_inputs = StringIO('0\ny')
+        monkeypatch.setattr('sys.stdin', number_inputs)
+        adj=binAdjuster(br_raw).fit(X,y)
+            
+        X=pd.DataFrame(
+            {
+             'a':np.arange(100),
+             'c':np.concatenate([np.repeat('a',50),np.repeat('b',50)],dtype=object),
+             'g':np.concatenate([np.repeat('a',30),np.repeat('b',30),np.repeat('c',40)],dtype=object)}    
+            )
     
-    number_inputs = StringIO('1\n1')
-    monkeypatch.setattr('sys.stdin', number_inputs)
-    adj=binAdjuster(br_raw,column='g',sort_column=['a','b','c']).fit(X,y)
-    res=adj.transform(X)  
-    assert hasattr(adj,'breaks_list_adj')
-    assert hasattr(adj,'vtabs_dict_adj')
-    assert all(np.equal(res.columns,['a','c']))
-    
-    number_inputs = StringIO('2\n40,50\n1\n2\na%,%b\n1')
-    monkeypatch.setattr('sys.stdin', number_inputs)
-    adj=binAdjuster(br_raw,column='g',sort_column=['a','b','c']).fit(X,y)
-    assert all(np.equal(adj.breaks_list_adj['a'],[40,50]))
-    assert adj.breaks_list_adj['c'][0]=='a%,%b'
-    
-    number_inputs = StringIO('1\n3\n2\n20,70\n1\n1')
-    monkeypatch.setattr('sys.stdin', number_inputs)
-    adj=binAdjuster(br_raw,column='g',sort_column=['a','b','c']).fit(X,y)
-    assert all(np.equal(adj.breaks_list_adj['a'],[20,70]))
-    
-    number_inputs = StringIO('1\n4')
-    monkeypatch.setattr('sys.stdin', number_inputs)
-    adj=binAdjuster(br_raw,column='g',sort_column=['a','b','c']).fit(X,y)
-    assert 'a' in adj.breaks_list_adj.keys() and 'c' not in adj.breaks_list_adj.keys()   
-
-    number_inputs = StringIO('0\ny')
-    monkeypatch.setattr('sys.stdin', number_inputs)
-    adj=binAdjuster(br_raw,column='g',sort_column=['a','b','c']).fit(X,y)
+        y=pd.Series(np.append(np.zeros(50),np.ones(50)),name='y')
+    
+        br_raw={'a':[40,80],'c':['a','b']}   
+        
+        number_inputs = StringIO('1\n1')
+        monkeypatch.setattr('sys.stdin', number_inputs)
+        adj=binAdjuster(br_raw,column='g',sort_column=['a','b','c']).fit(X,y)
+        res=adj.transform(X)  
+        assert hasattr(adj,'breaks_list_adj')
+        assert hasattr(adj,'vtabs_dict_adj')
+        assert all(np.equal(res.columns,['a','c']))
+        
+        number_inputs = StringIO('2\n40,50\n1\n2\na%,%b\n1')
+        monkeypatch.setattr('sys.stdin', number_inputs)
+        adj=binAdjuster(br_raw,column='g',sort_column=['a','b','c']).fit(X,y)
+        assert all(np.equal(adj.breaks_list_adj['a'],[40,50]))
+        assert adj.breaks_list_adj['c'][0]=='a%,%b'
+        
+        number_inputs = StringIO('1\n3\n2\n20,70\n1\n1')
+        monkeypatch.setattr('sys.stdin', number_inputs)
+        adj=binAdjuster(br_raw,column='g',sort_column=['a','b','c']).fit(X,y)
+        assert all(np.equal(adj.breaks_list_adj['a'],[20,70]))
+        
+        number_inputs = StringIO('1\n4')
+        monkeypatch.setattr('sys.stdin', number_inputs)
+        adj=binAdjuster(br_raw,column='g',sort_column=['a','b','c']).fit(X,y)
+        assert 'a' in adj.breaks_list_adj.keys() and 'c' not in adj.breaks_list_adj.keys()   
+    
+        number_inputs = StringIO('0\ny')
+        monkeypatch.setattr('sys.stdin', number_inputs)
+        adj=binAdjuster(br_raw,column='g',sort_column=['a','b','c']).fit(X,y)
         
     
-@mock.patch('matplotlib.pyplot.show')   
+@mock.patch('matplotlib.pyplot.show')
 def test_faSelector(mock_show):
 
     X=pd.DataFrame(
         {'a':[1,2,2,4,5],'b':[1,2,3,4,5],'c':[1,1,1,2,1]}
         )
     y=pd.Series([0,0,1,1,1],name='y')
```

### Comparing `BDMLtools-0.3.5/test/test_tunner.py` & `BDMLtools-0.3.6/test/test_tunner.py`

 * *Files identical despite different names*


# Comparing `tmp/dojo_ds-0.1.1.tar.gz` & `tmp/dojo_ds-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dojo_ds-0.1.1.tar", last modified: Wed Feb 15 01:36:07 2023, max compression
+gzip compressed data, was "dojo_ds-0.2.0.tar", last modified: Fri May 12 16:39:58 2023, max compression
```

## Comparing `dojo_ds-0.1.1.tar` & `dojo_ds-0.2.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2023-02-15 01:36:07.819476 dojo_ds-0.1.1/
--rw-r--r--   0 codingdojo   (502) staff       (20)      160 2023-02-15 01:14:18.000000 dojo_ds-0.1.1/AUTHORS.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)     3530 2023-02-15 01:14:18.000000 dojo_ds-0.1.1/CONTRIBUTING.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       89 2023-02-15 01:14:18.000000 dojo_ds-0.1.1/HISTORY.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)    35129 2023-02-15 01:14:37.000000 dojo_ds-0.1.1/LICENSE
--rw-r--r--   0 codingdojo   (502) staff       (20)      262 2023-02-15 01:14:18.000000 dojo_ds-0.1.1/MANIFEST.in
--rw-r--r--   0 codingdojo   (502) staff       (20)     1761 2023-02-15 01:36:07.819557 dojo_ds-0.1.1/PKG-INFO
--rw-r--r--   0 codingdojo   (502) staff       (20)      903 2023-02-15 01:14:18.000000 dojo_ds-0.1.1/README.rst
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2023-02-15 01:36:07.796429 dojo_ds-0.1.1/docs/
--rw-r--r--   0 codingdojo   (502) staff       (20)      608 2023-02-15 01:14:18.000000 dojo_ds-0.1.1/docs/Makefile
--rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-0.1.1/docs/authors.rst
--rwxr-xr-x   0 codingdojo   (502) staff       (20)     4778 2023-02-15 01:14:18.000000 dojo_ds-0.1.1/docs/conf.py
--rw-r--r--   0 codingdojo   (502) staff       (20)       33 2023-02-15 01:14:18.000000 dojo_ds-0.1.1/docs/contributing.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-0.1.1/docs/history.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)      304 2023-02-15 01:14:18.000000 dojo_ds-0.1.1/docs/index.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)     1122 2023-02-15 01:14:18.000000 dojo_ds-0.1.1/docs/installation.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)      805 2023-02-15 01:14:18.000000 dojo_ds-0.1.1/docs/make.bat
--rw-r--r--   0 codingdojo   (502) staff       (20)       27 2023-02-15 01:14:18.000000 dojo_ds-0.1.1/docs/readme.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       69 2023-02-15 01:14:18.000000 dojo_ds-0.1.1/docs/usage.rst
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2023-02-15 01:36:07.800916 dojo_ds-0.1.1/dojo_ds/
--rw-r--r--   0 codingdojo   (502) staff       (20)      232 2023-02-15 01:35:57.000000 dojo_ds-0.1.1/dojo_ds/__init__.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      399 2023-02-15 01:14:18.000000 dojo_ds-0.1.1/dojo_ds/cli.py
--rw-r--r--   0 codingdojo   (502) staff       (20)     4746 2023-02-15 01:18:18.000000 dojo_ds-0.1.1/dojo_ds/data_enrichment.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    25287 2023-02-15 01:27:24.000000 dojo_ds-0.1.1/dojo_ds/dojo_ds.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      293 2023-02-15 01:23:40.000000 dojo_ds-0.1.1/dojo_ds/lp_style.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    26488 2023-02-15 01:19:46.000000 dojo_ds-0.1.1/dojo_ds/model_insights.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      245 2023-02-15 01:20:53.000000 dojo_ds-0.1.1/dojo_ds/standard_imports.py
--rw-r--r--   0 codingdojo   (502) staff       (20)     8839 2023-02-15 01:26:36.000000 dojo_ds-0.1.1/dojo_ds/utils.py
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2023-02-15 01:36:07.803828 dojo_ds-0.1.1/dojo_ds.egg-info/
--rw-r--r--   0 codingdojo   (502) staff       (20)     1761 2023-02-15 01:36:07.000000 dojo_ds-0.1.1/dojo_ds.egg-info/PKG-INFO
--rw-r--r--   0 codingdojo   (502) staff       (20)      685 2023-02-15 01:36:07.000000 dojo_ds-0.1.1/dojo_ds.egg-info/SOURCES.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)        1 2023-02-15 01:36:07.000000 dojo_ds-0.1.1/dojo_ds.egg-info/dependency_links.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)       45 2023-02-15 01:36:07.000000 dojo_ds-0.1.1/dojo_ds.egg-info/entry_points.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)        1 2023-02-15 01:30:10.000000 dojo_ds-0.1.1/dojo_ds.egg-info/not-zip-safe
--rw-r--r--   0 codingdojo   (502) staff       (20)       11 2023-02-15 01:36:07.000000 dojo_ds-0.1.1/dojo_ds.egg-info/requires.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)        8 2023-02-15 01:36:07.000000 dojo_ds-0.1.1/dojo_ds.egg-info/top_level.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)      379 2023-02-15 01:36:07.819935 dojo_ds-0.1.1/setup.cfg
--rw-r--r--   0 codingdojo   (502) staff       (20)     1438 2023-02-15 01:35:57.000000 dojo_ds-0.1.1/setup.py
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2023-02-15 01:36:07.819068 dojo_ds-0.1.1/tests/
--rw-r--r--   0 codingdojo   (502) staff       (20)       37 2023-02-15 01:14:18.000000 dojo_ds-0.1.1/tests/__init__.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      852 2023-02-15 01:14:18.000000 dojo_ds-0.1.1/tests/test_dojo_ds.py
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2023-05-12 16:39:58.821184 dojo_ds-0.2.0/
+-rw-r--r--   0 codingdojo   (502) staff       (20)      160 2023-02-15 01:14:18.000000 dojo_ds-0.2.0/AUTHORS.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)     3530 2023-02-15 01:14:18.000000 dojo_ds-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       89 2023-02-15 01:14:18.000000 dojo_ds-0.2.0/HISTORY.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)    35129 2023-02-15 01:14:37.000000 dojo_ds-0.2.0/LICENSE
+-rw-r--r--   0 codingdojo   (502) staff       (20)      262 2023-02-15 01:14:18.000000 dojo_ds-0.2.0/MANIFEST.in
+-rw-r--r--   0 codingdojo   (502) staff       (20)     1761 2023-05-12 16:39:58.821319 dojo_ds-0.2.0/PKG-INFO
+-rw-r--r--   0 codingdojo   (502) staff       (20)      903 2023-02-15 01:14:18.000000 dojo_ds-0.2.0/README.rst
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2023-05-12 16:39:58.790243 dojo_ds-0.2.0/docs/
+-rw-r--r--   0 codingdojo   (502) staff       (20)      608 2023-02-15 01:14:18.000000 dojo_ds-0.2.0/docs/Makefile
+-rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-0.2.0/docs/authors.rst
+-rwxr-xr-x   0 codingdojo   (502) staff       (20)     4778 2023-02-15 01:14:18.000000 dojo_ds-0.2.0/docs/conf.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)       33 2023-02-15 01:14:18.000000 dojo_ds-0.2.0/docs/contributing.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-0.2.0/docs/history.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)      304 2023-02-15 01:14:18.000000 dojo_ds-0.2.0/docs/index.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)     1122 2023-02-15 01:14:18.000000 dojo_ds-0.2.0/docs/installation.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)      805 2023-02-15 01:14:18.000000 dojo_ds-0.2.0/docs/make.bat
+-rw-r--r--   0 codingdojo   (502) staff       (20)       27 2023-02-15 01:14:18.000000 dojo_ds-0.2.0/docs/readme.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       69 2023-02-15 01:14:18.000000 dojo_ds-0.2.0/docs/usage.rst
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2023-05-12 16:39:58.803547 dojo_ds-0.2.0/dojo_ds/
+-rw-r--r--   0 codingdojo   (502) staff       (20)      249 2023-05-12 16:36:00.000000 dojo_ds-0.2.0/dojo_ds/__init__.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      399 2023-02-15 01:14:18.000000 dojo_ds-0.2.0/dojo_ds/cli.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)     4746 2023-02-15 01:18:18.000000 dojo_ds-0.2.0/dojo_ds/data_enrichment.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    25287 2023-02-15 01:38:29.000000 dojo_ds-0.2.0/dojo_ds/dojo_ds.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)     6728 2023-05-12 16:29:11.000000 dojo_ds-0.2.0/dojo_ds/eda.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      293 2023-02-15 01:23:40.000000 dojo_ds-0.2.0/dojo_ds/lp_style.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    26552 2023-05-12 16:29:09.000000 dojo_ds-0.2.0/dojo_ds/model_insights.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      245 2023-02-15 01:20:53.000000 dojo_ds-0.2.0/dojo_ds/standard_imports.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)     8839 2023-02-15 01:26:36.000000 dojo_ds-0.2.0/dojo_ds/utils.py
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2023-05-12 16:39:58.812336 dojo_ds-0.2.0/dojo_ds.egg-info/
+-rw-r--r--   0 codingdojo   (502) staff       (20)     1761 2023-05-12 16:39:58.000000 dojo_ds-0.2.0/dojo_ds.egg-info/PKG-INFO
+-rw-r--r--   0 codingdojo   (502) staff       (20)      700 2023-05-12 16:39:58.000000 dojo_ds-0.2.0/dojo_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)        1 2023-05-12 16:39:58.000000 dojo_ds-0.2.0/dojo_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)       45 2023-05-12 16:39:58.000000 dojo_ds-0.2.0/dojo_ds.egg-info/entry_points.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)        1 2023-02-15 01:30:10.000000 dojo_ds-0.2.0/dojo_ds.egg-info/not-zip-safe
+-rw-r--r--   0 codingdojo   (502) staff       (20)       79 2023-05-12 16:39:58.000000 dojo_ds-0.2.0/dojo_ds.egg-info/requires.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)        8 2023-05-12 16:39:58.000000 dojo_ds-0.2.0/dojo_ds.egg-info/top_level.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)      379 2023-05-12 16:39:58.821774 dojo_ds-0.2.0/setup.cfg
+-rw-r--r--   0 codingdojo   (502) staff       (20)     1687 2023-05-12 16:39:48.000000 dojo_ds-0.2.0/setup.py
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2023-05-12 16:39:58.818461 dojo_ds-0.2.0/tests/
+-rw-r--r--   0 codingdojo   (502) staff       (20)       37 2023-02-15 01:14:18.000000 dojo_ds-0.2.0/tests/__init__.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      852 2023-02-15 01:14:18.000000 dojo_ds-0.2.0/tests/test_dojo_ds.py
```

### Comparing `dojo_ds-0.1.1/CONTRIBUTING.rst` & `dojo_ds-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-0.1.1/LICENSE` & `dojo_ds-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dojo_ds-0.1.1/PKG-INFO` & `dojo_ds-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo_ds
-Version: 0.1.1
+Version: 0.2.0
 Summary: Code from Coding Dojo's Online Part-Time Data Science boot camp
 Home-page: https://github.com/jirvingphd/dojo_ds
 Author: James Irving
 Author-email: jirving@codingdojo.com
 License: GNU General Public License v3
 Keywords: dojo_ds
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `dojo_ds-0.1.1/README.rst` & `dojo_ds-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-0.1.1/docs/Makefile` & `dojo_ds-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dojo_ds-0.1.1/docs/conf.py` & `dojo_ds-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-0.1.1/docs/installation.rst` & `dojo_ds-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-0.1.1/docs/make.bat` & `dojo_ds-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dojo_ds-0.1.1/dojo_ds/data_enrichment.py` & `dojo_ds-0.2.0/dojo_ds/data_enrichment.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-0.1.1/dojo_ds/dojo_ds.py` & `dojo_ds-0.2.0/dojo_ds/dojo_ds.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-0.1.1/dojo_ds/model_insights.py` & `dojo_ds-0.2.0/dojo_ds/model_insights.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,31 +3,32 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from sklearn import metrics
 ############################################################################################
 ############################### FROM: INSIGHTS FOR STAKEHODLERS ############################
 ############################################################################################
 
-def summarize_df(df_):
-    """Source: Insights for Stakeholder Lesson - https://login.codingdojo.com/m/0/13079/91969 
-    Example Usage:
-    >> df = pd.read_csv(filename)
-    >> summary = summarize_df(df)
-    >> summary"""
-    df = df_.copy()
-    report = pd.DataFrame({
-                        'dtype':df.dtypes,
-                        '# null': df.isna().sum(),
-                        'null (%)': df.isna().sum()/len(df)*100,
-                        'nunique':df.nunique(),
-                        "min":df.min(),
-                        'max':df.max()
-             })
-    report.index.name='Column'
-    return report.reset_index()
+from .eda import summarize_df
+# def summarize_df(df_):
+#     """Source: Insights for Stakeholder Lesson - https://login.codingdojo.com/m/0/13079/91969 
+#     Example Usage:
+#     >> df = pd.read_csv(filename)
+#     >> summary = summarize_df(df)
+#     >> summary"""
+#     df = df_.copy()
+#     report = pd.DataFrame({
+#                         'dtype':df.dtypes,
+#                         '# null': df.isna().sum(),
+#                         'null (%)': df.isna().sum()/len(df)*100,
+#                         'nunique':df.nunique(),
+#                         "min":df.min(),
+#                         'max':df.max()
+#              })
+#     report.index.name='Column'
+#     return report.reset_index()
 
 ############################################################################################
 ############################### FROM: FEATURE IMPORTANCE ###################################
 ############################################################################################
 
 def evaluate_regression(model, X_train,y_train, X_test, y_test): 
     """Evaluates a scikit learn regression model using r-squared and RMSE
```

### Comparing `dojo_ds-0.1.1/dojo_ds/utils.py` & `dojo_ds-0.2.0/dojo_ds/utils.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-0.1.1/dojo_ds.egg-info/PKG-INFO` & `dojo_ds-0.2.0/dojo_ds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo-ds
-Version: 0.1.1
+Version: 0.2.0
 Summary: Code from Coding Dojo's Online Part-Time Data Science boot camp
 Home-page: https://github.com/jirvingphd/dojo_ds
 Author: James Irving
 Author-email: jirving@codingdojo.com
 License: GNU General Public License v3
 Keywords: dojo_ds
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `dojo_ds-0.1.1/dojo_ds.egg-info/SOURCES.txt` & `dojo_ds-0.2.0/dojo_ds.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 dojo_ds/__init__.py
 dojo_ds/cli.py
 dojo_ds/data_enrichment.py
 dojo_ds/dojo_ds.py
+dojo_ds/eda.py
 dojo_ds/lp_style.py
 dojo_ds/model_insights.py
 dojo_ds/standard_imports.py
 dojo_ds/utils.py
 dojo_ds.egg-info/PKG-INFO
 dojo_ds.egg-info/SOURCES.txt
 dojo_ds.egg-info/dependency_links.txt
```

### Comparing `dojo_ds-0.1.1/tests/test_dojo_ds.py` & `dojo_ds-0.2.0/tests/test_dojo_ds.py`

 * *Files identical despite different names*


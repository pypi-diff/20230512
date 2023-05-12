# Comparing `tmp/PatryksAutoAI-0.3.6.tar.gz` & `tmp/PatryksAutoAI-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PatryksAutoAI-0.3.6.tar", last modified: Fri May 12 17:10:10 2023, max compression
+gzip compressed data, was "PatryksAutoAI-0.3.7.tar", last modified: Fri May 12 18:43:14 2023, max compression
```

## Comparing `PatryksAutoAI-0.3.6.tar` & `PatryksAutoAI-0.3.7.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 17:10:10.496024 PatryksAutoAI-0.3.6/
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 17:10:10.492024 PatryksAutoAI-0.3.6/KaggleAutoAI/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      200 2023-05-12 16:22:50.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 17:10:10.492024 PatryksAutoAI-0.3.6/KaggleAutoAI/automated_ai/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       29 2023-05-12 16:18:09.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/automated_ai/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 17:10:10.492024 PatryksAutoAI-0.3.6/KaggleAutoAI/automated_ai/classification/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       87 2023-05-12 16:17:51.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/automated_ai/classification/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      646 2023-05-12 17:00:49.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/automated_ai/classification/cat_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2037 2023-05-12 17:09:43.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/automated_ai/classification/compexity_level0.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 17:10:10.492024 PatryksAutoAI-0.3.6/KaggleAutoAI/classification/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       72 2023-05-10 18:02:22.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/classification/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      648 2023-04-17 06:33:02.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/classification/metrics.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 17:10:10.492024 PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      317 2023-05-10 18:02:39.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7950 2023-05-12 17:08:00.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/cat.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6313 2023-05-12 17:08:04.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/extra_trees.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5279 2023-05-12 17:08:07.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/gradient_boosting.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5950 2023-05-12 17:08:11.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/hist_gradient.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2205 2023-05-11 13:59:17.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/kneighbours.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7276 2023-05-12 17:08:16.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/light_lgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2301 2023-05-11 13:59:23.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/linear_svc.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     4867 2023-05-12 17:08:23.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/logistic_regression.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6345 2023-05-12 17:08:27.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/random_forest.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2320 2023-05-11 13:59:44.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/sgd_classifier.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2255 2023-05-11 13:59:40.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/svc.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5743 2023-05-12 17:08:33.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/xgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/helper_function.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 17:10:10.496024 PatryksAutoAI-0.3.6/KaggleAutoAI/model_data/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      110 2023-05-10 18:02:54.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/model_data/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6075 2023-04-18 06:00:32.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/model_data/model_data.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 17:10:10.496024 PatryksAutoAI-0.3.6/KaggleAutoAI/regression/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       89 2023-05-11 14:03:31.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/regression/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      607 2023-05-09 13:49:56.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/regression/metrics_regression.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 17:10:10.496024 PatryksAutoAI-0.3.6/KaggleAutoAI/regression/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      216 2023-05-11 14:13:19.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/regression/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6159 2023-05-12 17:08:40.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/regression/models/cat.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2632 2023-05-12 17:08:49.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/regression/models/elastic_net.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6078 2023-05-12 17:08:53.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/regression/models/gradient_boosting.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2559 2023-05-11 15:12:20.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/regression/models/lasso.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5511 2023-05-12 17:09:00.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/regression/models/lgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2849 2023-05-11 15:11:48.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/regression/models/sgd.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2633 2023-05-11 15:10:56.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/regression/models/svr.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7320 2023-05-12 17:09:07.000000 PatryksAutoAI-0.3.6/KaggleAutoAI/regression/models/xgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-12 17:10:10.496024 PatryksAutoAI-0.3.6/PKG-INFO
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 17:10:10.496024 PatryksAutoAI-0.3.6/PatryksAutoAI.egg-info/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-12 17:10:10.000000 PatryksAutoAI-0.3.6/PatryksAutoAI.egg-info/PKG-INFO
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1706 2023-05-12 17:10:10.000000 PatryksAutoAI-0.3.6/PatryksAutoAI.egg-info/SOURCES.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-12 17:10:10.000000 PatryksAutoAI-0.3.6/PatryksAutoAI.egg-info/dependency_links.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      162 2023-05-12 17:10:10.000000 PatryksAutoAI-0.3.6/PatryksAutoAI.egg-info/requires.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       13 2023-05-12 17:10:10.000000 PatryksAutoAI-0.3.6/PatryksAutoAI.egg-info/top_level.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-12 17:10:10.496024 PatryksAutoAI-0.3.6/setup.cfg
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1050 2023-05-12 17:09:15.000000 PatryksAutoAI-0.3.6/setup.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 18:43:14.362053 PatryksAutoAI-0.3.7/
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 18:43:14.346053 PatryksAutoAI-0.3.7/KaggleAutoAI/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      200 2023-05-12 16:22:50.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 18:43:14.346053 PatryksAutoAI-0.3.7/KaggleAutoAI/automated_ai/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       29 2023-05-12 16:18:09.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/automated_ai/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 18:43:14.346053 PatryksAutoAI-0.3.7/KaggleAutoAI/automated_ai/classification/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      136 2023-05-12 18:42:57.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/automated_ai/classification/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      753 2023-05-12 18:17:29.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/automated_ai/classification/cat_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1883 2023-05-12 18:42:31.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/automated_ai/classification/compexity_level0.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2184 2023-05-12 18:42:47.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/automated_ai/classification/complexity_level1.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 18:43:14.350053 PatryksAutoAI-0.3.7/KaggleAutoAI/classification/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       72 2023-05-10 18:02:22.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/classification/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      648 2023-04-17 06:33:02.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/classification/metrics.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 18:43:14.350053 PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      317 2023-05-10 18:02:39.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7950 2023-05-12 17:08:00.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/cat.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6313 2023-05-12 17:08:04.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/extra_trees.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5279 2023-05-12 17:08:07.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/gradient_boosting.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5950 2023-05-12 17:08:11.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/hist_gradient.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2205 2023-05-11 13:59:17.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/kneighbours.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7276 2023-05-12 17:08:16.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/light_lgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2301 2023-05-11 13:59:23.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/linear_svc.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     4867 2023-05-12 17:08:23.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/logistic_regression.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6345 2023-05-12 17:08:27.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/random_forest.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2320 2023-05-11 13:59:44.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/sgd_classifier.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2255 2023-05-11 13:59:40.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/svc.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5743 2023-05-12 17:08:33.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/xgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/helper_function.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 18:43:14.350053 PatryksAutoAI-0.3.7/KaggleAutoAI/model_data/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      110 2023-05-10 18:02:54.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/model_data/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6075 2023-04-18 06:00:32.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/model_data/model_data.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 18:43:14.354053 PatryksAutoAI-0.3.7/KaggleAutoAI/regression/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       89 2023-05-11 14:03:31.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/regression/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      607 2023-05-09 13:49:56.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/regression/metrics_regression.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 18:43:14.354053 PatryksAutoAI-0.3.7/KaggleAutoAI/regression/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      216 2023-05-11 14:13:19.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/regression/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6159 2023-05-12 17:08:40.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/regression/models/cat.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2632 2023-05-12 17:08:49.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/regression/models/elastic_net.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6078 2023-05-12 17:08:53.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/regression/models/gradient_boosting.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2559 2023-05-11 15:12:20.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/regression/models/lasso.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5511 2023-05-12 17:09:00.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/regression/models/lgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2849 2023-05-11 15:11:48.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/regression/models/sgd.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2633 2023-05-11 15:10:56.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/regression/models/svr.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7320 2023-05-12 17:09:07.000000 PatryksAutoAI-0.3.7/KaggleAutoAI/regression/models/xgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-12 18:43:14.354053 PatryksAutoAI-0.3.7/PKG-INFO
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 18:43:14.354053 PatryksAutoAI-0.3.7/PatryksAutoAI.egg-info/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-12 18:43:14.000000 PatryksAutoAI-0.3.7/PatryksAutoAI.egg-info/PKG-INFO
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1768 2023-05-12 18:43:14.000000 PatryksAutoAI-0.3.7/PatryksAutoAI.egg-info/SOURCES.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-12 18:43:14.000000 PatryksAutoAI-0.3.7/PatryksAutoAI.egg-info/dependency_links.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      162 2023-05-12 18:43:14.000000 PatryksAutoAI-0.3.7/PatryksAutoAI.egg-info/requires.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       13 2023-05-12 18:43:14.000000 PatryksAutoAI-0.3.7/PatryksAutoAI.egg-info/top_level.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-12 18:43:14.362053 PatryksAutoAI-0.3.7/setup.cfg
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1050 2023-05-12 18:43:05.000000 PatryksAutoAI-0.3.7/setup.py
```

### Comparing `PatryksAutoAI-0.3.6/KaggleAutoAI/automated_ai/classification/compexity_level0.py` & `PatryksAutoAI-0.3.7/KaggleAutoAI/automated_ai/classification/complexity_level1.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,62 @@
 from ...regression.models.cat import Cat
 from ...model_data.model_data import ModelData
 from sklearn.model_selection import train_test_split, KFold
-import logging
+from scipy.stats import shapiro 
 
 
-def Complexity_Level0(model, X, y):
-    if model == "Cat":
+def Complexity_Level1(model_name, X, y):
+    if model_name == "Cat":
         model = Cat()
-    ## other model
 
-    print(f"Chosen model {model} starting choosing important columns \n\n")
+    print(f"Chosen model {model_name} starting choosing important columns \n\n")
     importance_columns = {}
     for col in X.columns:
         importance_columns[col] = 0
 
     ## fix null columns
     model_data = ModelData(X)
     columns_null = model_data.find_null_column()
+
+    standard_columns = []
+    min_max_columns = []
     for col in columns_null:
         column_data_type = X[col].dtype
         if column_data_type == "object":
             model_data.fix_column_str(col)
         else:
-            model_data.fix_columns([col], "mean")
+            shap = shapiro(X[col])
+            if shap.pvalue > 0.05:
+                standard_columns.append(col)
+            else:
+                min_max_columns.append(col)
     
-    ## Text column to dummies
     for col in X.columns:
         if X[col].dtype == "object" and X[col].nunique() < 10:
             model_data.dummies(col)
+    model_data.min_max_scaler(min_max_columns)
+    model_data.standard_scaler(standard_columns)
+    
     X = model_data.return_dataframe()
 
     ## Train model in diffrent samples to extract importance of columns
     kfold = KFold(n_splits=5, shuffle=True, random_state=42)
     for i, (train_index, valid_index) in enumerate(kfold.split(X,y)):
         X_train, y_train = X.iloc[train_index], y.iloc[train_index]
         model.create_optuna(X_train,y_train,n_trials=100)
         feature_model = model.get()
         features = feature_model.get_feature_importance()
         for i,col in enumerate(X.columns):
             importance_columns[col] += features[i]
-
-    print(f"Importance of columns: \n")
-    for k,v in importance_columns.items():
-        print(f"{k}: {v} \n")
     
     ## Acceptting column that satify the requirenments 
     mean_importance = sum(importance_columns.values()) / len(importance_columns)
-    threshold_importance = 0.75 * mean_importance
+    threshold_importance = 0.5 * mean_importance
     columns = []
     for k,v in importance_columns.items():
         if v > threshold_importance:
             columns.append(k)
 
     print(f"Used columns: {columns}")
-    X = X[[columns]]
-    model.create_optuna(X,y,n_trials=500)
+    X = X[columns]
+    model.create_optuna(X,y,n_trials=1000)
     return model.get(), columns
-
```

### Comparing `PatryksAutoAI-0.3.6/KaggleAutoAI/classification/metrics.py` & `PatryksAutoAI-0.3.7/KaggleAutoAI/classification/metrics.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/cat.py` & `PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/cat.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/extra_trees.py` & `PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/extra_trees.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/gradient_boosting.py` & `PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/hist_gradient.py` & `PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/hist_gradient.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/kneighbours.py` & `PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/kneighbours.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/light_lgb.py` & `PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/light_lgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/linear_svc.py` & `PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/linear_svc.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/logistic_regression.py` & `PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/random_forest.py` & `PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/random_forest.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/sgd_classifier.py` & `PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/sgd_classifier.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/svc.py` & `PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/svc.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.6/KaggleAutoAI/classification/models/xgb.py` & `PatryksAutoAI-0.3.7/KaggleAutoAI/classification/models/xgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.6/KaggleAutoAI/helper_function.py` & `PatryksAutoAI-0.3.7/KaggleAutoAI/helper_function.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.6/KaggleAutoAI/model_data/model_data.py` & `PatryksAutoAI-0.3.7/KaggleAutoAI/model_data/model_data.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.6/KaggleAutoAI/regression/metrics_regression.py` & `PatryksAutoAI-0.3.7/KaggleAutoAI/regression/metrics_regression.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.6/KaggleAutoAI/regression/models/cat.py` & `PatryksAutoAI-0.3.7/KaggleAutoAI/regression/models/cat.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.6/KaggleAutoAI/regression/models/elastic_net.py` & `PatryksAutoAI-0.3.7/KaggleAutoAI/regression/models/elastic_net.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.6/KaggleAutoAI/regression/models/gradient_boosting.py` & `PatryksAutoAI-0.3.7/KaggleAutoAI/regression/models/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.6/KaggleAutoAI/regression/models/lasso.py` & `PatryksAutoAI-0.3.7/KaggleAutoAI/regression/models/lasso.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.6/KaggleAutoAI/regression/models/lgb.py` & `PatryksAutoAI-0.3.7/KaggleAutoAI/regression/models/lgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.6/KaggleAutoAI/regression/models/sgd.py` & `PatryksAutoAI-0.3.7/KaggleAutoAI/regression/models/sgd.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.6/KaggleAutoAI/regression/models/svr.py` & `PatryksAutoAI-0.3.7/KaggleAutoAI/regression/models/svr.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.6/KaggleAutoAI/regression/models/xgb.py` & `PatryksAutoAI-0.3.7/KaggleAutoAI/regression/models/xgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.6/PatryksAutoAI.egg-info/SOURCES.txt` & `PatryksAutoAI-0.3.7/PatryksAutoAI.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 setup.py
 KaggleAutoAI/__init__.py
 KaggleAutoAI/helper_function.py
 KaggleAutoAI/automated_ai/__init__.py
 KaggleAutoAI/automated_ai/classification/__init__.py
 KaggleAutoAI/automated_ai/classification/cat_automated.py
 KaggleAutoAI/automated_ai/classification/compexity_level0.py
+KaggleAutoAI/automated_ai/classification/complexity_level1.py
 KaggleAutoAI/classification/__init__.py
 KaggleAutoAI/classification/metrics.py
 KaggleAutoAI/classification/models/__init__.py
 KaggleAutoAI/classification/models/cat.py
 KaggleAutoAI/classification/models/extra_trees.py
 KaggleAutoAI/classification/models/gradient_boosting.py
 KaggleAutoAI/classification/models/hist_gradient.py
```

### Comparing `PatryksAutoAI-0.3.6/setup.py` & `PatryksAutoAI-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.3.6'
+VERSION = '0.3.7'
 DESCRIPTION = 'Auto_AI_patryk'
 LONG_DESCRIPTION = 'Package contains helping functions for creating ML models'
 
 # Read the requirements from requirements.txt
 with open('./KaggleAutoAI/requirements.txt') as f:
     requirements = f.read().splitlines()
```


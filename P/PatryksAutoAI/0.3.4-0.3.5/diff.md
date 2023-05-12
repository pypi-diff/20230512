# Comparing `tmp/PatryksAutoAI-0.3.4.tar.gz` & `tmp/PatryksAutoAI-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PatryksAutoAI-0.3.4.tar", last modified: Fri May 12 16:36:52 2023, max compression
+gzip compressed data, was "PatryksAutoAI-0.3.5.tar", last modified: Fri May 12 16:51:29 2023, max compression
```

## Comparing `PatryksAutoAI-0.3.4.tar` & `PatryksAutoAI-0.3.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 16:36:52.824614 PatryksAutoAI-0.3.4/
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 16:36:52.816614 PatryksAutoAI-0.3.4/KaggleAutoAI/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      200 2023-05-12 16:22:50.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 16:36:52.816614 PatryksAutoAI-0.3.4/KaggleAutoAI/automated_ai/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       29 2023-05-12 16:18:09.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/automated_ai/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 16:36:52.816614 PatryksAutoAI-0.3.4/KaggleAutoAI/automated_ai/classification/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       87 2023-05-12 16:17:51.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/automated_ai/classification/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      588 2023-05-12 16:26:44.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/automated_ai/classification/cat_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1797 2023-05-12 16:36:32.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/automated_ai/classification/compexity_level0.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 16:36:52.816614 PatryksAutoAI-0.3.4/KaggleAutoAI/classification/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       72 2023-05-10 18:02:22.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/classification/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      648 2023-04-17 06:33:02.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/classification/metrics.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 16:36:52.820614 PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      317 2023-05-10 18:02:39.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7909 2023-05-11 13:58:25.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/cat.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6273 2023-05-11 13:59:08.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/extra_trees.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5238 2023-05-11 13:59:11.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/gradient_boosting.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5909 2023-05-11 13:59:15.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/hist_gradient.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2205 2023-05-11 13:59:17.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/kneighbours.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7234 2023-05-11 13:59:20.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/light_lgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2301 2023-05-11 13:59:23.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/linear_svc.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     4826 2023-05-11 13:59:26.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/logistic_regression.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6304 2023-05-11 13:59:30.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/random_forest.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2320 2023-05-11 13:59:44.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/sgd_classifier.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2255 2023-05-11 13:59:40.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/svc.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5702 2023-05-11 13:59:04.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/xgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/helper_function.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 16:36:52.820614 PatryksAutoAI-0.3.4/KaggleAutoAI/model_data/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      110 2023-05-10 18:02:54.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/model_data/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6075 2023-04-18 06:00:32.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/model_data/model_data.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 16:36:52.820614 PatryksAutoAI-0.3.4/KaggleAutoAI/regression/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       89 2023-05-11 14:03:31.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/regression/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      607 2023-05-09 13:49:56.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/regression/metrics_regression.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 16:36:52.824614 PatryksAutoAI-0.3.4/KaggleAutoAI/regression/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      216 2023-05-11 14:13:19.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/regression/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6118 2023-05-11 15:13:02.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/regression/models/cat.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2631 2023-05-11 15:12:58.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/regression/models/elastic_net.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6037 2023-05-11 15:12:23.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/regression/models/gradient_boosting.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2559 2023-05-11 15:12:20.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/regression/models/lasso.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5469 2023-05-11 15:11:54.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/regression/models/lgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2849 2023-05-11 15:11:48.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/regression/models/sgd.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2633 2023-05-11 15:10:56.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/regression/models/svr.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7278 2023-05-11 15:10:54.000000 PatryksAutoAI-0.3.4/KaggleAutoAI/regression/models/xgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-12 16:36:52.824614 PatryksAutoAI-0.3.4/PKG-INFO
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 16:36:52.824614 PatryksAutoAI-0.3.4/PatryksAutoAI.egg-info/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-12 16:36:52.000000 PatryksAutoAI-0.3.4/PatryksAutoAI.egg-info/PKG-INFO
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1706 2023-05-12 16:36:52.000000 PatryksAutoAI-0.3.4/PatryksAutoAI.egg-info/SOURCES.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-12 16:36:52.000000 PatryksAutoAI-0.3.4/PatryksAutoAI.egg-info/dependency_links.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      162 2023-05-12 16:36:52.000000 PatryksAutoAI-0.3.4/PatryksAutoAI.egg-info/requires.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       13 2023-05-12 16:36:52.000000 PatryksAutoAI-0.3.4/PatryksAutoAI.egg-info/top_level.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-12 16:36:52.824614 PatryksAutoAI-0.3.4/setup.cfg
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1050 2023-05-12 16:36:38.000000 PatryksAutoAI-0.3.4/setup.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 16:51:29.563036 PatryksAutoAI-0.3.5/
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 16:51:29.559036 PatryksAutoAI-0.3.5/KaggleAutoAI/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      200 2023-05-12 16:22:50.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 16:51:29.559036 PatryksAutoAI-0.3.5/KaggleAutoAI/automated_ai/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       29 2023-05-12 16:18:09.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/automated_ai/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 16:51:29.559036 PatryksAutoAI-0.3.5/KaggleAutoAI/automated_ai/classification/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       87 2023-05-12 16:17:51.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/automated_ai/classification/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      588 2023-05-12 16:26:44.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/automated_ai/classification/cat_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2091 2023-05-12 16:51:18.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/automated_ai/classification/compexity_level0.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 16:51:29.559036 PatryksAutoAI-0.3.5/KaggleAutoAI/classification/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       72 2023-05-10 18:02:22.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/classification/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      648 2023-04-17 06:33:02.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/classification/metrics.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 16:51:29.559036 PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      317 2023-05-10 18:02:39.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7909 2023-05-11 13:58:25.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/cat.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6273 2023-05-11 13:59:08.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/extra_trees.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5238 2023-05-11 13:59:11.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/gradient_boosting.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5909 2023-05-11 13:59:15.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/hist_gradient.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2205 2023-05-11 13:59:17.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/kneighbours.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7234 2023-05-11 13:59:20.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/light_lgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2301 2023-05-11 13:59:23.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/linear_svc.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     4826 2023-05-11 13:59:26.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/logistic_regression.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6304 2023-05-11 13:59:30.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/random_forest.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2320 2023-05-11 13:59:44.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/sgd_classifier.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2255 2023-05-11 13:59:40.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/svc.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5702 2023-05-11 13:59:04.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/xgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/helper_function.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 16:51:29.559036 PatryksAutoAI-0.3.5/KaggleAutoAI/model_data/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      110 2023-05-10 18:02:54.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/model_data/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6075 2023-04-18 06:00:32.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/model_data/model_data.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 16:51:29.559036 PatryksAutoAI-0.3.5/KaggleAutoAI/regression/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       89 2023-05-11 14:03:31.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/regression/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      607 2023-05-09 13:49:56.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/regression/metrics_regression.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 16:51:29.563036 PatryksAutoAI-0.3.5/KaggleAutoAI/regression/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      216 2023-05-11 14:13:19.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/regression/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6118 2023-05-11 15:13:02.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/regression/models/cat.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2631 2023-05-11 15:12:58.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/regression/models/elastic_net.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6037 2023-05-11 15:12:23.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/regression/models/gradient_boosting.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2559 2023-05-11 15:12:20.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/regression/models/lasso.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5469 2023-05-11 15:11:54.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/regression/models/lgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2849 2023-05-11 15:11:48.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/regression/models/sgd.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2633 2023-05-11 15:10:56.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/regression/models/svr.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7278 2023-05-11 15:10:54.000000 PatryksAutoAI-0.3.5/KaggleAutoAI/regression/models/xgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-12 16:51:29.563036 PatryksAutoAI-0.3.5/PKG-INFO
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 16:51:29.563036 PatryksAutoAI-0.3.5/PatryksAutoAI.egg-info/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-12 16:51:29.000000 PatryksAutoAI-0.3.5/PatryksAutoAI.egg-info/PKG-INFO
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1706 2023-05-12 16:51:29.000000 PatryksAutoAI-0.3.5/PatryksAutoAI.egg-info/SOURCES.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-12 16:51:29.000000 PatryksAutoAI-0.3.5/PatryksAutoAI.egg-info/dependency_links.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      162 2023-05-12 16:51:29.000000 PatryksAutoAI-0.3.5/PatryksAutoAI.egg-info/requires.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       13 2023-05-12 16:51:29.000000 PatryksAutoAI-0.3.5/PatryksAutoAI.egg-info/top_level.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-12 16:51:29.563036 PatryksAutoAI-0.3.5/setup.cfg
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1050 2023-05-12 16:51:24.000000 PatryksAutoAI-0.3.5/setup.py
```

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/automated_ai/classification/cat_automated.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/automated_ai/classification/cat_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/automated_ai/classification/compexity_level0.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/automated_ai/classification/compexity_level0.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from ...regression.models.cat import Cat
 from ...model_data.model_data import ModelData
 from sklearn.model_selection import train_test_split, KFold
+import logging
+logging.basicConfig(level=logging.WARNING)
 
 def Complexity_Level0(model, X, y):
     if model == "Cat":
         model = Cat()
     ## other model
 
+    print(f"Chosen model {model} starting choosing important columns \n\n")
     importance_columns = {}
     for col in X.columns:
         importance_columns[col] = 0
 
     ## fix null columns
     model_data = ModelData(X)
     columns_null = model_data.find_null_column()
@@ -32,20 +35,25 @@
     for i, (train_index, valid_index) in enumerate(kfold.split(X,y)):
         X_train, y_train = X.iloc[train_index], y.iloc[train_index]
         model.create_optuna(X_train,y_train,n_trials=100)
         feature_model = model.get()
         features = feature_model.get_feature_importance()
         for i,col in enumerate(X.columns):
             importance_columns[col] += features[i]
+
+    print(f"Importance of columns: \n")
+    for k,v in importance_columns.items():
+        print(f"{k}: {v} \n")
     
     ## Acceptting column that satify the requirenments 
     mean_importance = sum(importance_columns.values()) / len(importance_columns)
     threshold_importance = 0.75 * mean_importance
     columns = []
     for k,v in importance_columns.items():
         if v > threshold_importance:
             columns.append(k)
-    
+            
+    print(f"Used columns: {columns}")
     X = X[[columns]]
     model.create_optuna(X,y,n_trials=500)
     return model.get(), columns
```

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/classification/metrics.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/classification/metrics.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/cat.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/cat.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/extra_trees.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/extra_trees.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/gradient_boosting.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/hist_gradient.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/hist_gradient.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/kneighbours.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/kneighbours.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/light_lgb.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/light_lgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/linear_svc.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/linear_svc.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/logistic_regression.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/random_forest.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/random_forest.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/sgd_classifier.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/sgd_classifier.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/svc.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/svc.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/classification/models/xgb.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/classification/models/xgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/helper_function.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/helper_function.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/model_data/model_data.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/model_data/model_data.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/regression/metrics_regression.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/regression/metrics_regression.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/regression/models/cat.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/regression/models/cat.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/regression/models/elastic_net.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/regression/models/elastic_net.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/regression/models/gradient_boosting.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/regression/models/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/regression/models/lasso.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/regression/models/lasso.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/regression/models/lgb.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/regression/models/lgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/regression/models/sgd.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/regression/models/sgd.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/regression/models/svr.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/regression/models/svr.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/KaggleAutoAI/regression/models/xgb.py` & `PatryksAutoAI-0.3.5/KaggleAutoAI/regression/models/xgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/PKG-INFO` & `PatryksAutoAI-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 0.3.4
+Version: 0.3.5
 Summary: Auto_AI_patryk
 Home-page: UNKNOWN
 Author: patryk
 Author-email: lyczkopatryk1@gmail.com
 License: UNKNOWN
 Keywords: python,machine_learning,auto
 Platform: UNKNOWN
```

### Comparing `PatryksAutoAI-0.3.4/PatryksAutoAI.egg-info/PKG-INFO` & `PatryksAutoAI-0.3.5/PatryksAutoAI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 0.3.4
+Version: 0.3.5
 Summary: Auto_AI_patryk
 Home-page: UNKNOWN
 Author: patryk
 Author-email: lyczkopatryk1@gmail.com
 License: UNKNOWN
 Keywords: python,machine_learning,auto
 Platform: UNKNOWN
```

### Comparing `PatryksAutoAI-0.3.4/PatryksAutoAI.egg-info/SOURCES.txt` & `PatryksAutoAI-0.3.5/PatryksAutoAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.3.4/setup.py` & `PatryksAutoAI-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.3.4'
+VERSION = '0.3.5'
 DESCRIPTION = 'Auto_AI_patryk'
 LONG_DESCRIPTION = 'Package contains helping functions for creating ML models'
 
 # Read the requirements from requirements.txt
 with open('./KaggleAutoAI/requirements.txt') as f:
     requirements = f.read().splitlines()
```


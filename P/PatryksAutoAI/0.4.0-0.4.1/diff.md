# Comparing `tmp/PatryksAutoAI-0.4.0.tar.gz` & `tmp/PatryksAutoAI-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PatryksAutoAI-0.4.0.tar", last modified: Fri May 12 20:22:07 2023, max compression
+gzip compressed data, was "PatryksAutoAI-0.4.1.tar", last modified: Fri May 12 20:37:44 2023, max compression
```

## Comparing `PatryksAutoAI-0.4.0.tar` & `PatryksAutoAI-0.4.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 20:22:07.588077 PatryksAutoAI-0.4.0/
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 20:22:07.584077 PatryksAutoAI-0.4.0/KaggleAutoAI/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      200 2023-05-12 20:11:00.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 20:22:07.584077 PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       81 2023-05-12 19:58:04.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 20:22:07.584077 PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/algorithms/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       97 2023-05-12 19:31:03.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/algorithms/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1863 2023-05-12 19:32:24.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/algorithms/complexity_level0.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2138 2023-05-12 19:35:14.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/algorithms/complexity_level1.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 20:22:07.584077 PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/classification/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      534 2023-05-12 19:33:34.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/classification/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      849 2023-05-12 19:35:36.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/classification/cat_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      880 2023-05-12 19:35:47.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/classification/extra_trees.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      910 2023-05-12 19:35:56.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/classification/gradient_boosting_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      882 2023-05-12 19:36:07.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/classification/hist_gradient_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      860 2023-05-12 19:36:17.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/classification/lgb_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-05-12 19:36:29.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/classification/logistic_regression_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      890 2023-05-12 19:36:40.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/classification/random_forest_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      844 2023-05-12 19:36:55.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/classification/xgb_automated.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 20:22:07.584077 PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/regression/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      308 2023-05-12 19:57:48.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/regression/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 19:54:22.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/regression/cat_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      905 2023-05-12 19:55:05.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/regression/gradient_boosting_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 19:55:24.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/regression/lgb_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 19:56:32.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/regression/xgb_automated.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 20:22:07.584077 PatryksAutoAI-0.4.0/KaggleAutoAI/classification/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       72 2023-05-10 18:02:22.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/classification/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      648 2023-04-17 06:33:02.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/classification/metrics.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 20:22:07.588077 PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      317 2023-05-10 18:02:39.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7950 2023-05-12 17:08:00.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/cat.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6313 2023-05-12 17:08:04.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/extra_trees.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5279 2023-05-12 17:08:07.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/gradient_boosting.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5950 2023-05-12 17:08:11.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/hist_gradient.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2205 2023-05-11 13:59:17.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/kneighbours.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7276 2023-05-12 17:08:16.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/light_lgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2301 2023-05-11 13:59:23.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/linear_svc.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     4867 2023-05-12 17:08:23.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/logistic_regression.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6345 2023-05-12 17:08:27.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/random_forest.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2320 2023-05-11 13:59:44.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/sgd_classifier.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2255 2023-05-11 13:59:40.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/svc.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5743 2023-05-12 17:08:33.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/xgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/helper_function.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 20:22:07.588077 PatryksAutoAI-0.4.0/KaggleAutoAI/model_data/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      110 2023-05-10 18:02:54.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/model_data/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6075 2023-04-18 06:00:32.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/model_data/model_data.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 20:22:07.588077 PatryksAutoAI-0.4.0/KaggleAutoAI/regression/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       89 2023-05-12 20:10:49.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/regression/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      607 2023-05-09 13:49:56.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/regression/metrics_regression.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 20:22:07.588077 PatryksAutoAI-0.4.0/KaggleAutoAI/regression/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      216 2023-05-12 20:11:18.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/regression/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6159 2023-05-12 17:08:40.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/regression/models/cat.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2632 2023-05-12 17:08:49.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/regression/models/elastic_net.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6078 2023-05-12 17:08:53.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/regression/models/gradient_boosting.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2559 2023-05-11 15:12:20.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/regression/models/lasso.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5511 2023-05-12 17:09:00.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/regression/models/lgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2849 2023-05-11 15:11:48.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/regression/models/sgd.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2633 2023-05-11 15:10:56.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/regression/models/svr.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7320 2023-05-12 17:09:07.000000 PatryksAutoAI-0.4.0/KaggleAutoAI/regression/models/xgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-12 20:22:07.588077 PatryksAutoAI-0.4.0/PKG-INFO
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 20:22:07.588077 PatryksAutoAI-0.4.0/PatryksAutoAI.egg-info/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-12 20:22:07.000000 PatryksAutoAI-0.4.0/PatryksAutoAI.egg-info/PKG-INFO
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2543 2023-05-12 20:22:07.000000 PatryksAutoAI-0.4.0/PatryksAutoAI.egg-info/SOURCES.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-12 20:22:07.000000 PatryksAutoAI-0.4.0/PatryksAutoAI.egg-info/dependency_links.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      162 2023-05-12 20:22:07.000000 PatryksAutoAI-0.4.0/PatryksAutoAI.egg-info/requires.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       13 2023-05-12 20:22:07.000000 PatryksAutoAI-0.4.0/PatryksAutoAI.egg-info/top_level.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-12 20:22:07.588077 PatryksAutoAI-0.4.0/setup.cfg
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1050 2023-05-12 20:22:02.000000 PatryksAutoAI-0.4.0/setup.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 20:37:44.220705 PatryksAutoAI-0.4.1/
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 20:37:44.208705 PatryksAutoAI-0.4.1/KaggleAutoAI/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      210 2023-05-12 20:28:11.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 20:37:44.208705 PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      101 2023-05-12 20:27:46.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 20:37:44.212705 PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/algorithms/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       97 2023-05-12 19:31:03.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/algorithms/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1863 2023-05-12 19:32:24.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/algorithms/complexity_level0.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2138 2023-05-12 19:35:14.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/algorithms/complexity_level1.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 20:37:44.216705 PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/classification_automated/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      534 2023-05-12 19:33:34.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/classification_automated/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      849 2023-05-12 19:35:36.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/classification_automated/cat_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      880 2023-05-12 19:35:47.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/classification_automated/extra_trees.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      910 2023-05-12 19:35:56.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/classification_automated/gradient_boosting_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      882 2023-05-12 19:36:07.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/classification_automated/hist_gradient_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      860 2023-05-12 19:36:17.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/classification_automated/lgb_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-05-12 19:36:29.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/classification_automated/logistic_regression_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      890 2023-05-12 19:36:40.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/classification_automated/random_forest_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      844 2023-05-12 19:36:55.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/classification_automated/xgb_automated.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 20:37:44.216705 PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/regression_automated/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      308 2023-05-12 19:57:48.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/regression_automated/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 19:54:22.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/regression_automated/cat_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      905 2023-05-12 19:55:05.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/regression_automated/gradient_boosting_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 19:55:24.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/regression_automated/lgb_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 19:56:32.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/regression_automated/xgb_automated.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 20:37:44.216705 PatryksAutoAI-0.4.1/KaggleAutoAI/classification/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       72 2023-05-10 18:02:22.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/classification/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      648 2023-04-17 06:33:02.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/classification/metrics.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 20:37:44.216705 PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      317 2023-05-10 18:02:39.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7950 2023-05-12 17:08:00.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/cat.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6313 2023-05-12 17:08:04.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/extra_trees.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5279 2023-05-12 17:08:07.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/gradient_boosting.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5950 2023-05-12 17:08:11.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/hist_gradient.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2205 2023-05-11 13:59:17.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/kneighbours.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7276 2023-05-12 17:08:16.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/light_lgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2301 2023-05-11 13:59:23.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/linear_svc.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     4867 2023-05-12 17:08:23.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/logistic_regression.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6345 2023-05-12 17:08:27.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/random_forest.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2320 2023-05-11 13:59:44.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/sgd_classifier.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2255 2023-05-11 13:59:40.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/svc.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5743 2023-05-12 17:08:33.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/xgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/helper_function.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 20:37:44.216705 PatryksAutoAI-0.4.1/KaggleAutoAI/model_data/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      110 2023-05-10 18:02:54.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/model_data/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6075 2023-04-18 06:00:32.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/model_data/model_data.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 20:37:44.216705 PatryksAutoAI-0.4.1/KaggleAutoAI/regression/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       89 2023-05-12 20:27:28.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/regression/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      607 2023-05-09 13:49:56.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/regression/metrics_regression.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 20:37:44.220705 PatryksAutoAI-0.4.1/KaggleAutoAI/regression/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      216 2023-05-12 20:11:18.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/regression/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6159 2023-05-12 17:08:40.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/regression/models/cat.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2632 2023-05-12 17:08:49.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/regression/models/elastic_net.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6078 2023-05-12 17:08:53.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/regression/models/gradient_boosting.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2559 2023-05-11 15:12:20.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/regression/models/lasso.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5511 2023-05-12 17:09:00.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/regression/models/lgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2849 2023-05-11 15:11:48.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/regression/models/sgd.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2633 2023-05-11 15:10:56.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/regression/models/svr.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7320 2023-05-12 17:09:07.000000 PatryksAutoAI-0.4.1/KaggleAutoAI/regression/models/xgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-12 20:37:44.220705 PatryksAutoAI-0.4.1/PKG-INFO
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-12 20:37:44.220705 PatryksAutoAI-0.4.1/PatryksAutoAI.egg-info/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-12 20:37:44.000000 PatryksAutoAI-0.4.1/PatryksAutoAI.egg-info/PKG-INFO
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2683 2023-05-12 20:37:44.000000 PatryksAutoAI-0.4.1/PatryksAutoAI.egg-info/SOURCES.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-12 20:37:44.000000 PatryksAutoAI-0.4.1/PatryksAutoAI.egg-info/dependency_links.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      162 2023-05-12 20:37:44.000000 PatryksAutoAI-0.4.1/PatryksAutoAI.egg-info/requires.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       13 2023-05-12 20:37:44.000000 PatryksAutoAI-0.4.1/PatryksAutoAI.egg-info/top_level.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-12 20:37:44.220705 PatryksAutoAI-0.4.1/setup.cfg
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1050 2023-05-12 20:37:32.000000 PatryksAutoAI-0.4.1/setup.py
```

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/algorithms/complexity_level0.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/algorithms/complexity_level0.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/algorithms/complexity_level1.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/algorithms/complexity_level1.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/classification/__init__.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/classification_automated/__init__.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/classification/cat_automated.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/classification_automated/cat_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/classification/extra_trees.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/classification_automated/extra_trees.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/classification/gradient_boosting_automated.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/classification_automated/gradient_boosting_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/classification/hist_gradient_automated.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/classification_automated/hist_gradient_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/classification/lgb_automated.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/classification_automated/lgb_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/classification/logistic_regression_automated.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/classification_automated/logistic_regression_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/classification/random_forest_automated.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/classification_automated/random_forest_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/classification/xgb_automated.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/classification_automated/xgb_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/regression/cat_automated.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/regression_automated/cat_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/regression/gradient_boosting_automated.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/regression_automated/gradient_boosting_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/regression/lgb_automated.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/regression_automated/lgb_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/automated_ai/regression/xgb_automated.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/automated_ai/regression_automated/xgb_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/classification/metrics.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/classification/metrics.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/cat.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/cat.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/extra_trees.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/extra_trees.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/gradient_boosting.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/hist_gradient.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/hist_gradient.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/kneighbours.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/kneighbours.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/light_lgb.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/light_lgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/linear_svc.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/linear_svc.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/logistic_regression.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/random_forest.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/random_forest.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/sgd_classifier.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/sgd_classifier.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/svc.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/svc.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/classification/models/xgb.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/classification/models/xgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/helper_function.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/helper_function.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/model_data/model_data.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/model_data/model_data.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/regression/metrics_regression.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/regression/metrics_regression.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/regression/models/cat.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/regression/models/cat.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/regression/models/elastic_net.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/regression/models/elastic_net.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/regression/models/gradient_boosting.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/regression/models/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/regression/models/lasso.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/regression/models/lasso.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/regression/models/lgb.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/regression/models/lgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/regression/models/sgd.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/regression/models/sgd.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/regression/models/svr.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/regression/models/svr.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/KaggleAutoAI/regression/models/xgb.py` & `PatryksAutoAI-0.4.1/KaggleAutoAI/regression/models/xgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.4.0/PKG-INFO` & `PatryksAutoAI-0.4.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 0.4.0
+Version: 0.4.1
 Summary: Auto_AI_patryk
 Home-page: UNKNOWN
 Author: patryk
 Author-email: lyczkopatryk1@gmail.com
 License: UNKNOWN
 Keywords: python,machine_learning,auto
 Platform: UNKNOWN
```

### Comparing `PatryksAutoAI-0.4.0/PatryksAutoAI.egg-info/PKG-INFO` & `PatryksAutoAI-0.4.1/PatryksAutoAI.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 0.4.0
+Version: 0.4.1
 Summary: Auto_AI_patryk
 Home-page: UNKNOWN
 Author: patryk
 Author-email: lyczkopatryk1@gmail.com
 License: UNKNOWN
 Keywords: python,machine_learning,auto
 Platform: UNKNOWN
```

### Comparing `PatryksAutoAI-0.4.0/PatryksAutoAI.egg-info/SOURCES.txt` & `PatryksAutoAI-0.4.1/PatryksAutoAI.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 setup.py
 KaggleAutoAI/__init__.py
 KaggleAutoAI/helper_function.py
 KaggleAutoAI/automated_ai/__init__.py
 KaggleAutoAI/automated_ai/algorithms/__init__.py
 KaggleAutoAI/automated_ai/algorithms/complexity_level0.py
 KaggleAutoAI/automated_ai/algorithms/complexity_level1.py
-KaggleAutoAI/automated_ai/classification/__init__.py
-KaggleAutoAI/automated_ai/classification/cat_automated.py
-KaggleAutoAI/automated_ai/classification/extra_trees.py
-KaggleAutoAI/automated_ai/classification/gradient_boosting_automated.py
-KaggleAutoAI/automated_ai/classification/hist_gradient_automated.py
-KaggleAutoAI/automated_ai/classification/lgb_automated.py
-KaggleAutoAI/automated_ai/classification/logistic_regression_automated.py
-KaggleAutoAI/automated_ai/classification/random_forest_automated.py
-KaggleAutoAI/automated_ai/classification/xgb_automated.py
-KaggleAutoAI/automated_ai/regression/__init__.py
-KaggleAutoAI/automated_ai/regression/cat_automated.py
-KaggleAutoAI/automated_ai/regression/gradient_boosting_automated.py
-KaggleAutoAI/automated_ai/regression/lgb_automated.py
-KaggleAutoAI/automated_ai/regression/xgb_automated.py
+KaggleAutoAI/automated_ai/classification_automated/__init__.py
+KaggleAutoAI/automated_ai/classification_automated/cat_automated.py
+KaggleAutoAI/automated_ai/classification_automated/extra_trees.py
+KaggleAutoAI/automated_ai/classification_automated/gradient_boosting_automated.py
+KaggleAutoAI/automated_ai/classification_automated/hist_gradient_automated.py
+KaggleAutoAI/automated_ai/classification_automated/lgb_automated.py
+KaggleAutoAI/automated_ai/classification_automated/logistic_regression_automated.py
+KaggleAutoAI/automated_ai/classification_automated/random_forest_automated.py
+KaggleAutoAI/automated_ai/classification_automated/xgb_automated.py
+KaggleAutoAI/automated_ai/regression_automated/__init__.py
+KaggleAutoAI/automated_ai/regression_automated/cat_automated.py
+KaggleAutoAI/automated_ai/regression_automated/gradient_boosting_automated.py
+KaggleAutoAI/automated_ai/regression_automated/lgb_automated.py
+KaggleAutoAI/automated_ai/regression_automated/xgb_automated.py
 KaggleAutoAI/classification/__init__.py
 KaggleAutoAI/classification/metrics.py
 KaggleAutoAI/classification/models/__init__.py
 KaggleAutoAI/classification/models/cat.py
 KaggleAutoAI/classification/models/extra_trees.py
 KaggleAutoAI/classification/models/gradient_boosting.py
 KaggleAutoAI/classification/models/hist_gradient.py
```

### Comparing `PatryksAutoAI-0.4.0/setup.py` & `PatryksAutoAI-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.4.0'
+VERSION = '0.4.1'
 DESCRIPTION = 'Auto_AI_patryk'
 LONG_DESCRIPTION = 'Package contains helping functions for creating ML models'
 
 # Read the requirements from requirements.txt
 with open('./KaggleAutoAI/requirements.txt') as f:
     requirements = f.read().splitlines()
```


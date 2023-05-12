# Comparing `tmp/sarus-0.6.1.tar.gz` & `tmp/sarus-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus-0.6.1.tar", last modified: Wed May 10 18:38:07 2023, max compression
+gzip compressed data, was "sarus-0.6.2.tar", last modified: Fri May 12 10:42:30 2023, max compression
```

## Comparing `sarus-0.6.1.tar` & `sarus-0.6.2.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.212508 sarus-0.6.1/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       25 2022-09-14 12:56:20.000000 sarus-0.6.1/MANIFEST.in
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1553 2023-05-10 18:38:07.212508 sarus-0.6.1/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      663 2021-08-24 10:18:30.000000 sarus-0.6.1/README.rst
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2021-09-06 19:14:48.000000 sarus-0.6.1/pyproject.toml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.200508 sarus-0.6.1/sarus/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      544 2023-05-10 13:10:09.000000 sarus-0.6.1/sarus/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13051 2023-04-21 19:49:48.000000 sarus-0.6.1/sarus/config.yaml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.204508 sarus-0.6.1/sarus/context/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/context/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3179 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/context/local_sdk.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      345 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/context/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13713 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/dataspec_wrapper.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      743 2023-04-21 19:49:48.000000 sarus-0.6.1/sarus/debug.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.204508 sarus-0.6.1/sarus/imblearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      265 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/imblearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      578 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/imblearn/over_sampling.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/imblearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/imblearn/under_sampling.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.204508 sarus-0.6.1/sarus/legacy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       42 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/legacy/__init__.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.204508 sarus-0.6.1/sarus/legacy/pandas/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2023-01-27 14:38:46.000000 sarus-0.6.1/sarus/legacy/pandas/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    16606 2023-01-27 14:38:46.000000 sarus-0.6.1/sarus/legacy/pandas/dataframe.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.204508 sarus-0.6.1/sarus/legacy/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/legacy/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13194 2022-12-01 13:21:20.000000 sarus-0.6.1/sarus/legacy/tensorflow/dataset.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    42361 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/legacy/tensorflow/model.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.208508 sarus-0.6.1/sarus/manager/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/manager/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5351 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/manager/arrow_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1925 2023-05-10 18:35:08.000000 sarus-0.6.1/sarus/manager/arrow_remote.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1239 2023-05-10 18:35:08.000000 sarus-0.6.1/sarus/manager/base_remote.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3734 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/manager/cache_scalar_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6201 2023-05-10 13:10:09.000000 sarus-0.6.1/sarus/manager/dataspec_api.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.208508 sarus-0.6.1/sarus/manager/ops/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/manager/ops/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      921 2023-04-21 19:49:48.000000 sarus-0.6.1/sarus/manager/ops/api.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3352 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/manager/parquet_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    19300 2023-05-10 13:10:09.000000 sarus-0.6.1/sarus/manager/sdk_manager.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2556 2023-05-04 12:45:45.000000 sarus-0.6.1/sarus/manager/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4591 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/manager/value_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1572 2023-05-10 18:35:08.000000 sarus-0.6.1/sarus/manager/value_remote.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.208508 sarus-0.6.1/sarus/numpy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      337 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/numpy/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/numpy/random.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      963 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/numpy/scalars.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.208508 sarus-0.6.1/sarus/pandas/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      197 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/pandas/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      822 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/pandas/core.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4918 2023-04-21 19:49:48.000000 sarus-0.6.1/sarus/pandas/dataframe.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      206 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/pandas/io.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.208508 sarus-0.6.1/sarus/pandas_profiling/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/pandas_profiling/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      377 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/pandas_profiling/profile_report.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.208508 sarus-0.6.1/sarus/plotly/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      108 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/plotly/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      138 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/plotly/express.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    55942 2023-05-10 13:10:09.000000 sarus-0.6.1/sarus/sarus.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.208508 sarus-0.6.1/sarus/scripts/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-04-21 19:49:48.000000 sarus-0.6.1/sarus/scripts/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4618 2023-04-21 19:49:48.000000 sarus-0.6.1/sarus/scripts/generate_op_list.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.208508 sarus-0.6.1/sarus/sklearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      680 2023-04-21 19:49:48.000000 sarus-0.6.1/sarus/sklearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6604 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/sklearn/cluster.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      766 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/sklearn/compose.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      814 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/sklearn/decomposition.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    11437 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/sklearn/ensemble.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      566 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/sklearn/impute.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      177 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/sklearn/inspection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      668 2023-04-21 19:49:48.000000 sarus-0.6.1/sarus/sklearn/linear_model.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      174 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/sklearn/metrics.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1112 2023-04-21 19:49:48.000000 sarus-0.6.1/sarus/sklearn/model_selection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/sklearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1569 2023-04-21 19:49:48.000000 sarus-0.6.1/sarus/sklearn/preprocessing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      594 2023-04-21 19:49:48.000000 sarus-0.6.1/sarus/sklearn/svm.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.212508 sarus-0.6.1/sarus/skopt/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      223 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/skopt/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      929 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/skopt/searchcv.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.212508 sarus-0.6.1/sarus/std/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      154 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/std/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1074 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/std/types.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.212508 sarus-0.6.1/sarus/storage/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-01-27 14:38:46.000000 sarus-0.6.1/sarus/storage/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4552 2023-01-27 14:38:46.000000 sarus-0.6.1/sarus/storage/legacy_local.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.212508 sarus-0.6.1/sarus/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1780 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    11037 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/utils.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1461 2023-04-21 19:49:48.000000 sarus-0.6.1/sarus/wrapper_factory.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.212508 sarus-0.6.1/sarus/xgboost/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      213 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/xgboost/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      755 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/xgboost/xgboost.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.204508 sarus-0.6.1/sarus.egg-info/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1553 2023-05-10 18:38:06.000000 sarus-0.6.1/sarus.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2086 2023-05-10 18:38:07.000000 sarus-0.6.1/sarus.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-05-10 18:38:06.000000 sarus-0.6.1/sarus.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2021-08-30 08:41:07.000000 sarus-0.6.1/sarus.egg-info/not-zip-safe
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      349 2023-05-10 18:38:06.000000 sarus-0.6.1/sarus.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        6 2023-05-10 18:38:06.000000 sarus-0.6.1/sarus.egg-info/top_level.txt
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1306 2023-05-10 18:38:07.212508 sarus-0.6.1/setup.cfg
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)      106 2023-05-10 18:37:18.000000 sarus-0.6.1/setup.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.212508 sarus-0.6.1/tests/
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)      101 2021-09-06 19:14:48.000000 sarus-0.6.1/tests/test_sanity.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.124224 sarus-0.6.2/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       25 2022-09-14 12:56:20.000000 sarus-0.6.2/MANIFEST.in
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1553 2023-05-12 10:42:30.124224 sarus-0.6.2/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      663 2021-08-24 10:18:30.000000 sarus-0.6.2/README.rst
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2021-09-06 19:14:48.000000 sarus-0.6.2/pyproject.toml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.104224 sarus-0.6.2/sarus/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      544 2023-05-12 10:41:41.000000 sarus-0.6.2/sarus/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13051 2023-04-21 19:49:48.000000 sarus-0.6.2/sarus/config.yaml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.104224 sarus-0.6.2/sarus/context/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/context/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3179 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/context/local_sdk.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      345 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/context/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13713 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/dataspec_wrapper.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      743 2023-04-21 19:49:48.000000 sarus-0.6.2/sarus/debug.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.104224 sarus-0.6.2/sarus/imblearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      265 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/imblearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      578 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/imblearn/over_sampling.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/imblearn/pipeline.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/imblearn/under_sampling.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.108224 sarus-0.6.2/sarus/legacy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       42 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/legacy/__init__.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.108224 sarus-0.6.2/sarus/legacy/pandas/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2023-01-27 14:38:46.000000 sarus-0.6.2/sarus/legacy/pandas/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    16606 2023-01-27 14:38:46.000000 sarus-0.6.2/sarus/legacy/pandas/dataframe.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.112224 sarus-0.6.2/sarus/legacy/tensorflow/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/legacy/tensorflow/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13194 2022-12-01 13:21:20.000000 sarus-0.6.2/sarus/legacy/tensorflow/dataset.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    42361 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/legacy/tensorflow/model.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.112224 sarus-0.6.2/sarus/manager/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/manager/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5351 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/manager/arrow_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1925 2023-05-10 18:35:08.000000 sarus-0.6.2/sarus/manager/arrow_remote.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1239 2023-05-10 18:35:08.000000 sarus-0.6.2/sarus/manager/base_remote.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3734 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/manager/cache_scalar_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6201 2023-05-10 13:10:09.000000 sarus-0.6.2/sarus/manager/dataspec_api.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.112224 sarus-0.6.2/sarus/manager/ops/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/manager/ops/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      921 2023-04-21 19:49:48.000000 sarus-0.6.2/sarus/manager/ops/api.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3352 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/manager/parquet_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    19506 2023-05-12 10:35:52.000000 sarus-0.6.2/sarus/manager/sdk_manager.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2556 2023-05-04 12:45:45.000000 sarus-0.6.2/sarus/manager/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4591 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/manager/value_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1572 2023-05-10 18:35:08.000000 sarus-0.6.2/sarus/manager/value_remote.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.116224 sarus-0.6.2/sarus/numpy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      337 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/numpy/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/numpy/random.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      963 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/numpy/scalars.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.116224 sarus-0.6.2/sarus/pandas/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      197 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/pandas/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      822 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/pandas/core.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4918 2023-04-21 19:49:48.000000 sarus-0.6.2/sarus/pandas/dataframe.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      206 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/pandas/io.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.116224 sarus-0.6.2/sarus/pandas_profiling/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/pandas_profiling/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      377 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/pandas_profiling/profile_report.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.116224 sarus-0.6.2/sarus/plotly/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      108 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/plotly/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      138 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/plotly/express.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    55942 2023-05-10 13:10:09.000000 sarus-0.6.2/sarus/sarus.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.120224 sarus-0.6.2/sarus/scripts/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-04-21 19:49:48.000000 sarus-0.6.2/sarus/scripts/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4618 2023-04-21 19:49:48.000000 sarus-0.6.2/sarus/scripts/generate_op_list.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.124224 sarus-0.6.2/sarus/sklearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      680 2023-04-21 19:49:48.000000 sarus-0.6.2/sarus/sklearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6604 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/sklearn/cluster.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      766 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/sklearn/compose.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      814 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/sklearn/decomposition.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    11437 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/sklearn/ensemble.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      566 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/sklearn/impute.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      177 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/sklearn/inspection.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      668 2023-04-21 19:49:48.000000 sarus-0.6.2/sarus/sklearn/linear_model.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      174 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/sklearn/metrics.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1112 2023-04-21 19:49:48.000000 sarus-0.6.2/sarus/sklearn/model_selection.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/sklearn/pipeline.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1569 2023-04-21 19:49:48.000000 sarus-0.6.2/sarus/sklearn/preprocessing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      594 2023-04-21 19:49:48.000000 sarus-0.6.2/sarus/sklearn/svm.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.124224 sarus-0.6.2/sarus/skopt/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      223 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/skopt/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      929 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/skopt/searchcv.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.124224 sarus-0.6.2/sarus/std/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      154 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/std/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1074 2022-11-29 13:03:29.000000 sarus-0.6.2/sarus/std/types.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.124224 sarus-0.6.2/sarus/storage/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-01-27 14:38:46.000000 sarus-0.6.2/sarus/storage/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4552 2023-01-27 14:38:46.000000 sarus-0.6.2/sarus/storage/legacy_local.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.124224 sarus-0.6.2/sarus/tensorflow/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/tensorflow/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1780 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    11037 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/utils.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1461 2023-04-21 19:49:48.000000 sarus-0.6.2/sarus/wrapper_factory.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.124224 sarus-0.6.2/sarus/xgboost/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      213 2022-09-14 12:56:20.000000 sarus-0.6.2/sarus/xgboost/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      755 2023-05-05 09:59:58.000000 sarus-0.6.2/sarus/xgboost/xgboost.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.104224 sarus-0.6.2/sarus.egg-info/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1553 2023-05-12 10:42:29.000000 sarus-0.6.2/sarus.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2086 2023-05-12 10:42:30.000000 sarus-0.6.2/sarus.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-05-12 10:42:29.000000 sarus-0.6.2/sarus.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2021-08-30 08:41:07.000000 sarus-0.6.2/sarus.egg-info/not-zip-safe
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      349 2023-05-12 10:42:29.000000 sarus-0.6.2/sarus.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        6 2023-05-12 10:42:29.000000 sarus-0.6.2/sarus.egg-info/top_level.txt
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1306 2023-05-12 10:42:30.124224 sarus-0.6.2/setup.cfg
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)      106 2023-05-12 10:42:04.000000 sarus-0.6.2/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-12 10:42:30.124224 sarus-0.6.2/tests/
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)      101 2021-09-06 19:14:48.000000 sarus-0.6.2/tests/test_sanity.py
```

### Comparing `sarus-0.6.1/PKG-INFO` & `sarus-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.6.1
+Version: 0.6.2
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
 Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
 Keywords: differential privacy,AI,Data privacy
```

### Comparing `sarus-0.6.1/README.rst` & `sarus-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/__init__.py` & `sarus-0.6.2/sarus/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         std,
         xgboost,
     )
 
     from .sarus import Client, Dataset
     from .utils import eval, eval_policy, floating, integer, length
 
-VERSION = "0.6.0"
+VERSION = "0.6.2"
 
 __all__ = [
     "Dataset",
     "Client",
     "length",
     "eval",
     "eval_policy",
```

### Comparing `sarus-0.6.1/sarus/config.yaml` & `sarus-0.6.2/sarus/config.yaml`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/context/local_sdk.py` & `sarus-0.6.2/sarus/context/local_sdk.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/dataspec_wrapper.py` & `sarus-0.6.2/sarus/dataspec_wrapper.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/debug.py` & `sarus-0.6.2/sarus/debug.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/imblearn/over_sampling.py` & `sarus-0.6.2/sarus/imblearn/over_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/imblearn/pipeline.py` & `sarus-0.6.2/sarus/imblearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/imblearn/under_sampling.py` & `sarus-0.6.2/sarus/imblearn/under_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/legacy/pandas/dataframe.py` & `sarus-0.6.2/sarus/legacy/pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/legacy/tensorflow/dataset.py` & `sarus-0.6.2/sarus/legacy/tensorflow/dataset.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/legacy/tensorflow/model.py` & `sarus-0.6.2/sarus/legacy/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/manager/arrow_local.py` & `sarus-0.6.2/sarus/manager/arrow_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/manager/arrow_remote.py` & `sarus-0.6.2/sarus/manager/arrow_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/manager/base_remote.py` & `sarus-0.6.2/sarus/manager/base_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/manager/cache_scalar_local.py` & `sarus-0.6.2/sarus/manager/cache_scalar_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/manager/dataspec_api.py` & `sarus-0.6.2/sarus/manager/dataspec_api.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/manager/ops/api.py` & `sarus-0.6.2/sarus/manager/ops/api.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/manager/parquet_local.py` & `sarus-0.6.2/sarus/manager/parquet_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/manager/sdk_manager.py` & `sarus-0.6.2/sarus/manager/sdk_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -475,24 +475,27 @@
             return await TransformedScalar(scalar).value()
         else:
             return await SourceScalar(scalar).value()
 
     def copy_status_from_server(
         self, dataspec: st.DataSpec, task_names: t.List[str]
     ) -> None:
+        """This method is to be used only temporary to retrieve
+        the schemas from the server when a dataset is created"""
         status = api.dataspec_status(
             self.client(), dataspec.uuid(), task_names=task_names
         )
         for task_name in task_names:
-            stt.ready(
-                dataspec,
-                manager=self,
-                task=task_name,
-                properties=status.task_stages[task_name].properties,
-            )
+            if dataspec.status([task_name]) is None:
+                stt.ready(
+                    dataspec,
+                    manager=self,
+                    task=task_name,
+                    properties=status.task_stages[task_name].properties,
+                )
 
     def dataspec_computation(
         self,
         dataspec: st.DataSpec,
     ) -> BaseComputation:
         """Return the computation for a DataSpec."""
         proto = dataspec.prototype()
```

### Comparing `sarus-0.6.1/sarus/manager/typing.py` & `sarus-0.6.2/sarus/manager/typing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/manager/value_local.py` & `sarus-0.6.2/sarus/manager/value_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/manager/value_remote.py` & `sarus-0.6.2/sarus/manager/value_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/numpy/scalars.py` & `sarus-0.6.2/sarus/numpy/scalars.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/pandas/core.py` & `sarus-0.6.2/sarus/pandas/core.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/pandas/dataframe.py` & `sarus-0.6.2/sarus/pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/sarus.py` & `sarus-0.6.2/sarus/sarus.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/scripts/generate_op_list.py` & `sarus-0.6.2/sarus/scripts/generate_op_list.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/sklearn/__init__.py` & `sarus-0.6.2/sarus/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/sklearn/cluster.py` & `sarus-0.6.2/sarus/sklearn/cluster.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/sklearn/compose.py` & `sarus-0.6.2/sarus/sklearn/compose.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/sklearn/decomposition.py` & `sarus-0.6.2/sarus/sklearn/decomposition.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/sklearn/ensemble.py` & `sarus-0.6.2/sarus/sklearn/ensemble.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/sklearn/impute.py` & `sarus-0.6.2/sarus/sklearn/impute.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/sklearn/linear_model.py` & `sarus-0.6.2/sarus/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/sklearn/model_selection.py` & `sarus-0.6.2/sarus/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/sklearn/pipeline.py` & `sarus-0.6.2/sarus/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/sklearn/preprocessing.py` & `sarus-0.6.2/sarus/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/sklearn/svm.py` & `sarus-0.6.2/sarus/sklearn/svm.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/skopt/searchcv.py` & `sarus-0.6.2/sarus/skopt/searchcv.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/std/types.py` & `sarus-0.6.2/sarus/std/types.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/storage/legacy_local.py` & `sarus-0.6.2/sarus/storage/legacy_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/typing.py` & `sarus-0.6.2/sarus/typing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/utils.py` & `sarus-0.6.2/sarus/utils.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/wrapper_factory.py` & `sarus-0.6.2/sarus/wrapper_factory.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus/xgboost/xgboost.py` & `sarus-0.6.2/sarus/xgboost/xgboost.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/sarus.egg-info/PKG-INFO` & `sarus-0.6.2/sarus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.6.1
+Version: 0.6.2
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
 Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
 Keywords: differential privacy,AI,Data privacy
```

### Comparing `sarus-0.6.1/sarus.egg-info/SOURCES.txt` & `sarus-0.6.2/sarus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarus-0.6.1/setup.cfg` & `sarus-0.6.2/setup.cfg`

 * *Files identical despite different names*


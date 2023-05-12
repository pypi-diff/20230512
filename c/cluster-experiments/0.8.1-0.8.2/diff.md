# Comparing `tmp/cluster_experiments-0.8.1.tar.gz` & `tmp/cluster_experiments-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cluster_experiments-0.8.1.tar", last modified: Wed May 10 12:57:00 2023, max compression
+gzip compressed data, was "dist/cluster_experiments-0.8.2.tar", last modified: Fri May 12 13:15:15 2023, max compression
```

## Comparing `cluster_experiments-0.8.1.tar` & `cluster_experiments-0.8.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 12:57:00.601783 cluster_experiments-0.8.1/
--rw-r--r--   0 davidmasip   (502) staff       (20)     1067 2022-09-02 16:02:23.000000 cluster_experiments-0.8.1/LICENSE
--rw-r--r--   0 davidmasip   (502) staff       (20)       16 2022-08-05 13:17:06.000000 cluster_experiments-0.8.1/MANIFEST.in
--rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-05-10 12:57:00.599527 cluster_experiments-0.8.1/PKG-INFO
--rw-r--r--   0 davidmasip   (502) staff       (20)     7603 2023-05-10 11:17:47.000000 cluster_experiments-0.8.1/README.md
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 12:57:00.540660 cluster_experiments-0.8.1/cluster_experiments/
--rw-r--r--   0 davidmasip   (502) staff       (20)     1760 2023-05-10 11:17:47.000000 cluster_experiments-0.8.1/cluster_experiments/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     7578 2023-04-14 13:06:22.000000 cluster_experiments-0.8.1/cluster_experiments/cupac.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    21014 2023-05-09 15:17:29.000000 cluster_experiments-0.8.1/cluster_experiments/experiment_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    16391 2023-05-10 11:17:47.000000 cluster_experiments-0.8.1/cluster_experiments/perturbator.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    19753 2023-05-09 09:26:42.000000 cluster_experiments-0.8.1/cluster_experiments/power_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     4748 2023-05-10 12:56:47.000000 cluster_experiments-0.8.1/cluster_experiments/power_config.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    17741 2023-05-08 15:05:16.000000 cluster_experiments-0.8.1/cluster_experiments/random_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      496 2023-02-10 16:31:12.000000 cluster_experiments-0.8.1/cluster_experiments/utils.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     6137 2023-04-12 08:53:42.000000 cluster_experiments-0.8.1/cluster_experiments/washover.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 12:57:00.549134 cluster_experiments-0.8.1/cluster_experiments.egg-info/
--rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-05-10 12:57:00.000000 cluster_experiments-0.8.1/cluster_experiments.egg-info/PKG-INFO
--rw-r--r--   0 davidmasip   (502) staff       (20)     1481 2023-05-10 12:57:00.000000 cluster_experiments-0.8.1/cluster_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)        1 2023-05-10 12:57:00.000000 cluster_experiments-0.8.1/cluster_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-05-10 12:57:00.000000 cluster_experiments-0.8.1/cluster_experiments.egg-info/requires.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)       26 2023-05-10 12:57:00.000000 cluster_experiments-0.8.1/cluster_experiments.egg-info/top_level.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)       38 2023-05-10 12:57:00.602026 cluster_experiments-0.8.1/setup.cfg
--rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-05-10 12:56:47.000000 cluster_experiments-0.8.1/setup.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 12:57:00.562217 cluster_experiments-0.8.1/tests/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-10-21 09:42:28.000000 cluster_experiments-0.8.1/tests/__init__.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 12:57:00.566452 cluster_experiments-0.8.1/tests/analysis/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.8.1/tests/analysis/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     4251 2023-05-09 15:17:29.000000 cluster_experiments-0.8.1/tests/analysis/test_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      488 2023-04-24 11:36:52.000000 cluster_experiments-0.8.1/tests/analysis/test_ols_analysis.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 12:57:00.570642 cluster_experiments-0.8.1/tests/cupac/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.8.1/tests/cupac/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1583 2023-04-24 11:36:52.000000 cluster_experiments-0.8.1/tests/cupac/test_aggregator.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2610 2023-04-14 15:07:31.000000 cluster_experiments-0.8.1/tests/cupac/test_cupac_handler.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2406 2023-05-09 09:26:42.000000 cluster_experiments-0.8.1/tests/examples.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 12:57:00.573227 cluster_experiments-0.8.1/tests/perturbator/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.8.1/tests/perturbator/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     9410 2023-05-10 12:56:47.000000 cluster_experiments-0.8.1/tests/perturbator/test_perturbator.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 12:57:00.587919 cluster_experiments-0.8.1/tests/power_analysis/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.8.1/tests/power_analysis/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3283 2023-05-09 09:26:42.000000 cluster_experiments-0.8.1/tests/power_analysis/conftest.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2121 2022-12-30 09:27:02.000000 cluster_experiments-0.8.1/tests/power_analysis/test_cupac_power.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3078 2022-12-30 09:27:02.000000 cluster_experiments-0.8.1/tests/power_analysis/test_multivariate.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1088 2023-04-12 09:19:03.000000 cluster_experiments-0.8.1/tests/power_analysis/test_parallel.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     6082 2023-04-28 14:00:38.000000 cluster_experiments-0.8.1/tests/power_analysis/test_power_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3931 2022-12-30 09:27:02.000000 cluster_experiments-0.8.1/tests/power_analysis/test_power_raises.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      941 2023-05-09 09:26:42.000000 cluster_experiments-0.8.1/tests/power_analysis/test_seed.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3107 2023-05-09 09:26:42.000000 cluster_experiments-0.8.1/tests/power_analysis/test_switchback_power.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 12:57:00.598063 cluster_experiments-0.8.1/tests/splitter/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.8.1/tests/splitter/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     5686 2023-05-08 15:05:16.000000 cluster_experiments-0.8.1/tests/splitter/conftest.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     9412 2022-12-23 16:22:32.000000 cluster_experiments-0.8.1/tests/splitter/test_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3579 2022-12-27 08:21:57.000000 cluster_experiments-0.8.1/tests/splitter/test_switchback_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2882 2023-02-10 16:31:12.000000 cluster_experiments-0.8.1/tests/splitter/test_time_col.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3157 2023-04-12 08:53:42.000000 cluster_experiments-0.8.1/tests/splitter/test_washover.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2282 2023-05-10 11:17:47.000000 cluster_experiments-0.8.1/tests/test_docs.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2727 2022-12-19 11:37:00.000000 cluster_experiments-0.8.1/tests/test_non_clustered.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      208 2023-03-01 11:31:23.000000 cluster_experiments-0.8.1/tests/test_utils.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1325 2023-04-24 11:36:52.000000 cluster_experiments-0.8.1/tests/utils.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-12 13:15:15.868112 cluster_experiments-0.8.2/
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1067 2022-09-02 16:02:23.000000 cluster_experiments-0.8.2/LICENSE
+-rw-r--r--   0 davidmasip   (502) staff       (20)       16 2022-08-05 13:17:06.000000 cluster_experiments-0.8.2/MANIFEST.in
+-rw-r--r--   0 davidmasip   (502) staff       (20)      659 2023-05-12 13:15:15.866697 cluster_experiments-0.8.2/PKG-INFO
+-rw-r--r--   0 davidmasip   (502) staff       (20)     7603 2023-05-10 11:17:47.000000 cluster_experiments-0.8.2/README.md
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-12 13:15:15.755470 cluster_experiments-0.8.2/cluster_experiments/
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1760 2023-05-10 11:17:47.000000 cluster_experiments-0.8.2/cluster_experiments/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     7578 2023-04-14 13:06:22.000000 cluster_experiments-0.8.2/cluster_experiments/cupac.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    21014 2023-05-09 15:17:29.000000 cluster_experiments-0.8.2/cluster_experiments/experiment_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    16391 2023-05-10 11:17:47.000000 cluster_experiments-0.8.2/cluster_experiments/perturbator.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    19753 2023-05-09 09:26:42.000000 cluster_experiments-0.8.2/cluster_experiments/power_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     4748 2023-05-10 12:56:47.000000 cluster_experiments-0.8.2/cluster_experiments/power_config.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    17741 2023-05-08 15:05:16.000000 cluster_experiments-0.8.2/cluster_experiments/random_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      496 2023-02-10 16:31:12.000000 cluster_experiments-0.8.2/cluster_experiments/utils.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     6137 2023-04-12 08:53:42.000000 cluster_experiments-0.8.2/cluster_experiments/washover.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-12 13:15:15.771010 cluster_experiments-0.8.2/cluster_experiments.egg-info/
+-rw-r--r--   0 davidmasip   (502) staff       (20)      659 2023-05-12 13:15:15.000000 cluster_experiments-0.8.2/cluster_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1481 2023-05-12 13:15:15.000000 cluster_experiments-0.8.2/cluster_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)        1 2023-05-12 13:15:15.000000 cluster_experiments-0.8.2/cluster_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-05-12 13:15:15.000000 cluster_experiments-0.8.2/cluster_experiments.egg-info/requires.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)       26 2023-05-12 13:15:15.000000 cluster_experiments-0.8.2/cluster_experiments.egg-info/top_level.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)       38 2023-05-12 13:15:15.868781 cluster_experiments-0.8.2/setup.cfg
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1724 2023-05-12 13:12:21.000000 cluster_experiments-0.8.2/setup.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-12 13:15:15.785893 cluster_experiments-0.8.2/tests/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-10-21 09:42:28.000000 cluster_experiments-0.8.2/tests/__init__.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-12 13:15:15.791983 cluster_experiments-0.8.2/tests/analysis/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.8.2/tests/analysis/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     4251 2023-05-09 15:17:29.000000 cluster_experiments-0.8.2/tests/analysis/test_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      488 2023-04-24 11:36:52.000000 cluster_experiments-0.8.2/tests/analysis/test_ols_analysis.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-12 13:15:15.813541 cluster_experiments-0.8.2/tests/cupac/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.8.2/tests/cupac/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1583 2023-04-24 11:36:52.000000 cluster_experiments-0.8.2/tests/cupac/test_aggregator.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2610 2023-04-14 15:07:31.000000 cluster_experiments-0.8.2/tests/cupac/test_cupac_handler.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2406 2023-05-09 09:26:42.000000 cluster_experiments-0.8.2/tests/examples.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-12 13:15:15.817396 cluster_experiments-0.8.2/tests/perturbator/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.8.2/tests/perturbator/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     9410 2023-05-10 12:56:47.000000 cluster_experiments-0.8.2/tests/perturbator/test_perturbator.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-12 13:15:15.844657 cluster_experiments-0.8.2/tests/power_analysis/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.8.2/tests/power_analysis/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3283 2023-05-09 09:26:42.000000 cluster_experiments-0.8.2/tests/power_analysis/conftest.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2121 2022-12-30 09:27:02.000000 cluster_experiments-0.8.2/tests/power_analysis/test_cupac_power.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3078 2022-12-30 09:27:02.000000 cluster_experiments-0.8.2/tests/power_analysis/test_multivariate.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1088 2023-04-12 09:19:03.000000 cluster_experiments-0.8.2/tests/power_analysis/test_parallel.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     6082 2023-04-28 14:00:38.000000 cluster_experiments-0.8.2/tests/power_analysis/test_power_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3931 2022-12-30 09:27:02.000000 cluster_experiments-0.8.2/tests/power_analysis/test_power_raises.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      941 2023-05-09 09:26:42.000000 cluster_experiments-0.8.2/tests/power_analysis/test_seed.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3107 2023-05-09 09:26:42.000000 cluster_experiments-0.8.2/tests/power_analysis/test_switchback_power.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-12 13:15:15.864427 cluster_experiments-0.8.2/tests/splitter/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.8.2/tests/splitter/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     5686 2023-05-08 15:05:16.000000 cluster_experiments-0.8.2/tests/splitter/conftest.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     9412 2022-12-23 16:22:32.000000 cluster_experiments-0.8.2/tests/splitter/test_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3579 2022-12-27 08:21:57.000000 cluster_experiments-0.8.2/tests/splitter/test_switchback_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2882 2023-02-10 16:31:12.000000 cluster_experiments-0.8.2/tests/splitter/test_time_col.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3157 2023-04-12 08:53:42.000000 cluster_experiments-0.8.2/tests/splitter/test_washover.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2282 2023-05-10 11:17:47.000000 cluster_experiments-0.8.2/tests/test_docs.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2727 2022-12-19 11:37:00.000000 cluster_experiments-0.8.2/tests/test_non_clustered.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      208 2023-03-01 11:31:23.000000 cluster_experiments-0.8.2/tests/test_utils.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1325 2023-04-24 11:36:52.000000 cluster_experiments-0.8.2/tests/utils.py
```

### Comparing `cluster_experiments-0.8.1/LICENSE` & `cluster_experiments-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/README.md` & `cluster_experiments-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/cluster_experiments/__init__.py` & `cluster_experiments-0.8.2/cluster_experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/cluster_experiments/cupac.py` & `cluster_experiments-0.8.2/cluster_experiments/cupac.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/cluster_experiments/experiment_analysis.py` & `cluster_experiments-0.8.2/cluster_experiments/experiment_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/cluster_experiments/perturbator.py` & `cluster_experiments-0.8.2/cluster_experiments/perturbator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/cluster_experiments/power_analysis.py` & `cluster_experiments-0.8.2/cluster_experiments/power_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/cluster_experiments/power_config.py` & `cluster_experiments-0.8.2/cluster_experiments/power_config.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/cluster_experiments/random_splitter.py` & `cluster_experiments-0.8.2/cluster_experiments/random_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/cluster_experiments/washover.py` & `cluster_experiments-0.8.2/cluster_experiments/washover.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/cluster_experiments.egg-info/SOURCES.txt` & `cluster_experiments-0.8.2/cluster_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/cluster_experiments.egg-info/requires.txt` & `cluster_experiments-0.8.2/cluster_experiments.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/tests/analysis/test_analysis.py` & `cluster_experiments-0.8.2/tests/analysis/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/tests/cupac/test_aggregator.py` & `cluster_experiments-0.8.2/tests/cupac/test_aggregator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/tests/cupac/test_cupac_handler.py` & `cluster_experiments-0.8.2/tests/cupac/test_cupac_handler.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/tests/examples.py` & `cluster_experiments-0.8.2/tests/examples.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/tests/perturbator/test_perturbator.py` & `cluster_experiments-0.8.2/tests/perturbator/test_perturbator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/tests/power_analysis/conftest.py` & `cluster_experiments-0.8.2/tests/power_analysis/conftest.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/tests/power_analysis/test_cupac_power.py` & `cluster_experiments-0.8.2/tests/power_analysis/test_cupac_power.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/tests/power_analysis/test_multivariate.py` & `cluster_experiments-0.8.2/tests/power_analysis/test_multivariate.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/tests/power_analysis/test_parallel.py` & `cluster_experiments-0.8.2/tests/power_analysis/test_parallel.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/tests/power_analysis/test_power_analysis.py` & `cluster_experiments-0.8.2/tests/power_analysis/test_power_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/tests/power_analysis/test_power_raises.py` & `cluster_experiments-0.8.2/tests/power_analysis/test_power_raises.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/tests/power_analysis/test_seed.py` & `cluster_experiments-0.8.2/tests/power_analysis/test_seed.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/tests/power_analysis/test_switchback_power.py` & `cluster_experiments-0.8.2/tests/power_analysis/test_switchback_power.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/tests/splitter/conftest.py` & `cluster_experiments-0.8.2/tests/splitter/conftest.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/tests/splitter/test_splitter.py` & `cluster_experiments-0.8.2/tests/splitter/test_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/tests/splitter/test_switchback_splitter.py` & `cluster_experiments-0.8.2/tests/splitter/test_switchback_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/tests/splitter/test_time_col.py` & `cluster_experiments-0.8.2/tests/splitter/test_time_col.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/tests/splitter/test_washover.py` & `cluster_experiments-0.8.2/tests/splitter/test_washover.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/tests/test_docs.py` & `cluster_experiments-0.8.2/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/tests/test_non_clustered.py` & `cluster_experiments-0.8.2/tests/test_non_clustered.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.1/tests/utils.py` & `cluster_experiments-0.8.2/tests/utils.py`

 * *Files identical despite different names*


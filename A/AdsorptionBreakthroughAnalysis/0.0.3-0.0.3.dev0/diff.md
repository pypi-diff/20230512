# Comparing `tmp/AdsorptionBreakthroughAnalysis-0.0.3.tar.gz` & `tmp/AdsorptionBreakthroughAnalysis-0.0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AdsorptionBreakthroughAnalysis-0.0.3.tar", last modified: Fri May 12 13:18:05 2023, max compression
+gzip compressed data, was "AdsorptionBreakthroughAnalysis-0.0.3.dev0.tar", last modified: Fri May 12 13:00:10 2023, max compression
```

## Comparing `AdsorptionBreakthroughAnalysis-0.0.3.tar` & `AdsorptionBreakthroughAnalysis-0.0.3.dev0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-12 13:18:05.348520 AdsorptionBreakthroughAnalysis-0.0.3/
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)     1079 2023-04-17 22:01:33.000000 AdsorptionBreakthroughAnalysis-0.0.3/LICENSE
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      475 2023-04-18 12:58:36.000000 AdsorptionBreakthroughAnalysis-0.0.3/MANIFEST.in
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)    10245 2023-05-12 13:18:05.348520 AdsorptionBreakthroughAnalysis-0.0.3/PKG-INFO
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)     8779 2023-04-17 22:20:14.000000 AdsorptionBreakthroughAnalysis-0.0.3/README.md
-drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-12 13:18:05.324520 AdsorptionBreakthroughAnalysis-0.0.3/docs/
-drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-12 13:18:05.328520 AdsorptionBreakthroughAnalysis-0.0.3/docs/source/
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      331 2023-04-17 22:01:33.000000 AdsorptionBreakthroughAnalysis-0.0.3/docs/source/cli.rst
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)     7505 2023-05-12 13:18:04.000000 AdsorptionBreakthroughAnalysis-0.0.3/docs/source/conf.py
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)     1851 2023-04-17 22:01:33.000000 AdsorptionBreakthroughAnalysis-0.0.3/docs/source/index.rst
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      645 2023-04-17 22:01:33.000000 AdsorptionBreakthroughAnalysis-0.0.3/docs/source/installation.rst
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)       77 2023-04-17 22:01:33.000000 AdsorptionBreakthroughAnalysis-0.0.3/docs/source/usage.rst
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      377 2023-04-17 22:01:33.000000 AdsorptionBreakthroughAnalysis-0.0.3/pyproject.toml
--rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)     2780 2023-05-12 13:18:05.352520 AdsorptionBreakthroughAnalysis-0.0.3/setup.cfg
-drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-12 13:18:05.324520 AdsorptionBreakthroughAnalysis-0.0.3/src/
-drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-12 13:18:05.328520 AdsorptionBreakthroughAnalysis-0.0.3/src/AdsorptionBreakthroughAnalysis/
--rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)      417 2023-05-11 13:00:28.000000 AdsorptionBreakthroughAnalysis-0.0.3/src/AdsorptionBreakthroughAnalysis/__init__.py
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      347 2023-04-18 13:14:08.000000 AdsorptionBreakthroughAnalysis-0.0.3/src/AdsorptionBreakthroughAnalysis/__main__.py
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)       42 2023-04-17 22:04:29.000000 AdsorptionBreakthroughAnalysis-0.0.3/src/AdsorptionBreakthroughAnalysis/api.py
--rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)    53740 2023-05-12 12:57:00.000000 AdsorptionBreakthroughAnalysis-0.0.3/src/AdsorptionBreakthroughAnalysis/breakthrough_analysis.py
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      979 2023-04-18 13:10:35.000000 AdsorptionBreakthroughAnalysis-0.0.3/src/AdsorptionBreakthroughAnalysis/cli.py
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)        1 2023-04-17 22:04:29.000000 AdsorptionBreakthroughAnalysis-0.0.3/src/AdsorptionBreakthroughAnalysis/py.typed
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)     1096 2023-05-12 13:18:04.000000 AdsorptionBreakthroughAnalysis-0.0.3/src/AdsorptionBreakthroughAnalysis/version.py
-drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-12 13:18:05.332520 AdsorptionBreakthroughAnalysis-0.0.3/src/AdsorptionBreakthroughAnalysis.egg-info/
--rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)    10245 2023-05-12 13:18:05.000000 AdsorptionBreakthroughAnalysis-0.0.3/src/AdsorptionBreakthroughAnalysis.egg-info/PKG-INFO
--rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)     1586 2023-05-12 13:18:05.000000 AdsorptionBreakthroughAnalysis-0.0.3/src/AdsorptionBreakthroughAnalysis.egg-info/SOURCES.txt
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)        1 2023-05-12 13:18:05.000000 AdsorptionBreakthroughAnalysis-0.0.3/src/AdsorptionBreakthroughAnalysis.egg-info/dependency_links.txt
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)       91 2023-05-12 13:18:05.000000 AdsorptionBreakthroughAnalysis-0.0.3/src/AdsorptionBreakthroughAnalysis.egg-info/entry_points.txt
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)        1 2023-05-11 12:45:00.000000 AdsorptionBreakthroughAnalysis-0.0.3/src/AdsorptionBreakthroughAnalysis.egg-info/not-zip-safe
--rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)      182 2023-05-12 13:18:05.000000 AdsorptionBreakthroughAnalysis-0.0.3/src/AdsorptionBreakthroughAnalysis.egg-info/requires.txt
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)       31 2023-05-12 13:18:05.000000 AdsorptionBreakthroughAnalysis-0.0.3/src/AdsorptionBreakthroughAnalysis.egg-info/top_level.txt
-drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-12 13:18:05.336520 AdsorptionBreakthroughAnalysis-0.0.3/tests/
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)       64 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.3/tests/__init__.py
-drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-12 13:18:05.324520 AdsorptionBreakthroughAnalysis-0.0.3/tests/data/
-drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-12 13:18:05.340520 AdsorptionBreakthroughAnalysis-0.0.3/tests/data/experimental_data/
--rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)  8324734 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.3/tests/data/experimental_data/220819-ZIF-8-dry-22%and60%40C20220819134938.txt
--rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)    35453 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.3/tests/data/experimental_data/220819ZIF8Blank22and60%CO2at40C.csv
--rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)    81913 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.3/tests/data/experimental_data/220824-ZIF-8-4and22%at40C.csv
--rw-r--r--   0 ffm2000   (1002) ffm2000   (1003) 18648765 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.3/tests/data/experimental_data/220824-ZIF-8-4and22%at40C.txt
-drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-12 13:18:05.348520 AdsorptionBreakthroughAnalysis-0.0.3/tests/data/processed_data/
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)    85579 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.3/tests/data/processed_data/bench_220819-ZIF-8-dry-22%and60%40C20220819134938.txt_220819ZIF8Blank22and60%CO2at40C.csv.csv
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)   113867 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.3/tests/data/processed_data/bench_220824-ZIF-8-4and22%at40C.txt_220824-ZIF-8-4and22%at40C.csv.csv
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      371 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.3/tests/data/processed_data/bench_loading_experiment_22perc_ZIF8.pickle
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      371 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.3/tests/data/processed_data/bench_loading_experiment_22perc_ZIF8_blank.pickle
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)     5248 2023-04-18 13:04:06.000000 AdsorptionBreakthroughAnalysis-0.0.3/tests/test_results.py
--rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      640 2023-04-18 12:35:25.000000 AdsorptionBreakthroughAnalysis-0.0.3/tests/test_version.py
+drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-12 13:00:10.931746 AdsorptionBreakthroughAnalysis-0.0.3.dev0/
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)     1079 2023-04-17 22:01:33.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/LICENSE
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      475 2023-04-18 12:58:36.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/MANIFEST.in
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)    10250 2023-05-12 13:00:10.931746 AdsorptionBreakthroughAnalysis-0.0.3.dev0/PKG-INFO
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)     8779 2023-04-17 22:20:14.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/README.md
+drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-12 13:00:10.903746 AdsorptionBreakthroughAnalysis-0.0.3.dev0/docs/
+drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-12 13:00:10.907746 AdsorptionBreakthroughAnalysis-0.0.3.dev0/docs/source/
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      331 2023-04-17 22:01:33.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/docs/source/cli.rst
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)     7509 2023-05-12 12:59:25.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/docs/source/conf.py
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)     1851 2023-04-17 22:01:33.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/docs/source/index.rst
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      645 2023-04-17 22:01:33.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/docs/source/installation.rst
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)       77 2023-04-17 22:01:33.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/docs/source/usage.rst
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      377 2023-04-17 22:01:33.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/pyproject.toml
+-rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)     2784 2023-05-12 13:00:10.935746 AdsorptionBreakthroughAnalysis-0.0.3.dev0/setup.cfg
+drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-12 13:00:10.903746 AdsorptionBreakthroughAnalysis-0.0.3.dev0/src/
+drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-12 13:00:10.911746 AdsorptionBreakthroughAnalysis-0.0.3.dev0/src/AdsorptionBreakthroughAnalysis/
+-rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)      417 2023-05-11 13:00:28.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/src/AdsorptionBreakthroughAnalysis/__init__.py
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      347 2023-04-18 13:14:08.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/src/AdsorptionBreakthroughAnalysis/__main__.py
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)       42 2023-04-17 22:04:29.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/src/AdsorptionBreakthroughAnalysis/api.py
+-rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)    53740 2023-05-12 12:57:00.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/src/AdsorptionBreakthroughAnalysis/breakthrough_analysis.py
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      979 2023-04-18 13:10:35.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/src/AdsorptionBreakthroughAnalysis/cli.py
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)        1 2023-04-17 22:04:29.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/src/AdsorptionBreakthroughAnalysis/py.typed
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)     1100 2023-05-12 12:59:25.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/src/AdsorptionBreakthroughAnalysis/version.py
+drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-12 13:00:10.915746 AdsorptionBreakthroughAnalysis-0.0.3.dev0/src/AdsorptionBreakthroughAnalysis.egg-info/
+-rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)    10250 2023-05-12 13:00:10.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/src/AdsorptionBreakthroughAnalysis.egg-info/PKG-INFO
+-rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)     1586 2023-05-12 13:00:10.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/src/AdsorptionBreakthroughAnalysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)        1 2023-05-12 13:00:10.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/src/AdsorptionBreakthroughAnalysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)       91 2023-05-12 13:00:10.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/src/AdsorptionBreakthroughAnalysis.egg-info/entry_points.txt
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)        1 2023-05-11 12:45:00.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/src/AdsorptionBreakthroughAnalysis.egg-info/not-zip-safe
+-rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)      182 2023-05-12 13:00:10.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/src/AdsorptionBreakthroughAnalysis.egg-info/requires.txt
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)       31 2023-05-12 13:00:10.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/src/AdsorptionBreakthroughAnalysis.egg-info/top_level.txt
+drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-12 13:00:10.915746 AdsorptionBreakthroughAnalysis-0.0.3.dev0/tests/
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)       64 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/tests/__init__.py
+drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-12 13:00:10.903746 AdsorptionBreakthroughAnalysis-0.0.3.dev0/tests/data/
+drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-12 13:00:10.919746 AdsorptionBreakthroughAnalysis-0.0.3.dev0/tests/data/experimental_data/
+-rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)  8324734 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/tests/data/experimental_data/220819-ZIF-8-dry-22%and60%40C20220819134938.txt
+-rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)    35453 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/tests/data/experimental_data/220819ZIF8Blank22and60%CO2at40C.csv
+-rw-r--r--   0 ffm2000   (1002) ffm2000   (1003)    81913 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/tests/data/experimental_data/220824-ZIF-8-4and22%at40C.csv
+-rw-r--r--   0 ffm2000   (1002) ffm2000   (1003) 18648765 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/tests/data/experimental_data/220824-ZIF-8-4and22%at40C.txt
+drwxrwxr-x   0 ffm2000   (1002) ffm2000   (1003)        0 2023-05-12 13:00:10.931746 AdsorptionBreakthroughAnalysis-0.0.3.dev0/tests/data/processed_data/
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)    85579 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/tests/data/processed_data/bench_220819-ZIF-8-dry-22%and60%40C20220819134938.txt_220819ZIF8Blank22and60%CO2at40C.csv.csv
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)   113867 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/tests/data/processed_data/bench_220824-ZIF-8-4and22%at40C.txt_220824-ZIF-8-4and22%at40C.csv.csv
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      371 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/tests/data/processed_data/bench_loading_experiment_22perc_ZIF8.pickle
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      371 2023-04-17 22:10:14.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/tests/data/processed_data/bench_loading_experiment_22perc_ZIF8_blank.pickle
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)     5248 2023-04-18 13:04:06.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/tests/test_results.py
+-rw-rw-r--   0 ffm2000   (1002) ffm2000   (1003)      640 2023-04-18 12:35:25.000000 AdsorptionBreakthroughAnalysis-0.0.3.dev0/tests/test_version.py
```

### Comparing `AdsorptionBreakthroughAnalysis-0.0.3/LICENSE` & `AdsorptionBreakthroughAnalysis-0.0.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `AdsorptionBreakthroughAnalysis-0.0.3/PKG-INFO` & `AdsorptionBreakthroughAnalysis-0.0.3.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AdsorptionBreakthroughAnalysis
-Version: 0.0.3
+Version: 0.0.3.dev0
 Summary: This program is used to analyse the breakthrough curves generated by the RCCS adsorption rig
 Home-page: https://github.com/RCCS-CaptureTeam/Adsorption_Breakthrough_Analysis
 Download-URL: https://github.com/RCCS-CaptureTeam/Adsorption_Breakthrough_Analysis/releases
 Author: Daniel Maroto-Andresen
 Author-email: dm937@cam.ac.uk
 Maintainer: Fergus Mcilwaine
 Maintainer-email: f.mcilwaine@hw.ac.uk
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: AdsorptionBreakthroughAnalysis Version: 0.0.3
+Metadata-Version: 2.1 Name: AdsorptionBreakthroughAnalysis Version: 0.0.3.dev0
 Summary: This program is used to analyse the breakthrough curves generated by
 the RCCS adsorption rig Home-page: https://github.com/RCCS-CaptureTeam/
 Adsorption_Breakthrough_Analysis Download-URL: https://github.com/RCCS-
 CaptureTeam/Adsorption_Breakthrough_Analysis/releases Author: Daniel Maroto-
 Andresen Author-email: dm937@cam.ac.uk Maintainer: Fergus Mcilwaine Maintainer-
 email: f.mcilwaine@hw.ac.uk License: MIT Project-URL: Bug Tracker, https://
 github.com/RCCS-CaptureTeam/Adsorption_Breakthrough_Analysis/issues Project-
```

### Comparing `AdsorptionBreakthroughAnalysis-0.0.3/README.md` & `AdsorptionBreakthroughAnalysis-0.0.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `AdsorptionBreakthroughAnalysis-0.0.3/docs/source/conf.py` & `AdsorptionBreakthroughAnalysis-0.0.3.dev0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "AdsorptionBreakthroughAnalysis"
 copyright = f"{date.today().year}, Daniel Maroto-Andresen"
 author = "Daniel Maroto-Andresen"
 
 # The full version, including alpha/beta/rc tags.
-release = "0.0.3"
+release = "0.0.3-dev"
 
 # The short X.Y version.
 parsed_version = re.match(
     "(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?",
     release,
 )
 version = parsed_version.expand("\g<major>.\g<minor>.\g<patch>")
```

### Comparing `AdsorptionBreakthroughAnalysis-0.0.3/docs/source/index.rst` & `AdsorptionBreakthroughAnalysis-0.0.3.dev0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `AdsorptionBreakthroughAnalysis-0.0.3/docs/source/installation.rst` & `AdsorptionBreakthroughAnalysis-0.0.3.dev0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `AdsorptionBreakthroughAnalysis-0.0.3/setup.cfg` & `AdsorptionBreakthroughAnalysis-0.0.3.dev0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = AdsorptionBreakthroughAnalysis
-version = 0.0.3
+version = 0.0.3-dev
 description = This program is used to analyse the breakthrough curves generated by the RCCS adsorption rig
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/RCCS-CaptureTeam/Adsorption_Breakthrough_Analysis
 download_url = https://github.com/RCCS-CaptureTeam/Adsorption_Breakthrough_Analysis/releases
 project_urls = 
 	Bug Tracker = https://github.com/RCCS-CaptureTeam/Adsorption_Breakthrough_Analysis/issues
```

### Comparing `AdsorptionBreakthroughAnalysis-0.0.3/src/AdsorptionBreakthroughAnalysis/breakthrough_analysis.py` & `AdsorptionBreakthroughAnalysis-0.0.3.dev0/src/AdsorptionBreakthroughAnalysis/breakthrough_analysis.py`

 * *Files identical despite different names*

### Comparing `AdsorptionBreakthroughAnalysis-0.0.3/src/AdsorptionBreakthroughAnalysis/cli.py` & `AdsorptionBreakthroughAnalysis-0.0.3.dev0/src/AdsorptionBreakthroughAnalysis/cli.py`

 * *Files identical despite different names*

### Comparing `AdsorptionBreakthroughAnalysis-0.0.3/src/AdsorptionBreakthroughAnalysis/version.py` & `AdsorptionBreakthroughAnalysis-0.0.3.dev0/src/AdsorptionBreakthroughAnalysis/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 __all__ = [
     "VERSION",
     "get_version",
     "get_git_hash",
 ]
 
-VERSION = "0.0.3"
+VERSION = "0.0.3-dev"
 
 
 def get_git_hash() -> str:
     """Get the :mod:`AdsorptionBreakthroughAnalysis` git hash."""
     with open(os.devnull, "w") as devnull:
         try:
             ret = check_output(  # noqa: S603,S607
```

### Comparing `AdsorptionBreakthroughAnalysis-0.0.3/src/AdsorptionBreakthroughAnalysis.egg-info/PKG-INFO` & `AdsorptionBreakthroughAnalysis-0.0.3.dev0/src/AdsorptionBreakthroughAnalysis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AdsorptionBreakthroughAnalysis
-Version: 0.0.3
+Version: 0.0.3.dev0
 Summary: This program is used to analyse the breakthrough curves generated by the RCCS adsorption rig
 Home-page: https://github.com/RCCS-CaptureTeam/Adsorption_Breakthrough_Analysis
 Download-URL: https://github.com/RCCS-CaptureTeam/Adsorption_Breakthrough_Analysis/releases
 Author: Daniel Maroto-Andresen
 Author-email: dm937@cam.ac.uk
 Maintainer: Fergus Mcilwaine
 Maintainer-email: f.mcilwaine@hw.ac.uk
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: AdsorptionBreakthroughAnalysis Version: 0.0.3
+Metadata-Version: 2.1 Name: AdsorptionBreakthroughAnalysis Version: 0.0.3.dev0
 Summary: This program is used to analyse the breakthrough curves generated by
 the RCCS adsorption rig Home-page: https://github.com/RCCS-CaptureTeam/
 Adsorption_Breakthrough_Analysis Download-URL: https://github.com/RCCS-
 CaptureTeam/Adsorption_Breakthrough_Analysis/releases Author: Daniel Maroto-
 Andresen Author-email: dm937@cam.ac.uk Maintainer: Fergus Mcilwaine Maintainer-
 email: f.mcilwaine@hw.ac.uk License: MIT Project-URL: Bug Tracker, https://
 github.com/RCCS-CaptureTeam/Adsorption_Breakthrough_Analysis/issues Project-
```

### Comparing `AdsorptionBreakthroughAnalysis-0.0.3/src/AdsorptionBreakthroughAnalysis.egg-info/SOURCES.txt` & `AdsorptionBreakthroughAnalysis-0.0.3.dev0/src/AdsorptionBreakthroughAnalysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AdsorptionBreakthroughAnalysis-0.0.3/tests/data/experimental_data/220819-ZIF-8-dry-22%and60%40C20220819134938.txt` & `AdsorptionBreakthroughAnalysis-0.0.3.dev0/tests/data/experimental_data/220819-ZIF-8-dry-22%and60%40C20220819134938.txt`

 * *Files identical despite different names*

### Comparing `AdsorptionBreakthroughAnalysis-0.0.3/tests/data/experimental_data/220819ZIF8Blank22and60%CO2at40C.csv` & `AdsorptionBreakthroughAnalysis-0.0.3.dev0/tests/data/experimental_data/220819ZIF8Blank22and60%CO2at40C.csv`

 * *Files identical despite different names*

### Comparing `AdsorptionBreakthroughAnalysis-0.0.3/tests/data/experimental_data/220824-ZIF-8-4and22%at40C.csv` & `AdsorptionBreakthroughAnalysis-0.0.3.dev0/tests/data/experimental_data/220824-ZIF-8-4and22%at40C.csv`

 * *Files identical despite different names*

### Comparing `AdsorptionBreakthroughAnalysis-0.0.3/tests/data/experimental_data/220824-ZIF-8-4and22%at40C.txt` & `AdsorptionBreakthroughAnalysis-0.0.3.dev0/tests/data/experimental_data/220824-ZIF-8-4and22%at40C.txt`

 * *Files identical despite different names*

### Comparing `AdsorptionBreakthroughAnalysis-0.0.3/tests/data/processed_data/bench_220819-ZIF-8-dry-22%and60%40C20220819134938.txt_220819ZIF8Blank22and60%CO2at40C.csv.csv` & `AdsorptionBreakthroughAnalysis-0.0.3.dev0/tests/data/processed_data/bench_220819-ZIF-8-dry-22%and60%40C20220819134938.txt_220819ZIF8Blank22and60%CO2at40C.csv.csv`

 * *Files identical despite different names*

### Comparing `AdsorptionBreakthroughAnalysis-0.0.3/tests/data/processed_data/bench_220824-ZIF-8-4and22%at40C.txt_220824-ZIF-8-4and22%at40C.csv.csv` & `AdsorptionBreakthroughAnalysis-0.0.3.dev0/tests/data/processed_data/bench_220824-ZIF-8-4and22%at40C.txt_220824-ZIF-8-4and22%at40C.csv.csv`

 * *Files identical despite different names*

### Comparing `AdsorptionBreakthroughAnalysis-0.0.3/tests/test_results.py` & `AdsorptionBreakthroughAnalysis-0.0.3.dev0/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `AdsorptionBreakthroughAnalysis-0.0.3/tests/test_version.py` & `AdsorptionBreakthroughAnalysis-0.0.3.dev0/tests/test_version.py`

 * *Files identical despite different names*


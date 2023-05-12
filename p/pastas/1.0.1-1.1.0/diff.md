# Comparing `tmp/pastas-1.0.1.tar.gz` & `tmp/pastas-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pastas-1.0.1.tar", last modified: Tue Feb  7 21:36:13 2023, max compression
+gzip compressed data, was "pastas-1.1.0.tar", last modified: Fri May 12 10:20:40 2023, max compression
```

## Comparing `pastas-1.0.1.tar` & `pastas-1.1.0.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:36:13.557702 pastas-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-02-07 21:35:52.000000 pastas-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-02-07 21:36:13.553702 pastas-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-02-07 21:35:52.000000 pastas-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:36:13.549702 pastas-1.0.1/pastas/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:36:13.549702 pastas-1.0.1/pastas/io/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/io/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/io/pas.py
--rw-r--r--   0 runner    (1001) docker     (123)    73174 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    32659 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/modelcompare.py
--rw-r--r--   0 runner    (1001) docker     (123)    34886 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/modelplots.py
--rw-r--r--   0 runner    (1001) docker     (123)    11985 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/modelstats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8002 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/noisemodels.py
--rw-r--r--   0 runner    (1001) docker     (123)    30986 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/rcparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    27935 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/recharge.py
--rw-r--r--   0 runner    (1001) docker     (123)    57874 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/rfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21402 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:36:13.553702 pastas-1.0.1/pastas/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13316 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/stats/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    20806 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/stats/dutch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19912 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/stats/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/stats/sgi.py
--rw-r--r--   0 runner    (1001) docker     (123)    32469 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/stats/signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)    18317 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/stats/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    56127 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/stressmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24622 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    15133 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/timeseries_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:36:13.553702 pastas-1.0.1/pastas/typing/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/typing/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-02-07 21:35:53.000000 pastas-1.0.1/pastas/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:36:13.549702 pastas-1.0.1/pastas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-02-07 21:36:13.000000 pastas-1.0.1/pastas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-02-07 21:36:13.000000 pastas-1.0.1/pastas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 21:36:13.000000 pastas-1.0.1/pastas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-07 21:36:13.000000 pastas-1.0.1/pastas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-07 21:36:13.000000 pastas-1.0.1/pastas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-02-07 21:35:53.000000 pastas-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 21:36:13.557702 pastas-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:36:13.553702 pastas-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-07 21:35:53.000000 pastas-1.0.1/tests/test_001.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-02-07 21:35:53.000000 pastas-1.0.1/tests/test_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-02-07 21:35:53.000000 pastas-1.0.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-02-07 21:35:53.000000 pastas-1.0.1/tests/test_gxg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-02-07 21:35:53.000000 pastas-1.0.1/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-02-07 21:35:53.000000 pastas-1.0.1/tests/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-02-07 21:35:53.000000 pastas-1.0.1/tests/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-02-07 21:35:53.000000 pastas-1.0.1/tests/test_qgxg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-02-07 21:35:53.000000 pastas-1.0.1/tests/test_recharge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-02-07 21:35:53.000000 pastas-1.0.1/tests/test_rfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-02-07 21:35:53.000000 pastas-1.0.1/tests/test_signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-02-07 21:35:53.000000 pastas-1.0.1/tests/test_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-02-07 21:35:53.000000 pastas-1.0.1/tests/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:20:40.982362 pastas-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-12 10:20:22.000000 pastas-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-05-12 10:20:40.982362 pastas-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-05-12 10:20:22.000000 pastas-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:20:40.978362 pastas-1.1.0/pastas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:20:40.978362 pastas-1.1.0/pastas/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/io/pas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73119 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35461 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/modelcompare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35559 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/modelplots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/modelstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8002 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/noisemodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31529 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/rcparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27937 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/recharge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56842 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/rfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21402 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:20:40.978362 pastas-1.1.0/pastas/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13317 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/stats/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20806 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/stats/dutch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19940 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/stats/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/stats/sgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32469 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/stats/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18317 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/stats/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56986 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/stressmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26063 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17016 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/timeseries_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:20:40.978362 pastas-1.1.0/pastas/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/typing/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-12 10:20:22.000000 pastas-1.1.0/pastas/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:20:40.978362 pastas-1.1.0/pastas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-05-12 10:20:40.000000 pastas-1.1.0/pastas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-12 10:20:40.000000 pastas-1.1.0/pastas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:20:40.000000 pastas-1.1.0/pastas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-12 10:20:40.000000 pastas-1.1.0/pastas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 10:20:40.000000 pastas-1.1.0/pastas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-05-12 10:20:22.000000 pastas-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 10:20:40.982362 pastas-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:20:40.982362 pastas-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 10:20:22.000000 pastas-1.1.0/tests/test_001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-12 10:20:22.000000 pastas-1.1.0/tests/test_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-12 10:20:22.000000 pastas-1.1.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-12 10:20:22.000000 pastas-1.1.0/tests/test_gxg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-12 10:20:22.000000 pastas-1.1.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-12 10:20:22.000000 pastas-1.1.0/tests/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-12 10:20:22.000000 pastas-1.1.0/tests/test_notebooks_bench.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-12 10:20:22.000000 pastas-1.1.0/tests/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-12 10:20:22.000000 pastas-1.1.0/tests/test_qgxg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-12 10:20:22.000000 pastas-1.1.0/tests/test_recharge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-12 10:20:22.000000 pastas-1.1.0/tests/test_rfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-12 10:20:22.000000 pastas-1.1.0/tests/test_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-12 10:20:22.000000 pastas-1.1.0/tests/test_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-12 10:20:22.000000 pastas-1.1.0/tests/test_stats.py
```

### Comparing `pastas-1.0.1/LICENSE` & `pastas-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pastas-1.0.1/PKG-INFO` & `pastas-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pastas
-Version: 1.0.1
+Version: 1.1.0
 Summary: Pastas is an open-source Python framework for the analysis of groundwater time series.
 Author: Collenteur et al. 2019
-Maintainer-email: "R.A. Collenteur" <raoulcollenteur@gmail.com>, "M. Bakker" <markbak@gmail.com>, "R. Calje" <r.calje@artesia-water.nl>, "F. Schaars" <f.schaars@artesia-water.nl>, "D.A. Brakenhoff" <d.brakenhoff@artesia-water.nl>, "O. Ebbens" <o.ebbens@artesia-water.nl>, "M.A. Vonk" <m.vonk@artesia-water.nl>
+Maintainer-email: "R.A. Collenteur" <raoulcollenteur@gmail.com>, "M. Bakker" <markbak@gmail.com>, "R. Calje" <r.calje@artesia-water.nl>, "F. Schaars" <f.schaars@artesia-water.nl>, "D.A. Brakenhoff" <d.brakenhoff@artesia-water.nl>, "O. Ebbens" <o.ebbens@artesia-water.nl>, "M.A. Vonk" <vonk.mart@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016-2021 R.A. Collenteur, M. Bakker, R. Calje, F. Schaars
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -34,17 +34,20 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+Provides-Extra: solvers
+Provides-Extra: latexify
 Provides-Extra: full
 Provides-Extra: formatting
 Provides-Extra: linting
 Provides-Extra: pytesting
 Provides-Extra: ci
 Provides-Extra: rtd
 Provides-Extra: dev
@@ -101,15 +104,15 @@
 - Pull requests will only be accepted on the development branch (dev) of
   this repository. Please take a look at the `developers section
   <http://pastas.readthedocs.io/>`_ on the documentation website for more
   information on how to contribute to Pastas.
 
 Quick installation guide
 ~~~~~~~~~~~~~~~~~~~~~~~~
-To install Pastas, a working version of Python 3.8, 3.9 or 3.10 has to be
+To install Pastas, a working version of Python 3.8, 3.9, 3.10, 3.11 has to be
 installed on your computer. We recommend using the `Anaconda Distribution
 <https://www.continuum.io/downloads>`_ as it includes most of the python
 package dependencies and the Jupyter Notebook software to run the notebooks.
 However, you are free to install any Python distribution you want.
 
 Stable version
 --------------
@@ -128,14 +131,15 @@
 To get the latest development version, use::
 
    pip install git+https://github.com/pastas/pastas.git@dev#egg=pastas
 
 Related packages
 ~~~~~~~~~~~~~~~~
 - `Pastastore <https://github.com/pastas/pastastore>`_ is a Python package for managing multiple timeseries and pastas models
+- `Metran <https://github.com/pastas/metran>`_ is a Python package to perform multivariate timeseries analysis using a technique called dynamic factor modelling.
 - `Hydropandas <https://github.com/ArtesiaWater/hydropandas/blob/master/examples/03_hydropandas_and_pastas.ipynb>`_ can be used to obtain Dutch timeseries (KNMI, Dinoloket, ..)
 - `PyEt <https://github.com/phydrus/pyet>`_ can be used to compute potential evaporation from meteorological variables.
 
 Dependencies
 ~~~~~~~~~~~~
 Pastas depends on a number of Python packages, of which all of the necessary
 are automatically installed when using the pip install manager. To
```

### Comparing `pastas-1.0.1/README.rst` & `pastas-1.1.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 - Pull requests will only be accepted on the development branch (dev) of
   this repository. Please take a look at the `developers section
   <http://pastas.readthedocs.io/>`_ on the documentation website for more
   information on how to contribute to Pastas.
 
 Quick installation guide
 ~~~~~~~~~~~~~~~~~~~~~~~~
-To install Pastas, a working version of Python 3.8, 3.9 or 3.10 has to be
+To install Pastas, a working version of Python 3.8, 3.9, 3.10, 3.11 has to be
 installed on your computer. We recommend using the `Anaconda Distribution
 <https://www.continuum.io/downloads>`_ as it includes most of the python
 package dependencies and the Jupyter Notebook software to run the notebooks.
 However, you are free to install any Python distribution you want.
 
 Stable version
 --------------
@@ -75,14 +75,15 @@
 To get the latest development version, use::
 
    pip install git+https://github.com/pastas/pastas.git@dev#egg=pastas
 
 Related packages
 ~~~~~~~~~~~~~~~~
 - `Pastastore <https://github.com/pastas/pastastore>`_ is a Python package for managing multiple timeseries and pastas models
+- `Metran <https://github.com/pastas/metran>`_ is a Python package to perform multivariate timeseries analysis using a technique called dynamic factor modelling.
 - `Hydropandas <https://github.com/ArtesiaWater/hydropandas/blob/master/examples/03_hydropandas_and_pastas.ipynb>`_ can be used to obtain Dutch timeseries (KNMI, Dinoloket, ..)
 - `PyEt <https://github.com/phydrus/pyet>`_ can be used to compute potential evaporation from meteorological variables.
 
 Dependencies
 ~~~~~~~~~~~~
 Pastas depends on a number of Python packages, of which all of the necessary
 are automatically installed when using the pip install manager. To
```

### Comparing `pastas-1.0.1/pastas/__init__.py` & `pastas-1.1.0/pastas/__init__.py`

 * *Files identical despite different names*

### Comparing `pastas-1.0.1/pastas/decorators.py` & `pastas-1.1.0/pastas/decorators.py`

 * *Files identical despite different names*

### Comparing `pastas-1.0.1/pastas/io/base.py` & `pastas-1.1.0/pastas/io/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -138,15 +138,19 @@
 
 def _load_stressmodel(ts, data):
     # Create and add stress model
     stressmodel = getattr(ps.stressmodels, ts.pop("class"))
 
     if "rfunc" in ts.keys():
         rfunc_class = ts["rfunc"].pop("class")  # Determine response class
-        ts["rfunc"] = getattr(ps.rfunc, rfunc_class)(**ts["rfunc"])
+        rfunc_up = ts["rfunc"].pop("up", None)  # get up value
+        rfunc_gsf = ts["rfunc"].pop("gain_scale_factor", None)  # get gain_scale_factor
+        rfunc = getattr(ps.rfunc, rfunc_class)(**ts["rfunc"])
+        rfunc.update_rfunc_settings(up=rfunc_up, gain_scale_factor=rfunc_gsf)
+        ts["rfunc"] = rfunc
 
     if "recharge" in ts.keys():
         recharge_class = ts["recharge"].pop("class")
         ts["recharge"] = getattr(ps.recharge, recharge_class)(**ts["recharge"])
 
     metadata = []
     settings = []
```

### Comparing `pastas-1.0.1/pastas/io/pas.py` & `pastas-1.1.0/pastas/io/pas.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,24 @@
 R.A. Collenteur - August 2017
 """
 import datetime
 import json
 from collections import OrderedDict
 from logging import getLogger
 
-from pandas import DataFrame, Series, Timedelta, Timestamp, isna, read_json, to_numeric
+from pandas import (
+    DataFrame,
+    Series,
+    Timedelta,
+    Timestamp,
+    isna,
+    read_json,
+    to_numeric,
+    to_timedelta,
+)
 
 logger = getLogger(__name__)
 
 
 def load(fname: str) -> dict:
     data = json.load(open(fname), object_hook=pastas_hook)
     return data
@@ -63,21 +72,23 @@
     -----
     Currently supported formats are: DataFrame, Series, Timedelta, Timestamps.
 
     see: https://docs.python.org/3/library/json.html
     """
 
     def default(self, o):
-        if isinstance(o, Timestamp) or isinstance(o, datetime.datetime):
+        if isinstance(o, (Timestamp, datetime.datetime)):
             return o.isoformat()
         elif isinstance(o, Series):
             return o.to_json(date_format="iso", orient="split")
         elif isinstance(o, DataFrame):
             # Necessary to maintain order when using the JSON format!
             # Do not use o.to_json() because of float precision
             return json.dumps(o.to_dict(orient="index"), indent=0)
-        elif isinstance(o, Timedelta):
+        elif isinstance(o, (Timedelta, datetime.timedelta)):
+            if isinstance(o, datetime.timedelta):
+                o = to_timedelta(o)
             return o.to_timedelta64().__str__()
         elif isna(o):
             return None
         else:
             return super(PastasEncoder, self).default(o)
```

### Comparing `pastas-1.0.1/pastas/model.py` & `pastas-1.1.0/pastas/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,21 +15,20 @@
     DataFrame,
     DatetimeIndex,
     Series,
     Timedelta,
     Timestamp,
     concat,
     date_range,
-    to_timedelta,
 )
 
 # Internal Pastas
 from pastas.decorators import get_stressmodel
 from pastas.io.base import _load_model, dump
-from pastas.modelplots import Plotting
+from pastas.modelplots import Plotting, _table_formatter_stderr
 from pastas.modelstats import Statistics
 from pastas.noisemodels import NoiseModel
 from pastas.solver import LeastSquares
 from pastas.stressmodels import Constant
 from pastas.timeseries import TimeSeries
 from pastas.timeseries_utils import (
     _frequency_is_supported,
@@ -114,19 +113,15 @@
         self.noisemodel = None
 
         # Default solve/simulation settings
         self.settings = {
             "tmin": None,
             "tmax": None,
             "freq": freq,
-            "warmup": (
-                Timedelta(3650, "D") / Timedelta(freq) * to_timedelta(freq)
-                if freq[0].isdigit()
-                else Timedelta(3650, freq)
-            ),
+            "warmup": Timedelta(3650, "D"),
             "time_offset": Timedelta(0),
             "noise": noisemodel,
             "solver": None,
             "fit_constant": True,
         }
 
         if constant:
@@ -160,15 +155,17 @@
             cls=self.__class__.__name__,
             os=self.oseries.name,
             name=self.name,
             const=True if self.constant else False,
             noise=True if self.noisemodel else False,
         )
 
-    def add_stressmodel(self, stressmodel: StressModel, replace: bool = False) -> None:
+    def add_stressmodel(
+        self, stressmodel: Union[StressModel, List[StressModel]], replace: bool = False
+    ) -> None:
         """Add a stressmodel to the main model.
 
         Parameters
         ----------
         stressmodel: pastas.stressmodel or list of pastas.stressmodel
             instance of a pastas.stressmodel class. Multiple stress models can be
             provided (e.g., ml.add_stressmodel([sm1, sm2]) in one call.
@@ -795,15 +792,15 @@
                 "Calibration series 'oseries_calib' is empty! Check 'tmin' or 'tmax'."
             )
 
         # If a solver is provided, use that one
         if solver is not None:
             self.fit = solver
             self.fit.set_model(self)
-        # Create the default solver is None is provided or already present
+        # Create the default solver if None is provided or already present
         elif self.fit is None:
             self.fit = LeastSquares()
             self.fit.set_model(self)
 
         self.settings["solver"] = self.fit._name
 
         # Solve model
@@ -1741,15 +1738,17 @@
             "Obj": f"{self.fit.obj_func:.2f}",
             "___": "",
             "Interp.": "Yes" if self.interpolate_simulation else "No",
         }
 
         parameters = self.parameters.loc[:, ["optimal", "stderr", "initial", "vary"]]
         stderr = parameters.loc[:, "stderr"] / parameters.loc[:, "optimal"]
-        parameters.loc[:, "stderr"] = stderr.abs().apply("±{:.2%}".format)
+        parameters.loc[:, "stderr"] = "±" + stderr.abs().apply(
+            _table_formatter_stderr, na_rep="nan"
+        )
 
         # Determine the width of the fit_report based on the parameters
         width = len(parameters.to_string().split("\n")[1])
         string = "{:{fill}{align}{width}}"
 
         # Create the first header with model information and stats
         wspace = max(width - (11 + 14 + len(self.name)), 1)
```

### Comparing `pastas-1.0.1/pastas/modelcompare.py` & `pastas-1.1.0/pastas/modelcompare.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """This module contains tools for visually comparing multiple models.
 """
 from itertools import combinations
+from logging import getLogger
 from typing import List, Optional, Tuple
 from warnings import warn
 
 import matplotlib.pyplot as plt
 import numpy as np
 from pandas import DataFrame, concat
 
 import pastas as ps
 from pastas.typing import Axes, Model
 
+logger = getLogger(__name__)
+
 
 class CompareModels:
     """Class for visually comparing pastas Models.
 
     This is a versatile class for constructing visual model comparison plots. The
     default `CompareModels.plot()` method mimics `ml.plots.results()` but allows
     multiple models to be included in the figure. Instead of parameter uncertainties,
@@ -23,18 +26,18 @@
 
     The visualization of each component (i.e. time series, a table) is controlled by
     separate functions allowing users to easily customize their figure. The layout of
     the figure is controlled by a so-called "mosaic", which is essentially a 2D array
     (in the form of nested lists) containing labels that refer to specific axes::
 
         mosaic = [
-            ["sim", "sim", "met"],   # oseries+simulation, and metrics
-            ["sim", "sim", "tab"],   # oseries+simulation and parameters
-            ["res", "res", "tab"],   # residuals+noise and parameters
-            ["con0", "con0", "rf0"]  # contributions and step response
+            ["sim", "sim", "met"],   # oseries+simulation (2x2), metrics       (1x1)
+            ["sim", "sim", "tab"],   # oseries+simulation (2x2), parameters    (2x1)
+            ["res", "res", "tab"],   # residuals+noise    (1x2), parameters    (2x1)
+            ["con0", "con0", "rf0"]  # contributions      (1x2), step response (1x1)
         ]
 
     In this example, the "sim" axis will be 2x2 in the top left portion of the figure
     (with total dimensions (4x3)), while the "met" axis will be 1x1 in the top right.
     Users can either use the default mosaic or provide their own.
 
     Additional logic is available to control plotting of multiple contributions of
@@ -59,27 +62,34 @@
 
         Parameters
         ----------
         models : list of ps.Model, optional
             list of models to compare.
         """
         self.models = models
+        # ensure unique model names
+        modelnames = [iml.name for iml in self.models]
+        if len(set(modelnames)) < len(modelnames):
+            logger.warning("Duplicate model names, appending a suffix.")
+            modelnames = [f"{iml.name}_{i}" for i, iml in enumerate(self.models)]
+        self.modelnames = modelnames
         # attributes that are set and used later
         self.figure = None
         self.axes = None
         self.mosaic = None
         self.cmap = None
         self.adjust_height = False
         self.smdict = None
 
     def initialize_figure(
         self,
         mosaic: Optional[List[List[str]]] = None,
         figsize: Tuple[int, int] = (10, 8),
         cmap: str = "tab10",
+        return_ax: bool = False,
     ) -> None:
         """initialize a custom figure based on a mosaic.
 
         Parameters
         ----------
         mosaic : list, optional
             subplot mosaic, by default None which uses the default mosaic.
@@ -87,19 +97,23 @@
             figure size, by default (10, 8).
         cmap : str, optional
             colormap, by default "tab10".
         """
         if mosaic is None:
             mosaic = self.get_default_mosaic()
 
-        self.mosaic = mosaic
-        figure, axes = plt.subplot_mosaic(self.mosaic, figsize=figsize)
+        self.cmap = plt.get_cmap(cmap)
+
+        figure, axes = plt.subplot_mosaic(mosaic, figsize=figsize)
+        if return_ax:
+            return axes
+
         self.figure = figure
         self.axes = axes
-        self.cmap = plt.get_cmap(cmap)
+        self.mosaic = mosaic
 
     def initialize_adjust_height_figure(
         self,
         mosaic: Optional[List[List[str]]] = None,
         figsize: Tuple[int] = (10, 8),
         cmap: str = "tab10",
         smdict: Optional[dict] = None,
@@ -299,21 +313,24 @@
         Returns
         -------
         metrics : pd.DataFrame
             DataFrame containing calculated metrics.
         """
         if models is None:
             models = self.models
+            modelnames = self.modelnames
+        else:
+            modelnames = [iml.name for iml in models]
 
         metrics = concat(
             [ml.stats.summary(stats=metric_selection) for ml in models],
             axis=1,
             sort=False,
         )
-        metrics.columns = [ml.name for ml in models]
+        metrics.columns = modelnames
         metrics.index.name = None
 
         return metrics
 
     def get_parameters(
         self,
         models: Optional[List[Model]] = None,
@@ -334,17 +351,20 @@
         Returns
         -------
         params : pd.DataFrame
             parameter DataFrame containing parameters for each model.
         """
         if models is None:
             models = self.models
+            modelnames = self.modelnames
+        else:
+            modelnames = [iml.name for iml in models]
 
         params = concat([ml.parameters[param_col] for ml in models], axis=1, sort=False)
-        params.columns = [x.name for x in models]
+        params.columns = modelnames
 
         if param_selection:
             sel = np.array([])
             for sub in param_selection:
                 sel = np.append(sel, [idx for idx in params.index if sub in idx])
             return params.loc[sel].sort_index()
         else:
@@ -360,121 +380,145 @@
         models : list of ps.Model, optional
             list of models to calculate diagnostics for.
         diag_col : str, optional
             name of diagnostics column to obtain, by default "P-value".
         """
         if models is None:
             models = self.models
+            modelnames = self.modelnames
+        else:
+            modelnames = [iml.name for iml in models]
 
-        diags = DataFrame(index=[x.name for x in models])
-        for ml in models:
+        diags = DataFrame(index=modelnames)
+        for i, ml in enumerate(models):
             mldiag = ml.stats.diagnostics()
-            diags.loc[f"{ml.name}", mldiag.index] = mldiag[diag_col].values
+            diags.loc[modelnames[i], mldiag.index] = mldiag[diag_col].values
 
         return diags.transpose()
 
     def plot_oseries(self, axn: str = "sim") -> None:
         """Plot all oseries, unless all oseries are the same.
 
         Parameters
         ----------
         axn : str, optional
             name of labeled axes to plot oseries on, by default "sim".
         """
         if self.axes is None:
-            self.initialize_figure(mosaic=[[axn]], figsize=(10, 3))
+            axs = self.initialize_figure(
+                mosaic=[[axn]], figsize=(10, 3), return_ax=True
+            )
+        else:
+            axs = self.axes
 
         oseries = [ml.oseries.series for ml in self.models]
         equals = np.array([])
         for pair in combinations(oseries, 2):
             equals = np.append(equals, np.array_equal(pair[0], pair[1]))
         if equals.all():
-            self.axes[axn].plot(
+            axs[axn].plot(
                 oseries[0].index,
                 oseries[0].values,
                 label=oseries[0].name,
                 linestyle="",
                 marker="o",
                 color="k",
                 markersize=3,
             )
         else:
             for i, oseries in enumerate(oseries):
-                self.axes[axn].scatter(
+                axs[axn].scatter(
                     oseries.index,
                     oseries.values,
                     label=oseries.name,
                     color=self.cmap(i),
                     s=15,
                     edgecolor="k",
                     linewidth=0.5,
                 )
+        return axs[axn]
 
     def plot_simulation(self, axn: str = "sim") -> None:
         """plot model simulation.
 
         Parameters
         ----------
         axn : str, optional
             name of labeled axes to plot model simulations on, by default "sim".
         """
         if self.axes is None:
-            self.initialize_figure(mosaic=[[axn]], figsize=(10, 3))
+            axs = self.initialize_figure(
+                mosaic=[[axn]], figsize=(10, 3), return_ax=True
+            )
+        else:
+            axs = self.axes
 
         for i, ml in enumerate(self.models):
             simulation = ml.simulate()
-            self.axes[axn].plot(
+            axs[axn].plot(
                 simulation.index,
                 simulation.values,
                 label=ml.name,
                 linestyle="-",
                 color=self.cmap(i),
             )
 
+        return axs[axn]
+
     def plot_residuals(self, axn: str = "res") -> None:
         """plot residuals.
 
         Parameters
         ----------
         axn : str, optional
             name of labeled axes to plot residuals on, by default "res".
         """
         if self.axes is None:
-            self.initialize_figure(mosaic=[[axn]], figsize=(10, 3))
+            axs = self.initialize_figure(
+                mosaic=[[axn]], figsize=(10, 3), return_ax=True
+            )
+        else:
+            axs = self.axes
 
         for i, ml in enumerate(self.models):
             residuals = ml.residuals()
-            self.axes[axn].plot(
+            axs[axn].plot(
                 residuals.index,
                 residuals.values,
                 label="Residuals",
                 color=self.cmap(i),
             )
+        return axs[axn]
 
     def plot_noise(self, axn: str = "res") -> None:
         """plot noise.
 
         Parameters
         ----------
         axn : str, optional
             name of labeled axes to plot noise on, by default "res".
         """
         if self.axes is None:
-            self.initialize_figure(mosaic=[[axn]], figsize=(10, 3))
+            axs = self.initialize_figure(
+                mosaic=[[axn]], figsize=(10, 3), return_ax=True
+            )
+        else:
+            axs = self.axes
 
         for i, ml in enumerate(self.models):
-            noise = ml.noise()
-            if noise is not None:
-                self.axes[axn].plot(
+            if ml.settings["noise"]:
+                noise = ml.noise()
+                axs[axn].plot(
                     noise.index,
                     noise.values,
                     label="Noise",
                     linestyle="--",
                     color=f"C{i}",
                 )
+        return axs[axn]
 
     def plot_response(
         self, smdict: Optional[dict] = None, axn: str = "rf{i}", response: str = "step"
     ) -> None:
         """plot step or block responses.
 
         Parameters
@@ -491,15 +535,17 @@
             label, e.g. key 0 indicates the response functions will be plotted on
             axes with label 'rf0'. Otherwise, each response function will be plotted
             on a separate subplot (i.e. 'rf0', 'rf1', ...).
         response : str, optional
             type of response to plot, either "step" or "block", by default "step".
         """
         if self.axes is None:
-            self.initialize_figure(mosaic=[[axn]], figsize=(5, 3))
+            axs = self.initialize_figure(
+                mosaic=[[axn.format(i=0)]], figsize=(5, 3), return_ax=True
+            )
 
         if smdict is None and self.smdict is None:
             self.smdict = {
                 i: [smn] for i, smn in enumerate(self.get_unique_stressmodels())
             }
         elif smdict is not None and self.smdict is None:
             self.smdict = smdict
@@ -508,28 +554,48 @@
             for j, namlist in self.smdict.items():
                 for smn in namlist:
                     # skip if contribution not in model
                     if smn not in ml.stressmodels:
                         continue
                     if response == "step":
                         step = ml.get_step_response(smn, add_0=True)
-                        self.axes[axn.format(i=j)].plot(
-                            step.index,
-                            step.values,
-                            label=f"{smn}",
-                            color=self.cmap(i),
-                        )
+                        if step is None:
+                            continue
+                        if self.axes is None:
+                            axs[axn.format(i=0)].plot(
+                                step.index,
+                                step.values,
+                                label=f"{smn}",
+                            )
+                        else:
+                            self.axes[axn.format(i=j)].plot(
+                                step.index,
+                                step.values,
+                                label=f"{smn}",
+                                color=self.cmap(i),
+                            )
                     elif response == "block":
                         block = ml.get_block_response(smn)
-                        self.axes[axn.format(i=j)].semilogx(
-                            block.index,
-                            block.values,
-                            label=f"{smn}",
-                            color=self.cmap(i),
-                        )
+                        if block is None:
+                            continue
+                        if self.axes is None:
+                            axs[axn.format(i=0)].semilogx(
+                                block.index,
+                                block.values,
+                                label=f"{smn}",
+                            )
+                        else:
+                            self.axes[axn.format(i=j)].semilogx(
+                                block.index,
+                                block.values,
+                                label=f"{smn}",
+                                color=self.cmap(i),
+                            )
+        if self.axes is None:
+            return axs[axn.format(i=0)]
 
     def plot_contribution(
         self,
         smdict: Optional[dict] = None,
         axn: str = "con{i}",
         normalized: bool = False,
     ) -> None:
@@ -550,15 +616,17 @@
             with label 'con0'. Otherwise, each contribution will be plotted on a
             separate subplot (i.e. 'con0', 'con1', ...).
         normalized : bool, optional
             normalize contributions with min/max depending on mean value, by default
             False.
         """
         if self.axes is None:
-            self.initialize_figure(mosaic=[[axn]], figsize=(10, 3))
+            axs = self.initialize_figure(
+                mosaic=[[axn.format(i=0)]], figsize=(10, 3), return_ax=True
+            )
 
         if smdict is None and self.smdict is None:
             if self.adjust_height:
                 warn(
                     "When combining stressmodels into one subplot in combination "
                     "with 'adjust_height', provide 'smdict' to "
                     "`initialize_adjust_height_figure()` for best results."
@@ -579,108 +647,129 @@
                             label = f"{con.name}"
                             if normalized:
                                 label += " (normalized)"
                                 if con.mean() < 0:
                                     con -= con.max()
                                 else:
                                     con -= con.min()
-
-                            self.axes[axn.format(i=j)].plot(
-                                con.index,
-                                con.values,
-                                label=label,
-                                color=self.cmap(i),
-                            )
+                            if self.axes is None:
+                                axs[axn.format(i=0)].plot(
+                                    con.index,
+                                    con.values,
+                                    label=label,
+                                )
+                            else:
+                                self.axes[axn.format(i=j)].plot(
+                                    con.index,
+                                    con.values,
+                                    label=label,
+                                    color=self.cmap(i),
+                                )
+        if self.axes is None:
+            return axs[axn.format(i=0)]
 
     def plot_stress(
         self, axn: str = "stress", names: Optional[List[str]] = None
     ) -> None:
         """plot stresses time series.
 
         Parameters
         ----------
         axn : str, optional
             name of labeled axes to plot stresses on, by default "stress".
         names : list of str, optional
             names of stresses to plot, by default None.
         """
         if self.axes is None:
-            self.initialize_figure(mosaic=[[axn]], figsize=(10, 3))
+            axs = self.initialize_figure(
+                mosaic=[[axn]], figsize=(10, 3), return_ax=True
+            )
+        else:
+            axs = self.axes
 
         if names is None:
             names = self.get_unique_stressmodels()
 
         for i, ml in enumerate(self.models):
             for smn in names:
                 if smn in ml.get_stressmodel_names():
                     stress = ml.get_stress(smn)
-                    self.axes[axn].plot(
+                    axs[axn].plot(
                         stress.index,
                         stress.values,
                         label=f"{smn}",
                         color=self.cmap(i),
                     )
+        return axs[axn]
 
     def plot_acf(self, axn: str = "acf") -> None:
         """plot autocorrelation plot.
 
         Parameters
         ----------
         axn : str, optional
             name of labeled axes to plot ACF on, by default "acf".
         """
         if self.axes is None:
-            self.initialize_figure(mosaic=[[axn]], figsize=(10, 3))
+            axs = self.initialize_figure(
+                mosaic=[[axn]], figsize=(10, 3), return_ax=True
+            )
+        else:
+            axs = self.axes
 
         for i, ml in enumerate(self.models):
             if ml.noise() is not None:
                 r = ps.stats.core.acf(ml.noise(), full_output=True)
                 label = "Autocorrelation Noise"
             else:
                 r = ps.stats.core.acf(ml.residuals(), full_output=True)
                 label = "Autocorrelation Residuals"
             conf = r.conf.rolling(10, min_periods=1).mean().values
 
-            self.axes[axn].fill_between(
+            axs[axn].fill_between(
                 r.index.days, conf, -conf, alpha=0.3, color=self.cmap(i)
             )
-            self.axes[axn].vlines(
+            axs[axn].vlines(
                 r.index.days,
                 [0],
                 r.loc[:, "acf"].values,
                 color=self.cmap(i),
                 label=label,
             )
+        return axs[axn]
 
     def plot_table(self, axn: str = "table", df: Optional[DataFrame] = None) -> None:
         """Plot dataframe as table.
 
         Parameters
         ----------
         axn : str, optional
             name of labeled axes to plot table on, by default "table".
         df : pandas.DataFrame, optional
             The Pandas.Dataframe to plot. Note that the first column is the index
             column that is shown.
         """
         if self.axes is None:
-            self.initialize_figure(mosaic=[[axn]], figsize=(6, 4))
+            axs = self.initialize_figure(mosaic=[[axn]], figsize=(6, 4), return_ax=True)
+        else:
+            axs = self.axes
 
         if df is None:
             df = DataFrame(["empty"])
 
-        self.axes[axn].table(
+        axs[axn].table(
             df.values.tolist(),
             colLabels=df.columns,
             colColours=[(1.0, 1.0, 1.0, 1.0)]
             + [self.cmap(i, alpha=0.75) for i in range(len(df.columns) - 1)],
             bbox=(0.0, 0.0, 1.0, 1.0),
         )
-        self.axes[axn].set_xticks([])
-        self.axes[axn].set_yticks([])
+        axs[axn].set_xticks([])
+        axs[axn].set_yticks([])
+        return axs[axn]
 
     def plot_table_params(
         self,
         axn: str = "tab",
         param_col: str = "optimal",
         param_selection: Optional[List[str]] = None,
     ) -> None:
@@ -692,82 +781,73 @@
             name of labeled axes to plot table on, by default "tab"
         param_col : str, optional
             name of parameter column to include, by default "optimal"
         param_selection : list of str, optional
             string to filter parameter names that are included in table, by default
             None.
         """
-        if self.axes is None:
-            self.initialize_figure(mosaic=[[axn]], figsize=(6, 4))
-
         params = self.get_parameters(
             self.models,
             param_selection=param_selection,
             param_col=param_col,
         ).applymap(ps.plots._table_formatter_params)
 
-        # add seperate column with parameter names
+        # add separate column with parameter names
         params.loc[:, "Parameters"] = params.index
         cols = params.columns.to_list()[-1:] + params.columns.to_list()[:-1]
-        self.plot_table(axn=axn, df=params[cols])
+        return self.plot_table(axn=axn, df=params[cols])
 
     def plot_table_metrics(
         self, axn: str = "met", metric_selection: Optional[List[str]] = None
     ) -> None:
         """plot metrics table.
 
         Parameters
         ----------
         axn : str, optional
             name of labeled axes to plot table on, by default "met"
         metric_selection : list, optional
             list of str describing which metrics to include, by default None which
             uses ["rsq", "aic"].
         """
-        if self.axes is None:
-            self.initialize_figure(mosaic=[[axn]], figsize=(6, 4))
-
         if metric_selection is None:
             metric_selection = ["rsq", "aic"]
 
         metrics = self.get_metrics(self.models, metric_selection=metric_selection)
         for met in ["aic", "bic"]:
             if met in metrics.index:
                 metrics.loc[met] -= metrics.loc[met].min()
                 metrics = metrics.rename(
                     index={met: f"\N{GREEK CAPITAL LETTER DELTA}{met.upper()}"}
                 )
         if "rsq" in metrics.index:
-            metrics = metrics.rename(index={"rsq": f"R\N{SUPERSCRIPT TWO}"})
+            metrics = metrics.rename(index={"rsq": "R\N{SUPERSCRIPT TWO}"})
 
         # add seperate column with parameter names
         metrics.loc[:, "Metrics"] = metrics.index
         cols = metrics.columns.to_list()[-1:] + metrics.columns.to_list()[:-1]
-        self.plot_table(axn=axn, df=metrics[cols].round(2))
+        return self.plot_table(axn=axn, df=metrics[cols].round(2))
 
     def plot_table_diagnostics(
         self, axn: str = "diag", diag_col: str = "P-value"
     ) -> None:
         """plot diagnostics table.
 
         Parameters
         ----------
         axn : str, optional
             name of labeled axis to plot table on, by default "diag".
         diag_col : str, optional
             name of diagnostics column to obtain, by default "P-value".
         """
-        if self.axes is None:
-            self.initialize_figure(mosaic=[[axn]], figsize=(6, 4))
-
         # add seperate column with parameter names
         diags = self.get_diagnostics(self.models, diag_col=diag_col)
         diags.loc[:, f"Test\n{diag_col}"] = diags.index
         cols = diags.columns.to_list()[-1:] + diags.columns.to_list()[:-1]
-        self.plot_table(axn=axn, df=diags[cols])
+        return self.plot_table(axn=axn, df=diags[cols])
 
     def share_xaxes(self, axes: List[Axes]) -> None:
         """share x-axes.
 
         Parameters
         ----------
         axes : list of matplotlib.Axes
@@ -835,37 +915,39 @@
         self.adjust_height = adjust_height
         if self.axes is None and not self.adjust_height:
             self.initialize_figure(figsize=figsize)
         if self.axes is None and self.adjust_height:
             self.initialize_adjust_height_figure(smdict=smdict, figsize=figsize)
 
         # sim
-        self.plot_oseries()
-        self.plot_simulation()
+        _ = self.plot_oseries()
+        _ = self.plot_simulation()
 
         # res
-        self.plot_residuals()
-        self.plot_noise()
+        _ = self.plot_residuals()
+        _ = self.plot_noise()
 
         # smn, rfn
-        self.plot_contribution(smdict=smdict, normalized=normalized)
-        self.plot_response(smdict=smdict)
+        _ = self.plot_contribution(smdict=smdict, normalized=normalized)
+        _ = self.plot_response(smdict=smdict)
 
         # share x-axes
         xshare_left = []
         xshare_right = []
         for axn in self.axes.keys():
             if axn not in ("tab", "met", "dia"):
                 self.axes[axn].grid(grid)
                 if legend and not axn.startswith("rf"):
                     if legend_kwargs is None:
                         legend_kwargs = {}
-                    _, l = self.axes[axn].get_legend_handles_labels()
+                    _, labels = self.axes[axn].get_legend_handles_labels()
                     self.axes[axn].legend(
-                        ncol=legend_kwargs.pop("ncol", max([int(np.ceil(len(l))), 4])),
+                        ncol=legend_kwargs.pop(
+                            "ncol", max([int(np.ceil(len(labels))), 4])
+                        ),
                         loc=legend_kwargs.pop("loc", (0, 1)),
                         frameon=legend_kwargs.pop("frameon", False),
                         markerscale=legend_kwargs.pop("markerscale", 1.0),
                         numpoints=legend_kwargs.pop("numpoints", 3),
                         **legend_kwargs,
                     )
             if axn in ("sim", "res") or axn.startswith("con"):
@@ -875,13 +957,13 @@
 
         if len(xshare_left) > 1:
             self.share_xaxes(xshare_left)
         if len(xshare_right) > 1:
             self.share_xaxes(xshare_right)
 
         # met
-        self.plot_table_metrics()
+        _ = self.plot_table_metrics()
 
         # tab
-        self.plot_table_params(param_selection=param_selection)
+        _ = self.plot_table_params(param_selection=param_selection)
 
         self.figure.tight_layout(pad=0.0)
```

### Comparing `pastas-1.0.1/pastas/modelplots.py` & `pastas-1.1.0/pastas/modelplots.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Type Hinting
 from typing import List, Optional, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.backends.backend_pdf import PdfPages
 from matplotlib.ticker import LogFormatter, MultipleLocator
-from pandas import Series, concat
+from pandas import Series, Timestamp, concat
 
 from pastas.typing import Axes, Figure, Model, TimestampType
 
 from .decorators import model_tmin_tmax
 from .plots import (
     _table_formatter_params,
     _table_formatter_stderr,
@@ -98,14 +98,19 @@
 
         if simulation:
             sim = self.ml.simulate(tmin=tmin, tmax=tmax)
             r2 = round(self.ml.stats.rsq(tmin=tmin, tmax=tmax) * 100, 1)
             sim.plot(ax=ax, label=f"{sim.name} ($R^2$ = {r2}%)")
 
         # Dress up the plot
+        # temporary fix, as set_xlim currently does not work with strings mpl=3.6.1
+        if tmin is not None:
+            tmin = Timestamp(tmin)
+        if tmax is not None:
+            tmax = Timestamp(tmax)
         ax.set_xlim(tmin, tmax)
         ax.set_ylabel("Groundwater levels [meter]")
         ax.set_title("Results of {}".format(self.ml.name))
 
         if legend:
             ax.legend(ncol=2, numpoints=3)
         plt.tight_layout()
@@ -279,14 +284,20 @@
 
         if axb is not None:
             axb.set_xlim(rmin, rmax)
 
         # xlim sets minorticks back after plots:
         ax1.minorticks_off()
 
+        # temporary fix, as set_xlim currently does not work with strings mpl=3.6.1
+        if tmin is not None:
+            tmin = Timestamp(tmin)
+        if tmax is not None:
+            tmax = Timestamp(tmax)
+
         if return_warmup:
             ax1.set_xlim(tmin - self.ml.settings["warmup"], tmax)
         else:
             ax1.set_xlim(tmin, tmax)
 
         # sometimes, ticks suddenly appear on top plot, turn off just in case
         plt.setp(ax1.get_xticklabels(), visible=False)
@@ -470,14 +481,19 @@
                     locator = MultipleLocator(base=ytick_base)
                     ax.yaxis.set_major_locator(locator)
                 ax.set_title(names[i])
                 ax.set_ylim(ylims[i + 1])
             ax.grid(True)
             ax.minorticks_off()
         if set_axes_properties:
+            # temporary fix, as set_xlim currently does not work with strings mpl=3.6.1
+            if tmin is not None:
+                tmin = Timestamp(tmin)
+            if tmax is not None:
+                tmax = Timestamp(tmax)
             axes[0].set_xlim(tmin, tmax)
         fig.tight_layout(pad=0.0)
 
         return axes
 
     @model_tmin_tmax
     def diagnostics(
@@ -862,15 +878,15 @@
                     h = self.ml.get_contribution(sm, tmin=tmin, tmax=tmax)
                     name = sm
                     contributions.append((name, h))
                 contributions.sort(key=custom_sort)
 
                 # add stacked plot to correct axes
                 ax = axes[i - 1]
-                del ax.lines[0]  # delete existing line
+                ax.lines[0].remove()  # delete existing line
 
                 contrib = [c[1] for c in contributions]  # get time series
                 vstack = concat(contrib, axis=1, sort=False)
                 names = [c[0] for c in contributions]  # get names
                 ax.stackplot(vstack.index, vstack.values.T, labels=names)
                 if stacklegend:
                     if stacklegend_kws is None:
```

### Comparing `pastas-1.0.1/pastas/modelstats.py` & `pastas-1.1.0/pastas/modelstats.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 # Type Hinting
 from typing import List, Optional
 
 from numpy import nan
 from pandas import DataFrame
 
 from pastas.typing import Model, TimestampType
+
 from .decorators import model_tmin_tmax
 from .stats import diagnostics, metrics
 
 
 class Statistics:
     # Save all statistics that can be calculated.
     ops = [
```

### Comparing `pastas-1.0.1/pastas/noisemodels.py` & `pastas-1.1.0/pastas/noisemodels.py`

 * *Files identical despite different names*

### Comparing `pastas-1.0.1/pastas/plots.py` & `pastas-1.1.0/pastas/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 
 
 def series(
     head: Optional[Series] = None,
     stresses: Optional[List[Series]] = None,
     hist: bool = True,
     kde: bool = False,
+    table: bool = False,
     titles: bool = True,
     tmin: Optional[TimestampType] = None,
     tmax: Optional[TimestampType] = None,
     labels: Optional[List[str]] = None,
     figsize: tuple = (10, 5),
 ) -> Axes:
     """Plot all the input time Series in a single plot.
@@ -68,19 +69,21 @@
     ----------
     head: pd.Series
         Pandas time series with DatetimeIndex.
     stresses: List of pd.Series
         List with Pandas time series with DatetimeIndex.
     hist: bool
         Histogram for the series. The number of bins is determined with Sturges rule.
-        Returns the number of observations, mean, skew and kurtosis.
     kde: bool
         Kernel density estimate for the series. The kde is obtained from
         scipy.gaussian_kde using scott to calculate the estimator bandwidth. Returns
         the number of observations, mean, skew and kurtosis.
+    table: bool
+        Show table with some basic statistics such as the number of
+        observations, mean, skew and kurtosis.
     titles: bool
         Set the titles or not. Taken from the name attribute of the series.
     tmin: str or pd.Timestamp
     tmax: str or pd.Timestamp
     labels: List of str
         List with the labels for each subplot.
     figsize: tuple
@@ -98,19 +101,24 @@
         if tmax is None:
             tmax = head.index[-1]
     if stresses is not None:
         rows += len(stresses)
     sharex = True
     gridspec_kw = {}
     cols = 1
+    if table and not hist and kde:
+        hist = True
     if hist or kde:
         sharex = False
-        gridspec_kw["width_ratios"] = (3, 1, 1)
-        cols = 3
-    _, axes = plt.subplots(
+        gridspec_kw["width_ratios"] = [3, 1]
+        cols += 1
+        if table:
+            cols += 1
+            gridspec_kw["width_ratios"].append(1)
+    fig, axes = plt.subplots(
         rows,
         cols,
         figsize=figsize,
         sharex=sharex,
         sharey="row",
         gridspec_kw=gridspec_kw,
     )
@@ -158,15 +166,15 @@
                 1000,
             )
             if hist:
                 colour = "C1"
             else:
                 colour = "k"
             axes[0, 1].plot(gkde.evaluate(ind), ind, color=colour)
-        if hist or kde:
+        if table:
             # stats table
             head_stats = [
                 ["Count", f"{head.count():0.0f}"],
                 ["Mean", f"{head.mean():0.2f}"],
                 ["Max", f"{head.max():0.2f}"],
                 ["Min", f"{head.min():0.2f}"],
                 ["Skew", f"{head.skew():0.2f}"],
@@ -213,32 +221,38 @@
                     1000,
                 )
                 if hist:
                     colour = "C1"
                 else:
                     colour = "k"
                 axes[i, 1].plot(gkde.evaluate(ind), ind, color=colour)
-            if hist or kde:
+            if table:
                 if i > 0:
                     axes[i, 0].sharex(axes[0, 0])
                 # stats table
                 stress_stats = [
                     ["Count", f"{stress.count():0.0f}"],
                     ["Mean", f"{stress.mean():0.2f}"],
                     ["Skew", f"{stress.skew():0.2f}"],
                     ["Kurtosis", f"{stress.kurtosis():0.2f}"],
                 ]
                 axes[i, 2].table(
                     bbox=(0, 0, 1, 1), colWidths=(1.5, 1), cellText=stress_stats
                 )
                 axes[i, 2].axis("off")
+
+    # temporary fix, as set_xlim currently does not work with strings mpl=3.6.1
+    if tmin is not None:
+        tmin = Timestamp(tmin)
+    if tmax is not None:
+        tmax = Timestamp(tmax)
     axes[0, 0].set_xlim([tmin, tmax])
     axes[0, 0].minorticks_off()
 
-    plt.tight_layout()
+    fig.tight_layout()
     return axes
 
 
 def acf(
     series: Series,
     alpha: float = 0.05,
     lags: int = 365,
@@ -721,15 +735,17 @@
             handle to the figure.
         """
         # create plot
         self.fig, self.axes = plt.subplots(3, 1, figsize=figsize, dpi=dpi)
         self.ax0, self.ax1, self.ax2 = self.axes
 
         # share x-axes between 2nd and 3rd axes
-        self.ax1.get_shared_x_axes().join(self.ax1, self.ax2)
+        self.ax1.sharex(self.ax2)
+        for t in self.ax1.get_xticklabels():
+            t.set_visible(False)
 
         # plot oseries
         self.ax0.plot(
             self.obs.index,
             self.obs,
             marker=".",
             ls="none",
@@ -851,29 +867,31 @@
         self.simplot.set_data(sim.index, sim.values)
 
         # update rmse residuals
         self.r_rmse_plot_line.set_data(
             range(self.itercount + 1), np.array(self.rmse_res)
         )
         self.r_rmse_plot_dot.set_data(
-            np.array([self.itercount]), np.array(self.rmse_res[-1])
+            np.array([self.itercount]), np.array([self.rmse_res[-1]])
         )
 
         if self.ml.settings["noise"] and self.ml.noisemodel is not None:
             # update rmse noise
             self.n_rmse_plot_line.set_data(
                 range(self.itercount + 1), np.array(self.rmse_noise)
             )
             self.n_rmse_plot_dot.set_data(
-                np.array([self.itercount]), np.array(self.rmse_noise[-1])
+                np.array([self.itercount]), np.array([self.rmse_noise[-1]])
             )
 
         # update parameter plots
         for j, (p1, p2) in enumerate(self.param_plot_handles):
-            p1.set_data(np.array([self.itercount]), np.abs(self.parameters.iloc[-1, j]))
+            p1.set_data(
+                np.array([self.itercount]), np.abs([self.parameters.iloc[-1, j]])
+            )
             p2.set_data(
                 range(self.itercount + 1), self.parameters.iloc[:, j].abs().values
             )
 
         # update title
         self.ax0.set_title(
             "Iteration: {0} (EVP: {1:.2f}%)".format(self.itercount, self.evp[-1])
@@ -906,51 +924,51 @@
         self.fig.axes[1].set_xlim(left=0)
         # because of bug with autoscaling log axis?
         self.fig.axes[1].set_ylim(top=1.05 * self.rmse_res.max())
 
         return fig.axes
 
 
-def _table_formatter_params(s: float) -> str:
+def _table_formatter_params(s: float, na_rep: str = "") -> str:
     """Internal method for formatting parameters in tables in Pastas plots.
 
     Parameters
     ----------
     s : float
         value to format.
 
     Returns
     -------
     str
         float formatted as str.
     """
     if np.isnan(s):
-        return ""
+        return na_rep
     elif np.floor(np.log10(np.abs(s))) <= -2:
         return f"{s:.2e}"
     elif np.floor(np.log10(np.abs(s))) > 5:
         return f"{s:.2e}"
     else:
         return f"{s:.2f}"
 
 
-def _table_formatter_stderr(s: float) -> str:
+def _table_formatter_stderr(s: float, na_rep: str = "") -> str:
     """Internal method for formatting stderrs in tables in Pastas plots.
 
     Parameters
     ----------
     s : float
         value to format.
 
     Returns
     -------
     str
         float formatted as str.
     """
     if np.isnan(s):
-        return ""
+        return na_rep
     elif np.floor(np.log10(np.abs(s))) <= -4:
         return f"{s * 100.:.2e}%"
     elif np.floor(np.log10(np.abs(s))) > 3:
         return f"{s * 100.:.2e}%"
     else:
         return f"{s:.2%}"
```

### Comparing `pastas-1.0.1/pastas/rcparams.py` & `pastas-1.1.0/pastas/rcparams.py`

 * *Files identical despite different names*

### Comparing `pastas-1.0.1/pastas/recharge.py` & `pastas-1.1.0/pastas/recharge.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 # Type Hinting
 from typing import Tuple, Union
 
 from numpy import add, exp, float64, multiply, nan_to_num, power, vstack, where, zeros
 from pandas import DataFrame
 
 from pastas.typing import ArrayLike
+
 from .decorators import njit
 
 logger = getLogger(__name__)
 
 
 class RechargeBase:
     """Base class for classes that calculate the recharge."""
```

### Comparing `pastas-1.0.1/pastas/rfunc.py` & `pastas-1.1.0/pastas/rfunc.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,24 +51,33 @@
 
 
 class RfuncBase:
     _name = "RfuncBase"
 
     def __init__(
         self,
-        up: bool = True,
-        gain_scale_factor: float = 1.0,
         cutoff: float = 0.999,
         **kwargs,
     ) -> None:
-        self.up = up
-        self.gain_scale_factor = gain_scale_factor
         self.cutoff = cutoff
+        if "up" in kwargs:
+            raise TypeError(
+                "keyword argument 'up' is not supported in init. "
+                "Set with update_rfunc_settings()."
+            )
+        if "gain_scale_factor" in kwargs:
+            raise TypeError(
+                "keyword argument 'gain_scale_factor' is not supported in "
+                "init. Set with update_rfunc_settings()."
+            )
+        # initialize attributes, these can be set with update_rfunc_settings()
+        self.up = None
+        self.gain_scale_factor = 1.0
 
-    def _update_rfunc_settings(
+    def update_rfunc_settings(
         self,
         up: Optional[bool] = "nochange",
         gain_scale_factor: Optional[float] = None,
         cutoff: Optional[float] = None,
     ) -> None:
         """Internal method to set the settings of the response function.
 
@@ -298,22 +307,18 @@
     The Gamma function is equal to the Exponential function when n=1.
     """
 
     _name = "Gamma"
 
     def __init__(
         self,
-        up: bool = True,
-        gain_scale_factor: float = 1.0,
         cutoff: float = 0.999,
         **kwargs,
     ) -> None:
-        RfuncBase.__init__(
-            self, up=up, gain_scale_factor=gain_scale_factor, cutoff=cutoff, **kwargs
-        )
+        RfuncBase.__init__(self, cutoff=cutoff, **kwargs)
         self.nparam = 3
 
     def get_init_parameters(self, name: str) -> DataFrame:
         parameters = DataFrame(columns=["initial", "pmin", "pmax", "vary", "name"])
         if self.up:
             parameters.loc[name + "_A"] = (
                 1 / self.gain_scale_factor,
@@ -394,22 +399,18 @@
 
     """
 
     _name = "Exponential"
 
     def __init__(
         self,
-        up: bool = True,
-        gain_scale_factor: float = 1.0,
         cutoff: float = 0.999,
         **kwargs,
     ) -> None:
-        RfuncBase.__init__(
-            self, up=up, gain_scale_factor=gain_scale_factor, cutoff=cutoff, **kwargs
-        )
+        RfuncBase.__init__(self, cutoff=cutoff, **kwargs)
         self.nparam = 2
 
     def get_init_parameters(self, name: str) -> DataFrame:
         parameters = DataFrame(columns=["initial", "pmin", "pmax", "vary", "name"])
         if self.up:
             parameters.loc[name + "_A"] = (
                 1 / self.gain_scale_factor,
@@ -499,24 +500,20 @@
     The implementation used here is explained in :cite:t:`veling_hantush_2010`.
     """
 
     _name = "HantushWellModel"
 
     def __init__(
         self,
-        up: bool = True,
-        gain_scale_factor: float = 1.0,
         cutoff: float = 0.999,
         use_numba: bool = False,
         quad: bool = False,
         **kwargs,
     ) -> None:
-        RfuncBase.__init__(
-            self, up=up, gain_scale_factor=gain_scale_factor, cutoff=cutoff, **kwargs
-        )
+        RfuncBase.__init__(self, cutoff=cutoff, **kwargs)
         self.distances = None
         self.nparam = 3
         self.use_numba = use_numba  # requires numba_scipy for real speedups
         self.quad = quad  # if quad=True, implicitly uses numba
         # check numba and numba_scipy installation
         if self.quad or self.use_numba:
             # turn off use_numba if numba_scipy is not available
@@ -791,24 +788,20 @@
 
     """
 
     _name = "Hantush"
 
     def __init__(
         self,
-        up: bool = True,
-        gain_scale_factor: float = 1.0,
         cutoff: float = 0.999,
         use_numba: bool = False,
         quad: bool = False,
         **kwargs,
     ) -> None:
-        RfuncBase.__init__(
-            self, up=up, gain_scale_factor=gain_scale_factor, cutoff=cutoff, **kwargs
-        )
+        RfuncBase.__init__(self, cutoff=cutoff, **kwargs)
         self.nparam = 3
         self.use_numba = use_numba
         self.quad = quad
         # check numba and numba_scipy installation
         if self.quad or self.use_numba:
             # turn off use_numba if numba_scipy is not available
             # or there is a version conflict
@@ -986,22 +979,18 @@
 
     """
 
     _name = "Polder"
 
     def __init__(
         self,
-        up: bool = True,
-        gain_scale_factor: float = 1.0,
         cutoff: float = 0.999,
         **kwargs,
     ) -> None:
-        RfuncBase.__init__(
-            self, up=up, gain_scale_factor=gain_scale_factor, cutoff=cutoff, **kwargs
-        )
+        RfuncBase.__init__(self, cutoff=cutoff, **kwargs)
         self.nparam = 3
 
     def get_init_parameters(self, name) -> DataFrame:
         parameters = DataFrame(columns=["initial", "pmin", "pmax", "vary", "name"])
         parameters.loc[name + "_A"] = (1, 0, 2, True, name)
         parameters.loc[name + "_a"] = (10, 0.01, 1000, True, name)
         parameters.loc[name + "_b"] = (1, 1e-6, 25, True, name)
@@ -1070,22 +1059,18 @@
         this response function.
     """
 
     _name = "One"
 
     def __init__(
         self,
-        up: bool = True,
-        gain_scale_factor: float = 1.0,
         cutoff: float = 0.999,
         **kwargs,
     ) -> None:
-        RfuncBase.__init__(
-            self, up=up, gain_scale_factor=gain_scale_factor, cutoff=cutoff, **kwargs
-        )
+        RfuncBase.__init__(self, cutoff=cutoff, **kwargs)
         self.nparam = 1
 
     def get_init_parameters(self, name: str) -> DataFrame:
         parameters = DataFrame(columns=["initial", "pmin", "pmax", "vary", "name"])
         if self.up:
             parameters.loc[name + "_d"] = (
                 self.gain_scale_factor,
@@ -1167,23 +1152,19 @@
 
     """
 
     _name = "FourParam"
 
     def __init__(
         self,
-        up: bool = True,
-        gain_scale_factor: float = 1.0,
         cutoff: float = 0.999,
         quad: bool = False,
         **kwargs,
     ) -> None:
-        RfuncBase.__init__(
-            self, up=up, gain_scale_factor=gain_scale_factor, cutoff=cutoff, **kwargs
-        )
+        RfuncBase.__init__(self, cutoff=cutoff, **kwargs)
         self.nparam = 4
         self.quad = quad
 
     def get_init_parameters(self, name: str) -> DataFrame:
         parameters = DataFrame(columns=["initial", "pmin", "pmax", "vary", "name"])
         if self.up:
             parameters.loc[name + "_A"] = (
@@ -1381,22 +1362,18 @@
 
     """
 
     _name = "DoubleExponential"
 
     def __init__(
         self,
-        up: bool = True,
-        gain_scale_factor: float = 1.0,
         cutoff: float = 0.999,
         **kwargs,
     ) -> None:
-        RfuncBase.__init__(
-            self, up=up, gain_scale_factor=gain_scale_factor, cutoff=cutoff, **kwargs
-        )
+        RfuncBase.__init__(self, cutoff=cutoff, **kwargs)
         self.nparam = 4
 
     def get_init_parameters(self, name: str) -> DataFrame:
         parameters = DataFrame(columns=["initial", "pmin", "pmax", "vary", "name"])
         if self.up:
             parameters.loc[name + "_A"] = (
                 1 / self.gain_scale_factor,
@@ -1485,22 +1462,18 @@
 
     """
 
     _name = "Edelman"
 
     def __init__(
         self,
-        up: bool = True,
-        gain_scale_factor: float = 1.0,
         cutoff: float = 0.999,
         **kwargs,
     ) -> None:
-        RfuncBase.__init__(
-            self, up=up, gain_scale_factor=gain_scale_factor, cutoff=cutoff, **kwargs
-        )
+        RfuncBase.__init__(self, cutoff=cutoff, **kwargs)
         self.nparam = 1
 
     def get_init_parameters(self, name: str) -> DataFrame:
         parameters = DataFrame(columns=["initial", "pmin", "pmax", "vary", "name"])
         beta_init = 1.0
         parameters.loc[name + "_beta"] = (beta_init, 0, 1000, True, name)
         return parameters
@@ -1574,23 +1547,19 @@
 
     """
 
     _name = "Kraijenhoff"
 
     def __init__(
         self,
-        up: bool = True,
-        gain_scale_factor: float = 1.0,
         cutoff: float = 0.999,
         n_terms: int = 10,
         **kwargs,
     ) -> None:
-        RfuncBase.__init__(
-            self, up=up, gain_scale_factor=gain_scale_factor, cutoff=cutoff, **kwargs
-        )
+        RfuncBase.__init__(self, cutoff=cutoff, **kwargs)
         self.nparam = 3
         self.n_terms = n_terms
 
     def get_init_parameters(self, name: str) -> DataFrame:
         parameters = DataFrame(columns=["initial", "pmin", "pmax", "vary", "name"])
         if self.up:
             parameters.loc[name + "_A"] = (
@@ -1719,24 +1688,20 @@
     response functions, that probably describe the groundwater system better.
     """
 
     _name = "Spline"
 
     def __init__(
         self,
-        up: bool = True,
-        gain_scale_factor: float = 1.0,
         cutoff: float = 0.999,
         kind: str = "quadratic",
         t: Optional[list] = None,
         **kwargs,
     ) -> None:
-        RfuncBase.__init__(
-            self, up=up, gain_scale_factor=gain_scale_factor, cutoff=cutoff, **kwargs
-        )
+        RfuncBase.__init__(self, cutoff=cutoff, **kwargs)
         self.kind = kind
         if t is None:
             t = [1, 2, 4, 8, 16, 32, 64, 128, 256, 512, 1024]
         self.t = t
         self.nparam = len(t) + 1
 
     def get_init_parameters(self, name: str) -> DataFrame:
```

### Comparing `pastas-1.0.1/pastas/solver.py` & `pastas-1.1.0/pastas/solver.py`

 * *Files identical despite different names*

### Comparing `pastas-1.0.1/pastas/stats/__init__.py` & `pastas-1.1.0/pastas/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `pastas-1.0.1/pastas/stats/core.py` & `pastas-1.1.0/pastas/stats/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     pi,
     sqrt,
 )
 from pandas import DataFrame, Series, Timedelta, TimedeltaIndex
 from scipy.stats import norm
 
 from pastas.typing import ArrayLike
+
 from ..decorators import njit
 
 
 def acf(
     x: Series,
     lags: ArrayLike = 365,
     bin_method: str = "rectangle",
```

### Comparing `pastas-1.0.1/pastas/stats/dutch.py` & `pastas-1.1.0/pastas/stats/dutch.py`

 * *Files identical despite different names*

### Comparing `pastas-1.0.1/pastas/stats/metrics.py` & `pastas-1.1.0/pastas/stats/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 """
 
 from logging import getLogger
 
 # Type Hinting
 from typing import Optional
 
-from numpy import abs, average, log, nan, sqrt
+from numpy import abs as npabs
+from numpy import average, log, nan, sqrt
 from pandas import Series
 
 from pastas.stats.core import _get_weights, mean, std, var
 
 __all__ = [
     "rmse",
     "sse",
@@ -83,15 +84,15 @@
 
     # Return nan if the time indices of the sim and obs don't match
     if err.index.size == 0:
         logger.warning("Time indices of the sim and obs don't match.")
         return nan
 
     w = _get_weights(err, weighted=weighted, max_gap=max_gap)
-    return (w * abs(err.to_numpy())).sum()
+    return (w * npabs(err.to_numpy())).sum()
 
 
 def rmse(
     obs: Optional[Series] = None,
     sim: Optional[Series] = None,
     res: Optional[Series] = None,
     missing: str = "drop",
```

### Comparing `pastas-1.0.1/pastas/stats/sgi.py` & `pastas-1.1.0/pastas/stats/sgi.py`

 * *Files identical despite different names*

### Comparing `pastas-1.0.1/pastas/stats/signatures.py` & `pastas-1.1.0/pastas/stats/signatures.py`

 * *Files identical despite different names*

### Comparing `pastas-1.0.1/pastas/stats/tests.py` & `pastas-1.1.0/pastas/stats/tests.py`

 * *Files identical despite different names*

### Comparing `pastas-1.0.1/pastas/stressmodels.py` & `pastas-1.1.0/pastas/stressmodels.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
 from pandas import DataFrame, Series, Timedelta, Timestamp, concat, date_range
 from scipy.signal import fftconvolve
 
 from pastas.typing import ArrayLike, Model, Recharge, RFunc, TimestampType
+
 from .decorators import njit, set_parameter
 from .recharge import Linear
 from .rfunc import Exponential, HantushWellModel, One
 from .timeseries import TimeSeries
 from .utils import validate_name
 
 logger = getLogger(__name__)
@@ -68,15 +69,15 @@
     ) -> None:
         self.name = validate_name(name)
         self.tmin = tmin
         self.tmax = tmax
         self.freq = None
 
         if rfunc is not None:
-            rfunc._update_rfunc_settings(up=up, gain_scale_factor=gain_scale_factor)
+            rfunc.update_rfunc_settings(up=up, gain_scale_factor=gain_scale_factor)
         self.rfunc = rfunc
 
         self.parameters = DataFrame(columns=["initial", "pmin", "pmax", "vary", "name"])
 
         self.stress = []
 
     @property
@@ -619,97 +620,102 @@
 class WellModel(StressModelBase):
     """Convolution of one or more stresses with a single scaled response function.
 
     Parameters
     ----------
     stress: list
         list containing the stresses time series.
-    rfunc: pastas.rfunc instance
-        this model only works with the HantushWellModel response function.
     name: str
-        Name of the stressmodel.
+        name of the stressmodel.
     distances: array_like
-        list of distances to oseries, must be ordered the same as the stresses.
+        array_like of distances between the stresses (wells) and the oseries
+        (monitoring well), must be in the same order as the stresses. This
+        distance is used to scale the HantushWellModel response function for
+        each stress.
+    rfunc: pastas.rfunc instance, optional
+        this model only works with the HantushWellModel response function, default is
+        None which will initialize a HantushWellModel response function.
     up: bool, optional
         whether a positive stress has an increasing or decreasing effect on the model,
         by default False, in which case positive stress lowers e.g., the groundwater
         level.
     settings: str, list of dict, optional
-        The settings of the stress. This can be a string referring to a predefined
-        settings dict (defined in ps.rcParams["timeseries"]), or a dict with the
-        settings to apply. Refer to the docs of pastas.Timeseries for further
-        information.
+        The settings of the stress. By default this is "well". This can be a string
+        referring to a predefined settings dict (defined in
+        ps.rcParams["timeseries"]), or a dict with the settings to apply. Refer
+        to the docs of pastas.Timeseries for further information.
     sort_wells: bool, optional
         sort wells from closest to furthest, by default True.
 
     Notes
     -----
     This class implements convolution of multiple series with the same response
     function. This can be applied when dealing with multiple wells in a time series
     model. The distance(s) from the pumping well(s) to the monitoring well have to be
     provided for each stress.
 
-    Warnings
-    --------
-    This model only works with the HantushWellModel response function.
+    Only works with the HantushWellModel response function.
     """
 
     _name = "WellModel"
 
     def __init__(
         self,
         stress: List[Series],
-        rfunc: RFunc,
         name: str,
         distances: ArrayLike,
+        rfunc: Optional[RFunc] = None,
         up: bool = False,
         settings: str = "well",
         sort_wells: bool = True,
         metadata: Optional[list] = None,
     ) -> None:
-        if not isinstance(rfunc, HantushWellModel):
+        # check response function
+        if rfunc is None:
+            rfunc = HantushWellModel()
+        elif not isinstance(rfunc, HantushWellModel):
             raise NotImplementedError(
                 "WellModel only supports the rfunc HantushWellModel!"
             )
 
-        # sort wells by distance
-        self.sort_wells = sort_wells
-        if self.sort_wells:
-            stress = [
-                s for _, s in sorted(zip(distances, stress), key=lambda pair: pair[0])
-            ]
-            if isinstance(settings, list):
-                settings = [
-                    s
-                    for _, s in sorted(
-                        zip(distances, settings), key=lambda pair: pair[0]
-                    )
-                ]
-
-            distances = np.sort(distances)
-
-        if settings is None or isinstance(settings, str) or isinstance(settings, dict):
-            settings = len(stress) * [settings]
-
-        # convert stresses to TimeSeries if necessary
-        stress = self._handle_stress(stress, settings)
-
-        # Check if number of stresses and distances match
+        # check if number of stresses and distances match
         if len(stress) != len(distances):
             msg = (
                 "The number of stresses does not match the number of distances "
                 "provided."
             )
             logger.error(msg)
             raise ValueError(msg)
         else:
             self.distances = Series(
-                index=[s.name for s in stress], data=distances, name="distances"
+                index=[s.squeeze().name for s in stress],
+                data=distances,
+                name="distances",
             )
 
+        # parse settings input
+        if settings is None or isinstance(settings, str) or isinstance(settings, dict):
+            settings = len(stress) * [settings]
+
+        # if metadata is passed as dict -> convert to list
+        if metadata is not None and isinstance(metadata, dict):
+            metadata = [metadata]
+
+        # parse stresses input
+        stress = self._handle_stress(stress, settings, metadata)
+
+        # sort wells by distance
+        self.sort_wells = sort_wells
+        if self.sort_wells:
+            stress = [
+                s for _, s in sorted(zip(distances, stress), key=lambda pair: pair[0])
+            ]
+            distances = np.sort(distances)
+
+        # estimate gain_scale_factor w/ max of stresses stdev
         gain_scale_factor = np.max([s.series.std() for s in stress])
 
         tmin = np.min([s.series.index.min() for s in stress])
         tmax = np.max([s.series.index.max() for s in stress])
 
         StressModelBase.__init__(
             self,
@@ -760,41 +766,56 @@
             else:
                 h.name = self.name + "_" + str(istress)
         else:
             h.name = self.name
         return h
 
     @staticmethod
-    def _handle_stress(stress, settings):
+    def _handle_stress(stress, settings, metadata):
         """Internal method to handle user provided stress in init.
 
         Parameters
         ----------
         stress: pandas.Series, list or dict
             stress or collection of stresses.
         settings: dict or iterable
             settings dictionary.
+        metadata : dict or list of dict
+            metadata dictionaries corresponding to stress
 
         Returns
         -------
         stress: list
-            return a list with the stresses transformed to pastas.TimeSeries.
+            return a list with the stresses transformed to pastas TimeSeries.
         """
         data = []
 
         if isinstance(stress, Series):
-            data.append(TimeSeries(stress, settings=settings))
+            data.append(TimeSeries(stress, settings=settings, metadata=metadata))
         elif isinstance(stress, dict):
             for i, (name, value) in enumerate(stress.items()):
-                data.append(TimeSeries(value, name=name, settings=settings[i]))
+                if metadata is not None:
+                    imeta = metadata[i]
+                else:
+                    imeta = None
+                data.append(
+                    TimeSeries(value, name=name, settings=settings[i], metadata=imeta)
+                )
         elif isinstance(stress, list):
             for i, value in enumerate(stress):
-                data.append(TimeSeries(value, settings=settings[i]))
+                if metadata is not None:
+                    imeta = metadata[i]
+                else:
+                    imeta = None
+                data.append(TimeSeries(value, settings=settings[i], metadata=imeta))
         else:
-            logger.error("Stress format is unknown. Provide a Series, dict or list.")
+            msg = "Cannot parse 'stress' input. Provide a Series, dict or list."
+            logger.error(msg)
+            raise TypeError(msg)
+
         return data
 
     def get_stress(
         self,
         p: Optional[ArrayLike] = None,
         tmin: Optional[TimestampType] = None,
         tmax: Optional[TimestampType] = None,
@@ -1407,15 +1428,14 @@
         elif dmin is None or dmax is None:
             msg = "Please specify either oseries or dmin and dmax"
             raise (Exception(msg))
         if rfunc is None:
             rfunc = Exponential()
         if not isinstance(rfunc, Exponential):
             raise NotImplementedError("TarsoModel only supports rfunc Exponential!")
-        self.oseries = oseries
         self.dmin = dmin
         self.dmax = dmax
         super().__init__(prec=prec, evap=evap, rfunc=rfunc, **kwargs)
 
     def set_init_parameters(self) -> None:
         # parameters for the first drainage level
         p0 = self.rfunc.get_init_parameters(self.name)
@@ -1478,15 +1498,14 @@
         -----
         Settings and metadata are exported with the stress.
 
         """
         data = super().to_dict(series)
         data["dmin"] = self.dmin
         data["dmax"] = self.dmax
-        data["oseries"] = self.oseries
         return data
 
     @staticmethod
     def _check_stressmodel_compatibility(ml: Model) -> None:
         """Internal method to check if no other stressmodels, a constants or a
         transform is used."""
         msg = (
@@ -1601,18 +1620,18 @@
             self,
             name=name,
             rfunc=None,
             tmin=stress.series.index.min(),
             tmax=stress.series.index.max(),
         )
 
-        rfunc1._update_rfunc_settings(up=up)
+        rfunc1.update_rfunc_settings(up=up)
         self.rfunc1 = rfunc1
 
-        rfunc2._update_rfunc_settings(up=up)
+        rfunc2.update_rfunc_settings(up=up)
         self.rfunc2 = rfunc2
         self.tchange = Timestamp(tchange)
 
         self.freq = stress.settings["freq"]
         self.stress.append(stress)
         self.set_init_parameters()
```

### Comparing `pastas-1.0.1/pastas/timer.py` & `pastas-1.1.0/pastas/timer.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,26 +15,24 @@
 
     Optimization progress: 73it [00:01, 67.68it/s]
 
 """
 
 try:
     from tqdm.auto import tqdm
-except ModuleNotFoundError:
-    raise ModuleNotFoundError("SolveTimer requires 'tqdm' to be installed.")
+except ModuleNotFoundError as e:
+    raise e("SolveTimer requires 'tqdm' to be installed.")
 
 # Type Hinting
 from typing import Optional
 
 
 class ExceededMaxSolveTime(Exception):
     """Custom Exception when model optimization exceeds threshold."""
 
-    pass
-
 
 class SolveTimer(tqdm):
     """Progress indicator for model optimization.
 
     Examples
     --------
     Print timer and number of iterations in console while running `ml.solve()`::
@@ -69,18 +67,18 @@
             ExceededMaxSolveTime Exception.
         """
         if "total" not in kwargs:
             kwargs["total"] = None
         if "desc" not in kwargs:
             kwargs["desc"] = "Optimization progress"
         self.max_time = max_time
-        super(SolveTimer, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     def timer(self, _, n: int = 1):
         """Callback method for ps.Model.solve()."""
-        displayed = super(SolveTimer, self).update(n)
+        displayed = super().update(n)
         if self.max_time is not None:
             if self.format_dict["elapsed"] > self.max_time:
                 raise ExceededMaxSolveTime(
                     "Model solve time exceeded" f" {self.max_time} seconds!"
                 )
         return displayed
```

### Comparing `pastas-1.0.1/pastas/timeseries.py` & `pastas-1.1.0/pastas/timeseries.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Optional, Union
 
 import pandas as pd
 from pandas import Series
 from pandas.tseries.frequencies import to_offset
 
 from .rcparams import rcParams
-from .timeseries_utils import _get_dt, _get_time_offset
+from .timeseries_utils import _get_dt, _get_time_offset, _infer_fixed_freq, resample
 from .utils import validate_name
 
 logger = getLogger(__name__)
 
 
 class TimeSeries:
     """Class that deals with all user-provided time series.
@@ -78,16 +78,16 @@
                         "because the stress time series  need to be equidistant. "
                         "Please change this."
                     )
             validate_stress(series)
 
         # Store a copy of the original series
         self._series_original = series.copy()  # copy of the original series
-        self._series = None  #
-        self.freq_original = pd.infer_freq(self._series_original.index)
+        self._series = None
+        self.freq_original = _infer_fixed_freq(self._series_original.index)
         self.settings = {
             "freq": self.freq_original,
             "sample_up": None,
             "sample_down": None,
             "fill_nan": "interpolate",
             "fill_before": None,
             "fill_after": None,
@@ -323,28 +323,25 @@
         series = series.loc[start_time:]
 
         # TODO: replace by adding offset to resample method with pandas 1.1.0
         # Shift time series back by offset so resample can take it into account
         if self.settings["time_offset"] > pd.Timedelta(0):
             series = series.shift(-1, freq=self.settings["time_offset"])
 
-        # Provide some standard pandas arguments for all options
-        kwargs = {"label": "right", "closed": "right"}
-
         success = True
         if method == "mean":
-            series = series.resample(freq, **kwargs).mean()
+            series = resample(series, freq).mean()
         elif method == "drop":
-            series = series.resample(freq, **kwargs).mean().dropna()
+            series = resample(series, freq).mean().dropna()
         elif method == "sum":
-            series = series.resample(freq, **kwargs).sum()
+            series = resample(series, freq).sum()
         elif method == "min":
-            series = series.resample(freq, **kwargs).min()
+            series = resample(series, freq).min()
         elif method == "max":
-            series = series.resample(freq, **kwargs).max()
+            series = resample(series, freq).max()
         else:
             success = False
 
         # TODO: replace by adding offset to resample method with pandas 1.1.0
         if self.settings["time_offset"] > pd.Timedelta(0):
             # The offset is removed by the resample-method, so we add it again
             series = series.shift(1, freq=self.settings["time_offset"])
@@ -427,14 +424,24 @@
                 logger.info(
                     "Time Series %s was extended in the past to %s with the mean "
                     "value (%.2g) of the time series.",
                     self.name,
                     series.index.min(),
                     mean_value,
                 )
+            elif method == "bfill":
+                first_value = series.loc[series.first_valid_index()]
+                series = series.fillna(method="bfill")  # Default option
+                logger.info(
+                    "Time Series %s was extended in the past to %s with the first "
+                    "value (%.2g) of the time series.",
+                    self.name,
+                    series.index.min(),
+                    first_value,
+                )
             elif isinstance(method, float):
                 series = series.fillna(method)
                 logger.info(
                     "Time Series %s was extended in the past to %s by adding %s "
                     "values.",
                     self.name,
                     series.index.min(),
@@ -477,14 +484,24 @@
                 logger.info(
                     "Time Series %s was extended in the future to %s with the mean "
                     "value (%.2g) of the time series.",
                     self.name,
                     series.index.max(),
                     mean_value,
                 )
+            elif method == "ffill":
+                last_value = series.loc[series.last_valid_index()]
+                series = series.fillna(method="ffill")
+                logger.info(
+                    "Time Series %s was extended in the future to %s with the last "
+                    "value (%.2g) of the time series.",
+                    self.name,
+                    series.index.max(),
+                    last_value,
+                )
             elif isinstance(method, float):
                 series = series.fillna(method)
                 logger.info(
                     "Time Series %s was extended in the future to %s by adding %s "
                     "values.",
                     self.name,
                     series.index.max(),
@@ -574,17 +591,18 @@
     -----
     The Series are validated for the following cases:
 
     0. Make sure the series is a Pandas.Series
     1. Make sure the values are floats
     2. Make sure the index is a DatetimeIndex
     3. Make sure the indices are datetime64
-    4. Make sure the index is monotonically increasing
-    5. Make sure there are no duplicate indices
-    6. Make sure the time series has no nan-values
+    4. Make sure the index has no NaT-values
+    5. Make sure the index is monotonically increasing
+    6. Make sure there are no duplicate indices
+    7. Make sure the time series has no nan-values
 
     If any of these checks are not passed the method will throw an error that needs
     to be fixed by the user.
 
     Examples
     --------
 
@@ -610,14 +628,19 @@
     to be fixed by the user.
 
     """
     # Because we are friendly and allow 1D DataFrames
     if isinstance(series, pd.DataFrame):
         if len(series.columns) == 1:
             series = series.iloc[:, 0]
+        elif len(series.columns) > 1:
+            # helpful specific message for multi-column DataFrames
+            msg = "DataFrame with multiple columns. Please select one."
+            logger.error(msg)
+            raise ValueError(msg)
 
     # 0. Make sure it is a Series and not something else (e.g., DataFrame)
     if not isinstance(series, pd.Series):
         msg = f"Expected a Pandas Series, got {type(series)}"
         logger.error(msg)
         raise ValueError(msg)
 
@@ -637,42 +660,52 @@
 
     # 3. Make sure the indices are datetime64
     if not pd.api.types.is_datetime64_dtype(series.index):
         msg = f"Indices os series {name} are not datetime64."
         logger.error(msg)
         raise ValueError(msg)
 
-    # 4. Make sure the index is monotonically increasing
+    # 4. Make sure there are no NaT in index
+    if series.index.hasnans:
+        msg = (
+            f"The index of series {name} contains NaNs. "
+            "Try to remove these with `series.loc[series.index.dropna()]`."
+        )
+        logger.error(msg)
+        raise ValueError(msg)
+
+    # 5. Make sure the index is monotonically increasing
     if not series.index.is_monotonic_increasing:
         msg = (
             f"The time-indices of series {name} are not monotonically increasing. Try "
             f"to use `series.sort_index()` to fix it."
         )
         logger.error(msg)
         raise ValueError(msg)
 
-    # 5. Make sure there are no duplicate indices
+    # 6. Make sure there are no duplicate indices
     if not series.index.is_unique:
         msg = (
             f"duplicate time-indexes were found in the time series {name}. Make sure "
-            f"there are no duplicate indices. For example by "
-            f"`grouped = series.groupby(level=0); series = grouped.mean()`"
+            "there are no duplicate indices. For example by "
+            "`grouped = series.groupby(level=0); series = grouped.mean()`"
+            "or `series = series.loc[~series.index.duplicated(keep='first/last')]`"
         )
         logger.error(msg)
         raise ValueError(msg)
 
-    # 6. Make sure the time series has no nan-values
+    # 7. Make sure the time series has no nan-values
     if series.hasnans:
         msg = (
             "The time series %s has nan-values. Pastas will use the fill_nan "
             "settings to fill up the nan-values."
         )
         logger.warning(msg, name)
 
-    # 7. Make sure the time series has equidistant time steps
+    # 8. Make sure the time series has equidistant time steps
     if equidistant:
         if not pd.infer_freq(series.index):
             msg = (
                 f"The frequency of the index of time series {name} could not be "
                 f"inferred. Please provide a time series with a regular time step."
             )
             logger.error(msg)
```

### Comparing `pastas-1.0.1/pastas/timeseries_utils.py` & `pastas-1.1.0/pastas/timeseries_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import logging
 
 # Type Hinting
 from typing import Optional
 
 import numpy as np
-from pandas import Index, Series, Timedelta, Timestamp, api, date_range
+from pandas import Index, Series, Timedelta, Timestamp, api, date_range, infer_freq
+from pandas.core.resample import Resampler
 from pandas.tseries.frequencies import to_offset
 from scipy import interpolate
 
 from .decorators import njit
 
 logger = logging.getLogger(__name__)
 
@@ -78,21 +79,23 @@
     Notes
     -----
     Used for comparison to determine if a time series needs to be up or downsampled.
 
     See http://pandas.pydata.org/pandas-docs/stable/timeseries.html#offset-aliases
     for the offset_aliases supported by Pandas.
     """
+    if freq is None:
+        return None
     # Get the frequency string and multiplier
     offset = to_offset(freq)
     if hasattr(offset, "delta"):
         dt = offset.delta / Timedelta(1, "D")
     else:
         num = offset.n
-        freq = offset.name
+        freq = offset._prefix
         if freq in ["A", "Y", "AS", "YS", "BA", "BY", "BAS", "BYS"]:
             # year
             dt = num * 365
         elif freq in ["BQ", "BQS", "Q", "QS"]:
             # quarter
             dt = num * 90
         elif freq in ["BM", "BMS", "CBM", "CBMS", "M", "MS"]:
@@ -150,14 +153,42 @@
     """
     if freq is None:
         raise TypeError("frequency is None")
 
     return t - t.floor(freq)
 
 
+def _infer_fixed_freq(tindex: Index) -> str:
+    """Internal method to get the frequency string.
+
+    This methods avoids returning anchored offsets, e.g.
+    'W-TUE' will return 7D.
+
+    Parameters
+    ----------
+    tindex : Index
+        DateTimeIndex
+
+    Returns
+    -------
+    str
+        frequency string
+    """
+    freq = infer_freq(tindex)
+    if freq is None:
+        return freq
+
+    offset = to_offset(freq)
+    if to_offset(offset.rule_code).is_anchored():
+        dt = _get_stress_dt(freq)
+        return f"{dt}D"
+
+    return freq
+
+
 def get_sample(tindex: Index, ref_tindex: Index) -> Index:
     """Sample the index so that the frequency is not higher than the frequency
     of ref_tindex.
 
     Parameters
     ----------
     tindex: pandas.Index
@@ -321,17 +352,15 @@
     sampling (meaning observations can be shifted in time), with additional filling
     logic that ensures each original measurement is only included once in the new
     time series. Values are filled as close as possible to their original timestamp
     in the new equidistant time series.
     """
 
     # build new equidistant index
-    idx = date_range(
-        series.index[0].floor(freq), series.index[-1].ceil(freq), freq=freq
-    )
+    idx = date_range(series.index[0], series.index[-1], freq=freq)
 
     # get linear interpolated index from original series
     fl = interpolate.interp1d(
         series.index.asi8,
         np.arange(0, series.index.size),
         kind="linear",
         bounds_error=False,
@@ -434,17 +463,17 @@
 
     Note: this method will shift observations in time and can introduce duplicate
     observations.
 
     Parameters
     ----------
     series : str
-        _description_
+        time series.
     freq : str
-        _description_
+        frequency string.
     tolerance : str, optional
         frequency type string (e.g. '7D') specifying maximum distance between original
         and new labels for inexact matches.
 
     Returns
     -------
     Series
@@ -486,7 +515,43 @@
         series.reset_index()
         .drop_duplicates(subset="index", keep="first", inplace=False)
         .set_index("index")
         .asfreq(freq)
         .squeeze()
     )
     return spandas
+
+
+def resample(
+    series: Series, freq: str, closed: str = "right", label: str = "right", **kwargs
+) -> Resampler:
+    """Resample time-series data.
+
+    Convenience method for frequency conversion and resampling of time series.
+    This function is a wrapper around Pandas' resample function with some
+    logical Pastas defaults. In Pastas, we assume the timestamp is at the end
+    of the period that belongs to each measurement. For more information on
+    this read the example notebook on preprocessing time series.
+
+    Parameters
+    ----------
+    series : pandas Series
+        Time series. The index must be a datetime-like index
+        (`DatetimeIndex`, `PeriodIndex`, or `TimedeltaIndex`).
+    freq : str
+        Frequency string.
+    closed: str, default 'right'
+        Which side/end of bin interval is closed.
+    label: str, default 'right'
+        Which bin edge label to label bucket with.
+    **kwargs: dict
+
+    Returns
+    -------
+    Resampler
+        pandas Resampler object which can be manipulated using methods such as:
+        '.interpolate()', '.mean()', '.max()' etc. For all options see:
+        https://pandas.pydata.org/docs/reference/resampling.html
+
+    """
+
+    return series.resample(freq, closed=closed, label=label, **kwargs)
```

### Comparing `pastas-1.0.1/pastas/transform.py` & `pastas-1.1.0/pastas/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 
 class ThresholdTransform:
     """ThresholdTransform lowers the simulation when it exceeds a certain value.
 
     Parameters
     ----------
     value : float, optional
-        The starting value above which the simulation is lowered.
+        The initial starting value above which the simulation is lowered.
     vmin : float, optional
         The minimum value above which the simulation is lowered.
-    vmin : float, optional
+    vmax : float, optional
         The maximum value above which the simulation is lowered.
     name: str, optional
         Name of the transform.
     nparam : int, optional
         The number of parameters. Default is nparam=2. The first parameter then is
         the threshold, and the second parameter is the factor with which the
         simulation is lowered.
```

### Comparing `pastas-1.0.1/pastas/typing/types.py` & `pastas-1.1.0/pastas/typing/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 # flake8: noqa
 # Type hinting for Pastas library
 # Typing
 from typing import TYPE_CHECKING, Any, Callable, TypeVar, Union
 
 # External libraries
 # Matplotlib
-from matplotlib.axes._base import _AxesBase
-from matplotlib.figure import FigureBase
+from matplotlib.axes import Axes as MatplotlibAxes
+from matplotlib.figure import Figure as MatplotlibFigure
 
 # Numpy
 from numpy.typing import ArrayLike as NumpyArrayLike
 
 # Pandas
 from pandas import Timestamp
 
 # External Types
-Axes = TypeVar("Axes", bound=_AxesBase)  # Matplotlib Axes
-Figure = TypeVar("Figure", bound=FigureBase)  # Matplotlib Figure
+Axes = TypeVar("Axes", bound=MatplotlibAxes)  # Matplotlib Axes
+Figure = TypeVar("Figure", bound=MatplotlibFigure)  # Matplotlib Figure
 ArrayLike = TypeVar("ArrayLike", bound=NumpyArrayLike)  # Array Like (NumPy based)
 
 # Internal library
 if TYPE_CHECKING:  # https://mypy.readthedocs.io/en/latest/runtime_troubles.html
     import pastas as ps
 
 # Internal Types
 TimestampType = TypeVar("TimestampType", bound=Union[str, Timestamp])  # Tmin or Tmax
 Model = TypeVar("Model", bound="ps.Model")  # Model
-TimeSeries = TypeVar("TimeSeries", bound="ps.TimeSeries")  # Time Series
+TimeSeries = TypeVar("TimeSeries", bound="ps.timeseries.TimeSeries")  # Time Series
 StressModel = TypeVar(
     "StressModel", bound="ps.stressmodels.StressModelBase"
 )  # Stress Model
 NoiseModel = TypeVar("NoiseModel", bound="ps.noisemodels.NoiseModelBase")  # Noise Model
 Solver = TypeVar("Solver", bound="ps.solver.BaseSolver")  # Base Solver
 Recharge = TypeVar("Recharge", bound="ps.recharge.RechargeBase")  # Recharge Base
-Reservoir = TypeVar("Reservoir", bound="ps.reservoir.ReservoirBase")  # Reservoir Base
 CallBack = TypeVar("CallBack", bound=Any)  # Callback
 Function = Callable[..., Any]  # Function (e.g. Objective Function)
 RFunc = TypeVar("RFunc", bound="ps.rfunc.RfuncBase")  # rFunc Base
```

### Comparing `pastas-1.0.1/pastas/utils.py` & `pastas-1.1.0/pastas/utils.py`

 * *Files identical despite different names*

### Comparing `pastas-1.0.1/pastas/version.py` & `pastas-1.1.0/pastas/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from importlib import import_module, metadata
 from platform import python_version
 
 logger = logging.getLogger(__name__)
 
-__version__ = "1.0.1"
+__version__ = "1.1.0"
 
 
 def check_numba_scipy() -> bool:
     try:
         import_module("numba_scipy")
     except ModuleNotFoundError:
         logger.warning(
```

### Comparing `pastas-1.0.1/pastas.egg-info/PKG-INFO` & `pastas-1.1.0/pastas.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pastas
-Version: 1.0.1
+Version: 1.1.0
 Summary: Pastas is an open-source Python framework for the analysis of groundwater time series.
 Author: Collenteur et al. 2019
-Maintainer-email: "R.A. Collenteur" <raoulcollenteur@gmail.com>, "M. Bakker" <markbak@gmail.com>, "R. Calje" <r.calje@artesia-water.nl>, "F. Schaars" <f.schaars@artesia-water.nl>, "D.A. Brakenhoff" <d.brakenhoff@artesia-water.nl>, "O. Ebbens" <o.ebbens@artesia-water.nl>, "M.A. Vonk" <m.vonk@artesia-water.nl>
+Maintainer-email: "R.A. Collenteur" <raoulcollenteur@gmail.com>, "M. Bakker" <markbak@gmail.com>, "R. Calje" <r.calje@artesia-water.nl>, "F. Schaars" <f.schaars@artesia-water.nl>, "D.A. Brakenhoff" <d.brakenhoff@artesia-water.nl>, "O. Ebbens" <o.ebbens@artesia-water.nl>, "M.A. Vonk" <vonk.mart@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016-2021 R.A. Collenteur, M. Bakker, R. Calje, F. Schaars
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -34,17 +34,20 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+Provides-Extra: solvers
+Provides-Extra: latexify
 Provides-Extra: full
 Provides-Extra: formatting
 Provides-Extra: linting
 Provides-Extra: pytesting
 Provides-Extra: ci
 Provides-Extra: rtd
 Provides-Extra: dev
@@ -101,15 +104,15 @@
 - Pull requests will only be accepted on the development branch (dev) of
   this repository. Please take a look at the `developers section
   <http://pastas.readthedocs.io/>`_ on the documentation website for more
   information on how to contribute to Pastas.
 
 Quick installation guide
 ~~~~~~~~~~~~~~~~~~~~~~~~
-To install Pastas, a working version of Python 3.8, 3.9 or 3.10 has to be
+To install Pastas, a working version of Python 3.8, 3.9, 3.10, 3.11 has to be
 installed on your computer. We recommend using the `Anaconda Distribution
 <https://www.continuum.io/downloads>`_ as it includes most of the python
 package dependencies and the Jupyter Notebook software to run the notebooks.
 However, you are free to install any Python distribution you want.
 
 Stable version
 --------------
@@ -128,14 +131,15 @@
 To get the latest development version, use::
 
    pip install git+https://github.com/pastas/pastas.git@dev#egg=pastas
 
 Related packages
 ~~~~~~~~~~~~~~~~
 - `Pastastore <https://github.com/pastas/pastastore>`_ is a Python package for managing multiple timeseries and pastas models
+- `Metran <https://github.com/pastas/metran>`_ is a Python package to perform multivariate timeseries analysis using a technique called dynamic factor modelling.
 - `Hydropandas <https://github.com/ArtesiaWater/hydropandas/blob/master/examples/03_hydropandas_and_pastas.ipynb>`_ can be used to obtain Dutch timeseries (KNMI, Dinoloket, ..)
 - `PyEt <https://github.com/phydrus/pyet>`_ can be used to compute potential evaporation from meteorological variables.
 
 Dependencies
 ~~~~~~~~~~~~
 Pastas depends on a number of Python packages, of which all of the necessary
 are automatically installed when using the pip install manager. To
```

### Comparing `pastas-1.0.1/pastas.egg-info/SOURCES.txt` & `pastas-1.1.0/pastas.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 pastas/typing/types.py
 tests/test_001.py
 tests/test_comparison.py
 tests/test_examples.py
 tests/test_gxg.py
 tests/test_model.py
 tests/test_notebooks.py
+tests/test_notebooks_bench.py
 tests/test_plots.py
 tests/test_qgxg.py
 tests/test_recharge.py
 tests/test_rfuncs.py
 tests/test_signatures.py
 tests/test_solvers.py
 tests/test_stats.py
```

### Comparing `pastas-1.0.1/pyproject.toml` & `pastas-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 [build-system]
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
-
 [project]
 name = "pastas"
 dynamic = ["version"]
 description = "Pastas is an open-source Python framework for the analysis of groundwater time series."
 license = { file = "LICENSE" }
 readme = "README.rst"
 authors = [{ name = "Collenteur et al. 2019" }]
 maintainers = [
     { name = "R.A. Collenteur", email = "raoulcollenteur@gmail.com" },
     { name = "M. Bakker", email = "markbak@gmail.com" },
     { name = "R. Calje", email = "r.calje@artesia-water.nl" },
     { name = "F. Schaars", email = "f.schaars@artesia-water.nl" },
     { name = "D.A. Brakenhoff", email = "d.brakenhoff@artesia-water.nl" },
     { name = "O. Ebbens", email = "o.ebbens@artesia-water.nl" },
-    { name = "M.A. Vonk", email = "m.vonk@artesia-water.nl" },
+    { name = "M.A. Vonk", email = "vonk.mart@gmail.com" },
 ]
 requires-python = ">= 3.8"
 dependencies = [
     "numpy >= 1.17, < 1.24",
     "matplotlib >= 3.1",
     "pandas >= 1.1",
     "scipy >= 1.8",
@@ -33,91 +32,101 @@
     'Intended Audience :: Science/Research',
     'Intended Audience :: Other Audience',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3 :: Only',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Topic :: Scientific/Engineering :: Hydrology',
 ]
 
 [project.urls]
 homepage = "https://pastas.dev"
 repository = "https://github.com/pastas/pastas"
 documentation = "https://pastas.readthedocs.io/en/latest/"
 
 [project.optional-dependencies]
-full = ["lmfit >= 1.0.0", "latexify-py"]
+solvers = ["lmfit >= 1.0.0"]
+latexify = ["latexify-py"]
+full = ["pastas[latexify,solvers]"]
 formatting = ["isort", "black[jupyter]"]
 linting = ["flake8"]
 pytesting = ["pytest>=7", "pytest-cov", "pytest-sugar"]
 ci = [
-    "pastas[full,pytesting]",
+    "pastas[pytesting,solvers]",
     "jupyter",
-    "codacy-coverage",
+    "coverage",
     "corner",
     "emcee",
     "tqdm",
 ]
 rtd = [
+    "pastas[solvers]",
     "nbsphinx",
     "Ipython",
     "ipykernel",
     "pydata-sphinx-theme",
     "sphinx>=3.1, <6.0",
     "sphinxcontrib-bibtex",
     "requests",
     "numpydoc",
     "sphinx-design",
 ]
 dev = ["tox", "pastas[formatting,linting,ci,rtd]"]
 numbascipy = ["numba-scipy >= 0.3.1"]
 
-
 [tool.setuptools.dynamic]
 version = { attr = "pastas.version.__version__" }
 
 [tool.black]
 line-length = 88
 
 [tool.isort]
 profile = "black"
 
 [tool.pytest.ini_options]
-addopts = "--strict-markers --durations=0 --cov-report xml:coverage.xml --cov pastas"
-markers = ["notebooks: run notebooks"]
+addopts = "--strict-markers --durations=0"
+markers = ["notebooks: run notebooks", "bnotebooks: run benchmark notebooks"]
 
 [tool.tox]
 legacy_tox_ini = """
     [tox]
     requires = tox>=4
-    env_list = format, lint, notebooks, py{38,39,310}
+    env_list = format, lint, notebooks, py{38,39,310,311}
 
     [testenv]
     description = run unit tests
     extras = ci
     commands =
-            pytest tests -m "not notebooks"
+            pytest tests -m "not notebooks" -m "not bnotebooks"
+
+    [testenv:all]
+    description = run all unit tests (including Notebooks) and obtain coverage
+    extras = ci
+    commands =
+            coverage run -m pytest tests -m "not bnotebooks"
+            coverage xml
 
     [testenv:notebooks]
-    description = run unit tests
+    description = run the benchmark notebooks
     extras = ci
     commands =
-            pytest tests
+            pytest tests -m "bnotebooks"
 
     [testenv:format]
     description = run formatters
     basepython = python3.9
     extras = formatting
     commands =
             black pastas --check --diff
             isort pastas --diff --profile=black
 
     [testenv:lint]
     description = run linters
     basepython = python3.9
     extras = linting
     commands =
-            flake8 pastas --count --show-source --exit-zero --max-line-length=88
-            flake8 pastas --count --exit-zero --max-line-length=88 --statistics
+            flake8 pastas --count --show-source --exit-zero --max-line-length=88 --ignore=E203,W503,W504
+            flake8 pastas --count --exit-zero --max-line-length=88 --statistics --ignore=E203,W503,W504
 
 """
```

### Comparing `pastas-1.0.1/tests/test_comparison.py` & `pastas-1.1.0/tests/test_comparison.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import pastas as ps
 
-from .fixtures import ml, ml_sm
 
-
-def test_comparison_plot(ml, ml_sm) -> None:
+def test_comparison_plot(ml: ps.Model, ml_sm: ps.Model) -> None:
     ml.solve()
     ml_sm.solve()
     mc = ps.CompareModels(models=[ml, ml_sm])
     _ = mc.plot(legend_kwargs={"ncol": 2})
 
 
-def test_comparison_plot_custom(ml, ml_sm) -> None:
+def test_comparison_plot_custom(ml: ps.Model, ml_sm: ps.Model) -> None:
     ml.solve()
     ml_sm.solve()
     mc = ps.CompareModels(models=[ml, ml_sm])
     mosaic = [
         ["ose", "ose", "met"],
         ["sim", "sim", "tab"],
         ["res", "res", "tab"],
```

### Comparing `pastas-1.0.1/tests/test_examples.py` & `pastas-1.1.0/tests/test_examples.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Mon Jun  3 12:10:05 2019
-
-@author: Artesia
-"""
 import os
 
 import matplotlib.pyplot as plt
 import pytest
 
 pathname = os.path.join("doc", "examples")
 # get list of examples to run
```

### Comparing `pastas-1.0.1/tests/test_gxg.py` & `pastas-1.1.0/tests/test_gxg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-# -*- coding: utf-8 -*-
-"""
-
-Author: T. van Steijn, R.A. Collenteur, 2017
-
-"""
-
 import numpy as np
 import pandas as pd
 
 import pastas as ps
 
 
 class TestGXG(object):
```

### Comparing `pastas-1.0.1/tests/test_notebooks.py` & `pastas-1.1.0/tests/test_notebooks_bench.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,47 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Mon Jun  3 12:10:05 2019
-
-@author: Artesia
-"""
 import os
 import shutil
 
 import pytest
 
-pathname = os.path.join("doc", "examples")
+pathname = os.path.join("doc", "benchmarks")
 # get list of notebooks to run
 files = [f for f in os.listdir(pathname) if f.endswith(".ipynb")]
 
 testdir = "build"
 if os.path.isdir(os.path.join(pathname, testdir)):
     shutil.rmtree(os.path.join(pathname, testdir))
 os.mkdir(os.path.join(pathname, testdir))
 
 
-@pytest.mark.notebooks
+@pytest.mark.bnotebooks
 @pytest.mark.parametrize("file", files)
 def test_notebook(file) -> None:
     cwd = os.getcwd()
 
     os.chdir(pathname)
-    if file not in [
-        "00_prepare_timeseries.ipynb",
-        "12_emcee_uncertainty.ipynb",
-    ]:
-        try:
-            # run autotest on each notebook
-            cmd = (
-                "jupyter "
-                + "nbconvert "
-                + "--ExecutePreprocessor.timeout=600 "
-                + "--to "
-                + "notebook "
-                + "--execute "
-                + '"{}" '.format(file)
-                + "--output-dir "
-                + "{} ".format(testdir)
-            )
-            ival = os.system(cmd)
-            msg = "could not run {}".format(file)
-            assert ival == 0, msg
-            assert os.path.isfile(os.path.join(testdir, file)), msg
-        except Exception as e:
-            os.chdir(cwd)
-            raise Exception(e)
+    try:
+        # run autotest on each notebook
+        cmd = (
+            "jupyter "
+            + "nbconvert "
+            + "--ExecutePreprocessor.timeout=600 "
+            + "--to "
+            + "notebook "
+            + "--execute "
+            + '"{}" '.format(file)
+            + "--output-dir "
+            + "{} ".format(testdir)
+        )
+        ival = os.system(cmd)
+        msg = "could not run {}".format(file)
+        assert ival == 0, msg
+        assert os.path.isfile(os.path.join(testdir, file)), msg
+    except Exception as e:
+        os.chdir(cwd)
+        raise Exception(e)
     os.chdir(cwd)
 
 
 if __name__ == "__main__":
     for file in files:
         test_notebook(file)
```

### Comparing `pastas-1.0.1/tests/test_plots.py` & `pastas-1.1.0/tests/test_plots.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,57 @@
 import matplotlib as mpl
 
+from pastas import Model
 from pastas.plots import TrackSolve, compare
 
-from .fixtures import ml
-
 mpl.use("Agg")  # prevent _tkinter.TclError: Can't find a usable tk.tcl error
 
 
-def test_plot(ml) -> None:
+def test_plot(ml: Model) -> None:
     _ = ml.plot()
 
 
-def test_decomposition(ml) -> None:
+def test_decomposition(ml: Model) -> None:
     _ = ml.plots.decomposition(min_ylim_diff=0.1)
 
 
-def test_results(ml) -> None:
+def test_results(ml: Model) -> None:
     _ = ml.plots.results()
 
 
-def test_stacked_results(ml) -> None:
+def test_stacked_results(ml: Model) -> None:
     _ = ml.plots.stacked_results()
 
 
-def test_block_response(ml) -> None:
+def test_block_response(ml: Model) -> None:
     _ = ml.plots.block_response()
 
 
-def test_step_response(ml) -> None:
+def test_step_response(ml: Model) -> None:
     _ = ml.plots.step_response()
 
 
-def test_diagnostics(ml) -> None:
+def test_diagnostics(ml: Model) -> None:
     _ = ml.plots.diagnostics(acf_options=dict(min_obs=10))
 
 
-def test_stresses(ml) -> None:
+def test_stresses(ml: Model) -> None:
     _ = ml.plots.stresses()
 
 
-def test_contributions_pie(ml) -> None:
+def test_contributions_pie(ml: Model) -> None:
     _ = ml.plots.contributions_pie()
 
 
-def test_compare(ml) -> None:
+def test_compare(ml: Model) -> None:
     ml2 = ml.copy()
-    ml2.name = "Test_Model2"
     models = [ml, ml2]
     _ = compare(models)
 
 
-def test_tracksolve(ml) -> None:
+def test_tracksolve(ml: Model) -> None:
     track = TrackSolve(ml)
     _ = ml.solve(callback=track.plot_track_solve)
 
 
-def test_summary_pdf(ml) -> None:
+def test_summary_pdf(ml: Model) -> None:
     _ = ml.plots.summary_pdf()
```

### Comparing `pastas-1.0.1/tests/test_qgxg.py` & `pastas-1.1.0/tests/test_qgxg.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-# -*- coding: utf-8 -*-
-"""
-
-Author: T. van Steijn, R.A. Collenteur, 2017
-
-"""
-
 import numpy as np
 import pandas as pd
 
 import pastas as ps
 
 
 class TestQGXG(object):
```

### Comparing `pastas-1.0.1/tests/test_recharge.py` & `pastas-1.1.0/tests/test_recharge.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from numpy import arange, isclose, sin
 from pandas import Series, read_csv
 
 import pastas as ps
 
-from .fixtures import ml, ml_empty
-
 # Load series before
 rain = (
     read_csv("tests/data/rain.csv", index_col=0, parse_dates=True)
     .squeeze("columns")
     .loc["2005":]
     * 1e3
 )
@@ -17,63 +15,63 @@
     .squeeze("columns")
     .loc["2005":]
     * 1e3
 )
 temp = Series(index=evap.index, data=sin(arange(evap.size) / 365 * 6), dtype=float)
 
 
-def test_model_solve(ml) -> None:
+def test_model_solve(ml: ps.Model) -> None:
     ml.solve()
 
 
-def test_model_copy(ml) -> None:
+def test_model_copy(ml: ps.Model) -> None:
     ml.copy()
 
 
-def test_berendrecht(ml_empty) -> None:
+def test_berendrecht(ml_empty: ps.Model) -> None:
     rm = ps.RechargeModel(prec=rain, evap=evap, recharge=ps.rch.Berendrecht())
     ml_empty.add_stressmodel(rm)
     ml_empty.solve()
 
 
-def test_peterson(ml_empty) -> None:
+def test_peterson(ml_empty: ps.Model) -> None:
     rm = ps.RechargeModel(prec=rain, evap=evap, recharge=ps.rch.Peterson())
     ml_empty.add_stressmodel(rm)
     ml_empty.solve()
 
 
-def test_linear(ml_empty) -> None:
+def test_linear(ml_empty: ps.Model) -> None:
     rm = ps.RechargeModel(prec=rain, evap=evap, recharge=ps.rch.Linear())
     ml_empty.add_stressmodel(rm)
     ml_empty.solve()
 
 
-def test_flexmodel(ml_empty) -> None:
+def test_flexmodel(ml_empty: ps.Model) -> None:
     rm = ps.RechargeModel(prec=rain, evap=evap, recharge=ps.rch.FlexModel())
     ml_empty.add_stressmodel(rm)
     ml_empty.solve()
 
 
-def test_flexmodel_no_interception(ml_empty) -> None:
+def test_flexmodel_no_interception(ml_empty: ps.Model) -> None:
     rm = ps.RechargeModel(
         prec=rain, evap=evap, recharge=ps.rch.FlexModel(interception=False)
     )
     ml_empty.add_stressmodel(rm)
     ml_empty.solve()
 
 
-def test_flexmodel_gw_uptake(ml_empty) -> None:
+def test_flexmodel_gw_uptake(ml_empty: ps.Model) -> None:
     rm = ps.RechargeModel(
         prec=rain, evap=evap, recharge=ps.rch.FlexModel(gw_uptake=True)
     )
     ml_empty.add_stressmodel(rm)
     ml_empty.solve()
 
 
-def test_flexmodel_snow(ml_empty) -> None:
+def test_flexmodel_snow(ml_empty: ps.Model) -> None:
     rm = ps.RechargeModel(
         prec=rain, evap=evap, temp=temp, recharge=ps.rch.FlexModel(snow=True)
     )
     ml_empty.add_stressmodel(rm)
     ml_empty.solve()
```

### Comparing `pastas-1.0.1/tests/test_rfuncs.py` & `pastas-1.1.0/tests/test_rfuncs.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 @pytest.mark.parametrize("rfunc_name", ps.rfunc.__all__)
 def test_to_dict_rfuncs(rfunc_name) -> None:
     rfunc1 = getattr(ps.rfunc, rfunc_name)(cutoff=0.5)
 
     # Create the exact same instance using to_dict
     data = rfunc1.to_dict()
     rfunc_class = data.pop("class")  # Determine response class
+    rfunc_up = data.pop("up", None)
+    rfunc_gsf = data.pop("gain_scale_factor", None)
     rfunc2 = getattr(ps.rfunc, rfunc_class)(**data)
+    rfunc2.update_rfunc_settings(up=rfunc_up, gain_scale_factor=rfunc_gsf)
 
     if rfunc_name == "HantushWellModel":
         rfunc1.set_distances(100.0)
         rfunc2.set_distances(100.0)
 
     p1 = rfunc1.get_init_parameters("test").initial
     p2 = rfunc2.get_init_parameters("test").initial
```

### Comparing `pastas-1.0.1/tests/test_signatures.py` & `pastas-1.1.0/tests/test_signatures.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 import numpy as np
-import pandas as pd
+from pandas import Series, date_range
 
 import pastas as ps
 
-from .fixtures import collwell_data
-
 
 def test_summary():
     """Test all signatures for minimal functioning."""
-    idx = pd.date_range("2000", "2010")
-    head = pd.Series(index=idx, data=np.random.rand(len(idx)), dtype=float)
+    idx = date_range("2000", "2010")
+    head = Series(index=idx, data=np.random.rand(len(idx)), dtype=float)
     ps.stats.signatures.summary(head)
 
 
-def test_colwell_components(collwell_data) -> None:
+def test_colwell_components(collwell_data: Series) -> None:
     ps.stats.signatures.colwell_components(collwell_data, freq="4M", bins=3)
     return
 
 
-def test_colwell_predictability(collwell_data) -> None:
+def test_colwell_predictability(collwell_data: Series) -> None:
     """Example Tree C from the publication."""
     p = ps.stats.signatures.colwell_components(collwell_data, freq="4M", bins=3)[0]
-    assert p.round(2) == 1.0
+    assert round(p, 2) == 1.0
 
 
-def test_colwell_constancy(collwell_data) -> None:
+def test_colwell_constancy(collwell_data: Series) -> None:
     """Example Tree C from the publication."""
     c = ps.stats.signatures.colwell_components(collwell_data, freq="4M", bins=3)[1]
-    assert c.round(2) == 0.42
+    assert round(c, 2) == 0.42
 
 
-def test_colwell_contingency(collwell_data) -> None:
+def test_colwell_contingency(collwell_data: Series) -> None:
     """Example Tree C from the publication."""
     m = ps.stats.signatures.colwell_components(collwell_data, freq="4M", bins=3)[2]
-    assert m.round(2) == 0.58
+    assert round(m, 2) == 0.58
```

### Comparing `pastas-1.0.1/tests/test_stats.py` & `pastas-1.1.0/tests/test_stats.py`

 * *Files identical despite different names*


# Comparing `tmp/siman-1.2.7.tar.gz` & `tmp/siman-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/siman-1.2.7.tar", last modified: Tue Apr  4 10:20:56 2023, max compression
+gzip compressed data, was "dist/siman-1.2.8.tar", last modified: Fri May 12 13:35:10 2023, max compression
```

## Comparing `siman-1.2.7.tar` & `siman-1.2.8.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-04-04 10:20:56.669774 siman-1.2.7/
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.2.7/LICENSE
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.2.7/MANIFEST.in
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-04-04 10:20:56.668774 siman-1.2.7/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.2.7/README.md
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2023-04-04 10:20:56.669774 siman-1.2.7/setup.cfg
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2023-04-04 10:20:54.000000 siman-1.2.7/setup.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-04-04 10:20:56.666774 siman-1.2.7/siman/
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2022-03-05 17:22:57.000000 siman-1.2.7/siman/3d_plot.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3140 2022-03-05 17:22:57.000000 siman-1.2.7/siman/SSHTools.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)       32 2021-02-17 13:28:25.000000 siman-1.2.7/siman/__init__.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    49532 2022-09-29 10:57:16.000000 siman-1.2.7/siman/analysis.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2022-03-05 17:22:57.000000 siman-1.2.7/siman/analysis_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-04-04 10:20:56.667774 siman-1.2.7/siman/analyze/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.2.7/siman/analyze/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.2.7/siman/analyze/segregation.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2022-03-05 17:22:57.000000 siman-1.2.7/siman/approximation.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2022-03-05 17:22:57.000000 siman-1.2.7/siman/bands.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   125725 2022-12-15 17:40:20.000000 siman-1.2.7/siman/calc_manage.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2022-03-05 17:22:57.000000 siman-1.2.7/siman/calcul.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-04-04 10:20:56.667774 siman-1.2.7/siman/calculators/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.2.7/siman/calculators/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.2.7/siman/calculators/aims.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8718 2022-09-20 15:22:50.000000 siman-1.2.7/siman/calculators/gaussian.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.2.7/siman/calculators/qe.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    56487 2023-04-01 18:47:04.000000 siman-1.2.7/siman/calculators/vasp.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.2.7/siman/calculators/vasp_old.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-04-04 10:20:56.667774 siman-1.2.7/siman/chg/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.2.7/siman/chg/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2021-02-17 13:28:25.000000 siman-1.2.7/siman/chg/chg_func.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.2.7/siman/chg/vasputil_chgarith_module.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    11072 2022-09-20 15:22:50.000000 siman-1.2.7/siman/classes.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-04-04 10:20:56.668774 siman-1.2.7/siman/core/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.2.7/siman/core/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53303 2023-04-04 10:20:35.000000 siman-1.2.7/siman/core/calculation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.2.7/siman/core/calculation_old.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33337 2023-02-13 17:12:02.000000 siman-1.2.7/siman/core/cluster_batch_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3698 2022-09-20 15:22:50.000000 siman-1.2.7/siman/core/cluster_run_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2127 2022-09-20 15:22:50.000000 siman-1.2.7/siman/core/molecule.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   118074 2023-04-01 17:58:09.000000 siman-1.2.7/siman/core/structure.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    20209 2022-12-15 17:24:44.000000 siman-1.2.7/siman/database.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2022-03-05 17:22:57.000000 siman-1.2.7/siman/default_project_conf.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2022-03-05 17:22:57.000000 siman-1.2.7/siman/dev_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    32406 2022-12-09 18:12:22.000000 siman-1.2.7/siman/dos_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2022-03-05 17:22:57.000000 siman-1.2.7/siman/fit_hex.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    28019 2022-09-20 15:22:50.000000 siman-1.2.7/siman/functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   113841 2023-03-06 17:27:57.000000 siman-1.2.7/siman/geo.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    14496 2023-01-30 17:40:21.000000 siman-1.2.7/siman/header.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      286 2022-03-05 17:22:57.000000 siman-1.2.7/siman/helper_for_writing_beatiful_code.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    40223 2022-09-20 15:22:50.000000 siman-1.2.7/siman/impurity.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    80434 2022-09-29 10:57:16.000000 siman-1.2.7/siman/inout.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2022-03-05 17:22:57.000000 siman-1.2.7/siman/kpoints_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-04-04 10:20:56.668774 siman-1.2.7/siman/mat_prop/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.2.7/siman/mat_prop/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.2.7/siman/mat_prop/mat_prop.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    45055 2022-09-29 10:57:16.000000 siman-1.2.7/siman/matproj_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2022-09-20 15:22:50.000000 siman-1.2.7/siman/monte.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      980 2022-03-05 17:22:57.000000 siman-1.2.7/siman/monte_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31643 2022-09-20 15:22:50.000000 siman-1.2.7/siman/neb.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2021-02-17 13:28:25.000000 siman-1.2.7/siman/pairs.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    49712 2023-01-25 18:10:57.000000 siman-1.2.7/siman/picture_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2022-03-05 17:22:57.000000 siman-1.2.7/siman/plot_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     4440 2023-02-08 10:08:27.000000 siman-1.2.7/siman/polaron.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2022-03-05 17:22:57.000000 siman-1.2.7/siman/polaron_hop.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2022-09-29 10:57:16.000000 siman-1.2.7/siman/polaron_mod.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   194580 2022-09-29 10:57:16.000000 siman-1.2.7/siman/project_funcs.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2022-03-05 17:22:57.000000 siman-1.2.7/siman/properties_2d.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2022-03-05 17:22:57.000000 siman-1.2.7/siman/properties_energy.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2022-03-05 17:22:57.000000 siman-1.2.7/siman/properties_lattice.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    30636 2023-04-04 10:03:08.000000 siman-1.2.7/siman/set_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2022-03-05 17:22:57.000000 siman-1.2.7/siman/simanrc.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      174 2022-03-05 17:22:57.000000 siman-1.2.7/siman/small_classes.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     6565 2022-09-29 10:57:16.000000 siman-1.2.7/siman/small_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2022-03-05 17:22:57.000000 siman-1.2.7/siman/structure_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2022-03-05 17:22:57.000000 siman-1.2.7/siman/table_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2022-03-05 17:22:57.000000 siman-1.2.7/siman/thermo.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2022-03-05 17:22:57.000000 siman-1.2.7/siman/workflow_utilities.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-04-04 10:20:56.667774 siman-1.2.7/siman.egg-info/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-04-04 10:20:56.000000 siman-1.2.7/siman.egg-info/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1677 2023-04-04 10:20:56.000000 siman-1.2.7/siman.egg-info/SOURCES.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2023-04-04 10:20:56.000000 siman-1.2.7/siman.egg-info/dependency_links.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2023-04-04 10:20:56.000000 siman-1.2.7/siman.egg-info/requires.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2023-04-04 10:20:56.000000 siman-1.2.7/siman.egg-info/top_level.txt
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-05-12 13:35:10.774413 siman-1.2.8/
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.2.8/LICENSE
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.2.8/MANIFEST.in
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-05-12 13:35:10.774413 siman-1.2.8/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.2.8/README.md
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2023-05-12 13:35:10.774413 siman-1.2.8/setup.cfg
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2023-05-12 13:35:04.000000 siman-1.2.8/setup.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-05-12 13:35:10.771413 siman-1.2.8/siman/
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2022-03-05 17:22:57.000000 siman-1.2.8/siman/3d_plot.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3140 2022-03-05 17:22:57.000000 siman-1.2.8/siman/SSHTools.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)       32 2021-02-17 13:28:25.000000 siman-1.2.8/siman/__init__.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    49532 2022-09-29 10:57:16.000000 siman-1.2.8/siman/analysis.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2022-03-05 17:22:57.000000 siman-1.2.8/siman/analysis_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-05-12 13:35:10.772413 siman-1.2.8/siman/analyze/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.2.8/siman/analyze/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.2.8/siman/analyze/segregation.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2022-03-05 17:22:57.000000 siman-1.2.8/siman/approximation.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2022-03-05 17:22:57.000000 siman-1.2.8/siman/bands.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   125759 2023-05-12 13:34:11.000000 siman-1.2.8/siman/calc_manage.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2022-03-05 17:22:57.000000 siman-1.2.8/siman/calcul.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-05-12 13:35:10.772413 siman-1.2.8/siman/calculators/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.2.8/siman/calculators/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.2.8/siman/calculators/aims.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8718 2022-09-20 15:22:50.000000 siman-1.2.8/siman/calculators/gaussian.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.2.8/siman/calculators/qe.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    56510 2023-04-04 10:46:17.000000 siman-1.2.8/siman/calculators/vasp.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.2.8/siman/calculators/vasp_old.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-05-12 13:35:10.772413 siman-1.2.8/siman/chg/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.2.8/siman/chg/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2021-02-17 13:28:25.000000 siman-1.2.8/siman/chg/chg_func.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.2.8/siman/chg/vasputil_chgarith_module.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    11072 2022-09-20 15:22:50.000000 siman-1.2.8/siman/classes.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-05-12 13:35:10.773413 siman-1.2.8/siman/core/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.2.8/siman/core/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53303 2023-04-04 10:20:35.000000 siman-1.2.8/siman/core/calculation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.2.8/siman/core/calculation_old.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33337 2023-02-13 17:12:02.000000 siman-1.2.8/siman/core/cluster_batch_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3698 2022-09-20 15:22:50.000000 siman-1.2.8/siman/core/cluster_run_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2127 2022-09-20 15:22:50.000000 siman-1.2.8/siman/core/molecule.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   118077 2023-04-18 16:31:52.000000 siman-1.2.8/siman/core/structure.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    20209 2022-12-15 17:24:44.000000 siman-1.2.8/siman/database.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2022-03-05 17:22:57.000000 siman-1.2.8/siman/default_project_conf.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2022-03-05 17:22:57.000000 siman-1.2.8/siman/dev_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    32406 2022-12-09 18:12:22.000000 siman-1.2.8/siman/dos_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2022-03-05 17:22:57.000000 siman-1.2.8/siman/fit_hex.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    28019 2022-09-20 15:22:50.000000 siman-1.2.8/siman/functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   113841 2023-03-06 17:27:57.000000 siman-1.2.8/siman/geo.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    14496 2023-01-30 17:40:21.000000 siman-1.2.8/siman/header.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      286 2022-03-05 17:22:57.000000 siman-1.2.8/siman/helper_for_writing_beatiful_code.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    40223 2022-09-20 15:22:50.000000 siman-1.2.8/siman/impurity.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    80434 2022-09-29 10:57:16.000000 siman-1.2.8/siman/inout.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2022-03-05 17:22:57.000000 siman-1.2.8/siman/kpoints_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-05-12 13:35:10.774413 siman-1.2.8/siman/mat_prop/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.2.8/siman/mat_prop/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.2.8/siman/mat_prop/mat_prop.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    45055 2022-09-29 10:57:16.000000 siman-1.2.8/siman/matproj_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2022-09-20 15:22:50.000000 siman-1.2.8/siman/monte.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      980 2022-03-05 17:22:57.000000 siman-1.2.8/siman/monte_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31643 2022-09-20 15:22:50.000000 siman-1.2.8/siman/neb.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2021-02-17 13:28:25.000000 siman-1.2.8/siman/pairs.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    49712 2023-01-25 18:10:57.000000 siman-1.2.8/siman/picture_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2022-03-05 17:22:57.000000 siman-1.2.8/siman/plot_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     4434 2023-04-06 13:23:01.000000 siman-1.2.8/siman/polaron.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2022-03-05 17:22:57.000000 siman-1.2.8/siman/polaron_hop.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2022-09-29 10:57:16.000000 siman-1.2.8/siman/polaron_mod.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   194580 2022-09-29 10:57:16.000000 siman-1.2.8/siman/project_funcs.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2022-03-05 17:22:57.000000 siman-1.2.8/siman/properties_2d.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2022-03-05 17:22:57.000000 siman-1.2.8/siman/properties_energy.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2022-03-05 17:22:57.000000 siman-1.2.8/siman/properties_lattice.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    30666 2023-04-04 10:53:58.000000 siman-1.2.8/siman/set_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2022-03-05 17:22:57.000000 siman-1.2.8/siman/simanrc.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      174 2022-03-05 17:22:57.000000 siman-1.2.8/siman/small_classes.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     6565 2022-09-29 10:57:16.000000 siman-1.2.8/siman/small_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2022-03-05 17:22:57.000000 siman-1.2.8/siman/structure_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2022-03-05 17:22:57.000000 siman-1.2.8/siman/table_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2022-03-05 17:22:57.000000 siman-1.2.8/siman/thermo.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2022-03-05 17:22:57.000000 siman-1.2.8/siman/workflow_utilities.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-05-12 13:35:10.772413 siman-1.2.8/siman.egg-info/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-05-12 13:35:10.000000 siman-1.2.8/siman.egg-info/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1677 2023-05-12 13:35:10.000000 siman-1.2.8/siman.egg-info/SOURCES.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2023-05-12 13:35:10.000000 siman-1.2.8/siman.egg-info/dependency_links.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2023-05-12 13:35:10.000000 siman-1.2.8/siman.egg-info/requires.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2023-05-12 13:35:10.000000 siman-1.2.8/siman.egg-info/top_level.txt
```

### Comparing `siman-1.2.7/LICENSE` & `siman-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/PKG-INFO` & `siman-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.2.7
+Version: 1.2.8
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.2.7/setup.py` & `siman-1.2.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="siman",
-    version="1.2.7",
+    version="1.2.8",
     author="Dmitry Aksenov",
     author_email="dimonaks@gmail.com",
     description="Manager for DFT calculations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dimonaks/siman",
     license = 'GPL',
```

### Comparing `siman-1.2.7/siman/3d_plot.py` & `siman-1.2.8/siman/3d_plot.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/SSHTools.py` & `siman-1.2.8/siman/SSHTools.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/analysis.py` & `siman-1.2.8/siman/analysis.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/analysis_functions.py` & `siman-1.2.8/siman/analysis_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/analyze/segregation.py` & `siman-1.2.8/siman/analyze/segregation.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/approximation.py` & `siman-1.2.8/siman/approximation.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/bands.py` & `siman-1.2.8/siman/bands.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/calc_manage.py` & `siman-1.2.8/siman/calc_manage.py`

 * *Files 0% similar despite different names*

```diff
@@ -874,15 +874,15 @@
 
 
         if ('polaron' in calc_method) or ('polaron2' in calc_method):
             pm = params['polaron']
             am = abs(pm['amp']) # amplitude of polaron, the sign is not important here
 
             existing = pm.get('polaron_status') and 'ex' in pm.get('polaron_status') 
-
+            nn = pm.get('nn') or 6
             # if pm.get('st1') and pm.get('st2'):
 
             if pm['polaron_type'] == 'electron':
                 if existing:
                     ''
                     #nothing is done
                 else:
```

### Comparing `siman-1.2.7/siman/calcul.py` & `siman-1.2.8/siman/calcul.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/calculators/aims.py` & `siman-1.2.8/siman/calculators/aims.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/calculators/gaussian.py` & `siman-1.2.8/siman/calculators/gaussian.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/calculators/qe.py` & `siman-1.2.8/siman/calculators/qe.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/calculators/vasp.py` & `siman-1.2.8/siman/calculators/vasp.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,20 +207,26 @@
                     self.init.zval.append(float(line.split()[5]))
             
             try: 
                 curset.add_nbands
             except AttributeError: 
                 curset.add_nbands = None
 
-            if curset.add_nbands != None:
-                tve =0
-                for i in range(st.ntypat):
-                    # print self.init.zval
-                    tve += self.init.zval[i] * st.nznucl[i] #number of electrons 
+
+            tve =0 # total number of valence electrons
+            for i in range(st.ntypat):
+                # print self.init.zval
+                tve += self.init.zval[i] * st.nznucl[i] #number of electrons 
                     # print(self.init.zval[i], self.init.nznucl[i])
+            if params and 'charge' in params and params['charge']:
+                vp['NELECT'] = int(tve - params['charge'])
+
+
+            if curset.add_nbands != None:
+
                 nbands_min = math.ceil(tve / 2.)
                 self.nbands = int ( round ( nbands_min * curset.add_nbands ) )
                 # print(self.nbands)
                 
 
                 vp['NBANDS'] = self.nbands
                 printlog('I found that at least', nbands_min, ' bands are required. I will use', self.nbands, 'bands; add_nbands = ', curset.add_nbands)
@@ -233,16 +239,15 @@
                 # print (vp)
                 printlog('SOC calculation detected; increasing number of bands by two', imp = 'Y')
                 vp['NBANDS']*=2
 
 
 
 
-            if params and 'charge' in params and params['charge']:
-                vp['NELECT'] = int(tve - params['charge'])
+
 
 
         else:
             printlog('Attention! No path_to_potcar! skipping NBANDS calculation')
 
         return
 
@@ -542,15 +547,15 @@
                 # sys.exit()
                 anions_set = []
                 for el in uelntypat.keys(): #
                     if uelntypat[el] > 1: # this condition shows that multitype regime was asked for
                         printlog('LDAUL are given for the following multitype elements: ',uels, imp = 'y')
                         for el_set in uels:
                             if el in el_set and '/' not in el_set: # check that correct format is used
-                                printlog('Warning! Element', el, f'has several types. LDAUL values should be given in format {el}/A but mixture of {el}/A and {el} was detected. Please check that U are assigned as you intend')
+                                printlog('Error! Element', el, f'has several types. LDAUL values should be given in format {el}/A but mixture of {el}/A and {el} was detected. Please check that U are assigned as you intend')
                             #check that required anions are present 
                             A = el_set.split('/')[1]
                             anions_set.append(A)
                             # print(A)
                             if A not in el_list:
                                 printlog(f'Warning! Anion {A} is absent in your structure but present in your set')
```

### Comparing `siman-1.2.7/siman/calculators/vasp_old.py` & `siman-1.2.8/siman/calculators/vasp_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/chg/chg_func.py` & `siman-1.2.8/siman/chg/chg_func.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/chg/vasputil_chgarith_module.py` & `siman-1.2.8/siman/chg/vasputil_chgarith_module.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/classes.py` & `siman-1.2.8/siman/classes.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/core/calculation.py` & `siman-1.2.8/siman/core/calculation.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/core/calculation_old.py` & `siman-1.2.8/siman/core/calculation_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/core/cluster_batch_script.py` & `siman-1.2.8/siman/core/cluster_batch_script.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/core/cluster_run_script.py` & `siman-1.2.8/siman/core/cluster_run_script.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/core/molecule.py` & `siman-1.2.8/siman/core/molecule.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/core/structure.py` & `siman-1.2.8/siman/core/structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -656,15 +656,15 @@
     def get_name(self):
         from siman.small_functions import latex_chem
         return latex_chem(self.get_reduced_formula())
 
     def get_formula(self):
         ''
         # pm = self.convert2pymatgen()
-        # cm = Composition(pm.formula)
+        # cm = Composition(pm.formula)cd 
         # cm = Composition(self.get_elements())
         return self.convert2pymatgen().formula
 
     def get_reduced_composition(self):
         ''
         pm = self.convert2pymatgen()
         cm = Composition(pm.formula)
```

### Comparing `siman-1.2.7/siman/database.py` & `siman-1.2.8/siman/database.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/default_project_conf.py` & `siman-1.2.8/siman/default_project_conf.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/dev_functions.py` & `siman-1.2.8/siman/dev_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/dos_functions.py` & `siman-1.2.8/siman/dos_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/fit_hex.py` & `siman-1.2.8/siman/fit_hex.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/functions.py` & `siman-1.2.8/siman/functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/geo.py` & `siman-1.2.8/siman/geo.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/header.py` & `siman-1.2.8/siman/header.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/impurity.py` & `siman-1.2.8/siman/impurity.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/inout.py` & `siman-1.2.8/siman/inout.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/kpoints_functions.py` & `siman-1.2.8/siman/kpoints_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/mat_prop/mat_prop.py` & `siman-1.2.8/siman/mat_prop/mat_prop.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/matproj_functions.py` & `siman-1.2.8/siman/matproj_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/monte.py` & `siman-1.2.8/siman/monte.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/monte_functions.py` & `siman-1.2.8/siman/monte_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/neb.py` & `siman-1.2.8/siman/neb.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/pairs.py` & `siman-1.2.8/siman/pairs.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/picture_functions.py` & `siman-1.2.8/siman/picture_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/plot_functions.py` & `siman-1.2.8/siman/plot_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/polaron.py` & `siman-1.2.8/siman/polaron.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from siman import header
 from siman.monte_functions import metropolis
 from siman.header import runBash, printlog
 from siman.header import ALKALI_ION_ELEMENTS as AM
 from siman.header import TRANSITION_ELEMENTS as TM
 from siman.classes import CalculationVasp, Structure
 from siman.inout import read_poscar
-from siman.functions import invert, update_incar
+from siman.functions import invert
 from siman.analysis import suf_en
 from siman.monte import vasp_run
 from siman.geo import interpolate
 debug2 = 0
 
 
 def copy_vasp_files(v):
@@ -105,27 +105,27 @@
             cl2.read_results(show = 'fo')
 
         """2. Create intermediate steps"""
         interpolate(cl1.end, cl2.end, images, 3)
         printlog('Interpolation was successful!\n', imp = 'y')
 
         """3. Calculate energies of intermediate steps"""
-        update_incar(parameter = 'NSW', value = 0, run = 1, write = 0)
+        cl1.update_incar(parameter = 'NSW', value = 0, run = 1, write = 0)
         
         for v in range(3, 3+images):
 
             vasp_step(v, 'Intermediate position '+str(v), 1 )
 
     elif mode =='inherit':
 
         #from initial to last
         cl2 = vasp_step(2, 'End position', 1 )
         cl1 = vasp_step(1, 'Start position', 0)
         # copyfile(str(v)+'.POSCAR', 'POSCAR')
-        update_incar(parameter = 'NSW', value = 0, run = 1, write = 0)
+        cl1.update_incar(parameter = 'NSW', value = 0, run = 1, write = 0)
         
         interpolate(cl1.end, cl2.end, images, 21, omit_edges = 0)
         for v in range(21, 21+images):
             vasp_step(v, 'Intermediate position '+str(v), rm = 0 )
 
         runBash('rm CHGCAR WAVECAR; gunzip 2.CHGCAR.gz; mv 2.CHGCAR CHGCAR')
```

### Comparing `siman-1.2.7/siman/polaron_hop.py` & `siman-1.2.8/siman/polaron_hop.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/polaron_mod.py` & `siman-1.2.8/siman/polaron_mod.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/project_funcs.py` & `siman-1.2.8/siman/project_funcs.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/properties_2d.py` & `siman-1.2.8/siman/properties_2d.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/properties_energy.py` & `siman-1.2.8/siman/properties_energy.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/properties_lattice.py` & `siman-1.2.8/siman/properties_lattice.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/set_functions.py` & `siman-1.2.8/siman/set_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -519,14 +519,15 @@
                             value = float(value)
                         else:
                             value = int(value)
                     except:
                         pass
 
                     self.vasp_params[token.strip()] = value
+        self.add_nbands = 1.0
         # self.update()
 
 
     def add_conv_kpoint(self,arg):
         if type(arg) is not str:
             sys.exit("\nadd_conv_kpoint error\n")
         if arg in self.conv_kpoint:
```

### Comparing `siman-1.2.7/siman/simanrc.py` & `siman-1.2.8/siman/simanrc.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/small_functions.py` & `siman-1.2.8/siman/small_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/structure_functions.py` & `siman-1.2.8/siman/structure_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/table_functions.py` & `siman-1.2.8/siman/table_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/thermo.py` & `siman-1.2.8/siman/thermo.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman/workflow_utilities.py` & `siman-1.2.8/siman/workflow_utilities.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.7/siman.egg-info/PKG-INFO` & `siman-1.2.8/siman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.2.7
+Version: 1.2.8
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.2.7/siman.egg-info/SOURCES.txt` & `siman-1.2.8/siman.egg-info/SOURCES.txt`

 * *Files identical despite different names*


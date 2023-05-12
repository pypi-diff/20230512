# Comparing `tmp/covsirphy-2.9.0.tar.gz` & `tmp/covsirphy-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/covsirphy-2.9.0.tar", last modified: Tue Oct 20 14:24:50 2020, max compression
+gzip compressed data, was "dist/covsirphy-2.9.1.tar", last modified: Sat Oct 24 13:20:11 2020, max compression
```

## Comparing `covsirphy-2.9.0.tar` & `covsirphy-2.9.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-10-20 14:24:50.494069 covsirphy-2.9.0/
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)    11357 2020-05-11 10:27:33.000000 covsirphy-2.9.0/LICENSE
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)       34 2020-07-04 06:44:41.000000 covsirphy-2.9.0/MANIFEST.in
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     8706 2020-10-20 14:24:50.495065 covsirphy-2.9.0/PKG-INFO
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     5883 2020-09-24 14:54:01.000000 covsirphy-2.9.0/README.md
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     6840 2020-10-20 14:24:19.000000 covsirphy-2.9.0/README.rst
-drwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-10-20 14:24:50.208336 covsirphy-2.9.0/covsirphy/
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     2486 2020-08-22 15:41:49.000000 covsirphy-2.9.0/covsirphy/__init__.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)       69 2020-10-20 14:23:50.000000 covsirphy-2.9.0/covsirphy/__version__.py
-drwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-10-20 14:24:50.237394 covsirphy-2.9.0/covsirphy/analysis/
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-08-22 15:41:49.000000 covsirphy-2.9.0/covsirphy/analysis/__init__.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     7909 2020-08-20 14:45:52.000000 covsirphy-2.9.0/covsirphy/analysis/example_data.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)    39320 2020-10-20 13:13:36.000000 covsirphy-2.9.0/covsirphy/analysis/scenario.py
-drwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-10-20 14:24:50.282623 covsirphy-2.9.0/covsirphy/cleaning/
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-08-22 15:41:49.000000 covsirphy-2.9.0/covsirphy/cleaning/__init__.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)    11098 2020-08-22 06:36:51.000000 covsirphy-2.9.0/covsirphy/cleaning/cbase.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     6196 2020-08-16 08:42:09.000000 covsirphy-2.9.0/covsirphy/cleaning/country_data.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)    21451 2020-08-31 13:56:34.000000 covsirphy-2.9.0/covsirphy/cleaning/dataloader.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)    10712 2020-09-07 15:43:21.000000 covsirphy-2.9.0/covsirphy/cleaning/jhu_data.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     3908 2020-08-15 12:51:36.000000 covsirphy-2.9.0/covsirphy/cleaning/oxcgrt.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     8198 2020-08-16 08:42:09.000000 covsirphy-2.9.0/covsirphy/cleaning/population.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)    12407 2020-10-18 14:45:01.000000 covsirphy-2.9.0/covsirphy/cleaning/term.py
-drwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-10-20 14:24:50.350573 covsirphy-2.9.0/covsirphy/ode/
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-08-22 15:41:49.000000 covsirphy-2.9.0/covsirphy/ode/__init__.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     7154 2020-08-20 13:19:51.000000 covsirphy-2.9.0/covsirphy/ode/mbase.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     7779 2020-08-20 13:19:48.000000 covsirphy-2.9.0/covsirphy/ode/sewirf.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     6370 2020-08-20 13:19:55.000000 covsirphy-2.9.0/covsirphy/ode/sir.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     6645 2020-08-20 13:19:58.000000 covsirphy-2.9.0/covsirphy/ode/sird.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     6790 2020-08-22 06:47:19.000000 covsirphy-2.9.0/covsirphy/ode/sirf.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     7722 2020-08-20 13:19:44.000000 covsirphy-2.9.0/covsirphy/ode/sirfv.py
-drwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-10-20 14:24:50.378162 covsirphy-2.9.0/covsirphy/phase/
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-08-22 15:41:49.000000 covsirphy-2.9.0/covsirphy/phase/__init__.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     5668 2020-10-20 12:35:19.000000 covsirphy-2.9.0/covsirphy/phase/phase_estimator.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)    15590 2020-10-20 09:25:50.000000 covsirphy-2.9.0/covsirphy/phase/phase_series.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)    18172 2020-10-20 13:13:36.000000 covsirphy-2.9.0/covsirphy/phase/phase_unit.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     8089 2020-09-08 10:53:08.000000 covsirphy-2.9.0/covsirphy/phase/sr_change.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     7697 2020-08-22 06:41:05.000000 covsirphy-2.9.0/covsirphy/phase/trend.py
-drwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-10-20 14:24:50.399107 covsirphy-2.9.0/covsirphy/simulation/
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-08-22 15:41:49.000000 covsirphy-2.9.0/covsirphy/simulation/__init__.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)    13539 2020-08-20 14:45:52.000000 covsirphy-2.9.0/covsirphy/simulation/estimator.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)    11934 2020-08-23 13:24:28.000000 covsirphy-2.9.0/covsirphy/simulation/optimize.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     8703 2020-08-18 15:11:16.000000 covsirphy-2.9.0/covsirphy/simulation/simulator.py
-drwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-10-20 14:24:50.413068 covsirphy-2.9.0/covsirphy/util/
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-08-22 15:41:49.000000 covsirphy-2.9.0/covsirphy/util/__init__.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)      718 2020-08-13 09:52:56.000000 covsirphy-2.9.0/covsirphy/util/argument.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)      850 2020-08-23 10:51:38.000000 covsirphy-2.9.0/covsirphy/util/error.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     2845 2020-06-30 14:08:36.000000 covsirphy-2.9.0/covsirphy/util/map.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     4756 2020-07-04 06:44:42.000000 covsirphy-2.9.0/covsirphy/util/plotting.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)      746 2020-08-13 17:25:10.000000 covsirphy-2.9.0/covsirphy/util/stopwatch.py
-drwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-10-20 14:24:50.434025 covsirphy-2.9.0/covsirphy/worldwide/
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-08-22 15:41:49.000000 covsirphy-2.9.0/covsirphy/worldwide/__init__.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)    11279 2020-10-20 14:18:19.000000 covsirphy-2.9.0/covsirphy/worldwide/policy.py
-drwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-10-20 14:24:50.217432 covsirphy-2.9.0/covsirphy.egg-info/
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     8706 2020-10-20 14:24:49.000000 covsirphy-2.9.0/covsirphy.egg-info/PKG-INFO
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     1518 2020-10-20 14:24:50.000000 covsirphy-2.9.0/covsirphy.egg-info/SOURCES.txt
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        1 2020-10-20 14:24:49.000000 covsirphy-2.9.0/covsirphy.egg-info/dependency_links.txt
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)      137 2020-10-20 14:24:49.000000 covsirphy-2.9.0/covsirphy.egg-info/requires.txt
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)       16 2020-10-20 14:24:49.000000 covsirphy-2.9.0/covsirphy.egg-info/top_level.txt
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)      803 2020-10-20 14:24:50.499049 covsirphy-2.9.0/setup.cfg
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)       38 2020-06-21 12:38:07.000000 covsirphy-2.9.0/setup.py
-drwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-10-20 14:24:50.490073 covsirphy-2.9.0/tests/
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-06-30 14:08:36.000000 covsirphy-2.9.0/tests/__init__.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)      660 2020-08-10 06:19:10.000000 covsirphy-2.9.0/tests/conftest.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     2586 2020-08-27 15:52:34.000000 covsirphy-2.9.0/tests/test_change_finder.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     9288 2020-08-23 10:51:38.000000 covsirphy-2.9.0/tests/test_data_loader.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     4119 2020-08-16 08:42:09.000000 covsirphy-2.9.0/tests/test_ode.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     8380 2020-09-19 07:21:53.000000 covsirphy-2.9.0/tests/test_phase_series.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     6861 2020-08-23 10:51:38.000000 covsirphy-2.9.0/tests/test_phase_unit.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     2195 2020-10-20 14:16:17.000000 covsirphy-2.9.0/tests/test_policy_measures.py
--rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)    10848 2020-10-20 13:13:36.000000 covsirphy-2.9.0/tests/test_scenario.py
+drwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-10-24 13:20:11.600363 covsirphy-2.9.1/
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)    11357 2020-05-11 10:27:33.000000 covsirphy-2.9.1/LICENSE
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)       34 2020-07-04 06:44:41.000000 covsirphy-2.9.1/MANIFEST.in
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     9739 2020-10-24 13:20:11.600363 covsirphy-2.9.1/PKG-INFO
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     6614 2020-10-24 13:17:57.000000 covsirphy-2.9.1/README.md
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     7657 2020-10-24 13:19:43.000000 covsirphy-2.9.1/README.rst
+drwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-10-24 13:20:11.408073 covsirphy-2.9.1/covsirphy/
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     2486 2020-08-22 15:41:49.000000 covsirphy-2.9.1/covsirphy/__init__.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)       69 2020-10-24 13:19:05.000000 covsirphy-2.9.1/covsirphy/__version__.py
+drwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-10-24 13:20:11.435484 covsirphy-2.9.1/covsirphy/analysis/
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-08-22 15:41:49.000000 covsirphy-2.9.1/covsirphy/analysis/__init__.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     7909 2020-08-20 14:45:52.000000 covsirphy-2.9.1/covsirphy/analysis/example_data.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)    39320 2020-10-20 13:13:36.000000 covsirphy-2.9.1/covsirphy/analysis/scenario.py
+drwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-10-24 13:20:11.471126 covsirphy-2.9.1/covsirphy/cleaning/
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-08-22 15:41:49.000000 covsirphy-2.9.1/covsirphy/cleaning/__init__.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)    11098 2020-08-22 06:36:51.000000 covsirphy-2.9.1/covsirphy/cleaning/cbase.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     6196 2020-08-16 08:42:09.000000 covsirphy-2.9.1/covsirphy/cleaning/country_data.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)    21530 2020-10-24 12:21:47.000000 covsirphy-2.9.1/covsirphy/cleaning/dataloader.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)    10712 2020-09-07 15:43:21.000000 covsirphy-2.9.1/covsirphy/cleaning/jhu_data.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     3908 2020-08-15 12:51:36.000000 covsirphy-2.9.1/covsirphy/cleaning/oxcgrt.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     8198 2020-08-16 08:42:09.000000 covsirphy-2.9.1/covsirphy/cleaning/population.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)    12407 2020-10-18 14:45:01.000000 covsirphy-2.9.1/covsirphy/cleaning/term.py
+drwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-10-24 13:20:11.496405 covsirphy-2.9.1/covsirphy/ode/
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-08-22 15:41:49.000000 covsirphy-2.9.1/covsirphy/ode/__init__.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     7154 2020-08-20 13:19:51.000000 covsirphy-2.9.1/covsirphy/ode/mbase.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     7779 2020-08-20 13:19:48.000000 covsirphy-2.9.1/covsirphy/ode/sewirf.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     6370 2020-08-20 13:19:55.000000 covsirphy-2.9.1/covsirphy/ode/sir.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     6645 2020-08-20 13:19:58.000000 covsirphy-2.9.1/covsirphy/ode/sird.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     6790 2020-08-22 06:47:19.000000 covsirphy-2.9.1/covsirphy/ode/sirf.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     7722 2020-08-20 13:19:44.000000 covsirphy-2.9.1/covsirphy/ode/sirfv.py
+drwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-10-24 13:20:11.523386 covsirphy-2.9.1/covsirphy/phase/
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-08-22 15:41:49.000000 covsirphy-2.9.1/covsirphy/phase/__init__.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     5668 2020-10-20 12:35:19.000000 covsirphy-2.9.1/covsirphy/phase/phase_estimator.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)    15590 2020-10-20 09:25:50.000000 covsirphy-2.9.1/covsirphy/phase/phase_series.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)    18172 2020-10-20 13:13:36.000000 covsirphy-2.9.1/covsirphy/phase/phase_unit.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     8089 2020-09-08 10:53:08.000000 covsirphy-2.9.1/covsirphy/phase/sr_change.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     7697 2020-08-22 06:41:05.000000 covsirphy-2.9.1/covsirphy/phase/trend.py
+drwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-10-24 13:20:11.540528 covsirphy-2.9.1/covsirphy/simulation/
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-08-22 15:41:49.000000 covsirphy-2.9.1/covsirphy/simulation/__init__.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)    13539 2020-08-20 14:45:52.000000 covsirphy-2.9.1/covsirphy/simulation/estimator.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)    11934 2020-08-23 13:24:28.000000 covsirphy-2.9.1/covsirphy/simulation/optimize.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     8703 2020-08-18 15:11:16.000000 covsirphy-2.9.1/covsirphy/simulation/simulator.py
+drwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-10-24 13:20:11.561482 covsirphy-2.9.1/covsirphy/util/
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-08-22 15:41:49.000000 covsirphy-2.9.1/covsirphy/util/__init__.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)      718 2020-08-13 09:52:56.000000 covsirphy-2.9.1/covsirphy/util/argument.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)      850 2020-08-23 10:51:38.000000 covsirphy-2.9.1/covsirphy/util/error.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     2845 2020-06-30 14:08:36.000000 covsirphy-2.9.1/covsirphy/util/map.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     4756 2020-07-04 06:44:42.000000 covsirphy-2.9.1/covsirphy/util/plotting.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)      746 2020-08-13 17:25:10.000000 covsirphy-2.9.1/covsirphy/util/stopwatch.py
+drwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-10-24 13:20:11.570446 covsirphy-2.9.1/covsirphy/worldwide/
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-08-22 15:41:49.000000 covsirphy-2.9.1/covsirphy/worldwide/__init__.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)    11356 2020-10-23 15:05:26.000000 covsirphy-2.9.1/covsirphy/worldwide/policy.py
+drwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-10-24 13:20:11.425138 covsirphy-2.9.1/covsirphy.egg-info/
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     9739 2020-10-24 13:20:11.000000 covsirphy-2.9.1/covsirphy.egg-info/PKG-INFO
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     1518 2020-10-24 13:20:11.000000 covsirphy-2.9.1/covsirphy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        1 2020-10-24 13:20:11.000000 covsirphy-2.9.1/covsirphy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)      150 2020-10-24 13:20:11.000000 covsirphy-2.9.1/covsirphy.egg-info/requires.txt
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)       16 2020-10-24 13:20:11.000000 covsirphy-2.9.1/covsirphy.egg-info/top_level.txt
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)      817 2020-10-24 13:20:11.605351 covsirphy-2.9.1/setup.cfg
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)       38 2020-06-21 12:38:07.000000 covsirphy-2.9.1/setup.py
+drwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-10-24 13:20:11.597372 covsirphy-2.9.1/tests/
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)        0 2020-06-30 14:08:36.000000 covsirphy-2.9.1/tests/__init__.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)      660 2020-08-10 06:19:10.000000 covsirphy-2.9.1/tests/conftest.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     2586 2020-08-27 15:52:34.000000 covsirphy-2.9.1/tests/test_change_finder.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     9288 2020-08-23 10:51:38.000000 covsirphy-2.9.1/tests/test_data_loader.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     4119 2020-08-16 08:42:09.000000 covsirphy-2.9.1/tests/test_ode.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     8380 2020-09-19 07:21:53.000000 covsirphy-2.9.1/tests/test_phase_series.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     6861 2020-08-23 10:51:38.000000 covsirphy-2.9.1/tests/test_phase_unit.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)     2195 2020-10-20 14:16:17.000000 covsirphy-2.9.1/tests/test_policy_measures.py
+-rwxrwxrwx   0 takayahr  (1000) takayahr  (1000)    10848 2020-10-20 13:13:36.000000 covsirphy-2.9.1/tests/test_scenario.py
```

### Comparing `covsirphy-2.9.0/LICENSE` & `covsirphy-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/PKG-INFO` & `covsirphy-2.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: covsirphy
-Version: 2.9.0
+Version: 2.9.1
 Summary: Package for COVID-19 analysis with phase-dependent SIR-derived ODE models
 Home-page: https://github.com/lisphilar/covid19-sir
 Author: Lisphilar
 Author-email: lisphilar@outlook.jp
 License: Apache License 2.0
 Description: | |PyPI version| |Downloads| |PyPI - Python Version| |Build Status|
         | |GitHub license| |Maintainability| |Test Coverage|
@@ -104,15 +104,42 @@
           Hub <https://covid19datahub.io/>`__ and the citation is
         | Guidotti, E., Ardia, D., (2020), "COVID-19 Data Hub", Journal of Open
           Source Software 5(51):2376, doi: 10.21105/joss.02376.
         
         Usage
         -----
         
-        Please read the following documents.
+        Quickest tour of CovsirPhy is here. The following codes analyze the
+        records in Japan, but we can change the country name when creating
+        ``Scenario`` class instance for your own analysis.
+        
+        .. code:: python
+        
+            import covsirphy as cs
+            # Download datasets
+            data_loader = cs.DataLoader("input")
+            jhu_data = data_loader.jhu()
+            population_data = data_loader.population()
+            # Check records
+            snl = cs.Scenario(jhu_data, population_data, country="Japan")
+            snl.records()
+            # S-R trend analysis
+            snl.trend().summary()
+            # Parameter estimation of SIR-F model
+            snl.estimate(cs.SIRF)
+            # History of reproduction number
+            _ = snl.history(target="Rt")
+            # History of parameters
+            _ = snl.history_rate()
+            _ = snl.history(target="rho")
+            # Simulation for 30 days
+            snl.add(days=30)
+            _ = snl.simulate()
+        
+        Further information:
         
         -  `Quickest
            version <https://lisphilar.github.io/covid19-sir/usage_quickest.html>`__
         -  `Quick
            version <https://lisphilar.github.io/covid19-sir/usage_quick.html>`__
         -  `Details:
            phases <https://lisphilar.github.io/covid19-sir/usage_phases.html>`__
```

### Comparing `covsirphy-2.9.0/README.md` & `covsirphy-2.9.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,40 @@
 ```
 
 Main datasets will be retrieved via [COVID-19 Data Hub](https://covid19datahub.io/) and the citation is  
 Guidotti, E., Ardia, D., (2020), "COVID-19 Data Hub", Journal of Open Source Software 5(51):2376, doi: 10.21105/joss.02376.
 
 
 ## Usage
-Please read the following documents.
+Quickest tour of CovsirPhy is here. The following codes analyze the records in Japan, but we can change the country name when creating `Scenario` class instance for your own analysis.
+
+```Python
+import covsirphy as cs
+# Download datasets
+data_loader = cs.DataLoader("input")
+jhu_data = data_loader.jhu()
+population_data = data_loader.population()
+# Check records
+snl = cs.Scenario(jhu_data, population_data, country="Japan")
+snl.records()
+# S-R trend analysis
+snl.trend().summary()
+# Parameter estimation of SIR-F model
+snl.estimate(cs.SIRF)
+# History of reproduction number
+_ = snl.history(target="Rt")
+# History of parameters
+_ = snl.history_rate()
+_ = snl.history(target="rho")
+# Simulation for 30 days
+snl.add(days=30)
+_ = snl.simulate()
+```
+
+Further information:
 
 - [Quickest version](https://lisphilar.github.io/covid19-sir/usage_quickest.html)
 - [Quick version](https://lisphilar.github.io/covid19-sir/usage_quick.html)
 - [Details: phases](https://lisphilar.github.io/covid19-sir/usage_phases.html)
 - [Details: theoretical datasets](https://lisphilar.github.io/covid19-sir/usage_theoretical.html)
 - [Details: policy measures](https://lisphilar.github.io/covid19-sir/usage_policy.html)
 - Example codes in ["example" directory of this repository](https://github.com/lisphilar/covid19-sir/tree/master/example)
```

### Comparing `covsirphy-2.9.0/README.rst` & `covsirphy-2.9.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -96,15 +96,42 @@
   Hub <https://covid19datahub.io/>`__ and the citation is
 | Guidotti, E., Ardia, D., (2020), "COVID-19 Data Hub", Journal of Open
   Source Software 5(51):2376, doi: 10.21105/joss.02376.
 
 Usage
 -----
 
-Please read the following documents.
+Quickest tour of CovsirPhy is here. The following codes analyze the
+records in Japan, but we can change the country name when creating
+``Scenario`` class instance for your own analysis.
+
+.. code:: python
+
+    import covsirphy as cs
+    # Download datasets
+    data_loader = cs.DataLoader("input")
+    jhu_data = data_loader.jhu()
+    population_data = data_loader.population()
+    # Check records
+    snl = cs.Scenario(jhu_data, population_data, country="Japan")
+    snl.records()
+    # S-R trend analysis
+    snl.trend().summary()
+    # Parameter estimation of SIR-F model
+    snl.estimate(cs.SIRF)
+    # History of reproduction number
+    _ = snl.history(target="Rt")
+    # History of parameters
+    _ = snl.history_rate()
+    _ = snl.history(target="rho")
+    # Simulation for 30 days
+    snl.add(days=30)
+    _ = snl.simulate()
+
+Further information:
 
 -  `Quickest
    version <https://lisphilar.github.io/covid19-sir/usage_quickest.html>`__
 -  `Quick
    version <https://lisphilar.github.io/covid19-sir/usage_quick.html>`__
 -  `Details:
    phases <https://lisphilar.github.io/covid19-sir/usage_phases.html>`__
```

### Comparing `covsirphy-2.9.0/covsirphy/__init__.py` & `covsirphy-2.9.1/covsirphy/__init__.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/analysis/example_data.py` & `covsirphy-2.9.1/covsirphy/analysis/example_data.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/analysis/scenario.py` & `covsirphy-2.9.1/covsirphy/analysis/scenario.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/cleaning/cbase.py` & `covsirphy-2.9.1/covsirphy/cleaning/cbase.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/cleaning/country_data.py` & `covsirphy-2.9.1/covsirphy/cleaning/country_data.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/cleaning/dataloader.py` & `covsirphy-2.9.1/covsirphy/cleaning/dataloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,27 +114,28 @@
         Get raw dataset from the URL.
 
         Args:
             url (str): URL to get raw dataset
             is_json (bool): if True, parse the response as Json data.
 
         Returns:
-            (pandas.DataFrame): raw dataset
+            pandas.DataFrame: raw dataset
         """
         if is_json:
             r = requests.get(url)
             try:
                 json_data = r.json()[1]
             except Exception:
                 raise TypeError(
                     f"Unknown data format was used in Web API {url}")
-            df = pd.json_normalize(json_data)
-            return df
-        df = dd.read_csv(url).compute()
-        return df
+            return pd.json_normalize(json_data)
+        try:
+            return dd.read_csv(url, blocksize=None).compute()
+        except (ValueError, FileNotFoundError):
+            return pd.read_csv(url)
 
     def _resolve_filename(self, basename):
         """
         Return the absolute path of the file in the @self.dir_path directory.
 
         Args:
             basename (str): basename of the file, like covid_19_data.csv
```

### Comparing `covsirphy-2.9.0/covsirphy/cleaning/jhu_data.py` & `covsirphy-2.9.1/covsirphy/cleaning/jhu_data.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/cleaning/oxcgrt.py` & `covsirphy-2.9.1/covsirphy/cleaning/oxcgrt.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/cleaning/population.py` & `covsirphy-2.9.1/covsirphy/cleaning/population.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/cleaning/term.py` & `covsirphy-2.9.1/covsirphy/cleaning/term.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/ode/mbase.py` & `covsirphy-2.9.1/covsirphy/ode/mbase.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/ode/sewirf.py` & `covsirphy-2.9.1/covsirphy/ode/sewirf.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/ode/sir.py` & `covsirphy-2.9.1/covsirphy/ode/sir.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/ode/sird.py` & `covsirphy-2.9.1/covsirphy/ode/sird.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/ode/sirf.py` & `covsirphy-2.9.1/covsirphy/ode/sirf.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/ode/sirfv.py` & `covsirphy-2.9.1/covsirphy/ode/sirfv.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/phase/phase_estimator.py` & `covsirphy-2.9.1/covsirphy/phase/phase_estimator.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/phase/phase_series.py` & `covsirphy-2.9.1/covsirphy/phase/phase_series.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/phase/phase_unit.py` & `covsirphy-2.9.1/covsirphy/phase/phase_unit.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/phase/sr_change.py` & `covsirphy-2.9.1/covsirphy/phase/sr_change.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/phase/trend.py` & `covsirphy-2.9.1/covsirphy/phase/trend.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/simulation/estimator.py` & `covsirphy-2.9.1/covsirphy/simulation/estimator.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/simulation/optimize.py` & `covsirphy-2.9.1/covsirphy/simulation/optimize.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/simulation/simulator.py` & `covsirphy-2.9.1/covsirphy/simulation/simulator.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/util/argument.py` & `covsirphy-2.9.1/covsirphy/util/argument.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/util/error.py` & `covsirphy-2.9.1/covsirphy/util/error.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/util/map.py` & `covsirphy-2.9.1/covsirphy/util/map.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/util/plotting.py` & `covsirphy-2.9.1/covsirphy/util/plotting.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/util/stopwatch.py` & `covsirphy-2.9.1/covsirphy/util/stopwatch.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/covsirphy/worldwide/policy.py` & `covsirphy-2.9.1/covsirphy/worldwide/policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,16 +111,19 @@
             covsirphy.PolicyMeasures: self
 
         Notes:
             Countries which do not have @min_len phases will be un-registered.
         """
         min_len = self.ensure_natural_int(min_len, name="min_len")
         for country in self._countries:
-            self.scenario_dict[country].trend(
-                set_phases=True, show_figure=False)
+            try:
+                self.scenario_dict[country].trend(
+                    set_phases=True, show_figure=False)
+            except ValueError:
+                pass
         countries = [
             country for country in self._countries
             if len(self.scenario_dict[country][self.MAIN]) >= min_len
         ]
         self.countries = countries
         return self
```

### Comparing `covsirphy-2.9.0/covsirphy.egg-info/PKG-INFO` & `covsirphy-2.9.1/covsirphy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: covsirphy
-Version: 2.9.0
+Version: 2.9.1
 Summary: Package for COVID-19 analysis with phase-dependent SIR-derived ODE models
 Home-page: https://github.com/lisphilar/covid19-sir
 Author: Lisphilar
 Author-email: lisphilar@outlook.jp
 License: Apache License 2.0
 Description: | |PyPI version| |Downloads| |PyPI - Python Version| |Build Status|
         | |GitHub license| |Maintainability| |Test Coverage|
@@ -104,15 +104,42 @@
           Hub <https://covid19datahub.io/>`__ and the citation is
         | Guidotti, E., Ardia, D., (2020), "COVID-19 Data Hub", Journal of Open
           Source Software 5(51):2376, doi: 10.21105/joss.02376.
         
         Usage
         -----
         
-        Please read the following documents.
+        Quickest tour of CovsirPhy is here. The following codes analyze the
+        records in Japan, but we can change the country name when creating
+        ``Scenario`` class instance for your own analysis.
+        
+        .. code:: python
+        
+            import covsirphy as cs
+            # Download datasets
+            data_loader = cs.DataLoader("input")
+            jhu_data = data_loader.jhu()
+            population_data = data_loader.population()
+            # Check records
+            snl = cs.Scenario(jhu_data, population_data, country="Japan")
+            snl.records()
+            # S-R trend analysis
+            snl.trend().summary()
+            # Parameter estimation of SIR-F model
+            snl.estimate(cs.SIRF)
+            # History of reproduction number
+            _ = snl.history(target="Rt")
+            # History of parameters
+            _ = snl.history_rate()
+            _ = snl.history(target="rho")
+            # Simulation for 30 days
+            snl.add(days=30)
+            _ = snl.simulate()
+        
+        Further information:
         
         -  `Quickest
            version <https://lisphilar.github.io/covid19-sir/usage_quickest.html>`__
         -  `Quick
            version <https://lisphilar.github.io/covid19-sir/usage_quick.html>`__
         -  `Details:
            phases <https://lisphilar.github.io/covid19-sir/usage_phases.html>`__
```

### Comparing `covsirphy-2.9.0/covsirphy.egg-info/SOURCES.txt` & `covsirphy-2.9.1/covsirphy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/setup.cfg` & `covsirphy-2.9.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -14,26 +14,27 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 
 [options]
 packages = find:
 install_requires = 
-	numpy
+	better-exceptions
+	covid19dh
+	dask[complete]
+	fsspec[http]
+	japanmap
 	matplotlib
+	numpy
 	optuna
 	pandas
+	requests
+	ruptures
 	seaborn
-	dask[complete]
 	scipy
 	scikit-learn
-	japanmap
-	better-exceptions
-	requests
-	ruptures
-	covid19dh
 	tabulate
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `covsirphy-2.9.0/tests/conftest.py` & `covsirphy-2.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/tests/test_change_finder.py` & `covsirphy-2.9.1/tests/test_change_finder.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/tests/test_data_loader.py` & `covsirphy-2.9.1/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/tests/test_ode.py` & `covsirphy-2.9.1/tests/test_ode.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/tests/test_phase_series.py` & `covsirphy-2.9.1/tests/test_phase_series.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/tests/test_phase_unit.py` & `covsirphy-2.9.1/tests/test_phase_unit.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/tests/test_policy_measures.py` & `covsirphy-2.9.1/tests/test_policy_measures.py`

 * *Files identical despite different names*

### Comparing `covsirphy-2.9.0/tests/test_scenario.py` & `covsirphy-2.9.1/tests/test_scenario.py`

 * *Files identical despite different names*


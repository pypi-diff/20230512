# Comparing `tmp/scipion-em-facilities-3.0.3.tar.gz` & `tmp/scipion-em-facilities-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-facilities-3.0.3.tar", last modified: Wed May  5 19:39:09 2021, max compression
+gzip compressed data, was "scipion-em-facilities-3.0.4.tar", last modified: Fri May 12 10:15:39 2023, max compression
```

## Comparing `scipion-em-facilities-3.0.3.tar` & `scipion-em-facilities-3.0.4.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 19:39:09.347211 scipion-em-facilities-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       72 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3538 2021-05-05 19:39:09.347211 scipion-em-facilities-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2215 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 19:39:09.343211 scipion-em-facilities-3.0.3/emfacilities/
--rw-r--r--   0 runner    (1001) docker     (121)     1776 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2113 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (121)     1392 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 19:39:09.343211 scipion-em-facilities-3.0.3/emfacilities/protocols/
--rw-r--r--   0 runner    (1001) docker     (121)      689 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3465 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/protocols/getnifs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7463 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/protocols/protocol_monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     7539 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/protocols/protocol_monitor_2d_streamer.py
--rw-r--r--   0 runner    (1001) docker     (121)    14395 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/protocols/protocol_monitor_ctf.py
--rw-r--r--   0 runner    (1001) docker     (121)     9659 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/protocols/protocol_monitor_movie_gain.py
--rw-r--r--   0 runner    (1001) docker     (121)    13991 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/protocols/protocol_monitor_summary.py
--rw-r--r--   0 runner    (1001) docker     (121)    19663 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/protocols/protocol_monitor_system.py
--rw-r--r--   0 runner    (1001) docker     (121)    55485 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/protocols/pynvml.py
--rw-r--r--   0 runner    (1001) docker     (121)    20617 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/protocols/report_html.py
--rw-r--r--   0 runner    (1001) docker     (121)    23869 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/protocols/report_influx.py
--rw-r--r--   0 runner    (1001) docker     (121)     4427 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/protocols/summary_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     3845 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/protocols/transport.py
--rw-r--r--   0 runner    (1001) docker     (121)     1428 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/scipion_icon.gif
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 19:39:09.347211 scipion-em-facilities-3.0.3/emfacilities/templates/
--rw-r--r--   0 runner    (1001) docker     (121)    39444 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/templates/execution.summary.template.html
--rw-r--r--   0 runner    (1001) docker     (121)    22634 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/templates/to_2Dclassification_noDoseWeithed.json.template
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 19:39:09.347211 scipion-em-facilities-3.0.3/emfacilities/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 19:39:09.347211 scipion-em-facilities-3.0.3/emfacilities/tests/protocols/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/tests/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3702 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/tests/protocols/test_protocols_ctf_monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     6391 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/tests/protocols/test_protocols_ctf_streaming.py
--rw-r--r--   0 runner    (1001) docker     (121)     2845 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/tests/protocols/test_protocols_system_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 19:39:09.347211 scipion-em-facilities-3.0.3/emfacilities/tests/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/tests/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1275 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/tests/workflows/test_workflow.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8374 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/tests/workflows/test_workflow_high_throughput.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    20356 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/tests/workflows/test_workflow_streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 19:39:09.347211 scipion-em-facilities-3.0.3/emfacilities/viewers/
--rw-r--r--   0 runner    (1001) docker     (121)     1288 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23322 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/emfacilities/viewers/viewer_monitors.py
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 19:39:09.347211 scipion-em-facilities-3.0.3/scipion_em_facilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3538 2021-05-05 19:39:09.000000 scipion-em-facilities-3.0.3/scipion_em_facilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1682 2021-05-05 19:39:09.000000 scipion-em-facilities-3.0.3/scipion_em_facilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-05 19:39:09.000000 scipion-em-facilities-3.0.3/scipion_em_facilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-05-05 19:39:09.000000 scipion-em-facilities-3.0.3/scipion_em_facilities.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-05-05 19:39:09.000000 scipion-em-facilities-3.0.3/scipion_em_facilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-05-05 19:39:09.000000 scipion-em-facilities-3.0.3/scipion_em_facilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1661 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/secrets_template.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-05 19:39:09.347211 scipion-em-facilities-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4010 2021-05-05 19:32:20.000000 scipion-em-facilities-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:39.110389 scipion-em-facilities-3.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-12 10:15:39.110389 scipion-em-facilities-3.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:39.106388 scipion-em-facilities-3.0.4/emfacilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:39.106388 scipion-em-facilities-3.0.4/emfacilities/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/protocols/getnifs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/protocols/protocol_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/protocols/protocol_monitor_2d_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14395 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/protocols/protocol_monitor_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9659 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/protocols/protocol_monitor_movie_gain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14402 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/protocols/protocol_monitor_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19663 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/protocols/protocol_monitor_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41018 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/protocols/protocol_trackUsedItems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55485 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/protocols/pynvml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24328 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/protocols/report_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23362 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/protocols/report_influx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/protocols/summary_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/protocols/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/scipion_icon.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:39.106388 scipion-em-facilities-3.0.4/emfacilities/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    39513 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/templates/execution.summary.template.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22634 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/templates/to_2Dclassification_noDoseWeithed.json.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:39.106388 scipion-em-facilities-3.0.4/emfacilities/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:39.106388 scipion-em-facilities-3.0.4/emfacilities/tests/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/tests/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/tests/protocols/test_protocols_ctf_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/tests/protocols/test_protocols_ctf_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/tests/protocols/test_protocols_system_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:39.106388 scipion-em-facilities-3.0.4/emfacilities/tests/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/tests/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/tests/workflows/test_workflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8374 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/tests/workflows/test_workflow_high_throughput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20446 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/tests/workflows/test_workflow_streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:39.110389 scipion-em-facilities-3.0.4/emfacilities/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24490 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/emfacilities/viewers/viewer_monitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:15:39.110389 scipion-em-facilities-3.0.4/scipion_em_facilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-12 10:15:39.000000 scipion-em-facilities-3.0.4/scipion_em_facilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-12 10:15:39.000000 scipion-em-facilities-3.0.4/scipion_em_facilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:15:39.000000 scipion-em-facilities-3.0.4/scipion_em_facilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-12 10:15:39.000000 scipion-em-facilities-3.0.4/scipion_em_facilities.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-12 10:15:39.000000 scipion-em-facilities-3.0.4/scipion_em_facilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-12 10:15:39.000000 scipion-em-facilities-3.0.4/scipion_em_facilities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/secrets_template.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 10:15:39.110389 scipion-em-facilities-3.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-12 10:13:53.000000 scipion-em-facilities-3.0.4/setup.py
```

### Comparing `scipion-em-facilities-3.0.3/LICENSE` & `scipion-em-facilities-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.3/PKG-INFO` & `scipion-em-facilities-3.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scipion-em-facilities
-Version: 3.0.3
+Version: 3.0.4
 Summary: Plugin for Cryo-EM facilities to be used within Scipion framework
 Home-page: https://scipion-em.github.io/docs/docs/facilities/facilities.html
 Author: J.M. De la Rosa Trevin, Roberto Marabini, David Maluenda
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: ======================
         Scipion for facilities
```

### Comparing `scipion-em-facilities-3.0.3/README.rst` & `scipion-em-facilities-3.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.3/emfacilities/__init__.py` & `scipion-em-facilities-3.0.4/emfacilities/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 """
 
 import os
 import pwem
 
 from .constants import *
 
-__version__ = "3.0.3"
+__version__ = "3.0.4"
 _logo = "scipion_icon.gif"
 _references = ["delaRosaTrevin201693"]
 
 
 class Plugin(pwem.Plugin):
     _homeVar = EMFACILITIES_HOME_VARNAME 
     _pathVars = [EMFACILITIES_HOME_VARNAME]
```

### Comparing `scipion-em-facilities-3.0.3/emfacilities/bibtex.py` & `scipion-em-facilities-3.0.4/emfacilities/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.3/emfacilities/constants.py` & `scipion-em-facilities-3.0.4/emfacilities/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.3/emfacilities/protocols/__init__.py` & `scipion-em-facilities-3.0.4/emfacilities/protocols/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,12 +9,14 @@
 from .protocol_monitor_ctf import ProtMonitorCTF, MonitorCTF, CTF_LOG_SQLITE
 from .protocol_monitor_system import ProtMonitorSystem
 from .protocol_monitor_movie_gain import ProtMonitorMovieGain, MonitorMovieGain
 
 from .protocol_monitor_2d_streamer import ProtMonitor2dStreamer
 
 from .report_html import ReportHtml
+
+from .protocol_trackUsedItems import UsedItemsTracker
 try:
     from .getnifs import *
 except ImportError:
     print("System monitor functionality compromised.")
 from .pynvml import nvmlInit, NVMLError
```

### Comparing `scipion-em-facilities-3.0.3/emfacilities/protocols/getnifs.py` & `scipion-em-facilities-3.0.4/emfacilities/protocols/getnifs.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.3/emfacilities/protocols/protocol_monitor.py` & `scipion-em-facilities-3.0.4/emfacilities/protocols/protocol_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,18 @@
                       pointerClass='EMProtocol',
                       help="this protocol/s will be monitorized")
 
         form.addParam('samplingInterval', params.IntParam, default=60,
                       label="Sampling Interval (sec)",
                       help="Take one sample each *samplingInterval* seconds")
 
+        form.addParam('monitorTime', params.FloatParam, default=34560,
+                      label="Total Logging time (min)",
+                      help="Log during this interval. 21 days by default")
+
     def _sendMailParams(self, form):
         g = form.addGroup('Email settings')
 
         g.addParam('doMail', params.BooleanParam,
                    label="Enable Email notification?", default=False,
                    help="Allow monitors to notify via email.")
```

### Comparing `scipion-em-facilities-3.0.3/emfacilities/protocols/protocol_monitor_2d_streamer.py` & `scipion-em-facilities-3.0.4/emfacilities/protocols/protocol_monitor_2d_streamer.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.3/emfacilities/protocols/protocol_monitor_ctf.py` & `scipion-em-facilities-3.0.4/emfacilities/protocols/protocol_monitor_ctf.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.3/emfacilities/protocols/protocol_monitor_movie_gain.py` & `scipion-em-facilities-3.0.4/emfacilities/protocols/protocol_monitor_movie_gain.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.3/emfacilities/protocols/protocol_monitor_summary.py` & `scipion-em-facilities-3.0.4/emfacilities/protocols/protocol_monitor_summary.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,17 +87,15 @@
                       help="Raise alarm if defocus is smaller than given "
                            "value")
         form.addParam('astigmatism', params.FloatParam, default=1000,
                       label="Raise Alarm if astigmatism >",
                       help="Raise alarm if astigmatism (defocusU-defocusV)is greater than given "
                            "value")
 
-        form.addParam('monitorTime', params.FloatParam, default=30000,
-                      label="Total Logging time (min)",
-                      help="Log during this interval")
+
 
         form.addSection('System Monitor')
         form.addParam('cpuAlert', params.FloatParam, default=101,
                       label="Raise Alarm if CPU > XX%",
                       help="Raise alarm if memory allocated is greater "
                            "than given percentage")
 
@@ -140,15 +138,14 @@
         form.addSection('HTML Report')
 
         form.addParam("doInflux", params.BooleanParam,
                       label="use grafana/influx",
                       default=False,
                       help="Use grafana+influx vs apache for reports")
         form.addParam('publishCmd', params.StringParam, default='',
-                      condition='doInflux == False',
                       label="Publish command",
                       help="Specify a command to publish the template. "
                            "You can use the special token %(REPORT_FOLDER)s "
                            "that will be replaced with the report folder. "
                            "For example: \n"
                            "rsync -avL %(REPORT_FOLDER)s "
                            "scipion@webserver:public_html/")
@@ -210,14 +207,20 @@
 
     def createReportDir(self):
         self.reportDir = os.path.abspath(self._getExtraPath(self.getProject().getShortName()))
         self.reportPath = os.path.join(self.reportDir, 'index.html')
         # create report dir
         pwutils.makePath(self.reportDir)
 
+        pathRepoSummary = self._getPath("pathRepo.txt")
+        pathRepoSummary = open(pathRepoSummary, "w")
+        pathRepoSummary.write("HTML path to summary: " + self.reportPath)
+        pathRepoSummary.close()
+
+
     def _getAlignProtocol(self):
         for protPointer in self.inputProtocols:
             prot = protPointer.get()
             if isinstance(prot, ProtAlignMovies):
                 return prot
         return None
 
@@ -320,7 +323,18 @@
         else:
             htmlReport = ReportHtml(self, ctfMonitor, sysMonitor, movieGainMonitor,
                                 self.publishCmd.get(),
                                 refreshSecs=self.samplingInterval.get())
             htmlReport.setUp()
 
         return htmlReport
+    def _summary(self):
+        summary = []
+        pathRepoSummary = self._getPath("pathRepo.txt")
+        if not os.path.exists(pathRepoSummary):
+            summary.append("No summary file yet.")
+        else:
+            pathRepoSummary = open(pathRepoSummary, "r")
+            for line in pathRepoSummary.readlines():
+                summary.append(line.rstrip())
+            pathRepoSummary.close()
+        return summary
```

### Comparing `scipion-em-facilities-3.0.3/emfacilities/protocols/protocol_monitor_system.py` & `scipion-em-facilities-3.0.4/emfacilities/protocols/protocol_monitor_system.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.3/emfacilities/protocols/pynvml.py` & `scipion-em-facilities-3.0.4/emfacilities/protocols/pynvml.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.3/emfacilities/protocols/report_html.py` & `scipion-em-facilities-3.0.4/emfacilities/protocols/report_html.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 import json
 import os
 from os.path import join, exists, abspath, basename
 import numpy as np
 import multiprocessing
 from datetime import datetime
+from statistics import median, mean
 
 from pyworkflow.protocol import getUpdatedProtocol
 import pyworkflow.utils as pwutils
 
 from pwem.emlib.image import ImageHandler
 
 from emfacilities import Plugin
@@ -73,28 +74,40 @@
         self.reportDir = protocol.reportDir
         self.provider = SummaryProvider(protocol)
         self.ctfMonitor = ctfMonitor
         self.sysMonitor = sysMonitor
         self.movieGainMonitor = movieGainMonitor
         self.lastThumbIndex = 0
         self.thumbsReady = 0
+        self.itemsAddedMovies = []
+        self.itemsAddedAlign = []
+        self.itemsAddedCTF = []
+
+        self.diffItemsAddedMovies = []
+        self.diffItemsAddedAlign = []
+        self.diffItemsAddedCTF = []
+
+        self.thresholdRate = 0.1
+
         self.thumbPaths = {MIC_THUMBS: [],
                            PSD_THUMBS: [],
                            SHIFT_THUMBS: [],
                            MIC_PATH: [],
                            SHIFT_PATH: [],
                            PSD_PATH: [],
                            MIC_ID: []}
 
         # Get the html template to be used, by default use the one
         # in scipion/config/templates
         self.template = self._getHTMLTemplatePath()
 
         self.publishCmd = publishCmd
         self.refreshSecs = kwargs.get('refreshSecs', 60)
+        self.one_minute_freq_operator = self.refreshSecs / 60.0
+        self.five_minute_freq_operator = self.refreshSecs / 300.0
 
     def _getHTMLTemplatePath(self):
         """ Returns the path of the customized template at
         config/execution.summary.html or the standard scipion HTML template"""
         # Try if there is a customized template
         template = os.path.join(os.path.dirname(pwutils.Config.SCIPION_CONFIG),
                                 'execution.summary.html')
@@ -145,15 +158,15 @@
                          join(self.reportDir, PSD_THUMBS),
                          join(self.reportDir, SHIFT_THUMBS))
         # check if align protocol already has thumbnails
         if (hasattr(self.alignProtocol, 'doComputeMicThumbnail')
                 and self.alignProtocol._doComputeMicThumbnail()):
             self.micThumbSymlinks = True
 
-    def getThumbPaths(self, thumbsDone=0, ctfData=None, ext='png', micIdSet=None):
+    def getThumbPaths(self, thumbsDone=0, ctfData=None, ext='jpg', micIdSet=None):
         """Adds to self.thumbPaths the paths to the report thumbnails
            that come from the alignment and/or ctf protocol.
 
             ===== Params =====
             - thumbsDone: how many thumbnails have already been generated.
                           we will get paths starting from this index
             - ctfData: dict resulting from ctfMonitor.getData()
@@ -267,17 +280,15 @@
             print('Generating images for mic %d' % (i+1))
             # mic thumbnails
             dstImgPath = join(self.reportDir, self.thumbPaths[MIC_THUMBS][i])
             if not exists(dstImgPath):
                 if self.micThumbSymlinks:
                     pwutils.copyFile(self.thumbPaths[MIC_PATH][i], dstImgPath)
                 else:
-                    ih.computeThumbnail(self.thumbPaths[MIC_PATH][i],
-                                        dstImgPath, scaleFactor=micScaleFactor,
-                                        flipOnY=True)
+                    ih.convert(self.thumbPaths[MIC_PATH][i], pwutils.replaceExt(dstImgPath, "jpg"))
 
             # shift plots
             if SHIFT_THUMBS in self.thumbPaths:
                 dstImgPath = join(self.reportDir, self.thumbPaths[SHIFT_THUMBS][i])
                 if not exists(dstImgPath):
                     pwutils.copyFile(self.thumbPaths[SHIFT_PATH][i], dstImgPath)
 
@@ -289,23 +300,21 @@
                     srcImgPath = self.thumbPaths[PSD_PATH][i]
                     dstImgPath = join(self.reportDir, self.thumbPaths[PSD_THUMBS][i])
                     if not exists(dstImgPath) and srcImgPath is not None:
                         if srcImgPath.endswith('psd'):
                             psdImg1 = ih.read(srcImgPath)
                             psdImg1.convertPSD()
                             psdImg1.write(dstImgPath)
-                            ih.computeThumbnail(dstImgPath, dstImgPath,
-                                                scaleFactor=1, flipOnY=True)
+                            ih.convert(dstImgPath, pwutils.replaceExt(dstImgPath, "jpg"))
                         else:
                             pwutils.copyFile(srcImgPath, dstImgPath)
                 else:
                     dstImgPath = join(self.reportDir, self.thumbPaths[PSD_THUMBS][i])
                     if not exists(dstImgPath):
-                        ih.computeThumbnail(self.thumbPaths[PSD_PATH][i],
-                                            dstImgPath, scaleFactor=1, flipOnY=True)
+                        ih.convert(self.thumbPaths[PSD_PATH][i], pwutils.replaceExt(dstImgPath, "jpg"))
 
         return
 
     def processDefocusValues(self, defocusList):
         maxDefocus = self.protocol.maxDefocus.get()*1e-4
         minDefocus = self.protocol.minDefocus.get()*1e-4
         # Convert defocus values to microns
@@ -324,14 +333,58 @@
         zipped = list(zip(values, labels))
         zipped[:0] = [(belowThresh, "0-%0.1f" % minDefocus)]
         # TODO unresolved method for class Iterator in python3
         # zipped.append((aboveThresh, "> %0.1f" % (maxDefocus)))
 
         return zipped
 
+    def rateCalculation(self, protocol):
+        statusRate = ''
+        if protocol == 'importMovies':
+            itemsAdded = self.itemsAddedMovies
+            diffItemsAdded = self.diffItemsAddedMovies
+        elif protocol == 'CTF':
+            itemsAdded = self.itemsAddedCTF
+            diffItemsAdded = self.diffItemsAddedCTF
+        elif protocol == 'Align':
+            itemsAdded = self.itemsAddedAlign
+            diffItemsAdded = self.diffItemsAddedAlign
+        try:
+            diffItemsAdded.append(float(itemsAdded[-1] - itemsAdded[-2]))
+            medianDiffItems = mean(diffItemsAdded[:-1])
+            threshold = self.thresholdRate * medianDiffItems
+            if medianDiffItems + threshold < diffItemsAdded[-1]:
+                statusRate = '<b> ↑ </b>'
+                #statusRate = '<b style="color:#15c51f";> ↑ </b>' #Why does it not work???
+            elif medianDiffItems - threshold > diffItemsAdded[-1]:
+                statusRate = '<b> ↓  </b>'
+            else:
+                statusRate = '<b> --  </b>'
+            rateFreq = round(diffItemsAdded[-1] * self.one_minute_freq_operator, 2)
+            rate, statusRate = self.estimateTimeRate(rateFreq, statusRate)
+            # print('itemsAdded: {}\ndiffItemsAdded: {}\nmedianDiffItems: {} threshold:{}\nrateFreq: {}, rate: {}, statusRate: {}\n'.format(
+            #     itemsAdded, diffItemsAdded, medianDiffItems, threshold, rateFreq, rate, statusRate))
+
+            return rate, statusRate
+        except Exception as e:
+            #print('e: {}'.format(e))
+            return '-', ' '
+
+    def estimateTimeRate(self, diffItem, statusRate):
+        rate1m = round(diffItem * self.one_minute_freq_operator, 2)
+        rate5m = round(diffItem * self.five_minute_freq_operator, 2)
+        if round(rate1m, 2) == 0.00 or round(rate5m, 1) == 0.00:
+            print('ZERO')
+            rate = ''
+            statusRate = 'No items added last {} secs'.format(self.refreshSecs)
+        else:
+            rate = str(rate1m) + ' items/min'
+        #rate = str(rate5m) + ' items/5 mins'
+        return rate, statusRate
+
     def getTimeSeries(self, data):
         from .protocol_monitor_ctf import (PHASE_SHIFT, TIME_STAMP,
                                            DEFOCUS_U, RESOLUTION)
 
         # Get timeStamp
         ts = data[TIME_STAMP]
 
@@ -364,14 +417,15 @@
             return []
         maxValue = int(np.ceil(max(resolutionValues)))
         edges = np.append(np.arange(0, maxValue, RESOLUTION_HIST_BIN_WIDTH), maxValue)
         values, binEdges = np.histogram(resolutionValues, bins=edges, range=(0, maxValue))
         return list(zip(values, binEdges))
 
     def generate(self, finished):
+        self.movieStatus = "-"
         reportTemplate = self.getHTMLReportText()
 
         if not reportTemplate:
             raise Exception("HTML template file '%s' not found. "
                             % self.template)
 
         project = self.protocol.getProject()
@@ -380,37 +434,58 @@
         self.provider.refreshObjects()
 
         for item in self.provider.acquisition:
             if not acquisitionLines == '':
                 acquisitionLines += ','
 
             acquisitionLines += '{propertyName:"%s", propertyValue:"%s"}' % item
-
+        protocolName = ''
         runLines = ''
         wasProtocol = None
         for obj in self.provider.getObjects():
-
             # If it's a protocol
             isProtocol = True if obj.name else False
 
             if isProtocol:
+                protocolName = obj.name
                 if runLines != '':
                     runLines += ']},'
                 runLines += '{protocolName: "%s", output:[' % obj.name
             else:
-                if not wasProtocol:
-                    runLines += ','
-                runLines += '{name: "%s",  size:"%s"}' % (obj.output,
-                                                          obj.outSize)
+                try:
+                    if not wasProtocol:
+                        runLines += ','
+                    if obj.output.find('outputMovies') != -1 and \
+                            protocolName.find("import movies") != -1:#TODOO: si cambia el nombre del protocolo ya no entra
+                        self.itemsAddedMovies.append(obj.outSize)
+                        rate, statusRate = self.rateCalculation('importMovies')
+                    elif obj.output.find('outputCTF') != -1 and \
+                        protocolName.find("CTF") != -1 or \
+                            protocolName.find("ctf") != -1:
+                        self.itemsAddedCTF.append(obj.outSize)
+                        rate, statusRate = self.rateCalculation('CTF')
+                    elif protocolName.find("Align") != -1 or\
+                        protocolName.find("align") != -1:
+                        if obj.output.find("outputMicrographs") != -1:
+                            #print('obj.output: {}'.format(obj.output))
+                            self.itemsAddedAlign.append(obj.outSize)
+                        rate, statusRate = self.rateCalculation('Align')
+                    else:
+                        break
+                    runLines += '{name: "%s",  size: "%s", rate: "%s"}' % (
+                        obj.output,
+                        obj.outSize,
+                        str(statusRate) + ' ' + str(rate))
+                except Exception as e:
+                    print(e)
 
             wasProtocol = isProtocol
-
         # End the runLines JSON object
         runLines += ']}'
-
+        print(runLines, "\n")
         # Ctf monitor chart data
         data = {} if self.ctfMonitor is None else self.ctfMonitor.getData()
 
         if data:
             numMicsDone = len(self.thumbPaths[PSD_THUMBS])
             numMics = len(data[PSD_PATH])
             numMicsToDo = numMics - numMicsDone
```

### Comparing `scipion-em-facilities-3.0.3/emfacilities/protocols/report_influx.py` & `scipion-em-facilities-3.0.4/emfacilities/protocols/report_influx.py`

 * *Files 2% similar despite different names*

```diff
@@ -440,52 +440,35 @@
             newPoints = []
             points = result.get_points()
             for point in points:
                 tags = {}
                 tags['section'] = 'ctf'
                 pointsDict = {}
                 source.append(point['shiftPlotPathLocal']) # shift plot
-                source.append(point['psdPathLocalPng'])    # psd image
-                source.append(point['micPathLocalPng'])    # micrograph
+                source.append(pwutils.replaceExt(point['psdPathLocalPng'], 'jpg'))    # psd image
+                source.append(pwutils.replaceExt(point['micPathLocalPng'], 'jpg'))    # micrograph
 
-                # default value 512
-                try:
-                    X, Y, Z, N = self.ih.getDimensions(point['psdPathLocal'])
-                except:
-                    print("file %s does not exist"% point['psdPathLocal'])
-                if X > 512:
-                    scaleFactor = X // 512
-                else:
-                    scaleFactor = 1
+                self.ih.convert(point['psdPathLocal'], pwutils.replaceExt(point['psdPathLocalPng'], 'jpg'))
 
-                self.ih.computeThumbnail(point['psdPathLocal'], point['psdPathLocalPng'],
-                                    scaleFactor=scaleFactor, flipOnY=True)
-
-                X, Y, Z, N = self.ih.getDimensions(point['micPathLocal'])
-                if X > 512:
-                    scaleFactor = X // 512
-                else:
-                    scaleFactor = 1
-                self.ih.computeThumbnail(point['micPathLocal'], point['micPathLocalPng'],
-                                    scaleFactor=scaleFactor, flipOnY=True)
+                self.ih.convert(point['micPathLocal'], pwutils.replaceExt(point['micPathLocalPng'], 'jpg'))
 
                 # add files to transfer list
                 target.append(os.path.join(self.projectName,
                                            basename(point['shiftPlotPathLocal'])))
-                target.append(os.path.join(self.projectName,
-                                           basename(point['psdPathLocalPng'])))
-                target.append(os.path.join(self.projectName,
-                                           basename(point['micPathLocalPng'])))
+                target.append(os.path.join(self.projectName, basename(pwutils.replaceExt(point['psdPathLocalPng'], 'jpg'))))
+                target.append(os.path.join(self.projectName, basename(pwutils.replaceExt(point['micPathLocalPng'], 'jpg'))))
                 #
                 point['transferImage'] = True
                 pointsDict['time'] = point['time']
                 tags['id'] = point['id']
                 del point['time']
                 del point['section']
                 del point['id']
+                point['micPath'] = point['micPath'].replace('.png', '.jpg')
+                point['psdPath'] = point['psdPath'].replace('.png', '.jpg')
                 pointsDict['fields'] = point
                 pointsDict['tags'] = tags
                 pointsDict['measurement'] = self.projectName
                 newPoints.append(pointsDict)
             try:
                 connect.put(source, target)
             except Exception as e:
```

### Comparing `scipion-em-facilities-3.0.3/emfacilities/protocols/summary_provider.py` & `scipion-em-facilities-3.0.4/emfacilities/protocols/summary_provider.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.3/emfacilities/protocols/transport.py` & `scipion-em-facilities-3.0.4/emfacilities/protocols/transport.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.3/emfacilities/scipion_icon.gif` & `scipion-em-facilities-3.0.4/emfacilities/scipion_icon.gif`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.3/emfacilities/templates/execution.summary.template.html` & `scipion-em-facilities-3.0.4/emfacilities/templates/execution.summary.template.html`

 * *Files 0% similar despite different names*

```diff
@@ -243,14 +243,15 @@
                 <DIV id="runs" class="column column-7">
                     <H2>Runs summary</H2>
                     <TABLE id="runsTable" class='center'>
                         <TR>
                             <TH>Name</TH>
                             <TH>Output</TH>
                             <TH>Number</TH>
+                            <TH>Rate</TH>
                         </TR>
                     </TABLE>
                 </DIV>
             </DIV>
 
             <SECTION id="ctf">
                 <H2 class="sectionTitle"><span class="glyphicon glyphicon-triangle-bottom glyphExpand" aria-hidden="true"></span>CTF histograms</H2>
@@ -345,19 +346,19 @@
 
         function addRuns(){
             // Get the runs table
             var runsTable = $('#runsTable');
 
             // For each protocol property
             $.each(report.runs, function(index, value){
-                var line = "<TR class='protocolLine'><TD>" + value.protocolName + "</TD><TD colspan='2'></TD></TR>";
+                var line = "<TR class='protocolLine'><TD>" + value.protocolName + "</TD><TD colspan='3'></TD></TR>";
                 $(runsTable).append(line);
 
                 $.each(value.output, function(index, value){
-                    var outputLine = "<TR><TD></TD><TD>" + value.name + "</TD><TD class='center'>" + value.size + "</TD></TR>";
+                    var outputLine = "<TR><TD></TD><TD>" + value.name + "</TD><TD class='center'>" + value.size + "</TD><TD>" + value.rate + "</TD></TR>";
                     $(runsTable).append(outputLine);
 
                 });
             });
         };
 
         function addMovieGainChart () {
```

#### html2text {}

```diff
@@ -11,15 +11,15 @@
 Start time: %(startTime)s
 Last update: %(dateStr)s
 Duration: %(projectDuration)s
 Status: %(projectStatus)s
 Scipion version: %(scipionVersion)s
 ***** Acquisition *****
 ***** Runs summary *****
-Name Output Number
+Name Output Number Rate
 ***** CTF histograms *****
 
 ***** CTF Time Series *****
 
 ***** Movie gain monitor *****
 
 ***** System monitor *****
```

### Comparing `scipion-em-facilities-3.0.3/emfacilities/templates/to_2Dclassification_noDoseWeithed.json.template` & `scipion-em-facilities-3.0.4/emfacilities/templates/to_2Dclassification_noDoseWeithed.json.template`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.3/emfacilities/tests/__init__.py` & `scipion-em-facilities-3.0.4/emfacilities/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.3/emfacilities/tests/protocols/test_protocols_ctf_monitor.py` & `scipion-em-facilities-3.0.4/emfacilities/tests/protocols/test_protocols_ctf_monitor.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.3/emfacilities/tests/protocols/test_protocols_ctf_streaming.py` & `scipion-em-facilities-3.0.4/emfacilities/tests/protocols/test_protocols_ctf_streaming.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.3/emfacilities/tests/protocols/test_protocols_system_monitor.py` & `scipion-em-facilities-3.0.4/emfacilities/tests/protocols/test_protocols_system_monitor.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.3/emfacilities/tests/workflows/test_workflow.py` & `scipion-em-facilities-3.0.4/emfacilities/tests/workflows/test_workflow.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.3/emfacilities/tests/workflows/test_workflow_high_throughput.py` & `scipion-em-facilities-3.0.4/emfacilities/tests/workflows/test_workflow_high_throughput.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.3/emfacilities/tests/workflows/test_workflow_streaming.py` & `scipion-em-facilities-3.0.4/emfacilities/tests/workflows/test_workflow_streaming.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,14 +164,18 @@
                                                      doRaise=True)
         protOF = self.newProtocol(XmippProtMovieCorr,
                                   objLabel='Movie alignment',
                                   doSaveMovie=False,
                                   doComputePSD=False,
                                   alignFrame0=3,
                                   alignFrameN=10,
+                                  autoControlPoints=False,
+                                  controlPointX=3,
+                                  controlPointY=3,
+                                  controlPointT=5,
                                   sumFrame0=3,
                                   sumFrameN=10,
                                   doApplyDoseFilter=False)
         protOF.inputMovies.set(protImport)
         protOF.inputMovies.setExtended('outputMovies')
         self.proj.launchProtocol(protOF, wait=False)
         self._waitOutput(protOF, 'outputMicrographs')
@@ -353,27 +357,25 @@
             slowSearch=False
         )
         self.proj.launchProtocol(protCtf, wait=False)
         self._waitOutput(protCtf, 'outputCTF')
 
         self._waitUntilMinSize(protCtf.outputCTF)
 
-        # Select some good averages from the iterations mrcs a
+        # Select some good averages from the iterations mrcs
 
         ProtRelion2Autopick = Domain.importFromPlugin('relion.protocols',
                                                       'ProtRelion2Autopick')
-        relion_RUN_COMPUTE = Domain.importFromPlugin('relion', 'RUN_COMPUTE')
 
         protPick = self.newProtocol(
             ProtRelion2Autopick, objLabel='autopick refs',
             inputMicrographs=protImport.outputMicrographs,
             ctfRelations=protCtf.outputCTF,
-            runType=relion_RUN_COMPUTE,
             inputReferences=protAvgs.outputAverages,
-            numberOfMpi = 2
+            numberOfMpi=2
         )
         self.launchProtocol(protPick)
 
 
 class TestFrameStacking(pwtests.BaseTest):
     """ Test the cases where the input movies are input as individual frames.
     """
```

### Comparing `scipion-em-facilities-3.0.3/emfacilities/viewers/__init__.py` & `scipion-em-facilities-3.0.4/emfacilities/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.3/emfacilities/viewers/viewer_monitors.py` & `scipion-em-facilities-3.0.4/emfacilities/viewers/viewer_monitors.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,18 @@
 import pyworkflow.utils as pwutils
 import pyworkflow.viewer as pwviewer
 from pwem.viewers.plotter import EmPlotter
 
 import emfacilities.protocols as monitorProt
 from emfacilities.protocols.protocol_monitor_system import MonitorSystem
 
+# anim is a object created by FuncAnimation. 
+# The object created by FuncAnimation must be assigned to a global 
+# variable apparently; if it's assigned to a local variable,  nothing will happen.
+anim = None 
 
 class ProtMonitorCTFViewer(pwviewer.Viewer):
     _environments = [pwviewer.DESKTOP_TKINTER]
     _label = 'ctf monitor'
     _targets = [monitorProt.ProtMonitorCTF]
 
     def _visualize(self, obj, **kwargs):
@@ -67,15 +71,15 @@
         self.oldWin = self.win
 
         self.lines = {}
         self.init = True
         self.stop = False
 
     def _getTitle(self):
-        return ("Use scrool wheel to change view window (win=%d)\n "
+        return ("Use mouse scroll wheel to change view window (win=%d)\n "
                 "S stops, C continues plotting" % self.win)
 
     def onscroll(self, event):
 
         if event.button == 'up':
             self.win += self.step
         else:
@@ -86,15 +90,14 @@
         if self.oldWin != self.win:
             self.ax.set_title(self._getTitle())
             self.oldWin = self.win
         self.animate()
         EmPlotter.show(self)
 
     def press(self, event):
-
         sys.stdout.flush()
         if event.key == 'S':
             self.stop = True
             self.ax.set_title('Plot is Stopped. Press C to continue plotting')
         elif event.key == 'C':
             self.ax.set_title(self._getTitle())
             self.stop = False
@@ -176,15 +179,15 @@
         self.oldWin = self.win
 
         self.lines = {}
         self.init = True
         self.stop = False
 
     def _getTitle(self):
-        return ("Use scrool wheel to change view window (win=%d)\n "
+        return ("Use scroll wheel to change view window (win=%d)\n "
                 "S stops, C continues plotting" % self.win)
 
     def onscroll(self, event):
 
         if event.button == 'up':
             self.win += self.step
         else:
@@ -320,35 +323,35 @@
         self.lines = {}
         self.init = True
         self.stop = False
 
         self.nifName = nifName
 
     def _getTitle(self):
-        return ("Use scrool wheel to change view window (win=%d)\n "
+        return ("Use scroll wheel to change view window (win=%d)\n "
                 "S stops, C continues plotting. Toggle ON/OFF GPU_X "
                 "by pressing X\n"
                 "c/n/d toggle ON-OFF cpu/network/disk usage\n" % self.win)
 
     def onscroll(self, event):
-
         if event.button == 'up':
             self.win += self.step
         else:
             self.win -= self.step
             if self.win < self.step:
                 self.win = self.step
 
         if self.oldWin != self.win:
             self.ax.set_title(self._getTitle())
             self.oldWin = self.win
         self.animate()
         EmPlotter.show(self)
 
-    def press(self, event):
+    def onpress(self, event):
+
         def numericKey(key):
             self.colorChanged = True
             number = int(key)
             index = 3 + number * 3
             if (index + 3) > self.lenPlots:
                 return
             if self.color['gpuMem_%d' % number] != 'w':
@@ -433,19 +436,21 @@
         EmPlotter.show(self)
 
     def has_been_closed(self, ax):
         fig = ax.figure.canvas.manager
         active_fig_managers = plt._pylab_helpers.Gcf.figs.values()
         return fig not in active_fig_managers
 
-    def animate(self, i=0):  # do NOT remove i
 
+    def animate(self, i=0):  # do NOT remove i, i is a counter
+                             # each call to animate  increases the
+                             # value of i by 1. 'i' is not used here but
+                             # is a mandatory argument to the function
         if self.stop:
             return
-
         data = self.monitor.getData()
         self.x = data['idValues']
         for k, v in self.lines.items():
             self.y = data[k]
 
             lenght = len(self.x)
             imin = max(0, len(self.x) - self.win)
@@ -457,26 +462,45 @@
         self.colorChanged = False
         self.ax.relim()
         self.ax.autoscale()
         self.ax.grid(True)
         self.ax.legend(loc=2).get_frame().set_alpha(0.5)
 
     def paint(self, labels):
+        # The object created by FuncAnimation, that is 'anim', must be assigned to a global variable 
+        # apparently; if it's assigned to a local variable, nothing will happen.
+        global anim
+        def on_press(event):
+            """I have no idea why but  mpl_connect fails
+             if a direct call to self.onpress is done"""
+            self.onpress(event)
+
+        def on_scroll(event):
+            """I have no idea why but this mpl_connect fails
+             if a direct call to self.onscroll is done"""
+            self.onscroll(event)
+
+        def animate(i=0):
+            """I have no idea why but this mpl_connect fails
+             if a direct call to self.animate is done"""
+            self.animate(i)
+
         for label in labels:
             labelValue = self.monitor.getData()[label]
             color = self.color[label]
             self.lines[label], = self.ax.plot(labelValue, '-', label=label,
                                               color=color)
         self.ax.legend()
         anim = animation.FuncAnimation(
-            self.fig, self.animate,
+            self.fig, animate,
             interval=self.monitor.samplingInterval * 1000)  # miliseconds
 
-        self.fig.canvas.mpl_connect('scroll_event', self.onscroll)
-        self.fig.canvas.mpl_connect('key_press_event', self.press)
+
+        self.fig.canvas.mpl_connect('scroll_event', on_scroll)
+        self.fig.canvas.mpl_connect('key_press_event', on_press)
         EmPlotter.show(self)
 
     def show(self):
         colortypes = ["k", "b", "r", "g", "y", "c", "m"]
         lenColortypes = len(colortypes)
         self.colorChanged = True
         self.color = {}
```

### Comparing `scipion-em-facilities-3.0.3/scipion_em_facilities.egg-info/PKG-INFO` & `scipion-em-facilities-3.0.4/scipion_em_facilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scipion-em-facilities
-Version: 3.0.3
+Version: 3.0.4
 Summary: Plugin for Cryo-EM facilities to be used within Scipion framework
 Home-page: https://scipion-em.github.io/docs/docs/facilities/facilities.html
 Author: J.M. De la Rosa Trevin, Roberto Marabini, David Maluenda
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: ======================
         Scipion for facilities
```

### Comparing `scipion-em-facilities-3.0.3/scipion_em_facilities.egg-info/SOURCES.txt` & `scipion-em-facilities-3.0.4/scipion_em_facilities.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 emfacilities/protocols/getnifs.py
 emfacilities/protocols/protocol_monitor.py
 emfacilities/protocols/protocol_monitor_2d_streamer.py
 emfacilities/protocols/protocol_monitor_ctf.py
 emfacilities/protocols/protocol_monitor_movie_gain.py
 emfacilities/protocols/protocol_monitor_summary.py
 emfacilities/protocols/protocol_monitor_system.py
+emfacilities/protocols/protocol_trackUsedItems.py
 emfacilities/protocols/pynvml.py
 emfacilities/protocols/report_html.py
 emfacilities/protocols/report_influx.py
 emfacilities/protocols/summary_provider.py
 emfacilities/protocols/transport.py
 emfacilities/templates/execution.summary.template.html
 emfacilities/templates/to_2Dclassification_noDoseWeithed.json.template
```

### Comparing `scipion-em-facilities-3.0.3/secrets_template.cfg` & `scipion-em-facilities-3.0.4/secrets_template.cfg`

 * *Files identical despite different names*

### Comparing `scipion-em-facilities-3.0.3/setup.py` & `scipion-em-facilities-3.0.4/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/pe-configurator-0.1.5.tar.gz` & `tmp/pe-configurator-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pe-configurator-0.1.5.tar", last modified: Fri Apr 28 14:20:28 2023, max compression
+gzip compressed data, was "pe-configurator-0.1.6.tar", last modified: Fri May 12 08:43:04 2023, max compression
```

## Comparing `pe-configurator-0.1.5.tar` & `pe-configurator-0.1.6.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:20:28.874263 pe-configurator-0.1.5/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    11456 2023-04-28 14:20:28.874263 pe-configurator-0.1.5/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10809 2023-04-19 17:29:14.000000 pe-configurator-0.1.5/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:20:28.820097 pe-configurator-0.1.5/blueprints/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      192 2023-04-19 17:29:14.000000 pe-configurator-0.1.5/blueprints/test.yaml
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:20:28.820097 pe-configurator-0.1.5/data/
--rw-r--r--   0 daniel    (1000) daniel    (1000)  2290335 2023-04-13 09:58:40.000000 pe-configurator-0.1.5/data/calibration_files.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:20:28.841763 pe-configurator-0.1.5/examples/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8196 2023-04-19 17:29:14.000000 pe-configurator-0.1.5/examples/.DS_Store
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:20:28.852597 pe-configurator-0.1.5/examples/test_GW190412/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   821276 2023-04-19 17:29:14.000000 pe-configurator-0.1.5/examples/test_GW190412/test.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      669 2023-04-19 17:29:14.000000 pe-configurator-0.1.5/examples/test_GW190412/test.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8592 2023-04-19 17:29:14.000000 pe-configurator-0.1.5/examples/test_GW190412/test.pdf
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:20:28.852597 pe-configurator-0.1.5/examples/test_GW190521/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   822260 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/examples/test_GW190521/test.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      710 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/examples/test_GW190521/test.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8565 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/examples/test_GW190521/test.pdf
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:20:28.863430 pe-configurator-0.1.5/examples/test_GW190814/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   844645 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/examples/test_GW190814/test.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      699 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/examples/test_GW190814/test.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8839 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/examples/test_GW190814/test.pdf
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:20:28.874263 pe-configurator-0.1.5/examples/test_GW191109/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   846106 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/examples/test_GW191109/test.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      682 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/examples/test_GW191109/test.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8663 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/examples/test_GW191109/test.pdf
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:20:28.874263 pe-configurator-0.1.5/pe_configurator.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    11456 2023-04-28 14:20:28.000000 pe-configurator-0.1.5/pe_configurator.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1024 2023-04-28 14:20:28.000000 pe-configurator-0.1.5/pe_configurator.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-04-28 14:20:28.000000 pe-configurator-0.1.5/pe_configurator.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)      142 2023-04-28 14:20:28.000000 pe-configurator-0.1.5/pe_configurator.egg-info/entry_points.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       94 2023-04-28 14:20:28.000000 pe-configurator-0.1.5/pe_configurator.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       15 2023-04-28 14:20:28.000000 pe-configurator-0.1.5/pe_configurator.egg-info/top_level.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:20:28.874263 pe-configurator-0.1.5/peconfigurator/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6877 2023-04-28 13:12:38.000000 pe-configurator-0.1.5/peconfigurator/asimov.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       73 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/peconfigurator/asimov_template.yaml
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:20:28.874263 pe-configurator-0.1.5/peconfigurator/auxiliary/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/peconfigurator/auxiliary/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10401 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/peconfigurator/auxiliary/make_report.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7114 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/peconfigurator/auxiliary/run_analyzer.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    10105 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/peconfigurator/get_settings.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    15907 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/peconfigurator/proc_samples.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2897 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/peconfigurator/run_on_many_events.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1313 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/pyproject.toml
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-04-28 14:20:28.874263 pe-configurator-0.1.5/setup.cfg
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:20:28.874263 pe-configurator-0.1.5/tests/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6015 2023-04-19 17:29:15.000000 pe-configurator-0.1.5/tests/test_get_settings.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:43:04.530877 pe-configurator-0.1.6/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1100 2023-05-12 08:39:45.000000 pe-configurator-0.1.6/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    11478 2023-05-12 08:43:04.530877 pe-configurator-0.1.6/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    10809 2023-04-19 17:29:14.000000 pe-configurator-0.1.6/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:43:04.490877 pe-configurator-0.1.6/blueprints/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      192 2023-04-19 17:29:14.000000 pe-configurator-0.1.6/blueprints/test.yaml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:43:04.490877 pe-configurator-0.1.6/data/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)  2290335 2023-04-13 09:58:40.000000 pe-configurator-0.1.6/data/calibration_files.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:43:04.500877 pe-configurator-0.1.6/examples/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8196 2023-04-19 17:29:14.000000 pe-configurator-0.1.6/examples/.DS_Store
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:43:04.510877 pe-configurator-0.1.6/examples/test_GW190412/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   821276 2023-04-19 17:29:14.000000 pe-configurator-0.1.6/examples/test_GW190412/test.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      669 2023-04-19 17:29:14.000000 pe-configurator-0.1.6/examples/test_GW190412/test.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8592 2023-04-19 17:29:14.000000 pe-configurator-0.1.6/examples/test_GW190412/test.pdf
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:43:04.510877 pe-configurator-0.1.6/examples/test_GW190521/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   822260 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/examples/test_GW190521/test.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      710 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/examples/test_GW190521/test.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8565 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/examples/test_GW190521/test.pdf
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:43:04.520877 pe-configurator-0.1.6/examples/test_GW190814/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   844645 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/examples/test_GW190814/test.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      699 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/examples/test_GW190814/test.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8839 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/examples/test_GW190814/test.pdf
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:43:04.520877 pe-configurator-0.1.6/examples/test_GW191109/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   846106 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/examples/test_GW191109/test.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      682 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/examples/test_GW191109/test.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8663 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/examples/test_GW191109/test.pdf
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:43:04.520877 pe-configurator-0.1.6/pe_configurator.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    11478 2023-05-12 08:43:04.000000 pe-configurator-0.1.6/pe_configurator.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1032 2023-05-12 08:43:04.000000 pe-configurator-0.1.6/pe_configurator.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-05-12 08:43:04.000000 pe-configurator-0.1.6/pe_configurator.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      142 2023-05-12 08:43:04.000000 pe-configurator-0.1.6/pe_configurator.egg-info/entry_points.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       94 2023-05-12 08:43:04.000000 pe-configurator-0.1.6/pe_configurator.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       15 2023-05-12 08:43:04.000000 pe-configurator-0.1.6/pe_configurator.egg-info/top_level.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:43:04.520877 pe-configurator-0.1.6/peconfigurator/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6877 2023-04-28 13:12:38.000000 pe-configurator-0.1.6/peconfigurator/asimov.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       73 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/peconfigurator/asimov_template.yaml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:43:04.520877 pe-configurator-0.1.6/peconfigurator/auxiliary/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/peconfigurator/auxiliary/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    10401 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/peconfigurator/auxiliary/make_report.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7114 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/peconfigurator/auxiliary/run_analyzer.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    10105 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/peconfigurator/get_settings.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    15907 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/peconfigurator/proc_samples.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2897 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/peconfigurator/run_on_many_events.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1313 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/pyproject.toml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-05-12 08:43:04.530877 pe-configurator-0.1.6/setup.cfg
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:43:04.520877 pe-configurator-0.1.6/tests/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6015 2023-04-19 17:29:15.000000 pe-configurator-0.1.6/tests/test_get_settings.py
```

### Comparing `pe-configurator-0.1.5/PKG-INFO` & `pe-configurator-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pe-configurator
-Version: 0.1.5
+Version: 0.1.6
 Summary: Tools to identify waveform settings and prior bounds for gravitational wave parameter estimation.
 Author-email: Hector Estelles <hector.estelles@ligo.org>, Serguei Ossokine <serguei.ossokine@ligo.org>, Daniel Williams <daniel.williams@ligo.org>
 License: MIT
 Project-URL: Source code, https://git.ligo.org/pe/get_eob_settings
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: asimov
+License-File: LICENSE
 
 # Introduction
 This package provides scripts that automatically try to determine some settings that must be applied for PE runs, especially for time-domain waveforms.
 The settings try to strike a balance between being conservative and being feasible.
 
 ### Top-level description
 The main script to use is `proc_samples.py`.  Given a preliminary PE run, it will perform some basic checks and then generate recommended PE settings. It can also optionally generate a `json` format result for automatic ingestion by `asimov` and a more detailed standalone, human-readable report. Users are _highly_ encouraged to take a look at the report.
```

### Comparing `pe-configurator-0.1.5/README.md` & `pe-configurator-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.5/data/calibration_files.txt` & `pe-configurator-0.1.6/data/calibration_files.txt`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.5/examples/.DS_Store` & `pe-configurator-0.1.6/examples/.DS_Store`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.5/examples/test_GW190412/test.html` & `pe-configurator-0.1.6/examples/test_GW190412/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.5/examples/test_GW190412/test.json` & `pe-configurator-0.1.6/examples/test_GW190412/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.5/examples/test_GW190412/test.pdf` & `pe-configurator-0.1.6/examples/test_GW190412/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.5/examples/test_GW190521/test.html` & `pe-configurator-0.1.6/examples/test_GW190521/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.5/examples/test_GW190521/test.json` & `pe-configurator-0.1.6/examples/test_GW190521/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.5/examples/test_GW190521/test.pdf` & `pe-configurator-0.1.6/examples/test_GW190521/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.5/examples/test_GW190814/test.html` & `pe-configurator-0.1.6/examples/test_GW190814/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.5/examples/test_GW190814/test.json` & `pe-configurator-0.1.6/examples/test_GW190814/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.5/examples/test_GW190814/test.pdf` & `pe-configurator-0.1.6/examples/test_GW190814/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.5/examples/test_GW191109/test.html` & `pe-configurator-0.1.6/examples/test_GW191109/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.5/examples/test_GW191109/test.json` & `pe-configurator-0.1.6/examples/test_GW191109/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.5/examples/test_GW191109/test.pdf` & `pe-configurator-0.1.6/examples/test_GW191109/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.5/pe_configurator.egg-info/PKG-INFO` & `pe-configurator-0.1.6/pe_configurator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pe-configurator
-Version: 0.1.5
+Version: 0.1.6
 Summary: Tools to identify waveform settings and prior bounds for gravitational wave parameter estimation.
 Author-email: Hector Estelles <hector.estelles@ligo.org>, Serguei Ossokine <serguei.ossokine@ligo.org>, Daniel Williams <daniel.williams@ligo.org>
 License: MIT
 Project-URL: Source code, https://git.ligo.org/pe/get_eob_settings
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: asimov
+License-File: LICENSE
 
 # Introduction
 This package provides scripts that automatically try to determine some settings that must be applied for PE runs, especially for time-domain waveforms.
 The settings try to strike a balance between being conservative and being feasible.
 
 ### Top-level description
 The main script to use is `proc_samples.py`.  Given a preliminary PE run, it will perform some basic checks and then generate recommended PE settings. It can also optionally generate a `json` format result for automatic ingestion by `asimov` and a more detailed standalone, human-readable report. Users are _highly_ encouraged to take a look at the report.
```

### Comparing `pe-configurator-0.1.5/pe_configurator.egg-info/SOURCES.txt` & `pe-configurator-0.1.6/pe_configurator.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 pyproject.toml
 blueprints/test.yaml
 data/calibration_files.txt
 examples/.DS_Store
 examples/test_GW190412/test.html
 examples/test_GW190412/test.json
```

### Comparing `pe-configurator-0.1.5/peconfigurator/asimov.py` & `pe-configurator-0.1.6/peconfigurator/asimov.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.5/peconfigurator/auxiliary/make_report.py` & `pe-configurator-0.1.6/peconfigurator/auxiliary/make_report.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.5/peconfigurator/auxiliary/run_analyzer.py` & `pe-configurator-0.1.6/peconfigurator/auxiliary/run_analyzer.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.5/peconfigurator/get_settings.py` & `pe-configurator-0.1.6/peconfigurator/get_settings.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.5/peconfigurator/proc_samples.py` & `pe-configurator-0.1.6/peconfigurator/proc_samples.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.5/peconfigurator/run_on_many_events.py` & `pe-configurator-0.1.6/peconfigurator/run_on_many_events.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.5/pyproject.toml` & `pe-configurator-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.5/tests/test_get_settings.py` & `pe-configurator-0.1.6/tests/test_get_settings.py`

 * *Files identical despite different names*


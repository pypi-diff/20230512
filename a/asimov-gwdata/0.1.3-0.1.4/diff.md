# Comparing `tmp/asimov-gwdata-0.1.3.tar.gz` & `tmp/asimov-gwdata-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asimov-gwdata-0.1.3.tar", last modified: Fri Apr 28 14:19:29 2023, max compression
+gzip compressed data, was "asimov-gwdata-0.1.4.tar", last modified: Fri May 12 08:23:42 2023, max compression
```

## Comparing `asimov-gwdata-0.1.3.tar` & `asimov-gwdata-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:19:29.648443 asimov-gwdata-0.1.3/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      655 2023-04-28 14:19:29.648443 asimov-gwdata-0.1.3/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      148 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.3/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:19:29.648443 asimov-gwdata-0.1.3/asimov_gwdata.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      655 2023-04-28 14:19:29.000000 asimov-gwdata-0.1.3/asimov_gwdata.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      452 2023-04-28 14:19:29.000000 asimov-gwdata-0.1.3/asimov_gwdata.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-04-28 14:19:29.000000 asimov-gwdata-0.1.3/asimov_gwdata.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)      104 2023-04-28 14:19:29.000000 asimov-gwdata-0.1.3/asimov_gwdata.egg-info/entry_points.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       45 2023-04-28 14:19:29.000000 asimov-gwdata-0.1.3/asimov_gwdata.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        9 2023-04-28 14:19:29.000000 asimov-gwdata-0.1.3/asimov_gwdata.egg-info/top_level.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:19:29.648443 asimov-gwdata-0.1.3/blueprints/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      168 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.3/blueprints/asimov-analysis.yaml
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:19:29.648443 asimov-gwdata-0.1.3/datafind/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        5 2023-02-19 16:31:31.000000 asimov-gwdata-0.1.3/datafind/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5690 2023-04-28 13:13:22.000000 asimov-gwdata-0.1.3/datafind/asimov.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1273 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.3/datafind/datafind_template.yml
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3349 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.3/datafind/main.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1037 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.3/pyproject.toml
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-28 14:19:29.648443 asimov-gwdata-0.1.3/scripts/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      251 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.3/scripts/asimov-test-script.sh
--rw-r--r--   0 daniel    (1000) daniel    (1000)      121 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.3/scripts/test-calibration-dump.yaml
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-04-28 14:19:29.648443 asimov-gwdata-0.1.3/setup.cfg
--rw-r--r--   0 daniel    (1000) daniel    (1000)      122 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.3/test_settings.yaml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:23:42.550984 asimov-gwdata-0.1.4/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1065 2023-05-12 08:22:13.000000 asimov-gwdata-0.1.4/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      677 2023-05-12 08:23:42.550984 asimov-gwdata-0.1.4/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      148 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.4/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:23:42.550984 asimov-gwdata-0.1.4/asimov_gwdata.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      677 2023-05-12 08:23:42.000000 asimov-gwdata-0.1.4/asimov_gwdata.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      460 2023-05-12 08:23:42.000000 asimov-gwdata-0.1.4/asimov_gwdata.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-05-12 08:23:42.000000 asimov-gwdata-0.1.4/asimov_gwdata.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      104 2023-05-12 08:23:42.000000 asimov-gwdata-0.1.4/asimov_gwdata.egg-info/entry_points.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       45 2023-05-12 08:23:42.000000 asimov-gwdata-0.1.4/asimov_gwdata.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        9 2023-05-12 08:23:42.000000 asimov-gwdata-0.1.4/asimov_gwdata.egg-info/top_level.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:23:42.550984 asimov-gwdata-0.1.4/blueprints/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      168 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.4/blueprints/asimov-analysis.yaml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:23:42.550984 asimov-gwdata-0.1.4/datafind/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        5 2023-02-19 16:31:31.000000 asimov-gwdata-0.1.4/datafind/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     6093 2023-05-11 13:58:29.000000 asimov-gwdata-0.1.4/datafind/asimov.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1273 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.4/datafind/datafind_template.yml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3349 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.4/datafind/main.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1037 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.4/pyproject.toml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-12 08:23:42.550984 asimov-gwdata-0.1.4/scripts/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      251 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.4/scripts/asimov-test-script.sh
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      121 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.4/scripts/test-calibration-dump.yaml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-05-12 08:23:42.550984 asimov-gwdata-0.1.4/setup.cfg
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      122 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.4/test_settings.yaml
```

### Comparing `asimov-gwdata-0.1.3/PKG-INFO` & `asimov-gwdata-0.1.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: asimov-gwdata
-Version: 0.1.3
+Version: 0.1.4
 Summary: An asimov plugin to make downloading gravitational wave data easier
 Author-email: Daniel Williams <daniel.williams@ligo.org>
 License: MIT
 Project-URL: Source code, https://git.ligo.org/asimov/asimov-gwdatahelp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: docs
+License-File: LICENSE
 
 # Asimov GWData
 
 This package provides an asimov pipeline for collecting published gravitational wave data for use in parameter estimation studies.
```

### Comparing `asimov-gwdata-0.1.3/asimov_gwdata.egg-info/PKG-INFO` & `asimov-gwdata-0.1.4/asimov_gwdata.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: asimov-gwdata
-Version: 0.1.3
+Version: 0.1.4
 Summary: An asimov plugin to make downloading gravitational wave data easier
 Author-email: Daniel Williams <daniel.williams@ligo.org>
 License: MIT
 Project-URL: Source code, https://git.ligo.org/asimov/asimov-gwdatahelp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: docs
+License-File: LICENSE
 
 # Asimov GWData
 
 This package provides an asimov pipeline for collecting published gravitational wave data for use in parameter estimation studies.
```

### Comparing `asimov-gwdata-0.1.3/datafind/asimov.py` & `asimov-gwdata-0.1.4/datafind/asimov.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import importlib
 import os
 import configparser
 import glob
+import pprint
 
 import asimov.pipeline
 
 from asimov import config
 import htcondor
 from asimov.utils import set_directory
 
@@ -153,7 +154,18 @@
 
         if os.path.exists(f"{self.production.rundir}/posterior/"):
             results = glob.glob(f"{self.production.rundir}/posterior/*")
 
             outputs["samples"] = results[0]
 
         return outputs
+
+    def html(self):
+        """Return the HTML representation of this pipeline."""
+        out = ""
+        if self.production.status in {"finished", "uploaded"}:
+            out += """<div class="asimov-pipeline">"""
+            pp = pprint.PrettyPrinter(indent=4)
+            out += f"<pre>{ pp.pprint(self.collect_assets()) }</pre>"
+            out += """</div>"""
+
+        return out
```

### Comparing `asimov-gwdata-0.1.3/datafind/datafind_template.yml` & `asimov-gwdata-0.1.4/datafind/datafind_template.yml`

 * *Files identical despite different names*

### Comparing `asimov-gwdata-0.1.3/datafind/main.py` & `asimov-gwdata-0.1.4/datafind/main.py`

 * *Files identical despite different names*

### Comparing `asimov-gwdata-0.1.3/pyproject.toml` & `asimov-gwdata-0.1.4/pyproject.toml`

 * *Files identical despite different names*


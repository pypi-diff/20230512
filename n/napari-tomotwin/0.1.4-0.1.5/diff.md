# Comparing `tmp/napari-tomotwin-0.1.4.tar.gz` & `tmp/napari-tomotwin-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-tomotwin-0.1.4.tar", last modified: Thu May 11 08:36:32 2023, max compression
+gzip compressed data, was "napari-tomotwin-0.1.5.tar", last modified: Fri May 12 07:23:22 2023, max compression
```

## Comparing `napari-tomotwin-0.1.4.tar` & `napari-tomotwin-0.1.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:36:32.582879 napari-tomotwin-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:36:32.578879 napari-tomotwin-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:36:32.582879 napari-tomotwin-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-05-11 08:36:13.000000 napari-tomotwin-0.1.4/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-11 08:36:13.000000 napari-tomotwin-0.1.4/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:36:32.582879 napari-tomotwin-0.1.4/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-11 08:36:13.000000 napari-tomotwin-0.1.4/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-11 08:36:13.000000 napari-tomotwin-0.1.4/.napari-hub/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-11 08:36:13.000000 napari-tomotwin-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-05-11 08:36:13.000000 napari-tomotwin-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 08:36:13.000000 napari-tomotwin-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-11 08:36:32.582879 napari-tomotwin-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-11 08:36:13.000000 napari-tomotwin-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-11 08:36:13.000000 napari-tomotwin-0.1.4/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-11 08:36:13.000000 napari-tomotwin-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-11 08:36:13.000000 napari-tomotwin-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-11 08:36:32.586880 napari-tomotwin-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:36:32.582879 napari-tomotwin-0.1.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 08:36:13.000000 napari-tomotwin-0.1.4/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:36:32.582879 napari-tomotwin-0.1.4/src/napari_tomotwin/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-11 08:36:13.000000 napari-tomotwin-0.1.4/src/napari_tomotwin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:36:32.582879 napari-tomotwin-0.1.4/src/napari_tomotwin/_qt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 08:36:13.000000 napari-tomotwin-0.1.4/src/napari_tomotwin/_qt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:36:32.582879 napari-tomotwin-0.1.4/src/napari_tomotwin/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 08:36:13.000000 napari-tomotwin-0.1.4/src/napari_tomotwin/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-11 08:36:13.000000 napari-tomotwin-0.1.4/src/napari_tomotwin/_tests/test_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 08:36:32.000000 napari-tomotwin-0.1.4/src/napari_tomotwin/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-05-11 08:36:13.000000 napari-tomotwin-0.1.4/src/napari_tomotwin/load_umap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-11 08:36:13.000000 napari-tomotwin-0.1.4/src/napari_tomotwin/make_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-11 08:36:13.000000 napari-tomotwin-0.1.4/src/napari_tomotwin/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:36:32.582879 napari-tomotwin-0.1.4/src/napari_tomotwin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-11 08:36:32.000000 napari-tomotwin-0.1.4/src/napari_tomotwin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-11 08:36:32.000000 napari-tomotwin-0.1.4/src/napari_tomotwin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:36:32.000000 napari-tomotwin-0.1.4/src/napari_tomotwin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-11 08:36:32.000000 napari-tomotwin-0.1.4/src/napari_tomotwin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-11 08:36:32.000000 napari-tomotwin-0.1.4/src/napari_tomotwin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-11 08:36:32.000000 napari-tomotwin-0.1.4/src/napari_tomotwin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-11 08:36:13.000000 napari-tomotwin-0.1.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:22.047435 napari-tomotwin-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:22.043435 napari-tomotwin-0.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:22.047435 napari-tomotwin-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-05-12 07:23:00.000000 napari-tomotwin-0.1.5/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-12 07:23:00.000000 napari-tomotwin-0.1.5/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:22.047435 napari-tomotwin-0.1.5/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-12 07:23:00.000000 napari-tomotwin-0.1.5/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-12 07:23:00.000000 napari-tomotwin-0.1.5/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-12 07:23:00.000000 napari-tomotwin-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-05-12 07:23:00.000000 napari-tomotwin-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-12 07:23:00.000000 napari-tomotwin-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-12 07:23:22.047435 napari-tomotwin-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-12 07:23:00.000000 napari-tomotwin-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-12 07:23:00.000000 napari-tomotwin-0.1.5/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-12 07:23:00.000000 napari-tomotwin-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 07:23:00.000000 napari-tomotwin-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-12 07:23:22.047435 napari-tomotwin-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:22.047435 napari-tomotwin-0.1.5/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:00.000000 napari-tomotwin-0.1.5/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:22.047435 napari-tomotwin-0.1.5/src/napari_tomotwin/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-12 07:23:00.000000 napari-tomotwin-0.1.5/src/napari_tomotwin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:22.047435 napari-tomotwin-0.1.5/src/napari_tomotwin/_qt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:00.000000 napari-tomotwin-0.1.5/src/napari_tomotwin/_qt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:22.047435 napari-tomotwin-0.1.5/src/napari_tomotwin/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:00.000000 napari-tomotwin-0.1.5/src/napari_tomotwin/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-12 07:23:00.000000 napari-tomotwin-0.1.5/src/napari_tomotwin/_tests/test_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-12 07:23:22.000000 napari-tomotwin-0.1.5/src/napari_tomotwin/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-12 07:23:00.000000 napari-tomotwin-0.1.5/src/napari_tomotwin/load_umap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-12 07:23:00.000000 napari-tomotwin-0.1.5/src/napari_tomotwin/make_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-12 07:23:00.000000 napari-tomotwin-0.1.5/src/napari_tomotwin/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:22.047435 napari-tomotwin-0.1.5/src/napari_tomotwin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-12 07:23:22.000000 napari-tomotwin-0.1.5/src/napari_tomotwin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-12 07:23:22.000000 napari-tomotwin-0.1.5/src/napari_tomotwin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 07:23:22.000000 napari-tomotwin-0.1.5/src/napari_tomotwin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-12 07:23:22.000000 napari-tomotwin-0.1.5/src/napari_tomotwin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-12 07:23:22.000000 napari-tomotwin-0.1.5/src/napari_tomotwin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-12 07:23:22.000000 napari-tomotwin-0.1.5/src/napari_tomotwin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-12 07:23:00.000000 napari-tomotwin-0.1.5/tox.ini
```

### Comparing `napari-tomotwin-0.1.4/.github/workflows/test_and_deploy.yml` & `napari-tomotwin-0.1.5/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.4/.gitignore` & `napari-tomotwin-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.4/.napari-hub/config.yml` & `napari-tomotwin-0.1.5/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.4/.pre-commit-config.yaml` & `napari-tomotwin-0.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.4/LICENSE` & `napari-tomotwin-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.4/PKG-INFO` & `napari-tomotwin-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-tomotwin
-Version: 0.1.4
+Version: 0.1.5
 Summary: Several tools for the work with TomoTwin
 Home-page: https://github.com/MPI-Dortmund/napari-tomotwin
 Author: Thorsten Wagner
 Author-email: twa1@posteo.de
 License: MPL-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `napari-tomotwin-0.1.4/README.md` & `napari-tomotwin-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.4/setup.cfg` & `napari-tomotwin-0.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 [options]
 packages = find:
 install_requires = 
 	numpy
 	pandas
 	matplotlib
-	tqdm
 	napari-clusters-plotter >= 0.7.2
 python_requires = >=3.10
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = 
 	setuptools-scm
```

### Comparing `napari-tomotwin-0.1.4/src/napari_tomotwin/load_umap.py` & `napari-tomotwin-0.1.5/src/napari_tomotwin/load_umap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import napari
 import pathlib
-from magicgui import magic_factory, tqdm
+from magicgui import magic_factory
 from napari_clusters_plotter._plotter import PlotterWidget
 import pandas as pd
 import numpy as np
 from matplotlib.patches import Circle
 
 plotter_widget: PlotterWidget = None
 circle: Circle = None
```

### Comparing `napari-tomotwin-0.1.4/src/napari_tomotwin/make_targets.py` & `napari-tomotwin-0.1.5/src/napari_tomotwin/make_targets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from magicgui import magic_factory, tqdm
+from magicgui import magic_factory
 import pathlib
 import pandas as pd
 import numpy as np
 import os
 from typing import List, Tuple
```

### Comparing `napari-tomotwin-0.1.4/src/napari_tomotwin/napari.yaml` & `napari-tomotwin-0.1.5/src/napari_tomotwin/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.4/src/napari_tomotwin.egg-info/PKG-INFO` & `napari-tomotwin-0.1.5/src/napari_tomotwin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-tomotwin
-Version: 0.1.4
+Version: 0.1.5
 Summary: Several tools for the work with TomoTwin
 Home-page: https://github.com/MPI-Dortmund/napari-tomotwin
 Author: Thorsten Wagner
 Author-email: twa1@posteo.de
 License: MPL-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `napari-tomotwin-0.1.4/src/napari_tomotwin.egg-info/SOURCES.txt` & `napari-tomotwin-0.1.5/src/napari_tomotwin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-tomotwin-0.1.4/tox.ini` & `napari-tomotwin-0.1.5/tox.ini`

 * *Files identical despite different names*


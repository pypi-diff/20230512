# Comparing `tmp/scdiffeq_plots-0.0.1rc0.tar.gz` & `tmp/scdiffeq_plots-0.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scdiffeq_plots-0.0.1rc0.tar", last modified: Thu May 11 20:21:37 2023, max compression
+gzip compressed data, was "scdiffeq_plots-0.0.1rc1.tar", last modified: Fri May 12 16:51:03 2023, max compression
```

## Comparing `scdiffeq_plots-0.0.1rc0.tar` & `scdiffeq_plots-0.0.1rc1.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:21:37.795623 scdiffeq_plots-0.0.1rc0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-11 20:21:26.000000 scdiffeq_plots-0.0.1rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-11 20:21:37.795623 scdiffeq_plots-0.0.1rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 20:21:26.000000 scdiffeq_plots-0.0.1rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:21:37.791622 scdiffeq_plots-0.0.1rc0/scdiffeq_plots/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-11 20:21:26.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-11 20:21:26.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots/_loss_viz_ax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:21:37.795623 scdiffeq_plots-0.0.1rc0/scdiffeq_plots/core/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-11 20:21:26.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-05-11 20:21:26.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots/core/_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-11 20:21:26.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots/core/_plot_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-11 20:21:26.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots/core/_style_spines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:21:37.795623 scdiffeq_plots-0.0.1rc0/scdiffeq_plots/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-11 20:21:26.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-11 20:21:26.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots/utils/_abc_parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:21:37.795623 scdiffeq_plots-0.0.1rc0/scdiffeq_plots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-11 20:21:37.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-11 20:21:37.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:21:37.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 20:21:37.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 20:21:37.000000 scdiffeq_plots-0.0.1rc0/scdiffeq_plots.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 20:21:37.795623 scdiffeq_plots-0.0.1rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-11 20:21:26.000000 scdiffeq_plots-0.0.1rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:51:03.604220 scdiffeq_plots-0.0.1rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-12 16:50:52.000000 scdiffeq_plots-0.0.1rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-12 16:51:03.604220 scdiffeq_plots-0.0.1rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-12 16:50:52.000000 scdiffeq_plots-0.0.1rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:51:03.604220 scdiffeq_plots-0.0.1rc1/scdiffeq_plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-12 16:50:52.000000 scdiffeq_plots-0.0.1rc1/scdiffeq_plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-12 16:50:52.000000 scdiffeq_plots-0.0.1rc1/scdiffeq_plots/_color_map_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-12 16:50:52.000000 scdiffeq_plots-0.0.1rc1/scdiffeq_plots/_discretized_color_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-12 16:50:52.000000 scdiffeq_plots-0.0.1rc1/scdiffeq_plots/_loss_viz_ax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-12 16:50:52.000000 scdiffeq_plots-0.0.1rc1/scdiffeq_plots/_temporal_cmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-12 16:50:52.000000 scdiffeq_plots-0.0.1rc1/scdiffeq_plots/_temporal_colormap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-12 16:50:52.000000 scdiffeq_plots-0.0.1rc1/scdiffeq_plots/_temporal_distances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:51:03.604220 scdiffeq_plots-0.0.1rc1/scdiffeq_plots/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-12 16:50:52.000000 scdiffeq_plots-0.0.1rc1/scdiffeq_plots/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-05-12 16:50:52.000000 scdiffeq_plots-0.0.1rc1/scdiffeq_plots/core/_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-12 16:50:52.000000 scdiffeq_plots-0.0.1rc1/scdiffeq_plots/core/_plot_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-12 16:50:52.000000 scdiffeq_plots-0.0.1rc1/scdiffeq_plots/core/_style_spines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:51:03.604220 scdiffeq_plots-0.0.1rc1/scdiffeq_plots/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-12 16:50:52.000000 scdiffeq_plots-0.0.1rc1/scdiffeq_plots/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-12 16:50:52.000000 scdiffeq_plots-0.0.1rc1/scdiffeq_plots/utils/_abc_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-12 16:50:52.000000 scdiffeq_plots-0.0.1rc1/scdiffeq_plots/utils/_extract_func_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-12 16:50:52.000000 scdiffeq_plots-0.0.1rc1/scdiffeq_plots/utils/_info_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:51:03.604220 scdiffeq_plots-0.0.1rc1/scdiffeq_plots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-12 16:51:03.000000 scdiffeq_plots-0.0.1rc1/scdiffeq_plots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-12 16:51:03.000000 scdiffeq_plots-0.0.1rc1/scdiffeq_plots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 16:51:03.000000 scdiffeq_plots-0.0.1rc1/scdiffeq_plots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-12 16:51:03.000000 scdiffeq_plots-0.0.1rc1/scdiffeq_plots.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-12 16:51:03.000000 scdiffeq_plots-0.0.1rc1/scdiffeq_plots.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 16:51:03.604220 scdiffeq_plots-0.0.1rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-12 16:50:52.000000 scdiffeq_plots-0.0.1rc1/setup.py
```

### Comparing `scdiffeq_plots-0.0.1rc0/LICENSE` & `scdiffeq_plots-0.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `scdiffeq_plots-0.0.1rc0/scdiffeq_plots/_loss_viz_ax.py` & `scdiffeq_plots-0.0.1rc1/scdiffeq_plots/_loss_viz_ax.py`

 * *Files identical despite different names*

### Comparing `scdiffeq_plots-0.0.1rc0/scdiffeq_plots/core/_plot.py` & `scdiffeq_plots-0.0.1rc1/scdiffeq_plots/core/_plot.py`

 * *Files identical despite different names*

### Comparing `scdiffeq_plots-0.0.1rc0/scdiffeq_plots/core/_plot_dimensions.py` & `scdiffeq_plots-0.0.1rc1/scdiffeq_plots/core/_plot_dimensions.py`

 * *Files identical despite different names*

### Comparing `scdiffeq_plots-0.0.1rc0/scdiffeq_plots/core/_style_spines.py` & `scdiffeq_plots-0.0.1rc1/scdiffeq_plots/core/_style_spines.py`

 * *Files identical despite different names*

### Comparing `scdiffeq_plots-0.0.1rc0/scdiffeq_plots.egg-info/PKG-INFO` & `scdiffeq_plots-0.0.1rc1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: scdiffeq-plots
-Version: 0.0.1rc0
+Name: scdiffeq_plots
+Version: 0.0.1rc1
 Summary: Plotting functions associated wtih analyses from scDiffEq
-Home-page: https://github.com/mvinyard/sc-neural-diffeqs
+Home-page: https://github.com/scDiffEq/scdiffeq-plots
 Author: Michael E. Vinyard - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard
 Author-email: mvinyard@broadinstitute.org
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `scdiffeq_plots-0.0.1rc0/setup.py` & `scdiffeq_plots-0.0.1rc1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 import re
 import os
 import sys
 
 setuptools.setup(
     name="scdiffeq_plots",
-    version="0.0.1rc0",
+    version="0.0.1rc1",
     python_requires=">3.9.0",
     author="Michael E. Vinyard - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard",
     author_email="mvinyard@broadinstitute.org",
-    url="https://github.com/mvinyard/sc-neural-diffeqs",
+    url="https://github.com/scDiffEq/scdiffeq-plots",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     description="Plotting functions associated wtih analyses from scDiffEq",
     packages=setuptools.find_packages(),
     install_requires=[
         "matplotlib>=3.7.1",
     ],
```


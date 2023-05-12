# Comparing `tmp/puma-hep-0.2.4.tar.gz` & `tmp/puma-hep-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puma-hep-0.2.4.tar", last modified: Thu Apr  6 17:39:26 2023, max compression
+gzip compressed data, was "puma-hep-0.2.5.tar", last modified: Fri May 12 15:12:42 2023, max compression
```

## Comparing `puma-hep-0.2.4.tar` & `puma-hep-0.2.5.tar`

### file list

```diff
@@ -1,54 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:39:26.337468 puma-hep-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-04-06 17:39:16.000000 puma-hep-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 17:39:16.000000 puma-hep-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-04-06 17:39:26.337468 puma-hep-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-04-06 17:39:16.000000 puma-hep-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:39:26.329468 puma-hep-0.2.4/puma/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23113 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/histogram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:39:26.329468 puma-hep-0.2.4/puma/hlplots/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/hlplots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/hlplots/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/hlplots/tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/line_plot_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/pie.py
--rw-r--r--   0 runner    (1001) docker     (123)    27383 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/plot_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20514 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/roc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:39:26.333468 puma-hep-0.2.4/puma/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:39:26.333468 puma-hep-0.2.4/puma/tests/hlplots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/tests/hlplots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/tests/hlplots/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/tests/hlplots/test_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)    27366 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/tests/test_line_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/tests/test_pie_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/tests/test_plot_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18980 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/tests/test_roc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13678 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/tests/test_var_vs_eff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:39:26.333468 puma-hep-0.2.4/puma/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/tests/utils/test_discriminant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/tests/utils/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/tests/utils/test_histogram_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/tests/utils/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/tests/utils/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:39:26.337468 puma-hep-0.2.4/puma/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/utils/discriminant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/utils/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/utils/histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    24727 2023-04-06 17:39:16.000000 puma-hep-0.2.4/puma/var_vs_eff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 17:39:26.337468 puma-hep-0.2.4/puma_hep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-04-06 17:39:26.000000 puma-hep-0.2.4/puma_hep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-06 17:39:26.000000 puma-hep-0.2.4/puma_hep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 17:39:26.000000 puma-hep-0.2.4/puma_hep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 17:39:26.000000 puma-hep-0.2.4/puma_hep.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-06 17:39:26.000000 puma-hep-0.2.4/puma_hep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-06 17:39:26.000000 puma-hep-0.2.4/puma_hep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-06 17:39:16.000000 puma-hep-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-06 17:39:26.337468 puma-hep-0.2.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      435 2023-04-06 17:39:16.000000 puma-hep-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:42.061276 puma-hep-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-05-12 15:12:32.000000 puma-hep-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:12:32.000000 puma-hep-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-05-12 15:12:42.061276 puma-hep-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-05-12 15:12:32.000000 puma-hep-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:42.053275 puma-hep-0.2.5/puma/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/fraction_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22871 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/histogram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:42.053275 puma-hep-0.2.5/puma/hlplots/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/hlplots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16037 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/hlplots/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/hlplots/tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/line_plot_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/pie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28069 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/plot_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20420 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/roc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:42.057276 puma-hep-0.2.5/puma/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:42.057276 puma-hep-0.2.5/puma/tests/hlplots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/hlplots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/hlplots/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/hlplots/test_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27352 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/test_line_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/test_pie_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/test_plot_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18908 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/test_roc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14968 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/test_var_vs_eff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/test_var_vs_var.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:42.057276 puma-hep-0.2.5/puma/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/utils/test_discriminant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/utils/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11373 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/utils/test_histogram_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/utils/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:42.057276 puma-hep-0.2.5/puma/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/utils/discriminant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/utils/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/utils/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15827 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/var_vs_eff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13877 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/var_vs_var.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:42.061276 puma-hep-0.2.5/puma_hep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-05-12 15:12:42.000000 puma-hep-0.2.5/puma_hep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-12 15:12:42.000000 puma-hep-0.2.5/puma_hep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:12:42.000000 puma-hep-0.2.5/puma_hep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:12:41.000000 puma-hep-0.2.5/puma_hep.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-12 15:12:42.000000 puma-hep-0.2.5/puma_hep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-12 15:12:42.000000 puma-hep-0.2.5/puma_hep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-12 15:12:32.000000 puma-hep-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-12 15:12:42.061276 puma-hep-0.2.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      435 2023-05-12 15:12:32.000000 puma-hep-0.2.5/setup.py
```

### Comparing `puma-hep-0.2.4/LICENSE` & `puma-hep-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.4/PKG-INFO` & `puma-hep-0.2.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: puma-hep
-Version: 0.2.4
-Summary: Plotting API for HEP flavour tagging plots.
-Home-page: https://github.com/umami-hep/puma
-Keywords: machine learning,flavour tagging,plots
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # puma - Plotting UMami Api
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Umami docs](https://img.shields.io/badge/info-documentation-informational)](https://umami-hep.github.io/puma/)
 [![PyPI version](https://badge.fury.io/py/puma-hep.svg)](https://badge.fury.io/py/puma-hep)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6607414.svg)](https://doi.org/10.5281/zenodo.6607414)
 
@@ -71,21 +61,8 @@
 
 On a machine/cluster with singularity installed:
 
 ```bash
 singularity shell -B $PWD docker://gitlab-registry.cern.ch/atlas-flavor-tagging-tools/training-images/puma-images/puma:latest
 ```
 
-### Extended image for development
-
-_For development, just replace the tag of the image_:
-
-`latest` -> `latest-dev`
-
-In addition to the minimal requirements that are required to use `puma`, the
-`puma:latest-dev` image has the `requirements.txt` from the `puma` repo installed as
-well.
-This means that packages like `pytest`, `black`, `pylint`, etc. are installed as well.
-However, note that `puma` itself is not installed in that image such that the dev-version
-on your machine can be used/tested.
-
 **The images are automatically updated via GitHub and pushed to this [repository registry](https://gitlab.cern.ch/atlas-flavor-tagging-tools/training-images/puma-images/container_registry).**
```

### Comparing `puma-hep-0.2.4/README.md` & `puma-hep-0.2.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: puma-hep
+Version: 0.2.5
+Summary: Plotting API for HEP flavour tagging plots.
+Home-page: https://github.com/umami-hep/puma
+Keywords: machine learning,flavour tagging,plots
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # puma - Plotting UMami Api
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Umami docs](https://img.shields.io/badge/info-documentation-informational)](https://umami-hep.github.io/puma/)
 [![PyPI version](https://badge.fury.io/py/puma-hep.svg)](https://badge.fury.io/py/puma-hep)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6607414.svg)](https://doi.org/10.5281/zenodo.6607414)
 
@@ -61,21 +71,8 @@
 
 On a machine/cluster with singularity installed:
 
 ```bash
 singularity shell -B $PWD docker://gitlab-registry.cern.ch/atlas-flavor-tagging-tools/training-images/puma-images/puma:latest
 ```
 
-### Extended image for development
-
-_For development, just replace the tag of the image_:
-
-`latest` -> `latest-dev`
-
-In addition to the minimal requirements that are required to use `puma`, the
-`puma:latest-dev` image has the `requirements.txt` from the `puma` repo installed as
-well.
-This means that packages like `pytest`, `black`, `pylint`, etc. are installed as well.
-However, note that `puma` itself is not installed in that image such that the dev-version
-on your machine can be used/tested.
-
 **The images are automatically updated via GitHub and pushed to this [repository registry](https://gitlab.cern.ch/atlas-flavor-tagging-tools/training-images/puma-images/container_registry).**
```

### Comparing `puma-hep-0.2.4/puma/histogram.py` & `puma-hep-0.2.5/puma/histogram.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,21 @@
 from ftag import Flavour, Flavours
 
 from puma.plot_base import PlotBase, PlotLineObject
 from puma.utils import get_good_colours, global_config, logger
 from puma.utils.histogram import hist_ratio, hist_w_unc
 
 
-class Histogram(
-    PlotLineObject
-):  # pylint: disable=too-few-public-methods,too-many-instance-attributes
+class Histogram(PlotLineObject):
     """
     Histogram class storing info about histogram and allows to calculate ratio w.r.t
     other histograms.
     """
 
-    def __init__(  # pylint: disable=too-many-arguments
+    def __init__(
         self,
         values: np.ndarray,
         weights: np.ndarray = None,
         ratio_group: str = None,
         flavour: str | Flavour = None,
         add_flavour_label: bool = True,
         histtype: str = "step",
@@ -75,17 +73,16 @@
             if len(values) == 0:
                 logger.warning("Histogram is empty.")
         else:
             raise ValueError(
                 "Invalid type of histogram input data. Allowed values are "
                 "numpy.ndarray, list, pandas.core.series.Series"
             )
-        if weights is not None:
-            if len(values) != len(weights):
-                raise ValueError("`values` and `weights` are not of same length.")
+        if weights is not None and len(values) != len(weights):
+            raise ValueError("`values` and `weights` are not of same length.")
 
         self.values = values
         self.weights = weights
         self.ratio_group = ratio_group
         self.flavour = Flavours[flavour] if isinstance(flavour, str) else flavour
         self.add_flavour_label = add_flavour_label
         self.histtype = histtype
@@ -169,30 +166,30 @@
         # To use the matplotlib.step() function later on, the first bin is duplicated
         ratio = np.append(np.array([ratio[0]]), ratio)
         ratio_unc = np.append(np.array([ratio_unc[0]]), ratio_unc)
 
         return (ratio, ratio_unc)
 
 
-class HistogramPlot(PlotBase):  # pylint: disable=too-many-instance-attributes
-    """Histogram plot class"""
+class HistogramPlot(PlotBase):
+    """Histogram plot class."""
 
-    def __init__(  # pylint: disable=too-many-arguments
+    def __init__(
         self,
         bins=40,
         bins_range: tuple = None,
         discrete_vals: list = None,
         norm: bool = True,
         logy: bool = False,
         bin_width_in_ylabel: bool = False,
         underoverflow: bool = False,
         grid: bool = False,
         **kwargs,
     ) -> None:
-        """histogram plot properties
+        """histogram plot properties.
 
         Parameters
         ----------
         bins : int or numpy.ndarray or list, optional
             If bins is an int, it defines the number of equal-width bins in the given
             range. If bins is a sequence, it defines a monotonically increasing array
             of bin edges, including the rightmost edge, allowing for non-uniform
@@ -288,15 +285,15 @@
 
         self.plot_objects[key] = histogram
         self.add_order.append(key)
         if reference is True:
             self.set_reference(key)
 
     def set_reference(self, key: str):
-        """Setting the reference histogram curves used in the ratios
+        """Setting the reference histogram curves used in the ratios.
 
         Parameters
         ----------
         key : str
             Unique identifier of histogram object
         """
         if self.reference_object is None:
@@ -321,20 +318,19 @@
             matplotlib Line2D object
 
         Raises
         ------
         ValueError
             If specified bins type is not supported.
         """
-        if self.ylabel is not None:
-            if self.norm and "norm" not in self.ylabel.lower():
-                logger.warning(
-                    "You are plotting normalised distributions but 'norm' is not "
-                    "included in your y-label."
-                )
+        if self.ylabel is not None and self.norm and "norm" not in self.ylabel.lower():
+            logger.warning(
+                "You are plotting normalised distributions but 'norm' is not "
+                "included in your y-label."
+            )
         plt_handles = []
 
         # Calculate bins of stacked histograms to ensure all histograms fit in plot
         if isinstance(self.bins, (np.ndarray, list)):
             logger.debug("Using bin edges defined in plot instance.")
             if self.bins_range is not None:
                 logger.warning(
@@ -418,15 +414,15 @@
             self.bins = bins
 
         self.plotting_done = True
         return plt_handles
 
     def get_discrete_values(self, elem: object):
         """Get discrete values of a variable and adjust the
-        bins accordingly
+        bins accordingly.
 
         Parameters
         ----------
         elem : histogram class
             Histogram we want to calculate the bins containing discrete values for
 
         Returns
@@ -439,15 +435,14 @@
         ValueError
             If the bin width is larger than 1 such that potentially not
             all discrete values are in a seperate bin
         ValueError
             If the number of bins is set to 1 such that no values can be
             distinguished
         """
-
         if len(elem.bin_edges) > 1:
             if abs(elem.bin_edges[1] - elem.bin_edges[0]) <= 1:
                 indice = []
                 for i in range(len(elem.bin_edges) - 1):
                     # Only keep this bin edge if one of the discrete
                     # values is withing this and the next bin edge
                     # TODO: This has to be improved.
@@ -472,22 +467,22 @@
             else:
                 raise ValueError(
                     "Bin width is larger than 1. Choose a binning with a bin"
                     " width<= 1 to plot only discrete values."
                 )
         else:
             raise ValueError(
-                "Choose a binning with more than one bin in order to plot"
-                "only discrete values."
+                "Choose a binning with more than one bin in order to plot only discrete"
+                " values."
             )
 
         return bins
 
     def get_reference_histo(self, histo):
-        """Get reference histogram from list of references
+        """Get reference histogram from list of references.
 
         Parameters
         ----------
         histo : puma.histogram.Histogram
             Histogram we want to calculate the ratio for
 
         Returns
@@ -496,15 +491,14 @@
             Identifier of the corresponding reference histogram
 
         Raises
         ------
         ValueError
             If no reference histo was found or multiple matches.
         """
-
         matches = 0
         reference_histo = None
 
         for key in self.reference_object:
             reference_candidate = self.plot_objects[key]
             if histo.ratio_group is not None:
                 if histo.ratio_group == reference_candidate.ratio_group:
@@ -512,16 +506,16 @@
                     reference_histo = reference_candidate
             else:
                 matches += 1
                 reference_histo = reference_candidate
 
         if matches != 1:
             raise ValueError(
-                f"Found {matches} matching reference candidates, but only one match "
-                "is allowed."
+                f"Found {matches} matching reference candidates, but only one match is"
+                " allowed."
             )
 
         logger.debug(
             "Reference histogram for '%s' is '%s'", histo.key, reference_histo.key
         )
 
         return reference_histo
@@ -579,15 +573,14 @@
         smaller than 0.01, scientific notation will be used.
 
         Raises
         ------
         ValueError
             If plotting_done is False (therefore `bins` is not yet calculated)
         """
-
         if self.plotting_done is False:
             raise ValueError(
                 "`add_bin_width_to_ylabel` should be called after plotting, since bins "
                 "are calculated during plotting."
             )
 
         bin_width = abs(self.bins[1] - self.bins[0])
```

### Comparing `puma-hep-0.2.4/puma/hlplots/results.py` & `puma-hep-0.2.5/puma/hlplots/results.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,46 @@
 """Results module for high level API."""
 from __future__ import annotations
 
 from dataclasses import dataclass, field
+from pathlib import Path
 
 import numpy as np
 from ftag import Cuts, Flavour, Flavours
 from ftag.hdf5 import H5Reader
 
-from puma import Histogram, HistogramPlot, Roc, RocPlot, VarVsEff, VarVsEffPlot
-from puma.metrics import calc_rej
+import puma.fraction_scan as fraction_scan
+from puma import (
+    Histogram,
+    HistogramPlot,
+    Line2D,
+    Line2DPlot,
+    Roc,
+    RocPlot,
+    VarVsEff,
+    VarVsEffPlot,
+)
+from puma.metrics import calc_eff, calc_rej
 from puma.utils import get_good_linestyles
 
 
 @dataclass
 class Results:
     """Store information about several taggers and plot results."""
 
-    signal: Flavour | str = Flavours.bjets
+    signal: Flavour | str
+    sample: str
     backgrounds: list = field(init=False)
     atlas_first_tag: str = "Simulation Internal"
     atlas_second_tag: str = None
     taggers: dict = field(default_factory=dict)
     sig_eff: float = None
     perf_var: str = "pt"
+    output_dir: str | Path = "."
+    extension: str = "png"
 
     def __post_init__(self):
         if isinstance(self.signal, str):
             self.signal = Flavours[self.signal]
         if self.signal == Flavours.bjets:
             self.backgrounds = [Flavours.cjets, Flavours.ujets]
         elif self.signal == Flavours.cjets:
@@ -34,14 +48,17 @@
         elif self.signal == Flavours.hbb:
             self.backgrounds = [Flavours.hcc, Flavours.top, Flavours.qcd]
         elif self.signal == Flavours.hcc:
             self.backgrounds = [Flavours.hbb, Flavours.top, Flavours.qcd]
         else:
             raise ValueError(f"Unsupported signal class {self.signal}.")
 
+        if isinstance(self.output_dir, str):
+            self.output_dir = Path(self.output_dir)
+
     @property
     def flavours(self):
         """Return a list of all flavours.
 
         Returns
         -------
         list
@@ -143,25 +160,106 @@
         Returns
         -------
         Tagger
             Instance of the puma.hlplots.Tagger class, containing tagger information.
         """
         return self.taggers[tagger_name]
 
+    def get_filename(self, plot_name: str, suffix: str = None):
+        """Get output name.
+
+        Parameters
+        ----------
+        plot_name : str
+            plot name
+        suffix : str, optional
+            suffix to add to output name, by default None
+
+        Returns
+        -------
+        str
+            output name
+        """
+        base = f"{self.sample}_{self.signal}_{plot_name}"
+        if suffix is not None:
+            base += f"_{suffix}"
+        return Path(self.output_dir / base).with_suffix(f".{self.extension}")
+
+    def plot_discs(
+        self,
+        suffix: str = None,
+        exclude_tagger: list = None,
+        xlabel: str = None,
+        **kwargs,
+    ):
+        """Plot discriminant distributions.
+
+        Parameters
+        ----------
+        suffix : str, optional
+            Suffix to add to output file name, by default None
+        exclude_tagger : list, optional
+            List of taggers to be excluded from this plot, by default None
+        xlabel : str, optional
+            x-axis label, by default "$D_{b}$"
+        **kwargs : kwargs
+            key word arguments for `puma.HistogramPlot`
+        """
+        if xlabel is None:
+            xlabel = rf"$D_{{{self.signal.name.rstrip('jets')}}}$"
+
+        line_styles = get_good_linestyles()
+
+        tagger_output_plot = HistogramPlot(
+            n_ratio_panels=0,
+            xlabel=xlabel,
+            ylabel="Normalised number of jets",
+            figsize=(7.0, 4.5),
+            atlas_first_tag=self.atlas_first_tag,
+            atlas_second_tag=self.atlas_second_tag,
+            **kwargs,
+        )
+        tag_i = 0
+        tag_labels = []
+        for tagger in self.taggers.values():
+            if exclude_tagger is not None and tagger.name in exclude_tagger:
+                continue
+            discs = tagger.discriminant(self.signal)
+            for flav in self.flavours:
+                tagger_output_plot.add(
+                    Histogram(
+                        discs[tagger.is_flav(flav)],
+                        ratio_group=flav,
+                        label=flav.label if tag_i == 0 else None,
+                        colour=flav.colour,
+                        linestyle=line_styles[tag_i],
+                    ),
+                    reference=tagger.reference,
+                )
+            tag_i += 1
+            tag_labels.append(tagger.label if tagger.label else tagger.name)
+        tagger_output_plot.draw()
+        tagger_output_plot.make_linestyle_legend(
+            linestyles=line_styles[:tag_i],
+            labels=tag_labels,
+            bbox_to_anchor=(0.55, 1),
+        )
+        tagger_output_plot.savefig(self.get_filename("disc", suffix))
+
     def plot_rocs(
         self,
-        plot_name: str,
+        suffix: str = None,
         args_roc_plot: dict = None,
     ):
-        """Plots rocs
+        """Plots rocs.
 
         Parameters
         ----------
-        plot_name : puma.RocPlot
-            roc plot object
+        suffix : str, optional
+            suffix to add to output file name, by default None
         args_roc_plot: dict, optional
             key word arguments being passed to `RocPlot`
         """
         roc_plot_args = {
             "n_ratio_panels": len(self.backgrounds),
             "ylabel": "Background rejection",
             "xlabel": self.signal.eff_str,
@@ -171,15 +269,15 @@
         }
         # TODO: update in python 3.9
         if args_roc_plot is not None:
             roc_plot_args.update(args_roc_plot)
         plot_roc = RocPlot(**roc_plot_args)
 
         for tagger in self.taggers.values():
-            discs = tagger.get_disc(self.signal)
+            discs = tagger.discriminant(self.signal)
             for background in self.backgrounds:
                 rej = calc_rej(
                     discs[tagger.is_flav(self.signal)],
                     discs[tagger.is_flav(background)],
                     self.sig_eff,
                 )
                 plot_roc.add_roc(
@@ -196,39 +294,37 @@
                 )
 
         # setting which flavour rejection ratio is drawn in which ratio panel
         for i, background in enumerate(self.backgrounds):
             plot_roc.set_ratio_class(i + 1, background)
 
         plot_roc.draw()
+        plot_name = self.get_filename("roc", suffix)
         plot_roc.savefig(plot_name)
 
     def plot_var_perf(  # pylint: disable=too-many-locals
         self,
-        plot_name: str,
+        suffix: str = None,
         xlabel: str = r"$p_{T}$ [GeV]",
         h_line: float = None,
-        ext: str = "png",
         **kwargs,
     ):
         """Variable vs efficiency/rejection plot.
 
         You can choose between different modes: "sig_eff", "bkg_eff", "sig_rej",
         "bkg_rej"
 
         Parameters
         ----------
-        plot_name : str
-            plot name base
+        suffix : str, optional
+            suffix to add to output file name, by default None
         xlabel : regexp, optional
             _description_, by default "$p_{T}$ [GeV]"
         h_line : float, optional
             draws a horizonatal line in the signal efficiency plot
-        ext : str, optional
-            changes the extension of the save plot
         **kwargs : kwargs
             key word arguments for `puma.VarVsEff`
         """
         # define the curves
         plot_sig_eff = VarVsEffPlot(
             mode="sig_eff",
             ylabel=self.signal.eff_str,
@@ -258,15 +354,15 @@
         working_point_in_kwargs = "working_point" in kwargs
         for tagger in self.taggers.values():
             if not disc_cut_in_kwargs:
                 kwargs["disc_cut"] = tagger.disc_cut
             if not working_point_in_kwargs:
                 kwargs["working_point"] = tagger.working_point
 
-            discs = tagger.get_disc(self.signal)
+            discs = tagger.discriminant(self.signal)
             is_signal = tagger.is_flav(self.signal)
             plot_sig_eff.add(
                 VarVsEff(
                     x_var_sig=tagger.perf_var[is_signal],
                     disc_sig=discs[is_signal],
                     label=tagger.label,
                     colour=tagger.colour,
@@ -288,73 +384,88 @@
                     ),
                     reference=tagger.reference,
                 )
 
         plot_sig_eff.draw()
         if h_line:
             plot_sig_eff.draw_hline(h_line)
-        plot_sig_eff.savefig(f"{plot_name}_{self.signal}_eff.{ext}")
+
+        plot_base = "profile_flat" if kwargs.get("fixed_eff_bin") else "profile_fixed"
+        plot_suffix = f"{self.signal}_eff_{suffix}" if suffix else f"{self.signal}_eff"
+        plot_sig_eff.savefig(self.get_filename(plot_base, plot_suffix))
         for i, background in enumerate(self.backgrounds):
             plot_bkg[i].draw()
-            plot_bkg[i].savefig(f"{plot_name}_{background}_rej.{ext}")
+            plot_suffix = (
+                f"{background}_rej_{suffix}" if suffix else f"{background}_rej"
+            )
+            plot_bkg[i].savefig(self.get_filename(plot_base, plot_suffix))
 
-    def plot_discs(
-        self,
-        plot_name: str,
-        exclude_tagger: list = None,
-        xlabel: str = None,
-        **kwargs,
+    def plot_fraction_scans(
+        self, suffix: str = None, efficiency: float = 0.7, rej: bool = False
     ):
-        """Plots discriminant
-
+        """Produce fraction scan (fc/fb) iso-efficiency plots.
 
         Parameters
         ----------
-        plot_name : _type_
-            Name of the plot.
-        exclude_tagger : list, optional
-            List of taggers to be excluded from this plot, by default None
-        xlabel : str, optional
-            x-axis label, by default "$D_{b}$"
-        **kwargs : kwargs
-            key word arguments for `puma.HistogramPlot`
+        suffix : str, optional
+            suffix to add to output file name, by default None
+        efficiency : float, optional
+            signal efficiency, by default 0.7
+        rej : bool, optional
+            if True, plot rejection instead of efficiency, by default False
         """
-        if xlabel is None:
-            xlabel = rf"$D_{{{self.signal.name.rstrip('jets')}}}$"
+        if self.signal not in (Flavours.bjets, Flavours.cjets):
+            raise ValueError("Signal flavour must be bjets or cjets")
+        if len(self.backgrounds) != 2:
+            raise ValueError("Only two background flavours are supported")
+
+        fxs = fraction_scan.get_fx_values()
+        plot = Line2DPlot(atlas_second_tag=self.atlas_second_tag)
+        eff_or_rej = calc_eff if not rej else calc_rej
 
-        line_styles = get_good_linestyles()
-
-        tagger_output_plot = HistogramPlot(
-            n_ratio_panels=0,
-            xlabel=xlabel,
-            ylabel="Normalised number of jets",
-            figsize=(7.0, 4.5),
-            atlas_first_tag=self.atlas_first_tag,
-            atlas_second_tag=self.atlas_second_tag,
-            **kwargs,
-        )
-        tag_i = 0
-        tag_labels = []
         for tagger in self.taggers.values():
-            if exclude_tagger is not None and tagger.name in exclude_tagger:
-                continue
-            discs = tagger.get_disc(self.signal)
-            for flav in self.flavours:
-                tagger_output_plot.add(
-                    Histogram(
-                        discs[tagger.is_flav(flav)],
-                        ratio_group=flav,
-                        label=flav.label if tag_i == 0 else None,
-                        colour=flav.colour,
-                        linestyle=line_styles[tag_i],
-                    ),
-                    reference=tagger.reference,
+            xs = []
+            ys = []
+            for fx in fxs:
+                sig_idx = tagger.is_flav(self.signal)
+                disc = tagger.discriminant(self.signal, fx=fx)
+                bkg_idx = tagger.is_flav(self.backgrounds[0])
+                xs.append(eff_or_rej(disc[sig_idx], disc[bkg_idx], efficiency))
+                bkg_idx = tagger.is_flav(self.backgrounds[1])
+                ys.append(eff_or_rej(disc[sig_idx], disc[bkg_idx], efficiency))
+
+            # add curve for this tagger
+            tagger_fx = tagger.f_c if self.signal == Flavours.bjets else tagger.f_b
+            plot.add(
+                Line2D(
+                    x_values=xs,
+                    y_values=ys,
+                    label=f"{tagger.label} ($f_x={tagger_fx}$)",
+                    colour=tagger.colour,
                 )
-            tag_i += 1
-            tag_labels.append(tagger.label if tagger.label else tagger.name)
-        tagger_output_plot.draw()
-        tagger_output_plot.make_linestyle_legend(
-            linestyles=line_styles[:tag_i],
-            labels=tag_labels,
-            bbox_to_anchor=(0.55, 1),
-        )
-        tagger_output_plot.savefig(plot_name)
+            )
+
+            # Add a marker for the just added fraction scan
+            # The is_marker bool tells the plot that this is a marker and not a line
+            fx_idx = np.argmin(np.abs(fxs - tagger_fx))
+            plot.add(
+                Line2D(
+                    x_values=xs[fx_idx],
+                    y_values=ys[fx_idx],
+                    marker="x",
+                    markersize=15,
+                    markeredgewidth=2,
+                ),
+                is_marker=True,
+            )
+
+            # Adding labels
+            if not rej:
+                plot.xlabel = self.backgrounds[0].eff_str
+                plot.ylabel = self.backgrounds[1].eff_str
+            else:
+                plot.xlabel = self.backgrounds[0].rej_str
+                plot.ylabel = self.backgrounds[1].rej_str
+
+            # Draw and save the plot
+            plot.draw()
+            plot.savefig(self.get_filename("fraction_scan", suffix))
```

### Comparing `puma-hep-0.2.4/puma/hlplots/tagger.py` & `puma-hep-0.2.5/puma/hlplots/tagger.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 
 import h5py
 import numpy as np
 import pandas as pd
-from ftag import Flavour, Flavours
-from numpy.lib.recfunctions import structured_to_unstructured
+from ftag import Flavour, Flavours, get_discriminant
 
-from puma.utils import calc_disc, logger
+from puma.utils import logger
 
 
 @dataclass
-class Tagger:  # pylint: disable=too-many-instance-attributes
+class Tagger:
     """Class storing information and results for a tagger."""
 
+    # commonly passed to the constructor
     name: str
     label: str = None
     reference: bool = False
+    colour: str = None
 
-    scores = None
-    labels = None
-    perf_var = None
+    # commonly set by the Results class
+    scores: np.ndarray = None
+    labels: np.ndarray = None
+    perf_var: np.ndarray = None
     output_nodes: list = field(
         default_factory=lambda: [Flavours.ujets, Flavours.cjets, Flavours.bjets]
     )
 
-    colour: str = None
-
     disc_cut: float = None
     working_point: float = None
     f_c: float = None
     f_b: float = None
 
     def __post_init__(self):
         if self.label is None:
@@ -54,25 +54,14 @@
         np.ndarray
             Array of indices of the given flavour
         """
         flavour = Flavours[flavour] if isinstance(flavour, str) else flavour
         return flavour.cuts(self.labels).idx
 
     @property
-    def output_nodes_lower(self):
-        """Return the lowercase output nodes.
-
-        Returns
-        -------
-        list
-            List of lower case output nodes
-        """
-        return [x.name.lower() for x in self.output_nodes]
-
-    @property
     def probabilities(self):
         """Return the probabilities of the tagger.
 
         Returns
         -------
         list
             List of probability names
@@ -84,15 +73,14 @@
         """Return a list of the outputs of the tagger.
 
         Returns
         -------
         list
             List of the outputs variable names of the tagger
         """
-
         return [f"{self.name}_{prob}" for prob in self.probabilities]
 
     def extract_tagger_scores(
         self, source: object, source_type: str = "data_frame", key: str = None
     ):
         """Extract tagger scores from data frame or file.
 
@@ -114,49 +102,46 @@
         Raises
         ------
         ValueError
             if source_type is wrongly specified
         """
         if source_type == "data_frame":
             logger.debug("Retrieving tagger `%s` from data frame.", self.name)
-            self.scores = source[self.variables].values
+            self.scores = source[self.variables]
             return
         if source_type == "structured_array":
             logger.debug(
                 "Retrieving tagger %s from h5py fields %s.",
                 self.name,
                 source,
             )
-            self.scores = structured_to_unstructured(source[self.variables])
-            self.scores = self.scores.astype("float32")
+            self.scores = source[self.variables]
             return
         if key is None:
             raise ValueError(
-                "When using a `source_type` other than `data_frame`, you need to "
-                "specify the `key`."
+                "When using a `source_type` other than `data_frame`, you need to"
+                " specify the `key`."
             )
         if source_type == "data_frame_path":
             logger.debug(
                 "Retrieving tagger %s in data frame from file %s.",
                 self.name,
                 source,
             )
             df_in = pd.read_hdf(source, key=key)
-            self.scores = df_in[self.variables].values
+            self.scores = df_in[self.variables]
 
         elif source_type == "h5_file":
             logger.debug(
                 "Retrieving tagger %s from structured h5 file %s.",
                 self.name,
                 source,
             )
             with h5py.File(source, "r") as f_h5:
-                self.scores = structured_to_unstructured(
-                    f_h5[key].fields(self.variables)[:]
-                )
+                self.scores = f_h5[key].fields(self.variables)[:]
 
         else:
             raise ValueError(f"{source_type} is not a valid value for `source_type`.")
 
     def n_jets(self, flavour: Flavour | str):
         """Retrieve number of jets of a given flavour.
 
@@ -169,86 +154,38 @@
         -------
         int
             Number of jets of given flavour
         """
         flavour = Flavours[flavour] if isinstance(flavour, str) else flavour
         return len(flavour.cuts(self.labels).values)
 
-    def get_disc(self, signal_class: Flavour):
+    def discriminant(self, signal: Flavour, fx: float = None):
         """Retrieve the discriminant for a given signal class.
 
         Parameters
         ----------
-        signal_class : str
+        signal : Flavour
             Signal class for which the discriminant should be retrieved
+        fx : float, optional
+            fc or fb value, by default None
 
         Returns
         -------
         np.ndarray
             Discriminant for given signal class
 
         Raises
         ------
         ValueError
             If no discriminant is defined for given signal class
         """
-        if signal_class == Flavours.bjets:
-            return self.calc_disc_b()
-        if signal_class == Flavours.cjets:
-            return self.calc_disc_c()
-        if signal_class in (Flavours.hbb, Flavours.hcc):
-            return self.scores[:, self.output_nodes_lower.index(signal_class.name)]
-        raise ValueError(f"No discriminant defined for {signal_class} signal.")
-
-    def calc_disc_b(self) -> np.ndarray:
-        """Calculate b-tagging discriminant
-
-        Returns
-        -------
-        np.ndarray
-            b-tagging discriminant
-
-        Raises
-        ------
-        ValueError
-            if f_c parameter is not specified for tagger
-        """
-        if self.f_c is None:
-            raise ValueError(
-                "Before calculating the b-tagging discriminant, specify `f_c`"
-            )
-        flv_map = {
-            "sig": {"pb": 1.0},
-            "bkg": {"pu": 1 - self.f_c, "pc": self.f_c},
-        }
-        return calc_disc(
-            scores=self.scores,
-            flvs=self.probabilities,
-            flv_map=flv_map,
-        )
-
-    def calc_disc_c(self) -> np.ndarray:
-        """Calculate c-tagging discriminant
-
-        Returns
-        -------
-        np.ndarray
-            c-tagging discriminant
-
-        Raises
-        ------
-        ValueError
-            if f_b parameter is not specified for tagger
-        """
-        if self.f_b is None:
-            raise ValueError(
-                "Before calculating the c-tagging discriminant, specify `f_b`"
-            )
-        flv_map = {
-            "sig": {"pc": 1.0},
-            "bkg": {"pu": 1 - self.f_b, "pb": self.f_b},
-        }
-        return calc_disc(
-            scores=self.scores,
-            flvs=self.probabilities,
-            flv_map=flv_map,
-        )
+        if fx is not None and signal not in (Flavours.bjets, Flavours.cjets):
+            raise ValueError("fx only valid for bjets and cjets.")
+        if fx is None:
+            fx = self.f_c if Flavours[signal] == Flavours.bjets else self.f_b
+        if Flavours[signal] == Flavours.bjets:
+            return get_discriminant(self.scores, self.name, signal, fx)
+        if Flavours[signal] == Flavours.cjets:
+            return get_discriminant(self.scores, self.name, signal, fx)
+        if Flavours[signal] in (Flavours.hbb, Flavours.hcc):
+            return self.scores[signal.px]
+        raise ValueError(f"No discriminant defined for {signal} signal.")
```

### Comparing `puma-hep-0.2.4/puma/line_plot_2d.py` & `puma-hep-0.2.5/puma/line_plot_2d.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Classes for 2D line plots."""
 import matplotlib as mpl
 import numpy as np
 import pandas as pd
 
 from puma.plot_base import PlotBase, PlotLineObject
-from puma.utils import get_good_colours, logger
+from puma.utils import get_good_colours, get_good_markers, logger
 
 
-class Line2D(PlotLineObject):  # pylint: disable=too-few-public-methods
+class Line2D(PlotLineObject):
     """Line2D class storing info about the x and y values and style."""
 
     def __init__(
         self,
         x_values: np.ndarray,
         y_values: np.ndarray,
         **kwargs,
@@ -37,15 +37,14 @@
             If provided y_values array is empty.
         ValueError
             If provided x_values and y_values arrays have different
             shapes.
         ValueError
             If an invalid type was given for x_values
         """
-
         super().__init__(**kwargs)
 
         # Check input dtype
         if isinstance(x_values, (np.ndarray, list, int, float, pd.Series)):
             if type(x_values) != type(y_values):  # pylint: disable=C0123
                 raise ValueError(
                     "Invalid types of input given! Both must be one of the following: "
@@ -77,16 +76,16 @@
                 raise ValueError(
                     "x_values and y_values have different dimensionalities! "
                     f"x_values: {len(x_values)}, y_values: {len(y_values)}"
                 )
 
         else:
             raise ValueError(
-                "Invalid type of input data. Allowed values are "
-                "numpy.ndarray, list, int, float"
+                "Invalid type of input data. Allowed values are numpy.ndarray, list,"
+                " int, float"
             )
 
         # Set inputs as attributes
         self.x_values = x_values
         self.y_values = y_values
 
         # Set key to None. Will be defined when plotting starts
@@ -98,26 +97,25 @@
 
     def __init__(
         self,
         logy: bool = False,
         grid: bool = True,
         **kwargs,
     ) -> None:
-        """Plot properties
+        """Plot properties.
 
         Parameters
         ----------
         logy : bool, optional
             Decide, if the y-axis of the plot will be in log, by default False
         grid : bool, optional
             Set the grid for the plots.
         **kwargs : kwargs
             Keyword arguments from `puma.PlotObject`
         """
-
         super().__init__(grid=grid, **kwargs)
 
         # Set inputs as attributes
         self.logy = logy
 
         # Init needed lists and dicts
         self.plot_objects = {}
@@ -143,15 +141,14 @@
             Defines if this is a marker (True) or a line (False). By default False.
 
         Raises
         ------
         KeyError
             If unique identifier key is used twice
         """
-
         # If key not defined, set it to a numerical value
         if key is None:
             key = len(self.plot_objects) + 1
 
         # Check that key is not double used
         if key in self.plot_objects:
             raise KeyError(f"Duplicated key {key} already used for unique identifier.")
@@ -179,15 +176,15 @@
         else:
             curve.is_marker = True
             # Set colour of the marker the same as the last line plotted
             if curve.colour is None:
                 curve.colour = self.plot_objects[len(self.plot_objects)].colour
             # Set markerstyle
             if curve.marker is None:
-                curve.marker = "x"
+                curve.marker = get_good_markers()[len(self.plot_objects)]
             # Set markersize
             if curve.markersize is None:
                 curve.markersize = 15
             # Set markersize
             if curve.markeredgewidth is None:
                 curve.markeredgewidth = 2
             # Set the linestyle for markers to None as string
@@ -244,15 +241,14 @@
             )
 
         self.plotting_done = True
         return plt_handles
 
     def draw(self):
         """Draw figure."""
-
         plt_handles = self.plot()
 
         # Make the legend
         self.make_legend(plt_handles, ax_mpl=self.axis_top)
 
         self.set_title()
         self.set_log()
```

### Comparing `puma-hep-0.2.4/puma/metrics.py` & `puma-hep-0.2.5/puma/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 def calc_eff(
     sig_disc: np.ndarray,
     bkg_disc: np.ndarray,
     target_eff,
     return_cuts: bool = False,
 ):
-    """Calculate efficiency
+    """Calculate efficiency.
 
     Parameters
     ----------
     sig_disc : np.ndarray
         Signal discriminant
     bkg_disc : np.ndarray
         Background discriminant
@@ -57,15 +57,15 @@
 
 def calc_rej(
     sig_disc: np.ndarray,
     bkg_disc: np.ndarray,
     target_eff,
     return_cuts: bool = False,
 ):
-    """Calculate efficiency
+    """Calculate efficiency.
 
     Parameters
     ----------
     sig_disc : np.ndarray
         Signal discriminant
     bkg_disc : np.ndarray
         Background discriminant
@@ -230,15 +230,14 @@
     numpy.ndarray
         Bins height of histogram a (only returned if `return_hist` is True)
     numpy.ndarray
         Bins height of histogram b (only returned if `return_hist` is True)
     numpy.ndarray
         Bin edges of the two histograms (only returned if `return_hist` is True)
     """
-
     _, bin_edges = np.histogram(
         np.hstack([values_a, values_b]), bins=bins, range=bins_range
     )
 
     _, hist_a, unc_a, _ = hist_w_unc(values_a, bin_edges)
     _, hist_b, unc_b, _ = hist_w_unc(values_b, bin_edges)
```

### Comparing `puma-hep-0.2.4/puma/pie.py` & `puma-hep-0.2.5/puma/pie.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 """Pie plot functions."""
 import matplotlib as mpl
 
 from puma.plot_base import PlotBase
 from puma.utils import get_good_pie_colours, logger
 
 
-class PiePlot(
-    PlotBase
-):  # pylint: disable=too-few-public-methods,too-many-instance-attributes
-    """Pie plot class"""
+class PiePlot(PlotBase):
+    """Pie plot class."""
 
-    def __init__(  # pylint: disable=too-many-arguments
+    def __init__(
         self,
         wedge_sizes,
         colours: list = None,
         colour_scheme: str = None,
         labels: list = None,
         draw_legend: bool = False,
         mpl_pie_kwargs: dict = None,
         **kwargs,
     ):
-        """Initialise the pie plot
+        """Initialise the pie plot.
 
         Parameters
         ----------
         wedge_sizes : 1D array like
             The size of the wedges. Will be translated into the fractions automatically.
             So they don't have to add up to 1 or 100. The fractional area of each
             wedge is given by x/sum(x).
@@ -75,16 +73,15 @@
 
         self.initialise_figure()
         self.plot()
 
     def plot(
         self,
     ):
-        """Plot the pie chart"""
-
+        """Plot the pie chart."""
         self.axis_top.pie(
             x=self.wedge_sizes,
             labels=None if self.draw_legend else self.labels,
             colors=self.colours,
             **self.mpl_pie_kwargs,
         )
```

### Comparing `puma-hep-0.2.4/puma/plot_base.py` & `puma-hep-0.2.5/puma/plot_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 atlasify.LINE_SPACING = 1.3  # overwrite the default, which is 1.2
 
 
 # TODO: enable `kw_only` when switching to Python 3.10
 # @dataclass(kw_only=True)
 @dataclass
-class PlotLineObject:  # pylint: disable=too-many-instance-attributes
+class PlotLineObject:
     """Base data class defining properties of a plot object.
 
     Parameters
     ----------
     xmin : float, optional
         Minimum value of the x-axis, by default None
     xmax : float, optional
@@ -55,15 +55,15 @@
     markeredgewidth: int = None
     is_marker: bool = None
 
 
 # TODO: enable `kw_only` when switching to Python 3.10
 # @dataclass(kw_only=True)
 @dataclass
-class PlotObject:  # pylint: disable=too-many-instance-attributes
+class PlotObject:
     """Data base class defining properties of a plot object.
 
     Parameters
     ----------
     title : str, optional
         Title of the plot, by default ""
     draw_errors : bool, optional
@@ -205,31 +205,38 @@
         self.__check_figsize()
         allowed_n_ratio_panels = [0, 1, 2, 3]
         if self.n_ratio_panels not in allowed_n_ratio_panels:
             raise ValueError(
                 f"{self.n_ratio_panels} not allwed value for `n_ratio_panels`. "
                 f"Allowed are {allowed_n_ratio_panels}"
             )
-        self.ymin_ratio = [None] * self.n_ratio_panels
-        self.ymax_ratio = [None] * self.n_ratio_panels
+        self.__check_yratio(self.ymin_ratio)
+        self.ymin_ratio = (
+            [None] * self.n_ratio_panels if self.ymin_ratio is None else self.ymin_ratio
+        )
+        self.__check_yratio(self.ymax_ratio)
+        self.ymax_ratio = (
+            [None] * self.n_ratio_panels if self.ymax_ratio is None else self.ymax_ratio
+        )
+
         self.ylabel_ratio = ["Ratio"] * self.n_ratio_panels
         if self.leg_fontsize is None:
             self.leg_fontsize = self.fontsize
         if self.atlas_fontsize is None:
             self.atlas_fontsize = self.fontsize
         if self.apply_atlas_style is False and (
             self.atlas_first_tag is not None or self.atlas_second_tag is not None
         ):
             logger.warning(
                 "You specified an ATLAS tag, but `apply_atlas_style` is set to false. "
                 "Tag will therefore not be shown on plot."
             )
 
     def __check_figsize(self):
-        """Check `figsize`
+        """Check `figsize`.
 
         Raises
         ------
         ValueError
             If shape of `figsize` is not a tuple or list with length 2
         """
         if self.figsize is None:
@@ -238,20 +245,41 @@
             self.figsize = tuple(self.figsize)
         elif not isinstance(self.figsize, tuple) or len(self.figsize) != 2:
             raise ValueError(
                 f"You passed `figsize` as {self.figsize} which is not allowed. "
                 "Either a tuple or a list of size 2 is allowed"
             )
 
+    def __check_yratio(self, yratio):
+        """Check `yratio`.
+
+        Parameters
+        ----------
+        yratio : list
+            List of min or max limits of ratio plots
+        Raises
+        ------
+        ValueError
+            If `yratio` is not a list and it's lenght
+            is not equal to number of ratio panels
+        """
+        if yratio is None:
+            return
+        if not isinstance(yratio, (list, tuple)) or len(yratio) != self.n_ratio_panels:
+            raise ValueError(
+                f"You passed `min/max_yratio` as {yratio} which is not allowed. "
+                f"Either a tuple or a list of size {self.n_ratio_panels} is allowed"
+            )
 
-class PlotBase(PlotObject):  # pylint: disable=too-many-instance-attributes
-    """Base class for plotting"""
+
+class PlotBase(PlotObject):
+    """Base class for plotting."""
 
     def __init__(self, **kwargs) -> None:
-        """Initialise class
+        """Initialise class.
 
         Parameters
         ----------
         **kwargs : kwargs
             Keyword arguments from `puma.PlotObject`
         """
         super().__init__(**kwargs)
@@ -319,16 +347,16 @@
         self,
         vlines_xvalues: list,
         vlines_label_list: list = None,
         vlines_line_height_list: list = None,
         same_height: bool = False,
         colour: str = "#000000",
         fontsize: int = 10,
-    ):  # pylint: disable=too-many-arguments
-        """Drawing working points in plot
+    ):
+        """Drawing working points in plot.
 
         Parameters
         ----------
         vlines_xvalues : list
             List of working points x values to draw
         vlines_label_list : list, optional
             List with labels for the vertical lines. Must be the same
@@ -399,15 +427,14 @@
         Parameters
         ----------
         force_x : bool, optional
             Forcing log on x-axis even if `logx` attribute is False, by default False
         force_y : bool, optional
             Forcing log on y-axis even if `logy` attribute is False, by default False
         """
-
         if self.logx or force_x:
             if not self.logx:
                 logger.warning(
                     "Setting log of x-axis but `logx` flag was set to False."
                 )
 
             # Set log scale for all plots
@@ -511,15 +538,15 @@
             self.axis_top.tick_params(axis="x", labelsize=labelsize, **kwargs)
         for i, ratio_axis in enumerate(self.ratio_axes):
             ratio_axis.tick_params(axis="y", labelsize=labelsize, **kwargs)
             if i == self.n_ratio_panels - 1:
                 ratio_axis.tick_params(axis="x", labelsize=labelsize, **kwargs)
 
     def set_xlim(self, xmin: float = None, xmax: float = None, **kwargs):
-        """Set limits of x-axis
+        """Set limits of x-axis.
 
         Parameters
         ----------
         xmin : float, optional
             Min of x-axis, by default None
         xmax : float, optional
             Max of x-axis, by default None
@@ -557,40 +584,39 @@
             plot_name,
             transparent=self.transparent if transparent is None else transparent,
             dpi=self.dpi if dpi is None else dpi,
             **kwargs,
         )
 
     def atlasify(self, use_tag: bool = True, force: bool = False):
-        """Apply ATLAS style to all axes using the atlasify package
+        """Apply ATLAS style to all axes using the atlasify package.
 
         Parameters
         ----------
         use_tag : bool, optional
             If False, ATLAS style will be applied but no tag will be put on the plot.
             If True, the tag will be put on as well, by default True
         force : bool, optional
             Force ATLAS style also if class variable is False, by default False
         """
-
         if self.plotting_done is False and force is False:
             logger.warning(
                 "`atlasify()` has to be called after plotting --> "
                 "ATLAS style will not be adapted. If you want to do it anyway, "
                 "you can use `force`."
             )
             return
 
         if self.apply_atlas_style or force:
             logger.debug("Initialise ATLAS style using atlasify.")
             if use_tag is True:
                 # TODO: for some reason, pylint complains about the used arguments
                 # when calling atlasify ("unexpected-keyword-arg") error
                 # --> fix this
-                atlasify.atlasify(  # pylint: disable=E1123
+                atlasify.atlasify(
                     atlas=self.atlas_first_tag,
                     subtext=self.atlas_second_tag,
                     axes=self.axis_top,
                     font_size=self.atlas_fontsize,
                     label_font_size=self.atlas_fontsize,
                     sub_font_size=self.atlas_fontsize,
                     offset=self.atlas_vertical_offset,
@@ -605,16 +631,16 @@
             for ratio_axis in self.ratio_axes:
                 atlasify.atlasify(atlas=False, axes=ratio_axis, enlarge=1)
             if self.vertical_split:
                 atlasify.atlasify(atlas=False, axes=self.axis_leg, enlarge=1)
             if force:
                 if self.apply_atlas_style is False:
                     logger.warning(
-                        "Initialising ATLAS style even though `apply_atlas_style` is  "
-                        "set to False."
+                        "Initialising ATLAS style even though `apply_atlas_style` is "
+                        " set to False."
                     )
                 if self.plotting_done is False:
                     logger.warning(
                         "Initialising ATLAS style even though `plotting_done` is set to"
                         " False."
                     )
 
@@ -654,15 +680,15 @@
     def make_linestyle_legend(
         self,
         linestyles: list,
         labels: list,
         loc: str = None,
         bbox_to_anchor: tuple = None,
         axis_for_legend=None,
-    ):  # pylint: disable=too-many-arguments
+    ):
         """Create a legend to indicate what different linestyles correspond to.
 
         Parameters
         ----------
         linestyles : list
             List of the linestyles to draw in the legend
         labels : list
@@ -672,15 +698,14 @@
             Location of the legend (matplotlib supported locations), by default None
         bbox_to_anchor : tuple, optional
             Allows to specify the precise position of this legend. Either a 2-tuple
             (x, y) or a 4-tuple (x, y, width, height), by default None
         axis_for_legend : matplotlib.Axes.axis, optional
             Axis on which to draw the legend, by default None
         """
-
         if axis_for_legend is None:
             axis_for_legend = self.axis_top
 
         lines_list = []
         for linestyle, label in zip(linestyles, labels):
             lines_list.append(
                 lines.Line2D(
@@ -699,15 +724,15 @@
             fontsize=self.leg_fontsize,
             bbox_to_anchor=bbox_to_anchor,
             frameon=False,
         )
         axis_for_legend.add_artist(linestyle_legend)
 
     def set_ratio_label(self, ratio_panel: int, label: str):
-        """Associate the rejection class to a ratio panel
+        """Associate the rejection class to a ratio panel.
 
         Parameters
         ----------
         ratio_panel : int
             Indicates which ratio panel to modify (either 1 or 2).
         label : str
             y-axis label of the ratio panel
@@ -721,15 +746,15 @@
         if self.n_ratio_panels < ratio_panel and ratio_panel not in [1, 2]:
             raise ValueError(
                 "Requested ratio panels and given ratio_panel do not match."
             )
         self.ylabel_ratio[ratio_panel - 1] = label
 
     def initialise_plot(self):
-        """Calls other methods which are usually used when plotting"""
+        """Calls other methods which are usually used when plotting."""
         self.set_title()
         self.set_log()
         self.set_y_lim()
         self.set_xlabel()
         self.set_ylabel(self.axis_top)
         self.set_tick_params()
         self.plotting_done = True
```

### Comparing `puma-hep-0.2.4/puma/roc.py` & `puma-hep-0.2.5/puma/roc.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,17 @@
 
 from puma.metrics import rej_err
 from puma.plot_base import PlotBase, PlotLineObject
 from puma.utils import get_good_colours, get_good_linestyles, logger
 
 
 class Roc(PlotLineObject):
-    """
-    ROC class storing info about curve and allows to calculate ratio w.r.t other roc.
-    """
+    """Represent a single ROC curve and allows to calculate ratio w.r.t other ROCs."""
 
-    def __init__(  # pylint: disable=too-many-arguments
+    def __init__(
         self,
         sig_eff: np.ndarray,
         bkg_rej: np.ndarray,
         n_test: int = None,
         rej_class: str | Flavour = None,
         signal_class: str = None,
         key: str = None,
@@ -153,15 +151,15 @@
         pchip
             Interpolation function
         """
         return pchip(self.sig_eff, self.bkg_rej)
 
     @property
     def non_zero_mask(self):
-        """Masking points where rejection is 0 and no signal efficiency change present
+        """Masking points where rejection is 0 and no signal efficiency change present.
 
         Returns
         -------
         numpy.array
             Masked indices
         """
         # Mask the points where there was no change in the signal eff
@@ -173,31 +171,31 @@
             nonzero = nonzero & (self.sig_eff >= self.xmin)
         if self.xmax is not None:
             nonzero = nonzero & (self.sig_eff <= self.xmax)
         return nonzero
 
     @property
     def non_zero(self):
-        """Abstraction of `non_zero_mask`
+        """Abstraction of `non_zero_mask`.
 
         Returns
         -------
         numpy.array
             Masked signal efficiency
         numpy.array
             Masked background rejection
         """
         return self.sig_eff[self.non_zero_mask], self.bkg_rej[self.non_zero_mask]
 
 
-class RocPlot(PlotBase):  # pylint: disable=too-many-instance-attributes
-    """ROC plot class"""
+class RocPlot(PlotBase):
+    """ROC plot class."""
 
     def __init__(self, grid: bool = True, **kwargs) -> None:
-        """ROC plot properties
+        """ROC plot properties.
 
         Parameters
         ----------
         grid : bool, optional
             Set the grid for the plots.
         **kwargs : kwargs
             Keyword arguments from `puma.PlotObject`
@@ -288,15 +286,15 @@
         if reference:
             logger.debug(
                 "Setting roc %s as reference for %s.", key, roc_curve.rej_class
             )
             self.set_roc_reference(key, roc_curve.rej_class)
 
     def set_roc_reference(self, key: str, rej_class: Flavour):
-        """Setting the reference roc curves used in the ratios
+        """Setting the reference roc curves used in the ratios.
 
         Parameters
         ----------
         key : str
             Unique identifier of roc object
         rej_class : str
             Rejection class encoded in roc curve
@@ -323,15 +321,15 @@
                 ),
                 key,
                 self.reference_roc[rej_class],
             )
             self.reference_roc[rej_class] = key
 
     def set_ratio_class(self, ratio_panel: int, rej_class: str | Flavour):
-        """Associate the rejection class to a ratio panel adn set the legend label
+        """Associate the rejection class to a ratio panel adn set the legend label.
 
         Parameters
         ----------
         ratio_panel : int
             Ratio panel either 1 or 2
         rej_class : Flavour
             Rejeciton class associated to that panel
@@ -371,30 +369,29 @@
                 "Ratio classes not set, set them first with `set_ratio_class`."
             )
 
         for rej_class, axis in self.rej_axes.items():
             self.plot_ratios(axis=axis, rej_class=rej_class)
 
     def get_xlim_auto(self):
-        """Returns min and max efficiency values
+        """Returns min and max efficiency values.
 
         Returns
         -------
         float
             Min and max efficiency values
         """
-
         for elem in self.rocs.values():
             self.eff_min = min(np.min(elem.sig_eff), self.eff_min)
             self.eff_max = max(np.max(elem.sig_eff), self.eff_min)
 
         return self.eff_min, self.eff_max
 
     def plot_ratios(self, axis: plt.axis, rej_class: str):
-        """Plotting ratio curves
+        """Plotting ratio curves.
 
         Parameters
         ----------
         axis : plt.axis
             matplotlib axis object
         rej_class : str
             Rejection class
@@ -430,15 +427,15 @@
         Parameters
         ----------
         option : str
             Defines where to place the legend for rejection class. Accepts all options
             from `matplotlib.axes.Axes.legend` as well as the option `ratio_legend`,
             which adds the legend into the ratio panels
 
-         Raises
+        Raises
         ------
         ValueError
             If not 2 ratios requested
         """
         if self.n_ratio_panels != 2:
             raise ValueError("For a rejection class legend you need 2 ratio panels.")
 
@@ -454,15 +451,14 @@
             List of Line2D objects to extract info for legend
 
         Raises
         ------
         ValueError
             If not 2 ratios requested
         """
-
         if self.n_ratio_panels < 2:
             raise ValueError("For a split legend you need 2 ratio panels.")
 
         if self.leg_rej_loc == "ratio_legend":
             for rej_class, axis in self.rej_axes.items():
                 legend_line = mpl.lines.Line2D(
                     [],
@@ -520,15 +516,15 @@
             ncol=self.leg_ncol,
         )
 
     def draw(
         self,
         labelpad: int = None,
     ):
-        """Draw plotting
+        """Draw plotting.
 
         Parameters
         ----------
         labelpad : int, optional
             Spacing in points from the axes bounding box including
             ticks and tick labels, by default None
         """
@@ -569,15 +565,15 @@
             self.atlasify(use_tag=self.use_atlas_tag)
             # atlasify can only handle one legend. Therefore, we remove the frame of
             # the second legend by hand
             if self.legend_flavs is not None:
                 self.legend_flavs.set_frame_on(False)
 
     def plot_roc(self, **kwargs) -> mpl.lines.Line2D:
-        """Plotting roc curves
+        """Plotting roc curves.
 
         Parameters
         ----------
         **kwargs: kwargs
             Keyword arguments passed to plt.axis.plot
 
         Returns
```

### Comparing `puma-hep-0.2.4/puma/tests/hlplots/test_results.py` & `puma-hep-0.2.5/puma/tests/hlplots/test_tagger.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,191 +1,176 @@
 #!/usr/bin/env python
-"""
-Unit test script for the functions in hlplots/tagger.py
-"""
+
+"""Unit test script for the functions in hlplots/tagger.py."""
 import tempfile
 import unittest
-from pathlib import Path
 
 import h5py
 import numpy as np
+import pandas as pd
+from numpy.lib.recfunctions import structured_to_unstructured as s2u
+from numpy.lib.recfunctions import unstructured_to_structured as u2s
 
-from puma.hlplots import Results
-from puma.hlplots.tagger import Tagger
-from puma.utils import (
-    get_dummy_2_taggers,
-    get_dummy_multiclass_scores,
-    logger,
-    set_log_level,
-)
+from puma.hlplots import Tagger
+from puma.utils import logger, set_log_level
 
 set_log_level(logger, "DEBUG")
 
 
-class ResultsTestCase(unittest.TestCase):
-    """Test class for the Results class."""
+class TaggerBasisTestCase(unittest.TestCase):
+    """Test class for the Tagger class."""
 
-    def test_add_duplicated(self):
+    def test_empty_string_tagger_name(self):
         """Test empty string as model name."""
-        dummy_tagger_1 = Tagger("dummy")
-        dummy_tagger_2 = Tagger("dummy")
-        results = Results()
-        results.add(dummy_tagger_1)
-        with self.assertRaises(KeyError):
-            results.add(dummy_tagger_2)
+        tagger = Tagger("")
+        self.assertEqual(tagger.name, "")
 
-    def test_add_2_taggers(self):
-        """Test empty string as model name."""
-        dummy_tagger_1 = Tagger("dummy")
-        dummy_tagger_2 = Tagger("dummy_2")
-        results = Results()
-        results.add(dummy_tagger_1)
-        results.add(dummy_tagger_2)
-        self.assertEqual(
-            list(results.taggers.keys()),
-            ["dummy (dummy)", "dummy_2 (dummy_2)"],  # pylint: disable=W0212
-        )
-
-    def test_get_taggers(self):
-        """Test empty string as model name."""
-        dummy_tagger_1 = Tagger("dummy")
-        dummy_tagger_2 = Tagger("dummy_2")
-        results = Results()
-        results.add(dummy_tagger_1)
-        results.add(dummy_tagger_2)
-        retrieved_dummy_tagger_2 = results["dummy_2 (dummy_2)"]
-        self.assertEqual(retrieved_dummy_tagger_2.name, dummy_tagger_2.name)
-
-    def test_add_taggers_from_file(self):
-        """Test for Results.add_taggers_from_file function"""
-        tmp_dir = tempfile.TemporaryDirectory()  # pylint: disable=R1732
-        rng = np.random.default_rng(seed=16)
-        with h5py.File(f"{tmp_dir.name}/test.h5", "w") as file:
-            data = get_dummy_2_taggers()
-            data["pt"] = rng.random(len(data))
-            file.create_dataset("jets", data=data.to_records())
-        results = Results()
-        taggers = [Tagger("rnnip")]
-        results.add_taggers_from_file(
-            taggers, f"{tmp_dir.name}/test.h5", perf_var=data["pt"]
-        )
-        self.assertEqual(list(results.taggers.values()), taggers)
+    def test_wrong_template(self):
+        """Test wrong template."""
+        template_wrong = {"test": 1}
+        with self.assertRaises(TypeError):
+            Tagger("dummy", **template_wrong)  # pylint: disable=W0212,E1123
+
+    def test_label_template(self):
+        """Test template with label."""
+        template_label = {"label": 1.5}
+        tagger = Tagger("dummy", **template_label)  # pylint: disable=W0212
+        self.assertEqual(tagger.label, 1.5)
+
+    def test_n_jets(self):
+        """Test if number of n_jets correctly calculated."""
+        tagger = Tagger("dummy", output_nodes=["ujets", "cjets", "bjets"])
+        labels = np.concatenate([np.zeros(80), np.ones(5) * 4, np.ones(15) * 5])
+        tagger.labels = np.array(labels, dtype=[("HadronConeExclTruthLabelID", "i4")])
+        with self.subTest():
+            self.assertEqual(tagger.n_jets("ujets"), 80)
+        with self.subTest():
+            self.assertEqual(tagger.n_jets("cjets"), 5)
+        with self.subTest():
+            self.assertEqual(tagger.n_jets("bjets"), 15)
 
 
-class ResultsPlotsTestCase(unittest.TestCase):
-    """Test class for the Results class running plots."""
+class TaggerScoreExtractionTestCase(unittest.TestCase):
+    """Test extract_tagger_scores function in Tagger class."""
 
     def setUp(self) -> None:
-        """Set up for unit tests."""
-        scores, labels = get_dummy_multiclass_scores()
-        dummy_tagger_1 = Tagger("dummy")
-        dummy_tagger_1.labels = np.array(
-            labels, dtype=[("HadronConeExclTruthLabelID", "i4")]
+        """Set up for tests."""
+        self.df_dummy = pd.DataFrame(
+            {
+                "dummy_pc": np.zeros(10),
+                "dummy_pu": np.ones(10),
+                "dummy_pb": np.zeros(10),
+            }
         )
-        dummy_tagger_1.scores = scores
-        dummy_tagger_1.label = "dummy tagger"
-        self.dummy_tagger_1 = dummy_tagger_1
-
-    def assertIsFile(self, path: str):  # pylint: disable=invalid-name
-        """Check for file to exist.
-        Taken from https://stackoverflow.com/a/59198749/10896585
-        Parameters
-        ----------
-        path : str
-            Path to file
-
-        Raises
-        ------
-        AssertionError
-            if file does not exist
-        """
-        if not Path(path).resolve().is_file():
-            raise AssertionError(f"File does not exist: {path}")
-
-    def test_plot_roc_bjets(self):
-        """Test that png file is being created."""
-        self.dummy_tagger_1.reference = True
-        self.dummy_tagger_1.f_c = 0.05
-        results = Results(signal="bjets")
-        results.add(self.dummy_tagger_1)
-        results.sig_eff = np.linspace(0.6, 0.95, 20)
-        with tempfile.TemporaryDirectory() as tmp_file:
-            plot_name = f"{tmp_file}/dummy_plot.png"
-            results.plot_rocs(plot_name=plot_name)
-            self.assertIsFile(plot_name)
-
-    def test_plot_roc_cjets(self):
-        """Test that png file is being created."""
-        self.dummy_tagger_1.reference = True
-        self.dummy_tagger_1.f_b = 0.05
-        results = Results(signal="cjets")
-        results.add(self.dummy_tagger_1)
-        results.sig_eff = np.linspace(0.2, 0.95, 20)
-        with tempfile.TemporaryDirectory() as tmp_file:
-            plot_name = f"{tmp_file}/dummy_plot.png"
-            results.plot_rocs(plot_name=plot_name)
-            self.assertIsFile(plot_name)
-
-    def test_plot_var_perf_bjets(self):
-        """Test that png file is being created."""
-        self.dummy_tagger_1.reference = True
-        self.dummy_tagger_1.f_c = 0.05
-        self.dummy_tagger_1.disc_cut = 2
-        rng = np.random.default_rng(seed=16)
-        self.dummy_tagger_1.perf_var = rng.exponential(
-            100, size=len(self.dummy_tagger_1.scores)
+        self.scores_expected = np.column_stack(
+            (np.ones(10), np.zeros(10), np.zeros(10))
         )
-        results = Results(signal="bjets")
-        results.add(self.dummy_tagger_1)
-        with tempfile.TemporaryDirectory() as tmp_file:
-            plot_name = f"{tmp_file}/dummy_plot"
-            results.plot_var_perf(
-                plot_name=plot_name,
-                bins=[20, 30, 40, 60, 85, 110, 140, 175, 250],
+
+    def test_wrong_source_type(self):
+        """Test using wrong source type."""
+        tagger = Tagger("dummy")
+        with self.assertRaises(ValueError):
+            tagger.extract_tagger_scores(self.df_dummy, source_type="dummy")
+
+    def test_data_frame_path_no_key(self):
+        """Test passing data frame path but no key."""
+        tagger = Tagger("dummy")
+        with self.assertRaises(ValueError):
+            tagger.extract_tagger_scores(self.df_dummy, source_type="data_frame_path")
+
+    def test_data_frame(self):
+        """Test passing data frame."""
+        tagger = Tagger("dummy")
+        tagger.extract_tagger_scores(self.df_dummy)
+        np.testing.assert_array_equal(tagger.scores, self.scores_expected)
+
+    def test_data_frame_path(self):
+        """Test passing data frame path."""
+        tagger = Tagger("dummy")
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            file_name = f"{tmp_dir}/dummy_df.h5"
+            self.df_dummy.to_hdf(file_name, key="dummy_tagger")
+
+            tagger.extract_tagger_scores(
+                file_name, key="dummy_tagger", source_type="data_frame_path"
             )
-            self.assertIsFile(plot_name + "_bjets_eff.png")
-            self.assertIsFile(plot_name + "_cjets_rej.png")
-            self.assertIsFile(plot_name + "_ujets_rej.png")
-
-    def test_plot_var_perf_cjets(self):
-        """Test that png file is being created."""
-        self.dummy_tagger_1.reference = True
-        self.dummy_tagger_1.f_b = 0.05
-        self.dummy_tagger_1.working_point = 0.5
-        rng = np.random.default_rng(seed=16)
-        self.dummy_tagger_1.perf_var = rng.exponential(
-            100, size=len(self.dummy_tagger_1.scores)
-        )
-        results = Results(signal="cjets")
-        results.add(self.dummy_tagger_1)
-        with tempfile.TemporaryDirectory() as tmp_file:
-            plot_name = f"{tmp_file}/dummy_plot"
-            results.plot_var_perf(
-                plot_name=plot_name,
-                h_line=self.dummy_tagger_1.working_point,
-                bins=[20, 30, 40, 60, 85, 110, 140, 175, 250],
+        np.testing.assert_array_equal(tagger.scores, self.scores_expected)
+
+    def test_h5_structured_numpy_path(self):
+        """Test passing structured h5 path."""
+        tagger = Tagger("dummy")
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            file_name = f"{tmp_dir}/dummy_df.h5"
+            with h5py.File(file_name, "w") as f_h5:
+                f_h5.create_dataset(
+                    data=self.df_dummy.to_records(), name="dummy_tagger"
+                )
+
+            tagger.extract_tagger_scores(
+                file_name, key="dummy_tagger", source_type="h5_file"
             )
-            self.assertIsFile(plot_name + "_cjets_eff.png")
-            self.assertIsFile(plot_name + "_bjets_rej.png")
-            self.assertIsFile(plot_name + "_ujets_rej.png")
-
-    def test_plot_discs_bjets(self):
-        """Test that png file is being created."""
-        self.dummy_tagger_1.reference = True
-        self.dummy_tagger_1.f_c = 0.05
-        results = Results(signal="bjets")
-        results.add(self.dummy_tagger_1)
-        with tempfile.TemporaryDirectory() as tmp_file:
-            plot_name = f"{tmp_file}/dummy_plot.png"
-            results.plot_discs(plot_name=plot_name)
-            self.assertIsFile(plot_name)
-
-    def test_plot_discs_cjets(self):
-        """Test that png file is being created."""
-        self.dummy_tagger_1.reference = True
-        self.dummy_tagger_1.f_b = 0.05
-        results = Results(signal="cjets")
-        results.add(self.dummy_tagger_1)
-        with tempfile.TemporaryDirectory() as tmp_file:
-            plot_name = f"{tmp_file}/dummy_plot.png"
-            results.plot_discs(plot_name=plot_name)
-            self.assertIsFile(plot_name)
+        np.testing.assert_array_equal(s2u(tagger.scores), self.scores_expected)
+
+    def test_structured_array(self):
+        """Test passing structured numpy array."""
+        tagger = Tagger("dummy")
+        tagger.extract_tagger_scores(
+            self.df_dummy.to_records(),
+            key="dummy_tagger",
+            source_type="structured_array",
+        )
+        np.testing.assert_array_equal(s2u(tagger.scores), self.scores_expected)
+
+
+class TaggerTestCase(unittest.TestCase):
+    """Test class for the Tagger class."""
+
+    def setUp(self) -> None:
+        """Set up for tests."""
+        scores = np.column_stack((np.ones(10), np.ones(10), np.ones(10)))
+        self.scores = u2s(
+            scores,
+            dtype=[("dummy_pu", "f4"), ("dummy_pc", "f4"), ("dummy_pb", "f4")],
+        )
+
+    def test_disc_cut_template(self):
+        """Test template with disc_cut."""
+        template_disc_cut = {"disc_cut": 1.5}
+        tagger = Tagger("dummy", **template_disc_cut)
+        self.assertEqual(tagger.disc_cut, 1.5)
+
+    def test_errors(self):
+        tagger = Tagger("dummy")
+        tagger.scores = self.scores
+        with self.assertRaises(ValueError):
+            tagger.discriminant("hbb", fx=0.1)
+        with self.assertRaises(ValueError):
+            tagger.discriminant("ujets")
+
+    def test_disc_b_calc_no_fc(self):
+        """Test b-disc calculation w/o f_c provided."""
+        tagger = Tagger("dummy")
+        tagger.scores = self.scores
+        with self.assertRaises(TypeError):
+            tagger.discriminant("bjets")
+
+    def test_disc_b_calc(self):
+        """Test b-disc calculation."""
+        tagger = Tagger("dummy", f_c=0.5)
+        tagger.scores = self.scores
+        discs = tagger.discriminant("bjets")
+        np.testing.assert_array_equal(discs, np.zeros(10))
+
+    def test_disc_c_calc_no_fb(self):
+        """Test c-disc calculation w/o f_c provided."""
+        tagger = Tagger("dummy")
+        tagger.scores = self.scores
+        with self.assertRaises(TypeError):
+            tagger.discriminant("cjets")
+
+    def test_disc_c_calc(self):
+        """Test c-disc calculation."""
+        tagger = Tagger("dummy", f_b=0.5)
+        tagger.scores = self.scores
+        discs = tagger.discriminant("cjets")
+
+        np.testing.assert_array_equal(discs, np.zeros(10))
```

### Comparing `puma-hep-0.2.4/puma/tests/test_histogram.py` & `puma-hep-0.2.5/puma/tests/test_histogram.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 #!/usr/bin/env python
 
 
-"""
-Unit test script for the functions in histogram.py
-"""
+"""Unit test script for the functions in histogram.py."""
 
 import os
 import tempfile
 import unittest
 
 import numpy as np
 from ftag import Flavours
@@ -19,27 +17,27 @@
 set_log_level(logger, "DEBUG")
 
 
 class HistogramTestCase(unittest.TestCase):
     """Test class for the puma.histogram functions."""
 
     def test_empty_histogram(self):
-        """test if providing wrong input type to histogram raises ValueError"""
+        """test if providing wrong input type to histogram raises ValueError."""
         with self.assertRaises(ValueError):
             Histogram(values=5)
 
     def test_divide_before_plotting(self):
-        """test if ValueError is raised when dividing before plotting the histograms"""
+        """test if ValueError is raised when dividing before plotting the histograms."""
         hist_1 = Histogram([1, 1, 1, 2, 2])
         hist_2 = Histogram([1, 2, 2, 2])
         with self.assertRaises(ValueError):
             hist_1.divide(hist_2)
 
     def test_divide_after_plotting_no_norm(self):
-        """test if ratio is calculated correctly after plotting (without norm)"""
+        """test if ratio is calculated correctly after plotting (without norm)."""
         hist_1 = Histogram([1, 1, 1, 2, 2])
         hist_2 = Histogram([1, 2, 2, 2])
         bins = np.array([1, 2, 3])
         hist_plot = HistogramPlot(bins=bins, norm=False)
         hist_plot.add(hist_1)
         hist_plot.add(hist_2)
         hist_plot.plot()
@@ -49,15 +47,15 @@
         expected_ratio = np.array([3, 3, 2 / 3])
         expected_ratio_unc = np.array([3.46410162, 3.46410162, 0.60858062])
 
         np.testing.assert_almost_equal(expected_ratio, hist_1.divide(hist_2)[0])
         np.testing.assert_almost_equal(expected_ratio_unc, hist_1.divide(hist_2)[1])
 
     def test_divide_after_plotting_norm(self):
-        """test if ratio is calculated correctly after plotting (with norm)"""
+        """test if ratio is calculated correctly after plotting (with norm)."""
         hist_1 = Histogram([1, 1, 1, 2, 2])
         hist_2 = Histogram([1, 2, 2, 2])
         bins = np.array([1, 2, 3])
         hist_plot = HistogramPlot(bins=bins, norm=True)
         hist_plot.add(hist_1)
         hist_plot.add(hist_2)
         hist_plot.plot()
@@ -67,15 +65,15 @@
         expected_ratio = np.array([2.4, 2.4, 0.53333333])
         expected_ratio_unc = np.array([2.77128129, 2.77128129, 0.4868645])
 
         np.testing.assert_almost_equal(expected_ratio, hist_1.divide(hist_2)[0])
         np.testing.assert_almost_equal(expected_ratio_unc, hist_1.divide(hist_2)[1])
 
     def test_ratio_same_histogram(self):
-        """test if ratio is 1 for equal histograms (with norm)"""
+        """test if ratio is 1 for equal histograms (with norm)."""
         hist_1 = Histogram([1, 1, 1, 2, 2])
         hist_2 = Histogram([1, 1, 1, 2, 2])
         bins = np.array([1, 2, 3])
         hist_plot = HistogramPlot(bins=bins, norm=True)
         hist_plot.add(hist_1)
         hist_plot.add(hist_2)
         hist_plot.plot()
@@ -107,63 +105,63 @@
     def test_multiple_references_wrong_flavour(self):
         """Tests if warning is raised with wrong flavour."""
         dummy_array = np.array([1, 1, 2, 3, 2, 3])
         with self.assertRaises(KeyError):
             Histogram(dummy_array, flavour="dummy")
 
 
-class HistogramPlotTestCase(
-    unittest.TestCase
-):  # pylint: disable=too-many-public-methods
-    """Test class for puma.histogram_plot"""
+class HistogramPlotTestCase(unittest.TestCase):
+    """Test class for puma.histogram_plot."""
 
     def setUp(self):
         np.random.seed(42)
         n_random = 10_000
         self.hist_1 = Histogram(
             np.random.normal(size=n_random), label=f"N={n_random:_}"
         )
         self.hist_2 = Histogram(
             np.random.normal(size=2 * n_random), label=f"N={2*n_random:_}"
         )
 
         # Set up directories for comparison plots
-        self.tmp_dir = tempfile.TemporaryDirectory()  # pylint: disable=R1732
+        self.tmp_dir = tempfile.TemporaryDirectory()
         self.actual_plots_dir = f"{self.tmp_dir.name}/"
         self.expected_plots_dir = os.path.join(
             os.path.dirname(__file__), "expected_plots"
         )
 
     def test_invalid_bins_type(self):
-        """check if ValueError is raised when using invalid type in `bins` argument"""
+        """check if ValueError is raised when using invalid type in `bins` argument."""
         hist_plot = HistogramPlot(bins=1.1)
         hist_plot.add(self.hist_1, reference=True)
         with self.assertRaises(ValueError):
             hist_plot.plot()
 
     def test_add_bin_width_to_ylabel(self):
-        """check if ValueError is raised when using invalid type in `bins` argument"""
+        """check if ValueError is raised when using invalid type in `bins` argument."""
         hist_plot = HistogramPlot(bins=60)
         hist_plot.add(self.hist_1, reference=True)
         with self.assertRaises(ValueError):
             hist_plot.add_bin_width_to_ylabel()
 
     def test_multiple_references_no_flavour(self):
-        """Tests if error is raised in case of non-unique reference histogram"""
+        """Tests if error is raised in case of non-unique reference histogram."""
         hist_plot = HistogramPlot(n_ratio_panels=1)
         hist_plot.add(self.hist_1, reference=True)
         hist_plot.add(self.hist_2, reference=True)
         hist_plot.add(self.hist_1)
         hist_plot.plot()
         with self.assertRaises(ValueError):
             hist_plot.plot_ratios()
 
     def test_multiple_references_flavour(self):
         """Tests if error is raised in case of non-unique reference histogram
-        when flavoured histograms are used"""
+        when flavoured histograms are used
+        .
+        """
         hist_plot = HistogramPlot(n_ratio_panels=1)
         dummy_array = np.array([1, 1, 2, 3, 2, 3])
         hist_plot.add(Histogram(dummy_array, flavour="ujets"), reference=True)
         hist_plot.add(Histogram(dummy_array, flavour="ujets"), reference=True)
         hist_plot.add(Histogram(dummy_array, flavour="ujets"))
         hist_plot.plot()
         with self.assertRaises(ValueError):
@@ -174,15 +172,15 @@
         with self.assertRaises(ValueError):
             HistogramPlot(n_ratio_panels=2)
 
     def test_custom_range(self):
         """check if
         1. bins_range argument is used correctly
         2. deactivate ATLAS branding works
-        3. adding bin width to ylabel works
+        3. adding bin width to ylabel works.
         """
         hist_plot = HistogramPlot(
             bins=20,
             bins_range=(0, 4),
             atlas_brand="",
             atlas_first_tag="Simulation, $\\sqrt{s}=13$ TeV",
             atlas_second_tag="Second tag with additional\ndistance from first tag",
@@ -204,15 +202,15 @@
                 f"{self.actual_plots_dir}/{plotname}",
                 f"{self.expected_plots_dir}/{plotname}",
                 tol=1,
             )
         )
 
     def test_discrete_values(self):
-        """check if discrete values are working properly"""
+        """check if discrete values are working properly."""
         hist_plot = HistogramPlot(
             bins=np.linspace(0, 10, 100),
             discrete_vals=[0, 5, 7, 9],
             atlas_first_tag="Simulation, $\\sqrt{s}=13$ TeV",
             figsize=(5, 4),
             xlabel="Discrete values",
             ylabel="Number of counts in specified bins",
@@ -235,15 +233,15 @@
                 f"{self.actual_plots_dir}/{plotname}",
                 f"{self.expected_plots_dir}/{plotname}",
                 tol=1,
             )
         )
 
     def test_output_ratio(self):
-        """check with a plot if the ratio is the expected value"""
+        """check with a plot if the ratio is the expected value."""
         hist_plot = HistogramPlot(
             norm=False,
             ymax_ratio=[4],
             figsize=(6.5, 5),
             n_ratio_panels=1,
         )
         hist_plot.add(self.hist_1, reference=True)
@@ -280,16 +278,16 @@
 
     def test_output_empty_histogram_norm(self):
         """Test empty normed histogram."""
         hist_plot = HistogramPlot(
             norm=True,
             figsize=(6.5, 5),
             atlas_second_tag=(
-                "Test if ratio is 1 for whole range if reference histogram is empty\n"
-                "(+ normalised)"
+                "Test if ratio is 1 for whole range if reference histogram is empty\n(+"
+                " normalised)"
             ),
             n_ratio_panels=1,
         )
         hist_plot.add(Histogram(np.array([]), label="empty histogram"), reference=True)
         hist_plot.add(self.hist_1)
         hist_plot.draw()
 
@@ -302,15 +300,15 @@
                 f"{self.actual_plots_dir}/{plotname}",
                 f"{self.expected_plots_dir}/{plotname}",
                 tol=1,
             )
         )
 
     def test_output_empty_histogram_no_norm(self):
-        """Test if ratio is 1 for whole range if reference histogram is empty"""
+        """Test if ratio is 1 for whole range if reference histogram is empty."""
         hist_plot = HistogramPlot(
             norm=False,
             figsize=(6.5, 5),
             atlas_second_tag=(
                 "Test if ratio is 1 for whole range if reference histogram is empty"
             ),
             n_ratio_panels=1,
@@ -329,16 +327,17 @@
                 f"{self.expected_plots_dir}/{plotname}",
                 tol=1,
             )
         )
 
     def test_output_different_range_histogram(self):
         """Test if ratio yields the expected values for case of different histogram
-        ranges"""
-
+        ranges
+        .
+        """
         hist_plot = HistogramPlot(
             atlas_second_tag=(
                 "Test ratio for the case of different histogram ranges. \n"
             ),
             xlabel="x",
             figsize=(7, 6),
             leg_loc="upper right",
@@ -573,16 +572,16 @@
                 f"{self.expected_plots_dir}/{plotname}",
                 tol=1,
             )
         )
 
     def test_flavoured_labels(self):
         """Test different combinations of specifying the label when also specifying a
-        flavour for the histogram."""
-
+        flavour for the histogram.
+        """
         rng = np.random.default_rng(seed=42)
 
         hist_plot = HistogramPlot(
             bins=100,
             atlas_brand=None,
             atlas_first_tag="",
             atlas_second_tag=(
@@ -636,15 +635,15 @@
                 f"{self.actual_plots_dir}/{plotname}",
                 f"{self.expected_plots_dir}/{plotname}",
                 tol=1,
             )
         )
 
     def test_weights(self):
-        """Output plot with weights"""
+        """Output plot with weights."""
         values = np.array([])
         values = np.array([0, 1, 2, 2, 3])
         weights = np.array([1, -1, 3, -2, 1])
         hist_exp = np.array([1, -1, 2])
         unc_exp = np.sqrt(np.array([1, (-1) ** 2, 3**2 + (-2) ** 2 + 1]))
 
         hist_plot = HistogramPlot(
@@ -675,26 +674,26 @@
                 f"{self.actual_plots_dir}/{plotname}",
                 f"{self.expected_plots_dir}/{plotname}",
                 tol=1,
             )
         )
 
     def test_weights_wrong_shape(self):
-        """Check if ValueError is raised if wieghts has"""
+        """Check if ValueError is raised if wieghts has."""
         values = np.array([0, 1, 2, 2, 3])
         weights = np.array([1, -1])
 
         with self.assertRaises(ValueError):
             Histogram(
                 values,
                 weights=weights,
             )
 
     def test_underoverflow_bin(self):
-        """Test if under/overflow bins work as expected"""
+        """Test if under/overflow bins work as expected."""
         vals = [-1, 1, 2, 3, 6]
         vals_with_inf = [-1, 1, 2, 6, np.inf]
 
         hist_plot = HistogramPlot(bins=5, bins_range=(0, 5))
         hist_plot.atlas_second_tag = "This plot does not have under/overflow bins"
         hist_plot.add(Histogram(vals, colour="b"))
         hist_plot.add(Histogram(vals_with_inf, colour="r", linestyle="dotted"))
```

### Comparing `puma-hep-0.2.4/puma/tests/test_line_2d.py` & `puma-hep-0.2.5/puma/tests/test_line_2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 #!/usr/bin/env python
 
-"""
-Unit test script for the functions in line_plot_2d.py
-"""
+"""Unit test script for the functions in line_plot_2d.py."""
 
 import os
 import tempfile
 import unittest
 
 import numpy as np
 from matplotlib.testing.compare import compare_images
@@ -17,58 +15,57 @@
 set_log_level(logger, "DEBUG")
 
 
 class Line2DTestCase(unittest.TestCase):
     """Test class for the puma.line_plot_2d functions."""
 
     def test_wrong_inputs_xvalues(self):
-        """test if providing wrong input type to Line2D raises ValueError"""
+        """test if providing wrong input type to Line2D raises ValueError."""
         with self.assertRaises(ValueError):
             Line2D(
                 x_values="Test",
                 y_values=int(5),
             )
 
     def test_differnt_input_types(self):
-        """test if providing different input types raises ValueError"""
+        """test if providing different input types raises ValueError."""
         with self.assertRaises(ValueError):
             Line2D(
                 x_values=[1, 2, 3],
                 y_values=np.array([1, 2, 3]),
             )
 
     def test_empty_input(self):
-        """test if ValueError is raised when one of the input values is zero"""
+        """test if ValueError is raised when one of the input values is zero."""
         with self.assertRaises(ValueError):
             Line2D(
                 x_values=[],
                 y_values=[1, 2],
             )
 
         with self.assertRaises(ValueError):
             Line2D(
                 x_values=[1, 2],
                 y_values=[],
             )
 
     def test_different_input_shapes(self):
-        """test if ValueError is raised when different lengths given"""
+        """test if ValueError is raised when different lengths given."""
         with self.assertRaises(ValueError):
             Line2D(
                 x_values=[1, 2, 3],
                 y_values=[1, 2],
             )
 
 
 class Line2DPlotTestCase(unittest.TestCase):
-    """Test class for puma.Line2DPlot"""
+    """Test class for puma.Line2DPlot."""
 
     def setUp(self):
         """Set up values needed."""
-
         # Line values
         self.x_values = np.arange(0.001, 1, 0.001)
         self.y_values = np.arange(0.001, 1, 0.001)
 
         # Marker values
         self.marker_x = 0.5
         self.marker_y = 0.5
@@ -77,15 +74,15 @@
         self.tmp_dir = tempfile.TemporaryDirectory()  # pylint: disable=R1732
         self.actual_plots_dir = f"{self.tmp_dir.name}"
         self.expected_plots_dir = os.path.join(
             os.path.dirname(__file__), "expected_plots"
         )
 
     def test_basic(self):
-        """Test the basic functions of Line2DPlot"""
+        """Test the basic functions of Line2DPlot."""
         frac_plot = Line2DPlot(**{"n_ratio_panels": 0})
 
         # Add line
         frac_plot.add(
             Line2D(
                 x_values=self.x_values,
                 y_values=self.y_values,
@@ -128,15 +125,15 @@
                 f"{self.actual_plots_dir}/{plotname}",
                 f"{self.expected_plots_dir}/{plotname}",
                 tol=1,
             )
         )
 
     def test_grid_off(self):
-        """Test the basic functions of Line2DPlot"""
+        """Test the basic functions of Line2DPlot."""
         frac_plot = Line2DPlot(**{"n_ratio_panels": 0}, grid=False)
 
         # Add line
         frac_plot.add(
             Line2D(
                 x_values=self.x_values,
                 y_values=self.y_values,
@@ -179,15 +176,15 @@
                 f"{self.actual_plots_dir}/{plotname}",
                 f"{self.expected_plots_dir}/{plotname}",
                 tol=1,
             )
         )
 
     def test_no_param_set(self):
-        """Test the basic functions of Line2DPlot"""
+        """Test the basic functions of Line2DPlot."""
         frac_plot = Line2DPlot(**{"n_ratio_panels": 0})
 
         # Add line
         frac_plot.add(
             Line2D(
                 x_values=self.x_values,
                 y_values=self.y_values,
@@ -232,15 +229,15 @@
                 f"{self.actual_plots_dir}/{plotname}",
                 f"{self.expected_plots_dir}/{plotname}",
                 tol=1,
             )
         )
 
     def test_double_key(self):
-        """Test the basic functions of Line2DPlot"""
+        """Test the basic functions of Line2DPlot."""
         frac_plot = Line2DPlot(**{"n_ratio_panels": 0})
 
         # Add line
         frac_plot.add(
             Line2D(
                 x_values=self.x_values,
                 y_values=self.y_values,
```

### Comparing `puma-hep-0.2.4/puma/tests/test_metrics.py` & `puma-hep-0.2.5/puma/tests/test_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 #!/usr/bin/env python
 
 
-"""
-Unit test script for the functions in metrics.py
-"""
+"""Unit test script for the functions in metrics.py."""
 
 import unittest
 
 import numpy as np
 
 from puma.metrics import calc_eff, calc_rej, calc_separation, eff_err, rej_err
 from puma.utils import logger, set_log_level
@@ -15,43 +13,45 @@
 set_log_level(logger, "DEBUG")
 
 
 class SeparationTestCase(unittest.TestCase):
     """Test class for the puma.metrics.calc_separation."""
 
     def setUp(self):
-        """Define a default (seeded) random number generator for all tests"""
+        """Define a default (seeded) random number generator for all tests."""
         self.rng = np.random.default_rng(42)
 
     def test_equal_datasets(self):
-        """Separation of two equal datasets (=0)"""
+        """Separation of two equal datasets (=0)."""
         values_a = np.array([1, 1, 2, 2])
         self.assertEqual(0, calc_separation(values_a, values_a)[0])
 
     def test_completely_separated(self):
-        """Separation of two completely separated distributions"""
+        """Separation of two completely separated distributions."""
         values_a = np.array([0.1, 0.5, 0.8, 1])
         values_b = np.array([1.1, 1.5, 1.8, 2])
         self.assertAlmostEqual(1, calc_separation(values_a, values_b)[0])
 
     def test_completely_separated_bad_binning(self):
         """Separation of two completely separated distributions if the binning
-        if chosen such that they share one bin"""
+        if chosen such that they share one bin
+        .
+        """
         values_a = np.array([0.1, 0.5, 0.8, 1])
         values_b = np.array([1.1, 1.5, 1.8, 2])
         self.assertNotAlmostEqual(1, calc_separation(values_a, values_b, bins=3)[0])
 
     def test_half_separated(self):
-        """Separation of 0.5"""
+        """Separation of 0.5."""
         values_a = np.array([0, 1])
         values_b = np.array([1, 2])
         self.assertAlmostEqual(0.5, calc_separation(values_a, values_b, bins=3)[0])
 
     def test_return_bins(self):
-        """Test if bins are correctly returned"""
+        """Test if bins are correctly returned."""
         values_a = np.array([0, 1])
         values_b = np.array([1, 2])
 
         _, _, hist_a, hist_b, bin_edges = calc_separation(
             values_a,
             values_b,
             bins=3,
@@ -84,23 +84,22 @@
 
     def setUp(self):
         rng = np.random.default_rng(seed=42)
         self.disc_sig = rng.normal(loc=3, size=100_000)
         self.disc_bkg = rng.normal(loc=0, size=100_000)
 
     def test_float_target(self):
-        """Test efficiency and cut value calculation for one target value"""
-
+        """Test efficiency and cut value calculation for one target value."""
         # we target a signal efficiency of 0.841345, which is the integral of a gaussian
-        # from μ-1σ to infinity
+        # from μ-1o to infinity
         # -->   the cut_value should be at 2, since the signal is a normal distribution
         #       with mean 3
         # https://www.wolframalpha.com/input?i=integrate+1%2Fsqrt%282+pi%29+*+exp%28-0.5*%28x-3%29**2%29+from+2+to+oo
         # -->   For the bkg efficiency this means that we integrate a normal distr.
-        #       from μ+2σ to infinity --> expect a value of 0.0227501
+        #       from μ+2o to infinity --> expect a value of 0.0227501
         # https://www.wolframalpha.com/input?i=integrate+1%2Fsqrt%282+pi%29+*+exp%28-0.5*x**2%29+from+2+to+oo
         bkg_eff, cut = calc_eff(
             self.disc_sig, self.disc_bkg, target_eff=0.841345, return_cuts=True
         )
         # the values here differ slightly from the values of the analytical integral,
         # since we use random numbers
         self.assertAlmostEqual(cut, 1.9956997)
@@ -110,16 +109,15 @@
         bkg_rej, cut = calc_rej(
             self.disc_sig, self.disc_bkg, target_eff=0.841345, return_cuts=True
         )
         self.assertAlmostEqual(cut, 1.9956997)
         self.assertAlmostEqual(bkg_rej, 1 / 0.02367)
 
     def test_array_target(self):
-        """Test efficiency and cut value calculation for list of target efficiencies"""
-
+        """Test efficiency and cut value calculation for list of target efficiencies."""
         # explanation is the same as above, now also cut the signal in the middle
         # --> target sig.efficiency 0.841345 and 0.5 --> cut at 2 and 3
         bkg_eff, cut = calc_eff(
             self.disc_sig, self.disc_bkg, target_eff=[0.841345, 0.5], return_cuts=True
         )
         # the values here differ slightly from the values of the analytical integral,
         # since we use random numbers
```

### Comparing `puma-hep-0.2.4/puma/tests/test_pie_chart.py` & `puma-hep-0.2.5/puma/tests/test_pie_chart.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 #!/usr/bin/env python
 
-"""
-Unit test script for the functions in histogram.py
-"""
+"""Unit test script for the functions in histogram.py."""
 
 import os
 import tempfile
 import unittest
 
 from matplotlib.testing.compare import compare_images
 
 from puma import PiePlot
 from puma.utils import get_good_colours, logger, set_log_level
 
 set_log_level(logger, "DEBUG")
 
 
 class PiePlotTestCase(unittest.TestCase):
-    """Test class for puma.PiePlot"""
+    """Test class for puma.PiePlot."""
 
     def setUp(self):
         # Set up directories for comparison plots
         self.tmp_dir = tempfile.TemporaryDirectory()  # pylint: disable=R1732
         self.actual_plots_dir = f"{self.tmp_dir.name}/"
         self.expected_plots_dir = os.path.join(
             os.path.dirname(__file__), "expected_plots"
         )
 
     def test_plot_pie_chart_default_style(self):
-        """check if pie chart is plotted correctly (using default style)"""
+        """check if pie chart is plotted correctly (using default style)."""
         pie_plot = PiePlot(
             wedge_sizes=[20, 40, 30, 10],
             labels=["light-flavour jets", "c-jets", "b-jets", "tau-jets"],
         )
         plotname = "test_pie_chart_default_style.png"
         pie_plot.savefig(f"{self.actual_plots_dir}/{plotname}")
         # Uncomment line below to update expected image
@@ -43,15 +41,15 @@
                 f"{self.actual_plots_dir}/{plotname}",
                 f"{self.expected_plots_dir}/{plotname}",
                 tol=1,
             )
         )
 
     def test_plot_pie_chart_custom_style(self):
-        """check if pie chart is plotted correctly (using default style)"""
+        """check if pie chart is plotted correctly (using default style)."""
         pie_plot = PiePlot(
             wedge_sizes=[20, 40, 30, 10],
             labels=["light-flavour jets", "c-jets", "b-jets", "tau-jets"],
             draw_legend=True,
             colours=get_good_colours()[:4],
             # have a look at the possible kwargs for matplotlib.pyplot.pie here:
             # https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.pie.html
```

### Comparing `puma-hep-0.2.4/puma/tests/test_roc.py` & `puma-hep-0.2.5/puma/tests/test_roc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 #!/usr/bin/env python
 
 
-"""
-Unit test script for the functions in roc.py
-"""
+"""Unit test script for the functions in roc.py."""
 
 import os
 import tempfile
 import unittest
 
 import numpy as np
 from matplotlib.testing.compare import compare_images
@@ -178,17 +176,15 @@
         result_bkg_rej = self.bkg_rej[[False, False, False, True, True, False, False]]
         result_sig_eff = self.sig_eff[[False, False, False, True, True, False, False]]
         np.testing.assert_array_almost_equal(
             roc_curve.non_zero, (result_bkg_rej, result_sig_eff)
         )
 
 
-class RocOutputTestCase(
-    unittest.TestCase
-):  # pylint: disable=too-many-instance-attributes
+class RocOutputTestCase(unittest.TestCase):
     """Test class for the puma.roc_plot function."""
 
     def setUp(self):
         # Set up temp directory for comparison plots
         self.tmp_dir = tempfile.TemporaryDirectory()  # pylint: disable=R1732
         self.actual_plots_dir = f"{self.tmp_dir.name}/"
         self.expected_plots_dir = os.path.join(
@@ -218,22 +214,22 @@
         """Test set_leg_rej_loc with one ratio panel."""
         plot = RocPlot(
             n_ratio_panels=2,
         )
         plot.set_leg_rej_loc("upper center")
 
     def test_output_two_curves_no_ratio(self):
-        """Test with two curves of same flavour, without ratio panel"""
+        """Test with two curves of same flavour, without ratio panel."""
         plot = RocPlot(
             n_ratio_panels=0,
             ylabel="Light-jet rejection",
             xlabel="$b$-jet efficiency",
             atlas_second_tag=(
-                "$\\sqrt{s}=13$ TeV, PFlow Jets,\n"
-                "$t\\bar{t}$ dummy sample, $f_{c}=0.018$"
+                "$\\sqrt{s}=13$ TeV, PFlow Jets,\n$t\\bar{t}$ dummy sample,"
+                " $f_{c}=0.018$"
             ),
             y_scale=1.5,
         )
 
         # Add two roc curves
         plot.add_roc(
             Roc(
@@ -265,22 +261,22 @@
                 f"{self.actual_plots_dir}/{plotname}",
                 f"{self.expected_plots_dir}/{plotname}",
                 tol=1,
             )
         )
 
     def test_output_two_curves_one_ratio(self):
-        """Test with two curves of same flavour, one ratio panel"""
+        """Test with two curves of same flavour, one ratio panel."""
         plot = RocPlot(
             n_ratio_panels=1,
             ylabel="Background rejection",
             xlabel="$b$-jet efficiency",
             atlas_second_tag=(
-                "$\\sqrt{s}=13$ TeV, PFlow Jets,\n"
-                "$t\\bar{t}$ dummy sample, $f_{c}=0.018$"
+                "$\\sqrt{s}=13$ TeV, PFlow Jets,\n$t\\bar{t}$ dummy sample,"
+                " $f_{c}=0.018$"
             ),
             y_scale=1.5,
             # logy=False,
         )
 
         # Add two roc curves
         plot.add_roc(
@@ -315,22 +311,22 @@
                 f"{self.actual_plots_dir}/{plotname}",
                 f"{self.expected_plots_dir}/{plotname}",
                 tol=1,
             )
         )
 
     def test_output_two_curves_one_ratio_uncertainties(self):
-        """Test with two curves of same flavour, one ratio panel"""
+        """Test with two curves of same flavour, one ratio panel."""
         plot = RocPlot(
             n_ratio_panels=1,
             ylabel="Background rejection",
             xlabel="$b$-jet efficiency",
             atlas_second_tag=(
-                "$\\sqrt{s}=13$ TeV, PFlow Jets,\n"
-                "$t\\bar{t}$ dummy sample, $f_{c}=0.018$"
+                "$\\sqrt{s}=13$ TeV, PFlow Jets,\n$t\\bar{t}$ dummy sample,"
+                " $f_{c}=0.018$"
             ),
             y_scale=1.5,
             # logy=False,
         )
 
         # Add two roc curves
         plot.add_roc(
@@ -367,22 +363,22 @@
                 f"{self.actual_plots_dir}/{plotname}",
                 f"{self.expected_plots_dir}/{plotname}",
                 tol=1,
             )
         )
 
     def test_output_four_curves_two_ratio(self):
-        """Test with two curves for each flavour, two ratio panels"""
+        """Test with two curves for each flavour, two ratio panels."""
         plot = RocPlot(
             n_ratio_panels=2,
             ylabel="Background rejection",
             xlabel="$b$-jet efficiency",
             atlas_second_tag=(
-                "$\\sqrt{s}=13$ TeV, PFlow Jets,\n"
-                "$t\\bar{t}$ dummy sample, $f_{c}=0.018$"
+                "$\\sqrt{s}=13$ TeV, PFlow Jets,\n$t\\bar{t}$ dummy sample,"
+                " $f_{c}=0.018$"
             ),
         )
 
         # Add four roc curves
         plot.add_roc(
             Roc(
                 self.sig_eff,
@@ -433,24 +429,22 @@
                 f"{self.actual_plots_dir}/{plotname}",
                 f"{self.expected_plots_dir}/{plotname}",
                 tol=1,
             )
         )
 
     def test_output_ratio_legend_four_curves_two_ratio(self):
-        """
-        Test with two curves for each flavour, two ratio panels, using ratio legend.
-        """
+        """Test with two curves for each flavour, two ratio panels, and ratio legend"""
         plot = RocPlot(
             n_ratio_panels=2,
             ylabel="Background rejection",
             xlabel="$b$-jet efficiency",
             atlas_second_tag=(
-                "$\\sqrt{s}=13$ TeV, PFlow Jets,\n"
-                "$t\\bar{t}$ dummy sample, $f_{c}=0.018$"
+                "$\\sqrt{s}=13$ TeV, PFlow Jets,\n$t\\bar{t}$ dummy sample,"
+                " $f_{c}=0.018$"
             ),
         )
 
         # Add four roc curves
         plot.add_roc(
             Roc(
                 self.sig_eff,
@@ -509,16 +503,16 @@
     def test_output_four_curves_two_ratio_uncertainties(self):
         """Test with two curves for each flavour, two ratio panels and binom. unc."""
         plot = RocPlot(
             n_ratio_panels=2,
             ylabel="Background rejection",
             xlabel="$b$-jet efficiency",
             atlas_second_tag=(
-                "$\\sqrt{s}=13$ TeV, PFlow Jets,\n"
-                "$t\\bar{t}$ dummy sample, $f_{c}=0.018$"
+                "$\\sqrt{s}=13$ TeV, PFlow Jets,\n$t\\bar{t}$ dummy sample,"
+                " $f_{c}=0.018$"
             ),
         )
 
         # Add four roc curves
         plot.add_roc(
             Roc(
                 self.sig_eff,
```

### Comparing `puma-hep-0.2.4/puma/tests/test_var_vs_eff.py` & `puma-hep-0.2.5/puma/tests/test_var_vs_eff.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 #!/usr/bin/env python
 
 
-"""
-Unit test script for the functions in var_vs_eff.py
-"""
+"""Unit test script for the functions in var_vs_eff.py."""
 
 import os
 import tempfile
 import unittest
 
 import numpy as np
 from matplotlib.testing.compare import compare_images
@@ -48,15 +46,15 @@
                 disc_cut=1.0,
                 working_point=0.77,
             )
 
     def test_var_vs_eff_init_fixed_eff_no_wp(self):
         """Test var_vs_eff init."""
         with self.assertRaises(ValueError):
-            VarVsEff(np.ones(6), np.ones(6), fixed_eff_bin=True)
+            VarVsEff(np.ones(6), np.ones(6), fixed_eff_bin=True, disc_cut=1.0)
 
     def test_var_vs_eff_init_disc_cut_wp(self):
         """Test var_vs_eff init."""
         with self.assertRaises(ValueError):
             VarVsEff(np.ones(6), np.ones(6), disc_cut=1.0, working_point=0.77)
 
     def test_var_vs_eff_init_no_disc_cut_no_wp(self):
@@ -172,32 +170,31 @@
             disc_sig=self.x_var_sig,
             x_var_bkg=self.disc_bkg,
             disc_bkg=self.x_var_bkg,
             working_point=self.working_point,
             fixed_eff_bin=True,
             bins=n_bins,
         )
-        np.testing.assert_array_almost_equal(
-            var_plot.divide(var_plot, mode="sig_eff")[0], np.ones(1)
-        )
+        var_plot.y_var_mean, var_plot.y_var_std = var_plot.get("sig_eff")
+        np.testing.assert_array_almost_equal(var_plot.divide(var_plot)[0], np.ones(1))
 
-    def test_var_vs_eff_divide_wrong_mode(self):
-        """Test var_vs_eff divide."""
+    def test_var_vs_eff_wrong_mode(self):
+        """Test var_vs_eff wrong mode."""
         n_bins = 1
         var_plot = VarVsEff(
             x_var_sig=self.disc_sig,
             disc_sig=self.x_var_sig,
             x_var_bkg=self.disc_bkg,
             disc_bkg=self.x_var_bkg,
             working_point=self.working_point,
             fixed_eff_bin=True,
             bins=n_bins,
         )
         with self.assertRaises(ValueError):
-            var_plot.divide(var_plot, mode="test")
+            var_plot.y_var_mean, var_plot.y_var_std = var_plot.get("test")
 
     def test_var_vs_eff_divide_different_binning(self):
         """Test var_vs_eff divide."""
         var_plot = VarVsEff(
             x_var_sig=self.disc_sig,
             disc_sig=self.x_var_sig,
             x_var_bkg=self.disc_bkg,
@@ -212,21 +209,42 @@
             x_var_bkg=self.disc_bkg,
             disc_bkg=self.x_var_bkg,
             working_point=self.working_point,
             fixed_eff_bin=True,
             bins=2,
         )
         with self.assertRaises(ValueError):
-            var_plot.divide(var_plot_comp, mode="sig_eff")
+            var_plot.y_var_mean, var_plot.y_var_std = var_plot.get("sig_eff")
+            var_plot_comp.y_var_mean, var_plot_comp.y_var_std = var_plot.get("sig_eff")
+            var_plot.divide(var_plot_comp)
+
+    def test_var_vs_eff_eq_different_classes(self):
+        """Test var_vs_eff eq."""
+        var_plot = VarVsEff(
+            x_var_sig=[0, 1, 2], disc_sig=[3, 4, 5], bins=2, working_point=0.7
+        )
+        self.assertNotEqual(var_plot, np.ones(6))
+
+    def test_var_vs_eff_get(self):
+        var_plot = VarVsEff(
+            x_var_sig=self.disc_sig,
+            disc_sig=self.x_var_sig,
+            x_var_bkg=self.disc_bkg,
+            disc_bkg=self.x_var_bkg,
+            working_point=self.working_point,
+            fixed_eff_bin=True,
+            bins=1,
+        )
+        mode_options = ["sig_eff", "bkg_eff", "sig_rej", "bkg_rej"]
+        for mode in mode_options:
+            var_plot.get(mode)
 
 
-class VarVsEffOutputTestCase(
-    unittest.TestCase
-):  # pylint:disable=too-many-instance-attributes
-    """Test class for the puma.var_vs_eff_plot output"""
+class VarVsEffOutputTestCase(unittest.TestCase):
+    """Test class for the puma.var_vs_eff_plot output."""
 
     def setUp(self):
         # Set up temp directory for comparison plots
         self.tmp_dir = tempfile.TemporaryDirectory()  # pylint:disable=R1732
         self.actual_plots_dir = f"{self.tmp_dir.name}/"
         self.expected_plots_dir = os.path.join(
             os.path.dirname(__file__), "expected_plots"
@@ -262,14 +280,27 @@
                 np.random.uniform(110, 250, size=n_random),
             )
         )
 
         # Define pT bins
         self.bins = [20, 30, 40, 60, 85, 110, 140, 175, 250]
 
+    def test_var_vs_eff_plot_mode_option(self):
+        with self.assertRaises(ValueError):
+            VarVsEffPlot(
+                mode="test",
+                ylabel="Background rejection",
+                xlabel=r"$p_{T}$ [GeV]",
+                logy=True,
+                atlas_second_tag="test",
+                y_scale=1.5,
+                n_ratio_panels=1,
+                figsize=(9, 6),
+            )
+
     def test_output_plot_fixed_eff_bin_bkg_rejection(self):
         """Test output plot with fixed eff per bin - bkg rejection."""
         # define the curves
         ref_light = VarVsEff(
             x_var_sig=self.x_var_sig_1,
             disc_sig=self.disc_sig_1,
             x_var_bkg=self.x_var_bkg,
```

### Comparing `puma-hep-0.2.4/puma/tests/utils/test_discriminant.py` & `puma-hep-0.2.5/puma/tests/utils/test_discriminant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 #!/usr/bin/env python
 
-"""
-Unit test script for the functions in utils/discriminant.py
-"""
+"""Unit test script for the functions in utils/discriminant.py."""
 
 import unittest
 
 import numpy as np
 
 from puma.utils import calc_disc, calc_disc_b, calc_disc_c, logger, set_log_level
```

### Comparing `puma-hep-0.2.4/puma/tests/utils/test_generate.py` & `puma-hep-0.2.5/puma/tests/utils/test_generate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
-"""
-Unit test script for the functions in utils/generate.py
-"""
+"""Unit test script for the functions in utils/generate.py."""
 
 import unittest
 
 import numpy as np
+from numpy.lib.recfunctions import structured_to_unstructured as s2u
 
 from puma.utils import logger, set_log_level
 from puma.utils.generate import get_dummy_2_taggers, get_dummy_multiclass_scores
 
 set_log_level(logger, "DEBUG")
 
 
@@ -23,20 +22,20 @@
         # returns 3 classes with the same amount of stats per class
         with self.subTest("output length"):
             self.assertEqual(len(output), 9)
         with self.subTest("label length"):
             self.assertEqual(len(labels), 9)
 
     def test_range(self):
-        """Check that correct range of output is returned"""
+        """Check that correct range of output is returned."""
         output, _ = get_dummy_multiclass_scores()
         with self.subTest("max val"):
-            self.assertLessEqual(np.max(output), 1)
+            self.assertLessEqual(np.max(s2u(output)), 1)
         with self.subTest("min val"):
-            self.assertGreaterEqual(np.min(output), 0)
+            self.assertGreaterEqual(np.min(s2u(output)), 0)
 
 
 class GetDummy2TaggersTestCase(unittest.TestCase):
     """Test case for get_dummy_2_taggers function."""
 
     def test_size(self):
         """Check that correct size is returned."""
```

### Comparing `puma-hep-0.2.4/puma/tests/utils/test_histogram_utils.py` & `puma-hep-0.2.5/puma/tests/utils/test_histogram_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 #!/usr/bin/env python
 
-"""
-Unit test script for the functions in utils/histogram.py
-"""
+"""Unit test script for the functions in utils/histogram.py."""
 
 import unittest
 
 import numpy as np
 from testfixtures import LogCapture
 
 from puma.utils import logger, set_log_level
 from puma.utils.histogram import hist_ratio, hist_w_unc, save_divide
 
 set_log_level(logger, "DEBUG")
 
 
-class HistWUncTestCase(
-    unittest.TestCase
-):  # pylint: disable=too-many-instance-attributes
+class HistWUncTestCase(unittest.TestCase):
     """Test case for hist_w_unc function."""
 
     def setUp(self):
         self.input = np.array([0, 1, 1, 3])
         self.weights = np.array([1, 2, 1, 1])
         self.n_bins = 3
         self.bin_edges = np.array([0, 1, 2, 3])
@@ -45,16 +41,15 @@
 
         self.hist_weighted = np.array([1, 3, 1])
         # use sqrt(sum of squared weights) for error calculation
         self.unc_weighted = np.sqrt(np.array([1, 2**2 + 1, 1]))
         self.band_weighted = self.hist_weighted - self.unc_weighted
 
     def test_under_overflow_values(self):
-        """Test behaviour for under- and overflow values"""
-
+        """Test behaviour for under- and overflow values."""
         values_with_inf = np.array([-1, 1, 2, 100, np.inf])
 
         with self.subTest("Under/overflow values without under/overflow bins."):
             bins, hist, _, _ = hist_w_unc(values_with_inf, bins=5, bins_range=(0, 5))
             np.testing.assert_almost_equal(bins, np.linspace(0, 5, 6))
             # in this case only 40% of the values are shown in the plot
             np.testing.assert_almost_equal(hist, np.array([0, 0.2, 0.2, 0, 0]))
@@ -101,39 +96,36 @@
         np.testing.assert_almost_equal(bins, self.bin_edges)
         np.testing.assert_almost_equal(hist, self.hist)
         np.testing.assert_almost_equal(unc, self.unc)
         np.testing.assert_almost_equal(band, self.band)
 
     def test_histogram_weighted_normalised(self):
         """Test weighted histogram (normalised)."""
-
         bin_edges, hist, unc, band = hist_w_unc(
             self.input, weights=self.weights, bins=self.n_bins, normed=True
         )
 
         np.testing.assert_array_almost_equal(self.bin_edges, bin_edges)
         np.testing.assert_array_almost_equal(self.hist_weighted_normed, hist)
         np.testing.assert_array_almost_equal(self.unc_weighted_normed, unc)
         np.testing.assert_array_almost_equal(self.band_weighted_normed, band)
 
     def test_histogram_weighted_not_normalised(self):
         """Test weighted histogram (not normalised)."""
-
         bin_edges, hist, unc, band = hist_w_unc(
             self.input, weights=self.weights, bins=self.n_bins, normed=False
         )
 
         np.testing.assert_array_almost_equal(self.bin_edges, bin_edges)
         np.testing.assert_array_almost_equal(self.hist_weighted, hist)
         np.testing.assert_array_almost_equal(self.unc_weighted, unc)
         np.testing.assert_array_almost_equal(self.band_weighted, band)
 
     def test_range_argument_ignored(self):
         """Test if the hist_range argument is ignored when bin_edges are provided."""
-
         bins_range = (1, 2)
 
         bin_edges, hist, _, _ = hist_w_unc(
             self.input,
             bins=self.bin_edges,
             bins_range=bins_range,
             normed=False,
@@ -141,15 +133,14 @@
 
         # check if we end up with the same bin edges anyway
         np.testing.assert_array_almost_equal(self.bin_edges, bin_edges)
         np.testing.assert_array_almost_equal(self.hist, hist)
 
     def test_range_argument(self):
         """Test if the hist_range argument is used when bins is an integer."""
-
         # we test with range from 0 to 2, with 3 bins -> [0, 0.66, 1.33, 2] exp. bins
         bins_range = (0, 2)
         bins_exp = np.array([0, 2 / 3, 1 + 1 / 3, 2])
         hist_exp = np.array([1, 2, 0])
 
         bin_edges, hist, _, _ = hist_w_unc(
             self.input,
@@ -160,29 +151,27 @@
 
         # check if we end up with the same bin edges anyway
         np.testing.assert_array_almost_equal(bins_exp, bin_edges)
         np.testing.assert_array_almost_equal(hist_exp, hist)
 
     def test_negative_weights(self):
         """Test if negative weights are properly handled."""
-
         values = np.array([0, 1, 2, 2, 3])
         weights = np.array([1, -1, 3, -2, 1])
 
         hist_exp = np.array([1, -1, 2])
         # uncertainties are the sqrt(sum of squared weights)
         unc_exp = np.sqrt(np.array([1, (-1) ** 2, 3**2 + (-2) ** 2 + 1]))
 
         _, hist, unc, _ = hist_w_unc(values, weights=weights, bins=3, normed=False)
         np.testing.assert_array_almost_equal(hist_exp, hist)
         np.testing.assert_array_almost_equal(unc_exp, unc)
 
     def test_inf_treatment(self):
         """Test if infinity values are treated as expected."""
-
         values_with_infs = np.array([1, 2, 3, -np.inf, +np.inf, +np.inf])
 
         with self.subTest(
             "Test if the warning for number of inf values is raised in hist_w_unc"
         ):
             with LogCapture("puma") as log:
                 _ = hist_w_unc(values_with_infs, bins=np.linspace(0, 3, 3))
@@ -191,21 +180,19 @@
                         "puma",
                         "WARNING",
                         "Histogram values contain 3 +-inf values!",
                     )
                 )
         with self.subTest(
             "Test if error is raised if inf values are in input but no range is defined"
-        ):
-            with self.assertRaises(ValueError):
-                hist_w_unc(values_with_infs, bins=10)
+        ), self.assertRaises(ValueError):
+            hist_w_unc(values_with_infs, bins=10)
 
     def test_nan_check(self):
-        """Test if the warning with number of nan values is raised in hist_w_unc"""
-
+        """Test if the warning with number of nan values is raised in hist_w_unc."""
         values_with_nans = np.array([1, 2, 3, np.nan, np.nan])
 
         with LogCapture("puma") as log:
             _ = hist_w_unc(values_with_nans, bins=4)
             log.check(
                 (
                     "puma",
```

### Comparing `puma-hep-0.2.4/puma/tests/utils/test_utils.py` & `puma-hep-0.2.5/puma/tests/utils/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 #!/usr/bin/env python
-"""
-Unit test script for the functions in utils/__init__.py
-"""
+"""Unit test script for the functions in utils/__init__.py."""
 
 import os
 import tempfile
 import unittest
 
 import numpy as np
 from matplotlib.testing.compare import compare_images
@@ -30,15 +28,14 @@
     def test_raise_value_error(self):
         """Test if ValueError is raised for wrong argument type."""
         with self.assertRaises(ValueError):
             get_good_linestyles(4)
 
     def test_get_good_linestyles(self):
         """Test if the default linestyles obtained are the correct ones."""
-
         with self.subTest("Testing default linestyles"):
             expected_linestyles = [
                 "solid",
                 (0, (3, 1, 1, 1)),
                 (0, (1, 1)),
                 (0, (5, 2)),
                 (0, (3, 1, 1, 1, 1, 1)),
@@ -64,16 +61,16 @@
         with self.subTest("Test case of only one name given (not list)"):
             expected_linestyle = (0, (5, 2))
             actual_linestyle = get_good_linestyles("densely dashed")
             self.assertTupleEqual(expected_linestyle, actual_linestyle)
 
     def test_linestyles_accepted_by_mpl(self):
         """Test if all the linestyles from get_good_linestyles() are accepted by
-        matplotlib."""
-
+        matplotlib.
+        """
         test_plot = Line2DPlot()
         for i, linestyle in enumerate(get_good_linestyles()):
             test_plot.add(
                 Line2D(
                     np.linspace(0, 10, 10),
                     i * np.linspace(0, 10, 10),
                     linestyle=linestyle,
```

### Comparing `puma-hep-0.2.4/puma/utils/__init__.py` & `puma-hep-0.2.5/puma/utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Module for usefule tools in puma."""
 
 # flake8: noqa
-# pylint: skip-file
+
 
 import numpy as np
 import pandas as pd
 from palettable.colorbrewer.qualitative import Dark2_8
 from scipy.special import softmax
 
 from puma.utils.discriminant import calc_disc, calc_disc_b, calc_disc_c
 from puma.utils.generate import get_dummy_2_taggers, get_dummy_multiclass_scores
-from puma.utils.logging import logger, set_log_level  # noqa: F401
+from puma.utils.logging import logger, set_log_level
 
 
 def set_xaxis_ticklabels_invisible(ax):
     """Helper function to set the ticklabels of the xaxis invisible
 
     Parameters
     ----------
@@ -101,16 +101,16 @@
             "#D19D00",
             "#FFBF00",
             "#FFCB2E",
             "#FFD65C",
             "#FFE28A",
         ]
     raise KeyError(
-        f"Given colour scheme is {colour_scheme} but it has to "
-        "be blue, red, green, yellow or None"
+        f"Given colour scheme is {colour_scheme} but it has to be blue, red, green,"
+        " yellow or None"
     )
 
 
 def get_good_colours(colour_scheme=None):
     """List of colours adequate for plotting
 
     Parameters
@@ -135,14 +135,35 @@
             "#BBBBBB",
         ] + Dark2_8.mpl_colors
 
     elif colour_scheme == "Dark2_8":
         return Dark2_8.mpl_colors
 
 
+def get_good_markers():
+    """List of markers adequate for plotting
+
+    Returns
+    -------
+    list
+        list with markers
+    """
+    # TODO needs improvements
+
+    return [
+        "o",  # Circle
+        "x",  # x
+        "v",  # Triangle down
+        "^",  # Triangle up
+        "D",  # Diamond
+        "p",  # Pentagon
+        "s",  # Square
+    ]
+
+
 def get_good_linestyles(names=None):
     """Returns a list of good linestyles
 
     Parameters
     ----------
     names : list or str, optional
         List or string of the name(s) of the linestyle(s) you want to retrieve, e.g.
```

### Comparing `puma-hep-0.2.4/puma/utils/discriminant.py` & `puma-hep-0.2.5/puma/utils/discriminant.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Discriminant calculation for flavour tagging."""
 import numpy as np
+from numpy.lib.recfunctions import structured_to_unstructured as s2u
 
 from puma.utils.histogram import save_divide
 
 
 def calc_disc(
     scores: np.ndarray,
     flvs: list = None,
@@ -44,14 +45,18 @@
     ... }
     >>> flvs = ["l", "c", "b"]
     >>> scores = np.column_stack((np.ones(10), np.ones(10), np.ones(10)))
     >>> calc_disc(scores, flvs=flvs, flv_map=flv_map)
     array([0., 0., 0., 0., 0., 0., 0., 0., 0., 0.])
     """
     flvs = ["l", "c", "b"] if flvs is None else flvs
+
+    if scores.dtype.names is not None:
+        scores = s2u(scores)
+
     if len(flvs) != scores.shape[1]:
         raise ValueError("`flvs` and `scores` have incompatible shapes.")
     flv_map = (
         {
             "sig": {"b": 1.0},
             "bkg": {"l": 1 - 0.5, "c": 0.5},
         }
```

### Comparing `puma-hep-0.2.4/puma/utils/generate.py` & `puma-hep-0.2.5/puma/utils/generate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Dummy data generation for plotting."""
 from tempfile import NamedTemporaryFile
 
 import h5py
 import numpy as np
 import pandas as pd
+from numpy.lib.recfunctions import structured_to_unstructured as s2u
+from numpy.lib.recfunctions import unstructured_to_structured as u2s
 from scipy.special import softmax
 
 
 def get_dummy_multiclass_scores(
     size: int = 9_999,
     bjets_mean: float = 1.4,
     seed: int = 42,
@@ -40,21 +42,22 @@
     rng = np.random.default_rng(seed=seed)
     ujets = softmax(rng.normal(loc=[-1, 0, 0], scale=1, size=(size_class, 3)), axis=1)
     cjets = softmax(rng.normal(loc=[0, 1, 0], scale=2.5, size=(size_class, 3)), axis=1)
     bjets = softmax(
         rng.normal(loc=[0, 0, bjets_mean], scale=2, size=(size_class, 3)), axis=1
     )
     output = np.concatenate((ujets, cjets, bjets))
+    output = u2s(output, dtype=[("ujets", "f4"), ("cjets", "f4"), ("bjets", "f4")])
     labels = np.concatenate(
         (np.zeros(size_class), np.ones(size_class) * 4, np.ones(size_class) * 5)
     )
     return output, labels
 
 
-def get_dummy_2_taggers(  # pylint: disable=R0913
+def get_dummy_2_taggers(
     size: int = 9_999,
     shuffle: bool = True,
     seed: int = 42,
     add_pt: bool = False,
     label: str = "HadronConeExclTruthLabelID",
     return_file: bool = False,
 ):
@@ -85,20 +88,22 @@
         Dataframe with columns
         [label, rnnip_pu, rnnip_pc, rnnip_pb, dips_pu, dips_pc,
         dips_pb] if `add_pt` is True also pt is added
     """
     output_rnnip, labels = get_dummy_multiclass_scores(
         bjets_mean=0.9, size=size, seed=seed
     )
-    df_gen = pd.DataFrame(output_rnnip, columns=["rnnip_pu", "rnnip_pc", "rnnip_pb"])
+    df_gen = pd.DataFrame(
+        s2u(output_rnnip), columns=["rnnip_pu", "rnnip_pc", "rnnip_pb"]
+    )
     df_gen[label] = labels
     output_dips, _ = get_dummy_multiclass_scores(
         bjets_mean=1.4, size=size, seed=seed + 10
     )
-    df_gen2 = pd.DataFrame(output_dips, columns=["dips_pu", "dips_pc", "dips_pb"])
+    df_gen2 = pd.DataFrame(s2u(output_dips), columns=["dips_pu", "dips_pc", "dips_pb"])
     df_gen = pd.concat([df_gen, df_gen2], axis=1)
     if add_pt:
         rng = np.random.default_rng(seed=seed)
         df_gen["pt"] = rng.exponential(100_000, size=len(df_gen))
     if shuffle:
         df_gen = df_gen.sample(frac=1).reset_index(drop=True)
```

### Comparing `puma-hep-0.2.4/puma/utils/histogram.py` & `puma-hep-0.2.5/puma/utils/histogram.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         where=(denominator != 0),
     )
     if output_shape == 1:
         return float(ratio)
     return ratio
 
 
-def hist_w_unc(  # pylint: disable=too-many-arguments,too-many-locals
+def hist_w_unc(
     arr,
     bins,
     bins_range=None,
     normed: bool = True,
     weights: np.ndarray = None,
     underoverflow: bool = False,
 ):
```

### Comparing `puma-hep-0.2.4/puma/utils/logging.py` & `puma-hep-0.2.5/puma/utils/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 
 class CustomFormatter(logging.Formatter):
     """
     Logging Formatter to add colours and count warning / errors using implementation
     from
-    https://stackoverflow.com/questions/384076/how-can-i-color-python-logging-output
+    https://stackoverflow.com/questions/384076/how-can-i-color-python-logging-output.
     """
 
     grey = "\x1b[38;21m"
     yellow = "\x1b[33;21m"
     green = "\x1b[32;21m"
     red = "\x1b[31;21m"
     bold_red = "\x1b[31;1m"
@@ -81,15 +81,14 @@
         If the log_level is not set, it will
 
     Returns
     -------
     logger
         logger object with new level set
     """
-
     log_level = get_log_level(
         os.environ.get("LOG_LEVEL", "INFO") if log_level is None else log_level
     )
 
     puma_logger = logging.getLogger("puma")
     puma_logger.setLevel(log_level)
     ch_handler = logging.StreamHandler()
@@ -110,14 +109,13 @@
     Parameters
     ----------
     puma_logger : logger
         logger object
     log_level : str
         Logging level corresponding CRITICAL, ERROR, WARNING, INFO, DEBUG, NOTSET
     """
-
     puma_logger.setLevel(get_log_level(log_level))
     for handler in puma_logger.handlers:
         handler.setLevel(get_log_level(log_level))
 
 
 logger = initialise_logger()
```

### Comparing `puma-hep-0.2.4/puma/var_vs_eff.py` & `puma-hep-0.2.5/puma/var_vs_eff.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Efficiency plots vs. specific variable."""
-import matplotlib as mpl
 import numpy as np
 
 # TODO: fix the import below
 from puma.metrics import eff_err, rej_err
-from puma.plot_base import PlotBase, PlotLineObject
-from puma.utils import get_good_colours, logger
-from puma.utils.histogram import hist_ratio, save_divide
+from puma.utils import logger
+from puma.utils.histogram import save_divide
+from puma.var_vs_var import VarVsVar, VarVsVarPlot
 
 
-class VarVsEff(PlotLineObject):  # pylint: disable=too-many-instance-attributes
+class VarVsEff(VarVsVar):  # pylint: disable=too-many-instance-attributes
     """
     var_vs_eff class storing info about curve and allows to calculate ratio w.r.t other
     efficiency plots.
     """
 
-    def __init__(  # pylint: disable=too-many-arguments
+    def __init__(
         self,
         x_var_sig: np.ndarray,
         disc_sig: np.ndarray,
         x_var_bkg: np.ndarray = None,
         disc_bkg: np.ndarray = None,
         bins=10,
         working_point: float = None,
@@ -61,15 +60,14 @@
         Raises
         ------
         ValueError
             If provided options are not compatible with each other
         """
         # TODO: in python 3.10 add multipe type operator | for bins and disc_cut
 
-        super().__init__(**kwargs)
         if len(x_var_sig) != len(disc_sig):
             raise ValueError(
                 f"Length of `x_var_sig` ({len(x_var_sig)}) and `disc_sig` "
                 f"({len(disc_sig)}) have to be identical."
             )
         if x_var_bkg is not None and len(x_var_bkg) != len(disc_bkg):
             raise ValueError(
@@ -84,25 +82,24 @@
         if fixed_eff_bin:
             if disc_cut is not None:
                 raise ValueError(
                     "You cannot specify `disc_cut` when `fixed_eff_bin` is set to True."
                 )
             if working_point is None:
                 raise ValueError(
-                    "You need to specify a working point `wp`, when `fixed_eff_bin` is "
-                    "set to True."
+                    "You need to specify a working point `wp`, when `fixed_eff_bin` is"
+                    " set to True."
                 )
         self.x_var_sig = np.array(x_var_sig)
         self.disc_sig = np.array(disc_sig)
         self.x_var_bkg = None if x_var_bkg is None else np.array(x_var_bkg)
         self.disc_bkg = None if disc_bkg is None else np.array(disc_bkg)
         self.working_point = working_point
         self.disc_cut = disc_cut
         self.fixed_eff_bin = fixed_eff_bin
-        self.key = key
         # Binning related variables
         self.n_bins = None
         self.bn_edges = None
         self.x_bin_centres = None
         self.bin_widths = None
         self.n_bins = None
         # Binned distributions
@@ -112,22 +109,35 @@
         self.disc_binned_bkg = None
 
         self._set_bin_edges(bins)
 
         if disc_cut is not None:
             if working_point is not None:
                 raise ValueError("You cannot specify `disc_cut` when providing `wp`.")
-            if isinstance(disc_cut, (list, np.ndarray)):
-                if self.n_bins != len(disc_cut):
-                    raise ValueError(
-                        "`disc_cut` has to be a float or has to have the same length "
-                        "as number of bins."
-                    )
+            if isinstance(disc_cut, (list, np.ndarray)) and self.n_bins != len(
+                disc_cut
+            ):
+                raise ValueError(
+                    "`disc_cut` has to be a float or has to have the same length as"
+                    " number of bins."
+                )
         self._apply_binning()
         self._get_disc_cuts()
+
+        VarVsVar.__init__(
+            self,
+            x_var=self.x_bin_centres,
+            y_var_mean=np.zeros_like(self.x_bin_centres),
+            y_var_std=np.zeros_like(self.x_bin_centres),
+            x_var_widths=2 * self.bin_widths,
+            key=key,
+            fill=True,
+            plot_y_std=False,
+            **kwargs,
+        )
         self.inverse_cut = False
 
     def _set_bin_edges(self, bins):
         """Calculate bin edges, centres and width and save them as class variables.
 
         Parameters
         ----------
@@ -216,18 +226,17 @@
         Returns
         -------
         float
             Efficiency
         float
             Efficiency error
         """
-        if self.inverse_cut:
-            eff = sum(arr < cut) / len(arr)
-        else:
-            eff = sum(arr > cut) / len(arr)
+        eff = (
+            sum(arr < cut) / len(arr) if self.inverse_cut else sum(arr > cut) / len(arr)
+        )
         eff_error = eff_err(eff, len(arr))
         return eff, eff_error
 
     def rejection(self, arr: np.ndarray, cut: float):
         """Calculate rejection and the associated error.
 
         Parameters
@@ -366,79 +375,24 @@
         if mode == "sig_rej":
             return self.sig_rej
         if mode == "bkg_rej":
             return self.bkg_rej
         # setting class variable again to False
         self.inverse_cut = False
         raise ValueError(
-            f"The selected mode {mode} is not supported. Use one of the following: "
-            f"{mode_options}."
-        )
-
-    def divide(
-        self, other, mode: str, inverse: bool = False, inverse_cut: bool = False
-    ):
-        """Calculate ratio between two class objects.
-
-        Parameters
-        ----------
-        other : var_vs_eff class
-            Second var_vs_eff object to calculate ratio with
-        mode : str
-            Defines the mode which is used for the ratoi calculation, can be the
-            following values: `sig_eff`, `bkg_eff`, `sig_rej`, `bkg_rej`
-        inverse : bool
-            If False the ratio is calculated `this / other`,
-            if True the inverse is calculated
-        inverse_cut : bool
-            Inverts the discriminant cut, which will yield the efficiency or rejection
-            of the jets not passing the working point, by default False
-
-        Returns
-        -------
-        np.ndarray
-            Ratio
-        np.ndarray
-            Ratio error
-        np.ndarray
-            Bin centres
-        np.ndarray
-            Bin widths
-
-        Raises
-        ------
-        ValueError
-            If binning is not identical between 2 objects
-        """
-        if not np.array_equal(self.bin_edges, other.bin_edges):
-            raise ValueError("The binning of the two given objects do not match.")
-        # TODO: python 3.10 switch to cases syntax
-        nom, nom_err = self.get(mode, inverse_cut=inverse_cut)
-        denom, denom_err = other.get(mode, inverse_cut=inverse_cut)
-
-        ratio, ratio_err = hist_ratio(
-            denom if inverse else nom,
-            nom if inverse else denom,
-            denom_err if inverse else nom_err,
-            nom_err if inverse else denom_err,
-            step=False,
-        )
-        return (
-            ratio,
-            ratio_err,
-            self.x_bin_centres,
-            self.bin_widths,
+            f"The selected mode {mode} is not supported. Use one of the following:"
+            f" {mode_options}."
         )
 
 
-class VarVsEffPlot(PlotBase):  # pylint: disable=too-many-instance-attributes
+class VarVsEffPlot(VarVsVarPlot):  # pylint: disable=too-many-instance-attributes
     """var_vs_eff plot class"""
 
     def __init__(self, mode, grid: bool = False, **kwargs) -> None:
-        """var_vs_eff plot properties
+        """var_vs_eff plot properties.
 
         Parameters
         ----------
         mode : str
             Defines which quantity is plotted, the following options ar available:
             "sig_eff", "bkg_eff", "sig_rej" or "bkg_rej"
         grid : bool, optional
@@ -455,253 +409,31 @@
         mode_options = ["sig_eff", "bkg_eff", "sig_rej", "bkg_rej"]
         if mode not in mode_options:
             raise ValueError(
                 f"The selected mode {mode} is not supported. Use one of the following: "
                 f"{mode_options}."
             )
         self.mode = mode
-        self.plot_objects = {}
-        self.add_order = []
-        self.ratios_objects = {}
-        self.reference_object = None
-        self.bin_edge_min = np.inf
-        self.bin_edge_max = -np.inf
-        self.inverse_cut = False
-        if self.n_ratio_panels > 1:
-            raise ValueError("Not more than one ratio panel supported.")
-        self.initialise_figure()
-
-    def add(self, curve: object, key: str = None, reference: bool = False):
-        """Adding var_vs_eff object to figure.
-
-        Parameters
-        ----------
-        curve : var_vs_eff class
-            Var_vs_eff curve
-        key : str, optional
-            Unique identifier for var_vs_eff, by default None
-        reference : bool, optional
-            If var_vs_eff is used as reference for ratio calculation, by default False
 
-        Raises
-        ------
-        KeyError
-            If unique identifier key is used twice
-        """
-        if key is None:
-            key = len(self.plot_objects) + 1
-        if key in self.plot_objects:
-            raise KeyError(f"Duplicated key {key} already used for unique identifier.")
-
-        self.plot_objects[key] = curve
-        self.add_order.append(key)
-        # set linestyle
-        if curve.linestyle is None:
-            curve.linestyle = "-"
-        # set colours
-        if curve.colour is None:
-            curve.colour = get_good_colours()[len(self.plot_objects) - 1]
-        # set alpha
-        if curve.alpha is None:
-            curve.alpha = 0.8
-        # set linewidth
-        if curve.linewidth is None:
-            curve.linewidth = 1.6
-
-        # set min and max bin edges
-        self.bin_edge_min = min(self.bin_edge_min, curve.bin_edges[0])
-        self.bin_edge_max = max(self.bin_edge_max, curve.bin_edges[-1])
-
-        if reference:
-            logger.debug("Setting roc %s as reference.", key)
-            self.set_reference(key)
-
-    def set_reference(self, key: str):
-        """Setting the reference roc curves used in the ratios
-
-        Parameters
-        ----------
-        key : str
-            Unique identifier of roc object
-        """
-        if self.reference_object is None:
-            self.reference_object = key
-        else:
-            logger.warning(
-                (
-                    "You specified a second curve %s as reference for ratio. "
-                    "Using it as new reference instead of %s."
-                ),
-                key,
-                self.reference_object,
-            )
-            self.reference_object = key
+    def _setup_curves(self):
+        for key in self.add_order:
+            elem = self.plot_objects[key]
+            y_value, y_error = elem.get(self.mode, inverse_cut=self.inverse_cut)
+            elem.y_var_mean = y_value
+            elem.y_var_std = y_error
 
     def plot(self, **kwargs):
-        """Plotting curves
+        """Plotting curves.
 
         Parameters
         ----------
         **kwargs: kwargs
             Keyword arguments passed to plt.axis.errorbar
 
         Returns
         -------
         Line2D
             matplotlib Line2D object
         """
         logger.debug("Plotting curves with mode %s", self.mode)
-        plt_handles = []
-        for key in self.add_order:
-            elem = self.plot_objects[key]
-            y_value, y_error = elem.get(self.mode, inverse_cut=self.inverse_cut)
-            error_bar = self.axis_top.errorbar(
-                elem.x_bin_centres,
-                y_value,
-                xerr=elem.bin_widths,
-                yerr=np.zeros(elem.n_bins),
-                color=elem.colour,
-                fmt="none",
-                label=elem.label,
-                alpha=elem.alpha,
-                linewidth=elem.linewidth,
-                **kwargs,
-            )
-            # set linestyle for errorbar
-            error_bar[-1][0].set_linestyle(elem.linestyle)
-            down_variation = y_value - y_error
-            up_variation = y_value + y_error
-            down_variation = np.concatenate((down_variation[:1], down_variation[:]))
-            up_variation = np.concatenate((up_variation[:1], up_variation[:]))
-
-            self.axis_top.fill_between(
-                elem.bin_edges,
-                down_variation,
-                up_variation,
-                color=elem.colour,
-                alpha=0.3,
-                zorder=1,
-                step="pre",
-                edgecolor="none",
-                linestyle=elem.linestyle,
-            )
-            plt_handles.append(
-                mpl.lines.Line2D(
-                    [],
-                    [],
-                    color=elem.colour,
-                    label=elem.label,
-                    linestyle=elem.linestyle,
-                )
-            )
-        return plt_handles
-
-    def plot_ratios(self):
-        """Plotting ratio curves.
-
-        Raises
-        ------
-        ValueError
-            If no reference curve is defined
-        """
-        if self.reference_object is None:
-            raise ValueError("Please specify a reference curve.")
-        for key in self.add_order:
-            elem = self.plot_objects[key]
-            (ratio, ratio_err, x_bin_centres, bin_widths) = elem.divide(
-                self.plot_objects[self.reference_object],
-                mode=self.mode,
-                inverse_cut=self.inverse_cut,
-            )
-            error_bar = self.ratio_axes[0].errorbar(
-                x_bin_centres,
-                ratio,
-                xerr=bin_widths,
-                yerr=np.zeros(elem.n_bins),
-                color=elem.colour,
-                fmt="none",
-                alpha=elem.alpha,
-                linewidth=elem.linewidth,
-            )
-            # set linestyle for errorbar
-            error_bar[-1][0].set_linestyle(elem.linestyle)
-            down_variation = ratio - ratio_err
-            up_variation = ratio + ratio_err
-            down_variation = np.concatenate((down_variation[:1], down_variation[:]))
-            up_variation = np.concatenate((up_variation[:1], up_variation[:]))
-
-            self.ratio_axes[0].fill_between(
-                elem.bin_edges,
-                down_variation,
-                up_variation,
-                color=elem.colour,
-                alpha=0.3,
-                zorder=1,
-                step="pre",
-                edgecolor="none",
-            )
-
-    def set_inverse_cut(self, inverse_cut=True):
-        """Invert the discriminant cut, which will yield the efficiency or rejection
-        of the jets not passing the working point.
-
-        Parameters
-        ----------
-        inverse_cut : bool, optional
-            Invert discriminant cut, by default True
-        """
-        self.inverse_cut = inverse_cut
-
-    def draw_hline(self, y_val: float):
-        """Draw hline in top plot panel.
-
-        Parameters
-        ----------
-        y_val : float
-            y value of the horizontal line
-        """
-        self.axis_top.hlines(
-            y=y_val,
-            xmin=self.bin_edge_min,
-            xmax=self.bin_edge_max,
-            colors="black",
-            linestyle="dotted",
-            alpha=0.5,
-        )
-
-    def draw(
-        self,
-        labelpad: int = None,
-    ):
-        """Draw figure.
-
-        Parameters
-        ----------
-        labelpad : int, optional
-            Spacing in points from the axes bounding box including
-            ticks and tick labels, by default "ratio"
-        """
-        self.set_xlim(
-            self.bin_edge_min if self.xmin is None else self.xmin,
-            self.bin_edge_max if self.xmax is None else self.xmax,
-        )
-        plt_handles = self.plot()
-        if self.n_ratio_panels == 1:
-            self.plot_ratios()
-        self.set_title()
-        self.set_log()
-        self.set_y_lim()
-        self.set_xlabel()
-        self.set_tick_params()
-        self.set_ylabel(self.axis_top)
-
-        if self.n_ratio_panels > 0:
-            self.set_ylabel(
-                self.ratio_axes[0],
-                self.ylabel_ratio[0],
-                align_right=False,
-                labelpad=labelpad,
-            )
-        self.make_legend(plt_handles, ax_mpl=self.axis_top)
-        self.plotting_done = True
-        if self.apply_atlas_style is True:
-            self.atlasify(use_tag=self.use_atlas_tag)
+        self._setup_curves()
+        return super().plot(**kwargs)
```

### Comparing `puma-hep-0.2.4/puma_hep.egg-info/PKG-INFO` & `puma-hep-0.2.5/puma_hep.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puma-hep
-Version: 0.2.4
+Version: 0.2.5
 Summary: Plotting API for HEP flavour tagging plots.
 Home-page: https://github.com/umami-hep/puma
 Keywords: machine learning,flavour tagging,plots
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -71,21 +71,8 @@
 
 On a machine/cluster with singularity installed:
 
 ```bash
 singularity shell -B $PWD docker://gitlab-registry.cern.ch/atlas-flavor-tagging-tools/training-images/puma-images/puma:latest
 ```
 
-### Extended image for development
-
-_For development, just replace the tag of the image_:
-
-`latest` -> `latest-dev`
-
-In addition to the minimal requirements that are required to use `puma`, the
-`puma:latest-dev` image has the `requirements.txt` from the `puma` repo installed as
-well.
-This means that packages like `pytest`, `black`, `pylint`, etc. are installed as well.
-However, note that `puma` itself is not installed in that image such that the dev-version
-on your machine can be used/tested.
-
 **The images are automatically updated via GitHub and pushed to this [repository registry](https://gitlab.cern.ch/atlas-flavor-tagging-tools/training-images/puma-images/container_registry).**
```

### Comparing `puma-hep-0.2.4/puma_hep.egg-info/SOURCES.txt` & `puma-hep-0.2.5/puma_hep.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 puma/__init__.py
+puma/fraction_scan.py
 puma/histogram.py
 puma/line_plot_2d.py
 puma/metrics.py
 puma/pie.py
 puma/plot_base.py
 puma/roc.py
 puma/var_vs_eff.py
+puma/var_vs_var.py
 puma/hlplots/__init__.py
 puma/hlplots/results.py
 puma/hlplots/tagger.py
 puma/tests/__init__.py
 puma/tests/test_histogram.py
 puma/tests/test_line_2d.py
 puma/tests/test_metrics.py
 puma/tests/test_pie_chart.py
 puma/tests/test_plot_base.py
 puma/tests/test_roc.py
 puma/tests/test_var_vs_eff.py
+puma/tests/test_var_vs_var.py
 puma/tests/hlplots/__init__.py
 puma/tests/hlplots/test_results.py
 puma/tests/hlplots/test_tagger.py
 puma/tests/utils/__init__.py
 puma/tests/utils/test_discriminant.py
 puma/tests/utils/test_generate.py
 puma/tests/utils/test_histogram_utils.py
```


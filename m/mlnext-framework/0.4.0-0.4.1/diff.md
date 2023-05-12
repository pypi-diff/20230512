# Comparing `tmp/mlnext_framework-0.4.0.tar.gz` & `tmp/mlnext_framework-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlnext_framework-0.4.0.tar", last modified: Fri Jan 27 14:15:36 2023, max compression
+gzip compressed data, was "mlnext_framework-0.4.1.tar", last modified: Fri May 12 21:32:43 2023, max compression
```

## Comparing `mlnext_framework-0.4.0.tar` & `mlnext_framework-0.4.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 14:15:36.250362 mlnext_framework-0.4.0/
--rw-rw-rw-   0 root         (0) root         (0)     8743 2023-01-27 13:33:08.000000 mlnext_framework-0.4.0/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-01-24 14:25:14.000000 mlnext_framework-0.4.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      158 2023-01-24 14:25:14.000000 mlnext_framework-0.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5657 2023-01-27 14:15:36.250362 mlnext_framework-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3589 2023-01-24 14:32:34.000000 mlnext_framework-0.4.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 14:15:36.170362 mlnext_framework-0.4.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)      639 2023-01-24 14:25:14.000000 mlnext_framework-0.4.0/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      765 2023-01-24 14:25:14.000000 mlnext_framework-0.4.0/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)      130 2023-01-24 14:25:14.000000 mlnext_framework-0.4.0/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 14:15:36.174362 mlnext_framework-0.4.0/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 14:15:36.190362 mlnext_framework-0.4.0/docs/source/_static/
--rw-rw-rw-   0 root         (0) root         (0)   102958 2023-01-24 14:25:15.000000 mlnext_framework-0.4.0/docs/source/_static/digital-factory-dark-logo.png
--rw-rw-rw-   0 root         (0) root         (0)    95413 2023-01-24 14:25:15.000000 mlnext_framework-0.4.0/docs/source/_static/digital-factory-logo.png
--rw-rw-rw-   0 root         (0) root         (0)      766 2023-01-24 14:25:14.000000 mlnext_framework-0.4.0/docs/source/_static/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)     2371 2023-01-24 14:25:15.000000 mlnext_framework-0.4.0/docs/source/_static/mlnext.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 14:15:36.194362 mlnext_framework-0.4.0/docs/source/_templates/
--rw-rw-rw-   0 root         (0) root         (0)      712 2023-01-24 14:25:14.000000 mlnext_framework-0.4.0/docs/source/_templates/custom-class-template.rst
--rw-rw-rw-   0 root         (0) root         (0)     1229 2023-01-24 14:25:14.000000 mlnext_framework-0.4.0/docs/source/_templates/custom-module-template.rst
--rw-rw-rw-   0 root         (0) root         (0)     2985 2023-01-24 14:25:14.000000 mlnext_framework-0.4.0/docs/source/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 14:15:36.230362 mlnext_framework-0.4.0/docs/source/images/
--rw-rw-rw-   0 root         (0) root         (0)    46181 2023-01-24 14:25:15.000000 mlnext_framework-0.4.0/docs/source/images/output_0_1.png
--rw-rw-rw-   0 root         (0) root         (0)    43785 2023-01-24 14:25:15.000000 mlnext_framework-0.4.0/docs/source/images/output_0_3.png
--rw-rw-rw-   0 root         (0) root         (0)    19869 2023-01-24 14:25:15.000000 mlnext_framework-0.4.0/docs/source/images/output_1_1.png
--rw-rw-rw-   0 root         (0) root         (0)    23837 2023-01-24 14:25:15.000000 mlnext_framework-0.4.0/docs/source/images/plot_error.png
--rw-rw-rw-   0 root         (0) root         (0)    49307 2023-01-24 14:25:15.000000 mlnext_framework-0.4.0/docs/source/images/plot_history.png
--rw-rw-rw-   0 root         (0) root         (0)    22733 2023-01-24 14:25:15.000000 mlnext_framework-0.4.0/docs/source/images/plot_point_adjust_metrics.png
--rw-rw-rw-   0 root         (0) root         (0)    28186 2023-01-24 14:25:15.000000 mlnext_framework-0.4.0/docs/source/images/plot_rankings.png
--rw-rw-rw-   0 root         (0) root         (0)     5318 2023-01-24 14:25:15.000000 mlnext_framework-0.4.0/docs/source/images/plot_signals.png
--rw-rw-rw-   0 root         (0) root         (0)     6172 2023-01-24 14:25:15.000000 mlnext_framework-0.4.0/docs/source/images/plot_signals_binary.png
--rw-rw-rw-   0 root         (0) root         (0)     6420 2023-01-24 14:25:15.000000 mlnext_framework-0.4.0/docs/source/images/plot_signals_norm.png
--rw-rw-rw-   0 root         (0) root         (0)    62574 2023-01-24 14:25:15.000000 mlnext_framework-0.4.0/docs/source/images/pr_curve.png
--rw-rw-rw-   0 root         (0) root         (0)      657 2023-01-27 13:47:31.000000 mlnext_framework-0.4.0/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 14:15:36.238362 mlnext_framework-0.4.0/docs/source/pages/
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-01-24 14:25:14.000000 mlnext_framework-0.4.0/docs/source/pages/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)      588 2023-01-24 14:25:14.000000 mlnext_framework-0.4.0/docs/source/pages/notice.rst
--rw-rw-rw-   0 root         (0) root         (0)     2969 2023-01-24 14:25:14.000000 mlnext_framework-0.4.0/docs/source/pages/readme.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 14:15:36.242362 mlnext_framework-0.4.0/mlnext/
--rw-rw-rw-   0 root         (0) root         (0)      502 2023-01-24 14:25:14.000000 mlnext_framework-0.4.0/mlnext/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11540 2023-01-24 14:32:34.000000 mlnext_framework-0.4.0/mlnext/anomaly.py
--rw-rw-rw-   0 root         (0) root         (0)     9441 2023-01-27 08:00:53.000000 mlnext_framework-0.4.0/mlnext/data.py
--rw-rw-rw-   0 root         (0) root         (0)     6951 2023-01-27 08:00:53.000000 mlnext_framework-0.4.0/mlnext/io.py
--rw-rw-rw-   0 root         (0) root         (0)    34739 2023-01-27 13:25:42.000000 mlnext_framework-0.4.0/mlnext/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)    24138 2023-01-27 08:00:53.000000 mlnext_framework-0.4.0/mlnext/plot.py
--rw-rw-rw-   0 root         (0) root         (0)    27761 2023-01-27 08:00:53.000000 mlnext_framework-0.4.0/mlnext/score.py
--rw-rw-rw-   0 root         (0) root         (0)     7678 2023-01-24 14:25:14.000000 mlnext_framework-0.4.0/mlnext/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 14:15:36.246362 mlnext_framework-0.4.0/mlnext_framework.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5657 2023-01-27 14:15:36.000000 mlnext_framework-0.4.0/mlnext_framework.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1414 2023-01-27 14:15:36.000000 mlnext_framework-0.4.0/mlnext_framework.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-27 14:15:36.000000 mlnext_framework-0.4.0/mlnext_framework.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      508 2023-01-27 14:15:36.000000 mlnext_framework-0.4.0/mlnext_framework.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-01-27 14:15:36.000000 mlnext_framework-0.4.0/mlnext_framework.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      891 2023-01-24 14:25:14.000000 mlnext_framework-0.4.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-01-24 14:32:34.000000 mlnext_framework-0.4.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-27 14:15:36.250362 mlnext_framework-0.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3334 2023-01-24 14:25:14.000000 mlnext_framework-0.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-27 14:15:36.250362 mlnext_framework-0.4.0/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-24 14:25:14.000000 mlnext_framework-0.4.0/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8654 2023-01-24 14:32:34.000000 mlnext_framework-0.4.0/test/test_anomaly.py
--rw-rw-rw-   0 root         (0) root         (0)     6620 2023-01-24 14:25:14.000000 mlnext_framework-0.4.0/test/test_data.py
--rw-rw-rw-   0 root         (0) root         (0)     7003 2023-01-24 14:25:14.000000 mlnext_framework-0.4.0/test/test_io.py
--rw-rw-rw-   0 root         (0) root         (0)    17126 2023-01-27 13:25:42.000000 mlnext_framework-0.4.0/test/test_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)      973 2023-01-24 14:25:14.000000 mlnext_framework-0.4.0/test/test_plot.py
--rw-rw-rw-   0 root         (0) root         (0)    11287 2023-01-24 15:11:24.000000 mlnext_framework-0.4.0/test/test_score.py
--rw-rw-rw-   0 root         (0) root         (0)     8883 2023-01-24 14:25:14.000000 mlnext_framework-0.4.0/test/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:32:43.393671 mlnext_framework-0.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)     9052 2023-05-12 21:32:27.000000 mlnext_framework-0.4.1/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      158 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5063 2023-05-12 21:32:43.393671 mlnext_framework-0.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3589 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:32:43.313671 mlnext_framework-0.4.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      639 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      765 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)      130 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:32:43.313671 mlnext_framework-0.4.1/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:32:43.329671 mlnext_framework-0.4.1/docs/source/_static/
+-rw-rw-rw-   0 root         (0) root         (0)   102958 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/docs/source/_static/digital-factory-dark-logo.png
+-rw-rw-rw-   0 root         (0) root         (0)    95413 2023-05-12 21:04:08.000000 mlnext_framework-0.4.1/docs/source/_static/digital-factory-logo.png
+-rw-rw-rw-   0 root         (0) root         (0)      766 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/docs/source/_static/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     2371 2023-05-12 21:04:08.000000 mlnext_framework-0.4.1/docs/source/_static/mlnext.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:32:43.333671 mlnext_framework-0.4.1/docs/source/_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      712 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/docs/source/_templates/custom-class-template.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/docs/source/_templates/custom-module-template.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2985 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/docs/source/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:32:43.373671 mlnext_framework-0.4.1/docs/source/images/
+-rw-rw-rw-   0 root         (0) root         (0)    46181 2023-05-12 21:04:08.000000 mlnext_framework-0.4.1/docs/source/images/output_0_1.png
+-rw-rw-rw-   0 root         (0) root         (0)    43785 2023-05-12 21:04:08.000000 mlnext_framework-0.4.1/docs/source/images/output_0_3.png
+-rw-rw-rw-   0 root         (0) root         (0)    19869 2023-05-12 21:04:08.000000 mlnext_framework-0.4.1/docs/source/images/output_1_1.png
+-rw-rw-rw-   0 root         (0) root         (0)    23837 2023-05-12 21:04:08.000000 mlnext_framework-0.4.1/docs/source/images/plot_error.png
+-rw-rw-rw-   0 root         (0) root         (0)    49307 2023-05-12 21:04:08.000000 mlnext_framework-0.4.1/docs/source/images/plot_history.png
+-rw-rw-rw-   0 root         (0) root         (0)    22733 2023-05-12 21:04:08.000000 mlnext_framework-0.4.1/docs/source/images/plot_point_adjust_metrics.png
+-rw-rw-rw-   0 root         (0) root         (0)    28186 2023-05-12 21:04:08.000000 mlnext_framework-0.4.1/docs/source/images/plot_rankings.png
+-rw-rw-rw-   0 root         (0) root         (0)     5318 2023-05-12 21:04:08.000000 mlnext_framework-0.4.1/docs/source/images/plot_signals.png
+-rw-rw-rw-   0 root         (0) root         (0)     6172 2023-05-12 21:04:08.000000 mlnext_framework-0.4.1/docs/source/images/plot_signals_binary.png
+-rw-rw-rw-   0 root         (0) root         (0)     6420 2023-05-12 21:04:08.000000 mlnext_framework-0.4.1/docs/source/images/plot_signals_norm.png
+-rw-rw-rw-   0 root         (0) root         (0)    62574 2023-05-12 21:04:08.000000 mlnext_framework-0.4.1/docs/source/images/pr_curve.png
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:32:43.385671 mlnext_framework-0.4.1/docs/source/pages/
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/docs/source/pages/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)      588 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/docs/source/pages/notice.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2969 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/docs/source/pages/readme.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:32:43.389671 mlnext_framework-0.4.1/mlnext/
+-rw-rw-rw-   0 root         (0) root         (0)      502 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/mlnext/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11555 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/mlnext/anomaly.py
+-rw-rw-rw-   0 root         (0) root         (0)     9441 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/mlnext/data.py
+-rw-rw-rw-   0 root         (0) root         (0)     6951 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/mlnext/io.py
+-rw-rw-rw-   0 root         (0) root         (0)    34739 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/mlnext/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)    24138 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/mlnext/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)    27761 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/mlnext/score.py
+-rw-rw-rw-   0 root         (0) root         (0)     7678 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/mlnext/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:32:43.389671 mlnext_framework-0.4.1/mlnext_framework.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5063 2023-05-12 21:32:43.000000 mlnext_framework-0.4.1/mlnext_framework.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-05-12 21:32:43.000000 mlnext_framework-0.4.1/mlnext_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 21:32:43.000000 mlnext_framework-0.4.1/mlnext_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      508 2023-05-12 21:32:43.000000 mlnext_framework-0.4.1/mlnext_framework.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-12 21:32:43.000000 mlnext_framework-0.4.1/mlnext_framework.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      891 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 21:32:43.397671 mlnext_framework-0.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3334 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:32:43.393671 mlnext_framework-0.4.1/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8679 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/test/test_anomaly.py
+-rw-rw-rw-   0 root         (0) root         (0)     6620 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/test/test_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     7003 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/test/test_io.py
+-rw-rw-rw-   0 root         (0) root         (0)    17126 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/test/test_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)      973 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/test/test_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)    11287 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/test/test_score.py
+-rw-rw-rw-   0 root         (0) root         (0)     8883 2023-05-12 21:04:07.000000 mlnext_framework-0.4.1/test/test_utils.py
```

### Comparing `mlnext_framework-0.4.0/CHANGELOG.rst` & `mlnext_framework-0.4.1/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,30 @@
 
    This changelog is managed by towncrier and is compiled at release time.
 
    See https://www.attrs.org/en/latest/contributing.html#changelog for details.
 
 .. towncrier release notes start
 
+0.4.1 (2023-05-12)
+------------------
+
+
+
+
+Features
+^^^^^^^^
+
+- fixed ``mlnext.find_anomalies`` for scalar inputs (every dimension 1)
+  `#52 <https://gitlab.phoenixcontact.com/vmm-factory-automation/digital-factory/data-collection-storage-evaluation/anomaly-detection/mlnext_framework/-/issues/52>`__
+
+
+----
+
+
 0.4.0 (2023-01-27)
 ------------------
 
 
 Changes
 ^^^^^^^
```

### Comparing `mlnext_framework-0.4.0/LICENSE` & `mlnext_framework-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/PKG-INFO` & `mlnext_framework-0.4.1/mlnext_framework.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mlnext_framework
-Version: 0.4.0
+Name: mlnext-framework
+Version: 0.4.1
 Summary: Machine learning utilities.
 Home-page: UNKNOWN
 Author: Phoenix Contact Electronics GmbH
 Author-email: digitalfactorynow@phoenixcontact.com
 Maintainer: Phoenix Contact Electronics GmbH
 Maintainer-email: digitalfactorynow@phoenixcontact.com
 License: UNKNOWN
@@ -103,48 +103,24 @@
    # hint: all functions can also be accessed from the root module
    import mlnext
 
 
 Release Information
 ===================
 
-0.4.0 (2023-01-27)
+0.4.1 (2023-05-12)
 ------------------
 
 
-Changes
-^^^^^^^
-
-- Updated the signature and docstrings of ``mlnext.plot.plot_signals``.
-  
-- Refactored ``mlnext.score.eval_sigmoid``.
-  
-- Removed ``roc_auc`` from ``mlnext.score.eval_metrics``.
-  
-- Fixed inconsistent ``typing`` import.
-  
-- Removed ``neg_label`` from ``score.apply_threshold``.
-  
 
 
 Features
 ^^^^^^^^
 
-- Added ``mlnext.pipeline.ClippingMinMaxScaler``.
-  
-- Added ``mlnext.recall_anomalies`` and integrations for ``mlnext.eval_metrics``, ``mlnext.pr_curve``.
-  
-
-
-Deprecations
-^^^^^^^^^^^^
-
-- Deprecated ``y_true`` in favor of ``y`` in ``mlnext.pr_curve``.
-  
-- ``score.apply_threshold`` superceedes the functionality of ``score.eval_sigmoid`` and is removed in 0.6.
+- fixed ``mlnext.find_anomalies`` for scalar inputs (every dimension 1)
   
 
 
 ----
```

### Comparing `mlnext_framework-0.4.0/README.rst` & `mlnext_framework-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/docs/Makefile` & `mlnext_framework-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/docs/make.bat` & `mlnext_framework-0.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/docs/source/_static/digital-factory-dark-logo.png` & `mlnext_framework-0.4.1/docs/source/_static/digital-factory-dark-logo.png`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/docs/source/_static/digital-factory-logo.png` & `mlnext_framework-0.4.1/docs/source/_static/digital-factory-logo.png`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/docs/source/_static/favicon.ico` & `mlnext_framework-0.4.1/docs/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/docs/source/_static/mlnext.png` & `mlnext_framework-0.4.1/docs/source/_static/mlnext.png`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/docs/source/_templates/custom-class-template.rst` & `mlnext_framework-0.4.1/docs/source/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/docs/source/_templates/custom-module-template.rst` & `mlnext_framework-0.4.1/docs/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/docs/source/conf.py` & `mlnext_framework-0.4.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/docs/source/images/output_0_1.png` & `mlnext_framework-0.4.1/docs/source/images/output_0_1.png`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/docs/source/images/output_0_3.png` & `mlnext_framework-0.4.1/docs/source/images/output_0_3.png`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/docs/source/images/output_1_1.png` & `mlnext_framework-0.4.1/docs/source/images/output_1_1.png`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/docs/source/images/plot_error.png` & `mlnext_framework-0.4.1/docs/source/images/plot_error.png`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/docs/source/images/plot_history.png` & `mlnext_framework-0.4.1/docs/source/images/plot_history.png`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/docs/source/images/plot_point_adjust_metrics.png` & `mlnext_framework-0.4.1/docs/source/images/plot_point_adjust_metrics.png`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/docs/source/images/plot_rankings.png` & `mlnext_framework-0.4.1/docs/source/images/plot_rankings.png`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/docs/source/images/plot_signals.png` & `mlnext_framework-0.4.1/docs/source/images/plot_signals.png`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/docs/source/images/plot_signals_binary.png` & `mlnext_framework-0.4.1/docs/source/images/plot_signals_binary.png`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/docs/source/images/plot_signals_norm.png` & `mlnext_framework-0.4.1/docs/source/images/plot_signals_norm.png`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/docs/source/images/pr_curve.png` & `mlnext_framework-0.4.1/docs/source/images/pr_curve.png`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/docs/source/index.rst` & `mlnext_framework-0.4.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/docs/source/pages/notice.rst` & `mlnext_framework-0.4.1/docs/source/pages/notice.rst`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/docs/source/pages/readme.rst` & `mlnext_framework-0.4.1/docs/source/pages/readme.rst`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/mlnext/anomaly.py` & `mlnext_framework-0.4.1/mlnext/anomaly.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 
     Example:
         >>> find_anomalies(np.array([0, 1, 1, 0, 1, 0, 1, 1]))
         [(1, 2), (4, 4), (6, 7)]
     """
 
-    y = np.array(y).squeeze()
+    y = np.atleast_1d(np.array(y).squeeze())
     check_ndim(y, ndim=1)
 
     y = pd.Series(y)
 
     # true for index i when y[i - 1] = 0 and y[i] = 1
     start = (y > y.shift(1, fill_value=0))
     # true for index i when y[i] = 1 and y[i + 1] = 0
```

### Comparing `mlnext_framework-0.4.0/mlnext/data.py` & `mlnext_framework-0.4.1/mlnext/data.py`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/mlnext/io.py` & `mlnext_framework-0.4.1/mlnext/io.py`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/mlnext/pipeline.py` & `mlnext_framework-0.4.1/mlnext/pipeline.py`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/mlnext/plot.py` & `mlnext_framework-0.4.1/mlnext/plot.py`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/mlnext/score.py` & `mlnext_framework-0.4.1/mlnext/score.py`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/mlnext/utils.py` & `mlnext_framework-0.4.1/mlnext/utils.py`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/mlnext_framework.egg-info/PKG-INFO` & `mlnext_framework-0.4.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mlnext-framework
-Version: 0.4.0
+Name: mlnext_framework
+Version: 0.4.1
 Summary: Machine learning utilities.
 Home-page: UNKNOWN
 Author: Phoenix Contact Electronics GmbH
 Author-email: digitalfactorynow@phoenixcontact.com
 Maintainer: Phoenix Contact Electronics GmbH
 Maintainer-email: digitalfactorynow@phoenixcontact.com
 License: UNKNOWN
@@ -103,48 +103,24 @@
    # hint: all functions can also be accessed from the root module
    import mlnext
 
 
 Release Information
 ===================
 
-0.4.0 (2023-01-27)
+0.4.1 (2023-05-12)
 ------------------
 
 
-Changes
-^^^^^^^
-
-- Updated the signature and docstrings of ``mlnext.plot.plot_signals``.
-  
-- Refactored ``mlnext.score.eval_sigmoid``.
-  
-- Removed ``roc_auc`` from ``mlnext.score.eval_metrics``.
-  
-- Fixed inconsistent ``typing`` import.
-  
-- Removed ``neg_label`` from ``score.apply_threshold``.
-  
 
 
 Features
 ^^^^^^^^
 
-- Added ``mlnext.pipeline.ClippingMinMaxScaler``.
-  
-- Added ``mlnext.recall_anomalies`` and integrations for ``mlnext.eval_metrics``, ``mlnext.pr_curve``.
-  
-
-
-Deprecations
-^^^^^^^^^^^^
-
-- Deprecated ``y_true`` in favor of ``y`` in ``mlnext.pr_curve``.
-  
-- ``score.apply_threshold`` superceedes the functionality of ``score.eval_sigmoid`` and is removed in 0.6.
+- fixed ``mlnext.find_anomalies`` for scalar inputs (every dimension 1)
   
 
 
 ----
```

### Comparing `mlnext_framework-0.4.0/mlnext_framework.egg-info/SOURCES.txt` & `mlnext_framework-0.4.1/mlnext_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/pyproject.toml` & `mlnext_framework-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/setup.py` & `mlnext_framework-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/test/test_anomaly.py` & `mlnext_framework-0.4.1/test/test_anomaly.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     'y,exp',
     [
         ([0, 1, 1, 0, 1, 0, 1, 1], [(1, 2), (4, 4), (6, 7)]),
         ([1, 1, 0, 1, 1], [(0, 1), (3, 4)]),
         ([0, 1, 0, 1, 0], [(1, 1), (3, 3)]),
         ([0, 0, 0, 0, 0], []),
         ([1, 1, 1, 1], [(0, 3)]),
+        ([1], [(0, 0)]),
 
         (np.array([[0, 1, 1, 0, 1, 0, 1, 1]]).T, [(1, 2), (4, 4), (6, 7)])
     ]
 )
 def test_find_anomalies(y: np.ndarray, exp: T.List[T.Tuple[int, int]]):
 
     result = find_anomalies(y=np.array(y))
```

### Comparing `mlnext_framework-0.4.0/test/test_data.py` & `mlnext_framework-0.4.1/test/test_data.py`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/test/test_io.py` & `mlnext_framework-0.4.1/test/test_io.py`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/test/test_pipeline.py` & `mlnext_framework-0.4.1/test/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/test/test_plot.py` & `mlnext_framework-0.4.1/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/test/test_score.py` & `mlnext_framework-0.4.1/test/test_score.py`

 * *Files identical despite different names*

### Comparing `mlnext_framework-0.4.0/test/test_utils.py` & `mlnext_framework-0.4.1/test/test_utils.py`

 * *Files identical despite different names*


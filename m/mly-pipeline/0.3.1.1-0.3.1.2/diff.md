# Comparing `tmp/mly_pipeline-0.3.1.1.tar.gz` & `tmp/mly_pipeline-0.3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mly_pipeline-0.3.1.1.tar", last modified: Fri May 12 10:04:43 2023, max compression
+gzip compressed data, was "mly_pipeline-0.3.1.2.tar", last modified: Fri May 12 11:19:42 2023, max compression
```

## Comparing `mly_pipeline-0.3.1.1.tar` & `mly_pipeline-0.3.1.2.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 10:04:43.350514 mly_pipeline-0.3.1.1/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      101 2023-05-11 15:58:46.000000 mly_pipeline-0.3.1.1/.gitignore
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1691 2023-05-10 09:58:07.000000 mly_pipeline-0.3.1.1/.gitlab-ci.yml
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-10 08:55:08.000000 mly_pipeline-0.3.1.1/LICENSE
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6683 2023-05-12 10:04:43.349514 mly_pipeline-0.3.1.1/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6313 2022-03-23 16:00:11.000000 mly_pipeline-0.3.1.1/README.md
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 10:04:43.028510 mly_pipeline-0.3.1.1/docs/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      584 2022-09-29 13:06:48.000000 mly_pipeline-0.3.1.1/docs/Makefile
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 10:04:43.006510 mly_pipeline-0.3.1.1/docs/build/
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 10:04:43.175512 mly_pipeline-0.3.1.1/docs/build/doctrees/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    29429 2022-09-29 13:06:48.000000 mly_pipeline-0.3.1.1/docs/build/doctrees/HowToUse.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10289 2022-09-29 13:06:48.000000 mly_pipeline-0.3.1.1/docs/build/doctrees/Installation.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  2070494 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.1/docs/build/doctrees/environment.pickle
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    62765 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.1/docs/build/doctrees/gettingstarted.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    42039 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.1/docs/build/doctrees/howtouse.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6320 2023-05-04 11:02:10.000000 mly_pipeline-0.3.1.1/docs/build/doctrees/index.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13735 2023-05-04 11:02:10.000000 mly_pipeline-0.3.1.1/docs/build/doctrees/installation.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    66958 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.1/docs/build/doctrees/runningasearch.doctree
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    72638 2023-05-04 11:10:20.000000 mly_pipeline-0.3.1.1/docs/build/doctrees/settingupasearch.doctree
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 10:04:43.224512 mly_pipeline-0.3.1.1/docs/build/html/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9207 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.1/docs/build/html/Getting Started.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9206 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.1/docs/build/html/GettingStarted.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4601 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.1/docs/build/html/How to use.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17205 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.1/docs/build/html/HowToUse.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8839 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.1/docs/build/html/Installation.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 10:04:43.227512 mly_pipeline-0.3.1.1/docs/build/html/_modules/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3285 2023-04-26 10:02:39.000000 mly_pipeline-0.3.1.1/docs/build/html/_modules/index.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13865 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.1/docs/build/html/_modules/io.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 10:04:43.234512 mly_pipeline-0.3.1.1/docs/build/html/_sources/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      979 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.1/docs/build/html/_sources/How to use.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5555 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.1/docs/build/html/_sources/HowToUse.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2490 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.1/docs/build/html/_sources/Installation.rst.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.1/docs/build/html/_sources/index.rst.txt
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 10:04:43.286513 mly_pipeline-0.3.1.1/docs/build/html/_static/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      673 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.1/docs/build/html/_static/ajax-loader.gif
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    11185 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.1/docs/build/html/_static/alabaster.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    15205 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.1/docs/build/html/_static/basic.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9799 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.1/docs/build/html/_static/bizstyle.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1139 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.1/docs/build/html/_static/bizstyle.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14940 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.1/docs/build/html/_static/css3-mediaqueries.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28634 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.1/docs/build/html/_static/css3-mediaqueries_src.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       42 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.1/docs/build/html/_static/custom.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8171 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.1/docs/build/html/_static/doctools.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      419 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.1/docs/build/html/_static/documentation_options.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   268039 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.1/docs/build/html/_static/jquery-3.2.1.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    89501 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.1/docs/build/html/_static/jquery.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4758 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.1/docs/build/html/_static/language_data.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4846 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.1/docs/build/html/_static/pygments.css
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17088 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.1/docs/build/html/_static/searchtools.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35168 2022-09-29 13:06:50.000000 mly_pipeline-0.3.1.1/docs/build/html/_static/underscore-1.3.1.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    19530 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.1/docs/build/html/_static/underscore.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    25355 2022-09-29 13:06:50.000000 mly_pipeline-0.3.1.1/docs/build/html/_static/websupport.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3121 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.1/docs/build/html/genindex.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22800 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.1/docs/build/html/gettingstarted.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17606 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.1/docs/build/html/howtouse.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7025 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.1/docs/build/html/index.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9665 2023-05-04 11:02:10.000000 mly_pipeline-0.3.1.1/docs/build/html/installation.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1490 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.1/docs/build/html/objects.inv
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3898 2022-09-29 13:06:50.000000 mly_pipeline-0.3.1.1/docs/build/html/py-modindex.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27021 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.1/docs/build/html/runningasearch.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3424 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.1/docs/build/html/search.html
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    21120 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.1/docs/build/html/searchindex.js
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    26724 2023-05-04 11:10:20.000000 mly_pipeline-0.3.1.1/docs/build/html/settingupasearch.html
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 10:04:43.294513 mly_pipeline-0.3.1.1/docs/source/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5971 2023-05-04 11:02:00.000000 mly_pipeline-0.3.1.1/docs/source/conf.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.1/docs/source/index.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2708 2023-05-04 11:22:06.000000 mly_pipeline-0.3.1.1/docs/source/installation.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14708 2023-05-04 11:18:26.000000 mly_pipeline-0.3.1.1/docs/source/runningasearch.rst
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13712 2023-05-04 11:10:15.000000 mly_pipeline-0.3.1.1/docs/source/settingupasearch.rst
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 10:04:43.320513 mly_pipeline-0.3.1.1/mly_pipeline/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      727 2023-05-10 09:44:52.000000 mly_pipeline-0.3.1.1/mly_pipeline/__init__.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    26455 2023-05-04 09:25:08.000000 mly_pipeline-0.3.1.1/mly_pipeline/continious_FAR.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    24615 2023-05-11 11:53:21.000000 mly_pipeline-0.3.1.1/mly_pipeline/initialization.py
--rwxrwxrwx   0 vasileios.skliris (44659) vasileios.skliris (44659)    13344 2023-05-10 09:57:38.000000 mly_pipeline-0.3.1.1/mly_pipeline/make_eff_estimation.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22791 2023-05-11 14:52:48.000000 mly_pipeline-0.3.1.1/mly_pipeline/manager.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5939 2023-04-14 10:51:44.000000 mly_pipeline-0.3.1.1/mly_pipeline/mly_to_grace.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    20321 2023-05-04 09:19:17.000000 mly_pipeline-0.3.1.1/mly_pipeline/offline_search.py
--rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    16260 2023-05-04 12:51:13.000000 mly_pipeline-0.3.1.1/mly_pipeline/search.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35533 2023-05-11 10:45:05.000000 mly_pipeline-0.3.1.1/mly_pipeline/search_functions.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 10:04:43.347514 mly_pipeline-0.3.1.1/mly_pipeline/tests/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      737 2023-05-10 09:14:51.000000 mly_pipeline-0.3.1.1/mly_pipeline/tests/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      663 2023-05-10 09:05:55.000000 mly_pipeline-0.3.1.1/mly_pipeline/tests/test_skymap_generation.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 10:04:43.336514 mly_pipeline-0.3.1.1/mly_pipeline.egg-info/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6683 2023-05-12 10:04:42.000000 mly_pipeline-0.3.1.1/mly_pipeline.egg-info/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2594 2023-05-12 10:04:43.000000 mly_pipeline-0.3.1.1/mly_pipeline.egg-info/SOURCES.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-05-12 10:04:42.000000 mly_pipeline-0.3.1.1/mly_pipeline.egg-info/dependency_links.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       71 2023-05-12 10:04:42.000000 mly_pipeline-0.3.1.1/mly_pipeline.egg-info/entry_points.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-05-12 10:04:42.000000 mly_pipeline-0.3.1.1/mly_pipeline.egg-info/requires.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       13 2023-05-12 10:04:42.000000 mly_pipeline-0.3.1.1/mly_pipeline.egg-info/top_level.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      631 2023-05-12 10:03:32.000000 mly_pipeline-0.3.1.1/pyproject.toml
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       38 2023-05-12 10:04:43.350514 mly_pipeline-0.3.1.1/setup.cfg
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 11:19:42.366246 mly_pipeline-0.3.1.2/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      101 2023-05-11 15:58:46.000000 mly_pipeline-0.3.1.2/.gitignore
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1691 2023-05-10 09:58:07.000000 mly_pipeline-0.3.1.2/.gitlab-ci.yml
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-10 08:55:08.000000 mly_pipeline-0.3.1.2/LICENSE
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6683 2023-05-12 11:19:42.365246 mly_pipeline-0.3.1.2/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6313 2022-03-23 16:00:11.000000 mly_pipeline-0.3.1.2/README.md
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 11:19:41.756240 mly_pipeline-0.3.1.2/docs/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      584 2022-09-29 13:06:48.000000 mly_pipeline-0.3.1.2/docs/Makefile
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 11:19:41.632239 mly_pipeline-0.3.1.2/docs/build/
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 11:19:42.056243 mly_pipeline-0.3.1.2/docs/build/doctrees/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    29429 2022-09-29 13:06:48.000000 mly_pipeline-0.3.1.2/docs/build/doctrees/HowToUse.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10289 2022-09-29 13:06:48.000000 mly_pipeline-0.3.1.2/docs/build/doctrees/Installation.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  2070494 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/doctrees/environment.pickle
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    62765 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/doctrees/gettingstarted.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    42039 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/doctrees/howtouse.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6320 2023-05-04 11:02:10.000000 mly_pipeline-0.3.1.2/docs/build/doctrees/index.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13735 2023-05-04 11:02:10.000000 mly_pipeline-0.3.1.2/docs/build/doctrees/installation.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    66958 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/doctrees/runningasearch.doctree
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    72638 2023-05-04 11:10:20.000000 mly_pipeline-0.3.1.2/docs/build/doctrees/settingupasearch.doctree
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 11:19:42.107244 mly_pipeline-0.3.1.2/docs/build/html/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9207 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/Getting Started.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9206 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/GettingStarted.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4601 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.2/docs/build/html/How to use.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17205 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/HowToUse.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8839 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/Installation.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 11:19:42.110244 mly_pipeline-0.3.1.2/docs/build/html/_modules/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3285 2023-04-26 10:02:39.000000 mly_pipeline-0.3.1.2/docs/build/html/_modules/index.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13865 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.2/docs/build/html/_modules/io.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 11:19:42.117244 mly_pipeline-0.3.1.2/docs/build/html/_sources/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      979 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.2/docs/build/html/_sources/How to use.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5555 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/_sources/HowToUse.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2490 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.2/docs/build/html/_sources/Installation.rst.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/_sources/index.rst.txt
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 11:19:42.212245 mly_pipeline-0.3.1.2/docs/build/html/_static/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      673 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/ajax-loader.gif
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    11185 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/alabaster.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    15205 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/basic.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9799 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/bizstyle.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1139 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/bizstyle.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14940 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/css3-mediaqueries.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28634 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/css3-mediaqueries_src.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       42 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/custom.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8171 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/doctools.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      419 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/documentation_options.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   268039 2022-09-29 13:06:49.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/jquery-3.2.1.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    89501 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/jquery.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4758 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/language_data.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4846 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/pygments.css
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17088 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/searchtools.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35168 2022-09-29 13:06:50.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/underscore-1.3.1.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    19530 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/underscore.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    25355 2022-09-29 13:06:50.000000 mly_pipeline-0.3.1.2/docs/build/html/_static/websupport.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3121 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/html/genindex.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22800 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/gettingstarted.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    17606 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/howtouse.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7025 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/html/index.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     9665 2023-05-04 11:02:10.000000 mly_pipeline-0.3.1.2/docs/build/html/installation.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1490 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/html/objects.inv
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3898 2022-09-29 13:06:50.000000 mly_pipeline-0.3.1.2/docs/build/html/py-modindex.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    27021 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/html/runningasearch.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3424 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/html/search.html
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    21120 2023-05-04 11:18:30.000000 mly_pipeline-0.3.1.2/docs/build/html/searchindex.js
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    26724 2023-05-04 11:10:20.000000 mly_pipeline-0.3.1.2/docs/build/html/settingupasearch.html
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 11:19:42.221245 mly_pipeline-0.3.1.2/docs/source/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5971 2023-05-04 11:02:00.000000 mly_pipeline-0.3.1.2/docs/source/conf.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      874 2023-02-20 18:02:10.000000 mly_pipeline-0.3.1.2/docs/source/index.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2708 2023-05-04 11:22:06.000000 mly_pipeline-0.3.1.2/docs/source/installation.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    14708 2023-05-04 11:18:26.000000 mly_pipeline-0.3.1.2/docs/source/runningasearch.rst
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13712 2023-05-04 11:10:15.000000 mly_pipeline-0.3.1.2/docs/source/settingupasearch.rst
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 11:19:42.237245 mly_pipeline-0.3.1.2/mly_pipeline/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      727 2023-05-10 09:44:52.000000 mly_pipeline-0.3.1.2/mly_pipeline/__init__.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    26455 2023-05-04 09:25:08.000000 mly_pipeline-0.3.1.2/mly_pipeline/continious_FAR.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    25296 2023-05-12 11:18:19.000000 mly_pipeline-0.3.1.2/mly_pipeline/initialization.py
+-rwxrwxrwx   0 vasileios.skliris (44659) vasileios.skliris (44659)    13344 2023-05-10 09:57:38.000000 mly_pipeline-0.3.1.2/mly_pipeline/make_eff_estimation.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22791 2023-05-11 14:52:48.000000 mly_pipeline-0.3.1.2/mly_pipeline/manager.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5939 2023-04-14 10:51:44.000000 mly_pipeline-0.3.1.2/mly_pipeline/mly_to_grace.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    20321 2023-05-04 09:19:17.000000 mly_pipeline-0.3.1.2/mly_pipeline/offline_search.py
+-rwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)    16260 2023-05-04 12:51:13.000000 mly_pipeline-0.3.1.2/mly_pipeline/search.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35533 2023-05-11 10:45:05.000000 mly_pipeline-0.3.1.2/mly_pipeline/search_functions.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 11:19:42.363246 mly_pipeline-0.3.1.2/mly_pipeline/tests/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      737 2023-05-10 09:14:51.000000 mly_pipeline-0.3.1.2/mly_pipeline/tests/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      663 2023-05-10 09:05:55.000000 mly_pipeline-0.3.1.2/mly_pipeline/tests/test_skymap_generation.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-05-12 11:19:42.244245 mly_pipeline-0.3.1.2/mly_pipeline.egg-info/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6683 2023-05-12 11:19:41.000000 mly_pipeline-0.3.1.2/mly_pipeline.egg-info/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     2594 2023-05-12 11:19:41.000000 mly_pipeline-0.3.1.2/mly_pipeline.egg-info/SOURCES.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-05-12 11:19:41.000000 mly_pipeline-0.3.1.2/mly_pipeline.egg-info/dependency_links.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      134 2023-05-12 11:19:41.000000 mly_pipeline-0.3.1.2/mly_pipeline.egg-info/entry_points.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-05-12 11:19:41.000000 mly_pipeline-0.3.1.2/mly_pipeline.egg-info/requires.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       13 2023-05-12 11:19:41.000000 mly_pipeline-0.3.1.2/mly_pipeline.egg-info/top_level.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      699 2023-05-12 11:19:24.000000 mly_pipeline-0.3.1.2/pyproject.toml
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       38 2023-05-12 11:19:42.366246 mly_pipeline-0.3.1.2/setup.cfg
```

### Comparing `mly_pipeline-0.3.1.1/.gitlab-ci.yml` & `mly_pipeline-0.3.1.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/LICENSE` & `mly_pipeline-0.3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/PKG-INFO` & `mly_pipeline-0.3.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mly_pipeline
-Version: 0.3.1.1
+Version: 0.3.1.2
 Summary: Search pipeline to run online and offline GW searches with mly package.
 Author-email: Vasileios SKliris <sklirisv@cardiff.ac.uk>
 Keywords: ml,gravitational waves,bursts
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mly_pipeline-0.3.1.1/README.md` & `mly_pipeline-0.3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/Makefile` & `mly_pipeline-0.3.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/doctrees/HowToUse.doctree` & `mly_pipeline-0.3.1.2/docs/build/doctrees/HowToUse.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/doctrees/Installation.doctree` & `mly_pipeline-0.3.1.2/docs/build/doctrees/Installation.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/doctrees/environment.pickle` & `mly_pipeline-0.3.1.2/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/doctrees/gettingstarted.doctree` & `mly_pipeline-0.3.1.2/docs/build/doctrees/gettingstarted.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/doctrees/howtouse.doctree` & `mly_pipeline-0.3.1.2/docs/build/doctrees/howtouse.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/doctrees/index.doctree` & `mly_pipeline-0.3.1.2/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/doctrees/installation.doctree` & `mly_pipeline-0.3.1.2/docs/build/doctrees/installation.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/doctrees/runningasearch.doctree` & `mly_pipeline-0.3.1.2/docs/build/doctrees/runningasearch.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/doctrees/settingupasearch.doctree` & `mly_pipeline-0.3.1.2/docs/build/doctrees/settingupasearch.doctree`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/Getting Started.html` & `mly_pipeline-0.3.1.2/docs/build/html/Getting Started.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/GettingStarted.html` & `mly_pipeline-0.3.1.2/docs/build/html/GettingStarted.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/How to use.html` & `mly_pipeline-0.3.1.2/docs/build/html/How to use.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/HowToUse.html` & `mly_pipeline-0.3.1.2/docs/build/html/HowToUse.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/Installation.html` & `mly_pipeline-0.3.1.2/docs/build/html/Installation.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/_modules/index.html` & `mly_pipeline-0.3.1.2/docs/build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/_modules/io.html` & `mly_pipeline-0.3.1.2/docs/build/html/_modules/io.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/_sources/How to use.rst.txt` & `mly_pipeline-0.3.1.2/docs/build/html/_sources/How to use.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/_sources/HowToUse.rst.txt` & `mly_pipeline-0.3.1.2/docs/build/html/_sources/HowToUse.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/_sources/Installation.rst.txt` & `mly_pipeline-0.3.1.2/docs/build/html/_sources/Installation.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/_sources/index.rst.txt` & `mly_pipeline-0.3.1.2/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/_static/ajax-loader.gif` & `mly_pipeline-0.3.1.2/docs/build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/_static/alabaster.css` & `mly_pipeline-0.3.1.2/docs/build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/_static/basic.css` & `mly_pipeline-0.3.1.2/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/_static/bizstyle.css` & `mly_pipeline-0.3.1.2/docs/build/html/_static/bizstyle.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/_static/bizstyle.js` & `mly_pipeline-0.3.1.2/docs/build/html/_static/bizstyle.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/_static/css3-mediaqueries.js` & `mly_pipeline-0.3.1.2/docs/build/html/_static/css3-mediaqueries.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/_static/css3-mediaqueries_src.js` & `mly_pipeline-0.3.1.2/docs/build/html/_static/css3-mediaqueries_src.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/_static/doctools.js` & `mly_pipeline-0.3.1.2/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/_static/jquery-3.2.1.js` & `mly_pipeline-0.3.1.2/docs/build/html/_static/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/_static/jquery.js` & `mly_pipeline-0.3.1.2/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/_static/language_data.js` & `mly_pipeline-0.3.1.2/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/_static/pygments.css` & `mly_pipeline-0.3.1.2/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/_static/searchtools.js` & `mly_pipeline-0.3.1.2/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/_static/underscore-1.3.1.js` & `mly_pipeline-0.3.1.2/docs/build/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/_static/underscore.js` & `mly_pipeline-0.3.1.2/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/_static/websupport.js` & `mly_pipeline-0.3.1.2/docs/build/html/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/genindex.html` & `mly_pipeline-0.3.1.2/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/gettingstarted.html` & `mly_pipeline-0.3.1.2/docs/build/html/gettingstarted.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/howtouse.html` & `mly_pipeline-0.3.1.2/docs/build/html/howtouse.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/index.html` & `mly_pipeline-0.3.1.2/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/installation.html` & `mly_pipeline-0.3.1.2/docs/build/html/installation.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/objects.inv` & `mly_pipeline-0.3.1.2/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/py-modindex.html` & `mly_pipeline-0.3.1.2/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/runningasearch.html` & `mly_pipeline-0.3.1.2/docs/build/html/runningasearch.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/search.html` & `mly_pipeline-0.3.1.2/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/searchindex.js` & `mly_pipeline-0.3.1.2/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/build/html/settingupasearch.html` & `mly_pipeline-0.3.1.2/docs/build/html/settingupasearch.html`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/source/conf.py` & `mly_pipeline-0.3.1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/source/index.rst` & `mly_pipeline-0.3.1.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/source/installation.rst` & `mly_pipeline-0.3.1.2/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/source/runningasearch.rst` & `mly_pipeline-0.3.1.2/docs/source/runningasearch.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/docs/source/settingupasearch.rst` & `mly_pipeline-0.3.1.2/docs/source/settingupasearch.rst`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/mly_pipeline/__init__.py` & `mly_pipeline-0.3.1.2/mly_pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/mly_pipeline/continious_FAR.py` & `mly_pipeline-0.3.1.2/mly_pipeline/continious_FAR.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/mly_pipeline/initialization.py` & `mly_pipeline-0.3.1.2/mly_pipeline/initialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -562,15 +562,41 @@
     # Saving config file to json format
     with open(configuration['path'] +"/"+"config.json", "w") as config_json:
         json.dump(configuration, config_json,indent=4)
         config_json.close()
 
     
     createRunAllScript(**configuration)
-        
+
+def _start_search():
+
+    #Construct argument parser:
+    parser = argparse.ArgumentParser()
+
+    parser.add_argument('-p', '--search_path', type=str
+                        , default = "./"
+                        , help = "The path to the search to start"
+                        , required = False)
+
+    # Pass arguments:
+    args = parser.parse_args()
+    
+
+    search_path = getattr(args, "search_path")      
+
+    if os.path.isfile(search_path+"runall.sh"):
+
+        os.system(f"nohup sh {search_path}runall.sh &> {search_path}runall.out &")
+
+    else:
+
+        raise FileNotFoundError(f"The path provided {search_path} does not have a runall.sh file to start the search.")
+
+      
         
         
 if __name__ == "__main__":
     
      main()
 
 
+
```

### Comparing `mly_pipeline-0.3.1.1/mly_pipeline/make_eff_estimation.py` & `mly_pipeline-0.3.1.2/mly_pipeline/make_eff_estimation.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/mly_pipeline/manager.py` & `mly_pipeline-0.3.1.2/mly_pipeline/manager.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/mly_pipeline/mly_to_grace.py` & `mly_pipeline-0.3.1.2/mly_pipeline/mly_to_grace.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/mly_pipeline/offline_search.py` & `mly_pipeline-0.3.1.2/mly_pipeline/offline_search.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/mly_pipeline/search.py` & `mly_pipeline-0.3.1.2/mly_pipeline/search.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/mly_pipeline/search_functions.py` & `mly_pipeline-0.3.1.2/mly_pipeline/search_functions.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/mly_pipeline/tests/__init__.py` & `mly_pipeline-0.3.1.2/mly_pipeline/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/mly_pipeline/tests/test_skymap_generation.py` & `mly_pipeline-0.3.1.2/mly_pipeline/tests/test_skymap_generation.py`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/mly_pipeline.egg-info/PKG-INFO` & `mly_pipeline-0.3.1.2/mly_pipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mly-pipeline
-Version: 0.3.1.1
+Version: 0.3.1.2
 Summary: Search pipeline to run online and offline GW searches with mly package.
 Author-email: Vasileios SKliris <sklirisv@cardiff.ac.uk>
 Keywords: ml,gravitational waves,bursts
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mly_pipeline-0.3.1.1/mly_pipeline.egg-info/SOURCES.txt` & `mly_pipeline-0.3.1.2/mly_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mly_pipeline-0.3.1.1/pyproject.toml` & `mly_pipeline-0.3.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>61", "setuptools-scm>=3.4.3", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mly_pipeline"
-version = "0.3.1.1"
+version = "0.3.1.2"
 authors = [
     {name = "Vasileios SKliris", email = "sklirisv@cardiff.ac.uk"},
 ]
 description = "Search pipeline to run online and offline GW searches with mly package."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["ml", "gravitational waves", "bursts"]
@@ -17,8 +17,11 @@
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "mly"
 ]
 
 [project.scripts]
-mly-pipeline-init = "mly_pipeline.initialization:main"
+mly-pipeline-init = "mly_pipeline.initialization:main"
+mly-pipeline-start = "mly_pipeline.initialization:_start_search"
+
+
```


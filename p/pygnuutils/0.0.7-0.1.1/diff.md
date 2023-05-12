# Comparing `tmp/pygnuutils-0.0.7.tar.gz` & `tmp/pygnuutils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygnuutils-0.0.7.tar", last modified: Sat Apr 22 21:14:31 2023, max compression
+gzip compressed data, was "pygnuutils-0.1.1.tar", last modified: Fri May 12 12:56:47 2023, max compression
```

## Comparing `pygnuutils-0.0.7.tar` & `pygnuutils-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:14:31.565856 pygnuutils-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-22 21:14:31.565856 pygnuutils-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:14:31.561856 pygnuutils-0.0.7/pygnuutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/basename.py
--rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/basenc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:14:31.565856 pygnuutils-0.0.7/pygnuutils/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/cli/basename.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/cli/basenc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/cli/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/cli/yes.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/filevercmp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/human_readable.py
--rw-r--r--   0 runner    (1001) docker     (123)    39147 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/pygnuutils/yes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:14:31.565856 pygnuutils-0.0.7/pygnuutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-22 21:14:31.000000 pygnuutils-0.0.7/pygnuutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-22 21:14:31.000000 pygnuutils-0.0.7/pygnuutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 21:14:31.000000 pygnuutils-0.0.7/pygnuutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-22 21:14:31.000000 pygnuutils-0.0.7/pygnuutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-22 21:14:31.000000 pygnuutils-0.0.7/pygnuutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-22 21:14:31.000000 pygnuutils-0.0.7/pygnuutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 21:14:31.565856 pygnuutils-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-22 21:14:16.000000 pygnuutils-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:56:47.662999 pygnuutils-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-12 12:56:21.000000 pygnuutils-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43096 2023-05-12 12:56:47.662999 pygnuutils-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-12 12:56:21.000000 pygnuutils-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:56:47.658999 pygnuutils-0.1.1/pygnuutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 12:56:21.000000 pygnuutils-0.1.1/pygnuutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-12 12:56:21.000000 pygnuutils-0.1.1/pygnuutils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-12 12:56:21.000000 pygnuutils-0.1.1/pygnuutils/basename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-05-12 12:56:21.000000 pygnuutils-0.1.1/pygnuutils/basenc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:56:47.662999 pygnuutils-0.1.1/pygnuutils/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 12:56:21.000000 pygnuutils-0.1.1/pygnuutils/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-12 12:56:21.000000 pygnuutils-0.1.1/pygnuutils/cli/basename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-12 12:56:21.000000 pygnuutils-0.1.1/pygnuutils/cli/basenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-05-12 12:56:21.000000 pygnuutils-0.1.1/pygnuutils/cli/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-12 12:56:21.000000 pygnuutils-0.1.1/pygnuutils/cli/yes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-12 12:56:21.000000 pygnuutils-0.1.1/pygnuutils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-12 12:56:21.000000 pygnuutils-0.1.1/pygnuutils/filevercmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-05-12 12:56:21.000000 pygnuutils-0.1.1/pygnuutils/human_readable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39147 2023-05-12 12:56:21.000000 pygnuutils-0.1.1/pygnuutils/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-12 12:56:21.000000 pygnuutils-0.1.1/pygnuutils/yes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:56:47.662999 pygnuutils-0.1.1/pygnuutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43096 2023-05-12 12:56:47.000000 pygnuutils-0.1.1/pygnuutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-12 12:56:47.000000 pygnuutils-0.1.1/pygnuutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 12:56:47.000000 pygnuutils-0.1.1/pygnuutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-12 12:56:47.000000 pygnuutils-0.1.1/pygnuutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-12 12:56:47.000000 pygnuutils-0.1.1/pygnuutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-12 12:56:47.000000 pygnuutils-0.1.1/pygnuutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-12 12:56:21.000000 pygnuutils-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-12 12:56:21.000000 pygnuutils-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 12:56:47.662999 pygnuutils-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:56:47.662999 pygnuutils-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-12 12:56:21.000000 pygnuutils-0.1.1/tests/test_basename.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-05-12 12:56:21.000000 pygnuutils-0.1.1/tests/test_basenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-12 12:56:21.000000 pygnuutils-0.1.1/tests/test_filevercmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-12 12:56:21.000000 pygnuutils-0.1.1/tests/test_human_readable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15157 2023-05-12 12:56:21.000000 pygnuutils-0.1.1/tests/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-12 12:56:21.000000 pygnuutils-0.1.1/tests/test_yes.py
```

### Comparing `pygnuutils-0.0.7/LICENSE` & `pygnuutils-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygnuutils-0.0.7/PKG-INFO` & `pygnuutils-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,9 @@
-Metadata-Version: 2.1
-Name: pygnuutils
-Version: 0.0.7
-Summary: A python implementation for GNU utils
-Home-page: https://github.com/matan1008/pygnuutils
-Author: Matan Perelman
-Project-URL: pygnuutils, https://github.com/matan1008/pygnuutils
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Python application](https://github.com/matan1008/pygnuutils/workflows/Python%20application/badge.svg)](https://github.com/matan1008/pygnuutils/actions/workflows/python-app.yml "Python application action")
 [![Pypi version](https://img.shields.io/pypi/v/pygnuutils.svg)](https://pypi.org/project/pygnuutils/ "PyPi package")
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/matan1008/pygnuutils.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/matan1008/pygnuutils/context:python)
 
 - [Description](#description)
 - [Installation](#installation)
 - [Usage](#usage)
     * [CLI](#cli)
     * [Python](#python)
```

### Comparing `pygnuutils-0.0.7/pygnuutils/basename.py` & `pygnuutils-0.1.1/pygnuutils/basename.py`

 * *Files identical despite different names*

### Comparing `pygnuutils-0.0.7/pygnuutils/basenc.py` & `pygnuutils-0.1.1/pygnuutils/basenc.py`

 * *Files identical despite different names*

### Comparing `pygnuutils-0.0.7/pygnuutils/cli/basenc.py` & `pygnuutils-0.1.1/pygnuutils/cli/basenc.py`

 * *Files identical despite different names*

### Comparing `pygnuutils-0.0.7/pygnuutils/cli/ls.py` & `pygnuutils-0.1.1/pygnuutils/cli/ls.py`

 * *Files identical despite different names*

### Comparing `pygnuutils-0.0.7/pygnuutils/filevercmp.py` & `pygnuutils-0.1.1/pygnuutils/filevercmp.py`

 * *Files identical despite different names*

### Comparing `pygnuutils-0.0.7/pygnuutils/human_readable.py` & `pygnuutils-0.1.1/pygnuutils/human_readable.py`

 * *Files identical despite different names*

### Comparing `pygnuutils-0.0.7/pygnuutils/ls.py` & `pygnuutils-0.1.1/pygnuutils/ls.py`

 * *Files identical despite different names*

### Comparing `pygnuutils-0.0.7/pygnuutils/yes.py` & `pygnuutils-0.1.1/pygnuutils/yes.py`

 * *Files identical despite different names*


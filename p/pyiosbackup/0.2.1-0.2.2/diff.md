# Comparing `tmp/pyiosbackup-0.2.1.tar.gz` & `tmp/pyiosbackup-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiosbackup-0.2.1.tar", last modified: Mon Apr 24 05:41:33 2023, max compression
+gzip compressed data, was "pyiosbackup-0.2.2.tar", last modified: Fri May 12 10:49:23 2023, max compression
```

## Comparing `pyiosbackup-0.2.1.tar` & `pyiosbackup-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:41:33.738164 pyiosbackup-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-24 05:41:33.738164 pyiosbackup-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:41:33.738164 pyiosbackup-0.2.1/pyiosbackup/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/pyiosbackup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/pyiosbackup/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/pyiosbackup/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/pyiosbackup/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/pyiosbackup/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/pyiosbackup/keybag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:41:33.738164 pyiosbackup-0.2.1/pyiosbackup/manifest_dbs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/pyiosbackup/manifest_dbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/pyiosbackup/manifest_dbs/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/pyiosbackup/manifest_dbs/manifest_db_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/pyiosbackup/manifest_dbs/mbdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/pyiosbackup/manifest_dbs/sqlite3.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/pyiosbackup/manifest_plist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:41:33.738164 pyiosbackup-0.2.1/pyiosbackup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-24 05:41:33.000000 pyiosbackup-0.2.1/pyiosbackup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-24 05:41:33.000000 pyiosbackup-0.2.1/pyiosbackup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 05:41:33.000000 pyiosbackup-0.2.1/pyiosbackup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-24 05:41:33.000000 pyiosbackup-0.2.1/pyiosbackup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-24 05:41:33.000000 pyiosbackup-0.2.1/pyiosbackup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 05:41:33.000000 pyiosbackup-0.2.1/pyiosbackup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 05:41:33.738164 pyiosbackup-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-24 05:41:17.000000 pyiosbackup-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:49:23.419187 pyiosbackup-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43919 2023-05-12 10:49:23.419187 pyiosbackup-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:49:23.419187 pyiosbackup-0.2.2/pyiosbackup/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyiosbackup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyiosbackup/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyiosbackup/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyiosbackup/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyiosbackup/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyiosbackup/keybag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:49:23.419187 pyiosbackup-0.2.2/pyiosbackup/manifest_dbs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyiosbackup/manifest_dbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyiosbackup/manifest_dbs/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyiosbackup/manifest_dbs/manifest_db_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyiosbackup/manifest_dbs/mbdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyiosbackup/manifest_dbs/sqlite3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyiosbackup/manifest_plist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:49:23.419187 pyiosbackup-0.2.2/pyiosbackup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43919 2023-05-12 10:49:23.000000 pyiosbackup-0.2.2/pyiosbackup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-12 10:49:23.000000 pyiosbackup-0.2.2/pyiosbackup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:49:23.000000 pyiosbackup-0.2.2/pyiosbackup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-12 10:49:23.000000 pyiosbackup-0.2.2/pyiosbackup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-12 10:49:23.000000 pyiosbackup-0.2.2/pyiosbackup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-12 10:49:23.000000 pyiosbackup-0.2.2/pyiosbackup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 10:49:23.419187 pyiosbackup-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:49:23.419187 pyiosbackup-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/tests/test_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-12 10:49:03.000000 pyiosbackup-0.2.2/tests/test_keybag.py
```

### Comparing `pyiosbackup-0.2.1/LICENSE` & `pyiosbackup-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.1/PKG-INFO` & `pyiosbackup-0.2.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,9 @@
-Metadata-Version: 2.1
-Name: pyiosbackup
-Version: 0.2.1
-Summary: A python parser for iOS backups
-Home-page: https://github.com/matan1008/pyiosbackup
-Author: Matan Perelman
-Project-URL: pyiosbackup, https://github.com/matan1008/pyiosbackup
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Python application](https://github.com/matan1008/pyiosbackup/workflows/Python%20application/badge.svg)](https://github.com/matan1008/pyiosbackup/actions/workflows/python-app.yml "Python application action")
 [![Pypi version](https://img.shields.io/pypi/v/pyiosbackup.svg)](https://pypi.org/project/pyiosbackup/ "PyPi package")
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/matan1008/pyiosbackup.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/matan1008/pyiosbackup/context:python)
 
 - [Description](#description)
 - [Installation](#installation)
 - [Usage](#usage)
     * [CLI](#cli)
     * [Python](#python)
```

### Comparing `pyiosbackup-0.2.1/pyiosbackup/__main__.py` & `pyiosbackup-0.2.2/pyiosbackup/__main__.py`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.1/pyiosbackup/backup.py` & `pyiosbackup-0.2.2/pyiosbackup/backup.py`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.1/pyiosbackup/entry.py` & `pyiosbackup-0.2.2/pyiosbackup/entry.py`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.1/pyiosbackup/keybag.py` & `pyiosbackup-0.2.2/pyiosbackup/keybag.py`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.1/pyiosbackup/manifest_dbs/factory.py` & `pyiosbackup-0.2.2/pyiosbackup/manifest_dbs/factory.py`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.1/pyiosbackup/manifest_dbs/manifest_db_interface.py` & `pyiosbackup-0.2.2/pyiosbackup/manifest_dbs/manifest_db_interface.py`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.1/pyiosbackup/manifest_dbs/mbdb.py` & `pyiosbackup-0.2.2/pyiosbackup/manifest_dbs/mbdb.py`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.1/pyiosbackup/manifest_dbs/sqlite3.py` & `pyiosbackup-0.2.2/pyiosbackup/manifest_dbs/sqlite3.py`

 * *Files identical despite different names*

### Comparing `pyiosbackup-0.2.1/pyiosbackup/manifest_plist.py` & `pyiosbackup-0.2.2/pyiosbackup/manifest_plist.py`

 * *Files identical despite different names*


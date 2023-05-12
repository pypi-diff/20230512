# Comparing `tmp/alcli-1.0.8.tar.gz` & `tmp/alcli-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alcli-1.0.8.tar", last modified: Mon Feb 24 17:02:28 2020, max compression
+gzip compressed data, was "dist/alcli-1.0.9.tar", last modified: Mon Feb 24 17:19:10 2020, max compression
```

## Comparing `alcli-1.0.8.tar` & `alcli-1.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 pavel    (746587408) staff       (20)        0 2020-02-24 17:02:28.000000 alcli-1.0.8/
--rw-r--r--   0 pavel    (746587408) staff       (20)      168 2020-02-06 20:11:20.000000 alcli-1.0.8/AUTHORS.rst
--rw-r--r--   0 pavel    (746587408) staff       (20)      178 2020-02-07 23:16:06.000000 alcli-1.0.8/HISTORY.rst
--rw-r--r--   0 pavel    (746587408) staff       (20)     1076 2020-02-06 20:11:20.000000 alcli-1.0.8/LICENSE
--rw-r--r--   0 pavel    (746587408) staff       (20)       74 2020-02-06 20:11:20.000000 alcli-1.0.8/MANIFEST.in
--rw-r--r--   0 pavel    (746587408) staff       (20)     3085 2020-02-24 17:02:28.000000 alcli-1.0.8/PKG-INFO
--rw-r--r--   0 pavel    (746587408) staff       (20)     2002 2020-02-07 23:16:06.000000 alcli-1.0.8/README.md
-drwxr-xr-x   0 pavel    (746587408) staff       (20)        0 2020-02-24 17:02:28.000000 alcli-1.0.8/alcli/
--rw-r--r--   0 pavel    (746587408) staff       (20)       55 2020-02-24 16:59:12.000000 alcli-1.0.8/alcli/__init__.py
--rw-r--r--   0 pavel    (746587408) staff       (20)     8333 2020-02-24 16:58:49.000000 alcli-1.0.8/alcli/alertlogic_cli.py
--rw-r--r--   0 pavel    (746587408) staff       (20)     3288 2020-01-26 23:10:20.000000 alcli-1.0.8/alcli/argparser.py
--rw-r--r--   0 pavel    (746587408) staff       (20)      474 2020-01-12 01:10:39.000000 alcli-1.0.8/alcli/arguments.py
--rw-r--r--   0 pavel    (746587408) staff       (20)     7033 2020-02-24 16:10:17.000000 alcli-1.0.8/alcli/clihelp.py
--rw-r--r--   0 pavel    (746587408) staff       (20)     5782 2020-01-28 23:39:43.000000 alcli-1.0.8/alcli/cliparser.py
-drwxr-xr-x   0 pavel    (746587408) staff       (20)        0 2020-02-24 17:02:28.000000 alcli-1.0.8/alcli.egg-info/
--rw-r--r--   0 pavel    (746587408) staff       (20)     3085 2020-02-24 17:02:28.000000 alcli-1.0.8/alcli.egg-info/PKG-INFO
--rw-r--r--   0 pavel    (746587408) staff       (20)      392 2020-02-24 17:02:28.000000 alcli-1.0.8/alcli.egg-info/SOURCES.txt
--rw-r--r--   0 pavel    (746587408) staff       (20)        1 2020-02-24 17:02:28.000000 alcli-1.0.8/alcli.egg-info/dependency_links.txt
--rw-r--r--   0 pavel    (746587408) staff       (20)       53 2020-02-24 17:02:28.000000 alcli-1.0.8/alcli.egg-info/entry_points.txt
--rw-r--r--   0 pavel    (746587408) staff       (20)        1 2020-01-16 19:05:17.000000 alcli-1.0.8/alcli.egg-info/not-zip-safe
--rw-r--r--   0 pavel    (746587408) staff       (20)      145 2020-02-24 17:02:28.000000 alcli-1.0.8/alcli.egg-info/requires.txt
--rw-r--r--   0 pavel    (746587408) staff       (20)        6 2020-02-24 17:02:28.000000 alcli-1.0.8/alcli.egg-info/top_level.txt
--rw-r--r--   0 pavel    (746587408) staff       (20)      175 2020-02-24 17:02:28.000000 alcli-1.0.8/setup.cfg
--rw-r--r--   0 pavel    (746587408) staff       (20)     1490 2020-02-24 16:59:41.000000 alcli-1.0.8/setup.py
+drwxr-xr-x   0 pavel    (746587408) staff       (20)        0 2020-02-24 17:19:10.000000 alcli-1.0.9/
+-rw-r--r--   0 pavel    (746587408) staff       (20)      168 2020-02-06 20:11:20.000000 alcli-1.0.9/AUTHORS.rst
+-rw-r--r--   0 pavel    (746587408) staff       (20)      178 2020-02-07 23:16:06.000000 alcli-1.0.9/HISTORY.rst
+-rw-r--r--   0 pavel    (746587408) staff       (20)     1076 2020-02-06 20:11:20.000000 alcli-1.0.9/LICENSE
+-rw-r--r--   0 pavel    (746587408) staff       (20)       74 2020-02-06 20:11:20.000000 alcli-1.0.9/MANIFEST.in
+-rw-r--r--   0 pavel    (746587408) staff       (20)     3085 2020-02-24 17:19:10.000000 alcli-1.0.9/PKG-INFO
+-rw-r--r--   0 pavel    (746587408) staff       (20)     2002 2020-02-07 23:16:06.000000 alcli-1.0.9/README.md
+drwxr-xr-x   0 pavel    (746587408) staff       (20)        0 2020-02-24 17:19:10.000000 alcli-1.0.9/alcli/
+-rw-r--r--   0 pavel    (746587408) staff       (20)       55 2020-02-24 17:17:58.000000 alcli-1.0.9/alcli/__init__.py
+-rw-r--r--   0 pavel    (746587408) staff       (20)     8333 2020-02-24 16:58:49.000000 alcli-1.0.9/alcli/alertlogic_cli.py
+-rw-r--r--   0 pavel    (746587408) staff       (20)     3288 2020-01-26 23:10:20.000000 alcli-1.0.9/alcli/argparser.py
+-rw-r--r--   0 pavel    (746587408) staff       (20)      474 2020-01-12 01:10:39.000000 alcli-1.0.9/alcli/arguments.py
+-rw-r--r--   0 pavel    (746587408) staff       (20)     7033 2020-02-24 16:10:17.000000 alcli-1.0.9/alcli/clihelp.py
+-rw-r--r--   0 pavel    (746587408) staff       (20)     5782 2020-01-28 23:39:43.000000 alcli-1.0.9/alcli/cliparser.py
+drwxr-xr-x   0 pavel    (746587408) staff       (20)        0 2020-02-24 17:19:10.000000 alcli-1.0.9/alcli.egg-info/
+-rw-r--r--   0 pavel    (746587408) staff       (20)     3085 2020-02-24 17:19:10.000000 alcli-1.0.9/alcli.egg-info/PKG-INFO
+-rw-r--r--   0 pavel    (746587408) staff       (20)      392 2020-02-24 17:19:10.000000 alcli-1.0.9/alcli.egg-info/SOURCES.txt
+-rw-r--r--   0 pavel    (746587408) staff       (20)        1 2020-02-24 17:19:10.000000 alcli-1.0.9/alcli.egg-info/dependency_links.txt
+-rw-r--r--   0 pavel    (746587408) staff       (20)       53 2020-02-24 17:19:10.000000 alcli-1.0.9/alcli.egg-info/entry_points.txt
+-rw-r--r--   0 pavel    (746587408) staff       (20)        1 2020-02-24 17:19:10.000000 alcli-1.0.9/alcli.egg-info/not-zip-safe
+-rw-r--r--   0 pavel    (746587408) staff       (20)      145 2020-02-24 17:19:10.000000 alcli-1.0.9/alcli.egg-info/requires.txt
+-rw-r--r--   0 pavel    (746587408) staff       (20)        6 2020-02-24 17:19:10.000000 alcli-1.0.9/alcli.egg-info/top_level.txt
+-rw-r--r--   0 pavel    (746587408) staff       (20)      175 2020-02-24 17:19:10.000000 alcli-1.0.9/setup.cfg
+-rw-r--r--   0 pavel    (746587408) staff       (20)     1490 2020-02-24 16:59:41.000000 alcli-1.0.9/setup.py
```

### Comparing `alcli-1.0.8/LICENSE` & `alcli-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alcli-1.0.8/PKG-INFO` & `alcli-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alcli
-Version: 1.0.8
+Version: 1.0.9
 Summary: The Alert Logic Command Line Utility (CLI).
 Home-page: https://github.com/alertlogic/alcli
 Author: Alert Logic Inc.
 Author-email: support@alertlogic.com
 License: MIT
 Description: # Installing the Alert Logic CLI
         The `pip` package manager for Python is used to install, upgrade and remove Alert Logic CLI.
```

### Comparing `alcli-1.0.8/README.md` & `alcli-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alcli-1.0.8/alcli/alertlogic_cli.py` & `alcli-1.0.9/alcli/alertlogic_cli.py`

 * *Files identical despite different names*

### Comparing `alcli-1.0.8/alcli/argparser.py` & `alcli-1.0.9/alcli/argparser.py`

 * *Files identical despite different names*

### Comparing `alcli-1.0.8/alcli/clihelp.py` & `alcli-1.0.9/alcli/clihelp.py`

 * *Files identical despite different names*

### Comparing `alcli-1.0.8/alcli/cliparser.py` & `alcli-1.0.9/alcli/cliparser.py`

 * *Files identical despite different names*

### Comparing `alcli-1.0.8/alcli.egg-info/PKG-INFO` & `alcli-1.0.9/alcli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alcli
-Version: 1.0.8
+Version: 1.0.9
 Summary: The Alert Logic Command Line Utility (CLI).
 Home-page: https://github.com/alertlogic/alcli
 Author: Alert Logic Inc.
 Author-email: support@alertlogic.com
 License: MIT
 Description: # Installing the Alert Logic CLI
         The `pip` package manager for Python is used to install, upgrade and remove Alert Logic CLI.
```

### Comparing `alcli-1.0.8/setup.py` & `alcli-1.0.9/setup.py`

 * *Files identical despite different names*


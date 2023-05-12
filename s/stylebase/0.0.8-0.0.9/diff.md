# Comparing `tmp/stylebase-0.0.8.tar.gz` & `tmp/stylebase-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stylebase-0.0.8.tar", last modified: Mon Jul 19 18:53:50 2021, max compression
+gzip compressed data, was "dist/stylebase-0.0.9.tar", last modified: Mon Jul 19 19:30:06 2021, max compression
```

## Comparing `stylebase-0.0.8.tar` & `stylebase-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2021-07-19 18:53:50.563826 stylebase-0.0.8/
--rw-r-----   0 alex      (1002) alex      (1003)     1075 2021-02-02 12:38:23.000000 stylebase-0.0.8/LICENSE
--rw-rw-r--   0 alex      (1002) alex      (1003)       72 2021-05-28 16:59:49.000000 stylebase-0.0.8/MANIFEST.in
--rw-rw-r--   0 alex      (1002) alex      (1003)      611 2021-07-19 18:53:50.563826 stylebase-0.0.8/PKG-INFO
--rw-r-----   0 alex      (1002) alex      (1003)        0 2021-05-20 09:49:50.000000 stylebase-0.0.8/README.md
--rw-rw-r--   0 alex      (1002) alex      (1003)        5 2021-07-19 18:33:44.000000 stylebase-0.0.8/VERSION
--rw-rw-r--   0 alex      (1002) alex      (1003)      100 2021-02-14 09:34:02.000000 stylebase-0.0.8/pyproject.toml
--rw-rw-r--   0 alex      (1002) alex      (1003)      800 2021-07-19 18:53:50.567826 stylebase-0.0.8/setup.cfg
--rw-rw-r--   0 alex      (1002) alex      (1003)       70 2021-02-14 09:31:37.000000 stylebase-0.0.8/setup.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2021-07-19 18:53:50.555826 stylebase-0.0.8/stylebase/
--rw-rw-r--   0 alex      (1002) alex      (1003)    18441 2021-05-27 08:29:22.000000 stylebase-0.0.8/stylebase/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)      103 2021-05-28 20:52:35.000000 stylebase-0.0.8/stylebase/__main__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2021-07-19 18:53:50.559826 stylebase-0.0.8/stylebase/hooking/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2021-06-08 08:04:35.000000 stylebase-0.0.8/stylebase/hooking/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)      449 2021-06-08 08:04:36.000000 stylebase-0.0.8/stylebase/hooking/ante_build_hook.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     4678 2021-06-08 08:04:36.000000 stylebase-0.0.8/stylebase/hooking/ante_release_hook.py
--rw-rw-r--   0 alex      (1002) alex      (1003)      449 2021-06-08 08:04:36.000000 stylebase-0.0.8/stylebase/hooking/post_build_hook.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     2175 2021-06-08 08:04:36.000000 stylebase-0.0.8/stylebase/hooking/post_release_hook.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2021-07-19 18:53:50.563826 stylebase-0.0.8/stylebase/pyrustic_data/
--rw-rw-r--   0 alex      (1002) alex      (1003)      137 2021-07-19 18:33:40.000000 stylebase-0.0.8/stylebase/pyrustic_data/build_report.json
--rw-rw-r--   0 alex      (1002) alex      (1003)      294 2021-06-10 17:27:27.000000 stylebase-0.0.8/stylebase/pyrustic_data/hooking.json
--rw-rw-r--   0 alex      (1002) alex      (1003)      166 2021-06-10 17:27:27.000000 stylebase-0.0.8/stylebase/pyrustic_data/hubstore.json
--rw-rw-r--   0 alex      (1002) alex      (1003)      419 2021-07-19 18:33:56.000000 stylebase-0.0.8/stylebase/pyrustic_data/release_info.json
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2021-07-19 18:53:50.559826 stylebase-0.0.8/stylebase.egg-info/
--rw-rw-r--   0 alex      (1002) alex      (1003)      611 2021-07-19 18:53:50.000000 stylebase-0.0.8/stylebase.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1002) alex      (1003)      674 2021-07-19 18:53:50.000000 stylebase-0.0.8/stylebase.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)        1 2021-07-19 18:53:50.000000 stylebase-0.0.8/stylebase.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)       55 2021-07-19 18:53:50.000000 stylebase-0.0.8/stylebase.egg-info/entry_points.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)        1 2021-05-27 17:09:13.000000 stylebase-0.0.8/stylebase.egg-info/not-zip-safe
--rw-rw-r--   0 alex      (1002) alex      (1003)       16 2021-07-19 18:53:50.000000 stylebase-0.0.8/stylebase.egg-info/top_level.txt
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2021-07-19 18:53:50.563826 stylebase-0.0.8/tests/
--rw-r-----   0 alex      (1002) alex      (1003)        0 2020-05-31 07:38:19.000000 stylebase-0.0.8/tests/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2021-07-19 19:30:06.951817 stylebase-0.0.9/
+-rw-r-----   0 alex      (1002) alex      (1003)     1075 2021-02-02 12:38:23.000000 stylebase-0.0.9/LICENSE
+-rw-rw-r--   0 alex      (1002) alex      (1003)       72 2021-05-28 16:59:49.000000 stylebase-0.0.9/MANIFEST.in
+-rw-rw-r--   0 alex      (1002) alex      (1003)      611 2021-07-19 19:30:06.951817 stylebase-0.0.9/PKG-INFO
+-rw-r-----   0 alex      (1002) alex      (1003)        0 2021-05-20 09:49:50.000000 stylebase-0.0.9/README.md
+-rw-rw-r--   0 alex      (1002) alex      (1003)        5 2021-07-19 18:54:10.000000 stylebase-0.0.9/VERSION
+-rw-rw-r--   0 alex      (1002) alex      (1003)      100 2021-02-14 09:34:02.000000 stylebase-0.0.9/pyproject.toml
+-rw-rw-r--   0 alex      (1002) alex      (1003)      800 2021-07-19 19:30:06.959817 stylebase-0.0.9/setup.cfg
+-rw-rw-r--   0 alex      (1002) alex      (1003)       70 2021-02-14 09:31:37.000000 stylebase-0.0.9/setup.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2021-07-19 19:30:06.939817 stylebase-0.0.9/stylebase/
+-rw-rw-r--   0 alex      (1002) alex      (1003)    18441 2021-05-27 08:29:22.000000 stylebase-0.0.9/stylebase/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)      103 2021-05-28 20:52:35.000000 stylebase-0.0.9/stylebase/__main__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2021-07-19 19:30:06.947817 stylebase-0.0.9/stylebase/hooking/
+-rw-rw-r--   0 alex      (1002) alex      (1003)        0 2021-06-08 08:04:35.000000 stylebase-0.0.9/stylebase/hooking/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)      449 2021-06-08 08:04:36.000000 stylebase-0.0.9/stylebase/hooking/ante_build_hook.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     4678 2021-06-08 08:04:36.000000 stylebase-0.0.9/stylebase/hooking/ante_release_hook.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)      449 2021-06-08 08:04:36.000000 stylebase-0.0.9/stylebase/hooking/post_build_hook.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     2175 2021-06-08 08:04:36.000000 stylebase-0.0.9/stylebase/hooking/post_release_hook.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2021-07-19 19:30:06.951817 stylebase-0.0.9/stylebase/pyrustic_data/
+-rw-rw-r--   0 alex      (1002) alex      (1003)      137 2021-07-19 18:53:50.000000 stylebase-0.0.9/stylebase/pyrustic_data/build_report.json
+-rw-rw-r--   0 alex      (1002) alex      (1003)      294 2021-06-10 17:27:27.000000 stylebase-0.0.9/stylebase/pyrustic_data/hooking.json
+-rw-rw-r--   0 alex      (1002) alex      (1003)      166 2021-06-10 17:27:27.000000 stylebase-0.0.9/stylebase/pyrustic_data/hubstore.json
+-rw-rw-r--   0 alex      (1002) alex      (1003)      419 2021-07-19 18:54:35.000000 stylebase-0.0.9/stylebase/pyrustic_data/release_info.json
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2021-07-19 19:30:06.943817 stylebase-0.0.9/stylebase.egg-info/
+-rw-rw-r--   0 alex      (1002) alex      (1003)      611 2021-07-19 19:30:06.000000 stylebase-0.0.9/stylebase.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1002) alex      (1003)      674 2021-07-19 19:30:06.000000 stylebase-0.0.9/stylebase.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)        1 2021-07-19 19:30:06.000000 stylebase-0.0.9/stylebase.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)       55 2021-07-19 19:30:06.000000 stylebase-0.0.9/stylebase.egg-info/entry_points.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)        1 2021-05-27 17:09:13.000000 stylebase-0.0.9/stylebase.egg-info/not-zip-safe
+-rw-rw-r--   0 alex      (1002) alex      (1003)       16 2021-07-19 19:30:06.000000 stylebase-0.0.9/stylebase.egg-info/top_level.txt
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2021-07-19 19:30:06.951817 stylebase-0.0.9/tests/
+-rw-r-----   0 alex      (1002) alex      (1003)        0 2020-05-31 07:38:19.000000 stylebase-0.0.9/tests/__init__.py
```

### Comparing `stylebase-0.0.8/LICENSE` & `stylebase-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stylebase-0.0.8/PKG-INFO` & `stylebase-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stylebase
-Version: 0.0.8
+Version: 0.0.9
 Summary: Create a style for your Python desktop app
 Home-page: https://github.com/pyrustic/stylebase
 Author: Pyrustic Evangelist
 Author-email: pyrustic@protonmail.com
 Maintainer: Pyrustic Evangelist
 Maintainer-email: pyrustic@protonmail.com
 License: MIT
```

### Comparing `stylebase-0.0.8/setup.cfg` & `stylebase-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `stylebase-0.0.8/stylebase/__init__.py` & `stylebase-0.0.9/stylebase/__init__.py`

 * *Files identical despite different names*

### Comparing `stylebase-0.0.8/stylebase/hooking/ante_release_hook.py` & `stylebase-0.0.9/stylebase/hooking/ante_release_hook.py`

 * *Files identical despite different names*

### Comparing `stylebase-0.0.8/stylebase/hooking/post_release_hook.py` & `stylebase-0.0.9/stylebase/hooking/post_release_hook.py`

 * *Files identical despite different names*

### Comparing `stylebase-0.0.8/stylebase.egg-info/PKG-INFO` & `stylebase-0.0.9/stylebase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stylebase
-Version: 0.0.8
+Version: 0.0.9
 Summary: Create a style for your Python desktop app
 Home-page: https://github.com/pyrustic/stylebase
 Author: Pyrustic Evangelist
 Author-email: pyrustic@protonmail.com
 Maintainer: Pyrustic Evangelist
 Maintainer-email: pyrustic@protonmail.com
 License: MIT
```

### Comparing `stylebase-0.0.8/stylebase.egg-info/SOURCES.txt` & `stylebase-0.0.9/stylebase.egg-info/SOURCES.txt`

 * *Files identical despite different names*


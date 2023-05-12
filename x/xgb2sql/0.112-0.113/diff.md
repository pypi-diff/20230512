# Comparing `tmp/xgb2sql-0.112.tar.gz` & `tmp/xgb2sql-0.113.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgb2sql-0.112.tar", last modified: Thu May 11 18:42:54 2023, max compression
+gzip compressed data, was "xgb2sql-0.113.tar", last modified: Fri May 12 18:49:42 2023, max compression
```

## Comparing `xgb2sql-0.112.tar` & `xgb2sql-0.113.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 benjaminjiang   (501) staff       (20)        0 2023-05-11 18:42:54.786851 xgb2sql-0.112/
--rw-r--r--   0 benjaminjiang   (501) staff       (20)     2348 2023-03-13 17:57:29.000000 xgb2sql-0.112/CONTRIBUTING.md
--rw-r--r--   0 benjaminjiang   (501) staff       (20)    11357 2023-03-13 17:09:07.000000 xgb2sql-0.112/LICENSE
--rw-r--r--   0 benjaminjiang   (501) staff       (20)      111 2023-03-13 17:09:07.000000 xgb2sql-0.112/MANIFEST.in
--rw-r--r--   0 benjaminjiang   (501) staff       (20)     8281 2023-05-11 18:42:54.786634 xgb2sql-0.112/PKG-INFO
--rw-r--r--   0 benjaminjiang   (501) staff       (20)     7514 2023-05-11 17:03:06.000000 xgb2sql-0.112/README.md
--rw-r--r--   0 benjaminjiang   (501) staff       (20)     1752 2023-05-11 18:42:10.000000 xgb2sql-0.112/settings.ini
--rw-r--r--   0 benjaminjiang   (501) staff       (20)       38 2023-05-11 18:42:54.786891 xgb2sql-0.112/setup.cfg
--rw-r--r--   0 benjaminjiang   (501) staff       (20)     1911 2023-05-11 18:25:54.000000 xgb2sql-0.112/setup.py
-drwxr-xr-x   0 benjaminjiang   (501) staff       (20)        0 2023-05-11 18:42:54.785551 xgb2sql-0.112/xgb2sql/
--rw-r--r--   0 benjaminjiang   (501) staff       (20)       22 2023-03-13 18:30:03.000000 xgb2sql-0.112/xgb2sql/__init__.py
--rw-r--r--   0 benjaminjiang   (501) staff       (20)     7281 2023-05-11 17:38:08.000000 xgb2sql-0.112/xgb2sql/core.py
-drwxr-xr-x   0 benjaminjiang   (501) staff       (20)        0 2023-05-11 18:42:54.786458 xgb2sql-0.112/xgb2sql.egg-info/
--rw-r--r--   0 benjaminjiang   (501) staff       (20)     8281 2023-05-11 18:42:54.000000 xgb2sql-0.112/xgb2sql.egg-info/PKG-INFO
--rw-r--r--   0 benjaminjiang   (501) staff       (20)      257 2023-05-11 18:42:54.000000 xgb2sql-0.112/xgb2sql.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminjiang   (501) staff       (20)        1 2023-05-11 18:42:54.000000 xgb2sql-0.112/xgb2sql.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminjiang   (501) staff       (20)        1 2023-05-11 18:39:29.000000 xgb2sql-0.112/xgb2sql.egg-info/not-zip-safe
--rw-r--r--   0 benjaminjiang   (501) staff       (20)        8 2023-05-11 18:42:54.000000 xgb2sql-0.112/xgb2sql.egg-info/top_level.txt
+drwxr-xr-x   0 benjaminjiang   (501) staff       (20)        0 2023-05-12 18:49:42.613446 xgb2sql-0.113/
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     2348 2023-03-13 17:57:29.000000 xgb2sql-0.113/CONTRIBUTING.md
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)    11357 2023-03-13 17:09:07.000000 xgb2sql-0.113/LICENSE
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)      111 2023-03-13 17:09:07.000000 xgb2sql-0.113/MANIFEST.in
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     8281 2023-05-12 18:49:42.613127 xgb2sql-0.113/PKG-INFO
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     7514 2023-05-11 17:03:06.000000 xgb2sql-0.113/README.md
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     1752 2023-05-12 16:24:23.000000 xgb2sql-0.113/settings.ini
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)       38 2023-05-12 18:49:42.613903 xgb2sql-0.113/setup.cfg
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     1911 2023-05-11 18:25:54.000000 xgb2sql-0.113/setup.py
+drwxr-xr-x   0 benjaminjiang   (501) staff       (20)        0 2023-05-12 18:49:42.607272 xgb2sql-0.113/xgb2sql/
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)       22 2023-03-13 18:30:03.000000 xgb2sql-0.113/xgb2sql/__init__.py
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     7281 2023-05-12 18:35:10.000000 xgb2sql-0.113/xgb2sql/core.py
+drwxr-xr-x   0 benjaminjiang   (501) staff       (20)        0 2023-05-12 18:49:42.609314 xgb2sql-0.113/xgb2sql.egg-info/
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)     8281 2023-05-12 18:49:42.000000 xgb2sql-0.113/xgb2sql.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)      257 2023-05-12 18:49:42.000000 xgb2sql-0.113/xgb2sql.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)        1 2023-05-12 18:49:42.000000 xgb2sql-0.113/xgb2sql.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)        1 2023-05-11 18:39:29.000000 xgb2sql-0.113/xgb2sql.egg-info/not-zip-safe
+-rw-r--r--   0 benjaminjiang   (501) staff       (20)        8 2023-05-12 18:49:42.000000 xgb2sql-0.113/xgb2sql.egg-info/top_level.txt
```

### Comparing `xgb2sql-0.112/CONTRIBUTING.md` & `xgb2sql-0.113/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `xgb2sql-0.112/LICENSE` & `xgb2sql-0.113/LICENSE`

 * *Files identical despite different names*

### Comparing `xgb2sql-0.112/PKG-INFO` & `xgb2sql-0.113/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgb2sql
-Version: 0.112
+Version: 0.113
 Summary: A simple library for converting the output of an XGB model to SQL.
 Home-page: https://github.com/Chryzanthemum/xgb2sql
 Author: Benjamin Jiang
 Author-email: benjamin.jiang@well.co
 License: Apache Software License 2.0
 Keywords: xgb2sql,xgb sql,xgboost sql,xgboost to sql,xgb to sql
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `xgb2sql-0.112/README.md` & `xgb2sql-0.113/README.md`

 * *Files identical despite different names*

### Comparing `xgb2sql-0.112/settings.ini` & `xgb2sql-0.113/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 user = Chryzanthemum
 description = A simple library for converting the output of an XGB model to SQL. 
 keywords = xgb2sql, xgb sql, xgboost sql, xgboost to sql, xgb to sql
 author = Benjamin Jiang
 author_email = benjamin.jiang@well.co
 copyright = Well
 branch = master
-version = 0.112
+version = 0.113
 min_python = 3.6
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
```

### Comparing `xgb2sql-0.112/setup.py` & `xgb2sql-0.113/setup.py`

 * *Files identical despite different names*

### Comparing `xgb2sql-0.112/xgb2sql/core.py` & `xgb2sql-0.113/xgb2sql/core.py`

 * *Files identical despite different names*

### Comparing `xgb2sql-0.112/xgb2sql.egg-info/PKG-INFO` & `xgb2sql-0.113/xgb2sql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgb2sql
-Version: 0.112
+Version: 0.113
 Summary: A simple library for converting the output of an XGB model to SQL.
 Home-page: https://github.com/Chryzanthemum/xgb2sql
 Author: Benjamin Jiang
 Author-email: benjamin.jiang@well.co
 License: Apache Software License 2.0
 Keywords: xgb2sql,xgb sql,xgboost sql,xgboost to sql,xgb to sql
 Classifier: Development Status :: 3 - Alpha
```


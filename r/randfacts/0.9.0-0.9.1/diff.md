# Comparing `tmp/randfacts-0.9.0.tar.gz` & `tmp/randfacts-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "randfacts-0.9.0.tar", last modified: Sun Aug 15 03:45:29 2021, max compression
+gzip compressed data, was "randfacts-0.9.1.tar", last modified: Mon Aug 30 18:13:55 2021, max compression
```

## Comparing `randfacts-0.9.0.tar` & `randfacts-0.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 tabulate  (1000) tabulate  (1000)        0 2021-08-15 03:45:29.420312 randfacts-0.9.0/
--rw-r--r--   0 tabulate  (1000) tabulate  (1000)     1086 2021-04-27 12:56:51.000000 randfacts-0.9.0/LICENSE.txt
--rw-r--r--   0 tabulate  (1000) tabulate  (1000)       23 2021-03-07 17:33:15.000000 randfacts-0.9.0/MANIFEST.in
--rw-r--r--   0 tabulate  (1000) tabulate  (1000)     4315 2021-08-15 03:45:29.420312 randfacts-0.9.0/PKG-INFO
--rw-r--r--   0 tabulate  (1000) tabulate  (1000)     3498 2021-07-29 23:56:36.000000 randfacts-0.9.0/README.md
-drwxr-xr-x   0 tabulate  (1000) tabulate  (1000)        0 2021-08-15 03:45:29.420312 randfacts-0.9.0/randfacts/
--rw-r--r--   0 tabulate  (1000) tabulate  (1000)     2307 2021-07-11 22:19:49.000000 randfacts-0.9.0/randfacts/__init__.py
--rw-r--r--   0 tabulate  (1000) tabulate  (1000)       56 2021-06-26 23:13:17.000000 randfacts-0.9.0/randfacts/__main__.py
--rw-r--r--   0 tabulate  (1000) tabulate  (1000)      295 2021-08-15 03:39:53.000000 randfacts-0.9.0/randfacts/__version__.py
--rw-r--r--   0 tabulate  (1000) tabulate  (1000)     1770 2021-07-18 16:48:07.000000 randfacts-0.9.0/randfacts/randfacts.py
--rw-r--r--   0 tabulate  (1000) tabulate  (1000)   500344 2021-08-15 03:43:50.000000 randfacts-0.9.0/randfacts/safe.txt
--rw-r--r--   0 tabulate  (1000) tabulate  (1000)     9384 2021-08-15 03:29:43.000000 randfacts-0.9.0/randfacts/unsafe.txt
-drwxr-xr-x   0 tabulate  (1000) tabulate  (1000)        0 2021-08-15 03:45:29.420312 randfacts-0.9.0/randfacts.egg-info/
--rw-r--r--   0 tabulate  (1000) tabulate  (1000)     4315 2021-08-15 03:45:29.000000 randfacts-0.9.0/randfacts.egg-info/PKG-INFO
--rw-r--r--   0 tabulate  (1000) tabulate  (1000)      316 2021-08-15 03:45:29.000000 randfacts-0.9.0/randfacts.egg-info/SOURCES.txt
--rw-r--r--   0 tabulate  (1000) tabulate  (1000)        1 2021-08-15 03:45:29.000000 randfacts-0.9.0/randfacts.egg-info/dependency_links.txt
--rw-r--r--   0 tabulate  (1000) tabulate  (1000)       10 2021-08-15 03:45:29.000000 randfacts-0.9.0/randfacts.egg-info/top_level.txt
--rw-r--r--   0 tabulate  (1000) tabulate  (1000)       79 2021-08-15 03:45:29.420312 randfacts-0.9.0/setup.cfg
--rw-r--r--   0 tabulate  (1000) tabulate  (1000)     1113 2021-07-18 17:04:03.000000 randfacts-0.9.0/setup.py
+drwxr-xr-x   0 tabulate  (1000) tabulate  (1000)        0 2021-08-30 18:13:55.588160 randfacts-0.9.1/
+-rw-r--r--   0 tabulate  (1000) tabulate  (1000)     1086 2021-08-17 11:26:41.000000 randfacts-0.9.1/LICENSE.txt
+-rw-r--r--   0 tabulate  (1000) tabulate  (1000)       23 2021-08-17 11:26:41.000000 randfacts-0.9.1/MANIFEST.in
+-rw-r--r--   0 tabulate  (1000) tabulate  (1000)     4315 2021-08-30 18:13:55.588160 randfacts-0.9.1/PKG-INFO
+-rw-r--r--   0 tabulate  (1000) tabulate  (1000)     3498 2021-08-17 11:26:41.000000 randfacts-0.9.1/README.md
+drwxr-xr-x   0 tabulate  (1000) tabulate  (1000)        0 2021-08-30 18:13:55.584827 randfacts-0.9.1/randfacts/
+-rw-r--r--   0 tabulate  (1000) tabulate  (1000)     1555 2021-08-30 18:10:12.000000 randfacts-0.9.1/randfacts/__init__.py
+-rw-r--r--   0 tabulate  (1000) tabulate  (1000)       56 2021-08-17 11:26:41.000000 randfacts-0.9.1/randfacts/__main__.py
+-rw-r--r--   0 tabulate  (1000) tabulate  (1000)      295 2021-08-30 18:10:37.000000 randfacts-0.9.1/randfacts/__version__.py
+-rw-r--r--   0 tabulate  (1000) tabulate  (1000)     1770 2021-08-17 11:26:41.000000 randfacts-0.9.1/randfacts/randfacts.py
+-rw-r--r--   0 tabulate  (1000) tabulate  (1000)   500344 2021-08-17 11:26:41.000000 randfacts-0.9.1/randfacts/safe.txt
+-rw-r--r--   0 tabulate  (1000) tabulate  (1000)     9384 2021-08-17 11:26:41.000000 randfacts-0.9.1/randfacts/unsafe.txt
+drwxr-xr-x   0 tabulate  (1000) tabulate  (1000)        0 2021-08-30 18:13:55.584827 randfacts-0.9.1/randfacts.egg-info/
+-rw-r--r--   0 tabulate  (1000) tabulate  (1000)     4315 2021-08-30 18:13:55.000000 randfacts-0.9.1/randfacts.egg-info/PKG-INFO
+-rw-r--r--   0 tabulate  (1000) tabulate  (1000)      316 2021-08-30 18:13:55.000000 randfacts-0.9.1/randfacts.egg-info/SOURCES.txt
+-rw-r--r--   0 tabulate  (1000) tabulate  (1000)        1 2021-08-30 18:13:55.000000 randfacts-0.9.1/randfacts.egg-info/dependency_links.txt
+-rw-r--r--   0 tabulate  (1000) tabulate  (1000)       10 2021-08-30 18:13:55.000000 randfacts-0.9.1/randfacts.egg-info/top_level.txt
+-rw-r--r--   0 tabulate  (1000) tabulate  (1000)       79 2021-08-30 18:13:55.588160 randfacts-0.9.1/setup.cfg
+-rw-r--r--   0 tabulate  (1000) tabulate  (1000)     1113 2021-08-17 11:26:41.000000 randfacts-0.9.1/setup.py
```

### Comparing `randfacts-0.9.0/LICENSE.txt` & `randfacts-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `randfacts-0.9.0/PKG-INFO` & `randfacts-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: randfacts
-Version: 0.9.0
+Version: 0.9.1
 Summary: Package to generate random facts
 Home-page: https://github.com/TabulateJarl8/randfacts
 Author: Tabulate
 Author-email: tabulatejarl8@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: randfacts Version: 0.9.0 Summary: Package to
+Metadata-Version: 2.1 Name: randfacts Version: 0.9.1 Summary: Package to
 generate random facts Home-page: https://github.com/TabulateJarl8/randfacts
 Author: Tabulate Author-email: tabulatejarl8@gmail.com License: UNKNOWN
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
```

### Comparing `randfacts-0.9.0/README.md` & `randfacts-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `randfacts-0.9.0/randfacts/randfacts.py` & `randfacts-0.9.1/randfacts/randfacts.py`

 * *Files identical despite different names*

### Comparing `randfacts-0.9.0/randfacts/safe.txt` & `randfacts-0.9.1/randfacts/safe.txt`

 * *Files identical despite different names*

### Comparing `randfacts-0.9.0/randfacts/unsafe.txt` & `randfacts-0.9.1/randfacts/unsafe.txt`

 * *Files identical despite different names*

### Comparing `randfacts-0.9.0/randfacts.egg-info/PKG-INFO` & `randfacts-0.9.1/randfacts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: randfacts
-Version: 0.9.0
+Version: 0.9.1
 Summary: Package to generate random facts
 Home-page: https://github.com/TabulateJarl8/randfacts
 Author: Tabulate
 Author-email: tabulatejarl8@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: randfacts Version: 0.9.0 Summary: Package to
+Metadata-Version: 2.1 Name: randfacts Version: 0.9.1 Summary: Package to
 generate random facts Home-page: https://github.com/TabulateJarl8/randfacts
 Author: Tabulate Author-email: tabulatejarl8@gmail.com License: UNKNOWN
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
```

### Comparing `randfacts-0.9.0/setup.py` & `randfacts-0.9.1/setup.py`

 * *Files identical despite different names*


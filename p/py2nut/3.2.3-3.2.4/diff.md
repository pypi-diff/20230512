# Comparing `tmp/py2nut-3.2.3.tar.gz` & `tmp/py2nut-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py2nut-3.2.3.tar", last modified: Mon Apr 17 03:25:34 2023, max compression
+gzip compressed data, was "py2nut-3.2.4.tar", last modified: Fri May 12 07:17:50 2023, max compression
```

## Comparing `py2nut-3.2.3.tar` & `py2nut-3.2.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.564768 py2nut-3.2.3/
--rw-rw-rw-   0        0        0    35803 2022-07-21 09:01:30.000000 py2nut-3.2.3/LICENSE
--rw-rw-rw-   0        0        0       22 2022-12-05 05:43:45.000000 py2nut-3.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0    21795 2023-04-17 03:25:34.560779 py2nut-3.2.3/PKG-INFO
--rw-rw-rw-   0        0        0    21290 2022-12-05 05:43:25.000000 py2nut-3.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.124852 py2nut-3.2.3/py2Nut/
--rw-rw-rw-   0        0        0       23 2023-04-14 05:42:20.000000 py2nut-3.2.3/py2Nut/__init__.py
--rw-rw-rw-   0        0        0        3 2022-12-05 07:43:05.000000 py2nut-3.2.3/py2Nut/_lib.py
--rw-rw-rw-   0        0        0       42 2022-12-05 07:42:35.000000 py2nut-3.2.3/py2Nut/nutApi.py
--rw-rw-rw-   0        0        0       52 2022-12-05 05:21:51.000000 py2nut-3.2.3/py2Nut/nutDataframe.py
--rw-rw-rw-   0        0        0       45 2022-12-05 07:42:04.000000 py2nut-3.2.3/py2Nut/nutDate.py
--rw-rw-rw-   0        0        0       37 2022-12-05 09:05:13.000000 py2nut-3.2.3/py2Nut/nutDb.py
--rw-rw-rw-   0        0        0       46 2022-12-05 09:05:55.000000 py2nut-3.2.3/py2Nut/nutEmail.py
--rw-rw-rw-   0        0        0       48 2022-12-05 09:04:21.000000 py2nut-3.2.3/py2Nut/nutFiles.py
--rw-rw-rw-   0        0        0       40 2022-12-05 09:20:39.000000 py2nut-3.2.3/py2Nut/nutFtp.py
--rw-rw-rw-   0        0        0       48 2022-12-05 07:42:53.000000 py2nut-3.2.3/py2Nut/nutOther.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.134854 py2nut-3.2.3/py2Nut/xlrd/
--rw-rw-rw-   0        0        0    34373 2022-07-21 09:01:30.000000 py2nut-3.2.3/py2Nut/xlrd/xlsx.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.264864 py2nut-3.2.3/py2nut.egg-info/
--rw-rw-rw-   0        0        0    21795 2023-04-17 03:25:33.000000 py2nut-3.2.3/py2nut.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1164 2023-04-17 03:25:33.000000 py2nut-3.2.3/py2nut.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 03:25:33.000000 py2nut-3.2.3/py2nut.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-17 03:25:33.000000 py2nut-3.2.3/py2nut.egg-info/requires.txt
--rw-rw-rw-   0        0        0       78 2023-04-17 03:25:33.000000 py2nut-3.2.3/py2nut.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.271846 py2nut-3.2.3/pynut_1tools/
-drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.380864 py2nut-3.2.3/pynut_1tools/pyNutTools/
--rw-rw-rw-   0        0        0       25 2023-04-04 08:29:08.000000 py2nut-3.2.3/pynut_1tools/pyNutTools/__init__.py
--rw-rw-rw-   0        0        0     2054 2022-12-07 03:56:44.000000 py2nut-3.2.3/pynut_1tools/pyNutTools/_lib.py
--rw-rw-rw-   0        0        0    32349 2023-04-04 08:31:33.000000 py2nut-3.2.3/pynut_1tools/pyNutTools/nutDataframe.py
--rw-rw-rw-   0        0        0    18046 2022-12-07 03:57:19.000000 py2nut-3.2.3/pynut_1tools/pyNutTools/nutDate.py
--rw-rw-rw-   0        0        0     8711 2023-03-07 04:16:53.000000 py2nut-3.2.3/pynut_1tools/pyNutTools/nutOther.py
--rw-rw-rw-   0        0        0     1029 2023-03-07 04:16:55.000000 py2nut-3.2.3/pynut_1tools/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.386540 py2nut-3.2.3/pynut_2api/
-drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.431927 py2nut-3.2.3/pynut_2api/pyNutApi/
--rw-rw-rw-   0        0        0       23 2023-03-07 04:16:57.000000 py2nut-3.2.3/pynut_2api/pyNutApi/__init__.py
--rw-rw-rw-   0        0        0     3607 2023-04-14 05:30:35.000000 py2nut-3.2.3/pynut_2api/pyNutApi/_lib.py
--rw-rw-rw-   0        0        0    29117 2023-04-17 03:23:52.000000 py2nut-3.2.3/pynut_2api/pyNutApi/nutApi.py
--rw-rw-rw-   0        0        0     1079 2023-04-14 05:27:51.000000 py2nut-3.2.3/pynut_2api/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.464837 py2nut-3.2.3/pynut_2files/
-drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.481792 py2nut-3.2.3/pynut_2files/pyNutFiles/
--rw-rw-rw-   0        0        0       23 2023-03-30 09:07:33.000000 py2nut-3.2.3/pynut_2files/pyNutFiles/__init__.py
--rw-rw-rw-   0        0        0     6710 2022-12-07 04:06:54.000000 py2nut-3.2.3/pynut_2files/pyNutFiles/_lib.py
--rw-rw-rw-   0        0        0   128574 2023-04-14 05:25:41.000000 py2nut-3.2.3/pynut_2files/pyNutFiles/nutFiles.py
--rw-rw-rw-   0        0        0     1170 2023-04-14 05:28:03.000000 py2nut-3.2.3/pynut_2files/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.490965 py2nut-3.2.3/pynut_3db/
-drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.504927 py2nut-3.2.3/pynut_3db/pyNutDB/
--rw-rw-rw-   0        0        0       23 2023-03-07 04:17:04.000000 py2nut-3.2.3/pynut_3db/pyNutDB/__init__.py
--rw-rw-rw-   0        0        0     2591 2022-12-05 13:21:28.000000 py2nut-3.2.3/pynut_3db/pyNutDB/_lib.py
--rw-rw-rw-   0        0        0    21550 2023-03-07 04:17:05.000000 py2nut-3.2.3/pynut_3db/pyNutDB/nutDb.py
--rw-rw-rw-   0        0        0     1051 2023-04-14 05:28:19.000000 py2nut-3.2.3/pynut_3db/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.509990 py2nut-3.2.3/pynut_3email/
-drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.525872 py2nut-3.2.3/pynut_3email/pyNutEmail/
--rw-rw-rw-   0        0        0       21 2023-04-14 05:29:30.000000 py2nut-3.2.3/pynut_3email/pyNutEmail/__init__.py
--rw-rw-rw-   0        0        0     4303 2022-12-05 13:20:03.000000 py2nut-3.2.3/pynut_3email/pyNutEmail/_lib.py
--rw-rw-rw-   0        0        0    35893 2023-01-04 05:22:20.000000 py2nut-3.2.3/pynut_3email/pyNutEmail/nutEmail.py
--rw-rw-rw-   0        0        0     1064 2023-04-14 05:28:29.000000 py2nut-3.2.3/pynut_3email/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.536843 py2nut-3.2.3/pynut_3ftp/
-drwxrwxrwx   0        0        0        0 2023-04-17 03:25:34.552852 py2nut-3.2.3/pynut_3ftp/pyNutFtp/
--rw-rw-rw-   0        0        0       23 2023-04-14 05:29:30.000000 py2nut-3.2.3/pynut_3ftp/pyNutFtp/__init__.py
--rw-rw-rw-   0        0        0     3476 2023-01-04 05:34:31.000000 py2nut-3.2.3/pynut_3ftp/pyNutFtp/_lib.py
--rw-rw-rw-   0        0        0    29570 2023-01-04 05:57:55.000000 py2nut-3.2.3/pynut_3ftp/pyNutFtp/nutFtp.py
--rw-rw-rw-   0        0        0     1072 2023-04-14 05:28:37.000000 py2nut-3.2.3/pynut_3ftp/setup.py
--rw-rw-rw-   0        0        0       42 2023-04-17 03:25:34.566763 py2nut-3.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1565 2023-02-08 10:26:55.000000 py2nut-3.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:17:50.871846 py2nut-3.2.4/
+-rw-rw-rw-   0        0        0    35803 2022-07-21 09:01:30.000000 py2nut-3.2.4/LICENSE
+-rw-rw-rw-   0        0        0       22 2022-12-05 05:43:45.000000 py2nut-3.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    21795 2023-05-12 07:17:50.869833 py2nut-3.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0    21290 2022-12-05 05:43:25.000000 py2nut-3.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 07:17:50.717321 py2nut-3.2.4/py2Nut/
+-rw-rw-rw-   0        0        0       23 2023-04-17 03:26:15.000000 py2nut-3.2.4/py2Nut/__init__.py
+-rw-rw-rw-   0        0        0        3 2022-12-05 07:43:05.000000 py2nut-3.2.4/py2Nut/_lib.py
+-rw-rw-rw-   0        0        0       42 2022-12-05 07:42:35.000000 py2nut-3.2.4/py2Nut/nutApi.py
+-rw-rw-rw-   0        0        0       52 2022-12-05 05:21:51.000000 py2nut-3.2.4/py2Nut/nutDataframe.py
+-rw-rw-rw-   0        0        0       45 2022-12-05 07:42:04.000000 py2nut-3.2.4/py2Nut/nutDate.py
+-rw-rw-rw-   0        0        0       37 2022-12-05 09:05:13.000000 py2nut-3.2.4/py2Nut/nutDb.py
+-rw-rw-rw-   0        0        0       46 2022-12-05 09:05:55.000000 py2nut-3.2.4/py2Nut/nutEmail.py
+-rw-rw-rw-   0        0        0       48 2022-12-05 09:04:21.000000 py2nut-3.2.4/py2Nut/nutFiles.py
+-rw-rw-rw-   0        0        0       40 2022-12-05 09:20:39.000000 py2nut-3.2.4/py2Nut/nutFtp.py
+-rw-rw-rw-   0        0        0       48 2022-12-05 07:42:53.000000 py2nut-3.2.4/py2Nut/nutOther.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:17:50.720311 py2nut-3.2.4/py2Nut/xlrd/
+-rw-rw-rw-   0        0        0    34373 2022-07-21 09:01:30.000000 py2nut-3.2.4/py2Nut/xlrd/xlsx.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:17:50.739588 py2nut-3.2.4/py2nut.egg-info/
+-rw-rw-rw-   0        0        0    21795 2023-05-12 07:17:50.000000 py2nut-3.2.4/py2nut.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1164 2023-05-12 07:17:50.000000 py2nut-3.2.4/py2nut.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 07:17:50.000000 py2nut-3.2.4/py2nut.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-12 07:17:50.000000 py2nut-3.2.4/py2nut.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       78 2023-05-12 07:17:50.000000 py2nut-3.2.4/py2nut.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 07:17:50.742877 py2nut-3.2.4/pynut_1tools/
+drwxrwxrwx   0        0        0        0 2023-05-12 07:17:50.770505 py2nut-3.2.4/pynut_1tools/pyNutTools/
+-rw-rw-rw-   0        0        0       25 2023-04-04 08:29:08.000000 py2nut-3.2.4/pynut_1tools/pyNutTools/__init__.py
+-rw-rw-rw-   0        0        0     2054 2022-12-07 03:56:44.000000 py2nut-3.2.4/pynut_1tools/pyNutTools/_lib.py
+-rw-rw-rw-   0        0        0    32469 2023-04-26 09:49:54.000000 py2nut-3.2.4/pynut_1tools/pyNutTools/nutDataframe.py
+-rw-rw-rw-   0        0        0    18046 2022-12-07 03:57:19.000000 py2nut-3.2.4/pynut_1tools/pyNutTools/nutDate.py
+-rw-rw-rw-   0        0        0     8711 2023-03-07 04:16:53.000000 py2nut-3.2.4/pynut_1tools/pyNutTools/nutOther.py
+-rw-rw-rw-   0        0        0     1029 2023-03-07 04:16:55.000000 py2nut-3.2.4/pynut_1tools/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:17:50.776489 py2nut-3.2.4/pynut_2api/
+drwxrwxrwx   0        0        0        0 2023-05-12 07:17:50.792447 py2nut-3.2.4/pynut_2api/pyNutApi/
+-rw-rw-rw-   0        0        0       23 2023-03-07 04:16:57.000000 py2nut-3.2.4/pynut_2api/pyNutApi/__init__.py
+-rw-rw-rw-   0        0        0     3607 2023-04-14 05:30:35.000000 py2nut-3.2.4/pynut_2api/pyNutApi/_lib.py
+-rw-rw-rw-   0        0        0    29117 2023-04-17 03:23:52.000000 py2nut-3.2.4/pynut_2api/pyNutApi/nutApi.py
+-rw-rw-rw-   0        0        0     1079 2023-04-14 05:27:51.000000 py2nut-3.2.4/pynut_2api/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:17:50.797652 py2nut-3.2.4/pynut_2files/
+drwxrwxrwx   0        0        0        0 2023-05-12 07:17:50.812393 py2nut-3.2.4/pynut_2files/pyNutFiles/
+-rw-rw-rw-   0        0        0       23 2023-03-30 09:07:33.000000 py2nut-3.2.4/pynut_2files/pyNutFiles/__init__.py
+-rw-rw-rw-   0        0        0     6710 2022-12-07 04:06:54.000000 py2nut-3.2.4/pynut_2files/pyNutFiles/_lib.py
+-rw-rw-rw-   0        0        0   131715 2023-05-12 07:07:11.000000 py2nut-3.2.4/pynut_2files/pyNutFiles/nutFiles.py
+-rw-rw-rw-   0        0        0     1170 2023-04-14 05:28:03.000000 py2nut-3.2.4/pynut_2files/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:17:50.817828 py2nut-3.2.4/pynut_3db/
+drwxrwxrwx   0        0        0        0 2023-05-12 07:17:50.828937 py2nut-3.2.4/pynut_3db/pyNutDB/
+-rw-rw-rw-   0        0        0       23 2023-03-07 04:17:04.000000 py2nut-3.2.4/pynut_3db/pyNutDB/__init__.py
+-rw-rw-rw-   0        0        0     2591 2022-12-05 13:21:28.000000 py2nut-3.2.4/pynut_3db/pyNutDB/_lib.py
+-rw-rw-rw-   0        0        0    21550 2023-03-07 04:17:05.000000 py2nut-3.2.4/pynut_3db/pyNutDB/nutDb.py
+-rw-rw-rw-   0        0        0     1051 2023-04-14 05:28:19.000000 py2nut-3.2.4/pynut_3db/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:17:50.834124 py2nut-3.2.4/pynut_3email/
+drwxrwxrwx   0        0        0        0 2023-05-12 07:17:50.847885 py2nut-3.2.4/pynut_3email/pyNutEmail/
+-rw-rw-rw-   0        0        0       21 2023-04-14 05:29:30.000000 py2nut-3.2.4/pynut_3email/pyNutEmail/__init__.py
+-rw-rw-rw-   0        0        0     4303 2022-12-05 13:20:03.000000 py2nut-3.2.4/pynut_3email/pyNutEmail/_lib.py
+-rw-rw-rw-   0        0        0    35893 2023-01-04 05:22:20.000000 py2nut-3.2.4/pynut_3email/pyNutEmail/nutEmail.py
+-rw-rw-rw-   0        0        0     1064 2023-04-14 05:28:29.000000 py2nut-3.2.4/pynut_3email/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:17:50.852947 py2nut-3.2.4/pynut_3ftp/
+drwxrwxrwx   0        0        0        0 2023-05-12 07:17:50.864329 py2nut-3.2.4/pynut_3ftp/pyNutFtp/
+-rw-rw-rw-   0        0        0       23 2023-04-14 05:29:30.000000 py2nut-3.2.4/pynut_3ftp/pyNutFtp/__init__.py
+-rw-rw-rw-   0        0        0     3476 2023-01-04 05:34:31.000000 py2nut-3.2.4/pynut_3ftp/pyNutFtp/_lib.py
+-rw-rw-rw-   0        0        0    29570 2023-01-04 05:57:55.000000 py2nut-3.2.4/pynut_3ftp/pyNutFtp/nutFtp.py
+-rw-rw-rw-   0        0        0     1072 2023-04-14 05:28:37.000000 py2nut-3.2.4/pynut_3ftp/setup.py
+-rw-rw-rw-   0        0        0       42 2023-05-12 07:17:50.872854 py2nut-3.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1565 2023-02-08 10:26:55.000000 py2nut-3.2.4/setup.py
```

### Comparing `py2nut-3.2.3/LICENSE` & `py2nut-3.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.3/PKG-INFO` & `py2nut-3.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2nut
-Version: 3.2.3
+Version: 3.2.4
 Summary: This Library allows you to make Misc operations in various domain
 Home-page: https://github.com/Laurent-Tupin/py2nut
 Author: Laurent Tupin
 Author-email: laurent.tupinn@gmail.com
 License: Copyright 2022-2035
 Platform: UNKNOWN
 Classifier: License :: Free For Home Use
```

### Comparing `py2nut-3.2.3/README.md` & `py2nut-3.2.4/README.md`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.3/py2Nut/xlrd/xlsx.py` & `py2nut-3.2.4/py2Nut/xlrd/xlsx.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.3/py2nut.egg-info/PKG-INFO` & `py2nut-3.2.4/py2nut.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2nut
-Version: 3.2.3
+Version: 3.2.4
 Summary: This Library allows you to make Misc operations in various domain
 Home-page: https://github.com/Laurent-Tupin/py2nut
 Author: Laurent Tupin
 Author-email: laurent.tupinn@gmail.com
 License: Copyright 2022-2035
 Platform: UNKNOWN
 Classifier: License :: Free For Home Use
```

### Comparing `py2nut-3.2.3/py2nut.egg-info/SOURCES.txt` & `py2nut-3.2.4/py2nut.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.3/pynut_1tools/pyNutTools/_lib.py` & `py2nut-3.2.4/pynut_1tools/pyNutTools/_lib.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.3/pynut_1tools/pyNutTools/nutDataframe.py` & `py2nut-3.2.4/pynut_1tools/pyNutTools/nutDataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -578,34 +578,38 @@
     # how{‘left’, ‘right’, ‘outer’, ‘inner’}, default ‘inner’
     # https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.merge.html
     
     # Verification
     if not str_columnON in df_left.columns :
         logger.error(' ERROR  in fDf_JoinDf: Column {0} is not in left dataframe: {1}'.format(str_columnON, list(df_left.columns)))
         logger.error(df_left.head(5) )
+        logger.error('\n')
         return df_left
     if str_columnRightON == '':
         if not str_columnON in df_right.columns:
             logger.error(' ERROR  in fDf_JoinDf: Column {0} is not in right dataframe: {1}'.format(str_columnON, list(df_right.columns)))
             logger.error(df_right.head(5) )
+            logger.error('\n')
             return df_left
     else:
         if not str_columnRightON in df_right.columns:
             logger.error(' ERROR  in fDf_JoinDf: Column {0} is not in right dataframe: {1}'.format(str_columnRightON, list(df_right.columns)))
             logger.error(df_right.head(5) )
+            logger.error('\n')
             return df_left
     # JOIN 
     try:
         if str_columnRightON == '':
             df = pd.merge(df_left, df_right, on = str_columnON, how = str_how)
         else:
             df = pd.merge(df_left, df_right, left_on = str_columnON, right_on = str_columnRightON, how = str_how)
         #df_Holds_MACI = df_Holds_MACI.join(df_Out_Fx[['Curr', 'Fx']].set_index('Curr'), on = 'Curr')
     except Exception as err:    
         logger.error(' ERROR  in fDf_JoinDf: |{}|'.format(str(err)) )
+        logger.error('\n')
         return df_left
     return df
 
 
 
 def fDf_imposerStr_0apVirgule(df, str_colName, int_0apVirgule = 2):
     try:
```

### Comparing `py2nut-3.2.3/pynut_1tools/pyNutTools/nutDate.py` & `py2nut-3.2.4/pynut_1tools/pyNutTools/nutDate.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.3/pynut_1tools/pyNutTools/nutOther.py` & `py2nut-3.2.4/pynut_1tools/pyNutTools/nutOther.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.3/pynut_1tools/setup.py` & `py2nut-3.2.4/pynut_1tools/setup.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.3/pynut_2api/pyNutApi/_lib.py` & `py2nut-3.2.4/pynut_2api/pyNutApi/_lib.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.3/pynut_2api/pyNutApi/nutApi.py` & `py2nut-3.2.4/pynut_2api/pyNutApi/nutApi.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.3/pynut_2api/setup.py` & `py2nut-3.2.4/pynut_2api/setup.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.3/pynut_2files/pyNutFiles/_lib.py` & `py2nut-3.2.4/pynut_2files/pyNutFiles/_lib.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.3/pynut_2files/pyNutFiles/nutFiles.py` & `py2nut-3.2.4/pynut_2files/pyNutFiles/nutFiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 oth = lib.nutOther()
 dat = lib.nutDate()
 dframe = lib.nutDataframe()
 logger = lib.logger()
 import os, sys
 import time
 import datetime as dt
+import warnings
 
 pd = lib.pandas()
 pickle = lib.pickle()
 shutil = lib.shutil()
 psutil = lib.psutil()
 glob = lib.glob()
 csv = lib.csv()
@@ -1439,14 +1440,51 @@
             logger.error('  ERROR: Could not create / Fill the XLSX file: |{}|'.format(err))
             logger.error('  - Path Origin : |{}|'.format(str_pathWkOrigin))
             logger.error('  - Path Dest : |{}|'.format(str_pathWkDest))
             logger.error('  - path Return : |{}|'.format(str_pathReturn))
     return True
 
 
+# Merge XLS workbook - COPY SHEET - 1 file out - several Sheet
+def fStr_fillExcel_MergeWk_CopySh(str_pathDest, l_wkToMerge = [], bl_header = None, bl_formatCopySheetXls = False):
+    """ Take a list of Workbook (path)
+    Copy the first input WK into destination (path)
+    Copy sheet by sheet into Dest for the rest
+        - Value / DF (Will use pd.ExcelWriter)
+        - with Format (will use class c_xlApp_xlwings)
+    """
+    if not l_wkToMerge == []:
+        # if only value needed, lets just use pandas.ExcelWriter / openxyl to add the sheet
+        if bl_formatCopySheetXls is False:
+            # Remove the openxyl warnings
+            with warnings.catch_warnings(record = True):
+                warnings.simplefilter("always")
+                with pd.ExcelWriter(str_pathDest, mode = 'a', engine = 'openpyxl', if_sheet_exists = 'error') as xl_writer:
+                    # , date_format = 'YYYY-MM-DD', datetime_format = 'YYYY-MM-DD'
+                    for _pcf in l_wkToMerge:
+                        # Find the sheet name
+                        l_sheetNames =  pd.ExcelFile(_pcf).sheet_names
+                        for _sheetName in l_sheetNames:
+                            # Get the dataframe from input
+                            df_data =   pd_read_excel(_pcf, str_SheetName = _sheetName, bl_header = bl_header)
+                            # Write it to a sheet in the output excel
+                            df_data.to_excel(xl_writer, sheet_name = _sheetName, index = False, header = bl_header)
+        # If we want format we will use EXCEL APP (xlwings)
+        else:
+            inst_xlWings =  c_xlApp_xlwings()
+            inst_xlWings.FindXlApp(bl_visible = True, bl_screen_updating = False, bl_display_alerts = False)
+            for _pcf in l_wkToMerge:
+                inst_xlWings.CopySheetFromAnotherBook(_pcf, str_pathDest = str_pathDest, bl_allSheets = True)
+            # Quit the APP
+            inst_xlWings.Quit_xlApp()
+    return str_pathDest
+
+
+
+
 # -----------------------------------------------------------------
 # CONVERT XLS File
 # -----------------------------------------------------------------
 def fDf_convertToXlsx(str_path, str_SheetName='', bl_header=None):
     """ Will use Act_win32_SaveAsCleanFile to make sure the file is not corrupted
     and SaveAs XLSX instead of XLS
     Read it and return the dataframe """
@@ -2282,14 +2320,41 @@
         self.d_wkOpen[self.wb_path] = xl_book
         # Fill PARAM
         self.xl_lastBook = xl_book
         self.__wkIsOpen = True
         return self.xl_lastBook
 
     # SHEET
+    def CopySheetFromAnotherBook(self, str_pathOrigin, str_pathDest='', bl_allSheets=False, str_shName=1):
+        # BOOKS
+        try:
+            if str_pathDest != '':      self.wb_path = str_pathDest
+            xl_origin = self.OpenWorkbook(str_pathOrigin)
+            xl_dest = self.OpenWorkbook(str_pathDest)
+        except Exception as err:
+            logger.error(f'ERROR: fl CopySheetFromAnotherBook BOOK |{err}|')
+            raise
+        # SHEETS
+        try:
+            int_lastSheet = int(len(xl_dest.sheets))
+            if bl_allSheets is True:
+                l_sheets = xl_origin.sheets
+                for o_sheet in l_sheets:
+                    o_sheet.api.Copy(After=xl_dest.sheets(int_lastSheet).api)
+            else:
+                o_sheet = xl_origin.sheets(str_shName)
+                o_sheet.api.Copy(After=xl_dest.sheets(int_lastSheet).api)
+
+        except Exception as err:
+            logger.error(f'ERROR: fl CopySheetFromAnotherBook sheets |{err}|')
+            raise
+        # SAVE
+        self.close_Book(bl_saveBeforeClose=True)
+
+
     def DefineWorksheet(self, str_sheetName='', int_sheetNumber=-1, str_sheetNameToADD=''):
         xl_lastBook = self.xl_lastBook
         self.xl_lastSheet_name = str_sheetName
         # Sheet with a Name
         if str_sheetName != '':
             try:
                 xl_sheet = xl_lastBook.sheets[str_sheetName]
```

### Comparing `py2nut-3.2.3/pynut_2files/setup.py` & `py2nut-3.2.4/pynut_2files/setup.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.3/pynut_3db/pyNutDB/_lib.py` & `py2nut-3.2.4/pynut_3db/pyNutDB/_lib.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.3/pynut_3db/pyNutDB/nutDb.py` & `py2nut-3.2.4/pynut_3db/pyNutDB/nutDb.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.3/pynut_3db/setup.py` & `py2nut-3.2.4/pynut_3db/setup.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.3/pynut_3email/pyNutEmail/_lib.py` & `py2nut-3.2.4/pynut_3email/pyNutEmail/_lib.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.3/pynut_3email/pyNutEmail/nutEmail.py` & `py2nut-3.2.4/pynut_3email/pyNutEmail/nutEmail.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.3/pynut_3email/setup.py` & `py2nut-3.2.4/pynut_3email/setup.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.3/pynut_3ftp/pyNutFtp/_lib.py` & `py2nut-3.2.4/pynut_3ftp/pyNutFtp/_lib.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.3/pynut_3ftp/pyNutFtp/nutFtp.py` & `py2nut-3.2.4/pynut_3ftp/pyNutFtp/nutFtp.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.3/pynut_3ftp/setup.py` & `py2nut-3.2.4/pynut_3ftp/setup.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.3/setup.py` & `py2nut-3.2.4/setup.py`

 * *Files identical despite different names*


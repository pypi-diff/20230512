# Comparing `tmp/crawler_commons-0.0.6.tar.gz` & `tmp/crawler_commons-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawler_commons-0.0.6.tar", last modified: Sat May  6 07:57:22 2023, max compression
+gzip compressed data, was "dist/crawler_commons-0.0.7.tar", last modified: Fri May 12 10:45:36 2023, max compression
```

## Comparing `crawler_commons-0.0.6.tar` & `crawler_commons-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:57:22.875394 crawler_commons-0.0.6/
--rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 crawler_commons-0.0.6/LICENSE
--rw-r--r--   0 nezah      (501) staff       (20)      399 2023-05-06 07:57:22.875200 crawler_commons-0.0.6/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)       27 2023-03-17 05:41:21.000000 crawler_commons-0.0.6/README.md
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:57:22.873460 crawler_commons-0.0.6/crawapi/
--rw-r--r--   0 nezah      (501) staff       (20)     2634 2023-05-06 07:54:17.000000 crawler_commons-0.0.6/crawapi/__init__.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:57:22.874118 crawler_commons-0.0.6/crawler_commons.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)      399 2023-05-06 07:57:22.000000 crawler_commons-0.0.6/crawler_commons.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      328 2023-05-06 07:57:22.000000 crawler_commons-0.0.6/crawler_commons.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-06 07:57:22.000000 crawler_commons-0.0.6/crawler_commons.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)       19 2023-05-06 07:57:22.000000 crawler_commons-0.0.6/crawler_commons.egg-info/top_level.txt
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:57:22.874967 crawler_commons-0.0.6/crawlutils/
--rw-r--r--   0 nezah      (501) staff       (20)     2535 2023-05-03 17:15:32.000000 crawler_commons-0.0.6/crawlutils/__init__.py
--rw-r--r--   0 nezah      (501) staff       (20)     1150 2022-12-27 06:40:36.000000 crawler_commons-0.0.6/crawlutils/date_utils.py
--rw-r--r--   0 nezah      (501) staff       (20)     1131 2023-05-06 07:52:34.000000 crawler_commons-0.0.6/crawlutils/num_utils.py
--rw-r--r--   0 nezah      (501) staff       (20)     1007 2023-05-06 07:56:32.000000 crawler_commons-0.0.6/crawlutils/soup_traversal.py
--rw-r--r--   0 nezah      (501) staff       (20)     1556 2023-05-06 07:27:29.000000 crawler_commons-0.0.6/crawlutils/text_utils.py
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-06 07:57:22.875450 crawler_commons-0.0.6/setup.cfg
--rw-r--r--   0 nezah      (501) staff       (20)      569 2023-05-06 07:57:22.000000 crawler_commons-0.0.6/setup.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-12 10:45:36.000000 crawler_commons-0.0.7/
+-rw-r--r--   0 nezah      (501) staff       (20)      419 2023-05-12 10:45:36.000000 crawler_commons-0.0.7/PKG-INFO
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-12 10:45:36.000000 crawler_commons-0.0.7/crawlutils/
+-rw-r--r--   0 nezah      (501) staff       (20)     1556 2023-05-06 07:27:29.000000 crawler_commons-0.0.7/crawlutils/text_utils.py
+-rw-r--r--   0 nezah      (501) staff       (20)      273 2023-05-12 10:44:28.000000 crawler_commons-0.0.7/crawlutils/log.py
+-rw-r--r--   0 nezah      (501) staff       (20)     1150 2022-12-27 06:40:36.000000 crawler_commons-0.0.7/crawlutils/date_utils.py
+-rw-r--r--   0 nezah      (501) staff       (20)     2535 2023-05-03 17:15:32.000000 crawler_commons-0.0.7/crawlutils/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)     1131 2023-05-06 07:52:34.000000 crawler_commons-0.0.7/crawlutils/num_utils.py
+-rw-r--r--   0 nezah      (501) staff       (20)     1007 2023-05-06 07:56:32.000000 crawler_commons-0.0.7/crawlutils/soup_traversal.py
+-rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 crawler_commons-0.0.7/LICENSE
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-12 10:45:36.000000 crawler_commons-0.0.7/crawapi/
+-rw-r--r--   0 nezah      (501) staff       (20)     2634 2023-05-06 07:54:17.000000 crawler_commons-0.0.7/crawapi/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)       27 2023-03-17 05:41:21.000000 crawler_commons-0.0.7/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      569 2023-05-12 10:45:32.000000 crawler_commons-0.0.7/setup.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-12 10:45:36.000000 crawler_commons-0.0.7/crawler_commons.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)      419 2023-05-12 10:45:36.000000 crawler_commons-0.0.7/crawler_commons.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      346 2023-05-12 10:45:36.000000 crawler_commons-0.0.7/crawler_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       19 2023-05-12 10:45:36.000000 crawler_commons-0.0.7/crawler_commons.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-12 10:45:36.000000 crawler_commons-0.0.7/crawler_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-12 10:45:36.000000 crawler_commons-0.0.7/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `crawler_commons-0.0.6/LICENSE` & `crawler_commons-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.6/crawapi/__init__.py` & `crawler_commons-0.0.7/crawapi/__init__.py`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.6/crawlutils/__init__.py` & `crawler_commons-0.0.7/crawlutils/__init__.py`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.6/crawlutils/date_utils.py` & `crawler_commons-0.0.7/crawlutils/date_utils.py`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.6/crawlutils/num_utils.py` & `crawler_commons-0.0.7/crawlutils/num_utils.py`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.6/crawlutils/soup_traversal.py` & `crawler_commons-0.0.7/crawlutils/soup_traversal.py`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.6/crawlutils/text_utils.py` & `crawler_commons-0.0.7/crawlutils/text_utils.py`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.6/setup.py` & `crawler_commons-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="crawler_commons",
-    version="0.0.6",
+    version="0.0.7",
     license='MIT',
     author="cheddars",
     author_email="nezahrish@gmail.com",
     description="crawler commons",
     long_description=open('README.md').read(),
     url="https://github.com/cheddars/crawler_commons",
     packages=setuptools.find_packages(exclude=("test",)),
```


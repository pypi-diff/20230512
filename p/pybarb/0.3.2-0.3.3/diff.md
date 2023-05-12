# Comparing `tmp/pybarb-0.3.2.tar.gz` & `tmp/pybarb-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybarb-0.3.2.tar", last modified: Thu May 11 11:39:43 2023, max compression
+gzip compressed data, was "pybarb-0.3.3.tar", last modified: Fri May 12 12:43:08 2023, max compression
```

## Comparing `pybarb-0.3.2.tar` & `pybarb-0.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 simon_business   (501) staff       (20)        0 2023-05-11 11:39:43.215998 pybarb-0.3.2/
--rw-r--r--   0 simon_business   (501) staff       (20)      200 2023-05-11 11:39:43.215762 pybarb-0.3.2/PKG-INFO
--rw-r--r--   0 simon_business   (501) staff       (20)     2744 2023-04-25 15:40:48.000000 pybarb-0.3.2/README.md
-drwxr-xr-x   0 simon_business   (501) staff       (20)        0 2023-05-11 11:39:43.213938 pybarb-0.3.2/pybarb/
--rw-r--r--   0 simon_business   (501) staff       (20)        0 2023-04-25 15:18:38.000000 pybarb-0.3.2/pybarb/__init__.py
--rw-r--r--   0 simon_business   (501) staff       (20)    23770 2023-04-25 15:18:38.000000 pybarb-0.3.2/pybarb/pybarb.py
-drwxr-xr-x   0 simon_business   (501) staff       (20)        0 2023-05-11 11:39:43.215429 pybarb-0.3.2/pybarb.egg-info/
--rw-r--r--   0 simon_business   (501) staff       (20)      200 2023-05-11 11:39:43.000000 pybarb-0.3.2/pybarb.egg-info/PKG-INFO
--rw-r--r--   0 simon_business   (501) staff       (20)      203 2023-05-11 11:39:43.000000 pybarb-0.3.2/pybarb.egg-info/SOURCES.txt
--rw-r--r--   0 simon_business   (501) staff       (20)        1 2023-05-11 11:39:43.000000 pybarb-0.3.2/pybarb.egg-info/dependency_links.txt
--rw-r--r--   0 simon_business   (501) staff       (20)       25 2023-05-11 11:39:43.000000 pybarb-0.3.2/pybarb.egg-info/requires.txt
--rw-r--r--   0 simon_business   (501) staff       (20)        7 2023-05-11 11:39:43.000000 pybarb-0.3.2/pybarb.egg-info/top_level.txt
--rw-r--r--   0 simon_business   (501) staff       (20)       38 2023-05-11 11:39:43.216086 pybarb-0.3.2/setup.cfg
--rw-r--r--   0 simon_business   (501) staff       (20)      384 2023-05-11 11:39:31.000000 pybarb-0.3.2/setup.py
+drwxr-xr-x   0 simon_business   (501) staff       (20)        0 2023-05-12 12:43:08.877211 pybarb-0.3.3/
+-rw-r--r--   0 simon_business   (501) staff       (20)      245 2023-05-12 12:43:08.876983 pybarb-0.3.3/PKG-INFO
+-rw-r--r--   0 simon_business   (501) staff       (20)     2744 2023-04-25 15:40:48.000000 pybarb-0.3.3/README.md
+drwxr-xr-x   0 simon_business   (501) staff       (20)        0 2023-05-12 12:43:08.874796 pybarb-0.3.3/pybarb/
+-rw-r--r--   0 simon_business   (501) staff       (20)       21 2023-05-12 12:41:57.000000 pybarb-0.3.3/pybarb/__init__.py
+-rw-r--r--   0 simon_business   (501) staff       (20)    23770 2023-04-25 15:18:38.000000 pybarb-0.3.3/pybarb/pybarb.py
+drwxr-xr-x   0 simon_business   (501) staff       (20)        0 2023-05-12 12:43:08.876606 pybarb-0.3.3/pybarb.egg-info/
+-rw-r--r--   0 simon_business   (501) staff       (20)      245 2023-05-12 12:43:08.000000 pybarb-0.3.3/pybarb.egg-info/PKG-INFO
+-rw-r--r--   0 simon_business   (501) staff       (20)      203 2023-05-12 12:43:08.000000 pybarb-0.3.3/pybarb.egg-info/SOURCES.txt
+-rw-r--r--   0 simon_business   (501) staff       (20)        1 2023-05-12 12:43:08.000000 pybarb-0.3.3/pybarb.egg-info/dependency_links.txt
+-rw-r--r--   0 simon_business   (501) staff       (20)       34 2023-05-12 12:43:08.000000 pybarb-0.3.3/pybarb.egg-info/requires.txt
+-rw-r--r--   0 simon_business   (501) staff       (20)        7 2023-05-12 12:43:08.000000 pybarb-0.3.3/pybarb.egg-info/top_level.txt
+-rw-r--r--   0 simon_business   (501) staff       (20)       38 2023-05-12 12:43:08.877304 pybarb-0.3.3/setup.cfg
+-rw-r--r--   0 simon_business   (501) staff       (20)      404 2023-05-12 12:42:25.000000 pybarb-0.3.3/setup.py
```

### Comparing `pybarb-0.3.2/README.md` & `pybarb-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pybarb-0.3.2/pybarb/pybarb.py` & `pybarb-0.3.3/pybarb/pybarb.py`

 * *Files identical despite different names*


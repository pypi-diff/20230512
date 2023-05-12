# Comparing `tmp/wombatoo-0.0.8.tar.gz` & `tmp/wombatoo-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Prashant\Desktop\wombatoo\dist\.tmp-0i8jp__a\wombatoo-0.0.8.tar", last modified: Fri May 12 10:31:20 2023, max compression
+gzip compressed data, was "C:\Users\Prashant\Desktop\wombatoo\dist\.tmp-oqicaxkm\wombatoo-0.0.9.tar", last modified: Fri May 12 12:37:50 2023, max compression
```

## Comparing `wombatoo-0.0.8.tar` & `wombatoo-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 10:31:20.000000 wombatoo-0.0.8/
--rw-rw-rw-   0        0        0     1092 2023-05-01 06:13:40.000000 wombatoo-0.0.8/LICENSE.md
--rw-rw-rw-   0        0        0      409 2023-05-12 10:31:20.000000 wombatoo-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-05-01 13:09:37.000000 wombatoo-0.0.8/README.md
--rw-rw-rw-   0        0        0      723 2023-05-12 10:30:44.000000 wombatoo-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 10:31:20.000000 wombatoo-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-12 10:31:20.000000 wombatoo-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-12 10:31:20.000000 wombatoo-0.0.8/src/wombatoo/
--rw-rw-rw-   0        0        0      189 2023-04-11 16:01:38.000000 wombatoo-0.0.8/src/wombatoo/DataCard.txt
--rw-rw-rw-   0        0        0        0 2023-05-01 07:27:57.000000 wombatoo-0.0.8/src/wombatoo/__init__.py
--rw-rw-rw-   0        0        0     8673 2023-05-12 10:27:46.000000 wombatoo-0.0.8/src/wombatoo/wombatoo.py
-drwxrwxrwx   0        0        0        0 2023-05-12 10:31:20.000000 wombatoo-0.0.8/src/wombatoo.egg-info/
--rw-rw-rw-   0        0        0      409 2023-05-12 10:31:20.000000 wombatoo-0.0.8/src/wombatoo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-05-12 10:31:20.000000 wombatoo-0.0.8/src/wombatoo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 10:31:20.000000 wombatoo-0.0.8/src/wombatoo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-05-12 10:31:20.000000 wombatoo-0.0.8/src/wombatoo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-12 10:31:20.000000 wombatoo-0.0.8/src/wombatoo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 12:37:50.000000 wombatoo-0.0.9/
+-rw-rw-rw-   0        0        0     1092 2023-05-01 06:13:40.000000 wombatoo-0.0.9/LICENSE.md
+-rw-rw-rw-   0        0        0      409 2023-05-12 12:37:50.000000 wombatoo-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-05-01 13:09:37.000000 wombatoo-0.0.9/README.md
+-rw-rw-rw-   0        0        0      723 2023-05-12 12:31:13.000000 wombatoo-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-12 12:37:50.000000 wombatoo-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-12 12:37:50.000000 wombatoo-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-12 12:37:50.000000 wombatoo-0.0.9/src/wombatoo/
+-rw-rw-rw-   0        0        0      189 2023-04-11 16:01:38.000000 wombatoo-0.0.9/src/wombatoo/DataCard.txt
+-rw-rw-rw-   0        0        0        0 2023-05-01 07:27:57.000000 wombatoo-0.0.9/src/wombatoo/__init__.py
+-rw-rw-rw-   0        0        0     8754 2023-05-12 12:30:57.000000 wombatoo-0.0.9/src/wombatoo/wombatoo.py
+drwxrwxrwx   0        0        0        0 2023-05-12 12:37:50.000000 wombatoo-0.0.9/src/wombatoo.egg-info/
+-rw-rw-rw-   0        0        0      409 2023-05-12 12:37:50.000000 wombatoo-0.0.9/src/wombatoo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-05-12 12:37:50.000000 wombatoo-0.0.9/src/wombatoo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 12:37:50.000000 wombatoo-0.0.9/src/wombatoo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-05-12 12:37:50.000000 wombatoo-0.0.9/src/wombatoo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-12 12:37:50.000000 wombatoo-0.0.9/src/wombatoo.egg-info/top_level.txt
```

### Comparing `wombatoo-0.0.8/LICENSE.md` & `wombatoo-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `wombatoo-0.0.8/pyproject.toml` & `wombatoo-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
                     
 [project]
 name = "wombatoo"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Prashant Singh", email="prashdash112@gmail.com" },
 ]
 description = "A Data-Ops tool for devs"
 readme = "README.md"
 requires-python = ">=3.6"
 dependencies = ["numpy==1.23.5",
```

### Comparing `wombatoo-0.0.8/src/wombatoo/wombatoo.py` & `wombatoo-0.0.9/src/wombatoo/wombatoo.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from datetime import datetime
 import os
 import random
 import string
 import hashlib
 import os
 from pyhtml2pdf import converter
+from distutils.sysconfig import get_python_lib
 
 def metric_summary(df, path_to_save=None, columns=None):
     '''
     Summarizes metrics of a dataframe:
 
     >>> from datetime import date
     >>> df = pd.DataFrame(
@@ -98,15 +99,15 @@
     df: pandas dataframe for which user wants to generate a data card
     
     path_to_save: user-specific location of data card txt file. 
                 Defaulted to current working directory.
     
     e.g: datacard(df, './DataCard.txt')
     '''
-    with open("DataCard.txt", "r+") as f:
+    with open(str(get_python_lib())+ "\wombatoo\DataCard.txt", "r+") as f:
         old = f.read()
     file_list = old.strip().split('\n')
     dt = datetime.now()
     file_list[2] = file_list[2] + str(dt)
     file_list[4] = file_list[4] + os.getlogin()
     arr = []
     for i in df.columns:
```


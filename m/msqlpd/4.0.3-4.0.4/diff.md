# Comparing `tmp/msqlpd-4.0.3.tar.gz` & `tmp/msqlpd-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msqlpd-4.0.3.tar", last modified: Sun May  7 11:20:45 2023, max compression
+gzip compressed data, was "msqlpd-4.0.4.tar", last modified: Fri May 12 08:55:41 2023, max compression
```

## Comparing `msqlpd-4.0.3.tar` & `msqlpd-4.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-07 11:20:45.656129 msqlpd-4.0.3/
--rwxrwxrwx   0 root         (0) root         (0)     1071 2023-05-07 10:45:43.000000 msqlpd-4.0.3/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      278 2023-05-07 11:20:45.655703 msqlpd-4.0.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      107 2023-05-07 11:20:44.000000 msqlpd-4.0.3/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-07 11:20:45.651814 msqlpd-4.0.3/msqlpd/
--rwxrwxrwx   0 root         (0) root         (0)       36 2023-05-07 10:45:43.000000 msqlpd-4.0.3/msqlpd/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-07 11:20:45.655145 msqlpd-4.0.3/msqlpd/src/
--rwxrwxrwx   0 root         (0) root         (0)    13819 2023-05-07 10:45:43.000000 msqlpd-4.0.3/msqlpd/src/connection.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-07 11:20:45.654677 msqlpd-4.0.3/msqlpd.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      278 2023-05-07 11:20:45.000000 msqlpd-4.0.3/msqlpd.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      219 2023-05-07 11:20:45.000000 msqlpd-4.0.3/msqlpd.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-07 11:20:45.000000 msqlpd-4.0.3/msqlpd.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       48 2023-05-07 11:20:45.000000 msqlpd-4.0.3/msqlpd.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-05-07 11:20:45.000000 msqlpd-4.0.3/msqlpd.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-07 11:20:45.656432 msqlpd-4.0.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      530 2023-05-07 11:20:09.000000 msqlpd-4.0.3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-12 08:55:41.369456 msqlpd-4.0.4/
+-rwxrwxrwx   0 root         (0) root         (0)     1071 2023-05-12 08:51:46.000000 msqlpd-4.0.4/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      278 2023-05-12 08:55:41.369251 msqlpd-4.0.4/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      107 2023-05-12 08:55:40.000000 msqlpd-4.0.4/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-12 08:55:41.366873 msqlpd-4.0.4/msqlpd/
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-05-12 08:51:46.000000 msqlpd-4.0.4/msqlpd/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-12 08:55:41.368835 msqlpd-4.0.4/msqlpd/src/
+-rwxrwxrwx   0 root         (0) root         (0)    13869 2023-05-12 08:52:38.000000 msqlpd-4.0.4/msqlpd/src/connection.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-12 08:55:41.368515 msqlpd-4.0.4/msqlpd.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      278 2023-05-12 08:55:41.000000 msqlpd-4.0.4/msqlpd.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      219 2023-05-12 08:55:41.000000 msqlpd-4.0.4/msqlpd.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-12 08:55:41.000000 msqlpd-4.0.4/msqlpd.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       48 2023-05-12 08:55:41.000000 msqlpd-4.0.4/msqlpd.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        7 2023-05-12 08:55:41.000000 msqlpd-4.0.4/msqlpd.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-12 08:55:41.369531 msqlpd-4.0.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      530 2023-05-12 08:52:52.000000 msqlpd-4.0.4/setup.py
```

### Comparing `msqlpd-4.0.3/LICENSE` & `msqlpd-4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `msqlpd-4.0.3/msqlpd/src/connection.py` & `msqlpd-4.0.4/msqlpd/src/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,16 @@
         return "integer"
     if "float" in dtype:
         return "float"
     if "double" in dtype:
         return "float"
     if "text" in dtype:
         return "string"
+    if "decimal" in dtype:
+        return "float"
     raise Exception(f"dtype {dtype} is not implemented yet.")
 
 class DataBase:
     def __init__(
         self,
         username: str,
         password: str,
```

### Comparing `msqlpd-4.0.3/setup.py` & `msqlpd-4.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="msqlpd",
-    version="4.0.3",
+    version="4.0.4",
     author="Moses Dastmard",
     description="return a path information",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'sqlalchemy',
         'pandas',
```


# Comparing `tmp/Dev-Helper-CLI-0.0.1.tar.gz` & `tmp/Dev-Helper-CLI-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Dev-Helper-CLI-0.0.1.tar", last modified: Fri May 12 04:03:13 2023, max compression
+gzip compressed data, was "Dev-Helper-CLI-0.0.2.tar", last modified: Fri May 12 04:11:13 2023, max compression
```

## Comparing `Dev-Helper-CLI-0.0.1.tar` & `Dev-Helper-CLI-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 04:03:13.398687 Dev-Helper-CLI-0.0.1/
-drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 04:03:13.398411 Dev-Helper-CLI-0.0.1/Dev_Helper_CLI.egg-info/
--rw-r--r--   0 luismoreno   (501) staff       (20)      551 2023-05-12 04:03:13.000000 Dev-Helper-CLI-0.0.1/Dev_Helper_CLI.egg-info/PKG-INFO
--rw-r--r--   0 luismoreno   (501) staff       (20)      271 2023-05-12 04:03:13.000000 Dev-Helper-CLI-0.0.1/Dev_Helper_CLI.egg-info/SOURCES.txt
--rw-r--r--   0 luismoreno   (501) staff       (20)        1 2023-05-12 04:03:13.000000 Dev-Helper-CLI-0.0.1/Dev_Helper_CLI.egg-info/dependency_links.txt
--rw-r--r--   0 luismoreno   (501) staff       (20)       36 2023-05-12 04:03:13.000000 Dev-Helper-CLI-0.0.1/Dev_Helper_CLI.egg-info/entry_points.txt
--rw-r--r--   0 luismoreno   (501) staff       (20)      957 2023-05-12 04:03:13.000000 Dev-Helper-CLI-0.0.1/Dev_Helper_CLI.egg-info/requires.txt
--rw-r--r--   0 luismoreno   (501) staff       (20)        1 2023-05-12 04:03:13.000000 Dev-Helper-CLI-0.0.1/Dev_Helper_CLI.egg-info/top_level.txt
--rw-r--r--   0 luismoreno   (501) staff       (20)     1065 2023-04-22 16:06:17.000000 Dev-Helper-CLI-0.0.1/LICENSE
--rw-r--r--   0 luismoreno   (501) staff       (20)      551 2023-05-12 04:03:13.398571 Dev-Helper-CLI-0.0.1/PKG-INFO
--rw-r--r--   0 luismoreno   (501) staff       (20)       19 2023-04-22 16:06:17.000000 Dev-Helper-CLI-0.0.1/README.md
--rw-r--r--   0 luismoreno   (501) staff       (20)       84 2023-05-11 22:07:52.000000 Dev-Helper-CLI-0.0.1/pyproject.toml
--rw-r--r--   0 luismoreno   (501) staff       (20)       38 2023-05-12 04:03:13.398727 Dev-Helper-CLI-0.0.1/setup.cfg
--rw-r--r--   0 luismoreno   (501) staff       (20)     1005 2023-05-12 04:02:57.000000 Dev-Helper-CLI-0.0.1/setup.py
+drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 04:11:13.003347 Dev-Helper-CLI-0.0.2/
+drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 04:11:13.003078 Dev-Helper-CLI-0.0.2/Dev_Helper_CLI.egg-info/
+-rw-r--r--   0 luismoreno   (501) staff       (20)      551 2023-05-12 04:11:12.000000 Dev-Helper-CLI-0.0.2/Dev_Helper_CLI.egg-info/PKG-INFO
+-rw-r--r--   0 luismoreno   (501) staff       (20)      271 2023-05-12 04:11:12.000000 Dev-Helper-CLI-0.0.2/Dev_Helper_CLI.egg-info/SOURCES.txt
+-rw-r--r--   0 luismoreno   (501) staff       (20)        1 2023-05-12 04:11:12.000000 Dev-Helper-CLI-0.0.2/Dev_Helper_CLI.egg-info/dependency_links.txt
+-rw-r--r--   0 luismoreno   (501) staff       (20)       36 2023-05-12 04:11:12.000000 Dev-Helper-CLI-0.0.2/Dev_Helper_CLI.egg-info/entry_points.txt
+-rw-r--r--   0 luismoreno   (501) staff       (20)      957 2023-05-12 04:11:12.000000 Dev-Helper-CLI-0.0.2/Dev_Helper_CLI.egg-info/requires.txt
+-rw-r--r--   0 luismoreno   (501) staff       (20)        1 2023-05-12 04:11:12.000000 Dev-Helper-CLI-0.0.2/Dev_Helper_CLI.egg-info/top_level.txt
+-rw-r--r--   0 luismoreno   (501) staff       (20)     1065 2023-04-22 16:06:17.000000 Dev-Helper-CLI-0.0.2/LICENSE
+-rw-r--r--   0 luismoreno   (501) staff       (20)      551 2023-05-12 04:11:13.003233 Dev-Helper-CLI-0.0.2/PKG-INFO
+-rw-r--r--   0 luismoreno   (501) staff       (20)       19 2023-04-22 16:06:17.000000 Dev-Helper-CLI-0.0.2/README.md
+-rw-r--r--   0 luismoreno   (501) staff       (20)       84 2023-05-11 22:07:52.000000 Dev-Helper-CLI-0.0.2/pyproject.toml
+-rw-r--r--   0 luismoreno   (501) staff       (20)       38 2023-05-12 04:11:13.003382 Dev-Helper-CLI-0.0.2/setup.cfg
+-rw-r--r--   0 luismoreno   (501) staff       (20)     1091 2023-05-12 04:11:05.000000 Dev-Helper-CLI-0.0.2/setup.py
```

### Comparing `Dev-Helper-CLI-0.0.1/Dev_Helper_CLI.egg-info/PKG-INFO` & `Dev-Helper-CLI-0.0.2/Dev_Helper_CLI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dev-Helper-CLI
-Version: 0.0.1
+Version: 0.0.2
 Summary: A CLI program to help devs be more productive.
 Home-page: https://github.com/luigicfh/Dev-Helper-2.0
 Author: Luis Moreno
 Author-email: luis.cfh.90@gmail.com
 Project-URL: Bug Tracker, https://github.com/luigicfh/Dev-Helper-2.0/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Dev-Helper-CLI-0.0.1/Dev_Helper_CLI.egg-info/requires.txt` & `Dev-Helper-CLI-0.0.2/Dev_Helper_CLI.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Dev-Helper-CLI-0.0.1/LICENSE` & `Dev-Helper-CLI-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Dev-Helper-CLI-0.0.1/PKG-INFO` & `Dev-Helper-CLI-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dev-Helper-CLI
-Version: 0.0.1
+Version: 0.0.2
 Summary: A CLI program to help devs be more productive.
 Home-page: https://github.com/luigicfh/Dev-Helper-2.0
 Author: Luis Moreno
 Author-email: luis.cfh.90@gmail.com
 Project-URL: Bug Tracker, https://github.com/luigicfh/Dev-Helper-2.0/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Dev-Helper-CLI-0.0.1/setup.py` & `Dev-Helper-CLI-0.0.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import setuptools
+import os
+
+cwd = os.getcwd()
+requirements_path = os.path.join(cwd, "requirements.txt")
 
 with open("README.md", "r", encoding="utf-8") as fhand:
     long_description = fhand.read()
 
-REQUIREMENTS = [i.strip() for i in open("requirements.txt").readlines()]
+REQUIREMENTS = [i.strip() for i in open(requirements_path).readlines()]
 
 setuptools.setup(
     name="Dev-Helper-CLI",
-    version="0.0.1",
+    version="0.0.2",
     author="Luis Moreno",
     author_email="luis.cfh.90@gmail.com",
     description=("A CLI program to help devs be more productive."),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/luigicfh/Dev-Helper-2.0",
     project_urls={
```


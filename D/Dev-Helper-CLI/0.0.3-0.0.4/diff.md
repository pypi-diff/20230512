# Comparing `tmp/Dev-Helper-CLI-0.0.3.tar.gz` & `tmp/Dev-Helper-CLI-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Dev-Helper-CLI-0.0.3.tar", last modified: Fri May 12 04:17:34 2023, max compression
+gzip compressed data, was "Dev-Helper-CLI-0.0.4.tar", last modified: Fri May 12 04:22:33 2023, max compression
```

## Comparing `Dev-Helper-CLI-0.0.3.tar` & `Dev-Helper-CLI-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,21 @@
-drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 04:17:34.560076 Dev-Helper-CLI-0.0.3/
-drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 04:17:34.559772 Dev-Helper-CLI-0.0.3/Dev_Helper_CLI.egg-info/
--rw-r--r--   0 luismoreno   (501) staff       (20)      551 2023-05-12 04:17:34.000000 Dev-Helper-CLI-0.0.3/Dev_Helper_CLI.egg-info/PKG-INFO
--rw-r--r--   0 luismoreno   (501) staff       (20)      271 2023-05-12 04:17:34.000000 Dev-Helper-CLI-0.0.3/Dev_Helper_CLI.egg-info/SOURCES.txt
--rw-r--r--   0 luismoreno   (501) staff       (20)        1 2023-05-12 04:17:34.000000 Dev-Helper-CLI-0.0.3/Dev_Helper_CLI.egg-info/dependency_links.txt
--rw-r--r--   0 luismoreno   (501) staff       (20)       36 2023-05-12 04:17:34.000000 Dev-Helper-CLI-0.0.3/Dev_Helper_CLI.egg-info/entry_points.txt
--rw-r--r--   0 luismoreno   (501) staff       (20)       33 2023-05-12 04:17:34.000000 Dev-Helper-CLI-0.0.3/Dev_Helper_CLI.egg-info/requires.txt
--rw-r--r--   0 luismoreno   (501) staff       (20)        1 2023-05-12 04:17:34.000000 Dev-Helper-CLI-0.0.3/Dev_Helper_CLI.egg-info/top_level.txt
--rw-r--r--   0 luismoreno   (501) staff       (20)     1065 2023-04-22 16:06:17.000000 Dev-Helper-CLI-0.0.3/LICENSE
--rw-r--r--   0 luismoreno   (501) staff       (20)      551 2023-05-12 04:17:34.559952 Dev-Helper-CLI-0.0.3/PKG-INFO
--rw-r--r--   0 luismoreno   (501) staff       (20)       19 2023-04-22 16:06:17.000000 Dev-Helper-CLI-0.0.3/README.md
--rw-r--r--   0 luismoreno   (501) staff       (20)       84 2023-05-11 22:07:52.000000 Dev-Helper-CLI-0.0.3/pyproject.toml
--rw-r--r--   0 luismoreno   (501) staff       (20)       38 2023-05-12 04:17:34.560115 Dev-Helper-CLI-0.0.3/setup.cfg
--rw-r--r--   0 luismoreno   (501) staff       (20)      993 2023-05-12 04:17:29.000000 Dev-Helper-CLI-0.0.3/setup.py
+drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 04:22:33.757272 Dev-Helper-CLI-0.0.4/
+drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 04:22:33.756060 Dev-Helper-CLI-0.0.4/Dev_Helper_CLI.egg-info/
+-rw-r--r--   0 luismoreno   (501) staff       (20)      551 2023-05-12 04:22:33.000000 Dev-Helper-CLI-0.0.4/Dev_Helper_CLI.egg-info/PKG-INFO
+-rw-r--r--   0 luismoreno   (501) staff       (20)      371 2023-05-12 04:22:33.000000 Dev-Helper-CLI-0.0.4/Dev_Helper_CLI.egg-info/SOURCES.txt
+-rw-r--r--   0 luismoreno   (501) staff       (20)        1 2023-05-12 04:22:33.000000 Dev-Helper-CLI-0.0.4/Dev_Helper_CLI.egg-info/dependency_links.txt
+-rw-r--r--   0 luismoreno   (501) staff       (20)       36 2023-05-12 04:22:33.000000 Dev-Helper-CLI-0.0.4/Dev_Helper_CLI.egg-info/entry_points.txt
+-rw-r--r--   0 luismoreno   (501) staff       (20)       33 2023-05-12 04:22:33.000000 Dev-Helper-CLI-0.0.4/Dev_Helper_CLI.egg-info/requires.txt
+-rw-r--r--   0 luismoreno   (501) staff       (20)        3 2023-05-12 04:22:33.000000 Dev-Helper-CLI-0.0.4/Dev_Helper_CLI.egg-info/top_level.txt
+-rw-r--r--   0 luismoreno   (501) staff       (20)     1065 2023-04-22 16:06:17.000000 Dev-Helper-CLI-0.0.4/LICENSE
+-rw-r--r--   0 luismoreno   (501) staff       (20)      551 2023-05-12 04:22:33.757083 Dev-Helper-CLI-0.0.4/PKG-INFO
+-rw-r--r--   0 luismoreno   (501) staff       (20)       19 2023-04-22 16:06:17.000000 Dev-Helper-CLI-0.0.4/README.md
+drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 04:22:33.756260 Dev-Helper-CLI-0.0.4/dh/
+-rw-r--r--   0 luismoreno   (501) staff       (20)        0 2023-05-12 04:22:00.000000 Dev-Helper-CLI-0.0.4/dh/__init__.py
+drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 04:22:33.756808 Dev-Helper-CLI-0.0.4/dh/backend/
+-rw-r--r--   0 luismoreno   (501) staff       (20)        0 2023-04-22 17:18:01.000000 Dev-Helper-CLI-0.0.4/dh/backend/__init__.py
+-rw-r--r--   0 luismoreno   (501) staff       (20)     1546 2023-05-10 22:26:56.000000 Dev-Helper-CLI-0.0.4/dh/backend/document_db.py
+-rw-r--r--   0 luismoreno   (501) staff       (20)     1314 2023-05-11 20:19:01.000000 Dev-Helper-CLI-0.0.4/dh/backend/validations.py
+-rw-r--r--   0 luismoreno   (501) staff       (20)     7506 2023-05-12 00:58:43.000000 Dev-Helper-CLI-0.0.4/dh/cli.py
+-rw-r--r--   0 luismoreno   (501) staff       (20)       84 2023-05-11 22:07:52.000000 Dev-Helper-CLI-0.0.4/pyproject.toml
+-rw-r--r--   0 luismoreno   (501) staff       (20)       38 2023-05-12 04:22:33.757312 Dev-Helper-CLI-0.0.4/setup.cfg
+-rw-r--r--   0 luismoreno   (501) staff       (20)      993 2023-05-12 04:22:31.000000 Dev-Helper-CLI-0.0.4/setup.py
```

### Comparing `Dev-Helper-CLI-0.0.3/Dev_Helper_CLI.egg-info/PKG-INFO` & `Dev-Helper-CLI-0.0.4/Dev_Helper_CLI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dev-Helper-CLI
-Version: 0.0.3
+Version: 0.0.4
 Summary: A CLI program to help devs be more productive.
 Home-page: https://github.com/luigicfh/Dev-Helper-2.0
 Author: Luis Moreno
 Author-email: luis.cfh.90@gmail.com
 Project-URL: Bug Tracker, https://github.com/luigicfh/Dev-Helper-2.0/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Dev-Helper-CLI-0.0.3/LICENSE` & `Dev-Helper-CLI-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Dev-Helper-CLI-0.0.3/PKG-INFO` & `Dev-Helper-CLI-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dev-Helper-CLI
-Version: 0.0.3
+Version: 0.0.4
 Summary: A CLI program to help devs be more productive.
 Home-page: https://github.com/luigicfh/Dev-Helper-2.0
 Author: Luis Moreno
 Author-email: luis.cfh.90@gmail.com
 Project-URL: Bug Tracker, https://github.com/luigicfh/Dev-Helper-2.0/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Dev-Helper-CLI-0.0.3/setup.py` & `Dev-Helper-CLI-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 cwd = os.getcwd()
 
 with open("README.md", "r", encoding="utf-8") as fhand:
     long_description = fhand.read()
 
 setuptools.setup(
     name="Dev-Helper-CLI",
-    version="0.0.3",
+    version="0.0.4",
     author="Luis Moreno",
     author_email="luis.cfh.90@gmail.com",
     description=("A CLI program to help devs be more productive."),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/luigicfh/Dev-Helper-2.0",
     project_urls={
```


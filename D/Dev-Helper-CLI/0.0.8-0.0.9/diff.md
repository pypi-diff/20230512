# Comparing `tmp/Dev-Helper-CLI-0.0.8.tar.gz` & `tmp/Dev-Helper-CLI-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Dev-Helper-CLI-0.0.8.tar", last modified: Fri May 12 14:47:04 2023, max compression
+gzip compressed data, was "Dev-Helper-CLI-0.0.9.tar", last modified: Fri May 12 14:49:57 2023, max compression
```

## Comparing `Dev-Helper-CLI-0.0.8.tar` & `Dev-Helper-CLI-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 14:47:04.030302 Dev-Helper-CLI-0.0.8/
-drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 14:47:04.028641 Dev-Helper-CLI-0.0.8/Dev_Helper_CLI.egg-info/
--rw-r--r--   0 luismoreno   (501) staff       (20)      551 2023-05-12 14:47:03.000000 Dev-Helper-CLI-0.0.8/Dev_Helper_CLI.egg-info/PKG-INFO
--rw-r--r--   0 luismoreno   (501) staff       (20)      371 2023-05-12 14:47:04.000000 Dev-Helper-CLI-0.0.8/Dev_Helper_CLI.egg-info/SOURCES.txt
--rw-r--r--   0 luismoreno   (501) staff       (20)        1 2023-05-12 14:47:03.000000 Dev-Helper-CLI-0.0.8/Dev_Helper_CLI.egg-info/dependency_links.txt
--rw-r--r--   0 luismoreno   (501) staff       (20)       36 2023-05-12 14:47:03.000000 Dev-Helper-CLI-0.0.8/Dev_Helper_CLI.egg-info/entry_points.txt
--rw-r--r--   0 luismoreno   (501) staff       (20)       42 2023-05-12 14:47:03.000000 Dev-Helper-CLI-0.0.8/Dev_Helper_CLI.egg-info/requires.txt
--rw-r--r--   0 luismoreno   (501) staff       (20)        3 2023-05-12 14:47:03.000000 Dev-Helper-CLI-0.0.8/Dev_Helper_CLI.egg-info/top_level.txt
--rw-r--r--   0 luismoreno   (501) staff       (20)     1065 2023-04-22 16:06:17.000000 Dev-Helper-CLI-0.0.8/LICENSE
--rw-r--r--   0 luismoreno   (501) staff       (20)      551 2023-05-12 14:47:04.030097 Dev-Helper-CLI-0.0.8/PKG-INFO
--rw-r--r--   0 luismoreno   (501) staff       (20)       19 2023-04-22 16:06:17.000000 Dev-Helper-CLI-0.0.8/README.md
-drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 14:47:04.028845 Dev-Helper-CLI-0.0.8/dh/
--rw-r--r--   0 luismoreno   (501) staff       (20)        0 2023-05-12 04:22:00.000000 Dev-Helper-CLI-0.0.8/dh/__init__.py
-drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 14:47:04.029686 Dev-Helper-CLI-0.0.8/dh/backend/
--rw-r--r--   0 luismoreno   (501) staff       (20)        0 2023-04-22 17:18:01.000000 Dev-Helper-CLI-0.0.8/dh/backend/__init__.py
--rw-r--r--   0 luismoreno   (501) staff       (20)     1546 2023-05-10 22:26:56.000000 Dev-Helper-CLI-0.0.8/dh/backend/document_db.py
--rw-r--r--   0 luismoreno   (501) staff       (20)     1314 2023-05-11 20:19:01.000000 Dev-Helper-CLI-0.0.8/dh/backend/validations.py
--rw-r--r--   0 luismoreno   (501) staff       (20)     7538 2023-05-12 14:42:00.000000 Dev-Helper-CLI-0.0.8/dh/cli.py
--rw-r--r--   0 luismoreno   (501) staff       (20)       84 2023-05-11 22:07:52.000000 Dev-Helper-CLI-0.0.8/pyproject.toml
--rw-r--r--   0 luismoreno   (501) staff       (20)       38 2023-05-12 14:47:04.030342 Dev-Helper-CLI-0.0.8/setup.cfg
--rw-r--r--   0 luismoreno   (501) staff       (20)     1005 2023-05-12 14:46:53.000000 Dev-Helper-CLI-0.0.8/setup.py
+drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 14:49:57.313794 Dev-Helper-CLI-0.0.9/
+drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 14:49:57.312574 Dev-Helper-CLI-0.0.9/Dev_Helper_CLI.egg-info/
+-rw-r--r--   0 luismoreno   (501) staff       (20)      551 2023-05-12 14:49:57.000000 Dev-Helper-CLI-0.0.9/Dev_Helper_CLI.egg-info/PKG-INFO
+-rw-r--r--   0 luismoreno   (501) staff       (20)      371 2023-05-12 14:49:57.000000 Dev-Helper-CLI-0.0.9/Dev_Helper_CLI.egg-info/SOURCES.txt
+-rw-r--r--   0 luismoreno   (501) staff       (20)        1 2023-05-12 14:49:57.000000 Dev-Helper-CLI-0.0.9/Dev_Helper_CLI.egg-info/dependency_links.txt
+-rw-r--r--   0 luismoreno   (501) staff       (20)       36 2023-05-12 14:49:57.000000 Dev-Helper-CLI-0.0.9/Dev_Helper_CLI.egg-info/entry_points.txt
+-rw-r--r--   0 luismoreno   (501) staff       (20)       42 2023-05-12 14:49:57.000000 Dev-Helper-CLI-0.0.9/Dev_Helper_CLI.egg-info/requires.txt
+-rw-r--r--   0 luismoreno   (501) staff       (20)        3 2023-05-12 14:49:57.000000 Dev-Helper-CLI-0.0.9/Dev_Helper_CLI.egg-info/top_level.txt
+-rw-r--r--   0 luismoreno   (501) staff       (20)     1065 2023-04-22 16:06:17.000000 Dev-Helper-CLI-0.0.9/LICENSE
+-rw-r--r--   0 luismoreno   (501) staff       (20)      551 2023-05-12 14:49:57.313609 Dev-Helper-CLI-0.0.9/PKG-INFO
+-rw-r--r--   0 luismoreno   (501) staff       (20)       19 2023-04-22 16:06:17.000000 Dev-Helper-CLI-0.0.9/README.md
+drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 14:49:57.312775 Dev-Helper-CLI-0.0.9/dh/
+-rw-r--r--   0 luismoreno   (501) staff       (20)        0 2023-05-12 04:22:00.000000 Dev-Helper-CLI-0.0.9/dh/__init__.py
+drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 14:49:57.313320 Dev-Helper-CLI-0.0.9/dh/backend/
+-rw-r--r--   0 luismoreno   (501) staff       (20)        0 2023-04-22 17:18:01.000000 Dev-Helper-CLI-0.0.9/dh/backend/__init__.py
+-rw-r--r--   0 luismoreno   (501) staff       (20)     1546 2023-05-10 22:26:56.000000 Dev-Helper-CLI-0.0.9/dh/backend/document_db.py
+-rw-r--r--   0 luismoreno   (501) staff       (20)     1314 2023-05-11 20:19:01.000000 Dev-Helper-CLI-0.0.9/dh/backend/validations.py
+-rw-r--r--   0 luismoreno   (501) staff       (20)     7529 2023-05-12 14:49:31.000000 Dev-Helper-CLI-0.0.9/dh/cli.py
+-rw-r--r--   0 luismoreno   (501) staff       (20)       84 2023-05-11 22:07:52.000000 Dev-Helper-CLI-0.0.9/pyproject.toml
+-rw-r--r--   0 luismoreno   (501) staff       (20)       38 2023-05-12 14:49:57.313835 Dev-Helper-CLI-0.0.9/setup.cfg
+-rw-r--r--   0 luismoreno   (501) staff       (20)     1005 2023-05-12 14:49:54.000000 Dev-Helper-CLI-0.0.9/setup.py
```

### Comparing `Dev-Helper-CLI-0.0.8/Dev_Helper_CLI.egg-info/PKG-INFO` & `Dev-Helper-CLI-0.0.9/Dev_Helper_CLI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dev-Helper-CLI
-Version: 0.0.8
+Version: 0.0.9
 Summary: A CLI program to help devs be more productive.
 Home-page: https://github.com/luigicfh/Dev-Helper-2.0
 Author: Luis Moreno
 Author-email: luis.cfh.90@gmail.com
 Project-URL: Bug Tracker, https://github.com/luigicfh/Dev-Helper-2.0/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Dev-Helper-CLI-0.0.8/LICENSE` & `Dev-Helper-CLI-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Dev-Helper-CLI-0.0.8/PKG-INFO` & `Dev-Helper-CLI-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dev-Helper-CLI
-Version: 0.0.8
+Version: 0.0.9
 Summary: A CLI program to help devs be more productive.
 Home-page: https://github.com/luigicfh/Dev-Helper-2.0
 Author: Luis Moreno
 Author-email: luis.cfh.90@gmail.com
 Project-URL: Bug Tracker, https://github.com/luigicfh/Dev-Helper-2.0/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Dev-Helper-CLI-0.0.8/dh/backend/document_db.py` & `Dev-Helper-CLI-0.0.9/dh/backend/document_db.py`

 * *Files identical despite different names*

### Comparing `Dev-Helper-CLI-0.0.8/dh/backend/validations.py` & `Dev-Helper-CLI-0.0.9/dh/backend/validations.py`

 * *Files identical despite different names*

### Comparing `Dev-Helper-CLI-0.0.8/dh/cli.py` & `Dev-Helper-CLI-0.0.9/dh/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,15 @@
         db.save()
         print(f"Command {args.shortcut} updated successfuly.")
         return
     
     if args.cmd == commands[4]:
         validate_run_input(args.shortcut)
         active_config = db.data.get("activeConfig")
-        if "project" not in active_config:
+        if active_config is None:
             print("It seems that you have not activated a project.")
             project = input(
             f"Please provide the project name of the command {args.shortcut}: ")
             if project is None:
                 raise ValueError("Please provide a valid project name.")
             if project not in db.data.keys():
                 raise ValueError(f"Project {project} does not exist.")
```

### Comparing `Dev-Helper-CLI-0.0.8/setup.py` & `Dev-Helper-CLI-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 cwd = os.getcwd()
 
 with open("README.md", "r", encoding="utf-8") as fhand:
     long_description = fhand.read()
 
 setuptools.setup(
     name="Dev-Helper-CLI",
-    version="0.0.8",
+    version="0.0.9",
     author="Luis Moreno",
     author_email="luis.cfh.90@gmail.com",
     description=("A CLI program to help devs be more productive."),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/luigicfh/Dev-Helper-2.0",
     project_urls={
```


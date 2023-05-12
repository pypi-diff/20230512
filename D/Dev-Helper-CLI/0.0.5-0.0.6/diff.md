# Comparing `tmp/Dev-Helper-CLI-0.0.5.tar.gz` & `tmp/Dev-Helper-CLI-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Dev-Helper-CLI-0.0.5.tar", last modified: Fri May 12 04:28:35 2023, max compression
+gzip compressed data, was "Dev-Helper-CLI-0.0.6.tar", last modified: Fri May 12 04:34:23 2023, max compression
```

## Comparing `Dev-Helper-CLI-0.0.5.tar` & `Dev-Helper-CLI-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 04:28:35.585040 Dev-Helper-CLI-0.0.5/
-drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 04:28:35.583604 Dev-Helper-CLI-0.0.5/Dev_Helper_CLI.egg-info/
--rw-r--r--   0 luismoreno   (501) staff       (20)      551 2023-05-12 04:28:35.000000 Dev-Helper-CLI-0.0.5/Dev_Helper_CLI.egg-info/PKG-INFO
--rw-r--r--   0 luismoreno   (501) staff       (20)      371 2023-05-12 04:28:35.000000 Dev-Helper-CLI-0.0.5/Dev_Helper_CLI.egg-info/SOURCES.txt
--rw-r--r--   0 luismoreno   (501) staff       (20)        1 2023-05-12 04:28:35.000000 Dev-Helper-CLI-0.0.5/Dev_Helper_CLI.egg-info/dependency_links.txt
--rw-r--r--   0 luismoreno   (501) staff       (20)       36 2023-05-12 04:28:35.000000 Dev-Helper-CLI-0.0.5/Dev_Helper_CLI.egg-info/entry_points.txt
--rw-r--r--   0 luismoreno   (501) staff       (20)       33 2023-05-12 04:28:35.000000 Dev-Helper-CLI-0.0.5/Dev_Helper_CLI.egg-info/requires.txt
--rw-r--r--   0 luismoreno   (501) staff       (20)        3 2023-05-12 04:28:35.000000 Dev-Helper-CLI-0.0.5/Dev_Helper_CLI.egg-info/top_level.txt
--rw-r--r--   0 luismoreno   (501) staff       (20)     1065 2023-04-22 16:06:17.000000 Dev-Helper-CLI-0.0.5/LICENSE
--rw-r--r--   0 luismoreno   (501) staff       (20)      551 2023-05-12 04:28:35.584860 Dev-Helper-CLI-0.0.5/PKG-INFO
--rw-r--r--   0 luismoreno   (501) staff       (20)       19 2023-04-22 16:06:17.000000 Dev-Helper-CLI-0.0.5/README.md
-drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 04:28:35.583803 Dev-Helper-CLI-0.0.5/dh/
--rw-r--r--   0 luismoreno   (501) staff       (20)        0 2023-05-12 04:22:00.000000 Dev-Helper-CLI-0.0.5/dh/__init__.py
-drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 04:28:35.584561 Dev-Helper-CLI-0.0.5/dh/backend/
--rw-r--r--   0 luismoreno   (501) staff       (20)        0 2023-04-22 17:18:01.000000 Dev-Helper-CLI-0.0.5/dh/backend/__init__.py
--rw-r--r--   0 luismoreno   (501) staff       (20)     1546 2023-05-10 22:26:56.000000 Dev-Helper-CLI-0.0.5/dh/backend/document_db.py
--rw-r--r--   0 luismoreno   (501) staff       (20)     1314 2023-05-11 20:19:01.000000 Dev-Helper-CLI-0.0.5/dh/backend/validations.py
--rw-r--r--   0 luismoreno   (501) staff       (20)     7508 2023-05-12 04:28:17.000000 Dev-Helper-CLI-0.0.5/dh/cli.py
--rw-r--r--   0 luismoreno   (501) staff       (20)       84 2023-05-11 22:07:52.000000 Dev-Helper-CLI-0.0.5/pyproject.toml
--rw-r--r--   0 luismoreno   (501) staff       (20)       38 2023-05-12 04:28:35.585208 Dev-Helper-CLI-0.0.5/setup.cfg
--rw-r--r--   0 luismoreno   (501) staff       (20)      993 2023-05-12 04:28:32.000000 Dev-Helper-CLI-0.0.5/setup.py
+drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 04:34:23.723067 Dev-Helper-CLI-0.0.6/
+drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 04:34:23.721800 Dev-Helper-CLI-0.0.6/Dev_Helper_CLI.egg-info/
+-rw-r--r--   0 luismoreno   (501) staff       (20)      551 2023-05-12 04:34:23.000000 Dev-Helper-CLI-0.0.6/Dev_Helper_CLI.egg-info/PKG-INFO
+-rw-r--r--   0 luismoreno   (501) staff       (20)      371 2023-05-12 04:34:23.000000 Dev-Helper-CLI-0.0.6/Dev_Helper_CLI.egg-info/SOURCES.txt
+-rw-r--r--   0 luismoreno   (501) staff       (20)        1 2023-05-12 04:34:23.000000 Dev-Helper-CLI-0.0.6/Dev_Helper_CLI.egg-info/dependency_links.txt
+-rw-r--r--   0 luismoreno   (501) staff       (20)       36 2023-05-12 04:34:23.000000 Dev-Helper-CLI-0.0.6/Dev_Helper_CLI.egg-info/entry_points.txt
+-rw-r--r--   0 luismoreno   (501) staff       (20)       42 2023-05-12 04:34:23.000000 Dev-Helper-CLI-0.0.6/Dev_Helper_CLI.egg-info/requires.txt
+-rw-r--r--   0 luismoreno   (501) staff       (20)        3 2023-05-12 04:34:23.000000 Dev-Helper-CLI-0.0.6/Dev_Helper_CLI.egg-info/top_level.txt
+-rw-r--r--   0 luismoreno   (501) staff       (20)     1065 2023-04-22 16:06:17.000000 Dev-Helper-CLI-0.0.6/LICENSE
+-rw-r--r--   0 luismoreno   (501) staff       (20)      551 2023-05-12 04:34:23.722892 Dev-Helper-CLI-0.0.6/PKG-INFO
+-rw-r--r--   0 luismoreno   (501) staff       (20)       19 2023-04-22 16:06:17.000000 Dev-Helper-CLI-0.0.6/README.md
+drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 04:34:23.722006 Dev-Helper-CLI-0.0.6/dh/
+-rw-r--r--   0 luismoreno   (501) staff       (20)        0 2023-05-12 04:22:00.000000 Dev-Helper-CLI-0.0.6/dh/__init__.py
+drwxr-xr-x   0 luismoreno   (501) staff       (20)        0 2023-05-12 04:34:23.722541 Dev-Helper-CLI-0.0.6/dh/backend/
+-rw-r--r--   0 luismoreno   (501) staff       (20)        0 2023-04-22 17:18:01.000000 Dev-Helper-CLI-0.0.6/dh/backend/__init__.py
+-rw-r--r--   0 luismoreno   (501) staff       (20)     1546 2023-05-10 22:26:56.000000 Dev-Helper-CLI-0.0.6/dh/backend/document_db.py
+-rw-r--r--   0 luismoreno   (501) staff       (20)     1314 2023-05-11 20:19:01.000000 Dev-Helper-CLI-0.0.6/dh/backend/validations.py
+-rw-r--r--   0 luismoreno   (501) staff       (20)     7508 2023-05-12 04:28:17.000000 Dev-Helper-CLI-0.0.6/dh/cli.py
+-rw-r--r--   0 luismoreno   (501) staff       (20)       84 2023-05-11 22:07:52.000000 Dev-Helper-CLI-0.0.6/pyproject.toml
+-rw-r--r--   0 luismoreno   (501) staff       (20)       38 2023-05-12 04:34:23.723110 Dev-Helper-CLI-0.0.6/setup.cfg
+-rw-r--r--   0 luismoreno   (501) staff       (20)     1005 2023-05-12 04:34:16.000000 Dev-Helper-CLI-0.0.6/setup.py
```

### Comparing `Dev-Helper-CLI-0.0.5/Dev_Helper_CLI.egg-info/PKG-INFO` & `Dev-Helper-CLI-0.0.6/Dev_Helper_CLI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dev-Helper-CLI
-Version: 0.0.5
+Version: 0.0.6
 Summary: A CLI program to help devs be more productive.
 Home-page: https://github.com/luigicfh/Dev-Helper-2.0
 Author: Luis Moreno
 Author-email: luis.cfh.90@gmail.com
 Project-URL: Bug Tracker, https://github.com/luigicfh/Dev-Helper-2.0/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Dev-Helper-CLI-0.0.5/LICENSE` & `Dev-Helper-CLI-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Dev-Helper-CLI-0.0.5/PKG-INFO` & `Dev-Helper-CLI-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dev-Helper-CLI
-Version: 0.0.5
+Version: 0.0.6
 Summary: A CLI program to help devs be more productive.
 Home-page: https://github.com/luigicfh/Dev-Helper-2.0
 Author: Luis Moreno
 Author-email: luis.cfh.90@gmail.com
 Project-URL: Bug Tracker, https://github.com/luigicfh/Dev-Helper-2.0/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Dev-Helper-CLI-0.0.5/dh/backend/document_db.py` & `Dev-Helper-CLI-0.0.6/dh/backend/document_db.py`

 * *Files identical despite different names*

### Comparing `Dev-Helper-CLI-0.0.5/dh/backend/validations.py` & `Dev-Helper-CLI-0.0.6/dh/backend/validations.py`

 * *Files identical despite different names*

### Comparing `Dev-Helper-CLI-0.0.5/dh/cli.py` & `Dev-Helper-CLI-0.0.6/dh/cli.py`

 * *Files identical despite different names*

### Comparing `Dev-Helper-CLI-0.0.5/setup.py` & `Dev-Helper-CLI-0.0.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 cwd = os.getcwd()
 
 with open("README.md", "r", encoding="utf-8") as fhand:
     long_description = fhand.read()
 
 setuptools.setup(
     name="Dev-Helper-CLI",
-    version="0.0.5",
+    version="0.0.6",
     author="Luis Moreno",
     author_email="luis.cfh.90@gmail.com",
     description=("A CLI program to help devs be more productive."),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/luigicfh/Dev-Helper-2.0",
     project_urls={
         "Bug Tracker": "https://github.com/luigicfh/Dev-Helper-2.0/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires=["PyYAML", "openai", "streamlit", "Pygments"],
+    install_requires=["PyYAML", "openai", "streamlit", "Pygments", "Markdown"],
     packages=setuptools.find_packages(),
     python_requires=">=3.6",
     entry_points={
         "console_scripts": [
             "dh = dh.cli:parse",
         ]
     }
```


# Comparing `tmp/fmo-cli-1.0.0.tar.gz` & `tmp/fmo-cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmo-cli-1.0.0.tar", last modified: Fri May 12 20:31:25 2023, max compression
+gzip compressed data, was "fmo-cli-1.0.1.tar", last modified: Fri May 12 20:38:16 2023, max compression
```

## Comparing `fmo-cli-1.0.0.tar` & `fmo-cli-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 gudjon     (501) staff       (20)        0 2023-05-12 20:31:25.782490 fmo-cli-1.0.0/
--rw-r--r--   0 gudjon     (501) staff       (20)     1872 2023-05-12 20:31:25.782324 fmo-cli-1.0.0/PKG-INFO
--rw-r--r--   0 gudjon     (501) staff       (20)     1589 2023-05-12 20:15:49.000000 fmo-cli-1.0.0/README.md
-drwxr-xr-x   0 gudjon     (501) staff       (20)        0 2023-05-12 20:31:25.780740 fmo-cli-1.0.0/fmo/
--rw-r--r--   0 gudjon     (501) staff       (20)        0 2023-05-12 19:03:23.000000 fmo-cli-1.0.0/fmo/__init__.py
--rw-r--r--   0 gudjon     (501) staff       (20)     2633 2023-05-12 19:38:22.000000 fmo-cli-1.0.0/fmo/cli.py
--rw-r--r--   0 gudjon     (501) staff       (20)     1732 2023-05-12 19:05:55.000000 fmo-cli-1.0.0/fmo/fmo.py
-drwxr-xr-x   0 gudjon     (501) staff       (20)        0 2023-05-12 20:31:25.782141 fmo-cli-1.0.0/fmo_cli.egg-info/
--rw-r--r--   0 gudjon     (501) staff       (20)     1872 2023-05-12 20:31:25.000000 fmo-cli-1.0.0/fmo_cli.egg-info/PKG-INFO
--rw-r--r--   0 gudjon     (501) staff       (20)      244 2023-05-12 20:31:25.000000 fmo-cli-1.0.0/fmo_cli.egg-info/SOURCES.txt
--rw-r--r--   0 gudjon     (501) staff       (20)        1 2023-05-12 20:31:25.000000 fmo-cli-1.0.0/fmo_cli.egg-info/dependency_links.txt
--rw-r--r--   0 gudjon     (501) staff       (20)       36 2023-05-12 20:31:25.000000 fmo-cli-1.0.0/fmo_cli.egg-info/entry_points.txt
--rw-r--r--   0 gudjon     (501) staff       (20)       65 2023-05-12 20:31:25.000000 fmo-cli-1.0.0/fmo_cli.egg-info/requires.txt
--rw-r--r--   0 gudjon     (501) staff       (20)        4 2023-05-12 20:31:25.000000 fmo-cli-1.0.0/fmo_cli.egg-info/top_level.txt
--rw-r--r--   0 gudjon     (501) staff       (20)       38 2023-05-12 20:31:25.782533 fmo-cli-1.0.0/setup.cfg
--rw-r--r--   0 gudjon     (501) staff       (20)      824 2023-05-12 20:22:46.000000 fmo-cli-1.0.0/setup.py
+drwxr-xr-x   0 gudjon     (501) staff       (20)        0 2023-05-12 20:38:16.340014 fmo-cli-1.0.1/
+-rw-r--r--   0 gudjon     (501) staff       (20)     1872 2023-05-12 20:38:16.339859 fmo-cli-1.0.1/PKG-INFO
+-rw-r--r--   0 gudjon     (501) staff       (20)     1589 2023-05-12 20:35:59.000000 fmo-cli-1.0.1/README.md
+drwxr-xr-x   0 gudjon     (501) staff       (20)        0 2023-05-12 20:38:16.338426 fmo-cli-1.0.1/fmo/
+-rw-r--r--   0 gudjon     (501) staff       (20)        0 2023-05-12 19:03:23.000000 fmo-cli-1.0.1/fmo/__init__.py
+-rw-r--r--   0 gudjon     (501) staff       (20)     2633 2023-05-12 19:38:22.000000 fmo-cli-1.0.1/fmo/cli.py
+-rw-r--r--   0 gudjon     (501) staff       (20)     1732 2023-05-12 19:05:55.000000 fmo-cli-1.0.1/fmo/fmo.py
+drwxr-xr-x   0 gudjon     (501) staff       (20)        0 2023-05-12 20:38:16.339664 fmo-cli-1.0.1/fmo_cli.egg-info/
+-rw-r--r--   0 gudjon     (501) staff       (20)     1872 2023-05-12 20:38:16.000000 fmo-cli-1.0.1/fmo_cli.egg-info/PKG-INFO
+-rw-r--r--   0 gudjon     (501) staff       (20)      244 2023-05-12 20:38:16.000000 fmo-cli-1.0.1/fmo_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 gudjon     (501) staff       (20)        1 2023-05-12 20:38:16.000000 fmo-cli-1.0.1/fmo_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 gudjon     (501) staff       (20)       36 2023-05-12 20:38:16.000000 fmo-cli-1.0.1/fmo_cli.egg-info/entry_points.txt
+-rw-r--r--   0 gudjon     (501) staff       (20)       65 2023-05-12 20:38:16.000000 fmo-cli-1.0.1/fmo_cli.egg-info/requires.txt
+-rw-r--r--   0 gudjon     (501) staff       (20)        4 2023-05-12 20:38:16.000000 fmo-cli-1.0.1/fmo_cli.egg-info/top_level.txt
+-rw-r--r--   0 gudjon     (501) staff       (20)       38 2023-05-12 20:38:16.340056 fmo-cli-1.0.1/setup.cfg
+-rw-r--r--   0 gudjon     (501) staff       (20)      824 2023-05-12 20:36:19.000000 fmo-cli-1.0.1/setup.py
```

### Comparing `fmo-cli-1.0.0/PKG-INFO` & `fmo-cli-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: fmo-cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: Command Line Interface to access and upload FindMyOyster data
 Author: Gudjon Magnusson
 Author-email: gmagnusson@fraunhofer.org
 Keywords: FindMyOyster,CLI
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 
 # FindMyOyster Command Line Interface
 
 This CLI tool allows you to interact with the [FindMyOyster](https://findmyoyster.com) backend to upload or access data. You can also use it as a library in your own scripts.
 
 ## Installation
 
 ```
-pip install fmo_cli
+pip install fmo-cli
 ```
 
 ## Authenticate 
 
 Before making any requests to the API you must authenticate. Requests are authenticated using a token.
 
 To get a token to must use the `authenticate` command.
```

### Comparing `fmo-cli-1.0.0/README.md` & `fmo-cli-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # FindMyOyster Command Line Interface
 
 This CLI tool allows you to interact with the [FindMyOyster](https://findmyoyster.com) backend to upload or access data. You can also use it as a library in your own scripts.
 
 ## Installation
 
 ```
-pip install fmo_cli
+pip install fmo-cli
 ```
 
 ## Authenticate 
 
 Before making any requests to the API you must authenticate. Requests are authenticated using a token.
 
 To get a token to must use the `authenticate` command.
```

### Comparing `fmo-cli-1.0.0/fmo/cli.py` & `fmo-cli-1.0.1/fmo/cli.py`

 * *Files identical despite different names*

### Comparing `fmo-cli-1.0.0/fmo/fmo.py` & `fmo-cli-1.0.1/fmo/fmo.py`

 * *Files identical despite different names*

### Comparing `fmo-cli-1.0.0/fmo_cli.egg-info/PKG-INFO` & `fmo-cli-1.0.1/fmo_cli.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: fmo-cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: Command Line Interface to access and upload FindMyOyster data
 Author: Gudjon Magnusson
 Author-email: gmagnusson@fraunhofer.org
 Keywords: FindMyOyster,CLI
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 
 # FindMyOyster Command Line Interface
 
 This CLI tool allows you to interact with the [FindMyOyster](https://findmyoyster.com) backend to upload or access data. You can also use it as a library in your own scripts.
 
 ## Installation
 
 ```
-pip install fmo_cli
+pip install fmo-cli
 ```
 
 ## Authenticate 
 
 Before making any requests to the API you must authenticate. Requests are authenticated using a token.
 
 To get a token to must use the `authenticate` command.
```

### Comparing `fmo-cli-1.0.0/setup.py` & `fmo-cli-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name="fmo-cli",
-    version="1.0.0",
+    version="1.0.1",
     author="Gudjon Magnusson",
     author_email="gmagnusson@fraunhofer.org",
     description="Command Line Interface to access and upload FindMyOyster data",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=["fmo"],
     keywords=["FindMyOyster", "CLI"],
```


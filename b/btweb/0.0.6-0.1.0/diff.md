# Comparing `tmp/btweb-0.0.6.tar.gz` & `tmp/btweb-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btweb-0.0.6.tar", last modified: Thu May 11 11:46:35 2023, max compression
+gzip compressed data, was "btweb-0.1.0.tar", last modified: Fri May 12 20:38:28 2023, max compression
```

## Comparing `btweb-0.0.6.tar` & `btweb-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 11:46:35.926124 btweb-0.0.6/
--rw-r--r--   0 etejeda    (501) staff       (20)     1347 2023-05-11 11:43:48.000000 btweb-0.0.6/.gitignore
--rw-r--r--   0 etejeda    (501) staff       (20)      175 2023-05-11 11:43:48.000000 btweb-0.0.6/AUTHORS.rst
--rw-r--r--   0 etejeda    (501) staff       (20)     1097 2023-05-11 11:43:48.000000 btweb-0.0.6/LICENSE
--rw-r--r--   0 etejeda    (501) staff       (20)      224 2023-05-11 11:43:48.000000 btweb-0.0.6/MANIFEST.in
--rw-r--r--   0 etejeda    (501) staff       (20)     2945 2023-05-11 11:46:35.926355 btweb-0.0.6/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)     1991 2023-05-11 11:43:48.000000 btweb-0.0.6/README.md
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 11:46:35.924046 btweb-0.0.6/btweb/
--rw-r--r--   0 etejeda    (501) staff       (20)     3610 2023-05-11 11:43:48.000000 btweb-0.0.6/btweb/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)      689 2023-05-11 11:43:48.000000 btweb-0.0.6/btweb/logger.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 11:46:35.925770 btweb-0.0.6/btweb.egg-info/
--rw-r--r--   0 etejeda    (501) staff       (20)     2945 2023-05-11 11:46:35.000000 btweb-0.0.6/btweb.egg-info/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)      302 2023-05-11 11:46:35.000000 btweb-0.0.6/btweb.egg-info/SOURCES.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-11 11:46:35.000000 btweb-0.0.6/btweb.egg-info/dependency_links.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-11 11:46:35.000000 btweb-0.0.6/btweb.egg-info/not-zip-safe
--rw-r--r--   0 etejeda    (501) staff       (20)       58 2023-05-11 11:46:35.000000 btweb-0.0.6/btweb.egg-info/requires.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        6 2023-05-11 11:46:35.000000 btweb-0.0.6/btweb.egg-info/top_level.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-11 11:43:48.000000 btweb-0.0.6/requirements.txt
--rw-r--r--   0 etejeda    (501) staff       (20)     1182 2023-05-11 11:46:35.927087 btweb-0.0.6/setup.cfg
--rw-r--r--   0 etejeda    (501) staff       (20)       36 2023-05-11 11:43:48.000000 btweb-0.0.6/setup.py
--rw-r--r--   0 etejeda    (501) staff       (20)      315 2023-05-11 11:43:48.000000 btweb-0.0.6/tox.ini
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:38:28.175279 btweb-0.1.0/
+-rw-r--r--   0 etejeda    (501) staff       (20)     1347 2023-05-11 11:43:48.000000 btweb-0.1.0/.gitignore
+-rw-r--r--   0 etejeda    (501) staff       (20)      175 2023-05-11 11:43:48.000000 btweb-0.1.0/AUTHORS.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)     1097 2023-05-11 11:43:48.000000 btweb-0.1.0/LICENSE
+-rw-r--r--   0 etejeda    (501) staff       (20)      224 2023-05-11 11:43:48.000000 btweb-0.1.0/MANIFEST.in
+-rw-r--r--   0 etejeda    (501) staff       (20)     2909 2023-05-12 20:38:28.175670 btweb-0.1.0/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)     1955 2023-05-11 11:58:32.000000 btweb-0.1.0/README.md
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:38:28.173113 btweb-0.1.0/btweb/
+-rw-r--r--   0 etejeda    (501) staff       (20)     3598 2023-05-12 20:19:16.000000 btweb-0.1.0/btweb/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      689 2023-05-11 11:43:48.000000 btweb-0.1.0/btweb/logger.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:38:28.174834 btweb-0.1.0/btweb.egg-info/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2909 2023-05-12 20:38:28.000000 btweb-0.1.0/btweb.egg-info/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)      302 2023-05-12 20:38:28.000000 btweb-0.1.0/btweb.egg-info/SOURCES.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-12 20:38:28.000000 btweb-0.1.0/btweb.egg-info/dependency_links.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-12 20:38:15.000000 btweb-0.1.0/btweb.egg-info/not-zip-safe
+-rw-r--r--   0 etejeda    (501) staff       (20)       58 2023-05-12 20:38:28.000000 btweb-0.1.0/btweb.egg-info/requires.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        6 2023-05-12 20:38:28.000000 btweb-0.1.0/btweb.egg-info/top_level.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-11 11:43:48.000000 btweb-0.1.0/requirements.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)     1182 2023-05-12 20:38:28.176636 btweb-0.1.0/setup.cfg
+-rw-r--r--   0 etejeda    (501) staff       (20)       36 2023-05-11 11:43:48.000000 btweb-0.1.0/setup.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      315 2023-05-11 11:43:48.000000 btweb-0.1.0/tox.ini
```

### Comparing `btweb-0.0.6/.gitignore` & `btweb-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `btweb-0.0.6/LICENSE` & `btweb-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `btweb-0.0.6/PKG-INFO` & `btweb-0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btweb
-Version: 0.0.6
+Version: 0.1.0
 Summary: Utilit library for fronting requests functionality
 Home-page: https://github.com/berttejeda/bert.webadapter.git
 Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com
 Keywords: requests,https,get,python,remote,file,download
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -37,39 +37,39 @@
 
 # Prerequisites:
 
 - Python 2.7+
 
 # Installation
 
-* From pypi: `pip3 install bertdotwebadapter`
+* From pypi: `pip3 install btweb`
 * From this git repo: `pip3 install git+https://github.com/berttejeda/bert.webadapter.git`<br />
   Note: To install a specific version of the library from this git repo, <br />
   suffix the git URL in the above command with @{ tag name }, e.g.: <br />
   git+https://github.com/berttejeda/bert.webadapter.git@0.0.1
 
 # Usage Examples
 
 ## Download a file from a URL using Basic HTTP Authentication
 
 ```python
 
-from bertdotwebadapter import WebAdapter
+from btweb import WebAdapter
 
 webadapter = WebAdapter()
 res = webadapter.get(url, 
   username=username,
   password=password)
 ```
 
 ## Download a file from a URL using Basic HTTP Authentication, caching the result for 30 minutes
 
 ```python
 
-from bertdotwebadapter import WebAdapter
+from btweb import WebAdapter
 
 webadapter = WebAdapter()
 res = webadapter.get(url, 
   username=username,
   password=password,        
   cache=True,
   cache_path='.',
```

### Comparing `btweb-0.0.6/README.md` & `btweb-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,39 +13,39 @@
 
 # Prerequisites:
 
 - Python 2.7+
 
 # Installation
 
-* From pypi: `pip3 install bertdotwebadapter`
+* From pypi: `pip3 install btweb`
 * From this git repo: `pip3 install git+https://github.com/berttejeda/bert.webadapter.git`<br />
   Note: To install a specific version of the library from this git repo, <br />
   suffix the git URL in the above command with @{ tag name }, e.g.: <br />
   git+https://github.com/berttejeda/bert.webadapter.git@0.0.1
 
 # Usage Examples
 
 ## Download a file from a URL using Basic HTTP Authentication
 
 ```python
 
-from bertdotwebadapter import WebAdapter
+from btweb import WebAdapter
 
 webadapter = WebAdapter()
 res = webadapter.get(url, 
   username=username,
   password=password)
 ```
 
 ## Download a file from a URL using Basic HTTP Authentication, caching the result for 30 minutes
 
 ```python
 
-from bertdotwebadapter import WebAdapter
+from btweb import WebAdapter
 
 webadapter = WebAdapter()
 res = webadapter.get(url, 
   username=username,
   password=password,        
   cache=True,
   cache_path='.',
```

### Comparing `btweb-0.0.6/btweb/__init__.py` & `btweb-0.1.0/btweb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import datetime
-from bertdotwebadapter.logger import Logger
+from btweb.logger import Logger
 import os
 import re
 import requests
 from requests.auth import HTTPBasicAuth
 import sys
 
 logger = Logger().init_logger(__name__)
```

### Comparing `btweb-0.0.6/btweb/logger.py` & `btweb-0.1.0/btweb/logger.py`

 * *Files identical despite different names*

### Comparing `btweb-0.0.6/btweb.egg-info/PKG-INFO` & `btweb-0.1.0/btweb.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btweb
-Version: 0.0.6
+Version: 0.1.0
 Summary: Utilit library for fronting requests functionality
 Home-page: https://github.com/berttejeda/bert.webadapter.git
 Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com
 Keywords: requests,https,get,python,remote,file,download
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -37,39 +37,39 @@
 
 # Prerequisites:
 
 - Python 2.7+
 
 # Installation
 
-* From pypi: `pip3 install bertdotwebadapter`
+* From pypi: `pip3 install btweb`
 * From this git repo: `pip3 install git+https://github.com/berttejeda/bert.webadapter.git`<br />
   Note: To install a specific version of the library from this git repo, <br />
   suffix the git URL in the above command with @{ tag name }, e.g.: <br />
   git+https://github.com/berttejeda/bert.webadapter.git@0.0.1
 
 # Usage Examples
 
 ## Download a file from a URL using Basic HTTP Authentication
 
 ```python
 
-from bertdotwebadapter import WebAdapter
+from btweb import WebAdapter
 
 webadapter = WebAdapter()
 res = webadapter.get(url, 
   username=username,
   password=password)
 ```
 
 ## Download a file from a URL using Basic HTTP Authentication, caching the result for 30 minutes
 
 ```python
 
-from bertdotwebadapter import WebAdapter
+from btweb import WebAdapter
 
 webadapter = WebAdapter()
 res = webadapter.get(url, 
   username=username,
   password=password,        
   cache=True,
   cache_path='.',
```

### Comparing `btweb-0.0.6/setup.cfg` & `btweb-0.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = btweb
 author = Engelbert Tejeda
 author_email = berttejeda@gmail.com
 description = Utilit library for fronting requests functionality
-version = 0.0.6
+version = 0.1.0
 url = https://github.com/berttejeda/bert.webadapter.git
 keywords = 
 	requests
 	https
 	get
 	python
 	remote
```


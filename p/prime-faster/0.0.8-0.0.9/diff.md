# Comparing `tmp/prime-faster-0.0.8.tar.gz` & `tmp/prime-faster-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prime-faster-0.0.8.tar", last modified: Fri May 12 13:05:00 2023, max compression
+gzip compressed data, was "prime-faster-0.0.9.tar", last modified: Fri May 12 13:16:34 2023, max compression
```

## Comparing `prime-faster-0.0.8.tar` & `prime-faster-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 akarichang   (501) staff       (20)        0 2023-05-12 13:05:00.893423 prime-faster-0.0.8/
--rw-r--r--   0 akarichang   (501) staff       (20)     1101 2023-05-12 13:01:29.000000 prime-faster-0.0.8/LICENSE
--rw-r--r--   0 akarichang   (501) staff       (20)      884 2023-05-12 13:05:00.893300 prime-faster-0.0.8/PKG-INFO
--rw-r--r--   0 akarichang   (501) staff       (20)      417 2023-05-12 12:22:18.000000 prime-faster-0.0.8/README.md
-drwxr-xr-x   0 akarichang   (501) staff       (20)        0 2023-05-12 13:05:00.892912 prime-faster-0.0.8/prime_faster.egg-info/
--rw-r--r--   0 akarichang   (501) staff       (20)      884 2023-05-12 13:05:00.000000 prime-faster-0.0.8/prime_faster.egg-info/PKG-INFO
--rw-r--r--   0 akarichang   (501) staff       (20)      221 2023-05-12 13:05:00.000000 prime-faster-0.0.8/prime_faster.egg-info/SOURCES.txt
--rw-r--r--   0 akarichang   (501) staff       (20)        1 2023-05-12 13:05:00.000000 prime-faster-0.0.8/prime_faster.egg-info/dependency_links.txt
--rw-r--r--   0 akarichang   (501) staff       (20)       12 2023-05-12 13:05:00.000000 prime-faster-0.0.8/prime_faster.egg-info/top_level.txt
-drwxr-xr-x   0 akarichang   (501) staff       (20)        0 2023-05-12 13:05:00.893139 prime-faster-0.0.8/primefaster/
--rw-r--r--   0 akarichang   (501) staff       (20)       37 2023-05-12 12:22:18.000000 prime-faster-0.0.8/primefaster/__init__.py
--rw-r--r--   0 akarichang   (501) staff       (20)     1079 2023-05-12 12:59:21.000000 prime-faster-0.0.8/primefaster/primefaster.py
--rw-r--r--   0 akarichang   (501) staff       (20)       38 2023-05-12 13:05:00.893465 prime-faster-0.0.8/setup.cfg
--rw-r--r--   0 akarichang   (501) staff       (20)      990 2023-05-12 13:01:48.000000 prime-faster-0.0.8/setup.py
+drwxr-xr-x   0 akarichang   (501) staff       (20)        0 2023-05-12 13:16:34.701260 prime-faster-0.0.9/
+-rw-r--r--   0 akarichang   (501) staff       (20)     1101 2023-05-12 13:01:29.000000 prime-faster-0.0.9/LICENSE
+-rw-r--r--   0 akarichang   (501) staff       (20)      884 2023-05-12 13:16:34.701126 prime-faster-0.0.9/PKG-INFO
+-rw-r--r--   0 akarichang   (501) staff       (20)      417 2023-05-12 12:22:18.000000 prime-faster-0.0.9/README.md
+drwxr-xr-x   0 akarichang   (501) staff       (20)        0 2023-05-12 13:16:34.700710 prime-faster-0.0.9/prime_faster.egg-info/
+-rw-r--r--   0 akarichang   (501) staff       (20)      884 2023-05-12 13:16:34.000000 prime-faster-0.0.9/prime_faster.egg-info/PKG-INFO
+-rw-r--r--   0 akarichang   (501) staff       (20)      221 2023-05-12 13:16:34.000000 prime-faster-0.0.9/prime_faster.egg-info/SOURCES.txt
+-rw-r--r--   0 akarichang   (501) staff       (20)        1 2023-05-12 13:16:34.000000 prime-faster-0.0.9/prime_faster.egg-info/dependency_links.txt
+-rw-r--r--   0 akarichang   (501) staff       (20)       12 2023-05-12 13:16:34.000000 prime-faster-0.0.9/prime_faster.egg-info/top_level.txt
+drwxr-xr-x   0 akarichang   (501) staff       (20)        0 2023-05-12 13:16:34.700953 prime-faster-0.0.9/primefaster/
+-rw-r--r--   0 akarichang   (501) staff       (20)       37 2023-05-12 12:22:18.000000 prime-faster-0.0.9/primefaster/__init__.py
+-rw-r--r--   0 akarichang   (501) staff       (20)     1090 2023-05-12 13:15:09.000000 prime-faster-0.0.9/primefaster/primefaster.py
+-rw-r--r--   0 akarichang   (501) staff       (20)       38 2023-05-12 13:16:34.701299 prime-faster-0.0.9/setup.cfg
+-rw-r--r--   0 akarichang   (501) staff       (20)      990 2023-05-12 13:15:09.000000 prime-faster-0.0.9/setup.py
```

### Comparing `prime-faster-0.0.8/LICENSE` & `prime-faster-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `prime-faster-0.0.8/PKG-INFO` & `prime-faster-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prime-faster
-Version: 0.0.8
+Version: 0.0.9
 Summary: prime-faster - Faster Prime Number Generator
 Home-page: https://github.com/takahashi-akari/prime-faster
 Author: Takahashi Akari
 Author-email: akaritakahashioss@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prime-faster-0.0.8/prime_faster.egg-info/PKG-INFO` & `prime-faster-0.0.9/prime_faster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prime-faster
-Version: 0.0.8
+Version: 0.0.9
 Summary: prime-faster - Faster Prime Number Generator
 Home-page: https://github.com/takahashi-akari/prime-faster
 Author: Takahashi Akari
 Author-email: akaritakahashioss@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prime-faster-0.0.8/primefaster/primefaster.py` & `prime-faster-0.0.9/primefaster/primefaster.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # prime-faster - Faster Prime Number Generator
 # Author: Takahashi Akari <akaritakahashioss@gmail.com>
 # License: MIT License Copyright (c) 2022 Takahashi Akari <akaritakahashioss@gmail.com>
-# Version: 0.0.8
+# Version: 0.0.9
 # Date: 2022-08-08
 # Python: 3.10.6
 # Description: prime-faster - Faster Prime Number Generator
 
-import sqrt
+from numpy import sqrt
 import numpy
 
 def is_prime(n):
     if n < 2:
         return False
     if n == 2:
         return True
```

### Comparing `prime-faster-0.0.8/setup.py` & `prime-faster-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # prime-faster - Faster Prime Number Generator
 # Author: Takahashi Akari <akaritakahashioss@gmail.com>
 # License: MIT License Copyright (c) 2022 Takahashi Akari <akaritakahashioss@gmail.com>
-# Version: 0.0.8
+# Version: 0.0.9
 # Date: 2022-08-08
 # Python: 3.10.6
 # Description: prime-faster - Faster Prime Number Generator
 
 import setuptools
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="prime-faster",
-    version="0.0.8",
+    version="0.0.9",
     author="Takahashi Akari",
     author_email="akaritakahashioss@gmail.com",
     description="prime-faster - Faster Prime Number Generator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/takahashi-akari/prime-faster",
     packages=setuptools.find_packages(),
```


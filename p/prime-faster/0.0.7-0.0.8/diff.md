# Comparing `tmp/prime-faster-0.0.7.tar.gz` & `tmp/prime-faster-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prime-faster-0.0.7.tar", last modified: Sun Aug  7 22:14:45 2022, max compression
+gzip compressed data, was "prime-faster-0.0.8.tar", last modified: Fri May 12 13:05:00 2023, max compression
```

## Comparing `prime-faster-0.0.7.tar` & `prime-faster-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 takahashiakari  (1000) takahashiakari  (1000)        0 2022-08-07 22:14:45.670610 prime-faster-0.0.7/
--rw-rw-r--   0 takahashiakari  (1000) takahashiakari  (1000)     1101 2022-08-07 18:57:03.000000 prime-faster-0.0.7/LICENSE
--rw-rw-r--   0 takahashiakari  (1000) takahashiakari  (1000)      884 2022-08-07 22:14:45.670610 prime-faster-0.0.7/PKG-INFO
--rw-rw-r--   0 takahashiakari  (1000) takahashiakari  (1000)      417 2022-08-07 22:13:49.000000 prime-faster-0.0.7/README.md
-drwxrwxr-x   0 takahashiakari  (1000) takahashiakari  (1000)        0 2022-08-07 22:14:45.670610 prime-faster-0.0.7/prime_faster.egg-info/
--rw-rw-r--   0 takahashiakari  (1000) takahashiakari  (1000)      884 2022-08-07 22:14:45.000000 prime-faster-0.0.7/prime_faster.egg-info/PKG-INFO
--rw-rw-r--   0 takahashiakari  (1000) takahashiakari  (1000)      221 2022-08-07 22:14:45.000000 prime-faster-0.0.7/prime_faster.egg-info/SOURCES.txt
--rw-rw-r--   0 takahashiakari  (1000) takahashiakari  (1000)        1 2022-08-07 22:14:45.000000 prime-faster-0.0.7/prime_faster.egg-info/dependency_links.txt
--rw-rw-r--   0 takahashiakari  (1000) takahashiakari  (1000)       12 2022-08-07 22:14:45.000000 prime-faster-0.0.7/prime_faster.egg-info/top_level.txt
-drwxrwxr-x   0 takahashiakari  (1000) takahashiakari  (1000)        0 2022-08-07 22:14:45.670610 prime-faster-0.0.7/primefaster/
--rw-rw-r--   0 takahashiakari  (1000) takahashiakari  (1000)       37 2022-08-07 21:29:03.000000 prime-faster-0.0.7/primefaster/__init__.py
--rw-rw-r--   0 takahashiakari  (1000) takahashiakari  (1000)     1081 2022-08-07 22:14:18.000000 prime-faster-0.0.7/primefaster/primefaster.py
--rw-rw-r--   0 takahashiakari  (1000) takahashiakari  (1000)       38 2022-08-07 22:14:45.670610 prime-faster-0.0.7/setup.cfg
--rw-rw-r--   0 takahashiakari  (1000) takahashiakari  (1000)      990 2022-08-07 22:14:18.000000 prime-faster-0.0.7/setup.py
+drwxr-xr-x   0 akarichang   (501) staff       (20)        0 2023-05-12 13:05:00.893423 prime-faster-0.0.8/
+-rw-r--r--   0 akarichang   (501) staff       (20)     1101 2023-05-12 13:01:29.000000 prime-faster-0.0.8/LICENSE
+-rw-r--r--   0 akarichang   (501) staff       (20)      884 2023-05-12 13:05:00.893300 prime-faster-0.0.8/PKG-INFO
+-rw-r--r--   0 akarichang   (501) staff       (20)      417 2023-05-12 12:22:18.000000 prime-faster-0.0.8/README.md
+drwxr-xr-x   0 akarichang   (501) staff       (20)        0 2023-05-12 13:05:00.892912 prime-faster-0.0.8/prime_faster.egg-info/
+-rw-r--r--   0 akarichang   (501) staff       (20)      884 2023-05-12 13:05:00.000000 prime-faster-0.0.8/prime_faster.egg-info/PKG-INFO
+-rw-r--r--   0 akarichang   (501) staff       (20)      221 2023-05-12 13:05:00.000000 prime-faster-0.0.8/prime_faster.egg-info/SOURCES.txt
+-rw-r--r--   0 akarichang   (501) staff       (20)        1 2023-05-12 13:05:00.000000 prime-faster-0.0.8/prime_faster.egg-info/dependency_links.txt
+-rw-r--r--   0 akarichang   (501) staff       (20)       12 2023-05-12 13:05:00.000000 prime-faster-0.0.8/prime_faster.egg-info/top_level.txt
+drwxr-xr-x   0 akarichang   (501) staff       (20)        0 2023-05-12 13:05:00.893139 prime-faster-0.0.8/primefaster/
+-rw-r--r--   0 akarichang   (501) staff       (20)       37 2023-05-12 12:22:18.000000 prime-faster-0.0.8/primefaster/__init__.py
+-rw-r--r--   0 akarichang   (501) staff       (20)     1079 2023-05-12 12:59:21.000000 prime-faster-0.0.8/primefaster/primefaster.py
+-rw-r--r--   0 akarichang   (501) staff       (20)       38 2023-05-12 13:05:00.893465 prime-faster-0.0.8/setup.cfg
+-rw-r--r--   0 akarichang   (501) staff       (20)      990 2023-05-12 13:01:48.000000 prime-faster-0.0.8/setup.py
```

### Comparing `prime-faster-0.0.7/LICENSE` & `prime-faster-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `prime-faster-0.0.7/PKG-INFO` & `prime-faster-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prime-faster
-Version: 0.0.7
+Version: 0.0.8
 Summary: prime-faster - Faster Prime Number Generator
 Home-page: https://github.com/takahashi-akari/prime-faster
 Author: Takahashi Akari
 Author-email: akaritakahashioss@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prime-faster-0.0.7/prime_faster.egg-info/PKG-INFO` & `prime-faster-0.0.8/prime_faster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prime-faster
-Version: 0.0.7
+Version: 0.0.8
 Summary: prime-faster - Faster Prime Number Generator
 Home-page: https://github.com/takahashi-akari/prime-faster
 Author: Takahashi Akari
 Author-email: akaritakahashioss@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prime-faster-0.0.7/primefaster/primefaster.py` & `prime-faster-0.0.8/primefaster/primefaster.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # prime-faster - Faster Prime Number Generator
 # Author: Takahashi Akari <akaritakahashioss@gmail.com>
 # License: MIT License Copyright (c) 2022 Takahashi Akari <akaritakahashioss@gmail.com>
-# Version: 0.0.7
+# Version: 0.0.8
 # Date: 2022-08-08
 # Python: 3.10.6
 # Description: prime-faster - Faster Prime Number Generator
 
-import math
+import sqrt
 import numpy
 
 def is_prime(n):
     if n < 2:
         return False
     if n == 2:
         return True
     if n % 2 == 0:
         return False
-    for i in range(3, int(n ** 0.5) + 1, 2):
+    for i in range(3, int(sqrt(n)) + 1, 2):
         if n % i == 0:
             return False
     return True
 
 def get_prime(n):
     if n < 2:
         return []
     if n == 2:
         return [2]
     if n == 3:
         return [2, 3]
     n += 1
     sieve = numpy.ones(n // 3 + (n % 6 == 2), dtype=bool)
-    for i in range(1, int(n ** 0.5) // 3 + 1):
+    for i in range(1, int(sqrt(n)) // 3 + 1):
         if sieve[i]:
             k = 3 * i + 1 | 1
             sieve[k * k // 3 :: 2 * k] = False
             sieve[k * ( k - 2 * (i & 1 ) + 4) // 3 :: 2 * k] = False
     np = numpy.r_[2, 3, ((3 * numpy.nonzero(sieve)[0][1:] + 1)|1)]
     # return array
     return np.tolist()
```

### Comparing `prime-faster-0.0.7/setup.py` & `prime-faster-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # prime-faster - Faster Prime Number Generator
 # Author: Takahashi Akari <akaritakahashioss@gmail.com>
 # License: MIT License Copyright (c) 2022 Takahashi Akari <akaritakahashioss@gmail.com>
-# Version: 0.0.7
+# Version: 0.0.8
 # Date: 2022-08-08
 # Python: 3.10.6
 # Description: prime-faster - Faster Prime Number Generator
 
 import setuptools
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="prime-faster",
-    version="0.0.7",
+    version="0.0.8",
     author="Takahashi Akari",
     author_email="akaritakahashioss@gmail.com",
     description="prime-faster - Faster Prime Number Generator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/takahashi-akari/prime-faster",
     packages=setuptools.find_packages(),
```


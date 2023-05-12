# Comparing `tmp/fast-bf-1.0.1.tar.gz` & `tmp/fast-bf-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fast-bf-1.0.1.tar", last modified: Fri May 12 08:35:49 2023, max compression
+gzip compressed data, was "dist/fast-bf-1.1.0.tar", last modified: Fri May 12 10:29:01 2023, max compression
```

## Comparing `fast-bf-1.0.1.tar` & `fast-bf-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,14 @@
-drwxr-xr-x   0 guocheng   (501) staff       (20)        0 2023-05-12 08:35:49.000000 fast-bf-1.0.1/
--rw-r--r--   0 guocheng   (501) staff       (20)      718 2023-05-12 08:35:49.000000 fast-bf-1.0.1/PKG-INFO
--rw-r--r--   0 guocheng   (501) staff       (20)     1281 2023-05-12 08:01:52.000000 fast-bf-1.0.1/README.md
-drwxr-xr-x   0 guocheng   (501) staff       (20)        0 2023-05-12 08:35:49.000000 fast-bf-1.0.1/fast_bf.egg-info/
--rw-r--r--   0 guocheng   (501) staff       (20)      718 2023-05-12 08:35:49.000000 fast-bf-1.0.1/fast_bf.egg-info/PKG-INFO
--rw-r--r--   0 guocheng   (501) staff       (20)      142 2023-05-12 08:35:49.000000 fast-bf-1.0.1/fast_bf.egg-info/SOURCES.txt
--rw-r--r--   0 guocheng   (501) staff       (20)        1 2023-05-12 08:35:49.000000 fast-bf-1.0.1/fast_bf.egg-info/dependency_links.txt
--rw-r--r--   0 guocheng   (501) staff       (20)        1 2023-05-12 08:35:49.000000 fast-bf-1.0.1/fast_bf.egg-info/top_level.txt
--rw-r--r--   0 guocheng   (501) staff       (20)       38 2023-05-12 08:35:49.000000 fast-bf-1.0.1/setup.cfg
--rw-r--r--   0 guocheng   (501) staff       (20)      867 2023-05-12 08:35:34.000000 fast-bf-1.0.1/setup.py
+drwxr-xr-x   0 guocheng   (501) staff       (20)        0 2023-05-12 10:29:01.000000 fast-bf-1.1.0/
+-rw-r--r--   0 guocheng   (501) staff       (20)     1061 2023-05-12 07:55:52.000000 fast-bf-1.1.0/LICENSE
+-rw-r--r--   0 guocheng   (501) staff       (20)      684 2023-05-12 10:29:01.000000 fast-bf-1.1.0/PKG-INFO
+-rw-r--r--   0 guocheng   (501) staff       (20)     1281 2023-05-12 08:01:52.000000 fast-bf-1.1.0/README.md
+drwxr-xr-x   0 guocheng   (501) staff       (20)        0 2023-05-12 10:29:01.000000 fast-bf-1.1.0/bloom_filter/
+-rw-r--r--   0 guocheng   (501) staff       (20)        0 2023-05-12 10:27:16.000000 fast-bf-1.1.0/bloom_filter/__init__.py
+-rw-r--r--   0 guocheng   (501) staff       (20)     1210 2023-05-12 07:50:37.000000 fast-bf-1.1.0/bloom_filter/bloom_filter.py
+drwxr-xr-x   0 guocheng   (501) staff       (20)        0 2023-05-12 10:29:01.000000 fast-bf-1.1.0/fast_bf.egg-info/
+-rw-r--r--   0 guocheng   (501) staff       (20)      684 2023-05-12 10:29:01.000000 fast-bf-1.1.0/fast_bf.egg-info/PKG-INFO
+-rw-r--r--   0 guocheng   (501) staff       (20)      204 2023-05-12 10:29:01.000000 fast-bf-1.1.0/fast_bf.egg-info/SOURCES.txt
+-rw-r--r--   0 guocheng   (501) staff       (20)        1 2023-05-12 10:29:01.000000 fast-bf-1.1.0/fast_bf.egg-info/dependency_links.txt
+-rw-r--r--   0 guocheng   (501) staff       (20)       13 2023-05-12 10:29:01.000000 fast-bf-1.1.0/fast_bf.egg-info/top_level.txt
+-rw-r--r--   0 guocheng   (501) staff       (20)       38 2023-05-12 10:29:01.000000 fast-bf-1.1.0/setup.cfg
+-rw-r--r--   0 guocheng   (501) staff       (20)      867 2023-05-12 10:28:40.000000 fast-bf-1.1.0/setup.py
```

### Comparing `fast-bf-1.0.1/PKG-INFO` & `fast-bf-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: fast-bf
-Version: 1.0.1
+Version: 1.1.0
 Summary: A fast bloom filter implementation in Python
 Home-page: https://github.com/GuoCheng-maker/bloom_filter.git
 Author: Cheng.guo
 Author-email: guocheng6868@126.com
-License: UNKNOWN
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+License-File: LICENSE
```

### Comparing `fast-bf-1.0.1/README.md` & `fast-bf-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `fast-bf-1.0.1/fast_bf.egg-info/PKG-INFO` & `fast-bf-1.1.0/fast_bf.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: fast-bf
-Version: 1.0.1
+Version: 1.1.0
 Summary: A fast bloom filter implementation in Python
 Home-page: https://github.com/GuoCheng-maker/bloom_filter.git
 Author: Cheng.guo
 Author-email: guocheng6868@126.com
-License: UNKNOWN
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+License-File: LICENSE
```

### Comparing `fast-bf-1.0.1/setup.py` & `fast-bf-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fast-bf',
-    version='1.0.1',
+    version='1.1.0',
     url='https://github.com/GuoCheng-maker/bloom_filter.git',
     author='Cheng.guo',
     author_email='guocheng6868@126.com',
     description='A fast bloom filter implementation in Python',
     packages=find_packages(),
     install_requires=[
         # add any dependencies here
```


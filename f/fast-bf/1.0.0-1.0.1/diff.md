# Comparing `tmp/fast-bf-1.0.0.tar.gz` & `tmp/fast-bf-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fast-bf-1.0.0.tar", last modified: Fri May 12 08:25:54 2023, max compression
+gzip compressed data, was "dist/fast-bf-1.0.1.tar", last modified: Fri May 12 08:35:49 2023, max compression
```

## Comparing `fast-bf-1.0.0.tar` & `fast-bf-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 guocheng   (501) staff       (20)        0 2023-05-12 08:25:54.000000 fast-bf-1.0.0/
--rw-r--r--   0 guocheng   (501) staff       (20)      709 2023-05-12 08:25:54.000000 fast-bf-1.0.0/PKG-INFO
--rw-r--r--   0 guocheng   (501) staff       (20)     1281 2023-05-12 08:01:52.000000 fast-bf-1.0.0/README.md
-drwxr-xr-x   0 guocheng   (501) staff       (20)        0 2023-05-12 08:25:54.000000 fast-bf-1.0.0/fast_bf.egg-info/
--rw-r--r--   0 guocheng   (501) staff       (20)      709 2023-05-12 08:25:54.000000 fast-bf-1.0.0/fast_bf.egg-info/PKG-INFO
--rw-r--r--   0 guocheng   (501) staff       (20)      142 2023-05-12 08:25:54.000000 fast-bf-1.0.0/fast_bf.egg-info/SOURCES.txt
--rw-r--r--   0 guocheng   (501) staff       (20)        1 2023-05-12 08:25:54.000000 fast-bf-1.0.0/fast_bf.egg-info/dependency_links.txt
--rw-r--r--   0 guocheng   (501) staff       (20)        1 2023-05-12 08:25:54.000000 fast-bf-1.0.0/fast_bf.egg-info/top_level.txt
--rw-r--r--   0 guocheng   (501) staff       (20)       38 2023-05-12 08:25:54.000000 fast-bf-1.0.0/setup.cfg
--rw-r--r--   0 guocheng   (501) staff       (20)      858 2023-05-12 08:25:40.000000 fast-bf-1.0.0/setup.py
+drwxr-xr-x   0 guocheng   (501) staff       (20)        0 2023-05-12 08:35:49.000000 fast-bf-1.0.1/
+-rw-r--r--   0 guocheng   (501) staff       (20)      718 2023-05-12 08:35:49.000000 fast-bf-1.0.1/PKG-INFO
+-rw-r--r--   0 guocheng   (501) staff       (20)     1281 2023-05-12 08:01:52.000000 fast-bf-1.0.1/README.md
+drwxr-xr-x   0 guocheng   (501) staff       (20)        0 2023-05-12 08:35:49.000000 fast-bf-1.0.1/fast_bf.egg-info/
+-rw-r--r--   0 guocheng   (501) staff       (20)      718 2023-05-12 08:35:49.000000 fast-bf-1.0.1/fast_bf.egg-info/PKG-INFO
+-rw-r--r--   0 guocheng   (501) staff       (20)      142 2023-05-12 08:35:49.000000 fast-bf-1.0.1/fast_bf.egg-info/SOURCES.txt
+-rw-r--r--   0 guocheng   (501) staff       (20)        1 2023-05-12 08:35:49.000000 fast-bf-1.0.1/fast_bf.egg-info/dependency_links.txt
+-rw-r--r--   0 guocheng   (501) staff       (20)        1 2023-05-12 08:35:49.000000 fast-bf-1.0.1/fast_bf.egg-info/top_level.txt
+-rw-r--r--   0 guocheng   (501) staff       (20)       38 2023-05-12 08:35:49.000000 fast-bf-1.0.1/setup.cfg
+-rw-r--r--   0 guocheng   (501) staff       (20)      867 2023-05-12 08:35:34.000000 fast-bf-1.0.1/setup.py
```

### Comparing `fast-bf-1.0.0/PKG-INFO` & `fast-bf-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 1.1
 Name: fast-bf
-Version: 1.0.0
-Summary: A short description of your package
+Version: 1.0.1
+Summary: A fast bloom filter implementation in Python
 Home-page: https://github.com/GuoCheng-maker/bloom_filter.git
 Author: Cheng.guo
 Author-email: guocheng6868@126.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fast-bf-1.0.0/README.md` & `fast-bf-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fast-bf-1.0.0/fast_bf.egg-info/PKG-INFO` & `fast-bf-1.0.1/fast_bf.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 1.1
 Name: fast-bf
-Version: 1.0.0
-Summary: A short description of your package
+Version: 1.0.1
+Summary: A fast bloom filter implementation in Python
 Home-page: https://github.com/GuoCheng-maker/bloom_filter.git
 Author: Cheng.guo
 Author-email: guocheng6868@126.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fast-bf-1.0.0/setup.py` & `fast-bf-1.0.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fast-bf',
-    version='1.0.0',
+    version='1.0.1',
     url='https://github.com/GuoCheng-maker/bloom_filter.git',
     author='Cheng.guo',
     author_email='guocheng6868@126.com',
-    description='A short description of your package',
+    description='A fast bloom filter implementation in Python',
     packages=find_packages(),
     install_requires=[
         # add any dependencies here
         # 'numpy>=1.18.1',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
```


# Comparing `tmp/WordsToPdfs-0.3.0.tar.gz` & `tmp/WordsToPdfs-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WordsToPdfs-0.3.0.tar", last modified: Fri May  5 12:23:35 2023, max compression
+gzip compressed data, was "WordsToPdfs-0.3.1.tar", last modified: Fri May 12 07:06:57 2023, max compression
```

## Comparing `WordsToPdfs-0.3.0.tar` & `WordsToPdfs-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 12:23:35.568752 WordsToPdfs-0.3.0/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 WordsToPdfs-0.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 WordsToPdfs-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0      421 2023-05-05 12:23:35.568752 WordsToPdfs-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 WordsToPdfs-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 12:23:35.557722 WordsToPdfs-0.3.0/WordsToPdfs/
-drwxrwxrwx   0        0        0        0 2023-05-05 12:23:35.566788 WordsToPdfs-0.3.0/WordsToPdfs/Function/
--rw-rw-rw-   0        0        0        0 2023-02-28 03:33:27.000000 WordsToPdfs-0.3.0/WordsToPdfs/Function/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:23:35.567746 WordsToPdfs-0.3.0/WordsToPdfs/Ui/
--rw-rw-rw-   0        0        0        0 2023-02-28 03:33:27.000000 WordsToPdfs-0.3.0/WordsToPdfs/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 03:33:27.000000 WordsToPdfs-0.3.0/WordsToPdfs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:23:35.564714 WordsToPdfs-0.3.0/WordsToPdfs.egg-info/
--rw-rw-rw-   0        0        0      421 2023-05-05 12:23:35.000000 WordsToPdfs-0.3.0/WordsToPdfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-05-05 12:23:35.000000 WordsToPdfs-0.3.0/WordsToPdfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 12:23:35.000000 WordsToPdfs-0.3.0/WordsToPdfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-05 12:23:35.000000 WordsToPdfs-0.3.0/WordsToPdfs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      135 2023-05-05 12:23:35.569754 WordsToPdfs-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      968 2023-05-05 12:23:31.000000 WordsToPdfs-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:06:57.193051 WordsToPdfs-0.3.1/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 WordsToPdfs-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 WordsToPdfs-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      404 2023-05-12 07:06:57.193051 WordsToPdfs-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 WordsToPdfs-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 07:06:57.157062 WordsToPdfs-0.3.1/WordsToPdfs/
+drwxrwxrwx   0        0        0        0 2023-05-12 07:06:57.179015 WordsToPdfs-0.3.1/WordsToPdfs/Function/
+-rw-rw-rw-   0        0        0        0 2023-02-28 03:33:26.000000 WordsToPdfs-0.3.1/WordsToPdfs/Function/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:06:57.189053 WordsToPdfs-0.3.1/WordsToPdfs/Ui/
+-rw-rw-rw-   0        0        0    58880 2023-04-28 06:31:28.000000 WordsToPdfs-0.3.1/WordsToPdfs/Ui/WordToPdfUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-28 03:33:26.000000 WordsToPdfs-0.3.1/WordsToPdfs/Ui/__init__.py
+-rw-rw-rw-   0        0        0   171008 2023-05-12 07:01:37.000000 WordsToPdfs-0.3.1/WordsToPdfs/WordsToPdfs.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-28 03:33:26.000000 WordsToPdfs-0.3.1/WordsToPdfs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:06:57.175051 WordsToPdfs-0.3.1/WordsToPdfs.egg-info/
+-rw-rw-rw-   0        0        0      404 2023-05-12 07:06:57.000000 WordsToPdfs-0.3.1/WordsToPdfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-05-12 07:06:57.000000 WordsToPdfs-0.3.1/WordsToPdfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 07:06:57.000000 WordsToPdfs-0.3.1/WordsToPdfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-12 07:06:57.000000 WordsToPdfs-0.3.1/WordsToPdfs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2023-05-12 07:06:57.195016 WordsToPdfs-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      972 2023-05-12 06:56:17.000000 WordsToPdfs-0.3.1/setup.py
```

### Comparing `WordsToPdfs-0.3.0/LICENSE.txt` & `WordsToPdfs-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `WordsToPdfs-0.3.0/setup.py` & `WordsToPdfs-0.3.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 3
-PATCH = 0
+PATCH = 1
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "WordsToPdfs",
 	version = VERSION,
     author ="wangweidong",
     author_email = "17891967090@163.com",
-    description='PDF撕裂者单个功能',
+    description='word文件转化为pdf文件',
     long_description_content_type="text/markdown",
 	url = 'https://alidocs.dingtalk.com/i/p/4oJRz0VRJyvmLZMydy0mV7WvjQn7MG89',
 	long_description = open('README.md',encoding="utf-8").read(),
     python_requires=">=3.8",
     install_requires=get_install_requires(),
 
 	packages = find_packages(),
```


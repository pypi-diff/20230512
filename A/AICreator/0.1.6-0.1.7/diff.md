# Comparing `tmp/AICreator-0.1.6.tar.gz` & `tmp/AICreator-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AICreator-0.1.6.tar", last modified: Fri May 12 12:33:02 2023, max compression
+gzip compressed data, was "AICreator-0.1.7.tar", last modified: Fri May 12 12:52:35 2023, max compression
```

## Comparing `AICreator-0.1.6.tar` & `AICreator-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 12:33:02.834842 AICreator-0.1.6/
-drwxrwxrwx   0        0        0        0 2023-05-12 12:33:02.824323 AICreator-0.1.6/AICreator.egg-info/
--rw-rw-rw-   0        0        0      559 2023-05-12 12:33:02.000000 AICreator-0.1.6/AICreator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-05-12 12:33:02.000000 AICreator-0.1.6/AICreator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 12:33:02.000000 AICreator-0.1.6/AICreator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-12 12:33:02.000000 AICreator-0.1.6/AICreator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-12 12:33:02.000000 AICreator-0.1.6/AICreator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-12 12:33:02.826324 AICreator-0.1.6/AICreatorPackage/
--rw-rw-rw-   0        0        0      156 2023-05-02 13:30:46.000000 AICreator-0.1.6/AICreatorPackage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 12:33:02.830323 AICreator-0.1.6/AICreatorPackage/functions/
--rw-rw-rw-   0        0        0      907 2023-05-12 12:15:09.000000 AICreator-0.1.6/AICreatorPackage/functions/AICreatorPackage.py
--rw-rw-rw-   0        0        0        0 2022-04-25 10:59:44.000000 AICreator-0.1.6/AICreatorPackage/functions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 12:33:02.831325 AICreator-0.1.6/AICreatorPackage/functions/init/
--rw-rw-rw-   0        0        0    52493 2023-05-12 12:14:40.000000 AICreator-0.1.6/AICreatorPackage/functions/init/ini.py
--rw-rw-rw-   0        0        0     1078 2022-04-24 17:23:55.000000 AICreator-0.1.6/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2021-08-13 08:55:17.000000 AICreator-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0      559 2023-05-12 12:33:02.834842 AICreator-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       73 2023-05-02 12:11:18.000000 AICreator-0.1.6/README.txt
--rw-rw-rw-   0        0        0        0 2022-04-24 17:21:54.000000 AICreator-0.1.6/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-12 12:33:02.835840 AICreator-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      675 2023-05-12 12:32:58.000000 AICreator-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 12:52:35.604026 AICreator-0.1.7/
+drwxrwxrwx   0        0        0        0 2023-05-12 12:52:35.592668 AICreator-0.1.7/AICreator.egg-info/
+-rw-rw-rw-   0        0        0      559 2023-05-12 12:52:35.000000 AICreator-0.1.7/AICreator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-05-12 12:52:35.000000 AICreator-0.1.7/AICreator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 12:52:35.000000 AICreator-0.1.7/AICreator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-12 12:52:35.000000 AICreator-0.1.7/AICreator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-12 12:52:35.000000 AICreator-0.1.7/AICreator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 12:52:35.593845 AICreator-0.1.7/AICreatorPackage/
+-rw-rw-rw-   0        0        0      156 2023-05-02 13:30:46.000000 AICreator-0.1.7/AICreatorPackage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 12:52:35.598844 AICreator-0.1.7/AICreatorPackage/functions/
+-rw-rw-rw-   0        0        0      907 2023-05-12 12:15:09.000000 AICreator-0.1.7/AICreatorPackage/functions/AICreatorPackage.py
+-rw-rw-rw-   0        0        0        0 2022-04-25 10:59:44.000000 AICreator-0.1.7/AICreatorPackage/functions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 12:52:35.600844 AICreator-0.1.7/AICreatorPackage/functions/init/
+-rw-rw-rw-   0        0        0    52493 2023-05-12 12:14:40.000000 AICreator-0.1.7/AICreatorPackage/functions/init/ini.py
+-rw-rw-rw-   0        0        0     1078 2022-04-24 17:23:55.000000 AICreator-0.1.7/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2021-08-13 08:55:17.000000 AICreator-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      559 2023-05-12 12:52:35.602844 AICreator-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       73 2023-05-02 12:11:18.000000 AICreator-0.1.7/README.txt
+-rw-rw-rw-   0        0        0        0 2022-04-24 17:21:54.000000 AICreator-0.1.7/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-12 12:52:35.604026 AICreator-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      675 2023-05-12 12:51:34.000000 AICreator-0.1.7/setup.py
```

### Comparing `AICreator-0.1.6/AICreatorPackage/functions/AICreatorPackage.py` & `AICreator-0.1.7/AICreatorPackage/functions/AICreatorPackage.py`

 * *Files identical despite different names*

### Comparing `AICreator-0.1.6/AICreatorPackage/functions/init/ini.py` & `AICreator-0.1.7/AICreatorPackage/functions/init/ini.py`

 * *Files identical despite different names*

### Comparing `AICreator-0.1.6/LICENCE.txt` & `AICreator-0.1.7/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `AICreator-0.1.6/setup.py` & `AICreator-0.1.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='AICreator',
-    version='0.1.6',
+    version='0.1.7',
     description='AI Creator Package By - oren',
     long_description=open('README.txt').read(),
     url='',
     author='oren',
     author_email='orennadle@gmail.com',
     license='MIT',
     classifiers=classifiers,
```


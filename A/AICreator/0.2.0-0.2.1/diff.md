# Comparing `tmp/AICreator-0.2.0.tar.gz` & `tmp/AICreator-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AICreator-0.2.0.tar", last modified: Fri May 12 13:01:19 2023, max compression
+gzip compressed data, was "AICreator-0.2.1.tar", last modified: Fri May 12 13:02:20 2023, max compression
```

## Comparing `AICreator-0.2.0.tar` & `AICreator-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 13:01:19.895778 AICreator-0.2.0/
-drwxrwxrwx   0        0        0        0 2023-05-12 13:01:19.881260 AICreator-0.2.0/AICreator.egg-info/
--rw-rw-rw-   0        0        0      559 2023-05-12 13:01:19.000000 AICreator-0.2.0/AICreator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-05-12 13:01:19.000000 AICreator-0.2.0/AICreator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 13:01:19.000000 AICreator-0.2.0/AICreator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-12 13:01:19.000000 AICreator-0.2.0/AICreator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-12 13:01:19.000000 AICreator-0.2.0/AICreator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-12 13:01:19.883261 AICreator-0.2.0/AICreatorPackage/
--rw-rw-rw-   0        0        0      156 2023-05-02 13:30:46.000000 AICreator-0.2.0/AICreatorPackage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 13:01:19.886260 AICreator-0.2.0/AICreatorPackage/functions1/
--rw-rw-rw-   0        0        0      904 2023-05-12 12:58:58.000000 AICreator-0.2.0/AICreatorPackage/functions1/AICreatorPackage.py
--rw-rw-rw-   0        0        0        0 2022-04-25 10:59:44.000000 AICreator-0.2.0/AICreatorPackage/functions1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 13:01:19.887260 AICreator-0.2.0/AICreatorPackage/functions1/co/
--rw-rw-rw-   0        0        0    52493 2023-05-12 12:14:40.000000 AICreator-0.2.0/AICreatorPackage/functions1/co/co.py
--rw-rw-rw-   0        0        0     1078 2022-04-24 17:23:55.000000 AICreator-0.2.0/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2021-08-13 08:55:17.000000 AICreator-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      559 2023-05-12 13:01:19.893775 AICreator-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       73 2023-05-02 12:11:18.000000 AICreator-0.2.0/README.txt
--rw-rw-rw-   0        0        0        0 2022-04-24 17:21:54.000000 AICreator-0.2.0/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-12 13:01:19.895778 AICreator-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      675 2023-05-12 13:00:59.000000 AICreator-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 13:02:20.744341 AICreator-0.2.1/
+drwxrwxrwx   0        0        0        0 2023-05-12 13:02:20.737827 AICreator-0.2.1/AICreator.egg-info/
+-rw-rw-rw-   0        0        0      559 2023-05-12 13:02:20.000000 AICreator-0.2.1/AICreator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2023-05-12 13:02:20.000000 AICreator-0.2.1/AICreator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 13:02:20.000000 AICreator-0.2.1/AICreator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-12 13:02:20.000000 AICreator-0.2.1/AICreator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-12 13:02:20.000000 AICreator-0.2.1/AICreator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 13:02:20.739334 AICreator-0.2.1/AICreatorPackage/
+-rw-rw-rw-   0        0        0      156 2023-05-02 13:30:46.000000 AICreator-0.2.1/AICreatorPackage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 13:02:20.742343 AICreator-0.2.1/AICreatorPackage/functions/
+-rw-rw-rw-   0        0        0      904 2023-05-12 12:58:58.000000 AICreator-0.2.1/AICreatorPackage/functions/AICreatorPackage.py
+-rw-rw-rw-   0        0        0        0 2022-04-25 10:59:44.000000 AICreator-0.2.1/AICreatorPackage/functions/__init__.py
+-rw-rw-rw-   0        0        0     1078 2022-04-24 17:23:55.000000 AICreator-0.2.1/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2021-08-13 08:55:17.000000 AICreator-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      559 2023-05-12 13:02:20.743348 AICreator-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       73 2023-05-02 12:11:18.000000 AICreator-0.2.1/README.txt
+-rw-rw-rw-   0        0        0        0 2022-04-24 17:21:54.000000 AICreator-0.2.1/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-12 13:02:20.744341 AICreator-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      675 2023-05-12 13:02:07.000000 AICreator-0.2.1/setup.py
```

### Comparing `AICreator-0.2.0/AICreator.egg-info/PKG-INFO` & `AICreator-0.2.1/AICreator.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AICreator
-Version: 0.2.0
+Version: 0.2.1
 Summary: AI Creator Package By - oren
 Home-page: 
 Author: oren
 Author-email: orennadle@gmail.com
 License: MIT
 Keywords: ai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `AICreator-0.2.0/AICreatorPackage/functions1/AICreatorPackage.py` & `AICreator-0.2.1/AICreatorPackage/functions/AICreatorPackage.py`

 * *Files identical despite different names*

### Comparing `AICreator-0.2.0/LICENCE.txt` & `AICreator-0.2.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `AICreator-0.2.0/PKG-INFO` & `AICreator-0.2.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AICreator
-Version: 0.2.0
+Version: 0.2.1
 Summary: AI Creator Package By - oren
 Home-page: 
 Author: oren
 Author-email: orennadle@gmail.com
 License: MIT
 Keywords: ai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `AICreator-0.2.0/setup.py` & `AICreator-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='AICreator',
-    version='0.2.0',
+    version='0.2.1',
     description='AI Creator Package By - oren',
     long_description=open('README.txt').read(),
     url='',
     author='oren',
     author_email='orennadle@gmail.com',
     license='MIT',
     classifiers=classifiers,
```


# Comparing `tmp/jaibasiccalculator-0.0.1.tar.gz` & `tmp/jaibasiccalculator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaibasiccalculator-0.0.1.tar", last modified: Thu May 11 10:19:31 2023, max compression
+gzip compressed data, was "jaibasiccalculator-0.0.2.tar", last modified: Fri May 12 06:06:56 2023, max compression
```

## Comparing `jaibasiccalculator-0.0.1.tar` & `jaibasiccalculator-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 10:19:31.132891 jaibasiccalculator-0.0.1/
--rw-rw-rw-   0        0        0       84 2023-05-11 10:15:05.000000 jaibasiccalculator-0.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1054 2023-05-11 10:19:03.000000 jaibasiccalculator-0.0.1/LICENCE.txt
--rw-rw-rw-   0        0        0       27 2023-05-11 10:15:05.000000 jaibasiccalculator-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      735 2023-05-11 10:19:31.131111 jaibasiccalculator-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      108 2023-05-11 10:15:05.000000 jaibasiccalculator-0.0.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-11 10:19:31.116757 jaibasiccalculator-0.0.1/jaibasiccalculator.egg-info/
--rw-rw-rw-   0        0        0      735 2023-05-11 10:19:30.000000 jaibasiccalculator-0.0.1/jaibasiccalculator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-05-11 10:19:30.000000 jaibasiccalculator-0.0.1/jaibasiccalculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 10:19:30.000000 jaibasiccalculator-0.0.1/jaibasiccalculator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-11 10:19:30.000000 jaibasiccalculator-0.0.1/jaibasiccalculator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-11 10:19:30.000000 jaibasiccalculator-0.0.1/jaibasiccalculator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-11 10:19:31.123757 jaibasiccalculator-0.0.1/joshbasiccalculator/
--rw-rw-rw-   0        0        0      235 2023-05-11 10:15:05.000000 jaibasiccalculator-0.0.1/joshbasiccalculator/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-11 10:19:31.135021 jaibasiccalculator-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      705 2023-05-11 10:18:59.000000 jaibasiccalculator-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 06:06:56.545156 jaibasiccalculator-0.0.2/
+-rw-rw-rw-   0        0        0       84 2023-05-11 10:15:05.000000 jaibasiccalculator-0.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1054 2023-05-11 10:19:03.000000 jaibasiccalculator-0.0.2/LICENCE.txt
+-rw-rw-rw-   0        0        0       27 2023-05-11 10:15:05.000000 jaibasiccalculator-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      735 2023-05-12 06:06:56.542156 jaibasiccalculator-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2023-05-11 10:15:05.000000 jaibasiccalculator-0.0.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 06:06:56.495390 jaibasiccalculator-0.0.2/jaibasiccalculator.egg-info/
+-rw-rw-rw-   0        0        0      735 2023-05-12 06:06:56.000000 jaibasiccalculator-0.0.2/jaibasiccalculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-05-12 06:06:56.000000 jaibasiccalculator-0.0.2/jaibasiccalculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 06:06:56.000000 jaibasiccalculator-0.0.2/jaibasiccalculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-12 06:06:56.000000 jaibasiccalculator-0.0.2/jaibasiccalculator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-12 06:06:56.000000 jaibasiccalculator-0.0.2/jaibasiccalculator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 06:06:56.534156 jaibasiccalculator-0.0.2/joshbasiccalculator/
+-rw-rw-rw-   0        0        0      291 2023-05-12 06:06:21.000000 jaibasiccalculator-0.0.2/joshbasiccalculator/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-05-12 06:05:16.000000 jaibasiccalculator-0.0.2/joshbasiccalculator/main.py
+-rw-rw-rw-   0        0        0       42 2023-05-12 06:06:56.547155 jaibasiccalculator-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      705 2023-05-12 05:46:35.000000 jaibasiccalculator-0.0.2/setup.py
```

### Comparing `jaibasiccalculator-0.0.1/LICENCE.txt` & `jaibasiccalculator-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `jaibasiccalculator-0.0.1/PKG-INFO` & `jaibasiccalculator-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaibasiccalculator
-Version: 0.0.1
+Version: 0.0.2
 Summary: A very basic calculator
 Home-page: UNKNOWN
 Author: Jaideep
 Author-email: jaideepkaushal2@gmail.com
 License: UNKNOWN
 Keywords: calculator
 Platform: UNKNOWN
```

### Comparing `jaibasiccalculator-0.0.1/jaibasiccalculator.egg-info/PKG-INFO` & `jaibasiccalculator-0.0.2/jaibasiccalculator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaibasiccalculator
-Version: 0.0.1
+Version: 0.0.2
 Summary: A very basic calculator
 Home-page: UNKNOWN
 Author: Jaideep
 Author-email: jaideepkaushal2@gmail.com
 License: UNKNOWN
 Keywords: calculator
 Platform: UNKNOWN
```

### Comparing `jaibasiccalculator-0.0.1/setup.py` & `jaibasiccalculator-0.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='jaibasiccalculator',
-  version='0.0.1',
+  version='0.0.2',
   description='A very basic calculator',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Jaideep',
   author_email='jaideepkaushal2@gmail.com',
   license='', 
   classifiers=classifiers,
```


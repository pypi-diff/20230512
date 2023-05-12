# Comparing `tmp/dfdfdfdfhhh-1.0.1.tar.gz` & `tmp/dfdfdfdfhhh-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dfdfdfdfhhh-1.0.1.tar", last modified: Fri May 12 21:17:26 2023, max compression
+gzip compressed data, was "dist\dfdfdfdfhhh-1.0.2.tar", last modified: Fri May 12 21:21:53 2023, max compression
```

## Comparing `dfdfdfdfhhh-1.0.1.tar` & `dfdfdfdfhhh-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 21:17:26.416802 dfdfdfdfhhh-1.0.1/
--rw-rw-rw-   0        0        0      558 2023-05-12 21:17:26.416302 dfdfdfdfhhh-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       39 2023-05-12 18:52:28.000000 dfdfdfdfhhh-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 21:17:26.411302 dfdfdfdfhhh-1.0.1/dfdfdfdfhhh/
--rw-rw-rw-   0        0        0       44 2023-05-12 20:47:44.000000 dfdfdfdfhhh-1.0.1/dfdfdfdfhhh/__init__.py
--rw-rw-rw-   0        0        0       30 2023-05-12 19:11:25.000000 dfdfdfdfhhh-1.0.1/dfdfdfdfhhh/requester.py
-drwxrwxrwx   0        0        0        0 2023-05-12 21:17:26.415302 dfdfdfdfhhh-1.0.1/dfdfdfdfhhh.egg-info/
--rw-rw-rw-   0        0        0      558 2023-05-12 21:17:26.000000 dfdfdfdfhhh-1.0.1/dfdfdfdfhhh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-05-12 21:17:26.000000 dfdfdfdfhhh-1.0.1/dfdfdfdfhhh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 21:17:26.000000 dfdfdfdfhhh-1.0.1/dfdfdfdfhhh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-12 21:17:26.000000 dfdfdfdfhhh-1.0.1/dfdfdfdfhhh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 21:17:26.416802 dfdfdfdfhhh-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1761 2023-05-12 21:17:20.000000 dfdfdfdfhhh-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 21:21:53.185128 dfdfdfdfhhh-1.0.2/
+-rw-rw-rw-   0        0        0      558 2023-05-12 21:21:53.185128 dfdfdfdfhhh-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       39 2023-05-12 18:52:28.000000 dfdfdfdfhhh-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 21:21:53.180628 dfdfdfdfhhh-1.0.2/dfdfdfdfhhh/
+-rw-rw-rw-   0        0        0       44 2023-05-12 20:47:44.000000 dfdfdfdfhhh-1.0.2/dfdfdfdfhhh/__init__.py
+-rw-rw-rw-   0        0        0       30 2023-05-12 19:11:25.000000 dfdfdfdfhhh-1.0.2/dfdfdfdfhhh/requester.py
+drwxrwxrwx   0        0        0        0 2023-05-12 21:21:53.184131 dfdfdfdfhhh-1.0.2/dfdfdfdfhhh.egg-info/
+-rw-rw-rw-   0        0        0      558 2023-05-12 21:21:53.000000 dfdfdfdfhhh-1.0.2/dfdfdfdfhhh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-05-12 21:21:53.000000 dfdfdfdfhhh-1.0.2/dfdfdfdfhhh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 21:21:53.000000 dfdfdfdfhhh-1.0.2/dfdfdfdfhhh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-12 21:21:53.000000 dfdfdfdfhhh-1.0.2/dfdfdfdfhhh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 21:21:53.185630 dfdfdfdfhhh-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1761 2023-05-12 21:21:33.000000 dfdfdfdfhhh-1.0.2/setup.py
```

### Comparing `dfdfdfdfhhh-1.0.1/PKG-INFO` & `dfdfdfdfhhh-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfdfdfdfhhh
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simplified version of urllib
 Author: HW
 Author-email: 
 Keywords: python,http,https,requests,urllib,sockets,tcp
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dfdfdfdfhhh-1.0.1/dfdfdfdfhhh.egg-info/PKG-INFO` & `dfdfdfdfhhh-1.0.2/dfdfdfdfhhh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfdfdfdfhhh
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simplified version of urllib
 Author: HW
 Author-email: 
 Keywords: python,http,https,requests,urllib,sockets,tcp
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dfdfdfdfhhh-1.0.1/setup.py` & `dfdfdfdfhhh-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
 
 
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = 'A simplified version of urllib'
 LONG_DESCRIPTION = 'Use this package to make your https requests.'
 
 class CustomInstallCommand(install):
     def run(self):
         print("hhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhh")
         print("hhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhh")
```


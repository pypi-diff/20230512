# Comparing `tmp/imio.dms.policy-3.0.tar.gz` & `tmp/imio.dms.policy-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imio.dms.policy-3.0.tar", last modified: Fri Aug 27 10:10:42 2021, max compression
+gzip compressed data, was "imio.dms.policy-3.0.1.tar", last modified: Fri May 12 09:55:45 2023, max compression
```

## Comparing `imio.dms.policy-3.0.tar` & `imio.dms.policy-3.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-08-27 10:10:42.285939 imio.dms.policy-3.0/
--rw-rw-r--   0 sge       (1000) sge       (1000)     1083 2021-08-27 10:10:42.000000 imio.dms.policy-3.0/CHANGES.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        7 2021-08-27 10:10:42.000000 imio.dms.policy-3.0/CONTRIBUTORS.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      101 2021-08-27 10:10:42.000000 imio.dms.policy-3.0/MANIFEST.in
--rw-rw-r--   0 sge       (1000) sge       (1000)     2203 2021-08-27 10:10:42.285939 imio.dms.policy-3.0/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)       42 2021-08-27 10:10:42.000000 imio.dms.policy-3.0/README.txt
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-08-27 10:10:42.285939 imio.dms.policy-3.0/docs/
--rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2021-08-27 10:10:42.000000 imio.dms.policy-3.0/docs/LICENSE.GPL
--rw-rw-r--   0 sge       (1000) sge       (1000)      725 2021-08-27 10:10:42.000000 imio.dms.policy-3.0/docs/LICENSE.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       38 2021-08-27 10:10:42.285939 imio.dms.policy-3.0/setup.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)     1708 2021-08-27 10:10:42.000000 imio.dms.policy-3.0/setup.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-08-27 10:10:42.285939 imio.dms.policy-3.0/src/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-08-27 10:10:42.285939 imio.dms.policy-3.0/src/imio/
--rw-rw-r--   0 sge       (1000) sge       (1000)       56 2021-08-27 10:10:42.000000 imio.dms.policy-3.0/src/imio/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-08-27 10:10:42.285939 imio.dms.policy-3.0/src/imio/dms/
--rw-rw-r--   0 sge       (1000) sge       (1000)       56 2021-08-27 10:10:42.000000 imio.dms.policy-3.0/src/imio/dms/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-08-27 10:10:42.285939 imio.dms.policy-3.0/src/imio/dms/policy/
--rw-rw-r--   0 sge       (1000) sge       (1000)       42 2021-08-27 10:10:42.000000 imio.dms.policy-3.0/src/imio/dms/policy/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      588 2021-08-27 10:10:42.000000 imio.dms.policy-3.0/src/imio/dms/policy/configure.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2021-08-27 10:10:42.285939 imio.dms.policy-3.0/src/imio.dms.policy.egg-info/
--rw-rw-r--   0 sge       (1000) sge       (1000)     2203 2021-08-27 10:10:42.000000 imio.dms.policy-3.0/src/imio.dms.policy.egg-info/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)      515 2021-08-27 10:10:42.000000 imio.dms.policy-3.0/src/imio.dms.policy.egg-info/SOURCES.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2021-08-27 10:10:42.000000 imio.dms.policy-3.0/src/imio.dms.policy.egg-info/dependency_links.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       14 2021-08-27 10:10:42.000000 imio.dms.policy-3.0/src/imio.dms.policy.egg-info/namespace_packages.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2021-08-27 10:10:42.000000 imio.dms.policy-3.0/src/imio.dms.policy.egg-info/not-zip-safe
--rw-rw-r--   0 sge       (1000) sge       (1000)      454 2021-08-27 10:10:42.000000 imio.dms.policy-3.0/src/imio.dms.policy.egg-info/requires.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        5 2021-08-27 10:10:42.000000 imio.dms.policy-3.0/src/imio.dms.policy.egg-info/top_level.txt
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-12 09:55:45.844659 imio.dms.policy-3.0.1/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1173 2023-05-12 09:55:45.000000 imio.dms.policy-3.0.1/CHANGES.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        7 2023-05-12 09:55:45.000000 imio.dms.policy-3.0.1/CONTRIBUTORS.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      101 2023-05-12 09:55:45.000000 imio.dms.policy-3.0.1/MANIFEST.in
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1652 2023-05-12 09:55:45.844659 imio.dms.policy-3.0.1/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)       42 2023-05-12 09:55:45.000000 imio.dms.policy-3.0.1/README.txt
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-12 09:55:45.844659 imio.dms.policy-3.0.1/docs/
+-rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2023-05-12 09:55:45.000000 imio.dms.policy-3.0.1/docs/LICENSE.GPL
+-rw-rw-r--   0 sge       (1000) sge       (1000)      725 2023-05-12 09:55:45.000000 imio.dms.policy-3.0.1/docs/LICENSE.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       38 2023-05-12 09:55:45.844659 imio.dms.policy-3.0.1/setup.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1750 2023-05-12 09:55:45.000000 imio.dms.policy-3.0.1/setup.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-12 09:55:45.844659 imio.dms.policy-3.0.1/src/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-12 09:55:45.844659 imio.dms.policy-3.0.1/src/imio/
+-rw-rw-r--   0 sge       (1000) sge       (1000)       56 2023-05-12 09:55:45.000000 imio.dms.policy-3.0.1/src/imio/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-12 09:55:45.844659 imio.dms.policy-3.0.1/src/imio/dms/
+-rw-rw-r--   0 sge       (1000) sge       (1000)       56 2023-05-12 09:55:45.000000 imio.dms.policy-3.0.1/src/imio/dms/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-12 09:55:45.844659 imio.dms.policy-3.0.1/src/imio/dms/policy/
+-rw-rw-r--   0 sge       (1000) sge       (1000)       42 2023-05-12 09:55:45.000000 imio.dms.policy-3.0.1/src/imio/dms/policy/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      640 2023-05-12 09:55:45.000000 imio.dms.policy-3.0.1/src/imio/dms/policy/configure.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2023-05-12 09:55:45.844659 imio.dms.policy-3.0.1/src/imio.dms.policy.egg-info/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1652 2023-05-12 09:55:45.000000 imio.dms.policy-3.0.1/src/imio.dms.policy.egg-info/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)      515 2023-05-12 09:55:45.000000 imio.dms.policy-3.0.1/src/imio.dms.policy.egg-info/SOURCES.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2023-05-12 09:55:45.000000 imio.dms.policy-3.0.1/src/imio.dms.policy.egg-info/dependency_links.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       14 2023-05-12 09:55:45.000000 imio.dms.policy-3.0.1/src/imio.dms.policy.egg-info/namespace_packages.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2023-05-12 09:55:45.000000 imio.dms.policy-3.0.1/src/imio.dms.policy.egg-info/not-zip-safe
+-rw-rw-r--   0 sge       (1000) sge       (1000)      481 2023-05-12 09:55:45.000000 imio.dms.policy-3.0.1/src/imio.dms.policy.egg-info/requires.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        5 2023-05-12 09:55:45.000000 imio.dms.policy-3.0.1/src/imio.dms.policy.egg-info/top_level.txt
```

### Comparing `imio.dms.policy-3.0/CHANGES.txt` & `imio.dms.policy-3.0.1/CHANGES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+3.0.1 (2023-05-12)
+------------------
+
+- Added imio.transmogrifier.iadocs.
+  [sgeulette]
+
 3.0 (2021-08-27)
 ----------------
 
 - Added Products.PloneHotfix20210518.
   [sgeulette]
 
 2.3.post2 (2020-11-05)
```

### Comparing `imio.dms.policy-3.0/docs/LICENSE.GPL` & `imio.dms.policy-3.0.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.dms.policy-3.0/docs/LICENSE.txt` & `imio.dms.policy-3.0.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `imio.dms.policy-3.0/setup.py` & `imio.dms.policy-3.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = '3.0'
+version = '3.0.1'
 
 long_description = (
     open('README.txt').read()
     + '\n' +
     'Contributors\n'
     '============\n'
     + '\n' +
@@ -45,13 +45,14 @@
           'collective.externaleditor',
           'collective.iconifieddocumentactions',
           'collective.messagesviewlet',
           'collective.monitor',
           'collective.usernamelogger',
           'communesplone.layout',
           'imio.transmogrifier.contact',
+          'imio.transmogrifier.iadocs',
           'plonetheme.imioapps',
           'five.z2monitor',
           'Products.PloneHotfix20210518',
           'Products.ZNagios',
           'zc.z3monitor'
       ])
```

### Comparing `imio.dms.policy-3.0/src/imio.dms.policy.egg-info/SOURCES.txt` & `imio.dms.policy-3.0.1/src/imio.dms.policy.egg-info/SOURCES.txt`

 * *Files identical despite different names*


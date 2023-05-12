# Comparing `tmp/capitalpayments-0.0.4.tar.gz` & `tmp/capitalpayments-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capitalpayments-0.0.4.tar", last modified: Thu May 11 23:46:55 2023, max compression
+gzip compressed data, was "capitalpayments-0.0.5.tar", last modified: Thu May 11 23:56:26 2023, max compression
```

## Comparing `capitalpayments-0.0.4.tar` & `capitalpayments-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,12 @@
-drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-11 23:46:55.270728 capitalpayments-0.0.4/
--rw-r--r--   0 javierfernandez   (501) staff       (20)     1066 2023-05-11 21:44:06.000000 capitalpayments-0.0.4/LICENSE
--rw-r--r--   0 javierfernandez   (501) staff       (20)     3247 2023-05-11 23:46:55.270582 capitalpayments-0.0.4/PKG-INFO
--rw-r--r--   0 javierfernandez   (501) staff       (20)     2677 2023-05-11 23:34:46.000000 capitalpayments-0.0.4/README.md
-drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-11 23:46:55.269431 capitalpayments-0.0.4/capitalpayments/
--rw-r--r--   0 javierfernandez   (501) staff       (20)       46 2023-05-11 23:41:41.000000 capitalpayments-0.0.4/capitalpayments/__init__.py
--rw-r--r--   0 javierfernandez   (501) staff       (20)     4191 2023-05-11 23:41:44.000000 capitalpayments-0.0.4/capitalpayments/capitalpayments.py
--rw-r--r--   0 javierfernandez   (501) staff       (20)      620 2023-05-11 23:35:08.000000 capitalpayments-0.0.4/capitalpayments/ipn.py
--rw-r--r--   0 javierfernandez   (501) staff       (20)     2073 2023-05-11 19:07:42.000000 capitalpayments-0.0.4/capitalpayments/url_manager.py
-drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-11 23:46:55.270340 capitalpayments-0.0.4/capitalpayments.egg-info/
--rw-r--r--   0 javierfernandez   (501) staff       (20)     3247 2023-05-11 23:46:55.000000 capitalpayments-0.0.4/capitalpayments.egg-info/PKG-INFO
--rw-r--r--   0 javierfernandez   (501) staff       (20)      337 2023-05-11 23:46:55.000000 capitalpayments-0.0.4/capitalpayments.egg-info/SOURCES.txt
--rw-r--r--   0 javierfernandez   (501) staff       (20)        1 2023-05-11 23:46:55.000000 capitalpayments-0.0.4/capitalpayments.egg-info/dependency_links.txt
--rw-r--r--   0 javierfernandez   (501) staff       (20)        9 2023-05-11 23:46:55.000000 capitalpayments-0.0.4/capitalpayments.egg-info/requires.txt
--rw-r--r--   0 javierfernandez   (501) staff       (20)       16 2023-05-11 23:46:55.000000 capitalpayments-0.0.4/capitalpayments.egg-info/top_level.txt
--rw-r--r--   0 javierfernandez   (501) staff       (20)       38 2023-05-11 23:46:55.270768 capitalpayments-0.0.4/setup.cfg
--rw-r--r--   0 javierfernandez   (501) staff       (20)     1091 2023-05-11 23:42:06.000000 capitalpayments-0.0.4/setup.py
+drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-11 23:56:26.928398 capitalpayments-0.0.5/
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     1066 2023-05-11 21:44:06.000000 capitalpayments-0.0.5/LICENSE
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     3247 2023-05-11 23:56:26.928147 capitalpayments-0.0.5/PKG-INFO
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     2677 2023-05-11 23:34:46.000000 capitalpayments-0.0.5/README.md
+drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-11 23:56:26.927934 capitalpayments-0.0.5/capitalpayments.egg-info/
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     3247 2023-05-11 23:56:26.000000 capitalpayments-0.0.5/capitalpayments.egg-info/PKG-INFO
+-rw-r--r--   0 javierfernandez   (501) staff       (20)      220 2023-05-11 23:56:26.000000 capitalpayments-0.0.5/capitalpayments.egg-info/SOURCES.txt
+-rw-r--r--   0 javierfernandez   (501) staff       (20)        1 2023-05-11 23:56:26.000000 capitalpayments-0.0.5/capitalpayments.egg-info/dependency_links.txt
+-rw-r--r--   0 javierfernandez   (501) staff       (20)        9 2023-05-11 23:56:26.000000 capitalpayments-0.0.5/capitalpayments.egg-info/requires.txt
+-rw-r--r--   0 javierfernandez   (501) staff       (20)        1 2023-05-11 23:56:26.000000 capitalpayments-0.0.5/capitalpayments.egg-info/top_level.txt
+-rw-r--r--   0 javierfernandez   (501) staff       (20)       38 2023-05-11 23:56:26.928455 capitalpayments-0.0.5/setup.cfg
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     1091 2023-05-11 23:56:23.000000 capitalpayments-0.0.5/setup.py
```

### Comparing `capitalpayments-0.0.4/LICENSE` & `capitalpayments-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `capitalpayments-0.0.4/PKG-INFO` & `capitalpayments-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capitalpayments
-Version: 0.0.4
+Version: 0.0.5
 Summary: For Api Capital Payments
 Author: Javier (leqjl93)
 Author-email: <javier.fernandez.pa93@gmail.com>
 Keywords: python,capitalpayments,paymentprocessor,usdt.trc20
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `capitalpayments-0.0.4/README.md` & `capitalpayments-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `capitalpayments-0.0.4/capitalpayments.egg-info/PKG-INFO` & `capitalpayments-0.0.5/capitalpayments.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capitalpayments
-Version: 0.0.4
+Version: 0.0.5
 Summary: For Api Capital Payments
 Author: Javier (leqjl93)
 Author-email: <javier.fernandez.pa93@gmail.com>
 Keywords: python,capitalpayments,paymentprocessor,usdt.trc20
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `capitalpayments-0.0.4/setup.py` & `capitalpayments-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'For Api Capital Payments'
 LONG_DESCRIPTION = 'This SDK connects to Capital Payments Payment Processor Api.'
 
 # Setting up
 setup(
     name="capitalpayments",
     version=VERSION,
```


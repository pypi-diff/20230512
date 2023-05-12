# Comparing `tmp/capitalpayments-0.0.7.tar.gz` & `tmp/capitalpayments-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capitalpayments-0.0.7.tar", last modified: Fri May 12 00:10:17 2023, max compression
+gzip compressed data, was "capitalpayments-0.0.9.tar", last modified: Fri May 12 00:59:04 2023, max compression
```

## Comparing `capitalpayments-0.0.7.tar` & `capitalpayments-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-12 00:10:17.837730 capitalpayments-0.0.7/
--rw-r--r--   0 javierfernandez   (501) staff       (20)     1066 2023-05-11 21:44:06.000000 capitalpayments-0.0.7/LICENSE
--rw-r--r--   0 javierfernandez   (501) staff       (20)     3247 2023-05-12 00:10:17.837583 capitalpayments-0.0.7/PKG-INFO
--rw-r--r--   0 javierfernandez   (501) staff       (20)     2677 2023-05-12 00:01:07.000000 capitalpayments-0.0.7/README.md
-drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-12 00:10:17.836417 capitalpayments-0.0.7/capitalpayments/
--rw-r--r--   0 javierfernandez   (501) staff       (20)       35 2023-05-12 00:10:03.000000 capitalpayments-0.0.7/capitalpayments/__init__.py
--rw-r--r--   0 javierfernandez   (501) staff       (20)     4176 2023-05-12 00:09:55.000000 capitalpayments-0.0.7/capitalpayments/capitalpaymentscore.py
--rw-r--r--   0 javierfernandez   (501) staff       (20)      620 2023-05-11 23:35:08.000000 capitalpayments-0.0.7/capitalpayments/ipn.py
--rw-r--r--   0 javierfernandez   (501) staff       (20)     2073 2023-05-11 19:07:42.000000 capitalpayments-0.0.7/capitalpayments/url_manager.py
-drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-12 00:10:17.837377 capitalpayments-0.0.7/capitalpayments.egg-info/
--rw-r--r--   0 javierfernandez   (501) staff       (20)     3247 2023-05-12 00:10:17.000000 capitalpayments-0.0.7/capitalpayments.egg-info/PKG-INFO
--rw-r--r--   0 javierfernandez   (501) staff       (20)      341 2023-05-12 00:10:17.000000 capitalpayments-0.0.7/capitalpayments.egg-info/SOURCES.txt
--rw-r--r--   0 javierfernandez   (501) staff       (20)        1 2023-05-12 00:10:17.000000 capitalpayments-0.0.7/capitalpayments.egg-info/dependency_links.txt
--rw-r--r--   0 javierfernandez   (501) staff       (20)        9 2023-05-12 00:10:17.000000 capitalpayments-0.0.7/capitalpayments.egg-info/requires.txt
--rw-r--r--   0 javierfernandez   (501) staff       (20)       16 2023-05-12 00:10:17.000000 capitalpayments-0.0.7/capitalpayments.egg-info/top_level.txt
--rw-r--r--   0 javierfernandez   (501) staff       (20)       38 2023-05-12 00:10:17.837768 capitalpayments-0.0.7/setup.cfg
--rw-r--r--   0 javierfernandez   (501) staff       (20)     1091 2023-05-12 00:10:12.000000 capitalpayments-0.0.7/setup.py
+drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-12 00:59:04.695207 capitalpayments-0.0.9/
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     1066 2023-05-11 21:44:06.000000 capitalpayments-0.0.9/LICENSE
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     3247 2023-05-12 00:59:04.695053 capitalpayments-0.0.9/PKG-INFO
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     2677 2023-05-12 00:01:07.000000 capitalpayments-0.0.9/README.md
+drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-12 00:59:04.694119 capitalpayments-0.0.9/capitalpayments/
+-rw-r--r--   0 javierfernandez   (501) staff       (20)       36 2023-05-12 00:50:40.000000 capitalpayments-0.0.9/capitalpayments/__init__.py
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     4177 2023-05-12 00:58:50.000000 capitalpayments-0.0.9/capitalpayments/capitalpaymentscore.py
+-rw-r--r--   0 javierfernandez   (501) staff       (20)      620 2023-05-11 23:35:08.000000 capitalpayments-0.0.9/capitalpayments/ipn.py
+-rw-r--r--   0 javierfernandez   (501) staff       (20)      977 2023-05-12 00:58:48.000000 capitalpayments-0.0.9/capitalpayments/url_manager.py
+drwxr-xr-x   0 javierfernandez   (501) staff       (20)        0 2023-05-12 00:59:04.694860 capitalpayments-0.0.9/capitalpayments.egg-info/
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     3247 2023-05-12 00:59:04.000000 capitalpayments-0.0.9/capitalpayments.egg-info/PKG-INFO
+-rw-r--r--   0 javierfernandez   (501) staff       (20)      341 2023-05-12 00:59:04.000000 capitalpayments-0.0.9/capitalpayments.egg-info/SOURCES.txt
+-rw-r--r--   0 javierfernandez   (501) staff       (20)        1 2023-05-12 00:59:04.000000 capitalpayments-0.0.9/capitalpayments.egg-info/dependency_links.txt
+-rw-r--r--   0 javierfernandez   (501) staff       (20)        9 2023-05-12 00:59:04.000000 capitalpayments-0.0.9/capitalpayments.egg-info/requires.txt
+-rw-r--r--   0 javierfernandez   (501) staff       (20)       16 2023-05-12 00:59:04.000000 capitalpayments-0.0.9/capitalpayments.egg-info/top_level.txt
+-rw-r--r--   0 javierfernandez   (501) staff       (20)       38 2023-05-12 00:59:04.695251 capitalpayments-0.0.9/setup.cfg
+-rw-r--r--   0 javierfernandez   (501) staff       (20)     1091 2023-05-12 00:50:47.000000 capitalpayments-0.0.9/setup.py
```

### Comparing `capitalpayments-0.0.7/LICENSE` & `capitalpayments-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `capitalpayments-0.0.7/PKG-INFO` & `capitalpayments-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capitalpayments
-Version: 0.0.7
+Version: 0.0.9
 Summary: For Api Capital Payments
 Author: Javier (leqjl93)
 Author-email: <javier.fernandez.pa93@gmail.com>
 Keywords: python,capitalpayments,paymentprocessor,usdt.trc20
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `capitalpayments-0.0.7/README.md` & `capitalpayments-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `capitalpayments-0.0.7/capitalpayments/capitalpaymentscore.py` & `capitalpayments-0.0.9/capitalpayments/capitalpaymentscore.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from url_manager import url_manager
+from .url_manager import url_manager
 import requests
 
 class SDK:
     def __init__(self, api_key, api_secret):
         self.api_key = api_key
         self.api_secret = api_secret
     def getLogin(self):
```

### Comparing `capitalpayments-0.0.7/capitalpayments/ipn.py` & `capitalpayments-0.0.9/capitalpayments/ipn.py`

 * *Files identical despite different names*

### Comparing `capitalpayments-0.0.7/capitalpayments.egg-info/PKG-INFO` & `capitalpayments-0.0.9/capitalpayments.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capitalpayments
-Version: 0.0.7
+Version: 0.0.9
 Summary: For Api Capital Payments
 Author: Javier (leqjl93)
 Author-email: <javier.fernandez.pa93@gmail.com>
 Keywords: python,capitalpayments,paymentprocessor,usdt.trc20
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `capitalpayments-0.0.7/setup.py` & `capitalpayments-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.7'
+VERSION = '0.0.9'
 DESCRIPTION = 'For Api Capital Payments'
 LONG_DESCRIPTION = 'This SDK connects to Capital Payments Payment Processor Api.'
 
 # Setting up
 setup(
     name="capitalpayments",
     version=VERSION,
```


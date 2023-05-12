# Comparing `tmp/zebedee-0.0.3.tar.gz` & `tmp/zebedee-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zebedee-0.0.3.tar", last modified: Thu May 11 06:00:45 2023, max compression
+gzip compressed data, was "zebedee-0.0.4.tar", last modified: Fri May 12 18:57:05 2023, max compression
```

## Comparing `zebedee-0.0.3.tar` & `zebedee-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 santos     (501) staff       (20)        0 2023-05-11 06:00:45.554039 zebedee-0.0.3/
--rw-r--r--   0 santos     (501) staff       (20)     1065 2023-04-03 00:04:47.000000 zebedee-0.0.3/LICENSE
--rw-r--r--   0 santos     (501) staff       (20)     7008 2023-05-11 06:00:45.553914 zebedee-0.0.3/PKG-INFO
--rw-r--r--   0 santos     (501) staff       (20)     6420 2023-05-11 06:00:25.000000 zebedee-0.0.3/README.md
--rw-r--r--   0 santos     (501) staff       (20)       38 2023-05-11 06:00:45.554077 zebedee-0.0.3/setup.cfg
--rw-r--r--   0 santos     (501) staff       (20)     1167 2023-05-11 06:00:38.000000 zebedee-0.0.3/setup.py
-drwxr-xr-x   0 santos     (501) staff       (20)        0 2023-05-11 06:00:45.553048 zebedee-0.0.3/zebedee/
--rw-r--r--   0 santos     (501) staff       (20)       19 2023-05-11 05:51:33.000000 zebedee-0.0.3/zebedee/__init__.py
--rw-r--r--   0 santos     (501) staff       (20)    10852 2023-05-11 05:51:16.000000 zebedee-0.0.3/zebedee/main.py
-drwxr-xr-x   0 santos     (501) staff       (20)        0 2023-05-11 06:00:45.553736 zebedee-0.0.3/zebedee.egg-info/
--rw-r--r--   0 santos     (501) staff       (20)     7008 2023-05-11 06:00:45.000000 zebedee-0.0.3/zebedee.egg-info/PKG-INFO
--rw-r--r--   0 santos     (501) staff       (20)      216 2023-05-11 06:00:45.000000 zebedee-0.0.3/zebedee.egg-info/SOURCES.txt
--rw-r--r--   0 santos     (501) staff       (20)        1 2023-05-11 06:00:45.000000 zebedee-0.0.3/zebedee.egg-info/dependency_links.txt
--rw-r--r--   0 santos     (501) staff       (20)       49 2023-05-11 06:00:45.000000 zebedee-0.0.3/zebedee.egg-info/requires.txt
--rw-r--r--   0 santos     (501) staff       (20)        8 2023-05-11 06:00:45.000000 zebedee-0.0.3/zebedee.egg-info/top_level.txt
+drwxr-xr-x   0 santos     (501) staff       (20)        0 2023-05-12 18:57:05.063788 zebedee-0.0.4/
+-rw-r--r--   0 santos     (501) staff       (20)     1065 2023-04-03 00:04:47.000000 zebedee-0.0.4/LICENSE
+-rw-r--r--   0 santos     (501) staff       (20)     7008 2023-05-12 18:57:05.063618 zebedee-0.0.4/PKG-INFO
+-rw-r--r--   0 santos     (501) staff       (20)     6420 2023-05-11 06:00:25.000000 zebedee-0.0.4/README.md
+-rw-r--r--   0 santos     (501) staff       (20)       38 2023-05-12 18:57:05.063846 zebedee-0.0.4/setup.cfg
+-rw-r--r--   0 santos     (501) staff       (20)     1167 2023-05-12 18:57:01.000000 zebedee-0.0.4/setup.py
+drwxr-xr-x   0 santos     (501) staff       (20)        0 2023-05-12 18:57:05.062493 zebedee-0.0.4/zebedee/
+-rw-r--r--   0 santos     (501) staff       (20)       19 2023-05-11 05:51:33.000000 zebedee-0.0.4/zebedee/__init__.py
+-rw-r--r--   0 santos     (501) staff       (20)    10974 2023-05-12 18:52:57.000000 zebedee-0.0.4/zebedee/main.py
+drwxr-xr-x   0 santos     (501) staff       (20)        0 2023-05-12 18:57:05.063318 zebedee-0.0.4/zebedee.egg-info/
+-rw-r--r--   0 santos     (501) staff       (20)     7008 2023-05-12 18:57:05.000000 zebedee-0.0.4/zebedee.egg-info/PKG-INFO
+-rw-r--r--   0 santos     (501) staff       (20)      216 2023-05-12 18:57:05.000000 zebedee-0.0.4/zebedee.egg-info/SOURCES.txt
+-rw-r--r--   0 santos     (501) staff       (20)        1 2023-05-12 18:57:05.000000 zebedee-0.0.4/zebedee.egg-info/dependency_links.txt
+-rw-r--r--   0 santos     (501) staff       (20)       49 2023-05-12 18:57:05.000000 zebedee-0.0.4/zebedee.egg-info/requires.txt
+-rw-r--r--   0 santos     (501) staff       (20)        8 2023-05-12 18:57:05.000000 zebedee-0.0.4/zebedee.egg-info/top_level.txt
```

### Comparing `zebedee-0.0.3/LICENSE` & `zebedee-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zebedee-0.0.3/PKG-INFO` & `zebedee-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zebedee
-Version: 0.0.3
+Version: 0.0.4
 Summary: Move Money at the Speed of the Internet 
 Author: zantoshi (Santos Hernandez)
 Author-email: <santosdhernandez@gmail.com>
 Keywords: python,payments,bitcoin,lightning network,django,lightning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zebedee-0.0.3/README.md` & `zebedee-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `zebedee-0.0.3/setup.py` & `zebedee-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Move Money at the Speed of the Internet '
 LONG_DESCRIPTION = 'A package that allows for faster integration of the ZEBEDEE API.'
 
 # Setting up
 setup(
     name="zebedee",
     version=VERSION,
```

### Comparing `zebedee-0.0.3/zebedee/main.py` & `zebedee-0.0.4/zebedee/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import requests, json, math
 
-class ZBD:
+class Project:
 
     '''
         This is the ZEBEDEE API library for python programmers.
         The full api reference available at https://api-reference.zebedee.io/
         Documentation is available at https://docs.zebedee.io .
     '''
 
     '''
         The goal of this library is to increase at which developers are able to deliver lightning payment solutions.
     '''
 
-    def __init__(self, apikey, callback_url = None):
+    def __init__(self, apikey, callback_url = ""):
         self.apikey = apikey
         self.callback_url = callback_url
 
     def __str__(self):
         return "ZEBEDEE Project Object"
 
     '''
@@ -168,22 +168,29 @@
         return requests.get(URL, headers=heads).json()["data"]
     
     def send_payment_to_lightning_address(self, lightning_address, amount_msats, comment, internal_id):
         URL = 'https://api.zebedee.io/v0/ln-address/send-payment'
         heads = {'Content-Type': 'application/json', 'apikey': self.apikey}
 
         payload = json.dumps({
-            "lnAddress": lightning_address,
+            "lnAddress": "santos@zbd.gg",
             "amount": str(amount_msats),
+            "unit" : "msats",
             "comment": comment,
             "callbackUrl": self.callback_url,
             "internalId": internal_id
         })
+        res = requests.post(URL, headers=heads, data=payload).json()
+        try:
+            return res["data"]
+        except:
+            return res
+        
 
-        return requests.post(URL, headers=heads, data=payload).json()["data"]
+        
 
     def fetch_charge_from_lightning_address(self, lightning_address, amount_msats, description):
         URL = 'https://api.zebedee.io/v0/ln-address/fetch-charge'
         heads = {'Content-Type': 'application/json', 'apikey': self.apikey}
 
         payload = json.dumps({
             "lnaddress": lightning_address,
```

### Comparing `zebedee-0.0.3/zebedee.egg-info/PKG-INFO` & `zebedee-0.0.4/zebedee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zebedee
-Version: 0.0.3
+Version: 0.0.4
 Summary: Move Money at the Speed of the Internet 
 Author: zantoshi (Santos Hernandez)
 Author-email: <santosdhernandez@gmail.com>
 Keywords: python,payments,bitcoin,lightning network,django,lightning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```


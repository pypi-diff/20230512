# Comparing `tmp/eyes_soatra-0.0.20.tar.gz` & `tmp/eyes_soatra-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyes_soatra-0.0.20.tar", last modified: Thu May 11 09:50:35 2023, max compression
+gzip compressed data, was "eyes_soatra-0.0.21.tar", last modified: Fri May 12 01:15:54 2023, max compression
```

## Comparing `eyes_soatra-0.0.20.tar` & `eyes_soatra-0.0.21.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-11 09:50:35.232869 eyes_soatra-0.0.20/
--rw-r--r--   0 soatra     (501) staff       (20)       13 2023-05-02 07:13:47.000000 eyes_soatra-0.0.20/LICENSE
--rw-r--r--   0 soatra     (501) staff       (20)      554 2023-05-11 09:50:35.232741 eyes_soatra-0.0.20/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)       49 2023-05-11 09:42:34.000000 eyes_soatra-0.0.20/README.md
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-11 09:50:35.228375 eyes_soatra-0.0.20/eyes_soatra/
--rw-r--r--   0 soatra     (501) staff       (20)       28 2023-05-02 07:14:02.000000 eyes_soatra-0.0.20/eyes_soatra/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-11 09:50:35.229434 eyes_soatra-0.0.20/eyes_soatra/depends/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-02 07:07:54.000000 eyes_soatra-0.0.20/eyes_soatra/depends/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)     7691 2023-05-11 01:49:20.000000 eyes_soatra-0.0.20/eyes_soatra/depends/depends_404.py
--rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.20/eyes_soatra/depends/depends_no_data.py
--rw-r--r--   0 soatra     (501) staff       (20)    12902 2023-05-11 09:41:42.000000 eyes_soatra-0.0.20/eyes_soatra/eyes.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-11 09:50:35.229786 eyes_soatra-0.0.20/eyes_soatra/needs/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-11 07:51:47.000000 eyes_soatra-0.0.20/eyes_soatra/needs/__init__.py
--rw-rw-r--   0 soatra     (501) staff       (20)  1339531 2023-05-11 09:13:03.000000 eyes_soatra-0.0.20/eyes_soatra/needs/user_agends.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-11 09:50:35.228970 eyes_soatra-0.0.20/eyes_soatra.egg-info/
--rw-r--r--   0 soatra     (501) staff       (20)      554 2023-05-11 09:50:35.000000 eyes_soatra-0.0.20/eyes_soatra.egg-info/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)      440 2023-05-11 09:50:35.000000 eyes_soatra-0.0.20/eyes_soatra.egg-info/SOURCES.txt
--rw-r--r--   0 soatra     (501) staff       (20)        1 2023-05-11 09:50:35.000000 eyes_soatra-0.0.20/eyes_soatra.egg-info/dependency_links.txt
--rw-r--r--   0 soatra     (501) staff       (20)       43 2023-05-11 09:50:35.000000 eyes_soatra-0.0.20/eyes_soatra.egg-info/requires.txt
--rw-r--r--   0 soatra     (501) staff       (20)       12 2023-05-11 09:50:35.000000 eyes_soatra-0.0.20/eyes_soatra.egg-info/top_level.txt
--rw-r--r--   0 soatra     (501) staff       (20)       38 2023-05-11 09:50:35.232912 eyes_soatra-0.0.20/setup.cfg
--rw-r--r--   0 soatra     (501) staff       (20)     1131 2023-05-10 03:53:31.000000 eyes_soatra-0.0.20/setup.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-11 09:50:35.232351 eyes_soatra-0.0.20/test/
--rw-r--r--   0 soatra     (501) staff       (20)     2464 2023-05-11 09:35:34.000000 eyes_soatra-0.0.20/test/test.py
--rw-r--r--   0 soatra     (501) staff       (20)     1495 2023-05-11 09:30:34.000000 eyes_soatra-0.0.20/test/test2.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-12 01:15:54.596730 eyes_soatra-0.0.21/
+-rw-r--r--   0 soatra     (501) staff       (20)       13 2023-05-02 07:13:47.000000 eyes_soatra-0.0.21/LICENSE
+-rw-r--r--   0 soatra     (501) staff       (20)      554 2023-05-12 01:15:54.596590 eyes_soatra-0.0.21/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)       49 2023-05-11 09:42:34.000000 eyes_soatra-0.0.21/README.md
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-12 01:15:54.594041 eyes_soatra-0.0.21/eyes_soatra/
+-rw-r--r--   0 soatra     (501) staff       (20)       28 2023-05-02 07:14:02.000000 eyes_soatra-0.0.21/eyes_soatra/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-12 01:15:54.595128 eyes_soatra-0.0.21/eyes_soatra/depends/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-02 07:07:54.000000 eyes_soatra-0.0.21/eyes_soatra/depends/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)     7691 2023-05-11 01:49:20.000000 eyes_soatra-0.0.21/eyes_soatra/depends/depends_404.py
+-rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.21/eyes_soatra/depends/depends_no_data.py
+-rw-r--r--   0 soatra     (501) staff       (20)    12552 2023-05-12 01:08:59.000000 eyes_soatra-0.0.21/eyes_soatra/eyes.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-12 01:15:54.595354 eyes_soatra-0.0.21/eyes_soatra/needs/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-11 07:51:47.000000 eyes_soatra-0.0.21/eyes_soatra/needs/__init__.py
+-rw-rw-r--   0 soatra     (501) staff       (20)  1339531 2023-05-11 09:13:03.000000 eyes_soatra-0.0.21/eyes_soatra/needs/user_agents.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-12 01:15:54.594640 eyes_soatra-0.0.21/eyes_soatra.egg-info/
+-rw-r--r--   0 soatra     (501) staff       (20)      554 2023-05-12 01:15:54.000000 eyes_soatra-0.0.21/eyes_soatra.egg-info/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)      440 2023-05-12 01:15:54.000000 eyes_soatra-0.0.21/eyes_soatra.egg-info/SOURCES.txt
+-rw-r--r--   0 soatra     (501) staff       (20)        1 2023-05-12 01:15:54.000000 eyes_soatra-0.0.21/eyes_soatra.egg-info/dependency_links.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       43 2023-05-12 01:15:54.000000 eyes_soatra-0.0.21/eyes_soatra.egg-info/requires.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       12 2023-05-12 01:15:54.000000 eyes_soatra-0.0.21/eyes_soatra.egg-info/top_level.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       38 2023-05-12 01:15:54.596774 eyes_soatra-0.0.21/setup.cfg
+-rw-r--r--   0 soatra     (501) staff       (20)     1131 2023-05-12 01:15:52.000000 eyes_soatra-0.0.21/setup.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-12 01:15:54.596387 eyes_soatra-0.0.21/test/
+-rw-r--r--   0 soatra     (501) staff       (20)     2463 2023-05-12 01:14:42.000000 eyes_soatra-0.0.21/test/test.py
+-rw-r--r--   0 soatra     (501) staff       (20)     1495 2023-05-11 09:30:34.000000 eyes_soatra-0.0.21/test/test2.py
```

### Comparing `eyes_soatra-0.0.20/PKG-INFO` & `eyes_soatra-0.0.21/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyes_soatra
-Version: 0.0.20
+Version: 0.0.21
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: python,crawler,scanner,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eyes_soatra-0.0.20/eyes_soatra/depends/depends_404.py` & `eyes_soatra-0.0.21/eyes_soatra/depends/depends_404.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.20/eyes_soatra/eyes.py` & `eyes_soatra-0.0.21/eyes_soatra/eyes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!python3
-from eyes_soatra.depends.depends_404 import depends as __depends_404
 from eyes_soatra.depends.depends_no_data import depends as __depends_no_data
+from eyes_soatra.depends.depends_404 import depends as __depends_404
 from eyes_soatra.needs.user_agents import User_Agents as __User_Agents
 from translate import Translator as __Translator
 from requests_html import HTML as __HTML
-import requests as __requests
 import jellyfish as __jellyfish
-import re as __re
+import requests as __requests
+import random as __random
 import time as __time
-import random
+import re as __re
 
 # Suppress only the single warning from urllib3 needed.
 __requests.packages.urllib3.disable_warnings()
 __requests.packages.urllib3.util.ssl_.DEFAULT_CIPHERS += ':HIGH:!DH:!aNULL'
 try:
     __requests.packages.urllib3.contrib.pyopenssl.util.ssl_.DEFAULT_CIPHERS += ':HIGH:!DH:!aNULL'
 except AttributeError:
@@ -82,15 +82,14 @@
     for xpath in __header_xpaths + (header_xpath if type(header_xpath) == list else []):
         header_list = html.xpath(f'({xpath})//text()')
         header = ' '.join(header_list)
         header = __strip(header)
         
         if len(header) >= __header_min_length:
             header_texts.append(header)
-        # for header in header_list:
     
     for xpath in __paragraph_xpaths + (paragraph_xpath if type(paragraph_xpath) == list else []):
         paragraph_list = html.xpath(f'({xpath})//text()')
         paragraph = ' '.join(paragraph_list)
         paragraph = __strip(paragraph)
         
         if len(paragraph) >= __paragraph_min_length:
@@ -155,17 +154,14 @@
         for depend in __depends_404 + (depends if type(depends) == list else []):
             for header in headers:                
                 for token_header in __re.split(__separator + (separator if separator else ''), header):
                     token_header = __strip(token_header)
                     
                     if len(token_header) >= __header_min_length:
                         s1 = __jellyfish.jaro_similarity(depend, token_header)
-                        # s2 = __jellyfish.jaro_winkler_similarity(depend, token_header)
-                        
-                        # points = (s1 + s2) / 2
                         points = s1
                         
                         if points > header_high_point:
                             header_high_point = points
                             header_similar = depend
                             header_keyword = token_header
                             
@@ -199,17 +195,14 @@
         for depend in __depends_no_data + (depends if type(depends) == list else []):
             for paragraph in paragraphs:
                 for token_paragraph in __re.split(__separator + (separator if separator else ''), paragraph):
                     token_paragraph = __strip(token_paragraph)
                     
                     if len(token_paragraph) >= __paragraph_min_length:
                         s1 = __jellyfish.jaro_similarity(depend, token_paragraph)
-                        # s2 = __jellyfish.jaro_winkler_similarity(depend, token_paragraph)
-                        
-                        # points = (s1 + s2) / 2
                         points = s1
                         
                         if points > paragraph_high_point:
                             paragraph_high_point = points
                             paragraph_similar = depend
                             paragraph_keyword = token_paragraph
                             
@@ -272,18 +265,18 @@
 ):
     tried = 0
     agents = []
     
     while True:
         try:
             tried += 1
-            user_agent = random.choice(__User_Agents)
+            user_agent = __random.choice(__User_Agents)
             
             while user_agent in agents:
-                user_agent = random.choice(__User_Agents)
+                user_agent = __random.choice(__User_Agents)
                 
             agents.append(user_agent)
                 
             response = __requests.get(
                 **requests_options,
                 url=url,
                 timeout=timeout,
```

### Comparing `eyes_soatra-0.0.20/eyes_soatra/needs/user_agends.py` & `eyes_soatra-0.0.21/eyes_soatra/needs/user_agents.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.20/eyes_soatra.egg-info/PKG-INFO` & `eyes_soatra-0.0.21/eyes_soatra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyes-soatra
-Version: 0.0.20
+Version: 0.0.21
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: python,crawler,scanner,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eyes_soatra-0.0.20/setup.py` & `eyes_soatra-0.0.21/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 NAME = 'eyes_soatra'
-VERSION = '0.0.20'
+VERSION = '0.0.21'
 DESCRIPTION = 'Eyes'
 
 AUTHOR_NAME = 'Soatra'
 AUTHOR_EMAIL = 'johnsoatra@gmail.com'
 
 # Setting up
 setup(
```

### Comparing `eyes_soatra-0.0.20/test/test.py` & `eyes_soatra-0.0.21/test/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!python3
 from threading import Thread
 from eyes_soatra import eyes
 import pandas
 import json
 import argparse
 
-read_from = 'test/data/exported.csv'
+read_from = 'test/data/approve.csv'
 records = pandas.read_csv(read_from).values
 founds = []
 
 def save_file(write_to):
     f = open(write_to, "w")
     
     try:
```

### Comparing `eyes_soatra-0.0.20/test/test2.py` & `eyes_soatra-0.0.21/test/test2.py`

 * *Files identical despite different names*


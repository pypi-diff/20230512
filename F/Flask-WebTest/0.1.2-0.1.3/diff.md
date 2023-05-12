# Comparing `tmp/Flask-WebTest-0.1.2.tar.gz` & `tmp/Flask-WebTest-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-WebTest-0.1.2.tar", last modified: Fri May 12 18:02:34 2023, max compression
+gzip compressed data, was "Flask-WebTest-0.1.3.tar", last modified: Fri May 12 18:59:49 2023, max compression
```

## Comparing `Flask-WebTest-0.1.2.tar` & `Flask-WebTest-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 18:02:34.967770 Flask-WebTest-0.1.2/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 18:02:34.967770 Flask-WebTest-0.1.2/Flask_WebTest.egg-info/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      803 2023-05-12 18:02:34.000000 Flask-WebTest-0.1.2/Flask_WebTest.egg-info/PKG-INFO
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      345 2023-05-12 18:02:34.000000 Flask-WebTest-0.1.2/Flask_WebTest.egg-info/SOURCES.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2023-05-12 18:02:34.000000 Flask-WebTest-0.1.2/Flask_WebTest.egg-info/dependency_links.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2022-08-16 18:02:52.000000 Flask-WebTest-0.1.2/Flask_WebTest.egg-info/not-zip-safe
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       55 2023-05-12 18:02:34.000000 Flask-WebTest-0.1.2/Flask_WebTest.egg-info/requires.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       14 2023-05-12 18:02:34.000000 Flask-WebTest-0.1.2/Flask_WebTest.egg-info/top_level.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1459 2022-08-16 18:00:53.000000 Flask-WebTest-0.1.2/LICENSE
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      803 2023-05-12 18:02:34.967770 Flask-WebTest-0.1.2/PKG-INFO
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      783 2023-03-02 13:34:53.000000 Flask-WebTest-0.1.2/README.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    11760 2023-05-12 18:01:09.000000 Flask-WebTest-0.1.2/flask_webtest.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       67 2023-05-12 18:02:34.967770 Flask-WebTest-0.1.2/setup.cfg
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1341 2023-03-02 13:42:43.000000 Flask-WebTest-0.1.2/setup.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 18:02:34.967770 Flask-WebTest-0.1.2/tests/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2022-08-16 18:00:53.000000 Flask-WebTest-0.1.2/tests/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      680 2023-05-12 16:27:27.000000 Flask-WebTest-0.1.2/tests/core.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1102 2023-03-02 13:34:53.000000 Flask-WebTest-0.1.2/tests/core_sqlalchemy.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4074 2023-05-12 16:25:42.000000 Flask-WebTest-0.1.2/tests/test.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 18:59:49.127525 Flask-WebTest-0.1.3/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 18:59:49.127525 Flask-WebTest-0.1.3/Flask_WebTest.egg-info/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      803 2023-05-12 18:59:48.000000 Flask-WebTest-0.1.3/Flask_WebTest.egg-info/PKG-INFO
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      345 2023-05-12 18:59:48.000000 Flask-WebTest-0.1.3/Flask_WebTest.egg-info/SOURCES.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2023-05-12 18:59:48.000000 Flask-WebTest-0.1.3/Flask_WebTest.egg-info/dependency_links.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2022-08-16 18:02:52.000000 Flask-WebTest-0.1.3/Flask_WebTest.egg-info/not-zip-safe
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       55 2023-05-12 18:59:48.000000 Flask-WebTest-0.1.3/Flask_WebTest.egg-info/requires.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       14 2023-05-12 18:59:48.000000 Flask-WebTest-0.1.3/Flask_WebTest.egg-info/top_level.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1459 2022-08-16 18:00:53.000000 Flask-WebTest-0.1.3/LICENSE
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      803 2023-05-12 18:59:49.135525 Flask-WebTest-0.1.3/PKG-INFO
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      783 2023-03-02 13:34:53.000000 Flask-WebTest-0.1.3/README.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    11894 2023-05-12 18:56:07.000000 Flask-WebTest-0.1.3/flask_webtest.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       67 2023-05-12 18:59:49.135525 Flask-WebTest-0.1.3/setup.cfg
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1341 2023-03-02 13:42:43.000000 Flask-WebTest-0.1.3/setup.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 18:59:49.127525 Flask-WebTest-0.1.3/tests/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2022-08-16 18:00:53.000000 Flask-WebTest-0.1.3/tests/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      680 2023-05-12 16:27:27.000000 Flask-WebTest-0.1.3/tests/core.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1102 2023-03-02 13:34:53.000000 Flask-WebTest-0.1.3/tests/core_sqlalchemy.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4074 2023-05-12 16:25:42.000000 Flask-WebTest-0.1.3/tests/test.py
```

### Comparing `Flask-WebTest-0.1.2/Flask_WebTest.egg-info/PKG-INFO` & `Flask-WebTest-0.1.3/Flask_WebTest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-WebTest
-Version: 0.1.2
+Version: 0.1.3
 Summary: Utilities for testing Flask applications with WebTest.
 Home-page: https://github.com/level12/flask-webtest
 Author: Anton Romanovich
 Author-email: anthony.romanovich@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Testing
```

### Comparing `Flask-WebTest-0.1.2/LICENSE` & `Flask-WebTest-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-WebTest-0.1.2/PKG-INFO` & `Flask-WebTest-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-WebTest
-Version: 0.1.2
+Version: 0.1.3
 Summary: Utilities for testing Flask applications with WebTest.
 Home-page: https://github.com/level12/flask-webtest
 Author: Anton Romanovich
 Author-email: anthony.romanovich@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Testing
```

### Comparing `Flask-WebTest-0.1.2/README.rst` & `Flask-WebTest-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-WebTest-0.1.2/flask_webtest.py` & `Flask-WebTest-0.1.3/flask_webtest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 from http import cookiejar
 from copy import copy
 from functools import partial
 from contextlib import contextmanager, nullcontext
 
 from werkzeug.local import LocalStack
-from flask import g, session, get_flashed_messages
+from flask import g, session, get_flashed_messages, __version__ as flask_version
 from flask.signals import template_rendered, request_started, request_finished
 from webtest import (TestApp as BaseTestApp,
                      TestRequest as BaseTestRequest,
                      TestResponse as BaseTestResponse)
 
 try:
     import flask_sqlalchemy
@@ -251,15 +251,16 @@
 
         Do some basic translation here for any cookies set in a session transaction.
         """
         if domain == 'localhost':
             # Domain does not matter much here, but the cookiejar policy will block
             # local domains that are not .local
             domain = 'local'
-        if not domain.startswith('.'):
+        if flask_version.startswith('2.2.') and not domain.startswith('.'):
+            # Flask 2.3 dropped the leading dot for cookie domains
             domain = f'.{domain}'
         cookie = cookiejar.Cookie(
             version=0,
             name=name,
             value=value,
             port=None,
             port_specified=False,
```

### Comparing `Flask-WebTest-0.1.2/setup.py` & `Flask-WebTest-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `Flask-WebTest-0.1.2/tests/core.py` & `Flask-WebTest-0.1.3/tests/core.py`

 * *Files identical despite different names*

### Comparing `Flask-WebTest-0.1.2/tests/core_sqlalchemy.py` & `Flask-WebTest-0.1.3/tests/core_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `Flask-WebTest-0.1.2/tests/test.py` & `Flask-WebTest-0.1.3/tests/test.py`

 * *Files identical despite different names*


# Comparing `tmp/Flask-WebTest-0.1.1.tar.gz` & `tmp/Flask-WebTest-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-WebTest-0.1.1.tar", last modified: Thu Mar  2 13:43:54 2023, max compression
+gzip compressed data, was "Flask-WebTest-0.1.2.tar", last modified: Fri May 12 18:02:34 2023, max compression
```

## Comparing `Flask-WebTest-0.1.1.tar` & `Flask-WebTest-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-02 13:43:54.637040 Flask-WebTest-0.1.1/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-02 13:43:54.625040 Flask-WebTest-0.1.1/Flask_WebTest.egg-info/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      803 2023-03-02 13:43:54.000000 Flask-WebTest-0.1.1/Flask_WebTest.egg-info/PKG-INFO
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      345 2023-03-02 13:43:54.000000 Flask-WebTest-0.1.1/Flask_WebTest.egg-info/SOURCES.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2023-03-02 13:43:54.000000 Flask-WebTest-0.1.1/Flask_WebTest.egg-info/dependency_links.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2022-08-16 18:02:52.000000 Flask-WebTest-0.1.1/Flask_WebTest.egg-info/not-zip-safe
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       55 2023-03-02 13:43:54.000000 Flask-WebTest-0.1.1/Flask_WebTest.egg-info/requires.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       14 2023-03-02 13:43:54.000000 Flask-WebTest-0.1.1/Flask_WebTest.egg-info/top_level.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1459 2022-08-16 18:00:53.000000 Flask-WebTest-0.1.1/LICENSE
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      803 2023-03-02 13:43:54.637040 Flask-WebTest-0.1.1/PKG-INFO
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      783 2023-03-02 13:34:53.000000 Flask-WebTest-0.1.1/README.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    10012 2023-03-02 13:34:53.000000 Flask-WebTest-0.1.1/flask_webtest.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       67 2023-03-02 13:43:54.637040 Flask-WebTest-0.1.1/setup.cfg
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1341 2023-03-02 13:42:43.000000 Flask-WebTest-0.1.1/setup.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-02 13:43:54.625040 Flask-WebTest-0.1.1/tests/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2022-08-16 18:00:53.000000 Flask-WebTest-0.1.1/tests/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      680 2022-08-16 18:00:53.000000 Flask-WebTest-0.1.1/tests/core.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1102 2023-03-02 13:34:53.000000 Flask-WebTest-0.1.1/tests/core_sqlalchemy.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4074 2023-03-02 13:34:53.000000 Flask-WebTest-0.1.1/tests/test.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 18:02:34.967770 Flask-WebTest-0.1.2/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 18:02:34.967770 Flask-WebTest-0.1.2/Flask_WebTest.egg-info/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      803 2023-05-12 18:02:34.000000 Flask-WebTest-0.1.2/Flask_WebTest.egg-info/PKG-INFO
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      345 2023-05-12 18:02:34.000000 Flask-WebTest-0.1.2/Flask_WebTest.egg-info/SOURCES.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2023-05-12 18:02:34.000000 Flask-WebTest-0.1.2/Flask_WebTest.egg-info/dependency_links.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2022-08-16 18:02:52.000000 Flask-WebTest-0.1.2/Flask_WebTest.egg-info/not-zip-safe
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       55 2023-05-12 18:02:34.000000 Flask-WebTest-0.1.2/Flask_WebTest.egg-info/requires.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       14 2023-05-12 18:02:34.000000 Flask-WebTest-0.1.2/Flask_WebTest.egg-info/top_level.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1459 2022-08-16 18:00:53.000000 Flask-WebTest-0.1.2/LICENSE
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      803 2023-05-12 18:02:34.967770 Flask-WebTest-0.1.2/PKG-INFO
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      783 2023-03-02 13:34:53.000000 Flask-WebTest-0.1.2/README.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    11760 2023-05-12 18:01:09.000000 Flask-WebTest-0.1.2/flask_webtest.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       67 2023-05-12 18:02:34.967770 Flask-WebTest-0.1.2/setup.cfg
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1341 2023-03-02 13:42:43.000000 Flask-WebTest-0.1.2/setup.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 18:02:34.967770 Flask-WebTest-0.1.2/tests/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2022-08-16 18:00:53.000000 Flask-WebTest-0.1.2/tests/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      680 2023-05-12 16:27:27.000000 Flask-WebTest-0.1.2/tests/core.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1102 2023-03-02 13:34:53.000000 Flask-WebTest-0.1.2/tests/core_sqlalchemy.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4074 2023-05-12 16:25:42.000000 Flask-WebTest-0.1.2/tests/test.py
```

### Comparing `Flask-WebTest-0.1.1/Flask_WebTest.egg-info/PKG-INFO` & `Flask-WebTest-0.1.2/Flask_WebTest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-WebTest
-Version: 0.1.1
+Version: 0.1.2
 Summary: Utilities for testing Flask applications with WebTest.
 Home-page: https://github.com/level12/flask-webtest
 Author: Anton Romanovich
 Author-email: anthony.romanovich@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Testing
```

### Comparing `Flask-WebTest-0.1.1/LICENSE` & `Flask-WebTest-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-WebTest-0.1.1/PKG-INFO` & `Flask-WebTest-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-WebTest
-Version: 0.1.1
+Version: 0.1.2
 Summary: Utilities for testing Flask applications with WebTest.
 Home-page: https://github.com/level12/flask-webtest
 Author: Anton Romanovich
 Author-email: anthony.romanovich@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Testing
```

### Comparing `Flask-WebTest-0.1.1/README.rst` & `Flask-WebTest-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-WebTest-0.1.1/flask_webtest.py` & `Flask-WebTest-0.1.2/flask_webtest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 # coding: utf-8
-try:
-    from http import cookiejar
-except ImportError:
-    import cookielib as cookiejar
+from http import cookiejar
 from copy import copy
 from functools import partial
 from contextlib import contextmanager, nullcontext
 
 from werkzeug.local import LocalStack
 from flask import g, session, get_flashed_messages
 from flask.signals import template_rendered, request_started, request_finished
@@ -242,14 +239,48 @@
                 message_flashed.disconnect(store_flashed_message)
 
         response.session = store.get('session', {})
         response.flashes = store.get('flashes', [])
         response.contexts = dict(store.get('contexts', []))
         return response
 
+    def set_werkzeug_cookie(self, name, value, domain, path):
+        """
+        As of Werkzeug 2.3.0, cookie implementation was refactored, and cookies
+        no longer have the same footprint as http.cookiejar.Cookie. But, webtest
+        expects the http-lib cookies to set up the test request.
+
+        Do some basic translation here for any cookies set in a session transaction.
+        """
+        if domain == 'localhost':
+            # Domain does not matter much here, but the cookiejar policy will block
+            # local domains that are not .local
+            domain = 'local'
+        if not domain.startswith('.'):
+            domain = f'.{domain}'
+        cookie = cookiejar.Cookie(
+            version=0,
+            name=name,
+            value=value,
+            port=None,
+            port_specified=False,
+            domain=domain,
+            domain_specified=True,
+            domain_initial_dot=False,
+            path=path,
+            path_specified=True,
+            secure=False,
+            expires=None,
+            discard=False,
+            comment=None,
+            comment_url=None,
+            rest=None
+        )
+        self.cookiejar.set_cookie(cookie)
+
     @contextmanager
     def session_transaction(self):
         """When used in combination with a with statement this opens
         a session transaction. This can be used to modify the session
         that the test client uses. Once the with block is left the session
         is stored back.
 
@@ -258,20 +289,34 @@
 
             with client.session_transaction() as sess:
                 sess['user_id'] = 1
 
         Internally it uses :meth:`flask.testing.FlaskClient.session_transaction`.
         """
         with self.app.test_client() as client:
+            translate_werkzeug_cookie = hasattr(client, 'get_cookie')
+
             for cookie in self.cookiejar:
-                client.cookie_jar.set_cookie(cookie)
+                if translate_werkzeug_cookie:
+                    client.set_cookie(
+                        cookie.name,
+                        value=cookie.value,
+                        domain=cookie.domain,
+                        path=cookie.path,
+                    )
+                else:
+                    client.cookie_jar.set_cookie(cookie)
 
             with client.session_transaction() as sess:
                 yield sess
 
-            for cookie in client.cookie_jar:
-                # Cookies from `client.cookie_jar` may contain unicode name
-                # and value. It would make WebTest linter (:mod:`webtest.lint`)
-                # throw assertion errors about unicode environmental
-                # variable (HTTP_COOKIE), but we use custom CookieJar that is
-                # aware of this oddity and always sets 8-bit headers.
-                self.cookiejar.set_cookie(cookie)
+            if translate_werkzeug_cookie:
+                for cookie in client._cookies.values():
+                    self.set_werkzeug_cookie(cookie.key, cookie.value, cookie.domain, cookie.path)
+            else:
+                for cookie in client.cookie_jar:
+                    # Cookies from `client.cookie_jar` may contain unicode name
+                    # and value. It would make WebTest linter (:mod:`webtest.lint`)
+                    # throw assertion errors about unicode environmental
+                    # variable (HTTP_COOKIE), but we use custom CookieJar that is
+                    # aware of this oddity and always sets 8-bit headers.
+                    self.cookiejar.set_cookie(cookie)
```

### Comparing `Flask-WebTest-0.1.1/setup.py` & `Flask-WebTest-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `Flask-WebTest-0.1.1/tests/core.py` & `Flask-WebTest-0.1.2/tests/core.py`

 * *Files identical despite different names*

### Comparing `Flask-WebTest-0.1.1/tests/core_sqlalchemy.py` & `Flask-WebTest-0.1.2/tests/core_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `Flask-WebTest-0.1.1/tests/test.py` & `Flask-WebTest-0.1.2/tests/test.py`

 * *Files identical despite different names*


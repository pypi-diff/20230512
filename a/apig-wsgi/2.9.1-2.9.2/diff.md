# Comparing `tmp/apig-wsgi-2.9.1.tar.gz` & `tmp/apig-wsgi-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/chainz/Documents/Projects/apig-wsgi/dist/tmp9v9207ly/apig-wsgi-2.9.1.tar", last modified: Tue Oct 13 09:12:31 2020, max compression
+gzip compressed data, was "/Users/chainz/Documents/Projects/apig-wsgi/dist/tmpaywnu0to/apig-wsgi-2.9.2.tar", last modified: Fri Oct 16 11:27:19 2020, max compression
```

## Comparing `apig-wsgi-2.9.1.tar` & `apig-wsgi-2.9.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-10-13 09:12:31.363819 apig-wsgi-2.9.1/
--rw-r--r--   0 chainz     (501) staff       (20)     5809 2020-10-13 09:12:14.000000 apig-wsgi-2.9.1/HISTORY.rst
--rw-r--r--   0 chainz     (501) staff       (20)     1074 2020-09-21 19:14:47.000000 apig-wsgi-2.9.1/LICENSE
--rw-r--r--   0 chainz     (501) staff       (20)      255 2020-07-22 13:22:10.000000 apig-wsgi-2.9.1/MANIFEST.in
--rw-r--r--   0 chainz     (501) staff       (20)     6972 2020-10-13 09:12:31.364029 apig-wsgi-2.9.1/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)     4888 2020-10-12 16:26:22.000000 apig-wsgi-2.9.1/README.rst
--rw-r--r--   0 chainz     (501) staff       (20)      172 2020-07-24 17:47:17.000000 apig-wsgi-2.9.1/pyproject.toml
--rw-r--r--   0 chainz     (501) staff       (20)     1282 2020-10-13 09:12:31.364851 apig-wsgi-2.9.1/setup.cfg
--rw-r--r--   0 chainz     (501) staff       (20)       38 2020-07-11 12:16:51.000000 apig-wsgi-2.9.1/setup.py
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-10-13 09:12:31.360158 apig-wsgi-2.9.1/src/
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-10-13 09:12:31.361811 apig-wsgi-2.9.1/src/apig_wsgi.egg-info/
--rw-r--r--   0 chainz     (501) staff       (20)     6972 2020-10-13 09:12:31.000000 apig-wsgi-2.9.1/src/apig_wsgi.egg-info/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)      362 2020-10-13 09:12:31.000000 apig-wsgi-2.9.1/src/apig_wsgi.egg-info/SOURCES.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2020-10-13 09:12:31.000000 apig-wsgi-2.9.1/src/apig_wsgi.egg-info/dependency_links.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2020-10-13 09:12:31.000000 apig-wsgi-2.9.1/src/apig_wsgi.egg-info/not-zip-safe
--rw-r--r--   0 chainz     (501) staff       (20)       10 2020-10-13 09:12:31.000000 apig-wsgi-2.9.1/src/apig_wsgi.egg-info/top_level.txt
--rw-r--r--   0 chainz     (501) staff       (20)    10242 2020-10-13 09:10:12.000000 apig-wsgi-2.9.1/src/apig_wsgi.py
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-10-13 09:12:31.362187 apig-wsgi-2.9.1/tests/
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-10-13 09:12:31.362959 apig-wsgi-2.9.1/tests/__pycache__/
--rw-r--r--   0 chainz     (501) staff       (20)    30526 2020-10-12 22:53:42.000000 apig-wsgi-2.9.1/tests/__pycache__/test_apig_wsgi.cpython-39-pytest-6.1.1.pyc
--rw-r--r--   0 chainz     (501) staff       (20)    25933 2020-10-13 09:10:12.000000 apig-wsgi-2.9.1/tests/test_apig_wsgi.py
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-10-16 11:27:19.854272 apig-wsgi-2.9.2/
+-rw-r--r--   0 chainz     (501) staff       (20)     6105 2020-10-16 11:26:51.000000 apig-wsgi-2.9.2/HISTORY.rst
+-rw-r--r--   0 chainz     (501) staff       (20)     1074 2020-09-21 19:14:47.000000 apig-wsgi-2.9.2/LICENSE
+-rw-r--r--   0 chainz     (501) staff       (20)      255 2020-07-22 13:22:10.000000 apig-wsgi-2.9.2/MANIFEST.in
+-rw-r--r--   0 chainz     (501) staff       (20)     6972 2020-10-16 11:27:19.854463 apig-wsgi-2.9.2/PKG-INFO
+-rw-r--r--   0 chainz     (501) staff       (20)     4888 2020-10-12 16:26:22.000000 apig-wsgi-2.9.2/README.rst
+-rw-r--r--   0 chainz     (501) staff       (20)      172 2020-07-24 17:47:17.000000 apig-wsgi-2.9.2/pyproject.toml
+-rw-r--r--   0 chainz     (501) staff       (20)     1282 2020-10-16 11:27:19.855165 apig-wsgi-2.9.2/setup.cfg
+-rw-r--r--   0 chainz     (501) staff       (20)       38 2020-07-11 12:16:51.000000 apig-wsgi-2.9.2/setup.py
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-10-16 11:27:19.851313 apig-wsgi-2.9.2/src/
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-10-16 11:27:19.852642 apig-wsgi-2.9.2/src/apig_wsgi.egg-info/
+-rw-r--r--   0 chainz     (501) staff       (20)     6972 2020-10-16 11:27:19.000000 apig-wsgi-2.9.2/src/apig_wsgi.egg-info/PKG-INFO
+-rw-r--r--   0 chainz     (501) staff       (20)      362 2020-10-16 11:27:19.000000 apig-wsgi-2.9.2/src/apig_wsgi.egg-info/SOURCES.txt
+-rw-r--r--   0 chainz     (501) staff       (20)        1 2020-10-16 11:27:19.000000 apig-wsgi-2.9.2/src/apig_wsgi.egg-info/dependency_links.txt
+-rw-r--r--   0 chainz     (501) staff       (20)        1 2020-10-16 11:27:19.000000 apig-wsgi-2.9.2/src/apig_wsgi.egg-info/not-zip-safe
+-rw-r--r--   0 chainz     (501) staff       (20)       10 2020-10-16 11:27:19.000000 apig-wsgi-2.9.2/src/apig_wsgi.egg-info/top_level.txt
+-rw-r--r--   0 chainz     (501) staff       (20)    10347 2020-10-16 11:24:28.000000 apig-wsgi-2.9.2/src/apig_wsgi.py
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-10-16 11:27:19.852912 apig-wsgi-2.9.2/tests/
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-10-16 11:27:19.853454 apig-wsgi-2.9.2/tests/__pycache__/
+-rw-r--r--   0 chainz     (501) staff       (20)    30526 2020-10-12 22:53:42.000000 apig-wsgi-2.9.2/tests/__pycache__/test_apig_wsgi.cpython-39-pytest-6.1.1.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)    26387 2020-10-16 11:24:28.000000 apig-wsgi-2.9.2/tests/test_apig_wsgi.py
```

### Comparing `apig-wsgi-2.9.1/HISTORY.rst` & `apig-wsgi-2.9.2/HISTORY.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =======
 History
 =======
 
+2.9.2 (2020-10-16)
+------------------
+
+* Unquote paths, as per the WSGI specification. This fixes a bug where paths
+  like ``/api/path%2Finfo"`` were not correctly received by the application as
+  ``/api/path/info"``
+  (`Pull Request #188 <https://github.com/adamchainz/apig-wsgi/pull/188>`__).
+
 2.9.1 (2020-10-13)
 ------------------
 
 * Support Python 3.9.
 * Fix query string parameter encoding so that symbols are correctly re-encoded
   for WSGI, for API Gateway format version 1
   (`Issue #186 <https://github.com/adamchainz/apig-wsgi/pull/186>`__).
```

### Comparing `apig-wsgi-2.9.1/LICENSE` & `apig-wsgi-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apig-wsgi-2.9.1/PKG-INFO` & `apig-wsgi-2.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apig-wsgi
-Version: 2.9.1
+Version: 2.9.2
 Summary: Wrap a WSGI application in an AWS Lambda handler function for running on API Gateway or an ALB.
 Home-page: https://github.com/adamchainz/apig-wsgi
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT License
 Project-URL: Changelog, https://github.com/adamchainz/apig-wsgi/blob/master/HISTORY.rst
 Project-URL: Twitter, https://twitter.com/adamchainz
```

### Comparing `apig-wsgi-2.9.1/README.rst` & `apig-wsgi-2.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `apig-wsgi-2.9.1/setup.cfg` & `apig-wsgi-2.9.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = apig-wsgi
-version = 2.9.1
+version = 2.9.2
 description = Wrap a WSGI application in an AWS Lambda handler function for running on API Gateway or an ALB.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Adam Johnson
 author_email = me@adamj.eu
 url = https://github.com/adamchainz/apig-wsgi
 project_urls =
```

### Comparing `apig-wsgi-2.9.1/src/apig_wsgi.egg-info/PKG-INFO` & `apig-wsgi-2.9.2/src/apig_wsgi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apig-wsgi
-Version: 2.9.1
+Version: 2.9.2
 Summary: Wrap a WSGI application in an AWS Lambda handler function for running on API Gateway or an ALB.
 Home-page: https://github.com/adamchainz/apig-wsgi
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT License
 Project-URL: Changelog, https://github.com/adamchainz/apig-wsgi/blob/master/HISTORY.rst
 Project-URL: Twitter, https://twitter.com/adamchainz
```

### Comparing `apig-wsgi-2.9.1/src/apig_wsgi.py` & `apig-wsgi-2.9.2/src/apig_wsgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sys
+import urllib
 from base64 import b64decode, b64encode
 from collections import defaultdict
 from io import BytesIO
 from urllib.parse import urlencode
 
 __all__ = ("make_lambda_handler",)
 
@@ -65,15 +66,15 @@
 
 
 def get_environ_v1(event, context, binary_support):
     body = get_body(event)
     environ = {
         "CONTENT_LENGTH": str(len(body)),
         "HTTP": "on",
-        "PATH_INFO": event["path"],
+        "PATH_INFO": urllib.parse.unquote(event["path"], encoding="iso-8859-1"),
         "REMOTE_ADDR": "127.0.0.1",
         "REQUEST_METHOD": event["httpMethod"],
         "SCRIPT_NAME": "",
         "SERVER_PROTOCOL": "HTTP/1.1",
         "SERVER_NAME": "",
         "SERVER_PORT": "",
         "wsgi.errors": sys.stderr,
@@ -130,19 +131,20 @@
     return environ
 
 
 def get_environ_v2(event, context, binary_support):
     body = get_body(event)
     headers = event["headers"]
     http = event["requestContext"]["http"]
+
     environ = {
         "CONTENT_LENGTH": str(len(body)),
         "HTTP": "on",
         "HTTP_COOKIE": ";".join(event.get("cookies", ())),
-        "PATH_INFO": http["path"],
+        "PATH_INFO": urllib.parse.unquote(http["path"], encoding="iso-8859-1"),
         "QUERY_STRING": event["rawQueryString"],
         "REMOTE_ADDR": http["sourceIp"],
         "REQUEST_METHOD": http["method"],
         "SCRIPT_NAME": "",
         "SERVER_NAME": "",
         "SERVER_PORT": "",
         "SERVER_PROTOCOL": http["protocol"],
```

### Comparing `apig-wsgi-2.9.1/tests/__pycache__/test_apig_wsgi.cpython-39-pytest-6.1.1.pyc` & `apig-wsgi-2.9.2/tests/__pycache__/test_apig_wsgi.cpython-39-pytest-6.1.1.pyc`

 * *Files identical despite different names*

### Comparing `apig-wsgi-2.9.1/tests/test_apig_wsgi.py` & `apig-wsgi-2.9.2/tests/test_apig_wsgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,29 +64,30 @@
 
 # v1 tests
 
 
 def make_v1_event(
     *,
     method="GET",
+    path="/",
     qs_params=None,
     qs_params_multi=True,
     headers=None,
     headers_multi=True,
     body="",
     binary=False,
     request_context=None
 ):
     if headers is None:
         headers = {"Host": ["example.com"]}
 
     event = {
         "version": "1.0",
         "httpMethod": method,
-        "path": "/",
+        "path": path,
     }
 
     if qs_params_multi:
         event["multiValueQueryStringParameters"] = qs_params
     else:
         if qs_params is None:
             event["queryStringParameters"] = None
@@ -282,14 +283,21 @@
         assert response == {
             "statusCode": 200,
             "multiValueHeaders": {"Content-Type": ["text/plain"]},
             "isBase64Encoded": False,
             "body": "Hello World\n",
         }
 
+    def test_path_unquoting(self, simple_app):
+        event = make_v1_event(path="/api/path%2Finfo")
+
+        simple_app.handler(event, None)
+
+        assert simple_app.environ["PATH_INFO"] == "/api/path/info"
+
     def test_querystring_none(self, simple_app):
         event = make_v1_event()
 
         simple_app.handler(event, None)
 
         assert simple_app.environ["QUERY_STRING"] == ""
 
@@ -521,14 +529,15 @@
 # v2 tests
 
 
 def make_v2_event(
     *,
     host="example.com",
     method="GET",
+    path="/",
     query_string=None,
     cookies=None,
     headers=None,
     body="",
     binary=False
 ):
     if cookies is None:
@@ -540,15 +549,15 @@
         "version": "2.0",
         "rawQueryString": query_string,
         "headers": headers,
         "cookies": cookies,
         "requestContext": {
             "http": {
                 "method": method,
-                "path": "/",
+                "path": path,
                 "sourceIp": "1.2.3.4",
                 "protocol": "https",
             },
         },
     }
 
     if binary:
@@ -769,14 +778,21 @@
         assert simple_app.environ["SERVER_NAME"] == "example.com"
         assert simple_app.environ["HTTP_HOST"] == "example.com"
         assert simple_app.environ["wsgi.url_scheme"] == "https"
         assert simple_app.environ["HTTP_X_FORWARDED_PROTO"] == "https"
         assert simple_app.environ["SERVER_PORT"] == "123"
         assert simple_app.environ["HTTP_X_FORWARDED_PORT"] == "123"
 
+    def test_path_unquoting(self, simple_app):
+        event = make_v2_event(path="/api/path%2Finfo")
+
+        simple_app.handler(event, None)
+
+        assert simple_app.environ["PATH_INFO"] == "/api/path/info"
+
 
 # unknown version test
 
 
 class TestUnknownVersionEvents:
     def test_errors(self, simple_app):
         with pytest.raises(ValueError) as excinfo:
```


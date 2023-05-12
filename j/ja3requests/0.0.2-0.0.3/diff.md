# Comparing `tmp/ja3requests-0.0.2.tar.gz` & `tmp/ja3requests-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ja3requests-0.0.2.tar", last modified: Thu May 11 09:20:12 2023, max compression
+gzip compressed data, was "ja3requests-0.0.3.tar", last modified: Fri May 12 09:34:27 2023, max compression
```

## Comparing `ja3requests-0.0.2.tar` & `ja3requests-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 pledgebox   (501) staff       (20)        0 2023-05-11 09:20:12.957403 ja3requests-0.0.2/
--rw-r--r--   0 pledgebox   (501) staff       (20)    11357 2023-04-25 06:02:38.000000 ja3requests-0.0.2/LICENSE
--rw-r--r--   0 pledgebox   (501) staff       (20)      444 2023-05-11 09:20:12.957089 ja3requests-0.0.2/PKG-INFO
--rw-r--r--   0 pledgebox   (501) staff       (20)       75 2023-04-25 06:02:38.000000 ja3requests-0.0.2/README.md
-drwxr-xr-x   0 pledgebox   (501) staff       (20)        0 2023-05-11 09:20:12.952049 ja3requests-0.0.2/ja3requests/
--rw-r--r--   0 pledgebox   (501) staff       (20)        0 2023-04-26 10:28:27.000000 ja3requests-0.0.2/ja3requests/__init__.py
--rw-r--r--   0 pledgebox   (501) staff       (20)      395 2023-05-11 09:18:32.000000 ja3requests-0.0.2/ja3requests/__version__.py
--rw-r--r--   0 pledgebox   (501) staff       (20)     3298 2023-05-11 09:18:14.000000 ja3requests-0.0.2/ja3requests/connections.py
--rw-r--r--   0 pledgebox   (501) staff       (20)      665 2023-04-26 10:28:27.000000 ja3requests-0.0.2/ja3requests/const.py
--rw-r--r--   0 pledgebox   (501) staff       (20)     1184 2023-05-11 09:18:14.000000 ja3requests-0.0.2/ja3requests/exceptions.py
--rw-r--r--   0 pledgebox   (501) staff       (20)     5848 2023-05-11 09:18:14.000000 ja3requests-0.0.2/ja3requests/request.py
--rw-r--r--   0 pledgebox   (501) staff       (20)     4537 2023-05-11 09:18:14.000000 ja3requests-0.0.2/ja3requests/sessions.py
--rw-r--r--   0 pledgebox   (501) staff       (20)     2118 2023-04-26 10:28:27.000000 ja3requests-0.0.2/ja3requests/utils.py
-drwxr-xr-x   0 pledgebox   (501) staff       (20)        0 2023-05-11 09:20:12.954583 ja3requests-0.0.2/ja3requests.egg-info/
--rw-r--r--   0 pledgebox   (501) staff       (20)      444 2023-05-11 09:20:12.000000 ja3requests-0.0.2/ja3requests.egg-info/PKG-INFO
--rw-r--r--   0 pledgebox   (501) staff       (20)      475 2023-05-11 09:20:12.000000 ja3requests-0.0.2/ja3requests.egg-info/SOURCES.txt
--rw-r--r--   0 pledgebox   (501) staff       (20)        1 2023-05-11 09:20:12.000000 ja3requests-0.0.2/ja3requests.egg-info/dependency_links.txt
--rw-r--r--   0 pledgebox   (501) staff       (20)        1 2023-05-11 09:20:12.000000 ja3requests-0.0.2/ja3requests.egg-info/not-zip-safe
--rw-r--r--   0 pledgebox   (501) staff       (20)       12 2023-05-11 09:20:12.000000 ja3requests-0.0.2/ja3requests.egg-info/top_level.txt
--rw-r--r--   0 pledgebox   (501) staff       (20)      640 2023-04-26 10:28:27.000000 ja3requests-0.0.2/pyproject.toml
--rw-r--r--   0 pledgebox   (501) staff       (20)       38 2023-05-11 09:20:12.957490 ja3requests-0.0.2/setup.cfg
--rw-r--r--   0 pledgebox   (501) staff       (20)     1890 2023-04-26 10:28:27.000000 ja3requests-0.0.2/setup.py
-drwxr-xr-x   0 pledgebox   (501) staff       (20)        0 2023-05-11 09:20:12.956283 ja3requests-0.0.2/test/
--rw-r--r--   0 pledgebox   (501) staff       (20)      431 2023-05-11 09:18:14.000000 ja3requests-0.0.2/test/test_ready_request.py
--rw-r--r--   0 pledgebox   (501) staff       (20)      248 2023-05-11 09:18:14.000000 ja3requests-0.0.2/test/test_session.py
--rw-r--r--   0 pledgebox   (501) staff       (20)      244 2023-04-26 10:28:27.000000 ja3requests-0.0.2/test/test_utils.py
+drwxr-xr-x   0 pledgebox   (501) staff       (20)        0 2023-05-12 09:34:27.260316 ja3requests-0.0.3/
+-rw-r--r--   0 pledgebox   (501) staff       (20)    11357 2023-04-25 06:02:38.000000 ja3requests-0.0.3/LICENSE
+-rw-r--r--   0 pledgebox   (501) staff       (20)      444 2023-05-12 09:34:27.259991 ja3requests-0.0.3/PKG-INFO
+-rw-r--r--   0 pledgebox   (501) staff       (20)       75 2023-04-25 06:02:38.000000 ja3requests-0.0.3/README.md
+drwxr-xr-x   0 pledgebox   (501) staff       (20)        0 2023-05-12 09:34:27.256071 ja3requests-0.0.3/ja3requests/
+-rw-r--r--   0 pledgebox   (501) staff       (20)        0 2023-04-26 10:28:27.000000 ja3requests-0.0.3/ja3requests/__init__.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)      395 2023-05-12 09:33:43.000000 ja3requests-0.0.3/ja3requests/__version__.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)     4320 2023-05-12 09:33:31.000000 ja3requests-0.0.3/ja3requests/connections.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)      665 2023-04-26 10:28:27.000000 ja3requests-0.0.3/ja3requests/const.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)     1223 2023-05-12 09:33:31.000000 ja3requests-0.0.3/ja3requests/context.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)     1537 2023-05-12 09:33:31.000000 ja3requests-0.0.3/ja3requests/exceptions.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)     6651 2023-05-12 09:33:31.000000 ja3requests-0.0.3/ja3requests/request.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)     3176 2023-05-12 09:33:31.000000 ja3requests-0.0.3/ja3requests/response.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)     4596 2023-05-12 09:33:31.000000 ja3requests-0.0.3/ja3requests/sessions.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)     2118 2023-05-12 09:33:31.000000 ja3requests-0.0.3/ja3requests/utils.py
+drwxr-xr-x   0 pledgebox   (501) staff       (20)        0 2023-05-12 09:34:27.257839 ja3requests-0.0.3/ja3requests.egg-info/
+-rw-r--r--   0 pledgebox   (501) staff       (20)      444 2023-05-12 09:34:27.000000 ja3requests-0.0.3/ja3requests.egg-info/PKG-INFO
+-rw-r--r--   0 pledgebox   (501) staff       (20)      522 2023-05-12 09:34:27.000000 ja3requests-0.0.3/ja3requests.egg-info/SOURCES.txt
+-rw-r--r--   0 pledgebox   (501) staff       (20)        1 2023-05-12 09:34:27.000000 ja3requests-0.0.3/ja3requests.egg-info/dependency_links.txt
+-rw-r--r--   0 pledgebox   (501) staff       (20)        1 2023-05-12 09:34:27.000000 ja3requests-0.0.3/ja3requests.egg-info/not-zip-safe
+-rw-r--r--   0 pledgebox   (501) staff       (20)       12 2023-05-12 09:34:27.000000 ja3requests-0.0.3/ja3requests.egg-info/top_level.txt
+-rw-r--r--   0 pledgebox   (501) staff       (20)      640 2023-04-26 10:28:27.000000 ja3requests-0.0.3/pyproject.toml
+-rw-r--r--   0 pledgebox   (501) staff       (20)       38 2023-05-12 09:34:27.260406 ja3requests-0.0.3/setup.cfg
+-rw-r--r--   0 pledgebox   (501) staff       (20)     1890 2023-04-26 10:28:27.000000 ja3requests-0.0.3/setup.py
+drwxr-xr-x   0 pledgebox   (501) staff       (20)        0 2023-05-12 09:34:27.259137 ja3requests-0.0.3/test/
+-rw-r--r--   0 pledgebox   (501) staff       (20)      431 2023-05-11 09:18:14.000000 ja3requests-0.0.3/test/test_ready_request.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)      310 2023-05-12 09:33:31.000000 ja3requests-0.0.3/test/test_session.py
+-rw-r--r--   0 pledgebox   (501) staff       (20)      244 2023-04-26 10:28:27.000000 ja3requests-0.0.3/test/test_utils.py
```

### Comparing `ja3requests-0.0.2/LICENSE` & `ja3requests-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ja3requests-0.0.2/ja3requests/const.py` & `ja3requests-0.0.3/ja3requests/const.py`

 * *Files identical despite different names*

### Comparing `ja3requests-0.0.2/ja3requests/exceptions.py` & `ja3requests-0.0.3/ja3requests/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,8 +40,26 @@
     If the scheme not allowed and raise it.
     """
 
 
 class InvalidParams(RequestException, ValueError):
     """
     If request params invalid and raise it.
+    """
+
+
+class InvalidHost(RequestException, ValueError):
+    """
+    Raised it while host can not parse.
+    """
+
+
+class InvalidStatusLine(RequestException, ValueError):
+    """
+    Raised it when can't receive streamline.
+    """
+
+
+class InvalidResponseHeaders(RequestException, ValueError):
+    """
+    Raised it when cant receive response headers.
     """
```

### Comparing `ja3requests-0.0.2/ja3requests/request.py` & `ja3requests-0.0.3/ja3requests/request.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """
 ja3requests.request
 ~~~~~~~~~~~~~~~~~~~
 
 This module create a request struct and ready request object.
 """
 from .base import BaseRequest
+from .utils import default_headers
+from .context import HTTPContext
 from .connections import HTTPConnection
 from .exceptions import NotAllowedRequestMethod, MissingScheme, NotAllowedScheme, InvalidParams
+import warnings
 from http.cookiejar import CookieJar
 from urllib.parse import urlparse, urlencode
 from typing import Any, AnyStr, Dict, List, Union, ByteString, Tuple
 
 
 class ReadyRequest(BaseRequest):
 
@@ -123,18 +126,37 @@
         """
         Todo: Ready form data.
         :return:
         """
 
     def ready_headers(self):
         """
-        Todo: Ready http headers.
+        Ready http headers.
         :return:
         """
 
+        # Default headers
+        if self.headers is None:
+            self.headers = default_headers()
+
+        # Check duplicate default item
+        new_headers = {}
+        header_list = []
+        for k, v in self.headers.items():
+            header = k.lower()
+            if header in header_list:
+                warnings.warn(f"Duplicate header: {k}, you should check the request headers.", RuntimeWarning)
+
+            header_list.append(header)
+            new_headers[header] = v
+
+        self.headers = new_headers
+        del new_headers
+        del header_list
+
     def ready_cookies(self):
         """
         Todo: Ready http cookies.
         :return:
         """
 
     def ready_auth(self):
@@ -195,15 +217,20 @@
             self.source,
             self.url,
             self.timeout,
             proxy,
             proxy_username,
             proxy_password
         )
-        response = conn.send()
+        context = HTTPContext(conn)
+        context.set_payload(
+            method=self.method,
+            headers=self.headers,
+        )
+        response = conn.send(context)
 
         return response
 
     def create_connect(self):
         """
         Create http connection or https connection by request scheme.
         :return:
```

### Comparing `ja3requests-0.0.2/ja3requests/sessions.py` & `ja3requests-0.0.3/ja3requests/sessions.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 ja3Requests.
 """
 import sys
 import time
 from http.cookiejar import CookieJar
 from typing import AnyStr, Any, Dict, ByteString, Union, List, Tuple
 from .base import BaseSession
+from .response import Response
 from .utils import default_headers
 from .const import DEFAULT_REDIRECT_LIMIT
 from .request import ReadyRequest, Request
 
 # Preferred clock, based on which one is more accurate on a given system.
 if sys.platform == "win32":
     preferred_clock = time.perf_counter
@@ -187,10 +188,11 @@
 
     def send(self, request: Request):
         """
         Send request.
         :return:
         """
 
-        response = request.send()
+        rep = request.send()
+        response = Response(rep)
 
         return response
```

### Comparing `ja3requests-0.0.2/ja3requests/utils.py` & `ja3requests-0.0.3/ja3requests/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -57,30 +57,30 @@
             pass
         elif isinstance(accept_encoding, list):
             accept_encoding = ",".join(accept_encoding)
         else:
             accept_encoding = ACCEPT_ENCODING
         headers["Accept-Encoding"] = accept_encoding
 
-    headers["User-Agent"] = user_agent if user_agent else default_user_agent()
-
     if keep_alive:
         headers["Connection"] = "keep-alive"
 
     if basic_auth:
         headers["Authorization"] = "Basic " + b64encode(b(basic_auth)).decode("utf-8")
 
     if proxy_basic_auth:
         headers["Proxy-Authorization"] = "Basic " + b64encode(
             b(proxy_basic_auth)
         ).decode("utf-8")
 
     if disable_cache:
         headers["Cache-Control"] = "no-cache"
 
+    headers["User-Agent"] = user_agent if user_agent else default_user_agent()
+
     return headers
 
 
 def default_headers():
     """
     Return default headers.
     :return:
```

### Comparing `ja3requests-0.0.2/pyproject.toml` & `ja3requests-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ja3requests-0.0.2/setup.py` & `ja3requests-0.0.3/setup.py`

 * *Files identical despite different names*


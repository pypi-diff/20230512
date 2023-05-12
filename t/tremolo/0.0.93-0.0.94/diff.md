# Comparing `tmp/tremolo-0.0.93.tar.gz` & `tmp/tremolo-0.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tremolo-0.0.93.tar", last modified: Fri May 12 00:21:54 2023, max compression
+gzip compressed data, was "dist/tremolo-0.0.94.tar", last modified: Fri May 12 01:23:05 2023, max compression
```

## Comparing `tremolo-0.0.93.tar` & `tremolo-0.0.94.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-12 00:21:54.000000 tremolo-0.0.93/
--rw-r--r--   0 tux       (1000) users      (100)     1063 2023-05-08 03:43:30.000000 tremolo-0.0.93/LICENSE.txt
--rw-r--r--   0 tux       (1000) users      (100)     3743 2023-05-12 00:21:54.000000 tremolo-0.0.93/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)     3143 2023-05-08 03:43:30.000000 tremolo-0.0.93/README.md
--rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-12 00:21:54.000000 tremolo-0.0.93/setup.cfg
--rwxr-xr-x   0 tux       (1000) users      (100)      975 2023-05-12 00:19:17.000000 tremolo-0.0.93/setup.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-12 00:21:54.000000 tremolo-0.0.93/tremolo/
--rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-05-08 03:43:30.000000 tremolo-0.0.93/tremolo/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)     4465 2023-05-08 03:43:30.000000 tremolo-0.0.93/tremolo/__main__.py
--rw-r--r--   0 tux       (1000) users      (100)     2278 2023-05-08 03:43:30.000000 tremolo-0.0.93/tremolo/asgi_lifespan.py
--rw-r--r--   0 tux       (1000) users      (100)     5688 2023-05-12 00:04:33.000000 tremolo-0.0.93/tremolo/asgi_server.py
--rw-r--r--   0 tux       (1000) users      (100)      542 2023-05-08 03:43:30.000000 tremolo-0.0.93/tremolo/contexts.py
--rw-r--r--   0 tux       (1000) users      (100)      586 2023-05-08 03:43:30.000000 tremolo-0.0.93/tremolo/exceptions.py
--rw-r--r--   0 tux       (1000) users      (100)    11243 2023-05-08 03:43:30.000000 tremolo-0.0.93/tremolo/http_server.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-12 00:21:54.000000 tremolo-0.0.93/tremolo/lib/
--rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-08 03:43:30.000000 tremolo-0.0.93/tremolo/lib/__init__.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-12 00:21:54.000000 tremolo-0.0.93/tremolo/lib/h1parser/
--rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-08 03:43:30.000000 tremolo-0.0.93/tremolo/lib/h1parser/__init__.py
--rwxr-xr-x   0 tux       (1000) users      (100)     4954 2023-05-08 03:43:30.000000 tremolo-0.0.93/tremolo/lib/h1parser/parse_header.py
--rw-r--r--   0 tux       (1000) users      (100)     1798 2023-05-08 03:43:30.000000 tremolo-0.0.93/tremolo/lib/http_exception.py
--rwxr-xr-x   0 tux       (1000) users      (100)    13737 2023-05-08 03:43:30.000000 tremolo-0.0.93/tremolo/lib/http_protocol.py
--rwxr-xr-x   0 tux       (1000) users      (100)     9307 2023-05-08 03:43:30.000000 tremolo-0.0.93/tremolo/lib/http_request.py
--rwxr-xr-x   0 tux       (1000) users      (100)    11332 2023-05-11 15:27:21.000000 tremolo-0.0.93/tremolo/lib/http_response.py
--rw-r--r--   0 tux       (1000) users      (100)      844 2023-05-08 03:43:30.000000 tremolo-0.0.93/tremolo/lib/object_pool.py
--rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-05-08 03:43:30.000000 tremolo-0.0.93/tremolo/lib/request.py
--rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-05-08 03:43:30.000000 tremolo-0.0.93/tremolo/lib/response.py
--rwxr-xr-x   0 tux       (1000) users      (100)    15287 2023-05-08 03:43:30.000000 tremolo-0.0.93/tremolo/tremolo.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-12 00:21:54.000000 tremolo-0.0.93/tremolo.egg-info/
--rw-r--r--   0 tux       (1000) users      (100)     3743 2023-05-12 00:21:54.000000 tremolo-0.0.93/tremolo.egg-info/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)      610 2023-05-12 00:21:54.000000 tremolo-0.0.93/tremolo.egg-info/SOURCES.txt
--rw-r--r--   0 tux       (1000) users      (100)        1 2023-05-12 00:21:54.000000 tremolo-0.0.93/tremolo.egg-info/dependency_links.txt
--rw-r--r--   0 tux       (1000) users      (100)        8 2023-05-12 00:21:54.000000 tremolo-0.0.93/tremolo.egg-info/top_level.txt
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-12 01:23:05.000000 tremolo-0.0.94/
+-rw-r--r--   0 tux       (1000) users      (100)     1063 2023-05-08 03:43:30.000000 tremolo-0.0.94/LICENSE.txt
+-rw-r--r--   0 tux       (1000) users      (100)     3743 2023-05-12 01:23:05.000000 tremolo-0.0.94/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)     3143 2023-05-08 03:43:30.000000 tremolo-0.0.94/README.md
+-rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-12 01:23:05.000000 tremolo-0.0.94/setup.cfg
+-rwxr-xr-x   0 tux       (1000) users      (100)      975 2023-05-12 01:20:49.000000 tremolo-0.0.94/setup.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-12 01:23:05.000000 tremolo-0.0.94/tremolo/
+-rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-05-08 03:43:30.000000 tremolo-0.0.94/tremolo/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)     4465 2023-05-08 03:43:30.000000 tremolo-0.0.94/tremolo/__main__.py
+-rw-r--r--   0 tux       (1000) users      (100)     2278 2023-05-08 03:43:30.000000 tremolo-0.0.94/tremolo/asgi_lifespan.py
+-rw-r--r--   0 tux       (1000) users      (100)     5682 2023-05-12 01:17:00.000000 tremolo-0.0.94/tremolo/asgi_server.py
+-rw-r--r--   0 tux       (1000) users      (100)      542 2023-05-08 03:43:30.000000 tremolo-0.0.94/tremolo/contexts.py
+-rw-r--r--   0 tux       (1000) users      (100)      586 2023-05-08 03:43:30.000000 tremolo-0.0.94/tremolo/exceptions.py
+-rw-r--r--   0 tux       (1000) users      (100)    11243 2023-05-08 03:43:30.000000 tremolo-0.0.94/tremolo/http_server.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-12 01:23:05.000000 tremolo-0.0.94/tremolo/lib/
+-rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-08 03:43:30.000000 tremolo-0.0.94/tremolo/lib/__init__.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-12 01:23:05.000000 tremolo-0.0.94/tremolo/lib/h1parser/
+-rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-08 03:43:30.000000 tremolo-0.0.94/tremolo/lib/h1parser/__init__.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     4954 2023-05-08 03:43:30.000000 tremolo-0.0.94/tremolo/lib/h1parser/parse_header.py
+-rw-r--r--   0 tux       (1000) users      (100)     1798 2023-05-08 03:43:30.000000 tremolo-0.0.94/tremolo/lib/http_exception.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    13737 2023-05-08 03:43:30.000000 tremolo-0.0.94/tremolo/lib/http_protocol.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     9307 2023-05-08 03:43:30.000000 tremolo-0.0.94/tremolo/lib/http_request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    11322 2023-05-12 01:18:27.000000 tremolo-0.0.94/tremolo/lib/http_response.py
+-rw-r--r--   0 tux       (1000) users      (100)      844 2023-05-08 03:43:30.000000 tremolo-0.0.94/tremolo/lib/object_pool.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-05-08 03:43:30.000000 tremolo-0.0.94/tremolo/lib/request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-05-08 03:43:30.000000 tremolo-0.0.94/tremolo/lib/response.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    15287 2023-05-08 03:43:30.000000 tremolo-0.0.94/tremolo/tremolo.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-12 01:23:05.000000 tremolo-0.0.94/tremolo.egg-info/
+-rw-r--r--   0 tux       (1000) users      (100)     3743 2023-05-12 01:23:05.000000 tremolo-0.0.94/tremolo.egg-info/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)      610 2023-05-12 01:23:05.000000 tremolo-0.0.94/tremolo.egg-info/SOURCES.txt
+-rw-r--r--   0 tux       (1000) users      (100)        1 2023-05-12 01:23:05.000000 tremolo-0.0.94/tremolo.egg-info/dependency_links.txt
+-rw-r--r--   0 tux       (1000) users      (100)        8 2023-05-12 01:23:05.000000 tremolo-0.0.94/tremolo.egg-info/top_level.txt
```

### Comparing `tremolo-0.0.93/LICENSE.txt` & `tremolo-0.0.94/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.93/PKG-INFO` & `tremolo-0.0.94/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.93
+Version: 0.0.94
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tremolo-0.0.93/README.md` & `tremolo-0.0.94/README.md`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.93/setup.py` & `tremolo-0.0.94/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='tremolo',
     packages=['tremolo'],
     package_data={'': ['lib/*', 'lib/h1parser/*']},
-    version='0.0.93',
+    version='0.0.94',
     license='MIT',
     author='nggit',
     author_email='contact@anggit.com',
     description='Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nggit/tremolo',
```

### Comparing `tremolo-0.0.93/tremolo/__main__.py` & `tremolo-0.0.94/tremolo/__main__.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.93/tremolo/asgi_lifespan.py` & `tremolo-0.0.94/tremolo/asgi_lifespan.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.93/tremolo/asgi_server.py` & `tremolo-0.0.94/tremolo/asgi_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,16 +100,16 @@
                 self._response.set_status(data['status'], HTTPStatus(data['status']).phrase)
                 self._response.append_header(b'Date: %s\r\nServer: %s\r\n' % (
                                              datetime.utcnow().strftime('%a, %d %b %Y %H:%M:%S GMT').encode(encoding='latin-1'),
                                              self.options['server_name']))
 
                 if 'headers' in data:
                     for header in data['headers']:
-                        if not (header[0].find(b'\r\n') == -1 and header[1].find(b'\r\n') == -1):
-                            raise ValueError('name or value cannot contain CRLF characters')
+                        if not (header[0].find(b'\n') == -1 and header[1].find(b'\n') == -1):
+                            raise ValueError('name or value cannot contain LF characters')
 
                         name = header[0].lower()
 
                         if name == b'content-type':
                             self._response.set_content_type(header[1])
                             continue
```

### Comparing `tremolo-0.0.93/tremolo/contexts.py` & `tremolo-0.0.94/tremolo/contexts.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.93/tremolo/exceptions.py` & `tremolo-0.0.94/tremolo/exceptions.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.93/tremolo/http_server.py` & `tremolo-0.0.94/tremolo/http_server.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.93/tremolo/lib/h1parser/parse_header.py` & `tremolo-0.0.94/tremolo/lib/h1parser/parse_header.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.93/tremolo/lib/http_exception.py` & `tremolo-0.0.94/tremolo/lib/http_exception.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.93/tremolo/lib/http_protocol.py` & `tremolo-0.0.94/tremolo/lib/http_protocol.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.93/tremolo/lib/http_request.py` & `tremolo-0.0.94/tremolo/lib/http_request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.93/tremolo/lib/http_response.py` & `tremolo-0.0.94/tremolo/lib/http_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,51 +46,51 @@
             if v:
                 cookie.extend(b'; %s=%s' % (k, bytes(quote(v), encoding='latin-1')))
 
         for k, v in ((secure, b'; secure'), (httponly, b'; httponly')):
             if k:
                 cookie.extend(v)
 
-        if cookie.find(b'\r\n') != -1:
+        if cookie.find(b'\n') != -1:
             raise InternalServerError
 
         self._header[1].extend(cookie + b'\r\n')
 
     def set_header(self, name, value=''):
         if isinstance(name, str):
             name = name.encode(encoding='latin-1')
 
         if isinstance(value, str):
             value = value.encode(encoding='latin-1')
 
-        if not (name.find(b'\r\n') == -1 and value.find(b'\r\n') == -1):
+        if not (name.find(b'\n') == -1 and value.find(b'\n') == -1):
             raise InternalServerError
 
         self._header[1].extend(b'%s: %s\r\n' % (name, value))
 
     def set_status(self, status=200, message=b'OK'):
         if isinstance(message, str):
             message = message.encode(encoding='latin-1')
 
-        if not (isinstance(status, int) and message.find(b'\r\n') == -1):
+        if not (isinstance(status, int) and message.find(b'\n') == -1):
             raise InternalServerError
 
         self._status.append((status, message))
 
     def get_status(self):
         try:
             return self._status.pop()
         except IndexError:
             return 200, b'OK'
 
     def set_content_type(self, content_type=b'text/html; charset=utf-8'):
         if isinstance(content_type, str):
             content_type = content_type.encode(encoding='latin-1')
 
-        if content_type.find(b'\r\n') != -1:
+        if content_type.find(b'\n') != -1:
             raise InternalServerError
 
         self._content_type.append(content_type)
 
     def get_content_type(self):
         try:
             return self._content_type.pop()
```

### Comparing `tremolo-0.0.93/tremolo/lib/object_pool.py` & `tremolo-0.0.94/tremolo/lib/object_pool.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.93/tremolo/lib/request.py` & `tremolo-0.0.94/tremolo/lib/request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.93/tremolo/lib/response.py` & `tremolo-0.0.94/tremolo/lib/response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.93/tremolo/tremolo.py` & `tremolo-0.0.94/tremolo/tremolo.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.93/tremolo.egg-info/PKG-INFO` & `tremolo-0.0.94/tremolo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.93
+Version: 0.0.94
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tremolo-0.0.93/tremolo.egg-info/SOURCES.txt` & `tremolo-0.0.94/tremolo.egg-info/SOURCES.txt`

 * *Files identical despite different names*


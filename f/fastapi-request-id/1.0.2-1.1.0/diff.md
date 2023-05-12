# Comparing `tmp/fastapi_request_id-1.0.2-py3-none-any.whl.zip` & `tmp/fastapi_request_id-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3791 bytes, number of entries: 8
+Zip file size: 3692 bytes, number of entries: 8
 -rw-r--r--  2.0 unx      197 b- defN 80-Jan-01 00:00 fastapi_request_id/__init__.py
--rw-r--r--  2.0 unx      680 b- defN 80-Jan-01 00:00 fastapi_request_id/context.py
--rw-r--r--  2.0 unx      614 b- defN 80-Jan-01 00:00 fastapi_request_id/handlers.py
--rw-r--r--  2.0 unx      265 b- defN 80-Jan-01 00:00 fastapi_request_id/logging.py
--rw-r--r--  2.0 unx      815 b- defN 80-Jan-01 00:00 fastapi_request_id/middleware.py
--rw-r--r--  2.0 unx     2325 b- defN 80-Jan-01 00:00 fastapi_request_id-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fastapi_request_id-1.0.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx      669 b- defN 16-Jan-01 00:00 fastapi_request_id-1.0.2.dist-info/RECORD
-8 files, 5653 bytes uncompressed, 2613 bytes compressed:  53.8%
+-rw-r--r--  2.0 unx      683 b- defN 80-Jan-01 00:00 fastapi_request_id/context.py
+-rw-r--r--  2.0 unx      534 b- defN 80-Jan-01 00:00 fastapi_request_id/handlers.py
+-rw-r--r--  2.0 unx      266 b- defN 80-Jan-01 00:00 fastapi_request_id/logging.py
+-rw-r--r--  2.0 unx      611 b- defN 80-Jan-01 00:00 fastapi_request_id/middleware.py
+-rw-r--r--  2.0 unx     2325 b- defN 80-Jan-01 00:00 fastapi_request_id-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fastapi_request_id-1.1.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx      669 b- defN 16-Jan-01 00:00 fastapi_request_id-1.1.0.dist-info/RECORD
+8 files, 5373 bytes uncompressed, 2514 bytes compressed:  53.2%
```

## zipnote {}

```diff
@@ -9,17 +9,17 @@
 
 Filename: fastapi_request_id/logging.py
 Comment: 
 
 Filename: fastapi_request_id/middleware.py
 Comment: 
 
-Filename: fastapi_request_id-1.0.2.dist-info/METADATA
+Filename: fastapi_request_id-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: fastapi_request_id-1.0.2.dist-info/WHEEL
+Filename: fastapi_request_id-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: fastapi_request_id-1.0.2.dist-info/RECORD
+Filename: fastapi_request_id-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fastapi_request_id/context.py

```diff
@@ -17,13 +17,16 @@
 def reset_request_id(token: Token):
     _request_id_ctx_var.reset(token)
 
 
 def get_headers(headers: dict = None) -> Optional[dict]:
     if headers is None:
         headers = {}
+
     request_id = get_request_id()
 
     if not request_id:
         return None
+
     headers["X-Request-ID"] = request_id
+
     return headers
```

## fastapi_request_id/handlers.py

```diff
@@ -1,22 +1,21 @@
 from abc import ABC, abstractmethod
-from typing import Optional
+from fastapi_request_id import get_request_id
 
 from fastapi import Request, Response
 
 
 class BaseExceptionHandler(ABC):
 
     def __call__(self, request: Request, exc: Exception):
-        request_id = getattr(exc, '__request_id__', None)
-        delattr(exc, '__request_id__')
-        response = self.build_response(request, exc, request_id)
+        request_id = get_request_id()
+        response = self.build_response(request, exc)
 
         if request_id:
             response.headers['X-Request-ID'] = request_id
 
         return response
 
     @staticmethod
     @abstractmethod
-    def build_response(request: Request, exc: Exception, request_id: Optional[str]) -> Response:
+    def build_response(request: Request, exc: Exception) -> Response:
         ...
```

## fastapi_request_id/logging.py

```diff
@@ -1,10 +1,11 @@
 import logging
 from .context import get_request_id
 
 
 class RequestIdFilter(logging.Filter):
     def filter(self, record: logging.LogRecord):
         request_id = get_request_id()
+
         if request_id:
             record.request_id = request_id
         return True
```

## fastapi_request_id/middleware.py

```diff
@@ -1,27 +1,20 @@
 from uuid import uuid4
 from .context import (
     get_request_id,
     set_request_id,
-    reset_request_id,
 )
 from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
 from starlette.requests import Request
 
 
 class RequestContextMiddleware(BaseHTTPMiddleware):
 
     async def dispatch(self, request: Request, call_next: RequestResponseEndpoint):
-        request_token = set_request_id(request.headers.get('X-Request-ID', str(uuid4())))
+        set_request_id(request.headers.get('X-Request-ID', str(uuid4())))
+        response = await call_next(request)
+        request_id = get_request_id()
 
-        try:
-            response = await call_next(request)
-        except Exception as error:
-            setattr(error, '__request_id__', get_request_id())
-            reset_request_id(request_token)
-            raise error
-
-        response.headers['X-Request-ID'] = get_request_id()
-
-        reset_request_id(request_token)
+        if request_id:
+            response.headers['X-Request-ID'] = request_id
 
         return response
```

## Comparing `fastapi_request_id-1.0.2.dist-info/METADATA` & `fastapi_request_id-1.1.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-request-id
-Version: 1.0.2
+Version: 1.1.0
 Summary: 
 Author: Stanislav Tsoy
 Author-email: dev.stanislav@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


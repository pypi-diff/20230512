# Comparing `tmp/asgi_matomo-0.1.4.tar.gz` & `tmp/asgi_matomo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgi_matomo-0.1.4.tar", max compression
+gzip compressed data, was "asgi_matomo-0.2.0.tar", max compression
```

## Comparing `asgi_matomo-0.1.4.tar` & `asgi_matomo-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-04-27 08:08:51.206959 asgi_matomo-0.1.4/LICENSE
--rw-r--r--   0        0        0     2656 2023-04-28 09:27:05.974228 asgi_matomo-0.1.4/README.md
--rw-r--r--   0        0        0       84 2023-04-27 08:57:22.265099 asgi_matomo-0.1.4/asgi_matomo/__init__.py
--rw-r--r--   0        0        0     6776 2023-05-10 08:15:11.684805 asgi_matomo-0.1.4/asgi_matomo/middleware.py
--rw-r--r--   0        0        0      691 2023-05-10 08:15:40.778584 asgi_matomo-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3205 1970-01-01 00:00:00.000000 asgi_matomo-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-27 08:08:51.206959 asgi_matomo-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4066 2023-05-12 12:30:13.375244 asgi_matomo-0.2.0/README.md
+-rw-r--r--   0        0        0       84 2023-04-27 08:57:22.265099 asgi_matomo-0.2.0/asgi_matomo/__init__.py
+-rw-r--r--   0        0        0     8752 2023-05-12 12:34:38.273538 asgi_matomo-0.2.0/asgi_matomo/middleware.py
+-rw-r--r--   0        0        0      879 2023-05-12 12:32:40.621441 asgi_matomo-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4799 1970-01-01 00:00:00.000000 asgi_matomo-0.2.0/PKG-INFO
```

### Comparing `asgi_matomo-0.1.4/LICENSE` & `asgi_matomo-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asgi_matomo-0.1.4/asgi_matomo/middleware.py` & `asgi_matomo-0.2.0/asgi_matomo/middleware.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import json
 import logging
 import random
+import re
 import time
 import traceback
 import typing
 import urllib.parse
 from typing import Any
 
 import httpx
@@ -40,22 +42,28 @@
         app: ASGI3Application,
         *,
         matomo_url,
         idsite: int,
         access_token: str | None = None,
         assume_https: bool = True,
         client: httpx.AsyncClient | None = None,
+        exclude_paths: list[str] | None = None,
+        exclude_patterns: list[str] | None = None,
     ) -> None:
         self.app = app
         self.matomo_url = matomo_url
         self.idsite = idsite
         self.assume_https = assume_https
         self.access_token = access_token
         self.lifespan_context = _DefaultLifespan(self)
         self.client = client
+        self.exclude_paths = set(exclude_paths or [])
+        self.compiled_patterns = [
+            re.compile(pattern) for pattern in (exclude_patterns or [])
+        ]
 
     async def startup(self) -> None:
         if self.client is None:
             self.client = httpx.AsyncClient()
 
     async def shutdown(self) -> None:
         if self.client is not None:
@@ -74,15 +82,15 @@
         try:
             async with self.lifespan_context(app) as maybe_state:
                 if maybe_state is not None:
                     if "state" not in scope:
                         raise RuntimeError(
                             'The server does not support "state" in the lifespan scope.'
                         )
-                    scope["state"].update(maybe_state)
+                    scope["state"].update(maybe_state)  # type: ignore
                 await send({"type": "lifespan.startup.complete"})
                 started = True
                 await receive()
         except BaseException:
             exc_text = traceback.format_exc()
             if started:
                 await send({"type": "lifespan.shutdown.failed", "message": exc_text})
@@ -91,14 +99,24 @@
             raise
         else:
             await send({"type": "lifespan.shutdown.complete"})
 
     async def __call__(
         self, scope: HTTPScope, receive: ASGIReceiveCallable, send: ASGISendCallable
     ) -> Any:
+        # locals inside the app function (send_wrapper) can't be assigned to,
+        # as the interpreter detects the assignment and thus creates a new
+        # local variable within that function, with that name.
+        instance = {"http_status_code": None}
+
+        def send_wrapper(response):
+            if response["type"] == "http.response.start":
+                instance["http_status_code"] = response["status"]
+            return send(response)
+
         if scope["type"] == "lifespan":
             await self.lifespan(scope, receive, send)
             return
 
         if scope["type"] != "http":
             await self.app(scope, receive, send)
             return
@@ -130,14 +148,22 @@
             logger.debug(
                 "splitting server addresses, using first",
                 extra={"server-orig": server, "servers": servers},
             )
             server = servers[0]
 
         path = scope["path"]
+        dont_track_this = False
+        if path in self.exclude_paths:
+            logger.debug("excluding path='%s'", path, extra={"path": path})
+            dont_track_this = True
+        elif any(pattern.match(path) for pattern in self.compiled_patterns):
+            logger.debug("excluding path='%s'", path, extra={"path": path})
+            dont_track_this = True
+
         if root_path := scope.get("root_path"):
             logger.debug("using root_path", extra={"root_path": root_path})
             path = f"{root_path}{path}"
 
         logger.debug(
             "building url",
             extra={
@@ -158,15 +184,15 @@
         )
 
         cip = scope["client"][0] if scope["client"] else None
 
         start_time_ns = time.perf_counter_ns()
 
         try:
-            await self.app(scope, receive, send)
+            await self.app(scope, receive, send_wrapper)
         except Exception:
             raise
         finally:
             end_time_ns = time.perf_counter_ns()
 
             params_that_require_token = {}
 
@@ -183,31 +209,47 @@
                 "idsite": self.idsite,
                 "url": url,
                 "rec": 1,
                 "rand": random.getrandbits(32),
                 "apiv": 1,
                 "ua": user_agent,
                 "gt_ms": (end_time_ns - start_time_ns) / 1000,
+                "send_image": 0,
+                "cvar": {
+                    "http_status_code": instance["http_status_code"],
+                    "http_method": scope["method"],
+                },
                 # "lang": accept_lang,
                 **params_that_require_token,
             }
 
             if accept_lang:
                 tracking_dict["lang"] = accept_lang
 
+            if "state" in scope and "asgi_matomo" in scope["state"]:  # type: ignore
+                for field, value in scope["state"]["asgi_matomo"].items():  # type: ignore
+                    if field == "cvar":
+                        tracking_dict["cvar"].update(value)  # type: ignore
+                    else:
+                        tracking_dict[field] = value
+
+            tracking_dict["cvar"] = json.dumps(tracking_dict["cvar"])
             tracking_params = urllib.parse.urlencode(tracking_dict)
             tracking_url = f"{self.matomo_url}?{tracking_params}"
-            logger.debug("Making tracking call", extra={"url": tracking_url})
-            try:
-                if self.client is None:
-                    logger.error("self.client is not set, can't track request")
-                else:
-                    tracking_response = await self.client.get(tracking_url)
-                    logger.debug(
-                        "tracking response",
-                        extra={
-                            "status": tracking_response.status_code,
-                            "content": tracking_response.text,
-                        },
-                    )
-            except httpx.HTTPError:
-                logger.exception("Error tracking view")
+            if dont_track_this:
+                logger.debug("NOT tracking call", extra={"url": tracking_url})
+            else:
+                logger.debug("Making tracking call", extra={"url": tracking_url})
+                try:
+                    if self.client is None:
+                        logger.error("self.client is not set, can't track request")
+                    else:
+                        tracking_response = await self.client.get(tracking_url)
+                        logger.debug(
+                            "tracking response",
+                            extra={
+                                "status": tracking_response.status_code,
+                                "content": tracking_response.text,
+                            },
+                        )
+                except httpx.HTTPError:
+                    logger.exception("Error tracking view")
```

### Comparing `asgi_matomo-0.1.4/pyproject.toml` & `asgi_matomo-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 [tool.poetry]
 name = "asgi-matomo"
-version = "0.1.4"
+version = "0.2.0"
 description = "Middleware for tracking ASGI reqeusts with Matomo"
 authors = ["Kristoffer Andersson <kristoffer.andersson@gu.se>"]
 license = "MIT"
 readme = "README.md"
+homepage = "https://spraakbanken.gu.se"
+repository = "https://github.com/spraakbanken/asgi-matomo"
 packages = [{include = "asgi_matomo"}]
 
+[tool.poetry.urls]
+"Bug Tracker" = "https://github.com/spraakbanken/asgi-matomo/issues"
+
 [tool.poetry.dependencies]
 python = "^3.10"
 asgiref = "^3.6.0"
 httpx = "^0.24.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
```

### Comparing `asgi_matomo-0.1.4/PKG-INFO` & `asgi_matomo-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,53 @@
-Metadata-Version: 2.1
-Name: asgi-matomo
-Version: 0.1.4
-Summary: Middleware for tracking ASGI reqeusts with Matomo
-License: MIT
-Author: Kristoffer Andersson
-Author-email: kristoffer.andersson@gu.se
-Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: asgiref (>=3.6.0,<4.0.0)
-Requires-Dist: httpx (>=0.24.0,<0.25.0)
-Description-Content-Type: text/markdown
-
 # asgi-matomo
 [![Packaging status](https://img.shields.io/pypi/v/asgi-matomo?color=%2334D058&label=pypi%20package)](https://pypi.org/project/asgi-matomo)
 [![CI](https://github.com/spraakbanken/asgi-matomo/workflows/CI/badge.svg)](https://github.com/spraakbanken/asgi-matomo/actions?query=workflow%3ACI)
 [![Coverage](https://github.com/spraakbanken/asgi-matomo/workflows/Coverage/badge.svg)](https://github.com/spraakbanken/asgi-matomo/actions?query=workflow%3ACoverage)
 [![codecov](https://codecov.io/gh/spraakbanken/asgi-matomo/branch/main/graph/badge.svg?token=MRJZVCJQF5)](https://codecov.io/gh/spraakbanken/asgi-matomo)
 
 Tracking requests with Matomo from ASGI apps.
 
-`MatomoMiddleware` adds tracking of all requests to Matomo to ASGI applications (Starlette, FastAPI, Quart, etc.).
+`MatomoMiddleware` adds tracking of all requests to Matomo to ASGI applications (Starlette, FastAPI, Quart, etc.). The intended usage is for api tracking (backends).
+
+**Note** If you serve HTML (directly or by templates), it is suggested to track those parts through Matomo's javascript tracking.
 
 **Installation**
 
 ```bash
 pip install asgi-matomo
 ```
 
+## What is tracked
+
+Currently this middleware tracks:
+- `url`
+- `ua`: user_agent
+- `gt_ms`: mesaured as the time before and after this middleware call next in the asgi stack.
+- `send_image=0` for performance issues
+- `cvar` with at least `http_status_code` and `http_method` set.
+- `lang` if `accept-lang` is set
+- `cip` client ip, **requires** `access_token` to be given.
+
+You can also pass variable to track by adding an `asgi_matomo`  dict in the `state` dict of the ASGI `scope`:
+```python
+scope = {
+  "state": {
+    "asgi_matomo": {
+      "e_a": "Playing",
+      "cvar": {
+        "your": "custom",
+        "data": "here",
+      }
+    }
+  }
+}
+```
+
+The keys of the `asgi_matomo` dict is expected to be valid parameter for the [Matomo HTTP Tracking API](https://developer.matomo.org/api-reference/tracking-api). `cvar` is serialized with the standard `json` lib.
+
 ## Examples
 
 ### Starlette
 
 ```python
 from starlette.applications import Starlette
 from starlette.responses import JSONResponse
@@ -81,36 +95,34 @@
 ```python
 app.add_middleware(
   MatomoMiddleware,
   matomo_url="YOUR MATOMO TRACKING URL",
   idsite=12345, # your service tracking id
   access_token="SECRETTOKEN",
   assume_https=True,
-  minimum_size=400,
+  exclude_paths=["/health"],
+  exclude_patterns=[".*/old.*"],
 )
 ```
 
 **Parameters**:
 
 - **(Required)** `matomo_url`: The URL to make your tracking calls to.
 - **(Required)** `idsite`: The tracking id for your service.
 - _(Optional)_ `access_token`: Access token for Matomo. If this is set `cip` is also tracked. Required for tracking some data.
 - _(Optional)_ `assume_https`: If `True`, set tracked url scheme to `https`, useful when running behind a proxy. Defaults to `True`.
+- _(Optional)_ `exclude_paths`: A list of paths to exclude, only excludes path that is equal to a path in this list. These are tried before `exclude_patterns`.
+- _(Optional)_ `exclude_patterns`: A list of regex patterns that are compiled, and then exclude a path from tracking if any pattern match.
+These are tried after `exclude_paths`.
 
 
 **Notes**:
 
 - Currently only some parts [Matomo Tracking HTTP API](https://developer.matomo.org/api-reference/tracking-api) is supported.
 
 ## Ideas for further work:
-- _filtering tracked of urls_
-- _custom extraction of tracked data_
-
-
-# Release Notes
-## Latest Changes
-
-## 0.1.0 - 2023-04-28
+- [x] _filtering tracked of urls_
+- [x] _custom extraction of tracked data_
 
-- Initial release.
 
+This project keeps a [changelog](./CHANGELOG.md).
```


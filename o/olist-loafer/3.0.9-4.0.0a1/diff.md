# Comparing `tmp/olist-loafer-3.0.9.tar.gz` & `tmp/olist_loafer-4.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olist-loafer-3.0.9.tar", max compression
+gzip compressed data, was "olist_loafer-4.0.0a1.tar", max compression
```

## Comparing `olist-loafer-3.0.9.tar` & `olist_loafer-4.0.0a1.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0     1083 2021-09-25 11:54:05.667849 olist-loafer-3.0.9/LICENSE
--rw-r--r--   0        0        0     1676 2021-09-25 11:54:05.667849 olist-loafer-3.0.9/README.md
--rw-r--r--   0        0        0        0 2021-09-25 11:54:05.667849 olist-loafer-3.0.9/loafer/__init__.py
--rw-r--r--   0        0        0     2517 2021-09-25 11:54:05.667849 olist-loafer-3.0.9/loafer/dispatchers.py
--rw-r--r--   0        0        0      237 2021-09-25 11:54:05.667849 olist-loafer-3.0.9/loafer/exceptions.py
--rw-r--r--   0        0        0        0 2021-09-25 11:54:05.667849 olist-loafer-3.0.9/loafer/ext/__init__.py
--rw-r--r--   0        0        0        0 2021-09-25 11:54:05.667849 olist-loafer-3.0.9/loafer/ext/aws/__init__.py
--rw-r--r--   0        0        0     1920 2021-10-12 18:13:14.113715 olist-loafer-3.0.9/loafer/ext/aws/bases.py
--rw-r--r--   0        0        0     1896 2021-09-25 11:54:05.667849 olist-loafer-3.0.9/loafer/ext/aws/handlers.py
--rw-r--r--   0        0        0     1752 2021-09-25 11:54:05.667849 olist-loafer-3.0.9/loafer/ext/aws/message_translators.py
--rw-r--r--   0        0        0     3356 2021-10-29 16:24:47.915708 olist-loafer-3.0.9/loafer/ext/aws/providers.py
--rw-r--r--   0        0        0     1130 2021-09-25 11:54:05.667849 olist-loafer-3.0.9/loafer/ext/aws/routes.py
--rw-r--r--   0        0        0      329 2021-09-25 11:54:05.667849 olist-loafer-3.0.9/loafer/ext/sentry.py
--rw-r--r--   0        0        0     2060 2021-10-12 22:41:21.453715 olist-loafer-3.0.9/loafer/managers.py
--rw-r--r--   0        0        0      735 2021-10-12 18:13:14.113715 olist-loafer-3.0.9/loafer/message_translators.py
--rw-r--r--   0        0        0      890 2021-10-12 18:13:14.113715 olist-loafer-3.0.9/loafer/providers.py
--rw-r--r--   0        0        0     2938 2021-09-25 11:54:05.667849 olist-loafer-3.0.9/loafer/routes.py
--rw-r--r--   0        0        0     2481 2021-10-29 17:20:45.775708 olist-loafer-3.0.9/loafer/runners.py
--rw-r--r--   0        0        0     1548 2021-09-25 12:45:54.182615 olist-loafer-3.0.9/loafer/utils.py
--rw-r--r--   0        0        0     1734 2021-10-29 17:20:45.785708 olist-loafer-3.0.9/pyproject.toml
--rw-r--r--   0        0        0     2478 2021-10-29 17:21:32.918672 olist-loafer-3.0.9/setup.py
--rw-r--r--   0        0        0     2896 2021-10-29 17:21:32.919817 olist-loafer-3.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-11-08 20:03:57.885056 olist_loafer-4.0.0a1/LICENSE
+-rw-r--r--   0        0        0     1676 2022-11-08 20:03:57.885056 olist_loafer-4.0.0a1/README.md
+-rw-r--r--   0        0        0        0 2022-11-08 20:03:57.895056 olist_loafer-4.0.0a1/loafer/__init__.py
+-rw-r--r--   0        0        0     2362 2023-05-12 15:01:11.963967 olist_loafer-4.0.0a1/loafer/dispatchers.py
+-rw-r--r--   0        0        0      237 2022-11-08 20:03:57.895056 olist_loafer-4.0.0a1/loafer/exceptions.py
+-rw-r--r--   0        0        0        0 2022-11-08 20:03:57.895056 olist_loafer-4.0.0a1/loafer/ext/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-08 20:03:57.905057 olist_loafer-4.0.0a1/loafer/ext/aws/__init__.py
+-rw-r--r--   0        0        0     1920 2023-04-29 19:25:57.593482 olist_loafer-4.0.0a1/loafer/ext/aws/bases.py
+-rw-r--r--   0        0        0     1896 2023-01-11 19:30:20.652969 olist_loafer-4.0.0a1/loafer/ext/aws/handlers.py
+-rw-r--r--   0        0        0     1752 2023-03-25 12:20:00.904444 olist_loafer-4.0.0a1/loafer/ext/aws/message_translators.py
+-rw-r--r--   0        0        0     3356 2023-04-29 19:25:57.593482 olist_loafer-4.0.0a1/loafer/ext/aws/providers.py
+-rw-r--r--   0        0        0     1130 2022-11-08 20:03:57.905057 olist_loafer-4.0.0a1/loafer/ext/aws/routes.py
+-rw-r--r--   0        0        0      329 2022-11-08 20:03:57.905057 olist_loafer-4.0.0a1/loafer/ext/sentry.py
+-rw-r--r--   0        0        0     2053 2023-04-29 19:25:57.603482 olist_loafer-4.0.0a1/loafer/managers.py
+-rw-r--r--   0        0        0      735 2023-04-29 19:25:57.603482 olist_loafer-4.0.0a1/loafer/message_translators.py
+-rw-r--r--   0        0        0      890 2023-04-29 19:25:57.603482 olist_loafer-4.0.0a1/loafer/providers.py
+-rw-r--r--   0        0        0     2938 2023-04-29 19:25:57.603482 olist_loafer-4.0.0a1/loafer/routes.py
+-rw-r--r--   0        0        0     2481 2023-04-29 19:25:57.603482 olist_loafer-4.0.0a1/loafer/runners.py
+-rw-r--r--   0        0        0      569 2023-04-29 19:25:57.603482 olist_loafer-4.0.0a1/loafer/utils.py
+-rw-r--r--   0        0        0     1727 2023-05-12 15:10:37.873968 olist_loafer-4.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     3053 1970-01-01 00:00:00.000000 olist_loafer-4.0.0a1/PKG-INFO
```

### Comparing `olist-loafer-3.0.9/LICENSE` & `olist_loafer-4.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `olist-loafer-3.0.9/README.md` & `olist_loafer-4.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `olist-loafer-3.0.9/loafer/dispatchers.py` & `olist_loafer-4.0.0a1/loafer/dispatchers.py`

 * *Files 18% similar despite different names*

```diff
@@ -41,35 +41,29 @@
         provider = route.provider
         if confirmation:
             await provider.confirm_message(message)
         else:
             await provider.message_not_processed(message)
         return confirmation
 
-    async def _get_route_messages(self, route):
-        messages = await route.provider.fetch_messages()
-        return messages, route
-
-    async def _dispatch_tasks(self):
-        provider_messages_tasks = [self._get_route_messages(route) for route in self.routes]
-
-        process_messages_tasks = []
-        for provider_task in asyncio.as_completed(provider_messages_tasks):
-            messages, route = await provider_task
-
-            process_messages_tasks += [self._process_message(message, route) for message in messages]
+    async def _dispatch_provider(self, route, forever=True):
+        while True:
+            messages = await route.provider.fetch_messages()
+            process_messages_tasks = [
+                asyncio.create_task(self._process_message(message, route)) for message in messages
+            ]
 
-        if not process_messages_tasks:
-            return
+            await asyncio.gather(*process_messages_tasks)
 
-        await asyncio.gather(*process_messages_tasks)
+            if not forever:
+                break
 
     async def dispatch_providers(self, forever=True):
-        while True:
-            await self._dispatch_tasks()
+        dispatch_provider_tasks = [
+            asyncio.create_task(self._dispatch_provider(route, forever)) for route in self.routes
+        ]
 
-            if not forever:
-                break
+        await asyncio.gather(*dispatch_provider_tasks)
 
     def stop(self):
         for route in self.routes:
             route.stop()
```

### Comparing `olist-loafer-3.0.9/loafer/ext/aws/bases.py` & `olist_loafer-4.0.0a1/loafer/ext/aws/bases.py`

 * *Files identical despite different names*

### Comparing `olist-loafer-3.0.9/loafer/ext/aws/handlers.py` & `olist_loafer-4.0.0a1/loafer/ext/aws/handlers.py`

 * *Files identical despite different names*

### Comparing `olist-loafer-3.0.9/loafer/ext/aws/message_translators.py` & `olist_loafer-4.0.0a1/loafer/ext/aws/message_translators.py`

 * *Files identical despite different names*

### Comparing `olist-loafer-3.0.9/loafer/ext/aws/providers.py` & `olist_loafer-4.0.0a1/loafer/ext/aws/providers.py`

 * *Files identical despite different names*

### Comparing `olist-loafer-3.0.9/loafer/ext/aws/routes.py` & `olist_loafer-4.0.0a1/loafer/ext/aws/routes.py`

 * *Files identical despite different names*

### Comparing `olist-loafer-3.0.9/loafer/managers.py` & `olist_loafer-4.0.0a1/loafer/managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import asyncio
 import logging
 import os
-
-from cached_property import cached_property
+from functools import cached_property
 
 from .dispatchers import LoaferDispatcher
 from .exceptions import ConfigurationError
 from .routes import Route
 from .runners import LoaferRunner
 
 logger = logging.getLogger(__name__)
```

### Comparing `olist-loafer-3.0.9/loafer/message_translators.py` & `olist_loafer-4.0.0a1/loafer/message_translators.py`

 * *Files identical despite different names*

### Comparing `olist-loafer-3.0.9/loafer/providers.py` & `olist_loafer-4.0.0a1/loafer/providers.py`

 * *Files identical despite different names*

### Comparing `olist-loafer-3.0.9/loafer/routes.py` & `olist_loafer-4.0.0a1/loafer/routes.py`

 * *Files identical despite different names*

### Comparing `olist-loafer-3.0.9/loafer/runners.py` & `olist_loafer-4.0.0a1/loafer/runners.py`

 * *Files identical despite different names*

### Comparing `olist-loafer-3.0.9/pyproject.toml` & `olist_loafer-4.0.0a1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 [tool.black]
 line-length = 110
-target-version = ["py37"]
+target-version = ["py38"]
 
 [tool.isort]
 line_length = 100
 multi_line_output = 3
 known_localfolder = ["loafer", "tests"]
 sections = ["FUTURE", "STDLIB", "THIRDPARTY", "LOCALFOLDER"]
 default_section = "THIRDPARTY"
 include_trailing_comma = true
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 addopts = "-vv --cov=loafer --cov-report=term-missing"
+asyncio_mode = "strict"
 
 [tool.poetry]
 name = "olist-loafer"
-version = "3.0.9"
+version = "4.0.0a1"
 description = "Asynchronous message dispatcher for concurrent tasks processing"
 license = "MIT"
 authors = ["Olist <developers@olist.com>"]
 readme = "README.md"
 repository = "https://github.com/olist/olist-loafer/"
 keywords = ["asyncio", "message", "dispatcher", "tasks", "microservices"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: System :: Distributed Computing",
 ]
 packages = [{ include = "loafer" }]
 
 [tool.poetry.urls]
 "Download" = "https://github.com/olist/olist-loafer/releases"
 
 [tool.poetry.dependencies]
-python = ">=3.7,<3.11"
-aiobotocore = { version = "^1.0.0", extras = ["boto3"] }
-cached-property = "^1.3.0"
+python = ">=3.8,<3.12"
+aiobotocore = { version = ">=1.0.0,<3.0.0", extras = ["boto3"] }
 
 [tool.poetry.dev-dependencies]
-asynctest = { version = "*", python = "<3.8" }
 pre-commit = "*"
-codecov = "*"
 pytest = "*"
 pytest-asyncio = "*"
 pytest-cov = "*"
 pytest-deadfixtures = "*"
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
```

### Comparing `olist-loafer-3.0.9/PKG-INFO` & `olist_loafer-4.0.0a1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 Metadata-Version: 2.1
 Name: olist-loafer
-Version: 3.0.9
+Version: 4.0.0a1
 Summary: Asynchronous message dispatcher for concurrent tasks processing
 Home-page: https://github.com/olist/olist-loafer/
 License: MIT
 Keywords: asyncio,message,dispatcher,tasks,microservices
 Author: Olist
 Author-email: developers@olist.com
-Requires-Python: >=3.7,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System :: Distributed Computing
-Requires-Dist: aiobotocore[boto3] (>=1.0.0,<2.0.0)
-Requires-Dist: cached-property (>=1.3.0,<2.0.0)
+Requires-Dist: aiobotocore[boto3] (>=1.0.0,<3.0.0)
 Project-URL: Download, https://github.com/olist/olist-loafer/releases
 Project-URL: Repository, https://github.com/olist/olist-loafer/
 Description-Content-Type: text/markdown
 
 [![PyPI latest](https://img.shields.io/pypi/v/olist-loafer.svg?maxAge=2592000)](https://pypi.python.org/pypi/loafer)
 [![Python versions](https://img.shields.io/pypi/pyversions/olist-loafer.svg?maxAge=2592000)](https://pypi.python.org/pypi/loafer)
 [![License](https://img.shields.io/pypi/l/loafer.svg?maxAge=2592000)](https://pypi.python.org/pypi/olist-loafer)
```


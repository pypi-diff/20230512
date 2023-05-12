# Comparing `tmp/vedro-cloud-0.3.0.tar.gz` & `tmp/vedro-cloud-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vedro-cloud-0.3.0.tar", last modified: Mon Dec 26 12:43:46 2022, max compression
+gzip compressed data, was "vedro-cloud-0.3.1.tar", last modified: Fri May 12 12:54:16 2023, max compression
```

## Comparing `vedro-cloud-0.3.0.tar` & `vedro-cloud-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-26 12:43:46.777839 vedro-cloud-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-26 12:43:36.000000 vedro-cloud-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2022-12-26 12:43:46.777839 vedro-cloud-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      896 2022-12-26 12:43:36.000000 vedro-cloud-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      727 2022-12-26 12:43:46.777839 vedro-cloud-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2022-12-26 12:43:36.000000 vedro-cloud-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-26 12:43:46.773839 vedro-cloud-0.3.0/vedro_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2022-12-26 12:43:36.000000 vedro-cloud-0.3.0/vedro_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2022-12-26 12:43:36.000000 vedro-cloud-0.3.0/vedro_cloud/_duration_orderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2022-12-26 12:43:36.000000 vedro-cloud-0.3.0/vedro_cloud/_validate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2022-12-26 12:43:36.000000 vedro-cloud-0.3.0/vedro_cloud/_vedro_cloud_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2022-12-26 12:43:36.000000 vedro-cloud-0.3.0/vedro_cloud/_vedro_cloud_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-26 12:43:36.000000 vedro-cloud-0.3.0/vedro_cloud/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-26 12:43:46.777839 vedro-cloud-0.3.0/vedro_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2022-12-26 12:43:46.000000 vedro-cloud-0.3.0/vedro_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2022-12-26 12:43:46.000000 vedro-cloud-0.3.0/vedro_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-26 12:43:46.000000 vedro-cloud-0.3.0/vedro_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2022-12-26 12:43:46.000000 vedro-cloud-0.3.0/vedro_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-26 12:43:46.000000 vedro-cloud-0.3.0/vedro_cloud.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:54:16.450305 vedro-cloud-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-12 12:54:03.000000 vedro-cloud-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-12 12:54:16.450305 vedro-cloud-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-12 12:54:03.000000 vedro-cloud-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-12 12:54:16.454305 vedro-cloud-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-12 12:54:03.000000 vedro-cloud-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:54:16.450305 vedro-cloud-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-12 12:54:03.000000 vedro-cloud-0.3.1/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:54:16.450305 vedro-cloud-0.3.1/vedro_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-12 12:54:03.000000 vedro-cloud-0.3.1/vedro_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-12 12:54:03.000000 vedro-cloud-0.3.1/vedro_cloud/_duration_orderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-12 12:54:03.000000 vedro-cloud-0.3.1/vedro_cloud/_validate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-12 12:54:03.000000 vedro-cloud-0.3.1/vedro_cloud/_vedro_cloud_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-05-12 12:54:03.000000 vedro-cloud-0.3.1/vedro_cloud/_vedro_cloud_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 12:54:03.000000 vedro-cloud-0.3.1/vedro_cloud/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:54:16.450305 vedro-cloud-0.3.1/vedro_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-12 12:54:16.000000 vedro-cloud-0.3.1/vedro_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-12 12:54:16.000000 vedro-cloud-0.3.1/vedro_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 12:54:16.000000 vedro-cloud-0.3.1/vedro_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-12 12:54:16.000000 vedro-cloud-0.3.1/vedro_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-12 12:54:16.000000 vedro-cloud-0.3.1/vedro_cloud.egg-info/top_level.txt
```

### Comparing `vedro-cloud-0.3.0/LICENSE` & `vedro-cloud-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vedro-cloud-0.3.0/PKG-INFO` & `vedro-cloud-0.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: vedro-cloud
-Version: 0.3.0
-Summary: Validator Cloud plugin
+Version: 0.3.1
+Summary: Vedro Cloud plugin
 Home-page: https://github.com/vedro-universe/vedro-cloud
 Author: Nikita Tsvetkov
-Author-email: nikitanovosibirsk@yandex.com
+Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Vedro Cloud
 
+[![Codecov](https://img.shields.io/codecov/c/github/vedro-universe/vedro-cloud/main.svg?style=flat-square)](https://codecov.io/gh/vedro-universe/vedro-cloud)
 [![PyPI](https://img.shields.io/pypi/v/vedro-cloud.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-cloud/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro-cloud?style=flat-square)](https://pypi.python.org/pypi/vedro-cloud/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro-cloud.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-cloud/)
 
 ## Installation
 
 ### 1. Install package
@@ -39,13 +40,28 @@
 
 class Config(vedro.Config):
 
     class Plugins(vedro.Config.Plugins):
 
         class VedroCloud(vedro_cloud.VedroCloud):
             enabled = True
-            api_url = "http://localhost:8080"
+            api_url = "http://localhost:8080"  # Vedro Cloud API
             project_id = "test"
 
         class Slicer(slicer.Slicer):
             enabled = False
 ```
+
+### 3. Run Server
+
+Use `docker-compose.yml` from [vedro-universe/vedro-cloud-api](https://github.com/vedro-universe/vedro-cloud-api)
+
+```shell
+$ docker-compose up -d
+===== Running on http://localhost:8080 =====
+```
+
+## Usage
+
+```shell
+$ vedro run --order-duration
+```
```

### Comparing `vedro-cloud-0.3.0/README.md` & `vedro-cloud-0.3.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Vedro Cloud
 
+[![Codecov](https://img.shields.io/codecov/c/github/vedro-universe/vedro-cloud/main.svg?style=flat-square)](https://codecov.io/gh/vedro-universe/vedro-cloud)
 [![PyPI](https://img.shields.io/pypi/v/vedro-cloud.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-cloud/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro-cloud?style=flat-square)](https://pypi.python.org/pypi/vedro-cloud/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro-cloud.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-cloud/)
 
 ## Installation
 
 ### 1. Install package
@@ -22,13 +23,28 @@
 
 class Config(vedro.Config):
 
     class Plugins(vedro.Config.Plugins):
 
         class VedroCloud(vedro_cloud.VedroCloud):
             enabled = True
-            api_url = "http://localhost:8080"
+            api_url = "http://localhost:8080"  # Vedro Cloud API
             project_id = "test"
 
         class Slicer(slicer.Slicer):
             enabled = False
 ```
+
+### 3. Run Server
+
+Use `docker-compose.yml` from [vedro-universe/vedro-cloud-api](https://github.com/vedro-universe/vedro-cloud-api)
+
+```shell
+$ docker-compose up -d
+===== Running on http://localhost:8080 =====
+```
+
+## Usage
+
+```shell
+$ vedro run --order-duration
+```
```

### Comparing `vedro-cloud-0.3.0/setup.cfg` & `vedro-cloud-0.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.3.0
+current_version = 0.3.1
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `vedro-cloud-0.3.0/setup.py` & `vedro-cloud-0.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="vedro-cloud",
-    version="0.3.0",
-    description="Validator Cloud plugin",
+    version="0.3.1",
+    description="Vedro Cloud plugin",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
-    author_email="nikitanovosibirsk@yandex.com",
+    author_email="tsv1@fastmail.com",
     python_requires=">=3.8",
     url="https://github.com/vedro-universe/vedro-cloud",
     license="Apache-2.0",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"vedro_cloud": ["py.typed"]},
     install_requires=find_required(),
     tests_require=find_dev_required(),
```

### Comparing `vedro-cloud-0.3.0/vedro_cloud/_duration_orderer.py` & `vedro-cloud-0.3.1/vedro_cloud/_duration_orderer.py`

 * *Files identical despite different names*

### Comparing `vedro-cloud-0.3.0/vedro_cloud/_validate_config.py` & `vedro-cloud-0.3.1/vedro_cloud/_validate_config.py`

 * *Files identical despite different names*

### Comparing `vedro-cloud-0.3.0/vedro_cloud/_vedro_cloud_client.py` & `vedro-cloud-0.3.1/vedro_cloud/_vedro_cloud_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     def __init__(self, project_id: str, api_url: str, timeout: float) -> None:
         self._project_id = project_id
         self._api_url = api_url
         self._timeout = timeout
 
     async def _do_request(self, method: str, url: str, **kwargs: Any) -> Any:
         async with AsyncClient() as client:
-            resp = await client.request(method, url, **kwargs)
+            resp = await client.request(method, url, timeout=self._timeout, **kwargs)
             try:
                 body = resp.json()
             except:  # noqa: E722
                 body = None
             if (resp.status_code != HTTPStatus.OK) or (body is None):
                 raise ValueError(
                     f"Invalid response from '{url}': {resp.status_code} {resp.read()!r}")
```

### Comparing `vedro-cloud-0.3.0/vedro_cloud/_vedro_cloud_plugin.py` & `vedro-cloud-0.3.1/vedro_cloud/_vedro_cloud_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, Dict, List, Optional, Type, TypedDict, Union
 from uuid import uuid4
 
+from rtry import retry
 from vedro.core import ConfigType, Dispatcher, Plugin, PluginConfig
 from vedro.events import (
     ArgParsedEvent,
     ArgParseEvent,
     CleanupEvent,
     ConfigLoadedEvent,
     ScenarioFailedEvent,
@@ -34,18 +35,19 @@
         self._results: List[Dict[str, Any]] = []
         self._timings: Dict[str, int] = {}
         self._total: Union[int, None] = None
         self._index: Union[int, None] = None
 
     async def _get_timings(self) -> Dict[str, int]:
         try:
-            self._timings = await self._client.get_timings(self._report_id)
+            self._timings = await retry(attempts=3,
+                                        delay=1.0)(self._client.get_timings)(self._report_id)
         except Exception as e:
             print(f"-> Failed to retrieve timings: {e!r}")
-            self._timings = {}
+            exit(1)
         if self._verbose:
             print("-> Retrieved timings:", len(self._timings), self._report_id)
         return self._timings
 
     async def _post_history(self) -> None:
         try:
             await self._client.post_history(self._results)
```

### Comparing `vedro-cloud-0.3.0/vedro_cloud.egg-info/PKG-INFO` & `vedro-cloud-0.3.1/vedro_cloud.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: vedro-cloud
-Version: 0.3.0
-Summary: Validator Cloud plugin
+Version: 0.3.1
+Summary: Vedro Cloud plugin
 Home-page: https://github.com/vedro-universe/vedro-cloud
 Author: Nikita Tsvetkov
-Author-email: nikitanovosibirsk@yandex.com
+Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Vedro Cloud
 
+[![Codecov](https://img.shields.io/codecov/c/github/vedro-universe/vedro-cloud/main.svg?style=flat-square)](https://codecov.io/gh/vedro-universe/vedro-cloud)
 [![PyPI](https://img.shields.io/pypi/v/vedro-cloud.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-cloud/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro-cloud?style=flat-square)](https://pypi.python.org/pypi/vedro-cloud/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro-cloud.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-cloud/)
 
 ## Installation
 
 ### 1. Install package
@@ -39,13 +40,28 @@
 
 class Config(vedro.Config):
 
     class Plugins(vedro.Config.Plugins):
 
         class VedroCloud(vedro_cloud.VedroCloud):
             enabled = True
-            api_url = "http://localhost:8080"
+            api_url = "http://localhost:8080"  # Vedro Cloud API
             project_id = "test"
 
         class Slicer(slicer.Slicer):
             enabled = False
 ```
+
+### 3. Run Server
+
+Use `docker-compose.yml` from [vedro-universe/vedro-cloud-api](https://github.com/vedro-universe/vedro-cloud-api)
+
+```shell
+$ docker-compose up -d
+===== Running on http://localhost:8080 =====
+```
+
+## Usage
+
+```shell
+$ vedro run --order-duration
+```
```


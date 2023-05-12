# Comparing `tmp/django_flyio-0.1.0.tar.gz` & `tmp/django_flyio-0.1.1.tar.gz`

## Comparing `django_flyio-0.1.0.tar` & `django_flyio-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 django_flyio-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 django_flyio-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 django_flyio-0.1.0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 django_flyio-0.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 django_flyio-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_flyio-0.1.0/src/django_flyio/__init__.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 django_flyio-0.1.0/src/django_flyio/db.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 django_flyio-0.1.0/src/django_flyio/middleware.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 django_flyio-0.1.0/src/django_flyio/routers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_flyio-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 django_flyio-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 django_flyio-0.1.0/tests/settings.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 django_flyio-0.1.0/tests/test_db.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 django_flyio-0.1.0/tests/test_middleware.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 django_flyio-0.1.0/tests/test_routers.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 django_flyio-0.1.0/tests/urls.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 django_flyio-0.1.0/tests/views.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 django_flyio-0.1.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 django_flyio-0.1.0/LICENSE
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 django_flyio-0.1.0/README.md
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 django_flyio-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 django_flyio-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 django_flyio-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 django_flyio-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 django_flyio-0.1.1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 django_flyio-0.1.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 django_flyio-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_flyio-0.1.1/src/django_flyio/__init__.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 django_flyio-0.1.1/src/django_flyio/db.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 django_flyio-0.1.1/src/django_flyio/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_flyio-0.1.1/src/django_flyio/py.typed
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 django_flyio-0.1.1/src/django_flyio/routers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_flyio-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 django_flyio-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 django_flyio-0.1.1/tests/settings.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 django_flyio-0.1.1/tests/test_db.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 django_flyio-0.1.1/tests/test_middleware.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 django_flyio-0.1.1/tests/test_routers.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 django_flyio-0.1.1/tests/urls.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 django_flyio-0.1.1/tests/views.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 django_flyio-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 django_flyio-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 django_flyio-0.1.1/README.md
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 django_flyio-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 django_flyio-0.1.1/PKG-INFO
```

### Comparing `django_flyio-0.1.0/.pre-commit-config.yaml` & `django_flyio-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django_flyio-0.1.0/CHANGELOG.md` & `django_flyio-0.1.1/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -3,23 +3,29 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project attempts to adhere to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.1.1] - 2023-05-12
+
+### Fixed
+
+- Added `py.typed` file to package to indicate that it supports type hints
 
 ## [0.1.0] - 2023-05-12
 
 Initial release!
 
 ### Added
 
 - A function that reads the environment and returns a `DATABASES` setting for a multi-region Fly Postgres database
 - A router that routes reads to a replica database if the `DATABASES` setting has a `replica` key
 - A middleware that sets the `Fly-Server` header containing the Fly server and region that served the request
 - Initial documentation (README.md)
 - Initial tests
 - Initial CI/CD (GitHub Actions)
 
-[unreleased]: https://github.com/joshuadavidthomas/django-flyio/compare/v0.1.0...HEAD
+[unreleased]: https://github.com/joshuadavidthomas/django-flyio/compare/v0.1.1...HEAD
+[0.1.1]: https://github.com/joshuadavidthomas/django-flyio/releases/tag/v0.1.1
 [0.1.0]: https://github.com/joshuadavidthomas/django-flyio/releases/tag/v0.1.0
```

### Comparing `django_flyio-0.1.0/.devcontainer/devcontainer.json` & `django_flyio-0.1.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `django_flyio-0.1.0/.github/workflows/release.yml` & `django_flyio-0.1.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django_flyio-0.1.0/.github/workflows/test.yml` & `django_flyio-0.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django_flyio-0.1.0/src/django_flyio/db.py` & `django_flyio-0.1.1/src/django_flyio/db.py`

 * *Files identical despite different names*

### Comparing `django_flyio-0.1.0/src/django_flyio/middleware.py` & `django_flyio-0.1.1/src/django_flyio/middleware.py`

 * *Files identical despite different names*

### Comparing `django_flyio-0.1.0/src/django_flyio/routers.py` & `django_flyio-0.1.1/src/django_flyio/routers.py`

 * *Files identical despite different names*

### Comparing `django_flyio-0.1.0/tests/test_middleware.py` & `django_flyio-0.1.1/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django_flyio-0.1.0/tests/test_routers.py` & `django_flyio-0.1.1/tests/test_routers.py`

 * *Files identical despite different names*

### Comparing `django_flyio-0.1.0/.gitignore` & `django_flyio-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `django_flyio-0.1.0/LICENSE` & `django_flyio-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_flyio-0.1.0/README.md` & `django_flyio-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -26,19 +26,18 @@
 2.  Add `django_flyio.routers.FlyDBReplicaRouter` to your `DATABASE_ROUTERS` settings.
 
     This router reads whether the `DATABASES` setting has a `replica` key and, if so, routes reads to the replica database.
 
 ```python
 # settings.py
 from django_flyio.db import get_db_config
-from django_flyio.routers import FlyDBReplicaRouter
 
 DATABASES = get_db_config()
 
-DATABASE_ROUTERS = [FlyDBReplicaRouter]
+DATABASE_ROUTERS = ["django_flyio.routers.FlyDBReplicaRouter"]
 ```
 
 ### Middleware
 
 To set the `Fly-Server` header containing the Fly server and region that served the request, add `django_flyio.middleware.FlyResponseMiddleware` to your `MIDDLEWARE` settings.
 
 ```python
```

### Comparing `django_flyio-0.1.0/pyproject.toml` & `django_flyio-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_flyio-0.1.0/PKG-INFO` & `django_flyio-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-flyio
-Version: 0.1.0
+Version: 0.1.1
 Summary: A set of simple utilities for Django apps running on Fly.io
 Project-URL: Documentation, https://github.com/joshuadavidthomas/django-flyio#readme
 Project-URL: Issues, https://github.com/joshuadavidthomas/django-flyio/issues
 Project-URL: Source, https://github.com/joshuadavidthomas/django-flyio
 Author-email: Josh <josh@joshthomas.dev>
 License-Expression: MIT
 License-File: LICENSE
@@ -65,19 +65,18 @@
 2.  Add `django_flyio.routers.FlyDBReplicaRouter` to your `DATABASE_ROUTERS` settings.
 
     This router reads whether the `DATABASES` setting has a `replica` key and, if so, routes reads to the replica database.
 
 ```python
 # settings.py
 from django_flyio.db import get_db_config
-from django_flyio.routers import FlyDBReplicaRouter
 
 DATABASES = get_db_config()
 
-DATABASE_ROUTERS = [FlyDBReplicaRouter]
+DATABASE_ROUTERS = ["django_flyio.routers.FlyDBReplicaRouter"]
 ```
 
 ### Middleware
 
 To set the `Fly-Server` header containing the Fly server and region that served the request, add `django_flyio.middleware.FlyResponseMiddleware` to your `MIDDLEWARE` settings.
 
 ```python
```


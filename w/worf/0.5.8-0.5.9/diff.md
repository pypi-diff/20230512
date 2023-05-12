# Comparing `tmp/worf-0.5.8.tar.gz` & `tmp/worf-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "worf-0.5.8.tar", last modified: Thu Jun 16 15:29:12 2022, max compression
+gzip compressed data, was "worf-0.5.9.tar", last modified: Fri Jun 24 15:55:34 2022, max compression
```

## Comparing `worf-0.5.8.tar` & `worf-0.5.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-16 15:29:12.655521 worf-0.5.8/
--rw-r--r--   0 root         (0) root         (0)    10337 2022-06-16 15:28:44.000000 worf-0.5.8/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1086 2022-02-04 06:42:11.000000 worf-0.5.8/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      176 2022-02-04 06:42:11.000000 worf-0.5.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    15597 2022-06-16 15:29:12.658273 worf-0.5.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14638 2022-05-04 08:45:52.000000 worf-0.5.8/README.md
--rw-r--r--   0 root         (0) root         (0)      206 2022-02-22 16:46:06.000000 worf-0.5.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      443 2022-06-16 15:29:12.662691 worf-0.5.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1985 2022-02-04 06:42:11.000000 worf-0.5.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-16 15:29:12.403414 worf-0.5.8/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-04 06:42:11.000000 worf-0.5.8/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2006 2022-05-04 09:05:10.000000 worf-0.5.8/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1334 2022-02-04 06:42:11.000000 worf-0.5.8/tests/factories.py
--rw-r--r--   0 root         (0) root         (0)     2621 2022-06-16 15:22:29.000000 worf-0.5.8/tests/models.py
--rw-r--r--   0 root         (0) root         (0)     1457 2022-06-16 15:22:29.000000 worf-0.5.8/tests/serializers.py
--rw-r--r--   0 root         (0) root         (0)      811 2022-02-04 06:42:11.000000 worf-0.5.8/tests/test_browsable_api.py
--rw-r--r--   0 root         (0) root         (0)     1069 2022-02-04 06:42:11.000000 worf-0.5.8/tests/test_casing.py
--rw-r--r--   0 root         (0) root         (0)      233 2022-02-04 06:42:11.000000 worf-0.5.8/tests/test_conf.py
--rw-r--r--   0 root         (0) root         (0)      924 2022-02-04 06:42:11.000000 worf-0.5.8/tests/test_permissions.py
--rw-r--r--   0 root         (0) root         (0)      130 2022-02-04 06:42:11.000000 worf-0.5.8/tests/test_shortcuts.py
--rw-r--r--   0 root         (0) root         (0)     3266 2022-06-16 15:22:29.000000 worf-0.5.8/tests/test_validators.py
--rw-r--r--   0 root         (0) root         (0)    16341 2022-06-16 15:22:29.000000 worf-0.5.8/tests/test_views.py
--rw-r--r--   0 root         (0) root         (0)      428 2022-02-04 06:42:11.000000 worf-0.5.8/tests/urls.py
--rw-r--r--   0 root         (0) root         (0)     2072 2022-02-07 08:37:51.000000 worf-0.5.8/tests/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-16 15:29:12.516507 worf-0.5.8/worf/
--rw-r--r--   0 root         (0) root         (0)       23 2022-06-16 15:28:44.000000 worf-0.5.8/worf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3457 2022-06-16 15:13:56.000000 worf-0.5.8/worf/assigns.py
--rw-r--r--   0 root         (0) root         (0)     1137 2022-02-23 09:19:00.000000 worf-0.5.8/worf/casing.py
--rw-r--r--   0 root         (0) root         (0)      159 2022-02-23 09:19:00.000000 worf-0.5.8/worf/conf.py
--rw-r--r--   0 root         (0) root         (0)      959 2022-02-23 09:19:00.000000 worf-0.5.8/worf/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      768 2022-06-16 15:22:29.000000 worf-0.5.8/worf/fields.py
--rw-r--r--   0 root         (0) root         (0)     1869 2022-02-23 09:19:00.000000 worf-0.5.8/worf/filters.py
--rw-r--r--   0 root         (0) root         (0)      498 2022-06-16 15:22:29.000000 worf-0.5.8/worf/lookups.py
--rw-r--r--   0 root         (0) root         (0)      354 2022-02-23 09:19:00.000000 worf-0.5.8/worf/permissions.py
--rw-r--r--   0 root         (0) root         (0)     1049 2022-02-23 09:19:00.000000 worf-0.5.8/worf/renderers.py
--rw-r--r--   0 root         (0) root         (0)     3254 2022-06-16 15:22:29.000000 worf-0.5.8/worf/serializers.py
--rw-r--r--   0 root         (0) root         (0)      465 2022-02-23 09:19:00.000000 worf-0.5.8/worf/settings.py
--rw-r--r--   0 root         (0) root         (0)      380 2022-02-23 09:19:00.000000 worf-0.5.8/worf/shortcuts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-16 15:29:12.209485 worf-0.5.8/worf/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-16 15:29:12.592635 worf-0.5.8/worf/templates/worf/
--rw-r--r--   0 root         (0) root         (0)      106 2022-02-23 09:19:00.000000 worf-0.5.8/worf/templates/worf/api.html
--rw-r--r--   0 root         (0) root         (0)     3190 2022-04-29 08:37:43.000000 worf-0.5.8/worf/templates/worf/base.html
--rw-r--r--   0 root         (0) root         (0)     1111 2022-02-23 09:19:00.000000 worf-0.5.8/worf/testing.py
--rw-r--r--   0 root         (0) root         (0)     8044 2022-06-16 15:22:29.000000 worf-0.5.8/worf/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-16 15:29:12.649352 worf-0.5.8/worf/views/
--rw-r--r--   0 root         (0) root         (0)      333 2022-02-23 09:19:00.000000 worf-0.5.8/worf/views/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7871 2022-06-16 15:22:29.000000 worf-0.5.8/worf/views/base.py
--rw-r--r--   0 root         (0) root         (0)      787 2022-06-16 15:22:29.000000 worf-0.5.8/worf/views/create.py
--rw-r--r--   0 root         (0) root         (0)      260 2022-02-23 09:19:00.000000 worf-0.5.8/worf/views/delete.py
--rw-r--r--   0 root         (0) root         (0)     1043 2022-06-16 15:22:29.000000 worf-0.5.8/worf/views/detail.py
--rw-r--r--   0 root         (0) root         (0)     8606 2022-06-16 15:22:29.000000 worf-0.5.8/worf/views/list.py
--rw-r--r--   0 root         (0) root         (0)      858 2022-06-16 15:22:29.000000 worf-0.5.8/worf/views/update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-16 15:29:12.575168 worf-0.5.8/worf.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15597 2022-06-16 15:29:11.000000 worf-0.5.8/worf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      988 2022-06-16 15:29:12.000000 worf-0.5.8/worf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-16 15:29:11.000000 worf-0.5.8/worf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-07 10:32:16.000000 worf-0.5.8/worf.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       65 2022-06-16 15:29:12.000000 worf-0.5.8/worf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2022-06-16 15:29:12.000000 worf-0.5.8/worf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-24 15:55:34.929518 worf-0.5.9/
+-rw-r--r--   0 root         (0) root         (0)    10758 2022-06-24 15:52:24.000000 worf-0.5.9/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2022-02-04 06:42:11.000000 worf-0.5.9/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      176 2022-02-04 06:42:11.000000 worf-0.5.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    15596 2022-06-24 15:55:34.932053 worf-0.5.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14637 2022-06-24 15:52:01.000000 worf-0.5.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      206 2022-02-22 16:46:06.000000 worf-0.5.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      443 2022-06-24 15:55:34.936425 worf-0.5.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1985 2022-02-04 06:42:11.000000 worf-0.5.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-24 15:55:34.633617 worf-0.5.9/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-04 06:42:11.000000 worf-0.5.9/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2006 2022-05-04 09:05:10.000000 worf-0.5.9/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2022-02-04 06:42:11.000000 worf-0.5.9/tests/factories.py
+-rw-r--r--   0 root         (0) root         (0)     2634 2022-06-24 15:52:01.000000 worf-0.5.9/tests/models.py
+-rw-r--r--   0 root         (0) root         (0)     2256 2022-06-24 15:52:01.000000 worf-0.5.9/tests/serializers.py
+-rw-r--r--   0 root         (0) root         (0)      811 2022-02-04 06:42:11.000000 worf-0.5.9/tests/test_browsable_api.py
+-rw-r--r--   0 root         (0) root         (0)     1069 2022-02-04 06:42:11.000000 worf-0.5.9/tests/test_casing.py
+-rw-r--r--   0 root         (0) root         (0)      233 2022-02-04 06:42:11.000000 worf-0.5.9/tests/test_conf.py
+-rw-r--r--   0 root         (0) root         (0)      924 2022-02-04 06:42:11.000000 worf-0.5.9/tests/test_permissions.py
+-rw-r--r--   0 root         (0) root         (0)      130 2022-02-04 06:42:11.000000 worf-0.5.9/tests/test_shortcuts.py
+-rw-r--r--   0 root         (0) root         (0)     3239 2022-06-24 15:52:01.000000 worf-0.5.9/tests/test_validators.py
+-rw-r--r--   0 root         (0) root         (0)    17109 2022-06-24 15:52:01.000000 worf-0.5.9/tests/test_views.py
+-rw-r--r--   0 root         (0) root         (0)      428 2022-02-04 06:42:11.000000 worf-0.5.9/tests/urls.py
+-rw-r--r--   0 root         (0) root         (0)     2111 2022-06-24 15:52:01.000000 worf-0.5.9/tests/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-24 15:55:34.762307 worf-0.5.9/worf/
+-rw-r--r--   0 root         (0) root         (0)       23 2022-06-24 15:52:24.000000 worf-0.5.9/worf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3457 2022-06-16 15:34:07.000000 worf-0.5.9/worf/assigns.py
+-rw-r--r--   0 root         (0) root         (0)     1137 2022-06-16 15:34:07.000000 worf-0.5.9/worf/casing.py
+-rw-r--r--   0 root         (0) root         (0)      159 2022-06-16 15:34:07.000000 worf-0.5.9/worf/conf.py
+-rw-r--r--   0 root         (0) root         (0)      981 2022-06-24 15:52:01.000000 worf-0.5.9/worf/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1842 2022-06-24 15:52:01.000000 worf-0.5.9/worf/fields.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2022-06-16 15:34:07.000000 worf-0.5.9/worf/filters.py
+-rw-r--r--   0 root         (0) root         (0)      498 2022-06-16 15:34:07.000000 worf-0.5.9/worf/lookups.py
+-rw-r--r--   0 root         (0) root         (0)      354 2022-06-16 15:34:07.000000 worf-0.5.9/worf/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     1049 2022-06-16 15:34:07.000000 worf-0.5.9/worf/renderers.py
+-rw-r--r--   0 root         (0) root         (0)     4518 2022-06-24 15:52:01.000000 worf-0.5.9/worf/serializers.py
+-rw-r--r--   0 root         (0) root         (0)      465 2022-06-16 15:34:08.000000 worf-0.5.9/worf/settings.py
+-rw-r--r--   0 root         (0) root         (0)      380 2022-06-16 15:34:08.000000 worf-0.5.9/worf/shortcuts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-24 15:55:34.421445 worf-0.5.9/worf/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-24 15:55:34.875253 worf-0.5.9/worf/templates/worf/
+-rw-r--r--   0 root         (0) root         (0)      106 2022-06-16 15:34:08.000000 worf-0.5.9/worf/templates/worf/api.html
+-rw-r--r--   0 root         (0) root         (0)     3190 2022-06-16 15:34:08.000000 worf-0.5.9/worf/templates/worf/base.html
+-rw-r--r--   0 root         (0) root         (0)     1111 2022-06-16 15:34:08.000000 worf-0.5.9/worf/testing.py
+-rw-r--r--   0 root         (0) root         (0)     8097 2022-06-24 15:52:01.000000 worf-0.5.9/worf/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-24 15:55:34.925690 worf-0.5.9/worf/views/
+-rw-r--r--   0 root         (0) root         (0)      333 2022-06-16 15:34:08.000000 worf-0.5.9/worf/views/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7322 2022-06-24 15:52:01.000000 worf-0.5.9/worf/views/base.py
+-rw-r--r--   0 root         (0) root         (0)      856 2022-06-24 15:52:01.000000 worf-0.5.9/worf/views/create.py
+-rw-r--r--   0 root         (0) root         (0)      283 2022-06-24 15:52:01.000000 worf-0.5.9/worf/views/delete.py
+-rw-r--r--   0 root         (0) root         (0)      638 2022-06-24 15:52:01.000000 worf-0.5.9/worf/views/detail.py
+-rw-r--r--   0 root         (0) root         (0)     8019 2022-06-24 15:52:01.000000 worf-0.5.9/worf/views/list.py
+-rw-r--r--   0 root         (0) root         (0)      880 2022-06-24 15:52:01.000000 worf-0.5.9/worf/views/update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-24 15:55:34.855181 worf-0.5.9/worf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15596 2022-06-24 15:55:34.000000 worf-0.5.9/worf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      988 2022-06-24 15:55:34.000000 worf-0.5.9/worf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-24 15:55:34.000000 worf-0.5.9/worf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-02-07 10:32:16.000000 worf-0.5.9/worf.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       65 2022-06-24 15:55:34.000000 worf-0.5.9/worf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2022-06-24 15:55:34.000000 worf-0.5.9/worf.egg-info/top_level.txt
```

### Comparing `worf-0.5.8/CHANGELOG.md` & `worf-0.5.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
+### [0.5.9](https://github.com/gundotio/worf/compare/v0.5.8...v0.5.9) (2022-06-24)
+
+- Strip support for legacy serializers [#96](https://github.com/gundotio/worf/pull/96)
+- Pass request + args + kwargs to view CRUD methods
+- Support fields param on detail endpoints in addition to lists
+- Apply fields param filtering in the serialization step
+- Serializer `__call__` now honors only/exclude rules from its predecessors
+
 ### [0.5.8](https://github.com/gundotio/worf/compare/v0.5.7...v0.5.8) (2022-06-16)
 
 - Add queryset support to `Pluck` field
 - Flatten validation checks and don't return `True`
 - Raise `DoesNotExist` for related models
 - Rename `CreateAPI` method `get_instance` to `new_instance`
 - Serializer context support via `get_serializer_context()`
```

### Comparing `worf-0.5.8/LICENSE.md` & `worf-0.5.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `worf-0.5.8/PKG-INFO` & `worf-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: worf
-Version: 0.5.8
+Version: 0.5.9
 Summary: Wade's own REST Framework: A more Djangonic approach to REST APIs
 Home-page: https://github.com/gundotio/worf
 Author: Wade Williams
 Author-email: wade@wadewilliams.com
 License: MIT
 Keywords: django,rest,framework,api
 Classifier: Development Status :: 4 - Beta
@@ -217,15 +217,15 @@
 
 
 Validators
 -----------
 
 Validation handling can be found in `worf.validators`.
 
-The basics come from `ValidationMixin` which `AbstractBaseAPI` inherits from, it
+The basics come from `ValidateFields` which `AbstractBaseAPI` inherits from, it
 performs some coercion on `self.bundle`, potentially resulting in a different
 bundle than what was originally passed to the view.
 
 
 Views
 -----
```

### Comparing `worf-0.5.8/README.md` & `worf-0.5.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 
 
 Validators
 -----------
 
 Validation handling can be found in `worf.validators`.
 
-The basics come from `ValidationMixin` which `AbstractBaseAPI` inherits from, it
+The basics come from `ValidateFields` which `AbstractBaseAPI` inherits from, it
 performs some coercion on `self.bundle`, potentially resulting in a different
 bundle than what was originally passed to the view.
 
 
 Views
 -----
```

### Comparing `worf-0.5.8/setup.py` & `worf-0.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `worf-0.5.8/tests/conftest.py` & `worf-0.5.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `worf-0.5.8/tests/factories.py` & `worf-0.5.9/tests/factories.py`

 * *Files identical despite different names*

### Comparing `worf-0.5.8/tests/models.py` & `worf-0.5.9/tests/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from hashlib import md5
 from uuid import uuid4
 
 from django.db import models
 from django.contrib.auth.models import User
 
 
 class Profile(models.Model):
@@ -22,39 +23,27 @@
     role = models.ForeignKey("Role", on_delete=models.CASCADE)
     team = models.ForeignKey("Team", blank=True, null=True, on_delete=models.SET_NULL)
     skills = models.ManyToManyField("Skill", through="RatedSkill")
     tags = models.ManyToManyField("Tag")
 
     recovery_email = models.EmailField(blank=True, max_length=320, null=True)
     recovery_phone = models.CharField(blank=True, max_length=32, null=True)
+    resume = models.FileField(upload_to="resumes/", blank=True)
 
     last_active = models.DateField(blank=True, null=True)
     created_at = models.DateTimeField(blank=True, null=True)
 
-    def api(self):
-        return dict(id=self.id, email=self.email, phone=self.phone)
+    def get_avatar_url(self):
+        return self.avatar.url if self.avatar else self.get_gravatar_url()
 
-    def api_update_fields(self):
-        return [
-            "id",
-            "email",
-            "phone",
-
-            "boolean",
-            "integer",
-            "json",
-            "positive_integer",
-            "slug",
-            "small_integer",
-
-            "recovery_email",
-
-            "last_active",
-            "created_at",
-        ]
+    def get_gravatar_hash(self):
+        return md5(self.user.email.lower().encode()).hexdigest()
+
+    def get_gravatar_url(self, default="identicon", size=512):
+        return f"https://www.gravatar.com/avatar/{self.get_gravatar_hash()}?d={default}&s={size}"
 
 
 class Role(models.Model):
     name = models.CharField(max_length=100)
 
 
 class Skill(models.Model):
```

### Comparing `worf-0.5.8/tests/test_browsable_api.py` & `worf-0.5.9/tests/test_browsable_api.py`

 * *Files identical despite different names*

### Comparing `worf-0.5.8/tests/test_casing.py` & `worf-0.5.9/tests/test_casing.py`

 * *Files identical despite different names*

### Comparing `worf-0.5.8/tests/test_permissions.py` & `worf-0.5.9/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `worf-0.5.8/tests/test_validators.py` & `worf-0.5.9/tests/test_validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
         recovery_email=email,
         recovery_phone=phone,
         last_active=now.date().isoformat(),
         created_at=now.isoformat(),
     ))
     view.request = RequestFactory().patch(f"/{uuid}/")
     view.kwargs = dict(id=str(uuid))
-    view.serializer = None
     return view
 
 
 def test_validate_bundle(profile_view):
     profile_view.validate_bundle("id")
     profile_view.validate_bundle("email")
     profile_view.validate_bundle("phone")
```

### Comparing `worf-0.5.8/tests/test_views.py` & `worf-0.5.9/tests/test_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,21 +142,21 @@
     assert result["role"]["name"] == role.name
     assert result["user"]["username"] == user.username
 
 
 @patch('django.core.files.storage.FileSystemStorage.save')
 @pytest.mark.parametrize("method", ["PATCH", "PUT"])
 def test_profile_multipart_update(mock_save, client, db, method, profile, role, user):
-    avatar = SimpleUploadedFile("avatar.jpg", b"", content_type="image/jpeg")
-    mock_save.return_value = "avatar.jpg"
-    payload = dict(avatar=avatar, role=role.pk, user=user.pk)
+    resume = SimpleUploadedFile("resume.pdf", b"", content_type="application/pdf")
+    mock_save.return_value = "resume.pdf"
+    payload = dict(resume=resume, role=role.pk, user=user.pk)
     response = client.generic(method, f"/profiles/{profile.pk}/", payload)
     result = response.json()
     assert response.status_code == 200, result
-    assert result["avatar"] == "/avatar.jpg"
+    assert result["resume"] == "/resume.pdf"
     assert result["role"]["id"] == role.pk
     assert result["role"]["name"] == role.name
     assert result["user"]["username"] == user.username
 
 
 @pytest.mark.parametrize("method", ["PATCH", "PUT"])
 def test_profile_update_fk(client, db, method, profile, role, team):
@@ -281,25 +281,45 @@
     assert "Invalid skills" in result["message"]
 
 
 def test_user_detail(client, db, user):
     response = client.get(f"/users/{user.pk}/")
     result = response.json()
     assert response.status_code == 200, result
+    assert result["id"] == user.pk
     assert result["username"] == user.username
 
 
+def test_user_detail_fields(client, db, user):
+    response = client.get(f"/users/{user.pk}/?fields=username")
+    result = response.json()
+    assert response.status_code == 200, result
+    assert result == dict(username=user.username)
+
+
 def test_user_list(client, db, user):
     response = client.get("/users/")
     result = response.json()
     assert response.status_code == 200, result
     assert len(result["users"]) == 1
+    assert result["users"][0]["id"] == user.pk
     assert result["users"][0]["username"] == user.username
 
 
+def test_user_list_fields(client, db, user):
+    response = client.get("/users/?fields=username")
+    result = response.json()
+    assert response.status_code == 200, result
+    assert result["users"] == [dict(username=user.username)]
+    response = client.get("/users/?fields=invalid")
+    result = response.json()
+    assert response.status_code == 400, result
+    assert result == dict(message="Invalid fields: OrderedSet(['invalid'])")
+
+
 def test_user_list_filters(client, db, user_factory):
     january = "2021-01-01T00:00:00Z"
     february = "2021-02-01T00:00:00Z"
     march = "2021-03-01T00:00:00Z"
 
     user1 = user_factory.create(date_joined=january)
     user2 = user_factory.create(date_joined=february)
```

### Comparing `worf-0.5.8/tests/views.py` & `worf-0.5.9/tests/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         return "+5555555555"
 
 
 class UserList(CreateAPI, ListAPI):
     model = User
     ordering = ["pk"]
     serializer = UserSerializer(only=[
+        "id",
         "username",
         "date_joined",
         "email",
     ])
     permissions = [PublicEndpoint]
     filter_fields = [
         "email",
@@ -74,9 +75,9 @@
         "id",
         "date_joined",
     ]
 
 
 class UserDetail(UpdateAPI, DetailAPI):
     model = User
-    serializer = UserSerializer
+    serializer = UserSerializer(exclude=["date_joined"])
     permissions = [PublicEndpoint]
```

### Comparing `worf-0.5.8/worf/assigns.py` & `worf-0.5.9/worf/assigns.py`

 * *Files identical despite different names*

### Comparing `worf-0.5.8/worf/casing.py` & `worf-0.5.9/worf/casing.py`

 * *Files identical despite different names*

### Comparing `worf-0.5.8/worf/exceptions.py` & `worf-0.5.9/worf/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 class HTTPException(Exception):
     def __init__(self, message=None):
         super().__init__(message)
-        if message is not None:
-            self.message = message
+        self.message = message or self.message
 
 
 class HTTP400(HTTPException):
     message = "Bad Request"
     status = 400
 
 
@@ -43,13 +42,17 @@
 HTTP_EXCEPTIONS = (HTTP400, HTTP401, HTTP404, HTTP409, HTTP410, HTTP420, HTTP422)
 
 
 class NamingThingsError(ValueError):
     pass
 
 
-class PermissionsException(Exception):
+class PermissionsError(Exception):
     pass
 
 
 class NotImplementedInWorfYet(NotImplementedError):
     pass
+
+
+class SerializerError(ValueError):
+    pass
```

### Comparing `worf-0.5.8/worf/filters.py` & `worf-0.5.9/worf/filters.py`

 * *Files identical despite different names*

### Comparing `worf-0.5.8/worf/renderers.py` & `worf-0.5.9/worf/renderers.py`

 * *Files identical despite different names*

### Comparing `worf-0.5.8/worf/templates/worf/base.html` & `worf-0.5.9/worf/templates/worf/base.html`

 * *Files identical despite different names*

### Comparing `worf-0.5.8/worf/testing.py` & `worf-0.5.9/worf/testing.py`

 * *Files identical despite different names*

### Comparing `worf-0.5.8/worf/validators.py` & `worf-0.5.9/worf/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from django.db import models
 from django.utils.dateparse import parse_datetime
 
 from worf.conf import settings
 from worf.exceptions import NotImplementedInWorfYet
 
 
-class ValidationMixin:
+class ValidateFields:
     boolean_values = {
         "1": True,
         "0": False,
         "true": True,
         "false": False,
     }
 
@@ -155,18 +155,19 @@
 
         Side Effects:
         As various bundle objects are parsed and validated, we reset the bundle.
         This may result in self.bundle changes.
 
         We expect to set a fully validated bundle keys and values.
         """
-        serializer = self.get_serializer()
+        serializer = self.load_serializer()
+        write_fields = list(serializer.load_fields.keys())
         write_methods = ("PATCH", "POST", "PUT")
 
-        if self.request.method in write_methods and key not in serializer.write():
+        if self.request.method in write_methods and key not in write_fields:
             message = f"{self.keymap[key]} is not editable"
             if settings.WORF_DEBUG:
                 message += f":: {serializer}"
             raise ValidationError(message)
 
         annotation = (
             self.get_queryset().query.annotations.get(key)
```

### Comparing `worf-0.5.8/worf/views/base.py` & `worf-0.5.9/worf/views/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,18 +13,25 @@
 from django.template.defaultfilters import filesizeformat
 from django.utils.decorators import method_decorator
 from django.views import View
 from django.views.decorators.cache import never_cache
 
 from worf.casing import camel_to_snake, snake_to_camel
 from worf.conf import settings
-from worf.exceptions import HTTP404, HTTP422, HTTP_EXCEPTIONS, PermissionsException
+from worf.exceptions import (
+    HTTP400,
+    HTTP404,
+    HTTP422,
+    HTTP_EXCEPTIONS,
+    PermissionsError,
+    SerializerError,
+)
 from worf.renderers import render_response
-from worf.serializers import LegacySerializer
-from worf.validators import ValidationMixin
+from worf.serializers import SerializeModels
+from worf.validators import ValidateFields
 
 
 @method_decorator(never_cache, name="dispatch")
 class APIResponse(View):
     def __init__(self, *args, **kwargs):
         self.codepath = f"{self.__module__}.{self.__class__.__name__}"
         return super().__init__(*args, **kwargs)
@@ -40,20 +47,17 @@
             msg = f"{self.codepath} did not pass an object to "
             msg += "render_to_response, nor did its serializer method"
             raise ImproperlyConfigured(msg)
 
         return render_response(self.request, data, status_code)
 
 
-class AbstractBaseAPI(APIResponse, ValidationMixin):
+class AbstractBaseAPI(APIResponse, SerializeModels, ValidateFields):
     model = None
     permissions = []
-    api_method = "api"
-    serializer = None
-    staff_serializer = None
     payload_key = None
 
     def __init__(self, *args, **kwargs):
         self.codepath = f"{self.__module__}.{self.__class__.__name__}"
 
         if self.model is None:
             raise ImproperlyConfigured(f"Model is not set on {self.codepath}")
@@ -81,24 +85,56 @@
     @property
     def name(self):
         if isinstance(self.payload_key, str):
             return self.payload_key
         verbose_name_plural = self.model._meta.verbose_name_plural
         return snake_to_camel(verbose_name_plural.replace(" ", "_").lower())
 
+    def dispatch(self, request, *args, **kwargs):
+        method = request.method.lower()
+        handler = self.http_method_not_allowed
+
+        if method in self.http_method_names:
+            handler = getattr(self, method, self.http_method_not_allowed)
+
+        try:
+            self._check_permissions()  # only returns 200 or HTTP_EXCEPTIONS
+            self.set_bundle_from_request(request)
+            return handler(request, *args, **kwargs)  # calls self.serialize()
+        except HTTP_EXCEPTIONS as e:
+            message = e.message
+            status = e.status
+        except ObjectDoesNotExist as e:
+            if self.model and not isinstance(e, self.model.DoesNotExist):
+                raise e
+            message = HTTP404.message
+            status = HTTP404.status
+        except RequestDataTooBig:
+            self.request._body = self.request.read(None)  # prevent further raises
+            message = f"Max upload size is {filesizeformat(settings.DATA_UPLOAD_MAX_MEMORY_SIZE)}"
+            status = HTTP422.status
+        except SerializerError as e:
+            message = str(e)
+            status = HTTP400.status
+        except ValidationError as e:
+            message = e.message
+            status = HTTP422.status
+
+        return self.render_to_response(dict(message=message), status)
+
     def _check_permissions(self):
         """Return a permissions exception when in debug mode instead of 404."""
         for method in self.permissions:
             permission_func = getattr(self, method.__name__)
             response = permission_func(self.request)
             if response == 200:
                 continue
 
             if settings.WORF_DEBUG:
-                raise PermissionsException(
+                raise PermissionsError(
                     "Permissions function {}.{} returned {}. You'd normally see a 404 here but WORF_DEBUG=True.".format(
                         method.__module__, method.__name__, response
                     )
                 )
 
             try:
                 raise response
@@ -111,28 +147,14 @@
 
     def get_instance(self):
         return self.instance if hasattr(self, "instance") else None
 
     def get_related_model(self, field):
         return self.model._meta.get_field(field).related_model
 
-    def get_serializer(self):
-        context = dict(request=self.request, **self.get_serializer_context())
-        if self.staff_serializer and self.request.user.is_staff:
-            return self.staff_serializer(context=context)
-        if self.serializer:
-            return self.serializer(context=context)
-        if self.api_method:
-            return LegacySerializer(self.model, self.api_method)
-        msg = f"{type(self).__name__}.get_serializer() did not return a serializer"
-        raise ImproperlyConfigured(msg)
-
-    def get_serializer_context(self):
-        return {}
-
     def flatten_bundle(self, raw_bundle):
         # parse_qs gives us a dictionary where all values are lists
         return {
             key: value[0] if len(value) == 1 else value
             for key, value in raw_bundle.items()
         }
 
@@ -187,33 +209,7 @@
         elif request.body:
             try:
                 raw_bundle = json.loads(request.body)
             except json.decoder.JSONDecodeError:
                 pass
 
         self.set_bundle(raw_bundle)
-
-    def dispatch(self, request, *args, **kwargs):
-        method = request.method.lower()
-        handler = self.http_method_not_allowed
-
-        if method in self.http_method_names:
-            handler = getattr(self, method, self.http_method_not_allowed)
-
-        try:
-            self._check_permissions()  # only returns 200 or HTTP_EXCEPTIONS
-            self.set_bundle_from_request(request)
-            return handler(request, *args, **kwargs)  # calls self.serialize()
-        except HTTP_EXCEPTIONS as e:
-            return self.render_to_response(dict(message=e.message), e.status)
-        except ObjectDoesNotExist as e:
-            if self.model and not isinstance(e, self.model.DoesNotExist):
-                raise e
-            return self.render_to_response(
-                dict(message=HTTP404.message), HTTP404.status
-            )
-        except RequestDataTooBig:
-            self.request._body = self.request.read(None)  # prevent further raises
-            message = f"Max upload size is {filesizeformat(settings.DATA_UPLOAD_MAX_MEMORY_SIZE)}"
-            return self.render_to_response(dict(message=message), HTTP422.status)
-        except ValidationError as e:
-            return self.render_to_response(dict(message=e.message), HTTP422.status)
```

### Comparing `worf-0.5.8/worf/views/create.py` & `worf-0.5.9/worf/views/update.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from worf.assigns import AssignAttributes
+from worf.lookups import FindInstance
 from worf.views.base import AbstractBaseAPI
 
 
-class CreateAPI(AssignAttributes, AbstractBaseAPI):
-    create_serializer = None
-
-    def create(self):
-        self.instance = self.new_instance()
-        self.validate()
-        self.save(self.instance, self.bundle)
-        self.instance.refresh_from_db()
-        return self.instance
+class UpdateAPI(AssignAttributes, FindInstance, AbstractBaseAPI):
+    update_serializer = None
 
     def get_serializer(self):
-        if self.create_serializer and self.request.method == "POST":
-            return self.create_serializer(context=self.get_serializer_context())
+        if self.update_serializer and self.request.method in ("PATCH", "PUT"):
+            return self.update_serializer(**self.get_serializer_kwargs())
         return super().get_serializer()
 
-    def new_instance(self):
-        return self.model()
+    def patch(self, *args, **kwargs):
+        self.update(*args, **kwargs)
+        return self.render_to_response()
+
+    def put(self, *args, **kwargs):
+        self.update(*args, **kwargs)
+        return self.render_to_response()
 
-    def post(self, request, *args, **kwargs):
-        return self.render_to_response(self.get_serializer().read(self.create()), 201)
+    def update(self, *args, **kwargs):
+        instance = self.get_instance()
+        self.validate()
+        self.save(instance, self.bundle)
+        instance.refresh_from_db()
+        return instance
```

### Comparing `worf-0.5.8/worf/views/detail.py` & `worf-0.5.9/worf/views/detail.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,22 @@
-from django.core.exceptions import ImproperlyConfigured
-
 from worf.lookups import FindInstance
 from worf.views.base import AbstractBaseAPI
 from worf.views.update import UpdateAPI
 
 
 class DetailAPI(FindInstance, AbstractBaseAPI):
     detail_serializer = None
 
-    def get(self, request, *args, **kwargs):
+    def get(self, *args, **kwargs):
         return self.render_to_response()
 
     def get_serializer(self):
         if self.detail_serializer and self.request.method == "GET":
-            return self.detail_serializer(context=self.get_serializer_context())
+            return self.detail_serializer(**self.get_serializer_kwargs())
         return super().get_serializer()
 
     def serialize(self):
-        """Return the model api, used for responses."""
-        serializer = self.get_serializer()
-        payload = serializer.read(self.get_instance())
-        if not isinstance(payload, dict):
-            raise ImproperlyConfigured(f"{serializer} did not return a dictionary")
-        return payload
+        return self.load_serializer().dump(self.get_instance())
 
 
 class DetailUpdateAPI(UpdateAPI, DetailAPI):
-    def patch(self, request, *args, **kwargs):
-        self.update()
-        return self.get(request)
+    pass
```

### Comparing `worf-0.5.8/worf/views/list.py` & `worf-0.5.9/worf/views/list.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         # support deprecated search_fields and/or dict syntax (note that `and` does nothing)
         if isinstance(self.search_fields, dict):  # pragma: no cover - deprecated
             warnings.warn(
                 f"Passing a dict to {codepath}.search_fields is deprecated. Pass a list instead."
             )
             self.search_fields = self.search_fields.get("or", [])
 
-    def get(self, request, *args, **kwargs):
+    def get(self, *args, **kwargs):
         return self.render_to_response()
 
     def _set_base_lookup_kwargs(self):
         # Filters set directly on the class
         self.lookup_kwargs.update(self.filters)
 
         # Filters set via URL
@@ -171,15 +171,15 @@
         return ordering or self.ordering
 
     def get_sort_field(self, field, descending=False):
         return OrderBy(F(field), descending=descending)
 
     def get_serializer(self):
         if self.list_serializer and self.request.method == "GET":
-            return self.list_serializer(context=self.get_serializer_context())
+            return self.list_serializer(**self.get_serializer_kwargs())
         return super().get_serializer()
 
     def paginated_results(self):
         queryset = self.get_processed_queryset()
         request = self.request
 
         if settings.WORF_DEBUG:
@@ -201,58 +201,37 @@
         self.count = paginator.count
 
         try:
             return paginator.page(self.page_num)
         except EmptyPage:
             return []
 
-    def specific_fields(self, result):
-        fields = self.bundle.get("fields", [])
-        if fields:
-            return {key: value for key, value in result.items() if key in fields}
-        return result
-
     def serialize(self):
-        serializer = self.get_serializer()
+        serializer = self.load_serializer()
 
-        payload = {
-            str(self.name): [
-                self.specific_fields(serializer.read(instance))
-                for instance in self.paginated_results()
-            ]
-        }
+        payload = {str(self.name): serializer(many=True).dump(self.paginated_results())}
 
         if self.per_page:
             payload.update(
                 {
                     "pagination": dict(
                         count=self.count,
                         pages=self.num_pages,
                         page=self.page_num,
                     )
                 }
             )
 
-        if not settings.WORF_DEBUG:
-            return payload
-
-        if not hasattr(self, "lookup_kwargs"):
-            # Debug throws an error in the event there are no lookup_kwargs
-            self.lookup_kwargs = {}
-
-        payload.update(
-            {
-                "debug": {
-                    "bundle": self.bundle,
-                    "lookup_kwargs": self.lookup_kwargs,
-                    "query": self.query,
-                    "search_query": str(self.search_query),
-                    "serializer": str(serializer).strip("<>"),
-                }
+        if settings.WORF_DEBUG:
+            payload["debug"] = {
+                "bundle": self.bundle,
+                "lookup_kwargs": getattr(self, "lookup_kwargs", {}),
+                "query": self.query,
+                "search_query": str(self.search_query),
+                "serializer": str(serializer).strip("<>"),
             }
-        )
 
         return payload
 
 
 class ListCreateAPI(CreateAPI, ListAPI):
     pass
```

### Comparing `worf-0.5.8/worf/views/update.py` & `worf-0.5.9/worf/views/create.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from worf.assigns import AssignAttributes
-from worf.lookups import FindInstance
 from worf.views.base import AbstractBaseAPI
 
 
-class UpdateAPI(AssignAttributes, FindInstance, AbstractBaseAPI):
-    update_serializer = None
+class CreateAPI(AssignAttributes, AbstractBaseAPI):
+    create_serializer = None
+
+    def create(self, *args, **kwargs):
+        self.instance = self.new_instance()
+        self.validate()
+        self.save(self.instance, self.bundle)
+        self.instance.refresh_from_db()
+        return self.instance
 
     def get_serializer(self):
-        if self.update_serializer and self.request.method in ("PATCH", "PUT"):
-            return self.update_serializer(context=self.get_serializer_context())
+        if self.create_serializer and self.request.method == "POST":
+            return self.create_serializer(**self.get_serializer_kwargs())
         return super().get_serializer()
 
-    def patch(self, request, *args, **kwargs):
-        self.update()
-        return self.render_to_response()
-
-    def put(self, request, *args, **kwargs):
-        self.update()
-        return self.render_to_response()
+    def new_instance(self):
+        return self.model()
 
-    def update(self):
-        instance = self.get_instance()
-        self.validate()
-        self.save(instance, self.bundle)
-        instance.refresh_from_db()
-        return instance
+    def post(self, *args, **kwargs):
+        instance = self.create(*args, **kwargs)
+        result = self.load_serializer().dump(instance)
+        return self.render_to_response(result, 201)
```

### Comparing `worf-0.5.8/worf.egg-info/PKG-INFO` & `worf-0.5.9/worf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: worf
-Version: 0.5.8
+Version: 0.5.9
 Summary: Wade's own REST Framework: A more Djangonic approach to REST APIs
 Home-page: https://github.com/gundotio/worf
 Author: Wade Williams
 Author-email: wade@wadewilliams.com
 License: MIT
 Keywords: django,rest,framework,api
 Classifier: Development Status :: 4 - Beta
@@ -217,15 +217,15 @@
 
 
 Validators
 -----------
 
 Validation handling can be found in `worf.validators`.
 
-The basics come from `ValidationMixin` which `AbstractBaseAPI` inherits from, it
+The basics come from `ValidateFields` which `AbstractBaseAPI` inherits from, it
 performs some coercion on `self.bundle`, potentially resulting in a different
 bundle than what was originally passed to the view.
 
 
 Views
 -----
```

### Comparing `worf-0.5.8/worf.egg-info/SOURCES.txt` & `worf-0.5.9/worf.egg-info/SOURCES.txt`

 * *Files identical despite different names*


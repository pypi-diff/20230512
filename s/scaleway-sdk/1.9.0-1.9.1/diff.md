# Comparing `tmp/scaleway-sdk-1.9.0.tar.gz` & `tmp/scaleway-sdk-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scaleway-sdk-1.9.0.tar", last modified: Thu Jul  4 14:51:11 2019, max compression
+gzip compressed data, was "dist/scaleway-sdk-1.9.1.tar", last modified: Mon Sep  9 16:25:27 2019, max compression
```

## Comparing `scaleway-sdk-1.9.0.tar` & `scaleway-sdk-1.9.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 jquere     (501) admin       (80)        0 2019-07-04 14:51:11.000000 scaleway-sdk-1.9.0/
--rw-r--r--   0 jquere     (501) admin       (80)     8961 2019-07-04 09:58:27.000000 scaleway-sdk-1.9.0/CHANGES.rst
--rw-r--r--   0 jquere     (501) admin       (80)     9311 2019-07-04 14:51:11.000000 scaleway-sdk-1.9.0/PKG-INFO
--rw-r--r--   0 jquere     (501) admin       (80)     1391 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.0/LICENSE
--rwxr-xr-x   0 jquere     (501) admin       (80)     5229 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.0/setup.py
-drwxr-xr-x   0 jquere     (501) admin       (80)        0 2019-07-04 14:51:11.000000 scaleway-sdk-1.9.0/scaleway_sdk.egg-info/
--rw-r--r--   0 jquere     (501) admin       (80)     9311 2019-07-04 14:51:10.000000 scaleway-sdk-1.9.0/scaleway_sdk.egg-info/PKG-INFO
--rw-r--r--   0 jquere     (501) admin       (80)       20 2019-07-04 14:51:10.000000 scaleway-sdk-1.9.0/scaleway_sdk.egg-info/entry_points.txt
--rw-r--r--   0 jquere     (501) admin       (80)      193 2019-07-04 14:51:10.000000 scaleway-sdk-1.9.0/scaleway_sdk.egg-info/requires.txt
--rw-r--r--   0 jquere     (501) admin       (80)        9 2019-07-04 14:51:10.000000 scaleway-sdk-1.9.0/scaleway_sdk.egg-info/top_level.txt
--rw-r--r--   0 jquere     (501) admin       (80)      695 2019-07-04 14:51:10.000000 scaleway-sdk-1.9.0/scaleway_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 jquere     (501) admin       (80)        1 2019-07-04 14:51:10.000000 scaleway-sdk-1.9.0/scaleway_sdk.egg-info/dependency_links.txt
-drwxr-xr-x   0 jquere     (501) admin       (80)        0 2019-07-04 14:51:11.000000 scaleway-sdk-1.9.0/scaleway/
-drwxr-xr-x   0 jquere     (501) admin       (80)        0 2019-07-04 14:51:11.000000 scaleway-sdk-1.9.0/scaleway/apis/
--rw-r--r--   0 jquere     (501) admin       (80)      258 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.0/scaleway/apis/api_billing.py
--rw-r--r--   0 jquere     (501) admin       (80)     5700 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.0/scaleway/apis/__init__.py
--rw-r--r--   0 jquere     (501) admin       (80)     1194 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.0/scaleway/apis/api_metadata.py
--rw-r--r--   0 jquere     (501) admin       (80)     7208 2019-07-03 19:08:27.000000 scaleway-sdk-1.9.0/scaleway/apis/api_account.py
--rw-r--r--   0 jquere     (501) admin       (80)     1321 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.0/scaleway/apis/api_compute.py
-drwxr-xr-x   0 jquere     (501) admin       (80)        0 2019-07-04 14:51:11.000000 scaleway-sdk-1.9.0/scaleway/tests/
-drwxr-xr-x   0 jquere     (501) admin       (80)        0 2019-07-04 14:51:11.000000 scaleway-sdk-1.9.0/scaleway/tests/apis/
--rw-r--r--   0 jquere     (501) admin       (80)     2346 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.0/scaleway/tests/apis/test_api_metadata.py
--rw-r--r--   0 jquere     (501) admin       (80)      225 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.0/scaleway/tests/apis/test_api_billing.py
--rw-r--r--   0 jquere     (501) admin       (80)     1070 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.0/scaleway/tests/apis/__init__.py
--rw-r--r--   0 jquere     (501) admin       (80)    10617 2019-07-03 19:08:27.000000 scaleway-sdk-1.9.0/scaleway/tests/apis/test_api_account.py
--rw-r--r--   0 jquere     (501) admin       (80)      901 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.0/scaleway/tests/apis/test_api_compute.py
--rw-r--r--   0 jquere     (501) admin       (80)     3369 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.0/scaleway/tests/apis/test_api.py
--rw-r--r--   0 jquere     (501) admin       (80)      448 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.0/scaleway/tests/__init__.py
--rw-r--r--   0 jquere     (501) admin       (80)      947 2019-07-04 09:58:27.000000 scaleway-sdk-1.9.0/scaleway/__init__.py
--rw-r--r--   0 jquere     (501) admin       (80)     5929 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.0/README.rst
--rw-r--r--   0 jquere     (501) admin       (80)      649 2019-07-04 14:51:11.000000 scaleway-sdk-1.9.0/setup.cfg
--rw-r--r--   0 jquere     (501) admin       (80)      155 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.0/MANIFEST.in
+drwxr-xr-x   0 jquere     (501) admin       (80)        0 2019-09-09 16:25:27.000000 scaleway-sdk-1.9.1/
+-rw-r--r--   0 jquere     (501) admin       (80)     9211 2019-09-09 16:25:12.000000 scaleway-sdk-1.9.1/CHANGES.rst
+-rw-r--r--   0 jquere     (501) admin       (80)     9339 2019-09-09 16:25:27.000000 scaleway-sdk-1.9.1/PKG-INFO
+-rw-r--r--   0 jquere     (501) admin       (80)     1391 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.1/LICENSE
+-rwxr-xr-x   0 jquere     (501) admin       (80)     5256 2019-09-09 16:21:09.000000 scaleway-sdk-1.9.1/setup.py
+drwxr-xr-x   0 jquere     (501) admin       (80)        0 2019-09-09 16:25:27.000000 scaleway-sdk-1.9.1/scaleway_sdk.egg-info/
+-rw-r--r--   0 jquere     (501) admin       (80)     9339 2019-09-09 16:25:27.000000 scaleway-sdk-1.9.1/scaleway_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 jquere     (501) admin       (80)       20 2019-09-09 16:25:27.000000 scaleway-sdk-1.9.1/scaleway_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 jquere     (501) admin       (80)      211 2019-09-09 16:25:27.000000 scaleway-sdk-1.9.1/scaleway_sdk.egg-info/requires.txt
+-rw-r--r--   0 jquere     (501) admin       (80)        9 2019-09-09 16:25:27.000000 scaleway-sdk-1.9.1/scaleway_sdk.egg-info/top_level.txt
+-rw-r--r--   0 jquere     (501) admin       (80)      695 2019-09-09 16:25:27.000000 scaleway-sdk-1.9.1/scaleway_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jquere     (501) admin       (80)        1 2019-09-09 16:25:27.000000 scaleway-sdk-1.9.1/scaleway_sdk.egg-info/dependency_links.txt
+drwxr-xr-x   0 jquere     (501) admin       (80)        0 2019-09-09 16:25:27.000000 scaleway-sdk-1.9.1/scaleway/
+drwxr-xr-x   0 jquere     (501) admin       (80)        0 2019-09-09 16:25:27.000000 scaleway-sdk-1.9.1/scaleway/apis/
+-rw-r--r--   0 jquere     (501) admin       (80)      258 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.1/scaleway/apis/api_billing.py
+-rw-r--r--   0 jquere     (501) admin       (80)     5700 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.1/scaleway/apis/__init__.py
+-rw-r--r--   0 jquere     (501) admin       (80)     1194 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.1/scaleway/apis/api_metadata.py
+-rw-r--r--   0 jquere     (501) admin       (80)     7281 2019-09-09 16:21:09.000000 scaleway-sdk-1.9.1/scaleway/apis/api_account.py
+-rw-r--r--   0 jquere     (501) admin       (80)     1321 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.1/scaleway/apis/api_compute.py
+drwxr-xr-x   0 jquere     (501) admin       (80)        0 2019-09-09 16:25:27.000000 scaleway-sdk-1.9.1/scaleway/tests/
+drwxr-xr-x   0 jquere     (501) admin       (80)        0 2019-09-09 16:25:27.000000 scaleway-sdk-1.9.1/scaleway/tests/apis/
+-rw-r--r--   0 jquere     (501) admin       (80)     2346 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.1/scaleway/tests/apis/test_api_metadata.py
+-rw-r--r--   0 jquere     (501) admin       (80)      225 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.1/scaleway/tests/apis/test_api_billing.py
+-rw-r--r--   0 jquere     (501) admin       (80)     1070 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.1/scaleway/tests/apis/__init__.py
+-rw-r--r--   0 jquere     (501) admin       (80)    10617 2019-07-03 19:08:27.000000 scaleway-sdk-1.9.1/scaleway/tests/apis/test_api_account.py
+-rw-r--r--   0 jquere     (501) admin       (80)      901 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.1/scaleway/tests/apis/test_api_compute.py
+-rw-r--r--   0 jquere     (501) admin       (80)     3369 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.1/scaleway/tests/apis/test_api.py
+-rw-r--r--   0 jquere     (501) admin       (80)      448 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.1/scaleway/tests/__init__.py
+-rw-r--r--   0 jquere     (501) admin       (80)      947 2019-09-09 16:25:12.000000 scaleway-sdk-1.9.1/scaleway/__init__.py
+-rw-r--r--   0 jquere     (501) admin       (80)     5929 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.1/README.rst
+-rw-r--r--   0 jquere     (501) admin       (80)      649 2019-09-09 16:25:27.000000 scaleway-sdk-1.9.1/setup.cfg
+-rw-r--r--   0 jquere     (501) admin       (80)      155 2019-07-03 19:00:55.000000 scaleway-sdk-1.9.1/MANIFEST.in
```

### Comparing `scaleway-sdk-1.9.0/CHANGES.rst` & `scaleway-sdk-1.9.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 ChangeLog
 =========
 
+`1.9.1 (2019-09-09) <https://github.com/scaleway/python-scaleway/compare/v1.9.0...v1.9.1>`_
+--------------------------------------------------------------------------------------------
+
+* Add a short (ttl-based) cache to ``AccountAPI.get_quotas()``
+
 `1.9.0 (2019-07-03) <https://github.com/scaleway/python-scaleway/compare/v1.8.1...v1.9.0>`_
 --------------------------------------------------------------------------------------------
 
 * Add support for unlimited quotas
 
 `1.8.1 (2019-06-18) <https://github.com/scaleway/python-scaleway/compare/v1.8.0...v1.8.1>`_
 --------------------------------------------------------------------------------------------
```

### Comparing `scaleway-sdk-1.9.0/PKG-INFO` & `scaleway-sdk-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scaleway-sdk
-Version: 1.9.0
+Version: 1.9.1
 Summary: Python SDK to query Scaleway APIs.
 Home-page: https://github.com/scaleway/python-scaleway
 Author: Scaleway
 Author-email: opensource@scaleway.com
 License: BSD
 Description: Scaleway SDK
         ============
@@ -200,18 +200,18 @@
         License
         -------
         
         This software is licensed under a `BSD 2-Clause License
         <https://github.com/scaleway/python-scaleway/blob/develop/LICENSE>`_.
         
         
-        `Changes for v1.9.0 (2019-07-03) <https://github.com/scaleway/python-scaleway/compare/v1.8.1...v1.9.0>`_
+        `Changes for v1.9.1 (2019-09-09) <https://github.com/scaleway/python-scaleway/compare/v1.9.0...v1.9.1>`_
         --------------------------------------------------------------------------------------------------------
         
-        * Add support for unlimited quotas
+        * Add a short (ttl-based) cache to ``AccountAPI.get_quotas()``
         
         
         `Full changelog <https://github.com/scaleway/python-scaleway/blob/develop/CHANGES.rst#changelog>`_.
 Keywords: network,compute,storage,api,sdk,cloud,iaas
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `scaleway-sdk-1.9.0/LICENSE` & `scaleway-sdk-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scaleway-sdk-1.9.0/setup.py` & `scaleway-sdk-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 from setuptools import find_packages, setup
 
 MODULE_NAME = 'scaleway'
 PACKAGE_NAME = 'scaleway-sdk'
 
 DEPENDENCIES = [
+    'cachetools >= 3.1.1',
     'slumber >= 0.6.2',
     'six']
 
 # Packages required to handle SNI, only for Python2.
 if sys.version_info.major == 2:
     DEPENDENCIES += [
         'pyOpenSSL',
```

### Comparing `scaleway-sdk-1.9.0/scaleway_sdk.egg-info/PKG-INFO` & `scaleway-sdk-1.9.1/scaleway_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scaleway-sdk
-Version: 1.9.0
+Version: 1.9.1
 Summary: Python SDK to query Scaleway APIs.
 Home-page: https://github.com/scaleway/python-scaleway
 Author: Scaleway
 Author-email: opensource@scaleway.com
 License: BSD
 Description: Scaleway SDK
         ============
@@ -200,18 +200,18 @@
         License
         -------
         
         This software is licensed under a `BSD 2-Clause License
         <https://github.com/scaleway/python-scaleway/blob/develop/LICENSE>`_.
         
         
-        `Changes for v1.9.0 (2019-07-03) <https://github.com/scaleway/python-scaleway/compare/v1.8.1...v1.9.0>`_
+        `Changes for v1.9.1 (2019-09-09) <https://github.com/scaleway/python-scaleway/compare/v1.9.0...v1.9.1>`_
         --------------------------------------------------------------------------------------------------------
         
-        * Add support for unlimited quotas
+        * Add a short (ttl-based) cache to ``AccountAPI.get_quotas()``
         
         
         `Full changelog <https://github.com/scaleway/python-scaleway/blob/develop/CHANGES.rst#changelog>`_.
 Keywords: network,compute,storage,api,sdk,cloud,iaas
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `scaleway-sdk-1.9.0/scaleway_sdk.egg-info/SOURCES.txt` & `scaleway-sdk-1.9.1/scaleway_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scaleway-sdk-1.9.0/scaleway/apis/__init__.py` & `scaleway-sdk-1.9.1/scaleway/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-sdk-1.9.0/scaleway/apis/api_metadata.py` & `scaleway-sdk-1.9.1/scaleway/apis/api_metadata.py`

 * *Files identical despite different names*

### Comparing `scaleway-sdk-1.9.0/scaleway/apis/api_account.py` & `scaleway-sdk-1.9.1/scaleway/apis/api_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 #                         Kevin Deldycke <kdeldycke@scaleway.com>
 #
 # Licensed under the BSD 2-Clause License (the "License"); you may not use this
 # file except in compliance with the License. You may obtain a copy of the
 # License at https://opensource.org/licenses/BSD-2-Clause
 
 import slumber
+from cachetools.func import ttl_cache
 from six.moves import zip_longest
 
 from . import API
 
 
 class InvalidToken(Exception):
     pass
@@ -175,14 +176,15 @@
         """ Checks if the token has a permission.
         """
         return bool(
             self.get_resources(service=service, name=name, resource=resource,
                                include_locked=include_locked)
         )
 
+    @ttl_cache(maxsize=10, ttl=60)
     def get_quotas(self, organization):
         """ Gets a list of quotas for the given organization.
         """
         # For now, request more than the default 50 lines
         # TODO: improve this, cf: CP-1660
         response = self.query().organizations(organization).quotas.get(
             per_page=100)
```

### Comparing `scaleway-sdk-1.9.0/scaleway/apis/api_compute.py` & `scaleway-sdk-1.9.1/scaleway/apis/api_compute.py`

 * *Files identical despite different names*

### Comparing `scaleway-sdk-1.9.0/scaleway/tests/apis/test_api_metadata.py` & `scaleway-sdk-1.9.1/scaleway/tests/apis/test_api_metadata.py`

 * *Files identical despite different names*

### Comparing `scaleway-sdk-1.9.0/scaleway/tests/apis/__init__.py` & `scaleway-sdk-1.9.1/scaleway/tests/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-sdk-1.9.0/scaleway/tests/apis/test_api_account.py` & `scaleway-sdk-1.9.1/scaleway/tests/apis/test_api_account.py`

 * *Files identical despite different names*

### Comparing `scaleway-sdk-1.9.0/scaleway/tests/apis/test_api_compute.py` & `scaleway-sdk-1.9.1/scaleway/tests/apis/test_api_compute.py`

 * *Files identical despite different names*

### Comparing `scaleway-sdk-1.9.0/scaleway/tests/apis/test_api.py` & `scaleway-sdk-1.9.1/scaleway/tests/apis/test_api.py`

 * *Files identical despite different names*

### Comparing `scaleway-sdk-1.9.0/scaleway/__init__.py` & `scaleway-sdk-1.9.1/scaleway/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,8 @@
             pass
 
 # Prevent message "No handlers could be found for logger "scaleway"" to be
 # displayed.
 logging.getLogger(__name__).addHandler(NullHandler())
 
 
-__version__ = '1.9.0'
+__version__ = '1.9.1'
```

### Comparing `scaleway-sdk-1.9.0/README.rst` & `scaleway-sdk-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `scaleway-sdk-1.9.0/setup.cfg` & `scaleway-sdk-1.9.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [bdist_wheel]
 universal = 1
 
 [bumpversion]
-current_version = 1.8.2
+current_version = 1.9.1
 files = ./scaleway/__init__.py ./CHANGES.rst
 allow_dirty = True
 commit = False
 tag = False
 tag_name = v{new_version}
 
 [isort]
```


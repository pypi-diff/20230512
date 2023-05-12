# Comparing `tmp/wagtail-sharing-2.8.tar.gz` & `tmp/wagtail-sharing-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-sharing-2.8.tar", last modified: Fri Mar 17 18:48:07 2023, max compression
+gzip compressed data, was "wagtail-sharing-2.9.tar", last modified: Fri May 12 12:56:07 2023, max compression
```

## Comparing `wagtail-sharing-2.8.tar` & `wagtail-sharing-2.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 18:48:07.567840 wagtail-sharing-2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10851 2023-03-17 18:48:07.567840 wagtail-sharing-2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 18:48:07.567840 wagtail-sharing-2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 18:48:07.559840 wagtail-sharing-2.8/wagtail_sharing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10851 2023-03-17 18:48:07.000000 wagtail-sharing-2.8/wagtail_sharing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-03-17 18:48:07.000000 wagtail-sharing-2.8/wagtail_sharing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 18:48:07.000000 wagtail-sharing-2.8/wagtail_sharing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-17 18:48:07.000000 wagtail-sharing-2.8/wagtail_sharing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-17 18:48:07.000000 wagtail-sharing-2.8/wagtail_sharing.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 18:48:07.563840 wagtail-sharing-2.8/wagtailsharing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 18:48:07.563840 wagtail-sharing-2.8/wagtailsharing/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/migrations/0002_shareableroutablepage.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/migrations/0003_delete_shareableroutablepage.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/migrations/0004_bigautofield.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 18:48:07.555840 wagtail-sharing-2.8/wagtailsharing/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 18:48:07.563840 wagtail-sharing-2.8/wagtailsharing/templates/wagtailsharing/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/templates/wagtailsharing/banner.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 18:48:07.563840 wagtail-sharing-2.8/wagtailsharing/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/tests/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 18:48:07.567840 wagtail-sharing-2.8/wagtailsharing/tests/shareable_routable_testapp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/tests/shareable_routable_testapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/tests/shareable_routable_testapp/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 18:48:07.567840 wagtail-sharing-2.8/wagtailsharing/tests/shareable_routable_testapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/tests/shareable_routable_testapp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/tests/shareable_routable_testapp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/tests/shareable_routable_testapp/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/tests/test_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/tests/test_wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-03-17 18:47:43.000000 wagtail-sharing-2.8/wagtailsharing/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:56:07.405244 wagtail-sharing-2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10851 2023-05-12 12:56:07.405244 wagtail-sharing-2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 12:56:07.405244 wagtail-sharing-2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:56:07.397244 wagtail-sharing-2.9/wagtail_sharing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10851 2023-05-12 12:56:07.000000 wagtail-sharing-2.9/wagtail_sharing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-12 12:56:07.000000 wagtail-sharing-2.9/wagtail_sharing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 12:56:07.000000 wagtail-sharing-2.9/wagtail_sharing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-12 12:56:07.000000 wagtail-sharing-2.9/wagtail_sharing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-12 12:56:07.000000 wagtail-sharing-2.9/wagtail_sharing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:56:07.397244 wagtail-sharing-2.9/wagtailsharing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:56:07.401244 wagtail-sharing-2.9/wagtailsharing/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/migrations/0002_shareableroutablepage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/migrations/0003_delete_shareableroutablepage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/migrations/0004_bigautofield.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:56:07.393244 wagtail-sharing-2.9/wagtailsharing/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:56:07.401244 wagtail-sharing-2.9/wagtailsharing/templates/wagtailsharing/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/templates/wagtailsharing/banner.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:56:07.405244 wagtail-sharing-2.9/wagtailsharing/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:56:07.405244 wagtail-sharing-2.9/wagtailsharing/tests/shareable_routable_testapp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/tests/shareable_routable_testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/tests/shareable_routable_testapp/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:56:07.405244 wagtail-sharing-2.9/wagtailsharing/tests/shareable_routable_testapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/tests/shareable_routable_testapp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/tests/shareable_routable_testapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/tests/shareable_routable_testapp/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/tests/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/tests/test_wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-12 12:55:46.000000 wagtail-sharing-2.9/wagtailsharing/wagtail_hooks.py
```

### Comparing `wagtail-sharing-2.8/LICENSE` & `wagtail-sharing-2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-sharing-2.8/PKG-INFO` & `wagtail-sharing-2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-sharing
-Version: 2.8
+Version: 2.9
 Summary: Easier sharing of Wagtail drafts
 Author-email: CFPB <tech@cfpb.gov>
 License: CC0
 Project-URL: Homepage, https://github.com/cfpb/wagtail-sharing
 Project-URL: Bug Reports, https://github.com/cfpb/wagtail-sharing/issues
 Project-URL: Source, https://github.com/cfpb/wagtail-sharing
 Classifier: Framework :: Django
```

### Comparing `wagtail-sharing-2.8/README.rst` & `wagtail-sharing-2.9/README.rst`

 * *Files identical despite different names*

### Comparing `wagtail-sharing-2.8/pyproject.toml` & `wagtail-sharing-2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "wagtail-sharing"
-version = "2.8"
+version = "2.9"
 description = "Easier sharing of Wagtail drafts"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {text = "CC0"}
 authors = [
     {name = "CFPB", email = "tech@cfpb.gov" }
 ]
```

### Comparing `wagtail-sharing-2.8/wagtail_sharing.egg-info/PKG-INFO` & `wagtail-sharing-2.9/wagtail_sharing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-sharing
-Version: 2.8
+Version: 2.9
 Summary: Easier sharing of Wagtail drafts
 Author-email: CFPB <tech@cfpb.gov>
 License: CC0
 Project-URL: Homepage, https://github.com/cfpb/wagtail-sharing
 Project-URL: Bug Reports, https://github.com/cfpb/wagtail-sharing/issues
 Project-URL: Source, https://github.com/cfpb/wagtail-sharing
 Classifier: Framework :: Django
```

### Comparing `wagtail-sharing-2.8/wagtail_sharing.egg-info/SOURCES.txt` & `wagtail-sharing-2.9/wagtail_sharing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wagtail-sharing-2.8/wagtailsharing/checks.py` & `wagtail-sharing-2.9/wagtailsharing/checks.py`

 * *Files identical despite different names*

### Comparing `wagtail-sharing-2.8/wagtailsharing/helpers.py` & `wagtail-sharing-2.9/wagtailsharing/helpers.py`

 * *Files identical despite different names*

### Comparing `wagtail-sharing-2.8/wagtailsharing/migrations/0001_initial.py` & `wagtail-sharing-2.9/wagtailsharing/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-sharing-2.8/wagtailsharing/migrations/0002_shareableroutablepage.py` & `wagtail-sharing-2.9/wagtailsharing/migrations/0002_shareableroutablepage.py`

 * *Files identical despite different names*

### Comparing `wagtail-sharing-2.8/wagtailsharing/models.py` & `wagtail-sharing-2.9/wagtailsharing/models.py`

 * *Files identical despite different names*

### Comparing `wagtail-sharing-2.8/wagtailsharing/tests/helpers.py` & `wagtail-sharing-2.9/wagtailsharing/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `wagtail-sharing-2.8/wagtailsharing/tests/settings.py` & `wagtail-sharing-2.9/wagtailsharing/tests/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail-sharing-2.8/wagtailsharing/tests/shareable_routable_testapp/migrations/0001_initial.py` & `wagtail-sharing-2.9/wagtailsharing/tests/shareable_routable_testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-sharing-2.8/wagtailsharing/tests/shareable_routable_testapp/models.py` & `wagtail-sharing-2.9/wagtailsharing/tests/shareable_routable_testapp/models.py`

 * *Files identical despite different names*

### Comparing `wagtail-sharing-2.8/wagtailsharing/tests/test_checks.py` & `wagtail-sharing-2.9/wagtailsharing/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `wagtail-sharing-2.8/wagtailsharing/tests/test_helpers.py` & `wagtail-sharing-2.9/wagtailsharing/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `wagtail-sharing-2.8/wagtailsharing/tests/test_models.py` & `wagtail-sharing-2.9/wagtailsharing/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-sharing-2.8/wagtailsharing/tests/test_urls.py` & `wagtail-sharing-2.9/wagtailsharing/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `wagtail-sharing-2.8/wagtailsharing/tests/test_views.py` & `wagtail-sharing-2.9/wagtailsharing/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `wagtail-sharing-2.8/wagtailsharing/tests/test_wagtail_hooks.py` & `wagtail-sharing-2.9/wagtailsharing/tests/test_wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-sharing-2.8/wagtailsharing/tests/urls.py` & `wagtail-sharing-2.9/wagtailsharing/tests/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail-sharing-2.8/wagtailsharing/views.py` & `wagtail-sharing-2.9/wagtailsharing/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-sharing-2.8/wagtailsharing/wagtail_hooks.py` & `wagtail-sharing-2.9/wagtailsharing/wagtail_hooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,22 +20,24 @@
     add_to_settings_menu = True
     list_display = ("site", "hostname", "port")
 
 
 modeladmin_register(SharingSiteModelAdmin)
 
 
+@hooks.register("register_page_header_buttons")
 @hooks.register("register_page_listing_more_buttons")
 def add_sharing_link(page, page_perms, is_parent=False, next_url=None):
     sharing_url = get_sharing_url(page)
 
     if sharing_url:
         yield wagtailadmin_widgets.Button(
             "View sharing link",
             sharing_url,
+            icon_name="draft",
             attrs={
                 "title": _("View shared revision of '{}'").format(
                     page.get_admin_display_title()
                 ),
             },
             priority=90,
         )
```


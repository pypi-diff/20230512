# Comparing `tmp/swimlane-4.1.2.tar.gz` & `tmp/swimlane-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swimlane-4.1.2.tar", last modified: Tue Apr 16 01:49:54 2019, max compression
+gzip compressed data, was "dist/swimlane-4.2.0.tar", last modified: Fri May 31 21:01:12 2019, max compression
```

## Comparing `swimlane-4.1.2.tar` & `swimlane-4.2.0.tar`

### file list

```diff
@@ -1,64 +1,69 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-04-16 01:49:54.000000 swimlane-4.1.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1899 2019-04-16 01:48:26.000000 swimlane-4.1.2/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1126 2019-04-16 01:48:26.000000 swimlane-4.1.2/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-04-16 01:49:54.000000 swimlane-4.1.2/swimlane/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6568 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      319 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-04-16 01:49:54.000000 swimlane-4.1.2/swimlane/core/
--rw-rw-r--   0 travis    (2000) travis    (2000)    14079 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2147 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/cursor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      705 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/resolver.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-04-16 01:49:54.000000 swimlane-4.1.2/swimlane/core/adapters/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1844 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/adapters/app.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2411 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/adapters/helper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13844 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/adapters/record.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5499 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/adapters/usergroup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      301 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/adapters/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1656 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/adapters/report.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-04-16 01:49:54.000000 swimlane-4.1.2/swimlane/core/fields/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1158 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/fields/number.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2174 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/fields/attachment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3747 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/fields/datetime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5182 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/fields/reference.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-04-16 01:49:54.000000 swimlane-4.1.2/swimlane/core/fields/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3067 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/fields/base/cursor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      400 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/fields/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3018 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/fields/base/multiselect.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4806 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/fields/base/field.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4709 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/fields/usergroup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1544 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/fields/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2405 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/fields/history.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2056 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/fields/valueslist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      647 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/fields/text.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10151 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/fields/list.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      240 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/fields/tracking.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1319 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/fields/comment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      485 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/search.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/bulk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-04-16 01:49:54.000000 swimlane-4.1.2/swimlane/core/resources/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3909 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/resources/app.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11883 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/resources/record.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1621 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/resources/attachment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4863 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/resources/usergroup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/resources/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4627 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/resources/report.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1831 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/resources/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1080 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/resources/comment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5883 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/cache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      567 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/core/wrappedsession.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-04-16 01:49:54.000000 swimlane-4.1.2/swimlane/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3299 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3674 2019-04-16 01:48:26.000000 swimlane-4.1.2/swimlane/utils/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32386 2019-04-16 01:48:26.000000 swimlane-4.1.2/LICENSE
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-04-16 01:49:54.000000 swimlane-4.1.2/swimlane.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2019-04-16 01:49:54.000000 swimlane-4.1.2/swimlane.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      171 2019-04-16 01:49:54.000000 swimlane-4.1.2/swimlane.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2969 2019-04-16 01:49:54.000000 swimlane-4.1.2/swimlane.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-04-16 01:49:54.000000 swimlane-4.1.2/swimlane.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1562 2019-04-16 01:49:54.000000 swimlane-4.1.2/swimlane.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      178 2019-04-16 01:49:54.000000 swimlane-4.1.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      171 2019-04-16 01:48:26.000000 swimlane-4.1.2/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       71 2019-04-16 01:48:26.000000 swimlane-4.1.2/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2969 2019-04-16 01:49:54.000000 swimlane-4.1.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)       62 2019-04-16 01:48:26.000000 swimlane-4.1.2/test-requirements.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-31 21:01:12.000000 swimlane-4.2.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1899 2019-05-31 20:59:37.000000 swimlane-4.2.0/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1126 2019-05-31 20:59:38.000000 swimlane-4.2.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-31 21:01:12.000000 swimlane-4.2.0/swimlane/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6568 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      319 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-31 21:01:12.000000 swimlane-4.2.0/swimlane/core/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14079 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2147 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/cursor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      705 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/resolver.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-31 21:01:12.000000 swimlane-4.2.0/swimlane/core/adapters/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1844 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/adapters/app.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2411 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/adapters/helper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13844 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/adapters/record.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1504 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/adapters/record_revision.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5499 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/adapters/usergroup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      397 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/adapters/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1505 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/adapters/app_revision.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1656 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/adapters/report.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-31 21:01:12.000000 swimlane-4.2.0/swimlane/core/fields/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1158 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/fields/number.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2174 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/fields/attachment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3747 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/fields/datetime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5182 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/fields/reference.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-31 21:01:12.000000 swimlane-4.2.0/swimlane/core/fields/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3067 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/fields/base/cursor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      400 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/fields/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3018 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/fields/base/multiselect.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4806 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/fields/base/field.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4709 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/fields/usergroup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1544 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/fields/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      935 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/fields/history.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2056 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/fields/valueslist.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      647 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/fields/text.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10151 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/fields/list.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      240 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/fields/tracking.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1319 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/fields/comment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      485 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/search.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/bulk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-31 21:01:12.000000 swimlane-4.2.0/swimlane/core/resources/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1460 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/resources/revision_base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3979 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/resources/app.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12042 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/resources/record.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1621 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/resources/attachment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1363 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/resources/record_revision.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4863 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/resources/usergroup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/resources/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1813 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/resources/app_revision.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4627 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/resources/report.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1831 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/resources/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1080 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/resources/comment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5883 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/cache.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      567 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/core/wrappedsession.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-31 21:01:12.000000 swimlane-4.2.0/swimlane/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3299 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3674 2019-05-31 20:59:38.000000 swimlane-4.2.0/swimlane/utils/version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32386 2019-05-31 20:59:37.000000 swimlane-4.2.0/LICENSE
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-31 21:01:12.000000 swimlane-4.2.0/swimlane.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2019-05-31 21:01:12.000000 swimlane-4.2.0/swimlane.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      171 2019-05-31 21:01:12.000000 swimlane-4.2.0/swimlane.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2969 2019-05-31 21:01:12.000000 swimlane-4.2.0/swimlane.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-05-31 21:01:12.000000 swimlane-4.2.0/swimlane.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1767 2019-05-31 21:01:12.000000 swimlane-4.2.0/swimlane.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      178 2019-05-31 21:01:12.000000 swimlane-4.2.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      171 2019-05-31 20:59:38.000000 swimlane-4.2.0/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       71 2019-05-31 20:59:37.000000 swimlane-4.2.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2969 2019-05-31 21:01:12.000000 swimlane-4.2.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)       62 2019-05-31 20:59:38.000000 swimlane-4.2.0/test-requirements.txt
```

### Comparing `swimlane-4.1.2/README.rst` & `swimlane-4.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/setup.py` & `swimlane-4.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 with open('./README.rst') as f:
     long_description = f.read()
 
 
 setup(
-    version="4.1.2",
+    version="4.2.0",
     name="swimlane",
     author="Swimlane LLC",
     author_email="info@swimlane.com",
     url="https://github.com/swimlane/swimlane-python",
     packages=find_packages(exclude=('tests', 'tests.*')),
     description="Python driver for the Swimlane API",
     long_description=long_description,
```

### Comparing `swimlane-4.1.2/swimlane/exceptions.py` & `swimlane-4.2.0/swimlane/exceptions.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/client.py` & `swimlane-4.2.0/swimlane/core/client.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/cursor.py` & `swimlane-4.2.0/swimlane/core/cursor.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/resolver.py` & `swimlane-4.2.0/swimlane/core/resolver.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/adapters/app.py` & `swimlane-4.2.0/swimlane/core/adapters/app.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/adapters/helper.py` & `swimlane-4.2.0/swimlane/core/adapters/helper.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/adapters/record.py` & `swimlane-4.2.0/swimlane/core/adapters/record.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/adapters/usergroup.py` & `swimlane-4.2.0/swimlane/core/adapters/usergroup.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/adapters/report.py` & `swimlane-4.2.0/swimlane/core/adapters/report.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/fields/number.py` & `swimlane-4.2.0/swimlane/core/fields/number.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/fields/attachment.py` & `swimlane-4.2.0/swimlane/core/fields/attachment.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/fields/datetime.py` & `swimlane-4.2.0/swimlane/core/fields/datetime.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/fields/reference.py` & `swimlane-4.2.0/swimlane/core/fields/reference.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/fields/base/cursor.py` & `swimlane-4.2.0/swimlane/core/fields/base/cursor.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/fields/base/multiselect.py` & `swimlane-4.2.0/swimlane/core/fields/base/multiselect.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/fields/base/field.py` & `swimlane-4.2.0/swimlane/core/fields/base/field.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/fields/usergroup.py` & `swimlane-4.2.0/swimlane/core/fields/usergroup.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/fields/__init__.py` & `swimlane-4.2.0/swimlane/core/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/fields/valueslist.py` & `swimlane-4.2.0/swimlane/core/fields/valueslist.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/fields/text.py` & `swimlane-4.2.0/swimlane/core/fields/text.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/fields/list.py` & `swimlane-4.2.0/swimlane/core/fields/list.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/fields/comment.py` & `swimlane-4.2.0/swimlane/core/fields/comment.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/bulk.py` & `swimlane-4.2.0/swimlane/core/bulk.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/resources/app.py` & `swimlane-4.2.0/swimlane/core/resources/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,17 +40,18 @@
             # Include original name to simplify name resolution
             self._keys_to_field_names[name] = name
             key = field_def.get('key')
             if key:
                 self._keys_to_field_names[key] = name
 
         # Avoid circular import
-        from swimlane.core.adapters import RecordAdapter, ReportAdapter
+        from swimlane.core.adapters import RecordAdapter, ReportAdapter, AppRevisionAdapter
         self.records = RecordAdapter(self)
         self.reports = ReportAdapter(self)
+        self.revisions = AppRevisionAdapter(self)
 
     def __str__(self):
         return '{self.name} ({self.acronym})'.format(self=self)
 
     def __hash__(self):
         return hash((self.id, self.name))
```

### Comparing `swimlane-4.1.2/swimlane/core/resources/record.py` & `swimlane-4.2.0/swimlane/core/resources/record.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,18 @@
             self.modified = pendulum.parse(self._raw['modifiedDate'])
 
         self.__allowed = []
 
         self._fields = {}
         self.__premap_fields()
 
+        # avoid circular reference
+        from swimlane.core.adapters import RecordRevisionAdapter
+        self.revisions = RecordRevisionAdapter(app, self)
+
     @property
     def app(self):
         return self.__app
 
     def __str__(self):
         if self.is_new:
             return '{} - New'.format(self.app.acronym)
```

### Comparing `swimlane-4.1.2/swimlane/core/resources/attachment.py` & `swimlane-4.2.0/swimlane/core/resources/attachment.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/resources/usergroup.py` & `swimlane-4.2.0/swimlane/core/resources/usergroup.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/resources/report.py` & `swimlane-4.2.0/swimlane/core/resources/report.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/resources/base.py` & `swimlane-4.2.0/swimlane/core/resources/base.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/resources/comment.py` & `swimlane-4.2.0/swimlane/core/resources/comment.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/cache.py` & `swimlane-4.2.0/swimlane/core/cache.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/core/wrappedsession.py` & `swimlane-4.2.0/swimlane/core/wrappedsession.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/utils/__init__.py` & `swimlane-4.2.0/swimlane/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane/utils/version.py` & `swimlane-4.2.0/swimlane/utils/version.py`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/LICENSE` & `swimlane-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swimlane-4.1.2/swimlane.egg-info/PKG-INFO` & `swimlane-4.2.0/swimlane.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: swimlane
-Version: 4.1.2
+Version: 4.2.0
 Summary: Python driver for the Swimlane API
 Home-page: https://github.com/swimlane/swimlane-python
 Author: Swimlane LLC
 Author-email: info@swimlane.com
 License: AGPLv3
 Description: .. image:: https://raw.githubusercontent.com/swimlane/swimlane-python/master/docs/logo.png
```

### Comparing `swimlane-4.1.2/swimlane.egg-info/SOURCES.txt` & `swimlane-4.2.0/swimlane.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,16 +18,18 @@
 swimlane/core/client.py
 swimlane/core/cursor.py
 swimlane/core/resolver.py
 swimlane/core/search.py
 swimlane/core/wrappedsession.py
 swimlane/core/adapters/__init__.py
 swimlane/core/adapters/app.py
+swimlane/core/adapters/app_revision.py
 swimlane/core/adapters/helper.py
 swimlane/core/adapters/record.py
+swimlane/core/adapters/record_revision.py
 swimlane/core/adapters/report.py
 swimlane/core/adapters/usergroup.py
 swimlane/core/fields/__init__.py
 swimlane/core/fields/attachment.py
 swimlane/core/fields/comment.py
 swimlane/core/fields/datetime.py
 swimlane/core/fields/history.py
@@ -40,15 +42,18 @@
 swimlane/core/fields/valueslist.py
 swimlane/core/fields/base/__init__.py
 swimlane/core/fields/base/cursor.py
 swimlane/core/fields/base/field.py
 swimlane/core/fields/base/multiselect.py
 swimlane/core/resources/__init__.py
 swimlane/core/resources/app.py
+swimlane/core/resources/app_revision.py
 swimlane/core/resources/attachment.py
 swimlane/core/resources/base.py
 swimlane/core/resources/comment.py
 swimlane/core/resources/record.py
+swimlane/core/resources/record_revision.py
 swimlane/core/resources/report.py
+swimlane/core/resources/revision_base.py
 swimlane/core/resources/usergroup.py
 swimlane/utils/__init__.py
 swimlane/utils/version.py
```

### Comparing `swimlane-4.1.2/PKG-INFO` & `swimlane-4.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: swimlane
-Version: 4.1.2
+Version: 4.2.0
 Summary: Python driver for the Swimlane API
 Home-page: https://github.com/swimlane/swimlane-python
 Author: Swimlane LLC
 Author-email: info@swimlane.com
 License: AGPLv3
 Description: .. image:: https://raw.githubusercontent.com/swimlane/swimlane-python/master/docs/logo.png
```


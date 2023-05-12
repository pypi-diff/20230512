# Comparing `tmp/wagtail-content-admin-4.1.0.tar.gz` & `tmp/wagtail-content-admin-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-content-admin-4.1.0.tar", last modified: Thu May 11 09:25:08 2023, max compression
+gzip compressed data, was "wagtail-content-admin-4.1.1.tar", last modified: Fri May 12 16:35:50 2023, max compression
```

## Comparing `wagtail-content-admin-4.1.0.tar` & `wagtail-content-admin-4.1.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 09:25:08.772687 wagtail-content-admin-4.1.0/
--rw-r--r--   0 work       (505) staff       (20)       19 2022-03-13 22:55:00.000000 wagtail-content-admin-4.1.0/AUTHORS.txt
--rw-r--r--   0 work       (505) staff       (20)     1525 2023-05-10 12:24:52.000000 wagtail-content-admin-4.1.0/LICENSE.txt
--rw-r--r--   0 work       (505) staff       (20)      459 2023-02-13 13:28:09.000000 wagtail-content-admin-4.1.0/MANIFEST.in
--rw-r--r--   0 work       (505) staff       (20)     1364 2023-05-11 09:25:08.772842 wagtail-content-admin-4.1.0/PKG-INFO
--rw-r--r--   0 work       (505) staff       (20)      635 2023-05-11 09:22:34.000000 wagtail-content-admin-4.1.0/README.md
--rw-r--r--   0 work       (505) staff       (20)      100 2021-02-16 17:38:13.000000 wagtail-content-admin-4.1.0/pyproject.toml
--rw-r--r--   0 work       (505) staff       (20)     1047 2023-05-11 09:25:08.773443 wagtail-content-admin-4.1.0/setup.cfg
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 09:25:08.586505 wagtail-content-admin-4.1.0/src/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 09:25:08.694771 wagtail-content-admin-4.1.0/src/wagtail_content_admin/
--rw-r--r--   0 work       (505) staff       (20)      101 2022-04-23 10:31:20.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin/__init__.py
--rw-r--r--   0 work       (505) staff       (20)     1281 2023-03-06 23:19:35.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin/apps.py
--rw-r--r--   0 work       (505) staff       (20)    26270 2023-03-06 23:42:39.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin/blocks.py
--rw-r--r--   0 work       (505) staff       (20)     7785 2023-02-16 21:07:38.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin/browser.py
--rw-r--r--   0 work       (505) staff       (20)     5598 2023-02-16 21:07:38.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin/chooser.py
--rw-r--r--   0 work       (505) staff       (20)     2100 2023-01-17 11:41:36.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin/config.py
--rw-r--r--   0 work       (505) staff       (20)     8608 2023-01-25 13:49:23.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin/content_admin.py
--rw-r--r--   0 work       (505) staff       (20)       44 2023-02-07 12:01:37.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin/default_settings.py
--rw-r--r--   0 work       (505) staff       (20)      291 2022-04-29 18:16:32.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin/delegate.py
--rw-r--r--   0 work       (505) staff       (20)     2456 2022-05-11 14:22:25.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin/form_fields.py
--rw-r--r--   0 work       (505) staff       (20)    11181 2023-04-04 10:17:07.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin/frontend.py
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 09:25:08.586746 wagtail-content-admin-4.1.0/src/wagtail_content_admin/static/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 09:25:08.586928 wagtail-content-admin-4.1.0/src/wagtail_content_admin/static/wagtail_content_admin/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 09:25:08.702985 wagtail-content-admin-4.1.0/src/wagtail_content_admin/static/wagtail_content_admin/css/
--rw-r--r--   0 work       (505) staff       (20)     2579 2023-03-07 14:02:14.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin/static/wagtail_content_admin/css/wagtail_content_admin.css
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 09:25:08.710703 wagtail-content-admin-4.1.0/src/wagtail_content_admin/static/wagtail_content_admin/js/
--rw-r--r--   0 work       (505) staff       (20)    33840 2023-03-07 14:02:14.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin/static/wagtail_content_admin/js/wagtail_content_admin.js
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 09:25:08.587117 wagtail-content-admin-4.1.0/src/wagtail_content_admin/templates/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 09:25:08.741402 wagtail-content-admin-4.1.0/src/wagtail_content_admin/templates/wagtail_content_admin/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 09:25:08.753481 wagtail-content-admin-4.1.0/src/wagtail_content_admin/templates/wagtail_content_admin/blocks/
--rw-r--r--   0 work       (505) staff       (20)      680 2023-04-03 12:02:02.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin/templates/wagtail_content_admin/blocks/content_render_block.html
--rw-r--r--   0 work       (505) staff       (20)      171 2023-02-13 13:43:40.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin/templates/wagtail_content_admin/blocks/content_render_block_base.html
--rw-r--r--   0 work       (505) staff       (20)     3795 2023-04-04 10:18:44.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin/templates/wagtail_content_admin/browser_index.html
--rw-r--r--   0 work       (505) staff       (20)     2100 2023-04-04 10:19:00.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin/templates/wagtail_content_admin/browser_results.html
--rw-r--r--   0 work       (505) staff       (20)     1985 2022-12-18 16:26:02.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin/templates/wagtail_content_admin/content_chooser.html
--rw-r--r--   0 work       (505) staff       (20)      937 2023-01-19 15:46:06.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin/templates/wagtail_content_admin/content_chooser_results.html
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 09:25:08.765484 wagtail-content-admin-4.1.0/src/wagtail_content_admin/templates/wagtail_content_admin/widgets/
--rw-r--r--   0 work       (505) staff       (20)     1089 2023-01-17 12:06:28.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin/templates/wagtail_content_admin/widgets/compare.html
--rw-r--r--   0 work       (505) staff       (20)     2382 2022-05-09 14:38:08.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin/templates/wagtail_content_admin/widgets/content_chooser.html
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 09:25:08.772282 wagtail-content-admin-4.1.0/src/wagtail_content_admin/templatetags/
--rw-r--r--   0 work       (505) staff       (20)        0 2022-04-23 12:14:08.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin/templatetags/__init__.py
--rw-r--r--   0 work       (505) staff       (20)     2595 2023-02-03 23:01:22.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin/templatetags/wagtail_content_admin_tags.py
--rw-r--r--   0 work       (505) staff       (20)     6829 2023-04-04 10:18:01.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin/widgets.py
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 09:25:08.696424 wagtail-content-admin-4.1.0/src/wagtail_content_admin.egg-info/
--rw-r--r--   0 work       (505) staff       (20)     1364 2023-05-11 09:25:08.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin.egg-info/PKG-INFO
--rw-r--r--   0 work       (505) staff       (20)     1786 2023-05-11 09:25:08.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin.egg-info/SOURCES.txt
--rw-r--r--   0 work       (505) staff       (20)        1 2023-05-11 09:25:08.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin.egg-info/dependency_links.txt
--rw-r--r--   0 work       (505) staff       (20)        1 2023-05-11 09:25:08.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin.egg-info/not-zip-safe
--rw-r--r--   0 work       (505) staff       (20)      182 2023-05-11 09:25:08.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin.egg-info/requires.txt
--rw-r--r--   0 work       (505) staff       (20)       22 2023-05-11 09:25:08.000000 wagtail-content-admin-4.1.0/src/wagtail_content_admin.egg-info/top_level.txt
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:35:50.150962 wagtail-content-admin-4.1.1/
+-rw-r--r--   0 work       (505) staff       (20)       19 2022-03-13 22:55:00.000000 wagtail-content-admin-4.1.1/AUTHORS.txt
+-rw-r--r--   0 work       (505) staff       (20)     1525 2023-05-10 12:24:52.000000 wagtail-content-admin-4.1.1/LICENSE.txt
+-rw-r--r--   0 work       (505) staff       (20)      459 2023-02-13 13:28:09.000000 wagtail-content-admin-4.1.1/MANIFEST.in
+-rw-r--r--   0 work       (505) staff       (20)     1364 2023-05-12 16:35:50.151214 wagtail-content-admin-4.1.1/PKG-INFO
+-rw-r--r--   0 work       (505) staff       (20)      635 2023-05-11 09:22:34.000000 wagtail-content-admin-4.1.1/README.md
+-rw-r--r--   0 work       (505) staff       (20)      100 2021-02-16 17:38:13.000000 wagtail-content-admin-4.1.1/pyproject.toml
+-rw-r--r--   0 work       (505) staff       (20)     1047 2023-05-12 16:35:50.153689 wagtail-content-admin-4.1.1/setup.cfg
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:35:49.798174 wagtail-content-admin-4.1.1/src/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:35:49.992335 wagtail-content-admin-4.1.1/src/wagtail_content_admin/
+-rw-r--r--   0 work       (505) staff       (20)      101 2022-04-23 10:31:20.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin/__init__.py
+-rw-r--r--   0 work       (505) staff       (20)     1281 2023-03-06 23:19:35.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin/apps.py
+-rw-r--r--   0 work       (505) staff       (20)    26270 2023-03-06 23:42:39.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin/blocks.py
+-rw-r--r--   0 work       (505) staff       (20)     7785 2023-02-16 21:07:38.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin/browser.py
+-rw-r--r--   0 work       (505) staff       (20)     5598 2023-02-16 21:07:38.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin/chooser.py
+-rw-r--r--   0 work       (505) staff       (20)     2100 2023-01-17 11:41:36.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin/config.py
+-rw-r--r--   0 work       (505) staff       (20)     8608 2023-01-25 13:49:23.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin/content_admin.py
+-rw-r--r--   0 work       (505) staff       (20)       44 2023-02-07 12:01:37.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin/default_settings.py
+-rw-r--r--   0 work       (505) staff       (20)      291 2022-04-29 18:16:32.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin/delegate.py
+-rw-r--r--   0 work       (505) staff       (20)     2456 2022-05-11 14:22:25.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin/form_fields.py
+-rw-r--r--   0 work       (505) staff       (20)    11185 2023-05-12 14:41:56.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin/frontend.py
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:35:49.798625 wagtail-content-admin-4.1.1/src/wagtail_content_admin/static/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:35:49.799037 wagtail-content-admin-4.1.1/src/wagtail_content_admin/static/wagtail_content_admin/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:35:50.026588 wagtail-content-admin-4.1.1/src/wagtail_content_admin/static/wagtail_content_admin/css/
+-rw-r--r--   0 work       (505) staff       (20)     2579 2023-03-07 14:02:14.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin/static/wagtail_content_admin/css/wagtail_content_admin.css
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:35:50.035474 wagtail-content-admin-4.1.1/src/wagtail_content_admin/static/wagtail_content_admin/js/
+-rw-r--r--   0 work       (505) staff       (20)    33840 2023-03-07 14:02:14.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin/static/wagtail_content_admin/js/wagtail_content_admin.js
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:35:49.799472 wagtail-content-admin-4.1.1/src/wagtail_content_admin/templates/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:35:50.093958 wagtail-content-admin-4.1.1/src/wagtail_content_admin/templates/wagtail_content_admin/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:35:50.126159 wagtail-content-admin-4.1.1/src/wagtail_content_admin/templates/wagtail_content_admin/blocks/
+-rw-r--r--   0 work       (505) staff       (20)      680 2023-04-03 12:02:02.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin/templates/wagtail_content_admin/blocks/content_render_block.html
+-rw-r--r--   0 work       (505) staff       (20)      171 2023-02-13 13:43:40.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin/templates/wagtail_content_admin/blocks/content_render_block_base.html
+-rw-r--r--   0 work       (505) staff       (20)     3795 2023-04-04 10:18:44.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin/templates/wagtail_content_admin/browser_index.html
+-rw-r--r--   0 work       (505) staff       (20)     2100 2023-04-04 10:19:00.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin/templates/wagtail_content_admin/browser_results.html
+-rw-r--r--   0 work       (505) staff       (20)     1985 2022-12-18 16:26:02.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin/templates/wagtail_content_admin/content_chooser.html
+-rw-r--r--   0 work       (505) staff       (20)      937 2023-01-19 15:46:06.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin/templates/wagtail_content_admin/content_chooser_results.html
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:35:50.140401 wagtail-content-admin-4.1.1/src/wagtail_content_admin/templates/wagtail_content_admin/widgets/
+-rw-r--r--   0 work       (505) staff       (20)     1089 2023-01-17 12:06:28.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin/templates/wagtail_content_admin/widgets/compare.html
+-rw-r--r--   0 work       (505) staff       (20)     2382 2022-05-09 14:38:08.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin/templates/wagtail_content_admin/widgets/content_chooser.html
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:35:50.149885 wagtail-content-admin-4.1.1/src/wagtail_content_admin/templatetags/
+-rw-r--r--   0 work       (505) staff       (20)        0 2022-04-23 12:14:08.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin/templatetags/__init__.py
+-rw-r--r--   0 work       (505) staff       (20)     2595 2023-02-03 23:01:22.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin/templatetags/wagtail_content_admin_tags.py
+-rw-r--r--   0 work       (505) staff       (20)     6829 2023-04-04 10:18:01.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin/widgets.py
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:35:50.001741 wagtail-content-admin-4.1.1/src/wagtail_content_admin.egg-info/
+-rw-r--r--   0 work       (505) staff       (20)     1364 2023-05-12 16:35:49.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin.egg-info/PKG-INFO
+-rw-r--r--   0 work       (505) staff       (20)     1786 2023-05-12 16:35:49.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 work       (505) staff       (20)        1 2023-05-12 16:35:49.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 work       (505) staff       (20)        1 2023-05-12 16:35:49.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin.egg-info/not-zip-safe
+-rw-r--r--   0 work       (505) staff       (20)      182 2023-05-12 16:35:49.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin.egg-info/requires.txt
+-rw-r--r--   0 work       (505) staff       (20)       22 2023-05-12 16:35:49.000000 wagtail-content-admin-4.1.1/src/wagtail_content_admin.egg-info/top_level.txt
```

### Comparing `wagtail-content-admin-4.1.0/LICENSE.txt` & `wagtail-content-admin-4.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wagtail-content-admin-4.1.0/PKG-INFO` & `wagtail-content-admin-4.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-content-admin
-Version: 4.1.0
+Version: 4.1.1
 Summary: A Wagtail app for working with content-driven model instances in the admin interface.
 Home-page: https://github.com/high-dimensional/wagtail-content-admin
 Author: High Dimensional Neurology Group, UCL
 Author-email: pypi@highdimensional.net
 License: BSD-3-Clause
 Platform: any
 Classifier: Framework :: Django
```

### Comparing `wagtail-content-admin-4.1.0/README.md` & `wagtail-content-admin-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-content-admin-4.1.0/setup.cfg` & `wagtail-content-admin-4.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wagtail-content-admin
-version = 4.1.0
+version = 4.1.1
 url = https://github.com/high-dimensional/wagtail-content-admin
 author = High Dimensional Neurology Group, UCL
 author_email = pypi@highdimensional.net
 description = A Wagtail app for working with content-driven model instances in the admin interface.
 long_description = file:README.md
 long_description_content_type = text/markdown
 license = BSD-3-Clause
```

### Comparing `wagtail-content-admin-4.1.0/src/wagtail_content_admin/apps.py` & `wagtail-content-admin-4.1.1/src/wagtail_content_admin/apps.py`

 * *Files identical despite different names*

### Comparing `wagtail-content-admin-4.1.0/src/wagtail_content_admin/blocks.py` & `wagtail-content-admin-4.1.1/src/wagtail_content_admin/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-content-admin-4.1.0/src/wagtail_content_admin/browser.py` & `wagtail-content-admin-4.1.1/src/wagtail_content_admin/browser.py`

 * *Files identical despite different names*

### Comparing `wagtail-content-admin-4.1.0/src/wagtail_content_admin/chooser.py` & `wagtail-content-admin-4.1.1/src/wagtail_content_admin/chooser.py`

 * *Files identical despite different names*

### Comparing `wagtail-content-admin-4.1.0/src/wagtail_content_admin/config.py` & `wagtail-content-admin-4.1.1/src/wagtail_content_admin/config.py`

 * *Files identical despite different names*

### Comparing `wagtail-content-admin-4.1.0/src/wagtail_content_admin/content_admin.py` & `wagtail-content-admin-4.1.1/src/wagtail_content_admin/content_admin.py`

 * *Files identical despite different names*

### Comparing `wagtail-content-admin-4.1.0/src/wagtail_content_admin/form_fields.py` & `wagtail-content-admin-4.1.1/src/wagtail_content_admin/form_fields.py`

 * *Files identical despite different names*

### Comparing `wagtail-content-admin-4.1.0/src/wagtail_content_admin/frontend.py` & `wagtail-content-admin-4.1.1/src/wagtail_content_admin/frontend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import copy
 import json
-from collections import Sequence
+from collections.abc import Sequence
 
 from urllib.parse import quote, unquote
 
 from django import forms
 
 from django.utils.translation import gettext_lazy as _
 from django.utils.functional import cached_property
```

### Comparing `wagtail-content-admin-4.1.0/src/wagtail_content_admin/static/wagtail_content_admin/css/wagtail_content_admin.css` & `wagtail-content-admin-4.1.1/src/wagtail_content_admin/static/wagtail_content_admin/css/wagtail_content_admin.css`

 * *Files identical despite different names*

### Comparing `wagtail-content-admin-4.1.0/src/wagtail_content_admin/static/wagtail_content_admin/js/wagtail_content_admin.js` & `wagtail-content-admin-4.1.1/src/wagtail_content_admin/static/wagtail_content_admin/js/wagtail_content_admin.js`

 * *Files identical despite different names*

### Comparing `wagtail-content-admin-4.1.0/src/wagtail_content_admin/templates/wagtail_content_admin/blocks/content_render_block.html` & `wagtail-content-admin-4.1.1/src/wagtail_content_admin/templates/wagtail_content_admin/blocks/content_render_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-content-admin-4.1.0/src/wagtail_content_admin/templates/wagtail_content_admin/browser_index.html` & `wagtail-content-admin-4.1.1/src/wagtail_content_admin/templates/wagtail_content_admin/browser_index.html`

 * *Files identical despite different names*

### Comparing `wagtail-content-admin-4.1.0/src/wagtail_content_admin/templates/wagtail_content_admin/browser_results.html` & `wagtail-content-admin-4.1.1/src/wagtail_content_admin/templates/wagtail_content_admin/browser_results.html`

 * *Files identical despite different names*

### Comparing `wagtail-content-admin-4.1.0/src/wagtail_content_admin/templates/wagtail_content_admin/content_chooser.html` & `wagtail-content-admin-4.1.1/src/wagtail_content_admin/templates/wagtail_content_admin/content_chooser.html`

 * *Files identical despite different names*

### Comparing `wagtail-content-admin-4.1.0/src/wagtail_content_admin/templates/wagtail_content_admin/content_chooser_results.html` & `wagtail-content-admin-4.1.1/src/wagtail_content_admin/templates/wagtail_content_admin/content_chooser_results.html`

 * *Files identical despite different names*

### Comparing `wagtail-content-admin-4.1.0/src/wagtail_content_admin/templates/wagtail_content_admin/widgets/compare.html` & `wagtail-content-admin-4.1.1/src/wagtail_content_admin/templates/wagtail_content_admin/widgets/compare.html`

 * *Files identical despite different names*

### Comparing `wagtail-content-admin-4.1.0/src/wagtail_content_admin/templates/wagtail_content_admin/widgets/content_chooser.html` & `wagtail-content-admin-4.1.1/src/wagtail_content_admin/templates/wagtail_content_admin/widgets/content_chooser.html`

 * *Files identical despite different names*

### Comparing `wagtail-content-admin-4.1.0/src/wagtail_content_admin/templatetags/wagtail_content_admin_tags.py` & `wagtail-content-admin-4.1.1/src/wagtail_content_admin/templatetags/wagtail_content_admin_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail-content-admin-4.1.0/src/wagtail_content_admin/widgets.py` & `wagtail-content-admin-4.1.1/src/wagtail_content_admin/widgets.py`

 * *Files identical despite different names*

### Comparing `wagtail-content-admin-4.1.0/src/wagtail_content_admin.egg-info/PKG-INFO` & `wagtail-content-admin-4.1.1/src/wagtail_content_admin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-content-admin
-Version: 4.1.0
+Version: 4.1.1
 Summary: A Wagtail app for working with content-driven model instances in the admin interface.
 Home-page: https://github.com/high-dimensional/wagtail-content-admin
 Author: High Dimensional Neurology Group, UCL
 Author-email: pypi@highdimensional.net
 License: BSD-3-Clause
 Platform: any
 Classifier: Framework :: Django
```

### Comparing `wagtail-content-admin-4.1.0/src/wagtail_content_admin.egg-info/SOURCES.txt` & `wagtail-content-admin-4.1.1/src/wagtail_content_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*


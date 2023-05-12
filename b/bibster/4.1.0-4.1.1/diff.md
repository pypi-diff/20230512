# Comparing `tmp/bibster-4.1.0.tar.gz` & `tmp/bibster-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibster-4.1.0.tar", last modified: Thu May 11 14:36:31 2023, max compression
+gzip compressed data, was "bibster-4.1.1.tar", last modified: Fri May 12 15:02:14 2023, max compression
```

## Comparing `bibster-4.1.0.tar` & `bibster-4.1.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:36:31.726124 bibster-4.1.0/
--rw-r--r--   0 work       (505) staff       (20)       19 2022-03-13 22:55:00.000000 bibster-4.1.0/AUTHORS.txt
--rw-r--r--   0 work       (505) staff       (20)     1525 2023-05-10 12:24:52.000000 bibster-4.1.0/LICENSE.txt
--rw-r--r--   0 work       (505) staff       (20)      357 2023-01-20 12:22:36.000000 bibster-4.1.0/MANIFEST.in
--rw-r--r--   0 work       (505) staff       (20)     1144 2023-05-11 14:36:31.726258 bibster-4.1.0/PKG-INFO
--rw-r--r--   0 work       (505) staff       (20)      497 2023-05-11 13:28:40.000000 bibster-4.1.0/README.md
--rw-r--r--   0 work       (505) staff       (20)      100 2021-02-16 17:38:13.000000 bibster-4.1.0/pyproject.toml
--rw-r--r--   0 work       (505) staff       (20)     1233 2023-05-11 14:36:31.727473 bibster-4.1.0/setup.cfg
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:36:31.649976 bibster-4.1.0/src/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:36:31.679323 bibster-4.1.0/src/bibster/
--rw-r--r--   0 work       (505) staff       (20)       50 2022-07-17 16:38:42.000000 bibster-4.1.0/src/bibster/__init__.py
--rw-r--r--   0 work       (505) staff       (20)      383 2023-02-04 22:58:26.000000 bibster-4.1.0/src/bibster/admin_urls.py
--rw-r--r--   0 work       (505) staff       (20)     1794 2023-03-06 23:13:41.000000 bibster-4.1.0/src/bibster/apps.py
--rw-r--r--   0 work       (505) staff       (20)    14140 2023-03-02 13:51:17.000000 bibster-4.1.0/src/bibster/auto_fill.py
--rw-r--r--   0 work       (505) staff       (20)    15592 2023-03-02 13:44:38.000000 bibster-4.1.0/src/bibster/auxiliaries.py
--rw-r--r--   0 work       (505) staff       (20)    20700 2023-03-02 13:45:11.000000 bibster-4.1.0/src/bibster/block_auxiliaries.py
--rw-r--r--   0 work       (505) staff       (20)    27302 2023-05-11 13:29:36.000000 bibster-4.1.0/src/bibster/blocks.py
--rw-r--r--   0 work       (505) staff       (20)     1078 2023-01-25 12:16:35.000000 bibster-4.1.0/src/bibster/content_admin.py
--rw-r--r--   0 work       (505) staff       (20)      416 2023-03-02 10:52:20.000000 bibster-4.1.0/src/bibster/default_settings.py
--rw-r--r--   0 work       (505) staff       (20)     4687 2022-10-05 14:45:26.000000 bibster-4.1.0/src/bibster/format_auxiliaries.py
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:36:31.715635 bibster-4.1.0/src/bibster/formatting/
--rw-r--r--   0 work       (505) staff       (20)      357 2022-10-16 14:34:27.000000 bibster-4.1.0/src/bibster/formatting/__init__.py
--rw-r--r--   0 work       (505) staff       (20)     1665 2022-10-05 10:54:59.000000 bibster-4.1.0/src/bibster/formatting/base.py
--rw-r--r--   0 work       (505) staff       (20)     4996 2022-10-04 10:21:17.000000 bibster-4.1.0/src/bibster/formatting/dictionary_format.py
--rw-r--r--   0 work       (505) staff       (20)     1355 2022-10-04 10:11:50.000000 bibster-4.1.0/src/bibster/formatting/ellipsis.py
--rw-r--r--   0 work       (505) staff       (20)     4933 2022-10-04 10:17:33.000000 bibster-4.1.0/src/bibster/formatting/grouping_format.py
--rw-r--r--   0 work       (505) staff       (20)     7123 2022-10-05 11:22:36.000000 bibster-4.1.0/src/bibster/formatting/markup.py
--rw-r--r--   0 work       (505) staff       (20)     6376 2022-10-04 10:22:24.000000 bibster-4.1.0/src/bibster/formatting/predicate_format.py
--rw-r--r--   0 work       (505) staff       (20)     8143 2022-10-04 10:37:08.000000 bibster-4.1.0/src/bibster/formatting/sequence_format.py
--rw-r--r--   0 work       (505) staff       (20)     2624 2022-10-04 10:40:52.000000 bibster-4.1.0/src/bibster/formatting/sequence_map.py
--rw-r--r--   0 work       (505) staff       (20)     2853 2022-10-04 10:20:00.000000 bibster-4.1.0/src/bibster/formatting/switch_format.py
--rw-r--r--   0 work       (505) staff       (20)     6316 2022-10-05 10:55:34.000000 bibster-4.1.0/src/bibster/formatting/titlecase.py
--rw-r--r--   0 work       (505) staff       (20)    18643 2022-10-04 10:44:40.000000 bibster-4.1.0/src/bibster/formatting/value_converters.py
--rw-r--r--   0 work       (505) staff       (20)     3709 2022-10-04 10:40:56.000000 bibster-4.1.0/src/bibster/formatting/value_format.py
--rw-r--r--   0 work       (505) staff       (20)     1842 2022-10-04 10:42:10.000000 bibster-4.1.0/src/bibster/formatting/xml_io.py
--rw-r--r--   0 work       (505) staff       (20)     1522 2023-04-04 10:32:03.000000 bibster-4.1.0/src/bibster/frontend.py
--rw-r--r--   0 work       (505) staff       (20)    33254 2023-01-10 10:34:51.000000 bibster-4.1.0/src/bibster/harvard_style.py
--rw-r--r--   0 work       (505) staff       (20)     7224 2023-02-03 13:33:54.000000 bibster-4.1.0/src/bibster/html_markup.py
--rw-r--r--   0 work       (505) staff       (20)     1950 2022-10-04 11:31:05.000000 bibster-4.1.0/src/bibster/identifiers.py
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:36:31.716678 bibster-4.1.0/src/bibster/migrations/
--rw-r--r--   0 work       (505) staff       (20)     8673 2023-03-07 11:38:12.000000 bibster-4.1.0/src/bibster/migrations/0001_initial.py
--rw-r--r--   0 work       (505) staff       (20)        0 2022-10-04 12:27:23.000000 bibster-4.1.0/src/bibster/migrations/__init__.py
--rw-r--r--   0 work       (505) staff       (20)     1718 2022-10-10 18:20:26.000000 bibster-4.1.0/src/bibster/mixins.py
--rw-r--r--   0 work       (505) staff       (20)      919 2023-02-04 22:53:44.000000 bibster-4.1.0/src/bibster/model_admin.py
--rw-r--r--   0 work       (505) staff       (20)     1652 2022-11-19 15:02:43.000000 bibster-4.1.0/src/bibster/model_porter.py
--rw-r--r--   0 work       (505) staff       (20)    13239 2023-03-07 11:38:05.000000 bibster-4.1.0/src/bibster/models.py
--rw-r--r--   0 work       (505) staff       (20)      237 2023-02-16 21:31:47.000000 bibster-4.1.0/src/bibster/permissions.py
--rw-r--r--   0 work       (505) staff       (20)     1880 2022-10-04 12:25:03.000000 bibster-4.1.0/src/bibster/plain_name_format.py
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:36:31.650488 bibster-4.1.0/src/bibster/static/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:36:31.650703 bibster-4.1.0/src/bibster/static/bibster/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:36:31.716876 bibster-4.1.0/src/bibster/static/bibster/css/
--rw-r--r--   0 work       (505) staff       (20)        0 2023-02-08 18:09:55.000000 bibster-4.1.0/src/bibster/static/bibster/css/bibster.css
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:36:31.718531 bibster-4.1.0/src/bibster/static/bibster/js/
--rw-r--r--   0 work       (505) staff       (20)     2871 2023-02-04 22:56:34.000000 bibster-4.1.0/src/bibster/static/bibster/js/publication_modeladmin.js
--rw-r--r--   0 work       (505) staff       (20)     2829 2022-07-18 08:48:15.000000 bibster-4.1.0/src/bibster/static/bibster/js/reference_block.js
--rw-r--r--   0 work       (505) staff       (20)     6491 2022-07-18 08:49:04.000000 bibster-4.1.0/src/bibster/static/bibster/js/reference_lookup.js
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:36:31.651152 bibster-4.1.0/src/bibster/templates/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:36:31.651009 bibster-4.1.0/src/bibster/templates/bibster/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:36:31.722187 bibster-4.1.0/src/bibster/templates/bibster/blocks/
--rw-r--r--   0 work       (505) staff       (20)     1795 2023-05-11 13:29:36.000000 bibster-4.1.0/src/bibster/templates/bibster/blocks/publication_list.html
--rw-r--r--   0 work       (505) staff       (20)       90 2023-01-25 13:14:01.000000 bibster-4.1.0/src/bibster/templates/bibster/blocks/publication_list_switch.html
--rw-r--r--   0 work       (505) staff       (20)       83 2023-02-11 13:53:57.000000 bibster-4.1.0/src/bibster/templates/bibster/blocks/publication_showcase.html
--rw-r--r--   0 work       (505) staff       (20)       90 2023-02-11 13:53:57.000000 bibster-4.1.0/src/bibster/templates/bibster/blocks/publication_showcase_switch.html
--rw-r--r--   0 work       (505) staff       (20)      125 2022-10-05 13:41:51.000000 bibster-4.1.0/src/bibster/templates/bibster/blocks/reference_block.html
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:36:31.651234 bibster-4.1.0/src/bibster/templates/modeladmin/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:36:31.651317 bibster-4.1.0/src/bibster/templates/modeladmin/bibster/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:36:31.722759 bibster-4.1.0/src/bibster/templates/modeladmin/bibster/publication/
--rw-r--r--   0 work       (505) staff       (20)      544 2023-02-04 23:02:46.000000 bibster-4.1.0/src/bibster/templates/modeladmin/bibster/publication/index.html
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:36:31.723540 bibster-4.1.0/src/bibster/templatetags/
--rw-r--r--   0 work       (505) staff       (20)        0 2022-07-18 10:45:11.000000 bibster-4.1.0/src/bibster/templatetags/__init__.py
--rw-r--r--   0 work       (505) staff       (20)     1608 2023-04-04 13:38:30.000000 bibster-4.1.0/src/bibster/templatetags/bibster_tags.py
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:36:31.725412 bibster-4.1.0/src/bibster/views/
--rw-r--r--   0 work       (505) staff       (20)        0 2022-07-17 20:44:31.000000 bibster-4.1.0/src/bibster/views/__init__.py
--rw-r--r--   0 work       (505) staff       (20)     1800 2023-02-04 23:08:15.000000 bibster-4.1.0/src/bibster/views/action.py
--rw-r--r--   0 work       (505) staff       (20)     1700 2023-02-16 21:32:13.000000 bibster-4.1.0/src/bibster/views/lookup.py
--rw-r--r--   0 work       (505) staff       (20)      529 2023-02-16 21:32:13.000000 bibster-4.1.0/src/bibster/wagtail_hooks.py
--rw-r--r--   0 work       (505) staff       (20)    22665 2019-02-06 10:42:22.000000 bibster-4.1.0/src/bibster/xml_io.py
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:36:31.705094 bibster-4.1.0/src/bibster.egg-info/
--rw-r--r--   0 work       (505) staff       (20)     1144 2023-05-11 14:36:31.000000 bibster-4.1.0/src/bibster.egg-info/PKG-INFO
--rw-r--r--   0 work       (505) staff       (20)     2218 2023-05-11 14:36:31.000000 bibster-4.1.0/src/bibster.egg-info/SOURCES.txt
--rw-r--r--   0 work       (505) staff       (20)        1 2023-05-11 14:36:31.000000 bibster-4.1.0/src/bibster.egg-info/dependency_links.txt
--rw-r--r--   0 work       (505) staff       (20)        1 2023-05-11 14:36:31.000000 bibster-4.1.0/src/bibster.egg-info/not-zip-safe
--rw-r--r--   0 work       (505) staff       (20)      440 2023-05-11 14:36:31.000000 bibster-4.1.0/src/bibster.egg-info/requires.txt
--rw-r--r--   0 work       (505) staff       (20)        8 2023-05-11 14:36:31.000000 bibster-4.1.0/src/bibster.egg-info/top_level.txt
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 15:02:14.147720 bibster-4.1.1/
+-rw-r--r--   0 work       (505) staff       (20)       19 2022-03-13 22:55:00.000000 bibster-4.1.1/AUTHORS.txt
+-rw-r--r--   0 work       (505) staff       (20)     1525 2023-05-10 12:24:52.000000 bibster-4.1.1/LICENSE.txt
+-rw-r--r--   0 work       (505) staff       (20)      357 2023-01-20 12:22:36.000000 bibster-4.1.1/MANIFEST.in
+-rw-r--r--   0 work       (505) staff       (20)     1144 2023-05-12 15:02:14.147978 bibster-4.1.1/PKG-INFO
+-rw-r--r--   0 work       (505) staff       (20)      497 2023-05-11 13:28:40.000000 bibster-4.1.1/README.md
+-rw-r--r--   0 work       (505) staff       (20)      100 2021-02-16 17:38:13.000000 bibster-4.1.1/pyproject.toml
+-rw-r--r--   0 work       (505) staff       (20)     1233 2023-05-12 15:02:14.162586 bibster-4.1.1/setup.cfg
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 15:02:14.090285 bibster-4.1.1/src/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 15:02:14.107833 bibster-4.1.1/src/bibster/
+-rw-r--r--   0 work       (505) staff       (20)       50 2022-07-17 16:38:42.000000 bibster-4.1.1/src/bibster/__init__.py
+-rw-r--r--   0 work       (505) staff       (20)      383 2023-02-04 22:58:26.000000 bibster-4.1.1/src/bibster/admin_urls.py
+-rw-r--r--   0 work       (505) staff       (20)     1794 2023-03-06 23:13:41.000000 bibster-4.1.1/src/bibster/apps.py
+-rw-r--r--   0 work       (505) staff       (20)    14140 2023-03-02 13:51:17.000000 bibster-4.1.1/src/bibster/auto_fill.py
+-rw-r--r--   0 work       (505) staff       (20)    15592 2023-03-02 13:44:38.000000 bibster-4.1.1/src/bibster/auxiliaries.py
+-rw-r--r--   0 work       (505) staff       (20)    20700 2023-03-02 13:45:11.000000 bibster-4.1.1/src/bibster/block_auxiliaries.py
+-rw-r--r--   0 work       (505) staff       (20)    27302 2023-05-11 13:29:36.000000 bibster-4.1.1/src/bibster/blocks.py
+-rw-r--r--   0 work       (505) staff       (20)     1078 2023-01-25 12:16:35.000000 bibster-4.1.1/src/bibster/content_admin.py
+-rw-r--r--   0 work       (505) staff       (20)      416 2023-03-02 10:52:20.000000 bibster-4.1.1/src/bibster/default_settings.py
+-rw-r--r--   0 work       (505) staff       (20)     4687 2022-10-05 14:45:26.000000 bibster-4.1.1/src/bibster/format_auxiliaries.py
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 15:02:14.136138 bibster-4.1.1/src/bibster/formatting/
+-rw-r--r--   0 work       (505) staff       (20)      357 2022-10-16 14:34:27.000000 bibster-4.1.1/src/bibster/formatting/__init__.py
+-rw-r--r--   0 work       (505) staff       (20)     1665 2022-10-05 10:54:59.000000 bibster-4.1.1/src/bibster/formatting/base.py
+-rw-r--r--   0 work       (505) staff       (20)     5000 2023-05-12 14:48:10.000000 bibster-4.1.1/src/bibster/formatting/dictionary_format.py
+-rw-r--r--   0 work       (505) staff       (20)     1355 2022-10-04 10:11:50.000000 bibster-4.1.1/src/bibster/formatting/ellipsis.py
+-rw-r--r--   0 work       (505) staff       (20)     4937 2023-05-12 14:48:15.000000 bibster-4.1.1/src/bibster/formatting/grouping_format.py
+-rw-r--r--   0 work       (505) staff       (20)     7123 2022-10-05 11:22:36.000000 bibster-4.1.1/src/bibster/formatting/markup.py
+-rw-r--r--   0 work       (505) staff       (20)     6376 2022-10-04 10:22:24.000000 bibster-4.1.1/src/bibster/formatting/predicate_format.py
+-rw-r--r--   0 work       (505) staff       (20)     8147 2023-05-12 14:48:10.000000 bibster-4.1.1/src/bibster/formatting/sequence_format.py
+-rw-r--r--   0 work       (505) staff       (20)     2624 2022-10-04 10:40:52.000000 bibster-4.1.1/src/bibster/formatting/sequence_map.py
+-rw-r--r--   0 work       (505) staff       (20)     2857 2023-05-12 14:47:35.000000 bibster-4.1.1/src/bibster/formatting/switch_format.py
+-rw-r--r--   0 work       (505) staff       (20)     6316 2022-10-05 10:55:34.000000 bibster-4.1.1/src/bibster/formatting/titlecase.py
+-rw-r--r--   0 work       (505) staff       (20)    18651 2023-05-12 14:48:24.000000 bibster-4.1.1/src/bibster/formatting/value_converters.py
+-rw-r--r--   0 work       (505) staff       (20)     3713 2023-05-12 14:48:28.000000 bibster-4.1.1/src/bibster/formatting/value_format.py
+-rw-r--r--   0 work       (505) staff       (20)     1842 2022-10-04 10:42:10.000000 bibster-4.1.1/src/bibster/formatting/xml_io.py
+-rw-r--r--   0 work       (505) staff       (20)     1522 2023-04-04 10:32:03.000000 bibster-4.1.1/src/bibster/frontend.py
+-rw-r--r--   0 work       (505) staff       (20)    33254 2023-01-10 10:34:51.000000 bibster-4.1.1/src/bibster/harvard_style.py
+-rw-r--r--   0 work       (505) staff       (20)     7224 2023-02-03 13:33:54.000000 bibster-4.1.1/src/bibster/html_markup.py
+-rw-r--r--   0 work       (505) staff       (20)     1950 2022-10-04 11:31:05.000000 bibster-4.1.1/src/bibster/identifiers.py
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 15:02:14.137666 bibster-4.1.1/src/bibster/migrations/
+-rw-r--r--   0 work       (505) staff       (20)     8673 2023-03-07 11:38:12.000000 bibster-4.1.1/src/bibster/migrations/0001_initial.py
+-rw-r--r--   0 work       (505) staff       (20)        0 2022-10-04 12:27:23.000000 bibster-4.1.1/src/bibster/migrations/__init__.py
+-rw-r--r--   0 work       (505) staff       (20)     1718 2022-10-10 18:20:26.000000 bibster-4.1.1/src/bibster/mixins.py
+-rw-r--r--   0 work       (505) staff       (20)      919 2023-02-04 22:53:44.000000 bibster-4.1.1/src/bibster/model_admin.py
+-rw-r--r--   0 work       (505) staff       (20)     1652 2022-11-19 15:02:43.000000 bibster-4.1.1/src/bibster/model_porter.py
+-rw-r--r--   0 work       (505) staff       (20)    13239 2023-03-07 11:38:05.000000 bibster-4.1.1/src/bibster/models.py
+-rw-r--r--   0 work       (505) staff       (20)      237 2023-02-16 21:31:47.000000 bibster-4.1.1/src/bibster/permissions.py
+-rw-r--r--   0 work       (505) staff       (20)     1880 2022-10-04 12:25:03.000000 bibster-4.1.1/src/bibster/plain_name_format.py
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 15:02:14.091284 bibster-4.1.1/src/bibster/static/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 15:02:14.091723 bibster-4.1.1/src/bibster/static/bibster/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 15:02:14.138146 bibster-4.1.1/src/bibster/static/bibster/css/
+-rw-r--r--   0 work       (505) staff       (20)        0 2023-02-08 18:09:55.000000 bibster-4.1.1/src/bibster/static/bibster/css/bibster.css
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 15:02:14.140336 bibster-4.1.1/src/bibster/static/bibster/js/
+-rw-r--r--   0 work       (505) staff       (20)     2871 2023-02-04 22:56:34.000000 bibster-4.1.1/src/bibster/static/bibster/js/publication_modeladmin.js
+-rw-r--r--   0 work       (505) staff       (20)     2829 2022-07-18 08:48:15.000000 bibster-4.1.1/src/bibster/static/bibster/js/reference_block.js
+-rw-r--r--   0 work       (505) staff       (20)     6491 2022-07-18 08:49:04.000000 bibster-4.1.1/src/bibster/static/bibster/js/reference_lookup.js
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 15:02:14.092651 bibster-4.1.1/src/bibster/templates/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 15:02:14.092353 bibster-4.1.1/src/bibster/templates/bibster/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 15:02:14.143568 bibster-4.1.1/src/bibster/templates/bibster/blocks/
+-rw-r--r--   0 work       (505) staff       (20)     1795 2023-05-11 13:29:36.000000 bibster-4.1.1/src/bibster/templates/bibster/blocks/publication_list.html
+-rw-r--r--   0 work       (505) staff       (20)       90 2023-01-25 13:14:01.000000 bibster-4.1.1/src/bibster/templates/bibster/blocks/publication_list_switch.html
+-rw-r--r--   0 work       (505) staff       (20)       83 2023-02-11 13:53:57.000000 bibster-4.1.1/src/bibster/templates/bibster/blocks/publication_showcase.html
+-rw-r--r--   0 work       (505) staff       (20)       90 2023-02-11 13:53:57.000000 bibster-4.1.1/src/bibster/templates/bibster/blocks/publication_showcase_switch.html
+-rw-r--r--   0 work       (505) staff       (20)      125 2022-10-05 13:41:51.000000 bibster-4.1.1/src/bibster/templates/bibster/blocks/reference_block.html
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 15:02:14.092827 bibster-4.1.1/src/bibster/templates/modeladmin/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 15:02:14.092996 bibster-4.1.1/src/bibster/templates/modeladmin/bibster/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 15:02:14.144571 bibster-4.1.1/src/bibster/templates/modeladmin/bibster/publication/
+-rw-r--r--   0 work       (505) staff       (20)      544 2023-02-04 23:02:46.000000 bibster-4.1.1/src/bibster/templates/modeladmin/bibster/publication/index.html
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 15:02:14.145585 bibster-4.1.1/src/bibster/templatetags/
+-rw-r--r--   0 work       (505) staff       (20)        0 2022-07-18 10:45:11.000000 bibster-4.1.1/src/bibster/templatetags/__init__.py
+-rw-r--r--   0 work       (505) staff       (20)     1608 2023-04-04 13:38:30.000000 bibster-4.1.1/src/bibster/templatetags/bibster_tags.py
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 15:02:14.147211 bibster-4.1.1/src/bibster/views/
+-rw-r--r--   0 work       (505) staff       (20)        0 2022-07-17 20:44:31.000000 bibster-4.1.1/src/bibster/views/__init__.py
+-rw-r--r--   0 work       (505) staff       (20)     1800 2023-02-04 23:08:15.000000 bibster-4.1.1/src/bibster/views/action.py
+-rw-r--r--   0 work       (505) staff       (20)     1700 2023-02-16 21:32:13.000000 bibster-4.1.1/src/bibster/views/lookup.py
+-rw-r--r--   0 work       (505) staff       (20)      529 2023-02-16 21:32:13.000000 bibster-4.1.1/src/bibster/wagtail_hooks.py
+-rw-r--r--   0 work       (505) staff       (20)    22665 2019-02-06 10:42:22.000000 bibster-4.1.1/src/bibster/xml_io.py
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 15:02:14.124463 bibster-4.1.1/src/bibster.egg-info/
+-rw-r--r--   0 work       (505) staff       (20)     1144 2023-05-12 15:02:14.000000 bibster-4.1.1/src/bibster.egg-info/PKG-INFO
+-rw-r--r--   0 work       (505) staff       (20)     2218 2023-05-12 15:02:14.000000 bibster-4.1.1/src/bibster.egg-info/SOURCES.txt
+-rw-r--r--   0 work       (505) staff       (20)        1 2023-05-12 15:02:14.000000 bibster-4.1.1/src/bibster.egg-info/dependency_links.txt
+-rw-r--r--   0 work       (505) staff       (20)        1 2023-05-12 15:02:13.000000 bibster-4.1.1/src/bibster.egg-info/not-zip-safe
+-rw-r--r--   0 work       (505) staff       (20)      440 2023-05-12 15:02:14.000000 bibster-4.1.1/src/bibster.egg-info/requires.txt
+-rw-r--r--   0 work       (505) staff       (20)        8 2023-05-12 15:02:14.000000 bibster-4.1.1/src/bibster.egg-info/top_level.txt
```

### Comparing `bibster-4.1.0/LICENSE.txt` & `bibster-4.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/PKG-INFO` & `bibster-4.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibster
-Version: 4.1.0
+Version: 4.1.1
 Summary: A bibliography app for Wagtail.
 Home-page: https://github.com/high-dimensional/bibster
 Author: High Dimensional Neurology Group, UCL
 Author-email: pypi@highdimensional.net
 License: BSD-3-Clause
 Platform: any
 Classifier: Framework :: Django
```

### Comparing `bibster-4.1.0/setup.cfg` & `bibster-4.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bibster
-version = 4.1.0
+version = 4.1.1
 url = https://github.com/high-dimensional/bibster
 author = High Dimensional Neurology Group, UCL
 author_email = pypi@highdimensional.net
 description = A bibliography app for Wagtail.
 long_description = file:README.md
 long_description_content_type = text/markdown
 license = BSD-3-Clause
```

### Comparing `bibster-4.1.0/src/bibster/apps.py` & `bibster-4.1.1/src/bibster/apps.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/auto_fill.py` & `bibster-4.1.1/src/bibster/auto_fill.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/auxiliaries.py` & `bibster-4.1.1/src/bibster/auxiliaries.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/block_auxiliaries.py` & `bibster-4.1.1/src/bibster/block_auxiliaries.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/blocks.py` & `bibster-4.1.1/src/bibster/blocks.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/content_admin.py` & `bibster-4.1.1/src/bibster/content_admin.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/format_auxiliaries.py` & `bibster-4.1.1/src/bibster/format_auxiliaries.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/formatting/base.py` & `bibster-4.1.1/src/bibster/formatting/base.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/formatting/dictionary_format.py` & `bibster-4.1.1/src/bibster/formatting/dictionary_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
         super().__init__()
 
         self.xml_keyword_assignments_ = xml_capture_caller_arguments()
 
         if converter is None:
             converter = []
-        elif not isinstance(converter, collections.Iterable):
+        elif not isinstance(converter, collections.abc.Iterable):
             converter = [converter]
 
         self.converter_ = list(converter)
         self.converter_.insert(0, DictionaryConverter())
 
         if attribute_formats is None:
             attribute_formats = {}
```

### Comparing `bibster-4.1.0/src/bibster/formatting/ellipsis.py` & `bibster-4.1.1/src/bibster/formatting/ellipsis.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/formatting/grouping_format.py` & `bibster-4.1.1/src/bibster/formatting/grouping_format.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         self.xml_keyword_assignments_ = xml_capture_caller_arguments()
 
         if key_group_formats is None:
             key_group_formats = []
 
         if converter is None:
             converter = []
-        elif not isinstance(converter, collections.Iterable):
+        elif not isinstance(converter, collections.abc.Iterable):
             converter = [converter]
 
         if key_group_sequence_format is None:
             key_group_sequence_format = SequenceFormat(ValueFormat(), SequenceMap([], ""))
 
         if default_key_values is None:
             default_key_values = {}
```

### Comparing `bibster-4.1.0/src/bibster/formatting/markup.py` & `bibster-4.1.1/src/bibster/formatting/markup.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/formatting/predicate_format.py` & `bibster-4.1.1/src/bibster/formatting/predicate_format.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/formatting/sequence_format.py` & `bibster-4.1.1/src/bibster/formatting/sequence_format.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
         super().__init__()
 
         self.xml_keyword_assignments_ = xml_capture_caller_arguments()
 
         if converter is None:
             converter = []
-        elif not isinstance(converter, collections.Iterable):
+        elif not isinstance(converter, collections.abc.Iterable):
             converter = [converter]
 
         if ellipsis is None:
             ellipsis = SequenceEllipsis() # noqa
 
         self.converter_ = list(converter)
         self.converter_.insert(0, ListConverter())
```

### Comparing `bibster-4.1.0/src/bibster/formatting/sequence_map.py` & `bibster-4.1.1/src/bibster/formatting/sequence_map.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/formatting/switch_format.py` & `bibster-4.1.1/src/bibster/formatting/switch_format.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
             if isinstance(case_key, MatchAny):
                 self.default_case_format_ = case_format
                 break
 
         if converter is None:
             converter = []
-        elif not isinstance(converter, collections.Iterable):
+        elif not isinstance(converter, collections.abc.Iterable):
             converter = [converter]
 
         self.converter_ = list(converter)
         self.converter_.insert(0, DictionaryConverter())
 
         self.case_formats_ = copy.copy(case_formats)
         self.empty_substitution_value_ = empty_substitution_value
```

### Comparing `bibster-4.1.0/src/bibster/formatting/titlecase.py` & `bibster-4.1.1/src/bibster/formatting/titlecase.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/formatting/value_converters.py` & `bibster-4.1.1/src/bibster/formatting/value_converters.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,15 +391,15 @@
 
     def __init__(self):
         super().__init__()
         self.xml_keyword_assignments_ = xml_capture_caller_arguments()
 
     def __call__(self, value, path: List[Tuple[int, List[Tuple[Any, Any]]]]):
 
-        if not isinstance(value, list) and not isinstance(value, collections.Iterable):
+        if not isinstance(value, list) and not isinstance(value, collections.abc.Iterable):
             value = []
 
         for element in value:
 
             if not isinstance(element, dict) or "value" not in element:
                 continue
 
@@ -428,15 +428,15 @@
 
     def __init__(self):
         super().__init__()
         self.xml_keyword_assignments_ = xml_capture_caller_arguments()
 
     def __call__(self, value, path: List[Tuple[int, List[Tuple[Any, Any]]]]):
 
-        if not isinstance(value, list) and not isinstance(value, collections.Iterable):
+        if not isinstance(value, list) and not isinstance(value, collections.abc.Iterable):
             value = []
 
         return value
 
     def __hash__(self):
         return hash(ListConverter)
```

### Comparing `bibster-4.1.0/src/bibster/formatting/value_format.py` & `bibster-4.1.1/src/bibster/formatting/value_format.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
         super().__init__()
 
         self.xml_keyword_assignments_ = xml_capture_caller_arguments()
 
         if converter is None:
             converter = []
-        elif not isinstance(converter, collections.Iterable):
+        elif not isinstance(converter, collections.abc.Iterable):
             converter = [converter]
 
         self.converter_ = list(converter)
         self.prefix_ = prefix
         self.suffix_ = suffix
         self.inner_markup_class_ = inner_markup_class
         self.outer_markup_class_ = outer_markup_class
```

### Comparing `bibster-4.1.0/src/bibster/formatting/xml_io.py` & `bibster-4.1.1/src/bibster/formatting/xml_io.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/frontend.py` & `bibster-4.1.1/src/bibster/frontend.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/harvard_style.py` & `bibster-4.1.1/src/bibster/harvard_style.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/html_markup.py` & `bibster-4.1.1/src/bibster/html_markup.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/identifiers.py` & `bibster-4.1.1/src/bibster/identifiers.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/migrations/0001_initial.py` & `bibster-4.1.1/src/bibster/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/mixins.py` & `bibster-4.1.1/src/bibster/mixins.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/model_admin.py` & `bibster-4.1.1/src/bibster/model_admin.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/model_porter.py` & `bibster-4.1.1/src/bibster/model_porter.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/models.py` & `bibster-4.1.1/src/bibster/models.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/plain_name_format.py` & `bibster-4.1.1/src/bibster/plain_name_format.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/static/bibster/js/publication_modeladmin.js` & `bibster-4.1.1/src/bibster/static/bibster/js/publication_modeladmin.js`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/static/bibster/js/reference_block.js` & `bibster-4.1.1/src/bibster/static/bibster/js/reference_block.js`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/static/bibster/js/reference_lookup.js` & `bibster-4.1.1/src/bibster/static/bibster/js/reference_lookup.js`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/templates/bibster/blocks/publication_list.html` & `bibster-4.1.1/src/bibster/templates/bibster/blocks/publication_list.html`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/templates/modeladmin/bibster/publication/index.html` & `bibster-4.1.1/src/bibster/templates/modeladmin/bibster/publication/index.html`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/templatetags/bibster_tags.py` & `bibster-4.1.1/src/bibster/templatetags/bibster_tags.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/views/action.py` & `bibster-4.1.1/src/bibster/views/action.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/views/lookup.py` & `bibster-4.1.1/src/bibster/views/lookup.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/wagtail_hooks.py` & `bibster-4.1.1/src/bibster/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster/xml_io.py` & `bibster-4.1.1/src/bibster/xml_io.py`

 * *Files identical despite different names*

### Comparing `bibster-4.1.0/src/bibster.egg-info/PKG-INFO` & `bibster-4.1.1/src/bibster.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibster
-Version: 4.1.0
+Version: 4.1.1
 Summary: A bibliography app for Wagtail.
 Home-page: https://github.com/high-dimensional/bibster
 Author: High Dimensional Neurology Group, UCL
 Author-email: pypi@highdimensional.net
 License: BSD-3-Clause
 Platform: any
 Classifier: Framework :: Django
```

### Comparing `bibster-4.1.0/src/bibster.egg-info/SOURCES.txt` & `bibster-4.1.1/src/bibster.egg-info/SOURCES.txt`

 * *Files identical despite different names*


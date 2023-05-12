# Comparing `tmp/tour-guide-4.1.0.tar.gz` & `tmp/tour-guide-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tour-guide-4.1.0.tar", last modified: Thu May 11 14:30:53 2023, max compression
+gzip compressed data, was "tour-guide-4.1.1.tar", last modified: Fri May 12 16:34:14 2023, max compression
```

## Comparing `tour-guide-4.1.0.tar` & `tour-guide-4.1.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:30:53.006321 tour-guide-4.1.0/
--rw-r--r--   0 work       (505) staff       (20)       19 2022-03-13 22:55:00.000000 tour-guide-4.1.0/AUTHORS.txt
--rw-r--r--   0 work       (505) staff       (20)     1525 2023-05-10 12:24:52.000000 tour-guide-4.1.0/LICENSE.txt
--rw-r--r--   0 work       (505) staff       (20)      529 2023-05-11 11:37:39.000000 tour-guide-4.1.0/MANIFEST.in
--rw-r--r--   0 work       (505) staff       (20)     1186 2023-05-11 14:30:53.006473 tour-guide-4.1.0/PKG-INFO
--rw-r--r--   0 work       (505) staff       (20)      524 2023-05-11 12:03:53.000000 tour-guide-4.1.0/README.md
--rw-r--r--   0 work       (505) staff       (20)      100 2021-02-16 17:38:13.000000 tour-guide-4.1.0/pyproject.toml
--rw-r--r--   0 work       (505) staff       (20)     1118 2023-05-11 14:30:53.007136 tour-guide-4.1.0/setup.cfg
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:30:52.882741 tour-guide-4.1.0/src/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:30:52.931047 tour-guide-4.1.0/src/tour_guide/
--rw-r--r--   0 work       (505) staff       (20)       80 2023-05-11 11:34:11.000000 tour-guide-4.1.0/src/tour_guide/__init__.py
--rw-r--r--   0 work       (505) staff       (20)      620 2023-05-11 11:26:56.000000 tour-guide-4.1.0/src/tour_guide/anchor_feature_names.py
--rw-r--r--   0 work       (505) staff       (20)     7729 2023-05-11 11:26:56.000000 tour-guide-4.1.0/src/tour_guide/anchor_features.py
--rw-r--r--   0 work       (505) staff       (20)    26584 2023-02-17 11:56:07.000000 tour-guide-4.1.0/src/tour_guide/anchors.py
--rw-r--r--   0 work       (505) staff       (20)     1427 2023-05-11 11:34:37.000000 tour-guide-4.1.0/src/tour_guide/apps.py
--rw-r--r--   0 work       (505) staff       (20)    25373 2023-05-11 11:26:56.000000 tour-guide-4.1.0/src/tour_guide/blocks.py
--rw-r--r--   0 work       (505) staff       (20)     1245 2023-01-28 19:01:26.000000 tour-guide-4.1.0/src/tour_guide/categories.py
--rw-r--r--   0 work       (505) staff       (20)      560 2023-03-07 23:21:51.000000 tour-guide-4.1.0/src/tour_guide/decorators.py
--rw-r--r--   0 work       (505) staff       (20)     5198 2023-02-16 21:27:17.000000 tour-guide-4.1.0/src/tour_guide/links.py
--rw-r--r--   0 work       (505) staff       (20)     2972 2022-07-18 19:06:16.000000 tour-guide-4.1.0/src/tour_guide/middleware.py
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:30:52.935291 tour-guide-4.1.0/src/tour_guide/migrations/
--rw-r--r--   0 work       (505) staff       (20)     6229 2023-05-11 11:51:19.000000 tour-guide-4.1.0/src/tour_guide/migrations/0001_initial.py
--rw-r--r--   0 work       (505) staff       (20)     5698 2023-05-11 11:26:56.000000 tour-guide-4.1.0/src/tour_guide/migrations/0002_add_anchor_category_settings.py
--rw-r--r--   0 work       (505) staff       (20)        0 2022-03-21 21:29:30.000000 tour-guide-4.1.0/src/tour_guide/migrations/__init__.py
--rw-r--r--   0 work       (505) staff       (20)     1835 2022-07-08 13:08:22.000000 tour-guide-4.1.0/src/tour_guide/mixins.py
--rw-r--r--   0 work       (505) staff       (20)     1189 2023-01-09 11:05:28.000000 tour-guide-4.1.0/src/tour_guide/model_fields.py
--rw-r--r--   0 work       (505) staff       (20)     2853 2023-05-11 11:48:29.000000 tour-guide-4.1.0/src/tour_guide/model_porter.py
--rw-r--r--   0 work       (505) staff       (20)     9033 2023-02-24 00:32:50.000000 tour-guide-4.1.0/src/tour_guide/models.py
--rw-r--r--   0 work       (505) staff       (20)      988 2022-12-13 15:42:39.000000 tour-guide-4.1.0/src/tour_guide/navigation.py
--rw-r--r--   0 work       (505) staff       (20)      303 2023-02-16 21:27:26.000000 tour-guide-4.1.0/src/tour_guide/permissions.py
--rw-r--r--   0 work       (505) staff       (20)     6742 2022-06-06 12:44:31.000000 tour-guide-4.1.0/src/tour_guide/query.py
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:30:52.883034 tour-guide-4.1.0/src/tour_guide/static/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:30:52.883208 tour-guide-4.1.0/src/tour_guide/static/tour_guide/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:30:52.956479 tour-guide-4.1.0/src/tour_guide/static/tour_guide/css/
--rw-r--r--   0 work       (505) staff       (20)      701 2022-07-14 21:02:38.000000 tour-guide-4.1.0/src/tour_guide/static/tour_guide/css/breadcrumbs.css
--rw-r--r--   0 work       (505) staff       (20)      389 2022-07-14 21:02:47.000000 tour-guide-4.1.0/src/tour_guide/static/tour_guide/css/breadcrumbs_style.css
--rw-r--r--   0 work       (505) staff       (20)     4197 2022-10-15 13:13:08.000000 tour-guide-4.1.0/src/tour_guide/static/tour_guide/css/dropdown.css
--rw-r--r--   0 work       (505) staff       (20)     6000 2022-11-14 20:16:02.000000 tour-guide-4.1.0/src/tour_guide/static/tour_guide/css/dropdown_style.css
--rw-r--r--   0 work       (505) staff       (20)     2016 2022-12-01 21:18:41.000000 tour-guide-4.1.0/src/tour_guide/static/tour_guide/css/site_map.css
--rw-r--r--   0 work       (505) staff       (20)     2017 2022-12-13 14:04:25.000000 tour-guide-4.1.0/src/tour_guide/static/tour_guide/css/site_map_style.css
--rw-r--r--   0 work       (505) staff       (20)      687 2023-05-11 11:52:25.000000 tour-guide-4.1.0/src/tour_guide/static/tour_guide/css/tour_guide.css
--rw-r--r--   0 work       (505) staff       (20)      379 2023-01-24 15:45:44.000000 tour-guide-4.1.0/src/tour_guide/static/tour_guide/css/tour_guide_extra.css
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:30:52.958833 tour-guide-4.1.0/src/tour_guide/static/tour_guide/js/
--rw-r--r--   0 work       (505) staff       (20)     3633 2023-05-11 11:31:29.000000 tour-guide-4.1.0/src/tour_guide/static/tour_guide/js/pointer-navigation.js
--rw-r--r--   0 work       (505) staff       (20)    53273 2023-05-11 11:52:25.000000 tour-guide-4.1.0/src/tour_guide/static/tour_guide/js/tour_guide.js
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:30:52.883395 tour-guide-4.1.0/src/tour_guide/templates/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:30:52.883973 tour-guide-4.1.0/src/tour_guide/templates/tour_guide/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:30:52.961799 tour-guide-4.1.0/src/tour_guide/templates/tour_guide/blocks/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:30:52.964337 tour-guide-4.1.0/src/tour_guide/templates/tour_guide/blocks/breadcrumbs/
--rw-r--r--   0 work       (505) staff       (20)        0 2022-07-14 18:51:17.000000 tour-guide-4.1.0/src/tour_guide/templates/tour_guide/blocks/breadcrumbs/navigation_choices.html
--rw-r--r--   0 work       (505) staff       (20)        0 2022-07-14 18:51:13.000000 tour-guide-4.1.0/src/tour_guide/templates/tour_guide/blocks/breadcrumbs/navigation_container.html
--rw-r--r--   0 work       (505) staff       (20)      782 2023-05-11 11:31:29.000000 tour-guide-4.1.0/src/tour_guide/templates/tour_guide/blocks/breadcrumbs/navigation_option.html
--rw-r--r--   0 work       (505) staff       (20)      191 2023-01-29 13:52:54.000000 tour-guide-4.1.0/src/tour_guide/templates/tour_guide/blocks/breadcrumbs/navigation_wrapper.html
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:30:52.973302 tour-guide-4.1.0/src/tour_guide/templates/tour_guide/blocks/dropdown/
--rw-r--r--   0 work       (505) staff       (20)       98 2022-07-08 16:53:19.000000 tour-guide-4.1.0/src/tour_guide/templates/tour_guide/blocks/dropdown/navigation_choices.html
--rw-r--r--   0 work       (505) staff       (20)      789 2023-01-29 13:48:14.000000 tour-guide-4.1.0/src/tour_guide/templates/tour_guide/blocks/dropdown/navigation_container.html
--rw-r--r--   0 work       (505) staff       (20)      572 2023-05-11 11:31:29.000000 tour-guide-4.1.0/src/tour_guide/templates/tour_guide/blocks/dropdown/navigation_option.html
--rw-r--r--   0 work       (505) staff       (20)      855 2023-01-29 14:25:35.000000 tour-guide-4.1.0/src/tour_guide/templates/tour_guide/blocks/dropdown/navigation_wrapper.html
--rw-r--r--   0 work       (505) staff       (20)      117 2023-05-11 11:31:29.000000 tour-guide-4.1.0/src/tour_guide/templates/tour_guide/blocks/navigation_block.html
--rw-r--r--   0 work       (505) staff       (20)      402 2022-10-06 13:05:24.000000 tour-guide-4.1.0/src/tour_guide/templates/tour_guide/blocks/rich_link_block.html
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:30:53.003652 tour-guide-4.1.0/src/tour_guide/templates/tour_guide/blocks/site_map/
--rw-r--r--   0 work       (505) staff       (20)       98 2022-07-08 16:53:19.000000 tour-guide-4.1.0/src/tour_guide/templates/tour_guide/blocks/site_map/navigation_choices.html
--rw-r--r--   0 work       (505) staff       (20)      396 2023-01-29 13:53:36.000000 tour-guide-4.1.0/src/tour_guide/templates/tour_guide/blocks/site_map/navigation_container.html
--rw-r--r--   0 work       (505) staff       (20)      572 2023-05-11 11:31:29.000000 tour-guide-4.1.0/src/tour_guide/templates/tour_guide/blocks/site_map/navigation_option.html
--rw-r--r--   0 work       (505) staff       (20)      246 2023-01-29 13:54:20.000000 tour-guide-4.1.0/src/tour_guide/templates/tour_guide/blocks/site_map/navigation_wrapper.html
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:30:53.004311 tour-guide-4.1.0/src/tour_guide/templates/tour_guide/tags/
--rw-r--r--   0 work       (505) staff       (20)      350 2022-06-05 13:13:35.000000 tour-guide-4.1.0/src/tour_guide/templates/tour_guide/tags/support.html
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:30:53.005667 tour-guide-4.1.0/src/tour_guide/templatetags/
--rw-r--r--   0 work       (505) staff       (20)        0 2018-09-12 10:34:17.000000 tour-guide-4.1.0/src/tour_guide/templatetags/__init__.py
--rw-r--r--   0 work       (505) staff       (20)     4778 2023-05-11 11:26:56.000000 tour-guide-4.1.0/src/tour_guide/templatetags/tour_guide_tags.py
--rw-r--r--   0 work       (505) staff       (20)     1382 2023-01-28 18:08:42.000000 tour-guide-4.1.0/src/tour_guide/utilities.py
--rw-r--r--   0 work       (505) staff       (20)      414 2022-07-05 13:48:21.000000 tour-guide-4.1.0/src/tour_guide/validators.py
--rw-r--r--   0 work       (505) staff       (20)      640 2023-04-04 10:28:57.000000 tour-guide-4.1.0/src/tour_guide/wagtail_hooks.py
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-11 14:30:52.933485 tour-guide-4.1.0/src/tour_guide.egg-info/
--rw-r--r--   0 work       (505) staff       (20)     1186 2023-05-11 14:30:52.000000 tour-guide-4.1.0/src/tour_guide.egg-info/PKG-INFO
--rw-r--r--   0 work       (505) staff       (20)     2743 2023-05-11 14:30:52.000000 tour-guide-4.1.0/src/tour_guide.egg-info/SOURCES.txt
--rw-r--r--   0 work       (505) staff       (20)        1 2023-05-11 14:30:52.000000 tour-guide-4.1.0/src/tour_guide.egg-info/dependency_links.txt
--rw-r--r--   0 work       (505) staff       (20)      316 2023-05-11 14:30:52.000000 tour-guide-4.1.0/src/tour_guide.egg-info/requires.txt
--rw-r--r--   0 work       (505) staff       (20)       11 2023-05-11 14:30:52.000000 tour-guide-4.1.0/src/tour_guide.egg-info/top_level.txt
--rw-r--r--   0 work       (505) staff       (20)        1 2023-05-11 14:30:52.000000 tour-guide-4.1.0/src/tour_guide.egg-info/zip-safe
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:34:14.655337 tour-guide-4.1.1/
+-rw-r--r--   0 work       (505) staff       (20)       19 2022-03-13 22:55:00.000000 tour-guide-4.1.1/AUTHORS.txt
+-rw-r--r--   0 work       (505) staff       (20)     1525 2023-05-10 12:24:52.000000 tour-guide-4.1.1/LICENSE.txt
+-rw-r--r--   0 work       (505) staff       (20)      529 2023-05-11 11:37:39.000000 tour-guide-4.1.1/MANIFEST.in
+-rw-r--r--   0 work       (505) staff       (20)     1186 2023-05-12 16:34:14.655475 tour-guide-4.1.1/PKG-INFO
+-rw-r--r--   0 work       (505) staff       (20)      524 2023-05-11 12:03:53.000000 tour-guide-4.1.1/README.md
+-rw-r--r--   0 work       (505) staff       (20)      100 2021-02-16 17:38:13.000000 tour-guide-4.1.1/pyproject.toml
+-rw-r--r--   0 work       (505) staff       (20)     1118 2023-05-12 16:34:14.656217 tour-guide-4.1.1/setup.cfg
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:34:14.176952 tour-guide-4.1.1/src/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:34:14.392793 tour-guide-4.1.1/src/tour_guide/
+-rw-r--r--   0 work       (505) staff       (20)       80 2023-05-11 11:34:11.000000 tour-guide-4.1.1/src/tour_guide/__init__.py
+-rw-r--r--   0 work       (505) staff       (20)      620 2023-05-11 11:26:56.000000 tour-guide-4.1.1/src/tour_guide/anchor_feature_names.py
+-rw-r--r--   0 work       (505) staff       (20)     7729 2023-05-11 11:26:56.000000 tour-guide-4.1.1/src/tour_guide/anchor_features.py
+-rw-r--r--   0 work       (505) staff       (20)    26584 2023-02-17 11:56:07.000000 tour-guide-4.1.1/src/tour_guide/anchors.py
+-rw-r--r--   0 work       (505) staff       (20)     1427 2023-05-11 11:34:37.000000 tour-guide-4.1.1/src/tour_guide/apps.py
+-rw-r--r--   0 work       (505) staff       (20)    25373 2023-05-11 11:26:56.000000 tour-guide-4.1.1/src/tour_guide/blocks.py
+-rw-r--r--   0 work       (505) staff       (20)     1245 2023-01-28 19:01:26.000000 tour-guide-4.1.1/src/tour_guide/categories.py
+-rw-r--r--   0 work       (505) staff       (20)      560 2023-03-07 23:21:51.000000 tour-guide-4.1.1/src/tour_guide/decorators.py
+-rw-r--r--   0 work       (505) staff       (20)     5198 2023-02-16 21:27:17.000000 tour-guide-4.1.1/src/tour_guide/links.py
+-rw-r--r--   0 work       (505) staff       (20)     2972 2022-07-18 19:06:16.000000 tour-guide-4.1.1/src/tour_guide/middleware.py
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:34:14.426569 tour-guide-4.1.1/src/tour_guide/migrations/
+-rw-r--r--   0 work       (505) staff       (20)     6229 2023-05-11 11:51:19.000000 tour-guide-4.1.1/src/tour_guide/migrations/0001_initial.py
+-rw-r--r--   0 work       (505) staff       (20)     5698 2023-05-11 11:26:56.000000 tour-guide-4.1.1/src/tour_guide/migrations/0002_add_anchor_category_settings.py
+-rw-r--r--   0 work       (505) staff       (20)        0 2022-03-21 21:29:30.000000 tour-guide-4.1.1/src/tour_guide/migrations/__init__.py
+-rw-r--r--   0 work       (505) staff       (20)     1835 2022-07-08 13:08:22.000000 tour-guide-4.1.1/src/tour_guide/mixins.py
+-rw-r--r--   0 work       (505) staff       (20)     1189 2023-01-09 11:05:28.000000 tour-guide-4.1.1/src/tour_guide/model_fields.py
+-rw-r--r--   0 work       (505) staff       (20)     2853 2023-05-11 11:48:29.000000 tour-guide-4.1.1/src/tour_guide/model_porter.py
+-rw-r--r--   0 work       (505) staff       (20)     9033 2023-02-24 00:32:50.000000 tour-guide-4.1.1/src/tour_guide/models.py
+-rw-r--r--   0 work       (505) staff       (20)      988 2022-12-13 15:42:39.000000 tour-guide-4.1.1/src/tour_guide/navigation.py
+-rw-r--r--   0 work       (505) staff       (20)      303 2023-02-16 21:27:26.000000 tour-guide-4.1.1/src/tour_guide/permissions.py
+-rw-r--r--   0 work       (505) staff       (20)     6742 2022-06-06 12:44:31.000000 tour-guide-4.1.1/src/tour_guide/query.py
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:34:14.177333 tour-guide-4.1.1/src/tour_guide/static/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:34:14.177561 tour-guide-4.1.1/src/tour_guide/static/tour_guide/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:34:14.496180 tour-guide-4.1.1/src/tour_guide/static/tour_guide/css/
+-rw-r--r--   0 work       (505) staff       (20)      701 2022-07-14 21:02:38.000000 tour-guide-4.1.1/src/tour_guide/static/tour_guide/css/breadcrumbs.css
+-rw-r--r--   0 work       (505) staff       (20)      389 2022-07-14 21:02:47.000000 tour-guide-4.1.1/src/tour_guide/static/tour_guide/css/breadcrumbs_style.css
+-rw-r--r--   0 work       (505) staff       (20)     4197 2022-10-15 13:13:08.000000 tour-guide-4.1.1/src/tour_guide/static/tour_guide/css/dropdown.css
+-rw-r--r--   0 work       (505) staff       (20)     6000 2022-11-14 20:16:02.000000 tour-guide-4.1.1/src/tour_guide/static/tour_guide/css/dropdown_style.css
+-rw-r--r--   0 work       (505) staff       (20)     2016 2022-12-01 21:18:41.000000 tour-guide-4.1.1/src/tour_guide/static/tour_guide/css/site_map.css
+-rw-r--r--   0 work       (505) staff       (20)     2017 2022-12-13 14:04:25.000000 tour-guide-4.1.1/src/tour_guide/static/tour_guide/css/site_map_style.css
+-rw-r--r--   0 work       (505) staff       (20)      687 2023-05-11 11:52:25.000000 tour-guide-4.1.1/src/tour_guide/static/tour_guide/css/tour_guide.css
+-rw-r--r--   0 work       (505) staff       (20)      379 2023-01-24 15:45:44.000000 tour-guide-4.1.1/src/tour_guide/static/tour_guide/css/tour_guide_extra.css
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:34:14.527747 tour-guide-4.1.1/src/tour_guide/static/tour_guide/js/
+-rw-r--r--   0 work       (505) staff       (20)     3633 2023-05-11 11:31:29.000000 tour-guide-4.1.1/src/tour_guide/static/tour_guide/js/pointer-navigation.js
+-rw-r--r--   0 work       (505) staff       (20)    53273 2023-05-11 11:52:25.000000 tour-guide-4.1.1/src/tour_guide/static/tour_guide/js/tour_guide.js
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:34:14.177797 tour-guide-4.1.1/src/tour_guide/templates/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:34:14.178465 tour-guide-4.1.1/src/tour_guide/templates/tour_guide/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:34:14.541553 tour-guide-4.1.1/src/tour_guide/templates/tour_guide/blocks/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:34:14.554563 tour-guide-4.1.1/src/tour_guide/templates/tour_guide/blocks/breadcrumbs/
+-rw-r--r--   0 work       (505) staff       (20)        0 2022-07-14 18:51:17.000000 tour-guide-4.1.1/src/tour_guide/templates/tour_guide/blocks/breadcrumbs/navigation_choices.html
+-rw-r--r--   0 work       (505) staff       (20)        0 2022-07-14 18:51:13.000000 tour-guide-4.1.1/src/tour_guide/templates/tour_guide/blocks/breadcrumbs/navigation_container.html
+-rw-r--r--   0 work       (505) staff       (20)      782 2023-05-11 11:31:29.000000 tour-guide-4.1.1/src/tour_guide/templates/tour_guide/blocks/breadcrumbs/navigation_option.html
+-rw-r--r--   0 work       (505) staff       (20)      191 2023-01-29 13:52:54.000000 tour-guide-4.1.1/src/tour_guide/templates/tour_guide/blocks/breadcrumbs/navigation_wrapper.html
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:34:14.594253 tour-guide-4.1.1/src/tour_guide/templates/tour_guide/blocks/dropdown/
+-rw-r--r--   0 work       (505) staff       (20)       98 2022-07-08 16:53:19.000000 tour-guide-4.1.1/src/tour_guide/templates/tour_guide/blocks/dropdown/navigation_choices.html
+-rw-r--r--   0 work       (505) staff       (20)      789 2023-01-29 13:48:14.000000 tour-guide-4.1.1/src/tour_guide/templates/tour_guide/blocks/dropdown/navigation_container.html
+-rw-r--r--   0 work       (505) staff       (20)      572 2023-05-11 11:31:29.000000 tour-guide-4.1.1/src/tour_guide/templates/tour_guide/blocks/dropdown/navigation_option.html
+-rw-r--r--   0 work       (505) staff       (20)      855 2023-01-29 14:25:35.000000 tour-guide-4.1.1/src/tour_guide/templates/tour_guide/blocks/dropdown/navigation_wrapper.html
+-rw-r--r--   0 work       (505) staff       (20)      117 2023-05-11 11:31:29.000000 tour-guide-4.1.1/src/tour_guide/templates/tour_guide/blocks/navigation_block.html
+-rw-r--r--   0 work       (505) staff       (20)      402 2022-10-06 13:05:24.000000 tour-guide-4.1.1/src/tour_guide/templates/tour_guide/blocks/rich_link_block.html
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:34:14.637871 tour-guide-4.1.1/src/tour_guide/templates/tour_guide/blocks/site_map/
+-rw-r--r--   0 work       (505) staff       (20)       98 2022-07-08 16:53:19.000000 tour-guide-4.1.1/src/tour_guide/templates/tour_guide/blocks/site_map/navigation_choices.html
+-rw-r--r--   0 work       (505) staff       (20)      396 2023-01-29 13:53:36.000000 tour-guide-4.1.1/src/tour_guide/templates/tour_guide/blocks/site_map/navigation_container.html
+-rw-r--r--   0 work       (505) staff       (20)      572 2023-05-11 11:31:29.000000 tour-guide-4.1.1/src/tour_guide/templates/tour_guide/blocks/site_map/navigation_option.html
+-rw-r--r--   0 work       (505) staff       (20)      246 2023-01-29 13:54:20.000000 tour-guide-4.1.1/src/tour_guide/templates/tour_guide/blocks/site_map/navigation_wrapper.html
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:34:14.644838 tour-guide-4.1.1/src/tour_guide/templates/tour_guide/tags/
+-rw-r--r--   0 work       (505) staff       (20)      350 2022-06-05 13:13:35.000000 tour-guide-4.1.1/src/tour_guide/templates/tour_guide/tags/support.html
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:34:14.654975 tour-guide-4.1.1/src/tour_guide/templatetags/
+-rw-r--r--   0 work       (505) staff       (20)        0 2018-09-12 10:34:17.000000 tour-guide-4.1.1/src/tour_guide/templatetags/__init__.py
+-rw-r--r--   0 work       (505) staff       (20)     4778 2023-05-11 11:26:56.000000 tour-guide-4.1.1/src/tour_guide/templatetags/tour_guide_tags.py
+-rw-r--r--   0 work       (505) staff       (20)     1386 2023-05-12 14:45:00.000000 tour-guide-4.1.1/src/tour_guide/utilities.py
+-rw-r--r--   0 work       (505) staff       (20)      414 2022-07-05 13:48:21.000000 tour-guide-4.1.1/src/tour_guide/validators.py
+-rw-r--r--   0 work       (505) staff       (20)      640 2023-04-04 10:28:57.000000 tour-guide-4.1.1/src/tour_guide/wagtail_hooks.py
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:34:14.397270 tour-guide-4.1.1/src/tour_guide.egg-info/
+-rw-r--r--   0 work       (505) staff       (20)     1186 2023-05-12 16:34:14.000000 tour-guide-4.1.1/src/tour_guide.egg-info/PKG-INFO
+-rw-r--r--   0 work       (505) staff       (20)     2743 2023-05-12 16:34:14.000000 tour-guide-4.1.1/src/tour_guide.egg-info/SOURCES.txt
+-rw-r--r--   0 work       (505) staff       (20)        1 2023-05-12 16:34:14.000000 tour-guide-4.1.1/src/tour_guide.egg-info/dependency_links.txt
+-rw-r--r--   0 work       (505) staff       (20)      316 2023-05-12 16:34:14.000000 tour-guide-4.1.1/src/tour_guide.egg-info/requires.txt
+-rw-r--r--   0 work       (505) staff       (20)       11 2023-05-12 16:34:14.000000 tour-guide-4.1.1/src/tour_guide.egg-info/top_level.txt
+-rw-r--r--   0 work       (505) staff       (20)        1 2023-05-12 16:34:13.000000 tour-guide-4.1.1/src/tour_guide.egg-info/zip-safe
```

### Comparing `tour-guide-4.1.0/LICENSE.txt` & `tour-guide-4.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/MANIFEST.in` & `tour-guide-4.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/PKG-INFO` & `tour-guide-4.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tour-guide
-Version: 4.1.0
+Version: 4.1.1
 Summary: A Wagtail app for navigation components.
 Home-page: https://github.com/high-dimensional/tour-guide
 Author: High Dimensional Neurology Group, UCL
 Author-email: pypi@highdimensional.net
 License: BSD-3-Clause
 Platform: any
 Classifier: Framework :: Django
```

### Comparing `tour-guide-4.1.0/README.md` & `tour-guide-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/setup.cfg` & `tour-guide-4.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tour-guide
-version = 4.1.0
+version = 4.1.1
 url = https://github.com/high-dimensional/tour-guide
 author = High Dimensional Neurology Group, UCL
 author_email = pypi@highdimensional.net
 description = A Wagtail app for navigation components.
 long_description = file:README.md
 long_description_content_type = text/markdown
 license = BSD-3-Clause
```

### Comparing `tour-guide-4.1.0/src/tour_guide/anchor_feature_names.py` & `tour-guide-4.1.1/src/tour_guide/anchor_feature_names.py`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/anchor_features.py` & `tour-guide-4.1.1/src/tour_guide/anchor_features.py`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/anchors.py` & `tour-guide-4.1.1/src/tour_guide/anchors.py`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/apps.py` & `tour-guide-4.1.1/src/tour_guide/apps.py`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/blocks.py` & `tour-guide-4.1.1/src/tour_guide/blocks.py`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/categories.py` & `tour-guide-4.1.1/src/tour_guide/categories.py`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/decorators.py` & `tour-guide-4.1.1/src/tour_guide/decorators.py`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/links.py` & `tour-guide-4.1.1/src/tour_guide/links.py`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/middleware.py` & `tour-guide-4.1.1/src/tour_guide/middleware.py`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/migrations/0001_initial.py` & `tour-guide-4.1.1/src/tour_guide/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/migrations/0002_add_anchor_category_settings.py` & `tour-guide-4.1.1/src/tour_guide/migrations/0002_add_anchor_category_settings.py`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/mixins.py` & `tour-guide-4.1.1/src/tour_guide/mixins.py`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/model_fields.py` & `tour-guide-4.1.1/src/tour_guide/model_fields.py`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/model_porter.py` & `tour-guide-4.1.1/src/tour_guide/model_porter.py`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/models.py` & `tour-guide-4.1.1/src/tour_guide/models.py`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/navigation.py` & `tour-guide-4.1.1/src/tour_guide/navigation.py`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/query.py` & `tour-guide-4.1.1/src/tour_guide/query.py`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/static/tour_guide/css/breadcrumbs.css` & `tour-guide-4.1.1/src/tour_guide/static/tour_guide/css/breadcrumbs.css`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/static/tour_guide/css/dropdown.css` & `tour-guide-4.1.1/src/tour_guide/static/tour_guide/css/dropdown.css`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/static/tour_guide/css/dropdown_style.css` & `tour-guide-4.1.1/src/tour_guide/static/tour_guide/css/dropdown_style.css`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/static/tour_guide/css/site_map.css` & `tour-guide-4.1.1/src/tour_guide/static/tour_guide/css/site_map.css`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/static/tour_guide/css/site_map_style.css` & `tour-guide-4.1.1/src/tour_guide/static/tour_guide/css/site_map_style.css`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/static/tour_guide/css/tour_guide.css` & `tour-guide-4.1.1/src/tour_guide/static/tour_guide/css/tour_guide.css`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/static/tour_guide/js/pointer-navigation.js` & `tour-guide-4.1.1/src/tour_guide/static/tour_guide/js/pointer-navigation.js`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/static/tour_guide/js/tour_guide.js` & `tour-guide-4.1.1/src/tour_guide/static/tour_guide/js/tour_guide.js`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/templates/tour_guide/blocks/breadcrumbs/navigation_option.html` & `tour-guide-4.1.1/src/tour_guide/templates/tour_guide/blocks/breadcrumbs/navigation_option.html`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/templates/tour_guide/blocks/dropdown/navigation_container.html` & `tour-guide-4.1.1/src/tour_guide/templates/tour_guide/blocks/dropdown/navigation_container.html`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/templates/tour_guide/blocks/dropdown/navigation_option.html` & `tour-guide-4.1.1/src/tour_guide/templates/tour_guide/blocks/dropdown/navigation_option.html`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/templates/tour_guide/blocks/dropdown/navigation_wrapper.html` & `tour-guide-4.1.1/src/tour_guide/templates/tour_guide/blocks/dropdown/navigation_wrapper.html`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/templates/tour_guide/blocks/site_map/navigation_option.html` & `tour-guide-4.1.1/src/tour_guide/templates/tour_guide/blocks/site_map/navigation_option.html`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/templatetags/tour_guide_tags.py` & `tour-guide-4.1.1/src/tour_guide/templatetags/tour_guide_tags.py`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide/utilities.py` & `tour-guide-4.1.1/src/tour_guide/utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-from collections import Sequence
+from collections.abc import Sequence
 
 from django.utils.translation import get_language_from_request
 
 from wagtail.models import Site
 
 from .apps import get_app_label
```

### Comparing `tour-guide-4.1.0/src/tour_guide/wagtail_hooks.py` & `tour-guide-4.1.1/src/tour_guide/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `tour-guide-4.1.0/src/tour_guide.egg-info/PKG-INFO` & `tour-guide-4.1.1/src/tour_guide.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tour-guide
-Version: 4.1.0
+Version: 4.1.1
 Summary: A Wagtail app for navigation components.
 Home-page: https://github.com/high-dimensional/tour-guide
 Author: High Dimensional Neurology Group, UCL
 Author-email: pypi@highdimensional.net
 License: BSD-3-Clause
 Platform: any
 Classifier: Framework :: Django
```

### Comparing `tour-guide-4.1.0/src/tour_guide.egg-info/SOURCES.txt` & `tour-guide-4.1.1/src/tour_guide.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/garpixcms-4.0.0rc9.tar.gz` & `tmp/garpixcms-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpixcms-4.0.0rc9.tar", last modified: Fri Mar 24 12:30:41 2023, max compression
+gzip compressed data, was "garpixcms-4.1.0.tar", last modified: Fri May 12 09:55:15 2023, max compression
```

## Comparing `garpixcms-4.0.0rc9.tar` & `garpixcms-4.1.0.tar`

### file list

```diff
@@ -1,109 +1,103 @@
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.339255 garpixcms-4.0.0rc9/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       30 2023-03-24 12:30:41.000000 garpixcms-4.0.0rc9/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1769 2023-03-24 12:30:41.339075 garpixcms-4.0.0rc9/PKG-INFO
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.297014 garpixcms-4.0.0rc9/garpixcms/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    12359 2023-03-24 12:30:31.000000 garpixcms-4.0.0rc9/garpixcms/CHANGELOG.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1084 2022-10-06 14:32:51.000000 garpixcms-4.0.0rc9/garpixcms/CONTRIBUTING.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       30 2022-06-29 08:47:07.000000 garpixcms-4.0.0rc9/garpixcms/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1207 2023-03-09 03:45:19.000000 garpixcms-4.0.0rc9/garpixcms/README.rst
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-06-29 08:47:07.000000 garpixcms-4.0.0rc9/garpixcms/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.303423 garpixcms-4.0.0rc9/garpixcms/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      161 2022-08-16 12:23:45.000000 garpixcms-4.0.0rc9/garpixcms/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      387 2022-10-07 14:06:21.000000 garpixcms-4.0.0rc9/garpixcms/__pycache__/apps.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6796 2023-03-13 04:19:08.000000 garpixcms-4.0.0rc9/garpixcms/__pycache__/settings.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1743 2023-03-09 03:45:38.000000 garpixcms-4.0.0rc9/garpixcms/__pycache__/urls.cpython-38.pyc
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.303673 garpixcms-4.0.0rc9/garpixcms/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       36 2022-06-29 08:47:07.000000 garpixcms-4.0.0rc9/garpixcms/admin/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.303920 garpixcms-4.0.0rc9/garpixcms/admin/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      205 2022-08-16 12:23:55.000000 garpixcms-4.0.0rc9/garpixcms/admin/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      487 2022-08-16 12:23:55.000000 garpixcms-4.0.0rc9/garpixcms/admin/__pycache__/page.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      173 2022-06-29 08:47:07.000000 garpixcms-4.0.0rc9/garpixcms/admin/page.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       93 2022-10-07 14:06:19.000000 garpixcms-4.0.0rc9/garpixcms/apps.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.306566 garpixcms-4.0.0rc9/garpixcms/contexts/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-06-29 08:47:07.000000 garpixcms-4.0.0rc9/garpixcms/contexts/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.307336 garpixcms-4.0.0rc9/garpixcms/contexts/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      170 2022-08-16 12:23:57.000000 garpixcms-4.0.0rc9/garpixcms/contexts/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      948 2023-02-10 12:24:11.000000 garpixcms-4.0.0rc9/garpixcms/contexts/__pycache__/global_context.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      691 2023-03-07 14:17:49.000000 garpixcms-4.0.0rc9/garpixcms/contexts/global_context.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.307742 garpixcms-4.0.0rc9/garpixcms/management/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-03-09 03:45:19.000000 garpixcms-4.0.0rc9/garpixcms/management/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.307870 garpixcms-4.0.0rc9/garpixcms/management/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      172 2023-03-13 04:19:20.000000 garpixcms-4.0.0rc9/garpixcms/management/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.308176 garpixcms-4.0.0rc9/garpixcms/management/commands/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-03-09 03:45:19.000000 garpixcms-4.0.0rc9/garpixcms/management/commands/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.319476 garpixcms-4.0.0rc9/garpixcms/management/commands/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      181 2022-11-07 06:29:29.000000 garpixcms-4.0.0rc9/garpixcms/management/commands/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1217 2022-11-07 06:29:29.000000 garpixcms-4.0.0rc9/garpixcms/management/commands/__pycache__/update_user_module.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      872 2023-03-09 03:45:19.000000 garpixcms-4.0.0rc9/garpixcms/management/commands/update_user_module.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.321612 garpixcms-4.0.0rc9/garpixcms/middleware/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-03-07 14:17:49.000000 garpixcms-4.0.0rc9/garpixcms/middleware/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.322032 garpixcms-4.0.0rc9/garpixcms/middleware/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      172 2023-03-09 03:38:29.000000 garpixcms-4.0.0rc9/garpixcms/middleware/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2037 2023-03-09 03:38:29.000000 garpixcms-4.0.0rc9/garpixcms/middleware/__pycache__/locale.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2196 2023-03-07 14:17:49.000000 garpixcms-4.0.0rc9/garpixcms/middleware/locale.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.322322 garpixcms-4.0.0rc9/garpixcms/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2022-10-07 15:53:24.000000 garpixcms-4.0.0rc9/garpixcms/models/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.322760 garpixcms-4.0.0rc9/garpixcms/models/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      201 2022-10-07 15:53:42.000000 garpixcms-4.0.0rc9/garpixcms/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      818 2022-08-16 12:23:46.000000 garpixcms-4.0.0rc9/garpixcms/models/__pycache__/page.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      413 2022-06-29 08:47:07.000000 garpixcms-4.0.0rc9/garpixcms/models/page.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8440 2023-03-09 04:14:34.000000 garpixcms-4.0.0rc9/garpixcms/settings.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1709 2023-03-24 12:30:06.000000 garpixcms-4.0.0rc9/garpixcms/setup.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.289338 garpixcms-4.0.0rc9/garpixcms/static/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.289539 garpixcms-4.0.0rc9/garpixcms/static/admin/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.335081 garpixcms-4.0.0rc9/garpixcms/static/admin/css/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8440 2023-03-07 14:17:49.000000 garpixcms-4.0.0rc9/garpixcms/static/admin/css/autocomplete.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    22662 2023-03-09 10:18:42.000000 garpixcms-4.0.0rc9/garpixcms/static/admin/css/base.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6469 2023-03-07 14:17:49.000000 garpixcms-4.0.0rc9/garpixcms/static/admin/css/changelists.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      355 2023-03-07 14:17:49.000000 garpixcms-4.0.0rc9/garpixcms/static/admin/css/dashboard.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      423 2023-03-07 14:17:49.000000 garpixcms-4.0.0rc9/garpixcms/static/admin/css/fonts.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8370 2023-03-07 14:17:49.000000 garpixcms-4.0.0rc9/garpixcms/static/admin/css/forms.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1185 2023-03-07 14:17:49.000000 garpixcms-4.0.0rc9/garpixcms/static/admin/css/login.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2505 2023-03-07 14:17:49.000000 garpixcms-4.0.0rc9/garpixcms/static/admin/css/nav_sidebar.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    18344 2023-03-07 14:17:49.000000 garpixcms-4.0.0rc9/garpixcms/static/admin/css/responsive.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1741 2023-03-07 14:17:49.000000 garpixcms-4.0.0rc9/garpixcms/static/admin/css/responsive_rtl.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3487 2023-03-07 14:17:49.000000 garpixcms-4.0.0rc9/garpixcms/static/admin/css/rtl.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      502 2023-03-07 14:17:49.000000 garpixcms-4.0.0rc9/garpixcms/static/admin/css/tabbed_translation_fields.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    10010 2023-03-07 14:17:49.000000 garpixcms-4.0.0rc9/garpixcms/static/admin/css/widgets.css
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.336137 garpixcms-4.0.0rc9/garpixcms/static/admin/img/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      908 2023-03-07 14:17:49.000000 garpixcms-4.0.0rc9/garpixcms/static/admin/img/icon-addlink.svg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      825 2023-03-07 14:17:49.000000 garpixcms-4.0.0rc9/garpixcms/static/admin/img/icon-changelink.svg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      218 2023-03-07 14:17:49.000000 garpixcms-4.0.0rc9/garpixcms/static/admin/img/icon-custom-checked.svg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      705 2023-03-07 14:17:49.000000 garpixcms-4.0.0rc9/garpixcms/static/admin/img/icon-deletelink.svg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      930 2023-03-07 14:17:49.000000 garpixcms-4.0.0rc9/garpixcms/static/admin/img/search.svg
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.336270 garpixcms-4.0.0rc9/garpixcms/static/admin/js/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      291 2023-03-07 14:17:49.000000 garpixcms-4.0.0rc9/garpixcms/static/admin/js/admin.js
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.289764 garpixcms-4.0.0rc9/garpixcms/templates/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.336771 garpixcms-4.0.0rc9/garpixcms/templates/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4421 2023-03-07 14:17:49.000000 garpixcms-4.0.0rc9/garpixcms/templates/admin/app_list.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4395 2023-03-07 14:17:49.000000 garpixcms-4.0.0rc9/garpixcms/templates/admin/base.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      809 2023-03-07 14:17:49.000000 garpixcms-4.0.0rc9/garpixcms/templates/admin/base_site.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.336910 garpixcms-4.0.0rc9/garpixcms/templates/garpixcms/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      450 2022-06-29 08:47:07.000000 garpixcms-4.0.0rc9/garpixcms/templates/garpixcms/base.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.337397 garpixcms-4.0.0rc9/garpixcms/templates/garpixcms/include/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      730 2022-06-29 08:47:07.000000 garpixcms-4.0.0rc9/garpixcms/templates/garpixcms/include/footer.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      642 2022-06-29 08:47:07.000000 garpixcms-4.0.0rc9/garpixcms/templates/garpixcms/include/header.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      428 2022-06-29 08:47:07.000000 garpixcms-4.0.0rc9/garpixcms/templates/garpixcms/include/login.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.337665 garpixcms-4.0.0rc9/garpixcms/templates/garpixcms/menus/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      202 2022-06-29 08:47:07.000000 garpixcms-4.0.0rc9/garpixcms/templates/garpixcms/menus/footer_menu.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      369 2022-06-29 08:47:07.000000 garpixcms-4.0.0rc9/garpixcms/templates/garpixcms/menus/header_menu.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.338305 garpixcms-4.0.0rc9/garpixcms/templates/garpixcms/pages/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      139 2022-06-29 08:47:07.000000 garpixcms-4.0.0rc9/garpixcms/templates/garpixcms/pages/default.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      202 2022-06-29 08:47:07.000000 garpixcms-4.0.0rc9/garpixcms/templates/garpixcms/pages/home.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      346 2022-06-29 08:47:07.000000 garpixcms-4.0.0rc9/garpixcms/templates/garpixcms/pages/login.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.338563 garpixcms-4.0.0rc9/garpixcms/translation/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       49 2022-06-29 08:47:07.000000 garpixcms-4.0.0rc9/garpixcms/translation/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.338853 garpixcms-4.0.0rc9/garpixcms/translation/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      224 2022-08-16 12:23:46.000000 garpixcms-4.0.0rc9/garpixcms/translation/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      502 2022-08-16 12:23:46.000000 garpixcms-4.0.0rc9/garpixcms/translation/__pycache__/page.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      189 2022-06-29 08:47:07.000000 garpixcms-4.0.0rc9/garpixcms/translation/page.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1842 2023-03-09 03:45:19.000000 garpixcms-4.0.0rc9/garpixcms/urls.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-03-24 12:30:41.302852 garpixcms-4.0.0rc9/garpixcms.egg-info/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1769 2023-03-24 12:30:41.000000 garpixcms-4.0.0rc9/garpixcms.egg-info/PKG-INFO
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3106 2023-03-24 12:30:41.000000 garpixcms-4.0.0rc9/garpixcms.egg-info/SOURCES.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-03-24 12:30:41.000000 garpixcms-4.0.0rc9/garpixcms.egg-info/dependency_links.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-03-24 12:30:41.000000 garpixcms-4.0.0rc9/garpixcms.egg-info/not-zip-safe
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      409 2023-03-24 12:30:41.000000 garpixcms-4.0.0rc9/garpixcms.egg-info/requires.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       10 2023-03-24 12:30:41.000000 garpixcms-4.0.0rc9/garpixcms.egg-info/top_level.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-03-24 12:30:41.339300 garpixcms-4.0.0rc9/setup.cfg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1709 2023-03-24 12:30:41.000000 garpixcms-4.0.0rc9/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.296266 garpixcms-4.1.0/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       30 2023-05-12 09:55:15.000000 garpixcms-4.1.0/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1766 2023-05-12 09:55:15.296028 garpixcms-4.1.0/PKG-INFO
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.242392 garpixcms-4.1.0/garpixcms/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    13299 2023-05-12 09:51:39.000000 garpixcms-4.1.0/garpixcms/CHANGELOG.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1084 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/CONTRIBUTING.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       30 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1207 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/README.rst
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.243751 garpixcms-4.1.0/garpixcms/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      161 2023-04-18 20:28:30.000000 garpixcms-4.1.0/garpixcms/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      387 2023-04-18 20:28:30.000000 garpixcms-4.1.0/garpixcms/__pycache__/apps.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6796 2023-04-18 20:28:30.000000 garpixcms-4.1.0/garpixcms/__pycache__/settings.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1743 2023-04-18 20:28:31.000000 garpixcms-4.1.0/garpixcms/__pycache__/urls.cpython-38.pyc
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.243991 garpixcms-4.1.0/garpixcms/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       36 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/admin/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.244340 garpixcms-4.1.0/garpixcms/admin/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      205 2023-04-18 20:28:31.000000 garpixcms-4.1.0/garpixcms/admin/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      487 2023-04-18 20:28:31.000000 garpixcms-4.1.0/garpixcms/admin/__pycache__/page.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      173 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/admin/page.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       93 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/apps.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.244564 garpixcms-4.1.0/garpixcms/contexts/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/contexts/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      691 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/contexts/global_context.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.244682 garpixcms-4.1.0/garpixcms/management/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/management/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.244782 garpixcms-4.1.0/garpixcms/management/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      172 2023-05-10 14:01:00.000000 garpixcms-4.1.0/garpixcms/management/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.245004 garpixcms-4.1.0/garpixcms/management/commands/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/management/commands/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      872 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/management/commands/update_user_module.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.245209 garpixcms-4.1.0/garpixcms/middleware/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/middleware/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.245461 garpixcms-4.1.0/garpixcms/middleware/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      172 2023-05-10 14:00:43.000000 garpixcms-4.1.0/garpixcms/middleware/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2037 2023-05-10 14:00:43.000000 garpixcms-4.1.0/garpixcms/middleware/__pycache__/locale.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2196 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/middleware/locale.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.245686 garpixcms-4.1.0/garpixcms/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/models/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.245968 garpixcms-4.1.0/garpixcms/models/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      201 2023-04-18 20:28:31.000000 garpixcms-4.1.0/garpixcms/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      818 2023-04-18 20:28:31.000000 garpixcms-4.1.0/garpixcms/models/__pycache__/page.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      413 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/models/page.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8440 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/settings.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1697 2023-05-12 09:51:39.000000 garpixcms-4.1.0/garpixcms/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.238129 garpixcms-4.1.0/garpixcms/static/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.238829 garpixcms-4.1.0/garpixcms/static/admin/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.251623 garpixcms-4.1.0/garpixcms/static/admin/css/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8440 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/static/admin/css/autocomplete.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    22662 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/static/admin/css/base.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6469 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/static/admin/css/changelists.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      355 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/static/admin/css/dashboard.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      423 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/static/admin/css/fonts.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8370 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/static/admin/css/forms.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1185 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/static/admin/css/login.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2505 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/static/admin/css/nav_sidebar.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    18344 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/static/admin/css/responsive.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1741 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/static/admin/css/responsive_rtl.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3487 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/static/admin/css/rtl.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      502 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/static/admin/css/tabbed_translation_fields.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    10010 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/static/admin/css/widgets.css
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.281125 garpixcms-4.1.0/garpixcms/static/admin/img/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      908 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/static/admin/img/icon-addlink.svg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      825 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/static/admin/img/icon-changelink.svg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      218 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/static/admin/img/icon-custom-checked.svg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      705 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/static/admin/img/icon-deletelink.svg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      930 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/static/admin/img/search.svg
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.281299 garpixcms-4.1.0/garpixcms/static/admin/js/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      291 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/static/admin/js/admin.js
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.239055 garpixcms-4.1.0/garpixcms/templates/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.281803 garpixcms-4.1.0/garpixcms/templates/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4421 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/templates/admin/app_list.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4395 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/templates/admin/base.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      809 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/templates/admin/base_site.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.281936 garpixcms-4.1.0/garpixcms/templates/garpixcms/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      450 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/templates/garpixcms/base.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.282991 garpixcms-4.1.0/garpixcms/templates/garpixcms/include/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      730 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/templates/garpixcms/include/footer.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      642 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/templates/garpixcms/include/header.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      428 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/templates/garpixcms/include/login.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.294430 garpixcms-4.1.0/garpixcms/templates/garpixcms/menus/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      202 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/templates/garpixcms/menus/footer_menu.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      369 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/templates/garpixcms/menus/header_menu.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.294858 garpixcms-4.1.0/garpixcms/templates/garpixcms/pages/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      139 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/templates/garpixcms/pages/default.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      202 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/templates/garpixcms/pages/home.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      346 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/templates/garpixcms/pages/login.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.295118 garpixcms-4.1.0/garpixcms/translation/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       49 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/translation/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.295645 garpixcms-4.1.0/garpixcms/translation/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      224 2023-04-18 20:28:31.000000 garpixcms-4.1.0/garpixcms/translation/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      502 2023-04-18 20:28:31.000000 garpixcms-4.1.0/garpixcms/translation/__pycache__/page.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      189 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/translation/page.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1842 2023-04-18 19:40:20.000000 garpixcms-4.1.0/garpixcms/urls.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 09:55:15.243189 garpixcms-4.1.0/garpixcms.egg-info/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1766 2023-05-12 09:55:15.000000 garpixcms-4.1.0/garpixcms.egg-info/PKG-INFO
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2848 2023-05-12 09:55:15.000000 garpixcms-4.1.0/garpixcms.egg-info/SOURCES.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-12 09:55:15.000000 garpixcms-4.1.0/garpixcms.egg-info/dependency_links.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-12 09:55:15.000000 garpixcms-4.1.0/garpixcms.egg-info/not-zip-safe
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      401 2023-05-12 09:55:15.000000 garpixcms-4.1.0/garpixcms.egg-info/requires.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       10 2023-05-12 09:55:15.000000 garpixcms-4.1.0/garpixcms.egg-info/top_level.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-05-12 09:55:15.296328 garpixcms-4.1.0/setup.cfg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1697 2023-05-12 09:55:15.000000 garpixcms-4.1.0/setup.py
```

### Comparing `garpixcms-4.0.0rc9/PKG-INFO` & `garpixcms-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpixcms
-Version: 4.0.0rc9
+Version: 4.1.0
 Home-page: https://github.com/garpixcms/garpixcms
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpixcms-4.0.0rc9/garpixcms/CHANGELOG.md` & `garpixcms-4.1.0/garpixcms/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,53 @@
-### 4.0.0-rc8-4.0.0-rc9 (24.03.2023)
+### 4.1.0 (12.05.2023)
 
-- Upgrade `garpix_page` to version 2.45.0-rc3.
+- Upgrade `garpix_page` to version 2.46.0
+
+### 4.0.0 (10.05.2023)
+
+- Upgrade `garpix_user` to version 3.5.0
+- Upgrade `garpix_page` to version 2.45.0
+- Upgrade `garpix_notify` to version 5.16.0.
+
+### 4.0.0-rc20 (28.04.2023)
+
+- Upgrade `garpix_page` to version 2.45.0-rc10.
+- Upgrade `garpix_menu` to version 1.16.0.
+
+
+### 4.0.0-rc18-4.0.0-rc19 (25.04.2023)
+
+- Upgrade `garpix_page` to version 2.45.0-rc9.
+- Upgrade `garpix_notify` to version 5.15.1.
+
+### 4.0.0-rc17 (19.04.2023)
+
+- Upgrade `garpix_user` to version 3.5.0-rc8.
+
+### 4.0.0-rc16 (18.04.2023)
+
+- Upgrade `garpix_user` to version 3.5.0-rc7.
+
+### 4.0.0-rc15 (14.04.2023)
+
+- Upgrade `garpix_page` to version 2.45.0-rc8.
+- Upgrade `garpix_notify` to version 5.15.0.
+- Upgrade `garpix_user` to version 3.5.0-rc6.
+
+### 4.0.0-rc14 (06.04.2023)
+
+- Upgrade `eqator` to version 2.7.0.
+
+### 4.0.0-rc13 (30.03.2023)
+
+- Upgrade `garpix_page` to version 2.45.0-rc7.
+
+### 4.0.0-rc8-4.0.0-rc12 (24.03.2023)
+
+- Upgrade `garpix_page` to version 2.45.0-rc6.
 
 ### 4.0.0-rc7 (24.03.2023)
 
 - Upgrade `garpix_page` to version 2.45.0-rc1.
 - Upgrade `garpix_menu` to version 1.15.0.
 - Upgrade `garpix_notify` to version 5.14.0.
```

### Comparing `garpixcms-4.0.0rc9/garpixcms/CONTRIBUTING.md` & `garpixcms-4.1.0/garpixcms/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms/README.rst` & `garpixcms-4.1.0/garpixcms/README.rst`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms/__pycache__/settings.cpython-38.pyc` & `garpixcms-4.1.0/garpixcms/__pycache__/settings.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Mar  9 04:14:34 2023 UTC, .py size: 8440 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 2a5d 0964 f820 0000  U.......*].d. ..
+00000000: 550d 0d0a 0000 0000 24f2 3e64 f820 0000  U.......$.>d. ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0022 0000 0040 0000 0073 6403 0000 6400  ."...@...sd...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6401 6c05 5a05 6400 6404 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 5400 6400 6406 6c09  ..d.d.l.T.d.d.l.
 00000070: 6d0a 5a0a 0100 6502 8300 5a0b 650b 6a0c  m.Z...e...Z.e.j.
```

### Comparing `garpixcms-4.0.0rc9/garpixcms/__pycache__/urls.cpython-38.pyc` & `garpixcms-4.1.0/garpixcms/__pycache__/urls.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Mar  9 03:45:19 2023 UTC, .py size: 1842 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 4f56 0964 3207 0000  U.......OV.d2...
+00000000: 550d 0d0a 0000 0000 24f2 3e64 3207 0000  U.......$.>d2...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 e001 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d08 5a08 0100 6400 6405 6c0a  m.Z.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6400 6406 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `garpixcms-4.0.0rc9/garpixcms/contexts/global_context.py` & `garpixcms-4.1.0/garpixcms/contexts/global_context.py`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms/management/commands/update_user_module.py` & `garpixcms-4.1.0/garpixcms/management/commands/update_user_module.py`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms/middleware/__pycache__/locale.cpython-38.pyc` & `garpixcms-4.1.0/garpixcms/middleware/__pycache__/locale.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Mar  7 14:17:49 2023 UTC, .py size: 2196 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 8d47 0764 9408 0000  U........G.d....
+00000000: 550d 0d0a 0000 0000 24f2 3e64 9408 0000  U.......$.>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 6d08 5a08  d.l.m.Z.m.Z.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6406  ..d.d.l.m.Z...d.
 00000070: 6407 8400 5a0b 6500 6a0c 6401 6408 8d01  d...Z.e.j.d.d...
```

### Comparing `garpixcms-4.0.0rc9/garpixcms/middleware/locale.py` & `garpixcms-4.1.0/garpixcms/middleware/locale.py`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms/models/__pycache__/page.cpython-38.pyc` & `garpixcms-4.1.0/garpixcms/models/__pycache__/page.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Jun 29 08:47:07 2022 UTC, .py size: 413 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 8b11 bc62 9d01 0000  U..........b....
+00000000: 550d 0d0a 0000 0000 24f2 3e64 9d01 0000  U.......$.>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 6503 8303 5a04 6405 5300 2906 e900 0000  e...Z.d.S.).....
 00000060: 0029 01da 1652 6963 6854 6578 7455 706c  .)...RichTextUpl
 00000070: 6f61 6469 6e67 4669 656c 6429 01da 0842  oadingField)...B
@@ -40,13 +40,13 @@
 00000270: 0000 0072 0a00 0000 720b 0000 0072 0200  ...r....r....r..
 00000280: 0000 da07 636f 6e74 656e 74da 0874 656d  ....content..tem
 00000290: 706c 6174 6572 1000 0000 720e 0000 0072  plater....r....r
 000002a0: 0e00 0000 720e 0000 0072 0f00 0000 7204  ....r....r....r.
 000002b0: 0000 0005 0000 0073 0600 0000 0801 0e02  .......s........
 000002c0: 0402 7204 0000 004e 2905 da18 636b 6564  ..r....N)...cked
 000002d0: 6974 6f72 5f75 706c 6f61 6465 722e 6669  itor_uploader.fi
-000002e0: 656c 6473 7202 0000 005a 1267 6172 7069  eldsr....Z.garpi
+000002e0: 656c 6473 7202 0000 00da 1267 6172 7069  eldsr......garpi
 000002f0: 785f 7061 6765 2e6d 6f64 656c 7372 0300  x_page.modelsr..
 00000300: 0000 7204 0000 0072 0e00 0000 720e 0000  ..r....r....r...
 00000310: 0072 0e00 0000 720f 0000 00da 083c 6d6f  .r....r......<mo
 00000320: 6475 6c65 3e01 0000 0073 0400 0000 0c01  dule>....s......
 00000330: 0c03                                     ..
```

### Comparing `garpixcms-4.0.0rc9/garpixcms/settings.py` & `garpixcms-4.1.0/garpixcms/settings.py`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms/setup.py` & `garpixcms-4.1.0/garpixcms/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpixcms')
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpixcms',
-    version='4.0.0-rc9',
+    version='4.1.0',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpixcms',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
@@ -28,20 +28,20 @@
         'Programming Language :: Python :: 3.8',
     ],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'Django >= 3.1, < 4',
         'garpix_utils == 1.8.0',
-        'garpix_page == 2.45.0-rc3',
-        'garpix_menu == 1.15.0',
-        'eqator == 2.6.0',
+        'garpix_page == 2.46.0',
+        'garpix_menu == 1.16.0',
+        'eqator == 2.7.0',
         'garpix_auth == 2.3.0',
-        'garpix_notify == 5.14.0',
-        'garpix_user == 3.5.0-rc5',
+        'garpix_notify == 5.16.0',
+        'garpix_user == 3.5.0',
         'garpix_package == 2.0.1',
         'psycopg2-binary >= 2.8.6',
         'uwsgi >= 2.0.19.1',
         'environs >= 9.3.2',
         'django-ckeditor == 6.3.0',
         'djangorestframework >= 3.12.4',
         'django-cors-headers >= 3.7.0, <= 3.13.0',
```

### Comparing `garpixcms-4.0.0rc9/garpixcms/static/admin/css/autocomplete.css` & `garpixcms-4.1.0/garpixcms/static/admin/css/autocomplete.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms/static/admin/css/base.css` & `garpixcms-4.1.0/garpixcms/static/admin/css/base.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms/static/admin/css/changelists.css` & `garpixcms-4.1.0/garpixcms/static/admin/css/changelists.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms/static/admin/css/forms.css` & `garpixcms-4.1.0/garpixcms/static/admin/css/forms.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms/static/admin/css/login.css` & `garpixcms-4.1.0/garpixcms/static/admin/css/login.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms/static/admin/css/nav_sidebar.css` & `garpixcms-4.1.0/garpixcms/static/admin/css/nav_sidebar.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms/static/admin/css/responsive.css` & `garpixcms-4.1.0/garpixcms/static/admin/css/responsive.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms/static/admin/css/responsive_rtl.css` & `garpixcms-4.1.0/garpixcms/static/admin/css/responsive_rtl.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms/static/admin/css/rtl.css` & `garpixcms-4.1.0/garpixcms/static/admin/css/rtl.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms/static/admin/css/widgets.css` & `garpixcms-4.1.0/garpixcms/static/admin/css/widgets.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms/static/admin/img/icon-addlink.svg` & `garpixcms-4.1.0/garpixcms/static/admin/img/icon-addlink.svg`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms/static/admin/img/icon-changelink.svg` & `garpixcms-4.1.0/garpixcms/static/admin/img/icon-changelink.svg`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms/static/admin/img/icon-deletelink.svg` & `garpixcms-4.1.0/garpixcms/static/admin/img/icon-deletelink.svg`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms/static/admin/img/search.svg` & `garpixcms-4.1.0/garpixcms/static/admin/img/search.svg`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms/templates/admin/app_list.html` & `garpixcms-4.1.0/garpixcms/templates/admin/app_list.html`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms/templates/admin/base.html` & `garpixcms-4.1.0/garpixcms/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms/templates/admin/base_site.html` & `garpixcms-4.1.0/garpixcms/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms/templates/garpixcms/include/footer.html` & `garpixcms-4.1.0/garpixcms/templates/garpixcms/include/footer.html`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms/templates/garpixcms/include/header.html` & `garpixcms-4.1.0/garpixcms/templates/garpixcms/include/header.html`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms/urls.py` & `garpixcms-4.1.0/garpixcms/urls.py`

 * *Files identical despite different names*

### Comparing `garpixcms-4.0.0rc9/garpixcms.egg-info/PKG-INFO` & `garpixcms-4.1.0/garpixcms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpixcms
-Version: 4.0.0rc9
+Version: 4.1.0
 Home-page: https://github.com/garpixcms/garpixcms
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpixcms-4.0.0rc9/garpixcms.egg-info/SOURCES.txt` & `garpixcms-4.1.0/garpixcms.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -21,22 +21,18 @@
 garpixcms/__pycache__/urls.cpython-38.pyc
 garpixcms/admin/__init__.py
 garpixcms/admin/page.py
 garpixcms/admin/__pycache__/__init__.cpython-38.pyc
 garpixcms/admin/__pycache__/page.cpython-38.pyc
 garpixcms/contexts/__init__.py
 garpixcms/contexts/global_context.py
-garpixcms/contexts/__pycache__/__init__.cpython-38.pyc
-garpixcms/contexts/__pycache__/global_context.cpython-38.pyc
 garpixcms/management/__init__.py
 garpixcms/management/__pycache__/__init__.cpython-38.pyc
 garpixcms/management/commands/__init__.py
 garpixcms/management/commands/update_user_module.py
-garpixcms/management/commands/__pycache__/__init__.cpython-38.pyc
-garpixcms/management/commands/__pycache__/update_user_module.cpython-38.pyc
 garpixcms/middleware/__init__.py
 garpixcms/middleware/locale.py
 garpixcms/middleware/__pycache__/__init__.cpython-38.pyc
 garpixcms/middleware/__pycache__/locale.cpython-38.pyc
 garpixcms/models/__init__.py
 garpixcms/models/page.py
 garpixcms/models/__pycache__/__init__.cpython-38.pyc
```

### Comparing `garpixcms-4.0.0rc9/setup.py` & `garpixcms-4.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpixcms')
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpixcms',
-    version='4.0.0-rc9',
+    version='4.1.0',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpixcms',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
@@ -28,20 +28,20 @@
         'Programming Language :: Python :: 3.8',
     ],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'Django >= 3.1, < 4',
         'garpix_utils == 1.8.0',
-        'garpix_page == 2.45.0-rc3',
-        'garpix_menu == 1.15.0',
-        'eqator == 2.6.0',
+        'garpix_page == 2.46.0',
+        'garpix_menu == 1.16.0',
+        'eqator == 2.7.0',
         'garpix_auth == 2.3.0',
-        'garpix_notify == 5.14.0',
-        'garpix_user == 3.5.0-rc5',
+        'garpix_notify == 5.16.0',
+        'garpix_user == 3.5.0',
         'garpix_package == 2.0.1',
         'psycopg2-binary >= 2.8.6',
         'uwsgi >= 2.0.19.1',
         'environs >= 9.3.2',
         'django-ckeditor == 6.3.0',
         'djangorestframework >= 3.12.4',
         'django-cors-headers >= 3.7.0, <= 3.13.0',
```


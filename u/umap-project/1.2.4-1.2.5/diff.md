# Comparing `tmp/umap-project-1.2.4.tar.gz` & `tmp/umap-project-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umap-project-1.2.4.tar", last modified: Thu Mar  2 09:24:04 2023, max compression
+gzip compressed data, was "umap-project-1.2.5.tar", last modified: Fri May 12 15:39:47 2023, max compression
```

## Comparing `umap-project-1.2.4.tar` & `umap-project-1.2.5.tar`

### file list

```diff
@@ -1,519 +1,519 @@
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.149282 umap-project-1.2.4/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      482 2016-04-23 07:38:39.000000 umap-project-1.2.4/LICENSE
--rw-r--r--   0 ybon      (1000) ybon      (1000)      196 2018-07-14 08:06:10.000000 umap-project-1.2.4/MANIFEST.in
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2221 2023-03-02 09:24:04.149282 umap-project-1.2.4/PKG-INFO
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1184 2019-02-22 20:49:23.000000 umap-project-1.2.4/README.md
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1391 2023-03-02 09:24:04.149282 umap-project-1.2.4/setup.cfg
--rw-r--r--   0 ybon      (1000) ybon      (1000)       37 2023-03-02 09:14:15.000000 umap-project-1.2.4/setup.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.042615 umap-project-1.2.4/umap/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      178 2023-03-02 09:14:15.000000 umap-project-1.2.4/umap/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      541 2023-03-02 09:15:56.000000 umap-project-1.2.4/umap/admin.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      109 2023-03-02 09:15:56.000000 umap-project-1.2.4/umap/apps.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      535 2023-02-22 09:51:22.000000 umap-project-1.2.4/umap/autocomplete.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.042615 umap-project-1.2.4/umap/bin/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      256 2016-09-17 20:05:31.000000 umap-project-1.2.4/umap/bin/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      358 2023-03-02 09:14:50.000000 umap-project-1.2.4/umap/context_processors.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2014 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/decorators.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      869 2023-03-02 09:15:56.000000 umap-project-1.2.4/umap/fields.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2740 2023-03-02 09:07:10.000000 umap-project-1.2.4/umap/forms.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.035948 umap-project-1.2.4/umap/locale/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/am_ET/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.042615 umap-project-1.2.4/umap/locale/am_ET/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6618 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/am_ET/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11054 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/am_ET/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/ar/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.042615 umap-project-1.2.4/umap/locale/ar/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4041 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9726 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/ast/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.045948 umap-project-1.2.4/umap/locale/ast/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      432 2020-11-09 08:22:17.000000 umap-project-1.2.4/umap/locale/ast/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8007 2020-03-09 07:59:50.000000 umap-project-1.2.4/umap/locale/ast/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/bg/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.045948 umap-project-1.2.4/umap/locale/bg/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7196 2023-03-02 09:13:29.000000 umap-project-1.2.4/umap/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11594 2023-03-02 09:13:29.000000 umap-project-1.2.4/umap/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/ca/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.045948 umap-project-1.2.4/umap/locale/ca/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7221 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10687 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/cs_CZ/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.045948 umap-project-1.2.4/umap/locale/cs_CZ/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7365 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/cs_CZ/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11029 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/cs_CZ/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/da/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.045948 umap-project-1.2.4/umap/locale/da/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7029 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/da/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10623 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/de/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.045948 umap-project-1.2.4/umap/locale/de/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7362 2023-03-02 09:13:29.000000 umap-project-1.2.4/umap/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11077 2023-03-02 09:13:29.000000 umap-project-1.2.4/umap/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/el/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.045948 umap-project-1.2.4/umap/locale/el/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10089 2023-03-02 09:22:58.000000 umap-project-1.2.4/umap/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    13756 2023-03-02 09:13:29.000000 umap-project-1.2.4/umap/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/en/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.045948 umap-project-1.2.4/umap/locale/en/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      337 2023-03-02 09:22:58.000000 umap-project-1.2.4/umap/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7939 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/es/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.045948 umap-project-1.2.4/umap/locale/es/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7282 2023-03-02 09:22:58.000000 umap-project-1.2.4/umap/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11052 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/et/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.045948 umap-project-1.2.4/umap/locale/et/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6166 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/et/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9991 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/et/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/fi/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.045948 umap-project-1.2.4/umap/locale/fi/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5815 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10409 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/fr/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.049282 umap-project-1.2.4/umap/locale/fr/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7331 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11117 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/gl/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.049282 umap-project-1.2.4/umap/locale/gl/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7205 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/gl/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10758 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/gl/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/he/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.049282 umap-project-1.2.4/umap/locale/he/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8051 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11524 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/hr/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.049282 umap-project-1.2.4/umap/locale/hr/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1845 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/hr/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8507 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/hu/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.049282 umap-project-1.2.4/umap/locale/hu/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7605 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11128 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/hu/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/id/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.049282 umap-project-1.2.4/umap/locale/id/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      425 2020-11-09 08:22:16.000000 umap-project-1.2.4/umap/locale/id/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8000 2020-03-09 07:59:50.000000 umap-project-1.2.4/umap/locale/id/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/is/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.049282 umap-project-1.2.4/umap/locale/is/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7647 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/is/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11116 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/is/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/it/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.049282 umap-project-1.2.4/umap/locale/it/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7314 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11155 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/ja/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.049282 umap-project-1.2.4/umap/locale/ja/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7724 2023-03-02 09:13:54.000000 umap-project-1.2.4/umap/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11254 2023-03-02 09:13:54.000000 umap-project-1.2.4/umap/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/ko/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.049282 umap-project-1.2.4/umap/locale/ko/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7670 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11139 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/lt/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.052615 umap-project-1.2.4/umap/locale/lt/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6879 2023-03-02 09:22:58.000000 umap-project-1.2.4/umap/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10671 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/nl/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.052615 umap-project-1.2.4/umap/locale/nl/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5942 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10002 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/no/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.052615 umap-project-1.2.4/umap/locale/no/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      423 2020-11-09 08:22:17.000000 umap-project-1.2.4/umap/locale/no/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7998 2020-03-09 16:17:49.000000 umap-project-1.2.4/umap/locale/no/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.032615 umap-project-1.2.4/umap/locale/pl/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.052615 umap-project-1.2.4/umap/locale/pl/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7336 2023-03-02 09:13:29.000000 umap-project-1.2.4/umap/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11013 2023-03-02 09:13:29.000000 umap-project-1.2.4/umap/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.035948 umap-project-1.2.4/umap/locale/pt/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.052615 umap-project-1.2.4/umap/locale/pt/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7240 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10774 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.035948 umap-project-1.2.4/umap/locale/pt_BR/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.052615 umap-project-1.2.4/umap/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6945 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10651 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.035948 umap-project-1.2.4/umap/locale/pt_PT/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.052615 umap-project-1.2.4/umap/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7255 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/pt_PT/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10789 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/pt_PT/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.035948 umap-project-1.2.4/umap/locale/ro/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.052615 umap-project-1.2.4/umap/locale/ro/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1482 2020-11-09 08:22:17.000000 umap-project-1.2.4/umap/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8428 2020-03-09 07:59:50.000000 umap-project-1.2.4/umap/locale/ro/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.035948 umap-project-1.2.4/umap/locale/ru/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.052615 umap-project-1.2.4/umap/locale/ru/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9291 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12951 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.035948 umap-project-1.2.4/umap/locale/si_LK/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.055948 umap-project-1.2.4/umap/locale/si_LK/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      447 2020-11-09 08:22:17.000000 umap-project-1.2.4/umap/locale/si_LK/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8022 2020-03-09 07:59:50.000000 umap-project-1.2.4/umap/locale/si_LK/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.035948 umap-project-1.2.4/umap/locale/sk_SK/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.055948 umap-project-1.2.4/umap/locale/sk_SK/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6929 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/sk_SK/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10746 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/sk_SK/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.035948 umap-project-1.2.4/umap/locale/sl/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.055948 umap-project-1.2.4/umap/locale/sl/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6853 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/sl/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10536 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.035948 umap-project-1.2.4/umap/locale/sr/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.055948 umap-project-1.2.4/umap/locale/sr/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8900 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/sr/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12384 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/sr/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.035948 umap-project-1.2.4/umap/locale/sv/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.055948 umap-project-1.2.4/umap/locale/sv/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7024 2023-03-02 09:13:29.000000 umap-project-1.2.4/umap/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10519 2023-03-02 09:13:29.000000 umap-project-1.2.4/umap/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.035948 umap-project-1.2.4/umap/locale/th_TH/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.055948 umap-project-1.2.4/umap/locale/th_TH/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      436 2020-11-09 08:22:17.000000 umap-project-1.2.4/umap/locale/th_TH/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8011 2020-03-09 07:59:50.000000 umap-project-1.2.4/umap/locale/th_TH/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.035948 umap-project-1.2.4/umap/locale/tr/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.055948 umap-project-1.2.4/umap/locale/tr/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7424 2023-03-02 09:13:29.000000 umap-project-1.2.4/umap/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10963 2023-03-02 09:13:29.000000 umap-project-1.2.4/umap/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.035948 umap-project-1.2.4/umap/locale/uk_UA/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.055948 umap-project-1.2.4/umap/locale/uk_UA/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9499 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/uk_UA/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    13002 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/uk_UA/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.035948 umap-project-1.2.4/umap/locale/vi/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.059282 umap-project-1.2.4/umap/locale/vi/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6096 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/vi/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10554 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/vi/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.035948 umap-project-1.2.4/umap/locale/zh/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.059282 umap-project-1.2.4/umap/locale/zh/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4419 2020-11-09 08:22:17.000000 umap-project-1.2.4/umap/locale/zh/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9338 2020-03-09 07:59:50.000000 umap-project-1.2.4/umap/locale/zh/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.035948 umap-project-1.2.4/umap/locale/zh_TW/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.059282 umap-project-1.2.4/umap/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6850 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10572 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/locale/zh_TW/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.059282 umap-project-1.2.4/umap/management/
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-09-17 20:05:31.000000 umap-project-1.2.4/umap/management/__init__.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.059282 umap-project-1.2.4/umap/management/commands/
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-09-17 20:05:31.000000 umap-project-1.2.4/umap/management/commands/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      839 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/management/commands/anonymous_edit_url.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1298 2019-04-07 14:33:20.000000 umap-project-1.2.4/umap/management/commands/generate_js_locale.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1902 2019-04-07 14:28:38.000000 umap-project-1.2.4/umap/management/commands/import_pictograms.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      207 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/managers.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      515 2023-03-02 09:07:10.000000 umap-project-1.2.4/umap/middleware.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.062615 umap-project-1.2.4/umap/migrations/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5563 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/migrations/0001_initial.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      373 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/migrations/0002_tilelayer_tms.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      812 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/migrations/0003_add_tilelayer.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      530 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/migrations/0004_add_licence.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      318 2018-07-14 11:58:47.000000 umap-project-1.2.4/umap/migrations/0005_remove_map_tilelayer.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      497 2019-04-07 08:09:35.000000 umap-project-1.2.4/umap/migrations/0006_auto_20190407_0719.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      515 2019-04-16 17:57:23.000000 umap-project-1.2.4/umap/migrations/0007_auto_20190416_1757.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      459 2023-03-02 09:17:01.000000 umap-project-1.2.4/umap/migrations/0008_alter_map_settings.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-11-26 16:02:45.000000 umap-project-1.2.4/umap/migrations/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11200 2023-03-02 09:08:49.000000 umap-project-1.2.4/umap/models.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.062615 umap-project-1.2.4/umap/settings/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1617 2023-03-02 09:07:10.000000 umap-project-1.2.4/umap/settings/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7833 2023-03-02 09:15:56.000000 umap-project-1.2.4/umap/settings/base.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      386 2018-05-19 15:10:46.000000 umap-project-1.2.4/umap/settings/dev.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.062615 umap-project-1.2.4/umap/static/
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-04-23 07:38:39.000000 umap-project-1.2.4/umap/static/.gitignore
--rw-r--r--   0 ybon      (1000) ybon      (1000)      638 2016-04-23 07:38:39.000000 umap-project-1.2.4/umap/static/favicon.ico
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.065948 umap-project-1.2.4/umap/static/umap/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    17943 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/base.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9125 2016-04-23 07:38:39.000000 umap-project-1.2.4/umap/static/umap/bitbucket.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5851 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/static/umap/content.css
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.069282 umap-project-1.2.4/umap/static/umap/font/
--rwxr-xr-x   0 ybon      (1000) ybon      (1000)   182984 2018-05-17 09:59:39.000000 umap-project-1.2.4/umap/static/umap/font/FiraSans-Light.woff
--rwxr-xr-x   0 ybon      (1000) ybon      (1000)   129180 2018-05-17 09:59:39.000000 umap-project-1.2.4/umap/static/umap/font/FiraSans-Light.woff2
--rwxr-xr-x   0 ybon      (1000) ybon      (1000)   191400 2018-05-17 09:59:39.000000 umap-project-1.2.4/umap/static/umap/font/FiraSans-LightItalic.woff
--rwxr-xr-x   0 ybon      (1000) ybon      (1000)   135744 2018-05-17 09:59:39.000000 umap-project-1.2.4/umap/static/umap/font/FiraSans-LightItalic.woff2
--rwxr-xr-x   0 ybon      (1000) ybon      (1000)   198128 2018-05-17 09:59:39.000000 umap-project-1.2.4/umap/static/umap/font/FiraSans-SemiBold.woff
--rwxr-xr-x   0 ybon      (1000) ybon      (1000)   140168 2018-05-17 09:59:39.000000 umap-project-1.2.4/umap/static/umap/font/FiraSans-SemiBold.woff2
--rw-r--r--   0 ybon      (1000) ybon      (1000)      832 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/static/umap/font.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1564 2016-04-23 07:38:39.000000 umap-project-1.2.4/umap/static/umap/github.png
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.079282 umap-project-1.2.4/umap/static/umap/img/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    13636 2020-03-28 10:15:31.000000 umap-project-1.2.4/umap/static/umap/img/16-white.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)    57263 2020-03-28 10:15:31.000000 umap-project-1.2.4/umap/static/umap/img/16-white.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11308 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/static/umap/img/16.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)    38140 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/static/umap/img/16.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)    19000 2019-04-09 07:59:04.000000 umap-project-1.2.4/umap/static/umap/img/24-white.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)    38375 2019-04-09 07:59:04.000000 umap-project-1.2.4/umap/static/umap/img/24-white.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)    15600 2020-03-22 13:36:34.000000 umap-project-1.2.4/umap/static/umap/img/24.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)    35215 2020-03-22 13:36:34.000000 umap-project-1.2.4/umap/static/umap/img/24.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)      430 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/static/umap/img/edit-16.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3491 2016-04-23 07:38:39.000000 umap-project-1.2.4/umap/static/umap/img/edit.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)      190 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/static/umap/img/icon-bg.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3338 2016-04-23 07:38:39.000000 umap-project-1.2.4/umap/static/umap/img/logo.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5537 2016-04-23 07:38:39.000000 umap-project-1.2.4/umap/static/umap/img/logo_filigree.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      375 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/static/umap/img/marker.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3679 2016-04-23 07:38:39.000000 umap-project-1.2.4/umap/static/umap/img/opensource.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8351 2016-04-23 07:38:39.000000 umap-project-1.2.4/umap/static/umap/img/osm.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1472 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/static/umap/img/search.gif
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.082615 umap-project-1.2.4/umap/static/umap/js/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9173 2019-01-30 10:00:11.000000 umap-project-1.2.4/umap/static/umap/js/umap.autocomplete.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    36638 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/js/umap.controls.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    20447 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/js/umap.core.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    35418 2023-02-28 14:58:59.000000 umap-project-1.2.4/umap/static/umap/js/umap.features.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    27098 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/js/umap.forms.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6376 2019-01-30 10:04:17.000000 umap-project-1.2.4/umap/static/umap/js/umap.icon.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    68064 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/js/umap.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    36832 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/js/umap.layer.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5905 2023-02-28 14:58:59.000000 umap-project-1.2.4/umap/static/umap/js/umap.permissions.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7420 2023-02-28 14:58:59.000000 umap-project-1.2.4/umap/static/umap/js/umap.popup.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5192 2020-03-28 10:15:31.000000 umap-project-1.2.4/umap/static/umap/js/umap.slideshow.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4527 2020-03-28 10:15:31.000000 umap-project-1.2.4/umap/static/umap/js/umap.tableeditor.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7351 2019-01-30 09:54:21.000000 umap-project-1.2.4/umap/static/umap/js/umap.ui.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10308 2020-03-28 10:15:31.000000 umap-project-1.2.4/umap/static/umap/js/umap.xhr.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.102615 umap-project-1.2.4/umap/static/umap/locale/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    26175 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/am_ET.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    26104 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/am_ET.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21793 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/ar.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21728 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/ar.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21441 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/ast.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21374 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/ast.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    25216 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/bg.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    25151 2023-03-02 09:13:29.000000 umap-project-1.2.4/umap/static/umap/locale/bg.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22330 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/ca.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22265 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/ca.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23183 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/cs_CZ.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23112 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/cs_CZ.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21882 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/da.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21817 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/da.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23385 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/de.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23320 2023-03-02 09:13:43.000000 umap-project-1.2.4/umap/static/umap/locale/de.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    32772 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/el.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    32707 2023-03-02 09:13:29.000000 umap-project-1.2.4/umap/static/umap/locale/el.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21439 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/en.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21374 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/en.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21074 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/en_US.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23662 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/es.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23597 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/es.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21722 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/et.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21657 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/et.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21385 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/fa_IR.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22517 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/fi.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22452 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/fi.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23449 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/fr.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23384 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/fr.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23153 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/gl.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23088 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/gl.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    25737 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/he.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    25672 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/he.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21649 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/hr.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21584 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/hr.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24563 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/hu.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24498 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/hu.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21439 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/id.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21374 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/id.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23074 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/is.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23009 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/is.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23148 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/it.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23083 2023-03-02 09:13:54.000000 umap-project-1.2.4/umap/static/umap/locale/it.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24685 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/ja.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24620 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/ja.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21661 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/ko.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21596 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/ko.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22412 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/lt.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22347 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/lt.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22430 2023-03-02 09:13:54.000000 umap-project-1.2.4/umap/static/umap/locale/ms.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23099 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/nl.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23034 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/nl.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21717 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/no.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21652 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/no.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22981 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/pl.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22916 2023-03-02 09:13:29.000000 umap-project-1.2.4/umap/static/umap/locale/pl.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21032 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/pl_PL.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22790 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/pt.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23065 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/pt.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23120 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/pt_BR.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23049 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/pt_BR.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23129 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/pt_PT.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23058 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/pt_PT.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21500 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/ro.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21435 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/ro.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    30478 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/ru.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    30413 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/ru.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21445 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/si_LK.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21374 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/si_LK.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22965 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/sk_SK.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22894 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/sk_SK.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22816 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/sl.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22751 2023-03-02 09:13:29.000000 umap-project-1.2.4/umap/static/umap/locale/sl.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24039 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/sr.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23974 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/sr.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22736 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/sv.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22671 2023-03-02 09:13:29.000000 umap-project-1.2.4/umap/static/umap/locale/sv.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21445 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/th_TH.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21374 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/th_TH.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23321 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/tr.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23256 2023-03-02 09:13:29.000000 umap-project-1.2.4/umap/static/umap/locale/tr.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    29961 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/uk_UA.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    29890 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/uk_UA.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21818 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/vi.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21753 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/vi.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21374 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/vi_VN.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21067 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/zh.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21002 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/zh.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21374 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/zh_CN.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21374 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/zh_TW.Big5.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21076 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap/static/umap/locale/zh_TW.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21005 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/locale/zh_TW.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    31281 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/map.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1492 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/static/umap/nav.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)    19408 2016-04-23 07:38:39.000000 umap-project-1.2.4/umap/static/umap/openstreetmap.png
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.105949 umap-project-1.2.4/umap/static/umap/test/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      464 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/static/umap/test/.eslintrc
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1827 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/static/umap/test/Controls.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12735 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/static/umap/test/DataLayer.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10204 2020-03-21 16:11:17.000000 umap-project-1.2.4/umap/static/umap/test/Feature.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    18216 2018-09-22 05:31:42.000000 umap-project-1.2.4/umap/static/umap/test/Map.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3472 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/static/umap/test/Marker.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2612 2018-09-22 08:09:19.000000 umap-project-1.2.4/umap/static/umap/test/Permissions.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    13314 2018-09-05 19:34:30.000000 umap-project-1.2.4/umap/static/umap/test/Polygon.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    14952 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/static/umap/test/Polyline.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3626 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/static/umap/test/TableEditor.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11986 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/test/Util.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10851 2018-09-05 19:34:50.000000 umap-project-1.2.4/umap/static/umap/test/_pre.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5695 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/static/umap/test/index.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)       49 2018-06-02 13:09:22.000000 umap-project-1.2.4/umap/static/umap/theme.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3225 2016-04-23 07:38:39.000000 umap-project-1.2.4/umap/static/umap/twitter.png
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.039282 umap-project-1.2.4/umap/static/umap/vendors/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.105949 umap-project-1.2.4/umap/static/umap/vendors/contextmenu/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1231 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)    16343 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)      990 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8994 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.105949 umap-project-1.2.4/umap/static/umap/vendors/csv2geojson/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    15029 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/csv2geojson/csv2geojson.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6994 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/csv2geojson/index.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.105949 umap-project-1.2.4/umap/static/umap/vendors/editable/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    74768 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/editable/Leaflet.Editable.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3898 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/editable/Path.Drag.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.109282 umap-project-1.2.4/umap/static/umap/vendors/editinosm/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1263 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9141 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.109282 umap-project-1.2.4/umap/static/umap/vendors/formbuilder/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12235 2023-02-28 13:04:38.000000 umap-project-1.2.4/umap/static/umap/vendors/formbuilder/Leaflet.FormBuilder.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.109282 umap-project-1.2.4/umap/static/umap/vendors/fullscreen/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5041 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3654 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.min.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)      299 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/fullscreen/fullscreen.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      420 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/fullscreen/fullscreen@2x.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      994 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/fullscreen/leaflet.fullscreen.css
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.109282 umap-project-1.2.4/umap/static/umap/vendors/georsstogeojson/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3202 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/georsstogeojson/GeoRSSToGeoJSON.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.109282 umap-project-1.2.4/umap/static/umap/vendors/hash/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3462 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/hash/leaflet-hash.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.109282 umap-project-1.2.4/umap/static/umap/vendors/heat/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5158 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/heat/leaflet-heat.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.109282 umap-project-1.2.4/umap/static/umap/vendors/i18n/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1305 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/i18n/Leaflet.i18n.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.122615 umap-project-1.2.4/umap/static/umap/vendors/leaflet/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.125949 umap-project-1.2.4/umap/static/umap/vendors/leaflet/images/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1259 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/leaflet/images/layers-2x.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      696 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/leaflet/images/layers.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2464 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/leaflet/images/marker-icon-2x.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1466 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/leaflet/images/marker-icon.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      618 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/leaflet/images/marker-shadow.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)   398517 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/leaflet/leaflet-src.esm.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)   759894 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/leaflet/leaflet-src.esm.js.map
--rw-r--r--   0 ybon      (1000) ybon      (1000)   400242 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/leaflet/leaflet-src.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)   759986 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/leaflet/leaflet-src.js.map
--rw-r--r--   0 ybon      (1000) ybon      (1000)    14106 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/leaflet/leaflet.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)   140468 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/leaflet/leaflet.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)   191112 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/leaflet/leaflet.js.map
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.129282 umap-project-1.2.4/umap/static/umap/vendors/loading/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3252 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/loading/Control.Loading.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)    14143 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/loading/Control.Loading.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.129282 umap-project-1.2.4/umap/static/umap/vendors/locatecontrol/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2471 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/locatecontrol/L.Control.Locate.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)    30907 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/locatecontrol/L.Control.Locate.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.132615 umap-project-1.2.4/umap/static/umap/vendors/markercluster/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1346 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/markercluster/MarkerCluster.Default.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)      886 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/markercluster/MarkerCluster.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)      318 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/markercluster/WhereAreTheJavascriptFiles.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)    80271 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)   157229 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js.map
--rw-r--r--   0 ybon      (1000) ybon      (1000)    33679 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/markercluster/leaflet.markercluster.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    27566 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/markercluster/leaflet.markercluster.js.map
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.132615 umap-project-1.2.4/umap/static/umap/vendors/measurable/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      937 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/measurable/Leaflet.Measurable.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7190 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/measurable/Leaflet.Measurable.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.135949 umap-project-1.2.4/umap/static/umap/vendors/minimap/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1998 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/minimap/Control.MiniMap.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12129 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/minimap/Control.MiniMap.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.135949 umap-project-1.2.4/umap/static/umap/vendors/minimap/images/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      219 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/minimap/images/toggle.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8057 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/minimap/images/toggle.svg
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.135949 umap-project-1.2.4/umap/static/umap/vendors/osmtogeojson/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    35642 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/osmtogeojson/osmtogeojson.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.135949 umap-project-1.2.4/umap/static/umap/vendors/photon/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    14433 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/photon/leaflet.photon.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.135949 umap-project-1.2.4/umap/static/umap/vendors/print/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    44559 2021-09-12 08:45:21.000000 umap-project-1.2.4/umap/static/umap/vendors/print/leaflet.browser.print.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23442 2021-09-12 08:45:21.000000 umap-project-1.2.4/umap/static/umap/vendors/print/leaflet.browser.print.min.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.135949 umap-project-1.2.4/umap/static/umap/vendors/togeojson/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    18098 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/togeojson/togeojson.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.135949 umap-project-1.2.4/umap/static/umap/vendors/togpx/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    17936 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/togpx/togpx.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.135949 umap-project-1.2.4/umap/static/umap/vendors/tokml/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11521 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/tokml/tokml.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.139282 umap-project-1.2.4/umap/static/umap/vendors/toolbar/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2890 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9060 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2244 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/toolbar/leaflet.toolbar.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5326 2022-11-24 20:22:27.000000 umap-project-1.2.4/umap/static/umap/vendors/toolbar/leaflet.toolbar.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.139282 umap-project-1.2.4/umap/templates/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      305 2016-04-23 07:38:39.000000 umap-project-1.2.4/umap/templates/404.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4904 2016-04-23 07:38:39.000000 umap-project-1.2.4/umap/templates/500.html
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.139282 umap-project-1.2.4/umap/templates/auth/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      467 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/templates/auth/user_detail.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      702 2020-03-28 10:15:31.000000 umap-project-1.2.4/umap/templates/base.html
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.139282 umap-project-1.2.4/umap/templates/registration/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1157 2023-03-01 18:10:17.000000 umap-project-1.2.4/umap/templates/registration/login.html
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.142615 umap-project-1.2.4/umap/templates/umap/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      128 2018-05-18 20:43:08.000000 umap-project-1.2.4/umap/templates/umap/about.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1844 2019-04-07 14:28:38.000000 umap-project-1.2.4/umap/templates/umap/about_summary.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2054 2019-02-09 11:02:16.000000 umap-project-1.2.4/umap/templates/umap/content.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      634 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/templates/umap/content_footer.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1212 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/templates/umap/css.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2018-05-18 20:43:08.000000 umap-project-1.2.4/umap/templates/umap/footer.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1117 2022-09-30 16:19:34.000000 umap-project-1.2.4/umap/templates/umap/home.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2987 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/templates/umap/js.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      112 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/templates/umap/locale.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)      423 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/templates/umap/login_popup_end.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      595 2021-09-12 08:45:40.000000 umap-project-1.2.4/umap/templates/umap/map_detail.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      200 2019-04-09 09:18:15.000000 umap-project-1.2.4/umap/templates/umap/map_fragment.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      165 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/templates/umap/map_init.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      597 2019-04-09 09:37:22.000000 umap-project-1.2.4/umap/templates/umap/map_list.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      299 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/templates/umap/map_messages.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      985 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/templates/umap/navigation.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      878 2018-05-18 20:43:08.000000 umap-project-1.2.4/umap/templates/umap/password_change.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      258 2018-05-18 20:43:08.000000 umap-project-1.2.4/umap/templates/umap/password_change_done.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      390 2019-04-09 09:39:35.000000 umap-project-1.2.4/umap/templates/umap/search.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      448 2018-05-18 20:43:08.000000 umap-project-1.2.4/umap/templates/umap/search_bar.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)        2 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/templates/umap/success.html
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.145949 umap-project-1.2.4/umap/templatetags/
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-04-23 07:38:39.000000 umap-project-1.2.4/umap/templatetags/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2405 2019-04-09 09:38:42.000000 umap-project-1.2.4/umap/templatetags/umap_tags.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.145949 umap-project-1.2.4/umap/tests/
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/tests/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2945 2023-03-02 09:07:10.000000 umap-project-1.2.4/umap/tests/base.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1285 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/tests/conftest.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      360 2023-03-02 09:09:54.000000 umap-project-1.2.4/umap/tests/settings.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2870 2023-02-27 10:29:01.000000 umap-project-1.2.4/umap/tests/test_datalayer.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7616 2023-03-02 09:06:37.000000 umap-project-1.2.4/umap/tests/test_datalayer_views.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      339 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/tests/test_licence.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3149 2018-07-14 13:10:40.000000 umap-project-1.2.4/umap/tests/test_map.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)    18857 2019-04-09 07:59:04.000000 umap-project-1.2.4/umap/tests/test_map_views.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      605 2018-07-14 08:06:10.000000 umap-project-1.2.4/umap/tests/test_tilelayer.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3974 2018-08-04 16:35:43.000000 umap-project-1.2.4/umap/tests/test_views.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4899 2023-03-02 09:16:07.000000 umap-project-1.2.4/umap/urls.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4287 2023-03-02 09:07:10.000000 umap-project-1.2.4/umap/utils.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)    27490 2023-03-02 09:16:45.000000 umap-project-1.2.4/umap/views.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1152 2018-05-19 15:10:36.000000 umap-project-1.2.4/umap/wsgi.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-03-02 09:24:04.149282 umap-project-1.2.4/umap_project.egg-info/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2221 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap_project.egg-info/PKG-INFO
--rw-r--r--   0 ybon      (1000) ybon      (1000)    13960 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap_project.egg-info/SOURCES.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)        1 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap_project.egg-info/dependency_links.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)       40 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap_project.egg-info/entry_points.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)      265 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap_project.egg-info/requires.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)        5 2023-03-02 09:24:03.000000 umap-project-1.2.4/umap_project.egg-info/top_level.txt
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:47.036565 umap-project-1.2.5/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      482 2016-04-23 07:38:39.000000 umap-project-1.2.5/LICENSE
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      196 2018-07-14 08:06:10.000000 umap-project-1.2.5/MANIFEST.in
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2165 2023-05-12 15:39:47.036565 umap-project-1.2.5/PKG-INFO
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1184 2019-02-22 20:49:23.000000 umap-project-1.2.5/README.md
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1391 2023-05-12 15:39:47.036565 umap-project-1.2.5/setup.cfg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)       37 2023-05-05 17:42:43.000000 umap-project-1.2.5/setup.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.653244 umap-project-1.2.5/umap/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      178 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/__init__.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      541 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/admin.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      109 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/apps.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      535 2023-02-22 09:51:22.000000 umap-project-1.2.5/umap/autocomplete.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.653244 umap-project-1.2.5/umap/bin/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      256 2016-09-17 20:05:31.000000 umap-project-1.2.5/umap/bin/__init__.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      358 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/context_processors.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2021 2023-05-12 15:17:55.000000 umap-project-1.2.5/umap/decorators.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      869 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/fields.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2740 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/forms.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.636577 umap-project-1.2.5/umap/locale/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.623245 umap-project-1.2.5/umap/locale/am_ET/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.653244 umap-project-1.2.5/umap/locale/am_ET/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6618 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/am_ET/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11054 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/am_ET/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.623245 umap-project-1.2.5/umap/locale/ar/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.656577 umap-project-1.2.5/umap/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     4041 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9726 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.623245 umap-project-1.2.5/umap/locale/ast/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.656577 umap-project-1.2.5/umap/locale/ast/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      432 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/locale/ast/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8007 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/locale/ast/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.623245 umap-project-1.2.5/umap/locale/bg/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.656577 umap-project-1.2.5/umap/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7196 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11594 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.623245 umap-project-1.2.5/umap/locale/ca/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.656577 umap-project-1.2.5/umap/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7221 2023-05-12 15:39:44.000000 umap-project-1.2.5/umap/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10687 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.626578 umap-project-1.2.5/umap/locale/cs_CZ/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.659910 umap-project-1.2.5/umap/locale/cs_CZ/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7365 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/cs_CZ/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11029 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/cs_CZ/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.626578 umap-project-1.2.5/umap/locale/da/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.659910 umap-project-1.2.5/umap/locale/da/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7029 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/da/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10623 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.626578 umap-project-1.2.5/umap/locale/de/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.659910 umap-project-1.2.5/umap/locale/de/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7362 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11077 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.626578 umap-project-1.2.5/umap/locale/el/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.659910 umap-project-1.2.5/umap/locale/el/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10089 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    13756 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.629911 umap-project-1.2.5/umap/locale/en/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.659910 umap-project-1.2.5/umap/locale/en/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      337 2023-05-12 15:39:44.000000 umap-project-1.2.5/umap/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7939 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.629911 umap-project-1.2.5/umap/locale/es/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.663243 umap-project-1.2.5/umap/locale/es/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7282 2023-05-12 15:39:44.000000 umap-project-1.2.5/umap/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11052 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.629911 umap-project-1.2.5/umap/locale/et/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.663243 umap-project-1.2.5/umap/locale/et/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6166 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/et/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9991 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/et/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.629911 umap-project-1.2.5/umap/locale/fi/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.663243 umap-project-1.2.5/umap/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5815 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10409 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.629911 umap-project-1.2.5/umap/locale/fr/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.663243 umap-project-1.2.5/umap/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7331 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11117 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.629911 umap-project-1.2.5/umap/locale/gl/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.663243 umap-project-1.2.5/umap/locale/gl/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7205 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/gl/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10758 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/gl/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.629911 umap-project-1.2.5/umap/locale/he/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.663243 umap-project-1.2.5/umap/locale/he/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8051 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11524 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.629911 umap-project-1.2.5/umap/locale/hr/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.663243 umap-project-1.2.5/umap/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1845 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/hr/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8507 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.629911 umap-project-1.2.5/umap/locale/hu/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.666576 umap-project-1.2.5/umap/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7605 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11128 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/hu/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.629911 umap-project-1.2.5/umap/locale/id/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.666576 umap-project-1.2.5/umap/locale/id/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      425 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8000 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.629911 umap-project-1.2.5/umap/locale/is/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.666576 umap-project-1.2.5/umap/locale/is/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7647 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/is/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11116 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/is/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.629911 umap-project-1.2.5/umap/locale/it/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.666576 umap-project-1.2.5/umap/locale/it/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7314 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11155 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.629911 umap-project-1.2.5/umap/locale/ja/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.666576 umap-project-1.2.5/umap/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7724 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11254 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.629911 umap-project-1.2.5/umap/locale/ko/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.666576 umap-project-1.2.5/umap/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7670 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11139 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.629911 umap-project-1.2.5/umap/locale/lt/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.666576 umap-project-1.2.5/umap/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6879 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10671 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.629911 umap-project-1.2.5/umap/locale/nl/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.669910 umap-project-1.2.5/umap/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5942 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10002 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.633244 umap-project-1.2.5/umap/locale/no/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.669910 umap-project-1.2.5/umap/locale/no/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      423 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/locale/no/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7998 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/locale/no/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.633244 umap-project-1.2.5/umap/locale/pl/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.669910 umap-project-1.2.5/umap/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7336 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11013 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.633244 umap-project-1.2.5/umap/locale/pt/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.669910 umap-project-1.2.5/umap/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7240 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10774 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.633244 umap-project-1.2.5/umap/locale/pt_BR/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.673243 umap-project-1.2.5/umap/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6945 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10651 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.633244 umap-project-1.2.5/umap/locale/pt_PT/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.673243 umap-project-1.2.5/umap/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7255 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10789 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/pt_PT/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.633244 umap-project-1.2.5/umap/locale/ro/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.673243 umap-project-1.2.5/umap/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1482 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8428 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/locale/ro/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.633244 umap-project-1.2.5/umap/locale/ru/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.673243 umap-project-1.2.5/umap/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9291 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    12951 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.633244 umap-project-1.2.5/umap/locale/si_LK/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.676576 umap-project-1.2.5/umap/locale/si_LK/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      447 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/locale/si_LK/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8022 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/locale/si_LK/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.633244 umap-project-1.2.5/umap/locale/sk_SK/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.679909 umap-project-1.2.5/umap/locale/sk_SK/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6929 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/sk_SK/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10746 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/sk_SK/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.633244 umap-project-1.2.5/umap/locale/sl/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.683243 umap-project-1.2.5/umap/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6853 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/sl/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10536 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.633244 umap-project-1.2.5/umap/locale/sr/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.683243 umap-project-1.2.5/umap/locale/sr/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8900 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/sr/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    12384 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/sr/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.633244 umap-project-1.2.5/umap/locale/sv/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.689909 umap-project-1.2.5/umap/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7024 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10519 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.633244 umap-project-1.2.5/umap/locale/th_TH/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.696575 umap-project-1.2.5/umap/locale/th_TH/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      436 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/th_TH/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8011 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/th_TH/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.633244 umap-project-1.2.5/umap/locale/tr/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.696575 umap-project-1.2.5/umap/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7424 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10963 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.633244 umap-project-1.2.5/umap/locale/uk_UA/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.699909 umap-project-1.2.5/umap/locale/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9499 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/uk_UA/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    13002 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/uk_UA/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.633244 umap-project-1.2.5/umap/locale/vi/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.699909 umap-project-1.2.5/umap/locale/vi/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6096 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/vi/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10554 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/vi/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.633244 umap-project-1.2.5/umap/locale/zh/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.699909 umap-project-1.2.5/umap/locale/zh/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     4419 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/locale/zh/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9338 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/locale/zh/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.636577 umap-project-1.2.5/umap/locale/zh_TW/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.699909 umap-project-1.2.5/umap/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6850 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10572 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/locale/zh_TW/LC_MESSAGES/django.po
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.699909 umap-project-1.2.5/umap/management/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-09-17 20:05:31.000000 umap-project-1.2.5/umap/management/__init__.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.703242 umap-project-1.2.5/umap/management/commands/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-09-17 20:05:31.000000 umap-project-1.2.5/umap/management/commands/__init__.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      839 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/management/commands/anonymous_edit_url.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1298 2019-04-07 14:33:20.000000 umap-project-1.2.5/umap/management/commands/generate_js_locale.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1902 2019-04-07 14:28:38.000000 umap-project-1.2.5/umap/management/commands/import_pictograms.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      207 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/managers.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      515 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/middleware.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.706575 umap-project-1.2.5/umap/migrations/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5563 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/migrations/0001_initial.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      373 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/migrations/0002_tilelayer_tms.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      812 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/migrations/0003_add_tilelayer.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      530 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/migrations/0004_add_licence.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      318 2018-07-14 11:58:47.000000 umap-project-1.2.5/umap/migrations/0005_remove_map_tilelayer.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      497 2019-04-07 08:09:35.000000 umap-project-1.2.5/umap/migrations/0006_auto_20190407_0719.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      515 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/migrations/0007_auto_20190416_1757.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      459 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/migrations/0008_alter_map_settings.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-11-26 16:02:45.000000 umap-project-1.2.5/umap/migrations/__init__.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11200 2023-05-10 08:16:33.000000 umap-project-1.2.5/umap/models.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.706575 umap-project-1.2.5/umap/settings/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1617 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/settings/__init__.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7922 2023-05-12 15:29:04.000000 umap-project-1.2.5/umap/settings/base.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      386 2018-05-19 15:10:46.000000 umap-project-1.2.5/umap/settings/dev.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.706575 umap-project-1.2.5/umap/static/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-04-23 07:38:39.000000 umap-project-1.2.5/umap/static/.gitignore
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      638 2016-04-23 07:38:39.000000 umap-project-1.2.5/umap/static/favicon.ico
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.743241 umap-project-1.2.5/umap/static/umap/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    17943 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/base.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9125 2016-04-23 07:38:39.000000 umap-project-1.2.5/umap/static/umap/bitbucket.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5851 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/static/umap/content.css
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.759907 umap-project-1.2.5/umap/static/umap/font/
+-rwxr-xr-x   0 ybon      (1000) ybon      (1000)   182984 2018-05-17 09:59:39.000000 umap-project-1.2.5/umap/static/umap/font/FiraSans-Light.woff
+-rwxr-xr-x   0 ybon      (1000) ybon      (1000)   129180 2018-05-17 09:59:39.000000 umap-project-1.2.5/umap/static/umap/font/FiraSans-Light.woff2
+-rwxr-xr-x   0 ybon      (1000) ybon      (1000)   191400 2018-05-17 09:59:39.000000 umap-project-1.2.5/umap/static/umap/font/FiraSans-LightItalic.woff
+-rwxr-xr-x   0 ybon      (1000) ybon      (1000)   135744 2018-05-17 09:59:39.000000 umap-project-1.2.5/umap/static/umap/font/FiraSans-LightItalic.woff2
+-rwxr-xr-x   0 ybon      (1000) ybon      (1000)   198128 2018-05-17 09:59:39.000000 umap-project-1.2.5/umap/static/umap/font/FiraSans-SemiBold.woff
+-rwxr-xr-x   0 ybon      (1000) ybon      (1000)   140168 2018-05-17 09:59:39.000000 umap-project-1.2.5/umap/static/umap/font/FiraSans-SemiBold.woff2
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      832 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/static/umap/font.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1564 2016-04-23 07:38:39.000000 umap-project-1.2.5/umap/static/umap/github.png
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.799906 umap-project-1.2.5/umap/static/umap/img/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    13636 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/static/umap/img/16-white.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    57263 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/static/umap/img/16-white.svg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11308 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/static/umap/img/16.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    38140 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/static/umap/img/16.svg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    19000 2023-05-10 08:16:33.000000 umap-project-1.2.5/umap/static/umap/img/24-white.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    38375 2023-05-10 08:16:33.000000 umap-project-1.2.5/umap/static/umap/img/24-white.svg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    15600 2023-05-10 08:16:33.000000 umap-project-1.2.5/umap/static/umap/img/24.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    35215 2023-05-10 08:16:33.000000 umap-project-1.2.5/umap/static/umap/img/24.svg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      430 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/static/umap/img/edit-16.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3491 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/img/edit.svg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      190 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/static/umap/img/icon-bg.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3338 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/img/logo.svg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5537 2016-04-23 07:38:39.000000 umap-project-1.2.5/umap/static/umap/img/logo_filigree.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      375 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/static/umap/img/marker.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3679 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/img/opensource.svg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8351 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/img/osm.svg
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1472 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/static/umap/img/search.gif
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.813238 umap-project-1.2.5/umap/static/umap/js/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9173 2019-01-30 10:00:11.000000 umap-project-1.2.5/umap/static/umap/js/umap.autocomplete.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    36638 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/js/umap.controls.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    20447 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/js/umap.core.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    35418 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/js/umap.features.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    27098 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/js/umap.forms.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6376 2019-01-30 10:04:17.000000 umap-project-1.2.5/umap/static/umap/js/umap.icon.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    68064 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/js/umap.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    37049 2023-05-12 15:33:20.000000 umap-project-1.2.5/umap/static/umap/js/umap.layer.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5905 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/static/umap/js/umap.permissions.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7420 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/js/umap.popup.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5192 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/static/umap/js/umap.slideshow.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     4527 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/static/umap/js/umap.tableeditor.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7351 2019-01-30 09:54:21.000000 umap-project-1.2.5/umap/static/umap/js/umap.ui.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10308 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/static/umap/js/umap.xhr.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.899902 umap-project-1.2.5/umap/static/umap/locale/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    26175 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/am_ET.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    26104 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/am_ET.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21793 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/ar.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21728 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/ar.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21441 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/ast.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21374 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/ast.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    25216 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/bg.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    25151 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/bg.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22330 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/ca.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22265 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/ca.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23183 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/cs_CZ.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23112 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/cs_CZ.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21882 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/da.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21817 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/da.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23385 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/de.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23320 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/de.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    32772 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/el.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    32707 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/el.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21439 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/en.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21374 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/en.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21074 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/en_US.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23662 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/es.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23597 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/es.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21722 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/et.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21657 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/et.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21385 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/fa_IR.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22517 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/fi.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22452 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/fi.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23449 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/fr.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23384 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/fr.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23153 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/gl.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23088 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/gl.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    25737 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/he.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    25672 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/he.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21649 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/hr.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21584 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/hr.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24563 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/hu.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24498 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/hu.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21439 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/id.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21374 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/id.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23074 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/is.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23009 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/is.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23148 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/it.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23083 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/it.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24685 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/ja.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24620 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/ja.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21661 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/ko.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21596 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/ko.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22412 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/lt.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22347 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/lt.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22430 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/ms.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23099 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/nl.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23034 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/nl.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21717 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/no.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21652 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/no.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22981 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/pl.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22916 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/pl.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21032 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/pl_PL.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22790 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/pt.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23065 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/pt.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23120 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/pt_BR.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23049 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/pt_BR.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23129 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/pt_PT.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23058 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/pt_PT.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21500 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/ro.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21435 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/ro.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    30478 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/ru.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    30413 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/ru.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21445 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/si_LK.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21374 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/si_LK.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22965 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/sk_SK.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22894 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/sk_SK.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22816 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/sl.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22751 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/sl.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    24039 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/sr.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23974 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/sr.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22736 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/sv.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    22671 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/sv.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21445 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/th_TH.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21374 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/th_TH.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23321 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/tr.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23256 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/tr.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    29961 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/uk_UA.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    29890 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/uk_UA.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21818 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/vi.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21753 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/vi.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21374 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/vi_VN.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21067 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/zh.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21002 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/zh.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21374 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/zh_CN.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21374 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/zh_TW.Big5.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21076 2023-05-12 15:39:45.000000 umap-project-1.2.5/umap/static/umap/locale/zh_TW.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    21005 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/locale/zh_TW.json
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    31281 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/map.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1492 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/static/umap/nav.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    19408 2016-04-23 07:38:39.000000 umap-project-1.2.5/umap/static/umap/openstreetmap.png
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.903236 umap-project-1.2.5/umap/static/umap/test/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      464 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/static/umap/test/.eslintrc
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1827 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/static/umap/test/Controls.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    12735 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/static/umap/test/DataLayer.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10204 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/static/umap/test/Feature.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    18216 2018-09-22 05:31:42.000000 umap-project-1.2.5/umap/static/umap/test/Map.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3472 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/static/umap/test/Marker.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2612 2018-09-22 08:09:19.000000 umap-project-1.2.5/umap/static/umap/test/Permissions.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    13314 2018-09-05 19:34:30.000000 umap-project-1.2.5/umap/static/umap/test/Polygon.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    14952 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/static/umap/test/Polyline.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3626 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/static/umap/test/TableEditor.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11986 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/test/Util.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    10851 2018-09-05 19:34:50.000000 umap-project-1.2.5/umap/static/umap/test/_pre.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5695 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/static/umap/test/index.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)       49 2018-06-02 13:09:22.000000 umap-project-1.2.5/umap/static/umap/theme.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3225 2016-04-23 07:38:39.000000 umap-project-1.2.5/umap/static/umap/twitter.png
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.643244 umap-project-1.2.5/umap/static/umap/vendors/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.906569 umap-project-1.2.5/umap/static/umap/vendors/contextmenu/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1231 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    16343 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      990 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8994 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.909902 umap-project-1.2.5/umap/static/umap/vendors/csv2geojson/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    15029 2023-05-02 15:41:08.000000 umap-project-1.2.5/umap/static/umap/vendors/csv2geojson/csv2geojson.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     6994 2023-05-02 15:41:08.000000 umap-project-1.2.5/umap/static/umap/vendors/csv2geojson/index.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.913235 umap-project-1.2.5/umap/static/umap/vendors/editable/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    74768 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/editable/Leaflet.Editable.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3898 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/editable/Path.Drag.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.916568 umap-project-1.2.5/umap/static/umap/vendors/editinosm/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1263 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9141 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.916568 umap-project-1.2.5/umap/static/umap/vendors/formbuilder/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    12235 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/formbuilder/Leaflet.FormBuilder.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.919902 umap-project-1.2.5/umap/static/umap/vendors/fullscreen/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5041 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3654 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.min.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      299 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/fullscreen/fullscreen.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      420 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/fullscreen/fullscreen@2x.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      994 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/fullscreen/leaflet.fullscreen.css
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.919902 umap-project-1.2.5/umap/static/umap/vendors/georsstogeojson/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3202 2023-05-02 15:41:08.000000 umap-project-1.2.5/umap/static/umap/vendors/georsstogeojson/GeoRSSToGeoJSON.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.919902 umap-project-1.2.5/umap/static/umap/vendors/hash/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3462 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/hash/leaflet-hash.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.919902 umap-project-1.2.5/umap/static/umap/vendors/heat/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5158 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/heat/leaflet-heat.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.919902 umap-project-1.2.5/umap/static/umap/vendors/i18n/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1305 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/i18n/Leaflet.i18n.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.943234 umap-project-1.2.5/umap/static/umap/vendors/leaflet/
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.949901 umap-project-1.2.5/umap/static/umap/vendors/leaflet/images/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1259 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/leaflet/images/layers-2x.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      696 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/leaflet/images/layers.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2464 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/leaflet/images/marker-icon-2x.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1466 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/leaflet/images/marker-icon.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      618 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/leaflet/images/marker-shadow.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)   398517 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/leaflet/leaflet-src.esm.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)   759894 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/leaflet/leaflet-src.esm.js.map
+-rw-r--r--   0 ybon      (1000) ybon      (1000)   400242 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/leaflet/leaflet-src.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)   759986 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/leaflet/leaflet-src.js.map
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    14106 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/leaflet/leaflet.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)   140468 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/leaflet/leaflet.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)   191112 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/leaflet/leaflet.js.map
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.959900 umap-project-1.2.5/umap/static/umap/vendors/loading/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3252 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/loading/Control.Loading.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    14143 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/loading/Control.Loading.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.959900 umap-project-1.2.5/umap/static/umap/vendors/locatecontrol/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2471 2023-05-02 15:41:08.000000 umap-project-1.2.5/umap/static/umap/vendors/locatecontrol/L.Control.Locate.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    30907 2023-05-02 15:41:08.000000 umap-project-1.2.5/umap/static/umap/vendors/locatecontrol/L.Control.Locate.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.966567 umap-project-1.2.5/umap/static/umap/vendors/markercluster/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1346 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/markercluster/MarkerCluster.Default.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      886 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/markercluster/MarkerCluster.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      318 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/markercluster/WhereAreTheJavascriptFiles.txt
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    80271 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)   157229 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js.map
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    33679 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/markercluster/leaflet.markercluster.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    27566 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/markercluster/leaflet.markercluster.js.map
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.969900 umap-project-1.2.5/umap/static/umap/vendors/measurable/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      937 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/measurable/Leaflet.Measurable.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7256 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/measurable/Leaflet.Measurable.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.969900 umap-project-1.2.5/umap/static/umap/vendors/minimap/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1998 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/minimap/Control.MiniMap.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    12129 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/minimap/Control.MiniMap.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.969900 umap-project-1.2.5/umap/static/umap/vendors/minimap/images/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      219 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/minimap/images/toggle.png
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     8057 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/minimap/images/toggle.svg
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.969900 umap-project-1.2.5/umap/static/umap/vendors/osmtogeojson/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    35642 2023-05-02 15:41:08.000000 umap-project-1.2.5/umap/static/umap/vendors/osmtogeojson/osmtogeojson.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.973233 umap-project-1.2.5/umap/static/umap/vendors/photon/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    14433 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/photon/leaflet.photon.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.979900 umap-project-1.2.5/umap/static/umap/vendors/print/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    44559 2021-09-12 08:45:21.000000 umap-project-1.2.5/umap/static/umap/vendors/print/leaflet.browser.print.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    23442 2021-09-12 08:45:21.000000 umap-project-1.2.5/umap/static/umap/vendors/print/leaflet.browser.print.min.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.979900 umap-project-1.2.5/umap/static/umap/vendors/togeojson/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    18098 2023-05-02 15:41:08.000000 umap-project-1.2.5/umap/static/umap/vendors/togeojson/togeojson.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.979900 umap-project-1.2.5/umap/static/umap/vendors/togpx/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    17936 2023-05-02 15:41:08.000000 umap-project-1.2.5/umap/static/umap/vendors/togpx/togpx.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.983233 umap-project-1.2.5/umap/static/umap/vendors/tokml/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    11521 2023-05-02 15:41:08.000000 umap-project-1.2.5/umap/static/umap/vendors/tokml/tokml.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.983233 umap-project-1.2.5/umap/static/umap/vendors/toolbar/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2890 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     9060 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2244 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/toolbar/leaflet.toolbar.css
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     5326 2023-05-02 15:41:07.000000 umap-project-1.2.5/umap/static/umap/vendors/toolbar/leaflet.toolbar.js
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.983233 umap-project-1.2.5/umap/templates/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      305 2016-04-23 07:38:39.000000 umap-project-1.2.5/umap/templates/404.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     4904 2016-04-23 07:38:39.000000 umap-project-1.2.5/umap/templates/500.html
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.986566 umap-project-1.2.5/umap/templates/auth/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      467 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/templates/auth/user_detail.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      702 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/templates/base.html
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:46.986566 umap-project-1.2.5/umap/templates/registration/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1157 2023-03-01 18:10:17.000000 umap-project-1.2.5/umap/templates/registration/login.html
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:47.013232 umap-project-1.2.5/umap/templates/umap/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      128 2018-05-18 20:43:08.000000 umap-project-1.2.5/umap/templates/umap/about.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1844 2019-04-07 14:28:38.000000 umap-project-1.2.5/umap/templates/umap/about_summary.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2054 2019-02-09 11:02:16.000000 umap-project-1.2.5/umap/templates/umap/content.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      634 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/templates/umap/content_footer.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1212 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/templates/umap/css.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2018-05-18 20:43:08.000000 umap-project-1.2.5/umap/templates/umap/footer.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1117 2022-09-30 16:19:34.000000 umap-project-1.2.5/umap/templates/umap/home.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2987 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/templates/umap/js.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      112 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/templates/umap/locale.js
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      423 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/templates/umap/login_popup_end.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      595 2021-09-12 08:45:40.000000 umap-project-1.2.5/umap/templates/umap/map_detail.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      200 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/templates/umap/map_fragment.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      165 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/templates/umap/map_init.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      597 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/templates/umap/map_list.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      299 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/templates/umap/map_messages.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      985 2023-05-12 14:58:25.000000 umap-project-1.2.5/umap/templates/umap/navigation.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      878 2018-05-18 20:43:08.000000 umap-project-1.2.5/umap/templates/umap/password_change.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      258 2018-05-18 20:43:08.000000 umap-project-1.2.5/umap/templates/umap/password_change_done.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      390 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/templates/umap/search.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      448 2018-05-18 20:43:08.000000 umap-project-1.2.5/umap/templates/umap/search_bar.html
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        2 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/templates/umap/success.html
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:47.026565 umap-project-1.2.5/umap/templatetags/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-04-23 07:38:39.000000 umap-project-1.2.5/umap/templatetags/__init__.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2405 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/templatetags/umap_tags.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:47.033231 umap-project-1.2.5/umap/tests/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/tests/__init__.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2945 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/tests/base.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1285 2023-05-10 17:41:08.000000 umap-project-1.2.5/umap/tests/conftest.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      360 2023-05-05 17:42:43.000000 umap-project-1.2.5/umap/tests/settings.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2870 2023-02-27 10:29:01.000000 umap-project-1.2.5/umap/tests/test_datalayer.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     7190 2023-05-12 15:36:40.000000 umap-project-1.2.5/umap/tests/test_datalayer_views.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      339 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/tests/test_licence.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3149 2018-07-14 13:10:40.000000 umap-project-1.2.5/umap/tests/test_map.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    19486 2023-05-12 15:17:55.000000 umap-project-1.2.5/umap/tests/test_map_views.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      605 2018-07-14 08:06:10.000000 umap-project-1.2.5/umap/tests/test_tilelayer.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     3974 2018-08-04 16:35:43.000000 umap-project-1.2.5/umap/tests/test_views.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     4899 2023-05-10 08:16:33.000000 umap-project-1.2.5/umap/urls.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     4381 2023-05-12 15:29:04.000000 umap-project-1.2.5/umap/utils.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    26856 2023-05-12 15:36:40.000000 umap-project-1.2.5/umap/views.py
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     1152 2018-05-19 15:10:36.000000 umap-project-1.2.5/umap/wsgi.py
+drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-05-12 15:39:47.036565 umap-project-1.2.5/umap_project.egg-info/
+-rw-r--r--   0 ybon      (1000) ybon      (1000)     2165 2023-05-12 15:39:46.000000 umap-project-1.2.5/umap_project.egg-info/PKG-INFO
+-rw-r--r--   0 ybon      (1000) ybon      (1000)    13960 2023-05-12 15:39:46.000000 umap-project-1.2.5/umap_project.egg-info/SOURCES.txt
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        1 2023-05-12 15:39:46.000000 umap-project-1.2.5/umap_project.egg-info/dependency_links.txt
+-rw-r--r--   0 ybon      (1000) ybon      (1000)       39 2023-05-12 15:39:46.000000 umap-project-1.2.5/umap_project.egg-info/entry_points.txt
+-rw-r--r--   0 ybon      (1000) ybon      (1000)      265 2023-05-12 15:39:46.000000 umap-project-1.2.5/umap_project.egg-info/requires.txt
+-rw-r--r--   0 ybon      (1000) ybon      (1000)        5 2023-05-12 15:39:46.000000 umap-project-1.2.5/umap_project.egg-info/top_level.txt
```

### Comparing `umap-project-1.2.4/PKG-INFO` & `umap-project-1.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: umap-project
-Version: 1.2.4
+Version: 1.2.5
 Summary: Create maps with OpenStreetMap layers in a minute and embed them in your site.
-Home-page: UNKNOWN
 Author: Yohan Boniface
-License: UNKNOWN
 Keywords: django leaflet geodjango openstreetmap map
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.4
@@ -37,9 +34,7 @@
 *Because we think that the more OSM will be used, the more OSM will be improved.*
 It uses [django-leaflet-storage](https://github.com/umap-project/django-leaflet-storage) and [Leaflet.Storage](https://github.com/umap-project/Leaflet.Storage),  built on top of Django and Leaflet.
 
 
 ## Installation and configuration
 
 See [developer documentation](https://umap-project.readthedocs.io/en/latest/install/).
-
-
```

### Comparing `umap-project-1.2.4/README.md` & `umap-project-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/setup.cfg` & `umap-project-1.2.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = umap-project
-version = 1.2.4
+version = 1.2.5
 description = Create maps with OpenStreetMap layers in a minute and embed them in your site.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Yohan Boniface
 homepage = https://github.com/umap-project/umap
 keywords = django leaflet geodjango openstreetmap map
 classifiers =
```

### Comparing `umap-project-1.2.4/umap/admin.py` & `umap-project-1.2.5/umap/admin.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/autocomplete.py` & `umap-project-1.2.5/umap/autocomplete.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/decorators.py` & `umap-project-1.2.5/umap/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,51 +6,56 @@
 from django.conf import settings
 
 from .views import simple_json_response
 from .models import Map
 
 
 LOGIN_URL = getattr(settings, "LOGIN_URL", "login")
-LOGIN_URL = (reverse_lazy(LOGIN_URL) if not LOGIN_URL.startswith("/")
-             else LOGIN_URL)
+LOGIN_URL = reverse_lazy(LOGIN_URL) if not LOGIN_URL.startswith("/") else LOGIN_URL
 
 
 def login_required_if_not_anonymous_allowed(view_func):
     @wraps(view_func)
     def wrapper(request, *args, **kwargs):
-        if (not getattr(settings, "UMAP_ALLOW_ANONYMOUS", False)
-                and not request.user.is_authenticated):
+        if (
+            not getattr(settings, "UMAP_ALLOW_ANONYMOUS", False)
+            and not request.user.is_authenticated
+        ):
             return simple_json_response(login_required=str(LOGIN_URL))
         return view_func(request, *args, **kwargs)
+
     return wrapper
 
 
 def map_permissions_check(view_func):
     """
     Used for URLs dealing with the map.
     """
+
     @wraps(view_func)
     def wrapper(request, *args, **kwargs):
-        map_inst = get_object_or_404(Map, pk=kwargs['map_id'])
+        map_inst = get_object_or_404(Map, pk=kwargs["map_id"])
         user = request.user
-        kwargs['map_inst'] = map_inst  # Avoid rerequesting the map in the view
+        kwargs["map_inst"] = map_inst  # Avoid rerequesting the map in the view
         if map_inst.edit_status >= map_inst.EDITORS:
             can_edit = map_inst.can_edit(user=user, request=request)
             if not can_edit:
                 if map_inst.owner and not user.is_authenticated:
                     return simple_json_response(login_required=str(LOGIN_URL))
                 return HttpResponseForbidden()
         return view_func(request, *args, **kwargs)
+
     return wrapper
 
 
 def jsonize_view(view_func):
     @wraps(view_func)
     def wrapper(request, *args, **kwargs):
         response = view_func(request, *args, **kwargs)
         response_kwargs = {}
-        if hasattr(response, 'rendered_content'):
-            response_kwargs['html'] = response.rendered_content
-        if response.has_header('location'):
-            response_kwargs['redirect'] = response['location']
+        if hasattr(response, "rendered_content"):
+            response_kwargs["html"] = response.rendered_content
+        if response.has_header("location"):
+            response_kwargs["redirect"] = response["location"]
         return simple_json_response(**response_kwargs)
+
     return wrapper
```

### Comparing `umap-project-1.2.4/umap/fields.py` & `umap-project-1.2.5/umap/fields.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/forms.py` & `umap-project-1.2.5/umap/forms.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/am_ET/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/am_ET/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/am_ET/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/am_ET/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/ar/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/ar/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/ast/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/ast/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/bg/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/bg/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/ca/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/ca/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/cs_CZ/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/cs_CZ/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/cs_CZ/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/cs_CZ/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/da/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/da/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/da/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/de/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/de/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/el/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/el/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/el/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/en/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/es/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/es/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/et/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/et/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/fi/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/fi/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/fr/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/fr/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/gl/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/gl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/gl/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/gl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/he/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/he/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/hr/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/hr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/hr/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/hu/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/hu/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/id/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/is/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/is/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/is/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/is/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/it/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/it/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/ja/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/ja/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/ko/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/ko/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/lt/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/lt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/lt/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/nl/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/nl/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/no/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/no/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/pl/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/pl/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/pt/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/pt/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/pt_BR/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/pt_BR/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/pt_PT/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/pt_PT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/pt_PT/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/ro/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/ro/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/ru/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/ru/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/si_LK/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/si_LK/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/sk_SK/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/sk_SK/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/sk_SK/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/sk_SK/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/sl/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/sl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/sl/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/sl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/sr/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/sr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/sr/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/sr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/sv/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/sv/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/th_TH/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/th_TH/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/tr/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/tr/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/uk_UA/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/uk_UA/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/uk_UA/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/uk_UA/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/vi/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/vi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/vi/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/vi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/zh/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/zh/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/zh/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/zh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/zh_TW/LC_MESSAGES/django.mo` & `umap-project-1.2.5/umap/locale/zh_TW/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/locale/zh_TW/LC_MESSAGES/django.po` & `umap-project-1.2.5/umap/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/management/commands/anonymous_edit_url.py` & `umap-project-1.2.5/umap/management/commands/anonymous_edit_url.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/management/commands/generate_js_locale.py` & `umap-project-1.2.5/umap/management/commands/generate_js_locale.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/management/commands/import_pictograms.py` & `umap-project-1.2.5/umap/management/commands/import_pictograms.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/middleware.py` & `umap-project-1.2.5/umap/middleware.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/migrations/0001_initial.py` & `umap-project-1.2.5/umap/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/migrations/0003_add_tilelayer.py` & `umap-project-1.2.5/umap/migrations/0003_add_tilelayer.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/migrations/0004_add_licence.py` & `umap-project-1.2.5/umap/migrations/0004_add_licence.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/migrations/0007_auto_20190416_1757.py` & `umap-project-1.2.5/umap/migrations/0007_auto_20190416_1757.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/models.py` & `umap-project-1.2.5/umap/models.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/settings/__init__.py` & `umap-project-1.2.5/umap/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/settings/base.py` & `umap-project-1.2.5/umap/settings/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,15 @@
 MEDIA_ROOT = os.path.join('uploads')
 
 STATICFILES_FINDERS = [
     'django.contrib.staticfiles.finders.FileSystemFinder',
     'django.contrib.staticfiles.finders.AppDirectoriesFinder',
     'compressor.finders.CompressorFinder',
 ]
+STATICFILES_DIRS = []  # May be extended when using UMAP_CUSTOM_STATICS
 
 # =============================================================================
 # Templates
 # =============================================================================
 
 TEMPLATES = [
     {
@@ -211,14 +212,15 @@
 DATABASES = {
     'default': {
         'ENGINE': 'django.contrib.gis.db.backends.postgis',
         'NAME': 'umap',
     }
 }
 UMAP_READONLY = False
+UMAP_GZIP = True
 LOCALE_PATHS = [os.path.join(PROJECT_DIR, 'locale')]
 
 # =============================================================================
 # Third party app settings
 # =============================================================================
 COMPRESS_ENABLED = True
 COMPRESS_OFFLINE = True
```

### Comparing `umap-project-1.2.4/umap/static/favicon.ico` & `umap-project-1.2.5/umap/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/base.css` & `umap-project-1.2.5/umap/static/umap/base.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/bitbucket.png` & `umap-project-1.2.5/umap/static/umap/bitbucket.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/content.css` & `umap-project-1.2.5/umap/static/umap/content.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/font/FiraSans-Light.woff` & `umap-project-1.2.5/umap/static/umap/font/FiraSans-Light.woff`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/font/FiraSans-Light.woff2` & `umap-project-1.2.5/umap/static/umap/font/FiraSans-Light.woff2`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/font/FiraSans-LightItalic.woff` & `umap-project-1.2.5/umap/static/umap/font/FiraSans-LightItalic.woff`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/font/FiraSans-LightItalic.woff2` & `umap-project-1.2.5/umap/static/umap/font/FiraSans-LightItalic.woff2`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/font/FiraSans-SemiBold.woff` & `umap-project-1.2.5/umap/static/umap/font/FiraSans-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/font/FiraSans-SemiBold.woff2` & `umap-project-1.2.5/umap/static/umap/font/FiraSans-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/font.css` & `umap-project-1.2.5/umap/static/umap/font.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/github.png` & `umap-project-1.2.5/umap/static/umap/github.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/img/16-white.png` & `umap-project-1.2.5/umap/static/umap/img/16-white.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/img/16-white.svg` & `umap-project-1.2.5/umap/static/umap/img/16-white.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/img/16.png` & `umap-project-1.2.5/umap/static/umap/img/16.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/img/16.svg` & `umap-project-1.2.5/umap/static/umap/img/16.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/img/24-white.png` & `umap-project-1.2.5/umap/static/umap/img/24-white.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/img/24-white.svg` & `umap-project-1.2.5/umap/static/umap/img/24-white.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/img/24.png` & `umap-project-1.2.5/umap/static/umap/img/24.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/img/24.svg` & `umap-project-1.2.5/umap/static/umap/img/24.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/img/edit.svg` & `umap-project-1.2.5/umap/static/umap/img/edit.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/img/logo.svg` & `umap-project-1.2.5/umap/static/umap/img/logo.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/img/logo_filigree.png` & `umap-project-1.2.5/umap/static/umap/img/logo_filigree.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/img/opensource.svg` & `umap-project-1.2.5/umap/static/umap/img/opensource.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/img/osm.svg` & `umap-project-1.2.5/umap/static/umap/img/osm.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/img/search.gif` & `umap-project-1.2.5/umap/static/umap/img/search.gif`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/js/umap.autocomplete.js` & `umap-project-1.2.5/umap/static/umap/js/umap.autocomplete.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/js/umap.controls.js` & `umap-project-1.2.5/umap/static/umap/js/umap.controls.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/js/umap.core.js` & `umap-project-1.2.5/umap/static/umap/js/umap.core.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/js/umap.features.js` & `umap-project-1.2.5/umap/static/umap/js/umap.features.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/js/umap.forms.js` & `umap-project-1.2.5/umap/static/umap/js/umap.forms.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/js/umap.icon.js` & `umap-project-1.2.5/umap/static/umap/js/umap.icon.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/js/umap.js` & `umap-project-1.2.5/umap/static/umap/js/umap.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/js/umap.layer.js` & `umap-project-1.2.5/umap/static/umap/js/umap.layer.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -289,15 +289,15 @@
         return this;
     },
 
     fetchData: function() {
         if (!this.umap_id) return;
         this.map.get(this._dataUrl(), {
             callback: function(geojson, response) {
-                this._etag = response.getResponseHeader('ETag');
+                this._last_modified = response.getResponseHeader('Last-Modified');
                 this.fromUmapGeoJSON(geojson);
                 this.backupOptions();
                 this.fire('loaded');
             },
             context: this
         });
     },
@@ -418,19 +418,22 @@
             this.map.datalayers[id] = this;
             if (L.Util.indexOf(this.map.datalayers_index, this) === -1) this.map.datalayers_index.push(this);
         }
         this.map.updateDatalayersControl();
     },
 
     _dataUrl: function() {
-        var template = this.map.options.urls.datalayer_view;
-        return L.Util.template(template, {
-            'pk': this.umap_id,
-            'map_id': this.map.options.umap_id
-        });
+        var template = this.map.options.urls.datalayer_view,
+            url = L.Util.template(template, {
+                'pk': this.umap_id,
+                'map_id': this.map.options.umap_id
+            });
+        // No browser cache for owners/editors.
+        if (this.map.options.allowEdit) url = url + '?' + Date.now();
+        return url;
     },
 
     isRemoteLayer: function() {
         return !!(this.options.remoteData && this.options.remoteData.url && this.options.remoteData.format);
     },
 
     isClustered: function() {
@@ -1136,28 +1139,28 @@
             type: 'application/json'
         });
         formData.append('geojson', blob);
         this.map.post(this.getSaveUrl(), {
             data: formData,
             callback: function(data, response) {
                 this._geojson = geojson;
-                this._etag = response.getResponseHeader('ETag');
+                this._last_modified = response.getResponseHeader('Last-Modified');
                 this.setUmapId(data.id);
                 this.updateOptions(data);
                 this.backupOptions();
                 this.connectToMap();
                 this._loaded = true;
                 this.redraw(); // Needed for reordering features
                 this.isDirty = false;
                 this.map.continueSaving();
             },
             context: this,
-            headers: {
-                'If-Match': this._etag || ''
-            }
+            headers: this._last_modified ? {
+                'If-Unmodified-Since': this._last_modified
+            } : {}
         });
     },
 
     saveDelete: function() {
         var callback = function() {
             this.isDirty = false;
             this.map.continueSaving();
```

### Comparing `umap-project-1.2.4/umap/static/umap/js/umap.permissions.js` & `umap-project-1.2.5/umap/static/umap/js/umap.permissions.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/js/umap.popup.js` & `umap-project-1.2.5/umap/static/umap/js/umap.popup.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/js/umap.slideshow.js` & `umap-project-1.2.5/umap/static/umap/js/umap.slideshow.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/js/umap.tableeditor.js` & `umap-project-1.2.5/umap/static/umap/js/umap.tableeditor.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/js/umap.ui.js` & `umap-project-1.2.5/umap/static/umap/js/umap.ui.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/js/umap.xhr.js` & `umap-project-1.2.5/umap/static/umap/js/umap.xhr.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/am_ET.js` & `umap-project-1.2.5/umap/static/umap/locale/am_ET.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/am_ET.json` & `umap-project-1.2.5/umap/static/umap/locale/am_ET.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/ar.js` & `umap-project-1.2.5/umap/static/umap/locale/ar.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/ar.json` & `umap-project-1.2.5/umap/static/umap/locale/ar.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/ast.js` & `umap-project-1.2.5/umap/static/umap/locale/ast.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/ast.json` & `umap-project-1.2.5/umap/static/umap/locale/ast.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/bg.js` & `umap-project-1.2.5/umap/static/umap/locale/bg.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/bg.json` & `umap-project-1.2.5/umap/static/umap/locale/bg.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/ca.js` & `umap-project-1.2.5/umap/static/umap/locale/ca.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/ca.json` & `umap-project-1.2.5/umap/static/umap/locale/ca.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/cs_CZ.js` & `umap-project-1.2.5/umap/static/umap/locale/cs_CZ.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/cs_CZ.json` & `umap-project-1.2.5/umap/static/umap/locale/cs_CZ.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/da.js` & `umap-project-1.2.5/umap/static/umap/locale/da.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/da.json` & `umap-project-1.2.5/umap/static/umap/locale/da.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/de.js` & `umap-project-1.2.5/umap/static/umap/locale/de.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/de.json` & `umap-project-1.2.5/umap/static/umap/locale/de.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/el.js` & `umap-project-1.2.5/umap/static/umap/locale/el.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/el.json` & `umap-project-1.2.5/umap/static/umap/locale/el.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/en.js` & `umap-project-1.2.5/umap/static/umap/locale/en.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/en.json` & `umap-project-1.2.5/umap/static/umap/locale/en.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/en_US.json` & `umap-project-1.2.5/umap/static/umap/locale/en_US.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/es.js` & `umap-project-1.2.5/umap/static/umap/locale/es.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/es.json` & `umap-project-1.2.5/umap/static/umap/locale/es.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/et.js` & `umap-project-1.2.5/umap/static/umap/locale/et.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/et.json` & `umap-project-1.2.5/umap/static/umap/locale/et.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/fa_IR.json` & `umap-project-1.2.5/umap/static/umap/locale/fa_IR.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/fi.js` & `umap-project-1.2.5/umap/static/umap/locale/fi.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/fi.json` & `umap-project-1.2.5/umap/static/umap/locale/fi.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/fr.js` & `umap-project-1.2.5/umap/static/umap/locale/fr.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/fr.json` & `umap-project-1.2.5/umap/static/umap/locale/fr.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/gl.js` & `umap-project-1.2.5/umap/static/umap/locale/gl.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/gl.json` & `umap-project-1.2.5/umap/static/umap/locale/gl.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/he.js` & `umap-project-1.2.5/umap/static/umap/locale/he.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/he.json` & `umap-project-1.2.5/umap/static/umap/locale/he.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/hr.js` & `umap-project-1.2.5/umap/static/umap/locale/hr.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/hr.json` & `umap-project-1.2.5/umap/static/umap/locale/hr.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/hu.js` & `umap-project-1.2.5/umap/static/umap/locale/hu.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/hu.json` & `umap-project-1.2.5/umap/static/umap/locale/hu.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/id.js` & `umap-project-1.2.5/umap/static/umap/locale/id.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/id.json` & `umap-project-1.2.5/umap/static/umap/locale/id.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/is.js` & `umap-project-1.2.5/umap/static/umap/locale/is.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/is.json` & `umap-project-1.2.5/umap/static/umap/locale/is.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/it.js` & `umap-project-1.2.5/umap/static/umap/locale/it.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/it.json` & `umap-project-1.2.5/umap/static/umap/locale/it.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/ja.js` & `umap-project-1.2.5/umap/static/umap/locale/ja.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/ja.json` & `umap-project-1.2.5/umap/static/umap/locale/ja.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/ko.js` & `umap-project-1.2.5/umap/static/umap/locale/ko.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/ko.json` & `umap-project-1.2.5/umap/static/umap/locale/ko.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/lt.js` & `umap-project-1.2.5/umap/static/umap/locale/lt.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/lt.json` & `umap-project-1.2.5/umap/static/umap/locale/lt.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/ms.json` & `umap-project-1.2.5/umap/static/umap/locale/ms.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/nl.js` & `umap-project-1.2.5/umap/static/umap/locale/nl.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/nl.json` & `umap-project-1.2.5/umap/static/umap/locale/nl.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/no.js` & `umap-project-1.2.5/umap/static/umap/locale/no.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/no.json` & `umap-project-1.2.5/umap/static/umap/locale/no.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/pl.js` & `umap-project-1.2.5/umap/static/umap/locale/pl.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/pl.json` & `umap-project-1.2.5/umap/static/umap/locale/pl.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/pl_PL.json` & `umap-project-1.2.5/umap/static/umap/locale/pl_PL.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/pt.js` & `umap-project-1.2.5/umap/static/umap/locale/pt.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/pt.json` & `umap-project-1.2.5/umap/static/umap/locale/pt.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/pt_BR.js` & `umap-project-1.2.5/umap/static/umap/locale/pt_BR.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/pt_BR.json` & `umap-project-1.2.5/umap/static/umap/locale/pt_BR.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/pt_PT.js` & `umap-project-1.2.5/umap/static/umap/locale/pt_PT.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/pt_PT.json` & `umap-project-1.2.5/umap/static/umap/locale/pt_PT.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/ro.js` & `umap-project-1.2.5/umap/static/umap/locale/ro.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/ro.json` & `umap-project-1.2.5/umap/static/umap/locale/ro.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/ru.js` & `umap-project-1.2.5/umap/static/umap/locale/ru.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/ru.json` & `umap-project-1.2.5/umap/static/umap/locale/ru.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/si_LK.js` & `umap-project-1.2.5/umap/static/umap/locale/si_LK.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/si_LK.json` & `umap-project-1.2.5/umap/static/umap/locale/si_LK.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/sk_SK.js` & `umap-project-1.2.5/umap/static/umap/locale/sk_SK.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/sk_SK.json` & `umap-project-1.2.5/umap/static/umap/locale/sk_SK.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/sl.js` & `umap-project-1.2.5/umap/static/umap/locale/sl.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/sl.json` & `umap-project-1.2.5/umap/static/umap/locale/sl.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/sr.js` & `umap-project-1.2.5/umap/static/umap/locale/sr.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/sr.json` & `umap-project-1.2.5/umap/static/umap/locale/sr.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/sv.js` & `umap-project-1.2.5/umap/static/umap/locale/sv.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/sv.json` & `umap-project-1.2.5/umap/static/umap/locale/sv.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/th_TH.js` & `umap-project-1.2.5/umap/static/umap/locale/th_TH.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/th_TH.json` & `umap-project-1.2.5/umap/static/umap/locale/th_TH.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/tr.js` & `umap-project-1.2.5/umap/static/umap/locale/tr.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/tr.json` & `umap-project-1.2.5/umap/static/umap/locale/tr.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/uk_UA.js` & `umap-project-1.2.5/umap/static/umap/locale/uk_UA.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/uk_UA.json` & `umap-project-1.2.5/umap/static/umap/locale/uk_UA.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/vi.js` & `umap-project-1.2.5/umap/static/umap/locale/vi.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/vi.json` & `umap-project-1.2.5/umap/static/umap/locale/vi.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/vi_VN.json` & `umap-project-1.2.5/umap/static/umap/locale/vi_VN.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/zh.js` & `umap-project-1.2.5/umap/static/umap/locale/zh.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/zh.json` & `umap-project-1.2.5/umap/static/umap/locale/zh.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/zh_CN.json` & `umap-project-1.2.5/umap/static/umap/locale/zh_CN.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/zh_TW.Big5.json` & `umap-project-1.2.5/umap/static/umap/locale/zh_TW.Big5.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/zh_TW.js` & `umap-project-1.2.5/umap/static/umap/locale/zh_TW.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/locale/zh_TW.json` & `umap-project-1.2.5/umap/static/umap/locale/zh_TW.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/map.css` & `umap-project-1.2.5/umap/static/umap/map.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/nav.css` & `umap-project-1.2.5/umap/static/umap/nav.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/openstreetmap.png` & `umap-project-1.2.5/umap/static/umap/openstreetmap.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/test/Controls.js` & `umap-project-1.2.5/umap/static/umap/test/Controls.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/test/DataLayer.js` & `umap-project-1.2.5/umap/static/umap/test/DataLayer.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/test/Feature.js` & `umap-project-1.2.5/umap/static/umap/test/Feature.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/test/Map.js` & `umap-project-1.2.5/umap/static/umap/test/Map.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/test/Marker.js` & `umap-project-1.2.5/umap/static/umap/test/Marker.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/test/Permissions.js` & `umap-project-1.2.5/umap/static/umap/test/Permissions.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/test/Polygon.js` & `umap-project-1.2.5/umap/static/umap/test/Polygon.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/test/Polyline.js` & `umap-project-1.2.5/umap/static/umap/test/Polyline.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/test/TableEditor.js` & `umap-project-1.2.5/umap/static/umap/test/TableEditor.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/test/Util.js` & `umap-project-1.2.5/umap/static/umap/test/Util.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/test/_pre.js` & `umap-project-1.2.5/umap/static/umap/test/_pre.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/test/index.html` & `umap-project-1.2.5/umap/static/umap/test/index.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/twitter.png` & `umap-project-1.2.5/umap/static/umap/twitter.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.css` & `umap-project-1.2.5/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.js` & `umap-project-1.2.5/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.css` & `umap-project-1.2.5/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.js` & `umap-project-1.2.5/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/csv2geojson/csv2geojson.js` & `umap-project-1.2.5/umap/static/umap/vendors/csv2geojson/csv2geojson.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/csv2geojson/index.js` & `umap-project-1.2.5/umap/static/umap/vendors/csv2geojson/index.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/editable/Leaflet.Editable.js` & `umap-project-1.2.5/umap/static/umap/vendors/editable/Leaflet.Editable.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/editable/Path.Drag.js` & `umap-project-1.2.5/umap/static/umap/vendors/editable/Path.Drag.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.css` & `umap-project-1.2.5/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.js` & `umap-project-1.2.5/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/formbuilder/Leaflet.FormBuilder.js` & `umap-project-1.2.5/umap/static/umap/vendors/formbuilder/Leaflet.FormBuilder.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.js` & `umap-project-1.2.5/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.min.js` & `umap-project-1.2.5/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.min.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/fullscreen/leaflet.fullscreen.css` & `umap-project-1.2.5/umap/static/umap/vendors/fullscreen/leaflet.fullscreen.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/georsstogeojson/GeoRSSToGeoJSON.js` & `umap-project-1.2.5/umap/static/umap/vendors/georsstogeojson/GeoRSSToGeoJSON.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/hash/leaflet-hash.js` & `umap-project-1.2.5/umap/static/umap/vendors/hash/leaflet-hash.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/heat/leaflet-heat.js` & `umap-project-1.2.5/umap/static/umap/vendors/heat/leaflet-heat.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/i18n/Leaflet.i18n.js` & `umap-project-1.2.5/umap/static/umap/vendors/i18n/Leaflet.i18n.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/leaflet/images/layers-2x.png` & `umap-project-1.2.5/umap/static/umap/vendors/leaflet/images/layers-2x.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/leaflet/images/layers.png` & `umap-project-1.2.5/umap/static/umap/vendors/leaflet/images/layers.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/leaflet/images/marker-icon-2x.png` & `umap-project-1.2.5/umap/static/umap/vendors/leaflet/images/marker-icon-2x.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/leaflet/images/marker-icon.png` & `umap-project-1.2.5/umap/static/umap/vendors/leaflet/images/marker-icon.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/leaflet/images/marker-shadow.png` & `umap-project-1.2.5/umap/static/umap/vendors/leaflet/images/marker-shadow.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/leaflet/leaflet-src.esm.js` & `umap-project-1.2.5/umap/static/umap/vendors/leaflet/leaflet-src.esm.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/leaflet/leaflet-src.esm.js.map` & `umap-project-1.2.5/umap/static/umap/vendors/leaflet/leaflet-src.esm.js.map`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/leaflet/leaflet-src.js` & `umap-project-1.2.5/umap/static/umap/vendors/leaflet/leaflet-src.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/leaflet/leaflet-src.js.map` & `umap-project-1.2.5/umap/static/umap/vendors/leaflet/leaflet-src.js.map`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/leaflet/leaflet.css` & `umap-project-1.2.5/umap/static/umap/vendors/leaflet/leaflet.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/leaflet/leaflet.js` & `umap-project-1.2.5/umap/static/umap/vendors/leaflet/leaflet.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/leaflet/leaflet.js.map` & `umap-project-1.2.5/umap/static/umap/vendors/leaflet/leaflet.js.map`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/loading/Control.Loading.css` & `umap-project-1.2.5/umap/static/umap/vendors/loading/Control.Loading.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/loading/Control.Loading.js` & `umap-project-1.2.5/umap/static/umap/vendors/loading/Control.Loading.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/locatecontrol/L.Control.Locate.css` & `umap-project-1.2.5/umap/static/umap/vendors/locatecontrol/L.Control.Locate.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/locatecontrol/L.Control.Locate.js` & `umap-project-1.2.5/umap/static/umap/vendors/locatecontrol/L.Control.Locate.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/markercluster/MarkerCluster.Default.css` & `umap-project-1.2.5/umap/static/umap/vendors/markercluster/MarkerCluster.Default.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/markercluster/MarkerCluster.css` & `umap-project-1.2.5/umap/static/umap/vendors/markercluster/MarkerCluster.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js` & `umap-project-1.2.5/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js.map` & `umap-project-1.2.5/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js.map`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/markercluster/leaflet.markercluster.js` & `umap-project-1.2.5/umap/static/umap/vendors/markercluster/leaflet.markercluster.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/markercluster/leaflet.markercluster.js.map` & `umap-project-1.2.5/umap/static/umap/vendors/markercluster/leaflet.markercluster.js.map`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/measurable/Leaflet.Measurable.css` & `umap-project-1.2.5/umap/static/umap/vendors/measurable/Leaflet.Measurable.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/measurable/Leaflet.Measurable.js` & `umap-project-1.2.5/umap/static/umap/vendors/measurable/Leaflet.Measurable.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -22,61 +22,61 @@
     readableArea: function(area, unit) {
         var areaStr;
 
         if (unit === 'mi') {
             // Square yards in 1 meter
             area /= 0.836127;
             //3097600 square yards in 1 square mile
-            if (area >= 3097600) areaStr = L._('{area} mi&sup2;', {
+            if (area >= 3097600) areaStr = L._('{area}&#8239;mi&sup2;', {
                 area: (area / 3097600).toFixed(2)
             });
             //48040 square yards in 1 acre
-            else if (area >= 4840) areaStr = L._('{area} acres', {
+            else if (area >= 4840) areaStr = L._('{area}&#8239;acres', {
                 area: (area / 4840).toFixed(2)
             });
-            else areaStr = L._('{area} yd&sup2;'), {
+            else areaStr = L._('{area}&#8239;yd&sup2;'), {
                 area: Math.ceil(area)
             };
         } else {
-            if (area >= 100000) areaStr = L._('{area} ha', {
+            if (area >= 100000) areaStr = L._('{area}&#8239;ha', {
                 area: (area * 0.0001).toFixed(2)
             });
-            else areaStr = L._('{area} m&sup2;', {
+            else areaStr = L._('{area}&#8239;m&sup2;', {
                 area: area.toFixed(2)
             });
         }
 
         return areaStr;
     },
 
     readableDistance: function(distance, unit) {
         var distanceStr;
 
         if (unit === 'mi') {
             distance *= 1.09361;
-            if (distance > 1760) distanceStr = L._('{distance} miles', {
-                distance: (distance / 1760).toFixed(2)
+            if (distance > 1760) distanceStr = L._('{distance}&#8239;miles', {
+                distance: (distance / 1760).toFixed(1)
             });
-            else distanceStr = L._('{distance} yd', {
-                distance: Math.ceil(distance)
+            else distanceStr = L._('{distance}&#8239;yd', {
+                distance: distance.toFixed(2)
             });
         } else if (unit === 'nm') {
             distance /= 1852;
-            distanceStr = L._('{distance} NM', {
+            distanceStr = L._('{distance}&#8239;NM', {
                 distance: Math.ceil(distance)
             });
         } else {
-            if (distance > 100000) distanceStr = L._('{distance} km', {
+            if (distance > 100000) distanceStr = L._('{distance}&#8239;km', {
                 distance: Math.ceil(distance / 1000)
             });
-            else if (distance > 1000) distanceStr = L._('{distance} km', {
-                distance: (distance / 1000).toFixed(2)
+            else if (distance > 1000) distanceStr = L._('{distance}&#8239;km', {
+                distance: (distance / 1000).toFixed(1)
             });
-            else distanceStr = L._('{distance} m', {
-                distance: Math.ceil(distance)
+            else distanceStr = L._('{distance}&#8239;m', {
+                distance: distance.toFixed(2)
             });
         }
 
         return distanceStr;
     },
 
     lineLength: function(map, latlngs) {
```

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/minimap/Control.MiniMap.css` & `umap-project-1.2.5/umap/static/umap/vendors/minimap/Control.MiniMap.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/minimap/Control.MiniMap.js` & `umap-project-1.2.5/umap/static/umap/vendors/minimap/Control.MiniMap.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/minimap/images/toggle.svg` & `umap-project-1.2.5/umap/static/umap/vendors/minimap/images/toggle.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/osmtogeojson/osmtogeojson.js` & `umap-project-1.2.5/umap/static/umap/vendors/osmtogeojson/osmtogeojson.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/photon/leaflet.photon.js` & `umap-project-1.2.5/umap/static/umap/vendors/photon/leaflet.photon.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/print/leaflet.browser.print.js` & `umap-project-1.2.5/umap/static/umap/vendors/print/leaflet.browser.print.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/print/leaflet.browser.print.min.js` & `umap-project-1.2.5/umap/static/umap/vendors/print/leaflet.browser.print.min.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/togeojson/togeojson.js` & `umap-project-1.2.5/umap/static/umap/vendors/togeojson/togeojson.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/togpx/togpx.js` & `umap-project-1.2.5/umap/static/umap/vendors/togpx/togpx.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/tokml/tokml.js` & `umap-project-1.2.5/umap/static/umap/vendors/tokml/tokml.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.css` & `umap-project-1.2.5/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.js` & `umap-project-1.2.5/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/toolbar/leaflet.toolbar.css` & `umap-project-1.2.5/umap/static/umap/vendors/toolbar/leaflet.toolbar.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/static/umap/vendors/toolbar/leaflet.toolbar.js` & `umap-project-1.2.5/umap/static/umap/vendors/toolbar/leaflet.toolbar.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/templates/500.html` & `umap-project-1.2.5/umap/templates/500.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/templates/base.html` & `umap-project-1.2.5/umap/templates/base.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/templates/registration/login.html` & `umap-project-1.2.5/umap/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/templates/umap/about_summary.html` & `umap-project-1.2.5/umap/templates/umap/about_summary.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/templates/umap/content.html` & `umap-project-1.2.5/umap/templates/umap/content.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/templates/umap/content_footer.html` & `umap-project-1.2.5/umap/templates/umap/content_footer.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/templates/umap/css.html` & `umap-project-1.2.5/umap/templates/umap/css.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/templates/umap/home.html` & `umap-project-1.2.5/umap/templates/umap/home.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/templates/umap/js.html` & `umap-project-1.2.5/umap/templates/umap/js.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/templates/umap/map_detail.html` & `umap-project-1.2.5/umap/templates/umap/map_detail.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/templates/umap/map_list.html` & `umap-project-1.2.5/umap/templates/umap/map_list.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/templates/umap/navigation.html` & `umap-project-1.2.5/umap/templates/umap/navigation.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/templates/umap/password_change.html` & `umap-project-1.2.5/umap/templates/umap/password_change.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/templatetags/umap_tags.py` & `umap-project-1.2.5/umap/templatetags/umap_tags.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/tests/base.py` & `umap-project-1.2.5/umap/tests/base.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/tests/conftest.py` & `umap-project-1.2.5/umap/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/tests/test_datalayer.py` & `umap-project-1.2.5/umap/tests/test_datalayer.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/tests/test_datalayer_views.py` & `umap-project-1.2.5/umap/tests/test_datalayer_views.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,16 +20,14 @@
         "geojson": '{"type":"FeatureCollection","features":[{"type":"Feature","geometry":{"type":"Polygon","coordinates":[[[-3.1640625,53.014783245859235],[-3.1640625,51.86292391360244],[-0.50537109375,51.385495069223204],[1.16455078125,52.38901106223456],[-0.41748046875,53.91728101547621],[-2.109375,53.85252660044951],[-3.1640625,53.014783245859235]]]},"properties":{"_umap_options":{},"name":"Ho god, sounds like a polygouine"}},{"type":"Feature","geometry":{"type":"LineString","coordinates":[[1.8017578124999998,51.16556659836182],[-0.48339843749999994,49.710272582105695],[-3.1640625,50.0923932109388],[-5.60302734375,51.998410382390325]]},"properties":{"_umap_options":{},"name":"Light line"}},{"type":"Feature","geometry":{"type":"Point","coordinates":[0.63720703125,51.15178610143037]},"properties":{"_umap_options":{},"name":"marker he"}}],"_umap_options":{"displayOnLoad":true,"name":"new name","id":1668,"remoteData":{},"color":"LightSeaGreen","description":"test"}}'  # noqa
     }
 
 
 def test_get(client, settings, datalayer):
     url = reverse('datalayer_view', args=(datalayer.pk, ))
     response = client.get(url)
-    if getattr(settings, 'UMAP_XSENDFILE_HEADER', None):
-        assert response['ETag'] is not None
     assert response['Last-Modified'] is not None
     assert response['Cache-Control'] is not None
     assert 'Content-Encoding' not in response
     j = json.loads(response.content.decode())
     assert '_umap_options' in j
     assert 'features' in j
     assert j['type'] == 'FeatureCollection'
@@ -83,57 +81,47 @@
     url = reverse('datalayer_delete', args=(other_map.pk, datalayer.pk))
     client.login(username=map.owner.username, password='123123')
     response = client.post(url, {}, follow=True)
     assert response.status_code == 403
     assert DataLayer.objects.filter(pk=datalayer.pk).exists()
 
 
-def test_get_gzipped(client, datalayer, settings):
-    url = reverse('datalayer_view', args=(datalayer.pk, ))
-    response = client.get(url, HTTP_ACCEPT_ENCODING='gzip')
-    if getattr(settings, 'UMAP_XSENDFILE_HEADER', None):
-        assert response['ETag'] is not None
-    assert response['Last-Modified'] is not None
-    assert response['Cache-Control'] is not None
-    assert response['Content-Encoding'] == 'gzip'
-
-
-def test_optimistic_concurrency_control_with_good_etag(client, datalayer, map, post_data):  # noqa
-    # Get Etag
+def test_optimistic_concurrency_control_with_good_last_modified(client, datalayer, map, post_data):  # noqa
+    # Get Last-Modified
     url = reverse('datalayer_view', args=(datalayer.pk, ))
     response = client.get(url)
-    etag = response['ETag']
+    last_modified = response['Last-Modified']
     url = reverse('datalayer_update',
                   args=(map.pk, datalayer.pk))
     client.login(username=map.owner.username, password="123123")
     name = 'new name'
     post_data['name'] = 'new name'
-    response = client.post(url, post_data, follow=True, HTTP_IF_MATCH=etag)
+    response = client.post(url, post_data, follow=True, HTTP_IF_UNMODIFIED_SINCE=last_modified)
     assert response.status_code == 200
     modified_datalayer = DataLayer.objects.get(pk=datalayer.pk)
     assert modified_datalayer.name == name
 
 
-def test_optimistic_concurrency_control_with_bad_etag(client, datalayer, map, post_data):  # noqa
+def test_optimistic_concurrency_control_with_bad_last_modified(client, datalayer, map, post_data):  # noqa
     url = reverse('datalayer_update', args=(map.pk, datalayer.pk))
     client.login(username=map.owner.username, password='123123')
     name = 'new name'
     post_data['name'] = name
-    response = client.post(url, post_data, follow=True, HTTP_IF_MATCH='xxx')
+    response = client.post(url, post_data, follow=True, HTTP_IF_UNMODIFIED_SINCE='xxx')
     assert response.status_code == 412
     modified_datalayer = DataLayer.objects.get(pk=datalayer.pk)
     assert modified_datalayer.name != name
 
 
-def test_optimistic_concurrency_control_with_empty_etag(client, datalayer, map, post_data):  # noqa
+def test_optimistic_concurrency_control_with_empty_last_modified(client, datalayer, map, post_data):  # noqa
     url = reverse('datalayer_update', args=(map.pk, datalayer.pk))
     client.login(username=map.owner.username, password='123123')
     name = 'new name'
     post_data['name'] = name
-    response = client.post(url, post_data, follow=True, HTTP_IF_MATCH=None)
+    response = client.post(url, post_data, follow=True, HTTP_IF_UNMODIFIED_SINCE=None)
     assert response.status_code == 200
     modified_datalayer = DataLayer.objects.get(pk=datalayer.pk)
     assert modified_datalayer.name == name
 
 
 def test_versions_should_return_versions(client, datalayer, map, settings):
     root = datalayer.storage_root()
```

### Comparing `umap-project-1.2.4/umap/tests/test_map.py` & `umap-project-1.2.5/umap/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/tests/test_map_views.py` & `umap-project-1.2.5/umap/tests/test_map_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 
 import pytest
 from django.contrib.auth import get_user_model
 from django.urls import reverse
 
+from django.core.signing import Signer
 from umap.models import DataLayer, Map
 
 from .base import login_required
 
 pytestmark = pytest.mark.django_db
 User = get_user_model()
 
@@ -395,14 +396,28 @@
     canonical = reverse('map', kwargs={'pk': anonymap.pk,
                                        'slug': anonymap.slug})
     response = cookieclient.get(url)
     assert response.status_code == 302
     assert response['Location'] == canonical
     key, value = anonymap.signed_cookie_elements
     assert key in cookieclient.cookies
+
+
+@pytest.mark.usefixtures('allow_anonymous')
+def test_sha1_anonymous_edit_url(cookieclient, anonymap):
+    signer = Signer(algorithm='sha1')
+    signature = signer.sign(anonymap.pk)
+    url = reverse('map_anonymous_edit_url', kwargs={'signature': signature})
+    canonical = reverse('map', kwargs={'pk': anonymap.pk,
+                                       'slug': anonymap.slug})
+    response = cookieclient.get(url)
+    assert response.status_code == 302
+    assert response['Location'] == canonical
+    key, value = anonymap.signed_cookie_elements
+    assert key in cookieclient.cookies
 
 
 @pytest.mark.usefixtures('allow_anonymous')
 def test_bad_anonymous_edit_url_should_return_403(cookieclient, anonymap):
     url = anonymap.get_anonymous_edit_url()
     url = reverse(
         'map_anonymous_edit_url',
```

### Comparing `umap-project-1.2.4/umap/tests/test_tilelayer.py` & `umap-project-1.2.5/umap/tests/test_tilelayer.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/tests/test_views.py` & `umap-project-1.2.5/umap/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/urls.py` & `umap-project-1.2.5/umap/urls.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap/utils.py` & `umap-project-1.2.5/umap/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import gzip
+import os
 
 from django.urls import get_resolver
 from django.urls import URLPattern, URLResolver
 
 
 def get_uri_template(urlname, args=None, prefix=""):
     '''
@@ -102,14 +103,16 @@
         for f in func:
             decorate(urls, f)
 
     return urls
 
 
 def gzip_file(from_path, to_path):
+    stat = os.stat(from_path)
     with open(from_path, 'rb') as f_in:
         with gzip.open(to_path, 'wb') as f_out:
             f_out.writelines(f_in)
+    os.utime(to_path, (stat.st_mtime, stat.st_mtime))
 
 
 def is_ajax(request):
     return request.headers.get('x-requested-with') == 'XMLHttpRequest'
```

### Comparing `umap-project-1.2.4/umap/views.py` & `umap-project-1.2.5/umap/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-import hashlib
 import json
+import mimetypes
 import os
 import re
 import socket
+from pathlib import Path
 
-import mimetypes
 from django.conf import settings
 from django.contrib import messages
 from django.contrib.auth import logout as do_logout
 from django.contrib.auth import get_user_model
 from django.contrib.gis.measure import D
 from django.core.paginator import EmptyPage, PageNotAnInteger, Paginator
 from django.core.signing import BadSignature, Signer
 from django.core.validators import URLValidator, ValidationError
 from django.db.models import Q
 from django.http import (HttpResponse, HttpResponseBadRequest,
                          HttpResponseForbidden, HttpResponsePermanentRedirect,
                          HttpResponseRedirect)
 from django.middleware.gzip import re_accepts_gzip
 from django.shortcuts import get_object_or_404
-from django.template.loader import render_to_string
 from django.urls import reverse, reverse_lazy
-from django.utils.encoding import force_bytes, smart_bytes
+from django.utils.encoding import smart_bytes
 from django.utils.http import http_date
 from django.utils.translation import gettext as _
 from django.utils.translation import to_locale
 from django.views.generic import DetailView, TemplateView, View
 from django.views.generic.base import RedirectView
 from django.views.generic.detail import BaseDetailView
 from django.views.generic.edit import CreateView, DeleteView, UpdateView
@@ -176,17 +175,17 @@
     template_name = "umap/search.html"
     list_template_name = "umap/map_list.html"
 
     def get_context_data(self, **kwargs):
         q = self.request.GET.get("q")
         results = []
         if q:
-            where = "to_tsvector(name) @@ plainto_tsquery(%s)"
+            where = "to_tsvector(name) @@ websearch_to_tsquery(%s)"
             if getattr(settings, "UMAP_USE_UNACCENT", False):
-                where = "to_tsvector(unaccent(name)) @@ plainto_tsquery(unaccent(%s))"  # noqa
+                where = "to_tsvector(unaccent(name)) @@ websearch_to_tsquery(unaccent(%s))"  # noqa
             results = Map.objects.filter(share_status=Map.PUBLIC)
             results = results.extra(where=[where], params=[q])
             results = results.order_by("-modified_at")
             results = self.paginate(results)
         kwargs.update({"maps": results, "q": q})
         return kwargs
 
@@ -314,23 +313,14 @@
             url.name for url in urlpatterns + i18n_urls if getattr(url, "name", None)
         ]
     urls = dict(zip(urls, [get_uri_template(url) for url in urls]))
     urls.update(getattr(settings, "UMAP_EXTRA_URLS", {}))
     return urls
 
 
-def render_to_json(templates, context, request):
-    """
-    Generate a JSON HttpResponse with rendered template HTML.
-    """
-    html = render_to_string(templates, context=context, request=request)
-    _json = json.dumps({"html": html})
-    return HttpResponse(_json)
-
-
 def simple_json_response(**kwargs):
     return HttpResponse(json.dumps(kwargs))
 
 
 # ############## #
 #      Map       #
 # ############## #
@@ -652,140 +642,129 @@
     permanent = False
 
     def get(self, request, *args, **kwargs):
         signer = Signer()
         try:
             pk = signer.unsign(self.kwargs["signature"])
         except BadSignature:
-            return HttpResponseForbidden()
-        else:
-            map_inst = get_object_or_404(Map, pk=pk)
-            url = map_inst.get_absolute_url()
-            response = HttpResponseRedirect(url)
-            if not map_inst.owner:
-                key, value = map_inst.signed_cookie_elements
-                response.set_signed_cookie(
-                    key=key, value=value, max_age=ANONYMOUS_COOKIE_MAX_AGE
-                )
-            return response
+            signer = Signer(algorithm='sha1')
+            try:
+                pk = signer.unsign(self.kwargs["signature"])
+            except BadSignature:
+                return HttpResponseForbidden()
+
+        map_inst = get_object_or_404(Map, pk=pk)
+        url = map_inst.get_absolute_url()
+        response = HttpResponseRedirect(url)
+        if not map_inst.owner:
+            key, value = map_inst.signed_cookie_elements
+            response.set_signed_cookie(
+                key=key, value=value, max_age=ANONYMOUS_COOKIE_MAX_AGE
+            )
+        return response
 
 
 # ############## #
 #    DataLayer   #
 # ############## #
 
 
 class GZipMixin(object):
 
     EXT = '.gz'
 
-    def _path(self):
-        return self.object.geojson.path
-
+    @property
     def path(self):
-        """
-        Serve gzip file if client accept it.
-        Generate or update the gzip file if needed.
-        """
-        path = self._path()
-        statobj = os.stat(path)
-        ae = self.request.META.get('HTTP_ACCEPT_ENCODING', '')
-        if re_accepts_gzip.search(ae) and getattr(settings, 'UMAP_GZIP', True):
-            gzip_path = "{path}{ext}".format(path=path, ext=self.EXT)
-            up_to_date = True
-            if not os.path.exists(gzip_path):
-                up_to_date = False
-            else:
-                gzip_statobj = os.stat(gzip_path)
-                if statobj.st_mtime > gzip_statobj.st_mtime:
-                    up_to_date = False
-            if not up_to_date:
-                gzip_file(path, gzip_path)
-            path = gzip_path
-        return path
+        return self.object.geojson.path
 
-    def etag(self):
-        path = self.path()
-        with open(path, mode='rb') as f:
-            return hashlib.md5(f.read()).hexdigest()
+    @property
+    def last_modified(self):
+        stat = os.stat(self.path)
+        return http_date(stat.st_mtime)
 
 
 class DataLayerView(GZipMixin, BaseDetailView):
     model = DataLayer
 
     def render_to_response(self, context, **response_kwargs):
         response = None
-        path = self.path()
+        path = self.path
+        # Generate gzip if needed
+        accepts_gzip = re_accepts_gzip.search(
+            self.request.META.get("HTTP_ACCEPT_ENCODING", "")
+        )
+        if accepts_gzip and settings.UMAP_GZIP:
+            gzip_path = Path(f"{path}{self.EXT}")
+            if not gzip_path.exists():
+                gzip_file(path, gzip_path)
 
         if getattr(settings, 'UMAP_XSENDFILE_HEADER', None):
             response = HttpResponse()
             path = path.replace(settings.MEDIA_ROOT, "/internal")
             response[settings.UMAP_XSENDFILE_HEADER] = path
         else:
-            # TODO IMS
+            # Do not use in production
+            # (no gzip/cache-control/If-Modified-Since/If-None-Match)
             statobj = os.stat(path)
             with open(path, "rb") as f:
                 # Should not be used in production!
-                response = HttpResponse(
-                    f.read(),
-                    content_type="application/json"
-                )
-            response["Last-Modified"] = http_date(statobj.st_mtime)
-            response['ETag'] = '%s' % hashlib.md5(force_bytes(response.content)).hexdigest()  # noqa
-            response['Content-Length'] = len(response.content)
-        if path.endswith(self.EXT):
-            response['Content-Encoding'] = 'gzip'
+                response = HttpResponse(f.read(), content_type="application/geo+json")
+            response["Last-Modified"] = self.last_modified
+            response["Content-Length"] = statobj.st_size
         return response
 
 
 class DataLayerVersion(DataLayerView):
-    def _path(self):
+    @property
+    def path(self):
         return "{root}/{path}".format(
             root=settings.MEDIA_ROOT,
             path=self.object.get_version_path(self.kwargs["name"]),
         )
 
 
 class DataLayerCreate(FormLessEditMixin, GZipMixin, CreateView):
     model = DataLayer
     form_class = DataLayerForm
 
     def form_valid(self, form):
         form.instance.map = self.kwargs['map_inst']
         self.object = form.save()
+        # Simple response with only metadatas (including new id)
         response = simple_json_response(**self.object.metadata)
-        response['ETag'] = self.etag()
+        response["Last-Modified"] = self.last_modified
         return response
 
 
 class DataLayerUpdate(FormLessEditMixin, GZipMixin, UpdateView):
     model = DataLayer
     form_class = DataLayerForm
 
     def form_valid(self, form):
         self.object = form.save()
+        # Simple response with only metadatas (client should not reload all data
+        # on save)
         response = simple_json_response(**self.object.metadata)
-        response['ETag'] = self.etag()
+        response["Last-Modified"] = self.last_modified
         return response
 
-    def if_match(self):
+    def is_unmodified(self):
         """Optimistic concurrency control."""
-        match = True
-        if_match = self.request.META.get('HTTP_IF_MATCH')
-        if if_match:
-            etag = self.etag()
-            if etag != if_match:
-                match = False
-        return match
+        modified = True
+        if_unmodified = self.request.META.get("HTTP_IF_UNMODIFIED_SINCE")
+        if if_unmodified:
+            if self.last_modified != if_unmodified:
+                modified = False
+        return modified
 
     def post(self, request, *args, **kwargs):
         self.object = self.get_object()
         if self.object.map != self.kwargs["map_inst"]:
             return HttpResponseForbidden()
-        if not self.if_match():
+        if not self.is_unmodified():
             return HttpResponse(status=412)
         return super(DataLayerUpdate, self).post(request, *args, **kwargs)
 
 
 class DataLayerDelete(DeleteView):
     model = DataLayer
```

### Comparing `umap-project-1.2.4/umap/wsgi.py` & `umap-project-1.2.5/umap/wsgi.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.2.4/umap_project.egg-info/PKG-INFO` & `umap-project-1.2.5/umap_project.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: umap-project
-Version: 1.2.4
+Version: 1.2.5
 Summary: Create maps with OpenStreetMap layers in a minute and embed them in your site.
-Home-page: UNKNOWN
 Author: Yohan Boniface
-License: UNKNOWN
 Keywords: django leaflet geodjango openstreetmap map
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.4
@@ -37,9 +34,7 @@
 *Because we think that the more OSM will be used, the more OSM will be improved.*
 It uses [django-leaflet-storage](https://github.com/umap-project/django-leaflet-storage) and [Leaflet.Storage](https://github.com/umap-project/Leaflet.Storage),  built on top of Django and Leaflet.
 
 
 ## Installation and configuration
 
 See [developer documentation](https://umap-project.readthedocs.io/en/latest/install/).
-
-
```

### Comparing `umap-project-1.2.4/umap_project.egg-info/SOURCES.txt` & `umap-project-1.2.5/umap_project.egg-info/SOURCES.txt`

 * *Files identical despite different names*


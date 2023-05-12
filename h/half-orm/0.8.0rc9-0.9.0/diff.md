# Comparing `tmp/half_orm-0.8.0rc9.tar.gz` & `tmp/half_orm-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "half_orm-0.8.0rc9.tar", last modified: Mon Mar  6 08:19:21 2023, max compression
+gzip compressed data, was "half_orm-0.9.0.tar", last modified: Fri May 12 08:38:28 2023, max compression
```

## Comparing `half_orm-0.8.0rc9.tar` & `half_orm-0.9.0.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-03-06 08:19:21.913335 half_orm-0.8.0rc9/
--rw-r--r--   0 joel      (1000) joel      (1000)       97 2023-02-02 08:59:25.000000 half_orm-0.8.0rc9/AUTHORS
--rw-r--r--   0 joel      (1000) joel      (1000)      699 2023-02-02 08:59:25.000000 half_orm-0.8.0rc9/LICENSE
--rw-r--r--   0 joel      (1000) joel      (1000)    27243 2023-03-06 08:19:21.913335 half_orm-0.8.0rc9/PKG-INFO
--rw-r--r--   0 joel      (1000) joel      (1000)    26299 2023-03-06 08:08:09.000000 half_orm-0.8.0rc9/README.md
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-03-06 08:19:21.897335 half_orm-0.8.0rc9/half_orm/
--rw-r--r--   0 joel      (1000) joel      (1000)      172 2023-02-02 08:59:25.000000 half_orm-0.8.0rc9/half_orm/__init__.py
--rw-r--r--   0 joel      (1000) joel      (1000)     5929 2023-03-02 13:06:39.000000 half_orm-0.8.0rc9/half_orm/field.py
--rw-r--r--   0 joel      (1000) joel      (1000)       70 2023-02-02 08:59:25.000000 half_orm-0.8.0rc9/half_orm/field_errors.py
--rw-r--r--   0 joel      (1000) joel      (1000)     5794 2023-03-02 13:12:11.000000 half_orm-0.8.0rc9/half_orm/fkey.py
--rw-r--r--   0 joel      (1000) joel      (1000)     3673 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/hotest.py
--rwxr-xr-x   0 joel      (1000) joel      (1000)    18902 2023-03-03 09:24:59.000000 half_orm-0.8.0rc9/half_orm/model.py
--rw-r--r--   0 joel      (1000) joel      (1000)     1370 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/model_errors.py
--rw-r--r--   0 joel      (1000) joel      (1000)      405 2023-02-28 09:49:19.000000 half_orm-0.8.0rc9/half_orm/null.py
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-03-06 08:19:21.905335 half_orm-0.8.0rc9/half_orm/packager/
--rw-r--r--   0 joel      (1000) joel      (1000)        0 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/__init__.py
--rw-r--r--   0 joel      (1000) joel      (1000)     3780 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/changelog.py
--rw-r--r--   0 joel      (1000) joel      (1000)     4472 2023-03-02 13:10:29.000000 half_orm-0.8.0rc9/half_orm/packager/database.py
--rw-r--r--   0 joel      (1000) joel      (1000)     4545 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/db_conn.py
--rw-r--r--   0 joel      (1000) joel      (1000)     7522 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/hgit.py
--rwxr-xr-x   0 joel      (1000) joel      (1000)     5335 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/hop.py
--rw-r--r--   0 joel      (1000) joel      (1000)     1274 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/manifest.py
--rwxr-xr-x   0 joel      (1000) joel      (1000)     8882 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/modules.py
--rwxr-xr-x   0 joel      (1000) joel      (1000)    13413 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/patch.py
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-03-06 08:19:21.905335 half_orm-0.8.0rc9/half_orm/packager/patches/
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-03-06 08:19:21.885335 half_orm-0.8.0rc9/half_orm/packager/patches/0/
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-03-06 08:19:21.885335 half_orm-0.8.0rc9/half_orm/packager/patches/0/1/
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-03-06 08:19:21.905335 half_orm-0.8.0rc9/half_orm/packager/patches/0/1/0/
--rw-r--r--   0 joel      (1000) joel      (1000)     1076 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/patches/0/1/0/00_half_orm_meta.database.sql
--rw-r--r--   0 joel      (1000) joel      (1000)      183 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/patches/0/1/0/01_alter_half_orm_meta.hop_release.sql
--rw-r--r--   0 joel      (1000) joel      (1000)       22 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/patches/log
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-03-06 08:19:21.905335 half_orm-0.8.0rc9/half_orm/packager/patches/sql/
--rw-r--r--   0 joel      (1000) joel      (1000)     4197 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/patches/sql/half_orm_meta.sql
--rw-r--r--   0 joel      (1000) joel      (1000)     8297 2023-03-02 12:49:19.000000 half_orm-0.8.0rc9/half_orm/packager/repo.py
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-03-06 08:19:21.913335 half_orm-0.8.0rc9/half_orm/packager/templates/
--rw-r--r--   0 joel      (1000) joel      (1000)       86 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/templates/.gitignore
--rw-r--r--   0 joel      (1000) joel      (1000)       25 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/templates/MANIFEST.in
--rw-r--r--   0 joel      (1000) joel      (1000)      218 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/templates/Pipfile
--rw-r--r--   0 joel      (1000) joel      (1000)      924 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/templates/README
--rw-r--r--   0 joel      (1000) joel      (1000)      367 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/templates/base_test
--rw-r--r--   0 joel      (1000) joel      (1000)      437 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/templates/db_connector.py
--rw-r--r--   0 joel      (1000) joel      (1000)      246 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/templates/module_template_1
--rw-r--r--   0 joel      (1000) joel      (1000)      120 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/templates/module_template_2
--rw-r--r--   0 joel      (1000) joel      (1000)       69 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/templates/module_template_3
--rw-r--r--   0 joel      (1000) joel      (1000)      460 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/templates/relation_test
--rw-r--r--   0 joel      (1000) joel      (1000)     2070 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/templates/setup.py
--rw-r--r--   0 joel      (1000) joel      (1000)      490 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/templates/warning
--rw-r--r--   0 joel      (1000) joel      (1000)     1733 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/utils.py
--rw-r--r--   0 joel      (1000) joel      (1000)        8 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/packager/version.txt
--rw-r--r--   0 joel      (1000) joel      (1000)    12382 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/pg_meta.py
--rw-r--r--   0 joel      (1000) joel      (1000)    40090 2023-03-02 13:22:03.000000 half_orm-0.8.0rc9/half_orm/relation.py
--rw-r--r--   0 joel      (1000) joel      (1000)     1521 2023-02-28 10:33:54.000000 half_orm-0.8.0rc9/half_orm/relation_errors.py
--rw-r--r--   0 joel      (1000) joel      (1000)     2276 2023-02-28 09:49:19.000000 half_orm-0.8.0rc9/half_orm/transaction.py
--rw-r--r--   0 joel      (1000) joel      (1000)        9 2023-03-06 08:08:04.000000 half_orm-0.8.0rc9/half_orm/version.txt
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-03-06 08:19:21.897335 half_orm-0.8.0rc9/half_orm.egg-info/
--rw-r--r--   0 joel      (1000) joel      (1000)    27243 2023-03-06 08:19:21.000000 half_orm-0.8.0rc9/half_orm.egg-info/PKG-INFO
--rw-r--r--   0 joel      (1000) joel      (1000)     1553 2023-03-06 08:19:21.000000 half_orm-0.8.0rc9/half_orm.egg-info/SOURCES.txt
--rw-r--r--   0 joel      (1000) joel      (1000)        1 2023-03-06 08:19:21.000000 half_orm-0.8.0rc9/half_orm.egg-info/dependency_links.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       51 2023-03-06 08:19:21.000000 half_orm-0.8.0rc9/half_orm.egg-info/entry_points.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       46 2023-03-06 08:19:21.000000 half_orm-0.8.0rc9/half_orm.egg-info/requires.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       27 2023-03-06 08:19:21.000000 half_orm-0.8.0rc9/half_orm.egg-info/top_level.txt
--rw-r--r--   0 joel      (1000) joel      (1000)      100 2023-01-04 14:18:53.000000 half_orm-0.8.0rc9/pyproject.toml
--rw-r--r--   0 joel      (1000) joel      (1000)       38 2023-03-06 08:19:21.913335 half_orm-0.8.0rc9/setup.cfg
--rw-r--r--   0 joel      (1000) joel      (1000)     2502 2023-03-06 08:18:37.000000 half_orm-0.8.0rc9/setup.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-12 08:38:28.598108 half_orm-0.9.0/
+-rw-r--r--   0 joel      (1000) joel      (1000)       97 2023-02-02 08:59:25.000000 half_orm-0.9.0/AUTHORS
+-rw-r--r--   0 joel      (1000) joel      (1000)      699 2023-02-02 08:59:25.000000 half_orm-0.9.0/LICENSE
+-rw-r--r--   0 joel      (1000) joel      (1000)    27298 2023-05-12 08:38:28.598108 half_orm-0.9.0/PKG-INFO
+-rw-r--r--   0 joel      (1000) joel      (1000)    26357 2023-05-12 08:37:33.000000 half_orm-0.9.0/README.md
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-12 08:38:28.582109 half_orm-0.9.0/half_orm/
+-rw-r--r--   0 joel      (1000) joel      (1000)      172 2023-02-02 08:59:25.000000 half_orm-0.9.0/half_orm/__init__.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     5495 2023-05-12 08:02:28.000000 half_orm-0.9.0/half_orm/field.py
+-rw-r--r--   0 joel      (1000) joel      (1000)       70 2023-02-02 08:59:25.000000 half_orm-0.9.0/half_orm/field_errors.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     5558 2023-05-12 08:04:47.000000 half_orm-0.9.0/half_orm/fkey.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     3513 2023-05-12 08:00:34.000000 half_orm-0.9.0/half_orm/hotest.py
+-rwxr-xr-x   0 joel      (1000) joel      (1000)    14440 2023-04-21 09:03:14.000000 half_orm-0.9.0/half_orm/model.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     1143 2023-03-21 09:29:02.000000 half_orm-0.9.0/half_orm/model_errors.py
+-rw-r--r--   0 joel      (1000) joel      (1000)      405 2023-03-18 07:38:44.000000 half_orm-0.9.0/half_orm/null.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-12 08:38:28.590108 half_orm-0.9.0/half_orm/packager/
+-rw-r--r--   0 joel      (1000) joel      (1000)        0 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/__init__.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     3780 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/changelog.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     4470 2023-05-12 08:15:08.000000 half_orm-0.9.0/half_orm/packager/database.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     4685 2023-04-21 09:03:14.000000 half_orm-0.9.0/half_orm/packager/db_conn.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     7522 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/hgit.py
+-rwxr-xr-x   0 joel      (1000) joel      (1000)     5335 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/hop.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     1274 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/manifest.py
+-rwxr-xr-x   0 joel      (1000) joel      (1000)     8882 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/modules.py
+-rwxr-xr-x   0 joel      (1000) joel      (1000)    13522 2023-03-17 13:09:31.000000 half_orm-0.9.0/half_orm/packager/patch.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-12 08:38:28.590108 half_orm-0.9.0/half_orm/packager/patches/
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-12 08:38:28.574109 half_orm-0.9.0/half_orm/packager/patches/0/
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-12 08:38:28.574109 half_orm-0.9.0/half_orm/packager/patches/0/1/
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-12 08:38:28.594108 half_orm-0.9.0/half_orm/packager/patches/0/1/0/
+-rw-r--r--   0 joel      (1000) joel      (1000)     1076 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/patches/0/1/0/00_half_orm_meta.database.sql
+-rw-r--r--   0 joel      (1000) joel      (1000)      183 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/patches/0/1/0/01_alter_half_orm_meta.hop_release.sql
+-rw-r--r--   0 joel      (1000) joel      (1000)       22 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/patches/log
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-12 08:38:28.594108 half_orm-0.9.0/half_orm/packager/patches/sql/
+-rw-r--r--   0 joel      (1000) joel      (1000)     4197 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/patches/sql/half_orm_meta.sql
+-rw-r--r--   0 joel      (1000) joel      (1000)     8297 2023-04-21 09:03:14.000000 half_orm-0.9.0/half_orm/packager/repo.py
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-12 08:38:28.598108 half_orm-0.9.0/half_orm/packager/templates/
+-rw-r--r--   0 joel      (1000) joel      (1000)       86 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/templates/.gitignore
+-rw-r--r--   0 joel      (1000) joel      (1000)       25 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/templates/MANIFEST.in
+-rw-r--r--   0 joel      (1000) joel      (1000)      218 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/templates/Pipfile
+-rw-r--r--   0 joel      (1000) joel      (1000)      924 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/templates/README
+-rw-r--r--   0 joel      (1000) joel      (1000)      367 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/templates/base_test
+-rw-r--r--   0 joel      (1000) joel      (1000)      437 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/templates/db_connector.py
+-rw-r--r--   0 joel      (1000) joel      (1000)      246 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/templates/module_template_1
+-rw-r--r--   0 joel      (1000) joel      (1000)      120 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/templates/module_template_2
+-rw-r--r--   0 joel      (1000) joel      (1000)       69 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/templates/module_template_3
+-rw-r--r--   0 joel      (1000) joel      (1000)      460 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/templates/relation_test
+-rw-r--r--   0 joel      (1000) joel      (1000)     2070 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/templates/setup.py
+-rw-r--r--   0 joel      (1000) joel      (1000)      490 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/templates/warning
+-rw-r--r--   0 joel      (1000) joel      (1000)     2099 2023-04-20 09:30:05.000000 half_orm-0.9.0/half_orm/packager/utils.py
+-rw-r--r--   0 joel      (1000) joel      (1000)        8 2023-02-28 10:33:54.000000 half_orm-0.9.0/half_orm/packager/version.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)    17049 2023-04-20 09:30:05.000000 half_orm-0.9.0/half_orm/pg_meta.py
+-rw-r--r--   0 joel      (1000) joel      (1000)    39274 2023-05-12 08:04:42.000000 half_orm-0.9.0/half_orm/relation.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     1520 2023-05-12 08:00:34.000000 half_orm-0.9.0/half_orm/relation_errors.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     3876 2023-05-12 08:00:07.000000 half_orm-0.9.0/half_orm/relation_factory.py
+-rw-r--r--   0 joel      (1000) joel      (1000)     2743 2023-03-21 09:29:02.000000 half_orm-0.9.0/half_orm/transaction.py
+-rw-r--r--   0 joel      (1000) joel      (1000)        6 2023-05-12 08:37:35.000000 half_orm-0.9.0/half_orm/version.txt
+drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-12 08:38:28.586109 half_orm-0.9.0/half_orm.egg-info/
+-rw-r--r--   0 joel      (1000) joel      (1000)    27298 2023-05-12 08:38:28.000000 half_orm-0.9.0/half_orm.egg-info/PKG-INFO
+-rw-r--r--   0 joel      (1000) joel      (1000)     1582 2023-05-12 08:38:28.000000 half_orm-0.9.0/half_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)        1 2023-05-12 08:38:28.000000 half_orm-0.9.0/half_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       51 2023-05-12 08:38:28.000000 half_orm-0.9.0/half_orm.egg-info/entry_points.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       46 2023-05-12 08:38:28.000000 half_orm-0.9.0/half_orm.egg-info/requires.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)       27 2023-05-12 08:38:28.000000 half_orm-0.9.0/half_orm.egg-info/top_level.txt
+-rw-r--r--   0 joel      (1000) joel      (1000)      100 2023-01-04 14:18:53.000000 half_orm-0.9.0/pyproject.toml
+-rw-r--r--   0 joel      (1000) joel      (1000)       38 2023-05-12 08:38:28.598108 half_orm-0.9.0/setup.cfg
+-rw-r--r--   0 joel      (1000) joel      (1000)     2502 2023-03-06 08:18:37.000000 half_orm-0.9.0/setup.py
```

### Comparing `half_orm-0.8.0rc9/LICENSE` & `half_orm-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc9/PKG-INFO` & `half_orm-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: half_orm
-Version: 0.8.0rc9
+Version: 0.9.0
 Summary: A simple PostgreSQL to Python mapper.
 Home-page: https://github.com/collorg/halfORM
 Author: Joël Maïzi
 Author-email: joel.maizi@collorg.org
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -18,24 +18,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
-# A simple PostgreSQL to Python mapper [0.8.0rc8]
-
+# A simple PostgreSQL to Python mapper [0.9.0] and its packager [0.1.0a2]
 
 ![PyPI version](https://img.shields.io/pypi/v/half_orm)
 ![Python versions](https://img.shields.io/pypi/pyversions/half_orm)
-![CI badge](https://github.com/collorg/halfORM/actions/workflows/python-package.yml/badge.svg) 
+![CI badge](https://github.com/collorg/halfORM/actions/workflows/python-package.yml/badge.svg)
+![Coveralls](https://img.shields.io/coverallsCoverage/github/collorg/halfORM)
 ![PyPI downloads](https://img.shields.io/pypi/dm/half_orm)
 ![Contributors](https://img.shields.io/github/contributors/collorg/halform)
 
-You have a PostgreSQL database at hand and you want to interact with it in Python (&ge; 3.6); `half_orm` maps your tables and views to Python classes that you can easily use to manipulate your data.
+You have a PostgreSQL database at hand and you want to interact with it in Python (&ge; 3.6); `half_orm` maps your tables and views to Python classes that you can easily use to manipulate your data. If you want to build or patch a model, you might be interested in the [`half_orm packager`](#next-hop-the-gitops-half_orm-packager-wipalpha).
 
 The 'half' part of `half_orm` name indicates that it only deals with the data manipulation language ([DML](https://www.postgresql.org/docs/current/dml.html)) part of SQL. Basically the [`INSERT`](https://www.postgresql.org/docs/current/sql-insert.html), [`SELECT`](https://www.postgresql.org/docs/current/sql-select.html), [`UPDATE`](https://www.postgresql.org/docs/current/sql-update.html) and [`DELETE`](https://www.postgresql.org/docs/current/sql-delete.html) commands. This is what makes `half_orm` so easy to learn an use.
 
 Here is what coding with `half_orm` looks like :
 
 ```python
 from half_orm.model import Model
@@ -57,44 +57,40 @@
 class Person(halftest.get_relation_class('actor.person')):
     Fkeys = {
         'posts_rfk': '_reverse_fkey_halftest_blog_post_author_first_name_author_last_name_author_birth_date',
         'comments_rfk': '_reverse_fkey_halftest_blog_comment_author_id'
     }
     @singleton # This ensures that the author of the post is well defined.
     def add_post(self, title: str=None, content: str=None) -> dict:
-        return self.posts_rfk(title=title, content=content)._ho_insert()
+        return self.posts_rfk(title=title, content=content).ho_insert()
     @singleton
     def add_comment(self, post: Post=None, content: str=None) -> dict:
-        return self.comments_rfk(content=content, post_id=post.id.value)._ho_insert()
+        return self.comments_rfk(content=content, post_id=post.id.value).ho_insert()
 
 def main():
     gaston = Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28')
-    gaston._ho_delete()
-    if gaston._ho_is_empty(): # gaston defines a subset of the actor.person table.
-        gaston._ho_insert()
+    gaston.ho_delete()
+    if gaston.ho_is_empty(): # gaston defines a subset of the actor.person table.
+        gaston.ho_insert()
     post = Post(**gaston.add_post(title='Easy', content='halfORM is fun!'))
     gaston.add_comment(content='This is a comment on the newly created post.', post=post)
     print(list(post.comments_rfk())) # The relational objects are iterators
-    post._ho_update(title='Super easy')
-    gaston._ho_delete()
+    post.ho_update(title='Super easy')
+    gaston.ho_delete()
 ```
 
 
 # Tutorial: Learn `half_orm` in half an hour
 
 
 
 ## Install `half_orm`
 
 run `pip install half_orm` in a virtual environment.
 
-## Install `half_orm` pre-release
-
-`pip install half_orm==0.8.0rc9`
-
 ### Set your HALFORM_CONF_DIR
 
 Create a directory to store your connection files and set the shell variable `HALFORM_CONF_DIR`
 (by default, `half_orm` looks in the /etc/half_orm directory):
  
 ```sh
 % mkdir ~/.half_orm
@@ -280,60 +276,60 @@
 assert len(nobody) == 0 # last_name is part of the PK
 ```
 
 ## Set operators
 
 You can use the set operators to set more complex constraints on your relations:
 - `&`, `|`, `^` and `-` for `and`, `or`, `xor` and `not`.
-Take a look at [the algebra test file](https://github.com/collorg/halfORM/blob/master/test/relation/algebra_test.py).
+Take a look at [the algebra test file](https://github.com/collorg/halfORM/blob/main/test/relation/algebra_test.py).
 - you can also use the `==`, `!=` and `in` operators to compare two sets.
 
 ```python
 my_selection = Person(last_name=('ilike', '_a%')) | Person(first_name=('like', 'A%'))
 ```
 
 `my_selection` represents the set of people whose second letter of the name is in `['a', 'A']` or whose first letter of the first name is an `A`.
 
 
-# DML. The `_ho_insert`, `_ho_select`, `_ho_update`, `_ho_delete` methods.
+# DML. The `ho_insert`, `ho_select`, `ho_update`, `ho_delete` methods.
 
 These methods trigger their corresponding SQL querie on the database. 
 For debugging purposes, you can print the SQL query built 
-by half_orm when the DML method is invoked using the _ho_mogrify() method.
+by half_orm when the DML method is invoked using the ho_mogrify() method.
 
 ```py
-people._ho_mogrify()
-people._ho_select()
+people.ho_mogrify()
+people.ho_select()
 ```
 
-## _ho_insert
-To insert a tuple in the relation, use the `_ho_insert` method as shown below:
+## ho_insert
+To insert a tuple in the relation, use the `ho_insert` method as shown below:
 ```python
-Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28')._ho_insert()
+Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28').ho_insert()
 ```
 
-By default, `_ho_insert` returns the inserted row as a dict:
+By default, `ho_insert` returns the inserted row as a dict:
 
 ```python
 lagaffe = Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28')
-lagaffe_id = lagaffe._ho_insert()['id']
+lagaffe_id = lagaffe.ho_insert()['id']
 ```
 
-You can trigger a transaction for any combination of insert, modify or delete operations using the `Relation._ho_transaction` decorator.
+You can trigger a transaction for any combination of insert, modify or delete operations using the `Relation.ho_transaction` decorator.
 
 ```py
 class Person(halftest.get_relation_class('actor.person')):
     # [...]
 
     def insert_many(self, *data):
         """Insert serveral people in a single transaction."""
-        @self._ho_transaction
+        @self.ho_transaction
         def insert(self, *data):
             for d_pers in data:
-                self(**d_pers)._ho_insert()
+                self(**d_pers).ho_insert()
         insert(self, *data)
 
 ```
 
 ```python
 people = Person()
 people.insert_many(*[
@@ -346,68 +342,68 @@
 ```
 
 **Note**: half_orm works in autocommit mode by default. Without a transaction, any missing data
 would be inserted.
 
 ### Returned values
 
-By default `_ho_insert` returns all the inserted values as a dictionary. You can specify the columns
-you want to get by passing their names as argurments to `_ho_insert`.
+By default `ho_insert` returns all the inserted values as a dictionary. You can specify the columns
+you want to get by passing their names as argurments to `ho_insert`.
 
-## _ho_select
-The `_ho_select` method is a generator. It returns all the data of the relation that matches the constraint defined on the Relation object.
+## ho_select
+The `ho_select` method is a generator. It returns all the data of the relation that matches the constraint defined on the Relation object.
 The data is returned in a list of `dict`s.
 
 ```python
 >>> people = Person()
->>> print(list(people._ho_select()))
+>>> print(list(people.ho_select()))
 [{'id': 6753, 'first_name': 'Gaston', 'last_name': 'Lagaffe', 'birth_date': datetime.date(1957, 2, 28)}, {'id': 6754, 'first_name': 'Bibi', 'last_name': 'Fricotin', 'birth_date': datetime.date(1924, 10, 5)}, {'id': 6755, 'first_name': 'Corto', 'last_name': 'Maltese', 'birth_date': datetime.date(1975, 1, 7)}, {'id': 6756, 'first_name': 'Achile', 'last_name': 'Talon', 'birth_date': datetime.date(1963, 11, 7)}, {'id': 6757, 'first_name': 'Gil', 'last_name': 'Jourdan', 'birth_date': datetime.date(1956, 9, 20)}]
 >>>
 ```
 
 You can set a limit or an offset:
 ```python
->>> people._ho_offset(1)._ho_limit(2)
->>> print(list(people)) # Relation objects are iterators. so _ho_select is optional
+>>> people.ho_offset(1).ho_limit(2)
+>>> print(list(people)) # Relation objects are iterators. so ho_select is optional
 [{'id': 6754, 'first_name': 'Bibi', 'last_name': 'Fricotin', 'birth_date': datetime.date(1924, 10, 5)}, {'id': 6755, 'first_name': 'Corto', 'last_name': 'Maltese', 'birth_date': datetime.date(1975, 1, 7)}]
 ```
 
-You can also get a subset of the attributes by passing a list of columns names to `_ho_select`:
+You can also get a subset of the attributes by passing a list of columns names to `ho_select`:
 
 ```python
->>> print(list(people._ho_select('last_name')))
+>>> print(list(people.ho_select('last_name')))
 [{'last_name': 'Lagaffe'}, {'last_name': 'Fricotin'}]
 ```
 
 **Note**: The offset and limit still apply.
 
-### Select one: the `_ho_get` method
+### Select one: the `ho_get` method
 
-The `_ho_get` method returns an Relation object whose fields are populated with the values from the corresponding row in the database.
-It raises an [ExpectedOneError](https://github.com/collorg/halfORM/blob/master/half_orm/relation_errors.py)
+The `ho_get` method returns an Relation object whose fields are populated with the values from the corresponding row in the database.
+It raises an [ExpectedOneError](https://github.com/collorg/halfORM/blob/main/half_orm/relation_errors.py)
 Exception if 0 or more than 1 rows match the intention. The returned object is a singleton (see below).
 
 ```py
-gaston = Person(last_name='Lagaffe')._ho_get()
+gaston = Person(last_name='Lagaffe').ho_get()
 ```
 
 is equivalent to
 
 ```py
 lagaffe = Person(last_name='Lagaffe')
-if lagaffe._ho_is_empty() or len(lagaffe) > 1:
+if lagaffe.ho_is_empty() or len(lagaffe) > 1:
     raise ExcpetedOneError
-gaston = Person(**next(lagaffe._ho_select()))
+gaston = Person(**next(lagaffe.ho_select()))
 gaston._ho_is_singleton = True
 ```
 
-You could use `_ho_get` to retreive the `id` of the row:
+You could use `ho_get` to retreive the `id` of the row:
 
 ```py
-gaston_id = Person(last_name='Lagaffe')._ho_get('id').id.value
+gaston_id = Person(last_name='Lagaffe').ho_get('id').id.value
 ```
 
 ### Is it a set? Is it an element of the set?
 
 Let's go back to our definition of the class `Person`. We would like to write a property that
 returns the full name of **a** person. 
 
@@ -456,107 +452,107 @@
     # [...]
     @singleton
     def do_something_else(self):
         "Needs self to be a singleton"
         ...
 
     def do_something(self):
-        for elt in self._ho_select():
+        for elt in self.ho_select():
             pers = Person(**elt)
             pers._ho_is_singleton = True # You must be pretty sure of what you're doing here. See the warning and the explanation.
             pers.do_something_else() # Warning! do_something_else won't check that pers is indeed a singleton
 ```
 
 **Warning!** By setting `_ho_is_singleton` value to `True`, you disable the check that `@singleton` would have made before executing `do_something_else`. 
 This example works for two reasons:
 
-1. `_ho_select` is called without argument ensuring that all columns are retreived from the database.
-Note: Calling `_ho_select` with columns corresponding to the primary key as arguments would also have worked;
+1. `ho_select` is called without argument ensuring that all columns are retreived from the database.
+Note: Calling `ho_select` with columns corresponding to the primary key as arguments would also have worked;
 2. The table `actor.person` has a primary key which makes it a set (ie. each element returned by select is
 indeed a singleton).
 
-## _ho_update
+## ho_update
 
 To update a subset, you first define the subset an then invoque the `ho_udpate`
 method with the new values passed as argument.
 
 ```py
 gaston = Person(first_name='Gaston')
-gaston._ho_update(birth_date='1970-01-01')
+gaston.ho_update(birth_date='1970-01-01')
 ```
 
 Let's look at how we could turn the last name into capital letters for a subset of people:
 
 ```python
 class Person(halftest.get_relation_class('actor.person')):
     # [...]
 
     def upper_last_name(self):
         "tranform last name to upper case."
-        @self._ho_transaction
+        @self.ho_transaction
         def update(self):
-            for d_pers in self._ho_select('id', 'last_name'):
+            for d_pers in self.ho_select('id', 'last_name'):
                 pers = Person(**d_pers)
-                pers._ho_update(last_name=d_pers['last_name'].upper())
+                pers.ho_update(last_name=d_pers['last_name'].upper())
         update(self)
 ```
 
-Again, we insure the atomicity of the transaction using the `Relation._ho_transaction` decorator.
+Again, we insure the atomicity of the transaction using the `Relation.ho_transaction` decorator.
 
 ```
 >>> a_pers = Person(last_name=('ilike', '_a%'))
->>> print([elt.last_name for elt in list(a_pers._ho_select())])
+>>> print([elt.last_name for elt in list(a_pers.ho_select())])
 >>> a_pers = Person(last_name = ('ilike', '_a%'))
->>> print([elt['last_name'] for elt in a_pers._ho_select('last_name')])
+>>> print([elt['last_name'] for elt in a_pers.ho_select('last_name')])
 ['Lagaffe', 'Maltese', 'Talon']
 >>> a_pers.upper_last_name()
->>> print([elt['last_name'] for elt in a_pers._ho_select('last_name')])
+>>> print([elt['last_name'] for elt in a_pers.ho_select('last_name')])
 ['LAGAFFE', 'MALTESE', 'TALON']
 ```
 
 ### Returning values
 
-To return the updated values, you can add to `_ho_update` the column names you want to get, or `*` if you want to get all the columns.
+To return the updated values, you can add to `ho_update` the column names you want to get, or `*` if you want to get all the columns.
 
 ```python
->>> gaston._ho_update('*', birth_date='1970-01-01')
+>>> gaston.ho_update('*', birth_date='1970-01-01')
 ```
 
 ### Update all data in a table
 
 If you want to update all the data in a relation, you must set the argument `update_all` to `True`. A `RuntimeError` is raised otherwise.
 
 ```py
-Person()._ho_update(birth_date='1970-01-01', update_all=True)
+Person().ho_update(birth_date='1970-01-01', update_all=True)
 ```
 
-## _ho_delete
+## ho_delete
 
-The `_ho_delete` method allows you to remove a set of elements from a table:
+The `ho_delete` method allows you to remove a set of elements from a table:
 
 ```py
 gaston = Person(first_name='Gaston')
-gaston._ho_delete()
+gaston.ho_delete()
 ```
 
 To remove every tuples from a table, you must set the argument `delete_all` to `True`. A `RuntimeError` is raised otherwise.
 
 ```python
-Person()._ho_delete(delete_all=True)
-if not Person()._ho_is_empty():
+Person().ho_delete(delete_all=True)
+if not Person().ho_is_empty():
     print('Weird! You should check your "on delete cascade".')
 ```
 Well, there is not much left after this in the `actor.person` table.
 
 ### Returning values
 
-As for `_ho_update`, to return the deleted values, you can add to `_ho_delete` the column names you want to get, or `*` if you want to get all the columns.
+As for `ho_update`, to return the deleted values, you can add to `ho_delete` the column names you want to get, or `*` if you want to get all the columns.
 
 ```python
->>> gaston._ho_delete('first_name', 'last_name', 'birth_date')
+>>> gaston.ho_delete('first_name', 'last_name', 'birth_date')
 ```
 
 # Working with foreign keys [WIP]
 
 > This is a work in progress
 
 A relational object integrates all the material necessary to process its foreign keys and the
@@ -653,40 +649,40 @@
 The Fkey class has the `set` method which allows you to constrain a foreign key with a Relation object.
 To get the comments made by Gaston, we simply constraint the `author_fk` Fkey to reference the entry corresponding to Gaston in the actor.person table. To do so, we use the `Fkey.set()` method:
 
 ```python
 gaston = Person(first_name='Gaston')
 gaston_comments = Comment()
 gaston_comments.author_fk.set(gaston)
-print(list(gaston_comments._ho_select())
+print(list(gaston_comments.ho_select())
 ```
 ## Chaining foreign keys
 
 **Important note**: Foreign key chaining will only work if the modules corresponding to the tables are ordered
 according to the names of the tables in the package. See the `hop` command.
 
 You can easily chain foreign keys. For example, if you want to get all the comments made by Gaston
 on his own posts:
 
 ```py
 gaston = {'last_name':'Lagaffe', 'first_name':'Gaston', 'birth_date':'1957-02-28'}
-gaston_id = Person(**gaston)._ho_get('id').id.value # we ensure that Gaston is a singleton
+gaston_id = Person(**gaston).ho_get('id').id.value # we ensure that Gaston is a singleton
 list(gaston
     .post_rfk(**gaston)
     .comment_rfk(author_id=gaston_id))
 ```
 
 **Note**: the `blog.post` table declares a foreign key on `actor.person(first_name, last_name, birth_date)` 
 while the `blog.comment` table declares a foreign key on `actor.person(id)`.
 
-## The *`_ho_join`* method
+## The *`ho_join`* method
 
-The *`_ho_join`* method allows you to integrate the data associated with a Relation object into the result obtained by the *`select`* method by using foreign keys of the object or by referencing the object.
+The *`ho_join`* method allows you to integrate the data associated with a Relation object into the result obtained by the *`select`* method by using foreign keys of the object or by referencing the object.
 
-Unlike the *`select`* method (which is a generator), the *`_ho_join`* method returns a list.
+Unlike the *`select`* method (which is a generator), the *`ho_join`* method returns a list.
 
 It takes a list of tuples each with two or three elements:
 
 * a remote Relation object that must be accessible by a foreign key (direct or "reverse");
 * the name of the key under which the associated data would be stored;
 * an optional list of columns (`str[]`) or the name of a column (`str`) to be retreived from the
   remote object.
@@ -694,15 +690,15 @@
   If the third argument is omitted, all columns are retreived.
 
 For example, the following code would return the list of people named `Lagaffe` with two
 additional attributes (`comments` and `posts`):
 
 ```#python
 lagaffe = Person(last_name='Lagaffe')
-res = lagaffe._ho_join(
+res = lagaffe.ho_join(
     (Comment(), 'comments', ['id', 'post_id']),
     (Post(), 'posts', 'id')
 )
 ```
 
 * The data associated with `comments` is a list of dictionaries whose keys are 'id' and 'post_id'.
 * The data associated  with  `posts` is a simple list of values corresponding to the 'id' column.
@@ -738,14 +734,14 @@
 
 By the way, this is the code used in the `Model.ping` method that makes sure the connection is established and attempts a reconnection if it is not.
 
 That's it! You've learn pretty much everything there is to know about `half_orm`.
 
 # Next: `hop`, the GitOps `half_orm` packager [WIP][alpha]
 
-The `hop` command, directly provided in this package (from version 0.8.0rc1), allows you to ***create*** a Python package corresponding to the model of your database, to ***patch*** the model and the corresponding Python code, to ***test*** your database model and your business code.
+The [`hop`](https://github.com/collorg/halfORM/blob/main/doc/hop.md) command, directly provided in this package (from version 0.8.0rc1), allows you to ***create*** a Python package corresponding to the model of your database, to ***patch*** the model and the corresponding Python code, to ***test*** your database model and your business code.
 
-No documentation at the moment, but you can check the idea with the [test script](https://github.com/collorg/halfORM/blob/master/half_orm/packager/test/dummy_test.sh).
+* More at https://github.com/collorg/halfORM/blob/main/doc/hop.md
 
 # Want to contribute?
 
 Fork me on Github: https://github.com/collorg/halfORM
```

### Comparing `half_orm-0.8.0rc9/README.md` & `half_orm-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# A simple PostgreSQL to Python mapper [0.8.0rc8]
-
+# A simple PostgreSQL to Python mapper [0.9.0] and its packager [0.1.0a2]
 
 ![PyPI version](https://img.shields.io/pypi/v/half_orm)
 ![Python versions](https://img.shields.io/pypi/pyversions/half_orm)
-![CI badge](https://github.com/collorg/halfORM/actions/workflows/python-package.yml/badge.svg) 
+![CI badge](https://github.com/collorg/halfORM/actions/workflows/python-package.yml/badge.svg)
+![Coveralls](https://img.shields.io/coverallsCoverage/github/collorg/halfORM)
 ![PyPI downloads](https://img.shields.io/pypi/dm/half_orm)
 ![Contributors](https://img.shields.io/github/contributors/collorg/halform)
 
-You have a PostgreSQL database at hand and you want to interact with it in Python (&ge; 3.6); `half_orm` maps your tables and views to Python classes that you can easily use to manipulate your data.
+You have a PostgreSQL database at hand and you want to interact with it in Python (&ge; 3.6); `half_orm` maps your tables and views to Python classes that you can easily use to manipulate your data. If you want to build or patch a model, you might be interested in the [`half_orm packager`](#next-hop-the-gitops-half_orm-packager-wipalpha).
 
 The 'half' part of `half_orm` name indicates that it only deals with the data manipulation language ([DML](https://www.postgresql.org/docs/current/dml.html)) part of SQL. Basically the [`INSERT`](https://www.postgresql.org/docs/current/sql-insert.html), [`SELECT`](https://www.postgresql.org/docs/current/sql-select.html), [`UPDATE`](https://www.postgresql.org/docs/current/sql-update.html) and [`DELETE`](https://www.postgresql.org/docs/current/sql-delete.html) commands. This is what makes `half_orm` so easy to learn an use.
 
 Here is what coding with `half_orm` looks like :
 
 ```python
 from half_orm.model import Model
@@ -33,44 +33,40 @@
 class Person(halftest.get_relation_class('actor.person')):
     Fkeys = {
         'posts_rfk': '_reverse_fkey_halftest_blog_post_author_first_name_author_last_name_author_birth_date',
         'comments_rfk': '_reverse_fkey_halftest_blog_comment_author_id'
     }
     @singleton # This ensures that the author of the post is well defined.
     def add_post(self, title: str=None, content: str=None) -> dict:
-        return self.posts_rfk(title=title, content=content)._ho_insert()
+        return self.posts_rfk(title=title, content=content).ho_insert()
     @singleton
     def add_comment(self, post: Post=None, content: str=None) -> dict:
-        return self.comments_rfk(content=content, post_id=post.id.value)._ho_insert()
+        return self.comments_rfk(content=content, post_id=post.id.value).ho_insert()
 
 def main():
     gaston = Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28')
-    gaston._ho_delete()
-    if gaston._ho_is_empty(): # gaston defines a subset of the actor.person table.
-        gaston._ho_insert()
+    gaston.ho_delete()
+    if gaston.ho_is_empty(): # gaston defines a subset of the actor.person table.
+        gaston.ho_insert()
     post = Post(**gaston.add_post(title='Easy', content='halfORM is fun!'))
     gaston.add_comment(content='This is a comment on the newly created post.', post=post)
     print(list(post.comments_rfk())) # The relational objects are iterators
-    post._ho_update(title='Super easy')
-    gaston._ho_delete()
+    post.ho_update(title='Super easy')
+    gaston.ho_delete()
 ```
 
 
 # Tutorial: Learn `half_orm` in half an hour
 
 
 
 ## Install `half_orm`
 
 run `pip install half_orm` in a virtual environment.
 
-## Install `half_orm` pre-release
-
-`pip install half_orm==0.8.0rc9`
-
 ### Set your HALFORM_CONF_DIR
 
 Create a directory to store your connection files and set the shell variable `HALFORM_CONF_DIR`
 (by default, `half_orm` looks in the /etc/half_orm directory):
  
 ```sh
 % mkdir ~/.half_orm
@@ -256,60 +252,60 @@
 assert len(nobody) == 0 # last_name is part of the PK
 ```
 
 ## Set operators
 
 You can use the set operators to set more complex constraints on your relations:
 - `&`, `|`, `^` and `-` for `and`, `or`, `xor` and `not`.
-Take a look at [the algebra test file](https://github.com/collorg/halfORM/blob/master/test/relation/algebra_test.py).
+Take a look at [the algebra test file](https://github.com/collorg/halfORM/blob/main/test/relation/algebra_test.py).
 - you can also use the `==`, `!=` and `in` operators to compare two sets.
 
 ```python
 my_selection = Person(last_name=('ilike', '_a%')) | Person(first_name=('like', 'A%'))
 ```
 
 `my_selection` represents the set of people whose second letter of the name is in `['a', 'A']` or whose first letter of the first name is an `A`.
 
 
-# DML. The `_ho_insert`, `_ho_select`, `_ho_update`, `_ho_delete` methods.
+# DML. The `ho_insert`, `ho_select`, `ho_update`, `ho_delete` methods.
 
 These methods trigger their corresponding SQL querie on the database. 
 For debugging purposes, you can print the SQL query built 
-by half_orm when the DML method is invoked using the _ho_mogrify() method.
+by half_orm when the DML method is invoked using the ho_mogrify() method.
 
 ```py
-people._ho_mogrify()
-people._ho_select()
+people.ho_mogrify()
+people.ho_select()
 ```
 
-## _ho_insert
-To insert a tuple in the relation, use the `_ho_insert` method as shown below:
+## ho_insert
+To insert a tuple in the relation, use the `ho_insert` method as shown below:
 ```python
-Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28')._ho_insert()
+Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28').ho_insert()
 ```
 
-By default, `_ho_insert` returns the inserted row as a dict:
+By default, `ho_insert` returns the inserted row as a dict:
 
 ```python
 lagaffe = Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28')
-lagaffe_id = lagaffe._ho_insert()['id']
+lagaffe_id = lagaffe.ho_insert()['id']
 ```
 
-You can trigger a transaction for any combination of insert, modify or delete operations using the `Relation._ho_transaction` decorator.
+You can trigger a transaction for any combination of insert, modify or delete operations using the `Relation.ho_transaction` decorator.
 
 ```py
 class Person(halftest.get_relation_class('actor.person')):
     # [...]
 
     def insert_many(self, *data):
         """Insert serveral people in a single transaction."""
-        @self._ho_transaction
+        @self.ho_transaction
         def insert(self, *data):
             for d_pers in data:
-                self(**d_pers)._ho_insert()
+                self(**d_pers).ho_insert()
         insert(self, *data)
 
 ```
 
 ```python
 people = Person()
 people.insert_many(*[
@@ -322,68 +318,68 @@
 ```
 
 **Note**: half_orm works in autocommit mode by default. Without a transaction, any missing data
 would be inserted.
 
 ### Returned values
 
-By default `_ho_insert` returns all the inserted values as a dictionary. You can specify the columns
-you want to get by passing their names as argurments to `_ho_insert`.
+By default `ho_insert` returns all the inserted values as a dictionary. You can specify the columns
+you want to get by passing their names as argurments to `ho_insert`.
 
-## _ho_select
-The `_ho_select` method is a generator. It returns all the data of the relation that matches the constraint defined on the Relation object.
+## ho_select
+The `ho_select` method is a generator. It returns all the data of the relation that matches the constraint defined on the Relation object.
 The data is returned in a list of `dict`s.
 
 ```python
 >>> people = Person()
->>> print(list(people._ho_select()))
+>>> print(list(people.ho_select()))
 [{'id': 6753, 'first_name': 'Gaston', 'last_name': 'Lagaffe', 'birth_date': datetime.date(1957, 2, 28)}, {'id': 6754, 'first_name': 'Bibi', 'last_name': 'Fricotin', 'birth_date': datetime.date(1924, 10, 5)}, {'id': 6755, 'first_name': 'Corto', 'last_name': 'Maltese', 'birth_date': datetime.date(1975, 1, 7)}, {'id': 6756, 'first_name': 'Achile', 'last_name': 'Talon', 'birth_date': datetime.date(1963, 11, 7)}, {'id': 6757, 'first_name': 'Gil', 'last_name': 'Jourdan', 'birth_date': datetime.date(1956, 9, 20)}]
 >>>
 ```
 
 You can set a limit or an offset:
 ```python
->>> people._ho_offset(1)._ho_limit(2)
->>> print(list(people)) # Relation objects are iterators. so _ho_select is optional
+>>> people.ho_offset(1).ho_limit(2)
+>>> print(list(people)) # Relation objects are iterators. so ho_select is optional
 [{'id': 6754, 'first_name': 'Bibi', 'last_name': 'Fricotin', 'birth_date': datetime.date(1924, 10, 5)}, {'id': 6755, 'first_name': 'Corto', 'last_name': 'Maltese', 'birth_date': datetime.date(1975, 1, 7)}]
 ```
 
-You can also get a subset of the attributes by passing a list of columns names to `_ho_select`:
+You can also get a subset of the attributes by passing a list of columns names to `ho_select`:
 
 ```python
->>> print(list(people._ho_select('last_name')))
+>>> print(list(people.ho_select('last_name')))
 [{'last_name': 'Lagaffe'}, {'last_name': 'Fricotin'}]
 ```
 
 **Note**: The offset and limit still apply.
 
-### Select one: the `_ho_get` method
+### Select one: the `ho_get` method
 
-The `_ho_get` method returns an Relation object whose fields are populated with the values from the corresponding row in the database.
-It raises an [ExpectedOneError](https://github.com/collorg/halfORM/blob/master/half_orm/relation_errors.py)
+The `ho_get` method returns an Relation object whose fields are populated with the values from the corresponding row in the database.
+It raises an [ExpectedOneError](https://github.com/collorg/halfORM/blob/main/half_orm/relation_errors.py)
 Exception if 0 or more than 1 rows match the intention. The returned object is a singleton (see below).
 
 ```py
-gaston = Person(last_name='Lagaffe')._ho_get()
+gaston = Person(last_name='Lagaffe').ho_get()
 ```
 
 is equivalent to
 
 ```py
 lagaffe = Person(last_name='Lagaffe')
-if lagaffe._ho_is_empty() or len(lagaffe) > 1:
+if lagaffe.ho_is_empty() or len(lagaffe) > 1:
     raise ExcpetedOneError
-gaston = Person(**next(lagaffe._ho_select()))
+gaston = Person(**next(lagaffe.ho_select()))
 gaston._ho_is_singleton = True
 ```
 
-You could use `_ho_get` to retreive the `id` of the row:
+You could use `ho_get` to retreive the `id` of the row:
 
 ```py
-gaston_id = Person(last_name='Lagaffe')._ho_get('id').id.value
+gaston_id = Person(last_name='Lagaffe').ho_get('id').id.value
 ```
 
 ### Is it a set? Is it an element of the set?
 
 Let's go back to our definition of the class `Person`. We would like to write a property that
 returns the full name of **a** person. 
 
@@ -432,107 +428,107 @@
     # [...]
     @singleton
     def do_something_else(self):
         "Needs self to be a singleton"
         ...
 
     def do_something(self):
-        for elt in self._ho_select():
+        for elt in self.ho_select():
             pers = Person(**elt)
             pers._ho_is_singleton = True # You must be pretty sure of what you're doing here. See the warning and the explanation.
             pers.do_something_else() # Warning! do_something_else won't check that pers is indeed a singleton
 ```
 
 **Warning!** By setting `_ho_is_singleton` value to `True`, you disable the check that `@singleton` would have made before executing `do_something_else`. 
 This example works for two reasons:
 
-1. `_ho_select` is called without argument ensuring that all columns are retreived from the database.
-Note: Calling `_ho_select` with columns corresponding to the primary key as arguments would also have worked;
+1. `ho_select` is called without argument ensuring that all columns are retreived from the database.
+Note: Calling `ho_select` with columns corresponding to the primary key as arguments would also have worked;
 2. The table `actor.person` has a primary key which makes it a set (ie. each element returned by select is
 indeed a singleton).
 
-## _ho_update
+## ho_update
 
 To update a subset, you first define the subset an then invoque the `ho_udpate`
 method with the new values passed as argument.
 
 ```py
 gaston = Person(first_name='Gaston')
-gaston._ho_update(birth_date='1970-01-01')
+gaston.ho_update(birth_date='1970-01-01')
 ```
 
 Let's look at how we could turn the last name into capital letters for a subset of people:
 
 ```python
 class Person(halftest.get_relation_class('actor.person')):
     # [...]
 
     def upper_last_name(self):
         "tranform last name to upper case."
-        @self._ho_transaction
+        @self.ho_transaction
         def update(self):
-            for d_pers in self._ho_select('id', 'last_name'):
+            for d_pers in self.ho_select('id', 'last_name'):
                 pers = Person(**d_pers)
-                pers._ho_update(last_name=d_pers['last_name'].upper())
+                pers.ho_update(last_name=d_pers['last_name'].upper())
         update(self)
 ```
 
-Again, we insure the atomicity of the transaction using the `Relation._ho_transaction` decorator.
+Again, we insure the atomicity of the transaction using the `Relation.ho_transaction` decorator.
 
 ```
 >>> a_pers = Person(last_name=('ilike', '_a%'))
->>> print([elt.last_name for elt in list(a_pers._ho_select())])
+>>> print([elt.last_name for elt in list(a_pers.ho_select())])
 >>> a_pers = Person(last_name = ('ilike', '_a%'))
->>> print([elt['last_name'] for elt in a_pers._ho_select('last_name')])
+>>> print([elt['last_name'] for elt in a_pers.ho_select('last_name')])
 ['Lagaffe', 'Maltese', 'Talon']
 >>> a_pers.upper_last_name()
->>> print([elt['last_name'] for elt in a_pers._ho_select('last_name')])
+>>> print([elt['last_name'] for elt in a_pers.ho_select('last_name')])
 ['LAGAFFE', 'MALTESE', 'TALON']
 ```
 
 ### Returning values
 
-To return the updated values, you can add to `_ho_update` the column names you want to get, or `*` if you want to get all the columns.
+To return the updated values, you can add to `ho_update` the column names you want to get, or `*` if you want to get all the columns.
 
 ```python
->>> gaston._ho_update('*', birth_date='1970-01-01')
+>>> gaston.ho_update('*', birth_date='1970-01-01')
 ```
 
 ### Update all data in a table
 
 If you want to update all the data in a relation, you must set the argument `update_all` to `True`. A `RuntimeError` is raised otherwise.
 
 ```py
-Person()._ho_update(birth_date='1970-01-01', update_all=True)
+Person().ho_update(birth_date='1970-01-01', update_all=True)
 ```
 
-## _ho_delete
+## ho_delete
 
-The `_ho_delete` method allows you to remove a set of elements from a table:
+The `ho_delete` method allows you to remove a set of elements from a table:
 
 ```py
 gaston = Person(first_name='Gaston')
-gaston._ho_delete()
+gaston.ho_delete()
 ```
 
 To remove every tuples from a table, you must set the argument `delete_all` to `True`. A `RuntimeError` is raised otherwise.
 
 ```python
-Person()._ho_delete(delete_all=True)
-if not Person()._ho_is_empty():
+Person().ho_delete(delete_all=True)
+if not Person().ho_is_empty():
     print('Weird! You should check your "on delete cascade".')
 ```
 Well, there is not much left after this in the `actor.person` table.
 
 ### Returning values
 
-As for `_ho_update`, to return the deleted values, you can add to `_ho_delete` the column names you want to get, or `*` if you want to get all the columns.
+As for `ho_update`, to return the deleted values, you can add to `ho_delete` the column names you want to get, or `*` if you want to get all the columns.
 
 ```python
->>> gaston._ho_delete('first_name', 'last_name', 'birth_date')
+>>> gaston.ho_delete('first_name', 'last_name', 'birth_date')
 ```
 
 # Working with foreign keys [WIP]
 
 > This is a work in progress
 
 A relational object integrates all the material necessary to process its foreign keys and the
@@ -629,40 +625,40 @@
 The Fkey class has the `set` method which allows you to constrain a foreign key with a Relation object.
 To get the comments made by Gaston, we simply constraint the `author_fk` Fkey to reference the entry corresponding to Gaston in the actor.person table. To do so, we use the `Fkey.set()` method:
 
 ```python
 gaston = Person(first_name='Gaston')
 gaston_comments = Comment()
 gaston_comments.author_fk.set(gaston)
-print(list(gaston_comments._ho_select())
+print(list(gaston_comments.ho_select())
 ```
 ## Chaining foreign keys
 
 **Important note**: Foreign key chaining will only work if the modules corresponding to the tables are ordered
 according to the names of the tables in the package. See the `hop` command.
 
 You can easily chain foreign keys. For example, if you want to get all the comments made by Gaston
 on his own posts:
 
 ```py
 gaston = {'last_name':'Lagaffe', 'first_name':'Gaston', 'birth_date':'1957-02-28'}
-gaston_id = Person(**gaston)._ho_get('id').id.value # we ensure that Gaston is a singleton
+gaston_id = Person(**gaston).ho_get('id').id.value # we ensure that Gaston is a singleton
 list(gaston
     .post_rfk(**gaston)
     .comment_rfk(author_id=gaston_id))
 ```
 
 **Note**: the `blog.post` table declares a foreign key on `actor.person(first_name, last_name, birth_date)` 
 while the `blog.comment` table declares a foreign key on `actor.person(id)`.
 
-## The *`_ho_join`* method
+## The *`ho_join`* method
 
-The *`_ho_join`* method allows you to integrate the data associated with a Relation object into the result obtained by the *`select`* method by using foreign keys of the object or by referencing the object.
+The *`ho_join`* method allows you to integrate the data associated with a Relation object into the result obtained by the *`select`* method by using foreign keys of the object or by referencing the object.
 
-Unlike the *`select`* method (which is a generator), the *`_ho_join`* method returns a list.
+Unlike the *`select`* method (which is a generator), the *`ho_join`* method returns a list.
 
 It takes a list of tuples each with two or three elements:
 
 * a remote Relation object that must be accessible by a foreign key (direct or "reverse");
 * the name of the key under which the associated data would be stored;
 * an optional list of columns (`str[]`) or the name of a column (`str`) to be retreived from the
   remote object.
@@ -670,15 +666,15 @@
   If the third argument is omitted, all columns are retreived.
 
 For example, the following code would return the list of people named `Lagaffe` with two
 additional attributes (`comments` and `posts`):
 
 ```#python
 lagaffe = Person(last_name='Lagaffe')
-res = lagaffe._ho_join(
+res = lagaffe.ho_join(
     (Comment(), 'comments', ['id', 'post_id']),
     (Post(), 'posts', 'id')
 )
 ```
 
 * The data associated with `comments` is a list of dictionaries whose keys are 'id' and 'post_id'.
 * The data associated  with  `posts` is a simple list of values corresponding to the 'id' column.
@@ -714,14 +710,14 @@
 
 By the way, this is the code used in the `Model.ping` method that makes sure the connection is established and attempts a reconnection if it is not.
 
 That's it! You've learn pretty much everything there is to know about `half_orm`.
 
 # Next: `hop`, the GitOps `half_orm` packager [WIP][alpha]
 
-The `hop` command, directly provided in this package (from version 0.8.0rc1), allows you to ***create*** a Python package corresponding to the model of your database, to ***patch*** the model and the corresponding Python code, to ***test*** your database model and your business code.
+The [`hop`](https://github.com/collorg/halfORM/blob/main/doc/hop.md) command, directly provided in this package (from version 0.8.0rc1), allows you to ***create*** a Python package corresponding to the model of your database, to ***patch*** the model and the corresponding Python code, to ***test*** your database model and your business code.
 
-No documentation at the moment, but you can check the idea with the [test script](https://github.com/collorg/halfORM/blob/master/half_orm/packager/test/dummy_test.sh).
+* More at https://github.com/collorg/halfORM/blob/main/doc/hop.md
 
 # Want to contribute?
 
 Fork me on Github: https://github.com/collorg/halfORM
```

### Comparing `half_orm-0.8.0rc9/half_orm/field.py` & `half_orm-0.9.0/half_orm/field.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         self.__metadata = metadata
         self.__sql_type = self.__metadata['fieldtype']
         self.__value = None
         self.__unaccent = False
         self.__comp = '='
 
     @property
-    def _relation(self):
+    def _relation(self): # pragma: no cover
         return self.__relation
 
     def is_set(self):
         "Returns if the field is set or not."
         return self.__is_set
 
     def _is_part_of_pk(self):
@@ -44,76 +44,71 @@
         if self.__is_set:
             repr_ = f"{repr_} ({self.__name} {self.__comp} {self.__value})"
         return repr_.strip()
 
     def __str__(self):
         return str(self.__value)
 
-    def _praf(self, query, _ho_id):
+    def __praf(self, query, ho_id):
         """Returns field_name prefixed with relation alias if the query is
         select. Otherwise, returns the field name quoted with ".
         """
-        _ho_id = f'r{_ho_id}'
+        ho_id = f'r{ho_id}'
         if query == 'select':
-            return f'{_ho_id}."{self.__name}"'
+            return f'{ho_id}."{self.__name}"'
         return f'"{self.__name}"'
 
-    def _where_repr(self, query, _ho_id):
+    def _where_repr(self, query, ho_id):
         """Returns the SQL representation of the field for the where clause
         """
         where_repr = ''
         comp_str = '%s'
         comp = self._comp()
         if comp == '@@':
             comp_str = 'websearch_to_tsquery(%s)'
         if isinstance(self.__value, (list, tuple)):
             if self.__sql_type[0] != '_': # not an array type
                 comp_str = 'any(%s)'
                 if comp == '@@':
                     comp_str = 'any(websearch_to_tsquery(%s))'
         if not self.unaccent:
-            where_repr = f"{self._praf(query, _ho_id)} {comp} {comp_str}"
+            where_repr = f"{self.__praf(query, ho_id)} {comp} {comp_str}"
         else:
-            where_repr = f"unaccent({self._praf(query, _ho_id)}) {comp} unaccent({comp_str})"
+            where_repr = f"unaccent({self.__praf(query, ho_id)}) {comp} unaccent({comp_str})"
         return where_repr
 
     @property
     def value(self):
         "Returns the value of the field object"
         return self.__value
 
     def _set(self, *args):
         "Sets the value of the field object"
         self.__set__(self.__relation, *args)
 
     def __set__(self, obj, *args):
         """Sets the value (and the comparator) associated with the field."""
         self.__relation._ho_is_singleton = False
-        if len(args) == 1:
-            value = args[0]
-            if value is None:
-                self._unset()
-                return
-            comp = None
-            self.__relation = obj
-            if isinstance(value, tuple):
-                if len(value) != 2:
-                    raise ValueError(f"Can't match {value} with (comp, value)!")
-                comp, value = value
-            if value is NULL and comp is None:
-                comp = 'is'
-            elif comp is None:
-                comp = '='
-        elif len(args) == 2:
-            # The first argument IS comp.
-            comp, value = args
-            if value is None:
-                raise ValueError("Can't have a None value with a comparator!")
-        else:
-            raise RuntimeError('')
+        value = args[0]
+        if value is None:
+            self._unset()
+            return
+        comp = None
+        self.__relation = obj
+        if isinstance(value, tuple):
+            if len(value) != 2:
+                raise ValueError(f"Can't match {value} with (comp, value)!")
+            comp, value = value
+        if value is None:
+            raise ValueError("Can't have a None value with a comparator!")
+        if value is NULL and comp is None:
+            comp = 'is'
+        elif comp is None:
+            comp = '='
+        comp = comp.lower()
         if value is NULL:
             if not comp in {'is', 'is not'}:
                 raise ValueError("comp should be 'is' or 'is not' with NULL value!")
         self.__is_set = True
         self.__value = value
         self.__comp = comp
 
@@ -125,15 +120,15 @@
 
     @property
     def unaccent(self):
         return self.__unaccent
     @unaccent.setter
     def unaccent(self, value):
         if not isinstance(value, bool):
-            raise RuntimeError('unaccent argument must be of boolean type!')
+            raise RuntimeError('unaccent value must be True or False!')
         self.__unaccent = value
 
     def _comp(self):
         "Returns the comparator associated to the value."
         if self.__comp == '%':
             return '%%'
         return self.__comp
@@ -155,23 +150,17 @@
     def _name(self):
         return self.__name
 
     def __call__(self):
         """In case someone inadvertently uses the name of a field for a method."""
         rel_class = self.__relation.__class__
         rcn = rel_class.__name__
-        method = None
-        try:
-            method = rel_class.__dict__[self.__name]
-            # print('XXX', isinstance(method, types.FunctionType))
-        except KeyError as err:
-            # genuine attemp to call a Field.
-            raise err
+        method = rel_class.__dict__.get(self.__name)
         err_msg = "'Field' object is not callable."
         warn_msg = f"'{self.__name}' is an attribute of type Field of the '{rcn}' object."
-        err_msg = f"{err_msg}\nWARNING:        {warn_msg}"
         if method:
-            err_msg = f"{err_msg}\n                Do not use '{self.__name}' as a method name."
+            err_msg = f"{err_msg}\n{warn_msg}"
+            err_msg = f"{err_msg}\nDo not use '{self.__name}' as a method name."
         raise TypeError(err_msg)
 
 psycopg2.extensions.register_adapter(Field, Field._psycopg_adapter)
 psycopg2.extensions.register_adapter(dict, psycopg2.extras.Json)
```

### Comparing `half_orm-0.8.0rc9/half_orm/fkey.py` & `half_orm-0.9.0/half_orm/fkey.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # -*- coding: utf-8 -*-
 # pylint: disable=protected-access
 
 """This module provides the FKey class."""
 
 from half_orm.pg_meta import normalize_fqrn, normalize_qrn
+from half_orm.packager import utils
 
 class FKey:
     """Foreign key class
 
     A foreign key is set by assigning to it a Relation object of the
     corresponding type (see FKey.set method).
-    It is then used to construct the join query for Relation._ho_select
+    It is then used to construct the join query for Relation.ho_select
     method.
     """
 
     def __init__(self,
                  fk_name, relation, fk_sfqrn,
                  fk_names=None, fields=None, confupdtype=None, confdeltype=None):
         self.__relation = relation
@@ -26,142 +27,125 @@
         self.__fk_to = None
         self.__confupdtype = confupdtype
         self.__confdeltype = confdeltype
         self.__fk_fqrn = fk_sfqrn
         self.__fields_names = fields
         self.__fields = [f'"{name}"' for name in fields]
 
+    def __get_rel(self, fqtn):
+        """Returns the relation class referenced by fqtn.
+        First try model._import_class fallback to model.get_relation_class on ImportError.
+        """
+        try:
+            return self.__relation._model._import_class(fqtn)
+        except ImportError:
+            return self.__relation._model.get_relation_class(fqtn)
+
     def __call__(self, __cast__=None, **kwargs):
         """Returns the relation referenced by the fkey.
-        If model._scope is set, instanciate the class from the scoped module.
-        Uses the __cast if it is set.
+        Uses the __cast__ if it is set.
         """
-        model = self.__relation._model
         f_cast = None
-        get_rel = model._import_class if model._scope is not None else model.get_relation_class
+        # get_rel = model._import_class if model._scope is not None else model.get_relation_class
         if self.__name.find('_reverse_fkey_') == 0 and __cast__:
-            self.__relation = get_rel(__cast__)(**self.__relation._ho_dict())
+            self.__relation = self.__get_rel(__cast__)(**self.__relation.ho_dict())
         else:
             f_cast = __cast__
-        f_relation = get_rel(f_cast or normalize_qrn(self.__fk_fqrn))(**kwargs)
-        rev_fkey_name = f'_reverse_{f_relation._ho_id}'
+        f_relation = self.__get_rel(f_cast or normalize_qrn(self.__fk_fqrn))(**kwargs)
+        rev_fkey_name = f'_reverse_{f_relation.ho_id}'
         f_relation._ho_fkeys[rev_fkey_name] = FKey(
             rev_fkey_name,
             f_relation,
             f_relation._t_fqrn, self.__fields, self.__fk_names)
         f_relation._ho_fkeys[rev_fkey_name].set(self.__relation)
         return f_relation
 
     def values(self):
-        return [list(elt.values()) for elt in self.__to_relation._ho_select(*self.__fk_names)]
+        return [list(elt.values()) for elt in self.__to_relation.ho_select(*self.__fk_names)]
+
+    def set(self, __to):
+        """Sets the relation associated to the foreign key.
 
-    def set(self, to_):
-        """Sets the relation associated to the foreign key."""
+        TODO: check that the __to is indeed atteinable from self
+        """
+        # pylint: disable=import-outside-toplevel
         from half_orm.relation import Relation
 
-        self.__to_relation = to_
+        if not issubclass(__to.__class__, Relation):
+            raise RuntimeError("Fkey.set excepts an argument of type Relation")
+        if id(self.__relation) == id(__to):
+            raise RuntimeError(f"Can't set Fkey {self.__name} on the same object")
+        self.__to_relation = __to
         from_ = self.__relation
-        if not issubclass(to_.__class__, Relation):
-            raise Exception("Expecting a Relation")
-        to_classes = set(type.mro(to_.__class__))
-        self_classes = set(type.mro(self.__relation.__class__))
-        common_classes = to_classes.intersection(self_classes)
-        if object in common_classes:
-            common_classes.remove(object)
-        if not common_classes:
-            raise Exception(f"Type mismatch:\n{self.__fk_fqrn} != {to_._fqrn}")
+        # to_classes = set(type.mro(__to.__class__))
+        # to_classes.add(__to.__class__)
+        # print('XXX', to_classes, self.__expected_to_relation)
+        # if not self.__expected_to_relation in to_classes:
+        #     raise RuntimeError(f"Type mismatch:\n{self.__fk_fqrn} != {__to._fqrn}")
         self.__fk_from = from_
-        self.__fk_to = to_
-        self.__is_set = to_._ho_is_set()
-        from_._ho_join_to[self] = to_
-
-    @classmethod
-    def __set__(cls, *args):
-        "Setting an Fkey is prohibited"
-        print('XXX', cls, '\n', args)
-        raise RuntimeError
+        self.__fk_to = __to
+        self.__is_set = __to.ho_is_set()
+        from_._ho_join_to[self] = __to
 
     def is_set(self):
         """Return if the foreign key is set (boolean)."""
         return self.__is_set
 
     @property
-    def to_(self):
-        """Returns the destination relation of the fkey."""
-        return self.__fk_to
-
-    @to_.setter
-    def to_(self, to_):
-        """Sets the destination relation of the fkey."""
-        self.__fk_to = to_
-
-    @property
-    def fk_fqrn(self):
-        """Returns the FQRN of the relation pointed to."""
-        return self.__fk_fqrn
-
-    @property
     def confupdtype(self):
         "on update configuration"
         return self.__confupdtype
 
     @property
     def confdeltype(self):
         "on delete configuration"
         return self.__confdeltype
 
+    #@utils.trace
     def _join_query(self, orig_rel):
         """Returns the join_query, join_values of a foreign key.
-        fkey interface: frel, from_, to_, fields, fk_names
+        fkey interface: frel, from_, __to, fields, fk_names
         """
         from_ = self.__fk_from
-        to_ = self.to_
-        if id(from_) == id(to_):
-            raise RuntimeError("You can't join a relation with itself!")
-        orig_rel_id = f'r{orig_rel._ho_id}'
-        to_id = f'r{to_._ho_id}'
-        from_id = f'r{from_._ho_id}'
-        if to_._qrn == orig_rel._qrn:
+        __to = self.__fk_to
+        orig_rel_id = f'r{orig_rel.ho_id}'
+        to_id = f'r{__to.ho_id}'
+        from_id = f'r{from_.ho_id}'
+        if __to._qrn == orig_rel._qrn:
             to_id = orig_rel_id
         if from_._qrn == orig_rel._qrn:
             from_id = orig_rel_id
         from_fields = (f'{from_id}.{name}' for name in self.__fields)
-        to_fields = (f'{to_id}.{name}' for name in self.fk_names)
+        to_fields = (f'{to_id}.{name}' for name in self.__fk_names)
         bounds = " and ".join(
             [f'{a} = {b}' for a, b in zip(to_fields, from_fields)])
         return f"({bounds})"
 
-    def _prep_select(self):
-        if self.__is_set:
-            return self.__fields, self.to_._ho_prep_select(*self.fk_names)
-        return None
+    #@utils.trace
+    def _fkey_prep_select(self):
+        return (self.__fields, self.__fk_to.ho_prep_select(*self.fk_names)) if self.__is_set else None
 
     @property
     def fk_names(self):
         """Returns the names of the fields composing the foreign key in the foreign table."""
         return self.__fk_names
 
-    @fk_names.setter
-    def fk_names(self, fk_names):
-        """Sets the names of the fields in the foreign table."""
-        self.__fk_names = fk_names
-
     @property
     def names(self):
         "Returns the names of the fields composing the foreign key in the table"
         return self.__fields_names
 
     def __repr__(self):
         """Representation of a foreign key
         """
         fields = list(self.__fields)
         fields.sort()
         fields = f"({', '.join(fields)})"
         repr_ = f"- {self.__name}: {fields}\n ↳ {normalize_fqrn(self.__fk_fqrn)}({', '.join(self.fk_names)})"
         if self.__is_set:
-            repr_value = str(self.to_)
+            repr_value = str(self.__fk_to)
             res = []
             for line in repr_value.split('\n'):
                 res.append(f'     {line}')
             res = '\n'.join(res)
             repr_ = f'{repr_}\n{res}'
         return repr_
```

### Comparing `half_orm-0.8.0rc9/half_orm/hotest.py` & `half_orm-0.9.0/half_orm/hotest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,42 @@
+# pylint: disable=protected-access
+
 import unittest
 from typing import List
 from half_orm.relation import Relation
 
 class HoTestCase(unittest.TestCase):
     def hotAssertIsPkey(self, relation: Relation, field_names: List[str]):
         "it shoud be the primary key"
         pkey = set(relation()._ho_pkey.keys())
         if set(field_names) != pkey:
             raise self.fail(f'PKey failure: {set(field_names)} != {pkey}')
 
     def hotAssertIsUnique(self, relation: Relation, fields_names: List[str]):
         "Checks if a list of fields is unique for the relation."
-        fields_nums = set()
-        pkeynum = []
+        if (set(fields_names) == set(relation._ho_pkey.keys())):
+            return # OK it's the primary key
         for field_name in fields_names:
-            field = relation()._fields[field_name]
-            metadata = field._Field__metadata
-            fields_nums.add(metadata['fieldnum'])
-            if not pkeynum and metadata['pkeynum']:
-                pkeynum = metadata['pkeynum']
-            if not metadata['uniq'] and pkeynum != metadata['pkeynum']:
+            field = relation()._ho_fields[field_name]
+            if not field._Field__metadata['uniq']:
                 raise self.fail(f"'{fields_names}' is not unique.")
-        if fields_nums != set(pkeynum):
-            raise self.fail(f"'{fields_names}' is not unique.")
 
     def hotAssertIsNotNull(self, relation: Relation, field_name: str):
-        if not relation()._fields[field_name].is_not_null():
+        if not relation()._ho_fields[field_name].is_not_null():
             raise self.fail(f"'{field_name}' is not 'not null'.")
         
     def hotAssertReferences(self, relation: Relation, fk_name: str, f_relation: Relation):
         referenced = relation()._ho_fkeys[fk_name]()
         if not referenced._qrn == f_relation._qrn:
-            raise self.fail(f"{relation}()._ho_fkeys['{fk_name}']() does not reference {f_relation}")
+            raise self.fail(f"{relation.__class__.__name__}()._ho_fkeys['{fk_name}']() does not reference {f_relation.__name__}")
 
     def hotAssertAliasReferences(self, relation: Relation, alias: str, f_relation: Relation):
         referenced = eval(f"relation().{alias}")
         if not referenced()._qrn == f_relation._qrn:
-            raise self.fail(f"{relation}.{alias}() does not reference {f_relation}")
+            raise self.fail(f"{relation.__class__.__name__}.{alias}() does not reference {f_relation.__name__}")
 
     def __check_update_action(self, relation: Relation, fk_name: str, update_type: str):
         return self.assertEqual(relation()._ho_fkeys[fk_name].confupdtype, update_type)
 
     def __check_delete_action(self, relation: Relation, fk_name: str, delete_type: str):
         return self.assertEqual(relation()._ho_fkeys[fk_name].confdeltype, delete_type)
```

### Comparing `half_orm-0.8.0rc9/half_orm/model.py` & `half_orm-0.9.0/half_orm/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,55 +17,32 @@
 
 Note:
     The default schema is ``public`` in PostgreSQL, so to reference a table
     ``my_table`` in this schema you'll have to use ``pubic.my_table``.
 """
 
 
-import inspect
 import os
 import sys
 from configparser import ConfigParser
 from os import environ
-from functools import wraps
-from typing import Generator, List
+from typing import List
 
 import psycopg2
-from psycopg2 import pool
 from psycopg2.extras import RealDictCursor
 
 from half_orm import model_errors
-from half_orm.relation import Relation, REL_INTERFACES, REL_CLASS_NAMES
 from half_orm import pg_meta
-from half_orm.packager import utils
+from half_orm.relation_factory import factory
 
 CONF_DIR = os.path.abspath(environ.get('HALFORM_CONF_DIR', '/etc/half_orm'))
 
 
 psycopg2.extras.register_uuid()
 
-def deprecated(fct):
-    @wraps(fct)
-    def wrapper(self, *args, **kwargs):
-        name = fct.__name__
-        dep_name = name.replace('_ho_', '')
-        callerframerecord = inspect.stack()[1]
-        frame = callerframerecord[0]
-        info = inspect.getframeinfo(frame)
-        context = ''
-        warn_msg = (f'HalfORM WARNING! "{utils.Color.bold(dep_name)}" is deprecated. '
-            'It will be removed in half_orm 1.0.\n'
-            f'Use "{utils.Color.bold(name)}" instead.\n')
-        if info.code_context:
-            context = info.code_context[0]
-            warn_msg += (f'{info.filename}:{info.lineno}, in {info.function}\n'
-                f'{context}\n')
-        sys.stderr.write(warn_msg)
-        return fct(self, *args, **kwargs)
-    return wrapper
 
 class Model:
     """
     Parameters:
         config_file (str): the configuration file that contains the informations to connect
             to the database.
         scope (Optional[str]): used to agregate several modules in a package.
@@ -90,22 +67,15 @@
     def __init__(self, config_file: str, scope: str=None):
         """Model constructor
 
         Use @config_file in your scripts. The @dbname parameter is
         reserved to the __factory metaclass.
         """
         self.__dbinfo = {}
-        self.__minconn = None
-        self.__maxconn = None
         self.__load_config(config_file)
-        self.__pool = None
-        if self.__minconn and self.__maxconn:
-            self.__pool =  pool.ThreadedConnectionPool(
-                self.__minconn, self.__maxconn, **self.__dbinfo)
-        self.__backend_pid = None
         self._scope = scope and scope.split('.')[0]
         self.__conn = None
         self.__connect()
 
     def __load_config(self, config_file):
         """Load the config file
 
@@ -126,27 +96,22 @@
         try:
             dbname = database['name']
         except KeyError as exc:
             raise model_errors.MalformedConfigFile(file_, 'Missing mandatory parameter', 'name') from exc
 
         if self.__dbinfo and config_file and dbname != self.__dbname:
             raise RuntimeError(
-                f"Can't reconnect to another database {dbname} != {self.__dbname}")
+                f"Can't reconnect to another database: {dbname} != {self.__dbname}")
 
         self.__dbinfo['dbname'] = dbname
         self.__dbinfo['user'] = database.get('user')
         self.__dbinfo['password'] = database.get('password')
         self.__dbinfo['host'] = database.get('host')
         self.__dbinfo['port'] = database.get('port')
 
-        if config.has_section('pool'):
-            c_pool = config['pool']
-            self.__minconn = c_pool.get('minconn')
-            self.__maxconn = c_pool.get('maxconn')
-
     def __connect(self, config_file: str=None, reload: bool=False):
         """Setup a new connection to the database.
 
         The reconnect method is an alias to the ``__connect`` method.
 
         Parameters:
             config_file (str): If a config_file is provided, the connection is made with the new
@@ -155,31 +120,22 @@
                 the model has changed.
         """
         self.disconnect()
 
         if config_file:
             self.__load_config(config_file)
 
-        try:
-            if self.__pool is None:
-                self.__conn = psycopg2.connect(
-                    **self.__dbinfo, cursor_factory=RealDictCursor)
-            else:
-                self.__conn = self.__pool.getconn()
-            self.__conn.autocommit = True
-            self.__pg_meta = pg_meta.PgMeta(self.__conn, reload)
-            self.__deja_vu[self.__dbname] = self
-            self.__backend_pid = self.execute_query(
-                "select pg_backend_pid()").fetchone()['pg_backend_pid']
-        except psycopg2.OperationalError as err:
-            raise err.__class__(err)
+        self.__conn = psycopg2.connect(**self.__dbinfo, cursor_factory=RealDictCursor)
+        self.__conn.autocommit = True
+        self.__pg_meta = pg_meta.PgMeta(self.__conn, reload)
+        self.__deja_vu[self.__dbname] = self
 
     reconnect = __connect
 
-    def get_relation_class(self, relation_name: str) -> Relation:
+    def get_relation_class(self, relation_name: str): # -> Relation
         """This method is a factory that generates a class that inherits the `Relation <#half_orm.relation.Relation>`_ class.
 
         Args:
             relation_name (string): the full name (`<schema>.<relation>`) of the targeted relation in the database.
 
         Raises:
             ValueError: if the schema is missing in relation_name
@@ -205,68 +161,14 @@
                 >>> model.get_relation_class('person')
                 [...]MissingSchemaInName: do you mean 'public.person'?
 
             An `UnknownRelation <#half_orm.model_errors.UnknownRelation>`_ is raised if the relation is not found in the model:
                 >>> model.get_relation_class('public.person')
                 [...]UnknownRelation: 'public.person' does not exist in the database halftest.
         """
-
-        def factory(dct):
-            """Function to build a Relation class corresponding to a PostgreSQL
-            relation.
-            """
-            def _gen_class_name(rel_kind, sfqrn):
-                """Generates class name from relation kind and FQRN tuple"""
-                class_name = "".join([elt.capitalize() for elt in
-                                    [elt.replace('.', '') for elt in sfqrn]])
-                return f"{rel_kind}_{class_name}"
-
-            bases = [Relation,]
-            tbl_attr = {}
-            tbl_attr['__base_classes'] = set()
-            tbl_attr['__fkeys_properties'] = False
-            tbl_attr['_qrn'] = pg_meta.normalize_qrn(dct['fqrn'])
-
-            tbl_attr.update(dict(zip(['_dbname', '_schemaname', '_relationname'], dct['fqrn'])))
-            if not tbl_attr['_dbname'] in Model._classes_:
-                Model._classes_[tbl_attr['_dbname']] = {}
-            if dct.get('model'):
-                tbl_attr['_model'] = dct['model']
-            else:
-                tbl_attr['_model'] = Model._deja_vu(tbl_attr['_dbname'])
-            rel_class = Model._check_deja_vu_class(*dct['fqrn'])
-            if rel_class:
-                return rel_class
-
-            try:
-                metadata = tbl_attr['_model']._relation_metadata(dct['fqrn'])
-            except KeyError as exc:
-                raise model_errors.UnknownRelation(dct['fqrn']) from exc
-            if metadata['inherits']:
-                metadata['inherits'].sort()
-                bases = []
-            for parent_fqrn in metadata['inherits']:
-                bases.append(factory({'fqrn': parent_fqrn}))
-            tbl_attr['__metadata'] = metadata
-            tbl_attr['_t_fqrn'] = dct['fqrn']
-            tbl_attr['_fqrn'] = pg_meta.normalize_fqrn(dct['fqrn'])
-            tbl_attr['__kind'] = REL_CLASS_NAMES[metadata['tablekind']]
-            tbl_attr['_fkeys'] = []
-            for fct_name, fct in REL_INTERFACES[metadata['tablekind']].items():
-                tbl_attr[fct_name] = fct
-                dep_fct_name = None
-                if fct_name[0:4] == '_ho_':
-                    dep_fct_name = fct_name[4:]
-                if dep_fct_name:
-                    tbl_attr[dep_fct_name] = deprecated(tbl_attr[fct_name])
-            class_name = _gen_class_name(REL_CLASS_NAMES[metadata['tablekind']], dct['fqrn'])
-            rel_class = type(class_name, tuple(bases), tbl_attr)
-            Model._classes_[tbl_attr['_dbname']][dct['fqrn']] = rel_class
-            return rel_class
-
         try:
             schema, table = relation_name.replace('"', '').rsplit('.', 1)
         except ValueError as err:
             raise model_errors.MissingSchemaInName(relation_name) from err
         return factory({'fqrn': (self.__dbname, schema, table), 'model': self})
 
 
@@ -292,16 +194,18 @@
         """
         try:
             self.execute_query("select 1")
             return True
         except (psycopg2.OperationalError, psycopg2.InterfaceError):
             try:
                 self.__connect()
-            except psycopg2.OperationalError as err:
-                sys.stderr.write(f'{err}\n')
+                self.execute_query("select 1")
+            except (psycopg2.OperationalError, psycopg2.InterfaceError) as exc: #pragma: no cover
+                # log reconnection attempt failure
+                sys.stderr.write(f'{exc.exception}\n')
                 sys.stderr.flush()
             return False
 
     def disconnect(self):
         """Closes the connection to the database.
         """
         if self.__conn is not None:
@@ -312,19 +216,14 @@
         """Reload metadata
 
         Updates the model according to changes made to the database.
         """
         self.__connect(config_file, True)
 
     @property
-    def _pg_backend_pid(self):
-        "backend PID"
-        return self.__backend_pid
-
-    @property
     def _dbname(self):
         """
         property. Returns the database name.
         """
         return self.__dbname
 
     @property
@@ -436,21 +335,14 @@
             >>> model.has_relation('public.person')
             False
             >>> model.has_relation('actor.person')
             True
         """
         return self.__pg_meta.has_relation(self.__dbname, *qtn.rsplit('.', 1))
 
-    @classmethod
-    def _check_deja_vu_class(cls, dbname, schema, relation):
-        """Not to use with _import_class.
-        """
-        if cls._classes_.get(dbname):
-            return cls._classes_[dbname].get((dbname, schema, relation))
-
     def _import_class(self, qtn, scope=None):
         """Used to return the class from the scope module.
 
         This method is used to import a class from a module. The module
         must reside in an accessible python package named `scope`.
         """
         t_qtn = qtn.replace('"', '').rsplit('.', 1)
```

### Comparing `half_orm-0.8.0rc9/half_orm/model_errors.py` & `half_orm-0.9.0/half_orm/model_errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,20 +13,14 @@
     """
     def __init__(self, filename, msg, missing_param):
         self.filename = filename
         Exception.__init__(
             self,
             f"Malformed config file: {filename}\n{msg}: {missing_param}")
 
-class UnknownDatabase(Exception):
-    """The database dbname couldn't be found. Connexion error ?"""
-    def __init__(self, dbname):
-        self.dbname = dbname
-        Exception.__init__(self, f'Unknown database: {dbname}')
-
 class UnknownRelation(Exception):
     """The FQRN doesn't match any relation in the database."""
     def __init__(self, sfqrn):
         self.dbname = sfqrn[0]
         self.schema = sfqrn[1]
         self.relation = sfqrn[2]
         Exception.__init__(self, f"'{sfqrn[1]}.{sfqrn[2]}' does not exist in the database {sfqrn[0]}.")
```

### Comparing `half_orm-0.8.0rc9/half_orm/packager/changelog.py` & `half_orm-0.9.0/half_orm/packager/changelog.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc9/half_orm/packager/database.py` & `half_orm-0.9.0/half_orm/packager/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         if get_release and self.__repo.devel:
             self.__last_release = self.last_release
 
     @property
     def last_release(self):
         "Returns the last release"
         self.__last_release = next(
-            self.__model.get_relation_class('half_orm_meta.view.hop_last_release')()._ho_select())
+            self.__model.get_relation_class('half_orm_meta.view.hop_last_release')().ho_select())
         return self.__last_release
 
     @property
     def last_release_s(self):
         "Returns the string representation of the last release X.Y.Z"
         return '{major}.{minor}.{patch}'.format(**self.last_release)
 
@@ -118,8 +118,8 @@
         "Helper: execute a postgresql command"
         return self.__connection_params.execute_pg_command
 
     def register_release(self, major, minor, patch, changelog):
         "Register the release into half_orm_meta.hop_release"
         return self.__model.get_relation_class('half_orm_meta.hop_release')(
             major=major, minor=minor, patch=patch, changelog=changelog
-        )._ho_insert()
+        ).ho_insert()
```

### Comparing `half_orm-0.8.0rc9/half_orm/packager/db_conn.py` & `half_orm-0.9.0/half_orm/packager/db_conn.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 
 from getpass import getpass
 from configparser import ConfigParser
 
 from half_orm.model import CONF_DIR
 from half_orm.packager import utils
 
+CONF_NOT_FOUND = '''
+The configuration file {} is missing.
+You must create it before proceeding.
+
+'''
 
 class DbConn:
     """Handles the connection parameters to the database.
     Provides the execute_pg_command."""
     __conf_dir = CONF_DIR # HALFORM_CONF_DIR
     def __init__(self, name):
         self.__name = name
@@ -22,15 +27,15 @@
         self.__password = None
         self.__host = None
         self.__port = None
         self.__production = None
         if name:
             self.__connection_file = os.path.join(self.__conf_dir, self.__name)
             if not os.path.exists(self.__connection_file):
-                raise FileNotFoundError
+                utils.error(CONF_NOT_FOUND.format(self.__connection_file), 1)
             self.__init()
 
     @property
     def production(self):
         "prod"
         return self.__production
```

### Comparing `half_orm-0.8.0rc9/half_orm/packager/hgit.py` & `half_orm-0.9.0/half_orm/packager/hgit.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc9/half_orm/packager/hop.py` & `half_orm-0.9.0/half_orm/packager/hop.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc9/half_orm/packager/manifest.py` & `half_orm-0.9.0/half_orm/packager/manifest.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc9/half_orm/packager/modules.py` & `half_orm-0.9.0/half_orm/packager/modules.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc9/half_orm/packager/patch.py` & `half_orm-0.9.0/half_orm/packager/patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,23 +61,26 @@
             next_release_s = f"{n_rel['major']}.{n_rel['minor']}.{n_rel['patch']}"
             n_rel['in_dev'] = ''
             if next_release_s in releases_in_dev:
                 n_rel['in_dev'] = '(IN DEV)'
             n_rels[level] = n_rel
         return n_rels
 
+    def __assert_main_branch(self):
+        if str(self.__repo.hgit.branch) != 'hop_main':
+            utils.error(
+                'ERROR! Wrong branch. Please, switch to the hop_main branch before.\n', exit_code=1)
+
     def prep_release(self, release_level, message=None):
         """Returns the next (major, minor, patch) tuple according to the release_level
 
         Args:
             release_level (str): one of ['patch', 'minor', 'major']
         """
-        if str(self.__repo.hgit.branch) != 'hop_main':
-            utils.error(
-                'ERROR! Wrong branch. Please, switch to the hop_main branch before.\n', exit_code=1)
+        self.__assert_main_branch()
         next_releases = self.__next_releases
         if release_level is None:
             next_levels = '\n'.join(
                 [f"""- {level}: {'{major}.{minor}.{patch} {in_dev}'.format(**next_releases[level])}"""
                 for level in self.__levels])
             print(f'Next releases:\n{next_levels}')
             next_possible_releases = [elt for elt in self.__levels if not next_releases[elt]['in_dev']]
@@ -298,14 +301,15 @@
             self.__repo.hgit.commit("-m", f"Add sql for release {next_release}")
             self.__repo.hgit.rebase_to_hop_main(push)
         else:
             utils.error('pytest is not installed!\n', 1)
 
     def upgrade_prod(self):
         "Upgrade the production"
+        self.__assert_main_branch()
         self.__save_db(self.__repo.database.last_release_s)
         for release in self.__repo.changelog.releases_to_apply_in_prod:
             self.apply(release, save_db=False)
 
     def restore(self, release):
         "Restore the database and package to a release (in production)"
         self.__restore_db(release)
```

### Comparing `half_orm-0.8.0rc9/half_orm/packager/patches/0/1/0/00_half_orm_meta.database.sql` & `half_orm-0.9.0/half_orm/packager/patches/0/1/0/00_half_orm_meta.database.sql`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc9/half_orm/packager/patches/sql/half_orm_meta.sql` & `half_orm-0.9.0/half_orm/packager/patches/sql/half_orm_meta.sql`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc9/half_orm/packager/repo.py` & `half_orm-0.9.0/half_orm/packager/repo.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -179,14 +179,15 @@
         return '\n'.join(res)
 
     def new(self, package_name, devel):
         "Create a new hop repository"
         cur_dir = os.path.abspath(os.path.curdir)
         self.__base_dir = os.path.join(cur_dir, package_name)
         self.__config = Config(self.__base_dir, name=package_name, devel=devel)
+        self.database = Database(self).init(self.__config.name)
         print(f"Installing new hop repo in {self.__base_dir}.")
 
         if not os.path.exists(self.__base_dir):
             os.makedirs(self.__base_dir)
         else:
             utils.error(f"ERROR! The path '{self.__base_dir}' already exists!\n", exit_code=1)
         readme = utils.read(os.path.join(utils.TEMPLATE_DIRS, 'README'))
@@ -204,15 +205,14 @@
                 half_orm_version=half_orm.VERSION,
                 hop_version=utils.hop_version())
         utils.write(os.path.join(self.__base_dir, 'Pipfile'), pipfile)
 
         os.mkdir(os.path.join(self.__base_dir, '.hop'))
         # self.__config = Config(self.__base_dir)
         self.__config.write()
-        self.database = Database(self).init(self.__config.name)
         modules.generate(self)
 
         readme = readme.format(
             hop_version=utils.hop_version(), dbname=self.__config.name, package_name=self.__config.name)
         utils.write(os.path.join(self.__base_dir, 'README.md'), readme)
         utils.write(os.path.join(self.__base_dir, '.gitignore'), git_ignore)
         self.hgit = HGit().init(self.__base_dir)
```

### Comparing `half_orm-0.8.0rc9/half_orm/packager/templates/README` & `half_orm-0.9.0/half_orm/packager/templates/README`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc9/half_orm/packager/templates/setup.py` & `half_orm-0.9.0/half_orm/packager/templates/setup.py`

 * *Files identical despite different names*

### Comparing `half_orm-0.8.0rc9/half_orm/packager/utils.py` & `half_orm-0.9.0/half_orm/packager/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 "Various utilities"
 
 import os
 import sys
+from functools import wraps
 
 class Color:
     "Colors for the console"
     @staticmethod
     def red(text):
         "red"
         return f"\033[1;31m{text}\033[0m"
@@ -55,7 +56,21 @@
     sys.stderr.write(f'{Color.bold("HOP ERROR")}: {Color.red(msg)}')
     if exit_code:
         sys.exit(exit_code)
 
 def warning(msg: str):
     "Write warning message on stderr"
     sys.stderr.write(Color.bold(f'HOP WARNING: {msg}'))
+
+trace_depth = 0
+def trace(fct):
+    @wraps(fct)
+    def wrapper(self, *args, **kwargs):
+        global trace_depth
+        name = fct.__name__
+        print(f'{" " * trace_depth}>>[{trace_depth}]>> {name}')
+        trace_depth += 1
+        res = fct(self, *args, **kwargs)
+        trace_depth -= 1
+        return res
+    return wrapper
+
```

### Comparing `half_orm-0.8.0rc9/half_orm/pg_meta.py` & `half_orm-0.9.0/half_orm/pg_meta.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,38 @@
-"""This module provides the SQL request to extract the metadata of a
-PostgreSQL database.
+"""This module provides the SQL query to extract the metadata of a PostgreSQL
+database. The query extracts information about tables, views, materialized
+views, foreign tables, and partitioned tables along with their columns,
+data types, constraints, inheritance hierarchy, and other related information.
+
+The module provides several helper functions to format the results of the
+query. These include functions to normalize fully qualified relation names,
+convert relation names to CamelCase, and strip double quotes from relation
+names.
+
+Functions:
+
+    * strip_quotes(qrn): Removes all double quotes from the given fully qualified
+      relation name (fqrn).
+    * __get_qrn(fqrn): Returns the qualified relation name (<schema>.<relation>)
+      from the given fully qualified relation name (fqrn).
+    * normalize_fqrn(t_fqrn): Transforms the tuple (<db name>, <schema name>, <table name>)
+      to "<db name>":"<schema name>"."<table name>". Dots are allowed only in the schema name.
+    * normalize_qrn(t_qrn): Returns "<schema name>"."<relation name>" for the given qualified
+      relation name (qrn) tuple. A schema name can have any number of dots in it, and a table
+      name can't have a dot in it.
+    * camel_case(string): Returns the given string transformed to camel case.
+    * class_name(qrn): Returns the class name from the given qualified relation name (qrn).
+
+The main query is defined as a string variable named _REQUEST. It includes joins
+between several PostgreSQL system tables and views to extract the metadata.
+The resulting query returns data about tables, views, materialized views, foreign
+tables, and partitioned tables in the database, along with information about their
+columns and constraints.
+
+Note that this module requires the psycopg2 library to be installed.
 """
 
 from collections import OrderedDict
 from psycopg2.extras import RealDictCursor
 
 def strip_quotes(qrn):
     "Removes all double quotes from the qrn/fqrn"
@@ -154,40 +183,67 @@
     @classmethod
     def register(cls, dbname, meta):
         cls.__d_meta[dbname] = meta
 
     def __getitem__(self, key):
         return _Meta.__d_meta.__getitem__(key)
 
-    def __setitem__(self, key, val):
-        _Meta.__d_meta.__setitem__(key, val)
+    # def __setitem__(self, key, val):
+    #     _Meta.__d_meta.__setitem__(key, val)
 
-    def __repr__(self):
-        dictrepr = dict.__repr__(self.__d_meta)
-        return f'{type(self).__name__}({dictrepr})'
-  
-    def update(self, *args, **kwargs):
-        for key, value in dict(*args, **kwargs).items():
-            self.__d_meta[key] = value
+    # def __repr__(self):
+    #     dictrepr = dict.__repr__(self.__d_meta)
+    #     return f'{type(self).__name__}({dictrepr})'
 
 class PgMeta:
+    """A utility class for loading and storing metadata of a PostgreSQL database.
+
+    Attributes:
+        meta (_Meta): A singleton instance of the `_Meta` class.
+    """
     meta = _Meta()
     def __init__(self, connection, reload=False):
+        """Initializes a new instance of the `PgMeta` class.
+
+        Args:
+            connection (psycopg2.extensions.connection): A connection object to a PostgreSQL database.
+            reload (bool, optional): A flag indicating whether to reload the metadata from the database. \
+            Defaults to False.
+        """
         self.__dbname = connection.get_dsn_parameters()['dbname']
         if not PgMeta.meta.deja_vu(self.__dbname) or reload:
             self.__load_metadata(connection)
 
     def metadata(self, dbname):
+        """Retrieves the metadata for the specified database name.
+
+        Args:
+            dbname (str): The name of the PostgreSQL database.
+
+        Returns:
+            dict: The metadata of the specified database.
+        """
         return self.meta[dbname].__metadata
 
     def relations_list(self, dbname):
+        """Retrieves a list of relations for the specified database.
+
+        Args:
+            dbname (str): The name of the PostgreSQL database.
+
+        Returns:
+            list: A list of relations for the specified database.
+        """
         return self.metadata(dbname)['relations_list']
 
     def __load_metadata(self, connection):
-        """Loads the metadata by querying the _REQUEST.
+        """Loads the metadata by querying the PostgreSQL database and registers it in the _Meta singleton.
+
+        Args:
+            connection (psycopg2.extensions.connection): A connection object to a PostgreSQL database.
         """
         metadata = {'relations_list': []}
         byname = metadata['byname'] = OrderedDict()
         byid = metadata['byid'] = {}
         with connection.cursor(cursor_factory=RealDictCursor) as cur:
             cur.execute(_REQUEST)
             all_ = [elt for elt in cur.fetchall()]
@@ -232,80 +288,125 @@
                     confupdtype = dct['fkey_confupdtype']
                     confdeltype = dct['fkey_confdeltype']
                     ffields = [byid[fkeytableid]['fields'][num] for num in dct['fkeynum']]
                     rev_fkey_name = f'_reverse_fkey_{"_".join(table_key)}.{".".join(fields)}'
                     rev_fkey_name = strip_quotes(rev_fkey_name.replace(".", "_").replace(":", "_"))
                     byname[table_key]['fkeys'][fkeyname] = (
                         ftable_key, ffields, fields, confupdtype, confdeltype)
-                    byname[ftable_key]['fkeys'][rev_fkey_name] = (table_key, fields, ffields)
+                    byname[ftable_key]['fkeys'][rev_fkey_name] = (table_key, fields, ffields, confupdtype, confdeltype)
 
         metadata['relations_list'].sort()
         self.__metadata = metadata
         PgMeta.meta.register(self.__dbname, self)
 
-    def getFqrn(self, dbname, qrn):
-        "Returns the Fully qualified relation name (quoted) from the unquoted (qrn)"
-        schema, table = qrn.rsplit('.', 1)
-        return f'"{dbname}":"{schema}"."{table}"'
-
     def has_relation(self, dbname, schema, relation):
-        """Checks if the qrn is a relation in the database
+        """Checks whether the specified relation exists in the specified database.
+
+        Args:
+            dbname (str): The name of the PostgreSQL database.
+            schema (str): The name of the schema containing the relation.
+            relation (str): The name of the relation.
 
-        @qrn is in the form <schema>.<table>
-        Returns True if the relation exists, False otherwise.
-        Also works for views and materialized views.
+        Returns:
+            bool: True if the relation exists, False otherwise.
         """
         return (dbname, schema, relation) in self.meta[dbname].__metadata['byname']
 
 
     def desc(self, dbname):
-        """Returns the list of the relations of the model.
+        """Returns a list of relations for the specified database.
 
-        Each line contains:
-        - the relation type: 'r' relation, 'v' view, 'm' materialized view,
-        - the quoted FQRN (Fully qualified relation name)
-          <"db name">:"<schema name>"."<relation name>"
-        - the list of the FQRN of the inherited relations.
+        Args:
+            dbname (str): The name of the PostgreSQL database.
 
-        If a qualified relation name (<schema name>.<table name>) is
-        passed, prints only the description of the corresponding relation.
+        Returns:
+            list: A list of relations for the specified database, with each item containing:
+                - The relation type ('r' for table, 'v' for view, or 'm' for materialized view).
+                - The fully qualified relation name (FQRN) in the format\
+                "<database name>:<schema name>.<relation name>".
+                - A list of the FQRN of the inherited relations.
         """
         ret_val = []
         entry = self.metadata(dbname)['byname']
         for key in entry:
             if key[1].find('half_orm_meta') == 0: continue
             inh = []
             tablekind = entry[key]['tablekind']
             if entry[key]['inherits']:
                 inh = [elt for elt in entry[key]['inherits']]
             ret_val.append((tablekind, key, inh))
         return ret_val
 
     def fields_meta(self, dbname, sfqrn):
-        "Retruns the fields metadata for a given sfqrn"
+        """Retrieves the metadata of the fields for the specified fully qualified relation name (FQRN).
+
+        Args:
+            dbname (str): The name of the PostgreSQL database.
+            sfqrn (str): The fully qualified relation name (FQRN) in the format \
+            "<schema name>.<relation name>".
+
+        Returns:
+            dict: The metadata of the fields for the specified relation.
+        """
         return self.metadata(dbname)['byname'][sfqrn]['fields']
 
     def fkeys_meta(self, dbname, sfqrn):
-        "Returns the foreign keys metadata for a given sfqrn"
+        """
+        Returns the foreign keys metadata for a given sfqrn.
+
+        Args:
+            dbname (str): The name of the database.
+            sfqrn (str): The fully qualified relation name for the table whose foreign key metadata you want.
+
+        Returns:
+            dict: A dictionary containing metadata about the foreign keys for the given table.
+        """
         return self.metadata(dbname)['byname'][sfqrn]['fkeys']
 
     def relation_meta(self, dbname, fqrn):
-        "Returns the relation metadata for a given fqrn"
+        """
+        Returns the relation metadata for a given fqrn.
+
+        Args:
+            dbname (str): The name of the database.
+            fqrn (str): The fully qualified relation name for the table whose metadata you want.
+
+        Returns:
+            dict: A dictionary containing metadata about the given table.
+        """
         return self.metadata(dbname)['byname'][fqrn]
 
     def str(self, dbname):
+        """
+        Returns a string representation of the metadata for all tables in the given database.
+
+        Args:
+            dbname (str): The name of the database.
+
+        Returns:
+            str: A string containing metadata about all tables in the given database.
+        """
         out = []
         entry = self.metadata(dbname)['byname']
         for key in entry:
             if key[1].find('half_orm_meta') == 0: continue
             out.append(f"{entry[key]['tablekind']} {normalize_qrn(key)}")
         return '\n'.join(out)
 
     def _unique_constraints_list(self, dbname, sfqrn):
-        "Returns the unique constraints of the given sfqrn"
+        """
+        Returns the unique constraints of the given sfqrn.
+
+        Args:
+            dbname (str): The name of the database.
+            sfqrn (str): The fully qualified relation name for the table whose unique constraints you want.
+
+        Returns:
+            list: A list of tuples, where each tuple contains the names of the fields that make up a unique constraint.
+        """
         rel_meta_by_name = self.metadata(dbname)['byname'][sfqrn]
         tableid = rel_meta_by_name['tableid']
         rel_meta_by_id = self.metadata(dbname)['byid']
         unique_by_num = []
         for key, value in rel_meta_by_name['fields'].items():
             if value['uniq']:
                 t_uniq = tuple(value['pkeynum'])
@@ -316,15 +417,23 @@
             fields_names = []
             for num in elt:
                 fields_names.append(rel_meta_by_id[tableid]['fields'][num])
             unique.append(tuple(fields_names))
         return unique
 
     def _pkey_constraint(self, dbname, sfqrn):
-        "Returns the pkey constraint"
+        """Returns the primary key constraint for the given sfqrn.
+
+        Args:
+            dbname (str): The name of the database.
+            sfqrn (str): The fully qualified relation name for the table whose primary key constraint you want.
+
+        Returns:
+            list: A list of the names of the fields that make up the primary key constraint.
+        """
         rel_meta_by_name = self.metadata(dbname)['byname'][sfqrn]
         tableid = rel_meta_by_name['tableid']
         rel_meta_by_id = self.metadata(dbname)['byid']
         pkey_by_num = []
         for key, value in rel_meta_by_name['fields'].items():
             if value['pkey']:
                 pkey_by_num.append(value['fieldnum'])
```

### Comparing `half_orm-0.8.0rc9/half_orm/relation.py` & `half_orm-0.9.0/half_orm/relation.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,35 +12,33 @@
     >>> model = Model('halftest')
     >>> class Person(model.get_relation_class('actor.person')):
     >>>     # your code goes here
 """
 
 """
 Main methods provided by the class Relation:
-- insert: inserts a tuple into the pg table.
-- select: returns a generator of the elements of the set defined by
+- ho_insert: inserts a tuple into the pg table.
+- ho_select: returns a generator of the elements of the set defined by
   the constraint on the Relation object. The elements are dictionaries with the
   keys corresponding to the selected columns names in the relation.
-  The result is affected by the methods: _ho_distinct, _ho_order_by, _ho_limit and _ho_offset
+  The result is affected by the methods: ho_distinct, ho_order_by, ho_limit and ho_offset
   (see below).
-- update: updates the set defined by the constraint on the Relation object
+- ho_update: updates the set defined by the constraint on the Relation object
   with the values passed as arguments.
-- delete: deletes from the relation the set of elements defined by the constraint
+- ho_delete: deletes from the relation the set of elements defined by the constraint
   on the Relation object.
-- get: returns the unique element defined by the constraint on the Relation object.
+- ho_get: returns the unique element defined by the constraint on the Relation object.
   the element returned if of the type of the Relation object.
-- count: returns the number of elements in the set defined by the constraint on the
-  Relation object.
 
 The following methods can be chained on the object before a select.
 
-- _ho_distinct: ensures that there are no duplicates on the select result.
-- _ho_order_by: sets the order of the select result.
-- _ho_limit: limits the number of elements returned by the select method.
-- _ho_offset: sets the offset for the select method.
+- ho_distinct: ensures that there are no duplicates on the select result.
+- ho_order_by: sets the order of the select result.
+- ho_limit: limits the number of elements returned by the select method.
+- ho_offset: sets the offset for the select method.
 
 """
 
 from functools import wraps
 from collections import OrderedDict
 from uuid import UUID
 from typing import Generator, List
@@ -52,14 +50,15 @@
 
 
 import yaml
 
 from half_orm import relation_errors
 from half_orm.transaction import Transaction
 from half_orm.field import Field
+from half_orm.packager import utils
 
 class _SetOperators:
     """_SetOperators class stores the set operations made on the Relation class objects
 
     - __operator is one of {'or', 'and', 'sub', 'neg'}
     - __right is a Relation object. It can be None if the operator is 'neg'.
     """
@@ -91,17 +90,14 @@
         """Property returning the right operand (relation)."""
         return self.__right
     @right.setter
     def right(self, right):
         """right operand (relation) setter."""
         self.__right = right
 
-    def __repr__(self):
-        return f"{self.__operator} {self.__right and self.__right._fqrn or None}"
-
 class Relation:
     """Used as a base class for the classes generated by
     `Model.get_relation_class <#half_orm.model.Model.get_relation_class>`_.
 
     Args:
         **kwargs: the arguments names must correspond to the columns names of the relation.
 
@@ -131,20 +127,27 @@
     """
 
 #### THE following METHODS are included in Relation class according to
 #### relation type (Table or View). See TABLE_INTERFACE and VIEW_INTERFACE.
 
 def __init__(self, **kwargs):
     _fqrn = ""
-    """The arguments names must correspond to the columns names of the relation.
+    """The names of the arguments must correspond to the names of the columns in the relation.
     """
+    module = __import__(self.__module__, globals(), locals(), ['FKEYS_PROPERTIES', 'FKEYS'], 0)
+    #TODO: remove in release 1.0.0
+    if hasattr(module, 'FKEYS_PROPERTIES') or hasattr(module, 'FKEYS'):
+        err = f'''{utils.Color.bold(module.__name__ + '.FKEYS')} variable is no longer supported!\n'''
+        err += f'''\tUse the "{utils.Color.bold(self.__class__.__name__ + '.Fkeys')}"''' + \
+            ''' class attribute instead.\n'''
+        raise DeprecationWarning(err)
     self._ho_fields = {}
     self._ho_pkey = {}
     self._ho_fkeys = OrderedDict()
-    self._ho_fkeys_attr = set()
+    self.__fkeys_attr = set()
     self._ho_join_to = {}
     self._ho_is_singleton = False
     self.__only = False
     self.__neg = False
     self.__set_fields()
     self.__set_fkeys()
     self.__query = ""
@@ -160,74 +163,69 @@
     kwk_ = set(kwargs.keys())
     if kwk_.intersection(self._ho_fields.keys()) != kwk_:
         raise relation_errors.UnknownAttributeError(str(kwk_.difference(self._ho_fields.keys())))
     _ = {self.__dict__[field_name]._set(value)
          for field_name, value in kwargs.items() if value is not None}
     self.__isfrozen = True
 
-def _ho_insert(self, *args, data=None) -> '[dict]':
+#@utils.trace
+def ho_insert(self, *args) -> '[dict]':
     """Insert a new tuple into the Relation.
 
     Returns:
         [dict]: A singleton containing the data inserted.
 
     Example:
-        >>> gaston = Person(last_name='Lagaffe', first_name='Gaston', birth_date='1970-01-01')._ho_insert()
+        >>> gaston = Person(last_name='Lagaffe', first_name='Gaston', birth_date='1970-01-01').ho_insert()
         >>> print(gaston)
         {'id': 1772, 'first_name': 'Gaston', 'last_name': 'Lagaffe', 'birth_date': datetime.date(1970, 1, 1)}
 
     Note:
         It is not possible to insert more than one row with the insert method
     """
     query_template = "insert into {} ({}) values ({})"
     self.__query_type = 'insert'
-    fields_names, values, fk_fields, fk_query, fk_values = self.__what_to_insert()
+    fields_names, values, fk_fields, fk_query, fk_values = self.__what()
     what_to_insert = ["%s" for _ in range(len(values))]
     if fk_fields:
         fields_names += fk_fields
         what_to_insert += fk_query
         values += fk_values
     query = query_template.format(self._qrn, ", ".join(fields_names), ", ".join(what_to_insert))
-    returning = args
-    if not (data or returning):
-        returning = ['*']
+    returning = args or ['*']
     if returning:
         query = self.__add_returning(query, *returning)
     self.__execute(query, tuple(values))
-    res = [dict(elt) for elt in self.__cursor.fetchall()]
-    if (args or not data) and len(res):
-        return res[0]
-    return {}
+    res = [dict(elt) for elt in self.__cursor.fetchall()] or [{}]
+    return res[0]
 
-def _ho_select(self, *args):
+#@utils.trace
+def ho_select(self, *args):
     """Gets the set of values correponding to the constraint attached to the object.
     This method is a generator.
 
     Arguments:
         *args: the fields names of the returned attributes. If omitted,
             all the fields are returned.
 
     Yields:
         the result of the query as a dictionary.
 
     Example:
-        >>> for person in Person(last_name=('like', 'La%'))._ho_select('id'):
+        >>> for person in Person(last_name=('like', 'La%')).ho_select('id'):
         >>>     print(person)
         {'id': 1772}
     """
-    query, values = self._ho_prep_select(*args)
-    try:
-        self.__execute(query, values)
-    except Exception as err:
-        sys.stderr.write(f"QUERY: {query}\nVALUES: {values}\n")
-        raise err
+    query, values = self.ho_prep_select(*args)
+    self.__execute(query, values)
     for elt in self.__cursor:
         yield dict(elt)
 
-def _ho_get(self, *args: List[str]) -> Relation:
+#@utils.trace
+def ho_get(self, *args: List[str]) -> Relation:
     """The get method allows you to fetch a singleton from the database.
     It garantees that the constraint references one and only one tuple.
 
     Args:
         args (List[str]): list of fields names.\
         If ommitted, all the values of the row retreived from the database\
         are set for the self object.\
@@ -236,107 +234,113 @@
     Returns:
         Relation: the object retreived from the database.
 
     Raises:
         ExpectedOneError: an exception is raised if no or more than one element is found.
 
     Example:
-        >>> gaston = Person(last_name='Lagaffe', first_name='Gaston')._ho_get()
+        >>> gaston = Person(last_name='Lagaffe', first_name='Gaston').ho_get()
         >>> type(gaston) is Person
         True
         >>> gaston.id
         (int4) NOT NULL (id = 1772)
         >>> str(gaston.id)
         '1772'
         >>> gaston.id.value
         1772
     """
     _count = len(self)
     if _count != 1:
         raise relation_errors.ExpectedOneError(self, _count)
     self._ho_is_singleton = True
-    ret = self(**(next(self._ho_select(*args))))
+    ret = self(**(next(self.ho_select(*args))))
     ret._ho_is_singleton = True
     return ret
 
-def _ho_update(self, *args, update_all=False, **kwargs):
+#@utils.trace
+def __fkey_where(self, where, values):
+    _, _, fk_fields, fk_query, fk_values = self.__what()
+    if fk_fields:
+        fk_where = " and ".join([f"({a}) in ({b})" for a, b in zip(fk_fields, fk_query)])
+        if fk_where:
+            if where:
+                where = f"{where} and {fk_where}"
+            else:
+                where = fk_where
+        values += fk_values
+    return where, values
+
+#@utils.trace
+def ho_update(self, *args, update_all=False, **kwargs):
     """
     kwargs represents the values to be updated {[field name:value]}
     The object self must be set unless update_all is True.
-    The constraints of the relations are updated with kwargs.
+    The constraints of self are updated with kwargs.
     """
-    if not (self._ho_is_set() or update_all):
+    if not (self.ho_is_set() or update_all):
         raise RuntimeError(
             f'Attempt to update all rows of {self.__class__.__name__}'
             ' without update_all being set to True!')
 
     update_args = dict(kwargs)
     for key, value in kwargs.items():
         # None values are first removed
-        if value is None:
+        if value is None: # pragma: no cover
             update_args.pop(key)
     if not update_args:
         return None # no new value update. Should we raise an error here?
 
     query_template = "update {} set {} {}"
     what, where, values = self.__update_args(**update_args)
-    _, _, fk_fields, fk_query, fk_values = self.__what_to_insert()
-    if fk_fields:
-        fk_where = " and ".join([f"({a}) in ({b})" for a, b in zip(fk_fields, fk_query)])
-        where = f"{where} and {fk_where}"
-        values += fk_values
+    where, values = self.__fkey_where(where, values)
     query = query_template.format(self._qrn, what, where)
     if args:
         query = self.__add_returning(query, *args)
     self.__execute(query, tuple(values))
     for field_name, value in update_args.items():
         self._ho_fields[field_name]._set(value)
     if args:
         return [dict(elt) for elt in self.__cursor.fetchall()]
 
-def _ho_delete(self, *args, delete_all=False):
+#@utils.trace
+def ho_delete(self, *args, delete_all=False):
     """Removes a set of tuples from the relation.
     To empty the relation, delete_all must be set to True.
     """
-    if not (self._ho_is_set() or delete_all):
+    if not (self.ho_is_set() or delete_all):
         raise RuntimeError(
             f'Attempt to delete all rows from {self.__class__.__name__}'
             ' without delete_all being set to True!')
     query_template = "delete from {} {}"
-    _, values = self.__get_query(query_template)
+    _, values = self.__prep_query(query_template)
     self.__query_type = 'delete'
     _, where, _ = self.__where_args()
-    _, _, fk_fields, fk_query, fk_values = self.__what_to_insert()
-    where = f" where {where}"
-    if where == "(1 = 1)" and not delete_all:
-        raise RuntimeError
-    if fk_fields:
-        fk_where = " and ".join([f"({a}) in ({b})" for a, b in zip(fk_fields, fk_query)])
-        where = f"{where} and {fk_where}"
-        values += fk_values
-    query = query_template.format(self._qrn, where)
+    where, values = self.__fkey_where(where, values)
+    if where:
+        where = f" where {where}"
+    query = f"delete from {self._qrn} {where}"
     if args:
         query = self.__add_returning(query, *args)
     self.__execute(query, tuple(values))
     if args:
         return [dict(elt) for elt in self.__cursor.fetchall()]
 
 @staticmethod
 def __add_returning(query, *args) -> str:
     "Adds the SQL returning clause to the query"
     if args:
-        returning = ','.join(args)
+        returning = ', '.join(args)
         return f'{query} returning {returning}'
     return query
 
-def _ho_unfreeze(self):
+def ho_unfreeze(self):
     "Allow to add attributs to a relation"
     self.__isfrozen = False
 
-def _ho_freeze(self):
+def ho_freeze(self):
     "set __isfrozen to True."
     self.__isfrozen = True
 
 def __setattr__(self, key, value):
     """Sets an attribute as long as __isfrozen is False
 
     The foreign keys properties are not detected by hasattr
@@ -348,36 +352,37 @@
     if self.__isfrozen and not hasattr(self, key):
         raise relation_errors.IsFrozenError(self.__class__, key)
     if self.__dict__.get(key) and isinstance(self.__dict__[key], Field):
         self.__dict__[key]._set(value)
         return
     object.__setattr__(self, key, value)
 
+#@utils.trace
 def __execute(self, query, values):
     try:
         if self.__mogrify:
             print(self.__cursor.mogrify(query, values).decode('utf-8'))
         return self.__cursor.execute(query, values)
     except (psycopg2.OperationalError, psycopg2.InterfaceError):
         self._model.ping()
         self.__cursor = self._model._connection.cursor(cursor_factory=RealDictCursor)
         return self.__cursor.execute(query, values)
 
 @property
-def _ho_id(self):
+def ho_id(self):
     """Return the __id_cast or the id of the relation.
     """
     return self.__id_cast or id(self)
 
 @property
-def _ho_only(self):
+def ho_only(self):
     "Returns the value of self.__only"
     return self.__only
-@_ho_only.setter
-def _ho_only(self, value):
+@ho_only.setter
+def ho_only(self, value):
     """Set the value of self.__only. Restrict the values of a query to
     the elements of the relation (no inherited values).
     """
     if not value in {True, False}:
         raise ValueError(f'{value} is not a bool!')
     self.__only = value
 
@@ -403,23 +408,24 @@
     if hasattr(self.__class__, 'Fkeys') and not self.__fkeys_properties:
         # if not hasattr(self.__class__.__base__, 'Fkeys'):
         #     setattr(self.__class__.__base__, 'Fkeys', self.__class__.Fkeys)
         for key, value in self.Fkeys.items():
             try:
                 if key != '': # we skip empty keys
                     setattr(self, key, self._ho_fkeys[value])
-                    self._ho_fkeys_attr.add(key)
+                    self.__fkeys_attr.add(key)
             except KeyError as exp:
                 raise relation_errors.WrongFkeyError(self, value) from exp
     self.__fkeys_properties = True
 
-def _ho_group_by(self, yml_directive):
+def ho_group_by(self, yml_directive): #pragma: no cover
     """Returns an aggregation of the data according to the yml directive
     description.
     """
+    utils.error("Use at your own risk. This method is not tested.\n")
     def inner_group_by(data, directive, grouped_data, gdata=None):
         """recursive fonction to actually group the data in grouped_data."""
         deja_vu_key = set()
         if gdata is None:
             gdata = grouped_data
         if isinstance(directive, list):
             directive = directive[0]
@@ -479,40 +485,41 @@
 
     grouped_data = {}
     data = list(self)
     directive = yaml.safe_load(yml_directive)
     inner_group_by(data, directive, grouped_data)
     return grouped_data
 
-def _ho_json(self, yml_directive=None, res_field_name='elements', **kwargs):
+def ho_json(self, yml_directive=None, res_field_name='elements', **kwargs): #pragma: no cover
     """Returns a JSON representation of the set returned by the select query.
     if kwargs, returns {res_field_name: [list of elements]}.update(kwargs)
     """
+    utils.error("Use at your own risk. This method is not tested.\n")
 
     def handler(obj):
         """Replacement of default handler for json.dumps."""
         if hasattr(obj, 'isoformat'):
             return str(obj.isoformat())
         if isinstance(obj, UUID):
             return str(obj)
         if isinstance(obj, timedelta):
             return obj.total_seconds()
         raise TypeError(
             f'Object of type {type(obj)} with value of {repr(obj)} is not JSON serializable')
 
     if yml_directive:
-        res = self._ho_group_by(yml_directive)
+        res = self.ho_group_by(yml_directive)
     else:
         res = list(self)
     if kwargs:
         res = {res_field_name: res}
         res.update(kwargs)
     return json.dumps(res, default=handler)
 
-def _ho_dict(self):
+def ho_dict(self):
     """Returns a dictionary containing only the values of the fields
     that are set."""
     return {key:field.value for key, field in self._ho_fields.items() if field.is_set()}
 
 def __to_dict_val_comp(self):
     """Returns a dictionary containing the values and comparators of the fields
     that are set."""
@@ -557,29 +564,30 @@
         ret.append('')
         ret.append(fkeys_usage)
         for fkey in self._ho_fkeys:
             ret.append(f"    '': '{fkey}',")
         ret.append('}')
     return '\n'.join(ret)
 
-def _ho_is_set(self):
+def ho_is_set(self):
     """Return True if one field at least is set or if self has been
     constrained by at least one of its foreign keys or self is the
     result of a combination of Relations (using set operators).
     """
     joined_to = False
     for _, jt_ in self._ho_join_to.items():
-        joined_to |= jt_._ho_is_set()
+        joined_to |= jt_.ho_is_set()
     return (joined_to or bool(self.__set_operators.operator) or bool(self.__neg) or
             bool({field for field in self._ho_fields.values() if field.is_set()}))
 
 def __get_set_fields(self):
     """Returns a list containing only the fields that are set."""
     return [field for field in self._ho_fields.values() if field.is_set()]
 
+#@utils.trace
 def __walk_op(self, rel_id_, out=None, _fields_=None):
     """Walk the set operators tree and return a list of SQL where
     representation of the query with a list of the fields of the query.
     """
     if out is None:
         out = []
         _fields_ = []
@@ -599,250 +607,222 @@
         if self.__neg:
             out.append(")")
     else:
         out.append(self.__where_repr(rel_id_))
         _fields_ += self.__get_set_fields()
     return out, _fields_
 
-def __join(self, orig_rel, deja_vu):
+def __sql_id(self):
+    """Returns the FQRN as alias for the sql query."""
+    return f"{self._qrn} as r{self.ho_id}"
+
+#@utils.trace
+def __get_from(self, orig_rel=None, deja_vu=None):
+    """Constructs the __sql_query and gets the __sql_values for self."""
+    if deja_vu is None:
+        orig_rel = self
+        self.__sql_query = [__sql_id(self)]
+        deja_vu = {self.ho_id:[(self, None)]}
     for fkey, fk_rel in self._ho_join_to.items():
         fk_rel.__query_type = orig_rel.__query_type
-        fk_rel.__get_from(orig_rel, deja_vu)
-        if fk_rel._ho_id not in deja_vu:
-            deja_vu[fk_rel._ho_id] = []
-        elif (fk_rel, fkey) in deja_vu[fk_rel._ho_id] or fk_rel is orig_rel:
+        if fk_rel.ho_id not in deja_vu:
+            deja_vu[fk_rel.ho_id] = []
+        elif (fk_rel, fkey) in deja_vu[fk_rel.ho_id] or fk_rel is orig_rel:
             #sys.stderr.write(f"déjà vu in from! {fk_rel._fqrn}\n")
             continue
-        deja_vu[fk_rel._ho_id].append((fk_rel, fkey))
-        if fk_rel.__set_operators.operator:
-            fk_rel.__get_from(self._ho_id)
+        fk_rel.__get_from(orig_rel, deja_vu)
+        deja_vu[fk_rel.ho_id].append((fk_rel, fkey))
         _, where, values = fk_rel.__where_args()
-        where = f" and\n    {where}"
+        where = f" and\n {where}"
         orig_rel.__sql_query.insert(1, f'\n  join {__sql_id(fk_rel)} on\n   ')
         orig_rel.__sql_query.insert(2, fkey._join_query(self))
         orig_rel.__sql_query.append(where)
         orig_rel.__sql_values += values
 
-def __sql_id(self):
-    """Returns the FQRN as alias for the sql query."""
-    return f"{self._qrn} as r{self._ho_id}"
-
-def __get_from(self, orig_rel=None, deja_vu=None):
-    """Constructs the __sql_query and gets the __sql_values for self."""
-    if deja_vu is None:
-        orig_rel = self
-        self.__sql_query = [__sql_id(self)]
-        deja_vu = {self._ho_id:[(self, None)]}
-    self.__join(orig_rel, deja_vu)
-
+#@utils.trace
 def __where_repr(self, rel_id_):
     where_repr = []
     for field in self.__get_set_fields():
         where_repr.append(field._where_repr(self.__query_type, rel_id_))
-    where_repr = ' and\n    '.join(where_repr) or '1 = 1'
+    where_repr = ' and '.join(where_repr) or '1 = 1'
     ret = f"({where_repr})"
     if self.__neg:
         ret = f"not ({ret})"
     return ret
 
+#@utils.trace
 def __where_args(self, *args):
     """Returns the what, where and values needed to construct the queries.
     """
-    rel_id_ = self._ho_id
+    rel_id_ = self.ho_id
     what = f'r{rel_id_}.*'
     if args:
         what = ', '.join([f'r{rel_id_}.{arg}' for arg in args])
     s_where, set_fields = self.__walk_op(rel_id_)
     s_where = ''.join(s_where)
-    if s_where == '()':
-        s_where = '(1 = 1)'
     return what, s_where, set_fields
 
-def __get_query(self, query_template, *args):
+#@utils.trace
+def __prep_query(self, query_template, *args):
     """Prepare the SQL query to be executed."""
     from half_orm.fkey import FKey
 
     self.__sql_values = []
     self.__query_type = 'select'
     what, where, values = self.__where_args(*args)
     where = f"\nwhere\n    {where}"
     self.__get_from()
     # remove duplicates
     for idx, elt in reversed(list(enumerate(self.__sql_query))):
         if elt.find('\n  join ') == 0 and self.__sql_query.count(elt) > 1:
             self.__sql_query[idx] = '  and\n'
     # check that fkeys are fkeys
-    for fkey_name in self._ho_fkeys_attr:
+    for fkey_name in self.__fkeys_attr:
         fkey_cls = self.__dict__[fkey_name].__class__
         if fkey_cls != FKey:
             raise RuntimeError(
                 f'self.{fkey_name} is not a FKey (got a {fkey_cls.__name__} object instead).\n'
                 f'- use: self.{fkey_name}.set({fkey_cls.__name__}(...))\n'
                 f'- not: self.{fkey_name} = {fkey_cls.__name__}(...)'
                 )
+    # print('XXX __prep_query', what, self.__sql_query, where, values)
     return (
         query_template.format(
             what,
             self.__only and "only" or "",
             ' '.join(self.__sql_query), where),
         values)
 
-def _ho_prep_select(self, *args):
-    self.__sql_values = []
+#@utils.trace
+def ho_prep_select(self, *args):
     query_template = f"select\n {self.__select_params.get('distinct', '')} {{}}\nfrom\n  {{}} {{}}\n  {{}}"
-    query, values = self.__get_query(query_template, *args)
+    query, values = self.__prep_query(query_template, *args)
     values = tuple(self.__sql_values + values)
-    if 'order_by' in self.__select_params.keys():
+    if 'order_by' in self.__select_params:
         query = f"{query} order by {self.__select_params['order_by']}"
-    if 'limit' in self.__select_params.keys():
+    if 'limit' in self.__select_params:
         query = f"{query} limit {self.__select_params['limit']}"
-    if 'offset' in self.__select_params.keys():
+    if 'offset' in self.__select_params:
         query = f"{query} offset {self.__select_params['offset']}"
     return query, values
 
-def _ho_distinct(self):
+def ho_distinct(self):
     """Set distinct in SQL select request."""
     self.__select_params['distinct'] = 'distinct'
     return self
 
-def _ho_unaccent(self, *fields_names):
+def ho_unaccent(self, *fields_names):
     "Sets unaccent for each field listed in fields_names"
     for field_name in fields_names:
         if not isinstance(self.__dict__[field_name], Field):
             raise ValueError(f'{field_name} is not a Field!')
         self.__dict__[field_name].unaccent = True
     return self
 
-def _ho_order_by(self, _order_):
+def ho_order_by(self, _order_):
     """Set SQL order by according to the "order" string passed
 
     @order string example :
     "field1, field2 desc, field3, field4 desc"
     """
     self.__select_params['order_by'] = _order_
     return self
 
-def _ho_limit(self, _limit_):
+def ho_limit(self, _limit_):
     """Set limit for the next SQL select request."""
     if _limit_:
         self.__select_params['limit'] = _limit_
     elif 'limit' in self.__select_params:
         self.__select_params.pop('limit')
     return self
 
-def _ho_offset(self, _offset_):
+def ho_offset(self, _offset_):
     """Set the offset for the next SQL select request."""
     self.__select_params['offset'] = _offset_
     return self
 
-def _ho_mogrify(self):
+def ho_mogrify(self):
     """Prints the select query."""
     self.__mogrify = True
     return self
 
 def __len__(self):
     """Returns the number of tuples matching the intention in the relation.
 
     See select for arguments.
     """
     self.__query = "select"
     query_template = "select\n  count(distinct {})\nfrom {}\n  {}\n  {}"
-    query, values = self.__get_query(query_template)
-    try:
-        vars_ = tuple(self.__sql_values + values)
-        self.__execute(query, vars_)
-    except Exception as err:
-        self._ho_mogrify()
-        self.__execute(query, vars_)
-        raise Exception from err
+    query, values = self.__prep_query(query_template)
+    vars_ = tuple(self.__sql_values + values)
+    self.__execute(query, vars_)
     return self.__cursor.fetchone()['count']
 
-def _ho_is_empty(self):
+def ho_is_empty(self):
     """Returns True if the relation is empty, False otherwise.
 
     Same as __len__ but limits the request to 1 element (faster).
     Use it instead of len(relation) == 0.
     """
     self.__query = "select"
     query_template = "select\n  count(distinct {})\nfrom {}\n  {}\n  {} limit 1"
-    query, values = self.__get_query(query_template)
-    try:
-        vars_ = tuple(self.__sql_values + values)
-        self.__execute(query, vars_)
-    except Exception as err:
-        print(query, vars_)
-        raise err
+    query, values = self.__prep_query(query_template)
+    vars_ = tuple(self.__sql_values + values)
+    self.__execute(query, vars_)
     return self.__cursor.fetchone()['count'] != 1
 
-def __count(self, *args, _distinct=False):
-    """Returns the number of tuples matching the intention in the relation.
-
-    See select for arguments.
-    """
-    self.__query = "select"
-    if _distinct:
-        query_template = "select\n  count(distinct {})\nfrom {}\n  {}\n  {}"
-    else:
-        query_template = "select\n  count({})\nfrom {}\n  {}\n  {}"
-    query, values = self.__get_query(query_template, *args)
-    try:
-        vars_ = tuple(self.__sql_values + values)
-        self.__execute(query, vars_)
-    except Exception as err:
-        self._ho_mogrify()
-        self.__execute(query, vars_)
-        raise Exception from err
-    return self.__cursor.fetchone()['count']
-
+#@utils.trace
 def __update_args(self, **kwargs):
     """Returns the what, where an values for the update query."""
     what_fields = []
     new_values = []
     self.__query_type = 'update'
     _, where, values = self.__where_args()
     where = f" where {where}"
     for field_name, new_value in kwargs.items():
         what_fields.append(field_name)
         new_values.append(new_value)
     what = ", ".join([f'"{elt}" = %s' for elt in what_fields])
     return what, where, new_values + values
 
-def __what_to_insert(self):
-    """Returns the field names and values to be inserted."""
-    fields_names = []
+#@utils.trace
+def __what(self):
+    """Returns the constrained fields and foreign keys.
+    """
     set_fields = self.__get_set_fields()
-    if set_fields:
-        fields_names = [
-            f'"{name}"' for name, field in self._ho_fields.items() if field.is_set()]
+    fields_names = [
+        f'"{name}"' for name, field in self._ho_fields.items() if field.is_set()]
     fk_fields = []
     fk_queries = ''
     fk_values = []
     for fkey in self._ho_fkeys.values():
-        fk_prep_select = fkey._prep_select()
+        fk_prep_select = fkey._fkey_prep_select()
         if fk_prep_select is not None:
             fk_values += list(fkey.values()[0])
             fk_fields += fk_prep_select[0]
             fk_queries = ["%s" for _ in range(len(fk_values))]
 
     return fields_names, set_fields, fk_fields, fk_queries, fk_values
 
 def __call__(self, **kwargs):
     return self.__class__(**kwargs)
 
-def _ho_cast(self, qrn):
+def ho_cast(self, qrn):
     """Cast a relation into another relation.
+
+    TODO: check that qrn inherits self (or is inherited by self)?
     """
     new = self._model._import_class(qrn)(**self.__to_dict_val_comp())
     new.__id_cast = id(self)
     new._ho_join_to = self._ho_join_to
     new.__set_operators = self.__set_operators
     return new
 
-def _ho_join(self, *f_rels):
-    """Joins data to self._ho_select() result. Returns a dict
+def ho_join(self, *f_rels):
+    """Joins data to self.ho_select() result. Returns a dict
     f_rels is a list of [(obj: Relation(), name: str, fields: Optional(<str|str[]>)), ...].
 
     Each obj in f_rels must have a direct or reverse fkey to self.
     If res is the result, res[name] contains the data associated to the element
     through the fkey or reversed fkey.
     If fields is a str, the data associated with res[name] is returned in a list (only one column).
     Otherwise (str[]), res[name] is a list of dict.
@@ -867,15 +847,15 @@
         TO_PROCESS = {UUID, date, datetime, time, timedelta}
         if value.__class__ in TO_PROCESS:
             return str(value)
         return value
 
     res = list(
         {key: to_str(value) for key, value in elt.items()}
-        for elt in self._ho_distinct()
+        for elt in self.ho_distinct()
     )
     result_as_list = False
     ref = self()
     for f_rel in f_rels:
         if not isinstance(f_rel, tuple):
             raise RuntimeError("f_rels must be a list of tuples.")
         if len(f_rel) == 3:
@@ -889,30 +869,30 @@
             fields = [fields]
             result_as_list = True
         res_remote = {}
 
         f_relation_fk_names = []
         fkey_found = False
         for fkey_12 in ref._ho_fkeys:
-            if type(ref._ho_fkeys[fkey_12]) != FKey:
+            if type(ref._ho_fkeys[fkey_12]) != FKey: #pragma: no cover
                 raise RuntimeError("This is not an Fkey")
             remote_fk = ref._ho_fkeys[fkey_12]
             remote = remote_fk()
             if remote.__class__ == f_relation.__class__:
                 for field in f_relation._ho_fields.keys():
                     if f_relation.__dict__[field].is_set():
                         remote.__dict__[field]._set(f_relation.__dict__[field])
                 fkey_found = True
                 f_relation_fk_names = remote_fk.fk_names
                 break
 
         if not fkey_found:
             raise RuntimeError(f"No foreign key between {self._fqrn} and {f_relation._fqrn}!")
         inter = [{key: to_str(val) for key, val in elt.items()}
-            for elt in remote._ho_distinct()._ho_select(
+            for elt in remote.ho_distinct().ho_select(
                 *([f'"{field}"' for field in fields] + f_relation_fk_names))]
         for elt in inter:
             key = tuple(elt[subelt] for subelt in f_relation_fk_names)
             if key not in res_remote:
                 res_remote[key] = []
             if result_as_list:
                 res_remote[key].append(to_str(elt[fields[0]]))
@@ -992,62 +972,57 @@
     return len(right - self) == 0
 
 def __eq__(self, right):
     if id(self) == id(right):
         return True
     return self in right and right in self
 
-def __ne__(self, right):
-    return not self == right
-
 def __enter__(self):
     """Context management entry
 
     Returns self in a transaction context.
 
     Example usage:
     with relation as rel:
-        rel._ho_update(col=new_val)
+        rel.ho_update(col=new_val)
 
     Equivalent to (in a transaction context):
-    rel = relation._ho_select()
+    rel = relation.ho_select()
     for elt in rel:
         new_elt = relation(**elt)
-        new_elt._ho_update(col=new_val)
+        new_elt.ho_update(col=new_val)
     """
-    @self._ho_transaction
-    def context(self):
-        return self
-    return context(self)
+    self.ho_transaction._enter(self._model)
+    return self
 
-def __exit__(_, *__):
+def __exit__(self, *__):
     """Context management exit
 
-    Not much to do here.
     """
+    self.ho_transaction._exit(self._model)
     return False
 
 def __iter__(self):
-    return self._ho_select()
+    return self.ho_select()
 
 def __next__(self):
-    return next(self._ho_select())
+    return next(self.ho_select())
 
 def singleton(fct):
     """Decorator. Enforces the relation to define a singleton.
 
     _ho_is_singleton is set by Relation.get.
     _ho_is_singleton is unset as soon as a Field is set.
     """
     @wraps(fct)
     def wrapper(self, *args, **kwargs):
         if self._ho_is_singleton:
             return fct(self, *args, **kwargs)
         try:
-            self = self._ho_get()
+            self = self.ho_get()
             return fct(self, *args, **kwargs)
         except relation_errors.ExpectedOneError as err:
             raise relation_errors.NotASingletonError(err)
     return wrapper
 
 #### Deprecated
 
@@ -1059,15 +1034,16 @@
     '__execute': __execute,
     '__set_fields': __set_fields,
     '__set_fkeys': __set_fkeys,
     '__call__': __call__,
     '__get_set_fields': __get_set_fields,
     '__repr__': __repr__,
     '__get_from': __get_from,
-    '__get_query': __get_query,
+    '__prep_query': __prep_query,
+    '__fkey_where': __fkey_where,
     '__where_repr': __where_repr,
     '__where_args': __where_args,
     '__len__': __len__,
 
     '__set__op__': __set__op__,
     '__and__': __and__,
     '__iand__': __iand__,
@@ -1079,52 +1055,51 @@
     '__ixor__': __ixor__,
     '__neg__': __neg__,
     '__contains__': __contains__,
     '__eq__': __eq__,
 
     '__sql_id': __sql_id,
     '__walk_op': __walk_op,
-    '__join': __join,
-    '__what_to_insert': __what_to_insert,
+    '__what': __what,
     '__update_args': __update_args,
     '__add_returning': __add_returning,
     '__to_dict_val_comp': __to_dict_val_comp,
     '__enter__': __enter__,
     '__exit__': __exit__,
     '__iter__': __iter__,
     '__next__': __next__,
 
     # protected methods
-    '_ho_freeze': _ho_freeze,
-    '_ho_unfreeze': _ho_unfreeze,
-    '_ho_prep_select': _ho_prep_select,
-    '_ho_mogrify': _ho_mogrify,
+    'ho_freeze': ho_freeze,
+    'ho_unfreeze': ho_unfreeze,
+    'ho_prep_select': ho_prep_select,
+    'ho_mogrify': ho_mogrify,
 
     # public methods
-    '_ho_id': _ho_id,
-    '_ho_order_by': _ho_order_by,
-    '_ho_limit': _ho_limit,
-    '_ho_offset': _ho_offset,
-    '_ho_distinct': _ho_distinct,
-    '_ho_unaccent': _ho_unaccent,
-    '_ho_cast': _ho_cast,
-    '_ho_only': _ho_only,
-    '_ho_is_empty': _ho_is_empty,
-    '_ho_group_by':_ho_group_by,
-    '_ho_json': _ho_json,
-    '_ho_dict': _ho_dict,
-    '_ho_is_set': _ho_is_set,
-    '_ho_get': _ho_get,
-    '_ho_join': _ho_join,
-    '_ho_insert': _ho_insert,
-    '_ho_select': _ho_select,
-    '_ho_update': _ho_update,
-    '_ho_delete': _ho_delete,
+    'ho_id': ho_id,
+    'ho_order_by': ho_order_by,
+    'ho_limit': ho_limit,
+    'ho_offset': ho_offset,
+    'ho_distinct': ho_distinct,
+    'ho_unaccent': ho_unaccent,
+    'ho_cast': ho_cast,
+    'ho_only': ho_only,
+    'ho_is_empty': ho_is_empty,
+    'ho_group_by': ho_group_by,
+    'ho_json': ho_json,
+    'ho_dict': ho_dict,
+    'ho_is_set': ho_is_set,
+    'ho_get': ho_get,
+    'ho_join': ho_join,
+    'ho_insert': ho_insert,
+    'ho_select': ho_select,
+    'ho_update': ho_update,
+    'ho_delete': ho_delete,
 
-    '_ho_transaction': Transaction,
+    'ho_transaction': Transaction,
 }
 
 
 TABLE_INTERFACE = COMMON_INTERFACE
 VIEW_INTERFACE = COMMON_INTERFACE
 MVIEW_INTERFACE = COMMON_INTERFACE
 FDATA_INTERFACE = COMMON_INTERFACE
```

### Comparing `half_orm-0.8.0rc9/half_orm/relation_errors.py` & `half_orm-0.9.0/half_orm/relation_errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         super().__init__(f"ERROR! Unknown attribute: {msg}.")
 
 class IsFrozenError(Exception):
     """Class is frozen"""
     def __init__(self, cls, msg):
         super().__init__(
             f"ERROR! The class {cls} is forzen.\n"
-            f"Use _ho_unfreeze to add the '{msg}' attribute to it.")
+            f"Use ho_unfreeze to add the '{msg}' attribute to it.")
 
 class DuplicateAttributeError(Exception):
     """Attempt to setattr to an already existing attribute."""
 
 class NotASingletonError(Exception):
     """The constraint do not define a singleton.
```

### Comparing `half_orm-0.8.0rc9/half_orm/transaction.py` & `half_orm-0.9.0/half_orm/transaction.py`

 * *Files 16% similar despite different names*

```diff
@@ -65,7 +65,25 @@
         except Exception as err:
             sys.stderr.write(f"Transaction error: {err}\nRolling back!\n")
             Transaction.__level = 0
             relation._model._connection.rollback()
             relation._model._connection.autocommit = True
             raise err
         return res
+
+    @classmethod
+    def _enter(cls, model):
+        "context manager entry"
+        model._connection.autocommit = False
+        Transaction.__level += 1
+
+    @classmethod
+    def _exit(cls, model):
+        "context manager exit"
+        Transaction.__level -= 1
+        if Transaction.__level == 0:
+            model._connection.commit()
+            model._connection.autocommit = True
+
+    @classmethod
+    def is_set(cls):
+        return Transaction.__level > 0
```

### Comparing `half_orm-0.8.0rc9/half_orm.egg-info/PKG-INFO` & `half_orm-0.9.0/half_orm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: half-orm
-Version: 0.8.0rc9
+Version: 0.9.0
 Summary: A simple PostgreSQL to Python mapper.
 Home-page: https://github.com/collorg/halfORM
 Author: Joël Maïzi
 Author-email: joel.maizi@collorg.org
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -18,24 +18,24 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
-# A simple PostgreSQL to Python mapper [0.8.0rc8]
-
+# A simple PostgreSQL to Python mapper [0.9.0] and its packager [0.1.0a2]
 
 ![PyPI version](https://img.shields.io/pypi/v/half_orm)
 ![Python versions](https://img.shields.io/pypi/pyversions/half_orm)
-![CI badge](https://github.com/collorg/halfORM/actions/workflows/python-package.yml/badge.svg) 
+![CI badge](https://github.com/collorg/halfORM/actions/workflows/python-package.yml/badge.svg)
+![Coveralls](https://img.shields.io/coverallsCoverage/github/collorg/halfORM)
 ![PyPI downloads](https://img.shields.io/pypi/dm/half_orm)
 ![Contributors](https://img.shields.io/github/contributors/collorg/halform)
 
-You have a PostgreSQL database at hand and you want to interact with it in Python (&ge; 3.6); `half_orm` maps your tables and views to Python classes that you can easily use to manipulate your data.
+You have a PostgreSQL database at hand and you want to interact with it in Python (&ge; 3.6); `half_orm` maps your tables and views to Python classes that you can easily use to manipulate your data. If you want to build or patch a model, you might be interested in the [`half_orm packager`](#next-hop-the-gitops-half_orm-packager-wipalpha).
 
 The 'half' part of `half_orm` name indicates that it only deals with the data manipulation language ([DML](https://www.postgresql.org/docs/current/dml.html)) part of SQL. Basically the [`INSERT`](https://www.postgresql.org/docs/current/sql-insert.html), [`SELECT`](https://www.postgresql.org/docs/current/sql-select.html), [`UPDATE`](https://www.postgresql.org/docs/current/sql-update.html) and [`DELETE`](https://www.postgresql.org/docs/current/sql-delete.html) commands. This is what makes `half_orm` so easy to learn an use.
 
 Here is what coding with `half_orm` looks like :
 
 ```python
 from half_orm.model import Model
@@ -57,44 +57,40 @@
 class Person(halftest.get_relation_class('actor.person')):
     Fkeys = {
         'posts_rfk': '_reverse_fkey_halftest_blog_post_author_first_name_author_last_name_author_birth_date',
         'comments_rfk': '_reverse_fkey_halftest_blog_comment_author_id'
     }
     @singleton # This ensures that the author of the post is well defined.
     def add_post(self, title: str=None, content: str=None) -> dict:
-        return self.posts_rfk(title=title, content=content)._ho_insert()
+        return self.posts_rfk(title=title, content=content).ho_insert()
     @singleton
     def add_comment(self, post: Post=None, content: str=None) -> dict:
-        return self.comments_rfk(content=content, post_id=post.id.value)._ho_insert()
+        return self.comments_rfk(content=content, post_id=post.id.value).ho_insert()
 
 def main():
     gaston = Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28')
-    gaston._ho_delete()
-    if gaston._ho_is_empty(): # gaston defines a subset of the actor.person table.
-        gaston._ho_insert()
+    gaston.ho_delete()
+    if gaston.ho_is_empty(): # gaston defines a subset of the actor.person table.
+        gaston.ho_insert()
     post = Post(**gaston.add_post(title='Easy', content='halfORM is fun!'))
     gaston.add_comment(content='This is a comment on the newly created post.', post=post)
     print(list(post.comments_rfk())) # The relational objects are iterators
-    post._ho_update(title='Super easy')
-    gaston._ho_delete()
+    post.ho_update(title='Super easy')
+    gaston.ho_delete()
 ```
 
 
 # Tutorial: Learn `half_orm` in half an hour
 
 
 
 ## Install `half_orm`
 
 run `pip install half_orm` in a virtual environment.
 
-## Install `half_orm` pre-release
-
-`pip install half_orm==0.8.0rc9`
-
 ### Set your HALFORM_CONF_DIR
 
 Create a directory to store your connection files and set the shell variable `HALFORM_CONF_DIR`
 (by default, `half_orm` looks in the /etc/half_orm directory):
  
 ```sh
 % mkdir ~/.half_orm
@@ -280,60 +276,60 @@
 assert len(nobody) == 0 # last_name is part of the PK
 ```
 
 ## Set operators
 
 You can use the set operators to set more complex constraints on your relations:
 - `&`, `|`, `^` and `-` for `and`, `or`, `xor` and `not`.
-Take a look at [the algebra test file](https://github.com/collorg/halfORM/blob/master/test/relation/algebra_test.py).
+Take a look at [the algebra test file](https://github.com/collorg/halfORM/blob/main/test/relation/algebra_test.py).
 - you can also use the `==`, `!=` and `in` operators to compare two sets.
 
 ```python
 my_selection = Person(last_name=('ilike', '_a%')) | Person(first_name=('like', 'A%'))
 ```
 
 `my_selection` represents the set of people whose second letter of the name is in `['a', 'A']` or whose first letter of the first name is an `A`.
 
 
-# DML. The `_ho_insert`, `_ho_select`, `_ho_update`, `_ho_delete` methods.
+# DML. The `ho_insert`, `ho_select`, `ho_update`, `ho_delete` methods.
 
 These methods trigger their corresponding SQL querie on the database. 
 For debugging purposes, you can print the SQL query built 
-by half_orm when the DML method is invoked using the _ho_mogrify() method.
+by half_orm when the DML method is invoked using the ho_mogrify() method.
 
 ```py
-people._ho_mogrify()
-people._ho_select()
+people.ho_mogrify()
+people.ho_select()
 ```
 
-## _ho_insert
-To insert a tuple in the relation, use the `_ho_insert` method as shown below:
+## ho_insert
+To insert a tuple in the relation, use the `ho_insert` method as shown below:
 ```python
-Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28')._ho_insert()
+Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28').ho_insert()
 ```
 
-By default, `_ho_insert` returns the inserted row as a dict:
+By default, `ho_insert` returns the inserted row as a dict:
 
 ```python
 lagaffe = Person(last_name='Lagaffe', first_name='Gaston', birth_date='1957-02-28')
-lagaffe_id = lagaffe._ho_insert()['id']
+lagaffe_id = lagaffe.ho_insert()['id']
 ```
 
-You can trigger a transaction for any combination of insert, modify or delete operations using the `Relation._ho_transaction` decorator.
+You can trigger a transaction for any combination of insert, modify or delete operations using the `Relation.ho_transaction` decorator.
 
 ```py
 class Person(halftest.get_relation_class('actor.person')):
     # [...]
 
     def insert_many(self, *data):
         """Insert serveral people in a single transaction."""
-        @self._ho_transaction
+        @self.ho_transaction
         def insert(self, *data):
             for d_pers in data:
-                self(**d_pers)._ho_insert()
+                self(**d_pers).ho_insert()
         insert(self, *data)
 
 ```
 
 ```python
 people = Person()
 people.insert_many(*[
@@ -346,68 +342,68 @@
 ```
 
 **Note**: half_orm works in autocommit mode by default. Without a transaction, any missing data
 would be inserted.
 
 ### Returned values
 
-By default `_ho_insert` returns all the inserted values as a dictionary. You can specify the columns
-you want to get by passing their names as argurments to `_ho_insert`.
+By default `ho_insert` returns all the inserted values as a dictionary. You can specify the columns
+you want to get by passing their names as argurments to `ho_insert`.
 
-## _ho_select
-The `_ho_select` method is a generator. It returns all the data of the relation that matches the constraint defined on the Relation object.
+## ho_select
+The `ho_select` method is a generator. It returns all the data of the relation that matches the constraint defined on the Relation object.
 The data is returned in a list of `dict`s.
 
 ```python
 >>> people = Person()
->>> print(list(people._ho_select()))
+>>> print(list(people.ho_select()))
 [{'id': 6753, 'first_name': 'Gaston', 'last_name': 'Lagaffe', 'birth_date': datetime.date(1957, 2, 28)}, {'id': 6754, 'first_name': 'Bibi', 'last_name': 'Fricotin', 'birth_date': datetime.date(1924, 10, 5)}, {'id': 6755, 'first_name': 'Corto', 'last_name': 'Maltese', 'birth_date': datetime.date(1975, 1, 7)}, {'id': 6756, 'first_name': 'Achile', 'last_name': 'Talon', 'birth_date': datetime.date(1963, 11, 7)}, {'id': 6757, 'first_name': 'Gil', 'last_name': 'Jourdan', 'birth_date': datetime.date(1956, 9, 20)}]
 >>>
 ```
 
 You can set a limit or an offset:
 ```python
->>> people._ho_offset(1)._ho_limit(2)
->>> print(list(people)) # Relation objects are iterators. so _ho_select is optional
+>>> people.ho_offset(1).ho_limit(2)
+>>> print(list(people)) # Relation objects are iterators. so ho_select is optional
 [{'id': 6754, 'first_name': 'Bibi', 'last_name': 'Fricotin', 'birth_date': datetime.date(1924, 10, 5)}, {'id': 6755, 'first_name': 'Corto', 'last_name': 'Maltese', 'birth_date': datetime.date(1975, 1, 7)}]
 ```
 
-You can also get a subset of the attributes by passing a list of columns names to `_ho_select`:
+You can also get a subset of the attributes by passing a list of columns names to `ho_select`:
 
 ```python
->>> print(list(people._ho_select('last_name')))
+>>> print(list(people.ho_select('last_name')))
 [{'last_name': 'Lagaffe'}, {'last_name': 'Fricotin'}]
 ```
 
 **Note**: The offset and limit still apply.
 
-### Select one: the `_ho_get` method
+### Select one: the `ho_get` method
 
-The `_ho_get` method returns an Relation object whose fields are populated with the values from the corresponding row in the database.
-It raises an [ExpectedOneError](https://github.com/collorg/halfORM/blob/master/half_orm/relation_errors.py)
+The `ho_get` method returns an Relation object whose fields are populated with the values from the corresponding row in the database.
+It raises an [ExpectedOneError](https://github.com/collorg/halfORM/blob/main/half_orm/relation_errors.py)
 Exception if 0 or more than 1 rows match the intention. The returned object is a singleton (see below).
 
 ```py
-gaston = Person(last_name='Lagaffe')._ho_get()
+gaston = Person(last_name='Lagaffe').ho_get()
 ```
 
 is equivalent to
 
 ```py
 lagaffe = Person(last_name='Lagaffe')
-if lagaffe._ho_is_empty() or len(lagaffe) > 1:
+if lagaffe.ho_is_empty() or len(lagaffe) > 1:
     raise ExcpetedOneError
-gaston = Person(**next(lagaffe._ho_select()))
+gaston = Person(**next(lagaffe.ho_select()))
 gaston._ho_is_singleton = True
 ```
 
-You could use `_ho_get` to retreive the `id` of the row:
+You could use `ho_get` to retreive the `id` of the row:
 
 ```py
-gaston_id = Person(last_name='Lagaffe')._ho_get('id').id.value
+gaston_id = Person(last_name='Lagaffe').ho_get('id').id.value
 ```
 
 ### Is it a set? Is it an element of the set?
 
 Let's go back to our definition of the class `Person`. We would like to write a property that
 returns the full name of **a** person. 
 
@@ -456,107 +452,107 @@
     # [...]
     @singleton
     def do_something_else(self):
         "Needs self to be a singleton"
         ...
 
     def do_something(self):
-        for elt in self._ho_select():
+        for elt in self.ho_select():
             pers = Person(**elt)
             pers._ho_is_singleton = True # You must be pretty sure of what you're doing here. See the warning and the explanation.
             pers.do_something_else() # Warning! do_something_else won't check that pers is indeed a singleton
 ```
 
 **Warning!** By setting `_ho_is_singleton` value to `True`, you disable the check that `@singleton` would have made before executing `do_something_else`. 
 This example works for two reasons:
 
-1. `_ho_select` is called without argument ensuring that all columns are retreived from the database.
-Note: Calling `_ho_select` with columns corresponding to the primary key as arguments would also have worked;
+1. `ho_select` is called without argument ensuring that all columns are retreived from the database.
+Note: Calling `ho_select` with columns corresponding to the primary key as arguments would also have worked;
 2. The table `actor.person` has a primary key which makes it a set (ie. each element returned by select is
 indeed a singleton).
 
-## _ho_update
+## ho_update
 
 To update a subset, you first define the subset an then invoque the `ho_udpate`
 method with the new values passed as argument.
 
 ```py
 gaston = Person(first_name='Gaston')
-gaston._ho_update(birth_date='1970-01-01')
+gaston.ho_update(birth_date='1970-01-01')
 ```
 
 Let's look at how we could turn the last name into capital letters for a subset of people:
 
 ```python
 class Person(halftest.get_relation_class('actor.person')):
     # [...]
 
     def upper_last_name(self):
         "tranform last name to upper case."
-        @self._ho_transaction
+        @self.ho_transaction
         def update(self):
-            for d_pers in self._ho_select('id', 'last_name'):
+            for d_pers in self.ho_select('id', 'last_name'):
                 pers = Person(**d_pers)
-                pers._ho_update(last_name=d_pers['last_name'].upper())
+                pers.ho_update(last_name=d_pers['last_name'].upper())
         update(self)
 ```
 
-Again, we insure the atomicity of the transaction using the `Relation._ho_transaction` decorator.
+Again, we insure the atomicity of the transaction using the `Relation.ho_transaction` decorator.
 
 ```
 >>> a_pers = Person(last_name=('ilike', '_a%'))
->>> print([elt.last_name for elt in list(a_pers._ho_select())])
+>>> print([elt.last_name for elt in list(a_pers.ho_select())])
 >>> a_pers = Person(last_name = ('ilike', '_a%'))
->>> print([elt['last_name'] for elt in a_pers._ho_select('last_name')])
+>>> print([elt['last_name'] for elt in a_pers.ho_select('last_name')])
 ['Lagaffe', 'Maltese', 'Talon']
 >>> a_pers.upper_last_name()
->>> print([elt['last_name'] for elt in a_pers._ho_select('last_name')])
+>>> print([elt['last_name'] for elt in a_pers.ho_select('last_name')])
 ['LAGAFFE', 'MALTESE', 'TALON']
 ```
 
 ### Returning values
 
-To return the updated values, you can add to `_ho_update` the column names you want to get, or `*` if you want to get all the columns.
+To return the updated values, you can add to `ho_update` the column names you want to get, or `*` if you want to get all the columns.
 
 ```python
->>> gaston._ho_update('*', birth_date='1970-01-01')
+>>> gaston.ho_update('*', birth_date='1970-01-01')
 ```
 
 ### Update all data in a table
 
 If you want to update all the data in a relation, you must set the argument `update_all` to `True`. A `RuntimeError` is raised otherwise.
 
 ```py
-Person()._ho_update(birth_date='1970-01-01', update_all=True)
+Person().ho_update(birth_date='1970-01-01', update_all=True)
 ```
 
-## _ho_delete
+## ho_delete
 
-The `_ho_delete` method allows you to remove a set of elements from a table:
+The `ho_delete` method allows you to remove a set of elements from a table:
 
 ```py
 gaston = Person(first_name='Gaston')
-gaston._ho_delete()
+gaston.ho_delete()
 ```
 
 To remove every tuples from a table, you must set the argument `delete_all` to `True`. A `RuntimeError` is raised otherwise.
 
 ```python
-Person()._ho_delete(delete_all=True)
-if not Person()._ho_is_empty():
+Person().ho_delete(delete_all=True)
+if not Person().ho_is_empty():
     print('Weird! You should check your "on delete cascade".')
 ```
 Well, there is not much left after this in the `actor.person` table.
 
 ### Returning values
 
-As for `_ho_update`, to return the deleted values, you can add to `_ho_delete` the column names you want to get, or `*` if you want to get all the columns.
+As for `ho_update`, to return the deleted values, you can add to `ho_delete` the column names you want to get, or `*` if you want to get all the columns.
 
 ```python
->>> gaston._ho_delete('first_name', 'last_name', 'birth_date')
+>>> gaston.ho_delete('first_name', 'last_name', 'birth_date')
 ```
 
 # Working with foreign keys [WIP]
 
 > This is a work in progress
 
 A relational object integrates all the material necessary to process its foreign keys and the
@@ -653,40 +649,40 @@
 The Fkey class has the `set` method which allows you to constrain a foreign key with a Relation object.
 To get the comments made by Gaston, we simply constraint the `author_fk` Fkey to reference the entry corresponding to Gaston in the actor.person table. To do so, we use the `Fkey.set()` method:
 
 ```python
 gaston = Person(first_name='Gaston')
 gaston_comments = Comment()
 gaston_comments.author_fk.set(gaston)
-print(list(gaston_comments._ho_select())
+print(list(gaston_comments.ho_select())
 ```
 ## Chaining foreign keys
 
 **Important note**: Foreign key chaining will only work if the modules corresponding to the tables are ordered
 according to the names of the tables in the package. See the `hop` command.
 
 You can easily chain foreign keys. For example, if you want to get all the comments made by Gaston
 on his own posts:
 
 ```py
 gaston = {'last_name':'Lagaffe', 'first_name':'Gaston', 'birth_date':'1957-02-28'}
-gaston_id = Person(**gaston)._ho_get('id').id.value # we ensure that Gaston is a singleton
+gaston_id = Person(**gaston).ho_get('id').id.value # we ensure that Gaston is a singleton
 list(gaston
     .post_rfk(**gaston)
     .comment_rfk(author_id=gaston_id))
 ```
 
 **Note**: the `blog.post` table declares a foreign key on `actor.person(first_name, last_name, birth_date)` 
 while the `blog.comment` table declares a foreign key on `actor.person(id)`.
 
-## The *`_ho_join`* method
+## The *`ho_join`* method
 
-The *`_ho_join`* method allows you to integrate the data associated with a Relation object into the result obtained by the *`select`* method by using foreign keys of the object or by referencing the object.
+The *`ho_join`* method allows you to integrate the data associated with a Relation object into the result obtained by the *`select`* method by using foreign keys of the object or by referencing the object.
 
-Unlike the *`select`* method (which is a generator), the *`_ho_join`* method returns a list.
+Unlike the *`select`* method (which is a generator), the *`ho_join`* method returns a list.
 
 It takes a list of tuples each with two or three elements:
 
 * a remote Relation object that must be accessible by a foreign key (direct or "reverse");
 * the name of the key under which the associated data would be stored;
 * an optional list of columns (`str[]`) or the name of a column (`str`) to be retreived from the
   remote object.
@@ -694,15 +690,15 @@
   If the third argument is omitted, all columns are retreived.
 
 For example, the following code would return the list of people named `Lagaffe` with two
 additional attributes (`comments` and `posts`):
 
 ```#python
 lagaffe = Person(last_name='Lagaffe')
-res = lagaffe._ho_join(
+res = lagaffe.ho_join(
     (Comment(), 'comments', ['id', 'post_id']),
     (Post(), 'posts', 'id')
 )
 ```
 
 * The data associated with `comments` is a list of dictionaries whose keys are 'id' and 'post_id'.
 * The data associated  with  `posts` is a simple list of values corresponding to the 'id' column.
@@ -738,14 +734,14 @@
 
 By the way, this is the code used in the `Model.ping` method that makes sure the connection is established and attempts a reconnection if it is not.
 
 That's it! You've learn pretty much everything there is to know about `half_orm`.
 
 # Next: `hop`, the GitOps `half_orm` packager [WIP][alpha]
 
-The `hop` command, directly provided in this package (from version 0.8.0rc1), allows you to ***create*** a Python package corresponding to the model of your database, to ***patch*** the model and the corresponding Python code, to ***test*** your database model and your business code.
+The [`hop`](https://github.com/collorg/halfORM/blob/main/doc/hop.md) command, directly provided in this package (from version 0.8.0rc1), allows you to ***create*** a Python package corresponding to the model of your database, to ***patch*** the model and the corresponding Python code, to ***test*** your database model and your business code.
 
-No documentation at the moment, but you can check the idea with the [test script](https://github.com/collorg/halfORM/blob/master/half_orm/packager/test/dummy_test.sh).
+* More at https://github.com/collorg/halfORM/blob/main/doc/hop.md
 
 # Want to contribute?
 
 Fork me on Github: https://github.com/collorg/halfORM
```

### Comparing `half_orm-0.8.0rc9/half_orm.egg-info/SOURCES.txt` & `half_orm-0.9.0/half_orm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 half_orm/hotest.py
 half_orm/model.py
 half_orm/model_errors.py
 half_orm/null.py
 half_orm/pg_meta.py
 half_orm/relation.py
 half_orm/relation_errors.py
+half_orm/relation_factory.py
 half_orm/transaction.py
 half_orm/version.txt
 half_orm.egg-info/PKG-INFO
 half_orm.egg-info/SOURCES.txt
 half_orm.egg-info/dependency_links.txt
 half_orm.egg-info/entry_points.txt
 half_orm.egg-info/requires.txt
```

### Comparing `half_orm-0.8.0rc9/setup.py` & `half_orm-0.9.0/setup.py`

 * *Files identical despite different names*


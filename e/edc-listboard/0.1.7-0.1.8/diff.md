# Comparing `tmp/edc-listboard-0.1.7.tar.gz` & `tmp/edc-listboard-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-listboard-0.1.7.tar", last modified: Wed Jan 25 02:37:54 2023, max compression
+gzip compressed data, was "edc-listboard-0.1.8.tar", last modified: Fri May 12 04:32:31 2023, max compression
```

## Comparing `edc-listboard-0.1.7.tar` & `edc-listboard-0.1.8.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 02:37:54.466524 edc-listboard-0.1.7/
--rw-r--r--   0 erikvw     (501) staff       (20)       99 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/.coveragrc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 02:37:54.454053 edc-listboard-0.1.7/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 02:37:54.458284 edc-listboard-0.1.7/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1934 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1821 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1075 2022-09-15 01:52:48.000000 edc-listboard-0.1.7/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       22 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-08-23 20:00:32.000000 edc-listboard-0.1.7/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1029 2023-01-25 02:37:54.466612 edc-listboard-0.1.7/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)       40 2022-08-25 03:17:45.000000 edc-listboard-0.1.7/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-09-26 00:16:33.000000 edc-listboard-0.1.7/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 02:37:54.459274 edc-listboard-0.1.7/edc_listboard/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      348 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      174 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/dashboard_templates.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 02:37:54.460496 edc-listboard-0.1.7/edc_listboard/filters/
--rw-r--r--   0 erikvw     (501) staff       (20)      103 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/filters/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1093 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/filters/listboard_filter.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1566 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/filters/listboard_view_filters.py
--rw-r--r--   0 erikvw     (501) staff       (20)      853 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/middleware.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 02:37:54.460780 edc-listboard-0.1.7/edc_listboard/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)     3713 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      299 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)      397 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/system_checks.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 02:37:54.454477 edc-listboard-0.1.7/edc_listboard/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 02:37:54.454542 edc-listboard-0.1.7/edc_listboard/templates/edc_listboard/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 02:37:54.460880 edc-listboard-0.1.7/edc_listboard/templates/edc_listboard/bootstrap3/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 02:37:54.461556 edc-listboard-0.1.7/edc_listboard/templates/edc_listboard/bootstrap3/include/
--rw-r--r--   0 erikvw     (501) staff       (20)     1244 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/templates/edc_listboard/bootstrap3/include/buttons_column.html
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/templates/edc_listboard/bootstrap3/include/columns.html
--rw-r--r--   0 erikvw     (501) staff       (20)      297 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/templates/edc_listboard/bootstrap3/include/results_body.html
--rw-r--r--   0 erikvw     (501) staff       (20)      197 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/templates/edc_listboard/bootstrap3/include/results_header.html
--rw-r--r--   0 erikvw     (501) staff       (20)     2549 2022-11-17 00:02:13.000000 edc-listboard-0.1.7/edc_listboard/templates/edc_listboard/bootstrap3/listboard.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 02:37:54.462073 edc-listboard-0.1.7/edc_listboard/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      457 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/tests/admin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 02:37:54.463393 edc-listboard-0.1.7/edc_listboard/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      113 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/tests/etc/django_crypto_fields
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1119 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 02:37:54.463621 edc-listboard-0.1.7/edc_listboard/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4469 2022-09-15 01:52:48.000000 edc-listboard-0.1.7/edc_listboard/tests/tests/test_view_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      928 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      173 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 02:37:54.465089 edc-listboard-0.1.7/edc_listboard/view_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      301 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/view_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2645 2022-09-26 00:16:33.000000 edc-listboard-0.1.7/edc_listboard/view_mixins/listboard_filter_view_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      924 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/view_mixins/querystring_view_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1152 2022-09-26 00:16:33.000000 edc-listboard-0.1.7/edc_listboard/view_mixins/search_form_view_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3316 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/view_mixins/search_listboard_view_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      254 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/view_mixins/site_queryset_view_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 02:37:54.465464 edc-listboard-0.1.7/edc_listboard/views/
--rw-r--r--   0 erikvw     (501) staff       (20)      127 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/views/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9546 2022-09-26 00:16:00.000000 edc-listboard-0.1.7/edc_listboard/views/listboard_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 02:37:54.466004 edc-listboard-0.1.7/edc_listboard/views/screen/
--rw-r--r--   0 erikvw     (501) staff       (20)      105 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/views/screen/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      678 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/views/screen/listboard_view_filter.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2581 2022-08-26 02:01:49.000000 edc-listboard-0.1.7/edc_listboard/views/screen/screening_listboard_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 02:37:54.466406 edc-listboard-0.1.7/edc_listboard/views/subject/
--rw-r--r--   0 erikvw     (501) staff       (20)       57 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/edc_listboard/views/subject/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2154 2023-01-25 02:37:46.000000 edc-listboard-0.1.7/edc_listboard/views/subject/subject_listboard_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-01-25 02:37:54.460055 edc-listboard-0.1.7/edc_listboard.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1029 2023-01-25 02:37:54.000000 edc-listboard-0.1.7/edc_listboard.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     2404 2023-01-25 02:37:54.000000 edc-listboard-0.1.7/edc_listboard.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-01-25 02:37:54.000000 edc-listboard-0.1.7/edc_listboard.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-23 20:16:36.000000 edc-listboard-0.1.7/edc_listboard.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       14 2023-01-25 02:37:54.000000 edc-listboard-0.1.7/edc_listboard.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1729 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1856 2022-08-25 03:16:05.000000 edc-listboard-0.1.7/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1248 2023-01-25 02:37:54.466945 edc-listboard-0.1.7/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.763881 edc-listboard-0.1.8/
+-rw-r--r--   0 erikvw     (501) staff       (20)       99 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/.coveragrc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.748431 edc-listboard-0.1.8/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.752426 edc-listboard-0.1.8/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1934 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1821 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-05-12 04:32:24.000000 edc-listboard-0.1.8/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-08-23 20:00:32.000000 edc-listboard-0.1.8/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)      902 2023-05-12 04:32:31.763967 edc-listboard-0.1.8/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)       40 2022-08-25 03:17:45.000000 edc-listboard-0.1.8/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-09-26 00:16:33.000000 edc-listboard-0.1.8/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.753416 edc-listboard-0.1.8/edc_listboard/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      348 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      174 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/dashboard_templates.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.755675 edc-listboard-0.1.8/edc_listboard/filters/
+-rw-r--r--   0 erikvw     (501) staff       (20)      103 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/filters/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1093 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/filters/listboard_filter.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1566 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/filters/listboard_view_filters.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      853 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/middleware.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.756022 edc-listboard-0.1.8/edc_listboard/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)     3713 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      299 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      397 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/system_checks.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.748844 edc-listboard-0.1.8/edc_listboard/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.748895 edc-listboard-0.1.8/edc_listboard/templates/edc_listboard/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.756124 edc-listboard-0.1.8/edc_listboard/templates/edc_listboard/bootstrap3/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.756857 edc-listboard-0.1.8/edc_listboard/templates/edc_listboard/bootstrap3/include/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1244 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/templates/edc_listboard/bootstrap3/include/buttons_column.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/templates/edc_listboard/bootstrap3/include/columns.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      297 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/templates/edc_listboard/bootstrap3/include/results_body.html
+-rw-r--r--   0 erikvw     (501) staff       (20)      197 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/templates/edc_listboard/bootstrap3/include/results_header.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     2549 2022-11-17 00:02:13.000000 edc-listboard-0.1.8/edc_listboard/templates/edc_listboard/bootstrap3/listboard.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.757441 edc-listboard-0.1.8/edc_listboard/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      457 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/admin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.758758 edc-listboard-0.1.8/edc_listboard/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      113 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/etc/django_crypto_fields
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1119 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.758990 edc-listboard-0.1.8/edc_listboard/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4469 2022-09-15 01:52:48.000000 edc-listboard-0.1.8/edc_listboard/tests/tests/test_view_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      928 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      173 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.760026 edc-listboard-0.1.8/edc_listboard/view_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      301 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/view_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2645 2022-09-26 00:16:33.000000 edc-listboard-0.1.8/edc_listboard/view_mixins/listboard_filter_view_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      924 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/view_mixins/querystring_view_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1152 2022-09-26 00:16:33.000000 edc-listboard-0.1.8/edc_listboard/view_mixins/search_form_view_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3316 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/view_mixins/search_listboard_view_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      254 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/view_mixins/site_queryset_view_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.760334 edc-listboard-0.1.8/edc_listboard/views/
+-rw-r--r--   0 erikvw     (501) staff       (20)      127 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/views/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9546 2022-09-26 00:16:00.000000 edc-listboard-0.1.8/edc_listboard/views/listboard_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.762330 edc-listboard-0.1.8/edc_listboard/views/screen/
+-rw-r--r--   0 erikvw     (501) staff       (20)      105 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/views/screen/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      678 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/views/screen/listboard_view_filter.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2581 2022-08-26 02:01:49.000000 edc-listboard-0.1.8/edc_listboard/views/screen/screening_listboard_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.763772 edc-listboard-0.1.8/edc_listboard/views/subject/
+-rw-r--r--   0 erikvw     (501) staff       (20)       57 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/edc_listboard/views/subject/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2246 2023-05-12 04:32:24.000000 edc-listboard-0.1.8/edc_listboard/views/subject/subject_listboard_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:32:31.755129 edc-listboard-0.1.8/edc_listboard.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)      902 2023-05-12 04:32:31.000000 edc-listboard-0.1.8/edc_listboard.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     2404 2023-05-12 04:32:31.000000 edc-listboard-0.1.8/edc_listboard.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-12 04:32:31.000000 edc-listboard-0.1.8/edc_listboard.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-23 20:16:36.000000 edc-listboard-0.1.8/edc_listboard.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       14 2023-05-12 04:32:31.000000 edc-listboard-0.1.8/edc_listboard.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1709 2023-05-12 04:32:24.000000 edc-listboard-0.1.8/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1856 2022-08-25 03:16:05.000000 edc-listboard-0.1.8/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1154 2023-05-12 04:32:31.764290 edc-listboard-0.1.8/setup.cfg
```

### Comparing `edc-listboard-0.1.7/.github/workflows/build.yml` & `edc-listboard-0.1.8/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.7/.gitignore` & `edc-listboard-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.7/.pre-commit-config.yaml` & `edc-listboard-0.1.8/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 ---
 exclude: tests/etc/user-*
+
 repos:
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.7.4
+    rev: 1.7.5
     hooks:
       - id: bandit
         args:
           - "-x *test*.py"
 
   - repo: https://github.com/psf/black
-    rev: 22.6.0
+    rev: 23.1.0
     hooks:
       - id: black
         language_version: python3.9
 
   - repo: https://github.com/pycqa/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
       - id: flake8
         args:
           - "--config=setup.cfg"
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: requirements-txt-fixer
         files: requirements/.*\.txt$
       - id: trailing-whitespace
       - id: check-added-large-files
       - id: fix-byte-order-marker
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: debug-statements
       - id: detect-private-key
 
   - repo: https://github.com/adrienverge/yamllint
-    rev: v1.27.1
+    rev: v1.30.0
     hooks:
       - id: yamllint
         args:
           - "--strict"
```

### Comparing `edc-listboard-0.1.7/LICENSE` & `edc-listboard-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.7/PKG-INFO` & `edc-listboard-0.1.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 Metadata-Version: 2.1
 Name: edc-listboard
-Version: 0.1.7
+Version: 0.1.8
 Summary: Classes for Listboard views in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-listboard
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc listboard,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 # edc-listboard
```

### Comparing `edc-listboard-0.1.7/edc_listboard/filters/listboard_filter.py` & `edc-listboard-0.1.8/edc_listboard/filters/listboard_filter.py`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.7/edc_listboard/filters/listboard_view_filters.py` & `edc-listboard-0.1.8/edc_listboard/filters/listboard_view_filters.py`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.7/edc_listboard/middleware.py` & `edc-listboard-0.1.8/edc_listboard/middleware.py`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.7/edc_listboard/migrations/0001_initial.py` & `edc-listboard-0.1.8/edc_listboard/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.7/edc_listboard/templates/edc_listboard/bootstrap3/include/buttons_column.html` & `edc-listboard-0.1.8/edc_listboard/templates/edc_listboard/bootstrap3/include/buttons_column.html`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.7/edc_listboard/templates/edc_listboard/bootstrap3/listboard.html` & `edc-listboard-0.1.8/edc_listboard/templates/edc_listboard/bootstrap3/listboard.html`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.7/edc_listboard/tests/etc/user-rsa-local-private.pem` & `edc-listboard-0.1.8/edc_listboard/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.7/edc_listboard/tests/etc/user-rsa-restricted-private.pem` & `edc-listboard-0.1.8/edc_listboard/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.7/edc_listboard/tests/models.py` & `edc-listboard-0.1.8/edc_listboard/tests/models.py`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.7/edc_listboard/tests/tests/test_view_mixins.py` & `edc-listboard-0.1.8/edc_listboard/tests/tests/test_view_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.7/edc_listboard/tests/urls.py` & `edc-listboard-0.1.8/edc_listboard/tests/urls.py`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.7/edc_listboard/view_mixins/listboard_filter_view_mixin.py` & `edc-listboard-0.1.8/edc_listboard/view_mixins/listboard_filter_view_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.7/edc_listboard/view_mixins/querystring_view_mixin.py` & `edc-listboard-0.1.8/edc_listboard/view_mixins/querystring_view_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.7/edc_listboard/view_mixins/search_form_view_mixin.py` & `edc-listboard-0.1.8/edc_listboard/view_mixins/search_form_view_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.7/edc_listboard/view_mixins/search_listboard_view_mixin.py` & `edc-listboard-0.1.8/edc_listboard/view_mixins/search_listboard_view_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.7/edc_listboard/views/listboard_view.py` & `edc-listboard-0.1.8/edc_listboard/views/listboard_view.py`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.7/edc_listboard/views/screen/listboard_view_filter.py` & `edc-listboard-0.1.8/edc_listboard/views/screen/listboard_view_filter.py`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.7/edc_listboard/views/screen/screening_listboard_view.py` & `edc-listboard-0.1.8/edc_listboard/views/screen/screening_listboard_view.py`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.7/edc_listboard/views/subject/subject_listboard_view.py` & `edc-listboard-0.1.8/edc_listboard/views/subject/subject_listboard_view.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 class SubjectListboardView(
     EdcViewMixin,
     NavbarViewMixin,
     ListboardFilterViewMixin,
     SearchFormViewMixin,
     ListboardView,
 ):
-
     listboard_model = get_consent_model_name()
     model_wrapper_cls = SubjectConsentModelWrapper
 
     listboard_template = "subject_listboard_template"
     listboard_url = "subject_listboard_url"
     listboard_panel_style = "success"
     listboard_fa_icon = "fas fa-user-circle fa-2x"
     listboard_view_permission_codename = "edc_subject_dashboard.view_subject_listboard"
 
     navbar_selected_item = "consented_subject"
     search_form_url = "subject_listboard_url"
 
     name_search_field: str = "first_name"
     identity_regex: str = r"^[0-9]+$"
+    identity_fields = ["identity"]
 
     def get_queryset_filter_options(self, request, *args, **kwargs):
         options = super().get_queryset_filter_options(request, *args, **kwargs)
         if kwargs.get("subject_identifier"):
             options.update({"subject_identifier": kwargs.get("subject_identifier")})
         return options
 
@@ -49,9 +49,10 @@
             q_objects.append(Q(initials__exact=search_term.upper()))
             q_objects.append(Q(**{f"{self.name_search_field}__exact": search_term.upper()}))
             q_objects.append(
                 Q(screening_identifier__icontains=search_term.replace("-", "").upper())
             )
             q_objects.append(Q(subject_identifier__icontains=search_term))
         if re.match(self.identity_regex, search_term):
-            q_objects.append(Q(identity__exact=search_term))
+            for field in self.identity_fields:
+                q_objects.append(Q(**{f"{field}__exact": search_term}))
         return q_objects
```

### Comparing `edc-listboard-0.1.7/edc_listboard.egg-info/PKG-INFO` & `edc-listboard-0.1.8/edc_listboard.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 Metadata-Version: 2.1
 Name: edc-listboard
-Version: 0.1.7
+Version: 0.1.8
 Summary: Classes for Listboard views in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-listboard
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc listboard,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 # edc-listboard
```

### Comparing `edc-listboard-0.1.7/edc_listboard.egg-info/SOURCES.txt` & `edc-listboard-0.1.8/edc_listboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.7/pyproject.toml` & `edc-listboard-0.1.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,70 +3,69 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "_version.py"
 
 [tool.black]
 line-length = 95
-target-version = ["py39"]
+target-version = ["py310"]
 extend-exclude = '''^(.*\/)*\b(migrations)\b($|\/.*$)'''
 
 [tool.isort]
 profile = "black"
-py_version = "39"
+py_version = "310"
 skip = [".tox", ".eggs", "migrations"]
 
 [tool.coverage.run]
 parallel = false
 branch = true
 source = ["edc_listboard"]
 
 [tool.coverage.paths]
 source = ["edc_listboard"]
 
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 omit = ["requirements.txt"]
+exclude_lines = [
+  "pragma: no cover",
+  "if TYPE_CHECKING:",
+]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
-    py{38,39,310}-dj{32,40,41,dev},
+    py{310,311}-dj{41,dev},
     lint
 
 isolated_build = true
 
 [gh-actions]
 python =
-    3.8: py38
-    3.9: py39, lint
     3.10: py310
+    3.11: py311, lint
 
 [gh-actions:env]
 DJANGO =
-    3.2: dj32, lint
-    4.0: dj40
-    4.1: dj41
+    4.1: dj41, lint
     dev: djdev
 
 [testenv]
 deps =
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/tox.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/test_utils.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/edc.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/third_party_dev.txt
-    dj32: Django>=3.2,<3.3
-    dj40: Django>=4.0,<4.1
     dj41: Django>=4.1,<4.2
     djdev: https://github.com/django/django/tarball/main
 
 commands =
-    pip install -U pip
+    pip install -U pip coverage[toml]
     pip --version
     pip freeze
     coverage run -a runtests.py
     coverage report
 
 [testenv:lint]
 deps = -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/lint.txt
```

### Comparing `edc-listboard-0.1.7/runtests.py` & `edc-listboard-0.1.8/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-listboard-0.1.7/setup.cfg` & `edc-listboard-0.1.8/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -8,23 +8,20 @@
 description = Classes for Listboard views in clinicedc/edc projects
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = django edc listboard, clinicedc, clinical trials
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
-	Framework :: Django :: 3.2
-	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 
 [options]
 python_requires = >=3.9
 zip_safe = False
 include_package_data = True
 packages = find:
```


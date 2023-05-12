# Comparing `tmp/microcosm-flask-4.1.1.tar.gz` & `tmp/microcosm-flask-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/microcosm-flask-4.1.1.tar", last modified: Mon Nov  7 17:00:35 2022, max compression
+gzip compressed data, was "dist/microcosm-flask-4.1.3.tar", last modified: Fri May 12 08:36:37 2023, max compression
```

## Comparing `microcosm-flask-4.1.1.tar` & `microcosm-flask-4.1.3.tar`

### file list

```diff
@@ -1,106 +1,107 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-07 17:00:35.000000 microcosm-flask-4.1.1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1936 2022-11-07 17:00:35.000000 microcosm-flask-4.1.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1419 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-07 17:00:35.000000 microcosm-flask-4.1.1/microcosm_flask/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11307 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/audit.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2116 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/basic_auth.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2468 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/cloning.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      961 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/context.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-07 17:00:35.000000 microcosm-flask-4.1.1/microcosm_flask/conventions/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/conventions/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1872 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/conventions/alias.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5085 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/conventions/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1858 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/conventions/build_info.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1053 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/conventions/catchall.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2208 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/conventions/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16621 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/conventions/crud.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2512 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/conventions/crud_adapter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2607 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/conventions/discovery.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5793 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/conventions/encoding.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4126 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/conventions/health.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3595 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/conventions/landing.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3201 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/conventions/logging_level.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4056 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/conventions/registry.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10430 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/conventions/relation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2427 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/conventions/saved_search.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2926 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/conventions/swagger.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4402 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/conventions/upload.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      178 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/converters.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-07 17:00:35.000000 microcosm-flask-4.1.1/microcosm_flask/decorators/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/decorators/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1022 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/decorators/logging.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3978 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/decorators/schemas.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-07 17:00:35.000000 microcosm-flask-4.1.1/microcosm_flask/encryption/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/encryption/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-07 17:00:35.000000 microcosm-flask-4.1.1/microcosm_flask/encryption/conventions/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/encryption/conventions/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1330 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/encryption/conventions/crud_adapter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1660 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/enums.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4697 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/errors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1039 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/factories.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-07 17:00:35.000000 microcosm-flask-4.1.1/microcosm_flask/fields/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      479 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/fields/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      460 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/fields/cleaned_field.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1734 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/fields/enum_field.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      860 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/fields/language_field.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1044 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/fields/query_string_list.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1589 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/fields/timestamp_field.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1979 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/fields/uri_field.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-07 17:00:35.000000 microcosm-flask-4.1.1/microcosm_flask/formatting/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      302 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/formatting/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1945 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/formatting/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2790 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/formatting/csv_formatter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       40 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/formatting/encoding.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      280 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/formatting/html_formatter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      331 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/formatting/json_formatter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      281 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/formatting/text_formatter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1932 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/forwarding.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3224 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/linking.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2196 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/matchers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2094 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/memory.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1422 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/metrics.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      995 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/metrics_classifier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5852 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/namespaces.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1508 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/naming.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3019 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/operations.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10233 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/paging.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      781 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/paths.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1387 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/profiling.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2965 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/routing.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      903 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/runserver.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2259 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/sentry.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1046 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/session.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-07 17:00:35.000000 microcosm-flask-4.1.1/microcosm_flask/swagger/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/swagger/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1095 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/swagger/api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      545 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/swagger/decorators.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12939 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/swagger/definitions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      879 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/swagger/naming.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-07 17:00:35.000000 microcosm-flask-4.1.1/microcosm_flask/swagger/parameters/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1917 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/swagger/parameters/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2904 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/swagger/parameters/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      889 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/swagger/parameters/decorated.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1965 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/swagger/parameters/default.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2271 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/swagger/parameters/enum.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      627 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/swagger/parameters/list.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      726 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/swagger/parameters/nested.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      588 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/swagger/parameters/numeric.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      708 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/swagger/parameters/timestamp.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3108 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/swagger/schemas.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-07 17:00:35.000000 microcosm-flask-4.1.1/microcosm_flask/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/templates/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3703 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/templates/landing.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1830 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/microcosm_flask/templates/swagger_ui.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-07 17:00:35.000000 microcosm-flask-4.1.1/microcosm_flask.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1936 2022-11-07 17:00:35.000000 microcosm-flask-4.1.1/microcosm_flask.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3301 2022-11-07 17:00:35.000000 microcosm-flask-4.1.1/microcosm_flask.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-11-07 17:00:35.000000 microcosm-flask-4.1.1/microcosm_flask.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1830 2022-11-07 17:00:35.000000 microcosm-flask-4.1.1/microcosm_flask.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-11-07 17:00:35.000000 microcosm-flask-4.1.1/microcosm_flask.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      486 2022-11-07 17:00:35.000000 microcosm-flask-4.1.1/microcosm_flask.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       16 2022-11-07 17:00:35.000000 microcosm-flask-4.1.1/microcosm_flask.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      761 2022-11-07 17:00:35.000000 microcosm-flask-4.1.1/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4003 2022-11-07 16:56:30.000000 microcosm-flask-4.1.1/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-12 08:36:37.000000 microcosm-flask-4.1.3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1936 2023-05-12 08:36:37.000000 microcosm-flask-4.1.3/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1419 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-12 08:36:37.000000 microcosm-flask-4.1.3/microcosm_flask/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11307 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/audit.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2116 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/basic_auth.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2483 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/cloning.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      961 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/context.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-12 08:36:37.000000 microcosm-flask-4.1.3/microcosm_flask/conventions/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/conventions/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1872 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/conventions/alias.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5085 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/conventions/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1858 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/conventions/build_info.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1053 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/conventions/catchall.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2208 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/conventions/config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16621 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/conventions/crud.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2512 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/conventions/crud_adapter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2607 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/conventions/discovery.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5793 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/conventions/encoding.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4681 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/conventions/health.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3595 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/conventions/landing.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3201 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/conventions/logging_level.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4056 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/conventions/registry.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10430 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/conventions/relation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2427 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/conventions/saved_search.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2926 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/conventions/swagger.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4402 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/conventions/upload.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      178 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/converters.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-12 08:36:37.000000 microcosm-flask-4.1.3/microcosm_flask/decorators/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/decorators/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1022 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/decorators/logging.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3978 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/decorators/schemas.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-12 08:36:37.000000 microcosm-flask-4.1.3/microcosm_flask/encryption/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/encryption/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-12 08:36:37.000000 microcosm-flask-4.1.3/microcosm_flask/encryption/conventions/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/encryption/conventions/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1330 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/encryption/conventions/crud_adapter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1660 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/enums.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4712 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/errors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1039 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/factories.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-12 08:36:37.000000 microcosm-flask-4.1.3/microcosm_flask/fields/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      479 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/fields/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      460 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/fields/cleaned_field.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1734 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/fields/enum_field.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      860 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/fields/language_field.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1044 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/fields/query_string_list.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1589 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/fields/timestamp_field.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1979 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/fields/uri_field.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-12 08:36:37.000000 microcosm-flask-4.1.3/microcosm_flask/formatting/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      302 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/formatting/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1945 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/formatting/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2790 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/formatting/csv_formatter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       40 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/formatting/encoding.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      280 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/formatting/html_formatter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      331 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/formatting/json_formatter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      281 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/formatting/text_formatter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1932 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/forwarding.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3224 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/linking.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2196 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/matchers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2094 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/memory.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1422 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/metrics.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      995 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/metrics_classifier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5852 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/namespaces.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1508 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/naming.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3019 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/operations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10244 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/paging.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      781 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/paths.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1387 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/profiling.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2965 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/routing.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      903 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/runserver.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2259 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/sentry.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1046 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/session.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-12 08:36:37.000000 microcosm-flask-4.1.3/microcosm_flask/swagger/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/swagger/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1095 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/swagger/api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      545 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/swagger/decorators.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12939 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/swagger/definitions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      879 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/swagger/naming.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-12 08:36:37.000000 microcosm-flask-4.1.3/microcosm_flask/swagger/parameters/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1917 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/swagger/parameters/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2904 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/swagger/parameters/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      921 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/swagger/parameters/constant.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      889 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/swagger/parameters/decorated.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2013 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/swagger/parameters/default.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2271 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/swagger/parameters/enum.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      627 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/swagger/parameters/list.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      726 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/swagger/parameters/nested.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      588 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/swagger/parameters/numeric.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      708 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/swagger/parameters/timestamp.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3108 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/swagger/schemas.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-12 08:36:37.000000 microcosm-flask-4.1.3/microcosm_flask/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/templates/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3703 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/templates/landing.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1830 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/microcosm_flask/templates/swagger_ui.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-12 08:36:37.000000 microcosm-flask-4.1.3/microcosm_flask.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1936 2023-05-12 08:36:36.000000 microcosm-flask-4.1.3/microcosm_flask.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3348 2023-05-12 08:36:36.000000 microcosm-flask-4.1.3/microcosm_flask.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-12 08:36:36.000000 microcosm-flask-4.1.3/microcosm_flask.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1910 2023-05-12 08:36:36.000000 microcosm-flask-4.1.3/microcosm_flask.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-12 08:36:36.000000 microcosm-flask-4.1.3/microcosm_flask.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      486 2023-05-12 08:36:36.000000 microcosm-flask-4.1.3/microcosm_flask.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       16 2023-05-12 08:36:36.000000 microcosm-flask-4.1.3/microcosm_flask.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      761 2023-05-12 08:36:37.000000 microcosm-flask-4.1.3/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4098 2023-05-12 08:33:31.000000 microcosm-flask-4.1.3/setup.py
```

### Comparing `microcosm-flask-4.1.1/LICENSE` & `microcosm-flask-4.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/PKG-INFO` & `microcosm-flask-4.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcosm-flask
-Version: 4.1.1
+Version: 4.1.3
 Summary: Opinionated persistence with FlaskQL
 Home-page: https://github.com/globality-corp/microcosm-flask
 Author: Globality Engineering
 Author-email: engineering@globality.com
 License: UNKNOWN
 Keywords: microcosm
 Platform: UNKNOWN
```

### Comparing `microcosm-flask-4.1.1/README.md` & `microcosm-flask-4.1.3/README.md`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/audit.py` & `microcosm-flask-4.1.3/microcosm_flask/audit.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/basic_auth.py` & `microcosm-flask-4.1.3/microcosm_flask/basic_auth.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/cloning.py` & `microcosm-flask-4.1.3/microcosm_flask/cloning.py`

 * *Files 21% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     )
     edges = fields.List(
         fields.Nested(EdgeSchema),
         required=True,
     )
     substitutions = fields.List(
         fields.Nested(SubstitutionSchema),
-        missing=[],
+        load_default=[],
         required=False,
     )
 
     @pre_dump
     def unflatten(self, obj, **kwargs):
         """
         Translate substitutions dictionary into objects.
@@ -76,20 +76,20 @@
             for key, value in getattr(obj, "substitutions", {}).items()
         ]
         return obj
 
 
 class NewCloneSchema(Schema):
     commit = fields.Boolean(
-        missing=True,
+        load_default=True,
         required=False,
     )
     substitutions = fields.List(
         fields.Nested(SubstitutionSchema),
-        missing=[],
+        load_default=[],
         required=False,
     )
 
     @post_load
     def flatten(self, obj, **kwargs):
         """
         Translate substitutions into a dictionary.
```

### Comparing `microcosm-flask-4.1.1/microcosm_flask/context.py` & `microcosm-flask-4.1.3/microcosm_flask/context.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/conventions/alias.py` & `microcosm-flask-4.1.3/microcosm_flask/conventions/alias.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/conventions/base.py` & `microcosm-flask-4.1.3/microcosm_flask/conventions/base.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/conventions/build_info.py` & `microcosm-flask-4.1.3/microcosm_flask/conventions/build_info.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/conventions/catchall.py` & `microcosm-flask-4.1.3/microcosm_flask/conventions/catchall.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/conventions/config.py` & `microcosm-flask-4.1.3/microcosm_flask/conventions/config.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/conventions/crud.py` & `microcosm-flask-4.1.3/microcosm_flask/conventions/crud.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/conventions/crud_adapter.py` & `microcosm-flask-4.1.3/microcosm_flask/conventions/crud_adapter.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/conventions/discovery.py` & `microcosm-flask-4.1.3/microcosm_flask/conventions/discovery.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/conventions/encoding.py` & `microcosm-flask-4.1.3/microcosm_flask/conventions/encoding.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/conventions/health.py` & `microcosm-flask-4.1.3/microcosm_flask/conventions/health.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 Health check convention.
 
 Reports service health and basic information from the "/api/health" endpoint,
 using HTTP 200/503 status codes to indicate healthiness.
 
 """
 from distutils.util import strtobool
+from functools import wraps
 from itertools import chain
+from logging import Logger
 from typing import Any, Dict
 
 from marshmallow import Schema, fields
 from microcosm.api import defaults
 
 from microcosm_flask.audit import skip_logging
 from microcosm_flask.conventions.base import Convention
@@ -56,39 +58,59 @@
 
     May contain zero or more "checks" which are just callables that take the
     current object graph as input.
 
     The overall health is OK if all checks are OK.
 
     """
+
     def __init__(self, graph, include_build_info=True):
         self.graph = graph
         self.name = graph.metadata.name
         self.optional_checks = dict()
         self.checks = dict()
+        self.logger: Logger = graph.logger
 
         if include_build_info:
-            self.checks.update(dict(
-                build_num=BuildInfo.check_build_num,
-                sha1=BuildInfo.check_sha1,
-            ))
+            self.checks.update(
+                dict(
+                    build_num=BuildInfo.check_build_num,
+                    sha1=BuildInfo.check_sha1,
+                )
+            )
+
+    def log_error(self, func):
+        """
+        Decorator to wrap a check function in error logging.
+
+        """
+
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            try:
+                return func(*args, **kwargs)
+            except Exception as error:
+                self.logger.exception("Exception in health check")
+                raise error
+
+        return wrapper
 
     def to_dict(self, full=None) -> Dict[str, Any]:
         """
         Encode the name, the status of all checks, and the current overall status.
 
         """
         if full:
             checks = chain(self.checks.items(), self.optional_checks.items())
         else:
             checks = self.checks.items()
 
         # evaluate checks
         check_results: Dict[str, HealthResult] = {
-            key: HealthResult.evaluate(func, self.graph)
+            key: HealthResult.evaluate(self.log_error(func), self.graph)
             for key, func in checks
         }
 
         dct = dict(
             # return the service name helps for routing debugging
             name=self.name,
             ok=all(check_results.values()),
```

### Comparing `microcosm-flask-4.1.1/microcosm_flask/conventions/landing.py` & `microcosm-flask-4.1.3/microcosm_flask/conventions/landing.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/conventions/logging_level.py` & `microcosm-flask-4.1.3/microcosm_flask/conventions/logging_level.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/conventions/registry.py` & `microcosm-flask-4.1.3/microcosm_flask/conventions/registry.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/conventions/relation.py` & `microcosm-flask-4.1.3/microcosm_flask/conventions/relation.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/conventions/saved_search.py` & `microcosm-flask-4.1.3/microcosm_flask/conventions/saved_search.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/conventions/swagger.py` & `microcosm-flask-4.1.3/microcosm_flask/conventions/swagger.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/conventions/upload.py` & `microcosm-flask-4.1.3/microcosm_flask/conventions/upload.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/decorators/logging.py` & `microcosm-flask-4.1.3/microcosm_flask/decorators/logging.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/decorators/schemas.py` & `microcosm-flask-4.1.3/microcosm_flask/decorators/schemas.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/encryption/conventions/crud_adapter.py` & `microcosm-flask-4.1.3/microcosm_flask/encryption/conventions/crud_adapter.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/enums.py` & `microcosm-flask-4.1.3/microcosm_flask/enums.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/errors.py` & `microcosm-flask-4.1.3/microcosm_flask/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 
 
 class ErrorContextSchema(Schema):
     errors = fields.List(fields.Nested(SubErrorSchema), required=True)
 
 
 class ErrorSchema(Schema):
-    message = fields.String(required=True, default="Unknown Error")
-    code = fields.Integer(required=True, default=500)
-    retryable = fields.Boolean(required=True, default=False)
+    message = fields.String(required=True, dump_default="Unknown Error")
+    code = fields.Integer(required=True, dump_default=500)
+    retryable = fields.Boolean(required=True, dump_default=False)
     context = fields.Nested(ErrorContextSchema, required=False)  # type: ignore
 
 
 def as_retryable(error):
     """
     Given an exception, mark it as retryable when serializing
     into HTTP error response.
```

### Comparing `microcosm-flask-4.1.1/microcosm_flask/factories.py` & `microcosm-flask-4.1.3/microcosm_flask/factories.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/fields/enum_field.py` & `microcosm-flask-4.1.3/microcosm_flask/fields/enum_field.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/fields/language_field.py` & `microcosm-flask-4.1.3/microcosm_flask/fields/language_field.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/fields/query_string_list.py` & `microcosm-flask-4.1.3/microcosm_flask/fields/query_string_list.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/fields/timestamp_field.py` & `microcosm-flask-4.1.3/microcosm_flask/fields/timestamp_field.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/fields/uri_field.py` & `microcosm-flask-4.1.3/microcosm_flask/fields/uri_field.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/formatting/base.py` & `microcosm-flask-4.1.3/microcosm_flask/formatting/base.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/formatting/csv_formatter.py` & `microcosm-flask-4.1.3/microcosm_flask/formatting/csv_formatter.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/forwarding.py` & `microcosm-flask-4.1.3/microcosm_flask/forwarding.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/linking.py` & `microcosm-flask-4.1.3/microcosm_flask/linking.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/matchers.py` & `microcosm-flask-4.1.3/microcosm_flask/matchers.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/memory.py` & `microcosm-flask-4.1.3/microcosm_flask/memory.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/metrics.py` & `microcosm-flask-4.1.3/microcosm_flask/metrics.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/metrics_classifier.py` & `microcosm-flask-4.1.3/microcosm_flask/metrics_classifier.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/namespaces.py` & `microcosm-flask-4.1.3/microcosm_flask/namespaces.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/naming.py` & `microcosm-flask-4.1.3/microcosm_flask/naming.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/operations.py` & `microcosm-flask-4.1.3/microcosm_flask/operations.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/paging.py` & `microcosm-flask-4.1.3/microcosm_flask/paging.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,21 +49,21 @@
     Identity function.
 
     """
     return x
 
 
 # NB: lots of code currently uses `PageSchema` to refer to `OffsetLimitPageSchema`
-# keeping this (mis)naming for backwards compatibilty
+# keeping this (mis)naming for backwards compatibility
 class PageSchema(Schema):
     offset = fields.Integer(
-        missing=None, metadata={"description": "The pagination starting offset."}
+        load_default=None, metadata={"description": "The pagination starting offset."}
     )
     limit = fields.Integer(
-        missing=None, metadata={"description": "The pagination limit."}
+        load_default=None, metadata={"description": "The pagination limit."}
     )
 
 
 class OffsetLimitPageSchema(PageSchema):
     pass
```

### Comparing `microcosm-flask-4.1.1/microcosm_flask/paths.py` & `microcosm-flask-4.1.3/microcosm_flask/paths.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/profiling.py` & `microcosm-flask-4.1.3/microcosm_flask/profiling.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/routing.py` & `microcosm-flask-4.1.3/microcosm_flask/routing.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/runserver.py` & `microcosm-flask-4.1.3/microcosm_flask/runserver.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/sentry.py` & `microcosm-flask-4.1.3/microcosm_flask/sentry.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/session.py` & `microcosm-flask-4.1.3/microcosm_flask/session.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/swagger/api.py` & `microcosm-flask-4.1.3/microcosm_flask/swagger/api.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/swagger/decorators.py` & `microcosm-flask-4.1.3/microcosm_flask/swagger/decorators.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/swagger/definitions.py` & `microcosm-flask-4.1.3/microcosm_flask/swagger/definitions.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/swagger/naming.py` & `microcosm-flask-4.1.3/microcosm_flask/swagger/naming.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/swagger/parameters/__init__.py` & `microcosm-flask-4.1.3/microcosm_flask/swagger/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/swagger/parameters/base.py` & `microcosm-flask-4.1.3/microcosm_flask/swagger/parameters/base.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/swagger/parameters/decorated.py` & `microcosm-flask-4.1.3/microcosm_flask/swagger/parameters/decorated.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/swagger/parameters/default.py` & `microcosm-flask-4.1.3/microcosm_flask/swagger/parameters/default.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     fields.Method: FieldInfo("object", None),
     fields.Number: FieldInfo("number", None),
     fields.Raw: FieldInfo("object", None),
     fields.String: FieldInfo("string", None),
     fields.Time: FieldInfo("string", None),
     fields.URL: FieldInfo("string", "url"),
     fields.UUID: FieldInfo("string", "uuid"),
+    fields.Constant: FieldInfo("object", None),
 }
 
 
 @logger
 class DefaultParameterBuilder(ParameterBuilder):
     """
     Builds parameters using default field mappings.
```

### Comparing `microcosm-flask-4.1.1/microcosm_flask/swagger/parameters/enum.py` & `microcosm-flask-4.1.3/microcosm_flask/swagger/parameters/enum.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/swagger/parameters/list.py` & `microcosm-flask-4.1.3/microcosm_flask/swagger/parameters/list.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/swagger/parameters/nested.py` & `microcosm-flask-4.1.3/microcosm_flask/swagger/parameters/nested.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/swagger/parameters/numeric.py` & `microcosm-flask-4.1.3/microcosm_flask/swagger/parameters/numeric.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/swagger/parameters/timestamp.py` & `microcosm-flask-4.1.3/microcosm_flask/swagger/parameters/timestamp.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/swagger/schemas.py` & `microcosm-flask-4.1.3/microcosm_flask/swagger/schemas.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/templates/landing.py` & `microcosm-flask-4.1.3/microcosm_flask/templates/landing.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask/templates/swagger_ui.py` & `microcosm-flask-4.1.3/microcosm_flask/templates/swagger_ui.py`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/microcosm_flask.egg-info/PKG-INFO` & `microcosm-flask-4.1.3/microcosm_flask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcosm-flask
-Version: 4.1.1
+Version: 4.1.3
 Summary: Opinionated persistence with FlaskQL
 Home-page: https://github.com/globality-corp/microcosm-flask
 Author: Globality Engineering
 Author-email: engineering@globality.com
 License: UNKNOWN
 Keywords: microcosm
 Platform: UNKNOWN
```

### Comparing `microcosm-flask-4.1.1/microcosm_flask.egg-info/SOURCES.txt` & `microcosm-flask-4.1.3/microcosm_flask.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 microcosm_flask/swagger/api.py
 microcosm_flask/swagger/decorators.py
 microcosm_flask/swagger/definitions.py
 microcosm_flask/swagger/naming.py
 microcosm_flask/swagger/schemas.py
 microcosm_flask/swagger/parameters/__init__.py
 microcosm_flask/swagger/parameters/base.py
+microcosm_flask/swagger/parameters/constant.py
 microcosm_flask/swagger/parameters/decorated.py
 microcosm_flask/swagger/parameters/default.py
 microcosm_flask/swagger/parameters/enum.py
 microcosm_flask/swagger/parameters/list.py
 microcosm_flask/swagger/parameters/nested.py
 microcosm_flask/swagger/parameters/numeric.py
 microcosm_flask/swagger/parameters/timestamp.py
```

### Comparing `microcosm-flask-4.1.1/microcosm_flask.egg-info/entry_points.txt` & `microcosm-flask-4.1.3/microcosm_flask.egg-info/entry_points.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 route = microcosm_flask.routing:configure_route_decorator
 route_metrics = microcosm_flask.metrics:RouteMetrics
 sentry_logging = microcosm_flask.sentry:configure_sentry
 swagger_convention = microcosm_flask.conventions.swagger:configure_swagger
 uuid = microcosm_flask.converters:configure_uuid
 
 [microcosm_flask.swagger.parameters]
+constant = microcosm_flask.swagger.parameters.constant:ConstantParameterBuilder
 decorated = microcosm_flask.swagger.parameters.decorated:DecoratedParameterBuilder
 enum = microcosm_flask.swagger.parameters.enum:EnumParameterBuilder
 list = microcosm_flask.swagger.parameters.list:ListParameterBuilder
 nested = microcosm_flask.swagger.parameters.nested:NestedParameterBuilder
 numeric = microcosm_flask.swagger.parameters.numeric:NumericParameterBuilder
 timestamp = microcosm_flask.swagger.parameters.timestamp:TimestampParameterBuilder
```

### Comparing `microcosm-flask-4.1.1/setup.cfg` & `microcosm-flask-4.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `microcosm-flask-4.1.1/setup.py` & `microcosm-flask-4.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import find_packages, setup
 
 
 project = "microcosm-flask"
-version = "4.1.1"
+version = "4.1.3"
 
 
 setup(
     name=project,
     version=version,
     description="Opinionated persistence with FlaskQL",
     long_description=open("README.md").read(),
@@ -56,14 +56,15 @@
     },
     setup_requires=[
         "nose>=1.3.7",
     ],
     dependency_links=[],
     entry_points={
         "microcosm_flask.swagger.parameters": [
+            "constant = microcosm_flask.swagger.parameters.constant:ConstantParameterBuilder",
             "decorated = microcosm_flask.swagger.parameters.decorated:DecoratedParameterBuilder",
             "enum = microcosm_flask.swagger.parameters.enum:EnumParameterBuilder",
             "list = microcosm_flask.swagger.parameters.list:ListParameterBuilder",
             "nested = microcosm_flask.swagger.parameters.nested:NestedParameterBuilder",
             "numeric = microcosm_flask.swagger.parameters.numeric:NumericParameterBuilder",
             "timestamp = microcosm_flask.swagger.parameters.timestamp:TimestampParameterBuilder",
         ],
```


# Comparing `tmp/oteapi-core-0.4.1.tar.gz` & `tmp/oteapi-core-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oteapi-core-0.4.1.tar", last modified: Fri Mar 10 10:18:39 2023, max compression
+gzip compressed data, was "oteapi-core-0.4.2.tar", last modified: Fri May 12 13:38:49 2023, max compression
```

## Comparing `oteapi-core-0.4.1.tar` & `oteapi-core-0.4.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:18:39.350888 oteapi-core-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-03-10 10:18:39.350888 oteapi-core-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12135 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:18:39.346888 oteapi-core-0.4.1/oteapi/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-10 10:18:35.000000 oteapi-core-0.4.1/oteapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:18:39.346888 oteapi-core-0.4.1/oteapi/datacache/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/datacache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/datacache/datacache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:18:39.346888 oteapi-core-0.4.1/oteapi/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/interfaces/idownloadstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/interfaces/ifilterstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/interfaces/ifunctionstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/interfaces/imappingstrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/interfaces/iparsestrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/interfaces/iresourcestrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/interfaces/itransformationstrategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:18:39.346888 oteapi-core-0.4.1/oteapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/models/datacacheconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/models/filterconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/models/functionconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/models/genericconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/models/mappingconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/models/resourceconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/models/secretconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/models/sessionupdate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/models/transformationconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/models/triplestoreconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:18:39.346888 oteapi-core-0.4.1/oteapi/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/plugins/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/plugins/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:18:39.346888 oteapi-core-0.4.1/oteapi/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/strategies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:18:39.350888 oteapi-core-0.4.1/oteapi/strategies/download/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/strategies/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/strategies/download/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/strategies/download/https.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/strategies/download/sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:18:39.350888 oteapi-core-0.4.1/oteapi/strategies/filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/strategies/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/strategies/filter/crop_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/strategies/filter/sql_query_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:18:39.350888 oteapi-core-0.4.1/oteapi/strategies/mapping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/strategies/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/strategies/mapping/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:18:39.350888 oteapi-core-0.4.1/oteapi/strategies/parse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/strategies/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/strategies/parse/application_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/strategies/parse/application_vnd_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/strategies/parse/excel_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/strategies/parse/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    12145 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/strategies/parse/text_csv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:18:39.350888 oteapi-core-0.4.1/oteapi/strategies/transformation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/strategies/transformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/strategies/transformation/celery_remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:18:39.350888 oteapi-core-0.4.1/oteapi/triplestore/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/triplestore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/triplestore/triplestore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:18:39.350888 oteapi-core-0.4.1/oteapi/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/oteapi/utils/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:18:39.350888 oteapi-core-0.4.1/oteapi_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-03-10 10:18:39.000000 oteapi-core-0.4.1/oteapi_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-03-10 10:18:39.000000 oteapi-core-0.4.1/oteapi_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 10:18:39.000000 oteapi-core-0.4.1/oteapi_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-03-10 10:18:39.000000 oteapi-core-0.4.1/oteapi_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-10 10:18:39.000000 oteapi-core-0.4.1/oteapi_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-10 10:18:39.000000 oteapi-core-0.4.1/oteapi_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-03-10 10:18:39.350888 oteapi-core-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-03-10 10:17:32.000000 oteapi-core-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.904651 oteapi-core-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-05-12 13:38:49.904651 oteapi-core-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12135 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.896651 oteapi-core-0.4.2/oteapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-12 13:38:46.000000 oteapi-core-0.4.2/oteapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.896651 oteapi-core-0.4.2/oteapi/datacache/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/datacache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/datacache/datacache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.896651 oteapi-core-0.4.2/oteapi/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/interfaces/idownloadstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/interfaces/ifilterstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/interfaces/ifunctionstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/interfaces/imappingstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/interfaces/iparsestrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/interfaces/iresourcestrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/interfaces/itransformationstrategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.900651 oteapi-core-0.4.2/oteapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/models/datacacheconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/models/filterconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/models/functionconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/models/genericconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/models/mappingconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/models/resourceconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/models/secretconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/models/sessionupdate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/models/transformationconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/models/triplestoreconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.900651 oteapi-core-0.4.2/oteapi/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/plugins/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/plugins/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.900651 oteapi-core-0.4.2/oteapi/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.900651 oteapi-core-0.4.2/oteapi/strategies/download/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/download/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/download/https.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/download/sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.900651 oteapi-core-0.4.2/oteapi/strategies/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/filter/crop_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/filter/sql_query_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.900651 oteapi-core-0.4.2/oteapi/strategies/mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/mapping/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.900651 oteapi-core-0.4.2/oteapi/strategies/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/parse/application_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/parse/application_vnd_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/parse/excel_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/parse/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12145 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/parse/text_csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.900651 oteapi-core-0.4.2/oteapi/strategies/transformation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/transformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/strategies/transformation/celery_remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.900651 oteapi-core-0.4.2/oteapi/triplestore/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/triplestore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/triplestore/triplestore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.900651 oteapi-core-0.4.2/oteapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/oteapi/utils/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:49.904651 oteapi-core-0.4.2/oteapi_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-05-12 13:38:49.000000 oteapi-core-0.4.2/oteapi_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-12 13:38:49.000000 oteapi-core-0.4.2/oteapi_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 13:38:49.000000 oteapi-core-0.4.2/oteapi_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-12 13:38:49.000000 oteapi-core-0.4.2/oteapi_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-12 13:38:49.000000 oteapi-core-0.4.2/oteapi_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 13:38:49.000000 oteapi-core-0.4.2/oteapi_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-12 13:38:49.904651 oteapi-core-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-12 13:37:42.000000 oteapi-core-0.4.2/setup.py
```

### Comparing `oteapi-core-0.4.1/LICENSE` & `oteapi-core-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/PKG-INFO` & `oteapi-core-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oteapi-core
-Version: 0.4.1
+Version: 0.4.2
 Summary: Open Translation Environment (OTE) API.
 Home-page: https://github.com/EMMC-ASBL/oteapi-core
 Author: SINTEF
 Author-email: Team4.0@SINTEF.no
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `oteapi-core-0.4.1/README.md` & `oteapi-core-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/datacache/datacache.py` & `oteapi-core-0.4.2/oteapi/datacache/datacache.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/interfaces/__init__.py` & `oteapi-core-0.4.2/oteapi/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/interfaces/idownloadstrategy.py` & `oteapi-core-0.4.2/oteapi/interfaces/idownloadstrategy.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/interfaces/ifilterstrategy.py` & `oteapi-core-0.4.2/oteapi/interfaces/ifilterstrategy.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/interfaces/ifunctionstrategy.py` & `oteapi-core-0.4.2/oteapi/interfaces/ifunctionstrategy.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/interfaces/imappingstrategy.py` & `oteapi-core-0.4.2/oteapi/interfaces/imappingstrategy.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/interfaces/iparsestrategy.py` & `oteapi-core-0.4.2/oteapi/interfaces/iparsestrategy.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/interfaces/iresourcestrategy.py` & `oteapi-core-0.4.2/oteapi/interfaces/iresourcestrategy.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/interfaces/itransformationstrategy.py` & `oteapi-core-0.4.2/oteapi/interfaces/itransformationstrategy.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/models/__init__.py` & `oteapi-core-0.4.2/oteapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/models/datacacheconfig.py` & `oteapi-core-0.4.2/oteapi/models/datacacheconfig.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/models/filterconfig.py` & `oteapi-core-0.4.2/oteapi/models/filterconfig.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/models/genericconfig.py` & `oteapi-core-0.4.2/oteapi/models/genericconfig.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/models/mappingconfig.py` & `oteapi-core-0.4.2/oteapi/models/mappingconfig.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/models/resourceconfig.py` & `oteapi-core-0.4.2/oteapi/models/resourceconfig.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/models/secretconfig.py` & `oteapi-core-0.4.2/oteapi/models/secretconfig.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/models/transformationconfig.py` & `oteapi-core-0.4.2/oteapi/models/transformationconfig.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/models/triplestoreconfig.py` & `oteapi-core-0.4.2/oteapi/models/triplestoreconfig.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/plugins/entry_points.py` & `oteapi-core-0.4.2/oteapi/plugins/entry_points.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/plugins/factories.py` & `oteapi-core-0.4.2/oteapi/plugins/factories.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/settings.py` & `oteapi-core-0.4.2/oteapi/settings.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/strategies/download/file.py` & `oteapi-core-0.4.2/oteapi/strategies/download/file.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/strategies/download/https.py` & `oteapi-core-0.4.2/oteapi/strategies/download/https.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/strategies/download/sftp.py` & `oteapi-core-0.4.2/oteapi/strategies/download/sftp.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/strategies/filter/crop_filter.py` & `oteapi-core-0.4.2/oteapi/strategies/filter/crop_filter.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/strategies/filter/sql_query_filter.py` & `oteapi-core-0.4.2/oteapi/strategies/filter/sql_query_filter.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/strategies/mapping/mapping.py` & `oteapi-core-0.4.2/oteapi/strategies/mapping/mapping.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/strategies/parse/application_json.py` & `oteapi-core-0.4.2/oteapi/strategies/parse/application_json.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/strategies/parse/application_vnd_sqlite.py` & `oteapi-core-0.4.2/oteapi/strategies/parse/application_vnd_sqlite.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/strategies/parse/excel_xlsx.py` & `oteapi-core-0.4.2/oteapi/strategies/parse/excel_xlsx.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/strategies/parse/image.py` & `oteapi-core-0.4.2/oteapi/strategies/parse/image.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/strategies/parse/text_csv.py` & `oteapi-core-0.4.2/oteapi/strategies/parse/text_csv.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/strategies/transformation/celery_remote.py` & `oteapi-core-0.4.2/oteapi/strategies/transformation/celery_remote.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/triplestore/triplestore.py` & `oteapi-core-0.4.2/oteapi/triplestore/triplestore.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi/utils/paths.py` & `oteapi-core-0.4.2/oteapi/utils/paths.py`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi_core.egg-info/PKG-INFO` & `oteapi-core-0.4.2/oteapi_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oteapi-core
-Version: 0.4.1
+Version: 0.4.2
 Summary: Open Translation Environment (OTE) API.
 Home-page: https://github.com/EMMC-ASBL/oteapi-core
 Author: SINTEF
 Author-email: Team4.0@SINTEF.no
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `oteapi-core-0.4.1/oteapi_core.egg-info/SOURCES.txt` & `oteapi-core-0.4.2/oteapi_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi_core.egg-info/entry_points.txt` & `oteapi-core-0.4.2/oteapi_core.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/oteapi_core.egg-info/requires.txt` & `oteapi-core-0.4.2/oteapi_core.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 agraph-python<102,>=101.0.7
 celery<6,>=5.2.3
 diskcache<6,>=5.4.0
-fastapi-plugins~=0.11.0
+fastapi-plugins~=0.12.0
 numpy<2,>=1.21
 openpyxl<4,>=3.0.9
 Pillow<10,>=9.0.0
 pydantic<2,>=1.9.0
 pysftp~=0.2.9
 requests<3,>=2.26.0
+urllib3<2
 
 [dev]
-pylint~=2.16
-pytest~=7.2
+pylint~=2.17
+pytest~=7.3
 pytest-celery
 pytest-cov~=4.0
 requests-mock~=1.10
 mike~=1.1
 mkdocs~=1.4
-mkdocs-awesome-pages-plugin~=2.8
+mkdocs-awesome-pages-plugin~=2.9
 mkdocs-material~=9.1
-mkdocstrings[python]~=0.20.0
+mkdocstrings[python]~=0.21.2
 
 [dev:python_version < "3.8"]
 pre-commit<3,>=2.21.0
 
 [dev:python_version >= "3.8"]
-pre-commit~=3.1
+pre-commit~=3.3
 
 [docs]
 mike~=1.1
 mkdocs~=1.4
-mkdocs-awesome-pages-plugin~=2.8
+mkdocs-awesome-pages-plugin~=2.9
 mkdocs-material~=9.1
-mkdocstrings[python]~=0.20.0
+mkdocstrings[python]~=0.21.2
```

### Comparing `oteapi-core-0.4.1/pyproject.toml` & `oteapi-core-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/setup.cfg` & `oteapi-core-0.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `oteapi-core-0.4.1/setup.py` & `oteapi-core-0.4.2/setup.py`

 * *Files identical despite different names*


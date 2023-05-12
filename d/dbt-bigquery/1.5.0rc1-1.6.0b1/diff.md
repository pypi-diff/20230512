# Comparing `tmp/dbt-bigquery-1.5.0rc1.tar.gz` & `tmp/dbt-bigquery-1.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-bigquery-1.5.0rc1.tar", last modified: Fri Apr 14 01:38:45 2023, max compression
+gzip compressed data, was "dbt-bigquery-1.6.0b1.tar", last modified: Fri May 12 20:06:21 2023, max compression
```

## Comparing `dbt-bigquery-1.5.0rc1.tar` & `dbt-bigquery-1.6.0b1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.434298 dbt-bigquery-1.5.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-14 01:38:45.434298 dbt-bigquery-1.5.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.426298 dbt-bigquery-1.5.0rc1/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.426298 dbt-bigquery-1.5.0rc1/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.426298 dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    25902 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/gcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    36364 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/python_submissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.426298 dbt-bigquery-1.5.0rc1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.426298 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.426298 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.430298 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/catalog.sql
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/etc.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.430298 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/copy.sql
--rw-r--r--   0 runner    (1001) docker     (123)     7706 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/incremental.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.430298 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/common.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.430298 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/python_model/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/python_model/python.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.430298 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/except.sql
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/get_columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/intersect.sql
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.434298 dbt-bigquery-1.5.0rc1/dbt_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-14 01:38:45.000000 dbt-bigquery-1.5.0rc1/dbt_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-14 01:38:45.000000 dbt-bigquery-1.5.0rc1/dbt_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 01:38:45.000000 dbt-bigquery-1.5.0rc1/dbt_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 01:38:45.000000 dbt-bigquery-1.5.0rc1/dbt_bigquery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-14 01:38:45.000000 dbt-bigquery-1.5.0rc1/dbt_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-14 01:38:45.000000 dbt-bigquery-1.5.0rc1/dbt_bigquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 01:38:45.434298 dbt-bigquery-1.5.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.526347 dbt-bigquery-1.6.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-12 20:06:21.526347 dbt-bigquery-1.6.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.518346 dbt-bigquery-1.6.0b1/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.518346 dbt-bigquery-1.6.0b1/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.522347 dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26002 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37860 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/python_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.518346 dbt-bigquery-1.6.0b1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.522347 dbt-bigquery-1.6.0b1/dbt/include/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.522347 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.522347 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/catalog.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/etc.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.522347 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/copy.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/incremental.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.522347 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/incremental_strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/incremental_strategy/common.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.522347 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/python_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/python_model/python.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.526347 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/except.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/get_columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/intersect.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.526347 dbt-bigquery-1.6.0b1/dbt_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-12 20:06:21.000000 dbt-bigquery-1.6.0b1/dbt_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-12 20:06:21.000000 dbt-bigquery-1.6.0b1/dbt_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:06:21.000000 dbt-bigquery-1.6.0b1/dbt_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:06:21.000000 dbt-bigquery-1.6.0b1/dbt_bigquery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-12 20:06:21.000000 dbt-bigquery-1.6.0b1/dbt_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-12 20:06:21.000000 dbt-bigquery-1.6.0b1/dbt_bigquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 20:06:21.526347 dbt-bigquery-1.6.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/setup.py
```

### Comparing `dbt-bigquery-1.5.0rc1/LICENSE.md` & `dbt-bigquery-1.6.0b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0rc1/PKG-INFO` & `dbt-bigquery-1.6.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-bigquery
-Version: 1.5.0rc1
+Version: 1.6.0b1
 Summary: The Bigquery adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-bigquery
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.5.0rc1 Summary: The
-Bigquery adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
-bigquery Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
-Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
-:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Python: >=3.7 Description-
-Content-Type: text/markdown License-File: LICENSE.md
+Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.6.0b1 Summary: The Bigquery
+adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-bigquery
+Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
+:: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Operating System :: Microsoft :: Windows Classifier:
+Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
+Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Python: >=3.7 Description-Content-Type:
+text/markdown License-File: LICENSE.md
                                   [dbt logo]
                  [Unit_Tests_Badge] [Integration_Tests_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-bigquery The `dbt-bigquery` package contains all of
```

### Comparing `dbt-bigquery-1.5.0rc1/README.md` & `dbt-bigquery-1.6.0b1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/__init__.py` & `dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/column.py` & `dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/column.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/connections.py` & `dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,26 +406,26 @@
         return credentials.job_retry_deadline_seconds
 
     @classmethod
     def get_table_from_response(cls, resp):
         column_names = [field.name for field in resp.schema]
         return agate_helper.table_from_data_flat(resp, column_names)
 
-    def raw_execute(self, sql, fetch=False, *, use_legacy_sql=False):
+    def raw_execute(self, sql, use_legacy_sql=False, limit: Optional[int] = None):
         conn = self.get_thread_connection()
         client = conn.handle
 
         fire_event(SQLQuery(conn_name=conn.name, sql=sql))
         if (
             hasattr(self.profile, "query_comment")
             and self.profile.query_comment
             and self.profile.query_comment.job_label
         ):
-            query_comment = self.query_header.comment.query_comment
-            labels = self._labels_from_query_comment(query_comment)
+            query_comment = self.profile.query_comment
+            labels = self._labels_from_query_comment(query_comment.comment)
         else:
             labels = {}
 
         if active_user:
             labels["dbt_invocation_id"] = active_user.invocation_id
 
         job_params = {"use_legacy_sql": use_legacy_sql, "labels": labels}
@@ -446,26 +446,27 @@
         def fn():
             return self._query_and_results(
                 client,
                 sql,
                 job_params,
                 job_creation_timeout=job_creation_timeout,
                 job_execution_timeout=job_execution_timeout,
+                limit=limit,
             )
 
         query_job, iterator = self._retry_and_handle(msg=sql, conn=conn, fn=fn)
 
         return query_job, iterator
 
     def execute(
-        self, sql, auto_begin=False, fetch=None
+        self, sql, auto_begin=False, fetch=None, limit: Optional[int] = None
     ) -> Tuple[BigQueryAdapterResponse, agate.Table]:
         sql = self._add_query_comment(sql)
         # auto_begin is ignored on bigquery, and only included for consistency
-        query_job, iterator = self.raw_execute(sql, fetch=fetch)
+        query_job, iterator = self.raw_execute(sql, limit=limit)
 
         if fetch:
             table = self.get_table_from_response(iterator)
         else:
             table = agate_helper.empty_table()
 
         message = "OK"
@@ -546,15 +547,15 @@
         def standard_to_legacy(table):
             return table.project + ":" + table.dataset + "." + table.identifier
 
         legacy_sql = "SELECT * FROM [" + standard_to_legacy(table) + "$__PARTITIONS_SUMMARY__]"
 
         sql = self._add_query_comment(legacy_sql)
         # auto_begin is ignored on bigquery, and only included for consistency
-        _, iterator = self.raw_execute(sql, fetch="fetch_result", use_legacy_sql=True)
+        _, iterator = self.raw_execute(sql, use_legacy_sql=True)
         return self.get_table_from_response(iterator)
 
     def copy_bq_table(self, source, destination, write_disposition):
         conn = self.get_thread_connection()
         client = conn.handle
 
         # -------------------------------------------------------------------------------
@@ -640,20 +641,21 @@
     def _query_and_results(
         self,
         client,
         sql,
         job_params,
         job_creation_timeout=None,
         job_execution_timeout=None,
+        limit: Optional[int] = None,
     ):
         """Query the client and wait for results."""
         # Cannot reuse job_config if destination is set and ddl is used
         job_config = google.cloud.bigquery.QueryJobConfig(**job_params)
         query_job = client.query(query=sql, job_config=job_config, timeout=job_creation_timeout)
-        iterator = query_job.result(timeout=job_execution_timeout)
+        iterator = query_job.result(max_results=limit, timeout=job_execution_timeout)
 
         return query_job, iterator
 
     def _retry_and_handle(self, msg, conn, fn):
         """retry a function call within the context of exception_handler."""
 
         def reopen_conn_on_error(error):
```

### Comparing `dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/dataset.py` & `dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/dataset.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/gcloud.py` & `dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/gcloud.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/impl.py` & `dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/impl.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from dataclasses import dataclass
 import threading
 from typing import Dict, List, Optional, Any, Set, Union, Type
 
-from dbt.contracts.graph.nodes import ColumnLevelConstraint, ModelLevelConstraint, ConstraintType
+from dbt.contracts.graph.nodes import ColumnLevelConstraint, ModelLevelConstraint, ConstraintType  # type: ignore
 from dbt.dataclass_schema import dbtClassMixin, ValidationError
 
 import dbt.deprecations
 import dbt.exceptions
 import dbt.clients.agate_helper
 
 from dbt import ui  # type: ignore
-from dbt.adapters.base import (
+from dbt.adapters.base import (  # type: ignore
     BaseAdapter,
     ConstraintSupport,
     available,
     RelationType,
     BaseRelation,
     SchemaSearchMap,
     AdapterConfig,
     PythonJobHelper,
 )
 
-from dbt.adapters.cache import _make_ref_key_dict
+from dbt.adapters.cache import _make_ref_key_dict  # type: ignore
 
 from dbt.adapters.bigquery.relation import BigQueryRelation
 from dbt.adapters.bigquery.dataset import add_access_entry_to_dataset
 from dbt.adapters.bigquery import BigQueryColumn
 from dbt.adapters.bigquery import BigQueryConnectionManager
 from dbt.adapters.bigquery.python_submissions import (
     ClusterDataprocHelper,
@@ -73,56 +73,88 @@
     field: str
     data_type: str = "date"
     granularity: str = "day"
     range: Optional[Dict[str, Any]] = None
     time_ingestion_partitioning: bool = False
     copy_partitions: bool = False
 
+    PARTITION_DATE = "_PARTITIONDATE"
+    PARTITION_TIME = "_PARTITIONTIME"
+
     def data_type_for_partition(self):
-        """Return the data type of partitions for replacement."""
-        return self.data_type if not self.time_ingestion_partitioning else "timestamp"
+        """Return the data type of partitions for replacement.
+        When time_ingestion_partitioning is enabled, the data type supported are date & timestamp.
+        """
+        if not self.time_ingestion_partitioning:
+            return self.data_type
+
+        return "date" if self.data_type == "date" else "timestamp"
 
     def reject_partition_field_column(self, columns: List[Any]) -> List[str]:
         return [c for c in columns if not c.name.upper() == self.field.upper()]
 
     def data_type_should_be_truncated(self):
         """Return true if the data type should be truncated instead of cast to the data type."""
         return not (
-            self.data_type.lower() == "int64"
-            or (self.data_type.lower() == "date" and self.granularity.lower() == "day")
+            self.data_type == "int64" or (self.data_type == "date" and self.granularity == "day")
         )
 
+    def time_partitioning_field(self) -> str:
+        """Return the time partitioning field name based on the data type.
+        The default is _PARTITIONTIME, but for date it is _PARTITIONDATE
+        else it will fail statements for type mismatch."""
+        if self.data_type == "date":
+            return self.PARTITION_DATE
+        else:
+            return self.PARTITION_TIME
+
+    def insertable_time_partitioning_field(self) -> str:
+        """Return the insertable time partitioning field name based on the data type.
+        Practically, only _PARTITIONTIME works so far.
+        The function is meant to keep the call sites consistent as it might evolve."""
+        return self.PARTITION_TIME
+
     def render(self, alias: Optional[str] = None):
-        column: str = self.field if not self.time_ingestion_partitioning else "_PARTITIONTIME"
+        column: str = (
+            self.field if not self.time_ingestion_partitioning else self.time_partitioning_field()
+        )
         if alias:
             column = f"{alias}.{column}"
 
         if self.data_type_should_be_truncated():
             return f"{self.data_type}_trunc({column}, {self.granularity})"
         else:
             return column
 
     def render_wrapped(self, alias: Optional[str] = None):
         """Wrap the partitioning column when time involved to ensure it is properly cast to matching time."""
         # if data type is going to be truncated, no need to wrap
         if (
             self.data_type in ("date", "timestamp", "datetime")
             and not self.data_type_should_be_truncated()
+            and not (
+                self.time_ingestion_partitioning and self.data_type == "date"
+            )  # _PARTITIONDATE is already a date
         ):
             return f"{self.data_type}({self.render(alias)})"
         else:
             return self.render(alias)
 
     @classmethod
     def parse(cls, raw_partition_by) -> Optional["PartitionConfig"]:
         if raw_partition_by is None:
             return None
         try:
             cls.validate(raw_partition_by)
-            return cls.from_dict(raw_partition_by)
+            return cls.from_dict(
+                {
+                    key: (value.lower() if isinstance(value, str) else value)
+                    for key, value in raw_partition_by.items()
+                }
+            )
         except ValidationError as exc:
             raise dbt.exceptions.DbtValidationError("Could not parse partition config") from exc
         except TypeError:
             raise dbt.exceptions.CompilationError(
                 f"Invalid partition_by config:\n"
                 f"  Got: {raw_partition_by}\n"
                 f'  Expected a dictionary with "field" and "data_type" keys'
@@ -269,17 +301,24 @@
             return self._get_dbt_columns_from_bq_table(table)
 
         except (ValueError, google.cloud.exceptions.NotFound) as e:
             logger.debug("get_columns_in_relation error: {}".format(e))
             return []
 
     @available.parse(lambda *a, **k: [])
-    def add_time_ingestion_partition_column(self, columns) -> List[BigQueryColumn]:
-        "Add time ingestion partition column to columns list"
-        columns.append(self.Column("_PARTITIONTIME", "TIMESTAMP", None, "NULLABLE"))
+    def add_time_ingestion_partition_column(self, partition_by, columns) -> List[BigQueryColumn]:
+        """Add time ingestion partition column to columns list"""
+        columns.append(
+            self.Column(
+                partition_by.insertable_time_partitioning_field(),
+                partition_by.data_type,
+                None,
+                "NULLABLE",
+            )
+        )
         return columns
 
     def expand_column_types(self, goal: BigQueryRelation, current: BigQueryRelation) -> None:  # type: ignore[override]
         # This is a no-op on BigQuery
         pass
 
     def expand_target_column_types(
@@ -560,26 +599,23 @@
         If there is a mismatch, then the table cannot be replaced directly.
         """
         is_partitioned = table.range_partitioning or table.time_partitioning
 
         if not is_partitioned and not conf_partition:
             return True
         elif conf_partition and table.time_partitioning is not None:
-            partitioning_field = table.time_partitioning.field or "_PARTITIONTIME"
-            table_field = partitioning_field.lower()
-            table_granularity = table.partitioning_type.lower()
-            conf_table_field = (
-                conf_partition.field
-                if not conf_partition.time_ingestion_partitioning
-                else "_PARTITIONTIME"
+            table_field = (
+                table.time_partitioning.field.lower() if table.time_partitioning.field else None
             )
+            table_granularity = table.partitioning_type
+            conf_table_field = conf_partition.field
             return (
-                table_field == conf_table_field.lower()
-                and table_granularity == conf_partition.granularity.lower()
-            )
+                table_field == conf_table_field
+                or (conf_partition.time_ingestion_partitioning and table_field is not None)
+            ) and table_granularity == conf_partition.granularity
         elif conf_partition and table.range_partitioning is not None:
             dest_part = table.range_partitioning
             conf_part = conf_partition.range or {}
 
             return (
                 dest_part.field == conf_partition.field
                 and dest_part.range_.start == conf_part.get("start")
@@ -653,15 +689,16 @@
             dotted_column_name = "{}.{}".format(parent, bq_column_dict["name"])
         else:
             dotted_column_name = bq_column_dict["name"]
 
         if dotted_column_name in dbt_columns:
             column_config = dbt_columns[dotted_column_name]
             bq_column_dict["description"] = column_config.get("description")
-            bq_column_dict["policyTags"] = {"names": column_config.get("policy_tags", list())}
+            if bq_column_dict["type"] != "RECORD":
+                bq_column_dict["policyTags"] = {"names": column_config.get("policy_tags", list())}
 
         new_fields = []
         for child_col_dict in bq_column_dict.get("fields", list()):
             new_child_column_dict = self._update_column_dict(
                 child_col_dict, dbt_columns, parent=dotted_column_name
             )
             new_fields.append(new_child_column_dict)
@@ -919,25 +956,25 @@
         return {
             "cluster": ClusterDataprocHelper,
             "serverless": ServerlessDataProcHelper,
         }
 
     @classmethod
     def render_column_constraint(cls, constraint: ColumnLevelConstraint) -> Optional[str]:
-        c = super().render_column_constraint(constraint)
+        c = super().render_column_constraint(constraint)  # type: ignore
         if (
             constraint.type == ConstraintType.primary_key
             or constraint.type == ConstraintType.foreign_key
         ):
             return f"{c} not enforced" if c else None
         return c
 
     @classmethod
     def render_model_constraint(cls, constraint: ModelLevelConstraint) -> Optional[str]:
-        c = super().render_model_constraint(constraint)
+        c = super().render_model_constraint(constraint)  # type: ignore
         if (
             constraint.type == ConstraintType.primary_key
             or constraint.type == ConstraintType.foreign_key
         ):
             return f"{c} not enforced" if c else None
 
         return c
```

### Comparing `dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/python_submissions.py` & `dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/python_submissions.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/relation.py` & `dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/adapters/apply_grants.sql` & `dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/adapters.sql` & `dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/adapters.sql`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 
 {% macro partition_by(partition_config) -%}
     {%- if partition_config is none -%}
       {% do return('') %}
+    {%- elif partition_config.time_ingestion_partitioning -%}
+        partition by {{ partition_config.render_wrapped() }}
     {%- elif partition_config.data_type | lower in ('date','timestamp','datetime') -%}
         partition by {{ partition_config.render() }}
     {%- elif partition_config.data_type | lower in ('int64') -%}
         {%- set range = partition_config.range -%}
         partition by range_bucket(
             {{ partition_config.field }},
             generate_array({{ range.start}}, {{ range.end }}, {{ range.interval }})
@@ -44,31 +46,45 @@
 {% macro bigquery__create_table_as(temporary, relation, compiled_code, language='sql') -%}
   {%- if language == 'sql' -%}
     {%- set raw_partition_by = config.get('partition_by', none) -%}
     {%- set raw_cluster_by = config.get('cluster_by', none) -%}
     {%- set sql_header = config.get('sql_header', none) -%}
 
     {%- set partition_config = adapter.parse_partition_by(raw_partition_by) -%}
+    {%- if partition_config.time_ingestion_partitioning -%}
+    {%- set columns = get_columns_with_types_in_query_sql(sql) -%}
+    {%- set table_dest_columns_csv = columns_without_partition_fields_csv(partition_config, columns) -%}
+    {%- set columns = '(' ~ table_dest_columns_csv ~ ')' -%}
+    {%- endif -%}
 
     {{ sql_header if sql_header is not none }}
 
     create or replace table {{ relation }}
       {%- set contract_config = config.get('contract') -%}
       {%- if contract_config.enforced -%}
         {{ get_assert_columns_equivalent(compiled_code) }}
         {{ get_table_columns_and_constraints() }}
         {%- set compiled_code = get_select_subquery(compiled_code) %}
+      {% else %}
+        {#-- cannot do contracts at the same time as time ingestion partitioning -#}
+        {{ columns }}
       {% endif %}
     {{ partition_by(partition_config) }}
     {{ cluster_by(raw_cluster_by) }}
 
     {{ bigquery_table_options(config, model, temporary) }}
+
+    {#-- PARTITION BY cannot be used with the AS query_statement clause.
+         https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#partition_expression
+    -#}
+    {%- if not partition_config.time_ingestion_partitioning %}
     as (
       {{ compiled_code }}
     );
+    {%- endif %}
   {%- elif language == 'python' -%}
     {#--
     N.B. Python models _can_ write to temp views HOWEVER they use a different session
     and have already expired by the time they need to be used (I.E. in merges for incremental models)
 
     TODO: Deep dive into spark sessions to see if we can reuse a single session for an entire
     dbt invocation.
```

### Comparing `dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/catalog.sql` & `dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/copy.sql` & `dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/copy.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/incremental.sql` & `dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/incremental.sql`

 * *Files 6% similar despite different names*

```diff
@@ -12,32 +12,33 @@
 
   {% do return(strategy) %}
 {% endmacro %}
 
 {% macro source_sql_with_partition(partition_by, source_sql) %}
 
   {%- if partition_by.time_ingestion_partitioning %}
-    {{ return(wrap_with_time_ingestion_partitioning_sql(build_partition_time_exp(partition_by.field), source_sql, False))  }}
+    {{ return(wrap_with_time_ingestion_partitioning_sql(partition_by, source_sql, False))  }}
   {% else %}
     {{ return(source_sql)  }}
   {%- endif -%}
 
 {% endmacro %}
-{% macro bq_create_table_as(is_time_ingestion_partitioning, temporary, relation, compiled_code, language='sql') %}
-  {% if is_time_ingestion_partitioning and language == 'python' %}
+
+{% macro bq_create_table_as(partition_by, temporary, relation, compiled_code, language='sql') %}
+  {%- set _dbt_max_partition = declare_dbt_max_partition(this, partition_by, compiled_code, language) -%}
+  {% if partition_by.time_ingestion_partitioning and language == 'python' %}
     {% do exceptions.raise_compiler_error(
       "Python models do not support ingestion time partitioning"
     ) %}
-  {% endif %}
-  {% if is_time_ingestion_partitioning and language == 'sql' %}
+  {% elif partition_by.time_ingestion_partitioning and language == 'sql' %}
     {#-- Create the table before inserting data as ingestion time partitioned tables can't be created with the transformed data --#}
-    {% do run_query(create_ingestion_time_partitioned_table_as_sql(temporary, relation, compiled_code)) %}
-    {{ return(bq_insert_into_ingestion_time_partitioned_table_sql(relation, compiled_code)) }}
+    {% do run_query(create_table_as(temporary, relation, compiled_code)) %}
+    {{ return(_dbt_max_partition + bq_insert_into_ingestion_time_partitioned_table_sql(relation, compiled_code)) }}
   {% else %}
-    {{ return(create_table_as(temporary, relation, compiled_code, language)) }}
+    {{ return(_dbt_max_partition + create_table_as(temporary, relation, compiled_code, language)) }}
   {% endif %}
 {% endmacro %}
 
 {% macro bq_generate_incremental_build_sql(
     strategy, tmp_relation, target_relation, sql, unique_key, partition_by, partitions, dest_columns, tmp_relation_exists, copy_partitions, incremental_predicates
 ) %}
   {#-- if partitioned, use BQ scripting to get the range of partition values to be updated --#}
@@ -89,32 +90,32 @@
         {% set wrong_strategy_msg -%}
         The 'copy_partitions' option requires the 'incremental_strategy' option to be set to 'insert_overwrite'.
         {%- endset %}
         {% do exceptions.raise_compiler_error(wrong_strategy_msg) %}
 
   {% elif existing_relation is none %}
       {%- call statement('main', language=language) -%}
-        {{ bq_create_table_as(partition_by.time_ingestion_partitioning, False, target_relation, compiled_code, language) }}
+        {{ bq_create_table_as(partition_by, False, target_relation, compiled_code, language) }}
       {%- endcall -%}
 
   {% elif existing_relation.is_view %}
       {#-- There's no way to atomically replace a view with a table on BQ --#}
       {{ adapter.drop_relation(existing_relation) }}
       {%- call statement('main', language=language) -%}
-        {{ bq_create_table_as(partition_by.time_ingestion_partitioning, False, target_relation, compiled_code, language) }}
+        {{ bq_create_table_as(partition_by, False, target_relation, compiled_code, language) }}
       {%- endcall -%}
 
   {% elif full_refresh_mode %}
       {#-- If the partition/cluster config has changed, then we must drop and recreate --#}
       {% if not adapter.is_replaceable(existing_relation, partition_by, cluster_by) %}
           {% do log("Hard refreshing " ~ existing_relation ~ " because it is not replaceable") %}
           {{ adapter.drop_relation(existing_relation) }}
       {% endif %}
       {%- call statement('main', language=language) -%}
-        {{ bq_create_table_as(partition_by.time_ingestion_partitioning, False, target_relation, compiled_code, language) }}
+        {{ bq_create_table_as(partition_by, False, target_relation, compiled_code, language) }}
       {%- endcall -%}
 
   {% else %}
     {%- if language == 'python' and strategy == 'insert_overwrite' -%}
       {#-- This lets us move forward assuming no python will be directly templated into a query --#}
       {%- set python_unsupported_msg -%}
         The 'insert_overwrite' strategy is not yet supported for python models.
@@ -123,29 +124,29 @@
     {%- endif -%}
 
     {% set tmp_relation_exists = false %}
     {% if on_schema_change != 'ignore' or language == 'python' %}
       {#-- Check first, since otherwise we may not build a temp table --#}
       {#-- Python always needs to create a temp table --#}
       {%- call statement('create_tmp_relation', language=language) -%}
-        {{ declare_dbt_max_partition(this, partition_by, compiled_code, language) +
-           bq_create_table_as(partition_by.time_ingestion_partitioning, True, tmp_relation, compiled_code, language)
-        }}
+        {{ bq_create_table_as(partition_by, True, tmp_relation, compiled_code, language) }}
       {%- endcall -%}
       {% set tmp_relation_exists = true %}
       {#-- Process schema changes. Returns dict of changes if successful. Use source columns for upserting/merging --#}
       {% set dest_columns = process_schema_changes(on_schema_change, tmp_relation, existing_relation) %}
     {% endif %}
 
     {% if not dest_columns %}
       {% set dest_columns = adapter.get_columns_in_relation(existing_relation) %}
     {% endif %}
+    {#--  Add time ingestion pseudo column to destination column as not part of the 'schema' but still need it for actual data insertion --#}
     {% if partition_by.time_ingestion_partitioning %}
-      {% set dest_columns = adapter.add_time_ingestion_partition_column(dest_columns) %}
+      {% set dest_columns = adapter.add_time_ingestion_partition_column(partition_by, dest_columns) %}
     {% endif %}
+
     {% set build_sql = bq_generate_incremental_build_sql(
         strategy, tmp_relation, target_relation, compiled_code, unique_key, partition_by, partitions, dest_columns, tmp_relation_exists, partition_by.copy_partitions, incremental_predicates
     ) %}
 
     {%- call statement('main') -%}
       {{ build_sql }}
     {% endcall %}
```

### Comparing `dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql` & `dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql`

 * *Files 6% similar despite different names*

```diff
@@ -54,15 +54,15 @@
               {{ partitions | join (', ') }}
           )
       {%- endset %}
 
       {%- set source_sql -%}
         (
           {%- if partition_by.time_ingestion_partitioning -%}
-          {{ wrap_with_time_ingestion_partitioning_sql(build_partition_time_exp(partition_by), sql, True) }}
+          {{ wrap_with_time_ingestion_partitioning_sql(partition_by, sql, True) }}
           {%- else -%}
           {{sql}}
           {%- endif -%}
         )
       {%- endset -%}
 
       {% if copy_partitions %}
@@ -81,16 +81,15 @@
 {% endmacro %}
 
 {% macro bq_dynamic_copy_partitions_insert_overwrite_sql(
   tmp_relation, target_relation, sql, unique_key, partition_by, dest_columns, tmp_relation_exists, copy_partitions
   ) %}
   {# We run temp table creation in a separated script to move to partitions copy #}
   {%- call statement('create_tmp_relation_for_copy', language='sql') -%}
-    {{ declare_dbt_max_partition(this, partition_by, sql, 'sql') +
-     bq_create_table_as(partition_by.time_ingestion_partitioning, True, tmp_relation, sql, 'sql')
+    {{ bq_create_table_as(partition_by, True, tmp_relation, sql, 'sql')
   }}
   {%- endcall %}
   {%- set partitions_sql -%}
     select distinct {{ partition_by.render_wrapped() }}
     from {{ tmp_relation }}
   {%- endset -%}
   {%- set partitions = run_query(partitions_sql).columns[0].values() -%}
@@ -108,38 +107,37 @@
           {{ partition_by.render_wrapped(alias='DBT_INTERNAL_DEST') }} in unnest(dbt_partitions_for_replacement)
       {%- endset %}
 
       {%- set source_sql -%}
       (
         select
         {% if partition_by.time_ingestion_partitioning -%}
-        _PARTITIONTIME,
+        {{ partition_by.insertable_time_partitioning_field() }},
         {%- endif -%}
         * from {{ tmp_relation }}
       )
       {%- endset -%}
 
       -- generated script to merge partitions into {{ target_relation }}
       declare dbt_partitions_for_replacement array<{{ partition_by.data_type_for_partition() }}>;
 
       {# have we already created the temp table to check for schema changes? #}
       {% if not tmp_relation_exists %}
-        {{ declare_dbt_max_partition(this, partition_by, sql) }}
-
        -- 1. create a temp table with model data
-        {{ bq_create_table_as(partition_by.time_ingestion_partitioning, True, tmp_relation, sql, 'sql') }}
+        {{ bq_create_table_as(partition_by, True, tmp_relation, sql, 'sql') }}
       {% else %}
         -- 1. temp table already exists, we used it to check for schema changes
       {% endif %}
+      {%- set partition_field = partition_by.time_partitioning_field() if partition_by.time_ingestion_partitioning else partition_by.render_wrapped() -%}
 
       -- 2. define partitions to update
       set (dbt_partitions_for_replacement) = (
           select as struct
               -- IGNORE NULLS: this needs to be aligned to _dbt_max_partition, which ignores null
-              array_agg(distinct {{ partition_by.render_wrapped() }} IGNORE NULLS)
+              array_agg(distinct {{ partition_field }} IGNORE NULLS)
           from {{ tmp_relation }}
       );
 
       -- 3. run the merge statement
       {{ get_insert_overwrite_merge_sql(target_relation, source_sql, dest_columns, [predicate]) }};
 
       -- 4. clean up the temp table
```

### Comparing `dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql` & `dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,22 @@
     tmp_relation, target_relation, sql, unique_key, partition_by, dest_columns, tmp_relation_exists, incremental_predicates
 ) %}
     {%- set source_sql -%}
         {%- if tmp_relation_exists -%}
         (
         select
         {% if partition_by.time_ingestion_partitioning -%}
-        _PARTITIONTIME,
+        {{ partition_by.insertable_time_partitioning_field() }},
         {%- endif -%}
         * from {{ tmp_relation }}
         )
         {%- else -%} {#-- wrap sql in parens to make it a subquery --#}
         (
             {%- if partition_by.time_ingestion_partitioning -%}
-            {{ wrap_with_time_ingestion_partitioning_sql(build_partition_time_exp(partition_by), sql, True) }}
+            {{ wrap_with_time_ingestion_partitioning_sql(partition_by, sql, True) }}
             {%- else -%}
             {{sql}}
             {%- endif %}
         )
         {%- endif -%}
     {%- endset -%}
```

### Comparing `dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql` & `dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,15 @@
-{% macro wrap_with_time_ingestion_partitioning_sql(partition_time_exp, sql, is_nested) %}
+{% macro wrap_with_time_ingestion_partitioning_sql(partition_by, sql, is_nested) %}
 
-  select {{ partition_time_exp['value'] }} as _partitiontime, * EXCEPT({{ partition_time_exp['field'] }}) from (
+  select TIMESTAMP({{ partition_by.field }}) as {{ partition_by.insertable_time_partitioning_field() }}, * EXCEPT({{ partition_by.field }}) from (
     {{ sql }}
   ){%- if not is_nested -%};{%- endif -%}
 
 {% endmacro %}
 
-{% macro create_ingestion_time_partitioned_table_as_sql(temporary, relation, sql) -%}
-  {%- set raw_partition_by = config.get('partition_by', none) -%}
-  {%- set raw_cluster_by = config.get('cluster_by', none) -%}
-  {%- set sql_header = config.get('sql_header', none) -%}
-
-  {%- set partition_config = adapter.parse_partition_by(raw_partition_by) -%}
-
-  {%- set columns = get_columns_with_types_in_query_sql(sql) -%}
-  {%- set table_dest_columns_csv = columns_without_partition_fields_csv(partition_config, columns) -%}
-
-  {{ sql_header if sql_header is not none }}
-
-  {% set ingestion_time_partition_config_raw = fromjson(tojson(raw_partition_by)) %}
-  {% do ingestion_time_partition_config_raw.update({'field':'_PARTITIONTIME'}) %}
-
-  {%- set ingestion_time_partition_config = adapter.parse_partition_by(ingestion_time_partition_config_raw) -%}
-
-  create or replace table {{ relation }} ({{table_dest_columns_csv}})
-  {{ partition_by(ingestion_time_partition_config) }}
-  {{ cluster_by(raw_cluster_by) }}
-  {{ bigquery_table_options(config, model, temporary) }}
-
-{%- endmacro -%}
-
 {% macro get_quoted_with_types_csv(columns) %}
     {% set quoted = [] %}
     {% for col in columns -%}
         {%- do quoted.append(adapter.quote(col.name) ~ " " ~ col.data_type) -%}
     {%- endfor %}
     {%- set dest_cols_csv = quoted | join(', ') -%}
     {{ return(dest_cols_csv) }}
@@ -44,25 +20,30 @@
   {%- set columns_no_partition = partition_config.reject_partition_field_column(columns) -%}
   {% set columns_names = get_quoted_with_types_csv(columns_no_partition) %}
   {{ return(columns_names) }}
 
 {%- endmacro -%}
 
 {% macro bq_insert_into_ingestion_time_partitioned_table_sql(target_relation, sql) -%}
-  {%- set partition_by = config.get('partition_by', none) -%}
+  {%- set sql_header = config.get('sql_header', none) -%}
+  {{ sql_header if sql_header is not none }}
+  {%- set raw_partition_by = config.get('partition_by', none) -%}
+  {%- set partition_by = adapter.parse_partition_by(raw_partition_by) -%}
   {% set dest_columns = adapter.get_columns_in_relation(target_relation) %}
   {%- set dest_columns_csv = get_quoted_csv(dest_columns | map(attribute="name")) -%}
 
-  insert into {{ target_relation }} (_partitiontime, {{ dest_columns_csv }})
-    {{ wrap_with_time_ingestion_partitioning_sql(build_partition_time_exp(partition_by), sql, False) }}
+  insert into {{ target_relation }} ({{ partition_by.insertable_time_partitioning_field() }}, {{ dest_columns_csv }})
+    {{ wrap_with_time_ingestion_partitioning_sql(partition_by, sql, False) }}
 
 {%- endmacro -%}
 
 {% macro get_columns_with_types_in_query_sql(select_sql) %}
   {% set sql %}
+    {%- set sql_header = config.get('sql_header', none) -%}
+    {{ sql_header if sql_header is not none }}
     select * from (
       {{ select_sql }}
     ) as __dbt_sbq
     where false
     limit 0
   {% endset %}
   {{ return(adapter.get_columns_in_select_sql(sql)) }}
```

### Comparing `dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/seed.sql` & `dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/table.sql` & `dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/view.sql` & `dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0rc1/dbt/include/bigquery/profile_template.yml` & `dbt-bigquery-1.6.0b1/dbt/include/bigquery/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0rc1/dbt_bigquery.egg-info/PKG-INFO` & `dbt-bigquery-1.6.0b1/dbt_bigquery.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-bigquery
-Version: 1.5.0rc1
+Version: 1.6.0b1
 Summary: The Bigquery adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-bigquery
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.5.0rc1 Summary: The
-Bigquery adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
-bigquery Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
-Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
-:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Python: >=3.7 Description-
-Content-Type: text/markdown License-File: LICENSE.md
+Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.6.0b1 Summary: The Bigquery
+adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-bigquery
+Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
+:: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Operating System :: Microsoft :: Windows Classifier:
+Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
+Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Python: >=3.7 Description-Content-Type:
+text/markdown License-File: LICENSE.md
                                   [dbt logo]
                  [Unit_Tests_Badge] [Integration_Tests_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-bigquery The `dbt-bigquery` package contains all of
```

### Comparing `dbt-bigquery-1.5.0rc1/dbt_bigquery.egg-info/SOURCES.txt` & `dbt-bigquery-1.6.0b1/dbt_bigquery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0rc1/setup.py` & `dbt-bigquery-1.6.0b1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     else:
         core_patch = "0"
 
     return f"{major}.{minor}.{core_patch}"
 
 
 package_name = "dbt-bigquery"
-package_version = "1.5.0rc1"
+package_version = "1.6.0b1"
 dbt_core_version = _dbt_core_version(_dbt_bigquery_version())
 description = """The BigQuery adapter plugin for dbt"""
 
 setup(
     name="dbt-bigquery",
     version=_dbt_bigquery_version(),
     description="The Bigquery adapter plugin for dbt",
```


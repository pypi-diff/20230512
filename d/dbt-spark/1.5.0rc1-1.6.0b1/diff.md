# Comparing `tmp/dbt-spark-1.5.0rc1.tar.gz` & `tmp/dbt-spark-1.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-spark-1.5.0rc1.tar", last modified: Sat Apr 22 13:25:25 2023, max compression
+gzip compressed data, was "dbt-spark-1.6.0b1.tar", last modified: Fri May 12 20:59:40 2023, max compression
```

## Comparing `dbt-spark-1.5.0rc1.tar` & `dbt-spark-1.6.0b1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:25:25.038011 dbt-spark-1.5.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-22 13:25:25.038011 dbt-spark-1.5.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:25:25.030011 dbt-spark-1.5.0rc1/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:25:25.030011 dbt-spark-1.5.0rc1/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:25:25.034011 dbt-spark-1.5.0rc1/dbt/adapters/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/adapters/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/adapters/spark/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/adapters/spark/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    21120 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/adapters/spark/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    19924 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/adapters/spark/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/adapters/spark/python_submissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/adapters/spark/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/adapters/spark/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:25:25.030011 dbt-spark-1.5.0rc1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:25:25.034011 dbt-spark-1.5.0rc1/dbt/include/spark/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:25:25.034011 dbt-spark-1.5.0rc1/dbt/include/spark/macros/
--rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/apply_grants.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:25:25.034011 dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:25:25.034011 dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/incremental/validate.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:25:25.038011 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/assert_not_null.sql
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/dbt/include/spark/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 13:25:25.038011 dbt-spark-1.5.0rc1/dbt_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-22 13:25:24.000000 dbt-spark-1.5.0rc1/dbt_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-22 13:25:25.000000 dbt-spark-1.5.0rc1/dbt_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 13:25:24.000000 dbt-spark-1.5.0rc1/dbt_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 13:25:24.000000 dbt-spark-1.5.0rc1/dbt_spark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-22 13:25:24.000000 dbt-spark-1.5.0rc1/dbt_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-22 13:25:24.000000 dbt-spark-1.5.0rc1/dbt_spark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 13:25:25.038011 dbt-spark-1.5.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-04-22 13:25:13.000000 dbt-spark-1.5.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:59:40.069594 dbt-spark-1.6.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-12 20:59:40.069594 dbt-spark-1.6.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:59:40.061594 dbt-spark-1.6.0b1/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:59:40.061594 dbt-spark-1.6.0b1/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:59:40.065594 dbt-spark-1.6.0b1/dbt/adapters/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/adapters/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/adapters/spark/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/adapters/spark/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21120 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/adapters/spark/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19051 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/adapters/spark/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/adapters/spark/python_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/adapters/spark/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/adapters/spark/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:59:40.061594 dbt-spark-1.6.0b1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:59:40.065594 dbt-spark-1.6.0b1/dbt/include/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:59:40.065594 dbt-spark-1.6.0b1/dbt/include/spark/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/apply_grants.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:59:40.065594 dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:59:40.065594 dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:59:40.069594 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/assert_not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/dbt/include/spark/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:59:40.069594 dbt-spark-1.6.0b1/dbt_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-12 20:59:40.000000 dbt-spark-1.6.0b1/dbt_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-12 20:59:40.000000 dbt-spark-1.6.0b1/dbt_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:59:40.000000 dbt-spark-1.6.0b1/dbt_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:59:40.000000 dbt-spark-1.6.0b1/dbt_spark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-12 20:59:40.000000 dbt-spark-1.6.0b1/dbt_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-12 20:59:40.000000 dbt-spark-1.6.0b1/dbt_spark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 20:59:40.069594 dbt-spark-1.6.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-12 20:59:26.000000 dbt-spark-1.6.0b1/setup.py
```

### Comparing `dbt-spark-1.5.0rc1/PKG-INFO` & `dbt-spark-1.6.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-spark
-Version: 1.5.0rc1
+Version: 1.6.0b1
 Summary: The Apache Spark adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-spark Version: 1.5.0rc1 Summary: The Apache
+Metadata-Version: 2.1 Name: dbt-spark Version: 1.6.0b1 Summary: The Apache
 Spark adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dbt-spark-1.5.0rc1/README.md` & `dbt-spark-1.6.0b1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0rc1/dbt/adapters/spark/column.py` & `dbt-spark-1.6.0b1/dbt/adapters/spark/column.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0rc1/dbt/adapters/spark/connections.py` & `dbt-spark-1.6.0b1/dbt/adapters/spark/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0rc1/dbt/adapters/spark/impl.py` & `dbt-spark-1.6.0b1/dbt/adapters/spark/impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,26 +20,23 @@
 from dbt.adapters.spark.python_submissions import (
     JobClusterPythonJobHelper,
     AllPurposeClusterPythonJobHelper,
 )
 from dbt.adapters.base import BaseRelation
 from dbt.clients.agate_helper import DEFAULT_TYPE_TESTER
 from dbt.events import AdapterLogger
-from dbt.flags import get_flags
 from dbt.utils import executor, AttrDict
 
 logger = AdapterLogger("Spark")
 
 GET_COLUMNS_IN_RELATION_RAW_MACRO_NAME = "get_columns_in_relation_raw"
 LIST_SCHEMAS_MACRO_NAME = "list_schemas"
 LIST_RELATIONS_MACRO_NAME = "list_relations_without_caching"
 LIST_RELATIONS_SHOW_TABLES_MACRO_NAME = "list_relations_show_tables_without_caching"
 DESCRIBE_TABLE_EXTENDED_MACRO_NAME = "describe_table_extended_without_caching"
-DROP_RELATION_MACRO_NAME = "drop_relation"
-FETCH_TBL_PROPERTIES_MACRO_NAME = "fetch_tbl_properties"
 
 KEY_TABLE_OWNER = "Owner"
 KEY_TABLE_STATISTICS = "Statistics"
 
 TABLE_OR_VIEW_NOT_FOUND_MESSAGES = (
     "[TABLE_OR_VIEW_NOT_FOUND]",
     "Table or view not found",
@@ -120,26 +117,14 @@
     @classmethod
     def convert_datetime_type(cls, agate_table, col_idx):
         return "timestamp"
 
     def quote(self, identifier):
         return "`{}`".format(identifier)
 
-    def add_schema_to_cache(self, schema) -> str:
-        """Cache a new schema in dbt. It will show up in `list relations`."""
-        if schema is None:
-            name = self.nice_connection_name()
-            raise dbt.exceptions.CompilationError(
-                "Attempted to cache a null schema for {}".format(name)
-            )
-        if get_flags().USE_CACHE:  # type: ignore
-            self.cache.add_schema(None, schema)
-        # so jinja doesn't render things
-        return ""
-
     def _get_relation_information(self, row: agate.Row) -> RelationInfo:
         """relation info was fetched with SHOW TABLES EXTENDED"""
         try:
             _schema, name, _, information = row
         except ValueError:
             raise dbt.exceptions.DbtRuntimeError(
                 f'Invalid value from "show tables extended ...", got {len(row)} values, expected 4'
@@ -186,15 +171,15 @@
             rel_type: RelationType = (
                 RelationType.View if "Type: VIEW" in information else RelationType.Table
             )
             is_delta: bool = "Provider: delta" in information
             is_hudi: bool = "Provider: hudi" in information
             is_iceberg: bool = "Provider: iceberg" in information
 
-            relation: BaseRelation = self.Relation.create(  # type: ignore
+            relation: BaseRelation = self.Relation.create(
                 schema=_schema,
                 identifier=name,
                 type=rel_type,
                 information=information,
                 is_delta=is_delta,
                 is_iceberg=is_iceberg,
                 is_hudi=is_hudi,
@@ -344,20 +329,14 @@
             # convert SparkColumns into catalog dicts
             as_dict = column.to_column_dict()
             as_dict["column_name"] = as_dict.pop("column", None)
             as_dict["column_type"] = as_dict.pop("dtype")
             as_dict["table_database"] = None
             yield as_dict
 
-    def get_properties(self, relation: Relation) -> Dict[str, str]:
-        properties = self.execute_macro(
-            FETCH_TBL_PROPERTIES_MACRO_NAME, kwargs={"relation": relation}
-        )
-        return dict(properties)
-
     def get_catalog(self, manifest):
         schema_map = self._get_catalog_schemas(manifest)
         if len(schema_map) > 1:
             raise dbt.exceptions.CompilationError(
                 f"Expected only one database in get_catalog, found " f"{list(schema_map)}"
             )
 
@@ -407,15 +386,15 @@
     def get_rows_different_sql(
         self,
         relation_a: BaseRelation,
         relation_b: BaseRelation,
         column_names: Optional[List[str]] = None,
         except_operator: str = "EXCEPT",
     ) -> str:
-        """Generate SQL for a query that returns a single row with a two
+        """Generate SQL for a query that returns a single row with two
         columns: the number of rows that are different between the two
         relations and the number of mismatched rows.
         """
         # This method only really exists for test reasons.
         names: List[str]
         if column_names is None:
             columns = self.get_columns_in_relation(relation_a)
```

### Comparing `dbt-spark-1.5.0rc1/dbt/adapters/spark/python_submissions.py` & `dbt-spark-1.6.0b1/dbt/adapters/spark/python_submissions.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0rc1/dbt/adapters/spark/relation.py` & `dbt-spark-1.6.0b1/dbt/adapters/spark/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0rc1/dbt/adapters/spark/session.py` & `dbt-spark-1.6.0b1/dbt/adapters/spark/session.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0rc1/dbt/include/spark/macros/adapters.sql` & `dbt-spark-1.6.0b1/dbt/include/spark/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0rc1/dbt/include/spark/macros/apply_grants.sql` & `dbt-spark-1.6.0b1/dbt/include/spark/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/incremental/column_helpers.sql` & `dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/incremental/incremental.sql` & `dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/incremental/strategies.sql` & `dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/incremental/validate.sql` & `dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/incremental/validate.sql`

 * *Files 6% similar despite different names*

```diff
@@ -36,24 +36,20 @@
   {%- endset %}
 
   {% set invalid_insert_overwrite_endpoint_msg -%}
     Invalid incremental strategy provided: {{ raw_strategy }}
     You cannot use this strategy when connecting via endpoint
     Use the 'append' or 'merge' strategy instead
   {%- endset %}
-
   {% if raw_strategy not in ['append', 'merge', 'insert_overwrite'] %}
     {% do exceptions.raise_compiler_error(invalid_strategy_msg) %}
   {%-else %}
     {% if raw_strategy == 'merge' and file_format not in ['delta', 'iceberg', 'hudi'] %}
       {% do exceptions.raise_compiler_error(invalid_merge_msg) %}
     {% endif %}
-    {% if raw_strategy == 'insert_overwrite' and file_format == 'delta' %}
-      {% do exceptions.raise_compiler_error(invalid_insert_overwrite_delta_msg) %}
-    {% endif %}
     {% if raw_strategy == 'insert_overwrite' and target.endpoint %}
       {% do exceptions.raise_compiler_error(invalid_insert_overwrite_endpoint_msg) %}
     {% endif %}
   {% endif %}
 
   {% do return(raw_strategy) %}
 {% endmacro %}
```

### Comparing `dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/seed.sql` & `dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/snapshot.sql` & `dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0rc1/dbt/include/spark/macros/materializations/table.sql` & `dbt-spark-1.6.0b1/dbt/include/spark/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/dateadd.sql` & `dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/datediff.sql` & `dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/listagg.sql` & `dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0rc1/dbt/include/spark/macros/utils/split_part.sql` & `dbt-spark-1.6.0b1/dbt/include/spark/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0rc1/dbt/include/spark/profile_template.yml` & `dbt-spark-1.6.0b1/dbt/include/spark/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0rc1/dbt_spark.egg-info/PKG-INFO` & `dbt-spark-1.6.0b1/dbt_spark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-spark
-Version: 1.5.0rc1
+Version: 1.6.0b1
 Summary: The Apache Spark adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-spark Version: 1.5.0rc1 Summary: The Apache
+Metadata-Version: 2.1 Name: dbt-spark Version: 1.6.0b1 Summary: The Apache
 Spark adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dbt-spark-1.5.0rc1/dbt_spark.egg-info/SOURCES.txt` & `dbt-spark-1.6.0b1/dbt_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.5.0rc1/setup.py` & `dbt-spark-1.6.0b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,19 +46,19 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-spark"
-package_version = "1.5.0rc1"
+package_version = "1.6.0b1"
 dbt_core_version = _get_dbt_core_version()
 description = """The Apache Spark adapter plugin for dbt"""
 
-odbc_extras = ["pyodbc>=4.0.30"]
+odbc_extras = ["pyodbc~=4.0.30"]
 pyhive_extras = [
     "PyHive[hive]>=0.6.0,<0.7.0",
     "thrift>=0.11.0,<0.17.0",
 ]
 session_extras = ["pyspark>=3.0.0,<4.0.0"]
 all_extras = odbc_extras + pyhive_extras + session_extras
```


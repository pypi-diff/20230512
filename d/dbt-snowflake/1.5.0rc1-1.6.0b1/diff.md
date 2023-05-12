# Comparing `tmp/dbt-snowflake-1.5.0rc1.tar.gz` & `tmp/dbt-snowflake-1.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-snowflake-1.5.0rc1.tar", last modified: Fri Apr 14 21:50:06 2023, max compression
+gzip compressed data, was "dbt-snowflake-1.6.0b1.tar", last modified: Fri May 12 20:22:27 2023, max compression
```

## Comparing `dbt-snowflake-1.5.0rc1.tar` & `dbt-snowflake-1.6.0b1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:50:06.329372 dbt-snowflake-1.5.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-14 21:50:06.329372 dbt-snowflake-1.5.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:50:06.325372 dbt-snowflake-1.5.0rc1/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:50:06.321372 dbt-snowflake-1.5.0rc1/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:50:06.325372 dbt-snowflake-1.5.0rc1/dbt/adapters/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/adapters/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/adapters/snowflake/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/adapters/snowflake/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    20442 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/adapters/snowflake/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/adapters/snowflake/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/adapters/snowflake/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:50:06.321372 dbt-snowflake-1.5.0rc1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:50:06.325372 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:50:06.325372 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/
--rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:50:06.325372 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/materializations/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/materializations/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/materializations/test.sql
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:50:06.325372 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/dbt/include/snowflake/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:50:06.329372 dbt-snowflake-1.5.0rc1/dbt_snowflake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-14 21:50:06.000000 dbt-snowflake-1.5.0rc1/dbt_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-14 21:50:06.000000 dbt-snowflake-1.5.0rc1/dbt_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:50:06.000000 dbt-snowflake-1.5.0rc1/dbt_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:50:06.000000 dbt-snowflake-1.5.0rc1/dbt_snowflake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 21:50:06.000000 dbt-snowflake-1.5.0rc1/dbt_snowflake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-14 21:50:06.000000 dbt-snowflake-1.5.0rc1/dbt_snowflake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 21:50:06.329372 dbt-snowflake-1.5.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-14 21:49:56.000000 dbt-snowflake-1.5.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:22:27.418135 dbt-snowflake-1.6.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-12 20:22:27.418135 dbt-snowflake-1.6.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:22:27.410135 dbt-snowflake-1.6.0b1/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:22:27.406135 dbt-snowflake-1.6.0b1/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:22:27.410135 dbt-snowflake-1.6.0b1/dbt/adapters/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/adapters/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/adapters/snowflake/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/adapters/snowflake/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20478 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/adapters/snowflake/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/adapters/snowflake/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/adapters/snowflake/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:22:27.406135 dbt-snowflake-1.6.0b1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:22:27.410135 dbt-snowflake-1.6.0b1/dbt/include/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:22:27.414135 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:22:27.414135 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/materializations/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/materializations/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/materializations/test.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:22:27.414135 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/dbt/include/snowflake/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:22:27.418135 dbt-snowflake-1.6.0b1/dbt_snowflake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-12 20:22:27.000000 dbt-snowflake-1.6.0b1/dbt_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-12 20:22:27.000000 dbt-snowflake-1.6.0b1/dbt_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:22:27.000000 dbt-snowflake-1.6.0b1/dbt_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:22:27.000000 dbt-snowflake-1.6.0b1/dbt_snowflake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-12 20:22:27.000000 dbt-snowflake-1.6.0b1/dbt_snowflake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-12 20:22:27.000000 dbt-snowflake-1.6.0b1/dbt_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 20:22:27.418135 dbt-snowflake-1.6.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-12 20:22:10.000000 dbt-snowflake-1.6.0b1/setup.py
```

### Comparing `dbt-snowflake-1.5.0rc1/LICENSE.md` & `dbt-snowflake-1.6.0b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.5.0rc1/PKG-INFO` & `dbt-snowflake-1.6.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-snowflake
-Version: 1.5.0rc1
+Version: 1.6.0b1
 Summary: The Snowflake adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-snowflake
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.5.0rc1 Summary: The
+Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.6.0b1 Summary: The
 Snowflake adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
 snowflake Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `dbt-snowflake-1.5.0rc1/README.md` & `dbt-snowflake-1.6.0b1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.5.0rc1/dbt/adapters/snowflake/__init__.py` & `dbt-snowflake-1.6.0b1/dbt/adapters/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.5.0rc1/dbt/adapters/snowflake/column.py` & `dbt-snowflake-1.6.0b1/dbt/adapters/snowflake/column.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.5.0rc1/dbt/adapters/snowflake/connections.py` & `dbt-snowflake-1.6.0b1/dbt/adapters/snowflake/connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -424,22 +424,22 @@
                 fixed_row.append(col)
 
             fixed.append(fixed_row)
 
         return super().process_results(column_names, fixed)
 
     def execute(
-        self, sql: str, auto_begin: bool = False, fetch: bool = False
+        self, sql: str, auto_begin: bool = False, fetch: bool = False, limit: Optional[int] = None
     ) -> Tuple[AdapterResponse, agate.Table]:
         # don't apply the query comment here
         # it will be applied after ';' queries are split
         _, cursor = self.add_query(sql, auto_begin)
         response = self.get_response(cursor)
         if fetch:
-            table = self.get_result_from_cursor(cursor)
+            table = self.get_result_from_cursor(cursor, limit)
         else:
             table = dbt.clients.agate_helper.empty_table()
         return response, table
 
     def add_standard_query(self, sql: str, **kwargs) -> Tuple[Connection, Any]:
         # This is the happy path for a single query. Snowflake has a few odd behaviors that
         # require preprocessing within the 'add_query' method below.
```

### Comparing `dbt-snowflake-1.5.0rc1/dbt/adapters/snowflake/impl.py` & `dbt-snowflake-1.6.0b1/dbt/adapters/snowflake/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/adapters.sql` & `dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/adapters.sql`

 * *Files 17% similar despite different names*

```diff
@@ -146,29 +146,98 @@
     {% endset %}
     {% do exceptions.raise_compiler_error(msg) %}
   {% endif %}
   {{ return(result) }}
 {% endmacro %}
 
 
-{% macro snowflake__list_relations_without_caching(schema_relation) %}
+{% macro snowflake__get_paginated_relations_array(max_iter, max_results_per_iter, max_total_results, schema_relation, watermark) %}
+
+  {% set paginated_relations = [] %}
+
+  {% for _ in range(0, max_iter) %}
+
+      {%- set paginated_sql -%}
+         show terse objects in {{ schema_relation }} limit {{ max_results_per_iter }} from '{{ watermark.table_name }}'
+      {%- endset -%}
+
+      {%- set paginated_result = run_query(paginated_sql) %}
+      {%- set paginated_n = (paginated_result | length) -%}
+
+      {#
+        terminating condition: if there are 0 records in the result we reached
+        the end exactly on the previous iteration
+      #}
+      {%- if paginated_n == 0 -%}
+        {%- break -%}
+      {%- endif -%}
+
+      {#
+        terminating condition: At some point the user needs to be reasonable with how
+        many objects are contained in their schemas. Since there was already
+        one iteration before attempting pagination, loop.index == max_iter means
+        the limit has been surpassed.
+      #}
+
+      {%- if loop.index == max_iter -%}
+        {%- set msg -%}
+           dbt will list a maximum of {{ max_total_results }} objects in schema {{ schema_relation }}.
+           Your schema exceeds this limit. Please contact support@getdbt.com for troubleshooting tips,
+           or review and reduce the number of objects contained.
+        {%- endset -%}
+
+        {% do exceptions.raise_compiler_error(msg) %}
+      {%- endif -%}
+
+      {%- do paginated_relations.append(paginated_result) -%}
+      {% set watermark.table_name = paginated_result.columns[1].values()[-1] %}
+
+      {#
+        terminating condition: paginated_n < max_results_per_iter means we reached the end
+      #}
+      {%- if paginated_n < max_results_per_iter -%}
+         {%- break -%}
+      {%- endif -%}
+    {%- endfor -%}
+
+  {{ return(paginated_relations) }}
+
+{% endmacro %}
+
+{% macro snowflake__list_relations_without_caching(schema_relation, max_iter=10, max_results_per_iter=10000) %}
+
+  {%- set max_total_results = max_results_per_iter * max_iter -%}
+
   {%- set sql -%}
-    show terse objects in {{ schema_relation }}
+    show terse objects in {{ schema_relation }} limit {{ max_results_per_iter }}
   {%- endset -%}
 
   {%- set result = run_query(sql) -%}
-  {% set maximum = 10000 %}
-  {% if (result | length) >= maximum %}
-    {% set msg %}
-      Too many objects in schema  {{ schema_relation }}! dbt can only get
-      information about schemas with fewer than {{ maximum }} objects.
-    {% endset %}
-    {% do exceptions.raise_compiler_error(msg) %}
+
+  {%- set n = (result | length) -%}
+  {%- set watermark = namespace(table_name=result.columns[1].values()[-1]) -%}
+  {%- set paginated = namespace(result=[]) -%}
+
+  {% if n >= max_results_per_iter %}
+
+    {% set paginated.result = snowflake__get_paginated_relations_array(
+         max_iter,
+         max_results_per_iter,
+         max_total_results,
+         schema_relation,
+         watermark
+       )
+    %}
+
   {% endif %}
+
+  {%- set all_results_array = [result] + paginated.result -%}
+  {%- set result = result.merge(all_results_array) -%}
   {%- do return(result) -%}
+
 {% endmacro %}
 
 
 {% macro snowflake__check_schema_exists(information_schema, schema) -%}
   {% call statement('check_schema_exists', fetch_result=True) -%}
         select count(*)
         from {{ information_schema }}.schemata
```

### Comparing `dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/catalog.sql` & `dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/materializations/incremental.sql` & `dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/materializations/merge.sql` & `dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/materializations/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/materializations/seed.sql` & `dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/materializations/table.sql` & `dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.5.0rc1/dbt/include/snowflake/macros/utils/timestamps.sql` & `dbt-snowflake-1.6.0b1/dbt/include/snowflake/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.5.0rc1/dbt/include/snowflake/profile_template.yml` & `dbt-snowflake-1.6.0b1/dbt/include/snowflake/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.5.0rc1/dbt_snowflake.egg-info/PKG-INFO` & `dbt-snowflake-1.6.0b1/dbt_snowflake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-snowflake
-Version: 1.5.0rc1
+Version: 1.6.0b1
 Summary: The Snowflake adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-snowflake
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.5.0rc1 Summary: The
+Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.6.0b1 Summary: The
 Snowflake adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
 snowflake Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `dbt-snowflake-1.5.0rc1/dbt_snowflake.egg-info/SOURCES.txt` & `dbt-snowflake-1.6.0b1/dbt_snowflake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.5.0rc1/setup.py` & `dbt-snowflake-1.6.0b1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-snowflake"
-package_version = "1.5.0rc1"
+package_version = "1.6.0b1"
 dbt_core_version = _get_dbt_core_version()
 description = """The Snowflake adapter plugin for dbt"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
```


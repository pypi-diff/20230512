# Comparing `tmp/dbt-redshift-1.5.1.tar.gz` & `tmp/dbt-redshift-1.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-redshift-1.5.1.tar", last modified: Wed May  3 17:50:00 2023, max compression
+gzip compressed data, was "dbt-redshift-1.6.0b1.tar", last modified: Fri May 12 19:51:48 2023, max compression
```

## Comparing `dbt-redshift-1.5.1.tar` & `dbt-redshift-1.6.0b1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:50:00.372565 dbt-redshift-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-03 17:50:00.372565 dbt-redshift-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:50:00.364565 dbt-redshift-1.5.1/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:50:00.364565 dbt-redshift-1.5.1/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:50:00.364565 dbt-redshift-1.5.1/dbt/adapters/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/adapters/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/adapters/redshift/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/adapters/redshift/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/adapters/redshift/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/adapters/redshift/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/adapters/redshift/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:50:00.364565 dbt-redshift-1.5.1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:50:00.368565 dbt-redshift-1.5.1/dbt/include/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:50:00.368565 dbt-redshift-1.5.1/dbt/include/redshift/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:50:00.368565 dbt-redshift-1.5.1/dbt/include/redshift/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:50:00.368565 dbt-redshift-1.5.1/dbt/include/redshift/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/materializations/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/relations.sql
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:50:00.368565 dbt-redshift-1.5.1/dbt/include/redshift/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/dbt/include/redshift/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:50:00.372565 dbt-redshift-1.5.1/dbt_redshift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-03 17:50:00.000000 dbt-redshift-1.5.1/dbt_redshift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-03 17:50:00.000000 dbt-redshift-1.5.1/dbt_redshift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 17:50:00.000000 dbt-redshift-1.5.1/dbt_redshift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 17:50:00.000000 dbt-redshift-1.5.1/dbt_redshift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-03 17:50:00.000000 dbt-redshift-1.5.1/dbt_redshift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-03 17:50:00.000000 dbt-redshift-1.5.1/dbt_redshift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 17:50:00.372565 dbt-redshift-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-03 17:49:47.000000 dbt-redshift-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:51:48.777905 dbt-redshift-1.6.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-12 19:51:48.777905 dbt-redshift-1.6.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:51:48.773905 dbt-redshift-1.6.0b1/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:51:48.773905 dbt-redshift-1.6.0b1/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:51:48.773905 dbt-redshift-1.6.0b1/dbt/adapters/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/adapters/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/adapters/redshift/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/adapters/redshift/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11710 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/adapters/redshift/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/adapters/redshift/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/adapters/redshift/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:51:48.773905 dbt-redshift-1.6.0b1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:51:48.773905 dbt-redshift-1.6.0b1/dbt/include/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:51:48.773905 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:51:48.773905 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:51:48.773905 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/materializations/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/relations.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:51:48.777905 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/dbt/include/redshift/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:51:48.777905 dbt-redshift-1.6.0b1/dbt_redshift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-12 19:51:48.000000 dbt-redshift-1.6.0b1/dbt_redshift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-12 19:51:48.000000 dbt-redshift-1.6.0b1/dbt_redshift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 19:51:48.000000 dbt-redshift-1.6.0b1/dbt_redshift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 19:51:48.000000 dbt-redshift-1.6.0b1/dbt_redshift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-12 19:51:48.000000 dbt-redshift-1.6.0b1/dbt_redshift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-12 19:51:48.000000 dbt-redshift-1.6.0b1/dbt_redshift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 19:51:48.777905 dbt-redshift-1.6.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-12 19:51:34.000000 dbt-redshift-1.6.0b1/setup.py
```

### Comparing `dbt-redshift-1.5.1/LICENSE.md` & `dbt-redshift-1.6.0b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.1/PKG-INFO` & `dbt-redshift-1.6.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-redshift
-Version: 1.5.1
+Version: 1.6.0b1
 Summary: The Redshift adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-redshift Version: 1.5.1 Summary: The Redshift
+Metadata-Version: 2.1 Name: dbt-redshift Version: 1.6.0b1 Summary: The Redshift
 adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dbt-redshift-1.5.1/README.md` & `dbt-redshift-1.6.0b1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.1/dbt/adapters/redshift/__init__.py` & `dbt-redshift-1.6.0b1/dbt/adapters/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.1/dbt/adapters/redshift/connections.py` & `dbt-redshift-1.6.0b1/dbt/adapters/redshift/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,20 +295,24 @@
             logger=logger,
             retry_limit=credentials.retries,
             retry_timeout=exponential_backoff,
             retryable_exceptions=retryable_exceptions,
         )
 
     def execute(
-        self, sql: str, auto_begin: bool = False, fetch: bool = False
+        self,
+        sql: str,
+        auto_begin: bool = False,
+        fetch: bool = False,
+        limit: Optional[int] = None,
     ) -> Tuple[AdapterResponse, agate.Table]:
         _, cursor = self.add_query(sql, auto_begin)
         response = self.get_response(cursor)
         if fetch:
-            table = self.get_result_from_cursor(cursor)
+            table = self.get_result_from_cursor(cursor, limit)
         else:
             table = dbt.clients.agate_helper.empty_table()
         return response, table
 
     def add_query(self, sql, auto_begin=True, bindings=None, abridge_sql_log=False):
         connection = None
         cursor = None
```

### Comparing `dbt-redshift-1.5.1/dbt/adapters/redshift/impl.py` & `dbt-redshift-1.6.0b1/dbt/adapters/redshift/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.1/dbt/adapters/redshift/relation.py` & `dbt-redshift-1.6.0b1/dbt/adapters/redshift/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.1/dbt/include/redshift/macros/adapters/apply_grants.sql` & `dbt-redshift-1.6.0b1/dbt/include/redshift/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.1/dbt/include/redshift/macros/adapters.sql` & `dbt-redshift-1.6.0b1/dbt/include/redshift/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.1/dbt/include/redshift/macros/catalog.sql` & `dbt-redshift-1.6.0b1/dbt/include/redshift/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.1/dbt/include/redshift/macros/utils/listagg.sql` & `dbt-redshift-1.6.0b1/dbt/include/redshift/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.1/dbt/include/redshift/profile_template.yml` & `dbt-redshift-1.6.0b1/dbt/include/redshift/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.1/dbt_redshift.egg-info/PKG-INFO` & `dbt-redshift-1.6.0b1/dbt_redshift.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-redshift
-Version: 1.5.1
+Version: 1.6.0b1
 Summary: The Redshift adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-redshift Version: 1.5.1 Summary: The Redshift
+Metadata-Version: 2.1 Name: dbt-redshift Version: 1.6.0b1 Summary: The Redshift
 adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dbt-redshift-1.5.1/dbt_redshift.egg-info/SOURCES.txt` & `dbt-redshift-1.6.0b1/dbt_redshift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.5.1/setup.py` & `dbt-redshift-1.6.0b1/setup.py`

 * *Files identical despite different names*


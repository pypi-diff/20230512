# Comparing `tmp/syncanysql-0.1.2.tar.gz` & `tmp/syncanysql-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncanysql-0.1.2.tar", last modified: Tue May  2 08:49:22 2023, max compression
+gzip compressed data, was "syncanysql-0.1.3.tar", last modified: Fri May 12 09:49:37 2023, max compression
```

## Comparing `syncanysql-0.1.2.tar` & `syncanysql-0.1.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:49:22.828186 syncanysql-0.1.2/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4345 2023-05-02 08:49:22.829187 syncanysql-0.1.2/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3018 2023-04-25 10:14:55.000000 syncanysql-0.1.2/README.md
--rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-05-02 08:49:22.841188 syncanysql-0.1.2/setup.cfg
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2030 2023-04-29 02:34:28.000000 syncanysql-0.1.2/setup.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:49:21.453193 syncanysql-0.1.2/syncanysql/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     9167 2023-04-26 01:56:02.000000 syncanysql-0.1.2/syncanysql/__init__.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:49:21.883188 syncanysql-0.1.2/syncanysql/calculaters/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1130 2023-04-23 06:35:38.000000 syncanysql-0.1.2/syncanysql/calculaters/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6152 2023-03-25 11:43:14.000000 syncanysql-0.1.2/syncanysql/calculaters/aggregate_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1207 2023-04-23 06:39:00.000000 syncanysql-0.1.2/syncanysql/calculaters/mysql_calculater.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:49:22.251187 syncanysql-0.1.2/syncanysql/calculaters/mysql_funcs/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      320 2023-03-14 09:33:57.000000 syncanysql-0.1.2/syncanysql/calculaters/mysql_funcs/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    10157 2023-04-20 04:07:01.000000 syncanysql-0.1.2/syncanysql/calculaters/mysql_funcs/datetime_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6002 2023-04-20 03:57:39.000000 syncanysql-0.1.2/syncanysql/calculaters/mysql_funcs/json_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6193 2023-04-24 06:11:11.000000 syncanysql-0.1.2/syncanysql/calculaters/mysql_funcs/number_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6461 2023-04-24 07:12:16.000000 syncanysql-0.1.2/syncanysql/calculaters/mysql_funcs/string_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)   133990 2023-05-01 03:18:26.000000 syncanysql-0.1.2/syncanysql/compiler.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    12804 2023-04-27 09:12:49.000000 syncanysql-0.1.2/syncanysql/config.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      229 2023-02-08 10:09:29.000000 syncanysql-0.1.2/syncanysql/errors.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7755 2023-04-27 09:10:45.000000 syncanysql-0.1.2/syncanysql/executor.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3750 2023-04-26 01:56:02.000000 syncanysql-0.1.2/syncanysql/main.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4366 2023-03-01 11:22:09.000000 syncanysql-0.1.2/syncanysql/parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6965 2023-04-27 09:10:45.000000 syncanysql-0.1.2/syncanysql/prompt.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:49:22.783187 syncanysql-0.1.2/syncanysql/taskers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)       59 2023-02-13 05:49:03.000000 syncanysql-0.1.2/syncanysql/taskers/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1356 2023-03-29 02:07:07.000000 syncanysql-0.1.2/syncanysql/taskers/delete.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1603 2023-04-24 02:15:57.000000 syncanysql-0.1.2/syncanysql/taskers/execute.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1325 2023-04-28 03:17:36.000000 syncanysql-0.1.2/syncanysql/taskers/explain.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4258 2023-04-26 01:31:23.000000 syncanysql-0.1.2/syncanysql/taskers/into.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    21238 2023-05-01 03:07:04.000000 syncanysql-0.1.2/syncanysql/taskers/query.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2744 2023-03-29 02:07:49.000000 syncanysql-0.1.2/syncanysql/taskers/set.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2143 2023-03-29 02:06:08.000000 syncanysql-0.1.2/syncanysql/taskers/show.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1221 2023-04-25 04:04:01.000000 syncanysql-0.1.2/syncanysql/taskers/use.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      641 2023-02-19 14:49:39.000000 syncanysql-0.1.2/syncanysql/utils.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      106 2023-04-29 02:34:28.000000 syncanysql-0.1.2/syncanysql/version.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-02 08:49:21.706187 syncanysql-0.1.2/syncanysql.egg-info/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4345 2023-05-02 08:49:20.000000 syncanysql-0.1.2/syncanysql.egg-info/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1111 2023-05-02 08:49:20.000000 syncanysql-0.1.2/syncanysql.egg-info/SOURCES.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-05-02 08:49:20.000000 syncanysql-0.1.2/syncanysql.egg-info/dependency_links.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       54 2023-05-02 08:49:20.000000 syncanysql-0.1.2/syncanysql.egg-info/entry_points.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-25 10:06:25.000000 syncanysql-0.1.2/syncanysql.egg-info/not-zip-safe
--rwxrwxrwx   0 snower    (1000) snower    (1000)      407 2023-05-02 08:49:20.000000 syncanysql-0.1.2/syncanysql.egg-info/requires.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2023-05-02 08:49:20.000000 syncanysql-0.1.2/syncanysql.egg-info/top_level.txt
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:49:37.662877 syncanysql-0.1.3/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4345 2023-05-12 09:49:37.664874 syncanysql-0.1.3/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3018 2023-04-25 10:14:55.000000 syncanysql-0.1.3/README.md
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-05-12 09:49:37.672875 syncanysql-0.1.3/setup.cfg
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2002 2023-05-08 07:06:40.000000 syncanysql-0.1.3/setup.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:49:36.232618 syncanysql-0.1.3/syncanysql/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     9167 2023-04-26 01:56:02.000000 syncanysql-0.1.3/syncanysql/__init__.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:49:36.723836 syncanysql-0.1.3/syncanysql/calculaters/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1130 2023-04-23 06:35:38.000000 syncanysql-0.1.3/syncanysql/calculaters/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6152 2023-03-25 11:43:14.000000 syncanysql-0.1.3/syncanysql/calculaters/aggregate_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1207 2023-04-23 06:39:00.000000 syncanysql-0.1.3/syncanysql/calculaters/mysql_calculater.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:49:37.095112 syncanysql-0.1.3/syncanysql/calculaters/mysql_funcs/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      320 2023-03-14 09:33:57.000000 syncanysql-0.1.3/syncanysql/calculaters/mysql_funcs/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    10197 2023-05-04 10:22:31.000000 syncanysql-0.1.3/syncanysql/calculaters/mysql_funcs/datetime_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6002 2023-04-20 03:57:39.000000 syncanysql-0.1.3/syncanysql/calculaters/mysql_funcs/json_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6193 2023-04-24 06:11:11.000000 syncanysql-0.1.3/syncanysql/calculaters/mysql_funcs/number_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6461 2023-04-24 07:12:16.000000 syncanysql-0.1.3/syncanysql/calculaters/mysql_funcs/string_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)   135990 2023-05-04 10:48:36.000000 syncanysql-0.1.3/syncanysql/compiler.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12804 2023-05-08 04:32:02.000000 syncanysql-0.1.3/syncanysql/config.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      229 2023-02-08 10:09:29.000000 syncanysql-0.1.3/syncanysql/errors.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8446 2023-05-08 04:35:48.000000 syncanysql-0.1.3/syncanysql/executor.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3750 2023-04-26 01:56:02.000000 syncanysql-0.1.3/syncanysql/main.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4366 2023-03-01 11:22:09.000000 syncanysql-0.1.3/syncanysql/parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6965 2023-04-27 09:10:45.000000 syncanysql-0.1.3/syncanysql/prompt.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:49:37.619874 syncanysql-0.1.3/syncanysql/taskers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       59 2023-02-13 05:49:03.000000 syncanysql-0.1.3/syncanysql/taskers/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1356 2023-03-29 02:07:07.000000 syncanysql-0.1.3/syncanysql/taskers/delete.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1603 2023-04-24 02:15:57.000000 syncanysql-0.1.3/syncanysql/taskers/execute.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1325 2023-04-28 03:17:36.000000 syncanysql-0.1.3/syncanysql/taskers/explain.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4258 2023-04-26 01:31:23.000000 syncanysql-0.1.3/syncanysql/taskers/into.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    21231 2023-05-04 02:54:58.000000 syncanysql-0.1.3/syncanysql/taskers/query.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2890 2023-05-08 04:04:28.000000 syncanysql-0.1.3/syncanysql/taskers/set.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2143 2023-03-29 02:06:08.000000 syncanysql-0.1.3/syncanysql/taskers/show.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1221 2023-04-25 04:04:01.000000 syncanysql-0.1.3/syncanysql/taskers/use.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      754 2023-05-08 04:04:28.000000 syncanysql-0.1.3/syncanysql/utils.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      106 2023-05-04 02:34:02.000000 syncanysql-0.1.3/syncanysql/version.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:49:36.542839 syncanysql-0.1.3/syncanysql.egg-info/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4345 2023-05-12 09:49:34.000000 syncanysql-0.1.3/syncanysql.egg-info/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1111 2023-05-12 09:49:35.000000 syncanysql-0.1.3/syncanysql.egg-info/SOURCES.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-05-12 09:49:34.000000 syncanysql-0.1.3/syncanysql.egg-info/dependency_links.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       54 2023-05-12 09:49:35.000000 syncanysql-0.1.3/syncanysql.egg-info/entry_points.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-25 10:06:25.000000 syncanysql-0.1.3/syncanysql.egg-info/not-zip-safe
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      390 2023-05-12 09:49:35.000000 syncanysql-0.1.3/syncanysql.egg-info/requires.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2023-05-12 09:49:35.000000 syncanysql-0.1.3/syncanysql.egg-info/top_level.txt
```

### Comparing `syncanysql-0.1.2/PKG-INFO` & `syncanysql-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanysql
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple and easy-to-use sql execution engine
 Home-page: https://github.com/snower/syncany-sql
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # Syncany-SQL
         [![Tests](https://img.shields.io/github/actions/workflow/status/snower/syncany-sql/ci.yml?label=tests)](https://github.com/snower/syncany-sql/actions/workflows/ci.yml)
```

### Comparing `syncanysql-0.1.2/README.md` & `syncanysql-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.2/setup.py` & `syncanysql-0.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 23/02/07
 # create by: snower
 
 import sys
 import os
 from setuptools import find_packages, setup
 
-version = "0.1.2"
+version = "0.1.3"
 
 if os.path.exists("README.md"):
     if sys.version_info[0] >= 3:
         try:
             with open("README.md", encoding="utf-8") as fp:
                 long_description = fp.read()
         except Exception as e:
@@ -34,16 +34,15 @@
     author_email='sujian199@gmail.com',
     license='MIT',
     packages=find_packages(exclude=['*tests*']),
     zip_safe=False,
     install_requires=[
         "pyyaml>=5.1.2",
         "sqlglot>=10.6.2",
-        "syncany>=0.2.8",
-        'Pygments>=2.14.0',
+        "syncany>=0.2.9",
         'Pygments>=2.14.0',
         'prompt-toolkit>=3.0.36',
         "rich>=9.11.1",
     ],
     extras_require={
         "pymongo": ['pymongo>=3.6.1'],
         "pymysql": ['PyMySQL>=0.8.1'],
```

### Comparing `syncanysql-0.1.2/syncanysql/__init__.py` & `syncanysql-0.1.3/syncanysql/__init__.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.2/syncanysql/calculaters/__init__.py` & `syncanysql-0.1.3/syncanysql/calculaters/__init__.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.2/syncanysql/calculaters/aggregate_calculater.py` & `syncanysql-0.1.3/syncanysql/calculaters/aggregate_calculater.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.2/syncanysql/calculaters/mysql_calculater.py` & `syncanysql-0.1.3/syncanysql/calculaters/mysql_calculater.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.2/syncanysql/calculaters/mysql_funcs/datetime_funcs.py` & `syncanysql-0.1.3/syncanysql/calculaters/mysql_funcs/datetime_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,22 +254,22 @@
     return int((dt2 - dt1).total_seconds() / 86400)
 
 def mysql_date_format(dt, f):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime(str(dt), None, get_timezone())
-    return dt.strftime(f)
+    return dt.strftime(f.replace("%v", "%V"))
 
 def mysql_time_format(dt, f):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime("2000-01-01 " + str(dt), None, get_timezone())
-    return dt.strftime(f)
+    return dt.strftime(f.replace("%v", "%V"))
 
 def mysql_weekday(dt):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime(str(dt), None, get_timezone())
     return dt.weekday()
```

### Comparing `syncanysql-0.1.2/syncanysql/calculaters/mysql_funcs/json_funcs.py` & `syncanysql-0.1.3/syncanysql/calculaters/mysql_funcs/json_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.2/syncanysql/calculaters/mysql_funcs/number_funcs.py` & `syncanysql-0.1.3/syncanysql/calculaters/mysql_funcs/number_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.2/syncanysql/calculaters/mysql_funcs/string_funcs.py` & `syncanysql-0.1.3/syncanysql/calculaters/mysql_funcs/string_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.2/syncanysql/compiler.py` & `syncanysql-0.1.3/syncanysql/compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -559,15 +559,15 @@
                 primary_table["loader_primary_keys"], primary_table["outputer_primary_keys"], primary_table["seted_primary_keys"] = [], [], True
             primary_table["loader_primary_keys"].append(column_info["column_name"])
             primary_table["outputer_primary_keys"].append(column_alias)
         elif not primary_table["seted_primary_keys"] and not primary_table["outputer_primary_keys"]:
             if not column_info["table_name"] or column_info["table_name"] == primary_table["table_name"]:
                 primary_table["loader_primary_keys"], primary_table["outputer_primary_keys"] = [column_info["column_name"]], [column_alias]
 
-    def compile_select_calculate_column(self, expression, config, arguments, primary_table, column_alias, join_tables):
+    def compile_select_calculate_column(self, expression, config, arguments, primary_table, column_alias, join_tables, parse_primary_key=True):
         calculate_fields = []
         self.parse_calculate(expression, config, arguments, primary_table, calculate_fields)
         calculate_table_names = set([])
         for calculate_field in calculate_fields:
             if not calculate_field["table_name"] or calculate_field["table_name"] == primary_table["table_name"]:
                 continue
             if calculate_field["table_name"] not in join_tables:
@@ -580,15 +580,16 @@
                                             [join_tables[calculate_table_name] for calculate_table_name in calculate_table_names],
                                             join_tables, column_join_tables)
             calculate_column = self.compile_calculate(expression, config, arguments, primary_table, column_join_tables)
             config["schema"][column_alias] = self.compile_join_column(expression, config, arguments, primary_table,
                                                                       calculate_column, column_join_tables)
         else:
             config["schema"][column_alias] = self.compile_calculate(expression, config, arguments, primary_table, [])
-        if not primary_table["seted_primary_keys"] and not primary_table["outputer_primary_keys"] and column_alias.isidentifier():
+        if parse_primary_key and not primary_table["seted_primary_keys"] and not primary_table["outputer_primary_keys"] \
+                and column_alias.isidentifier():
             loader_primary_keys = [calculate_field["column_name"] for calculate_field in calculate_fields
                                    if calculate_field["column_name"].isidentifier() and
                                    (not calculate_field["table_name"] or calculate_field["table_name"] == primary_table["table_name"])]
             if loader_primary_keys:
                 primary_table["loader_primary_keys"], primary_table["outputer_primary_keys"] = loader_primary_keys, [column_alias]
 
     def compile_join_column_tables(self, expression, config, arguments, primary_table, current_join_tables, join_tables,
@@ -657,15 +658,15 @@
 
         def parse_calucate(calculate_expression):
             if not isinstance(config.get("schema"), dict):
                 return calculate_expression
             if self.is_column(calculate_expression, config, arguments):
                 calculate_name = "__where_condition_value_%d__" % id(calculate_expression)
                 self.compile_select_calculate_column(calculate_expression, config, arguments, primary_table,
-                                                     calculate_name, join_tables)
+                                                     calculate_name, join_tables, False)
                 setattr(calculate_expression, "syncany_valuer", ["$." + calculate_name])
                 if "where_schema" not in config:
                     config["where_schema"] = {}
                 config["where_schema"][calculate_name] = copy.deepcopy(config["schema"][calculate_name])
                 return calculate_expression
             if not self.is_calculate(calculate_expression, config, arguments):
                 return calculate_expression
@@ -803,14 +804,16 @@
                 raise SyncanySqlCompileException(
                     'error having condition, like condition value must be const, related sql "%s"'
                     % self.to_sql(expression))
             return ["#if", ["@re::match", right_calculater[1].replace("%", ".*").replace(".*.*", "%"), left_calculater],
                     ["#const", True], ["#const", False]]
         elif isinstance(expression, (sqlglot_expressions.Not, sqlglot_expressions.Is)):
             return self.compile_calculate(parse_calucate(expression), config, arguments, primary_table, [])
+        elif isinstance(expression, sqlglot_expressions.Between):
+            return self.compile_calculate(parse_calucate(expression), config, arguments, primary_table, [])
         elif isinstance(expression, sqlglot_expressions.Paren):
             return self.compile_where_condition(expression.args.get("this"), config, arguments, primary_table, join_tables, False)
         else:
             raise SyncanySqlCompileException('unknown where condition, only "=,!=,>,>=,<,<=,in" operations are supported, related sql "%s"'
                                              % self.to_sql(expression))
 
     def compile_query_condition(self, expression, config, arguments, primary_table, typing_filters):
@@ -978,15 +981,16 @@
                                                                       "$$.value." + aggregate_value_key]
                 reduce_column[1][aggregate_value_key] = [reduce_calculate,
                                                                    "$." + column_alias + "." + aggregate_value_key,
                                                                    "$$." + column_alias + "." + aggregate_value_key]
                 setattr(aggregate_expressions[i], "syncany_valuer",
                         [final_calculate, "$." + column_alias + "." + aggregate_value_key]
                         if final_calculate else ("$." + column_alias + "." + aggregate_value_key))
-            self.compile_select_calculate_column(expression, config, arguments, primary_table, column_alias, join_tables)
+            self.compile_select_calculate_column(expression, config, arguments, primary_table, column_alias,
+                                                 join_tables, False)
             aggregate_column = {
                 "key": group_column,
                 "value": value_column,
                 "calculate": calculate_column,
                 "aggregate": [":#aggregate", "$.key", copy.deepcopy(calculate_column)],
                 "reduce": reduce_column,
                 "final_value": config["schema"][column_alias]
@@ -1001,14 +1005,24 @@
 
     def compile_aggregate_key(self, expression, config, arguments, primary_table, join_tables):
         if not expression:
             return ["@aggregate_key", ["#const", "__k_g__"]]
 
         group_column = ["@aggregate_key"]
         for group_expression in expression.args["expressions"]:
+            if self.is_column(group_expression, config, arguments):
+                group_expression_column = self.parse_column(group_expression, config, arguments)
+                if isinstance(config["schema"], dict) and not group_expression_column["table_name"] \
+                        and primary_table["table_alias"] and group_expression_column["column_name"] in config["schema"]:
+                    group_column.append(config["schema"][group_expression_column["column_name"]])
+                    continue
+                if not group_expression_column["table_name"] or group_expression_column["table_name"] == primary_table["table_name"]:
+                    group_column.append(self.compile_column(group_expression, config, arguments, group_expression_column))
+                    continue
+
             calculate_fields = []
             self.parse_calculate(group_expression, config, arguments, primary_table, calculate_fields)
             calculate_fields = [calculate_field for calculate_field in calculate_fields if calculate_field["table_name"]
                                 and calculate_field["table_name"] != primary_table["table_name"]]
             if not calculate_fields:
                 group_column.append(self.compile_calculate(group_expression, config, arguments, primary_table, []))
                 continue
@@ -1181,14 +1195,16 @@
                 typing_filter = None
             value_column = self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index)
             if typing_filter:
                 return ["#if", ["#const", True], value_column, None, ":$.*|" + typing_filter]
             return value_column
         elif isinstance(expression, sqlglot_expressions.Binary):
             func_name = expression.key.lower()
+            if isinstance(expression.args["expression"], sqlglot_expressions.Interval):
+                func_name = "date" + func_name
             return [
                 ("@mysql::" + func_name) if is_mysql_func(func_name) else ("@" + func_name),
                 self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index),
                 self.compile_calculate(expression.args["expression"], config, arguments, primary_table, column_join_tables, join_index)
             ]
         elif isinstance(expression, sqlglot_expressions.BitwiseNot):
             func_name = expression.key.lower()
@@ -1256,14 +1272,20 @@
         elif isinstance(expression, sqlglot_expressions.Distinct):
             return [self.compile_calculate(distinct_expression, config, arguments, primary_table, column_join_tables, join_index)
                     for distinct_expression in expression.args["expressions"]]
         elif isinstance(expression, (sqlglot_expressions.Select, sqlglot_expressions.Subquery, sqlglot_expressions.Union)):
             return self.compile_query_condition(expression, config, arguments, primary_table, None)
         elif isinstance(expression, sqlglot_expressions.Paren):
             return self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index)
+        elif isinstance(expression, sqlglot_expressions.Between):
+            return ["#make", {
+                "key_value": self.compile_calculate(expression.args["this"], config, arguments, primary_table, []),
+                "low_value": self.compile_calculate(expression.args["low"], config, arguments, primary_table, []),
+                "high_value": self.compile_calculate(expression.args["high"], config, arguments, primary_table, [])
+            }, [":@and", ["@gte", "$.key_value", "$.low_value"], ["@lte", "$.key_value", "$.high_value"]]]
         elif isinstance(expression, sqlglot_expressions.Not):
             return ["@not", self.compile_calculate(expression.args["this"], config, arguments, primary_table,
                                                    column_join_tables, join_index)]
         elif self.is_column(expression, config, arguments):
             join_column = self.parse_column(expression, config, arguments)
             return self.compile_join_column_field(expression, config, arguments, primary_table, join_index, 
                                                   join_column, column_join_tables)
@@ -1384,14 +1406,16 @@
             if not isinstance(right_calculater, list) or len(right_calculater) != 2 or right_calculater[0] != "#const":
                 raise SyncanySqlCompileException('error having condition, like condition value must be const, related sql "%s"'
                                                  % self.to_sql(expression))
             return ["#if", ["@re::match", right_calculater[1].replace("%", ".*").replace(".*.*", "%"), left_calculater],
                     ["#const", True], ["#const", False]]
         elif isinstance(expression, (sqlglot_expressions.Not, sqlglot_expressions.Is)):
             return self.compile_calculate(expression, config, arguments, primary_table, [])
+        elif isinstance(expression, sqlglot_expressions.Between):
+            return self.compile_calculate(expression, config, arguments, primary_table, [])
         elif isinstance(expression, sqlglot_expressions.Paren):
             return self.compile_having_condition(expression.args.get("this"), config, arguments, primary_table)
         else:
             raise SyncanySqlCompileException('unknown having condition, related sql "%s"' % self.to_sql(expression))
 
     def compile_order(self, expression, config, arguments, primary_table):
         primary_sort_keys, sort_keys = [], []
@@ -1958,16 +1982,16 @@
             return not isinstance(expression.args["this"], sqlglot_expressions.Neg) and self.is_const(expression.args["this"], config, arguments)
         return isinstance(expression, (sqlglot_expressions.Literal, sqlglot_expressions.Boolean,
                                        sqlglot_expressions.Null, sqlglot_expressions.HexString, sqlglot_expressions.BitString,
                                        sqlglot_expressions.ByteString, sqlglot_expressions.Parameter))
 
     def is_calculate(self, expression, config, arguments):
         return isinstance(expression, (sqlglot_expressions.Neg, sqlglot_expressions.Anonymous, sqlglot_expressions.Binary, sqlglot_expressions.Func,
-                                       sqlglot_expressions.Select, sqlglot_expressions.Subquery, sqlglot_expressions.Union, sqlglot_expressions.Not,
-                                       sqlglot_expressions.BitwiseNot, sqlglot_expressions.Tuple))
+                                       sqlglot_expressions.Select, sqlglot_expressions.Subquery, sqlglot_expressions.Union, sqlglot_expressions.Between,
+                                       sqlglot_expressions.Not, sqlglot_expressions.BitwiseNot, sqlglot_expressions.Tuple))
 
     def is_aggregate(self, expression, config, arguments):
         if isinstance(expression, (sqlglot_expressions.Count, sqlglot_expressions.Sum, sqlglot_expressions.Max,
                                        sqlglot_expressions.Min, sqlglot_expressions.Avg)):
             return True
         if isinstance(expression, sqlglot_expressions.Anonymous):
             calculater_name = expression.args["this"].lower()
```

### Comparing `syncanysql-0.1.2/syncanysql/config.py` & `syncanysql-0.1.3/syncanysql/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
             if filename not in self.config["extends"]:
                 self.config["extends"].append(filename)
         self.load_config()
         if custom_config and isinstance(custom_config, dict):
             self.merge_config(custom_config)
 
         if "timezone" in self.config:
-            timezone = self.config.pop("timezone")
+            timezone = self.config.get("timezone")
             set_timezone(pytz.timezone(timezone))
         if "databases" not in self.config:
             self.config["databases"] = []
         databases = {database["name"]: database for database in self.config["databases"]}
         if "-" not in databases:
             self.config["databases"].append({"name": "-", "driver": "textline"})
         if "--" not in databases:
@@ -152,18 +152,18 @@
         elif databases["--"]["driver"] == "redis":
             redis_default_config = {"prefix": "syncany:" + str(uuid.uuid1().int) + ":", "serialize": "pickle",
                                     "ignore_serialize_error": True, "expire_seconds": 900}
             for key, value in redis_default_config.items():
                 if key not in databases["--"]:
                     databases["--"][key] = value
 
-        encoding = self.config.pop("encoding", None)
-        datetime_format = self.config.pop("datetime_format", None)
-        date_format = self.config.pop("date_format", None)
-        time_format = self.config.pop("time_format", None)
+        encoding = self.config.get("encoding", None)
+        datetime_format = self.config.get("datetime_format", None)
+        date_format = self.config.get("date_format", None)
+        time_format = self.config.get("time_format", None)
         for database in self.config["databases"]:
             if database["driver"] not in ("textline", "json", "csv"):
                 continue
             if encoding:
                 database["encoding"] = encoding
             if datetime_format:
                 database["datetime_format"] = datetime_format
@@ -238,19 +238,19 @@
                     self.config[k].extend(v if isinstance(v, list) else [v])
                 else:
                     self.config[k] = v if isinstance(v, list) else [v]
             else:
                 self.config[k] = v
 
     def config_logging(self, isatty=True):
-        logfile = self.config.pop("logfile", None)
+        logfile = self.config.get("logfile", None)
         if not logfile or logfile == "-":
             logfile = None
-        logformat = self.config.pop("logformat", "%(asctime)s %(process)d %(levelname)s %(message)s")
-        loglevel = self.config.pop("loglevel", None)
+        logformat = self.config.get("logformat", "%(asctime)s %(process)d %(levelname)s %(message)s")
+        loglevel = self.config.get("loglevel", None)
         if "logger" in self.config and isinstance(self.config["logger"], dict):
             logging.config.dictConfig(self.config["logger"])
         else:
             if not logfile and not loglevel and not isatty:
                 loglevel = logging.CRITICAL
             else:
                 loglevel = {"CRITICAL": logging.CRITICAL, "FATAL": logging.FATAL, "ERROR": logging.ERROR,
```

### Comparing `syncanysql-0.1.2/syncanysql/executor.py` & `syncanysql-0.1.3/syncanysql/executor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # 2023/2/13
 # create by: snower
-
+import datetime
 import os
 import sys
 import re
 import threading
 from collections import deque
 from syncany.filters import StringFilter
 from syncany.calculaters import find_calculater
 from syncany.database import find_database
 from .errors import SyncanySqlCompileException
 from .utils import parse_value
 from .compiler import Compiler
 
-ENV_VARIABLE_RE = re.compile("(\$\{\w+?(:.*?){0,1}\})", re.DOTALL | re.M)
+ENV_VARIABLE_RE = re.compile("(\$\{[@\w]+?(:.*?){0,1}\})", re.DOTALL | re.M)
 RAW_SQL_RE = re.compile("(\/\*\s*raw\(([\w\.]+?)\)\s*(\*\/\s*\()?\s*(.*?)\s*(\)\s*\/\*)?\s*endraw\s*\*\/)", re.DOTALL | re.M)
 FUNC_RE = re.compile("^(\w+?)\(((.+),{0,1})*\)$", re.DOTALL)
 
 
 class EnvVariables(dict):
     def __init__(self, parent=None, *args, **kwargs):
         super(EnvVariables, self).__init__(*args, **kwargs)
@@ -90,23 +90,37 @@
             except KeyError:
                 try:
                     groups = FUNC_RE.match(default_value[1:].strip()).groups()
                     calculater_args = []
                     if groups[1]:
                         for arg in groups[1].split(","):
                             calculater_args.append(parse_value(arg))
-                    calculater = find_calculater(groups[0].split("__")[0])(groups[0].replace("__", "::"))
+                    calculater = find_calculater(groups[0].split("__")[0]).instance(groups[0].replace("__", "::"))
                     variable_value = calculater.calculate(*tuple(calculater_args))
                     variable_value = StringFilter().filter(variable_value)
                 except Exception as e:
                     variable_value = default_value[1:]
-            if isinstance(variable_value, str):
-                variable_value = "true" if variable_value is True else ("false" if variable_value is False else
-                                                                        ("null" if variable_value is None else str(variable_value)))
-            sql = sql.replace(variable, variable_value)
+
+            def format_variable_value(value):
+                if value is True:
+                    return "true"
+                if value is False:
+                    return "false"
+                if value is None:
+                    return "null"
+                if isinstance(value, datetime.date):
+                    if isinstance(value, datetime.datetime):
+                        return value.strftime(self.session_config.get().get("datetime_format", "%Y-%m-%d %H:%M:%S"))
+                    return value.strftime(self.session_config.get().get("date_format", "%Y-%m-%d"))
+                if isinstance(value, datetime.time):
+                    return value.strftime(self.session_config.get().get("time_format", "%H:%M:%S"))
+                if isinstance(value, (list, tuple, set)):
+                    return "(" + ",".join([format_variable_value(v) for v in value]) + ")"
+                return str(value)
+            sql = sql.replace(variable, format_variable_value(variable_value))
         return sql
 
     def run(self, name, sqls):
         for sql in sqls:
             lineno = sql.lineno
             sql = self.compile_variable(str(sql))
             raw_sqls = RAW_SQL_RE.findall(sql)
```

### Comparing `syncanysql-0.1.2/syncanysql/main.py` & `syncanysql-0.1.3/syncanysql/main.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.2/syncanysql/parser.py` & `syncanysql-0.1.3/syncanysql/parser.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.2/syncanysql/prompt.py` & `syncanysql-0.1.3/syncanysql/prompt.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.2/syncanysql/taskers/delete.py` & `syncanysql-0.1.3/syncanysql/taskers/delete.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.2/syncanysql/taskers/execute.py` & `syncanysql-0.1.3/syncanysql/taskers/execute.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.2/syncanysql/taskers/explain.py` & `syncanysql-0.1.3/syncanysql/taskers/explain.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.2/syncanysql/taskers/into.py` & `syncanysql-0.1.3/syncanysql/taskers/into.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.2/syncanysql/taskers/query.py` & `syncanysql-0.1.3/syncanysql/taskers/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,15 +310,15 @@
                 for key in where_schema:
                     config.pop(key, None)
             for key, column in config["schema"].items():
                 if key in aggregate["schema"] and aggregate["schema"][key]["final_value"]:
                     config["schema"][key] = aggregate["schema"][key]["final_value"]
                 else:
                     config["schema"][key] = "$." + key
-            config["name"] = config["name"] + "#select@final_reduce"
+            config["name"] = config["name"] + "#select@final"
         else:
             config["output"] = config["input"] + " use DI"
             config["name"] = config["name"] + "#select@reduce"
             config["intercepts"] = []
             config["pipelines"] = []
         if "intercepts" in config:
             config["intercepts"] = [intercept for intercept in config["intercepts"] if
```

### Comparing `syncanysql-0.1.2/syncanysql/taskers/set.py` & `syncanysql-0.1.3/syncanysql/taskers/set.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,17 +52,20 @@
             return value[1:-1].strip()
         if value.lower() == 'true':
             return True
         if value.lower() == 'false':
             return False
         if value.lower() == 'null':
             return None
-        digits = value.split(".")
-        if digits and len(digits) <= 2 and digits[0].isdigit():
-            return float(value) if len(digits) == 2 and digits[1].isdigit() else int(value)
+        if value.isdigit() or (value[0] == "-" and value[1:].isdigit()):
+            return int(value)
+        value_info = value.split(".")
+        if len(value_info) == 2 and (value_info[0].isdigit() or (value[0][0] == "-" and value[0][1:].isdigit())) \
+                and value_info[1].isdigit():
+            return float(value)
         raise ValueError("unknown value: %s" % value)
 
     def run(self, executor, session_config, manager):
         return 0
 
     def terminate(self):
         pass
```

### Comparing `syncanysql-0.1.2/syncanysql/taskers/show.py` & `syncanysql-0.1.3/syncanysql/taskers/show.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.2/syncanysql/taskers/use.py` & `syncanysql-0.1.3/syncanysql/taskers/use.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.2/syncanysql/utils.py` & `syncanysql-0.1.3/syncanysql/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 
 def parse_value(value):
     value = value.strip()
     if not value:
         return ""
     if len(value) >= 2 and value[0] in ("'", '"') and value[-1] in ("'", '"'):
         return value[1:-1]
-    if value.isdigit():
+    if value.isdigit() or (value[0] == "-" and value[1:].isdigit()):
         return int(value)
     if value.lower() == "true":
         return True
     if value.lower() == "false":
         return False
     if value.lower() == "null":
         return None
     value_info = value.split(".")
-    if len(value_info) == 2 and value_info[0].isdigit() and value_info[1].isdigit():
+    if len(value_info) == 2 and (value_info[0].isdigit() or (value[0][0] == "-" and value[0][1:].isdigit())) \
+            and value_info[1].isdigit():
         return float(value)
     return value
```

### Comparing `syncanysql-0.1.2/syncanysql.egg-info/PKG-INFO` & `syncanysql-0.1.3/syncanysql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanysql
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple and easy-to-use sql execution engine
 Home-page: https://github.com/snower/syncany-sql
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # Syncany-SQL
         [![Tests](https://img.shields.io/github/actions/workflow/status/snower/syncany-sql/ci.yml?label=tests)](https://github.com/snower/syncany-sql/actions/workflows/ci.yml)
```

### Comparing `syncanysql-0.1.2/syncanysql.egg-info/SOURCES.txt` & `syncanysql-0.1.3/syncanysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/volttron_lib_sql_historian-0.2.1rc0.tar.gz` & `tmp/volttron_lib_sql_historian-0.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_lib_sql_historian-0.2.1rc0.tar", max compression
+gzip compressed data, was "volttron_lib_sql_historian-0.2.1rc1.tar", max compression
```

## Comparing `volttron_lib_sql_historian-0.2.1rc0.tar` & `volttron_lib_sql_historian-0.2.1rc1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11928 2023-05-12 18:22:47.260723 volttron_lib_sql_historian-0.2.1rc0/LICENSE
--rw-r--r--   0        0        0     3179 2023-05-12 18:23:53.096791 volttron_lib_sql_historian-0.2.1rc0/README.md
--rw-r--r--   0        0        0     1140 2023-05-12 18:23:54.636887 volttron_lib_sql_historian-0.2.1rc0/pyproject.toml
--rw-r--r--   0        0        0     1134 2023-05-12 18:22:47.260723 volttron_lib_sql_historian-0.2.1rc0/src/historian/sql/__init__.py
--rw-r--r--   0        0        0    20476 2023-05-12 18:22:47.260723 volttron_lib_sql_historian-0.2.1rc0/src/historian/sql/basedb.py
--rw-r--r--   0        0        0    15683 2023-05-12 18:22:47.260723 volttron_lib_sql_historian-0.2.1rc0/src/historian/sql/historian.py
--rw-r--r--   0        0        0     1672 2023-05-12 18:22:47.260723 volttron_lib_sql_historian-0.2.1rc0/src/historian/sql/sqlutils.py
--rw-r--r--   0        0        0     3891 1970-01-01 00:00:00.000000 volttron_lib_sql_historian-0.2.1rc0/PKG-INFO
+-rw-r--r--   0        0        0    11928 2023-05-12 18:24:19.808612 volttron_lib_sql_historian-0.2.1rc1/LICENSE
+-rw-r--r--   0        0        0     3179 2023-05-12 18:24:19.808612 volttron_lib_sql_historian-0.2.1rc1/README.md
+-rw-r--r--   0        0        0     1140 2023-05-12 18:25:15.304620 volttron_lib_sql_historian-0.2.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     1134 2023-05-12 18:24:19.808612 volttron_lib_sql_historian-0.2.1rc1/src/historian/sql/__init__.py
+-rw-r--r--   0        0        0    20476 2023-05-12 18:24:19.812612 volttron_lib_sql_historian-0.2.1rc1/src/historian/sql/basedb.py
+-rw-r--r--   0        0        0    15683 2023-05-12 18:24:19.812612 volttron_lib_sql_historian-0.2.1rc1/src/historian/sql/historian.py
+-rw-r--r--   0        0        0     1672 2023-05-12 18:24:19.812612 volttron_lib_sql_historian-0.2.1rc1/src/historian/sql/sqlutils.py
+-rw-r--r--   0        0        0     3891 1970-01-01 00:00:00.000000 volttron_lib_sql_historian-0.2.1rc1/PKG-INFO
```

### Comparing `volttron_lib_sql_historian-0.2.1rc0/LICENSE` & `volttron_lib_sql_historian-0.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_lib_sql_historian-0.2.1rc0/README.md` & `volttron_lib_sql_historian-0.2.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `volttron_lib_sql_historian-0.2.1rc0/pyproject.toml` & `volttron_lib_sql_historian-0.2.1rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "volttron-lib-sql-historian"
-version = "0.2.1rc0"
+version = "0.2.1rc1"
 description = "A library for supporting sql based historians."
 authors = ["VOLTTRON Team <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/eclipse-volttron/volttron-lib-sql-historian"
 homepage = "https://github.com/eclipse-volttron/volttron-lib-sql-historian"
 keywords = []
```

### Comparing `volttron_lib_sql_historian-0.2.1rc0/src/historian/sql/__init__.py` & `volttron_lib_sql_historian-0.2.1rc1/src/historian/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_sql_historian-0.2.1rc0/src/historian/sql/basedb.py` & `volttron_lib_sql_historian-0.2.1rc1/src/historian/sql/basedb.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_sql_historian-0.2.1rc0/src/historian/sql/historian.py` & `volttron_lib_sql_historian-0.2.1rc1/src/historian/sql/historian.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_sql_historian-0.2.1rc0/src/historian/sql/sqlutils.py` & `volttron_lib_sql_historian-0.2.1rc1/src/historian/sql/sqlutils.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_sql_historian-0.2.1rc0/PKG-INFO` & `volttron_lib_sql_historian-0.2.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-lib-sql-historian
-Version: 0.2.1rc0
+Version: 0.2.1rc1
 Summary: A library for supporting sql based historians.
 Home-page: https://github.com/eclipse-volttron/volttron-lib-sql-historian
 License: Apache-2.0
 Author: VOLTTRON Team
 Author-email: volttron@pnnl.gov
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```


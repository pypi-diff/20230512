# Comparing `tmp/sqlalchemy_rqlite-1.1.1.tar.gz` & `tmp/sqlalchemy_rqlite-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_rqlite-1.1.1.tar", last modified: Tue Dec 21 17:25:57 2021, max compression
+gzip compressed data, was "sqlalchemy_rqlite-1.2.tar", last modified: Fri May 12 06:05:29 2023, max compression
```

## Comparing `sqlalchemy_rqlite-1.1.1.tar` & `sqlalchemy_rqlite-1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zmedico   (1000) zmedico   (1000)        0 2021-12-21 17:25:57.208084 sqlalchemy_rqlite-1.1.1/
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)     1077 2021-12-21 17:23:21.000000 sqlalchemy_rqlite-1.1.1/LICENSE
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)     1016 2021-12-21 17:25:57.208084 sqlalchemy_rqlite-1.1.1/PKG-INFO
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)      990 2021-12-21 17:23:21.000000 sqlalchemy_rqlite-1.1.1/README.rst
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)       95 2021-12-21 17:23:21.000000 sqlalchemy_rqlite-1.1.1/pyproject.toml
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)       38 2021-12-21 17:25:57.208084 sqlalchemy_rqlite-1.1.1/setup.cfg
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)     3677 2021-12-21 17:23:21.000000 sqlalchemy_rqlite-1.1.1/setup.py
-drwxr-xr-x   0 zmedico   (1000) zmedico   (1000)        0 2021-12-21 17:25:57.206084 sqlalchemy_rqlite-1.1.1/src/
-drwxr-xr-x   0 zmedico   (1000) zmedico   (1000)        0 2021-12-21 17:25:57.207084 sqlalchemy_rqlite-1.1.1/src/sqlalchemy_rqlite/
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)      447 2021-12-21 17:23:21.000000 sqlalchemy_rqlite-1.1.1/src/sqlalchemy_rqlite/__init__.py
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)      237 2021-12-21 17:25:38.000000 sqlalchemy_rqlite-1.1.1/src/sqlalchemy_rqlite/constants.py
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)     2524 2021-12-21 17:23:21.000000 sqlalchemy_rqlite-1.1.1/src/sqlalchemy_rqlite/pyrqlite.py
-drwxr-xr-x   0 zmedico   (1000) zmedico   (1000)        0 2021-12-21 17:25:57.208084 sqlalchemy_rqlite-1.1.1/src/sqlalchemy_rqlite.egg-info/
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)     1016 2021-12-21 17:25:57.000000 sqlalchemy_rqlite-1.1.1/src/sqlalchemy_rqlite.egg-info/PKG-INFO
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)      417 2021-12-21 17:25:57.000000 sqlalchemy_rqlite-1.1.1/src/sqlalchemy_rqlite.egg-info/SOURCES.txt
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)       65 2021-12-21 17:25:57.000000 sqlalchemy_rqlite-1.1.1/src/sqlalchemy_rqlite.egg-info/dependency_links.txt
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)       76 2021-12-21 17:25:57.000000 sqlalchemy_rqlite-1.1.1/src/sqlalchemy_rqlite.egg-info/entry_points.txt
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)       20 2021-12-21 17:25:57.000000 sqlalchemy_rqlite-1.1.1/src/sqlalchemy_rqlite.egg-info/requires.txt
--rw-r--r--   0 zmedico   (1000) zmedico   (1000)       18 2021-12-21 17:25:57.000000 sqlalchemy_rqlite-1.1.1/src/sqlalchemy_rqlite.egg-info/top_level.txt
+drwxr-xr-x   0 zmedico   (1000) zmedico   (1000)        0 2023-05-12 06:05:29.241138 sqlalchemy_rqlite-1.2/
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)     1077 2016-02-16 10:54:56.000000 sqlalchemy_rqlite-1.2/LICENSE
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)      985 2023-05-12 06:05:29.241138 sqlalchemy_rqlite-1.2/PKG-INFO
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)     1153 2023-05-12 06:02:33.000000 sqlalchemy_rqlite-1.2/README.rst
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)       95 2021-02-27 23:41:17.000000 sqlalchemy_rqlite-1.2/pyproject.toml
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)       38 2023-05-12 06:05:29.241138 sqlalchemy_rqlite-1.2/setup.cfg
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)     3677 2017-06-14 03:56:00.000000 sqlalchemy_rqlite-1.2/setup.py
+drwxr-xr-x   0 zmedico   (1000) zmedico   (1000)        0 2023-05-12 06:05:29.237138 sqlalchemy_rqlite-1.2/src/
+drwxr-xr-x   0 zmedico   (1000) zmedico   (1000)        0 2023-05-12 06:05:29.239138 sqlalchemy_rqlite-1.2/src/sqlalchemy_rqlite/
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)      447 2017-06-14 03:55:44.000000 sqlalchemy_rqlite-1.2/src/sqlalchemy_rqlite/__init__.py
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)      235 2023-05-12 06:04:24.000000 sqlalchemy_rqlite-1.2/src/sqlalchemy_rqlite/constants.py
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)     2863 2023-05-12 06:02:33.000000 sqlalchemy_rqlite-1.2/src/sqlalchemy_rqlite/pyrqlite.py
+drwxr-xr-x   0 zmedico   (1000) zmedico   (1000)        0 2023-05-12 06:05:29.240138 sqlalchemy_rqlite-1.2/src/sqlalchemy_rqlite.egg-info/
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)      985 2023-05-12 06:05:28.000000 sqlalchemy_rqlite-1.2/src/sqlalchemy_rqlite.egg-info/PKG-INFO
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)      417 2023-05-12 06:05:29.000000 sqlalchemy_rqlite-1.2/src/sqlalchemy_rqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)       65 2023-05-12 06:05:28.000000 sqlalchemy_rqlite-1.2/src/sqlalchemy_rqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)       75 2023-05-12 06:05:28.000000 sqlalchemy_rqlite-1.2/src/sqlalchemy_rqlite.egg-info/entry_points.txt
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)       20 2023-05-12 06:05:28.000000 sqlalchemy_rqlite-1.2/src/sqlalchemy_rqlite.egg-info/requires.txt
+-rw-r--r--   0 zmedico   (1000) zmedico   (1000)       18 2023-05-12 06:05:28.000000 sqlalchemy_rqlite-1.2/src/sqlalchemy_rqlite.egg-info/top_level.txt
```

### Comparing `sqlalchemy_rqlite-1.1.1/LICENSE` & `sqlalchemy_rqlite-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_rqlite-1.1.1/PKG-INFO` & `sqlalchemy_rqlite-1.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: sqlalchemy_rqlite
-Version: 1.1.1
+Version: 1.2
 Summary: SQLAlchemy dialect for rqlite
-Home-page: UNKNOWN
 Author: Zac Medico
 Author-email: zmedico@gmail.com
 Maintainer: Zac Medico
 Maintainer-email: zmedico@gmail.com
 License: MIT
 Keywords: rqlite SQLAlchemy
 Platform: Posix
@@ -21,10 +20,7 @@
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Database :: Front-Ends
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `sqlalchemy_rqlite-1.1.1/README.rst` & `sqlalchemy_rqlite-1.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 rqlite dialect for SQLAlchemy
 ==============================
+.. image:: https://circleci.com/gh/rqlite/sqlalchemy-rqlite/tree/master.svg?style=svg
+    :target: https://circleci.com/gh/rqlite/sqlalchemy-rqlite/?branch=master
 
 This is the rqlite dialect driver for SQLAlchemy.
 
 
 installation
 ------------
```

### Comparing `sqlalchemy_rqlite-1.1.1/setup.py` & `sqlalchemy_rqlite-1.2/setup.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_rqlite-1.1.1/src/sqlalchemy_rqlite/pyrqlite.py` & `sqlalchemy_rqlite-1.2/src/sqlalchemy_rqlite/pyrqlite.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         SQLiteDialect.colspecs,
         {
             sqltypes.Date: _SQLite_rqliteDate,
             sqltypes.TIMESTAMP: _SQLite_rqliteTimeStamp,
         }
     )
 
-    if not util.py2k:
+    if not getattr(util, "py2k", False):
         description_encoding = None
 
     driver = 'pyrqlite'
 
     # pylint: disable=method-hidden
     @classmethod
     def dbapi(cls):
@@ -85,9 +85,20 @@
         if url.password:
             opts['password'] = url.password
 
         return ([], opts)
 
     def is_disconnect(self, e, connection, cursor):
         return False
+    
+    def do_ping(self, dbapi_connection):
+        try:
+            dbapi_connection.ping(reconnect=True)
+        except self.dbapi.Error as err:
+            if self.is_disconnect(err, dbapi_connection, None):
+                return False
+            else:
+                raise
+        else:
+            return True
 
 dialect = SQLiteDialect_rqlite
```

### Comparing `sqlalchemy_rqlite-1.1.1/src/sqlalchemy_rqlite.egg-info/PKG-INFO` & `sqlalchemy_rqlite-1.2/src/sqlalchemy_rqlite.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-rqlite
-Version: 1.1.1
+Version: 1.2
 Summary: SQLAlchemy dialect for rqlite
-Home-page: UNKNOWN
 Author: Zac Medico
 Author-email: zmedico@gmail.com
 Maintainer: Zac Medico
 Maintainer-email: zmedico@gmail.com
 License: MIT
 Keywords: rqlite SQLAlchemy
 Platform: Posix
@@ -21,10 +20,7 @@
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Database :: Front-Ends
 License-File: LICENSE
-
-UNKNOWN
-
```


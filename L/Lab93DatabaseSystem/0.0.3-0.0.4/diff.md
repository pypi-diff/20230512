# Comparing `tmp/Lab93DatabaseSystem-0.0.3.tar.gz` & `tmp/Lab93DatabaseSystem-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lab93DatabaseSystem-0.0.3.tar", last modified: Wed May 10 00:38:37 2023, max compression
+gzip compressed data, was "Lab93DatabaseSystem-0.0.4.tar", last modified: Thu May 11 23:58:52 2023, max compression
```

## Comparing `Lab93DatabaseSystem-0.0.3.tar` & `Lab93DatabaseSystem-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-10 00:38:37.738439 Lab93DatabaseSystem-0.0.3/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      941 2023-05-10 00:38:37.738439 Lab93DatabaseSystem-0.0.3/PKG-INFO
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      652 2023-05-10 00:38:00.000000 Lab93DatabaseSystem-0.0.3/pyproject.toml
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      386 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.3/readme.md
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       38 2023-05-10 00:38:37.738439 Lab93DatabaseSystem-0.0.3/setup.cfg
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-10 00:38:37.718437 Lab93DatabaseSystem-0.0.3/src/
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-10 00:38:37.725104 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     5661 2023-05-10 00:02:51.000000 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem/__init__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-10 00:38:37.735105 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem/submodules/
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-10 00:38:37.738439 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem/submodules/DatabaseAPI/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     8087 2023-05-10 00:37:15.000000 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem/submodules/DatabaseAPI/SQLite3.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      928 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem/submodules/DatabaseAPI/Shelve.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem/submodules/DatabaseAPI/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem/submodules/__init__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-10 00:38:37.731772 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem.egg-info/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      941 2023-05-10 00:38:37.000000 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem.egg-info/PKG-INFO
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      469 2023-05-10 00:38:37.000000 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem.egg-info/SOURCES.txt
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        1 2023-05-10 00:38:37.000000 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem.egg-info/dependency_links.txt
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       20 2023-05-10 00:38:37.000000 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem.egg-info/top_level.txt
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-11 23:58:52.335261 Lab93DatabaseSystem-0.0.4/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      917 2023-05-11 23:58:52.331928 Lab93DatabaseSystem-0.0.4/PKG-INFO
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      628 2023-05-11 23:57:49.000000 Lab93DatabaseSystem-0.0.4/pyproject.toml
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      386 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.4/readme.md
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       38 2023-05-11 23:58:52.335261 Lab93DatabaseSystem-0.0.4/setup.cfg
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-11 23:58:52.305263 Lab93DatabaseSystem-0.0.4/src/
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-11 23:58:52.308596 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     5661 2023-05-10 00:02:51.000000 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem/__init__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-11 23:58:52.325262 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem/submodules/
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-11 23:58:52.331928 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem/submodules/DatabaseAPI/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     8703 2023-05-11 23:40:49.000000 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem/submodules/DatabaseAPI/SQLite3.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      928 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem/submodules/DatabaseAPI/Shelve.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem/submodules/DatabaseAPI/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem/submodules/__init__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-11 23:58:52.321929 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem.egg-info/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      917 2023-05-11 23:58:52.000000 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem.egg-info/PKG-INFO
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      469 2023-05-11 23:58:52.000000 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem.egg-info/SOURCES.txt
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        1 2023-05-11 23:58:52.000000 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem.egg-info/dependency_links.txt
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       20 2023-05-11 23:58:52.000000 Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem.egg-info/top_level.txt
```

### Comparing `Lab93DatabaseSystem-0.0.3/PKG-INFO` & `Lab93DatabaseSystem-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Lab93DatabaseSystem
-Version: 0.0.3
-Summary: An API for interfacing with SQLite3 databases from the command line.
+Version: 0.0.4
+Summary: An API for object persistence scriptability.
 Author-email: Hunter Dale <hunter@guyyatsu.me>
 Project-URL: Homepage, https://github.com/guyyatsu/Lab93-Database-System
 Project-URL: Bug Tracker, https://github.com/guyyatsu/Lab93-Database-System/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `Lab93DatabaseSystem-0.0.3/pyproject.toml` & `Lab93DatabaseSystem-0.0.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Lab93DatabaseSystem"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Hunter Dale", email="hunter@guyyatsu.me" },
 ]
 
-description = "An API for interfacing with SQLite3 databases from the command line."
+description = "An API for object persistence scriptability."
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem/__init__.py` & `Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem/submodules/DatabaseAPI/SQLite3.py` & `Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem/submodules/DatabaseAPI/SQLite3.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,15 +60,17 @@
     # Enumerate a list of tables within the master record.
     'queryTableList': "SELECT name FROM sqlite_schema WHERE type='table' ORDER BY name;",
 
     # Curate a list of headers for a given table.
     'queryHeaderList': "SELECT name FROM sqlite_master WHERE type='table'",
 
     # Add a new row to a specific table.
-    'createNewRow': "INSERT OR IGNORE INTO {}({}) VALUES({});",
+    'createNewUniqueRow': "INSERT OR IGNORE INTO {}({}) VALUES({});",
+
+    'querySelectRow': "SELECT * FROM {} WHERE {}='{}';"
 }
 
 
 def newColumn( database,
                table: str="test_table_one",
                column: str="test_column_one",
                column_type: str="UNIQUE PRIMARY TEXT" ) -> None:
@@ -202,24 +204,38 @@
     database = databaseConnection(database)
     return database.cursor\
                    .execute( statements['queryColumnExistence']\
                                  .format( table.lower(),
                                           column.lower() )            )\
                    .fetchall()[0][0]
 
+# NOTE: New function for version 0.0.4
+# TODO: This should actually be a querySpecificRow.
+def selectRow( database,
+              table,
+              row,
+              value ):
+    database = databaseConnection(database)
+    return database.cursor\
+                   .execute( statements['querySelectRow']\
+                                 .format( table.lower(),
+                                          row.lower(),
+                                          value         )     )\
+                   .fetchall()
+
 
-def newRow( database,
-            table: str="test_table_one",
-            columns: str="test_column_one, test_column_two",
-            values: str="test_value_one, test_value_two" ):
+def new_uniqueRow( database,
+                   table: str="test_table_one",
+                   columns: str="test_column_one, test_column_two",
+                   values: str="test_value_one, test_value_two" ):
     """
     """
 
     database = databaseConnection(database)
     database.cursor\
-            .execute( statements['createNewRow']\
+            .execute( statements['createNewUniqueRow']\
                           .format( table.lower(),
                                    columns.lower(),
                                    values.lower() )  )
 
     return database.connection\
                    .commit()
```

### Comparing `Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem/submodules/DatabaseAPI/Shelve.py` & `Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem/submodules/DatabaseAPI/Shelve.py`

 * *Files identical despite different names*

### Comparing `Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem.egg-info/PKG-INFO` & `Lab93DatabaseSystem-0.0.4/src/Lab93DatabaseSystem.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Lab93DatabaseSystem
-Version: 0.0.3
-Summary: An API for interfacing with SQLite3 databases from the command line.
+Version: 0.0.4
+Summary: An API for object persistence scriptability.
 Author-email: Hunter Dale <hunter@guyyatsu.me>
 Project-URL: Homepage, https://github.com/guyyatsu/Lab93-Database-System
 Project-URL: Bug Tracker, https://github.com/guyyatsu/Lab93-Database-System/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```


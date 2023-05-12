# Comparing `tmp/yw_etl_tap_sqlalchemy-0.1.3.tar.gz` & `tmp/yw_etl_tap_sqlalchemy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yw_etl_tap_sqlalchemy-0.1.3.tar", last modified: Fri May 12 02:58:30 2023, max compression
+gzip compressed data, was "yw_etl_tap_sqlalchemy-0.1.4.tar", last modified: Fri May 12 03:13:38 2023, max compression
```

## Comparing `yw_etl_tap_sqlalchemy-0.1.3.tar` & `yw_etl_tap_sqlalchemy-0.1.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 zhuxichi   (501) staff       (20)        0 2023-05-12 02:58:30.023455 yw_etl_tap_sqlalchemy-0.1.3/
--rw-r--r--   0 zhuxichi   (501) staff       (20)       32 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.3/MANIFEST.in
--rw-r--r--   0 zhuxichi   (501) staff       (20)       89 2023-05-12 02:58:30.022485 yw_etl_tap_sqlalchemy-0.1.3/PKG-INFO
--rw-r--r--   0 zhuxichi   (501) staff       (20)     6088 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.3/README.md
--rw-r--r--   0 zhuxichi   (501) staff       (20)      437 2023-05-12 02:57:58.000000 yw_etl_tap_sqlalchemy-0.1.3/pyproject.toml
--rw-r--r--   0 zhuxichi   (501) staff       (20)      109 2023-05-11 13:56:19.000000 yw_etl_tap_sqlalchemy-0.1.3/requirements.txt
--rw-r--r--   0 zhuxichi   (501) staff       (20)       38 2023-05-12 02:58:30.023631 yw_etl_tap_sqlalchemy-0.1.3/setup.cfg
-drwxr-xr-x   0 zhuxichi   (501) staff       (20)        0 2023-05-12 02:58:30.004305 yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy/
--rw-r--r--   0 zhuxichi   (501) staff       (20)     2070 2023-05-12 02:57:09.000000 yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy/Database.py
--rw-r--r--   0 zhuxichi   (501) staff       (20)     2070 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy/WorkingDirectory.py
--rw-r--r--   0 zhuxichi   (501) staff       (20)     1279 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy/WorkingDirectory_test.py
--rw-r--r--   0 zhuxichi   (501) staff       (20)        0 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy/__init__.py
--rw-r--r--   0 zhuxichi   (501) staff       (20)      343 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy/logging.conf
--rw-r--r--   0 zhuxichi   (501) staff       (20)     1514 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy/main.py
-drwxr-xr-x   0 zhuxichi   (501) staff       (20)        0 2023-05-12 02:58:30.019336 yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy/tapstream/
--rw-r--r--   0 zhuxichi   (501) staff       (20)     1149 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy/tapstream/CustomQueryTapStream.py
--rw-r--r--   0 zhuxichi   (501) staff       (20)     3203 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy/tapstream/CustomQueryTapStream_test.py
--rw-r--r--   0 zhuxichi   (501) staff       (20)      719 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy/tapstream/TapStream.py
--rw-r--r--   0 zhuxichi   (501) staff       (20)      906 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy/tapstream/__init__.py
--rw-r--r--   0 zhuxichi   (501) staff       (20)      195 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy/tapstream/helpers.py
--rw-r--r--   0 zhuxichi   (501) staff       (20)      499 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy/utils.py
-drwxr-xr-x   0 zhuxichi   (501) staff       (20)        0 2023-05-12 02:58:30.011114 yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy.egg-info/
--rw-r--r--   0 zhuxichi   (501) staff       (20)       89 2023-05-12 02:58:29.000000 yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 zhuxichi   (501) staff       (20)      827 2023-05-12 02:58:29.000000 yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 zhuxichi   (501) staff       (20)        1 2023-05-12 02:58:29.000000 yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 zhuxichi   (501) staff       (20)       67 2023-05-12 02:58:29.000000 yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy.egg-info/entry_points.txt
--rw-r--r--   0 zhuxichi   (501) staff       (20)      110 2023-05-12 02:58:29.000000 yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 zhuxichi   (501) staff       (20)       22 2023-05-12 02:58:29.000000 yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy.egg-info/top_level.txt
+drwxr-xr-x   0 zhuxichi   (501) staff       (20)        0 2023-05-12 03:13:38.421930 yw_etl_tap_sqlalchemy-0.1.4/
+-rw-r--r--   0 zhuxichi   (501) staff       (20)       32 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.4/MANIFEST.in
+-rw-r--r--   0 zhuxichi   (501) staff       (20)       89 2023-05-12 03:13:38.420168 yw_etl_tap_sqlalchemy-0.1.4/PKG-INFO
+-rw-r--r--   0 zhuxichi   (501) staff       (20)     6088 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.4/README.md
+-rw-r--r--   0 zhuxichi   (501) staff       (20)      437 2023-05-12 03:13:21.000000 yw_etl_tap_sqlalchemy-0.1.4/pyproject.toml
+-rw-r--r--   0 zhuxichi   (501) staff       (20)      109 2023-05-11 13:56:19.000000 yw_etl_tap_sqlalchemy-0.1.4/requirements.txt
+-rw-r--r--   0 zhuxichi   (501) staff       (20)       38 2023-05-12 03:13:38.422165 yw_etl_tap_sqlalchemy-0.1.4/setup.cfg
+drwxr-xr-x   0 zhuxichi   (501) staff       (20)        0 2023-05-12 03:13:38.409429 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/
+-rw-r--r--   0 zhuxichi   (501) staff       (20)     2070 2023-05-12 03:11:40.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/Database.py
+-rw-r--r--   0 zhuxichi   (501) staff       (20)     2070 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/WorkingDirectory.py
+-rw-r--r--   0 zhuxichi   (501) staff       (20)     1279 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/WorkingDirectory_test.py
+-rw-r--r--   0 zhuxichi   (501) staff       (20)        0 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/__init__.py
+-rw-r--r--   0 zhuxichi   (501) staff       (20)      343 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/logging.conf
+-rw-r--r--   0 zhuxichi   (501) staff       (20)     1514 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/main.py
+drwxr-xr-x   0 zhuxichi   (501) staff       (20)        0 2023-05-12 03:13:38.418097 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/tapstream/
+-rw-r--r--   0 zhuxichi   (501) staff       (20)     1183 2023-05-12 03:12:54.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/tapstream/CustomQueryTapStream.py
+-rw-r--r--   0 zhuxichi   (501) staff       (20)     3203 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/tapstream/CustomQueryTapStream_test.py
+-rw-r--r--   0 zhuxichi   (501) staff       (20)      719 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/tapstream/TapStream.py
+-rw-r--r--   0 zhuxichi   (501) staff       (20)      906 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/tapstream/__init__.py
+-rw-r--r--   0 zhuxichi   (501) staff       (20)      195 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/tapstream/helpers.py
+-rw-r--r--   0 zhuxichi   (501) staff       (20)      499 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/utils.py
+drwxr-xr-x   0 zhuxichi   (501) staff       (20)        0 2023-05-12 03:13:38.414191 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy.egg-info/
+-rw-r--r--   0 zhuxichi   (501) staff       (20)       89 2023-05-12 03:13:38.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 zhuxichi   (501) staff       (20)      827 2023-05-12 03:13:38.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 zhuxichi   (501) staff       (20)        1 2023-05-12 03:13:38.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 zhuxichi   (501) staff       (20)       67 2023-05-12 03:13:38.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy.egg-info/entry_points.txt
+-rw-r--r--   0 zhuxichi   (501) staff       (20)      110 2023-05-12 03:13:38.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 zhuxichi   (501) staff       (20)       22 2023-05-12 03:13:38.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy.egg-info/top_level.txt
```

### Comparing `yw_etl_tap_sqlalchemy-0.1.3/README.md` & `yw_etl_tap_sqlalchemy-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy/Database.py` & `yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/Database.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,16 +48,16 @@
         self.conn_str = conn_str
         self._test_conn()
         self._conn_ctx = None
 
     def _test_conn(self):
         engine = _get_engine(self.conn_str)
         with engine.connect() as con:
-            sql = "select 1" if "oracle" not in self.conn_str else text("select 1 from DUAL")
-            con.execute(sql).all()
+            sql = "select 1" if "oracle" not in self.conn_str else "select 1 from DUAL"
+            con.execute(text(sql)).all()
 
         self.engine = engine
 
     def __enter__(self):
         self._conn_ctx = self.engine.connect()
         return self._conn_ctx.__enter__()
```

### Comparing `yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy/WorkingDirectory.py` & `yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/WorkingDirectory.py`

 * *Files identical despite different names*

### Comparing `yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy/WorkingDirectory_test.py` & `yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/WorkingDirectory_test.py`

 * *Files identical despite different names*

### Comparing `yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy/main.py` & `yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/main.py`

 * *Files identical despite different names*

### Comparing `yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy/tapstream/CustomQueryTapStream.py` & `yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/tapstream/CustomQueryTapStream.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from pathlib import Path
 
 import singer
 from singer import CatalogEntry
 
+from sqlalchemy import text
 from yw_etl_tap_sqlalchemy.Database import Database
 from yw_etl_tap_sqlalchemy.tapstream.TapStream import TapStream
 
 
 class CustomQueryTapStream(TapStream):
     def __init__(self, catalog_entry: CatalogEntry, config, state, db: Database, sql_dir: Path):
         super().__init__(catalog_entry, config, state)
@@ -21,11 +22,11 @@
             self._query = query_file_path.read_text()
         else:
             self._query = (sql_dir / query_file_path).read_text(encoding='utf8')
 
     def sync(self):
         singer.write_schema(self.catalog_entry.stream, self.catalog_entry.schema.to_dict(), [])
         with self.db as conn:
-            cur = conn.execute(self._query)
+            cur = conn.execute(text(self._query))
             for row in cur:
                 record = {k: row[k] for k in row.keys()}
                 singer.write_record(self.stream_name, record)
```

### Comparing `yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy/tapstream/CustomQueryTapStream_test.py` & `yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/tapstream/CustomQueryTapStream_test.py`

 * *Files identical despite different names*

### Comparing `yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy/tapstream/TapStream.py` & `yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/tapstream/TapStream.py`

 * *Files identical despite different names*

### Comparing `yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy/tapstream/__init__.py` & `yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/tapstream/__init__.py`

 * *Files identical despite different names*

### Comparing `yw_etl_tap_sqlalchemy-0.1.3/yw_etl_tap_sqlalchemy.egg-info/SOURCES.txt` & `yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy.egg-info/SOURCES.txt`

 * *Files identical despite different names*


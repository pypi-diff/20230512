# Comparing `tmp/yw_etl_tap_sqlalchemy-0.1.4.tar.gz` & `tmp/yw_etl_tap_sqlalchemy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yw_etl_tap_sqlalchemy-0.1.4.tar", last modified: Fri May 12 03:13:38 2023, max compression
+gzip compressed data, was "yw_etl_tap_sqlalchemy-0.1.5.tar", last modified: Fri May 12 03:35:17 2023, max compression
```

## Comparing `yw_etl_tap_sqlalchemy-0.1.4.tar` & `yw_etl_tap_sqlalchemy-0.1.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 zhuxichi   (501) staff       (20)        0 2023-05-12 03:13:38.421930 yw_etl_tap_sqlalchemy-0.1.4/
--rw-r--r--   0 zhuxichi   (501) staff       (20)       32 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.4/MANIFEST.in
--rw-r--r--   0 zhuxichi   (501) staff       (20)       89 2023-05-12 03:13:38.420168 yw_etl_tap_sqlalchemy-0.1.4/PKG-INFO
--rw-r--r--   0 zhuxichi   (501) staff       (20)     6088 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.4/README.md
--rw-r--r--   0 zhuxichi   (501) staff       (20)      437 2023-05-12 03:13:21.000000 yw_etl_tap_sqlalchemy-0.1.4/pyproject.toml
--rw-r--r--   0 zhuxichi   (501) staff       (20)      109 2023-05-11 13:56:19.000000 yw_etl_tap_sqlalchemy-0.1.4/requirements.txt
--rw-r--r--   0 zhuxichi   (501) staff       (20)       38 2023-05-12 03:13:38.422165 yw_etl_tap_sqlalchemy-0.1.4/setup.cfg
-drwxr-xr-x   0 zhuxichi   (501) staff       (20)        0 2023-05-12 03:13:38.409429 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/
--rw-r--r--   0 zhuxichi   (501) staff       (20)     2070 2023-05-12 03:11:40.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/Database.py
--rw-r--r--   0 zhuxichi   (501) staff       (20)     2070 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/WorkingDirectory.py
--rw-r--r--   0 zhuxichi   (501) staff       (20)     1279 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/WorkingDirectory_test.py
--rw-r--r--   0 zhuxichi   (501) staff       (20)        0 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/__init__.py
--rw-r--r--   0 zhuxichi   (501) staff       (20)      343 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/logging.conf
--rw-r--r--   0 zhuxichi   (501) staff       (20)     1514 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/main.py
-drwxr-xr-x   0 zhuxichi   (501) staff       (20)        0 2023-05-12 03:13:38.418097 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/tapstream/
--rw-r--r--   0 zhuxichi   (501) staff       (20)     1183 2023-05-12 03:12:54.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/tapstream/CustomQueryTapStream.py
--rw-r--r--   0 zhuxichi   (501) staff       (20)     3203 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/tapstream/CustomQueryTapStream_test.py
--rw-r--r--   0 zhuxichi   (501) staff       (20)      719 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/tapstream/TapStream.py
--rw-r--r--   0 zhuxichi   (501) staff       (20)      906 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/tapstream/__init__.py
--rw-r--r--   0 zhuxichi   (501) staff       (20)      195 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/tapstream/helpers.py
--rw-r--r--   0 zhuxichi   (501) staff       (20)      499 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/utils.py
-drwxr-xr-x   0 zhuxichi   (501) staff       (20)        0 2023-05-12 03:13:38.414191 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy.egg-info/
--rw-r--r--   0 zhuxichi   (501) staff       (20)       89 2023-05-12 03:13:38.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 zhuxichi   (501) staff       (20)      827 2023-05-12 03:13:38.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 zhuxichi   (501) staff       (20)        1 2023-05-12 03:13:38.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 zhuxichi   (501) staff       (20)       67 2023-05-12 03:13:38.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy.egg-info/entry_points.txt
--rw-r--r--   0 zhuxichi   (501) staff       (20)      110 2023-05-12 03:13:38.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 zhuxichi   (501) staff       (20)       22 2023-05-12 03:13:38.000000 yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy.egg-info/top_level.txt
+drwxr-xr-x   0 zhuxichi   (501) staff       (20)        0 2023-05-12 03:35:17.228134 yw_etl_tap_sqlalchemy-0.1.5/
+-rw-r--r--   0 zhuxichi   (501) staff       (20)       32 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.5/MANIFEST.in
+-rw-r--r--   0 zhuxichi   (501) staff       (20)       89 2023-05-12 03:35:17.227285 yw_etl_tap_sqlalchemy-0.1.5/PKG-INFO
+-rw-r--r--   0 zhuxichi   (501) staff       (20)     6088 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.5/README.md
+-rw-r--r--   0 zhuxichi   (501) staff       (20)      437 2023-05-12 03:34:32.000000 yw_etl_tap_sqlalchemy-0.1.5/pyproject.toml
+-rw-r--r--   0 zhuxichi   (501) staff       (20)      109 2023-05-11 13:56:19.000000 yw_etl_tap_sqlalchemy-0.1.5/requirements.txt
+-rw-r--r--   0 zhuxichi   (501) staff       (20)       38 2023-05-12 03:35:17.228378 yw_etl_tap_sqlalchemy-0.1.5/setup.cfg
+drwxr-xr-x   0 zhuxichi   (501) staff       (20)        0 2023-05-12 03:35:17.211926 yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy/
+-rw-r--r--   0 zhuxichi   (501) staff       (20)     2075 2023-05-12 03:34:24.000000 yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy/Database.py
+-rw-r--r--   0 zhuxichi   (501) staff       (20)     2070 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy/WorkingDirectory.py
+-rw-r--r--   0 zhuxichi   (501) staff       (20)     1279 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy/WorkingDirectory_test.py
+-rw-r--r--   0 zhuxichi   (501) staff       (20)        0 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy/__init__.py
+-rw-r--r--   0 zhuxichi   (501) staff       (20)      343 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy/logging.conf
+-rw-r--r--   0 zhuxichi   (501) staff       (20)     1514 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy/main.py
+drwxr-xr-x   0 zhuxichi   (501) staff       (20)        0 2023-05-12 03:35:17.225691 yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy/tapstream/
+-rw-r--r--   0 zhuxichi   (501) staff       (20)     1194 2023-05-12 03:34:14.000000 yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy/tapstream/CustomQueryTapStream.py
+-rw-r--r--   0 zhuxichi   (501) staff       (20)     3203 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy/tapstream/CustomQueryTapStream_test.py
+-rw-r--r--   0 zhuxichi   (501) staff       (20)      719 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy/tapstream/TapStream.py
+-rw-r--r--   0 zhuxichi   (501) staff       (20)      906 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy/tapstream/__init__.py
+-rw-r--r--   0 zhuxichi   (501) staff       (20)      195 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy/tapstream/helpers.py
+-rw-r--r--   0 zhuxichi   (501) staff       (20)      499 2023-05-11 10:32:47.000000 yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy/utils.py
+drwxr-xr-x   0 zhuxichi   (501) staff       (20)        0 2023-05-12 03:35:17.217769 yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy.egg-info/
+-rw-r--r--   0 zhuxichi   (501) staff       (20)       89 2023-05-12 03:35:17.000000 yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 zhuxichi   (501) staff       (20)      827 2023-05-12 03:35:17.000000 yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 zhuxichi   (501) staff       (20)        1 2023-05-12 03:35:17.000000 yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 zhuxichi   (501) staff       (20)       67 2023-05-12 03:35:17.000000 yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy.egg-info/entry_points.txt
+-rw-r--r--   0 zhuxichi   (501) staff       (20)      110 2023-05-12 03:35:17.000000 yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 zhuxichi   (501) staff       (20)       22 2023-05-12 03:35:17.000000 yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy.egg-info/top_level.txt
```

### Comparing `yw_etl_tap_sqlalchemy-0.1.4/README.md` & `yw_etl_tap_sqlalchemy-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/Database.py` & `yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy/Database.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         self.conn_str = conn_str
         self._test_conn()
         self._conn_ctx = None
 
     def _test_conn(self):
         engine = _get_engine(self.conn_str)
         with engine.connect() as con:
-            sql = "select 1" if "oracle" not in self.conn_str else "select 1 from DUAL"
+            sql = "select 1" if "oracle" not in self.conn_str else "select 1 AS a from DUAL"
             con.execute(text(sql)).all()
 
         self.engine = engine
 
     def __enter__(self):
         self._conn_ctx = self.engine.connect()
         return self._conn_ctx.__enter__()
```

### Comparing `yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/WorkingDirectory.py` & `yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy/WorkingDirectory.py`

 * *Files identical despite different names*

### Comparing `yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/WorkingDirectory_test.py` & `yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy/WorkingDirectory_test.py`

 * *Files identical despite different names*

### Comparing `yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/main.py` & `yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy/main.py`

 * *Files identical despite different names*

### Comparing `yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/tapstream/CustomQueryTapStream.py` & `yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy/tapstream/CustomQueryTapStream.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,10 +23,10 @@
         else:
             self._query = (sql_dir / query_file_path).read_text(encoding='utf8')
 
     def sync(self):
         singer.write_schema(self.catalog_entry.stream, self.catalog_entry.schema.to_dict(), [])
         with self.db as conn:
             cur = conn.execute(text(self._query))
-            for row in cur:
+            for row in cur.mappings():
                 record = {k: row[k] for k in row.keys()}
                 singer.write_record(self.stream_name, record)
```

### Comparing `yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/tapstream/CustomQueryTapStream_test.py` & `yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy/tapstream/CustomQueryTapStream_test.py`

 * *Files identical despite different names*

### Comparing `yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/tapstream/TapStream.py` & `yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy/tapstream/TapStream.py`

 * *Files identical despite different names*

### Comparing `yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy/tapstream/__init__.py` & `yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy/tapstream/__init__.py`

 * *Files identical despite different names*

### Comparing `yw_etl_tap_sqlalchemy-0.1.4/yw_etl_tap_sqlalchemy.egg-info/SOURCES.txt` & `yw_etl_tap_sqlalchemy-0.1.5/yw_etl_tap_sqlalchemy.egg-info/SOURCES.txt`

 * *Files identical despite different names*


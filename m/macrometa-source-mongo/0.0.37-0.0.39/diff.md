# Comparing `tmp/macrometa-source-mongo-0.0.37.tar.gz` & `tmp/macrometa-source-mongo-0.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-mongo-0.0.37.tar", max compression
+gzip compressed data, was "macrometa-source-mongo-0.0.39.tar", max compression
```

## Comparing `macrometa-source-mongo-0.0.37.tar` & `macrometa-source-mongo-0.0.39.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    10765 2023-05-12 10:08:52.807187 macrometa-source-mongo-0.0.37/LICENSE
--rw-r--r--   0        0        0    20533 2023-05-12 10:08:52.807187 macrometa-source-mongo-0.0.37/macrometa_source_mongo/__init__.py
--rw-r--r--   0        0        0     6470 2023-05-12 10:08:52.807187 macrometa-source-mongo-0.0.37/macrometa_source_mongo/connection.py
--rw-r--r--   0        0        0      895 2023-05-12 10:08:52.807187 macrometa-source-mongo-0.0.37/macrometa_source_mongo/exceptions.py
--rw-r--r--   0        0        0     7252 2023-05-12 10:08:52.807187 macrometa-source-mongo-0.0.37/macrometa_source_mongo/helper.py
--rw-r--r--   0        0        0    10251 2023-05-12 10:08:52.807187 macrometa-source-mongo-0.0.37/macrometa_source_mongo/sync_strategies/common.py
--rw-r--r--   0        0        0     3647 2023-05-12 10:08:52.807187 macrometa-source-mongo-0.0.37/macrometa_source_mongo/sync_strategies/full_table.py
--rw-r--r--   0        0        0     7248 2023-05-12 10:08:52.807187 macrometa-source-mongo-0.0.37/macrometa_source_mongo/sync_strategies/log_based.py
--rw-r--r--   0        0        0     2292 2023-05-12 10:08:52.807187 macrometa-source-mongo-0.0.37/macrometa_source_mongo/sync_strategies/sample_data.py
--rw-r--r--   0        0        0     1548 2023-05-12 10:08:53.183191 macrometa-source-mongo-0.0.37/pyproject.toml
--rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.37/setup.py
--rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.37/PKG-INFO
+-rw-r--r--   0        0        0    10765 2023-05-12 12:47:36.526088 macrometa-source-mongo-0.0.39/LICENSE
+-rw-r--r--   0        0        0    20533 2023-05-12 12:47:36.526088 macrometa-source-mongo-0.0.39/macrometa_source_mongo/__init__.py
+-rw-r--r--   0        0        0     6470 2023-05-12 12:47:36.526088 macrometa-source-mongo-0.0.39/macrometa_source_mongo/connection.py
+-rw-r--r--   0        0        0      895 2023-05-12 12:47:36.526088 macrometa-source-mongo-0.0.39/macrometa_source_mongo/exceptions.py
+-rw-r--r--   0        0        0     7252 2023-05-12 12:47:36.526088 macrometa-source-mongo-0.0.39/macrometa_source_mongo/helper.py
+-rw-r--r--   0        0        0    10251 2023-05-12 12:47:36.526088 macrometa-source-mongo-0.0.39/macrometa_source_mongo/sync_strategies/common.py
+-rw-r--r--   0        0        0     3647 2023-05-12 12:47:36.526088 macrometa-source-mongo-0.0.39/macrometa_source_mongo/sync_strategies/full_table.py
+-rw-r--r--   0        0        0     7271 2023-05-12 12:47:36.526088 macrometa-source-mongo-0.0.39/macrometa_source_mongo/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     2292 2023-05-12 12:47:36.526088 macrometa-source-mongo-0.0.39/macrometa_source_mongo/sync_strategies/sample_data.py
+-rw-r--r--   0        0        0     1548 2023-05-12 12:47:36.766087 macrometa-source-mongo-0.0.39/pyproject.toml
+-rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.39/setup.py
+-rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.39/PKG-INFO
```

### Comparing `macrometa-source-mongo-0.0.37/LICENSE` & `macrometa-source-mongo-0.0.39/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.37/macrometa_source_mongo/__init__.py` & `macrometa-source-mongo-0.0.39/macrometa_source_mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.37/macrometa_source_mongo/connection.py` & `macrometa-source-mongo-0.0.39/macrometa_source_mongo/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.37/macrometa_source_mongo/exceptions.py` & `macrometa-source-mongo-0.0.39/macrometa_source_mongo/exceptions.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.37/macrometa_source_mongo/helper.py` & `macrometa-source-mongo-0.0.39/macrometa_source_mongo/helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.37/macrometa_source_mongo/sync_strategies/common.py` & `macrometa-source-mongo-0.0.39/macrometa_source_mongo/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.37/macrometa_source_mongo/sync_strategies/full_table.py` & `macrometa-source-mongo-0.0.39/macrometa_source_mongo/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.37/macrometa_source_mongo/sync_strategies/log_based.py` & `macrometa-source-mongo-0.0.39/macrometa_source_mongo/sync_strategies/log_based.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,7 +151,8 @@
                 LOGGER.error('Unhandled error type, exiting...')
                 raise e
         for stream_id in stream_ids:
             common.TIMES[stream_id] += time.time() - start_time
             if rows_saved[stream_id] - rows_saved_iter_start[stream_id] > 0:
                 common.COUNTS[stream_id] += (rows_saved[stream_id] - rows_saved_iter_start[stream_id])
                 LOGGER.info('The number of records synchronized till now for %s is %s.', stream_id, rows_saved[stream_id])
+        time.sleep(10)
```

### Comparing `macrometa-source-mongo-0.0.37/macrometa_source_mongo/sync_strategies/sample_data.py` & `macrometa-source-mongo-0.0.39/macrometa_source_mongo/sync_strategies/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.37/pyproject.toml` & `macrometa-source-mongo-0.0.39/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-mongo"
-version='0.0.37'
+version='0.0.39'
 description = "Macrometa Source for extracting data from MongoDB."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-mongo-0.0.37/setup.py` & `macrometa-source-mongo-0.0.39/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'tzlocal>=2.1.0,<2.2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-mongo = macrometa_source_mongo:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-mongo',
-    'version': '0.0.37',
+    'version': '0.0.39',
     'description': 'Macrometa Source for extracting data from MongoDB.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-mongo-0.0.37/PKG-INFO` & `macrometa-source-mongo-0.0.39/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-mongo
-Version: 0.0.37
+Version: 0.0.39
 Summary: Macrometa Source for extracting data from MongoDB.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,MongoDB,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```


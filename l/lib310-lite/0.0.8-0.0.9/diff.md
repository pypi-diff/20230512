# Comparing `tmp/lib310_lite-0.0.8.tar.gz` & `tmp/lib310_lite-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib310_lite-0.0.8.tar", max compression
+gzip compressed data, was "lib310_lite-0.0.9.tar", max compression
```

## Comparing `lib310_lite-0.0.8.tar` & `lib310_lite-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      249 2023-03-08 14:56:22.920616 lib310_lite-0.0.8/lib310_lite/__init__.py
--rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.0.8/lib310_lite/bigquery/_functions.py
--rw-r--r--   0        0        0     7467 2023-05-08 08:51:40.656605 lib310_lite-0.0.8/lib310_lite/bigquery/client.py
--rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.0.8/lib310_lite/bigquery/constants.py
--rw-r--r--   0        0        0       35 2023-03-07 10:52:53.179251 lib310_lite-0.0.8/lib310_lite/fucntion.py
--rw-r--r--   0        0        0    12058 2023-05-12 10:37:55.686425 lib310_lite-0.0.8/lib310_lite/mldl/mldl.py
--rw-r--r--   0        0        0     1528 2023-05-12 10:35:08.523571 lib310_lite-0.0.8/lib310_lite/mldl/models/InteractionModel.py
--rw-r--r--   0        0        0     2818 2023-05-12 10:35:08.531397 lib310_lite-0.0.8/lib310_lite/mldl/models/SeqLangModel.py
--rw-r--r--   0        0        0      799 2023-05-12 11:20:31.446520 lib310_lite-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      937 1970-01-01 00:00:00.000000 lib310_lite-0.0.8/setup.py
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 lib310_lite-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      249 2023-03-08 14:56:22.920616 lib310_lite-0.0.9/lib310_lite/__init__.py
+-rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.0.9/lib310_lite/bigquery/_functions.py
+-rw-r--r--   0        0        0     7479 2023-05-12 13:53:49.135436 lib310_lite-0.0.9/lib310_lite/bigquery/client.py
+-rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.0.9/lib310_lite/bigquery/constants.py
+-rw-r--r--   0        0        0       35 2023-03-07 10:52:53.179251 lib310_lite-0.0.9/lib310_lite/fucntion.py
+-rw-r--r--   0        0        0    12102 2023-05-12 14:37:15.279167 lib310_lite-0.0.9/lib310_lite/mldl/mldl.py
+-rw-r--r--   0        0        0     1528 2023-05-12 10:35:08.523571 lib310_lite-0.0.9/lib310_lite/mldl/models/InteractionModel.py
+-rw-r--r--   0        0        0     2818 2023-05-12 10:35:08.531397 lib310_lite-0.0.9/lib310_lite/mldl/models/SeqLangModel.py
+-rw-r--r--   0        0        0      799 2023-05-12 12:40:20.982239 lib310_lite-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      937 1970-01-01 00:00:00.000000 lib310_lite-0.0.9/setup.py
+-rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 lib310_lite-0.0.9/PKG-INFO
```

### Comparing `lib310_lite-0.0.8/lib310_lite/bigquery/client.py` & `lib310_lite-0.0.9/lib310_lite/bigquery/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import logging as log
 
 
 class Client(bigquery.Client):
     __PROJECT = 'pfsdb3'
     __CACHE_DATASET = 'cached'
     __BUCKET_NAME = 'bigquery_1'
-    __CACHE_TABLE = 'system.gcs_cache'
+    __CACHE_TABLE = 'system.cached_queries'
 
     def __init__(self):
         super(Client, self).__init__()
 
     def query(self,
               query: str,
               job_config=None,
@@ -111,15 +111,15 @@
         hashed_query = hashlib.sha1(query.encode('utf-8')).hexdigest()
         if days <= 0:
             days = 365
 
         # check for the hit
         row = None
         if not ignore_hit:
-            cached = self.query('SELECT * from `pfsdb3.system.gcs_cache` WHERE status_code != -1').result().to_dataframe()
+            cached = self.query(f'SELECT * from `pfsdb3.{Client.__CACHE_TABLE}` WHERE status_code != -1').result().to_dataframe()
             if len(cached) > 0:
                 cached = cached.where(cached['hash'] == hashed_query).dropna().sort_values(by=['created_at'],
                                                                                            ascending=False)
                 if len(cached) > 0:
                     row = cached.iloc[0].to_dict()
         if row is not None:
             # Hit happened
```

### Comparing `lib310_lite-0.0.8/lib310_lite/bigquery/constants.py` & `lib310_lite-0.0.9/lib310_lite/bigquery/constants.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.8/lib310_lite/mldl/mldl.py` & `lib310_lite-0.0.9/lib310_lite/mldl/mldl.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     __VAL = 'VAL'
     __MAIN = 'MAIN'
     __INTERACTION = 'INTERACTION'
     __PARTS = {__INTERACTION: 1}
 
     def __init__(self, db_url: str, cache_size: int = 50, num_threads: int = 10, random_seed: int = time.time()):
         random.seed(random_seed)
-        self.engine = create_engine(db_url, pool_size= 3 * num_threads, max_overflow = 6 * num_threads, isolation_level='AUTOCOMMIT')
+        self.engine = create_engine(db_url, pool_size=3 * num_threads, max_overflow=6 * num_threads, isolation_level='AUTOCOMMIT')
         self.Session = sessionmaker(bind=self.engine)
 
         self.bq_client = BigQueryClient()
 
         # this is the pool of samples row_id
         self.sample_cache = []
         # this is the maximum number of requests we fetch sooner from the database
@@ -104,19 +104,19 @@
             if interactions_count > 0:
                 tmp_query += f" and interactions_count >= {interactions_count}"
             res = self.bq_client.cache_query(
                 query=tmp_query,
                 name=f'{max_length}_{min_num_feature}_{stage}',
                 destination_format=FileFormat.CSV
             )
-            print(res)
+            # print(res)
             ddf = dd.read_csv(res['uri'])
             df = ddf.compute()
             self.sample_cache = df['row_id'].tolist()
-            print('HERE')
+            # print('HERE')
 
         # killing the previous thread
         if self.filler_thread is not None:
             self.kill_event.set()
             self.queue.get()
             self.filler_thread.join()
             self.kill_event.clear()
@@ -272,11 +272,12 @@
     def terminate(self):
         """
         Terminate the filler threads and clear the queue
         """
         # Terminate the filler thread
         if self.filler_thread is not None:
             self.kill_event.set()
-            self.queue.get()
+            if not self.queue.empty():
+                self.queue.get()
             self.filler_thread.join()
             self.kill_event.clear()
             self.queue = Queue(self.max_queue_size)
```

### Comparing `lib310_lite-0.0.8/lib310_lite/mldl/models/InteractionModel.py` & `lib310_lite-0.0.9/lib310_lite/mldl/models/InteractionModel.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.8/lib310_lite/mldl/models/SeqLangModel.py` & `lib310_lite-0.0.9/lib310_lite/mldl/models/SeqLangModel.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.8/pyproject.toml` & `lib310_lite-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib310_lite"
-version = "0.0.8"
+version = "0.0.9"
 description = "lib310 Lite Python Package"
 authors = ["310 <info@310.ai>"]
 maintainers = ["Saman Fekri <saman@310.ai>"]
 keywords = ["biology", "AI", "genomics", "bioinforma", "machine learning", "GAN"]
 packages = [
     { include = "lib310_lite" }
 ]
```

### Comparing `lib310_lite-0.0.8/setup.py` & `lib310_lite-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'google-cloud-bigquery>=3.2.0',
  'google-cloud>=0.34.0',
  'numpy<1.23.0',
  'psycopg2-binary>=2.9.0']
 
 setup_kwargs = {
     'name': 'lib310-lite',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'lib310 Lite Python Package',
     'long_description': 'None',
     'author': '310',
     'author_email': 'info@310.ai',
     'maintainer': 'Saman Fekri',
     'maintainer_email': 'saman@310.ai',
     'url': 'None',
```

### Comparing `lib310_lite-0.0.8/PKG-INFO` & `lib310_lite-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib310-lite
-Version: 0.0.8
+Version: 0.0.9
 Summary: lib310 Lite Python Package
 Keywords: biology,AI,genomics,bioinforma,machine learning,GAN
 Author: 310
 Author-email: info@310.ai
 Maintainer: Saman Fekri
 Maintainer-email: saman@310.ai
 Requires-Python: >=3.8
```


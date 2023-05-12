# Comparing `tmp/lib310_lite-0.0.7.tar.gz` & `tmp/lib310_lite-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib310_lite-0.0.7.tar", max compression
+gzip compressed data, was "lib310_lite-0.0.8.tar", max compression
```

## Comparing `lib310_lite-0.0.7.tar` & `lib310_lite-0.0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      249 2023-03-08 14:56:22.920616 lib310_lite-0.0.7/lib310_lite/__init__.py
--rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.0.7/lib310_lite/bigquery/_functions.py
--rw-r--r--   0        0        0     7467 2023-05-08 08:51:40.656605 lib310_lite-0.0.7/lib310_lite/bigquery/client.py
--rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.0.7/lib310_lite/bigquery/constants.py
--rw-r--r--   0        0        0       35 2023-03-07 10:52:53.179251 lib310_lite-0.0.7/lib310_lite/fucntion.py
--rw-r--r--   0        0        0     9904 2023-05-10 16:00:03.916082 lib310_lite-0.0.7/lib310_lite/mldl/mldl.py
--rw-r--r--   0        0        0      843 2023-05-10 15:57:55.593952 lib310_lite-0.0.7/lib310_lite/mldl/models/InteractionModel.py
--rw-r--r--   0        0        0     2102 2023-05-10 15:57:55.594201 lib310_lite-0.0.7/lib310_lite/mldl/models/SeqLangModel.py
--rw-r--r--   0        0        0      799 2023-05-10 16:00:38.896608 lib310_lite-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      937 1970-01-01 00:00:00.000000 lib310_lite-0.0.7/setup.py
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 lib310_lite-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      249 2023-03-08 14:56:22.920616 lib310_lite-0.0.8/lib310_lite/__init__.py
+-rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.0.8/lib310_lite/bigquery/_functions.py
+-rw-r--r--   0        0        0     7467 2023-05-08 08:51:40.656605 lib310_lite-0.0.8/lib310_lite/bigquery/client.py
+-rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.0.8/lib310_lite/bigquery/constants.py
+-rw-r--r--   0        0        0       35 2023-03-07 10:52:53.179251 lib310_lite-0.0.8/lib310_lite/fucntion.py
+-rw-r--r--   0        0        0    12058 2023-05-12 10:37:55.686425 lib310_lite-0.0.8/lib310_lite/mldl/mldl.py
+-rw-r--r--   0        0        0     1528 2023-05-12 10:35:08.523571 lib310_lite-0.0.8/lib310_lite/mldl/models/InteractionModel.py
+-rw-r--r--   0        0        0     2818 2023-05-12 10:35:08.531397 lib310_lite-0.0.8/lib310_lite/mldl/models/SeqLangModel.py
+-rw-r--r--   0        0        0      799 2023-05-12 11:20:31.446520 lib310_lite-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      937 1970-01-01 00:00:00.000000 lib310_lite-0.0.8/setup.py
+-rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 lib310_lite-0.0.8/PKG-INFO
```

### Comparing `lib310_lite-0.0.7/lib310_lite/bigquery/client.py` & `lib310_lite-0.0.8/lib310_lite/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.7/lib310_lite/bigquery/constants.py` & `lib310_lite-0.0.8/lib310_lite/bigquery/constants.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.7/lib310_lite/mldl/mldl.py` & `lib310_lite-0.0.8/lib310_lite/mldl/mldl.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,30 +11,32 @@
 from ..bigquery.constants import FileFormat
 import hashlib
 
 # PGSQL
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.pool import NullPool
-from .models.SeqLangModel import SeqLangModel
-from .models.InteractionModel import InteractionModel
+from .models.SeqLangModel import SeqLangModel, SeqLang300Model, SeqLangT10Model, SeqLang300T10Model
+from .models.InteractionModel import InteractionModel, Interaction300Model, InteractionT10Model, Interaction300T10Model
+
+import time
 
 
 class MLDL:
 
     __TRAIN = 'TRAIN'
     __TEST = 'TEST'
     __VAL = 'VAL'
     __MAIN = 'MAIN'
     __INTERACTION = 'INTERACTION'
     __PARTS = {__INTERACTION: 1}
 
     def __init__(self, db_url: str, cache_size: int = 50, num_threads: int = 10, random_seed: int = time.time()):
         random.seed(random_seed)
-        self.engine = create_engine(db_url, poolclass=NullPool, isolation_level='READ UNCOMMITTED')
+        self.engine = create_engine(db_url, pool_size= 3 * num_threads, max_overflow = 6 * num_threads, isolation_level='AUTOCOMMIT')
         self.Session = sessionmaker(bind=self.engine)
 
         self.bq_client = BigQueryClient()
 
         # this is the pool of samples row_id
         self.sample_cache = []
         # this is the maximum number of requests we fetch sooner from the database
@@ -102,82 +104,88 @@
             if interactions_count > 0:
                 tmp_query += f" and interactions_count >= {interactions_count}"
             res = self.bq_client.cache_query(
                 query=tmp_query,
                 name=f'{max_length}_{min_num_feature}_{stage}',
                 destination_format=FileFormat.CSV
             )
+            print(res)
             ddf = dd.read_csv(res['uri'])
             df = ddf.compute()
             self.sample_cache = df['row_id'].tolist()
+            print('HERE')
 
         # killing the previous thread
         if self.filler_thread is not None:
             self.kill_event.set()
             self.queue.get()
             self.filler_thread.join()
             self.kill_event.clear()
             self.queue = Queue(self.max_queue_size)
 
         # generate new key
         self.queue_key = qk
 
         # start new thread
-        self.filler_thread = Thread(target=self.filler, args=(num, stage, parts))
+        self.filler_thread = Thread(target=self.filler, args=(num, stage, max_length, min_num_feature, parts))
         self.filler_thread.start()
 
         # if we do not put this it could effect on the performance of the program because of the racing between threads
         time.sleep(3)
 
-        return self.fetch_sample(num, stage, parts)
+        return self.fetch_sample(num, stage, max_length, min_num_feature, parts)
 
-    def filler(self, num: int, stage: str, parts: dict = None):
+    def filler(self, num: int, stage: str, length: int, token_size: int, parts: dict = None):
         """
         This function is used to fill the queue with data then get batch read data from the queue
         :param num: number of samples
         :param stage: TRAIN or TEST
+        :param length: maximum length of the sequence
+        :param token_size: minimum number of features
         :param parts: the parts of the data that we want to fetch
         """
         if parts is None:
             parts = MLDL.__PARTS
         with BoundedThreadPoolExecutor(max_workers=self.num_threads) as executor:
             while not self.kill_event.is_set():
-                executor.submit(self.filler_worker, num, stage, parts)
+                executor.submit(self.filler_worker, num, stage, length, token_size, parts)
             while not self.queue.empty():
                 self.queue.get()
             executor.shutdown(wait=True)
 
-    def filler_worker(self, num: int, stage: str, parts: dict = None):
+    def filler_worker(self, num: int, stage: str, length: int, token_size: int, parts: dict = None):
         if parts is None:
             parts = MLDL.__PARTS
-        df = self.fetch_sample(num, stage, parts)
+        df = self.fetch_sample(num, stage, length, token_size, parts)
         self.queue.put(df)
         return
 
-    def fetch_sample(self, num: int, stage: str, parts: dict = None, retry: int = 0):
+    def fetch_sample(self, num: int, stage: str, length: int, token_size: int, parts: dict = None, retry: int = 0):
         """
         This function is used to fetch the data from the database
         Run two threads to fetch the data from the database
         :param num: number of samples
         :param stage: TRAIN or TEST or VAL or any other stage
+        :param length: maximum length of the sequence
+        :param token_size: minimum number of features
         :param parts: the parts of the data that we want to fetch
         :param retry: number of retries max is constant 7
         :return: dataframe of the data
         """
 
         if parts is None:
             parts = MLDL.__PARTS
         try:
             # get random row_id from the pool
             index_list = random.sample(self.sample_cache, min(num, len(self.sample_cache)))
 
             with concurrent.futures.ThreadPoolExecutor() as executor:
-                main_thread = executor.submit(self.fetch_sample_main, index_list, parts)
+                main_thread = executor.submit(self.fetch_sample_main, index_list, length, token_size, parts)
                 if parts[MLDL.__INTERACTION] and parts[MLDL.__INTERACTION] == 1:
-                    interaction_thread = executor.submit(self.fetch_sample_interaction, index_list)
+                    interaction_thread = executor.submit(self.fetch_sample_interaction, index_list, length, token_size)
 
                 main_df = main_thread.result()
 
                 interaction_df = pd.DataFrame()
                 if parts[MLDL.__INTERACTION] and parts[MLDL.__INTERACTION] == 1:
                     interaction_df = interaction_thread.result()
 
@@ -194,51 +202,75 @@
                 time.sleep(1)
             else:
                 time.sleep(retry * 10)
             retry += 1
             print(f'Cannot fetch data from database, retry number {retry} times')
             if retry > 7:
                 raise Exception('Cannot fetch data from database')
-            return self.fetch_sample(num, stage, parts, retry)
+            return self.fetch_sample(num, stage, length, token_size, parts, retry)
 
-    def fetch_sample_main(self, index_list: list, parts: dict = None):
+    def fetch_sample_main(self, index_list: list, length: int, token_size: int, parts: dict = None):
         """
         This function is used to fetch the main data from the database
         :param index_list: list of row_ids
+        :param length: maximum length of the sequence
+        :param token_size: minimum number of features
         :param parts: parts of the data
         :return: dataframe of main data
         """
+        # s = time.perf_counter()
         session = self.Session()
         if parts is None:
             parts = MLDL.__PARTS
         try:
-            results = session.query(SeqLangModel).filter(SeqLangModel.row_id.in_(index_list)).all()
+            if token_size >= 10 and length <= 300:
+                results = session.query(SeqLang300T10Model).filter(SeqLang300T10Model.row_id.in_(index_list)).all()
+            elif token_size >= 10:
+                results = session.query(SeqLangT10Model).filter(SeqLangT10Model.row_id.in_(index_list)).all()
+            elif length <= 300:
+                results = session.query(SeqLang300Model).filter(SeqLang300Model.row_id.in_(index_list)).all()
+            else:
+                results = session.query(SeqLangModel).filter(SeqLangModel.row_id.in_(index_list)).all()
             df = pd.DataFrame([r.to_dict() for r in results])
         except Exception as e:
             print(e)
             raise Exception('Cannot fetch data from database <SeqLang>')
         finally:
             session.close()
+        # print('fetch_sample_main')
+        # print(time.perf_counter() - s)
         return df
 
-    def fetch_sample_interaction(self, index_list: list):
+    def fetch_sample_interaction(self, index_list: list, length: int, token_size: int):
         """
         This function is used to fetch the interaction data from the database
         :param index_list: list of row_ids
+        :param length: maximum length of the sequence
+        :param token_size: size of the token
         :return: dataframe of interaction data
         """
+        # s = time.perf_counter()
         session = self.Session()
         try:
-            results = session.query(InteractionModel).filter(InteractionModel.row_id.in_(index_list)).all()
+            if token_size >= 10 and length <= 300:
+                results = session.query(Interaction300T10Model).filter(Interaction300T10Model.row_id.in_(index_list)).all()
+            elif token_size >= 10:
+                results = session.query(InteractionT10Model).filter(InteractionT10Model.row_id.in_(index_list)).all()
+            elif length <= 300:
+                results = session.query(Interaction300Model).filter(Interaction300Model.row_id.in_(index_list)).all()
+            else:
+                results = session.query(InteractionModel).filter(InteractionModel.row_id.in_(index_list)).all()
             df = pd.DataFrame([r.to_dict() for r in results])
         except Exception as e:
             print(e)
             raise Exception('Cannot fetch data from database <Interaction>')
         finally:
             session.close()
+        # print('fetch_sample_interaction')
+        # print(time.perf_counter() - s)
         return df
 
     def terminate(self):
         """
         Terminate the filler threads and clear the queue
         """
         # Terminate the filler thread
```

### Comparing `lib310_lite-0.0.7/lib310_lite/mldl/models/SeqLangModel.py` & `lib310_lite-0.0.8/lib310_lite/mldl/models/SeqLangModel.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any
 from sqlalchemy import Column, Integer, String, Float, ARRAY
 from sqlalchemy.ext.declarative import declarative_base
 
 Base = declarative_base()
 
 
-class SeqLangModel(Base):
-    __tablename__ = 'seq_lang'
+class SeqLangBaseModel(Base):
+    __abstract__ = True
 
     row_id = Column(Integer, primary_key=True)
     uniparc_id = Column(String)
     sequence = Column(String)
     len = Column(Integer)
     stage = Column(String)
     token_size = Column(Integer)
@@ -48,7 +48,35 @@
             'taxonomies': self.taxonomies,
             'organisms': self.organisms,
         }
         return d
 
     def __repr__(self) -> str:
         return f"<SeqLangModel(uniparc_id='{self.uniparc_id}', sequence='{self.sequence}', len={self.len}, stage='{self.stage}', token_size={self.token_size}, token_ids={self.token_ids}, token_names='{self.token_names}', protein_names='{self.protein_names}', taxonomies='{self.taxonomies}', organisms='{self.organisms}', rand={self.rand})>"
+
+
+class SeqLangModel(SeqLangBaseModel):
+    __tablename__ = 'seq_lang'
+
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        super().__init__(*args, **kwargs)
+
+
+class SeqLang300T10Model(SeqLangBaseModel):
+    __tablename__ = 'seq_lang_300_t10'
+
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        super().__init__(*args, **kwargs)
+
+
+class SeqLang300Model(SeqLangBaseModel):
+    __tablename__ = 'seq_lang_300'
+
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        super().__init__(*args, **kwargs)
+
+
+class SeqLangT10Model(SeqLangBaseModel):
+    __tablename__ = 'seq_lang_t10'
+
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        super().__init__(*args, **kwargs)
```

### Comparing `lib310_lite-0.0.7/pyproject.toml` & `lib310_lite-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib310_lite"
-version = "0.0.7"
+version = "0.0.8"
 description = "lib310 Lite Python Package"
 authors = ["310 <info@310.ai>"]
 maintainers = ["Saman Fekri <saman@310.ai>"]
 keywords = ["biology", "AI", "genomics", "bioinforma", "machine learning", "GAN"]
 packages = [
     { include = "lib310_lite" }
 ]
```

### Comparing `lib310_lite-0.0.7/setup.py` & `lib310_lite-0.0.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'google-cloud-bigquery>=3.2.0',
  'google-cloud>=0.34.0',
  'numpy<1.23.0',
  'psycopg2-binary>=2.9.0']
 
 setup_kwargs = {
     'name': 'lib310-lite',
-    'version': '0.0.7',
+    'version': '0.0.8',
     'description': 'lib310 Lite Python Package',
     'long_description': 'None',
     'author': '310',
     'author_email': 'info@310.ai',
     'maintainer': 'Saman Fekri',
     'maintainer_email': 'saman@310.ai',
     'url': 'None',
```

### Comparing `lib310_lite-0.0.7/PKG-INFO` & `lib310_lite-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib310-lite
-Version: 0.0.7
+Version: 0.0.8
 Summary: lib310 Lite Python Package
 Keywords: biology,AI,genomics,bioinforma,machine learning,GAN
 Author: 310
 Author-email: info@310.ai
 Maintainer: Saman Fekri
 Maintainer-email: saman@310.ai
 Requires-Python: >=3.8
```


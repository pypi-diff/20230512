# Comparing `tmp/mongomancy-0.1.6.tar.gz` & `tmp/mongomancy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongomancy-0.1.6.tar", last modified: Wed May 10 08:34:40 2023, max compression
+gzip compressed data, was "mongomancy-0.1.7.tar", last modified: Wed May 10 12:41:34 2023, max compression
```

## Comparing `mongomancy-0.1.6.tar` & `mongomancy-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-10 08:34:40.132743 mongomancy-0.1.6/
--rw-r--r--   0 trval     (1000) trval     (1000)     1947 2023-05-10 08:34:13.000000 mongomancy-0.1.6/CHANGELOG.md
--rw-rw-r--   0 trval     (1000) trval     (1000)     1329 2022-09-02 09:33:19.000000 mongomancy-0.1.6/CONTRIBUTING.md
--rw-r--r--   0 trval     (1000) trval     (1000)     1516 2023-04-04 08:06:59.000000 mongomancy-0.1.6/LICENSE
--rw-r--r--   0 trval     (1000) trval     (1000)       42 2023-04-12 12:30:41.000000 mongomancy-0.1.6/MANIFEST.in
--rw-r--r--   0 trval     (1000) trval     (1000)     4466 2023-05-10 08:34:40.132743 mongomancy-0.1.6/PKG-INFO
--rw-r--r--   0 trval     (1000) trval     (1000)     3675 2023-05-10 08:26:11.000000 mongomancy-0.1.6/README.md
--rw-r--r--   0 trval     (1000) trval     (1000)     1368 2023-04-12 12:30:41.000000 mongomancy-0.1.6/pyproject.toml
--rw-rw-r--   0 trval     (1000) trval     (1000)       68 2022-09-02 09:38:35.000000 mongomancy-0.1.6/requirements.txt
--rw-r--r--   0 trval     (1000) trval     (1000)       38 2023-05-10 08:34:40.132743 mongomancy-0.1.6/setup.cfg
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-10 08:34:40.129410 mongomancy-0.1.6/src/
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-10 08:34:40.132743 mongomancy-0.1.6/src/mongomancy/
--rw-r--r--   0 trval     (1000) trval     (1000)      431 2023-05-10 08:34:13.000000 mongomancy-0.1.6/src/mongomancy/__init__.py
--rw-r--r--   0 trval     (1000) trval     (1000)    13993 2023-05-10 08:26:11.000000 mongomancy-0.1.6/src/mongomancy/engine.py
--rw-rw-r--   0 trval     (1000) trval     (1000)      924 2022-08-29 12:44:42.000000 mongomancy-0.1.6/src/mongomancy/mongo_errors.py
--rw-r--r--   0 trval     (1000) trval     (1000)        0 2023-04-12 12:30:41.000000 mongomancy-0.1.6/src/mongomancy/py.typed
--rw-r--r--   0 trval     (1000) trval     (1000)    15558 2023-05-10 08:31:22.000000 mongomancy-0.1.6/src/mongomancy/schema.py
--rw-r--r--   0 trval     (1000) trval     (1000)     6194 2023-05-10 08:26:11.000000 mongomancy-0.1.6/src/mongomancy/types.py
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-10 08:34:40.132743 mongomancy-0.1.6/src/mongomancy.egg-info/
--rw-rw-r--   0 trval     (1000) trval     (1000)     4466 2023-05-10 08:34:40.000000 mongomancy-0.1.6/src/mongomancy.egg-info/PKG-INFO
--rw-rw-r--   0 trval     (1000) trval     (1000)      435 2023-05-10 08:34:40.000000 mongomancy-0.1.6/src/mongomancy.egg-info/SOURCES.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)        1 2023-05-10 08:34:40.000000 mongomancy-0.1.6/src/mongomancy.egg-info/dependency_links.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)       13 2023-05-10 08:34:40.000000 mongomancy-0.1.6/src/mongomancy.egg-info/requires.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)       11 2023-05-10 08:34:40.000000 mongomancy-0.1.6/src/mongomancy.egg-info/top_level.txt
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-10 12:41:34.288725 mongomancy-0.1.7/
+-rw-r--r--   0 trval     (1000) trval     (1000)     2152 2023-05-10 12:38:30.000000 mongomancy-0.1.7/CHANGELOG.md
+-rw-rw-r--   0 trval     (1000) trval     (1000)     1329 2022-09-02 09:33:19.000000 mongomancy-0.1.7/CONTRIBUTING.md
+-rw-r--r--   0 trval     (1000) trval     (1000)     1516 2023-04-04 08:06:59.000000 mongomancy-0.1.7/LICENSE
+-rw-r--r--   0 trval     (1000) trval     (1000)       42 2023-04-12 12:30:41.000000 mongomancy-0.1.7/MANIFEST.in
+-rw-r--r--   0 trval     (1000) trval     (1000)     4466 2023-05-10 12:41:34.288725 mongomancy-0.1.7/PKG-INFO
+-rw-r--r--   0 trval     (1000) trval     (1000)     3675 2023-05-10 08:26:11.000000 mongomancy-0.1.7/README.md
+-rw-r--r--   0 trval     (1000) trval     (1000)     1368 2023-04-12 12:30:41.000000 mongomancy-0.1.7/pyproject.toml
+-rw-rw-r--   0 trval     (1000) trval     (1000)       68 2022-09-02 09:38:35.000000 mongomancy-0.1.7/requirements.txt
+-rw-r--r--   0 trval     (1000) trval     (1000)       38 2023-05-10 12:41:34.288725 mongomancy-0.1.7/setup.cfg
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-10 12:41:34.285391 mongomancy-0.1.7/src/
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-10 12:41:34.288725 mongomancy-0.1.7/src/mongomancy/
+-rw-r--r--   0 trval     (1000) trval     (1000)      431 2023-05-10 12:38:30.000000 mongomancy-0.1.7/src/mongomancy/__init__.py
+-rw-r--r--   0 trval     (1000) trval     (1000)    14650 2023-05-10 12:38:30.000000 mongomancy-0.1.7/src/mongomancy/engine.py
+-rw-rw-r--   0 trval     (1000) trval     (1000)      924 2022-08-29 12:44:42.000000 mongomancy-0.1.7/src/mongomancy/mongo_errors.py
+-rw-r--r--   0 trval     (1000) trval     (1000)        0 2023-04-12 12:30:41.000000 mongomancy-0.1.7/src/mongomancy/py.typed
+-rw-r--r--   0 trval     (1000) trval     (1000)    15322 2023-05-10 12:38:30.000000 mongomancy-0.1.7/src/mongomancy/schema.py
+-rw-r--r--   0 trval     (1000) trval     (1000)     7743 2023-05-10 12:38:30.000000 mongomancy-0.1.7/src/mongomancy/types.py
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-10 12:41:34.288725 mongomancy-0.1.7/src/mongomancy.egg-info/
+-rw-rw-r--   0 trval     (1000) trval     (1000)     4466 2023-05-10 12:41:34.000000 mongomancy-0.1.7/src/mongomancy.egg-info/PKG-INFO
+-rw-rw-r--   0 trval     (1000) trval     (1000)      435 2023-05-10 12:41:34.000000 mongomancy-0.1.7/src/mongomancy.egg-info/SOURCES.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)        1 2023-05-10 12:41:34.000000 mongomancy-0.1.7/src/mongomancy.egg-info/dependency_links.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)       13 2023-05-10 12:41:34.000000 mongomancy-0.1.7/src/mongomancy.egg-info/requires.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)       11 2023-05-10 12:41:34.000000 mongomancy-0.1.7/src/mongomancy.egg-info/top_level.txt
```

### Comparing `mongomancy-0.1.6/CHANGELOG.md` & `mongomancy-0.1.7/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.1.7] - 2023-05-10
+
+### Fix
+
+- lock critical sections `Engine.reconnect`, `Engine.dispose` to prevent unexpected connections states
+- lock `Database.create_all` method to prevent double init at same
+
 ## [0.1.6] - 2023-05-10
 
 ### Fix
 
 - broken default data insert from last commit
 
 ## [0.1.5] - 2023-05-10
```

### Comparing `mongomancy-0.1.6/CONTRIBUTING.md` & `mongomancy-0.1.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.6/LICENSE` & `mongomancy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.6/PKG-INFO` & `mongomancy-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongomancy
-Version: 0.1.6
+Version: 0.1.7
 Summary: Pymongo based python client with data definition layer.
 Author-email: Tom Trval <thandeus@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Ryu-CZ/mongomancy
 Project-URL: Bug Tracker, https://github.com/Ryu-CZ/mongomancy/issues
 Keywords: mongo,python,pymongo,database,nosql
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `mongomancy-0.1.6/README.md` & `mongomancy-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.6/pyproject.toml` & `mongomancy-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.6/src/mongomancy/engine.py` & `mongomancy-0.1.7/src/mongomancy/engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     CONNECTION_ERRORS: ClassVar[Iterable[Type[pymongo.errors.PyMongoError]]] = (
         pymongo.errors.AutoReconnect,
         pymongo.errors.ConnectionFailure,
     )
     disposed: bool
     client: pymongo.MongoClient
     logger: LoggerType
+    semaphore_tower: types.SemaphoreTower
     retry_codes: Set[int]
     write_retry: int
     write_retry_delay: Union[float, int]
     read_retry: int
     read_retry_delay: Union[float, int]
     _address: str
     _connection_params: Mapping[str, Any]
@@ -51,16 +52,15 @@
         "write_retry_delay",
         "read_retry",
         "read_retry_delay",
         "retry_codes",
         "_address",
         "_connection_params",
         "reconnect_hooks",
-        "mp_semaphore",
-        "th_semaphore",
+        "semaphore_tower",
         "disposed",
     )
 
     def __init__(
         self,
         host: str = "localhost",
         port: int = 27017,
@@ -97,14 +97,15 @@
         :exception pymongo.errors.PyMongoError: if database connection could not be established
         """
         super(Engine, self).__init__()
         self.disposed = True
         self.reconnect_hooks = []
         self._address = f"{host}:{port}"
         self.logger = logger or logging.getLogger(type(self).__qualname__)
+        self.semaphore_tower = types.SemaphoreTower(logger=self.logger)
         self.retry_codes = set(retry_codes or mongo_errors.DEFAULT_RETRY)
         # how many times to retry write on error 10107 (switched master)
         self.write_retry = max(0, write_retry or 0)
         # how much time to sleep between retry write on error 10107 (switched master)
         self.write_retry_delay = max(0, write_retry_delay or 0)
         self.read_retry = max(0, read_retry or 0)
         self.read_retry_delay = max(0, read_retry_delay or 0)
@@ -120,17 +121,18 @@
             port=port,
             maxPoolSize=max_pool_size,
             waitQueueTimeoutMS=queue_timeout,
             connectTimeoutMS=connect_timeout,
             **authentication,
             **kwargs,
         )
-        self.client = self._new_client()
-        self.disposed = False
-        atexit.register(self.dispose)
+        with self.semaphore_tower:
+            self.client = self._new_client()
+            self.disposed = False
+            atexit.register(self.dispose)
 
     def __repr__(self) -> str:
         return f"{type(self).__qualname__}(server={self.address!r})"
 
     def __str__(self) -> str:
         return f"{type(self).__name__}(server={self.address!r})"
 
@@ -164,16 +166,27 @@
 
         :param reconnect_hook: hook to be called when client is reconnected
         """
         self.reconnect_hooks.append(reconnect_hook)
 
     def dispose(self) -> None:
         """
+        Cleanup client resources and disconnect from MongoDB. Thread locked and fork locked.
+        """
+        if self.disposed:
+            return
+        with self.semaphore_tower:
+            return self._dispose()
+
+    def _dispose(self) -> None:
+        """
         Cleanup client resources and disconnect from MongoDB.
         """
+        if self.disposed:
+            return
         try:
             self.client.close()
             self.disposed = True
         except PyMongoError as e:
             self.logger.debug(f"Cannot close mongo client because: {e}")
         self.logger.debug(f"{self} - disconnect from MongoDB")
 
@@ -197,15 +210,20 @@
                 time.sleep(self.read_retry_delay)
                 self.reconnect()
             except PyMongoError as e:
                 self.logger.info(f"failed to ping database={database!r} - e={e}")
                 self.logger.warning(traceback.format_stack())
         return bool(is_ok)
 
-    def reconnect(self):
+    def reconnect(self) -> None:
+        """Close existing MongoClient and create new one. Thread locked and fork locked."""
+        with self.semaphore_tower:
+            return self._reconnect()
+
+    def _reconnect(self) -> None:
         """Close existing MongoClient and create new one"""
         self.logger.debug(f"{type(self).__qualname__} - reconnecting client")
         try:
             self.client = self._new_client()
             self.disposed = False
         except (IOError, pymongo.errors.PyMongoError) as e:
             self.logger.error(f"{type(self).__qualname__} - cannot reconnect to mongo server because: {e}")
```

### Comparing `mongomancy-0.1.6/src/mongomancy/mongo_errors.py` & `mongomancy-0.1.7/src/mongomancy/mongo_errors.py`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.6/src/mongomancy/schema.py` & `mongomancy-0.1.7/src/mongomancy/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import logging
-import multiprocessing
-import threading
 import time
 import traceback
 from dataclasses import dataclass
 from typing import (
     List,
     Tuple,
     Union,
@@ -174,28 +172,26 @@
 
     """
 
     engine: types.Executor
     topology: List[types.CollectionDefinition]
     _database: pymongo.database.Database
     _collections: Dict[str, Collection]
-    mp_semaphore: multiprocessing.Semaphore
-    th_semaphore: threading.Semaphore
+    semaphore_tower: types.SemaphoreTower
     logger: LoggerType
     LOCK_COLLECTION: ClassVar[str] = "mongomancy_lock"
     wait_step: float
     max_wait: float
 
     __slots__ = (
         "engine",
         "topology",
         "_database",
         "_collections",
-        "mp_semaphore",
-        "th_semaphore",
+        "semaphore_tower",
         "logger",
         "wait_step",
         "max_wait",
     )
 
     def __init__(
         self,
@@ -204,19 +200,18 @@
         engine: types.Executor,
         *collections: types.CollectionDefinition,
         wait_step: float = 7,
         max_wait: float = 90,
     ) -> None:
         self.max_wait = max_wait
         self.wait_step = wait_step
-        self.mp_semaphore = multiprocessing.Semaphore()
-        self.th_semaphore = threading.Semaphore()
         self._collections = {}
         self.topology = []
         self.logger = logger
+        self.semaphore_tower = types.SemaphoreTower(logger=self.logger)
         self.engine = engine
         self._database = engine.get_database(name)
         for coll in collections:
             self.add_collection(coll)
         self.engine.register_hook(reconnect_hook=self.invalidate_cache_hook)
 
     def __getitem__(self, item: str) -> Collection:
@@ -307,33 +302,32 @@
 
     def create_all(self, skip_existing: bool = True) -> None:
         """
         Create all collections if not exists. Loads `self._collections` for use.
 
         :param skip_existing: skip collection init if collection already exists in db
         """
-        with self.mp_semaphore:
-            with self.th_semaphore:
-                wait_time = 0
-                while not self._lock():
-                    self.logger.debug(f"create_all - process or thread is waiting for master lock {wait_time}sec")
-                    time.sleep(self.wait_step)
-                    wait_time += self.wait_step
-                    if wait_time > self.max_wait:
-                        self.logger.warning(f"create_all - wait timeout after {wait_time}sec and stops waiting")
-                        self._unlock()
-                        break
-                try:
-                    for collection_definition in self.topology:
-                        _ = self.create_collection(collection_definition, skip_existing)
-                except (Exception, KeyError, IndexError, IOError) as e:
-                    self.logger.error(f"create_all failed on {e}")
+        with self.semaphore_tower:
+            wait_time = 0
+            while not self._lock():
+                self.logger.debug(f"create_all - process or thread is waiting for master lock {wait_time}sec")
+                time.sleep(self.wait_step)
+                wait_time += self.wait_step
+                if wait_time > self.max_wait:
+                    self.logger.warning(f"create_all - wait timeout after {wait_time}sec and stops waiting")
                     self._unlock()
-                    raise e from e
+                    break
+            try:
+                for collection_definition in self.topology:
+                    _ = self.create_collection(collection_definition, skip_existing)
+            except (Exception, KeyError, IndexError, IOError) as e:
+                self.logger.error(f"create_all failed on {e}")
                 self._unlock()
+                raise e from e
+            self._unlock()
 
     def create_collection(
         self,
         definition: types.CollectionDefinition,
         skip_existing: bool = True,
     ) -> Collection:
         """
```

### Comparing `mongomancy-0.1.6/src/mongomancy/types.py` & `mongomancy-0.1.7/src/mongomancy/types.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import abc
 import datetime as dt
+import logging
+import multiprocessing
 import sys
+import threading
 import typing
 from collections import OrderedDict
 from dataclasses import dataclass, field
 from typing import (
     OrderedDict as OrderedDictType,
     List,
     Tuple,
@@ -30,45 +33,92 @@
     "BsonList",
     "Index",
     "Document",
     "CollectionDefinition",
     "CollectionContainer",
     "Executor",
     "CommandCursor",
+    "SemaphoreTower",
 )
 
 Bson = Union[None, int, float, bool, str, ObjectId, dt.datetime, Sequence["Bson"], Mapping[str, "Bson"]]
 BsonDict = Mapping[str, Bson]
 BsonList = Sequence[Bson]
 
 OrderedFields = OrderedDictType[str, Union[str, int]]
 if sys.version_info >= (3, 7):
     OrderedFields = Dict[str, Union[str, int]]
 
 OrderedPairs = Union[OrderedFields, Sequence[Tuple[str, Union[str, int]]]]
 
-
-class CollectionContainer(typing.Protocol):
-    dialect_entity: pymongo.collection.Collection
-
-
 METHOD = typing.Literal[
     "find",
     "find_one",
     "find_one_and_update",
     "update_one",
     "update_many",
     "insert_one",
     "insert_many",
     "delete_one",
     "delete_many",
     "aggregate",
 ]
 
 
+class CollectionContainer(typing.Protocol):
+    dialect_entity: pymongo.collection.Collection
+
+
+class SemaphoreTower:
+    __slots__ = (
+        "multiprocess",
+        "thread",
+        "timeout",
+        "logger",
+    )
+    multiprocess: multiprocessing.Semaphore
+    thread: threading.Semaphore
+    timeout: Optional[float]
+    logger: Optional[logging.Logger]
+
+    def __init__(
+        self,
+        value: int = 1,
+        timeout: Optional[float] = None,
+        logger: Optional[logging.Logger] = None,
+    ) -> None:
+        """
+        Helper to make multiple semaphores work as one critical section
+
+        :param value: semaphore init value
+        :param timeout: timeout is used for EACH semaphore in cascade, so result timeout is 2xtimeout
+        :param logger: give me info about what happens here
+        """
+        value = min(value or 1, 1)
+        self.logger = logger
+        self.timeout = timeout
+        self.multiprocess = multiprocessing.Semaphore(value)
+        self.thread = threading.Semaphore(value)
+
+    def __enter__(self):
+        if self.logger:
+            self.logger.debug("waiting for semaphore tower")
+        self.multiprocess.acquire(timeout=self.timeout)
+        self.thread.acquire(timeout=self.timeout)
+        if self.logger:
+            self.logger.debug("entering semaphore tower context")
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.thread.release()
+        self.multiprocess.release()
+        if self.logger:
+            self.logger.debug("released semaphore tower context")
+
+
 @dataclass(init=False)
 class Index:
     """Collection Index data container"""
 
     fields: OrderedDict[str, Union[str, int]]
     name: Optional[str]
     unique: Optional[bool]
```

### Comparing `mongomancy-0.1.6/src/mongomancy.egg-info/PKG-INFO` & `mongomancy-0.1.7/src/mongomancy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongomancy
-Version: 0.1.6
+Version: 0.1.7
 Summary: Pymongo based python client with data definition layer.
 Author-email: Tom Trval <thandeus@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Ryu-CZ/mongomancy
 Project-URL: Bug Tracker, https://github.com/Ryu-CZ/mongomancy/issues
 Keywords: mongo,python,pymongo,database,nosql
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```


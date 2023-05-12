# Comparing `tmp/snapstream-0.0.3.tar.gz` & `tmp/snapstream-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapstream-0.0.3.tar", max compression
+gzip compressed data, was "snapstream-0.0.4.tar", max compression
```

## Comparing `snapstream-0.0.3.tar` & `snapstream-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2023-04-29 18:13:55.378851 snapstream-0.0.3/LICENSE
--rw-r--r--   0        0        0     2236 2023-04-29 18:13:55.378851 snapstream-0.0.3/README.md
--rw-r--r--   0        0        0     1350 2023-04-29 18:14:09.463051 snapstream-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2181 2023-04-29 18:13:55.382851 snapstream-0.0.3/snapstream/__init__.py
--rw-r--r--   0        0        0     7580 2023-04-29 18:13:55.382851 snapstream-0.0.3/snapstream/__main__.py
--rw-r--r--   0        0        0     9509 2023-04-29 18:13:55.382851 snapstream-0.0.3/snapstream/caching.py
--rw-r--r--   0        0        0     2538 2023-04-29 18:13:55.382851 snapstream-0.0.3/snapstream/codecs.py
--rw-r--r--   0        0        0     8531 2023-04-29 18:13:55.382851 snapstream-0.0.3/snapstream/core.py
--rw-r--r--   0        0        0     3241 2023-04-29 18:13:55.382851 snapstream-0.0.3/snapstream/utils.py
--rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 snapstream-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-12 20:12:28.224818 snapstream-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2536 2023-05-12 20:12:28.224818 snapstream-0.0.4/README.md
+-rw-r--r--   0        0        0     1976 2023-05-12 20:12:40.461104 snapstream-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2277 2023-05-12 20:12:28.228818 snapstream-0.0.4/snapstream/__init__.py
+-rw-r--r--   0        0        0     7763 2023-05-12 20:12:28.228818 snapstream-0.0.4/snapstream/__main__.py
+-rw-r--r--   0        0        0     9781 2023-05-12 20:12:28.228818 snapstream-0.0.4/snapstream/caching.py
+-rw-r--r--   0        0        0     2592 2023-05-12 20:12:28.228818 snapstream-0.0.4/snapstream/codecs.py
+-rw-r--r--   0        0        0     9129 2023-05-12 20:12:28.228818 snapstream-0.0.4/snapstream/core.py
+-rw-r--r--   0        0        0     3271 2023-05-12 20:12:28.228818 snapstream-0.0.4/snapstream/utils.py
+-rw-r--r--   0        0        0     4199 1970-01-01 00:00:00.000000 snapstream-0.0.4/PKG-INFO
```

### Comparing `snapstream-0.0.3/LICENSE` & `snapstream-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.3/README.md` & `snapstream-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-[![Test Python Package](https://github.com/Menziess/snapstream/actions/workflows/python-test.yml/badge.svg)](https://github.com/Menziess/snapstream/actions/workflows/python-test.yml)
+[![Test Python Package](https://github.com/Menziess/snapstream/actions/workflows/python-test.yml/badge.svg)](https://github.com/Menziess/snapstream/actions/workflows/python-test.yml) [![Documentation Status](https://readthedocs.org/projects/snapstream/badge/?version=latest)](https://snapstream.readthedocs.io/en/latest/?badge=latest) [![Downloads](https://static.pepy.tech/personalized-badge/snapstream?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=downloads/month)](https://pepy.tech/project/snapstream)
 
 # Snapstream
 
 <img src="https://raw.githubusercontent.com/menziess/snapstream/master/res/logo.png" width="25%" height="25%" align="right" />
 
-A tiny data-flow model with a user-friendly interface that provides sensible defaults for Kafka integration, message serialization/deserialization, and data caching.
+Snapstream provides a data-flow model to simplify development of stateful streaming applications.
 
 ## Installation
 
 ```sh
 pip install snapstream
 ```
 
@@ -57,12 +57,12 @@
 🏆
 ```
 
 ## Features
 
 - [`snapstream.snap`](snapstream/__init__.py): bind streams (iterables) and sinks (callables) to user defined handler functions
 - [`snapstream.stream`](snapstream/__init__.py): start streaming
-- [`snapstream.Topic`](snapstream/core.py): consume from (iterable) and produce to (callable) kafka using [**confluent-kafka**](https://docs.confluent.io/platform/current/clients/confluent-kafka-python/html/index.html)
+- [`snapstream.Topic`](snapstream/core.py): consume from (iterable), and produce to (callable) kafka using [**confluent-kafka**](https://docs.confluent.io/platform/current/clients/confluent-kafka-python/html/index.html)
 - [`snapstream.Cache`](snapstream/caching.py): store data to disk using [**rocksdict**](https://congyuwang.github.io/RocksDict/rocksdict.html)
 - [`snapstream.Conf`](snapstream/core.py): set global kafka configuration (can be overridden per topic)
 - [`snapstream.codecs.AvroCodec`](snapstream/codecs.py): serialize and deserialize avro messages
 - [`snapstream.codecs.JsonCodec`](snapstream/codecs.py): serialize and deserialize json messages
```

### Comparing `snapstream-0.0.3/snapstream/__init__.py` & `snapstream-0.0.4/snapstream/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Snapstream public objects."""
 
+import logging
 from inspect import signature
 from typing import Any, Callable, Generator, Iterable
 
 from pubsub import pub
 
 from snapstream.caching import Cache
 from snapstream.core import READ_FROM_END, READ_FROM_START, Conf, Topic
@@ -14,14 +15,16 @@
     'Conf',
     'Topic',
     'Cache',
     'READ_FROM_START',
     'READ_FROM_END',
 ]
 
+logging.basicConfig()
+
 
 def _sink_output(s: Callable[..., None], output: Any) -> None:
     if not isinstance(output, tuple) and isinstance(s, (Cache)):
         raise ValueError('Cache sink expects: Tuple[key, val].')
     elif isinstance(output, tuple) and isinstance(s, (Cache, Topic)):
         key, val = output
         s(key=key, val=val)
@@ -59,16 +62,18 @@
     c = Conf()
 
     def _deco(f):
         def _handler(msg, kwargs):
             parameters = signature(f).parameters.values()
             if any(p.kind == p.VAR_KEYWORD for p in parameters):
                 output = f(msg, **kwargs)
-            else:
+            elif parameters:
                 output = f(msg)
+            else:
+                output = f()
             _handle_generator_or_function(sink, output)
 
         for it in iterable:
             iterable_key = str(id(it))
             c.register_iterables((iterable_key, it))
             pub.subscribe(_handler, iterable_key)
         return _handler
```

### Comparing `snapstream-0.0.3/snapstream/__main__.py` & `snapstream-0.0.4/snapstream/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from argparse import ArgumentParser, Namespace
 from datetime import datetime as dt
 from datetime import timezone
 from json import dump, dumps, load
 from os import path
 from re import search
 from sys import argv, exit
-from typing import Optional
+from typing import Callable, Optional
 
 from rocksdict import AccessType
-from toolz import curry
+from toolz import compose, curry, identity
 
 from snapstream import READ_FROM_END, Cache, Topic
 from snapstream.codecs import AvroCodec
 from snapstream.utils import folder_size, get_variable
 
 DEFAULT_CONFIG_PATH = '~/'
 CONFIG_FILENAME = '.snapstreamcfg'
@@ -56,30 +56,30 @@
                        help='list of columns to extract from message (if dict), ex: "time,date,pk"')
     cache.add_argument('--stats', action='store_true',
                        help='print additional database statistics')
 
     return parser.parse_args(args)
 
 
-def default_topic_entry(name: str) -> dict:
+def default_topic_entry(name: str, prep: Callable) -> dict:
     """Create default topic entry."""
     return {
         'type': 'Topic',
-        'name': name,
+        'name': prep(name),
         'conf': {
             'bootstrap.servers': 'localhost:29091',
         }
     }
 
 
-def default_cache_entry(path: str) -> dict:
+def default_cache_entry(path: str, prep: Callable) -> dict:
     """Create default topic entry."""
     return {
         'type': 'Cache',
-        'name': path,
+        'path': prep(path),
         'conf': {}
     }
 
 
 def get_config_entry(config_path: str, args: Namespace) -> dict:
     """Update config file."""
     try:
@@ -93,45 +93,46 @@
             .upper()
             .startswith('Y')
         ):
             exit()
         config = []
 
     # Find prop having certain key
-    prop = {
-        'topic': 'name',
-        'cache': 'path',
+    prep, prop = {
+        'topic': [identity, 'name'],
+        'cache': [compose(path.abspath, path.expanduser), 'path'],
     }[args.action]
     key = getattr(args, prop)
     if entry := {
         key: _
         for _ in config
-        if _.get(prop) == key
+        if _.get(prop) == prep(key)
     }.get(key):
         return entry
 
     # If not found, create entry
     entry = (
-        default_topic_entry(args.name) if args.action == 'topic'
-        else default_cache_entry(args.path) if args.action == 'cache'
+        default_topic_entry(args.name, prep) if args.action == 'topic'
+        else default_cache_entry(args.path, prep) if args.action == 'cache'
         else {}
     )
     config.append(entry)
     with open(config_path, 'w') as f:
         dump(config, f, indent=4)
     return entry
 
 
 def replace_variable_references(entry: dict, args: Namespace) -> dict:
     """For every value starting with $, replace with env."""
     conf = entry['conf']
     for k, v in conf.items():
         if v.startswith('$'):
-            updated_v = get_variable(v[1:], args.secrets_base_path)
-            conf[k] = updated_v
+            conf[k] = get_variable(v[1:], args.secrets_base_path)
+        if v.startswith(r'\$'):
+            conf[k] = v.replace()
     entry['conf'] = conf
     return entry
 
 
 def regex_filter(regex: str, key: Optional[str]) -> bool:
     """Check whether key matches regex filter."""
     if regex and key:
```

### Comparing `snapstream-0.0.3/snapstream/caching.py` & `snapstream-0.0.4/snapstream/caching.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,24 @@
                        Rdict, RdictIter, ReadOptions, Snapshot, WriteOptions)
 from rocksdict.rocksdict import RdictItems, RdictKeys, RdictValues
 
 MB, MINUTES = 1024 * 1024, 60
 
 
 class Cache:
-    """A Rocksdb instance."""
+    """Create a RocksDB database in the specified folder.
+
+    >>> cache = Cache('db/mycache')            # doctest: +SKIP
+
+    The cache instance acts as a callable to store data:
+
+    >>> cache('key', {'msg': 'Hello World!'})  # doctest: +SKIP
+    >>> cache['key']                           # doctest: +SKIP
+    {'msg': 'Hello World!'}
+    """
 
     def __init__(
         self,
         path: str,
         options: Union[Options, None] = None,
         column_families: Union[Dict[str, Options], None] = None,
         access_type=AccessType.read_write(),
@@ -83,21 +92,21 @@
         except KeyError:
             pass
 
     def __setitem__(self, key, val) -> None:
         """Set item in db."""
         self.db[key] = val
 
-    def __enter__(self) -> Rdict:
+    def __enter__(self) -> 'Cache':
         """Contextmanager."""
-        return self.db.__enter__()
+        return self
 
     def __exit__(self, exc_type, exc_val, exc_tb) -> None:
         """Exit contextmanager."""
-        self.db.__exit__(exc_type, exc_val, exc_tb)
+        self.close()
 
     def set_dumps(self, dumps: Callable[[Any], bytes]) -> None:
         """Set custom dumps function."""
         return self.db.set_dumps(dumps)
 
     def set_loads(self, dumps: Callable[[bytes], Any]) -> None:
         """Set custom loads function."""
```

### Comparing `snapstream-0.0.3/snapstream/codecs.py` & `snapstream-0.0.4/snapstream/codecs.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Any, cast
 
 from avro.io import BinaryDecoder, BinaryEncoder, DatumReader, DatumWriter
 from avro.schema import Schema, parse
 from toolz import curry
 
 logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)
 
 
 def deserialize_json(msg: bytes) -> dict:
     """Deserialize json message."""
     return loads(msg.decode())
 
 
@@ -62,27 +63,27 @@
     @abstractmethod
     def decode(self, s: bytes) -> object:
         """Deserialize object."""
         raise NotImplementedError
 
 
 class JsonCodec(ICodec):
-    """Codec for avro messages."""
+    """Serialize/deserialize json messages."""
 
     def encode(self, obj: Any) -> bytes:
         """Serialize message."""
         return serialize_json(obj)
 
     def decode(self, s: bytes) -> object:
         """Deserialize message."""
         return deserialize_json(s)
 
 
 class AvroCodec(ICodec):
-    """Codec for avro messages."""
+    """Serialize/deserialize avro messages."""
 
     def __init__(self, path: str):
         """Load avro schema."""
         with open(path) as a:
             self.schema = parse(a.read())
 
     def encode(self, obj: Any) -> bytes:
```

### Comparing `snapstream-0.0.3/snapstream/core.py` & `snapstream-0.0.4/snapstream/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,22 +14,28 @@
 from confluent_kafka.error import KafkaException
 from pubsub import pub
 from toolz import pipe
 
 from snapstream.codecs import ICodec
 from snapstream.utils import KafkaIgnoredPropertyFilter, Singleton
 
-logger = logging.getLogger(__file__)
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)
+logger.addFilter(KafkaIgnoredPropertyFilter())
 
 READ_FROM_START = -2
 READ_FROM_END = -1
 
 
 class Conf(metaclass=Singleton):
-    """Defines app configuration."""
+    """Define default kafka configuration, optionally.
+
+    >>> Conf({'bootstrap.servers': 'localhost:29091'})
+    {'bootstrap.servers': 'localhost:29091'}
+    """
 
     iterables: Set[Tuple[str, Iterable]] = set()
 
     def register_iterables(self, *it):
         """Add iterables to global Conf."""
         self.iterables.add(*it)
 
@@ -45,16 +51,14 @@
             queue.put(e)
         finally:
             queue.put(None)
             logger.debug(f'Stopping thread {current_thread().name}.')
 
     def start(self, **kwargs):
         """Start the streams."""
-        logger.addFilter(KafkaIgnoredPropertyFilter())
-
         queue = Queue(maxsize=1)
         threads = [
             Thread(
                 target=self.distribute_messages,
                 args=(it, queue, kwargs)
             )
             for _, it in self.iterables
@@ -65,15 +69,15 @@
                 logger.debug(f'Spawning thread {t.name}.')
                 t.daemon = True
                 t.start()
             while any(t.is_alive() for t in threads):
                 if exception := queue.get():
                     raise exception
         except KeyboardInterrupt:
-            logger.info('You stopped the program.')
+            exit()
         finally:
             self.iterables = set()
 
     def __init__(self, conf: dict = {}) -> None:
         """Define init behavior."""
         self.conf: Dict[str, Any] = {}
         self.__update__(conf)
@@ -108,15 +112,15 @@
         """
         raise NotImplementedError
 
     @abstractmethod
     def create_topic(self, name: str, *args: Any, **kwargs: Dict[str, Any]) -> None:
         """Create topic.
 
-        - Should allow *args, **kwargs passthrough to kafka client.
+        - Should allow `*args`, `**kwargs` passthrough to kafka client.
         - Should log warning if topic already exists.
         """
         raise NotImplementedError
 
     @abstractmethod
     def __iter__(self) -> Iterable[Any]:
         """Consume from topic.
@@ -226,15 +230,31 @@
 
     yield produce
 
     p.flush(flush_timeout)
 
 
 class Topic(ITopic):
-    """Act as producer and consumer."""
+    """Act as a consumer and producer.
+
+    >>> topic = Topic('emoji', {
+    ...     'bootstrap.servers': 'localhost:29091',
+    ...     'auto.offset.reset': 'earliest',
+    ...     'group.id': 'demo',
+    ... })
+
+    Loop over topic (iterable) to consume from it:
+
+    >>> for msg in topic:               # doctest: +SKIP
+    ...     print(msg.value())
+
+    Call topic (callable) with data to produce to it:
+
+    >>> topic({'msg': 'Hello World!'})  # doctest: +SKIP
+    """
 
     def __init__(
         self,
         name: str,
         conf: dict = {},
         offset: Optional[int] = None,
         codec: Optional[ICodec] = None,
@@ -253,14 +273,18 @@
         self.poll_timeout = poll_timeout
         self.producer = None
         self.callback = callback
         self.poller = poller
         self.codec = codec
         self.dry = dry
 
+    def admin(self):
+        """Get admin client."""
+        return AdminClient(self.conf)
+
     def create_topic(self, *args, **kwargs) -> None:
         """Create topic."""
         admin = AdminClient(self.conf)
         for t, f in admin.create_topics([NewTopic(self.name, *args, **kwargs)]).items():
             try:
                 f.result()
                 logger.debug(f"Topic {t} created.")
@@ -276,14 +300,12 @@
         c = get_consumer(self.name, self.conf, self.starting_offset, self.codec, self.poll_timeout, self.poller)
         with c as consumer:
             for msg in consumer:
                 yield msg
 
     def __call__(self, val, key=None, *args, **kwargs) -> None:
         """Produce to topic."""
-        if not (key or val):
-            return
         self.producer = (
             self.producer or
             get_producer(self.name, self.conf, self.dry, self.codec, self.flush_timeout, self.callback).__enter__()
         )
         self.producer(key, val, *args, **kwargs)
```

### Comparing `snapstream-0.0.3/snapstream/utils.py` & `snapstream-0.0.4/snapstream/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pathlib import Path
 from re import match, sub
 from typing import Any, Dict, Optional
 
 from toolz.curried import compose, curry, last
 
 logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)
 
 
 def get_variable(
     secret: str,
     secrets_base_path='',
     required=False
 ) -> Optional[str]:
```

### Comparing `snapstream-0.0.3/PKG-INFO` & `snapstream-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 Metadata-Version: 2.1
 Name: snapstream
-Version: 0.0.3
+Version: 0.0.4
 Summary: Streamline your Kafka data processing, this tool aims to standardize streaming data from multiple Kafka clusters. With a pub-sub approach, multiple functions can easily subscribe to incoming messages, serialization can be specified per topic, and data is automatically processed by data sink functions.
 Home-page: https://github.com/Menziess/snapstream
 License: MIT
 Keywords: kafka,pubsub
 Author: Menziess
 Author-email: stefan_schenk@hotmail.com
 Requires-Python: >=3.8.1,<4.0.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: avro (>=1.11.1,<2.0.0)
 Requires-Dist: confluent-kafka (>=2.0.2,<3.0.0)
 Requires-Dist: pypubsub (>=4.0.3,<5.0.0)
 Requires-Dist: pyright (>=1.1.302,<2.0.0)
 Requires-Dist: rocksdict (>=0.3.10,<0.4.0)
 Requires-Dist: toolz (>=0.12.0,<0.13.0)
+Project-URL: Documentation, https://snapstream.readthedocs.io
 Project-URL: Repository, https://github.com/Menziess/snapstream
 Description-Content-Type: text/markdown
 
-[![Test Python Package](https://github.com/Menziess/snapstream/actions/workflows/python-test.yml/badge.svg)](https://github.com/Menziess/snapstream/actions/workflows/python-test.yml)
+[![Test Python Package](https://github.com/Menziess/snapstream/actions/workflows/python-test.yml/badge.svg)](https://github.com/Menziess/snapstream/actions/workflows/python-test.yml) [![Documentation Status](https://readthedocs.org/projects/snapstream/badge/?version=latest)](https://snapstream.readthedocs.io/en/latest/?badge=latest) [![Downloads](https://static.pepy.tech/personalized-badge/snapstream?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=downloads/month)](https://pepy.tech/project/snapstream)
 
 # Snapstream
 
 <img src="https://raw.githubusercontent.com/menziess/snapstream/master/res/logo.png" width="25%" height="25%" align="right" />
 
-A tiny data-flow model with a user-friendly interface that provides sensible defaults for Kafka integration, message serialization/deserialization, and data caching.
+Snapstream provides a data-flow model to simplify development of stateful streaming applications.
 
 ## Installation
 
 ```sh
 pip install snapstream
 ```
 
@@ -81,13 +91,13 @@
 🏆
 ```
 
 ## Features
 
 - [`snapstream.snap`](snapstream/__init__.py): bind streams (iterables) and sinks (callables) to user defined handler functions
 - [`snapstream.stream`](snapstream/__init__.py): start streaming
-- [`snapstream.Topic`](snapstream/core.py): consume from (iterable) and produce to (callable) kafka using [**confluent-kafka**](https://docs.confluent.io/platform/current/clients/confluent-kafka-python/html/index.html)
+- [`snapstream.Topic`](snapstream/core.py): consume from (iterable), and produce to (callable) kafka using [**confluent-kafka**](https://docs.confluent.io/platform/current/clients/confluent-kafka-python/html/index.html)
 - [`snapstream.Cache`](snapstream/caching.py): store data to disk using [**rocksdict**](https://congyuwang.github.io/RocksDict/rocksdict.html)
 - [`snapstream.Conf`](snapstream/core.py): set global kafka configuration (can be overridden per topic)
 - [`snapstream.codecs.AvroCodec`](snapstream/codecs.py): serialize and deserialize avro messages
 - [`snapstream.codecs.JsonCodec`](snapstream/codecs.py): serialize and deserialize json messages
```


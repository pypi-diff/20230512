# Comparing `tmp/amqp_workers-0.1.0.tar.gz` & `tmp/amqp_workers-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amqp_workers-0.1.0.tar", max compression
+gzip compressed data, was "amqp_workers-0.1.1.tar", max compression
```

## Comparing `amqp_workers-0.1.0.tar` & `amqp_workers-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0        0 2023-04-27 01:38:48.372295 amqp_workers-0.1.0/amqpworker/__init__.py
--rw-r--r--   0        0        0     8289 2023-04-28 03:17:45.822032 amqp_workers-0.1.0/amqpworker/app.py
--rw-r--r--   0        0        0      899 2023-04-27 00:37:11.054428 amqp_workers-0.1.0/amqpworker/bucket.py
--rw-r--r--   0        0        0     1108 2023-04-28 03:13:55.374031 amqp_workers-0.1.0/amqpworker/conf.py
--rw-r--r--   0        0        0     5247 2023-04-27 04:04:35.910995 amqp_workers-0.1.0/amqpworker/connections.py
--rw-r--r--   0        0        0     9166 2023-04-28 02:06:33.051333 amqp_workers-0.1.0/amqpworker/consumer.py
--rw-r--r--   0        0        0      867 2023-04-27 02:02:41.661122 amqp_workers-0.1.0/amqpworker/decorators.py
--rw-r--r--   0        0        0        0 2023-04-27 00:37:11.056429 amqp_workers-0.1.0/amqpworker/easyqueue/__init__.py
--rw-r--r--   0        0        0     2300 2023-04-27 06:31:02.852491 amqp_workers-0.1.0/amqpworker/easyqueue/connection.py
--rw-r--r--   0        0        0      415 2023-04-27 00:37:11.056929 amqp_workers-0.1.0/amqpworker/easyqueue/exceptions.py
--rw-r--r--   0        0        0     2682 2023-04-27 08:20:45.459864 amqp_workers-0.1.0/amqpworker/easyqueue/message.py
--rw-r--r--   0        0        0    12078 2023-04-28 03:28:54.313947 amqp_workers-0.1.0/amqpworker/easyqueue/queue.py
--rw-r--r--   0        0        0      652 2023-04-28 02:06:33.017336 amqp_workers-0.1.0/amqpworker/entrypoints.py
--rw-r--r--   0        0        0      220 2023-04-27 00:37:11.058429 amqp_workers-0.1.0/amqpworker/exceptions.py
--rw-r--r--   0        0        0      918 2023-04-28 02:06:33.010338 amqp_workers-0.1.0/amqpworker/options.py
--rw-r--r--   0        0        0      102 2023-04-27 03:25:18.698414 amqp_workers-0.1.0/amqpworker/rabbitmq/__init__.py
--rw-r--r--   0        0        0     1217 2023-04-28 02:06:33.068336 amqp_workers-0.1.0/amqpworker/rabbitmq/entrypoints.py
--rw-r--r--   0        0        0     2040 2023-04-27 08:36:53.107610 amqp_workers-0.1.0/amqpworker/rabbitmq/message.py
--rw-r--r--   0        0        0     3815 2023-04-28 02:06:33.060333 amqp_workers-0.1.0/amqpworker/routes.py
--rw-r--r--   0        0        0     6701 2023-04-28 00:01:14.997514 amqp_workers-0.1.0/amqpworker/scheduled/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 01:46:21.379571 amqp_workers-0.1.0/amqpworker/signals/__init__.py
--rw-r--r--   0        0        0     1023 2023-04-27 01:53:14.068404 amqp_workers-0.1.0/amqpworker/signals/base.py
--rw-r--r--   0        0        0        0 2023-04-27 01:49:26.864472 amqp_workers-0.1.0/amqpworker/signals/handlers/__init__.py
--rw-r--r--   0        0        0      288 2023-04-27 02:02:41.649901 amqp_workers-0.1.0/amqpworker/signals/handlers/base.py
--rw-r--r--   0        0        0     1613 2023-04-28 01:28:30.030083 amqp_workers-0.1.0/amqpworker/signals/handlers/rabbitmq.py
--rw-r--r--   0        0        0        0 2023-04-27 00:37:11.071433 amqp_workers-0.1.0/amqpworker/types/__init__.py
--rw-r--r--   0        0        0     1611 2023-04-27 03:21:21.484561 amqp_workers-0.1.0/amqpworker/types/registry.py
--rw-r--r--   0        0        0     1688 2023-04-27 03:25:18.733914 amqp_workers-0.1.0/amqpworker/typing/__init__.py
--rw-r--r--   0        0        0      208 2023-04-27 05:43:33.253806 amqp_workers-0.1.0/amqpworker/utils.py
--rw-r--r--   0        0        0     1131 2023-05-08 08:02:08.608402 amqp_workers-0.1.0/LICENSE
--rw-r--r--   0        0        0      791 2023-05-08 07:54:06.719209 amqp_workers-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2677 2023-05-08 07:41:58.705174 amqp_workers-0.1.0/README.md
--rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 amqp_workers-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-27 01:38:48.372295 amqp_workers-0.1.1/amqpworker/__init__.py
+-rw-r--r--   0        0        0     8274 2023-05-08 09:50:20.919904 amqp_workers-0.1.1/amqpworker/app.py
+-rw-r--r--   0        0        0      899 2023-04-27 00:37:11.054428 amqp_workers-0.1.1/amqpworker/bucket.py
+-rw-r--r--   0        0        0     1108 2023-04-28 03:13:55.374031 amqp_workers-0.1.1/amqpworker/conf.py
+-rw-r--r--   0        0        0     5247 2023-04-27 04:04:35.910995 amqp_workers-0.1.1/amqpworker/connections.py
+-rw-r--r--   0        0        0     9263 2023-05-12 00:55:25.860622 amqp_workers-0.1.1/amqpworker/consumer.py
+-rw-r--r--   0        0        0      867 2023-04-27 02:02:41.661122 amqp_workers-0.1.1/amqpworker/decorators.py
+-rw-r--r--   0        0        0        0 2023-04-27 00:37:11.056429 amqp_workers-0.1.1/amqpworker/easyqueue/__init__.py
+-rw-r--r--   0        0        0     2300 2023-04-27 06:31:02.852491 amqp_workers-0.1.1/amqpworker/easyqueue/connection.py
+-rw-r--r--   0        0        0      415 2023-04-27 00:37:11.056929 amqp_workers-0.1.1/amqpworker/easyqueue/exceptions.py
+-rw-r--r--   0        0        0     2660 2023-05-11 08:31:00.365632 amqp_workers-0.1.1/amqpworker/easyqueue/message.py
+-rw-r--r--   0        0        0    12224 2023-05-11 08:31:00.389109 amqp_workers-0.1.1/amqpworker/easyqueue/queue.py
+-rw-r--r--   0        0        0      652 2023-04-28 02:06:33.017336 amqp_workers-0.1.1/amqpworker/entrypoints.py
+-rw-r--r--   0        0        0      220 2023-04-27 00:37:11.058429 amqp_workers-0.1.1/amqpworker/exceptions.py
+-rw-r--r--   0        0        0      918 2023-04-28 02:06:33.010338 amqp_workers-0.1.1/amqpworker/options.py
+-rw-r--r--   0        0        0      102 2023-04-27 03:25:18.698414 amqp_workers-0.1.1/amqpworker/rabbitmq/__init__.py
+-rw-r--r--   0        0        0     1217 2023-04-28 02:06:33.068336 amqp_workers-0.1.1/amqpworker/rabbitmq/entrypoints.py
+-rw-r--r--   0        0        0     2040 2023-04-27 08:36:53.107610 amqp_workers-0.1.1/amqpworker/rabbitmq/message.py
+-rw-r--r--   0        0        0     3815 2023-04-28 02:06:33.060333 amqp_workers-0.1.1/amqpworker/routes.py
+-rw-r--r--   0        0        0     6701 2023-04-28 00:01:14.997514 amqp_workers-0.1.1/amqpworker/scheduled/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 01:46:21.379571 amqp_workers-0.1.1/amqpworker/signals/__init__.py
+-rw-r--r--   0        0        0     1023 2023-04-27 01:53:14.068404 amqp_workers-0.1.1/amqpworker/signals/base.py
+-rw-r--r--   0        0        0        0 2023-04-27 01:49:26.864472 amqp_workers-0.1.1/amqpworker/signals/handlers/__init__.py
+-rw-r--r--   0        0        0      288 2023-04-27 02:02:41.649901 amqp_workers-0.1.1/amqpworker/signals/handlers/base.py
+-rw-r--r--   0        0        0     1613 2023-04-28 01:28:30.030083 amqp_workers-0.1.1/amqpworker/signals/handlers/rabbitmq.py
+-rw-r--r--   0        0        0        0 2023-04-27 00:37:11.071433 amqp_workers-0.1.1/amqpworker/types/__init__.py
+-rw-r--r--   0        0        0     1611 2023-04-27 03:21:21.484561 amqp_workers-0.1.1/amqpworker/types/registry.py
+-rw-r--r--   0        0        0     1688 2023-04-27 03:25:18.733914 amqp_workers-0.1.1/amqpworker/typing/__init__.py
+-rw-r--r--   0        0        0      208 2023-04-27 05:43:33.253806 amqp_workers-0.1.1/amqpworker/utils.py
+-rw-r--r--   0        0        0     1131 2023-05-08 08:02:08.608402 amqp_workers-0.1.1/LICENSE
+-rw-r--r--   0        0        0      974 2023-05-12 01:53:10.320022 amqp_workers-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2970 2023-05-11 09:30:42.780253 amqp_workers-0.1.1/README.md
+-rw-r--r--   0        0        0     3776 1970-01-01 00:00:00.000000 amqp_workers-0.1.1/PKG-INFO
```

### Comparing `amqp_workers-0.1.0/amqpworker/app.py` & `amqp_workers-0.1.1/amqpworker/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import asyncio
 import time
 from collections.abc import MutableMapping
 from signal import Signals
-import signal
 from typing import Any, Dict, Iterable, Optional, Callable
 
 from amqpworker.conf import logger
 from amqpworker.connections import Connection, ConnectionsMapping
 from amqpworker.exceptions import InvalidConnection, InvalidRoute
 from amqpworker.options import Options, DefaultValues, RouteTypes
 from amqpworker.rabbitmq.entrypoints import AMQPRouteEntryPointImpl
```

### Comparing `amqp_workers-0.1.0/amqpworker/bucket.py` & `amqp_workers-0.1.1/amqpworker/bucket.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.0/amqpworker/conf.py` & `amqp_workers-0.1.1/amqpworker/conf.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.0/amqpworker/connections.py` & `amqp_workers-0.1.1/amqpworker/connections.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.0/amqpworker/consumer.py` & `amqp_workers-0.1.1/amqpworker/consumer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import time
 import traceback
 from concurrent.futures import ThreadPoolExecutor
-from concurrent.futures.thread import _shutdown
+# from concurrent.futures.thread import _shutdown
 from typing import Dict, Type, Union
 
 from amqpstorm import AMQPError
 from loguru import logger
 
 from amqpworker import conf
 from amqpworker.easyqueue.message import AMQPMessage
@@ -111,68 +111,69 @@
                     "dest": self.host,
                     "retry": True,
                     "exc_traceback": traceback.format_exc(),
                 }
             )
 
     def _flush_bucket_if_needed(self):
-        try:
-            if not self.bucket.is_empty():
-                all_messages = self.bucket.pop_all()
+
+        if not self.bucket.is_empty():
+            all_messages = self.bucket.pop_all()
+            try:
                 conf.logger.debug(
                     {
                         "event": "bucket-flush",
                         "bucket-size": len(all_messages),
                         "handler": self._handler.__name__,
                     }
                 )
                 if self.running:
                     rv = self._handler(all_messages)
-                    for fu in self.pool.map(call, [m.process_success for m in all_messages]):
+                    for _ in self.pool.map(call, [m.process_success for m in all_messages]):
                         pass
                     return rv
                 else:
                     for m in all_messages:
                         m.process_exception()
-        except AMQPError:
-            raise
-        except Exception as e:
-            traceback.print_exc()
-            if self.running:
-                for fu in self.pool.map(call, [m.process_exception for m in all_messages]):
-                    pass
-            else:
-                for m in all_messages:
-                    m.process_exception()
-            raise e
-
-    def on_queue_error(self, body, delivery_tag, error, queue):
-        """
-        Callback called every time that an error occurred during the validation
-        or deserialization stage.
-
-        :param body: unparsed, raw message content
-        :type body: Any
-        :param delivery_tag: delivery_tag of the consumed message
-        :type delivery_tag: int
-        :param error: THe error that caused the callback to be called
-        :type error: MessageError
-        :type queue: JsonQueue
-        """
-        conf.logger.error(
-            {
-                "parse-error": True,
-                "exception": "Error: not a JSON",
-                "original_msg": body,
-            }
-        )
-        try:
-            queue.ack(delivery_tag=delivery_tag)
-        except AMQPError as e:
-            self._log_exception(e)
+            except AMQPError:
+                raise
+            except Exception as e:
+                traceback.print_exc()
+                if self.running:
+                    for _ in self.pool.map(call, [m.process_exception for m in all_messages]):
+                        pass
+                else:
+                    for m in all_messages:
+                        m.process_exception()
+                raise e
+
+    # def on_queue_error(self, body, delivery_tag, error, queue):
+    #     """
+    #     Callback called every time that an error occurred during the validation
+    #     or deserialization stage.
+    #
+    #     :param body: unparsed, raw message content
+    #     :type body: Any
+    #     :param delivery_tag: delivery_tag of the consumed message
+    #     :type delivery_tag: int
+    #     :param error: THe error that caused the callback to be called
+    #     :type error: MessageError
+    #     :type queue: JsonQueue
+    #     """
+    #     conf.logger.error(
+    #         {
+    #             "parse-error": True,
+    #             "exception": "Error: not a JSON",
+    #             "original_msg": body,
+    #         }
+    #     )
+    #     try:
+    #         queue.ack(delivery_tag=delivery_tag)
+    #     except AMQPError as e:
+    #         self._log_exception(e)
 
     def on_message_handle_error(self, handler_error: Exception, **kwargs):
         """
         Callback called when an uncaught exception was raised during message
         handling stage.
 
         :param handler_error: The exception that triggered
@@ -228,15 +229,15 @@
             self.clock_task = self._flush_clocked
         while self.keep_runnig():
             if not self.queue.connection.has_channel_ready():
                 try:
                     self.consume_all_queues(self.queue)
                 except RuntimeError as e:
                     traceback.print_exc()
-                    if self.multiple_queue_pool._shutdown or _shutdown:
+                    if self.multiple_queue_pool._shutdown:  # or _shutdown:
                         conf.logger.info('app shutdown')
                     # if 'interpreter shutdown' in str(e):
                     #     return
                     else:
                         raise
                 except KeyboardInterrupt:
                     self.stop()
```

### Comparing `amqp_workers-0.1.0/amqpworker/decorators.py` & `amqp_workers-0.1.1/amqpworker/decorators.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.0/amqpworker/easyqueue/connection.py` & `amqp_workers-0.1.1/amqpworker/easyqueue/connection.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.0/amqpworker/easyqueue/message.py` & `amqp_workers-0.1.1/amqpworker/easyqueue/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 class AMQPMessage(Generic[T]):
     __slots__ = (
         "connection",
         "channel",
         "queue_name",
         "serialized_data",
         "delivery_tag",
-        "_envelope",
         "_properties",
         "_deserialization_method",
         "_deserialized_data",
         "_queue",
     )
 
     def __init__(
```

### Comparing `amqp_workers-0.1.0/amqpworker/easyqueue/queue.py` & `amqp_workers-0.1.1/amqpworker/easyqueue/queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,14 @@
     Optional,
     Type,
     TypeVar,
     Union,
 )
 
 from amqpstorm import Message
-from loguru import logger
-
 from amqpworker.easyqueue.connection import AMQPConnection
 from amqpworker.easyqueue.exceptions import UndecodableMessageException
 from amqpworker.easyqueue.message import AMQPMessage
 
 
 class DeliveryModes:
     NON_PERSISTENT = 1
@@ -258,23 +256,27 @@
         """
         :param data: A serializable data that should be serialized before
         publishing
         :param serialized_data: A payload to be published as is
         :param exchange: The exchange to publish the message
         :param routing_key: The routing key to publish the message
         """
+
         if data and serialized_data:
             raise ValueError("Only one of data or json should be specified")
 
         if data:
             if isinstance(data, (str, bytes)):
                 serialized_data = data
             else:
                 serialized_data = self.serialize(data, ensure_ascii=False)
-                properties['Content-Type'] = 'application/json'
+                if properties is None:
+                    properties = {'Content-Type': 'application/json'}
+                elif not properties.get('Content-Type'):
+                    properties['Content-Type'] = 'application/json'
 
         if not isinstance(serialized_data, bytes):
             serialized_data = serialized_data.encode()
 
         return self._write_connection.channel.basic.publish(
             body=serialized_data,
             exchange=exchange,
```

### Comparing `amqp_workers-0.1.0/amqpworker/entrypoints.py` & `amqp_workers-0.1.1/amqpworker/entrypoints.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.0/amqpworker/options.py` & `amqp_workers-0.1.1/amqpworker/options.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.0/amqpworker/rabbitmq/entrypoints.py` & `amqp_workers-0.1.1/amqpworker/rabbitmq/entrypoints.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.0/amqpworker/rabbitmq/message.py` & `amqp_workers-0.1.1/amqpworker/rabbitmq/message.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.0/amqpworker/routes.py` & `amqp_workers-0.1.1/amqpworker/routes.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.0/amqpworker/scheduled/__init__.py` & `amqp_workers-0.1.1/amqpworker/scheduled/__init__.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.0/amqpworker/signals/base.py` & `amqp_workers-0.1.1/amqpworker/signals/base.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.0/amqpworker/signals/handlers/rabbitmq.py` & `amqp_workers-0.1.1/amqpworker/signals/handlers/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.0/amqpworker/types/registry.py` & `amqp_workers-0.1.1/amqpworker/types/registry.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.0/amqpworker/typing/__init__.py` & `amqp_workers-0.1.1/amqpworker/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.0/LICENSE` & `amqp_workers-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `amqp_workers-0.1.0/pyproject.toml` & `amqp_workers-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 [tool.poetry]
 name = "amqp-workers"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["JimZhang <zzl22100048@gmail.com>"]
 readme = "README.md"
 packages = [{include = "amqpworker"}]
 repository = "https://git.loom.run/Coder/amqp-worker"
 keywords = ["amqp", "rabbitmq"]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.7"
 amqpstorm = {version = "^2.10.6", source = "douban"}
 pydantic = {version = "1.10.7", source = "douban"}
 loguru = {version = "^0.7.0", source = "douban"}
 cached-property = {version = "^1.5.2", source = "douban"}
 delayedqueue = {version = "^1.0.0", source = "douban"}
 
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3.1"
+pytest-mock = "^3.10.0"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 
 [[tool.poetry.source]]
 name = "douban"
 url = "https://mirror.baidu.com/pypi/simple"
+
+[tool.pytest.ini_options]
+minversion = "6.0"
+addopts = "-ra -q"
+testpaths = [
+    "tests",
+]
```

### Comparing `amqp_workers-0.1.0/README.md` & `amqp_workers-0.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,72 @@
 # 🐰amqp-worker
 
-amqp-worker 是一个基于 Python 的多线程 RabbitMQ 消费框架。它可以让你在消费消息时更加高效和稳定。
+English | [简体中文](https://git.loom.run/Coder/amqp-worker/src/branch/master/README_zh.md)
 
-## 功能特点
 
-- 批量消费：按批处理消息，提高消费效率。
-- 自动重连：当 RabbitMQ 服务断开连接时，amqp-worker 会自动重连，保证消费不中断。
-- 自定义消费模式：消费函数中自由决定使用多线程和协程。
-- 可配置的消息确认方式：支持自动确认和手动确认两种确认方式，根据你的消费需求进行配置。
-- 可配置的异常处理：支持全局配置消息异常的消费模式，重入队列、重新插入、消费消息。
+amqp-worker is a Python-based multi-threaded RabbitMQ consumer framework. It allows you to consume messages more efficiently and stably.
 
-## 安装方式
+## Features
 
-你可以使用 pip 工具来安装 amqp-worker:
+- Batch consumption: process messages in batches, improve consumption efficiency.
+- Automatic reconnection: when RabbitMQ service disconnects, amqp-worker will automatically reconnect, ensuring uninterrupted consumption.
+- Customizable consumption mode: freely decide to use multi-threading and coroutines in the consumption function.
+- Configurable message acknowledgment mode: support automatic acknowledgment and manual acknowledgment modes, configure according to your consumption needs.
+- Configurable exception handling: support global configuration of message exception consumption mode, re-enter queue, re-insert, consume message.
+
+## Installation
+
+You can use pip tool to install amqp-worker:
 
 ```
-pip install amqp-worker
+pip install amqp-workers
 ```
 
-## 使用方法
+## Usage
 
-首先，你需要在你的 Python 代码中引入 amqp_worker 模块：
+First, you need to import the amqp_worker module in your Python code:
 
 ```python
 from amqpworker.app import App
 ```
 
-然后，你需要实例化一个 App 对象，而App对象依赖AMQPConnection对象：
+Then, you need to instantiate an App object, and the App object depends on the AMQPConnection object:
 
 ```python
 from amqpworker.connections import AMQPConnection
 amqp_conn = AMQPConnection(hostname='127.0.0.1', username='guest', password='guest', port=5672)
 
 app = App(connections=[amqp_conn])
 ```
 
 
 
-接下来，你需要定义消费函数:
+Next, you need to define the consumption function:
 
 ```python
 @app.amqp.consume(
     ['test'],
     options=AMQPRouteOptions(bulk_size=1024 * 8, bulk_flush_interval=2)
 )
 def _handler(msgs: List[RabbitMQMessage]):
     print(f"Recv {len(msgs)} {datetime.now().isoformat()}")
 ```
 
 
-上面的代码中我们给消费函数一个装饰器，给出了消费的队列，每批消费的数量，值得注意的是，消费函数的参数类型为`List[RabbitMQMessage]`
+In the above code we give the consumption function a decorator, giving the consumption queue, the number of consumption per batch, it is worth noting that the parameter type of the consumption function is `List[RabbitMQMessage]`
 
-最后，只需要调用 `run` 方法即可开始消费：
+Finally, just call the `run` method to start consuming:
 
 ```python
 app.run()
 ```
 
-## 示例代码
+## Example code
 
-下面是一个简单的示例代码，它会消费名为 `test` 的队列中的消息：
+Below is a simple example code that will consume messages from a queue named `test`:
 
 ```python
 from datetime import datetime
 from typing import List
 
 from amqpworker.app import App
 from amqpworker.connections import AMQPConnection
@@ -80,14 +83,14 @@
 def _handler(msgs: List[RabbitMQMessage]):
     print(f"Recv {len(msgs)} {datetime.now().isoformat()}")
 
 app.run()
 
 ```
 
-## 贡献者
+## Contributors
 
 - [@JimZhang](https://git.loom.run/zzl221000)
 
-## 许可证
+## License
 
-amqp-worker 使用 MIT 许可证。详情请参阅 LICENSE 文件。
+amqp-worker uses MIT license. Please refer to LICENSE file for details.
```


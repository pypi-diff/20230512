# Comparing `tmp/aiormq-6.7.5.tar.gz` & `tmp/aiormq-6.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiormq-6.7.5.tar", max compression
+gzip compressed data, was "aiormq-6.7.6.tar", max compression
```

## Comparing `aiormq-6.7.5.tar` & `aiormq-6.7.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    17426 2023-02-18 21:26:40.811315 aiormq-6.7.5/README.rst
--rw-r--r--   0        0        0     1714 2022-12-15 11:27:13.176542 aiormq-6.7.5/aiormq/__init__.py
--rw-r--r--   0        0        0    17329 2023-05-11 09:07:24.799939 aiormq-6.7.5/aiormq/abc.py
--rw-r--r--   0        0        0      862 2022-12-12 22:30:18.703315 aiormq-6.7.5/aiormq/auth.py
--rw-r--r--   0        0        0     4800 2023-05-11 09:07:24.801438 aiormq-6.7.5/aiormq/base.py
--rw-r--r--   0        0        0    29505 2023-05-11 09:16:46.730769 aiormq-6.7.5/aiormq/channel.py
--rw-r--r--   0        0        0    29886 2023-05-11 11:26:19.689530 aiormq-6.7.5/aiormq/connection.py
--rw-r--r--   0        0        0     5831 2023-05-11 09:07:24.803621 aiormq-6.7.5/aiormq/exceptions.py
--rw-r--r--   0        0        0        0 2022-12-12 22:30:18.707721 aiormq-6.7.5/aiormq/py.typed
--rw-r--r--   0        0        0     3284 2023-05-11 09:07:24.804856 aiormq-6.7.5/aiormq/tools.py
--rw-r--r--   0        0        0      231 2023-05-11 09:07:24.805425 aiormq-6.7.5/aiormq/types.py
--rw-r--r--   0        0        0     2449 2023-05-11 11:26:19.690009 aiormq-6.7.5/pyproject.toml
--rw-r--r--   0        0        0    19407 1970-01-01 00:00:00.000000 aiormq-6.7.5/PKG-INFO
+-rw-r--r--   0        0        0    17426 2023-02-18 21:26:40.811315 aiormq-6.7.6/README.rst
+-rw-r--r--   0        0        0     1714 2022-12-15 11:27:13.176542 aiormq-6.7.6/aiormq/__init__.py
+-rw-r--r--   0        0        0    17329 2023-05-11 09:07:24.799939 aiormq-6.7.6/aiormq/abc.py
+-rw-r--r--   0        0        0      862 2022-12-12 22:30:18.703315 aiormq-6.7.6/aiormq/auth.py
+-rw-r--r--   0        0        0     4800 2023-05-11 09:07:24.801438 aiormq-6.7.6/aiormq/base.py
+-rw-r--r--   0        0        0    29505 2023-05-11 09:16:46.730769 aiormq-6.7.6/aiormq/channel.py
+-rw-r--r--   0        0        0    29929 2023-05-12 13:43:04.496203 aiormq-6.7.6/aiormq/connection.py
+-rw-r--r--   0        0        0     5831 2023-05-11 09:07:24.803621 aiormq-6.7.6/aiormq/exceptions.py
+-rw-r--r--   0        0        0        0 2022-12-12 22:30:18.707721 aiormq-6.7.6/aiormq/py.typed
+-rw-r--r--   0        0        0     3284 2023-05-11 09:07:24.804856 aiormq-6.7.6/aiormq/tools.py
+-rw-r--r--   0        0        0      231 2023-05-11 09:07:24.805425 aiormq-6.7.6/aiormq/types.py
+-rw-r--r--   0        0        0     2449 2023-05-12 13:43:13.645587 aiormq-6.7.6/pyproject.toml
+-rw-r--r--   0        0        0    19407 1970-01-01 00:00:00.000000 aiormq-6.7.6/PKG-INFO
```

### Comparing `aiormq-6.7.5/README.rst` & `aiormq-6.7.6/README.rst`

 * *Files identical despite different names*

### Comparing `aiormq-6.7.5/aiormq/__init__.py` & `aiormq-6.7.6/aiormq/__init__.py`

 * *Files identical despite different names*

### Comparing `aiormq-6.7.5/aiormq/abc.py` & `aiormq-6.7.6/aiormq/abc.py`

 * *Files identical despite different names*

### Comparing `aiormq-6.7.5/aiormq/auth.py` & `aiormq-6.7.6/aiormq/auth.py`

 * *Files identical despite different names*

### Comparing `aiormq-6.7.5/aiormq/base.py` & `aiormq-6.7.6/aiormq/base.py`

 * *Files identical despite different names*

### Comparing `aiormq-6.7.5/aiormq/channel.py` & `aiormq-6.7.6/aiormq/channel.py`

 * *Files identical despite different names*

### Comparing `aiormq-6.7.5/aiormq/connection.py` & `aiormq-6.7.6/aiormq/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -608,15 +608,16 @@
 
     async def __reader(self, frame_receiver: FrameReceiver) -> None:
         self.__connection_unblocked.set()
         self.connected.set()
 
         # Not very optimal, but avoid creating a task for each frame sending
         # noinspection PyAsyncCall
-        self.create_task(self.__heartbeat())
+        if self.heartbeat_timeout > 0:
+            self.create_task(self.__heartbeat())
 
         channel_frame_handlers: Mapping[Any, Callable[[Any], Awaitable[None]]]
         channel_frame_handlers = {
             spec.Connection.CloseOk: self.__handle_close_ok,
             spec.Connection.Close: self.__handle_close,
             Heartbeat: self.__handle_heartbeat,
             spec.Channel.CloseOk: self.__handle_channel_close_ok,
```

### Comparing `aiormq-6.7.5/aiormq/exceptions.py` & `aiormq-6.7.6/aiormq/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiormq-6.7.5/aiormq/tools.py` & `aiormq-6.7.6/aiormq/tools.py`

 * *Files identical despite different names*

### Comparing `aiormq-6.7.5/pyproject.toml` & `aiormq-6.7.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiormq"
-version = "6.7.5"
+version = "6.7.6"
 description = "Pure python AMQP asynchronous client library"
 authors = ["Dmitry Orlov <me@mosquito.su>"]
 readme = "README.rst"
 license = "Apache-2.0"
 keywords=["rabbitmq", "asyncio", "amqp", "amqp 0.9.1", "driver", "pamqp"]
 homepage = "https://github.com/mosquito/aiormq"
 classifiers = [
```

### Comparing `aiormq-6.7.5/PKG-INFO` & `aiormq-6.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiormq
-Version: 6.7.5
+Version: 6.7.6
 Summary: Pure python AMQP asynchronous client library
 Home-page: https://github.com/mosquito/aiormq
 License: Apache-2.0
 Keywords: rabbitmq,asyncio,amqp,amqp 0.9.1,driver,pamqp
 Author: Dmitry Orlov
 Author-email: me@mosquito.su
 Requires-Python: >=3.7,<4.0
```


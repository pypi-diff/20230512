# Comparing `tmp/foxglove-websocket-0.0.9.tar.gz` & `tmp/foxglove-websocket-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxglove-websocket-0.0.9.tar", last modified: Wed Jan 11 19:28:00 2023, max compression
+gzip compressed data, was "foxglove-websocket-0.1.0.tar", last modified: Fri May 12 16:01:53 2023, max compression
```

## Comparing `foxglove-websocket-0.0.9.tar` & `foxglove-websocket-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:28:00.869877 foxglove-websocket-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-01-11 19:28:00.869877 foxglove-websocket-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-01-11 19:27:25.000000 foxglove-websocket-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-01-11 19:27:25.000000 foxglove-websocket-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-01-11 19:28:00.869877 foxglove-websocket-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:28:00.865877 foxglove-websocket-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:28:00.865877 foxglove-websocket-0.0.9/src/foxglove_websocket/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-01-11 19:27:25.000000 foxglove-websocket-0.0.9/src/foxglove_websocket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:28:00.869877 foxglove-websocket-0.0.9/src/foxglove_websocket/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 19:27:25.000000 foxglove-websocket-0.0.9/src/foxglove_websocket/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-01-11 19:27:25.000000 foxglove-websocket-0.0.9/src/foxglove_websocket/examples/json_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-01-11 19:27:25.000000 foxglove-websocket-0.0.9/src/foxglove_websocket/examples/protobuf_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:28:00.869877 foxglove-websocket-0.0.9/src/foxglove_websocket/server/
--rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-01-11 19:27:25.000000 foxglove-websocket-0.0.9/src/foxglove_websocket/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-01-11 19:27:25.000000 foxglove-websocket-0.0.9/src/foxglove_websocket/server/client_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-01-11 19:27:25.000000 foxglove-websocket-0.0.9/src/foxglove_websocket/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 19:28:00.865877 foxglove-websocket-0.0.9/src/foxglove_websocket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-01-11 19:28:00.000000 foxglove-websocket-0.0.9/src/foxglove_websocket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-01-11 19:28:00.000000 foxglove-websocket-0.0.9/src/foxglove_websocket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 19:28:00.000000 foxglove-websocket-0.0.9/src/foxglove_websocket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 19:27:39.000000 foxglove-websocket-0.0.9/src/foxglove_websocket.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-01-11 19:28:00.000000 foxglove-websocket-0.0.9/src/foxglove_websocket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-11 19:28:00.000000 foxglove-websocket-0.0.9/src/foxglove_websocket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:53.301074 foxglove-websocket-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-12 16:01:53.301074 foxglove-websocket-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-12 16:01:17.000000 foxglove-websocket-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-12 16:01:17.000000 foxglove-websocket-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-12 16:01:53.305074 foxglove-websocket-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:53.289074 foxglove-websocket-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:53.293074 foxglove-websocket-0.1.0/src/foxglove_websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-12 16:01:17.000000 foxglove-websocket-0.1.0/src/foxglove_websocket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:53.301074 foxglove-websocket-0.1.0/src/foxglove_websocket/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:17.000000 foxglove-websocket-0.1.0/src/foxglove_websocket/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-12 16:01:17.000000 foxglove-websocket-0.1.0/src/foxglove_websocket/examples/json_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-12 16:01:17.000000 foxglove-websocket-0.1.0/src/foxglove_websocket/examples/param_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-12 16:01:17.000000 foxglove-websocket-0.1.0/src/foxglove_websocket/examples/protobuf_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:53.301074 foxglove-websocket-0.1.0/src/foxglove_websocket/server/
+-rw-r--r--   0 runner    (1001) docker     (123)    24188 2023-05-12 16:01:17.000000 foxglove-websocket-0.1.0/src/foxglove_websocket/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-12 16:01:17.000000 foxglove-websocket-0.1.0/src/foxglove_websocket/server/client_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-12 16:01:17.000000 foxglove-websocket-0.1.0/src/foxglove_websocket/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:53.297074 foxglove-websocket-0.1.0/src/foxglove_websocket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-12 16:01:53.000000 foxglove-websocket-0.1.0/src/foxglove_websocket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-12 16:01:53.000000 foxglove-websocket-0.1.0/src/foxglove_websocket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 16:01:53.000000 foxglove-websocket-0.1.0/src/foxglove_websocket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 16:01:32.000000 foxglove-websocket-0.1.0/src/foxglove_websocket.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-12 16:01:53.000000 foxglove-websocket-0.1.0/src/foxglove_websocket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-12 16:01:53.000000 foxglove-websocket-0.1.0/src/foxglove_websocket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:53.301074 foxglove-websocket-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-12 16:01:17.000000 foxglove-websocket-0.1.0/tests/test_client_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16057 2023-05-12 16:01:17.000000 foxglove-websocket-0.1.0/tests/test_server.py
```

### Comparing `foxglove-websocket-0.0.9/PKG-INFO` & `foxglove-websocket-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-websocket
-Version: 0.0.9
+Version: 0.1.0
 Summary: Foxglove WebSocket server
 Home-page: https://github.com/foxglove/ws-protocol
 License: MIT
 Project-URL: GitHub Issues, https://github.com/foxglove/ws-protocol/issues
 Project-URL: Foxglove Studio Documentation, https://foxglove.dev/docs
 Keywords: foxglove,websocket,robotics,ros,ros2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `foxglove-websocket-0.0.9/README.md` & `foxglove-websocket-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `foxglove-websocket-0.0.9/setup.cfg` & `foxglove-websocket-0.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = foxglove-websocket
-version = 0.0.9
+version = 0.1.0
 description = Foxglove WebSocket server
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = foxglove, websocket, robotics, ros, ros2
 license = MIT
 url = https://github.com/foxglove/ws-protocol
 project_urls =
```

### Comparing `foxglove-websocket-0.0.9/src/foxglove_websocket/__init__.py` & `foxglove-websocket-0.1.0/src/foxglove_websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `foxglove-websocket-0.0.9/src/foxglove_websocket/examples/protobuf_server.py` & `foxglove-websocket-0.1.0/src/foxglove_websocket/examples/protobuf_server.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,30 +45,31 @@
 
     append_file_descriptor(message_class.DESCRIPTOR.file)
     return file_descriptor_set
 
 
 async def main():
     class Listener(FoxgloveServerListener):
-        def on_subscribe(self, server: FoxgloveServer, channel_id: ChannelId):
+        async def on_subscribe(self, server: FoxgloveServer, channel_id: ChannelId):
             print("First client subscribed to", channel_id)
 
-        def on_unsubscribe(self, server: FoxgloveServer, channel_id: ChannelId):
+        async def on_unsubscribe(self, server: FoxgloveServer, channel_id: ChannelId):
             print("Last client unsubscribed from", channel_id)
 
     async with FoxgloveServer("0.0.0.0", 8765, "example server") as server:
         server.set_listener(Listener())
         chan_id = await server.add_channel(
             {
                 "topic": "example_msg",
                 "encoding": "protobuf",
                 "schemaName": SceneUpdate.DESCRIPTOR.full_name,
                 "schema": b64encode(
                     build_file_descriptor_set(SceneUpdate).SerializeToString()
                 ).decode("ascii"),
+                "schemaEncoding": "protobuf",
             }
         )
 
         i = 0
         while True:
             i += 1
             await asyncio.sleep(0.05)
```

### Comparing `foxglove-websocket-0.0.9/src/foxglove_websocket/server/client_state.py` & `foxglove-websocket-0.1.0/src/foxglove_websocket/server/client_state.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from types import MappingProxyType
-from typing import Optional, Iterable
+from typing import Optional, Set
 from dataclasses import field
 from websockets.server import WebSocketServerProtocol
 from dataclasses import dataclass
 
-from ..types import ChannelId, SubscriptionId
+from ..types import ChannelId, ClientChannel, ClientChannelId, SubscriptionId
 
 
 @dataclass
 class ClientState:
     """
     ClientState holds information about subscriptions from a given client, used by the server for
     bookkeeping. The `subscriptions` and `subscriptions_by_channel` are immutable, which makes them
@@ -16,21 +16,25 @@
     iteration.
     """
 
     connection: WebSocketServerProtocol
     subscriptions: "MappingProxyType[SubscriptionId, ChannelId]" = field(
         default_factory=lambda: MappingProxyType({})
     )
-    subscriptions_by_channel: "MappingProxyType[ChannelId, Iterable[SubscriptionId]]" = field(
+    subscriptions_by_channel: "MappingProxyType[ChannelId, SubscriptionId]" = field(
         default_factory=lambda: MappingProxyType({})
     )
+    advertisements_by_channel: "MappingProxyType[ClientChannelId, ClientChannel]" = (
+        field(default_factory=lambda: MappingProxyType({}))
+    )
+    subscribed_params: Set[str] = field(default_factory=lambda: set([]))
 
     def remove_channel(self, removed_chan_id: ChannelId):
-        subs = self.subscriptions_by_channel.get(removed_chan_id)
-        if subs is not None:
+        sub_id = self.subscriptions_by_channel.get(removed_chan_id)
+        if sub_id is not None:
             self.subscriptions = MappingProxyType(
                 {
                     sub: chan
                     for sub, chan in self.subscriptions.items()
                     if chan != removed_chan_id
                 }
             )
@@ -38,22 +42,26 @@
                 {
                     chan: subs
                     for chan, subs in self.subscriptions_by_channel.items()
                     if chan != removed_chan_id
                 }
             )
 
-    def add_subscription(self, sub_id: SubscriptionId, chan_id: ChannelId):
+    def add_subscription(self, sub_id: SubscriptionId, chan_id: ChannelId) -> bool:
+        if chan_id in self.subscriptions_by_channel:
+            return False
+
         self.subscriptions = MappingProxyType({**self.subscriptions, sub_id: chan_id})
         self.subscriptions_by_channel = MappingProxyType(
             {
                 **self.subscriptions_by_channel,
-                chan_id: {*self.subscriptions_by_channel.get(chan_id, ()), sub_id},
+                chan_id: sub_id,
             }
         )
+        return True
 
     def remove_subscription(
         self, removed_sub_id: SubscriptionId
     ) -> Optional[ChannelId]:
         chan_id = self.subscriptions.get(removed_sub_id)
         if chan_id is None:
             return None
@@ -65,17 +73,35 @@
             }
         )
         new_subscriptions_by_channel = {
             chan: subs
             for chan, subs in self.subscriptions_by_channel.items()
             if chan != chan_id
         }
-        new_subs = {
-            sub_id
-            for sub_id in self.subscriptions_by_channel.get(chan_id, ())
-            if sub_id != removed_sub_id
-        }
-        if new_subs:
-            new_subscriptions_by_channel[chan_id] = new_subs
         self.subscriptions_by_channel = MappingProxyType(new_subscriptions_by_channel)
 
         return chan_id
+
+    def add_client_channel(self, channel: ClientChannel) -> bool:
+        if channel["id"] in self.advertisements_by_channel:
+            return False
+
+        self.advertisements_by_channel = MappingProxyType(
+            {
+                **self.advertisements_by_channel,
+                channel["id"]: channel,
+            }
+        )
+        return True
+
+    def remove_client_channel(self, channel_id: ClientChannelId) -> bool:
+        if channel_id not in self.advertisements_by_channel:
+            return False
+
+        self.advertisements_by_channel = MappingProxyType(
+            {
+                chan: subs
+                for chan, subs in self.advertisements_by_channel.items()
+                if chan != channel_id
+            }
+        )
+        return True
```

### Comparing `foxglove-websocket-0.0.9/src/foxglove_websocket.egg-info/PKG-INFO` & `foxglove-websocket-0.1.0/src/foxglove_websocket.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-websocket
-Version: 0.0.9
+Version: 0.1.0
 Summary: Foxglove WebSocket server
 Home-page: https://github.com/foxglove/ws-protocol
 License: MIT
 Project-URL: GitHub Issues, https://github.com/foxglove/ws-protocol/issues
 Project-URL: Foxglove Studio Documentation, https://foxglove.dev/docs
 Keywords: foxglove,websocket,robotics,ros,ros2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `foxglove-websocket-0.0.9/src/foxglove_websocket.egg-info/SOURCES.txt` & `foxglove-websocket-0.1.0/src/foxglove_websocket.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,10 +7,13 @@
 src/foxglove_websocket.egg-info/SOURCES.txt
 src/foxglove_websocket.egg-info/dependency_links.txt
 src/foxglove_websocket.egg-info/not-zip-safe
 src/foxglove_websocket.egg-info/requires.txt
 src/foxglove_websocket.egg-info/top_level.txt
 src/foxglove_websocket/examples/__init__.py
 src/foxglove_websocket/examples/json_server.py
+src/foxglove_websocket/examples/param_server.py
 src/foxglove_websocket/examples/protobuf_server.py
 src/foxglove_websocket/server/__init__.py
-src/foxglove_websocket/server/client_state.py
+src/foxglove_websocket/server/client_state.py
+tests/test_client_state.py
+tests/test_server.py
```


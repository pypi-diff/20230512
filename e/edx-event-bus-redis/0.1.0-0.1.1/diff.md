# Comparing `tmp/edx_event_bus_redis-0.1.0.tar.gz` & `tmp/edx_event_bus_redis-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx_event_bus_redis-0.1.0.tar", last modified: Thu May  4 14:13:00 2023, max compression
+gzip compressed data, was "edx_event_bus_redis-0.1.1.tar", last modified: Fri May 12 13:15:22 2023, max compression
```

## Comparing `edx_event_bus_redis-0.1.0.tar` & `edx_event_bus_redis-0.1.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 14:13:00.222676 edx_event_bus_redis-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)      647 2023-05-04 14:12:55.000000 edx_event_bus_redis-0.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-04 14:12:55.000000 edx_event_bus_redis-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-05-04 14:12:55.000000 edx_event_bus_redis-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7935 2023-05-04 14:13:00.222676 edx_event_bus_redis-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6583 2023-05-04 14:12:55.000000 edx_event_bus_redis-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 14:13:00.218676 edx_event_bus_redis-0.1.0/edx_event_bus_redis/
--rw-r--r--   0 runner    (1001) docker     (122)      328 2023-05-04 14:12:55.000000 edx_event_bus_redis-0.1.0/edx_event_bus_redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-05-04 14:12:55.000000 edx_event_bus_redis-0.1.0/edx_event_bus_redis/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 14:13:00.218676 edx_event_bus_redis-0.1.0/edx_event_bus_redis/internal/
--rw-r--r--   0 runner    (1001) docker     (122)      245 2023-05-04 14:12:55.000000 edx_event_bus_redis-0.1.0/edx_event_bus_redis/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1791 2023-05-04 14:12:55.000000 edx_event_bus_redis-0.1.0/edx_event_bus_redis/internal/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    20197 2023-05-04 14:12:55.000000 edx_event_bus_redis-0.1.0/edx_event_bus_redis/internal/consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2195 2023-05-04 14:12:55.000000 edx_event_bus_redis-0.1.0/edx_event_bus_redis/internal/message.py
--rw-r--r--   0 runner    (1001) docker     (122)     5365 2023-05-04 14:12:55.000000 edx_event_bus_redis-0.1.0/edx_event_bus_redis/internal/producer.py
--rw-r--r--   0 runner    (1001) docker     (122)     4485 2023-05-04 14:12:55.000000 edx_event_bus_redis-0.1.0/edx_event_bus_redis/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 14:13:00.218676 edx_event_bus_redis-0.1.0/edx_event_bus_redis/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 14:12:55.000000 edx_event_bus_redis-0.1.0/edx_event_bus_redis/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 14:13:00.222676 edx_event_bus_redis-0.1.0/edx_event_bus_redis/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-04 14:12:55.000000 edx_event_bus_redis-0.1.0/edx_event_bus_redis/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-05-04 14:12:55.000000 edx_event_bus_redis-0.1.0/edx_event_bus_redis/management/commands/produce_event.py
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-04 14:12:55.000000 edx_event_bus_redis-0.1.0/edx_event_bus_redis/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 14:13:00.218676 edx_event_bus_redis-0.1.0/edx_event_bus_redis/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 14:13:00.222676 edx_event_bus_redis-0.1.0/edx_event_bus_redis/templates/edx_event_bus_redis/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-04 14:12:55.000000 edx_event_bus_redis-0.1.0/edx_event_bus_redis/templates/edx_event_bus_redis/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-05-04 14:12:55.000000 edx_event_bus_redis-0.1.0/edx_event_bus_redis/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 14:13:00.218676 edx_event_bus_redis-0.1.0/edx_event_bus_redis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7935 2023-05-04 14:13:00.000000 edx_event_bus_redis-0.1.0/edx_event_bus_redis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      964 2023-05-04 14:13:00.000000 edx_event_bus_redis-0.1.0/edx_event_bus_redis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 14:13:00.000000 edx_event_bus_redis-0.1.0/edx_event_bus_redis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 14:13:00.000000 edx_event_bus_redis-0.1.0/edx_event_bus_redis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-05-04 14:13:00.000000 edx_event_bus_redis-0.1.0/edx_event_bus_redis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-04 14:13:00.000000 edx_event_bus_redis-0.1.0/edx_event_bus_redis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 14:13:00.222676 edx_event_bus_redis-0.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-04 14:12:55.000000 edx_event_bus_redis-0.1.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-04 14:12:55.000000 edx_event_bus_redis-0.1.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-04 14:13:00.222676 edx_event_bus_redis-0.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5113 2023-05-04 14:12:55.000000 edx_event_bus_redis-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 14:13:00.222676 edx_event_bus_redis-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      250 2023-05-04 14:12:55.000000 edx_event_bus_redis-0.1.0/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:15:22.533420 edx_event_bus_redis-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      908 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8196 2023-05-12 13:15:22.533420 edx_event_bus_redis-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6583 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:15:22.529420 edx_event_bus_redis-0.1.1/edx_event_bus_redis/
+-rw-r--r--   0 runner    (1001) docker     (122)      328 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:15:22.529420 edx_event_bus_redis-0.1.1/edx_event_bus_redis/internal/
+-rw-r--r--   0 runner    (1001) docker     (122)      245 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1791 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/internal/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20908 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/internal/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2195 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/internal/message.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5365 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/internal/producer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4485 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:15:22.529420 edx_event_bus_redis-0.1.1/edx_event_bus_redis/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:15:22.529420 edx_event_bus_redis-0.1.1/edx_event_bus_redis/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/management/commands/produce_event.py
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:15:22.525420 edx_event_bus_redis-0.1.1/edx_event_bus_redis/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:15:22.529420 edx_event_bus_redis-0.1.1/edx_event_bus_redis/templates/edx_event_bus_redis/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/templates/edx_event_bus_redis/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:15:22.529420 edx_event_bus_redis-0.1.1/edx_event_bus_redis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8196 2023-05-12 13:15:22.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      964 2023-05-12 13:15:22.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-12 13:15:22.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-12 13:15:22.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-05-12 13:15:22.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-12 13:15:22.000000 edx_event_bus_redis-0.1.1/edx_event_bus_redis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:15:22.533420 edx_event_bus_redis-0.1.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-12 13:15:22.533420 edx_event_bus_redis-0.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5113 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:15:22.533420 edx_event_bus_redis-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      250 2023-05-12 13:15:17.000000 edx_event_bus_redis-0.1.1/tests/test_models.py
```

### Comparing `edx_event_bus_redis-0.1.0/CHANGELOG.rst` & `edx_event_bus_redis-0.1.1/CHANGELOG.rst`

 * *Files 26% similar despite different names*

```diff
@@ -12,14 +12,27 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+[0.1.1] - 2023-05-12
+************************************************
+
+Added
+=====
+
+* Option to claim messages from other consumers based on idle time.
+
+Changed
+=======
+
+* Setting ``check_backlog`` will read messages that were not read by this consumer group.
+
 [0.1.0] - 2023-05-04
 ************************************************
 
 Added
 =====
 
 * First release on PyPI.
```

### Comparing `edx_event_bus_redis-0.1.0/LICENSE.txt` & `edx_event_bus_redis-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.1.0/PKG-INFO` & `edx_event_bus_redis-0.1.1/edx_event_bus_redis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: edx_event_bus_redis
-Version: 0.1.0
+Name: edx-event-bus-redis
+Version: 0.1.1
 Summary: Redis Streams implementation for the Open edX event bus.
 Home-page: https://github.com/openedx/event-bus-redis
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -236,14 +236,27 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+[0.1.1] - 2023-05-12
+************************************************
+
+Added
+=====
+
+* Option to claim messages from other consumers based on idle time.
+
+Changed
+=======
+
+* Setting ``check_backlog`` will read messages that were not read by this consumer group.
+
 [0.1.0] - 2023-05-04
 ************************************************
 
 Added
 =====
 
 * First release on PyPI.
```

### Comparing `edx_event_bus_redis-0.1.0/README.rst` & `edx_event_bus_redis-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.1.0/edx_event_bus_redis/internal/config.py` & `edx_event_bus_redis-0.1.1/edx_event_bus_redis/internal/config.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.1.0/edx_event_bus_redis/internal/consumer.py` & `edx_event_bus_redis-0.1.1/edx_event_bus_redis/internal/consumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 # .. toggle_description: If set to False, consumer will exit immediately. This can be used as an emergency kill-switch
 #   to disable a consumer—as long as the management command is killed and restarted when settings change.
 # .. toggle_use_cases: opt_out
 # .. toggle_creation_date: 2022-01-31
 REDIS_CONSUMERS_ENABLED = SettingToggle('EVENT_BUS_REDIS_CONSUMERS_ENABLED', default=True)
 
 # .. setting_name: EVENT_BUS_REDIS_CONSUMER_POLL_TIMEOUT
-# .. setting_default: 1.0
+# .. setting_default: 1
 # .. setting_description: How long the consumer should wait, in seconds, for the Redis broker
 #   to respond to a poll() call.
 CONSUMER_POLL_TIMEOUT = getattr(settings, 'EVENT_BUS_REDIS_CONSUMER_POLL_TIMEOUT', 1)
 
 # .. setting_name: EVENT_BUS_REDIS_CONSUMER_POLL_FAILURE_SLEEP
 # .. setting_default: 1.0
 # .. setting_description: When the consumer fails to retrieve an event from the broker,
@@ -89,26 +89,33 @@
     Attributes:
         topic: Topic/stream name.
         group_id: consumer group name.
         signal: openedx_events signal.
         consumer_name: unique name for consumer within a group.
         last_read_msg_id: Start reading msgs from a specific redis msg id.
         check_backlog: flag to process all messages that were not read by this consumer group.
+        claim_msgs_older_than: claim pending msgs from other consumers in the group with idle time older
+            than a specific time (in milliseconds).
+        has_pending_msgs: flag to process pending msgs first.
         db: Walrus object for redis connection.
         full_topic: topic prefixed with environment name.
         consumer: consumer instance.
     """
 
-    def __init__(self, topic, group_id, signal, consumer_name, last_read_msg_id=None, check_backlog=False):
+    def __init__(self, topic, group_id, signal, consumer_name, last_read_msg_id=None, check_backlog=False,
+                 claim_msgs_older_than=None):
         self.topic = topic
         self.group_id = group_id
         self.signal = signal
         self.consumer_name = consumer_name
         self.last_read_msg_id = last_read_msg_id
         self.check_backlog = check_backlog
+        # always process read but pending msgs first for the consumer in the group.
+        self.has_pending_msgs = True
+        self.claim_msgs_older_than = claim_msgs_older_than
         self.db = self._create_db()
         self.full_topic = get_full_topic(self.topic)
         self.consumer = self._create_consumer(self.db, self.full_topic)
         self._shut_down_loop = False
 
     def _create_db(self) -> Database:
         """
@@ -146,23 +153,24 @@
         """
         Test utility for shutting down the consumer loop.
         """
         self._shut_down_loop = True
 
     def _read_pending_msgs(self) -> Optional[tuple]:
         """
-        Read pending messages, if no messages found set check_backlog to False.
+        Read pending messages, if no messages found return None.
         """
         logger.debug("Consuming pending msgs first.")
+        if self.claim_msgs_older_than is not None:
+            self.consumer.autoclaim(self.consumer_name, min_idle_time=self.claim_msgs_older_than, count=1)
         msg_meta = self.consumer.pending(count=1, consumer=self.consumer_name)
-        if not msg_meta:
-            logger.debug("No more pending messages.")
-            self.check_backlog = False
-            return None
-        return self.consumer[msg_meta[0]['message_id']]
+        if msg_meta:
+            return self.consumer[msg_meta[0]['message_id']]
+        logger.debug("No more pending messages.")
+        return None
 
     def _consume_indefinitely(self):
         """
         Consume events from a topic in an infinite loop.
         """
 
         if not REDIS_CONSUMERS_ENABLED.is_enabled():
@@ -211,16 +219,19 @@
                     )
 
                 redis_raw_msg = None
                 msg: Optional[RedisMessage] = None
                 try:
                     # The first time we want to read our pending messages, in case we crashed and are recovering.
                     # Once we consumed our history, we can start getting new messages.
-                    if self.check_backlog:
+                    if self.has_pending_msgs:
                         redis_raw_msg = self._read_pending_msgs()
+                        if redis_raw_msg is None:
+                            self.has_pending_msgs = False
+                            self.claim_msgs_older_than = None
                     else:
                         # poll for msg
                         redis_raw_msg = self.consumer.read(count=1, block=CONSUMER_POLL_TIMEOUT * 1000)
                     if redis_raw_msg:
                         if isinstance(redis_raw_msg, list):
                             redis_raw_msg = redis_raw_msg[0]
                         msg = RedisMessage.parse(redis_raw_msg, self.full_topic, expected_signal=self.signal)
```

### Comparing `edx_event_bus_redis-0.1.0/edx_event_bus_redis/internal/message.py` & `edx_event_bus_redis-0.1.1/edx_event_bus_redis/internal/message.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.1.0/edx_event_bus_redis/internal/producer.py` & `edx_event_bus_redis-0.1.1/edx_event_bus_redis/internal/producer.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.1.0/edx_event_bus_redis/internal/utils.py` & `edx_event_bus_redis-0.1.1/edx_event_bus_redis/internal/utils.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.1.0/edx_event_bus_redis/management/commands/produce_event.py` & `edx_event_bus_redis-0.1.1/edx_event_bus_redis/management/commands/produce_event.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.1.0/edx_event_bus_redis/templates/edx_event_bus_redis/base.html` & `edx_event_bus_redis-0.1.1/edx_event_bus_redis/templates/edx_event_bus_redis/base.html`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.1.0/edx_event_bus_redis.egg-info/PKG-INFO` & `edx_event_bus_redis-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: edx-event-bus-redis
-Version: 0.1.0
+Name: edx_event_bus_redis
+Version: 0.1.1
 Summary: Redis Streams implementation for the Open edX event bus.
 Home-page: https://github.com/openedx/event-bus-redis
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -236,14 +236,27 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+[0.1.1] - 2023-05-12
+************************************************
+
+Added
+=====
+
+* Option to claim messages from other consumers based on idle time.
+
+Changed
+=======
+
+* Setting ``check_backlog`` will read messages that were not read by this consumer group.
+
 [0.1.0] - 2023-05-04
 ************************************************
 
 Added
 =====
 
 * First release on PyPI.
```

### Comparing `edx_event_bus_redis-0.1.0/edx_event_bus_redis.egg-info/SOURCES.txt` & `edx_event_bus_redis-0.1.1/edx_event_bus_redis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.1.0/requirements/constraints.txt` & `edx_event_bus_redis-0.1.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.1.0/setup.py` & `edx_event_bus_redis-0.1.1/setup.py`

 * *Files identical despite different names*


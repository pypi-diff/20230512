# Comparing `tmp/ja2mqtt-1.0.5.tar.gz` & `tmp/ja2mqtt-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ja2mqtt-1.0.5.tar", last modified: Sun May  7 12:39:57 2023, max compression
+gzip compressed data, was "dist/ja2mqtt-1.0.6.tar", last modified: Fri May 12 20:29:23 2023, max compression
```

## Comparing `ja2mqtt-1.0.5.tar` & `ja2mqtt-1.0.6.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/README-pypi.text
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/ja2mqtt/
--rwxr-xr-x   0 runner    (1001) docker     (123)      167 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/ja2mqtt/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/commands/ja2mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/commands/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/ja2mqtt/components/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/components/bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/components/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/components/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/components/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15810 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/ja2mqtt/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/schemas/config-schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/schemas/ja2mqtt-schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/ja2mqtt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/ja2mqtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/ja2mqtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/ja2mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/ja2mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/ja2mqtt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/ja2mqtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/ja2mqtt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 12:39:57.000000 ja2mqtt-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-07 12:39:34.000000 ja2mqtt-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:29:23.000000 ja2mqtt-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-12 20:29:04.000000 ja2mqtt-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-12 20:29:23.000000 ja2mqtt-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-12 20:29:04.000000 ja2mqtt-1.0.6/README-pypi.text
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-12 20:29:04.000000 ja2mqtt-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:29:23.000000 ja2mqtt-1.0.6/ja2mqtt/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      167 2023-05-12 20:29:04.000000 ja2mqtt-1.0.6/ja2mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-12 20:29:04.000000 ja2mqtt-1.0.6/ja2mqtt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:29:23.000000 ja2mqtt-1.0.6/ja2mqtt/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-12 20:29:04.000000 ja2mqtt-1.0.6/ja2mqtt/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-12 20:29:04.000000 ja2mqtt-1.0.6/ja2mqtt/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-12 20:29:04.000000 ja2mqtt-1.0.6/ja2mqtt/commands/ja2mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-05-12 20:29:04.000000 ja2mqtt-1.0.6/ja2mqtt/commands/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-12 20:29:04.000000 ja2mqtt-1.0.6/ja2mqtt/commands/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:29:23.000000 ja2mqtt-1.0.6/ja2mqtt/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-12 20:29:04.000000 ja2mqtt-1.0.6/ja2mqtt/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14947 2023-05-12 20:29:04.000000 ja2mqtt-1.0.6/ja2mqtt/components/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-12 20:29:04.000000 ja2mqtt-1.0.6/ja2mqtt/components/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-05-12 20:29:04.000000 ja2mqtt-1.0.6/ja2mqtt/components/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-05-12 20:29:04.000000 ja2mqtt-1.0.6/ja2mqtt/components/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-12 20:29:04.000000 ja2mqtt-1.0.6/ja2mqtt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-05-12 20:29:04.000000 ja2mqtt-1.0.6/ja2mqtt/json2table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:29:23.000000 ja2mqtt-1.0.6/ja2mqtt/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-12 20:29:04.000000 ja2mqtt-1.0.6/ja2mqtt/schemas/config-schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-12 20:29:04.000000 ja2mqtt-1.0.6/ja2mqtt/schemas/ja2mqtt-schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-05-12 20:29:04.000000 ja2mqtt-1.0.6/ja2mqtt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:29:23.000000 ja2mqtt-1.0.6/ja2mqtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-12 20:29:23.000000 ja2mqtt-1.0.6/ja2mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-12 20:29:23.000000 ja2mqtt-1.0.6/ja2mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:29:23.000000 ja2mqtt-1.0.6/ja2mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-12 20:29:23.000000 ja2mqtt-1.0.6/ja2mqtt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-12 20:29:23.000000 ja2mqtt-1.0.6/ja2mqtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-12 20:29:23.000000 ja2mqtt-1.0.6/ja2mqtt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 20:29:23.000000 ja2mqtt-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-12 20:29:04.000000 ja2mqtt-1.0.6/setup.py
```

### Comparing `ja2mqtt-1.0.5/PKG-INFO` & `ja2mqtt-1.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ja2mqtt
-Version: 1.0.5
+Version: 1.0.6
 Summary: Jablotron MQTT bridge
 Home-page: UNKNOWN
 Author: Tomas Vitvar
 Author-email: tomas@vitvar.com
 License: UNKNOWN
 Description: ja2mqtt is a bridge that connects a Jablotron control unit, extended with the [JA-121T RS-485 bus interface](https://www.jablotron.com/en/produkt/rs-485-bus-interface-426/), to an MQTT broker.
```

### Comparing `ja2mqtt-1.0.5/README-pypi.text` & `ja2mqtt-1.0.6/README-pypi.text`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.5/README.md` & `ja2mqtt-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.5/ja2mqtt/commands/__init__.py` & `ja2mqtt-1.0.6/ja2mqtt/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.5/ja2mqtt/commands/config.py` & `ja2mqtt-1.0.6/ja2mqtt/commands/config.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.5/ja2mqtt/commands/ja2mqtt.py` & `ja2mqtt-1.0.6/ja2mqtt/commands/ja2mqtt.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import click
 
 import ja2mqtt.config as ja2mqtt_config
 from ja2mqtt import __version__
 from ja2mqtt.commands.config import command_config
 from ja2mqtt.commands.run import command_run
-from ja2mqtt.commands.test import command_publish
+from ja2mqtt.commands.query import command_publish, command_states
 from ja2mqtt.utils import bcolors, format_str_color
 
 
 class CoreCommand(click.core.Group):
     def invoke(self, ctx):
         ja2mqtt_config.ANSI_COLORS = not ctx.params.get("no-ansi", False)
         ja2mqtt_config.DEBUG = ctx.params.get("debug", False)
@@ -53,7 +53,8 @@
 def ja2mqtt(debug, no_ansi):
     pass
 
 
 ja2mqtt.add_command(command_run)
 ja2mqtt.add_command(command_config)
 ja2mqtt.add_command(command_publish)
+ja2mqtt.add_command(command_states)
```

### Comparing `ja2mqtt-1.0.5/ja2mqtt/commands/run.py` & `ja2mqtt-1.0.6/ja2mqtt/commands/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 @click.command("run", help="Run command.", cls=BaseCommand)
 def command_run(config, log):
     bridge = SerialMQTTBridge(config)
 
     simulator = None
     if config("simulator") is not None:
         simulator = Simulator(config.get_part("simulator"), bridge.prfstate_bits)
-    elif config("serial.use_simulator", False):
+    elif config("serial.use_simulator", True):
         log.error(
-            "The serial interface is be simulated but the simulator configuration does not exist!"
+            "The serial interface is set to be simulated but the simulator configuration does not exist!"
         )
 
     serial = Serial(config.get_part("serial"), simulator)
     mqtt = MQTT(f"ja2mqtt-client+{randomString(10)}", config.get_part("mqtt-broker"))
 
     bridge.set_mqtt(mqtt)
     bridge.set_serial(serial)
```

### Comparing `ja2mqtt-1.0.5/ja2mqtt/components/__init__.py` & `ja2mqtt-1.0.6/ja2mqtt/components/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,11 +24,11 @@
     def start(self, exit_event):
         self.thread = threading.Thread(
             target=self.worker, args=(exit_event,), daemon=True
         )
         self.thread.start()
 
 
-from .bridge import SerialMQTTBridge
+from .bridge import SerialMQTTBridge, JA2MQTTConfig
 from .mqtt import MQTT
 from .serial import Serial
 from .simulator import Simulator
```

### Comparing `ja2mqtt-1.0.5/ja2mqtt/components/bridge.py` & `ja2mqtt-1.0.6/ja2mqtt/components/bridge.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,19 +9,28 @@
 import threading
 import time
 from queue import Empty, Queue
 
 import paho.mqtt.client as mqtt
 
 from ja2mqtt.config import Config
-from ja2mqtt.utils import Map, PythonExpression, deep_eval, deep_merge, merge_dicts
+from ja2mqtt.utils import (
+    Map,
+    PythonExpression,
+    deep_eval,
+    deep_merge,
+    merge_dicts,
+    randomString,
+)
 
 from . import Component
 from .serial import SerialJA121TException, decode_prfstate
 
+PRFSTATE_RE = re.compile("PRFSTATE ([0-9A-F]+)")
+
 
 class Pattern:
     """
     Pattern class is used in the scope to evaluate that a data string matches the pattern
     defined in the ja2mqtt rule. It is possible to use the equal operator to compare the data string
     with the pattern object and then use the matcher to retrieve captured groups
     for the `wrtie` condition of the rule.
@@ -37,37 +46,110 @@
 
     def __eq__(self, other):
         self.match = self.re.match(other)
         return self.match is not None
 
 
 class PrfStateChange:
-    def __init__(self, pos, current_prfstate):
+    """
+    PrfStateChange evaluates a state change in a peripheral at position `pos`. It uses
+    the current state object that represents decoded peripheral states (a result of
+    `decode_prfstate`) and compares a new decoded state with the curent state at
+    a position `pos`. If the state changes, the `__eq__` method returns True otherwise
+    it returns False. After the evaluation of equality, the property `state` contains
+    the current state of the peripheral and property `updated` contains the updated
+    time of the peripheral.
+    """
+
+    def __init__(self, pos, current_state):
         self.pos = pos
-        self.current_prfstate = current_prfstate
+        self.current_state = current_state
         self.state = None
+        self.updated = None
 
     def __str__(self):
-        return f"position={self.pos}, state={self.state}"
+        """
+        String representation of the oject.
+        """
+        return f"pos={self.pos}, state={self.state}"
+
+    def decode(self, line):
+        """
+        Decode line to dict where keys are codes and values are states.
+        """
+        if line.startswith("PRFSTATE"):
+            d = decode_prfstate(line.split(" ")[1])
+            return True, d
+        else:
+            return False, None
 
     def __eq__(self, other):
-        if other.startswith("PRFSTATE"):
-            d = decode_prfstate(other.split(" ")[1])
+        res, d = self.decode(other)
+        if res:
+            if self.state != d[self.pos]:
+                self.updated = time.time()
             self.state = d[self.pos]
-            return (
-                self.current_prfstate is None
-                or d[self.pos] != self.current_prfstate[self.pos]
+            res = (
+                self.current_state is None
+                or d[self.pos] != self.current_state[self.pos]
             )
+        return res
+
+
+class SectionState:
+    def __init__(self, pattern, section_group=1, state_group=2):
+        self.re = re.compile(pattern)
+        self.section_group = section_group
+        self.state_group = state_group
+        self.state = None
+        self.match = None
+        self.updated = None
+
+    def __eq__(self, other):
+        self.match = self.re.match(other)
+        if self.match:
+            section = self.match.group(self.section_group)
+            state = self.match.group(self.state_group)
+            if self.state != state:
+                self.updated = time.time()
+                self.state = state
+            return True
         else:
             return False
 
 
+class PrfState:
+    def __init__(self, pos):
+        self.state = None
+        self.pos = str(pos)
+        self.report_on_next = False
+
+    def __eq__(self, other):
+        res = False
+        if other.startswith("PRFSTATE"):
+            d = decode_prfstate(other.split(" ")[1])
+            if self.state != d[self.pos]:
+                self.state = d[self.pos]
+                self.updated = time.time()
+                res = True
+            if self.report_on_next:
+                self.report_on_next = False
+                res = True
+        return res
+
+
 class Topic:
-    def __init__(self, topic):
-        self.name = topic["name"]
+    def __init__(self, prefix, topic):
+        if topic["name"].startswith(prefix):
+            self.name = topic["name"]
+        else:
+            sep = "/"
+            if prefix[-1] == "/" or topic["name"][0] == "/":
+                sep = ""
+            self.name = prefix + sep + topic["name"]
         self.disabled = topic.get("disabled", False)
         self.rules = []
         for rule_def in topic["rules"]:
             self.rules.append(Map(rule_def))
 
     def check_rule_data(self, read, data, scope, path=None):
         if path is None:
@@ -92,50 +174,112 @@
                             raise Exception(
                                 f"Invalid value of property {'.'.join(path)}, "
                                 + f"found: {data[k]}, exepcted: {v}"
                             )
         except Exception as e:
             raise Exception(f"Topic data validation failed. {str(e)}")
 
+    @classmethod
+    def list(cls, topics):
+        return ", ".join(
+            [x.name + ("" if not x.disabled else " (disabled)") for x in topics]
+        )
+
 
-class SerialMQTTBridge(Component):
+class JA2MQTTConfig:
     def __init__(self, config):
-        def _list(topics):
-            return ", ".join(
-                [x.name + ("" if not x.disabled else " (disabled)") for x in topics]
+        self._scope = None
+        self.config = config
+        self.topics_serial2mqtt = []
+        self.topics_mqtt2serial = []
+        self.ja2mqtt_file = self.config.get_dir_path(config.root("ja2mqtt"))
+        self.ja2mqtt = Config(
+            self.ja2mqtt_file,
+            scope=self.scope(),
+            use_template=True,
+            schema="ja2mqtt-schema.yaml",
+        )
+
+        # system properties
+        self.topic_prefix = self.ja2mqtt("system.topic_prefix", "ja2mqtt")
+        self.correlation_id = self.ja2mqtt("system.correlation_id", None)
+        self.correlation_timeout = self.ja2mqtt("system.correlation_timeout", 0)
+        self.topic_sys_error = self.ja2mqtt("system.topic_sys_error", None)
+        self.prfstate_bits = self.ja2mqtt("system.prfstate_bits", 128)
+
+        # topics
+        for topic_def in self.ja2mqtt("serial2mqtt"):
+            self.topics_serial2mqtt.append(Topic(self.topic_prefix, topic_def))
+        for topic_def in self.ja2mqtt("mqtt2serial"):
+            self.topics_mqtt2serial.append(Topic(self.topic_prefix, topic_def))
+
+    def scope(self):
+        section_states = {}
+
+        def _section_state(pattern, g1, g2):
+            if pattern not in section_states:
+                section_states[pattern] = SectionState(pattern, g1, g2)
+            return section_states[pattern]
+
+        prf_states = {}
+
+        def _prf_state(pos):
+            if pos not in prf_states:
+                prf_states[pos] = PrfState(pos)
+            return prf_states[pos]
+
+        def _write_prf_state():
+            for k, v in prf_states.items():
+                v.report_on_next = True
+            return "PRFSTATE"
+
+        if self._scope is None:
+            self._scope = Map(
+                topology=self.config.root("topology"),
+                pattern=lambda x: Pattern(x),
+                format=lambda x, **kwa: x.format(**kwa),
+                prf_state=lambda pos: _prf_state(pos),
+                section_state=lambda pattern, g1, g2: _section_state(pattern, g1, g2),
+                write_prf_state=_write_prf_state,
             )
+        return self._scope
 
-        super().__init__(config, "bridge")
+    def corr_id(self):
+        corrid_field = self.ja2mqtt("system.correlation_id", None)
+        corr_id = randomString(12, letters="abcdef0123456789")
+        return corrid_field, corr_id if corrid_field is not None else None
+
+    def topic_exists(self, name):
+        return name in [x.name for x in self.topics_mqtt2serial]
+
+
+class SerialMQTTBridge(Component, JA2MQTTConfig):
+    def __init__(self, config):
+        Component.__init__(self, config, "bridge")
+        JA2MQTTConfig.__init__(self, config)
         self.mqtt = None
         self.serial = None
-        self.topics_serial2mqtt = []
-        self.topics_mqtt2serial = []
         self._scope = None
         self.request_queue = Queue()
-
-        ja2mqtt_file = self.config.get_dir_path(config.root("ja2mqtt"))
-        ja2mqtt = Config(ja2mqtt_file, scope=self.scope(), use_template=True)
-        for topic_def in ja2mqtt("serial2mqtt"):
-            self.topics_serial2mqtt.append(Topic(topic_def))
-        for topic_def in ja2mqtt("mqtt2serial"):
-            self.topics_mqtt2serial.append(Topic(topic_def))
-        self.correlation_id = ja2mqtt("system.correlation_id", None)
-        self.correlation_timeout = ja2mqtt("system.correlation_timeout", 0)
-        self.topic_sys_error = ja2mqtt("system.topic_sys_error", None)
-        self.prfstate_bits = ja2mqtt("system.prfstate_bits", 128)
         self.request = None
-        self.prfstate = [decode_prfstate("".zfill(self.prfstate_bits))]
 
-        self.log.info(f"The ja2mqtt definition file is {ja2mqtt_file}")
+        self.log.info(f"The ja2mqtt definition file is {self.ja2mqtt_file}")
         self.log.info(
             f"There are {len(self.topics_serial2mqtt)} serial2mqtt and "
             + f"{len(self.topics_mqtt2serial)} mqtt2serial topics."
         )
-        self.log.debug(f"The serial2mqtt topics are: {_list(self.topics_serial2mqtt)}")
-        self.log.debug(f"The mqtt2serial topics are: {_list(self.topics_mqtt2serial)}")
+        self.log.debug(
+            f"The serial2mqtt topics are: {Topic.list(self.topics_serial2mqtt)}"
+        )
+        self.log.debug(
+            f"The mqtt2serial topics are: {Topic.list(self.topics_mqtt2serial)}"
+        )
+
+        # states of perihperals
+        self.prfstate = [decode_prfstate("".zfill(self.prfstate_bits))]
 
     def update_correlation(self, data):
         if self.request_queue.qsize() > 0:
             self.request = self.request_queue.get()
         if self.request is not None:
             if (
                 time.time() - self.request.created_time < self.correlation_timeout
@@ -148,46 +292,28 @@
                 self.log.debug(
                     "Discarding the request for correlation. The correlation timeout "
                     + "or TTL expired."
                 )
                 self.request = None
         return data
 
-    def scope(self):
-        def _write_prf_state(reset=False):
-            if reset:
-                self.log.debug("Reseting prfstate object to None.")
-                self.prfstate = []
-            return "PRFSTATE"
-
-        if self._scope is None:
-            self._scope = Map(
-                topology=self.config.root("topology"),
-                pattern=lambda x: Pattern(x),
-                format=lambda x, **kwa: x.format(**kwa),
-                prf_state_change=lambda pos: PrfStateChange(
-                    str(pos), self.prfstate[-2] if len(self.prfstate) > 1 else None
-                ),
-                write_prf_state=_write_prf_state,
-            )
-        return self._scope
-
     def update_scope(self, key, value=None, remove=False):
         if self._scope is None:
             self.scope()
         if not remove:
             self._scope[key] = value
         else:
             if key in self._scope:
                 del self._scope[key]
 
     def update_prfstate(self, data_str):
         try:
-            if data_str.startswith("PRFSTATE"):
-                self.prfstate.append(decode_prfstate(data_str.split(" ")[1]))
+            m = PRFSTATE_RE.match(data_str)
+            if m:
+                self.prfstate.append(decode_prfstate(m.group(1)))
                 if len(self.prfstate) > 1:
                     self.prfstate = self.prfstate[-2:]
                 self.log.debug(f"prfstate_decoded={self.prfstate[-1]}")
         except SerialJA121TException as e:
             self.log.error({str(e)})
 
     def on_mqtt_connect(self, client, userdata, flags, rc):
```

### Comparing `ja2mqtt-1.0.5/ja2mqtt/components/mqtt.py` & `ja2mqtt-1.0.6/ja2mqtt/components/mqtt.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
         self.reconnect_after = self.config.value_int("reconnect_after", default=30)
         self.loop_timeout = self.config.value_int("loop_timeout", default=1)
         self.username = self.config.value_str("username", default=None)
         self.password = self.config.value_str("password", default=None)
         self.protocol = {
             "MQTTv311": mqtt.MQTTv311,
             "MQTTv31": mqtt.MQTTv31,
-            "MQTTv5": mqtt.MQTTv5,
             "default": None,
         }[self.config.value_str("protocol", default="MQTTv311")]
         self.transport = self.config.value_str("transport", default="tcp")
         self.clean_session = self.config.value_str("clean_session", default=None)
         self.client = None
         self.connected = False
         self.on_connect_ext = None
```

### Comparing `ja2mqtt-1.0.5/ja2mqtt/components/serial.py` & `ja2mqtt-1.0.6/ja2mqtt/components/serial.py`

 * *Files 12% similar despite different names*

```diff
@@ -83,14 +83,18 @@
         and creates `ser` object that can be either `PySerial` or `Simulator` based on the
         `use_simulator` property in the configuration.
         """
         super().__init__(config, "serial")
         self.buffer = Queue()
         self.wait_on_ready = self.config.value_int("wait_on_ready", default=10)
         self.use_simulator = self.config.value_bool("use_simulator", default=False)
+        self.minimum_write_delay = self.config.value_int(
+            "minimum_write_delay", default=1
+        )
+        self.last_write_time = None
         if not self.use_simulator:
             self.ser = None
             self.port = self.config.value_str("port", required=True)
             self.log.info(f"The serial connection configured, the port is {self.port}")
         else:
             self.port = "<simulator>"
             self.ser = simulator
@@ -156,15 +160,27 @@
     def writeline(self, line):
         """
         Write a single line of string to the seiral port. It convers the string to bytes using
         the defined `encoding` and adds a LF at the end.
         """
         self.log.debug(f"Writing to serial: {line}")
         try:
+            current_time = time.time()
+            # wait the minimum_write_delay
+            if (
+                self.last_write_time is not None
+                and current_time - self.last_write_time < self.minimum_write_delay
+            ):
+                waiting_time = self.minimum_write_delay - (
+                    current_time - self.last_write_time
+                )
+                self.log.debug(f"Too frequent writes, waiting {waiting_time}.")
+                time.sleep(waiting_time)
             self.ser.write(bytes(line + "\n", ENCODING))
+            self.last_write_time = time.time()
         except Exception as e:
             self.log.error(str(e))
 
     def worker(self, exit_event):
         """
         The main worker of the serial object that reads data from the serial port and
         puts them to the queue `buffer`. Althoguh the `worker` method (that only reads
```

### Comparing `ja2mqtt-1.0.5/ja2mqtt/components/simulator.py` & `ja2mqtt-1.0.6/ja2mqtt/components/simulator.py`

 * *Files 11% similar despite different names*

```diff
@@ -79,19 +79,19 @@
 
     def open(self, exit_event):
         pass
 
     def close(self):
         pass
 
-    def generate_prfstate(self, on_prob=0.5):
-        return {
-            str(p): ("ON" if random.random() < on_prob else "OFF")
-            for p in self.peripherals
-        }
+    def generate_prfstate(self, *pos, on_prob=0.5):
+        _pos = self.peripherals
+        if len(pos) > 0:
+            _pos = list(pos)
+        return {str(p): ("ON" if random.random() < on_prob else "OFF") for p in _pos}
 
     def _add_to_buffer(self, data):
         time.sleep(self.response_delay)
         self.buffer.put(data)
 
     def write(self, data):
         def _match(pattern, data_str):
@@ -160,15 +160,15 @@
         except Empty:
             return b""
 
     def scope(self):
         from .serial import encode_prfstate
 
         def _prf_random_states(*pos, on_prob=0.5):
-            prf = self.generate_prfstate(on_prob)
+            prf = self.generate_prfstate(*pos, on_prob=on_prob)
             return "PRFSTATE " + encode_prfstate(prf, self.prfstate_bits)
 
         return Map(
             random=lambda a, b: a + round(random.random() * b),
             prf_random_states=_prf_random_states,
         )
```

### Comparing `ja2mqtt-1.0.5/ja2mqtt/config.py` & `ja2mqtt-1.0.6/ja2mqtt/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -462,21 +462,7 @@
                     "handlers": log_handlers,
                     "level": f"{log_level}",
                     "propagate": False,
                 }
             },
         }
     )
-
-
-def ja2mqtt_def(config):
-    return Config(
-        config.get_dir_path(config.root("ja2mqtt")),
-        scope=Map(topology=config.root("topology")),
-        use_template=True,
-    )
-
-
-def correlation_id(ja2mqtt):
-    corrid_field = ja2mqtt("system.correlation_id", None)
-    corr_id = randomString(12, letters="abcdef0123456789")
-    return corrid_field, corr_id if corrid_field is not None else None
```

### Comparing `ja2mqtt-1.0.5/ja2mqtt/schemas/config-schema.yaml` & `ja2mqtt-1.0.6/ja2mqtt/schemas/config-schema.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,17 @@
         enum:
           - 1
           - 2
       rtscts:
         type: "boolean"
       xonxoff:
         type: "boolean"
+      minimum_write_delay:
+        type: "number"
+        minimum: 0
 
   # Jablotron topology
   topology:
     type: "object"
     required:
       - section
     additionalProperties: False
@@ -151,14 +154,17 @@
               enum:
                 - "ARMED"
                 - "READY"
                 - "OFF"
       response_delay:
         type: "number"
         minimum: 0
+      peripherals:
+        type: "string"
+        pattern: "^[0-9]+(,[0-9]+)*$"
       rules:
         type: "array"
         items:
           type: "object"
           required:
             - "time_next"
             - "write"
```

### Comparing `ja2mqtt-1.0.5/ja2mqtt/schemas/ja2mqtt-schema.yaml` & `ja2mqtt-1.0.6/ja2mqtt/schemas/ja2mqtt-schema.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
         type: "number"
         minimum: 0
         maximum: 60
       prfstate_bits:
         type: "integer"
         minimum: 8
         maximum: 128
+      topic_prefix:
+        type: "string"
   serial2mqtt:
     type: "array"
     items:
       type: "object"
       additionalProperties: False
       required:
         - "name"
```

### Comparing `ja2mqtt-1.0.5/ja2mqtt/utils.py` & `ja2mqtt-1.0.6/ja2mqtt/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import random
 import re
 import string
 import threading
 import time
 from functools import reduce
+import json
 
 
 class bcolors:
     HEADER = "\033[95m"
     OKBLUE = "\033[94m"
     OKGREEN = "\033[32m"
     WARNING = "\033[33m"
```

### Comparing `ja2mqtt-1.0.5/ja2mqtt.egg-info/PKG-INFO` & `ja2mqtt-1.0.6/ja2mqtt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ja2mqtt
-Version: 1.0.5
+Version: 1.0.6
 Summary: Jablotron MQTT bridge
 Home-page: UNKNOWN
 Author: Tomas Vitvar
 Author-email: tomas@vitvar.com
 License: UNKNOWN
 Description: ja2mqtt is a bridge that connects a Jablotron control unit, extended with the [JA-121T RS-485 bus interface](https://www.jablotron.com/en/produkt/rs-485-bus-interface-426/), to an MQTT broker.
```

### Comparing `ja2mqtt-1.0.5/ja2mqtt.egg-info/SOURCES.txt` & `ja2mqtt-1.0.6/ja2mqtt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 MANIFEST.in
 README-pypi.text
 README.md
 setup.py
 ja2mqtt/__init__.py
 ja2mqtt/__main__.py
 ja2mqtt/config.py
+ja2mqtt/json2table.py
 ja2mqtt/utils.py
 ja2mqtt.egg-info/PKG-INFO
 ja2mqtt.egg-info/SOURCES.txt
 ja2mqtt.egg-info/dependency_links.txt
 ja2mqtt.egg-info/entry_points.txt
 ja2mqtt.egg-info/requires.txt
 ja2mqtt.egg-info/top_level.txt
 ja2mqtt/commands/__init__.py
 ja2mqtt/commands/config.py
 ja2mqtt/commands/ja2mqtt.py
+ja2mqtt/commands/query.py
 ja2mqtt/commands/run.py
-ja2mqtt/commands/test.py
 ja2mqtt/components/__init__.py
 ja2mqtt/components/bridge.py
 ja2mqtt/components/mqtt.py
 ja2mqtt/components/serial.py
 ja2mqtt/components/simulator.py
 ja2mqtt/schemas/config-schema.yaml
 ja2mqtt/schemas/ja2mqtt-schema.yaml
```

### Comparing `ja2mqtt-1.0.5/setup.py` & `ja2mqtt-1.0.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,30 +30,30 @@
 # required modules
 install_requires = [
     'click>=8.0.4',
     'Jinja2>=3.0.3',
     'paho-mqtt>=1.6.1',
     'pyserial>=3.5',
     'PyYAML>=6.0',
-    'jsonschema>=4.0.0'
+    'jsonschema>=4.0.0',
+    'pytz>=2023.3'
 ]
 
 setup(
     name='ja2mqtt',
     version=__version__,
     description='Jablotron MQTT bridge',
     long_description=read('README-pypi.text'),
     py_modules=['ja2mqtt'],
     author='Tomas Vitvar',
     author_email='tomas@vitvar.com',
     packages=find_packages(exclude=['tests.*', 'tests']),
     include_package_data=True,
     install_requires=install_requires,
     python_requires='>=3.6.0',
-    #scripts=['bin/ja2mqtt'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3.7',
     ],
     entry_points='''
```


# Comparing `tmp/nanolab-0.0.4.tar.gz` & `tmp/nanolab-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanolab-0.0.4.tar", last modified: Wed May 10 19:38:38 2023, max compression
+gzip compressed data, was "nanolab-0.0.5.tar", last modified: Fri May 12 12:49:29 2023, max compression
```

## Comparing `nanolab-0.0.4.tar` & `nanolab-0.0.5.tar`

### file list

```diff
@@ -1,47 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:38:38.279958 nanolab-0.0.4/
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-07 22:25:09.000000 nanolab-0.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1567 2023-05-10 19:38:38.279958 nanolab-0.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1371 2023-05-09 13:33:33.000000 nanolab-0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:38:38.275958 nanolab-0.0.4/nanolab/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 20:58:11.000000 nanolab-0.0.4/nanolab/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:38:38.275958 nanolab-0.0.4/nanolab/command/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 08:00:48.000000 nanolab-0.0.4/nanolab/command/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1202 2023-05-10 19:36:27.000000 nanolab-0.0.4/nanolab/command/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:38:38.275958 nanolab-0.0.4/nanolab/command/mixins/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 13:06:25.000000 nanolab-0.0.4/nanolab/command/mixins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-05-07 19:39:25.000000 nanolab-0.0.4/nanolab/command/mixins/base_mixin.py
--rw-r--r--   0 root         (0) root         (0)      839 2023-05-09 15:37:47.000000 nanolab-0.0.4/nanolab/command/mixins/bash_command_mixin.py
--rw-r--r--   0 root         (0) root         (0)     1589 2023-05-07 19:31:15.000000 nanolab-0.0.4/nanolab/command/mixins/python_command_mixin.py
--rw-r--r--   0 root         (0) root         (0)     2270 2023-05-10 19:36:27.000000 nanolab-0.0.4/nanolab/command/mixins/threaded_command_mixin.py
--rw-r--r--   0 root         (0) root         (0)      598 2023-04-26 22:11:20.000000 nanolab-0.0.4/nanolab/decorators.py
--rwxr-xr-x   0 root         (0) root         (0)      459 2023-05-09 11:04:51.000000 nanolab-0.0.4/nanolab/main.py
--rw-r--r--   0 root         (0) root         (0)    11028 2023-05-08 09:50:05.000000 nanolab-0.0.4/nanolab/node_interaction.py
--rw-r--r--   0 root         (0) root         (0)     6715 2023-05-09 20:51:58.000000 nanolab-0.0.4/nanolab/node_tools.py
--rw-r--r--   0 root         (0) root         (0)     1038 2023-05-10 19:34:06.000000 nanolab-0.0.4/nanolab/pycmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:38:38.275958 nanolab-0.0.4/nanolab/snippets/
--rw-r--r--   0 root         (0) root         (0)     2318 2023-05-09 15:33:56.000000 nanolab-0.0.4/nanolab/snippets/default_snips.json
--rw-r--r--   0 root         (0) root         (0)     1834 2023-05-10 19:36:27.000000 nanolab-0.0.4/nanolab/snippets/test_snippets.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:38:38.275958 nanolab-0.0.4/nanolab/src/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 06:56:43.000000 nanolab-0.0.4/nanolab/src/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3788 2023-05-10 19:36:27.000000 nanolab-0.0.4/nanolab/src/argparse_commands.py
--rw-r--r--   0 root         (0) root         (0)     4899 2023-05-10 19:36:27.000000 nanolab-0.0.4/nanolab/src/config_handler.py
--rw-r--r--   0 root         (0) root         (0)     5148 2023-05-10 19:36:27.000000 nanolab-0.0.4/nanolab/src/config_loader.py
--rw-r--r--   0 root         (0) root         (0)     1365 2023-05-08 12:45:36.000000 nanolab-0.0.4/nanolab/src/github.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-05-08 19:55:35.000000 nanolab-0.0.4/nanolab/src/resolver.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-05-10 13:22:47.000000 nanolab-0.0.4/nanolab/src/snippet_manager.py
--rw-r--r--   0 root         (0) root         (0)     2815 2023-05-10 19:36:27.000000 nanolab-0.0.4/nanolab/src/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:38:38.279958 nanolab-0.0.4/nanolab/xnomin/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 21:19:13.000000 nanolab-0.0.4/nanolab/xnomin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1688 2023-04-24 21:16:18.000000 nanolab-0.0.4/nanolab/xnomin/acctools.py
--rw-r--r--   0 root         (0) root         (0)     7345 2023-05-04 22:16:30.000000 nanolab-0.0.4/nanolab/xnomin/handshake.py
--rw-r--r--   0 root         (0) root         (0)    18867 2023-05-04 22:16:30.000000 nanolab-0.0.4/nanolab/xnomin/peers.py
--rwxr-xr-x   0 root         (0) root         (0)     2424 2023-05-10 19:36:27.000000 nanolab-0.0.4/nanolab/xnomin/telemetry_req.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:38:38.275958 nanolab-0.0.4/nanolab.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1567 2023-05-10 19:38:38.000000 nanolab-0.0.4/nanolab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1035 2023-05-10 19:38:38.000000 nanolab-0.0.4/nanolab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 19:38:38.000000 nanolab-0.0.4/nanolab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-10 19:38:38.000000 nanolab-0.0.4/nanolab.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-10 19:38:38.000000 nanolab-0.0.4/nanolab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-10 19:38:38.000000 nanolab-0.0.4/nanolab.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 19:38:38.279958 nanolab-0.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      627 2023-05-10 19:38:31.000000 nanolab-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:49:29.383990 nanolab-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-07 22:25:09.000000 nanolab-0.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-05-12 12:49:29.383990 nanolab-0.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1371 2023-05-09 13:33:33.000000 nanolab-0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:49:29.379990 nanolab-0.0.5/nanolab/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-10 19:38:38.000000 nanolab-0.0.5/nanolab/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:49:29.379990 nanolab-0.0.5/nanolab/command/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 08:00:48.000000 nanolab-0.0.5/nanolab/command/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1212 2023-05-10 21:50:30.000000 nanolab-0.0.5/nanolab/command/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:49:29.379990 nanolab-0.0.5/nanolab/command/mixins/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 13:06:25.000000 nanolab-0.0.5/nanolab/command/mixins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-05-10 21:50:04.000000 nanolab-0.0.5/nanolab/command/mixins/base_mixin.py
+-rw-r--r--   0 root         (0) root         (0)      839 2023-05-10 21:47:56.000000 nanolab-0.0.5/nanolab/command/mixins/bash_command_mixin.py
+-rw-r--r--   0 root         (0) root         (0)     1589 2023-05-10 21:48:04.000000 nanolab-0.0.5/nanolab/command/mixins/python_command_mixin.py
+-rw-r--r--   0 root         (0) root         (0)     3111 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/command/mixins/threaded_command_mixin.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:49:29.379990 nanolab-0.0.5/nanolab/loggers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/builders.py
+-rw-r--r--   0 root         (0) root         (0)      638 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/contracts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:49:29.379990 nanolab-0.0.5/nanolab/loggers/factories/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/factories/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/factories/logger_factory.py
+-rw-r--r--   0 root         (0) root         (0)      568 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/factories/sink_factory.py
+-rw-r--r--   0 root         (0) root         (0)     2141 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/logger_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:49:29.379990 nanolab-0.0.5/nanolab/loggers/sinks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/sinks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      920 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/sinks/console_sink.py
+-rw-r--r--   0 root         (0) root         (0)      997 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/sinks/csv_sink.py
+-rw-r--r--   0 root         (0) root         (0)     3689 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/sinks/sql_sink.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:49:29.379990 nanolab-0.0.5/nanolab/loggers/sources/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/sources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4283 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/sources/rpc_logger.py
+-rwxr-xr-x   0 root         (0) root         (0)      459 2023-05-09 11:04:51.000000 nanolab-0.0.5/nanolab/main.py
+-rw-r--r--   0 root         (0) root         (0)     8896 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/node_interaction.py
+-rw-r--r--   0 root         (0) root         (0)     6715 2023-05-09 20:51:58.000000 nanolab-0.0.5/nanolab/node_tools.py
+-rw-r--r--   0 root         (0) root         (0)      755 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/pycmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:49:29.379990 nanolab-0.0.5/nanolab/snippets/
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-05-09 15:33:56.000000 nanolab-0.0.5/nanolab/snippets/default_snips.json
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-05-10 19:36:27.000000 nanolab-0.0.5/nanolab/snippets/test_snippets.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:49:29.383990 nanolab-0.0.5/nanolab/src/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 06:56:43.000000 nanolab-0.0.5/nanolab/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3788 2023-05-10 19:36:27.000000 nanolab-0.0.5/nanolab/src/argparse_commands.py
+-rw-r--r--   0 root         (0) root         (0)     4898 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/src/config_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5148 2023-05-10 19:36:27.000000 nanolab-0.0.5/nanolab/src/config_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1365 2023-05-08 12:45:36.000000 nanolab-0.0.5/nanolab/src/github.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-05-08 19:55:35.000000 nanolab-0.0.5/nanolab/src/resolver.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-05-10 13:22:47.000000 nanolab-0.0.5/nanolab/src/snippet_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2815 2023-05-10 19:36:27.000000 nanolab-0.0.5/nanolab/src/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:49:29.383990 nanolab-0.0.5/nanolab/xnomin/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 21:19:13.000000 nanolab-0.0.5/nanolab/xnomin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-04-24 21:16:18.000000 nanolab-0.0.5/nanolab/xnomin/acctools.py
+-rw-r--r--   0 root         (0) root         (0)     7345 2023-05-04 22:16:30.000000 nanolab-0.0.5/nanolab/xnomin/handshake.py
+-rw-r--r--   0 root         (0) root         (0)    18867 2023-05-04 22:16:30.000000 nanolab-0.0.5/nanolab/xnomin/peers.py
+-rwxr-xr-x   0 root         (0) root         (0)     2424 2023-05-10 19:36:27.000000 nanolab-0.0.5/nanolab/xnomin/telemetry_req.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:49:29.379990 nanolab-0.0.5/nanolab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-05-12 12:49:29.000000 nanolab-0.0.5/nanolab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1492 2023-05-12 12:49:29.000000 nanolab-0.0.5/nanolab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 12:49:29.000000 nanolab-0.0.5/nanolab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-12 12:49:29.000000 nanolab-0.0.5/nanolab.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-12 12:49:29.000000 nanolab-0.0.5/nanolab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-12 12:49:29.000000 nanolab-0.0.5/nanolab.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 12:49:29.383990 nanolab-0.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      641 2023-05-12 12:49:17.000000 nanolab-0.0.5/setup.py
```

### Comparing `nanolab-0.0.4/PKG-INFO` & `nanolab-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanolab
-Version: 0.0.4
+Version: 0.0.5
 Summary: testing tool using nanomock
 Home-page: https://github.com/gr0vity-dev/nanolab
 Author: gr0vity
 Description-Content-Type: text/markdown
 
 ##NanoLab
```

### Comparing `nanolab-0.0.4/README.md` & `nanolab-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.4/nanolab/command/command.py` & `nanolab-0.0.5/nanolab/command/command.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         pass
 
     @abstractmethod
     def execute(self):
         pass
 
 
-class Command:
+class Command(ICommand):
 
     def __init__(self, command_config: dict):
         self.command_config = command_config
         self.mixins = {
             'bash': BashCommandMixin,
             'python': PythonCommandMixin,
             'threaded': ThreadedCommandMixin
```

### Comparing `nanolab-0.0.4/nanolab/command/mixins/base_mixin.py` & `nanolab-0.0.5/nanolab/command/mixins/base_mixin.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.4/nanolab/command/mixins/bash_command_mixin.py` & `nanolab-0.0.5/nanolab/command/mixins/bash_command_mixin.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.4/nanolab/command/mixins/python_command_mixin.py` & `nanolab-0.0.5/nanolab/command/mixins/python_command_mixin.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.4/nanolab/decorators.py` & `nanolab-0.0.5/nanolab/decorators.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,8 +20,18 @@
             if remaining_time > 0:
                 await asyncio.sleep(remaining_time)
 
             return result
 
         return wrapper
 
-    return decorator
+    return decorator
+
+
+def print_dot(func):
+
+    def wrapper(*args, **kwargs):
+        result = func(*args, **kwargs)
+        print('.', end='', flush=True)
+        return result
+
+    return wrapper
```

### Comparing `nanolab-0.0.4/nanolab/node_interaction.py` & `nanolab-0.0.5/nanolab/node_interaction.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,90 +7,34 @@
 from nanolab.src.utils import get_config_parser
 from typing import Any, Dict, List
 import asyncio
 import random
 import time
 import itertools
 
+from nanolab.loggers.logger_handler import LoggerHandler
+
 
 def load_nodes_config():
     """Load nodes configuration from a file."""
     return get_config_parser().get_nodes_config()
 
 
-async def create_logger(node, logger_type, hashes, logger_timeout,
-                        logger_expected_count):
+async def start_loggers(logger_type, sink_type, logger_params: dict):
+    logger_handler = LoggerHandler(load_nodes_config(), logger_params)
+    await logger_handler.start_logging(logger_type, sink_type)
+
 
-    nanorpc = NanoRpc(node["rpc_url"])
-    node_version = nanorpc.version()
-    formatted_node_version = f'{node_version["node_vendor"]} {node_version["build_info"][0:7]}'
-    start_block_count = nanorpc.block_count()
-
-    logger = StatsLogger(logger_type,
-                         node["name"],
-                         formatted_node_version,
-                         hashes,
-                         start_block_count,
-                         timeout=logger_timeout,
-                         expected_block_count=logger_expected_count,
-                         ws_url=node["ws_url"],
-                         rpc_url=node["rpc_url"])
-    return logger
-
-
-#Allow some time, to ensure StatsLoggers are correctly initialized before blocks are published by any thread
-@ensure_duration(duration=2)
-async def create_loggers(hashes,
-                         logger_type=None,
-                         logger_timeout=None,
-                         included_peers=None,
-                         excluded_peers=None,
-                         logger_expected_count=None):
-
-    if not logger_type: return []
-    nodes_config = load_nodes_config()
-    tasks = []
-    for node in nodes_config:
-        if included_peers and node["name"] not in included_peers:
-            continue
-        if excluded_peers and node["name"] in excluded_peers:
-            continue
-        tasks.append(
-            create_logger(node, logger_type, hashes, logger_timeout,
-                          logger_expected_count))
-
-    loggers = await asyncio.gather(*tasks)
-    return loggers
-
-
-async def start_loggers(loggers):
-    logger_tasks = [asyncio.create_task(logger.start()) for logger in loggers]
-    await asyncio.gather(*logger_tasks)
-
-
-async def xnolib_publish(params: dict,
-                         logger_type=None,
-                         logger_timeout=None,
-                         included_peers=None,
-                         excluded_peers=None,
-                         logger_expected_count=None):
+async def xnolib_publish(params: dict):
 
     block_lists = get_blocks_from_disk(params)
     sp = SocketPublish(params)
-    messages, hashes = sp.flatten_messages(block_lists)
-
-    loggers = await create_loggers(hashes, logger_type, logger_timeout,
-                                   included_peers, excluded_peers,
-                                   logger_expected_count)
-
-    enable_logging_task = asyncio.create_task(start_loggers(loggers))
+    messages, _ = sp.flatten_messages(block_lists)
     sp_task = asyncio.create_task(sp.run(messages))
-
-    # Await both tasks concurrently
-    await asyncio.gather(enable_logging_task, sp_task)
+    await asyncio.gather(sp_task)
 
 
 def read_blocks_from_disk(path, seeds=False, hashes=False, blocks=False):
     res = ConfigReadWrite().read_json(path)
     if seeds: return res["s"]
     if hashes: return res["h"]
     if blocks: return res["b"]
```

### Comparing `nanolab-0.0.4/nanolab/node_tools.py` & `nanolab-0.0.5/nanolab/node_tools.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.4/nanolab/pycmd.py` & `nanolab-0.0.5/nanolab/pycmd.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,24 +11,18 @@
 
 class NodeInteraction:
 
     def __init__(self):
         # Your existing code...
         self.logger = None
 
-    def publish_blocks(self,
-                       publish_params,
-                       logger_type=None,
-                       logger_timeout=600,
-                       logger_include_peers=None,
-                       logger_exclude_peers=None,
-                       logger_expected_count=None):
+    def start_logger(self, logger_type, sink_type, logger_params):
+        asyncio.run(nni.start_loggers(logger_type, sink_type, logger_params))
+
+    def publish_blocks(self, publish_params):
         '''
         mandatory publish_params: blocks_path, bps
-        optional  publish_params: peers, split, split_skip, reverse, shuffle, 
+         optional publish_params: peers, split, split_skip, reverse, shuffle, 
                   start_round, end_round, subset.start_index, subset.end_index
          '''
 
-        asyncio.run(
-            nni.xnolib_publish(publish_params, logger_type, logger_timeout,
-                               logger_include_peers, logger_exclude_peers,
-                               logger_expected_count))
+        asyncio.run(nni.xnolib_publish(publish_params))
```

### Comparing `nanolab-0.0.4/nanolab/snippets/default_snips.json` & `nanolab-0.0.5/nanolab/snippets/default_snips.json`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.4/nanolab/snippets/test_snippets.json` & `nanolab-0.0.5/nanolab/snippets/test_snippets.json`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.4/nanolab/src/argparse_commands.py` & `nanolab-0.0.5/nanolab/src/argparse_commands.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.4/nanolab/src/config_handler.py` & `nanolab-0.0.5/nanolab/src/config_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     def _copy_path(self,
                    source_path: str,
                    destination: Path,
                    force_copy=None) -> str:
         source = Path(source_path)
 
         copy_files = force_copy or environ.get("NL_COPY_FILES", "False")
-        if str(copy_files).lower() == "true" and not destination.exists():
+        if str(copy_files).lower() == "true" or not destination.exists():
             shutil.copy(source, destination)
         return destination
 
     def _download_url(self, url: str, resource_path: Path) -> Path:
         return download_data(url.strip(), Path(url).name, resource_path)
 
     def _download_config_file(self, destination: Path) -> Path:
```

### Comparing `nanolab-0.0.4/nanolab/src/config_loader.py` & `nanolab-0.0.5/nanolab/src/config_loader.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.4/nanolab/src/github.py` & `nanolab-0.0.5/nanolab/src/github.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.4/nanolab/src/resolver.py` & `nanolab-0.0.5/nanolab/src/resolver.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.4/nanolab/src/snippet_manager.py` & `nanolab-0.0.5/nanolab/src/snippet_manager.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.4/nanolab/src/utils.py` & `nanolab-0.0.5/nanolab/src/utils.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.4/nanolab/xnomin/acctools.py` & `nanolab-0.0.5/nanolab/xnomin/acctools.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.4/nanolab/xnomin/handshake.py` & `nanolab-0.0.5/nanolab/xnomin/handshake.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.4/nanolab/xnomin/peers.py` & `nanolab-0.0.5/nanolab/xnomin/peers.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.4/nanolab/xnomin/telemetry_req.py` & `nanolab-0.0.5/nanolab/xnomin/telemetry_req.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.4/nanolab.egg-info/PKG-INFO` & `nanolab-0.0.5/nanolab.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanolab
-Version: 0.0.4
+Version: 0.0.5
 Summary: testing tool using nanomock
 Home-page: https://github.com/gr0vity-dev/nanolab
 Author: gr0vity
 Description-Content-Type: text/markdown
 
 ##NanoLab
```

### Comparing `nanolab-0.0.4/nanolab.egg-info/SOURCES.txt` & `nanolab-0.0.5/nanolab.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -16,14 +16,27 @@
 nanolab/command/__init__.py
 nanolab/command/command.py
 nanolab/command/mixins/__init__.py
 nanolab/command/mixins/base_mixin.py
 nanolab/command/mixins/bash_command_mixin.py
 nanolab/command/mixins/python_command_mixin.py
 nanolab/command/mixins/threaded_command_mixin.py
+nanolab/loggers/__init__.py
+nanolab/loggers/builders.py
+nanolab/loggers/contracts.py
+nanolab/loggers/logger_handler.py
+nanolab/loggers/factories/__init__.py
+nanolab/loggers/factories/logger_factory.py
+nanolab/loggers/factories/sink_factory.py
+nanolab/loggers/sinks/__init__.py
+nanolab/loggers/sinks/console_sink.py
+nanolab/loggers/sinks/csv_sink.py
+nanolab/loggers/sinks/sql_sink.py
+nanolab/loggers/sources/__init__.py
+nanolab/loggers/sources/rpc_logger.py
 nanolab/snippets/default_snips.json
 nanolab/snippets/test_snippets.json
 nanolab/src/__init__.py
 nanolab/src/argparse_commands.py
 nanolab/src/config_handler.py
 nanolab/src/config_loader.py
 nanolab/src/github.py
```

### Comparing `nanolab-0.0.4/setup.py` & `nanolab-0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name="nanolab",
-      version="0.0.4",
+      version="0.0.5",
       author="gr0vity",
       description="testing tool using nanomock",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/gr0vity-dev/nanolab",
       packages=find_packages(exclude=["unit_tests"]),
       include_package_data=True,
-      install_requires=["nanomock>=0.0.10"],
+      install_requires=["nanomock>=0.0.10", "sqlalchemy"],
       entry_points={
           'console_scripts': [
               'nanolab=nanolab.main:main',
           ],
       })
```


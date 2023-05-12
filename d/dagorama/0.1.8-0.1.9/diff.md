# Comparing `tmp/dagorama-0.1.8.tar.gz` & `tmp/dagorama-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagorama-0.1.8.tar", max compression
+gzip compressed data, was "dagorama-0.1.9.tar", max compression
```

## Comparing `dagorama-0.1.8.tar` & `dagorama-0.1.9.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     1071 2023-03-14 00:35:34.466783 dagorama-0.1.8/LICENSE
--rw-r--r--   0        0        0    11160 2023-03-14 00:35:34.466783 dagorama-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/api/__init__.py
--rw-r--r--   0        0        0     4580 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/api/api_pb2.py
--rw-r--r--   0        0        0    10531 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/api/api_pb2.pyi
--rw-r--r--   0        0        0    13710 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/api/api_pb2_grpc.py
--rw-r--r--   0        0        0     3149 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/api/api_pb2_grpc.pyi
--rw-r--r--   0        0        0      441 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/cli.py
--rw-r--r--   0        0        0     1560 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/code_signature.py
--rw-r--r--   0        0        0     7734 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/decorators.py
--rw-r--r--   0        0        0     4793 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/definition.py
--rw-r--r--   0        0        0     2671 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/inspection.py
--rw-r--r--   0        0        0     1057 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/logging.py
--rw-r--r--   0        0        0        0 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/models/__init__.py
--rw-r--r--   0        0        0     1451 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/models/arguments.py
--rw-r--r--   0        0        0      557 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/models/promise.py
--rw-r--r--   0        0        0     1110 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/retry.py
--rw-r--r--   0        0        0     6834 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/runner.py
--rw-r--r--   0        0        0     2597 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/serializer.py
--rw-r--r--   0        0        0        0 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/tests/__init__.py
--rw-r--r--   0        0        0      225 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/tests/conftest.py
--rw-r--r--   0        0        0     1356 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/tests/test_code_signature.py
--rw-r--r--   0        0        0     3489 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/tests/test_decorators.py
--rw-r--r--   0        0        0      779 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/tests/test_definition.py
--rw-r--r--   0        0        0      410 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/tests/test_retry.py
--rw-r--r--   0        0        0     1071 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/tests/test_runner.py
--rw-r--r--   0        0        0     2043 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/tests/test_sample_dag.py
--rw-r--r--   0        0        0     1110 2023-03-14 00:35:34.470783 dagorama-0.1.8/dagorama/tests/test_typecheck.py
--rw-r--r--   0        0        0      630 2023-03-14 00:35:34.470783 dagorama-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    11618 1970-01-01 00:00:00.000000 dagorama-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-03-14 01:27:11.859324 dagorama-0.1.9/LICENSE
+-rw-r--r--   0        0        0    11160 2023-03-14 01:27:11.863324 dagorama-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-03-14 01:27:11.863324 dagorama-0.1.9/dagorama/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 01:27:11.863324 dagorama-0.1.9/dagorama/api/__init__.py
+-rw-r--r--   0        0        0     4580 2023-03-14 01:27:11.863324 dagorama-0.1.9/dagorama/api/api_pb2.py
+-rw-r--r--   0        0        0    10531 2023-03-14 01:27:11.863324 dagorama-0.1.9/dagorama/api/api_pb2.pyi
+-rw-r--r--   0        0        0    13710 2023-03-14 01:27:11.863324 dagorama-0.1.9/dagorama/api/api_pb2_grpc.py
+-rw-r--r--   0        0        0     3149 2023-03-14 01:27:11.863324 dagorama-0.1.9/dagorama/api/api_pb2_grpc.pyi
+-rw-r--r--   0        0        0      441 2023-03-14 01:27:11.863324 dagorama-0.1.9/dagorama/cli.py
+-rw-r--r--   0        0        0     1576 2023-03-14 01:27:11.863324 dagorama-0.1.9/dagorama/code_signature.py
+-rw-r--r--   0        0        0     7744 2023-03-14 01:27:11.863324 dagorama-0.1.9/dagorama/decorators.py
+-rw-r--r--   0        0        0     4793 2023-03-14 01:27:11.863324 dagorama-0.1.9/dagorama/definition.py
+-rw-r--r--   0        0        0     2671 2023-03-14 01:27:11.867324 dagorama-0.1.9/dagorama/inspection.py
+-rw-r--r--   0        0        0     1241 2023-03-14 01:27:11.867324 dagorama-0.1.9/dagorama/logging.py
+-rw-r--r--   0        0        0        0 2023-03-14 01:27:11.867324 dagorama-0.1.9/dagorama/models/__init__.py
+-rw-r--r--   0        0        0     1451 2023-03-14 01:27:11.867324 dagorama-0.1.9/dagorama/models/arguments.py
+-rw-r--r--   0        0        0      557 2023-03-14 01:27:11.867324 dagorama-0.1.9/dagorama/models/promise.py
+-rw-r--r--   0        0        0     1110 2023-03-14 01:27:11.867324 dagorama-0.1.9/dagorama/retry.py
+-rw-r--r--   0        0        0     6865 2023-03-14 01:27:11.867324 dagorama-0.1.9/dagorama/runner.py
+-rw-r--r--   0        0        0     2597 2023-03-14 01:27:11.867324 dagorama-0.1.9/dagorama/serializer.py
+-rw-r--r--   0        0        0        0 2023-03-14 01:27:11.867324 dagorama-0.1.9/dagorama/tests/__init__.py
+-rw-r--r--   0        0        0      225 2023-03-14 01:27:11.867324 dagorama-0.1.9/dagorama/tests/conftest.py
+-rw-r--r--   0        0        0     1356 2023-03-14 01:27:11.867324 dagorama-0.1.9/dagorama/tests/test_code_signature.py
+-rw-r--r--   0        0        0     3489 2023-03-14 01:27:11.867324 dagorama-0.1.9/dagorama/tests/test_decorators.py
+-rw-r--r--   0        0        0      779 2023-03-14 01:27:11.867324 dagorama-0.1.9/dagorama/tests/test_definition.py
+-rw-r--r--   0        0        0     1003 2023-03-14 01:27:11.867324 dagorama-0.1.9/dagorama/tests/test_logging.py
+-rw-r--r--   0        0        0      410 2023-03-14 01:27:11.867324 dagorama-0.1.9/dagorama/tests/test_retry.py
+-rw-r--r--   0        0        0     1071 2023-03-14 01:27:11.867324 dagorama-0.1.9/dagorama/tests/test_runner.py
+-rw-r--r--   0        0        0     2043 2023-03-14 01:27:11.867324 dagorama-0.1.9/dagorama/tests/test_sample_dag.py
+-rw-r--r--   0        0        0     1110 2023-03-14 01:27:11.867324 dagorama-0.1.9/dagorama/tests/test_typecheck.py
+-rw-r--r--   0        0        0      630 2023-03-14 01:27:11.867324 dagorama-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    11618 1970-01-01 00:00:00.000000 dagorama-0.1.9/PKG-INFO
```

### Comparing `dagorama-0.1.8/LICENSE` & `dagorama-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dagorama-0.1.8/README.md` & `dagorama-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dagorama-0.1.8/dagorama/api/api_pb2.py` & `dagorama-0.1.9/dagorama/api/api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagorama-0.1.8/dagorama/api/api_pb2.pyi` & `dagorama-0.1.9/dagorama/api/api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dagorama-0.1.8/dagorama/api/api_pb2_grpc.py` & `dagorama-0.1.9/dagorama/api/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagorama-0.1.8/dagorama/api/api_pb2_grpc.pyi` & `dagorama-0.1.9/dagorama/api/api_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `dagorama-0.1.8/dagorama/code_signature.py` & `dagorama-0.1.9/dagorama/code_signature.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from hashlib import md5
 from inspect import getfullargspec
 from marshal import dumps
 from typing import Any, Callable
 
 import pkg_resources
 
-from dagorama.logging import LOGGER
+from dagorama.logging import get_logger
 
 
 def get_explicit_dependencies():
     """
     Gets one layer of dependencies, does not attempt to recurse down the
     dependency tree.
 
@@ -33,19 +33,19 @@
         name=fn.__name__,
         code=fn.__code__.co_code,
         constants=fn.__code__.co_consts,
         args=argspec.args,
         kwargs=argspec.kwonlyargs,
     )
     runtime_code_raw = dumps(fn_definition)
-    LOGGER.debug(f"Hash: Definition: {fn_definition}")
+    get_logger().debug(f"Hash: Definition: {fn_definition}")
 
     if include_package_versions:
         dependencies = get_explicit_dependencies()
         dependencies = sorted(dependencies, key=lambda x: x[0])
 
         runtime_code_raw += dumps(dependencies)
 
     hash_value = b64encode(md5(runtime_code_raw).digest()).decode()
-    LOGGER.debug(f"Hash: Value: {hash_value} (include_package_versions: {include_package_versions})")
+    get_logger().debug(f"Hash: Value: {hash_value} (include_package_versions: {include_package_versions})")
 
     return hash_value
```

### Comparing `dagorama-0.1.8/dagorama/decorators.py` & `dagorama-0.1.9/dagorama/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Any, ParamSpec, TypeVar, cast
 from uuid import uuid4
 
 import dagorama.api.api_pb2 as pb2
 from dagorama.code_signature import calculate_function_hash
 from dagorama.definition import DAGDefinition, DAGInstance, dagorama_context
 from dagorama.inspection import find_promises
-from dagorama.logging import LOGGER
+from dagorama.logging import get_logger
 from dagorama.models.arguments import DAGArguments
 from dagorama.models.promise import DAGPromise
 from dagorama.retry import RetryConfiguration
 from dagorama.serializer import function_to_name
 
 T = TypeVar('T')
 P = ParamSpec('P')
@@ -166,15 +166,15 @@
         )
 
         # Find the dependencies
         promise_dependencies = find_promises([isolated_args, kwargs])
 
         # Add to the remote runloop
         with dagorama_context() as context:
-            LOGGER.debug(f"Creating node {promise.identifier} for {promise.function_name}")
+            get_logger().debug(f"Creating node {promise.identifier} for {promise.function_name}")
             context.CreateNode(
                 pb2.NodeConfigurationMessage(
                     identifier=str(promise.identifier),
                     functionName=cast(str, promise.function_name),
                     functionHash=calculate_function_hash(func),
                     taintName=self.taint_name or "",
                     queueName=self.queue_name or cast(str, promise.function_name),
```

### Comparing `dagorama-0.1.8/dagorama/definition.py` & `dagorama-0.1.9/dagorama/definition.py`

 * *Files identical despite different names*

### Comparing `dagorama-0.1.8/dagorama/inspection.py` & `dagorama-0.1.9/dagorama/inspection.py`

 * *Files identical despite different names*

### Comparing `dagorama-0.1.8/dagorama/models/arguments.py` & `dagorama-0.1.9/dagorama/models/arguments.py`

 * *Files identical despite different names*

### Comparing `dagorama-0.1.8/dagorama/models/promise.py` & `dagorama-0.1.9/dagorama/models/promise.py`

 * *Files identical despite different names*

### Comparing `dagorama-0.1.8/dagorama/retry.py` & `dagorama-0.1.9/dagorama/retry.py`

 * *Files identical despite different names*

### Comparing `dagorama-0.1.8/dagorama/runner.py` & `dagorama-0.1.9/dagorama/runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import grpc
 
 import dagorama.api.api_pb2 as pb2
 import dagorama.api.api_pb2_grpc as pb2_grpc
 from dagorama.code_signature import calculate_function_hash
 from dagorama.definition import dagorama_context
 from dagorama.inspection import resolve_promises
-from dagorama.logging import LOGGER, get_default_console_width
+from dagorama.logging import get_logger, get_default_console_width
 from dagorama.models.arguments import DAGArguments
 from dagorama.serializer import name_to_function
 
 
 class CodeMismatchException(Exception):
     """
     If raised, the queued DAGNode and the current runner are using
@@ -44,14 +44,16 @@
 async def execute_worker_async(
     exclude_queues: list | None = None,
     include_queues: list | None = None,
     queue_tolerations: list | None = None,
     infinite_loop: bool = True,
     catch_exceptions: bool = True,
 ):
+    logger = get_logger()
+
     with dagorama_context() as context:
         worker = context.CreateWorker(
             pb2.WorkerConfigurationMessage(
                 excludeQueues=exclude_queues or [],
                 includeQueues=include_queues or [],
                 queueTolerations=queue_tolerations or [],
             )
@@ -67,15 +69,15 @@
         while True:
             try:
                 next_item = context.GetWork(worker)
             except grpc.RpcError as e:
                 if e.details() == "no work available":
                     if not infinite_loop:
                         return
-                    LOGGER.debug("No work available, polling in 1s...")
+                    logger.debug("No work available, polling in 1s...")
                     sleep(1)
                     continue
                 else:
                     raise
 
             arguments = DAGArguments.from_server_bytes(next_item.arguments)
 
@@ -90,35 +92,35 @@
 
             # Since this function was queued as part of the worker, we can assume that it will
             # be a wrapped @dagorama function - it will therefore be a standard callable without
             # async since it takes care of the client-side async logic internally.
             resolved_fn = name_to_function(next_item.functionName, next_item.instanceId)
 
             console_width = get_default_console_width()
-            LOGGER.debug("-" * console_width)
-            LOGGER.debug(f"Executing {next_item} with {arguments}")
-            LOGGER.debug(f"Resolved values: {resolved_values} | {resolved_args} | {resolved_kwargs}")
-            LOGGER.debug(f"Resolved fn: {resolved_fn}")
-            LOGGER.debug("-" * console_width)
+            logger.debug("-" * console_width)
+            logger.debug(f"Executing {next_item} with {arguments}")
+            logger.debug(f"Resolved values: {resolved_values} | {resolved_args} | {resolved_kwargs}")
+            logger.debug(f"Resolved fn: {resolved_fn}")
+            logger.debug("-" * console_width)
 
             #print("COMPARE VALUES", calculate_function_hash(resolved_fn.original_fn), next_item.functionHash)
             # Ensure that we have the correct local version of the function
             current_fn_hash = calculate_function_hash(resolved_fn.original_fn)
             if current_fn_hash != next_item.functionHash:
-                LOGGER.debug(f"Function hash mismatch, expected {next_item.functionHash} but got {current_fn_hash}")
+                logger.debug(f"Function hash mismatch, expected {next_item.functionHash} but got {current_fn_hash}")
                 raise CodeMismatchException()
 
             if catch_exceptions:
                 try:
                     result = resolved_fn(*resolved_args, greedy_execution=True, **resolved_kwargs)
                     if isawaitable(result):
                         result = await result
                 except Exception as e:
                     traceback = format_exc()
-                    LOGGER.warning(f"Exception encountered, reporting to broker: {e}\n{traceback}")
+                    logger.warning(f"Exception encountered, reporting to broker: {e}\n{traceback}")
                     context.SubmitFailure(
                         pb2.WorkFailedMessage(
                             instanceId=next_item.instanceId,
                             nodeId=next_item.identifier,
                             workerId=worker.identifier,
                             traceback=traceback
                         )
```

### Comparing `dagorama-0.1.8/dagorama/serializer.py` & `dagorama-0.1.9/dagorama/serializer.py`

 * *Files identical despite different names*

### Comparing `dagorama-0.1.8/dagorama/tests/test_code_signature.py` & `dagorama-0.1.9/dagorama/tests/test_code_signature.py`

 * *Files identical despite different names*

### Comparing `dagorama-0.1.8/dagorama/tests/test_decorators.py` & `dagorama-0.1.9/dagorama/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `dagorama-0.1.8/dagorama/tests/test_definition.py` & `dagorama-0.1.9/dagorama/tests/test_definition.py`

 * *Files identical despite different names*

### Comparing `dagorama-0.1.8/dagorama/tests/test_runner.py` & `dagorama-0.1.9/dagorama/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `dagorama-0.1.8/dagorama/tests/test_sample_dag.py` & `dagorama-0.1.9/dagorama/tests/test_sample_dag.py`

 * *Files identical despite different names*

### Comparing `dagorama-0.1.8/dagorama/tests/test_typecheck.py` & `dagorama-0.1.9/dagorama/tests/test_typecheck.py`

 * *Files identical despite different names*

### Comparing `dagorama-0.1.8/pyproject.toml` & `dagorama-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dagorama"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Pierce Freeman <pierce@freeman.vc>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 grpcio = "^1.50.0"
```

### Comparing `dagorama-0.1.8/PKG-INFO` & `dagorama-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagorama
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Pierce Freeman
 Author-email: pierce@freeman.vc
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


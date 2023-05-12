# Comparing `tmp/aiosow-0.1.4.tar.gz` & `tmp/aiosow-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosow-0.1.4.tar", last modified: Thu May 11 16:22:17 2023, max compression
+gzip compressed data, was "aiosow-0.1.5.tar", last modified: Fri May 12 10:57:49 2023, max compression
```

## Comparing `aiosow-0.1.4.tar` & `aiosow-0.1.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:22:17.574811 aiosow-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-11 16:22:17.574811 aiosow-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-11 16:22:02.000000 aiosow-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:22:17.566811 aiosow-0.1.4/aiosow/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-11 16:22:02.000000 aiosow-0.1.4/aiosow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-11 16:22:02.000000 aiosow-0.1.4/aiosow/autofill.py
--rw-r--r--   0 runner    (1001) docker     (123)    13084 2023-05-11 16:22:02.000000 aiosow-0.1.4/aiosow/bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-11 16:22:02.000000 aiosow-0.1.4/aiosow/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-11 16:22:02.000000 aiosow-0.1.4/aiosow/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-05-11 16:22:02.000000 aiosow-0.1.4/aiosow/perpetuate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-11 16:22:02.000000 aiosow-0.1.4/aiosow/routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-11 16:22:02.000000 aiosow-0.1.4/aiosow/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:22:17.570811 aiosow-0.1.4/aiosow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-11 16:22:17.000000 aiosow-0.1.4/aiosow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-11 16:22:17.000000 aiosow-0.1.4/aiosow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:22:17.000000 aiosow-0.1.4/aiosow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-11 16:22:17.000000 aiosow-0.1.4/aiosow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-11 16:22:17.000000 aiosow-0.1.4/aiosow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 16:22:17.000000 aiosow-0.1.4/aiosow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 16:22:17.574811 aiosow-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-11 16:22:02.000000 aiosow-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:22:17.574811 aiosow-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-11 16:22:02.000000 aiosow-0.1.4/tests/test_autofill.py
--rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-05-11 16:22:02.000000 aiosow-0.1.4/tests/test_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:22:02.000000 aiosow-0.1.4/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-11 16:22:02.000000 aiosow-0.1.4/tests/test_perpetuate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-11 16:22:02.000000 aiosow-0.1.4/tests/test_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-11 16:22:02.000000 aiosow-0.1.4/tests/test_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:57:49.321510 aiosow-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-12 10:57:49.321510 aiosow-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-12 10:57:36.000000 aiosow-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:57:49.321510 aiosow-0.1.5/aiosow/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-12 10:57:36.000000 aiosow-0.1.5/aiosow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-05-12 10:57:36.000000 aiosow-0.1.5/aiosow/autofill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-12 10:57:36.000000 aiosow-0.1.5/aiosow/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-12 10:57:36.000000 aiosow-0.1.5/aiosow/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-12 10:57:36.000000 aiosow-0.1.5/aiosow/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-05-12 10:57:36.000000 aiosow-0.1.5/aiosow/perpetuate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-12 10:57:36.000000 aiosow-0.1.5/aiosow/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-12 10:57:36.000000 aiosow-0.1.5/aiosow/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:57:49.321510 aiosow-0.1.5/aiosow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-12 10:57:49.000000 aiosow-0.1.5/aiosow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-12 10:57:49.000000 aiosow-0.1.5/aiosow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:57:49.000000 aiosow-0.1.5/aiosow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-12 10:57:49.000000 aiosow-0.1.5/aiosow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-12 10:57:49.000000 aiosow-0.1.5/aiosow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 10:57:49.000000 aiosow-0.1.5/aiosow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 10:57:49.321510 aiosow-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-12 10:57:36.000000 aiosow-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:57:49.321510 aiosow-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-05-12 10:57:36.000000 aiosow-0.1.5/tests/test_autofill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-12 10:57:36.000000 aiosow-0.1.5/tests/test_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 10:57:36.000000 aiosow-0.1.5/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-12 10:57:36.000000 aiosow-0.1.5/tests/test_perpetuate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-12 10:57:36.000000 aiosow-0.1.5/tests/test_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-12 10:57:36.000000 aiosow-0.1.5/tests/test_setup.py
```

### Comparing `aiosow-0.1.4/PKG-INFO` & `aiosow-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosow
-Version: 0.1.4
+Version: 0.1.5
 Summary: An event-based framework
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 
 [![Pypi](https://img.shields.io/pypi/v/aiosow?color=white&style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/aiosow/)
```

### Comparing `aiosow-0.1.4/README.md` & `aiosow-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.4/aiosow/autofill.py` & `aiosow-0.1.5/aiosow/autofill.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 await function(*args, **memory) -> this doesn't work because :
     - it is not generic and will break whenever a function doesn't take **kwargs
     - kwargs itself is a copy and will break reference
 """
 from typing import Any, Callable, List
-from types import LambdaType
 
 import inspect, logging, asyncio
 
 ALIASES = {}
 
 
 def get_aliases():  # pragma: no cover
@@ -114,26 +113,32 @@
             param.kind == inspect.Parameter.VAR_POSITIONAL
             for param in inspect.signature(function).parameters.values()
         )
         given_args = given_args if not has_varargs else given_args + list(argscopy)
     return (name, given_args, kws)
 
 
+def get_function_representation(function):
+    name = function.__name__
+    if name == "<lambda>":
+        name = (
+            inspect.getsource(function)
+            .replace("\n", "")
+            .replace("\t", "")
+            .replace("    ", "")
+        )
+    return name
+
+
 async def autofill(function: Callable, args: Any = [], **kwargs) -> Any:
     name, given_args, kws = await fill_prototype(function, args=args, **kwargs)
     try:
-        if kwargs.get("memory", {}).get("log_autofill", False):
-            if name == "<lambda>":
-                name = (
-                    inspect.getsource(function)
-                    .replace("\n", "")
-                    .replace("\t", "")
-                    .replace("    ", "")
-                )
-            logging.info(f" -> {name}")
+        if kwargs.get("memory", {}).get("log_autofill", False):  # pragma: no cover
+            function_representation = get_function_representation(function)
+            logging.info(f" -> {function_representation}")
         result = function(*given_args, **kws)
         return await result if inspect.iscoroutine(result) else result
     except Exception as err:  # pragma: no cover
         logging.error(f"{name} : {err}")
         logging.debug(f" > error generated by calling {name}({given_args})")
         raise (err)  # `debug` needs `autofill` to raise
 
@@ -154,8 +159,8 @@
         loop = asyncio.get_event_loop()
         __name__, given_args, kws = await fill_prototype(function, args=args, **kwargs)
         return await loop.run_in_executor(None, function, *given_args, **kws)
 
     return wrapper
 
 
-__all__ = ["alias", "autofill", "make_async"]
+__all__ = ["alias", "autofill", "make_async", "fill_prototype"]
```

### Comparing `aiosow-0.1.4/aiosow/bindings.py` & `aiosow-0.1.5/aiosow/bindings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,38 @@
-from typing import Tuple, Callable, Any
+from typing import Tuple, Callable, Any, Union
 
 import pdb as _pdb
 import asyncio
 import time
 import inspect
-
 from functools import wraps
 
 from aiosow.autofill import autofill, alias, make_async
 from aiosow.options import option
 from aiosow.perpetuate import on, perpetuate
 from aiosow.setup import setup
 
 
+def adapter(resolve: Callable) -> Callable:
+    """
+    [unstable implementation]
+    Inverse of `wrap`. Allows to mutate the parameter given to a function
+    """
+
+    def wrapper(function: Callable) -> Callable:
+        async def caller(item, **kwargs):
+            value = await autofill(resolve, args=[item], **kwargs)
+            result = await autofill(function, args=[value], **kwargs)
+            return result
+
+        return caller
+
+    return wrapper
+
+
 def chain(*functions):
     """Applies functions iteratively and pass each result to next function"""
 
     async def _chain(*args, **kwargs):
         result = None
         has_result = False
         for function in functions:
@@ -147,15 +163,15 @@
     def listen_decorator(listener):
         listeners.append(listener)
         return listener
 
     return (trigger_decorator, listen_decorator)
 
 
-def accumulator(size: int | Callable) -> Callable:
+def accumulator(size: Union[int, Callable]) -> Callable:
     """
     Batch the calls to a function. Triggers it when the bucket size is reached.
     If the size passed is a `Callable`, accumulator will call it with `memory`
     to get the size.
     """
 
     def decorator(function: Callable) -> Callable:
@@ -275,15 +291,15 @@
             return wrapper_function(result)
 
         return execute
 
     return decorator
 
 
-def each(iter: Callable | None = None):
+def each(iter: Union[Callable, None] = None):
     """
     Applies a function to each item in :
         - result of iter
         or
         - first argument passed to the resulting function
 
     **Args**:
```

### Comparing `aiosow-0.1.4/aiosow/command.py` & `aiosow-0.1.5/aiosow/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,16 @@
     logging.debug(memory)
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
     tasks = loop.run_until_complete(initialize(memory))
     memory["running"] = True
     if TRIGGER_ROUTINES:
         consumer = loop.run_until_complete(spawn_routine_consumer(memory))
-        tasks = tasks + [consumer]
+        if consumer:
+            tasks = tasks + [consumer]
     # setups can return a task which is ran here
     # this allows setups to start tasks and still have them complete
     loop.run_until_complete(asyncio.gather(*tasks))
     if memory["run_forever"]:
         loop.run_forever()
```

### Comparing `aiosow-0.1.4/aiosow/options.py` & `aiosow-0.1.5/aiosow/options.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     - name: str -> the name of the option (will be used as f'--{name}')
     - kwargs: dict -> the options used by [argparse](https://docs.python.org/3/library/argparse.html)
     """
     global OPTIONS
     OPTIONS.append((args, kwargs))
 
 
-def command(name):
+def command(name):  # pragma: no cover
     """
     Register an argparse command to be available using the command-line.
 
     **args**:
     - name: str -> the name of the option (will be used as f'--{name}')
     - kwargs: dict -> the options used by [argparse](https://docs.python.org/3/library/argparse.html)
     """
```

### Comparing `aiosow-0.1.4/aiosow/perpetuate.py` & `aiosow-0.1.5/aiosow/perpetuate.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.4/aiosow/routines.py` & `aiosow-0.1.5/aiosow/routines.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,19 +75,16 @@
 
     return decorator
 
 
 async def consume_routines(memory):
     routines = get_routines()
     # Find the routine with the smallest remaining timeout or a timeout <= 0
-    if len(routines):
-        smallest_timeout_routine = min(routines, key=lambda x: x["timeout"])
-        smallest_timeout = smallest_timeout_routine["timeout"]
-    else:
-        smallest_timeout = 0
+    smallest_timeout_routine = min(routines, key=lambda x: x["timeout"])
+    smallest_timeout = smallest_timeout_routine["timeout"]
 
     # Wait until the smallest timeout has elapsed
     await asyncio.sleep(smallest_timeout)
 
     # Execute any routines that have timed out
     for routine in routines:
         routine["timeout"] -= smallest_timeout
@@ -115,11 +112,12 @@
 
 async def routine_consumer(memory):  # pragma: no cover
     while True:
         await autofill(consume_routines, memory=memory)
 
 
 async def spawn_routine_consumer(memory):  # pragma: no cover
-    return asyncio.create_task(routine_consumer(memory))
+    if len(ROUTINES) > 0:
+        return asyncio.create_task(routine_consumer(memory))
 
 
 __all__ = ["routine", "infinite_generator"]
```

### Comparing `aiosow-0.1.4/aiosow/setup.py` & `aiosow-0.1.5/aiosow/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 
 
 def clear_setups():  # pragma: no cover
     global SETUP_FUNCTIONS
     SETUP_FUNCTIONS = []
 
 
+def get_setups():  # pragma: no cover
+    global SETUP_FUNCTIONS
+    return SETUP_FUNCTIONS
+
+
 def setup(func: Callable) -> Callable:
     """
     Decorator to add a function to the list of initialization functions.
 
     **Args**:
     - func (Callable): Function to add to the list of initialization functions.
```

### Comparing `aiosow-0.1.4/aiosow.egg-info/PKG-INFO` & `aiosow-0.1.5/aiosow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosow
-Version: 0.1.4
+Version: 0.1.5
 Summary: An event-based framework
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 
 [![Pypi](https://img.shields.io/pypi/v/aiosow?color=white&style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/aiosow/)
```

### Comparing `aiosow-0.1.4/setup.py` & `aiosow-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="aiosow",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(include=["aiosow"]),
     description="An event-based framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     entry_points={
         "console_scripts": [
```

### Comparing `aiosow-0.1.4/tests/test_autofill.py` & `aiosow-0.1.5/tests/test_autofill.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 import pytest
 
 from aiosow.bindings import delay
-from aiosow.autofill import get_aliases, reset_aliases, autofill, alias
+from aiosow.autofill import (
+    get_aliases,
+    reset_aliases,
+    autofill,
+    alias,
+    get_function_representation,
+)
 
 
 def my_func(__a__, __b__=2, __c__=3):
     """__ is used to prevent linter error"""
 
 
 @pytest.mark.asyncio
@@ -131,7 +137,25 @@
     memory = {"test": "error"}
 
     def test():
         return "correct"
 
     alias("test")(test)
     assert await autofill(my_function7, args=args, memory=memory) == "correct"
+
+
+def test_get_function_representation():
+    # Test case 1: Test with a named function
+    def named_function():
+        pass
+
+    assert get_function_representation(named_function) == "named_function"
+
+    # Test case 2: Test with a lambda function
+    lambda_function = lambda x: x**2
+    expected_result = "lambda_function = lambda x: x**2"
+    assert get_function_representation(lambda_function) == expected_result
+
+    # Test case 3: Test with a lambda function with whitespace
+    lambda_function = lambda x: x**2
+    expected_result = "lambda_function = lambda x: x**2"
+    assert get_function_representation(lambda_function) == expected_result
```

### Comparing `aiosow-0.1.4/tests/test_bindings.py` & `aiosow-0.1.5/tests/test_bindings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import time, asyncio
 import pytest
 from aiosow.bindings import (
+    adapter,
     expect,
     do_raise,
     dont_raise,
     return_true,
     return_false,
     call_limit,
     chain,
@@ -316,7 +317,21 @@
 
     lock = False
     mocked = MagicMock(side_effect=raise_if_lock_is_false)
     patched = expect(
         dont_unlock, retries=1, on_raise=dont_raise, condition=return_false
     )(mocked)
     result = await patched()
+
+
+@pytest.mark.asyncio
+async def test_adapter():
+    async def resolve(item):
+        return item + 1
+
+    async def multiply_by_two(num):
+        return num * 2
+
+    # Test case 1: Test with a function that takes a single argument
+    adapter_func = adapter(resolve)(multiply_by_two)
+    result = await adapter_func(1)
+    assert result == 4
```

### Comparing `aiosow-0.1.4/tests/test_perpetuate.py` & `aiosow-0.1.5/tests/test_perpetuate.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.4/tests/test_routines.py` & `aiosow-0.1.5/tests/test_routines.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.4/tests/test_setup.py` & `aiosow-0.1.5/tests/test_setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from aiosow.setup import initialize, setup, clear_setups
+from aiosow.setup import initialize, setup, clear_setups, get_setups
 
 
 async def my_init_function_1(foo: dict):
     foo["key_1"] = "value_1"
 
 
 async def my_init_function_2(foo: dict):
@@ -25,7 +25,15 @@
     setup(my_init_function_1)
     setup(my_init_function_2)
     setup(my_init_function_3)
     tasks = await initialize(kwargs)
     assert kwargs == {"foo": {"key_1": "value_1", "key_2": "value_2"}}
     assert len(tasks) == 1
     await tasks[0]
+
+
+@pytest.mark.asyncio
+async def test_duplicate_setup_declaration():
+    clear_setups()
+    setup(my_init_function_1)
+    setup(my_init_function_1)
+    assert len(get_setups()) == 1
```


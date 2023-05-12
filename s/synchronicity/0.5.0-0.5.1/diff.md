# Comparing `tmp/synchronicity-0.5.0-py3-none-any.whl.zip` & `tmp/synchronicity-0.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 21786 bytes, number of entries: 12
+Zip file size: 22449 bytes, number of entries: 13
 -rw-rw-r--  2.0 unx      100 b- defN 23-May-10 19:02 synchronicity/__init__.py
--rw-rw-r--  2.0 unx     2581 b- defN 23-May-10 19:02 synchronicity/async_wrap.py
+-rw-rw-r--  2.0 unx     1188 b- defN 23-May-12 07:52 synchronicity/annotations.py
+-rw-rw-r--  2.0 unx     2581 b- defN 23-May-11 08:00 synchronicity/async_wrap.py
 -rw-rw-r--  2.0 unx     1485 b- defN 23-Mar-23 14:53 synchronicity/callback.py
 -rw-rw-r--  2.0 unx     1303 b- defN 23-Mar-20 08:05 synchronicity/exceptions.py
 -rw-rw-r--  2.0 unx      331 b- defN 23-May-10 19:02 synchronicity/interface.py
 -rw-rw-r--  2.0 unx     1792 b- defN 23-May-10 19:02 synchronicity/overload_tracking.py
--rw-rw-r--  2.0 unx    30174 b- defN 23-May-10 19:02 synchronicity/synchronizer.py
--rw-rw-r--  2.0 unx    24842 b- defN 23-May-10 19:02 synchronicity/type_stubs.py
--rw-rw-r--  2.0 unx     7736 b- defN 23-May-10 19:05 synchronicity-0.5.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-10 19:05 synchronicity-0.5.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-May-10 19:05 synchronicity-0.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      998 b- defN 23-May-10 19:05 synchronicity-0.5.0.dist-info/RECORD
-12 files, 71448 bytes uncompressed, 20108 bytes compressed:  71.9%
+-rw-rw-r--  2.0 unx    30159 b- defN 23-May-12 07:52 synchronicity/synchronizer.py
+-rw-rw-r--  2.0 unx    24852 b- defN 23-May-12 07:52 synchronicity/type_stubs.py
+-rw-rw-r--  2.0 unx     7736 b- defN 23-May-12 07:54 synchronicity-0.5.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-12 07:54 synchronicity-0.5.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-May-12 07:54 synchronicity-0.5.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1083 b- defN 23-May-12 07:54 synchronicity-0.5.1.dist-info/RECORD
+13 files, 72716 bytes uncompressed, 20639 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: synchronicity/__init__.py
 Comment: 
 
+Filename: synchronicity/annotations.py
+Comment: 
+
 Filename: synchronicity/async_wrap.py
 Comment: 
 
 Filename: synchronicity/callback.py
 Comment: 
 
 Filename: synchronicity/exceptions.py
@@ -18,20 +21,20 @@
 
 Filename: synchronicity/synchronizer.py
 Comment: 
 
 Filename: synchronicity/type_stubs.py
 Comment: 
 
-Filename: synchronicity-0.5.0.dist-info/METADATA
+Filename: synchronicity-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: synchronicity-0.5.0.dist-info/WHEEL
+Filename: synchronicity-0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: synchronicity-0.5.0.dist-info/top_level.txt
+Filename: synchronicity-0.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: synchronicity-0.5.0.dist-info/RECORD
+Filename: synchronicity-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## synchronicity/synchronizer.py

```diff
@@ -1,19 +1,20 @@
 import asyncio
 import atexit
 import collections.abc
 import contextlib
 import functools
 import inspect
 import platform
-import sys
 import threading
 import typing
 import warnings
-from typing import Optional
+from typing import ForwardRef, Optional
+
+from synchronicity.annotations import evaluated_annotation
 
 from .async_wrap import wraps_by_interface
 from .callback import Callback
 from .exceptions import UserCodeException, unwrap_coro_exception, wrap_coro_exception
 from .interface import Interface
 
 _BUILTIN_ASYNC_METHODS = {
@@ -55,36 +56,31 @@
     collections.abc.AsyncIterator,
     collections.abc.AsyncIterable,
     collections.abc.AsyncGenerator,
     contextlib.AbstractAsyncContextManager,
 )
 
 
-def _type_requires_aio_usage(annotation, home_module):
+def _type_requires_aio_usage(annotation, declaration_module):
+    if isinstance(annotation, ForwardRef):
+        annotation = annotation.__forward_arg__
     if isinstance(annotation, str):
-        # evaluate string annotations...
-        # mod = importlib.import_module(home_module)
-        if home_module in sys.modules:
-            mod = sys.modules[home_module]
-            try:
-                annotation = eval(annotation, mod.__dict__)
-            except NameError:
-                # this could happen with forward annotations,
-                # or imports that aren't available in the namespace when synchronicity wrapping occurs
-                # TODO: support eval of non-imported modules?
-                return False
-        else:
+        try:
+            annotation = evaluated_annotation(annotation, declaration_module=declaration_module)
+        except Exception:
+            # TODO: this will be incorrect in special case of `arg: "Awaitable[some_forward_ref_type]"`,
+            #       but its a hard problem to solve without passing around globals everywhere
             return False
 
     if hasattr(annotation, "__origin__"):
-        if annotation.__origin__ in ASYNC_GENERIC_ORIGINS:
+        if annotation.__origin__ in ASYNC_GENERIC_ORIGINS:  # type: ignore
             return True
-        # recurse
+        # recurse for generic subtypes
         for a in getattr(annotation, "__args__", ()):
-            if _type_requires_aio_usage(a, home_module):
+            if _type_requires_aio_usage(a, declaration_module):
                 return True
     return False
 
 
 def should_have_aio_interface(func):
     # determines if a blocking function gets an .aio attribute with an async interface to the function or not
     if inspect.iscoroutinefunction(func) or inspect.isasyncgenfunction(func):
```

## synchronicity/type_stubs.py

```diff
@@ -6,32 +6,36 @@
 * Let synchronicity emit actual function bodies, to avoid runtime wrapping altogether
 """
 import collections
 import collections.abc
 import contextlib
 import importlib
 import inspect
+from logging import getLogger
 import sys
 import typing
 from pathlib import Path
 from typing import TypeVar, Generic
 from unittest import mock
 
 import sigtools.specifiers  # type: ignore
 from sigtools._signatures import EmptyAnnotation, UpgradedAnnotation, UpgradedParameter  # type: ignore
 
 import synchronicity
 from synchronicity import Interface, overload_tracking
+from synchronicity.annotations import evaluated_annotation
 from synchronicity.synchronizer import (
     TARGET_INTERFACE_ATTR,
     SYNCHRONIZER_ATTR,
     MethodWithAio,
     FunctionWithAio,
 )
 
+logger = getLogger(__name__)
+
 
 class ReprObj:
     # Hacky repr passthrough object so we can pass verbatim type annotations as partial arguments
     # to generic and have them render correctly through `repr()`, used by inspect.Signature etc.
     def __init__(self, repr: str):
         assert isinstance(repr, str), f"{repr} is not a string!"
         self._repr = repr
@@ -308,25 +312,22 @@
         * eval for string annotations (importing `home_module` to be used as namespace)
         * re-mapping of the annotation to the correct synchronicity target
           (using synchronizer and synchronicity_target_interface)
         * registers imports for all referenced modules
         """
         if isinstance(annotation, typing.ForwardRef):  # TypeVars wrap their arguments as ForwardRefs (sometimes?)
             annotation = annotation.__forward_arg__
-
         if isinstance(annotation, str):
-            assert home_module is not None
-            mod = importlib.import_module(home_module)
             try:
-                annotation = eval(annotation, mod.__dict__)
-            except NameError:
-                # attempt to import
-                guessed_module, name = annotation.rsplit(".", 1)
-                exec(f"import {guessed_module}", mod.__dict__)  # import first
-                annotation = eval(annotation, mod.__dict__)
+                annotation = evaluated_annotation(annotation, declaration_module=home_module)
+            except Exception:
+                logger.exception(
+                    f"Error when evaluating {annotation} in {home_module}. Falling back to string annotation"
+                )
+                return annotation
 
         annotation = self._translate_annotation_map_types(
             annotation,
             synchronizer=synchronizer,
             interface=synchronicity_target_interface,
             home_module=home_module,
         )
```

## Comparing `synchronicity-0.5.0.dist-info/METADATA` & `synchronicity-0.5.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synchronicity
-Version: 0.5.0
+Version: 0.5.1
 Summary: Export blocking and async library versions from a single async implementation
 Requires-Python: >=3.7.9
 Description-Content-Type: text/markdown
 Requires-Dist: sigtools (==4.0.1)
 
 ![CI/CD badge](https://github.com/erikbern/synchronicity/actions/workflows/ci.yml/badge.svg)
 [![pypi badge](https://img.shields.io/pypi/v/synchronicity.svg?style=flat)](https://pypi.python.org/pypi/synchronicity)
```


# Comparing `tmp/capabilities-0.1.0.tar.gz` & `tmp/capabilities-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capabilities-0.1.0.tar", last modified: Sun Apr 30 16:48:22 2023, max compression
+gzip compressed data, was "capabilities-0.1.2.tar", last modified: Fri May 12 04:31:03 2023, max compression
```

## Comparing `capabilities-0.1.0.tar` & `capabilities-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:48:22.954115 capabilities-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-30 16:48:11.000000 capabilities-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-04-30 16:48:22.954115 capabilities-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-30 16:48:11.000000 capabilities-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:48:22.950114 capabilities-0.1.0/capabilities/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12737 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:48:22.954115 capabilities-0.1.0/capabilities/search/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/search/hf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/search/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/search/nomic_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/search/oai.py
--rw-r--r--   0 runner    (1001) docker     (123)    12208 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/search/search_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/search/simple_vector_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/search/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/search/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-04-30 16:48:11.000000 capabilities-0.1.0/capabilities/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:48:22.954115 capabilities-0.1.0/capabilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-04-30 16:48:22.000000 capabilities-0.1.0/capabilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-30 16:48:22.000000 capabilities-0.1.0/capabilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 16:48:22.000000 capabilities-0.1.0/capabilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-30 16:48:22.000000 capabilities-0.1.0/capabilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-30 16:48:22.000000 capabilities-0.1.0/capabilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-30 16:48:11.000000 capabilities-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 16:48:22.954115 capabilities-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-30 16:48:11.000000 capabilities-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 04:31:03.283925 capabilities-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-12 04:30:41.000000 capabilities-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-05-12 04:31:03.283925 capabilities-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-12 04:30:41.000000 capabilities-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 04:31:03.279925 capabilities-0.1.2/capabilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15365 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/dec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 04:31:03.283925 capabilities-0.1.2/capabilities/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/search/hf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/search/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/search/nomic_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/search/oai.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/search/search_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/search/simple_vector_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/search/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/search/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 04:31:03.279925 capabilities-0.1.2/capabilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-05-12 04:31:03.000000 capabilities-0.1.2/capabilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-12 04:31:03.000000 capabilities-0.1.2/capabilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 04:31:03.000000 capabilities-0.1.2/capabilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-12 04:31:03.000000 capabilities-0.1.2/capabilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-12 04:31:03.000000 capabilities-0.1.2/capabilities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-12 04:30:41.000000 capabilities-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 04:31:03.283925 capabilities-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-12 04:30:41.000000 capabilities-0.1.2/setup.py
```

### Comparing `capabilities-0.1.0/LICENSE` & `capabilities-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `capabilities-0.1.0/PKG-INFO` & `capabilities-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capabilities
-Version: 0.1.0
+Version: 0.1.2
 Summary: Build trusted, faster, and more powerful applications with the Blazon Capabilities API.
 Author-email: Blazon AI <support@blazon.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `capabilities-0.1.0/capabilities/core.py` & `capabilities-0.1.2/capabilities/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import os
 import dataclasses
+import typing
 import dacite
 from dataclasses import dataclass, field, is_dataclass
-from typing import Dict, Any, List, Union, Literal
+from typing import Dict, Any, List, Type, TypeAlias, TypeVar, Union, Literal
 from typing import Optional
 import requests
 import aiohttp
 import asyncio
 import time
 from capabilities.config import CONFIG
 from pydantic import BaseModel
+from pydantic.fields import ModelField
 from pydantic.main import ModelMetaclass
+import logging
+
+logger = logging.getLogger("capabilities")
 
 
 @dataclass
 class CapabilityBase:
     ...
 
 
@@ -47,47 +52,59 @@
                 A coroutine that resolves to a dictionary containing the answer returned
                 by the DocumentQA service.
             Raises:
                 Exception: When the retries hit maximum (8) times and nothing was returned.
     """
 
     def __call__(self, document: str, query: str):
-        print(f"[DocumentQA] running query against document with {len(document)} characters")
+        print(
+            f"[DocumentQA] running query against document with {len(document)} characters"
+        )
         patience = 8
         count = 0
         while count < patience:
             try:
                 url = "https://api.blazon.ai/blazon/documentqa"
-                headers = {"Content-type": "application/json", "api-key": CONFIG.api_key}
+                headers = {
+                    "Content-type": "application/json",
+                    "api-key": CONFIG.api_key,
+                }
                 payload = {
                     "document": document,
                     "query": query,
                 }
                 resp = requests.post(url=url, headers=headers, json=payload)
                 return resp.json()
             except:
                 sleep_duration = 2.0**count
                 print(f"retrying after sleeping for {sleep_duration:.2f}")
                 count += 1
                 time.sleep(sleep_duration)
         raise Exception("[DocumentQA] failed after hitting max retries")
 
     async def run_async(self, document: str, query: str, session=None):
-        print(f"[DocumentQA] running query against document with {len(document)} characters")
+        print(
+            f"[DocumentQA] running query against document with {len(document)} characters"
+        )
         patience = 8
         count = 0
         while count < patience:
             try:
                 url = "https://api.blazon.ai/blazon/documentqa"
                 if session is None:
                     async with aiohttp.ClientSession(
                         connector=aiohttp.TCPConnector(ssl=False)
                     ) as session:
-                        return await self.run_async(document=document, query=query, session=session)
-                headers = {"Content-type": "application/json", "api-key": CONFIG.api_key}
+                        return await self.run_async(
+                            document=document, query=query, session=session
+                        )
+                headers = {
+                    "Content-type": "application/json",
+                    "api-key": CONFIG.api_key,
+                }
                 payload = {
                     "document": document,
                     "query": query,
                 }
                 async with session.post(url, headers=headers, json=payload) as resp:
                     response = await resp.json()
                     try:
@@ -133,19 +150,24 @@
 
     def __call__(self, document: str):
         patience = 8
         count = 0
         while count < patience:
             try:
                 url = "https://api.blazon.ai/blazon/summarize"
-                headers = {"Content-type": "application/json", "api-key": CONFIG.api_key}
+                headers = {
+                    "Content-type": "application/json",
+                    "api-key": CONFIG.api_key,
+                }
                 payload = {
                     "document": document,
                 }
-                print(f"[Summarize] running query against document with {len(document)} characters")
+                print(
+                    f"[Summarize] running query against document with {len(document)} characters"
+                )
                 resp = requests.post(url=url, headers=headers, json=payload)
                 return resp.json()
             except:
                 sleep_duration = 2.0**count
                 print(f"retrying after sleeping for {sleep_duration:.2f}")
                 count += 1
                 time.sleep(sleep_duration)
@@ -158,19 +180,24 @@
             try:
                 url = "https://api.blazon.ai/blazon/summarize"
                 if session is None:
                     async with aiohttp.ClientSession(
                         connector=aiohttp.TCPConnector(ssl=False)
                     ) as session:
                         return await self.run_async(document=document, session=session)
-                headers = {"Content-type": "application/json", "api-key": CONFIG.api_key}
+                headers = {
+                    "Content-type": "application/json",
+                    "api-key": CONFIG.api_key,
+                }
                 payload = {
                     "document": document,
                 }
-                print(f"[Summarize] running query against document with {len(document)} characters")
+                print(
+                    f"[Summarize] running query against document with {len(document)} characters"
+                )
                 async with session.post(url, headers=headers, json=payload) as resp:
                     response = await resp.json()
                     try:
                         return response
                     except Exception as e:
                         print(f"caught exception={e}")
                         print(f"bad response={response}")
@@ -179,30 +206,105 @@
                 sleep_duration = 2.0**count
                 print(f"retrying after sleeping for {sleep_duration:.2f}")
                 count += 1
                 time.sleep(sleep_duration)
         raise Exception("[Summarize] failed after hitting max retries")
 
 
-def flatten_model(m: Union[ModelMetaclass, str, bool, float, int]) -> Dict[Any, Any]:
-    if hasattr(m, "__dict__"):
-        if m.__dict__.get("_name") == "List":
-            return [flatten_model(m.__args__[0])]
-    if isinstance(m, ModelMetaclass) or is_dataclass(m):
-        return {k: flatten_model(v) for k, v in m.__annotations__.items()}
+StructuredSchema: TypeAlias = Any
+
+
+def flatten_model(m: Type, path: list[str] = []) -> StructuredSchema:
+    """Converts the given type m to a structured schema.
+
+    Args:
+        * m (Type): The type to be converted.
+        * path (list[str], optional): The path to the current type,
+          used for more helpful diagnostic messages saying where
+          the conversion failed. Defaults to [].
+    """
+    orig = typing.get_origin(m)
+    if m == list or orig == list:
+        args = typing.get_args(m)
+        if len(args) != 1:
+            p = ".".join(path)
+            raise TypeError(
+                f"can't deduce list type arg for {m} at {p}, please provide a type annotation to list.",
+                path,
+            )
+        t = flatten_model(args[0])
+        return [t]
+    elif isinstance(m, ModelMetaclass):
+        fields: dict[str, ModelField] = m.__fields__ # type: ignore
+        return {
+            k: flatten_model(f.annotation, path=path + [k]) for k, f in fields.items()
+        }
+    elif is_dataclass(m):
+        return {
+            f.name: flatten_model(f.type, path=path + [f.name])
+            for f in dataclasses.fields(m)
+        }
     elif m == str:
         return "string"
     elif m == bool:
         return "bool"
     elif m == float:
         return "float"
     elif m == int:
         return "int"
     else:
-        raise Exception(f"unsupported datatype={m}")
+        p = ".".join(path)
+        raise TypeError(
+            f"unsupported datatype={m} at {p}\nPlease make sure that all fields are annotated with a bool, int, float, str or a dataclass, list, or pydantic BaseModel. If you need other types supported, let us know!"
+        )
+
+
+def to_dict(obj: Any) -> Any:
+    if isinstance(obj, BaseModel):
+        return obj.dict()
+    elif is_dataclass(obj):
+        return dataclasses.asdict(obj)
+    elif isinstance(obj, list):
+        return [to_dict(o) for o in obj]
+    elif isinstance(obj, dict):
+        return {k: to_dict(v) for k, v in obj.items()}
+    elif isinstance(obj, (str, bool, float, int)):
+        return obj
+    else:
+        raise TypeError(f"unsupported datatype={obj}")
+
+
+T = TypeVar("T")
+
+
+def of_dict(t: Type[T], d: Any) -> T:
+    if isinstance(t, ModelMetaclass):
+        assert isinstance(d, dict)
+        return t.parse_obj(d)
+    elif is_dataclass(t):
+        assert isinstance(d, dict)
+        return dacite.from_dict(t, d)  # type: ignore
+    elif t == list or typing.get_origin(t) == list:
+        assert isinstance(d, list)
+        args = typing.get_args(t)
+        if len(args)!= 1:
+            return d # type: ignore
+        (arg,) = args
+        return [of_dict(arg, o) for o in d]  # type: ignore
+    elif t == dict:
+        (kt, vt) = typing.get_args(t)
+        assert isinstance(d, dict)
+        assert kt in [str, int]
+        return {of_dict(kt, k): of_dict(vt, v) for k, v in d.items()}  # type: ignore
+    elif t in [str, int, float, bool]:
+        assert isinstance(d, t)
+        return d
+    else:
+        raise TypeError(f"unsupported datatype={t}")
+
 
 @dataclass
 class Structured(CapabilityBase):
     """
     `Structured` class allows making requests to the multi API for structured tasks. The class extends CapabilityBase which provides required functionality to interact with multi API. Structured tasks are tasks with specific input and output specs with a natural language instruction.
 
     Attributes:
@@ -211,74 +313,71 @@
 
     Methods:
         __call__(self, input_spec: ModelMetaclass, output_spec: ModelMetaclass, instructions: str, input: BaseModel) -> Union[output_spec, BaseModel]: Calls the API by sending a payload within a request object. Returns output_spec object if output_spec is ModelMetaclass or if it is an instance of a BaseModel.
 
         async run_async(self, input_spec: ModelMetaclass, output_spec: ModelMetaclass, instructions: str, input: BaseModel, session=None) -> Union[output_spec, BaseModel]: Calls the API asynchronously. Returns output_spec object if output_spec is ModelMetaclass or if it is an instance of a BaseModel.
     """
 
-    headers: Dict[Any, Any] = field(
-        default_factory=lambda: {"Content-type": "application/json", "api-key": CONFIG.api_key}
+    headers: dict = field(
+        default_factory=lambda: {
+            "Content-type": "application/json",
+            "api-key": CONFIG.api_key,
+        }
     )
     url: str = "https://api.blazon.ai/blazon/structured"
 
     def __call__(
         self,
         input_spec: ModelMetaclass,
         output_spec: ModelMetaclass,
         instructions: str,
-        input: BaseModel,
+        input: Any,
     ):
         payload = dict(
             input_spec=flatten_model(input_spec),
             output_spec=flatten_model(output_spec),
             instructions=instructions,
-            input=dataclasses.asdict(input) if is_dataclass(input) else input.dict(),
+            input=to_dict(input),
         )
         r = requests.post(self.url, headers=self.headers, json=payload)
-        print("R: ", r)
+        r.raise_for_status()
+        logger.debug("R: ", r)
         result = r.json()["output"]
-        return (
-            output_spec.parse_obj(result)
-            if isinstance(output_spec, ModelMetaclass)
-            else dacite.from_dict(output_spec, result)
-        )
+        return of_dict(output_spec, result)
 
     async def run_async(
         self,
         input_spec: ModelMetaclass,
         output_spec: ModelMetaclass,
         instructions: str,
         input: BaseModel,
         session=None,
     ):
         payload = dict(
             input_spec=flatten_model(input_spec),
             output_spec=flatten_model(output_spec),
-            input=dataclasses.asdict(input) if is_dataclass(input) else input.dict(),
+            input=to_dict(input),
             instructions=instructions,
         )
         if session is None:
-            async with aiohttp.ClientSession(connector=aiohttp.TCPConnector(ssl=False)) as session:
-                async with session.post(self.url, headers=self.headers, json=payload) as resp:
-
+            async with aiohttp.ClientSession(
+                connector=aiohttp.TCPConnector(ssl=False)
+            ) as session:
+                async with session.post(
+                    self.url, headers=self.headers, json=payload
+                ) as resp:
                     result = await resp.json()
                     result = result["output"]
-                    return (
-                        output_spec.parse_obj(result)
-                        if isinstance(output_spec, ModelMetaclass)
-                        else dacite.from_dict(output_spec, result)
-                    )
+                    return of_dict(output_spec, result)
         else:
-            async with session.post(self.url, headers=self.headers, json=payload) as resp:
+            async with session.post(
+                self.url, headers=self.headers, json=payload
+            ) as resp:
                 result = (await resp.json())["output"]
-                return (
-                    output_spec.parse_obj(result)
-                    if isinstance(output_spec, ModelMetaclass)
-                    else dacite.from_dict(output_spec, result)
-                )
+                return of_dict(output_spec, result)
 
 
 _CAPABILITIES = {
     "multi/structured": Structured(),
     "multi/document_qa": DocumentQA(),
     "multi/summarize": Summarize(),
     "blazon/structured": Structured(),
```

### Comparing `capabilities-0.1.0/capabilities/example.py` & `capabilities-0.1.2/capabilities/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,18 @@
 Write a bullet-pointed summary of the `text` as a list of supported bullet points, each with a `bullet_point` summarizing a passage from the `text` called `supporting_text`. Each `supporting_text` should be a passage of text extracted verbatim from `text` which supports its corresponding `bullet_point`. The list should contain no more than five (5) items.
     """
 
     inp = Document(text=EXAMPLE_PASSAGE)
 
     # synthesis call
     document_summary = Capability("blazon/structured")(
-        input_spec=Document, output_spec=DocumentSummary, input=inp, instructions=instructions
+        input_spec=Document,
+        output_spec=DocumentSummary,
+        input=inp,
+        instructions=instructions,
     )
 
     for x in document_summary.supportedBulletPoints:
         print(f"claim: {x.bullet_point}")
         print(f'    support: """{x.supporting_text}"""\n')
 
 
@@ -220,15 +223,17 @@
         text="Understand: I'll slip quietly away through twilit meadows with only this one dream - you come too."
     )
 
     # provide some instructions
     instructions = "Given the input `text`, produce a `french_translation` which translates the `text` into French. Also produce a word-level translation called `word_translations`, which is a list of (english word, french transliteration) pairs."
 
     # print the task to console
-    result = Capability("blazon/structured")(InputText, TranslationOutput, instructions, inp)
+    result = Capability("blazon/structured")(
+        InputText, TranslationOutput, instructions, inp
+    )
     import json
 
     print(json.dumps(result.dict(), indent=2))
 
 
 def example_summarize():
     print(Capability("blazon/summarize")(EXAMPLE_PASSAGE))
@@ -285,16 +290,14 @@
 
     input: SynthesisRequest = SynthesisRequest(
         goal="Retrieve the first three paragraphs",
         url="https://en.wikipedia.org/wiki/Selenium_(software)",
         title="Google",
     )
 
-    
-
     print(
         Capability("blazon/structured")(
             SynthesisRequest, SynthesisResponse, instructions, input=input
         ).dict()
     )
 
 
@@ -312,8 +315,9 @@
         BulletPoints(bullet_points=bullet_points),
     ).summary
 
 
 # example usage: python -m capabilities.example example_translation
 if __name__ == "__main__":
     import sys
+
     fire.Fire(component=locals()[sys.argv[1]], command=sys.argv[2:])
```

### Comparing `capabilities-0.1.0/capabilities/search/hf.py` & `capabilities-0.1.2/capabilities/search/hf.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.1.0/capabilities/search/loader.py` & `capabilities-0.1.2/capabilities/search/loader.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.1.0/capabilities/search/nomic_index.py` & `capabilities-0.1.2/capabilities/search/nomic_index.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,14 +42,18 @@
 
         Args:
           - project_name (str): name of the nomic project to use
           - embedding_model (EmbeddingModel, optional): the model to use for the index. Default is SentenceTransformer miniLM.
           - reset_project_if_exists (bool = False): whether to reset the project if it already exists. Defaults to True.
           - items (Iterable[T], optional): an iterable of items that will be used to update the index. If this is set, equivalent to calling `index.update(items)` after initialization.
         """
+        if embedding_model is None:
+            from .hf import STEmbeddingModel
+
+            embedding_model = STEmbeddingModel()
         self.embedding_model = embedding_model
         self.modality = "text" if embedding_model is None else "embedding"
         self.project = atlas.AtlasProject(
             name=project_name,
             **kwargs,
             modality=self.modality,
             unique_id_field="id",
@@ -92,18 +96,26 @@
                 name="main-index", colorable_fields=["item_id"]
             )
         else:
             return self.project.indices[0].projections[0]  # idk
 
     def update(self, items: Iterable[T]):
         items = list(items)
-        self.items.update({item.id: item for item in items})
+        for item in items:
+            if item.id in self.items:
+                raise RuntimeError(f"Item {item.id} already exists in the index.")
+            self.items[item.id] = item
         if self.embedding_model is not None:
             chunks = list(get_chunks(items, self.embedding_model))
-            self.chunks.update({c.unique_id: c for c in chunks})
+            for chunk in chunks:
+                if chunk.unique_id in self.chunks:
+                    raise RuntimeError(
+                        f"Chunk {chunk.unique_id} already exists in the index."
+                    )
+                self.chunks[chunk.unique_id] = chunk
             texts = [chunk.text for chunk in chunks]
             embeddings = self.embedding_model.encode(texts)
             assert isinstance(embeddings, np.ndarray)
             assert len(embeddings.shape) == 2
             self.project.add_embeddings(
                 data=[c.dict() for c in chunks],
                 embeddings=embeddings,
```

### Comparing `capabilities-0.1.0/capabilities/search/oai.py` & `capabilities-0.1.2/capabilities/search/oai.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.1.0/capabilities/search/search_index.py` & `capabilities-0.1.2/capabilities/search/search_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,17 +141,14 @@
         """Gets the item_id of the found item."""
         return self.item.id
 
     def get_text(self) -> str:
         """Gets the chunk text of the found item."""
         fulltext = self.item.get_text()
         if self.substring_range is not None:
-            assert (
-                self.chunk_id is not None
-            ), "chunk_id was not set but substring_range was"
             r = self.substring_range
             return fulltext[r.start : r.stop]
         else:
             return fulltext
 
 
 class AbstractSearchIndex(Generic[T], ABC):
```

### Comparing `capabilities-0.1.0/capabilities/search/simple_vector_index.py` & `capabilities-0.1.2/capabilities/search/simple_vector_index.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.1.0/capabilities/search/types.py` & `capabilities-0.1.2/capabilities/search/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         return digest(f"Chunk({self.item_id}, {self.chunk_id})")[:36]
 
     def dict(self):
         """Dict for feeding into databases like nomic."""
         return {
             "id": self.unique_id,
             "item_id": self.item_id,
-            "chunk_id": self.chunk_id,
+            "chunk_id": self.chunk_id if self.chunk_id is not None else "none",
             "text": self.text,
         }
 
 
 class TextItem(ABC):
     """A TextItem is anything that can be converted to text and embedded.
```

### Comparing `capabilities-0.1.0/capabilities/search/util.py` & `capabilities-0.1.2/capabilities/search/util.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.1.0/capabilities/util.py` & `capabilities-0.1.2/capabilities/util.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.1.0/capabilities.egg-info/PKG-INFO` & `capabilities-0.1.2/capabilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capabilities
-Version: 0.1.0
+Version: 0.1.2
 Summary: Build trusted, faster, and more powerful applications with the Blazon Capabilities API.
 Author-email: Blazon AI <support@blazon.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `capabilities-0.1.0/capabilities.egg-info/SOURCES.txt` & `capabilities-0.1.2/capabilities.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 capabilities/__init__.py
 capabilities/config.py
 capabilities/core.py
+capabilities/dec.py
 capabilities/example.py
 capabilities/util.py
 capabilities.egg-info/PKG-INFO
 capabilities.egg-info/SOURCES.txt
 capabilities.egg-info/dependency_links.txt
 capabilities.egg-info/requires.txt
 capabilities.egg-info/top_level.txt
```

### Comparing `capabilities-0.1.0/pyproject.toml` & `capabilities-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools==63.4.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "capabilities"
-version = "0.1.0"
+version = "0.1.2"
 authors = [
   { name="Blazon AI", email="support@blazon.ai" },
 ]
 description = "Build trusted, faster, and more powerful applications with the Blazon Capabilities API."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```


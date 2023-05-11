# Comparing `tmp/pons-0.5.1.tar.gz` & `tmp/pons-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pons-0.5.1.tar", last modified: Mon Nov 14 23:04:57 2022, max compression
+gzip compressed data, was "pons-0.6.0.tar", last modified: Thu May 11 22:24:26 2023, max compression
```

## Comparing `pons-0.5.1.tar` & `pons-0.6.0.tar`

### file list

```diff
@@ -1,30 +1,39 @@
--rw-r--r--   0 bogdan     (501) staff       (20)     1055 2022-02-27 04:36:26.118572 pons-0.5.1/LICENSE.md
--rw-r--r--   0 bogdan     (501) staff       (20)     1051 2022-06-06 01:00:07.574013 pons-0.5.1/README.md
--rw-r--r--   0 bogdan     (501) staff       (20)      617 2022-08-25 00:47:15.624837 pons-0.5.1/pons/__init__.py
--rw-r--r--   0 bogdan     (501) staff       (20)    18495 2022-11-10 22:43:13.488169 pons-0.5.1/pons/_abi_types.py
--rw-r--r--   0 bogdan     (501) staff       (20)    29113 2022-11-11 23:30:57.748641 pons-0.5.1/pons/_client.py
--rw-r--r--   0 bogdan     (501) staff       (20)     7317 2022-08-17 18:47:24.905391 pons-0.5.1/pons/_contract.py
--rw-r--r--   0 bogdan     (501) staff       (20)    27003 2022-11-12 00:16:34.111963 pons-0.5.1/pons/_contract_abi.py
--rw-r--r--   0 bogdan     (501) staff       (20)    19284 2022-08-17 18:47:24.907290 pons-0.5.1/pons/_entities.py
--rw-r--r--   0 bogdan     (501) staff       (20)     5431 2022-08-17 18:47:24.908078 pons-0.5.1/pons/_provider.py
--rw-r--r--   0 bogdan     (501) staff       (20)     1227 2022-08-17 18:47:24.908882 pons-0.5.1/pons/_signer.py
--rw-r--r--   0 bogdan     (501) staff       (20)      757 2022-04-24 22:22:36.234257 pons-0.5.1/pons/abi.py
--rw-r--r--   0 bogdan     (501) staff       (20)        0 2022-04-23 23:56:47.869339 pons-0.5.1/pons/py.typed
--rw-r--r--   0 bogdan     (501) staff       (20)      948 2022-11-14 23:00:57.444902 pons-0.5.1/pyproject.toml
--rw-r--r--   0 bogdan     (501) staff       (20)     2399 2022-06-05 01:05:34.948636 pons-0.5.1/tests/TestClient.sol
--rw-r--r--   0 bogdan     (501) staff       (20)      939 2022-05-25 05:17:34.628636 pons-0.5.1/tests/TestContract.sol
--rw-r--r--   0 bogdan     (501) staff       (20)     2045 2022-05-29 07:42:02.336089 pons-0.5.1/tests/TestContractFunctionality.sol
--rw-r--r--   0 bogdan     (501) staff       (20)      343 2022-03-06 23:50:17.744670 pons-0.5.1/tests/__init__.py
--rw-r--r--   0 bogdan     (501) staff       (20)      640 2022-05-24 03:06:04.493486 pons-0.5.1/tests/compile.py
--rw-r--r--   0 bogdan     (501) staff       (20)      585 2022-06-05 01:05:34.949279 pons-0.5.1/tests/conftest.py
--rw-r--r--   0 bogdan     (501) staff       (20)    10417 2022-08-13 05:24:45.008568 pons-0.5.1/tests/provider.py
--rw-r--r--   0 bogdan     (501) staff       (20)     2648 2022-09-14 20:33:08.949272 pons-0.5.1/tests/provider_server.py
--rw-r--r--   0 bogdan     (501) staff       (20)    11699 2022-06-05 06:14:54.793780 pons-0.5.1/tests/test_abi_types.py
--rw-r--r--   0 bogdan     (501) staff       (20)    34381 2022-09-14 20:33:08.950025 pons-0.5.1/tests/test_client.py
--rw-r--r--   0 bogdan     (501) staff       (20)     4556 2022-06-05 06:14:54.794938 pons-0.5.1/tests/test_contract.py
--rw-r--r--   0 bogdan     (501) staff       (20)    24687 2022-11-10 23:07:00.081689 pons-0.5.1/tests/test_contract_abi.py
--rw-r--r--   0 bogdan     (501) staff       (20)     5032 2022-11-11 00:21:41.301826 pons-0.5.1/tests/test_contract_functionality.py
--rw-r--r--   0 bogdan     (501) staff       (20)    12100 2022-08-17 18:47:24.909675 pons-0.5.1/tests/test_entities.py
--rw-r--r--   0 bogdan     (501) staff       (20)     6663 2022-09-14 20:33:08.950443 pons-0.5.1/tests/test_provider.py
--rw-r--r--   0 bogdan     (501) staff       (20)     1209 2022-06-05 01:05:34.954137 pons-0.5.1/tests/test_signer.py
--rw-------   0 bogdan     (501) staff       (20)     1386 2022-11-14 23:04:57.451518 pons-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      177 2022-04-23 23:56:47.860000 pons-0.6.0/.coveragerc
+-rw-r--r--   0        0        0     1055 2022-02-27 04:36:26.110000 pons-0.6.0/LICENSE.md
+-rw-r--r--   0        0        0     1051 2022-06-06 01:00:07.570000 pons-0.6.0/README.md
+-rw-r--r--   0        0        0      638 2022-02-28 05:30:25.300000 pons-0.6.0/docs/Makefile
+-rw-r--r--   0        0        0     4503 2022-08-06 01:36:45.100000 pons-0.6.0/docs/api.rst
+-rw-r--r--   0        0        0     4366 2023-05-11 22:23:05.214707 pons-0.6.0/docs/changelog.rst
+-rw-r--r--   0        0        0     2565 2023-02-05 09:02:39.350000 pons-0.6.0/docs/conf.py
+-rw-r--r--   0        0        0     3177 2022-09-14 20:33:08.940000 pons-0.6.0/docs/index.rst
+-rw-r--r--   0        0        0     6890 2022-11-10 22:51:25.580000 pons-0.6.0/docs/tutorial.rst
+-rw-r--r--   0        0        0      164 2023-01-21 08:19:29.290000 pons-0.6.0/mypy.ini
+-rw-r--r--   0        0        0      617 2022-08-25 00:47:15.620000 pons-0.6.0/pons/__init__.py
+-rw-r--r--   0        0        0    18449 2023-05-07 07:14:33.518659 pons-0.6.0/pons/_abi_types.py
+-rw-r--r--   0        0        0    29113 2022-11-11 23:30:57.740000 pons-0.6.0/pons/_client.py
+-rw-r--r--   0        0        0     7317 2022-08-17 18:47:24.899999 pons-0.6.0/pons/_contract.py
+-rw-r--r--   0        0        0    27975 2023-05-07 07:14:33.518858 pons-0.6.0/pons/_contract_abi.py
+-rw-r--r--   0        0        0    19283 2023-02-05 00:19:21.360000 pons-0.6.0/pons/_entities.py
+-rw-r--r--   0        0        0     5431 2022-08-17 18:47:24.899999 pons-0.6.0/pons/_provider.py
+-rw-r--r--   0        0        0     1227 2022-08-17 18:47:24.899999 pons-0.6.0/pons/_signer.py
+-rw-r--r--   0        0        0      757 2022-04-24 22:22:36.230000 pons-0.6.0/pons/abi.py
+-rw-r--r--   0        0        0        0 2022-04-23 23:56:47.860000 pons-0.6.0/pons/py.typed
+-rw-r--r--   0        0        0     1215 2023-05-11 22:22:15.121564 pons-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       26 2022-04-25 23:59:46.280000 pons-0.6.0/pytest.ini
+-rw-r--r--   0        0        0     2399 2022-06-05 01:05:34.940000 pons-0.6.0/tests/TestClient.sol
+-rw-r--r--   0        0        0      939 2022-05-25 05:17:34.620000 pons-0.6.0/tests/TestContract.sol
+-rw-r--r--   0        0        0     2045 2022-05-29 07:42:02.330000 pons-0.6.0/tests/TestContractFunctionality.sol
+-rw-r--r--   0        0        0      343 2022-03-06 23:50:17.740000 pons-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      640 2022-05-24 03:06:04.490000 pons-0.6.0/tests/compile.py
+-rw-r--r--   0        0        0      585 2022-06-05 01:05:34.940000 pons-0.6.0/tests/conftest.py
+-rw-r--r--   0        0        0    10942 2023-02-05 00:19:21.180000 pons-0.6.0/tests/provider.py
+-rw-r--r--   0        0        0     2648 2022-09-14 20:33:08.940000 pons-0.6.0/tests/provider_server.py
+-rw-r--r--   0        0        0    11696 2023-02-05 00:19:21.410000 pons-0.6.0/tests/test_abi_types.py
+-rw-r--r--   0        0        0    34366 2023-05-07 07:14:33.519168 pons-0.6.0/tests/test_client.py
+-rw-r--r--   0        0        0     4556 2022-06-05 06:14:54.790000 pons-0.6.0/tests/test_contract.py
+-rw-r--r--   0        0        0    24721 2023-05-07 07:14:33.519340 pons-0.6.0/tests/test_contract_abi.py
+-rw-r--r--   0        0        0     5030 2023-02-05 00:19:21.100000 pons-0.6.0/tests/test_contract_functionality.py
+-rw-r--r--   0        0        0    12097 2023-02-05 00:19:21.350000 pons-0.6.0/tests/test_entities.py
+-rw-r--r--   0        0        0     6662 2023-02-05 00:19:21.149999 pons-0.6.0/tests/test_provider.py
+-rw-r--r--   0        0        0     1209 2022-06-05 01:05:34.950000 pons-0.6.0/tests/test_signer.py
+-rw-r--r--   0        0        0     1386 1970-01-01 00:00:00.000000 pons-0.6.0/PKG-INFO
```

### Comparing `pons-0.5.1/LICENSE.md` & `pons-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pons-0.5.1/README.md` & `pons-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pons-0.5.1/pons/__init__.py` & `pons-0.6.0/pons/__init__.py`

 * *Files identical despite different names*

### Comparing `pons-0.5.1/pons/_abi_types.py` & `pons-0.6.0/pons/_abi_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,23 +26,23 @@
 """
 
 
 def encode_typed(types: Iterable[str], args: Iterable[ABIType]) -> bytes:
     # ``eth_abi.encode()`` does not have type annotations.
     # This is a typed wrapper (easier than making custom stubs).
     # Remove when typing is added in ``eth_abi``.
-    encoded = eth_abi.encode(types, args)  # type: ignore
-    return cast(bytes, encoded)
+    encoded = eth_abi.encode(types, args)
+    return encoded
 
 
 def decode_typed(types: Iterable[str], data: bytes) -> Tuple[ABIType, ...]:
     # ``eth_abi.decode()`` does not have type annotations.
     # This is a typed wrapper (easier than making custom stubs).
     # Remove when typing is added in ``eth_abi``.
-    decoded = eth_abi.decode(types, data)  # type: ignore
+    decoded = eth_abi.decode(types, data)
     return cast(Tuple[ABIType, ...], decoded)
 
 
 class Type(ABC):
     """The base type for Solidity types."""
 
     @property
@@ -528,15 +528,14 @@
     return encode_typed(
         [tp.canonical_form for tp in types],
         tuple(tp._normalize(arg) for tp, arg in zip(types, args)),
     )
 
 
 def decode_args(types: Iterable[Type], data: bytes) -> Tuple[ABIType, ...]:
-
     canonical_types = [tp.canonical_form for tp in types]
     try:
         values = decode_typed(canonical_types, data)
     except DecodingError as exc:
         # wrap possible `eth_abi` errors
         signature = "(" + ",".join(canonical_types) + ")"
         message = (
```

### Comparing `pons-0.5.1/pons/_client.py` & `pons-0.6.0/pons/_client.py`

 * *Files identical despite different names*

### Comparing `pons-0.5.1/pons/_contract.py` & `pons-0.6.0/pons/_contract.py`

 * *Files identical despite different names*

### Comparing `pons-0.5.1/pons/_contract_abi.py` & `pons-0.6.0/pons/_contract_abi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from abc import ABC, abstractmethod
 from functools import cached_property
 import inspect
 from itertools import chain
+from keyword import iskeyword
 from typing import (
     Any,
     AbstractSet,
     Iterable,
     List,
     Dict,
     Optional,
@@ -20,24 +21,35 @@
 
 from . import abi
 from ._abi_types import Type, dispatch_types, dispatch_type, encode_args, decode_args, keccak
 from ._entities import LogTopic, LogEntry
 from ._provider import JSON
 
 
+# We are using the `inspect` machinery to bind arguments to parameters.
+# From Py3.11 on it does not allow parameter names to coincide with keywords,
+# so we have to escape them.
+# This can be avoided if we write our own `inspect.Signature` implementation.
+def make_name_safe(name: str) -> str:
+    if iskeyword(name):
+        return name + "_"
+    else:
+        return name
+
+
 class Signature:
     """
     Generalized signature of either inputs or outputs of a method.
     """
 
     def __init__(self, parameters: Union[Mapping[str, Type], Sequence[Type]]):
         if isinstance(parameters, Mapping):
             self._signature = inspect.Signature(
                 parameters=[
-                    inspect.Parameter(name, inspect.Parameter.POSITIONAL_OR_KEYWORD)
+                    inspect.Parameter(make_name_safe(name), inspect.Parameter.POSITIONAL_OR_KEYWORD)
                     for name, tp in parameters.items()
                 ]
             )
             self._types = list(parameters.values())
             self._named_parameters = True
         else:
             self._signature = inspect.Signature(
@@ -99,14 +111,16 @@
 
 class EventSignature:
     """
     A signature representing the constructor of an event (that is, its fields).
     """
 
     def __init__(self, parameters: Mapping[str, Type], indexed: AbstractSet[str]):
+        parameters = {make_name_safe(name): val for name, val in parameters.items()}
+        indexed = {make_name_safe(name) for name in indexed}
         self._signature = inspect.Signature(
             parameters=[
                 inspect.Parameter(name, inspect.Parameter.POSITIONAL_OR_KEYWORD)
                 for name, tp in parameters.items()
                 if name in indexed
             ]
         )
@@ -230,14 +244,19 @@
         input_bytes = self.inputs.encode(*args, **kwargs)
         return self.selector + input_bytes
 
 
 class Constructor:
     """
     Contract constructor.
+
+    .. note::
+
+       If the name of a parameter given to the constructor matches a Python keyword,
+       ``_`` will be appended to it.
     """
 
     inputs: Signature
     """Input signature."""
 
     payable: bool
     """Whether this method is marked as payable"""
@@ -277,14 +296,19 @@
     def __str__(self) -> str:
         return f"constructor{self.inputs} " + ("payable" if self.payable else "nonpayable")
 
 
 class ReadMethod(Method):
     """
     A non-mutating contract method.
+
+    .. note::
+
+       If the name of a parameter (input or output) given to the constructor
+       matches a Python keyword, ``_`` will be appended to it.
     """
 
     outputs: Signature
     """Method's output signature."""
 
     @classmethod
     def from_json(cls, method_entry: Dict[str, Any]) -> "ReadMethod":
@@ -314,15 +338,14 @@
 
     def __init__(
         self,
         name: str,
         inputs: Union[Mapping[str, Type], Sequence[Type]],
         outputs: Union[Mapping[str, Type], Sequence[Type], Type],
     ):
-
         self._name = name
         self._inputs = Signature(inputs)
 
         if isinstance(outputs, Type):
             outputs = [outputs]
             self._single_output = True
         else:
@@ -356,14 +379,19 @@
     def __str__(self) -> str:
         return f"function {self.name}{self.inputs} returns {self.outputs}"
 
 
 class WriteMethod(Method):
     """
     A mutating contract method.
+
+    .. note::
+
+       If the name of a parameter given to the constructor matches a Python keyword,
+       ``_`` will be appended to it.
     """
 
     payable: bool
     """Whether this method is marked as payable"""
 
     @classmethod
     def from_json(cls, method_entry: Dict[str, Any]) -> "WriteMethod":
@@ -373,30 +401,27 @@
         if method_entry["type"] != "function":
             raise ValueError(
                 "WriteMethod object must be created from a JSON entry with type='function'"
             )
 
         name = method_entry["name"]
         inputs = dispatch_types(method_entry["inputs"])
-        if "outputs" in method_entry and method_entry["outputs"]:
-            raise ValueError("Mutating method's JSON entry cannot have non-empty `outputs`")
         if method_entry["stateMutability"] not in ("nonpayable", "payable"):
             raise ValueError(
                 "Mutating method's JSON entry state mutability must be `nonpayable` or `payable`"
             )
         payable = method_entry["stateMutability"] == "payable"
         return cls(name=name, inputs=inputs, payable=payable)
 
     def __init__(
         self,
         name: str,
         inputs: Union[Mapping[str, Type], Sequence[Type]],
         payable: bool = False,
     ):
-
         self._name = name
         self._inputs = Signature(inputs)
         self.payable = payable
 
     @property
     def name(self) -> str:
         return self._name
@@ -414,14 +439,19 @@
     def __str__(self) -> str:
         return f"function {self.name}{self.inputs} " + ("payable" if self.payable else "nonpayable")
 
 
 class Event:
     """
     A contract event.
+
+    .. note::
+
+       If the name of a field given to the constructor matches a Python keyword,
+       ``_`` will be appended to it.
     """
 
     @classmethod
     def from_json(cls, event_entry: Dict[str, Any]) -> "Event":
         """
         Creates this object from a JSON ABI method entry.
         """
@@ -733,15 +763,14 @@
         read = []
         write = []
         methods = set()
         events = {}
         errors = {}
 
         for entry in json_abi:
-
             if entry["type"] == "constructor":
                 if constructor:
                     raise ValueError("JSON ABI contains more than one constructor declarations")
                 constructor = Constructor.from_json(entry)
 
             elif entry["type"] == "function":
                 if entry["name"] in methods:
@@ -800,15 +829,14 @@
         fallback: Optional[Fallback] = None,
         receive: Optional[Receive] = None,
         read: Optional[Iterable[ReadMethod]] = None,
         write: Optional[Iterable[WriteMethod]] = None,
         events: Optional[Iterable[Event]] = None,
         errors: Optional[Iterable[Error]] = None,
     ):
-
         if constructor is None:
             constructor = Constructor(inputs=[])
 
         self.fallback = fallback
         self.receive = receive
         self.constructor = constructor
         self.read = Methods({method.name: method for method in (read or [])})
```

### Comparing `pons-0.5.1/pons/_entities.py` & `pons-0.6.0/pons/_entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -559,15 +559,14 @@
     """Hash of the block where this log was in."""
 
     block_number: int
     """The block number where this log was."""
 
     @classmethod
     def rpc_decode(cls, val: ResponseDict) -> "LogEntry":
-
         topics = val["topics"]
         if not isinstance(topics, Iterable):
             raise RPCDecodingError(f"`topics` in a log entry must be an iterable, got {topics}")
 
         return cls(
             removed=rpc_decode_bool(val["removed"]),
             log_index=rpc_decode_quantity(val["logIndex"]),
```

### Comparing `pons-0.5.1/pons/_provider.py` & `pons-0.6.0/pons/_provider.py`

 * *Files identical despite different names*

### Comparing `pons-0.5.1/pons/_signer.py` & `pons-0.6.0/pons/_signer.py`

 * *Files identical despite different names*

### Comparing `pons-0.5.1/pons/abi.py` & `pons-0.6.0/pons/abi.py`

 * *Files identical despite different names*

### Comparing `pons-0.5.1/pyproject.toml` & `pons-0.6.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "pons"
-version = "0.5.1"
+version = "0.6.0"
 description = "Async RPC client for Ethereum"
 authors = [
     { name = "Bogdan Opanchuk", email = "bogdan@opanchuk.net" },
 ]
 dependencies = [
     "httpx>=0.22",
     "eth-account>=0.6",
     "eth-utils>=2",
-    "eth-abi>=3",
+    "eth-abi>=4",
     "anyio>=3",
     "setuptools",
 ]
 requires-python = ">=3.8"
 license = "MIT"
 readme = "README.md"
 
@@ -23,35 +23,52 @@
 [project.optional-dependencies]
 tests = [
     "pytest>=6",
     "trio>=0.19.0",
     "pytest-trio",
     "pytest-cov",
     "py-solc-x>=1",
-    "eth-tester[pyevm]==0.7.0b1",
+    "eth-tester[pyevm]==0.8.0b3",
     "starlette",
     "hypercorn",
+    "mypy-extensions==0.4.4",
 ]
 docs = [
     "sphinx>=4",
     "furo",
     "sphinxcontrib-trio",
+    "setuptools-scm",
 ]
 lint = [
-    "mypy>=0.941",
+    "mypy>=1",
     "trio-typing[mypy]>=0.7.0",
-    "black",
+    "black>=23",
 ]
 
 [tool.black]
 line-length = 100
 target-version = [
     "py38",
 ]
 
-[tool.pdm.dev-dependencies]
+[tool.pdm.version]
+source = "scm"
+
+[tool.pdm.build]
+source-includes = [
+    "tests/*.sol",
+    "tests/*.py",
+    "docs/*.rst",
+    "docs/*.py",
+    "docs/Makefile",
+    ".coveragerc",
+    "mypy.ini",
+    "pytest.ini",
+]
+
+[tool.setuptools_scm]
 
 [build-system]
 requires = [
     "pdm-pep517",
 ]
 build-backend = "pdm.pep517.api"
```

### Comparing `pons-0.5.1/tests/TestClient.sol` & `pons-0.6.0/tests/TestClient.sol`

 * *Files identical despite different names*

### Comparing `pons-0.5.1/tests/TestContract.sol` & `pons-0.6.0/tests/TestContract.sol`

 * *Files identical despite different names*

### Comparing `pons-0.5.1/tests/TestContractFunctionality.sol` & `pons-0.6.0/tests/TestContractFunctionality.sol`

 * *Files identical despite different names*

### Comparing `pons-0.5.1/tests/compile.py` & `pons-0.6.0/tests/compile.py`

 * *Files identical despite different names*

### Comparing `pons-0.5.1/tests/conftest.py` & `pons-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pons-0.5.1/tests/provider.py` & `pons-0.6.0/tests/provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
 
 @contextmanager
 def pyevm_errors_into_rpc_errors():
     try:
         yield
     except TransactionFailed as exc:
-
         assert len(exc.args) == 1  # sanity check in case eth-tester suddenly changes API
         reason = exc.args[0]
 
         if isinstance(reason, Revert):
             # Happens when `require/revert` is called in a mutating method or a constructor.
             assert len(reason.args) == 1
             reason_data = reason.args[0]
@@ -208,23 +207,33 @@
         return normalize_return_value(result)
 
     def eth_get_block_by_hash(self, block_hash: str, with_transactions: bool):
         try:
             result = self._ethereum_tester.get_block_by_hash(
                 block_hash, full_transactions=with_transactions
             )
+            # TODO (#44): major providers still use "miner",
+            # but eth-tester is already using "coinbase". Replacing for now.
+            assert "miner" not in result
+            result["miner"] = result["coinbase"]
+            del result["coinbase"]
         except BlockNotFound:
             return None
         return normalize_return_value(result)
 
     def eth_get_block_by_number(self, block: str, with_transactions: bool):
         try:
             result = self._ethereum_tester.get_block_by_number(
                 rpc_decode_block(block), full_transactions=with_transactions
             )
+            # TODO (#44): major providers still use "miner",
+            # but eth-tester is already using "coinbase". Replacing for now.
+            assert "miner" not in result
+            result["miner"] = result["coinbase"]
+            del result["coinbase"]
         except BlockNotFound:
             return None
         return normalize_return_value(result)
 
     def eth_new_block_filter(self):
         filter_id = self._ethereum_tester.create_block_filter()
         return rpc_encode_quantity(filter_id)
```

### Comparing `pons-0.5.1/tests/provider_server.py` & `pons-0.6.0/tests/provider_server.py`

 * *Files identical despite different names*

### Comparing `pons-0.5.1/tests/test_abi_types.py` & `pons-0.6.0/tests/test_abi_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,14 @@
     assert abi.uint(8)[...][3][...].canonical_form == "uint8[][3][]"
 
     with pytest.raises(TypeError, match="Invalid array size specifier type: float"):
         abi.uint(8)[1.0]
 
 
 def test_normalization_roundtrip():
-
     struct = abi.struct(
         field1=abi.uint(8),
         field2=abi.uint(16)[2],
         field3=abi.address,
         field4=abi.struct(inner1=abi.bool, inner2=abi.string),
     )
 
@@ -254,15 +253,14 @@
     if can_be_decoded:
         assert tp.decode_from_topic(encoded_val) == val
     else:
         assert tp.decode_from_topic(encoded_val) is None
 
 
 def test_encode_to_topic():
-
     # Simple types
 
     check_topic_encode_decode(
         abi.uint(32), 0x12345678, b"\x00" * 28 + (0x12345678).to_bytes(4, "big")
     )
     check_topic_encode_decode(
         abi.int(32), 0x12345678, b"\x00" * 28 + (0x12345678).to_bytes(4, "big")
@@ -327,15 +325,14 @@
     assert decode_args(types, encoded) == args
 
     # empty types/args list
     assert encode_args() == b""
 
 
 def test_decoding_error():
-
     types = [abi.uint(256), abi.uint(256)]
     encoded_bytes = b"\x00" * 31 + b"\x01"  # Only one uint256
 
     expected_message = (
         r"Could not decode the return value with the expected signature \(uint256,uint256\): "
         r"Tried to read 32 bytes.  Only got 0 bytes"
     )
```

### Comparing `pons-0.5.1/tests/test_client.py` & `pons-0.6.0/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,14 @@
     # Non-existent address (which is technically just an unfunded address)
     random_addr = Address(os.urandom(20))
     balance = await session.eth_get_balance(random_addr)
     assert balance == Amount.ether(0)
 
 
 async def test_eth_get_transaction_receipt(test_provider, session, root_signer, another_signer):
-
     test_provider.disable_auto_mine_transactions()
     tx_hash = await session.broadcast_transfer(
         root_signer, another_signer.address, Amount.ether(10)
     )
     receipt = await session.eth_get_transaction_receipt(tx_hash)
     assert receipt is None
 
@@ -123,15 +122,14 @@
     await session.transfer(root_signer, another_signer.address, Amount.ether(10))
     assert await session.eth_get_transaction_count(root_signer.address) == 1
 
 
 async def test_wait_for_transaction_receipt(
     test_provider, session, root_signer, another_signer, autojump_clock
 ):
-
     to_transfer = Amount.ether(10)
     test_provider.disable_auto_mine_transactions()
     tx_hash = await session.broadcast_transfer(root_signer, another_signer.address, to_transfer)
 
     # The receipt won't be available until we mine, so the waiting should time out
     start_time = trio.current_time()
     with pytest.raises(trio.TooSlowError):
@@ -224,38 +222,35 @@
 
 async def test_eth_gas_price(session):
     gas_price = await session.eth_gas_price()
     assert isinstance(gas_price, Amount)
 
 
 async def test_eth_block_number(session, root_signer, another_signer):
-
     await session.transfer(root_signer, another_signer.address, Amount.ether(1))
     await session.transfer(root_signer, another_signer.address, Amount.ether(2))
     await session.transfer(root_signer, another_signer.address, Amount.ether(3))
     block_num = await session.eth_block_number()
 
     block_info = await session.eth_get_block_by_number(block_num - 1, with_transactions=True)
     assert block_info.transactions[0].value == Amount.ether(2)
 
 
 async def test_transfer(session, root_signer, another_signer):
-
     # Regular transfer
     root_balance = await session.eth_get_balance(root_signer.address)
     to_transfer = Amount.ether(10)
     await session.transfer(root_signer, another_signer.address, to_transfer)
     root_balance_after = await session.eth_get_balance(root_signer.address)
     acc1_balance_after = await session.eth_get_balance(another_signer.address)
     assert acc1_balance_after == to_transfer
     assert root_balance - root_balance_after > to_transfer
 
 
 async def test_transfer_custom_gas(session, root_signer, another_signer):
-
     root_balance = await session.eth_get_balance(root_signer.address)
     to_transfer = Amount.ether(10)
 
     # Override gas estimate
     # The standard transfer gas cost is 21000, we're being cautious here.
     await session.transfer(root_signer, another_signer.address, to_transfer, gas=22000)
     root_balance_after = await session.eth_get_balance(root_signer.address)
@@ -265,15 +260,14 @@
 
     # Not enough gas
     with pytest.raises(ProviderError, match="Insufficient gas"):
         await session.transfer(root_signer, another_signer.address, to_transfer, gas=20000)
 
 
 async def test_transfer_failed(test_provider, session, root_signer, another_signer):
-
     # TODO: it would be nice to reproduce the actual situation where this could happen
     # (tranfer was accepted for mining, but failed in the process,
     # and the resulting receipt has a 0 status).
     orig_get_transaction_receipt = test_provider.eth_get_transaction_receipt
 
     def mock_get_transaction_receipt(tx_hash_hex):
         receipt = orig_get_transaction_receipt(tx_hash_hex)
@@ -391,15 +385,14 @@
 
     non_existent = TxHash(b"abcd" * 8)
     tx_info = await session.eth_get_transaction_by_hash(non_existent)
     assert tx_info is None
 
 
 async def test_block_filter(test_provider, session, root_signer, another_signer):
-
     to_transfer = Amount.ether(1)
 
     await session.transfer(root_signer, another_signer.address, to_transfer)
 
     block_filter = await session.eth_new_block_filter()
 
     await session.transfer(root_signer, another_signer.address, to_transfer)
@@ -429,15 +422,14 @@
     test_provider.disable_auto_mine_transactions()
     tx_hash = await session.broadcast_transfer(root_signer, another_signer.address, to_transfer)
     tx_hashes = await session.eth_get_filter_changes(transaction_filter)
     assert tx_hashes == (tx_hash,)
 
 
 async def test_log_filter_all(session, compiled_contracts, root_signer, another_signer):
-
     basic_contract = compiled_contracts["BasicContract"]
     await session.transfer(root_signer, another_signer.address, Amount.ether(1))
     contract1 = await session.deploy(root_signer, basic_contract.constructor(123))
     contract2 = await session.deploy(another_signer, basic_contract.constructor(123))
 
     log_filter = await session.eth_new_filter()
     await session.transact(root_signer, contract1.write.deposit(b"1234"))
@@ -455,15 +447,14 @@
     assert (
         normalize_topics(entries[1].topics)
         == contract2.abi.event.Deposit2(another_signer.address, b"4567").topics
     )
 
 
 async def test_log_filter_by_address(session, compiled_contracts, root_signer, another_signer):
-
     basic_contract = compiled_contracts["BasicContract"]
     await session.transfer(root_signer, another_signer.address, Amount.ether(1))
     contract1 = await session.deploy(root_signer, basic_contract.constructor(123))
     contract2 = await session.deploy(another_signer, basic_contract.constructor(123))
 
     # Filter by a single address
 
@@ -499,15 +490,14 @@
     assert (
         normalize_topics(entries[1].topics)
         == contract3.abi.event.Deposit(root_signer.address, b"3333").topics
     )
 
 
 async def test_log_filter_by_topic(session, compiled_contracts, root_signer, another_signer):
-
     basic_contract = compiled_contracts["BasicContract"]
     await session.transfer(root_signer, another_signer.address, Amount.ether(1))
     contract1 = await session.deploy(root_signer, basic_contract.constructor(123))
     contract2 = await session.deploy(another_signer, basic_contract.constructor(123))
 
     # Filter by a specific topic or None at each position
 
@@ -554,15 +544,14 @@
     assert (
         normalize_topics(entries[1].topics)
         == contract2.abi.event.Deposit(another_signer.address, b"3333").topics
     )
 
 
 async def test_log_filter_by_block_num(session, compiled_contracts, root_signer, another_signer):
-
     basic_contract = compiled_contracts["BasicContract"]
     await session.transfer(root_signer, another_signer.address, Amount.ether(1))
     contract1 = await session.deploy(root_signer, basic_contract.constructor(123))
 
     await session.transact(root_signer, contract1.write.deposit(b"1111"))
     block_num = await session.eth_block_number()
     await session.transact(root_signer, contract1.write.deposit(b"2222"))  # filter will start here
@@ -579,15 +568,14 @@
         contract1.abi.event.Deposit(root_signer.address, b"2222").topics,
         contract1.abi.event.Deposit(root_signer.address, b"3333").topics,
         contract1.abi.event.Deposit(root_signer.address, b"4444").topics,
     ]
 
 
 async def test_block_filter_high_level(autojump_clock, session, root_signer, another_signer):
-
     block_hashes = []
 
     async def observer():
         # This loop always exits via break
         async for block_hash in session.iter_blocks(poll_interval=1):  # pragma: no branch
             block_hashes.append(block_hash)
             if len(block_hashes) == 3:
@@ -609,15 +597,14 @@
         block_info = await session.eth_get_block_by_hash(block_hash, with_transactions=True)
         assert block_info.transactions[0].value == Amount.ether(i + 2)
 
 
 async def test_pending_transaction_filter_high_level(
     autojump_clock, session, root_signer, another_signer
 ):
-
     tx_hashes = []
 
     async def observer():
         # This loop always exits via break
         async for tx_hash in session.iter_pending_transactions(  # pragma: no branch
             poll_interval=1
         ):
@@ -641,15 +628,14 @@
         tx_info = await session.eth_get_transaction_by_hash(tx_hash)
         assert tx_info.value == Amount.ether(i + 2)
 
 
 async def test_event_filter_high_level(
     autojump_clock, session, compiled_contracts, root_signer, another_signer
 ):
-
     basic_contract = compiled_contracts["BasicContract"]
     await session.transfer(root_signer, another_signer.address, Amount.ether(1))
     contract1 = await session.deploy(root_signer, basic_contract.constructor(123))
     contract2 = await session.deploy(another_signer, basic_contract.constructor(123))
 
     events = []
 
@@ -676,17 +662,17 @@
         await session.transact(
             another_signer, contract2.write.deposit2(b"1111"), amount=Amount.wei(2)
         )
         await session.transact(
             another_signer, contract2.write.deposit2(b"1111"), amount=Amount.wei(3)
         )
 
-    assert events[0] == {"from": root_signer.address, "id": b"1111", "value": 1, "value2": 2}
-    assert events[1] == {"from": another_signer.address, "id": b"1111", "value": 2, "value2": 3}
-    assert events[2] == {"from": another_signer.address, "id": b"1111", "value": 3, "value2": 4}
+    assert events[0] == {"from_": root_signer.address, "id": b"1111", "value": 1, "value2": 2}
+    assert events[1] == {"from_": another_signer.address, "id": b"1111", "value": 2, "value2": 3}
+    assert events[2] == {"from_": another_signer.address, "id": b"1111", "value": 3, "value2": 4}
 
 
 async def test_unknown_rpc_status_code(test_provider, session, monkeypatch):
     def faulty_net_version():
         # This is a known exception type, and it will be transferred through the network
         # keeping the status code.
         raise RPCError(666, "this method is possessed")
@@ -703,15 +689,14 @@
 
     assert exc.value.code == expected_code
     assert exc.value.message == expected_message
     assert exc.value.data == expected_data
 
 
 async def test_contract_exceptions(session, root_signer, compiled_contracts):
-
     compiled_contract = compiled_contracts["TestErrors"]
     contract = await session.deploy(root_signer, compiled_contract.constructor(999))
 
     error_selector = keccak(b"Error(string)")[:4]
     custom_error_selector = keccak(b"CustomError(uint256)")[:4]
 
     # `require(condition)`
@@ -752,15 +737,14 @@
         expected_message="execution reverted",
         expected_data=custom_error_selector + encode_args((abi.uint(256), 4)),
     )
     await check_rpc_error(session.eth_call(contract.read.viewError(4)), **kwargs)
 
 
 async def test_contract_panics(session, root_signer, compiled_contracts):
-
     compiled_contract = compiled_contracts["TestErrors"]
     contract = await session.deploy(root_signer, compiled_contract.constructor(999))
 
     panic_selector = keccak(b"Panic(uint256)")[:4]
 
     await check_rpc_error(
         session.eth_call(contract.read.viewPanic(0)),
@@ -774,15 +758,14 @@
         expected_code=ProviderError.Code.EXECUTION_ERROR,
         expected_message="execution reverted",
         expected_data=panic_selector + encode_args((abi.uint(256), 0x11)),
     )
 
 
 async def test_contract_exceptions_high_level(session, root_signer, compiled_contracts):
-
     compiled_contract = compiled_contracts["TestErrors"]
     contract = await session.deploy(root_signer, compiled_contract.constructor(999))
 
     with pytest.raises(ContractPanic) as exc:
         await session.estimate_transact(contract.write.transactPanic(1))
     assert exc.value.reason == ContractPanic.Reason.OVERFLOW
 
@@ -804,15 +787,14 @@
     with pytest.raises(ContractError) as exc:
         await session.estimate_deploy(compiled_contract.constructor(4))
     assert exc.value.error == contract.error.CustomError
     assert exc.value.data == {"x": 4}
 
 
 async def test_unknown_error_reasons(test_provider, session, compiled_contracts, root_signer):
-
     compiled_contract = compiled_contracts["TestErrors"]
     contract = await session.deploy(root_signer, compiled_contract.constructor(999))
 
     # Provider returns an unknown panic code
 
     def eth_estimate_gas(*args, **kwargs):
         # Invalid selector
```

### Comparing `pons-0.5.1/tests/test_contract.py` & `pons-0.6.0/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `pons-0.5.1/tests/test_contract_abi.py` & `pons-0.6.0/tests/test_contract_abi.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     sig = EventSignature(dict(a=abi.uint(8), b=abi.bool, c=abi.bytes(4)), {"a", "b"})
     assert str(sig) == "(uint8 indexed a, bool indexed b, bytes4 c)"
     assert sig.canonical_form == "(uint8,bool,bytes4)"
     assert sig.canonical_form_nonindexed == "(bytes4)"
 
 
 def test_event_signature_encode():
-
     sig = EventSignature(dict(a=abi.uint(8), b=abi.bool, c=abi.bytes(4)), {"a", "b"})
 
     # All indexed parameters provided
     encoded = sig.encode_to_topics(1, True)
     assert encoded == ((abi.uint(8).encode(1),), (abi.bool.encode(True),))
 
     # One indexed parameter not provided
@@ -72,15 +71,14 @@
     assert encoded == (
         (abi.uint(8).encode(1), abi.uint(8).encode(2)),
         (abi.bool.encode(True),),
     )
 
 
 def test_event_signature_decode():
-
     sig = EventSignature(dict(a=abi.uint(8), b=abi.bool, c=abi.bytes(4), d=abi.bytes()), {"a", "b"})
 
     decoded = sig.decode_log_entry(
         [abi.uint(8).encode(1), abi.bool.encode(True)],
         encode_args((abi.bytes(4), b"1234"), (abi.bytes(), b"bytestring")),
     )
     assert decoded == dict(a=1, b=True, c=b"1234", d=b"bytestring")
@@ -284,53 +282,51 @@
             ],
         )
     )
 
     _check_write_method(write)
 
 
+def test_write_method_with_output():
+    # Mutating methods can have outputs (in case they are called by other mutating methods),
+    # but we cannot get that output from the outside.
+    # So if we see those in a JSON ABI, we can just ignore them.
+    write = WriteMethod.from_json(
+        dict(
+            type="function",
+            name="someMethod",
+            stateMutability="payable",
+            inputs=[
+                dict(type="uint8", name="a"),
+                dict(type="bool", name="b"),
+            ],
+            outputs=[
+                dict(type="uint8", name="a"),
+                dict(type="bool", name="b"),
+            ],
+        )
+    )
+
+    _check_write_method(write)
+
+
 def test_write_method_init():
     write = WriteMethod(name="someMethod", inputs=dict(a=abi.uint(8), b=abi.bool), payable=True)
 
     _check_write_method(write)
 
 
 def test_write_method_errors():
-
     with pytest.raises(
         ValueError,
         match="WriteMethod object must be created from a JSON entry with type='function'",
     ):
         WriteMethod.from_json(dict(type="constructor"))
 
     with pytest.raises(
-        ValueError, match="Mutating method's JSON entry cannot have non-empty `outputs`"
-    ):
-        WriteMethod.from_json(
-            dict(
-                type="function",
-                name="someMethod",
-                stateMutability="payable",
-                inputs=[dict(type="uint8", name="a")],
-                outputs=[dict(type="uint8", name="a")],
-            )
-        )
-
-    # This is fine
-    WriteMethod.from_json(
-        dict(
-            type="function",
-            name="someMethod",
-            stateMutability="payable",
-            inputs=[dict(type="uint8", name="a")],
-            outputs=[],
-        )
-    )
-
-    with pytest.raises(
         ValueError,
         match="Mutating method's JSON entry state mutability must be `nonpayable` or `payable`",
     ):
         WriteMethod.from_json(
             dict(
                 type="function",
                 name="someMethod",
@@ -438,16 +434,16 @@
     assert str(cabi) == (
         "{\n"
         "    constructor(uint8 a, bool b) payable\n"
         "    fallback() payable\n"
         "    receive() payable\n"
         "    function readMethod(uint8 a, bool b) returns (uint8, bool)\n"
         "    function writeMethod(uint8 a, bool b) payable\n"
-        "    event Deposit(address indexed from, bytes indexed foo, uint8 bar) anonymous\n"
-        "    error CustomError(address from, bytes foo, uint8 bar)\n"
+        "    event Deposit(address indexed from_, bytes indexed foo, uint8 bar) anonymous\n"
+        "    error CustomError(address from_, bytes foo, uint8 bar)\n"
         "}"
     )
 
     assert isinstance(cabi.constructor, Constructor)
     assert isinstance(cabi.fallback, Fallback)
     assert isinstance(cabi.receive, Receive)
     assert isinstance(cabi.read.readMethod, ReadMethod)
@@ -559,15 +555,15 @@
             name="Foo",
             type="event",
         )
     )
     assert event.anonymous
     assert event.name == "Foo"
     assert event.indexed == {"from", "foo"}
-    assert str(event.fields) == "(address indexed from, bytes indexed foo, uint8 bar)"
+    assert str(event.fields) == "(address indexed from_, bytes indexed foo, uint8 bar)"
 
 
 def test_event_init():
     event = Event(
         "Foo",
         dict(from_=abi.address, foo=abi.bytes(), bar=abi.uint(8)),
         indexed={"from_", "foo"},
@@ -576,15 +572,14 @@
     assert event.anonymous
     assert event.name == "Foo"
     assert event.indexed == {"from_", "foo"}
     assert str(event.fields) == "(address indexed from_, bytes indexed foo, uint8 bar)"
 
 
 def test_event_encode():
-
     event = Event("Foo", dict(a=abi.bool, b=abi.uint(8), c=abi.bytes(4)), {"a", "b"})
     event_filter = event(b=Either(1, 2))
     assert event_filter.topics == (
         (LogTopic(keccak(event.name.encode() + event.fields.canonical_form.encode())),),
         None,
         (LogTopic(abi.uint(8).encode(1)), LogTopic(abi.uint(8).encode(2))),
     )
@@ -597,15 +592,14 @@
     assert event_filter.topics == (
         None,
         (LogTopic(abi.uint(8).encode(1)), LogTopic(abi.uint(8).encode(2))),
     )
 
 
 def test_event_decode():
-
     # We only need a couple of fields
     fake_log_entry = namedtuple("fake_log_entry", ["topics", "data"])
 
     event = Event("Foo", dict(a=abi.bool, b=abi.uint(8), c=abi.bytes(4), d=abi.bytes()), {"a", "b"})
 
     decoded = event.decode_log_entry(
         fake_log_entry(
@@ -693,15 +687,15 @@
                 dict(internalType="uint8", name="bar", type="uint8"),
             ],
             name="Foo",
             type="error",
         )
     )
     assert error.name == "Foo"
-    assert str(error.fields) == "(address from, bytes foo, uint8 bar)"
+    assert str(error.fields) == "(address from_, bytes foo, uint8 bar)"
 
     with pytest.raises(
         ValueError,
         match="Error object must be created from a JSON entry with type='error'",
     ):
         Error.from_json(dict(type="constructor"))
```

### Comparing `pons-0.5.1/tests/test_contract_functionality.py` & `pons-0.6.0/tests/test_contract_functionality.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     deployed_contract = await session.deploy(root_signer, compiled_contract.constructor())
     call = deployed_contract.read.getState(123)
     result = await session.eth_call(call)
     assert result == (1 + 123,)
 
 
 async def test_basics(session, root_signer, another_signer, compiled_contracts):
-
     compiled_contract = compiled_contracts["Test"]
 
     # Deploy the contract
     call = compiled_contract.constructor(12345, 56789)
     await session.transfer(root_signer, another_signer.address, Amount.ether(10))
     deployed_contract = await session.deploy(another_signer, call)
 
@@ -60,15 +59,14 @@
     inner = dict(inner1=1, inner2=2)
     outer = dict(inner=inner, outer1=3)
     result = await session.eth_call(deployed_contract.read.testStructs(inner, outer))
     assert result == (inner, outer)
 
 
 async def test_abi_declaration(session, root_signer, another_signer, compiled_contracts):
-
     compiled_contract = compiled_contracts["Test"]
 
     # Deploy the contract
     await session.transfer(root_signer, another_signer.address, Amount.ether(10))
     call = compiled_contract.constructor(12345, 56789)
     previously_deployed_contract = await session.deploy(another_signer, call)
```

### Comparing `pons-0.5.1/tests/test_entities.py` & `pons-0.6.0/tests/test_entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,14 @@
         Amount.wei(100) * 2.0
 
     with pytest.raises(TypeError, match="Expected an integer, got float"):
         Amount.wei(100) // 2.0
 
 
 def test_address():
-
     random_addr = b"dv\xbbCQ,\xfe\xd0\xbfF\x8aq\x07OK\xf9\xa1i\x88("
     random_addr_checksum = "0x6476Bb43512CFed0bF468a71074F4bF9A1698828"
 
     assert bytes(Address(random_addr)) == random_addr
     assert bytes(Address.from_hex(random_addr_checksum)) == random_addr
     assert bytes(Address.from_hex(random_addr_checksum.lower())) == random_addr
 
@@ -141,15 +140,14 @@
     # Everything else is in the base class which is tested elsewhere
     TxHash(os.urandom(32))
     BlockHash(os.urandom(32))
     LogTopic(os.urandom(32))
 
 
 def test_decode_tx_receipt():
-
     address = Address(os.urandom(20))
 
     tx_receipt_json = {
         "transactionHash": "0xf105e4ee72d1538a4e10ee9584581e2b6f13cd9be82acd14e8edd65d954483c5",
         "blockHash": "0x3f62ac76f9551dbf878c334657ce19a86881734cbf53f8ecd9c3afb9a22d5bee",
         "blockNumber": "0xa38696",
         "contractAddress": address.rpc_encode(),
@@ -222,15 +220,14 @@
     assert rpc_decode_bool(True) == True
 
     with pytest.raises(RPCDecodingError, match="Encoded boolean must be `true` or `false`"):
         rpc_decode_bool(1)
 
 
 def test_decode_block_info():
-
     json_result = {
         "baseFeePerGas": "0xbcdaf1db6",
         "difficulty": "0x2c72989f9145c8",
         "gasLimit": "0x1cb2a73",
         "gasUsed": "0x50c7cc",
         "hash": "0x477a8386bbcc43f54b0231317d6a95f62ab10909d2d985ac5957633090ae69a8",
         "miner": "0x7f101fe45e6649a6fb8f3f8b43ed03d353f2b90c",
```

### Comparing `pons-0.5.1/tests/test_provider.py` & `pons-0.6.0/tests/test_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,14 @@
     )
 
     with pytest.raises(BadResponseFormat, match="Expected a dictionary as a response, got str"):
         receipt = await session.eth_get_transaction_receipt(tx_hash)
 
 
 async def test_missing_field(test_provider, session, monkeypatch, root_signer, another_signer):
-
     orig_eth_get_transaction_receipt = test_provider.eth_get_transaction_receipt
 
     def faulty_eth_get_transaction_receipt(tx_hash):
         receipt = orig_eth_get_transaction_receipt(tx_hash)
         del receipt["status"]
         return receipt
```

### Comparing `pons-0.5.1/tests/test_signer.py` & `pons-0.6.0/tests/test_signer.py`

 * *Files identical despite different names*

### Comparing `pons-0.5.1/PKG-INFO` & `pons-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pons
-Version: 0.5.1
+Version: 0.6.0
 Summary: Async RPC client for Ethereum
 License: MIT
 Author-email: Bogdan Opanchuk <bogdan@opanchuk.net>
 Requires-Python: >=3.8
 Provides-Extra: docs
 Provides-Extra: lint
 Provides-Extra: tests
```


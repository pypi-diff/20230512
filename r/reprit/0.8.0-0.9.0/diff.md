# Comparing `tmp/reprit-0.8.0.tar.gz` & `tmp/reprit-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reprit-0.8.0.tar", last modified: Sat Jun 11 18:52:48 2022, max compression
+gzip compressed data, was "reprit-0.9.0.tar", last modified: Thu May 11 22:43:56 2023, max compression
```

## Comparing `reprit-0.8.0.tar` & `reprit-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-11 18:52:48.441241 reprit-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-06-11 18:52:29.000000 reprit-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-11 18:52:29.000000 reprit-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6124 2022-06-11 18:52:48.437241 reprit-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5304 2022-06-11 18:52:29.000000 reprit-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-11 18:52:48.437241 reprit-0.8.0/reprit/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-06-11 18:52:29.000000 reprit-0.8.0/reprit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8478 2022-06-11 18:52:29.000000 reprit-0.8.0/reprit/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-11 18:52:48.437241 reprit-0.8.0/reprit/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-11 18:52:29.000000 reprit-0.8.0/reprit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-06-11 18:52:29.000000 reprit-0.8.0/reprit/core/hints.py
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-06-11 18:52:29.000000 reprit-0.8.0/reprit/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-06-11 18:52:29.000000 reprit-0.8.0/reprit/hints.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-11 18:52:29.000000 reprit-0.8.0/reprit/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     1464 2022-06-11 18:52:29.000000 reprit-0.8.0/reprit/seekers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3657 2022-06-11 18:52:29.000000 reprit-0.8.0/reprit/serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-06-11 18:52:29.000000 reprit-0.8.0/reprit/serializers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-11 18:52:48.437241 reprit-0.8.0/reprit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6124 2022-06-11 18:52:47.000000 reprit-0.8.0/reprit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-06-11 18:52:48.000000 reprit-0.8.0/reprit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-11 18:52:47.000000 reprit-0.8.0/reprit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-06-11 18:52:48.000000 reprit-0.8.0/reprit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-11 18:52:48.441241 reprit-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-06-11 18:52:29.000000 reprit-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:43:56.702423 reprit-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-11 22:43:47.000000 reprit-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 22:43:47.000000 reprit-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-05-11 22:43:56.702423 reprit-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-11 22:43:47.000000 reprit-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-11 22:43:47.000000 reprit-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:43:56.702423 reprit-0.9.0/reprit/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-11 22:43:47.000000 reprit-0.9.0/reprit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-05-11 22:43:47.000000 reprit-0.9.0/reprit/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:43:56.702423 reprit-0.9.0/reprit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 22:43:47.000000 reprit-0.9.0/reprit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-11 22:43:47.000000 reprit-0.9.0/reprit/core/hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-11 22:43:47.000000 reprit-0.9.0/reprit/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-11 22:43:47.000000 reprit-0.9.0/reprit/hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 22:43:47.000000 reprit-0.9.0/reprit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-11 22:43:47.000000 reprit-0.9.0/reprit/seekers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-05-11 22:43:47.000000 reprit-0.9.0/reprit/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-11 22:43:47.000000 reprit-0.9.0/reprit/serializers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 22:43:56.702423 reprit-0.9.0/reprit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-05-11 22:43:56.000000 reprit-0.9.0/reprit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-11 22:43:56.000000 reprit-0.9.0/reprit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 22:43:56.000000 reprit-0.9.0/reprit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 22:43:56.000000 reprit-0.9.0/reprit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 22:43:56.000000 reprit-0.9.0/reprit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 22:43:56.702423 reprit-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-11 22:43:47.000000 reprit-0.9.0/setup.py
```

### Comparing `reprit-0.8.0/LICENSE` & `reprit-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reprit-0.8.0/PKG-INFO` & `reprit-0.9.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,18 @@
-Metadata-Version: 2.1
-Name: reprit
-Version: 0.8.0
-Summary: Auto __repr__ method generation.
-Home-page: https://github.com/lycantropos/reprit/
-Download-URL: https://github.com/lycantropos/reprit/archive/master.zip
-Author: Azat Ibrakov
-Author-email: azatibrakov@gmail.com
-License: MIT License
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 reprit
 ======
 
 [![](https://github.com/lycantropos/reprit/workflows/CI/badge.svg)](https://github.com/lycantropos/reprit/actions/workflows/ci.yml "Github Actions")
 [![](https://readthedocs.org/projects/reprit/badge/?version=latest)](https://reprit.readthedocs.io/en/latest "Documentation")
 [![](https://codecov.io/gh/lycantropos/reprit/branch/master/graph/badge.svg)](https://codecov.io/gh/lycantropos/reprit "Codecov")
 [![](https://img.shields.io/github/license/lycantropos/reprit.svg)](https://github.com/lycantropos/reprit/blob/master/LICENSE "License")
 [![](https://badge.fury.io/py/reprit.svg)](https://badge.fury.io/py/reprit "PyPI")
 
-In what follows `python` is an alias for `python3.6` or `pypy3.6`
-or any later version (`python3.7`, `pypy3.7` and so on).
+In what follows `python` is an alias for `python3.7` or `pypy3.7`
+or any later version (`python3.8`, `pypy3.8` and so on).
 
 Installation
 ------------
 
 Install the latest `pip` & `setuptools` packages versions
 ```bash
 python -m pip install --upgrade pip setuptools
```

### Comparing `reprit-0.8.0/reprit/base.py` & `reprit-0.9.0/reprit/base.py`

 * *Files identical despite different names*

### Comparing `reprit-0.8.0/reprit/seekers.py` & `reprit-0.9.0/reprit/seekers.py`

 * *Files identical despite different names*

### Comparing `reprit-0.8.0/reprit/serializers.py` & `reprit-0.9.0/reprit/serializers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,82 @@
+import sys as _sys
+import typing as _t
 from enum import Enum as _Enum
 from functools import singledispatch as _singledispatch
 from types import (BuiltinFunctionType as _BuiltinFunctionType,
                    BuiltinMethodType as _BuiltinMethodType,
+                   ClassMethodDescriptorType as _ClassMethodDescriptorType,
                    FunctionType as _FunctionType,
                    GetSetDescriptorType as _GetSetDescriptorType,
                    MemberDescriptorType as _MemberDescriptorType,
+                   MethodDescriptorType as _MethodDescriptorType,
                    MethodType as _MethodType,
-                   ModuleType as _ModuleType)
-from typing import Union as _Union
+                   MethodWrapperType as _MethodWrapperType,
+                   ModuleType as _ModuleType,
+                   WrapperDescriptorType as _WrapperDescriptorType)
+
+import typing_extensions as _te
+
+_Params = _te.ParamSpec('_Params')
+_T1 = _t.TypeVar('_T1')
+_T2 = _t.TypeVar('_T2')
+
+
+def _decorate_if(
+        decorator: _t.Callable[[_t.Callable[_Params, _T1]], _t.Any],
+        condition: bool
+) -> _t.Callable[[_t.Callable[_Params, _T1]], _t.Any]:
+    return decorator if condition else _identity_decorator
+
+
+def _identity_decorator(
+        value: _t.Callable[_Params, _T1]
+) -> _t.Callable[_Params, _T1]:
+    return value
 
-try:
-    from types import ClassMethodDescriptorType as _ClassMethodDescriptorType
-except ImportError:
-    _ClassMethodDescriptorType = type(dict.__dict__['fromkeys'])
-try:
-    from types import MethodDescriptorType as _MethodDescriptorType
-except ImportError:
-    _MethodDescriptorType = type(str.join)
-try:
-    from types import MethodWrapperType as _MethodWrapperType
-except ImportError:
-    _MethodWrapperType = type(object().__str__)
-try:
-    from types import WrapperDescriptorType as _WrapperDescriptorType
-except ImportError:
-    _WrapperDescriptorType = type(object.__init__)
 
 simple = repr
 
 
 @_singledispatch
 def complex_(object_):
     return repr(object_)
 
 
 @complex_.register(_BuiltinFunctionType)
 @complex_.register(_FunctionType)
 @complex_.register(type)
-def _(object_: _Union[_BuiltinFunctionType, _FunctionType, type]) -> str:
+def _(object_: _t.Union[_BuiltinFunctionType, _FunctionType, type]) -> str:
     return object_.__module__ + '.' + object_.__qualname__
 
 
-@complex_.register(_BuiltinMethodType)
+@_decorate_if(complex_.register(_BuiltinMethodType),
+              _sys.implementation.name != 'pypy')
 @complex_.register(_MethodType)
-def _(object_: _Union[_BuiltinMethodType, _MethodType]) -> str:
+def _(object_: _t.Union[_BuiltinMethodType, _MethodType]) -> str:
     return complex_(object_.__self__) + '.' + object_.__name__
 
 
-@complex_.register(_ClassMethodDescriptorType)
+@_decorate_if(complex_.register(_ClassMethodDescriptorType),
+              _sys.implementation.name != 'pypy')
+@_decorate_if(complex_.register(_MethodDescriptorType),
+              _sys.implementation.name != 'pypy')
+@_decorate_if(complex_.register(_MethodWrapperType),
+              _sys.implementation.name != 'pypy')
+@_decorate_if(complex_.register(_WrapperDescriptorType),
+              _sys.implementation.name != 'pypy')
 @complex_.register(_GetSetDescriptorType)
 @complex_.register(_MemberDescriptorType)
-@complex_.register(_MethodDescriptorType)
-@complex_.register(_MethodWrapperType)
-@complex_.register(_WrapperDescriptorType)
-def _(object_: _Union[_ClassMethodDescriptorType, _GetSetDescriptorType,
-                      _MemberDescriptorType, _MethodDescriptorType,
-                      _MethodWrapperType, _WrapperDescriptorType]) -> str:
+def _(
+        object_: _t.Union[
+            _ClassMethodDescriptorType, _GetSetDescriptorType,
+            _MemberDescriptorType, _MethodDescriptorType, _MethodWrapperType,
+            _WrapperDescriptorType
+        ]
+) -> str:
     return complex_(object_.__objclass__) + '.' + object_.__name__
 
 
 @complex_.register(_Enum)
 def _(object_: _Enum) -> str:
     return complex_(type(object_)) + '.' + object_.name
 
@@ -67,15 +84,15 @@
 @complex_.register(_ModuleType)
 def _(object_: _ModuleType) -> str:
     return object_.__name__
 
 
 @complex_.register(classmethod)
 @complex_.register(staticmethod)
-def _(object_: _Union[classmethod, staticmethod]) -> str:
+def _(object_: _t.Union[classmethod, staticmethod]) -> str:
     return '{}({})'.format(complex_(type(object_)), complex_(object_.__func__))
 
 
 @complex_.register(dict)
 def _(object_: dict) -> str:
     return '{' + ', '.join(map('{}: {}'.format,
                                map(complex_, object_.keys()),
```

### Comparing `reprit-0.8.0/reprit.egg-info/PKG-INFO` & `reprit-0.9.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,61 @@
 Metadata-Version: 2.1
 Name: reprit
-Version: 0.8.0
-Summary: Auto __repr__ method generation.
+Version: 0.9.0
 Home-page: https://github.com/lycantropos/reprit/
 Download-URL: https://github.com/lycantropos/reprit/archive/master.zip
-Author: Azat Ibrakov
-Author-email: azatibrakov@gmail.com
+Author-email: Azat Ibrakov <azatibrakov@gmail.com>
 License: MIT License
+        
+        Copyright (c) 2019 Azat Ibrakov
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: tests
 License-File: LICENSE
 
 reprit
 ======
 
 [![](https://github.com/lycantropos/reprit/workflows/CI/badge.svg)](https://github.com/lycantropos/reprit/actions/workflows/ci.yml "Github Actions")
 [![](https://readthedocs.org/projects/reprit/badge/?version=latest)](https://reprit.readthedocs.io/en/latest "Documentation")
 [![](https://codecov.io/gh/lycantropos/reprit/branch/master/graph/badge.svg)](https://codecov.io/gh/lycantropos/reprit "Codecov")
 [![](https://img.shields.io/github/license/lycantropos/reprit.svg)](https://github.com/lycantropos/reprit/blob/master/LICENSE "License")
 [![](https://badge.fury.io/py/reprit.svg)](https://badge.fury.io/py/reprit "PyPI")
 
-In what follows `python` is an alias for `python3.6` or `pypy3.6`
-or any later version (`python3.7`, `pypy3.7` and so on).
+In what follows `python` is an alias for `python3.7` or `pypy3.7`
+or any later version (`python3.8`, `pypy3.8` and so on).
 
 Installation
 ------------
 
 Install the latest `pip` & `setuptools` packages versions
 ```bash
 python -m pip install --upgrade pip setuptools
```


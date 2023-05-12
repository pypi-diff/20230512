# Comparing `tmp/pydio-0.4.0.tar.gz` & `tmp/pydio-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydio-0.4.0.tar", max compression
+gzip compressed data, was "pydio-0.4.1.tar", max compression
```

## Comparing `pydio-0.4.0.tar` & `pydio-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1094 2023-05-06 07:24:30.230336 pydio-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     3064 2023-05-06 07:24:30.230336 pydio-0.4.0/README.md
--rw-r--r--   0        0        0      525 2023-05-06 07:24:30.230336 pydio-0.4.0/pydio/__init__.py
--rw-r--r--   0        0        0      517 2023-05-06 07:24:30.230336 pydio-0.4.0/pydio/_compat.py
--rw-r--r--   0        0        0     3458 2023-05-06 07:24:30.230336 pydio-0.4.0/pydio/_factories.py
--rw-r--r--   0        0        0     2545 2023-05-06 07:24:30.230336 pydio-0.4.0/pydio/_unbound_factories.py
--rw-r--r--   0        0        0      845 2023-05-06 07:24:30.230336 pydio-0.4.0/pydio/api.py
--rw-r--r--   0        0        0     7043 2023-05-06 07:24:30.230336 pydio-0.4.0/pydio/base.py
--rw-r--r--   0        0        0     1765 2023-05-06 07:24:30.230336 pydio-0.4.0/pydio/exc.py
--rw-r--r--   0        0        0     7221 2023-05-06 07:24:30.230336 pydio-0.4.0/pydio/injector.py
--rw-r--r--   0        0        0     1663 2023-05-06 07:24:30.230336 pydio-0.4.0/pydio/keys.py
--rw-r--r--   0        0        0     4942 2023-05-06 07:24:30.230336 pydio-0.4.0/pydio/provider.py
--rw-r--r--   0        0        0     1568 2023-05-06 07:24:30.230336 pydio-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 pydio-0.4.0/setup.py
--rw-r--r--   0        0        0     4238 1970-01-01 00:00:00.000000 pydio-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-05-12 11:01:16.463130 pydio-0.4.1/LICENSE.txt
+-rw-r--r--   0        0        0     3064 2023-05-12 11:01:16.463130 pydio-0.4.1/README.md
+-rw-r--r--   0        0        0      525 2023-05-12 11:01:16.467130 pydio-0.4.1/pydio/__init__.py
+-rw-r--r--   0        0        0      517 2023-05-12 11:01:16.467130 pydio-0.4.1/pydio/_compat.py
+-rw-r--r--   0        0        0     3458 2023-05-12 11:01:16.467130 pydio-0.4.1/pydio/_factories.py
+-rw-r--r--   0        0        0     2545 2023-05-12 11:01:16.467130 pydio-0.4.1/pydio/_unbound_factories.py
+-rw-r--r--   0        0        0      845 2023-05-12 11:01:16.467130 pydio-0.4.1/pydio/api.py
+-rw-r--r--   0        0        0     7043 2023-05-12 11:01:16.467130 pydio-0.4.1/pydio/base.py
+-rw-r--r--   0        0        0     1765 2023-05-12 11:01:16.467130 pydio-0.4.1/pydio/exc.py
+-rw-r--r--   0        0        0     7627 2023-05-12 11:01:16.467130 pydio-0.4.1/pydio/injector.py
+-rw-r--r--   0        0        0     1663 2023-05-12 11:01:16.467130 pydio-0.4.1/pydio/keys.py
+-rw-r--r--   0        0        0     4942 2023-05-12 11:01:16.467130 pydio-0.4.1/pydio/provider.py
+-rw-r--r--   0        0        0     1568 2023-05-12 11:01:16.467130 pydio-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 pydio-0.4.1/setup.py
+-rw-r--r--   0        0        0     4238 1970-01-01 00:00:00.000000 pydio-0.4.1/PKG-INFO
```

### Comparing `pydio-0.4.0/LICENSE.txt` & `pydio-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydio-0.4.0/README.md` & `pydio-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pydio-0.4.0/pydio/__init__.py` & `pydio-0.4.1/pydio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 # This file is part of PyDio library and is released under the terms of the
 # MIT license: http://opensource.org/licenses/mit-license.php.
 #
 # See LICENSE.txt for details.
 # ---------------------------------------------------------------------------
 __released__ = 2021
 __author__ = 'Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>'
-__version__ = '0.4.0'
+__version__ = '0.4.1'
```

### Comparing `pydio-0.4.0/pydio/_compat.py` & `pydio-0.4.1/pydio/_compat.py`

 * *Files identical despite different names*

### Comparing `pydio-0.4.0/pydio/_factories.py` & `pydio-0.4.1/pydio/_factories.py`

 * *Files identical despite different names*

### Comparing `pydio-0.4.0/pydio/_unbound_factories.py` & `pydio-0.4.1/pydio/_unbound_factories.py`

 * *Files identical despite different names*

### Comparing `pydio-0.4.0/pydio/api.py` & `pydio-0.4.1/pydio/api.py`

 * *Files identical despite different names*

### Comparing `pydio-0.4.0/pydio/base.py` & `pydio-0.4.1/pydio/base.py`

 * *Files identical despite different names*

### Comparing `pydio-0.4.0/pydio/exc.py` & `pydio-0.4.1/pydio/exc.py`

 * *Files identical despite different names*

### Comparing `pydio-0.4.0/pydio/injector.py` & `pydio-0.4.1/pydio/injector.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # Copyright (C) 2021 - 2023 Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>
 #
 # This file is part of PyDio library and is released under the terms of the
 # MIT license: http://opensource.org/licenses/mit-license.php.
 #
 # See LICENSE.txt for details.
 # ---------------------------------------------------------------------------
+import asyncio
 import inspect
 import threading
 import typing
 import weakref
 from typing import Awaitable, Hashable, Optional
 
 from . import exc
@@ -124,26 +125,34 @@
             with self._lock:
                 provider = self._provider
                 awaitables = []
                 for child in self._child_injectors:
                     maybe_awaitable = child._do_close(exc_type, exc, tb)
                     if maybe_awaitable is not None:
                         awaitables.append(maybe_awaitable)
+                first_exc_raised = None
                 for instance in self._cache.values():
-                    maybe_awaitable = instance.close(exc_type, exc, tb)
-                    if maybe_awaitable is not None:
-                        awaitables.append(maybe_awaitable)
+                    try:
+                        maybe_awaitable = instance.close(exc_type, exc, tb)
+                        if maybe_awaitable is not None:
+                            awaitables.append(maybe_awaitable)
+                    except Exception as e:
+                        if first_exc_raised is None:
+                            first_exc_raised = e
                 if not provider.has_awaitables():
                     self._provider = None
+                    if first_exc_raised is not None:
+                        raise first_exc_raised
                 else:
 
                     async def do_async_close(awaitables):
                         self._provider = None
-                        for awaitable in awaitables:
-                            await awaitable
+                        await asyncio.gather(*awaitables)
+                        if first_exc_raised is not None:
+                            raise first_exc_raised
 
                     return do_async_close(awaitables)
 
     def is_closed(self) -> bool:
         """Return True if this injector was closed or False otherwise."""
         return self._provider is None
```

### Comparing `pydio-0.4.0/pydio/keys.py` & `pydio-0.4.1/pydio/keys.py`

 * *Files identical despite different names*

### Comparing `pydio-0.4.0/pydio/provider.py` & `pydio-0.4.1/pydio/provider.py`

 * *Files identical despite different names*

### Comparing `pydio-0.4.0/pyproject.toml` & `pydio-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyDio"
-version = "0.4.0"
+version = "0.4.1"
 description = "Simple and functional dependency injection toolkit for Python"
 authors = [
     "Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>"
 ]
 license = "MIT"
 readme = "README.md"
 documentation = "https://pydio.readthedocs.io"
@@ -41,15 +41,15 @@
 twine = "^4.0.1"
 toml = "^0.10.2"
 tox = "^3.27.0"
 myst-parser = "^0.18.1"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.4.0"
+version = "0.4.1"
 tag_format = "v$version"
 update_changelog_on_bump = true
 bump_message = "bump: $current_version -> $new_version [skip ci]"
 version_files = [
     "pydio/__init__.py",
     "pyproject.toml"
 ]
```

### Comparing `pydio-0.4.0/setup.py` & `pydio-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['pydio']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'pydio',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': 'Simple and functional dependency injection toolkit for Python',
     'long_description': "![PyPI](https://img.shields.io/pypi/v/pydio)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pydio)\n![PyPI - License](https://img.shields.io/pypi/l/pydio)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/pydio)\n[![codecov](https://codecov.io/gh/mwiatrzyk/pydio/branch/master/graph/badge.svg?token=Y6DJDSOR6M)](https://codecov.io/gh/mwiatrzyk/pydio)\n\n# PyDio\n\nSimple and functional dependency injection toolkit for Python.\n\n## About\n\nPyDio aims to be simple, yet still powerful, allowing you to feed\ndependencies inside your application in a flexible way. PyDio design is based\non simple assumption, that dependency injection can be achieved using simple\n**key-to-function** map, where **key** specifies **type of object** you want\nto inject and **function** is a **factory** function that creates\n**instances** of that type.\n\nIn PyDio, this is implemented using **providers** and **injectors**. You use\nproviders to configure your **key-to-function** mapping, and then you use\ninjectors to perform a **lookup** of a specific key and creation of the final\nobject.\n\nHere's a simple example:\n\n```python\nimport abc\n\nfrom pydio.api import Provider, Injector\n\nprovider = Provider()\n\n@provider.provides('greet')\ndef make_greet():\n    return 'Hello, world!'\n\ndef main():\n    injector = Injector(provider)\n    greet_message = injector.inject('greet')\n    print(greet_message)\n\nif __name__ == '__main__':\n    main()\n```\n\nNow you can save the snippet from above as ``example.py`` file and execute\nto see the output:\n\n```shell\n$ python example.py\nHello, world!\n```\n\n## Key features\n\n* Support for any hashable keys: class objects, strings, ints etc.\n* Support for any type of object factories: function, coroutine, generator,\n  asynchronous generator.\n* Automatic resource management via generator-based factories\n  (similar to pytest's fixtures)\n* Multiple environment support: testing, development, production etc.\n* Limiting created object's lifetime to user-defined scopes: global,\n  application, use-case etc.\n* No singletons used, so there is no global state...\n* ...but you still can create global injector on your own if you need it :-)\n\n## Installation\n\nYou can install PyDio using one of following methods:\n\n1) From PyPI (for stable releases):\n\n    ```shell\n    $ pip install PyDio\n    ```\n\n2) From test PyPI (for stable and development releases):\n\n    ```shell\n    $ pip install -i https://test.pypi.org/simple/ PyDio\n    ```\n\n3) Directly from source code repository (for all releases):\n\n    ```shell\n    $ pip install git+https://gitlab.com/zef1r/PyDio.git@[branch-or-tag]\n    ```\n\n## Documentation\n\nYou have two options available:\n\n1) Visit [PyDio's ReadTheDocs](https://pydio.readthedocs.io/en/latest/) site.\n\n2) Take a tour around [functional tests](https://github.com/mwiatrzyk/pydio/tree/master/tests/functional).\n\n## License\n\nThis project is released under the terms of the MIT license.\n\nSee [LICENSE.txt](https://github.com/mwiatrzyk/pydio/blob/master/LICENSE.txt) for more details.\n\n## Author\n\nMaciej Wiatrzyk <maciej.wiatrzyk@gmail.com>\n",
     'author': 'Maciej Wiatrzyk',
     'author_email': 'maciej.wiatrzyk@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mwiatrzyk/pydio',
```

### Comparing `pydio-0.4.0/PKG-INFO` & `pydio-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydio
-Version: 0.4.0
+Version: 0.4.1
 Summary: Simple and functional dependency injection toolkit for Python
 Home-page: https://github.com/mwiatrzyk/pydio
 License: MIT
 Keywords: dependency,injection,di,framework,toolkit,tool,library
 Author: Maciej Wiatrzyk
 Author-email: maciej.wiatrzyk@gmail.com
 Requires-Python: >=3.7.2,<4
```


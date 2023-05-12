# Comparing `tmp/logging_journald-0.6.5.tar.gz` & `tmp/logging_journald-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logging_journald-0.6.5.tar", max compression
+gzip compressed data, was "logging_journald-0.6.6.tar", max compression
```

## Comparing `logging_journald-0.6.5.tar` & `logging_journald-0.6.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      590 2022-11-30 19:52:18.876197 logging_journald-0.6.5/README.md
--rw-r--r--   0        0        0     7738 2022-11-30 19:52:18.876955 logging_journald-0.6.5/logging_journald.py
--rw-r--r--   0        0        0     1442 2023-05-12 18:03:39.791353 logging_journald-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     1877 1970-01-01 00:00:00.000000 logging_journald-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1289 2023-05-12 21:05:35.769108 logging_journald-0.6.6/README.md
+-rw-r--r--   0        0        0     7754 2023-05-12 21:32:58.290693 logging_journald-0.6.6/logging_journald.py
+-rw-r--r--   0        0        0     1726 2023-05-12 21:19:01.387410 logging_journald-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0     2627 1970-01-01 00:00:00.000000 logging_journald-0.6.6/PKG-INFO
```

### Comparing `logging_journald-0.6.5/logging_journald.py` & `logging_journald-0.6.6/logging_journald.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,10 +258,11 @@
                             )],
                         )
             except Exception:
                 self._fallback(record)
 
 
 __all__ = (
+    "Facility",
     "JournaldLogHandler",
     "check_journal_stream",
 )
```

### Comparing `logging_journald-0.6.5/pyproject.toml` & `logging_journald-0.6.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "logging-journald"
-version = "0.6.5"
+version = "0.6.6"
 license = "MIT"
 description = "Pure python logging handler for writing logs to the journald using native protocol"
 authors = ["Dmitry Orlov <me@mosquito.su>"]
 readme = "README.md"
 homepage = "https://github.com/mosquito/logging-journald"
 classifiers = [
     "Intended Audience :: Developers",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
 packages = [
     { include = "logging_journald.py" },
 ]
 
 [tool.poetry.urls]
@@ -29,14 +30,17 @@
 python = "^3.7"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-subtests = "^0.9.0"
 aiomisc = "^16.2.10"
 mypy = "^0.991"
+coveralls = "^3.3.1"
+pytest-cov = "^4.0.0"
+pylama = {extras = ["toml"], version = "^8.4.1"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 allow_subclassing_any = true
@@ -45,7 +49,14 @@
 ignore_missing_imports = true
 implicit_reexport = true
 pretty = true
 show_error_codes = true
 strict = true
 warn_return_any = false
 files = "logging_journald.py, tests"
+
+[tool.pylama]
+max_line_length = 80
+skip = "*/.venv/*, */.tox/*, */mypy_cache/*, ./dist, ./docs"
+
+[tool.pylama.linter.mccabe]
+max-complexity = 15
```

### Comparing `logging_journald-0.6.5/PKG-INFO` & `logging_journald-0.6.6/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logging-journald
-Version: 0.6.5
+Version: 0.6.6
 Summary: Pure python logging handler for writing logs to the journald using native protocol
 Home-page: https://github.com/mosquito/logging-journald
 License: MIT
 Author: Dmitry Orlov
 Author-email: me@mosquito.su
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
@@ -15,25 +15,28 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Project-URL: Source, https://github.com/mosquito/logging-journald
 Project-URL: Tracker, https://github.com/mosquito/logging-journald/issues
 Description-Content-Type: text/markdown
 
 logging-journald
 ================
 
+[![PyPI - License](https://img.shields.io/pypi/l/logging-journald)](https://pypi.org/project/logging-journald) [![Wheel](https://img.shields.io/pypi/wheel/logging-journald)](https://pypi.org/project/logging-journald) [![PyPI](https://img.shields.io/pypi/v/logging-journald)](https://pypi.org/project/logging-journald) [![PyPI](https://img.shields.io/pypi/pyversions/logging-journald)](https://pypi.org/project/logging-journald) [![Coverage Status](https://coveralls.io/repos/github/mosquito/logging-journald/badge.svg?branch=master)](https://coveralls.io/github/mosquito/logging-journald?branch=master) ![tests](https://github.com/mosquito/logging-journald/workflows/tests/badge.svg?branch=master)
+
 Pure python logging handler for writing logs to the journald using
 native protocol.
 
 ```python
 import logging
 from logging_journald import JournaldLogHandler, check_journal_stream
```


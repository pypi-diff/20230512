# Comparing `tmp/logging_journald-0.6.4.tar.gz` & `tmp/logging_journald-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logging_journald-0.6.4.tar", max compression
+gzip compressed data, was "logging_journald-0.6.5.tar", max compression
```

## Comparing `logging_journald-0.6.4.tar` & `logging_journald-0.6.5.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0      590 2022-11-30 19:52:18.876197 logging_journald-0.6.4/README.md
--rw-r--r--   0        0        0     7738 2022-11-30 19:52:18.876955 logging_journald-0.6.4/logging_journald.py
--rw-r--r--   0        0        0     1426 2022-11-30 19:52:32.297793 logging_journald-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     1183 1970-01-01 00:00:00.000000 logging_journald-0.6.4/setup.py
--rw-r--r--   0        0        0     1813 1970-01-01 00:00:00.000000 logging_journald-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0      590 2022-11-30 19:52:18.876197 logging_journald-0.6.5/README.md
+-rw-r--r--   0        0        0     7738 2022-11-30 19:52:18.876955 logging_journald-0.6.5/logging_journald.py
+-rw-r--r--   0        0        0     1442 2023-05-12 18:03:39.791353 logging_journald-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     1877 1970-01-01 00:00:00.000000 logging_journald-0.6.5/PKG-INFO
```

### Comparing `logging_journald-0.6.4/README.md` & `logging_journald-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `logging_journald-0.6.4/logging_journald.py` & `logging_journald-0.6.5/logging_journald.py`

 * *Files identical despite different names*

### Comparing `logging_journald-0.6.4/pyproject.toml` & `logging_journald-0.6.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [tool.poetry]
 name = "logging-journald"
-version = "0.6.4"
+version = "0.6.5"
+license = "MIT"
 description = "Pure python logging handler for writing logs to the journald using native protocol"
 authors = ["Dmitry Orlov <me@mosquito.su>"]
 readme = "README.md"
 homepage = "https://github.com/mosquito/logging-journald"
 classifiers = [
     "Intended Audience :: Developers",
     "Operating System :: POSIX :: Linux",
```

### Comparing `logging_journald-0.6.4/PKG-INFO` & `logging_journald-0.6.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: logging-journald
-Version: 0.6.4
+Version: 0.6.5
 Summary: Pure python logging handler for writing logs to the journald using native protocol
 Home-page: https://github.com/mosquito/logging-journald
+License: MIT
 Author: Dmitry Orlov
 Author-email: me@mosquito.su
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


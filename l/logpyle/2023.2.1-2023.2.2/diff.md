# Comparing `tmp/logpyle-2023.2.1.tar.gz` & `tmp/logpyle-2023.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logpyle-2023.2.1.tar", last modified: Tue May  9 18:05:04 2023, max compression
+gzip compressed data, was "logpyle-2023.2.2.tar", last modified: Fri May 12 04:22:39 2023, max compression
```

## Comparing `logpyle-2023.2.1.tar` & `logpyle-2023.2.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 mdiener    (501) staff       (20)        0 2023-05-09 18:05:04.550329 logpyle-2023.2.1/
-drwxr-xr-x   0 mdiener    (501) staff       (20)        0 2023-05-09 18:05:04.544297 logpyle-2023.2.1/.github/
-drwxr-xr-x   0 mdiener    (501) staff       (20)        0 2023-05-09 18:05:04.546221 logpyle-2023.2.1/.github/workflows/
--rw-r--r--   0 mdiener    (501) staff       (20)     4846 2023-05-09 17:27:57.000000 logpyle-2023.2.1/.github/workflows/ci.yaml
--rw-r--r--   0 mdiener    (501) staff       (20)      146 2022-08-30 23:00:42.000000 logpyle-2023.2.1/.gitignore
--rw-r--r--   0 mdiener    (501) staff       (20)      220 2023-04-06 17:32:47.000000 logpyle-2023.2.1/.readthedocs.yml
--rw-r--r--   0 mdiener    (501) staff       (20)     1212 2022-08-30 23:00:42.000000 logpyle-2023.2.1/LICENSE
--rw-r--r--   0 mdiener    (501) staff       (20)     1655 2023-05-09 18:05:04.550434 logpyle-2023.2.1/PKG-INFO
--rw-r--r--   0 mdiener    (501) staff       (20)      617 2022-08-30 23:00:42.000000 logpyle-2023.2.1/README.md
-drwxr-xr-x   0 mdiener    (501) staff       (20)        0 2023-05-09 18:05:04.546910 logpyle-2023.2.1/bin/
--rwxr-xr-x   0 mdiener    (501) staff       (20)     9253 2023-04-06 17:32:47.000000 logpyle-2023.2.1/bin/logtool
--rwxr-xr-x   0 mdiener    (501) staff       (20)     1730 2023-05-09 17:27:57.000000 logpyle-2023.2.1/bin/runalyzer
--rwxr-xr-x   0 mdiener    (501) staff       (20)    13649 2023-05-09 17:27:57.000000 logpyle-2023.2.1/bin/runalyzer-gather
-drwxr-xr-x   0 mdiener    (501) staff       (20)        0 2023-05-09 18:05:04.548195 logpyle-2023.2.1/doc/
--rw-r--r--   0 mdiener    (501) staff       (20)      605 2022-08-30 23:00:42.000000 logpyle-2023.2.1/doc/Makefile
--rw-r--r--   0 mdiener    (501) staff       (20)       61 2022-08-30 23:00:42.000000 logpyle-2023.2.1/doc/api.rst
--rw-r--r--   0 mdiener    (501) staff       (20)     3227 2023-05-01 00:34:44.000000 logpyle-2023.2.1/doc/conf.py
--rw-r--r--   0 mdiener    (501) staff       (20)      755 2022-08-30 23:00:42.000000 logpyle-2023.2.1/doc/index.rst
--rw-r--r--   0 mdiener    (501) staff       (20)     4586 2023-05-09 17:27:57.000000 logpyle-2023.2.1/doc/log.rst
--rw-r--r--   0 mdiener    (501) staff       (20)     1642 2022-08-30 23:00:42.000000 logpyle-2023.2.1/doc/misc.rst
-drwxr-xr-x   0 mdiener    (501) staff       (20)        0 2023-05-09 18:05:04.548623 logpyle-2023.2.1/examples/
--rwxr-xr-x   0 mdiener    (501) staff       (20)     2080 2023-05-09 17:27:57.000000 logpyle-2023.2.1/examples/log-mpi.py
--rwxr-xr-x   0 mdiener    (501) staff       (20)     2048 2023-05-09 17:27:57.000000 logpyle-2023.2.1/examples/log.py
--rwxr-xr-x   0 mdiener    (501) staff       (20)     1487 2023-04-06 17:32:47.000000 logpyle-2023.2.1/examples/optional-log.py
-drwxr-xr-x   0 mdiener    (501) staff       (20)        0 2023-05-09 18:05:04.549598 logpyle-2023.2.1/logpyle/
--rw-r--r--   0 mdiener    (501) staff       (20)    55483 2023-05-09 17:40:49.000000 logpyle-2023.2.1/logpyle/__init__.py
--rw-r--r--   0 mdiener    (501) staff       (20)        0 2023-04-06 17:32:47.000000 logpyle-2023.2.1/logpyle/py.typed
--rw-r--r--   0 mdiener    (501) staff       (20)    15519 2023-05-09 17:27:57.000000 logpyle-2023.2.1/logpyle/runalyzer.py
--rw-r--r--   0 mdiener    (501) staff       (20)      109 2023-05-09 18:04:45.000000 logpyle-2023.2.1/logpyle/version.py
-drwxr-xr-x   0 mdiener    (501) staff       (20)        0 2023-05-09 18:05:04.550219 logpyle-2023.2.1/logpyle.egg-info/
--rw-r--r--   0 mdiener    (501) staff       (20)     1655 2023-05-09 18:05:04.000000 logpyle-2023.2.1/logpyle.egg-info/PKG-INFO
--rw-r--r--   0 mdiener    (501) staff       (20)      517 2023-05-09 18:05:04.000000 logpyle-2023.2.1/logpyle.egg-info/SOURCES.txt
--rw-r--r--   0 mdiener    (501) staff       (20)        1 2023-05-09 18:05:04.000000 logpyle-2023.2.1/logpyle.egg-info/dependency_links.txt
--rw-r--r--   0 mdiener    (501) staff       (20)       25 2023-05-09 18:05:04.000000 logpyle-2023.2.1/logpyle.egg-info/requires.txt
--rw-r--r--   0 mdiener    (501) staff       (20)        8 2023-05-09 18:05:04.000000 logpyle-2023.2.1/logpyle.egg-info/top_level.txt
--rwxr-xr-x   0 mdiener    (501) staff       (20)      159 2023-04-06 17:32:47.000000 logpyle-2023.2.1/run-mypy.sh
--rw-r--r--   0 mdiener    (501) staff       (20)      393 2023-05-09 18:05:04.550708 logpyle-2023.2.1/setup.cfg
--rw-r--r--   0 mdiener    (501) staff       (20)     1781 2023-04-26 04:03:03.000000 logpyle-2023.2.1/setup.py
+drwxr-xr-x   0 mdiener    (501) staff       (20)        0 2023-05-12 04:22:39.135694 logpyle-2023.2.2/
+drwxr-xr-x   0 mdiener    (501) staff       (20)        0 2023-05-12 04:22:39.130231 logpyle-2023.2.2/.github/
+drwxr-xr-x   0 mdiener    (501) staff       (20)        0 2023-05-12 04:22:39.132099 logpyle-2023.2.2/.github/workflows/
+-rw-r--r--   0 mdiener    (501) staff       (20)     4846 2023-05-09 17:27:57.000000 logpyle-2023.2.2/.github/workflows/ci.yaml
+-rw-r--r--   0 mdiener    (501) staff       (20)      146 2022-08-30 23:00:42.000000 logpyle-2023.2.2/.gitignore
+-rw-r--r--   0 mdiener    (501) staff       (20)      220 2023-04-06 17:32:47.000000 logpyle-2023.2.2/.readthedocs.yml
+-rw-r--r--   0 mdiener    (501) staff       (20)     1212 2022-08-30 23:00:42.000000 logpyle-2023.2.2/LICENSE
+-rw-r--r--   0 mdiener    (501) staff       (20)     1655 2023-05-12 04:22:39.135780 logpyle-2023.2.2/PKG-INFO
+-rw-r--r--   0 mdiener    (501) staff       (20)      617 2022-08-30 23:00:42.000000 logpyle-2023.2.2/README.md
+drwxr-xr-x   0 mdiener    (501) staff       (20)        0 2023-05-12 04:22:39.132779 logpyle-2023.2.2/bin/
+-rwxr-xr-x   0 mdiener    (501) staff       (20)     9253 2023-04-06 17:32:47.000000 logpyle-2023.2.2/bin/logtool
+-rwxr-xr-x   0 mdiener    (501) staff       (20)     1730 2023-05-09 17:27:57.000000 logpyle-2023.2.2/bin/runalyzer
+-rwxr-xr-x   0 mdiener    (501) staff       (20)    13649 2023-05-09 17:27:57.000000 logpyle-2023.2.2/bin/runalyzer-gather
+drwxr-xr-x   0 mdiener    (501) staff       (20)        0 2023-05-12 04:22:39.134139 logpyle-2023.2.2/doc/
+-rw-r--r--   0 mdiener    (501) staff       (20)      605 2022-08-30 23:00:42.000000 logpyle-2023.2.2/doc/Makefile
+-rw-r--r--   0 mdiener    (501) staff       (20)       61 2022-08-30 23:00:42.000000 logpyle-2023.2.2/doc/api.rst
+-rw-r--r--   0 mdiener    (501) staff       (20)     3227 2023-05-01 00:34:44.000000 logpyle-2023.2.2/doc/conf.py
+-rw-r--r--   0 mdiener    (501) staff       (20)      755 2022-08-30 23:00:42.000000 logpyle-2023.2.2/doc/index.rst
+-rw-r--r--   0 mdiener    (501) staff       (20)     4586 2023-05-09 17:27:57.000000 logpyle-2023.2.2/doc/log.rst
+-rw-r--r--   0 mdiener    (501) staff       (20)     1642 2022-08-30 23:00:42.000000 logpyle-2023.2.2/doc/misc.rst
+drwxr-xr-x   0 mdiener    (501) staff       (20)        0 2023-05-12 04:22:39.134555 logpyle-2023.2.2/examples/
+-rwxr-xr-x   0 mdiener    (501) staff       (20)     2080 2023-05-09 17:27:57.000000 logpyle-2023.2.2/examples/log-mpi.py
+-rwxr-xr-x   0 mdiener    (501) staff       (20)     2048 2023-05-09 17:27:57.000000 logpyle-2023.2.2/examples/log.py
+-rwxr-xr-x   0 mdiener    (501) staff       (20)     1487 2023-04-06 17:32:47.000000 logpyle-2023.2.2/examples/optional-log.py
+drwxr-xr-x   0 mdiener    (501) staff       (20)        0 2023-05-12 04:22:39.135083 logpyle-2023.2.2/logpyle/
+-rw-r--r--   0 mdiener    (501) staff       (20)    56725 2023-05-12 04:02:40.000000 logpyle-2023.2.2/logpyle/__init__.py
+-rw-r--r--   0 mdiener    (501) staff       (20)        0 2023-04-06 17:32:47.000000 logpyle-2023.2.2/logpyle/py.typed
+-rw-r--r--   0 mdiener    (501) staff       (20)    15519 2023-05-09 17:27:57.000000 logpyle-2023.2.2/logpyle/runalyzer.py
+-rw-r--r--   0 mdiener    (501) staff       (20)      109 2023-05-12 04:22:22.000000 logpyle-2023.2.2/logpyle/version.py
+drwxr-xr-x   0 mdiener    (501) staff       (20)        0 2023-05-12 04:22:39.135597 logpyle-2023.2.2/logpyle.egg-info/
+-rw-r--r--   0 mdiener    (501) staff       (20)     1655 2023-05-12 04:22:39.000000 logpyle-2023.2.2/logpyle.egg-info/PKG-INFO
+-rw-r--r--   0 mdiener    (501) staff       (20)      517 2023-05-12 04:22:39.000000 logpyle-2023.2.2/logpyle.egg-info/SOURCES.txt
+-rw-r--r--   0 mdiener    (501) staff       (20)        1 2023-05-12 04:22:39.000000 logpyle-2023.2.2/logpyle.egg-info/dependency_links.txt
+-rw-r--r--   0 mdiener    (501) staff       (20)       25 2023-05-12 04:22:39.000000 logpyle-2023.2.2/logpyle.egg-info/requires.txt
+-rw-r--r--   0 mdiener    (501) staff       (20)        8 2023-05-12 04:22:39.000000 logpyle-2023.2.2/logpyle.egg-info/top_level.txt
+-rwxr-xr-x   0 mdiener    (501) staff       (20)      159 2023-04-06 17:32:47.000000 logpyle-2023.2.2/run-mypy.sh
+-rw-r--r--   0 mdiener    (501) staff       (20)      393 2023-05-12 04:22:39.136035 logpyle-2023.2.2/setup.cfg
+-rw-r--r--   0 mdiener    (501) staff       (20)     1781 2023-04-26 04:03:03.000000 logpyle-2023.2.2/setup.py
```

### Comparing `logpyle-2023.2.1/.github/workflows/ci.yaml` & `logpyle-2023.2.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `logpyle-2023.2.1/LICENSE` & `logpyle-2023.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `logpyle-2023.2.1/PKG-INFO` & `logpyle-2023.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logpyle
-Version: 2023.2.1
+Version: 2023.2.2
 Summary: Time series logging for Python
 Home-page: https://github.com/illinois-ceesd/logpyle
 Author: Andreas Kloeckner
 Author-email: inform@tiker.net
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `logpyle-2023.2.1/README.md` & `logpyle-2023.2.2/README.md`

 * *Files identical despite different names*

### Comparing `logpyle-2023.2.1/bin/logtool` & `logpyle-2023.2.2/bin/logtool`

 * *Files identical despite different names*

### Comparing `logpyle-2023.2.1/bin/runalyzer` & `logpyle-2023.2.2/bin/runalyzer`

 * *Files identical despite different names*

### Comparing `logpyle-2023.2.1/bin/runalyzer-gather` & `logpyle-2023.2.2/bin/runalyzer-gather`

 * *Files identical despite different names*

### Comparing `logpyle-2023.2.1/doc/Makefile` & `logpyle-2023.2.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `logpyle-2023.2.1/doc/conf.py` & `logpyle-2023.2.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `logpyle-2023.2.1/doc/index.rst` & `logpyle-2023.2.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `logpyle-2023.2.1/doc/log.rst` & `logpyle-2023.2.2/doc/log.rst`

 * *Files identical despite different names*

### Comparing `logpyle-2023.2.1/doc/misc.rst` & `logpyle-2023.2.2/doc/misc.rst`

 * *Files identical despite different names*

### Comparing `logpyle-2023.2.1/examples/log-mpi.py` & `logpyle-2023.2.2/examples/log-mpi.py`

 * *Files identical despite different names*

### Comparing `logpyle-2023.2.1/examples/log.py` & `logpyle-2023.2.2/examples/log.py`

 * *Files identical despite different names*

### Comparing `logpyle-2023.2.1/examples/optional-log.py` & `logpyle-2023.2.2/examples/optional-log.py`

 * *Files identical despite different names*

### Comparing `logpyle-2023.2.1/logpyle/__init__.py` & `logpyle-2023.2.2/logpyle/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -405,14 +405,24 @@
     expr: Expression
     dep_data: List[_DependencyData]
     compiled: CompiledExpression
     unit: Optional[str]
     format: str
 
 
+@dataclass(frozen=True)
+class _LogWarningInfo:
+    tick_count: int
+    time: float
+    message: str
+    category: str
+    filename: str
+    lineno: int
+
+
 class LogManager:
     """A distributed-memory-capable diagnostic time-series logging facility.
     It is meant to log data from a computation, with certain log quantities
     available before a cycle, and certain other ones afterwards. A timeline of
     invocations looks as follows::
 
         tick_before()
@@ -604,44 +614,51 @@
                     # try again, someone might have created a file with the same name
                     continue
 
                 self._load()
 
             break
 
+        # {{{ warnings/logging capture
+
+        self.warning_data: List[_LogWarningInfo] = []
         self.old_showwarning: Optional[Callable[..., Any]] = None
         if capture_warnings:
             self.capture_warnings(True)
 
+        self.logging_data: List[_LogWarningInfo] = []
         self.logging_handler: Optional[logging.Handler] = None
         if capture_logging:
             self.capture_logging(True)
 
+        # }}}
+
     def capture_warnings(self, enable: bool = True) -> None:
         def _showwarning(message: Union[Warning, str], category: Type[Warning],
                          filename: str, lineno: int, file: Optional[TextIO] = None,
                          line: Optional[str] = None) -> None:
             assert self.old_showwarning
             self.old_showwarning(message, category, filename, lineno, file, line)
 
             from time import time
 
-            if self.schema_version >= 1 and self.mode[0] == "w":
-                if self.schema_version >= 2:
-                    self.db_conn.execute(
-                            "insert into warnings values (?,?,?,?,?,?,?)",
-                            (self.rank, self.tick_count, time(), str(message),
-                             str(category), filename, lineno))
-                else:
-                    self.db_conn.execute("insert into warnings values (?,?,?,?,?)",
-                            (self.tick_count, str(message), str(category),
-                                filename, lineno))
+            self.warning_data.append(_LogWarningInfo(
+                tick_count=self.tick_count,
+                time=time(),
+                message=str(message),
+                category=str(category),
+                filename=filename,
+                lineno=lineno
+            ))
 
         import warnings
         if enable:
+            if self.schema_version < 3:
+                raise ValueError("Warnings capture needs at least schema_version 3, "
+                                f" got {self.schema_version}")
             if self.old_showwarning is None:
                 self.old_showwarning = warnings.showwarning
                 warnings.showwarning = _showwarning
             else:
                 raise RuntimeError("Warnings capture was enabled twice")
         else:
             if self.old_showwarning is None:
@@ -655,23 +672,28 @@
         class LogpyleLogHandler(logging.Handler):
             def __init__(self, mgr: LogManager) -> None:
                 logging.Handler.__init__(self)
                 self.mgr = mgr
 
             def emit(self, record: logging.LogRecord) -> None:
                 from time import time
-                self.mgr.db_conn.execute(
-                    "insert into logging values (?,?,?,?,?,?,?)",
-                    (self.mgr.rank, self.mgr.tick_count, time(), record.
-                     levelname, record.getMessage(), record.pathname,
-                     record.lineno))
+                self.mgr.logging_data.append(
+                    _LogWarningInfo(tick_count=self.mgr.tick_count,
+                                time=time(),
+                                message=record.getMessage(),
+                                category=record.levelname,
+                                filename=record.pathname,
+                                lineno=record.lineno))
 
         root_logger = logging.getLogger()
 
         if enable:
+            if self.schema_version < 3:
+                raise ValueError("Logging capture needs at least schema_version 3, "
+                                f" got {self.schema_version}")
             if self.mode[0] == "w" and self.logging_handler is None:
                 self.logging_handler = LogpyleLogHandler(self)
                 root_logger.addHandler(self.logging_handler)
             elif self.logging_handler:
                 from warnings import warn
                 warn("Logging capture already enabled")
         else:
@@ -915,15 +937,38 @@
 
     def _commit(self) -> None:
         self.commit_countdown -= 1
         if self.commit_countdown <= 0:
             self.commit_countdown = self.commit_interval
             self.db_conn.commit()
 
+    def save_logging(self) -> None:
+        for log in self.logging_data:
+            self.db_conn.execute(
+                "insert into logging values (?,?,?,?,?,?,?)",
+                (self.rank, log.tick_count, log.time,
+                log.category, log.message, log.filename,
+                log.lineno))
+
+        self.logging_data = []
+
+    def save_warnings(self) -> None:
+        for w in self.warning_data:
+            self.db_conn.execute(
+                "insert into warnings values (?,?,?,?,?,?,?)",
+                (self.rank, w.tick_count, w.time, w.message,
+                    w.category, w.filename, w.lineno))
+
+        self.warning_data = []
+
     def save(self) -> None:
+        if self.mode[0] == "w":
+            self.save_logging()
+            self.save_warnings()
+
         from sqlite3 import OperationalError
         try:
             self.db_conn.commit()
         except OperationalError as e:
             from warnings import warn
             warn("encountered sqlite error during commit: %s" % e)
```

### Comparing `logpyle-2023.2.1/logpyle/runalyzer.py` & `logpyle-2023.2.2/logpyle/runalyzer.py`

 * *Files identical despite different names*

### Comparing `logpyle-2023.2.1/logpyle.egg-info/PKG-INFO` & `logpyle-2023.2.2/logpyle.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logpyle
-Version: 2023.2.1
+Version: 2023.2.2
 Summary: Time series logging for Python
 Home-page: https://github.com/illinois-ceesd/logpyle
 Author: Andreas Kloeckner
 Author-email: inform@tiker.net
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `logpyle-2023.2.1/logpyle.egg-info/SOURCES.txt` & `logpyle-2023.2.2/logpyle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logpyle-2023.2.1/setup.py` & `logpyle-2023.2.2/setup.py`

 * *Files identical despite different names*


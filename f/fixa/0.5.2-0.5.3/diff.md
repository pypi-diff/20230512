# Comparing `tmp/fixa-0.5.2.tar.gz` & `tmp/fixa-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixa-0.5.2.tar", last modified: Fri May 12 03:36:34 2023, max compression
+gzip compressed data, was "fixa-0.5.3.tar", last modified: Fri May 12 18:00:50 2023, max compression
```

## Comparing `fixa-0.5.2.tar` & `fixa-0.5.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 03:36:34.046290 fixa-0.5.2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-06 00:03:13.000000 fixa-0.5.2/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1114 2023-05-06 00:03:13.000000 fixa-0.5.2/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      312 2023-05-06 00:03:13.000000 fixa-0.5.2/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-05-12 03:36:34.046124 fixa-0.5.2/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     2986 2023-05-06 00:03:13.000000 fixa-0.5.2/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 03:36:34.042149 fixa-0.5.2/fixa/
--rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-05-06 00:03:13.000000 fixa-0.5.2/fixa/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-12 03:32:03.000000 fixa-0.5.2/fixa/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4137 2023-05-08 06:09:51.000000 fixa-0.5.2/fixa/better_enum.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      533 2023-05-06 03:13:06.000000 fixa-0.5.2/fixa/better_pathlib.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6675 2023-05-06 00:03:13.000000 fixa-0.5.2/fixa/binarysearch.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1333 2023-05-06 03:12:23.000000 fixa-0.5.2/fixa/dataclass_dataframe.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 03:36:34.042846 fixa-0.5.2/fixa/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-06 00:03:13.000000 fixa-0.5.2/fixa/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2383 2023-05-06 03:09:12.000000 fixa-0.5.2/fixa/git_cli.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5877 2023-05-06 00:03:13.000000 fixa-0.5.2/fixa/hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    12219 2023-05-06 01:55:53.000000 fixa-0.5.2/fixa/iterable.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    17600 2023-05-12 03:30:17.000000 fixa-0.5.2/fixa/nest_logger.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      469 2023-05-06 03:18:07.000000 fixa-0.5.2/fixa/os_platform.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-05-06 05:18:39.000000 fixa-0.5.2/fixa/pytest_cov_helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3145 2023-05-06 01:57:52.000000 fixa-0.5.2/fixa/rnd.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1933 2023-05-06 03:17:46.000000 fixa-0.5.2/fixa/runtime.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 03:36:34.043061 fixa-0.5.2/fixa/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      539 2023-05-06 05:18:39.000000 fixa-0.5.2/fixa/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4757 2023-05-06 00:03:13.000000 fixa-0.5.2/fixa/timer.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 03:36:34.042730 fixa-0.5.2/fixa.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-05-12 03:36:34.000000 fixa-0.5.2/fixa.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      889 2023-05-12 03:36:34.000000 fixa-0.5.2/fixa.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-12 03:36:34.000000 fixa-0.5.2/fixa.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-05-12 03:36:34.000000 fixa-0.5.2/fixa.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        5 2023-05-12 03:36:34.000000 fixa-0.5.2/fixa.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     2097 2023-05-12 03:34:36.000000 fixa-0.5.2/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      295 2023-05-06 00:03:13.000000 fixa-0.5.2/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-06 00:03:13.000000 fixa-0.5.2/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-05-06 00:03:13.000000 fixa-0.5.2/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-05-06 00:03:13.000000 fixa-0.5.2/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-12 03:36:34.046340 fixa-0.5.2/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7699 2023-05-06 00:03:13.000000 fixa-0.5.2/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 03:36:34.045788 fixa-0.5.2/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     3858 2023-05-08 05:53:35.000000 fixa-0.5.2/tests/test_better_enum.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      663 2023-05-06 02:16:38.000000 fixa-0.5.2/tests/test_better_pathlib.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1633 2023-05-06 01:48:18.000000 fixa-0.5.2/tests/test_binarysearch.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      692 2023-05-06 01:42:50.000000 fixa-0.5.2/tests/test_dataclass_dataframe.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      740 2023-05-06 03:08:57.000000 fixa-0.5.2/tests/test_git_cli.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2178 2023-05-06 01:48:41.000000 fixa-0.5.2/tests/test_hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      214 2023-05-06 01:48:59.000000 fixa-0.5.2/tests/test_import.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6529 2023-05-06 01:56:07.000000 fixa-0.5.2/tests/test_iterable.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4127 2023-05-12 03:29:46.000000 fixa-0.5.2/tests/test_nest_logger.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      661 2023-05-06 01:58:16.000000 fixa-0.5.2/tests/test_rnd.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3432 2023-05-06 02:03:21.000000 fixa-0.5.2/tests/test_timer.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:00:50.518517 fixa-0.5.3/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-06 00:03:13.000000 fixa-0.5.3/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1114 2023-05-06 00:03:13.000000 fixa-0.5.3/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      312 2023-05-06 00:03:13.000000 fixa-0.5.3/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-05-12 18:00:50.518370 fixa-0.5.3/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2986 2023-05-06 00:03:13.000000 fixa-0.5.3/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:00:50.514682 fixa-0.5.3/fixa/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-05-06 00:03:13.000000 fixa-0.5.3/fixa/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-12 18:00:33.000000 fixa-0.5.3/fixa/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4137 2023-05-08 06:09:51.000000 fixa-0.5.3/fixa/better_enum.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      533 2023-05-06 03:13:06.000000 fixa-0.5.3/fixa/better_pathlib.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6675 2023-05-06 00:03:13.000000 fixa-0.5.3/fixa/binarysearch.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1333 2023-05-06 03:12:23.000000 fixa-0.5.3/fixa/dataclass_dataframe.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:00:50.515384 fixa-0.5.3/fixa/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-06 00:03:13.000000 fixa-0.5.3/fixa/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2383 2023-05-06 03:09:12.000000 fixa-0.5.3/fixa/git_cli.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5877 2023-05-06 00:03:13.000000 fixa-0.5.3/fixa/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    12219 2023-05-06 01:55:53.000000 fixa-0.5.3/fixa/iterable.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    17911 2023-05-12 16:53:54.000000 fixa-0.5.3/fixa/nest_logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      469 2023-05-06 03:18:07.000000 fixa-0.5.3/fixa/os_platform.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-05-06 05:18:39.000000 fixa-0.5.3/fixa/pytest_cov_helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3145 2023-05-06 01:57:52.000000 fixa-0.5.3/fixa/rnd.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1933 2023-05-06 03:17:46.000000 fixa-0.5.3/fixa/runtime.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:00:50.515601 fixa-0.5.3/fixa/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      539 2023-05-06 05:18:39.000000 fixa-0.5.3/fixa/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4757 2023-05-06 00:03:13.000000 fixa-0.5.3/fixa/timer.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:00:50.515263 fixa-0.5.3/fixa.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-05-12 18:00:50.000000 fixa-0.5.3/fixa.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      889 2023-05-12 18:00:50.000000 fixa-0.5.3/fixa.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-12 18:00:50.000000 fixa-0.5.3/fixa.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-05-12 18:00:50.000000 fixa-0.5.3/fixa.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        5 2023-05-12 18:00:50.000000 fixa-0.5.3/fixa.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2338 2023-05-12 17:59:25.000000 fixa-0.5.3/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      295 2023-05-06 00:03:13.000000 fixa-0.5.3/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-06 00:03:13.000000 fixa-0.5.3/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-05-06 00:03:13.000000 fixa-0.5.3/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-05-06 00:03:13.000000 fixa-0.5.3/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-12 18:00:50.518560 fixa-0.5.3/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7699 2023-05-06 00:03:13.000000 fixa-0.5.3/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:00:50.518108 fixa-0.5.3/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3858 2023-05-08 05:53:35.000000 fixa-0.5.3/tests/test_better_enum.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      663 2023-05-06 02:16:38.000000 fixa-0.5.3/tests/test_better_pathlib.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1633 2023-05-06 01:48:18.000000 fixa-0.5.3/tests/test_binarysearch.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      692 2023-05-06 01:42:50.000000 fixa-0.5.3/tests/test_dataclass_dataframe.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      740 2023-05-06 03:08:57.000000 fixa-0.5.3/tests/test_git_cli.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2178 2023-05-06 01:48:41.000000 fixa-0.5.3/tests/test_hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      214 2023-05-06 01:48:59.000000 fixa-0.5.3/tests/test_import.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6529 2023-05-06 01:56:07.000000 fixa-0.5.3/tests/test_iterable.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4127 2023-05-12 03:29:46.000000 fixa-0.5.3/tests/test_nest_logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      661 2023-05-06 01:58:16.000000 fixa-0.5.3/tests/test_rnd.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3432 2023-05-06 02:03:21.000000 fixa-0.5.3/tests/test_timer.py
```

### Comparing `fixa-0.5.2/LICENSE.txt` & `fixa-0.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/PKG-INFO` & `fixa-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fixa
-Version: 0.5.2
+Version: 0.5.3
 Summary: Like the Ikea FIXA, it is my toolbox to fix things.
 Home-page: https://github.com/MacHu-GWU/fixa-project
-Download-URL: https://pypi.python.org/pypi/fixa/0.5.2#downloads
+Download-URL: https://pypi.python.org/pypi/fixa/0.5.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `fixa-0.5.2/README.rst` & `fixa-0.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/fixa/better_enum.py` & `fixa-0.5.3/fixa/better_enum.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/fixa/better_pathlib.py` & `fixa-0.5.3/fixa/better_pathlib.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/fixa/binarysearch.py` & `fixa-0.5.3/fixa/binarysearch.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/fixa/dataclass_dataframe.py` & `fixa-0.5.3/fixa/dataclass_dataframe.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/fixa/git_cli.py` & `fixa-0.5.3/fixa/git_cli.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/fixa/hashes.py` & `fixa-0.5.3/fixa/hashes.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/fixa/iterable.py` & `fixa-0.5.3/fixa/iterable.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/fixa/nest_logger.py` & `fixa-0.5.3/fixa/nest_logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
 
 def encode_pipe(pipe: str) -> str:
     if len(pipe) == 1:
         return pipe + " "
     elif len(pipe) == 2 and pipe[1] == " ":
         return pipe
-    else: # pragma: no cover
+    else:  # pragma: no cover
         raise ValueError
 
 
 DEFAULT_PIPE = encode_pipe("| ")
 
 
 def format_line(
@@ -188,14 +188,15 @@
     return decorator
 
 
 class NestedLogger:
     """
     A logger that supports nested logging.
     """
+
     def __init__(
         self,
         logger: T.Optional[logging.Logger] = None,
         name: T.Optional[str] = None,
         level: int = logging.INFO,
         log_format: str = "[User %(asctime)s] %(message)s",
         datetime_format: str = "%Y-%m-%d %H:%m:%S",
@@ -203,15 +204,15 @@
         if logger is None:
             self._logger = create_logger(
                 name=name,
                 level=level,
                 log_format=log_format,
                 datetime_format=datetime_format,
             )
-        else: # pragma: no cover
+        else:  # pragma: no cover
             self._logger = logger
 
         # ``_nest`` stores the current level of nesting
         self._nest = 0
         # ``_pipes`` is a first in last out stack data structure that stores
         # the list of pipe character for different level of nesting
         self._pipes = [
@@ -354,15 +355,15 @@
         self,
         pipe: T.Optional[str] = None,
     ):
         self._nest += 1
 
         if pipe is None:
             self._pipes.append(DEFAULT_PIPE)
-        else: # pragma: no cover
+        else:  # pragma: no cover
             self._pipes.append(encode_pipe(pipe))
 
     def _nested_end(self):
         self._nest -= 1
         self._pipes.pop()
 
     @contextlib.contextmanager
@@ -471,15 +472,18 @@
                 for _ in range(nest):
                     self._nested_start(pipe=pipe)
 
                 if nest == 0 and (pipe is not None):
                     last_pipe = self._pipe_start(pipe)
 
                 self.ruler(
-                    msg=start_msg.format(func_name=func.__name__),
+                    msg=start_msg.format(
+                        func_name=func.__name__,
+                        **kwargs,
+                    ),
                     char=char,
                     align=align,
                     length=length,
                     left_padding=left_padding,
                     right_padding=right_padding,
                     corner=corner,
                 )
@@ -488,29 +492,37 @@
                 try:
                     result = func(*args, **kwargs)
                 except Exception as e:
                     et = datetime.utcnow()
                     elapsed = (et - st).total_seconds()
                     self.info("")
                     self.ruler(
-                        msg=error_msg.format(func_name=func.__name__, elapsed=elapsed),
+                        msg=error_msg.format(
+                            func_name=func.__name__,
+                            elapsed=elapsed,
+                            **kwargs,
+                        ),
                         char=char,
                         align=align,
                         length=length,
                         left_padding=left_padding,
                         right_padding=right_padding,
                         corner=corner,
                     )
                     raise e
 
                 et = datetime.utcnow()
                 elapsed = (et - st).total_seconds()
                 self.info("")
                 self.ruler(
-                    msg=end_msg.format(func_name=func.__name__, elapsed=elapsed),
+                    msg=end_msg.format(
+                        func_name=func.__name__,
+                        elapsed=elapsed,
+                        **kwargs,
+                    ),
                     char=char,
                     align=align,
                     length=length,
                     left_padding=left_padding,
                     right_padding=right_padding,
                     corner=corner,
                 )
```

### Comparing `fixa-0.5.2/fixa/pytest_cov_helper.py` & `fixa-0.5.3/fixa/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/fixa/rnd.py` & `fixa-0.5.3/fixa/rnd.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/fixa/runtime.py` & `fixa-0.5.3/fixa/runtime.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/fixa/tests/__init__.py` & `fixa-0.5.3/fixa/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/fixa/timer.py` & `fixa-0.5.3/fixa/timer.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/fixa.egg-info/PKG-INFO` & `fixa-0.5.3/fixa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fixa
-Version: 0.5.2
+Version: 0.5.3
 Summary: Like the Ikea FIXA, it is my toolbox to fix things.
 Home-page: https://github.com/MacHu-GWU/fixa-project
-Download-URL: https://pypi.python.org/pypi/fixa/0.5.2#downloads
+Download-URL: https://pypi.python.org/pypi/fixa/0.5.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `fixa-0.5.2/fixa.egg-info/SOURCES.txt` & `fixa-0.5.3/fixa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/release-history.rst` & `fixa-0.5.3/release-history.rst`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.5.3 (2023-05-12)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Minor Improvements**
+
+- allow mini string template in ``nest_logger.NestedLogger.pretty_log``, ``nest_logger.NestedLogger.start_and_end``.
+
+
 0.5.2 (2023-05-11)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Miscellaneous**
 
 - add ``get_names`` method for most of enum class in ``better_enum`` module
 - add ``error_emoji`` argument to ``nest_logger.NestedLogger.start_and_end`` decorator.
```

### Comparing `fixa-0.5.2/requirements-doc.txt` & `fixa-0.5.3/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/setup.py` & `fixa-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/tests/test_better_enum.py` & `fixa-0.5.3/tests/test_better_enum.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/tests/test_better_pathlib.py` & `fixa-0.5.3/tests/test_better_pathlib.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/tests/test_binarysearch.py` & `fixa-0.5.3/tests/test_binarysearch.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/tests/test_dataclass_dataframe.py` & `fixa-0.5.3/tests/test_dataclass_dataframe.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/tests/test_git_cli.py` & `fixa-0.5.3/tests/test_git_cli.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/tests/test_hashes.py` & `fixa-0.5.3/tests/test_hashes.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/tests/test_iterable.py` & `fixa-0.5.3/tests/test_iterable.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/tests/test_nest_logger.py` & `fixa-0.5.3/tests/test_nest_logger.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/tests/test_rnd.py` & `fixa-0.5.3/tests/test_rnd.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.2/tests/test_timer.py` & `fixa-0.5.3/tests/test_timer.py`

 * *Files identical despite different names*


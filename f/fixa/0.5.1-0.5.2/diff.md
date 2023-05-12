# Comparing `tmp/fixa-0.5.1.tar.gz` & `tmp/fixa-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixa-0.5.1.tar", last modified: Sat May  6 03:38:02 2023, max compression
+gzip compressed data, was "fixa-0.5.2.tar", last modified: Fri May 12 03:36:34 2023, max compression
```

## Comparing `fixa-0.5.1.tar` & `fixa-0.5.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-06 03:38:02.808993 fixa-0.5.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-06 00:03:13.000000 fixa-0.5.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1114 2023-05-06 00:03:13.000000 fixa-0.5.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      312 2023-05-06 00:03:13.000000 fixa-0.5.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-05-06 03:38:02.808829 fixa-0.5.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     2986 2023-05-06 00:03:13.000000 fixa-0.5.1/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-06 03:38:02.804586 fixa-0.5.1/fixa/
--rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-05-06 00:03:13.000000 fixa-0.5.1/fixa/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-06 03:25:53.000000 fixa-0.5.1/fixa/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4273 2023-05-06 03:16:26.000000 fixa-0.5.1/fixa/better_enum.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      533 2023-05-06 03:13:06.000000 fixa-0.5.1/fixa/better_pathlib.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6675 2023-05-06 00:03:13.000000 fixa-0.5.1/fixa/binarysearch.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1333 2023-05-06 03:12:23.000000 fixa-0.5.1/fixa/dataclass_dataframe.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-06 03:38:02.805281 fixa-0.5.1/fixa/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-06 00:03:13.000000 fixa-0.5.1/fixa/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2383 2023-05-06 03:09:12.000000 fixa-0.5.1/fixa/git_cli.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5877 2023-05-06 00:03:13.000000 fixa-0.5.1/fixa/hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    12219 2023-05-06 01:55:53.000000 fixa-0.5.1/fixa/iterable.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    15702 2023-05-06 03:32:05.000000 fixa-0.5.1/fixa/nest_logger.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      469 2023-05-06 03:18:07.000000 fixa-0.5.1/fixa/os_platform.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-05-06 03:24:32.000000 fixa-0.5.1/fixa/pytest_cov_helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3145 2023-05-06 01:57:52.000000 fixa-0.5.1/fixa/rnd.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1933 2023-05-06 03:17:46.000000 fixa-0.5.1/fixa/runtime.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-06 03:38:02.805531 fixa-0.5.1/fixa/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      539 2023-05-06 01:41:58.000000 fixa-0.5.1/fixa/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4757 2023-05-06 00:03:13.000000 fixa-0.5.1/fixa/timer.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-06 03:38:02.805169 fixa-0.5.1/fixa.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-05-06 03:38:02.000000 fixa-0.5.1/fixa.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      889 2023-05-06 03:38:02.000000 fixa-0.5.1/fixa.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-06 03:38:02.000000 fixa-0.5.1/fixa.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-05-06 03:38:02.000000 fixa-0.5.1/fixa.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        5 2023-05-06 03:38:02.000000 fixa-0.5.1/fixa.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     1814 2023-05-06 03:36:57.000000 fixa-0.5.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      295 2023-05-06 00:03:13.000000 fixa-0.5.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-06 00:03:13.000000 fixa-0.5.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-05-06 00:03:13.000000 fixa-0.5.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-05-06 00:03:13.000000 fixa-0.5.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-06 03:38:02.809045 fixa-0.5.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7699 2023-05-06 00:03:13.000000 fixa-0.5.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-06 03:38:02.808483 fixa-0.5.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     3615 2023-05-06 02:40:34.000000 fixa-0.5.1/tests/test_better_enum.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      663 2023-05-06 02:16:38.000000 fixa-0.5.1/tests/test_better_pathlib.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1633 2023-05-06 01:48:18.000000 fixa-0.5.1/tests/test_binarysearch.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      692 2023-05-06 01:42:50.000000 fixa-0.5.1/tests/test_dataclass_dataframe.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      740 2023-05-06 03:08:57.000000 fixa-0.5.1/tests/test_git_cli.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2178 2023-05-06 01:48:41.000000 fixa-0.5.1/tests/test_hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      214 2023-05-06 01:48:59.000000 fixa-0.5.1/tests/test_import.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6529 2023-05-06 01:56:07.000000 fixa-0.5.1/tests/test_iterable.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3581 2023-05-06 03:36:08.000000 fixa-0.5.1/tests/test_nest_logger.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      661 2023-05-06 01:58:16.000000 fixa-0.5.1/tests/test_rnd.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3432 2023-05-06 02:03:21.000000 fixa-0.5.1/tests/test_timer.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 03:36:34.046290 fixa-0.5.2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-06 00:03:13.000000 fixa-0.5.2/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1114 2023-05-06 00:03:13.000000 fixa-0.5.2/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      312 2023-05-06 00:03:13.000000 fixa-0.5.2/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-05-12 03:36:34.046124 fixa-0.5.2/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2986 2023-05-06 00:03:13.000000 fixa-0.5.2/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 03:36:34.042149 fixa-0.5.2/fixa/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-05-06 00:03:13.000000 fixa-0.5.2/fixa/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-12 03:32:03.000000 fixa-0.5.2/fixa/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4137 2023-05-08 06:09:51.000000 fixa-0.5.2/fixa/better_enum.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      533 2023-05-06 03:13:06.000000 fixa-0.5.2/fixa/better_pathlib.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6675 2023-05-06 00:03:13.000000 fixa-0.5.2/fixa/binarysearch.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1333 2023-05-06 03:12:23.000000 fixa-0.5.2/fixa/dataclass_dataframe.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 03:36:34.042846 fixa-0.5.2/fixa/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-06 00:03:13.000000 fixa-0.5.2/fixa/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2383 2023-05-06 03:09:12.000000 fixa-0.5.2/fixa/git_cli.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5877 2023-05-06 00:03:13.000000 fixa-0.5.2/fixa/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    12219 2023-05-06 01:55:53.000000 fixa-0.5.2/fixa/iterable.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    17600 2023-05-12 03:30:17.000000 fixa-0.5.2/fixa/nest_logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      469 2023-05-06 03:18:07.000000 fixa-0.5.2/fixa/os_platform.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-05-06 05:18:39.000000 fixa-0.5.2/fixa/pytest_cov_helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3145 2023-05-06 01:57:52.000000 fixa-0.5.2/fixa/rnd.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1933 2023-05-06 03:17:46.000000 fixa-0.5.2/fixa/runtime.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 03:36:34.043061 fixa-0.5.2/fixa/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      539 2023-05-06 05:18:39.000000 fixa-0.5.2/fixa/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4757 2023-05-06 00:03:13.000000 fixa-0.5.2/fixa/timer.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 03:36:34.042730 fixa-0.5.2/fixa.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-05-12 03:36:34.000000 fixa-0.5.2/fixa.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      889 2023-05-12 03:36:34.000000 fixa-0.5.2/fixa.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-12 03:36:34.000000 fixa-0.5.2/fixa.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-05-12 03:36:34.000000 fixa-0.5.2/fixa.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        5 2023-05-12 03:36:34.000000 fixa-0.5.2/fixa.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2097 2023-05-12 03:34:36.000000 fixa-0.5.2/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      295 2023-05-06 00:03:13.000000 fixa-0.5.2/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-06 00:03:13.000000 fixa-0.5.2/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-05-06 00:03:13.000000 fixa-0.5.2/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-05-06 00:03:13.000000 fixa-0.5.2/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-12 03:36:34.046340 fixa-0.5.2/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7699 2023-05-06 00:03:13.000000 fixa-0.5.2/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 03:36:34.045788 fixa-0.5.2/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3858 2023-05-08 05:53:35.000000 fixa-0.5.2/tests/test_better_enum.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      663 2023-05-06 02:16:38.000000 fixa-0.5.2/tests/test_better_pathlib.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1633 2023-05-06 01:48:18.000000 fixa-0.5.2/tests/test_binarysearch.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      692 2023-05-06 01:42:50.000000 fixa-0.5.2/tests/test_dataclass_dataframe.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      740 2023-05-06 03:08:57.000000 fixa-0.5.2/tests/test_git_cli.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2178 2023-05-06 01:48:41.000000 fixa-0.5.2/tests/test_hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      214 2023-05-06 01:48:59.000000 fixa-0.5.2/tests/test_import.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6529 2023-05-06 01:56:07.000000 fixa-0.5.2/tests/test_iterable.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4127 2023-05-12 03:29:46.000000 fixa-0.5.2/tests/test_nest_logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      661 2023-05-06 01:58:16.000000 fixa-0.5.2/tests/test_rnd.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3432 2023-05-06 02:03:21.000000 fixa-0.5.2/tests/test_timer.py
```

### Comparing `fixa-0.5.1/LICENSE.txt` & `fixa-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fixa-0.5.1/PKG-INFO` & `fixa-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fixa
-Version: 0.5.1
+Version: 0.5.2
 Summary: Like the Ikea FIXA, it is my toolbox to fix things.
 Home-page: https://github.com/MacHu-GWU/fixa-project
-Download-URL: https://pypi.python.org/pypi/fixa/0.5.1#downloads
+Download-URL: https://pypi.python.org/pypi/fixa/0.5.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `fixa-0.5.1/README.rst` & `fixa-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `fixa-0.5.1/fixa/better_enum.py` & `fixa-0.5.2/fixa/better_enum.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,33 @@
 Improve the original enum module.
 """
 
 import typing as T
 import enum
 
 
-class BetterIntEnum(int, enum.Enum):
+class Mixin:
+    @classmethod
+    def get_by_name(cls, name: str):
+        return cls[name]
+
+    @classmethod
+    def is_valid_name(cls, name: str) -> bool:
+        try:
+            _ = cls[name]
+            return True
+        except KeyError:
+            return False
+
+    @classmethod
+    def get_names(cls) -> T.List[str]:
+        return [i.name for i in cls]
+
+
+class BetterIntEnum(Mixin, int, enum.Enum):
     """
     Example:
 
     .. code-block:: python
 
         >>> class CodeEnum(BetterIntEnum):
         ...     succeeded = 1
@@ -43,30 +61,18 @@
         >>> CodeEnum.ensure_int(CodeEnum.succeeded)
         1
         >>> isinstance(CodeEnum.ensure_int(1), int)
         True
     """
 
     @classmethod
-    def get_by_name(cls, name: str):
-        return cls[name]
-
-    @classmethod
     def get_by_value(cls, value: int):
         return cls(value)
 
     @classmethod
-    def is_valid_name(cls, name: str) -> bool:
-        try:
-            _ = cls[name]
-            return True
-        except KeyError:
-            return False
-
-    @classmethod
     def is_valid_value(cls, value: int) -> bool:
         try:
             _ = cls(value)
             return True
         except ValueError:
             return False
 
@@ -79,19 +85,19 @@
     def ensure_int(cls, value: T.Union[int, "BetterIntEnum"]) -> int:
         if isinstance(value, cls):
             return value.value
         else:
             return cls(value).value
 
     @classmethod
-    def value_list(cls) -> T.List[int]:
+    def get_values(cls) -> T.List[int]:
         return [i.value for i in cls]
 
 
-class BetterStrEnum(str, enum.Enum):
+class BetterStrEnum(Mixin, str, enum.Enum):
     """
     Example:
 
     .. code-block:: python
 
         >>> class StatusEnum(BetterStrEnum):
         ...     succeeded = "SUCCEEDED"
@@ -118,30 +124,18 @@
         >>> StatusEnum.ensure_str(StatusEnum.succeeded)
         'SUCCEEDED'
         >>> isinstance(StatusEnum.ensure_str("SUCCEEDED"), str)
         True
     """
 
     @classmethod
-    def get_by_name(cls, name: str):
-        return cls[name]
-
-    @classmethod
     def get_by_value(cls, value: str):
         return cls(value)
 
     @classmethod
-    def is_valid_name(cls, name: str) -> bool:
-        try:
-            _ = cls[name]
-            return True
-        except KeyError:
-            return False
-
-    @classmethod
     def is_valid_value(cls, value: str) -> bool:
         try:
             _ = cls(value)
             return True
         except ValueError:
             return False
 
@@ -154,9 +148,9 @@
     def ensure_str(cls, value: T.Union[str, "BetterStrEnum"]) -> str:
         if isinstance(value, cls):
             return value.value
         else:
             return cls(value).value
 
     @classmethod
-    def value_list(cls) -> T.List[str]:
+    def get_values(cls) -> T.List[str]:
         return [i.value for i in cls]
```

### Comparing `fixa-0.5.1/fixa/better_pathlib.py` & `fixa-0.5.2/fixa/better_pathlib.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.1/fixa/binarysearch.py` & `fixa-0.5.2/fixa/binarysearch.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.1/fixa/dataclass_dataframe.py` & `fixa-0.5.2/fixa/dataclass_dataframe.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.1/fixa/git_cli.py` & `fixa-0.5.2/fixa/git_cli.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.1/fixa/hashes.py` & `fixa-0.5.2/fixa/hashes.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.1/fixa/iterable.py` & `fixa-0.5.2/fixa/iterable.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.1/fixa/nest_logger.py` & `fixa-0.5.2/fixa/nest_logger.py`

 * *Files 20% similar despite different names*

```diff
@@ -185,14 +185,17 @@
     """
     fix pycharm type hint bug for decorator.
     """
     return decorator
 
 
 class NestedLogger:
+    """
+    A logger that supports nested logging.
+    """
     def __init__(
         self,
         logger: T.Optional[logging.Logger] = None,
         name: T.Optional[str] = None,
         level: int = logging.INFO,
         log_format: str = "[User %(asctime)s] %(message)s",
         datetime_format: str = "%Y-%m-%d %H:%m:%S",
@@ -261,60 +264,78 @@
 
     def debug(
         self,
         msg: str,
         indent: int = 0,
         pipe: T.Optional[str] = None,
     ) -> str:  # pragma: no cover
+        """
+        Todo: add docstring
+        """
         return self._log(self._logger.debug, msg, indent, pipe)
 
     def info(
         self,
         msg: str,
         indent: int = 0,
         pipe: T.Optional[str] = None,
     ) -> str:
+        """
+        Todo: add docstring
+        """
         return self._log(self._logger.info, msg, indent, pipe)
 
     def warning(
         self,
         msg: str,
         indent: int = 0,
         pipe: T.Optional[str] = None,
     ) -> str:  # pragma: no cover
+        """
+        Todo: add docstring
+        """
         return self._log(self._logger.warning, msg, indent, pipe)
 
     def error(
         self,
         msg: str,
         indent: int = 0,
         pipe: T.Optional[str] = None,
     ) -> str:  # pragma: no cover
+        """
+        Todo: add docstring
+        """
         return self._log(self._logger.error, msg, indent, pipe)
 
     def critical(
         self,
         msg: str,
         indent: int = 0,
         pipe: T.Optional[str] = None,
     ) -> str:  # pragma: no cover
+        """
+        Todo: add docstring
+        """
         return self._log(self._logger.critical, msg, indent, pipe)
 
     def ruler(
         self,
         msg: str,
         char: str = "-",
         align: AlignEnum = AlignEnum.left,
         length: int = 80,
         left_padding: int = 5,
         right_padding: int = 5,
         corner: str = "+",
         pipe: T.Optional[str] = None,
         func: T.Optional[T.Callable] = None,
     ) -> str:
+        """
+        Todo: add docstring
+        """
         if func is None:
             func = self._logger.info
 
         with self.pipe(pipe=pipe):
             output = format_ruler(
                 msg,
                 char,
@@ -345,24 +366,55 @@
         self._pipes.pop()
 
     @contextlib.contextmanager
     def nested(
         self,
         pipe: T.Optional[str] = None,
     ):
+        """
+        A context manager that nest logging for one more level.
+
+        Example:
+
+        .. code-block:: python
+
+            logger.ruler("section 1")
+            logger.info("hello 1")
+            with logger.nested():
+                logger.ruler("section 1.1")
+                logger.info("hello 1.1")
+                with logger.nested():
+                    logger.ruler("section 1.1.1")
+                    logger.info("hello 1.1.1")
+                    logger.ruler("section 1.1.1")
+                logger.ruler("section 1.1")
+            logger.ruler("section 1")
+
+        The output looks like::
+
+            [User] +----- section 1 -------------------------------------------+
+            [User] | hello 1
+            [User] | +----- section 1.1 ---------------------------------------+
+            [User] | | hello 1.1
+            [User] | | +----- section 1.1.1 -----------------------------------+
+            [User] | | | hello 1.1.1
+            [User] | | +----- section 1.1.1 -----------------------------------+
+            [User] | +----- section 1.1 ---------------------------------------+
+            [User] +----- section 1 -------------------------------------------+
+        """
         self._nested_start(pipe=pipe)
         try:
             yield self
         finally:
             self._nested_end()
 
     def pretty_log(
         self,
         start_msg: str = "Start {func_name}()",
-        error_msg: str = "Error, elapsed = {elapsed:.2f} sec",
+        error_msg: str = "Error {func_name}(), elapsed = {elapsed:.2f} sec",
         end_msg: str = "End {func_name}(), elapsed = {elapsed:.2f} sec",
         char: str = "-",
         align: AlignEnum = AlignEnum.left,
         length: int = 80,
         left_padding: int = 5,
         right_padding: int = 5,
         corner: str = "+",
@@ -436,15 +488,15 @@
                 try:
                     result = func(*args, **kwargs)
                 except Exception as e:
                     et = datetime.utcnow()
                     elapsed = (et - st).total_seconds()
                     self.info("")
                     self.ruler(
-                        msg=error_msg.format(elapsed=elapsed),
+                        msg=error_msg.format(func_name=func.__name__, elapsed=elapsed),
                         char=char,
                         align=align,
                         length=length,
                         left_padding=left_padding,
                         right_padding=right_padding,
                         corner=corner,
                     )
@@ -474,58 +526,63 @@
             return wrapper
 
         return deco
 
     def start_and_end(
         self,
         msg: str,
-        start_emoji: str = "",
-        end_emoji: str = "",
+        start_emoji: str = "🟢",
+        error_emoji: str = "🔴",
+        end_emoji: str = "🟢",
         pipe: str = "| ",
     ):
         """
         A simplified version of the ``pretty_log`` decorator. Visually print
         the start and the end of a function.
 
         Example:
 
         .. code-block:: python
 
             @logger.start_and_end(
                 msg="My Function 1",
                 start_emoji="🟢",
-                end_emoji="🔴",
+                error_emoji="🔴",
+                end_emoji="🟢",
                 pipe="📦",
             )
             def my_func1(name: str):
                 time.sleep(1)
                 logger.info(f"{name} do something in my func 1")
 
             my_func1(name="alice")
 
         The output looks like::
 
             [User] +----- ⏱ 🟢 Start 'My Function 1' --------------------------+
             [User] 📦
             [User] 📦 alice do something in my func 1
             [User] 📦
-            [User] +----- ⏰ 🔴 End 'My Function 1', elapsed = 1.01 sec --------+
+            [User] +----- ⏰ 🟢 End 'My Function 1', elapsed = 1.01 sec --------+
 
         :param msg: indicate the name of the function
         :param start_emoji: custom emoji for the start message
         :param end_emoji: custom emoji for the end message
         :param pipe: custom pipe character
         :return:
         """
         if start_emoji and (not start_emoji.endswith(" ")):
             start_emoji = start_emoji + " "
+        if error_emoji and (not error_emoji.endswith(" ")):
+            error_emoji = error_emoji + " "
         if end_emoji and (not end_emoji.endswith(" ")):
             end_emoji = end_emoji + " "
         return self.pretty_log(
             start_msg=f"⏱ {start_emoji}Start {msg!r}",
+            error_msg=f"⏰ {error_emoji}Error {msg!r}, elapsed = {{elapsed:.2f}} sec",
             end_msg=f"⏰ {end_emoji}End {msg!r}, elapsed = {{elapsed:.2f}} sec",
             pipe=pipe,
         )
 
     @contextlib.contextmanager
     def disabled(
         self,
```

### Comparing `fixa-0.5.1/fixa/pytest_cov_helper.py` & `fixa-0.5.2/fixa/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.1/fixa/rnd.py` & `fixa-0.5.2/fixa/rnd.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.1/fixa/runtime.py` & `fixa-0.5.2/fixa/runtime.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.1/fixa/tests/__init__.py` & `fixa-0.5.2/fixa/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.1/fixa/timer.py` & `fixa-0.5.2/fixa/timer.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.1/fixa.egg-info/PKG-INFO` & `fixa-0.5.2/fixa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fixa
-Version: 0.5.1
+Version: 0.5.2
 Summary: Like the Ikea FIXA, it is my toolbox to fix things.
 Home-page: https://github.com/MacHu-GWU/fixa-project
-Download-URL: https://pypi.python.org/pypi/fixa/0.5.1#downloads
+Download-URL: https://pypi.python.org/pypi/fixa/0.5.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `fixa-0.5.1/fixa.egg-info/SOURCES.txt` & `fixa-0.5.2/fixa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixa-0.5.1/release-history.rst` & `fixa-0.5.2/release-history.rst`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,22 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.5.2 (2023-05-11)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Miscellaneous**
+
+- add ``get_names`` method for most of enum class in ``better_enum`` module
+- add ``error_emoji`` argument to ``nest_logger.NestedLogger.start_and_end`` decorator.
+
+
 0.5.1 (2023-05-05)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - add ``better_pathlib``
 - add ``dataclass_dataframe``
 - add ``pytest_cov_helper``
```

### Comparing `fixa-0.5.1/requirements-doc.txt` & `fixa-0.5.2/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `fixa-0.5.1/setup.py` & `fixa-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.1/tests/test_better_enum.py` & `fixa-0.5.2/tests/test_better_enum.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     succeeded = 1
     failed = 0
 
 
 class TestBetterIntEnum:
     def test(self):
         assert CodeEnum.succeeded == 1
+        assert 0 < CodeEnum.succeeded < 2
         assert (CodeEnum.succeeded + 1) == 2
         assert {CodeEnum.succeeded, CodeEnum.failed} == {0, 1}
 
     def test_get_by_name(self):
         assert CodeEnum.get_by_name("succeeded") is CodeEnum.succeeded
         with pytest.raises(KeyError):
             CodeEnum.get_by_name(1)
@@ -48,25 +49,27 @@
         assert CodeEnum.ensure_int(CodeEnum.succeeded) == 1
         assert isinstance(CodeEnum.ensure_int(1), int)
         assert isinstance(CodeEnum.ensure_int(CodeEnum.succeeded), int)
 
         with pytest.raises(ValueError):
             CodeEnum.ensure_int(9)
 
-    def test_value_list(self):
-        assert CodeEnum.value_list() == [1, 0]
+    def test_get_names_values(self):
+        assert CodeEnum.get_names() == ["succeeded", "failed"]
+        assert CodeEnum.get_values() == [1, 0]
 
 
 class StatusEnum(BetterStrEnum):
     succeeded = "SUCCEEDED"
     failed = "FAILED"
 
 
 class TestBetterStrEnum:
     def test(self):
+        assert StatusEnum.succeeded.replace("SUC", "") == "CEEDED"
         assert StatusEnum.succeeded == "SUCCEEDED"
         assert f"it is {StatusEnum.succeeded}" == "it is SUCCEEDED"
         assert {StatusEnum.succeeded, StatusEnum.failed} == {"SUCCEEDED", "FAILED"}
 
     def test_get_by_name(self):
         assert StatusEnum.get_by_name("succeeded") is StatusEnum.succeeded
         with pytest.raises(KeyError):
@@ -96,14 +99,15 @@
         assert isinstance(StatusEnum.ensure_str("SUCCEEDED"), str)
         assert isinstance(StatusEnum.ensure_str(StatusEnum.succeeded), str)
 
         with pytest.raises(ValueError):
             StatusEnum.ensure_str("succeeded")
 
     def test_value_list(self):
-        assert StatusEnum.value_list() == ["SUCCEEDED", "FAILED"]
+        assert StatusEnum.get_names() == ["succeeded", "failed"]
+        assert StatusEnum.get_values() == ["SUCCEEDED", "FAILED"]
 
 
 if __name__ == "__main__":
     from fixa.tests import run_cov_test
 
     run_cov_test(__file__, "fixa.better_enum", preview=False)
```

### Comparing `fixa-0.5.1/tests/test_better_pathlib.py` & `fixa-0.5.2/tests/test_better_pathlib.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.1/tests/test_binarysearch.py` & `fixa-0.5.2/tests/test_binarysearch.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.1/tests/test_dataclass_dataframe.py` & `fixa-0.5.2/tests/test_dataclass_dataframe.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.1/tests/test_git_cli.py` & `fixa-0.5.2/tests/test_git_cli.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.1/tests/test_hashes.py` & `fixa-0.5.2/tests/test_hashes.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.1/tests/test_iterable.py` & `fixa-0.5.2/tests/test_iterable.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.1/tests/test_nest_logger.py` & `fixa-0.5.2/tests/test_nest_logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 logger = NestedLogger(name="nested_logger_unit_test")
 
 
 def setup_module(module):
     print("")
 
 
-def test_format_line():
+def _test_format_line():
     assert format_line("hello") == "| hello"
     assert format_line("hello", nest=1) == "| | hello"
     assert format_line("hello", nest=1, _pipes=["| ", "# "]) == "| # hello"
 
     assert format_line("hello", indent=1) == "|   hello"
     assert format_line("hello", indent=1, nest=1) == "| |   hello"
     assert format_line("hello", indent=1, nest=1, _pipes=["| ", "# "]) == "| #   hello"
 
 
-def test_format_ruler():
+def _test_format_ruler():
     assert format_ruler("Hello", length=40) == (
         "---------------- Hello -----------------"
     )
     assert format_ruler("Hello", length=20) == ("------ Hello -------")
     assert format_ruler("Hello", char="=", length=40) == (
         "================ Hello ================="
     )
@@ -47,42 +47,42 @@
         "--- Hello ------------------------------"
     )
     assert format_ruler("Hello", right_padding=3, align=AlignEnum.right, length=40) == (
         "------------------------------ Hello ---"
     )
 
 
-def test_nested_context_manager():
+def _test_nested_context_manager():
     print("")
     logger.ruler("section 1")
     logger.info("hello 1")
     with logger.nested():
         logger.ruler("section 1.1")
         logger.info("hello 1.1")
         with logger.nested():
             logger.ruler("section 1.1.1")
             logger.info("hello 1.1.1")
             logger.ruler("section 1.1.1")
         logger.ruler("section 1.1")
     logger.ruler("section 1")
 
 
-def test_disabled_context_manager():
+def _test_disabled_context_manager():
     print("")
 
     logger.info("a")
     with logger.disabled(
         disable=True,
         # disable=False,
     ):
         logger.info("b")
     logger.info("c")
 
 
-def test_pretty_log_decorator():
+def _test_pretty_log_decorator():
     print("")
 
     @logger.pretty_log(pipe="🏭")
     def run_build():
         time.sleep(1)
         logger.info("run build")
 
@@ -96,16 +96,15 @@
     @logger.pretty_log(pipe="🚀")
     def run_deploy():
         time.sleep(1)
         logger.info("run deploy")
         with logger.nested():
             run_test()
 
-    run_deploy()
-
+    # run_deploy()
 
     @logger.pretty_log()
     def this_wont_work():
         logger.info("run this_wont_work")
         raise Exception("something wrong")
 
     @logger.pretty_log()
@@ -114,27 +113,50 @@
         with logger.nested():
             this_wont_work()
 
     with pytest.raises(Exception):
         outter_may_work()
 
 
-def test_block():
+def _test_block():
     print("")
 
     @logger.start_and_end(
         msg="My Function 1",
-        start_emoji="🟢",
-        end_emoji="🔴",
         pipe="📦",
     )
     def my_func1(name: str):
         time.sleep(1)
         logger.info(f"{name} do something in my func 1")
 
     my_func1(name="alice")
 
+    @logger.start_and_end(
+        msg="My Function 2",
+        pipe="📦",
+    )
+    def my_func2(name: str):
+        time.sleep(1)
+        logger.info(f"{name} do something in my func 1")
+        raise ValueError("something wrong")
+
+    with pytest.raises(Exception):
+        my_func2(name="alice")
+
+
+def test():
+    with logger.disabled(
+        disable=True,
+        # disable=False,
+    ):
+        _test_format_line()
+        _test_format_ruler()
+        _test_nested_context_manager()
+        _test_disabled_context_manager()
+        _test_pretty_log_decorator()
+        _test_block()
+
 
 if __name__ == "__main__":
     from fixa.tests import run_cov_test
 
     run_cov_test(__file__, "fixa.nest_logger", preview=False)
```

### Comparing `fixa-0.5.1/tests/test_rnd.py` & `fixa-0.5.2/tests/test_rnd.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.1/tests/test_timer.py` & `fixa-0.5.2/tests/test_timer.py`

 * *Files identical despite different names*


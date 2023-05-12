# Comparing `tmp/python-cli-handler-0.1.1.tar.gz` & `tmp/python-cli-handler-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-cli-handler-0.1.1.tar", last modified: Wed Nov  9 04:03:27 2022, max compression
+gzip compressed data, was "python-cli-handler-1.0.0.tar", last modified: Fri May 12 07:52:26 2023, max compression
```

## Comparing `python-cli-handler-0.1.1.tar` & `python-cli-handler-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 lam        (502) staff       (20)        0 2022-11-09 04:03:27.358284 python-cli-handler-0.1.1/
--rw-r--r--   0 lam        (502) staff       (20)     1129 2022-11-08 09:34:27.000000 python-cli-handler-0.1.1/LICENSE
--rw-r--r--   0 lam        (502) staff       (20)      822 2022-11-09 04:03:27.357828 python-cli-handler-0.1.1/PKG-INFO
--rw-r--r--   0 lam        (502) staff       (20)      260 2022-11-09 04:02:23.000000 python-cli-handler-0.1.1/README.md
--rw-r--r--   0 lam        (502) staff       (20)       89 2022-11-08 09:34:27.000000 python-cli-handler-0.1.1/pyproject.toml
--rw-r--r--   0 lam        (502) staff       (20)       38 2022-11-09 04:03:27.358436 python-cli-handler-0.1.1/setup.cfg
--rw-r--r--   0 lam        (502) staff       (20)     1027 2022-11-09 04:02:23.000000 python-cli-handler-0.1.1/setup.py
-drwxr-xr-x   0 lam        (502) staff       (20)        0 2022-11-09 04:03:27.345829 python-cli-handler-0.1.1/src/
-drwxr-xr-x   0 lam        (502) staff       (20)        0 2022-11-09 04:03:27.349433 python-cli-handler-0.1.1/src/cli_scheduler/
--rw-r--r--   0 lam        (502) staff       (20)       61 2022-11-09 04:02:54.000000 python-cli-handler-0.1.1/src/cli_scheduler/__init__.py
--rw-r--r--   0 lam        (502) staff       (20)     2370 2022-11-09 03:14:39.000000 python-cli-handler-0.1.1/src/cli_scheduler/cli_job.py
-drwxr-xr-x   0 lam        (502) staff       (20)        0 2022-11-09 04:03:27.350775 python-cli-handler-0.1.1/src/cli_scheduler/constants/
--rw-r--r--   0 lam        (502) staff       (20)        0 2022-11-08 09:41:36.000000 python-cli-handler-0.1.1/src/cli_scheduler/constants/__init__.py
--rw-r--r--   0 lam        (502) staff       (20)       71 2022-11-08 09:43:52.000000 python-cli-handler-0.1.1/src/cli_scheduler/constants/time_constants.py
--rw-r--r--   0 lam        (502) staff       (20)     1874 2022-11-09 03:16:02.000000 python-cli-handler-0.1.1/src/cli_scheduler/handler.py
-drwxr-xr-x   0 lam        (502) staff       (20)        0 2022-11-09 04:03:27.354224 python-cli-handler-0.1.1/src/cli_scheduler/utils/
--rw-r--r--   0 lam        (502) staff       (20)        0 2022-11-08 09:32:37.000000 python-cli-handler-0.1.1/src/cli_scheduler/utils/__init__.py
--rw-r--r--   0 lam        (502) staff       (20)      512 2022-11-08 09:34:27.000000 python-cli-handler-0.1.1/src/cli_scheduler/utils/function_utils.py
--rw-r--r--   0 lam        (502) staff       (20)      777 2022-10-18 03:30:15.000000 python-cli-handler-0.1.1/src/cli_scheduler/utils/logger_utils.py
--rw-r--r--   0 lam        (502) staff       (20)      310 2022-11-08 09:43:52.000000 python-cli-handler-0.1.1/src/cli_scheduler/utils/time_utils.py
-drwxr-xr-x   0 lam        (502) staff       (20)        0 2022-11-09 04:03:27.357176 python-cli-handler-0.1.1/src/python_cli_handler.egg-info/
--rw-r--r--   0 lam        (502) staff       (20)      822 2022-11-09 04:03:27.000000 python-cli-handler-0.1.1/src/python_cli_handler.egg-info/PKG-INFO
--rw-r--r--   0 lam        (502) staff       (20)      555 2022-11-09 04:03:27.000000 python-cli-handler-0.1.1/src/python_cli_handler.egg-info/SOURCES.txt
--rw-r--r--   0 lam        (502) staff       (20)        1 2022-11-09 04:03:27.000000 python-cli-handler-0.1.1/src/python_cli_handler.egg-info/dependency_links.txt
--rw-r--r--   0 lam        (502) staff       (20)       14 2022-11-09 04:03:27.000000 python-cli-handler-0.1.1/src/python_cli_handler.egg-info/top_level.txt
+drwxr-xr-x   0 lam        (502) staff       (20)        0 2023-05-12 07:52:26.002519 python-cli-handler-1.0.0/
+-rw-r--r--   0 lam        (502) staff       (20)     1129 2022-11-08 09:34:27.000000 python-cli-handler-1.0.0/LICENSE
+-rw-r--r--   0 lam        (502) staff       (20)     2271 2023-05-12 07:52:26.001799 python-cli-handler-1.0.0/PKG-INFO
+-rw-r--r--   0 lam        (502) staff       (20)     1708 2023-05-12 06:43:02.000000 python-cli-handler-1.0.0/README.md
+-rw-r--r--   0 lam        (502) staff       (20)       89 2022-11-08 09:34:27.000000 python-cli-handler-1.0.0/pyproject.toml
+-rw-r--r--   0 lam        (502) staff       (20)       38 2023-05-12 07:52:26.002691 python-cli-handler-1.0.0/setup.cfg
+-rw-r--r--   0 lam        (502) staff       (20)     1027 2022-11-09 04:02:23.000000 python-cli-handler-1.0.0/setup.py
+drwxr-xr-x   0 lam        (502) staff       (20)        0 2023-05-12 07:52:25.981040 python-cli-handler-1.0.0/src/
+drwxr-xr-x   0 lam        (502) staff       (20)        0 2023-05-12 07:52:25.989295 python-cli-handler-1.0.0/src/cli_scheduler/
+-rw-r--r--   0 lam        (502) staff       (20)       61 2023-05-12 04:31:51.000000 python-cli-handler-1.0.0/src/cli_scheduler/__init__.py
+-rw-r--r--   0 lam        (502) staff       (20)     2428 2023-05-12 04:29:26.000000 python-cli-handler-1.0.0/src/cli_scheduler/cli_job.py
+drwxr-xr-x   0 lam        (502) staff       (20)        0 2023-05-12 07:52:25.991451 python-cli-handler-1.0.0/src/cli_scheduler/constants/
+-rw-r--r--   0 lam        (502) staff       (20)        0 2022-11-08 09:41:36.000000 python-cli-handler-1.0.0/src/cli_scheduler/constants/__init__.py
+-rw-r--r--   0 lam        (502) staff       (20)      338 2023-05-12 04:29:26.000000 python-cli-handler-1.0.0/src/cli_scheduler/constants/time_constants.py
+-rw-r--r--   0 lam        (502) staff       (20)     1874 2022-11-09 03:16:02.000000 python-cli-handler-1.0.0/src/cli_scheduler/handler.py
+-rw-r--r--   0 lam        (502) staff       (20)     5350 2023-05-12 04:29:26.000000 python-cli-handler-1.0.0/src/cli_scheduler/scheduler_job.py
+drwxr-xr-x   0 lam        (502) staff       (20)        0 2023-05-12 07:52:25.995810 python-cli-handler-1.0.0/src/cli_scheduler/utils/
+-rw-r--r--   0 lam        (502) staff       (20)        0 2022-11-08 09:32:37.000000 python-cli-handler-1.0.0/src/cli_scheduler/utils/__init__.py
+-rw-r--r--   0 lam        (502) staff       (20)      512 2022-11-08 09:34:27.000000 python-cli-handler-1.0.0/src/cli_scheduler/utils/function_utils.py
+-rw-r--r--   0 lam        (502) staff       (20)      777 2022-10-18 03:30:15.000000 python-cli-handler-1.0.0/src/cli_scheduler/utils/logger_utils.py
+-rw-r--r--   0 lam        (502) staff       (20)      464 2023-05-12 05:00:35.000000 python-cli-handler-1.0.0/src/cli_scheduler/utils/time_utils.py
+drwxr-xr-x   0 lam        (502) staff       (20)        0 2023-05-12 07:52:26.000536 python-cli-handler-1.0.0/src/python_cli_handler.egg-info/
+-rw-r--r--   0 lam        (502) staff       (20)     2271 2023-05-12 07:52:25.000000 python-cli-handler-1.0.0/src/python_cli_handler.egg-info/PKG-INFO
+-rw-r--r--   0 lam        (502) staff       (20)      590 2023-05-12 07:52:25.000000 python-cli-handler-1.0.0/src/python_cli_handler.egg-info/SOURCES.txt
+-rw-r--r--   0 lam        (502) staff       (20)        1 2023-05-12 07:52:25.000000 python-cli-handler-1.0.0/src/python_cli_handler.egg-info/dependency_links.txt
+-rw-r--r--   0 lam        (502) staff       (20)       14 2023-05-12 07:52:25.000000 python-cli-handler-1.0.0/src/python_cli_handler.egg-info/top_level.txt
```

### Comparing `python-cli-handler-0.1.1/LICENSE` & `python-cli-handler-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-cli-handler-0.1.1/setup.py` & `python-cli-handler-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-cli-handler-0.1.1/src/cli_scheduler/cli_job.py` & `python-cli-handler-1.0.0/src/cli_scheduler/cli_job.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 from cli_scheduler.utils.logger_utils import get_logger
 from cli_scheduler.utils.time_utils import round_timestamp
 
 logger = get_logger('CLI Job')
 
 
 class CLIJob:
+    """
+    Deprecated. Use SchedulerJob instead.
+    """
     def __init__(self, interval=None, end_timestamp=None, retry=True):
         self.interval = interval
         self.end_timestamp = end_timestamp
 
         self.retry = retry
 
     def run(self, *args, **kwargs):
```

### Comparing `python-cli-handler-0.1.1/src/cli_scheduler/handler.py` & `python-cli-handler-1.0.0/src/cli_scheduler/handler.py`

 * *Files identical despite different names*

### Comparing `python-cli-handler-0.1.1/src/cli_scheduler/utils/function_utils.py` & `python-cli-handler-1.0.0/src/cli_scheduler/utils/function_utils.py`

 * *Files identical despite different names*

### Comparing `python-cli-handler-0.1.1/src/cli_scheduler/utils/logger_utils.py` & `python-cli-handler-1.0.0/src/cli_scheduler/utils/logger_utils.py`

 * *Files identical despite different names*

### Comparing `python-cli-handler-0.1.1/src/python_cli_handler.egg-info/SOURCES.txt` & `python-cli-handler-1.0.0/src/python_cli_handler.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/cli_scheduler/__init__.py
 src/cli_scheduler/cli_job.py
 src/cli_scheduler/handler.py
+src/cli_scheduler/scheduler_job.py
 src/cli_scheduler/constants/__init__.py
 src/cli_scheduler/constants/time_constants.py
 src/cli_scheduler/utils/__init__.py
 src/cli_scheduler/utils/function_utils.py
 src/cli_scheduler/utils/logger_utils.py
 src/cli_scheduler/utils/time_utils.py
 src/python_cli_handler.egg-info/PKG-INFO
```


# Comparing `tmp/lupin-grognard-2.0.0.dev1.tar.gz` & `tmp/lupin-grognard-2.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lupin-grognard-2.0.0.dev1.tar", last modified: Wed May 10 10:36:50 2023, max compression
+gzip compressed data, was "lupin-grognard-2.0.0.dev2.tar", last modified: Fri May 12 07:38:05 2023, max compression
```

## Comparing `lupin-grognard-2.0.0.dev1.tar` & `lupin-grognard-2.0.0.dev2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 10:36:50.381422 lupin-grognard-2.0.0.dev1/
--rw-rw-rw-   0        0        0     1091 2022-10-26 14:21:00.000000 lupin-grognard-2.0.0.dev1/LICENCE
--rw-rw-rw-   0        0        0       36 2023-03-02 22:35:36.000000 lupin-grognard-2.0.0.dev1/MANIFEST.in
--rw-rw-rw-   0        0        0      513 2023-05-10 10:36:50.382422 lupin-grognard-2.0.0.dev1/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-01-20 08:07:36.000000 lupin-grognard-2.0.0.dev1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 10:36:50.258725 lupin-grognard-2.0.0.dev1/lupin_grognard/
--rw-rw-rw-   0        0        0       28 2023-05-10 10:36:50.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/__init__.py
--rw-rw-rw-   0        0        0       77 2023-05-05 22:45:05.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:36:50.288257 lupin-grognard-2.0.0.dev1/lupin_grognard/core/
--rw-rw-rw-   0        0        0        0 2022-11-28 17:09:18.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/core/__init__.py
--rw-rw-rw-   0        0        0     2183 2023-05-05 22:45:05.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/core/check.py
--rw-rw-rw-   0        0        0      912 2022-12-09 16:33:58.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/core/cmd.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:36:50.304772 lupin-grognard-2.0.0.dev1/lupin_grognard/core/commit/
--rw-rw-rw-   0        0        0        0 2023-01-17 13:04:34.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/core/commit/__init__.py
--rw-rw-rw-   0        0        0     7379 2023-05-05 22:45:05.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/core/commit/commit.py
--rw-rw-rw-   0        0        0     1037 2023-05-10 10:03:25.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/core/commit/commit_error.py
--rw-rw-rw-   0        0        0     1816 2023-03-17 09:49:38.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/core/commit/commit_reporter.py
--rw-rw-rw-   0        0        0     5739 2023-05-10 10:03:25.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/core/commit/commit_validator.py
--rw-rw-rw-   0        0        0     1319 2023-05-10 10:16:15.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/core/config.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:36:50.327796 lupin-grognard-2.0.0.dev1/lupin_grognard/core/doc_generator/
--rw-rw-rw-   0        0        0        0 2023-03-17 11:16:03.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/core/doc_generator/__init__.py
--rw-rw-rw-   0        0        0    11923 2023-05-05 22:45:05.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/core/doc_generator/changelog.py
--rw-rw-rw-   0        0        0     1706 2023-05-10 10:03:25.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/core/doc_generator/jinja_generator.py
--rw-rw-rw-   0        0        0     5017 2023-05-05 22:45:05.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/core/doc_generator/reviewlog.py
--rw-rw-rw-   0        0        0     1625 2023-05-10 10:00:16.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/core/doc_generator/ros2_docs.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:36:50.345357 lupin-grognard-2.0.0.dev1/lupin_grognard/core/format/
--rw-rw-rw-   0        0        0        0 2023-02-10 13:59:49.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/core/format/__init__.py
--rw-rw-rw-   0        0        0     2709 2023-05-10 10:03:25.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/core/format/clang_format.py
--rw-rw-rw-   0        0        0     2598 2023-05-10 10:03:25.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/core/format/cmake_format.py
--rw-rw-rw-   0        0        0     4040 2023-03-31 14:48:27.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/core/git.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:36:50.347360 lupin-grognard-2.0.0.dev1/lupin_grognard/core/tools/
--rw-rw-rw-   0        0        0        0 2022-11-28 17:09:18.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/core/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:36:50.364897 lupin-grognard-2.0.0.dev1/lupin_grognard/core/tools/ros2/
--rw-rw-rw-   0        0        0        0 2023-05-05 22:45:05.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/core/tools/ros2/__init__.py
--rw-rw-rw-   0        0        0     2654 2023-05-10 10:03:25.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/core/tools/ros2/interfaces.py
--rw-rw-rw-   0        0        0     2415 2023-05-10 10:36:24.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/core/tools/ros2/package.py
--rw-rw-rw-   0        0        0    35591 2023-05-10 10:14:40.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/core/tools/ros2/parser.py
--rw-rw-rw-   0        0        0     4128 2023-03-31 10:47:54.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/core/tools/utils.py
--rw-rw-rw-   0        0        0     6324 2023-05-10 10:33:33.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/run.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:36:50.380424 lupin-grognard-2.0.0.dev1/lupin_grognard/templates/
--rw-rw-rw-   0        0        0     1848 2023-05-04 13:34:03.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/templates/changelog.j2
--rw-rw-rw-   0        0        0     3390 2023-03-24 10:41:51.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/templates/reviewlog.j2
--rw-rw-rw-   0        0        0      438 2023-05-09 21:16:03.000000 lupin-grognard-2.0.0.dev1/lupin_grognard/templates/rosapi.j2
-drwxrwxrwx   0        0        0        0 2023-05-10 10:36:50.275235 lupin-grognard-2.0.0.dev1/lupin_grognard.egg-info/
--rw-rw-rw-   0        0        0      513 2023-05-10 10:36:50.000000 lupin-grognard-2.0.0.dev1/lupin_grognard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1468 2023-05-10 10:36:50.000000 lupin-grognard-2.0.0.dev1/lupin_grognard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 10:36:50.000000 lupin-grognard-2.0.0.dev1/lupin_grognard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-10 10:36:50.000000 lupin-grognard-2.0.0.dev1/lupin_grognard.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-11-23 21:32:45.000000 lupin-grognard-2.0.0.dev1/lupin_grognard.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      133 2023-05-10 10:36:50.000000 lupin-grognard-2.0.0.dev1/lupin_grognard.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-10 10:36:50.000000 lupin-grognard-2.0.0.dev1/lupin_grognard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      938 2023-05-10 10:36:50.383422 lupin-grognard-2.0.0.dev1/setup.cfg
--rw-rw-rw-   0        0        0      171 2022-11-28 17:09:18.000000 lupin-grognard-2.0.0.dev1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:38:05.497585 lupin-grognard-2.0.0.dev2/
+-rw-rw-rw-   0        0        0     1091 2022-10-26 14:21:00.000000 lupin-grognard-2.0.0.dev2/LICENCE
+-rw-rw-rw-   0        0        0       36 2023-03-02 22:35:36.000000 lupin-grognard-2.0.0.dev2/MANIFEST.in
+-rw-rw-rw-   0        0        0      513 2023-05-12 07:38:05.497585 lupin-grognard-2.0.0.dev2/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-01-20 08:07:36.000000 lupin-grognard-2.0.0.dev2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 07:38:05.447971 lupin-grognard-2.0.0.dev2/lupin_grognard/
+-rw-rw-rw-   0        0        0       28 2023-05-12 07:38:05.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/__init__.py
+-rw-rw-rw-   0        0        0       77 2023-05-11 09:26:56.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:38:05.475324 lupin-grognard-2.0.0.dev2/lupin_grognard/core/
+-rw-rw-rw-   0        0        0        0 2022-11-28 17:09:18.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/__init__.py
+-rw-rw-rw-   0        0        0     2227 2023-05-11 14:39:06.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/check.py
+-rw-rw-rw-   0        0        0      912 2022-12-09 16:33:58.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/cmd.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:38:05.479834 lupin-grognard-2.0.0.dev2/lupin_grognard/core/commit/
+-rw-rw-rw-   0        0        0        0 2023-01-17 13:04:34.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/commit/__init__.py
+-rw-rw-rw-   0        0        0     7379 2023-05-11 09:26:56.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/commit/commit.py
+-rw-rw-rw-   0        0        0     1274 2023-05-12 07:35:54.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/commit/commit_error.py
+-rw-rw-rw-   0        0        0     1816 2023-03-17 09:49:38.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/commit/commit_reporter.py
+-rw-rw-rw-   0        0        0     5739 2023-05-12 07:34:25.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/commit/commit_validator.py
+-rw-rw-rw-   0        0        0     1395 2023-05-12 07:34:47.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/config.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:38:05.484833 lupin-grognard-2.0.0.dev2/lupin_grognard/core/doc_generator/
+-rw-rw-rw-   0        0        0        0 2023-03-17 11:16:03.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/doc_generator/__init__.py
+-rw-rw-rw-   0        0        0    11923 2023-05-11 09:26:56.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/doc_generator/changelog.py
+-rw-rw-rw-   0        0        0     1706 2023-05-12 07:34:25.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/doc_generator/jinja_generator.py
+-rw-rw-rw-   0        0        0     5017 2023-05-11 09:26:56.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/doc_generator/reviewlog.py
+-rw-rw-rw-   0        0        0     1625 2023-05-11 09:26:56.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/doc_generator/ros2_docs.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:38:05.487834 lupin-grognard-2.0.0.dev2/lupin_grognard/core/format/
+-rw-rw-rw-   0        0        0        0 2023-02-10 13:59:49.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/format/__init__.py
+-rw-rw-rw-   0        0        0     2709 2023-05-12 07:34:25.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/format/clang_format.py
+-rw-rw-rw-   0        0        0     2598 2023-05-12 07:34:25.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/format/cmake_format.py
+-rw-rw-rw-   0        0        0     4040 2023-03-31 14:48:27.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/git.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:38:05.490077 lupin-grognard-2.0.0.dev2/lupin_grognard/core/tools/
+-rw-rw-rw-   0        0        0        0 2022-11-28 17:09:18.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:38:05.493586 lupin-grognard-2.0.0.dev2/lupin_grognard/core/tools/ros2/
+-rw-rw-rw-   0        0        0        0 2023-05-11 09:26:56.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/tools/ros2/__init__.py
+-rw-rw-rw-   0        0        0     2654 2023-05-12 07:34:25.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/tools/ros2/interfaces.py
+-rw-rw-rw-   0        0        0     2640 2023-05-11 14:11:15.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/tools/ros2/package.py
+-rw-rw-rw-   0        0        0    35591 2023-05-11 09:26:56.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/tools/ros2/parser.py
+-rw-rw-rw-   0        0        0     3867 2023-05-12 07:35:36.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/tools/utils.py
+-rw-rw-rw-   0        0        0     6718 2023-05-12 07:35:36.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/run.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:38:05.496586 lupin-grognard-2.0.0.dev2/lupin_grognard/templates/
+-rw-rw-rw-   0        0        0     1848 2023-05-04 13:34:03.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/templates/changelog.j2
+-rw-rw-rw-   0        0        0     3390 2023-03-24 10:41:51.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/templates/reviewlog.j2
+-rw-rw-rw-   0        0        0      454 2023-05-11 09:26:56.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/templates/rosapi.j2
+drwxrwxrwx   0        0        0        0 2023-05-12 07:38:05.469326 lupin-grognard-2.0.0.dev2/lupin_grognard.egg-info/
+-rw-rw-rw-   0        0        0      513 2023-05-12 07:38:05.000000 lupin-grognard-2.0.0.dev2/lupin_grognard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1468 2023-05-12 07:38:05.000000 lupin-grognard-2.0.0.dev2/lupin_grognard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 07:38:05.000000 lupin-grognard-2.0.0.dev2/lupin_grognard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-12 07:38:05.000000 lupin-grognard-2.0.0.dev2/lupin_grognard.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-11-23 21:32:45.000000 lupin-grognard-2.0.0.dev2/lupin_grognard.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      133 2023-05-12 07:38:05.000000 lupin-grognard-2.0.0.dev2/lupin_grognard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-12 07:38:05.000000 lupin-grognard-2.0.0.dev2/lupin_grognard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      938 2023-05-12 07:38:05.499090 lupin-grognard-2.0.0.dev2/setup.cfg
+-rw-rw-rw-   0        0        0      171 2022-11-28 17:09:18.000000 lupin-grognard-2.0.0.dev2/setup.py
```

### Comparing `lupin-grognard-2.0.0.dev1/LICENCE` & `lupin-grognard-2.0.0.dev2/LICENCE`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev1/PKG-INFO` & `lupin-grognard-2.0.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lupin-grognard
-Version: 2.0.0.dev1
+Version: 2.0.0.dev2
 Summary: Lupin linter tool
 License: MIT License
 Keywords: cli,linter
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lupin-grognard-2.0.0.dev1/lupin_grognard/core/check.py` & `lupin-grognard-2.0.0.dev2/lupin_grognard/core/check.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             f"Error: found {major_commit_count} major commits to check in the "
             f"current branch while the maximum allowed number is {major_commit_limit}"
         )
         sys.exit(1)
     return True
 
 
-def check_commit(commits: List, merge_option: int) -> None:
+def check_commit(commits: List, merge_option: int, permisive: bool = False) -> None:
     """
     check_commit performs validation checks on each commit.
     If merge_option is set to 0, the function checks that merge commits
     have approvers.
     If merge_option is 1, the function only validates the title for a merge,
     the title and the body of the commit if it is a simple commit.
     The function also calls the error_report method of the ErrorCount
@@ -51,8 +51,8 @@
         commits (List): List of commits to check
         merge_option (int): 0 or 1
     """
     error_counter = ErrorCount()
     for c in commits:
         commit = CommitValidator(commit=c, error_counter=error_counter)
         commit.perform_checks(merge_option)
-    error_counter.error_report()
+    error_counter.error_report(permisive=permisive)
```

### Comparing `lupin-grognard-2.0.0.dev1/lupin_grognard/core/cmd.py` & `lupin-grognard-2.0.0.dev2/lupin_grognard/core/cmd.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev1/lupin_grognard/core/commit/commit.py` & `lupin-grognard-2.0.0.dev2/lupin_grognard/core/commit/commit.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev1/lupin_grognard/core/commit/commit_error.py` & `lupin-grognard-2.0.0.dev2/lupin_grognard/core/commit/commit_error.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from lupin_grognard.core.config import (
     BODY_FAILED,
     FAILED,
     MERGE_FAILED,
     SUCCESS,
     TITLE_FAILED,
 )
+from lupin_grognard.core.tools.utils import warn
 
 
 class ErrorCount:
     def __init__(self):
         self.body_error = 0
         self.title_error = 0
         self.merge_error = 0
@@ -20,22 +21,27 @@
 
     def increment_title_error(self):
         self.title_error += 1
 
     def increment_merge_error(self):
         self.merge_error += 1
 
-    def error_report(self):
+    def error_report(self, permisive: bool):
         if not (self.title_error + self.body_error + self.merge_error):
             print(SUCCESS)
         else:
             print(FAILED)
             print(
                 f"Errors found: {self.title_error + self.body_error + self.merge_error}"
             )
             if self.title_error > 0:
                 print(TITLE_FAILED)
             if self.body_error > 0:
                 print(BODY_FAILED)
             if self.merge_error > 0:
                 print(MERGE_FAILED)
-            sys.exit(1)
+
+            if permisive:
+                warn(msg="ignoring command failure because running in permissive mode")
+                sys.exit(0)
+            else:
+                sys.exit(1)
```

### Comparing `lupin-grognard-2.0.0.dev1/lupin_grognard/core/commit/commit_reporter.py` & `lupin-grognard-2.0.0.dev2/lupin_grognard/core/commit/commit_reporter.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev1/lupin_grognard/core/commit/commit_validator.py` & `lupin-grognard-2.0.0.dev2/lupin_grognard/core/commit/commit_validator.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev1/lupin_grognard/core/config.py` & `lupin-grognard-2.0.0.dev2/lupin_grognard/core/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+MAIN_BRANCHES_LIST = ["main", "master", "dev", "develop", "development"]
+
 INITIAL_COMMIT = [
     "Initial commit",  # Generated by GitLab
     "Add README.md",  # Generated by GitKraken
 ]
 
 COMMIT_DELIMITER = "--commit-delimiter--"
```

### Comparing `lupin-grognard-2.0.0.dev1/lupin_grognard/core/doc_generator/changelog.py` & `lupin-grognard-2.0.0.dev2/lupin_grognard/core/doc_generator/changelog.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev1/lupin_grognard/core/doc_generator/jinja_generator.py` & `lupin-grognard-2.0.0.dev2/lupin_grognard/core/doc_generator/jinja_generator.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev1/lupin_grognard/core/doc_generator/reviewlog.py` & `lupin-grognard-2.0.0.dev2/lupin_grognard/core/doc_generator/reviewlog.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev1/lupin_grognard/core/doc_generator/ros2_docs.py` & `lupin-grognard-2.0.0.dev2/lupin_grognard/core/doc_generator/ros2_docs.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev1/lupin_grognard/core/format/clang_format.py` & `lupin-grognard-2.0.0.dev2/lupin_grognard/core/format/clang_format.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev1/lupin_grognard/core/format/cmake_format.py` & `lupin-grognard-2.0.0.dev2/lupin_grognard/core/format/cmake_format.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev1/lupin_grognard/core/git.py` & `lupin-grognard-2.0.0.dev2/lupin_grognard/core/git.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev1/lupin_grognard/core/tools/ros2/interfaces.py` & `lupin-grognard-2.0.0.dev2/lupin_grognard/core/tools/ros2/interfaces.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev1/lupin_grognard/core/tools/ros2/package.py` & `lupin-grognard-2.0.0.dev2/lupin_grognard/core/tools/ros2/package.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from typing import List, Union
 
-from lupin_grognard.core.tools.utils import die
 from lupin_grognard.core.tools.ros2.interfaces import Action, Msg, Srv
+from lupin_grognard.core.tools.utils import die
 
 
 def find_ros_packages(path: str) -> List[str]:
     """
     Retrieves the names of ROS packages present in the directory `path` and its subdirectories.
 
     :param path: Absolute path of the directory to explore.
@@ -15,15 +15,15 @@
     :rtype: List[str]
     """
     package_xml_files = []
     for root, dirs, files in os.walk(path):
         for file in files:
             if file == "package.xml":
                 package_xml_files.append(root)
-    
+
     if len(package_xml_files) == 0:
         raise die(msg=f"No ROS package found in {path}")
     return package_xml_files
 
 
 class PackageRos2:
     def __init__(self, package_path: str):
@@ -33,15 +33,20 @@
 
     def _get_package_description(self) -> str:
         package_xml = os.path.join(self.package_path, "package.xml")
         if os.path.isfile(package_xml):
             with open(package_xml, "r", encoding="utf-8") as f:
                 for line in f:
                     if "<description>" in line:
-                        return line.split("<description>")[1].split("</description>")[0]
+                        description = line.split("<description>")[1].split(
+                            "</description>"
+                        )[0]
+                        if description.endswith("."):
+                            description = description.rstrip(".")
+                        return description
         return ""
 
     def _find_files(self, file_type: str) -> List[Union[Msg, Srv, Action]]:
         """
         Finds all files of a given type in the package directory.
 
         :param file_type: Type of files to search for, either "msg", "srv", or "action".
```

### Comparing `lupin-grognard-2.0.0.dev1/lupin_grognard/core/tools/ros2/parser.py` & `lupin-grognard-2.0.0.dev2/lupin_grognard/core/tools/ros2/parser.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev1/lupin_grognard/core/tools/utils.py` & `lupin-grognard-2.0.0.dev2/lupin_grognard/core/tools/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,33 +35,22 @@
         if group is not None:
             version = version + str(group)
     content = f'__version__ = "{version}"\n'
     write_file(file="lupin_grognard/__init__.py", content=content)
     return version
 
 
-def create_branch_list(branches_name: str) -> List:
-    comma = branches_name.find(",")
-    if comma == -1:
-        branch_list = branches_name.split()
-    else:
-        branches_name = branches_name.replace(",", " ")
-        branch_list = branches_name.split()
-    return branch_list
-
-
-def display_current_branch_name() -> None:
+def get_current_branch_name() -> str:
     branch_name = Git().get_branch_name()
     # branch name can be messing if running in CI
     if not branch_name:
         branch_name = os.getenv("CI_COMMIT_BRANCH")
     if not branch_name:
-        print("Warning: failed to get current branch name")
-    else:
-        print(f"Current branch: {branch_name}")
+        return ""
+    return branch_name
 
 
 def display_supported_commit_types() -> None:
     commit_type = [
         "build(add|change|remove)",
         "bump",
         "ci",
@@ -133,7 +122,11 @@
     return os.path.isfile(file_path)
 
 
 def configure_logging():
     logging.basicConfig(
         format="%(asctime)s %(levelname)s: %(message)s", level=logging.INFO
     )
+
+
+def is_main_branch(branch_name: str, main_branch_list: List) -> bool:
+    return branch_name in main_branch_list
```

### Comparing `lupin-grognard-2.0.0.dev1/lupin_grognard/run.py` & `lupin-grognard-2.0.0.dev2/lupin_grognard/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import os
-from typing import Optional
 
 import typer
 from dotenv import load_dotenv
 
 from lupin_grognard.__init__ import __version__
 from lupin_grognard.core.check import check_commit, check_max_allowed_major_commits
 from lupin_grognard.core.commit.commit import Commit
+from lupin_grognard.core.config import MAIN_BRANCHES_LIST
 from lupin_grognard.core.doc_generator.changelog import Changelog
 from lupin_grognard.core.doc_generator.reviewlog import Reviewlog
 from lupin_grognard.core.doc_generator.ros2_docs import Ros2Docs
 from lupin_grognard.core.format.clang_format import ClangFormatter
 from lupin_grognard.core.format.cmake_format import CMakeFormatter
 from lupin_grognard.core.git import Git
 from lupin_grognard.core.tools.ros2.package import find_ros_packages
 
 from .core.tools.utils import (
     configure_logging,
-    create_branch_list,
     die,
-    display_current_branch_name,
     display_number_of_commits_to_check,
     display_supported_commit_types,
     generate_commit_list,
     generate_commits_range_to_check,
+    get_current_branch_name,
+    info,
+    is_main_branch,
 )
 
 load_dotenv()
 GROG_BRANCHES = os.getenv("GROG_BRANCHES")
 GROG_MAX_ALLOWED_COMMITS = os.getenv("GROG_MAX_ALLOWED_COMMITS")
 GROG_DONT_CHECK_FOR_APPROVERS = os.getenv("GROG_DONT_CHECK_FOR_APPROVERS")
 GROG_CLANG_FORMAT = os.getenv("GROG_CLANG_FORMAT")
@@ -53,24 +54,25 @@
         0,
         "--grog-dont-check-for-approvers",
         "-dont-approvers",
         envvar="GROG_DONT_CHECK_FOR_APPROVERS",
         min=0,
         max=1,
     ),
-    branches_name: Optional[str] = typer.Argument(
-        default="master, main, dev, develop, development", envvar="GROG_BRANCHES"
+    permisive: bool = typer.Option(
+        False, "--permisive", "-p", help="ignore command failure"
     ),
 ):
     """
     Supported commit types: build(add|change|remove), bump, ci, deps(add|change|remove), docs, enabler,
     feat(add|change|remove), fix, refactor, test.
     Only one major commit types allowed per branch: "enabler", "feat", "fix" or "refactor".
 
-    Check every commit message since the last "merge request" in any of the branches in the branches_name list
+    Check every commit message since the last "merge request" in any of the branches in the
+    main_branches_list : "main", "master", "dev", "develop", "development"
 
     - With --all option :
     grog check-commits [--all or -a] to check all commits from initial commit
 
     - With --grog-max-allowed-commits option :
     grog check-commits [--grog-max-allowed-commits or -max] {int} to set the maximum number
     of commits allowed to the branch.
@@ -78,43 +80,49 @@
 
     - With --grog-dont-check-for-approvers option :
     by default, grog check commits will check for approvers in the Merge commit.
     grog check-commits [--grog-dont-check-for-approvers or -dont-approvers] 1 to disable option
 
     - With branches_name argument: grog check-commits "branch_1, branch_2..."
 
-    You can set GROG_BRANCHES, GROG_MAX_ALLOWED_COMMITS and GROG_DONT_CHECK_FOR_APPROVERS
+    You can set GROG_MAX_ALLOWED_COMMITS and GROG_DONT_CHECK_FOR_APPROVERS
     env var in .env, .gitlab-ci.yml, gitlab...
     """
     configure_logging()
     git = Git()
     if all:  # --all option
         git_log = git.get_log()
         grog_max_allowed_commits = 0
     else:
         git_log = git.get_log(max_line_count=50, first_parent=True)
     if git_log.stderr:
         die(f"git error {git_log.return_code}, {git_log.stderr}")
 
-    branch_list = create_branch_list(branches_name=branches_name)
     commit_list = generate_commit_list(data=git_log.stdout)
     display_supported_commit_types()
-    display_current_branch_name()
+    current_branch_name = get_current_branch_name()
+    info(f"Current branch: {current_branch_name}")
 
-    if all:  # --all option
+    if all or is_main_branch(current_branch_name, MAIN_BRANCHES_LIST):  # --all option
+        if is_main_branch(current_branch_name, MAIN_BRANCHES_LIST):
+            info(
+                msg=f"Processing all commits since current branch '{current_branch_name}' is a main one"
+            )
         if check_max_allowed_major_commits(
             commits_string=commit_list, major_commit_limit=grog_max_allowed_commits
         ):
             display_number_of_commits_to_check(commit_list=commit_list)
             check_commit(
-                commits=commit_list, merge_option=grog_dont_check_for_approvers
+                commits=commit_list,
+                merge_option=grog_dont_check_for_approvers,
+                permisive=permisive,
             )
     else:
         commit_range_list_to_check = generate_commits_range_to_check(
-            branch_list=branch_list, commit_list=commit_list
+            branch_list=MAIN_BRANCHES_LIST, commit_list=commit_list
         )
         if check_max_allowed_major_commits(
             commits_string=commit_range_list_to_check,
             major_commit_limit=grog_max_allowed_commits,
         ):
             display_number_of_commits_to_check(commit_list=commit_range_list_to_check)
             check_commit(
@@ -162,15 +170,17 @@
     commit_list = generate_commit_list(data=git_log.stdout)
     commits = Commit.add_additional_commit_info(commit_list=commit_list)
     Reviewlog(commits=commits).generate()
 
 
 @cli.command()
 def ros2docs(
-    path: str = typer.Option(..., "--path", "-p", help="path to search for ROS2 packages")
+    path: str = typer.Option(
+        ..., "--path", "-p", help="path to search for ROS2 packages"
+    )
 ):
     """Generate ROS2 documentation"""
     configure_logging()
 
     ros_packages = find_ros_packages(path)
     for path in ros_packages:
         api_doc = Ros2Docs(path=path)
```

### Comparing `lupin-grognard-2.0.0.dev1/lupin_grognard/templates/changelog.j2` & `lupin-grognard-2.0.0.dev2/lupin_grognard/templates/changelog.j2`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev1/lupin_grognard/templates/reviewlog.j2` & `lupin-grognard-2.0.0.dev2/lupin_grognard/templates/reviewlog.j2`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev1/lupin_grognard.egg-info/PKG-INFO` & `lupin-grognard-2.0.0.dev2/lupin_grognard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lupin-grognard
-Version: 2.0.0.dev1
+Version: 2.0.0.dev2
 Summary: Lupin linter tool
 License: MIT License
 Keywords: cli,linter
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lupin-grognard-2.0.0.dev1/lupin_grognard.egg-info/SOURCES.txt` & `lupin-grognard-2.0.0.dev2/lupin_grognard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev1/setup.cfg` & `lupin-grognard-2.0.0.dev2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 7570 696e 2d67 726f 676e 6172   = lupin-grognar
 00000020: 640d 0a76 6572 7369 6f6e 203d 2032 2e30  d..version = 2.0
-00000030: 2e30 2e64 6576 310d 0a64 6573 6372 6970  .0.dev1..descrip
+00000030: 2e30 2e64 6576 320d 0a64 6573 6372 6970  .0.dev2..descrip
 00000040: 7469 6f6e 203d 204c 7570 696e 206c 696e  tion = Lupin lin
 00000050: 7465 7220 746f 6f6c 0d0a 6c6f 6e67 5f64  ter tool..long_d
 00000060: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
 00000070: 653a 2052 4541 444d 452e 6d64 0d0a 6b65  e: README.md..ke
 00000080: 7977 6f72 6473 203d 2063 6c69 2c20 6c69  ywords = cli, li
 00000090: 6e74 6572 0d0a 6c69 6365 6e73 6520 3d20  nter..license = 
 000000a0: 4d49 5420 4c69 6365 6e73 650d 0a63 6c61  MIT License..cla
```


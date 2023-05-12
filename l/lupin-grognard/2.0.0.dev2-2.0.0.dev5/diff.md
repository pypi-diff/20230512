# Comparing `tmp/lupin-grognard-2.0.0.dev2.tar.gz` & `tmp/lupin-grognard-2.0.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lupin-grognard-2.0.0.dev2.tar", last modified: Fri May 12 07:38:05 2023, max compression
+gzip compressed data, was "lupin-grognard-2.0.0.dev5.tar", last modified: Fri May 12 10:15:20 2023, max compression
```

## Comparing `lupin-grognard-2.0.0.dev2.tar` & `lupin-grognard-2.0.0.dev5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 07:38:05.497585 lupin-grognard-2.0.0.dev2/
--rw-rw-rw-   0        0        0     1091 2022-10-26 14:21:00.000000 lupin-grognard-2.0.0.dev2/LICENCE
--rw-rw-rw-   0        0        0       36 2023-03-02 22:35:36.000000 lupin-grognard-2.0.0.dev2/MANIFEST.in
--rw-rw-rw-   0        0        0      513 2023-05-12 07:38:05.497585 lupin-grognard-2.0.0.dev2/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-01-20 08:07:36.000000 lupin-grognard-2.0.0.dev2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 07:38:05.447971 lupin-grognard-2.0.0.dev2/lupin_grognard/
--rw-rw-rw-   0        0        0       28 2023-05-12 07:38:05.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/__init__.py
--rw-rw-rw-   0        0        0       77 2023-05-11 09:26:56.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 07:38:05.475324 lupin-grognard-2.0.0.dev2/lupin_grognard/core/
--rw-rw-rw-   0        0        0        0 2022-11-28 17:09:18.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/__init__.py
--rw-rw-rw-   0        0        0     2227 2023-05-11 14:39:06.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/check.py
--rw-rw-rw-   0        0        0      912 2022-12-09 16:33:58.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/cmd.py
-drwxrwxrwx   0        0        0        0 2023-05-12 07:38:05.479834 lupin-grognard-2.0.0.dev2/lupin_grognard/core/commit/
--rw-rw-rw-   0        0        0        0 2023-01-17 13:04:34.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/commit/__init__.py
--rw-rw-rw-   0        0        0     7379 2023-05-11 09:26:56.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/commit/commit.py
--rw-rw-rw-   0        0        0     1274 2023-05-12 07:35:54.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/commit/commit_error.py
--rw-rw-rw-   0        0        0     1816 2023-03-17 09:49:38.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/commit/commit_reporter.py
--rw-rw-rw-   0        0        0     5739 2023-05-12 07:34:25.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/commit/commit_validator.py
--rw-rw-rw-   0        0        0     1395 2023-05-12 07:34:47.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/config.py
-drwxrwxrwx   0        0        0        0 2023-05-12 07:38:05.484833 lupin-grognard-2.0.0.dev2/lupin_grognard/core/doc_generator/
--rw-rw-rw-   0        0        0        0 2023-03-17 11:16:03.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/doc_generator/__init__.py
--rw-rw-rw-   0        0        0    11923 2023-05-11 09:26:56.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/doc_generator/changelog.py
--rw-rw-rw-   0        0        0     1706 2023-05-12 07:34:25.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/doc_generator/jinja_generator.py
--rw-rw-rw-   0        0        0     5017 2023-05-11 09:26:56.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/doc_generator/reviewlog.py
--rw-rw-rw-   0        0        0     1625 2023-05-11 09:26:56.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/doc_generator/ros2_docs.py
-drwxrwxrwx   0        0        0        0 2023-05-12 07:38:05.487834 lupin-grognard-2.0.0.dev2/lupin_grognard/core/format/
--rw-rw-rw-   0        0        0        0 2023-02-10 13:59:49.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/format/__init__.py
--rw-rw-rw-   0        0        0     2709 2023-05-12 07:34:25.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/format/clang_format.py
--rw-rw-rw-   0        0        0     2598 2023-05-12 07:34:25.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/format/cmake_format.py
--rw-rw-rw-   0        0        0     4040 2023-03-31 14:48:27.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/git.py
-drwxrwxrwx   0        0        0        0 2023-05-12 07:38:05.490077 lupin-grognard-2.0.0.dev2/lupin_grognard/core/tools/
--rw-rw-rw-   0        0        0        0 2022-11-28 17:09:18.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 07:38:05.493586 lupin-grognard-2.0.0.dev2/lupin_grognard/core/tools/ros2/
--rw-rw-rw-   0        0        0        0 2023-05-11 09:26:56.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/tools/ros2/__init__.py
--rw-rw-rw-   0        0        0     2654 2023-05-12 07:34:25.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/tools/ros2/interfaces.py
--rw-rw-rw-   0        0        0     2640 2023-05-11 14:11:15.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/tools/ros2/package.py
--rw-rw-rw-   0        0        0    35591 2023-05-11 09:26:56.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/tools/ros2/parser.py
--rw-rw-rw-   0        0        0     3867 2023-05-12 07:35:36.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/core/tools/utils.py
--rw-rw-rw-   0        0        0     6718 2023-05-12 07:35:36.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/run.py
-drwxrwxrwx   0        0        0        0 2023-05-12 07:38:05.496586 lupin-grognard-2.0.0.dev2/lupin_grognard/templates/
--rw-rw-rw-   0        0        0     1848 2023-05-04 13:34:03.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/templates/changelog.j2
--rw-rw-rw-   0        0        0     3390 2023-03-24 10:41:51.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/templates/reviewlog.j2
--rw-rw-rw-   0        0        0      454 2023-05-11 09:26:56.000000 lupin-grognard-2.0.0.dev2/lupin_grognard/templates/rosapi.j2
-drwxrwxrwx   0        0        0        0 2023-05-12 07:38:05.469326 lupin-grognard-2.0.0.dev2/lupin_grognard.egg-info/
--rw-rw-rw-   0        0        0      513 2023-05-12 07:38:05.000000 lupin-grognard-2.0.0.dev2/lupin_grognard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1468 2023-05-12 07:38:05.000000 lupin-grognard-2.0.0.dev2/lupin_grognard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 07:38:05.000000 lupin-grognard-2.0.0.dev2/lupin_grognard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-12 07:38:05.000000 lupin-grognard-2.0.0.dev2/lupin_grognard.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-11-23 21:32:45.000000 lupin-grognard-2.0.0.dev2/lupin_grognard.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      133 2023-05-12 07:38:05.000000 lupin-grognard-2.0.0.dev2/lupin_grognard.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-12 07:38:05.000000 lupin-grognard-2.0.0.dev2/lupin_grognard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      938 2023-05-12 07:38:05.499090 lupin-grognard-2.0.0.dev2/setup.cfg
--rw-rw-rw-   0        0        0      171 2022-11-28 17:09:18.000000 lupin-grognard-2.0.0.dev2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:15:20.361815 lupin-grognard-2.0.0.dev5/
+-rw-rw-rw-   0        0        0     1091 2022-10-26 14:21:00.000000 lupin-grognard-2.0.0.dev5/LICENCE
+-rw-rw-rw-   0        0        0       36 2023-03-02 22:35:36.000000 lupin-grognard-2.0.0.dev5/MANIFEST.in
+-rw-rw-rw-   0        0        0      513 2023-05-12 10:15:20.362815 lupin-grognard-2.0.0.dev5/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-01-20 08:07:36.000000 lupin-grognard-2.0.0.dev5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 10:15:20.303044 lupin-grognard-2.0.0.dev5/lupin_grognard/
+-rw-rw-rw-   0        0        0       28 2023-05-12 10:15:20.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/__init__.py
+-rw-rw-rw-   0        0        0       77 2023-05-11 09:26:56.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:15:20.340788 lupin-grognard-2.0.0.dev5/lupin_grognard/core/
+-rw-rw-rw-   0        0        0        0 2022-11-28 17:09:18.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/core/__init__.py
+-rw-rw-rw-   0        0        0     2227 2023-05-11 14:39:06.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/core/check.py
+-rw-rw-rw-   0        0        0      912 2022-12-09 16:33:58.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/core/cmd.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:15:20.345787 lupin-grognard-2.0.0.dev5/lupin_grognard/core/commit/
+-rw-rw-rw-   0        0        0        0 2023-01-17 13:04:34.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/core/commit/__init__.py
+-rw-rw-rw-   0        0        0     7379 2023-05-11 09:26:56.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/core/commit/commit.py
+-rw-rw-rw-   0        0        0     1274 2023-05-12 07:35:54.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/core/commit/commit_error.py
+-rw-rw-rw-   0        0        0     1816 2023-03-17 09:49:38.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/core/commit/commit_reporter.py
+-rw-rw-rw-   0        0        0     5739 2023-05-12 07:34:25.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/core/commit/commit_validator.py
+-rw-rw-rw-   0        0        0     1395 2023-05-12 07:34:47.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/core/config.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:15:20.351305 lupin-grognard-2.0.0.dev5/lupin_grognard/core/doc_generator/
+-rw-rw-rw-   0        0        0        0 2023-03-17 11:16:03.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/core/doc_generator/__init__.py
+-rw-rw-rw-   0        0        0    11923 2023-05-11 09:26:56.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/core/doc_generator/changelog.py
+-rw-rw-rw-   0        0        0     1706 2023-05-12 07:34:25.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/core/doc_generator/jinja_generator.py
+-rw-rw-rw-   0        0        0     5017 2023-05-11 09:26:56.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/core/doc_generator/reviewlog.py
+-rw-rw-rw-   0        0        0     1625 2023-05-11 09:26:56.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/core/doc_generator/ros2_docs.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:15:20.353299 lupin-grognard-2.0.0.dev5/lupin_grognard/core/format/
+-rw-rw-rw-   0        0        0        0 2023-02-10 13:59:49.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/core/format/__init__.py
+-rw-rw-rw-   0        0        0     2709 2023-05-12 07:34:25.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/core/format/clang_format.py
+-rw-rw-rw-   0        0        0     2598 2023-05-12 07:34:25.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/core/format/cmake_format.py
+-rw-rw-rw-   0        0        0     4040 2023-05-12 09:54:34.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/core/git.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:15:20.355301 lupin-grognard-2.0.0.dev5/lupin_grognard/core/tools/
+-rw-rw-rw-   0        0        0        0 2022-11-28 17:09:18.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/core/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:15:20.358302 lupin-grognard-2.0.0.dev5/lupin_grognard/core/tools/ros2/
+-rw-rw-rw-   0        0        0        0 2023-05-11 09:26:56.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/core/tools/ros2/__init__.py
+-rw-rw-rw-   0        0        0     2654 2023-05-12 07:34:25.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/core/tools/ros2/interfaces.py
+-rw-rw-rw-   0        0        0     2640 2023-05-11 14:11:15.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/core/tools/ros2/package.py
+-rw-rw-rw-   0        0        0    35591 2023-05-11 09:26:56.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/core/tools/ros2/parser.py
+-rw-rw-rw-   0        0        0     3867 2023-05-12 07:35:36.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/core/tools/utils.py
+-rw-rw-rw-   0        0        0     6781 2023-05-12 10:04:56.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/run.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:15:20.361815 lupin-grognard-2.0.0.dev5/lupin_grognard/templates/
+-rw-rw-rw-   0        0        0     1848 2023-05-04 13:34:03.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/templates/changelog.j2
+-rw-rw-rw-   0        0        0     3390 2023-03-24 10:41:51.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/templates/reviewlog.j2
+-rw-rw-rw-   0        0        0      454 2023-05-11 09:26:56.000000 lupin-grognard-2.0.0.dev5/lupin_grognard/templates/rosapi.j2
+drwxrwxrwx   0        0        0        0 2023-05-12 10:15:20.335273 lupin-grognard-2.0.0.dev5/lupin_grognard.egg-info/
+-rw-rw-rw-   0        0        0      513 2023-05-12 10:15:20.000000 lupin-grognard-2.0.0.dev5/lupin_grognard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1468 2023-05-12 10:15:20.000000 lupin-grognard-2.0.0.dev5/lupin_grognard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 10:15:20.000000 lupin-grognard-2.0.0.dev5/lupin_grognard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-12 10:15:20.000000 lupin-grognard-2.0.0.dev5/lupin_grognard.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-11-23 21:32:45.000000 lupin-grognard-2.0.0.dev5/lupin_grognard.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      133 2023-05-12 10:15:20.000000 lupin-grognard-2.0.0.dev5/lupin_grognard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-12 10:15:20.000000 lupin-grognard-2.0.0.dev5/lupin_grognard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      938 2023-05-12 10:15:20.363814 lupin-grognard-2.0.0.dev5/setup.cfg
+-rw-rw-rw-   0        0        0      171 2022-11-28 17:09:18.000000 lupin-grognard-2.0.0.dev5/setup.py
```

### Comparing `lupin-grognard-2.0.0.dev2/LICENCE` & `lupin-grognard-2.0.0.dev5/LICENCE`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev2/PKG-INFO` & `lupin-grognard-2.0.0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lupin-grognard
-Version: 2.0.0.dev2
+Version: 2.0.0.dev5
 Summary: Lupin linter tool
 License: MIT License
 Keywords: cli,linter
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lupin-grognard-2.0.0.dev2/lupin_grognard/core/check.py` & `lupin-grognard-2.0.0.dev5/lupin_grognard/core/check.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev2/lupin_grognard/core/cmd.py` & `lupin-grognard-2.0.0.dev5/lupin_grognard/core/cmd.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev2/lupin_grognard/core/commit/commit.py` & `lupin-grognard-2.0.0.dev5/lupin_grognard/core/commit/commit.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev2/lupin_grognard/core/commit/commit_error.py` & `lupin-grognard-2.0.0.dev5/lupin_grognard/core/commit/commit_error.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev2/lupin_grognard/core/commit/commit_reporter.py` & `lupin-grognard-2.0.0.dev5/lupin_grognard/core/commit/commit_reporter.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev2/lupin_grognard/core/commit/commit_validator.py` & `lupin-grognard-2.0.0.dev5/lupin_grognard/core/commit/commit_validator.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev2/lupin_grognard/core/config.py` & `lupin-grognard-2.0.0.dev5/lupin_grognard/core/config.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev2/lupin_grognard/core/doc_generator/changelog.py` & `lupin-grognard-2.0.0.dev5/lupin_grognard/core/doc_generator/changelog.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev2/lupin_grognard/core/doc_generator/jinja_generator.py` & `lupin-grognard-2.0.0.dev5/lupin_grognard/core/doc_generator/jinja_generator.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev2/lupin_grognard/core/doc_generator/reviewlog.py` & `lupin-grognard-2.0.0.dev5/lupin_grognard/core/doc_generator/reviewlog.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev2/lupin_grognard/core/doc_generator/ros2_docs.py` & `lupin-grognard-2.0.0.dev5/lupin_grognard/core/doc_generator/ros2_docs.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev2/lupin_grognard/core/format/clang_format.py` & `lupin-grognard-2.0.0.dev5/lupin_grognard/core/format/clang_format.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev2/lupin_grognard/core/format/cmake_format.py` & `lupin-grognard-2.0.0.dev5/lupin_grognard/core/format/cmake_format.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev2/lupin_grognard/core/git.py` & `lupin-grognard-2.0.0.dev5/lupin_grognard/core/git.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev2/lupin_grognard/core/tools/ros2/interfaces.py` & `lupin-grognard-2.0.0.dev5/lupin_grognard/core/tools/ros2/interfaces.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev2/lupin_grognard/core/tools/ros2/package.py` & `lupin-grognard-2.0.0.dev5/lupin_grognard/core/tools/ros2/package.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev2/lupin_grognard/core/tools/ros2/parser.py` & `lupin-grognard-2.0.0.dev5/lupin_grognard/core/tools/ros2/parser.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev2/lupin_grognard/core/tools/utils.py` & `lupin-grognard-2.0.0.dev5/lupin_grognard/core/tools/utils.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev2/lupin_grognard/run.py` & `lupin-grognard-2.0.0.dev5/lupin_grognard/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,25 +85,27 @@
     - With branches_name argument: grog check-commits "branch_1, branch_2..."
 
     You can set GROG_MAX_ALLOWED_COMMITS and GROG_DONT_CHECK_FOR_APPROVERS
     env var in .env, .gitlab-ci.yml, gitlab...
     """
     configure_logging()
     git = Git()
-    if all:  # --all option
+    current_branch_name = get_current_branch_name()
+
+    if all or is_main_branch(current_branch_name, MAIN_BRANCHES_LIST):  # --all option
         git_log = git.get_log()
         grog_max_allowed_commits = 0
     else:
         git_log = git.get_log(max_line_count=50, first_parent=True)
+
     if git_log.stderr:
         die(f"git error {git_log.return_code}, {git_log.stderr}")
 
     commit_list = generate_commit_list(data=git_log.stdout)
     display_supported_commit_types()
-    current_branch_name = get_current_branch_name()
     info(f"Current branch: {current_branch_name}")
 
     if all or is_main_branch(current_branch_name, MAIN_BRANCHES_LIST):  # --all option
         if is_main_branch(current_branch_name, MAIN_BRANCHES_LIST):
             info(
                 msg=f"Processing all commits since current branch '{current_branch_name}' is a main one"
             )
```

### Comparing `lupin-grognard-2.0.0.dev2/lupin_grognard/templates/changelog.j2` & `lupin-grognard-2.0.0.dev5/lupin_grognard/templates/changelog.j2`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev2/lupin_grognard/templates/reviewlog.j2` & `lupin-grognard-2.0.0.dev5/lupin_grognard/templates/reviewlog.j2`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev2/lupin_grognard.egg-info/PKG-INFO` & `lupin-grognard-2.0.0.dev5/lupin_grognard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lupin-grognard
-Version: 2.0.0.dev2
+Version: 2.0.0.dev5
 Summary: Lupin linter tool
 License: MIT License
 Keywords: cli,linter
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lupin-grognard-2.0.0.dev2/lupin_grognard.egg-info/SOURCES.txt` & `lupin-grognard-2.0.0.dev5/lupin_grognard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lupin-grognard-2.0.0.dev2/setup.cfg` & `lupin-grognard-2.0.0.dev5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 7570 696e 2d67 726f 676e 6172   = lupin-grognar
 00000020: 640d 0a76 6572 7369 6f6e 203d 2032 2e30  d..version = 2.0
-00000030: 2e30 2e64 6576 320d 0a64 6573 6372 6970  .0.dev2..descrip
+00000030: 2e30 2e64 6576 350d 0a64 6573 6372 6970  .0.dev5..descrip
 00000040: 7469 6f6e 203d 204c 7570 696e 206c 696e  tion = Lupin lin
 00000050: 7465 7220 746f 6f6c 0d0a 6c6f 6e67 5f64  ter tool..long_d
 00000060: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
 00000070: 653a 2052 4541 444d 452e 6d64 0d0a 6b65  e: README.md..ke
 00000080: 7977 6f72 6473 203d 2063 6c69 2c20 6c69  ywords = cli, li
 00000090: 6e74 6572 0d0a 6c69 6365 6e73 6520 3d20  nter..license = 
 000000a0: 4d49 5420 4c69 6365 6e73 650d 0a63 6c61  MIT License..cla
```


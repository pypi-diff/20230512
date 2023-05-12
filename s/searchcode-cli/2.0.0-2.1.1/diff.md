# Comparing `tmp/searchcode-cli-2.0.0.tar.gz` & `tmp/searchcode-cli-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchcode-cli-2.0.0.tar", last modified: Fri Apr 28 20:39:14 2023, max compression
+gzip compressed data, was "searchcode-cli-2.1.1.tar", last modified: Fri May 12 21:21:24 2023, max compression
```

## Comparing `searchcode-cli-2.0.0.tar` & `searchcode-cli-2.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:39:14.625085 searchcode-cli-2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:39:14.625085 searchcode-cli-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:39:14.625085 searchcode-cli-2.0.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-28 20:39:03.000000 searchcode-cli-2.0.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-28 20:39:03.000000 searchcode-cli-2.0.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 20:39:03.000000 searchcode-cli-2.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:39:14.625085 searchcode-cli-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-28 20:39:03.000000 searchcode-cli-2.0.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-28 20:39:03.000000 searchcode-cli-2.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-28 20:39:03.000000 searchcode-cli-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-04-28 20:39:03.000000 searchcode-cli-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42815 2023-04-28 20:39:14.625085 searchcode-cli-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-28 20:39:03.000000 searchcode-cli-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-28 20:39:03.000000 searchcode-cli-2.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:39:14.625085 searchcode-cli-2.0.0/searchcode/
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-04-28 20:39:03.000000 searchcode-cli-2.0.0/searchcode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-28 20:39:03.000000 searchcode-cli-2.0.0/searchcode/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    15984 2023-04-28 20:39:03.000000 searchcode-cli-2.0.0/searchcode/miscellaneous.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:39:14.625085 searchcode-cli-2.0.0/searchcode_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42815 2023-04-28 20:39:14.000000 searchcode-cli-2.0.0/searchcode_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-28 20:39:14.000000 searchcode-cli-2.0.0/searchcode_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 20:39:14.000000 searchcode-cli-2.0.0/searchcode_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 20:39:14.000000 searchcode-cli-2.0.0/searchcode_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 20:39:14.625085 searchcode-cli-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:21:23.998345 searchcode-cli-2.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:21:23.998345 searchcode-cli-2.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:21:23.998345 searchcode-cli-2.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-12 21:21:11.000000 searchcode-cli-2.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-12 21:21:11.000000 searchcode-cli-2.1.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-12 21:21:11.000000 searchcode-cli-2.1.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:21:23.998345 searchcode-cli-2.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-12 21:21:11.000000 searchcode-cli-2.1.1/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-12 21:21:11.000000 searchcode-cli-2.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-12 21:21:11.000000 searchcode-cli-2.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-05-12 21:21:11.000000 searchcode-cli-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42815 2023-05-12 21:21:23.998345 searchcode-cli-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-12 21:21:11.000000 searchcode-cli-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-12 21:21:11.000000 searchcode-cli-2.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:21:23.998345 searchcode-cli-2.1.1/searchcode/
+-rw-r--r--   0 runner    (1001) docker     (123)    19286 2023-05-12 21:21:11.000000 searchcode-cli-2.1.1/searchcode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-12 21:21:11.000000 searchcode-cli-2.1.1/searchcode/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15984 2023-05-12 21:21:11.000000 searchcode-cli-2.1.1/searchcode/miscellaneous.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:21:23.998345 searchcode-cli-2.1.1/searchcode_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42815 2023-05-12 21:21:23.000000 searchcode-cli-2.1.1/searchcode_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-12 21:21:23.000000 searchcode-cli-2.1.1/searchcode_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 21:21:23.000000 searchcode-cli-2.1.1/searchcode_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-12 21:21:23.000000 searchcode-cli-2.1.1/searchcode_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 21:21:23.998345 searchcode-cli-2.1.1/setup.cfg
```

### Comparing `searchcode-cli-2.0.0/.github/ISSUE_TEMPLATE/bug_report.md` & `searchcode-cli-2.1.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.0.0/.github/ISSUE_TEMPLATE/feature_request.md` & `searchcode-cli-2.1.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.0.0/.github/workflows/codeql.yml` & `searchcode-cli-2.1.1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.0.0/.github/workflows/python-publish.yml` & `searchcode-cli-2.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.0.0/.gitignore` & `searchcode-cli-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.0.0/LICENSE` & `searchcode-cli-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.0.0/PKG-INFO` & `searchcode-cli-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchcode-cli
-Version: 2.0.0
+Version: 2.1.1
 Summary: A Python wrapper around the searchcode API
 Author-email: Richard Mwewa <rly0nheart@duck.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `searchcode-cli-2.0.0/README.md` & `searchcode-cli-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.0.0/pyproject.toml` & `searchcode-cli-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "searchcode-cli"
-version = "2.0.0"
+version = "2.1.1"
 description = "A Python wrapper around the searchcode API"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = ["searchcode", "search-engine", "codesearch", "api-wrapper"]
 authors = [{name = "Richard Mwewa", email = "rly0nheart@duck.com"}]
 classifiers = [
```

### Comparing `searchcode-cli-2.0.0/searchcode/connection.py` & `searchcode-cli-2.1.1/searchcode/connection.py`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.0.0/searchcode/miscellaneous.py` & `searchcode-cli-2.1.1/searchcode/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.0.0/searchcode_cli.egg-info/PKG-INFO` & `searchcode-cli-2.1.1/searchcode_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchcode-cli
-Version: 2.0.0
+Version: 2.1.1
 Summary: A Python wrapper around the searchcode API
 Author-email: Richard Mwewa <rly0nheart@duck.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```


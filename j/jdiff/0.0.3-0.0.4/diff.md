# Comparing `tmp/jdiff-0.0.3.tar.gz` & `tmp/jdiff-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdiff-0.0.3.tar", max compression
+gzip compressed data, was "jdiff-0.0.4.tar", max compression
```

## Comparing `jdiff-0.0.3.tar` & `jdiff-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      471 2023-05-12 14:47:50.011106 jdiff-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0      533 2023-05-12 14:47:50.011106 jdiff-0.0.3/CONTRIBUTING.md
--rw-r--r--   0        0        0    10174 2023-05-12 14:47:50.011106 jdiff-0.0.3/LICENSE
--rw-r--r--   0        0        0     1910 2023-05-12 14:47:50.011106 jdiff-0.0.3/README.md
--rw-r--r--   0        0        0      165 2023-05-12 14:47:50.015106 jdiff-0.0.3/jdiff/__init__.py
--rw-r--r--   0        0        0    11759 2023-05-12 14:47:50.015106 jdiff-0.0.3/jdiff/check_types.py
--rw-r--r--   0        0        0     4439 2023-05-12 14:47:50.015106 jdiff-0.0.3/jdiff/evaluators.py
--rw-r--r--   0        0        0     4040 2023-05-12 14:47:50.015106 jdiff-0.0.3/jdiff/extract_data.py
--rw-r--r--   0        0        0     5066 2023-05-12 14:47:50.015106 jdiff-0.0.3/jdiff/operator.py
--rw-r--r--   0        0        0        0 2023-05-12 14:47:50.015106 jdiff-0.0.3/jdiff/utils/__init__.py
--rw-r--r--   0        0        0     2895 2023-05-12 14:47:50.015106 jdiff-0.0.3/jdiff/utils/data_normalization.py
--rw-r--r--   0        0        0     3678 2023-05-12 14:47:50.015106 jdiff-0.0.3/jdiff/utils/diff_helpers.py
--rw-r--r--   0        0        0     6775 2023-05-12 14:47:50.015106 jdiff-0.0.3/jdiff/utils/jmespath_parsers.py
--rw-r--r--   0        0        0     3196 2023-05-12 14:48:04.215322 jdiff-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 jdiff-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      510 2023-05-12 13:11:58.530808 jdiff-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0      533 2023-05-12 13:11:58.530808 jdiff-0.0.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0    10174 2023-05-12 13:11:58.530808 jdiff-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1910 2023-05-12 13:11:58.530808 jdiff-0.0.4/README.md
+-rw-r--r--   0        0        0      165 2023-05-12 13:11:58.534808 jdiff-0.0.4/jdiff/__init__.py
+-rw-r--r--   0        0        0    11759 2023-05-12 13:11:58.534808 jdiff-0.0.4/jdiff/check_types.py
+-rw-r--r--   0        0        0     4439 2023-05-12 13:11:58.534808 jdiff-0.0.4/jdiff/evaluators.py
+-rw-r--r--   0        0        0     4040 2023-05-12 13:11:58.534808 jdiff-0.0.4/jdiff/extract_data.py
+-rw-r--r--   0        0        0     5066 2023-05-12 13:11:58.534808 jdiff-0.0.4/jdiff/operator.py
+-rw-r--r--   0        0        0        0 2023-05-12 13:11:58.534808 jdiff-0.0.4/jdiff/utils/__init__.py
+-rw-r--r--   0        0        0     2895 2023-05-12 13:11:58.534808 jdiff-0.0.4/jdiff/utils/data_normalization.py
+-rw-r--r--   0        0        0     3678 2023-05-12 13:11:58.534808 jdiff-0.0.4/jdiff/utils/diff_helpers.py
+-rw-r--r--   0        0        0     6775 2023-05-12 13:11:58.534808 jdiff-0.0.4/jdiff/utils/jmespath_parsers.py
+-rw-r--r--   0        0        0     3202 2023-05-12 13:12:15.174885 jdiff-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3052 1970-01-01 00:00:00.000000 jdiff-0.0.4/PKG-INFO
```

### Comparing `jdiff-0.0.3/CONTRIBUTING.md` & `jdiff-0.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jdiff-0.0.3/LICENSE` & `jdiff-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jdiff-0.0.3/README.md` & `jdiff-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `jdiff-0.0.3/jdiff/check_types.py` & `jdiff-0.0.4/jdiff/check_types.py`

 * *Files identical despite different names*

### Comparing `jdiff-0.0.3/jdiff/evaluators.py` & `jdiff-0.0.4/jdiff/evaluators.py`

 * *Files identical despite different names*

### Comparing `jdiff-0.0.3/jdiff/extract_data.py` & `jdiff-0.0.4/jdiff/extract_data.py`

 * *Files identical despite different names*

### Comparing `jdiff-0.0.3/jdiff/operator.py` & `jdiff-0.0.4/jdiff/operator.py`

 * *Files identical despite different names*

### Comparing `jdiff-0.0.3/jdiff/utils/data_normalization.py` & `jdiff-0.0.4/jdiff/utils/data_normalization.py`

 * *Files identical despite different names*

### Comparing `jdiff-0.0.3/jdiff/utils/diff_helpers.py` & `jdiff-0.0.4/jdiff/utils/diff_helpers.py`

 * *Files identical despite different names*

### Comparing `jdiff-0.0.3/jdiff/utils/jmespath_parsers.py` & `jdiff-0.0.4/jdiff/utils/jmespath_parsers.py`

 * *Files identical despite different names*

### Comparing `jdiff-0.0.3/pyproject.toml` & `jdiff-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jdiff"
-version = "v0.0.3"
+version = "v0.0.4"
 description = "A light-weight library to compare structured output from network devices show commands."
 authors = ["Network to Code, LLC <info@networktocode.com>"]
 license = "Apache-2.0"
 homepage = "https://github.com/networktocode/jdiff"
 repository = "https://github.com/networktocode/jdiff"
 readme = "README.md"
 keywords = ["json", "diff", "network"]
@@ -19,15 +19,15 @@
     "CHANGELOG.md",
     "CONTRIBUTING.md",
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7.0"
-deepdiff = "^5.5.0"
+deepdiff = ">=5.5.0 <7.0"
 jmespath = "^0.10.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 requests_mock = "*"
 pyyaml = "*"
 black = "*"
```

### Comparing `jdiff-0.0.3/PKG-INFO` & `jdiff-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdiff
-Version: 0.0.3
+Version: 0.0.4
 Summary: A light-weight library to compare structured output from network devices show commands.
 Home-page: https://github.com/networktocode/jdiff
 License: Apache-2.0
 Keywords: json,diff,network
 Author: Network to Code, LLC
 Author-email: info@networktocode.com
 Requires-Python: >=3.7.0,<4.0.0
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: deepdiff (>=5.5.0,<6.0.0)
+Requires-Dist: deepdiff (>=5.5.0,<7.0)
 Requires-Dist: jmespath (>=0.10.0,<0.11.0)
 Project-URL: Repository, https://github.com/networktocode/jdiff
 Description-Content-Type: text/markdown
 
 # jdiff
 
 `jdiff` is a lightweight Python library allowing you to examine structured data. `jdiff` provides an interface to intelligently compare--via key presense/absense and value comparison--JSON data objects
```


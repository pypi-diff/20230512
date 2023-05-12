# Comparing `tmp/gen_pop_linkml2sheets-0.1.4.tar.gz` & `tmp/gen_pop_linkml2sheets-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_pop_linkml2sheets-0.1.4.tar", max compression
+gzip compressed data, was "gen_pop_linkml2sheets-0.1.6.tar", max compression
```

## Comparing `gen_pop_linkml2sheets-0.1.4.tar` & `gen_pop_linkml2sheets-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1075 2023-05-10 12:40:56.283705 gen_pop_linkml2sheets-0.1.4/LICENSE.md
--rw-r--r--   0        0        0     4403 2023-05-10 13:29:28.451789 gen_pop_linkml2sheets-0.1.4/README.md
--rw-r--r--   0        0        0     2365 2023-05-10 17:46:46.678845 gen_pop_linkml2sheets-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3748 2023-05-10 13:19:45.340546 gen_pop_linkml2sheets-0.1.4/src/gen_pop_linkml2sheets/generate_and_populate_template.py
--rw-r--r--   0        0        0     5125 1970-01-01 00:00:00.000000 gen_pop_linkml2sheets-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-10 12:40:56.283705 gen_pop_linkml2sheets-0.1.6/LICENSE.md
+-rw-r--r--   0        0        0     4403 2023-05-10 13:29:28.451789 gen_pop_linkml2sheets-0.1.6/README.md
+-rw-r--r--   0        0        0     2426 2023-05-12 17:28:17.006314 gen_pop_linkml2sheets-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      111 2023-05-10 17:53:28.805534 gen_pop_linkml2sheets-0.1.6/src/gen_pop_linkml2sheets/__init__.py
+-rw-r--r--   0        0        0     3748 2023-05-10 13:19:45.340546 gen_pop_linkml2sheets-0.1.6/src/gen_pop_linkml2sheets/generate_and_populate_template.py
+-rw-r--r--   0        0        0     5125 1970-01-01 00:00:00.000000 gen_pop_linkml2sheets-0.1.6/PKG-INFO
```

### Comparing `gen_pop_linkml2sheets-0.1.4/LICENSE.md` & `gen_pop_linkml2sheets-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gen_pop_linkml2sheets-0.1.4/README.md` & `gen_pop_linkml2sheets-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `gen_pop_linkml2sheets-0.1.4/pyproject.toml` & `gen_pop_linkml2sheets-0.1.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool.poetry]
 name = "gen-pop-linkml2sheets"
-version = "0.1.4"
+version = "0.1.6"
 description = ""
 authors = ["Mark Andrew Miller <MAM@lbl.gov>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/turbomam/gen-pop-linkml2sheets"
 repository = "https://github.com/turbomam/gen-pop-linkml2sheets"
+packages = [{ include = "gen_pop_linkml2sheets", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 linkml = "^1.5.2"
 pandas = "^1.3.4"
 schemasheets = "^0.1.21"
 
@@ -101,9 +102,9 @@
 
 [tool.black]
 line_length = 88
 include = '\.pyi?$'
 
 
 [tool.poetry.scripts]
-generate_and_populate_template = 'src.gen_pop_linkml2sheets.generate_and_populate_template:generate_and_populate_template'
+generate_and_populate_template = 'gen_pop_linkml2sheets.generate_and_populate_template:generate_and_populate_template'
```

### Comparing `gen_pop_linkml2sheets-0.1.4/src/gen_pop_linkml2sheets/generate_and_populate_template.py` & `gen_pop_linkml2sheets-0.1.6/src/gen_pop_linkml2sheets/generate_and_populate_template.py`

 * *Files identical despite different names*

### Comparing `gen_pop_linkml2sheets-0.1.4/PKG-INFO` & `gen_pop_linkml2sheets-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-pop-linkml2sheets
-Version: 0.1.4
+Version: 0.1.6
 Summary: 
 Home-page: https://github.com/turbomam/gen-pop-linkml2sheets
 License: MIT
 Author: Mark Andrew Miller
 Author-email: MAM@lbl.gov
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gen-pop-linkml2sheets Version: 0.1.4 Summary: Home-
+Metadata-Version: 2.1 Name: gen-pop-linkml2sheets Version: 0.1.6 Summary: Home-
 page: https://github.com/turbomam/gen-pop-linkml2sheets License: MIT Author:
 Mark Andrew Miller Author-email: MAM@lbl.gov Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: linkml (>=1.5.2,<2.0.0) Requires-
 Dist: pandas (>=1.3.4,<2.0.0) Requires-Dist: schemasheets (>=0.1.21,<0.2.0)
```


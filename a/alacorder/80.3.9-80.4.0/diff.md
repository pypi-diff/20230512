# Comparing `tmp/alacorder-80.3.9.tar.gz` & `tmp/alacorder-80.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.3.9.tar", max compression
+gzip compressed data, was "alacorder-80.4.0.tar", max compression
```

## Comparing `alacorder-80.3.9.tar` & `alacorder-80.4.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.3.9/LICENSE
--rw-r--r--   0        0        0     6592 2023-05-11 17:12:36.043202 alacorder-80.3.9/README.md
--rw-r--r--   0        0        0      697 2023-05-11 17:09:43.251588 alacorder-80.3.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.3.9/src/alacorder/__init__.py
--rw-r--r--   0        0        0   210936 2023-05-11 17:09:24.486510 alacorder-80.3.9/src/alacorder/__main__.py
--rw-r--r--   0        0        0   210936 2023-05-11 17:09:29.605342 alacorder-80.3.9/src/alacorder/alac.py
--rw-r--r--   0        0        0     7521 1970-01-01 00:00:00.000000 alacorder-80.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.4.0/LICENSE
+-rw-r--r--   0        0        0     6592 2023-05-11 17:12:36.043202 alacorder-80.4.0/README.md
+-rw-r--r--   0        0        0      697 2023-05-11 20:27:55.075565 alacorder-80.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-11 17:08:42.977651 alacorder-80.4.0/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.4.0/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   211136 2023-05-11 20:29:07.180937 alacorder-80.4.0/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   211136 2023-05-11 20:29:02.874296 alacorder-80.4.0/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7521 1970-01-01 00:00:00.000000 alacorder-80.4.0/PKG-INFO
```

### Comparing `alacorder-80.3.9/LICENSE` & `alacorder-80.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.3.9/README.md` & `alacorder-80.4.0/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.3.9/pyproject.toml` & `alacorder-80.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.3.9"
+version = "80.4.0"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.3.9/src/alacorder/__main__.py` & `alacorder-80.4.0/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.3.9"
+version = "80.4.0"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -3069,16 +3069,17 @@
                 "Remove TEMP columns from input query spreadsheet and try again."
             )
 
     if qskip > 0:
         qs = qskip - 1
         query = query[qs:-1]
 
-    if qmax > query.shape[1]:
-        query = query[0:qmax]
+    if qmax < query.shape[0] and qmax > 0:
+        found = query.shape[0]
+        query = query.sample(qmax)
 
     pscols = [
         "NAME",
         "PARTY_TYPE",
         "SSN",
         "DOB",
         "COUNTY",
@@ -3122,16 +3123,19 @@
 
     query = query.with_columns(
         [
             pl.col("RETRIEVED").cast(pl.Utf8, strict=False),
         ]
     )
 
-    if goodquery:
-        print(f"{query.shape[0]} queries found in input query file.")
+    if goodquery and qmax == 0:
+        print(f"{query.shape[0]} queries read from input query file.")
+        return query
+    elif goodquery and qmax > 0:
+        print(f"{query.shape[0]} of {found} queries read from input query file.")
         return query
     else:
         print(
             "Try again with at least one valid column header: [NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, NO_RECORDS, FILED_BEFORE, FILED_AFTER, RETRIEVED, CASES_FOUND, QUERY_COMPLETE]"
         )
         return None
```

### Comparing `alacorder-80.3.9/src/alacorder/alac.py` & `alacorder-80.4.0/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.3.9"
+version = "80.4.0"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -3069,16 +3069,17 @@
                 "Remove TEMP columns from input query spreadsheet and try again."
             )
 
     if qskip > 0:
         qs = qskip - 1
         query = query[qs:-1]
 
-    if qmax > query.shape[1]:
-        query = query[0:qmax]
+    if qmax < query.shape[0] and qmax > 0:
+        found = query.shape[0]
+        query = query.sample(qmax)
 
     pscols = [
         "NAME",
         "PARTY_TYPE",
         "SSN",
         "DOB",
         "COUNTY",
@@ -3122,16 +3123,19 @@
 
     query = query.with_columns(
         [
             pl.col("RETRIEVED").cast(pl.Utf8, strict=False),
         ]
     )
 
-    if goodquery:
-        print(f"{query.shape[0]} queries found in input query file.")
+    if goodquery and qmax == 0:
+        print(f"{query.shape[0]} queries read from input query file.")
+        return query
+    elif goodquery and qmax > 0:
+        print(f"{query.shape[0]} of {found} queries read from input query file.")
         return query
     else:
         print(
             "Try again with at least one valid column header: [NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, NO_RECORDS, FILED_BEFORE, FILED_AFTER, RETRIEVED, CASES_FOUND, QUERY_COMPLETE]"
         )
         return None
```

### Comparing `alacorder-80.3.9/PKG-INFO` & `alacorder-80.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.3.9
+Version: 80.4.0
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


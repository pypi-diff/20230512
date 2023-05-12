# Comparing `tmp/alacorder-80.4.1.tar.gz` & `tmp/alacorder-80.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.4.1.tar", max compression
+gzip compressed data, was "alacorder-80.4.2.tar", max compression
```

## Comparing `alacorder-80.4.1.tar` & `alacorder-80.4.2.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.4.1/LICENSE
--rw-r--r--   0        0        0     6592 2023-05-11 17:12:36.043202 alacorder-80.4.1/README.md
--rw-r--r--   0        0        0      697 2023-05-12 14:33:27.500039 alacorder-80.4.1/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-12 14:38:33.606941 alacorder-80.4.1/src/alacorder/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.4.1/src/alacorder/__init__.py
--rw-r--r--   0        0        0   211506 2023-05-12 14:33:09.701142 alacorder-80.4.1/src/alacorder/__main__.py
--rw-r--r--   0        0        0   211506 2023-05-12 14:32:46.715588 alacorder-80.4.1/src/alacorder/alac.py
--rw-r--r--   0        0        0     7521 1970-01-01 00:00:00.000000 alacorder-80.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.4.2/LICENSE
+-rw-r--r--   0        0        0     6592 2023-05-11 17:12:36.043202 alacorder-80.4.2/README.md
+-rw-r--r--   0        0        0      697 2023-05-12 14:49:25.784134 alacorder-80.4.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.4.2/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   211533 2023-05-12 14:49:05.669441 alacorder-80.4.2/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   211533 2023-05-12 14:49:09.510217 alacorder-80.4.2/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7521 1970-01-01 00:00:00.000000 alacorder-80.4.2/PKG-INFO
```

### Comparing `alacorder-80.4.1/LICENSE` & `alacorder-80.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.4.1/README.md` & `alacorder-80.4.2/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.4.1/pyproject.toml` & `alacorder-80.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.4.1"
+version = "80.4.2"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.4.1/src/alacorder/__main__.py` & `alacorder-80.4.2/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """
 ALACORDER --------------------
 ╔═╗╔╗╔╔═╗╦ ╦╔═╗╔═╗╦  ╔═╗╔═╗╔═╗
 ╚═╗║║║║ ║║║║╠═╝╠═╣║  ╠═╣║  ║╣ 
 ╚═╝╝╚╝╚═╝╚╩╝╩  ╩ ╩╩═╝╩ ╩╚═╝╚═╝
 (c) 2023 Sam Robson ----------
 
-Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
-
+Dependencies: 
+    python 3.9+, brotli ^1.0.9, click ^8.1.3,
+    polars ^0.17.6, PyMuPDF ^1.21.1, 
+    PySimpleGUI ^4.60.4, selenium ^4.8.3, 
+    tqdm ^4.65.0, xlsx2csv ^0.8.1, XlsxWriter ^3.0.9
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.4.1"
+version = "80.4.2"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
```

### Comparing `alacorder-80.4.1/src/alacorder/alac.py` & `alacorder-80.4.2/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """
 ALACORDER --------------------
 ╔═╗╔╗╔╔═╗╦ ╦╔═╗╔═╗╦  ╔═╗╔═╗╔═╗
 ╚═╗║║║║ ║║║║╠═╝╠═╣║  ╠═╣║  ║╣ 
 ╚═╝╝╚╝╚═╝╚╩╝╩  ╩ ╩╩═╝╩ ╩╚═╝╚═╝
 (c) 2023 Sam Robson ----------
 
-Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
-
+Dependencies: 
+    python 3.9+, brotli ^1.0.9, click ^8.1.3,
+    polars ^0.17.6, PyMuPDF ^1.21.1, 
+    PySimpleGUI ^4.60.4, selenium ^4.8.3, 
+    tqdm ^4.65.0, xlsx2csv ^0.8.1, XlsxWriter ^3.0.9
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.4.1"
+version = "80.4.2"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
```

### Comparing `alacorder-80.4.1/PKG-INFO` & `alacorder-80.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.4.1
+Version: 80.4.2
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


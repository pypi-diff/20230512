# Comparing `tmp/checksec_py-0.7.tar.gz` & `tmp/checksec_py-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checksec_py-0.7.tar", max compression
+gzip compressed data, was "checksec_py-0.7.1.tar", max compression
```

## Comparing `checksec_py-0.7.tar` & `checksec_py-0.7.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2020-04-26 12:10:04.349250 checksec_py-0.7/LICENSE
--rw-r--r--   0        0        0     8657 2022-10-02 20:01:10.750264 checksec_py-0.7/README.md
--rw-r--r--   0        0        0        0 2020-04-28 02:20:35.173787 checksec_py-0.7/checksec/__init__.py
--rw-r--r--   0        0        0     5901 2021-01-28 10:03:12.235800 checksec_py-0.7/checksec/__main__.py
--rw-r--r--   0        0        0      616 2021-01-26 09:37:03.708549 checksec_py-0.7/checksec/binary.py
--rw-r--r--   0        0        0     7384 2023-05-12 06:07:12.914764 checksec_py-0.7/checksec/elf.py
--rw-r--r--   0        0        0      218 2020-09-30 08:53:12.335957 checksec_py-0.7/checksec/errors.py
--rw-r--r--   0        0        0    13391 2021-09-08 07:58:59.369750 checksec_py-0.7/checksec/output.py
--rw-r--r--   0        0        0     4397 2023-05-12 06:07:12.914764 checksec_py-0.7/checksec/pe.py
--rw-r--r--   0        0        0     4809 2022-10-02 20:01:10.750264 checksec_py-0.7/checksec/utils.py
--rw-r--r--   0        0        0     1381 2023-05-12 06:13:28.527654 checksec_py-0.7/pyproject.toml
--rw-r--r--   0        0        0     9525 1970-01-01 00:00:00.000000 checksec_py-0.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-12 07:14:30.795878 checksec_py-0.7.1/LICENSE
+-rw-r--r--   0        0        0     8657 2023-05-12 07:14:30.795878 checksec_py-0.7.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-12 07:14:30.795878 checksec_py-0.7.1/checksec/__init__.py
+-rw-r--r--   0        0        0     5901 2023-05-12 07:14:30.795878 checksec_py-0.7.1/checksec/__main__.py
+-rw-r--r--   0        0        0      616 2023-05-12 07:14:30.795878 checksec_py-0.7.1/checksec/binary.py
+-rw-r--r--   0        0        0     7384 2023-05-12 07:14:30.795878 checksec_py-0.7.1/checksec/elf.py
+-rw-r--r--   0        0        0      218 2023-05-12 07:14:30.795878 checksec_py-0.7.1/checksec/errors.py
+-rw-r--r--   0        0        0    13391 2023-05-12 07:14:30.795878 checksec_py-0.7.1/checksec/output.py
+-rw-r--r--   0        0        0     4397 2023-05-12 07:14:30.795878 checksec_py-0.7.1/checksec/pe.py
+-rw-r--r--   0        0        0     4809 2023-05-12 07:14:30.795878 checksec_py-0.7.1/checksec/utils.py
+-rw-r--r--   0        0        0     1383 2023-05-12 07:14:30.795878 checksec_py-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     9527 1970-01-01 00:00:00.000000 checksec_py-0.7.1/PKG-INFO
```

### Comparing `checksec_py-0.7/LICENSE` & `checksec_py-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `checksec_py-0.7/README.md` & `checksec_py-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `checksec_py-0.7/checksec/__main__.py` & `checksec_py-0.7.1/checksec/__main__.py`

 * *Files identical despite different names*

### Comparing `checksec_py-0.7/checksec/binary.py` & `checksec_py-0.7.1/checksec/binary.py`

 * *Files identical despite different names*

### Comparing `checksec_py-0.7/checksec/elf.py` & `checksec_py-0.7.1/checksec/elf.py`

 * *Files identical despite different names*

### Comparing `checksec_py-0.7/checksec/output.py` & `checksec_py-0.7.1/checksec/output.py`

 * *Files identical despite different names*

### Comparing `checksec_py-0.7/checksec/pe.py` & `checksec_py-0.7.1/checksec/pe.py`

 * *Files identical despite different names*

### Comparing `checksec_py-0.7/checksec/utils.py` & `checksec_py-0.7.1/checksec/utils.py`

 * *Files identical despite different names*

### Comparing `checksec_py-0.7/pyproject.toml` & `checksec_py-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "checksec-py"
-version = "0.7"
+version = "0.7.1"
 description = "Checksec tool implemented in Python"
 authors = ["Mathieu Tarral <mathieu.tarral@protonmail.com>"]
 readme = "README.md"
 packages = [{include = "checksec"}]
 license = "GPL-3.0-only"
 repository = "https://github.com/Wenzel/checksec.py"
 keywords = ["checksec", "security", "ELF", "PE", "binary"]
```

### Comparing `checksec_py-0.7/PKG-INFO` & `checksec_py-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checksec-py
-Version: 0.7
+Version: 0.7.1
 Summary: Checksec tool implemented in Python
 Home-page: https://github.com/Wenzel/checksec.py
 License: GPL-3.0-only
 Keywords: checksec,security,ELF,PE,binary
 Author: Mathieu Tarral
 Author-email: mathieu.tarral@protonmail.com
 Requires-Python: >=3.8,<3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: checksec-py Version: 0.7 Summary: Checksec tool
+Metadata-Version: 2.1 Name: checksec-py Version: 0.7.1 Summary: Checksec tool
 implemented in Python Home-page: https://github.com/Wenzel/checksec.py License:
 GPL-3.0-only Keywords: checksec,security,ELF,PE,binary Author: Mathieu Tarral
 Author-email: mathieu.tarral@protonmail.com Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```


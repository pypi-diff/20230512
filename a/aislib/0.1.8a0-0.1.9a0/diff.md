# Comparing `tmp/aislib-0.1.8a0.tar.gz` & `tmp/aislib-0.1.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aislib-0.1.8a0.tar", max compression
+gzip compressed data, was "aislib-0.1.9a0.tar", max compression
```

## Comparing `aislib-0.1.8a0.tar` & `aislib-0.1.9a0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0    34523 2021-06-10 11:26:50.885977 aislib-0.1.8a0/LICENSE
--rw-r--r--   0        0        0      145 2021-06-09 15:11:33.835999 aislib-0.1.8a0/aislib/__init__.py
--rw-r--r--   0        0        0     4787 2021-06-09 15:11:33.836198 aislib-0.1.8a0/aislib/data_load.py
--rw-r--r--   0        0        0     1694 2021-06-09 15:11:33.836367 aislib-0.1.8a0/aislib/misc_utils.py
--rw-r--r--   0        0        0     4075 2021-06-09 15:11:33.836565 aislib-0.1.8a0/aislib/plink_utils.py
--rw-r--r--   0        0        0     7698 2021-06-09 15:11:33.836749 aislib-0.1.8a0/aislib/pytorch_modules.py
--rw-r--r--   0        0        0     3004 2021-06-09 15:11:33.836939 aislib-0.1.8a0/aislib/pytorch_utils.py
--rw-r--r--   0        0        0      678 2022-09-07 11:41:23.668117 aislib-0.1.8a0/pyproject.toml
--rw-r--r--   0        0        0      779 2022-09-07 11:44:27.769303 aislib-0.1.8a0/setup.py
--rw-r--r--   0        0        0      702 2022-09-07 11:44:27.769567 aislib-0.1.8a0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2021-06-10 11:26:50.885977 aislib-0.1.9a0/LICENSE
+-rw-r--r--   0        0        0      145 2021-06-09 15:11:33.835999 aislib-0.1.9a0/aislib/__init__.py
+-rw-r--r--   0        0        0     4787 2021-06-09 15:11:33.836198 aislib-0.1.9a0/aislib/data_load.py
+-rw-r--r--   0        0        0     1694 2021-06-09 15:11:33.836367 aislib-0.1.9a0/aislib/misc_utils.py
+-rw-r--r--   0        0        0     4075 2021-06-09 15:11:33.836565 aislib-0.1.9a0/aislib/plink_utils.py
+-rw-r--r--   0        0        0     7698 2021-06-09 15:11:33.836749 aislib-0.1.9a0/aislib/pytorch_modules.py
+-rw-r--r--   0        0        0     3004 2021-06-09 15:11:33.836939 aislib-0.1.9a0/aislib/pytorch_utils.py
+-rw-r--r--   0        0        0      682 2023-03-16 08:15:26.812801 aislib-0.1.9a0/pyproject.toml
+-rw-r--r--   0        0        0      761 1970-01-01 00:00:00.000000 aislib-0.1.9a0/PKG-INFO
```

### Comparing `aislib-0.1.8a0/LICENSE` & `aislib-0.1.9a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aislib-0.1.8a0/aislib/data_load.py` & `aislib-0.1.9a0/aislib/data_load.py`

 * *Files identical despite different names*

### Comparing `aislib-0.1.8a0/aislib/misc_utils.py` & `aislib-0.1.9a0/aislib/misc_utils.py`

 * *Files identical despite different names*

### Comparing `aislib-0.1.8a0/aislib/plink_utils.py` & `aislib-0.1.9a0/aislib/plink_utils.py`

 * *Files identical despite different names*

### Comparing `aislib-0.1.8a0/aislib/pytorch_modules.py` & `aislib-0.1.9a0/aislib/pytorch_modules.py`

 * *Files identical despite different names*

### Comparing `aislib-0.1.8a0/aislib/pytorch_utils.py` & `aislib-0.1.9a0/aislib/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `aislib-0.1.8a0/pyproject.toml` & `aislib-0.1.9a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "aislib"
-version = "0.1.8-alpha"
+version = "0.1.9-alpha"
 description = ""
 authors = ["Arnor Sigurdsson"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pandas = "^1.2"
 numpy = "^1.2"
-torch = "^1"
+torch = "^2.0.0"
 torchvision = "^0"
 py = "^1.10.0"
 matplotlib = "^3.3"
 scikit-learn = "^1"
 seaborn = "^0"
 sympy = "^1"
 tqdm = "^4.55"
```

### Comparing `aislib-0.1.8a0/PKG-INFO` & `aislib-0.1.9a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: aislib
-Version: 0.1.8a0
+Version: 0.1.9a0
 Summary: 
 Author: Arnor Sigurdsson
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3.3,<4.0)
 Requires-Dist: numpy (>=1.2,<2.0)
 Requires-Dist: pandas (>=1.2,<2.0)
 Requires-Dist: pandas-plink (>=2.2.4,<3.0.0)
 Requires-Dist: py (>=1.10.0,<2.0.0)
 Requires-Dist: scikit-learn (>=1,<2)
 Requires-Dist: seaborn (>=0,<1)
 Requires-Dist: sympy (>=1,<2)
-Requires-Dist: torch (>=1,<2)
+Requires-Dist: torch (>=2.0.0,<3.0.0)
 Requires-Dist: torchvision (>=0,<1)
 Requires-Dist: tqdm (>=4.55,<5.0)
```


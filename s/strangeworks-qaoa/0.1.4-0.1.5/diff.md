# Comparing `tmp/strangeworks_qaoa-0.1.4.tar.gz` & `tmp/strangeworks_qaoa-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_qaoa-0.1.4.tar", max compression
+gzip compressed data, was "strangeworks_qaoa-0.1.5.tar", max compression
```

## Comparing `strangeworks_qaoa-0.1.4.tar` & `strangeworks_qaoa-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-05-03 11:03:36.401419 strangeworks_qaoa-0.1.4/LICENSE
--rw-r--r--   0        0        0      576 2023-05-03 11:03:36.401419 strangeworks_qaoa-0.1.4/README.md
--rw-r--r--   0        0        0      791 2023-05-03 11:03:54.857458 strangeworks_qaoa-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      128 2023-05-03 11:03:36.405420 strangeworks_qaoa-0.1.4/strangeworks_qaoa/__init__.py
--rw-r--r--   0        0        0    16028 2023-05-03 11:03:36.405420 strangeworks_qaoa-0.1.4/strangeworks_qaoa/sdk.py
--rw-r--r--   0        0        0      691 2023-05-03 11:03:36.405420 strangeworks_qaoa-0.1.4/strangeworks_qaoa/serializer.py
--rw-r--r--   0        0        0    12428 2023-05-03 11:03:36.405420 strangeworks_qaoa-0.1.4/strangeworks_qaoa/utils.py
--rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 strangeworks_qaoa-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-12 14:41:14.374113 strangeworks_qaoa-0.1.5/LICENSE
+-rw-r--r--   0        0        0      679 2023-05-12 14:41:14.374113 strangeworks_qaoa-0.1.5/README.md
+-rw-r--r--   0        0        0      791 2023-05-12 14:41:26.858220 strangeworks_qaoa-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      128 2023-05-12 14:41:14.378113 strangeworks_qaoa-0.1.5/strangeworks_qaoa/__init__.py
+-rw-r--r--   0        0        0    16215 2023-05-12 14:41:14.378113 strangeworks_qaoa-0.1.5/strangeworks_qaoa/sdk.py
+-rw-r--r--   0        0        0      691 2023-05-12 14:41:14.378113 strangeworks_qaoa-0.1.5/strangeworks_qaoa/serializer.py
+-rw-r--r--   0        0        0    12428 2023-05-12 14:41:14.378113 strangeworks_qaoa-0.1.5/strangeworks_qaoa/utils.py
+-rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 strangeworks_qaoa-0.1.5/PKG-INFO
```

### Comparing `strangeworks_qaoa-0.1.4/LICENSE` & `strangeworks_qaoa-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.4/README.md` & `strangeworks_qaoa-0.1.5/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+![Tests](https://github.com/strangeworks/strangeworks-qaoa/actions/workflows/cron_test.yml/badge.svg)
+
 # Strangeworks QAOA SDK Extension
 
 This extension provides access to the Strangeworks QAOA service through the SDK.
 
 ## Installation
 
 Install using `poetry`
```

### Comparing `strangeworks_qaoa-0.1.4/pyproject.toml` & `strangeworks_qaoa-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strangeworks-qaoa"
-version = "0.1.4"
+version = "0.1.5"
 description = "Extension to strangeworks sdk to allow user to run qaoa service"
 authors = ["SFlann <stuart@strangeworks.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_qaoa"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `strangeworks_qaoa-0.1.4/strangeworks_qaoa/sdk.py` & `strangeworks_qaoa-0.1.5/strangeworks_qaoa/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,14 +244,19 @@
 
         problem_params["H"] = json.dumps(H)
         problem_params["ising"] = (
             json.dumps(problem_params["ising"])
             if problem_params.get("ising")
             else json.dumps(False)
         )
+        problem_params["warm_start"] = (
+            json.dumps(problem_params["warm_start"])
+            if problem_params.get("warm_start")
+            else json.dumps(False)
+        )
 
         if aws is True:
             input_params = {
                 "provider": "aws",
                 "backend": backend_id,
                 "hyperparams": json.dumps(problem_params),
             }
```

### Comparing `strangeworks_qaoa-0.1.4/strangeworks_qaoa/serializer.py` & `strangeworks_qaoa-0.1.5/strangeworks_qaoa/serializer.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.4/strangeworks_qaoa/utils.py` & `strangeworks_qaoa-0.1.5/strangeworks_qaoa/utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.4/PKG-INFO` & `strangeworks_qaoa-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks-qaoa
-Version: 0.1.4
+Version: 0.1.5
 Summary: Extension to strangeworks sdk to allow user to run qaoa service
 Author: SFlann
 Author-email: stuart@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -12,14 +12,16 @@
 Requires-Dist: dimod (>=0.12.4,<0.13.0)
 Requires-Dist: networkx (>=3.0,<4.0)
 Requires-Dist: numpy (==1.23.2)
 Requires-Dist: qiskit (>=0.41.0,<0.42.0)
 Requires-Dist: strangeworks (>=0.4.0,<0.5.0)
 Description-Content-Type: text/markdown
 
+![Tests](https://github.com/strangeworks/strangeworks-qaoa/actions/workflows/cron_test.yml/badge.svg)
+
 # Strangeworks QAOA SDK Extension
 
 This extension provides access to the Strangeworks QAOA service through the SDK.
 
 ## Installation
 
 Install using `poetry`
```


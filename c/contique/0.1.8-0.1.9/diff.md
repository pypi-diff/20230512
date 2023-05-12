# Comparing `tmp/contique-0.1.8.tar.gz` & `tmp/contique-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contique-0.1.8.tar", last modified: Fri Mar  5 09:31:30 2021, max compression
+gzip compressed data, was "contique-0.1.9.tar", last modified: Fri Mar  5 15:25:52 2021, max compression
```

## Comparing `contique-0.1.8.tar` & `contique-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-05 09:31:30.407143 contique-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (116)    35149 2021-03-05 09:31:21.000000 contique-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       33 2021-03-05 09:31:21.000000 contique-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     8272 2021-03-05 09:31:30.407143 contique-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6238 2021-03-05 09:31:21.000000 contique-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-05 09:31:30.407143 contique-0.1.8/contique/
--rw-r--r--   0 runner    (1001) docker     (116)       22 2021-03-05 09:31:21.000000 contique-0.1.8/contique/__about__.py
--rw-r--r--   0 runner    (1001) docker     (116)      138 2021-03-05 09:31:21.000000 contique-0.1.8/contique/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2859 2021-03-05 09:31:21.000000 contique-0.1.8/contique/helpers.py
--rw-r--r--   0 runner    (1001) docker     (116)     3292 2021-03-05 09:31:21.000000 contique-0.1.8/contique/jacobian.py
--rw-r--r--   0 runner    (1001) docker     (116)     4350 2021-03-05 09:31:21.000000 contique-0.1.8/contique/newton.py
--rw-r--r--   0 runner    (1001) docker     (116)     5228 2021-03-05 09:31:21.000000 contique-0.1.8/contique/newtonxt.py
--rw-r--r--   0 runner    (1001) docker     (116)     1779 2021-03-05 09:31:21.000000 contique-0.1.8/contique/printinfo.py
--rw-r--r--   0 runner    (1001) docker     (116)     7247 2021-03-05 09:31:21.000000 contique-0.1.8/contique/solve.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-05 09:31:30.407143 contique-0.1.8/contique.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     8272 2021-03-05 09:31:30.000000 contique-0.1.8/contique.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      507 2021-03-05 09:31:30.000000 contique-0.1.8/contique.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-05 09:31:30.000000 contique-0.1.8/contique.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2021-03-05 09:31:30.000000 contique-0.1.8/contique.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2021-03-05 09:31:30.000000 contique-0.1.8/contique.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       93 2021-03-05 09:31:21.000000 contique-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)     1076 2021-03-05 09:31:30.407143 contique-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-05 09:31:30.407143 contique-0.1.8/test/
--rw-r--r--   0 runner    (1001) docker     (116)     1140 2021-03-05 09:31:21.000000 contique-0.1.8/test/test_archimedean_spiral.py
--rw-r--r--   0 runner    (1001) docker     (116)     1197 2021-03-05 09:31:21.000000 contique-0.1.8/test/test_lituus_spiral.py
--rw-r--r--   0 runner    (1001) docker     (116)     1215 2021-03-05 09:31:21.000000 contique-0.1.8/test/test_log_spiral.py
--rw-r--r--   0 runner    (1001) docker     (116)     1161 2021-03-05 09:31:21.000000 contique-0.1.8/test/test_sin_rebalance.py
--rw-r--r--   0 runner    (1001) docker     (116)     1085 2021-03-05 09:31:21.000000 contique-0.1.8/test/test_sincos.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-05 15:25:52.408573 contique-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (116)    35149 2021-03-05 15:25:43.000000 contique-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)       33 2021-03-05 15:25:43.000000 contique-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     8272 2021-03-05 15:25:52.408573 contique-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     6238 2021-03-05 15:25:43.000000 contique-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-05 15:25:52.408573 contique-0.1.9/contique/
+-rw-r--r--   0 runner    (1001) docker     (116)       22 2021-03-05 15:25:43.000000 contique-0.1.9/contique/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      138 2021-03-05 15:25:43.000000 contique-0.1.9/contique/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2859 2021-03-05 15:25:43.000000 contique-0.1.9/contique/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3292 2021-03-05 15:25:43.000000 contique-0.1.9/contique/jacobian.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4350 2021-03-05 15:25:43.000000 contique-0.1.9/contique/newton.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5228 2021-03-05 15:25:43.000000 contique-0.1.9/contique/newtonxt.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1779 2021-03-05 15:25:43.000000 contique-0.1.9/contique/printinfo.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7246 2021-03-05 15:25:43.000000 contique-0.1.9/contique/solve.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-05 15:25:52.408573 contique-0.1.9/contique.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     8272 2021-03-05 15:25:52.000000 contique-0.1.9/contique.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      507 2021-03-05 15:25:52.000000 contique-0.1.9/contique.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-05 15:25:52.000000 contique-0.1.9/contique.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        6 2021-03-05 15:25:52.000000 contique-0.1.9/contique.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        9 2021-03-05 15:25:52.000000 contique-0.1.9/contique.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       93 2021-03-05 15:25:43.000000 contique-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)     1076 2021-03-05 15:25:52.408573 contique-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-05 15:25:52.408573 contique-0.1.9/test/
+-rw-r--r--   0 runner    (1001) docker     (116)     1140 2021-03-05 15:25:43.000000 contique-0.1.9/test/test_archimedean_spiral.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1197 2021-03-05 15:25:43.000000 contique-0.1.9/test/test_lituus_spiral.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1215 2021-03-05 15:25:43.000000 contique-0.1.9/test/test_log_spiral.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1161 2021-03-05 15:25:43.000000 contique-0.1.9/test/test_sin_rebalance.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1085 2021-03-05 15:25:43.000000 contique-0.1.9/test/test_sincos.py
```

### Comparing `contique-0.1.8/LICENSE` & `contique-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `contique-0.1.8/PKG-INFO` & `contique-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contique
-Version: 0.1.8
+Version: 0.1.9
 Summary: Numerical continuation of nonlinear equilibrium equations
 Home-page: https://github.com/adtzlr/contique
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License: GPL-3.0-or-later
 Project-URL: Code, https://github.com/adtzlr/contique
 Project-URL: Issues, https://github.com/adtzlr/contique/issues
```

### Comparing `contique-0.1.8/README.md` & `contique-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `contique-0.1.8/contique/helpers.py` & `contique-0.1.9/contique/helpers.py`

 * *Files identical despite different names*

### Comparing `contique-0.1.8/contique/jacobian.py` & `contique-0.1.9/contique/jacobian.py`

 * *Files identical despite different names*

### Comparing `contique-0.1.8/contique/newton.py` & `contique-0.1.9/contique/newton.py`

 * *Files identical despite different names*

### Comparing `contique-0.1.8/contique/newtonxt.py` & `contique-0.1.9/contique/newtonxt.py`

 * *Files identical despite different names*

### Comparing `contique-0.1.8/contique/printinfo.py` & `contique-0.1.9/contique/printinfo.py`

 * *Files identical despite different names*

### Comparing `contique-0.1.8/contique/solve.py` & `contique-0.1.9/contique/solve.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,22 +34,22 @@
     jac=None,
     args=(None,),
     dxmax=0.05,
     dlpfmax=0.05,
     control0="lpf",
     jacmode=3,
     jaceps=None,
-    maxsteps=80,
+    maxsteps=50,
     maxcycles=4,
-    maxiter=20,
+    maxiter=8,
     tol=1e-6,
     overshoot=1.0,
     rebalance=False,
     increase=0.5,
-    decrease=4.0,
+    decrease=2.0,
     high=10,
     low=1e-6,
     minlastfailed=3,
 ):
     """Numeric continuation of (nonlinear) equilibrium equations.
 
     Parameters
```

### Comparing `contique-0.1.8/contique.egg-info/PKG-INFO` & `contique-0.1.9/contique.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contique
-Version: 0.1.8
+Version: 0.1.9
 Summary: Numerical continuation of nonlinear equilibrium equations
 Home-page: https://github.com/adtzlr/contique
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License: GPL-3.0-or-later
 Project-URL: Code, https://github.com/adtzlr/contique
 Project-URL: Issues, https://github.com/adtzlr/contique/issues
```

### Comparing `contique-0.1.8/setup.cfg` & `contique-0.1.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = contique
-version = 0.1.8
+version = 0.1.9
 author = Andreas Dutzler
 author_email = a.dutzler@gmail.com
 description = Numerical continuation of nonlinear equilibrium equations
 url = https://github.com/adtzlr/contique
 project_urls = 
 	Code=https://github.com/adtzlr/contique
 	Issues=https://github.com/adtzlr/contique/issues
```

### Comparing `contique-0.1.8/test/test_archimedean_spiral.py` & `contique-0.1.9/test/test_archimedean_spiral.py`

 * *Files identical despite different names*

### Comparing `contique-0.1.8/test/test_lituus_spiral.py` & `contique-0.1.9/test/test_lituus_spiral.py`

 * *Files identical despite different names*

### Comparing `contique-0.1.8/test/test_log_spiral.py` & `contique-0.1.9/test/test_log_spiral.py`

 * *Files identical despite different names*

### Comparing `contique-0.1.8/test/test_sin_rebalance.py` & `contique-0.1.9/test/test_sin_rebalance.py`

 * *Files identical despite different names*

### Comparing `contique-0.1.8/test/test_sincos.py` & `contique-0.1.9/test/test_sincos.py`

 * *Files identical despite different names*


# Comparing `tmp/invopt-0.0.1.tar.gz` & `tmp/invopt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invopt-0.0.1.tar", last modified: Tue May  2 08:11:52 2023, max compression
+gzip compressed data, was "invopt-0.0.2.tar", last modified: Fri May 12 10:50:40 2023, max compression
```

## Comparing `invopt-0.0.1.tar` & `invopt-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 08:11:52.138140 invopt-0.0.1/
--rw-rw-rw-   0        0        0     1099 2023-05-01 20:52:18.000000 invopt-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      633 2023-05-02 08:11:52.125631 invopt-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       43 2023-05-01 20:57:00.000000 invopt-0.0.1/README.md
--rw-rw-rw-   0        0        0      743 2023-05-02 08:00:55.000000 invopt-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 08:11:52.138140 invopt-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-02 08:11:52.106375 invopt-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 08:11:52.125631 invopt-0.0.1/src/invopt/
--rw-rw-rw-   0        0        0      371 2023-05-02 08:10:57.000000 invopt-0.0.1/src/invopt/__init__.py
--rw-rw-rw-   0        0        0    52794 2023-05-01 15:41:02.000000 invopt-0.0.1/src/invopt/main.py
-drwxrwxrwx   0        0        0        0 2023-05-02 08:11:52.125631 invopt-0.0.1/src/invopt.egg-info/
--rw-rw-rw-   0        0        0      633 2023-05-02 08:11:52.000000 invopt-0.0.1/src/invopt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-02 08:11:52.000000 invopt-0.0.1/src/invopt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 08:11:52.000000 invopt-0.0.1/src/invopt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-05-02 08:11:52.000000 invopt-0.0.1/src/invopt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-02 08:11:52.000000 invopt-0.0.1/src/invopt.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 08:11:52.125631 invopt-0.0.1/tests/
--rw-rw-rw-   0        0        0     1607 2023-05-01 19:31:41.000000 invopt-0.0.1/tests/test_examples.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:50:40.340857 invopt-0.0.2/
+-rw-rw-rw-   0        0        0     1099 2023-05-01 20:52:18.000000 invopt-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2991 2023-05-12 10:50:40.340857 invopt-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2401 2023-05-11 19:19:40.000000 invopt-0.0.2/README.md
+-rw-rw-rw-   0        0        0      712 2023-05-12 10:50:14.000000 invopt-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-12 10:50:40.340857 invopt-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-12 10:50:40.300486 invopt-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-12 10:50:40.312416 invopt-0.0.2/src/invopt/
+-rw-rw-rw-   0        0        0      371 2023-05-02 08:10:57.000000 invopt-0.0.2/src/invopt/__init__.py
+-rw-rw-rw-   0        0        0    53363 2023-05-12 10:48:05.000000 invopt-0.0.2/src/invopt/main.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:50:40.336879 invopt-0.0.2/src/invopt.egg-info/
+-rw-rw-rw-   0        0        0     2991 2023-05-12 10:50:40.000000 invopt-0.0.2/src/invopt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-12 10:50:40.000000 invopt-0.0.2/src/invopt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 10:50:40.000000 invopt-0.0.2/src/invopt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-12 10:50:40.000000 invopt-0.0.2/src/invopt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-12 10:50:40.000000 invopt-0.0.2/src/invopt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 10:50:40.338871 invopt-0.0.2/tests/
+-rw-rw-rw-   0        0        0     1682 2023-05-12 10:16:00.000000 invopt-0.0.2/tests/test_examples.py
```

### Comparing `invopt-0.0.1/LICENSE.txt` & `invopt-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `invopt-0.0.1/pyproject.toml` & `invopt-0.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "invopt"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Pedro Zattoni Scroccaro", email="pedroszattoni@gmail.com" },
 ]
 description = "Inverse Optimization with Python"
 readme = "README.md"
 keywords = ["inverse-optimization"]
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "numpy",
-    "gurobipy",
-    "cvxpy"
+    "numpy"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/pedroszattoni/invopt"
 "Bug Tracker" = "https://github.com/pedroszattoni/inverse-optimization/issues"
```

### Comparing `invopt-0.0.1/src/invopt/main.py` & `invopt-0.0.2/src/invopt/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """
 invopt: Inverse Optimization with Python.
 
 Author: Pedro Zattoni Scroccaro
 """
 
 import numpy as np
-import gurobipy as gp
-import cvxpy as cp
 import warnings
 
 
 def check_Theta(Theta):
     """Check if Theta is valid."""
     if Theta not in [None, 'nonnegative']:
         raise Exception('Invalid Theta. Accepted values are: None (default) '
@@ -334,14 +332,20 @@
 
     Returns
     -------
     theta_opt : 1D ndarray
         An optimal cost vector according to the chosen strategy.
 
     """
+    try:
+        import gurobipy as gp
+    except ImportError:
+        print("gurobipy is required for invopt's discrete_model_consistent " +
+              "function.")
+
     # Check if inputs are valid
     check_Theta(Theta)
     check_decision_space(decision_space)
     check_regularizer(regularizer)
 
     warning_large_decision_space(decision_space)
 
@@ -506,14 +510,19 @@
 
     Returns
     -------
     theta_opt : 1D ndarray
         An optimal cost vector according to the chosen strategy.
 
     """
+    try:
+        import gurobipy as gp
+    except ImportError:
+        print("gurobipy is required for invopt's discrete_model function.")
+
     # Check if inputs are valid
     check_Theta(Theta)
     check_decision_space(decision_space)
     check_regularizer(regularizer)
     check_reg_parameter(reg_param)
     check_dist_func(dist_func, sub_loss)
 
@@ -678,14 +687,19 @@
 
     Returns
     -------
     theta_opt : 1D ndarray
         An optimal cost vector according to the chosen strategy.
 
     """
+    try:
+        import gurobipy as gp
+    except ImportError:
+        print("gurobipy is required for invopt's MIP_linear function.")
+
     # Check if inputs are valid
     check_Theta(Theta)
     check_decision_space(decision_space)
     check_regularizer(regularizer)
     check_reg_parameter(reg_param)
     check_dist_func(dist_func, sub_loss)
 
@@ -876,16 +890,16 @@
     FOP : callable
         (Augmented) forward optimization problem. Takes as input a cost vector
         theta, a signal s, and the respective response x. Returns the optimal
         (augmented) response. When using the Augmented Suboptimality loss,
         an augmented FOP should be used. Syntax: FOP(theta, s), or
         FOP(theta, s, x) for an augmented FOP.
     step_size : callable
-        Step-size function. Takes as input the iteration counter t and returns
-        the step-size. Syntax: step_size(t).
+        Step-size function. Takes as input the iteration counter t = 0,...,T-1
+        and returns the step-size. Syntax: step_size(t).
     T : int
         Number of iterations the algorithm is run.
     Theta : {None, 'nonnegative'}, optional
         Constraints on cost vector theta. The default is None.
     step : {'standard', 'exponentiated'}, optional
         Type of update step used for the first-order algorithm. If 'standard',
         uses standard "subgradient method" update steps:
@@ -1238,14 +1252,19 @@
 
     Returns
     -------
     theta_opt : 1D ndarray
         An optimal cost vector according to the chosen strategy.
 
     """
+    try:
+        import cvxpy as cp
+    except ImportError:
+        print("cvxpy is required for invopt's MIP_quadratic function.")
+
     # Check if inputs are valid
     check_Theta(Theta)
     check_decision_space(decision_space)
     check_regularizer(regularizer)
     check_reg_parameter(reg_param)
 
     # Warnings
```

### Comparing `invopt-0.0.1/tests/test_examples.py` & `invopt-0.0.2/tests/test_examples.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,29 +22,29 @@
     else:
         print(f"Script {script_name} ran successfully.")
         return True
 
 
 class TestScript(unittest.TestCase):
     def test_binary_LP_consistent_data(self):
-        script_name = 'binary_LP_consistent_data.py'
+        script_name = 'discrete_model_consistent\\binary_LP_consistent_data.py'
         self.assertTrue(test_script(path_to_examples, script_name))
 
     def test_binary_LP_inconsistent_data(self):
-        script_name = 'binary_LP_inconsistent_data.py'
+        script_name = 'discrete_model\\binary_LP_inconsistent_data.py'
         self.assertTrue(test_script(path_to_examples, script_name))
 
     def test_first_order_methods(self):
-        script_name = 'first_order_methods.py'
+        script_name = 'FOM\\first_order_methods.py'
         self.assertTrue(test_script(path_to_examples, script_name))
 
     def test_MILP(self):
-        script_name = 'MILP.py'
+        script_name = 'MIP_linear\\MILP.py'
         self.assertTrue(test_script(path_to_examples, script_name))
 
     def test_MIQP(self):
-        script_name = 'MIQP.py'
+        script_name = 'MIP_quadratic\\MIQP.py'
         self.assertTrue(test_script(path_to_examples, script_name))
 
 
 if __name__ == '__main__':
     unittest.main()
```


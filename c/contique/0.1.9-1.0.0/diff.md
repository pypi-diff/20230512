# Comparing `tmp/contique-0.1.9.tar.gz` & `tmp/contique-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contique-0.1.9.tar", last modified: Fri Mar  5 15:25:52 2021, max compression
+gzip compressed data, was "contique-1.0.0.tar", last modified: Fri May 12 21:15:12 2023, max compression
```

## Comparing `contique-0.1.9.tar` & `contique-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-05 15:25:52.408573 contique-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (116)    35149 2021-03-05 15:25:43.000000 contique-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       33 2021-03-05 15:25:43.000000 contique-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     8272 2021-03-05 15:25:52.408573 contique-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6238 2021-03-05 15:25:43.000000 contique-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-05 15:25:52.408573 contique-0.1.9/contique/
--rw-r--r--   0 runner    (1001) docker     (116)       22 2021-03-05 15:25:43.000000 contique-0.1.9/contique/__about__.py
--rw-r--r--   0 runner    (1001) docker     (116)      138 2021-03-05 15:25:43.000000 contique-0.1.9/contique/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2859 2021-03-05 15:25:43.000000 contique-0.1.9/contique/helpers.py
--rw-r--r--   0 runner    (1001) docker     (116)     3292 2021-03-05 15:25:43.000000 contique-0.1.9/contique/jacobian.py
--rw-r--r--   0 runner    (1001) docker     (116)     4350 2021-03-05 15:25:43.000000 contique-0.1.9/contique/newton.py
--rw-r--r--   0 runner    (1001) docker     (116)     5228 2021-03-05 15:25:43.000000 contique-0.1.9/contique/newtonxt.py
--rw-r--r--   0 runner    (1001) docker     (116)     1779 2021-03-05 15:25:43.000000 contique-0.1.9/contique/printinfo.py
--rw-r--r--   0 runner    (1001) docker     (116)     7246 2021-03-05 15:25:43.000000 contique-0.1.9/contique/solve.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-05 15:25:52.408573 contique-0.1.9/contique.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     8272 2021-03-05 15:25:52.000000 contique-0.1.9/contique.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      507 2021-03-05 15:25:52.000000 contique-0.1.9/contique.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-05 15:25:52.000000 contique-0.1.9/contique.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2021-03-05 15:25:52.000000 contique-0.1.9/contique.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2021-03-05 15:25:52.000000 contique-0.1.9/contique.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       93 2021-03-05 15:25:43.000000 contique-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)     1076 2021-03-05 15:25:52.408573 contique-0.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-05 15:25:52.408573 contique-0.1.9/test/
--rw-r--r--   0 runner    (1001) docker     (116)     1140 2021-03-05 15:25:43.000000 contique-0.1.9/test/test_archimedean_spiral.py
--rw-r--r--   0 runner    (1001) docker     (116)     1197 2021-03-05 15:25:43.000000 contique-0.1.9/test/test_lituus_spiral.py
--rw-r--r--   0 runner    (1001) docker     (116)     1215 2021-03-05 15:25:43.000000 contique-0.1.9/test/test_log_spiral.py
--rw-r--r--   0 runner    (1001) docker     (116)     1161 2021-03-05 15:25:43.000000 contique-0.1.9/test/test_sin_rebalance.py
--rw-r--r--   0 runner    (1001) docker     (116)     1085 2021-03-05 15:25:43.000000 contique-0.1.9/test/test_sincos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:15:12.408379 contique-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-05-12 21:15:03.000000 contique-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    49268 2023-05-12 21:15:12.408379 contique-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-05-12 21:15:03.000000 contique-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-12 21:15:03.000000 contique-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 21:15:12.408379 contique-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:15:12.404379 contique-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:15:12.404379 contique-1.0.0/src/contique/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-12 21:15:03.000000 contique-1.0.0/src/contique/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-12 21:15:03.000000 contique-1.0.0/src/contique/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-12 21:15:03.000000 contique-1.0.0/src/contique/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-12 21:15:03.000000 contique-1.0.0/src/contique/jacobian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-05-12 21:15:03.000000 contique-1.0.0/src/contique/newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-05-12 21:15:03.000000 contique-1.0.0/src/contique/newtonxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-05-12 21:15:03.000000 contique-1.0.0/src/contique/numcont.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-12 21:15:03.000000 contique-1.0.0/src/contique/printinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:15:12.404379 contique-1.0.0/src/contique.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    49268 2023-05-12 21:15:12.000000 contique-1.0.0/src/contique.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-12 21:15:12.000000 contique-1.0.0/src/contique.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 21:15:12.000000 contique-1.0.0/src/contique.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-12 21:15:12.000000 contique-1.0.0/src/contique.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 21:15:12.000000 contique-1.0.0/src/contique.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:15:12.404379 contique-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-12 21:15:03.000000 contique-1.0.0/tests/test_archimedean_spiral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-12 21:15:03.000000 contique-1.0.0/tests/test_archimedean_spiral_noargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-12 21:15:03.000000 contique-1.0.0/tests/test_bratu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-12 21:15:03.000000 contique-1.0.0/tests/test_lituus_spiral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-12 21:15:03.000000 contique-1.0.0/tests/test_log_spiral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-12 21:15:03.000000 contique-1.0.0/tests/test_sin_rebalance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-12 21:15:03.000000 contique-1.0.0/tests/test_sincos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-12 21:15:03.000000 contique-1.0.0/tests/test_twotruss.py
```

### Comparing `contique-0.1.9/LICENSE` & `contique-1.0.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -627,16 +627,16 @@
 free software which everyone can redistribute and change under these terms.
 
   To do so, attach the following notices to the program.  It is safest
 to attach them to the start of each source file to most effectively
 state the exclusion of warranty; and each file should have at least
 the "copyright" line and a pointer to where the full notice is found.
 
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
+    Numerical continuation of nonlinear equilibrium equations.
+    Copyright (C) 2023  Andreas Dutzler
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
@@ -648,15 +648,15 @@
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Also add information on how to contact you by electronic and paper mail.
 
   If the program does terminal interaction, make it output a short
 notice like this when it starts in an interactive mode:
 
-    <program>  Copyright (C) <year>  <name of author>
+    contique  Copyright (C) 2023  Andreas Dutzler
     This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
     This is free software, and you are welcome to redistribute it
     under certain conditions; type `show c' for details.
 
 The hypothetical commands `show w' and `show c' should show the appropriate
 parts of the General Public License.  Of course, your program's commands
 might be different; for a GUI interface, you would use an "about box".
```

### Comparing `contique-0.1.9/PKG-INFO` & `contique-1.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,145 +1,146 @@
-Metadata-Version: 2.1
-Name: contique
-Version: 0.1.9
-Summary: Numerical continuation of nonlinear equilibrium equations
-Home-page: https://github.com/adtzlr/contique
-Author: Andreas Dutzler
-Author-email: a.dutzler@gmail.com
-License: GPL-3.0-or-later
-Project-URL: Code, https://github.com/adtzlr/contique
-Project-URL: Issues, https://github.com/adtzlr/contique/issues
-Description: # contique
-        Numeric **conti**nuation of nonlinear e**qu**ilibrium **e**quations
-        
-        [![PyPI version shields.io](https://img.shields.io/pypi/v/contique.svg)](https://pypi.python.org/pypi/contique/)
-        [![PyPI pyversions](https://img.shields.io/pypi/pyversions/contique.svg)](https://pypi.python.org/pypi/contique/)
-        ![Made with love in Graz](https://madewithlove.now.sh/at?heart=true&colorA=%233b3b3b&colorB=%231f744f&text=Graz)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        
-        <img src="https://raw.githubusercontent.com/adtzlr/contique/main/test/test_archimedean_spiral.svg" width="75%">
-        
-        Fig. 1 [Archimedean spiral](https://en.wikipedia.org/wiki/Archimedean_spiral) equation solved with [contique](https://github.com/adtzlr/contique/blob/main/test/test_archimedean_spiral.py)
-        
-        ## Theory of `contique`'s numeric continuation
-        
-        A solution curve for `(n)` equilibrium equations `fun` in terms of `(n)` unknowns `x` and a load-proportionality-factor `lpf` should be found by numeric continuation from an initial equilibrium state `fun(x0, lpf0) = 0`. Contique's numeric continuation method is best classified as a 
-        - **component-based continuation** with an adaptive 
-        - **magnitude-based control-component switching**.
-          
-        ### Extended equilibrium equations
-        The `lpf` value is appended to the unknows `x` which gives the so-called extended unknowns `y = [x, lpf]`. One additional control equation is added to the equilibrium equations to ensure `(n+1)` equations in terms of `(n+1)` extended unknowns (see next section). This reduces the solution to a point on the initial solution curve.
-        
-        ### Control Equation
-        The control equation is defined as follows: First, a needle-vector with dimension `(n+1)` is created and filled with zeros `needle = 0`. For a given initial signed control component `j` the needle is positioned at `needle[|j|] = 1`. The maximum allowed values per component are calculated as `ymax = y0 + np.sign(j) dymax`. The control equation is finally formulated as `f(y) = needle.T (y - ymax)`.
-        
-        ### Solution technique
-        The numeric solution process is divided into three main parts:
-        
-        - **Step**
-            + Cycle
-                * *Iteration* (...of a Newton-Rhapson root method)
-          
-        As the name implies, a **Step** tries to find the extended unknowns for the next step forward of the equilibrium state. For each Cycle, the initial control component has to be evaluated first (see comment below). The additional control equation is evaluated with this initial control component. The generated extended equilibrium equations in terms of the extended unknows are now solved with the help of a root method (Newton-Rhapson *Iterations*). The solution of the root method `dy` is further normalized as `dy/dymax` and the final control component is evaluated as `j = |j| sign((dy/dymax)[|j|])` with `|j| = argmax(|dy/dymax|)`. If the control component changed, another Cycle is performed with the initial control component being now the final control component of the last cycle. This Cycle-loop is repeated until the control component does not change anymore.
-        
-        A note on the pre-evaluation of the initial control component of a **Step**: This is performed by the linear solution of the extended equilibrium equations. It is equal to the result of the first *Iteration* of the Newton-Rhapson root method.
-        
-        ## Example
-        A given set of equilibrium equations in terms of `x` and `lpf` (a.k.a. load-proportionality-factor) should be solved by numeric continuation of a given initial solution.
-        
-        ### Function definition
-        ```python
-        def fun(x, lpf, a, b):
-            return np.array([-a * np.sin(x[0]) + x[1]**2 + lpf, 
-                             -b * np.cos(x[1]) * x[1]    + lpf])
-        ```
-        
-        with its initial solution
-        ```python
-        x0 = np.zeros(2)
-        lpf0 = 0.0
-        ```
-        
-        and function parameters
-        ```python
-        a = 1
-        b = 1
-        ```
-        
-        ### Run `contique.solve` and plot equilibrium states
-        
-        ```python
-        Res = contique.solve(
-            fun=fun,
-            x0=x0,
-            args=(a, b),
-            lpf0=lpf0,
-            dxmax=0.1,
-            dlpfmax=0.1,
-            maxsteps=75,
-            maxcycles=4,
-            maxiter=20,
-            tol=1e-8,
-            overshoot=1.05
-        )
-        ```
-        
-        For each `step` a summary is printed out per `cylce`. This contains an information about the control component at the beginning and the end of a cycle as well as the norm of the residuals along with needed Newton-Rhapson `iterations` per `cycle`. As an example the ouput of some interesting `steps` 31-33 and 38-40 are shown below. The last column contains messages about the solution. On the one hand, in `step` 32, `cycle` 1 the control component changed from `+1` to `-2`, but the relative overshoot on the final control component `-2` was inside the tolerated range of `overshoot=1.05`. Therefore the solver proceeds with `step` 33 without re-cycling `step` 32. On the other hand, in `step` 39, `cycle` 1 the control component changed from `-2` to `-1` and this time the overshoot on the final control component `-1` was outside the tolerated range. A new `cycle` 2 is performed for `step` 39 with the new control component `-1`.
-        
-        ```markdown
-        |Step,C.| Control Comp. | Norm (Iter.#) | Message     |
-        |-------|---------------|---------------|-------------|
-        
-        (...)
-        
-        |  31,1 |   +1  =>   +1 | 7.6e-10 ( 3#) |             |
-        |  32,1 |   +1  =>   -2 | 1.7e-14 ( 4#) |tol.Overshoot|
-        |  33,1 |   -2  =>   -2 | 4.8e-12 ( 3#) |             |
-        
-         (...)
-         
-        |  38,1 |   -2  =>   -2 | 9.2e-12 ( 3#) |             |
-        |  39,1 |   -2  =>   -1 | 1.9e-13 ( 3#) | => re-Cycle |
-        |     2 |   -1  =>   -1 | 2.3e-13 ( 4#) |             |
-        |  40,1 |   -1  =>   -1 | 7.9e-09 ( 3#) |             |
-        
-        (...)
-        ```
-        
-        Next, we have to assemble the results
-        
-        ```python
-        X = np.array([res.x for res in Res])
-        ```
-        
-        and plot the solution curve.
-        
-        ```python
-        import matplotlib.pyplot as plt
-        
-        plt.plot(X[:, 0], X[:, 1], "C0.-")
-        plt.xlabel('$x_1$')
-        plt.ylabel('$x_2$')
-        plt.plot([0],[0],'C0o',lw=3)
-        plt.arrow(X[-2,0],X[-2,1],X[-1,0]-X[-2,0],X[-1,1]-X[-2,1],
-                  head_width=0.075, head_length=0.15, fc='C0', ec='C0')
-        plt.gca().set_aspect('equal')
-        ```
-        
-        <img src="https://raw.githubusercontent.com/adtzlr/contique/main/test/test_sincos.svg" width="75%">
-        
-        Fig. 2 Solution states of [equilibrium equations](https://github.com/adtzlr/contique/blob/main/test/test_sincos.py) solved with contique
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+<p align="center">
+  <img src="https://github.com/adtzlr/contique/assets/5793153/86662194-2e2f-4dd6-b7de-5adf3270105d" height="80px"/>
+  <p align="center">Numerical continuation of nonlinear equilibrium equations.</p>
+</p>
+
+[![PyPI version shields.io](https://img.shields.io/pypi/v/contique.svg)](https://pypi.python.org/pypi/contique/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/contique.svg)](https://pypi.python.org/pypi/contique/)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+![Made with love in Graz](https://madewithlove.now.sh/at?heart=true&colorA=%233b3b3b&colorB=%231f744f&text=Graz)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7931300.svg)](https://doi.org/10.5281/zenodo.7931300)
+[![codecov](https://codecov.io/gh/adtzlr/contique/branch/main/graph/badge.svg?token=CXKRL8TLQY)](https://codecov.io/gh/adtzlr/contique)
+
+Contique is a Python 3.7+ package that provides methods for numeric continuation. It depends on
+- `numpy` (for arrays) and
+- `scipy` (check if matrix is sparse and sparse solver).
+
+> **Note**
+> The original motivation was to create a generalized standalone package with the built-in numeric continuation methods taken from the nonlinear truss analysis package [trusspy](https://github.com/adtzlr/trusspy).
+
+## Theory of `contique`'s numeric continuation
+
+A solution curve for `(n)` equilibrium equations `fun` in terms of `(n)` unknowns `x` and a load-proportionality-factor `lpf` should be found by numeric continuation from an initial equilibrium state `fun(x0, lpf0) = 0`. Contique's numeric continuation method is best classified as a 
+
+- **component-based continuation** with an adaptive 
+- **magnitude-based control-component switching**.
+
+
+<a href="https://github.com/adtzlr/contique/blob/main/tests/test_archimedean_spiral.py"><img src="https://github.com/adtzlr/contique/assets/5793153/6b38c783-bdfc-470a-8a66-82a3ca663407" width="75%"></a>
+
+Fig. 1 [Archimedean spiral](https://en.wikipedia.org/wiki/Archimedean_spiral) equation solved with [contique](https://github.com/adtzlr/contique/blob/main/tests/test_archimedean_spiral.py)
+  
+### Extended equilibrium equations
+The `lpf` value is appended to the unknows `x` which gives the so-called extended unknowns `y = [x, lpf]`. One additional control equation is added to the equilibrium equations to ensure `(n+1)` equations in terms of `(n+1)` extended unknowns (see next section). This reduces the solution to a point on the initial solution curve.
+
+### Control Equation
+The control equation is defined as follows: First, a needle-vector with dimension `(n+1)` is created and filled with zeros `needle = 0`. For a given initial signed control component `j` the needle is positioned at `needle[|j|] = 1`. The maximum allowed values per component are calculated as `ymax = y0 + np.sign(j) dymax`. The control equation is finally formulated as `f(y) = needle.T (y - ymax)`.
+
+### Solution technique
+The numeric solution process is divided into three main parts:
+
+- **Step**
+    + Cycle
+        * *Iteration* (...of a Newton-Rhapson root method)
+  
+As the name implies, a **Step** tries to find the extended unknowns for the next step forward of the equilibrium state. For each Cycle, the initial control component has to be evaluated first (see comment below). The additional control equation is evaluated with this initial control component. The generated extended equilibrium equations in terms of the extended unknows are now solved with the help of a root method (Newton-Rhapson *Iterations*). The solution of the root method `dy` is further normalized as `dy/dymax` and the final control component is evaluated as `j = |j| sign((dy/dymax)[|j|])` with `|j| = argmax(|dy/dymax|)`. If the control component changed, another Cycle is performed with the initial control component being now the final control component of the last cycle. This Cycle-loop is repeated until the control component does not change anymore.
+
+A note on the pre-evaluation of the initial control component of a **Step**: This is performed by the linear solution of the extended equilibrium equations. It is equal to the result of the first *Iteration* of the Newton-Rhapson root method.
+
+## Example
+A given set of equilibrium equations in terms of `x` and `lpf` (a.k.a. load-proportionality-factor) should be solved by numeric continuation of a given initial solution.
+
+### Function definition
+```python
+def fun(x, lpf, a, b):
+    return np.array(
+        [-a * np.sin(x[0]) + x[1] ** 2 + lpf, -b * np.cos(x[1]) * x[1] + lpf]
+    )
+```
+
+with its initial solution
+```python
+x0 = np.zeros(2)
+lpf0 = 0.0
+```
+
+and function parameters
+```python
+a = 1
+b = 1
+```
+
+### Run `contique.solve` and plot equilibrium states
+
+```python
+Res = contique.solve(
+    fun=fun,
+    x0=x0,
+    args=(a, b),
+    lpf0=lpf0,
+    dxmax=0.1,
+    dlpfmax=0.1,
+    maxsteps=75,
+    maxcycles=4,
+    maxiter=20,
+    tol=1e-8,
+    overshoot=1.05,
+)
+```
+
+For each `step` a summary is printed out per `cycle`. This contains an information about the control component at the beginning and the end of a cycle as well as the norm of the residuals along with needed Newton-Rhapson `iterations` per `cycle`. As an example the ouput of some interesting `steps` 31-33 and 38-40 are shown below. The last column contains messages about the solution. On the one hand, in `step` 32, `cycle` 1 the control component changed from `+1` to `-2`, but the relative overshoot on the final control component `-2` was inside the tolerated range of `overshoot=1.05`. Therefore the solver proceeds with `step` 33 without re-cycling `step` 32. On the other hand, in `step` 39, `cycle` 1 the control component changed from `-2` to `-1` and this time the overshoot on the final control component `-1` was outside the tolerated range. A new `cycle` 2 is performed for `step` 39 with the new control component `-1`.
+
+```markdown
+|Step,C.| Control Comp. | Norm (Iter.#) | Message     |
+|-------|---------------|---------------|-------------|
+
+(...)
+
+|  31,1 |   +1  =>   +1 | 7.6e-10 ( 3#) |             |
+|  32,1 |   +1  =>   -2 | 1.7e-14 ( 4#) |tol.Overshoot|
+|  33,1 |   -2  =>   -2 | 4.8e-12 ( 3#) |             |
+
+ (...)
+ 
+|  38,1 |   -2  =>   -2 | 9.2e-12 ( 3#) |             |
+|  39,1 |   -2  =>   -1 | 1.9e-13 ( 3#) | => re-Cycle |
+|     2 |   -1  =>   -1 | 2.3e-13 ( 4#) |             |
+|  40,1 |   -1  =>   -1 | 7.9e-09 ( 3#) |             |
+
+(...)
+```
+
+Next, we have to assemble the results
+
+```python
+X = np.array([res.x for res in Res])
+```
+
+and plot the solution curve.
+
+```python
+import matplotlib.pyplot as plt
+
+plt.plot(X[:, 0], X[:, 1], "C0.-")
+plt.xlabel("$x_1$")
+plt.ylabel("$x_2$")
+plt.plot([0], [0], "C0o", lw=3)
+plt.arrow(
+    X[-2, 0],
+    X[-2, 1],
+    X[-1, 0] - X[-2, 0],
+    X[-1, 1] - X[-2, 1],
+    head_width=0.075,
+    head_length=0.15,
+    fc="C0",
+    ec="C0",
+)
+plt.gca().set_aspect("equal")
+```
+
+<a href="https://github.com/adtzlr/contique/blob/main/tests/test_sincos.py"><img src="https://github.com/adtzlr/contique/assets/5793153/20fb6415-d226-4859-b818-4f79194ba1e2" width="75%"></a>
+
+Fig. 2 Solution states of [equilibrium equations](https://github.com/adtzlr/contique/blob/main/tests/test_sincos.py) solved with contique
+
+# Changelog
+All notable changes to this project will be documented in [this file](CHANGELOG.md). The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
```

### Comparing `contique-0.1.9/contique/jacobian.py` & `contique-1.0.0/src/contique/jacobian.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,12 @@
-# -*- coding: utf-8 -*-
 """
-Created on Wed Feb 17 14:31:04 2021
-
-@author: adtzlr
-
-Contique - Numeric continuation of equilibrium equations
-Copyright (C) 2021 Andreas Dutzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <https://www.gnu.org/licenses/>.
+contique: Numerical continuation of nonlinear equilibrium equations.
+Andreas Dutzler, 2023
 """
+
 import copy
 import numpy as np
 
 
 def jacobian(fun, argnum=0, h=None, mode=3):
     """Decorator for the jacobian as 2- or 3-point finite-differences
     approximation w.r.t. a given argnum and h.
```

### Comparing `contique-0.1.9/contique/newton.py` & `contique-1.0.0/src/contique/newton.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,13 @@
-# -*- coding: utf-8 -*-
 """
-Created on Wed Feb 17 14:31:04 2021
-
-@author: adtzlr
-
-Contique - Numeric continuation of equilibrium equations
-Copyright (C) 2021 Andreas Dutzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <https://www.gnu.org/licenses/>.
+contique: Numerical continuation of nonlinear equilibrium equations.
+Andreas Dutzler, 2023
 """
 import numpy as np
+from scipy import sparse
 
 from .helpers import argparser
 
 
 class NewtonResult:
     """Class for handling the results of a Newton-Rhapson solution.
 
@@ -33,15 +16,16 @@
     Attributes
     ----------
     success : bool
         flag for the converged solution
     message : str
         message for the state
     status : int
-        integer representig the status of the solution (0 if not converged, 1 if converged).
+        integer representig the status of the solution (0 if not converged, 1 if
+        converged).
     niterations : int
         number of performed iterations
     x : ndarray
         1d-array containing the unknows
     fun : function
         function returning the equilibrium equations
     jac : function
@@ -54,69 +38,85 @@
 
         Parameters
         ----------
         fun : function
             function returning the equilibrium equations
         x0 : ndarray
             1d-array containing the initial unknows
-        jac : function
+        jac : function, optional
             function returning the jacobian of the equilibrium equations
         args : tuple, optional
             Optional tuple of arguments which are passed to the function. Eeven if only
-            one argument is passed, it has to be encapsulated in a tuple (default is (None,)).
+            one argument is passed, it has to be encapsulated in a tuple (default is
+            (None,)).
 
         """
         self.success = False
         self.message = "not started"
         self.status = 0
         self.niterations = 0
         self.x = x0.copy()
         self.fun = argparser(fun)(self.x, *args)
-        self.jac = argparser(jac)(self.x, *args)
+
+        if jac is not None:
+            self.jac = argparser(jac)(self.x, *args)
 
 
-def newtonrhapson(fun, x0, jac, args=(None,), maxiter=8, tol=1e-8):
+def newtonrhapson(fun, x0, jac, args=(None,), maxiter=8, tol=1e-8, solve=None):
     """A simple n-dimensional Newton-Rhapson solver.
 
     Parameters
     ----------
     fun : function
         function in terms of unknows x and optional args which returns the
         equilibrium equations.
     x0 : ndarray
         1d-array with initial values of unknows x
     jac : function
         jacobian of fun w.r.t. the unknows x
     args : tuple, optional
         Optional tuple of arguments which are passed to the function. Eeven if only
-        one argument is passed, it has to be encapsulated in a tuple (default is (None,)).
+        one argument is passed, it has to be encapsulated in a tuple (default is
+        (None,)).
     maxiter : int, optional
         maximum number of iterations (default is 8)
     tol : float, optional
         tolerated residual of the norm of the equilibrium equation (default is 1e-8)
 
     Returns
     -------
     res : NewtonResult
         Instance of NewtonResult with res.x being the final unknowns
 
     """
 
     # init result object with initial function evaluation
-    res = NewtonResult(fun, x0, jac, args)
+    res = NewtonResult(fun, x0, None, args)
 
     # iteration loop
     for res.niterations in range(1, 1 + maxiter):
 
+        # calculate jacobian at x
+        res.jac = argparser(jac)(res.x, *args)
+
+        # set solver according to dense or sparse jacobian
+        if solve is None:
+            if sparse.issparse(res.jac):
+                solve = sparse.linalg.spsolve
+            else:
+                solve = np.linalg.solve
+
         # solve linear equation system
-        res.x += np.linalg.solve(res.jac, -res.fun)
+        try:
+            res.x += solve(res.jac, -res.fun)
+        except:  # NOQA: E722
+            res.x *= np.nan
 
-        # calculate function and jacobian at updated x
+        # calculate function at updated x
         res.fun = argparser(fun)(res.x, *args)
-        res.jac = argparser(jac)(res.x, *args)
 
         # convergence check
         if np.linalg.norm(res.fun) < tol:
             res.success = True
             res.status = 1
             res.message = "Solution converged in {0:2d} Iteration".format(
                 res.niterations
@@ -125,12 +125,17 @@
                 res.message = res.message + "s"
 
             break
 
     # check if newton process failed
     if not res.success:
         if maxiter == 1:
-            res.message = "Calculated linear solution because of input parameter `maxiter=1` (not converged)."
+            res.message = " ".join(
+                [
+                    "Calculated linear solution",
+                    "because of input parameter `maxiter=1` (not converged).",
+                ]
+            )
         else:
             res.message = "Newton-R. process failed."
 
     return res
```

### Comparing `contique-0.1.9/contique/newtonxt.py` & `contique-1.0.0/src/contique/newtonxt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,169 +1,201 @@
-# -*- coding: utf-8 -*-
 """
-Created on Wed Feb 17 14:31:04 2021
-
-@author: adtzlr
-
-Contique - Numeric continuation of equilibrium equations
-Copyright (C) 2021 Andreas Dutzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <https://www.gnu.org/licenses/>.
+contique: Numerical continuation of nonlinear equilibrium equations.
+Andreas Dutzler, 2023
 """
 import numpy as np
+from scipy import sparse
 
 from .jacobian import jacobian
 from .helpers import needle, control
 from .newton import newtonrhapson
 
 
-def funxt(y, n, ymax, fun, jac, jacmode, jaceps, args):
-    """Extended equilibrium equations.
+def funxt(y, needle_vector, ymax, fun, jac=None, jacmode=3, jaceps=None, args=(None,)):
+    """Extend the given equilibrium equations.
 
     Parameters
     ----------
     y : array
-        1d-array of unknowns.
-    n : array
-        pre-evaluated needle-vector.
+        1d-array of unknowns
+    needle_vector : array
+        (pre-evaluated) needle-vector
     ymax : array
-        1d-array with max. allowed values of unknows.
+        1d-array with max. allowed values of unknows
     fun : function
         1d-array of equilibrium equations
-    jac : function
-        jacobian of equilibrium euqations (not used)
-    jacmode : int
-        2 or 3-point evaulation of the jacobian (not used)
-    jaceps : float
-        a small number to evaulate the jacobian (not used)
-    args : tuple
-        optional function arguments
+    jac : function, optional
+        jacobian of fun w.r.t. the extended unknows y
+    jacmode : int, optional
+        forward (2) or central (3) finite-differences approx. of the jacobian
+    jaceps : float, optional
+        user-specified stepwidth (if None, this defaults to eps^(1/mode))
+    args : tuple, optional
+        Optional tuple of arguments which are passed to the function. Even if
+        only one argument is passed, it has to be encapsulated in a tuple
+        (default is (None,)).
 
     Returns
     -------
     array
         extended 1d-array of equilibrium equations
         with control equation
     """
 
-    x, l = y[:-1], y[-1]
-    return np.append(fun(x, l, *args), np.dot(n, (y - ymax)))
+    # split the unknowns
+    x, lpf = y[:-1], y[-1]
+
+    # evaluate the given function
+    f = fun(x, lpf, *args)
 
+    if sparse.issparse(f):
+        # convert function vector to array
+        f = f.toarray()
 
-def jacxt(y, n, ymax, fun, jac=None, jacmode=3, jaceps=None, args=(None,)):
+    # extend the function
+    return np.append(f, np.dot(needle_vector, (y - ymax)))
+
+
+def jacxt(y, needle_vector, ymax, fun, jac=None, jacmode=3, jaceps=None, args=(None,)):
     """Jacobian of extended equilibrium equations.
 
     Parameters
     ----------
     y : ndarray
         1d-array of extended unknows
-    n : ndarray
+    needle_vector : ndarray
         1d-array with pre-evaluated needle-vector
     ymax : ndarray
         1d-array with max. allowed incremental increase values of y
     fun : function
         function in terms of unknows x and optional args which returns the
         equilibrium equations.
     jac : function, optional
         jacobian of fun w.r.t. the extended unknows y
     jacmode : int, optional
         forward (2) or central (3) finite-differences approx. of the jacobian
     jaceps : float, optional
         user-specified stepwidth (if None, this defaults to eps^(1/mode))
     args : tuple, optional
-        Optional tuple of arguments which are passed to the function. Eeven if only
-        one argument is passed, it has to be encapsulated in a tuple (default is (None,)).
+        Optional tuple of arguments which are passed to the function. Even if
+        only one argument is passed, it has to be encapsulated in a tuple
+        (default is (None,)).
 
     Returns
     -------
         ndarray
-        jacobian of fun w.r.t. y (contains both derivatives of x and lpf) as 2d-array
+        jacobian of fun w.r.t. y (contains both derivatives of x and lpf)
+        as 2d-array
     """
+
+    # split the unknowns
     x, lpf = y[:-1], y[-1]
+
     if jac is None:
+        # evaluate by finite differences method
         dfundx = jacobian(fun, argnum=0, mode=jacmode, h=jaceps)
         dfundl = jacobian(fun, argnum=1, mode=jacmode, h=jaceps)
     else:
         dfundx, dfundl = jac
-    return np.vstack(
-        (np.hstack((dfundx(x, lpf, *args), dfundl(x, lpf, *args).reshape(-1, 1))), n)
-    )
+
+    # evaluate the given jacobian
+    dfdx = dfundx(x, lpf, *args)
+    dfdl = dfundl(x, lpf, *args).reshape(-1, 1)
+
+    # define horizontal and vertical stack operations based on evaluated
+    # sparse or dense jacobian
+    if sparse.issparse(dfdx):
+        hstack = sparse.hstack
+        vstack = sparse.vstack
+        array = sparse.csr_matrix
+    else:
+        hstack = np.hstack
+        vstack = np.vstack
+        array = np.array
+
+    # extend the jacobian
+    dfdy = hstack([array(dfdx), array(dfdl)])
+    dgdy = vstack([dfdy, array(needle_vector)])
+
+    if sparse.issparse(dfdx):
+        # convert to compressed sparse row format
+        dgdy = dgdy.tocsr()
+
+    return dgdy
 
 
 def newtonxt(
     fun,
     jac,
     y0,
     control0,
     dymax,
     jacmode=3,
     jaceps=None,
     args=(None,),
     maxiter=20,
     tol=1e-8,
+    solve=None,
 ):
     """Solve equilibrium equations starting from an initial solution
-    with control component and max. allowed increase of unknowns.
+    with a given control component and a max. allowed increase of unknowns.
 
     Parameters
     ----------
     fun : function
-        function in terms of unknows x and optional args which returns the
-        equilibrium equations.
+        function in terms of extended unknows and optional args which returns
+        the extended equilibrium equations
     jac : function, optional
-        jacobian of fun w.r.t. the extended unknows y
+        jacobian of fun w.r.t. the extended unknows
     y0 : ndarray
         1d-array of initial extended unknows
-    control0 : int, optional
-        initial signed control component ( 1-indexed )
+    control0 : tuple of int, optional
+        initial tuple of control component and sign
     dxmax : float, optional
         max. allowed absolute incremental increase of extended unknowns per step
     jacmode : int, optional
         forward (2) or central (3) finite-differences approx. of the jacobian
     jaceps : float, optional
         user-specified stepwidth (if None, this defaults to eps^(1/mode))
     args : tuple, optional
         Optional tuple of arguments which are passed to the function. Eeven if only
-        one argument is passed, it has to be encapsulated in a tuple (default is (None,)).
+        one argument is passed, it has to be encapsulated in a tuple (default is
+        (None,)).
     maxiter : int, optional
         max. number of Newton-iterations per cycle
     tol : float, optional
         tolerated residual of the norm of the equilibrium equation (default is 1e-8)
+    solve: callable, optional
+        A solver.
 
     Returns
     -------
     res : NewtonResult
         Instance of NewtonResult with res.x being the final extended unknowns
     """
 
     # init needle-vector and obtain ymax
-    n = needle(control0, len(y0))
-    ymax = y0 + np.sign(control0) * dymax
+    component0, sign0 = control0
+    n = needle(component0, len(y0))
+    ymax = y0 + sign0 * dymax
 
     # Newton-Rhapson solver
     res = newtonrhapson(
         fun=funxt,
         x0=y0,
         jac=jacxt,
         args=(n, ymax, fun, jac, jacmode, jaceps, args),
         maxiter=maxiter,
         tol=tol,
+        solve=solve,
     )
 
     # normalized dy = dy/dymax
     res.dys = (res.x - y0) / dymax
 
-    # final control component based on dnormalized dy
-    res.control = control(res.dys)
+    # final control component based on normalized dy
+    if np.any(np.isnan(res.dys)):
+        res.control = control0
+    else:
+        res.control = control(res.dys)
 
     return res
```

### Comparing `contique-0.1.9/contique/solve.py` & `contique-1.0.0/src/contique/numcont.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,43 @@
-# -*- coding: utf-8 -*-
 """
-Created on Wed Feb 17 14:31:04 2021
-
-@author: adtzlr
-
-Contique - Numeric continuation of equilibrium equations
-Copyright (C) 2021 Andreas Dutzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <https://www.gnu.org/licenses/>.
+contique: Numerical continuation of nonlinear equilibrium equations.
+Andreas Dutzler, 2023
 """
 
 import numpy as np
 
+from .helpers import argparser2
 from .newtonxt import newtonxt
 from . import printinfo
 
 
 def solve(
     fun,
     x0,
     lpf0,
     jac=None,
     args=(None,),
     dxmax=0.05,
     dlpfmax=0.05,
-    control0="lpf",
+    control0=(-1, 1),
     jacmode=3,
     jaceps=None,
     maxsteps=50,
     maxcycles=4,
     maxiter=8,
     tol=1e-6,
     overshoot=1.0,
     rebalance=False,
     increase=0.5,
     decrease=2.0,
     high=10,
     low=1e-6,
     minlastfailed=3,
+    solve=None,
+    callback=lambda step, res: None,
 ):
     """Numeric continuation of (nonlinear) equilibrium equations.
 
     Parameters
     ----------
     fun : function
         function in terms of unknows x and optional args which returns the
@@ -61,15 +46,16 @@
         1d-array with initial values of unknows x
     lpf0 : float
         initial value for the load-proportionality-factor
     jac : function, optional
         jacobian of fun w.r.t. the unknows x
     args : tuple, optional
         Optional tuple of arguments which are passed to the function. Eeven if only
-        one argument is passed, it has to be encapsulated in a tuple (default is (None,)).
+        one argument is passed, it has to be encapsulated in a tuple (default is
+        (None,)).
     dxmax : float, optional
         max. allowed absolute incremental increase of unknowns per step
     dlpfmax : float, optional
         max. allowed absolute incremental increase of lpf per step
     control0 : int, optional
         initial signed control component ( 1-indexed )
     jacmode : int, optional
@@ -94,97 +80,138 @@
         rebalance decrease factor
     high : float, optional
         rebalance max. factor of incremental increase w.r.t. to the initial values
     low : float, optional
         rebalance min. factor of incremental increase w.r.t. to the initial values
     minlastfailed : int, optional
         rebalance increase only after a given number of converged steps
+    solve : callable, optional
+        a function which returns the solution of a linear equation system
+    callback : callable, optional
+        a function to interact with the results of each step
 
     Returns
     -------
     Res : list
         List of NewtonResults (with res.x being the final unknowns per step)
 
     """
 
+    # allow passing empty *args to fun(x, lpf)
+    fun = argparser2(fun)
+
     # init number of unknows
     ncomp = 1 + len(x0)
 
     # init rebalance and lastfailed
     # (not used if not rebalance)
     rebalanced = False
     lastfailed = 0
 
     # initial control component
-    if control0 == "lpf":
-        j0 = ncomp
-    else:
-        j0 = control0
+    control0 = list(control0)
+    if control0[0] < 0:
+        control0[0] = ncomp - abs(control0[0])
 
     # init y=(x,l)-combined quantities
     y0 = np.append(x0, lpf0)
     dymax = np.append(np.ones_like(x0) * dxmax, dlpfmax)
     dymax0 = dymax.copy()
 
     # init list of results
-    Res = [newtonxt(fun, jac, y0, j0, dymax, jacmode, jaceps, args, maxiter=0, tol=tol)]
+    res = newtonxt(
+        fun,
+        jac,
+        y0,
+        control0,
+        dymax,
+        jacmode,
+        jaceps,
+        args,
+        maxiter=0,
+        tol=tol,
+        solve=solve,
+    )
+    yield res
 
     printinfo.header()
 
     # Step loop.
     for step in 1 + np.arange(maxsteps):
-        ## pre-identification of control component
+        # pre-identification of control component
         res = newtonxt(
-            fun, jac, y0, j0, dymax, jacmode, jaceps, args, maxiter=1, tol=tol
+            fun,
+            jac,
+            y0,
+            control0,
+            dymax,
+            jacmode,
+            jaceps,
+            args,
+            maxiter=1,
+            tol=tol,
+            solve=solve,
         )
 
         # Cycle loop.
         for cycl in 1 + np.arange(maxcycles):
 
             # Newton Iterations.
             res = newtonxt(
-                fun, jac, y0, j0, dymax, jacmode, jaceps, args, maxiter=maxiter, tol=tol
+                fun,
+                jac,
+                y0,
+                control0,
+                dymax,
+                jacmode,
+                jaceps,
+                args,
+                maxiter=maxiter,
+                tol=tol,
+                solve=solve,
             )
             printinfo.cycle(
                 step,
                 cycl,
-                j0,
+                control0,
                 res.control,
                 res.status,
                 np.linalg.norm(res.fun),
                 res.niterations,
                 max(abs(res.dys)) <= overshoot,
             )
 
             # Did Newton Iterations converge?
             if res.success:
 
-                # Did control component change? OR Was overshoot inside allowed range?
-                if (res.control == j0) or (max(abs(res.dys)) <= overshoot):
+                # Did control component change? OR
+                # Was overshoot inside allowed range?
+                if np.allclose(control0, res.control) or max(abs(res.dys)) <= overshoot:
 
                     # Save results, move to next step.
-                    j0 = res.control
+                    control0 = res.control
                     y0 = res.x
-                    Res.append(res)
+
+                    callback(step, res)
+                    yield res
                     break
 
                 else:  # Were max. number of cycles reached?
                     if cycl == maxcycles:
                         # Print Error and set success-flag to False.
                         printinfo.errorcontrol()
                         res.success = False
                     else:
                         # re-cycle Step with new control component
-                        j0 = res.control
+                        control0 = res.control
             else:
                 # break cycle loop if Newton Iterations failed.
                 break
 
         # Rebalance max. incremental unknowns
-        # --------------------------------------------------------------------
         if rebalance:
             dymaxn = dymax.copy()
             dymax, rebalanced, lastfailed = adjust(
                 dymax0,
                 dymaxn,
                 success=res.success,
                 n=res.niterations,
@@ -192,22 +219,21 @@
                 increase=increase,
                 decrease=decrease,
                 high=high,
                 low=low,
                 minlastfailed=minlastfailed,
                 nref=8,
             )
-        # --------------------------------------------------------------------
 
         # break step loop if Newton Iterations failed.
         if not res.success and not rebalanced:
             printinfo.errorfinal()
             break
 
-    return Res
+    return
 
 
 def adjust(
     x0,
     xn,
     success,
     n,
```

### Comparing `contique-0.1.9/test/test_archimedean_spiral.py` & `contique-1.0.0/tests/test_archimedean_spiral.py`

 * *Files identical despite different names*

### Comparing `contique-0.1.9/test/test_lituus_spiral.py` & `contique-1.0.0/tests/test_lituus_spiral.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     # numeric continuation
     Res = contique.solve(
         fun=fun,
         x0=x0,
         args=(a,),
         lpf0=lpf0,
-        control0=3,
+        control0=(2, 1),
         dxmax=0.2,
         dlpfmax=0.2,
         jacmode=3,
         jaceps=1e-4,
         maxsteps=500,
         maxcycles=4,
         maxiter=20,
```

### Comparing `contique-0.1.9/test/test_log_spiral.py` & `contique-1.0.0/tests/test_log_spiral.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     # numeric continuation
     Res = contique.solve(
         fun=fun,
         x0=x0,
         args=(a, k),
         lpf0=lpf0,
-        control0=3,
+        control0=(2, 1),
         dxmax=0.2,
         dlpfmax=0.2,
         jacmode=3,
         jaceps=1e-4,
         maxsteps=500,
         maxcycles=4,
         maxiter=20,
```

### Comparing `contique-0.1.9/test/test_sin_rebalance.py` & `contique-1.0.0/tests/test_sin_rebalance.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 import pytest
 
 import contique
 
 
 def fun(x, l, a, b):
-    return np.array([-(a+b*x[0]) * np.sin(x[0]) + l])
+    return np.array([-(a + b * x[0]) * np.sin(x[0]) + l])
 
 
 def test_sin_rebalance():
 
     # initial solution
     x0 = np.zeros(1)
     lpf0 = 0.0
@@ -31,15 +31,15 @@
         maxcycles=4,
         maxiter=8,
         tol=1e-10,
         overshoot=1.0,
         rebalance=True,
         increase=0.5,
         decrease=2,
-        high=10
+        high=10,
     )
 
     X = np.array([res.x for res in Res])
 
     plt.plot(X[:, 0], X[:, 1], "C0.-")
     plt.xlabel("$x_1$")
     plt.ylabel("$x_2$")
```

### Comparing `contique-0.1.9/test/test_sincos.py` & `contique-1.0.0/tests/test_archimedean_spiral_noargs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pytest
 
 import contique
 
 
-def fun(x, l, a, b):
-    return np.array([-a * np.sin(x[0]) + x[1] ** 2 + l, -b * np.cos(x[1]) * x[1] + l])
+def fun(x, l):
+    a = 1
+    r = a * l
+    return np.array([-x[0] + r * np.cos(l), -x[1] + r * np.sin(l)])
 
 
-def test_sincos():
+def test_archimedian_spiral_noargs():
 
     # initial solution
     x0 = np.zeros(2)
     lpf0 = 0.0
 
-    # additional function arguments
-    a, b = 1, 1
-
     # numeric continuation
     Res = contique.solve(
         fun=fun,
         x0=x0,
-        args=(a, b),
         lpf0=lpf0,
-        dxmax=0.1,
-        dlpfmax=0.1,
-        maxsteps=75,
+        dxmax=0.2,
+        dlpfmax=0.2,
+        maxsteps=500,
         maxcycles=4,
-        maxiter=20,
+        maxiter=8,
         tol=1e-10,
-        overshoot=1.0,
+        overshoot=1.05,
     )
 
     X = np.array([res.x for res in Res])
 
-    plt.plot(X[:, 0], X[:, 1], "C0.-")
+    plt.plot(X[:, 0], X[:, 1], "-")
     plt.xlabel("$x_1$")
     plt.ylabel("$x_2$")
+    plt.xlim(-15, 15)
+    plt.ylim(-15, 15)
     plt.plot([0], [0], "C0o", lw=3)
     plt.arrow(
         X[-2, 0],
         X[-2, 1],
         X[-1, 0] - X[-2, 0],
         X[-1, 1] - X[-2, 1],
-        head_width=0.075,
-        head_length=0.15,
+        head_width=1,
+        head_length=2,
         fc="C0",
         ec="C0",
     )
     plt.gca().set_aspect("equal")
-    plt.savefig("test_sincos.svg")
+    plt.savefig("test_archimedean_spiral_noargs.svg")
 
 
 if __name__ == "__main__":
-    test_sincos()
+    test_archimedian_spiral_noargs()
```


# Comparing `tmp/cvxportfolio-0.2.0.tar.gz` & `tmp/cvxportfolio-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxportfolio-0.2.0.tar", max compression
+gzip compressed data, was "cvxportfolio-0.3.0.tar", last modified: Fri May 12 05:21:23 2023, max compression
```

## Comparing `cvxportfolio-0.2.0.tar` & `cvxportfolio-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,39 @@
--rw-r--r--   0        0        0      599 2023-04-08 05:48:25.320984 cvxportfolio-0.2.0/LICENSE
--rw-r--r--   0        0        0     4079 2023-04-24 03:28:10.413934 cvxportfolio-0.2.0/README.md
--rw-r--r--   0        0        0     1015 2023-04-24 03:29:00.463719 cvxportfolio-0.2.0/cvxportfolio/__init__.py
--rw-r--r--   0        0        0     7051 2023-04-22 22:02:01.434393 cvxportfolio-0.2.0/cvxportfolio/constraints.py
--rw-r--r--   0        0        0    14977 2023-04-22 22:02:01.434783 cvxportfolio-0.2.0/cvxportfolio/costs.py
--rw-r--r--   0        0        0    16552 2023-04-24 03:15:29.788318 cvxportfolio-0.2.0/cvxportfolio/data.py
--rw-r--r--   0        0        0      893 2023-04-18 17:41:30.519984 cvxportfolio-0.2.0/cvxportfolio/errors.py
--rw-r--r--   0        0        0    12075 2023-04-19 19:02:58.141925 cvxportfolio-0.2.0/cvxportfolio/estimator.py
--rw-r--r--   0        0        0     6018 2023-04-22 05:27:54.567565 cvxportfolio-0.2.0/cvxportfolio/legacy.py
--rw-r--r--   0        0        0    27168 2023-04-24 03:03:00.921115 cvxportfolio-0.2.0/cvxportfolio/policies.py
--rw-r--r--   0        0        0    10377 2023-04-24 02:57:04.982404 cvxportfolio-0.2.0/cvxportfolio/result.py
--rw-r--r--   0        0        0     8679 2023-04-23 12:41:41.143567 cvxportfolio-0.2.0/cvxportfolio/returns.py
--rw-r--r--   0        0        0    22577 2023-04-23 12:25:43.855388 cvxportfolio-0.2.0/cvxportfolio/risks.py
--rw-r--r--   0        0        0    27831 2023-04-23 10:56:36.475351 cvxportfolio-0.2.0/cvxportfolio/simulator.py
--rw-r--r--   0        0        0      675 2023-04-24 03:28:51.326012 cvxportfolio-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4711 1970-01-01 00:00:00.000000 cvxportfolio-0.2.0/PKG-INFO
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-05-12 05:21:23.927908 cvxportfolio-0.3.0/
+-rw-r--r--   0 enzo       (501) staff       (20)      199 2023-04-08 05:48:25.000000 cvxportfolio-0.3.0/AUTHORS
+-rw-r--r--   0 enzo       (501) staff       (20)      599 2023-04-08 05:48:25.000000 cvxportfolio-0.3.0/LICENSE
+-rw-r--r--   0 enzo       (501) staff       (20)      329 2023-05-12 05:21:23.927585 cvxportfolio-0.3.0/PKG-INFO
+-rw-r--r--   0 enzo       (501) staff       (20)     3487 2023-05-12 03:58:00.000000 cvxportfolio-0.3.0/README.md
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-05-12 05:21:23.910446 cvxportfolio-0.3.0/cvxportfolio/
+-rw-r--r--   0 enzo       (501) staff       (20)      888 2023-05-12 05:21:20.000000 cvxportfolio-0.3.0/cvxportfolio/__init__.py
+-rw-r--r--   0 enzo       (501) staff       (20)     6972 2023-05-12 04:06:18.000000 cvxportfolio-0.3.0/cvxportfolio/constraints.py
+-rw-r--r--   0 enzo       (501) staff       (20)     9746 2023-05-12 05:19:45.000000 cvxportfolio-0.3.0/cvxportfolio/costs.py
+-rw-r--r--   0 enzo       (501) staff       (20)    19217 2023-05-11 16:35:10.000000 cvxportfolio-0.3.0/cvxportfolio/data.py
+-rw-r--r--   0 enzo       (501) staff       (20)     1004 2023-05-11 16:35:10.000000 cvxportfolio-0.3.0/cvxportfolio/errors.py
+-rw-r--r--   0 enzo       (501) staff       (20)    10204 2023-05-11 16:35:10.000000 cvxportfolio-0.3.0/cvxportfolio/estimator.py
+-rw-r--r--   0 enzo       (501) staff       (20)    19854 2023-05-11 19:03:54.000000 cvxportfolio-0.3.0/cvxportfolio/policies.py
+-rw-r--r--   0 enzo       (501) staff       (20)     5909 2023-05-12 05:13:01.000000 cvxportfolio-0.3.0/cvxportfolio/result.py
+-rw-r--r--   0 enzo       (501) staff       (20)    10807 2023-05-12 05:05:30.000000 cvxportfolio-0.3.0/cvxportfolio/returns.py
+-rw-r--r--   0 enzo       (501) staff       (20)    18691 2023-05-12 05:01:19.000000 cvxportfolio-0.3.0/cvxportfolio/risks.py
+-rw-r--r--   0 enzo       (501) staff       (20)    24580 2023-05-12 04:34:39.000000 cvxportfolio-0.3.0/cvxportfolio/simulator.py
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-05-12 05:21:23.926979 cvxportfolio-0.3.0/cvxportfolio/tests/
+-rw-r--r--   0 enzo       (501) staff       (20)        0 2023-05-12 05:21:20.000000 cvxportfolio-0.3.0/cvxportfolio/tests/__init__.py
+-rw-r--r--   0 enzo       (501) staff       (20)     1626 2023-05-11 16:35:10.000000 cvxportfolio-0.3.0/cvxportfolio/tests/base.py
+-rw-r--r--   0 enzo       (501) staff       (20)   156730 2023-05-11 16:35:10.000000 cvxportfolio-0.3.0/cvxportfolio/tests/returns.csv
+-rw-r--r--   0 enzo       (501) staff       (20)   149356 2023-05-11 16:35:10.000000 cvxportfolio-0.3.0/cvxportfolio/tests/sigmas.csv
+-rw-r--r--   0 enzo       (501) staff       (20)     8855 2023-05-11 16:35:10.000000 cvxportfolio-0.3.0/cvxportfolio/tests/test_constraints.py
+-rw-r--r--   0 enzo       (501) staff       (20)     8306 2023-05-11 19:06:55.000000 cvxportfolio-0.3.0/cvxportfolio/tests/test_costs.py
+-rw-r--r--   0 enzo       (501) staff       (20)    10329 2023-05-11 16:35:10.000000 cvxportfolio-0.3.0/cvxportfolio/tests/test_data.py
+-rw-r--r--   0 enzo       (501) staff       (20)     6657 2023-05-11 16:35:10.000000 cvxportfolio-0.3.0/cvxportfolio/tests/test_estimator.py
+-rw-r--r--   0 enzo       (501) staff       (20)    21796 2023-05-11 19:07:12.000000 cvxportfolio-0.3.0/cvxportfolio/tests/test_policies.py
+-rw-r--r--   0 enzo       (501) staff       (20)     4349 2023-05-11 19:07:22.000000 cvxportfolio-0.3.0/cvxportfolio/tests/test_returns.py
+-rw-r--r--   0 enzo       (501) staff       (20)     8964 2023-05-11 19:07:41.000000 cvxportfolio-0.3.0/cvxportfolio/tests/test_risks.py
+-rw-r--r--   0 enzo       (501) staff       (20)    10577 2023-05-11 16:35:10.000000 cvxportfolio-0.3.0/cvxportfolio/tests/test_simulator.py
+-rw-r--r--   0 enzo       (501) staff       (20)   116620 2023-05-11 16:35:10.000000 cvxportfolio-0.3.0/cvxportfolio/tests/volumes.csv
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-05-12 05:21:23.913031 cvxportfolio-0.3.0/cvxportfolio.egg-info/
+-rw-r--r--   0 enzo       (501) staff       (20)      329 2023-05-12 05:21:23.000000 cvxportfolio-0.3.0/cvxportfolio.egg-info/PKG-INFO
+-rw-r--r--   0 enzo       (501) staff       (20)      910 2023-05-12 05:21:23.000000 cvxportfolio-0.3.0/cvxportfolio.egg-info/SOURCES.txt
+-rw-r--r--   0 enzo       (501) staff       (20)        1 2023-05-12 05:21:23.000000 cvxportfolio-0.3.0/cvxportfolio.egg-info/dependency_links.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       64 2023-05-12 05:21:23.000000 cvxportfolio-0.3.0/cvxportfolio.egg-info/requires.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       13 2023-05-12 05:21:23.000000 cvxportfolio-0.3.0/cvxportfolio.egg-info/top_level.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       38 2023-05-12 05:21:23.927992 cvxportfolio-0.3.0/setup.cfg
+-rw-r--r--   0 enzo       (501) staff       (20)      788 2023-05-12 05:21:20.000000 cvxportfolio-0.3.0/setup.py
```

### Comparing `cvxportfolio-0.2.0/LICENSE` & `cvxportfolio-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.2.0/README.md` & `cvxportfolio-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,100 +1,91 @@
 # Cvxportfolio
 
 [![CVXportfolio on PyPI](https://img.shields.io/pypi/v/cvxportfolio.svg)](https://pypi.org/project/cvxportfolio/)
 [![Downloads](https://static.pepy.tech/personalized-badge/cvxportfolio?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/cvxportfolio)
 [![Documentation Status](https://readthedocs.org/projects/cvxportfolio/badge/?version=latest)](https://cvxportfolio.readthedocs.io/en/latest/?badge=latest)
 
 
-**WORK IN PROGRESS. Cvxportfolio is currently under development. We will freeze the user interface by end of 2023Q2 and release the first stable version by end of 2023Q3. The script `hello_world.py` now runs with the new interface (see below).**
+**WORK IN PROGRESS. Cvxportfolio is currently under development. We will freeze the user interface by end of 2023Q2 and release the first stable version by end of 2023Q3.**
 
 
 `cvxportfolio` is a python library for portfolio optimization and simulation
-based on the book [Multi-Period Trading via Convex Optimization](https://web.stanford.edu/~boyd/papers/pdf/cvx_portfolio.pdf).
-It is written in Python, its main dependencies are [`cvxpy`](https://github.com/cvxgrp/cvxpy)
-and [`pandas`](https://github.com/pandas-dev/pandas). 
+based on the book [Multi-Period Trading via Convex Optimization](https://web.stanford.edu/~boyd/papers/pdf/cvx_portfolio.pdf)
+(also [available in print](https://www.amazon.com/Multi-Period-Trading-Convex-Optimization-Foundations/dp/1680833286/)).
 
 The documentation of the package is at [cvxportfolio.readthedocs.io](https://cvxportfolio.readthedocs.io/en/latest/).
 
 
 Installation
 ------------
 
 ```
-pip install cvxportfolio
+pip install -U cvxportfolio
 ```
 
-Testing
+Testing locally
 ------------
-
-To test it locally, for example, you can set up the development environment with [`poetry`](https://python-poetry.org/) and run [`pytest`](https://pytest.org/). 
+We ship our unit test suite with the pip package. After installing you can test in you local environment by
 
 ```
-git clone https://github.com/cvxgrp/cvxportfolio.git
-cd cvxportfolio
-poetry install
-poetry run pytest --cov
+python -m unittest discover cvxportfolio
 ```
 
 
 Example
 ------------
 To get a sneak preview of `cvxportfolio` you may try the following code. This is available in `examples/hello_world.py` and runs 
-with `cvxportfolio` >= 0.2.0
+with `cvxportfolio >= 0.3.0`
 
 
 ```python
-import cvxportfolio as cp
+import cvxportfolio as cvx
 import matplotlib.pyplot as plt
 
-# define a portfolio optimization policy
-# with rolling window mean (~10 yrs) returns
-# with forecast error risk on returns (see the book)
-# rolling window mean (~10 yrs) covariance
-# and forecast error risk on covariance (see the book)
-policy = cp.SinglePeriodOptimization(objective = 
-        cp.RollingWindowReturnsForecast(2500) -
-        cp.RollingWindowReturnsForecastErrorRisk(2500) -
-        5 * cp.RollingWindowFullCovariance(2500, forecast_error_kappa = 0.25), 
-        constraints = [cp.LeverageLimit(3)]
-        )
-        
-# define a market simulator, which downloads stock market data and stores it locally
-# in ~/cvxportfolio/        
-simulator = cp.MarketSimulator(["AMZN", "AAPL", "MSFT", "GOOGL", "TSLA", "GM"])
+objective = cvx.ReturnsForecast() - 3 * (cvx.FullCovariance() + \
+	0.05 * cvx.RiskForecastError()) - cvx.TransactionCost()
+constraints = [cvx.LeverageLimit(3)]
+
+policy = cvx.MultiPeriodOptimization(objective, constraints, planning_horizon=2)
+
+simulator = cvx.MarketSimulator(['AAPL', 'AMZN', 'TSLA', 'GM', 'CVX', 'NKE'])
+
+result = simulator.backtest(policy, start_time='2020-01-01')
 
-# perform a backtest (by default it starts with 1E6 USD cash)
-backtest = cp.BackTest(policy, simulator, '2023-01-01', '2023-04-21')
+print(result)
 
 # plot value of the portfolio in time
-backtest.v.plot(figsize=(12, 5), label='Single Period Optimization')
+result.v.plot(figsize=(12, 5), label='Multi Period Optimization')
 plt.ylabel('USD')
 plt.title('Total value of the portfolio in time')
 plt.show()
 
 # plot weights of the (non-cash) assets for the SPO policy
-backtest.w.iloc[:, :-1].plot()
+result.w.iloc[:, :-1].plot()
 plt.title('Weights of the portfolio in time')
 plt.show()
 
-print('total tcost', backtest.tcost.sum())
-print('total borrow cost', backtest.hcost_stocks.sum())
-print('total cash return + cost', backtest.hcost_cash.sum())
+print('\ntotal tcost ($)', result.tcost.sum())
+print('total borrow cost ($)', result.hcost_stocks.sum())
+print('total cash return + cost ($)', result.hcost_cash.sum())
 
 ```
 
-(*The other examples may currently have problems as we are changing various bits and pieces of `cvxportfolio`.*)
+Examples from the book
+--------------------
+In branch [0.0.X](https://github.com/cvxgrp/cvxportfolio/tree/0.0.X) you can find the original material used to generate plots
+and results in the book. 
 
 
 Academic
 ------------
 
 If you use `cvxportfolio` in your academic work please cite our book:
 ```
-@article{BBDKKNS:17,
+@book{BBDKKNS:17,
     author       = {S. Boyd and E. Busseti and S. Diamond and R. Kahn and K. Koh and P. Nystrup and J. Speth},
     title        = {Multi-Period Trading via Convex Optimization},
     journal      = {Foundations and Trends in Optimization},
     year         = {2017},
     month        = {August},
     volume       = {3},
     number       = {1},
```

### Comparing `cvxportfolio-0.2.0/cvxportfolio/__init__.py` & `cvxportfolio-0.3.0/cvxportfolio/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-# Copyright 2016-2020 Stephen Boyd, Enzo Busseti, Steven Diamond, BlackRock Inc.
-# Copyright 2023- The Cvxportfolio Contributors
+# Copyright 2016 Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.2.0"
-from .data import FredRate, Yfinance
-from .simulator import MarketSimulator
+__version__ = "0.3.0"
+from .data import *
+from .simulator import *
 from .result import *
 from .policies import *
 from .constraints import *
-from .costs import TcostModel, HcostModel
+from .costs import *
 from .returns import *
 from .estimator import DataEstimator
 from .risks import *
 from .returns import *
-from .legacy import *
```

### Comparing `cvxportfolio-0.2.0/cvxportfolio/constraints.py` & `cvxportfolio-0.3.0/cvxportfolio/constraints.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# Copyright 2016-2020 Stephen Boyd, Enzo Busseti, Steven Diamond, BlackRock Inc.
-# Copyright 2023- The Cvxportfolio Contributors
+# Copyright 2016 Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,15 +15,14 @@
 and MultiPeriodOptimization policies, or other Cvxpy-based policies.
 """
 
 
 import cvxpy as cvx
 import numpy as np
 
-# from .utils import values_in_time
 from .estimator import CvxpyExpressionEstimator, ParameterEstimator
 
 
 __all__ = [
     "LongOnly",
     "LeverageLimit",
     "LongCash",
@@ -36,28 +34,14 @@
     "FactorMinLimit",
     "FixedFactorLoading",
 ]
 
 
 class BaseConstraint(CvxpyExpressionEstimator):
     """Base cvxpy constraint class."""
-    
-    #INITIALIZED = False # used to interface w/ old cvxportfolio
-
-    # interface to old cvxportfolio
-    def weight_expr(self, t, w_plus, z, v):
-        #if not self.INITIALIZED:
-        self.pre_evaluation(None, None, t, None)
-        self.legacy_expression = self.compile_to_cvxpy(w_plus, z, v)
-        #self.INITIALIZED = True
-        self.values_in_time(t, None, None, None, None)
-        if hasattr(self.legacy_expression, "__iter__"):
-            return self.legacy_expression
-        else:
-            return [self.legacy_expression]
 
 
 class BaseTradeConstraint(BaseConstraint):
     """Base class for constraints that operate on trades."""
 
     pass
 
@@ -71,99 +55,112 @@
     """
 
     pass
 
 
 class ParticipationRateLimit(BaseTradeConstraint):
     """A limit on maximum trades size as a fraction of market volumes.
+    
 
-    Attributes:
-        self.volumes (ParameterEstimator): ParameterEstimator with point-in-time market volumes estimations
-        self.max_fraction_of_volumes (ParameterEstimator): ParameterEstimator with point-in-time,
-             and also possibly per-stock, requirements of maximum participation rate
-
+    :param volumes: per-stock and per-day market volume estimates, or constant in time
+    :type volumes: pd.Series or pd.DataFrame
+    :param max_fraction_of_volumes: max fraction of market volumes that we're allowed to trade
+    :type max_fraction_of_volumes: float, pd.Series, pd.DataFrame
     """
 
     def __init__(self, volumes, max_fraction_of_volumes=0.05):
         self.volumes = ParameterEstimator(volumes)
         self.max_participation_rate = ParameterEstimator(
             max_fraction_of_volumes)
+        self.portfolio_value = cvx.Parameter(nonneg=True)
 
-    def compile_to_cvxpy(self, w_plus, z, portfolio_value):
+    def values_in_time(self, current_portfolio_value, **kwargs):
+        self.portfolio_value.value = current_portfolio_value
+        super().values_in_time(current_portfolio_value=current_portfolio_value, **kwargs)
+        
+    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
-        return cvx.multiply(cvx.abs(z[:-1]), portfolio_value) <= cvx.multiply(
+        return cvx.multiply(cvx.abs(z[:-1]), self.portfolio_value) <= cvx.multiply(
             self.volumes, self.max_participation_rate
         )
 
 
 class LongOnly(BaseWeightConstraint):
-    """A long only constraint."""
+    """A long only constraint.
+    
+    Imposes that at each point in time the post-trade
+    weights are non-negative.
+    """
 
-    def compile_to_cvxpy(self, w_plus, z, portfolio_value):
+    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return w_plus[:-1] >= 0
 
 
 class LeverageLimit(BaseWeightConstraint):
     """A limit on leverage.
+    
+    Leverage is defined as the :math:`\ell_1` norm of non-cash
+    post-trade weights. Here we require that it is smaller than
+    a given value
 
-    Attributes:
-      limit: A (time) series or scalar giving the leverage limit.
+    :param limit: constant or varying in time leverage limit
+    :type limit: float or pd.Series
     """
 
     def __init__(self, limit):
         self.limit = ParameterEstimator(limit)
 
-    def compile_to_cvxpy(self, w_plus, z, portfolio_value):
+    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return cvx.norm(w_plus[:-1], 1) <= self.limit
 
 
 class LongCash(BaseWeightConstraint):
     """Requires that cash be non-negative."""
 
-    def compile_to_cvxpy(self, w_plus, z, portfolio_value):
+    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return w_plus[-1] >= 0
 
 
 class DollarNeutral(BaseWeightConstraint):
     """Long-short dollar neutral strategy."""
 
-    def compile_to_cvxpy(self, w_plus, z, portfolio_value):
+    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return w_plus[-1] == 1
 
 
 class MaxWeights(BaseWeightConstraint):
     """A max limit on weights.
 
     Attributes:
       limit: A series or number giving the weights limit.
     """
 
     def __init__(self, limit):
         self.limit = ParameterEstimator(limit)
 
-    def compile_to_cvxpy(self, w_plus, z, portfolio_value):
+    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return w_plus[:-1] <= self.limit
 
 
 class MinWeights(BaseWeightConstraint):
     """A min limit on weights.
 
     Attributes:
       limit: A series or number giving the weights limit.
     """
 
     def __init__(self, limit):
         self.limit = ParameterEstimator(limit)
 
-    def compile_to_cvxpy(self, w_plus, z, portfolio_value):
+    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return w_plus[:-1] >= self.limit
 
 
 class FactorMaxLimit(BaseWeightConstraint):
     """A max limit on portfolio-wide factor (e.g. beta) exposure.
 
@@ -173,15 +170,15 @@
         limit: A series of list or a single list giving the factor limits
     """
 
     def __init__(self, factor_exposure, limit):
         self.factor_exposure = ParameterEstimator(factor_exposure)
         self.limit = ParameterEstimator(limit)
 
-    def compile_to_cvxpy(self, w_plus, z, portfolio_value):
+    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return self.factor_exposure.T @ w_plus[:-1] <= self.limit
 
 
 class FactorMinLimit(BaseWeightConstraint):
     """A min limit on portfolio-wide factor (e.g. beta) exposure.
 
@@ -191,15 +188,15 @@
         limit: A series of list or a single list giving the factor limits
     """
 
     def __init__(self, factor_exposure, limit):
         self.factor_exposure = ParameterEstimator(factor_exposure)
         self.limit = ParameterEstimator(limit)
 
-    def compile_to_cvxpy(self, w_plus, z, portfolio_value):
+    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return self.factor_exposure.T @ w_plus[:-1] >= self.limit
 
 
 class FixedFactorLoading(BaseWeightConstraint):
     """A constraint to fix portfolio loadings to a set of factors.
 
@@ -211,10 +208,10 @@
         target: A series or number giving the targeted factor loading
     """
 
     def __init__(self, factor_exposure, target):
         self.factor_exposure = ParameterEstimator(factor_exposure)
         self.target = ParameterEstimator(target)
 
-    def compile_to_cvxpy(self, w_plus, z, portfolio_value):
+    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return self.factor_exposure.T @ w_plus[:-1] == self.target
```

### Comparing `cvxportfolio-0.2.0/cvxportfolio/data.py` & `cvxportfolio-0.3.0/cvxportfolio/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023- The Cvxportfolio Contributors
+# Copyright 2016 Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -17,16 +17,17 @@
 import pandas as pd
 import numpy as np
 import pandas_datareader
 import sqlite3
 
 from .estimator import DataEstimator
 
-__all__ = ["TimeSeries"]
+__all__ = ["YfinanceTimeSeries", "FredTimeSeries", "FredRateTimeSeries", "BASE_LOCATION"]
 
+BASE_LOCATION = Path.home() / "cvxportfolio_data"
 
 class BaseData:
     """Base class for Cvxportfolio database interface.
 
     Provides a back-end independent way to load and store
     pandas Series and DataFrames where the first index is a
     pandas Timestamp (or numpy datetime64). It also provides
@@ -145,29 +146,36 @@
         Returns:
             updated (pandas.DataFrame): updated DataFrame for the symbol
         """
         if (current is None) or (len(current) < overlap):
             updated = yf.download(symbol, progress=False, **kwargs)
             return cls.internal_process(updated)
         else:
-            new = yf.download(symbol, start=current.index[-overlap], **kwargs)
+            if (pd.Timestamp.today() - current.index[-1]) < pd.Timedelta('5d'):
+                return current
+            new = yf.download(symbol, progress=False, start=current.index[-overlap], **kwargs)
             new = cls.internal_process(new)
             return pd.concat([current.iloc[:-overlap], new])
 
     @staticmethod
     def preload(data):
         """Prepare data for use by Cvxportfolio.
 
         We drop the 'Volume' column expressed in number of stocks
         and replace it with 'ValueVolume' which is an estimate
         of the (e.g., US dollar) value of the volume exchanged
         on the day.
         """
         data["ValueVolume"] = data["Volume"] * data["Open"]
         del data["Volume"]
+        # remove infty values
+        data.iloc[:, :] = np.nan_to_num(data.values, copy=True, nan=np.nan, posinf=np.nan, neginf=np.nan)
+        # remove extreme values
+        data.loc[data["Return"] < -.99, "Return"] = np.nan
+        data.loc[data["Return"] > .99, "Return"] = np.nan
         return data
 
 
 class BaseDataStore(BaseData):
     """Base class for data storage systems.
 
     Attributes:
@@ -182,15 +190,15 @@
 
     Args:
         location (pathlib.Path or None): pathlib.Path base location of the databases
             directory or, if None, use ":memory:" for storing in RAM instead. Default
             is ~/cvxportfolio/
     """
 
-    def __init__(self, base_location=Path.home() / "cvxportfolio"):
+    def __init__(self, base_location=BASE_LOCATION):
         """Initialize sqlite connection and if necessary create database."""
         self.base_location = base_location
 
     def __open__(self):
         """Open database connection."""
         if self.base_location is None:
             self.connection = sqlite3.connect(":memory:")
@@ -266,29 +274,65 @@
                 multiindex = [tmp.index.name] + multiindex
                 tmp = tmp.reset_index().set_index(multiindex)
             return tmp.iloc[:, 0] if tmp.shape[1] == 1 else tmp
         except pd.errors.DatabaseError:
             return None
 
 
+
+class PickleStore(BaseDataStore):
+    """Pickle data store for pandas Series and DataFrames.
+
+    Args:
+        base_location (pathlib.Path): filesystem directory where to store files.
+
+    """
+
+    # base_location = BASE_LOCATION
+
+    @property
+    def location(self):
+        return self.base_location / self.__class__.__name__
+
+    def __init__(self, base_location=BASE_LOCATION):
+        self.base_location = base_location
+
+    def __create_if_not_existent(self):
+        if not self.location.is_dir():
+            self.location.mkdir(parents=True)
+            print(f"Created folder at {self.location}")
+
+    def load_raw(self, symbol, **kwargs):
+        """Load raw data from local store."""
+        try:
+            return pd.read_pickle(self.location / f"{symbol}.pickle")
+        except FileNotFoundError:
+            return None
+
+    def store(self, symbol, data, **kwargs):
+        """Store data locally."""
+        self.__create_if_not_existent()
+        data.to_pickle(self.location / f"{symbol}.pickle")
+        
+        
 class LocalDataStore(BaseDataStore):
     """Local data store for pandas Series and DataFrames.
 
     Args:
         base_location (pathlib.Path): filesystem directory where to store files.
 
     """
 
-    base_location = Path.home() / "cvxportfolio"
+    # base_location = Path.home() / "cvxportfolio"
 
     @property
     def location(self):
         return self.base_location / self.__class__.__name__
 
-    def __init__(self, base_location=Path.home() / "cvxportfolio"):
+    def __init__(self, base_location=BASE_LOCATION):
         self.base_location = base_location
 
     def __create_if_not_existent(self):
         if not self.location.is_dir():
             self.location.mkdir(parents=True)
             print(f"Created folder at {self.location}")
 
@@ -387,21 +431,48 @@
         """Update data for symbol and load it."""
         return super().update_and_load(symbol)
 
 
 class FredRate(FredBase, RateBase, SqliteDataStore):
     """Load and store FRED rates like DFF."""
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    pass
 
-    def update_and_load(self, symbol):
-        """Update data for symbol and load it."""
-        return super().update_and_load(symbol)
 
+class YfinanceTimeSeries(DataEstimator, YfinanceBase, PickleStore):
+    
+    def __init__(self, symbol, use_last_available_time=False, base_location=None):
+        self.symbol = symbol
+        self.base_location = base_location
+        self.use_last_available_time = use_last_available_time
+
+    def pre_evaluation(self, *args, **kwargs):
+        self.data = self.update_and_load(self.symbol)
+        
+        
+class FredTimeSeries(DataEstimator, FredBase, PickleStore):
+    
+    def __init__(self, symbol, use_last_available_time=False, base_location=None):
+        self.symbol = symbol
+        self.base_location = base_location
+        self.use_last_available_time = use_last_available_time
+
+    def pre_evaluation(self, *args, **kwargs):
+        self.data = self.update_and_load(self.symbol)
+    
+class FredRateTimeSeries(DataEstimator, FredBase, RateBase, PickleStore):
+    
+    def __init__(self, symbol, use_last_available_time=False, base_location=None):
+        self.symbol = symbol
+        self.base_location = base_location
+        self.use_last_available_time = use_last_available_time
+
+    def pre_evaluation(self, *args, **kwargs):
+        self.data = self.update_and_load(self.symbol)    
+        
 
 class TimeSeries(DataEstimator):
     """Class for time series data managed by Cvxportfolio.
 
     Args:
         symbol (str): name of the time series, such as 'AAPL',
             '^VIX', or 'DFF'.
@@ -421,15 +492,15 @@
 
     """
 
     def __init__(
         self,
         symbol,
         source="yahoo",
-        storage="csv",
+        storage="pickle",
         use_last_available_time=False,
         base_location=None,
     ):
         self.symbol = symbol
         if isinstance(source, str) and source == "yahoo":
             source = YfinanceBase
         if isinstance(source, str) and source == "fred":
@@ -442,14 +513,16 @@
             cls.__name__ + "With" + source.__name__, (cls, source), {}
         )
 
         if isinstance(storage, str) and storage == "sqlite":
             storage = SqliteDataStore
         if isinstance(storage, str) and storage == "csv":
             storage = LocalDataStore
+        if isinstance(storage, str) and storage == "pickle":
+            storage = PickleStore
 
         cls = self.__class__
         self.__class__ = cls.__class__(
             cls.__name__ + "With" + storage.__name__, (cls, storage), {}
         )
 
         self.base_location = base_location
```

### Comparing `cvxportfolio-0.2.0/cvxportfolio/errors.py` & `cvxportfolio-0.3.0/cvxportfolio/errors.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023- The Cvxportfolio Contributors
+# Copyright 2016 Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -19,11 +19,15 @@
     pass
 
 
 class MissingValuesError(DataError):
     """Cvxportfolio tried to access numpy.nan values."""
 
     pass
+    
+class ForeCastError(DataError):
+    """Forecast procedure failed."""
+    pass
 
 
 class PortfolioOptimizationError(Exception):
     """Errors with portfolio optimization problems."""
```

### Comparing `cvxportfolio-0.2.0/cvxportfolio/estimator.py` & `cvxportfolio-0.3.0/cvxportfolio/estimator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023- The Cvxportfolio Contributors
+# Copyright 2016 Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -31,103 +31,67 @@
     the `super()` corresponding method. It can make sense to call it before
     some logic, after, or not calling it at all. Also, any subclass of this that uses
     logic defined here should be careful to put estimator subclasses at the class
     attribute level, so that the two methods defined here get called recursively
     on them.
     """
 
-    def pre_evaluation(self, returns, volumes, start_time, end_time, **kwargs):
-        """Run computation on estimators before the simulation with full prescience.
+    def pre_evaluation(self, universe, backtest_times):
+        """Initialize estimator and its sub-estimators.
 
-        This function is called by Simulator classes before the
-        start of a backtest with the full dataset available to the
-        simulator. This is useful for estimators such as pandas.rolling_mean
-        which are faster (and easier) when vectorized rather than called separately
-        at each point in time.
-
-        It should be used very carefully, if you
-        are not sure do not implement this method. You can use
-        values_in_time to build lazily whatever you would
-        build here beforehand. If you do implement this, double
-        check that at each point in time only past data
-        (with respect to that point) is used and not future data.
-
-        Args:
-            returns (pandas.DataFrame): market returns.
-            volumes (pandas.DataFrame): market volumes.
-            start_time (pandas.Timestamp): start time of the backtest.
-            end_time (pandas.Timestamp): end time of the backtest.
-            **kwargs: extra arguments for future development.
+        :param universe: names of assets to be traded 
+        :type universe: pandas.Index
+        :param backtest_times: times at which the estimator will be evaluated
+        :type backtest_time: pandas.DatetimeIndex
         """
         for _, subestimator in self.__dict__.items():
             if hasattr(subestimator, "pre_evaluation"):
-                subestimator.pre_evaluation(
-                    returns, volumes, start_time, end_time, **kwargs)
+                subestimator.pre_evaluation(universe, backtest_times)
 
-    def values_in_time(
-            self,
-            t,
-            current_weights,
-            current_portfolio_value,
-            past_returns,
-            past_volumes,
-            **kwargs):
+    def values_in_time(self, **kwargs):
         """Evaluates estimator at a point in time recursively on its sub-estimators.
 
         This function is called by Simulator classes on Policy classes
         returning the current trades list. Policy classes, if
         they contain internal estimators, should declare them as attributes
         and call this base function (via `super()`) before
         they do their internal computation. CvxpyExpression estimators
         should instead define this method to update their Cvxpy parameters.
-
-        Args:
-            t (pd.TimeStamp): point in time of the simulation.
-            current_weights (pd.Series): current portfolio weights.
-            current_portfolio_value (float): current total value of the portfolio.
-            past_returns (pd.DataFrame): view of the market returns up to today (i.e., the
-                last row are equal to today's open prices divided by yesterday's, minus 1).
-            past_volumes (pd.DataFrame): view of the market volumes up to yesterday's.
-            kwargs (dict): extra arguments for future development.
+        
+        Once we finalize the interface all parameters will be listed here.
         """
         for _, subestimator in self.__dict__.items():
             if hasattr(subestimator, "values_in_time"):
-                subestimator.values_in_time(
-                    t,
-                    current_weights,
-                    current_portfolio_value,
-                    past_returns,
-                    past_volumes,
-                    **kwargs)
+                subestimator.values_in_time(**kwargs)
 
 
 class CvxpyExpressionEstimator(Estimator):
     """Base class for estimators that are Cvxpy expressions."""
 
-    def compile_to_cvxpy(self, w_plus, z, portfolio_value):
+    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Compile term to cvxpy expression.
 
         This is called by a Policy class on its terms before the start of the backtest
         to compile its Cvxpy problem. If the Policy changes in time
         this is called at every time step.
 
         It can either return a scalar expression, in the case of objective terms,
         or a list of cvxpy constraints, in the case of constraints.
 
         In MultiPeriodOptimization policies this is called separately
         for costs and constraints at different look-ahead steps with
         the corresponding w_plus and z.
-
-        Args:
-            w_plus (cvxpy.Variable): post-trade allocation weights vector
-            z (cvxpy.Variable): trades weight vector
-            portfolio_value (cvxpy.Parameter): scalar Parameter that holds the value of the portfolio
-
-        Returns:
-            cvxpy.Expression
+        
+        
+        :param w_plus: post-trade weights 
+        :type w_plus: cvxpy.Variable
+        :param z: trade weights 
+        :type z: cvxpy.Variable
+        :param w_plus_minus_w_bm: post-trade weights minus benchmark weights 
+        :type w_plus_minus_w_bm: cvxpy.Variable
         """
         raise NotImplementedError
 
 
 class DataEstimator(Estimator):
     """Estimator of point-in-time values from internal `self.data`.
 
@@ -147,17 +111,18 @@
         use_last_available_time (bool): if the pandas index exists
             and is a pandas.DateTimeIndex you can instruct self.values_in_time
             to retrieve the last available value at time t by setting
             this to True. Default is False.
 
     """
 
-    def __init__(self, data, use_last_available_time=False):
+    def __init__(self, data, use_last_available_time=False, allow_nans=False):
         self.data = data
         self.use_last_available_time = use_last_available_time
+        self.allow_nans = allow_nans
 
     def value_checker(self, result):
         """Ensure that only scalars or arrays without np.nan are returned.
 
         Args:
             result (int, float, or np.array): data produced by self.values_in_time
 
@@ -166,23 +131,23 @@
 
         Raises:
             cvxportfolio.MissingValuesError: if np.nan's are present in result
             cvxportfolio.DataError: if data is not in the right form
         """
 
         if np.isscalar(result):
-            if np.isnan(result):
+            if np.isnan(result) and not self.allow_nans:
                 raise MissingValuesError(
                     f"{self.__class__.__name__}.values_in_time result is a np.nan scalar."
                 )
             else:
                 return result
 
         if isinstance(result, np.ndarray):
-            if np.any(np.isnan(result)):
+            if np.any(np.isnan(result)) and not self.allow_nans:
                 raise MissingValuesError(
                     f"{self.__class__.__name__}.values_in_time result is an array with np.nan's."
                 )
             else:
                 return result
 
         raise DataError(
@@ -265,35 +230,25 @@
         parameter (cvxpy.Parameter): the parameter object to use with cvxpy
             expressions
     Args:
         same as cvxportfolio.DataEstimator
 
     """
 
-    def __init__(
-        self,
-        data,
-        positive_semi_definite=False,
-        non_negative=False,
-        use_last_available_time=False,
-    ):
+    def __init__(self, data, positive_semi_definite=False, non_negative=False, use_last_available_time=False, allow_nans=False):
         self.positive_semi_definite = positive_semi_definite
         self.non_negative = non_negative
         self.use_last_available_time = use_last_available_time
         self.data = data
+        self.allow_nans = allow_nans
         # super(DataEstimator).__init__(data, use_last_available_time)
 
-    def pre_evaluation(self, returns, volumes, start_time, end_time, **kwargs):
+    def pre_evaluation(self, universe, backtest_times):
         """Use the start time of the simulation to initialize the Parameter."""
-        super().pre_evaluation(returns, volumes, start_time, end_time, **kwargs)
-        value = super().values_in_time(start_time, None, None, None, None)
-        super().__init__(
-            value.shape if hasattr(value, "shape") else (),
-            PSD=self.positive_semi_definite,
-            nonneg=self.non_negative,
-        )
-        # self.parameter = self
-        # self.parameter = cvxpy.Parameter(value.shape if hasattr(value, 'shape') else (), PSD=self.positive_semi_definite, nonneg=self.non_negative)
+        super().pre_evaluation(universe, backtest_times)
+        value = super().values_in_time(t=backtest_times[0])
+        super().__init__(value.shape if hasattr(value, "shape") else (), 
+            PSD=self.positive_semi_definite, nonneg=self.non_negative)
 
-    def values_in_time(self, t, *args, **kwargs):
+    def values_in_time(self, t, **kwargs):
         """Update Cvxpy Parameter value."""
-        self.value = super().values_in_time(t, *args, **kwargs)
+        self.value = super().values_in_time(t=t, **kwargs)
```

### Comparing `cvxportfolio-0.2.0/cvxportfolio/simulator.py` & `cvxportfolio-0.3.0/cvxportfolio/simulator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# Copyright 2016-2020 Stephen Boyd, Enzo Busseti, Steven Diamond, BlackRock Inc.
-# Copyright 2023- The Cvxportfolio Contributors
+# Copyright 2016 Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -18,113 +17,118 @@
 In financial jargon this is called *backtesting*.
 """
 
 import copy
 import logging
 import time
 from pathlib import Path
+from multiprocessing import Pool
+# from multiprocess import Pool
 
-
-import multiprocess
+# import multiprocess
 import numpy as np
 import pandas as pd
 import cvxpy as cvx
 
-from .result import SimulationResult
 from .costs import BaseCost
-from .data import FredRate, Yfinance, TimeSeries
-from .returns import MultipleReturnsForecasts, ReturnsForecast
+from .data import FredRateTimeSeries, YfinanceTimeSeries, BASE_LOCATION
+from .returns import ReturnsForecast
 from .estimator import Estimator, DataEstimator
+from .result import BacktestResult
+
+__all__ = ['MarketSimulator']
+
 
+def parallel_worker(policy, simulator, start_time, end_time, h):
+
+    return simulator._single_backtest(policy, start_time, end_time, h)
+    
 
 class MarketSimulator(Estimator):
     """This class implements a simulator of market performance for trading strategies.
 
     We strive to make the parameters here as accurate as possible. The following is
     accurate as of 2023 using numbers obtained on the public website of a
-    [large US-based broker](https://www.interactivebrokers.com/).
-
-
-    Args:
+    `large US-based broker <https://www.interactivebrokers.com/>`_.
 
-        universe (list): list of [Yahoo Finance](https://finance.yahoo.com/) tickers on which to
-            simulate performance of the trading strategy. If left unspecified you should at least
-            pass `returns` and `volumes`. If you define a different market data access interface
-            (look in cvxportfolio.data for how to do it) you should pass instead
-            the symbol names for that data provider. Default is empty list.
 
-        returns (pandas.DataFrame): historical open-to-open returns. Default is None, it is ignored
-            if universe is specified.
-
-        volumes (pandas.DataFrame): historical market volumes expressed in value (e.g., US dollars).
+    :param universe: list of `Yahoo Finance <https://finance.yahoo.com/>`_ tickers on which to
+        simulate performance of the trading strategy. If left unspecified you should at least
+        pass `returns` and `volumes`. If you define a different market data access interface
+        (look in `cvxportfolio.data` for how to do it) you should pass instead
+        the symbol names for that data provider. Default is empty list.
+    :type universe: list or None
+    :param returns: historical open-to-open returns. Default is None, it is ignored
+        if universe is specified.
+    :type returns: pandas.DataFrame 
+    :param volumes: historical market volumes expressed in value (e.g., US dollars).
             Default is None, it is ignored if universe is specified.
-
-        prices (pandas.DataFrame): historical open prices. Default is None, it is ignored
-            if universe is specified. These are used to round the trades to integer number of stocks
-            if round_trades is True, and compute per-share transaction costs (if `per_share_fixed_cost`
-            is greater than zero).
-
-        spreads (pandas.DataFrame): historical bid-ask spreads expressed as (ask-bid)/bid. Default is None,
-            equivalent to 0.0. Practical spreads are negligible on US liquid stocks.
-
-        round_trades (bool): round the trade weights provided by a policy so they correspond to an integer
-            number of stocks traded. Default is True using Yahoo Finance open prices.
-
-        per_share_fixed_cost (float): transaction cost per share traded. Default value is 0.005 (USD), uses
-             Yahoo Finance open prices to simulate the number of stocks traded. See
-            https://www.interactivebrokers.com/en/pricing/commissions-home.php
-
-        transaction_cost_coefficient_b (float, pd.Series, or pd.DataFrame): coefficient that multiplies the non-linear
-            term of the transaction cost. Default value is 1, you can pass any other constant value, a per-stock Series,
-            or a per-day and per-stock DataFrame
-
-        transaction_cost_exponent (float): exponent of the non-linear term of the transaction cost model. Default value 1.5,
-             this is applied to the trade volume (in US dollars) over the total market volume (in US dollars). See the
-            paper for more details; this model is supported by a long tradition of research in market microstructure.
-
-        rolling_window_sigma_estimator (int): we use an historical rolling standard deviation to estimate the average
-            size of the return on a stock on each day, and this multiplies the second term of the transaction cost model.
-             See the paper for an explanation of the model. Here you specify the length of the rolling window to use,
-             default is 1000.
-
-        spread_on_borrowing_stocks_percent (float, pd.Series, pd.DataFrame): when shorting a stock,
-            you will pay a rate on the value
-            of the position equal to the cash return plus this spread, expressed in percent annualized. These
-            values are hard to find historically, if you are unsure consider long-only portfolios or look
-            at CFDs/futures instead. We set the default value to 0.5 (percent annualized) which is probably OK
-            for US large cap stocks. See https://www.interactivebrokers.com/en/pricing/short-sale-cost.php
-
-        spread_on_long_positions_percent (float, None, pd.Series, pd.DataFrame): if you trade CFDs you will pay interest
-            on your long positions
-            as well as your short positions, equal to the cash return plus this value (percent annualized). If
-             instead this is None, the default value, you pay nothing on your long positions (as you do if you trade
-            stocks). We don't consider dividend payments because those are already incorporated in the
-            open-to-open returns as we compute them from the Yahoo Finance data. See cvxportfolio.data for details.
-
-        dividends (float, pd.DataFrame): if not included in the returns (as they are by the default data interface,
-            based on `yfinance`), you can pass a DataFrame of dividend payments which will be credited to the cash
-            account (or debited, if short) at each round. Default is 0., corresponding to no dividends.
-
-        spread_on_lending_cash_percent (float, pd.Series): the cash account will generate annualized
-            return equal to the cash return minus this number, expressed in percent annualized, or zero if
-            the spread is larger than the cash return. For example with USDOLLAR cash,
-            if the FRED-DFF annualized rate is 4.8% and spread_on_lending_cash_percent is 0.5
-            (the default value), then the uninvested cash in the portfolio generates annualized
-            return of 4.3%. See https://www.interactivebrokers.com/en/accounts/fees/pricing-interest-rates.php
-
-        spread_on_borrowing_cash_percent (float, pd.Series): if we instead borrow cash we pay the
-            cash rate plus this spread, expressed in percent annualized. Default value is 0.5.
-            See https://www.interactivebrokers.com/en/trading/margin-rates.php
-
-        cash_key (str or None): name of the cash account. Default is 'USDOLLAR', which gets downloaded by `cvxportfolio.data`
-            as the Federal Funds effective rate from FRED. If None, you must pass the cash returns
-            along with the stock returns as its last column.
-
-        base_location (pathlib.Path): base location for (by default, sqlite) storage of data.
-            Default is `Path.home() / "cvxportfolio"`. Unused if passing `returns` and `volumes`.
+    :type volumes: pandas.DataFrame
+    :param prices: historical open prices. Default is None, it is ignored
+        if universe is specified. These are used to round the trades to integer number of stocks
+        if round_trades is True, and compute per-share transaction costs (if `per_share_fixed_cost`
+        is greater than zero).
+    :type prices: pandas.DataFrame
+    :param spreads: historical bid-ask spreads expressed as (ask-bid)/bid. Default is None,
+        equivalent to 0.0. Practical spreads are negligible on US liquid stocks.
+    :type spreads: pandas.DataFrame
+    :param round_trades: round the trade weights provided by a policy so they correspond to an integer
+        number of stocks traded. Default is True using Yahoo Finance open prices.
+    :type round_trades: bool
+    :param per_share_fixed_cost: transaction cost per share traded. Default value is 0.005 (USD), uses
+        Yahoo Finance open prices to simulate the number of stocks traded. See 
+        `this page <https://www.interactivebrokers.com/en/pricing/commissions-home.php>`_.
+    :type per_share_fixed_cost: float
+    :param transaction_cost_coefficient_b: coefficient that multiplies the non-linear
+        term of the transaction cost. Default value is 1, you can pass any other constant value, a per-stock Series,
+        or a per-day and per-stock DataFrame
+    :type transaction_cost_coefficient_b: float, pd.Series, or pd.DataFrame
+    :param transaction_cost_exponent: exponent of the non-linear term of the transaction cost model. Default value 1.5,
+        this is applied to the trade volume (in US dollars) over the total market volume (in US dollars). See the
+        paper for more details; this model is supported by a long tradition of research in market microstructure.
+    :type transaction_cost_exponent: float
+    :param window_sigma_estimate: we use an historical rolling standard deviation to estimate the average
+        size of the return on a stock on each day, and this multiplies the second term of the transaction cost model.
+        See the paper for an explanation of the model. Here you specify the length of the rolling window to use,
+        default is 252 (typical number of trading days in a year).
+    :type window_sigma_estimate: int
+    :param spread_on_borrowing_stocks_percent: when shorting a stock,
+        one pays a rate on the value of the position equal to the cash return plus this spread, 
+        expressed in percent annualized. These values are hard to find historically, if you are unsure consider 
+        long-only portfolios or look at CFDs/futures instead. We set the default value to 0.5 (percent annualized) 
+        which is probably OK for US large cap stocks. See `this page <https://www.interactivebrokers.com/en/pricing/short-sale-cost.php>`_.
+    :type spread_on_borrowing_stocks_percent: float, pd.Series, pd.DataFrame
+    :param spread_on_long_positions_percent: if you trade CFDs one pays interest on long positions  as well as your short positions, 
+        equal to the cash return plus this value (percent annualized). If
+        instead this is None, the default value, you pay nothing on your long positions (as you do if you trade
+        stocks). We don't consider dividend payments because those are already incorporated in the
+        open-to-open returns as we compute them from the Yahoo Finance data. See cvxportfolio.data for details.
+    :type spread_on_long_positions_percent: float, None, pd.Series, pd.DataFrame
+    :param dividends: if not included in the returns (as they are by the default data interface,
+        based on `yfinance`), you can pass a DataFrame of dividend payments which will be credited to the cash
+        account (or debited, if short) at each round. Default is 0., corresponding to no dividends.
+    :type dividends: float, pd.DataFrame
+    :param spread_on_lending_cash_percent: the cash account will generate annualized
+        return equal to the cash return minus this number, expressed in percent annualized, or zero if
+        the spread is larger than the cash return. For example with USDOLLAR cash,
+        if the FRED-DFF annualized rate is 4.8% and spread_on_lending_cash_percent is 0.5
+        (the default value), then the uninvested cash in the portfolio generates annualized
+        return of 4.3%. See `this page <https://www.interactivebrokers.com/en/accounts/fees/pricing-interest-rates.php>_`.
+    :type spread_on_lending_cash_percent: float, pd.Series
+    :param spread_on_borrowing_cash_percent: if one instead borrows cash he pays the
+        cash rate plus this spread, expressed in percent annualized. Default value is 0.5.
+        See `this page <https://www.interactivebrokers.com/en/trading/margin-rates.php>_`.
+    :type spread_on_borrowing_cash_percent: float, pd.Series 
+    :param cash_key: name of the cash account. Default is 'USDOLLAR', which gets downloaded by `cvxportfolio.data`
+        as the Federal Funds effective rate from FRED. If None, you must pass the cash returns
+        along with the stock returns as its last column.
+    :type cash_key: str or None
+    :param base_location: base location for storage of data.
+        Default is `Path.home() / "cvxportfolio_data"`. Unused if passing `returns` and `volumes`.
+    :type base_location: pathlib.Path or str: 
     """
 
     periods_per_year = 252
 
     def __init__(
             self,
             universe=[],
@@ -133,23 +137,22 @@
             costs=None,
             prices=None,
             spreads=0.,
             round_trades=True,
             per_share_fixed_cost=0.005,
             transaction_cost_coefficient_b=1.,
             transaction_cost_exponent=1.5,
-            rolling_window_sigma_estimator=1000,
+            window_sigma_estimate=252,
             spread_on_borrowing_stocks_percent=.5,
             spread_on_long_positions_percent=None,
             dividends=0.,
             spread_on_lending_cash_percent=.5,
             spread_on_borrowing_cash_percent=.5,
             cash_key="USDOLLAR",
-            base_location=Path.home() /
-            "cvxportfolio"):
+            base_location=BASE_LOCATION):
         """Initialize the Simulator and download data if necessary."""
         if not len(universe):
             if costs is None: # we allow old simulator syntax for the time being
                 if ((returns is None) or (volumes is None)):
                     raise SyntaxError(
                         "If you don't specify a universe you should pass `returns` and `volumes`.")
                 if not returns.shape[1] == volumes.shape[1] + 1:
@@ -178,42 +181,41 @@
 
         self.spreads = DataEstimator(spreads)
         self.dividends = DataEstimator(dividends)
         self.round_trades = round_trades
         self.per_share_fixed_cost = per_share_fixed_cost
         self.transaction_cost_coefficient_b = transaction_cost_coefficient_b
         self.transaction_cost_exponent = transaction_cost_exponent
-        self.rolling_window_sigma_estimator = rolling_window_sigma_estimator
+        self.window_sigma_estimate = window_sigma_estimate
         self.spread_on_borrowing_stocks_percent = spread_on_borrowing_stocks_percent
         self.spread_on_long_positions_percent = spread_on_long_positions_percent
         self.spread_on_lending_cash_percent = spread_on_lending_cash_percent
         self.spread_on_borrowing_cash_percent = spread_on_borrowing_cash_percent
 
         # compute my DataEstimator(s)
         self.sigma_estimate = DataEstimator(
-            self.returns.data.iloc[:, :-1].rolling(self.rolling_window_sigma_estimator).std().shift(1))
+            self.returns.data.iloc[:, :-1].rolling(window=self.window_sigma_estimate, min_periods=1).std().shift(1))
 
     def prepare_data(self):
         """Build data from data storage and download interfaces.
 
         This is a first cut, it's doing a for loop when we could instead parallelize
         at the `yfinance` level and use the estimator logic of TimeSeries directly.
         """
         self.database_accesses = {}
+        print('Updating data')
         for stock in self.universe:
-            print('Updating data...')
-            self.database_accesses[stock] = TimeSeries(
-                stock, base_location=self.base_location)
+            print('.')
+            self.database_accesses[stock] = YfinanceTimeSeries(stock, base_location=self.base_location)
             self.database_accesses[stock].pre_evaluation()
         if not self.cash_key == 'USDOLLAR':
-            raise NotImplementedError(
-                'Currently the only data pipeline built is for USDOLLAR cash')
-        self.database_accesses[self.cash_key] = TimeSeries(
-            'DFF', source='fred', base_location=self.base_location)
+            raise NotImplementedError('Currently the only data pipeline built is for USDOLLAR cash')
+        self.database_accesses[self.cash_key] = FredRateTimeSeries('DFF', base_location=self.base_location)
         self.database_accesses[self.cash_key].pre_evaluation()
+        # print()
 
         # build returns
         self.returns = pd.DataFrame(
             {stock: self.database_accesses[stock].data['Return'] for stock in self.universe})
         self.returns[self.cash_key] = self.database_accesses[self.cash_key].data
         self.returns[self.cash_key] = self.returns[self.cash_key].fillna(
             method='ffill')
@@ -243,15 +245,16 @@
         
         self.returns = DataEstimator(self.returns)
         self.volumes = DataEstimator(self.volumes)
         self.prices = DataEstimator(self.prices)
         
         
     def round_trade_vector(self, u):
-        """Round dollar trade vector u."""
+        """Round dollar trade vector u.
+        """
         result = pd.Series(u, copy=True)
         result[:-1] = np.round(u[:-1] / self.prices.current_value) * self.prices.current_value
         result[-1] = -sum(result[:-1])
         return result
 
 
     def transaction_costs(self, u):
@@ -262,24 +265,27 @@
         Args:
             u (pd.Series): dollar trade vector for all stocks including cash (but the cash
                 term is not used here).
         """
 
         result = 0.
         if self.prices is not None:
-            # compute number of shares traded.
-            # we assume round_trades is True and we add a small number to ensure
-            # we are on the safe side of rounding errors
+
             result += self.per_share_fixed_cost * int(sum(np.abs(u[:-1] + 1E-6) / self.prices.current_value))
 
         if self.spreads is not None:
             result += sum(self.spreads.current_value * np.abs(u[:-1]))/2.
 
-        result += (np.abs(u[:-1])**self.transaction_cost_exponent) @ (self.transaction_cost_coefficient_b * self.sigma_estimate.current_value / (
-            self.volumes.current_value ** (self.transaction_cost_exponent - 1)))
+        result += (np.abs(u[:-1])**self.transaction_cost_exponent) @ (self.transaction_cost_coefficient_b * 
+            self.sigma_estimate.current_value / (
+            (self.volumes.current_value+1 # we add 1 to prevent 0 volumes error
+             ) ** (self.transaction_cost_exponent - 1)))
+            
+        assert not np.isnan(result)
+        assert not np.isinf(result)
             
         return -result
 
     def stocks_holding_costs(self, h_plus):
         """Compute holding costs at current time for post trade holdings h_plus (only stocks).
 
         Args:
@@ -332,302 +338,168 @@
         because we pass the policy directly to it, and the past returns and past volumes
         are computed by it.
         """
         
         # translate to weights
         current_portfolio_value = sum(h)
         current_weights = h / current_portfolio_value
+        # print(t, current_portfolio_value)
 
         # get view of past data
         past_returns = self.returns.data.loc[self.returns.data.index < t]
         past_volumes = self.volumes.data.loc[self.volumes.data.index < t]
 
-        # update all internal estimators
-        super().values_in_time(t, current_weights, current_portfolio_value, past_returns, past_volumes, **kwargs)
+        # update internal estimators (spreads, dividends, volumes, ..., )
+        super().values_in_time(t=t)
 
         # evaluate the policy
-        z = policy.values_in_time(t, current_weights, current_portfolio_value, past_returns, past_volumes, **kwargs)
-        # for safety
+        z = policy.values_in_time(t=t, current_weights=current_weights, current_portfolio_value=current_portfolio_value, 
+            past_returns=past_returns, past_volumes=past_volumes, current_prices=self.prices.current_value, **kwargs)
+        
+        # for safety recompute cash
         z[-1] = -sum(z[:-1])
-
+        assert sum(z) == 0.
+        
         # trades in dollars
         u = z * current_portfolio_value
 
-        # zero out trades on stock that weren't trading on that day
-        current_volumes = self.volumes.current_value
-        non_tradable_stocks = current_volumes[current_volumes <= 0]
+        # zero out trades on stock that weren't trading on that day 
+        current_volumes = pd.Series(self.volumes.current_value, self.volumes.data.columns)
+        non_tradable_stocks = current_volumes[current_volumes <= 0].index
         u[non_tradable_stocks] = 0.
 
         # round trades
         if self.round_trades:
             u = self.round_trade_vector(u)
+            
+        # for safety recompute cash
+        u[-1] = -sum(u[:-1])
+        assert sum(u) == 0.
 
         # compute post-trade holdings (including cash balance)
         h_plus = h + u
 
-        # we have updated the internal estimators and they are used by these
-        # methods
+        # we have updated the internal estimators and they are used by these methods
         transaction_costs = self.transaction_costs(u)
         holding_costs = self.stocks_holding_costs(h_plus)
         cash_holding_costs = self.cash_holding_cost(h_plus)
 
-        # multiply positions by market returns
+        # multiply positions by market returns (only non-cash)
         h_next = pd.Series(h_plus, copy=True)
         h_next[:-1] *= (1 + self.returns.current_value[:-1])
         
         # credit costs to cash (includes cash return)
         h_next[-1] = h_plus[-1] + (transaction_costs + holding_costs + cash_holding_costs)
             
-        return h_next, z, u, transaction_costs, holding_costs, cash_holding_costs
+        return h_next, z, u, transaction_costs, holding_costs, cash_holding_costs, 
         
     def initialize_policy(self, policy, start_time, end_time):
         """Initialize the policy object.
-        
-        This method differs from other Estimators because it is the Simulator
-        that initializes the policy and all its dependents. It is called by Backtest.
         """
-        policy.pre_evaluation(self.returns.data.loc[self.returns.data.index<end_time], 
-                              self.volumes.data.loc[self.volumes.data.index<end_time], 
-                              start_time, end_time)
-        
-        
-    ### THE FOLLOWING METHODS ARE FROM THE ORIGINAL SIMULATOR (PRE-2023)
-    ### The main difference is that you pass a list of costs, which implement
-    ### a `value_expression` method, and those take care of the cost evaluation
-    ### during backtest. These can be used, as they are in the examples, using
-    ### `legacy_run_backtest` and `legacy_run_multiple_backtest`. 
-    ###
-    ### Also, we have two methods that are not part of the book
-    ### and are not well-documented, `what_if` and `attribute`. We may remove
-    ### all methods below this comment block in the coming months.
-
-    def propagate(self, h, u, t):
-        """Propagates the portfolio forward over time period t, given trades u.
-
-        Args:
-            h: pandas Series object describing current portfolio
-            u: n vector with the stock trades (not cash)
-            t: current time
-
-        Returns:
-            h_next: portfolio after returns propagation
-            u: trades vector with simulated cash balance
+        policy.pre_evaluation(universe = self.returns.data.columns, 
+                             backtest_times = self.returns.data.index[(self.returns.data.index<end_time) & 
+                                 (self.returns.data.index>=start_time)])
+                                 
+    def _single_backtest(self, policy, start_time, end_time, h):
+        
+        if hasattr(policy, 'compile_to_cvxpy'):
+            policy.compile_to_cvxpy()
+        
+        h_df = pd.DataFrame(columns=self.returns.data.columns)
+        u = pd.DataFrame(columns=self.returns.data.columns)
+        z = pd.DataFrame(columns=self.returns.data.columns)
+        tcost = pd.Series(dtype=float)
+        hcost_stocks = pd.Series(dtype=float)
+        hcost_cash = pd.Series(dtype=float)
+        
+        for t in self.returns.data.index[(self.returns.data.index >= start_time) & (self.returns.data.index < end_time)]:
+            h_df.loc[t] = h
+            h, z.loc[t], u.loc[t], tcost.loc[t], hcost_stocks.loc[t], hcost_cash.loc[t] = \
+                self.simulate(t=t, h=h, policy=policy)
+        
+        h_df.loc[pd.Timestamp(end_time)] = h  
+        
+        return BacktestResult(h=h_df, u=u, z=z, tcost=tcost, hcost_stocks=hcost_stocks, hcost_cash=hcost_cash, 
+            cash_returns=self.returns.data[self.cash_key].loc[u.index])
+        
+                  
+                                 
+    def backtest(self, policy, start_time, end_time=None, initial_value = 1E6, h=None, parallel=True):
+        """Backtest one or more trading policy.
+        
+        If runnning in parallel you must be careful at how you use this method. If 
+        you use this in a script, you should define the MarketSimulator
+        *in* the `if __name__ == '__main__:'` clause, and call this method there as well.
+        
+        The default initial portfolio is all cash, or you can pass any portfolio with
+        the `h` argument, or a list of those if running multiple backtests.
+        
+        :param policy: if passing a single trading policy it performs a single backtest 
+            in the main process. If passing a list, it uses Python multiprocessing to
+            create multiple processes and run many policies in parallel.
+        :type policy: cvx.BaseTradingPolicy or list
+        :param start_time: start time of the backtest(s), if holiday, the first trading day
+             after it is selected
+        :type start_time: str or datetime 
+        :param end_time: end time of the backtest(s), if holiday, the last trading day
+             before it is selected
+        :type end_time: str or datetime or None
+        :param initial_value: initial value in dollar of the portfolio, if not specifying
+            `h` it is assumed the initial portfolio is all cash
+        :type initial_value: float
+        :param h: initial portfolio `h` expressed in dollar positions, or list of those 
+            for multiple backtests
+        :type h: list or pd.Series or None
+        :param parallel: whether to run in parallel if there are multiple policies or not.
+            If not, it just iterates through the policies in the main process.
+        :type parallel: bool
+        
+        :returns result: instance of :class:`BacktestResult` which has all relevant backtest
+            data and logic to compute metrics, generate plots, ...
+        :rtype result: cvx.BacktestResult or list
         """
-        assert u.index.equals(h.index)
-
-        if self.volumes is not None:
-            # don't trade if volume is null
-            null_trades = self.volumes.data.columns[self.volumes.data.loc[t] == 0]
-            if len(null_trades):
-                logging.info(
-                    "No trade condition for stocks %s on %s" % (null_trades, t)
-                )
-                u.loc[null_trades] = 0.0
-
-        hplus = h + u
-        costs = [cost.value_expr(t, h_plus=hplus, u=u) for cost in self.costs]
-        for cost in costs:
-            assert not pd.isnull(cost)
-            assert not np.isinf(cost)
-
-        u[self.cash_key] = -sum(u[u.index != self.cash_key]) - sum(costs)
-        hplus[self.cash_key] = h[self.cash_key] + u[self.cash_key]
-
-        assert hplus.index.sort_values().equals(
-            self.returns.data.columns.sort_values()
-        )
-        h_next = self.returns.data.loc[t] * hplus + hplus
-
-        assert not h_next.isnull().values.any()
-        assert not u.isnull().values.any()
-        return h_next, u
-
-    def legacy_run_backtest(
-            self,
-            initial_portfolio,
-            start_time,
-            end_time,
-            policy,
-            loglevel=logging.WARNING):
-        """Backtest a single policy."""
-        logging.basicConfig(level=loglevel)
-
-        results = SimulationResult(
-            initial_portfolio=copy.copy(initial_portfolio),
-            policy=policy,
-            cash_key=self.cash_key,
-            simulator=self,
-        )
-        h = initial_portfolio
-
-        simulation_times = self.returns.data.index[
-            (self.returns.data.index >= start_time)
-            & (self.returns.data.index <= end_time)
-        ]
-        logging.info(
-            "Backtest started, from %s to %s"
-            % (simulation_times[0], simulation_times[-1])
-        )
-
-        for t in simulation_times:
-            logging.info("Getting trades at time %s" % t)
-            start = time.time()
-            try:
-                u = policy.get_trades(h, t)
-            except cvx.SolverError:
-                logging.warning(
-                    "Solver failed on timestamp %s. Default to no trades." % t
-                )
-                u = pd.Series(index=h.index, data=0.0)
-            end = time.time()
-            assert not pd.isnull(u).any()
-            results.log_policy(t, end - start)
-
-            logging.info("Propagating portfolio at time %s" % t)
-            start = time.time()
-            h, u = self.propagate(h, u, t)
-            end = time.time()
-            assert not h.isnull().values.any()
-            results.log_simulation(
-                t=t,
-                u=u,
-                h_next=h,
-                risk_free_return=self.returns.data.loc[t, self.cash_key],
-                exec_time=end - start,
-            )
-
-        logging.info(
-            "Backtest ended, from %s to %s"
-            % (simulation_times[0], simulation_times[-1])
-        )
-        return results
-
-    def legacy_run_multiple_backtest(
-        self,
-        initial_portf,
-        start_time,
-        end_time,
-        policies,
-        loglevel=logging.WARNING,
-        parallel=True,
-    ):
-        """Backtest multiple policies."""
-
-        def _legacy_run_backtest(policy):
-            return self.legacy_run_backtest(
-                initial_portf, start_time, end_time, policy, loglevel=loglevel
-            )
-
-        num_workers = min(multiprocess.cpu_count(), len(policies))
-        if parallel:
-            workers = multiprocess.Pool(num_workers)
-            results = workers.map(_legacy_run_backtest, policies)
-            workers.close()
-            return results
+        
+        # turn policy and h into lists
+        if not hasattr(policy, '__len__'):
+            policy = [policy]
+        
+        if not hasattr(h, '__len__'):
+            h = [h]*len(policy)
+            
+        if not (len(policy) == len(h)):
+            raise SyntaxError("If passing lists of policies and initial portfolios they must have the same length.")
+        
+        # discover start and end times
+        start_time = pd.Series(self.returns.data.index >= start_time, self.returns.data.index).idxmax()
+        if end_time is None:
+            end_time  = self.returns.data.index[-1]
         else:
-            return list(map(_legacy_run_backtest, policies))
-
-    def what_if(self, time, results, alt_policies, parallel=True):
-        """Run alternative policies starting from given time."""
-        # TODO fix
-        initial_portf = copy.copy(results.h.loc[time])
-        all_times = results.h.index
-        alt_results = self.legacy_run_multiple_backtest(
-            initial_portf, time, all_times[-1], alt_policies, parallel
-        )
-        for idx, alt_result in enumerate(alt_results):
-            alt_result.h.loc[time] = results.h.loc[time]
-            alt_result.h.sort_index(axis=0, inplace=True)
-        return alt_results
-
-    @staticmethod
-    def reduce_signal_perturb(initial_weights, delta):
-        """Compute matrix of perturbed weights given initial weights."""
-        perturb_weights_matrix = np.zeros(
-            (len(initial_weights), len(initial_weights)))
-        for i in range(len(initial_weights)):
-            perturb_weights_matrix[i, :] = initial_weights / (
-                1 - delta * initial_weights[i]
-            )
-            perturb_weights_matrix[i, i] = (1 - delta) * initial_weights[i]
-        return perturb_weights_matrix
-
-    def attribute(
-            self,
-            true_results,
-            policy,
-            selector=None,
-            delta=1,
-            fit="linear",
-            parallel=True):
-        """Attributes returns over a period to individual alpha sources.
-
-        Args:
-            true_results: observed results.
-            policy: the policy that achieved the returns.
-                    Alpha model must be a stream.
-            selector: A map from SimulationResult to time series.
-            delta: the fractional deviation.
-            fit: the type of fit to perform.
-        Returns:
-            A dict of alpha source to return series.
-        """
-        # Default selector looks at profits.
-        if selector is None:
-
-            def selector(result):
-                return result.v - sum(result.initial_portfolio)
-
-        alpha_stream = policy.return_forecast
-        assert isinstance(alpha_stream, MultipleReturnsForecasts)
-        times = true_results.h.index
-        weights = alpha_stream.weights
-        assert np.sum(weights) == 1
-        alpha_sources = alpha_stream.alpha_sources
-        num_sources = len(alpha_sources)
-        Wmat = self.reduce_signal_perturb(weights, delta)
-        perturb_pols = []
-        for idx in range(len(alpha_sources)):
-            new_pol = copy.copy(policy)
-            new_pol.return_forecast = MultipleReturnsForecasts(
-                [ReturnsForecast(el.expected_returns.data) for el in alpha_sources],
-                #alpha_sources,
-                Wmat[idx, :]
-            )
-            perturb_pols.append(new_pol)
-        # Simulate
-        p0 = true_results.initial_portfolio
-        alt_results = self.legacy_run_multiple_backtest(
-            p0, times[0], times[-1], perturb_pols, parallel=parallel
-        )
-        # Attribute.
-        true_arr = selector(true_results).values
-        attr_times = selector(true_results).index
-        Rmat = np.zeros((num_sources, len(attr_times)))
-        for idx, result in enumerate(alt_results):
-            Rmat[idx, :] = selector(result).values
-        Pmat = cvx.Variable((num_sources, len(attr_times)))
-        if fit == "linear":
-            prob = cvx.Problem(cvx.Minimize(0), [Wmat @ Pmat == Rmat])
-            prob.solve()
-        elif fit == "least-squares":
-            error = cvx.sum_squares(Wmat @ Pmat - Rmat)
-            prob = cvx.Problem(
-                cvx.Minimize(error), [
-                    Pmat.T @ weights == true_arr])
-            prob.solve()
+            end_time = self.returns.data.index[self.returns.data.index <= end_time][-1]
+        
+        # initialize policies and get initial portfolios
+        for i in range(len(policy)):
+            self.initialize_policy(policy[i], start_time, end_time)
+        
+            if h[i] is None:
+                h[i] = pd.Series(0., self.returns.data.columns)
+                h[i][-1] = initial_value
+                
+        def parallel_runner(zipped):
+            return self._single_backtest(zipped[0], start_time, end_time, zipped[1])
+            
+        # parallel_worker(policy, simulator, start_time, end_time, h)
+        
+        
+        # decide if run in parallel or not
+        if (not parallel) or len(policy) == 1:
+            result = list(map(parallel_runner, zip(policy, h)))
         else:
-            raise Exception("Unknown fitting method.")
-        # Dict of results.
-        wmask = np.tile(weights[:, np.newaxis], (1, len(attr_times))).T
-        data = pd.DataFrame(
-            columns=[s.name for s in alpha_sources],
-            index=attr_times,
-            data=Pmat.value.T * wmask,
-        )
-        data["residual"] = true_arr - \
-            np.asarray((weights @ Pmat).value).ravel()
-        data["RMS error"] = np.asarray(
-            cvx.norm(Wmat @ Pmat - Rmat, 2, axis=0).value
-        ).ravel()
-        data["RMS error"] /= np.sqrt(num_sources)
-        return data
+            with Pool() as p:
+                # if not __name__ == '__main__':
+                #     raise SyntaxError('When executing parallel backtests, the Simulator should be instantiated ')
+                result = p.starmap(parallel_worker, zip(policy, [self] * len(policy), [start_time] * len(policy), [end_time] * len(policy), h))
+                
+        if len(result) == 1:
+            return result[0]
+        return result
+        
+
```


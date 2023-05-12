# Comparing `tmp/predictable-0.0.0a0.tar.gz` & `tmp/predictable-0.0.1.tar.gz`

## Comparing `predictable-0.0.0a0.tar` & `predictable-0.0.1.tar`

### file list

```diff
@@ -1,46 +1,34 @@
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 predictable-0.0.0a0/.flake8
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 predictable-0.0.0a0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 predictable-0.0.0a0/.readthedocs.yml
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 predictable-0.0.0a0/make_docs.sh
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 predictable-0.0.0a0/requirements.txt
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 predictable-0.0.0a0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 predictable-0.0.0a0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 predictable-0.0.0a0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 predictable-0.0.0a0/.github/workflows/pytest.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 predictable-0.0.0a0/docs/.gitkeep
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 predictable-0.0.0a0/docs/Makefile
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 predictable-0.0.0a0/docs/api.md
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 predictable-0.0.0a0/docs/conf.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 predictable-0.0.0a0/docs/getting_started.md
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 predictable-0.0.0a0/docs/index.md
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 predictable-0.0.0a0/docs/license.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 predictable-0.0.0a0/docs/make.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 predictable-0.0.0a0/examples/__init__.py
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 predictable-0.0.0a0/examples/model.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 predictable-0.0.0a0/examples/run.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 predictable-0.0.0a0/examples/input/modelpoints.csv
--rw-r--r--   0        0        0     6517 2020-02-02 00:00:00.000000 predictable-0.0.0a0/examples/tables/economic.csv
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 predictable-0.0.0a0/examples/tables/lapses.csv
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 predictable-0.0.0a0/examples/tables/sa8990.csv
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 predictable-0.0.0a0/src/predictable/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 predictable-0.0.0a0/src/predictable/core/__init__.py
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 predictable-0.0.0a0/src/predictable/core/discounting.py
--rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 predictable-0.0.0a0/src/predictable/core/flows.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 predictable-0.0.0a0/src/predictable/core/lookup.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 predictable-0.0.0a0/src/predictable/core/model.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 predictable-0.0.0a0/src/predictable/core/precision.py
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 predictable-0.0.0a0/src/predictable/core/rating_factors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 predictable-0.0.0a0/src/predictable/engine/__init__.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 predictable-0.0.0a0/src/predictable/engine/run.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 predictable-0.0.0a0/tests/__init__.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 predictable-0.0.0a0/tests/test_discounting.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 predictable-0.0.0a0/tests/test_flows.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 predictable-0.0.0a0/tests/test_lookup.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 predictable-0.0.0a0/tests/test_model.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 predictable-0.0.0a0/tests/test_precision.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 predictable-0.0.0a0/tests/test_run.py
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 predictable-0.0.0a0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 predictable-0.0.0a0/LICENSE
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 predictable-0.0.0a0/README.md
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 predictable-0.0.0a0/pyproject.toml
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 predictable-0.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 predictable-0.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 predictable-0.0.1/.readthedocs.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 predictable-0.0.1/examples/__init__.py
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 predictable-0.0.1/examples/model.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 predictable-0.0.1/examples/rpt.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 predictable-0.0.1/examples/run.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 predictable-0.0.1/examples/input/modelpoints.csv
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 predictable-0.0.1/examples/input/modelpoints.rpt
+-rw-r--r--   0        0        0     6517 2020-02-02 00:00:00.000000 predictable-0.0.1/examples/tables/economic.csv
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 predictable-0.0.1/examples/tables/lapses.csv
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 predictable-0.0.1/examples/tables/sa8990.csv
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 predictable-0.0.1/predictable/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 predictable-0.0.1/predictable/core/__init__.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 predictable-0.0.1/predictable/core/discounting.py
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 predictable-0.0.1/predictable/core/flows.py
+-rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 predictable-0.0.1/predictable/core/io.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 predictable-0.0.1/predictable/core/lookup.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 predictable-0.0.1/predictable/core/model.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 predictable-0.0.1/predictable/core/precision.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 predictable-0.0.1/predictable/core/rating_factors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 predictable-0.0.1/predictable/engine/__init__.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 predictable-0.0.1/predictable/engine/run.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 predictable-0.0.1/tests/__init__.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 predictable-0.0.1/tests/test_discounting.py
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 predictable-0.0.1/tests/test_flows.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 predictable-0.0.1/tests/test_lookup.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 predictable-0.0.1/tests/test_model.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 predictable-0.0.1/tests/test_precision.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 predictable-0.0.1/tests/test_run.py
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 predictable-0.0.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 predictable-0.0.1/LICENSE
+-rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 predictable-0.0.1/README.md
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 predictable-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 predictable-0.0.1/PKG-INFO
```

### Comparing `predictable-0.0.0a0/examples/model.py` & `predictable-0.0.1/examples/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,76 +1,70 @@
-# `pip install -e .` to install the library in development
 # import the library
-
-import predictable as dv
+import predictable as pr
 
 
 def handler(modelpoint, **kwargs):
     # NOTE: **kwargs used to access info from RunConfig e.g.
     # NOTE: `table_location` can be used in TableLookup components
     # NOTE: `results_location` can be used to store results on a modelpoint level
 
     # Create new model instance
-    model = dv.Model()
+    model = pr.Model()
 
     # Add static components
-    age = dv.RatingFactor(
+    age = pr.RatingFactor(
         input_array=[modelpoint.age],
         formula=lambda prev: prev + 1,
         label="age",
     )
-    gender = dv.RatingFactor(input_array=[modelpoint.gender], label="gender")
-    smoker = dv.RatingFactor(
-        input_array=[modelpoint.smoker_status], label="smoker"
-    )
+    gender = pr.RatingFactor(input_array=[modelpoint.gender], label="gender")
+    smoker = pr.RatingFactor(input_array=[modelpoint.smoker_status], label="smoker")
 
     # Add components that have a projected value
-    prem = dv.CashFlow(
+    prem = pr.CashFlow(
         input_array=[modelpoint.premium],
         formula=lambda prev: prev * 1.05,
         label="premium",
     )
-    cover = dv.CashFlow(input_array=[modelpoint.cover], label="cover")
-    exp = dv.StaticFlow(
+    cover = pr.CashFlow(input_array=[modelpoint.cover], label="cover")
+    exp = pr.StaticFlow(
         input_array=[modelpoint.expenses for _ in range(5)],
         label="expense",
     )
 
     # Add actuarial components
-    qx = dv.TableLookup(
+    qx = pr.TableLookup(
         table_name=kwargs["table_location"] / "sa8990.csv",
         lookup_on=["age"],
         keep_column="qx",
         label="qx",
     )
-    lapses = dv.TableLookup(
+    lapses = pr.TableLookup(
         table_name=kwargs["table_location"] / "lapses.csv",
         lookup_on=["t"],
         keep_column="lapse_rate_pa",
         default_value=0,
         label="lapse",
     )
 
-    v = dv.DiscountFactors(interest_rate=0.05, label="V")
+    v = pr.DiscountFactors(interest_rate=0.05, label="V")
 
     # Attach components to the model
     component_list = [age, gender, smoker, prem, cover, exp, v, qx, lapses]
     model.add_components(component_list)
 
     # Project over a given term
     # Results return a pandas df object
     df = model.project(term=33 - modelpoint.age)
 
     # Perform linear combination style manipulations
     components = ["premium", "cover", "expense"]
     for component in components:
         # NOTE: The logic here is just for illustration purposes
-        df[f"EPV_{component}"] = (
-            df[component] * df["V"] * df["qx"] * (1 - df["lapse"])
-        )
+        df[f"EPV_{component}"] = df[component] * df["V"] * df["qx"] * (1 - df["lapse"])
 
     # Define reserving relationship
     df["EPV_BEL"] = df["EPV_cover"] + df["EPV_expense"] - df["EPV_premium"]
 
     df_out = df[["EPV_premium", "EPV_cover", "EPV_expense", "EPV_BEL"]].sum()
 
     print(df)
```

### Comparing `predictable-0.0.0a0/examples/run.py` & `predictable-0.0.1/examples/run.py`

 * *Files identical despite different names*

### Comparing `predictable-0.0.0a0/examples/tables/economic.csv` & `predictable-0.0.1/examples/tables/economic.csv`

 * *Files identical despite different names*

### Comparing `predictable-0.0.0a0/examples/tables/sa8990.csv` & `predictable-0.0.1/examples/tables/sa8990.csv`

 * *Files identical despite different names*

### Comparing `predictable-0.0.0a0/src/predictable/core/discounting.py` & `predictable-0.0.1/predictable/core/discounting.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,12 @@
         :param term: Term over which to project
         :type term: int
         :return: StaticDiscountFactors object containing projected values
         :rtype: StaticDiscountFactors
         """
         results = self
         for n in range(1, term + 1):
-            results = np.append(
-                results, i_to_v(self.formula(self.interest_rate)) ** n
-            )
+            results = np.append(results, i_to_v(self.formula(self.interest_rate)) ** n)
         return StaticFlow(
             input_array=results,
             label=self.label,
         )
```

### Comparing `predictable-0.0.0a0/src/predictable/core/flows.py` & `predictable-0.0.1/predictable/core/flows.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 from numpy.typing import ArrayLike
 from pandas import DataFrame
 
 from .precision import get_precision
 
 
 class StaticFlow(np.ndarray):
-    """Static cashflow object created from an Array-Like object. Subclasses numpy.ndarray"""
+    """
+    Static cashflow object created from an Array-Like object.
+    Subclasses numpy.ndarray
+    """
 
     def __new__(cls, input_array: ArrayLike, label: str = None):
         # We first cast to be our class type
         obj = np.asarray(input_array).view(cls)
         # add new attributes to the created instance
         obj.label = label
         # Finally, we must return the newly created object:
```

### Comparing `predictable-0.0.0a0/src/predictable/core/lookup.py` & `predictable-0.0.1/predictable/core/lookup.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,16 +53,16 @@
         :type term: int
         :return: StaticFlow object containing projected values
         :rtype: StaticFlow
         """
         table = read_csv(Path(self.table_name))
 
         # join the table and the results
-        results = results.join(
-            table, on=self.lookup_on, how="left", rsuffix="_table"
-        )[self.keep_column]
+        results = results.join(table, on=self.lookup_on, how="left", rsuffix="_table")[
+            self.keep_column
+        ]
 
         # Optionally handle nulls
         if self.default_value is not None:
             results = results.replace(np.NaN, self.default_value)
 
         return StaticFlow(input_array=results, label=self.label)
```

### Comparing `predictable-0.0.0a0/src/predictable/core/model.py` & `predictable-0.0.1/predictable/core/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,24 +18,26 @@
 
         :param component: Component to be added to the Model instance
         :type component: CashFlow
         """
         self.components[component.label] = component
 
     def add_components(self, components: List):
-        """This method is used to associate a list of components with the Model instance.
+        """
+        This method is used to associate a list of components with the Model instance.
 
         :param components: List of component to be added to the Model instance
         :type components: List
         """
         for component in components:
             self.components[component.label] = component
 
     def project(self, term: int) -> DataFrame:
-        """This method is used to invoke the project method in each of the associated components.
+        """
+        This method is used to invoke the 'project' method in each component.
 
         :param term: The term over which to project
         :type term: int
         :return: Results of each components project call
         :rtype: DataFrame
         """
         # Create time index
```

### Comparing `predictable-0.0.0a0/src/predictable/core/precision.py` & `predictable-0.0.1/predictable/core/precision.py`

 * *Files identical despite different names*

### Comparing `predictable-0.0.0a0/src/predictable/core/rating_factors.py` & `predictable-0.0.1/predictable/core/rating_factors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import numpy as np
 from numpy.typing import ArrayLike
 from pandas import DataFrame
 
 
 class StaticRatingFactor(np.ndarray):
-    """StaticRatingFactor object created from an Array-Like object. Subclasses numpy.ndarray"""
+    """
+    StaticRatingFactor object created from an Array-Like object.
+    Subclasses numpy.ndarray
+    """
 
     def __new__(cls, input_array: ArrayLike, label: str = None):
         # Input array is an already formed ndarray instance
         # We first cast to be our class type
         obj = np.asarray(input_array).view(cls)
         # add new attributes to the created instance
         obj.label = label
@@ -17,15 +20,16 @@
 
     def __array_finalize__(self, obj):
         if obj is None:
             return
         self.label = getattr(obj, "label", None)
 
     def project(self, term: int, results: DataFrame):
-        """This method is used to handle the projection logic for the component.
+        """
+        This method is used to handle the projection logic for the component.
 
         :param term: Term over which to project
         :type term: int
         :return: StaticRatingFactor object containing projected values
         :rtype: StaticRatingFactor
         """
         if len(self) == term:
@@ -35,15 +39,19 @@
             return StaticRatingFactor(input_array=results, label=self.label)
         elif len(self) > term:
             results = self[: term + 1]
             return StaticRatingFactor(input_array=results, label=self.label)
 
 
 class RatingFactor(np.ndarray):
-    """RatingFactor object created from an Array-Like object. Subclasses numpy.ndarray"""
+    """
+    RatingFactor object created from an Array-Like object.
+
+    Subclasses numpy.ndarray
+    """
 
     def __new__(
         cls,
         input_array: ArrayLike,
         formula=lambda previous: previous,
         label: str = None,
     ):
```

### Comparing `predictable-0.0.0a0/src/predictable/engine/run.py` & `predictable-0.0.1/predictable/engine/run.py`

 * *Files identical despite different names*

### Comparing `predictable-0.0.0a0/tests/test_discounting.py` & `predictable-0.0.1/tests/test_discounting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import pytest
 from pandas import DataFrame
-from src.predictable import DiscountFactors, i_to_v
+from predictable import DiscountFactors, i_to_v
 
 
-@pytest.mark.parametrize(
-    "i, v", [(0.05, 0.952381), (1, 0.5), (1.25, 0.444444)]
-)
+@pytest.mark.parametrize("i, v", [(0.05, 0.952381), (1, 0.5), (1.25, 0.444444)])
 def test_i_to_v(i, v):
     assert round(i_to_v(i), 6) == v
 
 
 def test_discounting_setup():
     d = DiscountFactors(interest_rate=0.05, label="test")
```

### Comparing `predictable-0.0.0a0/tests/test_flows.py` & `predictable-0.0.1/tests/test_flows.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 from pandas import DataFrame
-from src.predictable import CashFlow, StaticFlow
+from predictable import CashFlow, StaticFlow
 
 
 def test_cashflow_setup():
     c = CashFlow(input_array=[100], label="test")
     assert c.label == "test"
     assert len(c) == 1
     assert c.sum() == 100
```

### Comparing `predictable-0.0.0a0/tests/test_lookup.py` & `predictable-0.0.1/tests/test_lookup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from src.predictable import TableLookup
+from predictable import TableLookup
 
 
 def test_tablelookup():
     # Create a new instance
     tbl = TableLookup(
         table_name="test.csv",
         lookup_on="age",
```

### Comparing `predictable-0.0.0a0/tests/test_precision.py` & `predictable-0.0.1/tests/test_precision.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from src.predictable import PRECISION, get_precision, set_precision
+from predictable import PRECISION, get_precision, set_precision
 
 
 def test_get_precision():
     assert get_precision() == PRECISION
 
 
 @pytest.mark.parametrize("input_value, expected", [(2, 2), (2.0, 2), ("2", 2)])
```

### Comparing `predictable-0.0.0a0/tests/test_run.py` & `predictable-0.0.1/tests/test_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from src.predictable import RunConfig, dataclass
+from predictable import RunConfig, dataclass
 
 
 @dataclass
 class ModelPoint:
     test: str
```

### Comparing `predictable-0.0.0a0/.gitignore` & `predictable-0.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `predictable-0.0.0a0/LICENSE` & `predictable-0.0.1/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 
 Copyright (c) 2022 Ratul Maharaj
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `predictable-0.0.0a0/README.md` & `predictable-0.0.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Predictable
 
+[![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+![PyPI](https://img.shields.io/pypi/v/predictable)
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
 [![pytest](https://github.com/RatulMaharaj/predictable/actions/workflows/pytest.yaml/badge.svg?branch=main)](https://github.com/RatulMaharaj/predictable/actions/workflows/pytest.yaml)
+[![build](https://github.com/RatulMaharaj/predictable/actions/workflows/build.yaml/badge.svg?branch=main)](https://github.com/RatulMaharaj/predictable/actions/workflows/build.yaml)
 [![Documentation Status](https://readthedocs.org/projects/predictable/badge/?version=latest)](https://predictable.readthedocs.io/en/latest/?badge=latest)
 
 ## What is it?
 
 A framework for actuarial modelling.
 
 ## Installation
@@ -60,59 +64,71 @@
 # Define reserving relationship
 df["Reserve"] = df["V_cover"] + df["V_expense"] - df["V_premium"]
 
 # Results get returned as a pandas dataframe
 print(df)
 ```
 
-## License
-
-[MIT](https://github.com/RatulMaharaj/predictable/blob/main/LICENSE)
-
 ## Documentation
 
 This project is documented using sphinx and the full documentation can be found at [predictable.readthedocs.io](https://predictable.readthedocs.io/en/latest/).
 
 ## Development & Contibutions
 
 The following steps can be followed to set up a development environment.
 
 1. Clone the project:
 
-```sh
-git clone https://github.com/RatulMaharaj/predictable.git
-cd predictable
-```
+    ```sh
+    git clone https://github.com/RatulMaharaj/predictable.git
+    cd predictable
+    ```
+
+2. Install [hatch](https://hatch.pypa.io/latest/)
+
+    ```sh
+    pipx install hatch
+    ```
+
+3. Enter the default environment (this will activate the default virtual environment and install the project in editable mode).
+
+    ```sh
+    hatch shell default
+    ```
+
+### Testing
 
-2. Create a virtual environment and activate it using:
+This project uses `pytest` for testing purposes. The tests can be found in the `tests` directory. Tests will run after every commit (locally) and on every push (using github actions) but can also be run manually using:
 
 ```sh
-python -m venv venv
-source venv/bin/activate # mac
-venv\Scripts\activate # windows
+hatch run test
 ```
 
-3. Install the project dependencies:
+### Linting
+
+This project is linted using `ruff` and formatted with `black`. The linting and formatting can be run manually using:
 
 ```sh
-pip install -r requirements-dev.txt
+hatch run lint
 ```
 
-In development mode, the package can be installed by running:
-
 ```sh
-pip install -e .
+hatch run format
 ```
 
-4. Install the pre-commit hooks
+### Editing the docs
+
+The documentation for this project can be found in the `docs` directory. The documentation is built using sphinx and can be built locally using:
 
 ```sh
-pre-commit install
+hatch run docs:make
 ```
 
-### Testing
-
-The tests for this project can be found in the `predictable/tests` directory. Tests will run after every commit (locally) and on every push (using github actions) but can also be run manually using:
+You can then serve the documentation locally using:
 
 ```sh
-pytest
+hatch run docs:serve
 ```
+
+## License
+
+[MIT](https://github.com/RatulMaharaj/predictable/blob/main/LICENSE)
```

### Comparing `predictable-0.0.0a0/PKG-INFO` & `predictable-0.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: predictable
-Version: 0.0.0a0
+Version: 0.0.1
 Summary: A framework for actuarial modelling.
 Project-URL: Bug Tracker, https://github.com/RatulMaharaj/predictable/issues
 Project-URL: homepage, https://github.com/RatulMaharaj/predictable
 Project-URL: documentation, https://predictable.readthedocs.io
 Author-email: Ratul Maharaj <ratulmaharaj@gmail.com>
 License: MIT License
         
@@ -12,27 +12,35 @@
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 License-File: LICENSE
-Keywords: actuarial,financial services,modelling,numpy,pandas
+Keywords: actuarial,financial services,modelling,predictable,python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Requires-Dist: numpy
-Requires-Dist: pandas
+Requires-Python: >=3.11
+Requires-Dist: black==23.3.0
+Requires-Dist: numpy==1.24.3
+Requires-Dist: pandas==2.0.1
+Requires-Dist: pre-commit==3.3.1
+Requires-Dist: pydantic==1.10.7
+Requires-Dist: ruff==0.0.264
 Description-Content-Type: text/markdown
 
 # Predictable
 
+[![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+![PyPI](https://img.shields.io/pypi/v/predictable)
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
 [![pytest](https://github.com/RatulMaharaj/predictable/actions/workflows/pytest.yaml/badge.svg?branch=main)](https://github.com/RatulMaharaj/predictable/actions/workflows/pytest.yaml)
+[![build](https://github.com/RatulMaharaj/predictable/actions/workflows/build.yaml/badge.svg?branch=main)](https://github.com/RatulMaharaj/predictable/actions/workflows/build.yaml)
 [![Documentation Status](https://readthedocs.org/projects/predictable/badge/?version=latest)](https://predictable.readthedocs.io/en/latest/?badge=latest)
 
 ## What is it?
 
 A framework for actuarial modelling.
 
 ## Installation
@@ -87,59 +95,71 @@
 # Define reserving relationship
 df["Reserve"] = df["V_cover"] + df["V_expense"] - df["V_premium"]
 
 # Results get returned as a pandas dataframe
 print(df)
 ```
 
-## License
-
-[MIT](https://github.com/RatulMaharaj/predictable/blob/main/LICENSE)
-
 ## Documentation
 
 This project is documented using sphinx and the full documentation can be found at [predictable.readthedocs.io](https://predictable.readthedocs.io/en/latest/).
 
 ## Development & Contibutions
 
 The following steps can be followed to set up a development environment.
 
 1. Clone the project:
 
-```sh
-git clone https://github.com/RatulMaharaj/predictable.git
-cd predictable
-```
+    ```sh
+    git clone https://github.com/RatulMaharaj/predictable.git
+    cd predictable
+    ```
+
+2. Install [hatch](https://hatch.pypa.io/latest/)
+
+    ```sh
+    pipx install hatch
+    ```
+
+3. Enter the default environment (this will activate the default virtual environment and install the project in editable mode).
+
+    ```sh
+    hatch shell default
+    ```
+
+### Testing
 
-2. Create a virtual environment and activate it using:
+This project uses `pytest` for testing purposes. The tests can be found in the `tests` directory. Tests will run after every commit (locally) and on every push (using github actions) but can also be run manually using:
 
 ```sh
-python -m venv venv
-source venv/bin/activate # mac
-venv\Scripts\activate # windows
+hatch run test
 ```
 
-3. Install the project dependencies:
+### Linting
+
+This project is linted using `ruff` and formatted with `black`. The linting and formatting can be run manually using:
 
 ```sh
-pip install -r requirements-dev.txt
+hatch run lint
 ```
 
-In development mode, the package can be installed by running:
-
 ```sh
-pip install -e .
+hatch run format
 ```
 
-4. Install the pre-commit hooks
+### Editing the docs
+
+The documentation for this project can be found in the `docs` directory. The documentation is built using sphinx and can be built locally using:
 
 ```sh
-pre-commit install
+hatch run docs:make
 ```
 
-### Testing
-
-The tests for this project can be found in the `predictable/tests` directory. Tests will run after every commit (locally) and on every push (using github actions) but can also be run manually using:
+You can then serve the documentation locally using:
 
 ```sh
-pytest
+hatch run docs:serve
 ```
+
+## License
+
+[MIT](https://github.com/RatulMaharaj/predictable/blob/main/LICENSE)
```


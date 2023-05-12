# Comparing `tmp/jdiff-0.0.2.tar.gz` & `tmp/jdiff-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdiff-0.0.2.tar", max compression
+gzip compressed data, was "jdiff-0.0.4.tar", max compression
```

## Comparing `jdiff-0.0.2.tar` & `jdiff-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0      153 2022-09-26 09:27:40.321111 jdiff-0.0.2/CHANGELOG.md
--rw-r--r--   0        0        0      533 2022-09-26 09:27:40.321111 jdiff-0.0.2/CONTRIBUTING.md
--rw-r--r--   0        0        0    10174 2022-09-26 09:27:40.321111 jdiff-0.0.2/LICENSE
--rw-r--r--   0        0        0     1910 2022-09-26 09:27:40.321111 jdiff-0.0.2/README.md
--rw-r--r--   0        0        0      165 2022-09-26 09:27:40.321111 jdiff-0.0.2/jdiff/__init__.py
--rw-r--r--   0        0        0    11727 2022-09-26 09:27:40.321111 jdiff-0.0.2/jdiff/check_types.py
--rw-r--r--   0        0        0     4459 2022-09-26 09:27:40.321111 jdiff-0.0.2/jdiff/evaluators.py
--rw-r--r--   0        0        0     3685 2022-09-26 09:27:40.321111 jdiff-0.0.2/jdiff/extract_data.py
--rw-r--r--   0        0        0     4711 2022-09-26 09:27:40.321111 jdiff-0.0.2/jdiff/operator.py
--rw-r--r--   0        0        0        0 2022-09-26 09:27:40.321111 jdiff-0.0.2/jdiff/utils/__init__.py
--rw-r--r--   0        0        0     2895 2022-09-26 09:27:40.321111 jdiff-0.0.2/jdiff/utils/data_normalization.py
--rw-r--r--   0        0        0     3678 2022-09-26 09:27:40.321111 jdiff-0.0.2/jdiff/utils/diff_helpers.py
--rw-r--r--   0        0        0     4778 2022-09-26 09:27:40.321111 jdiff-0.0.2/jdiff/utils/jmespath_parsers.py
--rw-r--r--   0        0        0     3091 2022-09-26 09:27:49.465194 jdiff-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2713 1970-01-01 00:00:00.000000 jdiff-0.0.2/setup.py
--rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 jdiff-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      510 2023-05-12 13:11:58.530808 jdiff-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0      533 2023-05-12 13:11:58.530808 jdiff-0.0.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0    10174 2023-05-12 13:11:58.530808 jdiff-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1910 2023-05-12 13:11:58.530808 jdiff-0.0.4/README.md
+-rw-r--r--   0        0        0      165 2023-05-12 13:11:58.534808 jdiff-0.0.4/jdiff/__init__.py
+-rw-r--r--   0        0        0    11759 2023-05-12 13:11:58.534808 jdiff-0.0.4/jdiff/check_types.py
+-rw-r--r--   0        0        0     4439 2023-05-12 13:11:58.534808 jdiff-0.0.4/jdiff/evaluators.py
+-rw-r--r--   0        0        0     4040 2023-05-12 13:11:58.534808 jdiff-0.0.4/jdiff/extract_data.py
+-rw-r--r--   0        0        0     5066 2023-05-12 13:11:58.534808 jdiff-0.0.4/jdiff/operator.py
+-rw-r--r--   0        0        0        0 2023-05-12 13:11:58.534808 jdiff-0.0.4/jdiff/utils/__init__.py
+-rw-r--r--   0        0        0     2895 2023-05-12 13:11:58.534808 jdiff-0.0.4/jdiff/utils/data_normalization.py
+-rw-r--r--   0        0        0     3678 2023-05-12 13:11:58.534808 jdiff-0.0.4/jdiff/utils/diff_helpers.py
+-rw-r--r--   0        0        0     6775 2023-05-12 13:11:58.534808 jdiff-0.0.4/jdiff/utils/jmespath_parsers.py
+-rw-r--r--   0        0        0     3202 2023-05-12 13:12:15.174885 jdiff-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3052 1970-01-01 00:00:00.000000 jdiff-0.0.4/PKG-INFO
```

### Comparing `jdiff-0.0.2/CONTRIBUTING.md` & `jdiff-0.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jdiff-0.0.2/LICENSE` & `jdiff-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jdiff-0.0.2/README.md` & `jdiff-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `jdiff-0.0.2/jdiff/check_types.py` & `jdiff-0.0.4/jdiff/check_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """CheckType Implementation."""
-from typing import Mapping, Tuple, Dict, Any, Union
+from typing import List, Tuple, Dict, Any, Union
 from abc import ABC, abstractmethod
 from .evaluators import diff_generator, parameter_evaluator, regex_evaluator, operator_evaluator
 
 
 # pylint: disable=arguments-differ
 class CheckType(ABC):
     """Check Type Base Abstract Class."""
@@ -132,15 +132,15 @@
         if not mode:
             raise ValueError("'mode' argument is mandatory for ParameterMatch Check Type.")
         if mode not in mode_options:
             raise ValueError(
                 f"'mode' argument should be one of the following: {', '.join(mode_options)}. You have: {mode}"
             )
 
-    def evaluate(self, params: Dict, value_to_compare: Mapping, mode: str) -> Tuple[Dict, bool]:  # type: ignore[override]
+    def evaluate(self, params: Dict, value_to_compare: List[Dict], mode: str) -> Tuple[Dict, bool]:  # type: ignore[override]
         """Parameter Match evaluator implementation."""
         self._validate(params=params, mode=mode)
         # TODO: we don't use the mode?
         evaluation_result = parameter_evaluator(value_to_compare, params, mode)
         return self.result(evaluation_result)
 
 
@@ -157,30 +157,30 @@
             raise ValueError(f"'regex' argument must be a string. You have: {type(regex)}.")
 
         if not mode:
             raise ValueError("'mode' argument is mandatory for Regex Check Type.")
         if mode not in mode_options:
             raise ValueError(f"'mode' argument should be {mode_options}. You have: {mode}")
 
-    def evaluate(self, regex: str, value_to_compare: Mapping, mode: str) -> Tuple[Dict, bool]:  # type: ignore[override]
+    def evaluate(self, regex: str, value_to_compare: List[Dict[Any, Dict]], mode: str) -> Tuple[Dict, bool]:  # type: ignore[override]
         """Regex Match evaluator implementation."""
         self._validate(regex=regex, mode=mode)
         evaluation_result = regex_evaluator(value_to_compare, regex, mode)
         return self.result(evaluation_result)
 
 
 class OperatorType(CheckType):
     """Operator class implementation."""
 
     @staticmethod
     def _validate(params) -> None:  # type: ignore[override]
         """Validate operator parameters."""
         in_operators = ("is-in", "not-in", "in-range", "not-in-range")
         bool_operators = ("all-same",)
-        number_operators = ("is-gt", "is-lt")
+        number_operators = ("is-gt", "is-lt", "is-ge", "is-le")
         string_operators = ("contains", "not-contains")
         valid_options = (
             in_operators,
             bool_operators,
             number_operators,
             string_operators,
         )
```

### Comparing `jdiff-0.0.2/jdiff/evaluators.py` & `jdiff-0.0.4/jdiff/evaluators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Evaluators."""
 import re
-from typing import Any, Mapping, Dict, Tuple
+from typing import Any, Mapping, Dict, Tuple, List
 from deepdiff import DeepDiff
 from .utils.diff_helpers import get_diff_iterables_items, fix_deepdiff_key_names
 from .operator import Operator
 
 
 def diff_generator(pre_result: Any, post_result: Any) -> Dict:
     """Generates diff between pre and post data based on check definition.
@@ -32,76 +32,76 @@
     iterables_items = get_diff_iterables_items(diff_result)
     if iterables_items:
         result.update(iterables_items)
 
     return fix_deepdiff_key_names(result)
 
 
-def parameter_evaluator(values: Mapping, parameters: Mapping, mode: str) -> Dict:
+def parameter_evaluator(values: List[Dict], parameters: Mapping, mode: str) -> Dict:
     """Parameter Match evaluator engine.
 
     Args:
         values: List of items what we will check the parameters against
         parameters: Dict with the keys and reference values to check
 
     Example:
         values: [{'7.7.7.7': {'peerAddress': '7.7.7.7', 'localAsn': '65130.1100', 'linkType': 'external'}}]
         parameters: {'localAsn': '65130.1100', 'linkType': 'external'}
 
     Returns:
         Dictionary with all the items that have some value not matching the expectations from parameters
     """
     if not isinstance(values, list):
-        raise TypeError("Something went wrong during jmespath parsing. 'values' must be of type List.")
+        raise TypeError("'values' must be of type List.")
 
     result = {}
-    for value in values:
+    for index, value in enumerate(values):
         # value: {'7.7.7.7': {'peerAddress': '7.7.7.7', 'localAsn': '65130.1101', 'linkType': 'externals
         if not isinstance(value, dict):
-            raise TypeError(
-                "Something went wrong during jmespath parsing. ",
-                f"'value' ({value}) must be of type Dict, and it's {type(value)}",
-            )
+            raise TypeError(f"'value' ({value}) must be of type Dict, and it's {type(value)}")
 
         result_item = {}
 
-        # TODO: Why the 'value' dict has always ONE single element? we have to explain
-        # inner_key: '7.7.7.7'
-        inner_key = list(value.keys())[0]
-        # inner_value: [{'peerAddress': '7.7.7.7', 'localAsn': '65130.1101', 'linkType': 'externals'}]
-        inner_value = list(value.values())[0]
+        # When data has been normalized with $key$, get inner key and value
+        if len(value) == 1:
+            # inner_key: '7.7.7.7'
+            inner_key = list(value.keys())[0]
+            # inner_value: [{'peerAddress': '7.7.7.7', 'localAsn': '65130.1101', 'linkType': 'externals'}]
+            value = list(value.values())[0]
+        else:
+            inner_key = index
 
         for parameter_key, parameter_value in parameters.items():
-            if mode == "match" and inner_value[parameter_key] != parameter_value:
-                result_item[parameter_key] = inner_value[parameter_key]
-            elif mode == "no-match" and inner_value[parameter_key] == parameter_value:
-                result_item[parameter_key] = inner_value[parameter_key]
+            if mode == "match" and value[parameter_key] != parameter_value:
+                result_item[parameter_key] = value[parameter_key]
+            elif mode == "no-match" and value[parameter_key] == parameter_value:
+                result_item[parameter_key] = value[parameter_key]
 
         if result_item:
             result[inner_key] = result_item
 
     return result
 
 
-def regex_evaluator(values: Mapping, regex_expression: str, mode: str) -> Dict:
+def regex_evaluator(values: List[Dict[Any, Dict]], regex_expression: str, mode: str) -> Dict:
     """Regex Match evaluator engine."""
     # values: [{'7.7.7.7': {'peerGroup': 'EVPN-OVERLAY-SPINE'}}]
-    # parameter: {'regex': '.*UNDERLAY.*', 'mode': 'include'}
+    # parameter: {'regex': '.*UNDERLAY.*', 'mode': 'match'}
     result = {}
     if not isinstance(values, list):
         raise TypeError("Something went wrong during JMSPath parsing. 'values' must be of type List.")
 
     for item in values:
         for founded_value in item.values():
             for value in founded_value.values():
                 match_result = re.search(regex_expression, value)
-                # Fail if there is not regex match
+                # Fail if there is no regex match for "match" mode
                 if mode == "match" and not match_result:
                     result.update(item)
-                # Fail if there is regex match
+                # Fail if there is regex match for "no-match" mode.
                 elif mode == "no-match" and match_result:
                     result.update(item)
 
     return result
 
 
 def operator_evaluator(reference_data: Mapping, value_to_compare: Mapping) -> Tuple[Dict, bool]:
```

### Comparing `jdiff-0.0.2/jdiff/extract_data.py` & `jdiff-0.0.4/jdiff/extract_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Extract data from JSON. Based on custom JMSPath implementation."""
 import re
 import warnings
-from typing import Mapping, List, Dict, Any, Union
+from typing import Mapping, List, Dict, Any, Union, Optional
 import jmespath
 from .utils.data_normalization import exclude_filter, flatten_list
 from .utils.jmespath_parsers import (
     jmespath_value_parser,
     jmespath_refkey_parser,
     associate_key_of_my_value,
     keys_values_zipper,
+    multi_reference_keys,
 )
 
 
-def extract_data_from_json(data: Union[Mapping, List], path: str = "*", exclude: List = None) -> Any:
+def extract_data_from_json(data: Union[Mapping, List], path: str = "*", exclude: Optional[List] = None) -> Any:
     """Return wanted data from outpdevice data based on the check path. See unit test for complete example.
 
     Get the wanted values to be evaluated if JMESPath expression is defined,
     otherwise use the entire data if jmespath is not defined in check. This covers the "raw" diff type.
     Exclude data not desired to compare.
 
     Notes:
@@ -39,41 +40,44 @@
         warnings.warn("JMSPath cannot be empty string or type 'None'. Path argument reverted to default value '*'")
         path = "*"
 
     if path == "*":
         # return if path is not specified
         return data
 
+    # Multi ref_key
+    if len(re.findall(r"\$.*?\$", path)) > 1:
+        clean_path = path.replace("$", "")
+        values = jmespath.search(f"{clean_path}{' | []' * (path.count('*') - 1)}", data)
+        return keys_values_zipper(multi_reference_keys(path, data), associate_key_of_my_value(clean_path, values))
+
     values = jmespath.search(jmespath_value_parser(path), data)
 
     if values is None:
         raise TypeError("JMSPath returned 'None'. Please, verify your JMSPath regex.")
 
-    # check for multi-nested lists if not found return here
-    if not any(isinstance(i, list) for i in values):
-        return values
-
-    # process elements to check if lists should be flattened
-    for element in values:
-        for item in element:
-            # raise if there is a dict, path must be more specific to extract data
-            if isinstance(item, dict):
-                raise TypeError(
-                    f'Must be list of lists i.e. [["Idle", 75759616], ["Idle", 75759620]]. You have "{values}".'
-                )
-            if isinstance(item, list):
-                values = flatten_list(values)  # flatten list and rewrite values
-                break  # items are the same, need to check only first to see if this is a nested list
-
-    paired_key_value = associate_key_of_my_value(jmespath_value_parser(path), values)
+    # check for multi-nested lists
+    if any(isinstance(i, list) for i in values):
+        # process elements to check if lists should be flattened
+        for element in values:
+            for item in element:
+                # raise if there is a dict, path must be more specific to extract data
+                if isinstance(item, dict):
+                    raise TypeError(
+                        f'Must be list of lists i.e. [["Idle", 75759616], ["Idle", 75759620]]. You have "{values}".'
+                    )
+                if isinstance(item, list):
+                    values = flatten_list(values)  # flatten list and rewrite values
+                    break  # items are the same, need to check only first to see if this is a nested list
 
     # We need to get a list of reference keys - list of strings.
     # Based on the expression or data we might have different data types
     # therefore we need to normalize.
     if re.search(r"\$.*\$", path):
+        paired_key_value = associate_key_of_my_value(jmespath_value_parser(path), values)
         wanted_reference_keys = jmespath.search(jmespath_refkey_parser(path), data)
 
         if isinstance(wanted_reference_keys, dict):  # when wanted_reference_keys is dict() type
             list_of_reference_keys = list(wanted_reference_keys.keys())
         elif any(
             isinstance(element, list) for element in wanted_reference_keys
         ):  # when wanted_reference_keys is a nested list
```

### Comparing `jdiff-0.0.2/jdiff/operator.py` & `jdiff-0.0.4/jdiff/operator.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,17 @@
                     result.append(item)
             # "<", ">", "contains"
             elif not ops[call_ops](evaluated_value, self.reference_data):
                 result.append(item)
 
         ops = {
             ">": operator.gt,
+            ">=": operator.ge,
             "<": operator.lt,
+            "<=": operator.le,
             "is_in": operator.contains,
             "not_in": operator.contains,
             "contains": operator.contains,
             "not_contains": operator.contains,
         }
 
         result = []  # type: List
@@ -95,18 +97,26 @@
         """Not contains operator caller."""
         return self._loop_through_wrapper("not_contains")
 
     def is_gt(self) -> Tuple[List, bool]:
         """Is greather than operator caller."""
         return self._loop_through_wrapper(">")
 
+    def is_ge(self) -> Tuple[List, bool]:
+        """Is greather or equal than operator caller."""
+        return self._loop_through_wrapper(">=")
+
     def is_lt(self) -> Tuple[List, bool]:
         """Is lower than operator caller."""
         return self._loop_through_wrapper("<")
 
+    def is_le(self) -> Tuple[List, bool]:
+        """Is lower or equal than operator caller."""
+        return self._loop_through_wrapper("<=")
+
     def is_in(self) -> Tuple[List, bool]:
         """Is in operator caller."""
         return self._loop_through_wrapper("is_in")
 
     def not_in(self) -> Tuple[List, bool]:
         """Is not in operator caller."""
         return self._loop_through_wrapper("not_in")
```

### Comparing `jdiff-0.0.2/jdiff/utils/data_normalization.py` & `jdiff-0.0.4/jdiff/utils/data_normalization.py`

 * *Files identical despite different names*

### Comparing `jdiff-0.0.2/jdiff/utils/diff_helpers.py` & `jdiff-0.0.4/jdiff/utils/diff_helpers.py`

 * *Files identical despite different names*

### Comparing `jdiff-0.0.2/pyproject.toml` & `jdiff-0.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jdiff"
-version = "v0.0.2"
+version = "v0.0.4"
 description = "A light-weight library to compare structured output from network devices show commands."
 authors = ["Network to Code, LLC <info@networktocode.com>"]
 license = "Apache-2.0"
 homepage = "https://github.com/networktocode/jdiff"
 repository = "https://github.com/networktocode/jdiff"
 readme = "README.md"
 keywords = ["json", "diff", "network"]
@@ -19,15 +19,15 @@
     "CHANGELOG.md",
     "CONTRIBUTING.md",
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7.0"
-deepdiff = "^5.5.0"
+deepdiff = ">=5.5.0 <7.0"
 jmespath = "^0.10.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 requests_mock = "*"
 pyyaml = "*"
 black = "*"
@@ -37,14 +37,15 @@
 bandit = "*"
 invoke = "*"
 toml = "*"
 flake8 = "*"
 mypy = "*"
 mkdocs = "^1.3.1"
 mkdocs-include-markdown-plugin = "^3.6.1"
+importlib-metadata = "<5.0.0"  # https://importlib-metadata.readthedocs.io/en/latest/history.html#v5-0-0
 
 [tool.black]
 line-length = 120
 target-version = ['py37']
 include = '\.pyi?$'
 exclude = '''
 (
```

### Comparing `jdiff-0.0.2/PKG-INFO` & `jdiff-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: jdiff
-Version: 0.0.2
+Version: 0.0.4
 Summary: A light-weight library to compare structured output from network devices show commands.
 Home-page: https://github.com/networktocode/jdiff
 License: Apache-2.0
 Keywords: json,diff,network
 Author: Network to Code, LLC
 Author-email: info@networktocode.com
 Requires-Python: >=3.7.0,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: deepdiff (>=5.5.0,<6.0.0)
+Requires-Dist: deepdiff (>=5.5.0,<7.0)
 Requires-Dist: jmespath (>=0.10.0,<0.11.0)
 Project-URL: Repository, https://github.com/networktocode/jdiff
 Description-Content-Type: text/markdown
 
 # jdiff
 
 `jdiff` is a lightweight Python library allowing you to examine structured data. `jdiff` provides an interface to intelligently compare--via key presense/absense and value comparison--JSON data objects
```


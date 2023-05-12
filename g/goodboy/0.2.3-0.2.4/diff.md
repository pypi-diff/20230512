# Comparing `tmp/goodboy-0.2.3.tar.gz` & `tmp/goodboy-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodboy-0.2.3.tar", max compression
+gzip compressed data, was "goodboy-0.2.4.tar", max compression
```

## Comparing `goodboy-0.2.3.tar` & `goodboy-0.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1058 2021-12-02 13:38:21.559571 goodboy-0.2.3/LICENSE
--rw-r--r--   0        0        0       98 2021-12-02 13:47:07.189233 goodboy-0.2.3/README.md
--rw-r--r--   0        0        0      791 2023-02-17 10:18:17.214273 goodboy-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1461 2023-02-17 10:18:26.382241 goodboy-0.2.3/src/goodboy/__init__.py
--rw-r--r--   0        0        0    10642 2022-04-08 16:28:00.514302 goodboy-0.2.3/src/goodboy/declarative.py
--rw-r--r--   0        0        0     6709 2022-07-20 17:41:53.590813 goodboy-0.2.3/src/goodboy/errors.py
--rw-r--r--   0        0        0     5550 2022-03-30 17:25:03.152622 goodboy-0.2.3/src/goodboy/i18n.py
--rw-r--r--   0        0        0     2635 2022-03-07 17:15:11.940982 goodboy-0.2.3/src/goodboy/locale/en/LC_MESSAGES/goodboy.mo
--rw-r--r--   0        0        0     3927 2021-12-21 14:40:53.775108 goodboy-0.2.3/src/goodboy/locale/en/LC_MESSAGES/goodboy.po
--rw-r--r--   0        0        0     3079 2021-12-21 14:40:37.682436 goodboy-0.2.3/src/goodboy/locale/goodboy.pot
--rw-r--r--   0        0        0     3546 2022-03-07 17:15:11.940982 goodboy-0.2.3/src/goodboy/locale/ru/LC_MESSAGES/goodboy.mo
--rw-r--r--   0        0        0     4841 2021-12-21 14:41:07.831683 goodboy-0.2.3/src/goodboy/locale/ru/LC_MESSAGES/goodboy.po
--rw-r--r--   0        0        0     8233 2022-04-01 16:32:59.620901 goodboy-0.2.3/src/goodboy/messages.py
--rw-r--r--   0        0        0        0 2022-04-08 16:29:46.519612 goodboy-0.2.3/src/goodboy/py.typed
--rw-r--r--   0        0        0     2837 2022-04-01 16:18:30.959803 goodboy-0.2.3/src/goodboy/schema.py
--rw-r--r--   0        0        0        0 2021-12-03 11:40:22.066049 goodboy-0.2.3/src/goodboy/types/__init__.py
--rw-r--r--   0        0        0     7775 2022-04-01 16:18:30.959803 goodboy-0.2.3/src/goodboy/types/dates.py
--rw-r--r--   0        0        0     9227 2023-02-17 10:10:07.205392 goodboy-0.2.3/src/goodboy/types/dicts.py
--rw-r--r--   0        0        0     3509 2022-07-20 18:22:05.699055 goodboy-0.2.3/src/goodboy/types/lists.py
--rw-r--r--   0        0        0     5973 2022-04-01 16:18:30.963803 goodboy-0.2.3/src/goodboy/types/numeric.py
--rw-r--r--   0        0        0      912 2022-04-01 16:18:30.963803 goodboy-0.2.3/src/goodboy/types/python.py
--rw-r--r--   0        0        0     8245 2022-04-01 16:18:30.963803 goodboy-0.2.3/src/goodboy/types/simple.py
--rw-r--r--   0        0        0     1885 2022-04-01 16:18:30.963803 goodboy-0.2.3/src/goodboy/types/variants.py
--rw-r--r--   0        0        0     2218 2021-12-30 06:48:30.833424 goodboy-0.2.3/src/goodboy/validator.py
--rw-r--r--   0        0        0      927 1970-01-01 00:00:00.000000 goodboy-0.2.3/setup.py
--rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 goodboy-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1058 2021-12-02 13:38:21.559571 goodboy-0.2.4/LICENSE
+-rw-r--r--   0        0        0       98 2021-12-02 13:47:07.189233 goodboy-0.2.4/README.md
+-rw-r--r--   0        0        0      791 2023-05-12 13:08:01.247501 goodboy-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1497 2023-05-12 13:07:53.911259 goodboy-0.2.4/src/goodboy/__init__.py
+-rw-r--r--   0        0        0    10642 2022-04-08 16:28:00.514302 goodboy-0.2.4/src/goodboy/declarative.py
+-rw-r--r--   0        0        0     6709 2022-07-20 17:41:53.590813 goodboy-0.2.4/src/goodboy/errors.py
+-rw-r--r--   0        0        0     5550 2022-03-30 17:25:03.152622 goodboy-0.2.4/src/goodboy/i18n.py
+-rw-r--r--   0        0        0     2635 2022-03-07 17:15:11.940982 goodboy-0.2.4/src/goodboy/locale/en/LC_MESSAGES/goodboy.mo
+-rw-r--r--   0        0        0     3927 2021-12-21 14:40:53.775108 goodboy-0.2.4/src/goodboy/locale/en/LC_MESSAGES/goodboy.po
+-rw-r--r--   0        0        0     3079 2021-12-21 14:40:37.682436 goodboy-0.2.4/src/goodboy/locale/goodboy.pot
+-rw-r--r--   0        0        0     3546 2022-03-07 17:15:11.940982 goodboy-0.2.4/src/goodboy/locale/ru/LC_MESSAGES/goodboy.mo
+-rw-r--r--   0        0        0     4841 2021-12-21 14:41:07.831683 goodboy-0.2.4/src/goodboy/locale/ru/LC_MESSAGES/goodboy.po
+-rw-r--r--   0        0        0     8272 2023-05-12 13:03:17.744041 goodboy-0.2.4/src/goodboy/messages.py
+-rw-r--r--   0        0        0        0 2022-04-08 16:29:46.519612 goodboy-0.2.4/src/goodboy/py.typed
+-rw-r--r--   0        0        0     2837 2022-04-01 16:18:30.959803 goodboy-0.2.4/src/goodboy/schema.py
+-rw-r--r--   0        0        0        0 2021-12-03 11:40:22.066049 goodboy-0.2.4/src/goodboy/types/__init__.py
+-rw-r--r--   0        0        0     7775 2022-04-01 16:18:30.959803 goodboy-0.2.4/src/goodboy/types/dates.py
+-rw-r--r--   0        0        0     9227 2023-02-17 10:10:07.205392 goodboy-0.2.4/src/goodboy/types/dicts.py
+-rw-r--r--   0        0        0     3509 2022-07-20 18:22:05.699055 goodboy-0.2.4/src/goodboy/types/lists.py
+-rw-r--r--   0        0        0     7720 2023-05-12 13:06:00.167174 goodboy-0.2.4/src/goodboy/types/numeric.py
+-rw-r--r--   0        0        0      912 2022-04-01 16:18:30.963803 goodboy-0.2.4/src/goodboy/types/python.py
+-rw-r--r--   0        0        0     8245 2022-04-01 16:18:30.963803 goodboy-0.2.4/src/goodboy/types/simple.py
+-rw-r--r--   0        0        0     1885 2022-04-01 16:18:30.963803 goodboy-0.2.4/src/goodboy/types/variants.py
+-rw-r--r--   0        0        0     2218 2021-12-30 06:48:30.833424 goodboy-0.2.4/src/goodboy/validator.py
+-rw-r--r--   0        0        0      927 1970-01-01 00:00:00.000000 goodboy-0.2.4/setup.py
+-rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 goodboy-0.2.4/PKG-INFO
```

### Comparing `goodboy-0.2.3/LICENSE` & `goodboy-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `goodboy-0.2.3/pyproject.toml` & `goodboy-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "goodboy"
-version = "0.2.3"
+version = "0.2.4"
 description = "Data validation tool"
 license = "MIT"
 authors = ["Maxim Andryunin <maxim.andryunin@gmail.com>"]
 readme = "README.md"
 include = [
     "src/goodboy/locale/**/*.mo"
 ]
```

### Comparing `goodboy-0.2.3/src/goodboy/__init__.py` & `goodboy-0.2.4/src/goodboy/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,29 +18,30 @@
     SchemaErrorMixin,
     SchemaRulesMixin,
     SchemaWithUtils,
 )
 from goodboy.types.dates import Date, DateTime
 from goodboy.types.dicts import Dict, Key
 from goodboy.types.lists import List
-from goodboy.types.numeric import Float, Int
+from goodboy.types.numeric import DecimalSchema, Float, Int
 from goodboy.types.python import CallableValue
 from goodboy.types.simple import AnyValue, Bool, NoneValue, Str
 from goodboy.types.variants import AnyOf
 from goodboy.validator import Result, Validator, validate
 
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 
 __all__ = [
     "AnyOf",
     "AnyValue",
     "Bool",
     "CallableValue",
     "Date",
     "DateTime",
+    "DecimalSchema",
     "DeclarativeBuilder",
     "Dict",
     "Error",
     "ErrorFormatter",
     "Float",
     "I18nErrorFormatter",
     "Int",
```

### Comparing `goodboy-0.2.3/src/goodboy/declarative.py` & `goodboy-0.2.4/src/goodboy/declarative.py`

 * *Files identical despite different names*

### Comparing `goodboy-0.2.3/src/goodboy/errors.py` & `goodboy-0.2.4/src/goodboy/errors.py`

 * *Files identical despite different names*

### Comparing `goodboy-0.2.3/src/goodboy/i18n.py` & `goodboy-0.2.4/src/goodboy/i18n.py`

 * *Files identical despite different names*

### Comparing `goodboy-0.2.3/src/goodboy/locale/en/LC_MESSAGES/goodboy.mo` & `goodboy-0.2.4/src/goodboy/locale/en/LC_MESSAGES/goodboy.mo`

 * *Files identical despite different names*

### Comparing `goodboy-0.2.3/src/goodboy/locale/en/LC_MESSAGES/goodboy.po` & `goodboy-0.2.4/src/goodboy/locale/en/LC_MESSAGES/goodboy.po`

 * *Files identical despite different names*

### Comparing `goodboy-0.2.3/src/goodboy/locale/goodboy.pot` & `goodboy-0.2.4/src/goodboy/locale/goodboy.pot`

 * *Files identical despite different names*

### Comparing `goodboy-0.2.3/src/goodboy/locale/ru/LC_MESSAGES/goodboy.mo` & `goodboy-0.2.4/src/goodboy/locale/ru/LC_MESSAGES/goodboy.mo`

 * *Files identical despite different names*

### Comparing `goodboy-0.2.3/src/goodboy/locale/ru/LC_MESSAGES/goodboy.po` & `goodboy-0.2.4/src/goodboy/locale/ru/LC_MESSAGES/goodboy.po`

 * *Files identical despite different names*

### Comparing `goodboy-0.2.3/src/goodboy/messages.py` & `goodboy-0.2.4/src/goodboy/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,14 +218,15 @@
     Message("dict", json="object"),
     Message("list", json="array"),
     Message("str", json="string"),
     Message("date", json="string"),
     Message("datetime", json="string"),
     Message("int", json="integer"),
     Message("float", json="number"),
+    Message("decimal", json="number"),
     Message("bool", json="boolean"),
 ]
 
 _TYPE_NAMES = MessageCollection({m.render(): m for m in _TYPE_NAMES_LIST})
 
 
 def type_name(python_type_name: str) -> Message:
```

### Comparing `goodboy-0.2.3/src/goodboy/schema.py` & `goodboy-0.2.4/src/goodboy/schema.py`

 * *Files identical despite different names*

### Comparing `goodboy-0.2.3/src/goodboy/types/dates.py` & `goodboy-0.2.4/src/goodboy/types/dates.py`

 * *Files identical despite different names*

### Comparing `goodboy-0.2.3/src/goodboy/types/dicts.py` & `goodboy-0.2.4/src/goodboy/types/dicts.py`

 * *Files identical despite different names*

### Comparing `goodboy-0.2.3/src/goodboy/types/lists.py` & `goodboy-0.2.4/src/goodboy/types/lists.py`

 * *Files identical despite different names*

### Comparing `goodboy-0.2.3/src/goodboy/types/numeric.py` & `goodboy-0.2.4/src/goodboy/types/numeric.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from abc import abstractmethod
+from decimal import Decimal, InvalidOperation
 from typing import Any, Generic, Optional, TypeVar
 
 from goodboy.errors import Error
 from goodboy.messages import DEFAULT_MESSAGES, MessageCollectionType, type_name
 from goodboy.schema import Rule, SchemaWithUtils
 
 N = TypeVar("N")
@@ -122,14 +123,61 @@
             return float(value), []
         else:
             return None, [
                 self._error("unexpected_type", {"expected_type": type_name("float")})
             ]
 
 
+class DecimalSchema(NumericBase[Decimal]):
+    """
+    Accept ``decimal`` values. Integer and float values are converted to decimals.
+
+    :param allow_none: If true, value is allowed to be ``None``.
+    :param messages: Override error messages.
+    :param rules: Custom validation rules.
+    :param less_than: Accept only values less than option value.
+    :param less_or_equal_to: Accept only values less than or equal to option value.
+    :param greater_than: Accept only values greater than option value.
+    :param greater_or_equal_to: Accept only values greater than or equal to option
+        value.
+    :param allowed: Allow only certain values.
+    """
+
+    def _typecast(
+        self, input: Any, context: dict[str, Any] = {}
+    ) -> tuple[Optional[Decimal], list[Error]]:
+        if isinstance(input, Decimal):
+            return input, []
+
+        if isinstance(input, int):
+            return Decimal(input), []
+
+        if not isinstance(input, str):
+            return None, [
+                self._error("unexpected_type", {"expected_type": type_name("decimal")})
+            ]
+
+        try:
+            return Decimal(input), []
+        except InvalidOperation:
+            return None, [self._error("invalid_numeric_format")]
+
+    def _validate_exact_type(self, value: Any) -> tuple[Optional[Decimal], list[Error]]:
+        if isinstance(value, Decimal):
+            return value, []
+        elif isinstance(value, int):
+            return Decimal(value), []
+        elif isinstance(value, float):
+            return Decimal(value), []
+        else:
+            return None, [
+                self._error("unexpected_type", {"expected_type": type_name("decimal")})
+            ]
+
+
 class Int(NumericBase[int]):
     """
     Accept ``int`` values.
 
     When type casting enabled, strings and other values with magic method
     `__int__ <https://docs.python.org/3/reference/datamodel.html#object.__int__>`_ are
     converted to integers.
```

### Comparing `goodboy-0.2.3/src/goodboy/types/python.py` & `goodboy-0.2.4/src/goodboy/types/python.py`

 * *Files identical despite different names*

### Comparing `goodboy-0.2.3/src/goodboy/types/simple.py` & `goodboy-0.2.4/src/goodboy/types/simple.py`

 * *Files identical despite different names*

### Comparing `goodboy-0.2.3/src/goodboy/types/variants.py` & `goodboy-0.2.4/src/goodboy/types/variants.py`

 * *Files identical despite different names*

### Comparing `goodboy-0.2.3/src/goodboy/validator.py` & `goodboy-0.2.4/src/goodboy/validator.py`

 * *Files identical despite different names*

### Comparing `goodboy-0.2.3/setup.py` & `goodboy-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'goodboy': ['locale/*', 'locale/en/LC_MESSAGES/*', 'locale/ru/LC_MESSAGES/*']}
 
 extras_require = \
 {':python_version >= "3.6" and python_version < "3.8"': ['typing-extensions>=4.0']}
 
 setup_kwargs = {
     'name': 'goodboy',
-    'version': '0.2.3',
+    'version': '0.2.4',
     'description': 'Data validation tool',
     'long_description': '# Goodboy: Data Validation for Python\n\nThis project is currently in an early stage of development.',
     'author': 'Maxim Andryunin',
     'author_email': 'maxim.andryunin@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `goodboy-0.2.3/PKG-INFO` & `goodboy-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodboy
-Version: 0.2.3
+Version: 0.2.4
 Summary: Data validation tool
 License: MIT
 Author: Maxim Andryunin
 Author-email: maxim.andryunin@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


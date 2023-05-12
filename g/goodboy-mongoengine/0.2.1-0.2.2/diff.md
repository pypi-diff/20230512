# Comparing `tmp/goodboy_mongoengine-0.2.1.tar.gz` & `tmp/goodboy_mongoengine-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodboy_mongoengine-0.2.1.tar", max compression
+gzip compressed data, was "goodboy_mongoengine-0.2.2.tar", max compression
```

## Comparing `goodboy_mongoengine-0.2.1.tar` & `goodboy_mongoengine-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1058 2023-02-16 15:30:11.588202 goodboy_mongoengine-0.2.1/LICENSE
--rw-r--r--   0        0        0      116 2023-02-16 15:31:05.305377 goodboy_mongoengine-0.2.1/README.md
--rw-r--r--   0        0        0      845 2023-02-22 13:51:07.498572 goodboy_mongoengine-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1082 2023-02-22 13:51:14.090644 goodboy_mongoengine-0.2.1/src/goodboy_mongoengine/__init__.py
--rw-r--r--   0        0        0     5059 2023-02-17 10:40:12.239145 goodboy_mongoengine-0.2.1/src/goodboy_mongoengine/document.py
--rw-r--r--   0        0        0     5747 2023-02-17 14:04:38.341603 goodboy_mongoengine-0.2.1/src/goodboy_mongoengine/document_key.py
--rw-r--r--   0        0        0     2810 2023-02-17 10:41:12.271828 goodboy_mongoengine-0.2.1/src/goodboy_mongoengine/field.py
--rw-r--r--   0        0        0     2958 2023-02-19 15:37:20.894947 goodboy_mongoengine-0.2.1/src/goodboy_mongoengine/field_schemas.py
--rw-r--r--   0        0        0      110 2023-02-16 15:41:00.519812 goodboy_mongoengine-0.2.1/src/goodboy_mongoengine/messages.py
--rw-r--r--   0        0        0        0 2023-02-16 15:30:11.592202 goodboy_mongoengine-0.2.1/src/goodboy_mongoengine/py.typed
--rw-r--r--   0        0        0     1599 2023-02-19 15:33:19.539066 goodboy_mongoengine-0.2.1/src/goodboy_mongoengine/schemas.py
--rw-r--r--   0        0        0      990 1970-01-01 00:00:00.000000 goodboy_mongoengine-0.2.1/setup.py
--rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 goodboy_mongoengine-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1058 2023-02-16 15:30:11.588202 goodboy_mongoengine-0.2.2/LICENSE
+-rw-r--r--   0        0        0      116 2023-02-16 15:31:05.305377 goodboy_mongoengine-0.2.2/README.md
+-rw-r--r--   0        0        0      845 2023-05-12 13:20:55.452456 goodboy_mongoengine-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1082 2023-05-12 13:20:52.300408 goodboy_mongoengine-0.2.2/src/goodboy_mongoengine/__init__.py
+-rw-r--r--   0        0        0     5059 2023-02-17 10:40:12.239145 goodboy_mongoengine-0.2.2/src/goodboy_mongoengine/document.py
+-rw-r--r--   0        0        0     5747 2023-02-17 14:04:38.341603 goodboy_mongoengine-0.2.2/src/goodboy_mongoengine/document_key.py
+-rw-r--r--   0        0        0     2810 2023-02-17 10:41:12.271828 goodboy_mongoengine-0.2.2/src/goodboy_mongoengine/field.py
+-rw-r--r--   0        0        0     3301 2023-05-12 13:16:24.639900 goodboy_mongoengine-0.2.2/src/goodboy_mongoengine/field_schemas.py
+-rw-r--r--   0        0        0      110 2023-02-16 15:41:00.519812 goodboy_mongoengine-0.2.2/src/goodboy_mongoengine/messages.py
+-rw-r--r--   0        0        0        0 2023-02-16 15:30:11.592202 goodboy_mongoengine-0.2.2/src/goodboy_mongoengine/py.typed
+-rw-r--r--   0        0        0     1599 2023-02-19 15:33:19.539066 goodboy_mongoengine-0.2.2/src/goodboy_mongoengine/schemas.py
+-rw-r--r--   0        0        0      990 1970-01-01 00:00:00.000000 goodboy_mongoengine-0.2.2/setup.py
+-rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 goodboy_mongoengine-0.2.2/PKG-INFO
```

### Comparing `goodboy_mongoengine-0.2.1/LICENSE` & `goodboy_mongoengine-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `goodboy_mongoengine-0.2.1/pyproject.toml` & `goodboy_mongoengine-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "goodboy-mongoengine"
-version = "0.2.1"
+version = "0.2.2"
 description = "Data validation tool for MongoEngine"
 license = "MIT"
 authors = ["Maxim Andryunin <maxim.andryunin@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `goodboy_mongoengine-0.2.1/src/goodboy_mongoengine/__init__.py` & `goodboy_mongoengine-0.2.2/src/goodboy_mongoengine/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     FieldSchemaBuilderError,
     FieldSchemaFactory,
     field_schema_builder,
 )
 from goodboy_mongoengine.messages import DEFAULT_MESSAGES
 from goodboy_mongoengine.schemas import ObjectIdSchema
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 __all__ = [
     "DEFAULT_MESSAGES",
     "document_key_builder",
     "DocumentFieldKey",
     "DocumentInstanceProxy",
     "DocumentKey",
```

### Comparing `goodboy_mongoengine-0.2.1/src/goodboy_mongoengine/document.py` & `goodboy_mongoengine-0.2.2/src/goodboy_mongoengine/document.py`

 * *Files identical despite different names*

### Comparing `goodboy_mongoengine-0.2.1/src/goodboy_mongoengine/document_key.py` & `goodboy_mongoengine-0.2.2/src/goodboy_mongoengine/document_key.py`

 * *Files identical despite different names*

### Comparing `goodboy_mongoengine-0.2.1/src/goodboy_mongoengine/field.py` & `goodboy_mongoengine-0.2.2/src/goodboy_mongoengine/field.py`

 * *Files identical despite different names*

### Comparing `goodboy_mongoengine-0.2.1/src/goodboy_mongoengine/field_schemas.py` & `goodboy_mongoengine-0.2.2/src/goodboy_mongoengine/field_schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,23 @@
         return gb.Int(
             allow_none=not field.required,
             less_than=field.max_value,
             greater_than=field.min_value,
         )
 
 
+class DecimalFieldSchemaFactory(FieldSchemaFactory):
+    def build(self, field: me.Decimal128Field) -> gb.DecimalSchema:
+        return gb.DecimalSchema(
+            allow_none=not field.required,
+            less_than=field.max_value,
+            greater_than=field.min_value,
+        )
+
+
 class ObjectIdFieldSchemaFactory(FieldSchemaFactory):
     def build(self, field: me.ObjectIdField) -> ObjectIdSchema:
         return ObjectIdSchema(allow_none=not field.required)
 
 
 class DictFieldFieldSchemaFactory(FieldSchemaFactory):
     def build(self, field: me.DictField) -> gb.Dict:
@@ -61,14 +70,15 @@
 
 ME_TYPE_MAPPING: dict[Type[BaseField], FieldSchemaFactory] = {
     me.StringField: StringFieldSchemaFactory(),
     me.DictField: DictFieldFieldSchemaFactory(),
     me.BooleanField: BooleanFieldSchemaFactory(),
     me.IntField: IntFieldSchemaFactory(),
     me.ObjectIdField: ObjectIdFieldSchemaFactory(),
+    me.Decimal128Field: DecimalFieldSchemaFactory(),
 }
 
 
 class FieldSchemaBuilderError(Exception):
     pass
```

### Comparing `goodboy_mongoengine-0.2.1/src/goodboy_mongoengine/schemas.py` & `goodboy_mongoengine-0.2.2/src/goodboy_mongoengine/schemas.py`

 * *Files identical despite different names*

### Comparing `goodboy_mongoengine-0.2.1/setup.py` & `goodboy_mongoengine-0.2.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['goodboy>=0.2,<0.3', 'mongoengine']
 
 extras_require = \
 {':python_version >= "3.6" and python_version < "3.8"': ['typing-extensions>=4.0']}
 
 setup_kwargs = {
     'name': 'goodboy-mongoengine',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'Data validation tool for MongoEngine',
     'long_description': '# Goodboy-MongoEngine: Data Validation for MongoEngine\n\nThis project is currently in an early stage of development.\n',
     'author': 'Maxim Andryunin',
     'author_email': 'maxim.andryunin@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `goodboy_mongoengine-0.2.1/PKG-INFO` & `goodboy_mongoengine-0.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodboy-mongoengine
-Version: 0.2.1
+Version: 0.2.2
 Summary: Data validation tool for MongoEngine
 License: MIT
 Author: Maxim Andryunin
 Author-email: maxim.andryunin@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/django_choices_field-2.1.1.tar.gz` & `tmp/django_choices_field-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_choices_field-2.1.1.tar", max compression
+gzip compressed data, was "django_choices_field-2.1.2.tar", max compression
```

## Comparing `django_choices_field-2.1.1.tar` & `django_choices_field-2.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1077 2023-04-21 18:21:00.361194 django_choices_field-2.1.1/LICENSE
--rw-r--r--   0        0        0     2086 2023-04-21 18:21:00.365195 django_choices_field-2.1.1/README.md
--rw-r--r--   0        0        0      124 2023-04-21 18:21:00.365195 django_choices_field-2.1.1/django_choices_field/__init__.py
--rw-r--r--   0        0        0     3055 2023-04-21 18:21:00.365195 django_choices_field-2.1.1/django_choices_field/fields.py
--rw-r--r--   0        0        0     5609 2023-04-21 18:21:00.365195 django_choices_field-2.1.1/django_choices_field/fields.pyi
--rw-r--r--   0        0        0     3257 2023-04-21 18:21:00.365195 django_choices_field-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     3612 1970-01-01 00:00:00.000000 django_choices_field-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-12 17:14:33.664796 django_choices_field-2.1.2/LICENSE
+-rw-r--r--   0        0        0     2086 2023-05-12 17:14:33.664796 django_choices_field-2.1.2/README.md
+-rw-r--r--   0        0        0      124 2023-05-12 17:14:33.664796 django_choices_field-2.1.2/django_choices_field/__init__.py
+-rw-r--r--   0        0        0     3055 2023-05-12 17:14:33.664796 django_choices_field-2.1.2/django_choices_field/fields.py
+-rw-r--r--   0        0        0     4848 2023-05-12 17:14:33.664796 django_choices_field-2.1.2/django_choices_field/fields.pyi
+-rw-r--r--   0        0        0     3257 2023-05-12 17:14:33.668796 django_choices_field-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3612 1970-01-01 00:00:00.000000 django_choices_field-2.1.2/PKG-INFO
```

### Comparing `django_choices_field-2.1.1/LICENSE` & `django_choices_field-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_choices_field-2.1.1/README.md` & `django_choices_field-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `django_choices_field-2.1.1/django_choices_field/fields.py` & `django_choices_field-2.1.2/django_choices_field/fields.py`

 * *Files identical despite different names*

### Comparing `django_choices_field-2.1.1/django_choices_field/fields.pyi` & `django_choices_field-2.1.2/django_choices_field/fields.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 from typing import (
     Any,
     Callable,
+    Dict,
     Generic,
     Iterable,
     Literal,
     Optional,
     TypeVar,
     overload,
 )
 
 from django.db.models import Field, IntegerChoices, TextChoices
+from typing_extensions import TypeAlias
 
-_Choice = ...
-_ChoiceNamedGroup = ...
-_FieldChoices = ...
-_ValidatorCallable = ...
-_ErrorMessagesToOverride = ...
+_ValidatorCallable: TypeAlias = Callable[..., None]
+_ErrorMessagesToOverride: TypeAlias = Dict[str, Any]
 
-_C = TypeVar("_C", bound="Optional[TextChoices]")
+_C = TypeVar("_C", bound=Optional[TextChoices])
 
 class TextChoicesField(Generic[_C], Field[_C, _C]):
     choices_enum: type[_C]
     @overload
-    def __init__(
-        self: TextChoicesField[_C],
+    def __new__(
+        cls,
         choices_enum: type[_C],
         verbose_name: str | None = ...,
         name: str | None = ...,
         primary_key: bool = ...,
         max_length: int | None = ...,
         unique: bool = ...,
         blank: bool = ...,
@@ -46,18 +45,18 @@
         validators: Iterable[_ValidatorCallable] = ...,
         error_messages: _ErrorMessagesToOverride | None = ...,
         path: str | Callable[..., str] = ...,
         match: str | None = ...,
         recursive: bool = ...,
         allow_files: bool = ...,
         allow_folders: bool = ...,
-    ) -> None: ...
+    ) -> TextChoicesField[_C]: ...
     @overload
-    def __init__(
-        self: TextChoicesField[_C | None],
+    def __new__(
+        cls,
         choices_enum: type[_C],
         verbose_name: str | None = ...,
         name: str | None = ...,
         primary_key: bool = ...,
         max_length: int | None = ...,
         unique: bool = ...,
         blank: bool = ...,
@@ -76,39 +75,23 @@
         validators: Iterable[_ValidatorCallable] = ...,
         error_messages: _ErrorMessagesToOverride | None = ...,
         path: str | Callable[..., str] = ...,
         match: str | None = ...,
         recursive: bool = ...,
         allow_files: bool = ...,
         allow_folders: bool = ...,
-    ) -> None: ...
-    @overload
-    def __new__(
-        cls,
-        choices_enum: type[_C],
-        *args: Any,
-        null: Literal[False] = ...,
-        **kwargs: Any,
-    ) -> TextChoicesField[_C]: ...
-    @overload
-    def __new__(
-        cls,
-        choices_enum: type[_C],
-        *args: Any,
-        null: Literal[True],
-        **kwargs: Any,
     ) -> TextChoicesField[_C | None]: ...
 
-_I = TypeVar("_I", bound="Optional[IntegerChoices]")
+_I = TypeVar("_I", bound=Optional[IntegerChoices])
 
 class IntegerChoicesField(Generic[_I], Field[_I, _I]):
     choices_enum: type[_I]
     @overload
-    def __init__(
-        self: IntegerChoicesField[_I],
+    def __new__(
+        cls,
         choices_enum: type[_I],
         verbose_name: str | None = ...,
         name: str | None = ...,
         primary_key: bool = ...,
         max_length: int | None = ...,
         unique: bool = ...,
         blank: bool = ...,
@@ -127,18 +110,18 @@
         validators: Iterable[_ValidatorCallable] = ...,
         error_messages: _ErrorMessagesToOverride | None = ...,
         path: str | Callable[..., str] = ...,
         match: str | None = ...,
         recursive: bool = ...,
         allow_files: bool = ...,
         allow_folders: bool = ...,
-    ) -> None: ...
+    ) -> IntegerChoicesField[_I]: ...
     @overload
-    def __init__(
-        self: IntegerChoicesField[_I | None],
+    def __new__(
+        cls,
         choices_enum: type[_I],
         verbose_name: str | None = ...,
         name: str | None = ...,
         primary_key: bool = ...,
         max_length: int | None = ...,
         unique: bool = ...,
         blank: bool = ...,
@@ -157,24 +140,8 @@
         validators: Iterable[_ValidatorCallable] = ...,
         error_messages: _ErrorMessagesToOverride | None = ...,
         path: str | Callable[..., str] = ...,
         match: str | None = ...,
         recursive: bool = ...,
         allow_files: bool = ...,
         allow_folders: bool = ...,
-    ) -> None: ...
-    @overload
-    def __new__(
-        cls,
-        choices_enum: type[_I],
-        *args: Any,
-        null: Literal[False] = ...,
-        **kwargs: Any,
-    ) -> IntegerChoicesField[_I]: ...
-    @overload
-    def __new__(
-        cls,
-        choices_enum: type[_I],
-        *args: Any,
-        null: Literal[True],
-        **kwargs: Any,
     ) -> IntegerChoicesField[_I | None]: ...
```

### Comparing `django_choices_field-2.1.1/pyproject.toml` & `django_choices_field-2.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-choices-field"
-version = "2.1.1"
+version = "2.1.2"
 description = "Django field that set/get django's new TextChoices/IntegerChoices enum."
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bellini666/django-choices-field"
 repository = "https://github.com/bellini666/django-choices-field"
 documentation = "https://django-choices-field.readthedocs.io"
@@ -37,15 +37,15 @@
 black = "^23.3.0"
 codecov = "^2.1.11"
 django = "^4.0"
 django-types = "^0.17.0"
 pytest = "^7.1.2"
 pytest-cov = "^4.0.0"
 pytest-django = "^4.2.0"
-ruff = "^0.0.262"
+ruff = "^0.0.265"
 
 [tool.black]
 line-length = 100
 target-version = ['py38']
 preview = true
 exclude = '''
 /(
```

### Comparing `django_choices_field-2.1.1/PKG-INFO` & `django_choices_field-2.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-choices-field
-Version: 2.1.1
+Version: 2.1.2
 Summary: Django field that set/get django's new TextChoices/IntegerChoices enum.
 Home-page: https://github.com/bellini666/django-choices-field
 License: MIT
 Keywords: django,enum
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
```


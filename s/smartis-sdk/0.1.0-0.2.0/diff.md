# Comparing `tmp/smartis_sdk-0.1.0.tar.gz` & `tmp/smartis_sdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartis_sdk-0.1.0.tar", max compression
+gzip compressed data, was "smartis_sdk-0.2.0.tar", max compression
```

## Comparing `smartis_sdk-0.1.0.tar` & `smartis_sdk-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2023-05-11 10:40:57.750065 smartis_sdk-0.1.0/LICENSE
--rw-r--r--   0        0        0       27 2023-05-11 10:42:26.070440 smartis_sdk-0.1.0/README.md
--rw-r--r--   0        0        0     1199 2023-05-11 19:10:03.894612 smartis_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      409 2023-05-11 12:00:43.282493 smartis_sdk-0.1.0/src/smartis_sdk/__init__.py
--rw-r--r--   0        0        0     5899 2023-05-11 15:55:02.746357 smartis_sdk-0.1.0/src/smartis_sdk/client.py
--rw-r--r--   0        0        0     1303 2023-05-11 11:59:04.485496 smartis_sdk-0.1.0/src/smartis_sdk/common.py
--rw-r--r--   0        0        0     3202 2023-05-11 15:56:39.747233 smartis_sdk-0.1.0/src/smartis_sdk/entity.py
--rw-r--r--   0        0        0      169 2023-05-11 08:47:15.864966 smartis_sdk-0.1.0/src/smartis_sdk/utils.py
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 smartis_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-11 10:40:57.750065 smartis_sdk-0.2.0/LICENSE
+-rw-r--r--   0        0        0       27 2023-05-11 10:42:26.070440 smartis_sdk-0.2.0/README.md
+-rw-r--r--   0        0        0     1199 2023-05-12 02:25:16.269680 smartis_sdk-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      385 2023-05-12 02:24:39.116163 smartis_sdk-0.2.0/src/smartis_sdk/__init__.py
+-rw-r--r--   0        0        0     5899 2023-05-11 15:55:02.746357 smartis_sdk-0.2.0/src/smartis_sdk/client.py
+-rw-r--r--   0        0        0     1303 2023-05-11 11:59:04.485496 smartis_sdk-0.2.0/src/smartis_sdk/common.py
+-rw-r--r--   0        0        0     3135 2023-05-12 02:22:17.878788 smartis_sdk-0.2.0/src/smartis_sdk/entity.py
+-rw-r--r--   0        0        0      169 2023-05-11 08:47:15.864966 smartis_sdk-0.2.0/src/smartis_sdk/utils.py
+-rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 smartis_sdk-0.2.0/PKG-INFO
```

### Comparing `smartis_sdk-0.1.0/LICENSE` & `smartis_sdk-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smartis_sdk-0.1.0/pyproject.toml` & `smartis_sdk-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smartis_sdk"
-version = "0.1.0"
+version = "0.2.0"
 description = "SDK для Smartis API"
 license = "MIT"
 authors = ["viktor <vi.dave@yandex.ru>"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
```

### Comparing `smartis_sdk-0.1.0/src/smartis_sdk/client.py` & `smartis_sdk-0.2.0/src/smartis_sdk/client.py`

 * *Files identical despite different names*

### Comparing `smartis_sdk-0.1.0/src/smartis_sdk/common.py` & `smartis_sdk-0.2.0/src/smartis_sdk/common.py`

 * *Files identical despite different names*

### Comparing `smartis_sdk-0.1.0/src/smartis_sdk/entity.py` & `smartis_sdk-0.2.0/src/smartis_sdk/entity.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-from abc import abstractmethod
 from datetime import datetime
 
 from pydantic import BaseModel
 
 from .common import AttributionModel, GroupBy, TypeReport, FilterCategory
 from .utils import normalize_date
 
@@ -87,15 +86,14 @@
 class Filter:
     def __init__(self, category: FilterCategory, value: int, operand: str = "="):
         self.category = category.value
         self.value = value
         self.operand = operand
 
 
-@abstractmethod
 class Payload:
     """Базовый класс параметров для генерации параметров к запросам"""
 
     def __init__(self, project: str, metrics: [str], datetime_from: datetime, datetime_to: datetime,
                  group_by: GroupBy, attribution: Attribution, type_report: TypeReport = TypeReport.AGGREGATED,
                  filters: list[Filter] | None = None, fields: list[str] | None = None):
         self.project = project
@@ -107,15 +105,14 @@
         self.filters = filters
         self.attribution = attribution
         self.fields = ";".join(fields) if fields else ""
 
     def __str__(self):
         return f"{self.datetime_from}//{self.datetime_to}"
 
-    @abstractmethod
     def to_json(self) -> str:
         payload = {"project": self.project,
                    "metrics": self.metrics,
                    "datetimeFrom": self.datetime_from,
                    "datetimeTo": self.datetime_to,
                    "groupBy": self.group_by.value,
                    "type": self.type.value}
```

### Comparing `smartis_sdk-0.1.0/PKG-INFO` & `smartis_sdk-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartis-sdk
-Version: 0.1.0
+Version: 0.2.0
 Summary: SDK для Smartis API
 License: MIT
 Author: viktor
 Author-email: vi.dave@yandex.ru
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


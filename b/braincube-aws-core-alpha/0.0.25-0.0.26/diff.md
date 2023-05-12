# Comparing `tmp/braincube-aws-core-alpha-0.0.25.tar.gz` & `tmp/braincube-aws-core-alpha-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braincube-aws-core-alpha-0.0.25.tar", last modified: Wed May 10 14:13:56 2023, max compression
+gzip compressed data, was "braincube-aws-core-alpha-0.0.26.tar", last modified: Fri May 12 06:58:03 2023, max compression
```

## Comparing `braincube-aws-core-alpha-0.0.25.tar` & `braincube-aws-core-alpha-0.0.26.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 14:13:56.418710 braincube-aws-core-alpha-0.0.25/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.25/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     9101 2023-05-10 14:13:56.420648 braincube-aws-core-alpha-0.0.25/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8348 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.25/README.md
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.25/pyproject.toml
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      933 2023-05-10 14:13:56.426060 braincube-aws-core-alpha-0.0.25/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.25/setup.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 14:13:56.350566 braincube-aws-core-alpha-0.0.25/src/
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 14:13:56.366803 braincube-aws-core-alpha-0.0.25/src/braincube_aws_core_alpha.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     9101 2023-05-10 14:13:56.000000 braincube-aws-core-alpha-0.0.25/src/braincube_aws_core_alpha.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      733 2023-05-10 14:13:56.000000 braincube-aws-core-alpha-0.0.25/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-10 14:13:56.000000 braincube-aws-core-alpha-0.0.25/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-10 14:13:56.000000 braincube-aws-core-alpha-0.0.25/src/braincube_aws_core_alpha.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-10 14:13:56.000000 braincube-aws-core-alpha-0.0.25/src/braincube_aws_core_alpha.egg-info/top_level.txt
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 14:13:56.367630 braincube-aws-core-alpha-0.0.25/src/core/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.25/src/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 14:13:56.395820 braincube-aws-core-alpha-0.0.25/src/core/dal/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.25/src/core/dal/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1243 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.25/src/core/dal/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      248 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.25/src/core/dal/database_errors.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3354 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.25/src/core/dal/postgres_connection.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)    30511 2023-05-10 14:04:48.000000 braincube-aws-core-alpha-0.0.25/src/core/dal/postgres_repository.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 14:13:56.404563 braincube-aws-core-alpha-0.0.25/src/core/di/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.25/src/core/di/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      575 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.25/src/core/di/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4178 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.25/src/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 14:13:56.409858 braincube-aws-core-alpha-0.0.25/src/core/rest/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.25/src/core/rest/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2835 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.25/src/core/rest/app_controller.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3736 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.25/src/core/rest/app_module.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3597 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.25/src/core/rest/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 14:13:56.417212 braincube-aws-core-alpha-0.0.25/src/core/utils/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.25/src/core/utils/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      738 2023-05-10 14:02:40.000000 braincube-aws-core-alpha-0.0.25/src/core/utils/convert.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1391 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.25/src/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 06:58:03.900180 braincube-aws-core-alpha-0.0.26/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.26/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     9107 2023-05-12 06:58:03.900439 braincube-aws-core-alpha-0.0.26/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8354 2023-05-10 17:06:13.000000 braincube-aws-core-alpha-0.0.26/README.md
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.26/pyproject.toml
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      933 2023-05-12 06:58:03.901927 braincube-aws-core-alpha-0.0.26/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.26/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 06:58:03.883983 braincube-aws-core-alpha-0.0.26/src/
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 06:58:03.888391 braincube-aws-core-alpha-0.0.26/src/braincube_aws_core_alpha.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     9107 2023-05-12 06:58:03.000000 braincube-aws-core-alpha-0.0.26/src/braincube_aws_core_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      733 2023-05-12 06:58:03.000000 braincube-aws-core-alpha-0.0.26/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-12 06:58:03.000000 braincube-aws-core-alpha-0.0.26/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-12 06:58:03.000000 braincube-aws-core-alpha-0.0.26/src/braincube_aws_core_alpha.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-12 06:58:03.000000 braincube-aws-core-alpha-0.0.26/src/braincube_aws_core_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 06:58:03.888799 braincube-aws-core-alpha-0.0.26/src/core/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.26/src/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 06:58:03.892049 braincube-aws-core-alpha-0.0.26/src/core/dal/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.26/src/core/dal/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1990 2023-05-11 11:52:40.000000 braincube-aws-core-alpha-0.0.26/src/core/dal/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      241 2023-05-11 10:53:14.000000 braincube-aws-core-alpha-0.0.26/src/core/dal/database_errors.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3354 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.26/src/core/dal/postgres_connection.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)    31143 2023-05-11 16:43:27.000000 braincube-aws-core-alpha-0.0.26/src/core/dal/postgres_repository.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 06:58:03.894425 braincube-aws-core-alpha-0.0.26/src/core/di/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.26/src/core/di/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      561 2023-05-11 10:50:19.000000 braincube-aws-core-alpha-0.0.26/src/core/di/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4122 2023-05-11 10:51:25.000000 braincube-aws-core-alpha-0.0.26/src/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 06:58:03.897294 braincube-aws-core-alpha-0.0.26/src/core/rest/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.26/src/core/rest/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2793 2023-05-11 10:52:14.000000 braincube-aws-core-alpha-0.0.26/src/core/rest/app_controller.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3722 2023-05-11 10:52:31.000000 braincube-aws-core-alpha-0.0.26/src/core/rest/app_module.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3598 2023-05-11 17:50:46.000000 braincube-aws-core-alpha-0.0.26/src/core/rest/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 06:58:03.899565 braincube-aws-core-alpha-0.0.26/src/core/utils/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.26/src/core/utils/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      738 2023-05-10 14:02:40.000000 braincube-aws-core-alpha-0.0.26/src/core/utils/convert.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1377 2023-05-11 10:53:41.000000 braincube-aws-core-alpha-0.0.26/src/core/utils/data.py
```

### Comparing `braincube-aws-core-alpha-0.0.25/LICENSE` & `braincube-aws-core-alpha-0.0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.25/PKG-INFO` & `braincube-aws-core-alpha-0.0.26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.25
+Version: 0.0.26
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
@@ -139,21 +139,21 @@
         Column(name="country", ),
         Column(name="min_amount", alias="minAmount"),
     ],
     relations=[
         Relation(
             table="parties",
             alias="p",
-            force_join=False,
+            join_forced=False,
             columns=[
                 SimpleColumn(name="name"),
                 SimpleColumn(name="short_name", alias="shortName"),
             ],
             join_type=JoinType.left,
-            through=JoinThrough(from_column_name="issuer_id", to_column_name="id")
+            join_through=JoinThrough(from_column_name="issuer_id", to_column_name="id")
         )
     ]
 )
 
 
 # repository definition
 class EquitiesRepo(PostgresRepository):
```

### Comparing `braincube-aws-core-alpha-0.0.25/README.md` & `braincube-aws-core-alpha-0.0.26/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -119,21 +119,21 @@
         Column(name="country", ),
         Column(name="min_amount", alias="minAmount"),
     ],
     relations=[
         Relation(
             table="parties",
             alias="p",
-            force_join=False,
+            join_forced=False,
             columns=[
                 SimpleColumn(name="name"),
                 SimpleColumn(name="short_name", alias="shortName"),
             ],
             join_type=JoinType.left,
-            through=JoinThrough(from_column_name="issuer_id", to_column_name="id")
+            join_through=JoinThrough(from_column_name="issuer_id", to_column_name="id")
         )
     ]
 )
 
 
 # repository definition
 class EquitiesRepo(PostgresRepository):
```

### Comparing `braincube-aws-core-alpha-0.0.25/setup.cfg` & `braincube-aws-core-alpha-0.0.26/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = braincube-aws-core-alpha
-version = 0.0.25
+version = 0.0.26
 author = Braincube
 author_email = v.boudis@braincube.gr
 description = Microframework for python aws lambdas
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://bitbucket.org/braincube-common/core-aws.git
 license = MIT
```

### Comparing `braincube-aws-core-alpha-0.0.25/src/braincube_aws_core_alpha.egg-info/PKG-INFO` & `braincube-aws-core-alpha-0.0.26/src/braincube_aws_core_alpha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.25
+Version: 0.0.26
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
@@ -139,21 +139,21 @@
         Column(name="country", ),
         Column(name="min_amount", alias="minAmount"),
     ],
     relations=[
         Relation(
             table="parties",
             alias="p",
-            force_join=False,
+            join_forced=False,
             columns=[
                 SimpleColumn(name="name"),
                 SimpleColumn(name="short_name", alias="shortName"),
             ],
             join_type=JoinType.left,
-            through=JoinThrough(from_column_name="issuer_id", to_column_name="id")
+            join_through=JoinThrough(from_column_name="issuer_id", to_column_name="id")
         )
     ]
 )
 
 
 # repository definition
 class EquitiesRepo(PostgresRepository):
```

### Comparing `braincube-aws-core-alpha-0.0.25/src/braincube_aws_core_alpha.egg-info/SOURCES.txt` & `braincube-aws-core-alpha-0.0.26/src/braincube_aws_core_alpha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.25/src/core/dal/data.py` & `braincube-aws-core-alpha-0.0.26/src/core/dal/data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from enum import Enum
 from dataclasses import dataclass
 
-from ..utils.data import Order
+from ..utils.data import Order, OrderType
+
+from pypika import Table, Field
 
 
 class Key:
     def __init__(self, *args):
         self.values = list(args)
 
 
@@ -46,29 +48,67 @@
     insertable: bool = True
 
 
 @dataclass()
 class StatementField:
     alias: str
     statement: str
-    relations_aliases: list[str]
+    relations_aliases: list[str] | None = None
 
 
 @dataclass()
 class Relation:
     table: str
-    alias: str | None
-    force_join: bool
     columns: list[SimpleColumn]
     join_type: JoinType
-    through: JoinThrough
+    join_through: JoinThrough
+    join_forced: bool = False
+    alias: str | None = None
 
 
 @dataclass()
 class Schema:
     table: str
-    alias: str | None
     primary_key: list[str]
-    order: list[Order]
-    statement_fields: list[StatementField]
     columns: list[Column]
-    relations: list[Relation]
+    statement_fields: list[StatementField] | None = None
+    relations: list[Relation] | None = None
+    order: list[Order] | None = None
+    alias: str | None = None
+
+
+class FieldType(Enum):
+    column = "COLUMN"
+    statement = "STATEMENT"
+    related_column = "RELATED_COLUMN"
+
+
+@dataclass()
+class FieldData:
+    type_: FieldType
+    field: Field
+    name: str = None
+    updatable: bool = False
+    insertable: bool = False
+    statement: str = None
+    relations_aliases: list[str] = None
+
+
+@dataclass()
+class OrderData:
+    field: Field
+    order_type: OrderType
+
+
+@dataclass()
+class TableData:
+    name: str
+    table: Table
+
+
+@dataclass()
+class RelatedTableData:
+    table: Table
+    name: str
+    join_type: JoinType
+    join_through: JoinThrough
+    join_forced: bool = False
```

### Comparing `braincube-aws-core-alpha-0.0.25/src/core/dal/postgres_connection.py` & `braincube-aws-core-alpha-0.0.26/src/core/dal/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.25/src/core/dal/postgres_repository.py` & `braincube-aws-core-alpha-0.0.26/src/core/dal/postgres_repository.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import TypeVar
 
 from pydantic import BaseModel
 from pypika.queries import QueryBuilder
 from pypika import PostgreSQLQuery, Table, Field, Criterion, EmptyCriterion, CustomFunction, functions as fn
 
 from ..utils.data import Order, OrderType, Condition, ConditionType, Page, Pageable, Paging, Top, Metadata
-from .data import Key, Schema, Relation, SaveType, Column, StatementField
+from .data import Key, Schema, SaveType, TableData, FieldData, RelatedTableData, OrderData, FieldType
 from .database_errors import DatabaseError, DeleteError, SaveError
 from .postgres_connection import Pool, Connection
 
 T = TypeVar("T", bound=BaseModel)
 
 
 class PostgresRepository:
@@ -25,59 +25,86 @@
     def __init__(self, pool: Pool, schema: Schema, relation_separator: str = "_"):
         self._pool = pool
         self._relation_separator = relation_separator
         self.__construct_schema_data(schema)
 
     def __construct_schema_data(self, schema: Schema):
 
-        # master table definition:
-        self._master_table: tuple[Table, str] = \
-            Table(schema.table).as_(schema.alias) if schema.alias else Table(schema.table), schema.table
-
-        self._master_columns: dict[str, tuple[Field, Column]] = dict(
-            map(lambda c: (c.alias if c.alias else c.name, (
-                (self._master_table[0][c.name]).as_(c.alias) if c.alias else self._master_table[0][c.name], c)),
-                schema.columns))
-
-        self._master_statement_fields: dict[str, tuple[Field, StatementField]] = dict(
-            map(lambda f: (f.alias, (self._master_table[0][f.alias], f)), schema.statement_fields))
-
-        self._master_primary_key: dict[str, tuple[Field, Column]] = dict(
-            itertools.islice(self._master_columns.items(), len(schema.primary_key)))
-
-        # related tables definition:
-        self._related_tables: dict[str, tuple[Table, Relation]] = dict()
-        self._related_columns: dict[str, tuple[Field]] = dict()
+        # master table:
+        self._master_table: TableData = \
+            TableData(schema.table, Table(schema.table).as_(schema.alias) if schema.alias else Table(schema.table))
+
+        # master columns:
+        self._master_columns: dict[str, FieldData] = dict()
+        for column in schema.columns:
+            self._master_columns[column.alias if column.alias else column.name] = FieldData(
+                FieldType.column,
+                (self._master_table.table[column.name]).as_(column.alias)
+                if column.alias else self._master_table.table[column.name],
+                column.name,
+                column.insertable,
+                column.updatable
+            )
+
+        # statement fields:
+        self._statement_fields: dict[str, FieldData] = dict()
+        if schema.statement_fields:
+            for statement_field in schema.statement_fields:
+                self._statement_fields[statement_field.alias] = FieldData(
+                    FieldType.statement,
+                    self._master_table.table[statement_field.alias],
+                    statement=statement_field.statement,
+                    relations_aliases=statement_field.relations_aliases
+                )
+
+        # primary key:
+        self._primary_key: dict[str, FieldData] = \
+            dict(itertools.islice(self._master_columns.items(), len(schema.primary_key)))
+
+        # related tables:
+        self._related_tables: dict[str, RelatedTableData] = dict()
+        self._related_columns: dict[str, FieldData] = dict()
         self._related_forced_tables_aliases: list[str] = list()
 
-        for relation in schema.relations:
-            table_alias = relation.alias if relation.alias else relation.table
-            related_table = Table(relation.table).as_(relation.alias) if relation.alias else Table(relation.table)
-            self._related_tables[table_alias] = related_table, relation
-            if relation.force_join:
-                self._related_forced_tables_aliases.append(table_alias)
-            for column in relation.columns:
-                column_alias = \
-                    f"{relation.table}{self._relation_separator}{column.alias if column.alias else column.name}"
-                self._related_columns[column_alias] = (related_table[column.name]).as_(column_alias),
-
-        self._schema_columns: dict[str, tuple] = {**self._master_columns, **self._related_columns}
-        self._schema_columns_fields: dict[str, tuple] = {**self._schema_columns, **self._master_statement_fields}
-
-        # order by definition:
-        self._schema_order: list[tuple[Field, OrderType]] = [(self._schema_columns_fields[order.alias][0], order.type)
-                                                             for order in schema.order]
+        if schema.relations:
+            for relation in schema.relations:
+                table_alias: str = relation.alias if relation.alias else relation.table
+                related_table = Table(relation.table).as_(relation.alias) if relation.alias else Table(relation.table)
+                self._related_tables[table_alias] = RelatedTableData(
+                    related_table, relation.table, relation.join_type,
+                    relation.join_through, relation.join_forced
+                )
+                if relation.join_forced:
+                    self._related_forced_tables_aliases.append(table_alias)
+                for column in relation.columns:
+                    column_alias: str = \
+                        f"{relation.table}{self._relation_separator}{column.alias if column.alias else column.name}"
+                    self._related_columns[column_alias] = FieldData(
+                        FieldType.related_column,
+                        (related_table[column.name]).as_(column_alias),
+                        column.name
+                    )
+
+        # related columns and fields:
+        self._columns: dict[str, FieldData] = {**self._master_columns, **self._related_columns}
+        self._columns_and_statement_fields: dict[str, FieldData] = {**self._columns, **self._statement_fields}
+
+        # order by:
+        self._order_by: list[OrderData] = list()
+        if schema.order:
+            self._order_by.extend([OrderData(self._columns_and_statement_fields[order.alias].field, order.type)
+                                   for order in schema.order])
+        else:
+            self._order_by.extend([OrderData(pk.field, OrderType.asc) for pk in self._primary_key.values()])
 
     @staticmethod
-    def __base_model_aliases(cls: type[T]):
+    def __base_model_aliases(cls: type[T]) -> list[str]:
         return [f.alias for f in cls.__fields__.values()]
 
-    async def fetch(self, q: str,
-                    params: list | None = None,
-                    connection: Connection | None = None):
+    async def fetch(self, q: str, params: list = None, connection: Connection = None):
         """Retrieve records from raw PSQL query.
         :param q: Query.
         :param params: Query parameters.
         :param connection: (asyncpg) Connection that will execute the query.
         :return: Records as dictionary.
         """
 
@@ -87,110 +114,103 @@
                 return [dict(r) for r in (await connection.fetch(q, *params) if params else await connection.fetch(q))]
             async with self._pool.acquire() as connection_:
                 return [dict(r) for r in
                         (await connection_.fetch(q, *params) if params else await connection_.fetch(q))]
         except Exception as e:
             raise DatabaseError(e)
 
-    async def fetch_one(self, q: str,
-                        params: list | None = None,
-                        connection: Connection | None = None) -> dict[str, any] | None:
+    async def fetch_one(self, q: str, params: list = None, connection: Connection = None) -> dict[str, any] | None:
         """Retrieve record from raw PSQL query.
         :param q: Query.
         :param params: Query parameters.
         :param connection: (asyncpg) Connection that will execute the query.
         :return: Record as dictionary.
         """
 
         data = await self.fetch(q, params, connection)
 
         return data[0] if data else None
 
-    async def execute(self, q: str,
-                      params: list | None = None,
-                      connection: Connection | None = None) -> any:
+    async def execute(self, q: str, params: list = None, connection: Connection = None) -> any:
         """Execute raw PSQL query.
         :param q: Query.
         :param params: Query parameters.
         :param connection: (asyncpg) Connection that will execute the query.
         :return: Execution results as dictionary.
         """
 
         return await self.fetch(q, params, connection)
 
     async def _fetch(self, q: QueryBuilder,
-                     replace_fields=True,
-                     connection: Connection | None = None) -> list[dict[str, any]]:
+                     replace_fields: bool = True,
+                     connection: Connection = None) -> list[dict[str, any]]:
 
         query = self._replace_statement_fields(q) if replace_fields else str(q)
 
         return await self.fetch(query, connection=connection)
 
     async def _fetch_one(self, q: QueryBuilder,
-                         replace_fields=True,
-                         connection: Connection | None = None) -> dict[str, any] | None:
+                         replace_fields: bool = True,
+                         connection: Connection = None) -> dict[str, any] | None:
 
         data = await self._fetch(q, replace_fields, connection)
 
         return data[0] if data else None
 
     async def _execute(self, q: QueryBuilder,
-                       returning_aliases: list[str] | None = None,
-                       connection: Connection | None = None) -> any:
+                       returning_aliases: list[str] = None,
+                       connection: Connection = None) -> any:
 
-        table = Table(self._master_table[1])
+        table = Table(self._master_table.name)
 
-        for field, column in self._aliases_to_fields(returning_aliases, select=False):
-            q = q.returning(table[field.name].as_(field.alias))
+        for field in self._aliases_to_fields(returning_aliases, select=False):
+            field_ = field if isinstance(field, Field) else field.field
+            q = q.returning(table[field_.name].as_(field_.alias))
 
         return await self._fetch(q, False, connection)
 
     def _create_primary_key_criterion(self, key: Key, select: bool = True) -> Criterion:
-        return Criterion.all(
-            [pk[0] == key.values[i] if select else (Field(name=pk[1].name) == key.values[i]) for i, pk in
-             enumerate(self._master_primary_key.values())])
+        return Criterion.all([f.field == key.values[i] if select else (Field(name=f.name) == key.values[i]) for i, f in
+                              enumerate(self._primary_key.values())])
 
-    def _aliases_to_fields(self, aliases: list[str] | None = None,
-                           select: bool = True) -> list[tuple]:
+    def _aliases_to_fields(self, aliases: list[str] = None, select: bool = True) -> list[FieldData]:
 
         fields = list()
-        accepted = self._schema_columns_fields if select else self._master_columns
+        accepted = self._columns_and_statement_fields if select else self._master_columns
         if aliases:
             for alias in aliases:
                 field = accepted.get(alias)
                 if not field:
                     continue
                 fields.append(field)
-
         return fields if fields else list(
-            self._master_columns.values() if select else self._master_primary_key.values())
+            self._master_columns.values() if select else self._primary_key.values())
 
-    def _order_to_fields(self, order: list[Order]) -> list[tuple[Field, OrderType]]:
+    def _order_to_fields(self, order: list[Order]) -> list[OrderData]:
 
         data = list()
         for order_ in order:
-            field = self._schema_columns_fields.get(order_.alias)
-            if not field:
+            field_data = self._columns_and_statement_fields.get(order_.alias)
+            if not field_data:
                 continue
-            data.append((field[0], order_.type))
+            data.append(OrderData(field_data.field, order_.type))
 
-        return data if data else self._schema_order
+        return data if data else self._order_by
 
-    def _conditions_to_criterion(self, conditions: list[Condition] | None = None,
-                                 select: bool = True) -> Criterion:
+    def _conditions_to_criterion(self, conditions: list[Condition] = None, select: bool = True) -> Criterion:
 
         if not conditions:
             return EmptyCriterion()
 
         criteria = list()
         for con in conditions:
-            column = self._schema_columns.get(con.alias)
-            if not column:
+            field_data = self._columns.get(con.alias)
+            if not field_data:
                 continue
-            field = column[0] if select else Field(name=column[0].name)
+            field = field_data.field if select else Field(name=field_data.name)
             if isinstance(con.value, list):
                 if con.type == ConditionType.range:
                     if con.value[0]:
                         criteria.append(con.value[0] <= field)
                     if con.value[1]:
                         criteria.append(field <= con.value[1])
                 elif con.type == ConditionType.any:
@@ -201,123 +221,124 @@
 
         return Criterion.all(criteria)
 
     def _replace_statement_fields(self, q: QueryBuilder) -> str:
 
         query = str(q)
 
-        for field, schema_field in self._master_statement_fields.values():
-            query = query.replace(f"\"{self._master_table[0].alias}\".\"{field.name}\"",
-                                  f"{schema_field.statement} \"{field.name}\"")
+        for field_data in self._statement_fields.values():
+            query = query.replace(f"\"{self._master_table.table.alias}\".\"{field_data.field.name}\"",
+                                  f"{field_data.statement} \"{field_data.field.name}\"")
 
         return query
 
     def _filter_save_data(self, data: dict[str, any], type_: SaveType) -> dict[str, any]:
 
         data_: dict[str, any] = dict()
 
         for k, v in data.items():
             column = self._master_columns.get(k)
             if not column:
                 continue
-            if type_ == SaveType.insert and not column[1].insertable:
-                raise SaveError(f"column:'{column[1].name}' is not insertable", column[1].name)
-            if type_ == SaveType.update and not column[1].updatable:
-                raise SaveError(f"column:'{column[1].name}' is not updatable", column[1].name)
-            data_[column[1].name] = v
+            if type_ == SaveType.insert and not column.insertable:
+                raise SaveError(f"column:'{column.name}' is not insertable", column.name)
+            if type_ == SaveType.update and not column.updatable:
+                raise SaveError(f"column:'{column.name}' is not updatable", column.name)
+            data_[column.name] = v
 
         if not data_:
             raise SaveError("no columns provided")
 
         return data_
 
-    def __init_select_query(self, fields: list[tuple],
-                            criterion: Criterion | None = None,
-                            order: list[tuple[Field, OrderType]] | None = None,
+    def __init_select_query(self, fields: list[FieldData],
+                            criterion: Criterion = None,
+                            order: list[OrderData] = None,
                             count_query: bool = False) -> tuple[QueryBuilder, QueryBuilder | None]:
 
-        q = PostgreSQLQuery.from_(self._master_table[0])
+        q = PostgreSQLQuery.from_(self._master_table.table)
 
         table_aliases = self._related_forced_tables_aliases.copy()
 
         for field in fields:
-            if len(field) == 2 and isinstance(field[1], StatementField):
-                table_aliases.extend(field[1].relations_aliases)
+            if field.type_ == FieldType.statement and field.relations_aliases:
+                table_aliases.extend(field.relations_aliases)
             else:
-                table_aliases.append(field[0].table.alias)
+                table_aliases.append(field.field.table.alias)
 
         if criterion:
             table_aliases.extend([t.alias for t in criterion.tables_])
             q = q.where(criterion)
 
         if order:
-            table_aliases.extend([o[0].table.alias for o in order])
+            table_aliases.extend([order_.field.table.alias for order_ in order])
 
-        for alias in filter(lambda ta: ta != self._master_table[0].alias, set(table_aliases)):
-            table, relation = self._related_tables[alias]
+        for alias in filter(lambda ta: ta != self._master_table.table.alias, set(table_aliases)):
+            related_table = self._related_tables[alias]
             q = q \
-                .join(table, relation.join_type) \
-                .on(self._master_table[0][relation.through.from_column_name] == table[relation.through.to_column_name])
+                .join(related_table.table, related_table.join_type) \
+                .on(self._master_table.table[related_table.join_through.from_column_name] ==
+                    related_table.table[related_table.join_through.to_column_name])
 
         cq = q.select(fn.Count("*")) if count_query else None
 
         for field in fields:
-            q = q.select(field[0])
+            q = q.select(field.field)
 
         if order:
-            for field, type_ in order:
-                q = q.orderby(field, order=type_)
+            for order_ in order:
+                q = q.orderby(order_.field, order=order_.order_type)
 
         return q, cq
 
-    def _init_select_query(self, aliases: list[str] | None = None,
-                           criterion: Criterion | None = None,
-                           order: list[Order] | None = None,
+    def _init_select_query(self, aliases: list[str] = None,
+                           criterion: Criterion = None,
+                           order: list[Order] = None,
                            set_order: bool = True,
                            count_query: bool = False) -> tuple[QueryBuilder, QueryBuilder | None]:
 
         fields = self._aliases_to_fields(aliases)
-        order_ = self._order_to_fields(order) if order else (self._schema_order if set_order else None)
+        order_ = self._order_to_fields(order) if order else (self._order_by if set_order else None)
 
         return self.__init_select_query(fields, criterion, order_, count_query)
 
-    async def _find_one(self, aliases: list[str] | None = None,
-                        criterion: Criterion | None = None,
-                        order: list[Order] | None = None,
-                        connection: Connection | None = None) -> dict[str, any] | None:
+    async def _find_one(self, aliases: list[str] = None,
+                        criterion: Criterion = None,
+                        order: list[Order] = None,
+                        connection: Connection = None) -> dict[str, any] | None:
 
         q, _ = self._init_select_query(aliases, criterion, order)
 
         return await self._fetch_one(q.limit(1), connection=connection)
 
-    async def _find_all(self, aliases: list[str] | None = None,
-                        criterion: Criterion | None = None,
-                        order: list[Order] | None = None,
-                        connection: Connection | None = None) -> list[dict[str, any]]:
+    async def _find_all(self, aliases: list[str] = None,
+                        criterion: Criterion = None,
+                        order: list[Order] = None,
+                        connection: Connection = None) -> list[dict[str, any]]:
 
         q, _ = self._init_select_query(aliases, criterion, order)
 
         return await self._fetch(q, connection=connection)
 
-    async def _find_many(self, aliases: list[str] | None = None,
-                         criterion: Criterion | None = None,
+    async def _find_many(self, aliases: list[str] = None,
+                         criterion: Criterion = None,
                          page: Pageable = Pageable(),
-                         order: list[Order] | None = None,
-                         connection: Connection | None = None) -> Page | Top:
+                         order: list[Order] = None,
+                         connection: Connection = None) -> Page | Top:
 
         if connection:
             return await self.__find_many(connection, aliases, criterion, page, order)
         async with self._pool.acquire() as connection_:
             return await self.__find_many(connection_, aliases, criterion, page, order)
 
     async def __find_many(self, connection: Connection,
-                          aliases: list[str] | None = None,
-                          criterion: Criterion | None = None,
+                          aliases: list[str] = None,
+                          criterion: Criterion = None,
                           page: Pageable = Pageable(),
-                          order: list[Order] | None = None) -> Page | Top:
+                          order: list[Order] = None) -> Page | Top:
 
         if page.top_size < 0:
             data = await self._find_all(aliases, criterion, order, connection)
             return Top(data, page.top_size, False)
 
         start = time.time()
 
@@ -352,107 +373,107 @@
                                         connection=connection)
 
         return Page(records, Paging(page_no, page.page_size, total_pages, count),
                     Metadata(int((time.time() - start) * 1000)))
 
     async def _update(self, data: BaseModel | dict[str, any],
                       criterion: Criterion,
-                      returning_aliases: list[str] | None = None,
-                      connection: Connection | None = None) -> list[dict[str, any]] | None:
+                      returning_aliases: list[str] = None,
+                      connection: Connection = None) -> list[dict[str, any]] | None:
 
         if isinstance(criterion, EmptyCriterion):
             raise SaveError("update without conditions is not allowed")
 
-        uq = PostgreSQLQuery.update(self._master_table[1])
+        uq = PostgreSQLQuery.update(self._master_table.name)
 
         data_ = data.dict(by_alias=True, exclude_unset=True) if isinstance(data, BaseModel) else data.copy()
 
         for v, k in self._filter_save_data(data_, SaveType.update).items():
             uq = uq.set(v, k)
         uq = uq.where(criterion)
 
         return await self._execute(uq, returning_aliases, connection)
 
     async def _delete(self, criterion: Criterion,
-                      returning_aliases: list[str] | None = None,
-                      connection: Connection | None = None) -> list[dict[str, any]] | None:
+                      returning_aliases: list[str] = None,
+                      connection: Connection = None) -> list[dict[str, any]] | None:
 
         if isinstance(criterion, EmptyCriterion):
             raise DeleteError("delete without conditions is not allowed")
 
         dq = PostgreSQLQuery \
-            .from_(self._master_table[1]) \
+            .from_(self._master_table.name) \
             .delete() \
             .where(criterion)
 
         return await self._execute(dq, returning_aliases, connection)
 
     async def find_by_pk(self, key: Key,
-                         aliases: list[str] | None = None,
-                         connection: Connection | None = None) -> dict[str, any] | None:
+                         aliases: list[str] = None,
+                         connection: Connection = None) -> dict[str, any] | None:
         """Find the record from passed key.
         :param key: Record identifier.
         :param aliases: List of fields that will be selected by the query.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :return: Record as dictionary.
         """
 
         criterion = self._create_primary_key_criterion(key)
 
         q, _ = self._init_select_query(aliases, criterion, set_order=False)
 
         return await self._fetch_one(q, connection=connection)
 
-    async def exists_by_pk(self, key: Key, connection: Connection | None = None) -> bool:
+    async def exists_by_pk(self, key: Key, connection: Connection = None) -> bool:
         """Find if record exists from passed key.
         :param key: Record identifier.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :return: Record existence.
         """
 
-        aliases = [column.alias for field, column in self._master_primary_key.values()]
+        aliases = [pk.field.alias for pk in self._primary_key.values()]
 
         return await self.find_by_pk(key, aliases, connection) is not None
 
-    async def find_one(self, aliases: list[str] | None = None,
-                       conditions: list[Condition] | None = None,
-                       order: list[Order] | None = None,
-                       connection: Connection | None = None) -> dict[str, any] | None:
+    async def find_one(self, aliases: list[str] = None,
+                       conditions: list[Condition] = None,
+                       order: list[Order] = None,
+                       connection: Connection = None) -> dict[str, any] | None:
         """Find one record from passed filters.
         :param aliases: List of fields that will be selected by the query.
         :param conditions: List of filters that will be applied to query.
         :param order: Order that will be applied to query.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :return: Record as dictionary.
         """
 
         criterion = self._conditions_to_criterion(conditions)
 
         return await self._find_one(aliases, criterion, order, connection)
 
-    async def find_all(self, aliases: list[str] | None = None,
-                       conditions: list[Condition] | None = None,
-                       order: list[Order] | None = None,
-                       connection: Connection | None = None) -> list[dict[str, any]]:
+    async def find_all(self, aliases: list[str] = None,
+                       conditions: list[Condition] = None,
+                       order: list[Order] = None,
+                       connection: Connection = None) -> list[dict[str, any]]:
         """Find all records from passed filters.
         :param aliases: List of fields that will be selected by the query.
         :param conditions: List of filters that will be applied to query.
         :param order: Order in which the records will be returned.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :return: Records as dictionary list.
         """
 
         criterion = self._conditions_to_criterion(conditions)
 
         return await self._find_all(aliases, criterion, order, connection)
 
     async def find_all_by_pk(self, keys: list[Key],
-                             aliases: list[str] | None = None,
-                             order: list[Order] | None = None,
-                             connection: Connection | None = None) -> list[dict[str, any]]:
+                             aliases: list[str] = None,
+                             order: list[Order] = None,
+                             connection: Connection = None) -> list[dict[str, any]]:
         """Find all records from passed keys.
         :param keys: Records identifiers.
         :param aliases: List of fields that will be selected by the query.
         :param order: Order in which the records will be returned.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :return: Record as dictionary.
         """
@@ -460,87 +481,87 @@
         if not keys:
             raise DatabaseError("no keys provided")
 
         criterion = Criterion.any([self._create_primary_key_criterion(key) for key in keys])
 
         return await self._find_all(aliases, criterion, order, connection)
 
-    async def find_many(self, aliases: list[str] | None = None,
-                        conditions: list[Condition] | None = None,
+    async def find_many(self, aliases: list[str] = None,
+                        conditions: list[Condition] = None,
                         page: Pageable = Pageable(),
-                        order: list[Order] | None = None,
-                        connection: Connection | None = None) -> Page | Top:
+                        order: list[Order] = None,
+                        connection: Connection = None) -> Page | Top:
         """Find records from passed filters using paging.
         :param aliases: List of fields that will be selected by the query.
         :param conditions: List of filters that will be applied to query.
         :param page: Limit and offset of the query.
         :param order: Order in which the records will be returned.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :return: Records wrapped by Page or Top dataclass.
         """
 
         criterion = self._conditions_to_criterion(conditions)
 
         return await self._find_many(aliases, criterion, page, order, connection)
 
     async def insert(self, data: BaseModel | dict[str, any],
-                     returning_aliases: list[str] | None = None,
-                     connection: Connection | None = None) -> dict[str, any]:
+                     returning_aliases: list[str] = None,
+                     connection: Connection = None) -> dict[str, any]:
         """Insert one record from dictionary.
         :param data: Master column aliases with values.
         :param returning_aliases: Query returning data.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When does not adjust to insert-constraints or no master column is specified.
         :return: Execution results as dictionary.
         """
 
         data_ = self._filter_save_data(
             data.dict(by_alias=True, exclude_unset=True) if isinstance(data, BaseModel) else data.copy(),
             SaveType.insert
         )
 
         iq = PostgreSQLQuery \
-            .into(self._master_table[1]) \
+            .into(self._master_table.name) \
             .columns(list(data_.keys())) \
             .insert(list(data_.values()))
 
         records = await self._execute(iq, returning_aliases, connection)
 
         return records[0] if len(records) > 0 else None
 
     async def insert_returning_master(self, data: BaseModel | dict[str, any],
-                                      connection: Connection | None = None):
+                                      connection: Connection = None):
         """Insert one record from dictionary and return all master columns.
         :param data: Master column aliases with values.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When does not adjust to insert-constraints or no master column is specified.
         :return: Execution results as dictionary.
         """
 
         return await self.insert(data, list(self._master_columns.keys()), connection)
 
     async def insert_data(self, data: BaseModel | dict[str, any],
                           returning: type[T],
-                          connection: Connection | None = None) -> T:
+                          connection: Connection = None) -> T:
         """Insert a record using model.
         :param data: Model which contains master table column properties.
         :param returning: Result type.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When does not adjust to insert-constraints or no master column is specified.
         :return: Execution results with returning type.
         """
 
         result = await self.insert(data, self.__base_model_aliases(returning), connection)
 
         return returning(**result) if result else None
 
     async def insert_bulk(self, aliases: list[str],
                           data: list[list],
-                          returning_aliases: list[str] | None = None,
-                          connection: Connection | None = None) -> list[dict[str, any]]:
+                          returning_aliases: list[str] = None,
+                          connection: Connection = None) -> list[dict[str, any]]:
         """Insert many records at once from list.
         :param aliases: Master column aliases.
         :param data: Master column values.
         :param returning_aliases: Query returning data.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When does not adjust to insert-constraints or no master column is specified.
         :return: Execution result as dictionary list.
@@ -552,33 +573,33 @@
             raise SaveError("invalid bulk insert data")
 
         column_names: dict[str, int] = dict()
         for i, alias in enumerate(aliases):
             column = self._master_columns.get(alias)
             if not column:
                 continue
-            if not column[1].insertable:
-                raise SaveError(f"column:'{column[1].name}' is not insertable", column[1].name)
-            column_names[column[1].name] = i
+            if not column.insertable:
+                raise SaveError(f"column:'{column.name}' is not insertable", column.name)
+            column_names[column.name] = i
         if not column_names:
             raise SaveError("no columns provided")
 
         iq = PostgreSQLQuery \
-            .into(self._master_table[1]) \
+            .into(self._master_table.name) \
             .columns(list(column_names.keys()))
 
         for d in data:
             iq = iq.insert([d[i] for i in column_names.values()])
 
         return await self._execute(iq, returning_aliases, connection)
 
     async def update(self, data: BaseModel | dict[str, any],
                      conditions: list[Condition],
-                     returning_aliases: list[str] | None = None,
-                     connection: Connection | None = None) -> list[dict[str, any]] | None:
+                     returning_aliases: list[str] = None,
+                     connection: Connection = None) -> list[dict[str, any]] | None:
         """Update records with new data according conditions.
         :param data: Master column aliases with values.
         :param conditions: List of filters that will be applied into the query.
         :param returning_aliases: Query returning data.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When does not adjust to update-constraints or no master column is specified.
         :return: Execution results as dictionary list.
@@ -586,16 +607,16 @@
 
         criterion = self._conditions_to_criterion(conditions, select=False)
 
         return await self._update(data, criterion, returning_aliases, connection)
 
     async def update_by_pk(self, key: Key,
                            data: BaseModel | dict[str, any],
-                           returning_aliases: list[str] | None = None,
-                           connection: Connection | None = None) -> dict[str, any] | None:
+                           returning_aliases: list[str] = None,
+                           connection: Connection = None) -> dict[str, any] | None:
         """Update record with new data according to passed key.
         :param key: Record identifier.
         :param data: Master column aliases with values.
         :param returning_aliases: Query returning data.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When does not adjust to update-constraints or no master column is specified.
         :return: Execution result as dictionary.
@@ -606,15 +627,15 @@
         records = await self._update(data, criterion, returning_aliases, connection)
 
         return records[0] if len(records) > 0 else None
 
     async def update_data(self, data: BaseModel | dict[str, any],
                           conditions: list[Condition],
                           returning: type[T],
-                          connection: Connection | None = None) -> list[T] | None:
+                          connection: Connection = None) -> list[T] | None:
         """Update records with new data according conditions using model.
         :param data: Model which contains master table column properties.
         :param conditions: List of filters that will be applied into the query.
         :param returning: Result type.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When does not adjust to update-constraints or no master column is specified.
         :return: Execution results with returning type.
@@ -623,46 +644,46 @@
         results = await self.update(data, conditions, self.__base_model_aliases(returning), connection)
 
         return [returning(**r) for r in results] if results else None
 
     async def update_data_by_pk(self, key: Key,
                                 data: BaseModel | dict[str, any],
                                 returning: type[T],
-                                connection: Connection | None = None) -> T | None:
+                                connection: Connection = None) -> T | None:
         """Update record with new data according to passed key using model.
         :param key: Record identifier.
         :param data: Model which contains master table column properties.
         :param returning: Result type.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When does not adjust to update-constraints or no master column is specified.
         :return: Execution result with returning type.
         """
 
         result = await self.update_by_pk(key, data, self.__base_model_aliases(returning), connection)
 
         return returning(**result) if result else None
 
     async def delete(self, conditions: list[Condition],
-                     returning_aliases: list[str] | None = None,
-                     connection: Connection | None = None) -> list[dict[str, any]] | None:
+                     returning_aliases: list[str] = None,
+                     connection: Connection = None) -> list[dict[str, any]] | None:
         """Delete records according conditions.
         :param conditions: List of filters that will be applied into the query.
         :param returning_aliases: Query returning data.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When conditions are empty.
         :return: Execution results as dictionary list.
         """
 
         criterion = self._conditions_to_criterion(conditions, select=False)
 
         return await self._delete(criterion, returning_aliases, connection)
 
     async def delete_by_pk(self, key: Key,
-                           returning_aliases: list[str] | None = None,
-                           connection: Connection | None = None) -> dict[str, any] | None:
+                           returning_aliases: list[str] = None,
+                           connection: Connection = None) -> dict[str, any] | None:
         """Delete records according to passed key.
         :param key: Record identifier.
         :param returning_aliases: Query returning data.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When conditions are empty.
         :return: Execution results as dictionary.
         """
```

### Comparing `braincube-aws-core-alpha-0.0.25/src/core/di/data.py` & `braincube-aws-core-alpha-0.0.26/src/core/di/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 
 @dataclass()
 class Dependency(Generic[T]):
     scope: Scope
     cls: Type[T]
     params: list[tuple[type, str | None]] = None
-    name: str | None = None
-    instance: T | None = None
+    name: str = None
+    instance: T = None
     factory: callable = None
 
 
 def qualifier_to_data(qualifier: str) -> dict[str, str]:
     d = dict()
     for s in qualifier.split(","):
         q = s.split(":")
```

### Comparing `braincube-aws-core-alpha-0.0.25/src/core/di/injector.py` & `braincube-aws-core-alpha-0.0.26/src/core/di/injector.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     @staticmethod
     def init_config():
         _Injector.dependencies.append(Dependency(Scope.singleton, Pool, factory=get_pool))
         # here put any other dependency you want to provide out of the box
 
     @staticmethod
-    def inject(name: str | None = None, scope: Scope = Scope.singleton, qualifier: str | None = None):
+    def inject(name: str = None, scope: Scope = Scope.singleton, qualifier: str = None):
         def _inject(component):
             data = qualifier_to_data(qualifier) if qualifier else dict()
             if isfunction(component):
                 cls = component.__annotations__.get("return")
                 if not cls:
                     raise ValueError(f"injected function '{component.__name__}' must specify return type.")
 
@@ -33,15 +33,15 @@
                 params = [(v.annotation, data.get(k)) for k, v in items_.items()]
                 _Injector.dependencies.append(Dependency(scope, component, params, name))
             return component
 
         return _inject
 
     @staticmethod
-    async def provide(cls: Type[T], name: str | None = None) -> T:
+    async def provide(cls: Type[T], name: str = None) -> T:
 
         matched = list(filter(lambda d: (d.cls is cls or issubclass(d.cls, cls)) and
                                         (d.name == name if name else d.name is None), _Injector.dependencies))
 
         if not matched:
             raise ValueError(f"component name:'{name}', class:'{cls}' not found.")
         if len(matched) > 1:
@@ -58,45 +58,45 @@
                 instance = matched[0].cls(*nested)
             if matched[0].scope is Scope.request:
                 return instance
             matched[0].instance = instance
         return matched[0].instance
 
     @staticmethod
-    def register_instance(cls: Type[T], instance: T, name: str | None = None):
+    def register_instance(cls: Type[T], instance: T, name: str = None):
         _Injector.dependencies.append(Dependency(Scope.singleton, cls, name=name, instance=instance))
 
 
 def init_config():
     """Dependencies configuration using environment variables."""
 
     _Injector.init_config()
 
 
-def inject(name: str | None = None, scope: Scope = Scope.singleton, qualifier: str | None = None):
+def inject(name: str = None, scope: Scope = Scope.singleton, qualifier: str = None):
     """Inject a class or function.
     :param name: Component name.
     :param scope: Class of the Scope in which to resolve.
     :param qualifier: Comma separated string, used to specify components by name in case of multiple implementations.
     """
 
     return _Injector.inject(name, scope, qualifier)
 
 
-async def provide(cls: Type[T], name: str | None = None) -> T:
+async def provide(cls: Type[T], name: str = None) -> T:
     """Get an instance of the given type.
     :param cls: Interface whose implementation we want.
     :param name: Name of a specific component that implements the interface.
     :returns: An implementation of interface.
     """
 
     return await _Injector.provide(cls, name)
 
 
-def register_instance(cls: Type[T], instance: T, name: str | None = None):
+def register_instance(cls: Type[T], instance: T, name: str = None):
     """Create manually and register an instance of a specific type.
     :param cls: Component type.
     :param instance: Component instance.
     :param name: Component name.
     """
 
     return _Injector.register_instance(cls, instance, name)
```

### Comparing `braincube-aws-core-alpha-0.0.25/src/core/rest/app_controller.py` & `braincube-aws-core-alpha-0.0.26/src/core/rest/app_controller.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     :param base_path: base resource url.
     """
 
     def __init__(self, base_path: str):
         self.routes = dict()
         self._base_url = base_path
 
-    def route(self, path: str, method: str, qualifier: str | None = None):
+    def route(self, path: str, method: str, qualifier: str = None):
         """Function that represents an endpoint.
         :param path: Resource url.
         :param method: HTTP method.
         :param qualifier: Comma separated string, used by injection package in order to
          specify components by name in case of multiple implementations.
         """
 
@@ -20,51 +20,51 @@
             if path_ not in self.routes:
                 self.routes[path_] = dict()
             self.routes[path_][method] = func, qualifier
             return func
 
         return _route
 
-    def get(self, path: str = "", qualifier: str | None = None):
+    def get(self, path: str = "", qualifier: str = None):
         """Function that represents an HTTP GET method endpoint.
         :param path: Resource url.
         :param qualifier: Comma separated string, used by injection package in order to
          specify components by name in case of multiple implementations.
         """
 
         return self.route(path, "GET", qualifier)
 
-    def post(self, path: str = "", qualifier: str | None = None):
+    def post(self, path: str = "", qualifier: str = None):
         """Function that represents an HTTP POST method endpoint.
         :param path: Resource url.
         :param qualifier: Comma separated string, used by injection package in order to
          specify components by name in case of multiple implementations.
         """
 
         return self.route(path, "POST", qualifier)
 
-    def patch(self, path: str = "", qualifier: str | None = None):
+    def patch(self, path: str = "", qualifier: str = None):
         """Function that represents an HTTP PATCH method endpoint.
         :param path: Resource url.
         :param qualifier: Comma separated string, used by injection package in order to
          specify components by name in case of multiple implementations.
         """
 
         return self.route(path, "PATCH", qualifier)
 
-    def delete(self, path: str = "", qualifier: str | None = None):
+    def delete(self, path: str = "", qualifier: str = None):
         """Function that represents an HTTP DELETE method endpoint.
         :param path: Resource url.
         :param qualifier: Comma separated string, used by injection package in order to
          specify components by name in case of multiple implementations.
         """
 
         return self.route(path, "DELETE", qualifier)
 
-    def put(self, path: str = "", qualifier: str | None = None):
+    def put(self, path: str = "", qualifier: str = None):
         """Function that represents an HTTP PUT method endpoint.
         :param path: Resource url.
         :param qualifier: Comma separated string, used by injection package in order to
          specify components by name in case of multiple implementations.
         """
 
         return self.route(path, "PUT", qualifier)
```

### Comparing `braincube-aws-core-alpha-0.0.25/src/core/rest/app_module.py` & `braincube-aws-core-alpha-0.0.26/src/core/rest/app_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     """AWS lambda application main entry point.
     :param controllers: Application controllers.
     :param modules: Modules to force import.
     :param directories: Directories to force import.
     """
 
     def __init__(self, controllers: list[AppController],
-                 modules: list[str] | None = None,
-                 directories: list[str] | None = None):
+                 modules: list[str] = None,
+                 directories: list[str] = None):
 
         if modules:
             import_modules(modules)
         elif os.environ.get("IMPORT_MODULES"):
             import_modules(os.environ["IMPORT_MODULES"].split(","))
 
         root = os.environ["ROOT_DIRECTORY"] if os.environ.get("ROOT_DIRECTORY") else "/var/task/"
```

### Comparing `braincube-aws-core-alpha-0.0.25/src/core/rest/data.py` & `braincube-aws-core-alpha-0.0.26/src/core/rest/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 
 
 @dataclass()
 class QueryParameters:
     fields: list[str] = None
     conditions: list[Condition] = None
     page: Pageable = Pageable()
-    order: list[Order] | None = None
+    order: list[Order] = None
 
 
 @dataclass()
 class HTTPRequest(Generic[T]):
     query_parameters: QueryParameters = QueryParameters()
-    body: T | None = None
+    body: T = None
     headers: dict[str, any] = None
     path_parameters: dict[str, any] = None
 
 
 def http_event_to_request(cls: Type[T], event: dict[str, any], context) -> HTTPRequest[T]:
     data = json.loads(event["body"]) if event.get("body") else None
 
@@ -42,17 +42,17 @@
                           event.get("headers"),
                           event.get("pathParameters"))
 
     params: dict[str, any] | None = event.get("queryStringParameters")
 
     if params:
         fields = params["fields"].replace(" ", "").split(",") if params.get("fields") else list()
-        pageable = Pageable(page_param(params, alias="pageNo", default=0),
-                            page_param(params, alias="pageSize", default=20, max_=50),
-                            page_param(params, alias="topSize", default=0, max_=1000))
+        pageable = Pageable(page_param(params, alias="pageNo"),
+                            page_param(params, alias="pageSize", default=20, max_=50, min_=1),
+                            page_param(params, alias="topSize", max_=1000, min_=-1))
 
         conditions = list()
         for k, v in params.items():
             key = k.strip()
             if key in reserved_keys:
                 continue
             else:
@@ -84,19 +84,19 @@
             order.append(Order(order_type, alias=o[0]))
 
         request.query_parameters = QueryParameters(fields, conditions, pageable, order)
 
     return request
 
 
-def page_param(params: dict[str, any], alias: str, default: int, max_: int | None = None) -> int:
+def page_param(params: dict[str, any], alias: str, default: int = 0, max_: int = None, min_: int = 0) -> int:
     try:
         if not params.get(alias):
             return default
         value_ = int(params[alias])
-        return value_ if (max_ >= value_ > 0 if max_ else value_ > 0) else default
+        return value_ if (max_ >= value_ >= min_ if max_ else value_ >= min_) else default
     except ValueError:
         return default
 
 
 def condition_param(type_, p) -> list:
     return [try_str_to_float(i) for i in p[len(type_) + 1:len(p) - 1].replace(" ", "").split(",")]
```

### Comparing `braincube-aws-core-alpha-0.0.25/src/core/utils/convert.py` & `braincube-aws-core-alpha-0.0.26/src/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.25/src/core/utils/data.py` & `braincube-aws-core-alpha-0.0.26/src/core/utils/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     value: any
 
 
 @dataclass()
 class Paging:
     pageNo: int
     pageSize: int
-    totalPages: int | None = None
-    totalCount: int | None = None
+    totalPages: int = None
+    totalCount: int = None
 
 
 @dataclass
 class Metadata:
     dataElapsed: int
```


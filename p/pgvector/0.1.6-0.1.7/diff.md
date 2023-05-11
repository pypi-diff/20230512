# Comparing `tmp/pgvector-0.1.6-py2.py3-none-any.whl.zip` & `tmp/pgvector-0.1.7-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7159 bytes, number of entries: 11
+Zip file size: 7525 bytes, number of entries: 11
 -rw-r--r--  2.0 unx      272 b- defN 21-Jun-23 06:42 pgvector/asyncpg/__init__.py
 -rw-r--r--  2.0 unx     2333 b- defN 22-Jan-14 19:08 pgvector/django/__init__.py
--rw-r--r--  2.0 unx     1349 b- defN 21-Sep-12 20:50 pgvector/psycopg/__init__.py
+-rw-r--r--  2.0 unx     1743 b- defN 23-May-10 04:14 pgvector/psycopg/__init__.py
 -rw-r--r--  2.0 unx      881 b- defN 21-Jun-13 19:29 pgvector/psycopg2/__init__.py
 -rw-r--r--  2.0 unx     1033 b- defN 22-May-23 01:12 pgvector/sqlalchemy/__init__.py
 -rw-r--r--  2.0 unx     1305 b- defN 21-Jun-23 02:28 pgvector/utils/__init__.py
--rw-r--r--  2.0 unx     1083 b- defN 22-May-23 01:17 pgvector-0.1.6.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     5060 b- defN 22-May-23 01:17 pgvector-0.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-May-23 01:17 pgvector-0.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 22-May-23 01:17 pgvector-0.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      904 b- defN 22-May-23 01:17 pgvector-0.1.6.dist-info/RECORD
-11 files, 14339 bytes uncompressed, 5627 bytes compressed:  60.8%
+-rw-r--r--  2.0 unx     1083 b- defN 23-May-11 21:56 pgvector-0.1.7.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     6462 b- defN 23-May-11 21:56 pgvector-0.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-11 21:56 pgvector-0.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-11 21:56 pgvector-0.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      904 b- defN 23-May-11 21:56 pgvector-0.1.7.dist-info/RECORD
+11 files, 16135 bytes uncompressed, 5993 bytes compressed:  62.9%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: pgvector/sqlalchemy/__init__.py
 Comment: 
 
 Filename: pgvector/utils/__init__.py
 Comment: 
 
-Filename: pgvector-0.1.6.dist-info/LICENSE.txt
+Filename: pgvector-0.1.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pgvector-0.1.6.dist-info/METADATA
+Filename: pgvector-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: pgvector-0.1.6.dist-info/WHEEL
+Filename: pgvector-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: pgvector-0.1.6.dist-info/top_level.txt
+Filename: pgvector-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: pgvector-0.1.6.dist-info/RECORD
+Filename: pgvector-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pgvector/psycopg/__init__.py

```diff
@@ -41,16 +41,29 @@
         if isinstance(data, memoryview):
             data = bytes(data)
         return from_db_binary(data)
 
 
 def register_vector(context):
     info = TypeInfo.fetch(context, 'vector')
+    register_vector_info(context, info)
+
+
+async def register_vector_async(context):
+    info = await TypeInfo.fetch(context, 'vector')
+    register_vector_info(context, info)
+
+
+def register_vector_info(context, info):
     if info is None:
         raise psycopg.ProgrammingError('vector type not found in the database')
     info.register(context)
 
+    # add oid to anonymous class for set_types
+    text_dumper = type('', (VectorDumper,), {'oid': info.oid})
+    binary_dumper = type('', (VectorBinaryDumper,), {'oid': info.oid})
+
     adapters = context.adapters
-    adapters.register_dumper('numpy.ndarray', VectorDumper)
-    adapters.register_dumper('numpy.ndarray', VectorBinaryDumper)
+    adapters.register_dumper('numpy.ndarray', text_dumper)
+    adapters.register_dumper('numpy.ndarray', binary_dumper)
     adapters.register_loader(info.oid, VectorLoader)
     adapters.register_loader(info.oid, VectorBinaryLoader)
```

## Comparing `pgvector-0.1.6.dist-info/LICENSE.txt` & `pgvector-0.1.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*


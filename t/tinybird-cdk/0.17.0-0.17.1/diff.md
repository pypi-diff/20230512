# Comparing `tmp/tinybird-cdk-0.17.0.tar.gz` & `tmp/tinybird-cdk-0.17.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinybird-cdk-0.17.0.tar", last modified: Thu May 11 09:21:21 2023, max compression
+gzip compressed data, was "tinybird-cdk-0.17.1.tar", last modified: Fri May 12 08:55:58 2023, max compression
```

## Comparing `tinybird-cdk-0.17.0.tar` & `tinybird-cdk-0.17.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:21:21.691177 tinybird-cdk-0.17.0/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-11 09:21:21.691177 tinybird-cdk-0.17.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25361 2023-05-11 09:21:12.000000 tinybird-cdk-0.17.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 09:21:21.691177 tinybird-cdk-0.17.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-11 09:21:12.000000 tinybird-cdk-0.17.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:21:21.687177 tinybird-cdk-0.17.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tests/test_gcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:21:21.687177 tinybird-cdk-0.17.0/tinybird_cdk/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tinybird_cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:21:21.691177 tinybird-cdk-0.17.0/tinybird_cdk/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tinybird_cdk/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tinybird_cdk/cloud/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tinybird_cdk/cloud/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tinybird_cdk/cloud/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tinybird_cdk/cloud/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tinybird_cdk/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tinybird_cdk/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:21:21.691177 tinybird-cdk-0.17.0/tinybird_cdk/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tinybird_cdk/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tinybird_cdk/connectors/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tinybird_cdk/connectors/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tinybird_cdk/connectors/kinesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tinybird_cdk/connectors/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tinybird_cdk/connectors/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tinybird_cdk/connectors/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    17744 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tinybird_cdk/connectors/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tinybird_cdk/connectors/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tinybird_cdk/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tinybird_cdk/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tinybird_cdk/formats.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tinybird_cdk/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tinybird_cdk/migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tinybird_cdk/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    12911 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tinybird_cdk/tinybird.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-11 09:21:13.000000 tinybird-cdk-0.17.0/tinybird_cdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:21:21.691177 tinybird-cdk-0.17.0/tinybird_cdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-11 09:21:21.000000 tinybird-cdk-0.17.0/tinybird_cdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-11 09:21:21.000000 tinybird-cdk-0.17.0/tinybird_cdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 09:21:21.000000 tinybird-cdk-0.17.0/tinybird_cdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-11 09:21:21.000000 tinybird-cdk-0.17.0/tinybird_cdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-11 09:21:21.000000 tinybird-cdk-0.17.0/tinybird_cdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:55:58.814388 tinybird-cdk-0.17.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-12 08:55:58.814388 tinybird-cdk-0.17.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25361 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 08:55:58.814388 tinybird-cdk-0.17.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:55:58.810388 tinybird-cdk-0.17.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tests/test_gcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:55:58.810388 tinybird-cdk-0.17.1/tinybird_cdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tinybird_cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:55:58.814388 tinybird-cdk-0.17.1/tinybird_cdk/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tinybird_cdk/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tinybird_cdk/cloud/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tinybird_cdk/cloud/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tinybird_cdk/cloud/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tinybird_cdk/cloud/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tinybird_cdk/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tinybird_cdk/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:55:58.814388 tinybird-cdk-0.17.1/tinybird_cdk/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tinybird_cdk/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tinybird_cdk/connectors/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tinybird_cdk/connectors/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tinybird_cdk/connectors/kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tinybird_cdk/connectors/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tinybird_cdk/connectors/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tinybird_cdk/connectors/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17872 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tinybird_cdk/connectors/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tinybird_cdk/connectors/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tinybird_cdk/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tinybird_cdk/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tinybird_cdk/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tinybird_cdk/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tinybird_cdk/migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tinybird_cdk/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12911 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tinybird_cdk/tinybird.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-12 08:55:47.000000 tinybird-cdk-0.17.1/tinybird_cdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:55:58.810388 tinybird-cdk-0.17.1/tinybird_cdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-12 08:55:58.000000 tinybird-cdk-0.17.1/tinybird_cdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-12 08:55:58.000000 tinybird-cdk-0.17.1/tinybird_cdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 08:55:58.000000 tinybird-cdk-0.17.1/tinybird_cdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-12 08:55:58.000000 tinybird-cdk-0.17.1/tinybird_cdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-12 08:55:58.000000 tinybird-cdk-0.17.1/tinybird_cdk.egg-info/top_level.txt
```

### Comparing `tinybird-cdk-0.17.0/README.md` & `tinybird-cdk-0.17.1/README.md`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.0/setup.py` & `tinybird-cdk-0.17.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tinybird-cdk',
-    version='0.17.0',
+    version='0.17.1',
     description="Tinybird's Connector Development Kit.",
     long_description='This package is under active development and currently meant for internal use only.',
     long_description_content_type='text/markdown',
     author='tinybird.co',
     author_email="support@tinybird.co",
     python_requires='>=3.8, <3.12',
     install_requires=[
```

### Comparing `tinybird-cdk-0.17.0/tests/test_gcp.py` & `tinybird-cdk-0.17.1/tests/test_gcp.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.0/tinybird_cdk/cloud/__init__.py` & `tinybird-cdk-0.17.1/tinybird_cdk/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.0/tinybird_cdk/cloud/abstract_client.py` & `tinybird-cdk-0.17.1/tinybird_cdk/cloud/abstract_client.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.0/tinybird_cdk/cloud/gcp.py` & `tinybird-cdk-0.17.1/tinybird_cdk/cloud/gcp.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.0/tinybird_cdk/cloud/gcs.py` & `tinybird-cdk-0.17.1/tinybird_cdk/cloud/gcs.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.0/tinybird_cdk/cloud/s3.py` & `tinybird-cdk-0.17.1/tinybird_cdk/cloud/s3.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.0/tinybird_cdk/config.py` & `tinybird-cdk-0.17.1/tinybird_cdk/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.0/tinybird_cdk/connector.py` & `tinybird-cdk-0.17.1/tinybird_cdk/connector.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.0/tinybird_cdk/connectors/bigquery.py` & `tinybird-cdk-0.17.1/tinybird_cdk/connectors/bigquery.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.0/tinybird_cdk/connectors/kinesis.py` & `tinybird-cdk-0.17.1/tinybird_cdk/connectors/kinesis.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.0/tinybird_cdk/connectors/mysql.py` & `tinybird-cdk-0.17.1/tinybird_cdk/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.0/tinybird_cdk/connectors/postgresql.py` & `tinybird-cdk-0.17.1/tinybird_cdk/connectors/postgresql.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.0/tinybird_cdk/connectors/snowflake.py` & `tinybird-cdk-0.17.1/tinybird_cdk/connectors/snowflake.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,24 +96,15 @@
     #     grant create integration on account to role r_cdk_test;
     #
     # The 'allowed_location' parameter is the GCS path, including the bucket and the workspace-scoped folder.
     # For example: gcs://tinybird-cdk-production-europe-west3/689d9d2b-633b-4900-b6cd-4a8d1d36ac3c/
     #
     # Returns the stage name, and the service account Snowflake generates for the integration. Tinybird Analytics
     # has to grant this account access to the bucket.
-    def create_stage(self, allowed_location , integration_name='tinybird_integration'):
-        if not (database := config.get('SF_DATABASE')):
-            raise errors.MissingConfiguration('database')
-        if not (schema := config.get('SF_SCHEMA')):
-            raise errors.MissingConfiguration('schema')
-        if not (role := config.get('SF_ROLE')):
-            raise errors.MissingConfiguration('role')
-        if not (workspace_id := config.get('TB_WORKSPACE_ID')):
-            raise errors.MissingConfiguration('workspace_id')
-
+    def create_stage(self, allowed_location, integration_name='tinybird_integration', custom_stage_name=None):
 
         # Recreating a storage integration (using CREATE OR REPLACE STORAGE INTEGRATION) breaks the association
         # between the storage integration and any stage that references it.
         #
         # This is because a stage links to a storage integration using a hidden ID rather than the name of
         # the storage integration.
         #
@@ -144,15 +135,15 @@
                     storage_allowed_locations = ({', '.join(f'"{l}"' for l in allowed_locations)});
             ''')
 
         # Create one stage per workspace, since every stage must include the allowed location URL with
         # its workpace id in the path.
         #
         # Replace "-" chars for "_", so we can avoid using quotes in Snowflake resources and complicate everything
-        stage_name = f'{database}.{schema}.tinybird_stage__{workspace_id.replace("-", "_")}__{role}'
+        stage_name = custom_stage_name or self.get_default_stage_name()
         self._query(f'''
             create or replace stage {stage_name}
               url='{allowed_location}'
               file_format = (type = csv compression = none )
               storage_integration = "{integration_name}";
         ''')
 
@@ -173,14 +164,26 @@
                       \tcomment = 'Tinybird Snowflake Connector Integration'
                       \tstorage_allowed_locations = ('{allowed_location}');
 
                       grant create stage on all schemas in database <your_database> to role {role};
 
                       grant ownership on integration "{integration_name}" to role {role};''')
 
+    def get_default_stage_name(self):
+        if not (database := config.get('SF_DATABASE')):
+            raise errors.MissingConfiguration('database')
+        if not (schema := config.get('SF_SCHEMA')):
+            raise errors.MissingConfiguration('schema')
+        if not (role := config.get('SF_ROLE')):
+            raise errors.MissingConfiguration('role')
+        if not (workspace_id := config.get('TB_WORKSPACE_ID')):
+            raise errors.MissingConfiguration('workspace_id')
+
+        return f'{database}.{schema}.tinybird_stage__{workspace_id.replace("-", "_")}__{role}'
+
     #
     # --- Scopes ----------------------------------------------------------------------------------
     #
 
     def get_scopes(self):
         return (
             connector.Scope(name='Databases', value='database'),
```

### Comparing `tinybird-cdk-0.17.0/tinybird_cdk/connectors/sqlite.py` & `tinybird-cdk-0.17.1/tinybird_cdk/connectors/sqlite.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.0/tinybird_cdk/errors.py` & `tinybird-cdk-0.17.1/tinybird_cdk/errors.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.0/tinybird_cdk/export.py` & `tinybird-cdk-0.17.1/tinybird_cdk/export.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.0/tinybird_cdk/formats.py` & `tinybird-cdk-0.17.1/tinybird_cdk/formats.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.0/tinybird_cdk/logger.py` & `tinybird-cdk-0.17.1/tinybird_cdk/logger.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.0/tinybird_cdk/migration.py` & `tinybird-cdk-0.17.1/tinybird_cdk/migration.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.0/tinybird_cdk/schema.py` & `tinybird-cdk-0.17.1/tinybird_cdk/schema.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.0/tinybird_cdk/tinybird.py` & `tinybird-cdk-0.17.1/tinybird_cdk/tinybird.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.0/tinybird_cdk.egg-info/SOURCES.txt` & `tinybird-cdk-0.17.1/tinybird_cdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*


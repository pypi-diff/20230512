# Comparing `tmp/caraml-store-0.1.3.tar.gz` & `tmp/caraml-store-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/caraml-store-0.1.3.tar", last modified: Tue Mar 14 08:56:43 2023, max compression
+gzip compressed data, was "dist/caraml-store-0.1.4.tar", last modified: Fri May 12 07:15:15 2023, max compression
```

## Comparing `caraml-store-0.1.3.tar` & `caraml-store-0.1.4.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:56:43.000000 caraml-store-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-14 08:56:32.000000 caraml-store-0.1.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-03-14 08:56:43.000000 caraml-store-0.1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:56:43.000000 caraml-store-0.1.3/caraml_store.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-03-14 08:56:42.000000 caraml-store-0.1.3/caraml_store.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-03-14 08:56:43.000000 caraml-store-0.1.3/caraml_store.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 08:56:42.000000 caraml-store-0.1.3/caraml_store.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-14 08:56:42.000000 caraml-store-0.1.3/caraml_store.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-14 08:56:42.000000 caraml-store-0.1.3/caraml_store.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:56:43.000000 caraml-store-0.1.3/feast/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:56:43.000000 caraml-store-0.1.3/feast/core/
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/CoreService_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    28424 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/CoreService_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    30397 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/CoreService_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/DataFormat_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/DataFormat_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/DataFormat_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/DataSource_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/DataSource_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/DataSource_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/Entity_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/Entity_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/Entity_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/FeatureTable_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/FeatureTable_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/FeatureTable_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/Feature_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/Feature_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/Feature_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/LegacyJobService_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/LegacyJobService_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/LegacyJobService_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/OnlineStore_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/OnlineStore_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/OnlineStore_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/SparkOverride_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/SparkOverride_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/SparkOverride_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/data_format.py
--rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/feature_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:56:43.000000 caraml-store-0.1.3/feast/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/gcp/staging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:56:43.000000 caraml-store-0.1.3/feast/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/loaders/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/online_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/online_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:56:43.000000 caraml-store-0.1.3/feast/serving/
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/serving/ServingService_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/serving/ServingService_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/serving/ServingService_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/serving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:56:43.000000 caraml-store-0.1.3/feast/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/types/Field_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/types/Field_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/types/Value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9887 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/types/Value_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast/value_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:56:43.000000 caraml-store-0.1.3/feast_spark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast_spark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:56:43.000000 caraml-store-0.1.3/feast_spark/api/
--rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast_spark/api/JobService_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20503 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast_spark/api/JobService_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast_spark/api/JobService_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 08:56:32.000000 caraml-store-0.1.3/feast_spark/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-14 08:56:32.000000 caraml-store-0.1.3/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-14 08:56:32.000000 caraml-store-0.1.3/requirements-ci.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 08:56:43.000000 caraml-store-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-03-14 08:56:32.000000 caraml-store-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:56:43.000000 caraml-store-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 08:56:32.000000 caraml-store-0.1.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:56:43.000000 caraml-store-0.1.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-14 08:56:32.000000 caraml-store-0.1.3/tests/data/test_feature_table.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-03-14 08:56:32.000000 caraml-store-0.1.3/tests/test_model_protobuf_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 08:56:43.000000 caraml-store-0.1.3/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      932 2023-03-14 08:56:32.000000 caraml-store-0.1.3/utils/compile_protos.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:15:15.000000 caraml-store-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-12 07:15:02.000000 caraml-store-0.1.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-12 07:15:15.000000 caraml-store-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 07:15:02.000000 caraml-store-0.1.4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:15:15.000000 caraml-store-0.1.4/caraml_store.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-12 07:15:15.000000 caraml-store-0.1.4/caraml_store.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-12 07:15:15.000000 caraml-store-0.1.4/caraml_store.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 07:15:15.000000 caraml-store-0.1.4/caraml_store.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-12 07:15:15.000000 caraml-store-0.1.4/caraml_store.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-12 07:15:15.000000 caraml-store-0.1.4/caraml_store.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:15:15.000000 caraml-store-0.1.4/feast/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13615 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:15:15.000000 caraml-store-0.1.4/feast/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/CoreService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28424 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/CoreService_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    30397 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/CoreService_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/DataFormat_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/DataFormat_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/DataFormat_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/DataSource_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/DataSource_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/DataSource_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/Entity_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/Entity_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/Entity_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/FeatureTable_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/FeatureTable_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/FeatureTable_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/Feature_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/Feature_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/Feature_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/LegacyJobService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/LegacyJobService_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/LegacyJobService_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/OnlineStore_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/OnlineStore_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/OnlineStore_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/SparkOverride_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/SparkOverride_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/SparkOverride_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/data_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/feature_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:15:15.000000 caraml-store-0.1.4/feast/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/gcp/staging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:15:15.000000 caraml-store-0.1.4/feast/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/loaders/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/online_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/online_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:15:15.000000 caraml-store-0.1.4/feast/serving/
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/serving/ServingService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/serving/ServingService_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/serving/ServingService_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/serving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:15:15.000000 caraml-store-0.1.4/feast/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/types/Field_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/types/Field_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/types/Value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9887 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/types/Value_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast/value_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:15:15.000000 caraml-store-0.1.4/feast_spark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast_spark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:15:15.000000 caraml-store-0.1.4/feast_spark/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast_spark/api/JobService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20503 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast_spark/api/JobService_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast_spark/api/JobService_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 07:15:02.000000 caraml-store-0.1.4/feast_spark/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-12 07:15:02.000000 caraml-store-0.1.4/requirements-build.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-12 07:15:02.000000 caraml-store-0.1.4/requirements-ci.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 07:15:15.000000 caraml-store-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-12 07:15:02.000000 caraml-store-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:15:15.000000 caraml-store-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 07:15:02.000000 caraml-store-0.1.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:15:15.000000 caraml-store-0.1.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-12 07:15:02.000000 caraml-store-0.1.4/tests/data/test_feature_table.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-12 07:15:02.000000 caraml-store-0.1.4/tests/test_model_protobuf_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:15:15.000000 caraml-store-0.1.4/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      936 2023-05-12 07:15:02.000000 caraml-store-0.1.4/utils/compile_protos.sh
```

### Comparing `caraml-store-0.1.3/caraml_store.egg-info/SOURCES.txt` & `caraml-store-0.1.4/caraml_store.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 Dockerfile
+__init__.py
 requirements-build.txt
 requirements-ci.txt
 setup.py
 caraml_store.egg-info/PKG-INFO
 caraml_store.egg-info/SOURCES.txt
 caraml_store.egg-info/dependency_links.txt
 caraml_store.egg-info/requires.txt
```

### Comparing `caraml-store-0.1.3/feast/client.py` & `caraml-store-0.1.4/feast/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from feast.core.CoreService_pb2 import (
     ListOnlineStoresRequest,
     ListOnlineStoresResponse,
     GetFeatureTableRequest,
     ApplyFeatureTableRequest,
     ListProjectsRequest,
     ListFeatureTablesRequest,
+    DeleteFeatureTableRequest,
     GetEntityRequest,
     ListEntitiesRequest,
     ApplyEntityRequest,
 )
 from feast.data_source import FileSource, BigQuerySource
 from feast.entity import Entity
 from feast.feature import build_feature_references
@@ -365,7 +366,17 @@
             job_id: spark job id
 
         Returns: Job protobuf object
         """
         request = GetJobRequest(job_id=job_id)
         response = self._job_service.GetJob(request)
         return response.job
+
+    def delete_feature_table(self, feature_table: str, project: str):
+        """
+        Delete Feature Table
+        Args:
+            feature_table: feature table name
+            project: project name
+        """
+        request = DeleteFeatureTableRequest(name=feature_table, project=project)
+        self._core_service.DeleteFeatureTable(request)
```

### Comparing `caraml-store-0.1.3/feast/core/CoreService_pb2.py` & `caraml-store-0.1.4/feast/core/CoreService_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/core/CoreService_pb2.pyi` & `caraml-store-0.1.4/feast/core/CoreService_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/core/CoreService_pb2_grpc.py` & `caraml-store-0.1.4/feast/core/CoreService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/core/DataFormat_pb2.py` & `caraml-store-0.1.4/feast/core/DataFormat_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/core/DataFormat_pb2.pyi` & `caraml-store-0.1.4/feast/core/DataFormat_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/core/DataSource_pb2.py` & `caraml-store-0.1.4/feast/core/DataSource_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/core/DataSource_pb2.pyi` & `caraml-store-0.1.4/feast/core/DataSource_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/core/Entity_pb2.py` & `caraml-store-0.1.4/feast/core/Entity_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/core/Entity_pb2.pyi` & `caraml-store-0.1.4/feast/core/Entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/core/FeatureTable_pb2.py` & `caraml-store-0.1.4/feast/core/FeatureTable_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/core/FeatureTable_pb2.pyi` & `caraml-store-0.1.4/feast/core/FeatureTable_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/core/Feature_pb2.py` & `caraml-store-0.1.4/feast/core/Feature_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/core/Feature_pb2.pyi` & `caraml-store-0.1.4/feast/core/Feature_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/core/LegacyJobService_pb2.py` & `caraml-store-0.1.4/feast/core/LegacyJobService_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/core/LegacyJobService_pb2_grpc.py` & `caraml-store-0.1.4/feast/core/LegacyJobService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/core/OnlineStore_pb2.py` & `caraml-store-0.1.4/feast/core/OnlineStore_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/core/OnlineStore_pb2.pyi` & `caraml-store-0.1.4/feast/core/OnlineStore_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/core/SparkOverride_pb2.py` & `caraml-store-0.1.4/feast/core/SparkOverride_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/core/SparkOverride_pb2.pyi` & `caraml-store-0.1.4/feast/core/SparkOverride_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/data_format.py` & `caraml-store-0.1.4/feast/data_format.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/data_source.py` & `caraml-store-0.1.4/feast/data_source.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/entity.py` & `caraml-store-0.1.4/feast/entity.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/feature.py` & `caraml-store-0.1.4/feast/feature.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/feature_table.py` & `caraml-store-0.1.4/feast/feature_table.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/gcp/staging.py` & `caraml-store-0.1.4/feast/gcp/staging.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/loaders/file.py` & `caraml-store-0.1.4/feast/loaders/file.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/online_response.py` & `caraml-store-0.1.4/feast/online_response.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/online_store.py` & `caraml-store-0.1.4/feast/online_store.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/serving/ServingService_pb2.py` & `caraml-store-0.1.4/feast/serving/ServingService_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/serving/ServingService_pb2.pyi` & `caraml-store-0.1.4/feast/serving/ServingService_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/serving/ServingService_pb2_grpc.py` & `caraml-store-0.1.4/feast/serving/ServingService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/types/Field_pb2.py` & `caraml-store-0.1.4/feast/types/Field_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/types/Field_pb2.pyi` & `caraml-store-0.1.4/feast/types/Field_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/types/Value_pb2.py` & `caraml-store-0.1.4/feast/types/Value_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast/types/Value_pb2.pyi` & `caraml-store-0.1.4/feast/types/Value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast_spark/api/JobService_pb2.py` & `caraml-store-0.1.4/feast_spark/api/JobService_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast_spark/api/JobService_pb2.pyi` & `caraml-store-0.1.4/feast_spark/api/JobService_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/feast_spark/api/JobService_pb2_grpc.py` & `caraml-store-0.1.4/feast_spark/api/JobService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/setup.py` & `caraml-store-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(exclude=("tests",)),
     install_requires=REQUIRED,
     extras_require=EXTRA_REQUIRED,
-    use_scm_version={"root": "..", "relative_to": __file__, "tag_regex": TAG_REGEX},
+    use_scm_version={"root": "../..", "relative_to": __file__, "tag_regex": TAG_REGEX},
     setup_requires=["setuptools_scm"],
     # https://stackoverflow.com/questions/28509965/setuptools-development-requirements
     # Install dev requirements with: pip install -e .[dev]
     license="Apache",
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
```

### Comparing `caraml-store-0.1.3/tests/data/test_feature_table.yaml` & `caraml-store-0.1.4/tests/data/test_feature_table.yaml`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/tests/test_model_protobuf_conversion.py` & `caraml-store-0.1.4/tests/test_model_protobuf_conversion.py`

 * *Files identical despite different names*

### Comparing `caraml-store-0.1.3/utils/compile_protos.sh` & `caraml-store-0.1.4/utils/compile_protos.sh`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 fi
 
 PROTOS_PACKAGE_PATH=$1
 PROTOS_DIR="${PROTOS_PACKAGE_PATH}/src/main/proto"
 
 cd "${PROTOS_DIR}" || { echo "Proto directory - ${PROTOS_DIR} doesn't exist !!"; exit 2; }
 
-OUT_DIR=${PROTOS_PACKAGE_PATH}/../caraml-store-python
+OUT_DIR=${PROTOS_PACKAGE_PATH}/../caraml-store-sdk/python
 mkdir -p "${OUT_DIR}"
 
 PROTO_TYPE_SUBDIRS="core serving types"
 for dir in ${PROTO_TYPE_SUBDIRS}
 do
   python -m grpc_tools.protoc -I. --python_out="${OUT_DIR}" --mypy_out="${OUT_DIR}" feast/"${dir}"/*.proto;
 done
```


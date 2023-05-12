# Comparing `tmp/cognite_sdk-6.1.7.tar.gz` & `tmp/cognite_sdk-6.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-6.1.7.tar", max compression
+gzip compressed data, was "cognite_sdk-6.1.8.tar", max compression
```

## Comparing `cognite_sdk-6.1.7.tar` & `cognite_sdk-6.1.8.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0    11349 2023-05-12 08:45:20.915643 cognite_sdk-6.1.7/LICENSE
--rw-r--r--   0        0        0     3945 2023-05-12 08:45:20.915643 cognite_sdk-6.1.7/README.md
--rw-r--r--   0        0        0      503 2023-05-12 08:45:20.915643 cognite_sdk-6.1.7/cognite/client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 08:45:20.915643 cognite_sdk-6.1.7/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     6979 2023-05-12 08:45:20.915643 cognite_sdk-6.1.7/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    48450 2023-05-12 08:45:20.915643 cognite_sdk-6.1.7/cognite/client/_api/assets.py
--rw-r--r--   0        0        0    11025 2023-05-12 08:45:20.915643 cognite_sdk-6.1.7/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    54681 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    87464 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    12474 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    12245 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    20644 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_api/events.py
--rw-r--r--   0        0        0    17436 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    41397 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_api/files.py
--rw-r--r--   0        0        0    44308 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    49922 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0     9297 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6052 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_api/labels.py
--rw-r--r--   0        0        0    24648 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    22824 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    37975 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     7909 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    32132 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    27928 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    19140 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    21039 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     4983 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4638 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9570 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     1869 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     5910 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    36997 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_api_client.py
--rw-r--r--   0        0        0     5245 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      140 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_constants.py
--rw-r--r--   0        0        0     6501 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_http_client.py
--rw-r--r--   0        0        0      553 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     1985 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2495 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0     9509 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/beta.py
--rw-r--r--   0        0        0     4508 2023-05-12 08:45:20.919643 cognite_sdk-6.1.7/cognite/client/config.py
--rw-r--r--   0        0        0    18062 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/credentials.py
--rw-r--r--   0        0        0     8794 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    18565 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0        0 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     1595 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     2936 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0     8741 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    34178 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    33582 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     6682 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    33940 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    11008 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    14287 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    13657 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    16631 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    16465 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     6003 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5868 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     4098 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    12253 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    17651 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     8699 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0    16814 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    11789 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    12078 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    23040 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    11319 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    11425 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2354 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2451 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     2742 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     9383 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/py.typed
--rw-r--r--   0        0        0     8194 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/testing.py
--rw-r--r--   0        0        0      534 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     7894 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0     9511 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1396 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0     5919 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     2134 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     3548 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     6188 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/utils/_priority_tpe.py
--rw-r--r--   0        0        0     4149 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     2001 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/utils/_text.py
--rw-r--r--   0        0        0    24536 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     1820 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/utils/_validation.py
--rw-r--r--   0        0        0     3341 2023-05-12 08:45:20.923642 cognite_sdk-6.1.7/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0     2132 2023-05-12 08:45:20.927642 cognite_sdk-6.1.7/pyproject.toml
--rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-12 14:54:13.235233 cognite_sdk-6.1.8/LICENSE
+-rw-r--r--   0        0        0     3945 2023-05-12 14:54:13.235233 cognite_sdk-6.1.8/README.md
+-rw-r--r--   0        0        0      503 2023-05-12 14:54:13.235233 cognite_sdk-6.1.8/cognite/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 14:54:13.235233 cognite_sdk-6.1.8/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     6979 2023-05-12 14:54:13.235233 cognite_sdk-6.1.8/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    48450 2023-05-12 14:54:13.235233 cognite_sdk-6.1.8/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0    11025 2023-05-12 14:54:13.235233 cognite_sdk-6.1.8/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    54681 2023-05-12 14:54:13.235233 cognite_sdk-6.1.8/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    87464 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    12474 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    12245 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    20644 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    17419 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    41397 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    44308 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    49922 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0     9297 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6052 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0    24648 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    22824 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    37975 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     7909 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    32132 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    27928 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    19140 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    21039 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     4983 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4638 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9570 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     1869 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     5910 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    36997 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_api_client.py
+-rw-r--r--   0        0        0     5245 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      140 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6501 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      553 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     1985 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2495 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0     9509 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/beta.py
+-rw-r--r--   0        0        0     4508 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/config.py
+-rw-r--r--   0        0        0    18062 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/credentials.py
+-rw-r--r--   0        0        0     8794 2023-05-12 14:54:13.239233 cognite_sdk-6.1.8/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    18565 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0        0 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     1595 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     2936 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0     8741 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    34178 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    33582 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     6682 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    33940 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    11008 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    14299 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    13657 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    16631 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    16465 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     6003 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     5868 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     4098 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    12253 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    17651 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     8699 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0    16814 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    11789 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    12078 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    23040 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    11319 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    11425 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2354 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2451 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     2742 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0     9383 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/py.typed
+-rw-r--r--   0        0        0     8194 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/testing.py
+-rw-r--r--   0        0        0      534 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     7894 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0     9511 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1396 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0     5919 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     2134 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     3548 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     6188 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/utils/_priority_tpe.py
+-rw-r--r--   0        0        0     4149 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     2001 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0    24536 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     1820 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/utils/_validation.py
+-rw-r--r--   0        0        0     3341 2023-05-12 14:54:13.243233 cognite_sdk-6.1.8/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0     2132 2023-05-12 14:54:13.247234 cognite_sdk-6.1.8/pyproject.toml
+-rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.1.8/PKG-INFO
```

### Comparing `cognite_sdk-6.1.7/LICENSE` & `cognite_sdk-6.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/README.md` & `cognite_sdk-6.1.8/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/annotations.py` & `cognite_sdk-6.1.8/cognite/client/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/assets.py` & `cognite_sdk-6.1.8/cognite/client/_api/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/data_sets.py` & `cognite_sdk-6.1.8/cognite/client/_api/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-6.1.8/cognite/client/_api/datapoint_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/datapoints.py` & `cognite_sdk-6.1.8/cognite/client/_api/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/diagrams.py` & `cognite_sdk-6.1.8/cognite/client/_api/diagrams.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/entity_matching.py` & `cognite_sdk-6.1.8/cognite/client/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/events.py` & `cognite_sdk-6.1.8/cognite/client/_api/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-6.1.8/cognite/client/_api/extractionpipelines.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Dict, Optional, Sequence, Union, overload
+from typing import TYPE_CHECKING, Any, Dict, Literal, Optional, Sequence, Union, overload
 
 from cognite.client import utils
 from cognite.client._api_client import APIClient
 from cognite.client._constants import LIST_LIMIT_DEFAULT
 from cognite.client.data_classes import (
     ExtractionPipeline,
     ExtractionPipelineConfig,
@@ -260,29 +260,29 @@
         if statuses is not None or message_substring is not None or created_time is not None:
             filter = ExtractionPipelineRunFilter(
                 external_id=external_id,
                 statuses=statuses,
                 message=StringFilter(substring=message_substring),
                 created_time=created_time,
             ).dump(camel_case=True)
-            return self._list(
-                list_cls=ExtractionPipelineRunList,
-                resource_cls=ExtractionPipelineRun,
-                method="POST",
-                limit=limit,
-                filter=filter,
-            )
+            method: Literal["POST", "GET"] = "POST"
+        else:
+            filter = {"externalId": external_id}
+            method = "GET"
 
-        return self._list(
+        res = self._list(
             list_cls=ExtractionPipelineRunList,
             resource_cls=ExtractionPipelineRun,
-            method="GET",
+            method=method,
             limit=limit,
-            filter={"externalId": external_id},
+            filter=filter,
         )
+        for run in res:
+            run.extpipe_external_id = external_id
+        return res
 
     @overload
     def create(self, run: ExtractionPipelineRun) -> ExtractionPipelineRun:
         ...
 
     @overload
     def create(self, run: Sequence[ExtractionPipelineRun]) -> ExtractionPipelineRunList:
```

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/files.py` & `cognite_sdk-6.1.8/cognite/client/_api/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/functions.py` & `cognite_sdk-6.1.8/cognite/client/_api/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/geospatial.py` & `cognite_sdk-6.1.8/cognite/client/_api/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/iam.py` & `cognite_sdk-6.1.8/cognite/client/_api/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/labels.py` & `cognite_sdk-6.1.8/cognite/client/_api/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/raw.py` & `cognite_sdk-6.1.8/cognite/client/_api/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/relationships.py` & `cognite_sdk-6.1.8/cognite/client/_api/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/sequences.py` & `cognite_sdk-6.1.8/cognite/client/_api/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-6.1.8/cognite/client/_api/synthetic_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/templates.py` & `cognite_sdk-6.1.8/cognite/client/_api/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/three_d.py` & `cognite_sdk-6.1.8/cognite/client/_api/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/time_series.py` & `cognite_sdk-6.1.8/cognite/client/_api/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-6.1.8/cognite/client/_api/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-6.1.8/cognite/client/_api/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-6.1.8/cognite/client/_api/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-6.1.8/cognite/client/_api/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/transformations/schema.py` & `cognite_sdk-6.1.8/cognite/client/_api/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api/vision.py` & `cognite_sdk-6.1.8/cognite/client/_api/vision.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_api_client.py` & `cognite_sdk-6.1.8/cognite/client/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_cognite_client.py` & `cognite_sdk-6.1.8/cognite/client/_cognite_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_http_client.py` & `cognite_sdk-6.1.8/cognite/client/_http_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-6.1.8/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-6.1.8/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-6.1.8/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_proto/data_points.proto` & `cognite_sdk-6.1.8/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-6.1.8/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-6.1.8/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-6.1.8/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-6.1.8/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-6.1.8/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-6.1.8/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/config.py` & `cognite_sdk-6.1.8/cognite/client/config.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/credentials.py` & `cognite_sdk-6.1.8/cognite/client/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/__init__.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/_base.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/annotations.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/assets.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/contextualization.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/data_sets.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/datapoints.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/events.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/extractionpipelines.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,17 +238,17 @@
         # Note: No way to make this id/xid API mixup completely correct. Either:
         # 1. We use id / external_id for respecively "self id" / "ext.pipe external id"
         #   - Problem: Only dataclass in the SDK where id and external_id does not point to same object...
         # 2. We rename external_id to extpipe_external_id in the SDK only
         #   - Problem: This dump method might be surprising to the user - if used (its public)...
         # ...and 2 was chosen:
         if camel_case:
-            dct["externalId"] = dct.pop("extpipeExternalId")
+            dct["externalId"] = dct.pop("extpipeExternalId", None)
         else:
-            dct["external_id"] = dct.pop("extpipe_external_id")
+            dct["external_id"] = dct.pop("extpipe_external_id", None)
         return dct
 
 
 class ExtractionPipelineRunList(CogniteResourceList):
     _RESOURCE = ExtractionPipelineRun
```

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/files.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/functions.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/geospatial.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/iam.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/labels.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/raw.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/relationships.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/sequences.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/shared.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/templates.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/three_d.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/time_series.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/transformations/common.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/data_classes/transformations/schema.py` & `cognite_sdk-6.1.8/cognite/client/data_classes/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/exceptions.py` & `cognite_sdk-6.1.8/cognite/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/testing.py` & `cognite_sdk-6.1.8/cognite/client/testing.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/utils/__init__.py` & `cognite_sdk-6.1.8/cognite/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/utils/_auxiliary.py` & `cognite_sdk-6.1.8/cognite/client/utils/_auxiliary.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/utils/_concurrency.py` & `cognite_sdk-6.1.8/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/utils/_graph.py` & `cognite_sdk-6.1.8/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/utils/_identifier.py` & `cognite_sdk-6.1.8/cognite/client/utils/_identifier.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/utils/_logging.py` & `cognite_sdk-6.1.8/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-6.1.8/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/utils/_priority_tpe.py` & `cognite_sdk-6.1.8/cognite/client/utils/_priority_tpe.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-6.1.8/cognite/client/utils/_pyodide_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/utils/_text.py` & `cognite_sdk-6.1.8/cognite/client/utils/_text.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/utils/_time.py` & `cognite_sdk-6.1.8/cognite/client/utils/_time.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/utils/_validation.py` & `cognite_sdk-6.1.8/cognite/client/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/cognite/client/utils/_version_checker.py` & `cognite_sdk-6.1.8/cognite/client/utils/_version_checker.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.7/pyproject.toml` & `cognite_sdk-6.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "6.1.7"
+version = "6.1.8"
 
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = ["Erlend Vollset <erlend.vollset@cognite.com>"]
 license = "Apache-2.0"
```

### Comparing `cognite_sdk-6.1.7/PKG-INFO` & `cognite_sdk-6.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 6.1.7
+Version: 6.1.8
 Summary: Cognite Python SDK
 License: Apache-2.0
 Author: Erlend Vollset
 Author-email: erlend.vollset@cognite.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognite-sdk Version: 6.1.7 Summary: Cognite Python
+Metadata-Version: 2.1 Name: cognite-sdk Version: 6.1.8 Summary: Cognite Python
 SDK License: Apache-2.0 Author: Erlend Vollset Author-email:
 erlend.vollset@cognite.com Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-
 Extra: all Provides-Extra: functions Provides-Extra: geo Provides-Extra: numpy
```


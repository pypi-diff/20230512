# Comparing `tmp/cognite_transformations_cli-2.3.5.tar.gz` & `tmp/cognite_transformations_cli-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_transformations_cli-2.3.5.tar", max compression
+gzip compressed data, was "cognite_transformations_cli-2.3.6.tar", max compression
```

## Comparing `cognite_transformations_cli-2.3.5.tar` & `cognite_transformations_cli-2.3.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    10172 2023-05-10 15:06:52.945631 cognite_transformations_cli-2.3.5/LICENSE
--rw-r--r--   0        0        0     4288 2023-05-10 15:06:52.945631 cognite_transformations_cli-2.3.5/README.md
--rw-r--r--   0        0        0       22 2023-05-10 15:06:52.945631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/__init__.py
--rw-r--r--   0        0        0      270 2023-05-10 15:06:52.945631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/__main__.py
--rw-r--r--   0        0        0     1489 2023-05-10 15:06:52.945631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/clients.py
--rw-r--r--   0        0        0        0 2023-05-10 15:06:52.945631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/__init__.py
--rw-r--r--   0        0        0     3615 2023-05-10 15:06:52.945631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/base.py
--rw-r--r--   0        0        0     1491 2023-05-10 15:06:52.945631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/delete.py
--rw-r--r--   0        0        0        0 2023-05-10 15:06:52.945631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/__init__.py
--rw-r--r--   0        0        0     6459 2023-05-10 15:06:52.945631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/deploy.py
--rw-r--r--   0        0        0     6754 2023-05-10 15:06:52.945631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/load_yaml.py
--rw-r--r--   0        0        0     5351 2023-05-10 15:06:52.945631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/transformation_config.py
--rw-r--r--   0        0        0     4342 2023-05-10 15:06:52.949631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/transformation_types.py
--rw-r--r--   0        0        0     4705 2023-05-10 15:06:52.949631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/transformation_types_legacy.py
--rw-r--r--   0        0        0    13069 2023-05-10 15:06:52.949631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/transformations_api.py
--rw-r--r--   0        0        0     2166 2023-05-10 15:06:52.949631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/jobs.py
--rw-r--r--   0        0        0     2438 2023-05-10 15:06:52.949631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/list.py
--rw-r--r--   0        0        0     1242 2023-05-10 15:06:52.949631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/query.py
--rw-r--r--   0        0        0     3639 2023-05-10 15:06:52.949631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/run.py
--rw-r--r--   0        0        0     2787 2023-05-10 15:06:52.949631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/show.py
--rw-r--r--   0        0        0     5792 2023-05-10 15:06:52.949631 cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/utils.py
--rw-r--r--   0        0        0     1616 2023-05-10 15:06:52.949631 cognite_transformations_cli-2.3.5/pyproject.toml
--rw-r--r--   0        0        0     5474 1970-01-01 00:00:00.000000 cognite_transformations_cli-2.3.5/PKG-INFO
+-rw-r--r--   0        0        0    10172 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/LICENSE
+-rw-r--r--   0        0        0     4288 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/README.md
+-rw-r--r--   0        0        0       22 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/__init__.py
+-rw-r--r--   0        0        0      270 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/__main__.py
+-rw-r--r--   0        0        0     1489 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/clients.py
+-rw-r--r--   0        0        0        0 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/__init__.py
+-rw-r--r--   0        0        0     3615 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/base.py
+-rw-r--r--   0        0        0     1491 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/delete.py
+-rw-r--r--   0        0        0        0 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/__init__.py
+-rw-r--r--   0        0        0     6459 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/deploy.py
+-rw-r--r--   0        0        0     6754 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/load_yaml.py
+-rw-r--r--   0        0        0     4998 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/transformation_config.py
+-rw-r--r--   0        0        0     4005 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/transformation_types.py
+-rw-r--r--   0        0        0     4705 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/transformation_types_legacy.py
+-rw-r--r--   0        0        0    12780 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/transformations_api.py
+-rw-r--r--   0        0        0     2166 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/jobs.py
+-rw-r--r--   0        0        0     2438 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/list.py
+-rw-r--r--   0        0        0     1242 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/query.py
+-rw-r--r--   0        0        0     3639 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/run.py
+-rw-r--r--   0        0        0     2787 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/show.py
+-rw-r--r--   0        0        0     5792 2023-05-12 09:48:30.485538 cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/utils.py
+-rw-r--r--   0        0        0     1616 2023-05-12 09:48:30.489539 cognite_transformations_cli-2.3.6/pyproject.toml
+-rw-r--r--   0        0        0     5474 1970-01-01 00:00:00.000000 cognite_transformations_cli-2.3.6/PKG-INFO
```

### Comparing `cognite_transformations_cli-2.3.5/LICENSE` & `cognite_transformations_cli-2.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.5/README.md` & `cognite_transformations_cli-2.3.6/README.md`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.5/cognite/transformations_cli/clients.py` & `cognite_transformations_cli-2.3.6/cognite/transformations_cli/clients.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/base.py` & `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/delete.py` & `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/delete.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/deploy.py` & `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/deploy.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/load_yaml.py` & `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/load_yaml.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/transformation_config.py` & `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/transformation_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,14 @@
     # DestinationConfig and DestinationType cannot be used for the types such as raw and sequence_rows
     if isinstance(destination_type, DestinationConfig) or isinstance(destination_type, DestinationType):
         if flat_destination_type == DestinationType.raw:
             raise Exception(
                 f"Error on transformation manifest with external ID {external_id}: \
                             Raw destination type requires database and table properties to be set."
             )
-        if flat_destination_type == DestinationType.data_model_instances:
-            raise Exception(
-                f"Error on transformation manifest with external ID {external_id}: Data model instances destination requires model_external_id,  \
-                            space_external_id and instance_space_external_id to be set."
-            )
         if flat_destination_type == DestinationType.nodes:
             raise Exception(
                 f"Error on transformation manifest with external ID {external_id}: Nodes destination requires view space,  \
                             view external_id, view version and instance_space to be set."
             )
         if flat_destination_type == DestinationType.edges:
             raise Exception(
```

### Comparing `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/transformation_types.py` & `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/transformation_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     sequences = "sequences"
     files = "files"
     labels = "labels"
     relationships = "relationships"
     raw = "raw"
     data_sets = "data_sets"
     sequence_rows = "sequence_rows"
-    data_model_instances = "data_model_instances"
     nodes = "nodes"
     edges = "edges"
 
 
 class ActionType(Enum):
     create = "create"
     abort = "abort"
@@ -75,26 +74,14 @@
 
     database: str
     table: str
     type: DestinationType = DestinationType.raw
 
 
 @dataclass
-class DMIDestinationConfig:
-    """
-    Valid type values are: data_model_instances
-    """
-
-    model_external_id: str
-    space_external_id: str
-    instance_space_external_id: str
-    type: DestinationType = DestinationType.data_model_instances
-
-
-@dataclass
 class ViewInfo:
     space: str
     external_id: str
     version: Union[int, str]
 
     """
     CAST view version int to string
@@ -148,15 +135,14 @@
 
 
 DestinationConfigType = Union[
     DestinationType,
     DestinationConfig,
     RawDestinationConfig,
     SequenceRowsDestinationConfig,
-    DMIDestinationConfig,
     InstanceNodesDestinationConfig,
     InstanceEdgesDestinationConfig,
     RawDestinationAlternativeConfig,
 ]
 
 
 @dataclass
```

### Comparing `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/transformation_types_legacy.py` & `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/transformation_types_legacy.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/deploy/transformations_api.py` & `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/deploy/transformations_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,29 +8,27 @@
     Transformation,
     TransformationDestination,
     TransformationNotification,
     TransformationSchedule,
     TransformationUpdate,
 )
 from cognite.client.data_classes.transformations.common import (
-    DataModelInstances,
     EdgeType,
     InstanceEdges,
     InstanceNodes,
     SequenceRows,
     ViewInfo,
 )
 from cognite.client.exceptions import CogniteAPIError, CogniteDuplicatedError, CogniteNotFoundError
 
 from cognite.transformations_cli.commands.deploy.transformation_types import (
     ActionType,
     AuthConfig,
     DestinationConfig,
     DestinationConfigType,
-    DMIDestinationConfig,
     InstanceEdgesDestinationConfig,
     InstanceNodesDestinationConfig,
     QueryConfig,
     RawDestinationAlternativeConfig,
     RawDestinationConfig,
     ReadWriteAuthentication,
     ScheduleConfig,
@@ -94,20 +92,14 @@
         return TransformationDestination(destination.type.value)
     elif isinstance(destination, RawDestinationConfig):
         return TransformationDestination.raw(destination.raw_database, destination.raw_table)
     elif isinstance(destination, RawDestinationAlternativeConfig):
         return TransformationDestination.raw(destination.database, destination.table)
     elif isinstance(destination, SequenceRowsDestinationConfig):
         return SequenceRows(destination.external_id)
-    elif isinstance(destination, DMIDestinationConfig):
-        return DataModelInstances(
-            destination.model_external_id,
-            destination.space_external_id,
-            destination.instance_space_external_id,
-        )
 
     elif isinstance(destination, InstanceNodesDestinationConfig):
         view = None
         if destination.view:
             view = ViewInfo(
                 destination.view.space,
                 destination.view.external_id,
```

### Comparing `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/jobs.py` & `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/list.py` & `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/query.py` & `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/query.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/run.py` & `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/run.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/show.py` & `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/show.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.5/cognite/transformations_cli/commands/utils.py` & `cognite_transformations_cli-2.3.6/cognite/transformations_cli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.5/pyproject.toml` & `cognite_transformations_cli-2.3.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-transformations-cli"
-version = "2.3.5"
+version = "2.3.6"
 description = "A CLI for the Transformations service in CDF"
 authors = ["Mathias Lohne <mathias.lohne@cognite.com>", "Emel Varol <emel.varol@cognite.com>", "Einar Marstrander Omang <einar.omang@cognite.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cognitedata/transformations-cli"
 
 packages = [
@@ -26,15 +26,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.0.2"
 types-retry = "^0.1.5"
 tabulate = "^0.8.9"
 types-tabulate = "^0.8.3"
 sqlparse = "^0.4.2"
-cognite-sdk = "6.1.5"
+cognite-sdk = "6.1.7"
 regex = "^2021.11.10"
 dacite = "^1.6.0"
 python-dotenv = "^0.21.0"
 pyparsing = "^3.0.9"
 PyYAML = "^6.0"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `cognite_transformations_cli-2.3.5/PKG-INFO` & `cognite_transformations_cli-2.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cognite-transformations-cli
-Version: 2.3.5
+Version: 2.3.6
 Summary: A CLI for the Transformations service in CDF
 Home-page: https://github.com/cognitedata/transformations-cli
 License: Apache-2.0
 Author: Mathias Lohne
 Author-email: mathias.lohne@cognite.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: click (>=8.0.2,<9.0.0)
-Requires-Dist: cognite-sdk (==6.1.5)
+Requires-Dist: cognite-sdk (==6.1.7)
 Requires-Dist: dacite (>=1.6.0,<2.0.0)
 Requires-Dist: pyparsing (>=3.0.9,<4.0.0)
 Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
 Requires-Dist: regex (>=2021.11.10,<2022.0.0)
 Requires-Dist: sqlparse (>=0.4.2,<0.5.0)
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
 Requires-Dist: types-retry (>=0.1.5,<0.2.0)
```


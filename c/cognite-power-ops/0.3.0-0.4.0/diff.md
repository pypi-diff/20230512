# Comparing `tmp/cognite_power_ops-0.3.0.tar.gz` & `tmp/cognite_power_ops-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_power_ops-0.3.0.tar", max compression
+gzip compressed data, was "cognite_power_ops-0.4.0.tar", max compression
```

## Comparing `cognite_power_ops-0.3.0.tar` & `cognite_power_ops-0.4.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rw-r--r--   0        0        0    10758 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/LICENSE
--rw-r--r--   0        0        0       76 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/__init__.py
--rw-r--r--   0        0        0    10260 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/bootstrap.py
--rw-r--r--   0        0        0        0 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/client/__init__.py
--rw-r--r--   0        0        0     6203 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/client/asset_apis.py
--rw-r--r--   0        0        0      601 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/client/config_client.py
--rw-r--r--   0        0        0        0 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/client/dm/__init__.py
--rw-r--r--   0        0        0     1891 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/client/dm/client.py
--rw-r--r--   0        0        0      895 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/client/dm/schema.graphql
--rw-r--r--   0        0        0     2005 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/client/dm/schema.py
--rw-r--r--   0        0        0      486 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/client/mapping_client.py
--rw-r--r--   0        0        0     2532 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/client/powerops_client.py
--rw-r--r--   0        0        0      331 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/client/transformation_client.py
--rw-r--r--   0        0        0    26552 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/config.py
--rw-r--r--   0        0        0        0 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/data_classes/__init__.py
--rw-r--r--   0        0        0     1221 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/data_classes/asset_lists.py
--rw-r--r--   0        0        0     3057 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/data_classes/benchmarking_config.py
--rw-r--r--   0        0        0     2984 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/data_classes/bid_matrix_generator_config.py
--rw-r--r--   0        0        0    13238 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/cdf_resource_collection.py
--rw-r--r--   0        0        0     2513 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/common.py
--rw-r--r--   0        0        0      129 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/config_model.py
--rw-r--r--   0        0        0     3630 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/core.py
--rw-r--r--   0        0        0      128 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/generators.py
--rw-r--r--   0        0        0     1482 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/market_config.py
--rw-r--r--   0        0        0    16796 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/plant.py
--rw-r--r--   0        0        0       99 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/price_area.py
--rw-r--r--   0        0        0     5114 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/reserve_scenario.py
--rw-r--r--   0        0        0      180 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/reservoirs.py
--rw-r--r--   0        0        0     1609 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/rkom_bid_combination_config.py
--rw-r--r--   0        0        0      994 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/rkom_market_config.py
--rw-r--r--   0        0        0      163 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/shared.py
--rw-r--r--   0        0        0     2113 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/shop_file_config.py
--rw-r--r--   0        0        0     2815 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/shop_output_definition.py
--rw-r--r--   0        0        0     9189 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/time_series_mapping.py
--rw-r--r--   0        0        0     1144 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/transformation.py
--rw-r--r--   0        0        0     1042 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/logger.py
--rw-r--r--   0        0        0     2070 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/main.py
--rw-r--r--   0        0        0        0 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/__init__.py
--rw-r--r--   0        0        0     1936 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/asset_types.py
--rw-r--r--   0        0        0     1424 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/cdf_auth.py
--rw-r--r--   0        0        0     2724 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/cdf_utils.py
--rw-r--r--   0        0        0      744 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/common.py
--rw-r--r--   0        0        0      324 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/constants.py
--rw-r--r--   0        0        0     3271 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/files.py
--rw-r--r--   0        0        0     4979 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/labels.py
--rw-r--r--   0        0        0     1766 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/mapping/mapping.py
--rw-r--r--   0        0        0     2609 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/mapping/static_mapping.py
--rw-r--r--   0        0        0     3165 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/powerops_asset_hierarchy.py
--rw-r--r--   0        0        0      718 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/powerops_status_events.py
--rw-r--r--   0        0        0     4495 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/relationship_types.py
--rw-r--r--   0        0        0    11602 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/resource_generation.py
--rw-r--r--   0        0        0     1495 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/serializer.py
--rw-r--r--   0        0        0       22 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/version.py
--rw-r--r--   0        0        0     1330 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 cognite_power_ops-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    10758 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/LICENSE
+-rw-r--r--   0        0        0      250 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/README.md
+-rw-r--r--   0        0        0       76 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/__init__.py
+-rw-r--r--   0        0        0    10260 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/bootstrap.py
+-rw-r--r--   0        0        0       65 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/client/__init__.py
+-rw-r--r--   0        0        0     6203 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/client/asset_apis.py
+-rw-r--r--   0        0        0      601 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/client/config_client.py
+-rw-r--r--   0        0        0        0 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/client/dm/__init__.py
+-rw-r--r--   0        0        0     1891 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/client/dm/client.py
+-rw-r--r--   0        0        0      895 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/client/dm/schema.graphql
+-rw-r--r--   0        0        0     2037 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/client/dm/schema.py
+-rw-r--r--   0        0        0     1875 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/client/dm_apis.py
+-rw-r--r--   0        0        0     2275 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/client/powerops_client.py
+-rw-r--r--   0        0        0     3074 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/client/shop_api.py
+-rw-r--r--   0        0        0    26552 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/config.py
+-rw-r--r--   0        0        0        0 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/data_classes/__init__.py
+-rw-r--r--   0        0        0     1221 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/data_classes/asset_lists.py
+-rw-r--r--   0        0        0     3057 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/data_classes/benchmarking_config.py
+-rw-r--r--   0        0        0     2984 2023-05-12 14:27:38.753896 cognite_power_ops-0.4.0/cognite/powerops/data_classes/bid_matrix_generator_config.py
+-rw-r--r--   0        0        0    13238 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/cdf_resource_collection.py
+-rw-r--r--   0        0        0     2513 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/common.py
+-rw-r--r--   0        0        0      129 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/config_model.py
+-rw-r--r--   0        0        0     3630 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/core.py
+-rw-r--r--   0        0        0      128 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/generators.py
+-rw-r--r--   0        0        0     1482 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/market_config.py
+-rw-r--r--   0        0        0    16796 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/plant.py
+-rw-r--r--   0        0        0       99 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/price_area.py
+-rw-r--r--   0        0        0     5114 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/reserve_scenario.py
+-rw-r--r--   0        0        0      180 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/reservoirs.py
+-rw-r--r--   0        0        0     1609 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/rkom_bid_combination_config.py
+-rw-r--r--   0        0        0      994 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/rkom_market_config.py
+-rw-r--r--   0        0        0      163 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/shared.py
+-rw-r--r--   0        0        0     2113 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/shop_file_config.py
+-rw-r--r--   0        0        0     2815 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/shop_output_definition.py
+-rw-r--r--   0        0        0     9189 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/time_series_mapping.py
+-rw-r--r--   0        0        0     1144 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/data_classes/transformation.py
+-rw-r--r--   0        0        0     1042 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/logger.py
+-rw-r--r--   0        0        0     2070 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/main.py
+-rw-r--r--   0        0        0        0 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/__init__.py
+-rw-r--r--   0        0        0     1936 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/asset_types.py
+-rw-r--r--   0        0        0     1424 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/cdf_auth.py
+-rw-r--r--   0        0        0     2724 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/cdf_utils.py
+-rw-r--r--   0        0        0      744 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/common.py
+-rw-r--r--   0        0        0      324 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/constants.py
+-rw-r--r--   0        0        0     3271 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/files.py
+-rw-r--r--   0        0        0     4979 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/labels.py
+-rw-r--r--   0        0        0     1766 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/mapping/mapping.py
+-rw-r--r--   0        0        0     2609 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/mapping/static_mapping.py
+-rw-r--r--   0        0        0     3165 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/powerops_asset_hierarchy.py
+-rw-r--r--   0        0        0      718 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/powerops_status_events.py
+-rw-r--r--   0        0        0     4495 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/relationship_types.py
+-rw-r--r--   0        0        0    11602 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/resource_generation.py
+-rw-r--r--   0        0        0     1495 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/utils/serializer.py
+-rw-r--r--   0        0        0       22 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/cognite/powerops/version.py
+-rw-r--r--   0        0        0     1423 2023-05-12 14:27:38.757897 cognite_power_ops-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 cognite_power_ops-0.4.0/PKG-INFO
```

### Comparing `cognite_power_ops-0.3.0/LICENSE` & `cognite_power_ops-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/bootstrap.py` & `cognite_power_ops-0.4.0/cognite/powerops/bootstrap.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/client/asset_apis.py` & `cognite_power_ops-0.4.0/cognite/powerops/client/asset_apis.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             "bid_process_configurations",
             "POWEROPS_bid_process_configuration_",
             BidProcessConfig,
             BidProcessList,
         )
 
 
-class ROOMBidConfigurationsAPI(AssetAPI):
+class RKOMBidConfigurationsAPI(AssetAPI):
     def __init__(self, client: CogniteClient, read_dataset: str, write_dataset: str):
         super().__init__(
             client,
             read_dataset,
             write_dataset,
             "rkom_bid_process_configurations",
             "POWEROPS_",
```

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/client/config_client.py` & `cognite_power_ops-0.4.0/cognite/powerops/client/config_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/client/dm/client.py` & `cognite_power_ops-0.4.0/cognite/powerops/client/dm/client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/client/dm/schema.graphql` & `cognite_power_ops-0.4.0/cognite/powerops/client/dm/schema.graphql`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/client/dm/schema.py` & `cognite_power_ops-0.4.0/cognite/powerops/client/dm/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 @power_ops_dm_schema.register_type
 class ProcessingLog(DomainModel):
     state: Optional[str] = None
     timestamp: Optional[str] = None
     error_msg: Optional[str] = None
 
 
-@power_ops_dm_schema.register_type
+@power_ops_dm_schema.register_type(lowercase_type_name="commands")
 class CommandsConfig(DomainModel):
     commands: List[str]
 
 
 @power_ops_dm_schema.register_type
 class FileRef(DomainModel):
     type: str
```

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/client/powerops_client.py` & `cognite_power_ops-0.4.0/cognite/powerops/client/powerops_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,56 +7,46 @@
     BidConfigurationsAPI,
     GeneratorsAPI,
     MarketConfigurationsAPI,
     PlantAPI,
     PriceAreasAPI,
     ReservoirsAPI,
     RKOMBidCombinationConfiguration,
-    ROOMBidConfigurationsAPI,
+    RKOMBidConfigurationsAPI,
     WatercourseAPI,
 )
 from cognite.powerops.client.config_client import ConfigurationClient
-from cognite.powerops.client.mapping_client import MappingClient
-from cognite.powerops.client.transformation_client import TransformationClient
-from cognite.powerops.config import BootstrapConfig
-
-
-class SHOPAPI:
-    def __init__(self):
-        ...
-
-    def run(
-        self, external_id: str, configuration: BootstrapConfig, shop_version: str
-    ) -> dict:  # TODO is BootstrapConfig correct?
-        """Create a ShopRun event and a DM Case"""
+from cognite.powerops.client.dm.client import get_power_ops_dm_client
+from cognite.powerops.client.dm_apis import CaseAPI, CommandsAPI, MappingAPI, ScenarioAPI, TransformationAPI
+from cognite.powerops.client.shop_api import ShopAPI
 
 
 class ConfigurationsClient:
     def __init__(self, read_dataset: str, write_dataset: str, client: CogniteClient):
         self.bids = BidConfigurationsAPI(client, read_dataset, write_dataset)
-        self.rkom_bids = ROOMBidConfigurationsAPI(client, read_dataset, write_dataset)
+        self.rkom_bids = RKOMBidConfigurationsAPI(client, read_dataset, write_dataset)
         self.bechmarkings = BenchmarkingConfigurationsAPI(client, read_dataset, write_dataset)
         self.markets = MarketConfigurationsAPI(client, read_dataset, write_dataset)
         self.rkom_bid_combinations = RKOMBidCombinationConfiguration(client, read_dataset, write_dataset)
 
 
 class PowerOpsClient:
     def __init__(self, read_dataset: str, write_dataset: str, config: Optional[ClientConfig] = None):
-        self.core = CogniteClient(config)
+        self.dm = get_power_ops_dm_client()
+        self.core = self.dm._client
+
         self.configurations = ConfigurationClient()
 
+        self.shop = ShopAPI(po_client=self)
+
         self.configurations = ConfigurationsClient(read_dataset, write_dataset, self.core)
         self.generators = GeneratorsAPI(self.core, read_dataset, write_dataset)
         self.plants = PlantAPI(self.core, read_dataset, write_dataset)
         self.price_areas = PriceAreasAPI(self.core, read_dataset, write_dataset)
         self.reservoirs = ReservoirsAPI(self.core, read_dataset, write_dataset)
         self.watercourses = WatercourseAPI(self.core, read_dataset, write_dataset)
 
-        self.shop = SHOPAPI()
-
-        self.mappings = MappingClient()
-        self.transformations = TransformationClient()
-        ...
-
-        # low-level clients:
-        # self._dm = get_power_ops_dm_client()  # manage DM items (instances) directly
-        # self._cdf = self._dm._client  # CogniteClient plus DM v3 client (Nodes, Edges, Spaces, etc.)
+        self.cases = CaseAPI(self.dm)
+        self.commands = CommandsAPI(self.dm)
+        self.scenarios = ScenarioAPI(self.dm)
+        self.mappings = MappingAPI(self.dm)
+        self.transformations = TransformationAPI(self.dm)
```

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/config.py` & `cognite_power_ops-0.4.0/cognite/powerops/config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/data_classes/asset_lists.py` & `cognite_power_ops-0.4.0/cognite/powerops/data_classes/asset_lists.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/data_classes/benchmarking_config.py` & `cognite_power_ops-0.4.0/cognite/powerops/data_classes/benchmarking_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/data_classes/bid_matrix_generator_config.py` & `cognite_power_ops-0.4.0/cognite/powerops/data_classes/bid_matrix_generator_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/data_classes/cdf_resource_collection.py` & `cognite_power_ops-0.4.0/cognite/powerops/data_classes/cdf_resource_collection.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/data_classes/common.py` & `cognite_power_ops-0.4.0/cognite/powerops/data_classes/common.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/data_classes/core.py` & `cognite_power_ops-0.4.0/cognite/powerops/data_classes/core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/data_classes/market_config.py` & `cognite_power_ops-0.4.0/cognite/powerops/data_classes/market_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/data_classes/plant.py` & `cognite_power_ops-0.4.0/cognite/powerops/data_classes/plant.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/data_classes/reserve_scenario.py` & `cognite_power_ops-0.4.0/cognite/powerops/data_classes/reserve_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/data_classes/rkom_bid_combination_config.py` & `cognite_power_ops-0.4.0/cognite/powerops/data_classes/rkom_bid_combination_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/data_classes/rkom_market_config.py` & `cognite_power_ops-0.4.0/cognite/powerops/data_classes/rkom_market_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/data_classes/shop_file_config.py` & `cognite_power_ops-0.4.0/cognite/powerops/data_classes/shop_file_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/data_classes/shop_output_definition.py` & `cognite_power_ops-0.4.0/cognite/powerops/data_classes/shop_output_definition.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/data_classes/time_series_mapping.py` & `cognite_power_ops-0.4.0/cognite/powerops/data_classes/time_series_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/data_classes/transformation.py` & `cognite_power_ops-0.4.0/cognite/powerops/data_classes/transformation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/logger.py` & `cognite_power_ops-0.4.0/cognite/powerops/logger.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/main.py` & `cognite_power_ops-0.4.0/cognite/powerops/main.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/utils/asset_types.py` & `cognite_power_ops-0.4.0/cognite/powerops/utils/asset_types.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/utils/cdf_auth.py` & `cognite_power_ops-0.4.0/cognite/powerops/utils/cdf_auth.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/utils/cdf_utils.py` & `cognite_power_ops-0.4.0/cognite/powerops/utils/cdf_utils.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/utils/common.py` & `cognite_power_ops-0.4.0/cognite/powerops/utils/common.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/utils/files.py` & `cognite_power_ops-0.4.0/cognite/powerops/utils/files.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/utils/labels.py` & `cognite_power_ops-0.4.0/cognite/powerops/utils/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/utils/mapping/mapping.py` & `cognite_power_ops-0.4.0/cognite/powerops/utils/mapping/mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/utils/mapping/static_mapping.py` & `cognite_power_ops-0.4.0/cognite/powerops/utils/mapping/static_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/utils/powerops_asset_hierarchy.py` & `cognite_power_ops-0.4.0/cognite/powerops/utils/powerops_asset_hierarchy.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/utils/powerops_status_events.py` & `cognite_power_ops-0.4.0/cognite/powerops/utils/powerops_status_events.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/utils/relationship_types.py` & `cognite_power_ops-0.4.0/cognite/powerops/utils/relationship_types.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/utils/resource_generation.py` & `cognite_power_ops-0.4.0/cognite/powerops/utils/resource_generation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.3.0/cognite/powerops/utils/serializer.py` & `cognite_power_ops-0.4.0/cognite/powerops/utils/serializer.py`

 * *Files identical despite different names*


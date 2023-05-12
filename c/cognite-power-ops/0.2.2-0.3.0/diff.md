# Comparing `tmp/cognite_power_ops-0.2.2.tar.gz` & `tmp/cognite_power_ops-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_power_ops-0.2.2.tar", max compression
+gzip compressed data, was "cognite_power_ops-0.3.0.tar", max compression
```

## Comparing `cognite_power_ops-0.2.2.tar` & `cognite_power_ops-0.3.0.tar`

### file list

```diff
@@ -1,48 +1,55 @@
--rw-r--r--   0        0        0    10758 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/LICENSE
--rw-r--r--   0        0        0       76 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/__init__.py
--rw-r--r--   0        0        0    10260 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/bootstrap.py
--rw-r--r--   0        0        0        0 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/client/__init__.py
--rw-r--r--   0        0        0      601 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/client/config_client.py
--rw-r--r--   0        0        0        0 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/client/dm/__init__.py
--rw-r--r--   0        0        0     1891 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/client/dm/client.py
--rw-r--r--   0        0        0      895 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/client/dm/schema.graphql
--rw-r--r--   0        0        0     2005 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/client/dm/schema.py
--rw-r--r--   0        0        0      486 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/client/mapping_client.py
--rw-r--r--   0        0        0     1173 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/client/powerops_client.py
--rw-r--r--   0        0        0      331 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/client/transformation_client.py
--rw-r--r--   0        0        0      803 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/client/watercourse_client.py
--rw-r--r--   0        0        0    24691 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/config.py
--rw-r--r--   0        0        0        0 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/__init__.py
--rw-r--r--   0        0        0     2686 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/benchmarking_config.py
--rw-r--r--   0        0        0     2984 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/bid_matrix_generator_config.py
--rw-r--r--   0        0        0    13238 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/cdf_resource_collection.py
--rw-r--r--   0        0        0     2513 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/common.py
--rw-r--r--   0        0        0     1390 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/market_config.py
--rw-r--r--   0        0        0    16603 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/plant.py
--rw-r--r--   0        0        0     5114 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/reserve_scenario.py
--rw-r--r--   0        0        0     1224 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/rkom_bid_combination_config.py
--rw-r--r--   0        0        0      994 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/rkom_market_config.py
--rw-r--r--   0        0        0     2113 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/shop_file_config.py
--rw-r--r--   0        0        0     2815 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/shop_output_definition.py
--rw-r--r--   0        0        0     9189 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/time_series_mapping.py
--rw-r--r--   0        0        0     1144 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/data_classes/transformation.py
--rw-r--r--   0        0        0     1042 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/logger.py
--rw-r--r--   0        0        0     2070 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/main.py
--rw-r--r--   0        0        0        0 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/__init__.py
--rw-r--r--   0        0        0     1936 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/asset_types.py
--rw-r--r--   0        0        0     1424 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/cdf_auth.py
--rw-r--r--   0        0        0     2724 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/cdf_utils.py
--rw-r--r--   0        0        0      744 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/common.py
--rw-r--r--   0        0        0      324 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/constants.py
--rw-r--r--   0        0        0     3271 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/files.py
--rw-r--r--   0        0        0     4979 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/labels.py
--rw-r--r--   0        0        0     1766 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/mapping/mapping.py
--rw-r--r--   0        0        0     2609 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/mapping/static_mapping.py
--rw-r--r--   0        0        0     3165 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/powerops_asset_hierarchy.py
--rw-r--r--   0        0        0      718 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/powerops_status_events.py
--rw-r--r--   0        0        0     4495 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/relationship_types.py
--rw-r--r--   0        0        0    11602 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/resource_generation.py
--rw-r--r--   0        0        0     1495 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/utils/serializer.py
--rw-r--r--   0        0        0       22 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/cognite/powerops/version.py
--rw-r--r--   0        0        0     1330 2023-05-11 14:59:41.488843 cognite_power_ops-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 cognite_power_ops-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    10758 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/LICENSE
+-rw-r--r--   0        0        0       76 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/__init__.py
+-rw-r--r--   0        0        0    10260 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/bootstrap.py
+-rw-r--r--   0        0        0        0 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/client/__init__.py
+-rw-r--r--   0        0        0     6203 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/client/asset_apis.py
+-rw-r--r--   0        0        0      601 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/client/config_client.py
+-rw-r--r--   0        0        0        0 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/client/dm/__init__.py
+-rw-r--r--   0        0        0     1891 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/client/dm/client.py
+-rw-r--r--   0        0        0      895 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/client/dm/schema.graphql
+-rw-r--r--   0        0        0     2005 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/client/dm/schema.py
+-rw-r--r--   0        0        0      486 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/client/mapping_client.py
+-rw-r--r--   0        0        0     2532 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/client/powerops_client.py
+-rw-r--r--   0        0        0      331 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/client/transformation_client.py
+-rw-r--r--   0        0        0    26552 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/config.py
+-rw-r--r--   0        0        0        0 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/data_classes/__init__.py
+-rw-r--r--   0        0        0     1221 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/data_classes/asset_lists.py
+-rw-r--r--   0        0        0     3057 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/data_classes/benchmarking_config.py
+-rw-r--r--   0        0        0     2984 2023-05-12 11:21:56.095021 cognite_power_ops-0.3.0/cognite/powerops/data_classes/bid_matrix_generator_config.py
+-rw-r--r--   0        0        0    13238 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/cdf_resource_collection.py
+-rw-r--r--   0        0        0     2513 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/common.py
+-rw-r--r--   0        0        0      129 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/config_model.py
+-rw-r--r--   0        0        0     3630 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/core.py
+-rw-r--r--   0        0        0      128 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/generators.py
+-rw-r--r--   0        0        0     1482 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/market_config.py
+-rw-r--r--   0        0        0    16796 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/plant.py
+-rw-r--r--   0        0        0       99 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/price_area.py
+-rw-r--r--   0        0        0     5114 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/reserve_scenario.py
+-rw-r--r--   0        0        0      180 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/reservoirs.py
+-rw-r--r--   0        0        0     1609 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/rkom_bid_combination_config.py
+-rw-r--r--   0        0        0      994 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/rkom_market_config.py
+-rw-r--r--   0        0        0      163 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/shared.py
+-rw-r--r--   0        0        0     2113 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/shop_file_config.py
+-rw-r--r--   0        0        0     2815 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/shop_output_definition.py
+-rw-r--r--   0        0        0     9189 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/time_series_mapping.py
+-rw-r--r--   0        0        0     1144 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/data_classes/transformation.py
+-rw-r--r--   0        0        0     1042 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/logger.py
+-rw-r--r--   0        0        0     2070 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/main.py
+-rw-r--r--   0        0        0        0 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/__init__.py
+-rw-r--r--   0        0        0     1936 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/asset_types.py
+-rw-r--r--   0        0        0     1424 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/cdf_auth.py
+-rw-r--r--   0        0        0     2724 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/cdf_utils.py
+-rw-r--r--   0        0        0      744 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/common.py
+-rw-r--r--   0        0        0      324 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/constants.py
+-rw-r--r--   0        0        0     3271 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/files.py
+-rw-r--r--   0        0        0     4979 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/labels.py
+-rw-r--r--   0        0        0     1766 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/mapping/mapping.py
+-rw-r--r--   0        0        0     2609 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/mapping/static_mapping.py
+-rw-r--r--   0        0        0     3165 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/powerops_asset_hierarchy.py
+-rw-r--r--   0        0        0      718 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/powerops_status_events.py
+-rw-r--r--   0        0        0     4495 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/relationship_types.py
+-rw-r--r--   0        0        0    11602 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/resource_generation.py
+-rw-r--r--   0        0        0     1495 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/utils/serializer.py
+-rw-r--r--   0        0        0       22 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/cognite/powerops/version.py
+-rw-r--r--   0        0        0     1330 2023-05-12 11:21:56.099026 cognite_power_ops-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 cognite_power_ops-0.3.0/PKG-INFO
```

### Comparing `cognite_power_ops-0.2.2/LICENSE` & `cognite_power_ops-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/bootstrap.py` & `cognite_power_ops-0.3.0/cognite/powerops/bootstrap.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/client/config_client.py` & `cognite_power_ops-0.3.0/cognite/powerops/client/config_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/client/dm/client.py` & `cognite_power_ops-0.3.0/cognite/powerops/client/dm/client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/client/dm/schema.graphql` & `cognite_power_ops-0.3.0/cognite/powerops/client/dm/schema.graphql`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/client/dm/schema.py` & `cognite_power_ops-0.3.0/cognite/powerops/client/dm/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/config.py` & `cognite_power_ops-0.3.0/cognite/powerops/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from __future__ import annotations
 
+import ast
 import json
 import typing
 from collections import defaultdict
 from pathlib import Path
 from typing import ClassVar, Dict, Generator, List, Optional, Tuple, Union
 
 from cognite.client.data_classes import Asset, Label, Sequence
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, Field, root_validator, validator
 
 from cognite.powerops.data_classes.benchmarking_config import BenchmarkingConfig
 from cognite.powerops.data_classes.cdf_resource_collection import (
     BootstrapResourceCollection,
     SequenceContent,
     SequenceRows,
 )
 from cognite.powerops.data_classes.common import AggregationMethod, CommonConstants, RelativeTime, RetrievalType
+from cognite.powerops.data_classes.config_model import Configuration
 from cognite.powerops.data_classes.market_config import MarketConfig
 from cognite.powerops.data_classes.reserve_scenario import Auction, Block, Product, ReserveScenario
 from cognite.powerops.data_classes.rkom_bid_combination_config import RKOMBidCombinationConfig
 from cognite.powerops.data_classes.rkom_market_config import RkomMarketConfig
 from cognite.powerops.data_classes.time_series_mapping import (
     TimeSeriesMapping,
     TimeSeriesMappingEntry,
@@ -28,16 +30,20 @@
 from cognite.powerops.data_classes.transformation import Transformation, TransformationType
 from cognite.powerops.utils.cdf_utils import simple_relationship
 from cognite.powerops.utils.common import print_warning
 from cognite.powerops.utils.labels import AssetLabels, RelationshipLabels
 from cognite.powerops.utils.serializer import load_yaml
 
 
-class WatercourseConfig(BaseModel):
+class Watercourse(BaseModel):
     name: str
+    shop_penalty_limit: int = 42000
+
+
+class WatercourseConfig(Watercourse):
     version: str
     market_to_price_area: Dict[str, str]
     directory: str
     model_raw: str
     # ------------------------------------------------------------------
     yaml_raw_path: str = ""
     yaml_processed_path: str = ""  # TODO: not used here
@@ -48,15 +54,14 @@
     rrs_ids: Optional[List[str]] = None
     hardcoded_mapping: Optional[TimeSeriesMapping] = None  # TODO: not used here
     hist_flow_timeseries: Optional[Dict[str, str]] = None  # TODO: not used here
     # ------------------------------------------------------------------
     production_obligation_ts_ext_ids: Optional[List[str]] = None
     plant_display_names_and_order: Optional[Dict[str, tuple[str, int]]] = None
     reservoir_display_names_and_order: Optional[Dict[str, tuple[str, int]]] = None
-    shop_penalty_limit: int = 42000
     water_value_based_method_time_series_csv_filename: Optional[str] = None
 
     @classmethod
     def from_yaml(cls, yaml_path: Path) -> list["WatercourseConfig"]:
         return [cls(**watercourse_raw) for watercourse_raw in load_yaml(yaml_path)]
 
     def load_plants_by_price_area(self, path: Path) -> dict[str, list]:
@@ -206,25 +211,33 @@
             label_external_id=RelationshipLabels.BID_MATRIX_GENERATOR_CONFIG_SEQUENCE,
         )
         bootstrap_resource_collection.add(relationship)
 
         return bootstrap_resource_collection
 
 
-class BidProcessConfig(BaseModel):
+class BidProcessConfig(Configuration):
     name: str
-    price_area_name: str
-    price_scenarios: List[PriceScenarioID]
-    main_scenario: str
+    price_area_name: str = Field(alias="bid_price_area")
+    price_scenarios: List[PriceScenarioID] = Field(alias="bid_price_scenarios")
+    main_scenario: str = Field(alias="bid_main_scenario")
     bid_date: Optional[RelativeTime] = None
-    shop_start: Optional[RelativeTime] = None
-    shop_end: Optional[RelativeTime] = None
-    bid_matrix_generator: str
+    shop_start: Optional[RelativeTime] = Field(None, alias="shop_starttime")
+    shop_end: Optional[RelativeTime] = Field(None, alias="shop_endtime")
+    bid_matrix_generator: str = Field(alias="bid_bid_matrix_generator_config_external_id")
     price_scenarios_per_watercourse: Optional[Dict[str, typing.Set[str]]] = None
 
+    @validator("shop_start", "shop_end", "bid_date", pre=True)
+    def json_loads(cls, value):
+        return {"operations": json.loads(value)} if isinstance(value, str) else value
+
+    @validator("price_scenarios", pre=True)
+    def literal_eval(cls, value):
+        return [{"id": id_} for id_ in ast.literal_eval(value)] if isinstance(value, str) else value
+
     def to_cdf_asset(
         self,
         benchmark: BenchmarkingConfig,
         price_scenarios_by_id: dict[str, PriceScenario],
     ) -> Asset:
         def to_metadata(price_scenarios_by_id: dict[str, PriceScenario], benchmark: BenchmarkingConfig) -> dict:
             price_scenarios = map_price_scenarios_by_name(
@@ -439,32 +452,56 @@
                 mip_plant_time_series=self.mip_plant_time_series,
                 obligation_external_id=self.obligation_external_id,
             )
             for volume in self.volumes
         ]
 
 
-class RKOMBidProcessConfig(BaseModel):
-    watercourse: str
+class RKOMBidProcessConfig(Configuration):
+    watercourse: str = Field(alias="bid_watercourse")
 
-    price_scenarios: List[PriceScenarioID]
-    reserve_scenarios: ReserveScenarios
+    price_scenarios: List[PriceScenarioID] = Field(alias="bid_price_scenarios")
+    reserve_scenarios: ReserveScenarios = Field(alias="bid_reserve_scenarios")
 
-    shop_start: RelativeTime
-    shop_end: RelativeTime
+    shop_start: RelativeTime = Field(alias="shop_starttime")
+    shop_end: RelativeTime = Field(alias="shop_endtime")
 
     timezone: str = "Europe/Oslo"
     method: str = "simple"
 
     minimum_price: int = 0  # TODO: need to specify currency
     price_premium: int = 0  # TODO: need to specify currency
 
     parent_external_id: typing.ClassVar[str] = "rkom_bid_process_configurations"
     mapping_type: ClassVar[str] = "rkom_incremental_mapping"
 
+    @root_validator(pre=True)
+    def create_reserve_scenarios(cls, values):
+        if not isinstance(volumes := values.get("bid_reserve_scenarios"), str):
+            return values
+        volumes = [int(volume.removesuffix("MW")) for volume in volumes[1:-1].split(",")]
+
+        values["bid_reserve_scenarios"] = dict(
+            volumes=volumes,
+            auction=values["bid_auction"],
+            product=values["bid_product"],
+            block=values["bid_block"],
+            reserve_group=values["labels"][0]["externalId"],
+            mip_plant_time_series=[],
+        )
+        return values
+
+    @validator("shop_start", "shop_end", pre=True)
+    def json_loads(cls, value):
+        return {"operations": json.loads(value)} if isinstance(value, str) else value
+
+    @validator("price_scenarios", pre=True)
+    def literal_eval(cls, value):
+        return [{"id": id_} for id_ in ast.literal_eval(value)] if isinstance(value, str) else value
+
     @property
     def sorted_volumes(self) -> List[int]:
         return sorted(self.reserve_scenarios.volumes)
 
     @property
     def name(self) -> str:
         return (
```

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/data_classes/benchmarking_config.py` & `cognite_power_ops-0.3.0/cognite/powerops/data_classes/benchmarking_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import json
 from typing import Dict, List, Optional
 
 from cognite.client.data_classes import Asset
-from pydantic import BaseModel
+from pydantic import Field, validator
 
 from cognite.powerops.data_classes.common import RelativeTime
+from cognite.powerops.data_classes.config_model import Configuration
 
 
-class BenchmarkingConfig(BaseModel):
+class BenchmarkingConfig(Configuration):
     bid_date: RelativeTime
-    shop_start: RelativeTime
-    shop_end: RelativeTime
+    shop_start: RelativeTime = Field(alias="shop_starttime")
+    shop_end: RelativeTime = Field(alias="shop_endtime")
     production_plan_time_series: Optional[Dict[str, List[str]]]
-    market_config_external_id: str
+    market_config_external_id: str = Field(alias="bid_market_config_external_id")
     relevant_shop_objective_metrics: Dict[str, str] = {
         "grand_total": "Grand Total",
         "total": "Total",
         "sum_penalties": "Sum Penalties",
         "major_penalties": "Major Penalties",
         "minor_penalties": "Minor Penalties",
         "load_value": "Load Value",
@@ -32,14 +33,18 @@
         "reserve_violation_penalty": "Reserve Violation Penalty",
         "load_penalty": "Load Penalty",
     }  # Pydantic handles mutable defaults such that this is OK:
     # https://stackoverflow.com/questions/63793662/how-to-give-a-pydantic-list-field-a-default-value/63808835#63808835
     # TODO: Consider adding relationships to bid process config
     #  assets (or remove the optional part that uses those relationships in power-ops-functions)
 
+    @validator("shop_start", "shop_end", "bid_date", pre=True)
+    def json_loads(cls, value):
+        return {"operations": json.loads(value)} if isinstance(value, str) else value
+
     @property
     def metadata(self) -> dict:
         metadata = {
             "bid:date": str(self.bid_date),
             "shop:starttime": str(self.shop_start),
             "shop:endtime": str(self.shop_end),
             "bid:market_config_external_id": self.market_config_external_id,
```

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/data_classes/bid_matrix_generator_config.py` & `cognite_power_ops-0.3.0/cognite/powerops/data_classes/bid_matrix_generator_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/data_classes/cdf_resource_collection.py` & `cognite_power_ops-0.3.0/cognite/powerops/data_classes/cdf_resource_collection.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/data_classes/common.py` & `cognite_power_ops-0.3.0/cognite/powerops/data_classes/common.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/data_classes/plant.py` & `cognite_power_ops-0.3.0/cognite/powerops/data_classes/plant.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import json
 from pathlib import Path
 from typing import List, NamedTuple, Optional, Tuple
 
 import pandas as pd
 from cognite.client.data_classes import Asset, Label, Relationship
-from pydantic import BaseModel
+from pydantic import BaseModel, validator
 
 from cognite.powerops.data_classes.cdf_resource_collection import BootstrapResourceCollection
 from cognite.powerops.data_classes.time_series_mapping import TimeSeriesMapping
 from cognite.powerops.utils.common import print_warning
 from cognite.powerops.utils.labels import AssetLabels as al
 from cognite.powerops.utils.labels import RelationshipLabels as rl
 from cognite.powerops.utils.relationship_types import asset_to_time_series, plant_to_generator, plant_to_inlet_reservoir
@@ -43,14 +43,20 @@
     outlet_level_time_series: Optional[ExternalId] = None  # external ID of time series with values in m.a.s.l.
     water_value_time_series: Optional[ExternalId] = None  # external ID of time series with values in €/MWh
     feeding_fee_time_series: Optional[ExternalId] = None  # external ID of time series with values in percent
     p_min_time_series: Optional[ExternalId] = None  # external ID of time series with values in MW
     p_max_time_series: Optional[ExternalId] = None  # external ID of time series with values in MW
     startcost_split_hours_time_series: Optional[ExternalId] = None  # external ID of time series with values in h
 
+    @validator("penstock_head_loss_factors", pre=True)
+    def parse_dict(cls, value):
+        if isinstance(value, str):
+            value = json.loads(value)
+        return value
+
     def asset(self) -> Asset:
         """Returns the Asset representation of this Plant (without relationships)"""
         return Asset(
             name=self.name,
             external_id=self.external_id,
             parent_external_id="plants",
             metadata={
```

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/data_classes/reserve_scenario.py` & `cognite_power_ops-0.3.0/cognite/powerops/data_classes/reserve_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/data_classes/rkom_bid_combination_config.py` & `cognite_power_ops-0.3.0/cognite/powerops/data_classes/rkom_bid_combination_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,32 @@
+import ast
 import json
 from typing import ClassVar, List
 
 from cognite.client.data_classes import Asset
-from pydantic import BaseModel, validator
+from pydantic import Field, validator
 
+from cognite.powerops.data_classes.config_model import Configuration
 from cognite.powerops.data_classes.reserve_scenario import Auction
 
 
-class RKOMBidCombinationConfig(BaseModel):
-    auction: Auction
-    name: str = "default"
-    rkom_bid_config_external_ids: List[str]
+class RKOMBidCombinationConfig(Configuration):
+    auction: Auction = Field(alias="bid_auction")
+    name: str = Field("default", alias="bid_combination_name")
+    rkom_bid_config_external_ids: List[str] = Field(alias="bid_rkom_bid_configs")
     parent_external_id: ClassVar[str] = "rkom_bid_combination_configurations"
 
     @validator("auction", pre=True)
     def to_enum(cls, value):
         return Auction[value] if isinstance(value, str) else value
 
+    @validator("rkom_bid_config_external_ids", pre=True)
+    def parse_string(cls, value):
+        return [external_id for external_id in ast.literal_eval(value)] if isinstance(value, str) else value
+
     @property
     def cdf_asset(self) -> Asset:
         sequence_external_id = f"RKOM_bid_combination_configuration_{self.auction.value}_{self.name}"
 
         return Asset(
             name=sequence_external_id.replace("_", " "),
             description="Defining which RKOM bid methods should be combined (into the total bid form)",
```

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/data_classes/rkom_market_config.py` & `cognite_power_ops-0.3.0/cognite/powerops/data_classes/rkom_market_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/data_classes/shop_file_config.py` & `cognite_power_ops-0.3.0/cognite/powerops/data_classes/shop_file_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/data_classes/shop_output_definition.py` & `cognite_power_ops-0.3.0/cognite/powerops/data_classes/shop_output_definition.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/data_classes/time_series_mapping.py` & `cognite_power_ops-0.3.0/cognite/powerops/data_classes/time_series_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/data_classes/transformation.py` & `cognite_power_ops-0.3.0/cognite/powerops/data_classes/transformation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/logger.py` & `cognite_power_ops-0.3.0/cognite/powerops/logger.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/main.py` & `cognite_power_ops-0.3.0/cognite/powerops/main.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/utils/asset_types.py` & `cognite_power_ops-0.3.0/cognite/powerops/utils/asset_types.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/utils/cdf_auth.py` & `cognite_power_ops-0.3.0/cognite/powerops/utils/cdf_auth.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/utils/cdf_utils.py` & `cognite_power_ops-0.3.0/cognite/powerops/utils/cdf_utils.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/utils/common.py` & `cognite_power_ops-0.3.0/cognite/powerops/utils/common.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/utils/files.py` & `cognite_power_ops-0.3.0/cognite/powerops/utils/files.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/utils/labels.py` & `cognite_power_ops-0.3.0/cognite/powerops/utils/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/utils/mapping/mapping.py` & `cognite_power_ops-0.3.0/cognite/powerops/utils/mapping/mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/utils/mapping/static_mapping.py` & `cognite_power_ops-0.3.0/cognite/powerops/utils/mapping/static_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/utils/powerops_asset_hierarchy.py` & `cognite_power_ops-0.3.0/cognite/powerops/utils/powerops_asset_hierarchy.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/utils/powerops_status_events.py` & `cognite_power_ops-0.3.0/cognite/powerops/utils/powerops_status_events.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/utils/relationship_types.py` & `cognite_power_ops-0.3.0/cognite/powerops/utils/relationship_types.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/utils/resource_generation.py` & `cognite_power_ops-0.3.0/cognite/powerops/utils/resource_generation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/cognite/powerops/utils/serializer.py` & `cognite_power_ops-0.3.0/cognite/powerops/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.2.2/pyproject.toml` & `cognite_power_ops-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-power-ops"
-version = "0.2.2"
+version = "0.3.0"
 description = "SDK for power markets operations on Cognite Data Fusion"
 authors = ["Cognite <support@cognite.com>"]
 license = "Apache 2.0"
 packages = [{include = "cognite", from = "."}]
 
 [tool.black]
 line-length = 120
```

### Comparing `cognite_power_ops-0.2.2/PKG-INFO` & `cognite_power_ops-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-power-ops
-Version: 0.2.2
+Version: 0.3.0
 Summary: SDK for power markets operations on Cognite Data Fusion
 License: Apache 2.0
 Author: Cognite
 Author-email: support@cognite.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/dialogy-2.0.5.tar.gz` & `tmp/dialogy-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialogy-2.0.5.tar", max compression
+gzip compressed data, was "dialogy-2.0.6.tar", max compression
```

## Comparing `dialogy-2.0.5.tar` & `dialogy-2.0.6.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1069 2023-05-08 05:01:39.708229 dialogy-2.0.5/LICENSE.md
--rw-r--r--   0        0        0        0 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/__init__.py
--rw-r--r--   0        0        0      183 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/base/__init__.py
--rw-r--r--   0        0        0     4949 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/base/entity_extractor/__init__.py
--rw-r--r--   0        0        0     9777 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/base/input/__init__.py
--rw-r--r--   0        0        0     4595 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/base/output/__init__.py
--rw-r--r--   0        0        0    15662 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/base/plugin/__init__.py
--rw-r--r--   0        0        0     3908 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/cli/__init__.py
--rw-r--r--   0        0        0     2587 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/cli/project.py
--rw-r--r--   0        0        0     1865 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/cli/workflow.py
--rw-r--r--   0        0        0     5017 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/constants/__init__.py
--rw-r--r--   0        0        0     2011 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/registry.py
--rw-r--r--   0        0        0        0 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/__init__.py
--rw-r--r--   0        0        0     3995 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/address_parser/__init__.py
--rw-r--r--   0        0        0     1406 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/address_parser/mapmyindia.py
--rw-r--r--   0        0        0     4978 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/address_parser/maps.py
--rw-r--r--   0        0        0        0 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/calibration/__init__.py
--rw-r--r--   0        0        0     8868 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/calibration/xgb.py
--rw-r--r--   0        0        0     3790 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/canonicalization/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/classification/__init__.py
--rw-r--r--   0        0        0    11805 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/classification/mlp.py
--rw-r--r--   0        0        0     1179 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/classification/retain_intent.py
--rw-r--r--   0        0        0       58 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/classification/tokenizers.py
--rw-r--r--   0        0        0    17246 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/classification/xlmr.py
--rw-r--r--   0        0        0     7676 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/combine_date_time/__init__.py
--rw-r--r--   0        0        0    39327 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/duckling_plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/error_recovery/__init__.py
--rw-r--r--   0        0        0    20334 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/error_recovery/error_recovery.py
--rw-r--r--   0        0        0    12300 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/intent_entity_mutator/__init__.py
--rw-r--r--   0        0        0      743 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py
--rw-r--r--   0        0        0      797 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/intent_entity_mutator/const.py
--rw-r--r--   0        0        0      313 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/intent_entity_mutator/registry.py
--rw-r--r--   0        0        0     1792 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/lb_plugin/__init__.py
--rw-r--r--   0        0        0    14123 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/list_entity_plugin/__init__.py
--rw-r--r--   0        0        0    11523 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/list_search_plugin/__init__.py
--rw-r--r--   0        0        0     4841 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/list_search_plugin/sample_config.yaml
--rw-r--r--   0        0        0     4699 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/merge_asr_output/__init__.py
--rw-r--r--   0        0        0     1565 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/oos_filter/__init__.py
--rw-r--r--   0        0        0     4247 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/qc_plugin/__init__.py
--rw-r--r--   0        0        0      833 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/slot_filler/__init__.py
--rw-r--r--   0        0        0     4148 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/plugins/text/slot_filler/rule_slot_filler.py
--rw-r--r--   0        0        0        0 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/plugins/text/voting/__init__.py
--rw-r--r--   0        0        0     1862 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/__init__.py
--rw-r--r--   0        0        0      170 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/__init__.py
--rw-r--r--   0        0        0      914 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/address/__init__.py
--rw-r--r--   0        0        0     1811 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/amount_of_money/__init__.py
--rw-r--r--   0        0        0     7338 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/base_entity/__init__.py
--rw-r--r--   0        0        0     2281 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/credit_card_number/__init__.py
--rw-r--r--   0        0        0     3637 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/deserialize/__init__.py
--rw-r--r--   0        0        0     4317 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/duration/__init__.py
--rw-r--r--   0        0        0      975 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/keyword/__init__.py
--rw-r--r--   0        0        0     4698 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/numerical/__init__.py
--rw-r--r--   0        0        0     2271 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/people/__init__.py
--rw-r--r--   0        0        0      910 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/pincode/__init__.py
--rw-r--r--   0        0        0    13534 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/time/__init__.py
--rw-r--r--   0        0        0     8803 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/time_interval/__init__.py
--rw-r--r--   0        0        0     8893 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/intent/__init__.py
--rw-r--r--   0        0        0      154 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/signal/__init__.py
--rw-r--r--   0        0        0      194 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/signal/signal.py
--rw-r--r--   0        0        0      991 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/slots/__init__.py
--rw-r--r--   0        0        0      191 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/utterances/__init__.py
--rw-r--r--   0        0        0      638 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/utils/__init__.py
--rw-r--r--   0        0        0    10469 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/utils/config.py
--rw-r--r--   0        0        0     2180 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/utils/datetime.py
--rw-r--r--   0        0        0     3437 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/utils/file_handler.py
--rw-r--r--   0        0        0      808 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/utils/logger.py
--rw-r--r--   0        0        0     2687 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/utils/misc.py
--rw-r--r--   0        0        0      584 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/utils/naive_lang_detect.py
--rw-r--r--   0        0        0     8236 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/utils/normalize_utterance.py
--rw-r--r--   0        0        0     3605 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/utils/temperature_scaling.py
--rw-r--r--   0        0        0       47 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/workflow/__init__.py
--rw-r--r--   0        0        0     6795 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/workflow/workflow.py
--rw-r--r--   0        0        0     1425 2023-05-08 05:01:56.172423 dialogy-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     1611 1970-01-01 00:00:00.000000 dialogy-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-10 14:37:20.344091 dialogy-2.0.6/LICENSE.md
+-rw-r--r--   0        0        0        0 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/__init__.py
+-rw-r--r--   0        0        0      183 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/base/__init__.py
+-rw-r--r--   0        0        0     4949 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/base/entity_extractor/__init__.py
+-rw-r--r--   0        0        0     9777 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/base/input/__init__.py
+-rw-r--r--   0        0        0     4595 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/base/output/__init__.py
+-rw-r--r--   0        0        0    15679 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/base/plugin/__init__.py
+-rw-r--r--   0        0        0     3908 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/cli/__init__.py
+-rw-r--r--   0        0        0     2587 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/cli/project.py
+-rw-r--r--   0        0        0     1865 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/cli/workflow.py
+-rw-r--r--   0        0        0     5017 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/constants/__init__.py
+-rw-r--r--   0        0        0     2011 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/registry.py
+-rw-r--r--   0        0        0        0 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/__init__.py
+-rw-r--r--   0        0        0     4001 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/address_parser/__init__.py
+-rw-r--r--   0        0        0     1406 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/address_parser/mapmyindia.py
+-rw-r--r--   0        0        0     4978 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/address_parser/maps.py
+-rw-r--r--   0        0        0        0 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/calibration/__init__.py
+-rw-r--r--   0        0        0     8874 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/calibration/xgb.py
+-rw-r--r--   0        0        0     3796 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/canonicalization/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/classification/__init__.py
+-rw-r--r--   0        0        0    11811 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/classification/mlp.py
+-rw-r--r--   0        0        0     1185 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/classification/retain_intent.py
+-rw-r--r--   0        0        0       58 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/classification/tokenizers.py
+-rw-r--r--   0        0        0    16771 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/classification/xlmr.py
+-rw-r--r--   0        0        0     7682 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/combine_date_time/__init__.py
+-rw-r--r--   0        0        0    38996 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/duckling_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/error_recovery/__init__.py
+-rw-r--r--   0        0        0    20340 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/error_recovery/error_recovery.py
+-rw-r--r--   0        0        0    12306 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/intent_entity_mutator/__init__.py
+-rw-r--r--   0        0        0      743 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py
+-rw-r--r--   0        0        0      797 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/intent_entity_mutator/const.py
+-rw-r--r--   0        0        0      313 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/intent_entity_mutator/registry.py
+-rw-r--r--   0        0        0     1804 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/lb_plugin/__init__.py
+-rw-r--r--   0        0        0    14129 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/list_entity_plugin/__init__.py
+-rw-r--r--   0        0        0    11529 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/list_search_plugin/__init__.py
+-rw-r--r--   0        0        0     4841 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/list_search_plugin/sample_config.yaml
+-rw-r--r--   0        0        0     4705 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/merge_asr_output/__init__.py
+-rw-r--r--   0        0        0     1571 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/oos_filter/__init__.py
+-rw-r--r--   0        0        0     4253 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/qc_plugin/__init__.py
+-rw-r--r--   0        0        0      833 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/slot_filler/__init__.py
+-rw-r--r--   0        0        0     4154 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/slot_filler/rule_slot_filler.py
+-rw-r--r--   0        0        0        0 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/voting/__init__.py
+-rw-r--r--   0        0        0     1862 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/types/__init__.py
+-rw-r--r--   0        0        0      170 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/types/entity/__init__.py
+-rw-r--r--   0        0        0      914 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/types/entity/address/__init__.py
+-rw-r--r--   0        0        0     1811 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/types/entity/amount_of_money/__init__.py
+-rw-r--r--   0        0        0     7361 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/types/entity/base_entity/__init__.py
+-rw-r--r--   0        0        0     2281 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/types/entity/credit_card_number/__init__.py
+-rw-r--r--   0        0        0     3637 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/types/entity/deserialize/__init__.py
+-rw-r--r--   0        0        0     4432 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/types/entity/duration/__init__.py
+-rw-r--r--   0        0        0      975 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/types/entity/keyword/__init__.py
+-rw-r--r--   0        0        0     4698 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/types/entity/numerical/__init__.py
+-rw-r--r--   0        0        0     2271 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/types/entity/people/__init__.py
+-rw-r--r--   0        0        0      910 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/types/entity/pincode/__init__.py
+-rw-r--r--   0        0        0    13534 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/types/entity/time/__init__.py
+-rw-r--r--   0        0        0     8803 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/types/entity/time_interval/__init__.py
+-rw-r--r--   0        0        0     8893 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/types/intent/__init__.py
+-rw-r--r--   0        0        0      154 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/types/plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/types/signal/__init__.py
+-rw-r--r--   0        0        0      194 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/types/signal/signal.py
+-rw-r--r--   0        0        0      991 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/types/slots/__init__.py
+-rw-r--r--   0        0        0      191 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/types/utterances/__init__.py
+-rw-r--r--   0        0        0      638 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/utils/__init__.py
+-rw-r--r--   0        0        0    10469 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/utils/config.py
+-rw-r--r--   0        0        0     2180 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/utils/datetime.py
+-rw-r--r--   0        0        0     3437 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/utils/file_handler.py
+-rw-r--r--   0        0        0      808 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/utils/logger.py
+-rw-r--r--   0        0        0     2687 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/utils/misc.py
+-rw-r--r--   0        0        0      584 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/utils/naive_lang_detect.py
+-rw-r--r--   0        0        0     8236 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/utils/normalize_utterance.py
+-rw-r--r--   0        0        0     3605 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/utils/temperature_scaling.py
+-rw-r--r--   0        0        0       47 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/workflow/__init__.py
+-rw-r--r--   0        0        0     6917 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/workflow/workflow.py
+-rw-r--r--   0        0        0     1471 2023-05-10 14:37:36.824187 dialogy-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1651 1970-01-01 00:00:00.000000 dialogy-2.0.6/PKG-INFO
```

### Comparing `dialogy-2.0.5/LICENSE.md` & `dialogy-2.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/base/entity_extractor/__init__.py` & `dialogy-2.0.6/dialogy/base/entity_extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/base/input/__init__.py` & `dialogy-2.0.6/dialogy/base/input/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/base/output/__init__.py` & `dialogy-2.0.6/dialogy/base/output/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/base/plugin/__init__.py` & `dialogy-2.0.6/dialogy/base/plugin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,27 +252,27 @@
             logger.warning(
                 f"project_name is set to None for {type(self)} because no value was received during "
                 f"the instantiation of the plugin."
                 f"If you are seeing this on core-slu-service, pipeline will fail."
             )
 
     @abstractmethod
-    def utility(self, input_: Input, output: Output) -> Any:
+    async def utility(self, input_: Input, output: Output) -> Any:
         """
         An abstract method that describes the plugin's functionality.
 
         :param input: The workflow's input.
         :type input: Input
         :param output: The workflow's output.
         :type output: Output
         :return: The value returned by the plugin.
         :rtype: Any
         """
 
-    def __call__(self, input, output):  # type: ignore
+    async def __call__(self, input, output):  # type: ignore
         """
         Set workflow with output.
 
         This important book-keeping method is called by the workflow.
 
         - If the plugin guards evaluate to :code:`True`, we don't run the plugin's business logic.
         - Otherwise, we obtain the plugins transformation and set it on :code:`self.dest` path within the workflow.
@@ -282,26 +282,25 @@
 
         .. _PluginBookkeeping:
 
         :param workflow: An instance of :ref:`Workflow <WorkflowClass>`.
         :type workflow: Workflow
         """
         logger.enable(str(self)) if self.debug else logger.disable(str(self))
-
         if input is None:
             return input, output
 
         if output is None:
             return input, output
 
         if self.prevent(input, output):
             return input, output
 
         # compute
-        return_value = self.utility(input, output)
+        return_value = await self.utility(input, output)
         if return_value is None:
             return input, output
 
         if self.dynamic_output_path:
             value, dest = return_value[0], return_value[1]
         else:
             value, dest = return_value, self.dest
```

### Comparing `dialogy-2.0.5/dialogy/cli/__init__.py` & `dialogy-2.0.6/dialogy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/cli/project.py` & `dialogy-2.0.6/dialogy/cli/project.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/cli/workflow.py` & `dialogy-2.0.6/dialogy/cli/workflow.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/constants/__init__.py` & `dialogy-2.0.6/dialogy/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/plugins/registry.py` & `dialogy-2.0.6/dialogy/plugins/registry.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/plugins/text/address_parser/__init__.py` & `dialogy-2.0.6/dialogy/plugins/text/address_parser/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
         provider_functions: Dict[str, Callable[..., str]] = {
             "google": get_gmaps_address(maps_client),
             "mmi": get_mapmyindia_address(maps_client),
         }
         self.provider_fn = provider_functions[provider]
 
-    def utility(self, input_: Input, output: Output) -> List[Optional[AddressEntity]]:
+    async def utility(self, input_: Input, output: Output) -> List[Optional[AddressEntity]]:
 
         intents = output.intents
         pincode = ""
         matching_address: Optional[str] = None
         address: Optional[AddressEntity] = None
 
         if (not intents) or (not isinstance(intents, list)):
```

### Comparing `dialogy-2.0.5/dialogy/plugins/text/address_parser/mapmyindia.py` & `dialogy-2.0.6/dialogy/plugins/text/address_parser/mapmyindia.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/plugins/text/address_parser/maps.py` & `dialogy-2.0.6/dialogy/plugins/text/address_parser/maps.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/plugins/text/calibration/xgb.py` & `dialogy-2.0.6/dialogy/plugins/text/calibration/xgb.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
             return transcripts
 
         return normalize(self.filter_asr_output(utterances))
 
     def save(self, fname: str) -> None:
         pickle.dump(self, open(fname, "wb"))
 
-    def utility(self, input: Input, _: Output) -> Any:
+    async def utility(self, input: Input, _: Output) -> Any:
         return self.inference(
             input.transcripts, input.utterances
         )  # pylint: disable=no-value-for-parameter
 
     def validate(self, df: pd.DataFrame) -> bool:
         """
         Return if `df` is a valid trascription tagging job
```

### Comparing `dialogy-2.0.5/dialogy/plugins/text/canonicalization/__init__.py` & `dialogy-2.0.6/dialogy/plugins/text/canonicalization/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         for i, transcript in enumerate(canonicalized_transcripts):
             for pattern in self._mask_patterns:
                 canonicalized_transcripts[i] = pattern.sub(self.mask, transcript)
 
         return canonicalized_transcripts
 
-    def utility(self, input: Input, output: Output) -> Any:
+    async def utility(self, input: Input, output: Output) -> Any:
         entities = output.entities
         transcripts = input.transcripts
         return self.mask_transcript(entities, transcripts)
 
     def transform(self, training_data: pd.DataFrame) -> pd.DataFrame:
         if not self.use_transform:
             return training_data
```

### Comparing `dialogy-2.0.5/dialogy/plugins/text/classification/mlp.py` & `dialogy-2.0.6/dialogy/plugins/text/classification/mlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,11 +317,11 @@
         """
         Load the plugin artifacts.
         """
         self.model_pipeline = load_file(
             self.mlp_model_path, mode="rb", loader=joblib.load
         )
 
-    def utility(self, input: Input, _: Output) -> Any:
+    async def utility(self, input: Input, _: Output) -> Any:
         return self.inference(
             input.clf_feature
         )  # pylint: disable=no-value-for-parameter
```

### Comparing `dialogy-2.0.5/dialogy/plugins/text/classification/retain_intent.py` & `dialogy-2.0.6/dialogy/plugins/text/classification/retain_intent.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,9 +28,9 @@
     def retain(self, intents: List[Intent]) -> ORIGINAL_INTENT_TYPE:
         if not intents:
             return {}
 
         intent, *_ = intents
         return {const.NAME: intent.name, const.SCORE: intent.score}
 
-    def utility(self, _: Input, output: Output) -> ORIGINAL_INTENT_TYPE:
+    async def utility(self, _: Input, output: Output) -> ORIGINAL_INTENT_TYPE:
         return self.retain(output.intents)
```

### Comparing `dialogy-2.0.5/dialogy/plugins/text/classification/xlmr.py` & `dialogy-2.0.6/dialogy/plugins/text/classification/xlmr.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 from typing import Any, Dict, List, Optional, Tuple
 from pprint import pformat
 
 import numpy as np
 import pandas as pd
 from sklearn import preprocessing
 from tqdm import tqdm
+import aiohttp
+import json
+from aiohttp.client_exceptions import ClientConnectorError
 
 import dialogy.constants as const
 from dialogy.base import Guard, Input, Output, Plugin
 from dialogy.types import Intent
 from dialogy.utils import load_file, logger, read_from_json, save_file
 import torch
 from torch.profiler import profile, record_function, ProfilerActivity
@@ -138,21 +141,15 @@
                     "production or testing, then this should be checked!"
                 )
 
         elif self.purpose == const.PRODUCTION:
             # model inference service session configuration
             self.url = url
             self.timeout = timeout
-            self.session = requests.Session()
-            self.session.mount(
-                "http://",
-                requests.adapters.HTTPAdapter(
-                    max_retries=1, pool_maxsize=10, pool_block=True
-                ),
-            )
+            self.session = aiohttp.ClientSession()
             self.headers: Dict[str, str] = {
                 "Content-Type": "application/json"
             }
 
         self.debug = debug
 
     def init_model(self, label_count: Optional[int] = None) -> None:
@@ -193,45 +190,36 @@
                 **self.kwargs,
             )
 
     @property
     def valid_labelencoder(self) -> bool:
         return hasattr(self.labelencoder, "classes_")
 
-    def _request_model_inference(self, texts: List[str]) -> Tuple[Any, Any]:
+    async def _request_model_inference(self, texts: List[str]) -> Tuple[Any, Any]:
         payload = {"transcripts": texts}
-
         try:
-            response = self.session.post(
-                self.url, json=payload, headers=self.headers, timeout=self.timeout
-            )
-
-            if response.status_code == 200:
-                # The API call was successful, expect the following to contain entities.
-                # A list of dicts or an empty list.
-                result = response.json()
-                return result.get("intents", []), result.get("logits", [])
-            
-        except requests.exceptions.Timeout as timeout_exception:
-            logger.error(f"Model Inference Service timed out: {timeout_exception}")  # pragma: no cover
-            logger.error(pformat(payload))  # pragma: no cover
-            return [], []  # pragma: no cover
-        
-        except requests.exceptions.ConnectionError as connection_error:
+            async with self.session.post(self.url, data=json.dumps(payload), headers=self.headers) as resp:
+                status_code = resp.status
+                if status_code == 200:
+                    result = await resp.json()
+                    return result.get("intents", []), result.get("logits", [])
+                else:
+                    result = await resp.text()
+        except ClientConnectorError as connection_error:
             logger.error(f"Model Inference Service is turned off?: {connection_error}")
             logger.error(pformat(payload))
             raise requests.exceptions.ConnectionError from connection_error
 
         # Control flow reaching here would mean the API call wasn't successful.
         # To prevent rest of the things from crashing, we will raise an exception.
         raise ValueError(
-            f"Model Inference Service API call failed | [{response.status_code}]: {response.text}"
+            f"Model Inference Service API call failed | [{status_code}]: {result}"
         )
 
-    def inference(
+    async def inference(
         self,
         texts: Optional[List[str]],
         state: Optional[str] = None,
         lang: Optional[str] = None,
         nls_label: Optional[str] = None,
     ) -> List[Intent]:
 
@@ -275,15 +263,15 @@
         if self.use_state and state:
             texts[0] += "<s> " + state + " </s>"
 
         logger.debug(f"Classifier Input:\n{texts}")
 
         # inference
         if self.purpose == const.PRODUCTION:
-            predicted_intents, logits = self._request_model_inference(texts)
+            predicted_intents, logits = await self._request_model_inference(texts)
             # postprocessing
             logits = np.array(logits)
 
         elif self.purpose == const.TEST:
             if not self.model:
                 return [fallback_output]
             predictions, logits = self.model.predict(texts)
@@ -434,11 +422,11 @@
         """
         Load the plugin artifacts.
         """
         self.labelencoder = load_file(
             self.labelencoder_file_path, mode="rb", loader=pickle.load
         )
 
-    def utility(self, input: Input, _: Output) -> List[Intent]:
-        return self.inference(
+    async def utility(self, input: Input, _: Output) -> List[Intent]:
+        return await self.inference(
             input.clf_feature, input.current_state, input.lang, input.nls_label
         )
```

### Comparing `dialogy-2.0.5/dialogy/plugins/text/combine_date_time/__init__.py` & `dialogy-2.0.6/dialogy/plugins/text/combine_date_time/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,14 +196,14 @@
             in CombineDateTimeOverSlots.SUPPORTED_ENTITIES,
         )
         combined_time_entities = [
             self.join(entity, previously_filled_time_entity) for entity in time_entities
         ]
         return combined_time_entities + other_entities
 
-    def utility(self, input: Input, output: Output) -> List[BaseEntity]:
+    async def utility(self, input: Input, output: Output) -> List[BaseEntity]:
         """
         Combine the date and time entities collected across turns into a single entity.
         """
         return self.combine_time_entities_from_slots(
             input.slot_tracker, output.entities
         )
```

### Comparing `dialogy-2.0.5/dialogy/plugins/text/duckling_plugin/__init__.py` & `dialogy-2.0.6/dialogy/plugins/text/duckling_plugin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -498,21 +498,23 @@
     In [6]: input_, output = workflow.run(Input(utterances=utterances, reference_time=reference_time))
 
     In [7]: output
 
 Now we can see that it gives the correct entity value i.e *"2022-03-17T12:00:00+05:30"*
 
 """
-import json
 import operator
 import traceback
-from concurrent import futures
 from datetime import datetime
 from pprint import pformat
 from typing import Any, Callable, Dict, List, Optional, Union
+import aiohttp
+import asyncio
+import json
+from aiohttp.client_exceptions import ClientConnectorError
 
 import pandas as pd
 import pydash as py_
 import pytz
 import requests
 from pytz.tzinfo import BaseTzInfo
 from tqdm import tqdm
@@ -684,15 +686,15 @@
             if isinstance(activate_latent_entities, bool)
             else activate_latent_entities()
         )
 
         payload = {
             "text": text,
             "locale": locale or self.locale,
-            "tz": self.__set_timezone(),
+            "tz": str(self.__set_timezone()),
             "dims": json.dumps(dimensions),
             "reftime": reference_time,
             "latent": activate_latent_entities,
         }
         logger.debug("Duckling API payload:")
         logger.debug(pformat(payload))
 
@@ -796,16 +798,17 @@
                 constraints=self.constraints,
             )
             if entity and entity.value:
                 entity.add_parser(self)
                 deserialized_entities.append(entity)
         return deserialized_entities
 
-    def _get_entities(
+    async def _get_entities(
         self,
+        session: aiohttp.ClientSession,
         text: str,
         locale: str = "en_IN",
         reference_time: Optional[int] = None,
         use_latent: Union[Callable[..., bool], bool] = False,
         sort_idx: int = 0,
     ) -> Dict[str, Any]:
         """
@@ -823,40 +826,33 @@
         :raises ValueError: Duckling API call failure leading to no json response.
         :return: Duckling entities as :code:`dicts`.
         :rtype: List[Dict[str, Any]]
         """
         body = self.__create_req_body(
             text, reference_time=reference_time, locale=locale, use_latent=use_latent
         )
-
         try:
-            response = self.session.post(
-                self.url, data=body, headers=self.headers, timeout=self.timeout
-            )
+            async with session.post(self.url, data=body, headers=self.headers) as resp:
+                status = resp.status
+                if status == 200:
+                    result = await resp.json()
+                    # The API call was successful, expect the following to contain entities.
+                    # A list of dicts or an empty list.
+                    return {const.IDX: sort_idx, const.VALUE: result}
+                else:
+                    raise ValueError(
+                        f"Duckling API call failed | [{status}]: {await resp.text()}"
+                    )
 
-            if response.status_code == 200:
-                # The API call was successful, expect the following to contain entities.
-                # A list of dicts or an empty list.
-                return {const.IDX: sort_idx, const.VALUE: response.json()}
-        except requests.exceptions.Timeout as timeout_exception:
-            logger.error(f"Duckling timed out: {timeout_exception}")  # pragma: no cover
-            logger.error(pformat(body))  # pragma: no cover
-            return {const.IDX: sort_idx, const.VALUE: []}  # pragma: no cover
-        except requests.exceptions.ConnectionError as connection_error:
+        except ClientConnectorError as connection_error:
             logger.error(f"Duckling server is turned off?: {connection_error}")
             logger.error(pformat(body))
-            raise requests.exceptions.ConnectionError from connection_error
+            raise connection_error
 
-        # Control flow reaching here would mean the API call wasn't successful.
-        # To prevent rest of the things from crashing, we will raise an exception.
-        raise ValueError(
-            f"Duckling API call failed | [{response.status_code}]: {response.text}"
-        )
-
-    def _get_entities_concurrent(
+    async def _get_entities_concurrent(
         self,
         texts: List[str],
         locale: str = "en_IN",
         reference_time: Optional[int] = None,
         use_latent: Union[Callable[..., bool], bool] = False,
     ) -> List[List[Dict[str, Any]]]:
         """
@@ -871,34 +867,32 @@
                                 to parse the values into usable dates/times, defaults to None
         :type reference_time: Optional[int], optional
         :param use_latent: True returns latent entities, defaults to False
         :type use_latent: bool, optional
         :return: Duckling entities as :code:`dicts`.
         :rtype: List[List[Dict[str, Any]]]
         """
-        workers = min(10, max(len(texts), 1))
-        with futures.ThreadPoolExecutor(max_workers=workers) as executor:
-            futures_ = [
-                executor.submit(
-                    self._get_entities,
-                    text,
-                    locale,
-                    reference_time=reference_time,
-                    use_latent=use_latent,
-                    sort_idx=i,
+        async with aiohttp.ClientSession() as session:
+            tasks = []
+            for i, text in enumerate(texts):
+                tasks.append(asyncio.ensure_future(
+                    self._get_entities(
+                        session,
+                        text,
+                        locale,
+                        reference_time=reference_time,
+                        use_latent=use_latent,
+                        sort_idx=i)))
+            results = await asyncio.gather(*tasks)
+            return [
+                entities[const.VALUE]
+                for entities in sorted(
+                    results, key=lambda entities: entities[const.IDX]
                 )
-                for i, text in enumerate(texts)
             ]
-        entities_list = [future.result() for future in futures.as_completed(futures_)]
-        return [
-            entities[const.VALUE]
-            for entities in sorted(
-                entities_list, key=lambda entities: entities[const.IDX]
-            )
-        ]
 
     def apply_entity_classes(
         self,
         list_of_entities: List[List[Dict[str, Any]]],
         reference_time: Optional[int] = None,
         timezone: str = "UTC",
         duration_cast_operator: Optional[str] = None,
@@ -929,15 +923,15 @@
                 "https://stackoverflow.com/questions/20822821/what-is-a-unix-timestamp-and-why-use-it\n"
             )
 
         if not input_is_str and not inputs_are_list_of_strings:
             raise TypeError(f"Expected {input_} to be a List[str] or str.")
         return self
 
-    def parse(
+    async def parse(
         self,
         transcripts: Union[str, List[str]],
         locale: Optional[str] = None,
         reference_time: Optional[int] = None,
         use_latent: Union[Callable[..., bool], bool] = False,
         intents: Optional[List[Intent]] = None,
     ) -> List[BaseEntity]:
@@ -959,51 +953,51 @@
 
         locale = locale or self.locale
         self.reference_time = reference_time = reference_time or self.reference_time
         self.validate(transcripts, reference_time)
         if isinstance(transcripts, str):
             transcripts = [transcripts]  # pragma: no cover
 
-        list_of_entities = self._get_entities_concurrent(
+        list_of_entities = await self._get_entities_concurrent(
             transcripts,
             locale=locale,
             reference_time=reference_time,
             use_latent=use_latent,
         )
         entities = self.apply_entity_classes(
             list_of_entities,
             reference_time,
             duration_cast_operator=duration_cast_operator,
         )
         entities = self.entity_consensus(entities, len(transcripts))
         return self.apply_filters(entities)
 
-    def utility(self, input: Input, output: Output) -> List[BaseEntity]:
+    async def utility(self, input: Input, output: Output) -> List[BaseEntity]:
         """
         Produces Duckling entities, runs with a :ref:`Workflow's run<workflow_run>` method.
 
         :param argbrightons: Expects a tuple of :code:`Tuple[natural language for parsing entities, reference time in milliseconds, locale]`
         :type args: Tuple(Union[str, List[str]], int, str)
         :return: A list of duckling entities.
         :rtype: List[BaseEntity]
         """
         transcripts = input.transcripts
         self.reference_time = input.reference_time
         self.locale = input.locale or self.locale
         use_latent = input.latent_entities
 
-        return self.parse(
+        return await self.parse(
             transcripts,
             locale=self.locale,
             reference_time=self.reference_time,
             use_latent=use_latent,
             intents=output.intents,
         )
 
-    def transform(self, training_data: pd.DataFrame) -> pd.DataFrame:
+    async def transform(self, training_data: pd.DataFrame) -> pd.DataFrame:
         """
         Transform training data.
 
         :param training_data: Training data.
         :type training_data: pd.DataFrame
         :return: Transformed training data.
         :rtype: pd.DataFrame
@@ -1026,15 +1020,15 @@
             elif pd.isna(reference_time):
                 continue
             elif not isinstance(reference_time, int):
                 raise TypeError(
                     f"{reference_time=} should be isoformat date or unix timestamp integer."
                 )
             transcripts = self.make_transform_values(row[self.input_column])
-            entities = self.parse(
+            entities = await self.parse(
                 transcripts,
                 lang_detect_from_text(self.input_column),
                 reference_time=reference_time,
                 use_latent=self.activate_latent_entities,
             )
             if row[self.output_column] is None or pd.isnull(row[self.output_column]):
                 training_data.at[i, self.output_column] = entities
```

### Comparing `dialogy-2.0.5/dialogy/plugins/text/error_recovery/error_recovery.py` & `dialogy-2.0.6/dialogy/plugins/text/error_recovery/error_recovery.py`

 * *Files 1% similar despite different names*

```diff
@@ -521,15 +521,15 @@
     ) -> None:
         self.rules = Rule.from_list(rules)
         self.dest = dest
         self.guards = guards or []
         self.replace_output = replace_output
         self.debug = debug
 
-    def utility(self, input_: Input, output: Output) -> None:
+    async def utility(self, input_: Input, output: Output) -> None:
         environment = Environment(
             intents=output.intents,
             entities=output.entities,
             previous_intent=input_.previous_intent,
             current_state=input_.current_state,
             expected_slots=input_.expected_slots or set(),  # type: ignore
         )
```

### Comparing `dialogy-2.0.5/dialogy/plugins/text/intent_entity_mutator/__init__.py` & `dialogy-2.0.6/dialogy/plugins/text/intent_entity_mutator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,15 +293,15 @@
                     return intents, const.OUTPUT_DEST_INTENT
                 else:
                     mutate_entities = [BaseEntity.from_dict(mutate_to)]
                     return mutate_entities, const.OUTPUT_DEST_ENTITY
 
         return intents, const.OUTPUT_DEST_INTENT
 
-    def utility(
+    async def utility(
         self, input_: Input, output: Output
     ) -> Tuple[Union[List[Intent], List[BaseEntity]], str]:
 
         current_state = input_.current_state
         intents = output.intents
         entities = output.entities
         previous_intent = input_.previous_intent
```

### Comparing `dialogy-2.0.5/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py` & `dialogy-2.0.6/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/plugins/text/intent_entity_mutator/const.py` & `dialogy-2.0.6/dialogy/plugins/text/intent_entity_mutator/const.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/plugins/text/lb_plugin/__init__.py` & `dialogy-2.0.6/dialogy/plugins/text/lb_plugin/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,16 +41,16 @@
             input_column=input_column,
             output_column=output_column,
             use_transform=use_transform,
             debug=debug,
             **kwargs
         )
 
-    def utility(self, input_: Input, output: Output) -> List[BaseEntity]:
-        entity_list = super().utility(input_, output)
+    async def utility(self, input_: Input, output: Output) -> List[BaseEntity]:
+        entity_list = await super().utility(input_, output)
         datetime_list, other_list = partition(
             entity_list, lambda x: x.entity_type in ["datetime", "date", "time"]
         )
         if datetime_list:
             other_list.append(min(datetime_list, key=lambda x: x.alternative_index))
 
         return other_list
```

### Comparing `dialogy-2.0.5/dialogy/plugins/text/list_entity_plugin/__init__.py` & `dialogy-2.0.6/dialogy/plugins/text/list_entity_plugin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,15 +277,15 @@
 
         logger.debug("Parsed entities")
         logger.debug(entities)
 
         aggregated_entities = self.entity_consensus(entities, len(transcripts))
         return self.apply_filters(aggregated_entities)
 
-    def utility(self, input: Input, _: Output) -> Any:
+    async def utility(self, input: Input, _: Output) -> Any:
         transcripts = input.transcripts
         return self.get_entities(transcripts)  # pylint: disable=no-value-for-parameter
 
     def ner_search(self, transcript: str) -> MatchType:
         """
         Wrapper over spacy's ner search.
```

### Comparing `dialogy-2.0.5/dialogy/plugins/text/list_search_plugin/__init__.py` & `dialogy-2.0.6/dialogy/plugins/text/list_search_plugin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,11 +295,11 @@
                 entities.append(entity_)
 
         logger.debug("Parsed entities")
         logger.debug(entities)
         aggregated_entities = self.entity_consensus(entities, len(transcripts))
         return self.apply_filters(aggregated_entities)
 
-    def utility(self, input_: Input, _: Output) -> Any:
+    async def utility(self, input_: Input, _: Output) -> Any:
         return self.get_entities(
             input_.transcripts, input_.lang
         )  # pylint: disable=no-value-for-parameter
```

### Comparing `dialogy-2.0.5/dialogy/plugins/text/list_search_plugin/sample_config.yaml` & `dialogy-2.0.6/dialogy/plugins/text/list_search_plugin/sample_config.yaml`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/plugins/text/merge_asr_output/__init__.py` & `dialogy-2.0.6/dialogy/plugins/text/merge_asr_output/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             input_column=input_column,
             output_column=output_column,
             use_transform=use_transform,
             debug=debug,
             **kwargs
         )
 
-    def utility(self, input: Input, _: Output) -> Any:
+    async def utility(self, input: Input, _: Output) -> Any:
         return merge_asr_output(input.utterances)
 
     def transform(self, training_data: pd.DataFrame) -> pd.DataFrame:
         if not self.use_transform:
             return training_data
 
         training_data["use"] = True
```

### Comparing `dialogy-2.0.5/dialogy/plugins/text/oos_filter/__init__.py` & `dialogy-2.0.6/dialogy/plugins/text/oos_filter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,9 +42,9 @@
                 "Either OOSFilter was added before the intent classifier plugin or the intents list is empty"
             )
 
         if intents[0].score < self.threshold:
             intents[0].name = self.intent_oos
         return intents
 
-    def utility(self, input_: Input, output: Output) -> List[Intent]:
+    async def utility(self, input_: Input, output: Output) -> List[Intent]:
         return self.set_oos_intent(output.intents)
```

### Comparing `dialogy-2.0.5/dialogy/plugins/text/qc_plugin/__init__.py` & `dialogy-2.0.6/dialogy/plugins/text/qc_plugin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         training_data["conflicting_intents"] = training_data["frozen_set_hash"].map(
             filtered_hash_with_different_intents_tagged
         )
         training_data["use"] = training_data["conflicting_intents"].isna()
 
         return training_data
 
-    def utility(self, input: Input, _: Output) -> Any:
+    async def utility(self, input: Input, _: Output) -> Any:
         return
 
     def transform(self, training_data: pd.DataFrame) -> pd.DataFrame:
         if not self.use_transform:
             return training_data
 
         training_data["use"] = True
```

### Comparing `dialogy-2.0.5/dialogy/plugins/text/slot_filler/__init__.py` & `dialogy-2.0.6/dialogy/plugins/text/slot_filler/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/plugins/text/slot_filler/rule_slot_filler.py` & `dialogy-2.0.6/dialogy/plugins/text/slot_filler/rule_slot_filler.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,9 +103,9 @@
         for entity in entities:
             intent.fill_slot(
                 entity, fill_multiple=self.fill_multiple, expected_slots=expected_slots
             )
         intent.cleanup()
         return [intent, *rest]
 
-    def utility(self, input_: Input, output: Output) -> List[Intent]:
+    async def utility(self, input_: Input, output: Output) -> List[Intent]:
         return self.fill(output.intents, output.entities, set(input_.expected_slots))
```

### Comparing `dialogy-2.0.5/dialogy/types/__init__.py` & `dialogy-2.0.6/dialogy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/types/entity/address/__init__.py` & `dialogy-2.0.6/dialogy/types/entity/address/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/types/entity/amount_of_money/__init__.py` & `dialogy-2.0.6/dialogy/types/entity/amount_of_money/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/types/entity/base_entity/__init__.py` & `dialogy-2.0.6/dialogy/types/entity/base_entity/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         }
 
         class KeywordEntity {
         }
 
         class DurationEntity {
             +str unit
+            +str grain
             +dict normalized
             +DurationEntity from_duckling(d)
         }
 
         class NumericalEntity {
             +NumericalEntity from_duckling(d)
         }
```

### Comparing `dialogy-2.0.5/dialogy/types/entity/credit_card_number/__init__.py` & `dialogy-2.0.6/dialogy/types/entity/credit_card_number/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/types/entity/deserialize/__init__.py` & `dialogy-2.0.6/dialogy/types/entity/deserialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/types/entity/duration/__init__.py` & `dialogy-2.0.6/dialogy/types/entity/duration/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,35 +74,39 @@
     to get to a date that's 2 days ahead.
     """
 
     unit: str
     normalized: Dict[str, Any] = Field(default_factory=dict)
     _meta: Dict[str, str] = Field(default_factory=dict)
     entity_type: str = const.DURATION
+    grain: str
 
     @classmethod
     def from_duckling(
         cls,
         d: Dict[str, Any],
         alternative_index: int,
         reference_time: Optional[int] = None,
         timezone: Optional[str] = None,
         duration_cast_operator: Optional[str] = None,
         **kwargs: Any,
     ) -> Union[DurationEntity, TimeEntity]:
-        value = d[const.VALUE][const.NORMALIZED][const.VALUE]
+        value_dict = d[const.VALUE]
+        value = value_dict[const.NORMALIZED][const.VALUE]
+        grain = value_dict.get(const.UNIT)
         entity = cls(
             range={const.START: d[const.START], const.END: d[const.END]},
             body=d[const.BODY],
             dim=d[const.DIM],
             alternative_index=alternative_index,
             latent=d[const.LATENT],
             values=[{const.VALUE: value}],
             unit=d[const.VALUE][const.UNIT],
             normalized=d[const.VALUE][const.NORMALIZED],
+            grain=grain,
         )
         if reference_time and timezone and duration_cast_operator:
             return entity.as_time(reference_time, timezone, duration_cast_operator)
         return entity
 
     def as_time(
         self, reference_unix_ts: int, timezone: str, duration_cast_operator: str
```

### Comparing `dialogy-2.0.5/dialogy/types/entity/keyword/__init__.py` & `dialogy-2.0.6/dialogy/types/entity/keyword/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/types/entity/numerical/__init__.py` & `dialogy-2.0.6/dialogy/types/entity/numerical/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/types/entity/people/__init__.py` & `dialogy-2.0.6/dialogy/types/entity/people/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/types/entity/pincode/__init__.py` & `dialogy-2.0.6/dialogy/types/entity/pincode/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/types/entity/time/__init__.py` & `dialogy-2.0.6/dialogy/types/entity/time/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/types/entity/time_interval/__init__.py` & `dialogy-2.0.6/dialogy/types/entity/time_interval/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/types/intent/__init__.py` & `dialogy-2.0.6/dialogy/types/intent/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/types/slots/__init__.py` & `dialogy-2.0.6/dialogy/types/slots/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/utils/__init__.py` & `dialogy-2.0.6/dialogy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/utils/config.py` & `dialogy-2.0.6/dialogy/utils/config.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/utils/datetime.py` & `dialogy-2.0.6/dialogy/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/utils/file_handler.py` & `dialogy-2.0.6/dialogy/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/utils/logger.py` & `dialogy-2.0.6/dialogy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/utils/misc.py` & `dialogy-2.0.6/dialogy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/utils/naive_lang_detect.py` & `dialogy-2.0.6/dialogy/utils/naive_lang_detect.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/utils/normalize_utterance.py` & `dialogy-2.0.6/dialogy/utils/normalize_utterance.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/utils/temperature_scaling.py` & `dialogy-2.0.6/dialogy/utils/temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.5/dialogy/workflow/workflow.py` & `dialogy-2.0.6/dialogy/workflow/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         Post init hook.
         """
         self.lock = Lock()
         for plugin in self.plugins:
             if isinstance(plugin, Plugin):
                 plugin.debug = self.debug & plugin.debug
 
-    def run(self, input: Input, output: Output = None):  # type: ignore
+    async def run(self, input: Input, output: Output = None):  # type: ignore
         """
         .. _workflow_run:
 
         Get final results from the workflow.
 
         The current workflow exhibits the following simple procedure:
         pre-processing -> inference -> post-processing.
@@ -202,16 +202,18 @@
                     "before": {
                         "input": input.dict(),
                         "output": output.dict(),
                     },
                 }
 
             start = time.perf_counter()
-            with self.lock:
-                input, output = plugin(input, output)
+            # with self.lock:
+            # Removing the lock as plugins are
+            # expected to be implemented in a thread safe manner
+            input, output = await plugin(input, output)
             end = time.perf_counter()
 
             # logs are available only when debug=False during class initialization
             if self.debug:
                 history["after"] = {
                     "input": input.dict(),
                     "output": output.dict(),
```

### Comparing `dialogy-2.0.5/pyproject.toml` & `dialogy-2.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dialogy"
-version = "2.0.5"
+version = "2.0.6"
 description = "Dialogy is a library for building and managing SLU applications."
 authors = ["Amresh Venugopal <amresh.venugopal@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/skit-ai/dialogy"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
@@ -29,17 +29,19 @@
 types-pytz = "^2021.3.5"
 types-requests = "^2.27.11"
 types-setuptools = "^57.4.10"
 black = "^22.8.0"
 googlemaps = "^4.6.0"
 torch = "1.12.1"
 pydantic = "^1.10.2"
+aiohttp = "^3.8.4"
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.0"
+pytest = "^7.3.1"
+pytest-asyncio = "^0.21.0"
 pytest-cov = "^2.10.1"
 copier = "^6.0.0"
 mypy = "^0.982"
 httpretty = "^1.0.3"
 rope = "^0.18.0"
 bandit = "^1.7.0"
 pylint = "^2.6.0"
```

### Comparing `dialogy-2.0.5/PKG-INFO` & `dialogy-2.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: dialogy
-Version: 2.0.5
+Version: 2.0.6
 Summary: Dialogy is a library for building and managing SLU applications.
 Home-page: https://github.com/skit-ai/dialogy
 License: MIT
 Author: Amresh Venugopal
 Author-email: amresh.venugopal@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: MarkupSafe (==2.0.1)
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: attrs (==21.3.0)
 Requires-Dist: black (>=22.8.0,<23.0.0)
 Requires-Dist: copier (>=6.0.0,<7.0.0)
 Requires-Dist: googlemaps (>=4.6.0,<5.0.0)
 Requires-Dist: jiwer (>=2.2.0,<3.0.0)
 Requires-Dist: loguru (>=0.5.3,<0.6.0)
 Requires-Dist: matplotlib (>=3.5.1,<4.0.0)
```


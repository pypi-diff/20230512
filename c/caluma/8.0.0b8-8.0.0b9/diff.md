# Comparing `tmp/caluma-8.0.0b8.tar.gz` & `tmp/caluma-8.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caluma-8.0.0b8.tar", max compression
+gzip compressed data, was "caluma-8.0.0b9.tar", max compression
```

## Comparing `caluma-8.0.0b8.tar` & `caluma-8.0.0b9.tar`

### file list

```diff
@@ -1,210 +1,210 @@
--rw-r--r--   0        0        0    43466 2022-06-20 07:44:55.251595 caluma-8.0.0b8/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2022-06-20 07:44:55.251595 caluma-8.0.0b8/LICENSE
-drwxr-xr-x   0        0        0        0 2022-06-20 07:44:55.255595 caluma-8.0.0b8/LICENSES/
--rw-r--r--   0        0        0     1957 2022-06-20 07:44:55.255595 caluma-8.0.0b8/README.md
--rw-r--r--   0        0        0        0 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/__init__.py
--rw-r--r--   0        0        0     5442 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_analytics/README.md
--rw-r--r--   0        0        0        0 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_analytics/__init__.py
--rw-r--r--   0        0        0      105 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_analytics/apps.py
--rw-r--r--   0        0        0     3322 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_analytics/conftest.py
--rw-r--r--   0        0        0      797 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_analytics/factories.py
--rw-r--r--   0        0        0     1543 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_analytics/filters.py
--rw-r--r--   0        0        0     3416 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_analytics/management/commands/run_analytics.py
--rw-r--r--   0        0        0    11086 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_analytics/migrations/0001_initial.py
--rw-r--r--   0        0        0     2008 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_analytics/migrations/0002_analytics_pivot_table.py
--rw-r--r--   0        0        0     1026 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_analytics/migrations/0003_starting_objects.py
--rw-r--r--   0        0        0     1383 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_analytics/migrations/0004_simple_history.py
--rw-r--r--   0        0        0        0 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_analytics/migrations/__init__.py
--rw-r--r--   0        0        0     3469 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_analytics/models.py
--rw-r--r--   0        0        0     3666 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_analytics/pivot_table.py
--rw-r--r--   0        0        0     6996 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_analytics/schema.py
--rw-r--r--   0        0        0     3499 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_analytics/serializers.py
--rw-r--r--   0        0        0    32474 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_analytics/simple_table.py
--rw-r--r--   0        0        0    16037 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_analytics/sql.py
--rw-r--r--   0        0        0     1113 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_analytics/visibility.py
--rw-r--r--   0        0        0        0 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_core/__init__.py
--rw-r--r--   0        0        0      975 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_core/apps.py
--rw-r--r--   0        0        0      195 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_core/collections.py
--rw-r--r--   0        0        0    11297 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_core/conftest.py
--rw-r--r--   0        0        0     3074 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_core/events.py
--rw-r--r--   0        0        0      325 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_core/factories.py
--rw-r--r--   0        0        0      485 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_core/faker.py
--rw-r--r--   0        0        0    18433 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_core/filters.py
--rw-r--r--   0        0        0      642 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_core/forms.py
--rw-r--r--   0        0        0     4176 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_core/health_checks.py
--rw-r--r--   0        0        0     7855 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_core/jexl.py
--rw-r--r--   0        0        0        0 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_core/management/__init__.py
--rw-r--r--   0        0        0        0 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_core/management/commands/__init__.py
--rw-r--r--   0        0        0     1824 2022-06-20 07:44:55.255595 caluma-8.0.0b8/caluma/caluma_core/management/commands/cleanup_history.py
--rw-r--r--   0        0        0     3803 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_core/management/commands/dump_caluma_config.py
--rw-r--r--   0        0        0      794 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_core/management/commands/migrate.py
--rw-r--r--   0        0        0     4768 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_core/management/commands/migrate_to_prefixed_apps.py
--rw-r--r--   0        0        0     3078 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_core/models.py
--rw-r--r--   0        0        0    11206 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_core/mutation.py
--rw-r--r--   0        0        0     3216 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_core/ordering.py
--rw-r--r--   0        0        0     3195 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_core/pagination.py
--rw-r--r--   0        0        0     4485 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_core/permissions.py
--rw-r--r--   0        0        0     1253 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_core/relay.py
--rw-r--r--   0        0        0     4764 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_core/serializers.py
--rw-r--r--   0        0        0     7577 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_core/types.py
--rw-r--r--   0        0        0      387 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_core/urls.py
--rw-r--r--   0        0        0     2430 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_core/validations.py
--rw-r--r--   0        0        0     1607 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_core/views.py
--rw-r--r--   0        0        0     2937 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_core/visibilities.py
--rw-r--r--   0        0        0        0 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_data_source/__init__.py
--rw-r--r--   0        0        0      107 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_data_source/apps.py
--rw-r--r--   0        0        0     2028 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_data_source/data_source_handlers.py
--rw-r--r--   0        0        0     3104 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_data_source/data_sources.py
--rw-r--r--   0        0        0      989 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_data_source/schema.py
--rw-r--r--   0        0        0      486 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_data_source/utils.py
--rw-r--r--   0        0        0        0 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/__init__.py
--rw-r--r--   0        0        0     2472 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/api.py
--rw-r--r--   0        0        0      100 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/apps.py
--rw-r--r--   0        0        0     8317 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/domain_logic.py
--rw-r--r--   0        0        0     5702 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/factories.py
--rw-r--r--   0        0        0    16442 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/filters.py
--rw-r--r--   0        0        0     3283 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/format_validators.py
--rw-r--r--   0        0        0     7198 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/historical_schema.py
--rw-r--r--   0        0        0     7496 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/jexl.py
--rw-r--r--   0        0        0        0 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/management/__init__.py
--rw-r--r--   0        0        0        0 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/management/commands/__init__.py
--rw-r--r--   0        0        0     1880 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/management/commands/copy_form.py
--rw-r--r--   0        0        0      631 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/management/commands/create_bucket.py
--rw-r--r--   0        0        0    10984 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0001_initial.py
--rw-r--r--   0        0        0     2830 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0002_auto_20181221_1517.py
--rw-r--r--   0        0        0     3863 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0003_auto_20190130_0920.py
--rw-r--r--   0        0        0     1566 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0004_auto_20190207_1405.py
--rw-r--r--   0        0        0      826 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0005_auto_20190208_1016.py
--rw-r--r--   0        0        0      801 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0006_choice_type_conversion.py
--rw-r--r--   0        0        0      630 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0007_auto_20190208_1232.py
--rw-r--r--   0        0        0     1180 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0008_auto_20190319_1720.py
--rw-r--r--   0        0        0     2134 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0009_auto_20190321_1722.py
--rw-r--r--   0        0        0     2303 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0010_auto_20190404_0652.py
--rw-r--r--   0        0        0      605 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0011_auto_20190411_0607.py
--rw-r--r--   0        0        0      789 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0012_auto_20190416_1835.py
--rw-r--r--   0        0        0     1257 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0013_auto_20190418_0733.py
--rw-r--r--   0        0        0     1408 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0014_auto_20190429_0910.py
--rw-r--r--   0        0        0      660 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0015_question_format_validators.py
--rw-r--r--   0        0        0      531 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0016_auto_20190510_0843.py
--rw-r--r--   0        0        0      606 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0017_auto_20190619_1320.py
--rw-r--r--   0        0        0     1860 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0018_remove_answer_value_document_data_migration.py
--rw-r--r--   0        0        0      366 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0019_remove_answer_value_document.py
--rw-r--r--   0        0        0    27840 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0020_historicalanswer_historicalanswerdocument_historicaldocument_historicalfile_historicalform_historica.py
--rw-r--r--   0        0        0     2471 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0021_auto_20190708_0905.py
--rw-r--r--   0        0        0     1454 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0022_add_gin_index_to_jsonfields.py
--rw-r--r--   0        0        0      559 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0023_auto_20190729_1448.py
--rw-r--r--   0        0        0     1088 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0024_auto_20190919_1244.py
--rw-r--r--   0        0        0     4835 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0025_dynamicoption_historicaldynamicoption.py
--rw-r--r--   0        0        0      829 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0026_auto_20191031_0834.py
--rw-r--r--   0        0        0     2088 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0027_auto_20200113_0727.py
--rw-r--r--   0        0        0    12676 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0028_auto_20200210_0929.py
--rw-r--r--   0        0        0     1571 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0029_dynamic_option_unique_together.py
--rw-r--r--   0        0        0     1282 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0030_auto_20200219_1359.py
--rw-r--r--   0        0        0     1702 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0031_auto_20200220_0910.py
--rw-r--r--   0        0        0     1154 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0032_auto_20200220_1311.py
--rw-r--r--   0        0        0     1270 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0033_slugfield_length.py
--rw-r--r--   0        0        0      520 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0034_fix_fk_lengths.py
--rw-r--r--   0        0        0     1688 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0035_historicalanswer_history_question_type.py
--rw-r--r--   0        0        0     1387 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0036_default_answers.py
--rw-r--r--   0        0        0      611 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0037_default_answer_one2one.py
--rw-r--r--   0        0        0     3051 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0038_auto_20201224_0920.py
--rw-r--r--   0        0        0      461 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0038_remove_table_answer_value.py
--rw-r--r--   0        0        0      284 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0039_merge_20210114_0956.py
--rw-r--r--   0        0        0    10394 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0040_add_modified_by_user_group.py
--rw-r--r--   0        0        0     2150 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0041_action_button_question.py
--rw-r--r--   0        0        0      751 2022-06-20 07:44:55.259595 caluma-8.0.0b8/caluma/caluma_form/migrations/0042_auto_20220110_1051.py
--rw-r--r--   0        0        0     1210 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_form/migrations/0043_alter_historicalanswer_history_question_type.py
--rw-r--r--   0        0        0      991 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_form/migrations/0044_migrate_format_validators.py
--rw-r--r--   0        0        0     5739 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_form/migrations/0045_simple_history.py
--rw-r--r--   0        0        0        0 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_form/migrations/__init__.py
--rw-r--r--   0        0        0    20289 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_form/models.py
--rw-r--r--   0        0        0     2211 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_form/ordering.py
--rw-r--r--   0        0        0    36664 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_form/schema.py
--rw-r--r--   0        0        0    22614 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_form/serializers.py
--rw-r--r--   0        0        0     7337 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_form/signals.py
--rw-r--r--   0        0        0     3865 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_form/storage_clients.py
--rw-r--r--   0        0        0     7813 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_form/structure.py
--rw-r--r--   0        0        0    17441 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_form/validators.py
--rw-r--r--   0        0        0        0 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_logging/__init__.py
--rw-r--r--   0        0        0      103 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_logging/apps.py
--rw-r--r--   0        0        0      365 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_logging/factories.py
--rw-r--r--   0        0        0        0 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_logging/management/__init__.py
--rw-r--r--   0        0        0        0 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_logging/management/commands/__init__.py
--rw-r--r--   0        0        0     1087 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_logging/management/commands/cleanup_access_log.py
--rw-r--r--   0        0        0     1777 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_logging/middleware.py
--rw-r--r--   0        0        0     1560 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_logging/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_logging/migrations/__init__.py
--rw-r--r--   0        0        0      657 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_logging/models.py
--rw-r--r--   0        0        0        0 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_user/__init__.py
--rw-r--r--   0        0        0      100 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_user/apps.py
--rw-r--r--   0        0        0     1919 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_user/models.py
--rw-r--r--   0        0        0      506 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_user/permissions.py
--rw-r--r--   0        0        0     5012 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_user/views.py
--rw-r--r--   0        0        0      711 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_user/visibilities.py
--rw-r--r--   0        0        0        0 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_workflow/__init__.py
--rw-r--r--   0        0        0     7790 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_workflow/api.py
--rw-r--r--   0        0        0      618 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_workflow/apps.py
--rw-r--r--   0        0        0    20608 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_workflow/domain_logic.py
--rw-r--r--   0        0        0     1606 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_workflow/dynamic_groups.py
--rw-r--r--   0        0        0     1941 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_workflow/dynamic_tasks.py
--rw-r--r--   0        0        0      534 2022-06-20 07:44:55.263594 caluma-8.0.0b8/caluma/caluma_workflow/events.py
--rw-r--r--   0        0        0     2674 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/factories.py
--rw-r--r--   0        0        0     6090 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/filters.py
--rw-r--r--   0        0        0     6485 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/jexl.py
--rw-r--r--   0        0        0    11030 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0001_initial.py
--rw-r--r--   0        0        0      666 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0002_auto_20181213_1334.py
--rw-r--r--   0        0        0      756 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0003_auto_20181217_1051.py
--rw-r--r--   0        0        0     1632 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0004_auto_20181218_1352.py
--rw-r--r--   0        0        0     4269 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0005_auto_20181228_1243.py
--rw-r--r--   0        0        0      994 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0006_auto_20190121_1440.py
--rw-r--r--   0        0        0     1035 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0007_auto_20190206_0854.py
--rw-r--r--   0        0        0      687 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0008_auto_20190208_1302.py
--rw-r--r--   0        0        0     1621 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0009_auto_20190213_0939.py
--rw-r--r--   0        0        0      753 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0010_auto_20190213_1050.py
--rw-r--r--   0        0        0     1235 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0011_auto_20190220_1303.py
--rw-r--r--   0        0        0    21985 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0012_historicalcase_historicalflow_historicaltask_historicaltaskflow_historicalworkflow_historicalworkite.py
--rw-r--r--   0        0        0     3459 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0013_auto_20190718_1235.py
--rw-r--r--   0        0        0     1121 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0014_add_gin_index_to_jsonfields.py
--rw-r--r--   0        0        0     1299 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0015_add_work_item_skipped.py
--rw-r--r--   0        0        0     2220 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0016_auto_20200113_0727.py
--rw-r--r--   0        0        0     7594 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0017_auto_20200210_0929.py
--rw-r--r--   0        0        0      925 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0018_auto_20200219_1359.py
--rw-r--r--   0        0        0      925 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0019_slugfield_length.py
--rw-r--r--   0        0        0     2851 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0020_case_families.py
--rw-r--r--   0        0        0     1742 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0021_work_item_controlling_groups.py
--rw-r--r--   0        0        0     2504 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0022_workitem_name_description.py
--rw-r--r--   0        0        0     1064 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0023_auto_20200730_1135.py
--rw-r--r--   0        0        0     2491 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0024_auto_20200901_1026.py
--rw-r--r--   0        0        0     1453 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0025_auto_20200901_1415.py
--rw-r--r--   0        0        0     1337 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0026_auto_20200901_1435.py
--rw-r--r--   0        0        0     6416 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0027_add_modified_by_user_group.py
--rw-r--r--   0        0        0     2619 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0028_redoable_field.py
--rw-r--r--   0        0        0      854 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0029_task_continue_async.py
--rw-r--r--   0        0        0     3681 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0030_remove_choices_char_field.py
--rw-r--r--   0        0        0     3475 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/0031_simple_history.py
--rw-r--r--   0        0        0        0 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/migrations/__init__.py
--rw-r--r--   0        0        0     9946 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/models.py
--rw-r--r--   0        0        0    12372 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/schema.py
--rw-r--r--   0        0        0    21121 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/serializers.py
--rw-r--r--   0        0        0     4155 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/utils.py
--rw-r--r--   0        0        0     1202 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/validators.py
--rw-r--r--   0        0        0     2120 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/caluma_workflow/visibilities.py
--rw-r--r--   0        0        0    12222 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/conftest.py
--rw-r--r--   0        0        0        0 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/extensions/__init__.py
--rw-r--r--   0        0        0       53 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/extensions/data_sources.py
--rw-r--r--   0        0        0       39 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/extensions/dynamic_groups.py
--rw-r--r--   0        0        0       40 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/extensions/events.py
--rw-r--r--   0        0        0       58 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/extensions/format_validators.py
--rw-r--r--   0        0        0       52 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/extensions/permissions.py
--rw-r--r--   0        0        0       52 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/extensions/validations.py
--rw-r--r--   0        0        0       52 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/extensions/visibilities.py
--rw-r--r--   0        0        0     2782 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/schema.py
--rw-r--r--   0        0        0        0 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/settings/__init__.py
--rw-r--r--   0        0        0     3609 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/settings/caluma.py
--rw-r--r--   0        0        0     5752 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/settings/django.py
--rw-r--r--   0        0        0      100 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/urls.py
--rw-r--r--   0        0        0     3416 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/utils.py
--rw-r--r--   0        0        0      403 2022-06-20 07:44:55.267594 caluma-8.0.0b8/caluma/wsgi.py
--rw-r--r--   0        0        0     3542 2022-06-20 07:44:55.271594 caluma-8.0.0b8/pyproject.toml
--rw-r--r--   0        0        0     3945 2022-06-20 07:45:12.885155 caluma-8.0.0b8/setup.py
--rw-r--r--   0        0        0     3736 2022-06-20 07:45:12.885563 caluma-8.0.0b8/PKG-INFO
+-rw-r--r--   0        0        0    44302 2022-06-24 12:42:38.651433 caluma-8.0.0b9/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2022-06-24 12:42:38.651433 caluma-8.0.0b9/LICENSE
+drwxr-xr-x   0        0        0        0 2022-06-24 12:42:38.651433 caluma-8.0.0b9/LICENSES/
+-rw-r--r--   0        0        0     1957 2022-06-24 12:42:38.651433 caluma-8.0.0b9/README.md
+-rw-r--r--   0        0        0        0 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/__init__.py
+-rw-r--r--   0        0        0     5442 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/README.md
+-rw-r--r--   0        0        0        0 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/__init__.py
+-rw-r--r--   0        0        0      105 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/apps.py
+-rw-r--r--   0        0        0     3322 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/conftest.py
+-rw-r--r--   0        0        0      797 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/factories.py
+-rw-r--r--   0        0        0     1543 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/filters.py
+-rw-r--r--   0        0        0     3416 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/management/commands/run_analytics.py
+-rw-r--r--   0        0        0    11086 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2008 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/migrations/0002_analytics_pivot_table.py
+-rw-r--r--   0        0        0     1026 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/migrations/0003_starting_objects.py
+-rw-r--r--   0        0        0     1383 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/migrations/0004_simple_history.py
+-rw-r--r--   0        0        0        0 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/migrations/__init__.py
+-rw-r--r--   0        0        0     3469 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/models.py
+-rw-r--r--   0        0        0     3666 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/pivot_table.py
+-rw-r--r--   0        0        0     6996 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/schema.py
+-rw-r--r--   0        0        0     3499 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/serializers.py
+-rw-r--r--   0        0        0    32474 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/simple_table.py
+-rw-r--r--   0        0        0    16037 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/sql.py
+-rw-r--r--   0        0        0     1113 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_analytics/visibility.py
+-rw-r--r--   0        0        0        0 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/__init__.py
+-rw-r--r--   0        0        0      975 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/apps.py
+-rw-r--r--   0        0        0      195 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/collections.py
+-rw-r--r--   0        0        0    11297 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/conftest.py
+-rw-r--r--   0        0        0     3074 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/events.py
+-rw-r--r--   0        0        0      325 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/factories.py
+-rw-r--r--   0        0        0      485 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/faker.py
+-rw-r--r--   0        0        0    18433 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/filters.py
+-rw-r--r--   0        0        0      642 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/forms.py
+-rw-r--r--   0        0        0     4176 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/health_checks.py
+-rw-r--r--   0        0        0     7855 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/jexl.py
+-rw-r--r--   0        0        0        0 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/management/commands/__init__.py
+-rw-r--r--   0        0        0     1824 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/management/commands/cleanup_history.py
+-rw-r--r--   0        0        0     3803 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/management/commands/dump_caluma_config.py
+-rw-r--r--   0        0        0      794 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/management/commands/migrate.py
+-rw-r--r--   0        0        0     4768 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/management/commands/migrate_to_prefixed_apps.py
+-rw-r--r--   0        0        0     3078 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/models.py
+-rw-r--r--   0        0        0    11206 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/mutation.py
+-rw-r--r--   0        0        0     3216 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/ordering.py
+-rw-r--r--   0        0        0     3195 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/pagination.py
+-rw-r--r--   0        0        0     4485 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/permissions.py
+-rw-r--r--   0        0        0     1253 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/relay.py
+-rw-r--r--   0        0        0     4764 2022-06-24 12:42:38.651433 caluma-8.0.0b9/caluma/caluma_core/serializers.py
+-rw-r--r--   0        0        0     7577 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_core/types.py
+-rw-r--r--   0        0        0      387 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_core/urls.py
+-rw-r--r--   0        0        0     2430 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_core/validations.py
+-rw-r--r--   0        0        0     1607 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_core/views.py
+-rw-r--r--   0        0        0     2937 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_core/visibilities.py
+-rw-r--r--   0        0        0        0 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_data_source/__init__.py
+-rw-r--r--   0        0        0      107 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_data_source/apps.py
+-rw-r--r--   0        0        0     2028 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_data_source/data_source_handlers.py
+-rw-r--r--   0        0        0     3104 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_data_source/data_sources.py
+-rw-r--r--   0        0        0      989 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_data_source/schema.py
+-rw-r--r--   0        0        0      486 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_data_source/utils.py
+-rw-r--r--   0        0        0        0 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/__init__.py
+-rw-r--r--   0        0        0     2472 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/api.py
+-rw-r--r--   0        0        0      100 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/apps.py
+-rw-r--r--   0        0        0     8317 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/domain_logic.py
+-rw-r--r--   0        0        0     5702 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/factories.py
+-rw-r--r--   0        0        0    16457 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/filters.py
+-rw-r--r--   0        0        0     3283 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/format_validators.py
+-rw-r--r--   0        0        0     7860 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/historical_schema.py
+-rw-r--r--   0        0        0     7496 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/jexl.py
+-rw-r--r--   0        0        0        0 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/management/commands/__init__.py
+-rw-r--r--   0        0        0     1880 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/management/commands/copy_form.py
+-rw-r--r--   0        0        0      631 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/management/commands/create_bucket.py
+-rw-r--r--   0        0        0    10984 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2830 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0002_auto_20181221_1517.py
+-rw-r--r--   0        0        0     3863 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0003_auto_20190130_0920.py
+-rw-r--r--   0        0        0     1566 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0004_auto_20190207_1405.py
+-rw-r--r--   0        0        0      826 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0005_auto_20190208_1016.py
+-rw-r--r--   0        0        0      801 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0006_choice_type_conversion.py
+-rw-r--r--   0        0        0      630 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0007_auto_20190208_1232.py
+-rw-r--r--   0        0        0     1180 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0008_auto_20190319_1720.py
+-rw-r--r--   0        0        0     2134 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0009_auto_20190321_1722.py
+-rw-r--r--   0        0        0     2303 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0010_auto_20190404_0652.py
+-rw-r--r--   0        0        0      605 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0011_auto_20190411_0607.py
+-rw-r--r--   0        0        0      789 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0012_auto_20190416_1835.py
+-rw-r--r--   0        0        0     1257 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0013_auto_20190418_0733.py
+-rw-r--r--   0        0        0     1408 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0014_auto_20190429_0910.py
+-rw-r--r--   0        0        0      660 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0015_question_format_validators.py
+-rw-r--r--   0        0        0      531 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0016_auto_20190510_0843.py
+-rw-r--r--   0        0        0      606 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0017_auto_20190619_1320.py
+-rw-r--r--   0        0        0     1860 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0018_remove_answer_value_document_data_migration.py
+-rw-r--r--   0        0        0      366 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0019_remove_answer_value_document.py
+-rw-r--r--   0        0        0    27840 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0020_historicalanswer_historicalanswerdocument_historicaldocument_historicalfile_historicalform_historica.py
+-rw-r--r--   0        0        0     2471 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0021_auto_20190708_0905.py
+-rw-r--r--   0        0        0     1454 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0022_add_gin_index_to_jsonfields.py
+-rw-r--r--   0        0        0      559 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0023_auto_20190729_1448.py
+-rw-r--r--   0        0        0     1088 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0024_auto_20190919_1244.py
+-rw-r--r--   0        0        0     4835 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0025_dynamicoption_historicaldynamicoption.py
+-rw-r--r--   0        0        0      829 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0026_auto_20191031_0834.py
+-rw-r--r--   0        0        0     2088 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0027_auto_20200113_0727.py
+-rw-r--r--   0        0        0    12676 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0028_auto_20200210_0929.py
+-rw-r--r--   0        0        0     1571 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0029_dynamic_option_unique_together.py
+-rw-r--r--   0        0        0     1282 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0030_auto_20200219_1359.py
+-rw-r--r--   0        0        0     1702 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0031_auto_20200220_0910.py
+-rw-r--r--   0        0        0     1154 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0032_auto_20200220_1311.py
+-rw-r--r--   0        0        0     1270 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0033_slugfield_length.py
+-rw-r--r--   0        0        0      520 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0034_fix_fk_lengths.py
+-rw-r--r--   0        0        0     1688 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0035_historicalanswer_history_question_type.py
+-rw-r--r--   0        0        0     1387 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0036_default_answers.py
+-rw-r--r--   0        0        0      611 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0037_default_answer_one2one.py
+-rw-r--r--   0        0        0     3051 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0038_auto_20201224_0920.py
+-rw-r--r--   0        0        0      461 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0038_remove_table_answer_value.py
+-rw-r--r--   0        0        0      284 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0039_merge_20210114_0956.py
+-rw-r--r--   0        0        0    10394 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0040_add_modified_by_user_group.py
+-rw-r--r--   0        0        0     2150 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0041_action_button_question.py
+-rw-r--r--   0        0        0      751 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0042_auto_20220110_1051.py
+-rw-r--r--   0        0        0     1210 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0043_alter_historicalanswer_history_question_type.py
+-rw-r--r--   0        0        0      991 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0044_migrate_format_validators.py
+-rw-r--r--   0        0        0     5739 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/0045_simple_history.py
+-rw-r--r--   0        0        0        0 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/migrations/__init__.py
+-rw-r--r--   0        0        0    21045 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/models.py
+-rw-r--r--   0        0        0     2211 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/ordering.py
+-rw-r--r--   0        0        0    36664 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/schema.py
+-rw-r--r--   0        0        0    22614 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/serializers.py
+-rw-r--r--   0        0        0     7337 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/signals.py
+-rw-r--r--   0        0        0     3865 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/storage_clients.py
+-rw-r--r--   0        0        0     7813 2022-06-24 12:42:38.655433 caluma-8.0.0b9/caluma/caluma_form/structure.py
+-rw-r--r--   0        0        0    17803 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_form/validators.py
+-rw-r--r--   0        0        0        0 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_logging/__init__.py
+-rw-r--r--   0        0        0      103 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_logging/apps.py
+-rw-r--r--   0        0        0      365 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_logging/factories.py
+-rw-r--r--   0        0        0        0 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_logging/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_logging/management/commands/__init__.py
+-rw-r--r--   0        0        0     1087 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_logging/management/commands/cleanup_access_log.py
+-rw-r--r--   0        0        0     1777 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_logging/middleware.py
+-rw-r--r--   0        0        0     1560 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_logging/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_logging/migrations/__init__.py
+-rw-r--r--   0        0        0      657 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_logging/models.py
+-rw-r--r--   0        0        0        0 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_user/__init__.py
+-rw-r--r--   0        0        0      100 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_user/apps.py
+-rw-r--r--   0        0        0     1919 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_user/models.py
+-rw-r--r--   0        0        0      506 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_user/permissions.py
+-rw-r--r--   0        0        0     5012 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_user/views.py
+-rw-r--r--   0        0        0      711 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_user/visibilities.py
+-rw-r--r--   0        0        0        0 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/__init__.py
+-rw-r--r--   0        0        0     7790 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/api.py
+-rw-r--r--   0        0        0      618 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/apps.py
+-rw-r--r--   0        0        0    20682 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/domain_logic.py
+-rw-r--r--   0        0        0     1606 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/dynamic_groups.py
+-rw-r--r--   0        0        0     1941 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/dynamic_tasks.py
+-rw-r--r--   0        0        0      534 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/events.py
+-rw-r--r--   0        0        0     2674 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/factories.py
+-rw-r--r--   0        0        0     6090 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/filters.py
+-rw-r--r--   0        0        0     6485 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/jexl.py
+-rw-r--r--   0        0        0    11030 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0001_initial.py
+-rw-r--r--   0        0        0      666 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0002_auto_20181213_1334.py
+-rw-r--r--   0        0        0      756 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0003_auto_20181217_1051.py
+-rw-r--r--   0        0        0     1632 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0004_auto_20181218_1352.py
+-rw-r--r--   0        0        0     4269 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0005_auto_20181228_1243.py
+-rw-r--r--   0        0        0      994 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0006_auto_20190121_1440.py
+-rw-r--r--   0        0        0     1035 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0007_auto_20190206_0854.py
+-rw-r--r--   0        0        0      687 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0008_auto_20190208_1302.py
+-rw-r--r--   0        0        0     1621 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0009_auto_20190213_0939.py
+-rw-r--r--   0        0        0      753 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0010_auto_20190213_1050.py
+-rw-r--r--   0        0        0     1235 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0011_auto_20190220_1303.py
+-rw-r--r--   0        0        0    21985 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0012_historicalcase_historicalflow_historicaltask_historicaltaskflow_historicalworkflow_historicalworkite.py
+-rw-r--r--   0        0        0     3459 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0013_auto_20190718_1235.py
+-rw-r--r--   0        0        0     1121 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0014_add_gin_index_to_jsonfields.py
+-rw-r--r--   0        0        0     1299 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0015_add_work_item_skipped.py
+-rw-r--r--   0        0        0     2220 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0016_auto_20200113_0727.py
+-rw-r--r--   0        0        0     7594 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0017_auto_20200210_0929.py
+-rw-r--r--   0        0        0      925 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0018_auto_20200219_1359.py
+-rw-r--r--   0        0        0      925 2022-06-24 12:42:38.659433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0019_slugfield_length.py
+-rw-r--r--   0        0        0     2851 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0020_case_families.py
+-rw-r--r--   0        0        0     1742 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0021_work_item_controlling_groups.py
+-rw-r--r--   0        0        0     2504 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0022_workitem_name_description.py
+-rw-r--r--   0        0        0     1064 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0023_auto_20200730_1135.py
+-rw-r--r--   0        0        0     2491 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0024_auto_20200901_1026.py
+-rw-r--r--   0        0        0     1453 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0025_auto_20200901_1415.py
+-rw-r--r--   0        0        0     1337 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0026_auto_20200901_1435.py
+-rw-r--r--   0        0        0     6416 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0027_add_modified_by_user_group.py
+-rw-r--r--   0        0        0     2619 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0028_redoable_field.py
+-rw-r--r--   0        0        0      854 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0029_task_continue_async.py
+-rw-r--r--   0        0        0     3681 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0030_remove_choices_char_field.py
+-rw-r--r--   0        0        0     3475 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/0031_simple_history.py
+-rw-r--r--   0        0        0        0 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/migrations/__init__.py
+-rw-r--r--   0        0        0     9946 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/models.py
+-rw-r--r--   0        0        0    12372 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/schema.py
+-rw-r--r--   0        0        0    21121 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/serializers.py
+-rw-r--r--   0        0        0     4155 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/utils.py
+-rw-r--r--   0        0        0     1202 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/validators.py
+-rw-r--r--   0        0        0     2120 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/caluma_workflow/visibilities.py
+-rw-r--r--   0        0        0    12222 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/conftest.py
+-rw-r--r--   0        0        0        0 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/extensions/__init__.py
+-rw-r--r--   0        0        0       53 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/extensions/data_sources.py
+-rw-r--r--   0        0        0       39 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/extensions/dynamic_groups.py
+-rw-r--r--   0        0        0       40 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/extensions/events.py
+-rw-r--r--   0        0        0       58 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/extensions/format_validators.py
+-rw-r--r--   0        0        0       52 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/extensions/permissions.py
+-rw-r--r--   0        0        0       52 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/extensions/validations.py
+-rw-r--r--   0        0        0       52 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/extensions/visibilities.py
+-rw-r--r--   0        0        0     2782 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/schema.py
+-rw-r--r--   0        0        0        0 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/settings/__init__.py
+-rw-r--r--   0        0        0     3609 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/settings/caluma.py
+-rw-r--r--   0        0        0     5752 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/settings/django.py
+-rw-r--r--   0        0        0      100 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/urls.py
+-rw-r--r--   0        0        0     3416 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/utils.py
+-rw-r--r--   0        0        0      403 2022-06-24 12:42:38.663433 caluma-8.0.0b9/caluma/wsgi.py
+-rw-r--r--   0        0        0     3542 2022-06-24 12:42:38.663433 caluma-8.0.0b9/pyproject.toml
+-rw-r--r--   0        0        0     3945 2022-06-24 12:42:56.699962 caluma-8.0.0b9/setup.py
+-rw-r--r--   0        0        0     3736 2022-06-24 12:42:56.700354 caluma-8.0.0b9/PKG-INFO
```

### Comparing `caluma-8.0.0b8/CHANGELOG.md` & `caluma-8.0.0b9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+# v8.0.0-beta.9 (24 June 2022)
+
+### Fix
+* **document:** Copy dynamic options when copying documents ([`67910d9`](https://github.com/projectcaluma/caluma/commit/67910d96b98721be9953920ca23bddc33f4521ea))
+* ReopenCase should disregard WorkItems in status REDO ([`dded3a8`](https://github.com/projectcaluma/caluma/commit/dded3a8b1f54b4efcb4c654966dc2234d9909ddb))
+* **deps:** Update dependencies of dependencies ([`e3a5de3`](https://github.com/projectcaluma/caluma/commit/e3a5de38c3a9b1d1456e9fbee6f108913dc7b6df))
+* **form:** Set questions of searchAnswers as required ([`fb7ad5f`](https://github.com/projectcaluma/caluma/commit/fb7ad5feb120abeaf3ea45670fa5349c86eb8464))
+
+### Breaking
+* searchAnswers questions list is now required  ([`fb7ad5f`](https://github.com/projectcalum/caluma/commit/fb7ad5feb120abeaf3ea45670fa5349c86eb8464))
+
+
 # v8.0.0-beta.8 (20 June 2022)
 
 ### Fix
 * **default answer:** Don't set document when copying default answers ([`7b5ce74`](https://github.com/projectcaluma/caluma/commit/7b5ce74a8a62a8b0415226eb784cc8aae811f9c3))
 
 
 # v8.0.0-beta.7 (9 June 2022)
```

### Comparing `caluma-8.0.0b8/LICENSE` & `caluma-8.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/README.md` & `caluma-8.0.0b9/README.md`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_analytics/README.md` & `caluma-8.0.0b9/caluma/caluma_analytics/README.md`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_analytics/conftest.py` & `caluma-8.0.0b9/caluma/caluma_analytics/conftest.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_analytics/factories.py` & `caluma-8.0.0b9/caluma/caluma_analytics/factories.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_analytics/filters.py` & `caluma-8.0.0b9/caluma/caluma_analytics/filters.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_analytics/management/commands/run_analytics.py` & `caluma-8.0.0b9/caluma/caluma_analytics/management/commands/run_analytics.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_analytics/migrations/0001_initial.py` & `caluma-8.0.0b9/caluma/caluma_analytics/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_analytics/migrations/0002_analytics_pivot_table.py` & `caluma-8.0.0b9/caluma/caluma_analytics/migrations/0002_analytics_pivot_table.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_analytics/migrations/0003_starting_objects.py` & `caluma-8.0.0b9/caluma/caluma_analytics/migrations/0003_starting_objects.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_analytics/migrations/0004_simple_history.py` & `caluma-8.0.0b9/caluma/caluma_analytics/migrations/0004_simple_history.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_analytics/models.py` & `caluma-8.0.0b9/caluma/caluma_analytics/models.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_analytics/pivot_table.py` & `caluma-8.0.0b9/caluma/caluma_analytics/pivot_table.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_analytics/schema.py` & `caluma-8.0.0b9/caluma/caluma_analytics/schema.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_analytics/serializers.py` & `caluma-8.0.0b9/caluma/caluma_analytics/serializers.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_analytics/simple_table.py` & `caluma-8.0.0b9/caluma/caluma_analytics/simple_table.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_analytics/sql.py` & `caluma-8.0.0b9/caluma/caluma_analytics/sql.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_analytics/visibility.py` & `caluma-8.0.0b9/caluma/caluma_analytics/visibility.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_core/apps.py` & `caluma-8.0.0b9/caluma/caluma_core/apps.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_core/conftest.py` & `caluma-8.0.0b9/caluma/caluma_core/conftest.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_core/events.py` & `caluma-8.0.0b9/caluma/caluma_core/events.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_core/filters.py` & `caluma-8.0.0b9/caluma/caluma_core/filters.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_core/forms.py` & `caluma-8.0.0b9/caluma/caluma_core/forms.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_core/health_checks.py` & `caluma-8.0.0b9/caluma/caluma_core/health_checks.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_core/jexl.py` & `caluma-8.0.0b9/caluma/caluma_core/jexl.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_core/management/commands/cleanup_history.py` & `caluma-8.0.0b9/caluma/caluma_core/management/commands/cleanup_history.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_core/management/commands/dump_caluma_config.py` & `caluma-8.0.0b9/caluma/caluma_core/management/commands/dump_caluma_config.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_core/management/commands/migrate.py` & `caluma-8.0.0b9/caluma/caluma_core/management/commands/migrate.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_core/management/commands/migrate_to_prefixed_apps.py` & `caluma-8.0.0b9/caluma/caluma_core/management/commands/migrate_to_prefixed_apps.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_core/models.py` & `caluma-8.0.0b9/caluma/caluma_core/models.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_core/mutation.py` & `caluma-8.0.0b9/caluma/caluma_core/mutation.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_core/ordering.py` & `caluma-8.0.0b9/caluma/caluma_core/ordering.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_core/pagination.py` & `caluma-8.0.0b9/caluma/caluma_core/pagination.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_core/permissions.py` & `caluma-8.0.0b9/caluma/caluma_core/permissions.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_core/relay.py` & `caluma-8.0.0b9/caluma/caluma_core/relay.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_core/serializers.py` & `caluma-8.0.0b9/caluma/caluma_core/serializers.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_core/types.py` & `caluma-8.0.0b9/caluma/caluma_core/types.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_core/validations.py` & `caluma-8.0.0b9/caluma/caluma_core/validations.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_core/views.py` & `caluma-8.0.0b9/caluma/caluma_core/views.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_core/visibilities.py` & `caluma-8.0.0b9/caluma/caluma_core/visibilities.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_data_source/data_source_handlers.py` & `caluma-8.0.0b9/caluma/caluma_data_source/data_source_handlers.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_data_source/data_sources.py` & `caluma-8.0.0b9/caluma/caluma_data_source/data_sources.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_data_source/schema.py` & `caluma-8.0.0b9/caluma/caluma_data_source/schema.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/api.py` & `caluma-8.0.0b9/caluma/caluma_form/api.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/domain_logic.py` & `caluma-8.0.0b9/caluma/caluma_form/domain_logic.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/factories.py` & `caluma-8.0.0b9/caluma/caluma_form/factories.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/filters.py` & `caluma-8.0.0b9/caluma/caluma_form/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,15 +295,15 @@
     CONTAINS = "icontains"
     TEXT = "search"
 
 
 class SearchAnswersFilterType(InputObjectType):
     """Lookup type to search in answers."""
 
-    questions = List(graphene.ID)
+    questions = List(graphene.ID, required=True)
     value = graphene.types.generic.GenericScalar(required=True)
     lookup = SearchLookupMode(required=False)
 
 
 class SearchAnswersFilterField(CompositeFieldClass):
     pass
```

### Comparing `caluma-8.0.0b8/caluma/caluma_form/format_validators.py` & `caluma-8.0.0b9/caluma/caluma_form/format_validators.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/historical_schema.py` & `caluma-8.0.0b9/caluma/caluma_form/historical_schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from graphene import relay
 from graphene.types import ObjectType, generic
 
 from ..caluma_core.relay import extract_global_id
 from ..caluma_core.types import ConnectionField, CountableConnectionBase
 from . import models
 from .schema import (
-    QUESTION_ANSWER_TYPES,
     Answer,
     DateAnswer,
     FileAnswer,
     FloatAnswer,
     FormDjangoObjectType,
     IntegerAnswer,
     ListAnswer,
@@ -41,16 +40,15 @@
 class HistoricalAnswer(Answer):
     history_date = graphene.types.datetime.DateTime(required=True)
     history_user_id = graphene.String()
     history_type = graphene.String()
 
     @classmethod
     def resolve_type(cls, instance, info):
-        answer_type = QUESTION_ANSWER_TYPES[instance.history_question_type]
-        return f"Historical{answer_type.__name__}"
+        return HISTORICAL_ANSWER_TYPES[instance.history_question_type]
 
 
 class HistoricalAnswerConnection(CountableConnectionBase):
     class Meta:
         node = HistoricalAnswer
 
 
@@ -217,7 +215,23 @@
         HistoricalDocument,
         id=graphene.ID(required=True),
         as_of=graphene.types.datetime.DateTime(required=True),
     )
 
     def resolve_document_as_of(self, info, id, as_of):
         return document_as_of(info, id, as_of)
+
+
+HISTORICAL_ANSWER_TYPES = {
+    models.Question.TYPE_MULTIPLE_CHOICE: HistoricalListAnswer,
+    models.Question.TYPE_INTEGER: HistoricalIntegerAnswer,
+    models.Question.TYPE_FLOAT: HistoricalFloatAnswer,
+    models.Question.TYPE_DATE: HistoricalDateAnswer,
+    models.Question.TYPE_CHOICE: HistoricalStringAnswer,
+    models.Question.TYPE_TEXTAREA: HistoricalStringAnswer,
+    models.Question.TYPE_TEXT: HistoricalStringAnswer,
+    models.Question.TYPE_TABLE: HistoricalTableAnswer,
+    models.Question.TYPE_FILE: HistoricalFileAnswer,
+    models.Question.TYPE_DYNAMIC_CHOICE: HistoricalStringAnswer,
+    models.Question.TYPE_DYNAMIC_MULTIPLE_CHOICE: HistoricalListAnswer,
+    models.Question.TYPE_CALCULATED_FLOAT: HistoricalFloatAnswer,
+}
```

### Comparing `caluma-8.0.0b8/caluma/caluma_form/jexl.py` & `caluma-8.0.0b9/caluma/caluma_form/jexl.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/management/commands/copy_form.py` & `caluma-8.0.0b9/caluma/caluma_form/management/commands/copy_form.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/management/commands/create_bucket.py` & `caluma-8.0.0b9/caluma/caluma_form/management/commands/create_bucket.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0001_initial.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0002_auto_20181221_1517.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0002_auto_20181221_1517.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0003_auto_20190130_0920.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0003_auto_20190130_0920.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0004_auto_20190207_1405.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0004_auto_20190207_1405.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0005_auto_20190208_1016.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0005_auto_20190208_1016.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0006_choice_type_conversion.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0006_choice_type_conversion.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0007_auto_20190208_1232.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0007_auto_20190208_1232.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0008_auto_20190319_1720.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0008_auto_20190319_1720.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0009_auto_20190321_1722.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0009_auto_20190321_1722.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0010_auto_20190404_0652.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0010_auto_20190404_0652.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0011_auto_20190411_0607.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0011_auto_20190411_0607.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0012_auto_20190416_1835.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0012_auto_20190416_1835.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0013_auto_20190418_0733.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0013_auto_20190418_0733.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0014_auto_20190429_0910.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0014_auto_20190429_0910.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0015_question_format_validators.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0015_question_format_validators.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0016_auto_20190510_0843.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0016_auto_20190510_0843.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0017_auto_20190619_1320.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0017_auto_20190619_1320.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0018_remove_answer_value_document_data_migration.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0018_remove_answer_value_document_data_migration.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0020_historicalanswer_historicalanswerdocument_historicaldocument_historicalfile_historicalform_historica.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0020_historicalanswer_historicalanswerdocument_historicaldocument_historicalfile_historicalform_historica.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0021_auto_20190708_0905.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0021_auto_20190708_0905.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0022_add_gin_index_to_jsonfields.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0022_add_gin_index_to_jsonfields.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0023_auto_20190729_1448.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0023_auto_20190729_1448.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0024_auto_20190919_1244.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0024_auto_20190919_1244.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0025_dynamicoption_historicaldynamicoption.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0025_dynamicoption_historicaldynamicoption.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0026_auto_20191031_0834.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0026_auto_20191031_0834.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0027_auto_20200113_0727.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0027_auto_20200113_0727.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0028_auto_20200210_0929.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0028_auto_20200210_0929.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0029_dynamic_option_unique_together.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0029_dynamic_option_unique_together.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0030_auto_20200219_1359.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0030_auto_20200219_1359.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0031_auto_20200220_0910.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0031_auto_20200220_0910.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0032_auto_20200220_1311.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0032_auto_20200220_1311.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0033_slugfield_length.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0033_slugfield_length.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0034_fix_fk_lengths.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0034_fix_fk_lengths.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0035_historicalanswer_history_question_type.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0035_historicalanswer_history_question_type.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0036_default_answers.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0036_default_answers.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0037_default_answer_one2one.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0037_default_answer_one2one.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0038_auto_20201224_0920.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0038_auto_20201224_0920.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0040_add_modified_by_user_group.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0040_add_modified_by_user_group.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0041_action_button_question.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0041_action_button_question.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0042_auto_20220110_1051.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0042_auto_20220110_1051.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0043_alter_historicalanswer_history_question_type.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0043_alter_historicalanswer_history_question_type.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0044_migrate_format_validators.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0044_migrate_format_validators.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/migrations/0045_simple_history.py` & `caluma-8.0.0b9/caluma/caluma_form/migrations/0045_simple_history.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/models.py` & `caluma-8.0.0b9/caluma/caluma_form/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -465,14 +465,32 @@
             },
         )
 
         if self.question.type == Question.TYPE_FILE:
             new_answer.file = self.file.copy()
             new_answer.save()
 
+        if self.question.type in [
+            Question.TYPE_DYNAMIC_CHOICE,
+            Question.TYPE_DYNAMIC_MULTIPLE_CHOICE,
+        ]:
+            for dynamic_option in DynamicOption.objects.filter(
+                document=self.document, question=self.question
+            ):
+                DynamicOption.objects.update_or_create(
+                    document=to_document,
+                    question=dynamic_option.question,
+                    slug=dynamic_option.slug,
+                    defaults={
+                        "label": dynamic_option.slug,
+                        "created_by_user": user.username if user else None,
+                        "created_by_group": user.group if user else None,
+                    },
+                )
+
         # TableAnswer: copy AnswerDocument too
         for answer_doc in AnswerDocument.objects.filter(answer=self):
             new_doc = answer_doc.document.copy(family=document_family, user=user)
 
             AnswerDocument.objects.create(
                 answer=new_answer,
                 document=new_doc,
```

### Comparing `caluma-8.0.0b8/caluma/caluma_form/ordering.py` & `caluma-8.0.0b9/caluma/caluma_form/ordering.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/schema.py` & `caluma-8.0.0b9/caluma/caluma_form/schema.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/serializers.py` & `caluma-8.0.0b9/caluma/caluma_form/serializers.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/signals.py` & `caluma-8.0.0b9/caluma/caluma_form/signals.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/storage_clients.py` & `caluma-8.0.0b9/caluma/caluma_form/storage_clients.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/structure.py` & `caluma-8.0.0b9/caluma/caluma_form/structure.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_form/validators.py` & `caluma-8.0.0b9/caluma/caluma_form/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,35 @@
     def _validate_question_dynamic_choice(
         self, question, value, document, user, **kwargs
     ):
         if not isinstance(value, str):
             raise CustomValidationError(
                 f'Invalid value "{value}". Must be of type str.', slugs=[question.slug]
             )
+
         self._validate_dynamic_option(question, document, value, user)
+        self._remove_unused_dynamic_options(question, document, [value])
+
+    def _validate_question_dynamic_multiple_choice(
+        self, question, value, document, user, **kwargs
+    ):
+        if not isinstance(value, list):
+            raise CustomValidationError(
+                f'Invalid value: "{value}". Must be of type list', slugs=[question.slug]
+            )
+
+        for v in value:
+            if not isinstance(v, str):
+                raise CustomValidationError(
+                    f'Invalid value: "{v}". Must be of type string',
+                    slugs=[question.slug],
+                )
+            self._validate_dynamic_option(question, document, v, user)
+
+        self._remove_unused_dynamic_options(question, document, value)
 
     def _validate_dynamic_option(self, question, document, option, user):
         data_source = get_data_sources(dic=True)[question.data_source]
         data_source_object = data_source()
 
         valid_label = data_source_object.validate_answer_value(
             option, document, question, user
@@ -134,29 +154,18 @@
             defaults={
                 "label": valid_label,
                 "created_by_user": user.username,
                 "created_by_group": user.group,
             },
         )
 
-    def _validate_question_dynamic_multiple_choice(
-        self, question, value, document, user, **kwargs
-    ):
-        if not isinstance(value, list):
-            raise CustomValidationError(
-                f'Invalid value: "{value}". Must be of type list', slugs=[question.slug]
-            )
-
-        for v in value:
-            if not isinstance(v, str):
-                raise CustomValidationError(
-                    f'Invalid value: "{v}". Must be of type string',
-                    slugs=[question.slug],
-                )
-            self._validate_dynamic_option(question, document, v, user)
+    def _remove_unused_dynamic_options(self, question, document, used_values):
+        DynamicOption.objects.filter(document=document, question=question).exclude(
+            slug__in=used_values
+        ).delete()
 
     def _validate_question_table(
         self, question, value, document, user, instance=None, origin=False, **kwargs
     ):
         if not origin:
             for row_doc in value:
                 DocumentValidator().validate(row_doc, user=user, **kwargs)
```

### Comparing `caluma-8.0.0b8/caluma/caluma_logging/management/commands/cleanup_access_log.py` & `caluma-8.0.0b9/caluma/caluma_logging/management/commands/cleanup_access_log.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_logging/middleware.py` & `caluma-8.0.0b9/caluma/caluma_logging/middleware.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_logging/migrations/0001_initial.py` & `caluma-8.0.0b9/caluma/caluma_logging/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_logging/models.py` & `caluma-8.0.0b9/caluma/caluma_logging/models.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_user/models.py` & `caluma-8.0.0b9/caluma/caluma_user/models.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_user/views.py` & `caluma-8.0.0b9/caluma/caluma_user/views.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_user/visibilities.py` & `caluma-8.0.0b9/caluma/caluma_user/visibilities.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/api.py` & `caluma-8.0.0b9/caluma/caluma_workflow/api.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/apps.py` & `caluma-8.0.0b9/caluma/caluma_workflow/apps.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/domain_logic.py` & `caluma-8.0.0b9/caluma/caluma_workflow/domain_logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,15 +379,17 @@
         ]:
             raise ValidationError("Only completed and canceled cases can be reopened.")
 
         if not case.family == case:
             raise ValidationError("Child cases can not be reopened.")
 
         for work_item in work_items:
-            if work_item.succeeding_work_items.exists():
+            if work_item.succeeding_work_items.exclude(
+                status=models.WorkItem.STATUS_REDO
+            ).exists():
                 raise ValidationError(
                     "Only work items at the end of a branch can be reopened."
                 )
 
             if work_item.case != case:
                 raise ValidationError(
                     "Only work items belonging to the case specified can be reopend."
```

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/dynamic_groups.py` & `caluma-8.0.0b9/caluma/caluma_workflow/dynamic_groups.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/dynamic_tasks.py` & `caluma-8.0.0b9/caluma/caluma_workflow/dynamic_tasks.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/events.py` & `caluma-8.0.0b9/caluma/caluma_workflow/events.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/factories.py` & `caluma-8.0.0b9/caluma/caluma_workflow/factories.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/filters.py` & `caluma-8.0.0b9/caluma/caluma_workflow/filters.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/jexl.py` & `caluma-8.0.0b9/caluma/caluma_workflow/jexl.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0001_initial.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0002_auto_20181213_1334.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0002_auto_20181213_1334.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0003_auto_20181217_1051.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0003_auto_20181217_1051.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0004_auto_20181218_1352.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0004_auto_20181218_1352.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0005_auto_20181228_1243.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0005_auto_20181228_1243.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0006_auto_20190121_1440.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0006_auto_20190121_1440.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0007_auto_20190206_0854.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0007_auto_20190206_0854.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0008_auto_20190208_1302.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0008_auto_20190208_1302.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0009_auto_20190213_0939.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0009_auto_20190213_0939.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0010_auto_20190213_1050.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0010_auto_20190213_1050.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0011_auto_20190220_1303.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0011_auto_20190220_1303.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0012_historicalcase_historicalflow_historicaltask_historicaltaskflow_historicalworkflow_historicalworkite.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0012_historicalcase_historicalflow_historicaltask_historicaltaskflow_historicalworkflow_historicalworkite.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0013_auto_20190718_1235.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0013_auto_20190718_1235.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0014_add_gin_index_to_jsonfields.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0014_add_gin_index_to_jsonfields.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0015_add_work_item_skipped.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0015_add_work_item_skipped.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0016_auto_20200113_0727.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0016_auto_20200113_0727.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0017_auto_20200210_0929.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0017_auto_20200210_0929.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0018_auto_20200219_1359.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0018_auto_20200219_1359.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0019_slugfield_length.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0019_slugfield_length.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0020_case_families.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0020_case_families.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0021_work_item_controlling_groups.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0021_work_item_controlling_groups.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0022_workitem_name_description.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0022_workitem_name_description.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0023_auto_20200730_1135.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0023_auto_20200730_1135.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0024_auto_20200901_1026.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0024_auto_20200901_1026.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0025_auto_20200901_1415.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0025_auto_20200901_1415.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0026_auto_20200901_1435.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0026_auto_20200901_1435.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0027_add_modified_by_user_group.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0027_add_modified_by_user_group.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0028_redoable_field.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0028_redoable_field.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0029_task_continue_async.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0029_task_continue_async.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0030_remove_choices_char_field.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0030_remove_choices_char_field.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/migrations/0031_simple_history.py` & `caluma-8.0.0b9/caluma/caluma_workflow/migrations/0031_simple_history.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/models.py` & `caluma-8.0.0b9/caluma/caluma_workflow/models.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/schema.py` & `caluma-8.0.0b9/caluma/caluma_workflow/schema.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/serializers.py` & `caluma-8.0.0b9/caluma/caluma_workflow/serializers.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/utils.py` & `caluma-8.0.0b9/caluma/caluma_workflow/utils.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/validators.py` & `caluma-8.0.0b9/caluma/caluma_workflow/validators.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/caluma_workflow/visibilities.py` & `caluma-8.0.0b9/caluma/caluma_workflow/visibilities.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/conftest.py` & `caluma-8.0.0b9/caluma/conftest.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/schema.py` & `caluma-8.0.0b9/caluma/schema.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/settings/caluma.py` & `caluma-8.0.0b9/caluma/settings/caluma.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/settings/django.py` & `caluma-8.0.0b9/caluma/settings/django.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/caluma/utils.py` & `caluma-8.0.0b9/caluma/utils.py`

 * *Files identical despite different names*

### Comparing `caluma-8.0.0b8/pyproject.toml` & `caluma-8.0.0b9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "caluma"
-version = "8.0.0-beta.8"
+version = "8.0.0-beta.9"
 description = "Caluma Service providing GraphQL API"
 homepage = "https://caluma.io"
 repository = "https://github.com/projectcaluma/caluma"
 documentation = "https://caluma.gitbook.io/"
 authors = ["Caluma <info@caluma.io>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
@@ -43,17 +43,17 @@
 urllib3 = "^1.26.8"
 uWSGI = "^2.0.20"
 graphql-core = "~3.1.7"
 
 [tool.poetry.dev-dependencies]
 black = "22.3.0"
 factory-boy = "3.2.1"
-Faker = "13.13.0"
+Faker = "13.14.0"
 flake8 = "4.0.1"
-flake8-bugbear = "22.4.25"
+flake8-bugbear = "22.6.22"
 flake8-debugger = "4.1.2"
 flake8-docstrings = "1.6.0"
 flake8-isort = "4.1.1"
 flake8-string-format = "0.3.0"
 flake8-tuple = "0.4.1"
 gitlint = "0.17.0"
 isort = "5.10.1"
@@ -65,15 +65,15 @@
 pytest-django = "4.5.2"
 pytest-env = "0.6.2"
 pytest-factoryboy = "2.5.0"
 pytest-freezegun = "0.4.2"
 pytest-mock = "3.7.0"
 pytest-randomly = "3.12.0"
 pytest-xdist = "2.5.0"
-python-semantic-release = "7.29.1"
+python-semantic-release = "7.29.2"
 requests-mock = "1.9.3"
 reuse = "1.0.0"
 syrupy = "2.3.0"
 
 [tool.isort]
 skip = [
   "migrations",
```

### Comparing `caluma-8.0.0b8/setup.py` & `caluma-8.0.0b9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
  'python-memcached>=1.59,<2.0',
  'requests>=2.27.1,<3.0.0',
  'uWSGI>=2.0.20,<3.0.0',
  'urllib3>=1.26.8,<2.0.0']
 
 setup_kwargs = {
     'name': 'caluma',
-    'version': '8.0.0b8',
+    'version': '8.0.0b9',
     'description': 'Caluma Service providing GraphQL API',
     'long_description': "# ![Caluma Service](https://user-images.githubusercontent.com/6150577/60805422-51b1bf80-a180-11e9-9ae5-c794249c7a98.png)\n\n[![Build Status](https://github.com/projectcaluma/caluma/workflows/Tests/badge.svg)](https://github.com/projectcaluma/caluma/actions?query=workflow%3ATests)\n[![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen.svg)](https://github.com/projectcaluma/caluma/blob/main/setup.cfg#L57)\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)\n[![PyPI](https://img.shields.io/pypi/v/caluma)](https://pypi.org/project/caluma/)\n[![License: GPL-3.0-or-later](https://img.shields.io/github/license/projectcaluma/caluma)](https://spdx.org/licenses/GPL-3.0-or-later.html)\n\nCaluma is a collaborative form editing and workflow service.\n\n- Website: [caluma.io](https://caluma.io)\n- Documentation: [caluma.gitbook.io](https://caluma.gitbook.io)\n\n## Getting started\n\n**Requirements**\n\n- docker\n- docker-compose\n\nAfter installing and configuring those, download [docker-compose.yml](https://github.com/projectcaluma/caluma/blob/main/docker-compose.yml) and run the following command:\n\n```bash\ndocker-compose up -d\n```\nSchema introspection and documentation is available at [http://localhost:8000/graphql](localhost:8000/graphql) and can be accessed using a GraphQL client such as [Altair](https://altair.sirmuel.design/). The API allows to query and mutate form and workflow entities which are described below.\n\nYou can read more about running and configuring Caluma in the [documentation](https://caluma.gitbook.io).\n\n## License\n\nCode released under the [GPL-3.0-or-later license](LICENSE).\n\nFor further information on our license choice, you can read up on the [corresponding GitHub issue](https://github.com/projectcaluma/caluma/issues/751#issuecomment-547974930).\n\n---\n\n- Contributing guide: [CONTRIBUTING.md](CONTRIBUTING.md)\n- Maintainer's Handbook: [MAINTAINING.md](MAINTAINING.md)\n",
     'author': 'Caluma',
     'author_email': 'info@caluma.io',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://caluma.io',
```

### Comparing `caluma-8.0.0b8/PKG-INFO` & `caluma-8.0.0b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caluma
-Version: 8.0.0b8
+Version: 8.0.0b9
 Summary: Caluma Service providing GraphQL API
 Home-page: https://caluma.io
 License: GPL-3.0-or-later
 Author: Caluma
 Author-email: info@caluma.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```


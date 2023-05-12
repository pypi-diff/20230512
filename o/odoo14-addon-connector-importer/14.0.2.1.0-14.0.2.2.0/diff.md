# Comparing `tmp/odoo14_addon_connector_importer-14.0.2.1.0-py3-none-any.whl.zip` & `tmp/odoo14_addon_connector_importer-14.0.2.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,76 +1,77 @@
-Zip file size: 99489 bytes, number of entries: 74
--rw-r--r--  2.0 unx     4056 b- defN 23-May-12 14:04 odoo/addons/connector_importer/README.rst
--rw-r--r--  2.0 unx       72 b- defN 23-May-12 14:04 odoo/addons/connector_importer/__init__.py
--rw-r--r--  2.0 unx     1033 b- defN 23-May-12 14:04 odoo/addons/connector_importer/__manifest__.py
--rw-r--r--  2.0 unx      985 b- defN 23-May-12 14:04 odoo/addons/connector_importer/events.py
--rw-r--r--  2.0 unx      757 b- defN 23-May-12 14:04 odoo/addons/connector_importer/log.py
--rw-r--r--  2.0 unx     1059 b- defN 23-May-12 14:04 odoo/addons/connector_importer/menuitems.xml
--rw-r--r--  2.0 unx      227 b- defN 23-May-12 14:04 odoo/addons/connector_importer/components/__init__.py
--rw-r--r--  2.0 unx      566 b- defN 23-May-12 14:04 odoo/addons/connector_importer/components/automapper.py
--rw-r--r--  2.0 unx      332 b- defN 23-May-12 14:04 odoo/addons/connector_importer/components/base.py
--rw-r--r--  2.0 unx     6256 b- defN 23-May-12 14:04 odoo/addons/connector_importer/components/dynamicmapper.py
--rw-r--r--  2.0 unx    15079 b- defN 23-May-12 14:04 odoo/addons/connector_importer/components/importer.py
--rw-r--r--  2.0 unx     6589 b- defN 23-May-12 14:04 odoo/addons/connector_importer/components/importer_csv_std.py
--rw-r--r--  2.0 unx     4380 b- defN 23-May-12 14:04 odoo/addons/connector_importer/components/mapper.py
--rw-r--r--  2.0 unx     9021 b- defN 23-May-12 14:04 odoo/addons/connector_importer/components/odoorecord.py
--rw-r--r--  2.0 unx     1436 b- defN 23-May-12 14:04 odoo/addons/connector_importer/components/odoorecord_csv_std.py
--rw-r--r--  2.0 unx     4204 b- defN 23-May-12 14:04 odoo/addons/connector_importer/components/tracker.py
--rw-r--r--  2.0 unx       19 b- defN 23-May-12 14:04 odoo/addons/connector_importer/controllers/__init__.py
--rw-r--r--  2.0 unx      788 b- defN 23-May-12 14:04 odoo/addons/connector_importer/controllers/main.py
--rw-r--r--  2.0 unx      678 b- defN 23-May-12 14:04 odoo/addons/connector_importer/data/ir_cron.xml
--rw-r--r--  2.0 unx      827 b- defN 23-May-12 14:04 odoo/addons/connector_importer/data/queue_job_function_data.xml
--rw-r--r--  2.0 unx    32311 b- defN 23-May-12 14:04 odoo/addons/connector_importer/i18n/connector_importer.pot
--rw-r--r--  2.0 unx      187 b- defN 23-May-12 14:04 odoo/addons/connector_importer/models/__init__.py
--rw-r--r--  2.0 unx     5152 b- defN 23-May-12 14:04 odoo/addons/connector_importer/models/backend.py
--rw-r--r--  2.0 unx     2499 b- defN 23-May-12 14:04 odoo/addons/connector_importer/models/cron_mixin.py
--rw-r--r--  2.0 unx     5696 b- defN 23-May-12 14:04 odoo/addons/connector_importer/models/import_type.py
--rw-r--r--  2.0 unx      903 b- defN 23-May-12 14:04 odoo/addons/connector_importer/models/job_mixin.py
--rw-r--r--  2.0 unx     4078 b- defN 23-May-12 14:04 odoo/addons/connector_importer/models/record.py
--rw-r--r--  2.0 unx    11612 b- defN 23-May-12 14:04 odoo/addons/connector_importer/models/recordset.py
--rw-r--r--  2.0 unx     8955 b- defN 23-May-12 14:04 odoo/addons/connector_importer/models/reporter.py
--rw-r--r--  2.0 unx       88 b- defN 23-May-12 14:04 odoo/addons/connector_importer/models/sources/__init__.py
--rw-r--r--  2.0 unx     2409 b- defN 23-May-12 14:04 odoo/addons/connector_importer/models/sources/source_consumer_mixin.py
--rw-r--r--  2.0 unx     4005 b- defN 23-May-12 14:04 odoo/addons/connector_importer/models/sources/source_csv.py
--rw-r--r--  2.0 unx     4110 b- defN 23-May-12 14:04 odoo/addons/connector_importer/models/sources/source_mixin.py
--rw-r--r--  2.0 unx      184 b- defN 23-May-12 14:04 odoo/addons/connector_importer/readme/CONTRIBUTORS.rst
--rw-r--r--  2.0 unx      118 b- defN 23-May-12 14:04 odoo/addons/connector_importer/readme/DESCRIPTION.rst
--rw-r--r--  2.0 unx     1027 b- defN 23-May-12 14:04 odoo/addons/connector_importer/readme/ROADMAP.rst
--rw-r--r--  2.0 unx     1402 b- defN 23-May-12 14:04 odoo/addons/connector_importer/security/ir.model.access.csv
--rw-r--r--  2.0 unx      647 b- defN 23-May-12 14:04 odoo/addons/connector_importer/security/security.xml
--rw-r--r--  2.0 unx     8186 b- defN 23-May-12 14:04 odoo/addons/connector_importer/static/description/icon.png
--rw-r--r--  2.0 unx     4486 b- defN 23-May-12 14:04 odoo/addons/connector_importer/static/description/icon.svg
--rw-r--r--  2.0 unx    13479 b- defN 23-May-12 14:04 odoo/addons/connector_importer/static/description/index.html
--rw-r--r--  2.0 unx      344 b- defN 23-May-12 14:04 odoo/addons/connector_importer/tests/__init__.py
--rw-r--r--  2.0 unx     3171 b- defN 23-May-12 14:04 odoo/addons/connector_importer/tests/common.py
--rw-r--r--  2.0 unx     1814 b- defN 23-May-12 14:04 odoo/addons/connector_importer/tests/fake_components.py
--rw-r--r--  2.0 unx     1022 b- defN 23-May-12 14:04 odoo/addons/connector_importer/tests/fake_models.py
--rw-r--r--  2.0 unx     1543 b- defN 23-May-12 14:04 odoo/addons/connector_importer/tests/test_backend.py
--rw-r--r--  2.0 unx     1505 b- defN 23-May-12 14:04 odoo/addons/connector_importer/tests/test_cron.py
--rw-r--r--  2.0 unx     5840 b- defN 23-May-12 14:04 odoo/addons/connector_importer/tests/test_import_type.py
--rw-r--r--  2.0 unx     4087 b- defN 23-May-12 14:04 odoo/addons/connector_importer/tests/test_mapper.py
--rw-r--r--  2.0 unx     2700 b- defN 23-May-12 14:04 odoo/addons/connector_importer/tests/test_record_handler.py
--rw-r--r--  2.0 unx     4451 b- defN 23-May-12 14:04 odoo/addons/connector_importer/tests/test_record_importer.py
--rw-r--r--  2.0 unx     4258 b- defN 23-May-12 14:04 odoo/addons/connector_importer/tests/test_record_importer_basic.py
--rw-r--r--  2.0 unx     1847 b- defN 23-May-12 14:04 odoo/addons/connector_importer/tests/test_record_importer_xmlid.py
--rw-r--r--  2.0 unx     3008 b- defN 23-May-12 14:04 odoo/addons/connector_importer/tests/test_recordset.py
--rw-r--r--  2.0 unx     3352 b- defN 23-May-12 14:04 odoo/addons/connector_importer/tests/test_recordset_importer.py
--rw-r--r--  2.0 unx     2760 b- defN 23-May-12 14:04 odoo/addons/connector_importer/tests/test_source.py
--rw-r--r--  2.0 unx     2990 b- defN 23-May-12 14:04 odoo/addons/connector_importer/tests/test_source_csv.py
--rw-r--r--  2.0 unx       85 b- defN 23-May-12 14:04 odoo/addons/connector_importer/tests/fixtures/csv_source_test1.csv
--rw-r--r--  2.0 unx        0 b- defN 23-May-12 14:04 odoo/addons/connector_importer/utils/__init__.py
--rw-r--r--  2.0 unx     4114 b- defN 23-May-12 14:04 odoo/addons/connector_importer/utils/import_utils.py
--rw-r--r--  2.0 unx    11103 b- defN 23-May-12 14:04 odoo/addons/connector_importer/utils/mapper_utils.py
--rw-r--r--  2.0 unx     2418 b- defN 23-May-12 14:04 odoo/addons/connector_importer/utils/misc.py
--rw-r--r--  2.0 unx     4254 b- defN 23-May-12 14:04 odoo/addons/connector_importer/utils/report_html.py
--rw-r--r--  2.0 unx     6218 b- defN 23-May-12 14:04 odoo/addons/connector_importer/views/backend_views.xml
--rw-r--r--  2.0 unx     9503 b- defN 23-May-12 14:04 odoo/addons/connector_importer/views/docs_template.xml
--rw-r--r--  2.0 unx     1637 b- defN 23-May-12 14:04 odoo/addons/connector_importer/views/import_type_views.xml
--rw-r--r--  2.0 unx     5912 b- defN 23-May-12 14:04 odoo/addons/connector_importer/views/recordset_views.xml
--rw-r--r--  2.0 unx     2099 b- defN 23-May-12 14:04 odoo/addons/connector_importer/views/report_template.xml
--rw-r--r--  2.0 unx      576 b- defN 23-May-12 14:04 odoo/addons/connector_importer/views/source_config_template.xml
--rw-r--r--  2.0 unx     2616 b- defN 23-May-12 14:04 odoo/addons/connector_importer/views/source_views.xml
--rw-r--r--  2.0 unx     4764 b- defN 23-May-12 14:04 odoo14_addon_connector_importer-14.0.2.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-12 14:04 odoo14_addon_connector_importer-14.0.2.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-May-12 14:04 odoo14_addon_connector_importer-14.0.2.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     8129 b- defN 23-May-12 14:04 odoo14_addon_connector_importer-14.0.2.1.0.dist-info/RECORD
-74 files, 278115 bytes uncompressed, 85861 bytes compressed:  69.1%
+Zip file size: 100093 bytes, number of entries: 75
+-rw-r--r--  2.0 unx     4056 b- defN 23-May-12 14:44 odoo/addons/connector_importer/README.rst
+-rw-r--r--  2.0 unx       72 b- defN 23-May-12 14:44 odoo/addons/connector_importer/__init__.py
+-rw-r--r--  2.0 unx     1033 b- defN 23-May-12 14:44 odoo/addons/connector_importer/__manifest__.py
+-rw-r--r--  2.0 unx      985 b- defN 23-May-12 14:44 odoo/addons/connector_importer/events.py
+-rw-r--r--  2.0 unx      757 b- defN 23-May-12 14:44 odoo/addons/connector_importer/log.py
+-rw-r--r--  2.0 unx     1059 b- defN 23-May-12 14:44 odoo/addons/connector_importer/menuitems.xml
+-rw-r--r--  2.0 unx      227 b- defN 23-May-12 14:44 odoo/addons/connector_importer/components/__init__.py
+-rw-r--r--  2.0 unx      566 b- defN 23-May-12 14:44 odoo/addons/connector_importer/components/automapper.py
+-rw-r--r--  2.0 unx      332 b- defN 23-May-12 14:44 odoo/addons/connector_importer/components/base.py
+-rw-r--r--  2.0 unx     6520 b- defN 23-May-12 14:44 odoo/addons/connector_importer/components/dynamicmapper.py
+-rw-r--r--  2.0 unx    15079 b- defN 23-May-12 14:44 odoo/addons/connector_importer/components/importer.py
+-rw-r--r--  2.0 unx     6589 b- defN 23-May-12 14:44 odoo/addons/connector_importer/components/importer_csv_std.py
+-rw-r--r--  2.0 unx     4380 b- defN 23-May-12 14:44 odoo/addons/connector_importer/components/mapper.py
+-rw-r--r--  2.0 unx     8991 b- defN 23-May-12 14:44 odoo/addons/connector_importer/components/odoorecord.py
+-rw-r--r--  2.0 unx     1436 b- defN 23-May-12 14:44 odoo/addons/connector_importer/components/odoorecord_csv_std.py
+-rw-r--r--  2.0 unx     4204 b- defN 23-May-12 14:44 odoo/addons/connector_importer/components/tracker.py
+-rw-r--r--  2.0 unx       19 b- defN 23-May-12 14:44 odoo/addons/connector_importer/controllers/__init__.py
+-rw-r--r--  2.0 unx      788 b- defN 23-May-12 14:44 odoo/addons/connector_importer/controllers/main.py
+-rw-r--r--  2.0 unx      678 b- defN 23-May-12 14:44 odoo/addons/connector_importer/data/ir_cron.xml
+-rw-r--r--  2.0 unx      827 b- defN 23-May-12 14:44 odoo/addons/connector_importer/data/queue_job_function_data.xml
+-rw-r--r--  2.0 unx    32311 b- defN 23-May-12 14:44 odoo/addons/connector_importer/i18n/connector_importer.pot
+-rw-r--r--  2.0 unx      187 b- defN 23-May-12 14:44 odoo/addons/connector_importer/models/__init__.py
+-rw-r--r--  2.0 unx     5152 b- defN 23-May-12 14:44 odoo/addons/connector_importer/models/backend.py
+-rw-r--r--  2.0 unx     2499 b- defN 23-May-12 14:44 odoo/addons/connector_importer/models/cron_mixin.py
+-rw-r--r--  2.0 unx     5696 b- defN 23-May-12 14:44 odoo/addons/connector_importer/models/import_type.py
+-rw-r--r--  2.0 unx      903 b- defN 23-May-12 14:44 odoo/addons/connector_importer/models/job_mixin.py
+-rw-r--r--  2.0 unx     4078 b- defN 23-May-12 14:44 odoo/addons/connector_importer/models/record.py
+-rw-r--r--  2.0 unx    11612 b- defN 23-May-12 14:44 odoo/addons/connector_importer/models/recordset.py
+-rw-r--r--  2.0 unx     8955 b- defN 23-May-12 14:44 odoo/addons/connector_importer/models/reporter.py
+-rw-r--r--  2.0 unx       88 b- defN 23-May-12 14:44 odoo/addons/connector_importer/models/sources/__init__.py
+-rw-r--r--  2.0 unx     2409 b- defN 23-May-12 14:44 odoo/addons/connector_importer/models/sources/source_consumer_mixin.py
+-rw-r--r--  2.0 unx     4005 b- defN 23-May-12 14:44 odoo/addons/connector_importer/models/sources/source_csv.py
+-rw-r--r--  2.0 unx     4110 b- defN 23-May-12 14:44 odoo/addons/connector_importer/models/sources/source_mixin.py
+-rw-r--r--  2.0 unx      184 b- defN 23-May-12 14:44 odoo/addons/connector_importer/readme/CONTRIBUTORS.rst
+-rw-r--r--  2.0 unx      118 b- defN 23-May-12 14:44 odoo/addons/connector_importer/readme/DESCRIPTION.rst
+-rw-r--r--  2.0 unx     1027 b- defN 23-May-12 14:44 odoo/addons/connector_importer/readme/ROADMAP.rst
+-rw-r--r--  2.0 unx     1402 b- defN 23-May-12 14:44 odoo/addons/connector_importer/security/ir.model.access.csv
+-rw-r--r--  2.0 unx      647 b- defN 23-May-12 14:44 odoo/addons/connector_importer/security/security.xml
+-rw-r--r--  2.0 unx     8186 b- defN 23-May-12 14:44 odoo/addons/connector_importer/static/description/icon.png
+-rw-r--r--  2.0 unx     4486 b- defN 23-May-12 14:44 odoo/addons/connector_importer/static/description/icon.svg
+-rw-r--r--  2.0 unx    13479 b- defN 23-May-12 14:44 odoo/addons/connector_importer/static/description/index.html
+-rw-r--r--  2.0 unx      344 b- defN 23-May-12 14:44 odoo/addons/connector_importer/tests/__init__.py
+-rw-r--r--  2.0 unx     3171 b- defN 23-May-12 14:44 odoo/addons/connector_importer/tests/common.py
+-rw-r--r--  2.0 unx     1814 b- defN 23-May-12 14:44 odoo/addons/connector_importer/tests/fake_components.py
+-rw-r--r--  2.0 unx     1022 b- defN 23-May-12 14:44 odoo/addons/connector_importer/tests/fake_models.py
+-rw-r--r--  2.0 unx      754 b- defN 23-May-12 14:44 odoo/addons/connector_importer/tests/record_capturer.py
+-rw-r--r--  2.0 unx     1543 b- defN 23-May-12 14:44 odoo/addons/connector_importer/tests/test_backend.py
+-rw-r--r--  2.0 unx     1505 b- defN 23-May-12 14:44 odoo/addons/connector_importer/tests/test_cron.py
+-rw-r--r--  2.0 unx     5840 b- defN 23-May-12 14:44 odoo/addons/connector_importer/tests/test_import_type.py
+-rw-r--r--  2.0 unx     4372 b- defN 23-May-12 14:44 odoo/addons/connector_importer/tests/test_mapper.py
+-rw-r--r--  2.0 unx     2700 b- defN 23-May-12 14:44 odoo/addons/connector_importer/tests/test_record_handler.py
+-rw-r--r--  2.0 unx     4451 b- defN 23-May-12 14:44 odoo/addons/connector_importer/tests/test_record_importer.py
+-rw-r--r--  2.0 unx     4258 b- defN 23-May-12 14:44 odoo/addons/connector_importer/tests/test_record_importer_basic.py
+-rw-r--r--  2.0 unx     1847 b- defN 23-May-12 14:44 odoo/addons/connector_importer/tests/test_record_importer_xmlid.py
+-rw-r--r--  2.0 unx     3008 b- defN 23-May-12 14:44 odoo/addons/connector_importer/tests/test_recordset.py
+-rw-r--r--  2.0 unx     3352 b- defN 23-May-12 14:44 odoo/addons/connector_importer/tests/test_recordset_importer.py
+-rw-r--r--  2.0 unx     2760 b- defN 23-May-12 14:44 odoo/addons/connector_importer/tests/test_source.py
+-rw-r--r--  2.0 unx     2990 b- defN 23-May-12 14:44 odoo/addons/connector_importer/tests/test_source_csv.py
+-rw-r--r--  2.0 unx       85 b- defN 23-May-12 14:44 odoo/addons/connector_importer/tests/fixtures/csv_source_test1.csv
+-rw-r--r--  2.0 unx        0 b- defN 23-May-12 14:44 odoo/addons/connector_importer/utils/__init__.py
+-rw-r--r--  2.0 unx     4114 b- defN 23-May-12 14:44 odoo/addons/connector_importer/utils/import_utils.py
+-rw-r--r--  2.0 unx    11103 b- defN 23-May-12 14:44 odoo/addons/connector_importer/utils/mapper_utils.py
+-rw-r--r--  2.0 unx     2418 b- defN 23-May-12 14:44 odoo/addons/connector_importer/utils/misc.py
+-rw-r--r--  2.0 unx     4254 b- defN 23-May-12 14:44 odoo/addons/connector_importer/utils/report_html.py
+-rw-r--r--  2.0 unx     6218 b- defN 23-May-12 14:44 odoo/addons/connector_importer/views/backend_views.xml
+-rw-r--r--  2.0 unx     9503 b- defN 23-May-12 14:44 odoo/addons/connector_importer/views/docs_template.xml
+-rw-r--r--  2.0 unx     1637 b- defN 23-May-12 14:44 odoo/addons/connector_importer/views/import_type_views.xml
+-rw-r--r--  2.0 unx     5912 b- defN 23-May-12 14:44 odoo/addons/connector_importer/views/recordset_views.xml
+-rw-r--r--  2.0 unx     2099 b- defN 23-May-12 14:44 odoo/addons/connector_importer/views/report_template.xml
+-rw-r--r--  2.0 unx      576 b- defN 23-May-12 14:44 odoo/addons/connector_importer/views/source_config_template.xml
+-rw-r--r--  2.0 unx     2616 b- defN 23-May-12 14:44 odoo/addons/connector_importer/views/source_views.xml
+-rw-r--r--  2.0 unx     4764 b- defN 23-May-12 14:45 odoo14_addon_connector_importer-14.0.2.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-12 14:45 odoo14_addon_connector_importer-14.0.2.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-May-12 14:45 odoo14_addon_connector_importer-14.0.2.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     8240 b- defN 23-May-12 14:45 odoo14_addon_connector_importer-14.0.2.2.0.dist-info/RECORD
+75 files, 279499 bytes uncompressed, 86279 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -129,14 +129,17 @@
 
 Filename: odoo/addons/connector_importer/tests/fake_components.py
 Comment: 
 
 Filename: odoo/addons/connector_importer/tests/fake_models.py
 Comment: 
 
+Filename: odoo/addons/connector_importer/tests/record_capturer.py
+Comment: 
+
 Filename: odoo/addons/connector_importer/tests/test_backend.py
 Comment: 
 
 Filename: odoo/addons/connector_importer/tests/test_cron.py
 Comment: 
 
 Filename: odoo/addons/connector_importer/tests/test_import_type.py
@@ -204,20 +207,20 @@
 
 Filename: odoo/addons/connector_importer/views/source_config_template.xml
 Comment: 
 
 Filename: odoo/addons/connector_importer/views/source_views.xml
 Comment: 
 
-Filename: odoo14_addon_connector_importer-14.0.2.1.0.dist-info/METADATA
+Filename: odoo14_addon_connector_importer-14.0.2.2.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_connector_importer-14.0.2.1.0.dist-info/WHEEL
+Filename: odoo14_addon_connector_importer-14.0.2.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_connector_importer-14.0.2.1.0.dist-info/top_level.txt
+Filename: odoo14_addon_connector_importer-14.0.2.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_connector_importer-14.0.2.1.0.dist-info/RECORD
+Filename: odoo14_addon_connector_importer-14.0.2.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/connector_importer/__manifest__.py

```diff
@@ -1,15 +1,15 @@
 # Author: Simone Orsi
 # Copyright 2018 Camptocamp SA
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl.html).
 
 {
     "name": "Connector Importer",
     "summary": """This module takes care of import sessions.""",
-    "version": "14.0.2.1.0",
+    "version": "14.0.2.2.0",
     "depends": ["connector", "queue_job"],
     "author": "Camptocamp, Odoo Community Association (OCA)",
     "license": "AGPL-3",
     "category": "Connector",
     "website": "https://github.com/OCA/connector-interfaces",
     "maintainers": ["simahawk"],
     "data": [
```

## odoo/addons/connector_importer/components/dynamicmapper.py

```diff
@@ -78,24 +78,31 @@
         valid_keys = [k for k in record.keys() if not k.startswith("_")]
         prefix = self._source_key_prefix
         if prefix:
             valid_keys = [k for k in valid_keys if k.startswith(prefix)]
         whitelist = self._source_key_whitelist
         if whitelist:
             valid_keys = [k for k in valid_keys if k in whitelist]
+        blacklist = self._source_key_blacklist
+        if blacklist:
+            valid_keys = [k for k in valid_keys if k not in blacklist]
         return tuple(valid_keys)
 
     def _required_keys(self):
         return [k for k, v in self.model.fields_get().items() if v["required"]]
 
     @property
     def _source_key_whitelist(self):
         return self.work.options.mapper.get("source_key_whitelist", [])
 
     @property
+    def _source_key_blacklist(self):
+        return self.work.options.mapper.get("source_key_blacklist", [])
+
+    @property
     def _source_key_empty_skip(self):
         """List of source keys to skip when empty.
 
         Use cases:
 
             * field w/ unique constraint but not populated (eg: product barcode)
             * field not to override when empty
```

## odoo/addons/connector_importer/components/odoorecord.py

```diff
@@ -78,21 +78,19 @@
             raise ValueError(
                 f"Cannot find `{self.unique_key}` key in `values` nor `orig_values`"
             )
         return [(self.unique_key, "=", value)]
 
     def odoo_find(self, values, orig_values):
         """Find any existing item in odoo."""
-        if self.unique_key == "":
+        if self.unique_key and self.unique_key_is_xmlid:
             # if unique_key is None we might use as special find domain
-            return self.model
-        if self.unique_key_is_xmlid:
             xid = self._get_xmlid(values, orig_values)
             item = self.env.ref(xid, raise_if_not_found=False)
-            return item
+            return item or self.model
         item = self.model.search(
             self.odoo_find_domain(values, orig_values),
             order="create_date desc",
             limit=1,
         )
         return item
```

## odoo/addons/connector_importer/tests/test_mapper.py

```diff
@@ -57,14 +57,22 @@
             options=dict(source_key_whitelist=["name", "ref"])
         )
         expected = {
             "name": "John Doe",
             "ref": "12345",
         }
         self.assertEqual(mapper._clean_record(rec), expected)
+        # Blacklist
+        mapper = self._get_dynamyc_mapper(options=dict(source_key_blacklist=["ref"]))
+        expected = {
+            "name": "John Doe",
+            "some_one": 1,
+            "some_two": 2,
+        }
+        self.assertEqual(mapper._clean_record(rec), expected)
         # Prefix
         mapper = self._get_dynamyc_mapper(options=dict(source_key_prefix="some_"))
         expected = {
             "some_one": 1,
             "some_two": 2,
         }
         self.assertEqual(mapper._clean_record(rec), expected)
```

## Comparing `odoo14_addon_connector_importer-14.0.2.1.0.dist-info/METADATA` & `odoo14_addon_connector_importer-14.0.2.2.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-connector-importer
-Version: 14.0.2.1.0
+Version: 14.0.2.2.0
 Summary: This module takes care of import sessions.
 Home-page: https://github.com/OCA/connector-interfaces
 Author: Camptocamp, Odoo Community Association (OCA)
 Author-email: support@odoo-community.org
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

## Comparing `odoo14_addon_connector_importer-14.0.2.1.0.dist-info/RECORD` & `odoo14_addon_connector_importer-14.0.2.2.0.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 odoo/addons/connector_importer/README.rst,sha256=uvfiXXWG9O758SjPvOL_cS5OxJIDmq8X7Yvxc9zM9Wo,4056
 odoo/addons/connector_importer/__init__.py,sha256=5SeaXt24NrD4Cl8GdTw9cCoQGGsXBtNqjgaG5NwJZB8,72
-odoo/addons/connector_importer/__manifest__.py,sha256=buOkUBQuEkPm-dtLjWpOGAcEB7l2HciRwAqtzHDiYjo,1033
+odoo/addons/connector_importer/__manifest__.py,sha256=rcuhI0AjT7tIfAvKB3MXiCEp1xhULmO2PV4KhF1z9wk,1033
 odoo/addons/connector_importer/events.py,sha256=zCYEllpQE1FFKv_5HFzVDYJ3VrTe184JqD46tL661-Q,985
 odoo/addons/connector_importer/log.py,sha256=MFjVgOU0c3dRyBViLa8kiV7b3gYpE0cXc8_lD2qmgcc,757
 odoo/addons/connector_importer/menuitems.xml,sha256=9MWWuMwaebl0PByML1VYnaiz9BscvUwedEa8gJnfLYM,1059
 odoo/addons/connector_importer/components/__init__.py,sha256=R7E960FPDtW9OXhWEyIwd8Bfez2xXtrlMCzqxX8xsCs,227
 odoo/addons/connector_importer/components/automapper.py,sha256=N7gpp-NzFXvQN4uxfvRGaA-2uIzGMmEf1f8RctWezfc,566
 odoo/addons/connector_importer/components/base.py,sha256=SXRDM0H_I13Eu_qfUvZ9xaCZplXf9PSnAt1ydhJ176s,332
-odoo/addons/connector_importer/components/dynamicmapper.py,sha256=7J0XCePl1GcFQEWSNHUST6Bvl7XPXOh-tmkL24yF_Yg,6256
+odoo/addons/connector_importer/components/dynamicmapper.py,sha256=nncWvvfP8AAVTe4g8eLWEVIzEmM5PnCwfpbI387vyl8,6520
 odoo/addons/connector_importer/components/importer.py,sha256=G200k6m9w-6OTPBxPFXyWIBBDjQwICHEkgni4qw8mZ4,15079
 odoo/addons/connector_importer/components/importer_csv_std.py,sha256=A50NzEH5ZJY_6jmpZbaPoakVX6oDxNWDdUSkSZ92A9Q,6589
 odoo/addons/connector_importer/components/mapper.py,sha256=xCHab-xVM0sbqkunZEUZwmuMHoTEGlnDes7cI6zYegA,4380
-odoo/addons/connector_importer/components/odoorecord.py,sha256=gQQt1FVC4pcS3SKavCqaIUbzfu4uJTNFBqxpdpt4Hls,9021
+odoo/addons/connector_importer/components/odoorecord.py,sha256=GDMV11jQ-U7EdZog7Y5mwKA1pm_9zYwBKt0LrdmFulk,8991
 odoo/addons/connector_importer/components/odoorecord_csv_std.py,sha256=2a6suU7GEcbfJNYqpmwB0ABJVj0pTiuATAKQP0M02Cs,1436
 odoo/addons/connector_importer/components/tracker.py,sha256=LVATxle9Cme4mcs37Y0pdJqExRFnK-QrzeFjws1I2zU,4204
 odoo/addons/connector_importer/controllers/__init__.py,sha256=4KFqEP2QHFbPN66eQJMdGsmNz2v7ywWv_FR1pW_kkLk,19
 odoo/addons/connector_importer/controllers/main.py,sha256=nhoRxonfXSGRgiU4b3ZG_-VnOXx40fZbpgZucdvVilU,788
 odoo/addons/connector_importer/data/ir_cron.xml,sha256=rOMNu38Eyf6oP_wZ_RrGaLYAw2ppps1LeVAn3MRCvdY,678
 odoo/addons/connector_importer/data/queue_job_function_data.xml,sha256=2NLyI0tIRNqHCK6LzLR2HxqlJbP_IkXhdSWBRckEcrA,827
 odoo/addons/connector_importer/i18n/connector_importer.pot,sha256=C68K6cY8dM9q1QCqrssitDzrMqm9seXpou5Z1maCPWU,32311
@@ -39,18 +39,19 @@
 odoo/addons/connector_importer/static/description/icon.png,sha256=ztiNztfXtOo4rA4pIAvPMkmkj0G_lx2Ow8xv2R1XSlM,8186
 odoo/addons/connector_importer/static/description/icon.svg,sha256=cwI163PipvGJwxSvRXsVrmIYINcToB5BA6uljaCQqZI,4486
 odoo/addons/connector_importer/static/description/index.html,sha256=gRwsd4iBHpYfBWJU6ZcrRKv672_aLE-4Y2DEySo2yOw,13479
 odoo/addons/connector_importer/tests/__init__.py,sha256=70aHT5M-lnglwig0RYAirSGiJSXQCcPfG3BY7pzztQ8,344
 odoo/addons/connector_importer/tests/common.py,sha256=KXQEdAMczgXrWPaw78Lh9nrM8wM2rLo_--jNXd6qdik,3171
 odoo/addons/connector_importer/tests/fake_components.py,sha256=g8BGXc3KkKtubuKgUlT3fulR9KuzpeaDOreEZ4joAC4,1814
 odoo/addons/connector_importer/tests/fake_models.py,sha256=n14ncv6ivEJAwBZIKbyLpouFs8bji_W8UcBg-urcYuI,1022
+odoo/addons/connector_importer/tests/record_capturer.py,sha256=mpWzbqOsXd2fykIJ6O1_gngtroOZNa9Cl-PgR1giFak,754
 odoo/addons/connector_importer/tests/test_backend.py,sha256=CIgsUfTvZQ579jI6TOdYbiyY94MYoKZHmLgQ8vbCjUQ,1543
 odoo/addons/connector_importer/tests/test_cron.py,sha256=37fIpfhOc64J47NKI5E-kgW3aEGApAWuvRzYvgjerYM,1505
 odoo/addons/connector_importer/tests/test_import_type.py,sha256=BN5rncBa0zT8fMnLeMOBnxO1QKfwWcojlcKuCEFYHfk,5840
-odoo/addons/connector_importer/tests/test_mapper.py,sha256=Kd7RxT0mgMWyBy1RDtAklyCDP2CC2AHmok1dptkwk_0,4087
+odoo/addons/connector_importer/tests/test_mapper.py,sha256=KOjWdd6CVxeNu0aDgR4se04h5jdtyuD56YsBILpWBSE,4372
 odoo/addons/connector_importer/tests/test_record_handler.py,sha256=ihbyP3dYFMW1xN3Lvch1XuwfwN1FFXCzSDkoWarI-XY,2700
 odoo/addons/connector_importer/tests/test_record_importer.py,sha256=LIv0E2_nrfGPRk0aV1sUj-dglFDnsDGqc4HsNO1M0y0,4451
 odoo/addons/connector_importer/tests/test_record_importer_basic.py,sha256=Ujynpv0ElQq7qEr9nHjQ3yWoDOoXog6jb0A6cH5sKAo,4258
 odoo/addons/connector_importer/tests/test_record_importer_xmlid.py,sha256=4Qcp7o7tNbfpm7YJ8rS-IUnZyvA3Z0R9vvHI1WVPGdU,1847
 odoo/addons/connector_importer/tests/test_recordset.py,sha256=KcwunzLbNWV-yCSka-qYaKvIAV26djAP-NJ1186MYVA,3008
 odoo/addons/connector_importer/tests/test_recordset_importer.py,sha256=qXK23Bg6_-2y3UyvsRjvA2GAuivKmt_uLMqqVTdKhvg,3352
 odoo/addons/connector_importer/tests/test_source.py,sha256=U-dbcxAjoWCmDrwuQ_Y-spLCU7yq-8Ah9hif_1vRFeQ,2760
@@ -64,11 +65,11 @@
 odoo/addons/connector_importer/views/backend_views.xml,sha256=ed8t86WnZLFw9rgdUcTdstvTkOaCZU7Qd1x7iW6GCEk,6218
 odoo/addons/connector_importer/views/docs_template.xml,sha256=QHQgJtlEBqulmLzpulpHiAGSnHmkEYds-hGsf55AOmw,9503
 odoo/addons/connector_importer/views/import_type_views.xml,sha256=hklf5eaJ0NVGJDr3-tDr-ZXJy3I4IbTHoUKOsahdeHU,1637
 odoo/addons/connector_importer/views/recordset_views.xml,sha256=34TTS_vyNAskBZxSUqzhLVOV7XYFok0_jbP_qJnyXwg,5912
 odoo/addons/connector_importer/views/report_template.xml,sha256=DLYJgdxWw2FoH-1IFaKqQ5Vpl_J7wEzryPonpTGUzxc,2099
 odoo/addons/connector_importer/views/source_config_template.xml,sha256=LzIiidOvDNBRQV_5byrSQK6gyVDxcbVr4rlnxLTkKgw,576
 odoo/addons/connector_importer/views/source_views.xml,sha256=-8V2OP0V2Ier1ulc8L9mhY7mp104HkbVHGJj64e7Kkc,2616
-odoo14_addon_connector_importer-14.0.2.1.0.dist-info/METADATA,sha256=K1HyNKYHVEmupB8784shxEUy1KWl61UR2x4LvmVsla8,4764
-odoo14_addon_connector_importer-14.0.2.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-odoo14_addon_connector_importer-14.0.2.1.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_connector_importer-14.0.2.1.0.dist-info/RECORD,,
+odoo14_addon_connector_importer-14.0.2.2.0.dist-info/METADATA,sha256=Gn6DcdrOUb2FU6zi8tffyyoEMZB5SpjZpRTQieSSGkA,4764
+odoo14_addon_connector_importer-14.0.2.2.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+odoo14_addon_connector_importer-14.0.2.2.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_connector_importer-14.0.2.2.0.dist-info/RECORD,,
```


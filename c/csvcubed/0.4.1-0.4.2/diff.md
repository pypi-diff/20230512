# Comparing `tmp/csvcubed-0.4.1-py3-none-any.whl.zip` & `tmp/csvcubed-0.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,32 @@
-Zip file size: 217787 bytes, number of entries: 184
+Zip file size: 224259 bytes, number of entries: 189
 -rw-r--r--  2.0 unx     1515 b- defN 80-Jan-01 00:00 csvcubed/README.md
 -rw-r--r--  2.0 unx      218 b- defN 80-Jan-01 00:00 csvcubed/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/cli/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/cli/buildcsvw/__init__.py
 -rw-r--r--  2.0 unx     2881 b- defN 80-Jan-01 00:00 csvcubed/cli/buildcsvw/build.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/cli/codelist/__init__.py
 -rw-r--r--  2.0 unx     1414 b- defN 80-Jan-01 00:00 csvcubed/cli/codelist/build_code_list.py
 -rw-r--r--  2.0 unx     5742 b- defN 80-Jan-01 00:00 csvcubed/cli/entrypoint.py
 -rw-r--r--  2.0 unx     9572 b- defN 80-Jan-01 00:00 csvcubed/cli/error_mapping.py
 -rw-r--r--  2.0 unx      238 b- defN 80-Jan-01 00:00 csvcubed/cli/inspectcsvw/README.md
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/cli/inspectcsvw/__init__.py
--rw-r--r--  2.0 unx     4300 b- defN 80-Jan-01 00:00 csvcubed/cli/inspectcsvw/inspect.py
+-rw-r--r--  2.0 unx     4316 b- defN 80-Jan-01 00:00 csvcubed/cli/inspectcsvw/inspect.py
 -rw-r--r--  2.0 unx     3333 b- defN 80-Jan-01 00:00 csvcubed/cli/inspectcsvw/inspectdatasetmanager.py
 -rw-r--r--  2.0 unx     1517 b- defN 80-Jan-01 00:00 csvcubed/cli/inspectcsvw/metadatainputvalidator.py
--rw-r--r--  2.0 unx    13706 b- defN 80-Jan-01 00:00 csvcubed/cli/inspectcsvw/metadataprinter.py
+-rw-r--r--  2.0 unx    15006 b- defN 80-Jan-01 00:00 csvcubed/cli/inspectcsvw/metadataprinter.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/cli/pullcsvw/__init__.py
 -rw-r--r--  2.0 unx    13791 b- defN 80-Jan-01 00:00 csvcubed/cli/pullcsvw/pull.py
 -rw-r--r--  2.0 unx      840 b- defN 80-Jan-01 00:00 csvcubed/definitions.py
 -rw-r--r--  2.0 unx     1981 b- defN 80-Jan-01 00:00 csvcubed/inputs.py
+-rw-r--r--  2.0 unx     7577 b- defN 80-Jan-01 00:00 csvcubed/inspect/inspectorcolumns.py
+-rw-r--r--  2.0 unx     3425 b- defN 80-Jan-01 00:00 csvcubed/inspect/inspectorcomponents.py
+-rw-r--r--  2.0 unx     3241 b- defN 80-Jan-01 00:00 csvcubed/inspect/inspectors.py
+-rw-r--r--  2.0 unx     7419 b- defN 80-Jan-01 00:00 csvcubed/inspect/inspectortable.py
+-rw-r--r--  2.0 unx     1657 b- defN 80-Jan-01 00:00 csvcubed/inspect/lazyfuncdescriptor.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/models/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/models/codelistconfig/__init__.py
 -rw-r--r--  2.0 unx     8467 b- defN 80-Jan-01 00:00 csvcubed/models/codelistconfig/code_list_config.py
 -rw-r--r--  2.0 unx    14542 b- defN 80-Jan-01 00:00 csvcubed/models/csvcubedexception.py
 -rw-r--r--  2.0 unx      409 b- defN 80-Jan-01 00:00 csvcubed/models/csvwtype.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/models/cube/__init__.py
 -rw-r--r--  2.0 unx      676 b- defN 80-Jan-01 00:00 csvcubed/models/cube/catalog.py
@@ -57,15 +62,15 @@
 -rw-r--r--  2.0 unx      526 b- defN 80-Jan-01 00:00 csvcubed/models/rdf/conceptschemeincatalog.py
 -rw-r--r--  2.0 unx      858 b- defN 80-Jan-01 00:00 csvcubed/models/rdf/newattributevalueresource.py
 -rw-r--r--  2.0 unx     1670 b- defN 80-Jan-01 00:00 csvcubed/models/rdf/newunitresource.py
 -rw-r--r--  2.0 unx     1188 b- defN 80-Jan-01 00:00 csvcubed/models/rdf/prov.py
 -rw-r--r--  2.0 unx      447 b- defN 80-Jan-01 00:00 csvcubed/models/rdf/qbdatasetincatalog.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/models/sparql/__init__.py
 -rw-r--r--  2.0 unx      457 b- defN 80-Jan-01 00:00 csvcubed/models/sparql/valuesbinding.py
--rw-r--r--  2.0 unx    20070 b- defN 80-Jan-01 00:00 csvcubed/models/sparqlresults.py
+-rw-r--r--  2.0 unx    18128 b- defN 80-Jan-01 00:00 csvcubed/models/sparqlresults.py
 -rw-r--r--  2.0 unx     1814 b- defN 80-Jan-01 00:00 csvcubed/models/uriidentifiable.py
 -rw-r--r--  2.0 unx     3108 b- defN 80-Jan-01 00:00 csvcubed/models/validatedmodel.py
 -rw-r--r--  2.0 unx     3167 b- defN 80-Jan-01 00:00 csvcubed/models/validationerror.py
 -rw-r--r--  2.0 unx      110 b- defN 80-Jan-01 00:00 csvcubed/readers/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/readers/catalogmetadata/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/readers/catalogmetadata/v1/__init__.py
 -rw-r--r--  2.0 unx     1637 b- defN 80-Jan-01 00:00 csvcubed/readers/catalogmetadata/v1/catalog_metadata_reader.py
@@ -112,58 +117,58 @@
 -rw-r--r--  2.0 unx    26394 b- defN 80-Jan-01 00:00 csvcubed/schema/cube-config/v1_2/schema.json
 -rw-r--r--  2.0 unx    31399 b- defN 80-Jan-01 00:00 csvcubed/schema/cube-config/v1_3/schema.json
 -rw-r--r--  2.0 unx    32992 b- defN 80-Jan-01 00:00 csvcubed/schema/cube-config/v1_4/schema.json
 -rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 csvcubed/utils/__init__.py
 -rw-r--r--  2.0 unx      356 b- defN 80-Jan-01 00:00 csvcubed/utils/cache.py
 -rw-r--r--  2.0 unx     2979 b- defN 80-Jan-01 00:00 csvcubed/utils/cli.py
 -rw-r--r--  2.0 unx     6536 b- defN 80-Jan-01 00:00 csvcubed/utils/createlocalcopyresponse.py
--rw-r--r--  2.0 unx    14033 b- defN 80-Jan-01 00:00 csvcubed/utils/csvdataset.py
+-rw-r--r--  2.0 unx    13791 b- defN 80-Jan-01 00:00 csvcubed/utils/csvdataset.py
 -rw-r--r--  2.0 unx     4518 b- defN 80-Jan-01 00:00 csvcubed/utils/csvw.py
 -rw-r--r--  2.0 unx      453 b- defN 80-Jan-01 00:00 csvcubed/utils/datetime.py
 -rw-r--r--  2.0 unx     1488 b- defN 80-Jan-01 00:00 csvcubed/utils/dict.py
 -rw-r--r--  2.0 unx     1682 b- defN 80-Jan-01 00:00 csvcubed/utils/file.py
 -rw-r--r--  2.0 unx     1582 b- defN 80-Jan-01 00:00 csvcubed/utils/iterables.py
 -rw-r--r--  2.0 unx     4253 b- defN 80-Jan-01 00:00 csvcubed/utils/json.py
--rw-r--r--  2.0 unx     3333 b- defN 80-Jan-01 00:00 csvcubed/utils/log.py
+-rw-r--r--  2.0 unx     3348 b- defN 80-Jan-01 00:00 csvcubed/utils/log.py
 -rw-r--r--  2.0 unx     1783 b- defN 80-Jan-01 00:00 csvcubed/utils/pandas.py
 -rw-r--r--  2.0 unx     1169 b- defN 80-Jan-01 00:00 csvcubed/utils/printable.py
 -rw-r--r--  2.0 unx       41 b- defN 80-Jan-01 00:00 csvcubed/utils/qb/__init__.py
 -rw-r--r--  2.0 unx     4228 b- defN 80-Jan-01 00:00 csvcubed/utils/qb/components.py
 -rw-r--r--  2.0 unx     3512 b- defN 80-Jan-01 00:00 csvcubed/utils/qb/cube.py
 -rw-r--r--  2.0 unx     8509 b- defN 80-Jan-01 00:00 csvcubed/utils/qb/standardise.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/utils/qb/validation/__init__.py
 -rw-r--r--  2.0 unx     2983 b- defN 80-Jan-01 00:00 csvcubed/utils/qb/validation/cube.py
 -rw-r--r--  2.0 unx    18273 b- defN 80-Jan-01 00:00 csvcubed/utils/qb/validation/observations.py
 -rw-r--r--  2.0 unx     1672 b- defN 80-Jan-01 00:00 csvcubed/utils/qb/validation/uri_safe.py
 -rw-r--r--  2.0 unx     1945 b- defN 80-Jan-01 00:00 csvcubed/utils/rdf.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/utils/skos/__init__.py
 -rw-r--r--  2.0 unx     3017 b- defN 80-Jan-01 00:00 csvcubed/utils/skos/codelist.py
 -rw-r--r--  2.0 unx       89 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/__init__.py
--rw-r--r--  2.0 unx     6289 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/code_list_inspector.py
+-rw-r--r--  2.0 unx     6301 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/code_list_repository.py
 -rw-r--r--  2.0 unx      955 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/column_component_info.py
--rw-r--r--  2.0 unx     4583 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/csvw_inspector.py
--rw-r--r--  2.0 unx    24662 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/data_cube_inspector.py
--rw-r--r--  2.0 unx     3889 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparql.py
+-rw-r--r--  2.0 unx     4576 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/csvw_repository.py
+-rw-r--r--  2.0 unx    24631 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/data_cube_repository.py
+-rw-r--r--  2.0 unx     3901 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparql.py
 -rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparql_queries/ask_is_codelist.sparql
 -rw-r--r--  2.0 unx       75 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparql_queries/ask_is_qb_dataset.sparql
 -rw-r--r--  2.0 unx     2298 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparql_queries/select_catalog_metadata.sparql
 -rw-r--r--  2.0 unx     1006 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparql_queries/select_codelist_csv_url.sparql
 -rw-r--r--  2.0 unx      482 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparql_queries/select_codelist_primary_key_by_csv_url.sparql
 -rw-r--r--  2.0 unx      969 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparql_queries/select_codelists_and_cols.sparql
 -rw-r--r--  2.0 unx     2149 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparql_queries/select_column_definitions.sparql
 -rw-r--r--  2.0 unx      354 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparql_queries/select_csvw_table_schema_file_dependencies.sparql
 -rw-r--r--  2.0 unx     1188 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparql_queries/select_data_set_dsd_csv_url.sparql
 -rw-r--r--  2.0 unx     1339 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparql_queries/select_dsd_qube_components.sparql
--rw-r--r--  2.0 unx      757 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparql_queries/select_is_pivoted_shape_for_measures_in_data_set.sparql
+-rw-r--r--  2.0 unx      739 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparql_queries/select_is_pivoted_shape_data_set.sparql
 -rw-r--r--  2.0 unx      179 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparql_queries/select_labels_for_resource_uris.sparql
 -rw-r--r--  2.0 unx      379 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparql_queries/select_metadata_dependencies.sparql
 -rw-r--r--  2.0 unx      466 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparql_queries/select_table_schema_properties.sparql
 -rw-r--r--  2.0 unx      367 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparql_queries/select_units.sparql
--rw-r--r--  2.0 unx    11626 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparqlquerymanager.py
--rw-r--r--  2.0 unx     9198 b- defN 80-Jan-01 00:00 csvcubed/utils/tableschema.py
+-rw-r--r--  2.0 unx    11693 b- defN 80-Jan-01 00:00 csvcubed/utils/sparql_handler/sparqlquerymanager.py
+-rw-r--r--  2.0 unx     9203 b- defN 80-Jan-01 00:00 csvcubed/utils/tableschema.py
 -rw-r--r--  2.0 unx      356 b- defN 80-Jan-01 00:00 csvcubed/utils/text.py
 -rw-r--r--  2.0 unx     3467 b- defN 80-Jan-01 00:00 csvcubed/utils/uri.py
 -rw-r--r--  2.0 unx    11239 b- defN 80-Jan-01 00:00 csvcubed/utils/validations.py
 -rw-r--r--  2.0 unx       45 b- defN 80-Jan-01 00:00 csvcubed/utils/validators/__init__.py
 -rw-r--r--  2.0 unx     4360 b- defN 80-Jan-01 00:00 csvcubed/utils/validators/schema.py
 -rw-r--r--  2.0 unx      268 b- defN 80-Jan-01 00:00 csvcubed/utils/version.py
 -rw-r--r--  2.0 unx       62 b- defN 80-Jan-01 00:00 csvcubed/writers/__init__.py
@@ -174,13 +179,13 @@
 -rw-r--r--  2.0 unx    27378 b- defN 80-Jan-01 00:00 csvcubed/writers/helpers/qbwriter/urihelper.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 csvcubed/writers/helpers/skoscodelistwriter/__init__.py
 -rw-r--r--  2.0 unx      157 b- defN 80-Jan-01 00:00 csvcubed/writers/helpers/skoscodelistwriter/constants.py
 -rw-r--r--  2.0 unx     2437 b- defN 80-Jan-01 00:00 csvcubed/writers/helpers/skoscodelistwriter/newresourceurigenerator.py
 -rw-r--r--  2.0 unx    20804 b- defN 80-Jan-01 00:00 csvcubed/writers/qbwriter.py
 -rw-r--r--  2.0 unx     9470 b- defN 80-Jan-01 00:00 csvcubed/writers/skoscodelistwriter.py
 -rw-r--r--  2.0 unx      283 b- defN 80-Jan-01 00:00 csvcubed/writers/writerbase.py
--rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 csvcubed-0.4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3925 b- defN 80-Jan-01 00:00 csvcubed-0.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 csvcubed-0.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       64 b- defN 80-Jan-01 00:00 csvcubed-0.4.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx    18495 b- defN 16-Jan-01 00:00 csvcubed-0.4.1.dist-info/RECORD
-184 files, 787787 bytes uncompressed, 187445 bytes compressed:  76.2%
+-rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 csvcubed-0.4.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3930 b- defN 80-Jan-01 00:00 csvcubed-0.4.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 csvcubed-0.4.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       64 b- defN 80-Jan-01 00:00 csvcubed-0.4.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    18944 b- defN 16-Jan-01 00:00 csvcubed-0.4.2.dist-info/RECORD
+189 files, 810747 bytes uncompressed, 193209 bytes compressed:  76.2%
```

## zipnote {}

```diff
@@ -51,14 +51,29 @@
 
 Filename: csvcubed/definitions.py
 Comment: 
 
 Filename: csvcubed/inputs.py
 Comment: 
 
+Filename: csvcubed/inspect/inspectorcolumns.py
+Comment: 
+
+Filename: csvcubed/inspect/inspectorcomponents.py
+Comment: 
+
+Filename: csvcubed/inspect/inspectors.py
+Comment: 
+
+Filename: csvcubed/inspect/inspectortable.py
+Comment: 
+
+Filename: csvcubed/inspect/lazyfuncdescriptor.py
+Comment: 
+
 Filename: csvcubed/models/__init__.py
 Comment: 
 
 Filename: csvcubed/models/codelistconfig/__init__.py
 Comment: 
 
 Filename: csvcubed/models/codelistconfig/code_list_config.py
@@ -411,24 +426,24 @@
 
 Filename: csvcubed/utils/skos/codelist.py
 Comment: 
 
 Filename: csvcubed/utils/sparql_handler/__init__.py
 Comment: 
 
-Filename: csvcubed/utils/sparql_handler/code_list_inspector.py
+Filename: csvcubed/utils/sparql_handler/code_list_repository.py
 Comment: 
 
 Filename: csvcubed/utils/sparql_handler/column_component_info.py
 Comment: 
 
-Filename: csvcubed/utils/sparql_handler/csvw_inspector.py
+Filename: csvcubed/utils/sparql_handler/csvw_repository.py
 Comment: 
 
-Filename: csvcubed/utils/sparql_handler/data_cube_inspector.py
+Filename: csvcubed/utils/sparql_handler/data_cube_repository.py
 Comment: 
 
 Filename: csvcubed/utils/sparql_handler/sparql.py
 Comment: 
 
 Filename: csvcubed/utils/sparql_handler/sparql_queries/ask_is_codelist.sparql
 Comment: 
@@ -456,15 +471,15 @@
 
 Filename: csvcubed/utils/sparql_handler/sparql_queries/select_data_set_dsd_csv_url.sparql
 Comment: 
 
 Filename: csvcubed/utils/sparql_handler/sparql_queries/select_dsd_qube_components.sparql
 Comment: 
 
-Filename: csvcubed/utils/sparql_handler/sparql_queries/select_is_pivoted_shape_for_measures_in_data_set.sparql
+Filename: csvcubed/utils/sparql_handler/sparql_queries/select_is_pivoted_shape_data_set.sparql
 Comment: 
 
 Filename: csvcubed/utils/sparql_handler/sparql_queries/select_labels_for_resource_uris.sparql
 Comment: 
 
 Filename: csvcubed/utils/sparql_handler/sparql_queries/select_metadata_dependencies.sparql
 Comment: 
@@ -531,23 +546,23 @@
 
 Filename: csvcubed/writers/skoscodelistwriter.py
 Comment: 
 
 Filename: csvcubed/writers/writerbase.py
 Comment: 
 
-Filename: csvcubed-0.4.1.dist-info/LICENSE
+Filename: csvcubed-0.4.2.dist-info/LICENSE
 Comment: 
 
-Filename: csvcubed-0.4.1.dist-info/METADATA
+Filename: csvcubed-0.4.2.dist-info/METADATA
 Comment: 
 
-Filename: csvcubed-0.4.1.dist-info/WHEEL
+Filename: csvcubed-0.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: csvcubed-0.4.1.dist-info/entry_points.txt
+Filename: csvcubed-0.4.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: csvcubed-0.4.1.dist-info/RECORD
+Filename: csvcubed-0.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## csvcubed/cli/inspectcsvw/inspect.py

```diff
@@ -10,17 +10,17 @@
 from pathlib import Path
 from typing import Tuple
 
 from csvcubed.cli.inspectcsvw.metadatainputvalidator import MetadataValidator
 from csvcubed.cli.inspectcsvw.metadataprinter import MetadataPrinter
 from csvcubed.models.csvcubedexception import FailedToLoadRDFGraphException
 from csvcubed.models.csvwtype import CSVWType
-from csvcubed.utils.sparql_handler.code_list_inspector import CodeListInspector
-from csvcubed.utils.sparql_handler.csvw_inspector import CsvWInspector
-from csvcubed.utils.sparql_handler.data_cube_inspector import DataCubeInspector
+from csvcubed.utils.sparql_handler.code_list_repository import CodeListRepository
+from csvcubed.utils.sparql_handler.csvw_repository import CsvWRepository
+from csvcubed.utils.sparql_handler.data_cube_repository import DataCubeRepository
 from csvcubed.utils.tableschema import CsvWRdfManager
 
 _logger = logging.getLogger(__name__)
 
 
 def inspect(csvw_metadata_json_path: Path) -> None:
     """
@@ -48,15 +48,15 @@
         catalog_metadata_printable,
         codelist_info_printable,
         dataset_observations_printable,
         val_counts_by_measure_unit_printable,
         codelist_hierarchy_info_printable,
         column_component_info_printable,
     ) = _generate_printables(
-        csvw_rdf_manager.csvw_inspector,
+        csvw_rdf_manager.csvw_repository,
     )
 
     print(f"{linesep}{type_printable}")
     print(f"{linesep}{catalog_metadata_printable}")
     if csvw_type == CSVWType.QbDataSet:
         print(f"{linesep}{column_component_info_printable}")
         print(f"{linesep}{codelist_info_printable}")
@@ -64,32 +64,32 @@
     if csvw_type == CSVWType.QbDataSet:
         print(f"{linesep}{val_counts_by_measure_unit_printable}")
     if csvw_type == CSVWType.CodeList:
         print(f"{linesep}{codelist_hierarchy_info_printable}")
 
 
 def _generate_printables(
-    csvw_inspector: CsvWInspector,
+    csvw_repository: CsvWRepository,
 ) -> Tuple[str, str, str, str, str, str, str]:
     """
     Generates printables of type, metadata, dsd, code list, head/tail and value count information.
 
     Member of :file:`./inspect.py`
 
     :return: `Tuple[str, str, str, str, str]` - printables of metadata information.
     """
     metadata_printer: MetadataPrinter
 
-    csvw_type = csvw_inspector.csvw_type
+    csvw_type = csvw_repository.csvw_type
 
     if csvw_type == CSVWType.QbDataSet:
-        data_cube_inspector = DataCubeInspector(csvw_inspector)
-        metadata_printer = MetadataPrinter(data_cube_inspector)
+        data_cube_repository = DataCubeRepository(csvw_repository)
+        metadata_printer = MetadataPrinter(data_cube_repository)
     else:
-        code_list_state = CodeListInspector(csvw_inspector)
+        code_list_state = CodeListRepository(csvw_repository)
         metadata_printer = MetadataPrinter(code_list_state)
 
     type_info_printable: str = metadata_printer.type_info_printable
     catalog_metadata_printable: str = metadata_printer.catalog_metadata_printable
     column_component_info_printable: str = (
         metadata_printer.column_component_info_printable
         if csvw_type == CSVWType.QbDataSet
```

## csvcubed/cli/inspectcsvw/metadataprinter.py

```diff
@@ -43,27 +43,27 @@
     get_printable_tabular_str_from_list,
 )
 from csvcubed.utils.skos.codelist import (
     CodelistPropertyUrl,
     get_codelist_col_title_by_property_url,
     get_codelist_col_title_from_col_name,
 )
-from csvcubed.utils.sparql_handler.code_list_inspector import CodeListInspector
+from csvcubed.utils.sparql_handler.code_list_repository import CodeListRepository
 from csvcubed.utils.sparql_handler.column_component_info import ColumnComponentInfo
-from csvcubed.utils.sparql_handler.csvw_inspector import CsvWInspector
-from csvcubed.utils.sparql_handler.data_cube_inspector import DataCubeInspector
+from csvcubed.utils.sparql_handler.csvw_repository import CsvWRepository
+from csvcubed.utils.sparql_handler.data_cube_repository import DataCubeRepository
 
 
 @dataclass
 class MetadataPrinter:
     """
     This class produces the printables necessary for producing outputs to the CLI.
     """
 
-    state: Union[DataCubeInspector, CodeListInspector]
+    state: Union[DataCubeRepository, CodeListRepository]
 
     csvw_type_str: str = field(init=False)
     primary_csv_url: str = field(init=False)
     dataset: DataFrame = field(init=False)
 
     result_catalog_metadata: CatalogMetadataResult = field(init=False)
     result_column_component_infos: List[ColumnComponentInfo] = field(init=False)
@@ -75,36 +75,36 @@
         init=False
     )
     result_code_list_cols: List[ColumnDefinition] = field(init=False)
     result_concepts_hierachy_info: CodelistHierarchyInfoResult = field(init=False)
 
     def __post_init__(self):
         self.generate_general_results()
-        if self.state.csvw_inspector.csvw_type == CSVWType.QbDataSet:
+        if self.state.csvw_repository.csvw_type == CSVWType.QbDataSet:
             self.get_datacube_results()
-        elif self.state.csvw_inspector.csvw_type == CSVWType.CodeList:
+        elif self.state.csvw_repository.csvw_type == CSVWType.CodeList:
             self.generate_codelist_results()
 
     @staticmethod
     def get_csvw_type_str(csvw_type: CSVWType) -> str:
         if csvw_type == CSVWType.QbDataSet:
             return "data cube"
         elif csvw_type == CSVWType.CodeList:
             return "code list"
         else:
             raise InputNotSupportedException()
 
     def get_primary_csv_url(self) -> str:
         """Return the csv_url for the primary table in the graph."""
-        primary_metadata = self.state.csvw_inspector.get_primary_catalog_metadata()
-        if isinstance(self.state, DataCubeInspector):
+        primary_metadata = self.state.csvw_repository.get_primary_catalog_metadata()
+        if isinstance(self.state, DataCubeRepository):
             return self.state.get_cube_identifiers_for_data_set(
                 primary_metadata.dataset_uri
             ).csv_url
-        elif isinstance(self.state, CodeListInspector):
+        elif isinstance(self.state, CodeListRepository):
             return self.state.get_table_identifiers_for_concept_scheme(
                 primary_metadata.dataset_uri
             ).csv_url
         else:
             raise InputNotSupportedException()
 
     @staticmethod
@@ -125,45 +125,45 @@
 
     def generate_general_results(self):
         """
         Generates results related to data cubes and code lists.
 
         Member of :class:`./MetadataPrinter`.
         """
-        csvw_inspector = self.state.csvw_inspector
-        csvw_type = csvw_inspector.csvw_type
+        csvw_repository = self.state.csvw_repository
+        csvw_type = csvw_repository.csvw_type
 
         self.csvw_type_str = self.get_csvw_type_str(csvw_type)
-        self.result_catalog_metadata = csvw_inspector.get_primary_catalog_metadata()
+        self.result_catalog_metadata = csvw_repository.get_primary_catalog_metadata()
         self.primary_csv_url = self.get_primary_csv_url()
         self.dataset = load_csv_to_dataframe(
-            csvw_inspector.csvw_json_path, Path(self.primary_csv_url)
+            csvw_repository.csvw_json_path, Path(self.primary_csv_url)
         )
         self.result_dataset_observations_info = get_dataset_observations_info(
             self.dataset,
             csvw_type,
             self.state.get_shape_for_csv(self.primary_csv_url)
-            if isinstance(self.state, DataCubeInspector)
+            if isinstance(self.state, DataCubeRepository)
             else None,
         )
 
     def get_datacube_results(self):
         """
         Generates results specific to data cubes.
 
         Member of :class:`./MetadataPrinter`.
         """
-        assert isinstance(self.state, DataCubeInspector)  # Make pyright happier
+        assert isinstance(self.state, DataCubeRepository)  # Make pyright happier
 
         self.primary_cube_table_identifiers = self.state.get_cube_identifiers_for_csv(
             self.primary_csv_url
         )
 
         self.primary_csv_column_definitions = (
-            self.state.csvw_inspector.get_column_definitions_for_csv(
+            self.state.csvw_repository.get_column_definitions_for_csv(
                 self.primary_csv_url
             )
         )
         self.result_column_component_infos = self.state.get_column_component_info(
             self.primary_csv_url
         )
         self.result_primary_csv_code_lists = self.state.get_code_lists_and_cols(
@@ -188,20 +188,20 @@
 
     def generate_codelist_results(self):
         """
         Generates results specific to code lists.
 
         Member of :class:`./MetadataPrinter`.
         """
-        csvw_inspector = self.state.csvw_inspector
-        self.result_code_list_cols = csvw_inspector.get_column_definitions_for_csv(
+        csvw_repository = self.state.csvw_repository
+        self.result_code_list_cols = csvw_repository.get_column_definitions_for_csv(
             self.primary_csv_url
         )
         # Retrieving the primary key column names of the code list to identify the unique identifier
-        result_table_schema_properties = csvw_inspector.get_table_info_for_csv_url(
+        result_table_schema_properties = csvw_repository.get_table_info_for_csv_url(
             self.primary_csv_url
         )
 
         primary_key_col_names = result_table_schema_properties.primary_key_col_names
 
         # Currently, we do not support composite primary keys.
         if len(primary_key_col_names) != 1:
@@ -252,15 +252,15 @@
         """
         Returns a printable of file content type.
 
         Member of :class:`./MetadataPrinter`.
 
         :return: `str` - user-friendly string which will be output to CLI.
         """
-        if self.state.csvw_inspector.csvw_type == CSVWType.QbDataSet:
+        if self.state.csvw_repository.csvw_type == CSVWType.QbDataSet:
             return "- This file is a data cube."
         else:
             return "- This file is a code list."
 
     @property
     def column_component_info_printable(self) -> str:
         """
@@ -294,15 +294,43 @@
         """
         Returns a printable of catalog metadata (e.g. title, description).
 
         Member of :class:`./MetadataPrinter`.
 
         :return: `str` - user-friendly string which will be output to CLI.
         """
-        return f"- The {self.csvw_type_str} has the following catalog metadata:{self.result_catalog_metadata.output_str}"
+        formatted_landing_pages: str = get_printable_list_str(
+            self.result_catalog_metadata.landing_pages
+        )
+        formatted_themes: str = get_printable_list_str(
+            self.result_catalog_metadata.themes
+        )
+        formatted_keywords: str = get_printable_list_str(
+            self.result_catalog_metadata.keywords
+        )
+        formatted_description: str = self.result_catalog_metadata.description.replace(
+            linesep, f"{linesep}\t\t"
+        )
+        return f"""
+        - The {self.csvw_type_str} has the following catalog metadata:
+          - Title: {self.result_catalog_metadata.title}
+          - Label: {self.result_catalog_metadata.label}
+          - Issued: {self.result_catalog_metadata.issued}
+          - Modified: {self.result_catalog_metadata.modified}
+          - License: {self.result_catalog_metadata.license}
+          - Creator: {self.result_catalog_metadata.creator}
+          - Publisher: {self.result_catalog_metadata.publisher}
+          - Landing Pages: {formatted_landing_pages}
+          - Themes: {formatted_themes}
+          - Keywords: {formatted_keywords}
+          - Contact Point: {self.result_catalog_metadata.contact_point}
+          - Identifier: {self.result_catalog_metadata.identifier}
+          - Comment: {self.result_catalog_metadata.comment}
+          - Description: {formatted_description}
+        """
 
     @property
     def codelist_info_printable(self) -> str:
         """
         Returns a printable of data structure definition (DSD) code list information (e.g. column name, type, etc.).
 
         Member of :class:`./MetadataPrinter`.
```

## csvcubed/models/sparqlresults.py

```diff
@@ -1,26 +1,24 @@
 """
 SPARQL query results
 ----------------------------
 """
 
 import logging
 from dataclasses import dataclass
-from os import linesep
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 import uritemplate
 from csvcubedmodels.dataclassbase import DataClassBase
 from rdflib.query import ResultRow
 
 from csvcubed.definitions import QB_MEASURE_TYPE_DIMENSION_URI
 from csvcubed.models.cube.cube_shape import CubeShape
 from csvcubed.utils.iterables import first, group_by, single
-from csvcubed.utils.printable import get_printable_list_str
 from csvcubed.utils.qb.components import (
     ComponentPropertyType,
     get_component_property_as_relative_path,
     get_component_property_type,
 )
 from csvcubed.utils.sparql_handler.sparql import none_or_map
 
@@ -30,17 +28,17 @@
 @dataclass
 class CatalogMetadataResult:
     """
     Model to represent select catalog metadata sparql query result.
     """
 
     dataset_uri: str
-    """Data set here doesn't necessarily mean the qb:DataSet. It means eiither the qb:DataSet or the skos:ConceptScheme."""
+    """Data set here doesn't necessarily mean the qb:DataSet. It means either the qb:DataSet or the skos:ConceptScheme."""
     graph_uri: str
-    """URI representing the grapgh in which the Catalog Metadata was found."""
+    """URI representing the graph in which the Catalog Metadata was found."""
     title: str
     label: str
     issued: str
     modified: str
     license: str
     creator: str
     publisher: str
@@ -48,37 +46,14 @@
     themes: list[str]
     keywords: list[str]
     contact_point: str
     identifier: str
     comment: str
     description: str
 
-    @property
-    def output_str(self) -> str:
-        formatted_landing_pages: str = get_printable_list_str(self.landing_pages)
-        formatted_themes: str = get_printable_list_str(self.themes)
-        formatted_keywords: str = get_printable_list_str(self.keywords)
-        formatted_description: str = self.description.replace(linesep, f"{linesep}\t\t")
-        return f"""
-        - Title: {self.title}
-        - Label: {self.label}
-        - Issued: {self.issued}
-        - Modified: {self.modified}
-        - License: {self.license}
-        - Creator: {self.creator}
-        - Publisher: {self.publisher}
-        - Landing Pages: {formatted_landing_pages}
-        - Themes: {formatted_themes}
-        - Keywords: {formatted_keywords}
-        - Contact Point: {self.contact_point}
-        - Identifier: {self.identifier}
-        - Comment: {self.comment}
-        - Description: {formatted_description}
-        """
-
 
 @dataclass
 class CubeTableIdentifiers(DataClassBase):
     """
     Links the CSV URL, DataSet URL, DataSet Label and DataStructureDefinition URI for a given cube.
     """
 
@@ -135,53 +110,23 @@
     """
 
     unit_uri: str
     unit_label: str
 
 
 @dataclass
-class CodelistColumnResult(DataClassBase):
-    """
-    Model to represent a codelist column.
-    """
-
-    column_property_url: Optional[str]
-    column_value_url: Optional[str]
-    column_title: Optional[str]
-    column_name: Optional[str]
-
-
-@dataclass
-class CodeListColsByDatasetUrlResult:
-    """
-    Model to represent select codelist columns by table url.
-    """
-
-    columns: List[CodelistColumnResult]
-
-
-@dataclass
 class PrimaryKeyColNameByDatasetUrlResult:
     """
     Model to represent select primary key column name by table url.
     """
 
     value: str
 
 
 @dataclass
-class PrimaryKeyColNamesByDatasetUrlResult:
-    """
-    Model to represent select primary keys by table url.
-    """
-
-    primary_key_col_names: List[PrimaryKeyColNameByDatasetUrlResult]
-
-
-@dataclass
 class MetadataDependenciesResult:
     """
     Model representing a metadata dependency which should be loaded to make sense of the current graph.
     """
 
     data_set: str
     data_dump: str
@@ -196,22 +141,20 @@
 
     about_url: str
     csv_url: str
     primary_key_col_names: List[str]
 
 
 @dataclass
-class IsPivotedShapeMeasureResult:
+class IsPivotedShapeResult:
     """
-    A dataclass that is used to return the measure of from a cube's metadata and whether that measure is part of a
-    pivoted or standard shape cube.
+    A dataclass that is used to return whether a cube is in pivoted or standard shape.
     """
 
     csv_url: str
-    measure: str
     is_pivoted_shape: bool
 
 
 @dataclass(unsafe_hash=True)
 class ColumnDefinition:
     """
     Model representing the Column Titles and Column Names of a data set.
@@ -256,15 +199,15 @@
 
 @dataclass
 class QubeComponentsResult:
     """
     Model to represent select qube components sparql query result.
     """
 
-    qube_components: list[QubeComponentResult]
+    qube_components: List[QubeComponentResult]
     num_components: int
 
 
 @dataclass
 class ResourceURILabelResult:
     """
     Model to represent a resource attribute's URI and label.
@@ -565,32 +508,28 @@
         value=str(result_dict["tablePrimaryKey"]),
     )
     return result
 
 
 def map_primary_key_col_names_by_csv_url_result(
     sparql_results: List[ResultRow],
-) -> PrimaryKeyColNamesByDatasetUrlResult:
+) -> List[PrimaryKeyColNameByDatasetUrlResult]:
     """
     Maps sparql query result to `PrimaryKeyColNamesByDatasetUrlResult`
 
     Member of :file:`./models/sparqlresults.py`
 
     :return: `PrimaryKeyColNamesByDatasetUrlResult`
     """
-    primary_key_col_names = list(
+    return list(
         map(
             lambda result: _map_primary_key_col_name_by_csv_url_result(result),
             sparql_results,
         )
     )
-    result = PrimaryKeyColNamesByDatasetUrlResult(
-        primary_key_col_names=primary_key_col_names
-    )
-    return result
 
 
 def map_metadata_dependency_results(
     sparql_results: List[ResultRow],
 ) -> List[MetadataDependenciesResult]:
     def map_row(row_result: Dict[str, Any]) -> MetadataDependenciesResult:
         return MetadataDependenciesResult(
@@ -619,25 +558,24 @@
             csv_url=str(row_result["csvUrl"]),
             primary_key_col_names=str(row_result["tablePrimaryKeys"]).split("|"),
         )
 
     return [map_row(row.asdict()) for row in sparql_results]
 
 
-def map_is_pivoted_shape_for_measures_in_data_set(
+def map_is_pivoted_shape_data_set(
     sparql_results: List[ResultRow],
-) -> List[IsPivotedShapeMeasureResult]:
+) -> List[IsPivotedShapeResult]:
     """
-    Maps the sparql query result to objects of type IsPivotedMeasureResult that are then returned.
+    Maps the sparql query result to objects of type IsPivotedShapeResult that are then returned.
     """
 
-    def map_row(row_result: Dict[str, Any]) -> IsPivotedShapeMeasureResult:
-        return IsPivotedShapeMeasureResult(
+    def map_row(row_result: Dict[str, Any]) -> IsPivotedShapeResult:
+        return IsPivotedShapeResult(
             csv_url=str(row_result["csvUrl"]),
-            measure=str(row_result["measure"]),
             is_pivoted_shape=bool(row_result["isPivotedShape"]),
         )
 
     return [map_row(row.asdict()) for row in sparql_results]
 
 
 def map_labels_for_resource_uris(
```

## csvcubed/utils/csvdataset.py

```diff
@@ -3,43 +3,39 @@
 -----------
 
 Utilities for CSV Datasets
 """
 
 import logging
 from pathlib import Path
-from typing import Any, Dict, List, Set, Tuple, Optional
+from typing import Any, Dict, List, Optional, Set, Tuple
 from uuid import uuid1
 
 import pandas as pd
 import uritemplate
 from csvcubedmodels.rdf.namespaces import SDMX_Attribute
 from uritemplate.orderedset import OrderedSet
 
-from csvcubed.models.csvcubedexception import InvalidNumberOfRecordsException
-from csvcubed.models.inspectdataframeresults import DatasetSingleMeasureResult
-from csvcubed.models.sparqlresults import QubeComponentResult
-from csvcubed.utils.iterables import first
-from csvcubed.utils.qb.components import (
-    ComponentField,
-    ComponentPropertyAttributeURI,
-    ComponentPropertyType,
-    get_component_property_as_relative_path,
-)
 from csvcubed.models.csvcubedexception import (
     InvalidNumberOfRecordsException,
     InvalidNumOfDSDComponentsForObsValColTitleException,
     InvalidObservationColumnTitle,
     InvalidUnitColumnDefinition,
 )
 from csvcubed.models.cube.cube_shape import CubeShape
+from csvcubed.models.inspectdataframeresults import DatasetSingleMeasureResult
 from csvcubed.models.sparqlresults import ColumnDefinition, QubeComponentResult
 from csvcubed.utils.iterables import first
-from csvcubed.utils.qb.components import ComponentField, ComponentPropertyType
-from csvcubed.utils.sparql_handler.data_cube_inspector import DataCubeInspector
+from csvcubed.utils.qb.components import (
+    ComponentField,
+    ComponentPropertyAttributeURI,
+    ComponentPropertyType,
+    get_component_property_as_relative_path,
+)
+from csvcubed.utils.sparql_handler.data_cube_repository import DataCubeRepository
 
 _logger = logging.getLogger(__name__)
 
 
 def filter_components_from_dsd(
     components: List[QubeComponentResult],
     field: ComponentField,
@@ -174,15 +170,15 @@
     return uritemplate.expand(unit_col_value_url, col_name_value_map)
 
 
 def _create_unit_col_in_melted_data_set_for_pivoted_shape(
     col_name: str,
     melted_df: pd.DataFrame,
     column_definitions: List[ColumnDefinition],
-    data_cube_inspector: DataCubeInspector,
+    data_cube_repository: DataCubeRepository,
     measure_uris: Set[str],
 ):
     """
     Adds the unit column to the melted data set for the pivoted shape data set input.
     """
     # Creating a new column in pandas dataframe with empty values.
     melted_df[col_name] = ""
@@ -218,15 +214,15 @@
                 about_url=observed_value_column.about_url or "None",
                 num_of_value_urls=0,
             )
 
         unit_uri = _get_unit_uri_for_maybe_template(
             unit_column.value_url, column_definitions, row
         )
-        maybe_unit = data_cube_inspector.get_unit_for_uri(unit_uri)
+        maybe_unit = data_cube_repository.get_unit_for_uri(unit_uri)
         if maybe_unit is None:
             melted_df.loc[idx, col_name] = unit_uri
         else:
             melted_df.loc[idx, col_name] = maybe_unit.unit_label
 
 
 def _get_unit_uri_for_maybe_template(
@@ -318,22 +314,22 @@
         value_name="Value",
         var_name="Observation Value",
     )
 
 
 def _get_unit_measure_col_for_standard_shape_cube(
     qube_components: List[QubeComponentResult],
-    data_cube_inspector: DataCubeInspector,
+    data_cube_repository: DataCubeRepository,
     canonical_shape_dataset: pd.DataFrame,
     csvw_metadata_json_path: Path,
 ) -> Tuple[pd.DataFrame, str, str]:
     unit_col_retrived = get_standard_shape_unit_col_name_from_dsd(qube_components)
     if unit_col_retrived is None:
         unit_col = f"Unit_{str(uuid1())}"
-        units = data_cube_inspector.get_units()
+        units = data_cube_repository.get_units()
         if len(units) != 1:
             raise InvalidNumberOfRecordsException(
                 record_description=f"result for the `get_units()` function call",
                 excepted_num_of_records=1,
                 num_of_records=len(units),
             )
         unit = units[0]
@@ -354,23 +350,23 @@
         measure_col = measure_col_retrived
 
     return (canonical_shape_dataset, measure_col, unit_col)
 
 
 def _melt_pivoted_shape(
     csv_url: str,
-    data_cube_inspector: DataCubeInspector,
+    data_cube_repository: DataCubeRepository,
     qube_components: List[QubeComponentResult],
     canonical_shape_dataset: pd.DataFrame,
 ) -> Tuple[pd.DataFrame, str, str]:
     if csv_url is None:
         raise ValueError("csv_url cannot be None.")
 
     column_definitions = (
-        data_cube_inspector.csvw_inspector.get_column_definitions_for_csv(csv_url)
+        data_cube_repository.csvw_repository.get_column_definitions_for_csv(csv_url)
     )
 
     measure_components = filter_components_from_dsd(
         qube_components,
         ComponentField.PropertyType,
         ComponentPropertyType.Measure.value,
     )
@@ -384,44 +380,44 @@
 
     measure_col = f"Measure_{str(uuid1())}"
     unit_col = f"Unit_{str(uuid1())}"
     _create_measure_col_in_melted_data_set_for_pivoted_shape(
         measure_col, melted_df, measure_components
     )
     _create_unit_col_in_melted_data_set_for_pivoted_shape(
-        unit_col, melted_df, column_definitions, data_cube_inspector, measure_uris
+        unit_col, melted_df, column_definitions, data_cube_repository, measure_uris
     )
 
     canonical_shape_dataset = melted_df.drop("Observation Value", axis=1)
 
     return (canonical_shape_dataset, measure_col, unit_col)
 
 
 def transform_dataset_to_canonical_shape(
-    data_cube_inspector: DataCubeInspector,
+    data_cube_repository: DataCubeRepository,
     dataset: pd.DataFrame,
     csv_url: str,
     qube_components: List[QubeComponentResult],
 ) -> Tuple[pd.DataFrame, str, str]:
     """
     Transforms the given dataset into canonical shape if it is not in the canonical shape already.
 
     Member of :class:`./csvdataset`.
 
     :return: `Tuple[pd.DataFrame, str, str]` - canonical dataframe, measure column name, unit column name.
     """
     canonical_shape_dataset = dataset.copy()
 
-    cube_shape = data_cube_inspector.get_shape_for_csv(csv_url)
+    cube_shape = data_cube_repository.get_shape_for_csv(csv_url)
 
     if cube_shape == CubeShape.Standard:
         return _get_unit_measure_col_for_standard_shape_cube(
             qube_components,
-            data_cube_inspector,
+            data_cube_repository,
             canonical_shape_dataset,
-            data_cube_inspector.csvw_inspector.csvw_json_path,
+            data_cube_repository.csvw_repository.csvw_json_path,
         )
     else:
         # In pivoted shape
         return _melt_pivoted_shape(
-            csv_url, data_cube_inspector, qube_components, canonical_shape_dataset
+            csv_url, data_cube_repository, qube_components, canonical_shape_dataset
         )
```

## csvcubed/utils/log.py

```diff
@@ -7,15 +7,15 @@
 import logging
 import logging.handlers
 import sys
 import traceback
 from pathlib import Path
 from typing import Union
 
-from appdirs import AppDirs
+from platformdirs import PlatformDirs
 
 
 class CustomFormatter(logging.Formatter):
     grey = "\x1b[2;20m"
     light_grey = "\x1b[1;50m"
     yellow = "\x1b[33;20m"
     red = "\x1b[31;20m"
@@ -40,15 +40,15 @@
 
 
 def start_logging(
     log_dir_name: str, selected_logging_level: Union[str, int, None]
 ) -> None:
     logging_level = _get_logging_level(selected_logging_level)
 
-    dirs = AppDirs(log_dir_name, "csvcubed")
+    dirs = PlatformDirs(log_dir_name, "csvcubed")
     log_file_path = Path(dirs.user_log_dir) / "out.log"
     log_file_path.parent.mkdir(parents=True, exist_ok=True)
 
     logger = logging.getLogger()
     logger.setLevel(logging_level)
 
     console_handler = logging.StreamHandler(sys.stderr)
```

## csvcubed/utils/sparql_handler/sparql.py

```diff
@@ -7,15 +7,15 @@
 import os.path
 from pathlib import Path, PosixPath
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import rdflib.term
 from rdflib import Graph, Literal
 from rdflib.query import ResultRow
-from rdflib.term import Node
+from rdflib.term import Identifier
 
 from csvcubed.models.csvcubedexception import (
     UnexpectedSparqlAskQueryResponseTypeException,
     UnexpectedSparqlAskQueryResultsException,
 )
 from csvcubed.models.sparql.valuesbinding import ValuesBinding
 
@@ -48,15 +48,15 @@
     else:
         raise UnexpectedSparqlAskQueryResultsException(query_name, len(results))
 
 
 def select(
     query: str,
     graph: Graph,
-    init_bindings: Optional[Dict[str, Node]] = None,
+    init_bindings: Optional[Dict[str, Identifier]] = None,
     values_bindings: List[ValuesBinding] = [],
 ) -> List[ResultRow]:
     """
     Executes the given SELECT query on the rdf graph.
 
     Member of :file:`./sparql.py`.
```

## csvcubed/utils/sparql_handler/sparqlquerymanager.py

```diff
@@ -24,26 +24,26 @@
 from csvcubed.models.sparql.valuesbinding import ValuesBinding
 from csvcubed.models.sparqlresults import (
     CatalogMetadataResult,
     CodelistsResult,
     ColumnDefinition,
     CSVWTableSchemaFileDependenciesResult,
     CubeTableIdentifiers,
-    IsPivotedShapeMeasureResult,
+    IsPivotedShapeResult,
     MetadataDependenciesResult,
-    PrimaryKeyColNamesByDatasetUrlResult,
+    PrimaryKeyColNameByDatasetUrlResult,
     QubeComponentsResult,
     TableSchemaPropertiesResult,
     UnitResult,
     map_catalog_metadata_results,
     map_codelists_sparql_result,
     map_column_definition_results,
     map_csvw_table_schemas_file_dependencies_result,
     map_data_set_dsd_csv_url_result,
-    map_is_pivoted_shape_for_measures_in_data_set,
+    map_is_pivoted_shape_data_set,
     map_labels_for_resource_uris,
     map_metadata_dependency_results,
     map_primary_key_col_names_by_csv_url_result,
     map_qube_components_sparql_result,
     map_table_schema_properties_results,
     map_units,
 )
@@ -79,17 +79,15 @@
 
     SELECT_CODELIST_PRIMARY_KEY_BY_CSV_URL = "select_codelist_primary_key_by_csv_url"
 
     SELECT_METADATA_DEPENDENCIES = "select_metadata_dependencies"
 
     SELECT_TABLE_SCHEMA_PROPERTIES = "select_table_schema_properties"
 
-    SELECT_IS_PIVOTED_SHAPE_FOR_MEASURES_IN_DATA_SET = (
-        "select_is_pivoted_shape_for_measures_in_data_set"
-    )
+    SELECT_IS_PIVOTED_SHAPE_DATA_SET = "select_is_pivoted_shape_data_set"
 
     SELECT_COLUMN_DEFINITIONS = "select_column_definitions"
 
     SELECT_LABELS_FOR_RESOURCE_URIS = "select_labels_for_resource_uris"
 
 
 def _get_query_string_from_file(query_type: SPARQLQueryName) -> str:
@@ -157,29 +155,33 @@
     rdf_graph: rdflib.Graph,
 ) -> List[CatalogMetadataResult]:
     """
     Queries catalog metadata such as title, label, issued date/time, modified data/time, etc.
 
     Member of :file:`./sparqlquerymanager.py`
 
-    :return: `CatalogMetadataResult`
+    :return: `List[CatalogMetadataResult]`
     """
     results: List[ResultRow] = select(
         _get_query_string_from_file(SPARQLQueryName.SELECT_CATALOG_METADATA),
         rdf_graph,
     )
 
     return map_catalog_metadata_results(results)
 
 
 def select_data_set_dsd_and_csv_url(
     rdf_graph: rdflib.ConjunctiveGraph,
 ) -> List[CubeTableIdentifiers]:
     """
     Selects the dataset's DSD and CSV URL. Returns a list of cube table identifiers containing the results.
+
+    Member of :file:`./sparqlquerymanager.py`
+
+    :return: `List[CubeTableIdentifiers]`
     """
     results: List[ResultRow] = select(
         _get_query_string_from_file(SPARQLQueryName.SELECT_DATA_SET_DSD_CSV_URL),
         rdf_graph,
     )
 
     if len(results) == 0:
@@ -195,17 +197,15 @@
     rdf_graph: rdflib.ConjunctiveGraph,
     json_path: Path,
     map_dsd_uri_to_csv_url: Dict[str, str],
     map_csv_url_to_column_definitions: Dict[str, List[ColumnDefinition]],
     map_csv_url_to_cube_shape: Dict[str, CubeShape],
 ) -> Dict[str, QubeComponentsResult]:
     """
-    Queries the list of qube components.
-
-    Returns a map of csv_url to the `QubeComponentsResult`.
+    Queries the list of qube components. Returns a map of csv_url to the `QubeComponentsResult`.
 
     Member of :file:`./sparqlquerymanager.py`
 
     :return: `Dict[str, QubeComponentsResult]`
     """
     result_dsd_components: List[ResultRow] = select(
         _get_query_string_from_file(SPARQLQueryName.SELECT_DSD_QUBE_COMPONENTS),
@@ -217,32 +217,34 @@
         json_path,
         map_dsd_uri_to_csv_url,
         map_csv_url_to_column_definitions,
         map_csv_url_to_cube_shape,
     )
 
 
-def select_is_pivoted_shape_for_measures_in_data_set(
+def select_is_pivoted_shape_data_set(
     rdf_graph: rdflib.ConjunctiveGraph,
     cube_table_identifiers: List[CubeTableIdentifiers],
-) -> List[IsPivotedShapeMeasureResult]:
+) -> List[IsPivotedShapeResult]:
     """
     Queries the measure and whether it is a part of a pivoted or standard shape cube.
+
+    Member of :file:`./sparqlquerymanager.py`
+
+    :return: `List[IsPivotedShapeMeasureResult]`
     """
     result_is_pivoted_shape: List[ResultRow] = select(
-        _get_query_string_from_file(
-            SPARQLQueryName.SELECT_IS_PIVOTED_SHAPE_FOR_MEASURES_IN_DATA_SET
-        ),
+        _get_query_string_from_file(SPARQLQueryName.SELECT_IS_PIVOTED_SHAPE_DATA_SET),
         rdf_graph,
         values_bindings=[
             _cube_table_identifiers_to_values_binding(cube_table_identifiers)
         ],
     )
 
-    return map_is_pivoted_shape_for_measures_in_data_set(result_is_pivoted_shape)
+    return map_is_pivoted_shape_data_set(result_is_pivoted_shape)
 
 
 def _cube_table_identifiers_to_values_binding(
     csv_dsd_dataset_uris: List[CubeTableIdentifiers],
 ) -> ValuesBinding:
     return ValuesBinding(
         variable_names=["csvUrl", "dataSet", "dsd"],
@@ -263,15 +265,15 @@
     )
 
 
 def select_labels_for_resource_uris(
     rdf_graph: rdflib.ConjunctiveGraph, resource_uris: List[str]
 ) -> Dict[str, str]:
     """
-    Queries a list of value uris and returns associated labels
+    Queries a list of value uris and returns associated labels.
 
     Member of :file:`./sparqlquerymanager.py`
 
     :return: `Dict[str, str]`
     """
     results: List[ResultRow] = select(
         _get_query_string_from_file(SPARQLQueryName.SELECT_LABELS_FOR_RESOURCE_URIS),
@@ -287,15 +289,15 @@
     json_path: Path,
 ) -> Dict[str, CodelistsResult]:
     """
     Queries code lists and columns in the data cube.
 
     Member of :file:`./sparqlquerymanager.py`
 
-    :return: `CodelistInfoSparqlResult`
+    :return: `Dict[str, CodelistsResult]`
     """
     results: List[ResultRow] = select(
         _get_query_string_from_file(SPARQLQueryName.SELECT_CODELISTS_AND_COLS),
         rdf_graph,
     )
     return map_codelists_sparql_result(results, json_path)
 
@@ -304,15 +306,15 @@
     rdf_graph: rdflib.ConjunctiveGraph,
 ) -> CSVWTableSchemaFileDependenciesResult:
     """
     Queries the table schemas of the given csvw json-ld.
 
     Member of :file:`./sparqlquerymanager.py`
 
-    :return: `CSVWTabelSchemasResult`
+    :return: `CSVWTableSchemaFileDependenciesResult`
     """
     results: List[ResultRow] = select(
         _get_query_string_from_file(
             SPARQLQueryName.SELECT_CSVW_TABLE_SCHEMA_FILE_DEPENDENCIES
         ),
         rdf_graph,
     )
@@ -334,21 +336,21 @@
     )
 
     return map_units(results)
 
 
 def select_primary_key_col_names_by_csv_url(
     rdf_graph: rdflib.ConjunctiveGraph, table_url: str
-) -> PrimaryKeyColNamesByDatasetUrlResult:
+) -> List[PrimaryKeyColNameByDatasetUrlResult]:
     """
     Queries the primary keys for the given table url.
 
     Member of :file:`./sparqlquerymanager.py`
 
-    :return: `PrimaryKeyColNamesByDatasetUrlResult`
+    :return: `List[PrimaryKeyColNameByDatasetUrlResult]`
     """
     results: List[ResultRow] = select(
         _get_query_string_from_file(
             SPARQLQueryName.SELECT_CODELIST_PRIMARY_KEY_BY_CSV_URL
         ),
         rdf_graph,
         init_bindings={"table_url": Literal(table_url)},
```

## csvcubed/utils/tableschema.py

```diff
@@ -18,15 +18,15 @@
     FailedToLoadRDFGraphException,
     FailedToLoadTableSchemaIntoRdfGraphException,
     FailedToReadCsvwFileContentException,
     InvalidCsvwFileContentException,
 )
 from csvcubed.utils.csvw import load_table_schema_file_to_graph
 from csvcubed.utils.rdf import parse_graph_retain_relative
-from csvcubed.utils.sparql_handler.csvw_inspector import CsvWInspector
+from csvcubed.utils.sparql_handler.csvw_repository import CsvWRepository
 from csvcubed.utils.sparql_handler.sparql import path_to_file_uri_for_rdflib
 from csvcubed.utils.sparql_handler.sparqlquerymanager import (
     select_csvw_table_schema_file_dependencies,
     select_metadata_dependencies,
 )
 from csvcubed.utils.uri import looks_like_uri
 
@@ -39,16 +39,16 @@
     This class handles the loading of metadata jsons to RDFLib Graphs.
     """
 
     csvw_metadata_file_path: Path
     rdf_graph: rdflib.ConjunctiveGraph = field(init=False)
 
     @cached_property
-    def csvw_inspector(self) -> CsvWInspector:
-        return CsvWInspector(self.rdf_graph, self.csvw_metadata_file_path)
+    def csvw_repository(self) -> CsvWRepository:
+        return CsvWRepository(self.rdf_graph, self.csvw_metadata_file_path)
 
     def __post_init__(self):
         self.rdf_graph = self._load_json_ld_to_rdflib_graph()
 
         if self.rdf_graph is None:
             raise FailedToLoadRDFGraphException(self.csvw_metadata_file_path)
```

## Comparing `csvcubed/utils/sparql_handler/code_list_inspector.py` & `csvcubed/utils/sparql_handler/code_list_repository.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
-Code List Inspector
--------------------
+Code List Repository
+--------------------
 
-This module contains the `CodeListInspector` class which allows API-style access to information
+This module contains the `CodeListRepository` class which allows API-style access to information
 about code lists contained within an RDF graph.
 """
 from dataclasses import dataclass
 from functools import cached_property
 from typing import Dict, List, Optional
 from urllib.parse import urljoin, urlparse
 
@@ -15,30 +15,30 @@
 from csvcubed.models.sparqlresults import (
     CatalogMetadataResult,
     CodeListTableIdentifers,
     ColumnDefinition,
 )
 from csvcubed.utils.iterables import first
 from csvcubed.utils.pandas import read_csv
-from csvcubed.utils.sparql_handler.csvw_inspector import CsvWInspector
+from csvcubed.utils.sparql_handler.csvw_repository import CsvWRepository
 from csvcubed.utils.text import truncate
 from csvcubed.utils.uri import file_uri_to_path, looks_like_uri
 from csvcubed.writers.skoscodelistwriter import (
     LABEL_COL_TITLE,
     URI_IDENTIFIER_COL_TITLE,
 )
 
 
 @dataclass
-class CodeListInspector:
+class CodeListRepository:
     """
     Allows API-style access to information about code lists contained within an RDF graph.
     """
 
-    csvw_inspector: CsvWInspector
+    csvw_repository: CsvWRepository
 
     @cached_property
     def _code_list_table_identifiers(self) -> List[CodeListTableIdentifers]:
         """This holds the identifiers mapping between csv_url and the concept_scheme_url."""
 
         def get_table_identifiers(
             csv_url: str,
@@ -65,15 +65,15 @@
                 )
 
             raise KeyError(f"Found multiple skos:inScheme columns in '{csv_url}'.")
 
         # Get the csv_url -> column_scheme_url identifiers for all csv files.
         table_identifiers = [
             get_table_identifiers(csv_url, columns)
-            for (csv_url, columns) in self.csvw_inspector.column_definitions.items()
+            for (csv_url, columns) in self.csvw_repository.column_definitions.items()
         ]
 
         # If the csv file doesn't have a code list in it, don't include it in the code list identifiers returned.
         return [i for i in table_identifiers if i is not None]
 
     def get_table_identifiers_for_concept_scheme(
         self, concept_scheme_url: str
@@ -92,15 +92,15 @@
 
         return identifiers
 
     def get_catalog_metadata_for_concept_scheme(
         self, concept_scheme_url: str
     ) -> CatalogMetadataResult:
         """Returns the Catalogue Metadata for a given ConceptScheme. Raises a KeyError if it cannot be found."""
-        catalog_mdata_results = self.csvw_inspector.catalog_metadata
+        catalog_mdata_results = self.csvw_repository.catalog_metadata
 
         result = first(
             catalog_mdata_results, lambda i: i.dataset_uri == concept_scheme_url
         )
 
         if result is None:
             raise KeyError(
@@ -121,15 +121,15 @@
             if urlparse(csv_url).scheme == "file":
                 # pandas expects local file URLs to be in the format `file://localhost/path/to/table.csv.`
                 absolute_csv_url = file_uri_to_path(csv_url)
             else:
                 absolute_csv_url = csv_url
         else:
             absolute_csv_url = file_uri_to_path(
-                urljoin(self.csvw_inspector.csvw_json_path.as_uri(), csv_url)
+                urljoin(self.csvw_repository.csvw_json_path.as_uri(), csv_url)
             )
 
         (dataframe, _) = read_csv(
             absolute_csv_url, usecols=[URI_IDENTIFIER_COL_TITLE, LABEL_COL_TITLE]
         )
 
         duplicated_uris = dataframe[
@@ -159,11 +159,11 @@
 
     def get_primary_csv_url(self) -> str:
         """
         Retrieves the csv_url for the primary CSV defined in the CSV-W.
         This will only work if the primary file loaded into the graph was a
         code list.
         """
-        primary_catalog_metadata = self.csvw_inspector.get_primary_catalog_metadata()
+        primary_catalog_metadata = self.csvw_repository.get_primary_catalog_metadata()
         return self.get_table_identifiers_for_concept_scheme(
             primary_catalog_metadata.dataset_uri
         ).csv_url
```

## Comparing `csvcubed/utils/sparql_handler/csvw_inspector.py` & `csvcubed/utils/sparql_handler/csvw_repository.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-Code List Inspector
--------------------
+CsvW Repository
+---------------
 
 Provides access to inspect the contents of an rdflib graph containing
 one of more code lists.
 """
 
 from dataclasses import dataclass, field
 from functools import cached_property
@@ -28,15 +28,15 @@
     select_column_definitions,
     select_csvw_catalog_metadata,
     select_table_schema_properties,
 )
 
 
 @dataclass
-class CsvWInspector:
+class CsvWRepository:
     """
     Provides access to inspect the contents of an rdflib graph containing one of more code lists.
     """
 
     rdf_graph: rdflib.ConjunctiveGraph
     csvw_json_path: Path
```

## Comparing `csvcubed/utils/sparql_handler/data_cube_inspector.py` & `csvcubed/utils/sparql_handler/data_cube_repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-Data Cube Inspector
--------------------
+Data Cube Repository
+--------------------
 
 Provides access to inspect the contents of an rdflib graph containing
 one of more data cubes.
 """
 
 from dataclasses import InitVar, dataclass, field
 from functools import cache, cached_property
@@ -22,84 +22,84 @@
 from csvcubed.models.cube.cube_shape import CubeShape
 from csvcubed.models.cube.qb.components.constants import ACCEPTED_DATATYPE_MAPPING
 from csvcubed.models.sparqlresults import (
     CodelistResult,
     CodelistsResult,
     ColumnDefinition,
     CubeTableIdentifiers,
-    IsPivotedShapeMeasureResult,
+    IsPivotedShapeResult,
     QubeComponentResult,
     QubeComponentsResult,
     UnitResult,
 )
 from csvcubed.models.validationerror import ValidationError
 from csvcubed.utils.dict import get_from_dict_ensure_exists
 from csvcubed.utils.iterables import first, group_by, single
 from csvcubed.utils.pandas import read_csv
 from csvcubed.utils.qb.components import ComponentPropertyType, EndUserColumnType
-from csvcubed.utils.sparql_handler.code_list_inspector import CodeListInspector
+from csvcubed.utils.sparql_handler.code_list_repository import CodeListRepository
 from csvcubed.utils.sparql_handler.column_component_info import ColumnComponentInfo
-from csvcubed.utils.sparql_handler.csvw_inspector import CsvWInspector
+from csvcubed.utils.sparql_handler.csvw_repository import CsvWRepository
 from csvcubed.utils.sparql_handler.sparqlquerymanager import (
     select_csvw_dsd_qube_components,
     select_data_set_dsd_and_csv_url,
     select_dsd_code_list_and_cols,
-    select_is_pivoted_shape_for_measures_in_data_set,
+    select_is_pivoted_shape_data_set,
     select_labels_for_resource_uris,
     select_units,
 )
 from csvcubed.utils.uri import file_uri_to_path
 
 _XSD_BASE_URI: str = XSD[""].toPython()
 
 
 @dataclass
-class DataCubeInspector:
+class DataCubeRepository:
     """Provides access to inspect the data cubes contained in an rdflib graph."""
 
-    csvw_inspector: CsvWInspector
-    code_list_inspector_in: InitVar[Optional[CodeListInspector]] = None
-    _code_list_inspector: CodeListInspector = field(init=False)
-
-    def __post_init__(self, code_list_inspector_in: Optional[CodeListInspector]):
-        self._code_list_inspector = code_list_inspector_in or CodeListInspector(
-            self.csvw_inspector
+    csvw_repository: CsvWRepository
+    code_list_repository_in: InitVar[Optional[CodeListRepository]] = None
+    _code_list_repository: CodeListRepository = field(init=False)
+
+    def __post_init__(self, code_list_repository_in: Optional[CodeListRepository]):
+        self._code_list_repository = code_list_repository_in or CodeListRepository(
+            self.csvw_repository
         )
 
     def __hash__(self):
         """
         Necessary for `@cache` attributes above function definitions within this class.
 
         We *don't* want to make use of the dataclass hashing functionality, since it may end up evaluating all of
         our cached properties which would mean they're no longer lazy-loading.
 
-        The csvw_inspector can uniquely identify us by the file we originally loaded.
+        The csvw_repository can uniquely identify us by the file we originally loaded.
         """
-        return hash(self.csvw_inspector)
+        return hash(self.csvw_repository)
 
     """
     Private cached properties.
     """
 
     @cached_property
     def _units(self) -> Dict[str, UnitResult]:
         """
         Gets the unit_uri for each UnitResult
         """
-        results = select_units(self.csvw_inspector.rdf_graph)
+        results = select_units(self.csvw_repository.rdf_graph)
         return {result.unit_uri: result for result in results}
 
     @cached_property
     def _cube_table_identifiers(self) -> Dict[str, CubeTableIdentifiers]:
         """
         Identifiers linking a given qb:DataSet with a csvw table (identified by the csvw:url).
 
         Maps from csv_url to the identifiers.
         """
-        results = select_data_set_dsd_and_csv_url(self.csvw_inspector.rdf_graph)
+        results = select_data_set_dsd_and_csv_url(self.csvw_repository.rdf_graph)
         results_dict: Dict[str, CubeTableIdentifiers] = {}
         for result in results:
             results_dict[result.csv_url] = result
         return results_dict
 
     @cached_property
     def _dsd_qube_components(self) -> Dict[str, QubeComponentsResult]:
@@ -107,71 +107,71 @@
         Maps csv_url to the qb:DataStructureDefinition components associated with it.
         """
         map_dsd_uri_to_csv_url = {
             i.dsd_uri: i.csv_url for i in self._cube_table_identifiers.values()
         }
 
         return select_csvw_dsd_qube_components(
-            self.csvw_inspector.rdf_graph,
-            self.csvw_inspector.csvw_json_path,
+            self.csvw_repository.rdf_graph,
+            self.csvw_repository.csvw_json_path,
             map_dsd_uri_to_csv_url,
-            self.csvw_inspector.column_definitions,
+            self.csvw_repository.column_definitions,
             self._cube_shapes,
         )
 
     @cached_property
     def _cube_shapes(self) -> Dict[str, CubeShape]:
         """
         A mapping of csvUrl to the given CubeShape. CSV tables which aren't cubes
          are not present here.
         """
 
         def _detect_shape_for_cube(
-            measures_with_shape: List[IsPivotedShapeMeasureResult],
+            csv_url_with_shape: List[IsPivotedShapeResult],
         ) -> CubeShape:
             """
             Given a metadata validator as input, returns the shape of the cube that
              metadata describes (Pivoted or Standard).
             """
             all_pivoted = True
             all_standard_shape = True
-            for measure in measures_with_shape:
-                all_pivoted = all_pivoted and measure.is_pivoted_shape
-                all_standard_shape = all_standard_shape and not measure.is_pivoted_shape
+            for csv_url in csv_url_with_shape:
+                all_pivoted = all_pivoted and csv_url.is_pivoted_shape
+                all_standard_shape = all_standard_shape and not csv_url.is_pivoted_shape
 
             if all_pivoted:
                 return CubeShape.Pivoted
             elif all_standard_shape:
                 return CubeShape.Standard
             else:
                 raise TypeError(
                     "The input metadata is invalid as the shape of the cube it represents is "
                     "not supported. More specifically, the input contains some observation values "
                     "that are pivoted and some are not pivoted."
                 )
 
-        results = select_is_pivoted_shape_for_measures_in_data_set(
-            self.csvw_inspector.rdf_graph, list(self._cube_table_identifiers.values())
+        results = select_is_pivoted_shape_data_set(
+            self.csvw_repository.rdf_graph, list(self._cube_table_identifiers.values())
         )
 
-        map_csv_url_to_measure_shape = group_by(results, lambda r: r.csv_url)
+        map_csv_url_to_shape = group_by(results, lambda r: r.csv_url)
 
         return {
-            csv_url: _detect_shape_for_cube(measures_with_shape)
-            for (csv_url, measures_with_shape) in map_csv_url_to_measure_shape.items()
+            csv_url: _detect_shape_for_cube(csv_url_with_shape)
+            for (csv_url, csv_url_with_shape) in map_csv_url_to_shape.items()
         }
 
     @cached_property
     def _codelists_and_cols(self) -> Dict[str, CodelistsResult]:
         """
         Maps the csv url to the code lists/columns featured in the CSV.
         """
         return select_dsd_code_list_and_cols(
-            self.csvw_inspector.rdf_graph,
-            self.csvw_inspector.csvw_json_path,
+            self.csvw_repository.rdf_graph,
+            self.csvw_repository.csvw_json_path,
         )
 
     """
     Public getters for the cached properties.
     """
 
     def get_unit_for_uri(self, uri: str) -> Optional[UnitResult]:
@@ -237,15 +237,15 @@
           format), and an RDF Data Cube DataStructureDefinition component directly associated with them.
 
         Columns are defined in the same order as in the CSV file.
         """
 
         real_columns = [
             c
-            for c in self.csvw_inspector.get_column_definitions_for_csv(csv_url)
+            for c in self.csvw_repository.get_column_definitions_for_csv(csv_url)
             if not c.virtual
         ]
         qube_components = self.get_dsd_qube_components_for_csv(csv_url).qube_components
         cube_shape = self.get_shape_for_csv(csv_url)
 
         observations_columns = {
             col
@@ -316,15 +316,15 @@
 
     def get_primary_csv_url(self) -> str:
         """
         Retrieves the csv_url for the primary CSV defined in the CSV-W.
         This will only work if the primary file loaded into the graph was a
         data cube.
         """
-        primary_catalog_metadata = self.csvw_inspector.get_primary_catalog_metadata()
+        primary_catalog_metadata = self.csvw_repository.get_primary_catalog_metadata()
         return self.get_cube_identifiers_for_data_set(
             primary_catalog_metadata.dataset_uri
         ).csv_url
 
     def get_dataframe(
         self, csv_url: str, dereference_uris: bool = True
     ) -> Tuple[pd.DataFrame, List[ValidationError]]:
@@ -333,15 +333,15 @@
         Returns DuplicateColumnTitleError in the event of two instances of the
         same columns being defined.
         dereference_uris=True means URIs of column values are converted to their human readable labels.
         """
         cols = self.get_column_component_info(csv_url)
         dict_of_types = _get_data_types_of_all_cols(cols)
         absolute_csv_url = file_uri_to_path(
-            urljoin(self.csvw_inspector.csvw_json_path.as_uri(), csv_url)
+            urljoin(self.csvw_repository.csvw_json_path.as_uri(), csv_url)
         )
         (df, _errors) = read_csv(absolute_csv_url, dtype=dict_of_types)
 
         if dereference_uris:
             code_lists = self.get_code_lists_and_cols(csv_url).codelists
             for col in cols:
                 col_values = df[col.column_definition.title].values
@@ -457,15 +457,15 @@
         if col.column_definition.title is None:
             raise ValueError(f"Column title is not defined - {col.column_definition}")
 
         code_list = single(
             code_lists, lambda c: col.column_definition.title in c.cols_used_in
         )
         concept_scheme_uri = code_list.code_list
-        uri_labels_dict = self._code_list_inspector.get_map_code_list_uri_to_label(
+        uri_labels_dict = self._code_list_repository.get_map_code_list_uri_to_label(
             concept_scheme_uri
         )
 
         return list(uri_labels_dict.values())
 
     def _map_column_name_to_title_to_attribute_value_url(
         self, csv_url: str
@@ -498,15 +498,15 @@
         map_col_name_to_title: Dict[str, str],
         map_resource_attr_col_name_to_value_url: Dict[str, str],
     ) -> Dict[str, List[str]]:
         """
         Returns a dictionary of column name mapped to a list of all attribute value uris for that column
         """
         absolute_csv_url = file_uri_to_path(
-            urljoin(self.csvw_inspector.csvw_json_path.as_uri(), csv_url)
+            urljoin(self.csvw_repository.csvw_json_path.as_uri(), csv_url)
         )
         (dataframe, _) = read_csv(
             absolute_csv_url,
             usecols=[
                 map_col_name_to_title[col_name]
                 for col_name in map_resource_attr_col_name_to_value_url.keys()
             ],
@@ -538,15 +538,15 @@
             for col_name, uri_list in map_col_name_to_attribute_value_uris.items()
             for uri in uri_list
         }
 
         uris_to_query = list(map_uri_to_col_name.keys())
 
         sparql_results = select_labels_for_resource_uris(
-            self.csvw_inspector.rdf_graph, uris_to_query
+            self.csvw_repository.rdf_graph, uris_to_query
         )
 
         map_col_title_to_attr_val_uris_and_labels: Dict[str, Dict[str, str]] = {}
         for uri, label in sparql_results.items():
             col_name = map_uri_to_col_name[uri]
             col_title = map_col_name_to_title[col_name]
             results_for_col_title = map_col_title_to_attr_val_uris_and_labels.get(
```

## Comparing `csvcubed/utils/sparql_handler/sparql_queries/select_is_pivoted_shape_for_measures_in_data_set.sparql` & `csvcubed/utils/sparql_handler/sparql_queries/select_is_pivoted_shape_data_set.sparql`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
 PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
 PREFIX csvw: <http://www.w3.org/ns/csvw#>
 PREFIX qb: <http://purl.org/linked-data/cube#>
 
-SELECT ?csvUrl ?measure (max(?isPivoted) as ?isPivotedShape)
+SELECT ?csvUrl (max(?isPivoted) as ?isPivotedShape)
 WHERE {
     ?dsd a qb:DataStructureDefinition;
          qb:component/qb:measure ?measure.
 
     # N.B. The join between ?dsd and ?csvUrl is injected as a `VALUES` table when the query is executed.
 
     [] csvw:url ?csvUrl;
        csvw:tableSchema/csvw:column/rdf:rest*/rdf:first [ csvw:propertyUrl ?measureColumnPropertyUrl ].
 
     BIND((STRENDS(str(?measureColumnPropertyUrl), str(?measure)) || STRENDS(str(?measure), str(?measureColumnPropertyUrl))) as ?isPivoted).
 }
-GROUP BY ?csvUrl ?measure
+GROUP BY ?csvUrl
```

## Comparing `csvcubed-0.4.1.dist-info/LICENSE` & `csvcubed-0.4.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `csvcubed-0.4.1.dist-info/METADATA` & `csvcubed-0.4.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: csvcubed
-Version: 0.4.1
+Version: 0.4.2
 Summary: A tool to generate RDF Data Cube style CSV-W cubes from tidy CSV files. Part of the csvcubed family.
 License: Apache-2.0
 Author: Integrated Data Service - Dissemination
 Author-email: csvcubed@gsscogs.uk
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: click (>=8.0.0)
 Requires-Dist: csvcubed-models (==0.1.6)
 Requires-Dist: jsonschema (>=4.4.0,<5.0.0)
 Requires-Dist: pandas (>=1.3.3,<2.0.0)
+Requires-Dist: platformdirs (>=3.5.0,<4.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: requests-cache (>=0.9.3,<0.10.0)
 Requires-Dist: treelib (>=1.6.1,<2.0.0)
 Requires-Dist: uritemplate (>=4.1.1,<5.0.0)
 Description-Content-Type: text/markdown
```

## Comparing `csvcubed-0.4.1.dist-info/RECORD` & `csvcubed-0.4.2.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,27 @@
 csvcubed/cli/buildcsvw/build.py,sha256=HXHaCD4ZQXhbeWzg-xVfxD68_RkuxKFYJNZNRZ0iilM,2881
 csvcubed/cli/codelist/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 csvcubed/cli/codelist/build_code_list.py,sha256=5blizIwZKfzhD8Dx_PSsEgfW6EskDqRq0ikSfPfxBjY,1414
 csvcubed/cli/entrypoint.py,sha256=fyjDEiXA9LV5s1Z_CTyj2tghJRDm1yhcbPnvYujYg7Y,5742
 csvcubed/cli/error_mapping.py,sha256=1XpOAMOnZN5v44z5csHlhWNDlrBGF6ckDkmpajkUYqw,9572
 csvcubed/cli/inspectcsvw/README.md,sha256=1zx59skhdF11RyYiJUsV28pF6Xfhb85u1xDQbe1841o,238
 csvcubed/cli/inspectcsvw/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-csvcubed/cli/inspectcsvw/inspect.py,sha256=5l_jwepkIcSlHYFACEZThDzjzzcoyFFfoJIPfOfeuYI,4300
+csvcubed/cli/inspectcsvw/inspect.py,sha256=W2k1-ZgF8OJjiAnUI3ZE4NbROEgLnrNAWFMLAH6FmX4,4316
 csvcubed/cli/inspectcsvw/inspectdatasetmanager.py,sha256=48RwoGglHmCZrvaESmGRAwqkvpN4DwK7W3-XHKrzEs8,3333
 csvcubed/cli/inspectcsvw/metadatainputvalidator.py,sha256=TUWJ4542lhdEye5XhU0paGIWi9LTjyKuU7_Vg9wSRtw,1517
-csvcubed/cli/inspectcsvw/metadataprinter.py,sha256=YoJS8IOUTcIrZBNiybHSvyD-U-PwyVY2YtDHDYhgsjs,13706
+csvcubed/cli/inspectcsvw/metadataprinter.py,sha256=GM-8Hj_LvB7skmUSfNeBk3ezE3HznpK9vXOzMcvMbSk,15006
 csvcubed/cli/pullcsvw/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 csvcubed/cli/pullcsvw/pull.py,sha256=F2cXz6EivdwhHLgHgivXgo5EGnWPZQKxBu3uaKFwLds,13791
 csvcubed/definitions.py,sha256=l5mLOMGAdHEXfx7vIJUSxlargSWBW97IEzHvpblIUlg,840
 csvcubed/inputs.py,sha256=x2mTOfwIwz3mEjRJRwnVG-sns71Eyk_hEXGssXXe7i8,1981
+csvcubed/inspect/inspectorcolumns.py,sha256=yRF6M1LwHRORYfldqdgMwfrFw6mgBV7Xmy-Y988AvG0,7577
+csvcubed/inspect/inspectorcomponents.py,sha256=xxlCDGBsenAAXMvJgNw_Lg_1Q6ZtuP7PvzOgfrcpPxg,3425
+csvcubed/inspect/inspectors.py,sha256=rMmxgxS39XU1Q-USyIQJfwbMRmANMIhQg6Sgy9yvlS8,3241
+csvcubed/inspect/inspectortable.py,sha256=UL2xJlCEZc57r9AQ0_zJCrXpRtwTsc7RH65RCIfuM74,7419
+csvcubed/inspect/lazyfuncdescriptor.py,sha256=g5qu5-dWLPFl9NkJ_mvv1ba-StfAekKmOIqTOeIpo5E,1657
 csvcubed/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 csvcubed/models/codelistconfig/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 csvcubed/models/codelistconfig/code_list_config.py,sha256=dkPPoTyazqpYPuOJ2jUzCOL1DIDu16EveiqOEstLUSQ,8467
 csvcubed/models/csvcubedexception.py,sha256=cfE3N-06CZ_bjMJV5gZ4KK6JLuFdq7Jcbe4uZiA-Krc,14542
 csvcubed/models/csvwtype.py,sha256=7WXT5EcWT48YNFn3oyPJkgPKRDPoyJZZrXHvaeWC6Jk,409
 csvcubed/models/cube/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 csvcubed/models/cube/catalog.py,sha256=9AX4wIIglrjSTkhUI2YmzbLv_D9Z4rmz11bTMN74occ,676
@@ -56,15 +61,15 @@
 csvcubed/models/rdf/conceptschemeincatalog.py,sha256=p3e1CLP9c5qcGw3hhl8H_N6Y1VJW8K-wgvz4D75XYks,526
 csvcubed/models/rdf/newattributevalueresource.py,sha256=QJ2fWjQ_VuOVQFWDAD7N4Xhf4nzhp4q9A1BVTsJ_1Yo,858
 csvcubed/models/rdf/newunitresource.py,sha256=6vr5T8UGXrqjG6AINYcNcGsC1LMjt-eNO25jF8J3P9Q,1670
 csvcubed/models/rdf/prov.py,sha256=BzvPmYiKv1nOC0unrBg8lYu5pXemDz3syQLaQX62rIA,1188
 csvcubed/models/rdf/qbdatasetincatalog.py,sha256=IpRZBm6JWkfRzrlgSnl5n8IjRccb0_eOkNS9Hf-luTU,447
 csvcubed/models/sparql/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 csvcubed/models/sparql/valuesbinding.py,sha256=nJxVQgytQZrYrnCPssr_-EMO7uY2rpGxaNLwy9MTfLo,457
-csvcubed/models/sparqlresults.py,sha256=_Wvvzcg7Y6jlbfFj0TJGky9yaQb46Qw4AuJgZsTLIbY,20070
+csvcubed/models/sparqlresults.py,sha256=3pC53qeGRTrhlOBdQlI_Oz9fahiFTcHk9wV6p9VvD90,18128
 csvcubed/models/uriidentifiable.py,sha256=tP9hBDJj7LIUMjdvO7mc2PYNKOCmu8NjSt_2XFtpIFw,1814
 csvcubed/models/validatedmodel.py,sha256=IcRFWUvmXO839gU1HCLQ8h41_CGqkdSe8mfBD2uvD9Q,3108
 csvcubed/models/validationerror.py,sha256=uDx5TPS_VcZZT790HM_V_hlkKnRj19-YIJrBIJnfrEY,3167
 csvcubed/readers/__init__.py,sha256=j-b06j5EDS5IAqkd7FkyGb9TV-KLDyGB0_g65LnaoEA,110
 csvcubed/readers/catalogmetadata/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 csvcubed/readers/catalogmetadata/v1/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 csvcubed/readers/catalogmetadata/v1/catalog_metadata_reader.py,sha256=BqmMn8wEc5KCcAhtCkXfNr78BZe6bRvKAywQ5m_gMgY,1637
@@ -111,58 +116,58 @@
 csvcubed/schema/cube-config/v1_2/schema.json,sha256=1zuVO6WXBXRL-TZtMWgAWbhHrfjwcCwXNUO0z2jIDyk,26394
 csvcubed/schema/cube-config/v1_3/schema.json,sha256=vNobTvct1s70-XmovUf2kHhJ5v7t_A0ZKiLJo6Psck4,31399
 csvcubed/schema/cube-config/v1_4/schema.json,sha256=6CaymYv-yIMNpNAlPMpHZXPUUM7qOxKx22PRvBfi-IM,32992
 csvcubed/utils/__init__.py,sha256=GEljQsipGps0CgGfOBUMnoAeFqnQbZkZzfb86R96ZpQ,67
 csvcubed/utils/cache.py,sha256=FJtD-pWfWE7AVFYW36V1lpm5iw377cX4Z5H3YUIU07M,356
 csvcubed/utils/cli.py,sha256=az8WpfljZdlffBMpuYZ8FtCXhl8u_uGlCXMsma01WnQ,2979
 csvcubed/utils/createlocalcopyresponse.py,sha256=w2vD5f9DnW_D_9VwWP_MfEMro5bpmX77qXkJzmhAsgs,6536
-csvcubed/utils/csvdataset.py,sha256=X3aVbVESjLoOUxpDSbREQg0sQxjXviaq-cJqqr3sjbY,14033
+csvcubed/utils/csvdataset.py,sha256=0RKBgaVS2bhbN9JpBlUC-dDfzZLo5j6vUPoDdYCmKFk,13791
 csvcubed/utils/csvw.py,sha256=SIzMCURqDOnlCU_oHmSsyturOw2-ecA0QAsT4sicujw,4518
 csvcubed/utils/datetime.py,sha256=VaammJPt10PUuN4qGgsntobgbCKUOIoqNNEwpDHWtRA,453
 csvcubed/utils/dict.py,sha256=YlhEoyBELSrKcS0dd42b7SMBSHX7Eh0R1uV4cabXU8M,1488
 csvcubed/utils/file.py,sha256=9q_7i8MPriBdggvHCFIY2VYgeoiFru4kGyWWJ2Nb9F0,1682
 csvcubed/utils/iterables.py,sha256=cP-wcLYUj-M1QNc9ysnt7l_ILYPd-nMY9IzXPqG4WDA,1582
 csvcubed/utils/json.py,sha256=qg29-TkmSa9myqz1SHi6mUTsKCNCsmCx4Z4hmHLw9gs,4253
-csvcubed/utils/log.py,sha256=3dAi3C5CcDBzYFuhlHANoi-I0HmNUYbTfobGFp9pWtw,3333
+csvcubed/utils/log.py,sha256=lGVRX7XBYbCOr9xQg9H6unNRMqqCZ3CZ77V0kKuKiPw,3348
 csvcubed/utils/pandas.py,sha256=BSgdW897rJf5jgv4KvFggTmKa0qnRkoHazB7lstnQ-4,1783
 csvcubed/utils/printable.py,sha256=n_gY1VHZ71I0aMNzC9xaUtIFexxtdJXTNTw9DLdiLFI,1169
 csvcubed/utils/qb/__init__.py,sha256=co8SgYAU9PKQALalcvK4Ty96h0zLeGQ3Xf0UUMUd6tQ,41
 csvcubed/utils/qb/components.py,sha256=tFBtLHzhp9Rn1CnwLstgPzvBlLPOlNQy-PA6c7TMzjo,4228
 csvcubed/utils/qb/cube.py,sha256=NBPI1keSiGIUrg9dLADqNfSkSlrb5LFlcASCsDnrkxE,3512
 csvcubed/utils/qb/standardise.py,sha256=SZegTL5FE0JZsuZQRLwO8BmcjT7bwI5MMWCUNJ9h0Mc,8509
 csvcubed/utils/qb/validation/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 csvcubed/utils/qb/validation/cube.py,sha256=uZMkkEaRIrJw3HZxyZtQs9XFs1cMD7KQlSccvJuv12Y,2983
 csvcubed/utils/qb/validation/observations.py,sha256=Ubv0vTfdHkcmRQ9mE21Eb8I0xEu239zxEhC3D505aWM,18273
 csvcubed/utils/qb/validation/uri_safe.py,sha256=lgnkxSplAT1E5QUWAOD8i4pe2u3JneLEBa9N2th0AQQ,1672
 csvcubed/utils/rdf.py,sha256=Ki0Sqh0FWB6atz4q2xtbDcgQVDLcb00PuRkWuo5WJnk,1945
 csvcubed/utils/skos/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 csvcubed/utils/skos/codelist.py,sha256=nIENnG8nm-jEBnO05Ge-rWEItXLYDVmUey2qIvhe0bI,3017
 csvcubed/utils/sparql_handler/__init__.py,sha256=IUbRkPhSFfbFNEt0Jsht80tOyjmuWfEAlpCDHH6mUp8,89
-csvcubed/utils/sparql_handler/code_list_inspector.py,sha256=SF_cQlkPLkBN27bJ7rOE9D14gf7-HKGGo9W8qG8KBvI,6289
+csvcubed/utils/sparql_handler/code_list_repository.py,sha256=l9WZ9wvVCGDG1zLQ7DEfaccH2OEQVJGOPog_VDkeRCg,6301
 csvcubed/utils/sparql_handler/column_component_info.py,sha256=E5OrqZcxppALLqTMDyC8tEtA_4s0D3XyncMKIT3x18E,955
-csvcubed/utils/sparql_handler/csvw_inspector.py,sha256=rGJY6k4AzGWrz_7EiJquHbmhFdLRYNfx3l7qLKtnSrM,4583
-csvcubed/utils/sparql_handler/data_cube_inspector.py,sha256=D6rCaEd-mUsEJV9sr5voX4hugLJBvBq5896cqDXPTWo,24662
-csvcubed/utils/sparql_handler/sparql.py,sha256=t2rK3MztIy0JTbASmpxNfKBMCa0lZ-EAUn4CnLVxsWA,3889
+csvcubed/utils/sparql_handler/csvw_repository.py,sha256=1hPghg_lkN5dsrje9cj0x245C7SGRsdvllN5Ck6bIyE,4576
+csvcubed/utils/sparql_handler/data_cube_repository.py,sha256=8HLcn5jYC_PbPlTsmThG8WeEno_uqBieuMzSUahkHPE,24631
+csvcubed/utils/sparql_handler/sparql.py,sha256=qaNDCXySBavCCVWvhD_TXfCWU-xhgFmNU3gcEdg6Gzs,3901
 csvcubed/utils/sparql_handler/sparql_queries/ask_is_codelist.sparql,sha256=9_qf61Mn1b4H2huNFvhxDD78jTqWw7W2Zrk0g6msino,88
 csvcubed/utils/sparql_handler/sparql_queries/ask_is_qb_dataset.sparql,sha256=eYgoKHTGTaex3xizQ9lx5t9kEPu6ejvXC7El8M2aXSk,75
 csvcubed/utils/sparql_handler/sparql_queries/select_catalog_metadata.sparql,sha256=HSF4DAB79RvFMU6zWHXvQjEcvfZ8ivtUolMxUyFIsCo,2298
 csvcubed/utils/sparql_handler/sparql_queries/select_codelist_csv_url.sparql,sha256=LEFLJBati_-bGkBnnJEG7XgA5VYhiMm9kdB9gW7e3H8,1006
 csvcubed/utils/sparql_handler/sparql_queries/select_codelist_primary_key_by_csv_url.sparql,sha256=JLs1SHwPrTBsV45COO9gOk2hj4Z4vjSi4uBE2GFrsis,482
 csvcubed/utils/sparql_handler/sparql_queries/select_codelists_and_cols.sparql,sha256=oGxWovWaoGcyB-Ez8eM7oECscpaP1BiDbLWeSJxb-vw,969
 csvcubed/utils/sparql_handler/sparql_queries/select_column_definitions.sparql,sha256=3SKgOc4N8uexKI93DUivW05NZJSYw4gcDQVyaUJlB9g,2149
 csvcubed/utils/sparql_handler/sparql_queries/select_csvw_table_schema_file_dependencies.sparql,sha256=qk0zSe5baKHfXM9-IXk_0xY3KMog3ED1-7_p-sDSezA,354
 csvcubed/utils/sparql_handler/sparql_queries/select_data_set_dsd_csv_url.sparql,sha256=VuGw9y_aKTP3G59PUlUh_-wj7bfHILQnH2XajOJTcvM,1188
 csvcubed/utils/sparql_handler/sparql_queries/select_dsd_qube_components.sparql,sha256=_5LF2eWp_udc09q-U2F0ZwMHIxWwliF8tkKOgYGyXNw,1339
-csvcubed/utils/sparql_handler/sparql_queries/select_is_pivoted_shape_for_measures_in_data_set.sparql,sha256=HAKnXxouSVGIue0V_1YPHCMMcFR9lTxhxS-ljP0jMLY,757
+csvcubed/utils/sparql_handler/sparql_queries/select_is_pivoted_shape_data_set.sparql,sha256=6hgg7p37A_k7bz78LqICUEe17_O0q5WJpbI0msQZn2c,739
 csvcubed/utils/sparql_handler/sparql_queries/select_labels_for_resource_uris.sparql,sha256=R0e2hBvyTggTJW3iyRubeOsLomLlyoP_q_m6wi12dEM,179
 csvcubed/utils/sparql_handler/sparql_queries/select_metadata_dependencies.sparql,sha256=rmCH3---NlDNQXu1hlq-fvvMIAckNYkHZPe3tdlXdLU,379
 csvcubed/utils/sparql_handler/sparql_queries/select_table_schema_properties.sparql,sha256=2al7ZhCLHtPEVkvubzigAlmrTuT5AHup5B6WtoQxzBw,466
 csvcubed/utils/sparql_handler/sparql_queries/select_units.sparql,sha256=uuA1L0fywz9oosVyGd3WIKCILBi1KvYlZqfj519rmQE,367
-csvcubed/utils/sparql_handler/sparqlquerymanager.py,sha256=f_H6c8ryd5uh-lcyeDPhMlE5VlrxL6-UMpWRvHecNfo,11626
-csvcubed/utils/tableschema.py,sha256=N6zuJU1-RWWQNNZWPLsqhhU0LK54FM8u9gztSoadbJw,9198
+csvcubed/utils/sparql_handler/sparqlquerymanager.py,sha256=hTjum5Py3FJx3yu1njPCF9ECKSQtmVtR51torZ0agT8,11693
+csvcubed/utils/tableschema.py,sha256=5Mf4mSENxFPZ90NkqHRdPFNPFWdb6azeNR7scaPNyC8,9203
 csvcubed/utils/text.py,sha256=bIj2Ykra-bXaUk-EyrYCy07LrHZdY6dYXsYO8A6I_i0,356
 csvcubed/utils/uri.py,sha256=ZEX3IQG0r_xV4W_p4omhKs6x8YdXLnOGxa8vmwH_r4o,3467
 csvcubed/utils/validations.py,sha256=uWuLPturZRk6p59ya-U_zymGZBC4tM0MdGbeaGy7IE0,11239
 csvcubed/utils/validators/__init__.py,sha256=fHGeu6xOpC030v5SM2wzkvnKad8uC8_LavMJU5UxKho,45
 csvcubed/utils/validators/schema.py,sha256=txW2VLdGv1-Wo15aTgWjEiGLM3Jac1T4iU0k7eIifIc,4360
 csvcubed/utils/version.py,sha256=T-I5rVx5T08tqrTNldwwDYQVzarYtwQ_ap0g8JbgTbw,268
 csvcubed/writers/__init__.py,sha256=njopI6UIMFsqWF6i5v5huPhvRvixU-creIptscLQBUg,62
@@ -173,12 +178,12 @@
 csvcubed/writers/helpers/qbwriter/urihelper.py,sha256=BzVnUueyoE1DBncTByKnigeLozePdfFRfxzaguwCtxY,27378
 csvcubed/writers/helpers/skoscodelistwriter/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 csvcubed/writers/helpers/skoscodelistwriter/constants.py,sha256=FjVa2JsAc7uIxzQOJgNg3zf8Ha-YZvMzF75sqq_e93g,157
 csvcubed/writers/helpers/skoscodelistwriter/newresourceurigenerator.py,sha256=DWkL2zO4QsLV8Oo-nVXxS4cxA1ic4stSBp7NZpClbps,2437
 csvcubed/writers/qbwriter.py,sha256=fDesUmhWU1211z_wDQi8xFdfpB0CqdSHG7pM-YlsJQc,20804
 csvcubed/writers/skoscodelistwriter.py,sha256=dCK3RaOrv4jeD6l4SZ2PT9tr8zqZwR2x8kbRTsASIMc,9470
 csvcubed/writers/writerbase.py,sha256=lzEHMgqdWBIFbxthYjf5JuE3i5gp5Vbb1Xw359TY3to,283
-csvcubed-0.4.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-csvcubed-0.4.1.dist-info/METADATA,sha256=GaSNyyTY9XL66EbewEipZGCLRlMWIk-hQHYwe6JWHOo,3925
-csvcubed-0.4.1.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-csvcubed-0.4.1.dist-info/entry_points.txt,sha256=sGis93BsSIrPNIht5YkyuYCvefbri5nvVdOyI9ImAFs,64
-csvcubed-0.4.1.dist-info/RECORD,,
+csvcubed-0.4.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+csvcubed-0.4.2.dist-info/METADATA,sha256=XsZsCYdolL4NwGAXOywbYbc2pFjBc2PhFT5ngNEqraA,3930
+csvcubed-0.4.2.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+csvcubed-0.4.2.dist-info/entry_points.txt,sha256=sGis93BsSIrPNIht5YkyuYCvefbri5nvVdOyI9ImAFs,64
+csvcubed-0.4.2.dist-info/RECORD,,
```


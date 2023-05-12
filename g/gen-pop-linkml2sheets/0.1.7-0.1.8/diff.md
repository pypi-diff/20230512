# Comparing `tmp/gen_pop_linkml2sheets-0.1.7.tar.gz` & `tmp/gen_pop_linkml2sheets-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_pop_linkml2sheets-0.1.7.tar", max compression
+gzip compressed data, was "gen_pop_linkml2sheets-0.1.8.tar", max compression
```

## Comparing `gen_pop_linkml2sheets-0.1.7.tar` & `gen_pop_linkml2sheets-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1075 2023-05-10 12:40:56.283705 gen_pop_linkml2sheets-0.1.7/LICENSE.md
--rw-r--r--   0        0        0     4403 2023-05-10 13:29:28.451789 gen_pop_linkml2sheets-0.1.7/README.md
--rw-r--r--   0        0        0     2426 2023-05-12 17:46:52.489511 gen_pop_linkml2sheets-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      111 2023-05-10 17:53:28.805534 gen_pop_linkml2sheets-0.1.7/src/gen_pop_linkml2sheets/__init__.py
--rw-r--r--   0        0        0     6222 2023-05-12 17:44:08.001222 gen_pop_linkml2sheets-0.1.7/src/gen_pop_linkml2sheets/generate_and_populate_template.py
--rw-r--r--   0        0        0     5125 1970-01-01 00:00:00.000000 gen_pop_linkml2sheets-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-10 12:40:56.283705 gen_pop_linkml2sheets-0.1.8/LICENSE.md
+-rw-r--r--   0        0        0     4403 2023-05-10 13:29:28.451789 gen_pop_linkml2sheets-0.1.8/README.md
+-rw-r--r--   0        0        0     2426 2023-05-12 19:49:55.298273 gen_pop_linkml2sheets-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      111 2023-05-10 17:53:28.805534 gen_pop_linkml2sheets-0.1.8/src/gen_pop_linkml2sheets/__init__.py
+-rw-r--r--   0        0        0     6990 2023-05-12 19:15:11.113218 gen_pop_linkml2sheets-0.1.8/src/gen_pop_linkml2sheets/generate_and_populate_template.py
+-rw-r--r--   0        0        0     5125 1970-01-01 00:00:00.000000 gen_pop_linkml2sheets-0.1.8/PKG-INFO
```

### Comparing `gen_pop_linkml2sheets-0.1.7/LICENSE.md` & `gen_pop_linkml2sheets-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gen_pop_linkml2sheets-0.1.7/README.md` & `gen_pop_linkml2sheets-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `gen_pop_linkml2sheets-0.1.7/pyproject.toml` & `gen_pop_linkml2sheets-0.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gen-pop-linkml2sheets"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["Mark Andrew Miller <MAM@lbl.gov>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/turbomam/gen-pop-linkml2sheets"
 repository = "https://github.com/turbomam/gen-pop-linkml2sheets"
 packages = [{ include = "gen_pop_linkml2sheets", from = "src" }]
```

### Comparing `gen_pop_linkml2sheets-0.1.7/src/gen_pop_linkml2sheets/generate_and_populate_template.py` & `gen_pop_linkml2sheets-0.1.8/src/gen_pop_linkml2sheets/generate_and_populate_template.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,36 +33,60 @@
 @click.option('--meta-path',
               default="https://raw.githubusercontent.com/linkml/linkml-model/main/linkml_model/model/schema/meta.yaml",
               help='URL or filesystem path to the LinkML meta model YAML file')
 @click.option('--meta-model-excel-file',
               default="meta.xlsx",
               help='Where should a local XLSX representation of the meta model be saved?')
 @click.option('--base-class',
-              default='slot_definition',
+              default=['slot_definition'],
+              multiple=True,
               help="Which class' definition should form the basis of the report?")
 @click.option('--columns-to-insert',
               multiple=True,
               default=["slot", "class"],
               help="What LinkML meta slots (that don't appear in the base class) should be added to the report?")
 @click.option('--columns-to-remove',
               multiple=True,
-              default=["all_members", "all_of", "alt_descriptions", "annotations", "any_of", "enum_range",
-                       "exactly_one_of", "extensions", "has_member", "name", "none_of", "path_rule", "range_expression",
-                       "structured_aliases", "unit"],
+              default=[
+                  "all_members",
+                  "all_of",
+                  "alt_descriptions",
+                  "annotations",
+                  "any_of",
+                  "enum_range",
+                  "exactly_one_of",
+                  "extensions",
+                  "has_member",
+                  "include",
+                  "inherits",
+                  "matches",
+                  "minus",
+                  "name",
+                  "none_of",
+                  "path_rule",
+                  "permissible_values",
+                  "prefix_prefix",
+                  "pv_formula",
+                  "range_expression",
+                  "reachable_from",
+                  "structured_aliases",
+                  "text",
+                  "unit",
+              ],
               help='What LinkML meta slots from the base class should be added to the report?')
 @click.option('--columns-to-use',
               multiple=True,
               help='Overrides any other determinant of which columns to use in the report.')
 @click.option('--source-schema-path',
               required=True,
               help='URL or filesystem path to the schema that will populate the report')
 @click.option('--destination-template',
               default='usage_template.tsv',
               help='Where should the template and usage reports TSVs be saved?')
-def generate_and_populate_template(source_schema_path: str, meta_path: str, base_class: str, destination_template: str,
+def generate_and_populate_template(source_schema_path: str, meta_path: str, base_class: list, destination_template: str,
                                    columns_to_remove: list, columns_to_insert: list,
                                    meta_model_excel_file: str, columns_to_use: list) -> None:
     """Generate a TSV representation of slot usages in a schema, guided by an XLSX representation of the metamodel.
 
     Args:
         base_class (str): Name of the selected sheet in the intermediate Excel file, forming the basis of the usage report
         columns_to_insert (list): Columns to insert into the template.
@@ -86,16 +110,19 @@
 
     annotation_tags = discover_annotations(sv, verbose=False)
     # pprint.pprint(annotation_tags)
 
     excel_generator = ExcelGenerator(schema=meta_view.schema, output=meta_model_excel_file)
     excel_generator.serialize()
 
-    df = pd.read_excel(meta_model_excel_file, sheet_name=base_class)
-    columns_for_template = list(df.columns)
+    columns_for_template = set()
+    for one_base in base_class:
+        df = pd.read_excel(meta_model_excel_file, sheet_name=one_base)
+        columns_for_template.update(df.columns)
+    columns_for_template = list(columns_for_template)
 
     for column in columns_to_remove:
         if column in columns_for_template:
             columns_for_template.remove(column)
 
     columns_for_template.sort()
 
@@ -128,14 +155,17 @@
         writer.writerows(sheet)
 
     exporter = SchemaExporter()
 
     exporter.export(sv, specification=destination_template, to_file=populated_file)
 
     populated = pd.read_csv(populated_file, sep='\t')
-    populated = populated.iloc[1:]
+    if len(annotation_tags) > 0:
+        populated = populated.iloc[2:]
+    else:
+        populated = populated.iloc[1:]
     populated = populated.dropna(axis=1, how='all')
     populated.to_csv(useful_file, sep='\t', index=False)
 
 
 if __name__ == '__main__':
     generate_and_populate_template()
```

### Comparing `gen_pop_linkml2sheets-0.1.7/PKG-INFO` & `gen_pop_linkml2sheets-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-pop-linkml2sheets
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Home-page: https://github.com/turbomam/gen-pop-linkml2sheets
 License: MIT
 Author: Mark Andrew Miller
 Author-email: MAM@lbl.gov
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gen-pop-linkml2sheets Version: 0.1.7 Summary: Home-
+Metadata-Version: 2.1 Name: gen-pop-linkml2sheets Version: 0.1.8 Summary: Home-
 page: https://github.com/turbomam/gen-pop-linkml2sheets License: MIT Author:
 Mark Andrew Miller Author-email: MAM@lbl.gov Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: linkml (>=1.5.2,<2.0.0) Requires-
 Dist: pandas (>=1.3.4,<2.0.0) Requires-Dist: schemasheets (>=0.1.21,<0.2.0)
```


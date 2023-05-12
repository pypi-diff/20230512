# Comparing `tmp/semantic-field-definition-generator-1.2.1.tar.gz` & `tmp/semantic-field-definition-generator-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic-field-definition-generator-1.2.1.tar", last modified: Mon Apr 24 15:45:36 2023, max compression
+gzip compressed data, was "semantic-field-definition-generator-1.3.0.tar", last modified: Fri May 12 16:29:46 2023, max compression
```

## Comparing `semantic-field-definition-generator-1.2.1.tar` & `semantic-field-definition-generator-1.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-04-24 15:45:36.696265 semantic-field-definition-generator-1.2.1/
--rw-r--r--   0 casties    (501) staff       (20)     1073 2023-02-20 08:35:34.000000 semantic-field-definition-generator-1.2.1/LICENSE
--rw-r--r--   0 casties    (501) staff       (20)     7381 2023-04-24 15:45:36.696128 semantic-field-definition-generator-1.2.1/PKG-INFO
--rw-r--r--   0 casties    (501) staff       (20)     5578 2023-03-04 15:21:10.000000 semantic-field-definition-generator-1.2.1/README.md
--rw-r--r--   0 casties    (501) staff       (20)     1024 2023-04-24 15:43:35.000000 semantic-field-definition-generator-1.2.1/pyproject.toml
--rw-r--r--   0 casties    (501) staff       (20)       38 2023-04-24 15:45:36.696301 semantic-field-definition-generator-1.2.1/setup.cfg
-drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-04-24 15:45:36.692381 semantic-field-definition-generator-1.2.1/src/
-drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-04-24 15:45:36.693575 semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/
--rw-r--r--   0 casties    (501) staff       (20)        0 2023-02-25 16:29:53.000000 semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/__init__.py
--rw-r--r--   0 casties    (501) staff       (20)     3050 2023-03-02 18:37:44.000000 semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/generator.py
--rw-r--r--   0 casties    (501) staff       (20)    10346 2023-03-03 10:06:35.000000 semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/parser.py
--rwxr-xr-x   0 casties    (501) staff       (20)     5185 2023-04-24 15:28:47.000000 semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/semantic_field_util.py
-drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-04-24 15:45:36.694911 semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/templates/
--rw-r--r--   0 casties    (501) staff       (20)     2799 2023-03-02 18:26:32.000000 semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/templates/inline.handlebars
--rw-r--r--   0 casties    (501) staff       (20)     2853 2023-03-02 18:26:16.000000 semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/templates/json.handlebars
--rw-r--r--   0 casties    (501) staff       (20)     5200 2023-04-24 15:39:53.000000 semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/templates/metaphacts.handlebars
--rw-r--r--   0 casties    (501) staff       (20)     4049 2023-04-24 15:39:40.000000 semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/templates/researchspace.handlebars
--rw-r--r--   0 casties    (501) staff       (20)     5470 2023-04-24 15:39:59.000000 semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/templates/universal.handlebars
-drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-04-24 15:45:36.695913 semantic-field-definition-generator-1.2.1/src/semantic_field_definition_generator.egg-info/
--rw-r--r--   0 casties    (501) staff       (20)     7381 2023-04-24 15:45:36.000000 semantic-field-definition-generator-1.2.1/src/semantic_field_definition_generator.egg-info/PKG-INFO
--rw-r--r--   0 casties    (501) staff       (20)      955 2023-04-24 15:45:36.000000 semantic-field-definition-generator-1.2.1/src/semantic_field_definition_generator.egg-info/SOURCES.txt
--rw-r--r--   0 casties    (501) staff       (20)        1 2023-04-24 15:45:36.000000 semantic-field-definition-generator-1.2.1/src/semantic_field_definition_generator.egg-info/dependency_links.txt
--rw-r--r--   0 casties    (501) staff       (20)       98 2023-04-24 15:45:36.000000 semantic-field-definition-generator-1.2.1/src/semantic_field_definition_generator.egg-info/entry_points.txt
--rw-r--r--   0 casties    (501) staff       (20)       22 2023-04-24 15:45:36.000000 semantic-field-definition-generator-1.2.1/src/semantic_field_definition_generator.egg-info/requires.txt
--rw-r--r--   0 casties    (501) staff       (20)       33 2023-04-24 15:45:36.000000 semantic-field-definition-generator-1.2.1/src/semantic_field_definition_generator.egg-info/top_level.txt
+drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-05-12 16:29:46.473599 semantic-field-definition-generator-1.3.0/
+-rw-r--r--   0 casties    (501) staff       (20)     1073 2023-02-20 08:35:34.000000 semantic-field-definition-generator-1.3.0/LICENSE
+-rw-r--r--   0 casties    (501) staff       (20)     7412 2023-05-12 16:29:46.473481 semantic-field-definition-generator-1.3.0/PKG-INFO
+-rw-r--r--   0 casties    (501) staff       (20)     5609 2023-05-12 16:23:46.000000 semantic-field-definition-generator-1.3.0/README.md
+-rw-r--r--   0 casties    (501) staff       (20)     1024 2023-05-12 16:20:29.000000 semantic-field-definition-generator-1.3.0/pyproject.toml
+-rw-r--r--   0 casties    (501) staff       (20)       38 2023-05-12 16:29:46.473634 semantic-field-definition-generator-1.3.0/setup.cfg
+drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-05-12 16:29:46.469828 semantic-field-definition-generator-1.3.0/src/
+drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-05-12 16:29:46.471031 semantic-field-definition-generator-1.3.0/src/SemanticFieldDefinitionGenerator/
+-rw-r--r--   0 casties    (501) staff       (20)        0 2023-02-25 16:29:53.000000 semantic-field-definition-generator-1.3.0/src/SemanticFieldDefinitionGenerator/__init__.py
+-rw-r--r--   0 casties    (501) staff       (20)     3982 2023-05-12 16:22:41.000000 semantic-field-definition-generator-1.3.0/src/SemanticFieldDefinitionGenerator/generator.py
+-rw-r--r--   0 casties    (501) staff       (20)    10889 2023-05-12 15:10:03.000000 semantic-field-definition-generator-1.3.0/src/SemanticFieldDefinitionGenerator/parser.py
+-rwxr-xr-x   0 casties    (501) staff       (20)     5271 2023-05-12 16:23:09.000000 semantic-field-definition-generator-1.3.0/src/SemanticFieldDefinitionGenerator/semantic_field_util.py
+drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-05-12 16:29:46.472296 semantic-field-definition-generator-1.3.0/src/SemanticFieldDefinitionGenerator/templates/
+-rw-r--r--   0 casties    (501) staff       (20)     2799 2023-03-02 18:26:32.000000 semantic-field-definition-generator-1.3.0/src/SemanticFieldDefinitionGenerator/templates/inline.handlebars
+-rw-r--r--   0 casties    (501) staff       (20)     2853 2023-03-02 18:26:16.000000 semantic-field-definition-generator-1.3.0/src/SemanticFieldDefinitionGenerator/templates/json.handlebars
+-rw-r--r--   0 casties    (501) staff       (20)     5200 2023-04-24 15:39:53.000000 semantic-field-definition-generator-1.3.0/src/SemanticFieldDefinitionGenerator/templates/metaphacts.handlebars
+-rw-r--r--   0 casties    (501) staff       (20)     4049 2023-04-24 15:39:40.000000 semantic-field-definition-generator-1.3.0/src/SemanticFieldDefinitionGenerator/templates/researchspace.handlebars
+-rw-r--r--   0 casties    (501) staff       (20)     5470 2023-04-24 15:39:59.000000 semantic-field-definition-generator-1.3.0/src/SemanticFieldDefinitionGenerator/templates/universal.handlebars
+drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-05-12 16:29:46.473313 semantic-field-definition-generator-1.3.0/src/semantic_field_definition_generator.egg-info/
+-rw-r--r--   0 casties    (501) staff       (20)     7412 2023-05-12 16:29:46.000000 semantic-field-definition-generator-1.3.0/src/semantic_field_definition_generator.egg-info/PKG-INFO
+-rw-r--r--   0 casties    (501) staff       (20)      955 2023-05-12 16:29:46.000000 semantic-field-definition-generator-1.3.0/src/semantic_field_definition_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 casties    (501) staff       (20)        1 2023-05-12 16:29:46.000000 semantic-field-definition-generator-1.3.0/src/semantic_field_definition_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 casties    (501) staff       (20)       98 2023-05-12 16:29:46.000000 semantic-field-definition-generator-1.3.0/src/semantic_field_definition_generator.egg-info/entry_points.txt
+-rw-r--r--   0 casties    (501) staff       (20)       22 2023-05-12 16:29:46.000000 semantic-field-definition-generator-1.3.0/src/semantic_field_definition_generator.egg-info/requires.txt
+-rw-r--r--   0 casties    (501) staff       (20)       33 2023-05-12 16:29:46.000000 semantic-field-definition-generator-1.3.0/src/semantic_field_definition_generator.egg-info/top_level.txt
```

### Comparing `semantic-field-definition-generator-1.2.1/LICENSE` & `semantic-field-definition-generator-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `semantic-field-definition-generator-1.2.1/PKG-INFO` & `semantic-field-definition-generator-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-field-definition-generator
-Version: 1.2.1
+Version: 1.3.0
 Summary: A generator for Field Definitions for ResearchSpace and Metaphacts
 Author-email: Robert Casties <casties@mpiwg-berlin.mpg.de>, Florian Kräutli <florian.kraeutli@uzh.ch>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -53,46 +53,45 @@
 ### Command line tool
 
 For more details on the use of the command line tool run `semantic-field-util -h`:
 
 ```
 usage: semantic-field-util [-h] [--version] [-f {RS,MP,UNI,JSON,INLINE}] -y YAML_FILE [-u SPARQL_URI]
                            [--sparql-repository SPARQL_REPOSITORY] [--sparql-auth-user SPARQL_USER]
-                           [--sparql-auth-password SPARQL_PASS] [-t TRIG_FILE]
-                           [--field-id-prefix FIELD_PREFIX] [--split-fields] [-l {INFO,DEBUG,ERROR}]
+                           [--sparql-auth-password SPARQL_PASS] [-t TRIG_FILE] [--field-id-prefix FIELD_PREFIX]
+                           [--split-fields] [-l {INFO,DEBUG,ERROR}]
                            {read,write}
 
 Utility to convert ResarchSpace/Metaphacts semantic field definitions.
 
 positional arguments:
-  {read,write}          Action: read=read semantic field definitions in RDF (SPARQL store or file) and
-                        write YAML file, write=read YAML file and write semantic field definitions to
-                        RDF file
+  {read,write}          Action: read=read semantic field definitions in RDF (SPARQL store or file) and write YAML file,
+                        write=read YAML file and write semantic field definitions to RDF TriG file(s)
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -f {RS,MP,UNI,JSON,INLINE}, --flavor {RS,MP,UNI,JSON,INLINE}
-                        Flavor of RDF field definitions: RS=ResearchSpace, MP=Metaphacts,
-                        UNI=universal, JSON=JSON, INLINE=inline, default=RS
+                        Flavor of RDF field definitions: RS=ResearchSpace, MP=Metaphacts, UNI=universal, JSON=JSON,
+                        INLINE=inline, default=RS
   -y YAML_FILE, --yaml YAML_FILE
-                        YAML file with field definitions to read or write
+                        YAML file (can be directory containing *.yml files) with field definitions to read or write
   -u SPARQL_URI, --sparql-uri SPARQL_URI
                         SPARQL endpoint URI, e.g. http://localhost:8081/sparql
   --sparql-repository SPARQL_REPOSITORY
                         Optional SPARQL repository parameter, default=assets
   --sparql-auth-user SPARQL_USER
                         Optional SPARQL auth username, default=admin
   --sparql-auth-password SPARQL_PASS
                         Optional SPARQL auth password, default=admin
   -t TRIG_FILE, --trig TRIG_FILE
                         RDF TriG file (can be directory containing *.trig files) to read or write
   --field-id-prefix FIELD_PREFIX
                         Optional URL prefix for field ids
-  --split-fields        Optional split TriG output into one file per field (file name = field id)
+  --split-fields        Optional split TriG/YAML output into one file per field (file name = field id)
   -l {INFO,DEBUG,ERROR}, --log {INFO,DEBUG,ERROR}
                         Log level.
 ```
 
 ### Create field definitions
 
 Define field definitions as a Python dict or in an external YAML file:
```

### Comparing `semantic-field-definition-generator-1.2.1/README.md` & `semantic-field-definition-generator-1.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,46 +21,45 @@
 ### Command line tool
 
 For more details on the use of the command line tool run `semantic-field-util -h`:
 
 ```
 usage: semantic-field-util [-h] [--version] [-f {RS,MP,UNI,JSON,INLINE}] -y YAML_FILE [-u SPARQL_URI]
                            [--sparql-repository SPARQL_REPOSITORY] [--sparql-auth-user SPARQL_USER]
-                           [--sparql-auth-password SPARQL_PASS] [-t TRIG_FILE]
-                           [--field-id-prefix FIELD_PREFIX] [--split-fields] [-l {INFO,DEBUG,ERROR}]
+                           [--sparql-auth-password SPARQL_PASS] [-t TRIG_FILE] [--field-id-prefix FIELD_PREFIX]
+                           [--split-fields] [-l {INFO,DEBUG,ERROR}]
                            {read,write}
 
 Utility to convert ResarchSpace/Metaphacts semantic field definitions.
 
 positional arguments:
-  {read,write}          Action: read=read semantic field definitions in RDF (SPARQL store or file) and
-                        write YAML file, write=read YAML file and write semantic field definitions to
-                        RDF file
+  {read,write}          Action: read=read semantic field definitions in RDF (SPARQL store or file) and write YAML file,
+                        write=read YAML file and write semantic field definitions to RDF TriG file(s)
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -f {RS,MP,UNI,JSON,INLINE}, --flavor {RS,MP,UNI,JSON,INLINE}
-                        Flavor of RDF field definitions: RS=ResearchSpace, MP=Metaphacts,
-                        UNI=universal, JSON=JSON, INLINE=inline, default=RS
+                        Flavor of RDF field definitions: RS=ResearchSpace, MP=Metaphacts, UNI=universal, JSON=JSON,
+                        INLINE=inline, default=RS
   -y YAML_FILE, --yaml YAML_FILE
-                        YAML file with field definitions to read or write
+                        YAML file (can be directory containing *.yml files) with field definitions to read or write
   -u SPARQL_URI, --sparql-uri SPARQL_URI
                         SPARQL endpoint URI, e.g. http://localhost:8081/sparql
   --sparql-repository SPARQL_REPOSITORY
                         Optional SPARQL repository parameter, default=assets
   --sparql-auth-user SPARQL_USER
                         Optional SPARQL auth username, default=admin
   --sparql-auth-password SPARQL_PASS
                         Optional SPARQL auth password, default=admin
   -t TRIG_FILE, --trig TRIG_FILE
                         RDF TriG file (can be directory containing *.trig files) to read or write
   --field-id-prefix FIELD_PREFIX
                         Optional URL prefix for field ids
-  --split-fields        Optional split TriG output into one file per field (file name = field id)
+  --split-fields        Optional split TriG/YAML output into one file per field (file name = field id)
   -l {INFO,DEBUG,ERROR}, --log {INFO,DEBUG,ERROR}
                         Log level.
 ```
 
 ### Create field definitions
 
 Define field definitions as a Python dict or in an external YAML file:
```

### Comparing `semantic-field-definition-generator-1.2.1/pyproject.toml` & `semantic-field-definition-generator-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "semantic-field-definition-generator"
-version = "1.2.1"
+version = "1.3.0"
 authors = [
   { name="Robert Casties", email="casties@mpiwg-berlin.mpg.de" },
   { name="Florian Kräutli", email="florian.kraeutli@uzh.ch" },
 ]
 description = "A generator for Field Definitions for ResearchSpace and Metaphacts"
 readme = "README.md"
 license = {file = "LICENSE"}
```

### Comparing `semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/parser.py` & `semantic-field-definition-generator-1.3.0/src/SemanticFieldDefinitionGenerator/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from rdflib import Dataset, URIRef
 from rdflib.namespace import Namespace, NamespaceManager
 from rdflib.plugins.stores.sparqlstore import SPARQLStore
 from pathlib import Path
 import yaml
 import logging
+from urllib.parse import urlencode, quote_plus
 
-__version__ = '1.2'
+__version__ = '1.3'
 
 # flavors
 RESEARCHSPACE = 1
 METAPHACTS = 2
 
 ##
 ## namespaces
@@ -254,16 +255,28 @@
             _set_once(queries, 'valueSet', str(f.valueSetPattern))
         
         if queries:
             field['queries'] = [{k: v} for k, v in queries.items()]
     
     return field
 
-def write_fields_yaml(fields, filename, field_id_prefix=None):
+def write_fields_yaml(fields, filename, field_id_prefix=None, splitFields=False):
     """write all fields to YAML file filename."""
-    logging.info(f"writing {len(fields)} fields to YAML file {filename}")
-    with open(filename, 'w') as f:
-        data = {'fields': fields}
-        if field_id_prefix:
-            data['prefix'] = field_id_prefix
-        
-        yaml.dump(data, stream=f)
+    if splitFields:
+        logging.info(f"writing {len(fields)} fields to YAML directory {filename}")
+        for field in fields:
+            fn = quote_plus(field['id']) + '.yml'
+            with open(Path(filename, fn), 'w') as f:
+                data = {'fields': [field]}
+                if field_id_prefix:
+                    data['prefix'] = field_id_prefix
+                
+                yaml.dump(data, stream=f)
+            
+    else:
+        logging.info(f"writing {len(fields)} fields to YAML file {filename}")
+        with open(filename, 'w') as f:
+            data = {'fields': fields}
+            if field_id_prefix:
+                data['prefix'] = field_id_prefix
+            
+            yaml.dump(data, stream=f)
```

### Comparing `semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/semantic_field_util.py` & `semantic-field-definition-generator-1.3.0/src/SemanticFieldDefinitionGenerator/semantic_field_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,45 +2,45 @@
 from SemanticFieldDefinitionGenerator import generator, parser
 from pathlib import Path
 import urllib
 import argparse
 import logging
 import sys
 
-__version__ = '1.2'
+__version__ = '1.3'
 
 def main():
     ## 
     ## main
     ##
     argp = argparse.ArgumentParser(description='Utility to convert ResarchSpace/Metaphacts semantic field definitions.')
     argp.add_argument('--version', action='version', version='%(prog)s ' + __version__)
     argp.add_argument('action', choices=['read', 'write'],
                       help='Action: read=read semantic field definitions in RDF (SPARQL store or file) and write YAML file, '
-                      + 'write=read YAML file and write semantic field definitions to RDF file')
+                      + 'write=read YAML file and write semantic field definitions to RDF TriG file(s)')
     argp.add_argument('-f', '--flavor', dest='flavor', choices=['RS', 'MP', 'UNI', 'JSON', 'INLINE'],
                       default='RS',
                       help='Flavor of RDF field definitions: RS=ResearchSpace, MP=Metaphacts, UNI=universal, '
                       + 'JSON=JSON, INLINE=inline, default=RS')
     argp.add_argument('-y', '--yaml', required=True, dest='yaml_file',
-                      help='YAML file with field definitions to read or write')
+                      help='YAML file (can be directory containing *.yml files) with field definitions to read or write')
     argp.add_argument('-u', '--sparql-uri', dest='sparql_uri',
                       help='SPARQL endpoint URI, e.g. http://localhost:8081/sparql')
     argp.add_argument('--sparql-repository', dest='sparql_repository', default='assets',
                       help='Optional SPARQL repository parameter, default=assets')
     argp.add_argument('--sparql-auth-user', dest='sparql_user', default='admin',
                       help='Optional SPARQL auth username, default=admin')
     argp.add_argument('--sparql-auth-password', dest='sparql_pass', default='admin',
                       help='Optional SPARQL auth password, default=admin')
     argp.add_argument('-t', '--trig', dest='trig_file',
                       help='RDF TriG file (can be directory containing *.trig files) to read or write')
     argp.add_argument('--field-id-prefix', dest='field_prefix',
                       help='Optional URL prefix for field ids')
     argp.add_argument('--split-fields', dest='split_fields', action='store_true',
-                      help='Optional split TriG output into one file per field (file name = field id)')
+                      help='Optional split TriG/YAML output into one file per field (file name = field id)')
     argp.add_argument('-l', '--log', dest='loglevel', choices=['INFO', 'DEBUG', 'ERROR'], default='INFO', 
                       help='Log level.')
     args = argp.parse_args()
     
     logging.basicConfig(level=args.loglevel)
     
     ##
@@ -99,8 +99,8 @@
                                       auth_user=args.sparql_user, auth_pass=args.sparql_pass)
         elif args.trig_file:
             store = parser.read_trig_store(args.trig_file)
         else:
             sys.exit(f"ERROR: action 'read' requires SPARQL_URI or TRIG_FILE!")
     
         fields = parser.read_fields(store, flavor, field_id_prefix=args.field_prefix)
-        parser.write_fields_yaml(fields, args.yaml_file, field_id_prefix=args.field_prefix)
+        parser.write_fields_yaml(fields, args.yaml_file, field_id_prefix=args.field_prefix, splitFields=args.split_fields)
```

### Comparing `semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/templates/inline.handlebars` & `semantic-field-definition-generator-1.3.0/src/SemanticFieldDefinitionGenerator/templates/inline.handlebars`

 * *Files identical despite different names*

### Comparing `semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/templates/json.handlebars` & `semantic-field-definition-generator-1.3.0/src/SemanticFieldDefinitionGenerator/templates/json.handlebars`

 * *Files identical despite different names*

### Comparing `semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/templates/metaphacts.handlebars` & `semantic-field-definition-generator-1.3.0/src/SemanticFieldDefinitionGenerator/templates/metaphacts.handlebars`

 * *Files identical despite different names*

### Comparing `semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/templates/researchspace.handlebars` & `semantic-field-definition-generator-1.3.0/src/SemanticFieldDefinitionGenerator/templates/researchspace.handlebars`

 * *Files identical despite different names*

### Comparing `semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/templates/universal.handlebars` & `semantic-field-definition-generator-1.3.0/src/SemanticFieldDefinitionGenerator/templates/universal.handlebars`

 * *Files identical despite different names*

### Comparing `semantic-field-definition-generator-1.2.1/src/semantic_field_definition_generator.egg-info/PKG-INFO` & `semantic-field-definition-generator-1.3.0/src/semantic_field_definition_generator.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-field-definition-generator
-Version: 1.2.1
+Version: 1.3.0
 Summary: A generator for Field Definitions for ResearchSpace and Metaphacts
 Author-email: Robert Casties <casties@mpiwg-berlin.mpg.de>, Florian Kräutli <florian.kraeutli@uzh.ch>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -53,46 +53,45 @@
 ### Command line tool
 
 For more details on the use of the command line tool run `semantic-field-util -h`:
 
 ```
 usage: semantic-field-util [-h] [--version] [-f {RS,MP,UNI,JSON,INLINE}] -y YAML_FILE [-u SPARQL_URI]
                            [--sparql-repository SPARQL_REPOSITORY] [--sparql-auth-user SPARQL_USER]
-                           [--sparql-auth-password SPARQL_PASS] [-t TRIG_FILE]
-                           [--field-id-prefix FIELD_PREFIX] [--split-fields] [-l {INFO,DEBUG,ERROR}]
+                           [--sparql-auth-password SPARQL_PASS] [-t TRIG_FILE] [--field-id-prefix FIELD_PREFIX]
+                           [--split-fields] [-l {INFO,DEBUG,ERROR}]
                            {read,write}
 
 Utility to convert ResarchSpace/Metaphacts semantic field definitions.
 
 positional arguments:
-  {read,write}          Action: read=read semantic field definitions in RDF (SPARQL store or file) and
-                        write YAML file, write=read YAML file and write semantic field definitions to
-                        RDF file
+  {read,write}          Action: read=read semantic field definitions in RDF (SPARQL store or file) and write YAML file,
+                        write=read YAML file and write semantic field definitions to RDF TriG file(s)
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -f {RS,MP,UNI,JSON,INLINE}, --flavor {RS,MP,UNI,JSON,INLINE}
-                        Flavor of RDF field definitions: RS=ResearchSpace, MP=Metaphacts,
-                        UNI=universal, JSON=JSON, INLINE=inline, default=RS
+                        Flavor of RDF field definitions: RS=ResearchSpace, MP=Metaphacts, UNI=universal, JSON=JSON,
+                        INLINE=inline, default=RS
   -y YAML_FILE, --yaml YAML_FILE
-                        YAML file with field definitions to read or write
+                        YAML file (can be directory containing *.yml files) with field definitions to read or write
   -u SPARQL_URI, --sparql-uri SPARQL_URI
                         SPARQL endpoint URI, e.g. http://localhost:8081/sparql
   --sparql-repository SPARQL_REPOSITORY
                         Optional SPARQL repository parameter, default=assets
   --sparql-auth-user SPARQL_USER
                         Optional SPARQL auth username, default=admin
   --sparql-auth-password SPARQL_PASS
                         Optional SPARQL auth password, default=admin
   -t TRIG_FILE, --trig TRIG_FILE
                         RDF TriG file (can be directory containing *.trig files) to read or write
   --field-id-prefix FIELD_PREFIX
                         Optional URL prefix for field ids
-  --split-fields        Optional split TriG output into one file per field (file name = field id)
+  --split-fields        Optional split TriG/YAML output into one file per field (file name = field id)
   -l {INFO,DEBUG,ERROR}, --log {INFO,DEBUG,ERROR}
                         Log level.
 ```
 
 ### Create field definitions
 
 Define field definitions as a Python dict or in an external YAML file:
```

### Comparing `semantic-field-definition-generator-1.2.1/src/semantic_field_definition_generator.egg-info/SOURCES.txt` & `semantic-field-definition-generator-1.3.0/src/semantic_field_definition_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*


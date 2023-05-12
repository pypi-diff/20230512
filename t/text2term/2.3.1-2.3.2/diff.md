# Comparing `tmp/text2term-2.3.1.tar.gz` & `tmp/text2term-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2term-2.3.1.tar", last modified: Wed May 10 16:24:55 2023, max compression
+gzip compressed data, was "text2term-2.3.2.tar", last modified: Fri May 12 15:13:00 2023, max compression
```

## Comparing `text2term-2.3.1.tar` & `text2term-2.3.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-10 16:24:55.959643 text2term-2.3.1/
--rw-r--r--   0 jason      (501) staff       (20)     1117 2022-08-03 13:24:07.000000 text2term-2.3.1/LICENSE
--rw-r--r--   0 jason      (501) staff       (20)    14914 2023-05-10 16:24:55.959439 text2term-2.3.1/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)    14156 2023-05-04 15:09:10.000000 text2term-2.3.1/README.md
--rw-r--r--   0 jason      (501) staff       (20)       38 2023-05-10 16:24:55.959695 text2term-2.3.1/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)     1162 2023-03-27 17:45:54.000000 text2term-2.3.1/setup.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-10 16:24:55.955062 text2term-2.3.1/test/
--rw-r--r--   0 jason      (501) staff       (20)     1435 2023-04-25 18:43:12.000000 text2term-2.3.1/test/test-pypi.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-10 16:24:55.958185 text2term-2.3.1/text2term/
--rw-r--r--   0 jason      (501) staff       (20)      427 2023-05-04 15:09:10.000000 text2term-2.3.1/text2term/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     4540 2023-04-25 19:04:10.000000 text2term-2.3.1/text2term/__main__.py
--rw-r--r--   0 jason      (501) staff       (20)     4416 2023-05-10 15:07:50.000000 text2term-2.3.1/text2term/bioportal_mapper.py
--rw-r--r--   0 jason      (501) staff       (20)       17 2023-05-10 16:24:04.000000 text2term-2.3.1/text2term/config.py
--rw-r--r--   0 jason      (501) staff       (20)      469 2022-09-26 14:42:08.000000 text2term-2.3.1/text2term/mapper.py
--rw-r--r--   0 jason      (501) staff       (20)     3735 2023-05-10 16:24:04.000000 text2term-2.3.1/text2term/onto_cache.py
--rw-r--r--   0 jason      (501) staff       (20)     6692 2023-03-27 17:45:54.000000 text2term-2.3.1/text2term/onto_utils.py
--rw-r--r--   0 jason      (501) staff       (20)     5540 2023-03-27 17:45:54.000000 text2term-2.3.1/text2term/preprocess.py
--rw-r--r--   0 jason      (501) staff       (20)     5403 2023-05-10 15:07:50.000000 text2term-2.3.1/text2term/syntactic_mapper.py
--rw-r--r--   0 jason      (501) staff       (20)    12516 2023-05-10 15:07:50.000000 text2term-2.3.1/text2term/t2t.py
--rw-r--r--   0 jason      (501) staff       (20)      741 2023-02-24 16:05:08.000000 text2term-2.3.1/text2term/tagged_terms.py
--rw-r--r--   0 jason      (501) staff       (20)     2479 2023-04-18 15:25:34.000000 text2term-2.3.1/text2term/term.py
--rw-r--r--   0 jason      (501) staff       (20)    17050 2023-05-04 15:09:10.000000 text2term-2.3.1/text2term/term_collector.py
--rw-r--r--   0 jason      (501) staff       (20)     2697 2022-08-03 13:24:07.000000 text2term-2.3.1/text2term/term_graph.py
--rw-r--r--   0 jason      (501) staff       (20)     2991 2023-01-20 15:17:36.000000 text2term-2.3.1/text2term/term_graph_generator.py
--rw-r--r--   0 jason      (501) staff       (20)     2158 2023-04-11 13:56:32.000000 text2term-2.3.1/text2term/term_mapping.py
--rw-r--r--   0 jason      (501) staff       (20)     5108 2022-11-15 20:43:11.000000 text2term-2.3.1/text2term/tfidf_mapper.py
--rw-r--r--   0 jason      (501) staff       (20)     4098 2023-05-10 15:07:50.000000 text2term-2.3.1/text2term/zooma_mapper.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-10 16:24:55.959219 text2term-2.3.1/text2term.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)    14914 2023-05-10 16:24:55.000000 text2term-2.3.1/text2term.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)      649 2023-05-10 16:24:55.000000 text2term-2.3.1/text2term.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2023-05-10 16:24:55.000000 text2term-2.3.1/text2term.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)      248 2023-05-10 16:24:55.000000 text2term-2.3.1/text2term.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)       10 2023-05-10 16:24:55.000000 text2term-2.3.1/text2term.egg-info/top_level.txt
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-12 15:13:00.790068 text2term-2.3.2/
+-rw-r--r--   0 jason      (501) staff       (20)     1117 2022-08-03 13:24:07.000000 text2term-2.3.2/LICENSE
+-rw-r--r--   0 jason      (501) staff       (20)    14914 2023-05-12 15:13:00.789894 text2term-2.3.2/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)    14156 2023-05-04 15:09:10.000000 text2term-2.3.2/README.md
+-rw-r--r--   0 jason      (501) staff       (20)       38 2023-05-12 15:13:00.790109 text2term-2.3.2/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)     1162 2023-03-27 17:45:54.000000 text2term-2.3.2/setup.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-12 15:13:00.785980 text2term-2.3.2/test/
+-rw-r--r--   0 jason      (501) staff       (20)     1435 2023-04-25 18:43:12.000000 text2term-2.3.2/test/test-pypi.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-12 15:13:00.789025 text2term-2.3.2/text2term/
+-rw-r--r--   0 jason      (501) staff       (20)      427 2023-05-04 15:09:10.000000 text2term-2.3.2/text2term/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     4540 2023-04-25 19:04:10.000000 text2term-2.3.2/text2term/__main__.py
+-rw-r--r--   0 jason      (501) staff       (20)     4416 2023-05-10 15:07:50.000000 text2term-2.3.2/text2term/bioportal_mapper.py
+-rw-r--r--   0 jason      (501) staff       (20)       17 2023-05-12 15:12:28.000000 text2term-2.3.2/text2term/config.py
+-rw-r--r--   0 jason      (501) staff       (20)      469 2022-09-26 14:42:08.000000 text2term-2.3.2/text2term/mapper.py
+-rw-r--r--   0 jason      (501) staff       (20)     3735 2023-05-10 16:24:04.000000 text2term-2.3.2/text2term/onto_cache.py
+-rw-r--r--   0 jason      (501) staff       (20)     6692 2023-03-27 17:45:54.000000 text2term-2.3.2/text2term/onto_utils.py
+-rw-r--r--   0 jason      (501) staff       (20)     5540 2023-03-27 17:45:54.000000 text2term-2.3.2/text2term/preprocess.py
+-rw-r--r--   0 jason      (501) staff       (20)     5403 2023-05-10 15:07:50.000000 text2term-2.3.2/text2term/syntactic_mapper.py
+-rw-r--r--   0 jason      (501) staff       (20)    12868 2023-05-12 15:12:28.000000 text2term-2.3.2/text2term/t2t.py
+-rw-r--r--   0 jason      (501) staff       (20)      741 2023-02-24 16:05:08.000000 text2term-2.3.2/text2term/tagged_terms.py
+-rw-r--r--   0 jason      (501) staff       (20)     2479 2023-04-18 15:25:34.000000 text2term-2.3.2/text2term/term.py
+-rw-r--r--   0 jason      (501) staff       (20)    17050 2023-05-04 15:09:10.000000 text2term-2.3.2/text2term/term_collector.py
+-rw-r--r--   0 jason      (501) staff       (20)     2697 2022-08-03 13:24:07.000000 text2term-2.3.2/text2term/term_graph.py
+-rw-r--r--   0 jason      (501) staff       (20)     2991 2023-01-20 15:17:36.000000 text2term-2.3.2/text2term/term_graph_generator.py
+-rw-r--r--   0 jason      (501) staff       (20)     2158 2023-04-11 13:56:32.000000 text2term-2.3.2/text2term/term_mapping.py
+-rw-r--r--   0 jason      (501) staff       (20)     5108 2022-11-15 20:43:11.000000 text2term-2.3.2/text2term/tfidf_mapper.py
+-rw-r--r--   0 jason      (501) staff       (20)     4098 2023-05-10 15:07:50.000000 text2term-2.3.2/text2term/zooma_mapper.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-12 15:13:00.789692 text2term-2.3.2/text2term.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)    14914 2023-05-12 15:13:00.000000 text2term-2.3.2/text2term.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)      649 2023-05-12 15:13:00.000000 text2term-2.3.2/text2term.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2023-05-12 15:13:00.000000 text2term-2.3.2/text2term.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)      248 2023-05-12 15:13:00.000000 text2term-2.3.2/text2term.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)       10 2023-05-12 15:13:00.000000 text2term-2.3.2/text2term.egg-info/top_level.txt
```

### Comparing `text2term-2.3.1/LICENSE` & `text2term-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `text2term-2.3.1/PKG-INFO` & `text2term-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2term
-Version: 2.3.1
+Version: 2.3.2
 Summary: A tool for mapping free-text descriptions of (biomedical) entities to controlled terms in ontologies
 Home-page: https://github.com/ccb-hms/ontology-mapper
 Author: Center for Computational Biomedicine, Harvard Medical School
 Author-email: rafael_goncalves@hms.harvard.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `text2term-2.3.1/README.md` & `text2term-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `text2term-2.3.1/setup.py` & `text2term-2.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.1/test/test-pypi.py` & `text2term-2.3.2/test/test-pypi.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.1/text2term/__main__.py` & `text2term-2.3.2/text2term/__main__.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.1/text2term/bioportal_mapper.py` & `text2term-2.3.2/text2term/bioportal_mapper.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.1/text2term/onto_cache.py` & `text2term-2.3.2/text2term/onto_cache.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.1/text2term/onto_utils.py` & `text2term-2.3.2/text2term/onto_utils.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.1/text2term/preprocess.py` & `text2term-2.3.2/text2term/preprocess.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.1/text2term/syntactic_mapper.py` & `text2term-2.3.2/text2term/syntactic_mapper.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.1/text2term/t2t.py` & `text2term-2.3.2/text2term/t2t.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,26 +215,35 @@
     if len(onto_terms) == 0:
         raise RuntimeError("Could not find any terms in the given ontology.")
     return onto_terms
 
 def _do_mapping(source_terms, source_term_ids, ontology_terms, mapper, max_mappings, min_score):
     if mapper == Mapper.TFIDF:
         term_mapper = TFIDFMapper(ontology_terms)
-        return term_mapper.map(source_terms, source_term_ids, max_mappings=max_mappings, min_score=min_score)
+        mappings_df = term_mapper.map(source_terms, source_term_ids, max_mappings=max_mappings, min_score=min_score)
     elif mapper == Mapper.ZOOMA:
         term_mapper = ZoomaMapper()
-        return term_mapper.map(source_terms, source_term_ids, ontologies=ontology_terms, max_mappings=max_mappings)
+        mappings_df = term_mapper.map(source_terms, source_term_ids, ontologies=ontology_terms, max_mappings=max_mappings)
     elif mapper == Mapper.BIOPORTAL:
         term_mapper = BioPortalAnnotatorMapper("8f0cbe43-2906-431a-9572-8600d3f4266e")
-        return term_mapper.map(source_terms, source_term_ids, ontologies=ontology_terms, max_mappings=max_mappings)
+        mappings_df = term_mapper.map(source_terms, source_term_ids, ontologies=ontology_terms, max_mappings=max_mappings)
     elif mapper in {Mapper.LEVENSHTEIN, Mapper.JARO, Mapper.JARO_WINKLER, Mapper.INDEL, Mapper.FUZZY, Mapper.JACCARD}:
         term_mapper = SyntacticMapper(ontology_terms)
-        return term_mapper.map(source_terms, source_term_ids, mapper, max_mappings=max_mappings)
+        mappings_df = term_mapper.map(source_terms, source_term_ids, mapper, max_mappings=max_mappings)
     else:
         raise ValueError("Unsupported mapper: " + mapper)
+    df = _filter_mappings(mappings_df, min_score)
+    return df
+
+def _filter_mappings(mappings_df, min_score):
+    new_df = pd.DataFrame(columns=mappings_df.columns)
+    for index, row in mappings_df.iterrows():
+        if row['Mapping Score'] >= min_score:
+            new_df.loc[len(new_df.index)] = row
+    return new_df
 
 def _save_mappings(mappings, output_file, min_score, mapper, target_ontology, base_iris, excl_deprecated, max_mappings, term_type):
     if os.path.dirname(output_file):  # create output directories if needed
         os.makedirs(os.path.dirname(output_file), exist_ok=True)
     with open(output_file, "a") as f:
         f.write("# Date and time run: %s\n" % datetime.datetime.now())
         f.write("# Target Ontology: %s\n" % target_ontology)
```

### Comparing `text2term-2.3.1/text2term/tagged_terms.py` & `text2term-2.3.2/text2term/tagged_terms.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.1/text2term/term.py` & `text2term-2.3.2/text2term/term.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.1/text2term/term_collector.py` & `text2term-2.3.2/text2term/term_collector.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.1/text2term/term_graph.py` & `text2term-2.3.2/text2term/term_graph.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.1/text2term/term_graph_generator.py` & `text2term-2.3.2/text2term/term_graph_generator.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.1/text2term/term_mapping.py` & `text2term-2.3.2/text2term/term_mapping.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.1/text2term/tfidf_mapper.py` & `text2term-2.3.2/text2term/tfidf_mapper.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.1/text2term/zooma_mapper.py` & `text2term-2.3.2/text2term/zooma_mapper.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.1/text2term.egg-info/PKG-INFO` & `text2term-2.3.2/text2term.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2term
-Version: 2.3.1
+Version: 2.3.2
 Summary: A tool for mapping free-text descriptions of (biomedical) entities to controlled terms in ontologies
 Home-page: https://github.com/ccb-hms/ontology-mapper
 Author: Center for Computational Biomedicine, Harvard Medical School
 Author-email: rafael_goncalves@hms.harvard.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `text2term-2.3.1/text2term.egg-info/SOURCES.txt` & `text2term-2.3.2/text2term.egg-info/SOURCES.txt`

 * *Files identical despite different names*


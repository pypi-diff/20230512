# Comparing `tmp/simstring_fast-0.2.4.tar.gz` & `tmp/simstring_fast-0.2.6.tar.gz`

## Comparing `simstring_fast-0.2.4.tar` & `simstring_fast-0.2.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/__init__.py
--rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/searcher.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/database/__init__.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/database/base.py
--rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/database/dict.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/feature_extractor/__init__.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/feature_extractor/base.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/feature_extractor/character_ngram.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/feature_extractor/word_ngram.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/measure/__init__.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/measure/base.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/measure/cosine.py
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/measure/dice.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/measure/jaccard.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/measure/overlap.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/LICENSE
--rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/README.md
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 simstring_fast-0.2.6/simstring/__init__.py
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 simstring_fast-0.2.6/simstring/searcher.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 simstring_fast-0.2.6/simstring/database/__init__.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 simstring_fast-0.2.6/simstring/database/base.py
+-rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 simstring_fast-0.2.6/simstring/database/dict.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 simstring_fast-0.2.6/simstring/feature_extractor/__init__.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 simstring_fast-0.2.6/simstring/feature_extractor/base.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 simstring_fast-0.2.6/simstring/feature_extractor/character_ngram.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 simstring_fast-0.2.6/simstring/feature_extractor/word_ngram.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 simstring_fast-0.2.6/simstring/measure/__init__.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 simstring_fast-0.2.6/simstring/measure/base.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 simstring_fast-0.2.6/simstring/measure/cosine.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 simstring_fast-0.2.6/simstring/measure/dice.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 simstring_fast-0.2.6/simstring/measure/jaccard.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 simstring_fast-0.2.6/simstring/measure/overlap.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 simstring_fast-0.2.6/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 simstring_fast-0.2.6/LICENSE
+-rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 simstring_fast-0.2.6/README.md
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 simstring_fast-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 simstring_fast-0.2.6/PKG-INFO
```

### Comparing `simstring_fast-0.2.4/simstring/searcher.py` & `simstring_fast-0.2.6/simstring/searcher.py`

 * *Files identical despite different names*

### Comparing `simstring_fast-0.2.4/simstring/database/dict.py` & `simstring_fast-0.2.6/simstring/database/dict.py`

 * *Files identical despite different names*

### Comparing `simstring_fast-0.2.4/simstring/feature_extractor/base.py` & `simstring_fast-0.2.6/simstring/feature_extractor/base.py`

 * *Files identical despite different names*

### Comparing `simstring_fast-0.2.4/simstring/feature_extractor/character_ngram.py` & `simstring_fast-0.2.6/simstring/feature_extractor/character_ngram.py`

 * *Files identical despite different names*

### Comparing `simstring_fast-0.2.4/simstring/feature_extractor/word_ngram.py` & `simstring_fast-0.2.6/simstring/feature_extractor/word_ngram.py`

 * *Files identical despite different names*

### Comparing `simstring_fast-0.2.4/simstring/measure/cosine.py` & `simstring_fast-0.2.6/simstring/measure/cosine.py`

 * *Files identical despite different names*

### Comparing `simstring_fast-0.2.4/simstring/measure/dice.py` & `simstring_fast-0.2.6/simstring/measure/dice.py`

 * *Files identical despite different names*

### Comparing `simstring_fast-0.2.4/simstring/measure/jaccard.py` & `simstring_fast-0.2.6/simstring/measure/jaccard.py`

 * *Files identical despite different names*

### Comparing `simstring_fast-0.2.4/simstring/measure/overlap.py` & `simstring_fast-0.2.6/simstring/measure/overlap.py`

 * *Files identical despite different names*

### Comparing `simstring_fast-0.2.4/LICENSE` & `simstring_fast-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `simstring_fast-0.2.4/README.md` & `simstring_fast-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `simstring_fast-0.2.4/pyproject.toml` & `simstring_fast-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `simstring_fast-0.2.4/PKG-INFO` & `simstring_fast-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simstring-fast
-Version: 0.2.4
+Version: 0.2.6
 Summary: A fork of the Python implementation of the SimString by (Katsuma Narisawa), a simple and efficient algorithm for approximate string matching. Uses mypyc to improve speed
 Project-URL: Documentation, https://banking-circle-advanced-analytics.github.io/simstring-fast/
 Project-URL: Issues, https://github.com/banking-circle-advanced-analytics/simstring-fast
 Project-URL: Source, https://github.com/banking-circle-advanced-analytics/simstring-fast/issues
 Author-email: Ruben Menke <rum@bankingcircle.com>
 License-Expression: MIT
 License-File: LICENSE
```


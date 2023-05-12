# Comparing `tmp/simstring_fast-0.2.0.tar.gz` & `tmp/simstring_fast-0.2.4.tar.gz`

## Comparing `simstring_fast-0.2.0.tar` & `simstring_fast-0.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/__init__.py
--rw-r--r--   0        0        0     4838 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/searcher.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/database/__init__.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/database/base.py
--rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/database/dict.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/feature_extractor/__init__.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/feature_extractor/base.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/feature_extractor/character_ngram.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/feature_extractor/word_ngram.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/measure/__init__.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/measure/base.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/measure/cosine.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/measure/dice.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/measure/jaccard.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/measure/overlap.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/LICENSE
--rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/README.md
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/__init__.py
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/searcher.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/database/__init__.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/database/base.py
+-rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/database/dict.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/feature_extractor/__init__.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/feature_extractor/base.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/feature_extractor/character_ngram.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/feature_extractor/word_ngram.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/measure/__init__.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/measure/base.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/measure/cosine.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/measure/dice.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/measure/jaccard.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/simstring/measure/overlap.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/LICENSE
+-rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/README.md
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 simstring_fast-0.2.4/PKG-INFO
```

### Comparing `simstring_fast-0.2.0/simstring/searcher.py` & `simstring_fast-0.2.4/simstring/searcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding:utf-8 -*-
 from collections import defaultdict, OrderedDict
 from typing import List, Dict, Set, OrderedDict as OrderedDictType
 
+
 class Searcher:
     def __init__(self, db, measure) -> None:
         """Searcher class
 
         This is the main way of interacting with the simsting search.
 
         Args:
@@ -66,15 +67,17 @@
     def __min_overlap(
         self, query_size: int, candidate_feature_size: int, alpha: float
     ) -> int:
         return self.measure.minimum_common_feature_count(
             query_size, candidate_feature_size, alpha
         )
 
-    def __overlap_join(self, features: List[str], tau:int, candidate_feature_size: int) -> List[str]:
+    def __overlap_join(
+        self, features: List[str], tau: int, candidate_feature_size: int
+    ) -> List[str]:
         query_feature_size = len(features)
 
         features_mapped_to_lookup_strings_sets = {
             x: self.__lookup_strings_by_feature_set_size_and_feature(
                 candidate_feature_size, x
             )
             for x in features
```

### Comparing `simstring_fast-0.2.0/simstring/database/dict.py` & `simstring_fast-0.2.4/simstring/database/dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .base import BaseDatabase
 from simstring.feature_extractor.character_ngram import CharacterNgramFeatureExtractor
 from simstring.feature_extractor.word_ngram import WordNgramFeatureExtractor
 import pickle
 import ast
 from io import BufferedWriter
 
+
 def defaultdict_set():
     return defaultdict(set)
 
 
 class DictDatabase(BaseDatabase):
     def __init__(
         self,
@@ -28,15 +29,15 @@
         self._max_feature_size = 0
 
     def add(self, string: str) -> None:
         features = self.feature_extractor.features(string)
         size = len(features)
 
         self.strings.append(string)
-        
+
         if size not in self.feature_set_size_to_string_map:
             self.feature_set_size_to_string_map[size] = set()
 
         self.feature_set_size_to_string_map[size].add(string)
 
         self._min_feature_size = min(self._min_feature_size, size)
         self._max_feature_size = max(self._max_feature_size, size)
@@ -56,22 +57,22 @@
         return self._min_feature_size
 
     def max_feature_size(self) -> int:
         return self._max_feature_size
 
     def to_pickle(self, f: BufferedWriter) -> None:
         """Hack to get object savable with mypyc
-        
+
         Save a db object to pickle with:
 
         >>> with open("test.pkl", "wb") as f:
         ...     db.to_pickle(f)
 
         Args:
-            f (BufferedWriter): File object writer, where to save the data      
+            f (BufferedWriter): File object writer, where to save the data
         """
         data = {
             "feature_extractor": self.feature_extractor.__define__(),
             "strings": self.strings,
             "feature_set_size_to_string_map": self.feature_set_size_to_string_map,
             "feature_set_size_and_feature_to_string_map": self.feature_set_size_and_feature_to_string_map,
             "_min_feature_size": self._min_feature_size,
@@ -80,25 +81,25 @@
         pickle.dump(data, f)
 
     @staticmethod
     def from_dict(data: dict) -> "DictDatabase":
         """Hack to get object loadable with mypyc
 
         Careful, this runs eval on data["feature_extractor"], so only use pickles you trust.
-        
+
         Load a saved DB as a dict and then instatiate an object from that dict:
 
         Example:
         >>> with open("test.pkl", "rb") as f:
         ...     data = pickle.load(f)
 
         >>> new = DictDatabase.from_dict(data)
 
         Args:
-            data (dict): A dictionary as created by `to_pickle` 
+            data (dict): A dictionary as created by `to_pickle`
 
         """
         obj = DictDatabase(eval(data["feature_extractor"]))
         obj.strings = data["strings"]
         obj.feature_set_size_to_string_map.update(
             data["feature_set_size_to_string_map"]
         )
```

### Comparing `simstring_fast-0.2.0/simstring/feature_extractor/base.py` & `simstring_fast-0.2.4/simstring/feature_extractor/base.py`

 * *Files identical despite different names*

### Comparing `simstring_fast-0.2.0/simstring/feature_extractor/character_ngram.py` & `simstring_fast-0.2.4/simstring/feature_extractor/character_ngram.py`

 * *Files identical despite different names*

### Comparing `simstring_fast-0.2.0/simstring/feature_extractor/word_ngram.py` & `simstring_fast-0.2.4/simstring/feature_extractor/word_ngram.py`

 * *Files identical despite different names*

### Comparing `simstring_fast-0.2.0/simstring/measure/cosine.py` & `simstring_fast-0.2.4/simstring/measure/cosine.py`

 * *Files identical despite different names*

### Comparing `simstring_fast-0.2.0/simstring/measure/dice.py` & `simstring_fast-0.2.4/simstring/measure/dice.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import math
 from typing import Iterable
 
+
 class DiceMeasure:
     def min_feature_size(self, query_size: int, alpha: float) -> int:
         return int(math.ceil(alpha * 1.0 / (2 - alpha) * query_size))
 
     def max_feature_size(self, query_size: int, alpha: float) -> int:
         return int(math.floor((2 - alpha) * query_size * 1.0 / alpha))
```

### Comparing `simstring_fast-0.2.0/simstring/measure/jaccard.py` & `simstring_fast-0.2.4/simstring/measure/jaccard.py`

 * *Files identical despite different names*

### Comparing `simstring_fast-0.2.0/simstring/measure/overlap.py` & `simstring_fast-0.2.4/simstring/measure/overlap.py`

 * *Files identical despite different names*

### Comparing `simstring_fast-0.2.0/LICENSE` & `simstring_fast-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simstring_fast-0.2.0/README.md` & `simstring_fast-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `simstring_fast-0.2.0/pyproject.toml` & `simstring_fast-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `simstring_fast-0.2.0/PKG-INFO` & `simstring_fast-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simstring-fast
-Version: 0.2.0
+Version: 0.2.4
 Summary: A fork of the Python implementation of the SimString by (Katsuma Narisawa), a simple and efficient algorithm for approximate string matching. Uses mypyc to improve speed
 Project-URL: Documentation, https://banking-circle-advanced-analytics.github.io/simstring-fast/
 Project-URL: Issues, https://github.com/banking-circle-advanced-analytics/simstring-fast
 Project-URL: Source, https://github.com/banking-circle-advanced-analytics/simstring-fast/issues
 Author-email: Ruben Menke <rum@bankingcircle.com>
 License-Expression: MIT
 License-File: LICENSE
```


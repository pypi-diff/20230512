# Comparing `tmp/simstring_fast-0.1.7.tar.gz` & `tmp/simstring_fast-0.2.0.tar.gz`

## Comparing `simstring_fast-0.1.7.tar` & `simstring_fast-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 simstring_fast-0.1.7/simstring/__init__.py
--rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 simstring_fast-0.1.7/simstring/searcher.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 simstring_fast-0.1.7/simstring/database/__init__.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 simstring_fast-0.1.7/simstring/database/base.py
--rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 simstring_fast-0.1.7/simstring/database/dict.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 simstring_fast-0.1.7/simstring/feature_extractor/__init__.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 simstring_fast-0.1.7/simstring/feature_extractor/base.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 simstring_fast-0.1.7/simstring/feature_extractor/character_ngram.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 simstring_fast-0.1.7/simstring/feature_extractor/word_ngram.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 simstring_fast-0.1.7/simstring/measure/__init__.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 simstring_fast-0.1.7/simstring/measure/base.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 simstring_fast-0.1.7/simstring/measure/cosine.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 simstring_fast-0.1.7/simstring/measure/dice.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 simstring_fast-0.1.7/simstring/measure/jaccard.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 simstring_fast-0.1.7/simstring/measure/overlap.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 simstring_fast-0.1.7/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 simstring_fast-0.1.7/LICENSE
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 simstring_fast-0.1.7/README.md
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 simstring_fast-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 simstring_fast-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/__init__.py
+-rw-r--r--   0        0        0     4838 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/searcher.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/database/__init__.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/database/base.py
+-rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/database/dict.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/feature_extractor/__init__.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/feature_extractor/base.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/feature_extractor/character_ngram.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/feature_extractor/word_ngram.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/measure/__init__.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/measure/base.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/measure/cosine.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/measure/dice.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/measure/jaccard.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/simstring/measure/overlap.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/README.md
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 simstring_fast-0.2.0/PKG-INFO
```

### Comparing `simstring_fast-0.1.7/simstring/searcher.py` & `simstring_fast-0.2.0/simstring/searcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 # -*- coding:utf-8 -*-
 from collections import defaultdict, OrderedDict
-from typing import List, Tuple, Dict
-
-from typing import OrderedDict as OrderedDictType
-
+from typing import List, Dict, Set, OrderedDict as OrderedDictType
 
 class Searcher:
     def __init__(self, db, measure) -> None:
         """Searcher class
 
         This is the main way of interacting with the simsting search.
 
@@ -69,31 +66,33 @@
     def __min_overlap(
         self, query_size: int, candidate_feature_size: int, alpha: float
     ) -> int:
         return self.measure.minimum_common_feature_count(
             query_size, candidate_feature_size, alpha
         )
 
-    def __overlap_join(self, features, tau, candidate_feature_size: int) -> List[str]:
+    def __overlap_join(self, features: List[str], tau:int, candidate_feature_size: int) -> List[str]:
         query_feature_size = len(features)
 
         features_mapped_to_lookup_strings_sets = {
             x: self.__lookup_strings_by_feature_set_size_and_feature(
                 candidate_feature_size, x
             )
             for x in features
         }
 
         features.sort(key=lambda x: len(features_mapped_to_lookup_strings_sets[x]))
 
         # candidate_string_to_matched_count : Dict[str,int] = defaultdict(int) # Only in 3.10 and later
-        candidate_string_to_matched_count: Dict = defaultdict(int)
+        candidate_string_to_matched_count: Dict[str, int] = dict()
         results = []
         for feature in features[0 : query_feature_size - tau + 1]:
             for s in features_mapped_to_lookup_strings_sets[feature]:
+                if s not in candidate_string_to_matched_count:
+                    candidate_string_to_matched_count[s] = 0
                 candidate_string_to_matched_count[s] += 1
 
         # The next loop does not run for tau = 1, hence candidates are never checked, while all satisfies the criteria
         if tau == 1:
             results = list(candidate_string_to_matched_count.keys())
 
         for (
@@ -111,15 +110,15 @@
                 if candidate_match_count + remaining_feature_count < tau:
                     break
 
         return results
 
     def __lookup_strings_by_feature_set_size_and_feature(
         self, feature_size: int, feature: str
-    ):
+    ) -> Set[str]:
         if feature not in self.lookup_strings_result[feature_size]:
             self.lookup_strings_result[feature_size][
                 feature
             ] = self.db.lookup_strings_by_feature_set_size_and_feature(
                 feature_size, feature
             )
         return self.lookup_strings_result[feature_size][feature]
```

### Comparing `simstring_fast-0.1.7/simstring/database/dict.py` & `simstring_fast-0.2.0/simstring/database/dict.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,28 +16,30 @@
         self,
         feature_extractor: Union[
             CharacterNgramFeatureExtractor, WordNgramFeatureExtractor
         ],
     ):
         self.feature_extractor = feature_extractor
         self.strings: List[str] = []
-        self.feature_set_size_to_string_map: Dict[int, Set[str]] = defaultdict(
-            set
-        )  # 3.10 and up only
+        self.feature_set_size_to_string_map: Dict[int, Set[str]] = dict()
         self.feature_set_size_and_feature_to_string_map: dict = defaultdict(
             defaultdict_set
         )
         self._min_feature_size = 9999999
         self._max_feature_size = 0
 
     def add(self, string: str) -> None:
         features = self.feature_extractor.features(string)
         size = len(features)
 
         self.strings.append(string)
+        
+        if size not in self.feature_set_size_to_string_map:
+            self.feature_set_size_to_string_map[size] = set()
+
         self.feature_set_size_to_string_map[size].add(string)
 
         self._min_feature_size = min(self._min_feature_size, size)
         self._max_feature_size = max(self._max_feature_size, size)
 
         for feature in features:
             self.feature_set_size_and_feature_to_string_map[size][feature].add(string)
@@ -52,15 +54,14 @@
 
     def min_feature_size(self) -> int:
         return self._min_feature_size
 
     def max_feature_size(self) -> int:
         return self._max_feature_size
 
-
     def to_pickle(self, f: BufferedWriter) -> None:
         """Hack to get object savable with mypyc
         
         Save a db object to pickle with:
 
         >>> with open("test.pkl", "wb") as f:
         ...     db.to_pickle(f)
@@ -74,17 +75,14 @@
             "feature_set_size_to_string_map": self.feature_set_size_to_string_map,
             "feature_set_size_and_feature_to_string_map": self.feature_set_size_and_feature_to_string_map,
             "_min_feature_size": self._min_feature_size,
             "_max_feature_size": self._max_feature_size,
         }
         pickle.dump(data, f)
 
-   
-
-
     @staticmethod
     def from_dict(data: dict) -> "DictDatabase":
         """Hack to get object loadable with mypyc
 
         Careful, this runs eval on data["feature_extractor"], so only use pickles you trust.
         
         Load a saved DB as a dict and then instatiate an object from that dict:
@@ -107,16 +105,54 @@
         obj.feature_set_size_and_feature_to_string_map.update(
             data["feature_set_size_and_feature_to_string_map"]
         )
         obj._min_feature_size = data["_min_feature_size"]
         obj._max_feature_size = data["_max_feature_size"]
         return obj
 
-    @classmethod
-    def from_file(cls, filename: str) -> "DictDatabase":
-        with open(filename, "rb") as f:
-            data = pickle.load(f)
-        return cls.from_dict(data)  
+    def save(self, filename: str) -> None:
+        """Save the database to a file as defined by filename.
 
-    def to_file(self, filename: str) -> None:
+        Args:
+            filename: Filename to save the db at. Should include file extension.
+
+        Returns:
+            None
+        """
         with open(filename, "wb") as f:
-            self.to_pickle(f)
+            pickle.dump(self, f)
+
+    @staticmethod
+    def load(filename: str) -> "DictDatabase":
+        """Load db from a file
+
+        Args:
+            filename (str): Name of the file to load
+
+        Returns:
+            DictDatabase: the db
+        """
+        with open(filename, "rb") as f:
+            db = pickle.load(f)
+        return db
+
+    def dumps(self) -> bytes:
+        """Generate pickle byte stream
+
+        Returns:
+            _type_: _description_
+        """
+        return pickle.dumps(self)
+
+    @staticmethod
+    def loads(binary_data: bytes) -> "DictDatabase":
+        """Load a binary string representing a database
+
+        Initially only unpickles the data
+
+        Args:
+            binary_data (str): String of data to unpickle
+
+        Returns:
+            Model object
+        """
+        return pickle.loads(binary_data)
```

### Comparing `simstring_fast-0.1.7/simstring/feature_extractor/base.py` & `simstring_fast-0.2.0/simstring/feature_extractor/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,7 @@
             unique_list.append(f"{val}_{counter[val]}")
 
         return unique_list
 
     def __define__(self) -> str:
         "Custom representation string"
         raise NotImplementedError()
-
-    def __getstate__(self):
-        """To pickle the object"""
-        return self.__dict__
-
-    def __setstate__(self, d):
-        """To unpickle the object"""
-        self.__dict__ = d
```

### Comparing `simstring_fast-0.1.7/simstring/feature_extractor/character_ngram.py` & `simstring_fast-0.2.0/simstring/feature_extractor/character_ngram.py`

 * *Files identical despite different names*

### Comparing `simstring_fast-0.1.7/simstring/feature_extractor/word_ngram.py` & `simstring_fast-0.2.0/simstring/feature_extractor/word_ngram.py`

 * *Files identical despite different names*

### Comparing `simstring_fast-0.1.7/simstring/measure/dice.py` & `simstring_fast-0.2.0/simstring/measure/cosine.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import math
 from typing import Iterable
 
-from .base import BaseMeasure
 
-
-class DiceMeasure(BaseMeasure):
+class CosineMeasure:
     def min_feature_size(self, query_size: int, alpha: float) -> int:
-        return int(math.ceil(alpha * 1.0 / (2 - alpha) * query_size))
+        return int(math.ceil(alpha * alpha * query_size))
 
     def max_feature_size(self, query_size: int, alpha: float) -> int:
-        return int(math.floor((2 - alpha) * query_size * 1.0 / alpha))
+        return int(math.floor(query_size / (alpha * alpha)))
 
     def minimum_common_feature_count(
         self, query_size: int, y_size: int, alpha: float
     ) -> int:
-        return int(math.ceil(0.5 * alpha * query_size * y_size))
+        return int(math.ceil(alpha * math.sqrt(query_size * y_size)))
 
     def similarity(self, X: Iterable[str], Y: Iterable[str]) -> float:
-        return len(set(X) & set(Y)) * 2.0 / (len(set(X)) + len(set(Y)))
+        return len(set(X) & set(Y)) / math.sqrt(len(set(X)) * len(set(Y)))
```

### Comparing `simstring_fast-0.1.7/simstring/measure/jaccard.py` & `simstring_fast-0.2.0/simstring/measure/jaccard.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import math
 from typing import Iterable
-from .base import BaseMeasure
 
 
-class JaccardMeasure(BaseMeasure):
+class JaccardMeasure:
     def min_feature_size(self, query_size: int, alpha: float) -> int:
         return int(math.ceil(alpha * query_size))
 
     def max_feature_size(self, query_size: int, alpha: float) -> int:
         return int(math.floor(query_size / alpha))
 
     def minimum_common_feature_count(
```

### Comparing `simstring_fast-0.1.7/simstring/measure/overlap.py` & `simstring_fast-0.2.0/simstring/measure/overlap.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 import math
 from typing import Iterable
-from .base import BaseMeasure
 
 
-class OverlapMeasure(BaseMeasure):
+class OverlapMeasure:
     def __init__(self, db=None, maxsize: int = 100) -> None:
         super().__init__()
         if db:
             self.maxsize = db.max_feature_size()
         else:
             self.maxsize = maxsize
 
-    def min_feature_size(self, query_size, alpha) -> int:
+    def min_feature_size(self, query_size: int, alpha: float) -> int:
         # return 1 # Not sure the below isn't sufficient
         return math.floor(query_size * alpha) or 1
 
-    def max_feature_size(self, query_size, alpha) -> int:
+    def max_feature_size(self, query_size: int, alpha: float) -> int:
         return self.maxsize
 
     def minimum_common_feature_count(
         self, query_size: int, y_size: int, alpha: float
     ) -> int:
         return int(math.ceil(alpha * min(query_size, y_size)))
 
     def similarity(self, X: Iterable[str], Y: Iterable[str]) -> int:
         return min(len(set(X)), len(set(Y)))
 
 
-class LeftOverlapMeasure(BaseMeasure):
+class LeftOverlapMeasure:
     def __init__(self, db=None, maxsize: int = 100) -> None:
         super().__init__()
         if db:
             self.maxsize = db.max_feature_size()
         else:
             self.maxsize = maxsize
 
-    def min_feature_size(self, query_size, alpha) -> int:
+    def min_feature_size(self, query_size: int, alpha: float) -> int:
         return math.floor(query_size * alpha) or 1
 
-    def max_feature_size(self, query_size, alpha) -> int:
+    def max_feature_size(self, query_size: int, alpha: float) -> int:
         return self.maxsize
 
     def minimum_common_feature_count(
         self, query_size: int, y_size: int, alpha: float
     ) -> int:
         return math.floor(query_size * alpha) or 1
```

### Comparing `simstring_fast-0.1.7/LICENSE` & `simstring_fast-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simstring_fast-0.1.7/README.md` & `simstring_fast-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # simstring
 [![PyPI - Status](https://img.shields.io/pypi/status/simstring-fast.svg)](https://pypi.org/project/simstring-fast/)
 [![PyPI version](https://badge.fury.io/py/simstring-fast.svg)](https://badge.fury.io/py/simstring-fast)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/simstring-fast)
 [![MIT License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](LICENSE)
 
+![icon](simstring/docs/strings_icon.png)
+
 A Python implementation of the [SimString](http://www.chokkan.org/software/simstring/index.html.en), a simple and efficient algorithm for approximate string matching.
 
 Docs are [here](https://banking-circle-advanced-analytics.github.io/simstring-fast/)
 
 ## Features
 With this library, you can extract strings/texts which has certain similarity from large amount of strings/texts. It will help you when you develop applications related to language processing.
 
@@ -46,16 +48,16 @@
 # => ['foo', 'fooo']
 ```
 
 If you want to use other feature, measure, and database, simply replace these classes. You can replace these classes easily by your own classes if you want.
 
 ```python
 from simstring.feature_extractor.word_ngram import WordNgramFeatureExtractor
-from simstring.measure import JaccardMeasure
-from simstring.database import DictDatabase
+from simstring.measure.jaccard import JaccardMeasure
+from simstring.database.dict import DictDatabase
 from simstring.searcher import Searcher
 
 db = DictDatabase(WordNgramFeatureExtractor(2))
 db.add('You are so cool.')
 
 searcher = Searcher(db, JaccardMeasure())
 results = searcher.search('You are cool.', 0.8)
```

### Comparing `simstring_fast-0.1.7/pyproject.toml` & `simstring_fast-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "simstring-fast"
 description = "A fork of the Python implementation of the SimString by (Katsuma Narisawa), a simple and efficient algorithm for approximate string matching. Uses mypyc to improve speed"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Ruben Menke", email = "rum@bankingcircle.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
@@ -46,15 +46,16 @@
   "--install-types"
 ]
 
 [tool.hatch.envs.test]
 dependencies = [
   "pytest",
   "pytest-cov",
-  "build"
+  "build",
+  "cython"
 ]
 
 [tool.hatch.envs.default.scripts]
 version = "python --version"
 cov = "pytest --cov-report=term --cov-config=pyproject.toml"
 no-cov = "cov --no-cov {args}"
 build = "python -m build"
@@ -91,11 +92,13 @@
 
 
 
 [tool.hatch.envs.benchmark]
 dependencies = [
    "pyinstrument", "benchmarker" , "numpy"
 ]
+[[tool.hatch.envs.benchmark.matrix]]
+python = [ "38", "39", "310", "311"]
 
 [tool.hatch.envs.benchmark.scripts]
 run = "python dev/benchmark.py"
-instrument = "python dev/company_names.py"
+instrument = "pip install . && python dev/company_names.py"
```

### Comparing `simstring_fast-0.1.7/PKG-INFO` & `simstring_fast-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: simstring-fast
-Version: 0.1.7
+Version: 0.2.0
 Summary: A fork of the Python implementation of the SimString by (Katsuma Narisawa), a simple and efficient algorithm for approximate string matching. Uses mypyc to improve speed
 Project-URL: Documentation, https://banking-circle-advanced-analytics.github.io/simstring-fast/
 Project-URL: Issues, https://github.com/banking-circle-advanced-analytics/simstring-fast
 Project-URL: Source, https://github.com/banking-circle-advanced-analytics/simstring-fast/issues
 Author-email: Ruben Menke <rum@bankingcircle.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # simstring
 [![PyPI - Status](https://img.shields.io/pypi/status/simstring-fast.svg)](https://pypi.org/project/simstring-fast/)
 [![PyPI version](https://badge.fury.io/py/simstring-fast.svg)](https://badge.fury.io/py/simstring-fast)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/simstring-fast)
 [![MIT License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](LICENSE)
 
+![icon](simstring/docs/strings_icon.png)
+
 A Python implementation of the [SimString](http://www.chokkan.org/software/simstring/index.html.en), a simple and efficient algorithm for approximate string matching.
 
 Docs are [here](https://banking-circle-advanced-analytics.github.io/simstring-fast/)
 
 ## Features
 With this library, you can extract strings/texts which has certain similarity from large amount of strings/texts. It will help you when you develop applications related to language processing.
 
@@ -66,16 +68,16 @@
 # => ['foo', 'fooo']
 ```
 
 If you want to use other feature, measure, and database, simply replace these classes. You can replace these classes easily by your own classes if you want.
 
 ```python
 from simstring.feature_extractor.word_ngram import WordNgramFeatureExtractor
-from simstring.measure import JaccardMeasure
-from simstring.database import DictDatabase
+from simstring.measure.jaccard import JaccardMeasure
+from simstring.database.dict import DictDatabase
 from simstring.searcher import Searcher
 
 db = DictDatabase(WordNgramFeatureExtractor(2))
 db.add('You are so cool.')
 
 searcher = Searcher(db, JaccardMeasure())
 results = searcher.search('You are cool.', 0.8)
```


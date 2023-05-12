# Comparing `tmp/pyprocessors-chunk_sentences-0.5.10.tar.gz` & `tmp/pyprocessors-chunk_sentences-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprocessors-chunk_sentences-0.5.10.tar", last modified: Fri May 12 11:41:56 2023, max compression
+gzip compressed data, was "pyprocessors-chunk_sentences-0.5.5.tar", last modified: Fri Feb 24 14:18:21 2023, max compression
```

## Comparing `pyprocessors-chunk_sentences-0.5.10.tar` & `pyprocessors-chunk_sentences-0.5.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      504 2023-02-24 10:10:11.842208 pyprocessors-chunk_sentences-0.5.10/.bumpversion.cfg
--rw-r--r--   0        0        0     1760 2023-02-24 10:10:11.842208 pyprocessors-chunk_sentences-0.5.10/.gitignore
--rw-r--r--   0        0        0      419 2023-02-24 10:10:11.842208 pyprocessors-chunk_sentences-0.5.10/.pre-commit-config.yaml
--rw-r--r--   0        0        0      202 2023-02-24 10:10:11.842208 pyprocessors-chunk_sentences-0.5.10/.readthedocs.yml
--rw-r--r--   0        0        0      124 2023-02-24 10:10:11.842208 pyprocessors-chunk_sentences-0.5.10/AUTHORS.md
--rw-r--r--   0        0        0      268 2023-02-24 10:10:11.842208 pyprocessors-chunk_sentences-0.5.10/CHANGELOG.md
--rw-r--r--   0        0        0      476 2023-02-24 10:10:11.842208 pyprocessors-chunk_sentences-0.5.10/Dockerfile
--rw-r--r--   0        0        0    10243 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.10/Jenkinsfile
--rw-r--r--   0        0        0     1082 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.10/LICENSE
--rw-r--r--   0        0        0     1648 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.10/README.md
--rw-r--r--   0        0        0      955 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.10/RELEASE.md
--rw-r--r--   0        0        0     1559 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.10/bumpversion.py
--rw-r--r--   0        0        0       62 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.10/docs/.gitignore
--rw-r--r--   0        0        0      268 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.10/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.10/docs/LICENSE
--rw-r--r--   0        0        0        0 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.10/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.10/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     2914 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.10/docs/conf.py
--rw-r--r--   0        0        0      149 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.10/docs/index.rst
--rw-r--r--   0        0        0       98 2023-02-24 10:10:11.844208 pyprocessors-chunk_sentences-0.5.10/mypy.ini
--rw-r--r--   0        0        0     2289 2023-02-24 10:10:11.844208 pyprocessors-chunk_sentences-0.5.10/pyproject.toml
--rw-r--r--   0        0        0       64 2023-05-12 11:41:54.841753 pyprocessors-chunk_sentences-0.5.10/src/pyprocessors_chunk_sentences/__init__.py
--rw-r--r--   0        0        0     6289 2023-05-12 11:36:31.417140 pyprocessors-chunk_sentences-0.5.10/src/pyprocessors_chunk_sentences/chunk_sentences.py
--rw-r--r--   0        0        0        0 2023-02-24 10:10:11.844208 pyprocessors-chunk_sentences-0.5.10/tests/__init__.py
--rw-r--r--   0        0        0     3286 2023-02-24 10:10:11.844208 pyprocessors-chunk_sentences-0.5.10/tests/data/news_fr.json
--rw-r--r--   0        0        0     3002 2023-05-12 11:41:52.021678 pyprocessors-chunk_sentences-0.5.10/tests/data/news_fr_char_chunked.json
--rw-r--r--   0        0        0     2900 2023-05-12 11:41:52.022678 pyprocessors-chunk_sentences-0.5.10/tests/data/news_fr_char_chunked2.json
--rw-r--r--   0        0        0     3102 2023-05-12 11:41:52.025678 pyprocessors-chunk_sentences-0.5.10/tests/data/news_fr_token_chunked.json
--rw-r--r--   0        0        0     2900 2023-05-12 11:41:52.033678 pyprocessors-chunk_sentences-0.5.10/tests/data/news_fr_token_chunked2.json
--rw-r--r--   0        0        0     4671 2023-02-24 10:10:11.844208 pyprocessors-chunk_sentences-0.5.10/tests/test_chunk_sentences.py
--rw-r--r--   0        0        0      927 2023-02-24 10:10:11.845208 pyprocessors-chunk_sentences-0.5.10/tox.ini
--rw-r--r--   0        0        0     1385 1970-01-01 00:00:00.000000 pyprocessors-chunk_sentences-0.5.10/setup.py
--rw-r--r--   0        0        0     3430 1970-01-01 00:00:00.000000 pyprocessors-chunk_sentences-0.5.10/PKG-INFO
+-rw-r--r--   0        0        0      504 2023-02-24 10:10:11.842208 pyprocessors-chunk_sentences-0.5.5/.bumpversion.cfg
+-rw-r--r--   0        0        0     1760 2023-02-24 10:10:11.842208 pyprocessors-chunk_sentences-0.5.5/.gitignore
+-rw-r--r--   0        0        0      419 2023-02-24 10:10:11.842208 pyprocessors-chunk_sentences-0.5.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      202 2023-02-24 10:10:11.842208 pyprocessors-chunk_sentences-0.5.5/.readthedocs.yml
+-rw-r--r--   0        0        0      124 2023-02-24 10:10:11.842208 pyprocessors-chunk_sentences-0.5.5/AUTHORS.md
+-rw-r--r--   0        0        0      268 2023-02-24 10:10:11.842208 pyprocessors-chunk_sentences-0.5.5/CHANGELOG.md
+-rw-r--r--   0        0        0      476 2023-02-24 10:10:11.842208 pyprocessors-chunk_sentences-0.5.5/Dockerfile
+-rw-r--r--   0        0        0    10243 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.5/Jenkinsfile
+-rw-r--r--   0        0        0     1082 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.5/LICENSE
+-rw-r--r--   0        0        0     1648 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.5/README.md
+-rw-r--r--   0        0        0      955 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.5/RELEASE.md
+-rw-r--r--   0        0        0     1559 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.5/bumpversion.py
+-rw-r--r--   0        0        0       62 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.5/docs/.gitignore
+-rw-r--r--   0        0        0      268 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.5/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.5/docs/LICENSE
+-rw-r--r--   0        0        0        0 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.5/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.5/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     2914 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.5/docs/conf.py
+-rw-r--r--   0        0        0      149 2023-02-24 10:10:11.843208 pyprocessors-chunk_sentences-0.5.5/docs/index.rst
+-rw-r--r--   0        0        0       98 2023-02-24 10:10:11.844208 pyprocessors-chunk_sentences-0.5.5/mypy.ini
+-rw-r--r--   0        0        0     2289 2023-02-24 10:10:11.844208 pyprocessors-chunk_sentences-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0       63 2023-02-24 14:18:20.466203 pyprocessors-chunk_sentences-0.5.5/src/pyprocessors_chunk_sentences/__init__.py
+-rw-r--r--   0        0        0     6283 2023-02-24 10:23:31.993033 pyprocessors-chunk_sentences-0.5.5/src/pyprocessors_chunk_sentences/chunk_sentences.py
+-rw-r--r--   0        0        0        0 2023-02-24 10:10:11.844208 pyprocessors-chunk_sentences-0.5.5/tests/__init__.py
+-rw-r--r--   0        0        0     3286 2023-02-24 10:10:11.844208 pyprocessors-chunk_sentences-0.5.5/tests/data/news_fr.json
+-rw-r--r--   0        0        0     3002 2023-02-24 14:18:17.620129 pyprocessors-chunk_sentences-0.5.5/tests/data/news_fr_char_chunked.json
+-rw-r--r--   0        0        0     2900 2023-02-24 14:18:17.621129 pyprocessors-chunk_sentences-0.5.5/tests/data/news_fr_char_chunked2.json
+-rw-r--r--   0        0        0     3102 2023-02-24 14:18:17.624129 pyprocessors-chunk_sentences-0.5.5/tests/data/news_fr_token_chunked.json
+-rw-r--r--   0        0        0     2900 2023-02-24 14:18:17.630129 pyprocessors-chunk_sentences-0.5.5/tests/data/news_fr_token_chunked2.json
+-rw-r--r--   0        0        0     4671 2023-02-24 10:10:11.844208 pyprocessors-chunk_sentences-0.5.5/tests/test_chunk_sentences.py
+-rw-r--r--   0        0        0      927 2023-02-24 10:10:11.845208 pyprocessors-chunk_sentences-0.5.5/tox.ini
+-rw-r--r--   0        0        0     1384 1970-01-01 00:00:00.000000 pyprocessors-chunk_sentences-0.5.5/setup.py
+-rw-r--r--   0        0        0     3429 1970-01-01 00:00:00.000000 pyprocessors-chunk_sentences-0.5.5/PKG-INFO
```

### Comparing `pyprocessors-chunk_sentences-0.5.10/.gitignore` & `pyprocessors-chunk_sentences-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pyprocessors-chunk_sentences-0.5.10/Jenkinsfile` & `pyprocessors-chunk_sentences-0.5.5/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `pyprocessors-chunk_sentences-0.5.10/LICENSE` & `pyprocessors-chunk_sentences-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprocessors-chunk_sentences-0.5.10/README.md` & `pyprocessors-chunk_sentences-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `pyprocessors-chunk_sentences-0.5.10/RELEASE.md` & `pyprocessors-chunk_sentences-0.5.5/RELEASE.md`

 * *Files identical despite different names*

### Comparing `pyprocessors-chunk_sentences-0.5.10/bumpversion.py` & `pyprocessors-chunk_sentences-0.5.5/bumpversion.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-chunk_sentences-0.5.10/docs/LICENSE` & `pyprocessors-chunk_sentences-0.5.5/docs/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprocessors-chunk_sentences-0.5.10/docs/conf.py` & `pyprocessors-chunk_sentences-0.5.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-chunk_sentences-0.5.10/pyproject.toml` & `pyprocessors-chunk_sentences-0.5.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyprocessors-chunk_sentences-0.5.10/src/pyprocessors_chunk_sentences/chunk_sentences.py` & `pyprocessors-chunk_sentences-0.5.5/src/pyprocessors_chunk_sentences/chunk_sentences.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,11 +135,11 @@
         self.start = start or sentence.start
         self.end = end or sentence.end
 
 
 @lru_cache(maxsize=None)
 def get_blingfire(model: str):
     # load a provided with the package model
-    if model == TokenModel.wbd.value:
+    if model == TokenModel.wbd:
         return -1
     h = blingfire.load_model(os.path.join(os.path.dirname(blingfire.__file__), f"{model}.bin"))
     return h
```

### Comparing `pyprocessors-chunk_sentences-0.5.10/tests/data/news_fr.json` & `pyprocessors-chunk_sentences-0.5.5/tests/data/news_fr.json`

 * *Files identical despite different names*

### Comparing `pyprocessors-chunk_sentences-0.5.10/tests/data/news_fr_char_chunked.json` & `pyprocessors-chunk_sentences-0.5.5/tests/data/news_fr_char_chunked.json`

 * *Files identical despite different names*

### Comparing `pyprocessors-chunk_sentences-0.5.10/tests/data/news_fr_char_chunked2.json` & `pyprocessors-chunk_sentences-0.5.5/tests/data/news_fr_char_chunked2.json`

 * *Files identical despite different names*

### Comparing `pyprocessors-chunk_sentences-0.5.10/tests/data/news_fr_token_chunked.json` & `pyprocessors-chunk_sentences-0.5.5/tests/data/news_fr_token_chunked.json`

 * *Files identical despite different names*

### Comparing `pyprocessors-chunk_sentences-0.5.10/tests/data/news_fr_token_chunked2.json` & `pyprocessors-chunk_sentences-0.5.5/tests/data/news_fr_token_chunked2.json`

 * *Files identical despite different names*

### Comparing `pyprocessors-chunk_sentences-0.5.10/tests/test_chunk_sentences.py` & `pyprocessors-chunk_sentences-0.5.5/tests/test_chunk_sentences.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-chunk_sentences-0.5.10/tox.ini` & `pyprocessors-chunk_sentences-0.5.5/tox.ini`

 * *Files identical despite different names*

### Comparing `pyprocessors-chunk_sentences-0.5.10/setup.py` & `pyprocessors-chunk_sentences-0.5.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
           'dirty-equals']}
 
 entry_points = \
 {'pyprocessors.plugins': ['chunk_sentences = '
                           'pyprocessors_chunk_sentences.chunk_sentences:ChunkSentencesProcessor']}
 
 setup(name='pyprocessors-chunk_sentences',
-      version='0.5.10',
+      version='0.5.5',
       description='Sherpa sentence chunking processor',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://github.com/oterrier/pyprocessors_chunk_sentences/',
       packages=packages,
       package_data=package_data,
       package_dir=package_dir,
```

### Comparing `pyprocessors-chunk_sentences-0.5.10/PKG-INFO` & `pyprocessors-chunk_sentences-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprocessors-chunk_sentences
-Version: 0.5.10
+Version: 0.5.5
 Summary: Sherpa sentence chunking processor
 Home-page: https://github.com/oterrier/pyprocessors_chunk_sentences/
 Keywords: 
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```


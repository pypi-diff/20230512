# Comparing `tmp/s2aff-0.20.tar.gz` & `tmp/s2aff-0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2aff-0.20.tar", last modified: Thu May 11 17:55:27 2023, max compression
+gzip compressed data, was "s2aff-0.21.tar", last modified: Fri May 12 14:58:42 2023, max compression
```

## Comparing `s2aff-0.20.tar` & `s2aff-0.21.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-11 17:55:27.378123 s2aff-0.20/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.20/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-11 17:55:27.377929 s2aff-0.20/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.20/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-11 17:55:27.371046 s2aff-0.20/data/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.20/data/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.20/data/combine_gold.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.20/data/download_latest_ror.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-11 17:55:27.371387 s2aff-0.20/data/ner_model/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.20/data/ner_model/__init__.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-11 17:55:27.374363 s2aff-0.20/s2aff/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8094 2023-05-08 19:46:34.000000 s2aff-0.20/s2aff/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-08 19:52:35.000000 s2aff-0.20/s2aff/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.20/s2aff/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.20/s2aff/features.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.20/s2aff/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-11 17:45:39.000000 s2aff-0.20/s2aff/lightgbm_helpers.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-08 19:46:34.000000 s2aff-0.20/s2aff/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    34343 2023-05-08 19:46:34.000000 s2aff-0.20/s2aff/ror.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.20/s2aff/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-11 17:55:27.375984 s2aff-0.20/s2aff/timo/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.20/s2aff/timo/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.20/s2aff/timo/integration_test.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-08 19:46:34.000000 s2aff-0.20/s2aff/timo/interface.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-11 17:55:27.375352 s2aff-0.20/s2aff.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-11 17:55:26.000000 s2aff-0.20/s2aff.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-11 17:55:27.000000 s2aff-0.20/s2aff.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-11 17:55:26.000000 s2aff-0.20/s2aff.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-11 17:55:27.000000 s2aff-0.20/s2aff.egg-info/requires.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-11 17:55:27.000000 s2aff-0.20/s2aff.egg-info/top_level.txt
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-11 17:55:27.377629 s2aff-0.20/scripts/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.20/scripts/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-08 19:46:34.000000 s2aff-0.20/scripts/approximate_runtime_and_memory_usage.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-08 19:46:34.000000 s2aff-0.20/scripts/evaluate_first_stage_ranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-08 19:46:34.000000 s2aff-0.20/scripts/generate_lightgbm_training_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.20/scripts/train_lightgbm_reranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.20/scripts/train_ner_model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.20/scripts/update_openalex_works_counts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-11 17:55:27.378220 s2aff-0.20/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-11 17:55:21.000000 s2aff-0.20/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-12 14:58:42.770272 s2aff-0.21/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.21/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-12 14:58:42.770140 s2aff-0.21/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.21/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-12 14:58:42.763404 s2aff-0.21/data/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.21/data/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.21/data/combine_gold.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.21/data/download_latest_ror.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-12 14:58:42.763653 s2aff-0.21/data/ner_model/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.21/data/ner_model/__init__.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-12 14:58:42.766556 s2aff-0.21/s2aff/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8094 2023-05-08 19:46:34.000000 s2aff-0.21/s2aff/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.21/s2aff/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.21/s2aff/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.21/s2aff/features.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.21/s2aff/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-11 17:45:39.000000 s2aff-0.21/s2aff/lightgbm_helpers.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-08 19:46:34.000000 s2aff-0.21/s2aff/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    34343 2023-05-08 19:46:34.000000 s2aff-0.21/s2aff/ror.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.21/s2aff/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-12 14:58:42.767985 s2aff-0.21/s2aff/timo/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.21/s2aff/timo/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.21/s2aff/timo/integration_test.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-08 19:46:34.000000 s2aff-0.21/s2aff/timo/interface.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-12 14:58:42.767544 s2aff-0.21/s2aff.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-12 14:58:42.000000 s2aff-0.21/s2aff.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-12 14:58:42.000000 s2aff-0.21/s2aff.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-12 14:58:42.000000 s2aff-0.21/s2aff.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-12 14:58:42.000000 s2aff-0.21/s2aff.egg-info/requires.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-12 14:58:42.000000 s2aff-0.21/s2aff.egg-info/top_level.txt
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-12 14:58:42.769723 s2aff-0.21/scripts/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.21/scripts/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-08 19:46:34.000000 s2aff-0.21/scripts/approximate_runtime_and_memory_usage.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-08 19:46:34.000000 s2aff-0.21/scripts/evaluate_first_stage_ranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-08 19:46:34.000000 s2aff-0.21/scripts/generate_lightgbm_training_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.21/scripts/train_lightgbm_reranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.21/scripts/train_ner_model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.21/scripts/update_openalex_works_counts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-12 14:58:42.770322 s2aff-0.21/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-12 14:58:13.000000 s2aff-0.21/setup.py
```

### Comparing `s2aff-0.20/LICENSE` & `s2aff-0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `s2aff-0.20/README.md` & `s2aff-0.21/README.md`

 * *Files identical despite different names*

### Comparing `s2aff-0.20/data/combine_gold.py` & `s2aff-0.21/data/combine_gold.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.20/data/download_latest_ror.py` & `s2aff-0.21/data/download_latest_ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.20/s2aff/__init__.py` & `s2aff-0.21/s2aff/__init__.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.20/s2aff/consts.py` & `s2aff-0.21/s2aff/consts.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     PROJECT_ROOT_PATH = os.path.abspath(os.path.join(__file__, os.pardir, os.pardir))
 except NameError:
     PROJECT_ROOT_PATH = os.path.abspath(os.path.join(os.getcwd()))
 
 
 CACHE_ROOT = Path(os.getenv("S2AFF_CACHE", str(Path.home() / ".s2aff")))
 
-ROR_VERSION = "v1.24-2023-04-27"
+ROR_VERSION = "v1.25-2023-05-11"
 
 PATHS = {
     "ner_training_data": os.path.join(PROJECT_ROOT_PATH, "data", "ner_training_data.pickle"),
     "ror_data": os.path.join(PROJECT_ROOT_PATH, "data", f"{ROR_VERSION}-ror-data.json"),
     "country_info": os.path.join(PROJECT_ROOT_PATH, "data", "country_info.txt"),
     "openalex_works_counts": os.path.join(PROJECT_ROOT_PATH, "data", "openalex_works_counts.csv"),
     "gold_affiliation_annotations": os.path.join(PROJECT_ROOT_PATH, "data", "gold_affiliation_annotations.csv"),
```

### Comparing `s2aff-0.20/s2aff/data.py` & `s2aff-0.21/s2aff/data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.20/s2aff/features.py` & `s2aff-0.21/s2aff/features.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.20/s2aff/file_cache.py` & `s2aff-0.21/s2aff/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.20/s2aff/lightgbm_helpers.py` & `s2aff-0.21/s2aff/lightgbm_helpers.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.20/s2aff/model.py` & `s2aff-0.21/s2aff/model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.20/s2aff/ror.py` & `s2aff-0.21/s2aff/ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.20/s2aff/text.py` & `s2aff-0.21/s2aff/text.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.20/s2aff/timo/integration_test.py` & `s2aff-0.21/s2aff/timo/integration_test.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.20/s2aff/timo/interface.py` & `s2aff-0.21/s2aff/timo/interface.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.20/s2aff.egg-info/SOURCES.txt` & `s2aff-0.21/s2aff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2aff-0.20/scripts/approximate_runtime_and_memory_usage.py` & `s2aff-0.21/scripts/approximate_runtime_and_memory_usage.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.20/scripts/evaluate_first_stage_ranker.py` & `s2aff-0.21/scripts/evaluate_first_stage_ranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.20/scripts/generate_lightgbm_training_data.py` & `s2aff-0.21/scripts/generate_lightgbm_training_data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.20/scripts/train_lightgbm_reranker.py` & `s2aff-0.21/scripts/train_lightgbm_reranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.20/scripts/train_ner_model.py` & `s2aff-0.21/scripts/train_ner_model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.20/scripts/update_openalex_works_counts.py` & `s2aff-0.21/scripts/update_openalex_works_counts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.20/setup.py` & `s2aff-0.21/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from os import path
 
 requirements_file = path.join(path.dirname(__file__), "requirements.in")
 requirements = [r for r in open(requirements_file).read().split("\n") if not re.match(r"^\-", r)]
 
 setuptools.setup(
     name="s2aff",
-    version="0.20",
+    version="0.21",
     url="https://github.com/allenai/S2AFF",
     packages=setuptools.find_packages(),
     install_requires=requirements,  # dependencies specified in requirements.in
     description="Semantic Scholar's Affiliation Extraction: Link Your Raw Affiliations to ROR IDs",
 )
```


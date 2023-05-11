# Comparing `tmp/arize-7.0.1rc0.tar.gz` & `tmp/arize-7.0.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arize-7.0.1rc0.tar", last modified: Fri Apr 21 19:39:04 2023, max compression
+gzip compressed data, was "arize-7.0.2rc0.tar", last modified: Thu May  4 18:55:44 2023, max compression
```

## Comparing `arize-7.0.1rc0.tar` & `arize-7.0.2rc0.tar`

### file list

```diff
@@ -1,61 +1,63 @@
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-21 19:39:04.051568 arize-7.0.1rc0/
--rw-r--r--   0 kiko       (501) staff       (20)     1479 2023-03-30 21:17:25.000000 arize-7.0.1rc0/LICENSE.md
--rw-r--r--   0 kiko       (501) staff       (20)       65 2023-03-30 21:17:25.000000 arize-7.0.1rc0/MANIFEST.in
--rw-r--r--   0 kiko       (501) staff       (20)    12558 2023-04-21 19:39:04.052714 arize-7.0.1rc0/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)    11617 2023-03-30 21:17:25.000000 arize-7.0.1rc0/README.md
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-21 19:39:03.940431 arize-7.0.1rc0/arize/
--rw-r--r--   0 kiko       (501) staff       (20)       25 2023-04-21 19:37:33.000000 arize-7.0.1rc0/arize/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    26430 2023-04-21 06:56:16.000000 arize-7.0.1rc0/arize/api.py
--rw-r--r--   0 kiko       (501) staff       (20)     1126 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/bounded_executor.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-21 19:39:03.978476 arize-7.0.1rc0/arize/examples/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/examples/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1478 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/examples/bulk_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     1274 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/examples/bulk_client_shap.py
--rw-r--r--   0 kiko       (501) staff       (20)     1770 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/examples/client_shap_values.py
--rw-r--r--   0 kiko       (501) staff       (20)     2455 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/examples/log_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     3803 2023-04-10 03:28:13.000000 arize-7.0.1rc0/arize/examples/log_pandas_dataframe.py
--rw-r--r--   0 kiko       (501) staff       (20)     2637 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/examples/preproduction_client.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-21 19:39:03.980297 arize-7.0.1rc0/arize/pandas/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/pandas/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-21 19:39:03.999123 arize-7.0.1rc0/arize/pandas/embeddings/
--rw-r--r--   0 kiko       (501) staff       (20)      124 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/pandas/embeddings/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     2451 2023-04-18 19:34:15.000000 arize-7.0.1rc0/arize/pandas/embeddings/auto_generator.py
--rw-r--r--   0 kiko       (501) staff       (20)     6583 2023-04-18 21:41:36.000000 arize-7.0.1rc0/arize/pandas/embeddings/base_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      213 2023-04-13 06:03:38.000000 arize-7.0.1rc0/arize/pandas/embeddings/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)     1962 2023-04-10 03:28:13.000000 arize-7.0.1rc0/arize/pandas/embeddings/cv_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      571 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/pandas/embeddings/models.py
--rw-r--r--   0 kiko       (501) staff       (20)     3576 2023-04-13 06:03:38.000000 arize-7.0.1rc0/arize/pandas/embeddings/nlp_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)     5809 2023-04-10 03:28:13.000000 arize-7.0.1rc0/arize/pandas/embeddings/tabular_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      412 2023-04-13 06:03:38.000000 arize-7.0.1rc0/arize/pandas/embeddings/usecases.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-21 19:39:04.000800 arize-7.0.1rc0/arize/pandas/generative/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-13 06:03:38.000000 arize-7.0.1rc0/arize/pandas/generative/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-21 19:39:04.031073 arize-7.0.1rc0/arize/pandas/generative/llm_evaluation/
--rw-r--r--   0 kiko       (501) staff       (20)      160 2023-04-13 06:03:38.000000 arize-7.0.1rc0/arize/pandas/generative/llm_evaluation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)      183 2023-04-13 06:03:38.000000 arize-7.0.1rc0/arize/pandas/generative/llm_evaluation/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)    12188 2023-04-21 06:56:16.000000 arize-7.0.1rc0/arize/pandas/generative/llm_evaluation/hf_metrics.py
--rw-r--r--   0 kiko       (501) staff       (20)    22774 2023-04-21 19:38:35.000000 arize-7.0.1rc0/arize/pandas/logger.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-21 19:39:04.034056 arize-7.0.1rc0/arize/pandas/surrogate_explainer/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/pandas/surrogate_explainer/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     4910 2023-04-21 06:56:16.000000 arize-7.0.1rc0/arize/pandas/surrogate_explainer/mimic.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-21 19:39:04.038118 arize-7.0.1rc0/arize/pandas/validation/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/pandas/validation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    22928 2023-04-21 06:56:16.000000 arize-7.0.1rc0/arize/pandas/validation/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)    59550 2023-04-21 06:56:16.000000 arize-7.0.1rc0/arize/pandas/validation/validator.py
--rw-r--r--   0 kiko       (501) staff       (20)   169752 2023-04-19 18:46:11.000000 arize-7.0.1rc0/arize/public_pb2.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-21 19:39:04.045198 arize-7.0.1rc0/arize/utils/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/utils/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1244 2023-03-30 21:17:25.000000 arize-7.0.1rc0/arize/utils/logging.py
--rw-r--r--   0 kiko       (501) staff       (20)     4995 2023-04-19 18:46:11.000000 arize-7.0.1rc0/arize/utils/model_mapping.json
--rw-r--r--   0 kiko       (501) staff       (20)    22046 2023-04-21 06:56:16.000000 arize-7.0.1rc0/arize/utils/types.py
--rw-r--r--   0 kiko       (501) staff       (20)     7229 2023-04-21 06:56:16.000000 arize-7.0.1rc0/arize/utils/utils.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-21 19:39:03.949528 arize-7.0.1rc0/arize.egg-info/
--rw-r--r--   0 kiko       (501) staff       (20)    12558 2023-04-21 19:39:03.000000 arize-7.0.1rc0/arize.egg-info/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)     1463 2023-04-21 19:39:03.000000 arize-7.0.1rc0/arize.egg-info/SOURCES.txt
--rw-r--r--   0 kiko       (501) staff       (20)        1 2023-04-21 19:39:03.000000 arize-7.0.1rc0/arize.egg-info/dependency_links.txt
--rw-r--r--   0 kiko       (501) staff       (20)      434 2023-04-21 19:39:03.000000 arize-7.0.1rc0/arize.egg-info/requires.txt
--rw-r--r--   0 kiko       (501) staff       (20)        6 2023-04-21 19:39:03.000000 arize-7.0.1rc0/arize.egg-info/top_level.txt
--rw-r--r--   0 kiko       (501) staff       (20)      167 2023-03-30 21:17:25.000000 arize-7.0.1rc0/pyproject.toml
--rw-r--r--   0 kiko       (501) staff       (20)     1522 2023-04-21 19:39:04.055934 arize-7.0.1rc0/setup.cfg
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-04-21 19:39:04.050238 arize-7.0.1rc0/tests/
--rw-r--r--   0 kiko       (501) staff       (20)    44544 2023-04-21 06:56:16.000000 arize-7.0.1rc0/tests/test_api.py
--rw-r--r--   0 kiko       (501) staff       (20)      952 2023-03-30 21:17:25.000000 arize-7.0.1rc0/tests/test_utils.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-04 18:55:44.123271 arize-7.0.2rc0/
+-rw-r--r--   0 kiko       (501) staff       (20)     1479 2023-04-25 01:01:08.000000 arize-7.0.2rc0/LICENSE.md
+-rw-r--r--   0 kiko       (501) staff       (20)       65 2023-04-25 01:01:08.000000 arize-7.0.2rc0/MANIFEST.in
+-rw-r--r--   0 kiko       (501) staff       (20)    12558 2023-05-04 18:55:44.123592 arize-7.0.2rc0/PKG-INFO
+-rw-r--r--   0 kiko       (501) staff       (20)    11617 2023-04-25 01:01:08.000000 arize-7.0.2rc0/README.md
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-04 18:55:44.063003 arize-7.0.2rc0/arize/
+-rw-r--r--   0 kiko       (501) staff       (20)       25 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    29188 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/api.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1126 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/bounded_executor.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-04 18:55:44.079733 arize-7.0.2rc0/arize/examples/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/examples/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1478 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/examples/bulk_client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1274 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/examples/bulk_client_shap.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1770 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/examples/client_shap_values.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2455 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/examples/log_client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3803 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/examples/log_pandas_dataframe.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2637 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/examples/preproduction_client.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-04 18:55:44.081121 arize-7.0.2rc0/arize/pandas/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/pandas/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-04 18:55:44.107095 arize-7.0.2rc0/arize/pandas/embeddings/
+-rw-r--r--   0 kiko       (501) staff       (20)      124 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/pandas/embeddings/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2451 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/pandas/embeddings/auto_generator.py
+-rw-r--r--   0 kiko       (501) staff       (20)     6999 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/pandas/embeddings/base_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      213 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/pandas/embeddings/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2023 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/pandas/embeddings/cv_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      753 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/pandas/embeddings/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)      571 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/pandas/embeddings/models.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3675 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/pandas/embeddings/nlp_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5853 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/pandas/embeddings/tabular_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      412 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/pandas/embeddings/usecases.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-04 18:55:44.107927 arize-7.0.2rc0/arize/pandas/generative/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/pandas/generative/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-04 18:55:44.110660 arize-7.0.2rc0/arize/pandas/generative/llm_evaluation/
+-rw-r--r--   0 kiko       (501) staff       (20)      160 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/pandas/generative/llm_evaluation/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)      183 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/pandas/generative/llm_evaluation/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)    12178 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/pandas/generative/llm_evaluation/hf_metrics.py
+-rw-r--r--   0 kiko       (501) staff       (20)    22990 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/pandas/logger.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-04 18:55:44.112145 arize-7.0.2rc0/arize/pandas/surrogate_explainer/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/pandas/surrogate_explainer/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     4907 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/pandas/surrogate_explainer/mimic.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-04 18:55:44.114692 arize-7.0.2rc0/arize/pandas/validation/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/pandas/validation/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    25762 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/pandas/validation/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)    68436 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/pandas/validation/validator.py
+-rw-r--r--   0 kiko       (501) staff       (20)   167683 2023-05-04 02:38:51.000000 arize-7.0.2rc0/arize/public_pb2.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-04 18:55:44.119598 arize-7.0.2rc0/arize/utils/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/utils/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)      618 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/utils/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1244 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/utils/logging.py
+-rw-r--r--   0 kiko       (501) staff       (20)     4995 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/utils/model_mapping.json
+-rw-r--r--   0 kiko       (501) staff       (20)    22244 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/utils/types.py
+-rw-r--r--   0 kiko       (501) staff       (20)     7072 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/utils/utils.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-04 18:55:44.074296 arize-7.0.2rc0/arize.egg-info/
+-rw-r--r--   0 kiko       (501) staff       (20)    12558 2023-05-04 18:55:44.000000 arize-7.0.2rc0/arize.egg-info/PKG-INFO
+-rw-r--r--   0 kiko       (501) staff       (20)     1522 2023-05-04 18:55:44.000000 arize-7.0.2rc0/arize.egg-info/SOURCES.txt
+-rw-r--r--   0 kiko       (501) staff       (20)        1 2023-05-04 18:55:44.000000 arize-7.0.2rc0/arize.egg-info/dependency_links.txt
+-rw-r--r--   0 kiko       (501) staff       (20)      430 2023-05-04 18:55:44.000000 arize-7.0.2rc0/arize.egg-info/requires.txt
+-rw-r--r--   0 kiko       (501) staff       (20)        6 2023-05-04 18:55:44.000000 arize-7.0.2rc0/arize.egg-info/top_level.txt
+-rw-r--r--   0 kiko       (501) staff       (20)      167 2023-04-25 01:01:08.000000 arize-7.0.2rc0/pyproject.toml
+-rw-r--r--   0 kiko       (501) staff       (20)     1518 2023-05-04 18:55:44.125377 arize-7.0.2rc0/setup.cfg
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-04 18:55:44.121996 arize-7.0.2rc0/tests/
+-rw-r--r--   0 kiko       (501) staff       (20)    49432 2023-05-04 18:52:13.000000 arize-7.0.2rc0/tests/test_api.py
+-rw-r--r--   0 kiko       (501) staff       (20)      952 2023-04-25 01:01:08.000000 arize-7.0.2rc0/tests/test_utils.py
```

### Comparing `arize-7.0.1rc0/LICENSE.md` & `arize-7.0.2rc0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arize-7.0.1rc0/PKG-INFO` & `arize-7.0.2rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.0.1rc0
+Version: 7.0.2rc0
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arize-7.0.1rc0/README.md` & `arize-7.0.2rc0/README.md`

 * *Files identical despite different names*

### Comparing `arize-7.0.1rc0/arize/api.py` & `arize-7.0.2rc0/arize/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,22 @@
+# type: ignore[pb2]
 import concurrent.futures as cf
 import time
 from typing import Dict, Optional, Tuple, Union
 
 import numpy as np
 from arize.pandas.validation.errors import InvalidAdditionalHeaders
-from arize.utils.utils import MAX_PREDICTION_ID_LEN, MIN_PREDICTION_ID_LEN
+from arize.utils.constants import (
+    MAX_FUTURE_YEARS_FROM_CURRENT_TIME,
+    MAX_PAST_YEARS_FROM_CURRENT_TIME,
+    MAX_PREDICTION_ID_LEN,
+    MAX_TAG_LENGTH,
+    MIN_PREDICTION_ID_LEN,
+)
+from arize.utils.logging import logger
 from google.protobuf.json_format import MessageToDict
 from google.protobuf.wrappers_pb2 import DoubleValue
 from requests_futures.sessions import FuturesSession
 
 from . import public_pb2 as pb2
 from .__init__ import __version__
 from .bounded_executor import BoundedExecutor
@@ -26,14 +34,33 @@
     convert_dictionary,
     convert_element,
     get_python_version,
     get_timestamp,
     is_timestamp_in_range,
 )
 
+PredictionLabelTypes = Union[
+    str,
+    bool,
+    int,
+    float,
+    Tuple[str, float],
+    ObjectDetectionLabel,
+    RankingPredictionLabel,
+]
+ActualLabelTypes = Union[
+    str,
+    bool,
+    int,
+    float,
+    Tuple[str, float],
+    ObjectDetectionLabel,
+    RankingActualLabel,
+]
+
 
 class Client:
     """
     Arize API Client to log model predictions and actuals to the Arize AI platform
     """
 
     def __init__(
@@ -43,28 +70,32 @@
         uri: Optional[str] = "https://api.arize.com/v1",
         max_workers: Optional[int] = 8,
         max_queue_bound: Optional[int] = 5000,
         timeout: Optional[int] = 200,
         additional_headers: Optional[Dict[str, str]] = None,
     ) -> None:
         """
-        :param api_key (str): Arize provided API key associated with your account. Located on the
-        data upload page.
-        :param space_key (str): Arize provided identifier to connect records to spaces. Located on
-        the data upload page.
-        :param uri (str, optional): URI to send your records to Arize AI. Defaults to
-        "https://api.arize.com/v1".
-        :param max_workers (int, optional): maximum number of concurrent requests to Arize. Defaults
-        to 8.
-        :param max_queue_bound (int, optional): maximum number of concurrent future objects
-        generated for publishing to Arize. Defaults to 5000.
-        :param timeout (int, optional): How long to wait for the server to send data before giving
-        up. Defaults to 200.
-        :param additional_headers (Dict[str, str], optional): Dictionary of additional headers to
-        append to request
+        Initializes the Arize Client
+
+        Arguments:
+        ----------
+            api_key (str): Arize provided API key associated with your account. Located on the
+                data upload page.
+            space_key (str): Arize provided identifier to connect records to spaces. Located on
+                the data upload page.
+            uri (str, optional): URI to send your records to Arize AI. Defaults to
+                "https://api.arize.com/v1".
+            max_workers (int, optional): maximum number of concurrent requests to Arize. Defaults
+                to 8.
+            max_queue_bound (int, optional): maximum number of concurrent future objects
+                generated for publishing to Arize. Defaults to 5000.
+            timeout (int, optional): How long to wait for the server to send data before giving
+                up. Defaults to 200.
+            additional_headers (Dict[str, str], optional): Dictionary of additional headers to
+                append to request
         """
 
         if not isinstance(space_key, str):
             raise TypeError(f"space_key {space_key} is type {type(space_key)}, but must be a str")
         self._uri = f"{uri}/log"
         self._api_key = api_key
         self._space_key = space_key
@@ -87,76 +118,63 @@
         self,
         model_id: str,
         model_type: ModelTypes,
         environment: Environments,
         model_version: Optional[str] = None,
         prediction_id: Optional[Union[str, int, float]] = None,
         prediction_timestamp: Optional[int] = None,
-        prediction_label: Union[
-            str,
-            bool,
-            int,
-            float,
-            Tuple[str, float],
-            ObjectDetectionLabel,
-            RankingPredictionLabel,
-        ] = None,
-        actual_label: Union[
-            str,
-            bool,
-            int,
-            float,
-            Tuple[str, float],
-            ObjectDetectionLabel,
-            RankingActualLabel,
-        ] = None,
+        prediction_label: Optional[PredictionLabelTypes] = None,
+        actual_label: Optional[ActualLabelTypes] = None,
         features: Optional[Dict[str, Union[str, bool, float, int]]] = None,
         embedding_features: Optional[Dict[str, Embedding]] = None,
-        shap_values: Dict[str, float] = None,
+        shap_values: Optional[Dict[str, float]] = None,
         tags: Optional[Dict[str, Union[str, bool, float, int]]] = None,
         batch_id: Optional[str] = None,
     ) -> cf.Future:
         """
         Logs a record to Arize via a POST request.
 
-        :param model_id (str): A unique name to identify your model in the Arize platform.
-        :param model_type (ModelTypes): Declare your model type. Can check the supported model types
-        running `ModelTypes.list_types()`
-        :param environment (Environments): The environment that this dataframe is for (Production,
-        Training, Validation).
-        :param model_version (str, optional): Used to group together a subset of predictions
-        and actuals for a given model_id to track and compare changes. Defaults to None.
-        :param prediction_id (str, int, or float, optional): A unique string to identify a
-        prediction event. This value is used to match a prediction to delayed actuals in Arize. If
-        predictions are not provided, it will default to an empty string "" and Arize will create a
-        random prediction id on the server side.
-        :param prediction_timestamp (int, optional): Unix timestamp in seconds. If None, prediction
-        uses current timestamp. Defaults to None.
-        :param prediction_label (bool, int, float, str, Tuple(str, float), ObjectDetectionLabel or
-        RankingPredictionLabel; optional): The predicted value for a given model input. Defaults to
-        None.
-        :param actual_label (bool, int, float, str, Tuple[str, float], ObjectDetectionLabel or
-        RankingActualLabel; optional): The ground truth value for a given model input. This will be
-        be matched to the prediction with the same prediction_id as the one in this call. Defaults
-        to None.
-        :param features (Dict[str, Union[str, bool, float, int]], optional): Dictionary containing
-        human readable and debuggable model features. Defaults to None.
-        :param embedding_features (Dict[str, Embedding], optional): Dictionary containing model
-        embedding features. Keys must be strings. Values must be of Embedding type. Defaults to
-        None.
-        :param shap_values (Dict[str, float], optional): Dictionary containing human readable and
-        debuggable model features keys, along with SHAP feature importance values. Defaults to None.
-        :param tags (Dict[str, Union[str, bool, float, int]], optional): Dictionary containing human
-        readable and debuggable model tags. Defaults to None.
-        :param batch_id (str, optional): Used to distinguish different batch of data under the same
-        model_id and model_version. Required for VALIDATION environments. Defaults to None.
-
-        :return: `concurrent.futures.Future` object
+        Arguments:
+        ----------
+            model_id (str): A unique name to identify your model in the Arize platform.
+            model_type (ModelTypes): Declare your model type. Can check the supported model types
+                running `ModelTypes.list_types()`
+            environment (Environments): The environment that this dataframe is for (Production,
+                Training, Validation).
+            model_version (str, optional): Used to group together a subset of predictions
+                and actuals for a given model_id to track and compare changes. Defaults to None.
+            prediction_id (str, int, or float, optional): A unique string to identify a
+                prediction event. This value is used to match a prediction to delayed actuals in Arize. If
+                prediction id is not provided, Arize will, when possible, create a random prediction
+                id on the server side.
+            prediction_timestamp (int, optional): Unix timestamp in seconds. If None, prediction
+                uses current timestamp. Defaults to None.
+            prediction_label (bool, int, float, str, Tuple(str, float), ObjectDetectionLabel or
+                RankingPredictionLabel; optional): The predicted value for a given model input. Defaults to
+                None.
+            actual_label (bool, int, float, str, Tuple[str, float], ObjectDetectionLabel or
+                RankingActualLabel; optional): The ground truth value for a given model input. This will be
+                be matched to the prediction with the same prediction_id as the one in this call. Defaults
+                to None.
+            features (Dict[str, Union[str, bool, float, int]], optional): Dictionary containing
+                human readable and debuggable model features. Defaults to None.
+            embedding_features (Dict[str, Embedding], optional): Dictionary containing model
+                embedding features. Keys must be strings. Values must be of Embedding type. Defaults to
+                None.
+            shap_values (Dict[str, float], optional): Dictionary containing human readable and
+                debuggable model features keys, along with SHAP feature importance values. Defaults to None.
+            tags (Dict[str, Union[str, bool, float, int]], optional): Dictionary containing human
+                readable and debuggable model tags. Defaults to None.
+            batch_id (str, optional): Used to distinguish different batch of data under the same
+                model_id and model_version. Required for VALIDATION environments. Defaults to None.
+
+        Returns:
+        --------
+            `concurrent.futures.Future` object
         """
-
         # Validate model_id
         if not isinstance(model_id, str):
             raise TypeError(f"model_id {model_id} is type {type(model_id)}, but must be a str")
         # Validate model_type
         if not isinstance(model_type, ModelTypes):
             raise TypeError(
                 f"model_type {model_type} is type {type(model_type)}, but must be of "
@@ -171,21 +189,18 @@
         # Validate batch_id
         if environment == Environments.VALIDATION:
             if batch_id is None or not isinstance(batch_id, str) or len(batch_id.strip()) == 0:
                 raise ValueError(
                     "Batch ID must be a nonempty string if logging to validation environment."
                 )
 
-        # Validate prediction_id
-        if prediction_id is not None:
-            check_length = embedding_features is not None
-            _validate_prediction_id(prediction_id, check_length)
-            prediction_id = str(prediction_id)
-        else:
-            prediction_id = ""
+        # Convert & Validate prediction_id
+        prediction_id = _validate_and_convert_prediction_id(
+            prediction_id, environment, prediction_label, actual_label, shap_values
+        )
         # Validate feature types
         if features:
             for feat_name, feat_value in features.items():
                 _validate_mapping_key(feat_name)
                 val = convert_element(feat_value)
                 if val is not None and not isinstance(val, (str, bool, float, int)):
                     raise TypeError(
@@ -214,31 +229,44 @@
                 if val is not None and not isinstance(val, (str, bool, float, int)):
                     raise TypeError(
                         f"tag {tag_name} with value {tag_value} is type {type(tag_value)}, "
                         f"but expected one of: str, bool, float, int"
                     )
                 if isinstance(tag_name, str) and tag_name.endswith("_shap"):
                     raise ValueError(f"tag {tag_name} must not be named with a `_shap` suffix")
+                if len(str(val)) > MAX_TAG_LENGTH:
+                    raise ValueError(
+                        f"The number of characters for each tag must be less than or equal to "
+                        f"{MAX_TAG_LENGTH}. The tag {tag_name} with value {tag_value} has "
+                        f"{len(str(val))} characters."
+                    )
 
         # Check the timestamp present on the event
-        if prediction_timestamp is not None and not isinstance(prediction_timestamp, int):
-            raise TypeError(
-                f"prediction_timestamp {prediction_timestamp} is type "
-                f"{type(prediction_timestamp)} but expected int"
-            )
-
-        now = int(time.time())
-        if prediction_timestamp is not None and not is_timestamp_in_range(
-            now, prediction_timestamp
-        ):
-            raise ValueError(
-                f"prediction_timestamp: {prediction_timestamp} is out of range. Value must be "
-                f"within 1 year of the current time."
-            )
-
+        if prediction_timestamp is not None:
+            if not isinstance(prediction_timestamp, int):
+                raise TypeError(
+                    f"prediction_timestamp {prediction_timestamp} is type "
+                    f"{type(prediction_timestamp)} but expected int"
+                )
+            # Send warning if prediction is sent with future timestamp
+            now = int(time.time())
+            if prediction_timestamp > now:
+                logger.warning(
+                    "Caution when sending a prediction with future timestamp."
+                    "Arize only stores 2 years worth of data. For example, if you sent a prediction "
+                    "to Arize from 1.5 years ago, and now send a prediction with timestamp of a year in "
+                    "the future, the oldest 0.5 years will be dropped to maintain the 2 years worth of data "
+                    "requirement."
+                )
+            if not is_timestamp_in_range(now, prediction_timestamp):
+                raise ValueError(
+                    f"prediction_timestamp: {prediction_timestamp} is out of range."
+                    f"Prediction timestamps must be within {MAX_FUTURE_YEARS_FROM_CURRENT_TIME} year in the "
+                    f"future and {MAX_PAST_YEARS_FROM_CURRENT_TIME} years in the past from the current time."
+                )
         # Construct the prediction
         p = None
         if prediction_label is not None:
             if model_version is not None and not isinstance(model_version, str):
                 raise TypeError(
                     f"model_version {model_version} is type {type(model_version)}, but must be a "
                     f"str"
@@ -287,15 +315,15 @@
             a = pb2.Actual(
                 actual_label=_get_label(
                     prediction_or_actual="actual",
                     value=actual_label,
                     model_type=model_type,
                 )
             )
-            # Added to support latent tags on actuals.
+            # Added to support delayed tags on actuals.
             if tags is not None:
                 converted_tags = convert_dictionary(tags)
                 tgs = pb2.Actual(tags=converted_tags)
                 a.MergeFrom(tgs)
 
         # Validate and construct the optional feature importances
         fi = None
@@ -618,22 +646,51 @@
             f"feature {feat_name} must be named with string, type used: {type(feat_name)}"
         )
     if feat_name.endswith("_shap"):
         raise ValueError(f"feature {feat_name} must not be named with a `_shap` suffix")
     return
 
 
-def _validate_prediction_id(prediction_id: Union[str, int, float], validate_length: bool = False):
-    if prediction_id is not None and not isinstance(prediction_id, str):
+def _convert_prediction_id(prediction_id: Union[str, int, float]) -> str:
+    if not isinstance(prediction_id, str):
         try:
-            str(prediction_id)
+            prediction_id = str(
+                prediction_id
+            ).strip()  # strip ensures we don't receive whitespaces as part of the prediction id
         except Exception:
             raise ValueError(f"prediction_id value {prediction_id} must be convertible to a string")
 
-    if validate_length:
-        if prediction_id is None or len(str(prediction_id)) not in range(
-            MIN_PREDICTION_ID_LEN, MAX_PREDICTION_ID_LEN + 1
-        ):
+    if len(prediction_id) not in range(MIN_PREDICTION_ID_LEN, MAX_PREDICTION_ID_LEN + 1):
+        raise ValueError(
+            f"The string length of prediction_id {prediction_id} must be between {MIN_PREDICTION_ID_LEN} "
+            f"and {MAX_PREDICTION_ID_LEN}"
+        )
+    return prediction_id
+
+
+def _validate_and_convert_prediction_id(
+    prediction_id: Optional[Union[str, int, float]],
+    environment: Environments,
+    prediction_label: Optional[PredictionLabelTypes] = None,
+    actual_label: Optional[ActualLabelTypes] = None,
+    shap_values: Optional[Dict[str, float]] = None,
+) -> str:
+    # If the user does not provide prediction id
+    if prediction_id is None:
+        # delayed records have actual information but not prediction information
+        is_delayed_record = prediction_label is None and (
+            actual_label is not None or shap_values is not None
+        )
+        # Pre-production environment does not need prediction id
+        # Production environment needs prediction id for delayed record, since joins are needed
+        if is_delayed_record and environment == Environments.PRODUCTION:
             raise ValueError(
-                f"The string length of prediction_id {prediction_id} must be between {MIN_PREDICTION_ID_LEN} "
-                f"and {MAX_PREDICTION_ID_LEN}"
+                "prediction_id value cannot be None for delayed records, i.e., records ",
+                "without prediction_label and with either actual_label or shap_values",
             )
+        # Prediction ids are optional for:
+        # pre-production records and
+        # production records that are not delayed records
+        return ""
+
+    # If prediction id is given by user, convert it to string and validate length
+    return _convert_prediction_id(prediction_id)
```

### Comparing `arize-7.0.1rc0/arize/bounded_executor.py` & `arize-7.0.2rc0/arize/bounded_executor.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.1rc0/arize/examples/bulk_client.py` & `arize-7.0.2rc0/arize/examples/bulk_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.1rc0/arize/examples/bulk_client_shap.py` & `arize-7.0.2rc0/arize/examples/bulk_client_shap.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.1rc0/arize/examples/client_shap_values.py` & `arize-7.0.2rc0/arize/examples/client_shap_values.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.1rc0/arize/examples/log_client.py` & `arize-7.0.2rc0/arize/examples/log_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.1rc0/arize/examples/log_pandas_dataframe.py` & `arize-7.0.2rc0/arize/examples/log_pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.1rc0/arize/examples/preproduction_client.py` & `arize-7.0.2rc0/arize/examples/preproduction_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.1rc0/arize/pandas/embeddings/auto_generator.py` & `arize-7.0.2rc0/arize/pandas/embeddings/auto_generator.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.1rc0/arize/pandas/embeddings/base_generators.py` & `arize-7.0.2rc0/arize/pandas/embeddings/base_generators.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 from abc import ABC, abstractmethod
 from enum import Enum
-from typing import Dict, List
+from typing import Dict, List, Union
 
+import arize.pandas.embeddings.errors as err
+import pandas as pd
 from arize.utils.logging import logger
 
 from .constants import IMPORT_ERROR_MESSAGE
 from .models import CV_PRETRAINED_MODELS, NLP_PRETRAINED_MODELS
 
 try:
     import torch
@@ -87,14 +89,22 @@
             embeddings = outputs.last_hidden_state[:, 0, :]
         elif method == "avg_token":  # Select avg token vector
             embeddings = torch.mean(outputs.last_hidden_state, 1)
         else:
             raise ValueError(f"Invalid method = {method}")
         return {"embedding_vector": embeddings.cpu().numpy()}
 
+    @staticmethod
+    def check_invalid_index(field: Union[pd.Series, pd.DataFrame]) -> None:
+        if (field.index != field.reset_index(drop=True).index).any():
+            if isinstance(field, pd.DataFrame):
+                raise err.InvalidIndexError("DataFrame")
+            else:
+                raise err.InvalidIndexError(field.name)
+
     @abstractmethod
     def __repr__(self) -> str:
         pass
 
 
 class NLPEmbeddingGenerator(BaseEmbeddingGenerator):
     def __repr__(self) -> str:
```

### Comparing `arize-7.0.1rc0/arize/pandas/embeddings/cv_generators.py` & `arize-7.0.2rc0/arize/pandas/embeddings/cv_generators.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
         :param local_image_path_col: a pandas Series containing the local path to the images to
         be used to generate the embedding vectors.
         :return: a pandas Series containing the embedding vectors.
         """
         if not isinstance(local_image_path_col, pd.Series):
             raise TypeError("local_image_path_col_name must be pandas Series object")
+        self.check_invalid_index(field=local_image_path_col)
 
         # Validate that there are no null image paths
         if local_image_path_col.isnull().any():
             raise ValueError("There can't be any null values in the local_image_path_col series")
 
         ds = Dataset.from_dict({"local_path": local_image_path_col})
         ds.set_transform(
```

### Comparing `arize-7.0.1rc0/arize/pandas/embeddings/models.py` & `arize-7.0.2rc0/arize/pandas/embeddings/models.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.1rc0/arize/pandas/embeddings/nlp_generators.py` & `arize-7.0.2rc0/arize/pandas/embeddings/nlp_generators.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         :param class_label_col: if this column is passed, the sentence "The classification label
         is <class_label>" will be appended to the text in the `text_col`.
         :return: a pandas Series containing the embedding vectors.
         """
         if not isinstance(text_col, pd.Series):
             raise TypeError("text_col must be a pandas Series")
 
+        self.check_invalid_index(field=text_col)
+
         if class_label_col is not None:
             if not isinstance(class_label_col, pd.Series):
                 raise TypeError("class_label_col must be a pandas Series")
             df = pd.concat({"text": text_col, "class_label": class_label_col}, axis=1)
             prepared_text_col = df.apply(
                 lambda row: f" The classification label is {row['class_label']}. {row['text']}",
                 axis=1,
@@ -76,14 +78,15 @@
         Obtain embedding vectors from your text data using pre-trained large language models.
 
         :param text_col: a pandas Series containing the different pieces of text.
         :return: a pandas Series containing the embedding vectors.
         """
         if not isinstance(text_col, pd.Series):
             raise TypeError("text_col must be a pandas Series")
+        self.check_invalid_index(field=text_col)
 
         ds = Dataset.from_dict({"text": text_col})
 
         ds.set_transform(partial(self.tokenize, text_feat_name="text"))
         logger.info("Generating embedding vectors")
         ds = ds.map(
             lambda batch: self._get_embedding_vector(batch, "cls_token"),
```

### Comparing `arize-7.0.1rc0/arize/pandas/embeddings/tabular_generators.py` & `arize-7.0.2rc0/arize/pandas/embeddings/tabular_generators.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,14 +81,16 @@
         :param return_prompt_col: if set to True, an extra pandas Series will be returned
         containing the constructed prompts. Defaults to False.
         :return: a pandas Series containing the embedding vectors and, if `return_prompt_col` is
         set to True, a pandas Seres containing the prompts created from tabular features.
         """
         if not isinstance(df, pd.DataFrame):
             raise TypeError("df must be a pandas DataFrame")
+        self.check_invalid_index(field=df)
+
         if not is_list_of(selected_columns, str):
             raise TypeError("columns must be a list of column names (strings)")
         missing_cols = set(selected_columns).difference(df.columns)
         if missing_cols:
             raise ValueError(
                 "selected_columns list must only contain columns of the dataframe. "
                 f"The following columns are not found {missing_cols}"
```

### Comparing `arize-7.0.1rc0/arize/pandas/generative/llm_evaluation/hf_metrics.py` & `arize-7.0.2rc0/arize/pandas/generative/llm_evaluation/hf_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     them to a set of high-quality reference translations. These scores are then averaged over the entire
     corpus to obtain an estimate of the overall quality of the translation. Notably, BLEU does not consider
     factors such as intelligibility or grammatical correctness when computing the scores.
 
     NOTE: This metric is a wrapper around the Hugging Face's implementation of BLEU:
         https://github.com/huggingface/evaluate/blob/main/metrics/bleu/bleu.py
 
-    Parameters:
-    -----------
+    Arguments:
+    ----------
         response_col (pd.Series): Pandas Series containing the translations (as strings) to score.
         references_col (pd.Series): Pandas Series containing a reference, or list of several references,
             for each translation.
         max_order (int, optional):  Maximum n-gram order to use when computing BLEU score. Defaults to 4.
         smooth (bool, optional): Whether or not to apply Lin et al. 2004 smoothing. Defaults to False.
 
     Returns:
@@ -72,16 +72,16 @@
     SacreBLEU provides hassle-free computation of shareable, comparable, and reproducible BLEU scores.
     Inspired by Rico Sennrich's multi-bleu-detok.perl, it produces the official Workshop on Machine
     Translation (WMT) scores but works with plain text.
 
     NOTE: This metric is a wrapper around the Hugging Face's implementation of SacreBLEU:
         https://github.com/huggingface/evaluate/blob/main/metrics/sacrebleu/sacrebleu.py
 
-    Parameters:
-    -----------
+    Arguments:
+    ----------
         response_col (pd.Series): Pandas Series containing translations (as strings) to score.
         references_col (pd.Series): Pandas Series containing a reference, or list of several references,
             per prediction. Note that there must be the same number of references for each prediction
             (i.e. all sub-lists must be of the same length).
         smooth_method (str, optional): The smoothing method to use, defaults to 'exp'. Possible values are:
             - 'none': no smoothing
             - 'floor': increment zero counts
@@ -139,16 +139,16 @@
     The GLEU score ranges between 0 (no matches) and 1 (all matches), and it is symmetrical when we switch
     the output and target sequences. The GLEU score is highly correlated with the BLEU metric at the corpus
     level but does not have the limitations of the BLEU score for our per sentence reward objective.
 
     NOTE: This metric is a wrapper around the Hugging Face's implementation of Google BLEU:
         https://github.com/huggingface/evaluate/blob/main/metrics/google_bleu/google_bleu.py
 
-    Parameters:
-    -----------
+    Arguments:
+    ----------
         response_col (pd.Series): Pandas Series containing translations (as strings) to score.
         references_col (pd.Series): Pandas Series containing a reference, or list of several references,
             for each translation.
         min_len (int, optional): The minimum order of n-gram this function should extract. Defaults to 1.
         max_len (int, optional): The maximum order of n-gram this function should extract. Defaults to 4.
 
     Returns:
@@ -179,16 +179,16 @@
     uppercase and lowercase letters as equivalent, making the evaluation case-insensitive. By providing a
     standardized way to assess the quality of machine-generated summaries and translations, ROUGE is a useful
     tool in the field of natural language processing.
 
     NOTE: This metric is a wrapper around the Hugging Face's implementation of ROUGE:
         https://github.com/huggingface/evaluate/blob/main/metrics/rouge/rouge.py
 
-    Parameters:
-    -----------
+    Arguments:
+    ----------
         response_col (pd.Series): Pandas Series containing predictions (as strings) to score.
         references_col (pd.Series): Pandas Series containing a reference, or list of several references,
             per prediction.
         rouge_types (List[str], optional): A list of rouge types to calculate. Defaults to ['rougeL']. Valid
             rouge types:
                 - "rouge1": unigram (1-gram) based scoring
                 - "rouge2": bigram (2-gram) based scoring
@@ -237,16 +237,16 @@
     all generalized unigram matches between the two strings, METEOR calculates a score for this matching using
     a combination of unigram-precision, unigram-recall, and a measure of fragmentation, which is specifically
     designed to assess the order of the matched words in the machine translation compared to the reference.
 
     NOTE: This metric is a wrapper around the Hugging Face's implementation of METEOR:
         https://github.com/huggingface/evaluate/blob/main/metrics/meteor/meteor.py
 
-    Parameters:
-    -----------
+    Arguments:
+    ----------
         response_col (pd.Series): Pandas Series containing predictions (as strings) to score.
         references_col (pd.Series): Pandas Series containing a reference, or list of several references,
             per prediction.
         alpha (float, optional): Parameter for controlling relative weights of precision and recall.
             Default is 0.9.
         beta (float, optional): Parameter for controlling shape of penalty as a function of fragmentation.
             Default is 3.
```

### Comparing `arize-7.0.1rc0/arize/pandas/logger.py` & `arize-7.0.2rc0/arize/pandas/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,22 +34,26 @@
         self,
         api_key: str,
         space_key: str,
         uri: Optional[str] = "https://api.arize.com/v1",
         additional_headers: Optional[Dict[str, str]] = None,
     ) -> None:
         """
-        :param api_key (str): Arize provided API key associated with your account. Located on the
-        data upload page.
-        :param space_key (str): Arize provided identifier to connect records to spaces. Located on
-        the data upload page.
-        :param uri (str, optional): URI endpoint to send your records to Arize AI. Defaults to
-        "https://api.arize.com/v1".
-        :param additional_headers (Dict[str, str], optional): Dictionary of additional headers to
-        append to request
+        Initializes the Arize Client
+
+        Arguments:
+        ----------
+            api_key (str): Arize provided API key associated with your account. Located on the
+                data upload page.
+            space_key (str): Arize provided identifier to connect records to spaces. Located on
+                the data upload page.
+            uri (str, optional): URI endpoint to send your records to Arize AI. Defaults to
+                "https://api.arize.com/v1".
+            additional_headers (Dict[str, str], optional): Dictionary of additional headers to
+                append to request
         """
         self._api_key = api_key
         self._space_key = space_key
         self._files_uri = uri + "/pandas_arrow"
         self._additional_headers = {}
         if additional_headers is not None:
             reserved_headers = {
@@ -83,53 +87,52 @@
         verbose: Optional[bool] = False,
     ) -> requests.Response:
         """
         Logs a pandas dataframe containing inferences to Arize via a POST request. Returns a
         :class:`Response` object from the Requests HTTP library to ensure successful delivery of
         records.
 
-        :param dataframe (pd.DataFrame): The dataframe containing model data.
-        :param schema (Schema): A Schema instance that specifies the column names for corresponding
-        data in the dataframe.
-        :param environment (Environments): The environment the data corresponds to (Production,
-        Training, Validation).
-        :param model_id (str): A unique name to identify your model in the Arize platform.
-        :param model_type (ModelTypes): Declare your model type. Can check the supported model types
-        running `ModelTypes.list_types()`.
-        :param metrics_validation (List[Metrics], optional): A list of desired metric types;
-        defaults to None. When populated, and if validate=True, the presence of schema columns are
-        validated against the desired metrics.
-        :param model_version (str, optional): Used to group a subset of predictions and actuals for
-        a given model_id to compare and track changes. Defaults to None.
-        :param batch_id (str, optional): Used to distinguish different batch of data under the same
-        model_id and  model_version. Defaults to None.
-        :param sync (bool, optional): When sync is set to True, the log call will block, or wait,
-        until the data has been successfully ingested by the platform and immediately return the
-        status of the log. Defaults to False.
-        :param validate (bool, optional): When set to True, validation is run before sending data.
-        Defaults to True.
-        :param path (str, optional): Temporary directory/file to store the serialized data in binary
-        before sending to Arize.
-        :param surrogate_explainability (bool, optional): Computes feature importance values using
-        the surrogate explainability method. This requires that the arize module is installed with
-        the [MimicExplainer] option. If feature importance values are already specified by the
-        shap_values_column_names attribute in the Schema, this module will not run. Defaults to
-        False.
-        :param timeout (float, optional): You can stop waiting for a response after a given number
-        of seconds with the timeout parameter. Defaults to None.
-        :param verbose: (bool, optional) = When set to true, info messages are printed. Defaults to
-        False.
+        Arguments:
+        ----------
+            dataframe (pd.DataFrame): The dataframe containing model data.
+            schema (Schema): A Schema instance that specifies the column names for corresponding
+                data in the dataframe.
+            environment (Environments): The environment the data corresponds to (Production,
+                Training, Validation).
+            model_id (str): A unique name to identify your model in the Arize platform.
+            model_type (ModelTypes): Declare your model type. Can check the supported model types
+                running `ModelTypes.list_types()`.
+            metrics_validation (List[Metrics], optional): A list of desired metric types;
+                defaults to None. When populated, and if validate=True, the presence of schema columns are
+                validated against the desired metrics.
+            model_version (str, optional): Used to group a subset of predictions and actuals for
+                a given model_id to compare and track changes. Defaults to None.
+            batch_id (str, optional): Used to distinguish different batch of data under the same
+                model_id and  model_version. Defaults to None.
+            sync (bool, optional): When sync is set to True, the log call will block, or wait,
+                until the data has been successfully ingested by the platform and immediately return the
+                status of the log. Defaults to False.
+            validate (bool, optional): When set to True, validation is run before sending data.
+                Defaults to True.
+            path (str, optional): Temporary directory/file to store the serialized data in binary
+                before sending to Arize.
+            surrogate_explainability (bool, optional): Computes feature importance values using
+                the surrogate explainability method. This requires that the arize module is installed with
+                the [MimicExplainer] option. If feature importance values are already specified by the
+                shap_values_column_names attribute in the Schema, this module will not run. Defaults to
+                False.
+            timeout (float, optional): You can stop waiting for a response after a given number
+                of seconds with the timeout parameter. Defaults to None.
+            verbose: (bool, optional) = When set to true, info messages are printed. Defaults to
+                False.
+
+        Returns:
+        --------
+            `Response` object
         """
-        # Warning for when prediction_id is not provided by the user and we generate the default
-        # prediction ids
-        if schema.prediction_id_column_name is None:
-            logger.warning(
-                "Prediction ID is not specified. Arize generates UUIDs for the model's predictions "
-                "if not provided by the user, allowing referencing and joining with actuals."
-            )
         # Warning for when prediction_label is not provided and we generate default prediction
         # labels for GENERATIVE_LLM models
         if model_type == ModelTypes.GENERATIVE_LLM:
             self._generative_model_warnings(dataframe, schema)
 
         if verbose:
             logger.info("Performing required validation.")
@@ -261,14 +264,15 @@
             else:
                 schema.embedding_feature_column_names.update(prompt_response_map)
         if validate:
             if verbose:
                 logger.info("Performing values validation.")
             errors = Validator.validate_values(
                 dataframe=dataframe,
+                environment=environment,
                 schema=schema,
                 model_type=model_type,
             )
             if errors:
                 for e in errors:
                     logger.error(e)
                 raise err.ValidationFailure(errors)
@@ -367,15 +371,20 @@
             s.arrow_schema.actual_label_column_name = schema.attributions_column_name
         elif schema.actual_label_column_name is not None:
             s.arrow_schema.actual_label_column_name = schema.actual_label_column_name
 
         if model_type == ModelTypes.RANKING and schema.relevance_score_column_name is not None:
             s.arrow_schema.actual_score_column_name = schema.relevance_score_column_name
         elif schema.actual_score_column_name is not None:
-            s.arrow_schema.actual_score_column_name = schema.actual_score_column_name
+            if model_type in NUMERIC_MODEL_TYPES:
+                # allow numeric prediction to be sent in as either prediction_label (legacy) or
+                # prediction_score.
+                s.arrow_schema.actual_label_column_name = schema.actual_score_column_name
+            else:
+                s.arrow_schema.actual_score_column_name = schema.actual_score_column_name
 
         if schema.shap_values_column_names is not None:
             s.arrow_schema.shap_values_column_names.update(schema.shap_values_column_names)
 
         if schema.prediction_group_id_column_name is not None:
             s.arrow_schema.prediction_group_id_column_name = schema.prediction_group_id_column_name
```

### Comparing `arize-7.0.1rc0/arize/pandas/surrogate_explainer/mimic.py` & `arize-7.0.2rc0/arize/pandas/surrogate_explainer/mimic.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,23 +30,21 @@
             index=X.index,
         )
 
     @staticmethod
     def augment(
         df: pd.DataFrame, schema: Schema, model_type: ModelTypes
     ) -> Tuple[pd.DataFrame, Schema]:
-
         features = schema.feature_column_names
         X = df[features]
 
         if X.shape[1] == 0:
             return df, schema
 
         if model_type in CATEGORICAL_MODEL_TYPES:
-
             if not schema.prediction_score_column_name:
                 raise ValueError(
                     "To calculate surrogate explainability, "
                     f"prediction_score_column_name must be specified in schema for {model_type}."
                 )
 
             y_col_name = schema.prediction_score_column_name
@@ -61,15 +59,14 @@
                 )
 
             # model func requires 1 positional argument
             def model_func(_):
                 return np.column_stack((1 - y, y))
 
         elif model_type == ModelTypes.NUMERIC:
-
             y_col_name = schema.prediction_label_column_name
             y = df[y_col_name].to_numpy()
 
             _finite_count = np.isfinite(y).sum()
             if len(y) - _finite_count:
                 raise ValueError(
                     f"To calculate surrogate explainability for {model_type}, "
```

### Comparing `arize-7.0.1rc0/arize/pandas/validation/errors.py` & `arize-7.0.2rc0/arize/pandas/validation/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 from abc import ABC, abstractmethod
 from collections.abc import Iterable
 from typing import List
 
+from arize.utils.constants import (
+    MAX_FUTURE_YEARS_FROM_CURRENT_TIME,
+    MAX_PAST_YEARS_FROM_CURRENT_TIME,
+    MAX_TAG_LENGTH,
+)
 from arize.utils.types import Environments, Metrics, ModelTypes
 
 
 class ValidationError(Exception, ABC):
     def __str__(self) -> str:
         return self.error_message()
 
@@ -22,14 +27,27 @@
     def __init__(self, errors: List[ValidationError]) -> None:
         self.errors = errors
 
 
 # ----------------------
 # Minimum required checks
 # ----------------------
+class InvalidColumnNameEmptyString(ValidationError):
+    def __repr__(self) -> str:
+        return "Invalid_Column_Name_Empty_String"
+
+    @staticmethod
+    def error_message() -> str:
+        return (
+            "Empty column name found: ''. The schema cannot point to columns in the "
+            "dataframe denoted by an empty string. You can see the columns used in the "
+            "schema by running schema.get_used_columns()"
+        )
+
+
 class InvalidFieldTypeConversion(ValidationError):
     def __repr__(self) -> str:
         return "Invalid_Input_Type_Conversion"
 
     def __init__(self, fields: Iterable, type: str) -> None:
         self.fields = fields
         self.type = type
@@ -78,14 +96,39 @@
 
 
 # ----------------
 # Parameter checks
 # ----------------
 
 
+class MissingPredictionIdColumnForDelayedRecords(ValidationError):
+    def __repr__(self) -> str:
+        return "Missing_Prediction_Id_Column_For_Delayed_Records"
+
+    def __init__(self, has_actual_info, has_feature_importance_info) -> None:
+        self.has_actual_info = has_actual_info
+        self.has_feature_importance_info = has_feature_importance_info
+
+    def error_message(self) -> str:
+        actual = "actual" if self.has_actual_info else ""
+        feat_imp = "feature importance" if self.has_feature_importance_info else ""
+        if self.has_actual_info and self.has_feature_importance_info:
+            msg = " and ".join([actual, feat_imp])
+        else:
+            msg = "".join([actual, feat_imp])
+
+        return (
+            "Missing 'prediction_id_column_name'. While prediction id is optional for most cases, "
+            "it is required when sending delayed actuals, i.e. when sending actual or feature importances "
+            f"without predictions. In this case, {msg} information was found (without predictions)"
+            "To learn more about delayed joins, please see the docs at "
+            "https://docs.arize.com/arize/sending-data-guides/how-to-send-delayed-actuals"
+        )
+
+
 class MissingColumns(ValidationError):
     def __repr__(self) -> str:
         return "Missing_Columns"
 
     def __init__(self, cols: Iterable) -> None:
         self.missing_cols = cols
 
@@ -500,24 +543,24 @@
 # -----------
 
 
 class InvalidValueTimestamp(ValidationError):
     def __repr__(self) -> str:
         return "Invalid_Timestamp_Value"
 
-    def __init__(self, name: str, acceptable_range: str) -> None:
-        self.name = name
-        self.acceptable_range = acceptable_range
+    def __init__(self, timestamp_col_name: str) -> None:
+        self.timestamp_col_name = timestamp_col_name
 
     def error_message(self) -> str:
         return (
-            f"{self.name} is out of range. "
-            f"Predictions that are made more than {self.acceptable_range} in the future from the current "
-            "time are not accepted. If this is your pre-production data, you could also just remove the "
-            "timestamp column from the Schema."
+            f"Prediction timestamp in {self.timestamp_col_name} is out of range. "
+            f"Prediction timestamps must be within {MAX_FUTURE_YEARS_FROM_CURRENT_TIME} year "
+            f"in the future and {MAX_PAST_YEARS_FROM_CURRENT_TIME} years in the past from "
+            "the current time. If this is your pre-production data, you could also just "
+            "remove the timestamp column from the Schema."
         )
 
 
 class InvalidValueMissingValue(ValidationError):
     def __repr__(self) -> str:
         return "Invalid_Missing_Value"
 
@@ -553,15 +596,30 @@
         self.col_name = col_name
         self.min_length = min_length
         self.max_length = max_length
 
     def error_message(self) -> str:
         return (
             f"{self.schema_name} column {self.col_name} contains invalid values. "
-            f"Only string values of length within {self.min_length} - {self.max_length} are accepted."
+            f"Only string values of length between {self.min_length} and {self.max_length} are accepted."
+        )
+
+
+class InvalidTagLength(ValidationError):
+    def __repr__(self) -> str:
+        return "Invalid_Tag_Length"
+
+    def __init__(self, cols: Iterable) -> None:
+        self.wrong_value_columns = cols
+
+    def error_message(self) -> str:
+        return (
+            f"Only tag values with less than or equal to {MAX_TAG_LENGTH} characters are supported."
+            f"The following tag columns have more than {MAX_TAG_LENGTH} characters: "
+            f"{', '.join(map(str, self.wrong_value_columns))}."
         )
 
 
 class InvalidRankingCategoryValue(ValidationError):
     def __repr__(self) -> str:
         return "Invalid_Ranking_Relevance_Labels_Value"
 
@@ -693,7 +751,22 @@
         self.invalid_header_names = invalid_headers
 
     def error_message(self) -> str:
         return (
             "Found invalid additional header, cannot use reserved headers named: "
             f"{', '.join(map(str, self.invalid_header_names))}."
         )
+
+
+class InvalidRecord(ValidationError):
+    def __repr__(self) -> str:
+        return "Invalid_Record"
+
+    def __init__(self, columns: List[str], indexes: List[int]) -> None:
+        self.columns = columns
+        self.indexes = indexes
+
+    def error_message(self) -> str:
+        return (
+            f"{', '.join(self.columns)} must not all be null at row"
+            f"{', '.join(str(x) for x in self.indexes)}"
+        )
```

### Comparing `arize-7.0.1rc0/arize/pandas/validation/validator.py` & `arize-7.0.2rc0/arize/pandas/validation/validator.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,25 +2,32 @@
 from itertools import chain
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import arize.pandas.validation.errors as err
 import numpy as np
 import pandas as pd
 import pyarrow as pa
+from arize.utils.constants import (
+    MAX_FUTURE_YEARS_FROM_CURRENT_TIME,
+    MAX_PAST_YEARS_FROM_CURRENT_TIME,
+    MAX_PREDICTION_ID_LEN,
+    MAX_TAG_LENGTH,
+    MIN_PREDICTION_ID_LEN,
+    MODEL_MAPPING_CONFIG,
+)
 from arize.utils.logging import logger
 from arize.utils.types import (
     CATEGORICAL_MODEL_TYPES,
     NUMERIC_MODEL_TYPES,
     EmbeddingColumnNames,
     Environments,
     Metrics,
     ModelTypes,
     Schema,
 )
-from arize.utils.utils import MAX_PREDICTION_ID_LEN, MIN_PREDICTION_ID_LEN, MODEL_MAPPING_CONFIG
 
 
 class Validator:
     @staticmethod
     def validate_required_checks(
         dataframe: pd.DataFrame,
         model_id: str,
@@ -47,14 +54,16 @@
         schema: Schema,
         metric_families: Optional[List[Metrics]] = None,
         model_version: Optional[str] = None,
         batch_id: Optional[str] = None,
     ) -> List[err.ValidationError]:
         # general checks
         general_checks = chain(
+            Validator._check_column_names_for_empty_strings(schema),
+            Validator._check_existence_prediction_id_column_delayed_records(schema),
             Validator._check_invalid_model_id(model_id),
             Validator._check_invalid_model_version(model_version),
             Validator._check_invalid_model_type(model_type),
             Validator._check_invalid_environment(environment),
             Validator._check_invalid_batch_id(batch_id, environment),
             Validator._check_missing_columns(dataframe, schema),
             Validator._check_dataframe_for_duplicate_columns(schema, dataframe),
@@ -142,31 +151,41 @@
             return list(chain(general_checks, od_checks))
 
         return list(general_checks)
 
     @staticmethod
     def validate_values(
         dataframe: pd.DataFrame,
+        environment: Environments,
         schema: Schema,
         model_type: ModelTypes,
     ) -> List[err.ValidationError]:
         # ASSUMPTION: at this point the param and type checks should have passed.
         # This function may crash if that is not true, e.g. if columns are missing
         # or are of the wrong types.
 
         general_checks = chain(
             Validator._check_value_timestamp(dataframe, schema),
-            Validator._check_value_missing(dataframe, schema, model_type),
-            Validator._check_value_prediction_id(dataframe, schema),
+            Validator._check_invalid_missing_values(dataframe, schema, model_type),
+            Validator._check_id_field_str_length(
+                dataframe, "prediction_id_column_name", schema.prediction_id_column_name
+            ),
             Validator._check_embedding_features_dimensionality(dataframe, schema),
+            Validator._check_invalid_record_prod(dataframe, environment, schema, model_type),
+            Validator._check_invalid_record_training(dataframe, environment, schema, model_type),
+            Validator._check_value_tag(dataframe, schema),
         )
         if model_type == ModelTypes.RANKING:
             r_checks = chain(
                 Validator._check_value_rank(dataframe, schema),
-                Validator._check_value_prediction_group_id(dataframe, schema),
+                Validator._check_id_field_str_length(
+                    dataframe,
+                    "prediction_group_id_column_name",
+                    schema.prediction_group_id_column_name,
+                ),
                 Validator._check_value_ranking_category(dataframe, schema),
             )
             return list(chain(general_checks, r_checks))
         if model_type == ModelTypes.OBJECT_DETECTION:
             od_checks = chain(
                 Validator._check_value_bounding_boxes_coordinates(dataframe, schema),
                 Validator._check_value_bounding_boxes_categories(dataframe, schema),
@@ -175,14 +194,22 @@
             return list(chain(general_checks, od_checks))
         return list(general_checks)
 
     # ----------------------
     # Minimum requred checks
     # ----------------------
     @staticmethod
+    def _check_column_names_for_empty_strings(
+        schema: Schema,
+    ) -> List[err.InvalidColumnNameEmptyString]:
+        if "" in schema.get_used_columns():
+            return [err.InvalidColumnNameEmptyString()]
+        return []
+
+    @staticmethod
     def _check_field_convertible_to_str(
         model_id, model_version, batch_id
     ) -> List[err.InvalidFieldTypeConversion]:
         # converting to a set first makes the checks run a lot faster
         wrong_fields = []
         if model_id is not None and not isinstance(model_id, str):
             try:
@@ -302,15 +329,15 @@
                         metric_combinations.append([metric.upper() for metric in metrics_list])
                         if set(metrics_list) == set(
                             metric_family.name.lower() for metric_family in metric_families
                         ):
                             # This is a valid combination of model type + metrics.
                             # Now validate that required columns are in the schema.
                             is_valid_combination = True
-                            # If no prediction values are present, then latent actuals are being
+                            # If no prediction values are present, then delayed actuals are being
                             # logged, and we can't validate required columns.
                             if (schema.prediction_label_column_name is not None) or (
                                 schema.prediction_score_column_name is not None
                             ):
                                 # This is a list of lists.
                                 # In some cases, either one set of columns OR another set of
                                 # columns is required.
@@ -329,14 +356,59 @@
                                     else:
                                         break
                 if not is_valid_combination:
                     return False, [], metric_combinations
         return True, missing_columns, []
 
     @staticmethod
+    def _check_existence_prediction_id_column_delayed_records(
+        schema: Schema,
+    ) -> List[err.MissingPredictionIdColumnForDelayedRecords]:
+        if schema.prediction_id_column_name is not None:
+            return []
+        prediction_cols = (
+            schema.prediction_label_column_name,
+            schema.prediction_score_column_name,
+            schema.rank_column_name,
+            schema.prediction_group_id_column_name,
+            schema.object_detection_prediction_column_names,
+        )
+        actual_cols = (
+            schema.actual_label_column_name,
+            schema.actual_score_column_name,
+            schema.relevance_labels_column_name,
+            schema.relevance_score_column_name,
+            schema.object_detection_actual_column_names,
+        )
+        feature_importance_cols = (schema.shap_values_column_names,)
+
+        has_prediction_info = any(col is not None for col in prediction_cols)
+        has_actual_info = any(col is not None for col in actual_cols)
+        has_feature_importance_info = any(col is not None for col in feature_importance_cols)
+
+        is_delayed_record = (
+            has_actual_info or has_feature_importance_info
+        ) and not has_prediction_info
+        if is_delayed_record:
+            return [
+                err.MissingPredictionIdColumnForDelayedRecords(
+                    has_actual_info, has_feature_importance_info
+                )
+            ]
+        # Warning for when prediction_id is not provided by the user and we generate the default
+        # prediction ids
+        logger.warning(
+            "Prediction ID is not specified. Arize generates UUIDs for the model's predictions "
+            "if not provided by the user. Please note, you won't be able to send delayed data for "
+            "joining if a Prediction ID is not provided."
+        )
+
+        return []
+
+    @staticmethod
     def _check_missing_columns(
         dataframe: pd.DataFrame,
         schema: Schema,
     ) -> List[err.MissingColumns]:
         # converting to a set first makes the checks run a lot faster
         existing_columns = set(dataframe.columns)
         missing_columns = []
@@ -818,14 +890,15 @@
             allowed_datatypes = (
                 pa.float64(),
                 pa.int64(),
                 pa.float32(),
                 pa.int32(),
                 pa.int16(),
                 pa.int8(),
+                pa.null(),
             )
             for name, col in columns:
                 if (
                     col is not None
                     and col in column_types
                     and column_types[col] not in allowed_datatypes
                 ):
@@ -1080,83 +1153,96 @@
         if col is not None and col in dataframe.columns and len(dataframe):
             rank_min_max = dataframe[col].agg(["min", "max"])
             if rank_min_max["min"] < lbound or rank_min_max["max"] > ubound:
                 return [err.InvalidRankValue(col, "1-100")]
         return []
 
     @staticmethod
-    def _check_value_prediction_id(
-        dataframe: pd.DataFrame, schema: Schema
-    ) -> List[err.InvalidStringLength]:
-        """
-        Require prediction_id to be a string of length 1 - 128 if the model needs embeddings calculations.
+    def _check_id_field_str_length(
+        dataframe: pd.DataFrame, schema_name: str, id_col_name: Optional[str]
+    ) -> List[err.ValidationError]:
+        f"""
+        Require prediction_id to be a string of length between {MIN_PREDICTION_ID_LEN}
+        and {MAX_PREDICTION_ID_LEN}
         """
-        col = schema.prediction_id_column_name
-        if schema.embedding_feature_column_names is not None and not Validator._valid_char_limit(
-            col, dataframe, MIN_PREDICTION_ID_LEN, MAX_PREDICTION_ID_LEN
-        ):
-            return [
-                err.InvalidStringLength(
-                    schema_name="prediction_id_column_name",
-                    col_name=col,
-                    min_length=MIN_PREDICTION_ID_LEN,
-                    max_length=MAX_PREDICTION_ID_LEN,
-                )
-            ]
-        return []
+        # We check whether the column name can be None is allowed in `Validator.validate_params`
+        if id_col_name is None:
+            return []
 
-    @staticmethod
-    def _check_value_prediction_group_id(
-        dataframe: pd.DataFrame, schema: Schema
-    ) -> List[err.InvalidStringLength]:
-        col = schema.prediction_group_id_column_name
-        if not Validator._valid_char_limit(
-            col, dataframe, MIN_PREDICTION_ID_LEN, MAX_PREDICTION_ID_LEN
-        ):
-            return [
-                err.InvalidStringLength(
-                    schema_name="prediction_group_id_column_name",
-                    col_name=col,
-                    min_length=MIN_PREDICTION_ID_LEN,
-                    max_length=MAX_PREDICTION_ID_LEN,
-                )
-            ]
+        # _check_value_missing will return error if there are missing values in the id fields
+        # We can then proceed to check the character count of the values that are not None or missing.
+        if id_col_name in dataframe.columns:
+            if not (
+                # Check that the non-None values of the desired colum have a
+                # string length between min_len and max_len
+                # Does not check the None values
+                dataframe[~dataframe[id_col_name].isnull()][id_col_name]
+                .astype(str)
+                .str.len()
+                .between(MIN_PREDICTION_ID_LEN, MAX_PREDICTION_ID_LEN)
+                .all()
+            ):
+                return [
+                    err.InvalidStringLength(
+                        schema_name=schema_name,
+                        col_name=id_col_name,
+                        min_length=MIN_PREDICTION_ID_LEN,
+                        max_length=MAX_PREDICTION_ID_LEN,
+                    )
+                ]
         return []
 
     @staticmethod
     def _valid_char_limit(
         col_name: str, dataframe: pd.DataFrame, min_len: int, max_len: int
     ) -> bool:
         if col_name is not None and col_name in dataframe.columns and len(dataframe):
             if not (dataframe[col_name].astype(str).str.len().between(min_len, max_len).all()):
                 return False
         return True
 
     @staticmethod
+    def _check_value_tag(dataframe: pd.DataFrame, schema: Schema) -> List[err.InvalidTagLength]:
+        if schema.tag_column_names is not None and len(dataframe):
+            wrong_tag_cols = []
+            for col in schema.tag_column_names:
+                # This is to be defensive, validate_params should guarantee that this column is in
+                # the dataframe, via _check_missing_columns, and return an error before reaching this
+                # block if not
+                if col in dataframe.columns:
+                    max_tag_len = len(str(dataframe[col].agg(["max"])["max"]))
+                    if max_tag_len > MAX_TAG_LENGTH:
+                        wrong_tag_cols.append(col)
+            if wrong_tag_cols:
+                return [err.InvalidTagLength(wrong_tag_cols)]
+        return []
+
+    @staticmethod
     def _check_value_ranking_category(
         dataframe: pd.DataFrame, schema: Schema
     ) -> List[Union[err.InvalidValueMissingValue, err.InvalidRankingCategoryValue]]:
         if schema.relevance_labels_column_name is not None:
             col = schema.relevance_labels_column_name
         elif schema.attributions_column_name is not None:
             col = schema.attributions_column_name
         else:
             col = schema.actual_label_column_name
         if col is not None and col in dataframe.columns and len(dataframe):
             if dataframe[col].isnull().values.any():
                 # do not attach duplicated missing value error
-                # which would be caught by_check_value_missing
+                # which would be caught by _check_value_missing
                 return []
             if dataframe[col].astype(str).str.len().min() == 0:
                 return [err.InvalidRankingCategoryValue(col)]
             # empty list
-            if dataframe[col].map(len).min() == 0:
+            not_null_filter = dataframe[col].notnull()
+            if dataframe[not_null_filter][col].map(len).min() == 0:
                 return [err.InvalidValueMissingValue(col, "empty list")]
             # no empty string in list
-            if dataframe[col].map(lambda x: (min(map(len, x)))).min() == 0:
+            if dataframe[not_null_filter][col].map(lambda x: (min(map(len, x)))).min() == 0:
                 return [err.InvalidRankingCategoryValue(col)]
         return []
 
     @staticmethod
     def _check_value_timestamp(
         dataframe: pd.DataFrame, schema: Schema
     ) -> List[Union[err.InvalidValueMissingValue, err.InvalidValueTimestamp]]:
@@ -1169,86 +1255,199 @@
             # pandas min/max will fail due to type incompatibility. So we check for
             # missing value first.
             if dataframe[col].isnull().values.any():
                 return [err.InvalidValueMissingValue("Prediction timestamp", "missing")]
 
             now_t = datetime.datetime.now()
             lbound, ubound = (
-                (now_t - datetime.timedelta(days=730)).timestamp(),
-                (now_t + datetime.timedelta(days=365)).timestamp(),
+                (
+                    now_t - datetime.timedelta(days=MAX_PAST_YEARS_FROM_CURRENT_TIME * 365)
+                ).timestamp(),
+                (
+                    now_t + datetime.timedelta(days=MAX_FUTURE_YEARS_FROM_CURRENT_TIME * 365)
+                ).timestamp(),
             )
 
             # faster than pyarrow compute
             stats = dataframe[col].agg(["min", "max"])
 
             ta = pa.Table.from_pandas(stats.to_frame())
             type_ = ta.column(0).type
             min_, max_ = ta.column(0)
-
-            # this part needs improvement: dealing with python types is hard :(
-            # Add warning when minimum timestamp is lower than lower bound
+            # Add warning when future timestamps are sent
             if (
-                (isinstance(type_, pa.TimestampType) and (stats["min"].timestamp() < lbound))
-                or (type_ in (pa.int64(), pa.float64()) and (min_.as_py() < lbound))
+                (
+                    isinstance(type_, pa.TimestampType)
+                    and stats["max"].timestamp() > now_t.timestamp()
+                )
+                or (type_ in (pa.int64(), pa.float64()) and max_.as_py() > now_t.timestamp())
                 or (
                     type_ == pa.date32()
-                    and (int(min_.cast(pa.int32()).as_py() * 60 * 60 * 24) < lbound)
+                    and (int(max_.cast(pa.int32()).as_py() * 60 * 60 * 24) > now_t.timestamp())
+                )
+                or (
+                    type_ == pa.date64()
+                    and (int(max_.cast(pa.int64()).as_py() // 1000) > now_t.timestamp())
                 )
-                or (type_ == pa.date64() and (int(min_.cast(pa.int64()).as_py() // 1000) < lbound))
             ):
                 logger.warning(
-                    "Predictions with timestamps older than 2 years will not be shown in the Arize platform."
+                    "Caution when sending predictions with future timestamps."
+                    "Arize only stores 2 years worth of data. For example, if you sent predictions "
+                    "to Arize from 1.5 years ago, and now send predictions with timestamps of a year in "
+                    "the future, the oldest 0.5 years will be dropped to maintain the 2 years worth of data "
+                    "requirement."
                 )
 
-            # Check if max timestamp value exceeds 1 year limit
+            # this part needs improvement: dealing with python types is hard :(
+            # Return error if timestamp is out of range
             if (
-                (isinstance(type_, pa.TimestampType) and (stats["max"].timestamp() > ubound))
-                or (type_ in (pa.int64(), pa.float64()) and (max_.as_py() > ubound))
+                (
+                    isinstance(type_, pa.TimestampType)
+                    and (stats["min"].timestamp() < lbound or stats["max"].timestamp() > ubound)
+                )
+                or (
+                    type_ in (pa.int64(), pa.float64())
+                    and (min_.as_py() < lbound or max_.as_py() > ubound)
+                )
                 or (
                     type_ == pa.date32()
-                    and (int(max_.cast(pa.int32()).as_py() * 60 * 60 * 24) > ubound)
+                    and (
+                        int(min_.cast(pa.int32()).as_py() * 60 * 60 * 24) < lbound
+                        or int(max_.cast(pa.int32()).as_py() * 60 * 60 * 24) > ubound
+                    )
+                )
+                or (
+                    type_ == pa.date64()
+                    and (
+                        int(min_.cast(pa.int64()).as_py() // 1000) < lbound
+                        or int(max_.cast(pa.int64()).as_py() // 1000) > ubound
+                    )
                 )
-                or (type_ == pa.date64() and (int(max_.cast(pa.int64()).as_py() // 1000) > ubound))
             ):
-                return [
-                    err.InvalidValueTimestamp("Prediction timestamp", acceptable_range="one year")
-                ]
+                return [err.InvalidValueTimestamp(timestamp_col_name=col)]
 
         return []
 
+    # _check_invalid_missing_values validates that columns that cannot have any null values
+    # do not have any null values and returns an error if they do
     @staticmethod
-    def _check_value_missing(
+    def _check_invalid_missing_values(
         dataframe: pd.DataFrame, schema: Schema, model_type: ModelTypes
     ) -> List[err.InvalidValueMissingValue]:
         errors = []
         columns = ()
-        if model_type == ModelTypes.SCORE_CATEGORICAL:
-            columns = (("Prediction IDs", schema.prediction_id_column_name),)
-        else:
+        if model_type == ModelTypes.RANKING:
             columns = (
                 ("Prediction IDs", schema.prediction_id_column_name),
-                ("Prediction labels", schema.prediction_label_column_name),
-                ("Actual labels", schema.actual_label_column_name),
                 ("Prediction Group IDs", schema.prediction_group_id_column_name),
                 ("Ranks", schema.rank_column_name),
-                ("Attributions", schema.attributions_column_name),
-                ("Relevance Score", schema.relevance_score_column_name),
-                ("Relevance Labels", schema.relevance_labels_column_name),
             )
+        else:
+            columns = (("Prediction IDs", schema.prediction_id_column_name),)
+            # TODO: add separate logic for objective detection and generative model types
         for name, col in columns:
             if col is not None and col in dataframe.columns:
                 if dataframe[col].isnull().any():
                     errors.append(err.InvalidValueMissingValue(name, wrong_values="missing"))
                 elif (
                     dataframe[col].dtype in (np.dtype("float64"), np.dtype("float32"))
                     and np.isinf(dataframe[col]).any()
                 ):
                     errors.append(err.InvalidValueMissingValue(name, wrong_values="infinite"))
         return errors
 
+    # _check_invalid_record_prod validates there's not a single row in the dataframe
+    # with pred_label, pred_score, actual_label, actual_score, and shap_value
+    # columns all evaluates to null and returns an error with the row numbers
+    # where that is the case
+    @staticmethod
+    def _check_invalid_record_prod(
+        dataframe: pd.DataFrame, environment: Environments, schema: Schema, model_type: ModelTypes
+    ) -> List[err.InvalidRecord]:
+        if environment in (Environments.VALIDATION, Environments.TRAINING):
+            return []
+
+        if model_type in CATEGORICAL_MODEL_TYPES or model_type in NUMERIC_MODEL_TYPES:
+            columns_to_validate = [
+                schema.prediction_label_column_name,
+                schema.prediction_score_column_name,
+                schema.actual_label_column_name,
+                schema.actual_score_column_name,
+            ]
+        elif model_type == ModelTypes.RANKING:
+            columns_to_validate = [
+                schema.prediction_label_column_name,
+                schema.prediction_score_column_name,
+                schema.actual_label_column_name,
+                schema.actual_score_column_name,
+                schema.relevance_score_column_name,
+                schema.relevance_labels_column_name,
+            ]
+        else:
+            columns_to_validate = []
+            # TODO: add separate logic for objective detection and generative model types
+
+        if schema.shap_values_column_names is not None:
+            columns_to_validate.extend(list(schema.shap_values_column_names.values()))
+
+        return Validator._check_invalid_record_helper(dataframe, columns_to_validate)
+
+    # _check_invalid_record_training validates there's not a single row in the dataframe
+    # with pred_label, pred_score all evaluates to null OR with actual_label, actual_score
+    # all evaluates to null and returns errors if either of the two cases exists
+    def _check_invalid_record_training(
+        dataframe: pd.DataFrame, environment: Environments, schema: Schema, model_type: ModelTypes
+    ) -> List[err.InvalidRecord]:
+        if environment == Environments.PRODUCTION:
+            return []
+
+        if model_type in CATEGORICAL_MODEL_TYPES or model_type in NUMERIC_MODEL_TYPES:
+            pred_columns_to_validate = [
+                schema.prediction_label_column_name,
+                schema.prediction_score_column_name,
+            ]
+            actual_columns_to_validate = [
+                schema.actual_label_column_name,
+                schema.actual_score_column_name,
+            ]
+        elif model_type == ModelTypes.RANKING:
+            pred_columns_to_validate = [
+                schema.prediction_label_column_name,
+                schema.prediction_score_column_name,
+            ]
+            actual_columns_to_validate = [
+                schema.actual_label_column_name,
+                schema.actual_score_column_name,
+                schema.relevance_score_column_name,
+                schema.relevance_labels_column_name,
+            ]
+        else:
+            pred_columns_to_validate = []
+            actual_columns_to_validate = []
+            # TODO: add separate logic for objective detection and generative model types
+
+        return Validator._check_invalid_record_helper(
+            dataframe, pred_columns_to_validate
+        ) + Validator._check_invalid_record_helper(dataframe, actual_columns_to_validate)
+
+    def _check_invalid_record_helper(
+        dataframe: pd.DataFrame, column_names: List[str]
+    ) -> List[err.InvalidRecord]:
+        columns_subset = []
+        for col in column_names:
+            if col is not None and col in dataframe.columns:
+                columns_subset.append(col)
+        if len(columns_subset) == 0:
+            return []
+        null_filter = dataframe[columns_subset].isnull().all(axis=1)
+        null_index = null_filter[null_filter].index.values
+        if len(null_index) == 0:
+            return []
+        return [err.InvalidRecord(columns_subset, null_index)]
+
     @staticmethod
     def _check_type_prediction_group_id(
         schema: Schema, column_types: Dict[str, Any]
     ) -> List[err.InvalidType]:
         col = schema.prediction_group_id_column_name
         if col in column_types:
             # should mirror server side
@@ -1284,15 +1483,15 @@
         if schema.relevance_labels_column_name is not None:
             col = schema.relevance_labels_column_name
         elif schema.attributions_column_name is not None:
             col = schema.attributions_column_name
         else:
             col = schema.actual_label_column_name
         if col is not None and col in column_types:
-            allowed_datatypes = (pa.list_(pa.string()), pa.string())
+            allowed_datatypes = (pa.list_(pa.string()), pa.string(), pa.null())
             if column_types[col] not in allowed_datatypes:
                 return [
                     err.InvalidType(
                         "relevance labels column for ranking models",
                         expected_types=["list of string", "string"],
                     )
                 ]
```

### Comparing `arize-7.0.1rc0/arize/public_pb2.py` & `arize-7.0.2rc0/arize/public_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: public.proto
-"""Generated protocol buffer code."""
+
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
@@ -53,16 +53,16 @@
       name='PRODUCTION', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=4088,
-  serialized_end=4160,
+  serialized_start=3999,
+  serialized_end=4071,
 )
 _sym_db.RegisterEnumDescriptor(_FILEHEADER_ENVIRONMENT)
 
 _SCHEMA_ENVIRONMENT = _descriptor.EnumDescriptor(
   name='Environment',
   full_name='public.Schema.Environment',
   filename=None,
@@ -88,16 +88,16 @@
       name='PRODUCTION', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=8991,
-  serialized_end=9075,
+  serialized_start=8902,
+  serialized_end=8986,
 )
 _sym_db.RegisterEnumDescriptor(_SCHEMA_ENVIRONMENT)
 
 _SCHEMA_MODELTYPE = _descriptor.EnumDescriptor(
   name='ModelType',
   full_name='public.Schema.ModelType',
   filename=None,
@@ -566,47 +566,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1463,
-  serialized_end=1491,
-)
-
-_SCORECATEGORICAL_SCOREVALUE = _descriptor.Descriptor(
-  name='ScoreValue',
-  full_name='public.ScoreCategorical.ScoreValue',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='value', full_name='public.ScoreCategorical.ScoreValue.value', index=0,
-      number=1, type=1, cpp_type=5, label=1,
-      has_default_value=False, default_value=float(0),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=1493,
-  serialized_end=1520,
+  serialized_start=1403,
+  serialized_end=1431,
 )
 
 _SCORECATEGORICAL_SCORECATEGORY = _descriptor.Descriptor(
   name='ScoreCategory',
   full_name='public.ScoreCategorical.ScoreCategory',
   filename=None,
   file=DESCRIPTOR,
@@ -642,16 +611,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1522,
-  serialized_end=1600,
+  serialized_start=1433,
+  serialized_end=1511,
 )
 
 _SCORECATEGORICAL = _descriptor.Descriptor(
   name='ScoreCategorical',
   full_name='public.ScoreCategorical',
   filename=None,
   file=DESCRIPTOR,
@@ -682,40 +651,33 @@
     _descriptor.FieldDescriptor(
       name='score_category', full_name='public.ScoreCategorical.score_category', index=3,
       number=4, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='score_value', full_name='public.ScoreCategorical.score_value', index=4,
-      number=5, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[_SCORECATEGORICAL_CATEGORY, _SCORECATEGORICAL_SCOREVALUE, _SCORECATEGORICAL_SCORECATEGORY, ],
+  nested_types=[_SCORECATEGORICAL_CATEGORY, _SCORECATEGORICAL_SCORECATEGORY, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='type', full_name='public.ScoreCategorical.type',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
   serialized_start=1218,
-  serialized_end=1608,
+  serialized_end=1519,
 )
 
 
 _OBJECTDETECTION_BOUNDINGBOX = _descriptor.Descriptor(
   name='BoundingBox',
   full_name='public.ObjectDetection.BoundingBox',
   filename=None,
@@ -752,16 +714,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1691,
-  serialized_end=1788,
+  serialized_start=1602,
+  serialized_end=1699,
 )
 
 _OBJECTDETECTION = _descriptor.Descriptor(
   name='ObjectDetection',
   full_name='public.ObjectDetection',
   filename=None,
   file=DESCRIPTOR,
@@ -783,16 +745,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1611,
-  serialized_end=1788,
+  serialized_start=1522,
+  serialized_end=1699,
 )
 
 
 _RANKINGPREDICTION = _descriptor.Descriptor(
   name='RankingPrediction',
   full_name='public.RankingPrediction',
   filename=None,
@@ -836,16 +798,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1791,
-  serialized_end=1924,
+  serialized_start=1702,
+  serialized_end=1835,
 )
 
 
 _RANKINGACTUAL = _descriptor.Descriptor(
   name='RankingActual',
   full_name='public.RankingActual',
   filename=None,
@@ -875,16 +837,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1926,
-  serialized_end=2034,
+  serialized_start=1837,
+  serialized_end=1945,
 )
 
 
 _LABEL = _descriptor.Descriptor(
   name='Label',
   full_name='public.Label',
   filename=None,
@@ -933,16 +895,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='data', full_name='public.Label.data',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=2037,
-  serialized_end=2167,
+  serialized_start=1948,
+  serialized_end=2078,
 )
 
 
 _PREDICTIONLABEL = _descriptor.Descriptor(
   name='PredictionLabel',
   full_name='public.PredictionLabel',
   filename=None,
@@ -1005,16 +967,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='data', full_name='public.PredictionLabel.data',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=2170,
-  serialized_end=2409,
+  serialized_start=2081,
+  serialized_end=2320,
 )
 
 
 _ACTUALLABEL = _descriptor.Descriptor(
   name='ActualLabel',
   full_name='public.ActualLabel',
   filename=None,
@@ -1077,16 +1039,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='data', full_name='public.ActualLabel.data',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=2412,
-  serialized_end=2643,
+  serialized_start=2323,
+  serialized_end=2554,
 )
 
 
 _PREDICTION_FEATURESENTRY = _descriptor.Descriptor(
   name='FeaturesEntry',
   full_name='public.Prediction.FeaturesEntry',
   filename=None,
@@ -1116,16 +1078,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2911,
-  serialized_end=2973,
+  serialized_start=2822,
+  serialized_end=2884,
 )
 
 _PREDICTION_TAGSENTRY = _descriptor.Descriptor(
   name='TagsEntry',
   full_name='public.Prediction.TagsEntry',
   filename=None,
   file=DESCRIPTOR,
@@ -1154,16 +1116,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2975,
-  serialized_end=3033,
+  serialized_start=2886,
+  serialized_end=2944,
 )
 
 _PREDICTION = _descriptor.Descriptor(
   name='Prediction',
   full_name='public.Prediction',
   filename=None,
   file=DESCRIPTOR,
@@ -1220,16 +1182,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2646,
-  serialized_end=3033,
+  serialized_start=2557,
+  serialized_end=2944,
 )
 
 
 _VALUE = _descriptor.Descriptor(
   name='Value',
   full_name='public.Value',
   filename=None,
@@ -1285,16 +1247,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='data', full_name='public.Value.data',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=3036,
-  serialized_end=3185,
+  serialized_start=2947,
+  serialized_end=3096,
 )
 
 
 _MULTIVALUE = _descriptor.Descriptor(
   name='MultiValue',
   full_name='public.MultiValue',
   filename=None,
@@ -1317,16 +1279,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3187,
-  serialized_end=3215,
+  serialized_start=3098,
+  serialized_end=3126,
 )
 
 
 _EMBEDDING_RAWDATA = _descriptor.Descriptor(
   name='RawData',
   full_name='public.Embedding.RawData',
   filename=None,
@@ -1354,16 +1316,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='type', full_name='public.Embedding.RawData.type',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=3344,
-  serialized_end=3419,
+  serialized_start=3255,
+  serialized_end=3330,
 )
 
 _EMBEDDING_TOKENARRAY = _descriptor.Descriptor(
   name='TokenArray',
   full_name='public.Embedding.TokenArray',
   filename=None,
   file=DESCRIPTOR,
@@ -1385,16 +1347,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3421,
-  serialized_end=3449,
+  serialized_start=3332,
+  serialized_end=3360,
 )
 
 _EMBEDDING = _descriptor.Descriptor(
   name='Embedding',
   full_name='public.Embedding',
   filename=None,
   file=DESCRIPTOR,
@@ -1430,16 +1392,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3218,
-  serialized_end=3455,
+  serialized_start=3129,
+  serialized_end=3366,
 )
 
 
 _ACTUAL_TAGSENTRY = _descriptor.Descriptor(
   name='TagsEntry',
   full_name='public.Actual.TagsEntry',
   filename=None,
@@ -1469,16 +1431,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2975,
-  serialized_end=3033,
+  serialized_start=2886,
+  serialized_end=2944,
 )
 
 _ACTUAL = _descriptor.Descriptor(
   name='Actual',
   full_name='public.Actual',
   filename=None,
   file=DESCRIPTOR,
@@ -1521,16 +1483,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3458,
-  serialized_end=3690,
+  serialized_start=3369,
+  serialized_end=3601,
 )
 
 
 _FEATUREIMPORTANCES_FEATUREIMPORTANCESENTRY = _descriptor.Descriptor(
   name='FeatureImportancesEntry',
   full_name='public.FeatureImportances.FeatureImportancesEntry',
   filename=None,
@@ -1560,16 +1522,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3866,
-  serialized_end=3923,
+  serialized_start=3777,
+  serialized_end=3834,
 )
 
 _FEATUREIMPORTANCES = _descriptor.Descriptor(
   name='FeatureImportances',
   full_name='public.FeatureImportances',
   filename=None,
   file=DESCRIPTOR,
@@ -1605,16 +1567,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3693,
-  serialized_end=3923,
+  serialized_start=3604,
+  serialized_end=3834,
 )
 
 
 _PREDICTIONANDACTUAL = _descriptor.Descriptor(
   name='PredictionAndActual',
   full_name='public.PredictionAndActual',
   filename=None,
@@ -1644,16 +1606,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3925,
-  serialized_end=4018,
+  serialized_start=3836,
+  serialized_end=3929,
 )
 
 
 _FILEHEADER = _descriptor.Descriptor(
   name='FileHeader',
   full_name='public.FileHeader',
   filename=None,
@@ -1677,16 +1639,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4021,
-  serialized_end=4160,
+  serialized_start=3932,
+  serialized_end=4071,
 )
 
 
 _SCHEMA_CONSTANTS = _descriptor.Descriptor(
   name='Constants',
   full_name='public.Schema.Constants',
   filename=None,
@@ -1737,16 +1699,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4609,
-  serialized_end=4774,
+  serialized_start=4520,
+  serialized_end=4685,
 )
 
 _SCHEMA_ARIZECONCLUSIONS = _descriptor.Descriptor(
   name='ArizeConclusions',
   full_name='public.Schema.ArizeConclusions',
   filename=None,
   file=DESCRIPTOR,
@@ -1761,16 +1723,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4776,
-  serialized_end=4794,
+  serialized_start=4687,
+  serialized_end=4705,
 )
 
 _SCHEMA_ARIZEEXPLANATIONS = _descriptor.Descriptor(
   name='ArizeExplanations',
   full_name='public.Schema.ArizeExplanations',
   filename=None,
   file=DESCRIPTOR,
@@ -1785,16 +1747,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4796,
-  serialized_end=4815,
+  serialized_start=4707,
+  serialized_end=4726,
 )
 
 _SCHEMA_ARIZECONCLUSIONPOINTERS = _descriptor.Descriptor(
   name='ArizeConclusionPointers',
   full_name='public.Schema.ArizeConclusionPointers',
   filename=None,
   file=DESCRIPTOR,
@@ -1809,16 +1771,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4817,
-  serialized_end=4842,
+  serialized_start=4728,
+  serialized_end=4753,
 )
 
 _SCHEMA_ARIZEEXPLANATIONPOINTERS = _descriptor.Descriptor(
   name='ArizeExplanationPointers',
   full_name='public.Schema.ArizeExplanationPointers',
   filename=None,
   file=DESCRIPTOR,
@@ -1833,16 +1795,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4844,
-  serialized_end=4870,
+  serialized_start=4755,
+  serialized_end=4781,
 )
 
 _SCHEMA_ARROWSCHEMA_SHAPVALUESCOLUMNNAMESENTRY = _descriptor.Descriptor(
   name='ShapValuesColumnNamesEntry',
   full_name='public.Schema.ArrowSchema.ShapValuesColumnNamesEntry',
   filename=None,
   file=DESCRIPTOR,
@@ -1871,16 +1833,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5856,
-  serialized_end=5916,
+  serialized_start=5767,
+  serialized_end=5827,
 )
 
 _SCHEMA_ARROWSCHEMA_EMBEDDINGFEATURECOLUMNNAMESMAPENTRY = _descriptor.Descriptor(
   name='EmbeddingFeatureColumnNamesMapEntry',
   full_name='public.Schema.ArrowSchema.EmbeddingFeatureColumnNamesMapEntry',
   filename=None,
   file=DESCRIPTOR,
@@ -1909,16 +1871,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5918,
-  serialized_end=6024,
+  serialized_start=5829,
+  serialized_end=5935,
 )
 
 _SCHEMA_ARROWSCHEMA = _descriptor.Descriptor(
   name='ArrowSchema',
   full_name='public.Schema.ArrowSchema',
   filename=None,
   file=DESCRIPTOR,
@@ -2066,16 +2028,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4873,
-  serialized_end=6024,
+  serialized_start=4784,
+  serialized_end=5935,
 )
 
 _SCHEMA_OBJECTDETECTIONLABELCOLUMNNAMES = _descriptor.Descriptor(
   name='ObjectDetectionLabelColumnNames',
   full_name='public.Schema.ObjectDetectionLabelColumnNames',
   filename=None,
   file=DESCRIPTOR,
@@ -2111,16 +2073,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6027,
-  serialized_end=6174,
+  serialized_start=5938,
+  serialized_end=6085,
 )
 
 _SCHEMA_EMBEDDINGCOLUMNNAMES = _descriptor.Descriptor(
   name='EmbeddingColumnNames',
   full_name='public.Schema.EmbeddingColumnNames',
   filename=None,
   file=DESCRIPTOR,
@@ -2156,16 +2118,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6176,
-  serialized_end=6286,
+  serialized_start=6087,
+  serialized_end=6197,
 )
 
 _SCHEMA_GENERICSCHEMA_FIELDDESCRIPTOR = _descriptor.Descriptor(
   name='FieldDescriptor',
   full_name='public.Schema.GenericSchema.FieldDescriptor',
   filename=None,
   file=DESCRIPTOR,
@@ -2187,16 +2149,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7916,
-  serialized_end=7953,
+  serialized_start=7827,
+  serialized_end=7864,
 )
 
 _SCHEMA_GENERICSCHEMA_GROUPFIELDDESCRIPTOR = _descriptor.Descriptor(
   name='GroupFieldDescriptor',
   full_name='public.Schema.GenericSchema.GroupFieldDescriptor',
   filename=None,
   file=DESCRIPTOR,
@@ -2225,16 +2187,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7955,
-  serialized_end=8020,
+  serialized_start=7866,
+  serialized_end=7931,
 )
 
 _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_EMBEDDINGPROPERTYMAP_PROPERTIESMAPENTRY = _descriptor.Descriptor(
   name='PropertiesMapEntry',
   full_name='public.Schema.GenericSchema.EmbeddingFieldDescriptor.EmbeddingPropertyMap.PropertiesMapEntry',
   filename=None,
   file=DESCRIPTOR,
@@ -2263,16 +2225,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8286,
-  serialized_end=8338,
+  serialized_start=8197,
+  serialized_end=8249,
 )
 
 _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_EMBEDDINGPROPERTYMAP = _descriptor.Descriptor(
   name='EmbeddingPropertyMap',
   full_name='public.Schema.GenericSchema.EmbeddingFieldDescriptor.EmbeddingPropertyMap',
   filename=None,
   file=DESCRIPTOR,
@@ -2294,16 +2256,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8143,
-  serialized_end=8338,
+  serialized_start=8054,
+  serialized_end=8249,
 )
 
 _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR_PROPERTIESENTRY = _descriptor.Descriptor(
   name='PropertiesEntry',
   full_name='public.Schema.GenericSchema.EmbeddingFieldDescriptor.PropertiesEntry',
   filename=None,
   file=DESCRIPTOR,
@@ -2332,16 +2294,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8340,
-  serialized_end=8465,
+  serialized_start=8251,
+  serialized_end=8376,
 )
 
 _SCHEMA_GENERICSCHEMA_EMBEDDINGFIELDDESCRIPTOR = _descriptor.Descriptor(
   name='EmbeddingFieldDescriptor',
   full_name='public.Schema.GenericSchema.EmbeddingFieldDescriptor',
   filename=None,
   file=DESCRIPTOR,
@@ -2363,16 +2325,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8023,
-  serialized_end=8465,
+  serialized_start=7934,
+  serialized_end=8376,
 )
 
 _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_OBJECTDETECTIONLABELPROPERTYMAP_PROPERTIESMAPENTRY = _descriptor.Descriptor(
   name='PropertiesMapEntry',
   full_name='public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor.ObjectDetectionLabelPropertyMap.PropertiesMapEntry',
   filename=None,
   file=DESCRIPTOR,
@@ -2401,16 +2363,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8286,
-  serialized_end=8338,
+  serialized_start=8197,
+  serialized_end=8249,
 )
 
 _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_OBJECTDETECTIONLABELPROPERTYMAP = _descriptor.Descriptor(
   name='ObjectDetectionLabelPropertyMap',
   full_name='public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor.ObjectDetectionLabelPropertyMap',
   filename=None,
   file=DESCRIPTOR,
@@ -2432,16 +2394,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8610,
-  serialized_end=8839,
+  serialized_start=8521,
+  serialized_end=8750,
 )
 
 _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR_PROPERTIESENTRY = _descriptor.Descriptor(
   name='PropertiesEntry',
   full_name='public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor.PropertiesEntry',
   filename=None,
   file=DESCRIPTOR,
@@ -2470,16 +2432,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8842,
-  serialized_end=8989,
+  serialized_start=8753,
+  serialized_end=8900,
 )
 
 _SCHEMA_GENERICSCHEMA_OBJECTDETECTIONLABELFIELDDESCRIPTOR = _descriptor.Descriptor(
   name='ObjectDetectionLabelFieldDescriptor',
   full_name='public.Schema.GenericSchema.ObjectDetectionLabelFieldDescriptor',
   filename=None,
   file=DESCRIPTOR,
@@ -2501,16 +2463,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8468,
-  serialized_end=8989,
+  serialized_start=8379,
+  serialized_end=8900,
 )
 
 _SCHEMA_GENERICSCHEMA = _descriptor.Descriptor(
   name='GenericSchema',
   full_name='public.Schema.GenericSchema',
   filename=None,
   file=DESCRIPTOR,
@@ -2679,16 +2641,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6289,
-  serialized_end=8989,
+  serialized_start=6200,
+  serialized_end=8900,
 )
 
 _SCHEMA = _descriptor.Descriptor(
   name='Schema',
   full_name='public.Schema',
   filename=None,
   file=DESCRIPTOR,
@@ -2876,28 +2838,23 @@
 _PREPRODUCTIONRECORD.oneofs_by_name['record_type'].fields.append(
   _PREPRODUCTIONRECORD.fields_by_name['training_record'])
 _PREPRODUCTIONRECORD.fields_by_name['training_record'].containing_oneof = _PREPRODUCTIONRECORD.oneofs_by_name['record_type']
 _PREPRODUCTIONRECORD.oneofs_by_name['record_type'].fields.append(
   _PREPRODUCTIONRECORD.fields_by_name['validation_record'])
 _PREPRODUCTIONRECORD.fields_by_name['validation_record'].containing_oneof = _PREPRODUCTIONRECORD.oneofs_by_name['record_type']
 _SCORECATEGORICAL_CATEGORY.containing_type = _SCORECATEGORICAL
-_SCORECATEGORICAL_SCOREVALUE.containing_type = _SCORECATEGORICAL
 _SCORECATEGORICAL_SCORECATEGORY.containing_type = _SCORECATEGORICAL
 _SCORECATEGORICAL.fields_by_name['category'].message_type = _SCORECATEGORICAL_CATEGORY
 _SCORECATEGORICAL.fields_by_name['score_category'].message_type = _SCORECATEGORICAL_SCORECATEGORY
-_SCORECATEGORICAL.fields_by_name['score_value'].message_type = _SCORECATEGORICAL_SCOREVALUE
 _SCORECATEGORICAL.oneofs_by_name['type'].fields.append(
   _SCORECATEGORICAL.fields_by_name['category'])
 _SCORECATEGORICAL.fields_by_name['category'].containing_oneof = _SCORECATEGORICAL.oneofs_by_name['type']
 _SCORECATEGORICAL.oneofs_by_name['type'].fields.append(
   _SCORECATEGORICAL.fields_by_name['score_category'])
 _SCORECATEGORICAL.fields_by_name['score_category'].containing_oneof = _SCORECATEGORICAL.oneofs_by_name['type']
-_SCORECATEGORICAL.oneofs_by_name['type'].fields.append(
-  _SCORECATEGORICAL.fields_by_name['score_value'])
-_SCORECATEGORICAL.fields_by_name['score_value'].containing_oneof = _SCORECATEGORICAL.oneofs_by_name['type']
 _OBJECTDETECTION_BOUNDINGBOX.fields_by_name['score'].message_type = google_dot_protobuf_dot_wrappers__pb2._DOUBLEVALUE
 _OBJECTDETECTION_BOUNDINGBOX.containing_type = _OBJECTDETECTION
 _OBJECTDETECTION.fields_by_name['bounding_boxes'].message_type = _OBJECTDETECTION_BOUNDINGBOX
 _RANKINGPREDICTION.fields_by_name['prediction_score'].message_type = google_dot_protobuf_dot_wrappers__pb2._DOUBLEVALUE
 _RANKINGACTUAL.fields_by_name['category'].message_type = _MULTIVALUE
 _RANKINGACTUAL.fields_by_name['relevance_score'].message_type = google_dot_protobuf_dot_wrappers__pb2._DOUBLEVALUE
 _LABEL.fields_by_name['score_categorical'].message_type = _SCORECATEGORICAL
@@ -3183,34 +3140,26 @@
   'Category' : _reflection.GeneratedProtocolMessageType('Category', (_message.Message,), {
     'DESCRIPTOR' : _SCORECATEGORICAL_CATEGORY,
     '__module__' : 'public_pb2'
     # @@protoc_insertion_point(class_scope:public.ScoreCategorical.Category)
     })
   ,
 
-  'ScoreValue' : _reflection.GeneratedProtocolMessageType('ScoreValue', (_message.Message,), {
-    'DESCRIPTOR' : _SCORECATEGORICAL_SCOREVALUE,
-    '__module__' : 'public_pb2'
-    # @@protoc_insertion_point(class_scope:public.ScoreCategorical.ScoreValue)
-    })
-  ,
-
   'ScoreCategory' : _reflection.GeneratedProtocolMessageType('ScoreCategory', (_message.Message,), {
     'DESCRIPTOR' : _SCORECATEGORICAL_SCORECATEGORY,
     '__module__' : 'public_pb2'
     # @@protoc_insertion_point(class_scope:public.ScoreCategorical.ScoreCategory)
     })
   ,
   'DESCRIPTOR' : _SCORECATEGORICAL,
   '__module__' : 'public_pb2'
   # @@protoc_insertion_point(class_scope:public.ScoreCategorical)
   })
 _sym_db.RegisterMessage(ScoreCategorical)
 _sym_db.RegisterMessage(ScoreCategorical.Category)
-_sym_db.RegisterMessage(ScoreCategorical.ScoreValue)
 _sym_db.RegisterMessage(ScoreCategorical.ScoreCategory)
 
 ObjectDetection = _reflection.GeneratedProtocolMessageType('ObjectDetection', (_message.Message,), {
 
   'BoundingBox' : _reflection.GeneratedProtocolMessageType('BoundingBox', (_message.Message,), {
     'DESCRIPTOR' : _OBJECTDETECTION_BOUNDINGBOX,
     '__module__' : 'public_pb2'
```

### Comparing `arize-7.0.1rc0/arize/utils/logging.py` & `arize-7.0.2rc0/arize/utils/logging.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.1rc0/arize/utils/model_mapping.json` & `arize-7.0.2rc0/arize/utils/model_mapping.json`

 * *Files identical despite different names*

### Comparing `arize-7.0.1rc0/arize/utils/types.py` & `arize-7.0.2rc0/arize/utils/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dataclasses import asdict, dataclass, replace
 from enum import Enum, unique
 from typing import Dict, List, NamedTuple, Optional, Sequence, Set, TypeVar, Union
 
 import numpy as np
 import pandas as pd
+from arize.utils.constants import MAX_PREDICTION_ID_LEN, MIN_PREDICTION_ID_LEN
 
 
 @unique
 class ModelTypes(Enum):
     NUMERIC = 1
     SCORE_CATEGORICAL = 2
     RANKING = 3
@@ -91,16 +92,16 @@
     link_to_data: Optional[str] = None
 
     def validate(self, emb_name: Union[str, int, float]) -> None:
         """
         Validates that the embedding object passed is of the correct format. That is, validations must
         be passed for vector, data & link_to_data.
 
-        Parameters:
-        -----------
+        Arguments:
+        ----------
             emb_name (str, int, float): Name of the embedding feature the vector belongs to
 
         Raises:
         -------
             TypeError: If the embedding fields are of the wrong type
         """
 
@@ -123,16 +124,16 @@
     ) -> None:
         """
         Validates that the embedding vector passed is of the correct format. That is:
             1. Type must be list or convertible to list (like numpy arrays, pandas Series)
             2. List must not be empty
             3. Elements in list must be floats
 
-        Parameters:
-        -----------
+        Arguments:
+        ----------
             emb_name (str, int, float): Name of the embedding feature the vector belongs to
 
         Raises:
         -------
             TypeError: If the embedding does not satisfy requirements above
         """
 
@@ -157,16 +158,16 @@
         self,
         emb_name: Union[str, int, float],
     ) -> None:
         """
         Validates that the embedding raw data field is of the correct format. That is:
             1. Must be string or list of strings (NLP case)
 
-        Parameters:
-        -----------
+        Arguments:
+        ----------
             emb_name (str, int, float): Name of the embedding feature the vector belongs to
 
         Raises:
         -------
             TypeError: If the embedding does not satisfy requirements above
         """
         # Validate that data is a string or iterable of strings
@@ -184,16 +185,16 @@
                 raise TypeError("Embedding data field must contain strings")
 
     def _validate_embedding_link_to_data(self, emb_name: Union[str, int, float]) -> None:
         """
         Validates that the embedding link to data field is of the correct format. That is:
             1. Must be string
 
-        Parameters:
-        -----------
+        Arguments:
+        ----------
             emb_name (str, int, float): Name of the embedding feature the vector belongs to
 
         Raises:
         -------
             TypeError: If the embedding does not satisfy requirements above
         """
         if not isinstance(self.link_to_data, str):
@@ -206,16 +207,16 @@
     def _is_valid_iterable(data: Union[str, List[str], List[float], np.ndarray, pd.Series]) -> bool:
         """
         Validates that the input data field is of the correct iterable type. That is:
             1. List or
             2. numpy array or
             3. pandas Series
 
-        Parameters:
-        -----------
+        Arguments:
+        ----------
             data: input iterable
 
         Returns:
         --------
             True if the data type is one of the accepted iterable types, false otherwise
         """
         return any(isinstance(data, t) for t in (list, np.ndarray, pd.Series))
@@ -406,56 +407,57 @@
     attributions_column_name: Optional[str] = None
     relevance_score_column_name: Optional[str] = None
     relevance_labels_column_name: Optional[str] = None
     object_detection_prediction_column_names: Optional[ObjectDetectionColumnNames] = None
     object_detection_actual_column_names: Optional[ObjectDetectionColumnNames] = None
     prompt_column_names: Optional[EmbeddingColumnNames] = None
     response_column_names: Optional[EmbeddingColumnNames] = None
-    """
+    f"""
     Used to organize and map column names containing model data within your Pandas dataframe to
     Arize.
 
-    Parameters:
-    -----------
+    Arguments:
+    ----------
         prediction_id_column_name (str, optional): Column name for the predictions unique identifier.
-            This value is used to match a prediction to delayed actuals in Arize. If predictions are
-            not provided, it will default to an empty string "" and Arize will create a random
-            prediction id on the server side. Contents must be a string and indicate a unique
-            prediction event. Limited to 128 characters.
+            Unique IDs are used to match a prediction to delayed actuals or feature importances in Arize.
+            If prediction ids are not provided, it will default to an empty string "" and, when possible,
+            Arize will create a random prediction id on the server side. Contents must be a string and
+            indicate a unique prediction event. Must contain a minimum of {MIN_PREDICTION_ID_LEN} and a
+            maximum of {MAX_PREDICTION_ID_LEN} characters.
         feature_column_names (List[str], optional): List of column names for features. The content
             of this column can be int, float, string.
         tag_column_names (List[str], optional): List of column names for tags. The content of this
             column can be int, float, string.
         timestamp_column_name (str, optional): Column name for timestamps. The content of this
             column must be int Unix Timestamps in seconds.
         prediction_label_column_name (str, optional): Column name for categorical prediction values.
             The content of this column must be convertible to string.
         prediction_score_column_name (str, optional): Column name for numeric prediction values. The
             content of this column must be int/float.
         actual_label_column_name (str, optional): Column name for categorical ground truth values.
             The content of this column must be convertible to string.
         actual_score_column_name (str, optional): Column name for numeric ground truth values. The
             content of this column must be int/float.
-        shap_values_column_names (Dict[str, str], optional): Dictionary mapping human readable and
-            debuggable model features keys and SHAP feature importance values. Keys must be str,
-            while values must be float.
+        shap_values_column_names (Dict[str, str], optional): Dictionary mapping feature column name
+            and corresponding SHAP feature importance column name. e.g.
+            {{"feat_A": "feat_A_shap", "feat_B": "feat_B_shap"}}
         embedding_feature_column_names (Dict[str, EmbeddingColumnNames], optional): Dictionary
             mapping embedding display names to EmbeddingColumnNames objects.
         prediction_group_id_column_name (str, optional): Column name for ranking groups or lists in
             ranking models. The content of this column must be string and is limited to 128 characters.
         rank_column_name (str, optional): Column name for rank of each element on the its group or
             list. The content of this column must be integer between 1-100.
         relevance_score_column_name (str, optional): Column name for ranking model type numeric
             ground truth values. The content of this column must be int/float.
         relevance_labels_column_name (str, optional): Column name for ranking model type categorical
             ground truth values. The content of this column must be a string.
-        object_detection_prediction_column_name (ObjectDetectionColumnNames, optional):
+        object_detection_prediction_column_names (ObjectDetectionColumnNames, optional):
             ObjectDetectionColumnNames object containing information defining the predicted bounding
             boxes' coordinates, categories, and scores.
-        object_detection_prediction_column_name (ObjectDetectionColumnNames, optional):
+        object_detection_actual_column_names (ObjectDetectionColumnNames, optional):
             ObjectDetectionColumnNames object containing information defining the actual bounding
             boxes' coordinates, categories, and scores.
         prompt_column_names (EmbeddingCoulumnNames, optional): EmbeddingCoulumnNames object containing
             the embedding vector data (required) and raw text (optional) for the input text your
             model acts on.
         response_column_names (EmbeddingCoulumnNames, optional): EmbeddingCoulumnNames object
             containing the embedding vector data (required) and raw text (optional) for the text
```

### Comparing `arize-7.0.1rc0/arize/utils/utils.py` & `arize-7.0.2rc0/arize/utils/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 # type: ignore[pb2]
 import base64
 import json
 import math
 import sys
-from pathlib import Path
 from typing import Any, Optional, Union
 
 import pandas as pd
+from arize.utils.constants import (
+    MAX_FUTURE_YEARS_FROM_CURRENT_TIME,
+    MAX_PAST_YEARS_FROM_CURRENT_TIME,
+)
 from google.protobuf.timestamp_pb2 import Timestamp
 from google.protobuf.wrappers_pb2 import StringValue
 
 from .. import public_pb2 as pb2
+from .constants import MAX_BYTES_PER_BULK_RECORD
 from .types import Embedding, Schema
 
-MAX_BYTES_PER_BULK_RECORD = 100000
-MAX_DAYS_WITHIN_RANGE = 365
-MIN_PREDICTION_ID_LEN = 1
-MAX_PREDICTION_ID_LEN = 128
-MODEL_MAPPING_CONFIG = None
-
-path = Path(__file__).with_name("model_mapping.json")
-with path.open("r") as f:
-    MODEL_MAPPING_CONFIG = json.load(f)
-
 
 def num_chunks(records):
     total_bytes = sum(r.ByteSize() for r in records)
     num_of_bulk = math.ceil(total_bytes / MAX_BYTES_PER_BULK_RECORD)
     return math.ceil(len(records) / num_of_bulk)
 
 
@@ -134,21 +128,17 @@
         )
     ts = Timestamp()
     ts.FromSeconds(time)
     return ts
 
 
 def is_timestamp_in_range(now: int, ts: int):
-    max_time = now + (MAX_DAYS_WITHIN_RANGE * 24 * 60 * 60)
-    min_time = now - (MAX_DAYS_WITHIN_RANGE * 24 * 60 * 60)
-    if ts > max_time:
-        return False
-    if ts < min_time:
-        return False
-    return True
+    max_time = now + (MAX_FUTURE_YEARS_FROM_CURRENT_TIME * 365 * 24 * 60 * 60)
+    min_time = now - (MAX_PAST_YEARS_FROM_CURRENT_TIME * 365 * 24 * 60 * 60)
+    return min_time <= ts <= max_time
 
 
 def reconstruct_url(response: Any):
     returnedUrl = json.loads(response.content.decode())["realTimeIngestionUri"]
     parts = returnedUrl.split("/")
     encodedOrg = base64.b64encode(f"AccountOrganization:{parts[4]}".encode()).decode()
     encodedSpace = base64.b64encode(f"Space:{parts[6]}".encode()).decode()
@@ -163,16 +153,16 @@
     return f"{sys.version_info.major}.{sys.version_info.minor}.{sys.version_info.micro}"
 
 
 def overwrite_schema_fields(schema1: Schema, schema2: Schema) -> Schema:
     """This function overwrites a base Schema `schema1` with the fields of `schema2`
     that are not None
 
-    Parameters:
-    -----------
+    Arguments:
+    ----------
         schema1 (Schema): Base Schema with fields to be overwritten
         schema2 (Schema): New Schema used to overwrite schema1
 
     Returns:
     --------
         Schema: The resulting schema
     """
```

### Comparing `arize-7.0.1rc0/arize.egg-info/PKG-INFO` & `arize-7.0.2rc0/arize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.0.1rc0
+Version: 7.0.2rc0
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arize-7.0.1rc0/arize.egg-info/SOURCES.txt` & `arize-7.0.2rc0/arize.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -22,27 +22,29 @@
 arize/pandas/__init__.py
 arize/pandas/logger.py
 arize/pandas/embeddings/__init__.py
 arize/pandas/embeddings/auto_generator.py
 arize/pandas/embeddings/base_generators.py
 arize/pandas/embeddings/constants.py
 arize/pandas/embeddings/cv_generators.py
+arize/pandas/embeddings/errors.py
 arize/pandas/embeddings/models.py
 arize/pandas/embeddings/nlp_generators.py
 arize/pandas/embeddings/tabular_generators.py
 arize/pandas/embeddings/usecases.py
 arize/pandas/generative/__init__.py
 arize/pandas/generative/llm_evaluation/__init__.py
 arize/pandas/generative/llm_evaluation/constants.py
 arize/pandas/generative/llm_evaluation/hf_metrics.py
 arize/pandas/surrogate_explainer/__init__.py
 arize/pandas/surrogate_explainer/mimic.py
 arize/pandas/validation/__init__.py
 arize/pandas/validation/errors.py
 arize/pandas/validation/validator.py
 arize/utils/__init__.py
+arize/utils/constants.py
 arize/utils/logging.py
 arize/utils/model_mapping.json
 arize/utils/types.py
 arize/utils/utils.py
 tests/test_api.py
 tests/test_utils.py
```

### Comparing `arize-7.0.1rc0/setup.cfg` & `arize-7.0.2rc0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 [options.extras_require]
 MimicExplainer = 
 	numpy<1.24.0
 	scikit-learn>=0.12.0,<2
 	interpret>=0.2.7,<1
 	interpret-community>=0.22.0,<1
-	lightgbm>=2.2.3,<3.3.4
+	lightgbm>=2.2.3,<4
 AutoEmbeddings = 
 	transformers>=4.25, <5
 	tokenizers>=0.13, <1
 	datasets>=2.8, <3
 	torch>=1.13, <3
 	Pillow>=8.4.0, <10
 LLM_Evaluation =
```

### Comparing `arize-7.0.1rc0/tests/test_api.py` & `arize-7.0.2rc0/tests/test_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,23 @@
+import time
 from pathlib import Path
 
 import arize.public_pb2 as pb2
 import numpy as np
 import pandas as pd
 import pytest
 from arize.api import Client, Embedding
 from arize.pandas.validation.errors import InvalidAdditionalHeaders
+from arize.utils.constants import (
+    MAX_FUTURE_YEARS_FROM_CURRENT_TIME,
+    MAX_PAST_YEARS_FROM_CURRENT_TIME,
+    MAX_PREDICTION_ID_LEN,
+    MAX_TAG_LENGTH,
+    MIN_PREDICTION_ID_LEN,
+)
 from arize.utils.types import (
     Environments,
     ModelTypes,
     ObjectDetectionLabel,
     RankingActualLabel,
     RankingPredictionLabel,
 )
@@ -28,17 +36,14 @@
     "model_version": "v1.2.3.4",
     "model_type_numeric": ModelTypes.NUMERIC,
     "model_type_score_categorical": ModelTypes.SCORE_CATEGORICAL,
     "model_type_regression": ModelTypes.REGRESSION,
     "model_type_binary_classification": ModelTypes.BINARY_CLASSIFICATION,
     "model_type_object_detection": ModelTypes.OBJECT_DETECTION,
     "model_type_ranking": ModelTypes.RANKING,
-    "environment_training": Environments.TRAINING,
-    "environment_validation": Environments.VALIDATION,
-    "environment_production": Environments.PRODUCTION,
     "batch_id": "batch_id",
     "batch": "batch1234",
     "api_key": "API_KEY",
     "prediction_id": "prediction_0",
     "label_bool": BOOL_VAL,
     "label_str": STR_VAL,
     "label_int": INT_VAL,
@@ -353,26 +358,26 @@
 
 
 def test_build_pred_and_actual_label_bool():
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
-        environment=inputs["environment_production"],
+        environment=Environments.PRODUCTION,
         model_type=inputs["model_type_score_categorical"],
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_bool"],
         actual_label=inputs["label_bool"],
         features=inputs["features"],
         embedding_features=inputs["embedding_features"],
         tags=inputs["tags"],
     )
 
     #   Get environment in proto format
-    ep = _get_proto_environment_params(inputs["environment_production"])
+    ep = _get_proto_environment_params(Environments.PRODUCTION)
     #   Start constructing expected result by building the prediction
     p = _build_basic_prediction("score_categorical_bool")
     a = _build_basic_actual("score_categorical_bool")
     #   Add props to prediction according to this test
     p.MergeFrom(_attach_features_to_prediction())
     p.MergeFrom(_attach_embedding_features_to_prediction())
     p.MergeFrom(_attach_tags_to_prediction())
@@ -385,26 +390,26 @@
 
 
 def test_build_pred_and_actual_label_str():
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
-        environment=inputs["environment_production"],
+        environment=Environments.PRODUCTION,
         model_type=inputs["model_type_score_categorical"],
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_str"],
         actual_label=inputs["label_str"],
         features=inputs["features"],
         embedding_features=inputs["embedding_features"],
         tags=inputs["tags"],
     )
 
     #   Get environment in proto format
-    ep = _get_proto_environment_params(inputs["environment_production"])
+    ep = _get_proto_environment_params(Environments.PRODUCTION)
     #   Start constructing expected result by building the prediction
     p = _build_basic_prediction("score_categorical_str")
     a = _build_basic_actual("score_categorical_str")
     #   Add props to prediction according to this test
     p.MergeFrom(_attach_features_to_prediction())
     p.MergeFrom(_attach_embedding_features_to_prediction())
     p.MergeFrom(_attach_tags_to_prediction())
@@ -417,39 +422,39 @@
 
 
 def test_build_pred_and_actual_label_int():
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
-        environment=inputs["environment_production"],
+        environment=Environments.PRODUCTION,
         model_type=inputs["model_type_numeric"],
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_int"],
         actual_label=inputs["label_int"],
         features=inputs["features"],
         embedding_features=inputs["embedding_features"],
         tags=inputs["tags"],
     )
 
     record_new_model_type = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
-        environment=inputs["environment_production"],
+        environment=Environments.PRODUCTION,
         model_type=inputs["model_type_regression"],
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_int"],
         actual_label=inputs["label_int"],
         features=inputs["features"],
         embedding_features=inputs["embedding_features"],
         tags=inputs["tags"],
     )
 
     #   Get environment in proto format
-    ep = _get_proto_environment_params(inputs["environment_production"])
+    ep = _get_proto_environment_params(Environments.PRODUCTION)
     #   Start constructing expected result by building the prediction
     p = _build_basic_prediction("numeric_int")
     a = _build_basic_actual("numeric_int")
     #   Add props to prediction according to this test
     p.MergeFrom(_attach_features_to_prediction())
     p.MergeFrom(_attach_embedding_features_to_prediction())
     p.MergeFrom(_attach_tags_to_prediction())
@@ -462,39 +467,39 @@
 
 
 def test_build_pred_and_actual_label_float():
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
-        environment=inputs["environment_production"],
+        environment=Environments.PRODUCTION,
         model_type=inputs["model_type_numeric"],
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_float"],
         actual_label=inputs["label_float"],
         features=inputs["features"],
         embedding_features=inputs["embedding_features"],
         tags=inputs["tags"],
     )
 
     record_new_model_type = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
-        environment=inputs["environment_production"],
+        environment=Environments.PRODUCTION,
         model_type=inputs["model_type_regression"],
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_float"],
         actual_label=inputs["label_float"],
         features=inputs["features"],
         embedding_features=inputs["embedding_features"],
         tags=inputs["tags"],
     )
 
     #   Get environment in proto format
-    ep = _get_proto_environment_params(inputs["environment_production"])
+    ep = _get_proto_environment_params(Environments.PRODUCTION)
     #   Start constructing expected result by building the prediction
     p = _build_basic_prediction("numeric_float")
     a = _build_basic_actual("numeric_float")
     #   Add props to prediction according to this test
     p.MergeFrom(_attach_features_to_prediction())
     p.MergeFrom(_attach_embedding_features_to_prediction())
     p.MergeFrom(_attach_tags_to_prediction())
@@ -507,39 +512,39 @@
 
 
 def test_build_pred_and_actual_label_tuple():
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
-        environment=inputs["environment_production"],
+        environment=Environments.PRODUCTION,
         model_type=inputs["model_type_score_categorical"],
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_tuple"],
         actual_label=inputs["label_tuple"],
         features=inputs["features"],
         embedding_features=inputs["embedding_features"],
         tags=inputs["tags"],
     )
 
     record_new_model_type = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
-        environment=inputs["environment_production"],
+        environment=Environments.PRODUCTION,
         model_type=inputs["model_type_binary_classification"],
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_tuple"],
         actual_label=inputs["label_tuple"],
         features=inputs["features"],
         embedding_features=inputs["embedding_features"],
         tags=inputs["tags"],
     )
 
     #   Get environment in proto format
-    ep = _get_proto_environment_params(inputs["environment_production"])
+    ep = _get_proto_environment_params(Environments.PRODUCTION)
     #   Start constructing expected result by building the prediction
     p = _build_basic_prediction("score_categorical_tuple")
     a = _build_basic_actual("score_categorical_tuple")
     #   Add props to prediction according to this test
     p.MergeFrom(_attach_features_to_prediction())
     p.MergeFrom(_attach_embedding_features_to_prediction())
     p.MergeFrom(_attach_tags_to_prediction())
@@ -562,39 +567,75 @@
         relevance_labels=inputs["ranking_relevance_labels"],
         relevance_score=inputs["ranking_relevance_score"],
     )
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
-        environment=inputs["environment_production"],
+        environment=Environments.PRODUCTION,
         model_type=inputs["model_type_ranking"],
         prediction_id=inputs["prediction_id"],
         prediction_label=pred_label,
         actual_label=act_label,
         features=inputs["features"],
         tags=inputs["tags"],
     )
 
     #   Get environment in proto format
-    ep = _get_proto_environment_params(inputs["environment_production"])
+    ep = _get_proto_environment_params(Environments.PRODUCTION)
     #   Start constructing expected result by building the prediction
     p = _build_basic_prediction("ranking")
     a = _build_basic_actual("ranking")
     #   Add props to prediction according to this test
     p.MergeFrom(_attach_features_to_prediction())
     p.MergeFrom(_attach_tags_to_prediction())
     #   Add props to prediction according to this test
     a.MergeFrom(_attach_tags_to_actual())
     #   Build expected record using built prediction
     expected_record = _build_expected_record(p=p, a=a, ep=ep)
     #   Check result is as expected
     assert record == expected_record
 
 
+def test_build_wrong_timestamp():
+    c = get_stubbed_client()
+    wrong_min_time = int(time.time()) - (MAX_PAST_YEARS_FROM_CURRENT_TIME * 365 * 24 * 60 * 60 + 1)
+    wrong_max_time = int(time.time()) + (
+        MAX_FUTURE_YEARS_FROM_CURRENT_TIME * 365 * 24 * 60 * 60 + 1
+    )
+
+    with pytest.raises(ValueError) as excinfo:
+        _ = c.log(
+            model_id=inputs["model_id"],
+            model_version=inputs["model_version"],
+            environment=Environments.PRODUCTION,
+            prediction_timestamp=wrong_min_time,
+            model_type=inputs["model_type_numeric"],
+            prediction_id=inputs["prediction_id"],
+            prediction_label=inputs["label_float"],
+            features=inputs["features"],
+            tags=inputs["tags"],
+        )
+    assert f"prediction_timestamp: {wrong_min_time} is out of range." in str(excinfo.value)
+
+    with pytest.raises(ValueError) as excinfo:
+        _ = c.log(
+            model_id=inputs["model_id"],
+            model_version=inputs["model_version"],
+            environment=Environments.PRODUCTION,
+            prediction_timestamp=wrong_max_time,
+            model_type=inputs["model_type_numeric"],
+            prediction_id=inputs["prediction_id"],
+            prediction_label=inputs["label_float"],
+            features=inputs["features"],
+            tags=inputs["tags"],
+        )
+    assert f"prediction_timestamp: {wrong_max_time} is out of range." in str(excinfo.value)
+
+
 def test_ranking_label_missing_group_id_rank():
     with pytest.raises(TypeError) as excinfo:
         _ = RankingPredictionLabel(
             group_id=inputs["ranking_group_id"],
             score=inputs["ranking_prediction_score"],
             label=inputs["ranking_label"],
         )
@@ -622,26 +663,26 @@
         relevance_score=inputs["ranking_relevance_score"],
     )
 
     with pytest.raises(ValueError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
-            environment=inputs["environment_production"],
+            environment=Environments.PRODUCTION,
             model_type=inputs["model_type_ranking"],
             prediction_id=inputs["prediction_id"],
             prediction_label=pred_label,
             actual_label=act_label,
             features=inputs["features"],
             tags=inputs["tags"],
         )
     assert "Rank must be between 1 and 100, inclusive. Found 101" in str(excinfo.value)
 
 
-def test_build_wrong_ranking_group_id():
+def test_ranking_group_id():
     c = get_stubbed_client()
     pred_label = RankingPredictionLabel(
         group_id=1,
         rank=inputs["ranking_rank"],
         score=inputs["ranking_prediction_score"],
         label=inputs["ranking_label"],
     )
@@ -650,15 +691,15 @@
         relevance_score=inputs["ranking_relevance_score"],
     )
 
     with pytest.raises(TypeError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
-            environment=inputs["environment_production"],
+            environment=Environments.PRODUCTION,
             model_type=inputs["model_type_ranking"],
             prediction_id=inputs["prediction_id"],
             prediction_label=pred_label,
             actual_label=act_label,
             features=inputs["features"],
             tags=inputs["tags"],
         )
@@ -671,15 +712,15 @@
         label=inputs["ranking_label"],
     )
 
     with pytest.raises(ValueError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
-            environment=inputs["environment_production"],
+            environment=Environments.PRODUCTION,
             model_type=inputs["model_type_ranking"],
             prediction_id=inputs["prediction_id"],
             prediction_label=pred_label,
             actual_label=act_label,
             features=inputs["features"],
             tags=inputs["tags"],
         )
@@ -698,15 +739,15 @@
         relevance_labels=["click", ""], relevance_score=inputs["ranking_relevance_score"]
     )
 
     with pytest.raises(ValueError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
-            environment=inputs["environment_production"],
+            environment=Environments.PRODUCTION,
             model_type=inputs["model_type_ranking"],
             prediction_id=inputs["prediction_id"],
             prediction_label=pred_label,
             actual_label=act_label,
             features=inputs["features"],
             tags=inputs["tags"],
         )
@@ -725,15 +766,15 @@
         relevance_labels=inputs["ranking_relevance_labels"], relevance_score="click"
     )
 
     with pytest.raises(TypeError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
-            environment=inputs["environment_production"],
+            environment=Environments.PRODUCTION,
             model_type=inputs["model_type_ranking"],
             prediction_id=inputs["prediction_id"],
             prediction_label=pred_label,
             actual_label=act_label,
             features=inputs["features"],
             tags=inputs["tags"],
         )
@@ -750,26 +791,26 @@
         bounding_boxes_coordinates=inputs["object_detection_bounding_boxes"],
         categories=inputs["object_detection_categories"],
     )
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
-        environment=inputs["environment_production"],
+        environment=Environments.PRODUCTION,
         model_type=inputs["model_type_object_detection"],
         prediction_id=inputs["prediction_id"],
         prediction_label=pred_label,
         actual_label=act_label,
         features=inputs["features"],
         embedding_features=inputs["object_detection_embedding_feature"],
         tags=inputs["tags"],
     )
 
     #   Get environment in proto format
-    ep = _get_proto_environment_params(inputs["environment_production"])
+    ep = _get_proto_environment_params(Environments.PRODUCTION)
     #   Start constructing expected result by building the prediction
     p = _build_basic_prediction("object_detection")
     a = _build_basic_actual("object_detection")
     #   Add props to prediction according to this test
     p.MergeFrom(_attach_features_to_prediction())
     p.MergeFrom(_attach_image_embedding_feature_to_prediction())
     p.MergeFrom(_attach_tags_to_prediction())
@@ -782,24 +823,24 @@
 
 
 def test_build_prediction_no_embedding_features():
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
-        environment=inputs["environment_production"],
+        environment=Environments.PRODUCTION,
         model_type=inputs["model_type_numeric"],
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_float"],
         features=inputs["features"],
         tags=inputs["tags"],
     )
 
     #   Get environment in proto format
-    ep = _get_proto_environment_params(inputs["environment_production"])
+    ep = _get_proto_environment_params(Environments.PRODUCTION)
     #   Start constructing expected result by building the prediction
     p = _build_basic_prediction("numeric_float")
     #   Add props to prediction according to this test
     p.MergeFrom(_attach_features_to_prediction())
     p.MergeFrom(_attach_tags_to_prediction())
     #   Build expected record using built prediction
     expected_record = _build_expected_record(p=p, ep=ep)
@@ -809,24 +850,24 @@
 
 # Structured features refer to any feature that is not an embedding
 def test_build_prediction_no_structured_features():
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
-        environment=inputs["environment_production"],
+        environment=Environments.PRODUCTION,
         model_type=inputs["model_type_numeric"],
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_float"],
         embedding_features=inputs["embedding_features"],
         tags=inputs["tags"],
     )
 
     #   Get environment in proto format
-    ep = _get_proto_environment_params(inputs["environment_production"])
+    ep = _get_proto_environment_params(Environments.PRODUCTION)
     #   Start constructing expected result by building the prediction
     p = _build_basic_prediction("numeric_float")
     #   Add props to prediction according to this test
     p.MergeFrom(_attach_embedding_features_to_prediction())
     p.MergeFrom(_attach_tags_to_prediction())
     #   Build expected record using built prediction
     expected_record = _build_expected_record(p=p, ep=ep)
@@ -835,23 +876,23 @@
 
 
 def test_build_prediction_no_features():
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
-        environment=inputs["environment_production"],
+        environment=Environments.PRODUCTION,
         model_type=inputs["model_type_numeric"],
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_float"],
         tags=inputs["tags"],
     )
 
     #   Get environment in proto format
-    ep = _get_proto_environment_params(inputs["environment_production"])
+    ep = _get_proto_environment_params(Environments.PRODUCTION)
     #   Start constructing expected result by building the prediction
     p = _build_basic_prediction("numeric_float")
     #   Add props to prediction according to this test
     p.MergeFrom(_attach_tags_to_prediction())
     #   Build expected record using built prediction
     expected_record = _build_expected_record(p=p, ep=ep)
     #   Check result is as expected
@@ -859,24 +900,24 @@
 
 
 def test_build_prediction_no_tags():
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
-        environment=inputs["environment_production"],
+        environment=Environments.PRODUCTION,
         model_type=inputs["model_type_numeric"],
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_float"],
         features=inputs["features"],
         embedding_features=inputs["embedding_features"],
     )
 
     #   Get environment in proto format
-    ep = _get_proto_environment_params(inputs["environment_production"])
+    ep = _get_proto_environment_params(Environments.PRODUCTION)
     #   Start constructing expected result by building the prediction
     p = _build_basic_prediction("numeric_float")
     #   Add props to prediction according to this test
     p.MergeFrom(_attach_features_to_prediction())
     p.MergeFrom(_attach_embedding_features_to_prediction())
     #   Build expected record using built prediction
     expected_record = _build_expected_record(p=p, ep=ep)
@@ -885,59 +926,59 @@
 
 
 def test_build_prediction_no_tags_no_features():
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
         model_version=inputs["model_version"],
-        environment=inputs["environment_production"],
+        environment=Environments.PRODUCTION,
         model_type=inputs["model_type_numeric"],
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_float"],
     )
 
     #   Get environment in proto format
-    ep = _get_proto_environment_params(inputs["environment_production"])
+    ep = _get_proto_environment_params(Environments.PRODUCTION)
     #   Start constructing expected result by building the prediction
     p = _build_basic_prediction("numeric_float")
     #   Build expected record using built prediction
     expected_record = _build_expected_record(p=p, ep=ep)
     #   Check result is as expected
     assert record == expected_record
 
 
 def test_missing_model_type():
     c = get_stubbed_client()
     with pytest.raises(TypeError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
-            environment=inputs["environment_production"],
+            environment=Environments.PRODUCTION,
             prediction_id=inputs["prediction_id"],
             prediction_label=inputs["label_str"],
             actual_label=inputs["label_str"],
             features=inputs["features"],
             embedding_features=inputs["embedding_features"],
             tags=inputs["tags"],
         )
     assert "log() missing 1 required positional argument: 'model_type'" in str(excinfo.value)
 
 
 def test_model_version_optional():
     c = get_stubbed_client()
     record = c.log(
         model_id=inputs["model_id"],
-        environment=inputs["environment_production"],
+        environment=Environments.PRODUCTION,
         model_type=inputs["model_type_numeric"],
         prediction_id=inputs["prediction_id"],
         prediction_label=inputs["label_float"],
     )
 
     #   Get environment in proto format
-    ep = _get_proto_environment_params(inputs["environment_production"])
+    ep = _get_proto_environment_params(Environments.PRODUCTION)
     #   Start constructing expected result by building the prediction
     p = _build_basic_prediction("numeric_float")
     p.model_version = ""
     #   Build expected record using built prediction
     expected_record = _build_expected_record(p=p, ep=ep)
     #   Check result is as expected
     assert record == expected_record
@@ -969,15 +1010,15 @@
         categories=inputs["object_detection_categories"],
         scores=inputs["object_detection_scores"],
     )
     with pytest.raises(ValueError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
-            environment=inputs["environment_production"],
+            environment=Environments.PRODUCTION,
             model_type=inputs["model_type_object_detection"],
             prediction_id=inputs["prediction_id"],
             prediction_label=pred_label,
             features=inputs["features"],
             embedding_features=inputs["object_detection_embedding_feature"],
             tags=inputs["tags"],
         )
@@ -995,15 +1036,15 @@
         categories=inputs["object_detection_categories"],
         scores=inputs["object_detection_scores"],
     )
     with pytest.raises(ValueError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
-            environment=inputs["environment_production"],
+            environment=Environments.PRODUCTION,
             model_type=inputs["model_type_object_detection"],
             prediction_id=inputs["prediction_id"],
             prediction_label=pred_label,
             features=inputs["features"],
             embedding_features=inputs["object_detection_embedding_feature"],
             tags=inputs["tags"],
         )
@@ -1014,15 +1055,15 @@
         categories=inputs["object_detection_categories"],
         scores=inputs["object_detection_scores"],
     )
     with pytest.raises(ValueError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
-            environment=inputs["environment_production"],
+            environment=Environments.PRODUCTION,
             model_type=inputs["model_type_object_detection"],
             prediction_id=inputs["prediction_id"],
             prediction_label=pred_label,
             features=inputs["features"],
             embedding_features=inputs["object_detection_embedding_feature"],
             tags=inputs["tags"],
         )
@@ -1036,59 +1077,126 @@
 
     # test case - too long prediction_id
     with pytest.raises(ValueError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_type=inputs["model_type_binary_classification"],
             model_version=inputs["model_version"],
-            environment=inputs["environment_production"],
+            environment=Environments.PRODUCTION,
             prediction_id="A" * 129,
             prediction_label=inputs["label_str"],
             actual_label=inputs["label_str"],
             features=inputs["features"],
             embedding_features=inputs["embedding_features"],
             tags=inputs["tags"],
         )
     assert "The string length of prediction_id" in str(excinfo.value)
 
 
-def test_no_prediction_id():
+def test_prediction_id():
     c = get_stubbed_client()
 
-    # test case - None prediction_id
-    try:
-        _ = c.log(
-            model_id=inputs["model_id"],
-            model_type=inputs["model_type_binary_classification"],
-            model_version=inputs["model_version"],
-            environment=inputs["environment_production"],
-            prediction_id=None,
-            prediction_label=inputs["label_str"],
-            actual_label=inputs["label_str"],
-            features=inputs["features"],
-            embedding_features=inputs["embedding_features"],
-            tags=inputs["tags"],
-        )
-    except Exception as e:
-        assert False, f"Logging data without prediction_id raised an exception {e}"
+    correct_cases = [
+        {
+            # test case - None prediction_id, Training
+            "prediction_id": None,
+            "environment": Environments.TRAINING,
+            "prediction_label": inputs["label_str"],
+        },
+        {
+            # test case - None prediction_id, Production, not a delayed record
+            "prediction_id": None,
+            "environment": Environments.PRODUCTION,
+            "prediction_label": inputs["label_str"],
+        },
+    ]
+    for case in correct_cases:
+        try:
+            _ = c.log(
+                model_id=inputs["model_id"],
+                model_type=inputs["model_type_binary_classification"],
+                model_version=inputs["model_version"],
+                environment=case["environment"],
+                prediction_id=case["prediction_id"],
+                prediction_label=case["prediction_label"],
+                actual_label=inputs["label_str"],
+                features=inputs["features"],
+                embedding_features=inputs["embedding_features"],
+                tags=inputs["tags"],
+            )
+        except Exception as e:
+            msg = (
+                f"Logging data without prediction_id raised an exception {e}. "
+                + f"prediction_id={case['prediction_id']}, environment={case['environment']}, "
+                + f"prediction_label={case['prediction_label']}."
+            )
+            assert False, msg
+
+    short_prediction_id = "x" * (MIN_PREDICTION_ID_LEN - 1)
+    long_prediction_id = "x" * (MAX_PREDICTION_ID_LEN + 1)
+    incorrect_cases = [
+        {
+            # test case - None prediction_id, Production, delayed record
+            "prediction_id": None,
+            "environment": Environments.PRODUCTION,
+            "prediction_label": None,
+            "err_msg": "prediction_id value cannot be None for delayed records",
+        },
+        {
+            # test case - Wrong length prediction_id, Training
+            "prediction_id": short_prediction_id,
+            "environment": Environments.TRAINING,
+            "prediction_label": inputs["label_str"],
+            "err_msg": f"The string length of prediction_id {short_prediction_id} must be between",
+        },
+        {
+            # test case - Wrong length prediction_id, Production, delayed record
+            "prediction_id": short_prediction_id,
+            "environment": Environments.PRODUCTION,
+            "prediction_label": None,
+            "err_msg": f"The string length of prediction_id {short_prediction_id} must be between",
+        },
+        {
+            # test case - Wrong length prediction_id, Production, not a delayed record
+            "prediction_id": long_prediction_id,
+            "environment": Environments.PRODUCTION,
+            "prediction_label": inputs["label_str"],
+            "err_msg": f"The string length of prediction_id {long_prediction_id} must be between",
+        },
+    ]
+    for case in incorrect_cases:
+        with pytest.raises(ValueError) as exc_info:
+            _ = c.log(
+                model_id=inputs["model_id"],
+                model_type=inputs["model_type_binary_classification"],
+                model_version=inputs["model_version"],
+                environment=case["environment"],
+                prediction_id=case["prediction_id"],
+                prediction_label=case["prediction_label"],
+                actual_label=inputs["label_str"],
+                features=inputs["features"],
+                embedding_features=inputs["embedding_features"],
+                tags=inputs["tags"],
+            )
+        assert case["err_msg"] in str(exc_info.value)
 
 
 def test_object_detection_wrong_categories():
     c = get_stubbed_client()
 
     pred_label = ObjectDetectionLabel(
         bounding_boxes_coordinates=inputs["object_detection_bounding_boxes"],
         categories=["dog", None],
         scores=inputs["object_detection_scores"],
     )
     with pytest.raises(TypeError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
-            environment=inputs["environment_production"],
+            environment=Environments.PRODUCTION,
             model_type=inputs["model_type_object_detection"],
             prediction_id=inputs["prediction_id"],
             prediction_label=pred_label,
             features=inputs["features"],
             embedding_features=inputs["object_detection_embedding_feature"],
             tags=inputs["tags"],
         )
@@ -1103,15 +1211,15 @@
         categories=inputs["object_detection_categories"],
         scores=[-0.4],
     )
     with pytest.raises(ValueError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
-            environment=inputs["environment_production"],
+            environment=Environments.PRODUCTION,
             model_type=inputs["model_type_object_detection"],
             prediction_id=inputs["prediction_id"],
             prediction_label=pred_label,
             features=inputs["features"],
             embedding_features=inputs["object_detection_embedding_feature"],
             tags=inputs["tags"],
         )
@@ -1122,25 +1230,50 @@
         categories=inputs["object_detection_categories"],
         scores=[1.2],
     )
     with pytest.raises(ValueError) as excinfo:
         _ = c.log(
             model_id=inputs["model_id"],
             model_version=inputs["model_version"],
-            environment=inputs["environment_production"],
+            environment=Environments.PRODUCTION,
             model_type=inputs["model_type_object_detection"],
             prediction_id=inputs["prediction_id"],
             prediction_label=pred_label,
             features=inputs["features"],
             embedding_features=inputs["object_detection_embedding_feature"],
             tags=inputs["tags"],
         )
     assert "Bounding box confidence scores must be between 0 and 1, inclusive" in str(excinfo.value)
 
 
+def test_invalid_tags():
+    c = get_stubbed_client()
+    wrong_tags = {
+        "tag_str_incorrect": "a" * (MAX_TAG_LENGTH + 1),
+    }
+
+    # test case - too long tag value
+    with pytest.raises(ValueError) as excinfo:
+        _ = c.log(
+            model_id=inputs["model_id"],
+            model_type=inputs["model_type_binary_classification"],
+            model_version=inputs["model_version"],
+            environment=Environments.PRODUCTION,
+            prediction_id=inputs["prediction_id"],
+            prediction_label=inputs["label_str"],
+            actual_label=inputs["label_str"],
+            features=inputs["features"],
+            tags=wrong_tags,
+        )
+    assert (
+        f"The number of characters for each tag must be less than or equal to {MAX_TAG_LENGTH}."
+        in str(excinfo.value)
+    )
+
+
 def test_instantiating_client_duplicated_header():
     with pytest.raises(InvalidAdditionalHeaders) as excinfo:
         _ = get_stubbed_client({"authorization": "FAKE_VALUE"})
     assert (
         "Found invalid additional header, cannot use reserved headers named: authorization."
         in str(excinfo.value)
     )
```

### Comparing `arize-7.0.1rc0/tests/test_utils.py` & `arize-7.0.2rc0/tests/test_utils.py`

 * *Files identical despite different names*


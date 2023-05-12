# Comparing `tmp/spacy-llm-0.1.0.tar.gz` & `tmp/spacy-llm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-llm-0.1.0.tar", last modified: Thu May 11 17:08:32 2023, max compression
+gzip compressed data, was "spacy-llm-0.1.1.tar", last modified: Thu May 11 18:33:33 2023, max compression
```

## Comparing `spacy-llm-0.1.0.tar` & `spacy-llm-0.1.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 17:08:32.071598 spacy-llm-0.1.0/
--rw-r--r--   0 vsts      (1001) docker     (122)     1066 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      137 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    28656 2023-05-11 17:08:32.071598 spacy-llm-0.1.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    27541 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      402 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     1481 2023-05-11 17:08:32.071598 spacy-llm-0.1.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 17:08:32.063598 spacy-llm-0.1.0/spacy_llm/
--rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 17:08:32.063598 spacy-llm-0.1.0/spacy_llm/backends/
--rw-r--r--   0 vsts      (1001) docker     (122)      450 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/backends/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3454 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/backends/dolly.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2702 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/backends/langchain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2535 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/backends/minichain.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 17:08:32.067598 spacy-llm-0.1.0/spacy_llm/backends/rest/
--rw-r--r--   0 vsts      (1001) docker     (122)       63 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/backends/rest/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 17:08:32.067598 spacy-llm-0.1.0/spacy_llm/backends/rest/backend/
--rw-r--r--   0 vsts      (1001) docker     (122)      177 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/backends/rest/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4631 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/backends/rest/backend/base.py
--rw-r--r--   0 vsts      (1001) docker     (122)      538 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/backends/rest/backend/noop.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5222 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/backends/rest/backend/openai.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1501 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/backends/rest/registry.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6645 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/cache.py
--rw-r--r--   0 vsts      (1001) docker     (122)      981 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/compat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 17:08:32.067598 spacy-llm-0.1.0/spacy_llm/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10296 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/pipeline/llm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 17:08:32.067598 spacy-llm-0.1.0/spacy_llm/registry/
--rw-r--r--   0 vsts      (1001) docker     (122)      230 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/registry/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      604 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/registry/normalizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1327 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/registry/reader.py
--rw-r--r--   0 vsts      (1001) docker     (122)      413 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/registry/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 17:08:32.067598 spacy-llm-0.1.0/spacy_llm/tasks/
--rw-r--r--   0 vsts      (1001) docker     (122)      135 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tasks/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6632 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tasks/ner.py
--rw-r--r--   0 vsts      (1001) docker     (122)      876 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tasks/noop.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6313 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tasks/textcat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 17:08:32.067598 spacy-llm-0.1.0/spacy_llm/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 17:08:32.067598 spacy-llm-0.1.0/spacy_llm/tests/backends/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/backends/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1465 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/backends/test_dolly.py
--rw-r--r--   0 vsts      (1001) docker     (122)      602 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/backends/test_langchain.py
--rw-r--r--   0 vsts      (1001) docker     (122)      582 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/backends/test_minichain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2247 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/backends/test_rest.py
--rw-r--r--   0 vsts      (1001) docker     (122)      785 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/conftest.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 17:08:32.067598 spacy-llm-0.1.0/spacy_llm/tests/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3375 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/pipeline/test_llm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 17:08:32.067598 spacy-llm-0.1.0/spacy_llm/tests/tasks/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/tasks/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 17:08:32.071598 spacy-llm-0.1.0/spacy_llm/tests/tasks/examples/
--rw-r--r--   0 vsts      (1001) docker     (122)      409 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/tasks/examples/ner_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      233 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/tasks/examples/ner_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/tasks/examples/ner_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/tasks/examples/textcat_binary_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      355 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/tasks/examples/textcat_binary_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      359 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/tasks/examples/textcat_binary_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      417 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      367 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      379 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.json
--rw-r--r--   0 vsts      (1001) docker     (122)      383 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      395 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (122)    12989 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/tasks/test_ner.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14315 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/tasks/test_textcat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5598 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/test_cache.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1302 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/tests/test_combinations.py
--rw-r--r--   0 vsts      (1001) docker     (122)      483 2023-05-11 17:08:19.000000 spacy-llm-0.1.0/spacy_llm/ty.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 17:08:32.063598 spacy-llm-0.1.0/spacy_llm.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    28656 2023-05-11 17:08:32.000000 spacy-llm-0.1.0/spacy_llm.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     2235 2023-05-11 17:08:32.000000 spacy-llm-0.1.0/spacy_llm.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-11 17:08:32.000000 spacy-llm-0.1.0/spacy_llm.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       56 2023-05-11 17:08:32.000000 spacy-llm-0.1.0/spacy_llm.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-11 17:08:31.000000 spacy-llm-0.1.0/spacy_llm.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)       16 2023-05-11 17:08:32.000000 spacy-llm-0.1.0/spacy_llm.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       10 2023-05-11 17:08:32.000000 spacy-llm-0.1.0/spacy_llm.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 18:33:33.285718 spacy-llm-0.1.1/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1066 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      137 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    28518 2023-05-11 18:33:33.285718 spacy-llm-0.1.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    27405 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      402 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1487 2023-05-11 18:33:33.285718 spacy-llm-0.1.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 18:33:33.277718 spacy-llm-0.1.1/spacy_llm/
+-rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 18:33:33.277718 spacy-llm-0.1.1/spacy_llm/backends/
+-rw-r--r--   0 vsts      (1001) docker     (122)      338 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/backends/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3454 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/backends/dolly.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2702 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/backends/langchain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2535 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/backends/minichain.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 18:33:33.281718 spacy-llm-0.1.1/spacy_llm/backends/rest/
+-rw-r--r--   0 vsts      (1001) docker     (122)       63 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/backends/rest/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 18:33:33.281718 spacy-llm-0.1.1/spacy_llm/backends/rest/backend/
+-rw-r--r--   0 vsts      (1001) docker     (122)      177 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/backends/rest/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4631 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/backends/rest/backend/base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      538 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/backends/rest/backend/noop.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5334 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/backends/rest/backend/openai.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1501 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/backends/rest/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6645 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/cache.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      981 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/compat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 18:33:33.281718 spacy-llm-0.1.1/spacy_llm/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10296 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/pipeline/llm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 18:33:33.281718 spacy-llm-0.1.1/spacy_llm/registry/
+-rw-r--r--   0 vsts      (1001) docker     (122)      230 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/registry/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      604 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/registry/normalizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1327 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/registry/reader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      413 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/registry/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 18:33:33.281718 spacy-llm-0.1.1/spacy_llm/tasks/
+-rw-r--r--   0 vsts      (1001) docker     (122)      135 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tasks/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6632 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tasks/ner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      876 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tasks/noop.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6313 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tasks/textcat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 18:33:33.281718 spacy-llm-0.1.1/spacy_llm/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 18:33:33.281718 spacy-llm-0.1.1/spacy_llm/tests/backends/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/backends/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1465 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/backends/test_dolly.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      602 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/backends/test_langchain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      582 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/backends/test_minichain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2247 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/backends/test_rest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      785 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/conftest.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 18:33:33.281718 spacy-llm-0.1.1/spacy_llm/tests/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3375 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/pipeline/test_llm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 18:33:33.281718 spacy-llm-0.1.1/spacy_llm/tests/tasks/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/tasks/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 18:33:33.285718 spacy-llm-0.1.1/spacy_llm/tests/tasks/examples/
+-rw-r--r--   0 vsts      (1001) docker     (122)      409 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/tasks/examples/ner_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      233 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/tasks/examples/ner_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/tasks/examples/ner_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/tasks/examples/textcat_binary_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      355 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/tasks/examples/textcat_binary_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      359 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/tasks/examples/textcat_binary_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      417 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      367 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      379 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/tasks/examples/textcat_multi_excl_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      383 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      395 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)    12989 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/tasks/test_ner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14315 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/tasks/test_textcat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5487 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/test_cache.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1302 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/tests/test_combinations.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      483 2023-05-11 18:33:20.000000 spacy-llm-0.1.1/spacy_llm/ty.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-11 18:33:33.277718 spacy-llm-0.1.1/spacy_llm.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    28518 2023-05-11 18:33:33.000000 spacy-llm-0.1.1/spacy_llm.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     2235 2023-05-11 18:33:33.000000 spacy-llm-0.1.1/spacy_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-11 18:33:33.000000 spacy-llm-0.1.1/spacy_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       56 2023-05-11 18:33:33.000000 spacy-llm-0.1.1/spacy_llm.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-11 18:33:33.000000 spacy-llm-0.1.1/spacy_llm.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)       23 2023-05-11 18:33:33.000000 spacy-llm-0.1.1/spacy_llm.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       10 2023-05-11 18:33:33.000000 spacy-llm-0.1.1/spacy_llm.egg-info/top_level.txt
```

### Comparing `spacy-llm-0.1.0/LICENSE` & `spacy-llm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.0/PKG-INFO` & `spacy-llm-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: spacy-llm
-Version: 0.1.0
-Summary: Integrating generative LLM APIs into spaCy.
+Version: 0.1.1
+Summary: Integrating LLMs into structured NLP pipelines
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/spacy-llm/releases
 Project-URL: Source, https://github.com/explosion/spacy-llm
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
@@ -382,20 +382,19 @@
 
 All built-in backends are registered in `llm_backends`. If no backend is specified, the repo currently connects to the [`OpenAI` API](#openai) by default,
 using the built-in REST protocol, and accesses the `"text-davinci-003"` model.
 
 #### OpenAI
 
 When the backend uses OpenAI, you have to get an API key from openai.com, and ensure that the keys are set as
-environmental variables. For instance, set a `.env` file in the root of your directory with the following information,
-and make sure to exclude this file from git versioning:
+environmental variables:
 
 ```shell
-OPENAI_ORG = "org-..."
-OPENAI_API_KEY = "sk-..."
+export OPENAI_API_KEY="sk-..."
+export OPENAI_API_ORG="org-..."
 ```
 
 #### spacy.REST.v1
 
 This default backend uses `requests` and a simple retry mechanism to access an API.
 
 ```ini
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: spacy-llm Version: 0.1.0 Summary: Integrating
-generative LLM APIs into spaCy. Author: Explosion Author-email:
+Metadata-Version: 2.1 Name: spacy-llm Version: 0.1.1 Summary: Integrating LLMs
+into structured NLP pipelines Author: Explosion Author-email:
 contact@explosion.ai License: MIT Project-URL: Release notes, https://
 github.com/explosion/spacy-llm/releases Project-URL: Source, https://
-github.com/explosion/spacy-llm Classifier: Development Status :: 2 - Pre-Alpha
+github.com/explosion/spacy-llm Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: Microsoft :: Windows Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -224,79 +224,77 @@
 function of type `Callable[[Iterable[Any]], Iterable[Any]]`, but specific
 implementations can have other signatures, like `Callable[[Iterable[str]],
 Iterable[str]]`. All built-in backends are registered in `llm_backends`. If no
 backend is specified, the repo currently connects to the [`OpenAI` API]
 (#openai) by default, using the built-in REST protocol, and accesses the
 `"text-davinci-003"` model. #### OpenAI When the backend uses OpenAI, you have
 to get an API key from openai.com, and ensure that the keys are set as
-environmental variables. For instance, set a `.env` file in the root of your
-directory with the following information, and make sure to exclude this file
-from git versioning: ```shell OPENAI_ORG = "org-..." OPENAI_API_KEY = "sk-..."
-``` #### spacy.REST.v1 This default backend uses `requests` and a simple retry
-mechanism to access an API. ```ini [components.llm.backend] @llm_backends =
-"spacy.REST.v1" api = "OpenAI" config = {"model": "text-davinci-003",
-"temperature": 0.3} ``` | Argument | Type | Default | Description | | ---------
--- | ---------------- | ------- | ---------------------------------------------
------------------------------------------------------------------------ | |
-`api` | `str` | | The name of a supported API. In v.0.1.0, only "OpenAI" is
-supported. | | `config` | `Dict[Any, Any]` | `{}` | Further configuration
-passed on to the backend. | | `strict` | `bool` | `True` | If `True`, raises an
-error if the LLM API returns a malformed response. Otherwise, return the error
-responses as is. | | `max_tries` | `int` | `3` | Max. number of tries for API
-request. | | `timeout` | `int` | `30` | Timeout for API request in seconds. |
-When `api` is set to `OpenAI`, the following settings can be defined in the
-`config` dictionary: - `model`: one of the following list of supported models:
-- `"gpt-4"` - `"gpt-4-0314"` - `"gpt-4-32k"` - `"gpt-4-32k-0314"` - `"gpt-3.5-
-turbo"` - `"gpt-3.5-turbo-0301"` - `"text-davinci-003"` - `"text-davinci-002"`
-- `"text-curie-001"` - `"text-babbage-001"` - `"text-ada-001"` - `"davinci"` -
-`"curie"` - `"babbage"` - `"ada"` - `url`: By default, this is `https://
-api.openai.com/v1/completions`. For models requiring the chat endpoint, use
-`https://api.openai.com/v1/chat/completions`. #### spacy.MiniChain.v1 To use
-[MiniChain](https://github.com/srush/MiniChain) for the API retrieval part,
-make sure you have installed it first: ```shell python -m pip install
-"minichain>=0.3,<0.4" ``` Note that MiniChain currently only supports Python
-3.8, 3.9 and 3.10. Example config blocks: ```ini [components.llm.backend]
-@llm_backends = "spacy.MiniChain.v1" api = "OpenAI"
-[components.llm.backend.query] @llm_queries = "spacy.RunMiniChain.v1" ``` |
-Argument | Type | Default | Description | | -------- | ------------------------
---------------------------------------------------------- | ------- | ---------
--------------------------------------------------------------------------- | |
-`api` | `str` | | The name of an API supported by MiniChain, e.g. "OpenAI". | |
-`config` | `Dict[Any, Any]` | `{}` | Further configuration passed on to the
-backend. | | `query` | `Optional[Callable[["minichain.backend.Backend",
-Iterable[str]], Iterable[str]]]` | `None` | Function that executes the prompts.
-If `None`, defaults to `spacy.RunMiniChain.v1`. | The default `query`
-(`spacy.RunMiniChain.v1`) executes the prompts by running `model(text).run()`
-for each given textual prompt. #### spacy.LangChain.v1 To use [LangChain]
-(https://github.com/hwchase17/langchain) for the API retrieval part, make sure
-you have installed it first: ```shell python -m pip install
-"langchain>=0.0.144,<0.1" ``` Note that LangChain currently only supports
-Python 3.9 and beyond. Example config block: ```ini [components.llm.backend]
-@llm_backends = "spacy.LangChain.v1" api = "OpenAI" query = {"@llm_queries":
-"spacy.CallLangChain.v1"} config = {"temperature": 0.3} ``` | Argument | Type |
-Default | Description | | -------- | ------------------------------------------
------------------------------------- | ------- | ------------------------------
------------------------------------------------------- | | `api` | `str` | |
-The name of an API supported by LangChain, e.g. "OpenAI". | | `config` | `Dict
-[Any, Any]` | `{}` | Further configuration passed on to the backend. | |
-`query` | `Optional[Callable[["langchain.llms.BaseLLM", Iterable[Any]],
-Iterable[Any]]]` | `None` | Function that executes the prompts. If `None`,
-defaults to `spacy.CallLangChain.v1`. | The default `query`
-(`spacy.CallLangChain.v1`) executes the prompts by running `model(text)` for
-each given textual prompt. #### spacy.DollyHF.v1 To use this backend, ideally
-you have a GPU enabled and have installed `transformers`, `torch` and CUDA in
-your virtual environment. This allows you to have the setting `device=cuda:0`
-in your config, which ensures that the model is loaded entirely on the GPU (and
-fails otherwise). ```shell python -m pip install "cupy-cuda11x" python -m pip
-install "torch>=1.13.1,<2.0" python -m pip install "transformers>=4.28.1,<5.0"
-``` If you don't have access to a GPU, you can install `accelerate` and
-set`device_map=auto` instead, but be aware that this may result in some layers
-getting distributed to the CPU or even the hard drive, which may ultimately
-result in extremely slow queries. ```shell python -m pip install
-"accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
+environmental variables: ```shell export OPENAI_API_KEY="sk-..." export
+OPENAI_API_ORG="org-..." ``` #### spacy.REST.v1 This default backend uses
+`requests` and a simple retry mechanism to access an API. ```ini
+[components.llm.backend] @llm_backends = "spacy.REST.v1" api = "OpenAI" config
+= {"model": "text-davinci-003", "temperature": 0.3} ``` | Argument | Type |
+Default | Description | | ----------- | ---------------- | ------- | ----------
+-------------------------------------------------------------------------------
+--------------------------- | | `api` | `str` | | The name of a supported API.
+In v.0.1.0, only "OpenAI" is supported. | | `config` | `Dict[Any, Any]` | `{}`
+| Further configuration passed on to the backend. | | `strict` | `bool` |
+`True` | If `True`, raises an error if the LLM API returns a malformed
+response. Otherwise, return the error responses as is. | | `max_tries` | `int`
+| `3` | Max. number of tries for API request. | | `timeout` | `int` | `30` |
+Timeout for API request in seconds. | When `api` is set to `OpenAI`, the
+following settings can be defined in the `config` dictionary: - `model`: one of
+the following list of supported models: - `"gpt-4"` - `"gpt-4-0314"` - `"gpt-4-
+32k"` - `"gpt-4-32k-0314"` - `"gpt-3.5-turbo"` - `"gpt-3.5-turbo-0301"` -
+`"text-davinci-003"` - `"text-davinci-002"` - `"text-curie-001"` - `"text-
+babbage-001"` - `"text-ada-001"` - `"davinci"` - `"curie"` - `"babbage"` -
+`"ada"` - `url`: By default, this is `https://api.openai.com/v1/completions`.
+For models requiring the chat endpoint, use `https://api.openai.com/v1/chat/
+completions`. #### spacy.MiniChain.v1 To use [MiniChain](https://github.com/
+srush/MiniChain) for the API retrieval part, make sure you have installed it
+first: ```shell python -m pip install "minichain>=0.3,<0.4" ``` Note that
+MiniChain currently only supports Python 3.8, 3.9 and 3.10. Example config
+blocks: ```ini [components.llm.backend] @llm_backends = "spacy.MiniChain.v1"
+api = "OpenAI" [components.llm.backend.query] @llm_queries =
+"spacy.RunMiniChain.v1" ``` | Argument | Type | Default | Description | | -----
+--- | -------------------------------------------------------------------------
+-------- | ------- | ----------------------------------------------------------
+------------------------- | | `api` | `str` | | The name of an API supported by
+MiniChain, e.g. "OpenAI". | | `config` | `Dict[Any, Any]` | `{}` | Further
+configuration passed on to the backend. | | `query` | `Optional[Callable[
+["minichain.backend.Backend", Iterable[str]], Iterable[str]]]` | `None` |
+Function that executes the prompts. If `None`, defaults to
+`spacy.RunMiniChain.v1`. | The default `query` (`spacy.RunMiniChain.v1`)
+executes the prompts by running `model(text).run()` for each given textual
+prompt. #### spacy.LangChain.v1 To use [LangChain](https://github.com/
+hwchase17/langchain) for the API retrieval part, make sure you have installed
+it first: ```shell python -m pip install "langchain>=0.0.144,<0.1" ``` Note
+that LangChain currently only supports Python 3.9 and beyond. Example config
+block: ```ini [components.llm.backend] @llm_backends = "spacy.LangChain.v1" api
+= "OpenAI" query = {"@llm_queries": "spacy.CallLangChain.v1"} config =
+{"temperature": 0.3} ``` | Argument | Type | Default | Description | | -------
+- | ---------------------------------------------------------------------------
+--- | ------- | ---------------------------------------------------------------
+--------------------- | | `api` | `str` | | The name of an API supported by
+LangChain, e.g. "OpenAI". | | `config` | `Dict[Any, Any]` | `{}` | Further
+configuration passed on to the backend. | | `query` | `Optional[Callable[
+["langchain.llms.BaseLLM", Iterable[Any]], Iterable[Any]]]` | `None` | Function
+that executes the prompts. If `None`, defaults to `spacy.CallLangChain.v1`. |
+The default `query` (`spacy.CallLangChain.v1`) executes the prompts by running
+`model(text)` for each given textual prompt. #### spacy.DollyHF.v1 To use this
+backend, ideally you have a GPU enabled and have installed `transformers`,
+`torch` and CUDA in your virtual environment. This allows you to have the
+setting `device=cuda:0` in your config, which ensures that the model is loaded
+entirely on the GPU (and fails otherwise). ```shell python -m pip install
+"cupy-cuda11x" python -m pip install "torch>=1.13.1,<2.0" python -m pip install
+"transformers>=4.28.1,<5.0" ``` If you don't have access to a GPU, you can
+install `accelerate` and set`device_map=auto` instead, but be aware that this
+may result in some layers getting distributed to the CPU or even the hard
+drive, which may ultimately result in extremely slow queries. ```shell python -
+m pip install "accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
 [components.llm.backend] @llm_backends = "spacy.DollyHF.v1" model =
 "databricks/dolly-v2-3b" ``` | Argument | Type | Default | Description | | ----
 ---- | ---------------- | ------- | -------------------------------------------
 ----------------------------------------------------- | | `model` | `str` | |
 The name of a Dolly model that is supported. | | `config` | `Dict[Any, Any]` |
 `{}` | Further configuration passed on to the construction of the model with
 `transformers.pipeline()`. | Supported models (see the [Databricks models page]
```

### Comparing `spacy-llm-0.1.0/README.md` & `spacy-llm-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -354,20 +354,19 @@
 
 All built-in backends are registered in `llm_backends`. If no backend is specified, the repo currently connects to the [`OpenAI` API](#openai) by default,
 using the built-in REST protocol, and accesses the `"text-davinci-003"` model.
 
 #### OpenAI
 
 When the backend uses OpenAI, you have to get an API key from openai.com, and ensure that the keys are set as
-environmental variables. For instance, set a `.env` file in the root of your directory with the following information,
-and make sure to exclude this file from git versioning:
+environmental variables:
 
 ```shell
-OPENAI_ORG = "org-..."
-OPENAI_API_KEY = "sk-..."
+export OPENAI_API_KEY="sk-..."
+export OPENAI_API_ORG="org-..."
 ```
 
 #### spacy.REST.v1
 
 This default backend uses `requests` and a simple retry mechanism to access an API.
 
 ```ini
```

#### html2text {}

```diff
@@ -209,79 +209,77 @@
 function of type `Callable[[Iterable[Any]], Iterable[Any]]`, but specific
 implementations can have other signatures, like `Callable[[Iterable[str]],
 Iterable[str]]`. All built-in backends are registered in `llm_backends`. If no
 backend is specified, the repo currently connects to the [`OpenAI` API]
 (#openai) by default, using the built-in REST protocol, and accesses the
 `"text-davinci-003"` model. #### OpenAI When the backend uses OpenAI, you have
 to get an API key from openai.com, and ensure that the keys are set as
-environmental variables. For instance, set a `.env` file in the root of your
-directory with the following information, and make sure to exclude this file
-from git versioning: ```shell OPENAI_ORG = "org-..." OPENAI_API_KEY = "sk-..."
-``` #### spacy.REST.v1 This default backend uses `requests` and a simple retry
-mechanism to access an API. ```ini [components.llm.backend] @llm_backends =
-"spacy.REST.v1" api = "OpenAI" config = {"model": "text-davinci-003",
-"temperature": 0.3} ``` | Argument | Type | Default | Description | | ---------
--- | ---------------- | ------- | ---------------------------------------------
------------------------------------------------------------------------ | |
-`api` | `str` | | The name of a supported API. In v.0.1.0, only "OpenAI" is
-supported. | | `config` | `Dict[Any, Any]` | `{}` | Further configuration
-passed on to the backend. | | `strict` | `bool` | `True` | If `True`, raises an
-error if the LLM API returns a malformed response. Otherwise, return the error
-responses as is. | | `max_tries` | `int` | `3` | Max. number of tries for API
-request. | | `timeout` | `int` | `30` | Timeout for API request in seconds. |
-When `api` is set to `OpenAI`, the following settings can be defined in the
-`config` dictionary: - `model`: one of the following list of supported models:
-- `"gpt-4"` - `"gpt-4-0314"` - `"gpt-4-32k"` - `"gpt-4-32k-0314"` - `"gpt-3.5-
-turbo"` - `"gpt-3.5-turbo-0301"` - `"text-davinci-003"` - `"text-davinci-002"`
-- `"text-curie-001"` - `"text-babbage-001"` - `"text-ada-001"` - `"davinci"` -
-`"curie"` - `"babbage"` - `"ada"` - `url`: By default, this is `https://
-api.openai.com/v1/completions`. For models requiring the chat endpoint, use
-`https://api.openai.com/v1/chat/completions`. #### spacy.MiniChain.v1 To use
-[MiniChain](https://github.com/srush/MiniChain) for the API retrieval part,
-make sure you have installed it first: ```shell python -m pip install
-"minichain>=0.3,<0.4" ``` Note that MiniChain currently only supports Python
-3.8, 3.9 and 3.10. Example config blocks: ```ini [components.llm.backend]
-@llm_backends = "spacy.MiniChain.v1" api = "OpenAI"
-[components.llm.backend.query] @llm_queries = "spacy.RunMiniChain.v1" ``` |
-Argument | Type | Default | Description | | -------- | ------------------------
---------------------------------------------------------- | ------- | ---------
--------------------------------------------------------------------------- | |
-`api` | `str` | | The name of an API supported by MiniChain, e.g. "OpenAI". | |
-`config` | `Dict[Any, Any]` | `{}` | Further configuration passed on to the
-backend. | | `query` | `Optional[Callable[["minichain.backend.Backend",
-Iterable[str]], Iterable[str]]]` | `None` | Function that executes the prompts.
-If `None`, defaults to `spacy.RunMiniChain.v1`. | The default `query`
-(`spacy.RunMiniChain.v1`) executes the prompts by running `model(text).run()`
-for each given textual prompt. #### spacy.LangChain.v1 To use [LangChain]
-(https://github.com/hwchase17/langchain) for the API retrieval part, make sure
-you have installed it first: ```shell python -m pip install
-"langchain>=0.0.144,<0.1" ``` Note that LangChain currently only supports
-Python 3.9 and beyond. Example config block: ```ini [components.llm.backend]
-@llm_backends = "spacy.LangChain.v1" api = "OpenAI" query = {"@llm_queries":
-"spacy.CallLangChain.v1"} config = {"temperature": 0.3} ``` | Argument | Type |
-Default | Description | | -------- | ------------------------------------------
------------------------------------- | ------- | ------------------------------
------------------------------------------------------- | | `api` | `str` | |
-The name of an API supported by LangChain, e.g. "OpenAI". | | `config` | `Dict
-[Any, Any]` | `{}` | Further configuration passed on to the backend. | |
-`query` | `Optional[Callable[["langchain.llms.BaseLLM", Iterable[Any]],
-Iterable[Any]]]` | `None` | Function that executes the prompts. If `None`,
-defaults to `spacy.CallLangChain.v1`. | The default `query`
-(`spacy.CallLangChain.v1`) executes the prompts by running `model(text)` for
-each given textual prompt. #### spacy.DollyHF.v1 To use this backend, ideally
-you have a GPU enabled and have installed `transformers`, `torch` and CUDA in
-your virtual environment. This allows you to have the setting `device=cuda:0`
-in your config, which ensures that the model is loaded entirely on the GPU (and
-fails otherwise). ```shell python -m pip install "cupy-cuda11x" python -m pip
-install "torch>=1.13.1,<2.0" python -m pip install "transformers>=4.28.1,<5.0"
-``` If you don't have access to a GPU, you can install `accelerate` and
-set`device_map=auto` instead, but be aware that this may result in some layers
-getting distributed to the CPU or even the hard drive, which may ultimately
-result in extremely slow queries. ```shell python -m pip install
-"accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
+environmental variables: ```shell export OPENAI_API_KEY="sk-..." export
+OPENAI_API_ORG="org-..." ``` #### spacy.REST.v1 This default backend uses
+`requests` and a simple retry mechanism to access an API. ```ini
+[components.llm.backend] @llm_backends = "spacy.REST.v1" api = "OpenAI" config
+= {"model": "text-davinci-003", "temperature": 0.3} ``` | Argument | Type |
+Default | Description | | ----------- | ---------------- | ------- | ----------
+-------------------------------------------------------------------------------
+--------------------------- | | `api` | `str` | | The name of a supported API.
+In v.0.1.0, only "OpenAI" is supported. | | `config` | `Dict[Any, Any]` | `{}`
+| Further configuration passed on to the backend. | | `strict` | `bool` |
+`True` | If `True`, raises an error if the LLM API returns a malformed
+response. Otherwise, return the error responses as is. | | `max_tries` | `int`
+| `3` | Max. number of tries for API request. | | `timeout` | `int` | `30` |
+Timeout for API request in seconds. | When `api` is set to `OpenAI`, the
+following settings can be defined in the `config` dictionary: - `model`: one of
+the following list of supported models: - `"gpt-4"` - `"gpt-4-0314"` - `"gpt-4-
+32k"` - `"gpt-4-32k-0314"` - `"gpt-3.5-turbo"` - `"gpt-3.5-turbo-0301"` -
+`"text-davinci-003"` - `"text-davinci-002"` - `"text-curie-001"` - `"text-
+babbage-001"` - `"text-ada-001"` - `"davinci"` - `"curie"` - `"babbage"` -
+`"ada"` - `url`: By default, this is `https://api.openai.com/v1/completions`.
+For models requiring the chat endpoint, use `https://api.openai.com/v1/chat/
+completions`. #### spacy.MiniChain.v1 To use [MiniChain](https://github.com/
+srush/MiniChain) for the API retrieval part, make sure you have installed it
+first: ```shell python -m pip install "minichain>=0.3,<0.4" ``` Note that
+MiniChain currently only supports Python 3.8, 3.9 and 3.10. Example config
+blocks: ```ini [components.llm.backend] @llm_backends = "spacy.MiniChain.v1"
+api = "OpenAI" [components.llm.backend.query] @llm_queries =
+"spacy.RunMiniChain.v1" ``` | Argument | Type | Default | Description | | -----
+--- | -------------------------------------------------------------------------
+-------- | ------- | ----------------------------------------------------------
+------------------------- | | `api` | `str` | | The name of an API supported by
+MiniChain, e.g. "OpenAI". | | `config` | `Dict[Any, Any]` | `{}` | Further
+configuration passed on to the backend. | | `query` | `Optional[Callable[
+["minichain.backend.Backend", Iterable[str]], Iterable[str]]]` | `None` |
+Function that executes the prompts. If `None`, defaults to
+`spacy.RunMiniChain.v1`. | The default `query` (`spacy.RunMiniChain.v1`)
+executes the prompts by running `model(text).run()` for each given textual
+prompt. #### spacy.LangChain.v1 To use [LangChain](https://github.com/
+hwchase17/langchain) for the API retrieval part, make sure you have installed
+it first: ```shell python -m pip install "langchain>=0.0.144,<0.1" ``` Note
+that LangChain currently only supports Python 3.9 and beyond. Example config
+block: ```ini [components.llm.backend] @llm_backends = "spacy.LangChain.v1" api
+= "OpenAI" query = {"@llm_queries": "spacy.CallLangChain.v1"} config =
+{"temperature": 0.3} ``` | Argument | Type | Default | Description | | -------
+- | ---------------------------------------------------------------------------
+--- | ------- | ---------------------------------------------------------------
+--------------------- | | `api` | `str` | | The name of an API supported by
+LangChain, e.g. "OpenAI". | | `config` | `Dict[Any, Any]` | `{}` | Further
+configuration passed on to the backend. | | `query` | `Optional[Callable[
+["langchain.llms.BaseLLM", Iterable[Any]], Iterable[Any]]]` | `None` | Function
+that executes the prompts. If `None`, defaults to `spacy.CallLangChain.v1`. |
+The default `query` (`spacy.CallLangChain.v1`) executes the prompts by running
+`model(text)` for each given textual prompt. #### spacy.DollyHF.v1 To use this
+backend, ideally you have a GPU enabled and have installed `transformers`,
+`torch` and CUDA in your virtual environment. This allows you to have the
+setting `device=cuda:0` in your config, which ensures that the model is loaded
+entirely on the GPU (and fails otherwise). ```shell python -m pip install
+"cupy-cuda11x" python -m pip install "torch>=1.13.1,<2.0" python -m pip install
+"transformers>=4.28.1,<5.0" ``` If you don't have access to a GPU, you can
+install `accelerate` and set`device_map=auto` instead, but be aware that this
+may result in some layers getting distributed to the CPU or even the hard
+drive, which may ultimately result in extremely slow queries. ```shell python -
+m pip install "accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
 [components.llm.backend] @llm_backends = "spacy.DollyHF.v1" model =
 "databricks/dolly-v2-3b" ``` | Argument | Type | Default | Description | | ----
 ---- | ---------------- | ------- | -------------------------------------------
 ----------------------------------------------------- | | `model` | `str` | |
 The name of a Dolly model that is supported. | | `config` | `Dict[Any, Any]` |
 `{}` | Further configuration passed on to the construction of the model with
 `transformers.pipeline()`. | Supported models (see the [Databricks models page]
```

### Comparing `spacy-llm-0.1.0/setup.cfg` & `spacy-llm-0.1.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [metadata]
-version = 0.1.0
-description = Integrating generative LLM APIs into spaCy.
+version = 0.1.1
+description = Integrating LLMs into structured NLP pipelines
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
-	Development Status :: 2 - Pre-Alpha
+	Development Status :: 4 - Beta
 	Environment :: Console
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Operating System :: POSIX :: Linux
 	Operating System :: MacOS :: MacOS X
 	Operating System :: Microsoft :: Windows
@@ -28,14 +28,15 @@
 
 [options]
 zip_safe = false
 include_package_data = true
 python_requires = >=3.6
 install_requires = 
 	spacy>=3.5,<4.0
+	jinja2
 
 [options.entry_points]
 spacy_factories = 
 	llm = spacy_llm.pipeline.llm:make_llm
 
 [bdist_wheel]
 universal = true
```

### Comparing `spacy-llm-0.1.0/spacy_llm/backends/dolly.py` & `spacy-llm-0.1.1/spacy_llm/backends/dolly.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.0/spacy_llm/backends/langchain.py` & `spacy-llm-0.1.1/spacy_llm/backends/langchain.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.0/spacy_llm/backends/minichain.py` & `spacy-llm-0.1.1/spacy_llm/backends/minichain.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.0/spacy_llm/backends/rest/backend/base.py` & `spacy-llm-0.1.1/spacy_llm/backends/rest/backend/base.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.0/spacy_llm/backends/rest/backend/noop.py` & `spacy-llm-0.1.1/spacy_llm/backends/rest/backend/noop.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.0/spacy_llm/backends/rest/backend/openai.py` & `spacy-llm-0.1.1/spacy_llm/backends/rest/backend/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,24 +38,29 @@
         }
 
     @property
     def credentials(self) -> Dict[str, str]:
         model = self._config["model"]
         # Fetch and check the key
         api_key = os.getenv("OPENAI_API_KEY")
+        api_org = os.getenv("OPENAI_API_ORG")
         if api_key is None:
             raise ValueError(
                 "Could not find the API key to access the OpenAI API. Ensure you have an API key "
                 "set up via https://platform.openai.com/account/api-keys, then make it available as "
-                "an environment variable 'OPENAI_API_KEY', for instance in a .env file."
+                "an environment variable 'OPENAI_API_KEY."
             )
 
         # Check the access and get a list of available models to verify the model argument (if not None)
         # Even if the model is None, this call is used as a healthcheck to verify access.
-        headers = {"Authorization": f"Bearer {api_key}"}
+        headers = {
+            "Authorization": f"Bearer {api_key}",
+        }
+        if api_org:
+            headers["OpenAI-Organization"] = api_org
         r = self.retry(
             lambda: requests.get(
                 "https://api.openai.com/v1/models",
                 headers=headers,
             ),
         )
         if r.status_code == 422:
```

### Comparing `spacy-llm-0.1.0/spacy_llm/backends/rest/registry.py` & `spacy-llm-0.1.1/spacy_llm/backends/rest/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.0/spacy_llm/cache.py` & `spacy-llm-0.1.1/spacy_llm/cache.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.0/spacy_llm/compat.py` & `spacy-llm-0.1.1/spacy_llm/compat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.0/spacy_llm/pipeline/llm.py` & `spacy-llm-0.1.1/spacy_llm/pipeline/llm.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.0/spacy_llm/registry/normalizer.py` & `spacy-llm-0.1.1/spacy_llm/registry/normalizer.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.0/spacy_llm/registry/reader.py` & `spacy-llm-0.1.1/spacy_llm/registry/reader.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.0/spacy_llm/tasks/ner.py` & `spacy-llm-0.1.1/spacy_llm/tasks/ner.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.0/spacy_llm/tasks/noop.py` & `spacy-llm-0.1.1/spacy_llm/tasks/noop.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.0/spacy_llm/tasks/textcat.py` & `spacy-llm-0.1.1/spacy_llm/tasks/textcat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.0/spacy_llm/tests/backends/test_dolly.py` & `spacy-llm-0.1.1/spacy_llm/tests/backends/test_dolly.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.0/spacy_llm/tests/backends/test_langchain.py` & `spacy-llm-0.1.1/spacy_llm/tests/backends/test_langchain.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.0/spacy_llm/tests/backends/test_minichain.py` & `spacy-llm-0.1.1/spacy_llm/tests/backends/test_minichain.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.0/spacy_llm/tests/backends/test_rest.py` & `spacy-llm-0.1.1/spacy_llm/tests/backends/test_rest.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.0/spacy_llm/tests/conftest.py` & `spacy-llm-0.1.1/spacy_llm/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.0/spacy_llm/tests/pipeline/test_llm.py` & `spacy-llm-0.1.1/spacy_llm/tests/pipeline/test_llm.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.0/spacy_llm/tests/tasks/test_ner.py` & `spacy-llm-0.1.1/spacy_llm/tests/tasks/test_ner.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.0/spacy_llm/tests/tasks/test_textcat.py` & `spacy-llm-0.1.1/spacy_llm/tests/tasks/test_textcat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.0/spacy_llm/tests/test_cache.py` & `spacy-llm-0.1.1/spacy_llm/tests/test_cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import time
 from pathlib import Path
 from typing import Dict
 
 import pytest
 import srsly  # type: ignore[import]
-from dotenv import load_dotenv  # type: ignore[import]
 import spacy
 from spacy import Language
 from spacy.tokens import DocBin
 import copy
 
 from ..cache import Cache
 
 
-load_dotenv()  # take environment variables from .env.
-
 _DEFAULT_CFG = {
     "backend": {"api": "NoOp", "config": {"model": "NoOp"}},
     "task": {"@llm_tasks": "spacy.NoOp.v1"},
     "cache": {
         "batch_size": 2,
         "max_batches_in_mem": 3,
     },
```

### Comparing `spacy-llm-0.1.0/spacy_llm/tests/test_combinations.py` & `spacy-llm-0.1.1/spacy_llm/tests/test_combinations.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.1.0/spacy_llm.egg-info/PKG-INFO` & `spacy-llm-0.1.1/spacy_llm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: spacy-llm
-Version: 0.1.0
-Summary: Integrating generative LLM APIs into spaCy.
+Version: 0.1.1
+Summary: Integrating LLMs into structured NLP pipelines
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/spacy-llm/releases
 Project-URL: Source, https://github.com/explosion/spacy-llm
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
@@ -382,20 +382,19 @@
 
 All built-in backends are registered in `llm_backends`. If no backend is specified, the repo currently connects to the [`OpenAI` API](#openai) by default,
 using the built-in REST protocol, and accesses the `"text-davinci-003"` model.
 
 #### OpenAI
 
 When the backend uses OpenAI, you have to get an API key from openai.com, and ensure that the keys are set as
-environmental variables. For instance, set a `.env` file in the root of your directory with the following information,
-and make sure to exclude this file from git versioning:
+environmental variables:
 
 ```shell
-OPENAI_ORG = "org-..."
-OPENAI_API_KEY = "sk-..."
+export OPENAI_API_KEY="sk-..."
+export OPENAI_API_ORG="org-..."
 ```
 
 #### spacy.REST.v1
 
 This default backend uses `requests` and a simple retry mechanism to access an API.
 
 ```ini
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: spacy-llm Version: 0.1.0 Summary: Integrating
-generative LLM APIs into spaCy. Author: Explosion Author-email:
+Metadata-Version: 2.1 Name: spacy-llm Version: 0.1.1 Summary: Integrating LLMs
+into structured NLP pipelines Author: Explosion Author-email:
 contact@explosion.ai License: MIT Project-URL: Release notes, https://
 github.com/explosion/spacy-llm/releases Project-URL: Source, https://
-github.com/explosion/spacy-llm Classifier: Development Status :: 2 - Pre-Alpha
+github.com/explosion/spacy-llm Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: Microsoft :: Windows Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -224,79 +224,77 @@
 function of type `Callable[[Iterable[Any]], Iterable[Any]]`, but specific
 implementations can have other signatures, like `Callable[[Iterable[str]],
 Iterable[str]]`. All built-in backends are registered in `llm_backends`. If no
 backend is specified, the repo currently connects to the [`OpenAI` API]
 (#openai) by default, using the built-in REST protocol, and accesses the
 `"text-davinci-003"` model. #### OpenAI When the backend uses OpenAI, you have
 to get an API key from openai.com, and ensure that the keys are set as
-environmental variables. For instance, set a `.env` file in the root of your
-directory with the following information, and make sure to exclude this file
-from git versioning: ```shell OPENAI_ORG = "org-..." OPENAI_API_KEY = "sk-..."
-``` #### spacy.REST.v1 This default backend uses `requests` and a simple retry
-mechanism to access an API. ```ini [components.llm.backend] @llm_backends =
-"spacy.REST.v1" api = "OpenAI" config = {"model": "text-davinci-003",
-"temperature": 0.3} ``` | Argument | Type | Default | Description | | ---------
--- | ---------------- | ------- | ---------------------------------------------
------------------------------------------------------------------------ | |
-`api` | `str` | | The name of a supported API. In v.0.1.0, only "OpenAI" is
-supported. | | `config` | `Dict[Any, Any]` | `{}` | Further configuration
-passed on to the backend. | | `strict` | `bool` | `True` | If `True`, raises an
-error if the LLM API returns a malformed response. Otherwise, return the error
-responses as is. | | `max_tries` | `int` | `3` | Max. number of tries for API
-request. | | `timeout` | `int` | `30` | Timeout for API request in seconds. |
-When `api` is set to `OpenAI`, the following settings can be defined in the
-`config` dictionary: - `model`: one of the following list of supported models:
-- `"gpt-4"` - `"gpt-4-0314"` - `"gpt-4-32k"` - `"gpt-4-32k-0314"` - `"gpt-3.5-
-turbo"` - `"gpt-3.5-turbo-0301"` - `"text-davinci-003"` - `"text-davinci-002"`
-- `"text-curie-001"` - `"text-babbage-001"` - `"text-ada-001"` - `"davinci"` -
-`"curie"` - `"babbage"` - `"ada"` - `url`: By default, this is `https://
-api.openai.com/v1/completions`. For models requiring the chat endpoint, use
-`https://api.openai.com/v1/chat/completions`. #### spacy.MiniChain.v1 To use
-[MiniChain](https://github.com/srush/MiniChain) for the API retrieval part,
-make sure you have installed it first: ```shell python -m pip install
-"minichain>=0.3,<0.4" ``` Note that MiniChain currently only supports Python
-3.8, 3.9 and 3.10. Example config blocks: ```ini [components.llm.backend]
-@llm_backends = "spacy.MiniChain.v1" api = "OpenAI"
-[components.llm.backend.query] @llm_queries = "spacy.RunMiniChain.v1" ``` |
-Argument | Type | Default | Description | | -------- | ------------------------
---------------------------------------------------------- | ------- | ---------
--------------------------------------------------------------------------- | |
-`api` | `str` | | The name of an API supported by MiniChain, e.g. "OpenAI". | |
-`config` | `Dict[Any, Any]` | `{}` | Further configuration passed on to the
-backend. | | `query` | `Optional[Callable[["minichain.backend.Backend",
-Iterable[str]], Iterable[str]]]` | `None` | Function that executes the prompts.
-If `None`, defaults to `spacy.RunMiniChain.v1`. | The default `query`
-(`spacy.RunMiniChain.v1`) executes the prompts by running `model(text).run()`
-for each given textual prompt. #### spacy.LangChain.v1 To use [LangChain]
-(https://github.com/hwchase17/langchain) for the API retrieval part, make sure
-you have installed it first: ```shell python -m pip install
-"langchain>=0.0.144,<0.1" ``` Note that LangChain currently only supports
-Python 3.9 and beyond. Example config block: ```ini [components.llm.backend]
-@llm_backends = "spacy.LangChain.v1" api = "OpenAI" query = {"@llm_queries":
-"spacy.CallLangChain.v1"} config = {"temperature": 0.3} ``` | Argument | Type |
-Default | Description | | -------- | ------------------------------------------
------------------------------------- | ------- | ------------------------------
------------------------------------------------------- | | `api` | `str` | |
-The name of an API supported by LangChain, e.g. "OpenAI". | | `config` | `Dict
-[Any, Any]` | `{}` | Further configuration passed on to the backend. | |
-`query` | `Optional[Callable[["langchain.llms.BaseLLM", Iterable[Any]],
-Iterable[Any]]]` | `None` | Function that executes the prompts. If `None`,
-defaults to `spacy.CallLangChain.v1`. | The default `query`
-(`spacy.CallLangChain.v1`) executes the prompts by running `model(text)` for
-each given textual prompt. #### spacy.DollyHF.v1 To use this backend, ideally
-you have a GPU enabled and have installed `transformers`, `torch` and CUDA in
-your virtual environment. This allows you to have the setting `device=cuda:0`
-in your config, which ensures that the model is loaded entirely on the GPU (and
-fails otherwise). ```shell python -m pip install "cupy-cuda11x" python -m pip
-install "torch>=1.13.1,<2.0" python -m pip install "transformers>=4.28.1,<5.0"
-``` If you don't have access to a GPU, you can install `accelerate` and
-set`device_map=auto` instead, but be aware that this may result in some layers
-getting distributed to the CPU or even the hard drive, which may ultimately
-result in extremely slow queries. ```shell python -m pip install
-"accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
+environmental variables: ```shell export OPENAI_API_KEY="sk-..." export
+OPENAI_API_ORG="org-..." ``` #### spacy.REST.v1 This default backend uses
+`requests` and a simple retry mechanism to access an API. ```ini
+[components.llm.backend] @llm_backends = "spacy.REST.v1" api = "OpenAI" config
+= {"model": "text-davinci-003", "temperature": 0.3} ``` | Argument | Type |
+Default | Description | | ----------- | ---------------- | ------- | ----------
+-------------------------------------------------------------------------------
+--------------------------- | | `api` | `str` | | The name of a supported API.
+In v.0.1.0, only "OpenAI" is supported. | | `config` | `Dict[Any, Any]` | `{}`
+| Further configuration passed on to the backend. | | `strict` | `bool` |
+`True` | If `True`, raises an error if the LLM API returns a malformed
+response. Otherwise, return the error responses as is. | | `max_tries` | `int`
+| `3` | Max. number of tries for API request. | | `timeout` | `int` | `30` |
+Timeout for API request in seconds. | When `api` is set to `OpenAI`, the
+following settings can be defined in the `config` dictionary: - `model`: one of
+the following list of supported models: - `"gpt-4"` - `"gpt-4-0314"` - `"gpt-4-
+32k"` - `"gpt-4-32k-0314"` - `"gpt-3.5-turbo"` - `"gpt-3.5-turbo-0301"` -
+`"text-davinci-003"` - `"text-davinci-002"` - `"text-curie-001"` - `"text-
+babbage-001"` - `"text-ada-001"` - `"davinci"` - `"curie"` - `"babbage"` -
+`"ada"` - `url`: By default, this is `https://api.openai.com/v1/completions`.
+For models requiring the chat endpoint, use `https://api.openai.com/v1/chat/
+completions`. #### spacy.MiniChain.v1 To use [MiniChain](https://github.com/
+srush/MiniChain) for the API retrieval part, make sure you have installed it
+first: ```shell python -m pip install "minichain>=0.3,<0.4" ``` Note that
+MiniChain currently only supports Python 3.8, 3.9 and 3.10. Example config
+blocks: ```ini [components.llm.backend] @llm_backends = "spacy.MiniChain.v1"
+api = "OpenAI" [components.llm.backend.query] @llm_queries =
+"spacy.RunMiniChain.v1" ``` | Argument | Type | Default | Description | | -----
+--- | -------------------------------------------------------------------------
+-------- | ------- | ----------------------------------------------------------
+------------------------- | | `api` | `str` | | The name of an API supported by
+MiniChain, e.g. "OpenAI". | | `config` | `Dict[Any, Any]` | `{}` | Further
+configuration passed on to the backend. | | `query` | `Optional[Callable[
+["minichain.backend.Backend", Iterable[str]], Iterable[str]]]` | `None` |
+Function that executes the prompts. If `None`, defaults to
+`spacy.RunMiniChain.v1`. | The default `query` (`spacy.RunMiniChain.v1`)
+executes the prompts by running `model(text).run()` for each given textual
+prompt. #### spacy.LangChain.v1 To use [LangChain](https://github.com/
+hwchase17/langchain) for the API retrieval part, make sure you have installed
+it first: ```shell python -m pip install "langchain>=0.0.144,<0.1" ``` Note
+that LangChain currently only supports Python 3.9 and beyond. Example config
+block: ```ini [components.llm.backend] @llm_backends = "spacy.LangChain.v1" api
+= "OpenAI" query = {"@llm_queries": "spacy.CallLangChain.v1"} config =
+{"temperature": 0.3} ``` | Argument | Type | Default | Description | | -------
+- | ---------------------------------------------------------------------------
+--- | ------- | ---------------------------------------------------------------
+--------------------- | | `api` | `str` | | The name of an API supported by
+LangChain, e.g. "OpenAI". | | `config` | `Dict[Any, Any]` | `{}` | Further
+configuration passed on to the backend. | | `query` | `Optional[Callable[
+["langchain.llms.BaseLLM", Iterable[Any]], Iterable[Any]]]` | `None` | Function
+that executes the prompts. If `None`, defaults to `spacy.CallLangChain.v1`. |
+The default `query` (`spacy.CallLangChain.v1`) executes the prompts by running
+`model(text)` for each given textual prompt. #### spacy.DollyHF.v1 To use this
+backend, ideally you have a GPU enabled and have installed `transformers`,
+`torch` and CUDA in your virtual environment. This allows you to have the
+setting `device=cuda:0` in your config, which ensures that the model is loaded
+entirely on the GPU (and fails otherwise). ```shell python -m pip install
+"cupy-cuda11x" python -m pip install "torch>=1.13.1,<2.0" python -m pip install
+"transformers>=4.28.1,<5.0" ``` If you don't have access to a GPU, you can
+install `accelerate` and set`device_map=auto` instead, but be aware that this
+may result in some layers getting distributed to the CPU or even the hard
+drive, which may ultimately result in extremely slow queries. ```shell python -
+m pip install "accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
 [components.llm.backend] @llm_backends = "spacy.DollyHF.v1" model =
 "databricks/dolly-v2-3b" ``` | Argument | Type | Default | Description | | ----
 ---- | ---------------- | ------- | -------------------------------------------
 ----------------------------------------------------- | | `model` | `str` | |
 The name of a Dolly model that is supported. | | `config` | `Dict[Any, Any]` |
 `{}` | Further configuration passed on to the construction of the model with
 `transformers.pipeline()`. | Supported models (see the [Databricks models page]
```

### Comparing `spacy-llm-0.1.0/spacy_llm.egg-info/SOURCES.txt` & `spacy-llm-0.1.1/spacy_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*


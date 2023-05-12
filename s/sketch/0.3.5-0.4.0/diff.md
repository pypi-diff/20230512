# Comparing `tmp/sketch-0.3.5.tar.gz` & `tmp/sketch-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sketch-0.3.5.tar", last modified: Thu Feb 16 03:01:15 2023, max compression
+gzip compressed data, was "sketch-0.4.0.tar", last modified: Fri May 12 11:35:19 2023, max compression
```

## Comparing `sketch-0.3.5.tar` & `sketch-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 03:01:15.525432 sketch-0.3.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 03:01:15.513432 sketch-0.3.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 03:01:15.517432 sketch-0.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-02-16 03:01:05.000000 sketch-0.3.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-02-16 03:01:05.000000 sketch-0.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-02-16 03:01:05.000000 sketch-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-02-16 03:01:15.525432 sketch-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-02-16 03:01:05.000000 sketch-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-16 03:01:05.000000 sketch-0.3.5/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-02-16 03:01:05.000000 sketch-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-16 03:01:15.525432 sketch-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-16 03:01:05.000000 sketch-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 03:01:15.521432 sketch-0.3.5/sketch/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-16 03:01:05.000000 sketch-0.3.5/sketch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-02-16 03:01:05.000000 sketch-0.3.5/sketch/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-02-16 03:01:05.000000 sketch-0.3.5/sketch/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-02-16 03:01:05.000000 sketch-0.3.5/sketch/pandas_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-02-16 03:01:05.000000 sketch-0.3.5/sketch/references.py
--rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-02-16 03:01:05.000000 sketch-0.3.5/sketch/sketches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 03:01:15.521432 sketch-0.3.5/sketch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-02-16 03:01:15.000000 sketch-0.3.5/sketch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-02-16 03:01:15.000000 sketch-0.3.5/sketch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 03:01:15.000000 sketch-0.3.5/sketch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-02-16 03:01:15.000000 sketch-0.3.5/sketch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-16 03:01:15.000000 sketch-0.3.5/sketch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 03:01:15.521432 sketch-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-02-16 03:01:05.000000 sketch-0.3.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-02-16 03:01:05.000000 sketch-0.3.5/tests/test_calculate_sketches.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-02-16 03:01:05.000000 sketch-0.3.5/tests/test_metrics_from_sketchpads.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-02-16 03:01:05.000000 sketch-0.3.5/tests/test_pandas_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:35:19.117330 sketch-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:35:19.109330 sketch-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:35:19.113330 sketch-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-12 11:35:09.000000 sketch-0.4.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-12 11:35:09.000000 sketch-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-12 11:35:09.000000 sketch-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-12 11:35:19.117330 sketch-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-12 11:35:09.000000 sketch-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-12 11:35:09.000000 sketch-0.4.0/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-12 11:35:09.000000 sketch-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 11:35:19.117330 sketch-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 11:35:09.000000 sketch-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:35:19.117330 sketch-0.4.0/sketch/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-12 11:35:09.000000 sketch-0.4.0/sketch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-05-12 11:35:09.000000 sketch-0.4.0/sketch/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-05-12 11:35:09.000000 sketch-0.4.0/sketch/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-05-12 11:35:09.000000 sketch-0.4.0/sketch/pandas_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-12 11:35:09.000000 sketch-0.4.0/sketch/references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-05-12 11:35:09.000000 sketch-0.4.0/sketch/sketches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:35:19.117330 sketch-0.4.0/sketch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-12 11:35:19.000000 sketch-0.4.0/sketch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-12 11:35:19.000000 sketch-0.4.0/sketch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 11:35:19.000000 sketch-0.4.0/sketch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-12 11:35:19.000000 sketch-0.4.0/sketch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 11:35:19.000000 sketch-0.4.0/sketch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:35:19.117330 sketch-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-12 11:35:09.000000 sketch-0.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-12 11:35:09.000000 sketch-0.4.0/tests/test_calculate_sketches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-12 11:35:09.000000 sketch-0.4.0/tests/test_metrics_from_sketchpads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-12 11:35:09.000000 sketch-0.4.0/tests/test_pandas_extension.py
```

### Comparing `sketch-0.3.5/.github/workflows/publish-to-pypi.yml` & `sketch-0.4.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `sketch-0.3.5/.gitignore` & `sketch-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sketch-0.3.5/LICENSE` & `sketch-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sketch-0.3.5/PKG-INFO` & `sketch-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sketch
-Version: 0.3.5
+Version: 0.4.0
 Summary: Compute, store and operate on data sketches
 License: MIT License
         
         Copyright (c) 2023 Justin Waugh, Mike Biven
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -25,29 +25,31 @@
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/approximatelabs/sketch
 Keywords: data,sketch,model,etl,automatic,join,ai,embedding,profiling
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: local
+Provides-Extra: all
 License-File: LICENSE
 
 [![](https://dcbadge.vercel.app/api/server/kW9nBQErGe?compact=true&style=flat)](https://discord.gg/kW9nBQErGe)
 
 # sketch
 
 Sketch is an AI code-writing assistant for pandas users that understands the context of your data, greatly improving the relevance of suggestions. Sketch is usable in seconds and doesn't require adding a plugin to your IDE.
 
 ```bash
 pip install sketch
 ```
 
 ## Demo 
 
-Here we follow a "standard" (hypothetical) data-analysis workflow, showing a Natural Language interace that successfully navigates many tasks in the data stack landscape. 
+Here we follow a "standard" (hypothetical) data-analysis workflow, showing a Natural Language interface that successfully navigates many tasks in the data stack landscape. 
 
 - Data Catalogging:
   - General tagging (eg. PII identification)
   - Metadata generation (names and descriptions)
 - Data Engineering:
   - Data cleaning and masking (compliance)
   - Derived feature creation and extraction
@@ -97,15 +99,22 @@
 
 ```python
 df['capitol'] = pd.DataFrame({'State': ['Colorado', 'Kansas', 'California', 'New York']}).sketch.apply("What is the capitol of [{{ State }}]?")
 ```
 
 ## Sketch currently uses `prompts.approx.dev` to help run with minimal setup
 
-In the future, we plan to update the prompts at this endpoint with our own custom foundation model, built to answer questions more accurately than GPT-3 can with its minimal data context. 
+You can also directly use a few pre-built hugging face models (right now `MPT-7B` and `StarCoder`), which will run entirely locally (once you download the model weights from HF).
+Do this by setting environment 3 variables:
+
+```python
+os.environ['LAMBDAPROMPT_BACKEND'] = 'StarCoder'
+os.environ['SKETCH_USE_REMOTE_LAMBDAPROMPT'] = 'False'
+os.environ['HF_ACCESS_TOKEN'] = 'your_hugging_face_token'
+```
 
 You can also directly call OpenAI directly (and not use our endpoint) by using your own API key. To do this, set 2 environment variables.
 
 (1) `SKETCH_USE_REMOTE_LAMBDAPROMPT=False`
 (2) `OPENAI_API_KEY=YOUR_API_KEY`
 
 ## How it works
```

### Comparing `sketch-0.3.5/README.md` & `sketch-0.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ```bash
 pip install sketch
 ```
 
 ## Demo 
 
-Here we follow a "standard" (hypothetical) data-analysis workflow, showing a Natural Language interace that successfully navigates many tasks in the data stack landscape. 
+Here we follow a "standard" (hypothetical) data-analysis workflow, showing a Natural Language interface that successfully navigates many tasks in the data stack landscape. 
 
 - Data Catalogging:
   - General tagging (eg. PII identification)
   - Metadata generation (names and descriptions)
 - Data Engineering:
   - Data cleaning and masking (compliance)
   - Derived feature creation and extraction
@@ -64,15 +64,22 @@
 
 ```python
 df['capitol'] = pd.DataFrame({'State': ['Colorado', 'Kansas', 'California', 'New York']}).sketch.apply("What is the capitol of [{{ State }}]?")
 ```
 
 ## Sketch currently uses `prompts.approx.dev` to help run with minimal setup
 
-In the future, we plan to update the prompts at this endpoint with our own custom foundation model, built to answer questions more accurately than GPT-3 can with its minimal data context. 
+You can also directly use a few pre-built hugging face models (right now `MPT-7B` and `StarCoder`), which will run entirely locally (once you download the model weights from HF).
+Do this by setting environment 3 variables:
+
+```python
+os.environ['LAMBDAPROMPT_BACKEND'] = 'StarCoder'
+os.environ['SKETCH_USE_REMOTE_LAMBDAPROMPT'] = 'False'
+os.environ['HF_ACCESS_TOKEN'] = 'your_hugging_face_token'
+```
 
 You can also directly call OpenAI directly (and not use our endpoint) by using your own API key. To do this, set 2 environment variables.
 
 (1) `SKETCH_USE_REMOTE_LAMBDAPROMPT=False`
 (2) `OPENAI_API_KEY=YOUR_API_KEY`
 
 ## How it works
```

### Comparing `sketch-0.3.5/pyproject.toml` & `sketch-0.4.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -13,20 +13,23 @@
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "pandas>=1.3.0",
     "datasketch>=1.5.8",
     "datasketches>=4.0.0",
     "ipython",
-    "lambdaprompt",
+    "lambdaprompt>=0.5.2",
     "packaging"
 ]
 urls = {homepage = "https://github.com/approximatelabs/sketch"}
 dynamic = ["version"]
 
+[project.optional-dependencies]
+local = ["lambdaprompt[local]"]
+all = ["sketch[local]"]
 
 [tool.setuptools_scm]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist = py38, py39, py310, py311
```

### Comparing `sketch-0.3.5/sketch/core.py` & `sketch-0.4.0/sketch/core.py`

 * *Files identical despite different names*

### Comparing `sketch-0.3.5/sketch/metrics.py` & `sketch-0.4.0/sketch/metrics.py`

 * *Files identical despite different names*

### Comparing `sketch-0.3.5/sketch/pandas_extension.py` & `sketch-0.4.0/sketch/pandas_extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,15 +177,15 @@
             text_to_copy = f"SKETCH ERROR - see print logs for full error"
     else:
         # using local version
         text_to_copy = prompt(**prompt_kwargs)
     return text_to_copy
 
 
-howto_prompt = lambdaprompt.GPT3Prompt(
+howto_prompt = lambdaprompt.Completion(
     """
 For the pandas dataframe ({{ dfname }}) the user wants code to solve a problem.
 Summary statistics and descriptive data of dataframe [`{{ dfname }}`]:
 ```
 {{ data_description }}
 ```
 The dataframe is loaded and in memory, and currently named [ {{ dfname }} ].
@@ -230,15 +230,15 @@
             how=how,
             previous_answer=code,
             previous_error=str(e),
         )
     return code
 
 
-ask_prompt = lambdaprompt.GPT3Prompt(
+ask_prompt = lambdaprompt.Completion(
     """
 For the pandas dataframe ({{ dfname }}) the user wants an answer to a question about the data.
 Summary statistics and descriptive data of dataframe [`{{ dfname }}`]:
 ```
 {{ data_description }}
 ```
 
@@ -334,15 +334,15 @@
 
     def apply(self, prompt_template_string, **kwargs):
         row_limit = int(os.environ.get("SKETCH_ROW_OVERRIDE_LIMIT", "10"))
         if len(self._obj) > row_limit:
             raise RuntimeError(
                 f"Too many rows for apply \n (SKETCH_ROW_OVERRIDE_LIMIT: {row_limit}, Actual: {len(self._obj)})"
             )
-        new_gpt3_prompt = lambdaprompt.GPT3Prompt(prompt_template_string)
+        new_gpt3_prompt = lambdaprompt.Completion(prompt_template_string)
         named_args = new_gpt3_prompt.get_named_args()
         known_args = set(self._obj.columns) | set(kwargs.keys())
         needed_args = set(named_args)
         if needed_args - known_args:
             raise RuntimeError(
                 f"Missing: {needed_args - known_args}\nKnown: {known_args}"
             )
```

### Comparing `sketch-0.3.5/sketch/references.py` & `sketch-0.4.0/sketch/references.py`

 * *Files identical despite different names*

### Comparing `sketch-0.3.5/sketch/sketches.py` & `sketch-0.4.0/sketch/sketches.py`

 * *Files identical despite different names*

### Comparing `sketch-0.3.5/sketch.egg-info/PKG-INFO` & `sketch-0.4.0/sketch.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sketch
-Version: 0.3.5
+Version: 0.4.0
 Summary: Compute, store and operate on data sketches
 License: MIT License
         
         Copyright (c) 2023 Justin Waugh, Mike Biven
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -25,29 +25,31 @@
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/approximatelabs/sketch
 Keywords: data,sketch,model,etl,automatic,join,ai,embedding,profiling
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: local
+Provides-Extra: all
 License-File: LICENSE
 
 [![](https://dcbadge.vercel.app/api/server/kW9nBQErGe?compact=true&style=flat)](https://discord.gg/kW9nBQErGe)
 
 # sketch
 
 Sketch is an AI code-writing assistant for pandas users that understands the context of your data, greatly improving the relevance of suggestions. Sketch is usable in seconds and doesn't require adding a plugin to your IDE.
 
 ```bash
 pip install sketch
 ```
 
 ## Demo 
 
-Here we follow a "standard" (hypothetical) data-analysis workflow, showing a Natural Language interace that successfully navigates many tasks in the data stack landscape. 
+Here we follow a "standard" (hypothetical) data-analysis workflow, showing a Natural Language interface that successfully navigates many tasks in the data stack landscape. 
 
 - Data Catalogging:
   - General tagging (eg. PII identification)
   - Metadata generation (names and descriptions)
 - Data Engineering:
   - Data cleaning and masking (compliance)
   - Derived feature creation and extraction
@@ -97,15 +99,22 @@
 
 ```python
 df['capitol'] = pd.DataFrame({'State': ['Colorado', 'Kansas', 'California', 'New York']}).sketch.apply("What is the capitol of [{{ State }}]?")
 ```
 
 ## Sketch currently uses `prompts.approx.dev` to help run with minimal setup
 
-In the future, we plan to update the prompts at this endpoint with our own custom foundation model, built to answer questions more accurately than GPT-3 can with its minimal data context. 
+You can also directly use a few pre-built hugging face models (right now `MPT-7B` and `StarCoder`), which will run entirely locally (once you download the model weights from HF).
+Do this by setting environment 3 variables:
+
+```python
+os.environ['LAMBDAPROMPT_BACKEND'] = 'StarCoder'
+os.environ['SKETCH_USE_REMOTE_LAMBDAPROMPT'] = 'False'
+os.environ['HF_ACCESS_TOKEN'] = 'your_hugging_face_token'
+```
 
 You can also directly call OpenAI directly (and not use our endpoint) by using your own API key. To do this, set 2 environment variables.
 
 (1) `SKETCH_USE_REMOTE_LAMBDAPROMPT=False`
 (2) `OPENAI_API_KEY=YOUR_API_KEY`
 
 ## How it works
```

### Comparing `sketch-0.3.5/tests/test_pandas_extension.py` & `sketch-0.4.0/tests/test_pandas_extension.py`

 * *Files identical despite different names*


# Comparing `tmp/languagemodels-0.0.2.tar.gz` & `tmp/languagemodels-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "languagemodels-0.0.2.tar", last modified: Thu May 11 23:45:36 2023, max compression
+gzip compressed data, was "languagemodels-0.0.3.tar", last modified: Fri May 12 16:19:36 2023, max compression
```

## Comparing `languagemodels-0.0.2.tar` & `languagemodels-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-05-11 23:45:36.584200 languagemodels-0.0.2/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     3014 2023-05-11 23:45:36.584200 languagemodels-0.0.2/PKG-INFO
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-05-11 23:45:36.580199 languagemodels-0.0.2/languagemodels/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     4469 2023-05-11 23:45:12.000000 languagemodels-0.0.2/languagemodels/__init__.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     2265 2023-05-09 19:09:44.000000 languagemodels-0.0.2/languagemodels/embeddings.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     1908 2023-05-11 23:45:12.000000 languagemodels-0.0.2/languagemodels/inference.py
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-05-11 23:45:36.584200 languagemodels-0.0.2/languagemodels.egg-info/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     3014 2023-05-11 23:45:36.000000 languagemodels-0.0.2/languagemodels.egg-info/PKG-INFO
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      281 2023-05-11 23:45:36.000000 languagemodels-0.0.2/languagemodels.egg-info/SOURCES.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-05-11 23:45:36.000000 languagemodels-0.0.2/languagemodels.egg-info/dependency_links.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       52 2023-05-11 23:45:36.000000 languagemodels-0.0.2/languagemodels.egg-info/requires.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-05-11 23:45:36.000000 languagemodels-0.0.2/languagemodels.egg-info/top_level.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-05-11 23:45:36.584200 languagemodels-0.0.2/setup.cfg
--rw-r--r--   0 jncraton  (1000) jncraton  (1000)      788 2023-05-11 23:45:20.000000 languagemodels-0.0.2/setup.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-05-12 16:19:36.207180 languagemodels-0.0.3/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     3537 2023-05-12 16:19:36.207180 languagemodels-0.0.3/PKG-INFO
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-05-12 16:19:36.203180 languagemodels-0.0.3/languagemodels/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     6099 2023-05-12 14:02:41.000000 languagemodels-0.0.3/languagemodels/__init__.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     2265 2023-05-09 19:09:44.000000 languagemodels-0.0.3/languagemodels/embeddings.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     1910 2023-05-12 13:21:50.000000 languagemodels-0.0.3/languagemodels/inference.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-05-12 16:19:36.207180 languagemodels-0.0.3/languagemodels.egg-info/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     3537 2023-05-12 16:19:35.000000 languagemodels-0.0.3/languagemodels.egg-info/PKG-INFO
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      281 2023-05-12 16:19:35.000000 languagemodels-0.0.3/languagemodels.egg-info/SOURCES.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-05-12 16:19:35.000000 languagemodels-0.0.3/languagemodels.egg-info/dependency_links.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       52 2023-05-12 16:19:35.000000 languagemodels-0.0.3/languagemodels.egg-info/requires.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-05-12 16:19:35.000000 languagemodels-0.0.3/languagemodels.egg-info/top_level.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-05-12 16:19:36.207180 languagemodels-0.0.3/setup.cfg
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      788 2023-05-12 16:19:16.000000 languagemodels-0.0.3/setup.py
```

### Comparing `languagemodels-0.0.2/PKG-INFO` & `languagemodels-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
         
+        [![PyPI version](https://badge.fury.io/py/languagemodels.svg)](https://badge.fury.io/py/languagemodels)
         [![docs](https://img.shields.io/badge/docs-online-brightgreen)](https://languagemodels.netlify.app/)
         [![Build](https://github.com/jncraton/languagemodels/actions/workflows/build.yml/badge.svg)](https://github.com/jncraton/languagemodels/actions/workflows/build.yml)
         [![Netlify Status](https://api.netlify.com/api/v1/badges/722e625a-c6bc-4373-bd88-c017adc58c00/deploy-status)](https://app.netlify.com/sites/languagemodels/deploys)
         
-        Simple building blocks for exploring large language models.
+        `languagemodels` is a Python package providing simple building blocks for exploring natural language processing.
+        
+        ![Translation hello world example](media/hello.gif)
         
         Installation
         ------------
         
         This package can be installed using the following command:
         
         ```sh
@@ -82,14 +85,26 @@
         ### External Retrieval
         
         ```python
         >>> import languagemodels as lm
         
         >>> lm.fetch_wiki('Chemistry')
         'Chemistry is the scientific study...
+        
+        >>> lm.fetch_weather(41.8, -87.6)
+        'Partly cloudy with a chance of rain...
+        ```
+        
+        ### Misc Text Tools
+        
+        ```python
+        >>> import languagemodels as lm
+        
+        >>> get_date()
+        'Friday, May 12, 2023 at 09:27AM'
         ```
         
         [Full documentation](https://languagemodels.netlify.app/)
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `languagemodels-0.0.2/languagemodels/__init__.py` & `languagemodels-0.0.3/languagemodels/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,43 @@
 import requests
+import datetime
 import json
 
 from languagemodels.inference import generate_instruct, get_pipeline
 from languagemodels.embeddings import RetrievalContext
 
 docs = RetrievalContext()
 
 
+def complete(prompt: str) -> str:
+    """Provide one completion for a given open-ended prompt
+
+    :param prompt: Prompt to use as input to the model
+    :return: Completion returned from the language model
+
+    Examples:
+
+    >>> complete("Luke thought that he") #doctest: +SKIP
+    'was going to be a doctor.'
+
+    >>> complete("There are many mythical creatures who") #doctest: +SKIP
+    'are able to fly'
+
+    >>> complete("She hid in her room until") #doctest: +SKIP
+    'she was sure she was safe'
+    """
+    return generate_instruct(prompt, max_tokens=200, temperature=0.7)
+
+
 def do(prompt: str) -> str:
     """Follow a single-turn instructional prompt
 
+    :param prompt: Instructional prompt to follow
+    :return: Completion returned from the language model
+
     Examples:
 
     >>> do("Translate to Spanish: Hello, world!")
     'Hola, mundo!'
 
     >>> do("Pick the sport: baseball, texas, chemistry")
     'baseball'
@@ -23,29 +47,64 @@
 
     >>> do("Does this make sense: The course is jumping well.")
     'no'
     """
     return generate_instruct(prompt, max_tokens=200)
 
 
-def complete(prompt: str) -> str:
-    """Provide one completion for a given open-ended prompt
+def extract_answer(question: str, context: str) -> str:
+    """Extract an answer to a `question` from a provided `context`
 
-    Examples:
+    The returned answer will always be a substring extracted from `context`.
+    It may not always be a correct or meaningful answer, but it will never be
+    an arbitrary hallucination.
 
-    >>> complete("Luke thought that he") #doctest: +SKIP
-    'was going to be a doctor.'
+    :param question: A question to answer using knowledge from context
+    :param context: Knowledge used to answer the question
+    :return: Answer to the question.
 
-    >>> complete("There are many mythical creatures who") #doctest: +SKIP
-    'are able to fly'
+    >>> extract_answer("What color is the ball?", "There is a green ball and a red box")
+    'green'
+    >>> extract_answer("Who created Python?", fetch_wiki('Python'))
+    'Guido van Rossum'
+    """
 
-    >>> complete("She hid in her room until") #doctest: +SKIP
-    'she was sure she was safe'
+    qa = get_pipeline("question-answering", "distilbert-base-cased-distilled-squad")
+
+    return qa(question, context)["answer"]
+
+
+def classify(doc: str, label1: str, label2: str) -> str:
+    """Performs binary classification on an input
+
+    :param doc: A plain text input document to classify
+    :param label1: The first label to classify against
+    :param label2: The second label to classify against
+    :return: The closest matching class. The return value will always be
+    `label1` or `label2`
+
+    >>> classify("I love you!","positive","negative")
+    'positive'
+    >>> classify("That book was fine.","positive","negative")
+    'positive'
+    >>> classify("That movie was terrible.","positive","negative")
+    'negative'
+    >>> classify("The submarine is diving", "ocean", "space")
+    'ocean'
     """
-    return generate_instruct(prompt, max_tokens=200, temperature=0.7)
+
+    classifier = get_pipeline(
+        "zero-shot-classification", "valhalla/distilbart-mnli-12-1"
+    )
+
+    result = classifier(doc, [label1, label2])
+
+    top = max(zip(result["scores"], result["labels"]), key=lambda r: r[0])
+
+    return top[1]
 
 
 def store_doc(doc: str) -> None:
     """Store document for later retrieval
 
     :param doc: A plain text document to store.
 
@@ -55,14 +114,17 @@
 
 
 def search_docs(query: str) -> str:
     """Search stored documents
 
     A single document that best matches `query` will be returned.
 
+    :param prompt: Query to compare to stored documents
+    :return: Content of the closest matching document
+
     >>> store_doc("The sky is blue.")
     >>> store_doc("Paris is in France.")
     >>> search_docs("Where is Paris?")
     'Paris is in France.'
     """
     return docs.get_match(query)
 
@@ -70,14 +132,17 @@
 def fetch_wiki(topic: str) -> str:
     """
     Return Wikipedia summary for a topic
 
     This function ignores the complexity of disambiguation pages and simply
     returns the first result that is not a disambiguation page
 
+    :param topic: Topic to search for on Wikipedia
+    :return: Text content of the lead section of the most popular matching article
+
     >>> fetch_wiki('Python') # doctest: +ELLIPSIS
     'Python is a high-level...
 
     >>> fetch_wiki('Chemistry') # doctest: +ELLIPSIS
     'Chemistry is the scientific study...
     """
 
@@ -97,57 +162,42 @@
 
         summary = first["extract"]
         return summary
     else:
         return "No matching wiki page found."
 
 
-def extract_answer(question: str, context: str) -> str:
-    """Extract an answer to a `question` from a provided `context`
+def fetch_weather(latitude, longitude):
+    """Fetch the current weather for a supplied longitude and latitude
 
-    The returned answer will always be a substring extracted from `context`.
-    It may not always be a correct or meaningful answer, but it will never be
-    an arbitrary hallucination.
+    Weather is provided by the US government and this function only supports
+    locations in the United States.
 
-    :param question: A question to answer using knowledge from context
-    :param context: Knowledge used to answer the question
-    :return: Answer to the question.
+    :param latitude: Latitude value representing this location
+    :param longitude: Longitude value representing this location
+    :return: Plain text description of the current weather forecast
 
-    >>> extract_answer("What color is the ball?", "There is a green ball and a red box")
-    'green'
-    >>> extract_answer("Who created Python?", fetch_wiki('Python'))
-    'Guido van Rossum'
+    >>> fetch_weather(41.8, -87.6) # doctest: +SKIP
+    'Scattered showers and thunderstorms before 1pm with a high of 73.'
     """
 
-    qa = get_pipeline("question-answering", "distilbert-base-cased-distilled-squad")
+    res = requests.get(f"https://api.weather.gov/points/{latitude},{longitude}")
+    points = json.loads(res.text)
+    forecast_url = points["properties"]["forecast"]
 
-    return qa(question, context)["answer"]
+    res = requests.get(forecast_url)
+    forecast = json.loads(res.text)
+    current = forecast["properties"]["periods"][0]
 
+    return current["detailedForecast"]
 
-def classify(doc: str, label1: str, label2: str) -> str:
-    """Performs binary classification on an input
 
-    :param doc: A plain text input document to classify
-    :param label1: The first label to classify against
-    :param label2: The second label to classify against
-    :return: The closest matching class. The return value will always be
-    `label1` or `label2`
+def get_date() -> str:
+    """Returns the current date and time in natural language
 
-    >>> classify("I love you!","positive","negative")
-    'positive'
-    >>> classify("That book was fine.","positive","negative")
-    'positive'
-    >>> classify("That movie was terrible.","positive","negative")
-    'negative'
-    >>> classify("The submarine is diving", "ocean", "space")
-    'ocean'
+    >>> get_date() # doctest: +SKIP
+    'Friday, May 12, 2023 at 09:27AM'
     """
 
-    classifier = get_pipeline(
-        "zero-shot-classification", "valhalla/distilbart-mnli-12-1"
-    )
-
-    result = classifier(doc, [label1, label2])
+    now = datetime.datetime.now()
 
-    top = max(zip(result["scores"], result["labels"]), key=lambda r: r[0])
-
-    return top[1]
+    return now.strftime("%A, %B %d, %Y at %I:%M%p")
```

### Comparing `languagemodels-0.0.2/languagemodels/embeddings.py` & `languagemodels-0.0.3/languagemodels/embeddings.py`

 * *Files identical despite different names*

### Comparing `languagemodels-0.0.2/languagemodels/inference.py` & `languagemodels-0.0.3/languagemodels/inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,30 +29,30 @@
     resp = response.json()
     if "text" in resp:
         return resp["text"]
     else:
         raise InferenceException(f"TextSynth error: {resp}")
 
 
-def generate_instruct(prompt, max_tokens=200, temperature=.1, repetition_penalty=1.2):
+def generate_instruct(prompt, max_tokens=200, temperature=0.1, repetition_penalty=1.2):
     """Generates one completion for a prompt using an instruction-tuned model
 
     This may use a local model, or it may make an API call to an external
     model if API keys are available.
     """
     if os.environ.get("ts_key") or os.environ.get("ts_server"):
         return generate_ts("flan_t5_xxl_q4", prompt, max_tokens)
 
     generate = get_pipeline("text2text-generation", "google/flan-t5-large")
 
     return generate(
         prompt,
         repetition_penalty=repetition_penalty,
         temperature=temperature,
-        do_sample=temperature > .1,
+        do_sample=temperature > 0.1,
     )[0]["generated_text"]
 
 
 def get_pipeline(task, model):
     """Gets a pipeline instance
 
     This is thin wrapper around the pipeline constructor to provide caching
```

### Comparing `languagemodels-0.0.2/languagemodels.egg-info/PKG-INFO` & `languagemodels-0.0.3/languagemodels.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
         
+        [![PyPI version](https://badge.fury.io/py/languagemodels.svg)](https://badge.fury.io/py/languagemodels)
         [![docs](https://img.shields.io/badge/docs-online-brightgreen)](https://languagemodels.netlify.app/)
         [![Build](https://github.com/jncraton/languagemodels/actions/workflows/build.yml/badge.svg)](https://github.com/jncraton/languagemodels/actions/workflows/build.yml)
         [![Netlify Status](https://api.netlify.com/api/v1/badges/722e625a-c6bc-4373-bd88-c017adc58c00/deploy-status)](https://app.netlify.com/sites/languagemodels/deploys)
         
-        Simple building blocks for exploring large language models.
+        `languagemodels` is a Python package providing simple building blocks for exploring natural language processing.
+        
+        ![Translation hello world example](media/hello.gif)
         
         Installation
         ------------
         
         This package can be installed using the following command:
         
         ```sh
@@ -82,14 +85,26 @@
         ### External Retrieval
         
         ```python
         >>> import languagemodels as lm
         
         >>> lm.fetch_wiki('Chemistry')
         'Chemistry is the scientific study...
+        
+        >>> lm.fetch_weather(41.8, -87.6)
+        'Partly cloudy with a chance of rain...
+        ```
+        
+        ### Misc Text Tools
+        
+        ```python
+        >>> import languagemodels as lm
+        
+        >>> get_date()
+        'Friday, May 12, 2023 at 09:27AM'
         ```
         
         [Full documentation](https://languagemodels.netlify.app/)
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `languagemodels-0.0.2/setup.py` & `languagemodels-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="languagemodels",
-    version="0.0.2",
+    version="0.0.3",
     author="Jon Craton",
     author_email="jon@joncraton.com",
     description="Simple inference for large language models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jncraton/languagemodels",
     packages=setuptools.find_packages(),
```


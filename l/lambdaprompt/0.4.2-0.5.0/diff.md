# Comparing `tmp/lambdaprompt-0.4.2.tar.gz` & `tmp/lambdaprompt-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/lambdaprompt/lambdaprompt/dist/.tmp-0bz5gawl/lambdaprompt-0.4.2.tar", last modified: Thu Mar 23 03:36:29 2023, max compression
+gzip compressed data, was "/home/runner/work/lambdaprompt/lambdaprompt/dist/.tmp-9qyhp1d_/lambdaprompt-0.5.0.tar", last modified: Fri May 12 09:56:48 2023, max compression
```

## Comparing `lambdaprompt-0.4.2.tar` & `lambdaprompt-0.5.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:36:29.000000 lambdaprompt-0.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:36:29.000000 lambdaprompt-0.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:36:29.000000 lambdaprompt-0.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-03-23 03:36:18.000000 lambdaprompt-0.4.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-03-23 03:36:18.000000 lambdaprompt-0.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-23 03:36:18.000000 lambdaprompt-0.4.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-23 03:36:18.000000 lambdaprompt-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-03-23 03:36:29.000000 lambdaprompt-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-03-23 03:36:18.000000 lambdaprompt-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-23 03:36:18.000000 lambdaprompt-0.4.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:36:29.000000 lambdaprompt-0.4.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-23 03:36:18.000000 lambdaprompt-0.4.2/examples/one.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-03-23 03:36:18.000000 lambdaprompt-0.4.2/examples/two.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:36:29.000000 lambdaprompt-0.4.2/lambdaprompt/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-03-23 03:36:18.000000 lambdaprompt-0.4.2/lambdaprompt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-23 03:36:18.000000 lambdaprompt-0.4.2/lambdaprompt/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:36:29.000000 lambdaprompt-0.4.2/lambdaprompt/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 03:36:18.000000 lambdaprompt-0.4.2/lambdaprompt/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-23 03:36:18.000000 lambdaprompt-0.4.2/lambdaprompt/examples/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-03-23 03:36:18.000000 lambdaprompt-0.4.2/lambdaprompt/gpt3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-03-23 03:36:18.000000 lambdaprompt-0.4.2/lambdaprompt/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:36:29.000000 lambdaprompt-0.4.2/lambdaprompt/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 03:36:18.000000 lambdaprompt-0.4.2/lambdaprompt/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-03-23 03:36:18.000000 lambdaprompt-0.4.2/lambdaprompt/server/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-03-23 03:36:18.000000 lambdaprompt-0.4.2/lambdaprompt/server/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:36:29.000000 lambdaprompt-0.4.2/lambdaprompt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-03-23 03:36:29.000000 lambdaprompt-0.4.2/lambdaprompt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-23 03:36:29.000000 lambdaprompt-0.4.2/lambdaprompt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 03:36:29.000000 lambdaprompt-0.4.2/lambdaprompt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-23 03:36:29.000000 lambdaprompt-0.4.2/lambdaprompt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-23 03:36:29.000000 lambdaprompt-0.4.2/lambdaprompt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-23 03:36:18.000000 lambdaprompt-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 03:36:29.000000 lambdaprompt-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 03:36:18.000000 lambdaprompt-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:36:29.000000 lambdaprompt-0.4.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 03:36:29.000000 lambdaprompt-0.4.2/tests/library/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-23 03:36:18.000000 lambdaprompt-0.4.2/tests/library/serverexamples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-03-23 03:36:18.000000 lambdaprompt-0.4.2/tests/test_gpt3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-03-23 03:36:18.000000 lambdaprompt-0.4.2/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-03-23 03:36:18.000000 lambdaprompt-0.4.2/tests/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:48.000000 lambdaprompt-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:48.000000 lambdaprompt-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:48.000000 lambdaprompt-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-12 09:56:36.000000 lambdaprompt-0.5.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-12 09:56:36.000000 lambdaprompt-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-12 09:56:36.000000 lambdaprompt-0.5.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-12 09:56:36.000000 lambdaprompt-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-12 09:56:48.000000 lambdaprompt-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-12 09:56:36.000000 lambdaprompt-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-12 09:56:36.000000 lambdaprompt-0.5.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:48.000000 lambdaprompt-0.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-12 09:56:36.000000 lambdaprompt-0.5.0/examples/one.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-12 09:56:36.000000 lambdaprompt-0.5.0/examples/two.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:48.000000 lambdaprompt-0.5.0/lambdaprompt/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-12 09:56:36.000000 lambdaprompt-0.5.0/lambdaprompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-05-12 09:56:36.000000 lambdaprompt-0.5.0/lambdaprompt/backends.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:48.000000 lambdaprompt-0.5.0/lambdaprompt/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:36.000000 lambdaprompt-0.5.0/lambdaprompt/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-12 09:56:36.000000 lambdaprompt-0.5.0/lambdaprompt/examples/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-12 09:56:36.000000 lambdaprompt-0.5.0/lambdaprompt/gpt3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-05-12 09:56:36.000000 lambdaprompt-0.5.0/lambdaprompt/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:48.000000 lambdaprompt-0.5.0/lambdaprompt/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:36.000000 lambdaprompt-0.5.0/lambdaprompt/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-12 09:56:36.000000 lambdaprompt-0.5.0/lambdaprompt/server/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-12 09:56:36.000000 lambdaprompt-0.5.0/lambdaprompt/server/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:48.000000 lambdaprompt-0.5.0/lambdaprompt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-12 09:56:48.000000 lambdaprompt-0.5.0/lambdaprompt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-12 09:56:48.000000 lambdaprompt-0.5.0/lambdaprompt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 09:56:48.000000 lambdaprompt-0.5.0/lambdaprompt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 09:56:48.000000 lambdaprompt-0.5.0/lambdaprompt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-12 09:56:48.000000 lambdaprompt-0.5.0/lambdaprompt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-12 09:56:36.000000 lambdaprompt-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 09:56:48.000000 lambdaprompt-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 09:56:36.000000 lambdaprompt-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:48.000000 lambdaprompt-0.5.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:48.000000 lambdaprompt-0.5.0/tests/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-12 09:56:36.000000 lambdaprompt-0.5.0/tests/library/serverexamples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-12 09:56:36.000000 lambdaprompt-0.5.0/tests/test_gpt3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-12 09:56:36.000000 lambdaprompt-0.5.0/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-12 09:56:36.000000 lambdaprompt-0.5.0/tests/test_server.py
```

### Comparing `lambdaprompt-0.4.2/.github/workflows/publish-to-pypi.yml` & `lambdaprompt-0.5.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.4.2/.gitignore` & `lambdaprompt-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.4.2/LICENSE` & `lambdaprompt-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.4.2/PKG-INFO` & `lambdaprompt-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: lambdaprompt
-Version: 0.4.2
+Version: 0.5.0
 Summary: A functional programming interface for building AI systems
 License: MIT
 Project-URL: homepage, https://github.com/approximatelabs/lambdaprompt
 Keywords: nlp,ai,functional,composition,prompt,apply,chain,machine
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: server
+Provides-Extra: local
 Provides-Extra: all
 License-File: LICENSE
 
 [![](https://dcbadge.vercel.app/api/server/kW9nBQErGe?compact=true&style=flat)](https://discord.gg/kW9nBQErGe)
 
 # λprompt - Build, compose and call templated LLM prompts!
```

### Comparing `lambdaprompt-0.4.2/README.md` & `lambdaprompt-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.4.2/lambdaprompt/server/data.py` & `lambdaprompt-0.5.0/lambdaprompt/server/data.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.4.2/lambdaprompt/server/main.py` & `lambdaprompt-0.5.0/lambdaprompt/server/main.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.4.2/lambdaprompt.egg-info/PKG-INFO` & `lambdaprompt-0.5.0/lambdaprompt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: lambdaprompt
-Version: 0.4.2
+Version: 0.5.0
 Summary: A functional programming interface for building AI systems
 License: MIT
 Project-URL: homepage, https://github.com/approximatelabs/lambdaprompt
 Keywords: nlp,ai,functional,composition,prompt,apply,chain,machine
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: server
+Provides-Extra: local
 Provides-Extra: all
 License-File: LICENSE
 
 [![](https://dcbadge.vercel.app/api/server/kW9nBQErGe?compact=true&style=flat)](https://discord.gg/kW9nBQErGe)
 
 # λprompt - Build, compose and call templated LLM prompts!
```

### Comparing `lambdaprompt-0.4.2/lambdaprompt.egg-info/SOURCES.txt` & `lambdaprompt-0.5.0/lambdaprompt.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 dev-requirements.txt
 pyproject.toml
 setup.py
 .github/workflows/publish-to-pypi.yml
 examples/one.py
 examples/two.py
 lambdaprompt/__init__.py
-lambdaprompt/config.py
+lambdaprompt/backends.py
 lambdaprompt/gpt3.py
 lambdaprompt/prompt.py
 lambdaprompt.egg-info/PKG-INFO
 lambdaprompt.egg-info/SOURCES.txt
 lambdaprompt.egg-info/dependency_links.txt
 lambdaprompt.egg-info/requires.txt
 lambdaprompt.egg-info/top_level.txt
```

### Comparing `lambdaprompt-0.4.2/pyproject.toml` & `lambdaprompt-0.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -9,22 +9,23 @@
 requires-python = ">=3.7"
 keywords = ["nlp", "ai", "functional", "composition", "prompt", "apply", "chain", "machine"]
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
-    "requests", "aiohttp", "python-dotenv", "jinja2", "nest_asyncio", "pyyaml"
+    "requests", "aiohttp", "python-dotenv", "jinja2", "nest_asyncio", "pyyaml", "tenacity"
 ]
 urls = {homepage = "https://github.com/approximatelabs/lambdaprompt"}
 dynamic = ["version"]
 
 [project.optional-dependencies]
 server = ["fastapi", "uvicorn", "aiosqlite"]
-all = ["lambdaprompt[server]"]
+local = ["transformers"]
+all = ["lambdaprompt[server,local]"]
 
 [tool.setuptools_scm]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist = py37, py38, py39, py310, py311
```

### Comparing `lambdaprompt-0.4.2/tests/test_gpt3.py` & `lambdaprompt-0.5.0/tests/test_gpt3.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,27 +2,22 @@
 
 import pytest
 from aioresponses import aioresponses
 
 from lambdaprompt import AsyncGPT3Prompt, GPT3Prompt, prompt, register_call_callback
 
 
-@pytest.fixture(autouse=True)
-def ignore_load_dotenv(mocker):
-    mocker.patch("lambdaprompt.config.load_dotenv", return_value=None)
-
-
 def test_api_key_needed():
     with aioresponses() as m:
         m.post(
             "https://api.openai.com/v1/completions",
             payload={"choices": [{"text": "Wow!"}]},
         )
-        prompt = GPT3Prompt("test {{ hello }}")
         with pytest.raises(Exception):
+            prompt = GPT3Prompt("test {{ hello }}")
             prompt(hello="world")
 
 
 def test_gpt3_prompt_returns(mocker):
     mocker.patch.dict("os.environ", {"OPENAI_API_KEY": "TEST"})
     with aioresponses() as m:
         m.post(
```

### Comparing `lambdaprompt-0.4.2/tests/test_prompt.py` & `lambdaprompt-0.5.0/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.4.2/tests/test_server.py` & `lambdaprompt-0.5.0/tests/test_server.py`

 * *Files identical despite different names*


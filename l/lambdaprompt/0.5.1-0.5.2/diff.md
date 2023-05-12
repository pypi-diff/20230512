# Comparing `tmp/lambdaprompt-0.5.1.tar.gz` & `tmp/lambdaprompt-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/lambdaprompt/lambdaprompt/dist/.tmp-u_fx43ut/lambdaprompt-0.5.1.tar", last modified: Fri May 12 11:06:14 2023, max compression
+gzip compressed data, was "/home/runner/work/lambdaprompt/lambdaprompt/dist/.tmp-z5zihc3q/lambdaprompt-0.5.2.tar", last modified: Fri May 12 11:21:58 2023, max compression
```

## Comparing `lambdaprompt-0.5.1.tar` & `lambdaprompt-0.5.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:06:14.000000 lambdaprompt-0.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:06:14.000000 lambdaprompt-0.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:06:14.000000 lambdaprompt-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-12 11:06:04.000000 lambdaprompt-0.5.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-12 11:06:04.000000 lambdaprompt-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-12 11:06:04.000000 lambdaprompt-0.5.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-12 11:06:04.000000 lambdaprompt-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-12 11:06:14.000000 lambdaprompt-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-12 11:06:04.000000 lambdaprompt-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-12 11:06:04.000000 lambdaprompt-0.5.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:06:14.000000 lambdaprompt-0.5.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-12 11:06:04.000000 lambdaprompt-0.5.1/examples/one.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-12 11:06:04.000000 lambdaprompt-0.5.1/examples/two.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:06:14.000000 lambdaprompt-0.5.1/lambdaprompt/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-12 11:06:04.000000 lambdaprompt-0.5.1/lambdaprompt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-05-12 11:06:04.000000 lambdaprompt-0.5.1/lambdaprompt/backends.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:06:14.000000 lambdaprompt-0.5.1/lambdaprompt/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:06:04.000000 lambdaprompt-0.5.1/lambdaprompt/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-12 11:06:04.000000 lambdaprompt-0.5.1/lambdaprompt/examples/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-12 11:06:04.000000 lambdaprompt-0.5.1/lambdaprompt/gpt3.py
--rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-05-12 11:06:04.000000 lambdaprompt-0.5.1/lambdaprompt/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:06:14.000000 lambdaprompt-0.5.1/lambdaprompt/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:06:04.000000 lambdaprompt-0.5.1/lambdaprompt/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-12 11:06:04.000000 lambdaprompt-0.5.1/lambdaprompt/server/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-12 11:06:04.000000 lambdaprompt-0.5.1/lambdaprompt/server/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:06:14.000000 lambdaprompt-0.5.1/lambdaprompt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-12 11:06:14.000000 lambdaprompt-0.5.1/lambdaprompt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-12 11:06:14.000000 lambdaprompt-0.5.1/lambdaprompt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 11:06:14.000000 lambdaprompt-0.5.1/lambdaprompt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 11:06:14.000000 lambdaprompt-0.5.1/lambdaprompt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-12 11:06:14.000000 lambdaprompt-0.5.1/lambdaprompt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-12 11:06:04.000000 lambdaprompt-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 11:06:14.000000 lambdaprompt-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 11:06:04.000000 lambdaprompt-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:06:14.000000 lambdaprompt-0.5.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:06:14.000000 lambdaprompt-0.5.1/tests/library/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-12 11:06:04.000000 lambdaprompt-0.5.1/tests/library/serverexamples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-12 11:06:04.000000 lambdaprompt-0.5.1/tests/test_gpt3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-12 11:06:04.000000 lambdaprompt-0.5.1/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-12 11:06:04.000000 lambdaprompt-0.5.1/tests/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/examples/one.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/examples/two.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/lambdaprompt/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/lambdaprompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/lambdaprompt/backends.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/lambdaprompt/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/lambdaprompt/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/lambdaprompt/examples/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/lambdaprompt/gpt3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/lambdaprompt/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/lambdaprompt/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/lambdaprompt/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/lambdaprompt/server/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/lambdaprompt/server/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/lambdaprompt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/lambdaprompt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/lambdaprompt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/lambdaprompt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/lambdaprompt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/lambdaprompt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/tests/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/tests/library/serverexamples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/tests/test_gpt3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/tests/test_server.py
```

### Comparing `lambdaprompt-0.5.1/.github/workflows/publish-to-pypi.yml` & `lambdaprompt-0.5.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.1/.gitignore` & `lambdaprompt-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.1/LICENSE` & `lambdaprompt-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.1/PKG-INFO` & `lambdaprompt-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambdaprompt
-Version: 0.5.1
+Version: 0.5.2
 Summary: A functional programming interface for building AI systems
 License: MIT
 Project-URL: homepage, https://github.com/approximatelabs/lambdaprompt
 Keywords: nlp,ai,functional,composition,prompt,apply,chain,machine
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `lambdaprompt-0.5.1/README.md` & `lambdaprompt-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.1/lambdaprompt/__init__.py` & `lambdaprompt-0.5.2/lambdaprompt/__init__.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.1/lambdaprompt/backends.py` & `lambdaprompt-0.5.2/lambdaprompt/backends.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.1/lambdaprompt/gpt3.py` & `lambdaprompt-0.5.2/lambdaprompt/gpt3.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.1/lambdaprompt/prompt.py` & `lambdaprompt-0.5.2/lambdaprompt/prompt.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.1/lambdaprompt/server/data.py` & `lambdaprompt-0.5.2/lambdaprompt/server/data.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.1/lambdaprompt/server/main.py` & `lambdaprompt-0.5.2/lambdaprompt/server/main.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.1/lambdaprompt.egg-info/PKG-INFO` & `lambdaprompt-0.5.2/lambdaprompt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambdaprompt
-Version: 0.5.1
+Version: 0.5.2
 Summary: A functional programming interface for building AI systems
 License: MIT
 Project-URL: homepage, https://github.com/approximatelabs/lambdaprompt
 Keywords: nlp,ai,functional,composition,prompt,apply,chain,machine
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `lambdaprompt-0.5.1/lambdaprompt.egg-info/SOURCES.txt` & `lambdaprompt-0.5.2/lambdaprompt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.1/pyproject.toml` & `lambdaprompt-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 requires-python = ">=3.7"
 keywords = ["nlp", "ai", "functional", "composition", "prompt", "apply", "chain", "machine"]
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
-    "requests", "aiohttp", "python-dotenv", "jinja2", "nest_asyncio", "pyyaml", "tenacity"
+    "requests", "aiohttp", "python-dotenv", "jinja2", "nest_asyncio", "pyyaml", "tenacity", "pydantic"
 ]
 urls = {homepage = "https://github.com/approximatelabs/lambdaprompt"}
 dynamic = ["version"]
 
 [project.optional-dependencies]
 server = ["fastapi", "uvicorn", "aiosqlite"]
 local = ["transformers"]
```

### Comparing `lambdaprompt-0.5.1/tests/test_gpt3.py` & `lambdaprompt-0.5.2/tests/test_gpt3.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.1/tests/test_prompt.py` & `lambdaprompt-0.5.2/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.1/tests/test_server.py` & `lambdaprompt-0.5.2/tests/test_server.py`

 * *Files identical despite different names*


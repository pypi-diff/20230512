# Comparing `tmp/simple_chatgpt_cli-0.1.4.tar.gz` & `tmp/simple_chatgpt_cli-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_chatgpt_cli-0.1.4.tar", max compression
+gzip compressed data, was "simple_chatgpt_cli-0.1.5.tar", max compression
```

## Comparing `simple_chatgpt_cli-0.1.4.tar` & `simple_chatgpt_cli-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      901 2023-05-12 21:01:56.967474 simple_chatgpt_cli-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-05-12 12:32:57.857467 simple_chatgpt_cli-0.1.4/chatgpt_cli/__init__.py
--rw-r--r--   0        0        0     6444 2023-05-12 21:01:15.393834 simple_chatgpt_cli-0.1.4/chatgpt_cli/main.py
--rw-r--r--   0        0        0      701 2023-05-12 21:02:03.370348 simple_chatgpt_cli-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1347 1970-01-01 00:00:00.000000 simple_chatgpt_cli-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1321 2023-05-12 21:16:48.898764 simple_chatgpt_cli-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-12 12:32:57.857467 simple_chatgpt_cli-0.1.5/chatgpt_cli/__init__.py
+-rw-r--r--   0        0        0     6444 2023-05-12 21:01:15.393834 simple_chatgpt_cli-0.1.5/chatgpt_cli/main.py
+-rw-r--r--   0        0        0      701 2023-05-12 21:17:17.303436 simple_chatgpt_cli-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1767 1970-01-01 00:00:00.000000 simple_chatgpt_cli-0.1.5/PKG-INFO
```

### Comparing `simple_chatgpt_cli-0.1.4/chatgpt_cli/main.py` & `simple_chatgpt_cli-0.1.5/chatgpt_cli/main.py`

 * *Files identical despite different names*

### Comparing `simple_chatgpt_cli-0.1.4/pyproject.toml` & `simple_chatgpt_cli-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 wrap-descriptions = 88
 
 [tool.poetry.scripts]
 chatgpt = 'chatgpt_cli.main:run'
 
 [tool.poetry]
 name = "simple-chatgpt-cli"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["tailaiw <29800495+tailaiw@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "chatgpt_cli" }]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
```

### Comparing `simple_chatgpt_cli-0.1.4/PKG-INFO` & `simple_chatgpt_cli-0.1.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: simple-chatgpt-cli
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: tailaiw
 Author-email: 29800495+tailaiw@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=0.27.6,<0.28.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Description-Content-Type: text/markdown
 
 # Simple-ChatGPT-CLI
 
-A simple implementation of ChatGPT in terminal, so I can avoid using the ChatGPT website which is more expensive and less privacy-friendly.
+I believe many others have implement more sophisticated ChatGPT CLI tool. But this is a super simple one without fancy features that I created with Python for my own use case.
+My motivation was that using OpenAI API could be much cheaper than subscribing ChatGPT Plus, and is claimed to be more privacy friendly by some legal experts.
+
+I'm not planning adding fancy features unless I start to feel some feature would be a big plus to my productivity in my own use case. But everyone are welcomed to use this basic version or fork it to add their own features.
 
 ## Installation
 
 ```bash
 pip install simple-chatgpt-cli
 ```
```


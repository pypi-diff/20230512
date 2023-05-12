# Comparing `tmp/simple_chatgpt_cli-0.1.2.tar.gz` & `tmp/simple_chatgpt_cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_chatgpt_cli-0.1.2.tar", max compression
+gzip compressed data, was "simple_chatgpt_cli-0.1.3.tar", max compression
```

## Comparing `simple_chatgpt_cli-0.1.2.tar` & `simple_chatgpt_cli-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      889 2023-05-12 20:25:15.554984 simple_chatgpt_cli-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-12 12:32:57.857467 simple_chatgpt_cli-0.1.2/chatgpt_cli/__init__.py
--rw-r--r--   0        0        0     6293 2023-05-12 20:49:33.212605 simple_chatgpt_cli-0.1.2/chatgpt_cli/main.py
--rw-r--r--   0        0        0      701 2023-05-12 20:37:58.185435 simple_chatgpt_cli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1335 1970-01-01 00:00:00.000000 simple_chatgpt_cli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      880 2023-05-12 20:54:50.644831 simple_chatgpt_cli-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-12 12:32:57.857467 simple_chatgpt_cli-0.1.3/chatgpt_cli/__init__.py
+-rw-r--r--   0        0        0     6293 2023-05-12 20:51:38.053032 simple_chatgpt_cli-0.1.3/chatgpt_cli/main.py
+-rw-r--r--   0        0        0      701 2023-05-12 20:52:31.313668 simple_chatgpt_cli-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 simple_chatgpt_cli-0.1.3/PKG-INFO
```

### Comparing `simple_chatgpt_cli-0.1.2/README.md` & `simple_chatgpt_cli-0.1.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -6,21 +6,20 @@
 
 ```bash
 pip install simple-chatgpt-cli
 ```
 
 ## Usage
 
-You must have an environment variable `OPENAI_API_KEY` for a valid OpenAI API key.
-
+You can run the program with
 ```bash
-export OPENAI_API_KEY=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
 chatgpt
 ```
 
+You must either have environment variable `OPENAI_API_KEY` or set the key following the CLI prompts.
 
 ![screenshot](screenshot.png)
 
 ## Tips
 
 Use `#startover` to start a new conversation whenever you switch to a new topic and the bot doesn't need previous context anymore. This helps reduce your OpenAI bill.
```

### Comparing `simple_chatgpt_cli-0.1.2/chatgpt_cli/main.py` & `simple_chatgpt_cli-0.1.3/chatgpt_cli/main.py`

 * *Files identical despite different names*

### Comparing `simple_chatgpt_cli-0.1.2/pyproject.toml` & `simple_chatgpt_cli-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 wrap-descriptions = 88
 
 [tool.poetry.scripts]
 chatgpt = 'chatgpt_cli.main:run'
 
 [tool.poetry]
 name = "simple-chatgpt-cli"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["tailaiw <29800495+tailaiw@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "chatgpt_cli" }]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
```

### Comparing `simple_chatgpt_cli-0.1.2/PKG-INFO` & `simple_chatgpt_cli-0.1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-chatgpt-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: tailaiw
 Author-email: 29800495+tailaiw@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -20,21 +20,20 @@
 
 ```bash
 pip install simple-chatgpt-cli
 ```
 
 ## Usage
 
-You must have an environment variable `OPENAI_API_KEY` for a valid OpenAI API key.
-
+You can run the program with
 ```bash
-export OPENAI_API_KEY=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
 chatgpt
 ```
 
+You must either have environment variable `OPENAI_API_KEY` or set the key following the CLI prompts.
 
 ![screenshot](screenshot.png)
 
 ## Tips
 
 Use `#startover` to start a new conversation whenever you switch to a new topic and the bot doesn't need previous context anymore. This helps reduce your OpenAI bill.
```


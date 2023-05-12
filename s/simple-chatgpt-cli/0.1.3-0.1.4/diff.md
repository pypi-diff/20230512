# Comparing `tmp/simple_chatgpt_cli-0.1.3.tar.gz` & `tmp/simple_chatgpt_cli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_chatgpt_cli-0.1.3.tar", max compression
+gzip compressed data, was "simple_chatgpt_cli-0.1.4.tar", max compression
```

## Comparing `simple_chatgpt_cli-0.1.3.tar` & `simple_chatgpt_cli-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      880 2023-05-12 20:54:50.644831 simple_chatgpt_cli-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-05-12 12:32:57.857467 simple_chatgpt_cli-0.1.3/chatgpt_cli/__init__.py
--rw-r--r--   0        0        0     6293 2023-05-12 20:51:38.053032 simple_chatgpt_cli-0.1.3/chatgpt_cli/main.py
--rw-r--r--   0        0        0      701 2023-05-12 20:52:31.313668 simple_chatgpt_cli-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 simple_chatgpt_cli-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      901 2023-05-12 21:01:56.967474 simple_chatgpt_cli-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-12 12:32:57.857467 simple_chatgpt_cli-0.1.4/chatgpt_cli/__init__.py
+-rw-r--r--   0        0        0     6444 2023-05-12 21:01:15.393834 simple_chatgpt_cli-0.1.4/chatgpt_cli/main.py
+-rw-r--r--   0        0        0      701 2023-05-12 21:02:03.370348 simple_chatgpt_cli-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1347 1970-01-01 00:00:00.000000 simple_chatgpt_cli-0.1.4/PKG-INFO
```

### Comparing `simple_chatgpt_cli-0.1.3/README.md` & `simple_chatgpt_cli-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ## Usage
 
 You can run the program with
 ```bash
 chatgpt
 ```
 
-You must either have environment variable `OPENAI_API_KEY` or set the key following the CLI prompts.
+You must either set/save the key following the CLI prompts (recommended) or set an environment variable `OPENAI_API_KEY`.
 
 ![screenshot](screenshot.png)
 
 ## Tips
 
 Use `#startover` to start a new conversation whenever you switch to a new topic and the bot doesn't need previous context anymore. This helps reduce your OpenAI bill.
```

### Comparing `simple_chatgpt_cli-0.1.3/chatgpt_cli/main.py` & `simple_chatgpt_cli-0.1.4/chatgpt_cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,28 @@
 from rich import print
 from rich.prompt import Confirm, Prompt
 
 # disable CTRL+C
 signal.signal(signal.SIGINT, lambda signum, frame: None)
 
 # OpenAI API key
-key_file_path = os.path.join(os.path.expanduser("~"), ".config/openai_key")
+key_file_path = os.path.join(
+    os.path.expanduser("~"), ".config/simple_chatgpt_cli/openai_api_key"
+)
 if os.getenv("OPENAI_API_KEY") is None and not os.path.exists(key_file_path):
     openai_api_key = Prompt.ask(
         "OpenAI API key not found. Press Enter it here to continue", password=True
     )
     openai.api_key = openai_api_key
     confirm_save_key = Confirm.ask(
-        f"Do you want to save the key to {key_file_path}?", default=True
+        f"Do you want to save the key to {key_file_path} so you don't have to enter it again next time?",
+        default=True,
     )
     if confirm_save_key:
+        os.makedirs(os.path.dirname(key_file_path), exist_ok=True)
         with open(key_file_path, "w") as f:
             f.write(openai_api_key)
 elif os.getenv("OPENAI_API_KEY") is None and os.path.exists(key_file_path):
     with open(key_file_path, "r") as f:
         openai.api_key = f.read().strip()
 else:
     openai.api_key = os.getenv("OPENAI_API_KEY")
```

### Comparing `simple_chatgpt_cli-0.1.3/pyproject.toml` & `simple_chatgpt_cli-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 wrap-descriptions = 88
 
 [tool.poetry.scripts]
 chatgpt = 'chatgpt_cli.main:run'
 
 [tool.poetry]
 name = "simple-chatgpt-cli"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["tailaiw <29800495+tailaiw@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "chatgpt_cli" }]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
```

### Comparing `simple_chatgpt_cli-0.1.3/PKG-INFO` & `simple_chatgpt_cli-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-chatgpt-cli
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: tailaiw
 Author-email: 29800495+tailaiw@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -25,15 +25,15 @@
 ## Usage
 
 You can run the program with
 ```bash
 chatgpt
 ```
 
-You must either have environment variable `OPENAI_API_KEY` or set the key following the CLI prompts.
+You must either set/save the key following the CLI prompts (recommended) or set an environment variable `OPENAI_API_KEY`.
 
 ![screenshot](screenshot.png)
 
 ## Tips
 
 Use `#startover` to start a new conversation whenever you switch to a new topic and the bot doesn't need previous context anymore. This helps reduce your OpenAI bill.
```


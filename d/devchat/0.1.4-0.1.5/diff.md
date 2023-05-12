# Comparing `tmp/devchat-0.1.4.tar.gz` & `tmp/devchat-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devchat-0.1.4.tar", last modified: Mon May  8 09:08:26 2023, max compression
+gzip compressed data, was "devchat-0.1.5.tar", last modified: Fri May 12 04:10:23 2023, max compression
```

## Comparing `devchat-0.1.4.tar` & `devchat-0.1.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-08 09:08:26.267629 devchat-0.1.4/
--rw-r--r--   0 basicthinker   (501) staff       (20)    11357 2023-05-05 13:17:54.000000 devchat-0.1.4/LICENSE
--rw-r--r--   0 basicthinker   (501) staff       (20)      227 2023-05-08 09:08:26.267445 devchat-0.1.4/PKG-INFO
--rw-r--r--   0 basicthinker   (501) staff       (20)       44 2023-05-05 13:17:54.000000 devchat-0.1.4/README.md
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-08 09:08:26.264187 devchat-0.1.4/devchat/
--rw-r--r--   0 basicthinker   (501) staff       (20)        0 2023-05-05 13:17:54.000000 devchat-0.1.4/devchat/__init__.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     5399 2023-05-08 04:39:28.000000 devchat-0.1.4/devchat/_cli.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     4363 2023-05-08 03:39:48.000000 devchat-0.1.4/devchat/assistant.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     1464 2023-05-05 13:17:54.000000 devchat-0.1.4/devchat/chat.py
--rw-r--r--   0 basicthinker   (501) staff       (20)      614 2023-05-07 23:44:52.000000 devchat-0.1.4/devchat/message.py
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-08 09:08:26.265987 devchat-0.1.4/devchat/openai/
--rw-r--r--   0 basicthinker   (501) staff       (20)      248 2023-05-05 13:17:54.000000 devchat-0.1.4/devchat/openai/__init__.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     3402 2023-05-08 03:20:19.000000 devchat-0.1.4/devchat/openai/openai_chat.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     1561 2023-05-07 23:44:52.000000 devchat-0.1.4/devchat/openai/openai_message.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     5332 2023-05-07 23:44:52.000000 devchat-0.1.4/devchat/openai/openai_prompt.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     5891 2023-05-08 03:39:48.000000 devchat-0.1.4/devchat/prompt.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     3568 2023-05-08 03:39:48.000000 devchat-0.1.4/devchat/store.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     3783 2023-05-07 23:44:52.000000 devchat-0.1.4/devchat/utils.py
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-08 09:08:26.265090 devchat-0.1.4/devchat.egg-info/
--rw-r--r--   0 basicthinker   (501) staff       (20)      227 2023-05-08 09:08:26.000000 devchat-0.1.4/devchat.egg-info/PKG-INFO
--rw-r--r--   0 basicthinker   (501) staff       (20)      628 2023-05-08 09:08:26.000000 devchat-0.1.4/devchat.egg-info/SOURCES.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)        1 2023-05-08 09:08:26.000000 devchat-0.1.4/devchat.egg-info/dependency_links.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)       46 2023-05-08 09:08:26.000000 devchat-0.1.4/devchat.egg-info/entry_points.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)      100 2023-05-08 09:08:26.000000 devchat-0.1.4/devchat.egg-info/requires.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)       14 2023-05-08 09:08:26.000000 devchat-0.1.4/devchat.egg-info/top_level.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)      102 2023-05-05 13:17:54.000000 devchat-0.1.4/pyproject.toml
--rw-r--r--   0 basicthinker   (501) staff       (20)       38 2023-05-08 09:08:26.267666 devchat-0.1.4/setup.cfg
--rw-r--r--   0 basicthinker   (501) staff       (20)      547 2023-05-08 09:07:10.000000 devchat-0.1.4/setup.py
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-08 09:08:26.267191 devchat-0.1.4/tests/
--rw-r--r--   0 basicthinker   (501) staff       (20)        0 2023-05-05 13:17:54.000000 devchat-0.1.4/tests/__init__.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     3899 2023-05-08 03:39:48.000000 devchat-0.1.4/tests/test_cli.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     1809 2023-05-07 23:44:52.000000 devchat-0.1.4/tests/test_openai_message.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     5908 2023-05-07 23:44:52.000000 devchat-0.1.4/tests/test_openai_prompt.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     2303 2023-05-05 15:34:17.000000 devchat-0.1.4/tests/test_store.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     1225 2023-05-07 23:44:52.000000 devchat-0.1.4/tests/test_utils.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-12 04:10:23.687226 devchat-0.1.5/
+-rw-r--r--   0 basicthinker   (501) staff       (20)    11357 2023-05-05 13:17:54.000000 devchat-0.1.5/LICENSE
+-rw-r--r--   0 basicthinker   (501) staff       (20)      227 2023-05-12 04:10:23.687061 devchat-0.1.5/PKG-INFO
+-rw-r--r--   0 basicthinker   (501) staff       (20)       44 2023-05-05 13:17:54.000000 devchat-0.1.5/README.md
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-12 04:10:23.683537 devchat-0.1.5/devchat/
+-rw-r--r--   0 basicthinker   (501) staff       (20)        0 2023-05-05 13:17:54.000000 devchat-0.1.5/devchat/__init__.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5666 2023-05-12 01:45:56.000000 devchat-0.1.5/devchat/_cli.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     4552 2023-05-12 00:41:47.000000 devchat-0.1.5/devchat/assistant.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1464 2023-05-05 13:17:54.000000 devchat-0.1.5/devchat/chat.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)      614 2023-05-07 23:44:52.000000 devchat-0.1.5/devchat/message.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-12 04:10:23.685283 devchat-0.1.5/devchat/openai/
+-rw-r--r--   0 basicthinker   (501) staff       (20)      248 2023-05-05 13:17:54.000000 devchat-0.1.5/devchat/openai/__init__.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     3402 2023-05-08 03:20:19.000000 devchat-0.1.5/devchat/openai/openai_chat.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1561 2023-05-07 23:44:52.000000 devchat-0.1.5/devchat/openai/openai_message.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     6017 2023-05-12 02:31:16.000000 devchat-0.1.5/devchat/openai/openai_prompt.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     6447 2023-05-12 00:56:54.000000 devchat-0.1.5/devchat/prompt.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     3568 2023-05-08 03:39:48.000000 devchat-0.1.5/devchat/store.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     4981 2023-05-12 00:21:13.000000 devchat-0.1.5/devchat/utils.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-12 04:10:23.684398 devchat-0.1.5/devchat.egg-info/
+-rw-r--r--   0 basicthinker   (501) staff       (20)      227 2023-05-12 04:10:23.000000 devchat-0.1.5/devchat.egg-info/PKG-INFO
+-rw-r--r--   0 basicthinker   (501) staff       (20)      628 2023-05-12 04:10:23.000000 devchat-0.1.5/devchat.egg-info/SOURCES.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)        1 2023-05-12 04:10:23.000000 devchat-0.1.5/devchat.egg-info/dependency_links.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)       46 2023-05-12 04:10:23.000000 devchat-0.1.5/devchat.egg-info/entry_points.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)      116 2023-05-12 04:10:23.000000 devchat-0.1.5/devchat.egg-info/requires.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)       14 2023-05-12 04:10:23.000000 devchat-0.1.5/devchat.egg-info/top_level.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)      102 2023-05-05 13:17:54.000000 devchat-0.1.5/pyproject.toml
+-rw-r--r--   0 basicthinker   (501) staff       (20)       38 2023-05-12 04:10:23.687268 devchat-0.1.5/setup.cfg
+-rw-r--r--   0 basicthinker   (501) staff       (20)      547 2023-05-12 04:09:29.000000 devchat-0.1.5/setup.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-12 04:10:23.686789 devchat-0.1.5/tests/
+-rw-r--r--   0 basicthinker   (501) staff       (20)        0 2023-05-05 13:17:54.000000 devchat-0.1.5/tests/__init__.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5996 2023-05-12 00:42:14.000000 devchat-0.1.5/tests/test_cli.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1809 2023-05-07 23:44:52.000000 devchat-0.1.5/tests/test_openai_message.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5908 2023-05-12 00:53:18.000000 devchat-0.1.5/tests/test_openai_prompt.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     2303 2023-05-05 15:34:17.000000 devchat-0.1.5/tests/test_store.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1225 2023-05-07 23:44:52.000000 devchat-0.1.5/tests/test_utils.py
```

### Comparing `devchat-0.1.4/LICENSE` & `devchat-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `devchat-0.1.4/devchat/_cli.py` & `devchat-0.1.5/devchat/_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,35 +48,36 @@
     try:
         with open(os.path.join(chat_dir, 'config.json'), 'r', encoding='utf-8') as file:
             config_data = json.load(file)
     except FileNotFoundError:
         config_data = default_config_data
 
     store = Store(chat_dir)
-    git_ignore(git_root, store.graph_path, store.db_path)
+    git_ignore(git_root, chat_dir)
     return config_data, store
 
 
 @main.command()
 @click.argument('content', required=False)
 @click.option('-p', '--parent', help='Input the parent prompt hash to continue the conversation.')
 @click.option('-r', '--reference', multiple=True,
               help='Input one or more specific previous prompts to include in the current prompt.')
 @click.option('-i', '--instruct', multiple=True,
               help='Add one or more files to the prompt as instructions.')
 @click.option('-c', '--context', multiple=True,
               help='Add one or more files to the prompt as a context.')
-@click.option('-m', '--model', help='Specify the model to use for the prompt.')
+@click.option('-m', '--model', help='Specify the model to temporarily use for the prompt '
+              '(prefer to modify .chat/config.json).')
 def prompt(content: Optional[str], parent: Optional[str], reference: Optional[List[str]],
            instruct: Optional[List[str]], context: Optional[List[str]], model: Optional[str]):
     """
     Main function to run the chat application.
 
     This function initializes the chat system based on the specified large language model (LLM),
-    and performs interactions with the user by sending prompts and retrieving responses.
+    and performs interactions with the LLM by sending prompts and retrieving responses.
 
     Examples
     --------
 
     To send a single-line message to the LLM, provide the content as an argument:
 
     ```bash
@@ -93,31 +94,33 @@
     ```
 
     Note the quotes around EOF in the first line, to prevent the shell from expanding variables.
 
     Configuration
     -------------
 
-    The DevChat CLI reads its configuration from a file `.chatconfig.json` in the current directory.
+    DevChat CLI reads its configuration from `.chat/config.json` in your current Git root directory.
     If the file is not found, it uses the following default configuration:
     ```json
     {
         "model": "gpt-3.5-turbo",
+        "tokens-per-prompt": 3000,
         "provider": "OpenAI",
         "OpenAI": {
             "temperature": 0.2
         }
     }
     ```
 
-    To customize the configuration, create a `.chatconfig.json` file in the current directory and
-    modify the settings as needed. We recoommend the following settings:
+    To customize the configuration, create `.chat/config.json` in your current Git root directory
+    and modify the settings as needed. We recoommend the following settings:
     ```json
     {
         "model": "gpt-4",
+        "tokens-per-prompt": 6000,
         "provider": "OpenAI",
         "OpenAI": {
             "temperature": 0.2,
             "stream": true
         }
     }
     ```
@@ -146,19 +149,22 @@
         if provider == 'OpenAI':
             if model is None:
                 model = config['model']
             openai_config = OpenAIChatConfig(model=model, **config['OpenAI'])
 
             chat = OpenAIChat(openai_config)
 
-            openai_asisstant = Assistant(chat, store)
-            openai_asisstant.make_prompt(content, instruct_contents, context_contents,
-                                         parent, reference)
+            assistant = Assistant(chat, store)
+            if 'tokens-per-prompt' in config:
+                assistant.token_limit = config['tokens-per-prompt']
 
-            for response in openai_asisstant.iterate_response():
+            assistant.make_prompt(content, instruct_contents, context_contents,
+                                  parent, reference)
+
+            for response in assistant.iterate_response():
                 click.echo(response, nl=False)
         else:
             click.echo(f"Error: Invalid LLM in configuration '{provider}'", err=True)
             sys.exit(os.EX_DATAERR)
 
 
 @main.command()
@@ -170,9 +176,12 @@
     """
     _, store = init_dir()
 
     recent_prompts = store.select_recent(skip, skip + max_count)
 
     logs = []
     for record in recent_prompts:
-        logs.append(record.shortlog())
+        try:
+            logs.append(record.shortlog())
+        except Exception:
+            continue
     click.echo(json.dumps(logs, indent=2))
```

### Comparing `devchat-0.1.4/devchat/assistant.py` & `devchat-0.1.5/devchat/assistant.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,24 @@
 
         Args:
             chat (Chat): A Chat object used to communicate with chat APIs.
         """
         self._chat = chat
         self._store = store
         self._prompt = None
-        # TODO: Change to token limit and make the following configurable.
-        self.token_limit = 20
-        self._message_count = 0
+        self.token_limit = 3000
 
-    def _check_limit(self) -> bool:
-        return self._message_count < self.token_limit
+    @property
+    def available_tokens(self) -> int:
+        return self.token_limit - self._prompt.request_tokens
+
+    def _check_limit(self):
+        if self._prompt.request_tokens > self.token_limit:
+            raise ValueError(f"Prompt tokens {self._prompt.request_tokens} "
+                             f"beyond limit {self.token_limit}.")
 
     def make_prompt(self, request: str,
                     instruct_contents: Optional[List[str]], context_contents: Optional[List[str]],
                     parent: Optional[str] = None, references: Optional[List[str]] = None):
         """
         Make a prompt for the chat API.
 
@@ -34,24 +38,26 @@
             request (str): The user request.
             instruct_contents (Optional[List[str]]): A list of instructions to the prompt.
             context_contents (Optional[List[str]]): A list of context messages to the prompt.
             parent (Optional[str]): The parent prompt hash. None means a new topic.
             references (Optional[List[str]]): The reference prompt hashes.
         """
         self._prompt = self._chat.init_prompt(request)
+        self._check_limit()
         # Add instructions to the prompt
         if instruct_contents:
             combined_instruct = ''.join(instruct_contents)
             self._prompt.append_new(MessageType.INSTRUCT, combined_instruct)
-        # Set user request
-        self._prompt.set_request(request)
+            self._check_limit()
         # Add context to the prompt
         if context_contents:
             for context_content in context_contents:
                 self._prompt.append_new(MessageType.CONTEXT, context_content)
+                self._check_limit()
+
         # Add history to the prompt
         self._prompt.references = validate_hashes(references)
         for reference_hash in self._prompt.references:
             if not self._append_prompt(self._store.get_prompt(reference_hash)):
                 return
         if parent:
             self._prompt.parent = validate_hashes([parent])[0]
@@ -81,24 +87,20 @@
             self._prompt.set_response(response_str)
             self._store.store_prompt(self._prompt)
             for index in self._prompt.response.keys():
                 yield self._prompt.formatted_response(index) + '\n'
 
     def _append_prompt(self, prompt: Prompt) -> bool:
         # Append the first response and the request of the appended prompt
-        if not self._check_limit():
+        if not self._prompt.append_history(MessageType.CHAT, prompt.response[0],
+                                           self.available_tokens):
             return False
-        self._prompt.append_history(MessageType.CHAT, prompt.response[0])
-        self._message_count += 1
-
-        if not self._check_limit():
+        if not self._prompt.append_history(MessageType.CHAT, prompt.request,
+                                           self.available_tokens):
             return False
-        self._prompt.append_history(MessageType.CHAT, prompt.request)
-        self._message_count += 1
 
         # Append the context messages of the appended prompt
         for context_message in prompt.new_context:
-            if not self._check_limit():
+            if not self._prompt.append_history(MessageType.CONTEXT, context_message,
+                                               self.available_tokens):
                 return False
-            self._prompt.append_history(MessageType.CONTEXT, context_message)
-            self._message_count += 1
         return True
```

### Comparing `devchat-0.1.4/devchat/chat.py` & `devchat-0.1.5/devchat/chat.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.4/devchat/message.py` & `devchat-0.1.5/devchat/message.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.4/devchat/openai/openai_chat.py` & `devchat-0.1.5/devchat/openai/openai_chat.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.4/devchat/openai/openai_message.py` & `devchat-0.1.5/devchat/openai/openai_message.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.4/devchat/openai/openai_prompt.py` & `devchat-0.1.5/devchat/openai/openai_prompt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
+import math
 from typing import List
 from devchat.prompt import Prompt
 from devchat.message import MessageType, Message
-from devchat.utils import update_dict
+from devchat.utils import update_dict, message_tokens
 from .openai_message import OpenAIMessage
 
 
 class OpenAIPrompt(Prompt):
     """
     A class to represent a prompt and its corresponding responses from OpenAI APIs.
     """
@@ -25,47 +26,62 @@
 
     @property
     def messages(self) -> List[dict]:
         combined = []
         # Instruction
         if self._new_messages[MessageType.INSTRUCT]:
             combined += [msg.to_dict() for msg in self._new_messages[MessageType.INSTRUCT]]
-        # New context
-        if self.new_context:
-            combined += [update_dict(msg.to_dict(), 'content',
-                                     f"<context>\n{msg.content}\n</context>")
-                         for msg in self.new_context]
         # History context
         if self._history_messages[MessageType.CONTEXT]:
             combined += [update_dict(msg.to_dict(), 'content',
                                      f"<context>\n{msg.content}\n</context>")
                          for msg in self.new_context]
         # History chat
         if self._history_messages[MessageType.CHAT]:
             combined += [msg.to_dict() for msg
                          in reversed(self._history_messages[MessageType.CHAT])]
         # Request
         if self.request:
             combined += [self.request.to_dict()]
+        # New context
+        if self.new_context:
+            combined += [update_dict(msg.to_dict(), 'content',
+                                     f"<context>\n{msg.content}\n</context>")
+                         for msg in self.new_context]
         return combined
 
-    def append_new(self, message_type: MessageType, content: str):
+    def append_new(self, message_type: MessageType, content: str,
+                   available_tokens: int = math.inf) -> bool:
         if message_type not in (MessageType.INSTRUCT, MessageType.CONTEXT):
             raise ValueError(f"Current messages cannot be of type {message_type}.")
-        self._new_messages[message_type].append(OpenAIMessage(content, 'system'))
+        message = OpenAIMessage(content, 'system')
+        num_tokens = message_tokens(message.to_dict(), self.model)
+        if num_tokens > available_tokens:
+            return False
+        self._new_messages[message_type].append(message)
+        self._request_tokens += num_tokens
+        return True
 
-    def append_history(self, message_type: MessageType, message: Message):
+    def append_history(self, message_type: MessageType, message: Message,
+                       available_tokens: int = math.inf) -> bool:
         if message_type == MessageType.INSTRUCT:
             raise ValueError("History messages cannot be of type INSTRUCT.")
+        num_tokens = message_tokens(message.to_dict(), self.model)
+        if num_tokens > available_tokens:
+            return False
         self._history_messages[message_type].append(message)
+        self._request_tokens += num_tokens
+        return True
 
-    def set_request(self, content: str):
+    def set_request(self, content: str) -> int:
         if not content.strip():
             raise ValueError("The request cannot be empty.")
-        self._new_messages['request'] = OpenAIMessage(content, 'user')
+        message = OpenAIMessage(content, 'user')
+        self._new_messages['request'] = message
+        self._request_tokens += message_tokens(message.to_dict(), self.model)
 
     def set_response(self, response_str: str):
         """
         Parse the API response string and set the Prompt object's attributes.
 
         Args:
             response_str (str): The JSON-formatted response string from the chat API.
```

### Comparing `devchat-0.1.4/devchat/prompt.py` & `devchat-0.1.5/devchat/prompt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from abc import ABC, abstractmethod
 import hashlib
+import math
 from typing import Dict, List
 from devchat.message import MessageType, Message
 from devchat.utils import unix_to_local_datetime
 
 
 class Prompt(ABC):
     """
@@ -36,16 +37,16 @@
         self._history_messages: Dict[str, Message] = {
             MessageType.CONTEXT: [],
             MessageType.CHAT: []
         }
         self.parent: str = None
         self.references: List[str] = []
         self._timestamp: int = None
-        self._request_tokens: int = None
-        self._response_tokens: int = None
+        self._request_tokens: int = 0
+        self._response_tokens: int = 0
         self._hash: str = None
 
     @property
     def timestamp(self) -> int:
         return self._timestamp
 
     @property
@@ -80,30 +81,41 @@
         return self._response_tokens
 
     @property
     def hash(self) -> str:
         return self._hash
 
     @abstractmethod
-    def append_new(self, message_type: MessageType, content: str):
+    def append_new(self, message_type: MessageType, content: str,
+                   available_tokens: int = math.inf) -> bool:
         """
-        Add to the current messages of the prompt.
+        Append a new message provided by the user to the prompt.
 
         Args:
             message_type (MessageType): The type of the message.
             content (str): The content of the message.
+            available_tokens (int): The number of tokens available for the message.
+
+        Returns:
+            bool: Whether the message is appended.
         """
 
     @abstractmethod
-    def append_history(self, message_type: MessageType, message: Message):
+    def append_history(self, message_type: MessageType, message: Message,
+                       available_tokens: int = math.inf) -> bool:
         """
         Add to the history messages of the prompt.
 
         Args:
+            message_type (MessageType): The type of the message.
             message (Message): The message to add.
+            available_tokens (int): The number of tokens available for the message.
+
+        Returns:
+            bool: Whether the message is appended.
         """
 
     @abstractmethod
     def set_request(self, content: str):
         """
         Set the request message for the prompt.
 
@@ -172,11 +184,12 @@
         for message in self.response.values():
             shortlog_data = {
                 "user": f"{self._user_name} <{self._user_email}>",
                 "date": self._timestamp,
                 "context": [msg.to_dict() for msg in self.new_context],
                 "request": self.request.content,
                 "response": message.content,
-                "hash": self.hash
+                "hash": self.hash,
+                "parent": self.parent
             }
             logs.append(shortlog_data)
         return logs
```

### Comparing `devchat-0.1.4/devchat/store.py` & `devchat-0.1.5/devchat/store.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.4/devchat/utils.py` & `devchat-0.1.5/devchat/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+"""
+utils.py - Utility functions for DevChat.
+"""
 import os
 import re
 import getpass
 import socket
 import subprocess
 from typing import List, Tuple
 import datetime
 import pytz
 from dateutil import tz
+import tiktoken
 
 
 def find_git_root():
     try:
         root = subprocess.check_output(["git", "rev-parse", "--show-toplevel"])
         return root.decode("utf-8").strip()
     except subprocess.CalledProcessError as error:
@@ -109,7 +113,39 @@
 
 def update_dict(dict_to_update, key, value) -> dict:
     """
     Update a dictionary with a key-value pair and return the dictionary.
     """
     dict_to_update[key] = value
     return dict_to_update
+
+
+def message_tokens(message: dict, model: str) -> int:
+    """Returns the number of tokens used by a message."""
+    try:
+        encoding = tiktoken.encoding_for_model(model)
+    except KeyError as err:
+        raise ValueError(f"Invalid model {model} for tiktoken.") from err
+
+    num_tokens = 0
+    if model.startswith("gpt-3.5"):
+        num_tokens += 4  # every message follows <|start|>{role/name}\n{content}<|end|>\n
+        tokens_per_name = -1  # if there's a name, the role is omitted
+    elif model.startswith("gpt-4"):
+        num_tokens += 3
+        tokens_per_name = 1
+
+    for key, value in message.items():
+        num_tokens += len(encoding.encode(value))
+        if key == "name":
+            num_tokens += tokens_per_name
+    return num_tokens
+
+
+def response_tokens(response: str, model: str) -> int:
+    """Returns the number of tokens used by a response."""
+    try:
+        encoding = tiktoken.encoding_for_model(model)
+    except KeyError as err:
+        raise ValueError(f"Invalid model {model} for tiktoken.") from err
+
+    return len(encoding.encode(response)) + 3  # +3 for <|start|>assistant<|message|>
```

### Comparing `devchat-0.1.4/devchat.egg-info/SOURCES.txt` & `devchat-0.1.5/devchat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devchat-0.1.4/setup.py` & `devchat-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("devchat/requirements.txt", encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setup(
     name="devchat",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "devchat = devchat._cli:main",
         ],
     },
```

### Comparing `devchat-0.1.4/tests/test_cli.py` & `devchat-0.1.5/tests/test_cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+"""
+test_cli.py - Tests for the command line interface.
+"""
 import os
 import re
 import json
 import shutil
 import tempfile
 import pytest
 from git import Repo
 from click.testing import CliRunner
 from devchat._cli import main
+from devchat.utils import response_tokens
 
 runner = CliRunner()
 
 
 @pytest.fixture(name="git_repo")
 def fixture_git_repo(request):
     # Create a temporary directory
@@ -61,15 +65,15 @@
     assert "Paris" in result.output
 
 
 def test_main_with_temp_config_file(git_repo):
     config_data = {
         'model': 'gpt-3.5-turbo-0301',
         'provider': 'OpenAI',
-        'tokens-per-prompt': 6000,
+        'tokens-per-prompt': 3000,
         'OpenAI': {
             'temperature': 0
         }
     }
 
     chat_dir = os.path.join(git_repo, ".chat")
     if not os.path.exists(chat_dir):
@@ -111,7 +115,64 @@
 def test_main_with_instruct_and_context(git_repo, temp_files):  # pylint: disable=W0613
     result = runner.invoke(main, ['prompt', '-m', 'gpt-4',
                                   '-i', temp_files[0], '-i', temp_files[2],
                                   '--context', temp_files[3],
                                   "It is really scorching."])
     assert result.exit_code == 0
     assert _get_core_content(result.output) == "hot summer\n"
+
+
+def test_main_response_tokens_exceed_config(git_repo):  # pylint: disable=W0613
+    config_data = {
+        'model': 'gpt-3.5-turbo',
+        'provider': 'OpenAI',
+        'tokens-per-prompt': 2000,
+        'OpenAI': {
+            'temperature': 0
+        }
+    }
+
+    chat_dir = os.path.join(git_repo, ".chat")
+    if not os.path.exists(chat_dir):
+        os.makedirs(chat_dir)
+    temp_config_path = os.path.join(chat_dir, "config.json")
+
+    with open(temp_config_path, "w", encoding='utf-8') as temp_config_file:
+        json.dump(config_data, temp_config_file)
+
+    content = ""
+    while response_tokens(content, config_data["model"]) < config_data["tokens-per-prompt"]:
+        content += "This is a test. Ignore what I say. This is a test. Ignore what I say."
+    result = runner.invoke(main, ['prompt', content])
+    assert result.exit_code != 0
+    assert "beyond limit" in result.output
+
+
+def test_main_response_tokens_exceed_config_with_file(git_repo, tmpdir):  # pylint: disable=W0613
+    config_data = {
+        'model': 'gpt-3.5-turbo',
+        'provider': 'OpenAI',
+        'tokens-per-prompt': 2000,
+        'OpenAI': {
+            'temperature': 0
+        }
+    }
+
+    chat_dir = os.path.join(git_repo, ".chat")
+    if not os.path.exists(chat_dir):
+        os.makedirs(chat_dir)
+    temp_config_path = os.path.join(chat_dir, "config.json")
+
+    with open(temp_config_path, "w", encoding='utf-8') as temp_config_file:
+        json.dump(config_data, temp_config_file)
+
+    content_file = tmpdir.join("content.txt")
+    content = ""
+    while response_tokens(content + "This is a test. Ignore what I say.", config_data["model"]) < \
+            config_data["tokens-per-prompt"]:
+        content += "This is a test. Ignore what I say."
+    content_file.write(content)
+
+    input_str = "This is a test. Ignore what I say."
+    result = runner.invoke(main, ['prompt', '-c', str(content_file), input_str])
+    assert result.exit_code != 0
+    assert "beyond limit" in result.output
```

### Comparing `devchat-0.1.4/tests/test_openai_message.py` & `devchat-0.1.5/tests/test_openai_message.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.4/tests/test_openai_prompt.py` & `devchat-0.1.5/tests/test_openai_prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,16 +157,16 @@
     expected_context_message["content"] = "<context>\n" + context_message.content + "\n</context>"
 
     expected_request_message = request_message.to_dict()
     expected_request_message["content"] = request_message.content
 
     assert prompt.messages == [
         instruct_message.to_dict(),
-        expected_context_message,
-        expected_request_message
+        expected_request_message,
+        expected_context_message
     ]
 
 
 def test_messages_invalid_append():
     prompt = OpenAIPrompt("davinci-codex", "John Doe", "john.doe@example.com")
     with pytest.raises(ValueError):
         prompt.append_new('invalid', 'Instructions')
```

### Comparing `devchat-0.1.4/tests/test_store.py` & `devchat-0.1.5/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.4/tests/test_utils.py` & `devchat-0.1.5/tests/test_utils.py`

 * *Files identical despite different names*


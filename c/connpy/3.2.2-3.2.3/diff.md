# Comparing `tmp/connpy-3.2.2.tar.gz` & `tmp/connpy-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connpy-3.2.2.tar", last modified: Wed May 10 15:54:51 2023, max compression
+gzip compressed data, was "connpy-3.2.3.tar", last modified: Fri May 12 15:06:29 2023, max compression
```

## Comparing `connpy-3.2.2.tar` & `connpy-3.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:54:51.567473 connpy-3.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-10 15:54:40.000000 connpy-3.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-10 15:54:51.567473 connpy-3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-05-10 15:54:40.000000 connpy-3.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:54:51.563472 connpy-3.2.2/connpy/
--rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-05-10 15:54:40.000000 connpy-3.2.2/connpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-10 15:54:40.000000 connpy-3.2.2/connpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-10 15:54:40.000000 connpy-3.2.2/connpy/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15368 2023-05-10 15:54:40.000000 connpy-3.2.2/connpy/ai.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4840 2023-05-10 15:54:40.000000 connpy-3.2.2/connpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-10 15:54:40.000000 connpy-3.2.2/connpy/completion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15540 2023-05-10 15:54:40.000000 connpy-3.2.2/connpy/configfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    50300 2023-05-10 15:54:40.000000 connpy-3.2.2/connpy/connapp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28719 2023-05-10 15:54:40.000000 connpy-3.2.2/connpy/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:54:51.567473 connpy-3.2.2/connpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-10 15:54:51.000000 connpy-3.2.2/connpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-10 15:54:51.000000 connpy-3.2.2/connpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:54:51.000000 connpy-3.2.2/connpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-10 15:54:51.000000 connpy-3.2.2/connpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 15:54:51.000000 connpy-3.2.2/connpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 15:54:51.000000 connpy-3.2.2/connpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-10 15:54:51.567473 connpy-3.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 15:54:40.000000 connpy-3.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:06:29.679170 connpy-3.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-12 15:06:18.000000 connpy-3.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-12 15:06:29.679170 connpy-3.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-05-12 15:06:18.000000 connpy-3.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:06:29.679170 connpy-3.2.3/connpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-05-12 15:06:18.000000 connpy-3.2.3/connpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-12 15:06:18.000000 connpy-3.2.3/connpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 15:06:18.000000 connpy-3.2.3/connpy/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20394 2023-05-12 15:06:18.000000 connpy-3.2.3/connpy/ai.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5102 2023-05-12 15:06:18.000000 connpy-3.2.3/connpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-12 15:06:18.000000 connpy-3.2.3/connpy/completion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15540 2023-05-12 15:06:18.000000 connpy-3.2.3/connpy/configfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50300 2023-05-12 15:06:18.000000 connpy-3.2.3/connpy/connapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28719 2023-05-12 15:06:18.000000 connpy-3.2.3/connpy/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:06:29.679170 connpy-3.2.3/connpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-12 15:06:29.000000 connpy-3.2.3/connpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-12 15:06:29.000000 connpy-3.2.3/connpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:06:29.000000 connpy-3.2.3/connpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-12 15:06:29.000000 connpy-3.2.3/connpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-12 15:06:29.000000 connpy-3.2.3/connpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 15:06:29.000000 connpy-3.2.3/connpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-12 15:06:29.679170 connpy-3.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 15:06:18.000000 connpy-3.2.3/setup.py
```

### Comparing `connpy-3.2.2/LICENSE` & `connpy-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `connpy-3.2.2/PKG-INFO` & `connpy-3.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.2.2
+Version: 3.2.3
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
@@ -264,14 +264,16 @@
 * `expected` (optional, only used when the action is `test`): A single expected result for the test.
 * `options` (optional): Array to pass options to the run command, options are: `prompt`, `parallel`, `timeout`  
 
 #### Response:
 
 - A JSON object with the results of the executed commands on the nodes.
 
+---
+
 ### 4. Ask AI
 
 **Endpoint**: `/ask_ai`
 
 **Method**: `POST`
 
 **Description**: This route sends to chatgpt IA a request that will parse it into an understandable output for the application and then run the request.
```

### Comparing `connpy-3.2.2/README.md` & `connpy-3.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -242,14 +242,16 @@
 * `expected` (optional, only used when the action is `test`): A single expected result for the test.
 * `options` (optional): Array to pass options to the run command, options are: `prompt`, `parallel`, `timeout`  
 
 #### Response:
 
 - A JSON object with the results of the executed commands on the nodes.
 
+---
+
 ### 4. Ask AI
 
 **Endpoint**: `/ask_ai`
 
 **Method**: `POST`
 
 **Description**: This route sends to chatgpt IA a request that will parse it into an understandable output for the application and then run the request.
```

### Comparing `connpy-3.2.2/connpy/__init__.py` & `connpy-3.2.3/connpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,14 +148,16 @@
 * `expected` (optional, only used when the action is `test`): A single expected result for the test.
 * `options` (optional): Array to pass options to the run command, options are: `prompt`, `parallel`, `timeout`  
 
 #### Response:
 
 - A JSON object with the results of the executed commands on the nodes.
 
+---
+
 ### 4. Ask AI
 
 **Endpoint**: `/ask_ai`
 
 **Method**: `POST`
 
 **Description**: This route sends to chatgpt IA a request that will parse it into an understandable output for the application and then run the request.
```

### Comparing `connpy-3.2.2/connpy/ai.py` & `connpy-3.2.3/connpy/ai.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import openai
+import time
 import json
 import re
 import ast
 from textwrap import dedent
 from .core import nodes
+from copy import deepcopy
 
 class ai:
     ''' This class generates a ai object. Containts all the information and methods to make requests to openAI chatGPT to run actions on the application.
 
     ### Attributes:  
 
         - model        (str): Model of GPT api to use. Default is gpt-3.5-turbo.
@@ -112,17 +114,42 @@
 
     Devices:
     router1: cisco ios
     """
         self.__prompt["command_assistant"]= """
     router1: ['show running-config']
     """
+        self.__prompt["confirmation_system"] = """
+        Please analyze the user's input and categorize it as either an affirmation or negation. Based on this analysis, respond with:
+
+            'True' if the input is an affirmation like 'do it', 'go ahead', 'sure', etc.
+            'False' if the input is a negation.
+            If the input does not fit into either of these categories, kindly express that you didn't understand and request the user to rephrase their response.
+            """
+        self.__prompt["confirmation_user"] = "Yes go ahead!"
+        self.__prompt["confirmation_assistant"] = "True"
         self.model = model
         self.temp = temp
 
+    def _retry_function(self, function, max_retries, backoff_num, *args):
+        #Retry openai requests
+        retries = 0
+        while retries < max_retries:
+            try:
+                myfunction = function(*args)
+                break
+            except (openai.error.APIConnectionError, openai.error.RateLimitError):
+                wait_time = backoff_num * (2 ** retries)
+                time.sleep(wait_time)
+                retries += 1
+                continue
+        if retries == max_retries:
+            myfunction = False
+        return myfunction
+
     def _clean_original_response(self, raw_response):
         #Parse response for first request to openAI GPT.
         info_dict = {}
         info_dict["app_related"] = False
         current_key = "response"
         for line in raw_response.split("\n"):
             if line.strip() == "":
@@ -174,14 +201,22 @@
                             info_dict["commands"].append(f"{{command{i}}}")
                             info_dict["variables"]["__global__"][f"command{i}"] = ""
                     info_dict["variables"][key] = newvalue
                 except:
                     pass
         return info_dict
 
+    def _clean_confirmation_response(self, raw_response):
+        #Parse response for confirmation request to openAI GPT.
+        value = raw_response.strip()
+        if value.strip(".").lower() == "true":
+            value = True
+        elif value.strip(".").lower() == "false":
+            value = False
+        return value
 
     def _get_commands(self, user_input, nodes):
         #Send the request for commands for each device to openAI GPT.
         output_list = []
         for key, value in nodes.items():
             tags = value.get('tags', {})
             try:
@@ -229,15 +264,59 @@
         output["raw_response"] = response["choices"][0]["message"]["content"] 
         chat_history.append({"role": "assistant", "content": output["raw_response"]})
         output["chat_history"] = chat_history
         clear_response = self._clean_original_response(output["raw_response"])
         output["response"] = self._clean_original_response(output["raw_response"])
         return output
         
-    def ask(self, user_input, dryrun = False, chat_history = None):
+    def _get_confirmation(self, user_input):
+        #Send the request to identify if user is confirming or denying the task
+        message = []
+        message.append({"role": "system", "content": dedent(self.__prompt["confirmation_system"])})
+        message.append({"role": "user", "content": dedent(self.__prompt["confirmation_user"])})
+        message.append({"role": "assistant", "content": dedent(self.__prompt["confirmation_assistant"])})
+        message.append({"role": "user", "content": user_input})
+        response = openai.ChatCompletion.create(
+            model=self.model,
+            messages=message,
+            temperature=self.temp,
+            top_p=1
+            )
+        output = {}
+        output["dict_response"] = response
+        output["raw_response"] = response["choices"][0]["message"]["content"] 
+        output["response"] = self._clean_confirmation_response(output["raw_response"])
+        return output
+
+    def confirm(self, user_input, max_retries=3, backoff_num=1):
+        '''
+        Send the user input to openAI GPT and verify if response is afirmative or negative.
+
+        ### Parameters:  
+
+            - user_input (str): User response confirming or denying.
+
+        ### Optional Parameters:  
+
+            - max_retries (int): Maximum number of retries for gpt api.
+            - backoff_num (int): Backoff factor for exponential wait time
+                                 between retries.
+
+        ### Returns:  
+
+            bool or str: True, False or str if AI coudn't understand the response
+        '''
+        result = self._retry_function(self._get_confirmation, max_retries, backoff_num, user_input)
+        if result:
+            output = result["response"]
+        else:
+            output = f"{self.model} api is not responding right now, please try again later."
+        return output
+
+    def ask(self, user_input, dryrun = False, chat_history = None,  max_retries=3, backoff_num=1):
         '''
         Send the user input to openAI GPT and parse the response to run an action in the application.
 
         ### Parameters:  
 
             - user_input (str): Request to send to openAI that will be parsed
                                 and returned to execute on the application.
@@ -246,17 +325,21 @@
                                 - List a group of devices.
                                 - Test a command on a group of devices
                                   and verify if the output contain an
                                   expected value.
 
         ### Optional Parameters:  
 
-            - dryrun  (bool): Set to true to get the arguments to use to run
-                              in the app. Default is false and it will run 
-                              the actions directly.
+            - dryrun       (bool): Set to true to get the arguments to use to
+                                   run in the app. Default is false and it
+                                   will run the actions directly.
+            - chat_history (list): List in gpt api format for the chat history.
+            - max_retries   (int): Maximum number of retries for gpt api.
+            - backoff_num   (int): Backoff factor for exponential wait time
+                                   between retries.
 
         ### Returns:  
 
             dict: Dictionary formed with the following keys:
                   - input: User input received
                   - app_related: True if GPT detected the request to be related
                     to the application.
@@ -275,15 +358,19 @@
                   - chat_history: The chat history between user and chatbot.
                     It can be used as an attribute for next request.
                 
                     
 
         '''
         output = {}
-        original = self._get_filter(user_input, chat_history)
+        original = self._retry_function(self._get_filter, max_retries, backoff_num, user_input, chat_history)
+        if not original:
+            output["app_related"] = False
+            output["response"] = f"{self.model} api is not responding right now, please try again later."
+            return output
         output["input"] = user_input
         output["app_related"] = original["response"]["app_related"]
         output["dryrun"] = dryrun
         output["chat_history"] = original["chat_history"]
         if not output["app_related"]:
             output["response"] = original["response"]["response"]
         else:
@@ -297,27 +384,43 @@
                         output["filter"] = output["filter"].lower()
                 if not dryrun or type == "command":
                     thisnodes = self.config._getallnodesfull(output["filter"])
                     output["nodes"] = list(thisnodes.keys())
             if not type == "command":
                 output["action"] = "list_nodes"
             else:
-                commands = self._get_commands(user_input, thisnodes)
+                commands = self._retry_function(self._get_commands, max_retries, backoff_num, user_input, thisnodes)
+                if not commands:
+                    output = []
+                    output["app_related"] = False
+                    output["response"] = f"{self.model} api is not responding right now, please try again later."
+                    return output
                 output["args"] = {}
                 output["args"]["commands"] = commands["response"]["commands"]
                 output["args"]["vars"] = commands["response"]["variables"]
                 if original["response"]["expected"]:
                     output["args"]["expected"] = original["response"]["expected"]
                     output["action"] = "test"
                 else:
                     output["action"] = "run"
+                if dryrun:
+                    output["task"] = []
+                    if output["action"] == "test":
+                        output["task"].append({"Task": "Verify if expected value is in command(s) output"})
+                        output["task"].append({"Expected value to verify": output["args"]["expected"]})
+                    elif output["action"] == "run":
+                        output["task"].append({"Task": "Run command(s) on devices and return output"})
+                    varstocommands = deepcopy(output["args"]["vars"])
+                    del varstocommands["__global__"]
+                    output["task"].append({"Devices": varstocommands})
                 if not dryrun:
                     mynodes = nodes(self.config.getitems(output["nodes"]),config=self.config)
                     if output["action"] == "test":
                         output["result"] = mynodes.test(**output["args"])
+                        output["logs"] = mynodes.output
                     elif output["action"] == "run":
                         output["result"] = mynodes.run(**output["args"])
         return output
```

### Comparing `connpy-3.2.2/connpy/api.py` & `connpy-3.2.3/connpy/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,14 +66,21 @@
     if "chat_history" in data:
         chat_history = data["chat_history"]
     else:
         chat_history = None
     ai = myai(conf)
     return ai.ask(input, dryrun, chat_history)
 
+@app.route("/confirm", methods=["POST"])
+def confirm():
+    conf = app.custom_config
+    data = request.get_json()
+    input = data["input"]
+    ai = myai(conf)
+    return str(ai.confirm(input))
 
 @app.route("/run_commands", methods=["POST"])
 def run_commands():
     conf = app.custom_config
     data = request.get_json()
     case = conf.config["case"]
     mynodes = {}
@@ -95,27 +102,29 @@
         if nodelist.startswith("@"):
             mynodes = conf.getitem(nodelist)
         else:
             mynodes[nodelist] = conf.getitem(nodelist)
 
     mynodes = nodes(mynodes, config=conf)
     try:
-        args["vars"] = data["variables"]
+        args["vars"] = data["vars"]
     except:
         pass
     try:
         options = data["options"]
         thisoptions = {k: v for k, v in options.items() if k in ["prompt", "parallel", "timeout"]}
         args.update(thisoptions)
     except:
         options = None
     if action == "run":
         output = mynodes.run(**args)
     elif action == "test":
-        output = mynodes.test(**args)
+        output = {}
+        output["result"] = mynodes.test(**args)
+        output["output"] = mynodes.output
     else:
         error = "Wrong action '{}'".format(action)
         return({"DataError": error})
     return output
 
 def stop_api():
     # Read the process ID (pid) from the file
```

### Comparing `connpy-3.2.2/connpy/completion.py` & `connpy-3.2.3/connpy/completion.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.2/connpy/configfile.py` & `connpy-3.2.3/connpy/configfile.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.2/connpy/connapp.py` & `connpy-3.2.3/connpy/connapp.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.2/connpy/core.py` & `connpy-3.2.3/connpy/core.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.2/connpy.egg-info/PKG-INFO` & `connpy-3.2.3/connpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.2.2
+Version: 3.2.3
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
@@ -264,14 +264,16 @@
 * `expected` (optional, only used when the action is `test`): A single expected result for the test.
 * `options` (optional): Array to pass options to the run command, options are: `prompt`, `parallel`, `timeout`  
 
 #### Response:
 
 - A JSON object with the results of the executed commands on the nodes.
 
+---
+
 ### 4. Ask AI
 
 **Endpoint**: `/ask_ai`
 
 **Method**: `POST`
 
 **Description**: This route sends to chatgpt IA a request that will parse it into an understandable output for the application and then run the request.
```

### Comparing `connpy-3.2.2/setup.cfg` & `connpy-3.2.3/setup.cfg`

 * *Files identical despite different names*


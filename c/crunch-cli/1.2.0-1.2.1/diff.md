# Comparing `tmp/crunch-cli-1.2.0.tar.gz` & `tmp/crunch-cli-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crunch-cli-1.2.0.tar", last modified: Thu May 11 16:31:54 2023, max compression
+gzip compressed data, was "crunch-cli-1.2.1.tar", last modified: Fri May 12 10:10:48 2023, max compression
```

## Comparing `crunch-cli-1.2.0.tar` & `crunch-cli-1.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:31:54.218885 crunch-cli-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-11 16:31:54.218885 crunch-cli-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-11 16:31:47.000000 crunch-cli-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:31:54.214885 crunch-cli-1.2.0/crunch/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-11 16:31:47.000000 crunch-cli-1.2.0/crunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-11 16:31:47.000000 crunch-cli-1.2.0/crunch/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-11 16:31:47.000000 crunch-cli-1.2.0/crunch/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:31:54.218885 crunch-cli-1.2.0/crunch/command/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-11 16:31:47.000000 crunch-cli-1.2.0/crunch/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-11 16:31:47.000000 crunch-cli-1.2.0/crunch/command/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-11 16:31:47.000000 crunch-cli-1.2.0/crunch/command/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-11 16:31:47.000000 crunch-cli-1.2.0/crunch/command/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-11 16:31:47.000000 crunch-cli-1.2.0/crunch/command/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-11 16:31:47.000000 crunch-cli-1.2.0/crunch/command/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-11 16:31:47.000000 crunch-cli-1.2.0/crunch/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:31:54.218885 crunch-cli-1.2.0/crunch/demo-project/
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-11 16:31:47.000000 crunch-cli-1.2.0/crunch/demo-project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-11 16:31:47.000000 crunch-cli-1.2.0/crunch/demo-project/files.json
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-05-11 16:31:47.000000 crunch-cli-1.2.0/crunch/demo-project/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-11 16:31:47.000000 crunch-cli-1.2.0/crunch/demo-project/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-11 16:31:47.000000 crunch-cli-1.2.0/crunch/ensure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-11 16:31:47.000000 crunch-cli-1.2.0/crunch/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-11 16:31:47.000000 crunch-cli-1.2.0/crunch/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-11 16:31:47.000000 crunch-cli-1.2.0/crunch/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-11 16:31:47.000000 crunch-cli-1.2.0/crunch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:31:54.218885 crunch-cli-1.2.0/crunch_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-11 16:31:54.000000 crunch-cli-1.2.0/crunch_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-11 16:31:54.000000 crunch-cli-1.2.0/crunch_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:31:54.000000 crunch-cli-1.2.0/crunch_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-11 16:31:54.000000 crunch-cli-1.2.0/crunch_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:31:54.000000 crunch-cli-1.2.0/crunch_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 16:31:54.000000 crunch-cli-1.2.0/crunch_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 16:31:54.000000 crunch-cli-1.2.0/crunch_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 16:31:54.218885 crunch-cli-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-11 16:31:47.000000 crunch-cli-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:10:48.590359 crunch-cli-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-12 10:10:48.590359 crunch-cli-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:10:48.586359 crunch-cli-1.2.1/crunch/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:10:48.586359 crunch-cli-1.2.1/crunch/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/command/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/command/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/command/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/command/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/command/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:10:48.590359 crunch-cli-1.2.1/crunch/demo-project/
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/demo-project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/demo-project/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/demo-project/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/demo-project/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/ensure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:10:48.590359 crunch-cli-1.2.1/crunch_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-12 10:10:48.000000 crunch-cli-1.2.1/crunch_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-12 10:10:48.000000 crunch-cli-1.2.1/crunch_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:10:48.000000 crunch-cli-1.2.1/crunch_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-12 10:10:48.000000 crunch-cli-1.2.1/crunch_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:10:48.000000 crunch-cli-1.2.1/crunch_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-12 10:10:48.000000 crunch-cli-1.2.1/crunch_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 10:10:48.000000 crunch-cli-1.2.1/crunch_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 10:10:48.594359 crunch-cli-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/setup.py
```

### Comparing `crunch-cli-1.2.0/crunch/command/convert.py` & `crunch-cli-1.2.1/crunch/command/convert.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.0/crunch/command/download.py` & `crunch-cli-1.2.1/crunch/command/download.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import typing
+import datetime
 
 import click
 import requests
 import tqdm
 
 from .. import constants, utils
 
@@ -125,7 +126,18 @@
     return (
         embargo,
         moon_column_name,
         x_train_path,
         y_train_path,
         x_test_path
     )
+
+def download_no_data_available():
+    today = datetime.date.today()
+    
+    print("\n---")
+
+    # competition lunch
+    if today <= datetime.date(2023, 5, 16):
+        print("The data will be released on May 16th, 2023, 05.00 PM CET")
+    else:
+        print("No data is available yet")
```

### Comparing `crunch-cli-1.2.0/crunch/command/push.py` & `crunch-cli-1.2.1/crunch/command/push.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.0/crunch/command/setup.py` & `crunch-cli-1.2.1/crunch/command/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from .. import api, constants
 
 
 def _check_if_already_exists(directory: str, force: bool):
     if os.path.exists(directory):
         if force:
-            print(f"{directory}: deleting")
+            print(f"delete {directory}")
             shutil.rmtree(directory)
         else:
             print(f"{directory}: already exists (use --force to override)")
             raise click.Abort()
 
 
 def _setup_demo(directory: str):
```

### Comparing `crunch-cli-1.2.0/crunch/command/test.py` & `crunch-cli-1.2.1/crunch/command/test.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.0/crunch/constants.py` & `crunch-cli-1.2.1/crunch/constants.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.0/crunch/demo-project/.gitignore` & `crunch-cli-1.2.1/crunch/demo-project/.gitignore`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.0/crunch/demo-project/main.py` & `crunch-cli-1.2.1/crunch/demo-project/main.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.0/crunch/ensure.py` & `crunch-cli-1.2.1/crunch/ensure.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.0/crunch/inline.py` & `crunch-cli-1.2.1/crunch/inline.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import sys
 import typing
 
 import click
 import pandas
 
-from . import command, constants, tester, utils
+from . import command, constants, tester, utils, api
 
 
 class _Inline:
 
     def __init__(self, module: typing.Any, model_directory: str):
         self.module = module
         self.model_directory = model_directory
@@ -20,21 +20,25 @@
             os.environ.get(constants.API_BASE_URL_ENV_VAR, constants.API_BASE_URL_DEFAULT),
             bool(os.environ.get(constants.DEBUG_ENV_VAR, "False")),
         )
 
         print(f"loaded inline runner with module: {module}")
     
     def load_data(self) -> typing.Tuple[pandas.DataFrame, pandas.DataFrame, pandas.DataFrame]:
-        (
-            _,
-            _,
-            x_train_path,
-            y_train_path,
-            x_test_path
-        ) = command.download(self.session)
+        try:
+            (
+                _,
+                _,
+                x_train_path,
+                y_train_path,
+                x_test_path
+            ) = command.download(self.session)
+        except api.CurrentCrunchNotFoundException:
+            command.download_no_data_available()
+            raise click.Abort()
 
         x_train = utils.read(x_train_path)
         y_train = utils.read(y_train_path)
         x_test = utils.read(x_test_path)
 
         return x_train, y_train, x_test
```

### Comparing `crunch-cli-1.2.0/crunch/main.py` & `crunch-cli-1.2.1/crunch/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import click
 
-from . import command, constants, utils
+from . import command, constants, utils, api
 
 session = None
 debug = False
 
 
 @click.group()
 @click.option("--debug", "enable_debug", envvar=constants.DEBUG_ENV_VAR, is_flag=True, help="Enable debug output.")
@@ -61,15 +61,19 @@
         model_directory=model_directory_path,
         force=force,
         no_model=no_model,
     )
 
     if not no_data:
         os.chdir(directory)
-        command.download(session, force=True)
+
+        try:
+            command.download(session, force=True)
+        except api.CurrentCrunchNotFoundException:
+            command.download_no_data_available()
 
     print("\n---")
     print(f"Success! Your environment has been correctly setup.")
     print(f"Next recommended actions:")
     print(f" - To get inside your workspace directory, run: cd {directory}")
     print(f" - To see all of the available commands of the CrunchDAO CLI, run: crunch --help")
 
@@ -138,15 +142,18 @@
     )
 
 
 @cli.command(help="Download the data locally.")
 def download():
     utils.change_root()
 
-    command.download(session)
+    try:
+        command.download(session)
+    except api.CurrentCrunchNotFoundException:
+        command.download_no_data_available()
 
 
 @cli.command(help="Convert a notebook to a python script.")
 @click.option("--override", is_flag=True, help="Force overwrite of the python file.")
 @click.argument("notebook-file-path", required=True)
 @click.argument("python-file-path", default="main.py")
 def convert(
```

### Comparing `crunch-cli-1.2.0/crunch/tester.py` & `crunch-cli-1.2.1/crunch/tester.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import time
 import typing
 
 import coloredlogs
 import pandas
 import psutil
 import requests
+import click
 
-from . import command, constants, ensure, utils
+from . import command, constants, ensure, utils, api
 
 
 def _get_process_memory() -> int:
     process = psutil.Process(os.getpid())
     mem_info = process.memory_info()
     return mem_info.rss
 
@@ -45,21 +46,25 @@
 
     memory_before = _get_process_memory()
     start = time.time()
 
     train_handler = ensure.is_function(module, "train")
     infer_handler = ensure.is_function(module, "infer")
 
-    (
-        embargo,
-        moon_column_name,
-        x_train_path,
-        y_train_path,
-        x_test_path
-    ) = command.download(session)
+    try:
+        (
+            embargo,
+            moon_column_name,
+            x_train_path,
+            y_train_path,
+            x_test_path
+        ) = command.download(session)
+    except api.CurrentCrunchNotFoundException:
+        command.download_no_data_available()
+        raise click.Abort()
 
     x_train = utils.read(x_train_path)
     y_train = utils.read(y_train_path)
     x_test = utils.read(x_test_path)
 
     moons = x_test[moon_column_name].unique()
     moons.sort()
```

### Comparing `crunch-cli-1.2.0/crunch/utils.py` & `crunch-cli-1.2.1/crunch/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,14 +45,16 @@
                     print("your token seems to have expired or is invalid")
                     self.print_recopy_command()
                 elif code == "ENTITY_NOT_FOUND" and message.startswith("no user found with username"):
                     print("user not found, did you rename yourself?")
                     self.print_recopy_command()
                 elif code == "NEVER_SUBMITTED":
                     raise api.NeverSubmittedException(message)
+                elif code == "CURRENT_CRUNCH_NOT_FOUND":
+                    raise api.CurrentCrunchNotFoundException(message)
                 else:
                     print(f"{method} {url}: {status_code}")
                     print(json.dumps(error, indent=4))
 
             if self.debug:
                 traceback.print_stack()
```

### Comparing `crunch-cli-1.2.0/crunch_cli.egg-info/SOURCES.txt` & `crunch-cli-1.2.1/crunch_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.0/setup.py` & `crunch-cli-1.2.1/setup.py`

 * *Files identical despite different names*


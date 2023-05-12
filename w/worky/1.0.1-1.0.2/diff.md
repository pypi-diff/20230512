# Comparing `tmp/worky-1.0.1.tar.gz` & `tmp/worky-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "worky-1.0.1.tar", max compression
+gzip compressed data, was "worky-1.0.2.tar", max compression
```

## Comparing `worky-1.0.1.tar` & `worky-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    34523 2023-02-16 01:31:29.674033 worky-1.0.1/LICENSE
--rw-r--r--   0        0        0     5367 2023-04-29 17:08:00.469544 worky-1.0.1/README.md
--rw-r--r--   0        0        0      838 2023-04-29 17:24:42.307151 worky-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      119 2023-04-27 14:39:59.061967 worky-1.0.1/worky/__init__.py
--rw-r--r--   0        0        0      121 2023-04-27 14:33:11.629893 worky-1.0.1/worky/__main__.py
--rw-r--r--   0        0        0     3975 2023-04-29 17:24:34.500573 worky-1.0.1/worky/main.py
--rw-r--r--   0        0        0        0 2023-04-25 20:29:18.162484 worky-1.0.1/worky/models/__init__.py
--rw-r--r--   0        0        0     1759 2023-04-27 14:40:49.885173 worky-1.0.1/worky/models/config_model.py
--rw-r--r--   0        0        0      120 2023-04-27 10:00:41.124836 worky-1.0.1/worky/models/log_level.py
--rw-r--r--   0        0        0        0 2023-04-25 20:29:18.162484 worky-1.0.1/worky/utils/__init__.py
--rw-r--r--   0        0        0     1242 2023-04-27 12:32:08.612359 worky-1.0.1/worky/utils/logger.py
--rw-r--r--   0        0        0      156 2023-04-27 10:26:48.078234 worky-1.0.1/worky/utils/util.py
--rw-r--r--   0        0        0     6159 1970-01-01 00:00:00.000000 worky-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-12 04:54:21.042075 worky-1.0.2/LICENSE
+-rw-r--r--   0        0        0     5727 2023-05-12 05:17:56.803674 worky-1.0.2/README.md
+-rw-r--r--   0        0        0      838 2023-05-12 05:18:21.820316 worky-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-05-12 04:54:21.042075 worky-1.0.2/worky/__init__.py
+-rw-r--r--   0        0        0      121 2023-05-12 04:54:21.042075 worky-1.0.2/worky/__main__.py
+-rw-r--r--   0        0        0     3975 2023-05-12 04:54:21.042075 worky-1.0.2/worky/main.py
+-rw-r--r--   0        0        0        0 2023-05-12 04:54:21.042075 worky-1.0.2/worky/models/__init__.py
+-rw-r--r--   0        0        0     1760 2023-05-12 05:16:07.440441 worky-1.0.2/worky/models/config_model.py
+-rw-r--r--   0        0        0      120 2023-05-12 04:54:21.042075 worky-1.0.2/worky/models/log_level.py
+-rw-r--r--   0        0        0        0 2023-05-12 04:54:21.042075 worky-1.0.2/worky/utils/__init__.py
+-rw-r--r--   0        0        0     1242 2023-05-12 04:54:21.042075 worky-1.0.2/worky/utils/logger.py
+-rw-r--r--   0        0        0      156 2023-05-12 04:54:21.042075 worky-1.0.2/worky/utils/util.py
+-rw-r--r--   0        0        0     6519 1970-01-01 00:00:00.000000 worky-1.0.2/PKG-INFO
```

### Comparing `worky-1.0.1/LICENSE` & `worky-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `worky-1.0.1/README.md` & `worky-1.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -61,22 +61,40 @@
 condition = "docker"
 args = [
     "-f",
     "/path/to/docker-compose.yaml",
     "up"
 ]
 ```
+
 Then you can run `worky -f docker` to load the workspace and run the `compose` step.
 
+## Tips and tricks
+
+### Create an alias
+
+You can create an alias by simply create a symbolic link to your config file in the `~/.config/worky/` directory.
+
+```shell
+ln -s ~/.config/worky/very_long_project_name.toml ~/.config/worky/aliased_name.toml
+```
+
+Then you can use both `worky very_long_project_name` and `worky aliased_name` to load the workspace.
+
 ## Limitations
-Worky configuration depends on the [TOML](https://toml.io/en/) syntax. This means that you can't create two steps with the same name.
-You can crate two different steps using variables with the same value. Moreover, this helps to keep the configuration file clean and readable.
+
+Worky configuration depends on the [TOML](https://toml.io/en/) syntax. This means that you can't create two steps with
+the same name.
+You can crate two different steps using variables with the same value. Moreover, this helps to keep the configuration
+file clean and readable.
 
 ## Usage
+
 After installing and configured worky, you can use it to load your project workspace simply by running:
+
 ```shell
 worky  # If you have a .worky.toml file in the current directory
 # or
 worky {{project_name}}  # If you have a config file in ~/.config/worky/{{project_name}}/config.toml or ~/.config/worky/{{project_name}}.toml
 # or
 worky -c {{path_to_config_file}}  # Defining a custom config file
 ```
```

### Comparing `worky-1.0.1/pyproject.toml` & `worky-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "worky"
-version = "1.0.1"
+version = "1.0.2"
 description = "Worky is a tool that helps to define and load project workspaces."
 authors = ["ZappaBoy <federico.zappone@justanother.cloud>"]
 maintainers = ["ZappaBoy <federico.zappone@justanother.cloud>"]
 readme = "README.md"
 packages = [{ include = "worky" }]
 homepage = "https://github.com/ZappaBoy/worky"
 repository = "https://github.com/ZappaBoy/worky"
```

### Comparing `worky-1.0.1/worky/main.py` & `worky-1.0.2/worky/main.py`

 * *Files identical despite different names*

### Comparing `worky-1.0.1/worky/models/config_model.py` & `worky-1.0.2/worky/models/config_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from typing import List
 
 import toml  # replace with tomllib whet python 3.11 become stable
 
-expandable_variables_pattern = re.compile(r"\$\{.*}")
+expandable_variables_pattern = re.compile(r"\$\{.*?}")
 excluded_steps_entries = ['variables']
 
 
 class Config:
     variables: dict = {}
     steps: List = []
```

### Comparing `worky-1.0.1/worky/utils/logger.py` & `worky-1.0.2/worky/utils/logger.py`

 * *Files identical despite different names*

### Comparing `worky-1.0.1/PKG-INFO` & `worky-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: worky
-Version: 1.0.1
+Version: 1.0.2
 Summary: Worky is a tool that helps to define and load project workspaces.
 Home-page: https://github.com/ZappaBoy/worky
 Keywords: worky,productivity,workspace,initializer
 Author: ZappaBoy
 Author-email: federico.zappone@justanother.cloud
 Maintainer: ZappaBoy
 Maintainer-email: federico.zappone@justanother.cloud
@@ -81,22 +81,40 @@
 condition = "docker"
 args = [
     "-f",
     "/path/to/docker-compose.yaml",
     "up"
 ]
 ```
+
 Then you can run `worky -f docker` to load the workspace and run the `compose` step.
 
+## Tips and tricks
+
+### Create an alias
+
+You can create an alias by simply create a symbolic link to your config file in the `~/.config/worky/` directory.
+
+```shell
+ln -s ~/.config/worky/very_long_project_name.toml ~/.config/worky/aliased_name.toml
+```
+
+Then you can use both `worky very_long_project_name` and `worky aliased_name` to load the workspace.
+
 ## Limitations
-Worky configuration depends on the [TOML](https://toml.io/en/) syntax. This means that you can't create two steps with the same name.
-You can crate two different steps using variables with the same value. Moreover, this helps to keep the configuration file clean and readable.
+
+Worky configuration depends on the [TOML](https://toml.io/en/) syntax. This means that you can't create two steps with
+the same name.
+You can crate two different steps using variables with the same value. Moreover, this helps to keep the configuration
+file clean and readable.
 
 ## Usage
+
 After installing and configured worky, you can use it to load your project workspace simply by running:
+
 ```shell
 worky  # If you have a .worky.toml file in the current directory
 # or
 worky {{project_name}}  # If you have a config file in ~/.config/worky/{{project_name}}/config.toml or ~/.config/worky/{{project_name}}.toml
 # or
 worky -c {{path_to_config_file}}  # Defining a custom config file
 ```
```


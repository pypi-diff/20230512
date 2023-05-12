# Comparing `tmp/crunch-cli-1.2.1.tar.gz` & `tmp/crunch-cli-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crunch-cli-1.2.1.tar", last modified: Fri May 12 10:10:48 2023, max compression
+gzip compressed data, was "crunch-cli-1.2.2.tar", last modified: Fri May 12 10:13:35 2023, max compression
```

## Comparing `crunch-cli-1.2.1.tar` & `crunch-cli-1.2.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:10:48.590359 crunch-cli-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-12 10:10:48.590359 crunch-cli-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:10:48.586359 crunch-cli-1.2.1/crunch/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:10:48.586359 crunch-cli-1.2.1/crunch/command/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/command/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/command/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/command/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/command/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/command/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:10:48.590359 crunch-cli-1.2.1/crunch/demo-project/
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/demo-project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/demo-project/files.json
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/demo-project/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/demo-project/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/ensure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/crunch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:10:48.590359 crunch-cli-1.2.1/crunch_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-12 10:10:48.000000 crunch-cli-1.2.1/crunch_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-12 10:10:48.000000 crunch-cli-1.2.1/crunch_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:10:48.000000 crunch-cli-1.2.1/crunch_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-12 10:10:48.000000 crunch-cli-1.2.1/crunch_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:10:48.000000 crunch-cli-1.2.1/crunch_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-12 10:10:48.000000 crunch-cli-1.2.1/crunch_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 10:10:48.000000 crunch-cli-1.2.1/crunch_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 10:10:48.594359 crunch-cli-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-12 10:10:40.000000 crunch-cli-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:13:35.885020 crunch-cli-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-12 10:13:35.885020 crunch-cli-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-12 10:13:27.000000 crunch-cli-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:13:35.885020 crunch-cli-1.2.2/crunch/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-12 10:13:27.000000 crunch-cli-1.2.2/crunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-12 10:13:27.000000 crunch-cli-1.2.2/crunch/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-12 10:13:27.000000 crunch-cli-1.2.2/crunch/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:13:35.885020 crunch-cli-1.2.2/crunch/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-12 10:13:27.000000 crunch-cli-1.2.2/crunch/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-12 10:13:27.000000 crunch-cli-1.2.2/crunch/command/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-12 10:13:27.000000 crunch-cli-1.2.2/crunch/command/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-12 10:13:27.000000 crunch-cli-1.2.2/crunch/command/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-12 10:13:27.000000 crunch-cli-1.2.2/crunch/command/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-12 10:13:27.000000 crunch-cli-1.2.2/crunch/command/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-12 10:13:27.000000 crunch-cli-1.2.2/crunch/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:13:35.885020 crunch-cli-1.2.2/crunch/demo-project/
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-12 10:13:27.000000 crunch-cli-1.2.2/crunch/demo-project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 10:13:27.000000 crunch-cli-1.2.2/crunch/demo-project/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-12 10:13:27.000000 crunch-cli-1.2.2/crunch/demo-project/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-12 10:13:27.000000 crunch-cli-1.2.2/crunch/demo-project/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-12 10:13:27.000000 crunch-cli-1.2.2/crunch/ensure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-12 10:13:27.000000 crunch-cli-1.2.2/crunch/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-05-12 10:13:27.000000 crunch-cli-1.2.2/crunch/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-12 10:13:27.000000 crunch-cli-1.2.2/crunch/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-12 10:13:27.000000 crunch-cli-1.2.2/crunch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:13:35.885020 crunch-cli-1.2.2/crunch_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-12 10:13:35.000000 crunch-cli-1.2.2/crunch_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-12 10:13:35.000000 crunch-cli-1.2.2/crunch_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:13:35.000000 crunch-cli-1.2.2/crunch_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-12 10:13:35.000000 crunch-cli-1.2.2/crunch_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:13:35.000000 crunch-cli-1.2.2/crunch_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-12 10:13:35.000000 crunch-cli-1.2.2/crunch_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 10:13:35.000000 crunch-cli-1.2.2/crunch_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 10:13:35.885020 crunch-cli-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-12 10:13:27.000000 crunch-cli-1.2.2/setup.py
```

### Comparing `crunch-cli-1.2.1/crunch/command/convert.py` & `crunch-cli-1.2.2/crunch/command/convert.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.1/crunch/command/download.py` & `crunch-cli-1.2.2/crunch/command/download.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.1/crunch/command/push.py` & `crunch-cli-1.2.2/crunch/command/push.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.1/crunch/command/setup.py` & `crunch-cli-1.2.2/crunch/command/setup.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.1/crunch/command/test.py` & `crunch-cli-1.2.2/crunch/command/test.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.1/crunch/constants.py` & `crunch-cli-1.2.2/crunch/constants.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.1/crunch/demo-project/.gitignore` & `crunch-cli-1.2.2/crunch/demo-project/.gitignore`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.1/crunch/ensure.py` & `crunch-cli-1.2.2/crunch/ensure.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.1/crunch/inline.py` & `crunch-cli-1.2.2/crunch/inline.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.1/crunch/main.py` & `crunch-cli-1.2.2/crunch/main.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.1/crunch/tester.py` & `crunch-cli-1.2.2/crunch/tester.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.1/crunch/utils.py` & `crunch-cli-1.2.2/crunch/utils.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.1/crunch_cli.egg-info/SOURCES.txt` & `crunch-cli-1.2.2/crunch_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.2.1/setup.py` & `crunch-cli-1.2.2/setup.py`

 * *Files identical despite different names*


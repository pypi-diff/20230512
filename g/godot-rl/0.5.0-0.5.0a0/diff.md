# Comparing `tmp/godot_rl-0.5.0.tar.gz` & `tmp/godot_rl-0.5.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/edward/play/godot/godot_rl/tmp/godot_rl_agents/dist/.tmp-v2szpqtk/godot_rl-0.5.0.tar", last modified: Fri May 12 08:39:05 2023, max compression
+gzip compressed data, was "/home/edward/play/godot/godot_rl/tmp/godot_rl_agents/dist/.tmp-sg_t1odn/godot_rl-0.5.0a0.tar", last modified: Sat May  6 07:41:50 2023, max compression
```

## Comparing `godot_rl-0.5.0.tar` & `godot_rl-0.5.0a0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-12 08:39:05.577310 godot_rl-0.5.0/
--rw-r--r--   0 edward    (1000) edward    (1000)     1071 2023-05-06 07:37:30.000000 godot_rl-0.5.0/LICENSE
--rw-r--r--   0 edward    (1000) edward    (1000)     7817 2023-05-12 08:39:05.577310 godot_rl-0.5.0/PKG-INFO
--rw-r--r--   0 edward    (1000) edward    (1000)     6748 2023-05-06 07:37:30.000000 godot_rl-0.5.0/README.md
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-12 08:39:05.573310 godot_rl-0.5.0/godot_rl/
--rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-05-06 07:37:30.000000 godot_rl-0.5.0/godot_rl/__init__.py
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-12 08:39:05.573310 godot_rl-0.5.0/godot_rl/core/
--rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-05-06 07:37:30.000000 godot_rl-0.5.0/godot_rl/core/__init__.py
--rw-r--r--   0 edward    (1000) edward    (1000)    11885 2023-05-06 07:37:30.000000 godot_rl-0.5.0/godot_rl/core/godot_env.py
--rw-r--r--   0 edward    (1000) edward    (1000)     3181 2023-05-06 07:37:30.000000 godot_rl-0.5.0/godot_rl/core/utils.py
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-12 08:39:05.573310 godot_rl-0.5.0/godot_rl/custom_models/
--rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-05-06 07:37:30.000000 godot_rl-0.5.0/godot_rl/custom_models/__init__.py
--rw-r--r--   0 edward    (1000) edward    (1000)     3760 2023-05-06 07:37:30.000000 godot_rl-0.5.0/godot_rl/custom_models/attention_model.py
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-12 08:39:05.577310 godot_rl-0.5.0/godot_rl/download_utils/
--rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-05-06 07:37:30.000000 godot_rl-0.5.0/godot_rl/download_utils/__init__.py
--rw-r--r--   0 edward    (1000) edward    (1000)     1191 2023-05-06 07:37:30.000000 godot_rl-0.5.0/godot_rl/download_utils/download_examples.py
--rw-r--r--   0 edward    (1000) edward    (1000)     1746 2023-05-06 07:37:30.000000 godot_rl-0.5.0/godot_rl/download_utils/download_godot_editor.py
--rw-r--r--   0 edward    (1000) edward    (1000)      945 2023-05-06 07:37:30.000000 godot_rl-0.5.0/godot_rl/download_utils/from_hub.py
--rw-r--r--   0 edward    (1000) edward    (1000)     3595 2023-05-06 07:37:30.000000 godot_rl-0.5.0/godot_rl/main.py
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-12 08:39:05.577310 godot_rl-0.5.0/godot_rl/wrappers/
--rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-05-06 07:37:30.000000 godot_rl-0.5.0/godot_rl/wrappers/__init__.py
--rw-r--r--   0 edward    (1000) edward    (1000)     1475 2023-05-06 07:37:30.000000 godot_rl-0.5.0/godot_rl/wrappers/clean_rl_wrapper.py
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-12 08:39:05.577310 godot_rl-0.5.0/godot_rl/wrappers/onnx/
--rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-05-06 07:37:30.000000 godot_rl-0.5.0/godot_rl/wrappers/onnx/__init__.py
--rw-r--r--   0 edward    (1000) edward    (1000)     2855 2023-05-06 07:37:30.000000 godot_rl-0.5.0/godot_rl/wrappers/onnx/stable_baselines_export.py
--rw-r--r--   0 edward    (1000) edward    (1000)     5668 2023-05-06 07:37:30.000000 godot_rl-0.5.0/godot_rl/wrappers/ray_wrapper.py
--rw-r--r--   0 edward    (1000) edward    (1000)     5566 2023-05-06 07:37:30.000000 godot_rl-0.5.0/godot_rl/wrappers/sample_factory_wrapper.py
--rw-r--r--   0 edward    (1000) edward    (1000)     2349 2023-05-06 07:37:30.000000 godot_rl-0.5.0/godot_rl/wrappers/stable_baselines_wrapper.py
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-12 08:39:05.573310 godot_rl-0.5.0/godot_rl.egg-info/
--rw-r--r--   0 edward    (1000) edward    (1000)     7817 2023-05-12 08:39:05.000000 godot_rl-0.5.0/godot_rl.egg-info/PKG-INFO
--rw-r--r--   0 edward    (1000) edward    (1000)     1047 2023-05-12 08:39:05.000000 godot_rl-0.5.0/godot_rl.egg-info/SOURCES.txt
--rw-r--r--   0 edward    (1000) edward    (1000)        1 2023-05-12 08:39:05.000000 godot_rl-0.5.0/godot_rl.egg-info/dependency_links.txt
--rw-r--r--   0 edward    (1000) edward    (1000)      242 2023-05-12 08:39:05.000000 godot_rl-0.5.0/godot_rl.egg-info/entry_points.txt
--rw-r--r--   0 edward    (1000) edward    (1000)        1 2023-05-06 07:41:50.000000 godot_rl-0.5.0/godot_rl.egg-info/not-zip-safe
--rw-r--r--   0 edward    (1000) edward    (1000)      534 2023-05-12 08:39:05.000000 godot_rl-0.5.0/godot_rl.egg-info/requires.txt
--rw-r--r--   0 edward    (1000) edward    (1000)        9 2023-05-12 08:39:05.000000 godot_rl-0.5.0/godot_rl.egg-info/top_level.txt
--rw-r--r--   0 edward    (1000) edward    (1000)      886 2023-05-12 08:38:53.000000 godot_rl-0.5.0/pyproject.toml
--rw-r--r--   0 edward    (1000) edward    (1000)     1258 2023-05-12 08:39:05.577310 godot_rl-0.5.0/setup.cfg
-drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-12 08:39:05.577310 godot_rl-0.5.0/tests/
--rw-r--r--   0 edward    (1000) edward    (1000)     1333 2023-05-06 07:37:30.000000 godot_rl-0.5.0/tests/test_action_space_proprocessor.py
--rw-r--r--   0 edward    (1000) edward    (1000)      421 2023-05-06 07:37:30.000000 godot_rl-0.5.0/tests/test_call_method.py
--rw-r--r--   0 edward    (1000) edward    (1000)     3358 2023-05-06 07:37:30.000000 godot_rl-0.5.0/tests/test_godot_env.py
--rw-r--r--   0 edward    (1000) edward    (1000)      929 2023-05-06 07:37:30.000000 godot_rl-0.5.0/tests/test_sb3_onnx_export.py
--rw-r--r--   0 edward    (1000) edward    (1000)      588 2023-05-06 07:37:30.000000 godot_rl-0.5.0/tests/test_sb3_training.py
+drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.594258 godot_rl-0.5.0a0/
+-rw-r--r--   0 edward    (1000) edward    (1000)     1071 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/LICENSE
+-rw-r--r--   0 edward    (1000) edward    (1000)     7819 2023-05-06 07:41:50.594258 godot_rl-0.5.0a0/PKG-INFO
+-rw-r--r--   0 edward    (1000) edward    (1000)     6748 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/README.md
+drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.586258 godot_rl-0.5.0a0/godot_rl/
+-rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/__init__.py
+drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.590258 godot_rl-0.5.0a0/godot_rl/core/
+-rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/core/__init__.py
+-rw-r--r--   0 edward    (1000) edward    (1000)    11885 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/core/godot_env.py
+-rw-r--r--   0 edward    (1000) edward    (1000)     3181 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/core/utils.py
+drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.590258 godot_rl-0.5.0a0/godot_rl/custom_models/
+-rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/custom_models/__init__.py
+-rw-r--r--   0 edward    (1000) edward    (1000)     3760 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/custom_models/attention_model.py
+drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.590258 godot_rl-0.5.0a0/godot_rl/download_utils/
+-rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/download_utils/__init__.py
+-rw-r--r--   0 edward    (1000) edward    (1000)     1191 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/download_utils/download_examples.py
+-rw-r--r--   0 edward    (1000) edward    (1000)     1746 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/download_utils/download_godot_editor.py
+-rw-r--r--   0 edward    (1000) edward    (1000)      945 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/download_utils/from_hub.py
+-rw-r--r--   0 edward    (1000) edward    (1000)     3595 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/main.py
+drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.590258 godot_rl-0.5.0a0/godot_rl/wrappers/
+-rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/wrappers/__init__.py
+-rw-r--r--   0 edward    (1000) edward    (1000)     1475 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/wrappers/clean_rl_wrapper.py
+drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.590258 godot_rl-0.5.0a0/godot_rl/wrappers/onnx/
+-rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/wrappers/onnx/__init__.py
+-rw-r--r--   0 edward    (1000) edward    (1000)     2855 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/wrappers/onnx/stable_baselines_export.py
+-rw-r--r--   0 edward    (1000) edward    (1000)     5668 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/wrappers/ray_wrapper.py
+-rw-r--r--   0 edward    (1000) edward    (1000)     5566 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/wrappers/sample_factory_wrapper.py
+-rw-r--r--   0 edward    (1000) edward    (1000)     2349 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/wrappers/stable_baselines_wrapper.py
+drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.590258 godot_rl-0.5.0a0/godot_rl.egg-info/
+-rw-r--r--   0 edward    (1000) edward    (1000)     7819 2023-05-06 07:41:50.000000 godot_rl-0.5.0a0/godot_rl.egg-info/PKG-INFO
+-rw-r--r--   0 edward    (1000) edward    (1000)     1047 2023-05-06 07:41:50.000000 godot_rl-0.5.0a0/godot_rl.egg-info/SOURCES.txt
+-rw-r--r--   0 edward    (1000) edward    (1000)        1 2023-05-06 07:41:50.000000 godot_rl-0.5.0a0/godot_rl.egg-info/dependency_links.txt
+-rw-r--r--   0 edward    (1000) edward    (1000)      242 2023-05-06 07:41:50.000000 godot_rl-0.5.0a0/godot_rl.egg-info/entry_points.txt
+-rw-r--r--   0 edward    (1000) edward    (1000)        1 2023-05-06 07:41:50.000000 godot_rl-0.5.0a0/godot_rl.egg-info/not-zip-safe
+-rw-r--r--   0 edward    (1000) edward    (1000)      534 2023-05-06 07:41:50.000000 godot_rl-0.5.0a0/godot_rl.egg-info/requires.txt
+-rw-r--r--   0 edward    (1000) edward    (1000)        9 2023-05-06 07:41:50.000000 godot_rl-0.5.0a0/godot_rl.egg-info/top_level.txt
+-rw-r--r--   0 edward    (1000) edward    (1000)      887 2023-05-06 07:41:12.000000 godot_rl-0.5.0a0/pyproject.toml
+-rw-r--r--   0 edward    (1000) edward    (1000)     1258 2023-05-06 07:41:50.594258 godot_rl-0.5.0a0/setup.cfg
+drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.594258 godot_rl-0.5.0a0/tests/
+-rw-r--r--   0 edward    (1000) edward    (1000)     1333 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/tests/test_action_space_proprocessor.py
+-rw-r--r--   0 edward    (1000) edward    (1000)      421 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/tests/test_call_method.py
+-rw-r--r--   0 edward    (1000) edward    (1000)     3358 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/tests/test_godot_env.py
+-rw-r--r--   0 edward    (1000) edward    (1000)      929 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/tests/test_sb3_onnx_export.py
+-rw-r--r--   0 edward    (1000) edward    (1000)      588 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/tests/test_sb3_training.py
```

### Comparing `godot_rl-0.5.0/LICENSE` & `godot_rl-0.5.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0/PKG-INFO` & `godot_rl-0.5.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: godot_rl
-Version: 0.5.0
+Version: 0.5.0a0
 Summary: A Deep Reinforcement Learning package for the Godot game engine
 Author: Edward Beeching
 Author-email: Edward Beeching <edbeeching@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/pypa/godot_rl_agents
 Project-URL: Bug Tracker, https://github.com/pypa/godot_rl_agents/issues
 Platform: unix
```

### Comparing `godot_rl-0.5.0/README.md` & `godot_rl-0.5.0a0/README.md`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0/godot_rl/core/godot_env.py` & `godot_rl-0.5.0a0/godot_rl/core/godot_env.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0/godot_rl/core/utils.py` & `godot_rl-0.5.0a0/godot_rl/core/utils.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0/godot_rl/custom_models/attention_model.py` & `godot_rl-0.5.0a0/godot_rl/custom_models/attention_model.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0/godot_rl/download_utils/download_examples.py` & `godot_rl-0.5.0a0/godot_rl/download_utils/download_examples.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0/godot_rl/download_utils/download_godot_editor.py` & `godot_rl-0.5.0a0/godot_rl/download_utils/download_godot_editor.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0/godot_rl/download_utils/from_hub.py` & `godot_rl-0.5.0a0/godot_rl/download_utils/from_hub.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0/godot_rl/main.py` & `godot_rl-0.5.0a0/godot_rl/main.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0/godot_rl/wrappers/clean_rl_wrapper.py` & `godot_rl-0.5.0a0/godot_rl/wrappers/clean_rl_wrapper.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0/godot_rl/wrappers/onnx/stable_baselines_export.py` & `godot_rl-0.5.0a0/godot_rl/wrappers/onnx/stable_baselines_export.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0/godot_rl/wrappers/ray_wrapper.py` & `godot_rl-0.5.0a0/godot_rl/wrappers/ray_wrapper.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0/godot_rl/wrappers/sample_factory_wrapper.py` & `godot_rl-0.5.0a0/godot_rl/wrappers/sample_factory_wrapper.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0/godot_rl/wrappers/stable_baselines_wrapper.py` & `godot_rl-0.5.0a0/godot_rl/wrappers/stable_baselines_wrapper.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0/godot_rl.egg-info/PKG-INFO` & `godot_rl-0.5.0a0/godot_rl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: godot-rl
-Version: 0.5.0
+Version: 0.5.0a0
 Summary: A Deep Reinforcement Learning package for the Godot game engine
 Author: Edward Beeching
 Author-email: Edward Beeching <edbeeching@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/pypa/godot_rl_agents
 Project-URL: Bug Tracker, https://github.com/pypa/godot_rl_agents/issues
 Platform: unix
```

### Comparing `godot_rl-0.5.0/godot_rl.egg-info/SOURCES.txt` & `godot_rl-0.5.0a0/godot_rl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0/godot_rl.egg-info/requires.txt` & `godot_rl-0.5.0a0/godot_rl.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0/pyproject.toml` & `godot_rl-0.5.0a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "godot_rl"
-version = "0.5.0"
+version = "0.5.0a"
 authors = [
   { name="Edward Beeching", email="edbeeching@gmail.com" },
 ]
 description = "A Deep Reinforcement Learning package for the Godot game engine"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `godot_rl-0.5.0/setup.cfg` & `godot_rl-0.5.0a0/setup.cfg`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0/tests/test_action_space_proprocessor.py` & `godot_rl-0.5.0a0/tests/test_action_space_proprocessor.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0/tests/test_godot_env.py` & `godot_rl-0.5.0a0/tests/test_godot_env.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0/tests/test_sb3_onnx_export.py` & `godot_rl-0.5.0a0/tests/test_sb3_onnx_export.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.5.0/tests/test_sb3_training.py` & `godot_rl-0.5.0a0/tests/test_sb3_training.py`

 * *Files identical despite different names*


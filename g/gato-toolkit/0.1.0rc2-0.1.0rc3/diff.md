# Comparing `tmp/gato-toolkit-0.1.0rc2.tar.gz` & `tmp/gato-toolkit-0.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gato-toolkit-0.1.0rc2.tar", last modified: Fri May 12 06:45:17 2023, max compression
+gzip compressed data, was "gato-toolkit-0.1.0rc3.tar", last modified: Fri May 12 07:04:29 2023, max compression
```

## Comparing `gato-toolkit-0.1.0rc2.tar` & `gato-toolkit-0.1.0rc3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 06:45:17.002783 gato-toolkit-0.1.0rc2/
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     1070 2023-05-11 12:21:41.000000 gato-toolkit-0.1.0rc2/LICENSE
--rw-r--r--   0 lucaslofaro   (501) staff       (20)       71 2023-05-12 04:29:48.000000 gato-toolkit-0.1.0rc2/MANIFEST.in
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     2261 2023-05-12 06:45:17.002144 gato-toolkit-0.1.0rc2/PKG-INFO
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     1773 2023-05-11 12:58:50.000000 gato-toolkit-0.1.0rc2/README.md
--rw-r--r--   0 lucaslofaro   (501) staff       (20)       38 2023-05-12 06:45:17.002982 gato-toolkit-0.1.0rc2/setup.cfg
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      888 2023-05-12 06:45:11.000000 gato-toolkit-0.1.0rc2/setup.py
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 06:45:16.995939 gato-toolkit-0.1.0rc2/src/
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 06:45:16.998183 gato-toolkit-0.1.0rc2/src/gato/
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 06:45:16.998727 gato-toolkit-0.1.0rc2/src/gato/.config/
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      677 2023-05-04 05:53:25.000000 gato-toolkit-0.1.0rc2/src/gato/.config/action-system-message.txt
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 06:45:17.000247 gato-toolkit-0.1.0rc2/src/gato/.config/scenario-params/
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      240 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc2/src/gato/.config/scenario-params/categories.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      160 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc2/src/gato/.config/scenario-params/domains.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)    22221 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc2/src/gato/.config/scenario-params/entropies.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      123 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc2/src/gato/.config/scenario-params/regions.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      271 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc2/src/gato/.config/scenario-params/scopes.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      134 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc2/src/gato/.config/scenario-params/severities.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     1577 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc2/src/gato/.config/scenario-system-messages.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)        0 2023-05-11 23:28:21.000000 gato-toolkit-0.1.0rc2/src/gato/__init__.py
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      573 2023-05-11 12:46:27.000000 gato-toolkit-0.1.0rc2/src/gato/entity.py
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     1215 2023-05-12 00:47:38.000000 gato-toolkit-0.1.0rc2/src/gato/generator.py
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     1470 2023-05-11 13:42:46.000000 gato-toolkit-0.1.0rc2/src/gato/llm.py
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     2226 2023-05-12 00:47:38.000000 gato-toolkit-0.1.0rc2/src/gato/prompt.py
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      775 2023-05-12 00:47:38.000000 gato-toolkit-0.1.0rc2/src/gato/service.py
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 06:45:17.001693 gato-toolkit-0.1.0rc2/src/gato_toolkit.egg-info/
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     2261 2023-05-12 06:45:16.000000 gato-toolkit-0.1.0rc2/src/gato_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      720 2023-05-12 06:45:16.000000 gato-toolkit-0.1.0rc2/src/gato_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)        1 2023-05-12 06:45:16.000000 gato-toolkit-0.1.0rc2/src/gato_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)       32 2023-05-12 06:45:16.000000 gato-toolkit-0.1.0rc2/src/gato_toolkit.egg-info/requires.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)        5 2023-05-12 06:45:16.000000 gato-toolkit-0.1.0rc2/src/gato_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 07:04:29.569273 gato-toolkit-0.1.0rc3/
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     1070 2023-05-11 12:21:41.000000 gato-toolkit-0.1.0rc3/LICENSE
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)       71 2023-05-12 04:29:48.000000 gato-toolkit-0.1.0rc3/MANIFEST.in
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     2261 2023-05-12 07:04:29.568751 gato-toolkit-0.1.0rc3/PKG-INFO
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     1773 2023-05-11 12:58:50.000000 gato-toolkit-0.1.0rc3/README.md
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)       38 2023-05-12 07:04:29.569351 gato-toolkit-0.1.0rc3/setup.cfg
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      888 2023-05-12 07:03:52.000000 gato-toolkit-0.1.0rc3/setup.py
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 07:04:29.562209 gato-toolkit-0.1.0rc3/src/
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 07:04:29.564316 gato-toolkit-0.1.0rc3/src/gato/
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 07:04:29.564733 gato-toolkit-0.1.0rc3/src/gato/.config/
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      677 2023-05-04 05:53:25.000000 gato-toolkit-0.1.0rc3/src/gato/.config/action-system-message.txt
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 07:04:29.567011 gato-toolkit-0.1.0rc3/src/gato/.config/scenario-params/
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      240 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc3/src/gato/.config/scenario-params/categories.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      160 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc3/src/gato/.config/scenario-params/domains.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)    22221 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc3/src/gato/.config/scenario-params/entropies.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      123 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc3/src/gato/.config/scenario-params/regions.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      271 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc3/src/gato/.config/scenario-params/scopes.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      134 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc3/src/gato/.config/scenario-params/severities.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     1577 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc3/src/gato/.config/scenario-system-messages.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)        0 2023-05-11 23:28:21.000000 gato-toolkit-0.1.0rc3/src/gato/__init__.py
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      574 2023-05-12 06:55:28.000000 gato-toolkit-0.1.0rc3/src/gato/entity.py
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     1216 2023-05-12 07:02:20.000000 gato-toolkit-0.1.0rc3/src/gato/generator.py
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     1470 2023-05-11 13:42:46.000000 gato-toolkit-0.1.0rc3/src/gato/llm.py
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     2233 2023-05-12 07:02:20.000000 gato-toolkit-0.1.0rc3/src/gato/prompt.py
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      764 2023-05-12 07:02:20.000000 gato-toolkit-0.1.0rc3/src/gato/service.py
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 07:04:29.568410 gato-toolkit-0.1.0rc3/src/gato_toolkit.egg-info/
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     2261 2023-05-12 07:04:29.000000 gato-toolkit-0.1.0rc3/src/gato_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      720 2023-05-12 07:04:29.000000 gato-toolkit-0.1.0rc3/src/gato_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)        1 2023-05-12 07:04:29.000000 gato-toolkit-0.1.0rc3/src/gato_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)       32 2023-05-12 07:04:29.000000 gato-toolkit-0.1.0rc3/src/gato_toolkit.egg-info/requires.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)        5 2023-05-12 07:04:29.000000 gato-toolkit-0.1.0rc3/src/gato_toolkit.egg-info/top_level.txt
```

### Comparing `gato-toolkit-0.1.0rc2/LICENSE` & `gato-toolkit-0.1.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `gato-toolkit-0.1.0rc2/PKG-INFO` & `gato-toolkit-0.1.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gato-toolkit
-Version: 0.1.0rc2
+Version: 0.1.0rc3
 Summary: A toolkit for furthering research on AI alignment.
 Home-page: https://github.com/FyZyX/gato-toolkit
 Author: Lucas Lofaro <lucasmlofaro@gmail.com>
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gato-toolkit-0.1.0rc2/README.md` & `gato-toolkit-0.1.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `gato-toolkit-0.1.0rc2/setup.py` & `gato-toolkit-0.1.0rc3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def get_long_description():
     with open('README.md') as file:
         return file.read()
 
 
 setup(
     name="gato-toolkit",
-    version="0.1.0-rc2",
+    version="0.1.0-rc3",
     description="A toolkit for furthering research on AI alignment.",
     url="https://github.com/FyZyX/gato-toolkit",
     author="Lucas Lofaro <lucasmlofaro@gmail.com>",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     include_package_data=True,
     license='MIT',
```

### Comparing `gato-toolkit-0.1.0rc2/src/gato/.config/action-system-message.txt` & `gato-toolkit-0.1.0rc3/src/gato/.config/action-system-message.txt`

 * *Files identical despite different names*

### Comparing `gato-toolkit-0.1.0rc2/src/gato/.config/scenario-params/entropies.txt` & `gato-toolkit-0.1.0rc3/src/gato/.config/scenario-params/entropies.txt`

 * *Files identical despite different names*

### Comparing `gato-toolkit-0.1.0rc2/src/gato/.config/scenario-system-messages.txt` & `gato-toolkit-0.1.0rc3/src/gato/.config/scenario-system-messages.txt`

 * *Files identical despite different names*

### Comparing `gato-toolkit-0.1.0rc2/src/gato/entity.py` & `gato-toolkit-0.1.0rc3/src/gato/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import uuid
+
 from pydantic import BaseModel, Field
 
 
 class ScenarioParameters(BaseModel):
     random_word: str
     scope: str
     severity: str
```

### Comparing `gato-toolkit-0.1.0rc2/src/gato/generator.py` & `gato-toolkit-0.1.0rc3/src/gato/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import entity
-import llm
+from . import entity, llm
 
 
 class ScenarioGenerator:
 
     def __init__(self, model: llm.LLM, prompt: entity.ScenarioPrompt):
         self._model = model
         self._prompt = prompt
```

### Comparing `gato-toolkit-0.1.0rc2/src/gato/llm.py` & `gato-toolkit-0.1.0rc3/src/gato/llm.py`

 * *Files identical despite different names*

### Comparing `gato-toolkit-0.1.0rc2/src/gato/prompt.py` & `gato-toolkit-0.1.0rc3/src/gato/prompt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pathlib
 import random
 
-import entity
+from . import entity
 
 
 def read_file(path):
     with open(path, encoding="utf-8", errors="ignore") as file:
         return file.read()
```

### Comparing `gato-toolkit-0.1.0rc2/src/gato/service.py` & `gato-toolkit-0.1.0rc3/src/gato/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-import entity
-import generator
-import llm
-import prompt
+from . import entity, generator, llm, prompt
 
 
 class GatoService:
     _scenario_prompt_factory = prompt.ScenarioPromptFactory()
     _action_prompt_factory = prompt.ActionPromptFactory()
 
     def __init__(self, model: llm.LLM):
```

### Comparing `gato-toolkit-0.1.0rc2/src/gato_toolkit.egg-info/PKG-INFO` & `gato-toolkit-0.1.0rc3/src/gato_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gato-toolkit
-Version: 0.1.0rc2
+Version: 0.1.0rc3
 Summary: A toolkit for furthering research on AI alignment.
 Home-page: https://github.com/FyZyX/gato-toolkit
 Author: Lucas Lofaro <lucasmlofaro@gmail.com>
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gato-toolkit-0.1.0rc2/src/gato_toolkit.egg-info/SOURCES.txt` & `gato-toolkit-0.1.0rc3/src/gato_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*


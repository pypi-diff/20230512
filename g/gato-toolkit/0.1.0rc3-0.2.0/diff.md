# Comparing `tmp/gato-toolkit-0.1.0rc3.tar.gz` & `tmp/gato-toolkit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gato-toolkit-0.1.0rc3.tar", last modified: Fri May 12 07:04:29 2023, max compression
+gzip compressed data, was "gato-toolkit-0.2.0.tar", last modified: Fri May 12 09:51:41 2023, max compression
```

## Comparing `gato-toolkit-0.1.0rc3.tar` & `gato-toolkit-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 07:04:29.569273 gato-toolkit-0.1.0rc3/
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     1070 2023-05-11 12:21:41.000000 gato-toolkit-0.1.0rc3/LICENSE
--rw-r--r--   0 lucaslofaro   (501) staff       (20)       71 2023-05-12 04:29:48.000000 gato-toolkit-0.1.0rc3/MANIFEST.in
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     2261 2023-05-12 07:04:29.568751 gato-toolkit-0.1.0rc3/PKG-INFO
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     1773 2023-05-11 12:58:50.000000 gato-toolkit-0.1.0rc3/README.md
--rw-r--r--   0 lucaslofaro   (501) staff       (20)       38 2023-05-12 07:04:29.569351 gato-toolkit-0.1.0rc3/setup.cfg
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      888 2023-05-12 07:03:52.000000 gato-toolkit-0.1.0rc3/setup.py
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 07:04:29.562209 gato-toolkit-0.1.0rc3/src/
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 07:04:29.564316 gato-toolkit-0.1.0rc3/src/gato/
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 07:04:29.564733 gato-toolkit-0.1.0rc3/src/gato/.config/
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      677 2023-05-04 05:53:25.000000 gato-toolkit-0.1.0rc3/src/gato/.config/action-system-message.txt
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 07:04:29.567011 gato-toolkit-0.1.0rc3/src/gato/.config/scenario-params/
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      240 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc3/src/gato/.config/scenario-params/categories.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      160 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc3/src/gato/.config/scenario-params/domains.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)    22221 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc3/src/gato/.config/scenario-params/entropies.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      123 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc3/src/gato/.config/scenario-params/regions.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      271 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc3/src/gato/.config/scenario-params/scopes.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      134 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc3/src/gato/.config/scenario-params/severities.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     1577 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc3/src/gato/.config/scenario-system-messages.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)        0 2023-05-11 23:28:21.000000 gato-toolkit-0.1.0rc3/src/gato/__init__.py
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      574 2023-05-12 06:55:28.000000 gato-toolkit-0.1.0rc3/src/gato/entity.py
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     1216 2023-05-12 07:02:20.000000 gato-toolkit-0.1.0rc3/src/gato/generator.py
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     1470 2023-05-11 13:42:46.000000 gato-toolkit-0.1.0rc3/src/gato/llm.py
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     2233 2023-05-12 07:02:20.000000 gato-toolkit-0.1.0rc3/src/gato/prompt.py
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      764 2023-05-12 07:02:20.000000 gato-toolkit-0.1.0rc3/src/gato/service.py
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 07:04:29.568410 gato-toolkit-0.1.0rc3/src/gato_toolkit.egg-info/
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     2261 2023-05-12 07:04:29.000000 gato-toolkit-0.1.0rc3/src/gato_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      720 2023-05-12 07:04:29.000000 gato-toolkit-0.1.0rc3/src/gato_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)        1 2023-05-12 07:04:29.000000 gato-toolkit-0.1.0rc3/src/gato_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)       32 2023-05-12 07:04:29.000000 gato-toolkit-0.1.0rc3/src/gato_toolkit.egg-info/requires.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)        5 2023-05-12 07:04:29.000000 gato-toolkit-0.1.0rc3/src/gato_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 09:51:41.723868 gato-toolkit-0.2.0/
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     1070 2023-05-11 12:21:41.000000 gato-toolkit-0.2.0/LICENSE
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)       71 2023-05-12 04:29:48.000000 gato-toolkit-0.2.0/MANIFEST.in
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     2258 2023-05-12 09:51:41.723306 gato-toolkit-0.2.0/PKG-INFO
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     1773 2023-05-11 12:58:50.000000 gato-toolkit-0.2.0/README.md
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)       38 2023-05-12 09:51:41.723963 gato-toolkit-0.2.0/setup.cfg
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      884 2023-05-12 09:51:23.000000 gato-toolkit-0.2.0/setup.py
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 09:51:41.714201 gato-toolkit-0.2.0/src/
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 09:51:41.717156 gato-toolkit-0.2.0/src/gato/
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 09:51:41.717592 gato-toolkit-0.2.0/src/gato/.config/
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      677 2023-05-04 05:53:25.000000 gato-toolkit-0.2.0/src/gato/.config/action-system-message.txt
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 09:51:41.721042 gato-toolkit-0.2.0/src/gato/.config/scenario-params/
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      240 2023-05-04 05:53:23.000000 gato-toolkit-0.2.0/src/gato/.config/scenario-params/categories.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      160 2023-05-04 05:53:23.000000 gato-toolkit-0.2.0/src/gato/.config/scenario-params/domains.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)    22221 2023-05-04 05:53:23.000000 gato-toolkit-0.2.0/src/gato/.config/scenario-params/entropies.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      123 2023-05-04 05:53:23.000000 gato-toolkit-0.2.0/src/gato/.config/scenario-params/regions.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      271 2023-05-04 05:53:23.000000 gato-toolkit-0.2.0/src/gato/.config/scenario-params/scopes.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      134 2023-05-04 05:53:23.000000 gato-toolkit-0.2.0/src/gato/.config/scenario-params/severities.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     1577 2023-05-04 05:53:23.000000 gato-toolkit-0.2.0/src/gato/.config/scenario-system-messages.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)        0 2023-05-11 23:28:21.000000 gato-toolkit-0.2.0/src/gato/__init__.py
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      574 2023-05-12 06:55:28.000000 gato-toolkit-0.2.0/src/gato/entity.py
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     1216 2023-05-12 07:02:20.000000 gato-toolkit-0.2.0/src/gato/generator.py
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     1470 2023-05-11 13:42:46.000000 gato-toolkit-0.2.0/src/gato/llm.py
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     2071 2023-05-12 09:50:28.000000 gato-toolkit-0.2.0/src/gato/prompt.py
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     1247 2023-05-12 09:50:28.000000 gato-toolkit-0.2.0/src/gato/service.py
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 09:51:41.722979 gato-toolkit-0.2.0/src/gato_toolkit.egg-info/
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     2258 2023-05-12 09:51:41.000000 gato-toolkit-0.2.0/src/gato_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      720 2023-05-12 09:51:41.000000 gato-toolkit-0.2.0/src/gato_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)        1 2023-05-12 09:51:41.000000 gato-toolkit-0.2.0/src/gato_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)       32 2023-05-12 09:51:41.000000 gato-toolkit-0.2.0/src/gato_toolkit.egg-info/requires.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)        5 2023-05-12 09:51:41.000000 gato-toolkit-0.2.0/src/gato_toolkit.egg-info/top_level.txt
```

### Comparing `gato-toolkit-0.1.0rc3/LICENSE` & `gato-toolkit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gato-toolkit-0.1.0rc3/PKG-INFO` & `gato-toolkit-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gato-toolkit
-Version: 0.1.0rc3
+Version: 0.2.0
 Summary: A toolkit for furthering research on AI alignment.
 Home-page: https://github.com/FyZyX/gato-toolkit
 Author: Lucas Lofaro <lucasmlofaro@gmail.com>
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gato-toolkit-0.1.0rc3/README.md` & `gato-toolkit-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gato-toolkit-0.1.0rc3/setup.py` & `gato-toolkit-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def get_long_description():
     with open('README.md') as file:
         return file.read()
 
 
 setup(
     name="gato-toolkit",
-    version="0.1.0-rc3",
+    version="0.2.0",
     description="A toolkit for furthering research on AI alignment.",
     url="https://github.com/FyZyX/gato-toolkit",
     author="Lucas Lofaro <lucasmlofaro@gmail.com>",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     include_package_data=True,
     license='MIT',
```

### Comparing `gato-toolkit-0.1.0rc3/src/gato/.config/action-system-message.txt` & `gato-toolkit-0.2.0/src/gato/.config/action-system-message.txt`

 * *Files identical despite different names*

### Comparing `gato-toolkit-0.1.0rc3/src/gato/.config/scenario-params/entropies.txt` & `gato-toolkit-0.2.0/src/gato/.config/scenario-params/entropies.txt`

 * *Files identical despite different names*

### Comparing `gato-toolkit-0.1.0rc3/src/gato/.config/scenario-system-messages.txt` & `gato-toolkit-0.2.0/src/gato/.config/scenario-system-messages.txt`

 * *Files identical despite different names*

### Comparing `gato-toolkit-0.1.0rc3/src/gato/entity.py` & `gato-toolkit-0.2.0/src/gato/entity.py`

 * *Files identical despite different names*

### Comparing `gato-toolkit-0.1.0rc3/src/gato/generator.py` & `gato-toolkit-0.2.0/src/gato/generator.py`

 * *Files identical despite different names*

### Comparing `gato-toolkit-0.1.0rc3/src/gato/llm.py` & `gato-toolkit-0.2.0/src/gato/llm.py`

 * *Files identical despite different names*

### Comparing `gato-toolkit-0.1.0rc3/src/gato/prompt.py` & `gato-toolkit-0.2.0/src/gato/prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,49 +21,44 @@
         self._path = path
 
     def _get_random_parameter(self, name: str):
         path = self._base_dir / self._path / f"{name}.txt"
         choices = read_list(path)
         return random.choice(choices)
 
-    def random(self) -> entity.ScenarioParameters:
+    def new(self) -> entity.ScenarioParameters:
         return entity.ScenarioParameters(
             random_word=self._get_random_parameter("entropies"),
             scope=self._get_random_parameter("scopes"),
             severity=self._get_random_parameter("severities"),
             region=self._get_random_parameter("regions"),
             category=self._get_random_parameter("categories"),
             domain=self._get_random_parameter("domains"),
         )
 
 
 class ScenarioPromptFactory:
     _base_dir = pathlib.Path(__file__).parent
     _default_path = pathlib.Path(".config/scenario-system-messages.txt")
-    _parameters_factory = ScenarioParametersFactory()
 
-    def __init__(self,
-                 parameters: entity.ScenarioParameters = _parameters_factory.random(),
-                 path: pathlib.Path = _base_dir / _default_path):
-        self._parameters = parameters
-        self._system_message = random.choice(read_list(path))
+    def __init__(self, path: pathlib.Path = _base_dir / _default_path):
+        self._system_messages = read_list(path)
 
-    def new(self) -> entity.ScenarioPrompt:
+    def new(self, parameters: entity.ScenarioParameters) -> entity.ScenarioPrompt:
         return entity.ScenarioPrompt(
-            system_message=self._system_message,
-            parameters=self._parameters,
+            system_message=random.choice(self._system_messages),
+            parameters=parameters,
         )
 
 
 class ActionPromptFactory:
     _base_dir = pathlib.Path(__file__).parent
-    _default_path = pathlib.Path(".config/scenario-params")
+    _default_path = pathlib.Path(".config/action-system-message.txt")
 
-    def __init__(self, path: pathlib.Path = _default_path):
-        self._path = path
+    def __init__(self, path: pathlib.Path = _base_dir / _default_path):
+        self._system_message = read_file(path)
 
     def new(self, scenario: entity.Scenario) -> entity.ActionPrompt:
-        system_message = read_file(self._path)
         return entity.ActionPrompt(
-            system_message=system_message,
+            system_message=self._system_message,
             scenario=scenario,
         )
```

### Comparing `gato-toolkit-0.1.0rc3/src/gato_toolkit.egg-info/PKG-INFO` & `gato-toolkit-0.2.0/src/gato_toolkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gato-toolkit
-Version: 0.1.0rc3
+Version: 0.2.0
 Summary: A toolkit for furthering research on AI alignment.
 Home-page: https://github.com/FyZyX/gato-toolkit
 Author: Lucas Lofaro <lucasmlofaro@gmail.com>
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gato-toolkit-0.1.0rc3/src/gato_toolkit.egg-info/SOURCES.txt` & `gato-toolkit-0.2.0/src/gato_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*


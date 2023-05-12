# Comparing `tmp/gato-toolkit-0.1.0rc1.tar.gz` & `tmp/gato-toolkit-0.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gato-toolkit-0.1.0rc1.tar", last modified: Fri May 12 05:45:33 2023, max compression
+gzip compressed data, was "gato-toolkit-0.1.0rc2.tar", last modified: Fri May 12 06:45:17 2023, max compression
```

## Comparing `gato-toolkit-0.1.0rc1.tar` & `gato-toolkit-0.1.0rc2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 05:45:33.589437 gato-toolkit-0.1.0rc1/
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     1070 2023-05-11 12:21:41.000000 gato-toolkit-0.1.0rc1/LICENSE
--rw-r--r--   0 lucaslofaro   (501) staff       (20)       71 2023-05-12 04:29:48.000000 gato-toolkit-0.1.0rc1/MANIFEST.in
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     2261 2023-05-12 05:45:33.589218 gato-toolkit-0.1.0rc1/PKG-INFO
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     1773 2023-05-11 12:58:50.000000 gato-toolkit-0.1.0rc1/README.md
--rw-r--r--   0 lucaslofaro   (501) staff       (20)       38 2023-05-12 05:45:33.589520 gato-toolkit-0.1.0rc1/setup.cfg
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      860 2023-05-12 04:08:21.000000 gato-toolkit-0.1.0rc1/setup.py
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 05:45:33.580751 gato-toolkit-0.1.0rc1/src/
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 05:45:33.584174 gato-toolkit-0.1.0rc1/src/gato/
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 05:45:33.585157 gato-toolkit-0.1.0rc1/src/gato/.config/
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      677 2023-05-04 05:53:25.000000 gato-toolkit-0.1.0rc1/src/gato/.config/action-system-message.txt
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 05:45:33.587740 gato-toolkit-0.1.0rc1/src/gato/.config/scenario-params/
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      240 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc1/src/gato/.config/scenario-params/categories.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      160 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc1/src/gato/.config/scenario-params/domains.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)    22221 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc1/src/gato/.config/scenario-params/entropies.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      123 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc1/src/gato/.config/scenario-params/regions.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      271 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc1/src/gato/.config/scenario-params/scopes.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      134 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc1/src/gato/.config/scenario-params/severities.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     1577 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc1/src/gato/.config/scenario-system-messages.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)        0 2023-05-11 23:28:21.000000 gato-toolkit-0.1.0rc1/src/gato/__init__.py
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      573 2023-05-11 12:46:27.000000 gato-toolkit-0.1.0rc1/src/gato/entity.py
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     1215 2023-05-12 00:47:38.000000 gato-toolkit-0.1.0rc1/src/gato/generator.py
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     1470 2023-05-11 13:42:46.000000 gato-toolkit-0.1.0rc1/src/gato/llm.py
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     2226 2023-05-12 00:47:38.000000 gato-toolkit-0.1.0rc1/src/gato/prompt.py
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      775 2023-05-12 00:47:38.000000 gato-toolkit-0.1.0rc1/src/gato/service.py
-drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 05:45:33.588908 gato-toolkit-0.1.0rc1/src/gato_toolkit.egg-info/
--rw-r--r--   0 lucaslofaro   (501) staff       (20)     2261 2023-05-12 05:45:33.000000 gato-toolkit-0.1.0rc1/src/gato_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 lucaslofaro   (501) staff       (20)      720 2023-05-12 05:45:33.000000 gato-toolkit-0.1.0rc1/src/gato_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)        1 2023-05-12 05:45:33.000000 gato-toolkit-0.1.0rc1/src/gato_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)       15 2023-05-12 05:45:33.000000 gato-toolkit-0.1.0rc1/src/gato_toolkit.egg-info/requires.txt
--rw-r--r--   0 lucaslofaro   (501) staff       (20)        5 2023-05-12 05:45:33.000000 gato-toolkit-0.1.0rc1/src/gato_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 06:45:17.002783 gato-toolkit-0.1.0rc2/
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     1070 2023-05-11 12:21:41.000000 gato-toolkit-0.1.0rc2/LICENSE
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)       71 2023-05-12 04:29:48.000000 gato-toolkit-0.1.0rc2/MANIFEST.in
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     2261 2023-05-12 06:45:17.002144 gato-toolkit-0.1.0rc2/PKG-INFO
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     1773 2023-05-11 12:58:50.000000 gato-toolkit-0.1.0rc2/README.md
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)       38 2023-05-12 06:45:17.002982 gato-toolkit-0.1.0rc2/setup.cfg
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      888 2023-05-12 06:45:11.000000 gato-toolkit-0.1.0rc2/setup.py
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 06:45:16.995939 gato-toolkit-0.1.0rc2/src/
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 06:45:16.998183 gato-toolkit-0.1.0rc2/src/gato/
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 06:45:16.998727 gato-toolkit-0.1.0rc2/src/gato/.config/
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      677 2023-05-04 05:53:25.000000 gato-toolkit-0.1.0rc2/src/gato/.config/action-system-message.txt
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 06:45:17.000247 gato-toolkit-0.1.0rc2/src/gato/.config/scenario-params/
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      240 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc2/src/gato/.config/scenario-params/categories.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      160 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc2/src/gato/.config/scenario-params/domains.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)    22221 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc2/src/gato/.config/scenario-params/entropies.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      123 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc2/src/gato/.config/scenario-params/regions.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      271 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc2/src/gato/.config/scenario-params/scopes.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      134 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc2/src/gato/.config/scenario-params/severities.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     1577 2023-05-04 05:53:23.000000 gato-toolkit-0.1.0rc2/src/gato/.config/scenario-system-messages.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)        0 2023-05-11 23:28:21.000000 gato-toolkit-0.1.0rc2/src/gato/__init__.py
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      573 2023-05-11 12:46:27.000000 gato-toolkit-0.1.0rc2/src/gato/entity.py
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     1215 2023-05-12 00:47:38.000000 gato-toolkit-0.1.0rc2/src/gato/generator.py
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     1470 2023-05-11 13:42:46.000000 gato-toolkit-0.1.0rc2/src/gato/llm.py
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     2226 2023-05-12 00:47:38.000000 gato-toolkit-0.1.0rc2/src/gato/prompt.py
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      775 2023-05-12 00:47:38.000000 gato-toolkit-0.1.0rc2/src/gato/service.py
+drwxr-xr-x   0 lucaslofaro   (501) staff       (20)        0 2023-05-12 06:45:17.001693 gato-toolkit-0.1.0rc2/src/gato_toolkit.egg-info/
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)     2261 2023-05-12 06:45:16.000000 gato-toolkit-0.1.0rc2/src/gato_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)      720 2023-05-12 06:45:16.000000 gato-toolkit-0.1.0rc2/src/gato_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)        1 2023-05-12 06:45:16.000000 gato-toolkit-0.1.0rc2/src/gato_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)       32 2023-05-12 06:45:16.000000 gato-toolkit-0.1.0rc2/src/gato_toolkit.egg-info/requires.txt
+-rw-r--r--   0 lucaslofaro   (501) staff       (20)        5 2023-05-12 06:45:16.000000 gato-toolkit-0.1.0rc2/src/gato_toolkit.egg-info/top_level.txt
```

### Comparing `gato-toolkit-0.1.0rc1/LICENSE` & `gato-toolkit-0.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `gato-toolkit-0.1.0rc1/PKG-INFO` & `gato-toolkit-0.1.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gato-toolkit
-Version: 0.1.0rc1
+Version: 0.1.0rc2
 Summary: A toolkit for furthering research on AI alignment.
 Home-page: https://github.com/FyZyX/gato-toolkit
 Author: Lucas Lofaro <lucasmlofaro@gmail.com>
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gato-toolkit-0.1.0rc1/README.md` & `gato-toolkit-0.1.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `gato-toolkit-0.1.0rc1/setup.py` & `gato-toolkit-0.1.0rc2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def get_long_description():
     with open('README.md') as file:
         return file.read()
 
 
 setup(
     name="gato-toolkit",
-    version="0.1.0-rc1",
+    version="0.1.0-rc2",
     description="A toolkit for furthering research on AI alignment.",
     url="https://github.com/FyZyX/gato-toolkit",
     author="Lucas Lofaro <lucasmlofaro@gmail.com>",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     include_package_data=True,
     license='MIT',
@@ -22,9 +22,10 @@
         'Development Status :: 2 - Pre-Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.10',
     ],
     install_requires=[
         "openai>=0.27.6",
+        "pydantic>=1.10.7",
     ],
 )
```

### Comparing `gato-toolkit-0.1.0rc1/src/gato/.config/action-system-message.txt` & `gato-toolkit-0.1.0rc2/src/gato/.config/action-system-message.txt`

 * *Files identical despite different names*

### Comparing `gato-toolkit-0.1.0rc1/src/gato/.config/scenario-params/entropies.txt` & `gato-toolkit-0.1.0rc2/src/gato/.config/scenario-params/entropies.txt`

 * *Files identical despite different names*

### Comparing `gato-toolkit-0.1.0rc1/src/gato/.config/scenario-system-messages.txt` & `gato-toolkit-0.1.0rc2/src/gato/.config/scenario-system-messages.txt`

 * *Files identical despite different names*

### Comparing `gato-toolkit-0.1.0rc1/src/gato/entity.py` & `gato-toolkit-0.1.0rc2/src/gato/entity.py`

 * *Files identical despite different names*

### Comparing `gato-toolkit-0.1.0rc1/src/gato/generator.py` & `gato-toolkit-0.1.0rc2/src/gato/generator.py`

 * *Files identical despite different names*

### Comparing `gato-toolkit-0.1.0rc1/src/gato/llm.py` & `gato-toolkit-0.1.0rc2/src/gato/llm.py`

 * *Files identical despite different names*

### Comparing `gato-toolkit-0.1.0rc1/src/gato/prompt.py` & `gato-toolkit-0.1.0rc2/src/gato/prompt.py`

 * *Files identical despite different names*

### Comparing `gato-toolkit-0.1.0rc1/src/gato/service.py` & `gato-toolkit-0.1.0rc2/src/gato/service.py`

 * *Files identical despite different names*

### Comparing `gato-toolkit-0.1.0rc1/src/gato_toolkit.egg-info/PKG-INFO` & `gato-toolkit-0.1.0rc2/src/gato_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gato-toolkit
-Version: 0.1.0rc1
+Version: 0.1.0rc2
 Summary: A toolkit for furthering research on AI alignment.
 Home-page: https://github.com/FyZyX/gato-toolkit
 Author: Lucas Lofaro <lucasmlofaro@gmail.com>
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gato-toolkit-0.1.0rc1/src/gato_toolkit.egg-info/SOURCES.txt` & `gato-toolkit-0.1.0rc2/src/gato_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*


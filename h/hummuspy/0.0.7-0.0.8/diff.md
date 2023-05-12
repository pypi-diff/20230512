# Comparing `tmp/hummuspy-0.0.7.tar.gz` & `tmp/hummuspy-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hummuspy-0.0.7.tar", max compression
+gzip compressed data, was "hummuspy-0.0.8.tar", max compression
```

## Comparing `hummuspy-0.0.7.tar` & `hummuspy-0.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-04-04 11:48:19.958459 hummuspy-0.0.7/LICENSE
--rw-r--r--   0        0        0       46 2023-04-04 12:00:32.696076 hummuspy-0.0.7/README.md
--rw-r--r--   0        0        0      585 2023-05-12 08:50:29.364469 hummuspy-0.0.7/pyproject.toml
--rw-r--r--   0        0        0    37274 2023-04-05 16:53:37.048925 hummuspy-0.0.7/src/hummuspy/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0     6051 2023-04-05 17:15:37.384728 hummuspy-0.0.7/src/hummuspy/Untitled.ipynb
--rw-r--r--   0        0        0        0 2023-04-04 12:51:39.859533 hummuspy-0.0.7/src/hummuspy/__init__.py
--rw-r--r--   0        0        0     3458 2023-05-12 08:50:20.372094 hummuspy-0.0.7/src/hummuspy/config.py
--rw-r--r--   0        0        0       42 2023-04-04 12:58:18.183124 hummuspy-0.0.7/src/hummuspy/example.py
--rw-r--r--   0        0        0    15206 2023-05-08 09:02:31.288706 hummuspy-0.0.7/src/hummuspy/explore_network.py
--rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 hummuspy-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-04 11:48:19.958459 hummuspy-0.0.8/LICENSE
+-rw-r--r--   0        0        0       46 2023-04-04 12:00:32.696076 hummuspy-0.0.8/README.md
+-rw-r--r--   0        0        0      585 2023-05-12 09:09:54.803847 hummuspy-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    37274 2023-04-05 16:53:37.048925 hummuspy-0.0.8/src/hummuspy/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0     6051 2023-04-05 17:15:37.384728 hummuspy-0.0.8/src/hummuspy/Untitled.ipynb
+-rw-r--r--   0        0        0        0 2023-04-04 12:51:39.859533 hummuspy-0.0.8/src/hummuspy/__init__.py
+-rw-r--r--   0        0        0     3482 2023-05-12 09:09:17.352476 hummuspy-0.0.8/src/hummuspy/config.py
+-rw-r--r--   0        0        0       42 2023-04-04 12:58:18.183124 hummuspy-0.0.8/src/hummuspy/example.py
+-rw-r--r--   0        0        0    15206 2023-05-08 09:02:31.288706 hummuspy-0.0.8/src/hummuspy/explore_network.py
+-rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 hummuspy-0.0.8/PKG-INFO
```

### Comparing `hummuspy-0.0.7/pyproject.toml` & `hummuspy-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hummuspy"
-version = "0.0.7"
+version = "0.0.8"
 description = "HuMMuS is a novel method for the inference of regulatory mechanisms from multi-omics data with any type and number of omics, thorugh a heterogeneous multilayer networks framework."
 authors = ["Rémi Trimbour <remi.trimbour@pasteur.fr>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
```

### Comparing `hummuspy-0.0.7/src/hummuspy/.ipynb_checkpoints/Untitled-checkpoint.ipynb` & `hummuspy-0.0.8/src/hummuspy/.ipynb_checkpoints/Untitled-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `hummuspy-0.0.7/src/hummuspy/Untitled.ipynb` & `hummuspy-0.0.8/src/hummuspy/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `hummuspy-0.0.7/src/hummuspy/config.py` & `hummuspy-0.0.8/src/hummuspy/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 def general_config(
     multiplexes: typing.Union[dict[dict[str]]],
     bipartites: typing.Union[str, list[str], dict[str]],
     seed_path: str = 'seeds/seeds.txt',
     folder_multiplexes = 'multiplex',
     folder_bipartites = 'bipartite',
-    bipartite_type: typing.Union[str, list[str], dict[str]] = 'undirected',
+    bipartites_type: typing.Union[str, list[str], dict[str]] = 'undirected',
     self_loops = 0,
     restart_prob = 0.7,):
     
     """Create a very general config file for the hummus pipeline."""
     config = dict()
     config['multiplex'] = dict()
     config['bipartite'] = dict()
@@ -60,35 +60,36 @@
     config['self_loops'] = self_loops
 
     # We add the multiplexes to the config
     for multiplex_name in multiplexes:
         # If folder_multiplexes is None we use the multiplex name as folder name
         config['multiplex'][multiplex_name] = dict()
         config['multiplex'][multiplex_name]['layers'] =\
-            [(folder_multiplexes+'/'+multiplex_name+'/'+layer).replace('//', '/') for layer in multiplexes[multiplex_name]['layers']]
+            [(folder_multiplexes+'/'+multiplex_name+'/'+layer).replace('//', '/')
+              for layer in multiplexes[multiplex_name]['layers']]
         config['multiplex'][multiplex_name]['graph_type'] =\
             multiplexes[multiplex_name]['graph_type']
         
 
     # if type of bipartites not associated to their names already,
     # we create a dict with the same order as the bipartites
-    bipartite_type = make_values_list(bipartite_type)
+    bipartite_type = make_values_list(bipartites_type)
     if type(bipartite_type) == list:
         temp = dict()
         for i in range(len(bipartites)):
-            temp[bipartites.keys()[i]] = bipartite_type[i]
+            temp[list(bipartites.keys())[i]] = bipartites_type[i]
         bipartite_type = temp
 
     # we add the bipartites
     for bipartite in bipartites:
         bipartite_loc = folder_bipartites+'/'+bipartite
         config['bipartite'][bipartite_loc] = dict()
         config['bipartite'][bipartite_loc]['source'] = bipartites[bipartite]['multiplex_left']
         config['bipartite'][bipartite_loc]['target'] = bipartites[bipartite]['multiplex_right']
-        config['bipartite'][bipartite_loc]['graph_type'] = bipartite_type[bipartite]
+        config['bipartite'][bipartite_loc]['graph_type'] = bipartites_type[bipartite]
 
     config['r'] = restart_prob
     return config
 
 def save_config(config, filename):
     with open(filename, 'w') as f:
         yaml.dump(config, f)
```

### Comparing `hummuspy-0.0.7/src/hummuspy/explore_network.py` & `hummuspy-0.0.8/src/hummuspy/explore_network.py`

 * *Files identical despite different names*

### Comparing `hummuspy-0.0.7/PKG-INFO` & `hummuspy-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hummuspy
-Version: 0.0.7
+Version: 0.0.8
 Summary: HuMMuS is a novel method for the inference of regulatory mechanisms from multi-omics data with any type and number of omics, thorugh a heterogeneous multilayer networks framework.
 License: GPL-3.0-only
 Author: Rémi Trimbour
 Author-email: remi.trimbour@pasteur.fr
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```


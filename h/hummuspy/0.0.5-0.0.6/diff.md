# Comparing `tmp/hummuspy-0.0.5.tar.gz` & `tmp/hummuspy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hummuspy-0.0.5.tar", max compression
+gzip compressed data, was "hummuspy-0.0.6.tar", max compression
```

## Comparing `hummuspy-0.0.5.tar` & `hummuspy-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-04-04 11:48:19.958459 hummuspy-0.0.5/LICENSE
--rw-r--r--   0        0        0       46 2023-04-04 12:00:32.696076 hummuspy-0.0.5/README.md
--rw-r--r--   0        0        0      585 2023-05-08 11:45:57.232054 hummuspy-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    37274 2023-04-05 16:53:37.048925 hummuspy-0.0.5/src/hummuspy/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0     6051 2023-04-05 17:15:37.384728 hummuspy-0.0.5/src/hummuspy/Untitled.ipynb
--rw-r--r--   0        0        0        0 2023-04-04 12:51:39.859533 hummuspy-0.0.5/src/hummuspy/__init__.py
--rw-r--r--   0        0        0     3627 2023-05-08 11:39:34.811147 hummuspy-0.0.5/src/hummuspy/config.py
--rw-r--r--   0        0        0       42 2023-04-04 12:58:18.183124 hummuspy-0.0.5/src/hummuspy/example.py
--rw-r--r--   0        0        0    15206 2023-05-08 09:02:31.288706 hummuspy-0.0.5/src/hummuspy/explore_network.py
--rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 hummuspy-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-04 11:48:19.958459 hummuspy-0.0.6/LICENSE
+-rw-r--r--   0        0        0       46 2023-04-04 12:00:32.696076 hummuspy-0.0.6/README.md
+-rw-r--r--   0        0        0      585 2023-05-12 08:44:59.813124 hummuspy-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    37274 2023-04-05 16:53:37.048925 hummuspy-0.0.6/src/hummuspy/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0     6051 2023-04-05 17:15:37.384728 hummuspy-0.0.6/src/hummuspy/Untitled.ipynb
+-rw-r--r--   0        0        0        0 2023-04-04 12:51:39.859533 hummuspy-0.0.6/src/hummuspy/__init__.py
+-rw-r--r--   0        0        0     3432 2023-05-12 08:43:20.935579 hummuspy-0.0.6/src/hummuspy/config.py
+-rw-r--r--   0        0        0       42 2023-04-04 12:58:18.183124 hummuspy-0.0.6/src/hummuspy/example.py
+-rw-r--r--   0        0        0    15206 2023-05-08 09:02:31.288706 hummuspy-0.0.6/src/hummuspy/explore_network.py
+-rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 hummuspy-0.0.6/PKG-INFO
```

### Comparing `hummuspy-0.0.5/pyproject.toml` & `hummuspy-0.0.6/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hummuspy"
-version = "0.0.5"
+version = "0.0.6"
 description = "HuMMuS is a novel method for the inference of regulatory mechanisms from multi-omics data with any type and number of omics, thorugh a heterogeneous multilayer networks framework."
 authors = ["Rémi Trimbour <remi.trimbour@pasteur.fr>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
```

### Comparing `hummuspy-0.0.5/src/hummuspy/.ipynb_checkpoints/Untitled-checkpoint.ipynb` & `hummuspy-0.0.6/src/hummuspy/.ipynb_checkpoints/Untitled-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `hummuspy-0.0.5/src/hummuspy/Untitled.ipynb` & `hummuspy-0.0.6/src/hummuspy/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `hummuspy-0.0.5/src/hummuspy/config.py` & `hummuspy-0.0.6/src/hummuspy/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,31 +18,28 @@
     
 def group_per_layer(
         multiplex_list
         ):
     """Group multiplex info per layer.
     
     Structure returned:
-    {multiplex_name: {'layers': [layer1, layer2, ...],
-                      'graph_type': [graph_type1, graph_type2, ...]}
-     ...}
+    {multiplex1: [layer1, layer2, ...],
+     multiplex2: [layer1, layer2, ...]}
     
     """
     multiplex_organised = dict()
-    for multiplex_name in list(multiplex_list['networks'].keys()):
+    for multiplex_name in multiplex_list:
         # we instanciata a dict for each multiplex network
         multiplex_organised[multiplex_name] = dict()
         # we add the layer names
         multiplex_organised[multiplex_name]['layers'] =\
-            [layer for layer in multiplex_list['networks'][network_name]]
+            [layer for layer in multiplex_list[multiplex_name]]
         # we add the graph type
         multiplex_organised[multiplex_name]['graph_type'] =\
-            [str(int(directed))+str(int(weighted)) for directed, weighted in\
-             zip(multiplex_list['directed'][multiplex_name],\
-                 multiplex_list['weighted'][multiplex_name])]
+            [multiplex_list[multiplex_name][layer] for layer in multiplex_list[multiplex_name]]
     return multiplex_organised
 
 
 
 
 def general_config(
     multiplexes: typing.Union[dict[dict[str]]],
```

### Comparing `hummuspy-0.0.5/src/hummuspy/explore_network.py` & `hummuspy-0.0.6/src/hummuspy/explore_network.py`

 * *Files identical despite different names*

### Comparing `hummuspy-0.0.5/PKG-INFO` & `hummuspy-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hummuspy
-Version: 0.0.5
+Version: 0.0.6
 Summary: HuMMuS is a novel method for the inference of regulatory mechanisms from multi-omics data with any type and number of omics, thorugh a heterogeneous multilayer networks framework.
 License: GPL-3.0-only
 Author: Rémi Trimbour
 Author-email: remi.trimbour@pasteur.fr
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```


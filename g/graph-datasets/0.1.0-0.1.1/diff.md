# Comparing `tmp/graph_datasets-0.1.0.tar.gz` & `tmp/graph_datasets-0.1.1.tar.gz`

## Comparing `graph_datasets-0.1.0.tar` & `graph_datasets-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/.editorconfig
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    17935 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/.pylintrc
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/requirements-dev.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/requirements.txt
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/.vscode/extensions.json
--rw-r--r--   0        0        0    56106 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/configs/nb.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/demos/demo.ipynb
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/docs/Makefile
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/docs/conf.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/docs/make.bat
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/docs/rst/data_info.rst
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/docs/rst/load_data.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/docs/rst/src.utils.rst
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/docs/tpls/module.rst_t
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/docs/tpls/package.rst_t
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/docs/tpls/toc.rst_t
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/graph_datasets/__init__.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/graph_datasets/data_info.py
--rw-r--r--   0        0        0    27864 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/graph_datasets/load_data.py
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/graph_datasets/utils/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/scripts/build-publish.sh
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/scripts/bump.sh
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/scripts/cuda.sh
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/scripts/docs.sh
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/scripts/install-dev.sh
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/scripts/install.sh
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/scripts/nb.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/tests/test.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/.gitignore
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/README.md
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 graph_datasets-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/.editorconfig
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    17935 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/.pylintrc
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/requirements-dev.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/requirements.txt
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/.vscode/extensions.json
+-rw-r--r--   0        0        0    56106 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/configs/nb.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/demos/demo.ipynb
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/docs/make.bat
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/docs/rst/data_info.rst
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/docs/rst/load_data.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/docs/rst/src.utils.rst
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/docs/tpls/module.rst_t
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/docs/tpls/package.rst_t
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/docs/tpls/toc.rst_t
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/graph_datasets/__init__.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/graph_datasets/data_info.py
+-rw-r--r--   0        0        0    27860 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/graph_datasets/load_data.py
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/graph_datasets/utils/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/scripts/build-publish.sh
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/scripts/bump.sh
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/scripts/cuda.sh
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/scripts/docs.sh
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/scripts/install-dev.sh
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/scripts/install.sh
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/scripts/nb.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/tests/test.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/.gitignore
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/README.md
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/PKG-INFO
```

### Comparing `graph_datasets-0.1.0/.pre-commit-config.yaml` & `graph_datasets-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.0/.pylintrc` & `graph_datasets-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.0/.github/workflows/release.yml` & `graph_datasets-0.1.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.0/configs/nb.py` & `graph_datasets-0.1.1/configs/nb.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.0/demos/demo.ipynb` & `graph_datasets-0.1.1/demos/demo.ipynb`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.0/docs/Makefile` & `graph_datasets-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.0/docs/conf.py` & `graph_datasets-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.0/docs/index.rst` & `graph_datasets-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.0/docs/make.bat` & `graph_datasets-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.0/docs/tpls/package.rst_t` & `graph_datasets-0.1.1/docs/tpls/package.rst_t`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.0/graph_datasets/data_info.py` & `graph_datasets-0.1.1/graph_datasets/data_info.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.0/graph_datasets/load_data.py` & `graph_datasets-0.1.1/graph_datasets/load_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,15 +252,15 @@
         "wisconsin": "WisconsinDataset",
     }
 
     if dataset_name in ["cora", "citeseer", "pubmed"]:
         dataset = getattr(dgl.data, dataset_map[dataset_name])(
             raw_dir=directory,
             force_reload=False,
-            verbosity=False,
+            verbose=False,
             transform=None,
             reverse_edge=False,
             reorder=False,
         )
     elif dataset_name in [
             "chameleon",
             "squirrel",
@@ -270,15 +270,15 @@
             "wisconsin",
             "corafull",
             "reddit",
     ]:
         dataset = getattr(dgl.data, dataset_map[dataset_name])(
             raw_dir=directory,
             force_reload=False,
-            verbosity=False,
+            verbose=False,
             transform=None,
         )
     else:
         raise NotImplementedError(f"load_dgl_data does not support {dataset_name}.")
 
     graph = dataset[0]
```

### Comparing `graph_datasets-0.1.0/graph_datasets/utils/__init__.py` & `graph_datasets-0.1.1/graph_datasets/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.0/scripts/cuda.sh` & `graph_datasets-0.1.1/scripts/cuda.sh`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.0/scripts/install.sh` & `graph_datasets-0.1.1/scripts/install.sh`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.0/tests/test.py` & `graph_datasets-0.1.1/tests/test.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Test
 """
+# pylint:disable=duplicate-code
 import argparse
 
-from graph_datasets.load_data import load_data
+from graph_datasets import load_data
 
 
 def main():
     parser = argparse.ArgumentParser(
         prog="Load Graph datasets",
         description="Load Graph datasets",
     )
```

### Comparing `graph_datasets-0.1.0/.gitignore` & `graph_datasets-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.0/README.md` & `graph_datasets-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.0/pyproject.toml` & `graph_datasets-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "graph_datasets"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{ name = "galo.gm", email = "galo.gm.work@gmail.com" }]
 keywords = ["graph", "datasets"]
 description = "Load graph datasets."
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
-    "torch>=1.21.1",
-    "torch-geometric>=2.3.1",
-    "torchaudio>=0.12.1",
-    "torchvision>=0.13.1",
-    "dgl>=1.1.0",
+    "torch>=1.10.2",
+    "torch-geometric>=2.0.3",
+    "torchaudio>=0.10.2",
+    "torchvision>=0.11.3",
+    "dgl>=0.9.0",
     "dglgo>=0.0.2",
-    "gdown>=4.7.1",
+    "gdown>=4.7",
     "wget>=3.2",
-    "texttable>=1.6.7",
+    "texttable>=1.6",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/galogm/graph_datasets"
 "Bug Tracker" = "https://github.com/galogm/graph_datasets/issues"
```

### Comparing `graph_datasets-0.1.0/PKG-INFO` & `graph_datasets-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: graph_datasets
-Version: 0.1.0
+Version: 0.1.1
 Summary: Load graph datasets.
 Project-URL: Homepage, https://github.com/galogm/graph_datasets
 Project-URL: Bug Tracker, https://github.com/galogm/graph_datasets/issues
 Author-email: "galo.gm" <galo.gm.work@gmail.com>
 License-Expression: MIT
 Keywords: datasets,graph
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
-Requires-Dist: dgl>=1.1.0
+Requires-Dist: dgl>=0.9.0
 Requires-Dist: dglgo>=0.0.2
-Requires-Dist: gdown>=4.7.1
-Requires-Dist: texttable>=1.6.7
-Requires-Dist: torch-geometric>=2.3.1
-Requires-Dist: torch>=1.21.1
-Requires-Dist: torchaudio>=0.12.1
-Requires-Dist: torchvision>=0.13.1
+Requires-Dist: gdown>=4.7
+Requires-Dist: texttable>=1.6
+Requires-Dist: torch-geometric>=2.0.3
+Requires-Dist: torch>=1.10.2
+Requires-Dist: torchaudio>=0.10.2
+Requires-Dist: torchvision>=0.11.3
 Requires-Dist: wget>=3.2
 Description-Content-Type: text/markdown
 
 # Template
 
 ## Installation
```


# Comparing `tmp/graph_datasets-0.1.1.tar.gz` & `tmp/graph_datasets-0.1.2.tar.gz`

## Comparing `graph_datasets-0.1.1.tar` & `graph_datasets-0.1.2.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/.editorconfig
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    17935 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/.pylintrc
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/requirements-dev.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/requirements.txt
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/.github/workflows/release.yml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/.vscode/extensions.json
--rw-r--r--   0        0        0    56106 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/configs/nb.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/demos/demo.ipynb
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/docs/Makefile
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/docs/conf.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/docs/make.bat
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/docs/rst/data_info.rst
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/docs/rst/load_data.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/docs/rst/src.utils.rst
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/docs/tpls/module.rst_t
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/docs/tpls/package.rst_t
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/docs/tpls/toc.rst_t
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/graph_datasets/__init__.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/graph_datasets/data_info.py
--rw-r--r--   0        0        0    27860 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/graph_datasets/load_data.py
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/graph_datasets/utils/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/scripts/build-publish.sh
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/scripts/bump.sh
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/scripts/cuda.sh
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/scripts/docs.sh
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/scripts/install-dev.sh
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/scripts/install.sh
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/scripts/nb.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/tests/test.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/.gitignore
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/README.md
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 graph_datasets-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/.editorconfig
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    17935 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/.pylintrc
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/requirements-dev.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/requirements.txt
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/.vscode/extensions.json
+-rw-r--r--   0        0        0    56106 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/configs/nb.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/demos/demo.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/docs/Makefile
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/docs/conf.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/docs/make.bat
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/docs/rst/data_info.rst
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/docs/rst/load_data.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/docs/rst/src.utils.rst
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/docs/tpls/module.rst_t
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/docs/tpls/package.rst_t
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/docs/tpls/toc.rst_t
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/graph_datasets/__init__.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/graph_datasets/data_info.py
+-rw-r--r--   0        0        0    27860 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/graph_datasets/load_data.py
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/graph_datasets/utils/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/scripts/build-publish.sh
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/scripts/bump.sh
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/scripts/cuda.sh
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/scripts/docs.sh
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/scripts/install-dev.sh
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/scripts/install.sh
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/scripts/nb.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/tests/test.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/LICENSE
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/README.md
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/PKG-INFO
```

### Comparing `graph_datasets-0.1.1/.pre-commit-config.yaml` & `graph_datasets-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.1/.pylintrc` & `graph_datasets-0.1.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.1/.github/workflows/release.yml` & `graph_datasets-0.1.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.1/configs/nb.py` & `graph_datasets-0.1.2/configs/nb.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.1/docs/Makefile` & `graph_datasets-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.1/docs/conf.py` & `graph_datasets-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.1/docs/index.rst` & `graph_datasets-0.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.1/docs/make.bat` & `graph_datasets-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.1/docs/tpls/package.rst_t` & `graph_datasets-0.1.2/docs/tpls/package.rst_t`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.1/graph_datasets/data_info.py` & `graph_datasets-0.1.2/graph_datasets/data_info.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.1/graph_datasets/load_data.py` & `graph_datasets-0.1.2/graph_datasets/load_data.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.1/graph_datasets/utils/__init__.py` & `graph_datasets-0.1.2/graph_datasets/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.1/scripts/cuda.sh` & `graph_datasets-0.1.2/scripts/cuda.sh`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.1/scripts/install.sh` & `graph_datasets-0.1.2/scripts/install.sh`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.1/tests/test.py` & `graph_datasets-0.1.2/tests/test.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.1/.gitignore` & `graph_datasets-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.1/README.md` & `graph_datasets-0.1.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-# Template
+# Graph Datasets
+
+<div align="center">
+
+[![PYPI](https://img.shields.io/pypi/v/graph_datasets?style=flat)](https://pypi.org/project/graph-datasets/)  [![Latest Release](https://img.shields.io/github/v/tag/galogm/graph_datasets)](https://github.com/galogm/graph_datasets/tags)
+
+</div>
 
 ## Installation
 
 ```sh
 $ python -m pip install graph_datasets
 ```
```

### Comparing `graph_datasets-0.1.1/pyproject.toml` & `graph_datasets-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "graph_datasets"
-version = "0.1.1"
+version = "0.1.2"
 authors = [{ name = "galo.gm", email = "galo.gm.work@gmail.com" }]
 keywords = ["graph", "datasets"]
 description = "Load graph datasets."
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `graph_datasets-0.1.1/PKG-INFO` & `graph_datasets-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: graph_datasets
-Version: 0.1.1
+Version: 0.1.2
 Summary: Load graph datasets.
 Project-URL: Homepage, https://github.com/galogm/graph_datasets
 Project-URL: Bug Tracker, https://github.com/galogm/graph_datasets/issues
 Author-email: "galo.gm" <galo.gm.work@gmail.com>
 License-Expression: MIT
+License-File: LICENSE
 Keywords: datasets,graph
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Requires-Dist: dgl>=0.9.0
 Requires-Dist: dglgo>=0.0.2
@@ -18,15 +19,21 @@
 Requires-Dist: torch-geometric>=2.0.3
 Requires-Dist: torch>=1.10.2
 Requires-Dist: torchaudio>=0.10.2
 Requires-Dist: torchvision>=0.11.3
 Requires-Dist: wget>=3.2
 Description-Content-Type: text/markdown
 
-# Template
+# Graph Datasets
+
+<div align="center">
+
+[![PYPI](https://img.shields.io/pypi/v/graph_datasets?style=flat)](https://pypi.org/project/graph-datasets/)  [![Latest Release](https://img.shields.io/github/v/tag/galogm/graph_datasets)](https://github.com/galogm/graph_datasets/tags)
+
+</div>
 
 ## Installation
 
 ```sh
 $ python -m pip install graph_datasets
 ```
```


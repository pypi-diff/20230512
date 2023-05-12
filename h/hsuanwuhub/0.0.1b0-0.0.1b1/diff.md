# Comparing `tmp/hsuanwuhub-0.0.1b0.tar.gz` & `tmp/hsuanwuhub-0.0.1b1.tar.gz`

## Comparing `hsuanwuhub-0.0.1b0.tar` & `hsuanwuhub-0.0.1b1.tar`

### file list

```diff
@@ -1,14 +1,24 @@
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b0/CNAME
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b0/CONTRIBUTING.md
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b0/Makefile
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b0/index.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b0/hsuanwuhub/__init__.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b0/hsuanwuhub/datasets/__init__.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b0/hsuanwuhub/datasets/procgen.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b0/tests/test_download.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b0/.gitignore
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b0/LICENSE
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b0/README.md
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b0/pyproject.toml
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b0/PKG-INFO
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b1/CNAME
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b1/Makefile
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b1/index.html
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b1/cfgs/config.yaml
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b1/cfgs/task/daac_procgen.yaml
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b1/cfgs/task/drqv2_dmc_pixel.yaml
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b1/cfgs/task/impala_atari.yaml
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b1/cfgs/task/ppg_procgen.yaml
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b1/cfgs/task/ppo_atari.yaml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b1/cfgs/task/ppo_bullet.yaml
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b1/cfgs/task/ppo_procgen.yaml
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b1/cfgs/task/sac_dmc_state.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b1/hsuanwuhub/__init__.py
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b1/hsuanwuhub/train.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b1/hsuanwuhub/datasets/__init__.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b1/hsuanwuhub/datasets/procgen.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b1/tests/test_download.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b1/.gitignore
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b1/LICENSE
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b1/README.md
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b1/pyproject.toml
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 hsuanwuhub-0.0.1b1/PKG-INFO
```

### Comparing `hsuanwuhub-0.0.1b0/CODE_OF_CONDUCT.md` & `hsuanwuhub-0.0.1b1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hsuanwuhub-0.0.1b0/CONTRIBUTING.md` & `hsuanwuhub-0.0.1b1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hsuanwuhub-0.0.1b0/Makefile` & `hsuanwuhub-0.0.1b1/Makefile`

 * *Files identical despite different names*

### Comparing `hsuanwuhub-0.0.1b0/hsuanwuhub/datasets/procgen.py` & `hsuanwuhub-0.0.1b1/hsuanwuhub/datasets/procgen.py`

 * *Files identical despite different names*

### Comparing `hsuanwuhub-0.0.1b0/.gitignore` & `hsuanwuhub-0.0.1b1/.gitignore`

 * *Files identical despite different names*

### Comparing `hsuanwuhub-0.0.1b0/LICENSE` & `hsuanwuhub-0.0.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `hsuanwuhub-0.0.1b0/pyproject.toml` & `hsuanwuhub-0.0.1b1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hsuanwuhub"
-version = "0.0.1.beta00"
+version = "0.0.1.beta01"
 authors = [
-  { name="Reinforcement Learning Evolution Foundation", email="friedrichyuan19990827@gmail.com" },
+  { name="Reinforcement Learning Evolution Foundation", email="hsuanwudev@gmail.com" },
 ]
 description = "Model Hub of the Long-Term Evolution Project of Reinforcement Learning"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["Reinforcement Learning", "Algorithm", "Evolution", "Baseline", "Hub", "Datasets", "Models"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
   "huggingface_hub",
+  "hsuanwu",
+  "numpy",
   "pandas"
 ]
 
 [project.urls]
 "Code" = "https://github.com/RLE-Foundation/HsuanwuHub"
 "Documentation" = "https://docs.hsuanwu.dev/"
 "Benchmark" = "https://hub.hsuanwu.dev/"
@@ -41,12 +43,12 @@
 
 [tool.black]
 line-length = 127
 
 [tool.isort]
 profile = "black"
 line_length = 127
-src_paths = ["hsuanwu"]
+src_paths = ["hsuanwuhub"]
 
 [tool.pytype]
-inputs = ["hsuanwu"]
+inputs = ["hsuanwuhub"]
 disable = ["pyi-error"]
```

### Comparing `hsuanwuhub-0.0.1b0/PKG-INFO` & `hsuanwuhub-0.0.1b1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: hsuanwuhub
-Version: 0.0.1b0
+Version: 0.0.1b1
 Summary: Model Hub of the Long-Term Evolution Project of Reinforcement Learning
 Project-URL: Code, https://github.com/RLE-Foundation/HsuanwuHub
 Project-URL: Documentation, https://docs.hsuanwu.dev/
 Project-URL: Benchmark, https://hub.hsuanwu.dev/
 Project-URL: Bug Tracker, https://github.com/RLE-Foundation/HsuanwuHub/issues
-Author-email: Reinforcement Learning Evolution Foundation <friedrichyuan19990827@gmail.com>
+Author-email: Reinforcement Learning Evolution Foundation <hsuanwudev@gmail.com>
 License-File: LICENSE
 Keywords: Algorithm,Baseline,Datasets,Evolution,Hub,Models,Reinforcement Learning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: hsuanwu
 Requires-Dist: huggingface-hub
+Requires-Dist: numpy
 Requires-Dist: pandas
 Description-Content-Type: text/markdown
 
 # Hsuanwu-benchmark
 Benchmarking implementations of Hsuanwu project.
```


# Comparing `tmp/grecx-0.0.6.tar.gz` & `tmp/grecx-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/grecx-0.0.6.tar", last modified: Tue Apr 26 14:07:36 2022, max compression
+gzip compressed data, was "dist/grecx-0.0.8.tar", last modified: Fri May 12 07:35:43 2023, max compression
```

## Comparing `grecx-0.0.6.tar` & `grecx-0.0.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 caidesheng  (1005) caidesheng  (1006)        0 2022-04-26 14:07:36.000000 grecx-0.0.6/
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)    35149 2021-11-22 18:58:40.000000 grecx-0.0.6/LICENSE
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)     3587 2022-04-26 14:07:36.000000 grecx-0.0.6/PKG-INFO
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)     3207 2021-12-24 09:19:11.000000 grecx-0.0.6/README.rst
-drwxrwxr-x   0 caidesheng  (1005) caidesheng  (1006)        0 2022-04-26 14:07:36.000000 grecx-0.0.6/grecx/
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)       83 2021-12-24 06:47:06.000000 grecx-0.0.6/grecx/__init__.py
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)      802 2021-11-22 18:58:40.000000 grecx-0.0.6/grecx/config.py
-drwxrwxr-x   0 caidesheng  (1005) caidesheng  (1006)        0 2022-04-26 14:07:36.000000 grecx-0.0.6/grecx/datasets/
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)      268 2021-11-23 14:35:59.000000 grecx-0.0.6/grecx/datasets/__init__.py
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)     4237 2021-11-23 09:21:36.000000 grecx-0.0.6/grecx/datasets/diff_net_dataset.py
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)     4073 2021-12-24 06:47:06.000000 grecx-0.0.6/grecx/datasets/light_gcn_dataset.py
-drwxrwxr-x   0 caidesheng  (1005) caidesheng  (1006)        0 2022-04-26 14:07:36.000000 grecx-0.0.6/grecx/evaluation/
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)      188 2021-12-24 06:47:06.000000 grecx-0.0.6/grecx/evaluation/__init__.py
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)    11918 2021-12-24 06:47:06.000000 grecx-0.0.6/grecx/evaluation/ranking.py
-drwxrwxr-x   0 caidesheng  (1005) caidesheng  (1006)        0 2022-04-26 14:07:36.000000 grecx-0.0.6/grecx/layers/
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)      165 2021-12-24 06:47:06.000000 grecx-0.0.6/grecx/layers/__init__.py
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)     2395 2021-12-24 06:47:06.000000 grecx-0.0.6/grecx/layers/embedding.py
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)     3302 2022-04-26 13:58:56.000000 grecx-0.0.6/grecx/layers/light_gcn.py
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)     3585 2021-12-24 06:47:06.000000 grecx-0.0.6/grecx/layers/ngcf.py
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)     2019 2021-12-24 06:47:06.000000 grecx-0.0.6/grecx/layers/user_item_embedding.py
-drwxrwxr-x   0 caidesheng  (1005) caidesheng  (1006)        0 2022-04-26 14:07:36.000000 grecx-0.0.6/grecx/metrics/
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)       88 2021-12-24 06:47:06.000000 grecx-0.0.6/grecx/metrics/__init__.py
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)    55908 2021-12-24 06:47:06.000000 grecx-0.0.6/grecx/metrics/libranking.dll
--rwxrwxr-x   0 caidesheng  (1005) caidesheng  (1006)    16408 2021-12-24 06:47:06.000000 grecx-0.0.6/grecx/metrics/libranking.so
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)     2207 2021-12-24 06:47:06.000000 grecx-0.0.6/grecx/metrics/ranking.py
-drwxrwxr-x   0 caidesheng  (1005) caidesheng  (1006)        0 2022-04-26 14:07:36.000000 grecx-0.0.6/grecx/utils/
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)        0 2021-11-22 18:58:40.000000 grecx-0.0.6/grecx/utils/__init__.py
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)      490 2021-11-22 18:58:40.000000 grecx-0.0.6/grecx/utils/data_utils.py
-drwxrwxr-x   0 caidesheng  (1005) caidesheng  (1006)        0 2022-04-26 14:07:36.000000 grecx-0.0.6/grecx/vector_search/
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)        0 2021-11-23 09:21:36.000000 grecx-0.0.6/grecx/vector_search/__init__.py
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)      646 2021-12-24 06:47:06.000000 grecx-0.0.6/grecx/vector_search/vector_search.py
-drwxrwxr-x   0 caidesheng  (1005) caidesheng  (1006)        0 2022-04-26 14:07:36.000000 grecx-0.0.6/grecx.egg-info/
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)     3587 2022-04-26 14:07:36.000000 grecx-0.0.6/grecx.egg-info/PKG-INFO
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)      721 2022-04-26 14:07:36.000000 grecx-0.0.6/grecx.egg-info/SOURCES.txt
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)        1 2022-04-26 14:07:36.000000 grecx-0.0.6/grecx.egg-info/dependency_links.txt
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)       69 2022-04-26 14:07:36.000000 grecx-0.0.6/grecx.egg-info/requires.txt
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)        6 2022-04-26 14:07:36.000000 grecx-0.0.6/grecx.egg-info/top_level.txt
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)       38 2022-04-26 14:07:36.000000 grecx-0.0.6/setup.cfg
--rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)     1202 2022-04-26 14:07:26.000000 grecx-0.0.6/setup.py
+drwxrwxr-x   0 caidesheng  (1005) caidesheng  (1006)        0 2023-05-12 07:35:43.000000 grecx-0.0.8/
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)    35149 2021-11-22 18:58:40.000000 grecx-0.0.8/LICENSE
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)     3587 2023-05-12 07:35:43.000000 grecx-0.0.8/PKG-INFO
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)     3207 2021-12-24 09:19:11.000000 grecx-0.0.8/README.rst
+drwxrwxr-x   0 caidesheng  (1005) caidesheng  (1006)        0 2023-05-12 07:35:43.000000 grecx-0.0.8/grecx/
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)       83 2021-12-24 06:47:06.000000 grecx-0.0.8/grecx/__init__.py
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)      802 2021-11-22 18:58:40.000000 grecx-0.0.8/grecx/config.py
+drwxrwxr-x   0 caidesheng  (1005) caidesheng  (1006)        0 2023-05-12 07:35:43.000000 grecx-0.0.8/grecx/datasets/
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)      268 2021-11-23 14:35:59.000000 grecx-0.0.8/grecx/datasets/__init__.py
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)     4237 2021-11-23 09:21:36.000000 grecx-0.0.8/grecx/datasets/diff_net_dataset.py
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)     4073 2021-12-24 06:47:06.000000 grecx-0.0.8/grecx/datasets/light_gcn_dataset.py
+drwxrwxr-x   0 caidesheng  (1005) caidesheng  (1006)        0 2023-05-12 07:35:43.000000 grecx-0.0.8/grecx/evaluation/
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)      188 2021-12-24 06:47:06.000000 grecx-0.0.8/grecx/evaluation/__init__.py
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)    11918 2021-12-24 06:47:06.000000 grecx-0.0.8/grecx/evaluation/ranking.py
+drwxrwxr-x   0 caidesheng  (1005) caidesheng  (1006)        0 2023-05-12 07:35:43.000000 grecx-0.0.8/grecx/layers/
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)      165 2021-12-24 06:47:06.000000 grecx-0.0.8/grecx/layers/__init__.py
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)     2395 2021-12-24 06:47:06.000000 grecx-0.0.8/grecx/layers/embedding.py
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)     3302 2022-04-26 13:58:56.000000 grecx-0.0.8/grecx/layers/light_gcn.py
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)     3585 2021-12-24 06:47:06.000000 grecx-0.0.8/grecx/layers/ngcf.py
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)     2019 2021-12-24 06:47:06.000000 grecx-0.0.8/grecx/layers/user_item_embedding.py
+drwxrwxr-x   0 caidesheng  (1005) caidesheng  (1006)        0 2023-05-12 07:35:43.000000 grecx-0.0.8/grecx/metrics/
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)       88 2021-12-24 06:47:06.000000 grecx-0.0.8/grecx/metrics/__init__.py
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)    55908 2021-12-24 06:47:06.000000 grecx-0.0.8/grecx/metrics/libranking.dll
+-rwxrwxr-x   0 caidesheng  (1005) caidesheng  (1006)    16408 2021-12-24 06:47:06.000000 grecx-0.0.8/grecx/metrics/libranking.so
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)     2212 2023-05-12 07:26:01.000000 grecx-0.0.8/grecx/metrics/ranking.py
+drwxrwxr-x   0 caidesheng  (1005) caidesheng  (1006)        0 2023-05-12 07:35:43.000000 grecx-0.0.8/grecx/utils/
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)        0 2021-11-22 18:58:40.000000 grecx-0.0.8/grecx/utils/__init__.py
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)      490 2021-11-22 18:58:40.000000 grecx-0.0.8/grecx/utils/data_utils.py
+drwxrwxr-x   0 caidesheng  (1005) caidesheng  (1006)        0 2023-05-12 07:35:43.000000 grecx-0.0.8/grecx/vector_search/
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)        0 2021-11-23 09:21:36.000000 grecx-0.0.8/grecx/vector_search/__init__.py
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)      646 2021-12-24 06:47:06.000000 grecx-0.0.8/grecx/vector_search/vector_search.py
+drwxrwxr-x   0 caidesheng  (1005) caidesheng  (1006)        0 2023-05-12 07:35:43.000000 grecx-0.0.8/grecx.egg-info/
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)     3587 2023-05-12 07:35:42.000000 grecx-0.0.8/grecx.egg-info/PKG-INFO
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)      721 2023-05-12 07:35:42.000000 grecx-0.0.8/grecx.egg-info/SOURCES.txt
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)        1 2023-05-12 07:35:42.000000 grecx-0.0.8/grecx.egg-info/dependency_links.txt
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)       68 2023-05-12 07:35:42.000000 grecx-0.0.8/grecx.egg-info/requires.txt
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)        6 2023-05-12 07:35:42.000000 grecx-0.0.8/grecx.egg-info/top_level.txt
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)       38 2023-05-12 07:35:43.000000 grecx-0.0.8/setup.cfg
+-rw-rw-r--   0 caidesheng  (1005) caidesheng  (1006)     1202 2023-05-12 07:28:11.000000 grecx-0.0.8/setup.py
```

### Comparing `grecx-0.0.6/LICENSE` & `grecx-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `grecx-0.0.6/PKG-INFO` & `grecx-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grecx
-Version: 0.0.6
+Version: 0.0.8
 Summary: An Efficient and Unified Benchmark for GNN-based Recommendation.
 Home-page: https://github.com/maenzhier/GRecX
 Author: Desheng Cai
 Author-email: caidsml@gmail.com
 License: GNU General Public License v3.0 (See LICENSE)
 Platform: UNKNOWN
 Requires-Python: >3.5.0
```

### Comparing `grecx-0.0.6/README.rst` & `grecx-0.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `grecx-0.0.6/grecx/config.py` & `grecx-0.0.8/grecx/config.py`

 * *Files identical despite different names*

### Comparing `grecx-0.0.6/grecx/datasets/diff_net_dataset.py` & `grecx-0.0.8/grecx/datasets/diff_net_dataset.py`

 * *Files identical despite different names*

### Comparing `grecx-0.0.6/grecx/datasets/light_gcn_dataset.py` & `grecx-0.0.8/grecx/datasets/light_gcn_dataset.py`

 * *Files identical despite different names*

### Comparing `grecx-0.0.6/grecx/evaluation/ranking.py` & `grecx-0.0.8/grecx/evaluation/ranking.py`

 * *Files identical despite different names*

### Comparing `grecx-0.0.6/grecx/layers/embedding.py` & `grecx-0.0.8/grecx/layers/embedding.py`

 * *Files identical despite different names*

### Comparing `grecx-0.0.6/grecx/layers/light_gcn.py` & `grecx-0.0.8/grecx/layers/light_gcn.py`

 * *Files identical despite different names*

### Comparing `grecx-0.0.6/grecx/layers/ngcf.py` & `grecx-0.0.8/grecx/layers/ngcf.py`

 * *Files identical despite different names*

### Comparing `grecx-0.0.6/grecx/layers/user_item_embedding.py` & `grecx-0.0.8/grecx/layers/user_item_embedding.py`

 * *Files identical despite different names*

### Comparing `grecx-0.0.6/grecx/metrics/libranking.dll` & `grecx-0.0.8/grecx/metrics/libranking.dll`

 * *Files identical despite different names*

### Comparing `grecx-0.0.6/grecx/metrics/libranking.so` & `grecx-0.0.8/grecx/metrics/libranking.so`

 * *Files identical despite different names*

### Comparing `grecx-0.0.6/grecx/metrics/ranking.py` & `grecx-0.0.8/grecx/metrics/ranking.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,14 +72,14 @@
 except:
     print("cannot load c_ndcg_score, use Python version instead")
     pass
 
 
 
 def precision_score(reference, hypothesis):
-    result = np.sum(hypothesis, dtype=np.float)/len(hypothesis)
+    result = np.sum(hypothesis, dtype=np.float32)/len(hypothesis)
     return result
 
 
 def recall_score(reference, hypothesis):
-    result = np.sum(hypothesis, dtype=np.float) / len(reference)
-    return result
+    result = np.sum(hypothesis, dtype=np.float32) / len(reference)
+    return result
```

### Comparing `grecx-0.0.6/grecx/vector_search/vector_search.py` & `grecx-0.0.8/grecx/vector_search/vector_search.py`

 * *Files identical despite different names*

### Comparing `grecx-0.0.6/grecx.egg-info/PKG-INFO` & `grecx-0.0.8/grecx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grecx
-Version: 0.0.6
+Version: 0.0.8
 Summary: An Efficient and Unified Benchmark for GNN-based Recommendation.
 Home-page: https://github.com/maenzhier/GRecX
 Author: Desheng Cai
 Author-email: caidsml@gmail.com
 License: GNU General Public License v3.0 (See LICENSE)
 Platform: UNKNOWN
 Requires-Python: >3.5.0
```

### Comparing `grecx-0.0.6/grecx.egg-info/SOURCES.txt` & `grecx-0.0.8/grecx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grecx-0.0.6/setup.py` & `grecx-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 import io
 from setuptools import setup, find_packages
 
 setup(
     name="grecx",
     python_requires='>3.5.0',
-    version="0.0.6",
+    version="0.0.8",
     author="Desheng Cai",
     author_email="caidsml@gmail.com",
     packages=find_packages(
         exclude=[
             'benchmarks',
             'data',
             'demo',
@@ -18,15 +18,15 @@
             'docs',
             'logs',
             'models',
             'test'
         ]
     ),
     install_requires=[
-        "tf_geometric >= 0.0.83",
+        "tf_geometric >= 0.1.5",
         "numpy >= 1.17.4",
         # "tensorflow == 2.4.1",
         "scikit-learn >= 0.22",
         "tqdm",
         # "Sphinx == 3.5.4",
         "faiss-cpu"
     ],
@@ -36,8 +36,8 @@
     package_data={'grecx': ["metrics/libranking.so", "metrics/libranking.dll"]},
     description="An Efficient and Unified Benchmark for GNN-based Recommendation.",
     license="GNU General Public License v3.0 (See LICENSE)",
     long_description=io.open("README.rst", mode="r", encoding="utf-8").read(),
     # long_description="An Efficient and Unified Benchmark for GNN-based Recommendation.",
     long_description_content_type='text/x-rst',
     url="https://github.com/maenzhier/GRecX"
-)
+)
```


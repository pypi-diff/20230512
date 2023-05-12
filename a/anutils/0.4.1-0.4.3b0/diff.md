# Comparing `tmp/anutils-0.4.1.tar.gz` & `tmp/anutils-0.4.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anutils-0.4.1.tar", last modified: Thu Apr 27 06:46:41 2023, max compression
+gzip compressed data, was "anutils-0.4.3b0.tar", last modified: Fri May 12 15:30:54 2023, max compression
```

## Comparing `anutils-0.4.1.tar` & `anutils-0.4.3b0.tar`

### file list

```diff
@@ -1,45 +1,52 @@
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:46:41.375658 anutils-0.4.1/
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)     1799 2022-06-15 05:53:11.000000 anutils-0.4.1/.gitignore
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2164 2023-04-27 06:46:41.375658 anutils-0.4.1/PKG-INFO
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)     1710 2023-03-18 08:13:48.000000 anutils-0.4.1/README.md
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       38 2023-04-27 06:46:41.375658 anutils-0.4.1/setup.cfg
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)      850 2023-04-27 06:46:30.000000 anutils-0.4.1/setup.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:46:41.371658 anutils-0.4.1/src/
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:46:41.375658 anutils-0.4.1/src/anutils/
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)       67 2023-03-03 09:18:56.000000 anutils-0.4.1/src/anutils/__init__.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:46:41.375658 anutils-0.4.1/src/anutils/mlutils/
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)       70 2022-07-20 14:02:32.000000 anutils-0.4.1/src/anutils/mlutils/__init__.py
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)     2457 2022-07-20 14:06:26.000000 anutils-0.4.1/src/anutils/mlutils/mlutils.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:46:41.375658 anutils-0.4.1/src/anutils/scutils/
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)      145 2023-04-19 08:30:07.000000 anutils-0.4.1/src/anutils/scutils/__init__.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     4822 2023-04-26 13:10:33.000000 anutils-0.4.1/src/anutils/scutils/annotation.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:46:41.375658 anutils-0.4.1/src/anutils/scutils/data/
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       19 2023-04-18 12:39:59.000000 anutils-0.4.1/src/anutils/scutils/data/__init__.py
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)     3922 2023-04-10 19:26:09.000000 anutils-0.4.1/src/anutils/scutils/data/data.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1539 2023-04-18 21:48:37.000000 anutils-0.4.1/src/anutils/scutils/data/h5ad2mtx.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1211 2023-04-10 19:26:07.000000 anutils-0.4.1/src/anutils/scutils/data/mtx2rds.R
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:46:41.375658 anutils-0.4.1/src/anutils/scutils/external/
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       45 2023-04-19 06:02:41.000000 anutils-0.4.1/src/anutils/scutils/external/__init__.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:46:41.375658 anutils-0.4.1/src/anutils/scutils/external/integration/
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      102 2023-04-19 06:30:26.000000 anutils-0.4.1/src/anutils/scutils/external/integration/__init__.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1945 2023-04-23 09:52:44.000000 anutils-0.4.1/src/anutils/scutils/external/integration/harmony.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2809 2023-04-20 06:33:17.000000 anutils-0.4.1/src/anutils/scutils/external/integration/harmony_matrix.R
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     3812 2023-04-19 08:24:33.000000 anutils-0.4.1/src/anutils/scutils/external/integration/seurat.R
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1668 2023-04-26 13:02:47.000000 anutils-0.4.1/src/anutils/scutils/external/integration/seurat.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)    11085 2023-04-26 13:43:46.000000 anutils-0.4.1/src/anutils/scutils/plotting.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     3926 2023-04-23 14:56:13.000000 anutils-0.4.1/src/anutils/scutils/preprocessing.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:46:41.375658 anutils-0.4.1/src/anutils/scutils/sc_cuda/
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       72 2023-03-12 12:35:54.000000 anutils-0.4.1/src/anutils/scutils/sc_cuda/__init__.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)    29119 2023-04-20 13:48:41.000000 anutils-0.4.1/src/anutils/scutils/sc_cuda/rapids_scanpy_funcs.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2503 2023-04-20 13:50:49.000000 anutils-0.4.1/src/anutils/scutils/sc_cuda/scanpy_cuda.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     4564 2023-03-12 12:33:33.000000 anutils-0.4.1/src/anutils/scutils/sc_cuda/scib_cuda.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      687 2023-04-20 12:49:32.000000 anutils-0.4.1/src/anutils/scutils/utils.py
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)     9029 2023-04-23 04:03:59.000000 anutils-0.4.1/src/anutils/utils.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:46:41.375658 anutils-0.4.1/src/anutils.egg-info/
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)     2164 2023-04-27 06:46:41.000000 anutils-0.4.1/src/anutils.egg-info/PKG-INFO
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)     1116 2023-04-27 06:46:41.000000 anutils-0.4.1/src/anutils.egg-info/SOURCES.txt
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)        1 2023-04-27 06:46:41.000000 anutils-0.4.1/src/anutils.egg-info/dependency_links.txt
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)       57 2023-04-27 06:46:41.000000 anutils-0.4.1/src/anutils.egg-info/requires.txt
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)        8 2023-04-27 06:46:41.000000 anutils-0.4.1/src/anutils.egg-info/top_level.txt
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-04-27 06:46:41.375658 anutils-0.4.1/tests/
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)      581 2022-06-17 11:20:29.000000 anutils-0.4.1/tests/run_tests.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 15:30:54.371745 anutils-0.4.3b0/
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)     1799 2022-06-15 05:53:11.000000 anutils-0.4.3b0/.gitignore
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      250 2023-05-12 15:30:54.371745 anutils-0.4.3b0/PKG-INFO
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)     2372 2023-05-07 16:11:39.000000 anutils-0.4.3b0/README.md
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       38 2023-05-12 15:30:54.371745 anutils-0.4.3b0/setup.cfg
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)      903 2023-05-12 15:29:33.000000 anutils-0.4.3b0/setup.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 15:30:54.363745 anutils-0.4.3b0/src/
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 15:30:54.363745 anutils-0.4.3b0/src/anutils/
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)       80 2023-05-11 06:30:19.000000 anutils-0.4.3b0/src/anutils/__init__.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      416 2023-05-11 06:33:57.000000 anutils-0.4.3b0/src/anutils/exceptions.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 15:30:54.367745 anutils-0.4.3b0/src/anutils/mlutils/
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)       38 2023-05-11 06:32:55.000000 anutils-0.4.3b0/src/anutils/mlutils/__init__.py
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)     2498 2023-05-11 06:32:47.000000 anutils-0.4.3b0/src/anutils/mlutils/mlutils.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 15:30:54.367745 anutils-0.4.3b0/src/anutils/scutils/
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)      233 2023-05-12 15:10:03.000000 anutils-0.4.3b0/src/anutils/scutils/__init__.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     7665 2023-05-12 15:17:57.000000 anutils-0.4.3b0/src/anutils/scutils/annotation.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 15:30:54.367745 anutils-0.4.3b0/src/anutils/scutils/data/
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       39 2023-05-11 06:31:57.000000 anutils-0.4.3b0/src/anutils/scutils/data/__init__.py
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)     3942 2023-05-11 06:33:02.000000 anutils-0.4.3b0/src/anutils/scutils/data/data.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1539 2023-04-18 21:48:37.000000 anutils-0.4.3b0/src/anutils/scutils/data/h5ad2mtx.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1211 2023-04-10 19:26:07.000000 anutils-0.4.3b0/src/anutils/scutils/data/mtx2rds.R
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 15:30:54.367745 anutils-0.4.3b0/src/anutils/scutils/external/
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       68 2023-05-11 06:31:45.000000 anutils-0.4.3b0/src/anutils/scutils/external/__init__.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 15:30:54.367745 anutils-0.4.3b0/src/anutils/scutils/external/integration/
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      297 2023-05-11 14:19:55.000000 anutils-0.4.3b0/src/anutils/scutils/external/integration/__init__.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1707 2023-05-05 18:26:12.000000 anutils-0.4.3b0/src/anutils/scutils/external/integration/harmony.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2809 2023-04-20 06:33:17.000000 anutils-0.4.3b0/src/anutils/scutils/external/integration/harmony_matrix.R
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      577 2023-05-06 07:55:23.000000 anutils-0.4.3b0/src/anutils/scutils/external/integration/integration.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     3414 2023-05-11 14:37:17.000000 anutils-0.4.3b0/src/anutils/scutils/external/integration/scalex.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2187 2023-05-06 07:55:52.000000 anutils-0.4.3b0/src/anutils/scutils/external/integration/scvi.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     4242 2023-05-09 06:26:37.000000 anutils-0.4.3b0/src/anutils/scutils/external/integration/seurat.R
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1578 2023-05-06 07:50:07.000000 anutils-0.4.3b0/src/anutils/scutils/external/integration/seurat.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)    17278 2023-05-12 08:10:32.000000 anutils-0.4.3b0/src/anutils/scutils/plotting.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     7833 2023-05-05 13:05:09.000000 anutils-0.4.3b0/src/anutils/scutils/preprocessing.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 15:30:54.363745 anutils-0.4.3b0/src/anutils/scutils/resources/
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 15:30:54.367745 anutils-0.4.3b0/src/anutils/scutils/resources/gene_sets/
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      556 2023-05-12 15:00:19.000000 anutils-0.4.3b0/src/anutils/scutils/resources/gene_sets/regev_lab_cell_cycle_genes.txt
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 15:30:54.367745 anutils-0.4.3b0/src/anutils/scutils/sc_cuda/
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      116 2023-05-11 06:30:39.000000 anutils-0.4.3b0/src/anutils/scutils/sc_cuda/__init__.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)    29119 2023-04-20 13:48:41.000000 anutils-0.4.3b0/src/anutils/scutils/sc_cuda/rapids_scanpy_funcs.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2503 2023-04-20 13:50:49.000000 anutils-0.4.3b0/src/anutils/scutils/sc_cuda/scanpy_cuda.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     4564 2023-03-12 12:33:33.000000 anutils-0.4.3b0/src/anutils/scutils/sc_cuda/scib_cuda.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1229 2023-05-11 02:41:54.000000 anutils-0.4.3b0/src/anutils/scutils/utils.py
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)    10582 2023-05-04 16:21:28.000000 anutils-0.4.3b0/src/anutils/utils.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 15:30:54.363745 anutils-0.4.3b0/src/anutils.egg-info/
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)      250 2023-05-12 15:30:53.000000 anutils-0.4.3b0/src/anutils.egg-info/PKG-INFO
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)     1369 2023-05-12 15:30:54.000000 anutils-0.4.3b0/src/anutils.egg-info/SOURCES.txt
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)        1 2023-05-12 15:30:53.000000 anutils-0.4.3b0/src/anutils.egg-info/dependency_links.txt
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)       73 2023-05-12 15:30:54.000000 anutils-0.4.3b0/src/anutils.egg-info/requires.txt
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)        8 2023-05-12 15:30:54.000000 anutils-0.4.3b0/src/anutils.egg-info/top_level.txt
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-12 15:30:54.367745 anutils-0.4.3b0/tests/
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)      581 2022-06-17 11:20:29.000000 anutils-0.4.3b0/tests/run_tests.py
```

### Comparing `anutils-0.4.1/.gitignore` & `anutils-0.4.3b0/.gitignore`

 * *Files identical despite different names*

### Comparing `anutils-0.4.1/setup.py` & `anutils-0.4.3b0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,34 +4,33 @@
     from pypandoc import convert_file
     long_description = convert_file('README.md', 'rst')
 except:
     long_description = ''
 
 setup(
     name='anutils',
-    version='0.4.1',
+    version='0.4.3b0',
     license='MIT',
     author="Aaron Ning",
     author_email='aaronning98@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
-    
+
     # If any package contains *.r files, include them:
-    package_data={'': ['*.r', '*.R']},
+    package_data={'': ['*.r', '*.R', 'src/anutils/scutils/resources/**/*']},
     include_package_data=True,
-
     description='ml and single cell utils.',
-    long_description=long_description, 
-
+    long_description=long_description,
     url='https://github.com/AaronNing/anutils',
     keywords='anutils',
     install_requires=[
         'scipy',
         'numpy',
-        'pandas', 
+        'pandas',
         'matplotlib',
-        'seaborn', 
-        'scanpy', 
+        'seaborn',
+        'scanpy',
         'getkey',
         'muon',
-        ],
+        'statannotations',
+    ],
 )
```

### Comparing `anutils-0.4.1/src/anutils/mlutils/mlutils.py` & `anutils-0.4.3b0/src/anutils/mlutils/mlutils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from anutils.utils import flatten
 
 
-def plot_learning_curve(data: pd.DataFrame, keys: list, suptitle='', save: str = None, style: str = 'default'):
+def plot_learning_curve(data: pd.DataFrame,
+                        keys: list,
+                        suptitle='',
+                        save: str = None,
+                        style: str = 'default'):
     r"""
     data: dict of curves
     keys: list specifying the plot structures. E.g., [['tl', 'vl], ['ta', 'va']] means two subplots. 
     """
     plt.style.use(style)
     plt.rc('font', family='Helvetica')
     plt.rcParams['pdf.fonttype'] = 42
 
     n_subplots = len(keys)
     w = np.ceil(np.sqrt(n_subplots)).astype(int)
-    h = np.ceil(n_subplots/w).astype(int)
-    plt.figure(figsize=[5*w, 5*h], dpi=80, facecolor='white')
+    h = np.ceil(n_subplots / w).astype(int)
+    plt.figure(figsize=[5 * w, 5 * h], dpi=80, facecolor='white')
     for i_subp in range(n_subplots):
-        plt.subplot(h, w, i_subp+1)
+        plt.subplot(h, w, i_subp + 1)
         sns.lineplot(data=data.loc[:, keys[i_subp]], dashes=False)
         plt.grid()
     plt.suptitle(suptitle)
     if save:
         plt.savefig(save)
         plt.close()
     else:
@@ -54,27 +58,23 @@
     try:
         with open(path, 'r') as f:
             lines = f.readlines()
     except UnicodeDecodeError:
         with open(path, 'r', encoding='utf16') as f:
             lines = f.readlines()
     for line in lines:
-        line = (
-            line.replace(",", " ")
-            .replace(":", " ")
-            .replace("=", " "))
+        line = (line.replace(",", " ").replace(":", " ").replace("=", " "))
         words = line.split()
         words = [word.strip('`\'\"()[]{}') for word in words]
         for key in keys:
             if key in words:
-                value = float(words[words.index(key)+1])
+                value = float(words[words.index(key) + 1])
                 out[key].append(value)
     out = pd.DataFrame(out)
     if plot:
         if isinstance(plot, bool):
-            assert(path.endswith(".txt"))
+            assert (path.endswith(".txt"))
             plot = path[:-4] + '_learning_curve.' + format
         elif not isinstance(plot, str):
-            raise(AttributeError)
-        plot_learning_curve(out, keys=plot_structure,
-                            suptitle=suptitle, save=plot, style=style)
+            raise (AttributeError)
+        plot_learning_curve(out, keys=plot_structure, suptitle=suptitle, save=plot, style=style)
     return out
```

### Comparing `anutils-0.4.1/src/anutils/scutils/data/data.py` & `anutils-0.4.3b0/src/anutils/scutils/data/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 import pandas as pd
 import scanpy as sc
 import scipy.io
 
-from .h5ad2mtx import h5ad2mtx
+from anutils.scutils.data.h5ad2mtx import h5ad2mtx
 
 # def ad2mtx(ad_path: str) -> None:
 #     r"""
 #     convert adata to: `matrix.mtx`, `genes.txt` and `metadata.txt`
 #     """
 #     adata = sc.read_h5ad(ad_path)
 #     outdir = os.path.dirname(ad_path)
```

### Comparing `anutils-0.4.1/src/anutils/scutils/data/h5ad2mtx.py` & `anutils-0.4.3b0/src/anutils/scutils/data/h5ad2mtx.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.1/src/anutils/scutils/data/mtx2rds.R` & `anutils-0.4.3b0/src/anutils/scutils/data/mtx2rds.R`

 * *Files identical despite different names*

### Comparing `anutils-0.4.1/src/anutils/scutils/external/integration/harmony.py` & `anutils-0.4.3b0/src/anutils/scutils/external/integration/harmony.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,12 @@
 import os
 import pandas as pd
 
 HARMONY_MATRIX_R_SCRIPT = os.path.join(os.path.dirname(__file__), 'harmony_matrix.R')
 
-# check harmony is installed
-exit_code = os.system('Rscript -e "library(harmony)"')
-if exit_code != 0:
-    raise RuntimeError(
-        f'Error running Rscript -e "library(harmony)" (exit code: {exit_code}). Please install harmony'
-    )
-
 
 def harmony_matrix(
     input_path,
     output_path,
     metadata_path,
     batch_key='batch',
     # harmony arguments
```

### Comparing `anutils-0.4.1/src/anutils/scutils/external/integration/harmony_matrix.R` & `anutils-0.4.3b0/src/anutils/scutils/external/integration/harmony_matrix.R`

 * *Files identical despite different names*

### Comparing `anutils-0.4.1/src/anutils/scutils/external/integration/seurat.R` & `anutils-0.4.3b0/src/anutils/scutils/external/integration/seurat.R`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 parser$add_argument("-i", "--input_path", type="character", help="Path contains RNA data")
 parser$add_argument("-o", "--output_path", type="character", default='/home/tiankang/SCALEX/results/Seurat_v3', help="Output path")
 parser$add_argument("-mf", "--minFeatures", type="integer", default=600, help="Remove cells with less than minFeatures features")
 parser$add_argument("-mc", "--minCells", type="integer", default=3, help="Remove features with less than minCells cells")
 parser$add_argument("-nt", "--n_top_features", type="integer", default=2000, help="N highly variable features")
 parser$add_argument("-nj", "--n_jobs", type="integer", default=1, help="Number of jobs")
 parser$add_argument("--batch_key", type="character", default='batch', help="Batch key")
+parser$add_argument("--k_anchor", type="integer", default=5, help="k.anchor")
+parser$add_argument("--k_filter", type="integer", default=200, help="k.filter")
+parser$add_argument("--k_score", type="integer", default=30, help="k.score")
 args <- parser$parse_args()
 
 plan("multiprocess", workers = args$n_jobs)
 options(future.globals.maxSize = 100000 * 1024^2, warn = -1)
 
 # Read data
 message('Reading data...')
@@ -40,16 +43,19 @@
 cat('there are ', length(unique(metadata[[args$batch_key]])), ' batches\n')
 
 # PP and integration
 adata.list <- SplitObject(adata, split.by = args$batch_key)
 
 message('Preprocessing each batch...')
 adata.list <- future_lapply(X = adata.list, FUN = function(x) {
+    # calculate percent.mito
+    # x <- PercentageFeatureSet(x, pattern = "^MT-", col.name = "percent.mito")
     x <- NormalizeData(x, verbose = FALSE)
     x <- FindVariableFeatures(x, nfeatures = args$n_top_features, selection.method = "vst", verbose = FALSE)
+    # x <- ScaleData(x, verbose = FALSE, vars.to.regress = c('nUMI', 'percent.mito'))
 }, future.seed = TRUE)
 
 message('SelectIntegrationFeatures...')
 features <- SelectIntegrationFeatures(object.list = adata.list)
 
 message('PCA each batch...')
 adata.list <- future_lapply(X = adata.list, FUN = function(x) {
```

### Comparing `anutils-0.4.1/src/anutils/scutils/external/integration/seurat.py` & `anutils-0.4.3b0/src/anutils/scutils/external/integration/seurat.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 import os
 
 import pandas as pd
 
 SEURAT_R_SCRIPT = os.path.join(os.path.dirname(__file__), 'seurat.R')
 
-# check Seurat is installed
-exit_code = os.system('Rscript -e "library(Seurat)"')
-if exit_code != 0:
-    raise RuntimeError(
-        f'Error running Rscript -e "library(Seurat)" (exit code: {exit_code}). Please install Seurat'
-    )
-
 
 def seurat(
     input_path,
     output_path,
     min_features=150,
     min_cells=3,
     n_top_features=2000,
     n_jobs=1,
     batch_key='batch',
+    k_anchor=5,
+    k_filter=200,
+    k_score=30,
 ):
     """
     params:
     ---
     input_path: str
         dir containing `matrix.mtx`, `features.txt`, `metadata.txt`. can be generated by `anutils.scutils.data.h5ad2mtx`
     output_path: str
@@ -43,14 +39,17 @@
         '-i': input_path,
         '-o': output_path,
         '-mf': min_features,
         '-mc': min_cells,
         '-nt': n_top_features,
         '-nj': n_jobs,
         '--batch_key': batch_key,
+        '--k_anchor': k_anchor,
+        '--k_filter': k_filter,
+        '--k_score': k_score,
     }
     cmd = f'Rscript {SEURAT_R_SCRIPT} {" ".join([f"{k} {v}" for k, v in args.items()])}'
     exit_code = os.system(cmd)
     if exit_code != 0:
         raise RuntimeError(f'Error running seurat: {cmd} (exit code: {exit_code}')
 
     # collect results into memory
```

### Comparing `anutils-0.4.1/src/anutils/scutils/plotting.py` & `anutils-0.4.3b0/src/anutils/scutils/plotting.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+from itertools import combinations
+
 import matplotlib as mpl
 import matplotlib.pyplot as plt
-import scanpy as sc
 import numpy as np
 import pandas as pd
+import scanpy as sc
 import seaborn as sns
+from statannotations.Annotator import Annotator
+
+from anutils.utils import Silent
 
 
 def init_fig_params():
     plt.rcParams['axes.unicode_minus'] = False
     plt.rc('font', family='Helvetica')
     plt.rcParams['pdf.fonttype'] = 42
     # sc.settings.verbosity = 3  # verbosity: errors (0), warnings (1), info (2), hints (3)
@@ -16,33 +21,33 @@
     # %config InlineBackend.figure_format='retina'
     # %matplotlib inline
 
 
 def embeddings(adata,
                basis=None,
                *,
-               group_adata_by=None,
+               groupby,
                replicate_key=None,
                groups_order=None,
                add_bg=False,
                ncols=None,
                figsize=None,
                zoom=False,
                return_fig_axes=False,
                **embedding_kwargs):
     """plot embeddings of adata grouped by group_adata_by
 
     Parameters
     ----------
-    group_adata_by : str or list of str
+    groupby : str or list of str
         column(s) in adata.obs. if a list, they will be concatenated with '::' as the group key
     replicate_key : str, optional
         a column in adata.obs, by default None. If not None, the number of replicates will be shown in the title
     groups_order : iterable, optional
-        a ordered list of keys in `adata.obs[group_adata_by]`, by default None
+        a ordered list of keys in `adata.obs[groupby]`, by default None
     add_bg : bool, optional
         whether to add umap background (from other groups), by default False
     ncols : int, optional
         ncols, by default 3
     figsize : 2 length tuple, optional
         figsize, by default `(5 * ncols, 5 * nrows)`
     zoom : bool, optional
@@ -56,31 +61,29 @@
     -------
     fig
         the fig object
     """
     if basis is None:
         basis = 'X_umap'
 
-    assert group_adata_by is not None, 'argument `group_adata_by` is required'
-
     # reorder
-    if isinstance(group_adata_by, str):
+    if isinstance(groupby, str):
         pass
     else:  # iterable
-        group_adata_by = '::'.join(group_adata_by)
-        adata.obs[group_adata_by] = adata.obs[list(group_adata_by.split('::'))].apply(
-            lambda x: '::'.join(x), axis=1)
-    indices = adata.obs.groupby(group_adata_by).indices
+        groupby = '::'.join(groupby)
+        adata.obs[groupby] = adata.obs[list(groupby.split('::'))].apply(lambda x: '::'.join(x),
+                                                                        axis=1)
+    indices = adata.obs.groupby(groupby).indices
     if groups_order is None:
         groups_order = indices.keys()
     indices = {k: indices[k] for k in groups_order}
     if ncols is None:
         ncols = min(4, len(indices))
     # plot
-    N = adata.obs[group_adata_by].nunique()
+    N = adata.obs[groupby].nunique()
     nrows = (N - 1) // ncols + 1
     if figsize is None:
         figsize = (5 * ncols, 5 * nrows)
     fig, axes = plt.subplots(ncols=ncols, nrows=nrows, figsize=figsize)
 
     if 'color' in embedding_kwargs:
         if isinstance(embedding_kwargs['color'], str):
@@ -151,60 +154,85 @@
         # we change the bar width
         patch.set_width(new_value)
 
         # we recenter the bar
         patch.set_x(patch.get_x() + diff * .5)
 
 
-def barplot(df,
-            key='celltype',
-            color=sns.color_palette("tab20"),
-            width=0.6,
-            figsize=(16, 6),
-            save=False):
-    fig = plt.figure(figsize=figsize)
-    ax = sns.barplot(x=key, y='counts', data=df, color=color, saturation=1)
-    plt.xlabel('donor', fontsize=22, labelpad=8)
-    plt.ylabel('Cell Number', fontsize=22, labelpad=8)
-    plt.xticks(rotation=45, fontsize=20, ha='right')
-    plt.yticks([0, 5000, 10000, 15000], rotation=0, fontsize=20)
-    plt.title('', fontsize=25, ha='center')
-
-    change_bar_width(ax, width)
-
-    if save:
-        plt.savefig(save, dpi=100, format='pdf', bbox_inches='tight')
-
-
-def dotplot(adata, groupby, var_names, inplace=False, **dotplot_kwargs):
+def dotplot(adata,
+            groupby,
+            var_names,
+            inplace=False,
+            return_object=False,
+            dendogram=True,
+            **dotplot_kwargs):
     if not inplace:
         adata = adata.copy()
     if 'base' not in adata.uns['log1p']:
         adata.uns['log1p']['base'] = np.e
     adata.obs[groupby] = adata.obs[groupby].astype('category')
-    sc.tl.dendrogram(adata, groupby=groupby, var_names=var_names)
-    sc.pl.dotplot(adata,
-                  groupby=groupby,
-                  var_names=var_names,
-                  dendrogram=True,
-                  **dotplot_kwargs)
-
-
-def composition_plot(data,
-                     x,
-                     hue,
-                     x_subset=None,
-                     hue_subset=None,
-                     hue_colors=None,
-                     bar_width=None,
-                     figsize=None,
-                     legend_fontsize=None,
-                     label_fontsize=None,
-                     label_pad=None,
-                     label_rotation=None):
+
+    dp = sc.pl.DotPlot(adata,
+                       groupby=groupby,
+                       var_names=var_names,
+                       cmap='Reds',
+                       **dotplot_kwargs)
+    if dendogram:
+        sc.tl.dendrogram(adata, groupby=groupby, var_names=var_names)
+        dp.add_dendrogram()
+    dp.show()
+    return dp if return_object else None
+
+
+def matrixplot_zscore(adata,
+                      groupby,
+                      var_names,
+                      inplace=False,
+                      cmap='RdBu_r',
+                      return_object=False,
+                      dendogram=True,
+                      **matrixplot_kwargs):
+    if not inplace:
+        adata = adata.copy()
+    adata.obs[groupby] = adata.obs[groupby].astype('category')
+    mp = sc.pl.MatrixPlot(adata, var_names=var_names, groupby=groupby, **matrixplot_kwargs)
+    df = mp.values_df.copy()
+    df = df.sub(df.mean(0), 1).div(df.std(0), 1)
+    mp.values_df = df
+    mp.color_legend_title = 'z-score\nby gene'
+    mp = mp.style(cmap=cmap)
+
+    if dendogram:
+        sc.tl.dendrogram(adata, groupby=groupby, var_names=var_names)
+        mp.add_dendrogram()
+
+    mp.show()
+    return mp if return_object else None
+
+
+def composition_plot(
+    data,
+    x,
+    hue,
+    x_subset=None,
+    hue_subset=None,
+    hue_colors=None,
+    bar_width=0.6,
+    figsize=None,
+    legend_fontsize=None,
+    legend_ncols=2,
+    label_fontsize=None,
+    label_pad=None,
+    label_rotation=45,
+    return_df=False,
+    add_counts=True,
+    hspace=0.1,
+    counts_height_ratio=.25,
+    counts_color='#154c79',
+):
     """plot the composition of a categorical variable `hue` in different groups of `x`
 
     Parameters
     ----------
     data : Union[DataFrame, AnnData]
         data to plot
     x : str
@@ -213,69 +241,86 @@
         categorical variable to plot
     x_subset : List[str], optional
         x subset, by default None
     hue_subset : List[str], optional
         hue subset, by default None
     hue_colors : Iterable, optional
         hue colors, by default None
+    add_counts : bool, optional
+        whether to add an additional barplot of counts on the top, by default True
 
     Returns
     -------
     matplotlib.axes.Axes
         axes
 
     Raises
     ------
     ValueError
         data must be a pandas.DataFrame or an anndata.AnnData
     """
     if type(data).__name__ == 'DataFrame':
-        df = data
+        df: pd.DataFrame = data
     elif type(data).__name__ == 'AnnData':
-        df = data.obs
+        df: pd.DataFrame = data.obs
     else:
         raise ValueError('data must be a pandas.DataFrame or an anndata.AnnData')
-    tmp = df.groupby(x)[hue].value_counts().unstack()
+    
+    if figsize is None:
+        # get the scanpy default figsize
+        sc.set_figure_params
+
+    counts_df: pd.DataFrame = df.groupby(x)[hue].value_counts().unstack()
     if x_subset is None:
-        x_subset = tmp.index
+        x_subset = counts_df.index
     if hue_subset is None:
-        hue_subset = tmp.columns
-    if bar_width is None:
-        bar_width = .6
-    if figsize is None:
-        figsize = (16, 8)
-    if legend_fontsize is None:
-        legend_fontsize = 20
-    if label_rotation is None:
-        label_rotation = 45
-    if label_fontsize is None:
-        label_fontsize = 22
-    if label_pad is None:
-        label_pad = 8
-    tmp = tmp.loc[x_subset, hue_subset]
-    tmp = tmp.T
-    tmp = tmp.div(tmp.sum(axis=0), axis=1).T * 100
-    ax = tmp.plot(kind='bar', stacked=True, figsize=figsize, color=hue_colors)
-    plt.xticks(fontsize=label_fontsize, rotation=label_rotation)
-    plt.yticks(fontsize=label_fontsize)
-    plt.ylabel('Relative celltype abundacy(%)')
-    plt.xlabel('', fontsize=label_fontsize, labelpad=label_pad)
+        hue_subset = counts_df.columns
+    counts_df = counts_df.loc[x_subset, hue_subset]
+    counts_df = counts_df.T
+    counts = counts_df.sum(axis=0)
+    comp_df = counts_df.div(counts_df.sum(axis=0), axis=1).T * 100
+
+    if add_counts:
+        # make two axes, both share the same x axis. the top one is for the counts,
+        # the bottom one is for the composition. the top one's height is 1/3 of the bottom one.
+        fig, (ax1, ax2) = plt.subplots(
+            nrows=2,
+            ncols=1,
+            sharex=True,
+            gridspec_kw={'height_ratios': [counts_height_ratio, 1 - counts_height_ratio]},
+            figsize=figsize,
+        )
+        fig.subplots_adjust(hspace=hspace)
+        
+        # plot counts
+        ax = counts.plot.bar(ax=ax1, color=counts_color, width=bar_width)
+        ax.set_ylabel('Cell counts', fontsize=label_fontsize)
+        ax.set_yticklabels(ax.get_yticklabels(), fontsize=label_fontsize)
+    else:
+        fig, ax2 = plt.subplots(1, 1, figsize=figsize)
+
+    # plot composition
+    ax: plt.Axes = comp_df.plot.bar(ax=ax2, stacked=True, figsize=figsize, color=hue_colors)
+    ax.set_xticklabels(ax.get_xticklabels(), fontsize=label_fontsize, rotation=label_rotation)
+    ax.set_yticklabels(ax.get_yticklabels(), fontsize=label_fontsize)
+    ax.set_ylabel('Relative celltype abundacy(%)', fontsize=label_fontsize)
+    ax.set_xlabel('', fontsize=label_fontsize, labelpad=label_pad)
     legend_params = {
         'loc': 'center left',
         'bbox_to_anchor': (1.01, 0.5),
         'fontsize': legend_fontsize,
-        'ncol': 2,
+        'ncol': legend_ncols,
         'frameon': False,
         'markerscale': 100,
     }
-
-    plt.legend(**legend_params)
+    ax.legend(**legend_params)
 
     change_bar_width(ax, bar_width)
-    return ax
+    
+    return (ax1, ax2) if not return_df else ((ax1, ax2), comp_df)
 
 
 def get_cmap_colors(cmap, n, alpha=1, pad=1):
     colors = getattr(mpl.cm, cmap)(np.linspace(start=0, stop=1, num=n + 2 * pad), alpha=alpha)
     if pad > 0:
         colors = colors[pad:-pad]
     return colors
@@ -322,8 +367,167 @@
                                           n=len(group_items[g]),
                                           pad=pad,
                                           alpha=alpha)
         for i, item in enumerate(group_items[g]):
             item_colors[item] = group_colors[g][i]
     item_colors = {k: item_colors[k] for k in items}
     colors = list(item_colors.values())
-    return colors
+    return colors
+
+
+def barplot_with_pvals(data,
+                       x,
+                       y,
+                       order=None,
+                       pairs=None,
+                       verbose=True,
+                       ax=None,
+                       palette=None,
+                       add_swarmplot=True,
+                       showfliers=True,
+                       simple_format=False,
+                       test='t-test_ind',
+                       text_format='star'):
+    """sns.barplot with p-values
+    
+    Recommended to use with figsize = (1.5, 2)
+
+    Parameters
+    ----------
+    data : DataFrame
+        df
+    x : str
+        column name (group by)
+    y : str
+        column name (bar height)
+    order : Iterable, optional
+        order of x
+    pairs : Iterable of tuples, optional
+        pairs to compare and add p-values. If None, all pairs will be compared, by default None
+    verbose : bool, optional
+        whether to show p-val calculation details, by default True
+    ax : Axes, optional
+        ax, by default None
+    palette : _type_, optional
+        _description_, by default None
+    add_swarmplot : bool, optional
+        whether to add swarmplot, by default True
+    showfliers: bool, optional
+        whether to show outliers, by default True. When simple_format is True, this will be set to False
+    simple_format : bool, optional
+        if True, do not show outliers, and remove xlabel and ylabel, instead, use y key as x label, by default True
+    test : str, optional
+        see `statannotations.Annotator.Annotator`, by default 't-test_ind'
+    text_format : str, optional
+        see `statannotations.Annotator.Annotator`, by default 'star'
+
+    Returns
+    -------
+    Axes
+        ax
+    """
+    if order is None:
+        order = sorted(data[x].unique())
+    if pairs is None:
+        pairs = list(combinations(order, 2))
+    if simple_format:
+        showfliers = False
+
+    ax = sns.boxplot(
+        data=data[data[x].isin(order)],
+        x=x,
+        y=y,
+        ax=ax,
+        order=order,
+        linewidth=1,
+        width=.4,
+        saturation=1,
+        showfliers=showfliers,
+        palette=palette,
+    )
+    if add_swarmplot:
+        # if too many points, do not add swarmplot
+        if data.groupby(x).size().max() > 100:
+            print('Too many points, not adding swarmplot.')
+            add_swarmplot = False
+        else:
+            ax = sns.swarmplot(data=data[data[x].isin(order)],
+                               x=x,
+                               y=y,
+                               ax=ax,
+                               order=order,
+                               edgecolor='k',
+                               palette=palette,
+                               alpha=.9,
+                               size=3,
+                               linewidth=0.5)
+    ax.grid(False)
+    if simple_format:
+        ax.set_xlabel(y)
+        # ax.set_ylabel('Percentage')
+        ax.set_ylabel('')
+        # ax.set_xticks([])
+        ax.tick_params(bottom=False, labelbottom=False)
+    ax.spines[['top', 'right']].set_visible(False)
+    ax.tick_params(labelsize=8)
+    if verbose:
+        annotator = Annotator(ax, pairs, data=data, x=x, y=y, order=order)
+        annotator.configure(test='t-test_ind',
+                            text_format='star',
+                            loc='inside',
+                            show_test_name=False,
+                            line_width=1)
+        annotator.apply_and_annotate()
+    else:
+        with Silent('stdout'):
+            annotator = Annotator(ax, pairs, data=data, x=x, y=y, order=order)
+            annotator.configure(test=test,
+                                text_format=text_format,
+                                loc='outside',
+                                show_test_name=False,
+                                line_width=1)
+            annotator.apply_and_annotate()
+    return ax
+
+
+def plot_legend(
+    ax,
+    color_map,
+    ncol=1,
+    title='',
+    marker='s',
+    loc='lower right',
+):
+    """plot legend on an ax.
+
+    Parameters
+    ----------
+    ax : _type_
+        _description_
+    color_map : dict
+        {str: color} dict
+    ncol : int, optional
+        ncol of legend, by default 1
+    title : str, optional
+        title, by default ''
+    marker : str, optional
+        marker type, by default 's'
+
+    Returns
+    -------
+    Axes
+        ax
+    """
+    from matplotlib.lines import Line2D
+
+    # plt.figure(figsize=figsize)
+    legend_TN = [
+        Line2D([0], [0], color=color, label=c, marker=marker) for c, color in color_map.items()
+    ]
+    ax.legend(handles=legend_TN,
+              ncol=ncol,
+              frameon=False,
+              title=title,
+              prop={'size': 10},
+              loc=loc)
+    ax.axis('off')
+    return ax
```

### Comparing `anutils-0.4.1/src/anutils/scutils/sc_cuda/rapids_scanpy_funcs.py` & `anutils-0.4.3b0/src/anutils/scutils/sc_cuda/rapids_scanpy_funcs.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.1/src/anutils/scutils/sc_cuda/scanpy_cuda.py` & `anutils-0.4.3b0/src/anutils/scutils/sc_cuda/scanpy_cuda.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.1/src/anutils/scutils/sc_cuda/scib_cuda.py` & `anutils-0.4.3b0/src/anutils/scutils/sc_cuda/scib_cuda.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.1/src/anutils/utils.py` & `anutils-0.4.3b0/src/anutils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,14 +111,42 @@
             return ret
 
         return wrapped
 
     return silencer
 
 
+class Silent():
+
+    def __init__(self, mode):
+        if isinstance(mode, str):
+            mode = [mode]
+        for item in mode:
+            assert item in ['stdout', 'stderr']
+        self.mode = mode
+        self.out_bak = sys.stdout
+        self.err_bak = sys.stderr
+        self.devnull = open(os.devnull, 'w', encoding='utf-8')
+
+    def __enter__(self):
+        for mode in self.mode:
+            if mode == 'stdout':
+                sys.stdout = self.devnull
+            elif mode == 'stderr':
+                sys.stderr = self.devnull
+
+    def __exit__(self, type, value, traceback):
+        for mode in self.mode:
+            if mode == 'stdout':
+                sys.stdout = self.out_bak
+            elif mode == 'stderr':
+                sys.stderr = self.err_bak
+        self.devnull.close()
+
+
 def timing(fn, show_datetime: bool = True):
     r"""time a function.
     """
 
     def timed(*args, **kwargs):
         start = time.time()
         ret = fn(*args, **kwargs)
@@ -255,45 +283,66 @@
     """similar to R's `dplyr::glimpse`
     
     n: number of rows to show
     show_unique: show unique values
     columns: list of columns to show
     truncate_at: truncate string at
     """
-    print(f"Rows: {df.shape[0]}")
-    print(f"Columns: {df.shape[1]}")
+    print(f"DataFrame: {df.shape[0]} rows, {df.shape[1]} columns")
+
+    # info is a list of tuples
+    # if `show_unique`, each tuple is (column_name, dtype, values, nunique)
+    # else, each tuple is (column_name, dtype, values)
     info = []
+
+    # index
+    index_name = 'index ({})'.format(str(df.index.name) if df.index.name is not None else '')
+    if show_unique:
+        values = df.index.unique().tolist()[:n]
+        nunique = df.index.nunique()
+        info.append((index_name, str(df.index.dtype), values, nunique))
+    else:
+        values = df.index.head(n).values.tolist()
+        info.append((index_name, str(df.index.dtype), values))
+
+    # columns
     if columns is None:
         columns = df.columns
     for col in columns:
         if col not in df.columns:
             info.append((col, 'missing', [], 0))
         else:
             if show_unique:
                 values = df[col].unique().tolist()[:n]
                 nunique = df[col].nunique()
                 info.append((col, str(df[col].dtype), values, nunique))
             else:
                 values = df[col].head(n).values.tolist()
                 info.append((col, str(df[col].dtype), values))
+
     max_len_col = max([len(i[0]) for i in info])
     max_len_dtype = max([len(i[1]) for i in info])
     if show_unique:
         max_len_unique = max([len(str(i[3])) for i in info])
-    for i in info:
-        s = f"$ {i[0]:<{max_len_col}} {'<'+i[1]+'>':<{max_len_dtype+2}}"
+    for irow, i in enumerate(info):
+        # index
+        if irow == 0:
+            s = f"{i[0]:<{max_len_col+2}} {'<'+i[1]+'>':<{max_len_dtype+2}}"
+        else:
+            s = f"$ {i[0]:<{max_len_col}} {'<'+i[1]+'>':<{max_len_dtype+2}}"
         if show_unique:
             s += f" {'('+str(i[3])+')':<{max_len_unique+2}}"
         list_s = f"{i[2]}"
         if show_unique and i[3] <= n and len(list_s) <= truncate_at:
             pass
         else:
             list_s = list_s[:-1][:truncate_at] + ' ...'
         s += ' ' + list_s
         print(s)
+    print()
 
 
 def roman(num: int) -> str:
 
     chlist = "VXLCDM"
     rev = [int(ch) for ch in reversed(str(num))]
     chlist = ["I"] + [
```

### Comparing `anutils-0.4.1/src/anutils.egg-info/SOURCES.txt` & `anutils-0.4.3b0/src/anutils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitignore
 README.md
 setup.py
 src/anutils/__init__.py
+src/anutils/exceptions.py
 src/anutils/utils.py
 src/anutils.egg-info/PKG-INFO
 src/anutils.egg-info/SOURCES.txt
 src/anutils.egg-info/dependency_links.txt
 src/anutils.egg-info/requires.txt
 src/anutils.egg-info/top_level.txt
 src/anutils/mlutils/__init__.py
@@ -19,14 +20,18 @@
 src/anutils/scutils/data/data.py
 src/anutils/scutils/data/h5ad2mtx.py
 src/anutils/scutils/data/mtx2rds.R
 src/anutils/scutils/external/__init__.py
 src/anutils/scutils/external/integration/__init__.py
 src/anutils/scutils/external/integration/harmony.py
 src/anutils/scutils/external/integration/harmony_matrix.R
+src/anutils/scutils/external/integration/integration.py
+src/anutils/scutils/external/integration/scalex.py
+src/anutils/scutils/external/integration/scvi.py
 src/anutils/scutils/external/integration/seurat.R
 src/anutils/scutils/external/integration/seurat.py
+src/anutils/scutils/resources/gene_sets/regev_lab_cell_cycle_genes.txt
 src/anutils/scutils/sc_cuda/__init__.py
 src/anutils/scutils/sc_cuda/rapids_scanpy_funcs.py
 src/anutils/scutils/sc_cuda/scanpy_cuda.py
 src/anutils/scutils/sc_cuda/scib_cuda.py
 tests/run_tests.py
```

### Comparing `anutils-0.4.1/tests/run_tests.py` & `anutils-0.4.3b0/tests/run_tests.py`

 * *Files identical despite different names*


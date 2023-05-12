# Comparing `tmp/gmltools-0.0.61.tar.gz` & `tmp/gmltools-0.0.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.61.tar", last modified: Sun Apr 30 15:57:57 2023, max compression
+gzip compressed data, was "gmltools-0.0.62.tar", last modified: Fri May 12 09:22:20 2023, max compression
```

## Comparing `gmltools-0.0.61.tar` & `gmltools-0.0.62.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 15:57:57.920664 gmltools-0.0.61/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.61/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.61/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-04-30 15:57:57.919658 gmltools-0.0.61/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.61/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 15:57:57.633862 gmltools-0.0.61/dist/
--rw-rw-rw-   0        0        0    74791 2023-04-14 10:52:54.000000 gmltools-0.0.61/dist/gmltools-0.0.59.tar.gz
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.61/gmltools.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.61/mltools.yml
--rw-rw-rw-   0        0        0      546 2023-04-30 15:56:07.000000 gmltools-0.0.61/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-30 15:57:57.920664 gmltools-0.0.61/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-04-30 15:55:59.000000 gmltools-0.0.61/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 15:57:57.563552 gmltools-0.0.61/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 15:57:57.659415 gmltools-0.0.61/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.61/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.61/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 15:57:57.727767 gmltools-0.0.61/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.61/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    40126 2023-04-17 07:50:02.000000 gmltools-0.0.61/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-04-30 15:57:57.828422 gmltools-0.0.61/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.61/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.61/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.61/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0     5143 2023-04-14 11:04:34.000000 gmltools-0.0.61/src/gmltools/models/dummy_model.py
--rw-rw-rw-   0        0        0   119074 2023-04-30 15:55:22.000000 gmltools-0.0.61/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.61/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0    12799 2023-04-14 10:43:53.000000 gmltools-0.0.61/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-04-30 15:57:57.866742 gmltools-0.0.61/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.61/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.61/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.61/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-04-30 15:57:57.916638 gmltools-0.0.61/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.61/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.61/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.61/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.61/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-04-30 15:57:57.706203 gmltools-0.0.61/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-04-30 15:57:56.000000 gmltools-0.0.61/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      934 2023-04-30 15:57:57.000000 gmltools-0.0.61/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 15:57:56.000000 gmltools-0.0.61/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-04-30 15:57:56.000000 gmltools-0.0.61/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-30 15:57:56.000000 gmltools-0.0.61/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 09:22:20.317404 gmltools-0.0.62/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.62/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.62/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-05-12 09:22:20.317404 gmltools-0.0.62/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.62/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 09:22:20.092622 gmltools-0.0.62/dist/
+-rw-rw-rw-   0        0        0    74791 2023-04-14 10:52:54.000000 gmltools-0.0.62/dist/gmltools-0.0.59.tar.gz
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.62/gmltools.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.62/mltools.yml
+-rw-rw-rw-   0        0        0      546 2023-05-12 09:21:23.000000 gmltools-0.0.62/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-12 09:22:20.317404 gmltools-0.0.62/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-05-12 09:21:04.000000 gmltools-0.0.62/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:22:20.043668 gmltools-0.0.62/src/
+drwxrwxrwx   0        0        0        0 2023-05-12 09:22:20.099603 gmltools-0.0.62/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.62/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.62/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:22:20.138515 gmltools-0.0.62/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.62/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    40126 2023-04-17 07:50:02.000000 gmltools-0.0.62/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:22:20.258306 gmltools-0.0.62/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.62/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.62/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.62/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0     5143 2023-04-14 11:04:34.000000 gmltools-0.0.62/src/gmltools/models/dummy_model.py
+-rw-rw-rw-   0        0        0   119114 2023-05-09 11:31:39.000000 gmltools-0.0.62/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.62/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0    13212 2023-05-12 09:20:42.000000 gmltools-0.0.62/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:22:20.292445 gmltools-0.0.62/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.62/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.62/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.62/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:22:20.316401 gmltools-0.0.62/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.62/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.62/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.62/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.62/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:22:20.123408 gmltools-0.0.62/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-05-12 09:22:19.000000 gmltools-0.0.62/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      934 2023-05-12 09:22:19.000000 gmltools-0.0.62/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 09:22:19.000000 gmltools-0.0.62/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-05-12 09:22:19.000000 gmltools-0.0.62/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-12 09:22:19.000000 gmltools-0.0.62/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.61/LICENSE` & `gmltools-0.0.62/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.61/Models.ipynb` & `gmltools-0.0.62/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.61/PKG-INFO` & `gmltools-0.0.62/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.61
+Version: 0.0.62
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.61/README.md` & `gmltools-0.0.62/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.61/dist/gmltools-0.0.59.tar.gz` & `gmltools-0.0.62/dist/gmltools-0.0.59.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.61/gmltools.yml` & `gmltools-0.0.62/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.61/mltools.yml` & `gmltools-0.0.62/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.61/pyproject.toml` & `gmltools-0.0.62/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.61"
+version = "0.0.62"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.61/setup.py` & `gmltools-0.0.62/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.61',
+    'version': '0.0.62',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.61/src/gmltools/To_Do.txt` & `gmltools-0.0.62/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.61/src/gmltools/eda/eda.py` & `gmltools-0.0.62/src/gmltools/eda/eda.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.61/src/gmltools/models/bayes.py` & `gmltools-0.0.62/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.61/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.62/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.61/src/gmltools/models/dummy_model.py` & `gmltools-0.0.62/src/gmltools/models/dummy_model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.61/src/gmltools/models/model.py` & `gmltools-0.0.62/src/gmltools/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1822,14 +1822,15 @@
             if os.path.isfile(file_path):
                 df_summary = pd.read_excel(file_path, sheet_name='Sheet2')
                 df_summary = pd.concat([df_summary, df_best], axis=0,ignore_index=True)
                 df_summary.to_excel(file_path, index=False, sheet_name='Sheet2')
             else:
                 df_best.to_excel(file_path, index=False, sheet_name='Sheet2')
             if return_best_metrics:
+                self.results = df_best
                 return df_best
             
 
     def load(self):
 
         """
         Loads a model from a file.
```

### Comparing `gmltools-0.0.61/src/gmltools/models/models_info.py` & `gmltools-0.0.62/src/gmltools/models/models_info.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.61/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.62/src/gmltools/models/timeseriesplit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import numpy as np
 import matplotlib.pyplot as plt
+import re
+import pandas as pd
 
 class BlockingTimeSeriesSplit():
 
     """
     BlockingTimeSeriesSplit is a variation of TimeSeriesSplit that splits the data into n_splits blocks of equal size.
     https://towardsdatascience.com/4-things-to-do-when-applying-cross-validation-with-time-series-c6a5674ebf3a
     https://neptune.ai/blog/cross-validation-mistakes
@@ -118,14 +120,18 @@
                 and `n_features` is the number of features.
         Yields: 
             train : ndarray
                 The training set indices for that split.
             test : ndarray
                 The testing set indices for that split.
         """
+        if isinstance(self.initial, str):
+            assert re.match(r"^\d{4}-\d{2}-\d{2}$", self.initial) or re.match(r"^\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2}$", self.initial), "date format should be YYYY-MM-DD or YYYY-MM-DD HH:MM:SS, the same index as dataframe"
+            #obatin the iloc index of self.initial date
+            self.initial = X.index.get_loc(self.initial)
         n_samples = len(X)
         initial = self.initial
         gap = self.gap
         intra_gap=self.intra_gap
         increment_size = self.increment_size
 
         # Make sure we have enough samples for the given split parameters
```

### Comparing `gmltools-0.0.61/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.62/src/gmltools/models_analysis/classification_analysis.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.61/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.62/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.61/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.62/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.61/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.62/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.61/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.62/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.61/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.62/src/gmltools.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.61
+Version: 0.0.62
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.61/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.62/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*


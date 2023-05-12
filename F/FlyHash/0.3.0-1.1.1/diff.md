# Comparing `tmp/FlyHash-0.3.0.tar.gz` & `tmp/FlyHash-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlyHash-0.3.0.tar", last modified: Wed May 10 05:50:24 2023, max compression
+gzip compressed data, was "FlyHash-1.1.1.tar", last modified: Fri May 12 08:17:50 2023, max compression
```

## Comparing `FlyHash-0.3.0.tar` & `FlyHash-1.1.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:50:24.081652 FlyHash-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-10 05:49:39.000000 FlyHash-0.3.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-10 05:49:39.000000 FlyHash-0.3.0/.cz.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:50:24.077652 FlyHash-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:50:24.077652 FlyHash-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-10 05:49:39.000000 FlyHash-0.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-10 05:49:39.000000 FlyHash-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 05:49:39.000000 FlyHash-0.3.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-10 05:49:39.000000 FlyHash-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-10 05:49:39.000000 FlyHash-0.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-10 05:49:39.000000 FlyHash-0.3.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-10 05:49:39.000000 FlyHash-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-05-10 05:49:39.000000 FlyHash-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-10 05:49:39.000000 FlyHash-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-10 05:50:24.081652 FlyHash-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-10 05:49:39.000000 FlyHash-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:50:24.081652 FlyHash-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-10 05:49:39.000000 FlyHash-0.3.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:50:24.081652 FlyHash-0.3.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-10 05:49:39.000000 FlyHash-0.3.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-10 05:49:39.000000 FlyHash-0.3.0/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-10 05:49:39.000000 FlyHash-0.3.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-05-10 05:49:39.000000 FlyHash-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-10 05:49:39.000000 FlyHash-0.3.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-10 05:49:39.000000 FlyHash-0.3.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-10 05:49:39.000000 FlyHash-0.3.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 05:49:39.000000 FlyHash-0.3.0/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-10 05:49:39.000000 FlyHash-0.3.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-10 05:49:39.000000 FlyHash-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-10 05:49:39.000000 FlyHash-0.3.0/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-10 05:50:24.081652 FlyHash-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-10 05:49:39.000000 FlyHash-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:50:24.077652 FlyHash-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:50:24.081652 FlyHash-0.3.0/src/FlyHash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-10 05:50:24.000000 FlyHash-0.3.0/src/FlyHash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-10 05:50:24.000000 FlyHash-0.3.0/src/FlyHash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 05:50:24.000000 FlyHash-0.3.0/src/FlyHash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 05:50:23.000000 FlyHash-0.3.0/src/FlyHash.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-10 05:50:24.000000 FlyHash-0.3.0/src/FlyHash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 05:50:24.000000 FlyHash-0.3.0/src/FlyHash.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:50:24.081652 FlyHash-0.3.0/src/flyhash/
--rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-05-10 05:49:39.000000 FlyHash-0.3.0/src/flyhash/FlyHash.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-10 05:49:39.000000 FlyHash-0.3.0/src/flyhash/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:50:24.081652 FlyHash-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-10 05:49:39.000000 FlyHash-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-10 05:49:39.000000 FlyHash-0.3.0/tests/test_FlyHash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-10 05:49:39.000000 FlyHash-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:17:50.289327 FlyHash-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-12 08:16:55.000000 FlyHash-1.1.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-12 08:16:55.000000 FlyHash-1.1.1/.cz.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:17:50.281326 FlyHash-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:17:50.285327 FlyHash-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-12 08:16:55.000000 FlyHash-1.1.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-12 08:16:55.000000 FlyHash-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-12 08:16:55.000000 FlyHash-1.1.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-12 08:16:55.000000 FlyHash-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-12 08:16:55.000000 FlyHash-1.1.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-12 08:16:55.000000 FlyHash-1.1.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-12 08:16:55.000000 FlyHash-1.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-05-12 08:16:55.000000 FlyHash-1.1.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-12 08:16:55.000000 FlyHash-1.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-12 08:17:50.289327 FlyHash-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-12 08:16:55.000000 FlyHash-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:17:50.285327 FlyHash-1.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-12 08:16:55.000000 FlyHash-1.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:17:50.285327 FlyHash-1.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-12 08:16:55.000000 FlyHash-1.1.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-12 08:16:55.000000 FlyHash-1.1.1/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-12 08:16:55.000000 FlyHash-1.1.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-05-12 08:16:55.000000 FlyHash-1.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-12 08:16:55.000000 FlyHash-1.1.1/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-12 08:16:55.000000 FlyHash-1.1.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-12 08:16:55.000000 FlyHash-1.1.1/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-12 08:16:55.000000 FlyHash-1.1.1/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-12 08:16:55.000000 FlyHash-1.1.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-12 08:16:55.000000 FlyHash-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-12 08:16:55.000000 FlyHash-1.1.1/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-12 08:17:50.289327 FlyHash-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-12 08:16:55.000000 FlyHash-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:17:50.281326 FlyHash-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:17:50.285327 FlyHash-1.1.1/src/FlyHash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-12 08:17:50.000000 FlyHash-1.1.1/src/FlyHash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-12 08:17:50.000000 FlyHash-1.1.1/src/FlyHash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 08:17:50.000000 FlyHash-1.1.1/src/FlyHash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 08:17:50.000000 FlyHash-1.1.1/src/FlyHash.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-12 08:17:50.000000 FlyHash-1.1.1/src/FlyHash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-12 08:17:50.000000 FlyHash-1.1.1/src/FlyHash.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:17:50.285327 FlyHash-1.1.1/src/flyhash/
+-rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-05-12 08:16:55.000000 FlyHash-1.1.1/src/flyhash/FlyHash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-12 08:16:55.000000 FlyHash-1.1.1/src/flyhash/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:17:50.289327 FlyHash-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-12 08:16:55.000000 FlyHash-1.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-12 08:16:55.000000 FlyHash-1.1.1/tests/test_FlyHash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-12 08:16:55.000000 FlyHash-1.1.1/tox.ini
```

### Comparing `FlyHash-0.3.0/.coveragerc` & `FlyHash-1.1.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `FlyHash-0.3.0/.github/workflows/ci.yml` & `FlyHash-1.1.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `FlyHash-0.3.0/.gitignore` & `FlyHash-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `FlyHash-0.3.0/.pre-commit-config.yaml` & `FlyHash-1.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `FlyHash-0.3.0/.readthedocs.yml` & `FlyHash-1.1.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `FlyHash-0.3.0/CONTRIBUTING.md` & `FlyHash-1.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `FlyHash-0.3.0/LICENSE.txt` & `FlyHash-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FlyHash-0.3.0/PKG-INFO` & `FlyHash-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: FlyHash
-Version: 0.3.0
+Version: 1.1.1
 Summary: A novel hashing algorithm based on "A neural algorithm for a fundamental computing problem" by S. Dasgupta, C. F. Stevens, and S. Navlakha (2017)
 Home-page: https://github.com/TeddyHuang-00/FlyHash
 Author: TeddyHuang-00
 Author-email: teddyhuangnan@gmail.com
 License: MIT
 Project-URL: Documentation, https://flyhash.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/TeddyHuang-00/FlyHash/
 Project-URL: Changelog, https://flyhash.readthedocs.io/en/latest/changelog.html
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
+Requires-Python: <3.12,>=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: testing
 License-File: LICENSE.txt
 
-[![ReadTheDocs](https://readthedocs.org/projects/FlyHash/badge/?version=latest)](https://FlyHash.readthedocs.io/en/latest/)
+[![Documentation Status](https://readthedocs.org/projects/flyhash/badge/?version=latest)](https://flyhash.readthedocs.io/en/latest/?badge=latest)
 [![Coveralls](https://img.shields.io/coveralls/github/TeddyHuang-00/FlyHash/main.svg)](https://coveralls.io/r/TeddyHuang-00/FlyHash)
 [![PyPI-Server](https://img.shields.io/pypi/v/FlyHash.svg)](https://pypi.org/project/FlyHash/)
 [![Monthly Downloads](https://pepy.tech/badge/FlyHash/month)](https://pepy.tech/project/FlyHash)
 [![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
 
 # FlyHash
```

### Comparing `FlyHash-0.3.0/README.md` & `FlyHash-1.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![ReadTheDocs](https://readthedocs.org/projects/FlyHash/badge/?version=latest)](https://FlyHash.readthedocs.io/en/latest/)
+[![Documentation Status](https://readthedocs.org/projects/flyhash/badge/?version=latest)](https://flyhash.readthedocs.io/en/latest/?badge=latest)
 [![Coveralls](https://img.shields.io/coveralls/github/TeddyHuang-00/FlyHash/main.svg)](https://coveralls.io/r/TeddyHuang-00/FlyHash)
 [![PyPI-Server](https://img.shields.io/pypi/v/FlyHash.svg)](https://pypi.org/project/FlyHash/)
 [![Monthly Downloads](https://pepy.tech/badge/FlyHash/month)](https://pepy.tech/project/FlyHash)
 [![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
 
 # FlyHash
```

### Comparing `FlyHash-0.3.0/docs/Makefile` & `FlyHash-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `FlyHash-0.3.0/docs/conf.py` & `FlyHash-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `FlyHash-0.3.0/setup.cfg` & `FlyHash-1.1.1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -19,17 +19,19 @@
 
 [options]
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
+python_requires = >=3.7,<3.12
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	numpy>=1.19.5,<2.0.0
+	scipy>=1.6.0,<2.0.0
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `FlyHash-0.3.0/setup.py` & `FlyHash-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `FlyHash-0.3.0/src/FlyHash.egg-info/PKG-INFO` & `FlyHash-1.1.1/src/FlyHash.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: FlyHash
-Version: 0.3.0
+Version: 1.1.1
 Summary: A novel hashing algorithm based on "A neural algorithm for a fundamental computing problem" by S. Dasgupta, C. F. Stevens, and S. Navlakha (2017)
 Home-page: https://github.com/TeddyHuang-00/FlyHash
 Author: TeddyHuang-00
 Author-email: teddyhuangnan@gmail.com
 License: MIT
 Project-URL: Documentation, https://flyhash.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/TeddyHuang-00/FlyHash/
 Project-URL: Changelog, https://flyhash.readthedocs.io/en/latest/changelog.html
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
+Requires-Python: <3.12,>=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: testing
 License-File: LICENSE.txt
 
-[![ReadTheDocs](https://readthedocs.org/projects/FlyHash/badge/?version=latest)](https://FlyHash.readthedocs.io/en/latest/)
+[![Documentation Status](https://readthedocs.org/projects/flyhash/badge/?version=latest)](https://flyhash.readthedocs.io/en/latest/?badge=latest)
 [![Coveralls](https://img.shields.io/coveralls/github/TeddyHuang-00/FlyHash/main.svg)](https://coveralls.io/r/TeddyHuang-00/FlyHash)
 [![PyPI-Server](https://img.shields.io/pypi/v/FlyHash.svg)](https://pypi.org/project/FlyHash/)
 [![Monthly Downloads](https://pepy.tech/badge/FlyHash/month)](https://pepy.tech/project/FlyHash)
 [![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
 
 # FlyHash
```

### Comparing `FlyHash-0.3.0/src/FlyHash.egg-info/SOURCES.txt` & `FlyHash-1.1.1/src/FlyHash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlyHash-0.3.0/src/flyhash/FlyHash.py` & `FlyHash-1.1.1/src/flyhash/FlyHash.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Optional, Union
 
 import numpy as np
+from scipy import sparse
 
 __author__ = "TeddyHuang-00"
 __copyright__ = "TeddyHuang-00"
 __license__ = "MIT"
 
 
 class FlyHash:
@@ -112,15 +113,14 @@
         assert np.issubdtype(
             self.dtype, np.integer
         ), "dtype must be one of np.integer type"
         self.seed = seed
 
         self.rng = np.random.default_rng(self.seed)
 
-        self.projection_matrix = np.zeros((self.hash_dim, self.input_dim), dtype=bool)
         self._construct_projection_matrix()
 
     def __call__(self, input_data: np.ndarray) -> np.ndarray:
         """Hash input_data to hash_dim vector(s).
 
         Parameters
         ----------
@@ -161,28 +161,39 @@
             hash embeddings non-deterministic.
         """
         if isinstance(self.density, int):
             assert self.density <= self.hash_dim, "density must be less than hash_dim"
             # Create fixed number of connections when density is an integer.
             # Each column of the projection matrix has exactly density non-zero entries.
             # The non-zero entries are all 1.
-            for idx in range(self.hash_dim):
-                self.projection_matrix[
-                    idx, self.rng.choice(self.input_dim, self.density, replace=False)
-                ] = True
+            col = np.concatenate(
+                [
+                    self.rng.choice(self.input_dim, self.density, replace=False)
+                    for _ in range(self.hash_dim)
+                ]
+            )
+            row = np.repeat(np.arange(self.hash_dim), self.density)
+            self.projection_matrix = sparse.csr_matrix(
+                (np.ones_like(row, dtype=bool), (row, col)),
+                shape=(self.hash_dim, self.input_dim),
+            )
         else:
             # Create variable number of connections when density is a float.
             # Each column of the projection matrix has non-zero entries
             # with probability density.
             # The non-zero entries are all 1.
-            self.projection_matrix = self.rng.choice(
-                [False, True],
-                size=(self.hash_dim, self.input_dim),
-                p=[1 - self.density, self.density],
-            )
+            self.projection_matrix: sparse.csr_matrix = sparse.random(
+                self.hash_dim,
+                self.input_dim,
+                self.density,
+                format="csr",
+                random_state=self.rng,
+                dtype=bool,
+                data_rvs=lambda n: np.ones(n, dtype=bool),
+            ).tocsr()
 
     def _winner_take_all(self, input_vector: np.ndarray) -> np.ndarray:
         """Winner-take-all operation.
 
         This also includes quantization step using `quant_step` if specified,
         to reduce the number of unique values.
```

### Comparing `FlyHash-0.3.0/src/flyhash/__init__.py` & `FlyHash-1.1.1/src/flyhash/__init__.py`

 * *Files identical despite different names*

### Comparing `FlyHash-0.3.0/tests/test_FlyHash.py` & `FlyHash-1.1.1/tests/test_FlyHash.py`

 * *Files 11% similar despite different names*

```diff
@@ -132,19 +132,25 @@
     assert random_vector.shape == (normal_hash_dim,)
     assert random_matrix.dtype == normal_dtype
 
     # Test random seed
     hasher_1 = FlyHash(normal_input_dim, normal_hash_dim, seed=normal_seed)
     hasher_2 = FlyHash(normal_input_dim, normal_hash_dim, seed=normal_seed)
     assert np.all(hasher_1(normal_matrix_data) == hasher_2(normal_matrix_data))
-    assert np.all(hasher_1.projection_matrix == hasher_2.projection_matrix)
+    assert not np.any(
+        (hasher_1.projection_matrix != hasher_2.projection_matrix).data  # type: ignore
+    )
     hasher_2.reset()
-    assert not np.all(hasher_1.projection_matrix == hasher_2.projection_matrix)
+    assert np.any(
+        (hasher_1.projection_matrix != hasher_2.projection_matrix).data  # type: ignore
+    )
     hasher_2.reset(normal_seed + 1)
-    assert not np.all(hasher_1.projection_matrix == hasher_2.projection_matrix)
+    assert np.any(
+        (hasher_1.projection_matrix != hasher_2.projection_matrix).data  # type: ignore
+    )
 
     # Test clipping
     binary_clip_hasher = FlyHash(
         normal_input_dim,
         normal_hash_dim,
         sparsity=normal_sparsity,
         quant_step=None,
```

### Comparing `FlyHash-0.3.0/tox.ini` & `FlyHash-1.1.1/tox.ini`

 * *Files identical despite different names*


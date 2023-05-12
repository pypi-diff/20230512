# Comparing `tmp/antimeridian-0.2.3.tar.gz` & `tmp/antimeridian-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antimeridian-0.2.3.tar", last modified: Fri Apr 28 18:54:00 2023, max compression
+gzip compressed data, was "antimeridian-0.2.4.tar", last modified: Fri May 12 16:01:39 2023, max compression
```

## Comparing `antimeridian-0.2.3.tar` & `antimeridian-0.2.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:54:00.440942 antimeridian-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-04-28 18:53:50.000000 antimeridian-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-28 18:54:00.440942 antimeridian-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-28 18:53:50.000000 antimeridian-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-28 18:53:50.000000 antimeridian-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 18:54:00.440942 antimeridian-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:54:00.436942 antimeridian-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:54:00.436942 antimeridian-0.2.3/src/antimeridian/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-28 18:53:50.000000 antimeridian-0.2.3/src/antimeridian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-28 18:53:50.000000 antimeridian-0.2.3/src/antimeridian/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15349 2023-04-28 18:53:50.000000 antimeridian-0.2.3/src/antimeridian/_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:54:00.436942 antimeridian-0.2.3/src/antimeridian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-28 18:54:00.000000 antimeridian-0.2.3/src/antimeridian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-28 18:54:00.000000 antimeridian-0.2.3/src/antimeridian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 18:54:00.000000 antimeridian-0.2.3/src/antimeridian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-28 18:54:00.000000 antimeridian-0.2.3/src/antimeridian.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-28 18:54:00.000000 antimeridian-0.2.3/src/antimeridian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 18:54:00.000000 antimeridian-0.2.3/src/antimeridian.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:54:00.440942 antimeridian-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-28 18:53:50.000000 antimeridian-0.2.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-28 18:53:50.000000 antimeridian-0.2.3/tests/test_geojson.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-28 18:53:50.000000 antimeridian-0.2.3/tests/test_multi_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-28 18:53:50.000000 antimeridian-0.2.3/tests/test_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-28 18:53:50.000000 antimeridian-0.2.3/tests/test_segment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:39.228834 antimeridian-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-05-12 16:01:28.000000 antimeridian-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-12 16:01:39.228834 antimeridian-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-12 16:01:28.000000 antimeridian-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-12 16:01:28.000000 antimeridian-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 16:01:39.228834 antimeridian-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:39.224834 antimeridian-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:39.224834 antimeridian-0.2.4/src/antimeridian/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-12 16:01:28.000000 antimeridian-0.2.4/src/antimeridian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-12 16:01:28.000000 antimeridian-0.2.4/src/antimeridian/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15349 2023-05-12 16:01:28.000000 antimeridian-0.2.4/src/antimeridian/_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:39.228834 antimeridian-0.2.4/src/antimeridian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-12 16:01:39.000000 antimeridian-0.2.4/src/antimeridian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-12 16:01:39.000000 antimeridian-0.2.4/src/antimeridian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 16:01:39.000000 antimeridian-0.2.4/src/antimeridian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-12 16:01:39.000000 antimeridian-0.2.4/src/antimeridian.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-12 16:01:39.000000 antimeridian-0.2.4/src/antimeridian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-12 16:01:39.000000 antimeridian-0.2.4/src/antimeridian.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:01:39.228834 antimeridian-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-12 16:01:28.000000 antimeridian-0.2.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-12 16:01:28.000000 antimeridian-0.2.4/tests/test_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-12 16:01:28.000000 antimeridian-0.2.4/tests/test_multi_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-12 16:01:28.000000 antimeridian-0.2.4/tests/test_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-12 16:01:28.000000 antimeridian-0.2.4/tests/test_segment.py
```

### Comparing `antimeridian-0.2.3/LICENSE` & `antimeridian-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.3/PKG-INFO` & `antimeridian-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antimeridian
-Version: 0.2.3
+Version: 0.2.4
 Summary: Fix GeoJSON geometries that cross the antimeridian
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: documentation, https://antimeridian.readthedocs.io
 Project-URL: repository, https://github.com/gadomski/antimeridan
 Project-URL: changelog, https://github.com/gadomski/antimeridian/blob/main/CHANGELOG.md
 Keywords: geojson,antimeridian,shapely
@@ -16,15 +16,15 @@
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 # antimeridian
 
 [![CI Status](https://img.shields.io/github/actions/workflow/status/gadomski/antimeridian/ci.yaml?style=for-the-badge&label=CI)](https://github.com/gadomski/antimeridian/actions/workflows/ci.yaml)
-[![Read the Docs](https://img.shields.io/readthedocs/antimeridian?style=for-the-badge)](https://antimeridian.readthedocs.io/en/latest/)
+[![Read the Docs](https://img.shields.io/readthedocs/antimeridian?style=for-the-badge)](https://antimeridian.readthedocs.io/en/stable/)
 [![PyPI](https://img.shields.io/pypi/v/antimeridian?style=for-the-badge)](https://pypi.org/project/antimeridian/)
 
 [![GitHub](https://img.shields.io/github/license/gadomski/antimeridian?style=for-the-badge)](https://github.com/gadomski/antimeridian/blob/main/LICENSE)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg?style=for-the-badge)](https://github.com/gadomski/antimeridian/blob/main/CODE_OF_CONDUCT)
 
 Fix polygons that cross the antimeridian.
 See [the documentation](https://antimeridian.readthedocs.io) for information about the underlying algorithm.
@@ -42,14 +42,15 @@
 pip install antimeridian
 ```
 
 Then:
 
 ```python
 import antimeridian
+
 fixed = antimeridian.fix_geojson(geojson)
 ```
 
 ### Command line interface
 
 Use the `cli` optional dependency to install the `antimeridian` CLI:
```

### Comparing `antimeridian-0.2.3/README.md` & `antimeridian-0.2.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # antimeridian
 
 [![CI Status](https://img.shields.io/github/actions/workflow/status/gadomski/antimeridian/ci.yaml?style=for-the-badge&label=CI)](https://github.com/gadomski/antimeridian/actions/workflows/ci.yaml)
-[![Read the Docs](https://img.shields.io/readthedocs/antimeridian?style=for-the-badge)](https://antimeridian.readthedocs.io/en/latest/)
+[![Read the Docs](https://img.shields.io/readthedocs/antimeridian?style=for-the-badge)](https://antimeridian.readthedocs.io/en/stable/)
 [![PyPI](https://img.shields.io/pypi/v/antimeridian?style=for-the-badge)](https://pypi.org/project/antimeridian/)
 
 [![GitHub](https://img.shields.io/github/license/gadomski/antimeridian?style=for-the-badge)](https://github.com/gadomski/antimeridian/blob/main/LICENSE)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg?style=for-the-badge)](https://github.com/gadomski/antimeridian/blob/main/CODE_OF_CONDUCT)
 
 Fix polygons that cross the antimeridian.
 See [the documentation](https://antimeridian.readthedocs.io) for information about the underlying algorithm.
@@ -23,14 +23,15 @@
 pip install antimeridian
 ```
 
 Then:
 
 ```python
 import antimeridian
+
 fixed = antimeridian.fix_geojson(geojson)
 ```
 
 ### Command line interface
 
 Use the `cli` optional dependency to install the `antimeridian` CLI:
```

### Comparing `antimeridian-0.2.3/pyproject.toml` & `antimeridian-0.2.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,65 @@
 [build-system]
 requires = ["setuptools >= 64"]
 
 [project]
 name = "antimeridian"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
     {name = "Pete Gadomski", email = "pete.gadomski@gmail.com"}
 ]
 description = "Fix GeoJSON geometries that cross the antimeridian"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["geojson", "antimeridian", "shapely"]
 license = {text = "Apache-2.0"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
 ]
 dependencies = [
-    "shapely>=1.8"
+    "shapely>=2.0"
 ]
 
 [project.urls]
 documentation = "https://antimeridian.readthedocs.io"
 repository = "https://github.com/gadomski/antimeridan"
 changelog = "https://github.com/gadomski/antimeridian/blob/main/CHANGELOG.md"
 
 [project.optional-dependencies]
 cli = [
     "click~=8.1"
 ]
 dev = [
     "black~=23.3",
+    "blacken-docs~=1.13",
     "mypy~=1.2",
+    "packaging~=23.1",
     "pre-commit~=3.2",
     "pytest~=7.3",
     "pytest-console-scripts~=1.3",
-    "ruff==0.0.262",
+    "ruff==0.0.265",
+    "tomli~=2.0; python_version<'3.11'"
 ]
 docs = [
     "cartopy~=0.21",
     "ipykernel~=6.22",
     "jupytext~=1.14",
     "nbsphinx~=0.9",
     "pydata-sphinx-theme~=0.13",
     "scipy~=1.10",
-    "sphinx~=6.1",
+    "sphinx>=6.1,<8.0",
     "sphinx-click~=4.4",
 ]
 
 [project.scripts]
 antimeridian = "antimeridian._cli:cli"
 
+[tool.ruff]
+select = ["F", "E", "W", "I", "ERA", "RUF"]
+
 [tool.mypy]
 strict = true
 
 [[tool.mypy.overrides]]
 module = ["shapely", "shapely.geometry"]
 ignore_missing_imports = true
```

### Comparing `antimeridian-0.2.3/src/antimeridian/_cli.py` & `antimeridian-0.2.4/src/antimeridian/_cli.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.3/src/antimeridian/_implementation.py` & `antimeridian-0.2.4/src/antimeridian/_implementation.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.3/src/antimeridian.egg-info/PKG-INFO` & `antimeridian-0.2.4/src/antimeridian.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antimeridian
-Version: 0.2.3
+Version: 0.2.4
 Summary: Fix GeoJSON geometries that cross the antimeridian
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: documentation, https://antimeridian.readthedocs.io
 Project-URL: repository, https://github.com/gadomski/antimeridan
 Project-URL: changelog, https://github.com/gadomski/antimeridian/blob/main/CHANGELOG.md
 Keywords: geojson,antimeridian,shapely
@@ -16,15 +16,15 @@
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 # antimeridian
 
 [![CI Status](https://img.shields.io/github/actions/workflow/status/gadomski/antimeridian/ci.yaml?style=for-the-badge&label=CI)](https://github.com/gadomski/antimeridian/actions/workflows/ci.yaml)
-[![Read the Docs](https://img.shields.io/readthedocs/antimeridian?style=for-the-badge)](https://antimeridian.readthedocs.io/en/latest/)
+[![Read the Docs](https://img.shields.io/readthedocs/antimeridian?style=for-the-badge)](https://antimeridian.readthedocs.io/en/stable/)
 [![PyPI](https://img.shields.io/pypi/v/antimeridian?style=for-the-badge)](https://pypi.org/project/antimeridian/)
 
 [![GitHub](https://img.shields.io/github/license/gadomski/antimeridian?style=for-the-badge)](https://github.com/gadomski/antimeridian/blob/main/LICENSE)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg?style=for-the-badge)](https://github.com/gadomski/antimeridian/blob/main/CODE_OF_CONDUCT)
 
 Fix polygons that cross the antimeridian.
 See [the documentation](https://antimeridian.readthedocs.io) for information about the underlying algorithm.
@@ -42,14 +42,15 @@
 pip install antimeridian
 ```
 
 Then:
 
 ```python
 import antimeridian
+
 fixed = antimeridian.fix_geojson(geojson)
 ```
 
 ### Command line interface
 
 Use the `cli` optional dependency to install the `antimeridian` CLI:
```

### Comparing `antimeridian-0.2.3/tests/test_cli.py` & `antimeridian-0.2.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.3/tests/test_geojson.py` & `antimeridian-0.2.4/tests/test_geojson.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.3/tests/test_multi_polygon.py` & `antimeridian-0.2.4/tests/test_multi_polygon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
+import antimeridian
 import shapely.geometry
 from shapely.geometry import MultiPolygon
 
-import antimeridian
-
 from .conftest import Reader
 
 
 def test_multi_polygon(
     read_input: Reader,
     read_output: Reader,
 ) -> None:
```

### Comparing `antimeridian-0.2.3/tests/test_polygon.py` & `antimeridian-0.2.4/tests/test_polygon.py`

 * *Files identical despite different names*


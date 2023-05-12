# Comparing `tmp/jaraco.packaging-9.1.2.tar.gz` & `tmp/jaraco.packaging-9.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.packaging-9.1.2.tar", last modified: Wed Dec 28 18:05:06 2022, max compression
+gzip compressed data, was "jaraco.packaging-9.2.0.tar", last modified: Fri May 12 19:21:01 2023, max compression
```

## Comparing `jaraco.packaging-9.1.2.tar` & `jaraco.packaging-9.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 18:05:06.805370 jaraco.packaging-9.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2022-12-28 18:04:37.000000 jaraco.packaging-9.1.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2022-12-28 18:04:37.000000 jaraco.packaging-9.1.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      136 2022-12-28 18:04:37.000000 jaraco.packaging-9.1.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 18:05:06.801370 jaraco.packaging-9.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2022-12-28 18:04:37.000000 jaraco.packaging-9.1.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 18:05:06.801370 jaraco.packaging-9.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2022-12-28 18:04:37.000000 jaraco.packaging-9.1.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2022-12-28 18:04:37.000000 jaraco.packaging-9.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2022-12-28 18:04:37.000000 jaraco.packaging-9.1.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2022-12-28 18:04:37.000000 jaraco.packaging-9.1.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2022-12-28 18:04:37.000000 jaraco.packaging-9.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2022-12-28 18:05:06.805370 jaraco.packaging-9.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2022-12-28 18:04:37.000000 jaraco.packaging-9.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 18:05:06.801370 jaraco.packaging-9.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2022-12-28 18:04:37.000000 jaraco.packaging-9.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2022-12-28 18:04:37.000000 jaraco.packaging-9.1.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      398 2022-12-28 18:04:37.000000 jaraco.packaging-9.1.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 18:05:06.797369 jaraco.packaging-9.1.2/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 18:05:06.805370 jaraco.packaging-9.1.2/jaraco/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-28 18:04:37.000000 jaraco.packaging-9.1.2/jaraco/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2022-12-28 18:04:37.000000 jaraco.packaging-9.1.2/jaraco/packaging/make-tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2022-12-28 18:04:37.000000 jaraco.packaging-9.1.2/jaraco/packaging/sphinx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 18:05:06.801370 jaraco.packaging-9.1.2/jaraco.packaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2022-12-28 18:05:06.000000 jaraco.packaging-9.1.2/jaraco.packaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      539 2022-12-28 18:05:06.000000 jaraco.packaging-9.1.2/jaraco.packaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-28 18:05:06.000000 jaraco.packaging-9.1.2/jaraco.packaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      360 2022-12-28 18:05:06.000000 jaraco.packaging-9.1.2/jaraco.packaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-28 18:05:06.000000 jaraco.packaging-9.1.2/jaraco.packaging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2022-12-28 18:04:37.000000 jaraco.packaging-9.1.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      378 2022-12-28 18:04:37.000000 jaraco.packaging-9.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2022-12-28 18:04:37.000000 jaraco.packaging-9.1.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2022-12-28 18:05:06.805370 jaraco.packaging-9.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      754 2022-12-28 18:04:37.000000 jaraco.packaging-9.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:21:01.214823 jaraco.packaging-9.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:21:01.206822 jaraco.packaging-9.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:21:01.206822 jaraco.packaging-9.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-12 19:21:01.214823 jaraco.packaging-9.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:21:01.210823 jaraco.packaging-9.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:21:01.198822 jaraco.packaging-9.2.0/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:21:01.214823 jaraco.packaging-9.2.0/jaraco/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/jaraco/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/jaraco/packaging/make-tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/jaraco/packaging/sphinx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:21:01.210823 jaraco.packaging-9.2.0/jaraco.packaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-12 19:21:01.000000 jaraco.packaging-9.2.0/jaraco.packaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-12 19:21:01.000000 jaraco.packaging-9.2.0/jaraco.packaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 19:21:01.000000 jaraco.packaging-9.2.0/jaraco.packaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-12 19:21:01.000000 jaraco.packaging-9.2.0/jaraco.packaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 19:21:01.000000 jaraco.packaging-9.2.0/jaraco.packaging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-12 19:21:01.214823 jaraco.packaging-9.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-12 19:20:34.000000 jaraco.packaging-9.2.0/tox.ini
```

### Comparing `jaraco.packaging-9.1.2/.github/workflows/main.yml` & `jaraco.packaging-9.2.0/.github/workflows/main.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 name: tests
 
 on: [push, pull_request]
 
+permissions:
+  contents: read
+
 env:
   # Environment variables to support color support (jaraco/skeleton#66):
   # Request colored output from CLI tools supporting it. Different tools
   # interpret the value differently. For some, just being set is sufficient.
   # For others, it must be a non-zero integer. For yet others, being set
   # to a non-empty value is sufficient. For tox, it must be one of
   # <blank>, 0, 1, false, no, off, on, true, yes. The only enabling value
@@ -100,14 +103,16 @@
     steps:
     - name: Decide whether the needed jobs succeeded or failed
       uses: re-actors/alls-green@release/v1
       with:
         jobs: ${{ toJSON(needs) }}
 
   release:
+    permissions:
+      contents: write
     needs:
     - check
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
```

### Comparing `jaraco.packaging-9.1.2/CHANGES.rst` & `jaraco.packaging-9.2.0/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v9.2.0
+======
+
+#7, #10, #11: Added environment variable to bypass
+building metadata for offline builds.
+
 v9.1.2
 ======
 
 #6: Added minimal test to ``sphinx.packaging``.
 
 v9.1.1
 ======
```

### Comparing `jaraco.packaging-9.1.2/LICENSE` & `jaraco.packaging-9.2.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jaraco.packaging-9.1.2/PKG-INFO` & `jaraco.packaging-9.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.packaging
-Version: 9.1.2
+Version: 9.2.0
 Summary: tools to supplement packaging Python releases
 Home-page: https://github.com/jaraco/jaraco.packaging
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -28,15 +28,15 @@
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracopackaging/badge/?version=latest
    :target: https://jaracopackaging.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 Tools for packaging.
 
 sphinx
 ======
 
@@ -47,19 +47,25 @@
  - project (from name)
  - author
  - copyright (same as author)
  - version
  - release (same as version)
  - package_url (from url)
 
-To enable, include 'jaraco.packaging' in your requirements and add
-'jaraco.packaging.sphinx' to your list of extensions in your config file::
+To enable, include 'jaraco.packaging' in the requirements and add
+'jaraco.packaging.sphinx' to the list of extensions in a Sphinx config
+file::
 
     extensions=['jaraco.packaging.sphinx']
 
+The extension by default builds the project in an isolated environment in
+order to extract the metadata. To build the documentation offline,
+provide an already built wheel by setting the environment variable
+``JARACO_PACKAGING_SPHINX_WHEEL`` to the path of the existing wheel.
+
 make-tree
 =========
 
 A utility for taking output from ``pipdeptree --json`` and producing a tree
 rooted at a given package.
 
 Usage::
```

### Comparing `jaraco.packaging-9.1.2/docs/conf.py` & `jaraco.packaging-9.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.packaging-9.1.2/jaraco/packaging/make-tree.py` & `jaraco.packaging-9.2.0/jaraco/packaging/make-tree.py`

 * *Files identical despite different names*

### Comparing `jaraco.packaging-9.1.2/jaraco/packaging/sphinx.py` & `jaraco.packaging-9.2.0/jaraco/packaging/sphinx.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,43 +3,57 @@
 to conf.py, and the setup hook does the rest.
 
 >>> 'setup' in globals()
 True
 """
 
 import os
-import subprocess
 
 from build.util import project_wheel_metadata as load_metadata
+from jaraco.context import suppress
 
 try:
     import importlib.metadata as metadata
 except ImportError:
     import importlib_metadata as metadata  # type: ignore
 
 
-if 'check_output' not in dir(subprocess):
-    import subprocess32 as subprocess  # type: ignore
-
-
 def setup(app):
     app.add_config_value('package_url', '', '')
     app.connect('builder-inited', load_config_from_setup)
     app.connect('builder-inited', configure_substitutions)
     app.connect('html-page-context', add_package_url)
     return dict(version=metadata.version('jaraco.packaging'), parallel_read_safe=True)
 
 
+@suppress(KeyError)
+def _load_metadata_from_wheel():
+    """
+    If indicated by an environment variable, expect the metadata
+    to be present in a wheel and load it from there, avoiding
+    the build process. Ref jaraco/jaraco.packaging#7.
+
+    >>> _load_metadata_from_wheel()
+    >>> getfixture('static_wheel')
+    >>> meta = _load_metadata_from_wheel()
+    >>> meta['Name']
+    'sampleproject'
+    """
+    wheel = os.environ['JARACO_PACKAGING_SPHINX_WHEEL']
+    (dist,) = metadata.distributions(path=[wheel])
+    return dist.metadata
+
+
 def load_config_from_setup(app):
     """
     Replace values in app.config from package metadata
     """
     # for now, assume project root is one level up
     root = os.path.join(app.confdir, '..')
-    meta = load_metadata(root)
+    meta = _load_metadata_from_wheel() or load_metadata(root)
     app.config.project = meta['Name']
     app.config.version = app.config.release = meta['Version']
     app.config.package_url = meta['Home-page']
     app.config.author = app.config.copyright = meta['Author']
 
 
 def configure_substitutions(app):
```

### Comparing `jaraco.packaging-9.1.2/jaraco.packaging.egg-info/PKG-INFO` & `jaraco.packaging-9.2.0/jaraco.packaging.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.packaging
-Version: 9.1.2
+Version: 9.2.0
 Summary: tools to supplement packaging Python releases
 Home-page: https://github.com/jaraco/jaraco.packaging
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -28,15 +28,15 @@
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracopackaging/badge/?version=latest
    :target: https://jaracopackaging.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 Tools for packaging.
 
 sphinx
 ======
 
@@ -47,19 +47,25 @@
  - project (from name)
  - author
  - copyright (same as author)
  - version
  - release (same as version)
  - package_url (from url)
 
-To enable, include 'jaraco.packaging' in your requirements and add
-'jaraco.packaging.sphinx' to your list of extensions in your config file::
+To enable, include 'jaraco.packaging' in the requirements and add
+'jaraco.packaging.sphinx' to the list of extensions in a Sphinx config
+file::
 
     extensions=['jaraco.packaging.sphinx']
 
+The extension by default builds the project in an isolated environment in
+order to extract the metadata. To build the documentation offline,
+provide an already built wheel by setting the environment variable
+``JARACO_PACKAGING_SPHINX_WHEEL`` to the path of the existing wheel.
+
 make-tree
 =========
 
 A utility for taking output from ``pipdeptree --json`` and producing a tree
 rooted at a given package.
 
 Usage::
```

### Comparing `jaraco.packaging-9.1.2/jaraco.packaging.egg-info/SOURCES.txt` & `jaraco.packaging-9.2.0/jaraco.packaging.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .coveragerc
 .editorconfig
-.flake8
 .pre-commit-config.yaml
 .readthedocs.yaml
 CHANGES.rst
 LICENSE
 README.rst
+conftest.py
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
 tox.ini
 .github/dependabot.yml
 .github/workflows/main.yml
```

### Comparing `jaraco.packaging-9.1.2/setup.cfg` & `jaraco.packaging-9.2.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -16,35 +16,34 @@
 [options]
 packages = find_namespace:
 include_package_data = true
 python_requires = >=3.7
 install_requires = 
 	importlib_metadata; python_version < "3.8"
 	build[virtualenv]
+	jaraco.context
 
 [options.packages.find]
 exclude = 
 	build*
 	dist*
 	docs*
 	tests*
 
 [options.extras_require]
 testing = 
 	pytest >= 6
 	pytest-checkdocs >= 2.4
-	pytest-flake8; \
-	python_version < "3.12"
-	flake8 < 5
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
 	pytest-enabler >= 1.3
+	pytest-ruff
 docs = 
 	sphinx >= 3.5
 	jaraco.packaging >= 9
 	rst.linker >= 1.9
 	furo
 	sphinx-lint
```


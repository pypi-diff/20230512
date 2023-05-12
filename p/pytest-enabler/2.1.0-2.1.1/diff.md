# Comparing `tmp/pytest-enabler-2.1.0.tar.gz` & `tmp/pytest-enabler-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-enabler-2.1.0.tar", last modified: Fri Jan 27 23:34:19 2023, max compression
+gzip compressed data, was "pytest-enabler-2.1.1.tar", last modified: Fri May 12 21:28:15 2023, max compression
```

## Comparing `pytest-enabler-2.1.0.tar` & `pytest-enabler-2.1.1.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 23:34:19.431614 pytest-enabler-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-01-27 23:33:58.000000 pytest-enabler-2.1.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-01-27 23:33:58.000000 pytest-enabler-2.1.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-01-27 23:33:58.000000 pytest-enabler-2.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 23:34:19.431614 pytest-enabler-2.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-01-27 23:33:58.000000 pytest-enabler-2.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 23:34:19.431614 pytest-enabler-2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-01-27 23:33:58.000000 pytest-enabler-2.1.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-01-27 23:33:58.000000 pytest-enabler-2.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-01-27 23:33:58.000000 pytest-enabler-2.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-01-27 23:33:58.000000 pytest-enabler-2.1.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-01-27 23:33:58.000000 pytest-enabler-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-01-27 23:34:19.431614 pytest-enabler-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-01-27 23:33:58.000000 pytest-enabler-2.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 23:34:19.431614 pytest-enabler-2.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-01-27 23:33:58.000000 pytest-enabler-2.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-01-27 23:33:58.000000 pytest-enabler-2.1.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-01-27 23:33:58.000000 pytest-enabler-2.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-01-27 23:33:58.000000 pytest-enabler-2.1.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-01-27 23:33:58.000000 pytest-enabler-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-01-27 23:33:58.000000 pytest-enabler-2.1.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 23:34:19.431614 pytest-enabler-2.1.0/pytest_enabler/
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-01-27 23:33:58.000000 pytest-enabler-2.1.0/pytest_enabler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 23:34:19.431614 pytest-enabler-2.1.0/pytest_enabler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-01-27 23:34:19.000000 pytest-enabler-2.1.0/pytest_enabler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-01-27 23:34:19.000000 pytest-enabler-2.1.0/pytest_enabler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 23:34:19.000000 pytest-enabler-2.1.0/pytest_enabler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-01-27 23:34:19.000000 pytest-enabler-2.1.0/pytest_enabler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-01-27 23:34:19.000000 pytest-enabler-2.1.0/pytest_enabler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-27 23:34:19.000000 pytest-enabler-2.1.0/pytest_enabler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-01-27 23:34:19.431614 pytest-enabler-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 23:34:19.431614 pytest-enabler-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-01-27 23:33:58.000000 pytest-enabler-2.1.0/tests/test_enabler.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-01-27 23:33:58.000000 pytest-enabler-2.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:28:15.444024 pytest-enabler-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:28:15.444024 pytest-enabler-2.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:28:15.444024 pytest-enabler-2.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-12 21:28:15.444024 pytest-enabler-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:28:15.444024 pytest-enabler-2.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:28:15.444024 pytest-enabler-2.1.1/pytest_enabler/
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/pytest_enabler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:28:15.444024 pytest-enabler-2.1.1/pytest_enabler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-12 21:28:15.000000 pytest-enabler-2.1.1/pytest_enabler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-12 21:28:15.000000 pytest-enabler-2.1.1/pytest_enabler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 21:28:15.000000 pytest-enabler-2.1.1/pytest_enabler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 21:28:15.000000 pytest-enabler-2.1.1/pytest_enabler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-12 21:28:15.000000 pytest-enabler-2.1.1/pytest_enabler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-12 21:28:15.000000 pytest-enabler-2.1.1/pytest_enabler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-12 21:28:15.444024 pytest-enabler-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:28:15.444024 pytest-enabler-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/tests/test_enabler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/tox.ini
```

### Comparing `pytest-enabler-2.1.0/.github/workflows/main.yml` & `pytest-enabler-2.1.1/.github/workflows/main.yml`

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
@@ -104,14 +107,16 @@
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

### Comparing `pytest-enabler-2.1.0/CHANGES.rst` & `pytest-enabler-2.1.1/CHANGES.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+v2.1.1
+======
+
+Packaging refresh.
+
 v2.1.0
 ======
 
 Fixed EncodingWarning when PEP 597 warn_default_encoding is enabled.
 
 v2.0.0
 ======
```

### Comparing `pytest-enabler-2.1.0/LICENSE` & `pytest-enabler-2.1.1/LICENSE`

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

### Comparing `pytest-enabler-2.1.0/PKG-INFO` & `pytest-enabler-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-enabler
-Version: 2.1.0
+Version: 2.1.1
 Summary: Enable installed pytest plugins
 Home-page: https://github.com/jaraco/pytest-enabler
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -46,8 +46,9 @@
 
 Known to work with the following plugins:
 
 - pytest-black
 - pytest-cov
 - pytest-flake8
 - pytest-mypy
+- pytest-ruff
 - pytest-xdist
```

### Comparing `pytest-enabler-2.1.0/README.rst` & `pytest-enabler-2.1.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -28,8 +28,9 @@
 
 Known to work with the following plugins:
 
 - pytest-black
 - pytest-cov
 - pytest-flake8
 - pytest-mypy
+- pytest-ruff
 - pytest-xdist
```

### Comparing `pytest-enabler-2.1.0/docs/conf.py` & `pytest-enabler-2.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytest-enabler-2.1.0/pytest.ini` & `pytest-enabler-2.1.1/pytest.ini`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [pytest]
 norecursedirs=dist build .tox .eggs
 addopts=--doctest-modules
 filterwarnings=
+	## upstream
+
 	# Ensure ResourceWarnings are emitted
 	default::ResourceWarning
 
-	# Suppress deprecation warning in flake8
-	ignore:SelectableGroups dict interface is deprecated::flake8
-
 	# shopkeep/pytest-black#55
 	ignore:<class 'pytest_black.BlackItem'> is not using a cooperative constructor:pytest.PytestDeprecationWarning
 	ignore:The \(fspath. py.path.local\) argument to BlackItem is deprecated.:pytest.PytestDeprecationWarning
 	ignore:BlackItem is an Item subclass and should not be a collector:pytest.PytestWarning
 
-	# tholo/pytest-flake8#83
-	ignore:<class 'pytest_flake8.Flake8Item'> is not using a cooperative constructor:pytest.PytestDeprecationWarning
-	ignore:The \(fspath. py.path.local\) argument to Flake8Item is deprecated.:pytest.PytestDeprecationWarning
-	ignore:Flake8Item is an Item subclass and should not be a collector:pytest.PytestWarning
-
 	# shopkeep/pytest-black#67
 	ignore:'encoding' argument not specified::pytest_black
+
+	# realpython/pytest-mypy#152
+	ignore:'encoding' argument not specified::pytest_mypy
+
+	# python/cpython#100750
+	ignore:'encoding' argument not specified::platform
+
+	## end upstream
```

### Comparing `pytest-enabler-2.1.0/pytest_enabler/__init__.py` & `pytest-enabler-2.1.1/pytest_enabler/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-enabler-2.1.0/pytest_enabler.egg-info/PKG-INFO` & `pytest-enabler-2.1.1/pytest_enabler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-enabler
-Version: 2.1.0
+Version: 2.1.1
 Summary: Enable installed pytest plugins
 Home-page: https://github.com/jaraco/pytest-enabler
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -46,8 +46,9 @@
 
 Known to work with the following plugins:
 
 - pytest-black
 - pytest-cov
 - pytest-flake8
 - pytest-mypy
+- pytest-ruff
 - pytest-xdist
```

### Comparing `pytest-enabler-2.1.0/pytest_enabler.egg-info/SOURCES.txt` & `pytest-enabler-2.1.1/pytest_enabler.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 .coveragerc
 .editorconfig
-.flake8
 .pre-commit-config.yaml
 .readthedocs.yaml
 CHANGES.rst
 LICENSE
 README.rst
 mypy.ini
 pyproject.toml
```

### Comparing `pytest-enabler-2.1.0/setup.cfg` & `pytest-enabler-2.1.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -29,23 +29,21 @@
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
 	
 	types-toml
 docs = 
 	sphinx >= 3.5
 	jaraco.packaging >= 9
 	rst.linker >= 1.9
 	furo
```

### Comparing `pytest-enabler-2.1.0/tests/test_enabler.py` & `pytest-enabler-2.1.1/tests/test_enabler.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 def test_pytest_addoption(tmpdir_cur):
     pathlib.Path('pyproject.toml').write_text(
         textwrap.dedent(
             """
             [tool.pytest-enabler.black]
             addopts = "--black"
             """
-        )
+        ),
+        encoding='utf-8',
     )
     config = mock.MagicMock()
     config.pluginmanager.has_plugin = lambda name: name == 'black'
     args = []
     enabler.pytest_load_initial_conftests(config, None, args)
     assert args == ['--black']
```

### Comparing `pytest-enabler-2.1.0/tox.ini` & `pytest-enabler-2.1.1/tox.ini`

 * *Files identical despite different names*


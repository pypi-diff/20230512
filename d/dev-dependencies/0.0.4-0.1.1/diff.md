# Comparing `tmp/dev_dependencies-0.0.4.tar.gz` & `tmp/dev-dependencies-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dev_dependencies-0.0.4.tar", max compression
+gzip compressed data, was "dev-dependencies-0.1.1.tar", last modified: Thu Apr 27 15:06:26 2023, max compression
```

## Comparing `dev_dependencies-0.0.4.tar` & `dev-dependencies-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,26 @@
--rw-r--r--   0        0        0     1069 2023-05-12 16:19:41.280124 dev_dependencies-0.0.4/LICENSE
--rw-r--r--   0        0        0      839 2023-05-12 16:19:41.280124 dev_dependencies-0.0.4/README.md
--rw-r--r--   0        0        0      376 2023-05-12 16:19:41.280124 dev_dependencies-0.0.4/dev_dependencies/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 16:19:41.280124 dev_dependencies-0.0.4/dev_dependencies/py.typed
--rw-r--r--   0        0        0     1343 2023-05-12 16:20:05.100429 dev_dependencies-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1557 1970-01-01 00:00:00.000000 dev_dependencies-0.0.4/PKG-INFO
+drwxr-xr-x   0 justinmills   (501) staff       (20)        0 2023-04-27 15:06:26.370403 dev-dependencies-0.1.1/
+-rw-r--r--   0 justinmills   (501) staff       (20)       14 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/.envrc
+-rw-r--r--   0 justinmills   (501) staff       (20)      255 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/.flake8
+drwxr-xr-x   0 justinmills   (501) staff       (20)        0 2023-04-27 15:06:26.365117 dev-dependencies-0.1.1/.github/
+drwxr-xr-x   0 justinmills   (501) staff       (20)        0 2023-04-27 15:06:26.368474 dev-dependencies-0.1.1/.github/workflows/
+-rw-r--r--   0 justinmills   (501) staff       (20)     1223 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0 justinmills   (501) staff       (20)      192 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/.gitignore
+-rw-r--r--   0 justinmills   (501) staff       (20)        7 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/.python-version
+-rw-r--r--   0 justinmills   (501) staff       (20)     1069 2023-04-26 12:26:45.000000 dev-dependencies-0.1.1/LICENSE
+-rw-r--r--   0 justinmills   (501) staff       (20)      955 2023-04-27 15:06:26.370220 dev-dependencies-0.1.1/PKG-INFO
+-rw-r--r--   0 justinmills   (501) staff       (20)      281 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/Pipfile
+-rw-r--r--   0 justinmills   (501) staff       (20)    38840 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/Pipfile.lock
+-rw-r--r--   0 justinmills   (501) staff       (20)      686 2023-04-27 15:04:07.000000 dev-dependencies-0.1.1/README.md
+drwxr-xr-x   0 justinmills   (501) staff       (20)        0 2023-04-27 15:06:26.369303 dev-dependencies-0.1.1/dev_dependencies.egg-info/
+-rw-r--r--   0 justinmills   (501) staff       (20)      955 2023-04-27 15:06:26.000000 dev-dependencies-0.1.1/dev_dependencies.egg-info/PKG-INFO
+-rw-r--r--   0 justinmills   (501) staff       (20)      381 2023-04-27 15:06:26.000000 dev-dependencies-0.1.1/dev_dependencies.egg-info/SOURCES.txt
+-rw-r--r--   0 justinmills   (501) staff       (20)        1 2023-04-27 15:06:26.000000 dev-dependencies-0.1.1/dev_dependencies.egg-info/dependency_links.txt
+-rw-r--r--   0 justinmills   (501) staff       (20)      120 2023-04-27 15:06:26.000000 dev-dependencies-0.1.1/dev_dependencies.egg-info/requires.txt
+-rw-r--r--   0 justinmills   (501) staff       (20)        8 2023-04-27 15:06:26.000000 dev-dependencies-0.1.1/dev_dependencies.egg-info/top_level.txt
+drwxr-xr-x   0 justinmills   (501) staff       (20)        0 2023-04-27 15:06:26.369710 dev-dependencies-0.1.1/devdeps/
+-rw-r--r--   0 justinmills   (501) staff       (20)      225 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/devdeps/__init__.py
+-rw-r--r--   0 justinmills   (501) staff       (20)      160 2023-04-27 15:06:26.000000 dev-dependencies-0.1.1/devdeps/_version.py
+-rw-r--r--   0 justinmills   (501) staff       (20)     1501 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/pyproject.toml
+-rw-r--r--   0 justinmills   (501) staff       (20)       38 2023-04-27 15:06:26.370456 dev-dependencies-0.1.1/setup.cfg
+drwxr-xr-x   0 justinmills   (501) staff       (20)        0 2023-04-27 15:06:26.369903 dev-dependencies-0.1.1/tests/
+-rw-r--r--   0 justinmills   (501) staff       (20)      273 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/tests/test_version.py
```

### Comparing `dev_dependencies-0.0.4/LICENSE` & `dev-dependencies-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dev_dependencies-0.0.4/README.md` & `dev-dependencies-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -24,17 +24,12 @@
 
 * Tests
 
       pytest
 
 ## Building a package to release
 
-    # Build a distribution (for releases, do this on main with a fresh tag)
     python -m build
 
     # To release that package
     twine upload dist/dev-dependencies-*.tar.gz dist/dev_dependencies-*-py3-none-any.whl
 
-    # To see what the current version will be
-    python -m setuptools_scm
-
-
```

### Comparing `dev_dependencies-0.0.4/pyproject.toml` & `dev-dependencies-0.1.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,65 +1,76 @@
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "dev-dependencies"
+authors = [
+  { name = "Justin Mills" }
+]
+description = "An opinionated library of dev-time dependencies"
+requires-python = ">=3.11"
+keywords = ["library", "dependencies"]
+license = {text = "MIT"}
+dependencies = [
+    "pydantic",
+    "black",
+    "flake8",
+    "flake8-black",
+    "ruff",
+    "mypy",
+    "pydantic",
+    "pytest",
+    "pytest-cov",
+    "pytest-xdist",
+    "pytest-mock",
+    "pytest-md",
+    "pytest-emoji",
+]
+dynamic = ["version", "readme"]
+
+[tool.setuptools]
+packages = ["devdeps"]
+
+[tool.setuptools.dynamic]
+readme = {file = ["README.md"], content-type = "text/markdown"}
+
+[tool.setuptools_scm]
+write_to = "devdeps/_version.py"
 
 [tool.black]
 extend-exclude = '''
 (
   _version\.py
   |something-else
 )
 '''
 
 [tool.mypy]
-plugins = ["pydantic.mypy"]
+plugins = [
+  "pydantic.mypy"
+]
 
 follow_imports = "silent"
 warn_redundant_casts = true
 warn_unused_ignores = true
 disallow_any_generics = true
 check_untyped_defs = true
 no_implicit_reexport = true
 
 # for strict mypy: (this is the tricky one :-))
 disallow_untyped_defs = true
 
 [tool.pytest.ini_options]
 minversion = "6.0"
-addopts = "--verbose --doctest-modules --junitxml=junit/test-results.xml --cov=dev_dependencies --cov=tests --cov-report html --cov-report term --cov-fail-under=100 --capture=no"
-testpaths = ["tests"]
+addopts = "--verbose --doctest-modules --junitxml=junit/test-results.xml --cov=devdeps --cov=tests --cov-report html --cov-report term --cov-fail-under=100 --capture=no"
+testpaths = [
+    "tests"
+]
+pythonpath = [
+    "."
+]
 
 
 [tool.coverage.run]
 branch = true
-omit = ["dev_dependencies/_version.py"]
-
-[tool.poetry]
-name = "dev-dependencies"
-version = "0.0.4"
-description = "An opinionated library of dev-time dependencies"
-authors = ["Justin Mills <vortexjj@gmail.com>"]
-license = "MIT"
-readme = "README.md"
-packages = [{ include = "dev_dependencies" }]
-
-[tool.poetry.dependencies]
-python = "^3.11"
-# Types
-pydantic = "*"
-# Backup version parsing
-toml = "*"
-types-toml = "*"
-# Linting
-ruff = "*"
-# Formatting
-black = "*"
-# Typechecking
-mypy = "*"
-# Testing
-pytest = "*"
-pytest-mock = "*"
-hypothesis = "*"
-pytest-cov = "*"
-pytest-xdist = "*"
-pytest-md = "*"
-pytest-emoji = "*"
+omit = [ "devdeps/_version.py" ]
```


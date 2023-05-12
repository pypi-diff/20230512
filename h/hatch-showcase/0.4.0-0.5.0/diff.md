# Comparing `tmp/hatch_showcase-0.4.0.tar.gz` & `tmp/hatch_showcase-0.5.0.tar.gz`

## Comparing `hatch_showcase-0.4.0.tar` & `hatch_showcase-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,17 @@
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 hatch_showcase-0.4.0/.flake8
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_showcase-0.4.0/.gitattributes
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 hatch_showcase-0.4.0/.gitignore
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 hatch_showcase-0.4.0/HISTORY.md
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 hatch_showcase-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 hatch_showcase-0.4.0/README.md
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 hatch_showcase-0.4.0/hatch.toml
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 hatch_showcase-0.4.0/mypy.ini
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 hatch_showcase-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 hatch_showcase-0.4.0/src/hatch_showcase/__init__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 hatch_showcase-0.4.0/src/hatch_showcase/__main__.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 hatch_showcase-0.4.0/src/hatch_showcase/_version.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 hatch_showcase-0.4.0/src/hatch_showcase/fib.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 hatch_showcase-0.4.0/src/hatch_showcase/cli/__init__.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 hatch_showcase-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 hatch_showcase-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 hatch_showcase-0.4.0/tests/test_cli.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hatch_showcase-0.4.0/tests/test_fib.py
--rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 hatch_showcase-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 hatch_showcase-0.5.0/.gitattributes
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 hatch_showcase-0.5.0/HISTORY.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 hatch_showcase-0.5.0/src/hatch_showcase/__init__.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 hatch_showcase-0.5.0/src/hatch_showcase/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hatch_showcase-0.5.0/src/hatch_showcase/_version.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 hatch_showcase-0.5.0/src/hatch_showcase/fib.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 hatch_showcase-0.5.0/src/hatch_showcase/cli/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 hatch_showcase-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 hatch_showcase-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 hatch_showcase-0.5.0/tests/test_cli.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 hatch_showcase-0.5.0/tests/test_fib.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 hatch_showcase-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 hatch_showcase-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 hatch_showcase-0.5.0/README.md
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 hatch_showcase-0.5.0/hatch.toml
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 hatch_showcase-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 hatch_showcase-0.5.0/PKG-INFO
```

### Comparing `hatch_showcase-0.4.0/HISTORY.md` & `hatch_showcase-0.5.0/HISTORY.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
 
+## 0.5.0 - 2023-05-12
+
+***Added:***
+
+- Build standalone distributions
+
 ## 0.4.0 - 2022-02-13
 
 ***Added:***
 
 - Bump the version of `hatch-mypyc`
 
 ## 0.3.0 - 2022-01-19
```

### Comparing `hatch_showcase-0.4.0/LICENSE.txt` & `hatch_showcase-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_showcase-0.4.0/README.md` & `hatch_showcase-0.5.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # hatch-showcase
 
 | | |
 | --- | --- |
 | CI/CD | [![CI - Test](https://github.com/ofek/hatch-showcase/actions/workflows/test.yml/badge.svg)](https://github.com/ofek/hatch-showcase/actions/workflows/test.yml) [![CD - Build](https://github.com/ofek/hatch-showcase/actions/workflows/build.yml/badge.svg)](https://github.com/ofek/hatch-showcase/actions/workflows/build.yml) |
 | Package | [![PyPI - Version](https://img.shields.io/pypi/v/hatch-showcase.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/hatch-showcase/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hatch-showcase.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/hatch-showcase/) |
-| Meta | [![code style - black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/ambv/black) [![imports - isort](https://img.shields.io/badge/imports-isort-ef8336.svg)](https://github.com/pycqa/isort) [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/) [![GitHub Sponsors](https://img.shields.io/github/sponsors/ofek?logo=GitHub%20Sponsors&style=social)](https://github.com/sponsors/ofek) |
+| Meta | [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![code style - black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/ambv/black) [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/) [![GitHub Sponsors](https://img.shields.io/github/sponsors/ofek?logo=GitHub%20Sponsors&style=social)](https://github.com/sponsors/ofek) |
 
 -----
 
-This project is meant to showcase various features and plugins for [Hatch](https://github.com/ofek/hatch) as well as providing a place to test experimental functionality.
+This project is meant to showcase various features and plugins for [Hatch](https://github.com/pypa/hatch) as well as providing a place to test experimental functionality.
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [Version source](#version-source)
 - [Environments](#environments)
 - [Build](#build)
@@ -26,19 +26,21 @@
 
 ## Version source
 
 - The [hatch-vcs](https://github.com/ofek/hatch-vcs) version source plugin determines the project version using Git tags
 
 ## Environments
 
-- Defined neatly in a standalone [`hatch.toml`](https://ofek.dev/hatch/latest/intro/#configuration)
+- Defined neatly in a standalone [`hatch.toml`](https://hatch.pypa.io/latest/intro/#configuration)
 - The `test` matrix uses the [hatch-containers](https://github.com/ofek/hatch-containers) plugin to run each environment inside Docker containers; usage can be seen in the [test](.github/workflows/test.yml) GitHub workflow
 
 ## Build
 
 - All build targets use the [hatch-vcs](https://github.com/ofek/hatch-vcs) build hook plugin to ship a `_version.py` file so the version can be used at runtime
 - Wheels use the [hatch-mypyc](https://github.com/ofek/hatch-mypyc) build hook plugin to first compile all code with [Mypyc](https://github.com/mypyc/mypyc)
-- The [build](.github/workflows/build.yml) GitHub workflow shows how to use [cibuildwheel](https://github.com/pypa/cibuildwheel) to distribute binary wheels for every platform
+- The [build](.github/workflows/build.yml) GitHub workflow shows how to:
+  - use [cibuildwheel](https://github.com/pypa/cibuildwheel) to distribute binary wheels for every platform
+  - use the [app](https://hatch.pypa.io/latest/plugins/builder/app/) build target to build standalone distributions for every platform
 
 ## License
 
 `hatch-showcase` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `hatch_showcase-0.4.0/src/hatch_showcase/cli/__init__.py` & `hatch_showcase-0.5.0/src/hatch_showcase/cli/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 @click.version_option(version=version, prog_name='hatch-showcase')
 @click.group()
 def hatch_showcase():
     pass
 
 
 @click.argument('n', type=int)
-@hatch_showcase.command()  # type: ignore
+@hatch_showcase.command()
 def fib(n: int):
     click.echo(fibonacci(n))
```

### Comparing `hatch_showcase-0.4.0/tests/conftest.py` & `hatch_showcase-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hatch_showcase-0.4.0/PKG-INFO` & `hatch_showcase-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 Metadata-Version: 2.1
 Name: hatch-showcase
-Version: 0.4.0
+Version: 0.5.0
 Summary: A project showcasing features and plugins for Hatch
 Project-URL: Donate, https://github.com/sponsors/ofek
 Project-URL: History, https://github.com/ofek/hatch-showcase/blob/master/HISTORY.md
 Project-URL: Issues, https://github.com/ofek/hatch-showcase/issues
 Project-URL: Source, https://github.com/ofek/hatch-showcase
 Author-email: Ofek Lev <oss@ofek.dev>
+License: MIT
+License-File: LICENSE.txt
 Keywords: hatch
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: click>=8.0.3
 Description-Content-Type: text/markdown
 
 # hatch-showcase
 
 | | |
 | --- | --- |
 | CI/CD | [![CI - Test](https://github.com/ofek/hatch-showcase/actions/workflows/test.yml/badge.svg)](https://github.com/ofek/hatch-showcase/actions/workflows/test.yml) [![CD - Build](https://github.com/ofek/hatch-showcase/actions/workflows/build.yml/badge.svg)](https://github.com/ofek/hatch-showcase/actions/workflows/build.yml) |
 | Package | [![PyPI - Version](https://img.shields.io/pypi/v/hatch-showcase.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/hatch-showcase/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hatch-showcase.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/hatch-showcase/) |
-| Meta | [![code style - black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/ambv/black) [![imports - isort](https://img.shields.io/badge/imports-isort-ef8336.svg)](https://github.com/pycqa/isort) [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/) [![GitHub Sponsors](https://img.shields.io/github/sponsors/ofek?logo=GitHub%20Sponsors&style=social)](https://github.com/sponsors/ofek) |
+| Meta | [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![code style - black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/ambv/black) [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/) [![GitHub Sponsors](https://img.shields.io/github/sponsors/ofek?logo=GitHub%20Sponsors&style=social)](https://github.com/sponsors/ofek) |
 
 -----
 
-This project is meant to showcase various features and plugins for [Hatch](https://github.com/ofek/hatch) as well as providing a place to test experimental functionality.
+This project is meant to showcase various features and plugins for [Hatch](https://github.com/pypa/hatch) as well as providing a place to test experimental functionality.
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [Version source](#version-source)
 - [Environments](#environments)
 - [Build](#build)
@@ -49,19 +52,21 @@
 
 ## Version source
 
 - The [hatch-vcs](https://github.com/ofek/hatch-vcs) version source plugin determines the project version using Git tags
 
 ## Environments
 
-- Defined neatly in a standalone [`hatch.toml`](https://ofek.dev/hatch/latest/intro/#configuration)
+- Defined neatly in a standalone [`hatch.toml`](https://hatch.pypa.io/latest/intro/#configuration)
 - The `test` matrix uses the [hatch-containers](https://github.com/ofek/hatch-containers) plugin to run each environment inside Docker containers; usage can be seen in the [test](.github/workflows/test.yml) GitHub workflow
 
 ## Build
 
 - All build targets use the [hatch-vcs](https://github.com/ofek/hatch-vcs) build hook plugin to ship a `_version.py` file so the version can be used at runtime
 - Wheels use the [hatch-mypyc](https://github.com/ofek/hatch-mypyc) build hook plugin to first compile all code with [Mypyc](https://github.com/mypyc/mypyc)
-- The [build](.github/workflows/build.yml) GitHub workflow shows how to use [cibuildwheel](https://github.com/pypa/cibuildwheel) to distribute binary wheels for every platform
+- The [build](.github/workflows/build.yml) GitHub workflow shows how to:
+  - use [cibuildwheel](https://github.com/pypa/cibuildwheel) to distribute binary wheels for every platform
+  - use the [app](https://hatch.pypa.io/latest/plugins/builder/app/) build target to build standalone distributions for every platform
 
 ## License
 
 `hatch-showcase` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```


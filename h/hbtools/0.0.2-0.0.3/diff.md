# Comparing `tmp/hbtools-0.0.2.tar.gz` & `tmp/hbtools-0.0.3.tar.gz`

## Comparing `hbtools-0.0.2.tar` & `hbtools-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 hbtools-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 hbtools-0.0.2/requirements/README.md
--rw-r--r--   0        0        0    18614 2020-02-02 00:00:00.000000 hbtools-0.0.2/requirements/requirements-build.txt
--rw-r--r--   0        0        0    24980 2020-02-02 00:00:00.000000 hbtools-0.0.2/requirements/requirements-dev.txt
--rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 hbtools-0.0.2/requirements/requirements-flake8.txt
--rw-r--r--   0        0        0    16499 2020-02-02 00:00:00.000000 hbtools-0.0.2/requirements/requirements-terminal.txt
--rw-r--r--   0        0        0     4171 2020-02-02 00:00:00.000000 hbtools-0.0.2/requirements/requirements-test.txt
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 hbtools-0.0.2/requirements/requirements.txt
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hbtools-0.0.2/src/hbtools/__init__.py
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 hbtools-0.0.2/src/hbtools/logger.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 hbtools-0.0.2/src/hbtools/misc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hbtools-0.0.2/src/hbtools/py.typed
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 hbtools-0.0.2/src/hbtools/show_img.py
--rwxr-xr-x   0        0        0      101 2020-02-02 00:00:00.000000 hbtools-0.0.2/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hbtools-0.0.2/LICENSE
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 hbtools-0.0.2/README.md
--rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 hbtools-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 hbtools-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 hbtools-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 hbtools-0.0.3/noxfile.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 hbtools-0.0.3/requirements/README.md
+-rw-r--r--   0        0        0    18614 2020-02-02 00:00:00.000000 hbtools-0.0.3/requirements/requirements-build.txt
+-rw-r--r--   0        0        0    24980 2020-02-02 00:00:00.000000 hbtools-0.0.3/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 hbtools-0.0.3/requirements/requirements-flake8.txt
+-rw-r--r--   0        0        0    16499 2020-02-02 00:00:00.000000 hbtools-0.0.3/requirements/requirements-terminal.txt
+-rw-r--r--   0        0        0     5643 2020-02-02 00:00:00.000000 hbtools-0.0.3/requirements/requirements-test.txt
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 hbtools-0.0.3/requirements/requirements.txt
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hbtools-0.0.3/src/hbtools/__init__.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 hbtools-0.0.3/src/hbtools/logger.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 hbtools-0.0.3/src/hbtools/misc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hbtools-0.0.3/src/hbtools/py.typed
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 hbtools-0.0.3/src/hbtools/show_img.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 hbtools-0.0.3/tests/test_call_fn.py
+-rwxr-xr-x   0        0        0      101 2020-02-02 00:00:00.000000 hbtools-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hbtools-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 hbtools-0.0.3/README.md
+-rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 hbtools-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 hbtools-0.0.3/PKG-INFO
```

### Comparing `hbtools-0.0.2/.pre-commit-config.yaml` & `hbtools-0.0.3/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,16 @@
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
 
   - repo: https://github.com/RobertCraigie/pyright-python
     rev: v1.1.300
     hooks:
     - id: pyright
-      additional_dependencies: ["opencv-python>=4.7", "opencv-stubs", "numpy>=1.21", "term_image"]
+      # FIXME: Using "hbtools" here is not ideal, stop using pre-commit for pyright and set it up as a separate GA.
+      additional_dependencies: ["opencv-python>=4.7", "opencv-stubs", "numpy>=1.21", "term_image", "pytest", "nox", "hbtools"]
 
   - repo: https://github.com/PyCQA/flake8
     rev: 5.0.4
     hooks:
       - id: flake8
         additional_dependencies:
           - flake8-bugbear
```

### Comparing `hbtools-0.0.2/requirements/README.md` & `hbtools-0.0.3/requirements/README.md`

 * *Files identical despite different names*

### Comparing `hbtools-0.0.2/requirements/requirements-build.txt` & `hbtools-0.0.3/requirements/requirements-build.txt`

 * *Files identical despite different names*

### Comparing `hbtools-0.0.2/requirements/requirements-dev.txt` & `hbtools-0.0.3/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `hbtools-0.0.2/requirements/requirements-flake8.txt` & `hbtools-0.0.3/requirements/requirements-flake8.txt`

 * *Files identical despite different names*

### Comparing `hbtools-0.0.2/requirements/requirements-terminal.txt` & `hbtools-0.0.3/requirements/requirements-terminal.txt`

 * *Files identical despite different names*

### Comparing `hbtools-0.0.2/requirements/requirements-test.txt` & `hbtools-0.0.3/requirements/requirements.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --extra=test --generate-hashes --output-file=requirements/requirements-test.txt --resolver=backtracking pyproject.toml
+#    pip-compile --generate-hashes --output-file=requirements/requirements.txt --resolver=backtracking pyproject.toml
 #
-iniconfig==2.0.0 \
-    --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
-    --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
-    # via pytest
 numpy==1.24.3 \
     --hash=sha256:0ec87a7084caa559c36e0a2309e4ecb1baa03b687201d0a847c8b0ed476a7187 \
     --hash=sha256:1a7d6acc2e7524c9955e5c903160aa4ea083736fde7e91276b0e5d98e6332812 \
     --hash=sha256:202de8f38fc4a45a3eea4b63e2f376e5f2dc64ef0fa692838e31a808520efaf7 \
     --hash=sha256:210461d87fb02a84ef243cac5e814aad2b7f4be953b32cb53327bb49fd77fbb4 \
     --hash=sha256:2d926b52ba1367f9acb76b0df6ed21f0b16a1ad87c6720a1121674e5cf63e2b6 \
     --hash=sha256:352ee00c7f8387b44d19f4cada524586f07379c0d49270f87233983bc5087ca0 \
@@ -45,19 +41,7 @@
     --hash=sha256:7a297e7651e22eb17c265ddbbc80e2ba2a8ff4f4a1696a67c45e5f5798245842 \
     --hash=sha256:812af57553ec1c6709060c63f6b7e9ad07ddc0f592f3ccc6d00c71e0fe0e6376 \
     --hash=sha256:cd08343654c6b88c5a8c25bf425f8025aed2e3189b4d7306b5861d32affaf737 \
     --hash=sha256:d4f8880440c433a0025d78804dda6901d1e8e541a561dda66892d90290aef881 \
     --hash=sha256:ebfc0a3a2f57716e709028b992e4de7fd8752105d7a768531c4f434043c6f9ff \
     --hash=sha256:eda115797b114fc16ca6f182b91c5d984f0015c19bec3145e55d33d708e9bae1
     # via hbtools (pyproject.toml)
-packaging==23.1 \
-    --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
-    --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
-    # via pytest
-pluggy==1.0.0 \
-    --hash=sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159 \
-    --hash=sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3
-    # via pytest
-pytest==7.3.1 \
-    --hash=sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362 \
-    --hash=sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3
-    # via hbtools (pyproject.toml)
```

### Comparing `hbtools-0.0.2/src/hbtools/logger.py` & `hbtools-0.0.3/src/hbtools/logger.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 """Module providing an easy way to setup a minimal logger."""
 import logging
 import os
+import platform
 import sys
-from enum import StrEnum
 from logging import handlers, StreamHandler
 from pathlib import Path
-from typing import Literal, Self
+from typing import Literal
 
+if int(platform.python_version_tuple()[1]) >= 11:
+    from enum import StrEnum
+    from typing import Self
+else:
+    from enum import Enum
 
-class ConsoleColor(StrEnum):
+    from typing_extensions import Self
+    StrEnum = (str, Enum)
+
+
+class ConsoleColor(*StrEnum):
     """Simple shortcut to use colors in the console."""
 
     HEADER = "\033[95m"
     BLUE = "\033[94m"
     GREEN = "\033[92m"
     ORANGE = "\033[93m"
     RED = "\033[91m"
@@ -54,15 +63,16 @@
         stdout: If True then outputs to stdout.
         verbose_level: Either debug, info, error.
 
     Returns:
         The logger instance.
     """
     if log_dir is None and not stdout:
-        raise ValueError(f"Either `log_dir` must be a Path or stdout must be `True`, got {log_dir=} and {stdout=}.")
+        msg = f"Either `log_dir` must be a Path or stdout must be `True`, got {log_dir=} and {stdout=}."
+        raise ValueError(msg)
 
     logger = logging.getLogger(name)
 
     if log_dir is not None:
         log_dir.mkdir(parents=True, exist_ok=True)
         log_formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
         # Add a (rotating) file handler to the logging system
```

### Comparing `hbtools-0.0.2/src/hbtools/misc.py` & `hbtools-0.0.3/src/hbtools/misc.py`

 * *Files identical despite different names*

### Comparing `hbtools-0.0.2/src/hbtools/show_img.py` & `hbtools-0.0.3/src/hbtools/show_img.py`

 * *Files identical despite different names*

### Comparing `hbtools-0.0.2/LICENSE` & `hbtools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hbtools-0.0.2/README.md` & `hbtools-0.0.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # hbtools
 
 [![PyPI](https://img.shields.io/pypi/v/hbtools?color=green&style=flat)](https://pypi.org/project/hbtools)
-[![PyPI - Implementation](https://img.shields.io/pypi/implementation/hbtools?style=flat)](https://pypi.org/project/hbtools)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hbtools?style=flat)](https://pypi.org/project/hbtools)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/hbtools?style=flat-square)](https://pypistats.org/packages/hbtools)
 [![License](https://img.shields.io/pypi/l/hbtools?style=flat)](https://opensource.org/licenses/MIT)
 ![Linting](https://github.com/hoel-bagard/hbtools/actions/workflows/pre-commit.yaml/badge.svg)
+![Tests](https://github.com/hoel-bagard/coco-types/actions/workflows/nox.yaml/badge.svg)
 
 Package containing a few python utils functions.
 
 ## Installation
 
 The package is available on pypi [here](https://pypi.org/project/hbtools/) you can install it with:
```

### Comparing `hbtools-0.0.2/pyproject.toml` & `hbtools-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -6,34 +6,33 @@
 name = "hbtools"
 authors = [{name="Bagard Hoel"}]
 description = "Package containing a few python utils functions."
 readme = "README.md"
 classifiers = [
             "License :: OSI Approved :: MIT License",
             "Programming Language :: Python :: 3",
-            "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
             "Programming Language :: Python :: 3.11",
             "Operating System :: OS Independent",
             "Intended Audience :: Developers",
 ]
 license = {text = "MIT"}
 dynamic = ["version"]
-dependencies = ["opencv-python>=4.7", "numpy>=1.21"]
-requires-python = ">=3.11"
+dependencies = ["opencv-python>=4.7", "numpy>=1.21", "typing_extensions; python_version < '3.11'"]
+requires-python = ">=3.10"
 
 [project.urls]
 "Homepage" = "https://github.com/hoel-bagard/hbtools"
 "Bug Tracker" = "https://github.com/hoel-bagard/hbtools/issues"
 
 [project.optional-dependencies]
 terminal = ["Pillow", "term_image"]
 dev = ["pre-commit", "pip-tools", "ruff", "pyright", "opencv-stubs", "term_image"]
 build = ["hatch"]
-test = ["pytest"]
+test = ["pytest", "nox"]
 flake8 = ["flake8", "flake8-bugbear", "flake8-comprehensions", "flake8-docstrings", "flake8-builtins", "flake8-quotes", "pep8-naming", "flake8-import-order", "flake8-noqa", "flake8-broken-line", "flake8-commas", "Flake8-pyproject"]
 
 [tool.hatch.version]
 path = "src/hbtools/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
@@ -52,21 +51,32 @@
 publish_test = "hatch build --clean && hatch publish -r test"
 publish = "hatch build --clean && hatch publish"
 
 [tool.pytest.ini_options]
 addopts = ["--import-mode=importlib",]
 
 [tool.ruff]
-select = ["A", "B", "D", "C4", "E", "FBT", "I", "Q", "UP", "ANN", "S", "BLE", "COM", "DTZ", "PIE", "PT", "RSE", "SIM","PTH", "NPY", "RUF"]
-# D407: Missing dashed underline after section ("Args", "Returns")
+select = ["ALL"]
+# D1: Do not require docstrings
 # D203: one-blank-line-before-class  (incompatible)
 # D213: multi-line-summary-second-line  (incompatible)
-ignore = ["D203", "D213", "D407"]
+# D407: Missing dashed underline after section ("Args", "Returns")
+# ERA001: Found commented-out code
+# PLR2004: Magic value used in comparison, consider replacing X with a constant variable
+# T201: `print` found
+ignore = ["D1", "D203", "D213", "D407", "ERA001", "PLR2004", "T201", "TRY"]
 line-length = 120
 
+[tool.ruff.per-file-ignores]
+"noxfile.py" = ["ANN001"]
+# FBT001: Boolean positional arg in function definition
+# INP001 File `X` is part of an implicit namespace package. Add an `__init__.py`.
+# S101: Use of `assert` detected
+"tests/*.py" = ["FBT001", "INP001", "S101"]
+
 [tool.ruff.isort]
 order-by-type = false
 
 [tool.ruff.flake8-quotes]
 docstring-quotes = "double"
 
 [tool.pyright]
@@ -102,12 +112,22 @@
 reportImplicitStringConcatenation = false
 reportUnusedCallResult = false
 reportUnusedExpression = "warning"
 reportUnnecessaryTypeIgnoreComment = "warning"
 reportMatchNotExhaustive = "warning"
 
 [tool.flake8]
-exclude = ["env", "venv"]
 max-line-length = 120
 docstring-convention = "google"
 import-order-style = "smarkets"
 inline-quotes = "double"
+exclude = ["env", "venv", ".nox"]
+# D1: Do not require docstrings
+# NQA102 "# noqa: X" has no matching violations
+ignore = ["D1", "NQA102"]
+
+[tool.pylint.messages_control]
+max-line-length = 120
+disable = [
+    "no-member",
+    "import-outside-toplevel",
+]
```

### Comparing `hbtools-0.0.2/PKG-INFO` & `hbtools-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: hbtools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package containing a few python utils functions.
 Project-URL: Homepage, https://github.com/hoel-bagard/hbtools
 Project-URL: Bug Tracker, https://github.com/hoel-bagard/hbtools/issues
 Author: Bagard Hoel
 License: MIT
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Requires-Dist: numpy>=1.21
 Requires-Dist: opencv-python>=4.7
+Requires-Dist: typing-extensions; python_version < '3.11'
 Provides-Extra: build
 Requires-Dist: hatch; extra == 'build'
 Provides-Extra: dev
 Requires-Dist: opencv-stubs; extra == 'dev'
 Requires-Dist: pip-tools; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pyright; extra == 'dev'
@@ -39,25 +39,26 @@
 Requires-Dist: flake8-pyproject; extra == 'flake8'
 Requires-Dist: flake8-quotes; extra == 'flake8'
 Requires-Dist: pep8-naming; extra == 'flake8'
 Provides-Extra: terminal
 Requires-Dist: pillow; extra == 'terminal'
 Requires-Dist: term-image; extra == 'terminal'
 Provides-Extra: test
+Requires-Dist: nox; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
 # hbtools
 
 [![PyPI](https://img.shields.io/pypi/v/hbtools?color=green&style=flat)](https://pypi.org/project/hbtools)
-[![PyPI - Implementation](https://img.shields.io/pypi/implementation/hbtools?style=flat)](https://pypi.org/project/hbtools)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hbtools?style=flat)](https://pypi.org/project/hbtools)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/hbtools?style=flat-square)](https://pypistats.org/packages/hbtools)
 [![License](https://img.shields.io/pypi/l/hbtools?style=flat)](https://opensource.org/licenses/MIT)
 ![Linting](https://github.com/hoel-bagard/hbtools/actions/workflows/pre-commit.yaml/badge.svg)
+![Tests](https://github.com/hoel-bagard/coco-types/actions/workflows/nox.yaml/badge.svg)
 
 Package containing a few python utils functions.
 
 ## Installation
 
 The package is available on pypi [here](https://pypi.org/project/hbtools/) you can install it with:
```


# Comparing `tmp/ctitools-0.4.0.tar.gz` & `tmp/ctitools-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctitools-0.4.0.tar", max compression
+gzip compressed data, was "ctitools-0.4.2.tar", max compression
```

## Comparing `ctitools-0.4.0.tar` & `ctitools-0.4.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1524 2022-07-16 09:18:40.161474 ctitools-0.4.0/LICENSE
--rw-r--r--   0        0        0      899 2022-08-09 11:58:58.277412 ctitools-0.4.0/README.rst
--rw-r--r--   0        0        0      577 2022-07-16 20:31:33.760948 ctitools-0.4.0/berhoel/__init__.py
--rw-r--r--   0        0        0     8379 2022-12-02 19:55:13.119268 ctitools-0.4.0/berhoel/ctitools/__init__.py
--rw-r--r--   0        0        0      569 2022-07-30 19:39:33.591163 ctitools-0.4.0/berhoel/ctitools/__main__.py
--rw-r--r--   0        0        0     5683 2022-12-15 18:21:28.260507 ctitools-0.4.0/berhoel/ctitools/ct.py
--rw-r--r--   0        0        0     3498 2022-12-15 19:51:37.432703 ctitools-0.4.0/berhoel/ctitools/cti2bibtex/__init__.py
--rw-r--r--   0        0        0      571 2022-07-30 19:36:58.727250 ctitools-0.4.0/berhoel/ctitools/cti2bibtex/__main__.py
--rw-r--r--   0        0        0     1959 2022-10-20 19:16:43.373498 ctitools-0.4.0/berhoel/ctitools/cti2bibtex/tests/test_base.py
--rw-r--r--   0        0        0     2685 2022-12-15 19:17:59.996999 ctitools-0.4.0/berhoel/ctitools/cti2bibtex/tests/test_generate.py
--rw-r--r--   0        0        0     1260 2022-09-08 09:57:16.786064 ctitools-0.4.0/berhoel/ctitools/ctientry.py
--rw-r--r--   0        0        0     2772 2022-08-01 15:08:30.320285 ctitools-0.4.0/berhoel/ctitools/ix.py
--rw-r--r--   0        0        0     1278 2022-08-28 14:26:03.997542 ctitools-0.4.0/berhoel/ctitools/tests/test_ct.py
--rw-r--r--   0        0        0     1171 2022-08-01 14:00:56.594637 ctitools-0.4.0/berhoel/ctitools/tests/test_ctitools.py
--rw-r--r--   0        0        0     5561 2022-09-08 10:05:11.577264 ctitools-0.4.0/berhoel/ctitools/tests/test_processing.py
--rw-r--r--   0        0        0     2734 2022-12-15 20:19:31.888365 ctitools-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1962 1970-01-01 00:00:00.000000 ctitools-0.4.0/setup.py
--rw-r--r--   0        0        0     2017 1970-01-01 00:00:00.000000 ctitools-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1524 2022-07-16 09:18:40.161474 ctitools-0.4.2/LICENSE
+-rw-r--r--   0        0        0      899 2022-08-09 11:58:58.277412 ctitools-0.4.2/README.rst
+-rw-r--r--   0        0        0      577 2022-07-16 20:31:33.760948 ctitools-0.4.2/berhoel/__init__.py
+-rw-r--r--   0        0        0     8379 2022-12-02 19:55:13.119268 ctitools-0.4.2/berhoel/ctitools/__init__.py
+-rw-r--r--   0        0        0      569 2022-07-30 19:39:33.591163 ctitools-0.4.2/berhoel/ctitools/__main__.py
+-rw-r--r--   0        0        0     5926 2023-05-12 18:47:25.437032 ctitools-0.4.2/berhoel/ctitools/ct.py
+-rw-r--r--   0        0        0     3498 2022-12-15 19:51:37.432703 ctitools-0.4.2/berhoel/ctitools/cti2bibtex/__init__.py
+-rw-r--r--   0        0        0      571 2022-07-30 19:36:58.727250 ctitools-0.4.2/berhoel/ctitools/cti2bibtex/__main__.py
+-rw-r--r--   0        0        0     1959 2022-10-20 19:16:43.373498 ctitools-0.4.2/berhoel/ctitools/cti2bibtex/tests/test_base.py
+-rw-r--r--   0        0        0     2685 2022-12-15 19:17:59.996999 ctitools-0.4.2/berhoel/ctitools/cti2bibtex/tests/test_generate.py
+-rw-r--r--   0        0        0     1260 2022-09-08 09:57:16.786064 ctitools-0.4.2/berhoel/ctitools/ctientry.py
+-rw-r--r--   0        0        0     2772 2022-08-01 15:08:30.320285 ctitools-0.4.2/berhoel/ctitools/ix.py
+-rw-r--r--   0        0        0     1502 2023-05-12 18:48:31.253040 ctitools-0.4.2/berhoel/ctitools/tests/test_ct.py
+-rw-r--r--   0        0        0     1171 2022-08-01 14:00:56.594637 ctitools-0.4.2/berhoel/ctitools/tests/test_ctitools.py
+-rw-r--r--   0        0        0     5561 2022-09-08 10:05:11.577264 ctitools-0.4.2/berhoel/ctitools/tests/test_processing.py
+-rw-r--r--   0        0        0     3569 2023-05-12 18:56:05.717101 ctitools-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2017 1970-01-01 00:00:00.000000 ctitools-0.4.2/PKG-INFO
```

### Comparing `ctitools-0.4.0/LICENSE` & `ctitools-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.0/README.rst` & `ctitools-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.0/berhoel/__init__.py` & `ctitools-0.4.2/berhoel/__init__.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.0/berhoel/ctitools/__init__.py` & `ctitools-0.4.2/berhoel/ctitools/__init__.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.0/berhoel/ctitools/__main__.py` & `ctitools-0.4.2/berhoel/ctitools/__main__.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.0/berhoel/ctitools/ct.py` & `ctitools-0.4.2/berhoel/ctitools/ct.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Standard library imports.
 from datetime import datetime, timedelta
 
 # Local library imports.
 from .ctientry import CTIEntry
 
-__date__ = "2022/12/15 19:21:27 hoel"
+__date__ = "2023/05/12 20:47:25 hoel"
 __author__ = "Berthold Höllmann"
 __copyright__ = "Copyright © 2022 by Berthold Höllmann"
 __credits__ = ["Berthold Höllmann"]
 __maintainer__ = "Berthold Höllmann"
 __email__ = "berhoel@gmail.com"
 
 
@@ -39,19 +39,24 @@
         key = (year, issue)
         diff = timedelta(days=14)
         if self._cache.get(key) is not None:
             return self._cache[key]
         while key > self._issue_max:
             step_year, step_issue = self._issue_max
             step_issue += 1
-            if step_issue > 27:
+            if step_issue >= 27:
                 step_issue = 1
                 step_year += 1
             self._issue_max = (step_year, step_issue)
-            self._date_max += diff
+            if (step_year, step_issue) == (2023, 12):
+                self._date_max = datetime(2023, 5, 13)
+            elif (step_year, step_issue) == (2023, 13):
+                self._date_max = datetime(2023, 5, 20)
+            else:
+                self._date_max += diff
             self._cache[self._issue_max] = self._date_max
             assert self._date_max < datetime.now() + timedelta(
                 days=16
             ), f"{self._date_max=} < {datetime.now() + timedelta(days=14)=}, {key=}"
         while key < self._issue_min:
             if self._date_min <= datetime(1997, 10, 13):
                 step_issue -= 1
```

### Comparing `ctitools-0.4.0/berhoel/ctitools/cti2bibtex/__init__.py` & `ctitools-0.4.2/berhoel/ctitools/cti2bibtex/__init__.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.0/berhoel/ctitools/cti2bibtex/__main__.py` & `ctitools-0.4.2/berhoel/ctitools/cti2bibtex/__main__.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.0/berhoel/ctitools/cti2bibtex/tests/test_base.py` & `ctitools-0.4.2/berhoel/ctitools/cti2bibtex/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.0/berhoel/ctitools/cti2bibtex/tests/test_generate.py` & `ctitools-0.4.2/berhoel/ctitools/cti2bibtex/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.0/berhoel/ctitools/ctientry.py` & `ctitools-0.4.2/berhoel/ctitools/ctientry.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.0/berhoel/ctitools/ix.py` & `ctitools-0.4.2/berhoel/ctitools/ix.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.0/berhoel/ctitools/tests/test_ctitools.py` & `ctitools-0.4.2/berhoel/ctitools/tests/test_ctitools.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.0/berhoel/ctitools/tests/test_processing.py` & `ctitools-0.4.2/berhoel/ctitools/tests/test_processing.py`

 * *Files identical despite different names*

### Comparing `ctitools-0.4.0/pyproject.toml` & `ctitools-0.4.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ctitools"
-version = "0.4.0"
+version = "0.4.2"
 description = "Work with cti index files for the Heise papers c't and iX"
 packages = [{ include = "berhoel" }]
 exclude = ["**/.#*.py", "**/#*.py#"]
 authors = ["Berthold Höllmann <berthold@xn--hllmanns-n4a.de>"]
 license = "BSD 3"
 repository = "https://gitlab.com/berhoel/python/ctitools.git"
 homepage = "https://python.xn--hllmanns-n4a.de/ctitools/"
@@ -73,24 +73,58 @@
 import_heading_localfolder = 'Local library imports.'
 default_section = "THIRDPARTY"
 known_first_party = ["berhoel"]
 known_third_party = ["pytest"]
 
 [tool.tox]
 legacy_tox_ini = """
+
 [tox]
 isolated_build = true
-envlist = py37,py38,py39,py310
-#,py311
+skip_missing_interpreters = true
+envlist = py{39, 310, 311}
 
 [testenv]
+
+deps =
+   bhoelHelper
+   black
+   flake8
+   pdbpp
+   pylint
+   pylint-plugin-utils
+   pytest
+   pytest-benchmark
+   pytest-black
+   pytest-cov
+   pytest-flake8
+   pytest-isort
+   pytest-mock
+   pytest-runner
+   pytest-sugar
+   rope
+   toml
+   xdoctest
+
+commands_pre =
+   pip install git+https://gitlab.com/berhoel/python/berhoel-sphinx-settings.git
+   pip install "flake8>=4.0.0,<5.0.0"
+   set_lib_version
+
 whitelist_externals = poetry
+
 commands =
-    poetry install -v
-    poetry run pytest {posargs}
+   pytest                                                    \
+        --doctest-modules                                    \
+        --junitxml=ctitools-report.xml                       \
+        --isort                                              \
+        --cov berhoel/                                       \
+        --cov-report term --cov-report html --cov-report xml \
+        --cov-report annotate --cov-report term-missing      \
+        berhoel/
 """
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--doctest-modules --ff --pdb -s --cov=berhoel --cov-report=term --cov-report=html --cov-branch --isort --black --flake8"
 testpaths = ["berhoel"]
```

### Comparing `ctitools-0.4.0/PKG-INFO` & `ctitools-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctitools
-Version: 0.4.0
+Version: 0.4.2
 Summary: Work with cti index files for the Heise papers c't and iX
 Home-page: https://python.xn--hllmanns-n4a.de/ctitools/
 License: BSD 3
 Author: Berthold Höllmann
 Author-email: berthold@xn--hllmanns-n4a.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 1 - Planning
```


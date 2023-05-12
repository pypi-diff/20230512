# Comparing `tmp/mctk-py-0.0.1.tar.gz` & `tmp/mctk-py-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mctk-py-0.0.1.tar", last modified: Sun Mar 26 21:43:26 2023, max compression
+gzip compressed data, was "mctk-py-0.1.0.tar", last modified: Fri May 12 19:25:49 2023, max compression
```

## Comparing `mctk-py-0.0.1.tar` & `mctk-py-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-03-26 21:43:26.786500 mctk-py-0.0.1/
--rw-rw-rw-   0        0        0      407 2023-03-02 23:40:15.000000 mctk-py-0.0.1/.bumpversion.cfg
--rw-rw-rw-   0        0        0     8013 2023-03-26 20:44:55.000000 mctk-py-0.0.1/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    11558 2023-03-26 20:44:55.000000 mctk-py-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      425 2023-03-04 13:36:15.000000 mctk-py-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2540 2023-03-26 20:44:55.000000 mctk-py-0.0.1/Makefile
--rw-rw-rw-   0        0        0    16466 2023-03-26 21:43:26.785501 mctk-py-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2517 2023-03-26 20:44:55.000000 mctk-py-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-26 21:43:26.772656 mctk-py-0.0.1/mctk/
--rw-rw-rw-   0        0        0      118 2023-03-26 20:44:55.000000 mctk-py-0.0.1/mctk/__init__.py
--rw-rw-rw-   0        0        0       46 2023-03-26 20:44:55.000000 mctk-py-0.0.1/mctk/ctl.py
--rw-rw-rw-   0        0        0     8524 2023-03-26 20:44:55.000000 mctk-py-0.0.1/mctk/models.py
-drwxrwxrwx   0        0        0        0 2023-03-26 21:43:26.774651 mctk-py-0.0.1/mctk/tests/
--rw-rw-rw-   0        0        0    10503 2023-03-26 20:44:55.000000 mctk-py-0.0.1/mctk/tests/test_models.py
-drwxrwxrwx   0        0        0        0 2023-03-26 21:43:26.783505 mctk-py-0.0.1/mctk_py.egg-info/
--rw-rw-rw-   0        0        0    16466 2023-03-26 21:43:26.000000 mctk-py-0.0.1/mctk_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2023-03-26 21:43:26.000000 mctk-py-0.0.1/mctk_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-26 21:43:26.000000 mctk-py-0.0.1/mctk_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      171 2023-03-26 21:43:26.000000 mctk-py-0.0.1/mctk_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-26 21:43:26.000000 mctk-py-0.0.1/mctk_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2216 2023-03-26 21:43:22.000000 mctk-py-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-26 21:43:26.786500 mctk-py-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-03-02 23:40:15.000000 mctk-py-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:25:49.575613 mctk-py-0.1.0/
+-rw-rw-rw-   0        0        0      301 2023-05-12 19:18:05.000000 mctk-py-0.1.0/.bumpversion.cfg
+-rw-rw-rw-   0        0        0     8611 2023-05-12 18:58:08.000000 mctk-py-0.1.0/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    11558 2023-03-26 20:44:55.000000 mctk-py-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      437 2023-05-12 18:58:08.000000 mctk-py-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2536 2023-05-12 18:58:08.000000 mctk-py-0.1.0/Makefile
+-rw-rw-rw-   0        0        0    19450 2023-05-12 19:25:49.574754 mctk-py-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5501 2023-05-12 18:58:08.000000 mctk-py-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 19:25:49.562757 mctk-py-0.1.0/mctk/
+-rw-rw-rw-   0        0        0      401 2023-05-12 19:18:05.000000 mctk-py-0.1.0/mctk/__init__.py
+-rw-rw-rw-   0        0        0    13476 2023-05-12 18:58:08.000000 mctk-py-0.1.0/mctk/checking.py
+-rw-rw-rw-   0        0        0    12714 2023-05-12 18:58:08.000000 mctk-py-0.1.0/mctk/models.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:25:49.565756 mctk-py-0.1.0/mctk/tests/
+-rw-rw-rw-   0        0        0    10327 2023-05-12 18:58:08.000000 mctk-py-0.1.0/mctk/tests/test_checking.py
+-rw-rw-rw-   0        0        0    12318 2023-05-12 18:58:08.000000 mctk-py-0.1.0/mctk/tests/test_models.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:25:49.572757 mctk-py-0.1.0/mctk_py.egg-info/
+-rw-rw-rw-   0        0        0    19450 2023-05-12 19:25:49.000000 mctk-py-0.1.0/mctk_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-05-12 19:25:49.000000 mctk-py-0.1.0/mctk_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 19:25:49.000000 mctk-py-0.1.0/mctk_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      171 2023-05-12 19:25:49.000000 mctk-py-0.1.0/mctk_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-12 19:25:49.000000 mctk-py-0.1.0/mctk_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2216 2023-05-12 19:18:05.000000 mctk-py-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-12 19:25:49.575613 mctk-py-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-03-02 23:40:15.000000 mctk-py-0.1.0/setup.py
```

### Comparing `mctk-py-0.0.1/CONTRIBUTING.md` & `mctk-py-0.1.0/CONTRIBUTING.md`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 ### Submitting a Bug Report
 
 Please follow these steps:
 
 1. **Open a New Issue**: open a new issue on [MCTK Issues](https://github.com/marcusm117/mctk/issues). Please use the **Bug Report** template.
 2. **Label the Issue**: label the issue with the `bug` label.
 3. **Write a Meaningful Title**: write a concise, descriptive title. Try to use the same words you would use searching for an existing bug report. Please do not write titles like "Help!" or "Urgent!".
+4. **Congratulations!**: you have successfully contribued a Bug Report to MCTK. We will take a look at your report as soon as possible! Please feel free to add comments or ask questions in your issue.
 
 ## Suggesting Enhancements
 
 This section guides you through submitting an enhancement suggestion for MCTK, including completely new features and minor improvements to existing functionality. Following these guidelines helps maintainers and the community understand your suggestion and find related suggestions.
 
 ### Before Submitting an Enhancement Suggestion
 
@@ -45,14 +46,15 @@
 ### Submitting an Enhancement Suggestion
 
 Please follow these steps:
 
 1. **Open a New Issue**: open a new issue on [MCTK Issues](https://github.com/marcusm117/mctk/issues). Please use the **Enhancement Suggestion** template.
 2. **Label the Issue**: label the issue with the `enhancement` label.
 3. **Write a Meaningful Title**: write a concise, descriptive title. Try to use the same words you would use searching for an existing enhancement suggestion. Please do not write titles like "Help!" or "Urgent!".
+4. **Congratulations!**: you have successfully contribued an Enhancement Suggestion to MCTK. We will take a look at your suggestion as soon as possible! Please feel free to add comments or ask questions in your issue.
 
 ## Contributing Code
 
 This section guides you through contributing code to MCTK. Following these guidelines helps maintainers and the community understand your contribution and find related contributions.
 
 ### Before Opening a Pull Request
 
@@ -90,27 +92,33 @@
 
 8. **Lint Code**: lint your code and make sure that there are no errors. You can lint your code using the following command:
 
    ```bash
    make lint
    ```
 
-9. **Write Tests**: write tests for your changes. Make sure that all tests pass and the coverage is at least 100%. You can see the coverage using the following command:
+9. **Write Tests**: write tests for your changes. Make sure that all tests pass. You can run all your tests using the following command:
 
    ```bash
-   make coverage
+   make test
    ```
 
-10. **Commit your Changes**: commit your changes to your local repository. It's okay if you have multiple commits for a single pull request, since they will be squashed when merged, but please write meaningful commit messages. Please do not write commit messages like "fix" or "update".
+10. **Increase Coverage**: increase the test coverage for your changes. Make sure the coverage hits 100%. You can check the test coverage using the following command:
+
+    ```bash
+    make coverage
+    ```
+
+11. **Commit your Changes**: commit your changes to your local repository. It's okay if you have multiple commits for a single pull request, since they will be squashed when merged, but please write meaningful commit messages. Please do not write commit messages like "fix" or "update".
 
     ```bash
     git commit -m "[YOUR_COMMIT_MESSAGE]"
     ```
 
-11. **Push your Changes**: push your changes to your fork.
+12. **Push your Changes**: push your changes to your fork.
 
     ```bash
     git push origin MCTK-[YOUR_BRANCH_NUMBER]
     ```
 
 ### Opening a Pull Request
```

### Comparing `mctk-py-0.0.1/LICENSE` & `mctk-py-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mctk-py-0.0.1/Makefile` & `mctk-py-0.1.0/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 #########
 # LINTS #
 #########
 lint:  ## run static analysis with black, flake8, and pylint
 	python -m black --check mctk setup.py
 	python -m flake8 --max-line-length=120 --extend-ignore=E203 mctk setup.py
-	python -m pylint --disable=C0301,C0114,C0115,C0116,R1720 mctk setup.py
+	python -m pylint --disable=C0301,R1720,C0114,C0103,W1114 mctk setup.py
 
 # Alias
 lints: lint
 
 format:  ## run autoformatting with black
 	python -m black mctk/ setup.py
 
@@ -41,21 +41,21 @@
 type: annotate
 
 
 #########
 # TESTS #
 #########
 test: ## clean and run unit tests
-	python -m pytest -v mctk/tests
+	python -m pytest -vv mctk/tests
 
 # Alias
 tests: test
 
 coverage:  ## clean and run unit tests with coverage
-	python -m pytest -v mctk/tests --cov=mctk --cov-branch --cov-fail-under=75 --junitxml=python_junit.xml --cov-report term-missing
+	python -m pytest -v mctk/tests --cov=mctk --cov-branch --cov-fail-under=100 --junitxml=python_junit.xml --cov-report term-missing
 
 # Alias
 cov: coverage
 
 
 ###########
 # VERSION #
@@ -87,18 +87,18 @@
 publish:  # Upload python assets
 	echo "would usually run python -m twine upload dist/* --skip-existing"
 
 
 #########
 # CLEAN #
 #########
-clean-deep: ## clean everything untracked from the repository
+deep-clean: ## clean everything untracked from the repository
 	git clean -fdx
 
-clean-linux: ## clean the repository
+clean: ## clean the repository
 	rm -rf .coverage coverage cover htmlcov logs build dist *.egg-info .pytest_cache
 
 
 ############################################################################################
 
 
 # Thanks to Francoise at marmelab.com for this
```

### Comparing `mctk-py-0.0.1/PKG-INFO` & `mctk-py-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mctk-py
-Version: 0.0.1
+Version: 0.1.0
 Summary: Model Checking Toolkit for Python
 Author-email: marcusm117 <marcusmin117@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -217,51 +217,51 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
 # Model Checking Toolkit (MCTK)
 
-[![Build Status](https://github.com/marcusm117/mctk/workflows/Build%20Status/badge.svg?branch=dev)](https://github.com/marcusm117/mctk/actions?query=workflow%3A%22Build+Status%22) [![codecov](https://codecov.io/gh/marcusm117/mctk/branch/dev/graph/badge.svg)](https://codecov.io/gh/marcusm117/mctk) [![License](https://img.shields.io/badge/License-Apache_2.0-green)](https://github.com/marcusm117/mctk/blob/dev/LICENSE) [![Issues](https://img.shields.io/github/issues/marcusm117/FV_mctk?color=red&label=Issues)](https://github.com/marcusm117/mctk/issues)
+[![PyPI](https://img.shields.io/pypi/v/mctk-py?color=blue&label=PyPI)](https://pypi.org/project/mctk-py/) [![CI](https://github.com/marcusm117/mctk/workflows/CI/badge.svg?branch=dev)](https://github.com/marcusm117/mctk/actions?query=workflow%3A%22Build+Status%22) [![codecov](https://codecov.io/gh/marcusm117/mctk/branch/dev/graph/badge.svg)](https://codecov.io/gh/marcusm117/mctk) [![Docs](https://github.com/marcusm117/mctk/workflows/Docs/badge.svg?branch=dev)](https://marcusm117.github.io/mctk/) [![License](https://img.shields.io/badge/License-Apache_2.0-green)](https://github.com/marcusm117/mctk/blob/dev/LICENSE) [![Issues](https://img.shields.io/github/issues/marcusm117/FV_mctk?color=red&label=Issues)](https://github.com/marcusm117/mctk/issues)
 
-Model Checking Toolkit in Python.
+[Model Checking Toolkit for Python.](https://marcusm117.github.io/mctk/)
 
 ## Overview
 
-`mctk` is a Python library for Explicit-State Model Checking (will also support Symbolic Model Checking and Bounded Model Checking in the future) on Kripke Structures (will also support other Transition Systems) supporting the CTL(Computation Tree Logic) operators: EX, EU, and EG.
+`mctk` is a Python library for Explicit-State Model Checking (will also support Symbolic Model Checking and Bounded Model Checking in the future) on Kripke Structures (will also support other Transition Systems) supporting the CTL(Computation Tree Logic) operators: **EX, EU, EG, EF, AX, AU, AG, AF**, and the Propositional Logic operators: **NOT, AND, OR, IMPLIES, IFF**.
 
-Users can create checker instances to formally verify if a Kripke Structure (can be created during runtime or input in a JSON file) satisfies certain CTL properties. The checker instance will return a set of satisfying states and "SAT" if satisfied or an Error Trace if unsatisfied.
+Users can use functions that implements CTL operators to formally verify if a Kripke Structure (can be created during runtime or input in a JSON file) satisfies certain CTL properties. All checking functions will return a set of states that satisfy the CTL property, which means that if any start state of the Kripke Structure is in the returned set, then the Kripke Structure satisfies the CTL property.
 
 ## Getting Started
 
 ### Installation
 
-Get the latest version of `mctk` from PyPI:
+Get the latest version of `mctk` from PyPI. Note that the registered name is 'mctk-py' on PyPI due to the strict typo-squatting prevention mechanism of the registry. However, when using the library, you should import it as 'mctk'.
 
    ``` bash
-   pip3 install mctk
+   pip3 install mctk-py
    ```
 
 If you are having trouble with `pip3`, you can also install from the source code, see [Developing](#developing).
 
 ### Developing
 
-Clone this Repository to your Local Environment
+Clone this Repository to your Local Environment.
 
    ``` bash
    git clone https://github.com/marcusm117/mctk.git
    ```
 
-Go into the Repository Directory
+Go into the Repository Directory.
 
    ``` bash
    cd mctk
    ```
 
-Install the Library with all Dependencies
+Install the Library with all Dependencies.
 
    ``` bash
    make develop
    ```
 
 ### Linting & Testing
 
@@ -271,23 +271,81 @@
 - `make lint`: perform static analysis of this library with `black`, `flake8` and `pylint`
 - `make annotate`: run type checking using `mypy`
 - `make test`: run automated tests with `pytest`
 - `make coverage`: run automated tests with `pytest` and collect coverage information
 
 ## Usage
 
+Create a Krinke Structure from scratch.
+
 ``` python
-from mctk import KripkeStruct
+from mctk import *
 
+# create a Kripke Structure from scratch
 ks = KripkeStruct()
+
+# set 2 Atomic Propositions in this Kripke Structure
 ks.set_atoms(["p", "q"])
+
+# add 2 states to the Kripke Structure
+# a State Name is represented by a string, it must be unique
+# a State Label is represented by a binary number, it must be unique
+# for example, 0b10 means the state has the Atoms "p" but not "q"
 ks.add_state("s0", 0b10)
 ks.add_state("s1", 0b01)
-ks.set_start(["s0"])
+
+# set the Start States of the Kripke Structure
+# there can be multiple Start States
+ks.set_starts(["s0"])
+
+# add 2 Transitions to the Kripke Structure
+# a Transition is represented by a key-value pair
+# where key the Source State Name and value is a list of Destination State Names
 ks.add_trans({"s0": ["s1"], "s1": ["s0"]})
 ```
 
+Check if the Kripke Structure satisfies a simple CTL formula.
+
+``` python
+# check if the Kripke Structure satisfies the CTL formula: EX p
+# SAT_atom(ks, "p") returns a set of states that satisfy the Atomic Proposition p
+# EX returns a set of states that satisfy the CTL formula EX p
+sat_states = EX(ks, SAT_atom(ks, "p"))
+
+# the result should be {"s1"}
+# since the start state "s0" is not in sat_states, ks doesn't satisfy the CTL formula
+assert sat_states == {"s1"}
+
+# check if the Kripke Structure satisfies the CTL formula: E p U q
+# SAT_atom(ks, "p") returns a set of states that satisfy the Atomic Proposition p
+# SAT_atom(ks, "q") returns a set of states that satisfy the Atomic Proposition q
+# EU returns a set of states that satisfy the CTL formula E p U q
+sat_states = EU(ks, SAT_atom(ks, "p"), SAT_atom(ks, "q"))
+
+# the result should be {"s0", "s1"}
+# since the start state "s0" is in sat_states, ks satisfies the CTL formula
+assert sat_states == {"s0", "s1"}
+```
+
+Check if the Kripke Structure satisfies a composite CTL formula.
+
+``` python
+# check if the Kripke Structure satisfies the CTL formula: EX (p AND EX q)
+sat_states = EX(ks, AND(SAT_atom(ks, "p"), EX(ks, SAT_atom(ks, "q"))))
+
+# the result should be {"s1"}
+# since the start state "s0" is not in sat_states, ks doesn't satisfy the CTL formula
+assert sat_states == {"s1"}
+
+# check if the Kripke Structure satisfies the CTL formula: EG (A p U (NOT q))
+sat_states = EG(ks, AU(ks, SAT_atom(ks, "p"), NOT(ks, SAT_atom(ks, "q"))))
+
+# the result should be set(), empty set
+# since the start state "s0" is not in sat_states, ks doesn't satisfy the CTL formula
+assert sat_states == set()
+```
+
 ## Contributing
 
 All contrbutions are welcome!
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details.
```

### Comparing `mctk-py-0.0.1/mctk/tests/test_models.py` & `mctk-py-0.1.0/mctk/tests/test_models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,85 +1,85 @@
 # Authors: marcusm117
 # License: Apache 2.0
 
-# standard libraries
+# Standard Libraries
 from collections import defaultdict
 
-# external libraries
+# External Libraries
 import pytest
 
-# module to be tested
+# Internal Modules to be tested
 from mctk import KripkeStruct, KripkeStructError
 
 
-# test KripkeStruct()
-def test_ks_default_init():
+# Tests for KripkeStruct()
+def test_KS_default_init():
     ks = KripkeStruct()
     assert ks.atoms == ()
     assert ks.states == {}
-    assert ks.starts == ()
+    assert ks.starts == set()
     assert ks.trans == defaultdict(list)
     assert ks.trans_inverted == defaultdict(list)
 
 
-# test KripkeStruct(ks_json)
-def test_ks_file_init():
+# Tests for KripkeStruct(ks_json)
+def test_KS_file_init():
     ks_json = {
         "Atoms": ("a", "b", "c", "d"),
         "States": {"s1": 8, "s2": 12, "s3": 6, "s4": 7},
-        "Starts": ("s1",),
+        "Starts": ["s1"],
         "Trans": {"s1": ["s2"], "s2": ["s3", "s4"], "s3": ["s4"]},
     }
     ks = KripkeStruct(ks_json)
 
     assert ks.atoms == ("a", "b", "c", "d")
     assert ks.states == {"s1": 8, "s2": 12, "s3": 6, "s4": 7}
-    assert ks.starts == ("s1",)
+    assert ks.starts == {"s1"}
     assert dict(ks.trans) == {"s1": ["s2"], "s2": ["s3", "s4"], "s3": ["s4"]}
 
 
-# test ks.__str__()
-def test_ks_str_rep():
+# Tests for ks.__str__()
+def test_KS_str_rep():
     ks_json = {
         "Atoms": ("a", "b", "c", "d"),
         "States": {"s1": 8, "s2": 12, "s3": 6, "s4": 7},
-        "Starts": ("s1",),
+        "Starts": {"s1"},
         "Trans": {"s1": ["s2"], "s2": ["s3", "s4"], "s3": ["s4"]},
     }
     ks = KripkeStruct(ks_json)
     assert str(ks) == (
         "Atoms: ('a', 'b', 'c', 'd')\n"
         + "States: {'s1': 8, 's2': 12, 's3': 6, 's4': 7}\n"
-        + "Starts: ('s1',)\n"
+        + "Starts: {'s1'}\n"
         + "Trans: {'s1': ['s2'], 's2': ['s3', 's4'], 's3': ['s4']}"
     )
 
 
-def test_ks_set_atoms():
+def test_KS_set_atoms():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
     assert ks.atoms == ("a", "b", "c", "d")
 
     # if any state exists, can't reset atoms
     with pytest.raises(KripkeStructError) as error_info:
         ks.add_state("s1", 0b1000)
         atoms = ["a"]
         ks.set_atoms(atoms)
     assert str(error_info.value) == "Can't reset Atoms after States are Created"
 
 
-def test_ks_get_atoms():
+def test_KS_get_atoms():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
     assert ks.get_atoms() == atoms
 
 
-def test_ks_add_state():
+def test_KS_add_state():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
     ks.add_state("s1", 0b1000)
     assert ks.states == {"s1": 0b1000}
 
     # if the state name exists, can't add again
@@ -89,15 +89,15 @@
 
     # if the state label exisits, can't add again
     with pytest.raises(KripkeStructError) as error_info:
         ks.add_state("s8", 0b1000)
     assert str(error_info.value) == "Can't add an Exisiting State Label again"
 
 
-def test_ks_add_states():
+def test_KS_add_states():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
     states = {
         "s1": 0b1000,  # s1 has labels "a"
         "s2": 0b1100,  # s2 has labels "a", "b"
         "s3": 0b0110,  # s3 has labels "b", "c"
@@ -106,23 +106,36 @@
         "s6": 0b0010,  # s6 has label "c"
         "s7": 0b0001,  # s7 has label "d"
     }
     ks.add_states(states)
     assert ks.states == states
 
 
-def test_ks_get_states():
+def test_KS_get_states():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
     ks.add_state("s1", 0b1000)
     assert ks.get_states() == {"s1": 0b1000}
 
 
-def test_ks_remove_state():
+def test_KS_get_state_label_set():
+    ks = KripkeStruct()
+    atoms = ["a", "b", "c", "d"]
+    ks.set_atoms(atoms)
+    ks.add_state("s1", 0b1001)
+    assert ks.get_state_label_set("s1") == {"a", "d"}
+
+    # if the state doesn't exist, can't get the Label Set of it
+    with pytest.raises(KripkeStructError) as error_info:
+        assert ks.get_state_label_set("s2")
+    assert str(error_info.value) == "Can't get the Label Set of a Non-Exisiting State"
+
+
+def test_KS_remove_state():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
     states = {
         "s1": 0b1000,  # s1 has labels "a"
         "s2": 0b1100,  # s2 has labels "a", "b"
         "s3": 0b0110,  # s3 has labels "b", "c"
@@ -137,15 +150,15 @@
     assert ks.states == states
 
     # removing non-existing state won't have any effect
     ks.remove_state("s8")
     assert ks.states == states
 
 
-def test_ks_remove_states():
+def test_KS_remove_states():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
     states = {
         "s1": 0b1000,  # s1 has labels "a"
         "s2": 0b1100,  # s2 has labels "a", "b"
         "s3": 0b0110,  # s3 has labels "b", "c"
@@ -157,59 +170,59 @@
     ks.add_states(states)
     ks.remove_states(["s6", "s7"])
     states.pop("s7")
     states.pop("s6")
     assert ks.states == states
 
 
-def test_ks_set_starts():
+def test_KS_set_starts():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
     states = {
         "s1": 0b1000,  # s1 has labels "a"
         "s2": 0b1100,  # s2 has labels "a", "b"
         "s3": 0b0110,  # s3 has labels "b", "c"
         "s4": 0b0111,  # s4 has labels "b", "c", "d"
     }
     ks.add_states(states)
 
     starts = ["s1", "s4"]
     ks.set_starts(starts)
-    assert ks.starts == tuple(starts)
+    assert ks.starts == set(starts)
 
     # resetting the start states is allowed
     starts = ["s1"]
     ks.set_starts(starts)
-    assert ks.starts == tuple(starts)
+    assert ks.starts == set(starts)
 
     # if state doesn't exist, can't set as start state
     with pytest.raises(KripkeStructError) as error_info:
         ks.set_starts(["s5"])
     assert str(error_info.value) == "Can't set a Non-Exisiting State as Start State"
 
 
-def test_ks_get_starts():
+def test_KS_get_starts():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
     states = {
         "s1": 0b1000,  # s1 has labels "a"
         "s2": 0b1100,  # s2 has labels "a", "b"
         "s3": 0b0110,  # s3 has labels "b", "c"
         "s4": 0b0111,  # s4 has labels "b", "c", "d"
     }
     ks.add_states(states)
 
     starts = ["s1", "s4"]
     ks.set_starts(starts)
-    assert ks.get_starts() == starts
+    assert set(ks.get_starts()) == set(starts)
 
 
-def test_ks_add_trans():
+def test_KS_add_trans():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
     states = {
         "s1": 0b1000,  # s1 has labels "a"
         "s2": 0b1100,  # s2 has labels "a", "b"
         "s3": 0b0110,  # s3 has labels "b", "c"
@@ -236,15 +249,15 @@
     # if target state doesn't exist, can't add transition to it
     with pytest.raises(KripkeStructError) as error_info:
         trans = {"s1": ["s7"]}
         ks.add_trans(trans)
     assert str(error_info.value) == "Can't add Transition to a Non-Exisiting Target State"
 
 
-def test_ks_get_trans():
+def test_KS_get_trans():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
     states = {
         "s1": 0b1000,  # s1 has labels "a"
         "s2": 0b1100,  # s2 has labels "a", "b"
         "s3": 0b0110,  # s3 has labels "b", "c"
@@ -258,15 +271,15 @@
         "s3": ["s4", "s1"],  # bc -> bcd, a
         "s4": ["s2"],  # bcd -> ab
     }
     ks.add_trans(trans)
     assert ks.get_trans() == {"s1": ["s2"], "s2": ["s3", "s4"], "s3": ["s4", "s1"], "s4": ["s2"]}
 
 
-def test_ks_get_trans_inverted():
+def test_KS_get_trans_inverted():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
     states = {
         "s1": 0b1000,  # s1 has labels "a"
         "s2": 0b1100,  # s2 has labels "a", "b"
         "s3": 0b0110,  # s3 has labels "b", "c"
@@ -280,15 +293,15 @@
         "s3": ["s4", "s1"],  # bc -> bcd, a
         "s4": ["s2"],  # bcd -> ab
     }
     ks.add_trans(trans)
     assert ks.get_trans_inverted() == {"s1": ["s3"], "s2": ["s1", "s4"], "s3": ["s2"], "s4": ["s2", "s3"]}
 
 
-def test_ks_remove_trans():
+def test_KS_remove_trans():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
     states = {
         "s1": 0b1000,  # s1 has labels "a"
         "s2": 0b1100,  # s2 has labels "a", "b"
         "s3": 0b0110,  # s3 has labels "b", "c"
@@ -310,16 +323,57 @@
 
     # removing non-existing transition won't have any effect
     trans = {"s2": ["s4"]}
     ks.remove_trans(trans)
     assert ks.get_trans() == {"s1": ["s2"], "s2": ["s3"], "s3": ["s4", "s1"], "s4": []}
 
 
-# removing state will remove related transitions
-def test_ks_remove_states_will_remove_related_trans():
+def test_KS_get_SCCs():
+    ks_json = {
+        "Atoms": ("a", "b", "c", "d"),
+        "States": {
+            "s1": 0b1000,  # s1 has labels "a"
+            "s2": 0b1100,  # s2 has labels "a", "b"
+            "s3": 0b0110,  # s3 has labels "b", "c"
+            "s4": 0b0111,  # s4 has labels "b", "c", "d"
+            "s5": 0b0100,  # s5 has label "b"
+            "s6": 0b0010,  # s6 has label "c"
+            "s7": 0b0001,  # s7 has label "d"
+        },
+        "Starts": ["s1"],
+        "Trans": {
+            's1': ['s2'],
+            's2': ['s3', 's4'],
+            's3': ['s4'],
+            's4': ['s7'],
+            's5': ['s6'],
+            's6': ['s7', 's5'],
+            's7': ['s5'],
+        },
+    }
+    ks = KripkeStruct(ks_json)
+    SCC_1 = frozenset({"s1"})
+    SCC_2 = frozenset({"s2"})
+    SCC_3 = frozenset({"s3"})
+    SCC_4 = frozenset({"s4"})
+    SCC_5 = frozenset({"s5", "s6", "s7"})
+    assert ks.get_SCCs() == {SCC_1, SCC_2, SCC_3, SCC_4, SCC_5}
+
+    ks.add_trans({"s4": ["s2"]})
+    SCC_6 = frozenset({"s2", "s3", "s4"})
+    assert ks.get_SCCs() == {SCC_1, SCC_6, SCC_5}
+
+    ks.remove_states(["s3", "s4", "s6"])
+    SCC_7 = frozenset({"s5"})
+    SCC_8 = frozenset({"s7"})
+    assert ks.get_SCCs() == {SCC_1, SCC_2, SCC_7, SCC_8}
+
+
+# Integration Tests: removing state will remove related transitions
+def test_KS_remove_states_will_remove_related_trans():
     ks = KripkeStruct()
     atoms = ["a", "b", "c", "d"]
     ks.set_atoms(atoms)
     states = {
         "s1": 0b1000,  # s1 has labels "a"
         "s2": 0b1100,  # s2 has labels "a", "b"
         "s3": 0b0110,  # s3 has labels "b", "c"
```

### Comparing `mctk-py-0.0.1/mctk_py.egg-info/PKG-INFO` & `mctk-py-0.1.0/mctk_py.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mctk-py
-Version: 0.0.1
+Version: 0.1.0
 Summary: Model Checking Toolkit for Python
 Author-email: marcusm117 <marcusmin117@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -217,51 +217,51 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
 # Model Checking Toolkit (MCTK)
 
-[![Build Status](https://github.com/marcusm117/mctk/workflows/Build%20Status/badge.svg?branch=dev)](https://github.com/marcusm117/mctk/actions?query=workflow%3A%22Build+Status%22) [![codecov](https://codecov.io/gh/marcusm117/mctk/branch/dev/graph/badge.svg)](https://codecov.io/gh/marcusm117/mctk) [![License](https://img.shields.io/badge/License-Apache_2.0-green)](https://github.com/marcusm117/mctk/blob/dev/LICENSE) [![Issues](https://img.shields.io/github/issues/marcusm117/FV_mctk?color=red&label=Issues)](https://github.com/marcusm117/mctk/issues)
+[![PyPI](https://img.shields.io/pypi/v/mctk-py?color=blue&label=PyPI)](https://pypi.org/project/mctk-py/) [![CI](https://github.com/marcusm117/mctk/workflows/CI/badge.svg?branch=dev)](https://github.com/marcusm117/mctk/actions?query=workflow%3A%22Build+Status%22) [![codecov](https://codecov.io/gh/marcusm117/mctk/branch/dev/graph/badge.svg)](https://codecov.io/gh/marcusm117/mctk) [![Docs](https://github.com/marcusm117/mctk/workflows/Docs/badge.svg?branch=dev)](https://marcusm117.github.io/mctk/) [![License](https://img.shields.io/badge/License-Apache_2.0-green)](https://github.com/marcusm117/mctk/blob/dev/LICENSE) [![Issues](https://img.shields.io/github/issues/marcusm117/FV_mctk?color=red&label=Issues)](https://github.com/marcusm117/mctk/issues)
 
-Model Checking Toolkit in Python.
+[Model Checking Toolkit for Python.](https://marcusm117.github.io/mctk/)
 
 ## Overview
 
-`mctk` is a Python library for Explicit-State Model Checking (will also support Symbolic Model Checking and Bounded Model Checking in the future) on Kripke Structures (will also support other Transition Systems) supporting the CTL(Computation Tree Logic) operators: EX, EU, and EG.
+`mctk` is a Python library for Explicit-State Model Checking (will also support Symbolic Model Checking and Bounded Model Checking in the future) on Kripke Structures (will also support other Transition Systems) supporting the CTL(Computation Tree Logic) operators: **EX, EU, EG, EF, AX, AU, AG, AF**, and the Propositional Logic operators: **NOT, AND, OR, IMPLIES, IFF**.
 
-Users can create checker instances to formally verify if a Kripke Structure (can be created during runtime or input in a JSON file) satisfies certain CTL properties. The checker instance will return a set of satisfying states and "SAT" if satisfied or an Error Trace if unsatisfied.
+Users can use functions that implements CTL operators to formally verify if a Kripke Structure (can be created during runtime or input in a JSON file) satisfies certain CTL properties. All checking functions will return a set of states that satisfy the CTL property, which means that if any start state of the Kripke Structure is in the returned set, then the Kripke Structure satisfies the CTL property.
 
 ## Getting Started
 
 ### Installation
 
-Get the latest version of `mctk` from PyPI:
+Get the latest version of `mctk` from PyPI. Note that the registered name is 'mctk-py' on PyPI due to the strict typo-squatting prevention mechanism of the registry. However, when using the library, you should import it as 'mctk'.
 
    ``` bash
-   pip3 install mctk
+   pip3 install mctk-py
    ```
 
 If you are having trouble with `pip3`, you can also install from the source code, see [Developing](#developing).
 
 ### Developing
 
-Clone this Repository to your Local Environment
+Clone this Repository to your Local Environment.
 
    ``` bash
    git clone https://github.com/marcusm117/mctk.git
    ```
 
-Go into the Repository Directory
+Go into the Repository Directory.
 
    ``` bash
    cd mctk
    ```
 
-Install the Library with all Dependencies
+Install the Library with all Dependencies.
 
    ``` bash
    make develop
    ```
 
 ### Linting & Testing
 
@@ -271,23 +271,81 @@
 - `make lint`: perform static analysis of this library with `black`, `flake8` and `pylint`
 - `make annotate`: run type checking using `mypy`
 - `make test`: run automated tests with `pytest`
 - `make coverage`: run automated tests with `pytest` and collect coverage information
 
 ## Usage
 
+Create a Krinke Structure from scratch.
+
 ``` python
-from mctk import KripkeStruct
+from mctk import *
 
+# create a Kripke Structure from scratch
 ks = KripkeStruct()
+
+# set 2 Atomic Propositions in this Kripke Structure
 ks.set_atoms(["p", "q"])
+
+# add 2 states to the Kripke Structure
+# a State Name is represented by a string, it must be unique
+# a State Label is represented by a binary number, it must be unique
+# for example, 0b10 means the state has the Atoms "p" but not "q"
 ks.add_state("s0", 0b10)
 ks.add_state("s1", 0b01)
-ks.set_start(["s0"])
+
+# set the Start States of the Kripke Structure
+# there can be multiple Start States
+ks.set_starts(["s0"])
+
+# add 2 Transitions to the Kripke Structure
+# a Transition is represented by a key-value pair
+# where key the Source State Name and value is a list of Destination State Names
 ks.add_trans({"s0": ["s1"], "s1": ["s0"]})
 ```
 
+Check if the Kripke Structure satisfies a simple CTL formula.
+
+``` python
+# check if the Kripke Structure satisfies the CTL formula: EX p
+# SAT_atom(ks, "p") returns a set of states that satisfy the Atomic Proposition p
+# EX returns a set of states that satisfy the CTL formula EX p
+sat_states = EX(ks, SAT_atom(ks, "p"))
+
+# the result should be {"s1"}
+# since the start state "s0" is not in sat_states, ks doesn't satisfy the CTL formula
+assert sat_states == {"s1"}
+
+# check if the Kripke Structure satisfies the CTL formula: E p U q
+# SAT_atom(ks, "p") returns a set of states that satisfy the Atomic Proposition p
+# SAT_atom(ks, "q") returns a set of states that satisfy the Atomic Proposition q
+# EU returns a set of states that satisfy the CTL formula E p U q
+sat_states = EU(ks, SAT_atom(ks, "p"), SAT_atom(ks, "q"))
+
+# the result should be {"s0", "s1"}
+# since the start state "s0" is in sat_states, ks satisfies the CTL formula
+assert sat_states == {"s0", "s1"}
+```
+
+Check if the Kripke Structure satisfies a composite CTL formula.
+
+``` python
+# check if the Kripke Structure satisfies the CTL formula: EX (p AND EX q)
+sat_states = EX(ks, AND(SAT_atom(ks, "p"), EX(ks, SAT_atom(ks, "q"))))
+
+# the result should be {"s1"}
+# since the start state "s0" is not in sat_states, ks doesn't satisfy the CTL formula
+assert sat_states == {"s1"}
+
+# check if the Kripke Structure satisfies the CTL formula: EG (A p U (NOT q))
+sat_states = EG(ks, AU(ks, SAT_atom(ks, "p"), NOT(ks, SAT_atom(ks, "q"))))
+
+# the result should be set(), empty set
+# since the start state "s0" is not in sat_states, ks doesn't satisfy the CTL formula
+assert sat_states == set()
+```
+
 ## Contributing
 
 All contrbutions are welcome!
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details.
```

### Comparing `mctk-py-0.0.1/pyproject.toml` & `mctk-py-0.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "mctk-py"
 authors = [{name = "marcusm117", email = "marcusmin117@gmail.com"}]
 description="Model Checking Toolkit for Python"
 readme = "README.md"
-version = "0.0.1"
+version = "0.1.0"
 requires-python = ">=3.8"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
```


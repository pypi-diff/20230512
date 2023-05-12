# Comparing `tmp/choclo-0.0.1.tar.gz` & `tmp/choclo-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "choclo-0.0.1.tar", last modified: Sat Nov 19 00:38:23 2022, max compression
+gzip compressed data, was "choclo-0.1.0.tar", last modified: Fri May 12 20:36:31 2023, max compression
```

## Comparing `choclo-0.0.1.tar` & `choclo-0.1.0.tar`

### file list

```diff
@@ -1,43 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 00:38:23.266211 choclo-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-11-19 00:38:07.000000 choclo-0.0.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-11-19 00:38:07.000000 choclo-0.0.1/CITATION.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1496 2022-11-19 00:38:07.000000 choclo-0.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-11-19 00:38:07.000000 choclo-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5428 2022-11-19 00:38:23.266211 choclo-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3980 2022-11-19 00:38:07.000000 choclo-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 00:38:23.266211 choclo-0.0.1/choclo/
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-11-19 00:38:07.000000 choclo-0.0.1/choclo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-11-19 00:38:07.000000 choclo-0.0.1/choclo/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-19 00:38:23.000000 choclo-0.0.1/choclo/_version_generated.py
--rw-r--r--   0 runner    (1001) docker     (121)      503 2022-11-19 00:38:07.000000 choclo-0.0.1/choclo/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 00:38:23.266211 choclo-0.0.1/choclo/dipole/
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-11-19 00:38:07.000000 choclo-0.0.1/choclo/dipole/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10958 2022-11-19 00:38:07.000000 choclo-0.0.1/choclo/dipole/_forward.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 00:38:23.266211 choclo-0.0.1/choclo/point/
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-11-19 00:38:07.000000 choclo-0.0.1/choclo/point/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22079 2022-11-19 00:38:07.000000 choclo-0.0.1/choclo/point/_forward.py
--rw-r--r--   0 runner    (1001) docker     (121)    18198 2022-11-19 00:38:07.000000 choclo-0.0.1/choclo/point/_kernels.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 00:38:23.266211 choclo-0.0.1/choclo/prism/
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-11-19 00:38:07.000000 choclo-0.0.1/choclo/prism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    33356 2022-11-19 00:38:07.000000 choclo-0.0.1/choclo/prism/_gravity.py
--rw-r--r--   0 runner    (1001) docker     (121)    24958 2022-11-19 00:38:07.000000 choclo-0.0.1/choclo/prism/_kernels.py
--rw-r--r--   0 runner    (1001) docker     (121)    21700 2022-11-19 00:38:07.000000 choclo-0.0.1/choclo/prism/_magnetic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 00:38:23.266211 choclo-0.0.1/choclo/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-19 00:38:07.000000 choclo-0.0.1/choclo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27217 2022-11-19 00:38:07.000000 choclo-0.0.1/choclo/tests/test_dipole.py
--rw-r--r--   0 runner    (1001) docker     (121)     2328 2022-11-19 00:38:07.000000 choclo-0.0.1/choclo/tests/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (121)    26624 2022-11-19 00:38:07.000000 choclo-0.0.1/choclo/tests/test_point_gravity.py
--rw-r--r--   0 runner    (1001) docker     (121)    27376 2022-11-19 00:38:07.000000 choclo-0.0.1/choclo/tests/test_point_kernels.py
--rw-r--r--   0 runner    (1001) docker     (121)    42736 2022-11-19 00:38:07.000000 choclo-0.0.1/choclo/tests/test_prism_gravity.py
--rw-r--r--   0 runner    (1001) docker     (121)    28092 2022-11-19 00:38:07.000000 choclo-0.0.1/choclo/tests/test_prism_magnetic.py
--rw-r--r--   0 runner    (1001) docker     (121)     2808 2022-11-19 00:38:07.000000 choclo-0.0.1/choclo/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6538 2022-11-19 00:38:07.000000 choclo-0.0.1/choclo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 00:38:23.266211 choclo-0.0.1/choclo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5428 2022-11-19 00:38:23.000000 choclo-0.0.1/choclo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      833 2022-11-19 00:38:23.000000 choclo-0.0.1/choclo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-19 00:38:23.000000 choclo-0.0.1/choclo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-19 00:38:23.000000 choclo-0.0.1/choclo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-19 00:38:23.000000 choclo-0.0.1/choclo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-19 00:38:22.000000 choclo-0.0.1/choclo.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-11-19 00:38:07.000000 choclo-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1753 2022-11-19 00:38:23.270211 choclo-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:36:31.179335 choclo-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-12 20:36:16.000000 choclo-0.1.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-12 20:36:16.000000 choclo-0.1.0/CITATION.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-12 20:36:16.000000 choclo-0.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-12 20:36:16.000000 choclo-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-05-12 20:36:31.179335 choclo-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-05-12 20:36:16.000000 choclo-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:36:31.175335 choclo-0.1.0/choclo/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-12 20:36:31.000000 choclo-0.1.0/choclo/_version_generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:36:31.175335 choclo-0.1.0/choclo/dipole/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/dipole/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/dipole/_forward.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:36:31.175335 choclo-0.1.0/choclo/point/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/point/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21412 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/point/_forward.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:36:31.175335 choclo-0.1.0/choclo/prism/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/prism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46789 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/prism/_gravity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26070 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/prism/_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30129 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/prism/_magnetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14269 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/prism/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:36:31.179335 choclo-0.1.0/choclo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27024 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/tests/test_dipole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/tests/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26624 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/tests/test_point_gravity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66599 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/tests/test_prism_gravity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34717 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/tests/test_prism_magnetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-12 20:36:16.000000 choclo-0.1.0/choclo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:36:31.175335 choclo-0.1.0/choclo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-05-12 20:36:31.000000 choclo-0.1.0/choclo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-12 20:36:31.000000 choclo-0.1.0/choclo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:36:31.000000 choclo-0.1.0/choclo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 20:36:31.000000 choclo-0.1.0/choclo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 20:36:31.000000 choclo-0.1.0/choclo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:36:30.000000 choclo-0.1.0/choclo.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-12 20:36:16.000000 choclo-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-12 20:36:31.179335 choclo-0.1.0/setup.cfg
```

### Comparing `choclo-0.0.1/AUTHORS.md` & `choclo-0.1.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `choclo-0.0.1/LICENSE.txt` & `choclo-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `choclo-0.0.1/PKG-INFO` & `choclo-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: choclo
-Version: 0.0.1
+Version: 0.1.0
 Summary: Kernel functions for your geophysical models
 Home-page: https://github.com/fatiando/choclo
 Author: The Choclo Developers
 Author-email: fatiandoaterra@protonmail.com
 Maintainer: Santiago Soler
 Maintainer-email: santiago.r.soler@gmail.com
 License: BSD 3-Clause License
@@ -20,24 +20,23 @@
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Choclo
+<img src="https://github.com/fatiando/choclo/raw/main/doc/_static/readme-banner.png" alt="Choclo">
 
 <h2 align="center">Kernel functions for your geophysical models</h2>
 
 <p align="center">
 <a href="https://www.fatiando.org/choclo"><strong>Documentation</strong> (latest)</a> •
 <a href="https://www.fatiando.org/choclo/dev"><strong>Documentation</strong> (main branch)</a> •
 <a href="https://github.com/fatiando/choclo/blob/main/CONTRIBUTING.md"><strong>Contributing</strong></a> •
@@ -49,14 +48,15 @@
 </p>
 
 <p align="center">
 <a href="https://pypi.python.org/pypi/choclo"><img src="http://img.shields.io/pypi/v/choclo.svg?style=flat-square" alt="Latest version on PyPI"></a>
 <a href="https://github.com/conda-forge/choclo-feedstock"><img src="https://img.shields.io/conda/vn/conda-forge/choclo.svg?style=flat-square" alt="Latest version on conda-forge"></a>
 <a href="https://codecov.io/gh/fatiando/choclo"><img src="https://img.shields.io/codecov/c/github/fatiando/choclo/main.svg?style=flat-square" alt="Test coverage status"></a>
 <a href="https://pypi.python.org/pypi/choclo"><img src="https://img.shields.io/pypi/pyversions/choclo.svg?style=flat-square" alt="Compatible Python versions."></a>
+<a href="https://doi.org/10.5281/zenodo.7851747"><img src="https://img.shields.io/badge/doi-10.5281%2Fzenodo.7851747-blue?style=flat-square" alt="DOI used to cite Choclo"></a>
 </p>
 
 ## About
 
 **Choclo** is a Python library that hosts optimized kernel functions for
 running geophysical forward and inverse models, intended to be used by other
 libraries as the underlying layer of their computation.
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1 Name: choclo Version: 0.0.1 Summary: Kernel functions for
+Metadata-Version: 2.1 Name: choclo Version: 0.1.0 Summary: Kernel functions for
 your geophysical models Home-page: https://github.com/fatiando/choclo Author:
 The Choclo Developers Author-email: fatiandoaterra@protonmail.com Maintainer:
 Santiago Soler Maintainer-email: santiago.r.soler@gmail.com License: BSD 3-
 Clause License Project-URL: Documentation, https://www.fatiando.org/choclo
 Project-URL: Release Notes, https://github.com/fatiando/choclo/releases
 Project-URL: Bug Tracker, https://github.com/fatiando/choclo/issues Project-
 URL: Source Code, https://github.com/fatiando/choclo Keywords:
 geophysics,geoscience Platform: any Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Education Classifier: License ::
 OSI Approved :: BSD License Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
-3.6 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE.txt # Choclo
+3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
+LICENSE.txt [Choclo]
            ***** Kernel functions for your geophysical models *****
   Documentation_(latest) â¢ Documentation_(main_branch) â¢ Contributing â¢
                                     Contact
                      Part of the Fatiando_a_Terra project
 [Latest_version_on_PyPI] [Latest_version_on_conda-forge] [Test_coverage_status]
-                         [Compatible_Python_versions.]
+            [Compatible_Python_versions.] [DOI_used_to_cite_Choclo]
 ## About **Choclo** is a Python library that hosts optimized kernel functions
 for running geophysical forward and inverse models, intended to be used by
 other libraries as the underlying layer of their computation. "Choclo" is a
 term used in some countries of South America to refer to corn, originated from
 the [quechua](https://en.wikipedia.org/wiki/Quechuan_languages) word _chuqllu_.
 ## Project goals * Provide optimized kernel functions for gravity and magnetic
 forward and inverse models that can be easily harnessed by different
```

### Comparing `choclo-0.0.1/README.md` & `choclo-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Choclo
+<img src="https://github.com/fatiando/choclo/raw/main/doc/_static/readme-banner.png" alt="Choclo">
 
 <h2 align="center">Kernel functions for your geophysical models</h2>
 
 <p align="center">
 <a href="https://www.fatiando.org/choclo"><strong>Documentation</strong> (latest)</a> •
 <a href="https://www.fatiando.org/choclo/dev"><strong>Documentation</strong> (main branch)</a> •
 <a href="https://github.com/fatiando/choclo/blob/main/CONTRIBUTING.md"><strong>Contributing</strong></a> •
@@ -14,14 +14,15 @@
 </p>
 
 <p align="center">
 <a href="https://pypi.python.org/pypi/choclo"><img src="http://img.shields.io/pypi/v/choclo.svg?style=flat-square" alt="Latest version on PyPI"></a>
 <a href="https://github.com/conda-forge/choclo-feedstock"><img src="https://img.shields.io/conda/vn/conda-forge/choclo.svg?style=flat-square" alt="Latest version on conda-forge"></a>
 <a href="https://codecov.io/gh/fatiando/choclo"><img src="https://img.shields.io/codecov/c/github/fatiando/choclo/main.svg?style=flat-square" alt="Test coverage status"></a>
 <a href="https://pypi.python.org/pypi/choclo"><img src="https://img.shields.io/pypi/pyversions/choclo.svg?style=flat-square" alt="Compatible Python versions."></a>
+<a href="https://doi.org/10.5281/zenodo.7851747"><img src="https://img.shields.io/badge/doi-10.5281%2Fzenodo.7851747-blue?style=flat-square" alt="DOI used to cite Choclo"></a>
 </p>
 
 ## About
 
 **Choclo** is a Python library that hosts optimized kernel functions for
 running geophysical forward and inverse models, intended to be used by other
 libraries as the underlying layer of their computation.
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-# Choclo
+[Choclo]
            ***** Kernel functions for your geophysical models *****
   Documentation_(latest) â¢ Documentation_(main_branch) â¢ Contributing â¢
                                     Contact
                      Part of the Fatiando_a_Terra project
 [Latest_version_on_PyPI] [Latest_version_on_conda-forge] [Test_coverage_status]
-                         [Compatible_Python_versions.]
+            [Compatible_Python_versions.] [DOI_used_to_cite_Choclo]
 ## About **Choclo** is a Python library that hosts optimized kernel functions
 for running geophysical forward and inverse models, intended to be used by
 other libraries as the underlying layer of their computation. "Choclo" is a
 term used in some countries of South America to refer to corn, originated from
 the [quechua](https://en.wikipedia.org/wiki/Quechuan_languages) word _chuqllu_.
 ## Project goals * Provide optimized kernel functions for gravity and magnetic
 forward and inverse models that can be easily harnessed by different
```

### Comparing `choclo-0.0.1/choclo/_version.py` & `choclo-0.1.0/choclo/_version.py`

 * *Files identical despite different names*

### Comparing `choclo-0.0.1/choclo/dipole/_forward.py` & `choclo-0.1.0/choclo/dipole/_forward.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,23 @@
 from numba import jit
 
 from ..constants import VACUUM_MAGNETIC_PERMEABILITY
 
 
 @jit(nopython=True)
 def magnetic_field(
-    easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, magnetic_moment
+    easting_p,
+    northing_p,
+    upward_p,
+    easting_q,
+    northing_q,
+    upward_q,
+    magnetic_moment_east,
+    magnetic_moment_north,
+    magnetic_moment_up,
 ):
     r"""
     Magnetic field due to a dipole
 
     Returns the three components of the magnetic field due to a single dipole
     a single computation point.
 
@@ -37,18 +45,23 @@
         Upward coordinate of the observation point in meters.
     easting_q : float
         Easting coordinate of the dipole in meters.
     northing_q : float
         Northing coordinate of the dipole in meters.
     upward_q : float
         Upward coordinate of the dipole in meters.
-    magnetic_moment : 1d-array
-        Magnetic moment of the dipole. It should have three components in the
-        following order: ``mag_moment_easting``, ``mag_moment_northing``,
-        ``mag_moment_upward``. Should be in :math:`A m^2`.
+    magnetic_moment_east : float
+        The East component of the magnetic moment vector of the dipole. Must be
+        in :math:`A m^2`.
+    magnetic_moment_north : float
+        The North component of the magnetic moment vector of the dipole. Must
+        be in :math:`A m^2`.
+    magnetic_moment_up : float
+        The upward component of the magnetic moment vector of the dipole. Must
+        be in :math:`A m^2`.
 
     Returns
     -------
     b : array
         Array containing the three components of the magnetic field generated
         by the dipole on the observation point in :math:`\text{T}`.
         The components are returned in the following order: ``b_e``, ``b_n``,
@@ -85,32 +98,42 @@
     and :math:`\mu_0` is the vacuum magnetic permeability.
     """
     r_e = easting_p - easting_q
     r_n = northing_p - northing_q
     r_u = upward_p - upward_q
     distance = np.sqrt(r_e**2 + r_n**2 + r_u**2)
     dotproduct = (
-        magnetic_moment[0] * r_e + magnetic_moment[1] * r_n + magnetic_moment[2] * r_u
+        magnetic_moment_east * r_e
+        + magnetic_moment_north * r_n
+        + magnetic_moment_up * r_u
     )
     c_m = VACUUM_MAGNETIC_PERMEABILITY / 4 / np.pi
     b_e = c_m * (
-        3 * dotproduct * r_e / distance**5 - magnetic_moment[0] / distance**3
+        3 * dotproduct * r_e / distance**5 - magnetic_moment_east / distance**3
     )
     b_n = c_m * (
-        3 * dotproduct * r_n / distance**5 - magnetic_moment[1] / distance**3
+        3 * dotproduct * r_n / distance**5 - magnetic_moment_north / distance**3
     )
     b_u = c_m * (
-        3 * dotproduct * r_u / distance**5 - magnetic_moment[2] / distance**3
+        3 * dotproduct * r_u / distance**5 - magnetic_moment_up / distance**3
     )
     return b_e, b_n, b_u
 
 
 @jit(nopython=True)
 def magnetic_e(
-    easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, magnetic_moment
+    easting_p,
+    northing_p,
+    upward_p,
+    easting_q,
+    northing_q,
+    upward_q,
+    magnetic_moment_east,
+    magnetic_moment_north,
+    magnetic_moment_up,
 ):
     r"""
     Easting component of the magnetic field due to a dipole
 
     Returns the easting component of the magnetic field by a single dipole on
     a single computation point
 
@@ -124,18 +147,23 @@
         Upward coordinate of the observation point in meters.
     easting_q : float
         Easting coordinate of the dipole in meters.
     northing_q : float
         Northing coordinate of the dipole in meters.
     upward_q : float
         Upward coordinate of the dipole in meters.
-    magnetic_moment : 1d-array
-        Magnetic moment of the dipole. It should have three components in the
-        following order: ``mag_moment_easting``, ``mag_moment_northing``,
-        ``mag_moment_upward``. Should be in :math:`A m^2`.
+    magnetic_moment_east : float
+        The East component of the magnetic moment vector of the dipole. Must be
+        in :math:`A m^2`.
+    magnetic_moment_north : float
+        The North component of the magnetic moment vector of the dipole. Must
+        be in :math:`A m^2`.
+    magnetic_moment_up : float
+        The upward component of the magnetic moment vector of the dipole. Must
+        be in :math:`A m^2`.
 
     Returns
     -------
     b_e : float
         Easting component of the magnetic field generated by the dipole
         on the observation point in :math:`\text{T}`.
 
@@ -170,23 +198,33 @@
     and :math:`\mu_0` is the vacuum magnetic permeability.
     """
     r_e = easting_p - easting_q
     r_n = northing_p - northing_q
     r_u = upward_p - upward_q
     distance = np.sqrt(r_e**2 + r_n**2 + r_u**2)
     dotproduct = (
-        magnetic_moment[0] * r_e + magnetic_moment[1] * r_n + magnetic_moment[2] * r_u
+        magnetic_moment_east * r_e
+        + magnetic_moment_north * r_n
+        + magnetic_moment_up * r_u
     )
-    result = 3 * dotproduct * r_e / distance**5 - magnetic_moment[0] / distance**3
+    result = 3 * dotproduct * r_e / distance**5 - magnetic_moment_east / distance**3
     return VACUUM_MAGNETIC_PERMEABILITY / 4 / np.pi * result
 
 
 @jit(nopython=True)
 def magnetic_n(
-    easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, magnetic_moment
+    easting_p,
+    northing_p,
+    upward_p,
+    easting_q,
+    northing_q,
+    upward_q,
+    magnetic_moment_east,
+    magnetic_moment_north,
+    magnetic_moment_up,
 ):
     r"""
     Northing component of the magnetic field due to a dipole
 
     Returns the northing component of the magnetic field by a single dipole on
     a single computation point
 
@@ -200,18 +238,23 @@
         Upward coordinate of the observation point in meters.
     easting_q : float
         Easting coordinate of the dipole in meters.
     northing_q : float
         Northing coordinate of the dipole in meters.
     upward_q : float
         Upward coordinate of the dipole in meters.
-    magnetic_moment : 1d-array
-        Magnetic moment of the dipole. It should have three components in the
-        following order: ``mag_moment_easting``, ``mag_moment_northing``,
-        ``mag_moment_upward``. Should be in :math:`A m^2`.
+    magnetic_moment_east : float
+        The East component of the magnetic moment vector of the dipole. Must be
+        in :math:`A m^2`.
+    magnetic_moment_north : float
+        The North component of the magnetic moment vector of the dipole. Must
+        be in :math:`A m^2`.
+    magnetic_moment_up : float
+        The upward component of the magnetic moment vector of the dipole. Must
+        be in :math:`A m^2`.
 
     Returns
     -------
     b_n : float
         Northing component of the magnetic field generated by the dipole on the
         observation point in :math:`\text{T}`.
 
@@ -246,23 +289,35 @@
     and :math:`\mu_0` is the vacuum magnetic permeability.
     """
     r_e = easting_p - easting_q
     r_n = northing_p - northing_q
     r_u = upward_p - upward_q
     distance = np.sqrt(r_e**2 + r_n**2 + r_u**2)
     dotproduct = (
-        magnetic_moment[0] * r_e + magnetic_moment[1] * r_n + magnetic_moment[2] * r_u
+        magnetic_moment_east * r_e
+        + magnetic_moment_north * r_n
+        + magnetic_moment_up * r_u
+    )
+    result = (
+        3 * dotproduct * r_n / distance**5 - magnetic_moment_north / distance**3
     )
-    result = 3 * dotproduct * r_n / distance**5 - magnetic_moment[1] / distance**3
     return VACUUM_MAGNETIC_PERMEABILITY / 4 / np.pi * result
 
 
 @jit(nopython=True)
 def magnetic_u(
-    easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, magnetic_moment
+    easting_p,
+    northing_p,
+    upward_p,
+    easting_q,
+    northing_q,
+    upward_q,
+    magnetic_moment_east,
+    magnetic_moment_north,
+    magnetic_moment_up,
 ):
     r"""
     Upward component of the magnetic field due to a dipole
 
     Returns the upward component of the magnetic field by a single dipole on
     a single computation point
 
@@ -276,18 +331,23 @@
         Upward coordinate of the observation point in meters.
     easting_q : float
         Easting coordinate of the dipole in meters.
     northing_q : float
         Northing coordinate of the dipole in meters.
     upward_q : float
         Upward coordinate of the dipole in meters.
-    magnetic_moment : 1d-array
-        Magnetic moment of the dipole. It should have three components in the
-        following order: ``mag_moment_easting``, ``mag_moment_northing``,
-        ``mag_moment_upward``. Should be in :math:`A m^2`.
+    magnetic_moment_east : float
+        The East component of the magnetic moment vector of the dipole. Must be
+        in :math:`A m^2`.
+    magnetic_moment_north : float
+        The North component of the magnetic moment vector of the dipole. Must
+        be in :math:`A m^2`.
+    magnetic_moment_up : float
+        The upward component of the magnetic moment vector of the dipole. Must
+        be in :math:`A m^2`.
 
     Returns
     -------
     b_u : float
         Upward component of the magnetic field generated by the dipole on the
         observation point in :math:`\text{T}`.
 
@@ -322,11 +382,13 @@
     and :math:`\mu_0` is the vacuum magnetic permeability.
     """
     r_e = easting_p - easting_q
     r_n = northing_p - northing_q
     r_u = upward_p - upward_q
     distance = np.sqrt(r_e**2 + r_n**2 + r_u**2)
     dotproduct = (
-        magnetic_moment[0] * r_e + magnetic_moment[1] * r_n + magnetic_moment[2] * r_u
+        magnetic_moment_east * r_e
+        + magnetic_moment_north * r_n
+        + magnetic_moment_up * r_u
     )
-    result = 3 * dotproduct * r_u / distance**5 - magnetic_moment[2] / distance**3
+    result = 3 * dotproduct * r_u / distance**5 - magnetic_moment_up / distance**3
     return VACUUM_MAGNETIC_PERMEABILITY / 4 / np.pi * result
```

### Comparing `choclo-0.0.1/choclo/point/__init__.py` & `choclo-0.1.0/choclo/prism/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Copyright (c) 2022 The Choclo Developers.
 # Distributed under the terms of the BSD 3-Clause License.
 # SPDX-License-Identifier: BSD-3-Clause
 #
 # This code is part of the Fatiando a Terra project (https://www.fatiando.org)
 #
 """
-Kernels and forward modelling functions for point sources
+Kernels and forward modelling functions for rectangular prisms
 """
-from ._forward import (
+from ._gravity import (
     gravity_e,
     gravity_ee,
     gravity_en,
     gravity_eu,
     gravity_n,
     gravity_nn,
     gravity_nu,
@@ -27,7 +27,8 @@
     kernel_n,
     kernel_nn,
     kernel_nu,
     kernel_pot,
     kernel_u,
     kernel_uu,
 )
+from ._magnetic import magnetic_e, magnetic_field, magnetic_n, magnetic_u
```

### Comparing `choclo-0.0.1/choclo/point/_forward.py` & `choclo-0.1.0/choclo/point/_forward.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,26 +7,14 @@
 """
 Forward modelling function for point sources
 """
 from numba import jit
 
 from ..constants import GRAVITATIONAL_CONST
 from ..utils import distance_cartesian
-from ._kernels import (
-    kernel_e,
-    kernel_ee,
-    kernel_en,
-    kernel_eu,
-    kernel_n,
-    kernel_nn,
-    kernel_nu,
-    kernel_pot,
-    kernel_u,
-    kernel_uu,
-)
 
 
 @jit(nopython=True)
 def gravity_pot(easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, mass):
     r"""
     Gravitational potential field due to a point source
 
@@ -70,18 +58,15 @@
     where :math:`\lVert \cdot \rVert_2` refer to the :math:`L_2` norm (the
     Euclidean distance between :math:`\mathbf{p}` and :math:`\mathbf{q}`)
     and :math:`G` is the Universal Gravitational Constant.
     """
     distance = distance_cartesian(
         easting_p, northing_p, upward_p, easting_q, northing_q, upward_q
     )
-    kernel = kernel_pot(
-        easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, distance
-    )
-    return GRAVITATIONAL_CONST * mass * kernel
+    return GRAVITATIONAL_CONST * mass / distance
 
 
 @jit(nopython=True)
 def gravity_e(easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, mass):
     r"""
     Easting component of the gravitational acceleration due to a point source
 
@@ -130,17 +115,15 @@
     where :math:`\lVert \cdot \rVert_2` refer to the :math:`L_2` norm (the
     Euclidean distance between :math:`\mathbf{p}` and :math:`\mathbf{q}`)
     and :math:`G` is the Universal Gravitational Constant.
     """
     distance = distance_cartesian(
         easting_p, northing_p, upward_p, easting_q, northing_q, upward_q
     )
-    kernel = kernel_e(
-        easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, distance
-    )
+    kernel = -(easting_p - easting_q) / distance**3
     return GRAVITATIONAL_CONST * mass * kernel
 
 
 @jit(nopython=True)
 def gravity_n(easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, mass):
     r"""
     Northing component of the gravitational acceleration due to a point source
@@ -190,17 +173,15 @@
     where :math:`\lVert \cdot \rVert_2` refer to the :math:`L_2` norm (the
     Euclidean distance between :math:`\mathbf{p}` and :math:`\mathbf{q}`)
     and :math:`G` is the Universal Gravitational Constant.
     """
     distance = distance_cartesian(
         easting_p, northing_p, upward_p, easting_q, northing_q, upward_q
     )
-    kernel = kernel_n(
-        easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, distance
-    )
+    kernel = -(northing_p - northing_q) / distance**3
     return GRAVITATIONAL_CONST * mass * kernel
 
 
 @jit(nopython=True)
 def gravity_u(easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, mass):
     r"""
     Upward component of the gravitational acceleration due to a point source
@@ -250,17 +231,15 @@
     where :math:`\lVert \cdot \rVert_2` refer to the :math:`L_2` norm (the
     Euclidean distance between :math:`\mathbf{p}` and :math:`\mathbf{q}`)
     and :math:`G` is the Universal Gravitational Constant.
     """
     distance = distance_cartesian(
         easting_p, northing_p, upward_p, easting_q, northing_q, upward_q
     )
-    kernel = kernel_u(
-        easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, distance
-    )
+    kernel = -(upward_p - upward_q) / distance**3
     return GRAVITATIONAL_CONST * mass * kernel
 
 
 @jit(nopython=True)
 def gravity_ee(easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, mass):
     r"""
     Easting-easting component of the gravitational tensor due to a point source
@@ -317,17 +296,15 @@
     where :math:`\lVert \cdot \rVert_2` refer to the :math:`L_2` norm (the
     Euclidean distance between :math:`\mathbf{p}` and :math:`\mathbf{q}`)
     and :math:`G` is the Universal Gravitational Constant.
     """
     distance = distance_cartesian(
         easting_p, northing_p, upward_p, easting_q, northing_q, upward_q
     )
-    kernel = kernel_ee(
-        easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, distance
-    )
+    kernel = 3 * (easting_p - easting_q) ** 2 / distance**5 - 1 / distance**3
     return GRAVITATIONAL_CONST * mass * kernel
 
 
 @jit(nopython=True)
 def gravity_nn(easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, mass):
     r"""
     Northing-northing component of the gravitational tensor due to point source
@@ -384,17 +361,15 @@
     where :math:`\lVert \cdot \rVert_2` refer to the :math:`L_2` norm (the
     Euclidean distance between :math:`\mathbf{p}` and :math:`\mathbf{q}`)
     and :math:`G` is the Universal Gravitational Constant.
     """
     distance = distance_cartesian(
         easting_p, northing_p, upward_p, easting_q, northing_q, upward_q
     )
-    kernel = kernel_nn(
-        easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, distance
-    )
+    kernel = 3 * (northing_p - northing_q) ** 2 / distance**5 - 1 / distance**3
     return GRAVITATIONAL_CONST * mass * kernel
 
 
 @jit(nopython=True)
 def gravity_uu(easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, mass):
     r"""
     Upward-upward component of the gravitational tensor due to a point source
@@ -451,17 +426,15 @@
     where :math:`\lVert \cdot \rVert_2` refer to the :math:`L_2` norm (the
     Euclidean distance between :math:`\mathbf{p}` and :math:`\mathbf{q}`)
     and :math:`G` is the Universal Gravitational Constant.
     """
     distance = distance_cartesian(
         easting_p, northing_p, upward_p, easting_q, northing_q, upward_q
     )
-    kernel = kernel_uu(
-        easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, distance
-    )
+    kernel = 3 * (upward_p - upward_q) ** 2 / distance**5 - 1 / distance**3
     return GRAVITATIONAL_CONST * mass * kernel
 
 
 @jit(nopython=True)
 def gravity_en(easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, mass):
     r"""
     Easting-northing component of the gravitational tensor due to point source
@@ -513,17 +486,15 @@
     where :math:`\lVert \cdot \rVert_2` refer to the :math:`L_2` norm (the
     Euclidean distance between :math:`\mathbf{p}` and :math:`\mathbf{q}`)
     and :math:`G` is the Universal Gravitational Constant.
     """
     distance = distance_cartesian(
         easting_p, northing_p, upward_p, easting_q, northing_q, upward_q
     )
-    kernel = kernel_en(
-        easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, distance
-    )
+    kernel = 3 * (easting_p - easting_q) * (northing_p - northing_q) / distance**5
     return GRAVITATIONAL_CONST * mass * kernel
 
 
 @jit(nopython=True)
 def gravity_eu(easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, mass):
     r"""
     Easting-upward component of the gravitational tensor due to point source
@@ -575,17 +546,15 @@
     where :math:`\lVert \cdot \rVert_2` refer to the :math:`L_2` norm (the
     Euclidean distance between :math:`\mathbf{p}` and :math:`\mathbf{q}`)
     and :math:`G` is the Universal Gravitational Constant.
     """
     distance = distance_cartesian(
         easting_p, northing_p, upward_p, easting_q, northing_q, upward_q
     )
-    kernel = kernel_eu(
-        easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, distance
-    )
+    kernel = 3 * (easting_p - easting_q) * (upward_p - upward_q) / distance**5
     return GRAVITATIONAL_CONST * mass * kernel
 
 
 @jit(nopython=True)
 def gravity_nu(easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, mass):
     r"""
     Northing-upward component of the gravitational tensor due to point source
@@ -637,11 +606,9 @@
     where :math:`\lVert \cdot \rVert_2` refer to the :math:`L_2` norm (the
     Euclidean distance between :math:`\mathbf{p}` and :math:`\mathbf{q}`)
     and :math:`G` is the Universal Gravitational Constant.
     """
     distance = distance_cartesian(
         easting_p, northing_p, upward_p, easting_q, northing_q, upward_q
     )
-    kernel = kernel_nu(
-        easting_p, northing_p, upward_p, easting_q, northing_q, upward_q, distance
-    )
+    kernel = 3 * (northing_p - northing_q) * (upward_p - upward_q) / distance**5
     return GRAVITATIONAL_CONST * mass * kernel
```

### Comparing `choclo-0.0.1/choclo/prism/_gravity.py` & `choclo-0.1.0/choclo/prism/_kernels.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,1159 +1,848 @@
 # Copyright (c) 2022 The Choclo Developers.
 # Distributed under the terms of the BSD 3-Clause License.
 # SPDX-License-Identifier: BSD-3-Clause
 #
 # This code is part of the Fatiando a Terra project (https://www.fatiando.org)
 #
 """
-Gravity forward modelling functions for rectangular prisms
+Kernel functions for rectangular prisms
 """
 import numpy as np
 from numba import jit
 
-from ..constants import GRAVITATIONAL_CONST
-from ._kernels import (
-    kernel_e,
-    kernel_ee,
-    kernel_en,
-    kernel_eu,
-    kernel_n,
-    kernel_nn,
-    kernel_nu,
-    kernel_pot,
-    kernel_u,
-    kernel_uu,
-)
-
 
 @jit(nopython=True)
-def gravity_pot(easting, northing, upward, prism, density):
+def kernel_pot(easting, northing, upward, radius):
     r"""
-    Gravitational potential field due to a rectangular prism
+    Kernel for the potential field due to a rectangular prism
+
+    Evaluates the integration kernel for the potential field generated by
+    a prism [Nagy2000] on a single vertex of the prism. The coordinates that
+    must be passed are shifted coordinates: the coordinates of the vertex from
+    a Cartesian coordinate system whose origin is located in the observation
+    point.
 
-    Returns the gravitational potential field produced by a single rectangular
-    prism on a single computation point.
+    This function makes use of a safe natural logarithmic function and a safe
+    arctangent function [Fukushima2020]_ that guarantee a good accuracy on
+    every observation point.
 
     Parameters
     ----------
     easting : float
-        Easting coordinate of the observation point. Must be in meters.
+        Shifted easting coordinate of the vertex of the prism. Must be in
+        meters.
     northing : float
-        Northing coordinate of the observation point. Must be in meters.
+        Shifted northing coordinate of the vertex of the prism. Must be in
+        meters.
     upward : float
-        Upward coordinate of the observation point. Must be in meters.
-    prism : 1d-array
-        One dimensional array containing the coordinates of the prism in the
-        following order: ``west``, ``east``, ``south``, ``north``, ``bottom``,
-        ``top`` in a Cartesian coordinate system.
-        All coordinates should be in meters.
+        Shifted upward coordinate of the vertex of the prism. Must be in
+        meters.
+    radius : float
+        Square root of the sum of the squares of the ``easting``, ``northing``
+        and ``upward`` shifted coordinates.
 
     Returns
     -------
-    potential : float
-        Gravitational potential field generated by the rectangular prism on the
-        observation point in :math:`\text{J}/\text{kg}`.
+    kernel : float
+        Value of the numerical kernel function for the potential field due to
+        a rectangular prism evaluated on a single vertex.
 
     Notes
     -----
-    Returns the gravitational potential field :math:`V(\mathbf{p})` on the
-    observation point :math:`\mathbf{p} = (x_p, y_p, z_p)` generated by
-    a single rectangular prism defined by its boundaries :math:`x_1, x_2, y_1,
-    y_2, z_1, z_2` and with a density :math:`\rho`:
-
-    .. math::
-
-        V(\mathbf{p}) =
-            G
-            \rho \,\,
-            \Bigg\lvert \Bigg\lvert \Bigg\lvert
-            k_V(x, y, z)
-            \Bigg\rvert_{X_1}^{X_2}
-            \Bigg\rvert_{Y_1}^{Y_2}
-            \Bigg\rvert_{Z_1}^{Z_2}
-
-    where
+    Computes the following numerical kernel on the passed *shifted
+    coordinates*:
 
     .. math::
 
         k_V(x, y, z) &=
-            x y \, \text{ln2} (z + r)
-            + y z \, \text{ln2} (x + r)
-            + z x \, \text{ln2} (y + r) \\
-            - \frac{x^2}{2} &\text{arctan2} \left( \frac{yz}{xr} \right)
-            - \frac{y^2}{2} \text{arctan2} \left( \frac{zx}{yr} \right)
-            - \frac{z^2}{2} \text{arctan2} \left( \frac{xy}{zr} \right),
-
-    .. math::
-
-        r = \sqrt{x^2 + y^2 + z^2},
-
-    and
-
-    .. math::
-
-        X_1 = x_1 - x_p \\
-        X_2 = x_2 - x_p \\
-        Y_1 = y_1 - y_p \\
-        Y_2 = y_2 - y_p \\
-        Z_1 = z_1 - z_p \\
-        Z_2 = z_2 - z_p
+            x y \, \operatorname{safe-ln} (z + r)
+            + y z \, \operatorname{safe-ln} (x + r)
+            + z x \, \operatorname{safe-ln} (y + r) \\
+            & - \frac{x^2}{2} \operatorname{safe-arctan} \left( yz, xr \right)
+            - \frac{y^2}{2} \operatorname{safe-arctan} \left( zx, yr \right)
+            - \frac{z^2}{2} \operatorname{safe-arctan} \left( xy, zr \right)
 
-    are the shifted coordinates of the prism boundaries and :math:`G` is the
-    Universal Gravitational Constant.
-
-    The :math:`\text{ln2}` and :math:`\text{arctan2}` functions are defined as
-    follows:
+    where
 
     .. math::
 
-        \text{ln2}(x) =
+        \operatorname{safe-ln}(x) =
         \begin{cases}
             0 & |x| < 10^{-10} \\
             \ln (x)
         \end{cases}
 
+    and
+
     .. math::
 
-        \text{arctan2} \left( \frac{y}{x} \right) =
+        \operatorname{safe-arctan} \left( y, x \right) =
         \begin{cases}
             \text{arctan}\left( \frac{y}{x} \right) & x \ne 0 \\
             \frac{\pi}{2} & x = 0 \quad \text{and} \quad y > 0 \\
             -\frac{\pi}{2} & x = 0 \quad \text{and} \quad y < 0 \\
             0 & x = 0 \quad \text{and} \quad y = 0 \\
         \end{cases}
 
-    These were defined after [Fukushima2020]_ and guarantee a good accuracy on
-    any observation point.
-
     References
     ----------
     - [Nagy2000]_
     - [Nagy2002]_
     - [Fukushima2020]_
     """
-    return (
-        GRAVITATIONAL_CONST
-        * density
-        * _evaluate_kernel(easting, northing, upward, prism, kernel_pot)
+    kernel = (
+        easting * northing * _safe_log(upward, radius)
+        + northing * upward * _safe_log(easting, radius)
+        + easting * upward * _safe_log(northing, radius)
+        - 0.5 * easting**2 * _safe_atan2(upward * northing, easting * radius)
+        - 0.5 * northing**2 * _safe_atan2(upward * easting, northing * radius)
+        - 0.5 * upward**2 * _safe_atan2(easting * northing, upward * radius)
     )
+    return kernel
 
 
 @jit(nopython=True)
-def gravity_e(easting, northing, upward, prism, density):
+def kernel_e(easting, northing, upward, radius):
     r"""
-    Easting component of the gravitational acceleration due to a prism
+    Kernel for easting component of the gradient due to a rectangular prism
 
-    Returns the easting component of the gravitational acceleration produced by
-    a single rectangular prism on a single computation point.
+    Evaluates the integration kernel for the easting component of the gradient
+    of the potential field generated by a prism [Nagy2000]_ on a single vertex
+    of the prism. The coordinates that must be passed are shifted coordinates:
+    the coordinates of the vertex from a Cartesian coordinate system whose
+    origin is located in the observation point.
+
+    This function makes use of a safe natural logarithmic function and a safe
+    arctangent function [Fukushima2020]_ that guarantee a good accuracy on
+    every observation point.
 
     Parameters
     ----------
     easting : float
-        Easting coordinate of the observation point. Must be in meters.
+        Shifted easting coordinate of the vertex of the prism. Must be in
+        meters.
     northing : float
-        Northing coordinate of the observation point. Must be in meters.
+        Shifted northing coordinate of the vertex of the prism. Must be in
+        meters.
     upward : float
-        Upward coordinate of the observation point. Must be in meters.
-    prism : 1d-array
-        One dimensional array containing the coordinates of the prism in the
-        following order: ``west``, ``east``, ``south``, ``north``, ``bottom``,
-        ``top`` in a Cartesian coordinate system.
-        All coordinates should be in meters.
+        Shifted upward coordinate of the vertex of the prism. Must be in
+        meters.
+    radius : float
+        Square root of the sum of the squares of the ``easting``, ``northing``
+        and ``upward`` shifted coordinates.
 
     Returns
     -------
-    g_e : float
-        Easting component of the gravitational acceleration generated by the
-        rectangular prism on the observation point in
-        :math:`\text{m}/\text{s}^2`.
+    kernel : float
+        Value of the numerical kernel function for the easting component of the
+        gradient of the potential field due to a rectangular prism evaluated on
+        a single vertex.
 
     Notes
     -----
-    Returns the easting component :math:`g_x(\mathbf{p})` of the gravitational
-    acceleration :math:`\mathbf{g}` on the observation point :math:`\mathbf{p}
-    = (x_p, y_p, z_p)` generated by a single rectangular prism defined by its
-    boundaries :math:`x_1, x_2, y_1, y_2, z_1, z_2` and with a density
-    :math:`\rho`:
-
-    .. math::
-
-        g_x(\mathbf{p}) =
-            G
-            \rho \,\,
-            \Bigg\lvert \Bigg\lvert \Bigg\lvert
-            k_x(x, y, z)
-            \Bigg\rvert_{X_1}^{X_2}
-            \Bigg\rvert_{Y_1}^{Y_2}
-            \Bigg\rvert_{Z_1}^{Z_2}
-
-    where
+    Computes the following numerical kernel on the passed *shifted
+    coordinates*:
 
     .. math::
 
         k_x(x, y, z) =
-            \left[
-            y \, \text{ln2} (z + r)
-            + z \, \text{ln2} (y + r)
-            - x \, \text{arctan2} \left( \frac{yz}{xr} \right)
+            -\left[
+            y \, \operatorname{safe-ln} (z + r)
+            + z \, \operatorname{safe-ln} (y + r)
+            - x \, \operatorname{safe-arctan} \left( yz, xr \right)
             \right]
 
-    .. math::
-
-        r = \sqrt{x^2 + y^2 + z^2},
-
-    and
-
-    .. math::
-
-        X_1 = x_1 - x_p \\
-        X_2 = x_2 - x_p \\
-        Y_1 = y_1 - y_p \\
-        Y_2 = y_2 - y_p \\
-        Z_1 = z_1 - z_p \\
-        Z_2 = z_2 - z_p
-
-    are the shifted coordinates of the prism boundaries and :math:`G` is the
-    Universal Gravitational Constant.
-
-    The :math:`\text{ln2}` and :math:`\text{arctan2}` functions are defined as
-    follows:
+    where
 
     .. math::
 
-        \text{ln2}(x) =
+        \operatorname{safe-ln}(x) =
         \begin{cases}
             0 & |x| < 10^{-10} \\
             \ln (x)
         \end{cases}
 
+    and
+
     .. math::
 
-        \text{arctan2} \left( \frac{y}{x} \right) =
+        \operatorname{safe-arctan} \left( y, x \right) =
         \begin{cases}
             \text{arctan}\left( \frac{y}{x} \right) & x \ne 0 \\
             \frac{\pi}{2} & x = 0 \quad \text{and} \quad y > 0 \\
             -\frac{\pi}{2} & x = 0 \quad \text{and} \quad y < 0 \\
             0 & x = 0 \quad \text{and} \quad y = 0 \\
         \end{cases}
 
-    These were defined after [Fukushima2020]_ and guarantee a good accuracy on
-    any observation point.
+    .. important::
+
+        In the first equation a minus sign has been added to the one obtained
+        by [Nagy2000]_ in order to compute the numerical kernel for the
+        **eastward** component instead for the westward one.
 
     References
     ----------
     - [Nagy2000]_
     - [Nagy2002]_
     - [Fukushima2020]_
     """
-    return (
-        GRAVITATIONAL_CONST
-        * density
-        * _evaluate_kernel(easting, northing, upward, prism, kernel_e)
+    kernel = -(
+        northing * _safe_log(upward, radius)
+        + upward * _safe_log(northing, radius)
+        - easting * _safe_atan2(northing * upward, easting * radius)
     )
+    return kernel
 
 
 @jit(nopython=True)
-def gravity_n(easting, northing, upward, prism, density):
+def kernel_n(easting, northing, upward, radius):
     r"""
-    Northing component of the gravitational acceleration due to a prism
+    Kernel for northing component of the gradient due to a rectangular prism
 
-    Returns the northing component of the gravitational acceleration produced
-    by a single rectangular prism on a single computation point.
+    Evaluates the integration kernel for the northing component of the gradient
+    of the potential field generated by a prism [Nagy2000]_ on a single vertex
+    of the prism. The coordinates that must be passed are shifted coordinates:
+    the coordinates of the vertex from a Cartesian coordinate system whose
+    origin is located in the observation point.
+
+    This function makes use of a safe natural logarithmic function and a safe
+    arctangent function [Fukushima2020]_ that guarantee a good accuracy on
+    every observation point.
 
     Parameters
     ----------
     easting : float
-        Easting coordinate of the observation point. Must be in meters.
+        Shifted easting coordinate of the vertex of the prism. Must be in
+        meters.
     northing : float
-        Northing coordinate of the observation point. Must be in meters.
+        Shifted northing coordinate of the vertex of the prism. Must be in
+        meters.
     upward : float
-        Upward coordinate of the observation point. Must be in meters.
-    prism : 1d-array
-        One dimensional array containing the coordinates of the prism in the
-        following order: ``west``, ``east``, ``south``, ``north``, ``bottom``,
-        ``top`` in a Cartesian coordinate system.
-        All coordinates should be in meters.
+        Shifted upward coordinate of the vertex of the prism. Must be in
+        meters.
+    radius : float
+        Square root of the sum of the squares of the ``easting``, ``northing``
+        and ``upward`` shifted coordinates.
 
     Returns
     -------
-    g_n : float
-        Northing component of the gravitational acceleration generated by the
-        rectangular prism on the observation point in
-        :math:`\text{m}/\text{s}^2`.
+    kernel : float
+        Value of the numerical kernel function for the northing component of
+        the gradient of the potential field due to a rectangular prism
+        evaluated on a single vertex.
 
     Notes
     -----
-    Returns the northing component :math:`g_y(\mathbf{p})` of the gravitational
-    acceleration :math:`\mathbf{g}` on the observation point :math:`\mathbf{p}
-    = (x_p, y_p, z_p)` generated by a single rectangular prism defined by its
-    boundaries :math:`x_1, x_2, y_1, y_2, z_1, z_2` and with a density
-    :math:`\rho`:
-
-    .. math::
-
-        g_y(\mathbf{p}) =
-            G
-            \rho \,\,
-            \Bigg\lvert \Bigg\lvert \Bigg\lvert
-            k_y(x, y, z)
-            \Bigg\rvert_{X_1}^{X_2}
-            \Bigg\rvert_{Y_1}^{Y_2}
-            \Bigg\rvert_{Z_1}^{Z_2}
-
-    where
+    Computes the following numerical kernel on the passed *shifted
+    coordinates*:
 
     .. math::
 
         k_y(x, y, z) =
-            \left[
-            z \, \text{ln2} (x + r)
-            + x \, \text{ln2} (z + r)
-            - y \, \text{arctan2} \left( \frac{zx}{yr} \right)
+            -\left[
+            z \, \operatorname{safe-ln} (x + r)
+            + x \, \operatorname{safe-ln} (z + r)
+            - y \, \operatorname{safe-arctan} \left( zx, yr \right)
             \right]
 
-    .. math::
-
-        r = \sqrt{x^2 + y^2 + z^2},
-
-    and
-
-    .. math::
-
-        X_1 = x_1 - x_p \\
-        X_2 = x_2 - x_p \\
-        Y_1 = y_1 - y_p \\
-        Y_2 = y_2 - y_p \\
-        Z_1 = z_1 - z_p \\
-        Z_2 = z_2 - z_p
-
-    are the shifted coordinates of the prism boundaries and :math:`G` is the
-    Universal Gravitational Constant.
-
-    The :math:`\text{ln2}` and :math:`\text{arctan2}` functions are defined as
-    follows:
+    where
 
     .. math::
 
-        \text{ln2}(x) =
+        \operatorname{safe-ln}(x) =
         \begin{cases}
             0 & |x| < 10^{-10} \\
             \ln (x)
         \end{cases}
 
+    and
+
     .. math::
 
-        \text{arctan2} \left( \frac{y}{x} \right) =
+        \operatorname{safe-arctan} \left( y, x \right) =
         \begin{cases}
             \text{arctan}\left( \frac{y}{x} \right) & x \ne 0 \\
             \frac{\pi}{2} & x = 0 \quad \text{and} \quad y > 0 \\
             -\frac{\pi}{2} & x = 0 \quad \text{and} \quad y < 0 \\
             0 & x = 0 \quad \text{and} \quad y = 0 \\
         \end{cases}
 
-    These were defined after [Fukushima2020]_ and guarantee a good accuracy on
-    any observation point.
+    .. important::
+
+        In the first equation a minus sign has been added to the one obtained
+        by [Nagy2000]_ in order to compute the numerical kernel for the
+        **northward** component instead for the southward one.
 
     References
     ----------
     - [Nagy2000]_
     - [Nagy2002]_
     - [Fukushima2020]_
     """
-    return (
-        GRAVITATIONAL_CONST
-        * density
-        * _evaluate_kernel(easting, northing, upward, prism, kernel_n)
+    kernel = -(
+        upward * _safe_log(easting, radius)
+        + easting * _safe_log(upward, radius)
+        - northing * _safe_atan2(easting * upward, northing * radius)
     )
+    return kernel
 
 
 @jit(nopython=True)
-def gravity_u(easting, northing, upward, prism, density):
+def kernel_u(easting, northing, upward, radius):
     r"""
-    Upward component of the gravitational acceleration due to a prism
+    Kernel for upward component of the gradient due to a rectangular prism
+
+    Evaluates the integration kernel for the upward component of the gradient
+    of the potential field generated by a prism [Nagy2000]_ on a single vertex
+    of the prism. The coordinates that must be passed are shifted coordinates:
+    the coordinates of the vertex from a Cartesian coordinate system whose
+    origin is located in the observation point.
 
-    Returns the upward component of the gravitational acceleration produced by
-    a single rectangular prism on a single computation point.
+    This function makes use of a safe natural logarithmic function and a safe
+    arctangent function [Fukushima2020]_ that guarantee a good accuracy on
+    every observation point.
 
     Parameters
     ----------
     easting : float
-        Easting coordinate of the observation point. Must be in meters.
+        Shifted easting coordinate of the vertex of the prism. Must be in
+        meters.
     northing : float
-        Northing coordinate of the observation point. Must be in meters.
+        Shifted northing coordinate of the vertex of the prism. Must be in
+        meters.
     upward : float
-        Upward coordinate of the observation point. Must be in meters.
-    prism : 1d-array
-        One dimensional array containing the coordinates of the prism in the
-        following order: ``west``, ``east``, ``south``, ``north``, ``bottom``,
-        ``top`` in a Cartesian coordinate system.
-        All coordinates should be in meters.
+        Shifted upward coordinate of the vertex of the prism. Must be in
+        meters.
+    radius : float
+        Square root of the sum of the squares of the ``easting``, ``northing``
+        and ``upward`` shifted coordinates.
 
     Returns
     -------
-    g_u : float
-        Upward component of the gravitational acceleration generated by the
-        rectangular prism on the observation point in
-        :math:`\text{m}/\text{s}^2`.
+    kernel : float
+        Value of the numerical kernel function for the upward component of the
+        gradient of the potential field due to a rectangular prism evaluated on
+        a single vertex.
 
     Notes
     -----
-    Returns the upward component :math:`g_z(\mathbf{p})` of the gravitational
-    acceleration :math:`\mathbf{g}` on the observation point :math:`\mathbf{p}
-    = (x_p, y_p, z_p)` generated by a single rectangular prism defined by its
-    boundaries :math:`x_1, x_2, y_1, y_2, z_1, z_2` and with a density
-    :math:`\rho`:
-
-    .. math::
-
-        g_z(\mathbf{p}) =
-            G
-            \rho \,\,
-            \Bigg\lvert \Bigg\lvert \Bigg\lvert
-            k_z(x, y, z)
-            \Bigg\rvert_{X_1}^{X_2}
-            \Bigg\rvert_{Y_1}^{Y_2}
-            \Bigg\rvert_{Z_1}^{Z_2}
-
-    where
+    Computes the following numerical kernel on the passed *shifted
+    coordinates*:
 
     .. math::
 
         k_z(x, y, z) =
             - \left[
-            x \, \text{ln2} (y + r)
-            + y \, \text{ln2} (x + r)
-            - z \, \text{arctan2} \left( \frac{xy}{zr} \right)
+            x \, \operatorname{safe-ln} (y + r)
+            + y \, \operatorname{safe-ln} (x + r)
+            - z \, \operatorname{safe-arctan} \left( xy, zr \right)
             \right]
 
-    .. math::
-
-        r = \sqrt{x^2 + y^2 + z^2},
-
-    and
-
-    .. math::
-
-        X_1 = x_1 - x_p \\
-        X_2 = x_2 - x_p \\
-        Y_1 = y_1 - y_p \\
-        Y_2 = y_2 - y_p \\
-        Z_1 = z_1 - z_p \\
-        Z_2 = z_2 - z_p
-
-    are the shifted coordinates of the prism boundaries and :math:`G` is the
-    Universal Gravitational Constant.
-
-    .. important
-
-        The minus sign in the :math:`k_x(x, y, z)` function is needed to return
-        the **upward** component of the acceleration. [Nagy2000]_ and
-        [Nagy2002]_ equation corresponds to the *downward* coordinate.
-
-    The :math:`\text{ln2}` and :math:`\text{arctan2}` functions are defined as
-    follows:
+    where
 
     .. math::
 
-        \text{ln2}(x) =
+        \operatorname{safe-ln}(x) =
         \begin{cases}
             0 & |x| < 10^{-10} \\
             \ln (x)
         \end{cases}
 
+    and
+
     .. math::
 
-        \text{arctan2} \left( \frac{y}{x} \right) =
+        \operatorname{safe-arctan} \left( y, x \right) =
         \begin{cases}
             \text{arctan}\left( \frac{y}{x} \right) & x \ne 0 \\
             \frac{\pi}{2} & x = 0 \quad \text{and} \quad y > 0 \\
             -\frac{\pi}{2} & x = 0 \quad \text{and} \quad y < 0 \\
             0 & x = 0 \quad \text{and} \quad y = 0 \\
         \end{cases}
 
-    These were defined after [Fukushima2020]_ and guarantee a good accuracy on
-    any observation point.
+    .. important::
+
+        In the first equation a minus sign has been added to the one obtained
+        by [Nagy2000]_ in order to compute the numerical kernel for the
+        **upward** component instead for the downward one.
+
 
     References
     ----------
     - [Nagy2000]_
     - [Nagy2002]_
     - [Fukushima2020]_
     """
-    return (
-        GRAVITATIONAL_CONST
-        * density
-        * _evaluate_kernel(easting, northing, upward, prism, kernel_u)
+    # The minus sign is to return the kernel for the upward component instead
+    # of the downward one.
+    kernel = -(
+        easting * _safe_log(northing, radius)
+        + northing * _safe_log(easting, radius)
+        - upward * _safe_atan2(easting * northing, upward * radius)
     )
+    return kernel
 
 
 @jit(nopython=True)
-def gravity_ee(easting, northing, upward, prism, density):
+def kernel_ee(easting, northing, upward, radius):
     r"""
-    Easting-easting component of the gravitational tensor due to a prism
+    Kernel for easting-easting component of the tensor due to a prism
 
-    Returns the easting-easting component of the gravitational tensor produced
-    by a single rectangular prism on a single computation point.
+    Evaluates the integration kernel for the easting-easting component of the
+    tensor generated by a prism [Nagy2000]_ on a single vertex of the prism.
+    The coordinates that must be passed are shifted coordinates: the
+    coordinates of the vertex from a Cartesian coordinate system whose origin
+    is located in the observation point.
+
+    This function makes use of a safe arctangent function [Fukushima2020]_ that
+    guarantee a good accuracy on every observation point.
 
     Parameters
     ----------
     easting : float
-        Easting coordinate of the observation point. Must be in meters.
+        Shifted easting coordinate of the vertex of the prism. Must be in
+        meters.
     northing : float
-        Northing coordinate of the observation point. Must be in meters.
+        Shifted northing coordinate of the vertex of the prism. Must be in
+        meters.
     upward : float
-        Upward coordinate of the observation point. Must be in meters.
-    prism : 1d-array
-        One dimensional array containing the coordinates of the prism in the
-        following order: ``west``, ``east``, ``south``, ``north``, ``bottom``,
-        ``top`` in a Cartesian coordinate system.
-        All coordinates should be in meters.
+        Shifted upward coordinate of the vertex of the prism. Must be in
+        meters.
+    radius : float
+        Square root of the sum of the squares of the ``easting``, ``northing``
+        and ``upward`` shifted coordinates.
 
     Returns
     -------
-    g_ee : float
-        Easting-easting component of the gravitational tensor generated by the
-        rectangular prism on the observation point in
-        :math:`\text{m}/\text{s}^2`.
+    kernel : float
+        Value of the kernel function for the easting-easting component of the
+        tensor due to a rectangular prism evaluated on a single vertex.
 
     Notes
     -----
-    Returns the easting-easting component :math:`g_{xx}(\mathbf{p})` of the
-    gravitational tensor :math:`\mathbf{T}` on the observation point
-    :math:`\mathbf{p} = (x_p, y_p, z_p)` generated by a single rectangular
-    prism defined by its boundaries :math:`x_1, x_2, y_1, y_2, z_1, z_2` and
-    with a density :math:`\rho`:
+    Computes the following numerical kernel on the passed *shifted
+    coordinates*:
 
     .. math::
 
-        g_{xx}(\mathbf{p}) =
-            G
-            \rho \,\,
-            \Bigg\lvert \Bigg\lvert \Bigg\lvert
-            k_{xx}(x, y, z)
-            \Bigg\rvert_{X_1}^{X_2}
-            \Bigg\rvert_{Y_1}^{Y_2}
-            \Bigg\rvert_{Z_1}^{Z_2}
+        k_{xx}(x, y, z) = - \operatorname{safe-arctan} \left( yz, xr \right)
 
     where
 
     .. math::
 
-        k_{xx}(x, y, z) = - \text{arctan2} \left( \frac{yz}{xr} \right),
-
-    .. math::
-
-        r = \sqrt{x^2 + y^2 + z^2},
-
-    and
-
-    .. math::
-
-        X_1 = x_1 - x_p \\
-        X_2 = x_2 - x_p \\
-        Y_1 = y_1 - y_p \\
-        Y_2 = y_2 - y_p \\
-        Z_1 = z_1 - z_p \\
-        Z_2 = z_2 - z_p
-
-    are the shifted coordinates of the prism boundaries and :math:`G` is the
-    Universal Gravitational Constant.
-
-    The :math:`\text{arctan2}` function is defined as follows:
-
-    .. math::
-
-        \text{arctan2} \left( \frac{y}{x} \right) =
+        \operatorname{safe-arctan} \left( y, x \right) =
         \begin{cases}
             \text{arctan}\left( \frac{y}{x} \right) & x \ne 0 \\
             \frac{\pi}{2} & x = 0 \quad \text{and} \quad y > 0 \\
             -\frac{\pi}{2} & x = 0 \quad \text{and} \quad y < 0 \\
             0 & x = 0 \quad \text{and} \quad y = 0 \\
         \end{cases}
 
-    It was defined after [Fukushima2020]_ and guarantee a good accuracy on any
-    observation point.
-
     References
     ----------
     - [Nagy2000]_
     - [Nagy2002]_
     - [Fukushima2020]_
     """
-    return (
-        GRAVITATIONAL_CONST
-        * density
-        * _evaluate_kernel(easting, northing, upward, prism, kernel_ee)
-    )
+    return -_safe_atan2(northing * upward, easting * radius)
 
 
 @jit(nopython=True)
-def gravity_nn(easting, northing, upward, prism, density):
+def kernel_nn(easting, northing, upward, radius):
     r"""
-    Northing-northing component of the gravitational tensor due to a prism
+    Kernel for northing-northing component of the tensor due to a prism
+
+    Evaluates the integration kernel for the northing-northing component of the
+    tensor generated by a prism [Nagy2000]_ on a single vertex of the prism.
+    The coordinates that must be passed are shifted coordinates: the
+    coordinates of the vertex from a Cartesian coordinate system whose origin
+    is located in the observation point.
 
-    Returns the northing-northing component of the gravitational tensor
-    produced by a single rectangular prism on a single computation point.
+    This function makes use of a safe arctangent function [Fukushima2020]_ that
+    guarantee a good accuracy on every observation point.
 
     Parameters
     ----------
     easting : float
-        Easting coordinate of the observation point. Must be in meters.
+        Shifted easting coordinate of the vertex of the prism. Must be in
+        meters.
     northing : float
-        Northing coordinate of the observation point. Must be in meters.
+        Shifted northing coordinate of the vertex of the prism. Must be in
+        meters.
     upward : float
-        Upward coordinate of the observation point. Must be in meters.
-    prism : 1d-array
-        One dimensional array containing the coordinates of the prism in the
-        following order: ``west``, ``east``, ``south``, ``north``, ``bottom``,
-        ``top`` in a Cartesian coordinate system.
-        All coordinates should be in meters.
+        Shifted upward coordinate of the vertex of the prism. Must be in
+        meters.
+    radius : float
+        Square root of the sum of the squares of the ``easting``, ``northing``
+        and ``upward`` shifted coordinates.
 
     Returns
     -------
-    g_nn : float
-        Northing-northing component of the gravitational tensor generated by
-        the rectangular prism on the observation point in
-        :math:`\text{m}/\text{s}^2`.
+    kernel : float
+        Value of the kernel function for the northing-northing component of the
+        tensor due to a rectangular prism evaluated on a single vertex.
 
     Notes
     -----
-    Returns the northing-northing component :math:`g_{yy}(\mathbf{p})` of the
-    gravitational tensor :math:`\mathbf{T}` on the observation point
-    :math:`\mathbf{p} = (x_p, y_p, z_p)` generated by a single rectangular
-    prism defined by its boundaries :math:`x_1, x_2, y_1, y_2, z_1, z_2` and
-    with a density :math:`\rho`:
+    Computes the following numerical kernel on the passed *shifted
+    coordinates*:
 
     .. math::
 
-        g_{yy}(\mathbf{p}) =
-            G
-            \rho \,\,
-            \Bigg\lvert \Bigg\lvert \Bigg\lvert
-            k_{yy}(x, y, z)
-            \Bigg\rvert_{X_1}^{X_2}
-            \Bigg\rvert_{Y_1}^{Y_2}
-            \Bigg\rvert_{Z_1}^{Z_2}
+        k_{yy}(x, y, z) = - \operatorname{safe-arctan} \left( zx, yr \right)
 
     where
 
     .. math::
 
-        k_{yy}(x, y, z) = - \text{arctan2} \left( \frac{zx}{yr} \right),
-
-    .. math::
-
-        r = \sqrt{x^2 + y^2 + z^2},
-
-    and
-
-    .. math::
-
-        X_1 = x_1 - x_p \\
-        X_2 = x_2 - x_p \\
-        Y_1 = y_1 - y_p \\
-        Y_2 = y_2 - y_p \\
-        Z_1 = z_1 - z_p \\
-        Z_2 = z_2 - z_p
-
-    are the shifted coordinates of the prism boundaries and :math:`G` is the
-    Universal Gravitational Constant.
-
-    The :math:`\text{arctan2}` function is defined as follows:
-
-    .. math::
-
-        \text{arctan2} \left( \frac{y}{x} \right) =
+        \operatorname{safe-arctan} \left( y, x \right) =
         \begin{cases}
             \text{arctan}\left( \frac{y}{x} \right) & x \ne 0 \\
             \frac{\pi}{2} & x = 0 \quad \text{and} \quad y > 0 \\
             -\frac{\pi}{2} & x = 0 \quad \text{and} \quad y < 0 \\
             0 & x = 0 \quad \text{and} \quad y = 0 \\
         \end{cases}
 
-    It was defined after [Fukushima2020]_ and guarantee a good accuracy on any
-    observation point.
-
     References
     ----------
     - [Nagy2000]_
     - [Nagy2002]_
     - [Fukushima2020]_
     """
-    return (
-        GRAVITATIONAL_CONST
-        * density
-        * _evaluate_kernel(easting, northing, upward, prism, kernel_nn)
-    )
+    return -_safe_atan2(easting * upward, northing * radius)
 
 
 @jit(nopython=True)
-def gravity_uu(easting, northing, upward, prism, density):
+def kernel_uu(easting, northing, upward, radius):
     r"""
-    Upward-upward component of the gravitational tensor due to a prism
+    Kernel for upward-upward component of the tensor due to a prism
+
+    Evaluates the integration kernel for the upward-upward component of the
+    tensor generated by a prism [Nagy2000]_ on a single vertex of the prism.
+    The coordinates that must be passed are shifted coordinates: the
+    coordinates of the vertex from a Cartesian coordinate system whose origin
+    is located in the observation point.
 
-    Returns the northing-northing component of the gravitational tensor
-    produced by a single rectangular prism on a single computation point.
+    This function makes use of a safe arctangent function [Fukushima2020]_ that
+    guarantee a good accuracy on every observation point.
 
     Parameters
     ----------
     easting : float
-        Easting coordinate of the observation point. Must be in meters.
+        Shifted easting coordinate of the vertex of the prism. Must be in
+        meters.
     northing : float
-        Northing coordinate of the observation point. Must be in meters.
+        Shifted northing coordinate of the vertex of the prism. Must be in
+        meters.
     upward : float
-        Upward coordinate of the observation point. Must be in meters.
-    prism : 1d-array
-        One dimensional array containing the coordinates of the prism in the
-        following order: ``west``, ``east``, ``south``, ``north``, ``bottom``,
-        ``top`` in a Cartesian coordinate system.
-        All coordinates should be in meters.
+        Shifted upward coordinate of the vertex of the prism. Must be in
+        meters.
+    radius : float
+        Square root of the sum of the squares of the ``easting``, ``northing``
+        and ``upward`` shifted coordinates.
 
     Returns
     -------
-    g_uu : float
-        Upward-upward component of the gravitational tensor generated by
-        the rectangular prism on the observation point in
-        :math:`\text{m}/\text{s}^2`.
+    kernel : float
+        Value of the kernel function for the upward-upward component of the
+        tensor due to a rectangular prism evaluated on a single vertex.
 
     Notes
     -----
-    Returns the upward-upward component :math:`g_{zz}(\mathbf{p})` of the
-    gravitational tensor :math:`\mathbf{T}` on the observation point
-    :math:`\mathbf{p} = (x_p, y_p, z_p)` generated by a single rectangular
-    prism defined by its boundaries :math:`x_1, x_2, y_1, y_2, z_1, z_2` and
-    with a density :math:`\rho`:
+    Computes the following numerical kernel on the passed *shifted
+    coordinates*:
 
     .. math::
 
-        g_{zz}(\mathbf{p}) =
-            G
-            \rho \,\,
-            \Bigg\lvert \Bigg\lvert \Bigg\lvert
-            k_{zz}(x, y, z)
-            \Bigg\rvert_{X_1}^{X_2}
-            \Bigg\rvert_{Y_1}^{Y_2}
-            \Bigg\rvert_{Z_1}^{Z_2}
+        k_{zz}(x, y, z) = - \operatorname{safe-arctan} \left( xy, zr \right)
 
     where
 
     .. math::
 
-        k_{zz}(x, y, z) = - \text{arctan2} \left( \frac{xy}{zr} \right),
-
-    .. math::
-
-        r = \sqrt{x^2 + y^2 + z^2},
-
-    and
-
-    .. math::
-
-        X_1 = x_1 - x_p \\
-        X_2 = x_2 - x_p \\
-        Y_1 = y_1 - y_p \\
-        Y_2 = y_2 - y_p \\
-        Z_1 = z_1 - z_p \\
-        Z_2 = z_2 - z_p
-
-    are the shifted coordinates of the prism boundaries and :math:`G` is the
-    Universal Gravitational Constant.
-
-    The :math:`\text{arctan2}` function is defined as follows:
-
-    .. math::
-
-        \text{arctan2} \left( \frac{y}{x} \right) =
+        \operatorname{safe-arctan} \left( y, x \right) =
         \begin{cases}
             \text{arctan}\left( \frac{y}{x} \right) & x \ne 0 \\
             \frac{\pi}{2} & x = 0 \quad \text{and} \quad y > 0 \\
             -\frac{\pi}{2} & x = 0 \quad \text{and} \quad y < 0 \\
             0 & x = 0 \quad \text{and} \quad y = 0 \\
         \end{cases}
 
-    It was defined after [Fukushima2020]_ and guarantee a good accuracy on any
-    observation point.
-
     References
     ----------
     - [Nagy2000]_
     - [Nagy2002]_
     - [Fukushima2020]_
     """
-    return (
-        GRAVITATIONAL_CONST
-        * density
-        * _evaluate_kernel(easting, northing, upward, prism, kernel_uu)
-    )
+    return -_safe_atan2(easting * northing, upward * radius)
 
 
 @jit(nopython=True)
-def gravity_en(easting, northing, upward, prism, density):
+def kernel_en(easting, northing, upward, radius):
     r"""
-    Easting-northing component of the gravitational tensor due to a prism
+    Kernel for easting-northing component of the tensor due to a prism
+
+    Evaluates the integration kernel for the easting-northing component of the
+    tensor generated by a prism [Nagy2000]_ on a single vertex of the prism.
+    The coordinates that must be passed are shifted coordinates: the
+    coordinates of the vertex from a Cartesian coordinate system whose origin
+    is located in the observation point.
 
-    Returns the northing-northing component of the gravitational tensor
-    produced by a single rectangular prism on a single computation point.
+    This function makes use of a safe natural logarithmic function
+    [Fukushima2020]_ that guarantee a good accuracy on every observation point.
 
     Parameters
     ----------
     easting : float
-        Easting coordinate of the observation point. Must be in meters.
+        Shifted easting coordinate of the vertex of the prism. Must be in
+        meters.
     northing : float
-        Northing coordinate of the observation point. Must be in meters.
+        Shifted northing coordinate of the vertex of the prism. Must be in
+        meters.
     upward : float
-        Upward coordinate of the observation point. Must be in meters.
-    prism : 1d-array
-        One dimensional array containing the coordinates of the prism in the
-        following order: ``west``, ``east``, ``south``, ``north``, ``bottom``,
-        ``top`` in a Cartesian coordinate system.
-        All coordinates should be in meters.
+        Shifted upward coordinate of the vertex of the prism. Must be in
+        meters.
+    radius : float
+        Square root of the sum of the squares of the ``easting``, ``northing``
+        and ``upward`` shifted coordinates.
 
     Returns
     -------
-    g_en : float
-        Easting-northing component of the gravitational tensor generated by the
-        rectangular prism on the observation point in
-        :math:`\text{m}/\text{s}^2`.
+    kernel : float
+        Value of the kernel function for the easting-northing component of the
+        tensor due to a rectangular prism evaluated on a single vertex.
 
     Notes
     -----
-    Returns the easting-northing component :math:`g_{xy}(\mathbf{p})` of the
-    gravitational tensor :math:`\mathbf{T}` on the observation point
-    :math:`\mathbf{p} = (x_p, y_p, z_p)` generated by a single rectangular
-    prism defined by its boundaries :math:`x_1, x_2, y_1, y_2, z_1, z_2` and
-    with a density :math:`\rho`:
+    Computes the following numerical kernel on the passed *shifted
+    coordinates*:
 
     .. math::
 
-        g_{xy}(\mathbf{p}) =
-            G
-            \rho \,\,
-            \Bigg\lvert \Bigg\lvert \Bigg\lvert
-            k_{xy}(x, y, z)
-            \Bigg\rvert_{X_1}^{X_2}
-            \Bigg\rvert_{Y_1}^{Y_2}
-            \Bigg\rvert_{Z_1}^{Z_2}
+        k_{xy}(x, y, z) = \operatorname{safe-ln} \left( z + r \right)
 
     where
 
     .. math::
 
-        k_{xy}(x, y, z) = \text{ln2} \left( z + r \right),
-
-    .. math::
-
-        r = \sqrt{x^2 + y^2 + z^2},
-
-    and
-
-    .. math::
-
-        X_1 = x_1 - x_p \\
-        X_2 = x_2 - x_p \\
-        Y_1 = y_1 - y_p \\
-        Y_2 = y_2 - y_p \\
-        Z_1 = z_1 - z_p \\
-        Z_2 = z_2 - z_p
-
-    are the shifted coordinates of the prism boundaries and :math:`G` is the
-    Universal Gravitational Constant.
-
-    The :math:`\text{ln2}` function is defined as follows:
-
-    .. math::
-
-        \text{ln2}(x) =
+        \operatorname{safe-ln}(x) =
         \begin{cases}
             0 & |x| < 10^{-10} \\
             \ln (x)
         \end{cases}
 
-    It was defined after [Fukushima2020]_ and guarantee a good accuracy on any
-    observation point.
-
     References
     ----------
     - [Nagy2000]_
     - [Nagy2002]_
     - [Fukushima2020]_
     """
-    return (
-        GRAVITATIONAL_CONST
-        * density
-        * _evaluate_kernel(easting, northing, upward, prism, kernel_en)
-    )
+    return _safe_log(upward, radius)
 
 
 @jit(nopython=True)
-def gravity_eu(easting, northing, upward, prism, density):
+def kernel_eu(easting, northing, upward, radius):
     r"""
-    Easting-upward component of the gravitational tensor due to a prism
+    Kernel for easting-upward component of the tensor due to a prism
+
+    Evaluates the integration kernel for the easting-upward component of the
+    tensor generated by a prism [Nagy2000]_ on a single vertex of the prism.
+    The coordinates that must be passed are shifted coordinates: the
+    coordinates of the vertex from a Cartesian coordinate system whose origin
+    is located in the observation point.
 
-    Returns the easting-upward component of the gravitational tensor
-    produced by a single rectangular prism on a single computation point.
+    This function makes use of a safe natural logarithmic function
+    [Fukushima2020]_ that guarantee a good accuracy on every observation point.
 
     Parameters
     ----------
     easting : float
-        Easting coordinate of the observation point. Must be in meters.
+        Shifted easting coordinate of the vertex of the prism. Must be in
+        meters.
     northing : float
-        Northing coordinate of the observation point. Must be in meters.
+        Shifted northing coordinate of the vertex of the prism. Must be in
+        meters.
     upward : float
-        Upward coordinate of the observation point. Must be in meters.
-    prism : 1d-array
-        One dimensional array containing the coordinates of the prism in the
-        following order: ``west``, ``east``, ``south``, ``north``, ``bottom``,
-        ``top`` in a Cartesian coordinate system.
-        All coordinates should be in meters.
+        Shifted upward coordinate of the vertex of the prism. Must be in
+        meters.
+    radius : float
+        Square root of the sum of the squares of the ``easting``, ``northing``
+        and ``upward`` shifted coordinates.
 
     Returns
     -------
-    g_eu : float
-        Easting-upward component of the gravitational tensor generated by the
-        rectangular prism on the observation point in
-        :math:`\text{m}/\text{s}^2`.
+    kernel : float
+        Value of the kernel function for the easting-upward component of the
+        tensor due to a rectangular prism evaluated on a single vertex.
 
     Notes
     -----
-    Returns the easting-upward component :math:`g_{xz}(\mathbf{p})` of the
-    gravitational tensor :math:`\mathbf{T}` on the observation point
-    :math:`\mathbf{p} = (x_p, y_p, z_p)` generated by a single rectangular
-    prism defined by its boundaries :math:`x_1, x_2, y_1, y_2, z_1, z_2` and
-    with a density :math:`\rho`:
+    Computes the following numerical kernel on the passed *shifted
+    coordinates*:
 
     .. math::
 
-        g_{xz}(\mathbf{p}) =
-            G
-            \rho \,\,
-            \Bigg\lvert \Bigg\lvert \Bigg\lvert
-            k_{xz}(x, y, z)
-            \Bigg\rvert_{X_1}^{X_2}
-            \Bigg\rvert_{Y_1}^{Y_2}
-            \Bigg\rvert_{Z_1}^{Z_2}
+        k_{xz}(x, y, z) = \operatorname{safe-ln} \left( y + r \right)
 
     where
 
     .. math::
 
-        k_{xz}(x, y, z) = \text{ln2} \left( y + r \right),
-
-    .. math::
-
-        r = \sqrt{x^2 + y^2 + z^2},
-
-    and
-
-    .. math::
-
-        X_1 = x_1 - x_p \\
-        X_2 = x_2 - x_p \\
-        Y_1 = y_1 - y_p \\
-        Y_2 = y_2 - y_p \\
-        Z_1 = z_1 - z_p \\
-        Z_2 = z_2 - z_p
-
-    are the shifted coordinates of the prism boundaries and :math:`G` is the
-    Universal Gravitational Constant.
-
-    The :math:`\text{ln2}` function is defined as follows:
-
-    .. math::
-
-        \text{ln2}(x) =
+        \operatorname{safe-ln}(x) =
         \begin{cases}
             0 & |x| < 10^{-10} \\
             \ln (x)
         \end{cases}
 
-    It was defined after [Fukushima2020]_ and guarantee a good accuracy on any
-    observation point.
-
     References
     ----------
     - [Nagy2000]_
     - [Nagy2002]_
     - [Fukushima2020]_
     """
-    return (
-        GRAVITATIONAL_CONST
-        * density
-        * _evaluate_kernel(easting, northing, upward, prism, kernel_eu)
-    )
+    return _safe_log(northing, radius)
 
 
 @jit(nopython=True)
-def gravity_nu(easting, northing, upward, prism, density):
+def kernel_nu(easting, northing, upward, radius):
     r"""
-    Northing-upward component of the gravitational tensor due to a prism
+    Kernel for northing-upward component of the tensor due to a prism
 
-    Returns the northing-upward component of the gravitational tensor
-    produced by a single rectangular prism on a single computation point.
+    Evaluates the integration kernel for the northing-upward component of the
+    tensor generated by a prism [Nagy2000]_ on a single vertex of the prism.
+    The coordinates that must be passed are shifted coordinates: the
+    coordinates of the vertex from a Cartesian coordinate system whose origin
+    is located in the observation point.
+
+    This function makes use of a safe natural logarithmic function
+    [Fukushima2020]_ that guarantee a good accuracy on every observation point.
 
     Parameters
     ----------
     easting : float
-        Easting coordinate of the observation point. Must be in meters.
+        Shifted easting coordinate of the vertex of the prism. Must be in
+        meters.
     northing : float
-        Northing coordinate of the observation point. Must be in meters.
+        Shifted northing coordinate of the vertex of the prism. Must be in
+        meters.
     upward : float
-        Upward coordinate of the observation point. Must be in meters.
-    prism : 1d-array
-        One dimensional array containing the coordinates of the prism in the
-        following order: ``west``, ``east``, ``south``, ``north``, ``bottom``,
-        ``top`` in a Cartesian coordinate system.
-        All coordinates should be in meters.
+        Shifted upward coordinate of the vertex of the prism. Must be in
+        meters.
+    radius : float
+        Square root of the sum of the squares of the ``easting``, ``northing``
+        and ``upward`` shifted coordinates.
 
     Returns
     -------
-    g_nu : float
-        Northing-upward component of the gravitational tensor generated by the
-        rectangular prism on the observation point in
-        :math:`\text{m}/\text{s}^2`.
+    kernel : float
+        Value of the kernel function for the northing-upward component of the
+        tensor due to a rectangular prism evaluated on a single vertex.
 
     Notes
     -----
-    Returns the northing-upward component :math:`g_{yz}(\mathbf{p})` of the
-    gravitational tensor :math:`\mathbf{T}` on the observation point
-    :math:`\mathbf{p} = (x_p, y_p, z_p)` generated by a single rectangular
-    prism defined by its boundaries :math:`x_1, x_2, y_1, y_2, z_1, z_2` and
-    with a density :math:`\rho`:
+    Computes the following numerical kernel on the passed *shifted
+    coordinates*:
 
     .. math::
 
-        g_{yz}(\mathbf{p}) =
-            G
-            \rho \,\,
-            \Bigg\lvert \Bigg\lvert \Bigg\lvert
-            k_{yz}(x, y, z)
-            \Bigg\rvert_{X_1}^{X_2}
-            \Bigg\rvert_{Y_1}^{Y_2}
-            \Bigg\rvert_{Z_1}^{Z_2}
+        k_{yz}(x, y, z) = \operatorname{safe-ln} \left( x + r \right)
 
     where
 
     .. math::
 
-        k_{yz}(x, y, z) = \text{ln2} \left( x + r \right),
-
-    .. math::
-
-        r = \sqrt{x^2 + y^2 + z^2},
+        \operatorname{safe-ln}(x) =
+        \begin{cases}
+            0 & |x| < 10^{-10} \\
+            \ln (x)
+        \end{cases}
 
-    and
+    References
+    ----------
+    - [Nagy2000]_
+    - [Nagy2002]_
+    - [Fukushima2020]_
+    """
+    return _safe_log(easting, radius)
 
-    .. math::
 
-        X_1 = x_1 - x_p \\
-        X_2 = x_2 - x_p \\
-        Y_1 = y_1 - y_p \\
-        Y_2 = y_2 - y_p \\
-        Z_1 = z_1 - z_p \\
-        Z_2 = z_2 - z_p
+@jit(nopython=True)
+def _safe_atan2(y, x):
+    r"""
+    Principal value of the arctangent expressed as a two variable function
 
-    are the shifted coordinates of the prism boundaries and :math:`G` is the
-    Universal Gravitational Constant.
+    This modification has to be made to the arctangent function so the
+    gravitational field of the prism satisfies the Poisson's equation.
+    Therefore, it guarantees that the fields satisfies the symmetry properties
+    of the prism. This modified function has been defined according to
+    [Fukushima2020]_.
 
-    The :math:`\text{ln2}` function is defined as follows:
+    Notes
+    -----
 
     .. math::
 
-        \text{ln2}(x) =
+        \operatorname{safe-arctan} \left(y, x\right) =
         \begin{cases}
-            0 & |x| < 10^{-10} \\
-            \ln (x)
+            \text{arctan}\left( \frac{y}{x} \right) & x \ne 0 \\
+            \frac{\pi}{2} & x = 0 \quad \text{and} \quad y > 0 \\
+            -\frac{\pi}{2} & x = 0 \quad \text{and} \quad y < 0 \\
+            0 & x = 0 \quad \text{and} \quad y = 0 \\
         \end{cases}
 
-    It was defined after [Fukushima2020]_ and guarantee a good accuracy on any
-    observation point.
-
     References
     ----------
-    - [Nagy2000]_
-    - [Nagy2002]_
     - [Fukushima2020]_
     """
-    return (
-        GRAVITATIONAL_CONST
-        * density
-        * _evaluate_kernel(easting, northing, upward, prism, kernel_nu)
-    )
+    if x == 0:
+        if y > 0:
+            result = np.pi / 2
+        elif y < 0:
+            result = -np.pi / 2
+        else:
+            result = 0
+        return result
+    return np.arctan(y / x)
 
 
 @jit(nopython=True)
-def _evaluate_kernel(easting, northing, upward, prism, kernel):
+def _safe_log(x, r):
     r"""
-    Evaluate a kernel function on every shifted vertex of a prism
+    Safe log function to use in the prism kernels
 
-    Parameters
-    ----------
-    easting : float
-        Easting coordinate of the observation point. Must be in meters.
-    northing : float
-        Northing coordinate of the observation point. Must be in meters.
-    upward : float
-        Upward coordinate of the observation point. Must be in meters.
-    prism : 1d-array
-        One dimensional array containing the coordinates of the prism in the
-        following order: ``west``, ``east``, ``south``, ``north``, ``bottom``,
-        ``top`` in a Cartesian coordinate system.
-        All coordinates should be in meters.
-    kernel : callable
-        Kernel function that will be evaluated on each one of the shifted
-        vertices of the prism.
-
-    Returns
-    -------
-    result : float
-        Evaluation of the kernel function on each one of the vertices of the
-        prism.
-
-    Notes
-    -----
-    This function evaluates a numerical kernel :math:`k(x, y, z)` on each one
-    of the vertices of the prism:
+    Evaluates the :math:`\ln{x + r}` where :math:`x` is one of the shifted
+    coordinate of the prism vertex and :math:`r` is the Euclidean distance
+    (always non-negative) from the vertex to the observation point.
 
     .. math::
 
-        v(\mathbf{p}) =
-            \Bigg\lvert \Bigg\lvert \Bigg\lvert
-            k(x, y, z)
-            \Bigg\rvert_{X_1}^{X_2}
-            \Bigg\rvert_{Y_1}^{Y_2}
-            \Bigg\rvert_{Z_1}^{Z_2}
-
-    where :math:`X_1`, :math:`X_2`, :math:`Y_1`, :math:`Y_2`, :math:`Z_1` and
-    :math:`Z_2` are boundaries of the rectangular prism in the *shifted
-    coordinates* defined by the Cartesian coordinate system with its origin
-    located on the observation point :math:`\mathbf{p}`.
+        \text{safe_ln}(x, r) =
+        \begin{cases}
+            0 & x = 0, r = 0 \\
+            \ln(x + r) & x \ge 0 \\
+            \ln((r^2 - x^2) / (r - x)) & x < 0, r \ne -x \\
+            -\ln(-2 x) & x < 0, r = -x
+        \end{cases}
+
+    This function returns 0 when the observation point is located on the vertex
+    of the prism (:math:`r=0`); and two modified versions in case that
+    :math:`x` is negative: if :math:`x = -r` then the :math:`\ln{x + r}` can be
+    replaced by :math:`-\ln{|x| + r} = -\ln(-2x)`, and for any other negative
+    value of :math:`x` it returns :math:`\ln((r^2 - x^2) / (r - x))` which
+    helps by reducing the floating point errors ([Fukushima2020_]).
+    This modified version was inspired by [Nagy2000] and [Fukushima2020_]:
 
     References
     ----------
-    - [Nagy2000]_
-    - [Nagy2002]_
+    - [Fukushima2020]_
     """
-    # Initialize result float to zero
-    result = 0
-    # Iterate over the vertices of the prism
-    for i in range(2):
-        # Compute shifted easting coordinate
-        shift_east = prism[1 - i] - easting
-        shift_east_sq = shift_east**2
-        for j in range(2):
-            # Compute shifted northing coordinate
-            shift_north = prism[3 - j] - northing
-            shift_north_sq = shift_north**2
-            for k in range(2):
-                # Compute shifted upward coordinate
-                shift_upward = prism[5 - k] - upward
-                shift_upward_sq = shift_upward**2
-                # Compute the radius
-                radius = np.sqrt(shift_east_sq + shift_north_sq + shift_upward_sq)
-                # If i, j or k is 1, the corresponding shifted
-                # coordinate will refer to the lower boundary,
-                # meaning the corresponding term should have a minus
-                # sign.
-                result += (-1) ** (i + j + k) * kernel(
-                    shift_east, shift_north, shift_upward, radius
-                )
-    return result
+    if r == 0:
+        return 0
+    if x < 0:
+        if r == -x:
+            result = -np.log(-2 * x)
+        else:
+            result = np.log((r**2 - x**2) / (r - x))
+        return result
+    return np.log(x + r)
```

### Comparing `choclo-0.0.1/choclo/tests/test_dipole.py` & `choclo-0.1.0/choclo/tests/test_dipole.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 # Copyright (c) 2022 The Choclo Developers.
 # Distributed under the terms of the BSD 3-Clause License.
 # SPDX-License-Identifier: BSD-3-Clause
 #
 # This code is part of the Fatiando a Terra project (https://www.fatiando.org)
 #
-# Copyright (c) 2022 The Choclo Developers-.
-# Distributed under the terms of the BSD 3-Clause License.
-# SPDX-License-Identifier: BSD-3-Clause
-#
-# This code is part of the Fatiando a Terra project (https://www.fatiando.org)
-#
 """
 Test magnetic forward modelling functions for a dipole
 """
 import numpy as np
 import numpy.testing as npt
 import pytest
 
@@ -94,23 +88,23 @@
         upward_top = upward[is_top]
         # Create a symmetrical upward coordinate for points below the dipole
         upward_bottom = 2 * sample_dipole[2] - upward_top
         # Compute magnetic_e on every observation point
         magnetic_moment = np.array(magnetic_moment)
         b_e_top = np.array(
             list(
-                magnetic_e(e, n, u, *sample_dipole, magnetic_moment)
+                magnetic_e(e, n, u, *sample_dipole, *magnetic_moment)
                 for e, n, u in zip(
                     easting.ravel(), northing.ravel(), upward_top.ravel()
                 )
             )
         )
         b_e_bottom = np.array(
             list(
-                magnetic_e(e, n, u, *sample_dipole, magnetic_moment)
+                magnetic_e(e, n, u, *sample_dipole, *magnetic_moment)
                 for e, n, u in zip(
                     easting.ravel(), northing.ravel(), upward_bottom.ravel()
                 )
             )
         )
         # Check symmetry between top and bottom
         if magnetic_moment[2] != 0:
@@ -144,23 +138,23 @@
         upward = upward[is_north]
         # Create a symmetrical upward coordinate for points south the dipole
         northing_south = 2 * sample_dipole[1] - northing_north
         # Compute magnetic_e on every observation point
         magnetic_moment = np.array(magnetic_moment)
         b_e_north = np.array(
             list(
-                magnetic_e(e, n, u, *sample_dipole, magnetic_moment)
+                magnetic_e(e, n, u, *sample_dipole, *magnetic_moment)
                 for e, n, u in zip(
                     easting.ravel(), northing_north.ravel(), upward.ravel()
                 )
             )
         )
         b_e_south = np.array(
             list(
-                magnetic_e(e, n, u, *sample_dipole, magnetic_moment)
+                magnetic_e(e, n, u, *sample_dipole, *magnetic_moment)
                 for e, n, u in zip(
                     easting.ravel(), northing_south.ravel(), upward.ravel()
                 )
             )
         )
         # Check symmetry between south and north
         if magnetic_moment[1] != 0:
@@ -194,23 +188,23 @@
         upward = upward[is_east]
         # Create a symmetrical upward coordinate for points west the dipole
         easting_west = 2 * sample_dipole[0] - easting_east
         # Compute magnetic_e on every observation point
         magnetic_moment = np.array(magnetic_moment)
         b_e_east = np.array(
             list(
-                magnetic_e(e, n, u, *sample_dipole, magnetic_moment)
+                magnetic_e(e, n, u, *sample_dipole, *magnetic_moment)
                 for e, n, u in zip(
                     easting_east.ravel(), northing.ravel(), upward.ravel()
                 )
             )
         )
         b_e_west = np.array(
             list(
-                magnetic_e(e, n, u, *sample_dipole, magnetic_moment)
+                magnetic_e(e, n, u, *sample_dipole, *magnetic_moment)
                 for e, n, u in zip(
                     easting_west.ravel(), northing.ravel(), upward.ravel()
                 )
             )
         )
         # Check symmetry between west and east
         if magnetic_moment[0] != 0:
@@ -231,21 +225,21 @@
         # Define two magnetic moments
         magnetic_moment_east = np.array([500.0, 0, 0])
         magnetic_moment_west = np.array([-500.0, 0, 0])
         # Compute the magnetic field generated by each moment on the
         # observation points
         b_e_east = np.array(
             list(
-                magnetic_e(e, n, u, *sample_dipole, magnetic_moment_east)
+                magnetic_e(e, n, u, *sample_dipole, *magnetic_moment_east)
                 for e, n, u in zip(easting, northing, upward)
             )
         )
         b_e_west = np.array(
             list(
-                magnetic_e(e, n, u, *sample_dipole, magnetic_moment_west)
+                magnetic_e(e, n, u, *sample_dipole, *magnetic_moment_west)
                 for e, n, u in zip(easting, northing, upward)
             )
         )
         # Check if the sign gets inverted
         npt.assert_allclose(b_e_east, -b_e_west)
 
 
@@ -282,23 +276,23 @@
         upward_top = upward[is_top]
         # Create a symmetrical upward coordinate for points below the dipole
         upward_bottom = 2 * sample_dipole[2] - upward_top
         # Compute magnetic_n on every observation point
         magnetic_moment = np.array(magnetic_moment)
         b_n_top = np.array(
             list(
-                magnetic_n(e, n, u, *sample_dipole, magnetic_moment)
+                magnetic_n(e, n, u, *sample_dipole, *magnetic_moment)
                 for e, n, u in zip(
                     easting.ravel(), northing.ravel(), upward_top.ravel()
                 )
             )
         )
         b_n_bottom = np.array(
             list(
-                magnetic_n(e, n, u, *sample_dipole, magnetic_moment)
+                magnetic_n(e, n, u, *sample_dipole, *magnetic_moment)
                 for e, n, u in zip(
                     easting.ravel(), northing.ravel(), upward_bottom.ravel()
                 )
             )
         )
         # Check symmetry between top and bottom
         if magnetic_moment[2] != 0:
@@ -332,23 +326,23 @@
         upward = upward[is_north]
         # Create a symmetrical upward coordinate for points south the dipole
         northing_south = 2 * sample_dipole[1] - northing_north
         # Compute magnetic_n on every observation point
         magnetic_moment = np.array(magnetic_moment)
         b_n_north = np.array(
             list(
-                magnetic_n(e, n, u, *sample_dipole, magnetic_moment)
+                magnetic_n(e, n, u, *sample_dipole, *magnetic_moment)
                 for e, n, u in zip(
                     easting.ravel(), northing_north.ravel(), upward.ravel()
                 )
             )
         )
         b_n_south = np.array(
             list(
-                magnetic_n(e, n, u, *sample_dipole, magnetic_moment)
+                magnetic_n(e, n, u, *sample_dipole, *magnetic_moment)
                 for e, n, u in zip(
                     easting.ravel(), northing_south.ravel(), upward.ravel()
                 )
             )
         )
         # Check symmetry between south and north
         if magnetic_moment[1] != 0:
@@ -382,23 +376,23 @@
         upward = upward[is_east]
         # Create a symmetrical upward coordinate for points west the dipole
         easting_west = 2 * sample_dipole[0] - easting_east
         # Compute magnetic_n on every observation point
         magnetic_moment = np.array(magnetic_moment)
         b_n_east = np.array(
             list(
-                magnetic_n(e, n, u, *sample_dipole, magnetic_moment)
+                magnetic_n(e, n, u, *sample_dipole, *magnetic_moment)
                 for e, n, u in zip(
                     easting_east.ravel(), northing.ravel(), upward.ravel()
                 )
             )
         )
         b_n_west = np.array(
             list(
-                magnetic_n(e, n, u, *sample_dipole, magnetic_moment)
+                magnetic_n(e, n, u, *sample_dipole, *magnetic_moment)
                 for e, n, u in zip(
                     easting_west.ravel(), northing.ravel(), upward.ravel()
                 )
             )
         )
         # Check symmetry between west and east
         if magnetic_moment[0] != 0:
@@ -419,21 +413,21 @@
         # Define two magnetic moments
         magnetic_moment_north = np.array([0, 500.0, 0])
         magnetic_moment_south = np.array([0, -500.0, 0])
         # Compute the magnetic field generated by each moment on the
         # observation points
         b_n_north = np.array(
             list(
-                magnetic_n(e, n, u, *sample_dipole, magnetic_moment_north)
+                magnetic_n(e, n, u, *sample_dipole, *magnetic_moment_north)
                 for e, n, u in zip(easting, northing, upward)
             )
         )
         b_n_south = np.array(
             list(
-                magnetic_n(e, n, u, *sample_dipole, magnetic_moment_south)
+                magnetic_n(e, n, u, *sample_dipole, *magnetic_moment_south)
                 for e, n, u in zip(easting, northing, upward)
             )
         )
         # Check if the sign gets inverted
         npt.assert_allclose(b_n_north, -b_n_south)
 
 
@@ -470,23 +464,23 @@
         upward_top = upward[is_top]
         # Create a symmetrical upward coordinate for points below the dipole
         upward_bottom = 2 * sample_dipole[2] - upward_top
         # Compute magnetic_u on every observation point
         magnetic_moment = np.array(magnetic_moment)
         b_u_top = np.array(
             list(
-                magnetic_u(e, n, u, *sample_dipole, magnetic_moment)
+                magnetic_u(e, n, u, *sample_dipole, *magnetic_moment)
                 for e, n, u in zip(
                     easting.ravel(), northing.ravel(), upward_top.ravel()
                 )
             )
         )
         b_u_bottom = np.array(
             list(
-                magnetic_u(e, n, u, *sample_dipole, magnetic_moment)
+                magnetic_u(e, n, u, *sample_dipole, *magnetic_moment)
                 for e, n, u in zip(
                     easting.ravel(), northing.ravel(), upward_bottom.ravel()
                 )
             )
         )
         # Check symmetry between top and bottom
         if magnetic_moment[2] != 0:
@@ -520,23 +514,23 @@
         upward = upward[is_north]
         # Create a symmetrical upward coordinate for points south the dipole
         northing_south = 2 * sample_dipole[1] - northing_north
         # Compute magnetic_u on every observation point
         magnetic_moment = np.array(magnetic_moment)
         b_u_north = np.array(
             list(
-                magnetic_u(e, n, u, *sample_dipole, magnetic_moment)
+                magnetic_u(e, n, u, *sample_dipole, *magnetic_moment)
                 for e, n, u in zip(
                     easting.ravel(), northing_north.ravel(), upward.ravel()
                 )
             )
         )
         b_u_south = np.array(
             list(
-                magnetic_u(e, n, u, *sample_dipole, magnetic_moment)
+                magnetic_u(e, n, u, *sample_dipole, *magnetic_moment)
                 for e, n, u in zip(
                     easting.ravel(), northing_south.ravel(), upward.ravel()
                 )
             )
         )
         # Check symmetry between south and north
         if magnetic_moment[1] != 0:
@@ -570,23 +564,23 @@
         upward = upward[is_east]
         # Create a symmetrical upward coordinate for points west the dipole
         easting_west = 2 * sample_dipole[0] - easting_east
         # Compute magnetic_u on every observation point
         magnetic_moment = np.array(magnetic_moment)
         b_u_east = np.array(
             list(
-                magnetic_u(e, n, u, *sample_dipole, magnetic_moment)
+                magnetic_u(e, n, u, *sample_dipole, *magnetic_moment)
                 for e, n, u in zip(
                     easting_east.ravel(), northing.ravel(), upward.ravel()
                 )
             )
         )
         b_u_west = np.array(
             list(
-                magnetic_u(e, n, u, *sample_dipole, magnetic_moment)
+                magnetic_u(e, n, u, *sample_dipole, *magnetic_moment)
                 for e, n, u in zip(
                     easting_west.ravel(), northing.ravel(), upward.ravel()
                 )
             )
         )
         # Check symmetry between east and west
         if magnetic_moment[0] != 0:
@@ -607,21 +601,21 @@
         # Define two magnetic moments
         magnetic_moment_up = np.array([0, 0, 500.0])
         magnetic_moment_down = np.array([0, 0, -500.0])
         # Compute the magnetic field generated by each moment on the
         # observation points
         b_u_up = np.array(
             list(
-                magnetic_u(e, n, u, *sample_dipole, magnetic_moment_up)
+                magnetic_u(e, n, u, *sample_dipole, *magnetic_moment_up)
                 for e, n, u in zip(easting, northing, upward)
             )
         )
         b_u_down = np.array(
             list(
-                magnetic_u(e, n, u, *sample_dipole, magnetic_moment_down)
+                magnetic_u(e, n, u, *sample_dipole, *magnetic_moment_down)
                 for e, n, u in zip(easting, northing, upward)
             )
         )
         # Check if the sign gets inverted
         npt.assert_allclose(b_u_up, -b_u_down)
 
 
@@ -639,35 +633,35 @@
     ):
         """
         Test magnetic_field against each one of the other functions
         """
         # Compute all components of B using magnetic_field
         b = np.array(
             list(
-                magnetic_field(e, n, u, *sample_dipole, sample_magnetic_moment)
+                magnetic_field(e, n, u, *sample_dipole, *sample_magnetic_moment)
                 for e, n, u in zip(*sample_3d_grid)
             )
         )
         b_e, b_n, b_u = tuple(b[:, i] for i in range(3))
         # Computed the individual fields
         b_e_expected = np.array(
             list(
-                magnetic_e(e, n, u, *sample_dipole, sample_magnetic_moment)
+                magnetic_e(e, n, u, *sample_dipole, *sample_magnetic_moment)
                 for e, n, u in zip(*sample_3d_grid)
             )
         )
         b_n_expected = np.array(
             list(
-                magnetic_n(e, n, u, *sample_dipole, sample_magnetic_moment)
+                magnetic_n(e, n, u, *sample_dipole, *sample_magnetic_moment)
                 for e, n, u in zip(*sample_3d_grid)
             )
         )
         b_u_expected = np.array(
             list(
-                magnetic_u(e, n, u, *sample_dipole, sample_magnetic_moment)
+                magnetic_u(e, n, u, *sample_dipole, *sample_magnetic_moment)
                 for e, n, u in zip(*sample_3d_grid)
             )
         )
         npt.assert_allclose(b_e, b_e_expected)
         npt.assert_allclose(b_n, b_n_expected)
         npt.assert_allclose(b_u, b_u_expected)
 
@@ -689,21 +683,21 @@
         # Get original coordinates
         easting, northing, upward = coordinates
         # Shift coordinates using delta
         easting_shifted = easting + self.delta
         # Compute b_e on original and shifted coordinates
         b_e = np.array(
             list(
-                magnetic_e(e, n, u, *dipole, magnetic_moment)
+                magnetic_e(e, n, u, *dipole, *magnetic_moment)
                 for e, n, u in zip(easting, northing, upward)
             )
         )
         b_e_shifted = np.array(
             list(
-                magnetic_e(e, n, u, *dipole, magnetic_moment)
+                magnetic_e(e, n, u, *dipole, *magnetic_moment)
                 for e, n, u in zip(easting_shifted, northing, upward)
             )
         )
         # Compute b_ee
         b_ee = (b_e_shifted - b_e) / self.delta
         return b_ee
 
@@ -714,21 +708,21 @@
         # Get original coordinates
         easting, northing, upward = coordinates
         # Shift coordinates using delta
         northing_shifted = northing + self.delta
         # Compute b_e on original and shifted coordinates
         b_n = np.array(
             list(
-                magnetic_n(e, n, u, *dipole, magnetic_moment)
+                magnetic_n(e, n, u, *dipole, *magnetic_moment)
                 for e, n, u in zip(easting, northing, upward)
             )
         )
         b_n_shifted = np.array(
             list(
-                magnetic_n(e, n, u, *dipole, magnetic_moment)
+                magnetic_n(e, n, u, *dipole, *magnetic_moment)
                 for e, n, u in zip(easting, northing_shifted, upward)
             )
         )
         # Compute b_nn
         b_nn = (b_n_shifted - b_n) / self.delta
         return b_nn
 
@@ -739,21 +733,21 @@
         # Get original coordinates
         easting, northing, upward = coordinates
         # Shift coordinates using delta
         upward_shifted = upward + self.delta
         # Compute b_e on original and shifted coordinates
         b_u = np.array(
             list(
-                magnetic_u(e, n, u, *dipole, magnetic_moment)
+                magnetic_u(e, n, u, *dipole, *magnetic_moment)
                 for e, n, u in zip(easting, northing, upward)
             )
         )
         b_u_shifted = np.array(
             list(
-                magnetic_u(e, n, u, *dipole, magnetic_moment)
+                magnetic_u(e, n, u, *dipole, *magnetic_moment)
                 for e, n, u in zip(easting, northing, upward_shifted)
             )
         )
         # Compute b_uu
         b_uu = (b_u_shifted - b_u) / self.delta
         return b_uu
```

### Comparing `choclo-0.0.1/choclo/tests/test_distance.py` & `choclo-0.1.0/choclo/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `choclo-0.0.1/choclo/tests/test_point_gravity.py` & `choclo-0.1.0/choclo/tests/test_point_gravity.py`

 * *Files identical despite different names*

### Comparing `choclo-0.0.1/choclo/tests/test_prism_magnetic.py` & `choclo-0.1.0/choclo/tests/test_prism_magnetic.py`

 * *Files 14% similar despite different names*

```diff
@@ -103,23 +103,23 @@
         # Create a symmetrical upward coordinate for points below the prism
         # center
         upward_bottom = 2 * prism_center_u - upward_top
         # Compute magnetic_e on every observation point
         magnetization = np.array(magnetization)
         b_e_top = np.array(
             list(
-                magnetic_e(e, n, u, sample_prism, magnetization)
+                magnetic_e(e, n, u, *sample_prism, *magnetization)
                 for e, n, u in zip(
                     easting.ravel(), northing.ravel(), upward_top.ravel()
                 )
             )
         )
         b_e_bottom = np.array(
             list(
-                magnetic_e(e, n, u, sample_prism, magnetization)
+                magnetic_e(e, n, u, *sample_prism, *magnetization)
                 for e, n, u in zip(
                     easting.ravel(), northing.ravel(), upward_bottom.ravel()
                 )
             )
         )
         # Check symmetry between top and bottom
         if magnetization[2] != 0:
@@ -155,23 +155,23 @@
         # Create a symmetrical upward coordinate for points south the prism
         # center
         northing_south = 2 * prism_center_n - northing_north
         # Compute magnetic_e on every observation point
         magnetization = np.array(magnetization)
         b_e_north = np.array(
             list(
-                magnetic_e(e, n, u, sample_prism, magnetization)
+                magnetic_e(e, n, u, *sample_prism, *magnetization)
                 for e, n, u in zip(
                     easting.ravel(), northing_north.ravel(), upward.ravel()
                 )
             )
         )
         b_e_south = np.array(
             list(
-                magnetic_e(e, n, u, sample_prism, magnetization)
+                magnetic_e(e, n, u, *sample_prism, *magnetization)
                 for e, n, u in zip(
                     easting.ravel(), northing_south.ravel(), upward.ravel()
                 )
             )
         )
         # Check symmetry between south and north
         if magnetization[1] != 0:
@@ -207,23 +207,23 @@
         # Create a symmetrical upward coordinate for points west the prism
         # center
         easting_west = 2 * prism_center_e - easting_east
         # Compute magnetic_e on every observation point
         magnetization = np.array(magnetization)
         b_e_east = np.array(
             list(
-                magnetic_e(e, n, u, sample_prism, magnetization)
+                magnetic_e(e, n, u, *sample_prism, *magnetization)
                 for e, n, u in zip(
                     easting_east.ravel(), northing.ravel(), upward.ravel()
                 )
             )
         )
         b_e_west = np.array(
             list(
-                magnetic_e(e, n, u, sample_prism, magnetization)
+                magnetic_e(e, n, u, *sample_prism, *magnetization)
                 for e, n, u in zip(
                     easting_west.ravel(), northing.ravel(), upward.ravel()
                 )
             )
         )
         # Check symmetry between west and east
         if magnetization[0] != 0:
@@ -245,21 +245,21 @@
         # Define two magnetic moments
         magnetization_east = np.array([500.0, 0, 0])
         magnetization_west = np.array([-500.0, 0, 0])
         # Compute the magnetic field generated by each moment on the
         # observation points
         b_e_east = np.array(
             list(
-                magnetic_e(e, n, u, sample_prism, magnetization_east)
+                magnetic_e(e, n, u, *sample_prism, *magnetization_east)
                 for e, n, u in zip(easting, northing, upward)
             )
         )
         b_e_west = np.array(
             list(
-                magnetic_e(e, n, u, sample_prism, magnetization_west)
+                magnetic_e(e, n, u, *sample_prism, *magnetization_west)
                 for e, n, u in zip(easting, northing, upward)
             )
         )
         # Check if the sign gets inverted
         npt.assert_allclose(b_e_east, -b_e_west)
 
 
@@ -298,23 +298,23 @@
         # Create a symmetrical upward coordinate for points below the prism
         # center
         upward_bottom = 2 * prism_center_u - upward_top
         # Compute magnetic_n on every observation point
         magnetization = np.array(magnetization)
         b_n_top = np.array(
             list(
-                magnetic_n(e, n, u, sample_prism, magnetization)
+                magnetic_n(e, n, u, *sample_prism, *magnetization)
                 for e, n, u in zip(
                     easting.ravel(), northing.ravel(), upward_top.ravel()
                 )
             )
         )
         b_n_bottom = np.array(
             list(
-                magnetic_n(e, n, u, sample_prism, magnetization)
+                magnetic_n(e, n, u, *sample_prism, *magnetization)
                 for e, n, u in zip(
                     easting.ravel(), northing.ravel(), upward_bottom.ravel()
                 )
             )
         )
         # Check symmetry between top and bottom
         if magnetization[2] != 0:
@@ -350,23 +350,23 @@
         # Create a symmetrical upward coordinate for points south the prism
         # center
         northing_south = 2 * prism_center_n - northing_north
         # Compute magnetic_n on every observation point
         magnetization = np.array(magnetization)
         b_n_north = np.array(
             list(
-                magnetic_n(e, n, u, sample_prism, magnetization)
+                magnetic_n(e, n, u, *sample_prism, *magnetization)
                 for e, n, u in zip(
                     easting.ravel(), northing_north.ravel(), upward.ravel()
                 )
             )
         )
         b_n_south = np.array(
             list(
-                magnetic_n(e, n, u, sample_prism, magnetization)
+                magnetic_n(e, n, u, *sample_prism, *magnetization)
                 for e, n, u in zip(
                     easting.ravel(), northing_south.ravel(), upward.ravel()
                 )
             )
         )
         # Check symmetry between south and north
         if magnetization[1] != 0:
@@ -402,23 +402,23 @@
         # Create a symmetrical upward coordinate for points west the prism
         # center
         easting_west = 2 * prism_center_e - easting_east
         # Compute magnetic_n on every observation point
         magnetization = np.array(magnetization)
         b_n_east = np.array(
             list(
-                magnetic_n(e, n, u, sample_prism, magnetization)
+                magnetic_n(e, n, u, *sample_prism, *magnetization)
                 for e, n, u in zip(
                     easting_east.ravel(), northing.ravel(), upward.ravel()
                 )
             )
         )
         b_n_west = np.array(
             list(
-                magnetic_n(e, n, u, sample_prism, magnetization)
+                magnetic_n(e, n, u, *sample_prism, *magnetization)
                 for e, n, u in zip(
                     easting_west.ravel(), northing.ravel(), upward.ravel()
                 )
             )
         )
         # Check symmetry between west and east
         if magnetization[0] != 0:
@@ -440,21 +440,21 @@
         # Define two magnetic moments
         magnetization_north = np.array([0, 500.0, 0])
         magnetization_south = np.array([0, -500.0, 0])
         # Compute the magnetic field generated by each moment on the
         # observation points
         b_n_north = np.array(
             list(
-                magnetic_n(e, n, u, sample_prism, magnetization_north)
+                magnetic_n(e, n, u, *sample_prism, *magnetization_north)
                 for e, n, u in zip(easting, northing, upward)
             )
         )
         b_n_south = np.array(
             list(
-                magnetic_n(e, n, u, sample_prism, magnetization_south)
+                magnetic_n(e, n, u, *sample_prism, *magnetization_south)
                 for e, n, u in zip(easting, northing, upward)
             )
         )
         # Check if the sign gets inverted
         npt.assert_allclose(b_n_north, -b_n_south)
 
 
@@ -493,23 +493,23 @@
         # Create a symmetrical upward coordinate for points below the prism
         # center
         upward_bottom = 2 * prism_center_u - upward_top
         # Compute magnetic_u on every observation point
         magnetization = np.array(magnetization)
         b_u_top = np.array(
             list(
-                magnetic_u(e, n, u, sample_prism, magnetization)
+                magnetic_u(e, n, u, *sample_prism, *magnetization)
                 for e, n, u in zip(
                     easting.ravel(), northing.ravel(), upward_top.ravel()
                 )
             )
         )
         b_u_bottom = np.array(
             list(
-                magnetic_u(e, n, u, sample_prism, magnetization)
+                magnetic_u(e, n, u, *sample_prism, *magnetization)
                 for e, n, u in zip(
                     easting.ravel(), northing.ravel(), upward_bottom.ravel()
                 )
             )
         )
         # Check symmetry between top and bottom
         if magnetization[2] != 0:
@@ -545,23 +545,23 @@
         # Create a symmetrical upward coordinate for points south the prism
         # center
         northing_south = 2 * prism_center_n - northing_north
         # Compute magnetic_u on every observation point
         magnetization = np.array(magnetization)
         b_u_north = np.array(
             list(
-                magnetic_u(e, n, u, sample_prism, magnetization)
+                magnetic_u(e, n, u, *sample_prism, *magnetization)
                 for e, n, u in zip(
                     easting.ravel(), northing_north.ravel(), upward.ravel()
                 )
             )
         )
         b_u_south = np.array(
             list(
-                magnetic_u(e, n, u, sample_prism, magnetization)
+                magnetic_u(e, n, u, *sample_prism, *magnetization)
                 for e, n, u in zip(
                     easting.ravel(), northing_south.ravel(), upward.ravel()
                 )
             )
         )
         # Check symmetry between south and north
         if magnetization[1] != 0:
@@ -597,23 +597,23 @@
         # Create a symmetrical upward coordinate for points west the center of
         # the prism
         easting_west = 2 * prism_center_e - easting_east
         # Compute magnetic_u on every observation point
         magnetization = np.array(magnetization)
         b_u_east = np.array(
             list(
-                magnetic_u(e, n, u, sample_prism, magnetization)
+                magnetic_u(e, n, u, *sample_prism, *magnetization)
                 for e, n, u in zip(
                     easting_east.ravel(), northing.ravel(), upward.ravel()
                 )
             )
         )
         b_u_west = np.array(
             list(
-                magnetic_u(e, n, u, sample_prism, magnetization)
+                magnetic_u(e, n, u, *sample_prism, *magnetization)
                 for e, n, u in zip(
                     easting_west.ravel(), northing.ravel(), upward.ravel()
                 )
             )
         )
         # Check symmetry between east and west
         if magnetization[0] != 0:
@@ -635,21 +635,21 @@
         # Define two magnetic moments
         magnetization_up = np.array([0, 0, 500.0])
         magnetization_down = np.array([0, 0, -500.0])
         # Compute the magnetic field generated by each moment on the
         # observation points
         b_u_up = np.array(
             list(
-                magnetic_u(e, n, u, sample_prism, magnetization_up)
+                magnetic_u(e, n, u, *sample_prism, *magnetization_up)
                 for e, n, u in zip(easting, northing, upward)
             )
         )
         b_u_down = np.array(
             list(
-                magnetic_u(e, n, u, sample_prism, magnetization_down)
+                magnetic_u(e, n, u, *sample_prism, *magnetization_down)
                 for e, n, u in zip(easting, northing, upward)
             )
         )
         # Check if the sign gets inverted
         npt.assert_allclose(b_u_up, -b_u_down)
 
 
@@ -665,35 +665,35 @@
     def test_magnetic_field(self, sample_3d_grid, sample_prism, sample_magnetization):
         """
         Test magnetic_field against each one of the other functions
         """
         # Compute all components of B using magnetic_field
         b = np.array(
             list(
-                magnetic_field(e, n, u, sample_prism, sample_magnetization)
+                magnetic_field(e, n, u, *sample_prism, *sample_magnetization)
                 for e, n, u in zip(*sample_3d_grid)
             )
         )
         b_e, b_n, b_u = tuple(b[:, i] for i in range(3))
         # Computed the individual fields
         b_e_expected = np.array(
             list(
-                magnetic_e(e, n, u, sample_prism, sample_magnetization)
+                magnetic_e(e, n, u, *sample_prism, *sample_magnetization)
                 for e, n, u in zip(*sample_3d_grid)
             )
         )
         b_n_expected = np.array(
             list(
-                magnetic_n(e, n, u, sample_prism, sample_magnetization)
+                magnetic_n(e, n, u, *sample_prism, *sample_magnetization)
                 for e, n, u in zip(*sample_3d_grid)
             )
         )
         b_u_expected = np.array(
             list(
-                magnetic_u(e, n, u, sample_prism, sample_magnetization)
+                magnetic_u(e, n, u, *sample_prism, *sample_magnetization)
                 for e, n, u in zip(*sample_3d_grid)
             )
         )
         npt.assert_allclose(b_e, b_e_expected)
         npt.assert_allclose(b_n, b_n_expected)
         npt.assert_allclose(b_u, b_u_expected)
 
@@ -715,21 +715,21 @@
         # Get original coordinates
         easting, northing, upward = coordinates
         # Shift coordinates using delta
         easting_shifted = easting + self.delta
         # Compute b_e on original and shifted coordinates
         b_e = np.array(
             list(
-                magnetic_e(e, n, u, prism, magnetization)
+                magnetic_e(e, n, u, *prism, *magnetization)
                 for e, n, u in zip(easting, northing, upward)
             )
         )
         b_e_shifted = np.array(
             list(
-                magnetic_e(e, n, u, prism, magnetization)
+                magnetic_e(e, n, u, *prism, *magnetization)
                 for e, n, u in zip(easting_shifted, northing, upward)
             )
         )
         # Compute b_ee
         b_ee = (b_e_shifted - b_e) / self.delta
         return b_ee
 
@@ -740,21 +740,21 @@
         # Get original coordinates
         easting, northing, upward = coordinates
         # Shift coordinates using delta
         northing_shifted = northing + self.delta
         # Compute b_e on original and shifted coordinates
         b_n = np.array(
             list(
-                magnetic_n(e, n, u, prism, magnetization)
+                magnetic_n(e, n, u, *prism, *magnetization)
                 for e, n, u in zip(easting, northing, upward)
             )
         )
         b_n_shifted = np.array(
             list(
-                magnetic_n(e, n, u, prism, magnetization)
+                magnetic_n(e, n, u, *prism, *magnetization)
                 for e, n, u in zip(easting, northing_shifted, upward)
             )
         )
         # Compute b_nn
         b_nn = (b_n_shifted - b_n) / self.delta
         return b_nn
 
@@ -765,21 +765,21 @@
         # Get original coordinates
         easting, northing, upward = coordinates
         # Shift coordinates using delta
         upward_shifted = upward + self.delta
         # Compute b_e on original and shifted coordinates
         b_u = np.array(
             list(
-                magnetic_u(e, n, u, prism, magnetization)
+                magnetic_u(e, n, u, *prism, *magnetization)
                 for e, n, u in zip(easting, northing, upward)
             )
         )
         b_u_shifted = np.array(
             list(
-                magnetic_u(e, n, u, prism, magnetization)
+                magnetic_u(e, n, u, *prism, *magnetization)
                 for e, n, u in zip(easting, northing, upward_shifted)
             )
         )
         # Compute b_uu
         b_uu = (b_u_shifted - b_u) / self.delta
         return b_uu
 
@@ -792,7 +792,176 @@
             sample_3d_grid, sample_prism, sample_magnetization
         )
         b_uu = self.get_b_uu_finite_differences(
             sample_3d_grid, sample_prism, sample_magnetization
         )
         # Check if the divergence of B is zero
         npt.assert_allclose(-b_uu, b_ee + b_nn, atol=1e-11)
+
+
+class TestMagneticFieldSingularities:
+    """
+    Test if magnetic field components behave as expected on their singular
+    points
+
+    Magnetic field components have singular points on:
+    * prism vertices,
+    * prism edges,
+    * prism interior, and
+    * prism faces normal to the magnetic component direction.
+
+    For the first three cases, the forward modelling function should return
+    ``np.nan``. For the last case, it should return the limit of the field when
+    we approach from outside of the prism.
+    """
+
+    @pytest.fixture()
+    def sample_prism(self):
+        """
+        Return the boundaries of the sample prism
+        """
+        west, east, south, north, bottom, top = -5.4, 10.1, 43.2, 79.5, -53.7, -44.3
+        return np.array([west, east, south, north, bottom, top])
+
+    def get_vertices(self, prism):
+        """
+        Return the vertices of the prism
+        """
+        coordinates = tuple(
+            a.ravel() for a in np.meshgrid(prism[0:2], prism[2:4], prism[4:6])
+        )
+        return coordinates
+
+    def get_easting_edges_center(self, prism):
+        """
+        Return points on the center of prism edges parallel to easting
+        """
+        easting_c = (prism[0] + prism[1]) / 2
+        northing, upward = tuple(c.ravel() for c in np.meshgrid(prism[2:4], prism[4:6]))
+        easting = np.full_like(northing, easting_c)
+        return easting, northing, upward
+
+    def get_northing_edges_center(self, prism):
+        """
+        Return points on the center of prism edges parallel to northing
+        """
+        northing_c = (prism[2] + prism[3]) / 2
+        easting, upward = tuple(c.ravel() for c in np.meshgrid(prism[0:2], prism[4:6]))
+        northing = np.full_like(easting, northing_c)
+        return easting, northing, upward
+
+    def get_upward_edges_center(self, prism):
+        """
+        Return points on the center of prism edges parallel to upward
+        """
+        upward_c = (prism[4] + prism[5]) / 2
+        easting, northing = tuple(
+            c.ravel() for c in np.meshgrid(prism[0:2], prism[2:4])
+        )
+        upward = np.full_like(easting, upward_c)
+        return easting, northing, upward
+
+    def get_faces_centers(self, prism, direction):
+        """
+        Return points on the center of faces normal to the given direction
+        """
+        if direction == "easting":
+            easting = prism[0:2]
+            northing = np.mean(prism[2:4])
+            upward = np.mean(prism[4:6])
+        elif direction == "northing":
+            easting = np.mean(prism[0:2])
+            northing = prism[2:4]
+            upward = np.mean(prism[4:6])
+        elif direction == "upward":
+            easting = np.mean(prism[0:2])
+            northing = np.mean(prism[2:4])
+            upward = prism[4:6]
+        coordinates = tuple(c.ravel() for c in np.meshgrid(easting, northing, upward))
+        return coordinates
+
+    def get_interior_points(self, prism):
+        """
+        Return a set of interior points
+        """
+        west, east, south, north, bottom, top = prism
+        easting = np.linspace(west, east, 5)[1:-1]
+        northing = np.linspace(south, north, 5)[1:-1]
+        upward = np.linspace(bottom, top, 5)[1:-1]
+        coordinates = tuple(c.ravel() for c in np.meshgrid(easting, northing, upward))
+        return coordinates
+
+    @pytest.mark.parametrize(
+        "forward_func", (magnetic_field, magnetic_e, magnetic_n, magnetic_u)
+    )
+    def test_on_vertices(self, sample_prism, forward_func):
+        """
+        Test if magnetic field components on vertices are equal to NaN
+        """
+        easting, northing, upward = self.get_vertices(sample_prism)
+        magnetization = np.array([1.0, 1.0, 1.0])
+        results = list(
+            forward_func(e, n, u, *sample_prism, *magnetization)
+            for (e, n, u) in zip(easting, northing, upward)
+        )
+        assert np.isnan(results).all()
+
+    @pytest.mark.parametrize(
+        "forward_func", (magnetic_field, magnetic_e, magnetic_n, magnetic_u)
+    )
+    @pytest.mark.parametrize("direction", ("easting", "northing", "upward"))
+    def test_on_edges(self, sample_prism, direction, forward_func):
+        """
+        Test if magnetic field components are NaN on edges of the prism
+        """
+        # Build observation points on edges
+        coordinates = getattr(self, f"get_{direction}_edges_center")(sample_prism)
+        easting, northing, upward = coordinates
+        magnetization = np.array([1.0, 1.0, 1.0])
+        results = list(
+            forward_func(e, n, u, *sample_prism, *magnetization)
+            for (e, n, u) in zip(easting, northing, upward)
+        )
+        assert np.isnan(results).all()
+
+    @pytest.mark.parametrize(
+        "forward_func", (magnetic_field, magnetic_e, magnetic_n, magnetic_u)
+    )
+    def test_on_interior_points(self, sample_prism, forward_func):
+        """
+        Test if magnetic field components are NaN on internal points
+        """
+        easting, northing, upward = self.get_interior_points(sample_prism)
+        magnetization = np.array([1.0, 1.0, 1.0])
+        results = list(
+            forward_func(e, n, u, *sample_prism, *magnetization)
+            for (e, n, u) in zip(easting, northing, upward)
+        )
+        assert np.isnan(results).all()
+
+    @pytest.mark.parametrize(
+        "forward_func", (magnetic_field, magnetic_e, magnetic_n, magnetic_u)
+    )
+    @pytest.mark.parametrize("direction", ("easting", "northing", "upward"))
+    def test_symmetry_on_faces(self, sample_prism, direction, forward_func):
+        """
+        Tests symmetry of magnetic field components on the center of faces
+        normal to the component direction
+
+        For example, check if ``magnetic_u`` has the same value on points in
+        the top face and points of the bottom face.
+        """
+        easting, northing, upward = self.get_faces_centers(sample_prism, direction)
+        magnetization = np.array([1.0, 1.0, 1.0])
+        if forward_func == magnetic_field:
+            component_mapping = {"easting": 0, "northing": 1, "upward": 2}
+            index = component_mapping[direction]
+            results = list(
+                forward_func(e, n, u, *sample_prism, *magnetization)[index]
+                for (e, n, u) in zip(easting, northing, upward)
+            )
+        else:
+            results = list(
+                forward_func(e, n, u, *sample_prism, *magnetization)
+                for (e, n, u) in zip(easting, northing, upward)
+            )
+        npt.assert_allclose(results, results[0])
```

### Comparing `choclo-0.0.1/choclo/tests/utils.py` & `choclo-0.1.0/choclo/tests/utils.py`

 * *Files identical despite different names*

### Comparing `choclo-0.0.1/choclo/utils.py` & `choclo-0.1.0/choclo/utils.py`

 * *Files identical despite different names*

### Comparing `choclo-0.0.1/choclo.egg-info/PKG-INFO` & `choclo-0.1.0/choclo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: choclo
-Version: 0.0.1
+Version: 0.1.0
 Summary: Kernel functions for your geophysical models
 Home-page: https://github.com/fatiando/choclo
 Author: The Choclo Developers
 Author-email: fatiandoaterra@protonmail.com
 Maintainer: Santiago Soler
 Maintainer-email: santiago.r.soler@gmail.com
 License: BSD 3-Clause License
@@ -20,24 +20,23 @@
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Choclo
+<img src="https://github.com/fatiando/choclo/raw/main/doc/_static/readme-banner.png" alt="Choclo">
 
 <h2 align="center">Kernel functions for your geophysical models</h2>
 
 <p align="center">
 <a href="https://www.fatiando.org/choclo"><strong>Documentation</strong> (latest)</a> •
 <a href="https://www.fatiando.org/choclo/dev"><strong>Documentation</strong> (main branch)</a> •
 <a href="https://github.com/fatiando/choclo/blob/main/CONTRIBUTING.md"><strong>Contributing</strong></a> •
@@ -49,14 +48,15 @@
 </p>
 
 <p align="center">
 <a href="https://pypi.python.org/pypi/choclo"><img src="http://img.shields.io/pypi/v/choclo.svg?style=flat-square" alt="Latest version on PyPI"></a>
 <a href="https://github.com/conda-forge/choclo-feedstock"><img src="https://img.shields.io/conda/vn/conda-forge/choclo.svg?style=flat-square" alt="Latest version on conda-forge"></a>
 <a href="https://codecov.io/gh/fatiando/choclo"><img src="https://img.shields.io/codecov/c/github/fatiando/choclo/main.svg?style=flat-square" alt="Test coverage status"></a>
 <a href="https://pypi.python.org/pypi/choclo"><img src="https://img.shields.io/pypi/pyversions/choclo.svg?style=flat-square" alt="Compatible Python versions."></a>
+<a href="https://doi.org/10.5281/zenodo.7851747"><img src="https://img.shields.io/badge/doi-10.5281%2Fzenodo.7851747-blue?style=flat-square" alt="DOI used to cite Choclo"></a>
 </p>
 
 ## About
 
 **Choclo** is a Python library that hosts optimized kernel functions for
 running geophysical forward and inverse models, intended to be used by other
 libraries as the underlying layer of their computation.
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1 Name: choclo Version: 0.0.1 Summary: Kernel functions for
+Metadata-Version: 2.1 Name: choclo Version: 0.1.0 Summary: Kernel functions for
 your geophysical models Home-page: https://github.com/fatiando/choclo Author:
 The Choclo Developers Author-email: fatiandoaterra@protonmail.com Maintainer:
 Santiago Soler Maintainer-email: santiago.r.soler@gmail.com License: BSD 3-
 Clause License Project-URL: Documentation, https://www.fatiando.org/choclo
 Project-URL: Release Notes, https://github.com/fatiando/choclo/releases
 Project-URL: Bug Tracker, https://github.com/fatiando/choclo/issues Project-
 URL: Source Code, https://github.com/fatiando/choclo Keywords:
 geophysics,geoscience Platform: any Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Education Classifier: License ::
 OSI Approved :: BSD License Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
-3.6 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE.txt # Choclo
+3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
+LICENSE.txt [Choclo]
            ***** Kernel functions for your geophysical models *****
   Documentation_(latest) â¢ Documentation_(main_branch) â¢ Contributing â¢
                                     Contact
                      Part of the Fatiando_a_Terra project
 [Latest_version_on_PyPI] [Latest_version_on_conda-forge] [Test_coverage_status]
-                         [Compatible_Python_versions.]
+            [Compatible_Python_versions.] [DOI_used_to_cite_Choclo]
 ## About **Choclo** is a Python library that hosts optimized kernel functions
 for running geophysical forward and inverse models, intended to be used by
 other libraries as the underlying layer of their computation. "Choclo" is a
 term used in some countries of South America to refer to corn, originated from
 the [quechua](https://en.wikipedia.org/wiki/Quechuan_languages) word _chuqllu_.
 ## Project goals * Provide optimized kernel functions for gravity and magnetic
 forward and inverse models that can be easily harnessed by different
```

### Comparing `choclo-0.0.1/choclo.egg-info/SOURCES.txt` & `choclo-0.1.0/choclo.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -16,20 +16,19 @@
 choclo.egg-info/requires.txt
 choclo.egg-info/top_level.txt
 choclo.egg-info/zip-safe
 choclo/dipole/__init__.py
 choclo/dipole/_forward.py
 choclo/point/__init__.py
 choclo/point/_forward.py
-choclo/point/_kernels.py
 choclo/prism/__init__.py
 choclo/prism/_gravity.py
 choclo/prism/_kernels.py
 choclo/prism/_magnetic.py
+choclo/prism/_utils.py
 choclo/tests/__init__.py
 choclo/tests/test_dipole.py
 choclo/tests/test_distance.py
 choclo/tests/test_point_gravity.py
-choclo/tests/test_point_kernels.py
 choclo/tests/test_prism_gravity.py
 choclo/tests/test_prism_magnetic.py
 choclo/tests/utils.py
```

### Comparing `choclo-0.0.1/setup.cfg` & `choclo-0.1.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -19,42 +19,43 @@
 	Intended Audience :: Education
 	License :: OSI Approved :: BSD License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Topic :: Scientific/Engineering
 	Topic :: Software Development :: Libraries
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 url = https://github.com/fatiando/choclo
 project_urls = 
 	Documentation = https://www.fatiando.org/choclo
 	Release Notes = https://github.com/fatiando/choclo/releases
 	Bug Tracker = https://github.com/fatiando/choclo/issues
 	Source Code = https://github.com/fatiando/choclo
 
 [options]
 zip_safe = True
 packages = find:
-python_requires = >=3.6
+python_requires = >=3.7
 install_requires = 
 	numpy>=1.19
 	numba>=0.52
 
 [flake8]
 max-line-length = 88
 max-doc-length = 79
 ignore = 
 	E266,
 	E501,
 	E741,
 	W503,
+	CFQ001,
+	CFQ002,
 exclude = 
 	.git,
 	__pycache__,
 	.ipynb_checkpoints,
 	doc/_build,
 per-file-ignores = 
 	__init__.py: F401
@@ -62,13 +63,12 @@
 rst-roles = 
 	class,
 	func,
 	mod,
 	meth,
 	ref,
 extend-ignore = RST306
-max-parameters-amount = 10
 
 [egg_info]
 tag_build = 
 tag_date = 0
```


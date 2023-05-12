# Comparing `tmp/lincs-0.3.1.tar.gz` & `tmp/lincs-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lincs-0.3.1.tar", last modified: Fri May 12 08:54:07 2023, max compression
+gzip compressed data, was "lincs-0.3.2.tar", last modified: Fri May 12 12:23:46 2023, max compression
```

## Comparing `lincs-0.3.1.tar` & `lincs-0.3.2.tar`

### file list

```diff
@@ -1,31 +1,60 @@
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 08:54:07.058991 lincs-0.3.1/
--rw-rw-r--   0 user      (1002) user      (1002)       70 2023-05-12 08:52:07.000000 lincs-0.3.1/MANIFEST.in
--rw-r--r--   0 user      (1002) user      (1002)    16795 2023-05-12 08:54:07.058991 lincs-0.3.1/PKG-INFO
--rw-rw-r--   0 user      (1002) user      (1002)    16088 2023-05-11 17:35:39.000000 lincs-0.3.1/README.md
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 08:54:07.058991 lincs-0.3.1/lincs/
--rw-rw-r--   0 user      (1002) user      (1002)      762 2023-05-11 16:48:08.000000 lincs-0.3.1/lincs/__init__.py
--rw-r--r--   0 user      (1002) user      (1002)      136 2023-05-04 08:59:02.000000 lincs-0.3.1/lincs/__main__.py
--rw-rw-r--   0 user      (1002) user      (1002)    21943 2023-05-11 17:15:21.000000 lincs-0.3.1/lincs/command_line_interface.py
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 08:54:07.058991 lincs-0.3.1/lincs/liblincs/
--rw-rw-r--   0 user      (1002) user      (1002)     1566 2023-05-12 08:51:21.000000 lincs-0.3.1/lincs/liblincs/classification.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     9942 2023-05-12 08:51:21.000000 lincs-0.3.1/lincs/liblincs/generation.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     6492 2023-05-12 08:51:21.000000 lincs-0.3.1/lincs/liblincs/io.cpp
--rw-rw-r--   0 user      (1002) user      (1002)    26434 2023-05-12 08:51:21.000000 lincs-0.3.1/lincs/liblincs/learning.cpp
--rw-rw-r--   0 user      (1002) user      (1002)    15089 2023-05-12 08:51:21.000000 lincs-0.3.1/lincs/liblincs/liblincs_module.cpp
--rw-rw-r--   0 user      (1002) user      (1002)    11471 2023-05-12 08:51:21.000000 lincs-0.3.1/lincs/liblincs/lincs.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     2928 2023-05-12 08:51:14.000000 lincs-0.3.1/lincs/liblincs/median-and-max.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      609 2023-05-12 08:51:14.000000 lincs-0.3.1/lincs/liblincs/median-and-max.hpp
--rw-rw-r--   0 user      (1002) user      (1002)      741 2023-05-12 08:51:14.000000 lincs-0.3.1/lincs/liblincs/randomness-utils.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1391 2023-05-12 08:51:21.000000 lincs-0.3.1/lincs/liblincs/randomness-utils.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    10384 2023-05-11 16:48:16.000000 lincs-0.3.1/lincs/liblincs_module_tests.py
--rw-rw-r--   0 user      (1002) user      (1002)      759 2023-05-11 17:16:10.000000 lincs-0.3.1/lincs/visualization.py
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 08:54:07.058991 lincs-0.3.1/lincs.egg-info/
--rw-r--r--   0 user      (1002) user      (1002)    16795 2023-05-12 08:54:07.000000 lincs-0.3.1/lincs.egg-info/PKG-INFO
--rw-r--r--   0 user      (1002) user      (1002)      659 2023-05-12 08:54:07.000000 lincs-0.3.1/lincs.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1002) user      (1002)        1 2023-05-12 08:54:07.000000 lincs-0.3.1/lincs.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1002) user      (1002)       60 2023-05-12 08:54:07.000000 lincs-0.3.1/lincs.egg-info/entry_points.txt
--rw-r--r--   0 user      (1002) user      (1002)       27 2023-05-12 08:54:07.000000 lincs-0.3.1/lincs.egg-info/requires.txt
--rw-r--r--   0 user      (1002) user      (1002)       15 2023-05-12 08:54:07.000000 lincs-0.3.1/lincs.egg-info/top_level.txt
--rw-r--r--   0 user      (1002) user      (1002)       27 2023-05-05 13:01:57.000000 lincs-0.3.1/requirements.txt
--rw-r--r--   0 user      (1002) user      (1002)       38 2023-05-12 08:54:07.058991 lincs-0.3.1/setup.cfg
--rw-rw-r--   0 user      (1002) user      (1002)     2200 2023-05-12 08:53:31.000000 lincs-0.3.1/setup.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 12:23:46.596982 lincs-0.3.2/
+-rw-rw-r--   0 user      (1002) user      (1002)    35149 2023-05-12 12:03:36.000000 lincs-0.3.2/COPYING
+-rw-rw-r--   0 user      (1002) user      (1002)     7652 2023-05-12 12:04:16.000000 lincs-0.3.2/COPYING.LESSER
+-rw-rw-r--   0 user      (1002) user      (1002)      104 2023-05-12 11:51:00.000000 lincs-0.3.2/MANIFEST.in
+-rw-r--r--   0 user      (1002) user      (1002)    17319 2023-05-12 12:23:46.596982 lincs-0.3.2/PKG-INFO
+-rw-rw-r--   0 user      (1002) user      (1002)    16460 2023-05-12 12:10:40.000000 lincs-0.3.2/README.md
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 12:23:46.596982 lincs-0.3.2/lincs/
+-rw-rw-r--   0 user      (1002) user      (1002)      796 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/__init__.py
+-rw-rw-r--   0 user      (1002) user      (1002)      170 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/__main__.py
+-rw-rw-r--   0 user      (1002) user      (1002)    21977 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/command_line_interface.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 12:23:46.596982 lincs-0.3.2/lincs/liblincs/
+-rw-rw-r--   0 user      (1002) user      (1002)     1610 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/classification.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      368 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/classification.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    10039 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/generation.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1042 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/generation.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 12:23:46.596982 lincs-0.3.2/lincs/liblincs/io/
+-rw-rw-r--   0 user      (1002) user      (1002)     2461 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/io/alternatives.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1004 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/io/alternatives.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     2582 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/io/domain.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1886 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/io/domain.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1875 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/io/model.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1640 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/io/model.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)       53 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/io.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      186 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/io.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 12:23:46.596982 lincs-0.3.2/lincs/liblincs/learning/
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 12:23:46.592982 lincs-0.3.2/lincs/liblincs/learning/weights-profiles-breed-mrsort/
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 12:23:46.596982 lincs-0.3.2/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/
+-rw-rw-r--   0 user      (1002) user      (1002)     9494 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     2125 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 12:23:46.596982 lincs-0.3.2/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/
+-rw-rw-r--   0 user      (1002) user      (1002)     4406 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1265 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 12:23:46.596982 lincs-0.3.2/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/
+-rw-rw-r--   0 user      (1002) user      (1002)     4495 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/glop.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      922 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/glop.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 12:23:46.596982 lincs-0.3.2/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/
+-rw-rw-r--   0 user      (1002) user      (1002)      244 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      682 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     6757 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/learning/weights-profiles-breed-mrsort.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     3486 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/learning/weights-profiles-breed-mrsort.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1727 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/learning.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      551 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/learning.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    15121 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/liblincs_module.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      245 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/lincs.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     2963 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/median-and-max.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      751 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/median-and-max.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)      776 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/randomness-utils.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1539 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs/randomness-utils.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    10418 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/liblincs_module_tests.py
+-rw-rw-r--   0 user      (1002) user      (1002)      793 2023-05-12 11:51:00.000000 lincs-0.3.2/lincs/visualization.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 12:23:46.596982 lincs-0.3.2/lincs.egg-info/
+-rw-r--r--   0 user      (1002) user      (1002)    17319 2023-05-12 12:23:46.000000 lincs-0.3.2/lincs.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1002) user      (1002)     1874 2023-05-12 12:23:46.000000 lincs-0.3.2/lincs.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1002) user      (1002)        1 2023-05-12 12:23:46.000000 lincs-0.3.2/lincs.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1002) user      (1002)       60 2023-05-12 12:23:46.000000 lincs-0.3.2/lincs.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1002) user      (1002)       27 2023-05-12 12:23:46.000000 lincs-0.3.2/lincs.egg-info/requires.txt
+-rw-r--r--   0 user      (1002) user      (1002)       15 2023-05-12 12:23:46.000000 lincs-0.3.2/lincs.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1002) user      (1002)       61 2023-05-12 11:51:00.000000 lincs-0.3.2/requirements.txt
+-rw-r--r--   0 user      (1002) user      (1002)       38 2023-05-12 12:23:46.596982 lincs-0.3.2/setup.cfg
+-rw-rw-r--   0 user      (1002) user      (1002)     2298 2023-05-12 12:22:54.000000 lincs-0.3.2/setup.py
```

### Comparing `lincs-0.3.1/PKG-INFO` & `lincs-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 Metadata-Version: 2.1
 Name: lincs
-Version: 0.3.1
+Version: 0.3.2
 Summary: MCDA algorithms
-Home-page: https://github.com/jacquev6/lincs
+Home-page: https://github.com/MICS-Lab/lincs
 Author: Vincent Jacques
 Author-email: vincent@vincent-jacques.net
+License: LGPLv3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
+License-File: COPYING
+License-File: COPYING.LESSER
+
+<!-- Copyright 2023 Vincent Jacques -->
 
 *lincs* is a collection of MCDA algorithms, usable as a C++ library, a Python package and a command-line utility.
 
-Note that *lincs* is not licensed yet, so you don't have any rights besides reading it for now.
+*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files [COPYING](COPYING) and [COPYING.LESSER](COPYING.LESSER).
+
+@todo (When we have a paper to actually cite) Add a note asking academics to kindly cite our work.
+
+Questions? Remarks? Bugs? Want to contribute? Open [an issue](https://github.com/MICS-Lab/lincs/issues) or [a discussion](https://github.com/MICS-Lab/lincs/discussions)!
 
 # Contributors and previous work
 
 *lincs* is developed by the [MICS](https://mics.centralesupelec.fr/) research team at [CentraleSupélec](https://www.centralesupelec.fr/).
 
 Its main authors are (alphabetical order):
 - [Laurent Cabaret](http://perso.ecp.fr/~cabaretl/) (performance optimization)
@@ -267,15 +277,15 @@
 <!-- STOP -->
 <!-- EXTEND command-line-example/run.sh --><!--
     cp model.png ../../..
 --><!-- STOP -->
 
 It should output something like:
 
-![Model visualization](https://github.com/jacquev6/lincs/raw/v0.3.1/model.png)
+![Model visualization](https://github.com/MICS-Lab/lincs/raw/v0.3.2/model.png)
 
 And finally generate a set of classified alternatives (@todo Link to concepts and file formats):
 
 <!-- EXTEND command-line-example/run.sh -->
     lincs generate classified-alternatives domain.yml model.yml 1000 --output-classified-alternatives learning-set.csv
 <!-- APPEND-TO-LAST-LINE --random-seed 42 -->
 <!-- STOP -->
@@ -302,15 +312,15 @@
 <!-- STOP -->
 <!-- EXTEND command-line-example/run.sh --><!--
     cp alternatives.png ../../..
 --><!-- STOP -->
 
 It should output something like:
 
-![Alternatives visualization](https://github.com/jacquev6/lincs/raw/v0.3.1/alternatives.png)
+![Alternatives visualization](https://github.com/MICS-Lab/lincs/raw/v0.3.2/alternatives.png)
 
 @todo Improve how this graph looks:
 
 - display categories as stacked solid colors
 - display alternatives in a color that matches their assigned category
 - remove the legend, place names (categories and alternatives) directly on the graph
```

### Comparing `lincs-0.3.1/README.md` & `lincs-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
+<!-- Copyright 2023 Vincent Jacques -->
+
 *lincs* is a collection of MCDA algorithms, usable as a C++ library, a Python package and a command-line utility.
 
-Note that *lincs* is not licensed yet, so you don't have any rights besides reading it for now.
+*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files [COPYING](COPYING) and [COPYING.LESSER](COPYING.LESSER).
+
+@todo (When we have a paper to actually cite) Add a note asking academics to kindly cite our work.
+
+Questions? Remarks? Bugs? Want to contribute? Open [an issue](https://github.com/MICS-Lab/lincs/issues) or [a discussion](https://github.com/MICS-Lab/lincs/discussions)!
 
 # Contributors and previous work
 
 *lincs* is developed by the [MICS](https://mics.centralesupelec.fr/) research team at [CentraleSupélec](https://www.centralesupelec.fr/).
 
 Its main authors are (alphabetical order):
 - [Laurent Cabaret](http://perso.ecp.fr/~cabaretl/) (performance optimization)
```

### Comparing `lincs-0.3.1/lincs/__init__.py` & `lincs-0.3.2/lincs/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright 2023 Vincent Jacques
+
 from liblincs import ValueType, CategoryCorrelation, Criterion, Category, Domain, load_domain, generate_domain
 from liblincs import SufficientCoalitionsKind, SufficientCoalitions, Boundary, Model, load_model, generate_mrsort_model
 from liblincs import Alternative, Alternatives, load_alternatives, generate_alternatives, classify_alternatives
 from liblincs import ProfilesInitializationStrategy, InitializeProfilesForProbabilisticMaximalDiscriminationPowerPerCriterion
 from liblincs import WeightsOptimizationStrategy, OptimizeWeightsUsingGlop
 from liblincs import ProfilesImprovementStrategy, ImproveProfilesWithAccuracyHeuristic
 from liblincs import TerminationStrategy, TerminateAtAccuracy
```

### Comparing `lincs-0.3.1/lincs/command_line_interface.py` & `lincs-0.3.2/lincs/command_line_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright 2023 Vincent Jacques
+
 from __future__ import annotations
 import math
 import random
 import subprocess
 import sys
 
 import click
```

### Comparing `lincs-0.3.1/lincs/liblincs/classification.cpp` & `lincs-0.3.2/lincs/liblincs/classification.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-#include "lincs.hpp"
+// Copyright 2023 Vincent Jacques
+
+#include "classification.hpp"
 
 #include <cassert>
 
 
 namespace lincs {
 
 ClassificationResult classify_alternatives(const Domain& domain, const Model& model, Alternatives* alternatives) {
```

### Comparing `lincs-0.3.1/lincs/liblincs/generation.cpp` & `lincs-0.3.2/lincs/liblincs/generation.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,45 @@
-#include "lincs.hpp"
+// Copyright 2023 Vincent Jacques
+
+#include "generation.hpp"
 
 #include <algorithm>
 #include <cassert>
 #include <random>
 
+#include "classification.hpp"
+
 
 namespace lincs {
 
-Domain Domain::generate(const unsigned criteria_count, const unsigned categories_count, const unsigned random_seed) {
+Domain generate_domain(const unsigned criteria_count, const unsigned categories_count, const unsigned random_seed) {
   // There is nothing random yet. There will be when other value types and category correlations are added.
 
-  std::vector<Criterion> criteria;
+  std::vector<Domain::Criterion> criteria;
   criteria.reserve(criteria_count);
   for (unsigned criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
-    criteria.push_back(Criterion{
+    criteria.emplace_back(
       "Criterion " + std::to_string(criterion_index + 1),
-      Criterion::ValueType::real,
-      Criterion::CategoryCorrelation::growing,
-    });
+      Domain::Criterion::ValueType::real,
+      Domain::Criterion::CategoryCorrelation::growing
+    );
   }
 
-  std::vector<Category> categories;
+  std::vector<Domain::Category> categories;
   categories.reserve(categories_count);
   for (unsigned category_index = 0; category_index != categories_count; ++category_index) {
-    categories.push_back(Category{
-      "Category " + std::to_string(category_index + 1),
-    });
+    categories.emplace_back(
+      "Category " + std::to_string(category_index + 1)
+    );
   }
 
   return Domain{criteria, categories};
 }
 
-Model Model::generate_mrsort(const Domain& domain, const unsigned random_seed, const std::optional<float> fixed_weights_sum) {
+Model generate_mrsort_model(const Domain& domain, const unsigned random_seed, const std::optional<float> fixed_weights_sum) {
   const unsigned categories_count = domain.categories.size();
   const unsigned criteria_count = domain.criteria.size();
 
   std::mt19937 gen(random_seed);
 
   // Profile can take any values. We arbitrarily generate them uniformly
   std::uniform_real_distribution<float> values_distribution(0.01f, 0.99f);
@@ -78,23 +82,23 @@
   const float weights_sum = fixed_weights_sum ? *fixed_weights_sum : 1.f / std::uniform_real_distribution<float>(0.f, 1.f)(gen);
   std::vector<float> denormalized_weights(criteria_count);
   std::transform(
     normalized_weights.begin(), normalized_weights.end(),
     denormalized_weights.begin(),
     [weights_sum](float w) { return w * weights_sum; });
 
-  SufficientCoalitions coalitions{
-    SufficientCoalitions::Kind::weights,
+  Model::SufficientCoalitions coalitions{
+    Model::SufficientCoalitions::Kind::weights,
     denormalized_weights,
   };
 
-  std::vector<Boundary> boundaries;
+  std::vector<Model::Boundary> boundaries;
   boundaries.reserve(categories_count - 1);
   for (unsigned category_index = 0; category_index != categories_count - 1; ++category_index) {
-    boundaries.push_back(Boundary{profiles[category_index], coalitions});
+    boundaries.emplace_back(profiles[category_index], coalitions);
   }
 
   return Model(domain, boundaries);
 }
 
 Alternatives generate_uniform_alternatives(
   const Domain& domain,
@@ -240,15 +244,15 @@
 
     if (iterations_with_no_effect > max_iterations_with_no_effect) {
       throw BalancedAlternativesGenerationException(histogram);
     }
   }
 }
 
-Alternatives Alternatives::generate(
+Alternatives generate_alternatives(
   const Domain& domain,
   const Model& model,
   const unsigned alternatives_count,
   const unsigned random_seed,
   const std::optional<float> max_imbalance
 ) {
   std::mt19937 gen(random_seed);
```

### Comparing `lincs-0.3.1/lincs/liblincs/liblincs_module.cpp` & `lincs-0.3.2/lincs/liblincs/liblincs_module.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+// Copyright 2023 Vincent Jacques
+
 #include "lincs.hpp"
 
 #include <iostream>
 
 #include <boost/python.hpp>
 #include <boost/python/suite/indexing/vector_indexing_suite.hpp>
 #include <boost/iostreams/concepts.hpp>
@@ -220,15 +222,15 @@
     "load_domain",
     &load_domain,
     (bp::arg("in")),
     "Load a domain from the provided `.read()`-supporting file-like object, in YAML format."
   );
   bp::def(
     "generate_domain",
-    &lincs::Domain::generate,
+    &lincs::generate_domain,
     (bp::arg("criteria_count"), "categories_count", "random_seed"),
     "Generate a domain with `criteria_count` criteria and `categories_count` categories."
   );
 
   bp::class_<lincs::Model::SufficientCoalitions>("SufficientCoalitions", bp::init<lincs::Model::SufficientCoalitions::Kind, std::vector<float>>())
     .def_readwrite("kind", &lincs::Model::SufficientCoalitions::kind)
     .def_readwrite("criterion_weights", &lincs::Model::SufficientCoalitions::criterion_weights)
@@ -257,15 +259,15 @@
     "load_model",
     &load_model,
     (bp::arg("domain"), "in"),
     "Load a model for the provided `domain`, from the provided `.read()`-supporting file-like object, in YAML format."
   );
   bp::def(
     "generate_mrsort_model",
-    &lincs::Model::generate_mrsort,
+    &lincs::generate_mrsort_model,
     (bp::arg("domain"), "random_seed", bp::arg("fixed_weights_sum")=std::optional<float>()),
     "Generate an MR-Sort model for the provided `domain`."
   );
 
   bp::class_<lincs::Alternative>("Alternative", bp::init<std::string, std::vector<float>, std::string>())
     .def_readwrite("name", &lincs::Alternative::name)
     .def_readwrite("profile", &lincs::Alternative::profile)
@@ -287,15 +289,15 @@
     "load_alternatives",
     &load_alternatives,
     (bp::arg("domain"), "in"),
     "Load a set of alternatives (classified or not) from the provided `.read()`-supporting file-like object, in CSV format."
   );
   bp::def(
     "generate_alternatives",
-    &lincs::Alternatives::generate,
+    &lincs::generate_alternatives,
     (bp::arg("domain"), "model", "alternatives_count", "random_seed", bp::arg("max_imbalance")=std::optional<float>()),
     "Generate a set of `alternatives_count` pseudo-random alternatives for the provided `domain`, classified according to the provided `model`."
   );
 
   bp::class_<lincs::ClassificationResult>("ClassificationResult", bp::no_init)
     .def_readonly("changed", &lincs::ClassificationResult::changed)
     .def_readonly("unchanged", &lincs::ClassificationResult::unchanged)
```

### Comparing `lincs-0.3.1/lincs/liblincs/median-and-max.cpp` & `lincs-0.3.2/lincs/liblincs/median-and-max.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+// Copyright 2023 Vincent Jacques
+
 #include "median-and-max.hpp"
 
 #include <numeric>
 #include <random>
 
 #include <doctest.h>  // Keep last because it defines really common names like CHECK that we don't want injected into other headers
```

### Comparing `lincs-0.3.1/lincs/liblincs/randomness-utils.cpp` & `lincs-0.3.2/lincs/liblincs/randomness-utils.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+// Copyright 2023 Vincent Jacques
+
 #include "randomness-utils.hpp"
 
 #include <doctest.h>  // Keep last because it defines really common names like CHECK that we don't want injected into other headers
 
 
 TEST_CASE("ProbabilityWeightedGenerator") {
   std::map<std::string, double> value_probabilities = {
```

### Comparing `lincs-0.3.1/lincs/liblincs_module_tests.py` & `lincs-0.3.2/lincs/liblincs_module_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright 2023 Vincent Jacques
+
 import unittest
 
 from . import *
 
 
 class DomainTestCase(unittest.TestCase):
     def test_init_empty(self):
```

### Comparing `lincs-0.3.1/lincs/visualization.py` & `lincs-0.3.2/lincs/visualization.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright 2023 Vincent Jacques
+
 import matplotlib.pyplot as plt
 
 
 def visualize_model(domain, model, alternatives, alternatives_count, out):
     fig, ax = plt.subplots(1, 1, figsize=(6, 4), layout="constrained")
 
     xs = [criterion.name for criterion in domain.criteria]
```

### Comparing `lincs-0.3.1/lincs.egg-info/PKG-INFO` & `lincs-0.3.2/lincs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 Metadata-Version: 2.1
 Name: lincs
-Version: 0.3.1
+Version: 0.3.2
 Summary: MCDA algorithms
-Home-page: https://github.com/jacquev6/lincs
+Home-page: https://github.com/MICS-Lab/lincs
 Author: Vincent Jacques
 Author-email: vincent@vincent-jacques.net
+License: LGPLv3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
+License-File: COPYING
+License-File: COPYING.LESSER
+
+<!-- Copyright 2023 Vincent Jacques -->
 
 *lincs* is a collection of MCDA algorithms, usable as a C++ library, a Python package and a command-line utility.
 
-Note that *lincs* is not licensed yet, so you don't have any rights besides reading it for now.
+*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files [COPYING](COPYING) and [COPYING.LESSER](COPYING.LESSER).
+
+@todo (When we have a paper to actually cite) Add a note asking academics to kindly cite our work.
+
+Questions? Remarks? Bugs? Want to contribute? Open [an issue](https://github.com/MICS-Lab/lincs/issues) or [a discussion](https://github.com/MICS-Lab/lincs/discussions)!
 
 # Contributors and previous work
 
 *lincs* is developed by the [MICS](https://mics.centralesupelec.fr/) research team at [CentraleSupélec](https://www.centralesupelec.fr/).
 
 Its main authors are (alphabetical order):
 - [Laurent Cabaret](http://perso.ecp.fr/~cabaretl/) (performance optimization)
@@ -267,15 +277,15 @@
 <!-- STOP -->
 <!-- EXTEND command-line-example/run.sh --><!--
     cp model.png ../../..
 --><!-- STOP -->
 
 It should output something like:
 
-![Model visualization](https://github.com/jacquev6/lincs/raw/v0.3.1/model.png)
+![Model visualization](https://github.com/MICS-Lab/lincs/raw/v0.3.2/model.png)
 
 And finally generate a set of classified alternatives (@todo Link to concepts and file formats):
 
 <!-- EXTEND command-line-example/run.sh -->
     lincs generate classified-alternatives domain.yml model.yml 1000 --output-classified-alternatives learning-set.csv
 <!-- APPEND-TO-LAST-LINE --random-seed 42 -->
 <!-- STOP -->
@@ -302,15 +312,15 @@
 <!-- STOP -->
 <!-- EXTEND command-line-example/run.sh --><!--
     cp alternatives.png ../../..
 --><!-- STOP -->
 
 It should output something like:
 
-![Alternatives visualization](https://github.com/jacquev6/lincs/raw/v0.3.1/alternatives.png)
+![Alternatives visualization](https://github.com/MICS-Lab/lincs/raw/v0.3.2/alternatives.png)
 
 @todo Improve how this graph looks:
 
 - display categories as stacked solid colors
 - display alternatives in a color that matches their assigned category
 - remove the legend, place names (categories and alternatives) directly on the graph
```

### Comparing `lincs-0.3.1/setup.py` & `lincs-0.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+# Copyright 2023 Vincent Jacques
+
 import glob
 import setuptools
 
 
-version = "0.3.1"
+version = "0.3.2"
 
 with open("README.md") as f:
     long_description = f.read()
 for image in ["model", "alternatives"]:
-    long_description = long_description.replace(f"]({image}.png)", f"](https://github.com/jacquev6/lincs/raw/v{version}/{image}.png)")
+    long_description = long_description.replace(f"]({image}.png)", f"](https://github.com/MICS-Lab/lincs/raw/v{version}/{image}.png)")
 
 with open("requirements.txt") as f:
     install_requires = f.readlines()
 
 
 # @todo Consider using scikit-build:
 # it should make it easier to compile CUDA code using nvcc and to run C++ unit tests during build.
@@ -32,17 +34,18 @@
     extra_link_args=["-fopenmp"],
 )
 
 setuptools.setup(
     name="lincs",
     version=version,
     description="MCDA algorithms",
+    license="LGPLv3",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/jacquev6/lincs",
+    url="https://github.com/MICS-Lab/lincs",
     author="Vincent Jacques",
     author_email="vincent@vincent-jacques.net",
     install_requires=install_requires,
     packages=setuptools.find_packages(),
     include_package_data=True,
     entry_points={
         "console_scripts": [
@@ -51,14 +54,14 @@
     },
     ext_modules=[liblincs],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
-        # Note: no license classifier yet
+        "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: C++",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
 )
```


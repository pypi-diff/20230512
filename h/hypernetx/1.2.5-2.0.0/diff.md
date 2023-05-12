# Comparing `tmp/hypernetx-1.2.5.tar.gz` & `tmp/hypernetx-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/boni407/Workplace/aida/hypernetx/dist/tmpx301_z4d/hypernetx-1.2.5.tar", last modified: Thu Aug 25 17:28:24 2022, max compression
+gzip compressed data, was "hypernetx-2.0.0.tar", last modified: Fri May 12 20:04:27 2023, max compression
```

## Comparing `hypernetx-1.2.5.tar` & `hypernetx-2.0.0.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2022-08-25 17:28:24.000000 hypernetx-1.2.5/
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     1794 2022-07-07 16:12:57.000000 hypernetx-1.2.5/LICENSE.rst
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     2870 2022-08-25 17:28:24.000000 hypernetx-1.2.5/PKG-INFO
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    11326 2022-08-25 16:11:33.000000 hypernetx-1.2.5/README.md
-drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2022-08-25 17:28:24.000000 hypernetx-1.2.5/hypernetx/
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      416 2022-08-24 18:11:24.000000 hypernetx-1.2.5/hypernetx/__init__.py
-drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2022-08-25 17:28:24.000000 hypernetx-1.2.5/hypernetx/algorithms/
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      198 2022-08-25 16:11:33.000000 hypernetx-1.2.5/hypernetx/algorithms/__init__.py
-drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2022-08-25 17:28:24.000000 hypernetx-1.2.5/hypernetx/algorithms/contagion/
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)       50 2022-08-25 16:11:33.000000 hypernetx-1.2.5/hypernetx/algorithms/contagion/__init__.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     3706 2022-08-25 16:11:33.000000 hypernetx-1.2.5/hypernetx/algorithms/contagion/animation.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    36498 2022-08-25 16:11:33.000000 hypernetx-1.2.5/hypernetx/algorithms/contagion/epidemics.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     8682 2022-08-05 21:34:44.000000 hypernetx-1.2.5/hypernetx/algorithms/generative_models.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    24714 2022-08-25 16:11:33.000000 hypernetx-1.2.5/hypernetx/algorithms/homology_mod2.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    14911 2022-08-25 16:11:33.000000 hypernetx-1.2.5/hypernetx/algorithms/hypergraph_modularity.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     8317 2022-08-25 16:11:33.000000 hypernetx-1.2.5/hypernetx/algorithms/laplacians_clustering.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    11624 2022-08-25 16:11:33.000000 hypernetx-1.2.5/hypernetx/algorithms/s_centrality_measures.py
-drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2022-08-25 17:28:24.000000 hypernetx-1.2.5/hypernetx/classes/
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      129 2022-08-25 16:11:33.000000 hypernetx-1.2.5/hypernetx/classes/__init__.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    32107 2022-08-15 18:30:39.000000 hypernetx-1.2.5/hypernetx/classes/entity.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    87508 2022-08-24 18:11:24.000000 hypernetx-1.2.5/hypernetx/classes/hypergraph.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    42131 2022-08-15 18:30:39.000000 hypernetx-1.2.5/hypernetx/classes/staticentity.py
-drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2022-08-25 17:28:24.000000 hypernetx-1.2.5/hypernetx/drawing/
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)       78 2022-08-25 16:11:33.000000 hypernetx-1.2.5/hypernetx/drawing/__init__.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    15245 2022-08-25 16:11:33.000000 hypernetx-1.2.5/hypernetx/drawing/rubber_band.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     5626 2022-08-25 16:11:33.000000 hypernetx-1.2.5/hypernetx/drawing/two_column.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     3401 2022-08-05 21:34:44.000000 hypernetx-1.2.5/hypernetx/drawing/util.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      426 2022-08-05 21:34:44.000000 hypernetx-1.2.5/hypernetx/exception.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      379 2022-07-07 16:12:57.000000 hypernetx-1.2.5/hypernetx/read_write.py
-drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2022-08-25 17:28:24.000000 hypernetx-1.2.5/hypernetx/reports/
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)       33 2022-08-25 16:11:33.000000 hypernetx-1.2.5/hypernetx/reports/__init__.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    11690 2022-08-25 16:11:33.000000 hypernetx-1.2.5/hypernetx/reports/descriptive_stats.py
-drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2022-08-25 17:28:24.000000 hypernetx-1.2.5/hypernetx/utils/
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      375 2022-08-25 16:11:33.000000 hypernetx-1.2.5/hypernetx/utils/__init__.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     1725 2022-07-29 00:38:06.000000 hypernetx-1.2.5/hypernetx/utils/decorators.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     5966 2022-08-15 18:30:39.000000 hypernetx-1.2.5/hypernetx/utils/extras.py
-drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2022-08-25 17:28:24.000000 hypernetx-1.2.5/hypernetx/utils/toys/
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      188 2022-08-25 16:11:33.000000 hypernetx-1.2.5/hypernetx/utils/toys/__init__.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      377 2022-08-25 16:11:33.000000 hypernetx-1.2.5/hypernetx/utils/toys/gene_data.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     2951 2022-08-25 16:11:33.000000 hypernetx-1.2.5/hypernetx/utils/toys/harrypotter.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    14359 2022-08-25 16:11:33.000000 hypernetx-1.2.5/hypernetx/utils/toys/lesmis.py
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      587 2022-08-25 16:11:33.000000 hypernetx-1.2.5/hypernetx/utils/toys/transmission_problem.py
-drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2022-08-25 17:28:24.000000 hypernetx-1.2.5/hypernetx.egg-info/
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     2870 2022-08-25 17:28:24.000000 hypernetx-1.2.5/hypernetx.egg-info/PKG-INFO
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     1232 2022-08-25 17:28:24.000000 hypernetx-1.2.5/hypernetx.egg-info/SOURCES.txt
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)        1 2022-08-25 17:28:24.000000 hypernetx-1.2.5/hypernetx.egg-info/dependency_links.txt
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      362 2022-08-25 17:28:24.000000 hypernetx-1.2.5/hypernetx.egg-info/requires.txt
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)       10 2022-08-25 17:28:24.000000 hypernetx-1.2.5/hypernetx.egg-info/top_level.txt
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)       79 2022-08-25 17:28:24.000000 hypernetx-1.2.5/setup.cfg
--rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     3877 2022-08-25 17:28:05.000000 hypernetx-1.2.5/setup.py
+drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2023-05-12 20:04:27.403125 hypernetx-2.0.0/
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     1794 2023-05-11 23:29:15.000000 hypernetx-2.0.0/LICENSE.rst
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     3294 2023-05-11 23:29:15.000000 hypernetx-2.0.0/LONG_DESCRIPTION.rst
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     3883 2023-05-12 20:04:27.403361 hypernetx-2.0.0/PKG-INFO
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    13883 2023-05-12 17:41:52.000000 hypernetx-2.0.0/README.md
+drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2023-05-12 20:04:27.324388 hypernetx-2.0.0/hypernetx/
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      394 2023-05-11 23:29:16.000000 hypernetx-2.0.0/hypernetx/__init__.py
+drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2023-05-12 20:04:27.339773 hypernetx-2.0.0/hypernetx/algorithms/
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     2596 2023-05-11 23:29:16.000000 hypernetx-2.0.0/hypernetx/algorithms/__init__.py
+-rwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)    21350 2023-05-11 23:29:16.000000 hypernetx-2.0.0/hypernetx/algorithms/barycentric_subdivisions.py
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    39961 2023-05-11 23:29:16.000000 hypernetx-2.0.0/hypernetx/algorithms/contagion.py
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     8678 2023-05-11 23:28:49.000000 hypernetx-2.0.0/hypernetx/algorithms/generative_models.py
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    24275 2023-05-11 23:28:49.000000 hypernetx-2.0.0/hypernetx/algorithms/homology_mod2.py
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    15464 2023-05-11 23:29:16.000000 hypernetx-2.0.0/hypernetx/algorithms/hypergraph_modularity.py
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     7820 2023-05-11 23:29:16.000000 hypernetx-2.0.0/hypernetx/algorithms/laplacians_clustering.py
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     9966 2023-05-11 23:29:16.000000 hypernetx-2.0.0/hypernetx/algorithms/s_centrality_measures.py
+drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2023-05-12 20:04:27.345636 hypernetx-2.0.0/hypernetx/classes/
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      195 2023-05-11 23:29:16.000000 hypernetx-2.0.0/hypernetx/classes/__init__.py
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    55664 2023-05-11 23:29:16.000000 hypernetx-2.0.0/hypernetx/classes/entity.py
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    27383 2023-05-11 23:29:16.000000 hypernetx-2.0.0/hypernetx/classes/entityset.py
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     8557 2023-05-11 23:29:16.000000 hypernetx-2.0.0/hypernetx/classes/helpers.py
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    82331 2023-05-11 23:29:16.000000 hypernetx-2.0.0/hypernetx/classes/hypergraph.py
+drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2023-05-12 20:04:27.350859 hypernetx-2.0.0/hypernetx/drawing/
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      151 2023-05-11 23:28:49.000000 hypernetx-2.0.0/hypernetx/drawing/__init__.py
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    15120 2023-05-11 23:28:49.000000 hypernetx-2.0.0/hypernetx/drawing/rubber_band.py
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     5596 2023-05-11 23:29:16.000000 hypernetx-2.0.0/hypernetx/drawing/two_column.py
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     3398 2023-05-11 23:28:49.000000 hypernetx-2.0.0/hypernetx/drawing/util.py
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      640 2023-05-11 23:29:16.000000 hypernetx-2.0.0/hypernetx/exception.py
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      379 2022-07-07 16:12:57.000000 hypernetx-2.0.0/hypernetx/read_write.py
+drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2023-05-12 20:04:27.370413 hypernetx-2.0.0/hypernetx/reports/
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      491 2023-05-11 23:28:49.000000 hypernetx-2.0.0/hypernetx/reports/__init__.py
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    11362 2023-05-11 23:49:30.000000 hypernetx-2.0.0/hypernetx/reports/descriptive_stats.py
+drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2023-05-12 20:04:27.376064 hypernetx-2.0.0/hypernetx/utils/
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      760 2023-05-11 23:28:49.000000 hypernetx-2.0.0/hypernetx/utils/__init__.py
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     2428 2023-05-11 23:29:16.000000 hypernetx-2.0.0/hypernetx/utils/decorators.py
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     5960 2023-05-11 23:29:16.000000 hypernetx-2.0.0/hypernetx/utils/extras.py
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     1423 2023-05-11 23:29:16.000000 hypernetx-2.0.0/hypernetx/utils/log.py
+drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2023-05-12 20:04:27.402197 hypernetx-2.0.0/hypernetx/utils/toys/
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      409 2023-05-11 23:28:49.000000 hypernetx-2.0.0/hypernetx/utils/toys/__init__.py
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      353 2023-05-11 23:28:49.000000 hypernetx-2.0.0/hypernetx/utils/toys/gene_data.py
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     2844 2023-05-11 23:28:49.000000 hypernetx-2.0.0/hypernetx/utils/toys/harrypotter.py
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)    14357 2023-05-11 23:29:16.000000 hypernetx-2.0.0/hypernetx/utils/toys/lesmis.py
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)      552 2023-05-11 23:28:49.000000 hypernetx-2.0.0/hypernetx/utils/toys/transmission_problem.py
+drwxr-xr-x   0 boni407  (1550152542) PNL\Domain Users (2016721313)        0 2023-05-12 20:04:27.331010 hypernetx-2.0.0/hypernetx.egg-info/
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     3883 2023-05-12 20:04:27.000000 hypernetx-2.0.0/hypernetx.egg-info/PKG-INFO
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     1269 2023-05-12 20:04:27.000000 hypernetx-2.0.0/hypernetx.egg-info/SOURCES.txt
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)        1 2023-05-12 20:04:27.000000 hypernetx-2.0.0/hypernetx.egg-info/dependency_links.txt
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     1067 2023-05-12 20:04:27.000000 hypernetx-2.0.0/hypernetx.egg-info/requires.txt
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)       10 2023-05-12 20:04:27.000000 hypernetx-2.0.0/hypernetx.egg-info/top_level.txt
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)       97 2023-05-11 23:28:49.000000 hypernetx-2.0.0/pyproject.toml
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)     2369 2023-05-12 20:04:27.421576 hypernetx-2.0.0/setup.cfg
+-rw-r--r--   0 boni407  (1550152542) PNL\Domain Users (2016721313)       80 2023-05-11 23:29:16.000000 hypernetx-2.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `hypernetx-1.2.5/LICENSE.rst` & `hypernetx-2.0.0/LICENSE.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _license:
 
 License
 =======
 
 HyperNetX
 
-Copyright © 2018, Battelle Memorial Institute
+Copyright © 2023, Battelle Memorial Institute
 
 Battelle Memorial Institute (hereinafter Battelle) hereby grants permission
 to any person or entity lawfully obtaining a copy of this software and associated
 documentation files (hereinafter “the Software”) to redistribute and use the
 Software in source and binary forms, with or without modification.  Such person
 or entity may use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and may permit others to do so, subject to the
```

### Comparing `hypernetx-1.2.5/hypernetx/algorithms/contagion/epidemics.py` & `hypernetx-2.0.0/hypernetx/algorithms/contagion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,128 @@
 import random
-import heapq
 import numpy as np
 from collections import defaultdict
 from collections import Counter
+import hypernetx as hnx
+
+try:
+    from celluloid import Camera
+except Exception as e:
+    print(
+        f" {e}. If you need to use {__name__}, please install additional packages by running the following command: pip install .['all']"
+    )
+
+
+def contagion_animation(
+    fig,
+    H,
+    transition_events,
+    node_state_color_dict,
+    edge_state_color_dict,
+    node_radius=1,
+    fps=1,
+):
+    """
+    A function to animate discrete-time contagion models for hypergraphs. Currently only supports a circular layout.
+
+    Parameters
+    ----------
+    fig : matplotlib Figure object
+    H : HyperNetX Hypergraph object
+    transition_events : dictionary
+        The dictionary that is output from the discrete_SIS and discrete_SIR functions with return_full_data=True
+    node_state_color_dict : dictionary
+        Dictionary which specifies the colors of each node state. All node states must be specified.
+    edge_state_color_dict : dictionary
+        Dictionary with keys that are edge states and values which specify the colors of each edge state
+        (can specify an alpha parameter). All edge-dependent transition states must be specified
+        (most common is "I") and there must be a a default "OFF" setting.
+    node_radius : float, default: 1
+        The radius of the nodes to draw
+    fps : int > 0, default: 1
+        Frames per second of the animation
+
+    Returns
+    -------
+    matplotlib Animation object
+
+    Notes
+    -----
+
+    Example::
+
+        >>> import hypernetx.algorithms.contagion as contagion
+        >>> import random
+        >>> import hypernetx as hnx
+        >>> import matplotlib.pyplot as plt
+        >>> from IPython.display import HTML
+        >>> n = 1000
+        >>> m = 10000
+        >>> hyperedgeList = [random.sample(range(n), k=random.choice([2,3])) for i in range(m)]
+        >>> H = hnx.Hypergraph(hyperedgeList)
+        >>> tau = {2:0.1, 3:0.1}
+        >>> gamma = 0.1
+        >>> tmax = 100
+        >>> dt = 0.1
+        >>> transition_events = contagion.discrete_SIS(H, tau, gamma, rho=0.1, tmin=0, tmax=tmax, dt=dt, return_full_data=True)
+        >>> node_state_color_dict = {"S":"green", "I":"red", "R":"blue"}
+        >>> edge_state_color_dict = {"S":(0, 1, 0, 0.3), "I":(1, 0, 0, 0.3), "R":(0, 0, 1, 0.3), "OFF": (1, 1, 1, 0)}
+        >>> fps = 1
+        >>> fig = plt.figure()
+        >>> animation = contagion.contagion_animation(fig, H, transition_events, node_state_color_dict, edge_state_color_dict, node_radius=1, fps=fps)
+        >>> HTML(animation.to_jshtml())
+    """
+
+    nodeState = defaultdict(lambda: "S")
+
+    camera = Camera(fig)
+
+    for t in sorted(list(transition_events.keys())):
+        edgeState = defaultdict(lambda: "OFF")
+
+        # update edge and node states
+        for event in transition_events[t]:
+            status = event[0]
+            node = event[1]
+
+            # update node states
+            nodeState[node] = status
+
+            try:
+                # update the edge transmitters list if they are neighbor-dependent transitions
+                edgeID = event[2]
+                if edgeID is not None:
+                    edgeState[edgeID] = status
+            except:
+                pass
+
+        kwargs = {"layout_kwargs": {"seed": 39}}
+
+        nodeStyle = {
+            "facecolors": [node_state_color_dict[nodeState[node]] for node in H.nodes]
+        }
+        edgeStyle = {
+            "facecolors": [edge_state_color_dict[edgeState[edge]] for edge in H.edges],
+            "edgecolors": "black",
+        }
+
+        # draw hypergraph
+        hnx.draw(
+            H,
+            node_radius=node_radius,
+            nodes_kwargs=nodeStyle,
+            edges_kwargs=edgeStyle,
+            with_edge_labels=False,
+            with_node_labels=False,
+            **kwargs,
+        )
+        camera.snap()
+
+    return camera.animate(interval=1000 / fps)
+
 
 # Canned Contagion Functions
 def collective_contagion(node, status, edge):
     """
     The collective contagion mechanism described in
     "The effect of heterogeneity on hypergraph contagion models" by Landry and Restrepo
     https://doi.org/10.1063/5.0020034
@@ -346,15 +462,15 @@
     initial_infecteds=None,
     initial_recovereds=None,
     rho=None,
     tmin=0,
     tmax=float("Inf"),
     dt=1.0,
     return_full_data=False,
-    **args
+    **args,
 ):
     """
     A discrete-time SIR model for hypergraphs similar to the construction described in
     "The effect of heterogeneity on hypergraph contagion models" by Landry and Restrepo
     https://doi.org/10.1063/5.0020034 and
     "Simplicial models of social contagion" by Iacopini et al.
     https://doi.org/10.1038/s41467-019-10431-6
@@ -452,18 +568,15 @@
     R = [len(initial_recovereds)]
     S = [H.number_of_nodes() - I[-1] - R[-1]]
 
     t = tmin
     times = [t]
     newStatus = status.copy()
 
-    if H.isstatic:
-        edge_neighbors = lambda node: H.edges.memberships[node]
-    else:
-        edge_neighbors = lambda node: H.nodes[node].memberships
+    edge_neighbors = lambda node: H.edges.memberships[node]
 
     while t < tmax and I[-1] != 0:
         # Initialize the next step with the same numbers of S, I, and R as the last step before computing the changes
         S.append(S[-1])
         I.append(I[-1])
         R.append(R[-1])
 
@@ -513,15 +626,15 @@
     transmission_function=threshold,
     initial_infecteds=None,
     rho=None,
     tmin=0,
     tmax=100,
     dt=1.0,
     return_full_data=False,
-    **args
+    **args,
 ):
     """
     A discrete-time SIS model for hypergraphs as implemented in
     "The effect of heterogeneity on hypergraph contagion models" by Landry and Restrepo
     https://doi.org/10.1063/5.0020034 and
     "Simplicial models of social contagion" by Iacopini et al.
     https://doi.org/10.1038/s41467-019-10431-6
@@ -605,18 +718,15 @@
     I = [len(initial_infecteds)]
     S = [H.number_of_nodes() - I[-1]]
 
     t = tmin
     times = [t]
     newStatus = status.copy()
 
-    if H.isstatic:
-        edge_neighbors = lambda node: H.edges.memberships[node]
-    else:
-        edge_neighbors = lambda node: H.nodes[node].memberships
+    edge_neighbors = lambda node: H.edges.memberships[node]
 
     while t < tmax and I[-1] != 0:
         # Initialize the next step with the same numbers of S, I, and R as the last step before computing the changes
         S.append(S[-1])
         I.append(I[-1])
         if return_full_data:
             transition_events[t + dt] = list()
@@ -664,15 +774,15 @@
     gamma,
     transmission_function=threshold,
     initial_infecteds=None,
     initial_recovereds=None,
     rho=None,
     tmin=0,
     tmax=float("Inf"),
-    **args
+    **args,
 ):
     """
     A continuous-time SIR model for hypergraphs similar to the model in
     "The effect of heterogeneity on hypergraph contagion models" by Landry and Restrepo
     https://doi.org/10.1063/5.0020034 and
     implemented for networks in the EoN package by Joel C. Miller
     https://epidemicsonnetworks.readthedocs.io/en/latest/
@@ -754,18 +864,15 @@
     for node in initial_recovereds:
         status[node] = "R"
 
     I = [len(initial_infecteds)]
     R = [len(initial_recovereds)]
     S = [H.number_of_nodes() - I[-1] - R[-1]]
 
-    if H.isstatic:
-        edge_neighbors = lambda node: H.edges.memberships[node]
-    else:
-        edge_neighbors = lambda node: H.nodes[node].memberships
+    edge_neighbors = lambda node: H.edges.memberships[node]
 
     t = tmin
     times = [t]
 
     infecteds = _ListDict_()
 
     infectious_edges = dict()
@@ -868,15 +975,15 @@
     transmission_function=threshold,
     initial_infecteds=None,
     rho=None,
     tmin=0,
     tmax=float("Inf"),
     return_full_data=False,
     sim_kwargs=None,
-    **args
+    **args,
 ):
     """
     A continuous-time SIS model for hypergraphs similar to the model in
     "The effect of heterogeneity on hypergraph contagion models" by Landry and Restrepo
     https://doi.org/10.1063/5.0020034 and
     implemented for networks in the EoN package by Joel C. Miller
     https://epidemicsonnetworks.readthedocs.io/en/latest/
@@ -946,18 +1053,15 @@
 
     for node in initial_infecteds:
         status[node] = "I"
 
     I = [len(initial_infecteds)]
     S = [H.number_of_nodes() - I[-1]]
 
-    if H.isstatic:
-        edge_neighbors = lambda node: H.edges.memberships[node]
-    else:
-        edge_neighbors = lambda node: H.nodes[node].memberships
+    edge_neighbors = lambda node: H.edges.memberships[node]
 
     t = tmin
     times = [t]
 
     infecteds = _ListDict_()
 
     infectious_edges = dict()
```

### Comparing `hypernetx-1.2.5/hypernetx/algorithms/generative_models.py` & `hypernetx-2.0.0/hypernetx/algorithms/generative_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     Returns
     -------
     HyperNetX Hypergraph object
 
 
     Example::
-    
+
     >>> import hypernetx.algorithms.generative_models as gm
     >>> n = 1000
     >>> m = n
     >>> p = 0.01
     >>> H = gm.erdos_renyi_hypergraph(n, m, p)
 
     """
```

### Comparing `hypernetx-1.2.5/hypernetx/algorithms/homology_mod2.py` & `hypernetx-2.0.0/hypernetx/algorithms/homology_mod2.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,39 +33,16 @@
 import numpy as np
 import hypernetx as hnx
 import warnings
 import copy
 from hypernetx import HyperNetXError
 from collections import defaultdict
 import itertools as it
-import pickle
 from scipy.sparse import csr_matrix
 
-__all__ = [
-    "kchainbasis",
-    "bkMatrix",
-    "swap_rows",
-    "swap_columns",
-    "add_to_row",
-    "add_to_column",
-    "logical_dot",
-    "logical_matmul",
-    "matmulreduce",
-    "logical_matadd",
-    "smith_normal_form_mod2",
-    "reduced_row_echelon_form_mod2",
-    "boundary_group",
-    "chain_complex",
-    "betti",
-    "betti_numbers",
-    "homology_basis",
-    "hypergraph_homology_basis",
-    "interpret",
-]
-
 
 def kchainbasis(h, k):
     """
     Compute the set of k dimensional cells in the abstract simplicial
     complex associated with the hypergraph.
 
     Parameters
```

### Comparing `hypernetx-1.2.5/hypernetx/algorithms/hypergraph_modularity.py` & `hypernetx-2.0.0/hypernetx/algorithms/hypergraph_modularity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 """
 Hypergraph_Modularity
 ---------------------
 Modularity and clustering for hypergraphs using HyperNetX.
-Adapted from F. Théberge's GitHub repository: `Hypergraph Clustering <https://github.com/ftheberge/Hypergraph_Clustering>`_ 
+Adapted from F. Théberge's GitHub repository: `Hypergraph Clustering <https://github.com/ftheberge/Hypergraph_Clustering>`_
 See Tutorial 13 in the tutorials folder for library usage.
 
 References
----------- 
+----------
 .. [1] Kumar T., Vaidyanathan S., Ananthapadmanabhan H., Parthasarathy S. and Ravindran B. "A New Measure of Modularity in Hypergraphs: Theoretical Insights and Implications for Effective Clustering". In: Cherifi H., Gaito S., Mendes J., Moro E., Rocha L. (eds) Complex Networks and Their Applications VIII. COMPLEX NETWORKS 2019. Studies in Computational Intelligence, vol 881. Springer, Cham. https://doi.org/10.1007/978-3-030-36687-2_24
 .. [2] Kamiński  B., Prałat  P. and Théberge  F. "Community Detection Algorithm Using Hypergraph Modularity". In: Benito R.M., Cherifi C., Cherifi H., Moro E., Rocha L.M., Sales-Pardo M. (eds) Complex Networks & Their Applications IX. COMPLEX NETWORKS 2020. Studies in Computational Intelligence, vol 943. Springer, Cham. https://doi.org/10.1007/978-3-030-65347-7_13
 .. [3] Kamiński  B., Poulin V., Prałat  P., Szufel P. and Théberge  F. "Clustering via hypergraph modularity", Plos ONE 2019, https://doi.org/10.1371/journal.pone.0224307
 """
 
 from collections import Counter
 import numpy as np
-from functools import reduce
-import igraph as ig
 import itertools
 from scipy.special import comb
 
+try:
+    import igraph as ig
+except Exception as e:
+    print(
+        f" {e}. If you need to use {__name__}, please install additional packages by running the following command: pip install .['all']"
+    )
 ################################################################################
 
 # we use 2 representations for partitions (0-based part ids):
 # (1) dictionary or (2) list of sets
 
 
 def dict2part(D):
@@ -64,42 +68,42 @@
       a dictionary with {vertex: partition index}
     """
     x = []
     for i in range(len(A)):
         x.extend([(a, i) for a in A[i]])
     return {k: v for k, v in x}
 
+
 ################################################################################
 
 
-def precompute_attributes(HG):
+def precompute_attributes(H):
     """
-    Precompute some values on hypergraph HG for faster computing of hypergraph modularity. 
+    Precompute some values on hypergraph HG for faster computing of hypergraph modularity.
     This needs to be run before calling either modularity() or last_step().
 
     Note
     ----
 
-    If HG is unweighted, v.weight is set to 1 for each vertex v in HG. 
+    If HG is unweighted, v.weight is set to 1 for each vertex v in HG.
     The weighted degree for each vertex v is stored in v.strength.
     The total edge weigths for each edge cardinality is stored in HG.d_weights.
     Binomial coefficients to speed-up modularity computation are stored in HG.bin_coef.
     Isolated vertices found only in edge(s) of size 1 are dropped.
 
     Parameters
     ----------
     HG : Hypergraph
 
     Returns
     -------
     H : Hypergraph
-      New hypergraph with added attributes 
+      New hypergraph with added attributes
 
     """
-    H = HG.remove_singletons()
     # 1. compute node strenghts (weighted degrees)
     for v in H.nodes:
         H.nodes[v].strength = 0
     for e in H.edges:
         try:
             w = H.edges[e].weight
         except:
@@ -120,14 +124,15 @@
     bin_coef = {}
     for n in H.d_weights.keys():
         for k in np.arange(n // 2 + 1, n + 1):
             bin_coef[(n, k)] = comb(n, k, exact=True)
     H.bin_coef = bin_coef
     return H
 
+
 ################################################################################
 
 
 def linear(d, c):
     """
     Hyperparameter for hypergraph modularity [2]_ for d-edge with c vertices in the majority class.
     This is the default choice for modularity() and last_step() functions.
@@ -142,19 +147,20 @@
     Returns
     -------
     : float
       c/d if c>d/2 else 0
     """
     return c / d if c > d / 2 else 0
 
+
 # majority
 
 
 def majority(d, c):
-    """    
+    """
     Hyperparameter for hypergraph modularity [2]_ for d-edge with c vertices in the majority class.
     This corresponds to the majority rule [3]_
 
     Parameters
     ----------
     d : int
         Number of vertices in an edge
@@ -165,14 +171,15 @@
     -------
     : bool
       1 if c>d/2 else 0
 
     """
     return 1 if c > d / 2 else 0
 
+
 # strict
 
 
 def strict(d, c):
     """
     Hyperparameter for hypergraph modularity [2]_ for d-edge with c vertices in the majority class.
     This corresponds to the strict rule [3]_
@@ -187,14 +194,15 @@
     Returns
     -------
     : bool
       1 if c==d else 0
     """
     return 1 if c == d else 0
 
+
 #########################################
 
 
 def _compute_partition_probas(HG, A):
     """
     Compute vol(A_i)/vol(V) for each part A_i in A (list of sets)
 
@@ -216,15 +224,15 @@
         p.append(vol)
     s = sum(p)
     return [i / s for i in p]
 
 
 def _degree_tax(HG, Pr, wdc):
     """
-    Computes the expected fraction of edges falling in 
+    Computes the expected fraction of edges falling in
     the partition as per [2]_
 
     Parameters
     ----------
     HG : Hypergraph
 
     Pr : list
@@ -238,15 +246,15 @@
 
     """
     DT = 0
     for d in HG.d_weights.keys():
         tax = 0
         for c in np.arange(d // 2 + 1, d + 1):
             for p in Pr:
-                tax += p**c * (1 - p)**(d - c) * HG.bin_coef[(d, c)] * wdc(d, c)
+                tax += p**c * (1 - p) ** (d - c) * HG.bin_coef[(d, c)] * wdc(d, c)
         tax *= HG.d_weights[d]
         DT += tax
     DT /= HG.total_weight
     return DT
 
 
 def _edge_contribution(HG, A, wdc):
@@ -268,19 +276,22 @@
     : float
 
     """
     EC = 0
     for e in HG.edges:
         d = HG.size(e)
         for part in A:
-            if HG.size(e, part) > d / 2:
-                EC += wdc(d, HG.size(e, part)) * HG.edges[e].weight
+            hgs = HG.size(e, part)
+            if hgs > d / 2:
+                EC += wdc(d, hgs) * HG.edges[e].weight
+                break
     EC /= HG.total_weight
     return EC
 
+
 # HG: HNX hypergraph
 # A: partition (list of sets)
 # wcd: weight function (ex: strict, majority, linear)
 
 
 def modularity(HG, A, wdc=linear):
     """
@@ -289,29 +300,30 @@
     Parameters
     ----------
     HG : Hypergraph
         The hypergraph with some precomputed attributes via: precompute_attributes(HG)
     A : list of sets
         Partition of the vertices in HG
     wdc : func, optional
-        Hyperparameter for hypergraph modularity [2]_ 
+        Hyperparameter for hypergraph modularity [2]_
 
     Note
     ----
     For 'wdc', any function of the format w(d,c) that returns 0 when c <= d/2 and value in [0,1] otherwise can be used.
     Default is 'linear'; other supplied choices are 'majority' and 'strict'.
 
     Returns
     -------
     : float
       The modularity function for partition A on HG
     """
     Pr = _compute_partition_probas(HG, A)
     return _edge_contribution(HG, A, wdc) - _degree_tax(HG, Pr, wdc)
 
+
 ################################################################################
 
 
 def two_section(HG):
     """
     Creates a random walk based [1]_ 2-section igraph Graph with transition weights defined by the
     weights of the hyperedges.
@@ -331,21 +343,22 @@
         # random-walk 2-section (preserve nodes' weighted degrees)
         if len(E) > 1:
             try:
                 w = HG.edges[e].weight / (len(E) - 1)
             except:
                 w = 1 / (len(E) - 1)
             s.extend([(k[0], k[1], w) for k in itertools.combinations(E, 2)])
-    G = ig.Graph.TupleList(s, weights=True).simplify(combine_edges='sum')
+    G = ig.Graph.TupleList(s, weights=True).simplify(combine_edges="sum")
     return G
 
+
 ################################################################################
 
 
-def kumar(HG, delta=.01):
+def kumar(HG, delta=0.01):
     """
     Compute a partition of the vertices in hypergraph HG as per Kumar's algorithm [1]_
 
     Parameters
     ----------
     HG : Hypergraph
 
@@ -355,49 +368,56 @@
     Returns
     -------
     : list of sets
        A partition of the vertices in HG
 
     """
     # weights will be modified -- store initial weights
-    W = {e: HG.edges[e].weight for e in HG.edges}  # uses edge id for reference instead of int
+    W = {
+        e: HG.edges[e].weight for e in HG.edges
+    }  # uses edge id for reference instead of int
     # build graph
     G = two_section(HG)
     # apply clustering
-    CG = G.community_multilevel(weights='weight')
+    CG = G.community_multilevel(weights="weight")
     CH = []
     for comm in CG.as_cover():
-        CH.append(set([G.vs[x]['name'] for x in comm]))
+        CH.append(set([G.vs[x]["name"] for x in comm]))
 
     # LOOP
     diff = 1
     ctr = 0
     while diff > delta:
         # re-weight
         diff = 0
         for e in HG.edges:
             edge = HG.edges[e]
-            reweight = sum([1 / (1 + HG.size(e, c)) for c in CH]) * (HG.size(e) + len(CH)) / HG.number_of_edges()
+            reweight = (
+                sum([1 / (1 + HG.size(e, c)) for c in CH])
+                * (HG.size(e) + len(CH))
+                / HG.number_of_edges()
+            )
             diff = max(diff, 0.5 * abs(edge.weight - reweight))
             edge.weight = 0.5 * edge.weight + 0.5 * reweight
         # re-run louvain
         # build graph
         G = two_section(HG)
         # apply clustering
-        CG = G.community_multilevel(weights='weight')
+        CG = G.community_multilevel(weights="weight")
         CH = []
         for comm in CG.as_cover():
-            CH.append(set([G.vs[x]['name'] for x in comm]))
+            CH.append(set([G.vs[x]["name"] for x in comm]))
         ctr += 1
         if ctr > 50:  # this process sometimes gets stuck -- set limit
             break
-    G.vs['part'] = CG.membership
+    G.vs["part"] = CG.membership
     for e in HG.edges:
         HG.edges[e].weight = W[e]
-    return dict2part({v['name']: v['part'] for v in G.vs})
+    return dict2part({v["name"]: v["part"] for v in G.vs})
+
 
 ################################################################################
 
 
 def _delta_ec(HG, P, v, a, b, wdc):
     """
     Computes change in edge contribution --
@@ -421,19 +441,25 @@
     Returns
     -------
     : float
     """
     Pm = P[a] - {v}
     Pn = P[b].union({v})
     ec = 0
-    for e in list(HG.nodes[v].memberships):
+
+    # TODO: Verify the data shape of `memberships` (ie. what are the keys and values)
+    for e in list(HG.nodes.memberships[v]):
         d = HG.size(e)
         w = HG.edges[e].weight
-        ec += w * (wdc(d, HG.size(e, Pm)) + wdc(d, HG.size(e, Pn))
-                   - wdc(d, HG.size(e, P[a])) - wdc(d, HG.size(e, P[b])))
+        ec += w * (
+            wdc(d, HG.size(e, Pm))
+            + wdc(d, HG.size(e, Pn))
+            - wdc(d, HG.size(e, P[a]))
+            - wdc(d, HG.size(e, P[b]))
+        )
     return ec / HG.total_weight
 
 
 def _bin_ppmf(d, c, p):
     """
     exponential part of the binomial pmf
 
@@ -447,15 +473,15 @@
 
 
     Returns
     -------
     : float
 
     """
-    return p**c * (1 - p)**(d - c)
+    return p**c * (1 - p) ** (d - c)
 
 
 def _delta_dt(HG, P, v, a, b, wdc):
     """
     Compute change in degree tax --
     partition P (list), node v going from P[a] to P[b]
 
@@ -488,21 +514,29 @@
     vola /= vol
     volb /= vol
     DT = 0
 
     for d in HG.d_weights.keys():
         x = 0
         for c in np.arange(int(np.floor(d / 2)) + 1, d + 1):
-            x += HG.bin_coef[(d, c)] * wdc(d, c) * (_bin_ppmf(d, c, voln) + _bin_ppmf(d, c, volm)
-                                                    - _bin_ppmf(d, c, vola) - _bin_ppmf(d, c, volb))
+            x += (
+                HG.bin_coef[(d, c)]
+                * wdc(d, c)
+                * (
+                    _bin_ppmf(d, c, voln)
+                    + _bin_ppmf(d, c, volm)
+                    - _bin_ppmf(d, c, vola)
+                    - _bin_ppmf(d, c, volb)
+                )
+            )
         DT += x * HG.d_weights[d]
     return DT / HG.total_weight
 
 
-def last_step(HG, L, wdc=linear, delta=.01):
+def last_step(HG, L, wdc=linear, delta=0.01):
     """
     Given some initial partition L, compute a new partition of the vertices in HG as per Last-Step algorithm [2]_
 
     Note
     ----
     This is a very simple algorithm that tries moving nodes between communities to improve hypergraph modularity.
     It requires an initial non-trivial partition which can be obtained for example via graph clustering on the 2-section of HG,
@@ -512,18 +546,18 @@
     ----------
     HG : Hypergraph
 
     L : list of sets
       some initial partition of the vertices in HG
 
     wdc : func, optional
-        Hyperparameter for hypergraph modularity [2]_ 
+        Hyperparameter for hypergraph modularity [2]_
 
     delta : float, optional
-            convergence stopping criterion    
+            convergence stopping criterion
 
     Returns
     -------
     : list of sets
       A new partition for the vertices in HG
     """
     A = L[:]  # we will modify this, copy
@@ -535,21 +569,25 @@
             s = list(set([c] + [D[i] for i in HG.neighbors(v)]))
             M = []
             if len(s) > 0:
                 for i in s:
                     if c == i:
                         M.append(0)
                     else:
-                        M.append(_delta_ec(HG, A, v, c, i, wdc) - _delta_dt(HG, A, v, c, i, wdc))
+                        M.append(
+                            _delta_ec(HG, A, v, c, i, wdc)
+                            - _delta_dt(HG, A, v, c, i, wdc)
+                        )
                 i = s[np.argmax(M)]
                 if c != i:
                     A[c] = A[c] - {v}
                     A[i] = A[i].union({v})
                     D[v] = i
         Pr = _compute_partition_probas(HG, A)
         q2 = _edge_contribution(HG, A, wdc) - _degree_tax(HG, Pr, wdc)
         if (q2 - qH) < delta:
             break
         qH = q2
     return [a for a in A if len(a) > 0]
 
+
 ################################################################################
```

### Comparing `hypernetx-1.2.5/hypernetx/algorithms/laplacians_clustering.py` & `hypernetx-2.0.0/hypernetx/algorithms/laplacians_clustering.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,46 @@
 # Copyright © 2021 Battelle Memorial Institute
 # All rights reserved.
 
 """
 
 Hypergraph Probability Transition Matrices, Laplacians, and Clustering
 ======================================================================
-We contruct hypergraph random walks utilizing optional "edge-dependent vertex weights", which are 
+We contruct hypergraph random walks utilizing optional "edge-dependent vertex weights", which are
 weights associated with each vertex-hyperedge pair (i.e. cell weights on the incidence matrix).
-The probability transition matrix of this random walk is used to construct a normalized Laplacian 
+The probability transition matrix of this random walk is used to construct a normalized Laplacian
 matrix for the hypergraph. That normalized Laplacian then serves as the input for a spectral clustering
 algorithm. This spectral clustering algorithm, as well as the normalized Laplacian and other details of
-this methodology are described in 
+this methodology are described in
 
-K. Hayashi, S. Aksoy, C. Park, H. Park, "Hypergraph random walks, Laplacians, and clustering", 
+K. Hayashi, S. Aksoy, C. Park, H. Park, "Hypergraph random walks, Laplacians, and clustering",
 Proceedings of the 29th ACM International Conference on Information & Knowledge Management. 2020.
 https://doi.org/10.1145/3340531.3412034
 
 Please direct any inquiries concerning the clustering module to Sinan Aksoy, sinan.aksoy@pnnl.gov
 
 """
 
 import numpy as np
-from collections import defaultdict
-import networkx as nx
-import warnings
 import sys
-from scipy.sparse import csr_matrix, coo_matrix, diags, find, identity
+from scipy.sparse import csr_matrix, diags, identity
 from scipy.sparse.linalg import eigs
-from sklearn.cluster import SpectralClustering, KMeans
+from sklearn.cluster import KMeans
 from sklearn import preprocessing
-from functools import partial
 from hypernetx import HyperNetXError
 
 try:
     import nwhy
 
     nwhy_available = True
 except:
     nwhy_available = False
 
 sys.setrecursionlimit(10000)
 
-__all__ = [
-    "prob_trans",
-    "get_pi",
-    "norm_lap",
-    "spec_clus",
-]
-
 
 def prob_trans(H, weights=False, index=True, check_connected=True):
     """
     The probability transition matrix of a random walk on the vertices of a hypergraph.
     At each step in the walk, the next vertex is chosen by:
 
     1. Selecting a hyperedge e containing the vertex with probability proportional to w(e)
@@ -74,27 +63,25 @@
     index : bool, optional
         Whether to return matrix index to vertex label mapping
 
     Returns
     -------
      P : scipy.sparse.csr.csr_matrix
          Probability transition matrix of the random walk on the hypergraph
-     index: dict
-         mapping from row and column indices to corresponding vertex label
+     index: list
+         contains list of index of node ids for rows
     """
     # hypergraph must be connected
     if check_connected:
         if not H.is_connected():
             raise HyperNetXError("hypergraph must be connected")
 
-    # if no weighting function, each step in the random walk is chosen uniformly at random.
-    if weights == False:
-        R, index, _ = H.incidence_matrix(index=True)
-    else:
-        R, index, _ = H.incidence_matrix(index=True, weights=True)
+    R = H.incidence_matrix(index=index, weights=weights)
+    if index:
+        R, rdx, _ = R
 
     # transpose incidence matrix for notational convenience
     R = R.transpose()
 
     # generates hyperedge weight matrix, has same nonzero pattern as incidence matrix,
     # with values determined by the edge-dependent vertex weight standard deviation
     edgeScore = {
@@ -111,18 +98,17 @@
 
     [rowSums] = W.sum(axis=1).flatten().tolist()
     D_V = diags([1 / x for x in rowSums])
 
     # probability transition matrix P
     P = D_V * W * D_E * R
 
-    if index == False:
-        return P
-    else:
-        return P, index
+    if index:
+        return P, rdx
+    return P
 
 
 def get_pi(P):
     """
     Returns the eigenvector corresponding to the largest eigenvalue (in magnitude),
     normalized so its entries sum to 1. Intended for the probability transition matrix
     of a random walk on a (connected) hypergraph, in which case the output can
@@ -170,29 +156,28 @@
     index : bool, optional
         Whether to return matrix-index to vertex-label mapping
 
     Returns
     -------
      P : scipy.sparse.csr.csr_matrix
          Probability transition matrix of the random walk on the hypergraph
-     index: dict
-         mapping from row and column indices to corresponding vertex label
+     id: list
+         contains list of index of node ids for rows
     """
-    if weights == None:
-        P, index = prob_trans(H)
-    else:
-        P, index = prob_trans(H, weights=weights)
+    P = prob_trans(H, weights=weights, index=index)
+    if index:
+        P, idx = P
+
     pi = get_pi(P)
     gamma = diags(np.power(pi, 1 / 2)) * P * diags(np.power(pi, -1 / 2))
-    L = identity(gamma.shape[0]) - (1 / 2) * gamma + gamma.transpose()
+    L = identity(gamma.shape[0]) - (1 / 2) * (gamma + gamma.transpose())
 
     if index:
-        return L, index
-    else:
-        return L
+        return L, idx
+    return L
 
 
 def spec_clus(H, k, existing_lap=None, weights=False):
     """
     Hypergraph spectral clustering of the vertex set into k disjoint clusters
     using the normalized hypergraph Laplacian. Equivalent to the "RDC-Spec"
     Algorithm 1 in:
```

### Comparing `hypernetx-1.2.5/hypernetx/algorithms/s_centrality_measures.py` & `hypernetx-2.0.0/hypernetx/algorithms/s_centrality_measures.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,48 +7,36 @@
 =====================
 We generalize graph metrics to s-metrics for a hypergraph by using its s-connected
 components. This is accomplished by computing the s edge-adjacency matrix and
 constructing the corresponding graph of the matrix. We then use existing graph metrics
 on this representation of the hypergraph. In essence we construct an *s*-line graph
 corresponding to the hypergraph on which to apply our methods.
 
-S-Metrics for hypergraphs are discussed in depth in:        
+S-Metrics for hypergraphs are discussed in depth in:
 *Aksoy, S.G., Joslyn, C., Ortiz Marrero, C. et al. Hypernetwork science via high-order hypergraph walks.
 EPJ Data Sci. 9, 16 (2020). https://doi.org/10.1140/epjds/s13688-020-00231-0*
 
 """
 
-import numpy as np
-from collections import defaultdict
 import networkx as nx
 import warnings
 import sys
 from functools import partial
 
 try:
     import nwhy
 
     nwhy_available = True
 except:
     nwhy_available = False
 
 sys.setrecursionlimit(10000)
 
-__all__ = [
-    "s_betweenness_centrality",
-    "s_harmonic_closeness_centrality",
-    "s_harmonic_centrality",
-    "s_closeness_centrality",
-    "s_eccentricity",
-]
 
-
-def _s_centrality(
-    func, H, s=1, edges=True, f=None, return_singletons=True, use_nwhy=True, **kwargs
-):
+def _s_centrality(func, H, s=1, edges=True, f=None, return_singletons=True, **kwargs):
     """
     Wrapper for computing s-centrality either in NetworkX or in NWHy
 
     Parameters
     ----------
     func : function
         Function or partial function from NetworkX or NWHy
@@ -58,16 +46,14 @@
         s-width for computation
     edges : bool, optional
         If True, an edge linegraph will be used, otherwise a node linegraph will be used
     f : str, optional
         Identifier of node or edge of interest for computing centrality
     return_singletons : bool, optional
         If True will return 0 value for each singleton in the s-linegraph
-    use_nwhy : bool, optional
-        If True will attempt to use nwhy centrality methods if availaable
     **kwargs
         Centrality metric specific keyword arguments to be passed to func
 
     Returns
     -------
     dict
         dictionary of centrality scores keyed by names
@@ -80,52 +66,33 @@
             if (edges and f in cps.edges) or (not edges and f in cps.nodes):
                 comps = [cps]
                 break
         else:
             return {f: 0}
 
     stats = dict()
-    if H.isstatic:
-        for h in comps:
-            if edges:
-                vertices = h.edges
-            else:
-                vertices = h.nodes
-
-            if h.shape[edges * 1] == 1:
-                stats.update({v: 0 for v in vertices})
-            elif use_nwhy and nwhy_available and h.nwhy:
-                g = h.get_linegraph(s=s, edges=edges, use_nwhy=True)
-                stats.update(dict(zip(vertices, func(g, **kwargs))))
-            else:
-                g = h.get_linegraph(s=s, edges=edges, use_nwhy=False)
-                stats.update(
-                    {
-                        h.get_name(k, edges=edges): v
-                        for k, v in func(g, **kwargs).items()
-                    }
-                )
-            if f:
-                return {f: stats[f]}
-    else:
-        for h in comps:
-            if edges:
-                A, Adict = h.edge_adjacency_matrix(s=s, index=True)
-            else:
-                A, Adict = h.adjacency_matrix(s=s, index=True)
-            g = nx.from_scipy_sparse_matrix(A)
-            stats.update({Adict[k]: v for k, v in func(g, **kwargs).items()})
-            if f:
-                return {f: stats[f]}
+    for h in comps:
+        if edges:
+            vertices = h.edges
+        else:
+            vertices = h.nodes
+
+        if h.shape[edges * 1] == 1:
+            stats = {v: 0 for v in vertices}
+        else:
+            g = h.get_linegraph(s=s, edges=edges)
+            stats.update({k: v for k, v in func(g, **kwargs).items()})
+        if f:
+            return {f: stats[f]}
 
     return stats
 
 
 def s_betweenness_centrality(
-    H, s=1, edges=True, normalized=True, return_singletons=True, use_nwhy=True
+    H, s=1, edges=True, normalized=True, return_singletons=True
 ):
     r"""
     A centrality measure for an s-edge(node) subgraph of H based on shortest paths.
     Equals the betweenness centrality of vertices in the edge(node) s-linegraph.
 
     In a graph (2-uniform hypergraph) the betweenness centrality of a vertex $v$
     is the ratio of the number of non-trivial shortest paths between any pair of
@@ -157,38 +124,31 @@
 
     Returns
     -------
     dict
         A dictionary of s-betweenness centrality value of the edges.
 
     """
-    if use_nwhy and nwhy_available and H.nwhy:
-        func = partial(nwhy.Slinegraph.s_betweenness_centrality, normalized=False)
-    else:
-        use_nwhy = False
-        func = partial(nx.betweenness_centrality, normalized=False)
+    func = partial(nx.betweenness_centrality, normalized=False)
     result = _s_centrality(
         func,
         H,
         s=s,
         edges=edges,
         return_singletons=return_singletons,
-        use_nwhy=use_nwhy,
     )
 
     if normalized and H.shape[edges * 1] > 2:
         n = H.shape[edges * 1]
         return {k: v * 2 / ((n - 1) * (n - 2)) for k, v in result.items()}
     else:
         return result
 
 
-def s_closeness_centrality(
-    H, s=1, edges=True, return_singletons=True, source=None, use_nwhy=True
-):
+def s_closeness_centrality(H, s=1, edges=True, return_singletons=True, source=None):
     r"""
     In a connected component the reciprocal of the sum of the distance between an
     edge(node) and all other edges(nodes) in the component times the number of edges(nodes)
     in the component minus 1.
 
     $V$ = the set of vertices in the linegraph.
     $n = |V|$
@@ -207,57 +167,49 @@
 
     edges : bool, optional
         Indicates if method should compute edge linegraph (default) or node linegraph.
     return_singletons : bool, optional
         Indicates if method should return values for singleton components.
     source : str, optional
         Identifier of node or edge of interest for computing centrality
-    use_nwhy : bool, optional
-        If true will use the :ref:`NWHy library <nwhy>` if available.
 
     Returns
     -------
     dict or float
         returns the s-closeness centrality value of the edges(nodes).
         If source=None a dictionary of values for each s-edge in H is returned.
         If source then a single value is returned.
     """
-    if use_nwhy and nwhy_available and H.nwhy:
-        func = partial(nwhy.Slinegraph.s_closeness_centrality)
-    else:
-        use_nwhy = False
-        func = partial(nx.closeness_centrality)
+    func = partial(nx.closeness_centrality)
     return _s_centrality(
         func,
         H,
         s=s,
         edges=edges,
         return_singletons=return_singletons,
         f=source,
-        use_nwhy=use_nwhy,
     )
 
 
-def s_harmonic_closeness_centrality(H, s=1, edge=None, use_nwhy=True):
+def s_harmonic_closeness_centrality(H, s=1, edge=None):
     msg = """
-    s_harmonic_closeness_centrality is being replaced with s_harmonic_centrality 
-    and will not be available in future releases. 
+    s_harmonic_closeness_centrality is being replaced with s_harmonic_centrality
+    and will not be available in future releases.
     """
     warnings.warn(msg)
     return s_harmonic_centrality(H, s=s, edges=True, normalized=True, source=edge)
 
 
 def s_harmonic_centrality(
     H,
     s=1,
     edges=True,
     source=None,
     normalized=False,
     return_singletons=True,
-    use_nwhy=True,
 ):
     r"""
     A centrality measure for an s-edge subgraph of H. A value equal to 1 means the s-edge
     intersects every other s-edge in H. All values range between 0 and 1.
     Edges of size less than s return 0. If H contains only one s-edge a 0 is returned.
 
     The denormalized reciprocal of the harmonic mean of all distances from $u$ to all other vertices.
@@ -280,54 +232,59 @@
 
     edges : bool, optional
         Indicates if method should compute edge linegraph (default) or node linegraph.
     return_singletons : bool, optional
         Indicates if method should return values for singleton components.
     source : str, optional
         Identifier of node or edge of interest for computing centrality
-    use_nwhy : bool, optional
-        If true will use the :ref:`NWHy library <nwhy>` if available.
 
     Returns
     -------
     dict or float
         returns the s-harmonic closeness centrality value of the edges, a number between 0 and 1 inclusive.
         If source=None a dictionary of values for each s-edge in H is returned.
         If source then a single value is returned.
 
     """
 
-    if use_nwhy and nwhy_available and H.nwhy:
-        func = partial(nwhy.Slinegraph.s_harmonic_closeness_centrality)
-    else:
-        use_nwhy = False
-        func = partial(nx.harmonic_centrality)
-    result = _s_centrality(
-        func,
-        H,
-        s=s,
-        edges=edges,
-        return_singletons=return_singletons,
-        f=source,
-        use_nwhy=use_nwhy,
-    )
+    # func = partial(nx.harmonic_centrality)
+    # result = _s_centrality(
+    #     func,
+    #     H,
+    #     s=s,
+    #     edges=edges,
+    #     return_singletons=return_singletons,
+    #     f=source,
+    # )
+    g = H.get_linegraph(s=s, edges=edges)
+    result = nx.harmonic_centrality(g)
 
     if normalized and H.shape[edges * 1] > 2:
         n = H.shape[edges * 1]
-        return {k: v * 2 / ((n - 1) * (n - 2)) for k, v in result.items()}
+        factor = 2 / ((n - 1) * (n - 2))
     else:
-        return result
+        factor = 1
+
+    if source:
+        return result[source] * factor
+    else:
+        return {k: v * factor for k, v in result.items()}
 
+    # if normalized and H.shape[edges * 1] > 2:
+    #     n = H.shape[edges * 1]
+    #     result = {k: v * 2 / ((n - 1) * (n - 2)) for k, v in result.items()}
+    # else:
+    #     return result
 
-def s_eccentricity(
-    H, s=1, edges=True, source=None, return_singletons=True, use_nwhy=True
-):
+
+def s_eccentricity(H, s=1, edges=True, source=None, return_singletons=True):
     r"""
-    The length of the longest shortest path from a vertex $u$ to every other vertex in the linegraph.
-    $V$ = set of vertices in the linegraph
+    The length of the longest shortest path from a vertex $u$ to every other vertex in
+    the s-linegraph.
+    $V$ = set of vertices in the s-linegraph
     $d$ = shortest path distance
 
     .. math::
 
         \text{s-ecc}(u) = \text{max}\{d(u,v): v \in V\}
 
     Parameters
@@ -338,43 +295,44 @@
 
     edges : bool, optional
         Indicates if method should compute edge linegraph (default) or node linegraph.
     return_singletons : bool, optional
         Indicates if method should return values for singleton components.
     source : str, optional
         Identifier of node or edge of interest for computing centrality
-    use_nwhy : bool, optional
-        If true will use the :ref:`NWHy library <nwhy>` if available.
 
     Returns
     -------
     dict or float
         returns the s-eccentricity value of the edges(nodes).
         If source=None a dictionary of values for each s-edge in H is returned.
         If source then a single value is returned.
+        If the s-linegraph is disconnected, np.inf is returned.
 
     """
-    if use_nwhy and nwhy_available and H.nwhy:
-        func = nwhy.Slinegraph.s_eccentricity
-    else:
-        use_nwhy = False
-        func = nx.eccentricity
 
-    if source is not None:
-        return _s_centrality(
-            func,
-            H,
-            s=s,
-            edges=edges,
-            f=source,
-            return_singletons=return_singletons,
-            use_nwhy=use_nwhy,
-        )
+    g = H.get_linegraph(s=s, edges=edges)
+    result = nx.eccentricity(g)
+    if source:
+        return result[source]
     else:
-        return _s_centrality(
-            func,
-            H,
-            s=s,
-            edges=edges,
-            return_singletons=return_singletons,
-            use_nwhy=use_nwhy,
-        )
+        return result
+
+    # func = nx.eccentricity
+
+    # if source is not None:
+    #     return _s_centrality(
+    #         func,
+    #         H,
+    #         s=s,
+    #         edges=edges,
+    #         f=source,
+    #         return_singletons=return_singletons,
+    #     )
+    # else:
+    #     return _s_centrality(
+    #         func,
+    #         H,
+    #         s=s,
+    #         edges=edges,
+    #         return_singletons=return_singletons,
+    #     )
```

### Comparing `hypernetx-1.2.5/hypernetx/classes/hypergraph.py` & `hypernetx-2.0.0/hypernetx/classes/hypergraph.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,321 +1,685 @@
 # Copyright © 2018 Battelle Memorial Institute
 # All rights reserved.
+from __future__ import annotations
 
-import warnings
 import pickle
+import warnings
+from collections import defaultdict
+from collections.abc import Sequence, Iterable
+from typing import Optional, Any, TypeVar, Union, Mapping
+
 import networkx as nx
-from networkx.algorithms import bipartite
 import numpy as np
 import pandas as pd
-from scipy.sparse import issparse, coo_matrix, dok_matrix, csr_matrix
-from collections import OrderedDict, defaultdict
-from hypernetx.classes.entity import Entity, EntitySet
-from hypernetx.classes.staticentity import StaticEntity, StaticEntitySet
-from hypernetx.exception import HyperNetXError
-from hypernetx.utils.decorators import not_implemented_for
+from networkx.algorithms import bipartite
+from scipy.sparse import coo_matrix, csr_matrix
 
+from hypernetx.classes import Entity, EntitySet
+from hypernetx.exception import HyperNetXError
+from hypernetx.utils.decorators import warn_nwhy
+from hypernetx.classes.helpers import merge_nested_dicts, dict_depth
 
 __all__ = ["Hypergraph"]
 
+T = TypeVar("T", bound=Union[str, int])
+
 
 class Hypergraph:
     """
-    Hypergraph H = (V,E) references a pair of disjoint sets:
-    V = nodes (vertices) and E = (hyper)edges.
+    Parameters
+    ----------
+
+    setsystem : (optional) dict of iterables, dict of dicts,iterable of iterables,
+        pandas.DataFrame, numpy.ndarray, default = None
+        See SetSystem above for additional setsystem requirements.
+
+    edge_col : (optional) str | int, default = 0
+        column index (or name) in pandas.dataframe or numpy.ndarray,
+        used for (hyper)edge ids. Will be used to reference edgeids for
+        all set systems.
+
+    node_col : (optional) str | int, default = 1
+        column index (or name) in pandas.dataframe or numpy.ndarray,
+        used for node ids. Will be used to reference nodeids for all set systems.
+
+    cell_weight_col : (optional) str | int, default = None
+        column index (or name) in pandas.dataframe or numpy.ndarray used for
+        referencing cell weights. For a dict of dicts references key in cell
+        property dicts.
+
+    cell_weights : (optional) Sequence[float,int] | int |  float , default = 1.0
+        User specified cell_weights or default cell weight.
+        Sequential values are only used if setsystem is a
+        dataframe or ndarray in which case the sequence must
+        have the same length and order as these objects.
+        Sequential values are ignored for dataframes if cell_weight_col is already
+        a column in the data frame.
+        If cell_weights is assigned a single value
+        then it will be used as default for missing values or when no cell_weight_col
+        is given.
+
+    cell_properties : (optional) Sequence[int | str] | Mapping[T,Mapping[T,Mapping[str,Any]]],
+        default = None
+        Column names from pd.DataFrame to use as cell properties
+        or a dict assigning cell_property to incidence pairs of edges and
+        nodes. Will generate a misc_cell_properties, which may have variable lengths per cell.
+
+    misc_cell_properties : (optional) str | int, default = None
+        Column name of dataframe corresponding to a column of variable
+        length property dictionaries for the cell. Ignored for other setsystem
+        types.
+
+    aggregateby : (optional) str, dict, default = 'first'
+        By default duplicate edge,node incidences will be dropped unless
+        specified with `aggregateby`.
+        See pandas.DataFrame.agg() methods for additional syntax and usage
+        information.
+
+    edge_properties : (optional) pd.DataFrame | dict, default = None
+        Properties associated with edge ids.
+        First column of dataframe or keys of dict link to edge ids in
+        setsystem.
+
+    node_properties : (optional) pd.DataFrame | dict, default = None
+        Properties associated with node ids.
+        First column of dataframe or keys of dict link to node ids in
+        setsystem.
+
+    properties : (optional) pd.DataFrame | dict, default = None
+        Concatenation/union of edge_properties and node_properties.
+        By default, the object id is used and should be the first column of
+        the dataframe, or key in the dict. If there are nodes and edges
+        with the same ids and different properties then use the edge_properties
+        and node_properties keywords.
+
+    misc_properties : (optional) int | str, default = None
+        Column of property dataframes with dtype=dict. Intended for variable
+        length property dictionaries for the objects.
+
+    edge_weight_prop : (optional) str, default = None,
+        Name of property in edge_properties to use for weight.
+
+    node_weight_prop : (optional) str, default = None,
+        Name of property in node_properties to use for weight.
+
+    weight_prop : (optional) str, default = None
+        Name of property in properties to use for 'weight'
+
+    default_edge_weight : (optional) int | float, default = 1
+        Used when edge weight property is missing or undefined.
+
+    default_node_weight : (optional) int | float, default = 1
+        Used when node weight property is missing or undefined
+
+    name : (optional) str, default = None
+        Name assigned to hypergraph
+
+
+    ======================
+    Hypergraphs in HNX 2.0
+    ======================
 
-    An HNX Hypergraph is either dynamic or static.
-    Dynamic hypergraphs can change by adding or subtracting objects
-    from them. Static hypergraphs require that all of the nodes and edges
-    be known at creation. A hypergraph is dynamic by default.
-
-    *Dynamic hypergraphs* require the user to keep track of its objects,
-    by using a unique names for each node and edge. This allows for multi-edge graphs and
-    inseperable nodes.
-
-    For example: Let V = {1,2,3} and E = {e1,e2,e3},
-    where e1 = {1,2}, e2 = {1,2}, and e3 = {1,2,3}.
-    The edges e1 and e2 contain the same set of nodes and yet
-    are distinct and must be distinguishable within H.
-
-    In a dynamic hypergraph each node and edge is
-    instantiated as an Entity and given an identifier or uid. Entities
-    keep track of inclusion relationships and can be nested. Since
-    hypergraphs can be quite large, only the entity identifiers will be used
-    for computation intensive methods, this means the user must take care
-    to keep a one to one correspondence between their set of uids and
-    the objects in their hypergraph. See `Honor System`_
-    Dynamic hypergraphs are most practical for small to modestly sized
-    hypergraphs (<1000 objects).
-
-    *Static hypergraphs* store node and edge information in numpy arrays and
-    are immutable. Each node and edge receives a class generated internal
-    identifier used for computations so do not require the user to create
-    different ids for nodes and edges. To create a static hypergraph set
-    `static = True` in the signature.
-
-    We will create hypergraphs in multiple ways:
-
-    1. As an empty instance: ::
-
-        >>> H = hnx.Hypergraph()
-        >>> H.nodes, H.edges
-        ({}, {})
-
-    2. From a dictionary of iterables (elements of iterables must be of type hypernetx.Entity or hashable): ::
-
-        >>> H = Hypergraph({'a':[1,2,3],'b':[4,5,6]})
-        >>> H.nodes, H.edges
-        # output: (EntitySet(_:Nodes,[1, 2, 3, 4, 5, 6],{}), EntitySet(_:Edges,['b', 'a'],{}))
-
-    3. From an iterable of iterables: (elements of iterables must be of type hypernetx.Entity or hashable): ::
-
-        >>> H = Hypergraph([{'a','b'},{'b','c'},{'a','c','d'}])
-        >>> H.nodes, H.edges
-        # output: (EntitySet(_:Nodes,['d', 'b', 'c', 'a'],{}), EntitySet(_:Edges,['_1', '_2', '_0'],{}))
-
-    4. From a hypernetx.EntitySet or StaticEntitySet: ::
-
-        >>> a = Entity('a',{1,2}); b = Entity('b',{2,3})
-        >>> E = EntitySet('sample',elements=[a,b])
-        >>> H = Hypergraph(E)
-        >>> H.nodes, H.edges.
-        # output: (EntitySet(_:Nodes,[1, 2, 3],{}), EntitySet(_:Edges,['b', 'a'],{}))
-
-    All of these constructions apply for both dynamic and static hypergraphs. To
-    create a static hypergraph set the parameter `static=True`. In addition a static
-    hypergraph is automatically created if a StaticEntity, StaticEntitySet, or pandas.DataFrame object
-    is passed to the Hypergraph constructor.
-
-    5. | From a pandas.DataFrame. The dataframe must have at least two columns with headers and there can be no nans.
-       | By default the first column corresponds to the edge names and the second column to the node names.
-       | You can specify the columns by restricting the dataframe to the columns of interest in the order:
-       | :code:`hnx.Hypergraph(df[[edge_column_name,node_column_name]])`
-       | See :ref:`Colab Tutorials <colab>`  Tutorial 6 - Static Hypergraphs and Entities for additional information.
+    An hnx.Hypergraph H = (V,E) references a pair of disjoint sets:
+    V = nodes (vertices) and E = (hyper)edges.
 
+    HNX allows for multi-edges by distinguishing edges by
+    their identifiers instead of their contents. For example, if
+    V = {1,2,3} and E = {e1,e2,e3},
+    where e1 = {1,2}, e2 = {1,2}, and e3 = {1,2,3},
+    the edges e1 and e2 contain the same set of nodes and yet
+    are distinct and are distinguishable within H = (V,E).
+
+    New as of version 2.0, HNX provides methods to easily store and
+    access additional metadata such as cell, edge, and node weights.
+    Metadata associated with (edge,node) incidences
+    are referenced as **cell_properties**.
+    Metadata associated with a single edge or node is referenced
+    as its **properties**.
+
+    The fundamental object needed to create a hypergraph is a **setsystem**. The
+    setsystem defines the many-to-many relationships between edges and nodes in
+    the hypergraph. Cell properties for the incidence pairs can be defined within
+    the setsystem or in a separate pandas.Dataframe or dict.
+    Edge and node properties are defined with a pandas.DataFrame or dict.
 
-    Parameters
+    SetSystems
     ----------
-    setsystem : (optional) EntitySet, StaticEntitySet, dict, iterable, pandas.dataframe, default: None
-        See notes above for setsystem requirements.
-    name : hashable, optional, default: None
-        If None then a placeholder '_'  will be inserted as name
-    static : boolean, optional, default: False
-        If True the hypergraph will be immutable, edges and nodes may not be changed.
-    weights : array-like, optional, default : None
-        User specified weights corresponding to setsytem of type pandas.DataFrame,
-        length must equal number of rows in dataframe.
-        If None, weight for all rows is assumed to be 1.
-    keep_weights : bool, optional, default : True
-        Whether or not to use existing weights when input is StaticEntity, or StaticEntitySet.
-    aggregateby : str, optional, {'count', 'sum', 'mean', 'median', max', 'min', 'first','last', None}, default : 'sum'
-        Method to aggregate cell_weights of duplicate rows if setsystem  is of type pandas.DataFrame or
-        StaticEntity. If None all cell weights will be set to 1.
-    use_nwhy : boolean, optional, default : False
-        If True hypergraph will be static and computations will be done using
-        C++ backend offered by NWHypergraph. This requires installation of the
-        NWHypergraph C++ library. Please see the :ref:`NWHy documentation <nwhy>` for more information.
-    filepath : str, optional, default : None
+    There are five types of setsystems currently accepted by the library.
 
-    """
+    1.  **iterable of iterables** : Barebones hypergraph uses Pandas default
+        indexing to generate hyperedge ids. Elements must be hashable.: ::
+
+        >>> H = Hypergraph([{1,2},{1,2},{1,2,3}])
 
-    # TODO: remove lambda functions from constructor in H and E.
+    2.  **dictionary of iterables** : the most basic way to express many-to-many
+        relationships providing edge ids. The elements of the iterables must be
+        hashable): ::
+
+        >>> H = Hypergraph({'e1':[1,2],'e2':[1,2],'e3':[1,2,3]})
+
+    3.  **dictionary of dictionaries**  : allows cell properties to be assigned
+        to a specific (edge, node) incidence. This is particularly useful when
+        there are variable length dictionaries assigned to each pair: ::
+
+        >>> d = {'e1':{ 1: {'w':0.5, 'name': 'related_to'},
+        >>>             2: {'w':0.1, 'name': 'related_to',
+        >>>                 'startdate': '05.13.2020'}},
+        >>>      'e2':{ 1: {'w':0.52, 'name': 'owned_by'},
+        >>>             2: {'w':0.2}},
+        >>>      'e3':{ 1: {'w':0.5, 'name': 'related_to'},
+        >>>             2: {'w':0.2, 'name': 'owner_of'},
+        >>>             3: {'w':1, 'type': 'relationship'}}
+
+        >>> H = Hypergraph(d, cell_weight_col='w')
+
+    4.  **pandas.DataFrame** For large datasets and for datasets with cell
+        properties it is most efficient to construct a hypergraph directly from
+        a pandas.DataFrame. Incidence pairs are in the first two columns.
+        Cell properties shared by all incidence pairs can be placed in their own
+        column of the dataframe. Variable length dictionaries of cell properties
+        particular to only some of the incidence pairs may be placed in a single
+        column of the dataframe. Representing the data above as a dataframe df:
+
+        +-----------+-----------+-----------+-----------------------------------+
+        |   col1    |   col2    |   w       |  col3                             |
+        +-----------+-----------+-----------+-----------------------------------+
+        |   e1      |   1       |   0.5     | {'name':'related_to'}             |
+        +-----------+-----------+-----------+-----------------------------------+
+        |   e1      |   2       |   0.1     | {"name":"related_to",             |
+        |           |           |           |  "startdate":"05.13.2020"}        |
+        +-----------+-----------+-----------+-----------------------------------+
+        |   e2      |   1       |   0.52    | {"name":"owned_by"}               |
+        +-----------+-----------+-----------+-----------------------------------+
+        |   e2      |   2       |   0.2     |                                   |
+        +-----------+-----------+-----------+-----------------------------------+
+        |   ...     |   ...     |   ...     | {...}                             |
+        +-----------+-----------+-----------+-----------------------------------+
+
+        The first row of the dataframe is used to reference each column. ::
+
+        >>> H = Hypergraph(df,edge_col="col1",node_col="col2",
+        >>>                 cell_weight_col="w",misc_cell_properties="col3")
+
+    5.  **numpy.ndarray** For homogeneous datasets given in an ndarray a
+        pandas dataframe is generated and column names are added from the
+        edge_col and node_col arguments. Cell properties containing multiple data
+        types are added with a separate dataframe or dict and passed through the
+        cell_properties keyword. ::
+
+        >>> arr = np.array([['e1','1'],['e1','2'],
+        >>>                 ['e2','1'],['e2','2'],
+        >>>                 ['e3','1'],['e3','2'],['e3','3']])
+        >>> H = hnx.Hypergraph(arr, column_names=['col1','col2'])
+
+
+    Edge and Node Properties
+    ------------------------
+    Properties specific to a single edge or node are passed through the
+    keywords: **edge_properties, node_properties, properties**.
+    Properties may be passed as dataframes or dicts.
+    The first column or index of the dataframe or keys of the dict keys
+    correspond to the edge and/or node identifiers.
+    If identifiers are shared among edges and nodes, or are distinct
+    for edges and nodes, properties may be combined into a single
+    object and passed to the **properties** keyword. For example:
+
+    +-----------+-----------+---------------------------------------+
+    |   id      |   weight  |   properties                          |
+    +-----------+-----------+---------------------------------------+
+    |   e1      |   5.0     |   {'type':'event'}                    |
+    +-----------+-----------+---------------------------------------+
+    |   e2      |   0.52    |   {"name":"owned_by"}                 |
+    +-----------+-----------+---------------------------------------+
+    |   ...     |   ...     |   {...}                               |
+    +-----------+-----------+---------------------------------------+
+    |   1       |   1.2     |   {'color':'red'}                     |
+    +-----------+-----------+---------------------------------------+
+    |   2       |   .003    |   {'name':'Fido','color':'brown'}     |
+    +-----------+-----------+---------------------------------------+
+    |   3       |   1.0     |    {}                                 |
+    +-----------+-----------+---------------------------------------+
+
+    A properties dictionary should have the format: ::
+
+        dp = {id1 : {prop1:val1, prop2,val2,...}, id2 : ... }
+
+    A properties dataframe may be used for nodes and edges sharing ids
+    but differing in cell properties by adding a level index using 0
+    for edges and 1 for nodes:
+
+    +-----------+-----------+-----------+---------------------------+
+    |  level    |   id      |   weight  |       properties          |
+    +-----------+-----------+-----------+---------------------------+
+    |   0       |   e1      |   5.0     |   {'type':'event'}        |
+    +-----------+-----------+-----------+---------------------------+
+    |   0       |   e2      |    0.52   |   {"name":"owned_by"}     |
+    +-----------+-----------+-----------+---------------------------+
+    |   ...     |   ...     |    ...    |          {...}            |
+    +-----------+-----------+-----------+---------------------------+
+    |   1       |   1.2     |   {'color':'red'}                     |
+    +-----------+-----------+-----------+---------------------------+
+    |   2       |   .003    |   {'name':'Fido','color':'brown'}     |
+    +-----------+-----------+-----------+---------------------------+
+    |   ...     |   ...     |    ...    |          {...}            |
+    +-----------+-----------+-----------+---------------------------+
+
+
+
+    Weights
+    -------
+    The default key for cell and object weights is "weight". The default value
+    is 1. Weights may be assigned and/or a new default prescribed in the
+    constructor using **cell_weight_col** and **cell_weights** for incidence pairs,
+    and using **edge_weight_prop, node_weight_prop, weight_prop,
+    default_edge_weight,** and **default_node_weight** for node and edge weights.
 
+    """
+
+    @warn_nwhy
     def __init__(
         self,
-        setsystem=None,
-        name=None,
-        static=False,
-        weights=None,
-        aggregateby="sum",
-        use_nwhy=False,
-        filepath=None,
+        setsystem: Optional[
+            pd.DataFrame
+            | np.ndarray
+            | Mapping[T, Iterable[T]]
+            | Iterable[Iterable[T]]
+            | Mapping[T, Mapping[T, Mapping[str, Any]]]
+        ] = None,
+        edge_col: str | int = 0,
+        node_col: str | int = 1,
+        cell_weight_col: Optional[str | int] = "cell_weights",
+        cell_weights: Sequence[float] | float = 1.0,
+        cell_properties: Optional[
+            Sequence[str | int] | Mapping[T, Mapping[T, Mapping[str, Any]]]
+        ] = None,
+        misc_cell_properties_col: Optional[str | int] = None,
+        aggregateby: str | dict[str, str] = "first",
+        edge_properties: Optional[pd.DataFrame | dict[T, dict[Any, Any]]] = None,
+        node_properties: Optional[pd.DataFrame | dict[T, dict[Any, Any]]] = None,
+        properties: Optional[
+            pd.DataFrame | dict[T, dict[Any, Any]] | dict[T, dict[T, dict[Any, Any]]]
+        ] = None,
+        misc_properties_col: Optional[str | int] = None,
+        edge_weight_prop_col: str | int = "weight",
+        node_weight_prop_col: str | int = "weight",
+        weight_prop_col: str | int = "weight",
+        default_edge_weight: Optional[float | None] = None,
+        default_node_weight: Optional[float | None] = None,
+        default_weight: float = 1.0,
+        name: Optional[str] = None,
+        **kwargs,
     ):
-        self.filepath = filepath
-        if use_nwhy:
-            static = True
-            try:
-                import nwhy
-
-                self.nwhy = True
-
-            except:
-                self.nwhy = False
-                print("NWHypergraph is not available. Will continue with static=True.")
-                use_nwhy = False
-        else:
-            self.nwhy = False
-        if not name:
-            self.name = ""
-        else:
-            self.name = name
+        self.name = name or ""
+        self.misc_cell_properties_col = misc_cell_properties = (
+            misc_cell_properties_col or "cell_properties"
+        )
+        self.misc_properties_col = misc_properties_col = (
+            misc_properties_col or "properties"
+        )
+        self.default_edge_weight = default_edge_weight = (
+            default_edge_weight or default_weight
+        )
+        self.default_node_weight = default_node_weight = (
+            default_node_weight or default_weight
+        )
+        ### cell properties
 
-        if static == True or (
-            isinstance(setsystem, StaticEntitySet)
-            or isinstance(setsystem, StaticEntity)
-            or isinstance(setsystem, pd.DataFrame)
-        ):
-            self._static = True
-            if setsystem is None:
-                self._edges = StaticEntitySet()
-                self._nodes = StaticEntitySet()
-            else:
-                if weights is not None:
-                    E = StaticEntitySet(
-                        entity=setsystem, weights=weights, aggregateby=aggregateby
+        if setsystem is None:  #### Empty Case
+
+            self._edges = EntitySet({})
+            self._nodes = EntitySet({})
+            self._state_dict = {}
+
+        else:  #### DataFrame case
+            if isinstance(setsystem, pd.DataFrame):
+                if isinstance(edge_col, int):
+                    self._edge_col = edge_col = setsystem.columns[edge_col]
+                    if isinstance(edge_col, int):
+                        setsystem = setsystem.rename(columns={edge_col: "edges"})
+                        self._edge_col = edge_col = "edges"
+                else:
+                    self._edge_col = edge_col
+
+                if isinstance(node_col, int):
+                    self._node_col = node_col = setsystem.columns[node_col]
+                    if isinstance(node_col, int):
+                        setsystem = setsystem.rename(columns={node_col: "nodes"})
+                        self._node_col = node_col = "nodes"
+                else:
+                    self._node_col = node_col
+
+                entity = setsystem.copy()
+
+                if isinstance(cell_weight_col, int):
+                    self._cell_weight_col = setsystem.columns[cell_weight_col]
+                else:
+                    self._cell_weight_col = cell_weight_col
+
+                if cell_weight_col in entity:
+                    entity = entity.fillna({cell_weight_col: cell_weights})
+                else:
+                    entity[cell_weight_col] = cell_weights
+
+                if isinstance(cell_properties, Sequence):
+                    cell_properties = [
+                        c
+                        for c in cell_properties
+                        if not c in [edge_col, node_col, cell_weight_col]
+                    ]
+                    cols = [edge_col, node_col, cell_weight_col] + cell_properties
+                    entity = entity[cols]
+                elif isinstance(cell_properties, dict):
+                    cp = []
+                    for idx in entity.index:
+                        edge, node = entity.iloc[idx][[edge_col, node_col]].values
+                        cp.append(cell_properties[edge][node])
+                    entity["cell_properties"] = cp
+
+            else:  ### Cases Other than DataFrame
+                self._edge_col = edge_col = edge_col or "edges"
+                if node_col == 1:
+                    self._node_col = node_col = "nodes"
+                else:
+                    self._node_col = node_col
+                self._cell_weight_col = cell_weight_col
+
+                if isinstance(setsystem, np.ndarray):
+                    if setsystem.shape[1] != 2:
+                        raise HyperNetXError("Numpy array must have exactly 2 columns.")
+                    entity = pd.DataFrame(setsystem, columns=[edge_col, node_col])
+                    entity[cell_weight_col] = cell_weights
+
+                elif isinstance(setsystem, dict):
+                    ## check if it is a dict of iterables or a nested dict. if the latter then pull
+                    ## out the nested dicts as cell properties.
+                    ## cell properties must be of the same type as setsystem
+
+                    entity = pd.Series(setsystem).explode()
+                    entity = pd.DataFrame(
+                        {edge_col: entity.index.to_list(), node_col: entity.values}
                     )
+
+                    if dict_depth(setsystem) > 2:
+                        cell_props = dict(setsystem)
+                        if isinstance(cell_properties, dict):
+                            ## if setsystem is a dict then cell properties must be a dict
+                            cell_properties = merge_nested_dicts(
+                                cell_props, cell_properties
+                            )
+                        else:
+                            cell_properties = cell_props
+
+                        df = setsystem
+                        cp = []
+                        wt = []
+                        for idx in entity.index:
+                            edge, node = entity.values[idx][[0, 1]]
+                            wt.append(df[edge][node].get(cell_weight_col, cell_weights))
+                            cp.append(df[edge][node])
+                        entity[self._cell_weight_col] = wt
+                        entity["cell_properties"] = cp
+
+                    else:
+                        entity[self._cell_weight_col] = cell_weights
+
+                elif isinstance(setsystem, Iterable):
+                    entity = pd.Series(setsystem).explode()
+                    entity = pd.DataFrame(
+                        {edge_col: entity.index.to_list(), node_col: entity.values}
+                    )
+                    entity["cell_weights"] = cell_weights
+
                 else:
-                    E = StaticEntitySet(entity=setsystem)
-                self._edges = E
-                self._nodes = E.restrict_to_levels([1], weights=False, aggregateby=None)
-                self._nodes._memberships = E.memberships
-                for n in self._nodes:
-                    self._nodes[n].memberships = self._nodes._memberships[n]  ### a bit of a hack to get same functionality from static as dynamic
-                                                                            ### we will have to see if it slows things down too much
-        else:
-            self._static = False
-            if setsystem is None:
-                setsystem = EntitySet("_", elements=[])
-            elif isinstance(setsystem, Entity):
-                setsystem = EntitySet("_", setsystem.incidence_dict)
-            elif isinstance(setsystem, dict):
-                # Must be a dictionary with values equal to iterables of Entities and hashables.
-                # Keys will be uids for new edges and values of the dictionary will generate the nodes.
-                setsystem = EntitySet("_", setsystem)
-            elif not isinstance(setsystem, EntitySet):
-                # If no ids are given, return default ids indexed by position in iterator
-                # This should be an iterable of sets
-                edge_labels = [self.name + str(x) for x in range(len(setsystem))]
-                setsystem = EntitySet("_", dict(zip(edge_labels, setsystem)))
-
-            _reg = setsystem.registry
-            _nodes = {k: Entity(k, **_reg[k].properties) for k in _reg}
-            _elements = {j: {k: _nodes[k] for k in setsystem[j]} for j in setsystem}
-            _edges = {
-                j: Entity(j, elements=_elements[j].values(), **setsystem[j].properties)
-                for j in setsystem
-            }
+                    raise HyperNetXError(
+                        "setsystem is not supported or is in the wrong format."
+                    )
 
-            self._edges = EntitySet(
-                f"{self.name}:Edges", elements=_edges.values(), **setsystem.properties
+            def props2dict(df=None):
+                if df is None:
+                    return {}
+                elif isinstance(df, pd.DataFrame):
+                    return df.set_index(df.columns[0]).to_dict(orient="index")
+                else:
+                    return dict(df)
+
+            if properties is None:
+                if edge_properties is not None or node_properties is not None:
+                    if edge_properties is not None:
+                        edge_properties = props2dict(edge_properties)
+                        for e in entity[edge_col].unique():
+                            if not e in edge_properties:
+                                edge_properties[e] = {}
+                        for v in edge_properties.values():
+                            v.setdefault(edge_weight_prop_col, default_edge_weight)
+                    else:
+                        edge_properties = {}
+                    if node_properties is not None:
+                        node_properties = props2dict(node_properties)
+                        for nd in entity[node_col].unique():
+                            if not nd in node_properties:
+                                node_properties[nd] = {}
+                        for v in node_properties.values():
+                            v.setdefault(node_weight_prop_col, default_node_weight)
+                    else:
+                        node_properties = {}
+                    properties = {0: edge_properties, 1: node_properties}
+            else:
+                if isinstance(properties, pd.DataFrame):
+                    if weight_prop_col in properties.columns:
+                        properties = properties.fillna(
+                            {weight_prop_col: default_weight}
+                        )
+                    elif misc_properties_col in properties.columns:
+                        for idx in properties.index:
+                            if not isinstance(
+                                properties[misc_properties_col][idx], dict
+                            ):
+                                properties[misc_properties_col][idx] = {
+                                    weight_prop_col: default_weight
+                                }
+                            else:
+                                properties[misc_properties_col][idx].setdefault(
+                                    weight_prop_col, default_weight
+                                )
+                    else:
+                        properties[weight_prop_col] = default_weight
+                if isinstance(properties, dict):
+                    if dict_depth(properties) <= 2:
+                        properties = pd.DataFrame(
+                            [
+                                {"id": k, misc_properties_col: v}
+                                for k, v in properties.items()
+                            ]
+                        )
+                        for idx in properties.index:
+                            if isinstance(properties[misc_properties_col][idx], dict):
+                                properties[misc_properties_col][idx].setdefault(
+                                    weight_prop_col, default_weight
+                                )
+                            else:
+                                properties[misc_properties_col][idx] = {
+                                    weight_prop_col: default_weight
+                                }
+                    elif set(properties.keys()) == {0, 1}:
+                        edge_properties = properties[0]
+                        for e in entity[edge_col].unique():
+                            if not e in edge_properties:
+                                edge_properties[e] = {
+                                    edge_weight_prop_col: default_edge_weight
+                                }
+                            else:
+                                edge_properties[e].setdefault(
+                                    edge_weight_prop_col, default_edge_weight
+                                )
+                        node_properties = properties[1]
+                        for nd in entity[node_col].unique():
+                            if not nd in node_properties:
+                                node_properties[nd] = {
+                                    node_weight_prop_col: default_node_weight
+                                }
+                            else:
+                                node_properties[nd].setdefault(
+                                    node_weight_prop_col, default_node_weight
+                                )
+                        for idx in properties.index:
+                            if not isinstance(
+                                properties[misc_properties_col][idx], dict
+                            ):
+                                properties[misc_properties_col][idx] = {
+                                    weight_prop_col: default_weight
+                                }
+                            else:
+                                properties[misc_properties_col][idx].setdefault(
+                                    weight_prop_col, default_weight
+                                )
+
+            self.E = EntitySet(
+                entity=entity,
+                level1=edge_col,
+                level2=node_col,
+                weight_col=cell_weight_col,
+                weights=cell_weights,
+                cell_properties=cell_properties,
+                misc_cell_props_col=misc_cell_properties_col or "cell_properties",
+                aggregateby=aggregateby or "sum",
+                properties=properties,
+                misc_props_col=misc_properties_col,
             )
-            self._nodes = EntitySet(f"{self.name}:Nodes", elements=_nodes.values())
-        if self._static:
-            temprows, tempcols = self.edges.data.T
-            tempdata = np.ones(len(temprows), dtype=int)
-            self.state_dict = {
-                "data": (temprows, tempcols, tempdata)
-            }  # how can we incorporate the counts into the nwhy hypergraph?
-            if self.nwhy:
-                self.g = nwhy.NWHypergraph(*self.state_dict["data"])
-                self.nwhy_dict = {"snodelg": dict(), "sedgelg": dict()}
-            self.state_dict["snodelg"] = dict()
-            self.state_dict["sedgelg"] = dict()
-            if self.filepath is not None:
-                self.save_state(fpath=self.filepath)
+
+            self._edges = self.E
+            self._nodes = self.E.restrict_to_levels([1])
+            self._dataframe = self.E.cell_properties.reset_index()
+            self._data_cols = data_cols = [self._edge_col, self._node_col]
+            self._dataframe[data_cols] = self._dataframe[data_cols].astype("category")
+
+            self.__dict__.update(locals())
+            self._set_default_state()
 
     @property
     def edges(self):
         """
         Object associated with self._edges.
 
         Returns
         -------
-        StaticEntitySet or EntitySet
-            If self.isstatic the StaticEntitySet, otherwise EntitySet.
+        EntitySet
         """
         return self._edges
 
     @property
     def nodes(self):
         """
         Object associated with self._nodes.
 
         Returns
         -------
-        StaticEntitySet or EntitySet
-            If self.isstatic the StaticEntitySet, otherwise EntitySet.
-
+        EntitySet
         """
         return self._nodes
 
     @property
-    def isstatic(self):
+    def dataframe(self):
+        """Returns dataframe of incidence pairs and their properties.
+
+        Returns
+        -------
+        pd.DataFrame
+        """
+        return self._dataframe
+
+    @property
+    def properties(self):
+        """Returns dataframe of edge and node properties.
+
+        Returns
+        -------
+        pd.DataFrame
         """
-        Checks whether nodes and edges are immutable
+        return self.E.properties
+
+    @property
+    def edge_props(self):
+        """Dataframe of edge properties
+        indexed on edge ids
 
         Returns
         -------
-        Boolean
+        pd.DataFrame
+        """
+        return self.E.properties.loc[0]
+
+    @property
+    def node_props(self):
+        """Dataframe of node properties
+        indexed on node ids
 
+        Returns
+        -------
+        pd.DataFrame
         """
-        return self._static
+        return self.E.properties.loc[1]
 
     @property
     def incidence_dict(self):
         """
-        Dictionary keyed by edge uids with values the uids of nodes in each edge
+        Dictionary keyed by edge uids with values the uids of nodes in each
+        edge
 
         Returns
         -------
         dict
 
         """
-        return self._edges.incidence_dict
+        return self.E.incidence_dict
 
     @property
     def shape(self):
         """
         (number of nodes, number of edges)
 
         Returns
         -------
         tuple
 
         """
-        if self.nwhy:
-            return (self.g.number_of_nodes(), self.g.number_of_edges())
-        else:
-            return (len(self._nodes.elements), len(self._edges.elements))
+        return len(self._nodes.elements), len(self._edges.elements)
 
     def __str__(self):
         """
         String representation of hypergraph
 
         Returns
         -------
         str
 
         """
-        return f"Hypergraph({self.edges.elements},name={self.name})"
+        return f"{self.name}, <class 'hypernetx.classes.hypergraph.Hypergraph'>"
 
     def __repr__(self):
         """
         String representation of hypergraph
 
         Returns
         -------
         str
 
         """
-        return f"Hypergraph({self.edges.elements},name={self.name})"
+        return f"{self.name}, hypernetx.classes.hypergraph.Hypergraph"
 
     def __len__(self):
         """
         Number of nodes
 
         Returns
         -------
         int
 
         """
-        if self.nwhy:
-            return self.g.number_of_nodes()
-        else:
-            return len(self._nodes)
+        return len(self._nodes)
 
     def __iter__(self):
         """
         Iterate over the nodes of the hypergraph
 
         Returns
         -------
@@ -329,18 +693,15 @@
         Returns boolean indicating if item is in self.nodes
 
         Parameters
         ----------
         item : hashable or Entity
 
         """
-        if isinstance(item, Entity):
-            return item.uid in self.nodes
-        else:
-            return item in self.nodes
+        return item in self.nodes
 
     def __getitem__(self, node):
         """
         Returns the neighbors of node
 
         Parameters
         ----------
@@ -350,365 +711,186 @@
         Returns
         -------
         neighbors(node) : iterator
 
         """
         return self.neighbors(node)
 
-    @not_implemented_for("dynamic")
-    def get_id(self, uid, edges=False):
-        """
-        Return the internally assigned id associated with a label.
+    def get_cell_properties(
+        self, edge: str, node: str, prop_name: Optional[str] = None
+    ) -> Any | dict[str, Any]:
+        """Get cell properties on a specified edge and node
 
         Parameters
         ----------
-        uid : string
-            User provided name/id/label for hypergraph object
-        edges : bool, optional
-            Determines if uid is an edge or node name
+        edge : str
+            edgeid
+        node : str
+            nodeid
+        prop_name : str, optional
+            name of a cell property; if None, all cell properties will be returned
 
         Returns
         -------
-        : int
-            internal id assigned at construction
+        : int or str or dict of {str: any}
+            cell property value if `prop_name` is provided, otherwise ``dict`` of all
+            cell properties and values
         """
-        kdx = (edges + 1) % 2
-        # return list(self.edges.labs(kdx)).index(uid)
-        return int(np.argwhere(self.edges.labs(kdx) == uid)[0])
+        if prop_name is None:
+            return self.edges.get_cell_properties(edge, node)
 
-    @not_implemented_for("dynamic")
-    def get_name(self, id, edges=False):
-        """
-        Return the user defined name/id/label associated to an
-        internally assigned id.
+        return self.edges.get_cell_property(edge, node, prop_name)
+
+    def get_properties(self, id, level=None, prop_name=None):
+        """Returns an object's specific property or all properties
 
         Parameters
         ----------
-        id : int
-            Internally assigned id
-        edges : bool, optional
-            Determines if id references an edge or node
+        id : hashable
+            edge or node id
+        level : int | None , optional, default = None
+            if separate edge and node properties then enter 0 for edges
+            and 1 for nodes.
+        prop_name : str | None, optional, default = None
+            if None then all properties associated with the object will  be
+            returned.
 
         Returns
         -------
-        str
-            User provided name/id/label for hypergraph object
+        : str or dict
+            single property or dictionary of properties
         """
-        kdx = (edges + 1) % 2
-        return self.edges.labs(kdx)[id]
+        if prop_name == None:
+            return self.E.get_properties(id, level=level)
+        else:
+            return self.E.get_property(id, prop_name, level=level)
 
-    @not_implemented_for("dynamic")
-    def get_linegraph(self, s, edges=True, use_nwhy=True):
+    @warn_nwhy
+    def get_linegraph(self, s=1, edges=True):
         """
         Creates an ::term::s-linegraph for the Hypergraph.
-        If edges=True (default)then the edges will be the vertices of the line graph.
-        Two vertices are connected by an s-line-graph edge if the corresponding
-        hypergraphedges intersect in at least s hypergraph nodes.
-        If edges=False, the hypergraph nodes will be the vertices of the line graph.
-        Two vertices are connected if the nodes they correspond to share at least s
-        incident hyper edges.
+        If edges=True (default)then the edges will be the vertices of the line
+        graph. Two vertices are connected by an s-line-graph edge if the
+        corresponding hypergraph edges intersect in at least s hypergraph nodes.
+        If edges=False, the hypergraph nodes will be the vertices of the line
+        graph. Two vertices are connected if the nodes they correspond to share
+        at least s incident hyper edges.
 
         Parameters
         ----------
         s : int
             The width of the connections.
-        edges : bool, optional
+        edges : bool, optional, default = True
             Determine if edges or nodes will be the vertices in the linegraph.
-        use_nwhy : bool, optional
-            Requests that nwhy be used to construct the linegraph. If NWHy is not available this is ignored.
 
         Returns
         -------
         nx.Graph
             A NetworkX graph.
         """
-        if use_nwhy and self.nwhy:
-            d = self.nwhy_dict
-        else:
-            d = self.state_dict
+        d = self._state_dict
         key = "sedgelg" if edges else "snodelg"
         if s in d[key]:
             return d[key][s]
+
+        if edges:
+            A, Amap = self.edge_adjacency_matrix(s=s, index=True)
+            Amaplst = [(k, self.edge_props.loc[k].to_dict()) for k in Amap]
         else:
-            if use_nwhy and self.nwhy:
-                d[key][s] = self.g.s_linegraph(s=s, edges=edges)
-            else:
-                if edges:
-                    A = self.edge_adjacency_matrix(s=s)
-                else:
-                    A = self.adjacency_matrix(s=s)
-                d[key][s] = nx.from_scipy_sparse_matrix(A)
-                if self.filepath is not None:
-                    self.save_state(fpath=self.filepath)
-            return d[key][s]
+            A, Amap = self.adjacency_matrix(s=s, index=True)
+            Amaplst = [(k, self.node_props.loc[k].to_dict()) for k in Amap]
+
+        ### TODO: add key function to compute weights lambda x,y : funcval
+
+        A = np.array(np.nonzero(A))
+        e1 = np.array([Amap[idx] for idx in A[0]])
+        e2 = np.array([Amap[idx] for idx in A[1]])
+        A = np.array([e1, e2]).T
+        g = nx.Graph()
+        g.add_edges_from(A)
+        g.add_nodes_from(Amaplst)
+        d[key][s] = g
+        return g
 
-    @not_implemented_for("dynamic")
     def set_state(self, **kwargs):
         """
         Allow state_dict updates from outside of class. Use with caution.
 
         Parameters
         ----------
         **kwargs
             key=value pairs to save in state dictionary
         """
-        self.state_dict.update(kwargs)
-        if self.filepath is not None:
-            self.save_state(fpath=self.filepath)
-
-    @not_implemented_for("dynamic")
-    def save_state(self, fpath=None):
-        """
-        Save the hypergraph as an ordered pair: [state_dict,labels]
-        The hypergraph can be recovered using the command:
-
-            >>> H = hnx.Hypergraph.recover_from_state(fpath)
-
-        Parameters
-        ----------
-        fpath : str, optional
-        """
-        if fpath is None:
-            fpath = self.filepath or "current_state.p"
-        pickle.dump([self.state_dict, self.edges.labels], open(fpath, "wb"))
+        self._state_dict.update(kwargs)
 
-    @classmethod
-    def recover_from_state(cls, fpath="current_state.p", newfpath=None, use_nwhy=True):
-        """
-        Recover a static hypergraph pickled using save_state.
-
-        Parameters
-        ----------
-        fpath : str
-            Full path to pickle file containing state_dict and labels
-            of hypergraph
-
-        Returns
-        -------
-        H : Hypergraph
-            static hypergraph with state dictionary prefilled
-        """
-        temp, labels = pickle.load(open(fpath, "rb"))
-        recovered_data = np.array(temp["data"])[[0, 1]].T  # need to save counts as well
-        recovered_counts = np.array(temp["data"])[
-            [2]
-        ]  # ammend this to store cell weights
-        E = StaticEntitySet(data=recovered_data, labels=labels)
-        E.properties["counts"] = recovered_counts
-        H = Hypergraph(E, use_nwhy=use_nwhy)
-        H.state_dict.update(temp)
-        if newfpath == "same":
-            newfpath = fpath
-        if newfpath is not None:
-            H.filepath = newfpath
-            H.save_state()
-        return H
-
-    @classmethod
-    def add_nwhy(cls, h, fpath=None):
-        """
-        Add nwhy functionality to a hypergraph.
-
-        Parameters
-        ----------
-        h : hnx.Hypergraph
-        fpath : file path for storage of hypergraph state dictionary
-
-        Returns
-        -------
-        hnx.Hypergraph
-            Returns a copy of h with static set to true and nwhy set to True
-            if it is available.
-
-        """
-
-        if h.isstatic:
-            sd = h.state_dict
-            H = Hypergraph(h.edges, use_nwhy=True, filepath=fpath)
-            H.state_dict.update(sd)
-            return H
-        else:
-            return Hypergraph(StaticEntitySet(h.edges), use_nwhy=True, filepath=fpath)
+    def _set_default_state(self):
+        """Populate state_dict with default values"""
+        self._state_dict = {}
+
+        self._state_dict["dataframe"] = df = self.dataframe
+        self._state_dict["labels"] = {
+            "edges": np.array(df[self._edge_col].cat.categories),
+            "nodes": np.array(df[self._node_col].cat.categories),
+        }
+        self._state_dict["data"] = np.array(
+            [df[self._edge_col].cat.codes, df[self._node_col].cat.codes], dtype=int
+        ).T
+        self._state_dict["snodelg"] = dict()  ### s: nx.graph
+        self._state_dict["sedgelg"] = dict()
+        self._state_dict["neighbors"] = defaultdict(dict)  ### s: {node: neighbors}
+        self._state_dict["edge_neighbors"] = defaultdict(
+            dict
+        )  ### s: {edge: edge_neighbors}
+        self._state_dict["adjacency_matrix"] = dict()  ### s: scipy.sparse.csr_matrix
+        self._state_dict["edge_adjacency_matrix"] = dict()
 
     def edge_size_dist(self):
         """
         Returns the size for each edge
 
         Returns
         -------
         np.array
 
         """
-        if self.isstatic:
-            dist = self.state_dict.get("edge_size_dist", None)
-            if dist:
-                return dist
-            else:
-                if self.nwhy:
-                    dist = self.g.edge_size_dist()
-                else:
-                    dist = list(np.array(np.sum(self.incidence_matrix(), axis=0))[0])
 
-                self.set_state(edge_size_dist=dist)
-                return dist
+        if "edge_size_dist" not in self._state_dict:
+            dist = np.array(np.sum(self.incidence_matrix(), axis=0))[0].tolist()
+            self.set_state(edge_size_dist=dist)
+            return dist
         else:
-            return list(np.array(np.sum(self.incidence_matrix(), axis=0))[0])
-
-    def convert_to_static(
-        self,
-        name=None,
-        use_nwhy=False,
-        filepath=None,
-    ):
-        """
-        Returns new static hypergraph with the same dictionary as original hypergraph
-
-        Parameters
-        ----------
-        name : None, optional
-            Name
-        use_nwhy : bool, optional, default : False
-            Description
-        filepath : None, optional, default : False
-            Description
-
-        Returned
-        ------------------
-        hnx.Hypergraph
-            Will have attribute static = True
-
-        Note
-        ----
-        Static hypergraphs store the user defined node and edge names in
-        a dictionary of labeled lists. The order of the lists provides an
-        index, which the hypergraph uses in place of the node and edge names
-        for faster processing.
-
-        """
-        if self.isstatic:
-            return self
-        else:
-            edict = self.incidence_dict
-            E = StaticEntitySet(edict)
-            return Hypergraph(E, use_nwhy=use_nwhy, filepath=filepath, name=name)
-
-    def remove_static(self, name=None):
-        """
-        Returns dynamic hypergraph
-
-        Parameters
-        ----------
-        name : None, optional
-            User defined namae of hypergraph
-
-        Returns
-        -------
-        hnx.Hypergraph
-            A new hypergraph with the same dictionary as self but allowing dynamic
-            changes to nodes and edges.
-            If hypergraph is not static, returns self.
-        """
-        if not self.isstatic:
-            return self
-        else:
-            return Hypergraph(self.edges.incidence_dict, name=name)
-
-    def translate(self, idx, edges=False):
-        """
-        Returns the translation of numeric values associated with hypergraph.
-        Only needed if exposing the static identifiers assigned by the class.
-        If not static then the idx is returned.
-
-        Parameters
-        ----------
-        idx : int
-            class assigned integer for internal manipulation of Hypergraph data
-        edges : bool, optional, default: True
-            If True then translates from edge index. Otherwise will translate from
-            node index, default=False
-
-        Returns
-        -------
-         : int or string
-            User assigned identifier corresponding to idx
-        """
-        if self.isstatic:
-            return self.get_name(idx, edges=edges)
-        else:
-            return idx
-
-    def s_degree(self, node, s=1):  # deprecate this to degree
-        """
-        Same as `degree`
-
-        Parameters
-        ----------
-        node : Entity or hashable
-            If hashable, then must be uid of node in hypergraph
-
-        s : positive integer, optional, default: 1
-
-        Returns
-        -------
-        s_degree : int
-            The degree of a node in the subgraph induced by edges
-            of size s
-
-        Note
-        ----
-        The :term:`s-degree` of a node is the number of edges of size
-        at least s that contain the node.
-
-        """
-        msg = (
-            "s-degree is deprecated and will be removed in"
-            " release 1.0.0. Use degree(node,s=int) instead."
-        )
-
-        warnings.warn(msg, DeprecationWarning)
-        return self.degree(node, s)
+            return self._state_dict["edge_size_dist"]
 
     def degree(self, node, s=1, max_size=None):
         """
         The number of edges of size s that contain node.
 
         Parameters
         ----------
         node : hashable
             identifier for the node.
-        s : positive integer, optional, default: 1
+        s : positive integer, optional, default 1
             smallest size of edge to consider in degree
-        max_size : positive integer or None, optional, default: None
+        max_size : positive integer or None, optional, default = None
             largest size of edge to consider in degree
 
         Returns
         -------
          : int
 
         """
-        if self.isstatic:
-            ndx = self.get_id(node)
-            if self.nwhy:                
-                return self.g.degree(ndx, min_size=s, max_size=None)
-            else:
-                memberships = set(self.nodes.memberships[node])
-        else:
-            memberships = set(self.nodes[node].memberships)
-                                  
-        if max_size is not None:
-            return len(
-                set(
-                    e
-                    for e in memberships
-                    if len(self.edges[e]) in range(s, max_size + 1)
-                )
-            )
-        elif s > 1:
-            return len(set(e for e in memberships if len(self.edges[e]) >= s))
+        if s == 1 and max_size == None:
+            return len(self.E.memberships[node])
         else:
+            memberships = set()
+            for edge in self.E.memberships[node]:
+                size = len(self.edges[edge])
+                if size >= s and (max_size is None or size <= max_size):
+                    memberships.add(edge)
+
             return len(memberships)
 
     def size(self, edge, nodeset=None):
         """
         The number of nodes in nodeset that belong to edge.
         If nodeset is None then returns the size of edge
 
@@ -720,76 +902,63 @@
         Returns
         -------
         size : int
 
         """
         if nodeset is not None:
             return len(set(nodeset).intersection(set(self.edges[edge])))
-        else:
-            if self.nwhy:
-                edx = self.get_id(edge,edges=True)
-                return self.g.size(edx)
-            else:
-                return len(self.edges[edge])
+
+        return len(self.edges[edge])
 
     def number_of_nodes(self, nodeset=None):
         """
         The number of nodes in nodeset belonging to hypergraph.
 
         Parameters
         ----------
-        nodeset : an interable of Entities, optional, default: None
+        nodeset : an interable of Entities, optional, default = None
             If None, then return the number of nodes in hypergraph.
 
         Returns
         -------
         number_of_nodes : int
 
         """
-        if nodeset:
+        if nodeset is not None:
             return len([n for n in self.nodes if n in nodeset])
-        else:
-            if self.nwhy == True:
-                return self.g.number_of_nodes()
-            else:
-                return len(self.nodes)
+
+        return len(self.nodes)
 
     def number_of_edges(self, edgeset=None):
         """
         The number of edges in edgeset belonging to hypergraph.
 
         Parameters
         ----------
-        edgeset : an interable of Entities, optional, default: None
+        edgeset : an iterable of Entities, optional, default = None
             If None, then return the number of edges in hypergraph.
 
         Returns
         -------
         number_of_edges : int
         """
         if edgeset:
             return len([e for e in self.edges if e in edgeset])
-        else:
-            if self.nwhy == True:
-                return self.g.number_of_edges()
-            else:
-                return len(self.edges)
+
+        return len(self.edges)
 
     def order(self):
         """
         The number of nodes in hypergraph.
 
         Returns
         -------
         order : int
         """
-        if self.nwhy:
-            return self.g.number_of_nodes()
-        else:
-            return len(self.nodes)
+        return len(self.nodes)
 
     def dim(self, edge):
         """
         Same as size(edge)-1.
         """
         return self.size(edge) - 1
 
@@ -798,916 +967,645 @@
         The nodes in hypergraph which share s edge(s) with node.
 
         Parameters
         ----------
         node : hashable or Entity
             uid for a node in hypergraph or the node Entity
 
-        s : int, list, optional, default : 1
+        s : int, list, optional, default = 1
             Minimum number of edges shared by neighbors with node.
 
         Returns
         -------
-         : list
-            List of neighbors
+        neighbors : list
+            s-neighbors share at least s edges in the hypergraph
 
         """
-        if not node in self.nodes:
-            print(f"Node is not in hypergraph {self.name}.")
-            return
-
-        if self.isstatic:
-            g = self.get_linegraph(s=s, edges=False)
-            ndx = self.get_id(node)
-            if self.nwhy == True:
-                nbrs = g.s_neighbors(ndx)
+        if node not in self.nodes:
+            print(f"{node} is not in hypergraph {self.name}.")
+            return None
+        if node in self._state_dict["neighbors"][s]:
+            return self._state_dict["neighbors"][s][node]
+        else:
+            M = self.incidence_matrix()
+            rdx = self._state_dict["labels"]["nodes"]
+            jdx = np.where(rdx == node)
+            idx = (M[jdx].dot(M.T) >= s) * 1
+            idx = np.nonzero(idx)[1]
+            neighbors = list(rdx[idx])
+            if len(neighbors) > 0:
+                neighbors.remove(node)
+                self._state_dict["neighbors"][s][node] = neighbors
             else:
-                nbrs = list(g.neighbors(ndx))
-            return [self.translate(nb, edges=False) for nb in nbrs]
-
-        else:
-            node = self.nodes[
-                node
-            ].uid  # this allows node to be an Entity instead of a string
-            memberships = set(self.nodes[node].memberships).intersection(
-                self.edges.uidset
-            )
-            edgeset = {e for e in memberships if len(self.edges[e]) >= s}
-
-            neighborlist = set()
-            for e in edgeset:
-                neighborlist.update(self.edges[e].uidset)
-            neighborlist.discard(node)
-            return list(neighborlist)
+                self._state_dict["neighbors"][s][node] = []
+        return neighbors
 
     def edge_neighbors(self, edge, s=1):
         """
         The edges in hypergraph which share s nodes(s) with edge.
 
         Parameters
         ----------
         edge : hashable or Entity
             uid for a edge in hypergraph or the edge Entity
 
-        s : int, list, optional, default : 1
+        s : int, list, optional, default = 1
             Minimum number of nodes shared by neighbors edge node.
 
         Returns
         -------
          : list
             List of edge neighbors
 
         """
-        if not edge in self.edges:
-            print(f"Edge is not in hypergraph {self.name}.")
-            return
-
-        if self.isstatic:
-            g = self.get_linegraph(s=s, edges=True)
-            edx = self.get_id(edge, edges=True)
-            if self.nwhy == True:
-                nbrs = g.s_neighbors(edx)
-            else:
-                nbrs = list(g.neighbors(edx))
-            return [self.translate(nb, edges=True) for nb in nbrs]
-
-        else:
-            node = self.edges[edge].uid
-            return self.dual().neighbors(node, s=s)
-
-    @not_implemented_for("static")
-    def remove_node(self, node):
-        """
-        Removes node from edges and deletes reference in hypergraph nodes
-
-        Parameters
-        ----------
-        node : hashable or Entity
-            a node in hypergraph
-
-        Returns
-        -------
-        hypergraph : Hypergraph
-
-        """
-        if not node in self._nodes:
-            return self
-        else:
-            if not isinstance(node, Entity):
-                node = self._nodes[node]
-            for edge in node.memberships:
-                self._edges[edge].remove(node)
-            self._nodes.remove(node)
-        return self
-
-    @not_implemented_for("static")
-    def remove_nodes(self, node_set):
-        """
-        Removes nodes from edges and deletes references in hypergraph nodes
-
-        Parameters
-        ----------
-        node_set : an iterable of hashables or Entities
-            Nodes in hypergraph
-
-        Returns
-        -------
-        hypergraph : Hypergraph
 
-        """
-        for node in node_set:
-            self.remove_node(node)
-        return self
-
-    @not_implemented_for("static")
-    def _add_nodes_from(self, nodes):
-        """
-        Private helper method instantiates new nodes when edges added to hypergraph.
-
-        Parameters
-        ----------
-        nodes : iterable of hashables or Entities
-
-        """
-        for node in nodes:
-            if node in self._edges:
-                raise HyperNetXError("Node already an edge.")
-            elif node in self._nodes and isinstance(node, Entity):
-                self._nodes[node].__dict__.update(node.properties)
-            elif node not in self._nodes:
-                if isinstance(node, Entity):
-                    self._nodes.add(Entity(node.uid, **node.properties))
-                else:
-                    self._nodes.add(Entity(node))
-
-    @not_implemented_for("static")
-    def add_edge(self, edge):
-        """
-
-        Adds a single edge to hypergraph.
-
-        Parameters
-        ----------
-        edge : hashable or Entity
-            If hashable the edge returned will be empty.
-
-        Returns
-        -------
-        hypergraph : Hypergraph
-
-        Notes
-        -----
-        When adding an edge to a hypergraph children must be removed
-        so that nodes do not have elements.
-        Each node (element of edge) must be instantiated as a node,
-        making sure its uid isn't already present in the self.
-        If an added edge contains nodes that cannot be added to hypergraph
-        then an error will be raised.
-
-        """
-        if edge in self._edges:
-            warnings.warn("Cannot add edge. Edge already in hypergraph")
-        elif edge in self._nodes:
-            warnings.warn("Cannot add edge. Edge is already a Node")
-        elif isinstance(edge, Entity):
-            if len(edge) > 0:
-                self._add_nodes_from(edge.elements.values())
-                self._edges.add(
-                    Entity(
-                        edge.uid,
-                        elements=[self._nodes[k] for k in edge],
-                        **edge.properties,
-                    )
-                )
-                for n in edge.elements:
-                    self._nodes[n].memberships[edge.uid] = self._edges[edge.uid]
-            else:
-                self._edges.add(Entity(edge.uid, **edge.properties))
-        else:
-            self._edges.add(Entity(edge))  # this generates an empty edge
-        return self
-
-    @not_implemented_for("static")
-    def add_edges_from(self, edge_set):
-        """
-        Add edges to hypergraph.
-
-        Parameters
-        ----------
-        edge_set : iterable of hashables or Entities
-            For hashables the edges returned will be empty.
-
-        Returns
-        -------
-        hypergraph : Hypergraph
-
-        """
-        for edge in edge_set:
-            self.add_edge(edge)
-        return self
-
-    @not_implemented_for("static")
-    def add_node_to_edge(self, node, edge):
-        """
-
-        Adds node to an edge in hypergraph edges
-
-        Parameters
-        ----------
-        node: hashable or Entity
-            If Entity, only uid and properties will be used.
-            If uid is already in nodes then the known node will
-            be used
-
-        edge: uid of edge or edge, must belong to self.edges
-
-        Returns
-        -------
-        hypergraph : Hypergraph
-
-        """
-        if edge in self._edges:
-            if not isinstance(edge, Entity):
-                edge = self._edges[edge]
-            if node in self._nodes:
-                self._edges[edge].add(self._nodes[node])
+        if edge not in self.edges:
+            print(f"Edge is not in hypergraph {self.name}.")
+            return None
+        if edge in self._state_dict["edge_neighbors"][s]:
+            return self._state_dict["edge_neighbors"][s][edge]
+        else:
+            M = self.incidence_matrix()
+            cdx = self._state_dict["labels"]["edges"]
+            jdx = np.where(cdx == edge)
+            idx = (M.T[jdx].dot(M) >= s) * 1
+            idx = np.nonzero(idx)[1]
+            edge_neighbors = list(cdx[idx])
+            if len(edge_neighbors) > 0:
+                edge_neighbors.remove(edge)
+                self._state_dict["edge_neighbors"][s][edge] = edge_neighbors
             else:
-                if not isinstance(node, Entity):
-                    node = Entity(node)
-                else:
-                    node = Entity(node.uid, **node.properties)
-                self._edges[edge].add(node)
-                self._nodes.add(node)
-
-        return self
-
-    @not_implemented_for("static")
-    def remove_edge(self, edge):
-        """
-        Removes a single edge from hypergraph.
-
-        Parameters
-        ----------
-        edge : hashable or Entity
-
-        Returns
-        -------
-        hypergraph : Hypergraph
-
-        Notes
-        -----
-
-        Deletes reference to edge from all of its nodes.
-        If any of its nodes do not belong to any other edges
-        the node is dropped from self.
-
-        """
-        if edge in self._edges:
-            if not isinstance(edge, Entity):
-                edge = self._edges[edge]
-            for node in edge.uidset:
-                edge.remove(node)
-                if len(self._nodes[node]._memberships) == 1:
-                    self._nodes.remove(node)
-            self._edges.remove(edge)
-        return self
-
-    @not_implemented_for("static")
-    def remove_edges(self, edge_set):
-        """
-        Removes edges from hypergraph.
-
-        Parameters
-        ----------
-        edge_set : iterable of hashables or Entities
-
-        Returns
-        -------
-        hypergraph : Hypergraph
-
-        """
-        for edge in edge_set:
-            self.remove_edge(edge)
-        return self
+                self._state_dict["edge_neighbors"][s][edge] = []
+            return edge_neighbors
 
     def incidence_matrix(self, weights=False, index=False):
         """
         An incidence matrix for the hypergraph indexed by nodes x edges.
 
         Parameters
         ----------
-        weights : bool, default=False
+        weights : bool, default =False
             If False all nonzero entries are 1.
             If True and self.static all nonzero entries are filled by
             self.edges.cell_weights dictionary values.
 
-        index : boolean, optional, default False
+        index : boolean, optional, default = False
             If True return will include a dictionary of node uid : row number
             and edge uid : column number
 
         Returns
         -------
         incidence_matrix : scipy.sparse.csr.csr_matrix or np.ndarray
 
-        row dictionary : dict
-            Dictionary identifying rows with nodes
-
-        column dictionary : dict
-            Dictionary identifying columns with edges
+        row_index : list
+            index of node ids for rows
 
-        """
-        if self.isstatic:
-            if weights == False:
-                mat = self.state_dict.get("incidence_matrix", None)
-                if mat is None:
-                    mat = self.edges.incidence_matrix()
-                    self.state_dict["incidence_matrix"] = mat
-                if index:
-                    rdict = dict(enumerate(self.edges.labs(1)))
-                    cdict = dict(enumerate(self.edges.labs(0)))
-                    return mat, rdict, cdict
-                else:
-                    return mat
-            if weights == True:
-                mat = self.state_dict.get("weighted_incidence_matrix", None)
-                if mat is None:
-                    mat = self.edges.incidence_matrix(weights=True)
-                    self.state_dict["weighted_incidence_matrix"] = mat
-                if index:
-                    rdict = dict(enumerate(self.edges.labs(1)))
-                    cdict = dict(enumerate(self.edges.labs(0)))
-                    return mat, rdict, cdict
-                else:
-                    return mat
-        else:
-            return self.edges.incidence_matrix(index=index)
+        col_index : list
+            index of edge ids for columns
 
-    @staticmethod
-    def _incidence_to_adjacency(M, s=1, weights=False):
         """
-        Helper method to obtain adjacency matrix from 
-        boolean incidence matrix for s-metrics.
-        Self loops are not supported.
-        The adjacency matrix will define an s-linegraph.
-
-        Parameters
-        ----------
-        M : scipy.sparse.csr.csr_matrix 
-            incidence matrix of 0's and 1's
-
-        s : int, optional, default: 1
-
-        # weights : bool, dict optional, default=True
-        #     If False all nonzero entries are 1.
-        #     Otherwise, weights will be as in product.
+        sdkey = "incidence_matrix"
+        if weights:
+            sdkey = "weighted_" + sdkey
 
-        Returns
-        -------
-        a matrix : scipy.sparse.csr.csr_matrix
-
-        """
-        M = csr_matrix(M)
-        weights = False ## currently weighting is not supported
+        if sdkey in self._state_dict:
+            M = self._state_dict[sdkey]
+        else:
+            df = self.dataframe
+            data_cols = [self._node_col, self._edge_col]
+            if weights == True:
+                data = df[self._cell_weight_col].values
+                M = csr_matrix(
+                    (data, tuple(np.array(df[col].cat.codes) for col in data_cols))
+                )
+            else:
+                M = csr_matrix(
+                    (
+                        [1] * len(df),
+                        tuple(np.array(df[col].cat.codes) for col in data_cols),
+                    )
+                )
+            self._state_dict[sdkey] = M
 
-        if weights == False:
-            A = M.dot(M.transpose())
-            A.setdiag(0)
-            A = (A >= s) * 1
-        return A
+        if index == True:
+            rdx = self.dataframe[self._node_col].cat.categories
+            cdx = self.dataframe[self._edge_col].cat.categories
 
+            return M, rdx, cdx
+        else:
+            return M
 
-    def adjacency_matrix(self, index=False, s=1):## , weights=False):
+    def adjacency_matrix(self, s=1, index=False, remove_empty_rows=False):
         """
-        The sparse weighted :term:`s-adjacency matrix`
+        The :term:`s-adjacency matrix` for the hypergraph.
 
         Parameters
         ----------
-        s : int, optional, default: 1
+        s : int, optional, default = 1
 
-        index: boolean, optional, default: False
-            if True, will return a rowdict of row to node uid
+        index: boolean, optional, default = False
+            if True, will return the index of ids for rows and columns
 
-        weights: bool, default=True
-            If False all nonzero entries are 1.
-            If True adjacency matrix will depend on weighted incidence matrix,
+        remove_empty_rows: boolean, optional, default = False
 
         Returns
         -------
         adjacency_matrix : scipy.sparse.csr.csr_matrix
 
-        row dictionary : dict
+        node_index : list
+            index of ids for rows and columns
 
         """
-        weights = False ## Currently default weights are not supported.
-        M = self.incidence_matrix(index=index, weights=weights)
-        if index:
-            return Hypergraph._incidence_to_adjacency(M[0], s=s, weights=weights), M[1]
+        try:
+            A = self._state_dict["adjacency_matrix"][s]
+        except:
+            M = self.incidence_matrix()
+            A = M @ (M.T)
+            A.setdiag(0)
+            A = (A >= s) * 1
+            self._state_dict["adjacency_matrix"][s] = A
+        if index == True:
+            return A, self._state_dict["labels"]["nodes"]
         else:
-            return Hypergraph._incidence_to_adjacency(M, s=s, weights=weights)
+            return A
 
-    def edge_adjacency_matrix(self, index=False, s=1, weights=False):
+    def edge_adjacency_matrix(self, s=1, index=False):
         """
-        The weighted :term:`s-adjacency matrix` for the dual hypergraph.
+        The :term:`s-adjacency matrix` for the dual hypergraph.
 
         Parameters
         ----------
-        s : int, optional, default: 1
-
-        index: boolean, optional, default: False
-            if True, will return a coldict of column to edge uid
+        s : int, optional, default 1
 
-        sparse: boolean, optional, default: True
-
-        weighted: boolean, optional, default: True
+        index: boolean, optional, default = False
+            if True, will return the index of ids for rows and columns
 
         Returns
         -------
-        edge_adjacency_matrix : scipy.sparse.csr.csr_matrix or numpy.ndarray
+        edge_adjacency_matrix : scipy.sparse.csr.csr_matrix
 
-        column dictionary : dict
+        edge_index : list
+            index of ids for rows and columns
 
         Notes
         -----
         This is also the adjacency matrix for the line graph.
         Two edges are s-adjacent if they share at least s nodes.
-        If index=True, returns a dictionary column_index:edge_uid
+        If remove_zeros is True will return the auxillary matrix
 
         """
-        weights=False  ## Currently default weights are not supported
-
-        M = self.incidence_matrix(index=index, weights=weights)
-        if index:
-            return (
-                Hypergraph._incidence_to_adjacency(
-                    M[0].transpose(), s=s, weights=weights
-                ),
-                M[2],
-            )
+        try:
+            A = self._state_dict["edge_adjacency_matrix"][s]
+        except:
+            M = self.incidence_matrix()
+            A = (M.T) @ (M)
+            A.setdiag(0)
+            A = (A >= s) * 1
+            self._state_dict["edge_adjacency_matrix"][s] = A
+        if index == True:
+            return A, self._state_dict["labels"]["edges"]
         else:
-            return Hypergraph._incidence_to_adjacency(
-                M.transpose(), s=s, weights=weights
-            )
+            return A
 
-    def auxiliary_matrix(self, s=1, index=False):
+    def auxiliary_matrix(self, s=1, node=True, index=False):
         """
-        The unweighted :term:`s-auxiliary matrix` for hypergraph
+        The unweighted :term:`s-edge or node auxiliary matrix` for hypergraph
 
         Parameters
         ----------
-        s : int
-        index : bool, optional, default: False
-            return a dictionary of labels for the rows of the matrix
-
+        s : int, optional, default = 1
+        node : bool, optional, default = True
+            whether to return based on node or edge adjacencies
 
         Returns
         -------
-        auxiliary_matrix : scipy.sparse.csr.csr_matrix or numpy.ndarray
-            Will return the same type of matrix as self.arr
-
-        Notes
-        -----
-        Creates subgraph by restricting to edges of cardinality at least s.
-        Returns the unweighted s-edge adjacency matrix for the subgraph.
+        auxiliary_matrix : scipy.sparse.csr.csr_matrix
+            Node/Edge adjacency matrix with empty rows and columns
+            removed
+        index : np.array
+            row and column index of userids
 
         """
+        if node == True:
+            A, Amap = self.adjacency_matrix(s, index=True)
+        else:
+            A, Amap = self.edge_adjacency_matrix(s, index=True)
 
-        edges = [e for e in self.edges if len(self.edges[e]) >= s]
-        H = self.restrict_to_edges(edges)
-        return H.edge_adjacency_matrix(s=s, index=index, weights=False)
+        idx = np.nonzero(np.sum(A, axis=1))[0]
+        if len(idx) < A.shape[0]:
+            B = A[idx][:, idx]
+        else:
+            B = A
+        if index:
+            return B, Amap[idx]
+        else:
+            return B
 
     def bipartite(self):
         """
         Constructs the networkX bipartite graph associated to hypergraph.
 
         Returns
         -------
         bipartite : nx.Graph()
 
         Notes
         -----
         Creates a bipartite networkx graph from hypergraph.
-        The nodes and (hyper)edges of hypergraph become the nodes of bipartite graph.
-        For every (hyper)edge e in the hypergraph and node n in e there is an edge (n,e)
-        in the graph.
+        The nodes and (hyper)edges of hypergraph become the nodes of bipartite
+        graph. For every (hyper)edge e in the hypergraph and node n in e there
+        is an edge (n,e) in the graph.
 
         """
         B = nx.Graph()
-        E = self.edges
-        V = self.nodes
-        B.add_nodes_from(E, bipartite=1)
-        B.add_nodes_from(V, bipartite=0)
-        B.add_edges_from([(v, e) for e in E for v in self.edges[e]])
+        nodes = self._state_dict["labels"]["nodes"]
+        edges = self._state_dict["labels"]["edges"]
+        B.add_nodes_from(self.edges, bipartite=0)
+        B.add_nodes_from(self.nodes, bipartite=1)
+        B.add_edges_from([(v, e) for e in self.edges for v in self.edges[e]])
         return B
 
-    def dual(self, name=None):
+    def dual(self, name=None, switch_names=True):
         """
-        Constructs a new hypergraph with roles of edges and nodes of hypergraph reversed.
+        Constructs a new hypergraph with roles of edges and nodes of hypergraph
+        reversed.
 
         Parameters
         ----------
-        name : hashable
+        name : hashable, optional
+
+        switch_names : bool, optional, default = True
+            reverses edge_col and node_col names
+            unless edge_col = 'edges' and node_col = 'nodes'
 
         Returns
         -------
-        dual : hypergraph
-        """
-        if self.isstatic:
-            E = self.edges.restrict_to_levels((1, 0))
-            return Hypergraph(E, name=name, use_nwhy=self.nwhy)
-        else:
-            E = defaultdict(list)
-            for k, v in self.edges.incidence_dict.items():
-                for n in v:
-                    E[n].append(k)
-            return Hypergraph(E, name=name)
+        : hypergraph
 
-    def _collapse_nwhy(self, edges, rec):
         """
-        Helper method for collapsing nodes and edges when hypergraph
-        is static and using nwhy
+        dfp = self.edges.properties.copy()
+        if "level" in dfp.columns:
+            dfp = dfp.reset_index()
+            dfp.level = dfp.level.apply(lambda x: 1 * (x == 0))
+            dfp = dfp.set_index(["level", "id"])
 
-        Parameters
-        ----------
-        edges : bool
-            Collapse the edges if True, otherwise the nodes
-        rec : bool
-            return the equivalence classes
-        """
+        edge, node, wt = self._edge_col, self._node_col, self._cell_weight_col
+        df = self.dataframe.copy()
+        cprops = [col for col in df.columns if not col in [edge, node, wt]]
 
-        if edges:
-            d = self.g.collapse_edges(return_equivalence_class=rec)
-        else:
-            d = self.g.collapse_nodes(return_equivalence_class=rec)
+        df[[edge, node]] = df[[node, edge]]
+        if edge != "edges" or node != "nodes":
+            df = df.rename(columns={edge: self._node_col, node: self._edge_col})
+            node = self._edge_col
+            edge = self._node_col
 
-        if rec:
-            en = {
-                self.get_name(
-                    k, edges=edges
-                ): f"{self.get_name(k,edges=edges)}:{len(v)}"
-                for k, v in d.items()
-            }
-            ec = {
-                f"{self.get_name(k,edges=edges)}:{len(v)}": {
-                    self.get_name(vd, edges=edges) for vd in v
-                }
-                for k, v in d.items()
-            }
-        else:
-            en = {
-                self.get_name(
-                    k, edges=edges
-                ): f"{self.get_name(k,edges=edges)}:{v.pop()}"
-                for k, v in d.items()
-            }
-            ec = {}
-        lev = self.edges.keys[1 - 1 * edges]
-        E = self.edges.restrict_to_indices(sorted(d.keys()), level=1 - 1 * edges)
-        E.labels[str(lev)] = np.array([en[k] for k in E.labels[lev]])
-        if rec:
-            return E, ec
-        else:
-            return E
+        return Hypergraph(
+            df,
+            edge_col=edge,
+            node_col=node,
+            cell_weight_col=wt,
+            cell_properties=cprops,
+            properties=dfp,
+            name=name,
+        )
 
     def collapse_edges(
         self,
         name=None,
+        return_equivalence_classes=False,
         use_reps=None,
         return_counts=None,
-        return_equivalence_classes=False,
     ):
         """
-        Constructs a new hypergraph gotten by identifying edges containing the same nodes
+        Constructs a new hypergraph gotten by identifying edges containing the
+        same nodes
 
         Parameters
         ----------
-        name : hashable, optional, default: None
+        name : hashable, optional, default = None
 
-        return_equivalence_classes: boolean, optional, default: False
-            Returns a dictionary of edge equivalence classes keyed by frozen sets of nodes
+        return_equivalence_classes: boolean, optional, default = False
+            Returns a dictionary of edge equivalence classes keyed by frozen
+            sets of nodes
 
         Returns
         -------
         new hypergraph : Hypergraph
-            Equivalent edges are collapsed to a single edge named by a representative of the equivalent
-            edges followed by a colon and the number of edges it represents.
+            Equivalent edges are collapsed to a single edge named by a
+            representative of the equivalent edges followed by a colon and the
+            number of edges it represents.
 
         equivalence_classes : dict
-            A dictionary keyed by representative edge names with values equal to the edges in
-            its equivalence class
+            A dictionary keyed by representative edge names with values equal
+            to the edges in its equivalence class
 
         Notes
         -----
         Two edges are identified if their respective elements are the same.
-        Using this as an equivalence relation, the uids of the edges are partitioned into
-        equivalence classes.
+        Using this as an equivalence relation, the uids of the edges are
+        partitioned into equivalence classes.
 
-        A single edge from the collapsed edges followed by a colon and the number of elements
-        in its equivalence class as uid for the new edge
+        A single edge from the collapsed edges followed by a colon and the
+        number of elements in its equivalence class as uid for the new edge
 
 
         """
         if use_reps is not None or return_counts is not None:
             msg = """
-            use_reps ane return_counts are no longer supported keyword arguments and will throw
-            an error in the next release.
-            collapsed hypergraph automatically names collapsed objects by a string "rep:count"
+            use_reps ane return_counts are no longer supported keyword
+            arguments and will throw an error in the next release.
+            collapsed hypergraph automatically names collapsed objects by a
+            string "rep:count"
             """
             warnings.warn(msg, DeprecationWarning)
 
-        if self.nwhy:
-            temp = self._collapse_nwhy(True, return_equivalence_classes)
-        else:
-            temp = self.edges.collapse_identical_elements(
-                "_", return_equivalence_classes=return_equivalence_classes
-            )
+        temp = self.edges.collapse_identical_elements(
+            return_equivalence_classes=return_equivalence_classes
+        )
+
         if return_equivalence_classes:
-            return Hypergraph(temp[0], name, use_nwhy=self.nwhy), temp[1]
-        else:
-            return Hypergraph(temp, name, use_nwhy=self.nwhy)
+            return Hypergraph(temp[0].incidence_dict, name), temp[1]
+
+        return Hypergraph(temp.incidence_dict, name)
 
     def collapse_nodes(
         self,
         name=None,
-        use_reps=True,
-        return_counts=True,
         return_equivalence_classes=False,
+        use_reps=None,
+        return_counts=None,
     ):
         """
-        Constructs a new hypergraph gotten by identifying nodes contained by the same edges
+        Constructs a new hypergraph gotten by identifying nodes contained by
+        the same edges
 
         Parameters
         ----------
-        name: str, optional, default: None
+        name: str, optional, default = None
 
-        return_equivalence_classes: boolean, optional, default: False
-            Returns a dictionary of node equivalence classes keyed by frozen sets of edges
+        return_equivalence_classes: boolean, optional, default = False
+            Returns a dictionary of node equivalence classes keyed by frozen
+            sets of edges
 
-        use_reps : boolean, optional, default: False - Deprecated, this no longer works and will be removed
-            Choose a single element from the collapsed nodes as uid for the new node, otherwise uses
-            a frozen set of the uids of nodes in the equivalence class
+        use_reps : boolean, optional, default = False - Deprecated, this no
+            longer works and will be removed. Choose a single element from the
+            collapsed nodes as uid for the new node, otherwise uses a frozen
+            set of the uids of nodes in the equivalence class
 
-        return_counts: boolean, - Deprecated, this no longer works and will be removed
-            if use_reps is True the new nodes have uids given by a tuple of the rep
-            and the count
+        return_counts: boolean, - Deprecated, this no longer works and will be
+            removed if use_reps is True the new nodes have uids given by a
+            tuple of the rep and the count
 
         Returns
         -------
         new hypergraph : Hypergraph
 
         Notes
         -----
         Two nodes are identified if their respective memberships are the same.
-        Using this as an equivalence relation, the uids of the nodes are partitioned into
-        equivalence classes. A single member of the equivalence class is chosen to represent
-        the class followed by the number of members of the class.
+        Using this as an equivalence relation, the uids of the nodes are
+        partitioned into equivalence classes. A single member of the
+        equivalence class is chosen to represent the class followed by the
+        number of members of the class.
 
         Example
         -------
 
-            >>> h = Hypergraph(EntitySet('example',elements=[Entity('E1', ['a','b']),Entity('E2',['a','b'])]))
+            >>> h = Hypergraph(EntitySet('example',elements=[Entity('E1', /
+                                        ['a','b']),Entity('E2',['a','b'])]))
             >>> h.incidence_dict
             {'E1': {'a', 'b'}, 'E2': {'a', 'b'}}
             >>> h.collapse_nodes().incidence_dict
-            {'E1': {frozenset({'a', 'b'})}, 'E2': {frozenset({'a', 'b'})}} ### Fix this
+            {'E1': {frozenset({'a', 'b'})}, 'E2': {frozenset({'a', 'b'})}}
+            ### Fix this
             >>> h.collapse_nodes(use_reps=True).incidence_dict
             {'E1': {('a', 2)}, 'E2': {('a', 2)}}
 
         """
         if use_reps is not None or return_counts is not None:
             msg = """
-            use_reps ane return_counts are no longer supported keyword arguments and will throw
+            use_reps and return_counts are no longer supported keyword arguments and will throw
             an error in the next release.
             collapsed hypergraph automatically names collapsed objects by a string "rep:count"
             """
             warnings.warn(msg, DeprecationWarning)
 
-        if self.nwhy:
-            temp = self._collapse_nwhy(False, return_equivalence_classes)
-            if return_equivalence_classes:
-                return Hypergraph(temp[0], name, use_nwhy=self.nwhy), temp[1]
-            else:
-                return Hypergraph(temp, name, use_nwhy=self.nwhy)
-        else:
-            temp = self.dual().edges.collapse_identical_elements(
-                "_", return_equivalence_classes=return_equivalence_classes
-            )
+        temp = self.dual().edges.collapse_identical_elements(
+            return_equivalence_classes=return_equivalence_classes
+        )
 
-            if return_equivalence_classes:
-                return Hypergraph(temp[0], name, use_nwhy=self.nwhy).dual(), temp[1]
-            else:
-                return Hypergraph(temp, name, use_nwhy=self.nwhy).dual()
+        if return_equivalence_classes:
+            return Hypergraph(temp[0].incidence_dict).dual(), temp[1]
+
+        return Hypergraph(temp.incidence_dict, name).dual()
 
     def collapse_nodes_and_edges(
         self,
         name=None,
-        use_reps=True,
-        return_counts=True,
         return_equivalence_classes=False,
+        use_reps=None,
+        return_counts=None,
     ):
         """
         Returns a new hypergraph by collapsing nodes and edges.
 
         Parameters
         ----------
 
-        name: str, optional, default: None
-
-        use_reps: boolean, optional, default: False
-            Choose a single element from the collapsed elements as a representative
+        name: str, optional, default = None
 
-        return_counts: boolean, optional, default: True
-            if use_reps is True the new elements are keyed by a tuple of the rep
-            and the count
-
-        return_equivalence_classes: boolean, optional, default: False
-            Returns a dictionary of edge equivalence classes keyed by frozen sets of nodes
+        use_reps: boolean, optional, default = False
+            Choose a single element from the collapsed elements as a
+            representative
+
+        return_counts: boolean, optional, default = True
+            if use_reps is True the new elements are keyed by a tuple of the
+            rep and the count
+
+        return_equivalence_classes: boolean, optional, default = False
+            Returns a dictionary of edge equivalence classes keyed by frozen
+            sets of nodes
 
         Returns
         -------
         new hypergraph : Hypergraph
 
         Notes
         -----
-        Collapses the Nodes and Edges EntitySets. Two nodes(edges) are duplicates
-        if their respective memberships(elements) are the same. Using this as an
-        equivalence relation, the uids of the nodes(edges) are partitioned into
-        equivalence classes. A single member of the equivalence class is chosen to represent
-        the class followed by the number of members of the class.
+        Collapses the Nodes and Edges EntitySets. Two nodes(edges) are
+        duplicates if their respective memberships(elements) are the same.
+        Using this as an equivalence relation, the uids of the nodes(edges)
+        are partitioned into equivalence classes. A single member of the
+        equivalence class is chosen to represent the class followed by the
+        number of members of the class.
 
         Example
         -------
 
-            >>> h = Hypergraph(EntitySet('example',elements=[Entity('E1', ['a','b']),Entity('E2',['a','b'])]))
+            >>> h = Hypergraph(EntitySet('example',elements=[Entity('E1', /
+                                           ['a','b']),Entity('E2',['a','b'])]))
             >>> h.incidence_dict
             {'E1': {'a', 'b'}, 'E2': {'a', 'b'}}
             >>> h.collapse_nodes_and_edges().incidence_dict   ### Fix this
             {('E1', 2): {('a', 2)}}
 
         """
         if use_reps is not None or return_counts is not None:
             msg = """
-            use_reps ane return_counts are no longer supported keyword arguments and will throw
-            an error in the next release.
-            collapsed hypergraph automatically names collapsed objects by a string "rep:count"
+            use_reps and return_counts are no longer supported keyword
+            arguments and will throw an error in the next release.
+            collapsed hypergraph automatically names collapsed objects by a
+            string "rep:count"
             """
             warnings.warn(msg, DeprecationWarning)
 
         if return_equivalence_classes:
             temp, neq = self.collapse_nodes(
                 name="temp", return_equivalence_classes=True
             )
             ntemp, eeq = temp.collapse_edges(name=name, return_equivalence_classes=True)
             return ntemp, neq, eeq
-        else:
-            temp = self.collapse_nodes(name="temp")
-            return temp.collapse_edges(name=name)
 
-    def restrict_to_edges(self, edgeset, name=None):
-        """
-        Constructs a hypergraph using a subset of the edges in hypergraph
+        temp = self.collapse_nodes(name="temp")
+        return temp.collapse_edges(name=name)
+
+    def restrict_to_nodes(self, nodes, name=None):
+        """New hypergraph gotten by restricting to nodes
 
         Parameters
         ----------
-        edgeset: iterable of hashables or Entities
-            A subset of elements of the hypergraph edges
-
-        name: str, optional
+        nodes : Iterable
+            nodeids to restrict to
 
         Returns
         -------
-        new hypergraph : Hypergraph
-        """
-        if self._static:
-            E = self._edges
-            setsystem = E.restrict_to(sorted(E.indices(E.keys[0], list(edgeset))))
-            return Hypergraph(setsystem, name=name, use_nwhy=self.nwhy)
-        else:
-            inneredges = set()
-            for e in edgeset:
-                if isinstance(e, Entity):
-                    inneredges.add(e.uid)
-                else:
-                    inneredges.add(e)
-            return Hypergraph({e: self.edges[e] for e in inneredges}, name=name)
+        : hnx. Hypergraph
 
-    def restrict_to_nodes(self, nodeset, name=None):
         """
-        Constructs a new hypergraph by restricting the edges in the hypergraph to
-        the nodes referenced by nodeset.
+        keys = set(self._state_dict["labels"]["nodes"]).difference(nodes)
+        return self.remove(keys, level=1)
+
+    def restrict_to_edges(self, edges, name=None):
+        """New hypergraph gotten by restricting to edges
 
         Parameters
         ----------
-        nodeset: iterable of hashables
-            References a subset of elements of self.nodes
-
-        name: string, optional, default: None
+        edges : Iterable
+            edgeids to restrict to
 
         Returns
         -------
-        new hypergraph : Hypergraph
-        """
-        if self.isstatic:
-            E = self.edges.restrict_to_levels((1, 0))
-            setsystem = E.restrict_to(sorted(E.indices(E.keys[0], list(nodeset))))
-            return Hypergraph(
-                setsystem.restrict_to_levels((1, 0)), name=name, use_nwhy=self.nwhy
-            )
-        else:
-            memberships = set()
-            innernodes = set()
-            for node in nodeset:
-                innernodes.add(node)
-                if node in self.nodes:
-                    memberships.update(set(self.nodes[node].memberships))
-            newedgeset = dict()
-            for e in memberships:
-                if e in self.edges:
-                    temp = self.edges[e].uidset.intersection(innernodes)
-                    if temp:
-                        newedgeset[e] = Entity(e, temp, **self.edges[e].properties)
-            return Hypergraph(newedgeset, name=name)
+        hnx.Hypergraph
 
-    def toplexes(self, name=None, collapse=False, use_reps=False, return_counts=True):
         """
-        Returns a :term:`simple hypergraph` corresponding to self.
+        keys = set(self._state_dict["labels"]["edges"]).difference(edges)
+        return self.remove(keys, level=0)
 
-        Warning
-        -------
-        Collapsing is no longer supported inside the toplexes method. Instead generate a new
-        collapsed hypergraph and compute the toplexes of the new hypergraph.
+    def remove_edges(self, keys, name=None):
+        return self.remove(keys, level=0, name=name)
+
+    def remove_nodes(self, keys, name=None):
+        return self.remove(keys, level=1, name=name)
+
+    def remove(self, keys, level=None, name=None):
+        """Creates a new hypergraph with nodes and/or edges indexed by keys
+        removed. More efficient for creating a restricted hypergraph if the
+        restricted set is greater than what is being removed.
 
         Parameters
         ----------
-        name: str, optional, default: None
+        keys : list | tuple | set
+            node and/or edge id to restrict to
+        level : None, optional
+            Enter 0 to remove edges with ids in keys.
+            Enter 1 to remove nodes with ids in keys.
+            If None then all objects in nodes and edges with the id will
+            be removed.
 
-        # collapse: boolean, optional, default: False
-        #     Should the hypergraph be collapsed? This would preserve a link between duplicate maximal sets.
-        #     If False then only one of these sets will be used and uniqueness will be up to sets of equal size.
+        Returns
+        -------
+        : hnx.Hypergraph
+
+        """
+        rdfprop = self.properties.copy()
+        rdf = self.dataframe.copy()
+        if not isinstance(keys, (list, tuple, set)):
+            keys = list(keys)
+        if level == 0:
+            kdx = set(keys).intersection(set(self._state_dict["labels"]["edges"]))
+            for k in kdx:
+                rdfprop = rdfprop.drop((0, k))
+            rdf = rdf.loc[~rdf[self._edge_col].isin(kdx)]
+        elif level == 1:
+            kdx = set(keys).intersection(set(self._state_dict["labels"]["nodes"]))
+            for k in kdx:
+                rdfprop = rdfprop.drop((1, k))
+            rdf = rdf.loc[~rdf[self._node_col].isin(kdx)]
+        else:
+            rdfprop = rdfprop.reset_index()
+            kdx = set(keys).intersection(rdfprop.id.unique())
+            rdfprop = rdfprop.set_index("id")
+            rdfprop = rdfprop.drop(index=kdx)
+            rdf = rdf.loc[~rdf[self._edge_col].isin(kdx)]
+            rdf = rdf.loc[~rdf[self._node_col].isin(kdx)]
+
+        return Hypergraph(
+            setsystem=rdf,
+            edge_col=self._edge_col,
+            node_col=self._node_col,
+            cell_weight_col=self._cell_weight_col,
+            misc_cell_properties_col=self.edges._misc_cell_props_col,
+            properties=rdfprop,
+            misc_properties_col=self.edges._misc_props_col,
+        )
 
-        # use_reps: boolean, optional, default: False
-        #     If collapse=True then each toplex will be named by a representative of the set of
-        #     equivalent edges, default is False (see collapse_edges).
+    def toplexes(self, name=None):
+        """
+        Returns a :term:`simple hypergraph` corresponding to self.
 
-        return_counts: boolean, optional, default: True
-            # If collapse=True then each toplex will be named by a tuple of the representative
-            # of the set of equivalent edges and their count
+        Warning
+        -------
+        Collapsing is no longer supported inside the toplexes method. Instead
+        generate a new collapsed hypergraph and compute the toplexes of the
+        new hypergraph.
 
+        Parameters
+        ----------
+        name: str, optional, default = None
         """
-        # TODO: There is a better way to do this....need to refactor
-        if collapse:
-            if len(self.edges) > 20:  # TODO: Determine how big is too big.
-                warnings.warn(
-                    "Collapsing a hypergraph can take a long time. It may be preferable to collapse the graph first and pickle it then apply the toplex method separately."
-                )
-            temp = self.collapse_edges()
-        else:
-            temp = self
 
-        if collapse:
-            msg = """
-            collapse, return_counts, and use_reps are no longer supported keyword arguments 
-            and will throw an error in the next release.
-            """
-            warnings.warn(msg, DeprecationWarning)
+        thdict = {}
+        for e in self.edges:
+            thdict[e] = self.edges[e]
 
-        thdict = dict()
-        if self.nwhy:
-            tops = self.g.toplexes()
-            E = self.edges.restrict_to(tops)
-            return Hypergraph(E, use_nwhy=True)
-        else:
-            if self.isstatic:
-                for e in temp.edges:
-                    thdict[e] = temp.edges[e]
-            else:
-                for e in temp.edges:
-                    thdict[e] = temp.edges[e].uidset
-            tops = list()
-            for e in temp.edges:
-                flag = True
-                old_tops = list(tops)
-                for top in old_tops:
-                    if set(thdict[e]).issubset(thdict[top]):
-                        flag = False
-                        break
-                    elif set(thdict[top]).issubset(thdict[e]):
-                        tops.remove(top)
-                if flag:
-                    tops += [e]
-            return self.restrict_to_edges(tops, name=name)
+        tops = []
+        for e in self.edges:
+            flag = True
+            old_tops = list(tops)
+            for top in old_tops:
+                if set(thdict[e]).issubset(thdict[top]):
+                    flag = False
+                    break
+
+                if set(thdict[top]).issubset(thdict[e]):
+                    tops.remove(top)
+            if flag:
+                tops += [e]
+        return self.restrict_to_edges(tops, name=name)
 
     def is_connected(self, s=1, edges=False):
         """
-        Determines if hypergraph is :term:`s-connected <s-connected, s-node-connected>`.
+        Determines if hypergraph is :term:`s-connected <s-connected,
+        s-node-connected>`.
 
         Parameters
         ----------
-        s: int, optional, default: 1
+        s: int, optional, default 1
 
-        edges: boolean, optional, default: False
+        edges: boolean, optional, default = False
             If True, will determine if s-edge-connected.
             For s=1 s-edge-connected is the same as s-connected.
 
         Returns
         -------
         is_connected : boolean
 
@@ -1722,422 +1620,357 @@
         A hypergraph is s edge connected if for any two edges e0,en
         there exists a sequence of edges e0,e1,e2,...,e(n-1),en
         such that every consecutive pair of edges e(i),e(i+1)
         share at least s nodes.
 
         """
 
-        if self.isstatic:
-            g = self.get_linegraph(s=s, edges=edges)
-            if self.nwhy:
-                return g.is_s_connected()
-            else:
-                return nx.is_connected(g)
-        else:
-            if edges:
-                A = self.edge_adjacency_matrix(s=s)
-            else:
-                A = self.adjacency_matrix(s=s)
-            g = nx.from_scipy_sparse_matrix(A)
-            return nx.is_connected(g)
+        g = self.get_linegraph(s=s, edges=edges)
+        is_connected = None
+
+        try:
+            is_connected = nx.is_connected(g)
+        except nx.NetworkXPointlessConcept:
+            warnings.warn("Graph is null; ")
+            is_connected = False
+
+        return is_connected
 
     def singletons(self):
         """
         Returns a list of singleton edges. A singleton edge is an edge of
         size 1 with a node of degree 1.
 
         Returns
         -------
         singles : list
             A list of edge uids.
         """
-        if self.nwhy:
-            return self.edges.translate(0, self.g.singletons())
-        else:
-            M, rdict, cdict = self.incidence_matrix(index=True)
-            idx = np.argmax(M.shape)  # which axis has fewest members? if 1 then columns
-            cols = M.sum(idx)  # we add down the row index if there are fewer columns
-            singles = list()
-            for c in range(cols.shape[(idx + 1) % 2]):  # index along opposite axis
-                if cols[idx * c, c * ((idx + 1) % 2)] == 1:
-                    # then see if the singleton entry in that column is also singleton in its row
-                    # find the entry
-                    if idx == 0:
-                        r = np.argmax(M.getcol(c))
-                        # and get its sum
-                        s = np.sum(M.getrow(r))
-                        # if this is also 1 then the entry in r,c represents a singleton
-                        # so we want to change that entry to 0 and remove the row.
-                        # this means we want to remove the edge corresponding to c
-                        if s == 1:
-                            singles.append(cdict[c])
-                    else:  # switch the role of r and c
-                        r = np.argmax(M.getrow(c))
-                        s = np.sum(M.getcol(r))
-                        if s == 1:
-                            singles.append(cdict[r])
-            return singles
+
+        M, _, cdict = self.incidence_matrix(index=True)
+        # which axis has fewest members? if 1 then columns
+        idx = np.argmax(M.shape).tolist()
+        # we add down the row index if there are fewer columns
+        cols = M.sum(idx)
+        singles = []
+        # index along opposite axis with one entry each
+        for c in np.nonzero((cols - 1 == 0))[(idx + 1) % 2]:
+            # if the singleton entry in that column is also
+            # singleton in its row find the entry
+            if idx == 0:
+                r = np.argmax(M.getcol(c))
+                # and get its sum
+                s = np.sum(M.getrow(r))
+                # if this is also 1 then the entry in r,c represents a
+                # singleton so we want to change that entry to 0 and
+                # remove the row. this means we want to remove the
+                # edge corresponding to c
+                if s == 1:
+                    singles.append(cdict[c])
+            else:  # switch the role of r and c
+                r = np.argmax(M.getrow(c))
+                s = np.sum(M.getcol(r))
+                if s == 1:
+                    singles.append(cdict[r])
+        return singles
 
     def remove_singletons(self, name=None):
         """
         Constructs clone of hypergraph with singleton edges removed.
 
-        Parameters
-        ----------
-        name: str, optional, default: None
-
         Returns
         -------
         new hypergraph : Hypergraph
 
         """
-        E = [e for e in self.edges if e not in self.singletons()]
-        return self.restrict_to_edges(E)
+        singletons = self.singletons()
+        if len(singletons) > len(self.edges):
+            E = [e for e in self.edges if e not in singletons]
+            return self.restrict_to_edges(E, name=name)
+        else:
+            return self.remove(singletons, level=0, name=name)
 
     def s_connected_components(self, s=1, edges=True, return_singletons=False):
         """
-        Returns a generator for the :term:`s-edge-connected components <s-edge-connected component>`
-        or the :term:`s-node-connected components <s-connected component, s-node-connected component>`
-        of the hypergraph.
+        Returns a generator for the :term:`s-edge-connected components
+        <s-edge-connected component>`
+        or the :term:`s-node-connected components <s-connected component,
+        s-node-connected component>` of the hypergraph.
 
         Parameters
         ----------
-        s : int, optional, default: 1
+        s : int, optional, default 1
 
-        edges : boolean, optional, default: True
-            If True will return edge components, if False will return node components
-        return_singletons : bool, optional, default : False
+        edges : boolean, optional, default = True
+            If True will return edge components, if False will return node
+            components
+        return_singletons : bool, optional, default = False
 
         Notes
         -----
         If edges=True, this method returns the s-edge-connected components as
         lists of lists of edge uids.
         An s-edge-component has the property that for any two edges e1 and e2
         there is a sequence of edges starting with e1 and ending with e2
         such that pairwise adjacent edges in the sequence intersect in at least
         s nodes. If s=1 these are the path components of the hypergraph.
 
         If edges=False this method returns s-node-connected components.
         A list of sets of uids of the nodes which are s-walk connected.
         Two nodes v1 and v2 are s-walk-connected if there is a
-        sequence of nodes starting with v1 and ending with v2 such that pairwise
-        adjacent nodes in the sequence share s edges. If s=1 these are the
-        path components of the hypergraph.
+        sequence of nodes starting with v1 and ending with v2 such that
+        pairwise adjacent nodes in the sequence share s edges. If s=1 these
+        are the path components of the hypergraph.
 
         Example
         -------
             >>> S = {'A':{1,2,3},'B':{2,3,4},'C':{5,6},'D':{6}}
             >>> H = Hypergraph(S)
 
             >>> list(H.s_components(edges=True))
             [{'C', 'D'}, {'A', 'B'}]
             >>> list(H.s_components(edges=False))
             [{1, 2, 3, 4}, {5, 6}]
 
         Yields
         ------
         s_connected_components : iterator
-            Iterator returns sets of uids of the edges (or nodes) in the s-edge(node)
-            components of hypergraph.
+            Iterator returns sets of uids of the edges (or nodes) in the
+            s-edge(node) components of hypergraph.
 
         """
-        components = list()
-
-        if self.nwhy:
-            g = self.get_linegraph(s, edges=edges)
-            if return_singletons:
-                allobjects = set(self.edges) if edges == True else set(self.nodes)
-                for c in g.s_connected_components():
-                    comp = {self.get_name(nd, edges=edges) for nd in c}
-                    allobjects.difference_update(comp)
-                for c in g.s_connected_components():
-                    yield {self.get_name(nd, edges=edges) for nd in c}
-                for obj in allobjects:
-                    yield {obj}
-            else:
-                for c in g.s_connected_components():
-                    comp = {self.get_name(nd, edges=edges) for nd in c}
-                    yield comp
-
-        elif self.isstatic:
-            g = self.get_linegraph(s, edges=edges)
-            for c in nx.connected_components(g):
-                if not return_singletons and len(c) == 1:
-                    continue
-                yield {self.get_name(n, edges=edges) for n in c}
-        else:
-            if edges:
-                A, coldict = self.edge_adjacency_matrix(s=s, index=True)
-                G = nx.from_scipy_sparse_matrix(A)
-                # if not return_singletons:
-                #     temp = [c for c in nx.connected_components(G) if len(c) > 1]
-                # else:
-                #     temp = nx.connected_components(G)
-                for c in nx.connected_components(G):
-                    if not return_singletons and len(c) == 1:
-                        continue
-                    yield {coldict[n] for n in c}
-            else:
-                A, rowdict = self.adjacency_matrix(s=s, index=True)
-                G = nx.from_scipy_sparse_matrix(A)
-                for c in nx.connected_components(G):
-                    if not return_singletons:
-                        if len(c) == 1:
-                            continue
-                    yield {rowdict[n] for n in c}
+        g = self.get_linegraph(s, edges=edges)
+        for c in nx.connected_components(g):
+            if not return_singletons and len(c) == 1:
+                continue
+            yield c
 
-    def s_component_subgraphs(self, s=1, edges=True, return_singletons=False):
+    def s_component_subgraphs(
+        self, s=1, edges=True, return_singletons=False, name=None
+    ):
         """
 
-        Returns a generator for the induced subgraphs of s_connected components.
-        Removes singletons unless return_singletons is set to True. Computed using
-        s-linegraph generated either by the hypergraph (edges=True) or its dual
-        (edges = False)
+        Returns a generator for the induced subgraphs of s_connected
+        components. Removes singletons unless return_singletons is set to True.
+        Computed using s-linegraph generated either by the hypergraph
+        (edges=True) or its dual (edges = False)
 
         Parameters
         ----------
-        s : int, optional, default: 1
+        s : int, optional, default 1
 
         edges : boolean, optional, edges=False
             Determines if edge or node components are desired. Returns
-            subgraphs equal to the hypergraph restricted to each set of nodes(edges) in the
-            s-connected components or s-edge-connected components
+            subgraphs equal to the hypergraph restricted to each set of
+            nodes(edges) in the s-connected components or s-edge-connected
+            components
         return_singletons : bool, optional
 
         Yields
         ------
         s_component_subgraphs : iterator
             Iterator returns subgraphs generated by the edges (or nodes) in the
             s-edge(node) components of hypergraph.
 
         """
         for idx, c in enumerate(
             self.s_components(s=s, edges=edges, return_singletons=return_singletons)
         ):
             if edges:
-                yield self.restrict_to_edges(c, name=f"{self.name}:{idx}")
+                yield self.restrict_to_edges(c, name=f"{name or self.name}:{idx}")
             else:
-                yield self.restrict_to_nodes(c, name=f"{self.name}:{idx}")
+                yield self.restrict_to_nodes(c, name=f"{name or self.name}:{idx}")
 
     def s_components(self, s=1, edges=True, return_singletons=True):
         """
         Same as s_connected_components
 
         See Also
         --------
         s_connected_components
         """
         return self.s_connected_components(
             s=s, edges=edges, return_singletons=return_singletons
         )
 
-    def connected_components(self, edges=False, return_singletons=True):
+    def connected_components(self, edges=False):
         """
         Same as :meth:`s_connected_components` with s=1, but nodes are returned
         by default. Return iterator.
 
         See Also
         --------
         s_connected_components
         """
         return self.s_connected_components(edges=edges, return_singletons=True)
 
-    def connected_component_subgraphs(self, return_singletons=True):
+    def connected_component_subgraphs(self, return_singletons=True, name=None):
         """
         Same as :meth:`s_component_subgraphs` with s=1. Returns iterator
 
         See Also
         --------
         s_component_subgraphs
         """
-        return self.s_component_subgraphs(return_singletons=return_singletons)
+        return self.s_component_subgraphs(
+            return_singletons=return_singletons, name=name
+        )
 
-    def components(self, edges=False, return_singletons=True):
+    def components(self, edges=False):
         """
         Same as :meth:`s_connected_components` with s=1, but nodes are returned
         by default. Return iterator.
 
         See Also
         --------
         s_connected_components
         """
         return self.s_connected_components(s=1, edges=edges)
 
-    def component_subgraphs(self, return_singletons=False):
+    def component_subgraphs(self, return_singletons=False, name=None):
         """
         Same as :meth:`s_components_subgraphs` with s=1. Returns iterator.
 
         See Also
         --------
         s_component_subgraphs
         """
-        return self.s_component_subgraphs(return_singletons=return_singletons)
+        return self.s_component_subgraphs(
+            return_singletons=return_singletons, name=name
+        )
 
     def node_diameters(self, s=1):
         """
         Returns the node diameters of the connected components in hypergraph.
 
         Parameters
         ----------
         list of the diameters of the s-components and
         list of the s-component nodes
         """
-        if self.nwhy:
-            g = self.get_linegraph(s, edges=False)
-            if g.is_s_connected():
-                return g.s_diameter()
-            else:
-                diameters = list()
-                nodelists = list()
-                for c in g.s_connected_components():
-                    tc = self.edges.labs(1)[c]
-                    nodelists.append(tc)
-                    diameters.append(self.restrict_to_nodes(tc).node_diameters(s=s))
-        else:
-            A, coldict = self.adjacency_matrix(s=s, index=True)
-            G = nx.from_scipy_sparse_matrix(A)
-            diams = []
-            comps = []
-            for c in nx.connected_components(G):
-                diamc = nx.diameter(G.subgraph(c))
-                temp = set()
-                for e in c:
-                    temp.add(coldict[e])
-                comps.append(temp)
-                diams.append(diamc)
-            loc = np.argmax(diams)
-            return diams[loc], diams, comps
+        A, coldict = self.adjacency_matrix(s=s, index=True)
+        G = nx.from_scipy_sparse_matrix(A)
+        diams = []
+        comps = []
+        for c in nx.connected_components(G):
+            diamc = nx.diameter(G.subgraph(c))
+            temp = set()
+            for e in c:
+                temp.add(coldict[e])
+            comps.append(temp)
+            diams.append(diamc)
+        loc = np.argmax(diams).tolist()
+        return diams[loc], diams, comps
 
     def edge_diameters(self, s=1):
         """
         Returns the edge diameters of the s_edge_connected component subgraphs
         in hypergraph.
 
         Parameters
         ----------
-        s : int, optional, default: 1
+        s : int, optional, default 1
 
         Returns
         -------
         maximum diameter : int
 
         list of diameters : list
             List of edge_diameters for s-edge component subgraphs in hypergraph
 
         list of component : list
             List of the edge uids in the s-edge component subgraphs.
 
         """
-        if self.nwhy:
-            g = self.get_linegraph(s, edges=True)
-            if g.is_s_connected():
-                return g.s_diameter()
-            else:
-                diameters = list()
-                edgelists = list()
-                for c in g.s_connected_components():
-                    tc = self.edges.labs(0)[c]
-                    edgelists.append(tc)
-                    diameters.append(self.restrict_to_edges(tc).edge_diameters(s=s))
-        else:
-            A, coldict = self.edge_adjacency_matrix(s=s, index=True)
-            G = nx.from_scipy_sparse_matrix(A)
-            diams = []
-            comps = []
-            for c in nx.connected_components(G):
-                diamc = nx.diameter(G.subgraph(c))
-                temp = set()
-                for e in c:
-                    temp.add(coldict[e])
-                comps.append(temp)
-                diams.append(diamc)
-            loc = np.argmax(diams)
-            return diams[loc], diams, comps
+        A, coldict = self.edge_adjacency_matrix(s=s, index=True)
+        G = nx.from_scipy_sparse_matrix(A)
+        diams = []
+        comps = []
+        for c in nx.connected_components(G):
+            diamc = nx.diameter(G.subgraph(c))
+            temp = set()
+            for e in c:
+                temp.add(coldict[e])
+            comps.append(temp)
+            diams.append(diamc)
+        loc = np.argmax(diams).tolist()
+        return diams[loc], diams, comps
 
     def diameter(self, s=1):
         """
-        Returns the length of the longest shortest s-walk between nodes in hypergraph
+        Returns the length of the longest shortest s-walk between nodes in
+        hypergraph
 
         Parameters
         ----------
-        s : int, optional, default: 1
+        s : int, optional, default 1
 
         Returns
         -------
         diameter : int
 
         Raises
         ------
         HyperNetXError
             If hypergraph is not s-edge-connected
 
         Notes
         -----
         Two nodes are s-adjacent if they share s edges.
-        Two nodes v_start and v_end are s-walk connected if there is a sequence of
-        nodes v_start, v_1, v_2, ... v_n-1, v_end such that consecutive nodes
-        are s-adjacent. If the graph is not connected, an error will be raised.
+        Two nodes v_start and v_end are s-walk connected if there is a
+        sequence of nodes v_start, v_1, v_2, ... v_n-1, v_end such that
+        consecutive nodes are s-adjacent. If the graph is not connected,
+        an error will be raised.
 
         """
-        if self.nwhy:
-            g = self.get_linegraph(s, edges=False)
-            if g.is_s_connected():
-                return g.s_diameter()
-            else:
-                raise HyperNetXError(f"Hypergraph is not s-connected. s={s}")
-        else:
-            A = self.adjacency_matrix(s=s)
-            G = nx.from_scipy_sparse_matrix(A)
-            if nx.is_connected(G):
-                return nx.diameter(G)
-            else:
-                raise HyperNetXError(f"Hypergraph is not s-connected. s={s}")
+        A = self.adjacency_matrix(s=s)
+        G = nx.from_scipy_sparse_matrix(A)
+        if nx.is_connected(G):
+            return nx.diameter(G)
+
+        raise HyperNetXError(f"Hypergraph is not s-connected. s={s}")
 
     def edge_diameter(self, s=1):
         """
-        Returns the length of the longest shortest s-walk between edges in hypergraph
+        Returns the length of the longest shortest s-walk between edges in
+        hypergraph
 
         Parameters
         ----------
-        s : int, optional, default: 1
+        s : int, optional, default 1
 
         Return
         ------
         edge_diameter : int
 
         Raises
         ------
         HyperNetXError
             If hypergraph is not s-edge-connected
 
         Notes
         -----
         Two edges are s-adjacent if they share s nodes.
-        Two nodes e_start and e_end are s-walk connected if there is a sequence of
-        edges e_start, e_1, e_2, ... e_n-1, e_end such that consecutive edges
-        are s-adjacent. If the graph is not connected, an error will be raised.
+        Two nodes e_start and e_end are s-walk connected if there is a
+        sequence of edges e_start, e_1, e_2, ... e_n-1, e_end such that
+        consecutive edges are s-adjacent. If the graph is not connected, an
+        error will be raised.
 
         """
-        if self.nwhy:
-            g = self.get_linegraph(s, edges=True)
-            if g.is_s_connected():
-                return g.s_diameter()
-            else:
-                raise HyperNetXError(f"Hypergraph is not s-connected. s={s}")
-        else:
-            A = self.edge_adjacency_matrix(s=s)
-            G = nx.from_scipy_sparse_matrix(A)
-            if nx.is_connected(G):
-                return nx.diameter(G)
-            else:
-                raise HyperNetXError(f"Hypergraph is not s-connected. s={s}")
+        A = self.edge_adjacency_matrix(s=s)
+        G = nx.from_scipy_sparse_matrix(A)
+        if nx.is_connected(G):
+            return nx.diameter(G)
+
+        raise HyperNetXError(f"Hypergraph is not s-connected. s={s}")
 
     def distance(self, source, target, s=1):
         """
-        Returns the shortest s-walk distance between two nodes in the hypergraph.
+        Returns the shortest s-walk distance between two nodes in the
+        hypergraph.
 
         Parameters
         ----------
         source : node.uid or node
             a node in the hypergraph
 
         target : node.uid or node
@@ -2161,63 +1994,41 @@
         at least s edges. The length of the shortest s-walk is 1 less than
         the number of nodes in the path sequence.
 
         Uses the networkx shortest_path_length method on the graph
         generated by the s-adjacency matrix.
 
         """
-        if self.isstatic:
-            g = self.get_linegraph(s=s, edges=False)
-            src = self.get_id(source, edges=False)
-            tgt = self.get_id(target, edges=False)
-            try:
-                if self.nwhy:
-                    d = g.s_distance(src, tgt)
-                    if d == -1:
-                        warnings.warn(f"No {s}-path between {source} and {target}")
-                        return np.inf
-                    else:
-                        return d
-                else:
-                    return nx.shortest_path(g, src, tgt)
-            except:
-                warnings.warn(f"No {s}-path between {source} and {target}")
-                return np.inf
-        else:
-            if isinstance(source, Entity):
-                source = source.uid
-            if isinstance(target, Entity):
-                target = target.uid
-            A, rowdict = self.adjacency_matrix(s=s, index=True)
-            g = nx.from_scipy_sparse_matrix(A)
-            rkey = {v: k for k, v in rowdict.items()}
-            try:
-                path = nx.shortest_path_length(g, rkey[source], rkey[target])
-                return path
-            except:
-                warnings.warn(f"No {s}-path between {source} and {target}")
-                return np.inf
+        g = self.get_linegraph(s=s, edges=False)
+        try:
+            dist = nx.shortest_path_length(g, source, target)
+        except (nx.NetworkXNoPath, nx.NodeNotFound):
+            warnings.warn(f"No {s}-path between {source} and {target}")
+            dist = np.inf
+
+        return dist
 
     def edge_distance(self, source, target, s=1):
-        """XX TODO: still need to return path and translate into user defined nodes and edges
-        Returns the shortest s-walk distance between two edges in the hypergraph.
+        """XX TODO: still need to return path and translate into user defined
+        nodes and edges Returns the shortest s-walk distance between two edges
+        in the hypergraph.
 
         Parameters
         ----------
         source : edge.uid or edge
             an edge in the hypergraph
 
         target : edge.uid or edge
             an edge in the hypergraph
 
         s : positive integer
             the number of intersections between pairwise consecutive edges
 
         TODO: add edge weights
-        weight : None or string, optional, default: None
+        weight : None or string, optional, default = None
             if None then all edges have weight 1. If string then edge attribute
             string is used if available.
 
 
         Returns
         -------
         s- walk distance : the shortest s-walk edge distance
@@ -2228,168 +2039,165 @@
         See Also
         --------
         distance
 
         Notes
         -----
             The s-distance is the shortest s-walk length between the edges.
-            An s-walk between edges is a sequence of edges such that consecutive pairwise
-            edges intersect in at least s nodes. The length of the shortest s-walk is 1 less than
-            the number of edges in the path sequence.
+            An s-walk between edges is a sequence of edges such that
+            consecutive pairwise edges intersect in at least s nodes. The
+            length of the shortest s-walk is 1 less than the number of edges
+            in the path sequence.
 
             Uses the networkx shortest_path_length method on the graph
             generated by the s-edge_adjacency matrix.
 
         """
-        if self.isstatic:
-            g = self.get_linegraph(s=s, edges=True)
-            src = self.get_id(source, edges=True)
-            tgt = self.get_id(target, edges=True)
-            try:
-                if self.nwhy:
-                    d = g.s_distance(src, tgt)
-                    if d == -1:
-                        warnings.warn(f"No {s}-path between {source} and {target}")
-                        return np.inf
-                    else:
-                        return d
-                else:
-                    return nx.shortest_path(g, src, tgt)
-            except:
-                warnings.warn(f"No {s}-path between {source} and {target}")
-                return np.inf
-        else:
-            if isinstance(source, Entity):
-                source = source.uid
-            if isinstance(target, Entity):
-                target = target.uid
-            A, coldict = self.edge_adjacency_matrix(s=s, index=True)
-            g = nx.from_scipy_sparse_matrix(A)
-            ckey = {v: k for k, v in coldict.items()}
-            try:
-                path = nx.shortest_path_length(g, ckey[source], ckey[target])
-                return path
-            except:
-                warnings.warn(f"No {s}-path between {source} and {target}")
-                return np.inf
+        g = self.get_linegraph(s=s, edges=True)
+        try:
+            edge_dist = nx.shortest_path_length(g, source, target)
+        except (nx.NetworkXNoPath, nx.NodeNotFound):
+            warnings.warn(f"No {s}-path between {source} and {target}")
+            edge_dist = np.inf
+
+        return edge_dist
 
-    def dataframe(self, sort_rows=False, sort_columns=False, cell_weights=True):
+    def incidence_dataframe(
+        self, sort_rows=False, sort_columns=False, cell_weights=True
+    ):
         """
         Returns a pandas dataframe for hypergraph indexed by the nodes and
         with column headers given by the edge names.
 
         Parameters
         ----------
-        sort_rows : bool, optional, default=True
+        sort_rows : bool, optional, default =True
             sort rows based on hashable node names
-        sort_columns : bool, optional, default=True
+        sort_columns : bool, optional, default =True
             sort columns based on hashable edge names
-        cell_weights : bool, optional, default=True
-            if self.isstatic then include cell weights
+        cell_weights : bool, optional, default =True
 
         """
-        if self.isstatic:
-            mat, rdx, cdx = self.edges.incidence_matrix(index=True, weights=True)
-        else:
-            mat, rdx, cdx = self.edges.incidence_matrix(index=True)
-        index = [rdx[i] for i in rdx]
-        columns = [cdx[j] for j in cdx]
-        df = pd.DataFrame(mat.todense(), index=index, columns=columns)
+
+        ## An entity dataframe is already an incidence dataframe.
+        df = self.E.dataframe.pivot(
+            index=self.E._data_cols[1],
+            columns=self.E._data_cols[0],
+            values=self.E._cell_weight_col,
+        ).fillna(0)
+
         if sort_rows:
-            df = df.sort_index()
+            df = df.sort_index("index")
         if sort_columns:
-            df = df[sorted(columns)]
+            df = df.sort_index("columns")
+        if not cell_weights:
+            df[df > 0] = 1
+
         return df
 
     @classmethod
-    def from_bipartite(
-        cls, B, set_names=("edges", "nodes"), name=None, static=False, use_nwhy=False
-    ):
+    @warn_nwhy
+    def from_bipartite(cls, B, set_names=("edges", "nodes"), name=None, **kwargs):
         """
         Static method creates a Hypergraph from a bipartite graph.
 
         Parameters
         ----------
 
         B: nx.Graph()
             A networkx bipartite graph. Each node in the graph has a property
-            'bipartite' taking the value of 0 or 1 indicating a 2-coloring of the graph.
+            'bipartite' taking the value of 0 or 1 indicating a 2-coloring of
+            the graph.
 
-        set_names: iterable of length 2, optional, default = ['nodes','edges']
-            Category names assigned to the graph nodes associated to each bipartite set
+        set_names: iterable of length 2, optional, default = ['edges','nodes']
+            Category names assigned to the graph nodes associated to each
+            bipartite set
 
-        name: hashable
-
-        static: bool
+        name: hashable, optional
 
         Returns
         -------
          : Hypergraph
 
         Notes
         -----
         A partition for the nodes in a bipartite graph generates a hypergraph.
 
             >>> import networkx as nx
             >>> B = nx.Graph()
             >>> B.add_nodes_from([1, 2, 3, 4], bipartite=0)
             >>> B.add_nodes_from(['a', 'b', 'c'], bipartite=1)
-            >>> B.add_edges_from([(1, 'a'), (1, 'b'), (2, 'b'), (2, 'c'), (3, 'c'), (4, 'a')])
+            >>> B.add_edges_from([(1, 'a'), (1, 'b'), (2, 'b'), (2, 'c'), /
+                (3, 'c'), (4, 'a')])
             >>> H = Hypergraph.from_bipartite(B)
             >>> H.nodes, H.edges
-            # output: (EntitySet(_:Nodes,[1, 2, 3, 4],{}), EntitySet(_:Edges,['b', 'c', 'a'],{}))
+            # output: (EntitySet(_:Nodes,[1, 2, 3, 4],{}), /
+            # EntitySet(_:Edges,['b', 'c', 'a'],{}))
 
         """
-        # TODO: Add filepath keyword to signatures here and with dataframe and numpy array
+
         edges = []
         nodes = []
         for n, d in B.nodes(data=True):
-            if d["bipartite"] == 0:
+            if d["bipartite"] == 1:
                 nodes.append(n)
             else:
                 edges.append(n)
 
         if not bipartite.is_bipartite_node_set(B, nodes):
             raise HyperNetXError(
                 "Error: Method requires a 2-coloring of a bipartite graph."
             )
 
-        if static:
-            elist = []
-            for e in list(B.edges):
-                if e[0] in edges:
-                    elist.append([e[0], e[1]])
-                else:
-                    elist.append([e[1], e[0]])
-            df = pd.DataFrame(elist, columns=set_names)
-            E = StaticEntitySet(entity=df)
-            name = name or "_"
-            return Hypergraph(E, name=name, use_nwhy=use_nwhy)
-        else:
-            node_entities = {
-                n: Entity(n, [], properties=B.nodes(data=True)[n]) for n in nodes
-            }
-            edge_dict = {
-                e: [node_entities[n] for n in list(B.neighbors(e))] for e in edges
-            }
-            name = name or "_"
-            return Hypergraph(setsystem=edge_dict, name=name)
+        elist = []
+        for e in list(B.edges):
+            if e[0] in edges:
+                elist.append([e[0], e[1]])
+            else:
+                elist.append([e[1], e[0]])
+        df = pd.DataFrame(elist, columns=set_names)
+        return Hypergraph(df, name=name, **kwargs)
 
     @classmethod
+    def from_incidence_matrix(
+        cls,
+        M,
+        node_names=None,
+        edge_names=None,
+        node_label="nodes",
+        edge_label="edges",
+        name=None,
+        key=None,
+        **kwargs,
+    ):
+        """
+        Same as from_numpy_array.
+        """
+        return Hypergraph.from_numpy_array(
+            M,
+            node_names=node_names,
+            edge_names=edge_names,
+            node_label=node_label,
+            edge_label=edge_label,
+            name=name,
+            key=key,
+        )
+
+    @classmethod
+    @warn_nwhy
     def from_numpy_array(
         cls,
         M,
         node_names=None,
         edge_names=None,
         node_label="nodes",
         edge_label="edges",
         name=None,
         key=None,
-        static=False,
-        use_nwhy=False,
+        **kwargs,
     ):
         """
         Create a hypergraph from a real valued matrix represented as a 2 dimensionsl numpy array.
         The matrix is converted to a matrix of 0's and 1's so that any truthy cells are converted to 1's and
         all others to 0's.
 
         Parameters
@@ -2426,15 +2234,15 @@
         # Create names for nodes and edges
         # Validate the size of the node and edge arrays
 
         M = np.array(M)
         if len(M.shape) != (2):
             raise HyperNetXError("Input requires a 2 dimensional numpy array")
         # apply boolean key if available
-        if key:
+        if key is not None:
             M = key(M)
 
         if node_names is not None:
             nodenames = np.array(node_names)
             if len(nodenames) != M.shape[0]:
                 raise HyperNetXError(
                     "Number of node names does not match number of rows."
@@ -2447,63 +2255,38 @@
             if len(edgenames) != M.shape[1]:
                 raise HyperNetXError(
                     "Number of edge_names does not match number of columns."
                 )
         else:
             edgenames = np.array([f"e{jdx}" for jdx in range(M.shape[1])])
 
-        if static or use_nwhy:
-            arr = np.array(M)
-            if key:
-                arr = key(arr) * 1
-            arr = arr.transpose()
-            labels = OrderedDict([(edge_label, edgenames), (node_label, nodenames)])
-            E = StaticEntitySet(arr=arr, labels=labels)
-            return Hypergraph(E, name=name, use_nwhy=use_nwhy)
-
-        else:
-            # Remove empty column indices from M columns and edgenames
-            colidx = np.array([jdx for jdx in range(M.shape[1]) if any(M[:, jdx])])
-            colidxsum = np.sum(colidx)
-            if not colidxsum:
-                return Hypergraph()
-            else:
-                M = M[:, colidx]
-                edgenames = edgenames[colidx]
-                edict = dict()
-                # Create an EntitySet of edges from M
-                for jdx, e in enumerate(edgenames):
-                    edict[e] = nodenames[
-                        [idx for idx in range(M.shape[0]) if M[idx, jdx]]
-                    ]
-                return Hypergraph(edict, name=name)
+        df = pd.DataFrame(M, columns=edgenames, index=nodenames)
+        return Hypergraph.from_incidence_dataframe(df, name=name)
 
     @classmethod
-    def from_dataframe(
+    @warn_nwhy
+    def from_incidence_dataframe(
         cls,
         df,
         columns=None,
         rows=None,
+        edge_col: str = "edges",
+        node_col: str = "nodes",
         name=None,
         fillna=0,
         transpose=False,
         transforms=[],
         key=None,
-        node_label="nodes",
-        edge_label="edges",
-        static=False,
-        use_nwhy=False,
+        return_only_dataframe=False,
+        **kwargs,
     ):
         """
-        Create a hypergraph from a Pandas Dataframe object using index to label vertices
-        and Columns to label edges. The values of the dataframe are transformed into an
-        incidence matrix.
-        Note this is different than passing a dataframe directly
-        into the Hypergraph constructor. The latter automatically generates a static hypergraph
-        with edge and node labels given by the cell values.
+        Create a hypergraph from a Pandas Dataframe object, which has values equal
+        to the incidence matrix of a hypergraph. Its index will identify the nodes
+        and its columns will identify its edges.
 
         Parameters
         ----------
         df : Pandas.Dataframe
             a real valued dataframe with a single index
 
         columns : (optional) list, default = None
@@ -2511,96 +2294,81 @@
 
         rows : (optional) list, default = None
             restricts df to the rows indexed by the elements in this list.
 
         name : (optional) string, default = None
 
         fillna : float, default = 0
-            a real value to place in empty cell, all-zero columns will not generate
-            an edge.
+            a real value to place in empty cell, all-zero columns will not
+            generate an edge.
 
         transpose : (optional) bool, default = False
-            option to transpose the dataframe, in this case df.Index will label the edges
-            and df.columns will label the nodes, transpose is applied before transforms and
-            key
+            option to transpose the dataframe, in this case df.Index will
+            identify the edges and df.columns will identify the nodes, transpose is
+            applied before transforms and key
 
         transforms : (optional) list, default = []
             optional list of transformations to apply to each column,
             of the dataframe using pd.DataFrame.apply().
             Transformations are applied in the order they are
             given (ex. abs). To apply transforms to rows or for additional
-            functionality, consider transforming df using pandas.DataFrame methods
-            prior to generating the hypergraph.
+            functionality, consider transforming df using pandas.DataFrame
+            methods prior to generating the hypergraph.
 
         key : (optional) function, default = None
-            boolean function to be applied to dataframe. Must be defined on numpy
-            arrays.
+            boolean function to be applied to dataframe. will be applied to
+            entire dataframe.
+
+        return_only_dataframe : (optional) bool, default = False
+            to use the incidence_dataframe with cell_properties or properties, set this
+            to true and use it as the setsystem in the Hypergraph constructor.
 
         See also
         --------
-        from_numpy_array())
+        from_numpy_array
 
 
         Returns
         -------
         : Hypergraph
 
-        Notes
-        -----
-        The `from_dataframe` constructor does not generate empty edges.
-        All-zero columns in df are removed and the names corresponding to these
-        edges are discarded.
-        Restrictions and data processing will occur in this order:
-
-            1. column and row restrictions
-            2. fillna replace NaNs in dataframe
-            3. transpose the dataframe
-            4. transforms in the order listed
-            5. boolean key
-
-        This method offers the above options for wrangling a dataframe into an incidence
-        matrix for a hypergraph. For more flexibility we recommend you use the Pandas
-        library to format the values of your dataframe before submitting it to this
-        constructor.
-
         """
 
-        if type(df) != pd.core.frame.DataFrame:
+        if not isinstance(df, pd.DataFrame):
             raise HyperNetXError("Error: Input object must be a pandas dataframe.")
 
         if columns:
             df = df[columns]
         if rows:
             df = df.loc[rows]
 
         df = df.fillna(fillna)
         if transpose:
             df = df.transpose()
 
-        # node_names = np.array(df.index)
-        # edge_names = np.array(df.columns)
-
         for t in transforms:
             df = df.apply(t)
         if key:
             mat = key(df.values) * 1
         else:
             mat = df.values * 1
 
-        params = {
-            "node_names": np.array(df.index),
-            "edge_names": np.array(df.columns),
-            "name": name,
-            "node_label": node_label,
-            "edge_label": edge_label,
-            "static": static,
-            "use_nwhy": use_nwhy,
-        }
-        return cls.from_numpy_array(mat, **params)
-
-
-# end of Hypergraph class
-
-
-def _make_3_arrays(mat):
-    arr = coo_matrix(mat)
-    return arr.row, arr.col, arr.data
+        cols = df.columns
+        rows = df.index
+        CM = coo_matrix(mat)
+        c1 = CM.row
+        c1 = [rows[c1[idx]] for idx in range(len(c1))]
+        c2 = CM.col
+        c2 = [cols[c2[idx]] for idx in range(len(c2))]
+        c3 = CM.data
+
+        dfnew = pd.DataFrame({edge_col: c2, node_col: c1, "cell_weights": c3})
+        if return_only_dataframe == True:
+            return dfnew
+        else:
+            return Hypergraph(
+                dfnew,
+                edge_col=edge_col,
+                node_col=node_col,
+                weights="cell_weights",
+                name=None,
+            )
```

### Comparing `hypernetx-1.2.5/hypernetx/drawing/rubber_band.py` & `hypernetx-2.0.0/hypernetx/drawing/rubber_band.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 # Copyright © 2018 Battelle Memorial Institute
 # All rights reserved.
 
 from hypernetx import Hypergraph
-from .util import (
+from hypernetx.drawing.util import (
     get_frozenset_label,
     get_collapsed_size,
     get_set_layering,
     inflate_kwargs,
     transpose_inflated_kwargs,
 )
 
 import matplotlib.pyplot as plt
-from matplotlib.collections import PolyCollection, LineCollection, CircleCollection
+from matplotlib.collections import PolyCollection
 
 import networkx as nx
 
-from itertools import combinations
-from collections import defaultdict
 
 import numpy as np
 from scipy.spatial.distance import pdist
 from scipy.spatial import ConvexHull
-from scipy.spatial import Voronoi
 
 # increases the default figure size to 8in square.
 plt.rcParams["figure.figsize"] = (8, 8)
 
 N_CONTROL_POINTS = 24
 
 theta = np.linspace(0, 2 * np.pi, N_CONTROL_POINTS + 1)[:-1]
@@ -322,14 +319,15 @@
                     if hasattr(d, "__getitem__") and type(d) not in {str, tuple}
                     else d
                 )
                 for k, d in kwargs.items()
             }
         )
 
+
 def draw(
     H,
     pos=None,
     with_color=True,
     with_node_counts=False,
     with_edge_counts=False,
     layout=nx.spring_layout,
@@ -426,17 +424,15 @@
 
     ax = ax or plt.gca()
 
     if pos is None:
         pos = layout_node_link(H, layout=layout, **layout_kwargs)
 
     r0 = get_default_radius(H, pos)
-    a0 = np.pi * r0 ** 2
-
-
+    a0 = np.pi * r0**2
 
     def get_node_radius(v):
         if node_radius is None:
             return np.sqrt(a0 * get_collapsed_size(v) / np.pi)
         elif hasattr(node_radius, "get"):
             return node_radius.get(v, 1) * r0
         return node_radius * r0
```

### Comparing `hypernetx-1.2.5/hypernetx/drawing/two_column.py` & `hypernetx-2.0.0/hypernetx/drawing/two_column.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # All rights reserved.
 
 import matplotlib.pyplot as plt
 from matplotlib.collections import LineCollection
 
 import networkx as nx
 
-from .util import get_frozenset_label
+from hypernetx.drawing.util import get_frozenset_label
 
 
 def layout_two_column(H, spacing=2):
     """
     Two column (bipartite) layout algorithm.
 
     This algorithm first converts the hypergraph into a bipartite graph and
@@ -75,15 +75,15 @@
     Returns
     -------
     LineCollection
         the hyper edges
     """
     ax = ax or plt.gca()
 
-    pairs = [(v, e.uid) for e in H.edges() for v in e]
+    pairs = [(v, e) for e in H.edges() for v in H.edges[e]]
 
     kwargs = {
         k: v if type(v) != dict else [v.get(e) for _, e in pairs]
         for k, v in kwargs.items()
     }
 
     lines = LineCollection([(pos[u], pos[v]) for u, v in pairs], **kwargs)
@@ -116,26 +116,24 @@
     kwargs: dict
         keyword arguments passed to matplotlib.LineCollection
 
     """
 
     ax = ax or plt.gca()
 
-    edges = [e.uid for e in H.edges()]
-
     to_draw = []
     if with_node_labels:
-        to_draw.append((H.nodes(), "right"))
+        to_draw.append((list(H.nodes()), "right"))
 
     if with_edge_labels:
-        to_draw.append((H.edges(), "left"))
+        to_draw.append((list(H.edges()), "left"))
 
     for points, ha in to_draw:
         for p in points:
-            ax.annotate(labels.get(p.uid, p.uid), pos[p.uid], ha=ha, va="center")
+            ax.annotate(labels.get(p, p), pos[p], ha=ha, va="center")
 
 
 def draw(
     H,
     with_node_labels=True,
     with_edge_labels=True,
     with_node_counts=False,
@@ -179,24 +177,24 @@
 
     edge_kwargs = edge_kwargs or {}
 
     ax = ax or plt.gca()
 
     pos = layout_two_column(H)
 
-    V = [v.uid for v in H.nodes()]
-    E = [e.uid for e in H.edges()]
+    V = [v for v in H.nodes()]
+    E = [e for e in H.edges()]
 
     labels = {}
     labels.update(get_frozenset_label(V, count=with_node_counts))
     labels.update(get_frozenset_label(E, count=with_edge_counts))
 
     if with_color:
         edge_kwargs["color"] = {
-            e.uid: plt.cm.tab10(i % 10) for i, e in enumerate(H.edges())
+            e: plt.cm.tab10(i % 10) for i, e in enumerate(H.edges())
         }
 
     draw_hyper_edges(H, pos, ax=ax, **edge_kwargs)
     draw_hyper_labels(
         H,
         pos,
         labels,
```

### Comparing `hypernetx-1.2.5/hypernetx/drawing/util.py` & `hypernetx-2.0.0/hypernetx/drawing/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,21 +40,22 @@
 
 def transpose_inflated_kwargs(inflated):
     return [dict(zip(inflated, v)) for v in zip(*inflated.values())]
 
 
 def get_collapsed_size(v):
     try:
-        if type(v) == str and ':' in v:
-            return int(v.split(':')[-1])
+        if type(v) == str and ":" in v:
+            return int(v.split(":")[-1])
     except:
         pass
-    
+
     return 1
 
+
 def get_frozenset_label(S, count=False, override={}):
     """
     Helper function for rendering the labels of possibly collapsed nodes and edges
 
     Parameters
     ----------
     S: iterable
```

### Comparing `hypernetx-1.2.5/hypernetx/reports/descriptive_stats.py` & `hypernetx-2.0.0/hypernetx/reports/descriptive_stats.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,32 +6,16 @@
     * Toplex size distribution
     * Diameter
 
 Also computes general hypergraph information: number of nodes, edges, cells, aspect ratio, incidence matrix density
 """
 from collections import Counter
 import numpy as np
-import networkx as nx
-from hypernetx import *
 from hypernetx.utils.decorators import not_implemented_for
 
-__all__ = [
-    "centrality_stats",
-    "edge_size_dist",
-    "degree_dist",
-    "comp_dist",
-    "s_comp_dist",
-    "toplex_dist",
-    "s_node_diameter_dist",
-    "s_edge_diameter_dist",
-    "info",
-    "info_dict",
-    "dist_stats",
-]
-
 
 def centrality_stats(X):
     """
     Computes basic centrality statistics for X
 
     Parameters
     ----------
@@ -39,15 +23,21 @@
         an iterable of numbers
 
     Returns
     -------
     [min, max, mean, median, standard deviation] : list
         List of centrality statistics for X
     """
-    return [min(X), max(X), np.mean(X), np.median(X), np.std(X)]
+    return [
+        min(X),
+        max(X),
+        np.mean(X).tolist(),
+        np.median(X).tolist(),
+        np.std(X).tolist(),
+    ]
 
 
 def edge_size_dist(H, aggregated=False):
     """
     Computes edge sizes of a hypergraph.
 
     Parameters
@@ -83,18 +73,15 @@
         list of degrees in H.
 
     Returns
     -------
      degree_dist : list or dict
         List of degrees or dictionary of degree distribution
     """
-    if H.nwhy:
-        distr = H.g.node_size_dist()
-    else:
-        distr = [H.degree(n) for n in H.nodes]
+    distr = [H.degree(n) for n in H.nodes]
     if aggregated:
         return Counter(distr)
     else:
         return distr
 
 
 def comp_dist(H, aggregated=False):
@@ -350,18 +337,17 @@
     H : Hypergraph
 
     Returns
     -------
      dist_stats : dict
         Dictionary which keeps track of each of the above items (e.g., basic['nrows'] = the number of nodes in H)
     """
-    if H.isstatic:
-        stats = H.state_dict.get("dist_stats", None)
-        if stats is not None:
-            return H.state_dict["dist_stats"]
+    stats = H._state_dict.get("dist_stats", None)
+    if stats is not None:
+        return H._state_dict["dist_stats"]
 
     cstats = ["min", "max", "mean", "median", "std"]
     basic = dict()
 
     # Number of rows (nodes), columns (edges), and aspect ratio
     basic["nrows"] = len(H.nodes)
     basic["ncols"] = len(H.edges)
@@ -404,10 +390,9 @@
 
     # Number of components
     basic["num comps"] = len(basic["comp nodes list"])
 
     # # Diameters
     # basic['s edge diam list'] = s_edge_diameter_dist(H)
     # basic['s node diam list'] = s_node_diameter_dist(H)
-    if H.isstatic:
-        H.set_state(dist_stats=basic)
+    H.set_state(dist_stats=basic)
     return basic
```

### Comparing `hypernetx-1.2.5/hypernetx/utils/decorators.py` & `hypernetx-2.0.0/hypernetx/utils/decorators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-import sys
-from warnings import warn
-import hypernetx as hnx
+import warnings
+from functools import wraps
+
 from decorator import decorator
-from hypernetx.exception import HyperNetXError, HyperNetXNotImplementedError
 
-try:
-    import nwhy
-except:
-    pass
+import hypernetx as hnx
+from hypernetx.exception import NWHY_WARNING
 
 __all__ = [
     "not_implemented_for",
+    "warn_nwhy",
 ]
 
 
 def not_implemented_for(*object_types):
     """Decorator to hypergraph methods to mark algorithms as not implemented
     Ruthlessly copied from NetworkX.
 
@@ -61,7 +59,33 @@
         if match:
             msg = f'{not_implemented_for_func.__name__} is not implemented for {" ".join(object_types)} {this_object.__class__.__name__}'
             raise hnx.HyperNetXNotImplementedError(msg)
         else:
             return not_implemented_for_func(*args, **kwargs)
 
     return _not_implemented_for
+
+
+def warn_nwhy(func):
+    """Decorator for methods that allow the deprecated `use_nwhy` kwarg
+
+    As of HyperNetX v2.0.0, NWHy C++ backend is no longer supported.
+    Public references to the deprecated NWHy add-on will be removed from the Hypergraph
+    API in a future release.
+
+    Warns
+    -----
+    FutureWarning
+        If kwargs contain ``use_nwhy=True``
+    """
+
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        if kwargs.get("use_nwhy"):
+            kwargs.update(use_nwhy=False)
+            warnings.simplefilter("always", FutureWarning)
+            warnings.warn(NWHY_WARNING, FutureWarning, stacklevel=2)
+            warnings.simplefilter("default", FutureWarning)
+
+        return func(*args, **kwargs)
+
+    return wrapper
```

### Comparing `hypernetx-1.2.5/hypernetx/utils/extras.py` & `hypernetx-2.0.0/hypernetx/utils/extras.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 
     nodelabel : str, optional, default : 'Nodes'
 
 
     Returns
     -------
     OrderedDict
-        used for labels in constructing a StaticEntitySet
+        used for labels in constructing a EntitySet
     """
     enames = np.array([f"{edgeprefix}{idx}" for idx in range(num_edges)])
     nnames = np.array([f"{nodeprefix}{jdx}" for jdx in range(num_nodes)])
     return OrderedDict([(edgelabel, enames), (nodelabel, nnames)])
 
 
 def reverse_dictionary(d):
```

### Comparing `hypernetx-1.2.5/hypernetx/utils/toys/harrypotter.py` & `hypernetx-2.0.0/hypernetx/utils/toys/harrypotter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import os
 from hypernetx.utils import HNXCount, remove_row_duplicates
 from collections import OrderedDict, defaultdict
-import scipy
-from scipy.sparse import coo_matrix, issparse
+
 import pandas as pd
 import numpy as np
-import itertools as it
 
-__all__ = ["HarryPotter"]
 
 current_dir = os.path.dirname(os.path.abspath(__file__))
 
 
 class HarryPotter(object):
     def __init__(self, cols=None):
```

### Comparing `hypernetx-1.2.5/hypernetx/utils/toys/lesmis.py` & `hypernetx-2.0.0/hypernetx/utils/toys/lesmis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # Copyright © 2018 Battelle Memorial Institute
 # All rights reserved.
 
-import numpy as np
 import pandas as pd
 from itertools import islice, chain, repeat
 
-import networkx as nx
-
 import matplotlib.pyplot as plt
 
 import hypernetx as hnx
 
-__all__ = ["LesMis", "lesmis_hypergraph_from_df", "book_tour"]
-
 
 class LesMis(object):
     def __init__(self):
         self.volumes = pd.DataFrame.from_dict(volume_names, orient="index")
 
-        accents = {"\`e": "è", "\\`e": "è", "'e": "é", "\\c{c}": "ç", "\^o": "ô"}
+        accents = {
+            r"\`e": "è",
+            r"\\'e": "è",
+            r"\\`e": "è",
+            r"'e": "é",
+            r"\\c{c}": "ç",
+            r"\^o": "ô",
+        }
         for k, v in accents.items():
             self.names = names.replace(k, v)
 
         self.df_names = pd.DataFrame(
             [parse_name_row(row) for row in self.names.split("\n")],
             columns=["Symbol", "FullName", "Description"],
         )
@@ -110,15 +112,15 @@
             for i, si in enumerate(characters.split(";")):
                 for c in si.split(","):
                     yield int(volume), int(book), int(chapter), i, t, c
                 t += 1
 
 
 # LesMis Data:
-names = """AZ Anzelma, daughter of TH and TM
+names = r"""AZ Anzelma, daughter of TH and TM
 BA Bahorel, `Friends of the ABC' cutup
 BB Babet, tooth-pulling bandit of Paris
 BJ Brujon, notorious criminal
 BL Blacheville, Parisian student from Montauban
 BM Monsieur Bamatabois, idler of M-- sur M--
 BO Bossuet (Lesgle), `Friends of the ABC' klutz
 BR Brevet, convict in the galleys with JV
```

### Comparing `hypernetx-1.2.5/hypernetx/utils/toys/transmission_problem.py` & `hypernetx-2.0.0/hypernetx/utils/toys/transmission_problem.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import pandas as pd
 import os
 
 
-__all__ = ["TransmissionProblem"]
-
 current_dir = os.path.dirname(os.path.abspath(__file__))
 
 
 class TransmissionProblem(object):
     def __init__(self):
 
         try:
```

### Comparing `hypernetx-1.2.5/hypernetx.egg-info/SOURCES.txt` & `hypernetx-2.0.0/hypernetx.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 LICENSE.rst
+LONG_DESCRIPTION.rst
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 hypernetx/__init__.py
 hypernetx/exception.py
 hypernetx/read_write.py
 hypernetx.egg-info/PKG-INFO
 hypernetx.egg-info/SOURCES.txt
 hypernetx.egg-info/dependency_links.txt
 hypernetx.egg-info/requires.txt
 hypernetx.egg-info/top_level.txt
 hypernetx/algorithms/__init__.py
+hypernetx/algorithms/barycentric_subdivisions.py
+hypernetx/algorithms/contagion.py
 hypernetx/algorithms/generative_models.py
 hypernetx/algorithms/homology_mod2.py
 hypernetx/algorithms/hypergraph_modularity.py
 hypernetx/algorithms/laplacians_clustering.py
 hypernetx/algorithms/s_centrality_measures.py
-hypernetx/algorithms/contagion/__init__.py
-hypernetx/algorithms/contagion/animation.py
-hypernetx/algorithms/contagion/epidemics.py
 hypernetx/classes/__init__.py
 hypernetx/classes/entity.py
+hypernetx/classes/entityset.py
+hypernetx/classes/helpers.py
 hypernetx/classes/hypergraph.py
-hypernetx/classes/staticentity.py
 hypernetx/drawing/__init__.py
 hypernetx/drawing/rubber_band.py
 hypernetx/drawing/two_column.py
 hypernetx/drawing/util.py
 hypernetx/reports/__init__.py
 hypernetx/reports/descriptive_stats.py
 hypernetx/utils/__init__.py
 hypernetx/utils/decorators.py
 hypernetx/utils/extras.py
+hypernetx/utils/log.py
 hypernetx/utils/toys/__init__.py
 hypernetx/utils/toys/gene_data.py
 hypernetx/utils/toys/harrypotter.py
 hypernetx/utils/toys/lesmis.py
 hypernetx/utils/toys/transmission_problem.py
```


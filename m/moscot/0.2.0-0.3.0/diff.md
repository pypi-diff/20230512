# Comparing `tmp/moscot-0.2.0.tar.gz` & `tmp/moscot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moscot-0.2.0.tar", last modified: Wed Mar 22 11:10:14 2023, max compression
+gzip compressed data, was "moscot-0.3.0.tar", last modified: Fri May 12 09:56:06 2023, max compression
```

## Comparing `moscot-0.2.0.tar` & `moscot-0.3.0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:10:14.965309 moscot-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-03-22 11:08:52.000000 moscot-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-22 11:08:52.000000 moscot-0.2.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-22 11:08:52.000000 moscot-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-22 11:08:52.000000 moscot-0.2.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-03-22 11:08:52.000000 moscot-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-22 11:08:52.000000 moscot-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-03-22 11:10:14.961309 moscot-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-03-22 11:08:52.000000 moscot-0.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-22 11:08:52.000000 moscot-0.2.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-03-22 11:08:52.000000 moscot-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 11:10:14.965309 moscot-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:10:14.929309 moscot-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:10:14.933309 moscot-0.2.0/src/moscot/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:10:14.937309 moscot-0.2.0/src/moscot/_docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/_docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16311 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/_docs/_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/_docs/_docs_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/_docs/_docs_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/_docs/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:10:14.937309 moscot-0.2.0/src/moscot/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:10:14.941309 moscot-0.2.0/src/moscot/backends/ott/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/backends/ott/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/backends/ott/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/backends/ott/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    12331 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/backends/ott/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/backends/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:10:14.941309 moscot-0.2.0/src/moscot/base/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/base/cost.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/base/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:10:14.945309 moscot-0.2.0/src/moscot/base/problems/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/base/problems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24017 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/base/problems/_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    23604 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/base/problems/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10775 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/base/problems/birth_death.py
--rw-r--r--   0 runner    (1001) docker     (123)    22344 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/base/problems/compound_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/base/problems/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    26078 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/base/problems/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/base/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:10:14.945309 moscot-0.2.0/src/moscot/costs/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/costs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/costs/_costs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/costs/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:10:14.949309 moscot-0.2.0/src/moscot/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/plotting/_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    23419 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/plotting/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:10:14.949309 moscot-0.2.0/src/moscot/problems/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/problems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/problems/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:10:14.949309 moscot-0.2.0/src/moscot/problems/generic/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/problems/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/problems/generic/_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/problems/generic/_mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:10:14.953309 moscot-0.2.0/src/moscot/problems/space/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/problems/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/problems/space/_alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/problems/space/_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    22205 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/problems/space/_mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:10:14.957309 moscot-0.2.0/src/moscot/problems/spatiotemporal/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/problems/spatiotemporal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/problems/spatiotemporal/_spatio_temporal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:10:14.957309 moscot-0.2.0/src/moscot/problems/time/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/problems/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/problems/time/_lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)    32147 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/problems/time/_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:10:14.961309 moscot-0.2.0/src/moscot/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:10:14.961309 moscot-0.2.0/src/moscot/utils/_data/
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/utils/_data/allTFs_dmel.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/utils/_data/allTFs_hg38.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/utils/_data/allTFs_mm.txt
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/utils/_data/human_apoptosis.txt
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/utils/_data/human_proliferation.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/utils/_data/mouse_apoptosis.txt
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/utils/_data/mouse_proliferation.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/utils/subset_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-03-22 11:08:52.000000 moscot-0.2.0/src/moscot/utils/tagged_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 11:10:14.937309 moscot-0.2.0/src/moscot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-03-22 11:10:14.000000 moscot-0.2.0/src/moscot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-03-22 11:10:14.000000 moscot-0.2.0/src/moscot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 11:10:14.000000 moscot-0.2.0/src/moscot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-22 11:10:14.000000 moscot-0.2.0/src/moscot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-22 11:10:14.000000 moscot-0.2.0/src/moscot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.420514 moscot-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-12 09:54:41.000000 moscot-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-12 09:54:41.000000 moscot-0.3.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-12 09:54:41.000000 moscot-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-12 09:54:41.000000 moscot-0.3.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-12 09:54:41.000000 moscot-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-12 09:54:41.000000 moscot-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-12 09:56:06.420514 moscot-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-12 09:54:41.000000 moscot-0.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-12 09:54:41.000000 moscot-0.3.0/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8649 2023-05-12 09:54:41.000000 moscot-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 09:56:06.420514 moscot-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.408513 moscot-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.412513 moscot-0.3.0/src/moscot/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.412513 moscot-0.3.0/src/moscot/_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/_docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15359 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/_docs/_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/_docs/_docs_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/_docs/_docs_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/_docs/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.412513 moscot-0.3.0/src/moscot/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.412513 moscot-0.3.0/src/moscot/backends/ott/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/backends/ott/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/backends/ott/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/backends/ott/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/backends/ott/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/backends/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.412513 moscot-0.3.0/src/moscot/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/base/cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/base/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.416514 moscot-0.3.0/src/moscot/base/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/base/problems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22166 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/base/problems/_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25439 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/base/problems/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/base/problems/birth_death.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22334 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/base/problems/compound_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/base/problems/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27779 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/base/problems/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/base/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.416514 moscot-0.3.0/src/moscot/costs/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/costs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/costs/_costs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/costs/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15430 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.416514 moscot-0.3.0/src/moscot/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/plotting/_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23707 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/plotting/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.416514 moscot-0.3.0/src/moscot/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.416514 moscot-0.3.0/src/moscot/problems/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/generic/_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/generic/_mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.416514 moscot-0.3.0/src/moscot/problems/space/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/space/_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/space/_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22205 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/space/_mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.416514 moscot-0.3.0/src/moscot/problems/spatiotemporal/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/spatiotemporal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/spatiotemporal/_spatio_temporal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.416514 moscot-0.3.0/src/moscot/problems/time/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/time/_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31747 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/problems/time/_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.420514 moscot-0.3.0/src/moscot/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.420514 moscot-0.3.0/src/moscot/utils/_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/utils/_data/allTFs_dmel.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/utils/_data/allTFs_hg38.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/utils/_data/allTFs_mm.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/utils/_data/human_apoptosis.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/utils/_data/human_proliferation.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/utils/_data/mouse_apoptosis.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/utils/_data/mouse_proliferation.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/utils/subset_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-05-12 09:54:41.000000 moscot-0.3.0/src/moscot/utils/tagged_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:56:06.412513 moscot-0.3.0/src/moscot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-12 09:56:06.000000 moscot-0.3.0/src/moscot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-12 09:56:06.000000 moscot-0.3.0/src/moscot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 09:56:06.000000 moscot-0.3.0/src/moscot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-12 09:56:06.000000 moscot-0.3.0/src/moscot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 09:56:06.000000 moscot-0.3.0/src/moscot.egg-info/top_level.txt
```

### Comparing `moscot-0.2.0/.gitignore` & `moscot-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `moscot-0.2.0/.pre-commit-config.yaml` & `moscot-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `moscot-0.2.0/LICENSE` & `moscot-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moscot-0.2.0/PKG-INFO` & `moscot-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moscot
-Version: 0.2.0
+Version: 0.3.0
 Summary: Multi-omic single-cell optimal transport tools
 Author: Dominik Klein, Giovanni Palla, Michal Klein, Zoe Piran, Marius Lange
 Maintainer-email: Dominik Klein <dominik.klein@helmholtz-muenchen.de>, Giovanni Palla <giovanni.palla@helmholtz-muenchen.de>, Michal Klein <michal.klein@helmholtz-muenchen.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Theis Lab
         All rights reserved.
@@ -104,8 +104,8 @@
 ---------
 
 Please have a look at our `documentation <https://moscot.readthedocs.io>`_
 
 Reference
 ---------
 
-Our manuscript will be available soon.
+Our preprint "Mapping cells through time and space with moscot" can be found `here <https://www.biorxiv.org/content/10.1101/2023.05.11.540374v1>`_.
```

### Comparing `moscot-0.2.0/README.rst` & `moscot-0.3.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -40,8 +40,8 @@
 ---------
 
 Please have a look at our `documentation <https://moscot.readthedocs.io>`_
 
 Reference
 ---------
 
-Our manuscript will be available soon.
+Our preprint "Mapping cells through time and space with moscot" can be found `here <https://www.biorxiv.org/content/10.1101/2023.05.11.540374v1>`_.
```

### Comparing `moscot-0.2.0/pyproject.toml` & `moscot-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     {name = "Michal Klein", email = "michal.klein@helmholtz-muenchen.de"}
 ]
 
 
 dependencies = [
     "numpy>=1.20.0",
     "scipy>=1.7.0",
-    "pandas>=1.4.0",
+    "pandas<2.0",
     "networkx>=2.6.3",
     # https://github.com/scverse/scanpy/issues/2411
     "matplotlib>=3.5.0",
     "anndata>=0.8.0",
     "scanpy>=1.9.3",
     "wrapt>=1.13.2",
     "docrep>=0.3.2",
@@ -176,15 +176,14 @@
 
 [tool.pytest.ini_options]
 markers = ["fast: marks tests as fask"]
 xfail_strict = true
 filterwarnings = [
     "ignore:X.dtype being converted:FutureWarning",
     "ignore:No data for colormapping:UserWarning",
-    "ignore:jax\\.experimental\\.pjit\\.PartitionSpec:DeprecationWarning",
 ]
 
 [tool.coverage.run]
 branch = true
 parallel = true
 source = ["src/"]
 omit = [
@@ -320,8 +319,18 @@
 allowlist_externals = rm
 commands =
     rm -rf {tox_root}{/}dist
     python -m build --sdist --wheel --outdir {tox_root}{/}dist{/} {posargs:}
     python -m twine check {tox_root}{/}dist{/}*
 commands_post =
     python -c 'import pathlib; print(f"Package is under:", pathlib.Path("{tox_root}") / "dist")'
+
+[testenv:format-references]
+description = Format references.bib.
+deps =
+skip_install = true
+allowlist_externals = biber
+commands = biber --tool --output_file={tox_root}{/}docs{/}references.bib --nolog \
+    --output_align --output_indent=2 --output_fieldcase=lower \
+    --output_legacy_dates --output-field-replace=journaltitle:journal,thesis:phdthesis,institution:school \
+    {tox_root}{/}docs{/}references.bib
 """
```

### Comparing `moscot-0.2.0/src/moscot/_docs/_docs.py` & `moscot-0.3.0/src/moscot/_docs/_docs.py`

 * *Files 8% similar despite different names*

```diff
@@ -171,23 +171,23 @@
 joint_attr
 
     - If `None`, PCA on :attr:`anndata.AnnData.X` is computed.
     - If `str`, it must refer to a key in :attr:`anndata.AnnData.obsm`.
     - If `dict`, the dictionary stores `attr` (attribute of :class:`anndata.AnnData`) and `key`
       (key of :class:`anndata.AnnData` ``['{attr}']``).
 """
-_GW_x = """\
-GW_x
+_x_attr = """\
+x_attr
 
     - If `str`, it must refer to a key in :attr:`anndata.AnnData.obsm`.
     - If `dict`, the dictionary stores `attr` (attribute of :class:`anndata.AnnData`) and `key`
       (key of :class:`anndata.AnnData` ``['{attr}']``).
 """
-_GW_y = """\
-GW_y
+_y_attr = """\
+y_attr
 
     - If `str`, it must refer to a key in :attr:`anndata.AnnData.obsm`.
     - If `dict`, the dictionary stores `attr` (attribute of :class:`anndata.AnnData`) and `key`
       (key of :class:`anndata.AnnData` ``['{attr}']``).
 """
 _split_mass = """\
 split_mass
@@ -272,48 +272,27 @@
 inner_iterations
     The Sinkhorn error is not recomputed at each iteration but every ``inner_iterations`` instead.
 min_iterations
     The minimum number of Sinkhorn iterations carried out before the error is computed and monitored.
 max_iterations
     The maximum number of Sinkhorn iterations.
 """
-_sinkhorn_lr_kwargs = """\
-gamma
-    Only in low-rank setting: the (inverse of the) gradient step size used by the mirror descent algorithm
-    (:cite:`scetbon:22b`).
-gamma_rescale
-    Only in low-rank setting: whether to rescale `gamma` every iteration as described in :cite:`scetbon:22b`.
-"""
 _cost_matrix_rank = """\
 cost_matrix_rank
     Rank of the matrix the cost matrix is approximated by. Only applies if a custom cost matrix is passed.
     If `None`, `cost_matrix_rank` is set to `rank`.
 """
 _gw_kwargs = """\
 min_iterations
     Minimal number of outer Gromov-Wasserstein iterations.
 max_iterations
     Maximal number of outer Gromov-Wasserstein iterations.
 threshold
     Threshold used as convergence criterion for the outer Gromov-Wasserstein loop.
 """
-_gw_lr_kwargs = """\
-ranks
-    Ranks of the cost matrices, see
-    :meth:`~ott.geometry.geometry.Geometry.to_LRCGeometry`. Used when
-    geometries are *not* :class:`~ott.geometry.pointcloud.PointCloud` with
-    `'sqeucl'` cost function. If `-1`, the geometries will not be converted
-    to low-rank. If :class:`tuple`, it specifies the ranks of ``geom_xx``,
-    ``geom_yy`` and ``geom_xy``, respectively. If :class:`int`, rank is shared
-    across all geometries.
-tolerances
-    Tolerances used when converting geometries to low-rank. Used
-    when geometries are not :class:`~ott.geometry.pointcloud.PointCloud` with
-    `'sqeucl'` cost. If :class:`float`, it is shared across all geometries.
-"""
 _scale_cost = """\
 scale_cost
     How to rescale the cost matrix. Implemented scalings are
     'median', 'mean', 'max_cost', 'max_norm' and 'max_bound'.
     Alternatively, a float factor can be given to rescale the cost such
     that ``cost_matrix /= scale_cost``.
 """
@@ -325,14 +304,18 @@
 cost
     Cost between two points in dimension d. Only used if no precomputed cost matrix is passed.
     If `cost` is of type :obj:`str`, the cost will be used for all point clouds. If `cost` is of type :obj:`dict`,
     it is expected to have keys `x`, `y`, and/or `xy`, with values corresponding to the cost functions
     in the quadratic term of the source distribution, the quadratic term of the target distribution, and/or the
     linear term, respectively.
     """
+_cost_kwargs = """\
+cost_kwargs
+    Keyword arguments for the cost.
+"""
 _pointcloud_kwargs = """\
 batch_size
     Number of data points the matrix-vector products are applied to at the same time. The larger, the more memory
     is required. Only used if no precomputed cost matrix is used.
 """
 _device_solve = """\
 device
@@ -419,34 +402,33 @@
     b_temporal=_b_temporal,
     time_key=_time_key,
     spatial_key=_spatial_key,
     batch_key=_batch_key,
     policy=_policy,
     key=_key,
     joint_attr=_joint_attr,
-    GW_x=_GW_x,
-    GW_y=_GW_y,
+    x_attr=_x_attr,
+    y_attr=_y_attr,
     split_mass=_split_mass,
     inplace=_inplace,
     alignment_mixin_returns=_alignment_mixin_returns,
     rank=_rank,
     stage=_stage,
     solve_kwargs=_solve_kwargs,
     initializer_lin=_initializer_lin,
     initializer_quad=_initializer_quad,
     initializer_kwargs=_initializer_kwargs,
     jit=_jit,
     sinkhorn_kwargs=_sinkhorn_kwargs,
-    sinkhorn_lr_kwargs=_sinkhorn_lr_kwargs,
     cost_matrix_rank=_cost_matrix_rank,  # TODO(@MUCDK): test for this. cannot be tested with current `test_pass_for_arguments`.  # noqa: E501
     gw_kwargs=_gw_kwargs,
-    gw_lr_kwargs=_gw_lr_kwargs,
     scale_cost=_scale_cost,
     cost_lin=_cost_lin,
     cost=_cost,
+    cost_kwargs=_cost_kwargs,
     pointcloud_kwargs=_pointcloud_kwargs,
     device_solve=_device_solve,
     linear_solver_kwargs=_linear_solver_kwargs,
     kwargs_linear=_kwargs_linear,
     kwargs_quad=_kwargs_quad,
     kwargs_quad_fused=_kwargs_quad_fused,
     kwargs_prepare=_kwargs_prepare,
```

### Comparing `moscot-0.2.0/src/moscot/_docs/_docs_mixins.py` & `moscot-0.3.0/src/moscot/_docs/_docs_mixins.py`

 * *Files identical despite different names*

### Comparing `moscot-0.2.0/src/moscot/_docs/_docs_plot.py` & `moscot-0.3.0/src/moscot/_docs/_docs_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,14 @@
     Size of the figure in inches.
 dpi
     Dots per inch.
 save
     Path where to save the plot. If `None`, the plot is not saved.
 {_ax}"""
 
-
 d_plotting = DocstringProcessor(
     desc_cell_transition=_desc_cell_transition,
     transition_labels_cell_transition=_transition_labels_cell_transition,
     cbar_kwargs_cell_transition=_cbar_kwargs_cell_transition,
     return_cell_transition=_return_cell_transition,
     notes_cell_transition=_notes_cell_transition,
     desc_sankey=_desc_sankey,
```

### Comparing `moscot-0.2.0/src/moscot/_docs/_utils.py` & `moscot-0.3.0/src/moscot/_docs/_utils.py`

 * *Files identical despite different names*

### Comparing `moscot-0.2.0/src/moscot/_logging.py` & `moscot-0.3.0/src/moscot/_logging.py`

 * *Files identical despite different names*

### Comparing `moscot-0.2.0/src/moscot/_registry.py` & `moscot-0.3.0/src/moscot/_registry.py`

 * *Files identical despite different names*

### Comparing `moscot-0.2.0/src/moscot/_types.py` & `moscot-0.3.0/src/moscot/_types.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,32 +12,47 @@
 except (ImportError, TypeError):
     ArrayLike = np.ndarray  # type: ignore[misc]
     DTypeLike = np.dtype  # type: ignore[misc]
 
 ProblemKind_t = Literal["linear", "quadratic", "unknown"]
 Numeric_t = Union[int, float]  # type of `time_key` arguments
 Filter_t = Optional[Union[str, Mapping[str, Sequence[Any]]]]  # type how to filter adata
-Str_Dict_t = Union[str, Mapping[str, Sequence[Any]]]  # type for `cell_transition`
+Str_Dict_t = Optional[Union[str, Mapping[str, Sequence[Any]]]]  # type for `cell_transition`
 SinkFullRankInit = Literal["default", "gaussian", "sorting"]
 LRInitializer_t = Literal["random", "rank2", "k-means", "generalized-k-means"]
 
 SinkhornInitializer_t = Optional[Union[SinkFullRankInit, LRInitializer_t]]
 QuadInitializer_t = Optional[LRInitializer_t]
 
 Initializer_t = Union[SinkhornInitializer_t, LRInitializer_t]
 ProblemStage_t = Literal["initialized", "prepared", "solved"]
-Device_t = Literal["cpu", "gpu", "tpu"]
+Device_t = Union[Literal["cpu", "gpu", "tpu"], str]
 
 # TODO(michalk8): autogenerate from the enums
 ScaleCost_t = Optional[Union[float, Literal["mean", "max_cost", "max_bound", "max_norm", "median"]]]
-OttCostFn_t = Literal["euclidean", "sq_euclidean", "cosine", "bures", "unbalanced_bures"]
+OttCostFn_t = Literal[
+    "euclidean",
+    "sq_euclidean",
+    "cosine",
+    "PNormP",
+    "SqPNorm",
+    "Euclidean",
+    "SqEuclidean",
+    "Cosine",
+    "ElasticL1",
+    "ElasticSTVS",
+    "ElasticSqKOverlap",
+]
+OttCostFnMap_t = Union[OttCostFn_t, Mapping[str, OttCostFn_t]]
 GenericCostFn_t = Literal["barcode_distance", "leaf_distance", "custom"]
 CostFn_t = Union[str, GenericCostFn_t, OttCostFn_t]
+CostFnMap_t = Union[Union[OttCostFn_t, GenericCostFn_t], Mapping[str, Union[OttCostFn_t, GenericCostFn_t]]]
 PathLike = Union[os.PathLike, str]
 Policy_t = Literal[
     "sequential",
     "star",
     "external_star",
     "triu",
     "tril",
     "explicit",
 ]
+CostKwargs_t = Union[Mapping[str, Any], Mapping[Literal["x", "y", "xy"], Mapping[str, Any]]]
```

### Comparing `moscot-0.2.0/src/moscot/backends/ott/__init__.py` & `moscot-0.3.0/src/moscot/backends/ott/__init__.py`

 * *Files identical despite different names*

### Comparing `moscot-0.2.0/src/moscot/backends/ott/output.py` & `moscot-0.3.0/src/moscot/backends/ott/output.py`

 * *Files identical despite different names*

### Comparing `moscot-0.2.0/src/moscot/backends/utils.py` & `moscot-0.3.0/src/moscot/backends/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-from typing import TYPE_CHECKING, Any, Literal, Tuple, Union
+from typing import TYPE_CHECKING, Any, Literal, Tuple, Type, Union
 
 from moscot import _registry
 from moscot._types import ProblemKind_t
 
 if TYPE_CHECKING:
     from moscot.backends import ott
 
 __all__ = ["get_solver", "register_solver", "get_available_backends"]
 
 
 _REGISTRY = _registry.Registry()
 
 
-def get_solver(problem_kind: ProblemKind_t, *, backend: str = "ott", **kwargs: Any) -> Any:
+def get_solver(problem_kind: ProblemKind_t, *, backend: str = "ott", return_class: bool = False, **kwargs: Any) -> Any:
     """TODO."""
     if backend not in _REGISTRY:
         raise ValueError(f"Backend `{backend!r}` is not available.")
-    return _REGISTRY[backend](problem_kind, **kwargs)
+    solver_class = _REGISTRY[backend](problem_kind)
+    return solver_class if return_class else solver_class(**kwargs)
 
 
 def register_solver(backend: str) -> Any:
     """TODO."""
     return _REGISTRY.register(backend)
 
 
 @register_solver("ott")
-def _(problem_kind: Literal["linear", "quadratic"], **kwargs: Any) -> Union["ott.SinkhornSolver", "ott.GWSolver"]:
+def _(problem_kind: Literal["linear", "quadratic"]) -> Union[Type["ott.SinkhornSolver"], Type["ott.GWSolver"]]:
     from moscot.backends import ott
 
     if problem_kind == "linear":
-        return ott.SinkhornSolver(**kwargs)
+        return ott.SinkhornSolver
     if problem_kind == "quadratic":
-        return ott.GWSolver(**kwargs)
+        return ott.GWSolver
     raise NotImplementedError(f"Unable to create solver for `{problem_kind!r}` problem.")
 
 
 def get_available_backends() -> Tuple[str, ...]:
     """TODO."""
     return tuple(backend for backend in _REGISTRY)
```

### Comparing `moscot-0.2.0/src/moscot/base/cost.py` & `moscot-0.3.0/src/moscot/base/cost.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             Keyword arguments for computation.
 
         Returns
         -------
         The computed cost matrix.
         """
         cost = self._compute(*args, **kwargs)
-        if not np.all(np.isnan(cost)):
+        if np.any(np.isnan(cost)):
             maxx = np.nanmax(cost)
             logger.warning(f"Cost matrix contains `NaN` values, setting them to the maximum value `{maxx}`.")
             cost = np.nan_to_num(cost, nan=maxx)  # type: ignore[call-overload]
         if np.any(cost < 0):
             raise ValueError("Cost matrix contains negative values.")
         return cost
```

### Comparing `moscot-0.2.0/src/moscot/base/output.py` & `moscot-0.3.0/src/moscot/base/output.py`

 * *Files identical despite different names*

### Comparing `moscot-0.2.0/src/moscot/base/problems/__init__.py` & `moscot-0.3.0/src/moscot/base/problems/__init__.py`

 * *Files identical despite different names*

### Comparing `moscot-0.2.0/src/moscot/base/problems/_mixins.py` & `moscot-0.3.0/src/moscot/base/problems/_mixins.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from moscot._types import ArrayLike, Numeric_t, Str_Dict_t
 from moscot.base.output import BaseSolverOutput
 from moscot.base.problems._utils import (
     _check_argument_compatibility_cell_transition,
     _correlation_test,
     _get_df_cell_transition,
     _order_transition_matrix,
-    _validate_annotations_helper,
+    _validate_annotations,
     _validate_args_cell_transition,
 )
 from moscot.base.problems.compound_problem import ApplyOutput_t, B, K
 from moscot.plotting._utils import set_plotting_vars
 from moscot.utils.data import transcription_factors
 from moscot.utils.subset_policy import SubsetPolicy
 
@@ -95,57 +95,51 @@
         other_key: Optional[str] = None,
         other_adata: Optional[str] = None,
         batch_size: Optional[int] = None,
         normalize: bool = True,
     ) -> pd.DataFrame:
         ...
 
-    def _validate_annotations(
-        self: "AnalysisMixinProtocol[K, B]",
-        df_source: pd.DataFrame,
-        df_target: pd.DataFrame,
-        source_annotation_key: Optional[str] = None,
-        target_annotation_key: Optional[str] = None,
-        source_annotations: Optional[List[Any]] = None,
-        target_annotations: Optional[List[Any]] = None,
-        aggregation_mode: Literal["annotation", "cell"] = "annotation",
-        forward: bool = False,
-    ) -> Tuple[List[Any], List[Any]]:
-        ...
-
 
 class AnalysisMixin(Generic[K, B]):
     """Base Analysis Mixin."""
 
     def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
 
     def _cell_transition(
         self: AnalysisMixinProtocol[K, B],
         source: K,
         target: K,
         source_groups: Str_Dict_t,
         target_groups: Str_Dict_t,
+        aggregation_mode: Literal["annotation", "cell"] = "annotation",
         key_added: Optional[str] = _constants.CELL_TRANSITION,
         **kwargs: Any,
     ) -> pd.DataFrame:
+        if aggregation_mode == "annotation" and (source_groups is None or target_groups is None):
+            raise ValueError("If `aggregation_mode=annotation`, `source_groups` and `target_groups` cannot be `None`.")
+        if aggregation_mode == "cell" and source_groups is None and target_groups is None:
+            raise ValueError("At least one of `source_groups` and `target_group` must be specified.")
+
         _check_argument_compatibility_cell_transition(
             source_annotation=source_groups,
             target_annotation=target_groups,
+            aggregation_mode=aggregation_mode,
             **kwargs,
         )
         tm = self._cell_transition_online(
             source=source,
             target=target,
             source_groups=source_groups,
             target_groups=target_groups,
+            aggregation_mode=aggregation_mode,
             **kwargs,
         )
         if key_added is not None:
-            aggregation_mode = kwargs.pop("aggregation_mode")
             forward = kwargs.pop("forward")
             if aggregation_mode == "cell" and "cell" in self.adata.obs:
                 raise KeyError(f"Aggregation is already present in `adata.obs[{aggregation_mode!r}]`.")
             plot_vars = {
                 "transition_matrix": tm,
                 "source": source,
                 "target": target,
@@ -179,26 +173,26 @@
             self.adata, source_groups
         )
         target_annotation_key, target_annotations, target_annotations_ordered = _validate_args_cell_transition(
             self.adata if other_adata is None else other_adata, target_groups
         )
         df_source = _get_df_cell_transition(
             self.adata,
+            [source_annotation_key, target_annotation_key],
             key,
             source,
-            source_annotation_key,
         )
         df_target = _get_df_cell_transition(
             self.adata if other_adata is None else other_adata,
+            [source_annotation_key, target_annotation_key],
             key if other_adata is None else other_key,
             target,
-            target_annotation_key,
         )
 
-        source_annotations_verified, target_annotations_verified = self._validate_annotations(
+        source_annotations_verified, target_annotations_verified = _validate_annotations(
             df_source=df_source,
             df_target=df_target,
             source_annotation_key=source_annotation_key,
             target_annotation_key=target_annotation_key,
             source_annotations=source_annotations,
             target_annotations=target_annotations,
             aggregation_mode=aggregation_mode,
@@ -372,50 +366,14 @@
     def _flatten(self: AnalysisMixinProtocol[K, B], data: Dict[K, ArrayLike], *, key: Optional[str]) -> ArrayLike:
         tmp = np.full(len(self.adata), np.nan)
         for k, v in data.items():
             mask = self.adata.obs[key] == k
             tmp[mask] = np.squeeze(v)
         return tmp
 
-    def _validate_annotations(
-        self: AnalysisMixinProtocol[K, B],
-        df_source: pd.DataFrame,
-        df_target: pd.DataFrame,
-        source_annotation_key: Optional[str] = None,
-        target_annotation_key: Optional[str] = None,
-        source_annotations: Optional[List[Any]] = None,
-        target_annotations: Optional[List[Any]] = None,
-        aggregation_mode: Literal["annotation", "cell"] = "annotation",
-        forward: bool = False,
-    ) -> Tuple[List[Any], List[Any]]:
-        if forward:
-            if TYPE_CHECKING:  # checked in _check_argument_compatibility_cell_transition(
-                assert target_annotations is not None
-            target_annotations_verified = list(
-                set(df_target[target_annotation_key].cat.categories).intersection(target_annotations)
-            )
-            if not len(target_annotations_verified):
-                raise ValueError(f"None of `{target_annotations}`, found in the target annotations.")
-            source_annotations_verified = _validate_annotations_helper(
-                df_source, source_annotation_key, source_annotations, aggregation_mode
-            )
-            return source_annotations_verified, target_annotations_verified
-
-        if TYPE_CHECKING:  # checked in _check_argument_compatibility_cell_transition(
-            assert source_annotations is not None
-        source_annotations_verified = list(
-            set(df_source[source_annotation_key].cat.categories).intersection(set(source_annotations))
-        )
-        if not len(source_annotations_verified):
-            raise ValueError(f"None of `{source_annotations}`, found in the source annotations.")
-        target_annotations_verified = _validate_annotations_helper(
-            df_target, target_annotation_key, target_annotations, aggregation_mode
-        )
-        return source_annotations_verified, target_annotations_verified
-
     def _annotation_aggregation_transition(
         self: AnalysisMixinProtocol[K, B],
         source: K,
         target: K,
         annotation_key: str,
         annotations_1: List[Any],
         annotations_2: List[Any],
@@ -436,15 +394,15 @@
                 return_all=False,
                 scale_by_marginals=False,
                 split_mass=False,
                 key_added=None,
                 return_data=True,
             )
             df["distribution"] = result
-            cell_dist = df[df[annotation_key].isin(annotations_2)].groupby(annotation_key).sum()
+            cell_dist = df[df[annotation_key].isin(annotations_2)].groupby(annotation_key).sum(numeric_only=True)
             cell_dist /= cell_dist.sum()
             tm.loc[subset, :] = [
                 cell_dist.loc[annotation, "distribution"] if annotation in cell_dist.distribution.index else 0
                 for annotation in annotations_2
             ]
         return tm
```

### Comparing `moscot-0.2.0/src/moscot/base/problems/_utils.py` & `moscot-0.3.0/src/moscot/base/problems/_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -37,14 +37,50 @@
 from moscot._docs._docs import d
 from moscot._logging import logger
 from moscot._types import ArrayLike, Str_Dict_t
 
 Callback = Callable[..., Any]
 
 
+def _validate_annotations(
+    df_source: pd.DataFrame,
+    df_target: pd.DataFrame,
+    source_annotation_key: Optional[str] = None,
+    target_annotation_key: Optional[str] = None,
+    source_annotations: Optional[List[Any]] = None,
+    target_annotations: Optional[List[Any]] = None,
+    aggregation_mode: Literal["annotation", "cell"] = "annotation",
+    forward: bool = False,
+) -> Tuple[List[Any], List[Any]]:
+    if forward:
+        if TYPE_CHECKING:  # checked in _check_argument_compatibility_cell_transition(
+            assert target_annotations is not None
+        target_annotations_verified = list(
+            set(df_target[target_annotation_key].cat.categories).intersection(target_annotations)
+        )
+        if not len(target_annotations_verified):
+            raise ValueError(f"None of `{target_annotations}`, found in the target annotations.")
+        source_annotations_verified = _validate_annotations_helper(
+            df_source, source_annotation_key, source_annotations, aggregation_mode
+        )
+        return source_annotations_verified, target_annotations_verified
+
+    if TYPE_CHECKING:  # checked in _check_argument_compatibility_cell_transition(
+        assert source_annotations is not None
+    source_annotations_verified = list(
+        set(df_source[source_annotation_key].cat.categories).intersection(set(source_annotations))
+    )
+    if not len(source_annotations_verified):
+        raise ValueError(f"None of `{source_annotations}`, found in the source annotations.")
+    target_annotations_verified = _validate_annotations_helper(
+        df_target, target_annotation_key, target_annotations, aggregation_mode
+    )
+    return source_annotations_verified, target_annotations_verified
+
+
 def _validate_annotations_helper(
     df: pd.DataFrame,
     annotation_key: Optional[str] = None,
     annotations: Optional[List[Any]] = None,
     aggregation_mode: Literal["annotation", "cell"] = "annotation",
 ) -> List[Any]:
     if aggregation_mode == "annotation":
@@ -78,27 +114,29 @@
         raise ValueError(
             "If aggregation mode is `'annotation'`, " "source or target annotation in `adata.obs` must be provided."
         )
 
 
 def _get_df_cell_transition(
     adata: AnnData,
-    key: Optional[str] = None,
-    key_value: Optional[Any] = None,
-    annotation_key: Optional[str] = None,
+    annotation_keys: List[Optional[str]],
+    filter_key: Optional[str] = None,
+    filter_value: Optional[Any] = None,
 ) -> pd.DataFrame:
-    if key is None:
-        return adata.obs[[annotation_key]].copy()
-    return adata[adata.obs[key] == key_value].obs[[annotation_key]].copy()
+    if filter_key is not None:
+        adata = adata[adata.obs[filter_key] == filter_value]
+    return adata.obs[list({ak for ak in annotation_keys if ak is not None})].copy()
 
 
 def _validate_args_cell_transition(
     adata: AnnData,
     arg: Str_Dict_t,
-) -> Tuple[str, List[Any], Optional[List[str]]]:
+) -> Tuple[Optional[str], List[Any], Optional[List[str]]]:
+    if arg is None:
+        return None, [], None
     if isinstance(arg, str):
         try:
             return arg, adata.obs[arg].cat.categories, None
         except KeyError:
             raise KeyError(f"Unable to fetch data from `adata.obs[{arg!r}]`.") from None
         except AttributeError:
             raise AttributeError(f"Data in `adata.obs[{arg!r}]` is not categorical.") from None
```

### Comparing `moscot-0.2.0/src/moscot/base/problems/birth_death.py` & `moscot-0.3.0/src/moscot/base/problems/birth_death.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,43 +109,32 @@
             - human, proliferation - :cite:`tirosh:16:science`.
             - human, apoptosis - `Hallmark Apoptosis,
               MSigDB <https://www.gsea-msigdb.org/gsea/msigdb/cards/HALLMARK_APOPTOSIS>`_.
             - mouse, proliferation - :cite:`tirosh:16:nature`.
             - mouse, apoptosis - `Hallmark P53 Pathway, MSigDB
               <https://www.gsea-msigdb.org/gsea/msigdb/cards/HALLMARK_P53_PATHWAY>`_.
         """
-        # TODO(michalk8): make slightly more compact
-        if gene_set_proliferation is None:
-            self.proliferation_key = None
-        else:
-            if isinstance(gene_set_proliferation, str):
-                sc.tl.score_genes(
-                    self.adata,
-                    proliferation_markers(gene_set_proliferation),  # type: ignore[arg-type]
-                    score_name=proliferation_key,
-                    **kwargs,
-                )
-            else:
-                sc.tl.score_genes(self.adata, gene_set_proliferation, score_name=proliferation_key, **kwargs)
+        if isinstance(gene_set_proliferation, str):
+            gene_set_proliferation = proliferation_markers(gene_set_proliferation)  # type: ignore[arg-type]
+        if gene_set_proliferation is not None:
+            sc.tl.score_genes(self.adata, gene_set_proliferation, score_name=proliferation_key, **kwargs)
             self.proliferation_key = proliferation_key
-        if gene_set_apoptosis is None:
-            self.apoptosis_key = None
         else:
-            if isinstance(gene_set_apoptosis, str):
-                sc.tl.score_genes(
-                    self.adata,
-                    apoptosis_markers(gene_set_apoptosis),  # type: ignore[arg-type]
-                    score_name=apoptosis_key,
-                    **kwargs,
-                )
-            else:
-                sc.tl.score_genes(self.adata, gene_set_apoptosis, score_name=apoptosis_key, **kwargs)
+            self.proliferation_key = None
+
+        if isinstance(gene_set_apoptosis, str):
+            gene_set_apoptosis = apoptosis_markers(gene_set_apoptosis)  # type: ignore[arg-type]
+        if gene_set_apoptosis is not None:
+            sc.tl.score_genes(self.adata, gene_set_apoptosis, score_name=apoptosis_key, **kwargs)
             self.apoptosis_key = apoptosis_key
-        if gene_set_proliferation is None and gene_set_apoptosis is None:
-            logger.info(
+        else:
+            self.apoptosis_key = None
+
+        if self.proliferation_key is None and self.apoptosis_key is None:
+            logger.warning(
                 "At least one of `gene_set_proliferation` or `gene_set_apoptosis` must be provided to score genes."
             )
 
         return self  # type: ignore[return-value]
 
     @property
     def proliferation_key(self) -> Optional[str]:
```

### Comparing `moscot-0.2.0/src/moscot/base/problems/compound_problem.py` & `moscot-0.3.0/src/moscot/base/problems/compound_problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,15 +260,16 @@
         Returns
         -------
         The solver problem.
         """
         if TYPE_CHECKING:
             assert isinstance(self._problem_manager, ProblemManager)
         problems = self._problem_manager.get_problems(stage=stage)
-        # TODO(michalk8): print how many problems are being solved?
+
+        logger.info(f"Solving `{len(problems)}` problems")
         for _, problem in problems.items():
             logger.info(f"Solving problem {problem}.")
             _ = problem.solve(**kwargs)
 
         return self
 
     @attributedispatch(attr="_policy")
@@ -648,14 +649,14 @@
             linear_cost_matrix = data[mask, :][:, mask_2]
             if sp.issparse(linear_cost_matrix):
                 logger.warning("Linear cost matrix being densified.")
                 linear_cost_matrix = linear_cost_matrix.A
             return {"xy": TaggedArray(linear_cost_matrix, tag=Tag.COST_MATRIX)}
 
         if term in ("x", "y"):
-            quad_cost_matrix = data[mask, :][:, mask_2]
+            quad_cost_matrix = data[mask, :][:, mask]
             if sp.issparse(quad_cost_matrix):
                 logger.warning("Quadratic cost matrix being densified.")
                 quad_cost_matrix = quad_cost_matrix.A
             return {term: TaggedArray(quad_cost_matrix, tag=Tag.COST_MATRIX)}
 
         raise ValueError(f"Expected `term` to be one of `x`, `y`, or `xy`, found `{term!r}`.")
```

### Comparing `moscot-0.2.0/src/moscot/base/problems/manager.py` & `moscot-0.3.0/src/moscot/base/problems/manager.py`

 * *Files identical despite different names*

### Comparing `moscot-0.2.0/src/moscot/base/problems/problem.py` & `moscot-0.3.0/src/moscot/base/problems/problem.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import types
 from abc import ABC, abstractmethod
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     List,
     Literal,
@@ -19,15 +20,15 @@
 import scanpy as sc
 from anndata import AnnData
 
 from moscot import backends
 from moscot._docs._docs import d
 from moscot._logging import logger
 from moscot._types import ArrayLike, CostFn_t, Device_t, ProblemKind_t, ProblemStage_t
-from moscot.base.output import BaseSolverOutput
+from moscot.base.output import BaseSolverOutput, MatrixSolverOutput
 from moscot.base.problems._utils import require_solution, wrap_prepare, wrap_solve
 from moscot.base.solver import OTSolver
 from moscot.utils.tagged_array import Tag, TaggedArray
 
 __all__ = ["BaseProblem", "OTProblem"]
 
 
@@ -86,17 +87,16 @@
                 data[range(start, min(start + offset, adata.n_obs))] = 1.0
             else:
                 raise TypeError(f"Unable to interpret subset of type `{type(subset)}`.")
         elif not hasattr(data, "shape"):
             if subset is None:  # allow for numeric values
                 data = np.asarray(adata.obs[data], dtype=float)
             else:
-                if isinstance(subset, str):
-                    subset = [subset]
-                data = np.asarray(adata.obs[data].isin(subset), dtype=float)
+                sset = subset if isinstance(subset, list) else [subset]  # type:ignore[list-item]
+                data = np.asarray(adata.obs[data].isin(sset), dtype=float)
         else:
             data = np.asarray(data, dtype=float)
 
         if split_mass:
             data = _split_mass(data)
 
         if data.ndim != 2:
@@ -209,39 +209,39 @@
 
         # restich together
         return TaggedArray(data_src=x_array.data_src, data_tgt=y_array.data_src, tag=Tag.POINT_CLOUD, cost=x_array.cost)
 
     @wrap_prepare
     def prepare(
         self,
-        xy: Optional[Union[Mapping[str, Any], TaggedArray]] = None,
-        x: Optional[Union[Mapping[str, Any], TaggedArray]] = None,
-        y: Optional[Union[Mapping[str, Any], TaggedArray]] = None,
+        xy: Union[Mapping[str, Any], TaggedArray] = types.MappingProxyType({}),
+        x: Union[Mapping[str, Any], TaggedArray] = types.MappingProxyType({}),
+        y: Union[Mapping[str, Any], TaggedArray] = types.MappingProxyType({}),
         a: Optional[Union[bool, str, ArrayLike]] = None,
         b: Optional[Union[bool, str, ArrayLike]] = None,
         **kwargs: Any,
     ) -> "OTProblem":
         """Prepare optimal transport problem.
 
         Depending on which arguments are passed:
 
-        - if only ``xy`` is passed, :attr:`problem_kind` will be ``'linear'``.
-        - if only ``x`` and ``y`` are passed, :attr:`problem_kind` will be ``'quadratic'``.
-        - if all ``xy``, ``x`` and ``y`` are passed, :attr:`problem_kind` will be ``'quadratic'``.
+        - if only ``xy`` is non-empty, :attr:`problem_kind` will be ``'linear'``.
+        - if only ``x`` and ``y`` are non-empty, :attr:`problem_kind` will be ``'quadratic'``.
+        - if all ``xy``, ``x`` and ``y`` are non-empty, :attr:`problem_kind` will be ``'quadratic'``.
 
         Parameters
         ----------
         xy
-            Geometry defining the linear term. If passed as a :class:`dict`,
+            Geometry defining the linear term. If a non-empty :class:`dict`,
             :meth:`~moscot.utils.tagged_array.TaggedArray.from_adata` will be called.
         x
-            First geometry defining the quadratic term. If passed as a :class:`dict`,
+            First geometry defining the quadratic term. If a non-empty :class:`dict`,
             :meth:`~moscot.utils.tagged_array.TaggedArray.from_adata` will be called.
         y
-            Second geometry defining the quadratic term. If passed as a :class:`dict`,
+            Second geometry defining the quadratic term. If a non-empty :class:`dict`,
             :meth:`~moscot.utils.tagged_array.TaggedArray.from_adata` will be called.
         a
             Source marginals. Valid value are:
 
             - :class:`str`: key in :attr:`adata_src` :attr:`~anndata.AnnData.obs` where the marginals are stored.
             - :class:`bool`: if `True`, compute the marginals from :attr:`adata_src`, otherwise use uniform.
             - :class:`~numpy.ndarray`: array of shape ``[n,]`` containing the source marginals.
@@ -267,28 +267,28 @@
         - :attr:`b`: target marginals of shape ``[m,]``.
         - :attr:`problem_kind`: kind of the optimal transport problem.
         - :attr:`solution`: set to :obj:`None`.
         """
         self._x = self._y = self._xy = self._solution = None
         # TODO(michalk8): in the future, have a better dispatch
         # fmt: off
-        if xy is not None and x is None and y is None:
+        if xy and not x and not y:
             self._problem_kind = "linear"
             self._xy = xy if isinstance(xy, TaggedArray) else self._handle_linear(**xy)
-        elif x is not None and y is not None and xy is None:
+        elif x and y and not xy:
             self._problem_kind = "quadratic"
             if isinstance(x, TaggedArray):
                 self._x = x
             else:
                 self._x = TaggedArray.from_adata(self.adata_src, dist_key=self._src_key, **x)
             if isinstance(y, TaggedArray):
                 self._y = y
             else:
                 self._y = TaggedArray.from_adata(self.adata_tgt, dist_key=self._tgt_key, **y)
-        elif xy is not None and x is not None and y is not None:
+        elif xy and x and y:
             self._problem_kind = "quadratic"
             self._xy = xy if isinstance(xy, TaggedArray) else self._handle_linear(**xy)
             if isinstance(x, TaggedArray):
                 self._x = x
             else:
                 self._x = TaggedArray.from_adata(self.adata_src, dist_key=self._src_key, **x)
             if isinstance(y, TaggedArray):
@@ -315,35 +315,36 @@
         Parameters
         ----------
         backend
             Which backend to use, see :func:`~moscot.backends.utils.get_available_backends`.
         device
             Device where to transfer the solution, see :meth:`moscot.base.output.BaseSolverOutput.to`.
         kwargs
-            Keyword arguments for :meth:`moscot.base.solver.BaseSolver.__call__`.
+            Keyword arguments for :class:`moscot.base.solver.BaseSolver` or
+            :meth:`moscot.base.solver.BaseSolver.__call__`.
 
         Returns
         -------
         Self and modifies the following attributes:
 
         - :attr:`solver`: optimal transport solver.
         - :attr:`solution`: optimal transport solution.
         """
-        self._solver = backends.get_solver(self.problem_kind, backend=backend, **kwargs)
-
-        # TODO: add ScaleCost(scale_cost)
+        solver_class = backends.get_solver(self.problem_kind, backend=backend, return_class=True)
+        init_kwargs, call_kwargs = solver_class._partition_kwargs(**kwargs)
+        self._solver = solver_class(**init_kwargs)
 
         self._solution = self._solver(  # type: ignore[misc]
             xy=self._xy,
             x=self._x,
             y=self._y,
             a=self.a,
             b=self.b,
             device=device,
-            **kwargs,
+            **call_kwargs,
         )
         return self
 
     @require_solution
     def push(
         self,
         data: Optional[Union[str, ArrayLike]] = None,
@@ -419,14 +420,50 @@
         Array of shape ``[n, d]``.
         """
         if TYPE_CHECKING:
             assert isinstance(self.solution, BaseSolverOutput)
         data = self._get_mass(self.adata_tgt, data=data, subset=subset, normalize=normalize, split_mass=split_mass)
         return self.solution.pull(data, **kwargs)
 
+    def set_solution(
+        self, solution: Union[ArrayLike, pd.DataFrame, BaseSolverOutput], *, overwrite: bool = False, **kwargs: Any
+    ) -> "OTProblem":
+        """Set the :attr:`solution`.
+
+        Parameters
+        ----------
+        solution
+            Solution for this problem. If a :class:`~pandas.DataFrame` is passed, its index and columns
+            must match the indexes of :attr:`adata_src` and :attr:`adata_tgt`, respectively.
+        overwrite
+            Whether to overwrite an existing solution.
+        kwargs
+            Keyword arguments for :class:`~moscot.base.output.MatrixSolverOutput`.
+
+        Returns
+        -------
+        Set :attr:`solution` and return self.
+        """
+        if not overwrite and self.solution is not None:
+            raise ValueError(f"`{self}` already contains a solution, use `overwrite=True` to overwrite it.")
+
+        if isinstance(solution, pd.DataFrame):
+            pd.testing.assert_series_equal(self.adata_src.obs_names.to_series(), solution.index.to_series())
+            pd.testing.assert_series_equal(self.adata_tgt.obs_names.to_series(), solution.columns.to_series())
+            solution = solution.to_numpy()
+        if not isinstance(solution, BaseSolverOutput):
+            solution = MatrixSolverOutput(solution, **kwargs)
+
+        if solution.shape != self.shape:
+            raise ValueError(f"Expected solution to have shape `{self.shape}`, found `{solution.shape}`.")
+
+        self._stage = "solved"
+        self._solution = solution
+        return self
+
     @staticmethod
     def _local_pca_callback(
         term: Literal["x", "y", "xy"],
         adata: AnnData,
         adata_y: Optional[AnnData] = None,
         layer: Optional[str] = None,
         n_comps: int = 30,
```

### Comparing `moscot-0.2.0/src/moscot/base/solver.py` & `moscot-0.3.0/src/moscot/base/solver.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     Any,
     Dict,
     Generic,
     Literal,
     Mapping,
     NamedTuple,
     Optional,
+    Set,
     Tuple,
     TypeVar,
     Union,
 )
 
 from moscot._docs._docs import d
 from moscot._logging import logger
@@ -133,14 +134,40 @@
         Returns
         -------
         The solver output.
         """
         data = self._prepare(**kwargs)
         return self._solve(data)
 
+    @classmethod
+    @abc.abstractmethod
+    def _call_kwargs(cls) -> Tuple[Set[str], Set[str]]:
+        """Return arguments specific for :meth:`__call__` and arguments shared with :class:`BaseSolver`."""
+
+    @classmethod
+    def _partition_kwargs(cls, **kwargs: Any) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+        """Partition keyword arguments.
+
+        Used by the :meth:`~moscot.problems.base.BaseProblem.solve`.
+
+        Parameters
+        ----------
+        kwargs
+            Keyword arguments to partition.
+
+        Returns
+        -------
+        Keyword arguments for :class:`BaseSolver` and :meth:`__call__`, respectively.
+        """
+        call_kws, shared_kws = cls._call_kwargs()
+        init_kwargs = {k: v for k, v in kwargs.items() if k not in call_kws or k in shared_kws}
+        call_kwargs = {k: v for k, v in kwargs.items() if k in call_kws or k in shared_kws}
+
+        return init_kwargs, call_kwargs
+
 
 @d.get_sections(base="OTSolver", sections=["Parameters", "Raises"])
 @d.dedent
 class OTSolver(TagConverter, BaseSolver[O], abc.ABC):
     """Base class for optimal transport solvers."""
 
     def __call__(
@@ -170,22 +197,22 @@
             Keyword arguments for parent's :meth:`__call__`.
 
         Returns
         -------
         The optimal transport solution.
         """
         data = self._get_array_data(xy=xy, x=x, y=y, tags=tags)
-        kwargs = {**kwargs, **self._prepare_kwargs(data)}
+        kwargs = {**kwargs, **self._untag(data)}
         res = super().__call__(**kwargs)
         if not res.converged:
             logger.warning("Solver did not converge")
 
         return res.to(device=device)  # type: ignore[return-value]
 
-    def _prepare_kwargs(self, data: TaggedArrayData) -> Dict[str, Any]:
+    def _untag(self, data: TaggedArrayData) -> Dict[str, Any]:
         if self.problem_kind == "linear":
             if data.xy is None:
                 raise ValueError("No data specified for the linear term.")
             data_kwargs: Dict[str, Any] = {"xy": data.xy}
         elif self.problem_kind == "quadratic":
             if data.x is None or data.y is None:
                 raise ValueError("No data specified for the quadratic term.")
```

### Comparing `moscot-0.2.0/src/moscot/costs/_costs.py` & `moscot-0.3.0/src/moscot/costs/_costs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, List, Mapping, Optional
 
 import networkx as nx
 import numpy as np
 
+from moscot._logging import logger
 from moscot._types import ArrayLike
 from moscot.base.cost import BaseCost
 from moscot.costs._utils import register_cost
 
 __all__ = ["LeafDistance", "BarcodeDistance"]
 
 
@@ -25,14 +26,15 @@
             raise KeyError(f"Unable to find data in `adata.{self._attr}[{self._key!r}]`.") from None
 
     def _compute(
         self,
         *_: Any,
         **__: Any,
     ) -> ArrayLike:
+        logger.info("Computing barcode distance")
         barcodes = self.data
         n_cells = barcodes.shape[0]
         distances = np.zeros((n_cells, n_cells))
         for i in range(n_cells):
             distances[i, i + 1 :] = [
                 self._scaled_hamming_dist(barcodes[i, :], barcodes[j, :]) for j in range(i + 1, n_cells)
             ]
@@ -76,14 +78,15 @@
         except KeyError:
             raise KeyError(f"Unable to find tree in `adata.{self._attr}[{self._key!r}][{self._dist_key!r}]`.") from None
 
     def _compute(
         self,
         **kwargs: Any,
     ) -> ArrayLike:
+        logger.info("Computing tree distance")
         tree = self.data
         undirected_tree = tree.to_undirected()
         leaves = self._get_leaves(undirected_tree)
         n_leaves = len(leaves)
 
         distances = np.zeros((n_leaves, n_leaves), dtype=np.float_)
         for i, leaf in enumerate(leaves):
```

### Comparing `moscot-0.2.0/src/moscot/costs/_utils.py` & `moscot-0.3.0/src/moscot/costs/_utils.py`

 * *Files identical despite different names*

### Comparing `moscot-0.2.0/src/moscot/datasets.py` & `moscot-0.3.0/src/moscot/datasets.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,76 @@
+import contextlib
 import os
+import pathlib
+import pickle
+import shutil
+import tempfile
+import urllib.request
 import warnings
 from types import MappingProxyType
-from typing import Any, List, Literal, Mapping, Optional, Tuple
+from typing import Any, Dict, List, Literal, Mapping, Optional, Tuple
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 
 from anndata import AnnData
 from scanpy import read
 
 from moscot._types import PathLike
 
-__all__ = ["mosta", "hspc", "drosophila", "sim_align", "simulate_data"]
+__all__ = [
+    "mosta",
+    "hspc",
+    "drosophila",
+    "c_elegans",
+    "zebrafish",
+    "sim_align",
+    "simulate_data",
+    "bone_marrow",
+]
 
 
 def mosta(
     path: PathLike = "~/.cache/moscot/mosta.h5ad",
+    force_download: bool = False,
     **kwargs: Any,
 ) -> AnnData:  # pragma: no cover
     """Preprocessed and extracted data as provided in :cite:`chen:22`.
 
     Includes embryo sections `E9.5`, `E2S1`, `E10.5`, `E2S1`, `E11.5`, `E1S2`.
 
     The :attr:`anndata.AnnData.X` is based on reprocessing of the counts data using
     :func:`scanpy.pp.normalize_total` and :func:`scanpy.pp.log1p`.
 
     Parameters
     ----------
     path
         Path where to save the file.
+    force_download
+        Whether to force-download the data.
     kwargs
         Keyword arguments for :func:`scanpy.read`.
 
     Returns
     -------
     Annotated data object.
     """
     return _load_dataset_from_url(
-        path, backup_url="https://figshare.com/ndownloader/files/37953852", expected_shape=(54134, 2000), **kwargs
+        path,
+        backup_url="https://figshare.com/ndownloader/files/37953852",
+        expected_shape=(54134, 2000),
+        force_download=force_download,
+        **kwargs,
     )
 
 
 def hspc(
     path: PathLike = "~/.cache/moscot/hspc.h5ad",
+    force_download: bool = False,
     **kwargs: Any,
 ) -> AnnData:  # pragma: no cover
     """CD34+ hematopoietic stem and progenitor cells from 4 healthy human donors.
 
     From the `NeurIPS Multimodal Single-Cell Integration Challenge
     <https://www.kaggle.com/competitions/open-problems-multimodal/data>`_.
 
@@ -55,114 +78,262 @@
     Subsequently, the top 2000 highly variable genes were selected. Peaks appearing in less than 5%
     of the cells were filtered out, resulting in 11595 peaks.
 
     Parameters
     ----------
     path
         Path where to save the file.
+    force_download
+        Whether to force-download the data.
     kwargs
         Keyword arguments for :func:`scanpy.read`.
 
     Returns
     -------
     Annotated data object.
     """
     return _load_dataset_from_url(
-        path, backup_url="https://figshare.com/ndownloader/files/37993503", expected_shape=(4000, 2000), **kwargs
+        path,
+        backup_url="https://figshare.com/ndownloader/files/37993503",
+        expected_shape=(4000, 2000),
+        force_download=force_download,
+        **kwargs,
     )
 
 
 def drosophila(
     path: PathLike = "~/.cache/moscot/drosophila.h5ad",
     *,
     spatial: bool,
+    force_download: bool = False,
     **kwargs: Any,
 ) -> AnnData:
     """Embryo of Drosophila melanogaster described in :cite:`Li-spatial:22`.
 
     Minimal pre-processing was performed, such as gene and cell filtering, as well as normalization.
 
     Parameters
     ----------
     path
         Path where to save the file.
     spatial
         Whether to return the spatial or the scRNA-seq dataset.
+    force_download
+        Whether to force-download the data.
     kwargs
         Keyword arguments for :func:`scanpy.read`.
 
     Returns
     -------
     Annotated data object.
     """
     path, _ = os.path.splitext(path)
     if spatial:
         return _load_dataset_from_url(
             path + "_sp.h5ad",
             backup_url="https://figshare.com/ndownloader/files/37984935",
             expected_shape=(3039, 82),
+            force_download=force_download,
             **kwargs,
         )
 
     return _load_dataset_from_url(
         path + "_sc.h5ad",
         backup_url="https://figshare.com/ndownloader/files/37984938",
         expected_shape=(1297, 2000),
+        force_download=force_download,
+        **kwargs,
+    )
+
+
+def c_elegans(
+    path: PathLike = "~/.cache/moscot/c_elegans.h5ad",
+    force_download: bool = False,
+    **kwargs: Any,
+) -> Tuple[AnnData, nx.DiGraph]:  # pragma: no cover
+    """scRNA-seq time-series dataset of C.elegans embryogenesis :cite:`packer:19`.
+
+    Contains raw counts of 46,151 cells with at least partial lineage information.
+    In addition, this downloads the known C. elegans lineage tree.
+
+    Parameters
+    ----------
+    path
+        Path where to save the file.
+    force_download
+        Whether to force-download the data.
+    kwargs
+        Keyword arguments for :func:`scanpy.read`.
+
+    Returns
+    -------
+    Annotated data object and the lineage tree.
+    """
+    adata = _load_dataset_from_url(
+        path,
+        backup_url="https://figshare.com/ndownloader/files/39943585",
+        expected_shape=(46151, 20222),
+        force_download=force_download,
+        **kwargs,
+    )
+    # TODO(michalk8): also cache or store in AnnData ad Newick + reconstruct?
+    with urllib.request.urlopen("https://figshare.com/ndownloader/files/39943603") as fin:
+        tree = pickle.load(fin)
+
+    return adata, tree
+
+
+def zebrafish(
+    path: PathLike = "~/.cache/moscot/zebrafish.h5ad",
+    force_download: bool = False,
+    **kwargs: Any,
+) -> Tuple[AnnData, Dict[str, nx.DiGraph]]:
+    """Lineage-traced scRNA-seq time-series dataset of zebrafish heart regeneration :cite:`hu:22`.
+
+    Contains gene expression vectors, LINNAEUS :cite:`spanjaard:18` reconstructed lineage trees,
+    a low-dimensional embedding, and additional metadata.
+
+    Parameters
+    ----------
+    path
+        Path where to save the file.
+    force_download
+        Whether to force-download the data.
+    kwargs
+        Keyword arguments for :func:`scanpy.read`.
+
+    Returns
+    -------
+    Annotated data object and the lineage trees.
+    """
+    adata = _load_dataset_from_url(
+        path,
+        backup_url="https://figshare.com/ndownloader/files/39951073",
+        expected_shape=(44014, 31466),
+        force_download=force_download,
+        **kwargs,
+    )
+    # TODO(michalk8): also cache or store in AnnData ad Newick + reconstruct?
+    with urllib.request.urlopen("https://figshare.com/ndownloader/files/39951076") as fin:
+        trees = pickle.load(fin)
+
+    return adata, trees
+
+
+def bone_marrow(
+    path: PathLike = "~/.cache/moscot/bone_marrow.h5ad",
+    *,
+    rna: bool,
+    force_download: bool = False,
+    **kwargs: Any,
+) -> AnnData:
+    """Multiome data of bone marrow measurements :cite:`luecken:21`.
+
+    Contains processed counts of 6,224 cells. The RNA data was filtered to 2,000 top
+    highly variable genes, the ATAC data was filtered to 8,000 top highly variable
+    peaks.
+
+    Parameters
+    ----------
+    path
+        Path where to save the file.
+    rna
+        Return the RNA data if `True`, otherwise return ATAC data.
+    force_download
+        Whether to force-download the data.
+    kwargs
+        Keyword arguments for :func:`scanpy.read`.
+
+    Returns
+    -------
+    Annotated data object.
+    """
+    path, _ = os.path.splitext(path)
+    if rna:
+        return _load_dataset_from_url(
+            path + "_rna.h5ad",
+            backup_url="https://figshare.com/ndownloader/files/40195114",
+            expected_shape=(6224, 2000),
+            force_download=force_download,
+            **kwargs,
+        )
+    return _load_dataset_from_url(
+        path + "_atac.h5ad",
+        backup_url="https://figshare.com/ndownloader/files/40195102",
+        expected_shape=(6224, 8000),
+        force_download=force_download,
         **kwargs,
     )
 
 
 def tedsim(
     path: PathLike = "~/.cache/moscot/tedsim.h5ad",
+    force_download: bool = False,
     **kwargs: Any,
 ) -> AnnData:  # pragma: no cover
     """Dataset simulated with TedSim :cite:`pan:22`.
 
-    The data was simulated with asymmetric division rate of `0.2` and intermediate state step size of `0.2` and contains
-    the following fields:
-
-    - :attr:`anndata.AnnData.obsm` ``['barcodes']``: barcodes.
-    - :attr:`anndata.AnnData.obsp` ``['barcodes_cost']``: pre-computed barcode distances.
-    - :attr:`anndata.AnnData.uns` ``['tree']``: lineage tree in the Newick format.
+    Simulated scRNA-seq dataset of a differentiation trajectory. For each cell, the dataset includes a (raw counts)
+    gene expression vector as well as a lineage barcodes. The data was simulated with asymmetric division rate of
+    :math:`0.2`, intermediate state step size of :math:`0.2` and contains the following fields:
+
+    - :attr:`obsm['barcodes'] <anndata.AnnData.obsm>` - barcodes.
+    - :attr:`obsp['cost_matrices'] <anndata.AnnData.obsp>` - precomputed lineage cost matrices.
+    - :attr:`uns['tree'] <anndata.AnnData.uns>` - lineage tree in the
+      `Newick format <https://en.wikipedia.org/wiki/Newick_format>`_.
+    - :attr:`uns['couplings' ] <anndata.AnnData.uns>` - coupling matrix based on the ground-truth lineage tree.
 
     Parameters
     ----------
     path
         Path where to save the file.
+    force_download
+        Whether to force-download the data.
     kwargs
         Keyword arguments for :func:`scanpy.read`.
 
     Returns
     -------
     Annotated data object.
     """
     return _load_dataset_from_url(
-        path, backup_url="https://figshare.com/ndownloader/files/38031258", expected_shape=(16382, 500), **kwargs
+        path,
+        backup_url="https://figshare.com/ndownloader/files/40178644",
+        expected_shape=(8448, 500),
+        force_download=force_download,
+        **kwargs,
     )
 
 
 def sim_align(
     path: PathLike = "~/.cache/moscot/sim_align.h5ad",
+    force_download: bool = False,
     **kwargs: Any,
 ) -> AnnData:  # pragma: no cover
     """Spatial transcriptomics simulated dataset as described in :cite:`Jones-spatial:22`.
 
     Parameters
     ----------
     path
         Location where the file is saved to.
+    force_download
+        Whether to force-download the data.
     kwargs
         Keyword arguments for :func:`scanpy.read`.
 
     Returns
     -------
     Annotated data object.
     """
     return _load_dataset_from_url(
-        path, backup_url="https://figshare.com/ndownloader/files/37984926", expected_shape=(1200, 500), **kwargs
+        path,
+        backup_url="https://figshare.com/ndownloader/files/37984926",
+        expected_shape=(1200, 500),
+        force_download=force_download,
+        **kwargs,
     )
 
 
 def simulate_data(
     n_distributions: int = 2,
     cells_per_distribution: int = 20,
     n_genes: int = 60,
@@ -172,16 +343,15 @@
     marginals: Optional[Tuple[str, str]] = None,
     seed: int = 0,
     quad_term: Optional[Literal["tree", "barcode", "spatial"]] = None,
     lin_cost_matrix: Optional[str] = None,
     quad_cost_matrix: Optional[str] = None,
     **kwargs: Any,
 ) -> AnnData:
-    """
-    Simulate data.
+    """Simulate data.
 
     This function is used to generate data, mainly for the purpose of
     demonstrating certain functionalities of :mod:`moscot`.
 
     Parameters
     ----------
     n_distributions
@@ -263,24 +433,33 @@
 
 
 def _load_dataset_from_url(
     fpath: PathLike,
     *,
     backup_url: str,
     expected_shape: Tuple[int, int],
+    force_download: bool = False,
     sparse: bool = True,
     cache: bool = True,
     **kwargs: Any,
 ) -> AnnData:
-    fpath = str(fpath)
+    fpath = os.path.expanduser(fpath)
     if not fpath.endswith(".h5ad"):
         fpath += ".h5ad"
-    fpath = os.path.expanduser(fpath)
 
-    adata = read(filename=fpath, backup_url=backup_url, sparse=sparse, cache=cache, **kwargs)
+    if force_download:
+        with tempfile.TemporaryDirectory() as tmpdir:
+            tmp = pathlib.Path(tmpdir) / "data.h5ad"
+            adata = read(filename=tmp, backup_url=backup_url, sparse=sparse, cache=cache, **kwargs)
+            with contextlib.suppress(FileNotFoundError):
+                os.remove(fpath)
+            shutil.move(tmp, fpath)
+    else:
+        adata = read(filename=fpath, backup_url=backup_url, sparse=sparse, cache=cache, **kwargs)
+
     if adata.shape != expected_shape:
         raise ValueError(f"Expected `AnnData` object to have shape `{expected_shape}`, found `{adata.shape}`.")
 
     return adata
 
 
 def _get_random_trees(
```

### Comparing `moscot-0.2.0/src/moscot/plotting/_plotting.py` & `moscot-0.3.0/src/moscot/plotting/_plotting.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     _plot_temporal,
     _sankey,
     get_plotting_vars,
 )
 
 if TYPE_CHECKING:
     from moscot.base.problems import CompoundProblem
-    from moscot.problems import LineageProblem, TemporalProblem
+    from moscot.problems import LineageProblem, SpatioTemporalProblem, TemporalProblem
 
 __all__ = ["cell_transition", "sankey", "push", "pull"]
 
 
 @d_plotting.dedent
 def cell_transition(
     inp: Union[AnnData, Tuple[AnnData, AnnData], "CompoundProblem"],  # type: ignore[type-arg]
@@ -116,15 +116,15 @@
     cmap: Union[str, mpl.colors.Colormap] = "viridis",
     figsize: Optional[Tuple[float, float]] = None,
     dpi: Optional[int] = None,
     save: Optional[str] = None,
     ax: Optional[mpl.axes.Axes] = None,
     return_fig: bool = False,
     **kwargs: Any,
-) -> mpl.figure.Figure:
+) -> Optional[mpl.figure.Figure]:
     """
     Plot a Sankey diagram.
 
     {desc_sankey}
 
     Parameters
     ----------
@@ -168,15 +168,15 @@
     if save:
         fig.figure.savefig(save)
     return fig if return_fig else None
 
 
 @d_plotting.dedent
 def push(
-    inp: Union[AnnData, "TemporalProblem", "LineageProblem", "CompoundProblem"],  # type: ignore[type-arg]
+    inp: Union[AnnData, "TemporalProblem", "LineageProblem", "SpatioTemporalProblem", "CompoundProblem"],  # type: ignore[type-arg]  # noqa: 501
     uns_key: str = _constants.PUSH,
     time_points: Optional[Sequence[float]] = None,
     basis: str = "umap",
     fill_value: float = np.nan,
     scale: bool = True,
     title: Optional[Union[str, List[str]]] = None,
     suptitle: Optional[str] = None,
@@ -247,20 +247,20 @@
         suptitle=suptitle,
         figsize=figsize,
         dpi=dpi,
         ax=ax,
         suptitle_fontsize=suptitle_fontsize,
         **kwargs,
     )
-    return fig.figure if return_fig else None
+    return fig if return_fig else None
 
 
 @d_plotting.dedent
 def pull(
-    inp: Union[AnnData, "TemporalProblem", "LineageProblem", "CompoundProblem"],  # type: ignore[type-arg]
+    inp: Union[AnnData, "TemporalProblem", "LineageProblem", "SpatioTemporalProblem", "CompoundProblem"],  # type: ignore[type-arg]  # noqa: 501
     uns_key: str = _constants.PULL,
     time_points: Optional[Sequence[float]] = None,
     basis: str = "umap",
     fill_value: float = np.nan,
     scale: bool = True,
     title: Optional[Union[str, List[str]]] = None,
     suptitle: Optional[str] = None,
@@ -270,15 +270,15 @@
     figsize: Optional[Tuple[float, float]] = None,
     dpi: Optional[int] = None,
     save: Optional[str] = None,
     ax: Optional[mpl.axes.Axes] = None,
     return_fig: bool = False,
     suptitle_fontsize: Optional[float] = None,
     **kwargs: Any,
-) -> mpl.figure.Figure:
+) -> Optional[mpl.figure.Figure]:
     """
     Visualise the pull result in an embedding.
 
     %(desc_sankey)s
 
     Parameters
     ----------
@@ -332,8 +332,8 @@
         suptitle=suptitle,
         figsize=figsize,
         dpi=dpi,
         ax=ax,
         suptitle_fontsize=suptitle_fontsize,
         **kwargs,
     )
-    return fig.figure if return_fig else None
+    return fig if return_fig else None
```

### Comparing `moscot-0.2.0/src/moscot/plotting/_utils.py` & `moscot-0.3.0/src/moscot/plotting/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -393,27 +393,29 @@
     suptitle: Optional[str] = None,
     figsize: Optional[Tuple[float, float]] = None,
     dpi: Optional[int] = None,
     dot_scale_factor: float = 2.0,
     na_color: str = "#e8ebe9",
     save: Optional[str] = None,
     ax: Optional[mpl.axes.Axes] = None,
-    show: bool = False,
     suptitle_fontsize: Optional[float] = None,
     **kwargs: Any,
-) -> plt.Figure:
+) -> Optional[plt.Figure]:
     if time_points is not None:
         time_points = sorted(time_points)
     if cont_cmap is None or isinstance(cont_cmap, str):
         cont_cmap = plt.get_cmap(cont_cmap)
 
-    fig, axs = plt.subplots(
-        1, 1 if time_points is None else len(time_points), figsize=figsize, dpi=dpi, constrained_layout=True
-    )
-    axs = np.ravel(axs)  # make into iterable
+    if ax is None:
+        fig, ax = plt.subplots(
+            1, 1 if time_points is None else len(time_points), figsize=figsize, dpi=dpi, constrained_layout=True
+        )
+    else:
+        fig = None
+    axs = np.ravel([ax])  # make into iterable
 
     if not push and time_points is not None:
         time_points = time_points[::-1]
 
     if isinstance(title, list):
         if TYPE_CHECKING:
             assert isinstance(time_points, list)
@@ -485,21 +487,26 @@
             sc.pl.embedding(
                 adata=adata_view,
                 basis=basis,
                 color=keys[0],
                 title=titles[i],
                 size=size,
                 ax=ax,
-                show=show,
+                show=False,
+                return_fig=False,
                 **kwargs,
             )
     if suptitle is not None:
+        if fig is None:
+            raise Warning("Cannot set `suptitle` of figure when `ax` is not `None`.")
         fig.suptitle(suptitle, fontsize=suptitle_fontsize)
     if save:
-        fig.figure.savefig(save, bbox_inches="tight")
+        if fig is None:
+            raise ValueError("Figure cannot be saved when `ax` is not `None`.")
+        fig.savefig(save, bbox_inches="tight")
     return fig
 
 
 def _color_transition(c1: str, c2: str, num: int, alpha: float) -> List[str]:
     if not mpl.colors.is_color_like(c1):
         raise ValueError(f"{c1} cannot be interpreted as an RGB color.")
     if not mpl.colors.is_color_like(c2):
```

### Comparing `moscot-0.2.0/src/moscot/problems/_utils.py` & `moscot-0.3.0/src/moscot/problems/_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+import types
 from typing import Any, Dict, Mapping, Optional, Tuple, Union
 
-from moscot._types import CostFn_t
+from moscot._types import CostFn_t, CostKwargs_t
 
 
 def handle_joint_attr(
     joint_attr: Optional[Union[str, Mapping[str, Any]]], kwargs: Dict[str, Any]
-) -> Tuple[Optional[Dict[str, Any]], Dict[str, Any]]:
+) -> Tuple[Dict[str, Any], Dict[str, Any]]:
     if joint_attr is None:
         if "xy_callback" not in kwargs:
             kwargs["xy_callback"] = "local-pca"
         kwargs.setdefault("xy_callback_kwargs", {})
-        return None, kwargs
+        return {}, kwargs
     if isinstance(joint_attr, str):
         xy = {
             "x_attr": "obsm",
             "x_key": joint_attr,
             "y_attr": "obsm",
             "y_key": joint_attr,
         }
@@ -44,38 +45,45 @@
             kwargs.setdefault("xy_callback_kwargs", {"key": joint_attr["key"]})
         kwargs.setdefault("xy_callback_kwargs", {})
         return joint_attr, kwargs
     raise TypeError(f"Expected `joint_attr` to be either `str` or `dict`, found `{type(joint_attr)}`.")
 
 
 def handle_cost(
-    xy: Optional[Mapping[str, Any]] = None,
-    x: Optional[Mapping[str, Any]] = None,
-    y: Optional[Mapping[str, Any]] = None,
+    xy: Mapping[str, Any] = types.MappingProxyType({}),
+    x: Mapping[str, Any] = types.MappingProxyType({}),
+    y: Mapping[str, Any] = types.MappingProxyType({}),
     cost: Optional[Union[CostFn_t, Mapping[str, CostFn_t]]] = None,
+    cost_kwargs: CostKwargs_t = types.MappingProxyType({}),
     **_: Any,
-) -> Tuple[Optional[Mapping[str, Any]], Optional[Mapping[str, Any]], Optional[Mapping[str, Any]]]:
+) -> Tuple[Dict[str, Any], Dict[str, Any], Dict[str, Any]]:
+    x = dict(x)
+    y = dict(y)
+    xy = dict(xy)
     if cost is None:
         return xy, x, y
-    if isinstance(cost, str):
-        if xy is not None and "cost" not in xy:
-            xy = dict(xy)
-            xy["cost"] = cost
-        if x is not None and "cost" not in x:
-            x = dict(x)
+    if isinstance(cost, str):  # if cost is a str, we use it in all terms
+        if xy and ("x_cost" not in xy or "y_cost" not in xy):
+            xy["x_cost"] = xy["y_cost"] = cost
+        if x and "cost" not in x:
             x["cost"] = cost
-        if y is not None and "cost" not in y:
-            y = dict(y)
+        if y and "cost" not in y:
             y["cost"] = cost
-        return xy, x, y
-    if isinstance(cost, Mapping):
-        if xy is not None and "cost" not in xy:
-            xy = dict(xy)
-            xy["cost"] = cost["xy"]
-        if x is not None and "cost" not in x:
-            x = dict(x)
+    elif isinstance(cost, Mapping):  # if cost is a dict, the cost is specified for each term
+        if xy and ("x_cost" not in xy or "y_cost" not in xy):
+            xy["x_cost"] = xy["y_cost"] = cost["xy"]
+        if x and "cost" not in x:
             x["cost"] = cost["x"]
-        if y is not None and "cost" not in y:
-            y = dict(y)
+        if y and "cost" not in y:
             y["cost"] = cost["y"]
-        return xy, x, y
-    raise TypeError(type(cost))
+    else:
+        raise TypeError(f"Expected `cost` to be either `str` or `dict`, found `{type(cost)}`.")
+    if xy and cost_kwargs:  # distribute the cost_kwargs, possibly explicit to x/y/xy-term
+        # extract cost_kwargs explicit to xy-term if possible
+        items = cost_kwargs["xy"].items() if "xy" in cost_kwargs else cost_kwargs.items()
+        for k, v in items:
+            xy[f"x_{k}"] = xy[f"y_{k}"] = v
+    if x and cost_kwargs:  # extract cost_kwargs explicit to x-term if possible
+        x.update(cost_kwargs.get("x", cost_kwargs))  # type:ignore[call-overload]
+    if y and cost_kwargs:  # extract cost_kwargs explicit to y-term if possible
+        y.update(cost_kwargs.get("y", cost_kwargs))  # type:ignore[call-overload]
+    return xy, x, y
```

### Comparing `moscot-0.2.0/src/moscot/problems/generic/_generic.py` & `moscot-0.3.0/src/moscot/problems/generic/_generic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-from types import MappingProxyType
-from typing import Any, Dict, List, Literal, Mapping, Optional, Tuple, Type, Union
+import types
+from typing import Any, Dict, Literal, Mapping, Optional, Tuple, Type, Union
 
 from anndata import AnnData
 
 from moscot import _constants
 from moscot._docs._docs import d
 from moscot._types import (
+    CostKwargs_t,
+    OttCostFn_t,
+    OttCostFnMap_t,
     Policy_t,
     ProblemStage_t,
     QuadInitializer_t,
     ScaleCost_t,
     SinkhornInitializer_t,
 )
 from moscot.base.problems.compound_problem import B, CompoundProblem, K
@@ -35,28 +38,30 @@
 
     @d.dedent
     def prepare(
         self,
         key: str,
         joint_attr: Optional[Union[str, Mapping[str, Any]]] = None,
         policy: Literal["sequential", "pairwise", "explicit"] = "sequential",
-        cost: Literal["sq_euclidean", "cosine", "bures", "unbalanced_bures"] = "sq_euclidean",
+        cost: OttCostFn_t = "sq_euclidean",
+        cost_kwargs: CostKwargs_t = types.MappingProxyType({}),
         a: Optional[str] = None,
         b: Optional[str] = None,
         **kwargs: Any,
     ) -> "SinkhornProblem[K, B]":
         """
         Prepare the :class:`moscot.problems.generic.SinkhornProblem`.
 
         Parameters
         ----------
         %(key)s
         %(joint_attr)s
         %(policy)s
         %(cost_lin)s
+        %(cost_kwargs)s
         %(a)s
         %(b)s
         %(kwargs_prepare)s
 
         Returns
         -------
         :class:`moscot.problems.generic.SinkhornProblem`
@@ -67,15 +72,15 @@
 
         Examples
         --------
         %(ex_prepare)s
         """
         self.batch_key = key  # type: ignore[misc]
         xy, kwargs = handle_joint_attr(joint_attr, kwargs)
-        xy, _, _ = handle_cost(xy=xy, cost=cost)
+        xy, _, _ = handle_cost(xy=xy, cost=cost, cost_kwargs=cost_kwargs)
         return super().prepare(
             key=key,
             policy=policy,
             xy=xy,
             cost=cost,
             a=a,
             b=b,
@@ -89,24 +94,22 @@
         tau_a: float = 1.0,
         tau_b: float = 1.0,
         rank: int = -1,
         scale_cost: ScaleCost_t = "mean",
         batch_size: Optional[int] = None,
         stage: Union[ProblemStage_t, Tuple[ProblemStage_t, ...]] = ("prepared", "solved"),
         initializer: SinkhornInitializer_t = None,
-        initializer_kwargs: Mapping[str, Any] = MappingProxyType({}),
+        initializer_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
         jit: bool = True,
         threshold: float = 1e-3,
         lse_mode: bool = True,
         norm_error: int = 1,
         inner_iterations: int = 10,
         min_iterations: int = 0,
         max_iterations: int = 2000,
-        gamma: float = 10.0,
-        gamma_rescale: bool = True,
         device: Optional[Literal["cpu", "gpu", "tpu"]] = None,
         cost_matrix_rank: Optional[int] = None,
         **kwargs: Any,
     ) -> "SinkhornProblem[K,B]":
         """
         Solve optimal transport problems defined in :class:`moscot.problems.generic.SinkhornProblem`.
 
@@ -119,15 +122,14 @@
         %(scale_cost)s
         %(pointcloud_kwargs)s
         %(stage)s
         %(initializer_lin)s
         %(initializer_kwargs)s
         %(jit)s
         %(sinkhorn_kwargs)s
-        %(sinkhorn_lr_kwargs)s
         %(device_solve)s
         %(cost_matrix_rank)s
         %(kwargs_linear)s
 
         Returns
         -------
         :class:`moscot.problems.generic.SinkhornProblem`.
@@ -149,16 +151,14 @@
             jit=jit,
             threshold=threshold,
             lse_mode=lse_mode,
             norm_error=norm_error,
             inner_iterations=inner_iterations,
             min_iterations=min_iterations,
             max_iterations=max_iterations,
-            gamma=gamma,
-            gamma_rescale=gamma_rescale,
             cost_matrix_rank=cost_matrix_rank,
             device=device,
             **kwargs,
         )
 
     @property
     def _base_problem_type(self) -> Type[B]:
@@ -183,37 +183,36 @@
     def __init__(self, adata: AnnData, **kwargs: Any):
         super().__init__(adata, **kwargs)
 
     @d.dedent
     def prepare(
         self,
         key: str,
-        GW_x: Union[str, Mapping[str, Any]],
-        GW_y: Union[str, Mapping[str, Any]],
+        x_attr: Union[str, Mapping[str, Any]],
+        y_attr: Union[str, Mapping[str, Any]],
         joint_attr: Optional[Union[str, Mapping[str, Any]]] = None,
         policy: Literal["sequential", "pairwise", "explicit"] = "sequential",
-        cost: Union[
-            Literal["sq_euclidean", "cosine", "bures", "unbalanced_bures"],
-            Mapping[str, Literal["sq_euclidean", "cosine", "bures", "unbalanced_bures"]],
-        ] = "sq_euclidean",
+        cost: OttCostFnMap_t = "sq_euclidean",
+        cost_kwargs: CostKwargs_t = types.MappingProxyType({}),
         a: Optional[str] = None,
         b: Optional[str] = None,
         **kwargs: Any,
     ) -> "GWProblem[K, B]":
         """
         Prepare the :class:`moscot.problems.generic.GWProblem`.
 
         Parameters
         ----------
         %(key)s
-        %(GW_x)s
-        %(GW_y)s
+        %(x_attr)s
+        %(y_attr)s
         %(joint_attr)s
         %(policy)s
         %(cost)s
+        %(cost_kwargs)s
         %(a)s
         %(b)s
         %(kwargs_prepare)s
 
         Returns
         -------
         :class:`moscot.problems.generic.GWProblem`
@@ -224,25 +223,25 @@
 
         Examples
         --------
         %(ex_prepare)s
         """
         self.batch_key = key  # type: ignore[misc]
 
-        GW_updated: List[Dict[str, Any]] = [{}] * 2
-        for i, z in enumerate([GW_x, GW_y]):
+        def set_quad_defaults(z: Union[str, Mapping[str, Any]]) -> Dict[str, str]:
             if isinstance(z, str):
-                GW_updated[i] = {"attr": "obsm", "key": z, "tag": "point_cloud"}  # cost handled by handle_cost
-            elif isinstance(z, dict):
-                GW_updated[i] = z
-            else:
-                raise TypeError("`GW_x` and `GW_y` must be of type `str` or `dict`.")
+                return {"attr": "obsm", "key": z, "tag": "point_cloud"}  # cost handled by handle_cost
+            if isinstance(z, Mapping):
+                return dict(z)
+            raise TypeError("`x_attr` and `y_attr` must be of type `str` or `dict`.")
 
         xy, kwargs = handle_joint_attr(joint_attr, kwargs)
-        xy, x, y = handle_cost(xy=xy, x=GW_updated[0], y=GW_updated[1], cost=cost)
+        x = set_quad_defaults(x_attr)
+        y = set_quad_defaults(y_attr)
+        xy, x, y = handle_cost(xy=xy, x=x, y=y, cost=cost, cost_kwargs=cost_kwargs)
         return super().prepare(
             key=key,
             xy=xy,
             x=x,
             y=y,
             policy=policy,
             cost=cost,
@@ -259,24 +258,20 @@
         tau_a: float = 1.0,
         tau_b: float = 1.0,
         rank: int = -1,
         scale_cost: ScaleCost_t = "mean",
         batch_size: Optional[int] = None,
         stage: Union[ProblemStage_t, Tuple[ProblemStage_t, ...]] = ("prepared", "solved"),
         initializer: QuadInitializer_t = None,
-        initializer_kwargs: Mapping[str, Any] = MappingProxyType({}),
+        initializer_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
         jit: bool = True,
         min_iterations: int = 5,
         max_iterations: int = 50,
         threshold: float = 1e-3,
-        gamma: float = 10.0,
-        gamma_rescale: bool = True,
-        ranks: Union[int, Tuple[int, ...]] = -1,
-        tolerances: Union[float, Tuple[float, ...]] = 1e-2,
-        linear_solver_kwargs: Mapping[str, Any] = MappingProxyType({}),
+        linear_solver_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
         device: Optional[Literal["cpu", "gpu", "tpu"]] = None,
         **kwargs: Any,
     ) -> "GWProblem[K,B]":
         """
         Solve optimal transport problems defined in :class:`moscot.problems.generic.GWProblem`.
 
         Parameters
@@ -288,16 +283,14 @@
         %(rank)s
         %(scale_cost)s
         %(pointcloud_kwargs)s
         %(stage)s
         %(initializer_quad)s
         %(initializer_kwargs)s
         %(gw_kwargs)s
-        %(sinkhorn_lr_kwargs)s
-        %(gw_lr_kwargs)s
         %(linear_solver_kwargs)s
         %(device_solve)s
         %(kwargs_quad)s
 
         Returns
         -------
         :class:`moscot.problems.generic.GWProblem`.
@@ -317,18 +310,14 @@
             stage=stage,
             initializer=initializer,
             initializer_kwargs=initializer_kwargs,
             jit=jit,
             min_iterations=min_iterations,
             max_iterations=max_iterations,
             threshold=threshold,
-            gamma=gamma,
-            gamma_rescale=gamma_rescale,
-            ranks=ranks,
-            tolerances=tolerances,
             linear_solver_kwargs=linear_solver_kwargs,
             device=device,
             **kwargs,
         )
 
     @property
     def _base_problem_type(self) -> Type[B]:
```

### Comparing `moscot-0.2.0/src/moscot/problems/generic/_mixins.py` & `moscot-0.3.0/src/moscot/problems/generic/_mixins.py`

 * *Files identical despite different names*

### Comparing `moscot-0.2.0/src/moscot/problems/space/_alignment.py` & `moscot-0.3.0/src/moscot/problems/spatiotemporal/_spatio_temporal.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,139 +1,165 @@
-from types import MappingProxyType
+import types
 from typing import Any, Literal, Mapping, Optional, Tuple, Type, Union
 
+from anndata import AnnData
+
 from moscot import _constants
 from moscot._docs._docs import d
-from moscot._types import Policy_t, ProblemStage_t, QuadInitializer_t, ScaleCost_t
-from moscot.base.problems.compound_problem import B, CompoundProblem, K
-from moscot.base.problems.problem import OTProblem
-from moscot.problems._utils import handle_cost, handle_joint_attr
-from moscot.problems.space._mixins import SpatialAlignmentMixin
+from moscot._types import (
+    CostKwargs_t,
+    Numeric_t,
+    OttCostFnMap_t,
+    Policy_t,
+    ProblemStage_t,
+    QuadInitializer_t,
+    ScaleCost_t,
+)
+from moscot.base.problems.birth_death import BirthDeathMixin, BirthDeathProblem
+from moscot.base.problems.compound_problem import B
+from moscot.problems.space import AlignmentProblem, SpatialAlignmentMixin
+from moscot.problems.time import TemporalMixin
 
-__all__ = ["AlignmentProblem"]
+__all__ = ["SpatioTemporalProblem"]
 
 
 @d.dedent
-class AlignmentProblem(CompoundProblem[K, B], SpatialAlignmentMixin[K, B]):
+class SpatioTemporalProblem(
+    TemporalMixin[Numeric_t, BirthDeathProblem],
+    BirthDeathMixin,
+    AlignmentProblem[Numeric_t, BirthDeathProblem],
+    SpatialAlignmentMixin[Numeric_t, BirthDeathProblem],
+):
     """
-    Class for aligning spatial omics data, based on :cite:`zeira:22`.
+    Class for analyzing time series spatial single cell data.
 
-    The `AlignmentProblem` allows to align spatial omics data via optimal transport.
+    The `SpatioTemporalProblem` allows to model and analyze spatio-temporal single cell data
+    by matching cells belonging to two different time points via OT.
 
     Parameters
     ----------
     %(adata)s
     """
 
+    # TODO(michalk8): check if this is necessary
+    def __init__(self, adata: AnnData, **kwargs: Any):
+        super().__init__(adata, **kwargs)
+
     @d.dedent
     def prepare(
         self,
-        batch_key: str,
+        time_key: str,
         spatial_key: str = "spatial",
         joint_attr: Optional[Union[str, Mapping[str, Any]]] = None,
-        policy: Literal["sequential", "star"] = "sequential",
-        reference: Optional[str] = None,
-        cost: Union[
-            Literal["sq_euclidean", "cosine", "bures", "unbalanced_bures"],
-            Mapping[str, Literal["sq_euclidean", "cosine", "bures", "unbalanced_bures"]],
-        ] = "sq_euclidean",
+        policy: Literal["sequential", "tril", "triu", "explicit"] = "sequential",
+        cost: OttCostFnMap_t = "sq_euclidean",
+        cost_kwargs: CostKwargs_t = types.MappingProxyType({}),
         a: Optional[str] = None,
         b: Optional[str] = None,
+        marginal_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
         **kwargs: Any,
-    ) -> "AlignmentProblem[K, B]":
+    ) -> "SpatioTemporalProblem":
         """Prepare the problem.
 
-        This method prepares the data to be passed to the optimal transport solver.
+        This method executes multiple steps to prepare the problem for the Optimal Transport solver to be ready
+        to solve it.
 
         Parameters
         ----------
-        %(batch_key)s
+        %(time_key)s
         %(spatial_key)s
         %(joint_attr)s
         %(policy)s
-
-        reference
-            Only used if `policy="star"`, it's the value for reference stored
-            in :attr:`anndata.AnnData.obs` ``["batch_key"]``.
-
         %(cost)s
+        %(cost_kwargs)s
         %(a)s
         %(b)s
         %(kwargs_prepare)s
 
         Returns
         -------
-        :class:`moscot.problems.space.MappingProblem`.
+        The prepared problem.
+
+        Notes
+        -----
+        If `a` and `b` are provided `marginal_kwargs` are ignored.
 
         Examples
         --------
         %(ex_prepare)s
         """
-        self.spatial_key = spatial_key
-        self.batch_key = batch_key
-
-        x = y = {"attr": "obsm", "key": self.spatial_key, "tag": "point_cloud"}
-
-        xy, kwargs = handle_joint_attr(joint_attr, kwargs)
-        xy, x, y = handle_cost(xy=xy, x=x, y=y, cost=cost)
+        # spatial key set in AlignmentProblem
+        # handle_joint_attr and handle_cost in AlignmentProblem
+        self.temporal_key = time_key
+        # TODO(michalk8): needs to be modified, move into BirthDeathMixin?
+        marginal_kwargs = dict(marginal_kwargs)
+        marginal_kwargs["proliferation_key"] = self.proliferation_key
+        marginal_kwargs["apoptosis_key"] = self.apoptosis_key
+        if a is None:
+            a = self.proliferation_key is not None or self.apoptosis_key is not None
+        if b is None:
+            b = self.proliferation_key is not None or self.apoptosis_key is not None
 
         return super().prepare(
-            x=x, y=y, xy=xy, policy=policy, key=batch_key, reference=reference, cost=cost, a=a, b=b, **kwargs
+            spatial_key=spatial_key,
+            batch_key=time_key,
+            joint_attr=joint_attr,
+            policy=policy,
+            reference=None,
+            cost=cost,
+            cost_kwargs=cost_kwargs,
+            a=a,
+            b=b,
+            marginal_kwargs=marginal_kwargs,
+            **kwargs,
         )
 
     @d.dedent
     def solve(
         self,
         alpha: Optional[float] = 0.5,
-        epsilon: Optional[float] = 1e-2,
+        epsilon: Optional[float] = 1e-3,
         tau_a: float = 1.0,
         tau_b: float = 1.0,
         rank: int = -1,
         scale_cost: ScaleCost_t = "mean",
         batch_size: Optional[int] = None,
         stage: Union[ProblemStage_t, Tuple[ProblemStage_t, ...]] = ("prepared", "solved"),
         initializer: QuadInitializer_t = None,
-        initializer_kwargs: Mapping[str, Any] = MappingProxyType({}),
+        initializer_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
         jit: bool = True,
         min_iterations: int = 5,
         max_iterations: int = 50,
         threshold: float = 1e-3,
-        gamma: float = 10.0,
-        gamma_rescale: bool = True,
-        ranks: Union[int, Tuple[int, ...]] = -1,
-        tolerances: Union[float, Tuple[float, ...]] = 1e-2,
-        linear_solver_kwargs: Mapping[str, Any] = MappingProxyType({}),
+        linear_solver_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
         device: Optional[Literal["cpu", "gpu", "tpu"]] = None,
         **kwargs: Any,
-    ) -> "AlignmentProblem[K,B]":
-        """
-        Solve optimal transport problems defined in :class:`moscot.problems.space.AlignmentProblem`.
+    ) -> "SpatioTemporalProblem":
+        """Solve the problem.
 
         Parameters
         ----------
         %(alpha)s
         %(epsilon)s
         %(tau_a)s
         %(tau_b)s
         %(rank)s
         %(scale_cost)s
         %(pointcloud_kwargs)s
         %(stage)s
         %(initializer_quad)s
         %(initializer_kwargs)s
         %(gw_kwargs)s
-        %(sinkhorn_lr_kwargs)s
-        %(gw_lr_kwargs)s
         %(linear_solver_kwargs)s
         %(device_solve)s
         %(kwargs_quad_fused)s
 
         Returns
         -------
-        :class:`moscot.problems.space.AlignmentProblem`.
+        The solved problem.
 
         Examples
         --------
         %(ex_solve_quadratic)s
         """
         return super().solve(
             alpha=alpha,
@@ -146,23 +172,24 @@
             stage=stage,
             initializer=initializer,
             initializer_kwargs=initializer_kwargs,
             jit=jit,
             min_iterations=min_iterations,
             max_iterations=max_iterations,
             threshold=threshold,
-            gamma=gamma,
-            gamma_rescale=gamma_rescale,
-            ranks=ranks,
-            tolerances=tolerances,
             linear_solver_kwargs=linear_solver_kwargs,
             device=device,
             **kwargs,
-        )  # type: ignore[return-value]
+        )
 
     @property
-    def _base_problem_type(self) -> Type[B]:
-        return OTProblem  # type: ignore[return-value]
+    def _valid_policies(self) -> Tuple[Policy_t, ...]:
+        return (
+            _constants.SEQUENTIAL,
+            _constants.TRIL,
+            _constants.TRIU,
+            _constants.EXPLICIT,
+        )  # type: ignore[return-value]
 
     @property
-    def _valid_policies(self) -> Tuple[Policy_t, ...]:
-        return _constants.SEQUENTIAL, _constants.STAR  # type: ignore[return-value]
+    def _base_problem_type(self) -> Type[B]:  # type: ignore[override]
+        return BirthDeathProblem  # type: ignore[return-value]
```

### Comparing `moscot-0.2.0/src/moscot/problems/space/_mapping.py` & `moscot-0.3.0/src/moscot/problems/space/_mapping.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from types import MappingProxyType
+import types
 from typing import Any, Literal, Mapping, Optional, Sequence, Tuple, Type, Union
 
 from anndata import AnnData
 
 from moscot import _constants
 from moscot._docs._docs import d
 from moscot._types import (
     ArrayLike,
+    CostKwargs_t,
+    OttCostFnMap_t,
     Policy_t,
     ProblemStage_t,
     QuadInitializer_t,
     ScaleCost_t,
-    Str_Dict_t,
 )
 from moscot.base.problems.compound_problem import B, CompoundProblem, K
 from moscot.base.problems.problem import OTProblem
 from moscot.problems._utils import handle_cost, handle_joint_attr
 from moscot.problems.space._mixins import SpatialMappingMixin
 from moscot.utils.subset_policy import DummyPolicy, ExternalStarPolicy
 
@@ -74,23 +75,21 @@
             tgt_key=tgt,
             **kwargs,
         )
 
     @d.dedent
     def prepare(
         self,
-        sc_attr: Str_Dict_t,
+        sc_attr: Union[str, Mapping[str, Any]],
         batch_key: Optional[str] = None,
         spatial_key: Union[str, Mapping[str, Any]] = "spatial",
         var_names: Optional[Sequence[Any]] = None,
         joint_attr: Optional[Union[str, Mapping[str, Any]]] = None,
-        cost: Union[
-            Literal["sq_euclidean", "cosine", "bures", "unbalanced_bures"],
-            Mapping[str, Literal["sq_euclidean", "cosine", "bures", "unbalanced_bures"]],
-        ] = "sq_euclidean",
+        cost: OttCostFnMap_t = "sq_euclidean",
+        cost_kwargs: CostKwargs_t = types.MappingProxyType({}),
         a: Optional[str] = None,
         b: Optional[str] = None,
         **kwargs: Any,
     ) -> "MappingProblem[K]":
         """
         Prepare the :class:`moscot.problems.space.MappingProblem`.
 
@@ -106,14 +105,15 @@
 
         var_names
             List of shared features to be used for the linear problem. If None, it defaults to the intersection
             between ``adata_sc`` and ``adata_sp``. If an empty list is pass, it defines a quadratic problem.
 
         %(joint_attr)s
         %(cost)s
+        %(cost_kwargs)s
         %(a)s
         %(b)s
         %(kwargs_prepare)s
 
         Returns
         -------
         :class:`moscot.problems.space.MappingProblem`.
@@ -129,17 +129,17 @@
             self.spatial_key = spatial_key
         else:
             self.spatial_key = spatial_key["key"]
         self.filtered_vars = var_names
         if self.filtered_vars is not None:
             xy, kwargs = handle_joint_attr(joint_attr, kwargs)
         else:
-            xy = None
-        xy, x, y = handle_cost(xy=xy, x=x, y=y, cost=cost)
-        if xy is not None:
+            xy = {}
+        xy, x, y = handle_cost(xy=xy, x=x, y=y, cost=cost, cost_kwargs=cost_kwargs)
+        if xy:
             kwargs["xy"] = xy
         return super().prepare(x=x, y=y, policy="external_star", key=batch_key, cost=cost, a=a, b=b, **kwargs)
 
     @d.dedent
     def solve(
         self,
         alpha: Optional[float] = 0.5,
@@ -147,24 +147,20 @@
         tau_a: float = 1.0,
         tau_b: float = 1.0,
         rank: int = -1,
         scale_cost: ScaleCost_t = "mean",
         batch_size: Optional[int] = None,
         stage: Union[ProblemStage_t, Tuple[ProblemStage_t, ...]] = ("prepared", "solved"),
         initializer: QuadInitializer_t = None,
-        initializer_kwargs: Mapping[str, Any] = MappingProxyType({}),
+        initializer_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
         jit: bool = True,
         min_iterations: int = 5,
         max_iterations: int = 50,
         threshold: float = 1e-3,
-        gamma: float = 10.0,
-        gamma_rescale: bool = True,
-        ranks: Union[int, Tuple[int, ...]] = -1,
-        tolerances: Union[float, Tuple[float, ...]] = 1e-2,
-        linear_solver_kwargs: Mapping[str, Any] = MappingProxyType({}),
+        linear_solver_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
         device: Optional[Literal["cpu", "gpu", "tpu"]] = None,
         **kwargs: Any,
     ) -> "MappingProblem[K]":
         """
         Solve optimal transport problems defined in :class:`moscot.problems.space.MappingProblem`.
 
         Parameters
@@ -176,16 +172,14 @@
         %(rank)s
         %(scale_cost)s
         %(pointcloud_kwargs)s
         %(stage)s
         %(initializer_quad)s
         %(initializer_kwargs)s
         %(gw_kwargs)s
-        %(sinkhorn_lr_kwargs)s
-        %(gw_lr_kwargs)s
         %(linear_solver_kwargs)s
         %(device_solve)s
         %(kwargs_quad_fused)s
 
         Returns
         -------
         :class:`moscot.problems.space.MappingProblem`.
@@ -205,18 +199,14 @@
             stage=stage,
             initializer=initializer,
             initializer_kwargs=initializer_kwargs,
             jit=jit,
             min_iterations=min_iterations,
             max_iterations=max_iterations,
             threshold=threshold,
-            gamma=gamma,
-            gamma_rescale=gamma_rescale,
-            ranks=ranks,
-            tolerances=tolerances,
             linear_solver_kwargs=linear_solver_kwargs,
             device=device,
             **kwargs,
         )  # type: ignore[return-value]
 
     @property
     def adata_sc(self) -> AnnData:
@@ -240,11 +230,7 @@
     @property
     def _base_problem_type(self) -> Type[B]:
         return OTProblem  # type: ignore[return-value]
 
     @property
     def _valid_policies(self) -> Tuple[Policy_t, ...]:
         return _constants.EXTERNAL_STAR, _constants.DUMMY  # type: ignore[return-value]
-
-    @property
-    def _secondary_adata(self) -> Optional[AnnData]:
-        return self._adata_sc
```

### Comparing `moscot-0.2.0/src/moscot/problems/space/_mixins.py` & `moscot-0.3.0/src/moscot/problems/space/_mixins.py`

 * *Files identical despite different names*

### Comparing `moscot-0.2.0/src/moscot/problems/spatiotemporal/_spatio_temporal.py` & `moscot-0.3.0/src/moscot/problems/time/_lineage.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,113 +1,284 @@
-from types import MappingProxyType
+import types
 from typing import Any, Literal, Mapping, Optional, Tuple, Type, Union
 
 from anndata import AnnData
 
 from moscot import _constants
 from moscot._docs._docs import d
 from moscot._types import (
+    CostFnMap_t,
+    CostKwargs_t,
     Numeric_t,
+    OttCostFn_t,
     Policy_t,
     ProblemStage_t,
     QuadInitializer_t,
     ScaleCost_t,
+    SinkhornInitializer_t,
 )
 from moscot.base.problems.birth_death import BirthDeathMixin, BirthDeathProblem
-from moscot.base.problems.compound_problem import B
-from moscot.problems.space import AlignmentProblem, SpatialAlignmentMixin
-from moscot.problems.time import TemporalMixin
+from moscot.base.problems.compound_problem import B, CompoundProblem
+from moscot.problems._utils import handle_cost, handle_joint_attr
+from moscot.problems.time._mixins import TemporalMixin
 
-__all__ = ["SpatioTemporalProblem"]
+__all__ = ["TemporalProblem", "LineageProblem"]
 
 
 @d.dedent
-class SpatioTemporalProblem(
-    TemporalMixin[Numeric_t, BirthDeathProblem],
-    BirthDeathMixin,
-    AlignmentProblem[Numeric_t, BirthDeathProblem],
-    SpatialAlignmentMixin[Numeric_t, BirthDeathProblem],
+class TemporalProblem(
+    TemporalMixin[Numeric_t, BirthDeathProblem], BirthDeathMixin, CompoundProblem[Numeric_t, BirthDeathProblem]
 ):
     """
-    Class for analyzing time series spatial single cell data.
+    Class for analyzing time series single cell data based on :cite:`schiebinger:19`.
 
-    The `SpatioTemporalProblem` allows to model and analyze spatio-temporal single cell data
-    by matching cells belonging to two different time points via OT.
+    The `TemporalProblem` allows to model and analyze time series single cell data by matching
+    cells from previous time points to later time points via OT.
+    Based on the assumption that the considered cell modality is similar in consecutive time points
+    probabilistic couplings are computed between different time points.
+    This allows to understand cell trajectories by inferring ancestors and descendants of single cells.
 
     Parameters
     ----------
     %(adata)s
+
     """
 
-    # TODO(michalk8): check if this is necessary
     def __init__(self, adata: AnnData, **kwargs: Any):
         super().__init__(adata, **kwargs)
 
     @d.dedent
     def prepare(
         self,
         time_key: str,
-        spatial_key: str = "spatial",
         joint_attr: Optional[Union[str, Mapping[str, Any]]] = None,
         policy: Literal["sequential", "tril", "triu", "explicit"] = "sequential",
-        cost: Union[
-            Literal["sq_euclidean", "cosine", "bures", "unbalanced_bures"],
-            Mapping[str, Literal["sq_euclidean", "cosine", "bures", "unbalanced_bures"]],
-        ] = "sq_euclidean",
+        cost: OttCostFn_t = "sq_euclidean",
+        cost_kwargs: CostKwargs_t = types.MappingProxyType({}),
         a: Optional[str] = None,
         b: Optional[str] = None,
-        marginal_kwargs: Mapping[str, Any] = MappingProxyType({}),
+        marginal_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
         **kwargs: Any,
-    ) -> "SpatioTemporalProblem":
-        """Prepare the problem.
+    ) -> "TemporalProblem":
+        """
+        Prepare the :class:`moscot.problems.time.TemporalProblem`.
 
-        This method executes multiple steps to prepare the problem for the Optimal Transport solver to be ready
-        to solve it.
+        This method executes multiple steps to prepare the optimal transport problems.
 
         Parameters
         ----------
         %(time_key)s
-        %(spatial_key)s
         %(joint_attr)s
         %(policy)s
-        %(cost)s
-        %(a)s
-        %(b)s
+        %(cost_lin)s
+        %(cost_kwargs)s
+        %(a_temporal)s
+        %(b_temporal)s
+        %(marginal_kwargs)s
         %(kwargs_prepare)s
 
+
         Returns
         -------
-        The prepared problem.
+        :class:`moscot.problems.time.TemporalProblem`.
 
         Notes
         -----
         If `a` and `b` are provided `marginal_kwargs` are ignored.
 
         Examples
         --------
         %(ex_prepare)s
         """
-        # spatial key set in AlignmentProblem
-        # handle_joint_attr and handle_cost in AlignmentProblem
         self.temporal_key = time_key
-        # TODO(michalk8): needs to be modified, move into BirthDeathMixin?
+        xy, kwargs = handle_joint_attr(joint_attr, kwargs)
+        xy, x, y = handle_cost(xy=xy, x=kwargs.pop("x", {}), y=kwargs.pop("y", {}), cost=cost, cost_kwargs=cost_kwargs)
+
+        # TODO(michalk8): needs to be modified
         marginal_kwargs = dict(marginal_kwargs)
         marginal_kwargs["proliferation_key"] = self.proliferation_key
         marginal_kwargs["apoptosis_key"] = self.apoptosis_key
         if a is None:
             a = self.proliferation_key is not None or self.apoptosis_key is not None
         if b is None:
             b = self.proliferation_key is not None or self.apoptosis_key is not None
 
         return super().prepare(
-            spatial_key=spatial_key,
-            batch_key=time_key,
-            joint_attr=joint_attr,
+            key=time_key,
+            xy=xy,
+            x=x,
+            y=y,
+            policy=policy,
+            cost=None,  # cost information is already stored in x,y,xy
+            marginal_kwargs=marginal_kwargs,
+            a=a,
+            b=b,
+            **kwargs,
+        )
+
+    @d.dedent
+    def solve(
+        self,
+        epsilon: Optional[float] = 1e-3,
+        tau_a: float = 1.0,
+        tau_b: float = 1.0,
+        rank: int = -1,
+        scale_cost: ScaleCost_t = "mean",
+        batch_size: Optional[int] = None,
+        stage: Union[ProblemStage_t, Tuple[ProblemStage_t, ...]] = ("prepared", "solved"),
+        initializer: SinkhornInitializer_t = None,
+        initializer_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
+        jit: bool = True,
+        threshold: float = 1e-3,
+        lse_mode: bool = True,
+        norm_error: int = 1,
+        inner_iterations: int = 10,
+        min_iterations: int = 0,
+        max_iterations: int = 2000,
+        cost_matrix_rank: Optional[int] = None,
+        device: Optional[Literal["cpu", "gpu", "tpu"]] = None,
+        **kwargs: Any,
+    ) -> "TemporalProblem":
+        """
+        Solve optimal transport problems defined in :class:`moscot.problems.time.TemporalProblem`.
+
+        Parameters
+        ----------
+        %(epsilon)s
+        %(tau_a)s
+        %(tau_b)s
+        %(rank)s
+        %(scale_cost)s
+        %(pointcloud_kwargs)s
+        %(stage)s
+        %(initializer_lin)s
+        %(initializer_kwargs)s
+        %(jit)s
+        %(sinkhorn_kwargs)s
+        %(device_solve)s
+        %(cost_matrix_rank)s
+        %(kwargs_linear)s
+
+        Returns
+        -------
+        :class:`moscot.problems.time.TemporalProblem`.
+
+        Examples
+        --------
+        %(ex_solve_linear)s
+        """
+        return super().solve(
+            epsilon=epsilon,
+            tau_a=tau_a,
+            tau_b=tau_b,
+            rank=rank,
+            scale_cost=scale_cost,
+            batch_size=batch_size,
+            stage=stage,
+            initializer=initializer,
+            initializer_kwargs=initializer_kwargs,
+            jit=jit,
+            threshold=threshold,
+            lse_mode=lse_mode,
+            norm_error=norm_error,
+            inner_iterations=inner_iterations,
+            min_iterations=min_iterations,
+            max_iterations=max_iterations,
+            cost_matrix_rank=cost_matrix_rank,
+            device=device,
+            **kwargs,
+        )  # type:ignore[return-value]
+
+    @property
+    def _base_problem_type(self) -> Type[B]:  # type: ignore[override]
+        return BirthDeathProblem  # type: ignore[return-value]
+
+    @property
+    def _valid_policies(self) -> Tuple[Policy_t, ...]:
+        return _constants.SEQUENTIAL, _constants.TRIU, _constants.EXPLICIT  # type: ignore[return-value]
+
+
+@d.dedent
+class LineageProblem(TemporalProblem):
+    """
+    Estimator for modelling time series single cell data based on moslin.
+
+    Class handling the computation and downstream analysis of temporal single cell data with lineage prior.
+
+    Parameters
+    ----------
+    %(adata)s
+    """
+
+    @d.dedent
+    def prepare(
+        self,
+        time_key: str,
+        lineage_attr: Mapping[str, Any] = types.MappingProxyType({}),
+        joint_attr: Optional[Union[str, Mapping[str, Any]]] = None,
+        policy: Literal["sequential", "tril", "triu", "sequential"] = "sequential",
+        # TODO(michalk8): update
+        cost: CostFnMap_t = "sq_euclidean",
+        cost_kwargs: CostKwargs_t = types.MappingProxyType({}),
+        a: Optional[str] = None,
+        b: Optional[str] = None,
+        marginal_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
+        **kwargs: Any,
+    ) -> "LineageProblem":
+        """
+        Prepare the :class:`moscot.problems.time.LineageProblem`.
+
+        Parameters
+        ----------
+        %(time_key)s
+
+        lineage_attr
+            Specifies the way the lineage information is processed. TODO: Specify.
+
+        %(joint_attr)s
+        %(policy)s
+        %(cost)s
+        %(cost_kwargs)s
+        %(a_temporal)s
+        %(b_temporal)s
+        %(marginal_kwargs)s
+        %(kwargs_prepare)s
+
+        Returns
+        -------
+        :class:`moscot.problems.time.LineageProblem`
+
+        Examples
+        --------
+        %(ex_prepare)s
+        """
+        if not len(lineage_attr) and ("cost_matrices" not in self.adata.obsp):
+            raise KeyError("Unable to find cost matrices in `adata.obsp['cost_matrices']`.")
+
+        x = y = lineage_attr
+
+        xy, kwargs = handle_joint_attr(joint_attr, kwargs)
+        xy, x, y = handle_cost(xy=xy, x=x, y=y, cost=cost, cost_kwargs=cost_kwargs)
+
+        x.setdefault("attr", "obsp")
+        x.setdefault("key", "cost_matrices")
+        x.setdefault("cost", "custom")
+        x.setdefault("tag", "cost_matrix")
+
+        y.setdefault("attr", "obsp")
+        y.setdefault("key", "cost_matrices")
+        y.setdefault("cost", "custom")
+        y.setdefault("tag", "cost_matrix")
+
+        return super().prepare(
+            time_key,
+            joint_attr=xy,
+            x=x,
+            y=y,
             policy=policy,
-            reference=None,
             cost=cost,
             a=a,
             b=b,
             marginal_kwargs=marginal_kwargs,
             **kwargs,
         )
 
@@ -119,51 +290,46 @@
         tau_a: float = 1.0,
         tau_b: float = 1.0,
         rank: int = -1,
         scale_cost: ScaleCost_t = "mean",
         batch_size: Optional[int] = None,
         stage: Union[ProblemStage_t, Tuple[ProblemStage_t, ...]] = ("prepared", "solved"),
         initializer: QuadInitializer_t = None,
-        initializer_kwargs: Mapping[str, Any] = MappingProxyType({}),
+        initializer_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
         jit: bool = True,
         min_iterations: int = 5,
         max_iterations: int = 50,
         threshold: float = 1e-3,
-        gamma: float = 10.0,
-        gamma_rescale: bool = True,
-        ranks: Union[int, Tuple[int, ...]] = -1,
-        tolerances: Union[float, Tuple[float, ...]] = 1e-2,
-        linear_solver_kwargs: Mapping[str, Any] = MappingProxyType({}),
+        linear_solver_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
         device: Optional[Literal["cpu", "gpu", "tpu"]] = None,
         **kwargs: Any,
-    ) -> "SpatioTemporalProblem":
-        """Solve the problem.
+    ) -> "LineageProblem":
+        """
+        Solve optimal transport problems defined in :class:`moscot.problems.time.LineageProblem`.
 
         Parameters
         ----------
         %(alpha)s
         %(epsilon)s
         %(tau_a)s
         %(tau_b)s
         %(rank)s
         %(scale_cost)s
         %(pointcloud_kwargs)s
         %(stage)s
         %(initializer_quad)s
         %(initializer_kwargs)s
         %(gw_kwargs)s
-        %(sinkhorn_lr_kwargs)s
-        %(gw_lr_kwargs)s
         %(linear_solver_kwargs)s
         %(device_solve)s
         %(kwargs_quad_fused)s
 
         Returns
         -------
-        The solved problem.
+        :class:`moscot.problems.time.LineageProblem`
 
         Examples
         --------
         %(ex_solve_quadratic)s
         """
         return super().solve(
             alpha=alpha,
@@ -176,28 +342,11 @@
             stage=stage,
             initializer=initializer,
             initializer_kwargs=initializer_kwargs,
             jit=jit,
             min_iterations=min_iterations,
             max_iterations=max_iterations,
             threshold=threshold,
-            gamma=gamma,
-            gamma_rescale=gamma_rescale,
-            ranks=ranks,
-            tolerances=tolerances,
             linear_solver_kwargs=linear_solver_kwargs,
             device=device,
             **kwargs,
         )
-
-    @property
-    def _valid_policies(self) -> Tuple[Policy_t, ...]:
-        return (
-            _constants.SEQUENTIAL,
-            _constants.TRIL,
-            _constants.TRIU,
-            _constants.EXPLICIT,
-        )  # type: ignore[return-value]
-
-    @property
-    def _base_problem_type(self) -> Type[B]:  # type: ignore[override]
-        return BirthDeathProblem  # type: ignore[return-value]
```

### Comparing `moscot-0.2.0/src/moscot/problems/time/_mixins.py` & `moscot-0.3.0/src/moscot/problems/time/_mixins.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from pandas.api.types import infer_dtype, is_numeric_dtype
 
 from anndata import AnnData
 
 from moscot import _constants
 from moscot._docs._docs_mixins import d_mixins
 from moscot._types import ArrayLike, Numeric_t, Str_Dict_t
-from moscot.base.output import BaseSolverOutput
 from moscot.base.problems._mixins import AnalysisMixin, AnalysisMixinProtocol
 from moscot.base.problems.birth_death import BirthDeathProblem
 from moscot.base.problems.compound_problem import ApplyOutput_t, B, K
 from moscot.plotting._utils import set_plotting_vars
 from moscot.utils.tagged_array import Tag
 
 __all__ = ["TemporalMixin"]
@@ -423,110 +422,88 @@
             self.adata.obs[key_added] = self._flatten(result, key=self.temporal_key)
             set_plotting_vars(self.adata, _constants.PULL, key=key_added, value=plot_vars)
         return result if return_data else None
 
     @property
     def prior_growth_rates(self: TemporalMixinProtocol[K, B]) -> Optional[pd.DataFrame]:
         """Return the prior estimate of growth rates of the cells in the source distribution."""
-        # TODO(michalk8): FIXME
+        computed = [isinstance(p.prior_growth_rates, np.ndarray) for p in self.problems.values()]
+        if not np.sum(computed):
+            return None
+
         cols = ["prior_growth_rates"]
         df_list = [
-            pd.DataFrame(problem.prior_growth_rates, index=problem.adata.obs.index, columns=cols)
+            pd.DataFrame(problem.prior_growth_rates, index=problem.adata.obs_names, columns=cols)
             for problem in self.problems.values()
         ]
-        tup = list(self)[-1]
-        df_list.append(
-            pd.DataFrame(
-                np.full(
-                    shape=(len(self.problems[tup].adata_tgt.obs), 1),
-                    fill_value=np.nan,
-                ),
-                index=self.problems[tup].adata_tgt.obs.index,
-                columns=cols,
-            )
-        )
-        return pd.concat(df_list, verify_integrity=True)
+        df_1 = pd.concat(df_list, verify_integrity=True)
+        indices_remaining = set(self.adata.obs_names) - set(df_1.index)
+        df_2 = pd.DataFrame(np.nan, index=list(indices_remaining), columns=cols)
+
+        return pd.concat([df_1, df_2], verify_integrity=True)
 
     @property
     def posterior_growth_rates(self: TemporalMixinProtocol[K, B]) -> Optional[pd.DataFrame]:
         """Return the posterior estimate of growth rates of the cells in the source distribution."""
-        # TODO(michalk8): FIXME
+        computed = [isinstance(p.posterior_growth_rates, np.ndarray) for p in self.problems.values()]
+        if not np.sum(computed):
+            return None
+
         cols = ["posterior_growth_rates"]
         df_list = [
-            pd.DataFrame(problem.posterior_growth_rates, index=problem.adata.obs.index, columns=cols)
+            pd.DataFrame(problem.posterior_growth_rates, index=problem.adata.obs_names, columns=cols)
             for problem in self.problems.values()
         ]
-        tup = list(self)[-1]
-        df_list.append(
-            pd.DataFrame(
-                np.full(
-                    shape=(len(self.problems[tup].adata_tgt.obs), 1),
-                    fill_value=np.nan,
-                ),
-                index=self.problems[tup].adata_tgt.obs.index,
-                columns=cols,
-            )
-        )
-        return pd.concat(df_list, verify_integrity=True)
+        df_1 = pd.concat(df_list, verify_integrity=True)
+        indices_remaining = set(self.adata.obs_names) - set(df_1.index)
+        df_2 = pd.DataFrame(np.nan, index=list(indices_remaining), columns=cols)
+
+        return pd.concat([df_1, df_2], verify_integrity=True)
 
-    # TODO(michalk8): refactor me
     @property
     def cell_costs_source(self: TemporalMixinProtocol[K, B]) -> Optional[pd.DataFrame]:
         """Return the cost of a cell obtained by the potentials of the optimal transport solution."""
-        sol = list(self.problems.values())[0].solution
-        if TYPE_CHECKING:
-            assert isinstance(sol, BaseSolverOutput)
-        if sol.potentials is None:
+        computed = [isinstance(s.potentials, tuple) for s in self.solutions.values()]
+        if not np.sum(computed):
             return None
+
+        cols = ["cell_cost_source"]
         df_list = [
             pd.DataFrame(
-                np.array(np.abs(problem.solution.potentials[0])),  # type: ignore[union-attr,index]
+                np.asarray(problem.solution.potentials[0]),  # type: ignore[union-attr,index]
                 index=problem.adata_src.obs_names,
-                columns=["cell_cost_source"],
+                columns=cols,
             )
             for problem in self.problems.values()
         ]
-        tup = list(self)[-1]
-        df_list.append(
-            pd.DataFrame(
-                np.full(shape=(len(self.problems[tup].adata_tgt.obs), 1), fill_value=np.nan),
-                index=self.problems[tup].adata_tgt.obs_names,
-                columns=["cell_cost_source"],
-            )
-        )
-        return pd.concat(df_list, verify_integrity=True)
+        df_1 = pd.concat(df_list, verify_integrity=True)
+        indices_remaining = set(self.adata.obs_names) - set(df_1.index)
+        df_2 = pd.DataFrame(np.nan, index=list(indices_remaining), columns=cols)
+        return pd.concat([df_1, df_2], verify_integrity=True)
 
     @property
     def cell_costs_target(self: TemporalMixinProtocol[K, B]) -> Optional[pd.DataFrame]:
-        """Return the cost of a cell (see online methods) obtained by the potentials of the OT solution."""
-        sol = list(self.problems.values())[0].solution
-        if TYPE_CHECKING:
-            assert isinstance(sol, BaseSolverOutput)
-        if sol.potentials is None:
+        """Return the cost of a cell obtained by the potentials of the optimal transport solution."""
+        computed = [isinstance(s.potentials, tuple) for s in self.solutions.values()]
+        if not np.sum(computed):
             return None
 
-        tup = list(self)[0]
+        cols = ["cell_cost_target"]
         df_list = [
             pd.DataFrame(
-                np.full(shape=(len(self.problems[tup].adata_src), 1), fill_value=np.nan),
-                index=self.problems[tup].adata_src.obs_names,
-                columns=["cell_cost_target"],
+                np.array(problem.solution.potentials[1]),  # type: ignore[union-attr,index]
+                index=problem.adata_tgt.obs_names,
+                columns=cols,
             )
+            for problem in self.problems.values()
         ]
-        df_list.extend(
-            [
-                pd.DataFrame(
-                    np.array(np.abs(problem.solution.potentials[1])),  # type: ignore[union-attr,index]
-                    index=problem.adata_tgt.obs_names,
-                    columns=["cell_cost_target"],
-                )
-                for problem in self.problems.values()
-            ]
-        )
-        return pd.concat(df_list, verify_integrity=True)
+        df_1 = pd.concat(df_list, verify_integrity=True)
+        indices_remaining = set(self.adata.obs_names) - set(df_1.index)
+        df_2 = pd.DataFrame(np.nan, index=list(indices_remaining), columns=cols)
+        return pd.concat([df_1, df_2], verify_integrity=True)
 
     # TODO(michalk8): refactor me
     def _get_data(
         self: TemporalMixinProtocol[K, B],
         source: K,
         intermediate: Optional[K] = None,
         target: Optional[K] = None,
```

### Comparing `moscot-0.2.0/src/moscot/utils/_data/allTFs_dmel.txt` & `moscot-0.3.0/src/moscot/utils/_data/allTFs_dmel.txt`

 * *Files identical despite different names*

### Comparing `moscot-0.2.0/src/moscot/utils/_data/allTFs_hg38.txt` & `moscot-0.3.0/src/moscot/utils/_data/allTFs_hg38.txt`

 * *Files identical despite different names*

### Comparing `moscot-0.2.0/src/moscot/utils/_data/allTFs_mm.txt` & `moscot-0.3.0/src/moscot/utils/_data/allTFs_mm.txt`

 * *Files identical despite different names*

### Comparing `moscot-0.2.0/src/moscot/utils/_data/human_apoptosis.txt` & `moscot-0.3.0/src/moscot/utils/_data/human_apoptosis.txt`

 * *Files identical despite different names*

### Comparing `moscot-0.2.0/src/moscot/utils/_data/human_proliferation.txt` & `moscot-0.3.0/src/moscot/utils/_data/human_proliferation.txt`

 * *Files identical despite different names*

### Comparing `moscot-0.2.0/src/moscot/utils/_data/mouse_apoptosis.txt` & `moscot-0.3.0/src/moscot/utils/_data/mouse_apoptosis.txt`

 * *Files identical despite different names*

### Comparing `moscot-0.2.0/src/moscot/utils/_data/mouse_proliferation.txt` & `moscot-0.3.0/src/moscot/utils/_data/mouse_proliferation.txt`

 * *Files identical despite different names*

### Comparing `moscot-0.2.0/src/moscot/utils/data.py` & `moscot-0.3.0/src/moscot/utils/data.py`

 * *Files identical despite different names*

### Comparing `moscot-0.2.0/src/moscot/utils/subset_policy.py` & `moscot-0.3.0/src/moscot/utils/subset_policy.py`

 * *Files identical despite different names*

### Comparing `moscot-0.2.0/src/moscot/utils/tagged_array.py` & `moscot-0.3.0/src/moscot/utils/tagged_array.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,35 +91,38 @@
         cost
             Cost function to apply to the extracted array, depending on ``tag``:
 
             - if ``tag = 'point_cloud'``, it is extracted from the ``backend``.
             - if ``tag = 'cost'`` or ``tag = 'kernel'``, and ``cost = 'custom'``,
               the extracted array is already assumed to be a cost/kernel matrix.
               Otherwise, :class:`~moscot.base.cost.BaseCost` is used to compute the cost matrix.
+        cost_kwargs
+            Keyword arguments for TODO
         backend
             Which backend to use, see :func:`~moscot.backends.utils.get_available_backends`.
         kwargs
-            Keyword arguments for :class:`~moscot.base.cost.BaseCost`.
+            Keyword arguments for :class:`~moscot.base.cost.BaseCost` or any backend-specific cost.
 
         Returns
         -------
         The tagged array.
 
         Notes
         -----
         Sparse arrays will be always densified.
         """
         if tag == Tag.COST_MATRIX:
             if cost == "custom":  # our custom cost functions
+                modifier = f"adata.{attr}" if key is None else f"adata.{attr}[{key!r}]"
                 data = cls._extract_data(adata, attr=attr, key=key)
                 if np.any(data < 0):
-                    raise ValueError("Cost matrix contains negative values.")
+                    raise ValueError(f"Cost matrix in `{modifier}` contains negative values.")
                 return cls(data_src=data, tag=Tag.COST_MATRIX, cost=None)
 
-            cost_fn = get_cost(cost, adata=adata, attr=attr, key=key, dist_key=dist_key)
+            cost_fn = get_cost(cost, backend="moscot", adata=adata, attr=attr, key=key, dist_key=dist_key)
             cost_matrix = cost_fn(**kwargs)
             return cls(data_src=cost_matrix, tag=Tag.COST_MATRIX, cost=None)
 
         # tag is either a point cloud or a kernel
         data = cls._extract_data(adata, attr=attr, key=key)
         cost_fn = get_cost(cost, backend=backend, **kwargs)
         return cls(data_src=data, tag=tag, cost=cost_fn)
```

### Comparing `moscot-0.2.0/src/moscot.egg-info/PKG-INFO` & `moscot-0.3.0/src/moscot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moscot
-Version: 0.2.0
+Version: 0.3.0
 Summary: Multi-omic single-cell optimal transport tools
 Author: Dominik Klein, Giovanni Palla, Michal Klein, Zoe Piran, Marius Lange
 Maintainer-email: Dominik Klein <dominik.klein@helmholtz-muenchen.de>, Giovanni Palla <giovanni.palla@helmholtz-muenchen.de>, Michal Klein <michal.klein@helmholtz-muenchen.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Theis Lab
         All rights reserved.
@@ -104,8 +104,8 @@
 ---------
 
 Please have a look at our `documentation <https://moscot.readthedocs.io>`_
 
 Reference
 ---------
 
-Our manuscript will be available soon.
+Our preprint "Mapping cells through time and space with moscot" can be found `here <https://www.biorxiv.org/content/10.1101/2023.05.11.540374v1>`_.
```

### Comparing `moscot-0.2.0/src/moscot.egg-info/SOURCES.txt` & `moscot-0.3.0/src/moscot.egg-info/SOURCES.txt`

 * *Files identical despite different names*


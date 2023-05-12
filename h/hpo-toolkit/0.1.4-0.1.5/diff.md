# Comparing `tmp/hpo-toolkit-0.1.4.tar.gz` & `tmp/hpo-toolkit-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpo-toolkit-0.1.4.tar", last modified: Fri Apr 14 16:17:45 2023, max compression
+gzip compressed data, was "hpo-toolkit-0.1.5.tar", last modified: Fri May 12 17:21:42 2023, max compression
```

## Comparing `hpo-toolkit-0.1.4.tar` & `hpo-toolkit-0.1.5.tar`

### file list

```diff
@@ -1,79 +1,86 @@
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.613534 hpo-toolkit-0.1.4/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)    35149 2022-12-16 17:20:05.000000 hpo-toolkit-0.1.4/LICENSE
--rw-rw-r--   0 ielis     (1000) ielis     (1000)    41595 2023-04-14 16:17:45.613534 hpo-toolkit-0.1.4/PKG-INFO
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      549 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.4/README.md
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      809 2023-03-03 16:00:11.000000 hpo-toolkit-0.1.4/pyproject.toml
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       38 2023-04-14 16:17:45.613534 hpo-toolkit-0.1.4/setup.cfg
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.601534 hpo-toolkit-0.1.4/src/
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.605534 hpo-toolkit-0.1.4/src/hpo_toolkit.egg-info/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)    41595 2023-04-14 16:17:45.000000 hpo-toolkit-0.1.4/src/hpo_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1847 2023-04-14 16:17:45.000000 hpo-toolkit-0.1.4/src/hpo_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 ielis     (1000) ielis     (1000)        1 2023-04-14 16:17:45.000000 hpo-toolkit-0.1.4/src/hpo_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 ielis     (1000) ielis     (1000)        1 2023-02-27 14:40:18.000000 hpo-toolkit-0.1.4/src/hpo_toolkit.egg-info/not-zip-safe
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       12 2023-04-14 16:17:45.000000 hpo-toolkit-0.1.4/src/hpo_toolkit.egg-info/requires.txt
--rw-rw-r--   0 ielis     (1000) ielis     (1000)        6 2023-04-14 16:17:45.000000 hpo-toolkit-0.1.4/src/hpo_toolkit.egg-info/top_level.txt
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.605534 hpo-toolkit-0.1.4/src/hpotk/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      202 2023-04-14 16:09:26.000000 hpo-toolkit-0.1.4/src/hpotk/__init__.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.605534 hpo-toolkit-0.1.4/src/hpotk/algorithm/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      158 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.4/src/hpotk/algorithm/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     6912 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.4/src/hpotk/algorithm/_traversal.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.605534 hpo-toolkit-0.1.4/src/hpotk/annotations/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      267 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.4/src/hpotk/annotations/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     9105 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.4/src/hpotk/annotations/_base.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2577 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.4/src/hpotk/annotations/_simple.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.605534 hpo-toolkit-0.1.4/src/hpotk/annotations/load/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       54 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.4/src/hpotk/annotations/load/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      307 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.4/src/hpotk/annotations/load/_api.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.605534 hpo-toolkit-0.1.4/src/hpotk/annotations/load/hpoa/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       43 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.4/src/hpotk/annotations/load/hpoa/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     8861 2023-04-14 14:23:26.000000 hpo-toolkit-0.1.4/src/hpotk/annotations/load/hpoa/_impl.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.605534 hpo-toolkit-0.1.4/src/hpotk/constants/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       18 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/constants/__init__.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.605534 hpo-toolkit-0.1.4/src/hpotk/constants/hpo/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      139 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/constants/hpo/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      452 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/constants/hpo/base.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2428 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.4/src/hpotk/constants/hpo/frequency.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1925 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/constants/hpo/inheritance.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1419 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/constants/hpo/onset.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1989 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/constants/hpo/organ_system.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      376 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/constants/hpo/severity.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.609534 hpo-toolkit-0.1.4/src/hpotk/graph/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      154 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/graph/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1289 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/graph/_api.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1625 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/graph/_csr_graph.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     4741 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.4/src/hpotk/graph/_factory.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.609534 hpo-toolkit-0.1.4/src/hpotk/graph/csr/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       55 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/graph/csr/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     7494 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/graph/csr/_csr.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     5587 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/graph/csr/test__csr.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.609534 hpo-toolkit-0.1.4/src/hpotk/model/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      365 2023-04-14 14:23:26.000000 hpo-toolkit-0.1.4/src/hpotk/model/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      887 2023-04-13 21:02:33.000000 hpo-toolkit-0.1.4/src/hpotk/model/_base.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)    10107 2023-04-14 14:23:26.000000 hpo-toolkit-0.1.4/src/hpotk/model/_term.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2821 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.4/src/hpotk/model/_term_id.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      856 2023-04-14 14:23:26.000000 hpo-toolkit-0.1.4/src/hpotk/model/_util.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.609534 hpo-toolkit-0.1.4/src/hpotk/ontology/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      126 2022-12-22 14:58:29.000000 hpo-toolkit-0.1.4/src/hpotk/ontology/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2003 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.4/src/hpotk/ontology/_api.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      238 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.4/src/hpotk/ontology/_attrs.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     4567 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/ontology/_default.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.609534 hpo-toolkit-0.1.4/src/hpotk/ontology/load/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       24 2023-02-27 15:19:11.000000 hpo-toolkit-0.1.4/src/hpotk/ontology/load/__init__.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.609534 hpo-toolkit-0.1.4/src/hpotk/ontology/load/obographs/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      110 2023-02-27 15:20:14.000000 hpo-toolkit-0.1.4/src/hpotk/ontology/load/obographs/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     5930 2023-04-14 14:23:26.000000 hpo-toolkit-0.1.4/src/hpotk/ontology/load/obographs/_factory.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     6859 2023-03-14 15:54:53.000000 hpo-toolkit-0.1.4/src/hpotk/ontology/load/obographs/_load.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     9853 2023-04-14 14:23:26.000000 hpo-toolkit-0.1.4/src/hpotk/ontology/load/obographs/_model.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      828 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.4/src/hpotk/ontology/load/obographs/test_load.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     3432 2023-02-28 13:59:18.000000 hpo-toolkit-0.1.4/src/hpotk/util.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.613534 hpo-toolkit-0.1.4/src/hpotk/validate/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      213 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.4/src/hpotk/validate/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     4412 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.4/src/hpotk/validate/_hpo.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1756 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.4/src/hpotk/validate/_model.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.613534 hpo-toolkit-0.1.4/tests/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     3052 2023-02-27 17:09:23.000000 hpo-toolkit-0.1.4/tests/test_algorithm.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2400 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.4/tests/test_disease.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     7087 2023-04-14 14:23:26.000000 hpo-toolkit-0.1.4/tests/test_obographs.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     4681 2023-04-14 14:23:26.000000 hpo-toolkit-0.1.4/tests/test_term.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2070 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/tests/test_term_id.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     4962 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.4/tests/test_validate.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.885328 hpo-toolkit-0.1.5/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)    35149 2022-12-16 17:20:05.000000 hpo-toolkit-0.1.5/LICENSE
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)    42078 2023-05-12 17:21:42.885328 hpo-toolkit-0.1.5/PKG-INFO
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      834 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/README.md
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      987 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/pyproject.toml
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       38 2023-05-12 17:21:42.885328 hpo-toolkit-0.1.5/setup.cfg
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.857328 hpo-toolkit-0.1.5/src/
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.865328 hpo-toolkit-0.1.5/src/hpo_toolkit.egg-info/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)    42078 2023-05-12 17:21:42.000000 hpo-toolkit-0.1.5/src/hpo_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2092 2023-05-12 17:21:42.000000 hpo-toolkit-0.1.5/src/hpo_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)        1 2023-05-12 17:21:42.000000 hpo-toolkit-0.1.5/src/hpo_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)        1 2023-02-27 14:40:18.000000 hpo-toolkit-0.1.5/src/hpo_toolkit.egg-info/not-zip-safe
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       12 2023-05-12 17:21:42.000000 hpo-toolkit-0.1.5/src/hpo_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)        6 2023-05-12 17:21:42.000000 hpo-toolkit-0.1.5/src/hpo_toolkit.egg-info/top_level.txt
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.865328 hpo-toolkit-0.1.5/src/hpotk/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      380 2023-05-12 17:16:47.000000 hpo-toolkit-0.1.5/src/hpotk/__init__.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.865328 hpo-toolkit-0.1.5/src/hpotk/algorithm/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      183 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/algorithm/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2696 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/algorithm/_augment.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     6339 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/algorithm/_traversal.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.869328 hpo-toolkit-0.1.5/src/hpotk/algorithm/similarity/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      206 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/algorithm/similarity/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1898 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/algorithm/similarity/_ic.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     6489 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/algorithm/similarity/_model.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2728 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/algorithm/similarity/_resnik.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.869328 hpo-toolkit-0.1.5/src/hpotk/annotations/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      351 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/annotations/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     3309 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/annotations/_api.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     8192 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/annotations/_base.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     3409 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/annotations/_simple.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.869328 hpo-toolkit-0.1.5/src/hpotk/annotations/load/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       54 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.5/src/hpotk/annotations/load/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      307 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.5/src/hpotk/annotations/load/_api.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.869328 hpo-toolkit-0.1.5/src/hpotk/annotations/load/hpoa/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       43 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.5/src/hpotk/annotations/load/hpoa/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     8895 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/annotations/load/hpoa/_impl.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.869328 hpo-toolkit-0.1.5/src/hpotk/constants/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       18 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.5/src/hpotk/constants/__init__.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.873328 hpo-toolkit-0.1.5/src/hpotk/constants/hpo/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      139 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.5/src/hpotk/constants/hpo/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      452 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.5/src/hpotk/constants/hpo/base.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2428 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.5/src/hpotk/constants/hpo/frequency.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1925 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.5/src/hpotk/constants/hpo/inheritance.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1419 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.5/src/hpotk/constants/hpo/onset.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1989 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.5/src/hpotk/constants/hpo/organ_system.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      376 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.5/src/hpotk/constants/hpo/severity.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.877328 hpo-toolkit-0.1.5/src/hpotk/graph/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      239 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/graph/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2064 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/graph/_api.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     5865 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/graph/_csr_graph.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     9243 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/graph/_factory.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.877328 hpo-toolkit-0.1.5/src/hpotk/graph/csr/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       90 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/graph/csr/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     7766 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/graph/csr/_csr.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     5587 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.5/src/hpotk/graph/csr/test__csr.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     4768 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/graph/test__csr_graph.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     5299 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/graph/test__factory.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.877328 hpo-toolkit-0.1.5/src/hpotk/model/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      380 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/model/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1908 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/model/_base.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)    10107 2023-05-10 21:31:14.000000 hpo-toolkit-0.1.5/src/hpotk/model/_term.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2821 2023-05-09 16:09:29.000000 hpo-toolkit-0.1.5/src/hpotk/model/_term_id.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.881328 hpo-toolkit-0.1.5/src/hpotk/ontology/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      126 2022-12-22 14:58:29.000000 hpo-toolkit-0.1.5/src/hpotk/ontology/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2003 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.5/src/hpotk/ontology/_api.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      238 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.5/src/hpotk/ontology/_attrs.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     4567 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.5/src/hpotk/ontology/_default.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.881328 hpo-toolkit-0.1.5/src/hpotk/ontology/load/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       24 2023-02-27 15:19:11.000000 hpo-toolkit-0.1.5/src/hpotk/ontology/load/__init__.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.881328 hpo-toolkit-0.1.5/src/hpotk/ontology/load/obographs/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      110 2023-02-27 15:20:14.000000 hpo-toolkit-0.1.5/src/hpotk/ontology/load/obographs/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     5930 2023-04-14 14:23:26.000000 hpo-toolkit-0.1.5/src/hpotk/ontology/load/obographs/_factory.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     6917 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/ontology/load/obographs/_load.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     9853 2023-04-14 14:23:26.000000 hpo-toolkit-0.1.5/src/hpotk/ontology/load/obographs/_model.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      828 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.5/src/hpotk/ontology/load/obographs/test_load.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     7105 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/util.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.881328 hpo-toolkit-0.1.5/src/hpotk/validate/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      213 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.5/src/hpotk/validate/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     4770 2023-05-12 17:05:54.000000 hpo-toolkit-0.1.5/src/hpotk/validate/_hpo.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2356 2023-05-12 17:05:54.000000 hpo-toolkit-0.1.5/src/hpotk/validate/_model.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.885328 hpo-toolkit-0.1.5/tests/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2400 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.5/tests/test_disease.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2922 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/tests/test_obographs.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     4681 2023-04-14 14:23:26.000000 hpo-toolkit-0.1.5/tests/test_term.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2070 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.5/tests/test_term_id.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     4962 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.5/tests/test_validate.py
```

### Comparing `hpo-toolkit-0.1.4/LICENSE` & `hpo-toolkit-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.4/PKG-INFO` & `hpo-toolkit-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpo-toolkit
-Version: 0.1.4
+Version: 0.1.5
 Summary: A toolkit for working with Human Phenotype Ontology in Python
 Author-email: Daniel Danis <daniel.gordon.danis@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -676,22 +676,30 @@
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Repository, https://github.com/TheJacksonLaboratory/hpo-toolkit
 Keywords: human phenotype ontology,HPO,library
-Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hpo-toolkit
 
+![Build status](https://img.shields.io/github/actions/workflow/status/TheJacksonLaboratory/hpo-toolkit/python_ci.yml)
+![PyPi downloads](https://img.shields.io/pypi/dm/hpo-toolkit.svg?label=Pypi%20downloads)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hpo-toolkit)
+
 A toolkit for working with Human Phenotype Ontology in Python
 
 ## Install
 
 HPO toolkit is available from PyPi:
 
 ```shell
```

### Comparing `hpo-toolkit-0.1.4/src/hpo_toolkit.egg-info/PKG-INFO` & `hpo-toolkit-0.1.5/src/hpo_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpo-toolkit
-Version: 0.1.4
+Version: 0.1.5
 Summary: A toolkit for working with Human Phenotype Ontology in Python
 Author-email: Daniel Danis <daniel.gordon.danis@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -676,22 +676,30 @@
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Repository, https://github.com/TheJacksonLaboratory/hpo-toolkit
 Keywords: human phenotype ontology,HPO,library
-Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hpo-toolkit
 
+![Build status](https://img.shields.io/github/actions/workflow/status/TheJacksonLaboratory/hpo-toolkit/python_ci.yml)
+![PyPi downloads](https://img.shields.io/pypi/dm/hpo-toolkit.svg?label=Pypi%20downloads)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hpo-toolkit)
+
 A toolkit for working with Human Phenotype Ontology in Python
 
 ## Install
 
 HPO toolkit is available from PyPi:
 
 ```shell
```

### Comparing `hpo-toolkit-0.1.4/src/hpo_toolkit.egg-info/SOURCES.txt` & `hpo-toolkit-0.1.5/src/hpo_toolkit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,22 @@
 src/hpo_toolkit.egg-info/dependency_links.txt
 src/hpo_toolkit.egg-info/not-zip-safe
 src/hpo_toolkit.egg-info/requires.txt
 src/hpo_toolkit.egg-info/top_level.txt
 src/hpotk/__init__.py
 src/hpotk/util.py
 src/hpotk/algorithm/__init__.py
+src/hpotk/algorithm/_augment.py
 src/hpotk/algorithm/_traversal.py
+src/hpotk/algorithm/similarity/__init__.py
+src/hpotk/algorithm/similarity/_ic.py
+src/hpotk/algorithm/similarity/_model.py
+src/hpotk/algorithm/similarity/_resnik.py
 src/hpotk/annotations/__init__.py
+src/hpotk/annotations/_api.py
 src/hpotk/annotations/_base.py
 src/hpotk/annotations/_simple.py
 src/hpotk/annotations/load/__init__.py
 src/hpotk/annotations/load/_api.py
 src/hpotk/annotations/load/hpoa/__init__.py
 src/hpotk/annotations/load/hpoa/_impl.py
 src/hpotk/constants/__init__.py
@@ -26,34 +32,34 @@
 src/hpotk/constants/hpo/onset.py
 src/hpotk/constants/hpo/organ_system.py
 src/hpotk/constants/hpo/severity.py
 src/hpotk/graph/__init__.py
 src/hpotk/graph/_api.py
 src/hpotk/graph/_csr_graph.py
 src/hpotk/graph/_factory.py
+src/hpotk/graph/test__csr_graph.py
+src/hpotk/graph/test__factory.py
 src/hpotk/graph/csr/__init__.py
 src/hpotk/graph/csr/_csr.py
 src/hpotk/graph/csr/test__csr.py
 src/hpotk/model/__init__.py
 src/hpotk/model/_base.py
 src/hpotk/model/_term.py
 src/hpotk/model/_term_id.py
-src/hpotk/model/_util.py
 src/hpotk/ontology/__init__.py
 src/hpotk/ontology/_api.py
 src/hpotk/ontology/_attrs.py
 src/hpotk/ontology/_default.py
 src/hpotk/ontology/load/__init__.py
 src/hpotk/ontology/load/obographs/__init__.py
 src/hpotk/ontology/load/obographs/_factory.py
 src/hpotk/ontology/load/obographs/_load.py
 src/hpotk/ontology/load/obographs/_model.py
 src/hpotk/ontology/load/obographs/test_load.py
 src/hpotk/validate/__init__.py
 src/hpotk/validate/_hpo.py
 src/hpotk/validate/_model.py
-tests/test_algorithm.py
 tests/test_disease.py
 tests/test_obographs.py
 tests/test_term.py
 tests/test_term_id.py
 tests/test_validate.py
```

### Comparing `hpo-toolkit-0.1.4/src/hpotk/algorithm/_traversal.py` & `hpo-toolkit-0.1.5/src/hpotk/algorithm/_traversal.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,125 +1,107 @@
 import typing
 from warnings import warn
-from collections import deque
 
 from hpotk.model import TermId, CURIE_OR_TERM_ID
 from hpotk.graph import OntologyGraph, GraphAware
 
 
 def get_ancestors(g: typing.Union[GraphAware, OntologyGraph],
                   source: CURIE_OR_TERM_ID,
                   include_source: bool = False) -> typing.FrozenSet[TermId]:
     """
-    Get all ancestor `TermId`s of the `source` term (parents, grandparents, great-grandparents etc.)..
+    Get all ancestor :class:`TermId`\\ (s). of the `source` term (parents, grandparents, great-grandparents etc.)..
 
-    The method raises a `ValueError` if inputs do not meet the requirement described below.
+    The method raises a :class:`ValueError` if inputs do not meet the requirement described below.
 
     :param g: the ontology graph or a graph-aware entity
-    :param source: `TermId` or a term ID curie as a `str (e.g. `HP:1234567`)
+    :param source: `:class:`TermId` or a term ID curie as a `str (e.g. `HP:1234567`)
     :param include_source: whether to include the `source` term in the resulting set
-    :return: a `frozenset` with ancestor `TermId`s
+    :return: a `frozenset` with ancestor :class:`TermId`\\ (s).
     """
     # Check
     g = _check_ontology_graph_is_available(g)
     source = _check_curie_or_term_id(source)
 
     # Init
-    buffer: typing.Deque[TermId] = deque()
+    builder: set[TermId] = set()
     if include_source:
-        buffer.append(source)
-    else:
-        for parent in g.get_parents(source):
-            buffer.append(parent)
+        builder.add(source)
+
+    builder.update(g.get_ancestors(source))
 
-    # Loop
-    builder: typing.Set[TermId] = set()
-    while buffer:
-        current = buffer.popleft()
-        for parent in g.get_parents(current):
-            buffer.append(parent)
-        builder.add(current)
     return frozenset(builder)
 
 
 def get_parents(g: typing.Union[GraphAware, OntologyGraph],
                 source: CURIE_OR_TERM_ID,
                 include_source: bool = False) -> typing.FrozenSet[TermId]:
     """
-    Get `TermId`s of the direct parents of the `source` term.
+    Get :class:`TermId`\\ (s). of the direct parents of the `source` term.
 
-    The method raises a `ValueError` if inputs do not meet the requirement described below.
+    The method raises a :class:`ValueError` if inputs do not meet the requirement described below.
 
     :param g: the ontology graph or a graph-aware entity
-    :param source: `TermId` or a term ID curie as a `str (e.g. `HP:1234567`)
-    :param include_source: whether to include the `source` term in the resulting set
-    :return: a `frozenset` with parent `TermId`s
+    :param source: :class:`TermId` or a term ID curie as a :class:`str (e.g. `HP:1234567`)
+    :param include_source:  whether to include the `source` term ID(s) in the results
+    :return: a :class:`frozenset` with parent `TermId`s
     """
     # Check
     g = _check_ontology_graph_is_available(g)
     source = _check_curie_or_term_id(source)
 
     # Init
     builder: typing.Set[TermId] = set()
     if include_source:
         builder.add(source)
 
-    # Loop
-    for parent in g.get_parents(source):
-        builder.add(parent)
+    builder.update(g.get_parents(source))
+
     return frozenset(builder)
 
 
 def get_descendants(g: typing.Union[GraphAware, OntologyGraph],
                     source: CURIE_OR_TERM_ID,
                     include_source: bool = False) -> typing.FrozenSet[TermId]:
     """
     Get all descendants `TermId`s of the `source` term (children, grandchildren, great-grandchildren etc.)..
 
     The method raises a `ValueError` if inputs do not meet the requirement described below.
 
     :param g: the ontology graph or a graph-aware entity
     :param source: `TermId` or a term ID curie as a `str (e.g. `HP:1234567`)
-    :param include_source: whether to include the `source` term in the resulting set
-    :return: a `frozenset` with descendants `TermId`s
+    :param include_source:  whether to include the `source` term ID(s) in the results
+    :return: a :class:`frozenset` with descendants `TermId`s
     """
     # Check
     g = _check_ontology_graph_is_available(g)
     source = _check_curie_or_term_id(source)
 
     # Init
-    buffer: typing.Deque[TermId] = deque()
+    builder: set[TermId] = set()
     if include_source:
-        buffer.append(source)
-    else:
-        for child in g.get_children(source):
-            buffer.append(child)
+        builder.add(source)
+
+    builder.update(g.get_descendants(source))
 
-    # Loop
-    builder: typing.Set[TermId] = set()
-    while buffer:
-        current = buffer.popleft()
-        for child in g.get_children(current):
-            buffer.append(child)
-        builder.add(current)
     return frozenset(builder)
 
 
 def get_descendents(g: typing.Union[GraphAware, OntologyGraph],
                     source: CURIE_OR_TERM_ID,
                     include_source: bool = False) -> typing.FrozenSet[TermId]:
     """
     Get all descendants `TermId`s of the `source` term (children, grandchildren, great-grandchildren etc.)..
 
     The method raises a `ValueError` if inputs do not meet the requirement described below.
 
     :param g: the ontology graph or a graph-aware entity
     :param source: `TermId` or a term ID curie as a `str (e.g. `HP:1234567`)
-    :param include_source: whether to include the `source` term in the resulting set
-    :return: a `frozenset` with descendants `TermId`s
+    :param include_source: whether to include the `source` term in the results
+    :return: a :class:`frozenset` with descendants `TermId`s
     """
     # TODO[v0.3.0] - remove the deprecated method
     warn('The method is deprecated due to typo and will be removed in v0.3.0. Use get_descendants() instead',
          DeprecationWarning, stacklevel=2)
     return get_descendants(g, source, include_source)
 
 
@@ -129,29 +111,27 @@
     """
     Get `TermId`s of the direct children of the `source` term.
 
     The method raises a `ValueError` if inputs do not meet the requirement described below.
 
     :param g: the ontology graph or a graph-aware entity
     :param source: `TermId` or a CURIE `str` (e.g. `HP:1234567`)
-    :param include_source: whether to include the `source` term in the resulting set
-    :return: a `frozenset` with children `TermId`s
+    :param include_source: whether to include the `source` term in the results
+    :return: an iterable with child `TermId`s
     """
     # Check
     g = _check_ontology_graph_is_available(g)
     source = _check_curie_or_term_id(source)
 
-    # Init
-    builder: typing.Set[TermId] = set()
+    builder: set[TermId] = set()
     if include_source:
         builder.add(source)
 
-    # Loop
-    for child in g.get_children(source):
-        builder.add(child)
+    builder.update(g.get_children(source))
+
     return frozenset(builder)
 
 
 def exists_path(g: typing.Union[GraphAware, OntologyGraph],
                 source: CURIE_OR_TERM_ID,
                 destination: CURIE_OR_TERM_ID) -> bool:
     """
```

### Comparing `hpo-toolkit-0.1.4/src/hpotk/annotations/_base.py` & `hpo-toolkit-0.1.5/src/hpotk/annotations/_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import abc
 import enum
 import typing
 
 from hpotk.model import Identified, Named, Versioned, TermId
 from hpotk.model import CURIE_OR_TERM_ID
+from ._api import ObservableAnnotation, AnnotatedItem, AnnotatedItemContainer
 
 
 class Ratio(metaclass=abc.ABCMeta):
 
     @staticmethod
     def create(numerator: int, denominator: int):
         return SimpleRatio(numerator, denominator)
@@ -90,19 +91,19 @@
         return f"SimpleRatio(" \
                f"numerator={self._numerator}, " \
                f"denominator={self._denominator})"
 
 
 class EvidenceCode(enum.Enum):
     """Inferred from electronic evidence."""
-    IEA = 0
+    IEA = enum.auto()
     """Traceable author statement."""
-    TAS = 1
+    TAS = enum.auto()
     """Published clinical study."""
-    PCS = 2
+    PCS = enum.auto()
 
     @staticmethod
     def parse(value: str):
         """
         Parse evidence code from `str` value.
 
         :param value: a str with the evidence code.
@@ -116,22 +117,22 @@
         elif value == 'PCS':
             return EvidenceCode.PCS
         else:
             return None
 
 
 class Sex(enum.Enum):
-    UNKNOWN = 0
-    MALE = 1
-    FEMALE = 2
+    UNKNOWN = enum.auto()
+    MALE = enum.auto()
+    FEMALE = enum.auto()
 
     @staticmethod
     def parse(value: str):
         """
-        Parse :class:`Sex` from `str` value.
+        Parse :class:`Sex` from :class:`str` value.
 
         :param value: a `str` with the sex code.
         :return: the parsed enum member or `None` if `value` is not valid :class:`Sex` value.
         """
         value = value.upper()
         if value == 'MALE':
             return Sex.MALE
@@ -177,26 +178,30 @@
 
     def __repr__(self):
         return f"AnnotationReference(" \
                f"identifier={repr(self._identifier)}, " \
                f"evidence_code={repr(self._evidence_code)})"
 
 
-class HpoDiseaseAnnotation(Identified, metaclass=abc.ABCMeta):
+class HpoDiseaseAnnotation(ObservableAnnotation, metaclass=abc.ABCMeta):
 
     @property
     @abc.abstractmethod
     def ratio(self) -> Ratio:
         """
         :return: ratio representing a total number of the cohort members who displayed presence
-        of the phenotypic feature represented by `HpoDiseaseAnnotation` at some point in their life.
+                 of the phenotypic feature represented by :class:`HpoDiseaseAnnotation` at some point in their life.
         """
         pass
 
     @property
+    def is_present(self) -> bool:
+        return not self.ratio.is_zero()
+
+    @property
     @abc.abstractmethod
     def references(self) -> typing.List[AnnotationReference]:
         """
         :return: a list of `AnnotationReference`s that support presence/absence of the disease annotation
         """
         pass
 
@@ -204,93 +209,52 @@
     @abc.abstractmethod
     def modifiers(self) -> typing.List[TermId]:
         """
         :return: a list of disease annotation modifiers
         """
         pass
 
-    def is_absent(self) -> bool:
-        return self.ratio.is_zero()
-
-    def is_present(self) -> bool:
-        return not self.is_absent()
-
     def __str__(self):
         return f"HpoDiseaseAnnotation(" \
                f"identifier={self.identifier}, " \
                f"ratio={self.ratio}, " \
                f"references={self.references}, " \
                f"modifiers={self.modifiers})"
 
 
-class HpoDisease(Identified, Named, metaclass=abc.ABCMeta):
-
-    @property
-    @abc.abstractmethod
-    def annotations(self) -> typing.Collection[HpoDiseaseAnnotation]:
-        """
-        :return a collection of all (present and absent) disease annotations.
-        """
-        pass
+class HpoDisease(AnnotatedItem[HpoDiseaseAnnotation], Identified, Named, metaclass=abc.ABCMeta):
 
     @property
     @abc.abstractmethod
     def modes_of_inheritance(self) -> typing.Collection[TermId]:
         """
         :return: a collection of modes of inheritance associated with the disease.
         """
         pass
 
-    def present_annotations(self) -> typing.Iterable[HpoDiseaseAnnotation]:
-        """
-        :return: an iterable over present disease features.
-        """
-        return filter(lambda a: a.is_present(), self.annotations)
-
-    def absent_annotations(self) -> typing.Iterable[HpoDiseaseAnnotation]:
-        """
-        :return: an iterable over absent/excluded disease features.
-        """
-        return filter(lambda a: a.is_absent(), self.annotations)
-
     def __str__(self):
         return f"HpoDisease(" \
                f"identifier={self.identifier}, " \
                f"name={self.name}, " \
                f"n_annotations={len(self.annotations)})"
 
 
-class HpoDiseases(Versioned, typing.Sized, metaclass=abc.ABCMeta):
+class HpoDiseases(AnnotatedItemContainer[HpoDiseaseAnnotation], metaclass=abc.ABCMeta):
     """
     A container for a set of :class:`HpoDisease`s that allows iteration over all diseases,
     knows about the number of diseases in the container, and supports retrieval of the disease by its identifier.
     """
 
-    @property
-    @abc.abstractmethod
-    def diseases(self) -> typing.Iterable[HpoDisease]:
-        """
-        :return: an iterable over :class:`HpoDisease`s of the container.
-        """
-        pass
-
     @abc.abstractmethod
     def __getitem__(self, disease_id: CURIE_OR_TERM_ID) -> typing.Optional[HpoDisease]:
         """
         Get :class:`HpoDisease` based on given `disease_id` or `None` if the disease for the identifier is not present
         in the container.
 
         :param disease_id: a `str` or :class:`TermId` of the disease
         :return: :class:`HpoDisease` or `None`
         """
         pass
 
-    @property
-    def disease_ids(self) -> typing.Iterable[TermId]:
-        """
-        :return: an iterable over all disease IDs.
-        """
-        return map(lambda d: d.identifier, self.diseases)
-
     def __str__(self):
         return f"HpoDiseases(n_diseases={len(self)}, " \
                f"version={self.version})"
```

### Comparing `hpo-toolkit-0.1.4/src/hpotk/annotations/_simple.py` & `hpo-toolkit-0.1.5/src/hpotk/annotations/_simple.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import typing
+import warnings
 
 from hpotk.model import TermId, CURIE_OR_TERM_ID
+from ._api import ANNOTATED_ITEM
 from ._base import AnnotationReference, Ratio
 from ._base import HpoDisease, HpoDiseaseAnnotation, HpoDiseases
 
 
 class SimpleHpoDiseaseAnnotation(HpoDiseaseAnnotation):
 
     def __init__(self, identifier: TermId,
@@ -59,22 +61,41 @@
     @property
     def modes_of_inheritance(self) -> typing.Collection[TermId]:
         return self._modes_of_inheritance
 
 
 class SimpleHpoDiseases(HpoDiseases):
 
+    def __iter__(self) -> typing.Iterator[HpoDiseaseAnnotation]:
+        return iter(self._diseases.values())
+
     def __init__(self, diseases: typing.Iterable[HpoDisease], version: str = None):
         self._diseases = {d.identifier: d for d in diseases}
         self._version = version
 
     @property
+    def items(self) -> typing.Collection[ANNOTATED_ITEM]:
+        return self._diseases.values()
+
+    @property
     def diseases(self) -> typing.Collection[HpoDisease]:
+        # REMOVE(v1.0.0)
+        warnings.warn('The `diseases` property has been deprecated and will be removed in `v1.0.0`. '
+                      'Use `items()` instead',
+                      category=DeprecationWarning, stacklevel=2)
         return self._diseases.values()
 
+    @property
+    def disease_ids(self):
+        # REMOVE(v1.0.0)
+        warnings.warn(f'`disease_ids` property has been deprecated and will be removed in v1.0.0. '
+                      f'Iterate over `item_ids()` instead.',
+                      DeprecationWarning, stacklevel=2)
+        return list(self.item_ids())
+
     def __getitem__(self, item: CURIE_OR_TERM_ID) -> typing.Optional[HpoDisease]:
         if isinstance(item, TermId):
             pass
         elif isinstance(item, str):
             item = TermId.from_curie(item)
         else:
             raise ValueError(f'Expected a `str` or `TermId` but got {type(item)}')
```

### Comparing `hpo-toolkit-0.1.4/src/hpotk/annotations/load/hpoa/_impl.py` & `hpo-toolkit-0.1.5/src/hpotk/annotations/load/hpoa/_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 import typing
 from collections import defaultdict, namedtuple
 
 from hpotk.annotations import HpoDiseases, EvidenceCode, AnnotationReference, Sex, Ratio
 from hpotk.annotations import SimpleHpoDiseaseAnnotation, SimpleHpoDisease, SimpleHpoDiseases
 from hpotk.model import TermId
 from hpotk.ontology import MinimalOntology
-from hpotk.util import open_text_io_handle
+from hpotk.util import open_text_io_handle_for_reading
 from hpotk.constants.hpo.frequency import parse_hpo_frequency
 from hpotk.annotations.load._api import HpoDiseaseLoader
 
 HpoAnnotationLine = namedtuple('HpoAnnotationLine',
                                field_names=[
                                    'disease_id', 'disease_name', 'is_negated',
                                    'phenotype_term_id',
                                    'annotation_references', 'onset', 'frequency',
                                    'sex', 'modifiers', 'aspect', 'curators']
                                )
 
-HPOA_VERSION_PATTERN = re.compile(r'^#date: (?P<version>[\w-]+)\w?$')
+HPOA_VERSION_PATTERN = re.compile(r'^#(date|version): (?P<version>[\w-]+)\w?$')
 HPO_PATTERN = re.compile(r'^HP:\d{7}$')
 RATIO_PATTERN = re.compile(r'^(?P<numerator>\d+)/(?P<denominator>\d+)$')
 PERCENTAGE_PATTERN = re.compile(r'^(?P<value>\d+\.?(\d+)?)%$')
 
 
 class SimpleHpoaDiseaseLoader(HpoDiseaseLoader):
     """
@@ -39,15 +39,15 @@
         self._cohort_size = cohort_size
         self._salvage_negated_frequencies = salvage_negated_frequencies
 
     def load(self, file: typing.Union[typing.IO, str]) -> HpoDiseases:
         data = defaultdict(list)
         version = None
         expecting_to_see_header_line = True
-        with open_text_io_handle(file) as fh:
+        with open_text_io_handle_for_reading(file) as fh:
             for line in fh:
                 if expecting_to_see_header_line:
                     if line.startswith('#'):
                         # header
                         if line.startswith('#DatabaseID'):
                             # The older HPOA format
                             expecting_to_see_header_line = False
```

### Comparing `hpo-toolkit-0.1.4/src/hpotk/constants/hpo/frequency.py` & `hpo-toolkit-0.1.5/src/hpotk/constants/hpo/frequency.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.4/src/hpotk/constants/hpo/inheritance.py` & `hpo-toolkit-0.1.5/src/hpotk/constants/hpo/inheritance.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.4/src/hpotk/constants/hpo/onset.py` & `hpo-toolkit-0.1.5/src/hpotk/constants/hpo/onset.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.4/src/hpotk/constants/hpo/organ_system.py` & `hpo-toolkit-0.1.5/src/hpotk/constants/hpo/organ_system.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.4/src/hpotk/graph/_api.py` & `hpo-toolkit-0.1.5/src/hpotk/graph/_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,61 @@
 import abc
-
 import typing
 
 from hpotk.model import TermId
 
+# TODO - enforce presence of the natural ordering?
+# Note, the NODE must also have natural ordering.
 NODE = typing.TypeVar('NODE', bound=TermId)
 # Term ID that is added as an artificial root if >1 root candidates are found in the ontology graph.
 OWL_THING = TermId.from_curie("owl:Thing")
 
 
 class OntologyGraph(typing.Generic[NODE], metaclass=abc.ABCMeta):
     """
     A simple graph with one node type and one edge type.
 
-    The graph is generic over a node type which must extend `hpotk.base.model.TermId`. The graph must not be empty
+    The graph is generic over a node type which must extend :class:`TermId`.
+    The graph must not be empty, it must consist of at least one node.
     """
 
     @property
     @abc.abstractmethod
     def root(self) -> NODE:
+        """
+        Get the root node of the ontology graph.
+        """
+        pass
+
+    @abc.abstractmethod
+    def get_children(self, source: NODE) -> typing.Iterable[NODE]:
+        """
+        Get an iterable with the children of the `source` node.
+        """
+        pass
+
+    @abc.abstractmethod
+    def get_descendants(self, source: NODE) -> typing.Iterable[NODE]:
+        """
+        Get an iterable with the descendants of the `source` node.
+        """
         pass
 
     @abc.abstractmethod
-    def get_children(self, source: NODE) -> typing.Iterator[NODE]:
+    def get_parents(self, source: NODE) -> typing.Iterable[NODE]:
+        """
+        Get an iterable with the parents of the `source` node.
+        """
         pass
 
     @abc.abstractmethod
-    def get_parents(self, source: NODE) -> typing.Iterator[NODE]:
+    def get_ancestors(self, source: NODE) -> typing.Iterable[NODE]:
+        """
+        Get an iterable with the ancestors of the `source` node.
+        """
         pass
 
     @abc.abstractmethod
     def __contains__(self, item: NODE) -> bool:
         pass
 
     @abc.abstractmethod
```

### Comparing `hpo-toolkit-0.1.4/src/hpotk/graph/csr/_csr.py` & `hpo-toolkit-0.1.5/src/hpotk/graph/csr/_csr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 import abc
 import typing
+import warnings
 
 import numpy as np
 from collections import deque
 
 
 class ShapedMixin(metaclass=abc.ABCMeta):
 
     @property
     @abc.abstractmethod
     def shape(self):
         pass
 
 
 class CsrMatrixBuilder(ShapedMixin):
+    """
+    The builder has been deprecated due to poor performance and will be removed in v1.0.0.
+    """
 
     def __init__(self, shape: typing.Tuple[int, int]):
         _check_shape(shape)
         self._shape = shape
         self._row = np.zeros(shape=(shape[0] + 1,), dtype=int)
         self._col = deque([])
         self._data = deque([])
+        warnings.warn('CsrMatrixBuilder has been deprecated and will be removed in v1.0.0',
+                      DeprecationWarning, stacklevel=2)
 
     def __setitem__(self, key, value):
         if isinstance(key, tuple):
             if len(key) == 2:
                 qrow, qcol = key
                 _check_bounds(qrow, qcol, self._shape)
 
@@ -149,15 +155,15 @@
             else:
                 raise ValueError(f'Requesting {len(item)} dimensions but only 2D indexing is supported')
         else:
             raise IndexError(f'Unknown index type {type(item)}')
 
     def col_indices_of_val(self, row: int, query):
         """
-        Return indices of colums with matching query value in a given row.
+        Return indices of columns with matching query value in a given row.
 
         Raises IndexError if `row` is out of bounds.
         """
         if not (isinstance(row, int) and 0 <= row < self._shape[0]):
             raise IndexError(f'row must be an int in range [0, {self.shape[0]}) but was {row}')
 
         start_row, end_row = self._row[row: row + 2]
```

### Comparing `hpo-toolkit-0.1.4/src/hpotk/graph/csr/test__csr.py` & `hpo-toolkit-0.1.5/src/hpotk/graph/csr/test__csr.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.4/src/hpotk/model/_base.py` & `hpo-toolkit-0.1.5/src/hpotk/model/_base.py`

 * *Files 24% similar despite different names*

```diff
@@ -40,7 +40,43 @@
     @property
     @abc.abstractmethod
     def version(self) -> typing.Optional[str]:
         """
         :return: version `str` or `None` if the version is not available.
         """
         pass
+
+
+class MetadataAware(metaclass=abc.ABCMeta):
+    """
+    Base class for entities that have metadata.
+    """
+
+    @property
+    @abc.abstractmethod
+    def metadata(self) -> typing.MutableMapping[str, str]:
+        """
+        :return: a mapping with entity metadata.
+        """
+        pass
+
+    def metadata_to_str(self) -> str:
+        """
+        Dump the metadata to a single string.
+        """
+        forbidden = {';', '='}
+        for k, v in self.metadata.items():
+            if any([token in k or token in v for token in forbidden]):
+                raise ValueError(f'Metadata contains forbidden characters {forbidden}')
+
+        return ';'.join([f'{k}={v}' for k, v in self.metadata.items()])
+
+    @staticmethod
+    def metadata_from_str(value: str) -> typing.Mapping[str, str]:
+        """
+        Load the metadata from `str` created by `metadata_to_str`.
+        """
+        data = {}
+        for item in value.split(';'):
+            k, v = item.split('=')
+            data[k] = v
+        return data
```

### Comparing `hpo-toolkit-0.1.4/src/hpotk/model/_term.py` & `hpo-toolkit-0.1.5/src/hpotk/model/_term.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.4/src/hpotk/model/_term_id.py` & `hpo-toolkit-0.1.5/src/hpotk/model/_term_id.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.4/src/hpotk/ontology/_api.py` & `hpo-toolkit-0.1.5/src/hpotk/ontology/_api.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.4/src/hpotk/ontology/_default.py` & `hpo-toolkit-0.1.5/src/hpotk/ontology/_default.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.4/src/hpotk/ontology/load/obographs/_factory.py` & `hpo-toolkit-0.1.5/src/hpotk/ontology/load/obographs/_factory.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.4/src/hpotk/ontology/load/obographs/_load.py` & `hpo-toolkit-0.1.5/src/hpotk/ontology/load/obographs/_load.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import re
 import json
 import typing
 import logging
 
 from hpotk.model import TermId, MinimalTerm, Term
 from hpotk.graph import OntologyGraph
-from hpotk.graph import GraphFactory, CsrGraphFactory, OWL_THING
+from hpotk.graph import GraphFactory, IncrementalCsrGraphFactory, OWL_THING
 from hpotk.ontology import MinimalOntology, Ontology, create_ontology, create_minimal_ontology
-from hpotk.util import open_text_io_handle
+from hpotk.util import open_text_io_handle_for_reading
 
 from ._model import create_node, create_edge
 from ._model import Node, Edge, NodeType
 from ._factory import MinimalTermFactory, TermFactory, ObographsTermFactory, MINIMAL_TERM
 
 logger = logging.getLogger(__name__)
 
 # TODO - verify PURL works for other ontologies than HPO
 # A pattern to match an obolibrary PURL. The PURL should is expected to have 3 parts: `prefix`, `id`, and `curie`
 # The `curie` is `prefix` + '_' + `id`.
 PURL_PATTERN = re.compile(r'http://purl\.obolibrary\.org/obo/(?P<curie>(?P<prefix>\w+)_(?P<id>\d{7}))')
 DATE_PATTERN = re.compile(r'.*/(?P<date>\d{4}-\d{2}-\d{2})/.*')
 
+
 def load_minimal_ontology(file: typing.Union[typing.IO, str],
                           term_factory: ObographsTermFactory[MinimalTerm] = MinimalTermFactory(),
-                          graph_factory: GraphFactory = CsrGraphFactory()) -> MinimalOntology:
+                          graph_factory: GraphFactory = IncrementalCsrGraphFactory()) -> MinimalOntology:
     return _load_impl(file, term_factory, graph_factory, create_minimal_ontology)
 
 
 def load_ontology(file: typing.Union[typing.IO, str],
                   term_factory: ObographsTermFactory[Term] = TermFactory(),
-                  graph_factory: GraphFactory = CsrGraphFactory()) -> Ontology:
+                  graph_factory: GraphFactory = IncrementalCsrGraphFactory()) -> Ontology:
     return _load_impl(file, term_factory, graph_factory, create_ontology)
 
 
 def _load_impl(file: typing.Union[typing.IO, str],
                term_factory: ObographsTermFactory[MinimalTerm],
                graph_factory: GraphFactory,
                ontology_creator):
@@ -49,15 +50,15 @@
         pass
     version = extract_ontology_version(hpo['meta'])
     logger.debug(f"Assembling the ontology")
     return ontology_creator(graph, terms, version)
 
 
 def get_hpo_graph(file: typing.Union[typing.IO, str]):
-    with open_text_io_handle(file) as fh:
+    with open_text_io_handle_for_reading(file) as fh:
         document = json.load(fh)
     if not isinstance(document, dict):
         raise ValueError(f'The JSON document should have been a dict but was {type(document)}')
     if 'graphs' not in document:
         raise ValueError(f'Did not find the `graphs` attribute in the JSON document')
     graphs = document['graphs']
     if not isinstance(graphs, typing.Sequence):
```

### Comparing `hpo-toolkit-0.1.4/src/hpotk/ontology/load/obographs/_model.py` & `hpo-toolkit-0.1.5/src/hpotk/ontology/load/obographs/_model.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.4/src/hpotk/ontology/load/obographs/test_load.py` & `hpo-toolkit-0.1.5/src/hpotk/ontology/load/obographs/test_load.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.4/src/hpotk/validate/_hpo.py` & `hpo-toolkit-0.1.5/src/hpotk/validate/_hpo.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 from ._model import ValidationResult, ValidationResults, ValidationLevel, RuleValidator
 
 
 class BaseOntologyRuleValidator(RuleValidator, metaclass=abc.ABCMeta):
 
     def __init__(self, ontology: MinimalOntology):
+        if not isinstance(ontology, MinimalOntology):
+            raise ValueError(f'ontology must be an instance of hpotk.ontology.MinimalOntology '
+                             f'but it was an instance of {type(ontology)}')
         self._ontology = ontology
 
     def _primary_term_id(self, identifier: TermId) -> typing.Optional[TermId]:
         """
         Map the provided `identifier` into the primary term ID in case the `identifier` is obsolete.
         """
         current_term = self._ontology.get_term(identifier)
@@ -28,16 +31,16 @@
 
     The validator replaces obsolete term IDs with the current term IDs before performing the validation.
     """
 
     def __init__(self, ontology: MinimalOntology):
         super().__init__(ontology)
 
-    def validate(self, items: typing.Sequence[Identified]) -> ValidationResults:
-        term_ids = {self._primary_term_id(term.identifier) for term in items}
+    def validate(self, items: typing.Sequence[typing.Union[Identified, TermId]]) -> ValidationResults:
+        term_ids = {self._primary_term_id(self.extract_term_id(item)) for item in items}
         results = []
         for term_id in term_ids:
             for ancestor in get_ancestors(self._ontology, source=term_id, include_source=False):
                 if ancestor in term_ids:
                     current_term = self._ontology.get_term(term_id)
                     ancestor_term = self._ontology.get_term(ancestor)
                     results.append(
@@ -58,47 +61,49 @@
 
     The validator replaces obsolete term IDs with the current term IDs before performing the validation.
     """
 
     def __init__(self, ontology: MinimalOntology):
         super().__init__(ontology)
 
-    def validate(self, items: typing.Sequence[Identified]) -> ValidationResults:
+    def validate(self, items: typing.Sequence[typing.Union[Identified, TermId]]) -> ValidationResults:
         results = []
-        for term in items:
-            term_id = self._primary_term_id(term.identifier)
+        for item in items:
+            term_id = self.extract_term_id(item)
+            term_id = self._primary_term_id(term_id)
             ancestors = get_ancestors(self._ontology, source=term_id, include_source=False)
             if PHENOTYPIC_ABNORMALITY not in ancestors:
-                term = self._ontology.get_term(term_id)
+                item = self._ontology.get_term(term_id)
                 results.append(
                     ValidationResult(
                         level=ValidationLevel.ERROR,
                         category='phenotypic_abnormality_descendant',
-                        message=f'{term.name} [{term.identifier.value}] '
+                        message=f'{item.name} [{item.identifier.value}] '
                                 f'is not a descendant of Phenotypic abnormality [{PHENOTYPIC_ABNORMALITY.value}]'
                     )
                 )
 
         return ValidationResults(results)
 
 
 class ObsoleteTermIdsValidator(BaseOntologyRuleValidator):
 
     def __init__(self, ontology: MinimalOntology):
         super().__init__(ontology)
 
-    def validate(self, items: typing.Sequence[Identified]) -> ValidationResults:
+    def validate(self, items: typing.Sequence[typing.Union[Identified, TermId]]) -> ValidationResults:
         results = []
-        for term in items:
-            current_id = self._primary_term_id(term.identifier)
-            if current_id != term.identifier:
-                current_term = self._ontology.get_term(term.identifier)
+        for item in items:
+            term_id = self.extract_term_id(item)
+            current_id = self._primary_term_id(term_id)
+            if current_id != term_id:
+                current_term = self._ontology.get_term(current_id)
                 results.append(
                     ValidationResult(
                         level=ValidationLevel.WARNING,
                         category='obsolete_term_id_is_used',
-                        message=f'Using the obsolete {term.identifier.value} instead of {current_id.value} '
+                        message=f'Using the obsolete {term_id} instead of {current_id.value} '
                                 f'for {current_term.name}'
                     )
                 )
 
         return ValidationResults(results)
```

### Comparing `hpo-toolkit-0.1.4/src/hpotk/validate/_model.py` & `hpo-toolkit-0.1.5/src/hpotk/validate/_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing
 import abc
 import enum
 
 from collections import namedtuple
 
-from hpotk.model import Identified
+from hpotk.model import Identified, TermId
 
 
 class ValidationLevel(enum.Enum):
     WARNING = 1
     ERROR = 2
 
 
@@ -35,32 +35,46 @@
 
     def __repr__(self) -> str:
         return f"ValidationResults(results={[self._results]})"
 
 
 class RuleValidator(metaclass=abc.ABCMeta):
     """
-    `RuleValidator` checks if a sequence of `Identified` items meet the validation requirements.
-    The issues are returned as `ValidationResults`.
+    `RuleValidator` checks if a sequence of :class:`Identified` or :class:`TermId` instances meet
+    the validation requirements.
+
+    The validators can check each item individually or as a collection, for instance,
+    to discover violation of the annotation propagation rule, etc.
+
+    The issues are returned as :class:`ValidationResults`.
     """
 
     @abc.abstractmethod
-    def validate(self, items: typing.Sequence[Identified]) -> ValidationResults:
+    def validate(self, items: typing.Sequence[typing.Union[Identified, TermId]]) -> ValidationResults:
         pass
 
+    @staticmethod
+    def extract_term_id(item: typing.Union[Identified, TermId]) -> TermId:
+        if isinstance(item, Identified):
+            return item.identifier
+        elif isinstance(item, TermId):
+            return item
+        else:
+            raise ValueError(f'Item {item} of type {type(item)} is not a TermId nor extends Identified')
+
 
 class ValidationRunner:
     """
     The runner applies a sequence of `RuleValidator`s on items and returns the results as `ValidationResults`.
     """
 
     def __init__(self, validators: typing.Sequence[RuleValidator]):
         self._validators = validators
 
-    def validate_all(self, items: typing.Sequence[Identified]) -> ValidationResults:
+    def validate_all(self, items: typing.Sequence[typing.Union[Identified, TermId]]) -> ValidationResults:
         overall = []
         for validator in self._validators:
             results = validator.validate(items)
             for result in results.results:
                 overall.append(result)
 
         return ValidationResults(overall)
```

### Comparing `hpo-toolkit-0.1.4/tests/test_disease.py` & `hpo-toolkit-0.1.5/tests/test_disease.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.4/tests/test_term.py` & `hpo-toolkit-0.1.5/tests/test_term.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.4/tests/test_term_id.py` & `hpo-toolkit-0.1.5/tests/test_term_id.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.4/tests/test_validate.py` & `hpo-toolkit-0.1.5/tests/test_validate.py`

 * *Files identical despite different names*


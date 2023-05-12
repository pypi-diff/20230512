# Comparing `tmp/pyreason-1.4.1.tar.gz` & `tmp/pyreason-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreason-1.4.1.tar", last modified: Thu May 11 15:52:00 2023, max compression
+gzip compressed data, was "pyreason-1.4.2.tar", last modified: Fri May 12 16:47:53 2023, max compression
```

## Comparing `pyreason-1.4.1.tar` & `pyreason-1.4.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.485568 pyreason-1.4.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-05-11 15:51:46.000000 pyreason-1.4.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-11 15:51:46.000000 pyreason-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-11 15:52:00.485568 pyreason-1.4.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-05-11 15:51:46.000000 pyreason-1.4.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       85 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.481568 pyreason-1.4.1/pyreason/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/.cache_status.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.481568 pyreason-1.4.1/pyreason/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.481568 pyreason-1.4.1/pyreason/examples/hello-world/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/examples/hello-world/facts.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/examples/hello-world/friends.graphml
--rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/examples/hello-world/ipl.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/examples/hello-world/labels.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/examples/hello-world/rules.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    27250 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/pyreason.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.481568 pyreason-1.4.1/pyreason/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.481568 pyreason-1.4.1/pyreason/scripts/annotation_functions/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/annotation_functions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/annotation_functions/annotation_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.481568 pyreason-1.4.1/pyreason/scripts/components/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/components/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/components/label.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/components/world.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/diffuse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.481568 pyreason-1.4.1/pyreason/scripts/facts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/facts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/facts/fact_edge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/facts/fact_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.485568 pyreason-1.4.1/pyreason/scripts/interpretation/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/interpretation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    65031 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/interpretation/interpretation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.485568 pyreason-1.4.1/pyreason/scripts/interval/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/interval/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/interval/interval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.485568 pyreason-1.4.1/pyreason/scripts/numba_wrapper/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/numba_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.485568 pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6220 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5992 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/label_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10162 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/world_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.485568 pyreason-1.4.1/pyreason/scripts/program/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/program/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1793 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/program/program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.485568 pyreason-1.4.1/pyreason/scripts/rules/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1119 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/rules/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.485568 pyreason-1.4.1/pyreason/scripts/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4564 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/utils/filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4217 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/utils/graphml_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/utils/output.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/utils/plotter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/utils/visuals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-05-11 15:51:46.000000 pyreason-1.4.1/pyreason/scripts/utils/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:52:00.481568 pyreason-1.4.1/pyreason.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-11 15:52:00.000000 pyreason-1.4.1/pyreason.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-11 15:52:00.000000 pyreason-1.4.1/pyreason.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:52:00.000000 pyreason-1.4.1/pyreason.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 15:52:00.000000 pyreason-1.4.1/pyreason.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 15:52:00.000000 pyreason-1.4.1/pyreason.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 15:52:00.485568 pyreason-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-11 15:51:46.000000 pyreason-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.772425 pyreason-1.4.2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-05-12 16:47:42.000000 pyreason-1.4.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-12 16:47:42.000000 pyreason-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-12 16:47:53.772425 pyreason-1.4.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-05-12 16:47:42.000000 pyreason-1.4.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       85 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.768425 pyreason-1.4.2/pyreason/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/.cache_status.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.768425 pyreason-1.4.2/pyreason/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.768425 pyreason-1.4.2/pyreason/examples/hello-world/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/examples/hello-world/facts.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/examples/hello-world/friends.graphml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/examples/hello-world/ipl.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/examples/hello-world/labels.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/examples/hello-world/rules.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27566 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/pyreason.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.768425 pyreason-1.4.2/pyreason/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.772425 pyreason-1.4.2/pyreason/scripts/annotation_functions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/annotation_functions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/annotation_functions/annotation_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.772425 pyreason-1.4.2/pyreason/scripts/components/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/components/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/components/label.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/components/world.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/diffuse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.772425 pyreason-1.4.2/pyreason/scripts/facts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/facts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/facts/fact_edge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/facts/fact_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.772425 pyreason-1.4.2/pyreason/scripts/interpretation/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/interpretation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    65031 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/interpretation/interpretation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.772425 pyreason-1.4.2/pyreason/scripts/interval/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/interval/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/interval/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.772425 pyreason-1.4.2/pyreason/scripts/numba_wrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/numba_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.772425 pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6220 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5992 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/label_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10162 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/world_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.772425 pyreason-1.4.2/pyreason/scripts/program/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/program/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1793 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/program/program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.772425 pyreason-1.4.2/pyreason/scripts/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1119 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/rules/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.772425 pyreason-1.4.2/pyreason/scripts/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4564 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/utils/filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4217 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/utils/graphml_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/utils/output.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/utils/plotter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/utils/visuals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-05-12 16:47:42.000000 pyreason-1.4.2/pyreason/scripts/utils/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:47:53.768425 pyreason-1.4.2/pyreason.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-12 16:47:53.000000 pyreason-1.4.2/pyreason.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-12 16:47:53.000000 pyreason-1.4.2/pyreason.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 16:47:53.000000 pyreason-1.4.2/pyreason.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 16:47:53.000000 pyreason-1.4.2/pyreason.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 16:47:53.000000 pyreason-1.4.2/pyreason.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 16:47:53.772425 pyreason-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-12 16:47:42.000000 pyreason-1.4.2/setup.py
```

### Comparing `pyreason-1.4.1/LICENSE.md` & `pyreason-1.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/PKG-INFO` & `pyreason-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.4.1
+Version: 1.4.2
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.4.1/README.md` & `pyreason-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/__init__.py` & `pyreason-1.4.2/pyreason/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/examples/hello-world/facts.yaml` & `pyreason-1.4.2/pyreason/examples/hello-world/facts.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/examples/hello-world/friends.graphml` & `pyreason-1.4.2/pyreason/examples/hello-world/friends.graphml`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/examples/hello-world/rules.yaml` & `pyreason-1.4.2/pyreason/examples/hello-world/rules.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/pyreason.py` & `pyreason-1.4.2/pyreason/pyreason.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,14 +302,25 @@
 __timestamp = ''
 __program = None
 
 __graphml_parser = GraphmlParser()
 settings = _Settings()
 
 
+def reset():
+    """Resets certain variables to None to be able to do pr.reason() multiple times in a program
+    without memory blowing up
+    """
+    global __node_facts, __edge_facts, __node_labels, __edge_labels
+    __node_facts = None
+    __edge_facts = None
+    __node_labels = None
+    __edge_labels = None
+
+
 # FUNCTIONS
 def load_graph(path: str) -> None:
     """Loads graph from GraphMl file path into program
 
     :param path: Path for the GraphMl file
     """
     global __graph, __graphml_parser, __non_fluent_graph_facts_node, __non_fluent_graph_facts_edge, __specific_graph_node_labels, __specific_graph_edge_labels, settings
```

### Comparing `pyreason-1.4.1/pyreason/scripts/annotation_functions/annotation_functions.py` & `pyreason-1.4.2/pyreason/scripts/annotation_functions/annotation_functions.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/scripts/args.py` & `pyreason-1.4.2/pyreason/scripts/args.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/scripts/components/world.py` & `pyreason-1.4.2/pyreason/scripts/components/world.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/scripts/diffuse.py` & `pyreason-1.4.2/pyreason/scripts/diffuse.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/scripts/facts/fact_edge.py` & `pyreason-1.4.2/pyreason/scripts/facts/fact_edge.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/scripts/facts/fact_node.py` & `pyreason-1.4.2/pyreason/scripts/facts/fact_node.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/scripts/interpretation/interpretation.py` & `pyreason-1.4.2/pyreason/scripts/interpretation/interpretation.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/scripts/interval/interval.py` & `pyreason-1.4.2/pyreason/scripts/interval/interval.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py` & `pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py` & `pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/interval_type.py` & `pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/interval_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/label_type.py` & `pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/label_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/rule_type.py` & `pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/rule_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/scripts/numba_wrapper/numba_types/world_type.py` & `pyreason-1.4.2/pyreason/scripts/numba_wrapper/numba_types/world_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/scripts/program/program.py` & `pyreason-1.4.2/pyreason/scripts/program/program.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/scripts/rules/rule.py` & `pyreason-1.4.2/pyreason/scripts/rules/rule.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/scripts/utils/filter.py` & `pyreason-1.4.2/pyreason/scripts/utils/filter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/scripts/utils/graphml_parser.py` & `pyreason-1.4.2/pyreason/scripts/utils/graphml_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/scripts/utils/output.py` & `pyreason-1.4.2/pyreason/scripts/utils/output.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/scripts/utils/plotter.py` & `pyreason-1.4.2/pyreason/scripts/utils/plotter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/scripts/utils/visuals.py` & `pyreason-1.4.2/pyreason/scripts/utils/visuals.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason/scripts/utils/yaml_parser.py` & `pyreason-1.4.2/pyreason/scripts/utils/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/pyreason.egg-info/PKG-INFO` & `pyreason-1.4.2/pyreason.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.4.1
+Version: 1.4.2
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.4.1/pyreason.egg-info/SOURCES.txt` & `pyreason-1.4.2/pyreason.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyreason-1.4.1/setup.py` & `pyreason-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name = 'pyreason',
-    version = '1.4.1',
+    version = '1.4.2',
     author = 'Dyuman Aditya',
     author_email = 'dyuman.aditya@gmail.com',
     description = 'An explainable inference software supporting annotated, real valued, graph based and temporal logic',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/lab-v2/pyreason',
     license = 'BSD 3-clause',
```


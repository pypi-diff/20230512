# Comparing `tmp/baguette_verse-0.9.5.tar.gz` & `tmp/baguette_verse-1.0.0.tar.gz`

## Comparing `baguette_verse-0.9.5.tar` & `baguette_verse-1.0.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0    22934 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/bake.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/metalib.py
--rw-r--r--   0        0        0    19314 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/toast.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/__init__.py
--rw-r--r--   0        0        0    21861 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/rack.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/__init__.py
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/compiler.py
--rw-r--r--   0        0        0     7238 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/cuckoo_api_list.md
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/logger.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/__init__.py
--rw-r--r--   0        0        0    13059 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/build.py
--rw-r--r--   0        0        0    16047 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/colors.py
--rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/config.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/event.py
--rw-r--r--   0        0        0     9276 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/filters.py
--rw-r--r--   0        0        0    32413 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/graph.py
--rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/record.py
--rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/utils.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/__init__.py
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/utils.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/data/__init__.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/data/__proc__.py
--rw-r--r--   0        0        0    13178 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/data/entities.py
--rw-r--r--   0        0        0     7971 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/data/integration.py
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/data/relations.py
--rw-r--r--   0        0        0     9533 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/data/utils.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/execution/__init__.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/execution/__proc__.py
--rw-r--r--   0        0        0     9835 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/execution/entities.py
--rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/execution/integration.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/execution/relations.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/execution/utils.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/filesystem/__init__.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/filesystem/__proc__.py
--rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/filesystem/entities.py
--rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/filesystem/integration.py
--rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/filesystem/relations.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/imports/__init__.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/imports/__proc__.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/imports/entities.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/imports/integration.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/imports/relations.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/network/__init__.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/network/__proc__.py
--rw-r--r--   0        0        0    10216 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/network/entities.py
--rw-r--r--   0        0        0     9921 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/network/integration.py
--rw-r--r--   0        0        0     5198 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/network/relations.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/registry/__init__.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/registry/__proc__.py
--rw-r--r--   0        0        0    10597 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/registry/entities.py
--rw-r--r--   0        0        0    16707 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/registry/integration.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/bakery/source/types/registry/relations.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/croutons/__init__.py
--rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/croutons/extractor.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/croutons/metalib/__init__.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/croutons/metalib/evaluator.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/croutons/metalib/interact.py
--rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/croutons/metalib/utils.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/croutons/source/__init__.py
--rw-r--r--   0        0        0    31599 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/croutons/source/metagraph.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/baguette/croutons/source/utils.py
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/.gitignore
--rw-r--r--   0        0        0    35123 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/LICENSE
--rw-r--r--   0        0        0     8273 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/README.md
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/pyproject.toml
--rw-r--r--   0        0        0    48653 2020-02-02 00:00:00.000000 baguette_verse-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0    25829 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/bake.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/metalib.py
+-rw-r--r--   0        0        0    22402 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/toast.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/__init__.py
+-rw-r--r--   0        0        0    24206 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/rack.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/__init__.py
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/compiler.py
+-rw-r--r--   0        0        0     7238 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/cuckoo_api_list.md
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/logger.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/__init__.py
+-rw-r--r--   0        0        0    12988 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/build.py
+-rw-r--r--   0        0        0    17232 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/colors.py
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/config.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/event.py
+-rw-r--r--   0        0        0     9266 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/filters.py
+-rw-r--r--   0        0        0    33256 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/graph.py
+-rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/record.py
+-rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/utils.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/__init__.py
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/utils.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/data/__init__.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/data/__proc__.py
+-rw-r--r--   0        0        0    13655 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/data/entities.py
+-rw-r--r--   0        0        0     7829 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/data/integration.py
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/data/relations.py
+-rw-r--r--   0        0        0     9533 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/data/utils.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/execution/__init__.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/execution/__proc__.py
+-rw-r--r--   0        0        0    10103 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/execution/entities.py
+-rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/execution/integration.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/execution/relations.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/execution/utils.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/filesystem/__init__.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/filesystem/__proc__.py
+-rw-r--r--   0        0        0     6523 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/filesystem/entities.py
+-rw-r--r--   0        0        0    13693 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/filesystem/integration.py
+-rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/filesystem/relations.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/imports/__init__.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/imports/__proc__.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/imports/entities.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/imports/integration.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/imports/relations.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/network/__init__.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/network/__proc__.py
+-rw-r--r--   0        0        0    10481 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/network/entities.py
+-rw-r--r--   0        0        0     9921 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/network/integration.py
+-rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/network/relations.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/registry/__init__.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/registry/__proc__.py
+-rw-r--r--   0        0        0    11043 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/registry/entities.py
+-rw-r--r--   0        0        0    16621 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/registry/integration.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/bakery/source/types/registry/relations.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/croutons/__init__.py
+-rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/croutons/extractor.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/croutons/metalib/__init__.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/croutons/metalib/evaluator.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/croutons/metalib/interact.py
+-rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/croutons/metalib/utils.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/croutons/source/__init__.py
+-rw-r--r--   0        0        0    30591 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/croutons/source/metagraph.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/baguette/croutons/source/utils.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/.gitignore
+-rw-r--r--   0        0        0    35123 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/LICENSE
+-rw-r--r--   0        0        0     8273 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/README.md
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    48653 2020-02-02 00:00:00.000000 baguette_verse-1.0.0/PKG-INFO
```

### Comparing `baguette_verse-0.9.5/bake.py` & `baguette_verse-1.0.0/bake.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
         import argparse
         from os import environ
         import pathlib
         from typing import Literal, Iterator
         from baguette.bakery.compiler import compile
         from baguette.bakery.source import filters
+        from baguette.bakery.source.colors import Color
         from baguette.rack import BaguetteRack, TimeoutExit
 
         parser = argparse.ArgumentParser(
             description = 'Bakes Cuckoo reports into baguettes (gexf and pyt graphs).',
             add_help = True,
             conflict_handler = 'resolve',
             epilog = """
@@ -97,25 +98,82 @@
                 v = float(arg)
                 if v <= 0 or isnan(v):
                     parser.error("got a negative, null or nan maxtime")
                 return v
             except:
                 parser.error("expected positive float for maxtime, got : '{}'".format(arg))
 
+        def paint_color(c : str) -> Color:
+            if c in dir(Color):
+                color = getattr(Color, c)
+                if not isinstance(color, Color):
+                    parser.error(f"not a valid color name : '{c}'")
+                return color
+            else:
+                # We can match colors in ALLL LANGUAGES!!!!
+                import re
+                color_re = r"([\d\.eE-]+|\d+|0[xX][\daAbBcCdDeEfF]+)"
+                sep_re = r"(?:[ ,;:\|\&]+)"
+                inner_expr = r"(?:" + color_re + sep_re + color_re + sep_re + color_re + r")"
+                fmatch = re.compile(inner_expr).fullmatch(c) or re.compile(r"\(" + inner_expr + r"\)").fullmatch(c) or re.compile(r"\[" + inner_expr + r"\]").fullmatch(c) or re.compile(r"\{" + inner_expr + r"\}").fullmatch(c)
+                if not fmatch:
+                    parser.error(f"could not understand color format : '{c}'")
+                r, g, b = fmatch.groups()
+
+                def is_float(s : str) -> bool:
+                    try:
+                        f = float(s)
+                        if not 0 <= f <= 1:
+                            return False
+                        return True
+                    except:
+                        return False
+                
+                def is_int(s : str) -> bool:
+                    try:
+                        i = int(s)
+                        if not 0 <= i <= 255:
+                            return False
+                        return True
+                    except:
+                        return False
+                
+                def is_hex(s : str) -> bool:
+                    try:
+                        i = int(s, base=16)
+                        if not 0 <= i <= 255:
+                            return False
+                        return True
+                    except:
+                        return False
+                    
+                if all(is_float(x) for x in (r, g, b)):
+                    r, g, b = float(r), float(g), float(b)
+                elif all(is_int(x) for x in (r, g, b)):
+                    r, g, b = int(r), int(g), int(b)
+                elif all(is_hex(x) for x in (r, g, b)):
+                    r, g, b = int(r, 16), int(g, 16), int(b, 16)
+                else:
+                    parser.error(f"could not understand color format : '{c}'")
+
+                return Color(r, g, b)
+
         parser.add_argument("reports", type=PathSorter(reports, "report"), default=None, nargs="*" if "BAGUETTE_REPORTS" in environ else "+", help="Cuckoo report files (.json) to bake baguettes from. Can also be folders containing reports. Defaults to environment variable 'BAGUETTE_REPORTS' if set.")
         parser.add_argument("--baguettes", type=PathSorter(baguettes, "baguette"), default=None, action="extend", nargs="*", help="the path(s) to the output baguette files (.pyt). Use '-' to leave it to the automatic destination. Defaults to environment variable 'BAGUETTE_BAGUETTES' or '-' if not set.")
         parser.add_argument("--visuals", type=PathSorter(visuals, "visual"), default=None, action="extend", nargs="*", help="the path(s) to the output visual (Gephi) files (.gexf). Use '-' to leave it to the automatic destination. Defaults to environment variable 'BAGUETTE_VISUALS' or '-' if not set.")
         parser.add_argument("-o", "--outputs", type=PathSorter(outputs, "output"), default=None, action="extend", nargs="*", help="the path to the result index folders (which end in .bag). They contain the index file (.pyt) which stores all the information about a given baguette. Use '-' to leave it to the automatic destination. Defaults to environment variable 'BAGUETTE_OUTPUTS' or '.' if not set.")
         parser.add_argument("--pool", type=pool_size, default=pool_size("0.5"), help="the size of the process pool to use to bake in parallel.")
         parser.add_argument("--maxtime", type=time, default=time("inf"), help="the maximum amount of time spent baking a single baguette. No maxtime by default.")
         parser.add_argument("-f", "--filters", type=str, default=[], choices=[name for name in dir(filters) if isinstance(getattr(filters, name), filters.Filter)], nargs="*", help="a list of filters that can be used when exporting the baguette to the visual file (.gexf).")
         parser.add_argument("--perf", action="store_true", default=False, help="if this is enabled, a performance report will be printed at the end of the baking process.")
         parser.add_argument("-v", "--verbosity", action="count", default=0, help="increases the verbosity of the output.")
         parser.add_argument("--skip_data_comparison", action="store_true", default=False, help="if enabled, the computation of the Levenshtein similarity between all Data nodes will be skipped.")
         parser.add_argument("--skip_diff_comparison", action="store_true", default=False, help="same as skip_data_comparison but for Diff nodes.")
+        parser.add_argument("--background", type=paint_color, default=Color.black, help="If a color is given for background, the color settings which are close to the background color will be change to be more visible on background. Must be a valid color name or RGB values.")
+
 
         args = parser.parse_args()
 
         # Setting logging level
 
         levels = {
             0 : logging.ERROR,
@@ -390,14 +448,15 @@
                 bg.visual = v if v is not None else (bg.working_directory / "visual.gexf")
                 bg.verbosity = verbosity
                 bg.skip_data_comparison = args.skip_data_comparison
                 bg.skip_diff_comparison = args.skip_diff_comparison
                 bg.filter_names = args.filters
                 bg.maxtime = args.maxtime
                 bg.perf = args.perf
+                bg.background_color = args.background
                 work.append(bg)
         
         
         # Compile now...
 
         from multiprocessing.pool import Pool
         from threading import Lock, Thread
@@ -413,15 +472,16 @@
                     return False
                 br = work.pop()
             try:
                 br = P.apply(compile, (br, ))
             except KeyboardInterrupt as e:
                 from traceback import TracebackException
                 br.exception = TracebackException.from_exception(e)
-            br.export()
+            if br.exception is None or not br.suppressed:
+                br.export()
             if br.exception is not None and issubclass(br.exception.exc_type, KeyboardInterrupt):
                 return False
             elif br.exception is not None and not issubclass(br.exception.exc_type, TimeoutExit):
                 with lock:
                     failed += 1
                 logger.error("Got a '{}' error during the baking of '{}'.".format(br.exception.exc_type.__name__, br.report.name))
             elif br.exception is not None and issubclass(br.exception.exc_type, TimeoutExit):
```

### Comparing `baguette_verse-0.9.5/toast.py` & `baguette_verse-1.0.0/toast.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         from baguette.bakery.logger import logger, set_level
         set_level(logging.ERROR)
 
         import argparse
         from os import environ
         import pathlib
         from typing import Literal, Iterator
+        from baguette.bakery.source.colors import Color
         from baguette.croutons.extractor import extract
         from baguette.croutons.metalib.utils import entries
         from baguette.rack import BaguetteRack, TimeoutExit
 
         parser = argparse.ArgumentParser(
             description = 'Toasts Baguettes, picking up interesting slices as defined by MetaGraphs patterns.',
             add_help = True,
@@ -94,20 +95,76 @@
                 v = float(arg)
                 if v <= 0 or isnan(v):
                     parser.error("got a negative, null or nan maxtime")
                 return v
             except:
                 parser.error("expected positive float for maxtime, got : '{}'".format(arg))
 
+        def paint_color(c : str) -> Color:
+            if c in dir(Color):
+                color = getattr(Color, c)
+                if not isinstance(color, Color):
+                    parser.error(f"not a valid color name : '{c}'")
+                return color
+            else:
+                # We can match colors in ALLL LANGUAGES!!!!
+                import re
+                color_re = r"([\d\.eE-]+|\d+|0[xX][\daAbBcCdDeEfF]+)"
+                sep_re = r"(?:[ ,;:\|\&]+)"
+                inner_expr = r"(?:" + color_re + sep_re + color_re + sep_re + color_re + r")"
+                fmatch = re.compile(inner_expr).fullmatch(c) or re.compile(r"\(" + inner_expr + r"\)").fullmatch(c) or re.compile(r"\[" + inner_expr + r"\]").fullmatch(c) or re.compile(r"\{" + inner_expr + r"\}").fullmatch(c)
+                if not fmatch:
+                    parser.error(f"could not understand color format : '{c}'")
+                r, g, b = fmatch.groups()
+
+                def is_float(s : str) -> bool:
+                    try:
+                        f = float(s)
+                        if not 0 <= f <= 1:
+                            return False
+                        return True
+                    except:
+                        return False
+                
+                def is_int(s : str) -> bool:
+                    try:
+                        i = int(s)
+                        if not 0 <= i <= 255:
+                            return False
+                        return True
+                    except:
+                        return False
+                
+                def is_hex(s : str) -> bool:
+                    try:
+                        i = int(s, base=16)
+                        if not 0 <= i <= 255:
+                            return False
+                        return True
+                    except:
+                        return False
+                    
+                if all(is_float(x) for x in (r, g, b)):
+                    r, g, b = float(r), float(g), float(b)
+                elif all(is_int(x) for x in (r, g, b)):
+                    r, g, b = int(r), int(g), int(b)
+                elif all(is_hex(x) for x in (r, g, b)):
+                    r, g, b = int(r, 16), int(g, 16), int(b, 16)
+                else:
+                    parser.error(f"could not understand color format : '{c}'")
+
+                return Color(r, g, b)
+
         parser.add_argument("inputs", type=PathSorter(inputs, "input"), default=None, nargs="*" if ("BAGUETTE_INPUTS" in environ or "BAGUETTE_OUTPUTS" in environ) else "+", help="Baguette folders. These should contain the index file resulting from the baking. Can also be folders baguette folders. Defaults to environment variable 'BAGUETTE_INPUTS' (or 'BAGUETTE_OUTPUTS') if set.")
         parser.add_argument("--extracted", type=PathSorter(extracted, "extracted"), default=None, action="extend", nargs="*", help="the path(s) to the output extracted match files (.pyt). Use '-' to leave it to the automatic destination. Defaults to environment variable 'BAGUETTE_EXTRACTED' or '-' if not set.")
         parser.add_argument("--pool", type=pool_size, default=pool_size("0.5"), help="the size of the process pool to use to bake in parallel.")
         parser.add_argument("--maxtime", type=time, default=time("inf"), help="the maximum amount of time spent baking a single baguette. No maxtime by default.")
         parser.add_argument("-p", "--pattern", type=str, action="extend", choices=["-"] + entries(), nargs="+", help="The metapath names (as in the source.metalib module) to search for. Leave empty or use '-' to search for all defined metagraphs.")
         parser.add_argument("--perf", action="store_true", default=False, help="if this is enabled, a performance report will be printed at the end of the baking process.")
+        parser.add_argument("--paint", type=paint_color, nargs="+", default=[], help="If a color is given for painting, the matches found will be painted in the visual.gexf file. Must be a valid color name or RGB values.")
         parser.add_argument("-v", "--verbosity", action="count", default=0, help="increases the verbosity of the output.")
 
         args = parser.parse_args()
 
         # Setting logging level
 
         levels = {
@@ -141,17 +198,23 @@
                     parser.error("invalid extraction path in environment variable : '{}'".format(environ["BAGUETTE_EXTRACTED"]))
             else:
                 extracted = ["-"]
         
         if not args.pattern:
             args.pattern = entries()
         if "-" in args.pattern and len(args.pattern) > 1:
-            parser.error("If '-' is given for pattern, it should be the only.")
+            parser.error("if '-' is given for pattern, it should be the only.")
         if "-" in args.pattern:
             args.pattern = entries()
+
+        if args.paint:
+            if len(args.paint) == 1:
+                args.paint *= len(args.pattern)
+            if len(args.paint) != len(args.pattern):
+                parser.error("expected one color or as many colors as patterns to match.")
         
         class JobQueue:
 
             """
             These objects hold a series of grouped jobs.
             """
 
@@ -338,14 +401,15 @@
                 if not (i / "index.pyt").is_file():
                     parser.error("baguette folder does not have the appropriate index file : '{}' is not a file.".format(i / "index.pyt"))
                 bg = BaguetteRack.import_from(i / "index.pyt")
                 bg.extracted = e if e is not None else bg.working_directory / "extracted.pyt"
                 bg.pattern_names = args.pattern
                 bg.maxtime = args.maxtime
                 bg.perf = args.perf
+                bg.paint_color = args.paint
                 work.append(bg)
         
         
         # Extract now...
 
         from multiprocessing.pool import Pool
         from threading import Lock, Thread
@@ -361,15 +425,16 @@
                     return False
                 br = work.pop()
             try:
                 br = P.apply(extract, (br, ))
             except KeyboardInterrupt as e:
                 from traceback import TracebackException
                 br.exception = TracebackException.from_exception(e)
-            br.export()
+            if br.exception is None or not br.suppressed:
+                br.export()
             if br.exception is not None and issubclass(br.exception.exc_type, KeyboardInterrupt):
                 return False
             elif br.exception is not None and not issubclass(br.exception.exc_type, TimeoutExit):
                 with lock:
                     failed += 1
                 logger.error("Got a '{}' error during the toasting of '{}'.".format(br.exception.exc_type.__name__, br.working_directory.name))
             elif br.exception is not None and issubclass(br.exception.exc_type, TimeoutExit):
```

### Comparing `baguette_verse-0.9.5/baguette/rack.py` & `baguette_verse-1.0.0/baguette/rack.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from pathlib import Path
 from traceback import TracebackException
 from typing import Any, Literal, TypeVar
 
 from .croutons.source.metagraph import MetaGraph
 from .bakery.source.filters import Filter
+from .bakery.source.colors import Color
 
 __all__ = ["BaguetteRack", "TimeoutExit"]
 
 
 
 
 
@@ -41,15 +42,18 @@
         "__patterns" : "The list of MetaGraphs to search for during the extraction phase",
         "__skip_data_comparison" : "A boolean indicating if Data nodes were compared during compilation",
         "__skip_diff_comparison" : "A boolean indicating if Diff nodes were compared during compilation",
         "__exception" : "The last caught exception",
         "__baked" : "Indicates if the baguette has been successfully baked",
         "__toasted" : "Indicates if the baguette has been successfully toasted",
         "__verbosity" : "The verbosity level to apply when baking or toasting", 
-        "__maxtime" : "The maximum amount of time to spend on this baguette"
+        "__maxtime" : "The maximum amount of time to spend on this baguette",
+        "__paint_color" : "The color to use to paint MetaGraph matches in the visual file",
+        "__suppressed" : "Indicates if an exception should suppress the index file output",
+        "__background_color" : "The color of the background for the visual graph"
     }
 
     names = {
         "working_directory" : "BAGUETTE Directory",
         "index" : "BAGUETTE Index File",
         "report" : "Cuckoo Report File",
         "baguette" : "Python BAGUETTE File",
@@ -57,14 +61,15 @@
         "extracted" : "Extracted MetaGraphs Python File",
     }
 
     def __init__(self, working_directory : str | Path | None = None) -> None:
         from pathlib import Path
         from traceback import TracebackException
         from typing import Literal
+        from .bakery.source.colors import Color
         self.__working_directory : Path | None = None
         self.__index : Path | None = None
         self.__report : Path | None = None
         self.__baguette : Path | None = None
         self.__visual : Path | None = None
         self.__extracted : Path | None = None
         self.__perf : bool = False
@@ -73,14 +78,15 @@
         self.__skip_data_comparison : bool = False
         self.__skip_diff_comparison : bool = False
         self.__exception : TracebackException | None = None
         self.__baked : bool = False
         self.__toasted : bool = False
         self.__verbosity : Literal[0, 1, 2, 3] = 0
         self.__maxtime : float = float("inf")
+        self.__paint_color : list[Color] | None = None
         if working_directory is not None and not isinstance(working_directory, str | Path):
             raise TypeError("Expected Path, got " + repr(type(working_directory).__name__))
         if working_directory is not None:
             self.set_defaults(Path(working_directory))
         
     def set_defaults(self, working_directory : Path):
         """
@@ -91,14 +97,62 @@
         self.__index = working_directory / "index.pyt"
         self.__baguette = working_directory / "baguette.pyt"
         self.__visual = working_directory / "visual.gexf"
         self.__extracted = working_directory / "extracted.pyt"
         self.check()
 
     @property
+    def suppressed(self) -> bool:
+        """
+        Indicates if a raised exception should suppress the output file writing.
+        """
+        return self.__suppressed
+
+    @suppressed.setter
+    def suppressed(self, value : bool):
+        if not isinstance(value, bool):
+            raise TypeError(f"Expected bool, got '{type(value).__name__}'")
+        self.__suppressed = value
+
+    @property
+    def paint_color(self) -> list[Color] | None:
+        """
+        The Colors in which to paint the MetaGraph matches found during toasting.
+        The index of the color correspond to the index of the MetaGraph in the "patterns" attribute.
+        None indicates no painting.
+        """
+        return self.__paint_color
+    
+    @paint_color.setter
+    def paint_color(self, value : list[Color] | None):
+        from .bakery.source.colors import Color
+        if value is not None and not isinstance(value, list):
+            raise TypeError("Expected None or list of Colors, got " + repr(type(value).__name__))
+        if isinstance(value, list):
+            for c in value:
+                if not isinstance(c, Color):
+                    raise TypeError("Expected list of Colors, got a " + repr(type(c).__name__))
+        self.__paint_color = value
+
+    @property
+    def background_color(self) -> Color:
+        """
+        The background color that will be used for the visual file.
+        This is used to change the color settings which are too close from the background color in order to make the visual sharper.
+        """
+        return self.__background_color
+    
+    @background_color.setter
+    def background_color(self, value : Color):
+        from .bakery.source.colors import Color
+        if not isinstance(value, Color):
+            raise TypeError(f"Expected Color, got '{type(value).__name__}'")
+        self.__background_color = value
+
+    @property
     def maxtime(self) -> float:
         """
         The maximum amount of time (in seconds) to spend on the baking or toasting process of this baguette.
         Defaults to infinity.
         """
         return self.__maxtime
```

### Comparing `baguette_verse-0.9.5/baguette/bakery/compiler.py` & `baguette_verse-1.0.0/baguette/bakery/compiler.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,48 +36,56 @@
         set_level(levels[rack.verbosity])
 
         logger.debug("Just change worker's verbosity level.")
 
         import os
         from pickle import dump
         from .source.build import Builder
-        from .source.config import CompilationParameters
+        from .source.config import CompilationParameters, ajust_for_background_color
         from .source import types
         from Viper.better_threading import Future, DaemonThread
 
         if rack.perf:
             from .source.utils import chrono
             chrono.enabled = True
             chrono.auto_report = True
 
         if not os.path.exists(rack.report):
+            rack.suppressed = True
             raise FileNotFoundError("Could not find report file: {}".format(rack.report))
         if not os.path.isfile(rack.report):
+            rack.suppressed = True
             raise FileExistsError("Given path to report file is not a file.")
         if os.path.exists(rack.baguette) and not os.path.isfile(rack.baguette):
+            rack.suppressed = True
             raise FileExistsError("Given baguette output file exists and is not a file.")
         if os.path.exists(rack.visual) and not os.path.isfile(rack.visual):
+            rack.suppressed = True
             raise FileExistsError("Given visual output file exists and is not a file.")
 
         if rack.skip_data_comparison:
-            CompilationParameters.get_config().SkipLevenshteinForDataNodes = True
+            CompilationParameters.SkipLevenshteinForDataNodes = True
         if rack.skip_diff_comparison:
-            CompilationParameters.get_config().SkipLevenshteinForDiffNodes = True
+            CompilationParameters.SkipLevenshteinForDiffNodes = True
 
         result : Future[bool] = Future()
 
         def compile_main():
             
             try:
                 logger.info("Loading file...")
-                with rack.report.open("r") as file:
-                    b = Builder(file)
-                if not b.data:
-                    logger.error("Could not load file properly...")
-                    raise RuntimeError("Could not load file properly")
+                from json import JSONDecodeError
+                try:
+                    with rack.report.open("r") as file:
+                        b = Builder(file)
+                except JSONDecodeError:
+                    rack.suppressed = True
+                    raise
+                logger.info("Checking color settings...")
+                ajust_for_background_color(rack.background_color)
                 logger.info("Building graph...")
                 b.build()
                 G = b.graph
                 logger.info("Analyzing graph...")
                 logger.info("Got {} vertices and {} edges.".format(G.n, G.m))
                 logger.info("Saving with pickle")
                 rack.baguette.parent.mkdir(parents = True, exist_ok = True)
```

### Comparing `baguette_verse-0.9.5/baguette/bakery/cuckoo_api_list.md` & `baguette_verse-1.0.0/baguette/bakery/cuckoo_api_list.md`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9.5/baguette/bakery/logger.py` & `baguette_verse-1.0.0/baguette/bakery/logger.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/build.py` & `baguette_verse-1.0.0/baguette/bakery/source/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,16 +65,15 @@
                 raise 
         if isinstance(data, IOBase):
             from json import load, JSONDecodeError
             try:
                 data = load(data)
                 logger.info("File loaded and structured.")
             except JSONDecodeError:
-                data = {}
-                logger.error("JSON file has strutural problems.")
+                raise
         if not isinstance(data, dict):
             raise TypeError("Expected dict or json file, got " + repr(data.__class__.__name__))
         self.data = data
         self._progress = 0
         self._target = 1
     
     @property
```

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/colors.py` & `baguette_verse-1.0.0/baguette/bakery/source/colors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module defines colors to be used for graphs.
 """
 
-from typing import Any, Iterable, Tuple, Union
+from typing import Any, Iterable, Iterator, Tuple, Union
 
 __all__ = ["chart", "Color"]
 
 
 
 
 
@@ -171,14 +171,20 @@
         try:
             return super().__getattribute__(name)
         except AttributeError:
             if name in chart:
                 return chart[name]
             else:
                 raise AttributeError("type object " + repr(super().__getattribute__("__name__")) + " has no attribute " + repr(name))
+            
+    def __dir__(self) -> list[str]:
+        """
+        Implements dir(Color).
+        """
+        return list(super().__dir__()) + list(chart)
 
 
 
 
 
 class Color(metaclass = ColorType):
 
@@ -211,16 +217,16 @@
 
     def __str__(self) -> str:
         """
         Implements str(self).
         """
         for name, value in chart.items():
             if Color(value.R, value.G, value.B) == self:
-                return "color." + name
-        return "color" + str((self.R, self.G, self.B))
+                return "Color." + name
+        return "Color" + str((self.R, self.G, self.B))
     
 
     __repr__ = __str__
     
 
     def __eq__(self, o: object) -> bool:
         """
@@ -296,14 +302,38 @@
         """
         Implements self ** o.
         """
         if isinstance(o, int | float):
             return Color(min(1.0, max(0.0, self.R ** o)), min(1.0, max(0.0, self.G ** o)), min(1.0, max(0.0, self.B ** o)))
         else:
             return NotImplemented
+        
+
+    def negative_to(self, ref : "Color") -> "Color":
+        """
+        Returns the negative of this color relative to another color. (Equivalent to -self relatively to any whitescale color)
+        """
+        if not isinstance(ref, Color):
+            raise TypeError(f"Exepcted Color, got '{type(ref).__name__}'")
+        M = Color(0.5, 0.5, 0.5)
+        if ref == M:
+            raise ZeroDivisionError(f"Cannot compute negative relative to central Color ({M})")
+        SM : tuple[float, float, float] = tuple(Mi - Si for Mi, Si in zip(M, self))
+        RM : tuple[float, float, float] = tuple(Mi - Ri for Mi, Ri in zip(M, ref))
+        fact = 2 * sum(a * b for a, b in zip(SM, RM)) / sum(b ** 2 for b in RM)
+        return Color(*(max(min(Si + fact * RMi, 1.0), 0.0) for Si, RMi in zip(self, RM)))
+
+
+    def __iter__(self) -> Iterator[float]:
+        """
+        Implements iter(self).
+        """
+        yield self.R
+        yield self.G
+        yield self.B
 
     
     def to_int(self) -> Tuple[int, int, int]:
         """
         Returns a tuple of three integers representing the color.
         """
         return (round(self.R * 255), round(self.G * 255), round(self.B * 255))
@@ -336,8 +366,8 @@
 
 
 
 
 # Convert color vectors of the __chart_init to Color objects in the real chart
 chart.update((name, Color(*value)) for name, value in __chart_init.items())
 
-del Any, Tuple, Union, ColorType, Iterable, __chart_init
+del Any, Tuple, Union, ColorType, Iterable, Iterator, __chart_init
```

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/event.py` & `baguette_verse-1.0.0/baguette/bakery/source/event.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/filters.py` & `baguette_verse-1.0.0/baguette/bakery/source/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,30 +137,30 @@
 
 Key_KeyEntry_Model : System[Key | KeyEntry | Handle] = System()
 _strong_keys : set[Key] = set()
 
 @cache
 def changed_registry(u : Vertex) -> bool:           # This filter is so fucking complicated!!!
     from .types.registry import Key, KeyEntry, Handle, ChangesTowards, SetsEntry, DeletesEntry, HasSubKey
-    from .config import ColorMap
+    from .config import ColorSetting
 
     if not isinstance(u, Key | KeyEntry | Handle):
         return True
     
     if isinstance(u, Handle):
         with Key_KeyEntry_Model.Entangled(u):
             return any(changed_registry(v) for v in u.neighbors() if isinstance(v, KeyEntry) if v not in Key_KeyEntry_Model) or any(changed_registry(v) for v in u.neighbors() if isinstance(v, Key) and v not in Key_KeyEntry_Model)
     
     if isinstance(u, KeyEntry):
         with Key_KeyEntry_Model.Entangled(u):              # Checking this Entry: do not do it twice!
 
             if u.key in _strong_keys:               # We are actually propagating the collapse of the wave function!
                 return True
             
-            if u.color == ColorMap.get_config().Deleted:        # This is an important Entry : it collapses the wave function!
+            if u.color == u.deleted_key_entry_color:        # This is an important Entry : it collapses the wave function!
                 _strong_keys.add(u.key)
                 Key_KeyEntry_Model.add_callback(_strong_keys.remove, u.key)
                 return True
 
             for e in u.edges:
                 if isinstance(e, SetsEntry | DeletesEntry):     # This is an important Entry : it collapses the wave function!
                     _strong_keys.add(u.key)
@@ -180,15 +180,15 @@
                 return False
     
     if isinstance(u, Key):
     
         with Key_KeyEntry_Model.Entangled(u):
             Key_KeyEntry_Model.population = u.entries       # Set the populations of entries to entangle with.
 
-            if u.color == ColorMap.get_config().Deleted:        # This is an important Key : it collapses the wave function!
+            if u.color == u.deleted_key_color:        # This is an important Key : it collapses the wave function!
                 _strong_keys.add(u)
                 Key_KeyEntry_Model.add_callback(_strong_keys.remove, u)
 
             if Key_KeyEntry_Model.population and all(changed_registry(v) for v in Key_KeyEntry_Model.include()):       # If it is a strong key, positive collapse will start in one of the entries and propagate to all others.
                 return True
             
             if u in _strong_keys:       # It was a strong Key due to its own color.
```

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/graph.py` & `baguette_verse-1.0.0/baguette/bakery/source/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 This module defines all graph-related objects.
 """
 
 from threading import RLock, Thread
-from typing import Any, Callable, Dict, Iterable, Iterator, Optional, Set, Tuple, Type, TypeVar, Union
+from typing import Any, Callable, Iterable, Iterator, Optional, TypeVar, Union
 from .colors import Color
+from .config import ColorSetting, SizeSetting, SwitchSetting, WeightSetting
 from Viper.meta.iterable import InstanceReferencingClass
 
 __all__ = ["Vertex", "UniqueVertex", "Edge", "Arrow", "Graph", "find_or_create"]
 
 
 
 
@@ -17,76 +18,100 @@
 
     """
     A vertex for a graph. Can be linked to other vertices and added to a graph.
     """
 
     __slots__ = {
         "edges" : "The set of edges linking this vertex to others.",
-        "color" : "The color to use for representation (three values between 0 and 1)",
         "parent" : "A vertex that 'contains' this one.",
         "children" : "The tuple of vertices (directly) contained by this one.",
         "graph" : "The graph object containing this vertex",
-        "__size" : "The size of the vertex"
+        "__size" : "The customized size of the vertex",
+        "__color" : "The customized color of the vertex"
         }
     
     __pickle_slots__ = {
         "color",
         "parent",
         "size"
     }
 
-    def __init__(self, *, c : Color | None = None, parent : Optional["Vertex"] = None) -> None:
+    default_color = ColorSetting(Color.white)
+    default_size = SizeSetting(2.0)
+
+    def __init__(self, *, parent : Optional["Vertex"] = None) -> None:
         from .colors import Color
-        from .config import ColorMap, SizeMap
-        if c is None:
-            c = ColorMap.get_config().get_color(type(self))
-        if not isinstance(c, Color):
-            raise TypeError("Expected color for c, got " + repr(c.__class__.__name__))
         if parent != None and not isinstance(parent, Vertex):
             raise TypeError("Expected vertex for parent, got " + repr(parent.__class__.__name__))
-        self.edges : Set[Edge] = set()
-        self.color : Color = c
-        self.__size : float = SizeMap.get_config().get_size(type(self))
+        self.edges : set[Edge] = set()
+        self.__color : Color | None = None
+        self.__size : float | None = None
         self.parent : Vertex | None = parent
         self.graph : Graph | None = None
         if parent:
             parent.children += (self, )
-        self.children : Tuple[Vertex, ...] = ()
+        self.children : tuple[Vertex, ...] = ()
         for g in Graph.active_graphs():
             g.vertices.add(self)
 
     __vertexing = False
     __comparing : set[tuple["Vertex", ...]] = set()
 
     @property
-    def label(self) -> str:
+    def color(self) -> Color:
         """
-        The label used when plotting this vertex.
+        The Color of this Vertex.
         """
-        return type(self).__name__
+        if self.__color is not None:
+            return self.__color
+        return self.default_color
+    
+    @color.setter
+    def color(self, value : Color):
+        from .colors import Color
+        if not isinstance(value, Color):
+            raise TypeError(f"Expected Color, got '{type(value).__name__}'")
+        self.__color = value
+
+    @color.deleter
+    def color(self):
+        self.__color = None
 
     @property
     def size(self) -> float:
         """
-        The size of this Vertex. Default is 20.0.
+        The size of this Vertex.
         """
-        return self.__size
+        if self.__size is not None:
+            return self.__size
+        return self.default_size
     
     @size.setter
     def size(self, value : float):
         if not isinstance(value, float):
             try:
                 value = float(value)
             except:
                 pass
         if not isinstance(value, float):
-            raise TypeError("Expected float for size, got " + repr(type(value).__name__))
+            raise TypeError("Expected float, got " + repr(type(value).__name__))
         if value < 0 or value in (float("inf"), float("nan")):
             raise ValueError("Expected positive finite number for size, got " + repr(value))
         self.__size = value
+    
+    @size.deleter
+    def size(self):
+        self.__size = None
+
+    @property
+    def label(self) -> str:
+        """
+        The label used when plotting this vertex.
+        """
+        return type(self).__name__
 
     def __repr__(self) -> str:
         """
         Implements repr(self)
         """
         if Vertex.__vertexing:
             return str(type(self)) + "()"
@@ -144,22 +169,22 @@
             raise TypeError("Expected tuple from parent's __reduce__, got str")
         func, args, state = pickle_data
         state : dict
         if "edges" in state or "graph" in state:
             raise RuntimeError("Cannot pickle edges or graph of a vertex")
         return type(self), (), state
     
-    def __setstate__(self, state : Dict[str, Any]):
+    def __setstate__(self, state : dict[str, Any]):
         """
         Implements loading of self
         """
         for k, v in state.items():
             setattr(self, k, v)
     
-    def __getstate__(self) -> Dict[str, Any]:
+    def __getstate__(self) -> dict[str, Any]:
         """
         Implements dumping of self
         """
         from .utils import extract_pickle_slots
         return {name : getattr(self, name) for name in extract_pickle_slots(type(self))}
     
     def __copy__(self) -> "Vertex":
@@ -170,15 +195,15 @@
         cp = type(self)()
         cp.color = self.color
         for name in dir(self):
             if not name.startswith("_") and not name.endswith("_") and name not in Vertex.__slots__ and not ismethod(getattr(self, name)):
                 setattr(cp, name, getattr(self, name))
         return cp
     
-    def __deepcopy__(self, memo : Dict[int, Any]) -> "Vertex":
+    def __deepcopy__(self, memo : dict[int, Any]) -> "Vertex":
         """
         Implements deepcopy of self
         """
         from copy import deepcopy
         from inspect import ismethod
         cp = type(self)()
         cp.color = self.color
@@ -218,34 +243,30 @@
         """
         Iterates over the undirected neighbors if this vertex (neighbors linked by a strict edge).
         """
         for e in self.edges:
             if not isinstance(e, Arrow):
                 yield (e.source if e is not e.source else e.destination)
 
-    def connect(self, o : "Vertex", *, directional : bool = False, c : Optional[Color] = None) -> None:
+    def connect(self, o : "Vertex", *, directional : bool = False) -> None:
         """
         Links this vertex to another. Directional indicates if the link should be an arrow instead of an edge.
         """
         if not isinstance(o, Vertex):
             raise TypeError("Expected vertex, got " + repr(o.__class__.__name__))
         if not isinstance(directional, bool):
             raise TypeError("Expected bool for directional, got" + repr(directional.__class__.__name__))
-        if c == None:
-            c = Color.average(self.color, o.color)
-        if not isinstance(c, Color):
-            raise TypeError("Expected color for c, got " + repr(c.__class__.__name__))
         if directional:
-            e = Arrow(self, o, c=c)
+            e = Arrow(self, o)
         else:
-            e = Edge(self, o, c=c)
+            e = Edge(self, o)
         e.write()
 
     @classmethod
-    def add_vertices_to_graph(cls : Type["Vertex"], G : "Graph", fil : Optional[Callable[["Vertex"], bool]] = None):
+    def add_vertices_to_graph(cls : type["Vertex"], G : "Graph", fil : Optional[Callable[["Vertex"], bool]] = None):
         """
         Adds all vertices of this class to a graph.
         If given a filter function fil, only filtered vertices will be added.
         """
         if not isinstance(G, Graph):
             raise TypeError("Expected graph, got " + repr(G.__class__.__name__))
         if fil != None and not callable(fil):
@@ -286,74 +307,101 @@
     """
     An (undirected) edge for a graph. Links two vertices together.
     """
 
     __slots__ = {
         "source" : "The source vertex.",
         "destination" : "The destination vertex.",
-        "color" : "The color to use for representation (all between 0 and 1)",
-        "__weight" : "The weight of the edge"
+        "__weight" : "The customized weight of the edge",
+        "__color" : "The customized color of the edge"
     }
 
     __pickle_slots__ = {
         "color",
         "source",
         "destination",
         "weight"
     }
 
-    def __init__(self, source : Vertex, destination : Vertex, *, c: Color | None = None, auto_write : bool = True) -> None:
+    default_color = ColorSetting(Color.white)
+    default_weight = WeightSetting(1.0)
+
+    blend_vertices_colors = SwitchSetting(True)
+
+    def __init__(self, source : Vertex, destination : Vertex, *, auto_write : bool = True) -> None:
         from .colors import Color
         if not isinstance(source, Vertex) or not isinstance(destination, Vertex):
             raise TypeError("Expected vertex, vertex, got " + repr(source.__class__.__name__) + " and " + repr(destination.__class__.__name__))
-        if c == None:
-            from .config import ColorMap
-            if ColorMap.get_config().has_color(type(self)):
-                c = ColorMap.get_config().get_color(type(self))
-            else:
-                c = Color.average(source.color, destination.color)
-        if not isinstance(c, Color):
-            raise TypeError("Expected color for c, got " + repr(c.__class__.__name__))
         if not isinstance(auto_write, bool):
             raise TypeError("Expected bool for write, got " + repr(auto_write.__class__.__name__))
         self.source : Vertex = source
         self.destination : Vertex = destination
-        self.color : Color = c
-        self.__weight : float = 1.
+        self.__color : Color | None = None
+        self.__weight : float | None = None
         if auto_write:
             self.write()
         for g in Graph.active_graphs():
             g.edges.add(self)
-    
+
     @property
-    def label(self) -> str:
+    def color(self) -> Color:
         """
-        The label used when plotting this edge.
+        The Color of this Vertex.
         """
-        return type(self).__name__
+        if self.__color is not None:
+            return self.__color
+        if self.blend_vertices_colors:
+            from .colors import Color
+            return Color.average(self.source.color, self.destination.color)
+        else:
+            return self.default_color
     
+    @color.setter
+    def color(self, value : Color):
+        from .colors import Color
+        if not isinstance(value, Color):
+            raise TypeError(f"Expected Color, got '{type(value).__name__}'")
+        self.__color = value
+
+    @color.deleter
+    def color(self):
+        self.__color = None
+        
     @property
     def weight(self) -> float:
         """
-        The weight of this Edge. Default is 1.0.
+        The weight of this Edge.
         """
-        return self.__weight
+        if self.__weight is not None:
+            return self.__weight
+        return self.default_weight
     
     @weight.setter
     def weight(self, value : float):
         if not isinstance(value, float):
             try:
                 value = float(value)
             except:
                 pass
         if not isinstance(value, float):
             raise TypeError("Expected float for weight, got " + repr(type(value).__name__))
         if value < 0 or value in (float("inf"), float("nan")):
             raise ValueError("Expected positive finite number for weight, got " + repr(value))
         self.__weight = value
+
+    @weight.deleter
+    def weight(self):
+        self.__weight = None
+
+    @property
+    def label(self) -> str:
+        """
+        The label used when plotting this edge.
+        """
+        return type(self).__name__
     
     def __repr__(self) -> str:
         """
         Implements repr(self)
         """
         return "edge(" + repr(self.source) + ", " + repr(self.destination) + ")"
     
@@ -373,22 +421,22 @@
         """
         Implements self == o
         """
         if not isinstance(o, type(self)):
             return False
         return (self.source == o.source and self.destination == o.destination) or (self.source == o.destination and self.destination == o.source)
         
-    def __setstate__(self, state : Dict[str, Any]):
+    def __setstate__(self, state : dict[str, Any]):
         """
         Implements loading of self
         """
         for k, v in state.items():
             setattr(self, k, v)
     
-    def __getstate__(self) -> Dict[str, Any]:
+    def __getstate__(self) -> dict[str, Any]:
         """
         Implements dumping of self
         """
         from .utils import extract_pickle_slots
         return {name : getattr(self, name) for name in extract_pickle_slots(type(self))}
     
     def __copy__(self) -> "Edge":
@@ -404,28 +452,28 @@
         self.source.edges.add(self)
         self.destination.edges.add(self)
         if self.source.graph:
             self.source.graph.edges.add(self)
         elif self.destination.graph:
             self.destination.graph.edges.add(self)
     
-    def delete(self) -> Tuple[Vertex, Vertex]:
+    def delete(self) -> tuple[Vertex, Vertex]:
         """
         Deletes the link. (Deletes it from the vertices egde sets)
         """
         self.source.edges.discard(self)
         self.destination.edges.discard(self)
         if self.source.graph:
             self.source.graph.edges.discard(self)
         elif self.destination.graph:
             self.destination.graph.edges.discard(self)
         return self.source, self.destination
     
     @classmethod
-    def add_edges_to_graph(cls : Type["Edge"], G : "Graph", fil : Optional[Callable[["Edge"], bool]] = None):
+    def add_edges_to_graph(cls : type["Edge"], G : "Graph", fil : Optional[Callable[["Edge"], bool]] = None):
         """
         Adds all edges of this class to a graph.
         If given a filter function fil, only filtered edges will be added.
         """
         if not isinstance(G, Graph):
             raise TypeError("Expected graph, got " + repr(G.__class__.__name__))
         if fil != None and not callable(fil):
@@ -474,15 +522,15 @@
 
 
 
 
 
 CLS = TypeVar("CLS", bound=Vertex)
 
-def find_or_create(cls : Type[CLS], **kwargs) -> Tuple[CLS, bool]:
+def find_or_create(cls : type[CLS], **kwargs) -> tuple[CLS, bool]:
     """
     Finds in the given class cls for a vertex which attributes have values matching the given keyword arguments.
     If there is one, returns it. Otherwise, creates it.
     Returns the object and a boolean indicating if the object existed before.
     """
     for ist in cls:
         if all(hasattr(ist, name) and getattr(ist, name) == value for name, value in kwargs.items()):
@@ -509,16 +557,16 @@
         "data" : "A dictionary holding additional data for this graph"
     }
 
     __active_graphs : dict[Thread, list["Graph"]] = {}
 
     def __init__(self) -> None:
         from typing import Any
-        self.vertices : Set[Vertex] = set()
-        self.edges : Set[Edge] = set()
+        self.vertices : set[Vertex] = set()
+        self.edges : set[Edge] = set()
         self.data : dict[str, Any] = {}
     
     def __enter__(self):
         """
         Implements with self.
         """
         from threading import current_thread
@@ -690,25 +738,25 @@
         if not isinstance(c, Color):
             raise TypeError("Expected Color, got " + repr(type(c).__name__))
         for u in self.vertices:
             u.color = c
         for e in self.edges:
             e.color = c
 
-    def __getstate__(self) -> Dict[str, Any]:
+    def __getstate__(self) -> dict[str, Any]:
         """
         Implements dumping of self.
         """
         return {
             "vertices" : self.vertices,
             "edges" : self.edges, 
             "data" : self.data
         }
 
-    def __setstate__(self, state : Dict[str, Any]):
+    def __setstate__(self, state : dict[str, Any]):
         """
         Implements loading of self.
         """
         for name, value in state.items():
             setattr(self, name, value)
         for v in self.vertices:
             v.graph = self
@@ -776,15 +824,15 @@
                 node_attr = ET.SubElement(graph, "attributes", **{"class" : "node", "mode" : "static"})
                 node_attributes = {}
                 edge_attr = ET.SubElement(graph, "attributes", **{"class" : "edge", "mode" : "static"})
                 edge_attributes = {}
                 nodes = ET.SubElement(graph, "nodes")
                 edges = ET.SubElement(graph, "edges")
                 n_ids = {u : i for i, u in enumerate(self.vertices)}
-                additional_links : Set[Tuple[Vertex, Vertex]] = set()
+                additional_links : set[tuple[Vertex, Vertex]] = set()
                 for u, i in n_ids.items():
                     d = {name : str(getattr(u, name)).translate(forbidden_characters) for name in u.__pickle_slots__ if not name.startswith("_")}
                     d["Type"] = type(u).__name__
                     if "__weakref__" in d:
                         d = {}
                     if u.parent:
                         if subgraph_supported:
@@ -836,8 +884,8 @@
                 ET.indent(root, "\t")
                 for line in ET.tostringlist(root):
                     f.write(line + b"\n")
         except Exception as E:
             raise
     
 
-del RLock, Any, Callable, Dict, Iterable, Iterator, Optional, Set, Tuple, Type, TypeVar, Union, Color, InstanceReferencingClass, CLS
+del RLock, Any, Callable, Iterable, Iterator, Optional, TypeVar, Union, Color, InstanceReferencingClass, CLS, ColorSetting, SizeSetting, SwitchSetting, WeightSetting
```

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/record.py` & `baguette_verse-1.0.0/baguette/bakery/source/record.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/utils.py` & `baguette_verse-1.0.0/baguette/bakery/source/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/types/__init__.py` & `baguette_verse-1.0.0/baguette/bakery/source/types/__init__.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/types/utils.py` & `baguette_verse-1.0.0/baguette/bakery/source/types/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/types/data/entities.py` & `baguette_verse-1.0.0/baguette/bakery/source/types/data/entities.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 This module contains Vertex subclasses for this behavioral package.
 """
 
 from typing import Iterator, Optional
 
 from ....logger import logger
+from ...config import ColorSetting, SizeSetting
 from ...colors import Color
 from ...graph import UniqueVertex, Vertex
 from ...utils import chrono
 from ..filesystem.entities import File, Handle
 from ..network.entities import Connection, Socket
 from .utils import IOOperation
 
@@ -41,16 +42,19 @@
         "data",
         "length",
         "entropy",
         "time",
         "isprintable"
     }
 
-    def __init__(self, *, c: Color | None = None, parent: Optional[Vertex] = None) -> None:
-        super().__init__(c=c, parent=parent)
+    default_color = ColorSetting(Color(0.5882352941176471, 1.0, 1.0))
+    default_size = SizeSetting(0.5)
+
+    def __init__(self, *, parent: Optional[Vertex] = None) -> None:
+        super().__init__(parent=parent)
         self.__initialized = False
         self.data : bytes = b""
         self.length : int = 0
         self.entropy : float = 0.0
         self.time : float = 0.0
         self.isprintable : bool = False
     
@@ -158,17 +162,26 @@
         "printable_rate",
         "encoding",
     }
 
     _active_target_diff : dict[File | Connection, "Diff"] = {}
     _active_vector_diff : dict[Handle | Socket, "Diff"] = {}
 
-    def __init__(self, *, c: Color | None = None, parent: Optional["Vertex"] = None) -> None:
+    default_color = ColorSetting(Color(50, 150, 255))
+    default_size = SizeSetting(1.5)
+
+    min_size = SizeSetting(0.5)
+    max_size = SizeSetting(2.5)
+
+    diff_low_entropy_color = ColorSetting(Color(50, 150, 255))
+    diff_high_entropy_color = ColorSetting(Color(255, 50, 150))
+
+    def __init__(self, *, parent: Optional["Vertex"] = None) -> None:
         from .utils import DiffFile, IOOperation
-        super().__init__(c=c, parent=parent)
+        super().__init__(parent=parent)
         self.__initialized : bool = False
         self.__reader_difffile = DiffFile()
         self.__writer_difffile = DiffFile()
         self.__glob_difffile = DiffFile()
         self.__operations : list[IOOperation] = []
         self.read : bytes = b""
         self.read_type : list[str] = []
@@ -278,15 +291,15 @@
             for e in self.edges:
                 if isinstance(e, IsDiffOf):
                     IsReadBy(e.destination, e.source)
                     e.delete()
                     for G in Graph.active_graphs():
                         G.remove(e)
 
-        if CompilationParameters.get_config().SkipLevenshteinForDiffNodes:
+        if CompilationParameters.SkipLevenshteinForDiffNodes:
             return
         
         for u in Diff:
             if u not in self.neighbors() and u is not self:
                 lw, ls, ld = 0.0, "", ""
                 for sn, sb in zip(("read_buffer", "write_buffer", "global_buffer"), (r, w, g)):
                     if sb:
@@ -297,15 +310,15 @@
                                 s = levenshtein_similarity(sb, ub, Diff.similarity_threshold)
                                 if s >= lw:
                                     lw = s
                                     ls = sn
                                     ld= un
                 if ls and lw >= Diff.similarity_threshold:      # Heuristic is not perfect : checking that the threshold has indeed been reached!
                     l = HasSimilarContent(self, u)
-                    l.weight = lw
+                    l.weight = lw * (l.max_weight - l.min_weight) + l.min_weight        # 0 <= lw <= 1
                     l.source_buffer = ls
                     l.destination_buffer = ld
     
     @property
     def label(self) -> str:
         """
         The name of the node to display. It is the global data type.
@@ -336,8 +349,8 @@
             if isinstance(u, File | Connection):
                 yield u
 
 
 
 
 
-del Color, Connection, File, Handle, IOOperation, Iterator, Optional, Socket, UniqueVertex, Vertex, chrono, logger
+del Color, ColorSetting, SizeSetting, Connection, File, Handle, IOOperation, Iterator, Optional, Socket, UniqueVertex, Vertex, chrono, logger
```

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/types/data/integration.py` & `baguette_verse-1.0.0/baguette/bakery/source/types/data/integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
     from Viper.format import duration
 
     from ....logger import logger
     from ...config import CompilationParameters
     from .entities import Diff
     if e.major == "Finalizer" and e.minor == __N_diff_comparison_phase:
-        logger.debug("Finalizing{} {} Diff nodes.".format(" and comparing" if not CompilationParameters.get_config().SkipLevenshteinForDiffNodes else "",len(Diff)))
+        logger.debug("Finalizing{} {} Diff nodes.".format(" and comparing" if not CompilationParameters.SkipLevenshteinForDiffNodes else "",len(Diff)))
         n = len(Diff)
         t0 = time_ns()
         t = t0
         for i, d in enumerate(Diff):
             d.compute_data()
             if (time_ns() - t) / 1000000000 > 15:
                 t = time_ns()
@@ -110,15 +110,14 @@
     """
     When called with the right finalizing phase event, will cause all Diff nodes to compare their diff file sizes and change their size accordingly.
     """
     from typing import Type
 
     from ....logger import logger
     from ...colors import Color
-    from ...config import ColorMap, SizeMap
     from ...graph import Vertex
     from ..filesystem import File, Handle
     from ..network import Connection, Socket
     from .entities import Diff
 
     def project_range(x : float, sa : float, sb : float, da : float, db : float) -> float:
         if sa == sb:
@@ -126,16 +125,16 @@
         p = (x - sa) / (sb - sa)
         return p * (db - da) + da
 
     def normalize_neighbor(cls : Type[Vertex]):
         if len(cls) > 0:
             logger.debug("Normalizing {} {} nodes.".format(len(cls), cls.__name__))
             a, b = min(sum(v.size for v in u.neighbors() if isinstance(v, Diff)) for u in cls), max(sum(v.size for v in u.neighbors() if isinstance(v, Diff)) for u in cls)
-            minsize = SizeMap.get_config().get_size(cls) * 0.75
-            maxsize = SizeMap.get_config().get_size(cls) * 1.25
+            minsize = Diff.min_size
+            maxsize = Diff.max_size
             for u in cls:
                 u.size = project_range(sum(v.size for v in u.neighbors() if isinstance(v, Diff)), a, b, minsize, maxsize)
 
     if e.major == "Finalizer" and e.minor == __N_diff_normalization_phase:
         logger.debug("Normalizing sizes of {} Diff nodes.".format(len(Diff)))
         if len(Diff) == 0:
             return
@@ -147,15 +146,15 @@
     
         for cls in (File, Handle, Socket, Connection):
             normalize_neighbor(cls)
         
         logger.debug("Normalizing colors of {} Diff nodes.".format(len(Diff)))
         a, b = min(d.glob_entropy for d in Diff), max(d.glob_entropy for d in Diff)
         for d in Diff:
-            d.color = Color.linear((ColorMap.get_config().data.DiffLowEntropy, ColorMap.get_config().data.DiffHighEntropy), (1 - d.glob_entropy / 8, d.glob_entropy / 8))
+            d.color = Color.linear((Diff.diff_low_entropy_color, Diff.diff_high_entropy_color), (1 - d.glob_entropy / 8, d.glob_entropy / 8))
 
 @chrono
 def fuse_diff_nodes(e : BuildingPhase):
     """
     When called with the right finalizing phase event, will cause all identical Diff nodes to be merged with their size increasing.
     """
     from ....logger import logger
```

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/types/data/relations.py` & `baguette_verse-1.0.0/baguette/bakery/source/types/data/relations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 This module contains Edge and Arrow subclasses for this behavioral package.
 """
 
 from ....logger import logger
+from ...config import WeightSetting
 from ...colors import Color
 from ...graph import Arrow, Edge, Vertex
 from ..filesystem.entities import File, Handle
 from ..network.entities import Connection, Socket
 from .entities import Data, Diff
 
 __all__ = ["IsSimilarTo", "IsAlmostIn", "IsDiffOf", "IsReadBy", "WritesInto", "HasSimilarContent"]
@@ -105,16 +106,19 @@
     }
 
     label : str = ""
 
     source : Diff
     destination : Diff
 
-    def __init__(self, source: Vertex, destination: Vertex, *, c: Color | None = None, auto_write: bool = True) -> None:
-        super().__init__(source, destination, c=c, auto_write=auto_write)
+    min_weight = WeightSetting(0.5)
+    max_weight = WeightSetting(1.0)
+
+    def __init__(self, source: Vertex, destination: Vertex, *, auto_write: bool = True) -> None:
+        super().__init__(source, destination, auto_write=auto_write)
         self.__source_buffer = "global_buffer"
         self.__destination_buffer = "global_buffer"
         
     @property
     def source_buffer(self) -> str:
         """
         Returns the name of the content selected for comparison in the source node.
@@ -140,8 +144,8 @@
             raise ValueError("Diff node buffers can only be set to one of ('read_buffer', 'write_buffer', 'global_buffer')")
         self.__destination_buffer = name
 
 
 
 
 
-del Arrow, Color, Connection, Data, Diff, Edge, File, Handle, Socket, Vertex, logger
+del Arrow, Color, WeightSetting, Connection, Data, Diff, Edge, File, Handle, Socket, Vertex, logger
```

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/types/data/utils.py` & `baguette_verse-1.0.0/baguette/bakery/source/types/data/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/types/execution/entities.py` & `baguette_verse-1.0.0/baguette/bakery/source/types/execution/entities.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 This module contains Vertex subclasses for this behavioral package.
 """
 
 from typing import Optional
 
 from ....logger import logger
 from ...colors import Color
+from ...config import ColorSetting, SizeSetting
 from ...graph import UniqueVertex, Vertex
 from ...utils import chrono
 
 __all__ = ["Process", "Thread", "Call"]
 
 
 
@@ -39,16 +40,19 @@
         "command",
         "executable",
         "start",
         "stop",
         "sub_commands"
     }
 
-    def __init__(self, *, c: Color | None = None, parent: Vertex | None = None) -> None:
-        super().__init__(c=c, parent=parent)
+    default_color = ColorSetting(Color(255, 255, 50))
+    default_size = SizeSetting(5.0)
+
+    def __init__(self, *, parent: Vertex | None = None) -> None:
+        super().__init__(parent=parent)
         self.PID : int = 0
         self.__command : tuple[str] = tuple()
         self.executable : str = ""
         self.start : float = 0.0
         self.stop : float = 0.0
         self.__sub_commands : CommandTree | None = None
 
@@ -195,16 +199,19 @@
         "Ncalls",
         "first",
         "last",
         "start",
         "stop"
     }
 
-    def __init__(self, *, c: Color | None = None, parent: Optional[Vertex] = None) -> None:
-        super().__init__(c=c, parent=parent)
+    default_color = ColorSetting(Color(255, 204, 0))
+    default_size = SizeSetting(2.0)
+
+    def __init__(self, *, parent: Optional[Vertex] = None) -> None:
+        super().__init__(parent=parent)
         self.TID : int = 0
         self.Ncalls : int = 0
         self.first : Call | None = None
         self.last : Call | None = None
         self.start : float = 0.0
         self.stop : float = 0.0
 
@@ -257,19 +264,22 @@
         "arguments",
         "return_value",
         "time",
         "flags",
         "thread"
     }
 
-    def __init__(self, *, c: Color | None = None, parent: Optional[Vertex] = None) -> None:
+    default_color = ColorSetting(Color(255, 153, 0))
+    default_size = SizeSetting(0.3)
+
+    def __init__(self, *, parent: Optional[Vertex] = None) -> None:
         from typing import Any
 
         from ...record import record
-        super().__init__(c=c, parent=parent)
+        super().__init__(parent=parent)
         self.name : str = ""
         self.category : str = ""
         self.stacktrace : tuple = ()
         self.status : int = 0
         self.arguments : record = record()
         self.return_value : Any = None
         self.time : float = 0.0
@@ -298,8 +308,8 @@
         """
         return self.name
     
 
 
 
 
-del Color, CommandTree, Optional, UniqueVertex, Vertex, chrono, logger
+del Color,ColorSetting, SizeSetting, CommandTree, Optional, UniqueVertex, Vertex, chrono, logger
```

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/types/execution/integration.py` & `baguette_verse-1.0.0/baguette/bakery/source/types/execution/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/types/execution/relations.py` & `baguette_verse-1.0.0/baguette/bakery/source/types/execution/relations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 This module contains Edge and Arrow subclasses for this behavioral package.
 """
 
 from ....logger import logger
+from ...config import SwitchSetting
 from ...colors import Color
 from ...graph import Arrow, Edge, Vertex
 from ..filesystem.entities import Directory, File
 from .entities import Call, Process, Thread
 
 __all__ = ["HasChildProcess", "UsesAsArgument", "Runs", "HasThread", "HasFirstCall", "FollowedBy", "NextSignificantCall", "StartedThread", "InjectedThread", "StartedProcess"]
 
@@ -129,16 +130,16 @@
     }
 
     label : str = ""
 
     source : Call
     destination : Thread
 
-    def __init__(self, source: Vertex, destination: Vertex, *, c: Color | None = None, auto_write: bool = True) -> None:
-        super().__init__(source, destination, c=c, auto_write=auto_write)
+    def __init__(self, source: Vertex, destination: Vertex, *, auto_write: bool = True) -> None:
+        super().__init__(source, destination, auto_write=auto_write)
         self.remote : bool = False
     
 
 
 
 
 class InjectedThread(Arrow):
@@ -165,8 +166,8 @@
     source : Call
     destination : Process
 
 
 
 
 
-del Arrow, Call, Color, Directory, Edge, File, Process, Thread, Vertex, logger
+del Arrow, Call, Color, SwitchSetting, Directory, Edge, File, Process, Thread, Vertex, logger
```

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/types/execution/utils.py` & `baguette_verse-1.0.0/baguette/bakery/source/types/execution/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/types/filesystem/entities.py` & `baguette_verse-1.0.0/baguette/bakery/source/types/filesystem/entities.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 This module contains Vertex subclasses for this behavioral package.
 """
 
 import pathlib
 
 from ....logger import logger
+from ...config import ColorSetting, SizeSetting
 from ...colors import Color
 from ...graph import UniqueVertex, Vertex
 
 __all__ = ["File", "Directory", "Handle"]
 
 
 
@@ -26,17 +27,22 @@
         "__path" : "The path to the file in the file system",
     }
 
     __pickle_slots__ = {
         "path"
     }
 
-    def __init__(self, *, c: Color | None = None, parent: Vertex | None = None) -> None:
+    default_color = ColorSetting(Color(0, 255, 50))
+    default_size = SizeSetting(2.5)
+
+    deleted_file_color = ColorSetting(Color(100, 100, 100))
+
+    def __init__(self, *, parent: Vertex | None = None) -> None:
         from pathlib import PurePath
-        super().__init__(c=c, parent=parent)
+        super().__init__(parent=parent)
         self.__path : PurePath | None = None
 
     @property
     def path(self) -> pathlib.PurePath:
         """
         The absolute path to the file.
         """
@@ -87,18 +93,23 @@
     __slots__ = {
         "__path" : "The path to the directory in the file system",
     }
 
     __pickle_slots__ = {
         "path"
         }
+    
+    default_color = ColorSetting(Color(0, 100, 0))
+    default_size = SizeSetting(2.5)
 
-    def __init__(self, *, c: Color | None = None, parent: Vertex | None = None) -> None:
+    deleted_directory_color = ColorSetting(Color(100, 100, 100))
+
+    def __init__(self, *, parent: Vertex | None = None) -> None:
         from pathlib import PurePath
-        super().__init__(c=c, parent=parent)
+        super().__init__(parent=parent)
         self.__path : PurePath | None = None
 
     @property
     def path(self) -> pathlib.PurePath:
         """
         The absolute path to the directory.
         """
@@ -170,16 +181,19 @@
         "write_attributes",
         "read_extended_attributes",
         "write_extended_attributes",
         "list_directory",
         "traverse"
     }
 
-    def __init__(self, *, c: Color | None = None, parent: Vertex | None = None) -> None:
-        super().__init__(c=c, parent=parent)
+    default_color = ColorSetting(Color(128, 255, 50))
+    default_size = SizeSetting(1.5)
+
+    def __init__(self, *, parent: Vertex | None = None) -> None:
+        super().__init__(parent=parent)
 
         self.synchronize : bool = False
 
         self.read : bool = False
         self.write : bool = False
         self.append : bool = False
         self.execute : bool = False
@@ -202,9 +216,8 @@
                 return e.destination
         raise RuntimeError("Got a Handle working on no File or Directory.")
 
 
 
 
 
-
-del Color, UniqueVertex, Vertex, logger, pathlib
+del Color, ColorSetting, SizeSetting, UniqueVertex, Vertex, logger, pathlib
```

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/types/filesystem/integration.py` & `baguette_verse-1.0.0/baguette/bakery/source/types/filesystem/integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,29 +247,28 @@
             NewFile(fd).throw()
         IsCopyiedInto(fs, fd)
 
 @chrono
 def integrate_file_deleting(c : Call):
     # You need to make it possible to have multiple times the same file name...
     from ....logger import logger
-    from ...config import ColorMap
     from .entities import File
     if c.status == 1:
         logger.debug("Deleting file.")
         if c.arguments.filepath not in __existing_files:
             f = File()
             f.path = c.arguments.filepath
             __existing_files[c.arguments.filepath] = f
             if c.arguments.filepath not in __all_files:
                 __all_files[c.arguments.filepath] = []
             __all_files[c.arguments.filepath].append(f)
             NewFile(f).throw()
         else:
             f = __existing_files[c.arguments.filepath]
-        f.color = ColorMap.get_config().Deleted
+        f.color = f.deleted_file_color
         __existing_files.pop(c.arguments.filepath)
 
 
 
 
 
 # File creation
```

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/types/filesystem/relations.py` & `baguette_verse-1.0.0/baguette/bakery/source/types/filesystem/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/types/imports/entities.py` & `baguette_verse-1.0.0/baguette/bakery/source/types/imports/entities.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 This module contains Vertex subclasses for this behavioral package.
 """
 
 from ....logger import logger
+from ...config import ColorSetting, SizeSetting
 from ...colors import Color
 from ...graph import UniqueVertex, Vertex
 
 __all__ = ["Import"]
 
 
 
@@ -35,44 +36,49 @@
     __suspicious_keyword_names = {
         "crypt",
         "advapi",
         "kernel",
         "sock"
     }
 
-    def __init__(self, *, c: Color | None = None, parent: Vertex | None = None) -> None:
-        super().__init__(c=c, parent=parent)
+    default_color = ColorSetting(Color(150, 150, 0))
+    default_size = SizeSetting(0.75)
+
+    suspicious_import_color = ColorSetting(Color(255, 150, 0))
+
+    def __init__(self, *, parent: Vertex | None = None) -> None:
+        super().__init__(parent=parent)
         self.__name : str = ""
         self.path : str = ""
         self.length : int = 0
 
     @property
     def name(self) -> str:
         """
         The name of the imported library.
         """
         return self.__name
 
     @name.setter
     def name(self, n : str):
-        from ...config import ColorMap
+        from ...config import ColorSetting
         if not isinstance(n, str):
             raise TypeError("Expected str, got " + repr(type(n).__name__))
         self.__name = n
-        self.color = ColorMap.get_config().imports.Import
+        self.color = self.default_color
         for kw in self.__suspicious_keyword_names:
             if kw in n.lower():
-                self.color = ColorMap.get_config().imports.SuspiciousImport
+                self.color = self.suspicious_import_color
                 break
     
     @property
     def label(self) -> str:
         """
         Returns a label for this Import node.
         """
         return "Import {}".format(self.__name.lower())
     
 
 
 
 
-del Color, UniqueVertex, Vertex, logger
+del Color, ColorSetting, SizeSetting, UniqueVertex, Vertex, logger
```

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/types/imports/integration.py` & `baguette_verse-1.0.0/baguette/bakery/source/types/imports/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/types/imports/relations.py` & `baguette_verse-1.0.0/baguette/bakery/source/types/imports/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/types/network/entities.py` & `baguette_verse-1.0.0/baguette/bakery/source/types/network/entities.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from collections import defaultdict
 from typing import Optional
 
 from Viper.meta.decorators import staticproperty
 
 from ....logger import logger
+from ...config import ColorSetting, SizeSetting
 from ...colors import Color
 from ...graph import UniqueVertex, Vertex
 
 __all__ = ["Connection", "Socket", "Host"]
 
 
 
@@ -35,17 +36,20 @@
     __pickle_slots__ = {
         "duration",
         "volume",
         "src",
         "dest"
     }
 
-    def __init__(self, *, c: Color | None = None, parent: Optional[Vertex] = None) -> None:
+    default_color = ColorSetting(Color(100, 50, 255))
+    default_size = SizeSetting(1.5)
+
+    def __init__(self, *, parent: Optional[Vertex] = None) -> None:
         from typing import Any
-        super().__init__(c=c, parent=parent)
+        super().__init__(parent=parent)
         self.duration : float = 0.
         self.volume : int = 0
         self.src : Any = None
         self.dest : Any = None
 
     @property
     def socket(self) -> "Socket":
@@ -76,14 +80,17 @@
 
     __pickle_slots__ = {
         "family",
         "protocol",
         "type"
     }
 
+    default_color = ColorSetting(Color(178, 153, 153))
+    default_size = SizeSetting(2.5)
+
     families = defaultdict(lambda : ("Uncharted", "The value does not correspond to any known address family"), {
         16 : ('AppleTalk', 'AppleTalk address.'),
         22 : ('Atm', 'Native ATM services address.'),
         21 : ('Banyan', 'Banyan address.'),
         10 : ('Ccitt', 'Addresses for CCITT protocols, such as X.25.'),
         5 : ('Chaos', 'Address for MIT CHAOS protocols.'),
         24 : ('Cluster', 'Address for Microsoft cluster products.'),
@@ -149,16 +156,16 @@
         3 : ('Raw', 'Supports access to the underlying transport protocol. Using Raw, you can communicate using protocols like Internet Control Message Protocol (ProtocolType.Icmp) and Internet Group Management Protocol (ProtocolType.Igmp). Your application must provide a complete IP header when sending. Received datagrams return with the IP header and options intact.'),
         4 : ('Rdm', 'Supports connectionless, message-oriented, reliably delivered messages, and preserves message boundaries in data. Rdm (Reliably Delivered Messages) messages arrive unduplicated and in order. Furthermore, the sender is notified if messages are lost. If you initialize a Socket using Rdm, you do not require a remote host connection before sending and receiving data. With Rdm, you can communicate with multiple peers.'),
         5 : ('Seqpacket', 'Provides connection-oriented and reliable two-way transfer of ordered byte streams across a network. Seqpacket does not duplicate data, and it preserves boundaries within the data stream. A Socket of type Seqpacket communicates with a single peer and requires a remote host connection before communication can begin.'),
         1 : ('Stream', 'Supports reliable, two-way, connection-based byte streams without the duplication of data and without preservation of boundaries. A Socket of this type communicates with a single peer and requires a remote host connection before communication can begin. Stream uses the Transmission Control Protocol (ProtocolType.Tcp) and the AddressFamily.InterNetwork address family.'),
         -1 : ('Unknown', 'Specifies an unknown Socket type.'),
     })
 
-    def __init__(self, *, c: Color | None = None, parent: Optional[Vertex] = None) -> None:
-        super().__init__(c=c, parent=parent)
+    def __init__(self, *, parent: Optional[Vertex] = None) -> None:
+        super().__init__(parent=parent)
         self.family : str = ""
         self.protocol : str = ""
         self.type : str = ""
 
 
 
 
@@ -196,16 +203,19 @@
     __pickle_slots__ = {
         "address",
         "domain",
         "name",
         "platform"
     }
 
-    def __init__(self, *, c: Color | None = None, parent: Vertex | None = None) -> None:
-        super().__init__(c=c, parent=parent)
+    default_color = ColorSetting(Color.white)
+    default_size = SizeSetting(10.0)
+
+    def __init__(self, *, parent: Vertex | None = None) -> None:
+        super().__init__(parent=parent)
         self.address : str = ""
         self.domain : str = ""
         self.name : str = ""
         self.platform : str = "Unknown"
     
     @property
     def label(self) -> str:
@@ -216,8 +226,8 @@
             return "Host " + repr(self.name)
         return "Host at " + self.address
 
 
 
 
 
-del Color, Optional, UniqueVertex, Vertex, defaultdict, logger, staticproperty
+del Color, ColorSetting, SizeSetting, Optional, UniqueVertex, Vertex, defaultdict, logger, staticproperty
```

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/types/network/integration.py` & `baguette_verse-1.0.0/baguette/bakery/source/types/network/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/types/network/relations.py` & `baguette_verse-1.0.0/baguette/bakery/source/types/network/relations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 This module contains Edge and Arrow subclasses for this behavioral package.
 """
 
 from ....logger import logger
+from ...config import SwitchSetting
 from ...colors import Color
 from ...graph import Arrow, Edge, Vertex
 from ..data.entities import Data
 from ..execution.entities import Call, Process
 from .entities import Connection, Host, Socket
 
 __all__ = ["SpawnedProcess", "HasSocket", "HasConnection", "Communicates", "CreatesSocket", "Binds", "Connects", "Sends", "Receives", "Conveys", "Closes", "CloseSocket", "ListensOn", "Shutdown", "Accepts", "Duplicates"]
@@ -103,17 +104,17 @@
     }
 
     label : str = ""
 
     source : Call
     destination : Connection
 
-    def __init__(self, source: Vertex, destination: Vertex, *, c: Color | None = None, auto_write: bool = True) -> None:
+    def __init__(self, source: Vertex, destination: Vertex, *, auto_write: bool = True) -> None:
         from typing import Any
-        super().__init__(source, destination, c=c, auto_write=auto_write)
+        super().__init__(source, destination, auto_write=auto_write)
         self.src : Any = None
 
 
 
 
 
 class Connects(Edge):
@@ -131,17 +132,17 @@
     }
 
     label : str = ""
 
     source : Call
     destination : Connection
 
-    def __init__(self, source: Vertex, destination: Vertex, *, c: Color | None = None, auto_write: bool = True) -> None:
+    def __init__(self, source: Vertex, destination: Vertex, *, auto_write: bool = True) -> None:
         from typing import Any
-        super().__init__(source, destination, c=c, auto_write=auto_write)
+        super().__init__(source, destination, auto_write=auto_write)
         self.dest : Any = None
 
 
 
 
 
 class Sends(Arrow):
@@ -256,17 +257,17 @@
     __pickle_slots__ = {
         "dest"
     }
 
     source : Call
     destination : Connection
 
-    def __init__(self, source: Vertex, destination: Vertex, *, c: Color | None = None, auto_write: bool = True) -> None:
+    def __init__(self, source: Vertex, destination: Vertex, *, auto_write: bool = True) -> None:
         from typing import Any
-        super().__init__(source, destination, c=c, auto_write=auto_write)
+        super().__init__(source, destination, auto_write=auto_write)
         self.dest : Any = None
 
 
 
 
 
 class Duplicates(Arrow):
@@ -278,8 +279,8 @@
     source : Socket
     destination : Socket
 
 
 
 
 
-del Arrow, Call, Color, Connection, Data, Edge, Host, Process, Socket, Vertex, logger
+del Arrow, Call, Color, SwitchSetting, Connection, Data, Edge, Host, Process, Socket, Vertex, logger
```

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/types/registry/entities.py` & `baguette_verse-1.0.0/baguette/bakery/source/types/registry/entities.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 from abc import abstractmethod
 from types import NoneType
 from typing import Any, Callable, Generic, Optional, TypeVar
 
 from ....logger import logger
+from ...config import ColorSetting, SizeSetting
 from ...colors import Color
 from ...graph import UniqueVertex, Vertex
 
 __all__ = ["Key", "KeyEntry", "Handle"]
 
 
 
@@ -28,16 +29,22 @@
         "__name" : "The local name of the registry key int the registry tree."
     }
 
     __pickle_slots__ = {
         "name"
     }
 
-    def __init__(self, *, c: Color | None = None, parent: Vertex | None = None) -> None:
-        super().__init__(c=c, parent=parent)
+    default_color = ColorSetting(Color(0, 150, 255))
+    default_size = SizeSetting(1.5)
+
+    unprintable_key_color = ColorSetting(Color(255, 0, 50))
+    deleted_key_color = ColorSetting(Color(100, 100, 100))
+
+    def __init__(self, *, parent: Vertex | None = None) -> None:
+        super().__init__(parent=parent)
         self.__name : str = ""
 
     @property
     def name(self) -> str:
         """
         The (local) name of the registry key.
         """
@@ -50,17 +57,17 @@
         if "\\" in value:
             raise ValueError("'\\' not permitted in a registry key name")
         if len(value) > 255:
             raise ValueError("Key name is too long to be allowed by registry")
         self.__name = value.lower().title().replace("\x00", "\uFFFD")
         if not self.printable:
             from ....logger import logger
-            from ...config import ColorMap
+            from ...config import ColorSetting
             logger.info("Got an unprintable registry key.")
-            self.color = ColorMap.get_config().registry.UnprintableKey
+            self.color = self.unprintable_key_color
     
     @property
     def path(self) -> str:
         """
         The global key name (path from root key and all sub-keys to reach this key included).
         """
         if not self.parent_key:
@@ -117,16 +124,21 @@
     }
 
     __pickle_slots__ = {
         "name",
         "value"
     }
 
-    def __init__(self, *, c: Color | None = None, parent: Optional["Vertex"] = None) -> None:
-        super().__init__(c=c, parent=parent)
+    default_color = ColorSetting(Color(0, 255, 255))
+    default_size = SizeSetting(1.0)
+
+    deleted_key_entry_color = ColorSetting(Color(100, 100, 100))
+
+    def __init__(self, *, parent: Optional["Vertex"] = None) -> None:
+        super().__init__(parent=parent)
         self.__name : str = ""
 
     @property
     def name(self) -> str:
         """
         The name of this registry key entry.
         """
@@ -352,16 +364,19 @@
 
 class Handle(UniqueVertex):
 
     """
     A handle vertex. Represents a registry key handle, used when a program opens a registry key.
     """
 
-    def __init__(self, *, c: Color | None = None, parent: Optional[Vertex] = None) -> None:
-        super().__init__(c=c, parent=parent)
+    default_color = ColorSetting(Color(128, 203, 153))
+    default_size = SizeSetting(1.0)
+
+    def __init__(self, *, parent: Optional[Vertex] = None) -> None:
+        super().__init__(parent=parent)
     
     @property
     def key(self) -> Key:
         """
         Returns the key node that this handle is working on.
         """
         from .relations import UsesKey
@@ -370,8 +385,8 @@
                 return e.destination
         raise RuntimeError("Key handle with no attached key")
     
 
 
 
 
-del Any, Color, Generic, Optional, TypeVar, UniqueVertex, Vertex, logger, T, Callable, NoneType, abstractmethod
+del Any, Color, ColorSetting, SizeSetting, Generic, Optional, TypeVar, UniqueVertex, Vertex, logger, T, Callable, NoneType, abstractmethod
```

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/types/registry/integration.py` & `baguette_verse-1.0.0/baguette/bakery/source/types/registry/integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,22 +142,21 @@
 
 @chrono 
 def integrate_key_deleting(c : Call):
     """
     Marks a registry Key as deleted.
     """
     from ....logger import logger
-    from ...config import ColorMap
     if c.status == 1:
         logger.debug("Deleting registry key.")
         if c.arguments.key_handle.lower() not in __inverted_handles:
             logger.warning("Trying to delete key from unseen handle.")
             return
         k = __create_key_tree(c.arguments.regkey)
-        k.color = ColorMap.get_config().Deleted
+        k.color = k.deleted_key_color
         __existing_keys.pop(k.path.lower())
         if k not in __deleted_entries:
             __deleted_entries[k] = {}
         if k in __existing_entries:
             __deleted_entries[k].update(__existing_entries.pop(k))
 
 @chrono
@@ -273,15 +272,14 @@
 
 @chrono
 def integrate_key_value_deleting(c : Call):
     """
     Creates a KeyEntry node and marks it as deleted by a key Handle.
     """
     from ....logger import logger
-    from ...config import ColorMap
     from ...graph import Graph
     from .entities import KeyEntry
     from .relations import ChangesTowards, DeletesEntry, HasEntry
     if c.status == 1:
         logger.debug("Deleting key entry.")
         if c.arguments.key_handle.lower() not in __inverted_handles:
             logger.warning("Trying to set value with unseen key handle.")
@@ -319,15 +317,15 @@
         
         if k not in __existing_entries:
             __existing_entries[k] = {}
         __existing_entries[k][v.name] = v
         if k not in __deleted_entries:
             __deleted_entries[k] = {}
         __deleted_entries[k][v.name] = v
-        v.color = ColorMap.get_config().Deleted
+        v.color = v.deleted_key_entry_color
         if v not in sk.neighbors():
             HasEntry(sk, v)
         DeletesEntry(h, v)
```

### Comparing `baguette_verse-0.9.5/baguette/bakery/source/types/registry/relations.py` & `baguette_verse-1.0.0/baguette/bakery/source/types/registry/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9.5/baguette/croutons/extractor.py` & `baguette_verse-1.0.0/baguette/croutons/extractor.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         
         from ..bakery.logger import set_level, logger
         set_level(levels[rack.verbosity])
 
         logger.debug("Just change worker's verbosity level.")
 
         import os
-        from pickle import dump, load
+        from pickle import dump, load, UnpicklingError
         from Viper.better_threading import Future, DaemonThread
         from ..bakery.source.graph import Graph
 
         if rack.perf:
             from ..bakery.source.utils import chrono
             chrono.enabled = True
             chrono.auto_report = True
@@ -56,33 +56,53 @@
 
         result : Future[bool] = Future()
 
         def extract_main():
             
             try:
                 logger.info("Loading baguette...")
-                with rack.baguette.open("rb") as file:
-                    b = load(file)
+                try:
+                    with rack.baguette.open("rb") as file:
+                        b = load(file)
+                except UnpicklingError:
+                    rack.suppressed = True
+                    raise
+
+                if not isinstance(b, Graph):
+                    raise TypeError("Given file did not contain a Graph object")
 
                 logger.info("Loading necessary MetaGraphs...")
                 patterns, pattern_names = rack.patterns, rack.pattern_names
 
                 logger.info("Searching patterns in baguette graph...")
                 matches : dict[str, list[Graph]] = {}
 
-                for name, MG in zip(pattern_names, patterns):
-                    l = list(MG.search_iter(b))
+                for i, (name, MG) in enumerate(zip(pattern_names, patterns)):
+                    l = []
+                    for match in MG.search_iter(b):
+                        l.append(match)
+                        if rack.paint_color:
+                            match.paint(rack.paint_color[i])
                     if l:
                         matches[name] = l
 
                 logger.info("Exporting {} matches to file '{}'...".format(sum(len(l) for l in matches.values()), rack.extracted))
                 rack.extracted.parent.mkdir(parents = True, exist_ok = True)
                 with open(rack.extracted, "wb") as file:
                     dump(matches, file)
 
+                if matches and rack.paint_color:
+                    logger.info("Exporting visual with colors")
+                    for i, (f, name) in enumerate(zip(rack.filters, rack.filter_names)):
+                        logger.info("Applying filters {}/{} : {}".format(i + 1, len(rack.filters), name))
+                        f.apply(b)
+                    logger.info("Exporting to .gexf")
+                    rack.visual.parent.mkdir(parents = True, exist_ok = True)
+                    b.export(str(rack.visual))
+
                 result.set(True)
                 logger.info("Done !")
             except BaseException as e:
                 result.set_exception(e)
 
         def death_timer():
             from time import sleep
```

### Comparing `baguette_verse-0.9.5/baguette/croutons/metalib/evaluator.py` & `baguette_verse-1.0.0/baguette/croutons/metalib/evaluator.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9.5/baguette/croutons/metalib/interact.py` & `baguette_verse-1.0.0/baguette/croutons/metalib/interact.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9.5/baguette/croutons/metalib/utils.py` & `baguette_verse-1.0.0/baguette/croutons/metalib/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9.5/baguette/croutons/source/metagraph.py` & `baguette_verse-1.0.0/baguette/croutons/source/metagraph.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,76 +35,70 @@
     }
 
     __pickle_slots__ = {
         "cls",
         "condition"
     }
 
-    def __init__(self, *, c: Color | None = None, parent: Optional[Vertex] = None) -> None:
+    def __init__(self, *, parent: Optional[Vertex] = None) -> None:
         from ...bakery.source.colors import Color
-        super().__init__(c=c, parent=parent)
-        self.__class : type[Vertex] = Vertex
+        super().__init__(parent=parent)
+        self.__class : tuple[type[Vertex], ...] = (Vertex, )
         self.__condition : Callable[[Vertex], bool] | bool = True
-        self.__color : Color | None = c
+        self.__color : Color | None = None
         self.edges : set[MetaEdge]
 
     @property
     def color(self) -> Color:
         """
         The color of this MetaVertex. Defaults to the average of the colors of all its Vertex classes.
         """
         from ...bakery.source.colors import Color
-        from ...bakery.source.config import ColorMap
-        if self.__color !=  None:
+        if self.__color is not None:
             return self.__color
-        if isinstance(self.cls, type):
-            if not hasattr(self.cls, "color") or not isinstance(self.cls.color, Color):
-                return ColorMap.get_config().get_color(self.cls)
-            return self.cls.color
-        else:
-            return Color.average(*[(cls.color if hasattr(cls, "color") and isinstance(cls.color, Color) else ColorMap.get_config().get_color(cls)) for cls in self.cls.__args__])
+        return Color.average(*[(cls.default_color) for cls in self.cls])
     
     @color.setter
     def color(self, c : Color):
         from ...bakery.source.colors import Color
         if not isinstance(c, Color):
             raise TypeError("Expected Color, got " + repr(type(c).__name__))
         self.__color = c
+
+    @color.deleter
+    def color(self):
+        self.__color = None
     
     @property
-    def cls(self) -> type[Vertex]:
+    def cls(self) -> tuple[type[Vertex], ...]:
         """
-        The class that his vertex represents.
+        The classes that this vertex represents.
         """
         return self.__class
     
     @cls.setter
-    def cls(self, cls : type[Vertex]):
+    def cls(self, cls : type[Vertex] | tuple[type[Vertex], ...]):
         """
-        Sets the class associated with this vertex.
+        Sets the class(es) associated with this vertex.
         """
-        from typing import _UnionGenericAlias
-        from types import UnionType
-        from .utils import class_union
         from ...bakery.source.graph import Vertex
         if isinstance(cls, type) and issubclass(cls, Vertex):
-            self.__class = cls
-        elif isinstance(cls, _UnionGenericAlias):
-            cls = class_union(*cls.__args__)
-            for c in cls.__args__:
-                if not isinstance(c, type) or not issubclass(c, Vertex):
-                    raise TypeError("Expected subclasses of Vertex , got " + repr(c))
-            self.__class = cls
-        elif isinstance(cls, UnionType):
-            for c in cls.__args__:
+            self.__class = (cls, )
+        elif isinstance(cls, tuple):
+            for c in cls:
                 if not isinstance(c, type) or not issubclass(c, Vertex):
-                    raise TypeError("Expected subclasses of Vertex , got " + repr(c))
+                    raise TypeError("Expected subclass of Vertex or tuple of subclasses, got a " + repr(c))
             self.__class = cls
         else:
-            raise TypeError("Expected subclass of Vertex , got " + repr(cls))
+            raise TypeError("Expected subclass of Vertex or tuple of subclasses, got " + repr(cls))
+    
+    @cls.deleter
+    def cls(self):
+        from ...bakery.source.graph import Vertex
+        self.__class = (Vertex, )
 
     @property
     def condition(self) -> Callable[[Vertex], bool] | bool:
         """
         An additional condition to check when trying to match a Vertex to this MetaVertex.
         """
         return self.__condition
@@ -113,29 +107,30 @@
     def condition(self, cond : Callable[[Vertex], bool] | bool):
         """
         Sets the additional condition function for this MetaVertex.
         """
         if not callable(cond) and not isinstance(cond, bool):
             raise TypeError("Expected callable or bool, got " + repr(type(cond).__name__))
         self.__condition = cond
+
+    @condition.deleter
+    def condition(self):
+        self.__condition = True
     
     def match(self, v : Vertex) -> bool:
         """
         Returns True if the Vertex v has a matching type.
         """
         return isinstance(v, self.__class) and (self.__condition(v) if callable(self.__condition) else self.__condition)
     
     def __get_cls_str(self) -> str:
         """
         Returns a string to display the class of a MetaVertex.
         """
-        if isinstance(self.__class, type):
-            return self.__class.__name__
-        else:
-            return str(self.__class)
+        return " | ".join(c.__name__ for c in self.__class)
 
     @property
     def label(self) -> str:
         return "Vertex[" + self.__get_cls_str() + "]" + ("{" + str(self.__condition) + "}" if callable(self.__condition) else "")
 
     def __str__(self) -> str:
         return type(self).__name__ + "[" + self.__get_cls_str() + "]" + ("*" if callable(self.__condition) else "")
@@ -153,85 +148,85 @@
     This class describes a type edge. One or multiple Edge subclasses can be associated to it.
     Note that a MetaEdge can represent a subclass of Arrow and in this case, the match can be made in both directions.
     """
 
     __slots__ = {
         "__class" : "The class that this MetaEdge represents.",
         "__condition" : "An additional condition function. Takes an Edge as an input and tells whether or not it can be a valid match (does not need to check type)",
-        "__color" : "The Color forcefully set to this MetaVertex."
+        "__color" : "The Color forcefully set to this MetaEdge."
     }
 
     __pickle_slots__ = {
         "cls",
         "condition"
     }
 
-    def __init__(self, source: MetaVertex, destination: MetaVertex, *, c: Color | None = None, auto_write: bool = True) -> None:
+    def __init__(self, source: MetaVertex, destination: MetaVertex, *, auto_write: bool = True) -> None:
         from ...bakery.source.colors import Color
         if not isinstance(source, MetaVertex) or not isinstance(destination, MetaVertex):
             raise TypeError("Expected two MetaVertices, got " + repr(type(source).__name__) + " and " + repr(type(destination).__name__))
-        super().__init__(source, destination, c=c, auto_write=auto_write)
-        self.__class : type[Edge] = Edge
+        super().__init__(source, destination, auto_write=auto_write)
+        self.__class : tuple[type[Edge], ...] = (Edge, )
         self.__condition : Callable[[Edge], bool] | bool = True
-        self.__color : Color | None = c
+        self.__color : Color | None = None
         self.source : MetaVertex
         self.destination : MetaVertex
 
     @property
     def color(self) -> Color:
         """
         The color of this MetaEdge. Defaults to the average of the colors of all its Edge classes.
         """
         from ...bakery.source.colors import Color
-        from ...bakery.source.config import ColorMap
-        if self.__color !=  None:
+        if self.__color != None:
             return self.__color
-        if isinstance(self.cls, type):
-            if not hasattr(self.cls, "color") or not isinstance(self.cls.color, Color):
-                return ColorMap.get_config().get_color(self.cls)
-            return self.cls.color
+        edge_colors = [cls.default_color for cls in self.cls if not cls.blend_vertices_colors]
+        if edge_colors:
+            return Color.average(*edge_colors)
         else:
-            return Color.average(*[(cls.color if hasattr(cls, "color") and isinstance(cls.color, Color) else ColorMap.get_config().get_color(cls)) for cls in self.cls.__args__])
+            return Color.average(self.source.color, self.destination.color)
     
     @color.setter
     def color(self, c : Color):
         from ...bakery.source.colors import Color
         if not isinstance(c, Color):
             raise TypeError("Expected Color, got " + repr(type(c).__name__))
         self.__color = c
+
+    @color.deleter
+    def color(self):
+        self.__color = None
     
     @property
-    def cls(self) -> type[Edge]:
+    def cls(self) -> tuple[type[Edge], ...]:
         """
-        The class that his edge represents.
+        The classes that this edge represents.
         """
         return self.__class
     
     @cls.setter
-    def cls(self, cls : type[Edge]):
+    def cls(self, cls : type[Edge] | tuple[type[Edge], ...]):
         """
-        Sets the class associated with this edge.
+        Sets the class(es) associated with this edge.
         """
-        from typing import _UnionGenericAlias
-        from types import UnionType
-        from .utils import class_union
         from ...bakery.source.graph import Edge
         if isinstance(cls, type) and issubclass(cls, Edge):
-            self.__class = cls
-        elif isinstance(cls, _UnionGenericAlias):
-            cls = class_union(*cls.__args__)
-            for c in cls.__args__:
-                if not isinstance(c, type) or not issubclass(c, Edge):
-                    raise TypeError("Expected subclasses of Edge , got " + repr(c))
-            self.__class = cls
-        elif isinstance(cls, UnionType):
-            for c in cls.__args__:
+            self.__class = (cls, )
+        elif isinstance(cls, tuple):
+            for c in cls:
                 if not isinstance(c, type) or not issubclass(c, Edge):
-                    raise TypeError("Expected subclasses of Edge , got " + repr(c))
+                    raise TypeError("Expected subclasses of Edge or tuple of subclasses, got a " + repr(c))
             self.__class = cls
+        else:
+            raise TypeError("Expected subclass of Edge or tuple of subclasses, got " + repr(cls))
+        
+    @cls.deleter
+    def cls(self):
+        from ...bakery.source.graph import Edge
+        self.__class = (Edge, )
         
     @property
     def condition(self) -> Callable[[Edge], bool] | bool:
         """
         An additional condition to check when trying to match an Edge to this MetaEdge.
         """
         return self.__condition
@@ -241,42 +236,43 @@
         """
         Sets the additional condition function for this MetaEdge.
         """
         if not callable(cond) and not isinstance(cond, bool):
             raise TypeError("Expected callable or bool, got " + repr(type(cond).__name__))
         self.__condition = cond
     
+    @condition.deleter
+    def condition(self):
+        self.__condition = True
+    
     def match(self, e : Edge) -> bool:
         """
         Returns True if the Egde e has a matching type.
         """
         return isinstance(e, self.__class) and (self.__condition(e) if callable(self.__condition) else self.__condition)
     
     def __get_cls_str(self) -> str:
         """
         Returns a string to display the class of a MetaEdge.
         """
-        if isinstance(self.__class, type):
-            return self.__class.__name__
-        else:
-            return str(self.__class)
+        return " | ".join(c.__name__ for c in self.cls)
 
     @property
     def label(self) -> str:
         return "Edge[" + self.__get_cls_str() + "]" + ("{" + str(self.__condition) + "}" if callable(self.__condition) else "")
 
     def __str__(self) -> str:
         return type(self).__name__ + "[" + self.__get_cls_str() + "]" + ("*" if callable(self.__condition) else "")
     
     def __repr__(self) -> str:
         return type(self).__name__ + "[" + self.__get_cls_str() + "]" + ("{" + str(self.__condition) + "}" if callable(self.__condition) else "")
 
-    def __getitem__(self, cls : type[Edge]) -> Self:
+    def __getitem__(self, cls : type[Edge] | tuple[type[Edge], ...]) -> Self:
         try:
-            self.__class = cls
+            self.cls = cls
             return self
         except BaseException as E:
             raise E from None
 
 
 
 
@@ -292,96 +288,92 @@
     }
 
     __pickle_slots__ = {
         "cls",
         "condition"
     }
 
-    def __init__(self, source: MetaVertex, destination: MetaVertex, *, c: Color | None = None, auto_write: bool = True) -> None:
-        super().__init__(source, destination, c=c, auto_write=auto_write)
-        self.__class : type[Arrow] = Arrow
+    def __init__(self, source: MetaVertex, destination: MetaVertex, *, auto_write: bool = True) -> None:
+        from ...bakery.source.graph import Arrow
+        super().__init__(source, destination, auto_write=auto_write)
+        self.__class : tuple[type[Arrow], ...] = (Arrow, )
         self.__condition : Callable[[Arrow], bool] | bool = True
-    
+
     @property
-    def cls(self) -> type[Arrow]:
+    def cls(self) -> tuple[type[Arrow], ...]:
         """
-        The class that his arrow represents.
+        The classes that this arrow represents.
         """
         return self.__class
     
     @cls.setter
-    def cls(self, cls : type[Arrow]):
+    def cls(self, cls : type[Arrow] | tuple[type[Arrow], ...]):
         """
-        Sets the class associated with this arrow.
+        Sets the class(es) associated with this arrow.
         """
-        from typing import _UnionGenericAlias
-        from types import UnionType
-        from .utils import class_union
         from ...bakery.source.graph import Arrow
         if isinstance(cls, type) and issubclass(cls, Arrow):
-            self.__class = cls
-        elif isinstance(cls, _UnionGenericAlias):
-            cls = class_union(*cls.__args__)
-            for c in cls.__args__:
-                if not isinstance(c, type) or not issubclass(c, Arrow):
-                    raise TypeError("Expected subclasses of Arrow , got " + repr(c))
-            self.__class = cls
-        elif isinstance(cls, UnionType):
-            for c in cls.__args__:
+            self.__class = (cls, )
+        elif isinstance(cls, tuple):
+            for c in cls:
                 if not isinstance(c, type) or not issubclass(c, Arrow):
-                    raise TypeError("Expected subclasses of Arrow , got " + repr(c))
+                    raise TypeError("Expected subclasses of Arrow or tuple of subclasses, got a " + repr(c))
             self.__class = cls
-
+        else:
+            raise TypeError("Expected subclass of Arrow or tuple of subclasses, got " + repr(cls))
+        
+    @cls.deleter
+    def cls(self):
+        from ...bakery.source.graph import Arrow
+        self.__class = (Arrow, )
+        
     @property
     def condition(self) -> Callable[[Arrow], bool] | bool:
         """
-        An additional condition to check when trying to match an Arrow to this MetaArrow.
+        An additional condition to check when trying to match an Edge to this MetaEdge.
         """
         return self.__condition
     
     @condition.setter
     def condition(self, cond : Callable[[Arrow], bool] | bool):
         """
-        Sets the additional condition function for this MetaArrow.
+        Sets the additional condition function for this MetaEdge.
         """
         if not callable(cond) and not isinstance(cond, bool):
             raise TypeError("Expected callable or bool, got " + repr(type(cond).__name__))
         self.__condition = cond
     
-    def match(self, a : Edge) -> bool:
+    @condition.deleter
+    def condition(self):
+        self.__condition = True
+    
+    def match(self, a : Arrow) -> bool:
         """
         Returns True if the Arrow a has a matching type.
         """
         return isinstance(a, self.__class) and (self.__condition(a) if callable(self.__condition) else self.__condition)
 
     def __get_cls_str(self) -> str:
         """
         Returns a string to display the class of a MetaArrow.
         """
-        if isinstance(self.__class, type):
-            return self.__class.__name__
-        else:
-            return str(self.__class)
+        return " | ".join(c.__name__ for c in self.cls)
 
     @property
     def label(self) -> str:
         return "Arrow[" + self.__get_cls_str() + "]" + ("{" + str(self.__condition) + "}" if callable(self.__condition) else "")
     
     def __str__(self) -> str:
         return type(self).__name__ + "[" + self.__get_cls_str() + "]" + ("*" if callable(self.__condition) else "")
     
     def __repr__(self) -> str:
         return type(self).__name__ + "[" + self.__get_cls_str() + "]" + ("{" + str(self.__condition) + "}" if callable(self.__condition) else "")
     
-    def __getitem__(self, cls : type[Arrow]) -> Self:
-        try:
-            self.__class = cls
-            return self
-        except BaseException as E:
-            raise E from None
+    def __getitem__(self, cls : type[Arrow] | tuple[type[Arrow], ...]) -> Self:
+        return super().__getitem__(cls)
     
 
 
 
 
 class MetaGraph(Graph):
```

### Comparing `baguette_verse-0.9.5/baguette/croutons/source/utils.py` & `baguette_verse-1.0.0/baguette/croutons/source/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9.5/.gitignore` & `baguette_verse-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9.5/LICENSE` & `baguette_verse-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9.5/README.md` & `baguette_verse-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `baguette_verse-0.9.5/pyproject.toml` & `baguette_verse-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "baguette-verse"
-version = "0.9.5"
+version = "1.0.0"
 authors = [
   { name="Vincent Raulin", email="vincent.raulin@inria.fr" },
 ]
 description = "A malware behavioral analysis framework centered around BAGUETTE!"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
```

### Comparing `baguette_verse-0.9.5/PKG-INFO` & `baguette_verse-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baguette-verse
-Version: 0.9.5
+Version: 1.0.0
 Summary: A malware behavioral analysis framework centered around BAGUETTE!
 Project-URL: Repository, https://gitlab.inria.fr/vraulin/baguette-verse
 Project-URL: Bug Tracker, https://gitlab.inria.fr/vraulin/baguette-verse/-/issues
 Author-email: Vincent Raulin <vincent.raulin@inria.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
```


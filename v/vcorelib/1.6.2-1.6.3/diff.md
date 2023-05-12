# Comparing `tmp/vcorelib-1.6.2.tar.gz` & `tmp/vcorelib-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcorelib-1.6.2.tar", last modified: Mon May  8 06:04:05 2023, max compression
+gzip compressed data, was "vcorelib-1.6.3.tar", last modified: Fri May 12 03:22:46 2023, max compression
```

## Comparing `vcorelib-1.6.2.tar` & `vcorelib-1.6.3.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:04:05.621438 vcorelib-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-08 06:02:27.000000 vcorelib-1.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-08 06:04:05.621438 vcorelib-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-08 06:02:27.000000 vcorelib-1.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-08 06:02:27.000000 vcorelib-1.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 06:04:05.621438 vcorelib-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-08 06:02:27.000000 vcorelib-1.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:04:05.613438 vcorelib-1.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-08 06:02:27.000000 vcorelib-1.6.2/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-08 06:02:27.000000 vcorelib-1.6.2/tests/test_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-08 06:02:27.000000 vcorelib-1.6.2/tests/test_namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:04:05.613438 vcorelib-1.6.2/vcorelib/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:04:05.613438 vcorelib-1.6.2/vcorelib/args/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/args/newline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:04:05.613438 vcorelib-1.6.2/vcorelib/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/asyncio/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/asyncio/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:04:05.617438 vcorelib-1.6.2/vcorelib/dict/
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/dict/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/dict/codec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/dict/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/dict/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:04:05.617438 vcorelib-1.6.2/vcorelib/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/graph/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/graph/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/graph/port.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:04:05.617438 vcorelib-1.6.2/vcorelib/io/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/io/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:04:05.617438 vcorelib-1.6.2/vcorelib/io/arbiter/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/io/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/io/arbiter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/io/arbiter/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/io/arbiter/directory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:04:05.617438 vcorelib-1.6.2/vcorelib/io/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/io/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/io/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/io/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/io/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/io/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/io/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:04:05.617438 vcorelib-1.6.2/vcorelib/math/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/math/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:04:05.617438 vcorelib-1.6.2/vcorelib/math/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/math/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/math/analysis/average.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:04:05.617438 vcorelib-1.6.2/vcorelib/math/analysis/rate/
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/math/analysis/rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/math/analysis/rate/limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/math/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:04:05.621438 vcorelib-1.6.2/vcorelib/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/paths/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/paths/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/paths/info_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:04:05.621438 vcorelib-1.6.2/vcorelib/platform/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:04:05.621438 vcorelib-1.6.2/vcorelib/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/schemas/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/schemas/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:04:05.621438 vcorelib-1.6.2/vcorelib/script/
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:04:05.621438 vcorelib-1.6.2/vcorelib/target/
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/target/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/target/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/target/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/target/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:04:05.621438 vcorelib-1.6.2/vcorelib/task/
--rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:04:05.621438 vcorelib-1.6.2/vcorelib/task/dict/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/task/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/task/dict/melder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/task/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:04:05.621438 vcorelib-1.6.2/vcorelib/task/subprocess/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/task/subprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/task/subprocess/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:04:05.621438 vcorelib-1.6.2/vcorelib/task/time/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/task/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-08 06:02:27.000000 vcorelib-1.6.2/vcorelib/task/time/sleep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 06:04:05.613438 vcorelib-1.6.2/vcorelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-08 06:04:05.000000 vcorelib-1.6.2/vcorelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-08 06:04:05.000000 vcorelib-1.6.2/vcorelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 06:04:05.000000 vcorelib-1.6.2/vcorelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-08 06:04:05.000000 vcorelib-1.6.2/vcorelib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 06:04:05.000000 vcorelib-1.6.2/vcorelib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:22:46.664836 vcorelib-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-12 03:21:29.000000 vcorelib-1.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-12 03:22:46.664836 vcorelib-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-12 03:21:29.000000 vcorelib-1.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-12 03:21:29.000000 vcorelib-1.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 03:22:46.664836 vcorelib-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-12 03:21:29.000000 vcorelib-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:22:46.656836 vcorelib-1.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-12 03:21:29.000000 vcorelib-1.6.3/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-12 03:21:29.000000 vcorelib-1.6.3/tests/test_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-12 03:21:29.000000 vcorelib-1.6.3/tests/test_namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:22:46.660836 vcorelib-1.6.3/vcorelib/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:22:46.660836 vcorelib-1.6.3/vcorelib/args/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/args/newline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:22:46.660836 vcorelib-1.6.3/vcorelib/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/asyncio/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/asyncio/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:22:46.660836 vcorelib-1.6.3/vcorelib/dict/
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/dict/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/dict/codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/dict/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/dict/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:22:46.660836 vcorelib-1.6.3/vcorelib/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/graph/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/graph/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/graph/port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:22:46.660836 vcorelib-1.6.3/vcorelib/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/io/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:22:46.660836 vcorelib-1.6.3/vcorelib/io/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/io/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/io/arbiter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/io/arbiter/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/io/arbiter/directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:22:46.664836 vcorelib-1.6.3/vcorelib/io/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/io/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/io/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/io/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/io/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/io/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/io/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:22:46.664836 vcorelib-1.6.3/vcorelib/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/math/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:22:46.664836 vcorelib-1.6.3/vcorelib/math/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/math/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/math/analysis/average.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:22:46.664836 vcorelib-1.6.3/vcorelib/math/analysis/rate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/math/analysis/rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/math/analysis/rate/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/math/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:22:46.664836 vcorelib-1.6.3/vcorelib/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/paths/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/paths/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/paths/info_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:22:46.664836 vcorelib-1.6.3/vcorelib/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:22:46.664836 vcorelib-1.6.3/vcorelib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/schemas/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/schemas/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:22:46.664836 vcorelib-1.6.3/vcorelib/script/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:22:46.664836 vcorelib-1.6.3/vcorelib/target/
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/target/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/target/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/target/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/target/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:22:46.664836 vcorelib-1.6.3/vcorelib/task/
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:22:46.664836 vcorelib-1.6.3/vcorelib/task/dict/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/task/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/task/dict/melder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/task/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:22:46.664836 vcorelib-1.6.3/vcorelib/task/subprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/task/subprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/task/subprocess/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:22:46.664836 vcorelib-1.6.3/vcorelib/task/time/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/task/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-12 03:21:29.000000 vcorelib-1.6.3/vcorelib/task/time/sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 03:22:46.660836 vcorelib-1.6.3/vcorelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-12 03:22:46.000000 vcorelib-1.6.3/vcorelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-12 03:22:46.000000 vcorelib-1.6.3/vcorelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 03:22:46.000000 vcorelib-1.6.3/vcorelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-12 03:22:46.000000 vcorelib-1.6.3/vcorelib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 03:22:46.000000 vcorelib-1.6.3/vcorelib.egg-info/top_level.txt
```

### Comparing `vcorelib-1.6.2/LICENSE` & `vcorelib-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/PKG-INFO` & `vcorelib-1.6.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 1.6.2
+Version: 1.6.3
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=cca40b35b424697e8e46bfdcaeb25b87
+    hash=ec5ffc72419ba7fbcac519669f59c236
     =====================================
 -->
 
-# vcorelib ([1.6.2](https://pypi.org/project/vcorelib/))
+# vcorelib ([1.6.3](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-1.6.2/README.md` & `vcorelib-1.6.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=cca40b35b424697e8e46bfdcaeb25b87
+    hash=ec5ffc72419ba7fbcac519669f59c236
     =====================================
 -->
 
-# vcorelib ([1.6.2](https://pypi.org/project/vcorelib/))
+# vcorelib ([1.6.3](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-1.6.2/pyproject.toml` & `vcorelib-1.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "vcorelib"
-version = "1.6.2"
+version = "1.6.3"
 description = "A collection of core Python utilities."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `vcorelib-1.6.2/setup.py` & `vcorelib-1.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/tests/test_logging.py` & `vcorelib-1.6.3/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/tests/test_names.py` & `vcorelib-1.6.3/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/tests/test_namespace.py` & `vcorelib-1.6.3/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/args/__init__.py` & `vcorelib-1.6.3/vcorelib/args/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/args/newline.py` & `vcorelib-1.6.3/vcorelib/args/newline.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/asyncio/__init__.py` & `vcorelib-1.6.3/vcorelib/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/asyncio/cli.py` & `vcorelib-1.6.3/vcorelib/asyncio/cli.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/asyncio/subprocess.py` & `vcorelib-1.6.3/vcorelib/asyncio/subprocess.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/dict/__init__.py` & `vcorelib-1.6.3/vcorelib/dict/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/dict/cache.py` & `vcorelib-1.6.3/vcorelib/dict/cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/dict/codec.py` & `vcorelib-1.6.3/vcorelib/dict/codec.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/dict/config.py` & `vcorelib-1.6.3/vcorelib/dict/config.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/dict/env.py` & `vcorelib-1.6.3/vcorelib/dict/env.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/graph/__init__.py` & `vcorelib-1.6.3/vcorelib/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/graph/abc.py` & `vcorelib-1.6.3/vcorelib/graph/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/graph/edge.py` & `vcorelib-1.6.3/vcorelib/graph/edge.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/graph/node.py` & `vcorelib-1.6.3/vcorelib/graph/node.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/graph/port.py` & `vcorelib-1.6.3/vcorelib/graph/port.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/io/__init__.py` & `vcorelib-1.6.3/vcorelib/io/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/io/abc.py` & `vcorelib-1.6.3/vcorelib/io/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/io/arbiter/base.py` & `vcorelib-1.6.3/vcorelib/io/arbiter/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/io/arbiter/context.py` & `vcorelib-1.6.3/vcorelib/io/arbiter/context.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/io/arbiter/directory.py` & `vcorelib-1.6.3/vcorelib/io/arbiter/directory.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/io/archive/__init__.py` & `vcorelib-1.6.3/vcorelib/io/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/io/cache.py` & `vcorelib-1.6.3/vcorelib/io/cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/io/decode.py` & `vcorelib-1.6.3/vcorelib/io/decode.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/io/encode.py` & `vcorelib-1.6.3/vcorelib/io/encode.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/io/mapping.py` & `vcorelib-1.6.3/vcorelib/io/mapping.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/io/types.py` & `vcorelib-1.6.3/vcorelib/io/types.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/logging.py` & `vcorelib-1.6.3/vcorelib/logging.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/math/__init__.py` & `vcorelib-1.6.3/vcorelib/math/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/math/analysis/average.py` & `vcorelib-1.6.3/vcorelib/math/analysis/average.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/math/analysis/rate/__init__.py` & `vcorelib-1.6.3/vcorelib/math/analysis/rate/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/math/analysis/rate/limiter.py` & `vcorelib-1.6.3/vcorelib/math/analysis/rate/limiter.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/math/time.py` & `vcorelib-1.6.3/vcorelib/math/time.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/names.py` & `vcorelib-1.6.3/vcorelib/names.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/namespace.py` & `vcorelib-1.6.3/vcorelib/namespace.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/paths/__init__.py` & `vcorelib-1.6.3/vcorelib/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/paths/context.py` & `vcorelib-1.6.3/vcorelib/paths/context.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/paths/info.py` & `vcorelib-1.6.3/vcorelib/paths/info.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/paths/info_cache.py` & `vcorelib-1.6.3/vcorelib/paths/info_cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/platform/__init__.py` & `vcorelib-1.6.3/vcorelib/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/schemas/__init__.py` & `vcorelib-1.6.3/vcorelib/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/schemas/base.py` & `vcorelib-1.6.3/vcorelib/schemas/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/schemas/json.py` & `vcorelib-1.6.3/vcorelib/schemas/json.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/schemas/mixins.py` & `vcorelib-1.6.3/vcorelib/schemas/mixins.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/script/__init__.py` & `vcorelib-1.6.3/vcorelib/script/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,28 +2,35 @@
 A module for working with external scripts.
 """
 
 # built-in
 import importlib.machinery
 import importlib.util
 from pathlib import Path as _Path
+from sys import path as _path
 from typing import Any as _Any
 from typing import Set as _Set
 
 # internal
 from vcorelib.paths import Pathlike as _Pathlike
 from vcorelib.paths import normalize as _normalize
 
 
 def invoke_script(script: _Pathlike, method: str, *args, **kwargs) -> _Any:
     """Invoke a method from an external script."""
 
-    loader = importlib.machinery.SourceFileLoader(
-        "script", str(_normalize(script))
-    )
+    path = _normalize(script)
+
+    # Add the parent directory to the system path so that the external script
+    # can load adjacent modules.
+    parent = str(path.parent.resolve())
+    if parent not in _path:
+        _path.append(parent)
+
+    loader = importlib.machinery.SourceFileLoader("script", str(path))
     spec = importlib.util.spec_from_loader("script", loader)
     assert spec is not None
     script_module = importlib.util.module_from_spec(spec)
     loader.exec_module(script_module)
 
     # Invoke the script method.
     return getattr(script_module, method)(*args, **kwargs)
```

### Comparing `vcorelib-1.6.2/vcorelib/target/__init__.py` & `vcorelib-1.6.3/vcorelib/target/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/target/evaluation.py` & `vcorelib-1.6.3/vcorelib/target/evaluation.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/target/expression.py` & `vcorelib-1.6.3/vcorelib/target/expression.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/target/resolver.py` & `vcorelib-1.6.3/vcorelib/target/resolver.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/task/__init__.py` & `vcorelib-1.6.3/vcorelib/task/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/task/dict/melder.py` & `vcorelib-1.6.3/vcorelib/task/dict/melder.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/task/manager.py` & `vcorelib-1.6.3/vcorelib/task/manager.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/task/subprocess/run.py` & `vcorelib-1.6.3/vcorelib/task/subprocess/run.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib/task/time/sleep.py` & `vcorelib-1.6.3/vcorelib/task/time/sleep.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.2/vcorelib.egg-info/PKG-INFO` & `vcorelib-1.6.3/vcorelib.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 1.6.2
+Version: 1.6.3
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=cca40b35b424697e8e46bfdcaeb25b87
+    hash=ec5ffc72419ba7fbcac519669f59c236
     =====================================
 -->
 
-# vcorelib ([1.6.2](https://pypi.org/project/vcorelib/))
+# vcorelib ([1.6.3](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-1.6.2/vcorelib.egg-info/SOURCES.txt` & `vcorelib-1.6.3/vcorelib.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/aqueduct-1.8.1.tar.gz` & `tmp/aqueduct-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqueduct-1.8.1.tar", last modified: Tue Nov 16 08:14:45 2021, max compression
+gzip compressed data, was "aqueduct-1.9.0.tar", last modified: Mon Nov 22 11:00:59 2021, max compression
```

## Comparing `aqueduct-1.8.1.tar` & `aqueduct-1.9.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 bugrimov   (503) staff       (20)        0 2021-11-16 08:14:45.443084 aqueduct-1.8.1/
--rw-r--r--   0 bugrimov   (503) staff       (20)     6915 2021-11-16 08:14:45.442811 aqueduct-1.8.1/PKG-INFO
--rw-r--r--   0 bugrimov   (503) staff       (20)     5835 2021-09-30 14:31:22.000000 aqueduct-1.8.1/README.rst
-drwxr-xr-x   0 bugrimov   (503) staff       (20)        0 2021-11-16 08:14:45.431502 aqueduct-1.8.1/aqueduct/
--rw-r--r--   0 bugrimov   (503) staff       (20)      153 2021-11-16 08:12:58.000000 aqueduct-1.8.1/aqueduct/__init__.py
--rw-r--r--   0 bugrimov   (503) staff       (20)      324 2021-09-02 13:20:17.000000 aqueduct-1.8.1/aqueduct/exceptions.py
--rw-r--r--   0 bugrimov   (503) staff       (20)    10090 2021-10-15 17:26:57.000000 aqueduct-1.8.1/aqueduct/flow.py
--rw-r--r--   0 bugrimov   (503) staff       (20)     1011 2021-09-02 13:20:17.000000 aqueduct-1.8.1/aqueduct/handler.py
-drwxr-xr-x   0 bugrimov   (503) staff       (20)        0 2021-11-16 08:14:45.433951 aqueduct-1.8.1/aqueduct/integrations/
--rw-r--r--   0 bugrimov   (503) staff       (20)        0 2021-09-27 22:16:38.000000 aqueduct-1.8.1/aqueduct/integrations/__init__.py
--rw-r--r--   0 bugrimov   (503) staff       (20)     1881 2021-10-15 17:26:57.000000 aqueduct-1.8.1/aqueduct/integrations/aiohttp.py
--rw-r--r--   0 bugrimov   (503) staff       (20)      301 2021-09-02 13:20:17.000000 aqueduct-1.8.1/aqueduct/logger.py
-drwxr-xr-x   0 bugrimov   (503) staff       (20)        0 2021-11-16 08:14:45.436093 aqueduct-1.8.1/aqueduct/metrics/
--rw-r--r--   0 bugrimov   (503) staff       (20)      105 2021-09-02 13:20:17.000000 aqueduct-1.8.1/aqueduct/metrics/__init__.py
--rw-r--r--   0 bugrimov   (503) staff       (20)     1119 2021-09-02 13:20:17.000000 aqueduct-1.8.1/aqueduct/metrics/base.py
--rw-r--r--   0 bugrimov   (503) staff       (20)     2319 2021-09-02 13:20:17.000000 aqueduct-1.8.1/aqueduct/metrics/collect.py
--rw-r--r--   0 bugrimov   (503) staff       (20)     2570 2021-09-02 13:20:17.000000 aqueduct-1.8.1/aqueduct/metrics/export.py
--rw-r--r--   0 bugrimov   (503) staff       (20)     1287 2021-09-02 13:20:17.000000 aqueduct-1.8.1/aqueduct/metrics/manager.py
--rw-r--r--   0 bugrimov   (503) staff       (20)     1362 2021-09-02 13:20:17.000000 aqueduct-1.8.1/aqueduct/metrics/task.py
--rw-r--r--   0 bugrimov   (503) staff       (20)      878 2021-09-02 13:20:17.000000 aqueduct-1.8.1/aqueduct/metrics/timer.py
--rw-r--r--   0 bugrimov   (503) staff       (20)     7180 2021-09-02 13:20:17.000000 aqueduct-1.8.1/aqueduct/multiprocessing.py
--rw-r--r--   0 bugrimov   (503) staff       (20)     8284 2021-11-16 08:12:58.000000 aqueduct-1.8.1/aqueduct/shm.py
--rw-r--r--   0 bugrimov   (503) staff       (20)     2098 2021-09-02 13:20:17.000000 aqueduct-1.8.1/aqueduct/task.py
--rw-r--r--   0 bugrimov   (503) staff       (20)     5178 2021-10-15 17:26:57.000000 aqueduct-1.8.1/aqueduct/worker.py
-drwxr-xr-x   0 bugrimov   (503) staff       (20)        0 2021-11-16 08:14:45.433237 aqueduct-1.8.1/aqueduct.egg-info/
--rw-r--r--   0 bugrimov   (503) staff       (20)     6915 2021-11-16 08:14:45.000000 aqueduct-1.8.1/aqueduct.egg-info/PKG-INFO
--rw-r--r--   0 bugrimov   (503) staff       (20)     1516 2021-11-16 08:14:45.000000 aqueduct-1.8.1/aqueduct.egg-info/SOURCES.txt
--rw-r--r--   0 bugrimov   (503) staff       (20)        1 2021-11-16 08:14:45.000000 aqueduct-1.8.1/aqueduct.egg-info/dependency_links.txt
--rw-r--r--   0 bugrimov   (503) staff       (20)       13 2021-11-16 08:14:45.000000 aqueduct-1.8.1/aqueduct.egg-info/requires.txt
--rw-r--r--   0 bugrimov   (503) staff       (20)       15 2021-11-16 08:14:45.000000 aqueduct-1.8.1/aqueduct.egg-info/top_level.txt
--rw-r--r--   0 bugrimov   (503) staff       (20)       38 2021-11-16 08:14:45.443164 aqueduct-1.8.1/setup.cfg
--rw-r--r--   0 bugrimov   (503) staff       (20)     1476 2021-11-16 08:13:40.000000 aqueduct-1.8.1/setup.py
-drwxr-xr-x   0 bugrimov   (503) staff       (20)        0 2021-11-16 08:14:45.436356 aqueduct-1.8.1/tests/
--rw-r--r--   0 bugrimov   (503) staff       (20)        0 2021-09-02 13:20:17.000000 aqueduct-1.8.1/tests/__init__.py
-drwxr-xr-x   0 bugrimov   (503) staff       (20)        0 2021-11-16 08:14:45.437021 aqueduct-1.8.1/tests/benchmarks/
--rw-r--r--   0 bugrimov   (503) staff       (20)        0 2021-09-02 13:20:17.000000 aqueduct-1.8.1/tests/benchmarks/__init__.py
--rw-r--r--   0 bugrimov   (503) staff       (20)     3302 2021-09-02 13:20:17.000000 aqueduct-1.8.1/tests/benchmarks/bench_queue_transfer.py
-drwxr-xr-x   0 bugrimov   (503) staff       (20)        0 2021-11-16 08:14:45.437280 aqueduct-1.8.1/tests/benchmarks/bench_service/
--rw-r--r--   0 bugrimov   (503) staff       (20)        0 2021-09-02 13:20:17.000000 aqueduct-1.8.1/tests/benchmarks/bench_service/__init__.py
-drwxr-xr-x   0 bugrimov   (503) staff       (20)        0 2021-11-16 08:14:45.439069 aqueduct-1.8.1/tests/benchmarks/bench_service/bench/
--rw-r--r--   0 bugrimov   (503) staff       (20)        0 2021-09-02 13:20:17.000000 aqueduct-1.8.1/tests/benchmarks/bench_service/bench/__init__.py
--rw-r--r--   0 bugrimov   (503) staff       (20)     1528 2021-09-02 13:20:17.000000 aqueduct-1.8.1/tests/benchmarks/bench_service/bench/base.py
--rw-r--r--   0 bugrimov   (503) staff       (20)     4829 2021-09-02 13:20:17.000000 aqueduct-1.8.1/tests/benchmarks/bench_service/bench/bench_configurations.py
--rw-r--r--   0 bugrimov   (503) staff       (20)     2583 2021-09-02 13:20:17.000000 aqueduct-1.8.1/tests/benchmarks/bench_service/bench/bench_steps.py
--rw-r--r--   0 bugrimov   (503) staff       (20)     6933 2021-09-02 13:20:17.000000 aqueduct-1.8.1/tests/benchmarks/bench_service/bench/pulemet_kassym.py
--rw-r--r--   0 bugrimov   (503) staff       (20)     7276 2021-09-02 13:20:17.000000 aqueduct-1.8.1/tests/benchmarks/bench_service/bench/rps_counter.py
--rw-r--r--   0 bugrimov   (503) staff       (20)     1467 2021-09-02 13:20:17.000000 aqueduct-1.8.1/tests/benchmarks/bench_service/bench/utils.py
--rw-r--r--   0 bugrimov   (503) staff       (20)     1316 2021-09-02 13:20:17.000000 aqueduct-1.8.1/tests/benchmarks/utils.py
-drwxr-xr-x   0 bugrimov   (503) staff       (20)        0 2021-11-16 08:14:45.440526 aqueduct-1.8.1/tests/unit/
--rw-r--r--   0 bugrimov   (503) staff       (20)        0 2021-09-02 13:20:17.000000 aqueduct-1.8.1/tests/unit/__init__.py
--rw-r--r--   0 bugrimov   (503) staff       (20)     5253 2021-11-16 08:12:58.000000 aqueduct-1.8.1/tests/unit/conftest.py
-drwxr-xr-x   0 bugrimov   (503) staff       (20)        0 2021-11-16 08:14:45.440945 aqueduct-1.8.1/tests/unit/integrations/
--rw-r--r--   0 bugrimov   (503) staff       (20)        0 2021-09-27 22:16:38.000000 aqueduct-1.8.1/tests/unit/integrations/__init__.py
--rw-r--r--   0 bugrimov   (503) staff       (20)     2406 2021-10-15 17:26:57.000000 aqueduct-1.8.1/tests/unit/integrations/test_aiohttp.py
-drwxr-xr-x   0 bugrimov   (503) staff       (20)        0 2021-11-16 08:14:45.442375 aqueduct-1.8.1/tests/unit/metrics/
--rw-r--r--   0 bugrimov   (503) staff       (20)        0 2021-09-02 13:20:17.000000 aqueduct-1.8.1/tests/unit/metrics/__init__.py
--rw-r--r--   0 bugrimov   (503) staff       (20)      272 2021-09-27 22:16:38.000000 aqueduct-1.8.1/tests/unit/metrics/test_collect.py
--rw-r--r--   0 bugrimov   (503) staff       (20)     5919 2021-10-15 17:26:57.000000 aqueduct-1.8.1/tests/unit/metrics/test_export.py
--rw-r--r--   0 bugrimov   (503) staff       (20)     1446 2021-09-02 13:20:17.000000 aqueduct-1.8.1/tests/unit/metrics/test_metrics.py
--rw-r--r--   0 bugrimov   (503) staff       (20)      437 2021-09-02 13:20:17.000000 aqueduct-1.8.1/tests/unit/metrics/test_task.py
--rw-r--r--   0 bugrimov   (503) staff       (20)    10778 2021-10-15 17:26:57.000000 aqueduct-1.8.1/tests/unit/test_flow.py
--rw-r--r--   0 bugrimov   (503) staff       (20)     6285 2021-11-10 11:54:36.000000 aqueduct-1.8.1/tests/unit/test_shm.py
--rw-r--r--   0 bugrimov   (503) staff       (20)     2447 2021-09-02 13:20:17.000000 aqueduct-1.8.1/tests/unit/test_task.py
--rw-r--r--   0 bugrimov   (503) staff       (20)      900 2021-09-02 13:20:17.000000 aqueduct-1.8.1/tests/unit/test_worker.py
+drwxr-xr-x   0 bugrimov   (503) staff       (20)        0 2021-11-22 11:00:59.584201 aqueduct-1.9.0/
+-rw-r--r--   0 bugrimov   (503) staff       (20)     6915 2021-11-22 11:00:59.583917 aqueduct-1.9.0/PKG-INFO
+-rw-r--r--   0 bugrimov   (503) staff       (20)     5835 2021-09-30 14:31:22.000000 aqueduct-1.9.0/README.rst
+drwxr-xr-x   0 bugrimov   (503) staff       (20)        0 2021-11-22 11:00:59.558149 aqueduct-1.9.0/aqueduct/
+-rw-r--r--   0 bugrimov   (503) staff       (20)      153 2021-11-16 08:12:58.000000 aqueduct-1.9.0/aqueduct/__init__.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)      324 2021-09-02 13:20:17.000000 aqueduct-1.9.0/aqueduct/exceptions.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)    10704 2021-11-22 11:00:34.000000 aqueduct-1.9.0/aqueduct/flow.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     1011 2021-09-02 13:20:17.000000 aqueduct-1.9.0/aqueduct/handler.py
+drwxr-xr-x   0 bugrimov   (503) staff       (20)        0 2021-11-22 11:00:59.560386 aqueduct-1.9.0/aqueduct/integrations/
+-rw-r--r--   0 bugrimov   (503) staff       (20)        0 2021-09-27 22:16:38.000000 aqueduct-1.9.0/aqueduct/integrations/__init__.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     1881 2021-10-15 17:26:57.000000 aqueduct-1.9.0/aqueduct/integrations/aiohttp.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)      301 2021-09-02 13:20:17.000000 aqueduct-1.9.0/aqueduct/logger.py
+drwxr-xr-x   0 bugrimov   (503) staff       (20)        0 2021-11-22 11:00:59.563789 aqueduct-1.9.0/aqueduct/metrics/
+-rw-r--r--   0 bugrimov   (503) staff       (20)      105 2021-09-02 13:20:17.000000 aqueduct-1.9.0/aqueduct/metrics/__init__.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     1119 2021-09-02 13:20:17.000000 aqueduct-1.9.0/aqueduct/metrics/base.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     2319 2021-09-02 13:20:17.000000 aqueduct-1.9.0/aqueduct/metrics/collect.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     2570 2021-09-02 13:20:17.000000 aqueduct-1.9.0/aqueduct/metrics/export.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     1287 2021-09-02 13:20:17.000000 aqueduct-1.9.0/aqueduct/metrics/manager.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     1362 2021-09-02 13:20:17.000000 aqueduct-1.9.0/aqueduct/metrics/task.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)      878 2021-09-02 13:20:17.000000 aqueduct-1.9.0/aqueduct/metrics/timer.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     7180 2021-09-02 13:20:17.000000 aqueduct-1.9.0/aqueduct/multiprocessing.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     8284 2021-11-16 08:12:58.000000 aqueduct-1.9.0/aqueduct/shm.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     2098 2021-09-02 13:20:17.000000 aqueduct-1.9.0/aqueduct/task.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     5202 2021-11-22 11:00:34.000000 aqueduct-1.9.0/aqueduct/worker.py
+drwxr-xr-x   0 bugrimov   (503) staff       (20)        0 2021-11-22 11:00:59.559870 aqueduct-1.9.0/aqueduct.egg-info/
+-rw-r--r--   0 bugrimov   (503) staff       (20)     6915 2021-11-22 11:00:59.000000 aqueduct-1.9.0/aqueduct.egg-info/PKG-INFO
+-rw-r--r--   0 bugrimov   (503) staff       (20)     1516 2021-11-22 11:00:59.000000 aqueduct-1.9.0/aqueduct.egg-info/SOURCES.txt
+-rw-r--r--   0 bugrimov   (503) staff       (20)        1 2021-11-22 11:00:59.000000 aqueduct-1.9.0/aqueduct.egg-info/dependency_links.txt
+-rw-r--r--   0 bugrimov   (503) staff       (20)       13 2021-11-22 11:00:59.000000 aqueduct-1.9.0/aqueduct.egg-info/requires.txt
+-rw-r--r--   0 bugrimov   (503) staff       (20)       15 2021-11-22 11:00:59.000000 aqueduct-1.9.0/aqueduct.egg-info/top_level.txt
+-rw-r--r--   0 bugrimov   (503) staff       (20)       38 2021-11-22 11:00:59.584281 aqueduct-1.9.0/setup.cfg
+-rw-r--r--   0 bugrimov   (503) staff       (20)     1476 2021-11-22 11:00:34.000000 aqueduct-1.9.0/setup.py
+drwxr-xr-x   0 bugrimov   (503) staff       (20)        0 2021-11-22 11:00:59.564252 aqueduct-1.9.0/tests/
+-rw-r--r--   0 bugrimov   (503) staff       (20)        0 2021-09-02 13:20:17.000000 aqueduct-1.9.0/tests/__init__.py
+drwxr-xr-x   0 bugrimov   (503) staff       (20)        0 2021-11-22 11:00:59.565312 aqueduct-1.9.0/tests/benchmarks/
+-rw-r--r--   0 bugrimov   (503) staff       (20)        0 2021-09-02 13:20:17.000000 aqueduct-1.9.0/tests/benchmarks/__init__.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     3302 2021-09-02 13:20:17.000000 aqueduct-1.9.0/tests/benchmarks/bench_queue_transfer.py
+drwxr-xr-x   0 bugrimov   (503) staff       (20)        0 2021-11-22 11:00:59.566120 aqueduct-1.9.0/tests/benchmarks/bench_service/
+-rw-r--r--   0 bugrimov   (503) staff       (20)        0 2021-09-02 13:20:17.000000 aqueduct-1.9.0/tests/benchmarks/bench_service/__init__.py
+drwxr-xr-x   0 bugrimov   (503) staff       (20)        0 2021-11-22 11:00:59.576517 aqueduct-1.9.0/tests/benchmarks/bench_service/bench/
+-rw-r--r--   0 bugrimov   (503) staff       (20)        0 2021-09-02 13:20:17.000000 aqueduct-1.9.0/tests/benchmarks/bench_service/bench/__init__.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     1528 2021-09-02 13:20:17.000000 aqueduct-1.9.0/tests/benchmarks/bench_service/bench/base.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     4829 2021-09-02 13:20:17.000000 aqueduct-1.9.0/tests/benchmarks/bench_service/bench/bench_configurations.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     2583 2021-09-02 13:20:17.000000 aqueduct-1.9.0/tests/benchmarks/bench_service/bench/bench_steps.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     6933 2021-09-02 13:20:17.000000 aqueduct-1.9.0/tests/benchmarks/bench_service/bench/pulemet_kassym.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     7276 2021-09-02 13:20:17.000000 aqueduct-1.9.0/tests/benchmarks/bench_service/bench/rps_counter.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     1467 2021-09-02 13:20:17.000000 aqueduct-1.9.0/tests/benchmarks/bench_service/bench/utils.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     1316 2021-09-02 13:20:17.000000 aqueduct-1.9.0/tests/benchmarks/utils.py
+drwxr-xr-x   0 bugrimov   (503) staff       (20)        0 2021-11-22 11:00:59.580266 aqueduct-1.9.0/tests/unit/
+-rw-r--r--   0 bugrimov   (503) staff       (20)        0 2021-09-02 13:20:17.000000 aqueduct-1.9.0/tests/unit/__init__.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     5253 2021-11-16 08:12:58.000000 aqueduct-1.9.0/tests/unit/conftest.py
+drwxr-xr-x   0 bugrimov   (503) staff       (20)        0 2021-11-22 11:00:59.580950 aqueduct-1.9.0/tests/unit/integrations/
+-rw-r--r--   0 bugrimov   (503) staff       (20)        0 2021-09-27 22:16:38.000000 aqueduct-1.9.0/tests/unit/integrations/__init__.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     2406 2021-10-15 17:26:57.000000 aqueduct-1.9.0/tests/unit/integrations/test_aiohttp.py
+drwxr-xr-x   0 bugrimov   (503) staff       (20)        0 2021-11-22 11:00:59.583281 aqueduct-1.9.0/tests/unit/metrics/
+-rw-r--r--   0 bugrimov   (503) staff       (20)        0 2021-09-02 13:20:17.000000 aqueduct-1.9.0/tests/unit/metrics/__init__.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)      272 2021-09-27 22:16:38.000000 aqueduct-1.9.0/tests/unit/metrics/test_collect.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     5919 2021-10-15 17:26:57.000000 aqueduct-1.9.0/tests/unit/metrics/test_export.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     1446 2021-09-02 13:20:17.000000 aqueduct-1.9.0/tests/unit/metrics/test_metrics.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)      437 2021-09-02 13:20:17.000000 aqueduct-1.9.0/tests/unit/metrics/test_task.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)    10779 2021-11-22 11:00:34.000000 aqueduct-1.9.0/tests/unit/test_flow.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     6285 2021-11-10 11:54:36.000000 aqueduct-1.9.0/tests/unit/test_shm.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     2447 2021-09-02 13:20:17.000000 aqueduct-1.9.0/tests/unit/test_task.py
+-rw-r--r--   0 bugrimov   (503) staff       (20)     2617 2021-11-22 11:00:34.000000 aqueduct-1.9.0/tests/unit/test_worker.py
```

### Comparing `aqueduct-1.8.1/PKG-INFO` & `aqueduct-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduct
-Version: 1.8.1
+Version: 1.9.0
 Summary: Builder for performance-efficient prediction.
 Home-page: https://github.com/avito-tech/aqueduct
 Author: Data Science SWAT
 Author-email: UnitDataScienceSwat@avito.ru
 License: MIT
 Download-URL: https://github.com/avito-tech/aqueduct/archive/refs/heads/main.zip
 Keywords: datascience,learning
```

### Comparing `aqueduct-1.8.1/README.rst` & `aqueduct-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/aqueduct/flow.py` & `aqueduct-1.9.0/aqueduct/flow.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from enum import Enum
 from functools import cached_property
 from functools import reduce
 from multiprocessing import Barrier
 from threading import BrokenBarrierError
 from typing import Callable, Dict, List, Optional, Union
 
+from concurrent.futures import ThreadPoolExecutor
 from multiprocessing.resource_tracker import _resource_tracker  # noqa
 
 from .exceptions import FlowError, NotRunningError
 from .handler import BaseTaskHandler
 from .logger import log
 from .metrics import MAIN_PROCESS, MetricsTypes
 from .metrics.collect import Collector, TasksStats
@@ -228,36 +229,58 @@
         self._metrics_manager.start(queues_info=self._get_queues_info())
 
     def _get_queues_info(self) -> Dict[mp.Queue, str]:
         """Returns queues between Step handlers and its names.
 
         The queue name consists of two handler names that are connected by this queue.
         """
+
         def step_names(handlers):
             from_step = MAIN_PROCESS
             for step_number, handler in enumerate(handlers, 1):
                 to_step = handler.get_step_name(step_number)
                 yield from_step, to_step
                 from_step = to_step
             yield from_step, MAIN_PROCESS
 
         return {queue_: f'from_{from_}_to_{to}'
                 for queue_, (from_, to) in zip(self._queues, step_names(self._contexts))}
 
+    @staticmethod
+    def _fetch_from_queue(out_queue: mp.Queue) -> Union[BaseTask, None]:
+        try:
+            task = out_queue.get(timeout=1.)
+            return task
+        except queue.Empty:
+            return None
+
     async def _fetch_processed(self):
-        while True:
-            try:
-                task: BaseTask = self._queues[-1].get(block=False)
+        """ Fetching messages from output queue.
+
+        To handle messages from another process and not block asyncio loop, we run queue.get()
+        in a separate thread
+
+        """
+        loop = asyncio.get_event_loop()
+
+        with ThreadPoolExecutor(max_workers=1) as queue_fetch_executor:
+            while True:
+                task = await loop.run_in_executor(
+                    queue_fetch_executor,
+                    self._fetch_from_queue,
+                    self._queues[-1]
+                )
+                if not task:
+                    continue
+
                 task.metrics.stop_transfer_timer(MAIN_PROCESS)
-            except queue.Empty:
-                await asyncio.sleep(0.001)
-                continue
-            if task.task_id in self._task_futures:
-                future = self._task_futures[task.task_id]
-                if not future.cancelled() and not future.done():
+
+                future = self._task_futures.get(task.task_id)
+
+                if future and not future.cancelled() and not future.done():
                     future.set_result(task)
 
     async def _check_is_alive(self, sleep_sec: float = 1.):
         """Checks that all child processes are alive.
 
         If at least one process is not alive, it stops Flow.
         """
```

### Comparing `aqueduct-1.8.1/aqueduct/handler.py` & `aqueduct-1.9.0/aqueduct/handler.py`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/aqueduct/integrations/aiohttp.py` & `aqueduct-1.9.0/aqueduct/integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/aqueduct/metrics/base.py` & `aqueduct-1.9.0/aqueduct/metrics/base.py`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/aqueduct/metrics/collect.py` & `aqueduct-1.9.0/aqueduct/metrics/collect.py`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/aqueduct/metrics/export.py` & `aqueduct-1.9.0/aqueduct/metrics/export.py`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/aqueduct/metrics/manager.py` & `aqueduct-1.9.0/aqueduct/metrics/manager.py`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/aqueduct/metrics/task.py` & `aqueduct-1.9.0/aqueduct/metrics/task.py`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/aqueduct/metrics/timer.py` & `aqueduct-1.9.0/aqueduct/metrics/timer.py`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/aqueduct/multiprocessing.py` & `aqueduct-1.9.0/aqueduct/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/aqueduct/shm.py` & `aqueduct-1.9.0/aqueduct/shm.py`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/aqueduct/task.py` & `aqueduct-1.9.0/aqueduct/task.py`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/aqueduct/worker.py` & `aqueduct-1.9.0/aqueduct/worker.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,47 +5,14 @@
 
 from .handler import BaseTaskHandler
 from .logger import log
 from .metrics.timer import timeit
 from .task import BaseTask, StopTask
 
 
-def batches(
-        elements: Iterable,
-        batch_size: int,
-        timeout: float,
-) -> Iterator[List]:
-    batch = []
-    timeout_end = time.monotonic() + timeout
-
-    for elem in elements:
-        if elem:
-            batch.append(elem)
-        if time.monotonic() >= timeout_end or len(batch) == batch_size:
-            if batch:
-                yield batch
-                batch = []
-            timeout_end = time.monotonic() + timeout
-
-    if batch:
-        yield batch
-
-
-def batches_with_lock(batches_gen: Iterator[List], lock: mp.Lock) -> Iterator[List]:
-    while True:
-        lock.acquire()
-        try:
-            batch = next(batches_gen)
-        except StopIteration:
-            return
-        finally:
-            lock.release()
-        yield batch
-
-
 class Worker:
     """Обертка над классом BaseTaskHandler.
 
     Достает из входной очереди задачу, пропускает ее через обработчика task_handler и кладет ее
     в выходную очередь.
     """
 
@@ -71,65 +38,99 @@
         self._batch_lock = batch_lock
         self._stop_task: BaseTask = None  # noqa
 
     def _start(self):
         """Runs something huge (e.g. model) in child process."""
         self.task_handler.on_start()
 
-    def _tasks(self) -> Iterator[Optional[BaseTask]]:
-        """Provides suitable for processing tasks."""
+    def _wait_task(self, timeout: float) -> Optional[BaseTask]:
+        try:
+            task: BaseTask = self.queue_in.get(timeout=timeout)
+        except queue.Empty:
+            return
+
+        if isinstance(task, StopTask):
+            self._stop_task = task
+            return
+
+        log.debug(f'[{self.name}] Have message')
+        task.metrics.stop_transfer_timer(self.step_name)
+
+        # don't pass an expired task to the next steps
+        if task.is_expired():
+            log.debug(f'[{self.name}] Task expired. Skip: {task}')
+            return
+
+        # don't process unsuitable tasks
+        if not self.handle_condition(task):
+            self._post_handle(task)
+            return
+
+        return task
+
+    def _wait_batch(self) -> List[BaseTask]:
+        batch = []
+
+        # wait for the first task
         while True:
-            try:
-                task: BaseTask = self.queue_in.get(block=False)
-            except queue.Empty:
-                # returns control
-                yield
-                time.sleep(0.001)
-                continue
-            if isinstance(task, StopTask):
-                self._stop_task = task
+            task = self._wait_task(10.)
+            if task:
+                batch.append(task)
                 break
-            log.debug(f'[{self.name}] Have message')
-            task.metrics.stop_transfer_timer(self.step_name)
-            # dont't pass an expired task to the next steps
-            if task.is_expired():
-                log.debug(f'[{self.name}] Task expired. Skip: {task}')
-                continue
-            # don't process unsuitable tasks
-            if not self.handle_condition(task):
-                self._post_handle(task)
-                continue
-            yield task
+            elif self._stop_task:
+                return []
 
-    def _tasks_batches(self) -> Iterator[Optional[List[BaseTask]]]:
+        # if batch size is 1, there is no need to wait anymore
         if self._batch_size == 1:
-            # pseudo batching
-            for task in self._tasks():
-                if task:
-                    yield [task]
-        else:
-            tasks_batches: Iterator[List[BaseTask]] = batches(
-                self._tasks(),
-                batch_size=self._batch_size,
-                timeout=self._batch_timeout,
-            )
-            if self._batch_lock:
-                # to take a queue_in lock for the duration of batch filling time
-                tasks_batches = batches_with_lock(tasks_batches, self._batch_lock)
-
-            while True:
-                try:
-                    with timeit() as timer:
-                        tasks_batch = next(tasks_batches)
+            return batch
+
+        # waiting for the rest of the batch
+        timeout = self._batch_timeout
+        while True:
+            with timeit() as passed_time:
+                task = self._wait_task(timeout)
+
+            if task:
+                batch.append(task)
+
+                if len(batch) == self._batch_size:
+                    return batch
+
+            timeout -= passed_time.seconds
+
+            if self._stop_task or timeout <= 0:
+                return batch
+
+            # timeout should not be less then 1ms, to avoid unnecessary short sleeps
+            timeout = max(timeout, 0.001)
+
+    def _iter_batches(self) -> Iterator[Optional[List[BaseTask]]]:
+        """ Returns iterator over input task batches.
+        If there is no tasks in queue -> block until task appears.
+        This iterator takes into account batch_timeout and batch size.
+        If input task is expired or filtered by condition - it would not be placed in batch.
+        """
+        while True:
+            with timeit() as timer:
+                if self._batch_lock:
+                    # to take a queue_in lock for the duration of batch filling time
+                    with self._batch_lock:
+                        tasks_batch = self._wait_batch()
+                else:
+                    tasks_batch = self._wait_batch()
+
+            if tasks_batch and len(tasks_batch) > 0:
+                if self._batch_size > 1:
                     tasks_batch[0].metrics.batch_times.add(self.step_name, timer.seconds)
                     tasks_batch[0].metrics.batch_sizes.add(self.step_name, len(tasks_batch))
-                except StopIteration:
-                    return
                 yield tasks_batch
 
+            if self._stop_task:
+                break
+
     def _post_handle(self, task: BaseTask):
         task.metrics.start_transfer_timer(self.step_name)
         self.queue_out.put(task)
 
     def loop(self, pid: int, start_barrier: mp.Barrier):
         """Main worker loop.
 
@@ -138,15 +139,15 @@
         log.info(f'[Worker] initialising handler {self.name}')
         self._start()
         log.info(f'[Worker] handler {self.name} ok, waiting for others to start')
         start_barrier.wait()
 
         log.info(f'[Worker] handler {self.name} ok, starting loop')
 
-        for tasks_batch in self._tasks_batches():
+        for tasks_batch in self._iter_batches():
             with timeit() as timer:
                 self.task_handler.handle(*tasks_batch)
 
             for task in tasks_batch:
                 task.metrics.handle_times.add(self.step_name, timer.seconds)
                 self._post_handle(task)
```

### Comparing `aqueduct-1.8.1/aqueduct.egg-info/PKG-INFO` & `aqueduct-1.9.0/aqueduct.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduct
-Version: 1.8.1
+Version: 1.9.0
 Summary: Builder for performance-efficient prediction.
 Home-page: https://github.com/avito-tech/aqueduct
 Author: Data Science SWAT
 Author-email: UnitDataScienceSwat@avito.ru
 License: MIT
 Download-URL: https://github.com/avito-tech/aqueduct/archive/refs/heads/main.zip
 Keywords: datascience,learning
```

### Comparing `aqueduct-1.8.1/aqueduct.egg-info/SOURCES.txt` & `aqueduct-1.9.0/aqueduct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/setup.py` & `aqueduct-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 packages = ['aqueduct']
 
 setup(
     name='aqueduct',
     packages=find_packages(),
-    version='1.8.1',
+    version='1.9.0',
     license='MIT',
     license_files='LICENSE.txt',
     author='Data Science SWAT',
     author_email='UnitDataScienceSwat@avito.ru',
     description='Builder for performance-efficient prediction.',
     url='https://github.com/avito-tech/aqueduct',
     download_url='https://github.com/avito-tech/aqueduct/archive/refs/heads/main.zip',
```

### Comparing `aqueduct-1.8.1/tests/benchmarks/bench_queue_transfer.py` & `aqueduct-1.9.0/tests/benchmarks/bench_queue_transfer.py`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/tests/benchmarks/bench_service/bench/base.py` & `aqueduct-1.9.0/tests/benchmarks/bench_service/bench/base.py`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/tests/benchmarks/bench_service/bench/bench_configurations.py` & `aqueduct-1.9.0/tests/benchmarks/bench_service/bench/bench_configurations.py`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/tests/benchmarks/bench_service/bench/bench_steps.py` & `aqueduct-1.9.0/tests/benchmarks/bench_service/bench/bench_steps.py`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/tests/benchmarks/bench_service/bench/pulemet_kassym.py` & `aqueduct-1.9.0/tests/benchmarks/bench_service/bench/pulemet_kassym.py`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/tests/benchmarks/bench_service/bench/rps_counter.py` & `aqueduct-1.9.0/tests/benchmarks/bench_service/bench/rps_counter.py`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/tests/benchmarks/bench_service/bench/utils.py` & `aqueduct-1.9.0/tests/benchmarks/bench_service/bench/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/tests/benchmarks/utils.py` & `aqueduct-1.9.0/tests/benchmarks/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/tests/unit/conftest.py` & `aqueduct-1.9.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/tests/unit/integrations/test_aiohttp.py` & `aqueduct-1.9.0/tests/unit/integrations/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/tests/unit/metrics/test_export.py` & `aqueduct-1.9.0/tests/unit/metrics/test_export.py`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/tests/unit/metrics/test_metrics.py` & `aqueduct-1.9.0/tests/unit/metrics/test_metrics.py`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/tests/unit/test_flow.py` & `aqueduct-1.9.0/tests/unit/test_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         yield flow
 
 
 class CatDetector:
     """GPU model emulator that predicts the presence of the cat in the image."""
     IMAGE_PROCESS_TIME = 0.01
     BATCH_REDUCTION_FACTOR = 0.7
-    OVERHEAD_TIME = 0.02
+    OVERHEAD_TIME = 0.025
     BATCH_PROCESS_TIME = IMAGE_PROCESS_TIME * TASKS_BATCH_SIZE * BATCH_REDUCTION_FACTOR + OVERHEAD_TIME
 
     def predict(self, images: np.array) -> np.array:
         """Always says that there is a cat in the image.
 
         The image is represented by a one-dimensional array.
         The model spends less time for processing batch of images due to GPU optimizations. It's emulated
```

### Comparing `aqueduct-1.8.1/tests/unit/test_shm.py` & `aqueduct-1.9.0/tests/unit/test_shm.py`

 * *Files identical despite different names*

### Comparing `aqueduct-1.8.1/tests/unit/test_task.py` & `aqueduct-1.9.0/tests/unit/test_task.py`

 * *Files identical despite different names*


# Comparing `tmp/distributed-2023.4.1.tar.gz` & `tmp/distributed-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distributed-2023.4.1.tar", last modified: Fri Apr 28 17:30:07 2023, max compression
+gzip compressed data, was "distributed-2023.5.0.tar", last modified: Fri May 12 15:53:52 2023, max compression
```

## Comparing `distributed-2023.4.1.tar` & `distributed-2023.5.0.tar`

### file list

```diff
@@ -1,287 +1,295 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.864022 distributed-2023.4.1/
--rw-r--r--   0 james      (501) staff       (20)      104 2020-06-30 15:19:20.000000 distributed-2023.4.1/AUTHORS.md
--rw-r--r--   0 james      (501) staff       (20)     1533 2022-10-21 17:45:03.000000 distributed-2023.4.1/LICENSE.txt
--rw-r--r--   0 james      (501) staff       (20)      633 2023-04-26 17:04:39.000000 distributed-2023.4.1/MANIFEST.in
--rw-r--r--   0 james      (501) staff       (20)     2882 2023-04-28 17:30:07.863188 distributed-2023.4.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     1801 2022-10-21 17:45:03.000000 distributed-2023.4.1/README.rst
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.864668 distributed-2023.4.1/distributed/
--rw-r--r--   0 james      (501) staff       (20)     3836 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     5528 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/_concurrent_futures_thread.py
--rw-r--r--   0 james      (501) staff       (20)     1297 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/_signals.py
--rw-r--r--   0 james      (501) staff       (20)     1372 2022-11-10 20:28:41.000000 distributed-2023.4.1/distributed/_stories.py
--rw-r--r--   0 james      (501) staff       (20)      500 2023-04-28 17:30:07.864812 distributed-2023.4.1/distributed/_version.py
--rw-r--r--   0 james      (501) staff       (20)    29277 2023-04-26 17:04:39.000000 distributed-2023.4.1/distributed/active_memory_manager.py
--rw-r--r--   0 james      (501) staff       (20)    10649 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/actor.py
--rw-r--r--   0 james      (501) staff       (20)     7347 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/batched.py
--rw-r--r--   0 james      (501) staff       (20)      121 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/bokeh.py
--rw-r--r--   0 james      (501) staff       (20)     5742 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/cfexecutor.py
--rw-r--r--   0 james      (501) staff       (20)     1947 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/chaos.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.666386 distributed-2023.4.1/distributed/cli/
--rw-r--r--   0 james      (501) staff       (20)        0 2020-06-30 15:19:20.000000 distributed-2023.4.1/distributed/cli/__init__.py
--rwxr-xr-x   0 james      (501) staff       (20)     7077 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/cli/dask_scheduler.py
--rw-r--r--   0 james      (501) staff       (20)     1269 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/cli/dask_spec.py
--rwxr-xr-x   0 james      (501) staff       (20)     5468 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/cli/dask_ssh.py
--rwxr-xr-x   0 james      (501) staff       (20)    15948 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/cli/dask_worker.py
--rw-r--r--   0 james      (501) staff       (20)     1092 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/cli/utils.py
--rw-r--r--   0 james      (501) staff       (20)   201344 2023-04-28 16:00:56.000000 distributed-2023.4.1/distributed/client.py
--rw-r--r--   0 james      (501) staff       (20)    10985 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/cluster_dump.py
--rw-r--r--   0 james      (501) staff       (20)     6717 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/collections.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.677491 distributed-2023.4.1/distributed/comm/
--rw-r--r--   0 james      (501) staff       (20)     1285 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/comm/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     8597 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/comm/addressing.py
--rw-r--r--   0 james      (501) staff       (20)    37224 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/comm/asyncio_tcp.py
--rw-r--r--   0 james      (501) staff       (20)    11809 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/comm/core.py
--rw-r--r--   0 james      (501) staff       (20)    10253 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/comm/inproc.py
--rw-r--r--   0 james      (501) staff       (20)     2815 2022-11-15 16:22:42.000000 distributed-2023.4.1/distributed/comm/registry.py
--rw-r--r--   0 james      (501) staff       (20)    24495 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/comm/tcp.py
--rw-r--r--   0 james      (501) staff       (20)    22794 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/comm/ucx.py
--rw-r--r--   0 james      (501) staff       (20)     4220 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/comm/utils.py
--rw-r--r--   0 james      (501) staff       (20)    14184 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/comm/ws.py
--rw-r--r--   0 james      (501) staff       (20)     7959 2023-04-26 17:04:39.000000 distributed-2023.4.1/distributed/compatibility.py
--rw-r--r--   0 james      (501) staff       (20)     7357 2023-04-26 17:04:43.000000 distributed-2023.4.1/distributed/config.py
--rw-r--r--   0 james      (501) staff       (20)    56072 2023-04-26 17:04:43.000000 distributed-2023.4.1/distributed/core.py
--rw-r--r--   0 james      (501) staff       (20)     2146 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/counter.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.685936 distributed-2023.4.1/distributed/dashboard/
--rw-r--r--   0 james      (501) staff       (20)        0 2021-11-11 17:33:03.000000 distributed-2023.4.1/distributed/dashboard/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.693297 distributed-2023.4.1/distributed/dashboard/components/
--rw-r--r--   0 james      (501) staff       (20)     1550 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/dashboard/components/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     5818 2022-11-15 18:24:05.000000 distributed-2023.4.1/distributed/dashboard/components/nvml.py
--rw-r--r--   0 james      (501) staff       (20)     7055 2023-04-26 17:04:39.000000 distributed-2023.4.1/distributed/dashboard/components/rmm.py
--rw-r--r--   0 james      (501) staff       (20)   146950 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/dashboard/components/scheduler.py
--rw-r--r--   0 james      (501) staff       (20)    19467 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/dashboard/components/shared.py
--rw-r--r--   0 james      (501) staff       (20)    15424 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/dashboard/components/worker.py
--rw-r--r--   0 james      (501) staff       (20)     1690 2023-04-26 17:04:39.000000 distributed-2023.4.1/distributed/dashboard/core.py
--rw-r--r--   0 james      (501) staff       (20)     2313 2021-07-06 20:52:40.000000 distributed-2023.4.1/distributed/dashboard/export_tool.js
--rw-r--r--   0 james      (501) staff       (20)      763 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/dashboard/export_tool.py
--rw-r--r--   0 james      (501) staff       (20)     5717 2023-04-26 17:04:39.000000 distributed-2023.4.1/distributed/dashboard/scheduler.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.694214 distributed-2023.4.1/distributed/dashboard/templates/
--rw-r--r--   0 james      (501) staff       (20)      241 2022-06-06 20:36:46.000000 distributed-2023.4.1/distributed/dashboard/templates/performance_report.html
--rw-r--r--   0 james      (501) staff       (20)      199 2022-08-08 21:17:38.000000 distributed-2023.4.1/distributed/dashboard/theme.yaml
--rw-r--r--   0 james      (501) staff       (20)     1668 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/dashboard/utils.py
--rw-r--r--   0 james      (501) staff       (20)      840 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/dashboard/worker.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.705854 distributed-2023.4.1/distributed/deploy/
--rw-r--r--   0 james      (501) staff       (20)      466 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/deploy/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     6702 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/deploy/adaptive.py
--rw-r--r--   0 james      (501) staff       (20)     7802 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/deploy/adaptive_core.py
--rw-r--r--   0 james      (501) staff       (20)    21498 2023-04-26 17:04:39.000000 distributed-2023.4.1/distributed/deploy/cluster.py
--rw-r--r--   0 james      (501) staff       (20)    10434 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/deploy/local.py
--rw-r--r--   0 james      (501) staff       (20)    15514 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/deploy/old_ssh.py
--rw-r--r--   0 james      (501) staff       (20)    23732 2023-04-26 17:04:43.000000 distributed-2023.4.1/distributed/deploy/spec.py
--rw-r--r--   0 james      (501) staff       (20)    15265 2022-11-15 18:24:05.000000 distributed-2023.4.1/distributed/deploy/ssh.py
--rw-r--r--   0 james      (501) staff       (20)     7656 2023-04-26 17:04:39.000000 distributed-2023.4.1/distributed/deploy/subprocess.py
--rw-r--r--   0 james      (501) staff       (20)      888 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/deploy/utils.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.718672 distributed-2023.4.1/distributed/diagnostics/
--rw-r--r--   0 james      (501) staff       (20)      221 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/diagnostics/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     1302 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/diagnostics/cluster_dump.py
--rw-r--r--   0 james      (501) staff       (20)     2190 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/diagnostics/eventstream.py
--rw-r--r--   0 james      (501) staff       (20)     4994 2023-04-26 17:04:39.000000 distributed-2023.4.1/distributed/diagnostics/graph_layout.py
--rw-r--r--   0 james      (501) staff       (20)     6972 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/diagnostics/memory_sampler.py
--rw-r--r--   0 james      (501) staff       (20)    10781 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/diagnostics/nvml.py
--rw-r--r--   0 james      (501) staff       (20)    27724 2023-04-28 16:00:56.000000 distributed-2023.4.1/distributed/diagnostics/plugin.py
--rw-r--r--   0 james      (501) staff       (20)    12565 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/diagnostics/progress.py
--rw-r--r--   0 james      (501) staff       (20)     6063 2022-11-07 19:30:53.000000 distributed-2023.4.1/distributed/diagnostics/progress_stream.py
--rw-r--r--   0 james      (501) staff       (20)    14665 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/diagnostics/progressbar.py
--rw-r--r--   0 james      (501) staff       (20)     1124 2023-04-26 17:04:39.000000 distributed-2023.4.1/distributed/diagnostics/rmm.py
--rw-r--r--   0 james      (501) staff       (20)     5677 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/diagnostics/task_stream.py
--rw-r--r--   0 james      (501) staff       (20)     2434 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/diagnostics/websocket.py
--rw-r--r--   0 james      (501) staff       (20)     9172 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/diskutils.py
--rw-r--r--   0 james      (501) staff       (20)    45370 2023-04-27 19:19:46.000000 distributed-2023.4.1/distributed/distributed-schema.yaml
--rw-r--r--   0 james      (501) staff       (20)    14015 2023-04-27 19:19:46.000000 distributed-2023.4.1/distributed/distributed.yaml
--rw-r--r--   0 james      (501) staff       (20)     8536 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/event.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.725871 distributed-2023.4.1/distributed/http/
--rw-r--r--   0 james      (501) staff       (20)       84 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/http/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      258 2022-08-08 21:17:38.000000 distributed-2023.4.1/distributed/http/health.py
--rw-r--r--   0 james      (501) staff       (20)     1480 2022-11-15 18:24:05.000000 distributed-2023.4.1/distributed/http/prometheus.py
--rw-r--r--   0 james      (501) staff       (20)     4377 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/http/proxy.py
--rw-r--r--   0 james      (501) staff       (20)     2548 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/http/routing.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.730333 distributed-2023.4.1/distributed/http/scheduler/
--rw-r--r--   0 james      (501) staff       (20)        0 2021-11-11 17:33:04.000000 distributed-2023.4.1/distributed/http/scheduler/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     2899 2023-04-26 17:04:39.000000 distributed-2023.4.1/distributed/http/scheduler/api.py
--rw-r--r--   0 james      (501) staff       (20)     6926 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/http/scheduler/info.py
--rw-r--r--   0 james      (501) staff       (20)     2159 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/http/scheduler/json.py
--rw-r--r--   0 james      (501) staff       (20)      625 2023-04-26 17:04:39.000000 distributed-2023.4.1/distributed/http/scheduler/missing_bokeh.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.734307 distributed-2023.4.1/distributed/http/scheduler/prometheus/
--rw-r--r--   0 james      (501) staff       (20)      291 2022-11-15 18:24:05.000000 distributed-2023.4.1/distributed/http/scheduler/prometheus/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     7049 2023-04-26 17:04:39.000000 distributed-2023.4.1/distributed/http/scheduler/prometheus/core.py
--rw-r--r--   0 james      (501) staff       (20)     3514 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/http/scheduler/prometheus/semaphore.py
--rw-r--r--   0 james      (501) staff       (20)     1617 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/http/scheduler/prometheus/stealing.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.735352 distributed-2023.4.1/distributed/http/static/
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.738770 distributed-2023.4.1/distributed/http/static/css/
--rw-r--r--   0 james      (501) staff       (20)     2260 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/http/static/css/base.css
--rw-r--r--   0 james      (501) staff       (20)      250 2021-11-11 21:43:12.000000 distributed-2023.4.1/distributed/http/static/css/gpu.css
--rw-r--r--   0 james      (501) staff       (20)      840 2021-11-11 17:33:04.000000 distributed-2023.4.1/distributed/http/static/css/individual-cluster-map.css
--rw-r--r--   0 james      (501) staff       (20)     1012 2022-08-08 21:17:38.000000 distributed-2023.4.1/distributed/http/static/css/status.css
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.745015 distributed-2023.4.1/distributed/http/static/images/
--rw-r--r--   0 james      (501) staff       (20)     1607 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/http/static/images/dask-logo.svg
--rw-r--r--   0 james      (501) staff       (20)      552 2021-11-11 17:33:04.000000 distributed-2023.4.1/distributed/http/static/images/fa-bars.svg
--rw-r--r--   0 james      (501) staff       (20)    15086 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/http/static/images/favicon.ico
--rw-r--r--   0 james      (501) staff       (20)    11002 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/http/static/images/jupyter.svg
--rw-r--r--   0 james      (501) staff       (20)    18663 2022-08-08 21:17:38.000000 distributed-2023.4.1/distributed/http/static/images/numpy.png
--rw-r--r--   0 james      (501) staff       (20)     1213 2022-08-08 21:17:38.000000 distributed-2023.4.1/distributed/http/static/images/pandas.png
--rw-r--r--   0 james      (501) staff       (20)   830916 2022-08-08 21:17:38.000000 distributed-2023.4.1/distributed/http/static/images/python.png
--rw-r--r--   0 james      (501) staff       (20)      667 2021-11-11 17:33:04.000000 distributed-2023.4.1/distributed/http/static/individual-cluster-map.html
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.752414 distributed-2023.4.1/distributed/http/static/js/
--rw-r--r--   0 james      (501) staff       (20)    17271 2021-11-11 17:33:04.000000 distributed-2023.4.1/distributed/http/static/js/anime.min.js
--rw-r--r--   0 james      (501) staff       (20)     9337 2021-11-11 17:33:04.000000 distributed-2023.4.1/distributed/http/static/js/individual-cluster-map.js
--rw-r--r--   0 james      (501) staff       (20)     3276 2021-11-11 17:33:04.000000 distributed-2023.4.1/distributed/http/static/js/reconnecting-websocket.min.js
--rw-r--r--   0 james      (501) staff       (20)      223 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/http/statics.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.765521 distributed-2023.4.1/distributed/http/templates/
--rw-r--r--   0 james      (501) staff       (20)     2930 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/http/templates/base.html
--rw-r--r--   0 james      (501) staff       (20)      388 2021-11-11 17:33:04.000000 distributed-2023.4.1/distributed/http/templates/call-stack.html
--rw-r--r--   0 james      (501) staff       (20)     1351 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/http/templates/exceptions.html
--rw-r--r--   0 james      (501) staff       (20)      404 2021-11-11 21:43:12.000000 distributed-2023.4.1/distributed/http/templates/gpu.html
--rw-r--r--   0 james      (501) staff       (20)      276 2021-11-11 17:33:04.000000 distributed-2023.4.1/distributed/http/templates/json-index.html
--rw-r--r--   0 james      (501) staff       (20)      116 2021-11-11 17:33:04.000000 distributed-2023.4.1/distributed/http/templates/logs.html
--rw-r--r--   0 james      (501) staff       (20)      369 2021-11-11 17:33:04.000000 distributed-2023.4.1/distributed/http/templates/main.html
--rw-r--r--   0 james      (501) staff       (20)       95 2021-11-11 17:33:04.000000 distributed-2023.4.1/distributed/http/templates/simple.html
--rw-r--r--   0 james      (501) staff       (20)      635 2022-11-15 16:22:42.000000 distributed-2023.4.1/distributed/http/templates/status.html
--rw-r--r--   0 james      (501) staff       (20)     5672 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/http/templates/task.html
--rw-r--r--   0 james      (501) staff       (20)     1405 2021-11-11 17:33:04.000000 distributed-2023.4.1/distributed/http/templates/worker-table.html
--rw-r--r--   0 james      (501) staff       (20)     2024 2021-11-11 17:33:04.000000 distributed-2023.4.1/distributed/http/templates/worker.html
--rw-r--r--   0 james      (501) staff       (20)      457 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/http/templates/workers.html
--rw-r--r--   0 james      (501) staff       (20)     1184 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/http/utils.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.766682 distributed-2023.4.1/distributed/http/worker/
--rw-r--r--   0 james      (501) staff       (20)        0 2021-11-11 17:33:04.000000 distributed-2023.4.1/distributed/http/worker/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.768277 distributed-2023.4.1/distributed/http/worker/prometheus/
--rw-r--r--   0 james      (501) staff       (20)      288 2022-11-15 18:24:05.000000 distributed-2023.4.1/distributed/http/worker/prometheus/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     9973 2023-04-26 17:04:39.000000 distributed-2023.4.1/distributed/http/worker/prometheus/core.py
--rw-r--r--   0 james      (501) staff       (20)     5599 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/lock.py
--rwxr-xr-x   0 james      (501) staff       (20)    12252 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/metrics.py
--rw-r--r--   0 james      (501) staff       (20)     8044 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/multi_lock.py
--rw-r--r--   0 james      (501) staff       (20)    33598 2023-04-26 17:04:43.000000 distributed-2023.4.1/distributed/nanny.py
--rw-r--r--   0 james      (501) staff       (20)     6710 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/node.py
--rw-r--r--   0 james      (501) staff       (20)     1449 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/objects.py
--rw-r--r--   0 james      (501) staff       (20)     7513 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/preloading.py
--rw-r--r--   0 james      (501) staff       (20)    12887 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/process.py
--rw-r--r--   0 james      (501) staff       (20)      931 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/proctitle.py
--rw-r--r--   0 james      (501) staff       (20)    16141 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/profile.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.785493 distributed-2023.4.1/distributed/protocol/
--rw-r--r--   0 james      (501) staff       (20)     3442 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/protocol/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     1336 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/protocol/arrow.py
--rw-r--r--   0 james      (501) staff       (20)     6159 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/protocol/compression.py
--rw-r--r--   0 james      (501) staff       (20)     5964 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/protocol/core.py
--rw-r--r--   0 james      (501) staff       (20)     1181 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/protocol/cuda.py
--rw-r--r--   0 james      (501) staff       (20)     2788 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/protocol/cupy.py
--rw-r--r--   0 james      (501) staff       (20)      836 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/protocol/h5py.py
--rw-r--r--   0 james      (501) staff       (20)     1127 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/protocol/keras.py
--rw-r--r--   0 james      (501) staff       (20)     1466 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/protocol/netcdf4.py
--rw-r--r--   0 james      (501) staff       (20)     2139 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/protocol/numba.py
--rw-r--r--   0 james      (501) staff       (20)     6664 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/protocol/numpy.py
--rw-r--r--   0 james      (501) staff       (20)     3043 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/protocol/pickle.py
--rw-r--r--   0 james      (501) staff       (20)     1507 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/protocol/rmm.py
--rw-r--r--   0 james      (501) staff       (20)      800 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/protocol/scipy.py
--rw-r--r--   0 james      (501) staff       (20)    28504 2023-04-26 17:04:39.000000 distributed-2023.4.1/distributed/protocol/serialize.py
--rw-r--r--   0 james      (501) staff       (20)      955 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/protocol/sparse.py
--rw-r--r--   0 james      (501) staff       (20)     1993 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/protocol/torch.py
--rw-r--r--   0 james      (501) staff       (20)     6102 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/protocol/utils.py
--rw-r--r--   0 james      (501) staff       (20)     3733 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/publish.py
--rw-r--r--   0 james      (501) staff       (20)    15652 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/pubsub.py
--rw-r--r--   0 james      (501) staff       (20)        0 2022-08-08 21:17:38.000000 distributed-2023.4.1/distributed/py.typed
--rw-r--r--   0 james      (501) staff       (20)    10082 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/queues.py
--rw-r--r--   0 james      (501) staff       (20)     7620 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/recreate_tasks.py
--rw-r--r--   0 james      (501) staff       (20)   301675 2023-04-28 16:00:56.000000 distributed-2023.4.1/distributed/scheduler.py
--rw-r--r--   0 james      (501) staff       (20)    13825 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/security.py
--rw-r--r--   0 james      (501) staff       (20)    20568 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/semaphore.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.795692 distributed-2023.4.1/distributed/shuffle/
--rw-r--r--   0 james      (501) staff       (20)      692 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/shuffle/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     2938 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/shuffle/_arrow.py
--rw-r--r--   0 james      (501) staff       (20)     9212 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/shuffle/_buffer.py
--rw-r--r--   0 james      (501) staff       (20)     2499 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/shuffle/_comms.py
--rw-r--r--   0 james      (501) staff       (20)     3550 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/shuffle/_disk.py
--rw-r--r--   0 james      (501) staff       (20)     2361 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/shuffle/_limiter.py
--rw-r--r--   0 james      (501) staff       (20)    11736 2023-04-26 17:04:39.000000 distributed-2023.4.1/distributed/shuffle/_merge.py
--rw-r--r--   0 james      (501) staff       (20)     5203 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/shuffle/_rechunk.py
--rw-r--r--   0 james      (501) staff       (20)    10437 2023-04-26 17:04:39.000000 distributed-2023.4.1/distributed/shuffle/_scheduler_extension.py
--rw-r--r--   0 james      (501) staff       (20)     8299 2023-04-26 17:04:39.000000 distributed-2023.4.1/distributed/shuffle/_shuffle.py
--rw-r--r--   0 james      (501) staff       (20)    33146 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/shuffle/_worker_extension.py
--rw-r--r--   0 james      (501) staff       (20)      607 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/sizeof.py
--rw-r--r--   0 james      (501) staff       (20)    13216 2023-04-26 17:04:39.000000 distributed-2023.4.1/distributed/spill.py
--rw-r--r--   0 james      (501) staff       (20)    19859 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/stealing.py
--rw-r--r--   0 james      (501) staff       (20)     1883 2022-10-27 14:20:24.000000 distributed-2023.4.1/distributed/system.py
--rw-r--r--   0 james      (501) staff       (20)     8532 2023-04-28 16:00:56.000000 distributed-2023.4.1/distributed/system_monitor.py
--rw-r--r--   0 james      (501) staff       (20)     7104 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/threadpoolexecutor.py
--rw-r--r--   0 james      (501) staff       (20)    55458 2023-04-26 17:04:43.000000 distributed-2023.4.1/distributed/utils.py
--rw-r--r--   0 james      (501) staff       (20)    13992 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/utils_comm.py
--rw-r--r--   0 james      (501) staff       (20)     8050 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/utils_perf.py
--rw-r--r--   0 james      (501) staff       (20)    80266 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/utils_test.py
--rw-r--r--   0 james      (501) staff       (20)     8463 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/variable.py
--rw-r--r--   0 james      (501) staff       (20)     5194 2023-04-26 17:04:39.000000 distributed-2023.4.1/distributed/versions.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.796843 distributed-2023.4.1/distributed/widgets/
--rw-r--r--   0 james      (501) staff       (20)      267 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/widgets/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.812497 distributed-2023.4.1/distributed/widgets/templates/
--rw-r--r--   0 james      (501) staff       (20)     2265 2022-11-10 20:28:41.000000 distributed-2023.4.1/distributed/widgets/templates/client.html.j2
--rw-r--r--   0 james      (501) staff       (20)     1589 2022-08-08 21:17:38.000000 distributed-2023.4.1/distributed/widgets/templates/cluster.html.j2
--rw-r--r--   0 james      (501) staff       (20)     1270 2023-04-26 17:04:39.000000 distributed-2023.4.1/distributed/widgets/templates/computation.html.j2
--rw-r--r--   0 james      (501) staff       (20)      518 2022-08-08 21:17:38.000000 distributed-2023.4.1/distributed/widgets/templates/future.html.j2
--rw-r--r--   0 james      (501) staff       (20)      544 2022-08-08 21:17:38.000000 distributed-2023.4.1/distributed/widgets/templates/has_what.html.j2
--rw-r--r--   0 james      (501) staff       (20)      234 2022-08-08 21:17:38.000000 distributed-2023.4.1/distributed/widgets/templates/local_cluster.html.j2
--rw-r--r--   0 james      (501) staff       (20)      636 2022-08-08 21:17:38.000000 distributed-2023.4.1/distributed/widgets/templates/log.html.j2
--rw-r--r--   0 james      (501) staff       (20)      168 2022-08-08 21:17:38.000000 distributed-2023.4.1/distributed/widgets/templates/logs.html.j2
--rw-r--r--   0 james      (501) staff       (20)     1290 2022-08-08 21:17:38.000000 distributed-2023.4.1/distributed/widgets/templates/process_interface.html.j2
--rw-r--r--   0 james      (501) staff       (20)      317 2022-08-08 21:17:38.000000 distributed-2023.4.1/distributed/widgets/templates/scheduler.html.j2
--rw-r--r--   0 james      (501) staff       (20)     6705 2022-10-21 17:45:03.000000 distributed-2023.4.1/distributed/widgets/templates/scheduler_info.html.j2
--rw-r--r--   0 james      (501) staff       (20)      407 2022-08-08 21:17:38.000000 distributed-2023.4.1/distributed/widgets/templates/security.html.j2
--rw-r--r--   0 james      (501) staff       (20)      448 2022-08-08 21:17:38.000000 distributed-2023.4.1/distributed/widgets/templates/task_state.html.j2
--rw-r--r--   0 james      (501) staff       (20)      295 2022-08-08 21:17:38.000000 distributed-2023.4.1/distributed/widgets/templates/who_has.html.j2
--rw-r--r--   0 james      (501) staff       (20)      407 2022-08-08 21:17:38.000000 distributed-2023.4.1/distributed/widgets/templates/worker_state.html.j2
--rw-r--r--   0 james      (501) staff       (20)   126882 2023-04-26 17:04:43.000000 distributed-2023.4.1/distributed/worker.py
--rw-r--r--   0 james      (501) staff       (20)     2276 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/worker_client.py
--rw-r--r--   0 james      (501) staff       (20)    21367 2023-04-26 17:04:39.000000 distributed-2023.4.1/distributed/worker_memory.py
--rw-r--r--   0 james      (501) staff       (20)   141533 2023-04-25 18:34:44.000000 distributed-2023.4.1/distributed/worker_state_machine.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.661780 distributed-2023.4.1/distributed.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     2882 2023-04-28 17:30:07.000000 distributed-2023.4.1/distributed.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     8264 2023-04-28 17:30:07.000000 distributed-2023.4.1/distributed.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-04-28 17:30:07.000000 distributed-2023.4.1/distributed.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)      335 2023-04-28 17:30:07.000000 distributed-2023.4.1/distributed.egg-info/entry_points.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-04-28 17:30:06.000000 distributed-2023.4.1/distributed.egg-info/not-zip-safe
--rw-r--r--   0 james      (501) staff       (20)      227 2023-04-28 17:30:07.000000 distributed-2023.4.1/distributed.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       12 2023-04-28 17:30:07.000000 distributed-2023.4.1/distributed.egg-info/top_level.txt
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.577981 distributed-2023.4.1/docs/
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.860934 distributed-2023.4.1/docs/source/
--rw-r--r--   0 james      (501) staff       (20)    11754 2022-10-27 14:20:24.000000 distributed-2023.4.1/docs/source/active_memory_manager.rst
--rw-r--r--   0 james      (501) staff       (20)     8000 2022-11-15 18:24:05.000000 distributed-2023.4.1/docs/source/actors.rst
--rw-r--r--   0 james      (501) staff       (20)     4113 2022-10-21 17:45:03.000000 distributed-2023.4.1/docs/source/api.rst
--rw-r--r--   0 james      (501) staff       (20)     3519 2022-11-15 18:24:05.000000 distributed-2023.4.1/docs/source/asynchronous.rst
--rw-r--r--   0 james      (501) staff       (20)   253389 2023-04-28 17:20:35.000000 distributed-2023.4.1/docs/source/changelog.rst
--rw-r--r--   0 james      (501) staff       (20)     7084 2021-11-11 21:43:12.000000 distributed-2023.4.1/docs/source/client.rst
--rw-r--r--   0 james      (501) staff       (20)     3770 2021-11-11 17:33:04.000000 distributed-2023.4.1/docs/source/communications.rst
--rw-r--r--   0 james      (501) staff       (20)     7048 2022-08-08 21:17:38.000000 distributed-2023.4.1/docs/source/develop.rst
--rw-r--r--   0 james      (501) staff       (20)     6823 2022-10-21 17:45:03.000000 distributed-2023.4.1/docs/source/diagnosing-performance.rst
--rw-r--r--   0 james      (501) staff       (20)     3392 2022-10-21 17:45:03.000000 distributed-2023.4.1/docs/source/efficiency.rst
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-04-28 17:30:07.862225 distributed-2023.4.1/docs/source/examples/
--rw-r--r--   0 james      (501) staff       (20)     8953 2022-10-21 17:45:03.000000 distributed-2023.4.1/docs/source/examples/word-count.rst
--rw-r--r--   0 james      (501) staff       (20)       75 2020-06-30 15:19:20.000000 distributed-2023.4.1/docs/source/examples-overview.rst
--rw-r--r--   0 james      (501) staff       (20)     4228 2022-10-21 17:45:03.000000 distributed-2023.4.1/docs/source/faq.rst
--rw-r--r--   0 james      (501) staff       (20)     4613 2022-10-21 17:45:03.000000 distributed-2023.4.1/docs/source/foundations.rst
--rw-r--r--   0 james      (501) staff       (20)     4016 2022-10-21 17:45:03.000000 distributed-2023.4.1/docs/source/http_services.rst
--rw-r--r--   0 james      (501) staff       (20)     4423 2023-04-25 18:34:44.000000 distributed-2023.4.1/docs/source/index.rst
--rw-r--r--   0 james      (501) staff       (20)     1182 2022-08-08 21:17:38.000000 distributed-2023.4.1/docs/source/install.rst
--rw-r--r--   0 james      (501) staff       (20)     7293 2021-11-11 17:33:04.000000 distributed-2023.4.1/docs/source/journey.rst
--rw-r--r--   0 james      (501) staff       (20)     6470 2023-04-25 18:34:44.000000 distributed-2023.4.1/docs/source/killed.rst
--rw-r--r--   0 james      (501) staff       (20)     1828 2022-10-21 17:45:03.000000 distributed-2023.4.1/docs/source/limitations.rst
--rw-r--r--   0 james      (501) staff       (20)     6458 2022-10-21 17:45:03.000000 distributed-2023.4.1/docs/source/locality.rst
--rw-r--r--   0 james      (501) staff       (20)     2807 2021-11-11 17:33:04.000000 distributed-2023.4.1/docs/source/logging.rst
--rw-r--r--   0 james      (501) staff       (20)     6546 2021-07-06 20:52:40.000000 distributed-2023.4.1/docs/source/manage-computation.rst
--rw-r--r--   0 james      (501) staff       (20)     8550 2022-10-21 17:45:03.000000 distributed-2023.4.1/docs/source/memory.rst
--rw-r--r--   0 james      (501) staff       (20)     4100 2023-02-14 16:13:20.000000 distributed-2023.4.1/docs/source/plugins.rst
--rw-r--r--   0 james      (501) staff       (20)     3265 2021-11-11 21:43:12.000000 distributed-2023.4.1/docs/source/priority.rst
--rw-r--r--   0 james      (501) staff       (20)     7481 2023-04-26 17:04:39.000000 distributed-2023.4.1/docs/source/prometheus.rst
--rw-r--r--   0 james      (501) staff       (20)    11199 2022-10-21 17:45:03.000000 distributed-2023.4.1/docs/source/protocol.rst
--rw-r--r--   0 james      (501) staff       (20)     3107 2020-12-18 22:54:04.000000 distributed-2023.4.1/docs/source/publish.rst
--rw-r--r--   0 james      (501) staff       (20)      402 2023-04-25 18:34:44.000000 distributed-2023.4.1/docs/source/queues.rst
--rw-r--r--   0 james      (501) staff       (20)     2942 2022-10-21 17:45:03.000000 distributed-2023.4.1/docs/source/quickstart.rst
--rw-r--r--   0 james      (501) staff       (20)     8773 2022-10-21 17:45:03.000000 distributed-2023.4.1/docs/source/related-work.rst
--rw-r--r--   0 james      (501) staff       (20)     3418 2022-10-21 17:45:03.000000 distributed-2023.4.1/docs/source/resilience.rst
--rw-r--r--   0 james      (501) staff       (20)     6049 2022-11-15 18:24:05.000000 distributed-2023.4.1/docs/source/resources.rst
--rw-r--r--   0 james      (501) staff       (20)    16084 2023-04-25 18:34:44.000000 distributed-2023.4.1/docs/source/scheduling-policies.rst
--rw-r--r--   0 james      (501) staff       (20)    16901 2022-11-15 18:24:05.000000 distributed-2023.4.1/docs/source/scheduling-state.rst
--rw-r--r--   0 james      (501) staff       (20)     6518 2021-11-11 17:33:04.000000 distributed-2023.4.1/docs/source/serialization.rst
--rw-r--r--   0 james      (501) staff       (20)     8343 2022-08-08 21:17:38.000000 distributed-2023.4.1/docs/source/task-launch.rst
--rw-r--r--   0 james      (501) staff       (20)     4190 2022-10-21 17:45:03.000000 distributed-2023.4.1/docs/source/tls.rst
--rw-r--r--   0 james      (501) staff       (20)     5557 2021-11-11 17:33:04.000000 distributed-2023.4.1/docs/source/work-stealing.rst
--rw-r--r--   0 james      (501) staff       (20)    13489 2023-04-25 18:34:44.000000 distributed-2023.4.1/docs/source/worker-memory.rst
--rw-r--r--   0 james      (501) staff       (20)    22542 2023-04-25 18:34:44.000000 distributed-2023.4.1/docs/source/worker-state.rst
--rw-r--r--   0 james      (501) staff       (20)     3467 2022-10-21 17:45:03.000000 distributed-2023.4.1/docs/source/worker.rst
--rw-r--r--   0 james      (501) staff       (20)     9049 2023-04-28 17:21:01.000000 distributed-2023.4.1/pyproject.toml
--rw-r--r--   0 james      (501) staff       (20)       38 2023-04-28 17:30:07.864189 distributed-2023.4.1/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)      171 2023-04-26 17:04:39.000000 distributed-2023.4.1/setup.py
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.962293 distributed-2023.5.0/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      104 2019-09-09 13:11:44.000000 distributed-2023.5.0/AUTHORS.md
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1533 2022-08-02 08:55:18.000000 distributed-2023.5.0/LICENSE.txt
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      633 2023-05-12 15:12:44.000000 distributed-2023.5.0/MANIFEST.in
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     2882 2023-05-12 15:53:52.961881 distributed-2023.5.0/PKG-INFO
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1801 2022-08-02 08:55:18.000000 distributed-2023.5.0/README.rst
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.962784 distributed-2023.5.0/distributed/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     3836 2023-02-09 17:00:24.000000 distributed-2023.5.0/distributed/__init__.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     5528 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/_concurrent_futures_thread.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1297 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/_signals.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1372 2022-11-28 16:53:03.000000 distributed-2023.5.0/distributed/_stories.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      500 2023-05-12 15:53:52.962880 distributed-2023.5.0/distributed/_version.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    29277 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/active_memory_manager.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    10649 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/actor.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     7347 2022-08-17 10:33:17.000000 distributed-2023.5.0/distributed/batched.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      121 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/bokeh.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     5742 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/cfexecutor.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1947 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/chaos.py
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.703605 distributed-2023.5.0/distributed/cli/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)        0 2019-09-09 13:13:25.000000 distributed-2023.5.0/distributed/cli/__init__.py
+-rwxr-xr-x   0 jtomlinson   (502) staff       (20)     7077 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/cli/dask_scheduler.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1269 2023-02-09 17:00:24.000000 distributed-2023.5.0/distributed/cli/dask_spec.py
+-rwxr-xr-x   0 jtomlinson   (502) staff       (20)     5468 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/cli/dask_ssh.py
+-rwxr-xr-x   0 jtomlinson   (502) staff       (20)    15948 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/cli/dask_worker.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1092 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/cli/utils.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)   201985 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/client.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    10985 2022-11-28 16:53:03.000000 distributed-2023.5.0/distributed/cluster_dump.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     6717 2023-02-09 17:00:24.000000 distributed-2023.5.0/distributed/collections.py
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.724113 distributed-2023.5.0/distributed/comm/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1285 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/comm/__init__.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     8597 2022-08-17 10:33:17.000000 distributed-2023.5.0/distributed/comm/addressing.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    37224 2023-02-09 17:00:24.000000 distributed-2023.5.0/distributed/comm/asyncio_tcp.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    13369 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/comm/core.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    10321 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/comm/inproc.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     2815 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/comm/registry.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    24495 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/comm/tcp.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    22962 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/comm/ucx.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     4220 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/comm/utils.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    14868 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/comm/ws.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     7959 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/compatibility.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     7357 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/config.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    58993 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/core.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     2146 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/counter.py
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.731410 distributed-2023.5.0/distributed/dashboard/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)        0 2021-06-02 14:34:47.000000 distributed-2023.5.0/distributed/dashboard/__init__.py
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.740536 distributed-2023.5.0/distributed/dashboard/components/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1550 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/dashboard/components/__init__.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     5818 2022-11-28 16:53:03.000000 distributed-2023.5.0/distributed/dashboard/components/nvml.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     7055 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/dashboard/components/rmm.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)   146950 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/dashboard/components/scheduler.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    19467 2023-02-09 17:00:24.000000 distributed-2023.5.0/distributed/dashboard/components/shared.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    15424 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/dashboard/components/worker.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1786 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/dashboard/core.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     2313 2019-09-09 13:13:25.000000 distributed-2023.5.0/distributed/dashboard/export_tool.js
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      763 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/dashboard/export_tool.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     5717 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/dashboard/scheduler.py
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.742124 distributed-2023.5.0/distributed/dashboard/templates/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/dashboard/templates/__init__.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      241 2022-08-02 08:25:26.000000 distributed-2023.5.0/distributed/dashboard/templates/performance_report.html
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      199 2022-08-02 08:25:26.000000 distributed-2023.5.0/distributed/dashboard/theme.yaml
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1668 2023-02-09 17:00:24.000000 distributed-2023.5.0/distributed/dashboard/utils.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      840 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/dashboard/worker.py
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.809759 distributed-2023.5.0/distributed/deploy/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      466 2023-02-09 17:00:24.000000 distributed-2023.5.0/distributed/deploy/__init__.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     6702 2022-11-28 16:53:03.000000 distributed-2023.5.0/distributed/deploy/adaptive.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     7802 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/deploy/adaptive_core.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    21498 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/deploy/cluster.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    10434 2022-11-28 16:53:03.000000 distributed-2023.5.0/distributed/deploy/local.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    15514 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/deploy/old_ssh.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    23732 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/deploy/spec.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    15265 2022-11-28 16:53:03.000000 distributed-2023.5.0/distributed/deploy/ssh.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     7656 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/deploy/subprocess.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      888 2022-11-28 16:53:03.000000 distributed-2023.5.0/distributed/deploy/utils.py
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.826585 distributed-2023.5.0/distributed/diagnostics/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      221 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/diagnostics/__init__.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1302 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/diagnostics/cluster_dump.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     2190 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/diagnostics/eventstream.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     4994 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/diagnostics/graph_layout.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     6972 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/diagnostics/memory_sampler.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    10781 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/diagnostics/nvml.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    28172 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/diagnostics/plugin.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    12565 2022-11-28 16:53:03.000000 distributed-2023.5.0/distributed/diagnostics/progress.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     6063 2022-11-28 16:53:03.000000 distributed-2023.5.0/distributed/diagnostics/progress_stream.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    14665 2022-11-28 16:53:03.000000 distributed-2023.5.0/distributed/diagnostics/progressbar.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1124 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/diagnostics/rmm.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     5677 2022-11-28 16:53:03.000000 distributed-2023.5.0/distributed/diagnostics/task_stream.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     2434 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/diagnostics/websocket.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     9172 2022-11-28 16:53:03.000000 distributed-2023.5.0/distributed/diskutils.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    46226 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/distributed-schema.yaml
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    14146 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/distributed.yaml
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     8536 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/event.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      586 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/exceptions.py
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.837097 distributed-2023.5.0/distributed/http/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)       84 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/http/__init__.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      258 2022-08-02 08:32:00.000000 distributed-2023.5.0/distributed/http/health.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1480 2022-11-28 16:53:03.000000 distributed-2023.5.0/distributed/http/prometheus.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     4377 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/http/proxy.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     2548 2022-08-02 15:50:17.000000 distributed-2023.5.0/distributed/http/routing.py
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.841936 distributed-2023.5.0/distributed/http/scheduler/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)        0 2021-06-02 14:34:47.000000 distributed-2023.5.0/distributed/http/scheduler/__init__.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     2899 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/http/scheduler/api.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     6926 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/http/scheduler/info.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     2159 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/http/scheduler/json.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      625 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/http/scheduler/missing_bokeh.py
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.847537 distributed-2023.5.0/distributed/http/scheduler/prometheus/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      291 2022-11-28 16:53:03.000000 distributed-2023.5.0/distributed/http/scheduler/prometheus/__init__.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     7049 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/http/scheduler/prometheus/core.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     3514 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/http/scheduler/prometheus/semaphore.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1617 2022-11-28 16:53:03.000000 distributed-2023.5.0/distributed/http/scheduler/prometheus/stealing.py
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.849140 distributed-2023.5.0/distributed/http/static/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/http/static/__init__.py
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.855940 distributed-2023.5.0/distributed/http/static/css/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/http/static/css/__init__.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     2260 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/http/static/css/base.css
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      250 2022-08-02 08:25:26.000000 distributed-2023.5.0/distributed/http/static/css/gpu.css
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      840 2021-06-02 14:34:47.000000 distributed-2023.5.0/distributed/http/static/css/individual-cluster-map.css
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1012 2022-08-02 08:25:26.000000 distributed-2023.5.0/distributed/http/static/css/status.css
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.864971 distributed-2023.5.0/distributed/http/static/images/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/http/static/images/__init__.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1607 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/http/static/images/dask-logo.svg
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      552 2021-06-02 14:34:47.000000 distributed-2023.5.0/distributed/http/static/images/fa-bars.svg
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    15086 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/http/static/images/favicon.ico
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    11002 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/http/static/images/jupyter.svg
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    18663 2022-08-02 08:25:26.000000 distributed-2023.5.0/distributed/http/static/images/numpy.png
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1213 2022-08-02 08:25:26.000000 distributed-2023.5.0/distributed/http/static/images/pandas.png
+-rw-r--r--   0 jtomlinson   (502) staff       (20)   830916 2022-08-02 08:25:26.000000 distributed-2023.5.0/distributed/http/static/images/python.png
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      667 2021-06-02 14:34:47.000000 distributed-2023.5.0/distributed/http/static/individual-cluster-map.html
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.871436 distributed-2023.5.0/distributed/http/static/js/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/http/static/js/__init__.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    17271 2021-06-02 14:34:47.000000 distributed-2023.5.0/distributed/http/static/js/anime.min.js
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     9337 2021-06-02 14:34:47.000000 distributed-2023.5.0/distributed/http/static/js/individual-cluster-map.js
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     3276 2021-06-02 14:34:47.000000 distributed-2023.5.0/distributed/http/static/js/reconnecting-websocket.min.js
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      223 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/http/statics.py
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.883706 distributed-2023.5.0/distributed/http/templates/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/http/templates/__init__.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     2930 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/http/templates/base.html
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      388 2021-06-02 14:34:47.000000 distributed-2023.5.0/distributed/http/templates/call-stack.html
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1351 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/http/templates/exceptions.html
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      404 2022-08-02 08:25:26.000000 distributed-2023.5.0/distributed/http/templates/gpu.html
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      276 2021-06-02 14:34:47.000000 distributed-2023.5.0/distributed/http/templates/json-index.html
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      116 2021-06-02 14:34:47.000000 distributed-2023.5.0/distributed/http/templates/logs.html
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      369 2021-06-02 14:34:47.000000 distributed-2023.5.0/distributed/http/templates/main.html
+-rw-r--r--   0 jtomlinson   (502) staff       (20)       95 2021-06-02 14:34:47.000000 distributed-2023.5.0/distributed/http/templates/simple.html
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      635 2022-08-02 08:25:26.000000 distributed-2023.5.0/distributed/http/templates/status.html
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     5672 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/http/templates/task.html
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1405 2021-06-02 14:34:47.000000 distributed-2023.5.0/distributed/http/templates/worker-table.html
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     2024 2021-06-02 14:34:47.000000 distributed-2023.5.0/distributed/http/templates/worker.html
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      457 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/http/templates/workers.html
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1184 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/http/utils.py
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.884639 distributed-2023.5.0/distributed/http/worker/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)        0 2021-06-02 14:34:47.000000 distributed-2023.5.0/distributed/http/worker/__init__.py
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.886190 distributed-2023.5.0/distributed/http/worker/prometheus/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      288 2022-11-28 16:53:03.000000 distributed-2023.5.0/distributed/http/worker/prometheus/__init__.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     9973 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/http/worker/prometheus/core.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     5599 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/lock.py
+-rwxr-xr-x   0 jtomlinson   (502) staff       (20)    12252 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/metrics.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     8044 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/multi_lock.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    33721 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/nanny.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     6710 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/node.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1449 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/objects.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     7513 2022-11-28 16:53:03.000000 distributed-2023.5.0/distributed/preloading.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    12887 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/process.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      931 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/proctitle.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    16141 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/profile.py
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.901586 distributed-2023.5.0/distributed/protocol/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     3363 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/protocol/__init__.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1336 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/protocol/arrow.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     6671 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/protocol/compression.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     5964 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/protocol/core.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1181 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/protocol/cuda.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     2788 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/protocol/cupy.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      836 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/protocol/h5py.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1127 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/protocol/keras.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1466 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/protocol/netcdf4.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     2139 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/protocol/numba.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     6664 2023-02-09 17:00:24.000000 distributed-2023.5.0/distributed/protocol/numpy.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     3043 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/protocol/pickle.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1507 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/protocol/rmm.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      800 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/protocol/scipy.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    29121 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/protocol/serialize.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      955 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/protocol/sparse.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1993 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/protocol/torch.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     6102 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/protocol/utils.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     3733 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/publish.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    15652 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/pubsub.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)        0 2022-08-02 08:32:00.000000 distributed-2023.5.0/distributed/py.typed
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    10082 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/queues.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     7620 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/recreate_tasks.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)   302091 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/scheduler.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    13825 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/security.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    20568 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/semaphore.py
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.910990 distributed-2023.5.0/distributed/shuffle/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      692 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/shuffle/__init__.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     2948 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/shuffle/_arrow.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     9212 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/shuffle/_buffer.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     2499 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/shuffle/_comms.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     3550 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/shuffle/_disk.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     2361 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/shuffle/_limiter.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    11854 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/shuffle/_merge.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     5030 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/shuffle/_rechunk.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    12834 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/shuffle/_scheduler_extension.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     8218 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/shuffle/_shuffle.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    33686 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/shuffle/_worker_extension.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      607 2022-08-02 08:55:18.000000 distributed-2023.5.0/distributed/sizeof.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    13597 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/spill.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    19859 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/stealing.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1883 2022-11-28 16:53:03.000000 distributed-2023.5.0/distributed/system.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     8532 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/system_monitor.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     7104 2022-08-02 08:55:19.000000 distributed-2023.5.0/distributed/threadpoolexecutor.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    55458 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/utils.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    13992 2023-03-16 13:18:33.000000 distributed-2023.5.0/distributed/utils_comm.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     8050 2023-02-09 17:00:24.000000 distributed-2023.5.0/distributed/utils_perf.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    80577 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/utils_test.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     8463 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/variable.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     5194 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/versions.py
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.912022 distributed-2023.5.0/distributed/widgets/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      267 2022-11-28 16:53:03.000000 distributed-2023.5.0/distributed/widgets/__init__.py
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.925695 distributed-2023.5.0/distributed/widgets/templates/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/widgets/templates/__init__.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     2265 2022-11-28 16:53:03.000000 distributed-2023.5.0/distributed/widgets/templates/client.html.j2
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1589 2022-08-02 08:27:54.000000 distributed-2023.5.0/distributed/widgets/templates/cluster.html.j2
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1270 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/widgets/templates/computation.html.j2
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      518 2022-08-02 08:25:26.000000 distributed-2023.5.0/distributed/widgets/templates/future.html.j2
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      544 2022-08-02 08:25:26.000000 distributed-2023.5.0/distributed/widgets/templates/has_what.html.j2
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      234 2022-08-02 08:25:26.000000 distributed-2023.5.0/distributed/widgets/templates/local_cluster.html.j2
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      636 2022-08-02 08:25:26.000000 distributed-2023.5.0/distributed/widgets/templates/log.html.j2
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      168 2022-08-02 08:25:26.000000 distributed-2023.5.0/distributed/widgets/templates/logs.html.j2
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1290 2022-08-02 08:27:54.000000 distributed-2023.5.0/distributed/widgets/templates/process_interface.html.j2
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      317 2022-08-02 08:25:26.000000 distributed-2023.5.0/distributed/widgets/templates/scheduler.html.j2
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     6705 2022-11-28 16:53:03.000000 distributed-2023.5.0/distributed/widgets/templates/scheduler_info.html.j2
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      407 2022-08-02 08:27:54.000000 distributed-2023.5.0/distributed/widgets/templates/security.html.j2
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      448 2022-08-02 08:25:26.000000 distributed-2023.5.0/distributed/widgets/templates/task_state.html.j2
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      295 2022-08-02 08:25:26.000000 distributed-2023.5.0/distributed/widgets/templates/who_has.html.j2
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      407 2022-08-02 08:32:00.000000 distributed-2023.5.0/distributed/widgets/templates/worker_state.html.j2
+-rw-r--r--   0 jtomlinson   (502) staff       (20)   124811 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/worker.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     2276 2023-02-09 17:00:24.000000 distributed-2023.5.0/distributed/worker_client.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    21367 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/worker_memory.py
+-rw-r--r--   0 jtomlinson   (502) staff       (20)   141533 2023-05-12 15:12:44.000000 distributed-2023.5.0/distributed/worker_state_machine.py
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.688453 distributed-2023.5.0/distributed.egg-info/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     2882 2023-05-12 15:53:52.000000 distributed-2023.5.0/distributed.egg-info/PKG-INFO
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     8573 2023-05-12 15:53:52.000000 distributed-2023.5.0/distributed.egg-info/SOURCES.txt
+-rw-r--r--   0 jtomlinson   (502) staff       (20)        1 2023-05-12 15:53:52.000000 distributed-2023.5.0/distributed.egg-info/dependency_links.txt
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      335 2023-05-12 15:53:52.000000 distributed-2023.5.0/distributed.egg-info/entry_points.txt
+-rw-r--r--   0 jtomlinson   (502) staff       (20)        1 2023-05-12 15:53:51.000000 distributed-2023.5.0/distributed.egg-info/not-zip-safe
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      227 2023-05-12 15:53:52.000000 distributed-2023.5.0/distributed.egg-info/requires.txt
+-rw-r--r--   0 jtomlinson   (502) staff       (20)       12 2023-05-12 15:53:52.000000 distributed-2023.5.0/distributed.egg-info/top_level.txt
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.587384 distributed-2023.5.0/docs/
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.960296 distributed-2023.5.0/docs/source/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    11754 2022-11-28 16:53:03.000000 distributed-2023.5.0/docs/source/active_memory_manager.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     8000 2022-11-28 16:53:03.000000 distributed-2023.5.0/docs/source/actors.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     4113 2022-11-28 16:53:03.000000 distributed-2023.5.0/docs/source/api.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     3519 2022-11-28 16:53:03.000000 distributed-2023.5.0/docs/source/asynchronous.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)   254647 2023-05-12 15:39:49.000000 distributed-2023.5.0/docs/source/changelog.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     7084 2022-08-02 08:25:26.000000 distributed-2023.5.0/docs/source/client.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     3770 2021-06-02 14:34:47.000000 distributed-2023.5.0/docs/source/communications.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     7048 2022-08-02 08:32:00.000000 distributed-2023.5.0/docs/source/develop.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     6823 2022-11-28 16:53:03.000000 distributed-2023.5.0/docs/source/diagnosing-performance.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     3392 2022-11-28 16:53:03.000000 distributed-2023.5.0/docs/source/efficiency.rst
+drwxr-xr-x   0 jtomlinson   (502) staff       (20)        0 2023-05-12 15:53:52.960998 distributed-2023.5.0/docs/source/examples/
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     8953 2022-08-02 08:55:19.000000 distributed-2023.5.0/docs/source/examples/word-count.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)       75 2019-09-09 13:13:25.000000 distributed-2023.5.0/docs/source/examples-overview.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     4228 2022-11-28 16:53:03.000000 distributed-2023.5.0/docs/source/faq.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     4613 2022-08-02 08:55:19.000000 distributed-2023.5.0/docs/source/foundations.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     4016 2022-08-02 08:55:19.000000 distributed-2023.5.0/docs/source/http_services.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     4423 2023-02-09 17:00:24.000000 distributed-2023.5.0/docs/source/index.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1182 2022-08-02 08:32:00.000000 distributed-2023.5.0/docs/source/install.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     7293 2021-06-02 14:34:47.000000 distributed-2023.5.0/docs/source/journey.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     6470 2023-05-12 15:12:44.000000 distributed-2023.5.0/docs/source/killed.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     1828 2022-11-28 16:53:03.000000 distributed-2023.5.0/docs/source/limitations.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     6458 2022-11-28 16:53:03.000000 distributed-2023.5.0/docs/source/locality.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     2807 2022-01-14 14:33:02.000000 distributed-2023.5.0/docs/source/logging.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     6546 2019-09-18 12:29:39.000000 distributed-2023.5.0/docs/source/manage-computation.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     8550 2022-08-02 08:55:19.000000 distributed-2023.5.0/docs/source/memory.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     4100 2022-11-28 16:53:03.000000 distributed-2023.5.0/docs/source/plugins.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     3265 2022-08-02 08:25:26.000000 distributed-2023.5.0/docs/source/priority.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     7481 2023-05-12 15:12:44.000000 distributed-2023.5.0/docs/source/prometheus.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    11199 2022-08-02 08:55:19.000000 distributed-2023.5.0/docs/source/protocol.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     3107 2019-09-09 13:13:25.000000 distributed-2023.5.0/docs/source/publish.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      402 2023-05-12 15:12:44.000000 distributed-2023.5.0/docs/source/queues.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     2942 2022-11-28 16:53:03.000000 distributed-2023.5.0/docs/source/quickstart.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     8773 2022-08-02 08:55:19.000000 distributed-2023.5.0/docs/source/related-work.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     3418 2022-11-28 16:53:03.000000 distributed-2023.5.0/docs/source/resilience.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     6049 2022-11-28 16:53:03.000000 distributed-2023.5.0/docs/source/resources.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    16084 2022-11-28 16:53:03.000000 distributed-2023.5.0/docs/source/scheduling-policies.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    16901 2022-11-28 16:53:03.000000 distributed-2023.5.0/docs/source/scheduling-state.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     6518 2021-06-02 14:34:47.000000 distributed-2023.5.0/docs/source/serialization.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     8343 2022-08-02 08:27:54.000000 distributed-2023.5.0/docs/source/task-launch.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     4190 2022-11-28 16:53:03.000000 distributed-2023.5.0/docs/source/tls.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     5557 2019-09-18 12:29:43.000000 distributed-2023.5.0/docs/source/work-stealing.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    13489 2023-02-09 17:00:24.000000 distributed-2023.5.0/docs/source/worker-memory.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)    22542 2023-05-12 15:12:44.000000 distributed-2023.5.0/docs/source/worker-state.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     3467 2022-11-28 16:53:03.000000 distributed-2023.5.0/docs/source/worker.rst
+-rw-r--r--   0 jtomlinson   (502) staff       (20)     9049 2023-05-12 15:29:23.000000 distributed-2023.5.0/pyproject.toml
+-rw-r--r--   0 jtomlinson   (502) staff       (20)       38 2023-05-12 15:53:52.962408 distributed-2023.5.0/setup.cfg
+-rw-r--r--   0 jtomlinson   (502) staff       (20)      171 2023-05-12 15:12:44.000000 distributed-2023.5.0/setup.py
```

### Comparing `distributed-2023.4.1/LICENSE.txt` & `distributed-2023.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/MANIFEST.in` & `distributed-2023.5.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/PKG-INFO` & `distributed-2023.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distributed
-Version: 2023.4.1
+Version: 2023.5.0
 Summary: Distributed scheduler for Dask
 Maintainer-email: Matthew Rocklin <mrocklin@gmail.com>
 License: BSD
 Project-URL: Homepage, https://distributed.dask.org
 Project-URL: Source, https://github.com/dask/distributed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `distributed-2023.4.1/README.rst` & `distributed-2023.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/__init__.py` & `distributed-2023.5.0/distributed/__init__.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/_concurrent_futures_thread.py` & `distributed-2023.5.0/distributed/_concurrent_futures_thread.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/_signals.py` & `distributed-2023.5.0/distributed/_signals.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/_stories.py` & `distributed-2023.5.0/distributed/_stories.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/active_memory_manager.py` & `distributed-2023.5.0/distributed/active_memory_manager.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/actor.py` & `distributed-2023.5.0/distributed/actor.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/batched.py` & `distributed-2023.5.0/distributed/batched.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/cfexecutor.py` & `distributed-2023.5.0/distributed/cfexecutor.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/chaos.py` & `distributed-2023.5.0/distributed/chaos.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/cli/dask_scheduler.py` & `distributed-2023.5.0/distributed/cli/dask_scheduler.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/cli/dask_spec.py` & `distributed-2023.5.0/distributed/cli/dask_spec.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/cli/dask_ssh.py` & `distributed-2023.5.0/distributed/cli/dask_ssh.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/cli/dask_worker.py` & `distributed-2023.5.0/distributed/cli/dask_worker.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/cli/utils.py` & `distributed-2023.5.0/distributed/cli/utils.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/client.py` & `distributed-2023.5.0/distributed/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     parse_timedelta,
     stringify,
     typename,
 )
 from dask.widgets import get_template
 
 from distributed.core import ErrorMessage
+from distributed.protocol.serialize import _is_dumpable
 from distributed.utils import wait_for
 
 try:
     from dask.delayed import single_key
 except ImportError:
     single_key = first
 from tornado import gen
@@ -70,14 +71,15 @@
     clean_exception,
     connect,
     rpc,
 )
 from distributed.diagnostics.plugin import (
     ForwardLoggingPlugin,
     NannyPlugin,
+    SchedulerUploadFile,
     UploadFile,
     WorkerPlugin,
     _get_plugin_name,
 )
 from distributed.metrics import time
 from distributed.objects import HasWhat, SchedulerInfo, WhoHas
 from distributed.protocol import to_serialize
@@ -2011,20 +2013,20 @@
             See :doc:`actors` for additional details.
         actors : bool (default False)
             Alias for `actor`
         pure : bool (defaults to True)
             Whether or not the function is pure.  Set ``pure=False`` for
             impure functions like ``np.random.random``.
             See :ref:`pure functions` for more details.
-        batch_size : int, optional
+        batch_size : int, optional (default: just one batch whose size is the entire iterable)
             Submit tasks to the scheduler in batches of (at most)
             ``batch_size``.
-            Larger batch sizes can be useful for very large ``iterables``,
-            as the cluster can start processing tasks while later ones are
-            submitted asynchronously.
+            The tradeoff in batch size is that large batches avoid more per-batch overhead,
+            but batches that are too big can take a long time to submit and unreasonably delay
+            the cluster from starting its processing.
         **kwargs : dict
             Extra keyword arguments to send to the function.
             Large values will be included explicitly in the task graph.
 
         Examples
         --------
         >>> L = client.map(func, sequence)  # doctest: +SKIP
@@ -3730,18 +3732,26 @@
 
         Examples
         --------
         >>> client.upload_file('mylibrary.egg')  # doctest: +SKIP
         >>> from mylibrary import myfunc  # doctest: +SKIP
         >>> L = client.map(myfunc, seq)  # doctest: +SKIP
         """
-        return self.register_worker_plugin(
-            UploadFile(filename),
-            name=filename + str(uuid.uuid4()),
-        )
+        name = filename + str(uuid.uuid4())
+
+        async def _():
+            results = await asyncio.gather(
+                self.register_scheduler_plugin(
+                    SchedulerUploadFile(filename), name=name
+                ),
+                self.register_worker_plugin(UploadFile(filename), name=name),
+            )
+            return results[1]  # Results from workers upload
+
+        return self.sync(_)
 
     async def _rebalance(self, futures=None, workers=None):
         if futures is not None:
             await _wait(futures)
             keys = list({stringify(f.key) for f in self.futures_of(futures)})
         else:
             keys = None
@@ -4399,14 +4409,18 @@
             Event message to log. Note this must be msgpack serializable.
 
         Examples
         --------
         >>> from time import time
         >>> client.log_event("current-time", time())
         """
+        if not _is_dumpable(msg):
+            raise TypeError(
+                f"Message must be msgpack serializable. Got {type(msg)=} instead."
+            )
         return self.sync(self.scheduler.log_event, topic=topic, msg=msg)
 
     def get_events(self, topic: str | None = None):
         """Retrieve structured topic logs
 
         Parameters
         ----------
```

### Comparing `distributed-2023.4.1/distributed/cluster_dump.py` & `distributed-2023.5.0/distributed/cluster_dump.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/collections.py` & `distributed-2023.5.0/distributed/collections.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/comm/__init__.py` & `distributed-2023.5.0/distributed/comm/__init__.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/comm/addressing.py` & `distributed-2023.5.0/distributed/comm/addressing.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/comm/asyncio_tcp.py` & `distributed-2023.5.0/distributed/comm/asyncio_tcp.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/comm/core.py` & `distributed-2023.5.0/distributed/comm/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from contextlib import suppress
 from typing import Any, ClassVar
 
 import dask
 from dask.utils import parse_timedelta
 
 from distributed.comm import registry
-from distributed.comm.addressing import parse_address
+from distributed.comm.addressing import get_address_host, parse_address, resolve_address
 from distributed.metrics import time
-from distributed.protocol.compression import get_default_compression
+from distributed.protocol.compression import get_compression_settings
 from distributed.protocol.pickle import HIGHEST_PROTOCOL
 from distributed.utils import wait_for
 
 logger = logging.getLogger(__name__)
 
 
 class CommClosedError(IOError):
@@ -109,40 +109,84 @@
     @abstractmethod
     def closed(self):
         """Return whether the stream is closed."""
 
     @property
     @abstractmethod
     def local_address(self) -> str:
-        """The local address. For logging and debugging purposes only."""
+        """The local address"""
 
     @property
     @abstractmethod
     def peer_address(self) -> str:
-        """The peer's address. For logging and debugging purposes only."""
+        """The peer's address"""
+
+    @property
+    def same_host(self) -> bool:
+        """Return True if the peer is on localhost; False otherwise"""
+        local_ipaddr = get_address_host(resolve_address(self.local_address))
+        peer_ipaddr = get_address_host(resolve_address(self.peer_address))
+
+        # Note: this is not the same as testing `peer_ipaddr == "127.0.0.1"`.
+        # When you start a Server, by default it starts listening on the LAN interface,
+        # so its advertised address will be 10.x or 192.168.x.
+        return local_ipaddr == peer_ipaddr
 
     @property
     def extra_info(self):
         """
         Return backend-specific information about the communication,
         as a dict.  Typically, this is information which is initialized
         when the communication is established and doesn't vary afterwards.
         """
         return {}
 
-    @staticmethod
-    def handshake_info():
+    def handshake_info(self) -> dict[str, Any]:
+        """Share environment information with the peer that may differ, i.e. compression
+        settings.
+
+        Notes
+        -----
+        By the time this method runs, the "auto" compression setting has been updated to
+        an actual compression algorithm. This matters if both peers had compression set
+        to 'auto' but only one has lz4 installed. See
+        distributed.protocol.compression._update_and_check_compression_settings()
+
+        See also
+        --------
+        handshake_configuration
+        """
+        if self.same_host:
+            compression = None
+        else:
+            compression = get_compression_settings("distributed.comm.compression")
+
         return {
-            "compression": get_default_compression(),
+            "compression": compression,
             "python": tuple(sys.version_info)[:3],
             "pickle-protocol": HIGHEST_PROTOCOL,
         }
 
     @staticmethod
-    def handshake_configuration(local, remote):
+    def handshake_configuration(
+        local: dict[str, Any], remote: dict[str, Any]
+    ) -> dict[str, Any]:
+        """Find a configuration that is suitable for both local and remote
+
+        Parameters
+        ----------
+        local
+            Output of handshake_info() in this process
+        remote
+            Output of handshake_info() on the remote host
+
+        See also
+        --------
+        handshake_info
+        """
         try:
             out = {
                 "pickle-protocol": min(
                     local["pickle-protocol"], remote["pickle-protocol"]
                 )
             }
         except KeyError as e:
```

### Comparing `distributed-2023.4.1/distributed/comm/inproc.py` & `distributed-2023.5.0/distributed/comm/inproc.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,18 @@
     def local_address(self) -> str:
         return self._local_addr
 
     @property
     def peer_address(self) -> str:
         return self._peer_addr
 
+    @property
+    def same_host(self) -> bool:
+        return True
+
     async def read(self, deserializers="ignored"):
         if self._closed:
             raise CommClosedError()
 
         msg = await self._read_q.get()
         if msg is _EOF:
             self._closed = True
```

### Comparing `distributed-2023.4.1/distributed/comm/registry.py` & `distributed-2023.5.0/distributed/comm/registry.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/comm/tcp.py` & `distributed-2023.5.0/distributed/comm/tcp.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/comm/ucx.py` & `distributed-2023.5.0/distributed/comm/ucx.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,14 +274,19 @@
     def local_address(self) -> str:
         return self._local_addr
 
     @property
     def peer_address(self) -> str:
         return self._peer_addr
 
+    @property
+    def same_host(self) -> bool:
+        """Unlike in TCP, local_address can be blank"""
+        return super().same_host if self._local_addr else False
+
     @log_errors
     async def write(
         self,
         msg: dict,
         serializers: Collection[str] | None = None,
         on_error: str = "message",
     ) -> int:
```

### Comparing `distributed-2023.4.1/distributed/comm/utils.py` & `distributed-2023.5.0/distributed/comm/utils.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/comm/ws.py` & `distributed-2023.5.0/distributed/comm/ws.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import asyncio
 import logging
+import socket
 import struct
 import warnings
 import weakref
 from collections.abc import Callable
 from ssl import SSLError
 from typing import Any
 
@@ -169,14 +170,24 @@
 
     @property
     def peer_address(self) -> str:
         ip = self.handler.request.remote_ip
         assert isinstance(ip, str)
         return ip + ":0"
 
+    @property
+    def same_host(self) -> bool:
+        """Override Comm.same_host, adding support for HTTP-only subdomains, which won't
+        have a port and that may not be known to the DNS service
+        """
+        try:
+            return super().same_host
+        except (ValueError, socket.gaierror):
+            return False
+
     def closed(self):
         return (
             self.handler.closed
             or not self.handler.ws_connection
             or self.handler.request.connection.stream
             and self.handler.request.connection.stream.closed
         )
@@ -281,14 +292,24 @@
     def local_address(self) -> str:
         return f"{self.prefix}{self.sock.parsed.netloc}"
 
     @property
     def peer_address(self) -> str:
         return f"{self.prefix}{self.sock.parsed.netloc}"
 
+    @property
+    def same_host(self) -> bool:
+        """Override Comm.same_host, adding support for HTTP-only subdomains, which won't
+        have a port and that may not be known to the DNS service
+        """
+        try:
+            return super().same_host
+        except (ValueError, socket.gaierror):
+            return False
+
     def _read_extra(self):
         pass
 
     @property
     def extra_info(self):
         return self._extra
```

### Comparing `distributed-2023.4.1/distributed/compatibility.py` & `distributed-2023.5.0/distributed/compatibility.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/config.py` & `distributed-2023.5.0/distributed/config.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/core.py` & `distributed-2023.5.0/distributed/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 import asyncio
 import inspect
 import logging
+import os
 import sys
+import tempfile
 import threading
 import traceback
 import types
 import uuid
 import warnings
 import weakref
 from collections import defaultdict, deque
@@ -20,46 +22,67 @@
 from tlz import merge
 from tornado.ioloop import IOLoop
 
 import dask
 from dask.utils import parse_timedelta
 
 from distributed import profile, protocol
+from distributed.collections import LRU
 from distributed.comm import (
     Comm,
     CommClosedError,
     connect,
     get_address_host_port,
     listen,
     normalize_address,
     unparse_host_port,
 )
 from distributed.compatibility import PeriodicCallback
 from distributed.counter import Counter
+from distributed.diskutils import WorkDir, WorkSpace
 from distributed.metrics import context_meter, time
+from distributed.protocol import pickle
 from distributed.system_monitor import SystemMonitor
 from distributed.utils import (
     NoOpAwaitable,
     get_traceback,
     has_keyword,
+    import_file,
     iscoroutinefunction,
+    offload,
     recursive_to_dict,
     truncate_exception,
     wait_for,
+    warn_on_duration,
 )
 
 if TYPE_CHECKING:
     from typing_extensions import ParamSpec, Self
 
     P = ParamSpec("P")
     R = TypeVar("R")
     T = TypeVar("T")
     Coro = Coroutine[Any, Any, T]
 
 
+cache_loads = LRU(maxsize=100)
+
+
+def loads_function(bytes_object):
+    """Load a function from bytes, cache bytes"""
+    if len(bytes_object) < 100000:
+        try:
+            result = cache_loads[bytes_object]
+        except KeyError:
+            result = pickle.loads(bytes_object)
+            cache_loads[bytes_object] = result
+        return result
+    return pickle.loads(bytes_object)
+
+
 class Status(Enum):
     """
     This Enum contains the various states a cluster, worker, scheduler and nanny can be
     in. Some of the status can only be observed in one of cluster, nanny, scheduler or
     worker but we put them in the same Enum as they are compared with each
     other.
     """
@@ -299,28 +322,63 @@
     *  ``{'op': 'ping'}``
     *  ``{'op': 'add', 'x': 10, 'y': 20}``
 
     """
 
     default_ip = ""
     default_port = 0
+    local_directory: str
+    _workspace: WorkSpace
+    _workdir: None | WorkDir
 
     def __init__(
         self,
         handlers,
         blocked_handlers=None,
         stream_handlers=None,
         connection_limit=512,
         deserialize=True,
         serializers=None,
         deserializers=None,
         connection_args=None,
         timeout=None,
         io_loop=None,
+        local_directory=None,
+        needs_workdir=True,
     ):
+        if local_directory is None:
+            local_directory = (
+                dask.config.get("temporary-directory") or tempfile.gettempdir()
+            )
+
+        if "dask-scratch-space" not in str(local_directory):
+            local_directory = os.path.join(local_directory, "dask-scratch-space")
+
+        self._original_local_dir = local_directory
+
+        with warn_on_duration(
+            "1s",
+            "Creating scratch directories is taking a surprisingly long time. ({duration:.2f}s) "
+            "This is often due to running workers on a network file system. "
+            "Consider specifying a local-directory to point workers to write "
+            "scratch data to a local disk.",
+        ):
+            self._workspace = WorkSpace(local_directory)
+
+            if not needs_workdir:  # eg. Nanny will not need a WorkDir
+                self._workdir = None
+                self.local_directory = self._workspace.base_dir
+            else:
+                name = type(self).__name__.lower()
+                self._workdir = self._workspace.new_work_dir(prefix=f"{name}-")
+                self.local_directory = self._workdir.dir_path
+
+        if self.local_directory not in sys.path:
+            sys.path.insert(0, self.local_directory)
+
         if io_loop is not None:
             warnings.warn(
                 "The io_loop kwarg to Server is ignored and will be deprecated",
                 DeprecationWarning,
                 stacklevel=2,
             )
 
@@ -433,14 +491,43 @@
             connection_args=connection_args,
             timeout=timeout,
             server=self,
         )
 
         self.__stopped = False
 
+    async def upload_file(
+        self, filename: str, data: str | bytes, load: bool = True
+    ) -> dict[str, Any]:
+        out_filename = os.path.join(self.local_directory, filename)
+
+        def func(data):
+            if isinstance(data, str):
+                data = data.encode()
+            with open(out_filename, "wb") as f:
+                f.write(data)
+                f.flush()
+                os.fsync(f.fileno())
+            return data
+
+        if len(data) < 10000:
+            data = func(data)
+        else:
+            data = await offload(func, data)
+
+        if load:
+            try:
+                import_file(out_filename)
+                cache_loads.data.clear()
+            except Exception as e:
+                logger.exception(e)
+                raise e
+
+        return {"status": "OK", "nbytes": len(data)}
+
     def _shift_counters(self):
         for counter in self.counters.values():
             counter.shift()
         if self.digests is not None:
             for digest in self.digests.values():
                 digest.shift()
 
@@ -569,14 +656,17 @@
             if not pc.is_running():
                 pc.start()
 
     def stop(self):
         if self.__stopped:
             return
 
+        if self._workdir is not None:
+            self._workdir.release()
+
         self.monitor.close()
 
         self.__stopped = True
         _stops = set()
         for listener in self.listeners:
             future = listener.stop()
             if inspect.isawaitable(future):
```

### Comparing `distributed-2023.4.1/distributed/counter.py` & `distributed-2023.5.0/distributed/counter.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/dashboard/components/__init__.py` & `distributed-2023.5.0/distributed/dashboard/components/__init__.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/dashboard/components/nvml.py` & `distributed-2023.5.0/distributed/dashboard/components/nvml.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/dashboard/components/rmm.py` & `distributed-2023.5.0/distributed/dashboard/components/rmm.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/dashboard/components/scheduler.py` & `distributed-2023.5.0/distributed/dashboard/components/scheduler.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/dashboard/components/shared.py` & `distributed-2023.5.0/distributed/dashboard/components/shared.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/dashboard/components/worker.py` & `distributed-2023.5.0/distributed/dashboard/components/worker.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/dashboard/core.py` & `distributed-2023.5.0/distributed/dashboard/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from bokeh.server.util import create_hosts_allowlist
 
 import dask
 
 from distributed.dashboard.utils import BOKEH_VERSION
 from distributed.versions import BOKEH_REQUIREMENT
 
-if BOKEH_VERSION not in BOKEH_REQUIREMENT.specifier:
+# Set `prereleases=True` to allow for use with dev versions of `bokeh`
+if not BOKEH_REQUIREMENT.specifier.contains(BOKEH_VERSION, prereleases=True):
     warnings.warn(
         f"\nDask needs {BOKEH_REQUIREMENT} for the dashboard."
         f"\nYou have bokeh={BOKEH_VERSION}."
         "\nContinuing without the dashboard."
     )
     raise ImportError(
         f"Dask needs {BOKEH_REQUIREMENT} for the dashboard, not bokeh={BOKEH_VERSION}"
```

### Comparing `distributed-2023.4.1/distributed/dashboard/export_tool.js` & `distributed-2023.5.0/distributed/dashboard/export_tool.js`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/dashboard/export_tool.py` & `distributed-2023.5.0/distributed/dashboard/export_tool.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/dashboard/scheduler.py` & `distributed-2023.5.0/distributed/dashboard/scheduler.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/dashboard/utils.py` & `distributed-2023.5.0/distributed/dashboard/utils.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/dashboard/worker.py` & `distributed-2023.5.0/distributed/dashboard/worker.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/deploy/adaptive.py` & `distributed-2023.5.0/distributed/deploy/adaptive.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/deploy/adaptive_core.py` & `distributed-2023.5.0/distributed/deploy/adaptive_core.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/deploy/cluster.py` & `distributed-2023.5.0/distributed/deploy/cluster.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/deploy/local.py` & `distributed-2023.5.0/distributed/deploy/local.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/deploy/old_ssh.py` & `distributed-2023.5.0/distributed/deploy/old_ssh.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/deploy/spec.py` & `distributed-2023.5.0/distributed/deploy/spec.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/deploy/ssh.py` & `distributed-2023.5.0/distributed/deploy/ssh.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/deploy/subprocess.py` & `distributed-2023.5.0/distributed/deploy/subprocess.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/deploy/utils.py` & `distributed-2023.5.0/distributed/deploy/utils.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/diagnostics/cluster_dump.py` & `distributed-2023.5.0/distributed/diagnostics/cluster_dump.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/diagnostics/eventstream.py` & `distributed-2023.5.0/distributed/diagnostics/eventstream.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/diagnostics/graph_layout.py` & `distributed-2023.5.0/distributed/diagnostics/graph_layout.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/diagnostics/memory_sampler.py` & `distributed-2023.5.0/distributed/diagnostics/memory_sampler.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/diagnostics/nvml.py` & `distributed-2023.5.0/distributed/diagnostics/nvml.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/diagnostics/plugin.py` & `distributed-2023.5.0/distributed/diagnostics/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,14 +307,29 @@
     """
     if hasattr(plugin, "name"):
         return plugin.name
     else:
         return funcname(type(plugin)) + "-" + str(uuid.uuid4())
 
 
+class SchedulerUploadFile(SchedulerPlugin):
+    name = "upload_file"
+
+    def __init__(self, filepath):
+        """
+        Initialize the plugin by reading in the data from the given file.
+        """
+        self.filename = os.path.basename(filepath)
+        with open(filepath, "rb") as f:
+            self.data = f.read()
+
+    async def start(self, scheduler: Scheduler) -> None:
+        await scheduler.upload_file(self.filename, self.data)
+
+
 class PackageInstall(WorkerPlugin, abc.ABC):
     """Abstract parent class for a worker plugin to install a set of packages
 
     This accepts a set of packages to install on all workers.
     You can also optionally ask for the worker to restart itself after
     performing this installation.
```

### Comparing `distributed-2023.4.1/distributed/diagnostics/progress.py` & `distributed-2023.5.0/distributed/diagnostics/progress.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/diagnostics/progress_stream.py` & `distributed-2023.5.0/distributed/diagnostics/progress_stream.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/diagnostics/progressbar.py` & `distributed-2023.5.0/distributed/diagnostics/progressbar.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/diagnostics/rmm.py` & `distributed-2023.5.0/distributed/diagnostics/rmm.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/diagnostics/task_stream.py` & `distributed-2023.5.0/distributed/diagnostics/task_stream.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/diagnostics/websocket.py` & `distributed-2023.5.0/distributed/diagnostics/websocket.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/diskutils.py` & `distributed-2023.5.0/distributed/diskutils.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/distributed-schema.yaml` & `distributed-2023.5.0/distributed/distributed-schema.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -592,14 +592,23 @@
                   Limit of number of bytes to be spilled on disk.
 
               monitor-interval:
                 type: string
                 description: >-
                   Interval between checks for the spill, pause, and terminate thresholds
 
+              spill-compression:
+                enum: [null, false, auto, zlib, lz4, snappy, zstd]
+                description:
+                  The compression algorithm to use. 'auto' defaults to lz4 if installed,
+                  otherwise to snappy if installed, otherwise to false. zlib and zstd
+                  are only used if explicitly requested here. Uncompressible data is
+                  always uncompressed, regardless of this setting.
+                  See also distributed.comm.compression.
+
           http:
             type: object
             description: Settings for Dask's embedded HTTP Server
             properties:
               routes:
                 type: array
                 description: |
@@ -768,19 +777,21 @@
                     type: string
                     description: The first non-zero delay between retry attempts
                   max:
                     type: string
                     description: The maximum delay between retries
 
           compression:
-            type: string
-            description: |
-              The compression algorithm to use
-
-              This could be one of lz4, snappy, zstd
+            enum: [null, false, auto, zlib, lz4, snappy, zstd]
+            description:
+              The compression algorithm to use. 'auto' defaults to lz4 if installed,
+              otherwise to snappy if installed, otherwise to false. zlib and zstd are
+              only used if explicitly requested here. Uncompressible data and transfers
+              on localhost are always uncompressed, regardless of this setting.
+              See also distributed.worker.memory.spill-compression.
 
           offload:
             type:
             - boolean
             - string
             description: |
               The size of message after which we choose to offload serialization to another thread
```

### Comparing `distributed-2023.4.1/distributed/distributed.yaml` & `distributed-2023.5.0/distributed/distributed.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,16 @@
       pause: 0.80      # fraction of process memory at which we pause worker threads
       terminate: 0.95  # fraction of process memory at which we terminate the worker
 
       # Max size of the spill file on disk (e.g. "10 GB")
       # Set to false for no maximum.
       max-spill: false
 
+      spill-compression: auto  # See also: distributed.comm.compression
+
       # Interval between checks for the spill, pause, and terminate thresholds.
       # The target threshold is checked every time new data is inserted.
       monitor-interval: 100ms
 
     http:
       routes:
         - distributed.http.worker.prometheus
@@ -213,15 +215,15 @@
 
   comm:
     retry:  # some operations (such as gathering data) are subject to re-tries with the below parameters
       count: 0  # the maximum retry attempts. 0 disables re-trying.
       delay:
          min: 1s  # the first non-zero delay between re-tries
          max: 20s  # the maximum delay between re-tries
-    compression: auto
+    compression: false  # See also: distributed.worker.memory.spill-compression
     shard: 64MiB
     offload: 10MiB # Size after which we choose to offload serialization to another thread
     default-scheme: tcp
     socket-backlog: 2048
     recent-messages-log-length: 0  # number of messages to keep for debugging
     ucx:
       cuda-copy: null  # enable cuda-copy
```

### Comparing `distributed-2023.4.1/distributed/event.py` & `distributed-2023.5.0/distributed/event.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/prometheus.py` & `distributed-2023.5.0/distributed/http/prometheus.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/proxy.py` & `distributed-2023.5.0/distributed/http/proxy.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/routing.py` & `distributed-2023.5.0/distributed/http/routing.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/scheduler/api.py` & `distributed-2023.5.0/distributed/http/scheduler/api.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/scheduler/info.py` & `distributed-2023.5.0/distributed/http/scheduler/info.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/scheduler/json.py` & `distributed-2023.5.0/distributed/http/scheduler/json.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/scheduler/missing_bokeh.py` & `distributed-2023.5.0/distributed/http/scheduler/missing_bokeh.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/scheduler/prometheus/core.py` & `distributed-2023.5.0/distributed/http/scheduler/prometheus/core.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/scheduler/prometheus/semaphore.py` & `distributed-2023.5.0/distributed/http/scheduler/prometheus/semaphore.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/scheduler/prometheus/stealing.py` & `distributed-2023.5.0/distributed/http/scheduler/prometheus/stealing.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/static/css/base.css` & `distributed-2023.5.0/distributed/http/static/css/base.css`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/static/css/individual-cluster-map.css` & `distributed-2023.5.0/distributed/http/static/css/individual-cluster-map.css`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/static/css/status.css` & `distributed-2023.5.0/distributed/http/static/css/status.css`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/static/images/dask-logo.svg` & `distributed-2023.5.0/distributed/http/static/images/dask-logo.svg`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/static/images/fa-bars.svg` & `distributed-2023.5.0/distributed/http/static/images/fa-bars.svg`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/static/images/favicon.ico` & `distributed-2023.5.0/distributed/http/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/static/images/jupyter.svg` & `distributed-2023.5.0/distributed/http/static/images/jupyter.svg`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/static/images/numpy.png` & `distributed-2023.5.0/distributed/http/static/images/numpy.png`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/static/images/pandas.png` & `distributed-2023.5.0/distributed/http/static/images/pandas.png`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/static/images/python.png` & `distributed-2023.5.0/distributed/http/static/images/python.png`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/static/individual-cluster-map.html` & `distributed-2023.5.0/distributed/http/static/individual-cluster-map.html`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/static/js/anime.min.js` & `distributed-2023.5.0/distributed/http/static/js/anime.min.js`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/static/js/individual-cluster-map.js` & `distributed-2023.5.0/distributed/http/static/js/individual-cluster-map.js`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/static/js/reconnecting-websocket.min.js` & `distributed-2023.5.0/distributed/http/static/js/reconnecting-websocket.min.js`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/templates/base.html` & `distributed-2023.5.0/distributed/http/templates/base.html`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/templates/exceptions.html` & `distributed-2023.5.0/distributed/http/templates/exceptions.html`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/templates/status.html` & `distributed-2023.5.0/distributed/http/templates/status.html`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/templates/task.html` & `distributed-2023.5.0/distributed/http/templates/task.html`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/templates/worker-table.html` & `distributed-2023.5.0/distributed/http/templates/worker-table.html`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/templates/worker.html` & `distributed-2023.5.0/distributed/http/templates/worker.html`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/utils.py` & `distributed-2023.5.0/distributed/http/utils.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/http/worker/prometheus/core.py` & `distributed-2023.5.0/distributed/http/worker/prometheus/core.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/lock.py` & `distributed-2023.5.0/distributed/lock.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/metrics.py` & `distributed-2023.5.0/distributed/metrics.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/multi_lock.py` & `distributed-2023.5.0/distributed/multi_lock.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/nanny.py` & `distributed-2023.5.0/distributed/nanny.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import contextlib
 import errno
 import functools
 import logging
 import multiprocessing
 import os
 import shutil
-import tempfile
 import threading
 import uuid
 import warnings
 import weakref
 from collections.abc import Collection
 from inspect import isawaitable
 from queue import Empty
@@ -35,20 +34,20 @@
     ErrorMessage,
     RPCClosed,
     Status,
     coerce_to_address,
     error_message,
 )
 from distributed.diagnostics.plugin import _get_plugin_name
-from distributed.diskutils import WorkSpace
 from distributed.metrics import time
 from distributed.node import ServerNode
 from distributed.process import AsyncProcess
 from distributed.proctitle import enable_proctitle_on_children
 from distributed.protocol import pickle
+from distributed.protocol.serialize import _is_dumpable
 from distributed.security import Security
 from distributed.utils import (
     get_ip,
     get_mp_context,
     json_load_robust,
     log_errors,
     parse_ports,
@@ -171,39 +170,45 @@
 
         if isinstance(security, dict):
             security = Security(**security)
         self.security = security or Security()
         assert isinstance(self.security, Security)
         self.connection_args = self.security.get_connection_args("worker")
 
-        if local_directory is None:
-            local_directory = (
-                dask.config.get("temporary-directory") or tempfile.gettempdir()
-            )
-            self._original_local_dir = local_directory
-            local_directory = os.path.join(local_directory, "dask-worker-space")
-        else:
-            self._original_local_dir = local_directory
-
-        # Create directory if it doesn't exist and test for write access.
-        # In case of PermissionError, change the name.
-        self.local_directory = WorkSpace(local_directory).base_dir
-
         self.preload = preload
         if self.preload is None:
             self.preload = dask.config.get("distributed.worker.preload")
         self.preload_argv = preload_argv
         if self.preload_argv is None:
             self.preload_argv = dask.config.get("distributed.worker.preload-argv")
 
         if preload_nanny is None:
             preload_nanny = dask.config.get("distributed.nanny.preload")
         if preload_nanny_argv is None:
             preload_nanny_argv = dask.config.get("distributed.nanny.preload-argv")
 
+        handlers = {
+            "instantiate": self.instantiate,
+            "kill": self.kill,
+            "restart": self.restart,
+            "get_logs": self.get_logs,
+            # cannot call it 'close' on the rpc side for naming conflict
+            "terminate": self.close,
+            "close_gracefully": self.close_gracefully,
+            "run": self.run,
+            "plugin_add": self.plugin_add,
+            "plugin_remove": self.plugin_remove,
+        }
+        super().__init__(
+            handlers=handlers,
+            connection_args=self.connection_args,
+            local_directory=local_directory,
+            needs_workdir=False,
+        )
+
         self.preloads = preloading.process_preloads(
             self, preload_nanny, preload_nanny_argv, file_dir=self.local_directory
         )
 
         self.death_timeout = parse_timedelta(death_timeout)
         if scheduler_file:
             cfg = json_load_robust(scheduler_file, timeout=self.death_timeout)
@@ -217,15 +222,15 @@
 
         if protocol is None:
             protocol_address = self.scheduler_addr.split("://")
             if len(protocol_address) == 2:
                 protocol = protocol_address[0]
 
         self._given_worker_port = worker_port
-        self.nthreads = nthreads or CPU_COUNT
+        self.nthreads: int = nthreads or CPU_COUNT
         self.reconnect = reconnect
         self.validate = validate
         self.resources = resources
 
         self.Worker = Worker if worker_class is None else worker_class
 
         self.pre_spawn_env = _get_env_variables("distributed.nanny.pre-spawn-environ")
@@ -252,31 +257,15 @@
         self.name = name
         self.quiet = quiet
 
         if silence_logs:
             stack.enter_context(silence_logging_cmgr(level=silence_logs))
         self.silence_logs = silence_logs
 
-        handlers = {
-            "instantiate": self.instantiate,
-            "kill": self.kill,
-            "restart": self.restart,
-            "get_logs": self.get_logs,
-            # cannot call it 'close' on the rpc side for naming conflict
-            "terminate": self.close,
-            "close_gracefully": self.close_gracefully,
-            "run": self.run,
-            "plugin_add": self.plugin_add,
-            "plugin_remove": self.plugin_remove,
-        }
-
         self.plugins: dict[str, NannyPlugin] = {}
-
-        super().__init__(handlers=handlers, connection_args=self.connection_args)
-
         self.scheduler = self.rpc(self.scheduler_addr)
         self.memory_manager = NannyMemoryManager(self, memory_limit=memory_limit)
 
         if (
             not host
             and not interface
             and not self.scheduler_addr.startswith("inproc://")
@@ -618,14 +607,32 @@
     async def _log_event(self, topic, msg):
         await self.scheduler.log_event(
             topic=topic,
             msg=msg,
         )
 
     def log_event(self, topic, msg):
+        """Log an event under a given topic
+
+        Parameters
+        ----------
+        topic : str, list[str]
+            Name of the topic under which to log an event. To log the same
+            event under multiple topics, pass a list of topic names.
+        msg
+            Event message to log. Note this must be msgpack serializable.
+
+        See also
+        --------
+        Client.log_event
+        """
+        if not _is_dumpable(msg):
+            raise TypeError(
+                f"Message must be msgpack serializable. Got {type(msg)=} instead."
+            )
         self._ongoing_background_tasks.call_soon(self._log_event, topic, msg)
 
 
 class WorkerProcess:
     running: asyncio.Event
     stopped: asyncio.Event
```

### Comparing `distributed-2023.4.1/distributed/node.py` & `distributed-2023.5.0/distributed/node.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/objects.py` & `distributed-2023.5.0/distributed/objects.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/preloading.py` & `distributed-2023.5.0/distributed/preloading.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/process.py` & `distributed-2023.5.0/distributed/process.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/proctitle.py` & `distributed-2023.5.0/distributed/proctitle.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/profile.py` & `distributed-2023.5.0/distributed/profile.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/protocol/__init__.py` & `distributed-2023.5.0/distributed/protocol/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 from contextlib import suppress
 from functools import partial
 
-from distributed.protocol.compression import compressions, default_compression
 from distributed.protocol.core import decompress, dumps, loads, maybe_compress, msgpack
 from distributed.protocol.cuda import cuda_deserialize, cuda_serialize
 from distributed.protocol.serialize import (
     Serialize,
     Serialized,
     dask_deserialize,
     dask_serialize,
```

### Comparing `distributed-2023.4.1/distributed/protocol/arrow.py` & `distributed-2023.5.0/distributed/protocol/arrow.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/protocol/compression.py` & `distributed-2023.5.0/distributed/protocol/compression.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,87 +1,88 @@
 """
 Record known compressors
 
 Includes utilities for determining whether or not to compress
 """
 from __future__ import annotations
 
-import logging
-from collections.abc import Callable
+import zlib
+from collections.abc import Callable, Iterable
 from contextlib import suppress
 from functools import partial
 from random import randint
-from typing import Literal
+from typing import TYPE_CHECKING, Any, Literal, NamedTuple
 
 from packaging.version import parse as parse_version
 from tlz import identity
 
 import dask
 
 from distributed.metrics import context_meter
-from distributed.utils import ensure_memoryview, nbytes, no_default
+from distributed.utils import ensure_memoryview, nbytes
 
-compressions: dict[
-    str | None | Literal[False],
-    dict[Literal["compress", "decompress"], Callable[[bytes], bytes]],
-] = {None: {"compress": identity, "decompress": identity}}
+if TYPE_CHECKING:
+    # TODO import from typing (requires Python >=3.10)
+    from typing_extensions import TypeAlias
 
-compressions[False] = compressions[None]  # alias
+# TODO remove quotes (requires Python >=3.10)
+AnyBytes: TypeAlias = "bytes | bytearray | memoryview"
 
 
-default_compression = None
+class Compression(NamedTuple):
+    name: None | str
+    compress: Callable[[AnyBytes], AnyBytes]
+    decompress: Callable[[AnyBytes], AnyBytes]
 
 
-logger = logging.getLogger(__name__)
+compressions: dict[str | None | Literal[False], Compression] = {
+    None: Compression(None, identity, identity),
+    False: Compression(None, identity, identity),  # alias
+    "auto": Compression(None, identity, identity),
+    "zlib": Compression("zlib", zlib.compress, zlib.decompress),
+}
 
 
 with suppress(ImportError):
-    import zlib
-
-    compressions["zlib"] = {"compress": zlib.compress, "decompress": zlib.decompress}
-
-with suppress(ImportError):
     import snappy
 
     # In python-snappy 0.5.3, support for the Python Buffer Protocol was added.
     # This is needed to handle other objects (like `memoryview`s) without
     # copying to `bytes` first.
     #
     # Note: `snappy.__version__` doesn't exist in a release yet.
     #       So do a little test that will fail if snappy is not 0.5.3 or later.
     try:
         snappy.compress(memoryview(b""))
     except TypeError:
         raise ImportError("Need snappy >= 0.5.3")
 
-    compressions["snappy"] = {
-        "compress": snappy.compress,
-        "decompress": snappy.decompress,
-    }
-    default_compression = "snappy"
+    compressions["snappy"] = Compression("snappy", snappy.compress, snappy.decompress)
+    compressions["auto"] = compressions["snappy"]
 
 with suppress(ImportError):
     import lz4
 
     # Required to use `lz4.block` APIs and Python Buffer Protocol support.
     if parse_version(lz4.__version__) < parse_version("0.23.1"):
         raise ImportError("Need lz4 >= 0.23.1")
 
     import lz4.block
 
-    compressions["lz4"] = {
-        "compress": lz4.block.compress,
+    compressions["lz4"] = Compression(
+        "lz4",
+        lz4.block.compress,
         # Avoid expensive deep copies when deserializing writeable numpy arrays
         # See distributed.protocol.numpy.deserialize_numpy_ndarray
         # Note that this is only useful for buffers smaller than distributed.comm.shard;
         # larger ones are deep-copied between decompression and serialization anyway in
         # order to merge them.
-        "decompress": partial(lz4.block.decompress, return_bytearray=True),
-    }
-    default_compression = "lz4"
+        partial(lz4.block.decompress, return_bytearray=True),
+    )
+    compressions["auto"] = compressions["lz4"]
 
 
 with suppress(ImportError):
     import zstandard
 
     # Required for Python Buffer Protocol support.
     if parse_version(zstandard.__version__) < parse_version("0.9.0"):
@@ -94,113 +95,110 @@
         )
         return zstd_compressor.compress(data)
 
     def zstd_decompress(data):
         zstd_decompressor = zstandard.ZstdDecompressor()
         return zstd_decompressor.decompress(data)
 
-    compressions["zstd"] = {"compress": zstd_compress, "decompress": zstd_decompress}
-
-
-def get_default_compression():
-    default = dask.config.get("distributed.comm.compression")
-    if default == "auto":
-        return default_compression
-    if default in compressions:
-        return default
-    raise ValueError(
-        "Default compression '%s' not found.\n"
-        "Choices include auto, %s"
-        % (default, ", ".join(sorted(map(str, compressions))))
-    )
+    compressions["zstd"] = Compression("zstd", zstd_compress, zstd_decompress)
 
 
-get_default_compression()
+def get_compression_settings(key: str) -> str | None:
+    """Fetch and validate compression settings, with a nice error message in case of
+    failure. This also resolves 'auto', which may differ between different hosts of the
+    same cluster.
+    """
+    name = dask.config.get(key)
+    try:
+        return compressions[name].name
+    except KeyError:
+        valid = ",".join(repr(n) for n in compressions)
+        raise ValueError(
+            f"Invalid compression setting {key}={name}. Valid options are {valid}."
+        )
 
 
-def byte_sample(b, size, n):
+def byte_sample(b: memoryview, size: int, n: int) -> memoryview:
     """Sample a bytestring from many locations
 
     Parameters
     ----------
-    b : bytes or memoryview
+    b : full memoryview
     size : int
         target size of each sample to collect
         (may be smaller if samples collide)
     n : int
         number of samples to collect
     """
     assert size >= 0 and n >= 0
     if size == 0 or n == 0:
         return memoryview(b"")
 
-    b = ensure_memoryview(b)
-
-    parts = n * [None]
+    parts = []
     max_start = b.nbytes - size
     start = randint(0, max_start)
-    for i in range(n - 1):
+    for _ in range(n - 1):
         next_start = randint(0, max_start)
         end = min(start + size, next_start)
-        parts[i] = b[start:end]
+        parts.append(b[start:end])
         start = next_start
-    parts[-1] = b[start : start + size]
+    parts.append(b[start : start + size])
 
     if n == 1:
         return parts[0]
     else:
         return memoryview(b"".join(parts))
 
 
 @context_meter.meter("compress")
 def maybe_compress(
-    payload,
-    min_size=10_000,
-    sample_size=10_000,
-    nsamples=5,
-    compression=no_default,
-):
+    payload: bytes | bytearray | memoryview,
+    *,
+    min_size: int = 10_000,
+    sample_size: int = 10_000,
+    nsamples: int = 5,
+    min_ratio: float = 0.7,
+    compression: str | None | Literal[False] = "auto",
+) -> tuple[str | None, AnyBytes]:
+    """Maybe compress payload
+
+    1. Don't compress payload if smaller than min_size
+    2. Sample the payload in <nsamples> spots, compress those, and if it doesn't
+       compress to at least <min_ratio> to the original, return the original
+    3. Then compress the full original; it doesn't compress at least to <min_ratio>,
+       return the original
+    4. Return the compressed output
+
+    Returns
+    -------
+    - Name of compression algorithm used
+    - Either compressed or original payload
     """
-    Maybe compress payload
-
-    1.  We don't compress small messages
-    2.  We sample the payload in a few spots, compress that, and if it doesn't
-        do any good we return the original
-    3.  We then compress the full original, it it doesn't compress well then we
-        return the original
-    4.  We return the compressed result
-    """
-    if compression is no_default:
-        compression = dask.config.get("distributed.comm.compression")
-    if not compression:
+    comp = compressions[compression]
+    if not comp.name:
         return None, payload
     if not (min_size <= nbytes(payload) <= 2**31):
         # Either too small to bother
         # or too large (compression libraries often fail)
         return None, payload
 
-    # Normalize function arguments
-    if compression == "auto":
-        compression = default_compression
-    compress = compressions[compression]["compress"]
-
     # Take a view of payload for efficient usage
     mv = ensure_memoryview(payload)
 
     # Try compressing a sample to see if it compresses well
     sample = byte_sample(mv, sample_size, nsamples)
-    if len(compress(sample)) <= 0.9 * sample.nbytes:
+    if len(comp.compress(sample)) <= min_ratio * sample.nbytes:
         # Try compressing the real thing and check how compressed it is
-        compressed = compress(mv)
-        if len(compressed) <= 0.9 * mv.nbytes:
-            return compression, compressed
+        compressed = comp.compress(mv)
+        if len(compressed) <= min_ratio * mv.nbytes:
+            return comp.name, compressed
     # Skip compression as the sample or the data didn't compress well
     return None, payload
 
 
 @context_meter.meter("decompress")
-def decompress(header, frames):
+def decompress(header: dict[str, Any], frames: Iterable[AnyBytes]) -> list[AnyBytes]:
     """Decompress frames according to information in the header"""
     return [
-        compressions[c]["decompress"](frame)
-        for c, frame in zip(header["compression"], frames)
+        compressions[name].decompress(frame)
+        for name, frame in zip(header["compression"], frames)
     ]
```

### Comparing `distributed-2023.4.1/distributed/protocol/core.py` & `distributed-2023.5.0/distributed/protocol/core.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/protocol/cuda.py` & `distributed-2023.5.0/distributed/protocol/cuda.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/protocol/cupy.py` & `distributed-2023.5.0/distributed/protocol/cupy.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/protocol/h5py.py` & `distributed-2023.5.0/distributed/protocol/h5py.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/protocol/keras.py` & `distributed-2023.5.0/distributed/protocol/keras.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/protocol/netcdf4.py` & `distributed-2023.5.0/distributed/protocol/netcdf4.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/protocol/numba.py` & `distributed-2023.5.0/distributed/protocol/numba.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/protocol/numpy.py` & `distributed-2023.5.0/distributed/protocol/numpy.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/protocol/pickle.py` & `distributed-2023.5.0/distributed/protocol/pickle.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/protocol/rmm.py` & `distributed-2023.5.0/distributed/protocol/rmm.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/protocol/scipy.py` & `distributed-2023.5.0/distributed/protocol/scipy.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/protocol/serialize.py` & `distributed-2023.5.0/distributed/protocol/serialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -655,21 +655,22 @@
 
 @sizeof.register(Pickled)
 @sizeof.register(Serialized)
 def sizeof_serialized(obj):
     return sizeof(obj.header) + sizeof(obj.frames)
 
 
-def serialize_bytelist(x, **kwargs):
+def serialize_bytelist(
+    x: object, compression: str | None | Literal[False] = "auto", **kwargs: Any
+) -> list[bytes | bytearray | memoryview]:
     header, frames = serialize_and_split(x, **kwargs)
     if frames:
-        compression, frames = zip(*map(maybe_compress, frames))
-    else:
-        compression = []
-    header["compression"] = compression
+        header["compression"], frames = zip(
+            *(maybe_compress(frame, compression=compression) for frame in frames)
+        )
     header["count"] = len(frames)
 
     header = msgpack.dumps(header, use_bin_type=True)
     frames2 = [header, *frames]
     frames2.insert(0, pack_frames_prelude(frames2))
     return frames2
 
@@ -844,14 +845,35 @@
         and all(map(_is_msgpack_serializable, v.values()))
         and all(type(x) is str for x in v.keys())
         or isinstance(v, (list, tuple))
         and all(map(_is_msgpack_serializable, v))
     )
 
 
+def _is_dumpable(v):
+    typ = type(v)
+    return (
+        v is None
+        or typ is str
+        or typ is bool
+        or typ is bytes
+        or typ is int
+        or typ is float
+        or typ is Pickled
+        or typ is Serialize
+        or typ is Serialized
+        or typ is ToPickle
+        or isinstance(v, dict)
+        and all(map(_is_dumpable, v.values()))
+        and all(type(x) is str for x in v.keys())
+        or isinstance(v, (list, tuple))
+        and all(map(_is_dumpable, v))
+    )
+
+
 class ObjectDictSerializer:
     def __init__(self, serializer):
         self.serializer = serializer
 
     def serialize(self, est):
         header = {
             "serializer": self.serializer,
```

### Comparing `distributed-2023.4.1/distributed/protocol/sparse.py` & `distributed-2023.5.0/distributed/protocol/sparse.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/protocol/torch.py` & `distributed-2023.5.0/distributed/protocol/torch.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/protocol/utils.py` & `distributed-2023.5.0/distributed/protocol/utils.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/publish.py` & `distributed-2023.5.0/distributed/publish.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/pubsub.py` & `distributed-2023.5.0/distributed/pubsub.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/queues.py` & `distributed-2023.5.0/distributed/queues.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/recreate_tasks.py` & `distributed-2023.5.0/distributed/recreate_tasks.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/scheduler.py` & `distributed-2023.5.0/distributed/scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -17704,1152 +17704,1178 @@
 00045270: 790a 2020 2020 2020 2020 290a 2020 2020  y.        ).    
 00045280: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
 00045290: 7473 0a0a 2020 2020 6465 6620 6c6f 675f  ts..    def log_
 000452a0: 6576 656e 7428 7365 6c66 2c20 746f 7069  event(self, topi
 000452b0: 633a 2073 7472 207c 2043 6f6c 6c65 6374  c: str | Collect
 000452c0: 696f 6e5b 7374 725d 2c20 6d73 673a 2041  ion[str], msg: A
 000452d0: 6e79 2920 2d3e 204e 6f6e 653a 0a20 2020  ny) -> None:.   
-000452e0: 2020 2020 2065 7665 6e74 203d 2028 7469       event = (ti
-000452f0: 6d65 2829 2c20 6d73 6729 0a20 2020 2020  me(), msg).     
-00045300: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
-00045310: 616e 6365 2874 6f70 6963 2c20 7374 7229  ance(topic, str)
-00045320: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-00045330: 7220 7420 696e 2074 6f70 6963 3a0a 2020  r t in topic:.  
-00045340: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00045350: 6c66 2e65 7665 6e74 735b 745d 2e61 7070  lf.events[t].app
-00045360: 656e 6428 6576 656e 7429 0a20 2020 2020  end(event).     
-00045370: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00045380: 6576 656e 745f 636f 756e 7473 5b74 5d20  event_counts[t] 
-00045390: 2b3d 2031 0a20 2020 2020 2020 2020 2020  += 1.           
-000453a0: 2020 2020 2073 656c 662e 5f72 6570 6f72       self._repor
-000453b0: 745f 6576 656e 7428 742c 2065 7665 6e74  t_event(t, event
-000453c0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-000453d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000453e0: 2e65 7665 6e74 735b 746f 7069 635d 2e61  .events[topic].a
-000453f0: 7070 656e 6428 6576 656e 7429 0a20 2020  ppend(event).   
-00045400: 2020 2020 2020 2020 2073 656c 662e 6576           self.ev
-00045410: 656e 745f 636f 756e 7473 5b74 6f70 6963  ent_counts[topic
-00045420: 5d20 2b3d 2031 0a20 2020 2020 2020 2020  ] += 1.         
-00045430: 2020 2073 656c 662e 5f72 6570 6f72 745f     self._report_
-00045440: 6576 656e 7428 746f 7069 632c 2065 7665  event(topic, eve
-00045450: 6e74 290a 0a20 2020 2020 2020 2020 2020  nt)..           
-00045460: 2066 6f72 2070 6c75 6769 6e20 696e 206c   for plugin in l
-00045470: 6973 7428 7365 6c66 2e70 6c75 6769 6e73  ist(self.plugins
-00045480: 2e76 616c 7565 7328 2929 3a0a 2020 2020  .values()):.    
-00045490: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-000454a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000454b0: 2020 2020 2070 6c75 6769 6e2e 6c6f 675f       plugin.log_
-000454c0: 6576 656e 7428 746f 7069 632c 206d 7367  event(topic, msg
-000454d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000454e0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-000454f0: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
-00045500: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
-00045510: 6e66 6f28 2250 6c75 6769 6e20 6661 696c  nfo("Plugin fail
-00045520: 6564 2077 6974 6820 6578 6365 7074 696f  ed with exceptio
-00045530: 6e22 2c20 6578 635f 696e 666f 3d54 7275  n", exc_info=Tru
-00045540: 6529 0a0a 2020 2020 6465 6620 5f72 6570  e)..    def _rep
-00045550: 6f72 745f 6576 656e 7428 7365 6c66 2c20  ort_event(self, 
-00045560: 6e61 6d65 2c20 6576 656e 7429 3a0a 2020  name, event):.  
-00045570: 2020 2020 2020 6d73 6720 3d20 7b0a 2020        msg = {.  
-00045580: 2020 2020 2020 2020 2020 226f 7022 3a20            "op": 
-00045590: 2265 7665 6e74 222c 0a20 2020 2020 2020  "event",.       
-000455a0: 2020 2020 2022 746f 7069 6322 3a20 6e61       "topic": na
-000455b0: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-000455c0: 2265 7665 6e74 223a 2065 7665 6e74 2c0a  "event": event,.
-000455d0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-000455e0: 2020 636c 6965 6e74 5f6d 7367 7320 3d20    client_msgs = 
-000455f0: 7b63 6c69 656e 743a 205b 6d73 675d 2066  {client: [msg] f
-00045600: 6f72 2063 6c69 656e 7420 696e 2073 656c  or client in sel
-00045610: 662e 6576 656e 745f 7375 6273 6372 6962  f.event_subscrib
-00045620: 6572 5b6e 616d 655d 7d0a 2020 2020 2020  er[name]}.      
-00045630: 2020 7365 6c66 2e73 656e 645f 616c 6c28    self.send_all(
-00045640: 636c 6965 6e74 5f6d 7367 732c 2077 6f72  client_msgs, wor
-00045650: 6b65 725f 6d73 6773 3d7b 7d29 0a0a 2020  ker_msgs={})..  
-00045660: 2020 6465 6620 7375 6273 6372 6962 655f    def subscribe_
-00045670: 746f 7069 6328 7365 6c66 2c20 746f 7069  topic(self, topi
-00045680: 632c 2063 6c69 656e 7429 3a0a 2020 2020  c, client):.    
-00045690: 2020 2020 7365 6c66 2e65 7665 6e74 5f73      self.event_s
-000456a0: 7562 7363 7269 6265 725b 746f 7069 635d  ubscriber[topic]
-000456b0: 2e61 6464 2863 6c69 656e 7429 0a0a 2020  .add(client)..  
-000456c0: 2020 6465 6620 756e 7375 6273 6372 6962    def unsubscrib
-000456d0: 655f 746f 7069 6328 7365 6c66 2c20 746f  e_topic(self, to
-000456e0: 7069 632c 2063 6c69 656e 7429 3a0a 2020  pic, client):.  
-000456f0: 2020 2020 2020 7365 6c66 2e65 7665 6e74        self.event
-00045700: 5f73 7562 7363 7269 6265 725b 746f 7069  _subscriber[topi
-00045710: 635d 2e64 6973 6361 7264 2863 6c69 656e  c].discard(clien
-00045720: 7429 0a0a 2020 2020 6465 6620 6765 745f  t)..    def get_
-00045730: 6576 656e 7473 2873 656c 662c 2074 6f70  events(self, top
-00045740: 6963 3d4e 6f6e 6529 3a0a 2020 2020 2020  ic=None):.      
-00045750: 2020 6966 2074 6f70 6963 2069 7320 6e6f    if topic is no
-00045760: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00045770: 2020 2020 7265 7475 726e 2074 7570 6c65      return tuple
-00045780: 2873 656c 662e 6576 656e 7473 5b74 6f70  (self.events[top
-00045790: 6963 5d29 0a20 2020 2020 2020 2065 6c73  ic]).        els
-000457a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000457b0: 6574 7572 6e20 7661 6c6d 6170 2874 7570  eturn valmap(tup
-000457c0: 6c65 2c20 7365 6c66 2e65 7665 6e74 7329  le, self.events)
-000457d0: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-000457e0: 6765 745f 776f 726b 6572 5f6d 6f6e 6974  get_worker_monit
-000457f0: 6f72 5f69 6e66 6f28 7365 6c66 2c20 7265  or_info(self, re
-00045800: 6365 6e74 3d46 616c 7365 2c20 7374 6172  cent=False, star
-00045810: 7473 3d4e 6f6e 6529 3a0a 2020 2020 2020  ts=None):.      
-00045820: 2020 6966 2073 7461 7274 7320 6973 204e    if starts is N
-00045830: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00045840: 2073 7461 7274 7320 3d20 7b7d 0a20 2020   starts = {}.   
-00045850: 2020 2020 2072 6573 756c 7473 203d 2061       results = a
-00045860: 7761 6974 2061 7379 6e63 696f 2e67 6174  wait asyncio.gat
-00045870: 6865 7228 0a20 2020 2020 2020 2020 2020  her(.           
-00045880: 202a 280a 2020 2020 2020 2020 2020 2020   *(.            
-00045890: 2020 2020 7365 6c66 2e72 7063 2877 292e      self.rpc(w).
-000458a0: 6765 745f 6d6f 6e69 746f 725f 696e 666f  get_monitor_info
-000458b0: 2872 6563 656e 743d 7265 6365 6e74 2c20  (recent=recent, 
-000458c0: 7374 6172 743d 7374 6172 7473 2e67 6574  start=starts.get
-000458d0: 2877 2c20 3029 290a 2020 2020 2020 2020  (w, 0)).        
-000458e0: 2020 2020 2020 2020 666f 7220 7720 696e          for w in
-000458f0: 2073 656c 662e 776f 726b 6572 730a 2020   self.workers.  
-00045900: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00045910: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
-00045920: 7475 726e 2064 6963 7428 7a69 7028 7365  turn dict(zip(se
-00045930: 6c66 2e77 6f72 6b65 7273 2c20 7265 7375  lf.workers, resu
-00045940: 6c74 7329 290a 0a20 2020 2023 2323 2323  lts))..    #####
-00045950: 2323 2323 2323 0a20 2020 2023 2043 6c65  ######.    # Cle
-00045960: 616e 7570 2023 0a20 2020 2023 2323 2323  anup #.    #####
-00045970: 2323 2323 2323 0a0a 2020 2020 6173 796e  ######..    asyn
-00045980: 6320 6465 6620 6368 6563 6b5f 776f 726b  c def check_work
-00045990: 6572 5f74 746c 2873 656c 6629 3a0a 2020  er_ttl(self):.  
-000459a0: 2020 2020 2020 6e6f 7720 3d20 7469 6d65        now = time
-000459b0: 2829 0a20 2020 2020 2020 2073 7469 6d75  ().        stimu
-000459c0: 6c75 735f 6964 203d 2066 2263 6865 636b  lus_id = f"check
-000459d0: 2d77 6f72 6b65 722d 7474 6c2d 7b6e 6f77  -worker-ttl-{now
-000459e0: 7d22 0a20 2020 2020 2020 2066 6f72 2077  }".        for w
-000459f0: 7320 696e 2073 656c 662e 776f 726b 6572  s in self.worker
-00045a00: 732e 7661 6c75 6573 2829 3a0a 2020 2020  s.values():.    
-00045a10: 2020 2020 2020 2020 6966 2028 7773 2e6c          if (ws.l
-00045a20: 6173 745f 7365 656e 203c 206e 6f77 202d  ast_seen < now -
-00045a30: 2073 656c 662e 776f 726b 6572 5f74 746c   self.worker_ttl
-00045a40: 2920 616e 6420 280a 2020 2020 2020 2020  ) and (.        
-00045a50: 2020 2020 2020 2020 7773 2e6c 6173 745f          ws.last_
-00045a60: 7365 656e 203c 206e 6f77 202d 2031 3020  seen < now - 10 
-00045a70: 2a20 6865 6172 7462 6561 745f 696e 7465  * heartbeat_inte
-00045a80: 7276 616c 286c 656e 2873 656c 662e 776f  rval(len(self.wo
-00045a90: 726b 6572 7329 290a 2020 2020 2020 2020  rkers)).        
-00045aa0: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
-00045ab0: 2020 2020 2020 206c 6f67 6765 722e 7761         logger.wa
-00045ac0: 726e 696e 6728 0a20 2020 2020 2020 2020  rning(.         
-00045ad0: 2020 2020 2020 2020 2020 2022 576f 726b             "Work
-00045ae0: 6572 2066 6169 6c65 6420 746f 2068 6561  er failed to hea
-00045af0: 7274 6265 6174 2077 6974 6869 6e20 2573  rtbeat within %s
-00045b00: 2073 6563 6f6e 6473 2e20 436c 6f73 696e   seconds. Closin
-00045b10: 673a 2025 7322 2c0a 2020 2020 2020 2020  g: %s",.        
-00045b20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00045b30: 2e77 6f72 6b65 725f 7474 6c2c 0a20 2020  .worker_ttl,.   
-00045b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00045b50: 2077 732c 0a20 2020 2020 2020 2020 2020   ws,.           
-00045b60: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00045b70: 2020 2020 2020 2061 7761 6974 2073 656c         await sel
-00045b80: 662e 7265 6d6f 7665 5f77 6f72 6b65 7228  f.remove_worker(
-00045b90: 6164 6472 6573 733d 7773 2e61 6464 7265  address=ws.addre
-00045ba0: 7373 2c20 7374 696d 756c 7573 5f69 643d  ss, stimulus_id=
-00045bb0: 7374 696d 756c 7573 5f69 6429 0a0a 2020  stimulus_id)..  
-00045bc0: 2020 6465 6620 6368 6563 6b5f 6964 6c65    def check_idle
-00045bd0: 2873 656c 6629 202d 3e20 666c 6f61 7420  (self) -> float 
-00045be0: 7c20 4e6f 6e65 3a0a 2020 2020 2020 2020  | None:.        
-00045bf0: 6966 2073 656c 662e 7374 6174 7573 2069  if self.status i
-00045c00: 6e20 2853 7461 7475 732e 636c 6f73 696e  n (Status.closin
-00045c10: 672c 2053 7461 7475 732e 636c 6f73 6564  g, Status.closed
-00045c20: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-00045c30: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
-00045c40: 2020 2020 6966 2073 656c 662e 7472 616e      if self.tran
-00045c50: 7369 7469 6f6e 5f63 6f75 6e74 6572 2021  sition_counter !
-00045c60: 3d20 7365 6c66 2e5f 6964 6c65 5f74 7261  = self._idle_tra
-00045c70: 6e73 6974 696f 6e5f 636f 756e 7465 723a  nsition_counter:
-00045c80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00045c90: 662e 5f69 646c 655f 7472 616e 7369 7469  f._idle_transiti
-00045ca0: 6f6e 5f63 6f75 6e74 6572 203d 2073 656c  on_counter = sel
-00045cb0: 662e 7472 616e 7369 7469 6f6e 5f63 6f75  f.transition_cou
-00045cc0: 6e74 6572 0a20 2020 2020 2020 2020 2020  nter.           
-00045cd0: 2073 656c 662e 6964 6c65 5f73 696e 6365   self.idle_since
-00045ce0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-00045cf0: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-00045d00: 0a20 2020 2020 2020 2069 6620 280a 2020  .        if (.  
-00045d10: 2020 2020 2020 2020 2020 7365 6c66 2e71            self.q
-00045d20: 7565 7565 640a 2020 2020 2020 2020 2020  ueued.          
-00045d30: 2020 6f72 2073 656c 662e 756e 7275 6e6e    or self.unrunn
-00045d40: 6162 6c65 0a20 2020 2020 2020 2020 2020  able.           
-00045d50: 206f 7220 616e 7928 7773 2e70 726f 6365   or any(ws.proce
-00045d60: 7373 696e 6720 666f 7220 7773 2069 6e20  ssing for ws in 
-00045d70: 7365 6c66 2e77 6f72 6b65 7273 2e76 616c  self.workers.val
-00045d80: 7565 7328 2929 0a20 2020 2020 2020 2029  ues()).        )
-00045d90: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00045da0: 6c66 2e69 646c 655f 7369 6e63 6520 3d20  lf.idle_since = 
-00045db0: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-00045dc0: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
-00045dd0: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-00045de0: 662e 6964 6c65 5f73 696e 6365 3a0a 2020  f.idle_since:.  
-00045df0: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
-00045e00: 646c 655f 7369 6e63 6520 3d20 7469 6d65  dle_since = time
-00045e10: 2829 0a20 2020 2020 2020 2020 2020 2072  ().            r
-00045e20: 6574 7572 6e20 7365 6c66 2e69 646c 655f  eturn self.idle_
-00045e30: 7369 6e63 650a 0a20 2020 2020 2020 2069  since..        i
-00045e40: 6620 7365 6c66 2e6a 7570 7974 6572 3a0a  f self.jupyter:.
-00045e50: 2020 2020 2020 2020 2020 2020 6c61 7374              last
-00045e60: 5f61 6374 6976 6974 7920 3d20 280a 2020  _activity = (.  
-00045e70: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00045e80: 6c66 2e5f 6a75 7079 7465 725f 7365 7276  lf._jupyter_serv
-00045e90: 6572 5f61 7070 6c69 6361 7469 6f6e 2e77  er_application.w
-00045ea0: 6562 5f61 7070 2e6c 6173 745f 6163 7469  eb_app.last_acti
-00045eb0: 7669 7479 2829 2e74 696d 6573 7461 6d70  vity().timestamp
-00045ec0: 2829 0a20 2020 2020 2020 2020 2020 2029  ().            )
-00045ed0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00045ee0: 6c61 7374 5f61 6374 6976 6974 7920 3e20  last_activity > 
-00045ef0: 7365 6c66 2e69 646c 655f 7369 6e63 653a  self.idle_since:
-00045f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00045f10: 2073 656c 662e 6964 6c65 5f73 696e 6365   self.idle_since
-00045f20: 203d 206c 6173 745f 6163 7469 7669 7479   = last_activity
-00045f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00045f40: 2072 6574 7572 6e20 7365 6c66 2e69 646c   return self.idl
-00045f50: 655f 7369 6e63 650a 0a20 2020 2020 2020  e_since..       
-00045f60: 2069 6620 7365 6c66 2e69 646c 655f 7469   if self.idle_ti
-00045f70: 6d65 6f75 743a 0a20 2020 2020 2020 2020  meout:.         
-00045f80: 2020 2069 6620 7469 6d65 2829 203e 2073     if time() > s
-00045f90: 656c 662e 6964 6c65 5f73 696e 6365 202b  elf.idle_since +
-00045fa0: 2073 656c 662e 6964 6c65 5f74 696d 656f   self.idle_timeo
-00045fb0: 7574 3a0a 2020 2020 2020 2020 2020 2020  ut:.            
-00045fc0: 2020 2020 6173 7365 7274 2073 656c 662e      assert self.
-00045fd0: 6964 6c65 5f73 696e 6365 0a20 2020 2020  idle_since.     
-00045fe0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00045ff0: 722e 696e 666f 280a 2020 2020 2020 2020  r.info(.        
-00046000: 2020 2020 2020 2020 2020 2020 2253 6368              "Sch
-00046010: 6564 756c 6572 2063 6c6f 7369 6e67 2061  eduler closing a
-00046020: 6674 6572 2062 6569 6e67 2069 646c 6520  fter being idle 
-00046030: 666f 7220 2573 222c 0a20 2020 2020 2020  for %s",.       
-00046040: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00046050: 6d61 745f 7469 6d65 2873 656c 662e 6964  mat_time(self.id
-00046060: 6c65 5f74 696d 656f 7574 292c 0a20 2020  le_timeout),.   
-00046070: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00046080: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00046090: 656c 662e 5f6f 6e67 6f69 6e67 5f62 6163  elf._ongoing_bac
-000460a0: 6b67 726f 756e 645f 7461 736b 732e 6361  kground_tasks.ca
-000460b0: 6c6c 5f73 6f6f 6e28 7365 6c66 2e63 6c6f  ll_soon(self.clo
-000460c0: 7365 290a 2020 2020 2020 2020 7265 7475  se).        retu
-000460d0: 726e 2073 656c 662e 6964 6c65 5f73 696e  rn self.idle_sin
-000460e0: 6365 0a0a 2020 2020 6465 6620 6164 6170  ce..    def adap
-000460f0: 7469 7665 5f74 6172 6765 7428 7365 6c66  tive_target(self
-00046100: 2c20 7461 7267 6574 5f64 7572 6174 696f  , target_duratio
-00046110: 6e3d 4e6f 6e65 293a 0a20 2020 2020 2020  n=None):.       
-00046120: 2022 2222 4465 7369 7265 6420 6e75 6d62   """Desired numb
-00046130: 6572 206f 6620 776f 726b 6572 7320 6261  er of workers ba
-00046140: 7365 6420 6f6e 2074 6865 2063 7572 7265  sed on the curre
-00046150: 6e74 2077 6f72 6b6c 6f61 640a 0a20 2020  nt workload..   
-00046160: 2020 2020 2054 6869 7320 6c6f 6f6b 7320       This looks 
-00046170: 6174 2074 6865 2063 7572 7265 6e74 2072  at the current r
-00046180: 756e 6e69 6e67 2074 6173 6b73 2061 6e64  unning tasks and
-00046190: 206d 656d 6f72 7920 7573 652c 2061 6e64   memory use, and
-000461a0: 2072 6574 7572 6e73 2061 0a20 2020 2020   returns a.     
-000461b0: 2020 206e 756d 6265 7220 6f66 2064 6573     number of des
-000461c0: 6972 6564 2077 6f72 6b65 7273 2e20 2054  ired workers.  T
-000461d0: 6869 7320 6973 206f 6674 656e 2075 7365  his is often use
-000461e0: 6420 6279 2061 6461 7074 6976 6520 7363  d by adaptive sc
-000461f0: 6865 6475 6c69 6e67 2e0a 0a20 2020 2020  heduling...     
-00046200: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-00046210: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-00046220: 0a20 2020 2020 2020 2074 6172 6765 745f  .        target_
-00046230: 6475 7261 7469 6f6e 203a 2073 7472 0a20  duration : str. 
-00046240: 2020 2020 2020 2020 2020 2041 2064 6573             A des
-00046250: 6972 6564 2064 7572 6174 696f 6e20 6f66  ired duration of
-00046260: 2074 696d 6520 666f 7220 636f 6d70 7574   time for comput
-00046270: 6174 696f 6e73 2074 6f20 7461 6b65 2e20  ations to take. 
-00046280: 2054 6869 7320 6166 6665 6374 730a 2020   This affects.  
-00046290: 2020 2020 2020 2020 2020 686f 7720 7261            how ra
-000462a0: 7069 646c 7920 7468 6520 7363 6865 6475  pidly the schedu
-000462b0: 6c65 7220 7769 6c6c 2061 736b 2074 6f20  ler will ask to 
-000462c0: 7363 616c 652e 0a0a 2020 2020 2020 2020  scale...        
-000462d0: 5365 6520 416c 736f 0a20 2020 2020 2020  See Also.       
-000462e0: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020   --------.      
-000462f0: 2020 6469 7374 7269 6275 7465 642e 6465    distributed.de
-00046300: 706c 6f79 2e41 6461 7074 6976 650a 2020  ploy.Adaptive.  
-00046310: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00046320: 2020 6966 2074 6172 6765 745f 6475 7261    if target_dura
-00046330: 7469 6f6e 2069 7320 4e6f 6e65 3a0a 2020  tion is None:.  
-00046340: 2020 2020 2020 2020 2020 7461 7267 6574            target
-00046350: 5f64 7572 6174 696f 6e20 3d20 6461 736b  _duration = dask
-00046360: 2e63 6f6e 6669 672e 6765 7428 2264 6973  .config.get("dis
-00046370: 7472 6962 7574 6564 2e61 6461 7074 6976  tributed.adaptiv
-00046380: 652e 7461 7267 6574 2d64 7572 6174 696f  e.target-duratio
-00046390: 6e22 290a 2020 2020 2020 2020 7461 7267  n").        targ
-000463a0: 6574 5f64 7572 6174 696f 6e20 3d20 7061  et_duration = pa
-000463b0: 7273 655f 7469 6d65 6465 6c74 6128 7461  rse_timedelta(ta
-000463c0: 7267 6574 5f64 7572 6174 696f 6e29 0a0a  rget_duration)..
-000463d0: 2020 2020 2020 2020 2320 4350 550a 0a20          # CPU.. 
-000463e0: 2020 2020 2020 2023 2054 4f44 4f20 636f         # TODO co
-000463f0: 6e73 6964 6572 2061 6e79 2075 7365 722d  nsider any user-
-00046400: 7370 6563 6966 6965 6420 6465 6661 756c  specified defaul
-00046410: 7420 7461 736b 2064 7572 6174 696f 6e73  t task durations
-00046420: 2066 6f72 2071 7565 7565 6420 7461 736b   for queued task
-00046430: 730a 2020 2020 2020 2020 7175 6575 6564  s.        queued
-00046440: 5f6f 6363 7570 616e 6379 203d 206c 656e  _occupancy = len
-00046450: 2873 656c 662e 7175 6575 6564 2920 2a20  (self.queued) * 
-00046460: 7365 6c66 2e55 4e4b 4e4f 574e 5f54 4153  self.UNKNOWN_TAS
-00046470: 4b5f 4455 5241 5449 4f4e 0a20 2020 2020  K_DURATION.     
-00046480: 2020 2063 7075 203d 206d 6174 682e 6365     cpu = math.ce
-00046490: 696c 280a 2020 2020 2020 2020 2020 2020  il(.            
-000464a0: 2873 656c 662e 746f 7461 6c5f 6f63 6375  (self.total_occu
-000464b0: 7061 6e63 7920 2b20 7175 6575 6564 5f6f  pancy + queued_o
-000464c0: 6363 7570 616e 6379 2920 2f20 7461 7267  ccupancy) / targ
-000464d0: 6574 5f64 7572 6174 696f 6e0a 2020 2020  et_duration.    
-000464e0: 2020 2020 2920 2023 2054 4f44 4f3a 2074      )  # TODO: t
-000464f0: 6872 6561 6473 2070 6572 2077 6f72 6b65  hreads per worke
-00046500: 720a 0a20 2020 2020 2020 2023 2041 766f  r..        # Avo
-00046510: 6964 2061 2066 6577 206c 6f6e 6720 7461  id a few long ta
-00046520: 736b 7320 6672 6f6d 2061 736b 696e 6720  sks from asking 
-00046530: 666f 7220 6d61 6e79 2063 6f72 6573 0a20  for many cores. 
-00046540: 2020 2020 2020 2074 6173 6b73 5f72 6561         tasks_rea
-00046550: 6479 203d 206c 656e 2873 656c 662e 7175  dy = len(self.qu
-00046560: 6575 6564 290a 2020 2020 2020 2020 666f  eued).        fo
-00046570: 7220 7773 2069 6e20 7365 6c66 2e77 6f72  r ws in self.wor
-00046580: 6b65 7273 2e76 616c 7565 7328 293a 0a20  kers.values():. 
-00046590: 2020 2020 2020 2020 2020 2074 6173 6b73             tasks
-000465a0: 5f72 6561 6479 202b 3d20 6c65 6e28 7773  _ready += len(ws
-000465b0: 2e70 726f 6365 7373 696e 6729 0a0a 2020  .processing)..  
-000465c0: 2020 2020 2020 2020 2020 6966 2074 6173            if tas
-000465d0: 6b73 5f72 6561 6479 203e 2063 7075 3a0a  ks_ready > cpu:.
-000465e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000465f0: 6272 6561 6b0a 2020 2020 2020 2020 656c  break.        el
-00046600: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00046610: 6370 7520 3d20 6d69 6e28 7461 736b 735f  cpu = min(tasks_
-00046620: 7265 6164 792c 2063 7075 290a 0a20 2020  ready, cpu)..   
-00046630: 2020 2020 2069 6620 2873 656c 662e 756e       if (self.un
-00046640: 7275 6e6e 6162 6c65 206f 7220 7365 6c66  runnable or self
-00046650: 2e71 7565 7565 6429 2061 6e64 206e 6f74  .queued) and not
-00046660: 2073 656c 662e 776f 726b 6572 733a 0a20   self.workers:. 
-00046670: 2020 2020 2020 2020 2020 2063 7075 203d             cpu =
-00046680: 206d 6178 2831 2c20 6370 7529 0a0a 2020   max(1, cpu)..  
-00046690: 2020 2020 2020 2320 6164 6420 6d6f 7265        # add more
-000466a0: 2077 6f72 6b65 7273 2069 6620 6d6f 7265   workers if more
-000466b0: 2074 6861 6e20 3630 2520 6f66 206d 656d   than 60% of mem
-000466c0: 6f72 7920 6973 2075 7365 640a 2020 2020  ory is used.    
-000466d0: 2020 2020 6c69 6d69 7420 3d20 7375 6d28      limit = sum(
-000466e0: 7773 2e6d 656d 6f72 795f 6c69 6d69 7420  ws.memory_limit 
-000466f0: 666f 7220 7773 2069 6e20 7365 6c66 2e77  for ws in self.w
-00046700: 6f72 6b65 7273 2e76 616c 7565 7328 2929  orkers.values())
-00046710: 0a20 2020 2020 2020 2075 7365 6420 3d20  .        used = 
-00046720: 7375 6d28 7773 2e6e 6279 7465 7320 666f  sum(ws.nbytes fo
-00046730: 7220 7773 2069 6e20 7365 6c66 2e77 6f72  r ws in self.wor
-00046740: 6b65 7273 2e76 616c 7565 7328 2929 0a20  kers.values()). 
-00046750: 2020 2020 2020 206d 656d 6f72 7920 3d20         memory = 
-00046760: 300a 2020 2020 2020 2020 6966 2075 7365  0.        if use
-00046770: 6420 3e20 302e 3620 2a20 6c69 6d69 7420  d > 0.6 * limit 
-00046780: 616e 6420 6c69 6d69 7420 3e20 303a 0a20  and limit > 0:. 
-00046790: 2020 2020 2020 2020 2020 206d 656d 6f72             memor
-000467a0: 7920 3d20 3220 2a20 6c65 6e28 7365 6c66  y = 2 * len(self
-000467b0: 2e77 6f72 6b65 7273 290a 0a20 2020 2020  .workers)..     
-000467c0: 2020 2074 6172 6765 7420 3d20 6d61 7828     target = max(
-000467d0: 6d65 6d6f 7279 2c20 6370 7529 0a20 2020  memory, cpu).   
-000467e0: 2020 2020 2069 6620 7461 7267 6574 203e       if target >
-000467f0: 3d20 6c65 6e28 7365 6c66 2e77 6f72 6b65  = len(self.worke
-00046800: 7273 293a 0a20 2020 2020 2020 2020 2020  rs):.           
-00046810: 2072 6574 7572 6e20 7461 7267 6574 0a20   return target. 
-00046820: 2020 2020 2020 2065 6c73 653a 2020 2320         else:  # 
-00046830: 5363 616c 6520 646f 776e 3f0a 2020 2020  Scale down?.    
-00046840: 2020 2020 2020 2020 746f 5f63 6c6f 7365          to_close
-00046850: 203d 2073 656c 662e 776f 726b 6572 735f   = self.workers_
-00046860: 746f 5f63 6c6f 7365 2829 0a20 2020 2020  to_close().     
-00046870: 2020 2020 2020 2072 6574 7572 6e20 6c65         return le
-00046880: 6e28 7365 6c66 2e77 6f72 6b65 7273 2920  n(self.workers) 
-00046890: 2d20 6c65 6e28 746f 5f63 6c6f 7365 290a  - len(to_close).
-000468a0: 0a20 2020 2064 6566 2072 6571 7565 7374  .    def request
-000468b0: 5f61 6371 7569 7265 5f72 6570 6c69 6361  _acquire_replica
-000468c0: 7328 0a20 2020 2020 2020 2073 656c 662c  s(.        self,
-000468d0: 2061 6464 723a 2073 7472 2c20 6b65 7973   addr: str, keys
-000468e0: 3a20 4974 6572 6162 6c65 5b73 7472 5d2c  : Iterable[str],
-000468f0: 202a 2c20 7374 696d 756c 7573 5f69 643a   *, stimulus_id:
-00046900: 2073 7472 0a20 2020 2029 202d 3e20 4e6f   str.    ) -> No
-00046910: 6e65 3a0a 2020 2020 2020 2020 2222 2241  ne:.        """A
-00046920: 7379 6e63 6872 6f6e 6f75 736c 7920 6173  synchronously as
-00046930: 6b20 6120 776f 726b 6572 2074 6f20 6163  k a worker to ac
-00046940: 7175 6972 6520 6120 7265 706c 6963 6120  quire a replica 
-00046950: 6f66 2074 6865 206c 6973 7465 6420 6b65  of the listed ke
-00046960: 7973 2066 726f 6d0a 2020 2020 2020 2020  ys from.        
-00046970: 6f74 6865 7220 776f 726b 6572 732e 2054  other workers. T
-00046980: 6869 7320 6973 2061 2066 6972 652d 616e  his is a fire-an
-00046990: 642d 666f 7267 6574 206f 7065 7261 7469  d-forget operati
-000469a0: 6f6e 2077 6869 6368 206f 6666 6572 7320  on which offers 
-000469b0: 6e6f 2066 6565 6462 6163 6b20 666f 720a  no feedback for.
-000469c0: 2020 2020 2020 2020 7375 6363 6573 7320          success 
-000469d0: 6f72 2066 6169 6c75 7265 2c20 616e 6420  or failure, and 
-000469e0: 6973 2069 6e74 656e 6465 6420 666f 7220  is intended for 
-000469f0: 686f 7573 656b 6565 7069 6e67 2061 6e64  housekeeping and
-00046a00: 206e 6f74 2066 6f72 2063 6f6d 7075 7461   not for computa
-00046a10: 7469 6f6e 2e0a 2020 2020 2020 2020 2222  tion..        ""
-00046a20: 220a 2020 2020 2020 2020 7768 6f5f 6861  ".        who_ha
-00046a30: 7320 3d20 7b7d 0a20 2020 2020 2020 206e  s = {}.        n
-00046a40: 6279 7465 7320 3d20 7b7d 0a20 2020 2020  bytes = {}.     
-00046a50: 2020 2066 6f72 206b 6579 2069 6e20 6b65     for key in ke
-00046a60: 7973 3a0a 2020 2020 2020 2020 2020 2020  ys:.            
-00046a70: 7473 203d 2073 656c 662e 7461 736b 735b  ts = self.tasks[
-00046a80: 6b65 795d 0a20 2020 2020 2020 2020 2020  key].           
-00046a90: 2061 7373 6572 7420 7473 2e77 686f 5f68   assert ts.who_h
-00046aa0: 6173 0a20 2020 2020 2020 2020 2020 2077  as.            w
-00046ab0: 686f 5f68 6173 5b6b 6579 5d20 3d20 5b77  ho_has[key] = [w
-00046ac0: 732e 6164 6472 6573 7320 666f 7220 7773  s.address for ws
-00046ad0: 2069 6e20 7473 2e77 686f 5f68 6173 5d0a   in ts.who_has].
-00046ae0: 2020 2020 2020 2020 2020 2020 6e62 7974              nbyt
-00046af0: 6573 5b6b 6579 5d20 3d20 7473 2e6e 6279  es[key] = ts.nby
-00046b00: 7465 730a 0a20 2020 2020 2020 2073 656c  tes..        sel
-00046b10: 662e 7374 7265 616d 5f63 6f6d 6d73 5b61  f.stream_comms[a
-00046b20: 6464 725d 2e73 656e 6428 0a20 2020 2020  ddr].send(.     
-00046b30: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-00046b40: 2020 2020 2020 2020 2022 6f70 223a 2022           "op": "
-00046b50: 6163 7175 6972 652d 7265 706c 6963 6173  acquire-replicas
-00046b60: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00046b70: 2020 2022 7768 6f5f 6861 7322 3a20 7768     "who_has": wh
-00046b80: 6f5f 6861 732c 0a20 2020 2020 2020 2020  o_has,.         
-00046b90: 2020 2020 2020 2022 6e62 7974 6573 223a         "nbytes":
-00046ba0: 206e 6279 7465 732c 0a20 2020 2020 2020   nbytes,.       
-00046bb0: 2020 2020 2020 2020 2022 7374 696d 756c           "stimul
-00046bc0: 7573 5f69 6422 3a20 7374 696d 756c 7573  us_id": stimulus
-00046bd0: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
-00046be0: 207d 2c0a 2020 2020 2020 2020 290a 0a20   },.        ).. 
-00046bf0: 2020 2064 6566 2072 6571 7565 7374 5f72     def request_r
-00046c00: 656d 6f76 655f 7265 706c 6963 6173 280a  emove_replicas(.
-00046c10: 2020 2020 2020 2020 7365 6c66 2c20 6164          self, ad
-00046c20: 6472 3a20 7374 722c 206b 6579 733a 206c  dr: str, keys: l
-00046c30: 6973 745b 7374 725d 2c20 2a2c 2073 7469  ist[str], *, sti
-00046c40: 6d75 6c75 735f 6964 3a20 7374 720a 2020  mulus_id: str.  
-00046c50: 2020 2920 2d3e 204e 6f6e 653a 0a20 2020    ) -> None:.   
-00046c60: 2020 2020 2022 2222 4173 796e 6368 726f       """Asynchro
-00046c70: 6e6f 7573 6c79 2061 736b 2061 2077 6f72  nously ask a wor
-00046c80: 6b65 7220 746f 2064 6973 6361 7264 2069  ker to discard i
-00046c90: 7473 2072 6570 6c69 6361 206f 6620 7468  ts replica of th
-00046ca0: 6520 6c69 7374 6564 206b 6579 732e 0a20  e listed keys.. 
-00046cb0: 2020 2020 2020 2054 6869 7320 6d75 7374         This must
-00046cc0: 206e 6576 6572 2062 6520 7573 6564 2074   never be used t
-00046cd0: 6f20 6465 7374 726f 7920 7468 6520 6c61  o destroy the la
-00046ce0: 7374 2072 6570 6c69 6361 206f 6620 6120  st replica of a 
-00046cf0: 6b65 792e 2054 6869 7320 6973 2061 0a20  key. This is a. 
-00046d00: 2020 2020 2020 2066 6972 652d 616e 642d         fire-and-
-00046d10: 666f 7267 6574 206f 7065 7261 7469 6f6e  forget operation
-00046d20: 2c20 696e 7465 6e64 6564 2066 6f72 2068  , intended for h
-00046d30: 6f75 7365 6b65 6570 696e 6720 616e 6420  ousekeeping and 
-00046d40: 6e6f 7420 666f 7220 636f 6d70 7574 6174  not for computat
-00046d50: 696f 6e2e 0a0a 2020 2020 2020 2020 5468  ion...        Th
-00046d60: 6520 7265 706c 6963 6120 6469 7361 7070  e replica disapp
-00046d70: 6561 7273 2069 6d6d 6564 6961 7465 6c79  ears immediately
-00046d80: 2066 726f 6d20 5461 736b 5374 6174 652e   from TaskState.
-00046d90: 7768 6f5f 6861 7320 6f6e 2074 6865 2053  who_has on the S
-00046da0: 6368 6564 756c 6572 2073 6964 653b 0a20  cheduler side;. 
-00046db0: 2020 2020 2020 2069 6620 7468 6520 776f         if the wo
-00046dc0: 726b 6572 2072 6566 7573 6573 2074 6f20  rker refuses to 
-00046dd0: 6465 6c65 7465 2c20 652e 672e 2062 6563  delete, e.g. bec
-00046de0: 6175 7365 2074 6865 2074 6173 6b20 6973  ause the task is
-00046df0: 2061 2064 6570 656e 6465 6e63 7920 6f66   a dependency of
-00046e00: 0a20 2020 2020 2020 2061 6e6f 7468 6572  .        another
-00046e10: 2074 6173 6b20 7275 6e6e 696e 6720 6f6e   task running on
-00046e20: 2069 742c 2069 7420 7769 6c6c 2028 616c   it, it will (al
-00046e30: 736f 2061 7379 6e63 6872 6f6e 6f75 736c  so asynchronousl
-00046e40: 7929 2069 6e66 6f72 6d20 7468 6520 7363  y) inform the sc
-00046e50: 6865 6475 6c65 720a 2020 2020 2020 2020  heduler.        
-00046e60: 746f 2072 652d 6164 6420 6974 7365 6c66  to re-add itself
-00046e70: 2074 6f20 7768 6f5f 6861 732e 2049 6620   to who_has. If 
-00046e80: 7468 6520 776f 726b 6572 2061 6772 6565  the worker agree
-00046e90: 7320 746f 2064 6973 6361 7264 2074 6865  s to discard the
-00046ea0: 2074 6173 6b2c 2074 6865 7265 2069 730a   task, there is.
-00046eb0: 2020 2020 2020 2020 6e6f 2066 6565 6462          no feedb
-00046ec0: 6163 6b2e 0a20 2020 2020 2020 2022 2222  ack..        """
-00046ed0: 0a20 2020 2020 2020 2077 7320 3d20 7365  .        ws = se
-00046ee0: 6c66 2e77 6f72 6b65 7273 5b61 6464 725d  lf.workers[addr]
-00046ef0: 0a0a 2020 2020 2020 2020 2320 5468 6520  ..        # The 
-00046f00: 7363 6865 6475 6c65 7220 696d 6d65 6469  scheduler immedi
-00046f10: 6174 656c 7920 666f 7267 6574 7320 6162  ately forgets ab
-00046f20: 6f75 7420 7468 6520 7265 706c 6963 6120  out the replica 
-00046f30: 616e 6420 7375 6767 6573 7473 2074 6865  and suggests the
-00046f40: 2077 6f72 6b65 7220 746f 0a20 2020 2020   worker to.     
-00046f50: 2020 2023 2064 726f 7020 6974 2e20 5468     # drop it. Th
-00046f60: 6520 776f 726b 6572 206d 6179 2072 6566  e worker may ref
-00046f70: 7573 652c 2061 7420 7768 6963 6820 706f  use, at which po
-00046f80: 696e 7420 6974 2077 696c 6c20 7365 6e64  int it will send
-00046f90: 2062 6163 6b20 616e 2061 6464 2d6b 6579   back an add-key
-00046fa0: 730a 2020 2020 2020 2020 2320 6d65 7373  s.        # mess
-00046fb0: 6167 6520 746f 2072 6569 6e73 7461 7465  age to reinstate
-00046fc0: 2069 742e 0a20 2020 2020 2020 2066 6f72   it..        for
-00046fd0: 206b 6579 2069 6e20 6b65 7973 3a0a 2020   key in keys:.  
-00046fe0: 2020 2020 2020 2020 2020 7473 203d 2073            ts = s
-00046ff0: 656c 662e 7461 736b 735b 6b65 795d 0a20  elf.tasks[key]. 
-00047000: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00047010: 6c66 2e76 616c 6964 6174 653a 0a20 2020  lf.validate:.   
-00047020: 2020 2020 2020 2020 2020 2020 2023 2044               # D
-00047030: 6f20 6e6f 7420 6465 7374 726f 7920 7468  o not destroy th
-00047040: 6520 6c61 7374 2063 6f70 790a 2020 2020  e last copy.    
-00047050: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-00047060: 7274 206c 656e 2874 732e 7768 6f5f 6861  rt len(ts.who_ha
-00047070: 7329 203e 2031 0a20 2020 2020 2020 2020  s) > 1.         
-00047080: 2020 2073 656c 662e 7265 6d6f 7665 5f72     self.remove_r
-00047090: 6570 6c69 6361 2874 732c 2077 7329 0a0a  eplica(ts, ws)..
-000470a0: 2020 2020 2020 2020 7365 6c66 2e73 7472          self.str
-000470b0: 6561 6d5f 636f 6d6d 735b 6164 6472 5d2e  eam_comms[addr].
-000470c0: 7365 6e64 280a 2020 2020 2020 2020 2020  send(.          
-000470d0: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-000470e0: 2020 2020 226f 7022 3a20 2272 656d 6f76      "op": "remov
-000470f0: 652d 7265 706c 6963 6173 222c 0a20 2020  e-replicas",.   
-00047100: 2020 2020 2020 2020 2020 2020 2022 6b65               "ke
-00047110: 7973 223a 206b 6579 732c 0a20 2020 2020  ys": keys,.     
-00047120: 2020 2020 2020 2020 2020 2022 7374 696d             "stim
-00047130: 756c 7573 5f69 6422 3a20 7374 696d 756c  ulus_id": stimul
-00047140: 7573 5f69 642c 0a20 2020 2020 2020 2020  us_id,.         
-00047150: 2020 207d 0a20 2020 2020 2020 2029 0a0a     }.        )..
-00047160: 0a64 6566 205f 7461 736b 5f74 6f5f 7265  .def _task_to_re
-00047170: 706f 7274 5f6d 7367 2874 733a 2054 6173  port_msg(ts: Tas
-00047180: 6b53 7461 7465 2920 2d3e 2064 6963 745b  kState) -> dict[
-00047190: 7374 722c 2041 6e79 5d20 7c20 4e6f 6e65  str, Any] | None
-000471a0: 3a0a 2020 2020 6966 2074 732e 7374 6174  :.    if ts.stat
-000471b0: 6520 3d3d 2022 666f 7267 6f74 7465 6e22  e == "forgotten"
-000471c0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-000471d0: 207b 226f 7022 3a20 2263 616e 6365 6c6c   {"op": "cancell
-000471e0: 6564 2d6b 6579 7322 2c20 226b 6579 7322  ed-keys", "keys"
-000471f0: 3a20 5b74 732e 6b65 795d 7d0a 2020 2020  : [ts.key]}.    
-00047200: 656c 6966 2074 732e 7374 6174 6520 3d3d  elif ts.state ==
-00047210: 2022 6d65 6d6f 7279 223a 0a20 2020 2020   "memory":.     
-00047220: 2020 2072 6574 7572 6e20 7b22 6f70 223a     return {"op":
-00047230: 2022 6b65 792d 696e 2d6d 656d 6f72 7922   "key-in-memory"
-00047240: 2c20 226b 6579 223a 2074 732e 6b65 797d  , "key": ts.key}
-00047250: 0a20 2020 2065 6c69 6620 7473 2e73 7461  .    elif ts.sta
-00047260: 7465 203d 3d20 2265 7272 6564 223a 0a20  te == "erred":. 
-00047270: 2020 2020 2020 2066 6169 6c69 6e67 5f74         failing_t
-00047280: 7320 3d20 7473 2e65 7863 6570 7469 6f6e  s = ts.exception
-00047290: 5f62 6c61 6d65 0a20 2020 2020 2020 2061  _blame.        a
-000472a0: 7373 6572 7420 6661 696c 696e 675f 7473  ssert failing_ts
-000472b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000472c0: 7b0a 2020 2020 2020 2020 2020 2020 226f  {.            "o
-000472d0: 7022 3a20 2274 6173 6b2d 6572 7265 6422  p": "task-erred"
-000472e0: 2c0a 2020 2020 2020 2020 2020 2020 226b  ,.            "k
-000472f0: 6579 223a 2074 732e 6b65 792c 0a20 2020  ey": ts.key,.   
-00047300: 2020 2020 2020 2020 2022 6578 6365 7074           "except
-00047310: 696f 6e22 3a20 6661 696c 696e 675f 7473  ion": failing_ts
-00047320: 2e65 7863 6570 7469 6f6e 2c0a 2020 2020  .exception,.    
-00047330: 2020 2020 2020 2020 2274 7261 6365 6261          "traceba
-00047340: 636b 223a 2066 6169 6c69 6e67 5f74 732e  ck": failing_ts.
-00047350: 7472 6163 6562 6163 6b2c 0a20 2020 2020  traceback,.     
-00047360: 2020 207d 0a20 2020 2065 6c73 653a 0a20     }.    else:. 
-00047370: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-00047380: 6e65 0a0a 0a64 6566 205f 7461 736b 5f74  ne...def _task_t
-00047390: 6f5f 636c 6965 6e74 5f6d 7367 7328 7473  o_client_msgs(ts
-000473a0: 3a20 5461 736b 5374 6174 6529 202d 3e20  : TaskState) -> 
-000473b0: 6469 6374 5b73 7472 2c20 6c69 7374 5b64  dict[str, list[d
-000473c0: 6963 745b 7374 722c 2041 6e79 5d5d 5d3a  ict[str, Any]]]:
-000473d0: 0a20 2020 2069 6620 7473 2e77 686f 5f77  .    if ts.who_w
-000473e0: 616e 7473 3a0a 2020 2020 2020 2020 7265  ants:.        re
-000473f0: 706f 7274 5f6d 7367 203d 205f 7461 736b  port_msg = _task
-00047400: 5f74 6f5f 7265 706f 7274 5f6d 7367 2874  _to_report_msg(t
-00047410: 7329 0a20 2020 2020 2020 2069 6620 7265  s).        if re
-00047420: 706f 7274 5f6d 7367 2069 7320 6e6f 7420  port_msg is not 
-00047430: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00047440: 2020 7265 7475 726e 207b 6373 2e63 6c69    return {cs.cli
-00047450: 656e 745f 6b65 793a 205b 7265 706f 7274  ent_key: [report
-00047460: 5f6d 7367 5d20 666f 7220 6373 2069 6e20  _msg] for cs in 
-00047470: 7473 2e77 686f 5f77 616e 7473 7d0a 2020  ts.who_wants}.  
-00047480: 2020 7265 7475 726e 207b 7d0a 0a0a 6465    return {}...de
-00047490: 6620 6465 6369 6465 5f77 6f72 6b65 7228  f decide_worker(
-000474a0: 0a20 2020 2074 733a 2054 6173 6b53 7461  .    ts: TaskSta
-000474b0: 7465 2c0a 2020 2020 616c 6c5f 776f 726b  te,.    all_work
-000474c0: 6572 733a 2049 7465 7261 626c 655b 576f  ers: Iterable[Wo
-000474d0: 726b 6572 5374 6174 655d 2c0a 2020 2020  rkerState],.    
-000474e0: 7661 6c69 645f 776f 726b 6572 733a 2073  valid_workers: s
-000474f0: 6574 5b57 6f72 6b65 7253 7461 7465 5d20  et[WorkerState] 
-00047500: 7c20 4e6f 6e65 2c0a 2020 2020 6f62 6a65  | None,.    obje
-00047510: 6374 6976 653a 2043 616c 6c61 626c 655b  ctive: Callable[
-00047520: 5b57 6f72 6b65 7253 7461 7465 5d2c 2041  [WorkerState], A
-00047530: 6e79 5d2c 0a29 202d 3e20 576f 726b 6572  ny],.) -> Worker
-00047540: 5374 6174 6520 7c20 4e6f 6e65 3a0a 2020  State | None:.  
-00047550: 2020 2222 220a 2020 2020 4465 6369 6465    """.    Decide
-00047560: 2077 6869 6368 2077 6f72 6b65 7220 7368   which worker sh
-00047570: 6f75 6c64 2074 616b 6520 7461 736b 202a  ould take task *
-00047580: 7473 2a2e 0a0a 2020 2020 5765 2063 686f  ts*...    We cho
-00047590: 6f73 6520 7468 6520 776f 726b 6572 2074  ose the worker t
-000475a0: 6861 7420 6861 7320 7468 6520 6461 7461  hat has the data
-000475b0: 206f 6e20 7768 6963 6820 2a74 732a 2064   on which *ts* d
-000475c0: 6570 656e 6473 2e0a 0a20 2020 2049 6620  epends...    If 
-000475d0: 7365 7665 7261 6c20 776f 726b 6572 7320  several workers 
-000475e0: 6861 7665 2064 6570 656e 6465 6e63 6965  have dependencie
-000475f0: 7320 7468 656e 2077 6520 6368 6f6f 7365  s then we choose
-00047600: 2074 6865 206c 6573 732d 6275 7379 2077   the less-busy w
-00047610: 6f72 6b65 722e 0a0a 2020 2020 4f70 7469  orker...    Opti
-00047620: 6f6e 616c 6c79 2070 726f 7669 6465 202a  onally provide *
-00047630: 7661 6c69 645f 776f 726b 6572 732a 206f  valid_workers* o
-00047640: 6620 7768 6572 6520 6a6f 6273 2061 7265  f where jobs are
-00047650: 2061 6c6c 6f77 6564 2074 6f20 6f63 6375   allowed to occu
-00047660: 720a 2020 2020 2869 6620 616c 6c20 776f  r.    (if all wo
-00047670: 726b 6572 7320 6172 6520 616c 6c6f 7765  rkers are allowe
-00047680: 6420 746f 2074 616b 6520 7468 6520 7461  d to take the ta
-00047690: 736b 2c20 7061 7373 204e 6f6e 6520 696e  sk, pass None in
-000476a0: 7374 6561 6429 2e0a 0a20 2020 2049 6620  stead)...    If 
-000476b0: 7468 6520 7461 736b 2072 6571 7569 7265  the task require
-000476c0: 7320 6461 7461 2063 6f6d 6d75 6e69 6361  s data communica
-000476d0: 7469 6f6e 2062 6563 6175 7365 206e 6f20  tion because no 
-000476e0: 656c 6967 6962 6c65 2077 6f72 6b65 7220  eligible worker 
-000476f0: 6861 730a 2020 2020 616c 6c20 7468 6520  has.    all the 
-00047700: 6465 7065 6e64 656e 6369 6573 2061 6c72  dependencies alr
-00047710: 6561 6479 2c20 7468 656e 2077 6520 6368  eady, then we ch
-00047720: 6f6f 7365 2074 6f20 6d69 6e69 6d69 7a65  oose to minimize
-00047730: 2074 6865 206e 756d 6265 720a 2020 2020   the number.    
-00047740: 6f66 2062 7974 6573 2073 656e 7420 6265  of bytes sent be
-00047750: 7477 6565 6e20 776f 726b 6572 732e 2020  tween workers.  
-00047760: 5468 6973 2069 7320 6465 7465 726d 696e  This is determin
-00047770: 6564 2062 7920 6361 6c6c 696e 6720 7468  ed by calling th
-00047780: 650a 2020 2020 2a6f 626a 6563 7469 7665  e.    *objective
-00047790: 2a20 6675 6e63 7469 6f6e 2e0a 2020 2020  * function..    
-000477a0: 2222 220a 2020 2020 6173 7365 7274 2061  """.    assert a
-000477b0: 6c6c 2864 7473 2e77 686f 5f68 6173 2066  ll(dts.who_has f
-000477c0: 6f72 2064 7473 2069 6e20 7473 2e64 6570  or dts in ts.dep
-000477d0: 656e 6465 6e63 6965 7329 0a20 2020 2069  endencies).    i
-000477e0: 6620 7473 2e61 6374 6f72 3a0a 2020 2020  f ts.actor:.    
-000477f0: 2020 2020 6361 6e64 6964 6174 6573 203d      candidates =
-00047800: 2073 6574 2861 6c6c 5f77 6f72 6b65 7273   set(all_workers
-00047810: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-00047820: 2020 2020 6361 6e64 6964 6174 6573 203d      candidates =
-00047830: 207b 7777 7320 666f 7220 6474 7320 696e   {wws for dts in
-00047840: 2074 732e 6465 7065 6e64 656e 6369 6573   ts.dependencies
-00047850: 2066 6f72 2077 7773 2069 6e20 6474 732e   for wws in dts.
-00047860: 7768 6f5f 6861 737d 0a20 2020 2069 6620  who_has}.    if 
-00047870: 7661 6c69 645f 776f 726b 6572 7320 6973  valid_workers is
-00047880: 204e 6f6e 653a 0a20 2020 2020 2020 2069   None:.        i
-00047890: 6620 6e6f 7420 6361 6e64 6964 6174 6573  f not candidates
-000478a0: 3a0a 2020 2020 2020 2020 2020 2020 6361  :.            ca
-000478b0: 6e64 6964 6174 6573 203d 2073 6574 2861  ndidates = set(a
-000478c0: 6c6c 5f77 6f72 6b65 7273 290a 2020 2020  ll_workers).    
-000478d0: 656c 7365 3a0a 2020 2020 2020 2020 6361  else:.        ca
-000478e0: 6e64 6964 6174 6573 2026 3d20 7661 6c69  ndidates &= vali
-000478f0: 645f 776f 726b 6572 730a 2020 2020 2020  d_workers.      
-00047900: 2020 6966 206e 6f74 2063 616e 6469 6461    if not candida
-00047910: 7465 733a 0a20 2020 2020 2020 2020 2020  tes:.           
-00047920: 2063 616e 6469 6461 7465 7320 3d20 7661   candidates = va
-00047930: 6c69 645f 776f 726b 6572 730a 2020 2020  lid_workers.    
-00047940: 2020 2020 2020 2020 6966 206e 6f74 2063          if not c
-00047950: 616e 6469 6461 7465 733a 0a20 2020 2020  andidates:.     
-00047960: 2020 2020 2020 2020 2020 2069 6620 7473             if ts
-00047970: 2e6c 6f6f 7365 5f72 6573 7472 6963 7469  .loose_restricti
-00047980: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
-00047990: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000479a0: 6465 6369 6465 5f77 6f72 6b65 7228 7473  decide_worker(ts
-000479b0: 2c20 616c 6c5f 776f 726b 6572 732c 204e  , all_workers, N
-000479c0: 6f6e 652c 206f 626a 6563 7469 7665 290a  one, objective).
-000479d0: 0a20 2020 2069 6620 6e6f 7420 6361 6e64  .    if not cand
-000479e0: 6964 6174 6573 3a0a 2020 2020 2020 2020  idates:.        
-000479f0: 7265 7475 726e 204e 6f6e 650a 2020 2020  return None.    
-00047a00: 656c 6966 206c 656e 2863 616e 6469 6461  elif len(candida
-00047a10: 7465 7329 203d 3d20 313a 0a20 2020 2020  tes) == 1:.     
-00047a20: 2020 2072 6574 7572 6e20 6e65 7874 2869     return next(i
-00047a30: 7465 7228 6361 6e64 6964 6174 6573 2929  ter(candidates))
-00047a40: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-00047a50: 2020 2072 6574 7572 6e20 6d69 6e28 6361     return min(ca
-00047a60: 6e64 6964 6174 6573 2c20 6b65 793d 6f62  ndidates, key=ob
-00047a70: 6a65 6374 6976 6529 0a0a 0a64 6566 2076  jective)...def v
-00047a80: 616c 6964 6174 655f 7461 736b 5f73 7461  alidate_task_sta
-00047a90: 7465 2874 733a 2054 6173 6b53 7461 7465  te(ts: TaskState
-00047aa0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2022  ) -> None:.    "
-00047ab0: 2222 5661 6c69 6461 7465 2074 6865 2067  ""Validate the g
-00047ac0: 6976 656e 2054 6173 6b53 7461 7465 2222  iven TaskState""
-00047ad0: 220a 2020 2020 6173 7365 7274 2074 732e  ".    assert ts.
-00047ae0: 7374 6174 6520 696e 2041 4c4c 5f54 4153  state in ALL_TAS
-00047af0: 4b5f 5354 4154 4553 2c20 7473 0a0a 2020  K_STATES, ts..  
-00047b00: 2020 6966 2074 732e 7761 6974 696e 675f    if ts.waiting_
-00047b10: 6f6e 3a0a 2020 2020 2020 2020 6173 7365  on:.        asse
-00047b20: 7274 2074 732e 7761 6974 696e 675f 6f6e  rt ts.waiting_on
-00047b30: 2e69 7373 7562 7365 7428 7473 2e64 6570  .issubset(ts.dep
-00047b40: 656e 6465 6e63 6965 7329 2c20 280a 2020  endencies), (.  
-00047b50: 2020 2020 2020 2020 2020 2277 6169 7469            "waiti
-00047b60: 6e67 206e 6f74 2073 7562 7365 7420 6f66  ng not subset of
-00047b70: 2064 6570 656e 6465 6e63 6965 7322 2c0a   dependencies",.
-00047b80: 2020 2020 2020 2020 2020 2020 7374 7228              str(
-00047b90: 7473 2e77 6169 7469 6e67 5f6f 6e29 2c0a  ts.waiting_on),.
-00047ba0: 2020 2020 2020 2020 2020 2020 7374 7228              str(
-00047bb0: 7473 2e64 6570 656e 6465 6e63 6965 7329  ts.dependencies)
-00047bc0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-00047bd0: 6966 2074 732e 7761 6974 6572 733a 0a20  if ts.waiters:. 
-00047be0: 2020 2020 2020 2061 7373 6572 7420 7473         assert ts
-00047bf0: 2e77 6169 7465 7273 2e69 7373 7562 7365  .waiters.issubse
-00047c00: 7428 7473 2e64 6570 656e 6465 6e74 7329  t(ts.dependents)
-00047c10: 2c20 280a 2020 2020 2020 2020 2020 2020  , (.            
-00047c20: 2277 6169 7465 7273 206e 6f74 2073 7562  "waiters not sub
-00047c30: 7365 7420 6f66 2064 6570 656e 6465 6e74  set of dependent
-00047c40: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-00047c50: 7374 7228 7473 2e77 6169 7465 7273 292c  str(ts.waiters),
-00047c60: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
-00047c70: 2874 732e 6465 7065 6e64 656e 7473 292c  (ts.dependents),
-00047c80: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00047c90: 666f 7220 6474 7320 696e 2074 732e 7761  for dts in ts.wa
-00047ca0: 6974 696e 675f 6f6e 3a0a 2020 2020 2020  iting_on:.      
-00047cb0: 2020 6173 7365 7274 206e 6f74 2064 7473    assert not dts
-00047cc0: 2e77 686f 5f68 6173 2c20 2822 7761 6974  .who_has, ("wait
-00047cd0: 696e 6720 6f6e 2069 6e2d 6d65 6d6f 7279  ing on in-memory
-00047ce0: 2064 6570 222c 2073 7472 2874 7329 2c20   dep", str(ts), 
-00047cf0: 7374 7228 6474 7329 290a 2020 2020 2020  str(dts)).      
-00047d00: 2020 6173 7365 7274 2064 7473 2e73 7461    assert dts.sta
-00047d10: 7465 2021 3d20 2272 656c 6561 7365 6422  te != "released"
-00047d20: 2c20 2822 7761 6974 696e 6720 6f6e 2072  , ("waiting on r
-00047d30: 656c 6561 7365 6420 6465 7022 2c20 7374  eleased dep", st
-00047d40: 7228 7473 292c 2073 7472 2864 7473 2929  r(ts), str(dts))
-00047d50: 0a20 2020 2066 6f72 2064 7473 2069 6e20  .    for dts in 
-00047d60: 7473 2e64 6570 656e 6465 6e63 6965 733a  ts.dependencies:
-00047d70: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00047d80: 7473 2069 6e20 6474 732e 6465 7065 6e64  ts in dts.depend
-00047d90: 656e 7473 2c20 280a 2020 2020 2020 2020  ents, (.        
-00047da0: 2020 2020 226e 6f74 2069 6e20 6465 7065      "not in depe
-00047db0: 6e64 656e 6379 2773 2064 6570 656e 6465  ndency's depende
-00047dc0: 6e74 7322 2c0a 2020 2020 2020 2020 2020  nts",.          
-00047dd0: 2020 7374 7228 7473 292c 0a20 2020 2020    str(ts),.     
-00047de0: 2020 2020 2020 2073 7472 2864 7473 292c         str(dts),
-00047df0: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
-00047e00: 2864 7473 2e64 6570 656e 6465 6e74 7329  (dts.dependents)
-00047e10: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-00047e20: 2020 2020 6966 2074 732e 7374 6174 6520      if ts.state 
-00047e30: 696e 2028 2277 6169 7469 6e67 222c 2022  in ("waiting", "
-00047e40: 7175 6575 6564 222c 2022 7072 6f63 6573  queued", "proces
-00047e50: 7369 6e67 222c 2022 6e6f 2d77 6f72 6b65  sing", "no-worke
-00047e60: 7222 293a 0a20 2020 2020 2020 2020 2020  r"):.           
-00047e70: 2061 7373 6572 7420 6474 7320 696e 2074   assert dts in t
-00047e80: 732e 7761 6974 696e 675f 6f6e 206f 7220  s.waiting_on or 
-00047e90: 6474 732e 7768 6f5f 6861 732c 2028 0a20  dts.who_has, (. 
-00047ea0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00047eb0: 6465 7020 6d69 7373 696e 6722 2c0a 2020  dep missing",.  
-00047ec0: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00047ed0: 7228 7473 292c 0a20 2020 2020 2020 2020  r(ts),.         
-00047ee0: 2020 2020 2020 2073 7472 2864 7473 292c         str(dts),
-00047ef0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00047f00: 2020 2020 2020 2061 7373 6572 7420 6474         assert dt
-00047f10: 732e 7374 6174 6520 213d 2022 666f 7267  s.state != "forg
-00047f20: 6f74 7465 6e22 0a0a 2020 2020 666f 7220  otten"..    for 
-00047f30: 6474 7320 696e 2074 732e 7761 6974 6572  dts in ts.waiter
-00047f40: 733a 0a20 2020 2020 2020 2061 7373 6572  s:.        asser
-00047f50: 7420 6474 732e 7374 6174 6520 696e 2028  t dts.state in (
-00047f60: 2277 6169 7469 6e67 222c 2022 7175 6575  "waiting", "queu
-00047f70: 6564 222c 2022 7072 6f63 6573 7369 6e67  ed", "processing
-00047f80: 222c 2022 6e6f 2d77 6f72 6b65 7222 292c  ", "no-worker"),
-00047f90: 2028 0a20 2020 2020 2020 2020 2020 2022   (.            "
-00047fa0: 7761 6974 6572 206e 6f74 2069 6e20 706c  waiter not in pl
-00047fb0: 6179 222c 0a20 2020 2020 2020 2020 2020  ay",.           
-00047fc0: 2073 7472 2874 7329 2c0a 2020 2020 2020   str(ts),.      
-00047fd0: 2020 2020 2020 7374 7228 6474 7329 2c0a        str(dts),.
-00047fe0: 2020 2020 2020 2020 290a 2020 2020 666f          ).    fo
-00047ff0: 7220 6474 7320 696e 2074 732e 6465 7065  r dts in ts.depe
-00048000: 6e64 656e 7473 3a0a 2020 2020 2020 2020  ndents:.        
-00048010: 6173 7365 7274 2074 7320 696e 2064 7473  assert ts in dts
-00048020: 2e64 6570 656e 6465 6e63 6965 732c 2028  .dependencies, (
-00048030: 0a20 2020 2020 2020 2020 2020 2022 6e6f  .            "no
-00048040: 7420 696e 2064 6570 656e 6465 6e74 2773  t in dependent's
-00048050: 2064 6570 656e 6465 6e63 6965 7322 2c0a   dependencies",.
-00048060: 2020 2020 2020 2020 2020 2020 7374 7228              str(
-00048070: 7473 292c 0a20 2020 2020 2020 2020 2020  ts),.           
-00048080: 2073 7472 2864 7473 292c 0a20 2020 2020   str(dts),.     
-00048090: 2020 2020 2020 2073 7472 2864 7473 2e64         str(dts.d
-000480a0: 6570 656e 6465 6e63 6965 7329 2c0a 2020  ependencies),.  
-000480b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000480c0: 6173 7365 7274 2064 7473 2e73 7461 7465  assert dts.state
-000480d0: 2021 3d20 2266 6f72 676f 7474 656e 220a   != "forgotten".
-000480e0: 0a20 2020 2061 7373 6572 7420 2874 732e  .    assert (ts.
-000480f0: 7072 6f63 6573 7369 6e67 5f6f 6e20 6973  processing_on is
-00048100: 206e 6f74 204e 6f6e 6529 203d 3d20 2874   not None) == (t
-00048110: 732e 7374 6174 6520 3d3d 2022 7072 6f63  s.state == "proc
-00048120: 6573 7369 6e67 2229 0a20 2020 2061 7373  essing").    ass
-00048130: 6572 7420 626f 6f6c 2874 732e 7768 6f5f  ert bool(ts.who_
-00048140: 6861 7329 203d 3d20 2874 732e 7374 6174  has) == (ts.stat
-00048150: 6520 3d3d 2022 6d65 6d6f 7279 2229 2c20  e == "memory"), 
-00048160: 2874 732c 2074 732e 7768 6f5f 6861 732c  (ts, ts.who_has,
-00048170: 2074 732e 7374 6174 6529 0a0a 2020 2020   ts.state)..    
-00048180: 6966 2074 732e 7374 6174 6520 3d3d 2022  if ts.state == "
-00048190: 7175 6575 6564 223a 0a20 2020 2020 2020  queued":.       
-000481a0: 2061 7373 6572 7420 6e6f 7420 7473 2e70   assert not ts.p
-000481b0: 726f 6365 7373 696e 675f 6f6e 0a20 2020  rocessing_on.   
-000481c0: 2020 2020 2061 7373 6572 7420 6e6f 7420       assert not 
-000481d0: 7473 2e77 686f 5f68 6173 0a20 2020 2020  ts.who_has.     
-000481e0: 2020 2061 7373 6572 7420 616c 6c28 6474     assert all(dt
-000481f0: 732e 7768 6f5f 6861 7320 666f 7220 6474  s.who_has for dt
-00048200: 7320 696e 2074 732e 6465 7065 6e64 656e  s in ts.dependen
-00048210: 6369 6573 292c 2028 0a20 2020 2020 2020  cies), (.       
-00048220: 2020 2020 2022 7461 736b 2071 7565 7565       "task queue
-00048230: 6420 7769 7468 6f75 7420 616c 6c20 6465  d without all de
-00048240: 7073 222c 0a20 2020 2020 2020 2020 2020  ps",.           
-00048250: 2073 7472 2874 7329 2c0a 2020 2020 2020   str(ts),.      
-00048260: 2020 2020 2020 7374 7228 7473 2e64 6570        str(ts.dep
-00048270: 656e 6465 6e63 6965 7329 2c0a 2020 2020  endencies),.    
-00048280: 2020 2020 290a 0a20 2020 2069 6620 7473      )..    if ts
-00048290: 2e73 7461 7465 203d 3d20 2270 726f 6365  .state == "proce
-000482a0: 7373 696e 6722 3a0a 2020 2020 2020 2020  ssing":.        
-000482b0: 6173 7365 7274 2061 6c6c 2864 7473 2e77  assert all(dts.w
-000482c0: 686f 5f68 6173 2066 6f72 2064 7473 2069  ho_has for dts i
-000482d0: 6e20 7473 2e64 6570 656e 6465 6e63 6965  n ts.dependencie
-000482e0: 7329 2c20 280a 2020 2020 2020 2020 2020  s), (.          
-000482f0: 2020 2274 6173 6b20 7072 6f63 6573 7369    "task processi
-00048300: 6e67 2077 6974 686f 7574 2061 6c6c 2064  ng without all d
-00048310: 6570 7322 2c0a 2020 2020 2020 2020 2020  eps",.          
-00048320: 2020 7374 7228 7473 292c 0a20 2020 2020    str(ts),.     
-00048330: 2020 2020 2020 2073 7472 2874 732e 6465         str(ts.de
-00048340: 7065 6e64 656e 6369 6573 292c 0a20 2020  pendencies),.   
-00048350: 2020 2020 2029 0a20 2020 2020 2020 2061       ).        a
-00048360: 7373 6572 7420 6e6f 7420 7473 2e77 6169  ssert not ts.wai
-00048370: 7469 6e67 5f6f 6e0a 0a20 2020 2069 6620  ting_on..    if 
-00048380: 7473 2e77 686f 5f68 6173 3a0a 2020 2020  ts.who_has:.    
-00048390: 2020 2020 6173 7365 7274 2074 732e 7761      assert ts.wa
-000483a0: 6974 6572 7320 6f72 2074 732e 7768 6f5f  iters or ts.who_
-000483b0: 7761 6e74 732c 2028 0a20 2020 2020 2020  wants, (.       
-000483c0: 2020 2020 2022 756e 6e65 6564 6564 2074       "unneeded t
-000483d0: 6173 6b20 696e 206d 656d 6f72 7922 2c0a  ask in memory",.
-000483e0: 2020 2020 2020 2020 2020 2020 7374 7228              str(
-000483f0: 7473 292c 0a20 2020 2020 2020 2020 2020  ts),.           
-00048400: 2073 7472 2874 732e 7768 6f5f 6861 7329   str(ts.who_has)
-00048410: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-00048420: 2020 2020 6966 2074 732e 7275 6e5f 7370      if ts.run_sp
-00048430: 6563 3a20 2023 2077 6173 2063 6f6d 7075  ec:  # was compu
-00048440: 7465 640a 2020 2020 2020 2020 2020 2020  ted.            
-00048450: 6173 7365 7274 2074 732e 7479 7065 0a20  assert ts.type. 
-00048460: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-00048470: 7420 6973 696e 7374 616e 6365 2874 732e  t isinstance(ts.
-00048480: 7479 7065 2c20 7374 7229 0a20 2020 2020  type, str).     
-00048490: 2020 2061 7373 6572 7420 6e6f 7420 616e     assert not an
-000484a0: 7928 5b74 7320 696e 2064 7473 2e77 6169  y([ts in dts.wai
-000484b0: 7469 6e67 5f6f 6e20 666f 7220 6474 7320  ting_on for dts 
-000484c0: 696e 2074 732e 6465 7065 6e64 656e 7473  in ts.dependents
-000484d0: 5d29 0a20 2020 2020 2020 2066 6f72 2077  ]).        for w
-000484e0: 7320 696e 2074 732e 7768 6f5f 6861 733a  s in ts.who_has:
-000484f0: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-00048500: 6572 7420 7473 2069 6e20 7773 2e68 6173  ert ts in ws.has
-00048510: 5f77 6861 742c 2028 0a20 2020 2020 2020  _what, (.       
-00048520: 2020 2020 2020 2020 2022 6e6f 7420 696e           "not in
-00048530: 2077 686f 5f68 6173 2720 6861 735f 7768   who_has' has_wh
-00048540: 6174 222c 0a20 2020 2020 2020 2020 2020  at",.           
-00048550: 2020 2020 2073 7472 2874 7329 2c0a 2020       str(ts),.  
-00048560: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00048570: 7228 7773 292c 0a20 2020 2020 2020 2020  r(ws),.         
-00048580: 2020 2020 2020 2073 7472 2877 732e 6861         str(ws.ha
-00048590: 735f 7768 6174 292c 0a20 2020 2020 2020  s_what),.       
-000485a0: 2020 2020 2029 0a0a 2020 2020 666f 7220       )..    for 
-000485b0: 6373 2069 6e20 7473 2e77 686f 5f77 616e  cs in ts.who_wan
-000485c0: 7473 3a0a 2020 2020 2020 2020 6173 7365  ts:.        asse
-000485d0: 7274 2074 7320 696e 2063 732e 7761 6e74  rt ts in cs.want
-000485e0: 735f 7768 6174 2c20 280a 2020 2020 2020  s_what, (.      
-000485f0: 2020 2020 2020 226e 6f74 2069 6e20 7768        "not in wh
-00048600: 6f5f 7761 6e74 7327 2077 616e 7473 5f77  o_wants' wants_w
-00048610: 6861 7422 2c0a 2020 2020 2020 2020 2020  hat",.          
-00048620: 2020 7374 7228 7473 292c 0a20 2020 2020    str(ts),.     
-00048630: 2020 2020 2020 2073 7472 2863 7329 2c0a         str(cs),.
-00048640: 2020 2020 2020 2020 2020 2020 7374 7228              str(
-00048650: 6373 2e77 616e 7473 5f77 6861 7429 2c0a  cs.wants_what),.
-00048660: 2020 2020 2020 2020 290a 0a20 2020 2069          )..    i
-00048670: 6620 7473 2e61 6374 6f72 3a0a 2020 2020  f ts.actor:.    
-00048680: 2020 2020 6966 2074 732e 7374 6174 6520      if ts.state 
-00048690: 3d3d 2022 6d65 6d6f 7279 223a 0a20 2020  == "memory":.   
-000486a0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-000486b0: 7375 6d28 7473 2069 6e20 7773 2e61 6374  sum(ts in ws.act
-000486c0: 6f72 7320 666f 7220 7773 2069 6e20 7473  ors for ws in ts
-000486d0: 2e77 686f 5f68 6173 2920 3d3d 2031 0a20  .who_has) == 1. 
-000486e0: 2020 2020 2020 2069 6620 7473 2e73 7461         if ts.sta
-000486f0: 7465 203d 3d20 2270 726f 6365 7373 696e  te == "processin
-00048700: 6722 3a0a 2020 2020 2020 2020 2020 2020  g":.            
-00048710: 6173 7365 7274 2074 732e 7072 6f63 6573  assert ts.proces
-00048720: 7369 6e67 5f6f 6e0a 2020 2020 2020 2020  sing_on.        
-00048730: 2020 2020 6173 7365 7274 2074 7320 696e      assert ts in
-00048740: 2074 732e 7072 6f63 6573 7369 6e67 5f6f   ts.processing_o
-00048750: 6e2e 6163 746f 7273 0a20 2020 2020 2020  n.actors.       
-00048760: 2061 7373 6572 7420 7473 2e73 7461 7465   assert ts.state
-00048770: 2021 3d20 2271 7565 7565 6422 0a0a 0a64   != "queued"...d
-00048780: 6566 2076 616c 6964 6174 655f 776f 726b  ef validate_work
-00048790: 6572 5f73 7461 7465 2877 733a 2057 6f72  er_state(ws: Wor
-000487a0: 6b65 7253 7461 7465 2920 2d3e 204e 6f6e  kerState) -> Non
-000487b0: 653a 0a20 2020 2066 6f72 2074 7320 696e  e:.    for ts in
-000487c0: 2077 732e 6861 735f 7768 6174 3a0a 2020   ws.has_what:.  
-000487d0: 2020 2020 2020 6173 7365 7274 2077 7320        assert ws 
-000487e0: 696e 2074 732e 7768 6f5f 6861 732c 2028  in ts.who_has, (
-000487f0: 0a20 2020 2020 2020 2020 2020 2022 6e6f  .            "no
-00048800: 7420 696e 2068 6173 5f77 6861 7427 2077  t in has_what' w
-00048810: 686f 5f68 6173 222c 0a20 2020 2020 2020  ho_has",.       
-00048820: 2020 2020 2073 7472 2877 7329 2c0a 2020       str(ws),.  
-00048830: 2020 2020 2020 2020 2020 7374 7228 7473            str(ts
-00048840: 292c 0a20 2020 2020 2020 2020 2020 2073  ),.            s
-00048850: 7472 2874 732e 7768 6f5f 6861 7329 2c0a  tr(ts.who_has),.
-00048860: 2020 2020 2020 2020 290a 0a20 2020 2066          )..    f
-00048870: 6f72 2074 7320 696e 2077 732e 6163 746f  or ts in ws.acto
-00048880: 7273 3a0a 2020 2020 2020 2020 6173 7365  rs:.        asse
-00048890: 7274 2074 732e 7374 6174 6520 696e 2028  rt ts.state in (
-000488a0: 226d 656d 6f72 7922 2c20 2270 726f 6365  "memory", "proce
-000488b0: 7373 696e 6722 290a 0a0a 6465 6620 7661  ssing")...def va
-000488c0: 6c69 6461 7465 5f73 7461 7465 280a 2020  lidate_state(.  
-000488d0: 2020 7461 736b 733a 2064 6963 745b 7374    tasks: dict[st
-000488e0: 722c 2054 6173 6b53 7461 7465 5d2c 0a20  r, TaskState],. 
-000488f0: 2020 2077 6f72 6b65 7273 3a20 6469 6374     workers: dict
-00048900: 5b73 7472 2c20 576f 726b 6572 5374 6174  [str, WorkerStat
-00048910: 655d 2c0a 2020 2020 636c 6965 6e74 733a  e],.    clients:
-00048920: 2064 6963 745b 7374 722c 2043 6c69 656e   dict[str, Clien
-00048930: 7453 7461 7465 5d2c 0a29 202d 3e20 4e6f  tState],.) -> No
-00048940: 6e65 3a0a 2020 2020 2222 2256 616c 6964  ne:.    """Valid
-00048950: 6174 6520 6120 6375 7272 656e 7420 7275  ate a current ru
-00048960: 6e74 696d 6520 7374 6174 652e 0a0a 2020  ntime state...  
-00048970: 2020 5468 6973 2070 6572 666f 726d 7320    This performs 
-00048980: 6120 7365 7175 656e 6365 206f 6620 6368  a sequence of ch
-00048990: 6563 6b73 206f 6e20 7468 6520 656e 7469  ecks on the enti
-000489a0: 7265 2067 7261 7068 2c20 7275 6e6e 696e  re graph, runnin
-000489b0: 6720 696e 2061 626f 7574 206c 696e 6561  g in about linea
-000489c0: 720a 2020 2020 7469 6d65 2e20 5468 6973  r.    time. This
-000489d0: 2072 6169 7365 7320 6173 7365 7274 2065   raises assert e
-000489e0: 7272 6f72 7320 6966 2061 6e79 7468 696e  rrors if anythin
-000489f0: 6720 646f 6573 6e27 7420 6368 6563 6b20  g doesn't check 
-00048a00: 6f75 742e 0a20 2020 2022 2222 0a20 2020  out..    """.   
-00048a10: 2066 6f72 2074 7320 696e 2074 6173 6b73   for ts in tasks
-00048a20: 2e76 616c 7565 7328 293a 0a20 2020 2020  .values():.     
-00048a30: 2020 2076 616c 6964 6174 655f 7461 736b     validate_task
-00048a40: 5f73 7461 7465 2874 7329 0a0a 2020 2020  _state(ts)..    
-00048a50: 666f 7220 7773 2069 6e20 776f 726b 6572  for ws in worker
-00048a60: 732e 7661 6c75 6573 2829 3a0a 2020 2020  s.values():.    
-00048a70: 2020 2020 7661 6c69 6461 7465 5f77 6f72      validate_wor
-00048a80: 6b65 725f 7374 6174 6528 7773 290a 0a20  ker_state(ws).. 
-00048a90: 2020 2066 6f72 2063 7320 696e 2063 6c69     for cs in cli
-00048aa0: 656e 7473 2e76 616c 7565 7328 293a 0a20  ents.values():. 
-00048ab0: 2020 2020 2020 2066 6f72 2074 7320 696e         for ts in
-00048ac0: 2063 732e 7761 6e74 735f 7768 6174 3a0a   cs.wants_what:.
-00048ad0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-00048ae0: 7274 2063 7320 696e 2074 732e 7768 6f5f  rt cs in ts.who_
-00048af0: 7761 6e74 732c 2028 0a20 2020 2020 2020  wants, (.       
-00048b00: 2020 2020 2020 2020 2022 6e6f 7420 696e           "not in
-00048b10: 2077 616e 7473 5f77 6861 7427 2077 686f   wants_what' who
-00048b20: 5f77 616e 7473 222c 0a20 2020 2020 2020  _wants",.       
-00048b30: 2020 2020 2020 2020 2073 7472 2863 7329           str(cs)
-00048b40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00048b50: 2020 7374 7228 7473 292c 0a20 2020 2020    str(ts),.     
-00048b60: 2020 2020 2020 2020 2020 2073 7472 2874             str(t
-00048b70: 732e 7768 6f5f 7761 6e74 7329 2c0a 2020  s.who_wants),.  
-00048b80: 2020 2020 2020 2020 2020 290a 0a0a 6465            )...de
-00048b90: 6620 6865 6172 7462 6561 745f 696e 7465  f heartbeat_inte
-00048ba0: 7276 616c 286e 3a20 696e 7429 202d 3e20  rval(n: int) -> 
-00048bb0: 666c 6f61 743a 0a20 2020 2022 2222 496e  float:.    """In
-00048bc0: 7465 7276 616c 2069 6e20 7365 636f 6e64  terval in second
-00048bd0: 7320 7468 6174 2077 6520 6465 7369 7265  s that we desire
-00048be0: 2068 6561 7274 6265 6174 7320 6261 7365   heartbeats base
-00048bf0: 6420 6f6e 206e 756d 6265 7220 6f66 2077  d on number of w
-00048c00: 6f72 6b65 7273 2222 220a 2020 2020 6966  orkers""".    if
-00048c10: 206e 203c 3d20 3130 3a0a 2020 2020 2020   n <= 10:.      
-00048c20: 2020 7265 7475 726e 2030 2e35 0a20 2020    return 0.5.   
-00048c30: 2065 6c69 6620 6e20 3c20 3530 3a0a 2020   elif n < 50:.  
-00048c40: 2020 2020 2020 7265 7475 726e 2031 0a20        return 1. 
-00048c50: 2020 2065 6c69 6620 6e20 3c20 3230 303a     elif n < 200:
-00048c60: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00048c70: 320a 2020 2020 656c 7365 3a0a 2020 2020  2.    else:.    
-00048c80: 2020 2020 2320 4e6f 206d 6f72 6520 7468      # No more th
-00048c90: 616e 2032 3030 2068 6561 7274 6265 6174  an 200 heartbeat
-00048ca0: 7320 6120 7365 636f 6e64 2073 6361 6c65  s a second scale
-00048cb0: 6420 6279 2077 6f72 6b65 7273 0a20 2020  d by workers.   
-00048cc0: 2020 2020 2072 6574 7572 6e20 6e20 2f20       return n / 
-00048cd0: 3230 3020 2b20 310a 0a0a 6465 6620 5f74  200 + 1...def _t
-00048ce0: 6173 6b5f 736c 6f74 735f 6176 6169 6c61  ask_slots_availa
-00048cf0: 626c 6528 7773 3a20 576f 726b 6572 5374  ble(ws: WorkerSt
-00048d00: 6174 652c 2073 6174 7572 6174 696f 6e5f  ate, saturation_
-00048d10: 6661 6374 6f72 3a20 666c 6f61 7429 202d  factor: float) -
-00048d20: 3e20 696e 743a 0a20 2020 2022 2222 4e75  > int:.    """Nu
-00048d30: 6d62 6572 206f 6620 7461 736b 7320 7468  mber of tasks th
-00048d40: 6174 2063 616e 2062 6520 7365 6e74 2074  at can be sent t
-00048d50: 6f20 7468 6973 2077 6f72 6b65 7220 7769  o this worker wi
-00048d60: 7468 6f75 7420 6f76 6572 7361 7475 7261  thout oversatura
-00048d70: 7469 6e67 2069 7422 2222 0a20 2020 2061  ting it""".    a
-00048d80: 7373 6572 7420 6e6f 7420 6d61 7468 2e69  ssert not math.i
-00048d90: 7369 6e66 2873 6174 7572 6174 696f 6e5f  sinf(saturation_
-00048da0: 6661 6374 6f72 290a 2020 2020 7265 7475  factor).    retu
-00048db0: 726e 206d 6178 286d 6174 682e 6365 696c  rn max(math.ceil
-00048dc0: 2873 6174 7572 6174 696f 6e5f 6661 6374  (saturation_fact
-00048dd0: 6f72 202a 2077 732e 6e74 6872 6561 6473  or * ws.nthreads
-00048de0: 292c 2031 2920 2d20 280a 2020 2020 2020  ), 1) - (.      
-00048df0: 2020 6c65 6e28 7773 2e70 726f 6365 7373    len(ws.process
-00048e00: 696e 6729 202d 206c 656e 2877 732e 6c6f  ing) - len(ws.lo
-00048e10: 6e67 5f72 756e 6e69 6e67 290a 2020 2020  ng_running).    
-00048e20: 290a 0a0a 6465 6620 5f77 6f72 6b65 725f  )...def _worker_
-00048e30: 6675 6c6c 2877 733a 2057 6f72 6b65 7253  full(ws: WorkerS
-00048e40: 7461 7465 2c20 7361 7475 7261 7469 6f6e  tate, saturation
-00048e50: 5f66 6163 746f 723a 2066 6c6f 6174 2920  _factor: float) 
-00048e60: 2d3e 2062 6f6f 6c3a 0a20 2020 2069 6620  -> bool:.    if 
-00048e70: 6d61 7468 2e69 7369 6e66 2873 6174 7572  math.isinf(satur
-00048e80: 6174 696f 6e5f 6661 6374 6f72 293a 0a20  ation_factor):. 
-00048e90: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00048ea0: 6c73 650a 2020 2020 7265 7475 726e 205f  lse.    return _
-00048eb0: 7461 736b 5f73 6c6f 7473 5f61 7661 696c  task_slots_avail
-00048ec0: 6162 6c65 2877 732c 2073 6174 7572 6174  able(ws, saturat
-00048ed0: 696f 6e5f 6661 6374 6f72 2920 3c3d 2030  ion_factor) <= 0
-00048ee0: 0a0a 0a63 6c61 7373 204b 696c 6c65 6457  ...class KilledW
-00048ef0: 6f72 6b65 7228 4578 6365 7074 696f 6e29  orker(Exception)
-00048f00: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-00048f10: 5f5f 2873 656c 662c 2074 6173 6b3a 2073  __(self, task: s
-00048f20: 7472 2c20 6c61 7374 5f77 6f72 6b65 723a  tr, last_worker:
-00048f30: 2057 6f72 6b65 7253 7461 7465 2c20 616c   WorkerState, al
-00048f40: 6c6f 7765 645f 6661 696c 7572 6573 3a20  lowed_failures: 
-00048f50: 696e 7429 3a0a 2020 2020 2020 2020 7375  int):.        su
-00048f60: 7065 7228 292e 5f5f 696e 6974 5f5f 2874  per().__init__(t
-00048f70: 6173 6b2c 206c 6173 745f 776f 726b 6572  ask, last_worker
-00048f80: 2c20 616c 6c6f 7765 645f 6661 696c 7572  , allowed_failur
-00048f90: 6573 290a 0a20 2020 2040 7072 6f70 6572  es)..    @proper
-00048fa0: 7479 0a20 2020 2064 6566 2074 6173 6b28  ty.    def task(
-00048fb0: 7365 6c66 2920 2d3e 2073 7472 3a0a 2020  self) -> str:.  
-00048fc0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00048fd0: 662e 6172 6773 5b30 5d0a 0a20 2020 2040  f.args[0]..    @
-00048fe0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00048ff0: 206c 6173 745f 776f 726b 6572 2873 656c   last_worker(sel
-00049000: 6629 202d 3e20 576f 726b 6572 5374 6174  f) -> WorkerStat
-00049010: 653a 0a20 2020 2020 2020 2072 6574 7572  e:.        retur
-00049020: 6e20 7365 6c66 2e61 7267 735b 315d 0a0a  n self.args[1]..
-00049030: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00049040: 2020 6465 6620 616c 6c6f 7765 645f 6661    def allowed_fa
-00049050: 696c 7572 6573 2873 656c 6629 202d 3e20  ilures(self) -> 
-00049060: 696e 743a 0a20 2020 2020 2020 2072 6574  int:.        ret
-00049070: 7572 6e20 7365 6c66 2e61 7267 735b 325d  urn self.args[2]
-00049080: 0a0a 2020 2020 6465 6620 5f5f 7374 725f  ..    def __str_
-00049090: 5f28 7365 6c66 2920 2d3e 2073 7472 3a0a  _(self) -> str:.
-000490a0: 2020 2020 2020 2020 7265 7475 726e 2028          return (
-000490b0: 0a20 2020 2020 2020 2020 2020 2066 2241  .            f"A
-000490c0: 7474 656d 7074 6564 2074 6f20 7275 6e20  ttempted to run 
-000490d0: 7461 736b 207b 7365 6c66 2e74 6173 6b7d  task {self.task}
-000490e0: 206f 6e20 7b73 656c 662e 616c 6c6f 7765   on {self.allowe
-000490f0: 645f 6661 696c 7572 6573 7d20 6469 6666  d_failures} diff
-00049100: 6572 656e 7420 220a 2020 2020 2020 2020  erent ".        
-00049110: 2020 2020 2277 6f72 6b65 7273 2c20 6275      "workers, bu
-00049120: 7420 616c 6c20 7468 6f73 6520 776f 726b  t all those work
-00049130: 6572 7320 6469 6564 2077 6869 6c65 2072  ers died while r
-00049140: 756e 6e69 6e67 2069 742e 2022 0a20 2020  unning it. ".   
-00049150: 2020 2020 2020 2020 2066 2254 6865 206c           f"The l
-00049160: 6173 7420 776f 726b 6572 2074 6861 7420  ast worker that 
-00049170: 6174 7465 6d70 7420 746f 2072 756e 2074  attempt to run t
-00049180: 6865 2074 6173 6b20 7761 7320 7b73 656c  he task was {sel
-00049190: 662e 6c61 7374 5f77 6f72 6b65 722e 6164  f.last_worker.ad
-000491a0: 6472 6573 737d 2e20 220a 2020 2020 2020  dress}. ".      
-000491b0: 2020 2020 2020 2249 6e73 7065 6374 696e        "Inspectin
-000491c0: 6720 776f 726b 6572 206c 6f67 7320 6973  g worker logs is
-000491d0: 206f 6674 656e 2061 2067 6f6f 6420 6e65   often a good ne
-000491e0: 7874 2073 7465 7020 746f 2064 6961 676e  xt step to diagn
-000491f0: 6f73 6520 7768 6174 2077 656e 7420 7772  ose what went wr
-00049200: 6f6e 672e 2022 0a20 2020 2020 2020 2020  ong. ".         
-00049210: 2020 2022 466f 7220 6d6f 7265 2069 6e66     "For more inf
-00049220: 6f72 6d61 7469 6f6e 2073 6565 2068 7474  ormation see htt
-00049230: 7073 3a2f 2f64 6973 7472 6962 7574 6564  ps://distributed
-00049240: 2e64 6173 6b2e 6f72 672f 656e 2f73 7461  .dask.org/en/sta
-00049250: 626c 652f 6b69 6c6c 6564 2e68 746d 6c2e  ble/killed.html.
-00049260: 220a 2020 2020 2020 2020 290a 0a0a 636c  ".        )...cl
-00049270: 6173 7320 576f 726b 6572 5374 6174 7573  ass WorkerStatus
-00049280: 506c 7567 696e 2853 6368 6564 756c 6572  Plugin(Scheduler
-00049290: 506c 7567 696e 293a 0a20 2020 2022 2222  Plugin):.    """
-000492a0: 4120 706c 7567 696e 2074 6f20 7368 6172  A plugin to shar
-000492b0: 6520 776f 726b 6572 2073 7461 7475 7320  e worker status 
-000492c0: 7769 7468 2061 2072 656d 6f74 6520 6f62  with a remote ob
-000492d0: 7365 7276 6572 0a0a 2020 2020 5468 6973  server..    This
-000492e0: 2069 7320 7573 6564 2069 6e20 636c 7573   is used in clus
-000492f0: 7465 7220 6d61 6e61 6765 7273 2074 6f20  ter managers to 
-00049300: 6b65 6570 2075 7064 6174 6564 2061 626f  keep updated abo
-00049310: 7574 2074 6865 2073 7461 7475 7320 6f66  ut the status of
-00049320: 2074 6865 2073 6368 6564 756c 6572 2e0a   the scheduler..
-00049330: 2020 2020 2222 220a 0a20 2020 206e 616d      """..    nam
-00049340: 653a 2043 6c61 7373 5661 725b 7374 725d  e: ClassVar[str]
-00049350: 203d 2022 776f 726b 6572 2d73 7461 7475   = "worker-statu
-00049360: 7322 0a20 2020 2062 636f 6d6d 3a20 4261  s".    bcomm: Ba
-00049370: 7463 6865 6453 656e 640a 0a20 2020 2064  tchedSend..    d
-00049380: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00049390: 2c20 7363 6865 6475 6c65 723a 2053 6368  , scheduler: Sch
-000493a0: 6564 756c 6572 2c20 636f 6d6d 3a20 436f  eduler, comm: Co
-000493b0: 6d6d 293a 0a20 2020 2020 2020 2073 656c  mm):.        sel
-000493c0: 662e 6263 6f6d 6d20 3d20 4261 7463 6865  f.bcomm = Batche
-000493d0: 6453 656e 6428 696e 7465 7276 616c 3d22  dSend(interval="
-000493e0: 356d 7322 290a 2020 2020 2020 2020 7365  5ms").        se
-000493f0: 6c66 2e62 636f 6d6d 2e73 7461 7274 2863  lf.bcomm.start(c
-00049400: 6f6d 6d29 0a20 2020 2020 2020 2073 6368  omm).        sch
-00049410: 6564 756c 6572 2e61 6464 5f70 6c75 6769  eduler.add_plugi
-00049420: 6e28 7365 6c66 290a 0a20 2020 2064 6566  n(self)..    def
-00049430: 2061 6464 5f77 6f72 6b65 7228 7365 6c66   add_worker(self
-00049440: 2c20 7363 6865 6475 6c65 723a 2053 6368  , scheduler: Sch
-00049450: 6564 756c 6572 2c20 776f 726b 6572 3a20  eduler, worker: 
-00049460: 7374 7229 202d 3e20 4e6f 6e65 3a0a 2020  str) -> None:.  
-00049470: 2020 2020 2020 6964 656e 7420 3d20 7363        ident = sc
-00049480: 6865 6475 6c65 722e 776f 726b 6572 735b  heduler.workers[
-00049490: 776f 726b 6572 5d2e 6964 656e 7469 7479  worker].identity
-000494a0: 2829 0a20 2020 2020 2020 2064 656c 2069  ().        del i
-000494b0: 6465 6e74 5b22 6d65 7472 6963 7322 5d0a  dent["metrics"].
-000494c0: 2020 2020 2020 2020 6465 6c20 6964 656e          del iden
-000494d0: 745b 226c 6173 745f 7365 656e 225d 0a20  t["last_seen"]. 
-000494e0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-000494f0: 2020 2020 2020 2020 7365 6c66 2e62 636f          self.bco
-00049500: 6d6d 2e73 656e 6428 5b22 6164 6422 2c20  mm.send(["add", 
-00049510: 7b22 776f 726b 6572 7322 3a20 7b77 6f72  {"workers": {wor
-00049520: 6b65 723a 2069 6465 6e74 7d7d 5d29 0a20  ker: ident}}]). 
-00049530: 2020 2020 2020 2065 7863 6570 7420 436f         except Co
-00049540: 6d6d 436c 6f73 6564 4572 726f 723a 0a20  mmClosedError:. 
-00049550: 2020 2020 2020 2020 2020 2073 6368 6564             sched
-00049560: 756c 6572 2e72 656d 6f76 655f 706c 7567  uler.remove_plug
-00049570: 696e 286e 616d 653d 7365 6c66 2e6e 616d  in(name=self.nam
-00049580: 6529 0a0a 2020 2020 6465 6620 7265 6d6f  e)..    def remo
-00049590: 7665 5f77 6f72 6b65 7228 7365 6c66 2c20  ve_worker(self, 
-000495a0: 7363 6865 6475 6c65 723a 2053 6368 6564  scheduler: Sched
-000495b0: 756c 6572 2c20 776f 726b 6572 3a20 7374  uler, worker: st
-000495c0: 7229 202d 3e20 4e6f 6e65 3a0a 2020 2020  r) -> None:.    
-000495d0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-000495e0: 2020 2020 2073 656c 662e 6263 6f6d 6d2e       self.bcomm.
-000495f0: 7365 6e64 285b 2272 656d 6f76 6522 2c20  send(["remove", 
-00049600: 776f 726b 6572 5d29 0a20 2020 2020 2020  worker]).       
-00049610: 2065 7863 6570 7420 436f 6d6d 436c 6f73   except CommClos
-00049620: 6564 4572 726f 723a 0a20 2020 2020 2020  edError:.       
-00049630: 2020 2020 2073 6368 6564 756c 6572 2e72       scheduler.r
-00049640: 656d 6f76 655f 706c 7567 696e 286e 616d  emove_plugin(nam
-00049650: 653d 7365 6c66 2e6e 616d 6529 0a0a 2020  e=self.name)..  
-00049660: 2020 6465 6620 7465 6172 646f 776e 2873    def teardown(s
-00049670: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-00049680: 2020 2020 2020 7365 6c66 2e62 636f 6d6d        self.bcomm
-00049690: 2e63 6c6f 7365 2829 0a0a 0a63 6c61 7373  .close()...class
-000496a0: 2043 6f6c 6c65 6374 5461 736b 4d65 7461   CollectTaskMeta
-000496b0: 4461 7461 506c 7567 696e 2853 6368 6564  DataPlugin(Sched
-000496c0: 756c 6572 506c 7567 696e 293a 0a20 2020  ulerPlugin):.   
-000496d0: 2073 6368 6564 756c 6572 3a20 5363 6865   scheduler: Sche
-000496e0: 6475 6c65 720a 2020 2020 6e61 6d65 3a20  duler.    name: 
-000496f0: 7374 720a 2020 2020 6b65 7973 3a20 7365  str.    keys: se
-00049700: 745b 7374 725d 0a20 2020 206d 6574 6164  t[str].    metad
-00049710: 6174 613a 2064 6963 745b 7374 722c 2041  ata: dict[str, A
-00049720: 6e79 5d0a 2020 2020 7374 6174 653a 2064  ny].    state: d
-00049730: 6963 745b 7374 722c 2073 7472 5d0a 0a20  ict[str, str].. 
-00049740: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00049750: 7365 6c66 2c20 7363 6865 6475 6c65 723a  self, scheduler:
-00049760: 2053 6368 6564 756c 6572 2c20 6e61 6d65   Scheduler, name
-00049770: 3a20 7374 7229 3a0a 2020 2020 2020 2020  : str):.        
-00049780: 7365 6c66 2e73 6368 6564 756c 6572 203d  self.scheduler =
-00049790: 2073 6368 6564 756c 6572 0a20 2020 2020   scheduler.     
-000497a0: 2020 2073 656c 662e 6e61 6d65 203d 206e     self.name = n
-000497b0: 616d 650a 2020 2020 2020 2020 7365 6c66  ame.        self
-000497c0: 2e6b 6579 7320 3d20 7365 7428 290a 2020  .keys = set().  
-000497d0: 2020 2020 2020 7365 6c66 2e6d 6574 6164        self.metad
-000497e0: 6174 6120 3d20 7b7d 0a20 2020 2020 2020  ata = {}.       
-000497f0: 2073 656c 662e 7374 6174 6520 3d20 7b7d   self.state = {}
-00049800: 0a0a 2020 2020 6465 6620 7570 6461 7465  ..    def update
-00049810: 5f67 7261 7068 280a 2020 2020 2020 2020  _graph(.        
-00049820: 7365 6c66 2c0a 2020 2020 2020 2020 7363  self,.        sc
-00049830: 6865 6475 6c65 723a 2053 6368 6564 756c  heduler: Schedul
-00049840: 6572 2c0a 2020 2020 2020 2020 2a2c 0a20  er,.        *,. 
-00049850: 2020 2020 2020 206b 6579 733a 2073 6574         keys: set
-00049860: 5b73 7472 5d2c 0a20 2020 2020 2020 202a  [str],.        *
-00049870: 2a6b 7761 7267 733a 2041 6e79 2c0a 2020  *kwargs: Any,.  
-00049880: 2020 2920 2d3e 204e 6f6e 653a 0a20 2020    ) -> None:.   
-00049890: 2020 2020 2073 656c 662e 6b65 7973 2e75       self.keys.u
-000498a0: 7064 6174 6528 6b65 7973 290a 0a20 2020  pdate(keys)..   
-000498b0: 2064 6566 2074 7261 6e73 6974 696f 6e28   def transition(
-000498c0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-000498d0: 2020 2020 2020 206b 6579 3a20 7374 722c         key: str,
-000498e0: 0a20 2020 2020 2020 2073 7461 7274 3a20  .        start: 
-000498f0: 5461 736b 5374 6174 6553 7461 7465 2c0a  TaskStateState,.
-00049900: 2020 2020 2020 2020 6669 6e69 7368 3a20          finish: 
-00049910: 5461 736b 5374 6174 6553 7461 7465 2c0a  TaskStateState,.
-00049920: 2020 2020 2020 2020 2a61 7267 733a 2041          *args: A
-00049930: 6e79 2c0a 2020 2020 2020 2020 2a2a 6b77  ny,.        **kw
-00049940: 6172 6773 3a20 416e 792c 0a20 2020 2029  args: Any,.    )
-00049950: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00049960: 2020 6966 2066 696e 6973 6820 696e 2028    if finish in (
-00049970: 226d 656d 6f72 7922 2c20 2265 7272 6564  "memory", "erred
-00049980: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-00049990: 7473 203d 2073 656c 662e 7363 6865 6475  ts = self.schedu
-000499a0: 6c65 722e 7461 736b 732e 6765 7428 6b65  ler.tasks.get(ke
-000499b0: 7929 0a20 2020 2020 2020 2020 2020 2069  y).            i
-000499c0: 6620 7473 2069 7320 6e6f 7420 4e6f 6e65  f ts is not None
-000499d0: 2061 6e64 2074 732e 6b65 7920 696e 2073   and ts.key in s
-000499e0: 656c 662e 6b65 7973 3a0a 2020 2020 2020  elf.keys:.      
-000499f0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00049a00: 6574 6164 6174 615b 6b65 795d 203d 2074  etadata[key] = t
-00049a10: 732e 6d65 7461 6461 7461 0a20 2020 2020  s.metadata.     
-00049a20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00049a30: 7374 6174 655b 6b65 795d 203d 2066 696e  state[key] = fin
-00049a40: 6973 680a 2020 2020 2020 2020 2020 2020  ish.            
-00049a50: 2020 2020 7365 6c66 2e6b 6579 732e 6469      self.keys.di
-00049a60: 7363 6172 6428 6b65 7929 0a              scard(key).
+000452e0: 2020 2020 2022 2222 4c6f 6720 616e 2065       """Log an e
+000452f0: 7665 6e74 2075 6e64 6572 2061 2067 6976  vent under a giv
+00045300: 656e 2074 6f70 6963 0a0a 2020 2020 2020  en topic..      
+00045310: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00045320: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+00045330: 2020 2020 2020 2020 746f 7069 6320 3a20          topic : 
+00045340: 7374 722c 206c 6973 745b 7374 725d 0a20  str, list[str]. 
+00045350: 2020 2020 2020 2020 2020 204e 616d 6520             Name 
+00045360: 6f66 2074 6865 2074 6f70 6963 2075 6e64  of the topic und
+00045370: 6572 2077 6869 6368 2074 6f20 6c6f 6720  er which to log 
+00045380: 616e 2065 7665 6e74 2e20 546f 206c 6f67  an event. To log
+00045390: 2074 6865 2073 616d 650a 2020 2020 2020   the same.      
+000453a0: 2020 2020 2020 6576 656e 7420 756e 6465        event unde
+000453b0: 7220 6d75 6c74 6970 6c65 2074 6f70 6963  r multiple topic
+000453c0: 732c 2070 6173 7320 6120 6c69 7374 206f  s, pass a list o
+000453d0: 6620 746f 7069 6320 6e61 6d65 732e 0a20  f topic names.. 
+000453e0: 2020 2020 2020 206d 7367 0a20 2020 2020         msg.     
+000453f0: 2020 2020 2020 2045 7665 6e74 206d 6573         Event mes
+00045400: 7361 6765 2074 6f20 6c6f 672e 204e 6f74  sage to log. Not
+00045410: 6520 7468 6973 206d 7573 7420 6265 206d  e this must be m
+00045420: 7367 7061 636b 2073 6572 6961 6c69 7a61  sgpack serializa
+00045430: 626c 652e 0a0a 2020 2020 2020 2020 5365  ble...        Se
+00045440: 6520 616c 736f 0a20 2020 2020 2020 202d  e also.        -
+00045450: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00045460: 436c 6965 6e74 2e6c 6f67 5f65 7665 6e74  Client.log_event
+00045470: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00045480: 2020 2020 2065 7665 6e74 203d 2028 7469       event = (ti
+00045490: 6d65 2829 2c20 6d73 6729 0a20 2020 2020  me(), msg).     
+000454a0: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
+000454b0: 616e 6365 2874 6f70 6963 2c20 7374 7229  ance(topic, str)
+000454c0: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+000454d0: 7220 7420 696e 2074 6f70 6963 3a0a 2020  r t in topic:.  
+000454e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000454f0: 6c66 2e65 7665 6e74 735b 745d 2e61 7070  lf.events[t].app
+00045500: 656e 6428 6576 656e 7429 0a20 2020 2020  end(event).     
+00045510: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00045520: 6576 656e 745f 636f 756e 7473 5b74 5d20  event_counts[t] 
+00045530: 2b3d 2031 0a20 2020 2020 2020 2020 2020  += 1.           
+00045540: 2020 2020 2073 656c 662e 5f72 6570 6f72       self._repor
+00045550: 745f 6576 656e 7428 742c 2065 7665 6e74  t_event(t, event
+00045560: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00045570: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00045580: 2e65 7665 6e74 735b 746f 7069 635d 2e61  .events[topic].a
+00045590: 7070 656e 6428 6576 656e 7429 0a20 2020  ppend(event).   
+000455a0: 2020 2020 2020 2020 2073 656c 662e 6576           self.ev
+000455b0: 656e 745f 636f 756e 7473 5b74 6f70 6963  ent_counts[topic
+000455c0: 5d20 2b3d 2031 0a20 2020 2020 2020 2020  ] += 1.         
+000455d0: 2020 2073 656c 662e 5f72 6570 6f72 745f     self._report_
+000455e0: 6576 656e 7428 746f 7069 632c 2065 7665  event(topic, eve
+000455f0: 6e74 290a 0a20 2020 2020 2020 2020 2020  nt)..           
+00045600: 2066 6f72 2070 6c75 6769 6e20 696e 206c   for plugin in l
+00045610: 6973 7428 7365 6c66 2e70 6c75 6769 6e73  ist(self.plugins
+00045620: 2e76 616c 7565 7328 2929 3a0a 2020 2020  .values()):.    
+00045630: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+00045640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00045650: 2020 2020 2070 6c75 6769 6e2e 6c6f 675f       plugin.log_
+00045660: 6576 656e 7428 746f 7069 632c 206d 7367  event(topic, msg
+00045670: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00045680: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+00045690: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
+000456a0: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
+000456b0: 6e66 6f28 2250 6c75 6769 6e20 6661 696c  nfo("Plugin fail
+000456c0: 6564 2077 6974 6820 6578 6365 7074 696f  ed with exceptio
+000456d0: 6e22 2c20 6578 635f 696e 666f 3d54 7275  n", exc_info=Tru
+000456e0: 6529 0a0a 2020 2020 6465 6620 5f72 6570  e)..    def _rep
+000456f0: 6f72 745f 6576 656e 7428 7365 6c66 2c20  ort_event(self, 
+00045700: 6e61 6d65 2c20 6576 656e 7429 3a0a 2020  name, event):.  
+00045710: 2020 2020 2020 6d73 6720 3d20 7b0a 2020        msg = {.  
+00045720: 2020 2020 2020 2020 2020 226f 7022 3a20            "op": 
+00045730: 2265 7665 6e74 222c 0a20 2020 2020 2020  "event",.       
+00045740: 2020 2020 2022 746f 7069 6322 3a20 6e61       "topic": na
+00045750: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+00045760: 2265 7665 6e74 223a 2065 7665 6e74 2c0a  "event": event,.
+00045770: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00045780: 2020 636c 6965 6e74 5f6d 7367 7320 3d20    client_msgs = 
+00045790: 7b63 6c69 656e 743a 205b 6d73 675d 2066  {client: [msg] f
+000457a0: 6f72 2063 6c69 656e 7420 696e 2073 656c  or client in sel
+000457b0: 662e 6576 656e 745f 7375 6273 6372 6962  f.event_subscrib
+000457c0: 6572 5b6e 616d 655d 7d0a 2020 2020 2020  er[name]}.      
+000457d0: 2020 7365 6c66 2e73 656e 645f 616c 6c28    self.send_all(
+000457e0: 636c 6965 6e74 5f6d 7367 732c 2077 6f72  client_msgs, wor
+000457f0: 6b65 725f 6d73 6773 3d7b 7d29 0a0a 2020  ker_msgs={})..  
+00045800: 2020 6465 6620 7375 6273 6372 6962 655f    def subscribe_
+00045810: 746f 7069 6328 7365 6c66 2c20 746f 7069  topic(self, topi
+00045820: 632c 2063 6c69 656e 7429 3a0a 2020 2020  c, client):.    
+00045830: 2020 2020 7365 6c66 2e65 7665 6e74 5f73      self.event_s
+00045840: 7562 7363 7269 6265 725b 746f 7069 635d  ubscriber[topic]
+00045850: 2e61 6464 2863 6c69 656e 7429 0a0a 2020  .add(client)..  
+00045860: 2020 6465 6620 756e 7375 6273 6372 6962    def unsubscrib
+00045870: 655f 746f 7069 6328 7365 6c66 2c20 746f  e_topic(self, to
+00045880: 7069 632c 2063 6c69 656e 7429 3a0a 2020  pic, client):.  
+00045890: 2020 2020 2020 7365 6c66 2e65 7665 6e74        self.event
+000458a0: 5f73 7562 7363 7269 6265 725b 746f 7069  _subscriber[topi
+000458b0: 635d 2e64 6973 6361 7264 2863 6c69 656e  c].discard(clien
+000458c0: 7429 0a0a 2020 2020 6465 6620 6765 745f  t)..    def get_
+000458d0: 6576 656e 7473 2873 656c 662c 2074 6f70  events(self, top
+000458e0: 6963 3d4e 6f6e 6529 3a0a 2020 2020 2020  ic=None):.      
+000458f0: 2020 6966 2074 6f70 6963 2069 7320 6e6f    if topic is no
+00045900: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00045910: 2020 2020 7265 7475 726e 2074 7570 6c65      return tuple
+00045920: 2873 656c 662e 6576 656e 7473 5b74 6f70  (self.events[top
+00045930: 6963 5d29 0a20 2020 2020 2020 2065 6c73  ic]).        els
+00045940: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00045950: 6574 7572 6e20 7661 6c6d 6170 2874 7570  eturn valmap(tup
+00045960: 6c65 2c20 7365 6c66 2e65 7665 6e74 7329  le, self.events)
+00045970: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+00045980: 6765 745f 776f 726b 6572 5f6d 6f6e 6974  get_worker_monit
+00045990: 6f72 5f69 6e66 6f28 7365 6c66 2c20 7265  or_info(self, re
+000459a0: 6365 6e74 3d46 616c 7365 2c20 7374 6172  cent=False, star
+000459b0: 7473 3d4e 6f6e 6529 3a0a 2020 2020 2020  ts=None):.      
+000459c0: 2020 6966 2073 7461 7274 7320 6973 204e    if starts is N
+000459d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000459e0: 2073 7461 7274 7320 3d20 7b7d 0a20 2020   starts = {}.   
+000459f0: 2020 2020 2072 6573 756c 7473 203d 2061       results = a
+00045a00: 7761 6974 2061 7379 6e63 696f 2e67 6174  wait asyncio.gat
+00045a10: 6865 7228 0a20 2020 2020 2020 2020 2020  her(.           
+00045a20: 202a 280a 2020 2020 2020 2020 2020 2020   *(.            
+00045a30: 2020 2020 7365 6c66 2e72 7063 2877 292e      self.rpc(w).
+00045a40: 6765 745f 6d6f 6e69 746f 725f 696e 666f  get_monitor_info
+00045a50: 2872 6563 656e 743d 7265 6365 6e74 2c20  (recent=recent, 
+00045a60: 7374 6172 743d 7374 6172 7473 2e67 6574  start=starts.get
+00045a70: 2877 2c20 3029 290a 2020 2020 2020 2020  (w, 0)).        
+00045a80: 2020 2020 2020 2020 666f 7220 7720 696e          for w in
+00045a90: 2073 656c 662e 776f 726b 6572 730a 2020   self.workers.  
+00045aa0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00045ab0: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
+00045ac0: 7475 726e 2064 6963 7428 7a69 7028 7365  turn dict(zip(se
+00045ad0: 6c66 2e77 6f72 6b65 7273 2c20 7265 7375  lf.workers, resu
+00045ae0: 6c74 7329 290a 0a20 2020 2023 2323 2323  lts))..    #####
+00045af0: 2323 2323 2323 0a20 2020 2023 2043 6c65  ######.    # Cle
+00045b00: 616e 7570 2023 0a20 2020 2023 2323 2323  anup #.    #####
+00045b10: 2323 2323 2323 0a0a 2020 2020 6173 796e  ######..    asyn
+00045b20: 6320 6465 6620 6368 6563 6b5f 776f 726b  c def check_work
+00045b30: 6572 5f74 746c 2873 656c 6629 3a0a 2020  er_ttl(self):.  
+00045b40: 2020 2020 2020 6e6f 7720 3d20 7469 6d65        now = time
+00045b50: 2829 0a20 2020 2020 2020 2073 7469 6d75  ().        stimu
+00045b60: 6c75 735f 6964 203d 2066 2263 6865 636b  lus_id = f"check
+00045b70: 2d77 6f72 6b65 722d 7474 6c2d 7b6e 6f77  -worker-ttl-{now
+00045b80: 7d22 0a20 2020 2020 2020 2066 6f72 2077  }".        for w
+00045b90: 7320 696e 2073 656c 662e 776f 726b 6572  s in self.worker
+00045ba0: 732e 7661 6c75 6573 2829 3a0a 2020 2020  s.values():.    
+00045bb0: 2020 2020 2020 2020 6966 2028 7773 2e6c          if (ws.l
+00045bc0: 6173 745f 7365 656e 203c 206e 6f77 202d  ast_seen < now -
+00045bd0: 2073 656c 662e 776f 726b 6572 5f74 746c   self.worker_ttl
+00045be0: 2920 616e 6420 280a 2020 2020 2020 2020  ) and (.        
+00045bf0: 2020 2020 2020 2020 7773 2e6c 6173 745f          ws.last_
+00045c00: 7365 656e 203c 206e 6f77 202d 2031 3020  seen < now - 10 
+00045c10: 2a20 6865 6172 7462 6561 745f 696e 7465  * heartbeat_inte
+00045c20: 7276 616c 286c 656e 2873 656c 662e 776f  rval(len(self.wo
+00045c30: 726b 6572 7329 290a 2020 2020 2020 2020  rkers)).        
+00045c40: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+00045c50: 2020 2020 2020 206c 6f67 6765 722e 7761         logger.wa
+00045c60: 726e 696e 6728 0a20 2020 2020 2020 2020  rning(.         
+00045c70: 2020 2020 2020 2020 2020 2022 576f 726b             "Work
+00045c80: 6572 2066 6169 6c65 6420 746f 2068 6561  er failed to hea
+00045c90: 7274 6265 6174 2077 6974 6869 6e20 2573  rtbeat within %s
+00045ca0: 2073 6563 6f6e 6473 2e20 436c 6f73 696e   seconds. Closin
+00045cb0: 673a 2025 7322 2c0a 2020 2020 2020 2020  g: %s",.        
+00045cc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00045cd0: 2e77 6f72 6b65 725f 7474 6c2c 0a20 2020  .worker_ttl,.   
+00045ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00045cf0: 2077 732c 0a20 2020 2020 2020 2020 2020   ws,.           
+00045d00: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00045d10: 2020 2020 2020 2061 7761 6974 2073 656c         await sel
+00045d20: 662e 7265 6d6f 7665 5f77 6f72 6b65 7228  f.remove_worker(
+00045d30: 6164 6472 6573 733d 7773 2e61 6464 7265  address=ws.addre
+00045d40: 7373 2c20 7374 696d 756c 7573 5f69 643d  ss, stimulus_id=
+00045d50: 7374 696d 756c 7573 5f69 6429 0a0a 2020  stimulus_id)..  
+00045d60: 2020 6465 6620 6368 6563 6b5f 6964 6c65    def check_idle
+00045d70: 2873 656c 6629 202d 3e20 666c 6f61 7420  (self) -> float 
+00045d80: 7c20 4e6f 6e65 3a0a 2020 2020 2020 2020  | None:.        
+00045d90: 6966 2073 656c 662e 7374 6174 7573 2069  if self.status i
+00045da0: 6e20 2853 7461 7475 732e 636c 6f73 696e  n (Status.closin
+00045db0: 672c 2053 7461 7475 732e 636c 6f73 6564  g, Status.closed
+00045dc0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00045dd0: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
+00045de0: 2020 2020 6966 2073 656c 662e 7472 616e      if self.tran
+00045df0: 7369 7469 6f6e 5f63 6f75 6e74 6572 2021  sition_counter !
+00045e00: 3d20 7365 6c66 2e5f 6964 6c65 5f74 7261  = self._idle_tra
+00045e10: 6e73 6974 696f 6e5f 636f 756e 7465 723a  nsition_counter:
+00045e20: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00045e30: 662e 5f69 646c 655f 7472 616e 7369 7469  f._idle_transiti
+00045e40: 6f6e 5f63 6f75 6e74 6572 203d 2073 656c  on_counter = sel
+00045e50: 662e 7472 616e 7369 7469 6f6e 5f63 6f75  f.transition_cou
+00045e60: 6e74 6572 0a20 2020 2020 2020 2020 2020  nter.           
+00045e70: 2073 656c 662e 6964 6c65 5f73 696e 6365   self.idle_since
+00045e80: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00045e90: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+00045ea0: 0a20 2020 2020 2020 2069 6620 280a 2020  .        if (.  
+00045eb0: 2020 2020 2020 2020 2020 7365 6c66 2e71            self.q
+00045ec0: 7565 7565 640a 2020 2020 2020 2020 2020  ueued.          
+00045ed0: 2020 6f72 2073 656c 662e 756e 7275 6e6e    or self.unrunn
+00045ee0: 6162 6c65 0a20 2020 2020 2020 2020 2020  able.           
+00045ef0: 206f 7220 616e 7928 7773 2e70 726f 6365   or any(ws.proce
+00045f00: 7373 696e 6720 666f 7220 7773 2069 6e20  ssing for ws in 
+00045f10: 7365 6c66 2e77 6f72 6b65 7273 2e76 616c  self.workers.val
+00045f20: 7565 7328 2929 0a20 2020 2020 2020 2029  ues()).        )
+00045f30: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00045f40: 6c66 2e69 646c 655f 7369 6e63 6520 3d20  lf.idle_since = 
+00045f50: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+00045f60: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
+00045f70: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
+00045f80: 662e 6964 6c65 5f73 696e 6365 3a0a 2020  f.idle_since:.  
+00045f90: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
+00045fa0: 646c 655f 7369 6e63 6520 3d20 7469 6d65  dle_since = time
+00045fb0: 2829 0a20 2020 2020 2020 2020 2020 2072  ().            r
+00045fc0: 6574 7572 6e20 7365 6c66 2e69 646c 655f  eturn self.idle_
+00045fd0: 7369 6e63 650a 0a20 2020 2020 2020 2069  since..        i
+00045fe0: 6620 7365 6c66 2e6a 7570 7974 6572 3a0a  f self.jupyter:.
+00045ff0: 2020 2020 2020 2020 2020 2020 6c61 7374              last
+00046000: 5f61 6374 6976 6974 7920 3d20 280a 2020  _activity = (.  
+00046010: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00046020: 6c66 2e5f 6a75 7079 7465 725f 7365 7276  lf._jupyter_serv
+00046030: 6572 5f61 7070 6c69 6361 7469 6f6e 2e77  er_application.w
+00046040: 6562 5f61 7070 2e6c 6173 745f 6163 7469  eb_app.last_acti
+00046050: 7669 7479 2829 2e74 696d 6573 7461 6d70  vity().timestamp
+00046060: 2829 0a20 2020 2020 2020 2020 2020 2029  ().            )
+00046070: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00046080: 6c61 7374 5f61 6374 6976 6974 7920 3e20  last_activity > 
+00046090: 7365 6c66 2e69 646c 655f 7369 6e63 653a  self.idle_since:
+000460a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000460b0: 2073 656c 662e 6964 6c65 5f73 696e 6365   self.idle_since
+000460c0: 203d 206c 6173 745f 6163 7469 7669 7479   = last_activity
+000460d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000460e0: 2072 6574 7572 6e20 7365 6c66 2e69 646c   return self.idl
+000460f0: 655f 7369 6e63 650a 0a20 2020 2020 2020  e_since..       
+00046100: 2069 6620 7365 6c66 2e69 646c 655f 7469   if self.idle_ti
+00046110: 6d65 6f75 743a 0a20 2020 2020 2020 2020  meout:.         
+00046120: 2020 2069 6620 7469 6d65 2829 203e 2073     if time() > s
+00046130: 656c 662e 6964 6c65 5f73 696e 6365 202b  elf.idle_since +
+00046140: 2073 656c 662e 6964 6c65 5f74 696d 656f   self.idle_timeo
+00046150: 7574 3a0a 2020 2020 2020 2020 2020 2020  ut:.            
+00046160: 2020 2020 6173 7365 7274 2073 656c 662e      assert self.
+00046170: 6964 6c65 5f73 696e 6365 0a20 2020 2020  idle_since.     
+00046180: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00046190: 722e 696e 666f 280a 2020 2020 2020 2020  r.info(.        
+000461a0: 2020 2020 2020 2020 2020 2020 2253 6368              "Sch
+000461b0: 6564 756c 6572 2063 6c6f 7369 6e67 2061  eduler closing a
+000461c0: 6674 6572 2062 6569 6e67 2069 646c 6520  fter being idle 
+000461d0: 666f 7220 2573 222c 0a20 2020 2020 2020  for %s",.       
+000461e0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+000461f0: 6d61 745f 7469 6d65 2873 656c 662e 6964  mat_time(self.id
+00046200: 6c65 5f74 696d 656f 7574 292c 0a20 2020  le_timeout),.   
+00046210: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00046220: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00046230: 656c 662e 5f6f 6e67 6f69 6e67 5f62 6163  elf._ongoing_bac
+00046240: 6b67 726f 756e 645f 7461 736b 732e 6361  kground_tasks.ca
+00046250: 6c6c 5f73 6f6f 6e28 7365 6c66 2e63 6c6f  ll_soon(self.clo
+00046260: 7365 290a 2020 2020 2020 2020 7265 7475  se).        retu
+00046270: 726e 2073 656c 662e 6964 6c65 5f73 696e  rn self.idle_sin
+00046280: 6365 0a0a 2020 2020 6465 6620 6164 6170  ce..    def adap
+00046290: 7469 7665 5f74 6172 6765 7428 7365 6c66  tive_target(self
+000462a0: 2c20 7461 7267 6574 5f64 7572 6174 696f  , target_duratio
+000462b0: 6e3d 4e6f 6e65 293a 0a20 2020 2020 2020  n=None):.       
+000462c0: 2022 2222 4465 7369 7265 6420 6e75 6d62   """Desired numb
+000462d0: 6572 206f 6620 776f 726b 6572 7320 6261  er of workers ba
+000462e0: 7365 6420 6f6e 2074 6865 2063 7572 7265  sed on the curre
+000462f0: 6e74 2077 6f72 6b6c 6f61 640a 0a20 2020  nt workload..   
+00046300: 2020 2020 2054 6869 7320 6c6f 6f6b 7320       This looks 
+00046310: 6174 2074 6865 2063 7572 7265 6e74 2072  at the current r
+00046320: 756e 6e69 6e67 2074 6173 6b73 2061 6e64  unning tasks and
+00046330: 206d 656d 6f72 7920 7573 652c 2061 6e64   memory use, and
+00046340: 2072 6574 7572 6e73 2061 0a20 2020 2020   returns a.     
+00046350: 2020 206e 756d 6265 7220 6f66 2064 6573     number of des
+00046360: 6972 6564 2077 6f72 6b65 7273 2e20 2054  ired workers.  T
+00046370: 6869 7320 6973 206f 6674 656e 2075 7365  his is often use
+00046380: 6420 6279 2061 6461 7074 6976 6520 7363  d by adaptive sc
+00046390: 6865 6475 6c69 6e67 2e0a 0a20 2020 2020  heduling...     
+000463a0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+000463b0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+000463c0: 0a20 2020 2020 2020 2074 6172 6765 745f  .        target_
+000463d0: 6475 7261 7469 6f6e 203a 2073 7472 0a20  duration : str. 
+000463e0: 2020 2020 2020 2020 2020 2041 2064 6573             A des
+000463f0: 6972 6564 2064 7572 6174 696f 6e20 6f66  ired duration of
+00046400: 2074 696d 6520 666f 7220 636f 6d70 7574   time for comput
+00046410: 6174 696f 6e73 2074 6f20 7461 6b65 2e20  ations to take. 
+00046420: 2054 6869 7320 6166 6665 6374 730a 2020   This affects.  
+00046430: 2020 2020 2020 2020 2020 686f 7720 7261            how ra
+00046440: 7069 646c 7920 7468 6520 7363 6865 6475  pidly the schedu
+00046450: 6c65 7220 7769 6c6c 2061 736b 2074 6f20  ler will ask to 
+00046460: 7363 616c 652e 0a0a 2020 2020 2020 2020  scale...        
+00046470: 5365 6520 416c 736f 0a20 2020 2020 2020  See Also.       
+00046480: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020   --------.      
+00046490: 2020 6469 7374 7269 6275 7465 642e 6465    distributed.de
+000464a0: 706c 6f79 2e41 6461 7074 6976 650a 2020  ploy.Adaptive.  
+000464b0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000464c0: 2020 6966 2074 6172 6765 745f 6475 7261    if target_dura
+000464d0: 7469 6f6e 2069 7320 4e6f 6e65 3a0a 2020  tion is None:.  
+000464e0: 2020 2020 2020 2020 2020 7461 7267 6574            target
+000464f0: 5f64 7572 6174 696f 6e20 3d20 6461 736b  _duration = dask
+00046500: 2e63 6f6e 6669 672e 6765 7428 2264 6973  .config.get("dis
+00046510: 7472 6962 7574 6564 2e61 6461 7074 6976  tributed.adaptiv
+00046520: 652e 7461 7267 6574 2d64 7572 6174 696f  e.target-duratio
+00046530: 6e22 290a 2020 2020 2020 2020 7461 7267  n").        targ
+00046540: 6574 5f64 7572 6174 696f 6e20 3d20 7061  et_duration = pa
+00046550: 7273 655f 7469 6d65 6465 6c74 6128 7461  rse_timedelta(ta
+00046560: 7267 6574 5f64 7572 6174 696f 6e29 0a0a  rget_duration)..
+00046570: 2020 2020 2020 2020 2320 4350 550a 0a20          # CPU.. 
+00046580: 2020 2020 2020 2023 2054 4f44 4f20 636f         # TODO co
+00046590: 6e73 6964 6572 2061 6e79 2075 7365 722d  nsider any user-
+000465a0: 7370 6563 6966 6965 6420 6465 6661 756c  specified defaul
+000465b0: 7420 7461 736b 2064 7572 6174 696f 6e73  t task durations
+000465c0: 2066 6f72 2071 7565 7565 6420 7461 736b   for queued task
+000465d0: 730a 2020 2020 2020 2020 7175 6575 6564  s.        queued
+000465e0: 5f6f 6363 7570 616e 6379 203d 206c 656e  _occupancy = len
+000465f0: 2873 656c 662e 7175 6575 6564 2920 2a20  (self.queued) * 
+00046600: 7365 6c66 2e55 4e4b 4e4f 574e 5f54 4153  self.UNKNOWN_TAS
+00046610: 4b5f 4455 5241 5449 4f4e 0a20 2020 2020  K_DURATION.     
+00046620: 2020 2063 7075 203d 206d 6174 682e 6365     cpu = math.ce
+00046630: 696c 280a 2020 2020 2020 2020 2020 2020  il(.            
+00046640: 2873 656c 662e 746f 7461 6c5f 6f63 6375  (self.total_occu
+00046650: 7061 6e63 7920 2b20 7175 6575 6564 5f6f  pancy + queued_o
+00046660: 6363 7570 616e 6379 2920 2f20 7461 7267  ccupancy) / targ
+00046670: 6574 5f64 7572 6174 696f 6e0a 2020 2020  et_duration.    
+00046680: 2020 2020 2920 2023 2054 4f44 4f3a 2074      )  # TODO: t
+00046690: 6872 6561 6473 2070 6572 2077 6f72 6b65  hreads per worke
+000466a0: 720a 0a20 2020 2020 2020 2023 2041 766f  r..        # Avo
+000466b0: 6964 2061 2066 6577 206c 6f6e 6720 7461  id a few long ta
+000466c0: 736b 7320 6672 6f6d 2061 736b 696e 6720  sks from asking 
+000466d0: 666f 7220 6d61 6e79 2063 6f72 6573 0a20  for many cores. 
+000466e0: 2020 2020 2020 2074 6173 6b73 5f72 6561         tasks_rea
+000466f0: 6479 203d 206c 656e 2873 656c 662e 7175  dy = len(self.qu
+00046700: 6575 6564 290a 2020 2020 2020 2020 666f  eued).        fo
+00046710: 7220 7773 2069 6e20 7365 6c66 2e77 6f72  r ws in self.wor
+00046720: 6b65 7273 2e76 616c 7565 7328 293a 0a20  kers.values():. 
+00046730: 2020 2020 2020 2020 2020 2074 6173 6b73             tasks
+00046740: 5f72 6561 6479 202b 3d20 6c65 6e28 7773  _ready += len(ws
+00046750: 2e70 726f 6365 7373 696e 6729 0a0a 2020  .processing)..  
+00046760: 2020 2020 2020 2020 2020 6966 2074 6173            if tas
+00046770: 6b73 5f72 6561 6479 203e 2063 7075 3a0a  ks_ready > cpu:.
+00046780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00046790: 6272 6561 6b0a 2020 2020 2020 2020 656c  break.        el
+000467a0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000467b0: 6370 7520 3d20 6d69 6e28 7461 736b 735f  cpu = min(tasks_
+000467c0: 7265 6164 792c 2063 7075 290a 0a20 2020  ready, cpu)..   
+000467d0: 2020 2020 2069 6620 2873 656c 662e 756e       if (self.un
+000467e0: 7275 6e6e 6162 6c65 206f 7220 7365 6c66  runnable or self
+000467f0: 2e71 7565 7565 6429 2061 6e64 206e 6f74  .queued) and not
+00046800: 2073 656c 662e 776f 726b 6572 733a 0a20   self.workers:. 
+00046810: 2020 2020 2020 2020 2020 2063 7075 203d             cpu =
+00046820: 206d 6178 2831 2c20 6370 7529 0a0a 2020   max(1, cpu)..  
+00046830: 2020 2020 2020 2320 6164 6420 6d6f 7265        # add more
+00046840: 2077 6f72 6b65 7273 2069 6620 6d6f 7265   workers if more
+00046850: 2074 6861 6e20 3630 2520 6f66 206d 656d   than 60% of mem
+00046860: 6f72 7920 6973 2075 7365 640a 2020 2020  ory is used.    
+00046870: 2020 2020 6c69 6d69 7420 3d20 7375 6d28      limit = sum(
+00046880: 7773 2e6d 656d 6f72 795f 6c69 6d69 7420  ws.memory_limit 
+00046890: 666f 7220 7773 2069 6e20 7365 6c66 2e77  for ws in self.w
+000468a0: 6f72 6b65 7273 2e76 616c 7565 7328 2929  orkers.values())
+000468b0: 0a20 2020 2020 2020 2075 7365 6420 3d20  .        used = 
+000468c0: 7375 6d28 7773 2e6e 6279 7465 7320 666f  sum(ws.nbytes fo
+000468d0: 7220 7773 2069 6e20 7365 6c66 2e77 6f72  r ws in self.wor
+000468e0: 6b65 7273 2e76 616c 7565 7328 2929 0a20  kers.values()). 
+000468f0: 2020 2020 2020 206d 656d 6f72 7920 3d20         memory = 
+00046900: 300a 2020 2020 2020 2020 6966 2075 7365  0.        if use
+00046910: 6420 3e20 302e 3620 2a20 6c69 6d69 7420  d > 0.6 * limit 
+00046920: 616e 6420 6c69 6d69 7420 3e20 303a 0a20  and limit > 0:. 
+00046930: 2020 2020 2020 2020 2020 206d 656d 6f72             memor
+00046940: 7920 3d20 3220 2a20 6c65 6e28 7365 6c66  y = 2 * len(self
+00046950: 2e77 6f72 6b65 7273 290a 0a20 2020 2020  .workers)..     
+00046960: 2020 2074 6172 6765 7420 3d20 6d61 7828     target = max(
+00046970: 6d65 6d6f 7279 2c20 6370 7529 0a20 2020  memory, cpu).   
+00046980: 2020 2020 2069 6620 7461 7267 6574 203e       if target >
+00046990: 3d20 6c65 6e28 7365 6c66 2e77 6f72 6b65  = len(self.worke
+000469a0: 7273 293a 0a20 2020 2020 2020 2020 2020  rs):.           
+000469b0: 2072 6574 7572 6e20 7461 7267 6574 0a20   return target. 
+000469c0: 2020 2020 2020 2065 6c73 653a 2020 2320         else:  # 
+000469d0: 5363 616c 6520 646f 776e 3f0a 2020 2020  Scale down?.    
+000469e0: 2020 2020 2020 2020 746f 5f63 6c6f 7365          to_close
+000469f0: 203d 2073 656c 662e 776f 726b 6572 735f   = self.workers_
+00046a00: 746f 5f63 6c6f 7365 2829 0a20 2020 2020  to_close().     
+00046a10: 2020 2020 2020 2072 6574 7572 6e20 6c65         return le
+00046a20: 6e28 7365 6c66 2e77 6f72 6b65 7273 2920  n(self.workers) 
+00046a30: 2d20 6c65 6e28 746f 5f63 6c6f 7365 290a  - len(to_close).
+00046a40: 0a20 2020 2064 6566 2072 6571 7565 7374  .    def request
+00046a50: 5f61 6371 7569 7265 5f72 6570 6c69 6361  _acquire_replica
+00046a60: 7328 0a20 2020 2020 2020 2073 656c 662c  s(.        self,
+00046a70: 2061 6464 723a 2073 7472 2c20 6b65 7973   addr: str, keys
+00046a80: 3a20 4974 6572 6162 6c65 5b73 7472 5d2c  : Iterable[str],
+00046a90: 202a 2c20 7374 696d 756c 7573 5f69 643a   *, stimulus_id:
+00046aa0: 2073 7472 0a20 2020 2029 202d 3e20 4e6f   str.    ) -> No
+00046ab0: 6e65 3a0a 2020 2020 2020 2020 2222 2241  ne:.        """A
+00046ac0: 7379 6e63 6872 6f6e 6f75 736c 7920 6173  synchronously as
+00046ad0: 6b20 6120 776f 726b 6572 2074 6f20 6163  k a worker to ac
+00046ae0: 7175 6972 6520 6120 7265 706c 6963 6120  quire a replica 
+00046af0: 6f66 2074 6865 206c 6973 7465 6420 6b65  of the listed ke
+00046b00: 7973 2066 726f 6d0a 2020 2020 2020 2020  ys from.        
+00046b10: 6f74 6865 7220 776f 726b 6572 732e 2054  other workers. T
+00046b20: 6869 7320 6973 2061 2066 6972 652d 616e  his is a fire-an
+00046b30: 642d 666f 7267 6574 206f 7065 7261 7469  d-forget operati
+00046b40: 6f6e 2077 6869 6368 206f 6666 6572 7320  on which offers 
+00046b50: 6e6f 2066 6565 6462 6163 6b20 666f 720a  no feedback for.
+00046b60: 2020 2020 2020 2020 7375 6363 6573 7320          success 
+00046b70: 6f72 2066 6169 6c75 7265 2c20 616e 6420  or failure, and 
+00046b80: 6973 2069 6e74 656e 6465 6420 666f 7220  is intended for 
+00046b90: 686f 7573 656b 6565 7069 6e67 2061 6e64  housekeeping and
+00046ba0: 206e 6f74 2066 6f72 2063 6f6d 7075 7461   not for computa
+00046bb0: 7469 6f6e 2e0a 2020 2020 2020 2020 2222  tion..        ""
+00046bc0: 220a 2020 2020 2020 2020 7768 6f5f 6861  ".        who_ha
+00046bd0: 7320 3d20 7b7d 0a20 2020 2020 2020 206e  s = {}.        n
+00046be0: 6279 7465 7320 3d20 7b7d 0a20 2020 2020  bytes = {}.     
+00046bf0: 2020 2066 6f72 206b 6579 2069 6e20 6b65     for key in ke
+00046c00: 7973 3a0a 2020 2020 2020 2020 2020 2020  ys:.            
+00046c10: 7473 203d 2073 656c 662e 7461 736b 735b  ts = self.tasks[
+00046c20: 6b65 795d 0a20 2020 2020 2020 2020 2020  key].           
+00046c30: 2061 7373 6572 7420 7473 2e77 686f 5f68   assert ts.who_h
+00046c40: 6173 0a20 2020 2020 2020 2020 2020 2077  as.            w
+00046c50: 686f 5f68 6173 5b6b 6579 5d20 3d20 5b77  ho_has[key] = [w
+00046c60: 732e 6164 6472 6573 7320 666f 7220 7773  s.address for ws
+00046c70: 2069 6e20 7473 2e77 686f 5f68 6173 5d0a   in ts.who_has].
+00046c80: 2020 2020 2020 2020 2020 2020 6e62 7974              nbyt
+00046c90: 6573 5b6b 6579 5d20 3d20 7473 2e6e 6279  es[key] = ts.nby
+00046ca0: 7465 730a 0a20 2020 2020 2020 2073 656c  tes..        sel
+00046cb0: 662e 7374 7265 616d 5f63 6f6d 6d73 5b61  f.stream_comms[a
+00046cc0: 6464 725d 2e73 656e 6428 0a20 2020 2020  ddr].send(.     
+00046cd0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00046ce0: 2020 2020 2020 2020 2022 6f70 223a 2022           "op": "
+00046cf0: 6163 7175 6972 652d 7265 706c 6963 6173  acquire-replicas
+00046d00: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00046d10: 2020 2022 7768 6f5f 6861 7322 3a20 7768     "who_has": wh
+00046d20: 6f5f 6861 732c 0a20 2020 2020 2020 2020  o_has,.         
+00046d30: 2020 2020 2020 2022 6e62 7974 6573 223a         "nbytes":
+00046d40: 206e 6279 7465 732c 0a20 2020 2020 2020   nbytes,.       
+00046d50: 2020 2020 2020 2020 2022 7374 696d 756c           "stimul
+00046d60: 7573 5f69 6422 3a20 7374 696d 756c 7573  us_id": stimulus
+00046d70: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
+00046d80: 207d 2c0a 2020 2020 2020 2020 290a 0a20   },.        ).. 
+00046d90: 2020 2064 6566 2072 6571 7565 7374 5f72     def request_r
+00046da0: 656d 6f76 655f 7265 706c 6963 6173 280a  emove_replicas(.
+00046db0: 2020 2020 2020 2020 7365 6c66 2c20 6164          self, ad
+00046dc0: 6472 3a20 7374 722c 206b 6579 733a 206c  dr: str, keys: l
+00046dd0: 6973 745b 7374 725d 2c20 2a2c 2073 7469  ist[str], *, sti
+00046de0: 6d75 6c75 735f 6964 3a20 7374 720a 2020  mulus_id: str.  
+00046df0: 2020 2920 2d3e 204e 6f6e 653a 0a20 2020    ) -> None:.   
+00046e00: 2020 2020 2022 2222 4173 796e 6368 726f       """Asynchro
+00046e10: 6e6f 7573 6c79 2061 736b 2061 2077 6f72  nously ask a wor
+00046e20: 6b65 7220 746f 2064 6973 6361 7264 2069  ker to discard i
+00046e30: 7473 2072 6570 6c69 6361 206f 6620 7468  ts replica of th
+00046e40: 6520 6c69 7374 6564 206b 6579 732e 0a20  e listed keys.. 
+00046e50: 2020 2020 2020 2054 6869 7320 6d75 7374         This must
+00046e60: 206e 6576 6572 2062 6520 7573 6564 2074   never be used t
+00046e70: 6f20 6465 7374 726f 7920 7468 6520 6c61  o destroy the la
+00046e80: 7374 2072 6570 6c69 6361 206f 6620 6120  st replica of a 
+00046e90: 6b65 792e 2054 6869 7320 6973 2061 0a20  key. This is a. 
+00046ea0: 2020 2020 2020 2066 6972 652d 616e 642d         fire-and-
+00046eb0: 666f 7267 6574 206f 7065 7261 7469 6f6e  forget operation
+00046ec0: 2c20 696e 7465 6e64 6564 2066 6f72 2068  , intended for h
+00046ed0: 6f75 7365 6b65 6570 696e 6720 616e 6420  ousekeeping and 
+00046ee0: 6e6f 7420 666f 7220 636f 6d70 7574 6174  not for computat
+00046ef0: 696f 6e2e 0a0a 2020 2020 2020 2020 5468  ion...        Th
+00046f00: 6520 7265 706c 6963 6120 6469 7361 7070  e replica disapp
+00046f10: 6561 7273 2069 6d6d 6564 6961 7465 6c79  ears immediately
+00046f20: 2066 726f 6d20 5461 736b 5374 6174 652e   from TaskState.
+00046f30: 7768 6f5f 6861 7320 6f6e 2074 6865 2053  who_has on the S
+00046f40: 6368 6564 756c 6572 2073 6964 653b 0a20  cheduler side;. 
+00046f50: 2020 2020 2020 2069 6620 7468 6520 776f         if the wo
+00046f60: 726b 6572 2072 6566 7573 6573 2074 6f20  rker refuses to 
+00046f70: 6465 6c65 7465 2c20 652e 672e 2062 6563  delete, e.g. bec
+00046f80: 6175 7365 2074 6865 2074 6173 6b20 6973  ause the task is
+00046f90: 2061 2064 6570 656e 6465 6e63 7920 6f66   a dependency of
+00046fa0: 0a20 2020 2020 2020 2061 6e6f 7468 6572  .        another
+00046fb0: 2074 6173 6b20 7275 6e6e 696e 6720 6f6e   task running on
+00046fc0: 2069 742c 2069 7420 7769 6c6c 2028 616c   it, it will (al
+00046fd0: 736f 2061 7379 6e63 6872 6f6e 6f75 736c  so asynchronousl
+00046fe0: 7929 2069 6e66 6f72 6d20 7468 6520 7363  y) inform the sc
+00046ff0: 6865 6475 6c65 720a 2020 2020 2020 2020  heduler.        
+00047000: 746f 2072 652d 6164 6420 6974 7365 6c66  to re-add itself
+00047010: 2074 6f20 7768 6f5f 6861 732e 2049 6620   to who_has. If 
+00047020: 7468 6520 776f 726b 6572 2061 6772 6565  the worker agree
+00047030: 7320 746f 2064 6973 6361 7264 2074 6865  s to discard the
+00047040: 2074 6173 6b2c 2074 6865 7265 2069 730a   task, there is.
+00047050: 2020 2020 2020 2020 6e6f 2066 6565 6462          no feedb
+00047060: 6163 6b2e 0a20 2020 2020 2020 2022 2222  ack..        """
+00047070: 0a20 2020 2020 2020 2077 7320 3d20 7365  .        ws = se
+00047080: 6c66 2e77 6f72 6b65 7273 5b61 6464 725d  lf.workers[addr]
+00047090: 0a0a 2020 2020 2020 2020 2320 5468 6520  ..        # The 
+000470a0: 7363 6865 6475 6c65 7220 696d 6d65 6469  scheduler immedi
+000470b0: 6174 656c 7920 666f 7267 6574 7320 6162  ately forgets ab
+000470c0: 6f75 7420 7468 6520 7265 706c 6963 6120  out the replica 
+000470d0: 616e 6420 7375 6767 6573 7473 2074 6865  and suggests the
+000470e0: 2077 6f72 6b65 7220 746f 0a20 2020 2020   worker to.     
+000470f0: 2020 2023 2064 726f 7020 6974 2e20 5468     # drop it. Th
+00047100: 6520 776f 726b 6572 206d 6179 2072 6566  e worker may ref
+00047110: 7573 652c 2061 7420 7768 6963 6820 706f  use, at which po
+00047120: 696e 7420 6974 2077 696c 6c20 7365 6e64  int it will send
+00047130: 2062 6163 6b20 616e 2061 6464 2d6b 6579   back an add-key
+00047140: 730a 2020 2020 2020 2020 2320 6d65 7373  s.        # mess
+00047150: 6167 6520 746f 2072 6569 6e73 7461 7465  age to reinstate
+00047160: 2069 742e 0a20 2020 2020 2020 2066 6f72   it..        for
+00047170: 206b 6579 2069 6e20 6b65 7973 3a0a 2020   key in keys:.  
+00047180: 2020 2020 2020 2020 2020 7473 203d 2073            ts = s
+00047190: 656c 662e 7461 736b 735b 6b65 795d 0a20  elf.tasks[key]. 
+000471a0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+000471b0: 6c66 2e76 616c 6964 6174 653a 0a20 2020  lf.validate:.   
+000471c0: 2020 2020 2020 2020 2020 2020 2023 2044               # D
+000471d0: 6f20 6e6f 7420 6465 7374 726f 7920 7468  o not destroy th
+000471e0: 6520 6c61 7374 2063 6f70 790a 2020 2020  e last copy.    
+000471f0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+00047200: 7274 206c 656e 2874 732e 7768 6f5f 6861  rt len(ts.who_ha
+00047210: 7329 203e 2031 0a20 2020 2020 2020 2020  s) > 1.         
+00047220: 2020 2073 656c 662e 7265 6d6f 7665 5f72     self.remove_r
+00047230: 6570 6c69 6361 2874 732c 2077 7329 0a0a  eplica(ts, ws)..
+00047240: 2020 2020 2020 2020 7365 6c66 2e73 7472          self.str
+00047250: 6561 6d5f 636f 6d6d 735b 6164 6472 5d2e  eam_comms[addr].
+00047260: 7365 6e64 280a 2020 2020 2020 2020 2020  send(.          
+00047270: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00047280: 2020 2020 226f 7022 3a20 2272 656d 6f76      "op": "remov
+00047290: 652d 7265 706c 6963 6173 222c 0a20 2020  e-replicas",.   
+000472a0: 2020 2020 2020 2020 2020 2020 2022 6b65               "ke
+000472b0: 7973 223a 206b 6579 732c 0a20 2020 2020  ys": keys,.     
+000472c0: 2020 2020 2020 2020 2020 2022 7374 696d             "stim
+000472d0: 756c 7573 5f69 6422 3a20 7374 696d 756c  ulus_id": stimul
+000472e0: 7573 5f69 642c 0a20 2020 2020 2020 2020  us_id,.         
+000472f0: 2020 207d 0a20 2020 2020 2020 2029 0a0a     }.        )..
+00047300: 0a64 6566 205f 7461 736b 5f74 6f5f 7265  .def _task_to_re
+00047310: 706f 7274 5f6d 7367 2874 733a 2054 6173  port_msg(ts: Tas
+00047320: 6b53 7461 7465 2920 2d3e 2064 6963 745b  kState) -> dict[
+00047330: 7374 722c 2041 6e79 5d20 7c20 4e6f 6e65  str, Any] | None
+00047340: 3a0a 2020 2020 6966 2074 732e 7374 6174  :.    if ts.stat
+00047350: 6520 3d3d 2022 666f 7267 6f74 7465 6e22  e == "forgotten"
+00047360: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00047370: 207b 226f 7022 3a20 2263 616e 6365 6c6c   {"op": "cancell
+00047380: 6564 2d6b 6579 7322 2c20 226b 6579 7322  ed-keys", "keys"
+00047390: 3a20 5b74 732e 6b65 795d 7d0a 2020 2020  : [ts.key]}.    
+000473a0: 656c 6966 2074 732e 7374 6174 6520 3d3d  elif ts.state ==
+000473b0: 2022 6d65 6d6f 7279 223a 0a20 2020 2020   "memory":.     
+000473c0: 2020 2072 6574 7572 6e20 7b22 6f70 223a     return {"op":
+000473d0: 2022 6b65 792d 696e 2d6d 656d 6f72 7922   "key-in-memory"
+000473e0: 2c20 226b 6579 223a 2074 732e 6b65 797d  , "key": ts.key}
+000473f0: 0a20 2020 2065 6c69 6620 7473 2e73 7461  .    elif ts.sta
+00047400: 7465 203d 3d20 2265 7272 6564 223a 0a20  te == "erred":. 
+00047410: 2020 2020 2020 2066 6169 6c69 6e67 5f74         failing_t
+00047420: 7320 3d20 7473 2e65 7863 6570 7469 6f6e  s = ts.exception
+00047430: 5f62 6c61 6d65 0a20 2020 2020 2020 2061  _blame.        a
+00047440: 7373 6572 7420 6661 696c 696e 675f 7473  ssert failing_ts
+00047450: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00047460: 7b0a 2020 2020 2020 2020 2020 2020 226f  {.            "o
+00047470: 7022 3a20 2274 6173 6b2d 6572 7265 6422  p": "task-erred"
+00047480: 2c0a 2020 2020 2020 2020 2020 2020 226b  ,.            "k
+00047490: 6579 223a 2074 732e 6b65 792c 0a20 2020  ey": ts.key,.   
+000474a0: 2020 2020 2020 2020 2022 6578 6365 7074           "except
+000474b0: 696f 6e22 3a20 6661 696c 696e 675f 7473  ion": failing_ts
+000474c0: 2e65 7863 6570 7469 6f6e 2c0a 2020 2020  .exception,.    
+000474d0: 2020 2020 2020 2020 2274 7261 6365 6261          "traceba
+000474e0: 636b 223a 2066 6169 6c69 6e67 5f74 732e  ck": failing_ts.
+000474f0: 7472 6163 6562 6163 6b2c 0a20 2020 2020  traceback,.     
+00047500: 2020 207d 0a20 2020 2065 6c73 653a 0a20     }.    else:. 
+00047510: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+00047520: 6e65 0a0a 0a64 6566 205f 7461 736b 5f74  ne...def _task_t
+00047530: 6f5f 636c 6965 6e74 5f6d 7367 7328 7473  o_client_msgs(ts
+00047540: 3a20 5461 736b 5374 6174 6529 202d 3e20  : TaskState) -> 
+00047550: 6469 6374 5b73 7472 2c20 6c69 7374 5b64  dict[str, list[d
+00047560: 6963 745b 7374 722c 2041 6e79 5d5d 5d3a  ict[str, Any]]]:
+00047570: 0a20 2020 2069 6620 7473 2e77 686f 5f77  .    if ts.who_w
+00047580: 616e 7473 3a0a 2020 2020 2020 2020 7265  ants:.        re
+00047590: 706f 7274 5f6d 7367 203d 205f 7461 736b  port_msg = _task
+000475a0: 5f74 6f5f 7265 706f 7274 5f6d 7367 2874  _to_report_msg(t
+000475b0: 7329 0a20 2020 2020 2020 2069 6620 7265  s).        if re
+000475c0: 706f 7274 5f6d 7367 2069 7320 6e6f 7420  port_msg is not 
+000475d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000475e0: 2020 7265 7475 726e 207b 6373 2e63 6c69    return {cs.cli
+000475f0: 656e 745f 6b65 793a 205b 7265 706f 7274  ent_key: [report
+00047600: 5f6d 7367 5d20 666f 7220 6373 2069 6e20  _msg] for cs in 
+00047610: 7473 2e77 686f 5f77 616e 7473 7d0a 2020  ts.who_wants}.  
+00047620: 2020 7265 7475 726e 207b 7d0a 0a0a 6465    return {}...de
+00047630: 6620 6465 6369 6465 5f77 6f72 6b65 7228  f decide_worker(
+00047640: 0a20 2020 2074 733a 2054 6173 6b53 7461  .    ts: TaskSta
+00047650: 7465 2c0a 2020 2020 616c 6c5f 776f 726b  te,.    all_work
+00047660: 6572 733a 2049 7465 7261 626c 655b 576f  ers: Iterable[Wo
+00047670: 726b 6572 5374 6174 655d 2c0a 2020 2020  rkerState],.    
+00047680: 7661 6c69 645f 776f 726b 6572 733a 2073  valid_workers: s
+00047690: 6574 5b57 6f72 6b65 7253 7461 7465 5d20  et[WorkerState] 
+000476a0: 7c20 4e6f 6e65 2c0a 2020 2020 6f62 6a65  | None,.    obje
+000476b0: 6374 6976 653a 2043 616c 6c61 626c 655b  ctive: Callable[
+000476c0: 5b57 6f72 6b65 7253 7461 7465 5d2c 2041  [WorkerState], A
+000476d0: 6e79 5d2c 0a29 202d 3e20 576f 726b 6572  ny],.) -> Worker
+000476e0: 5374 6174 6520 7c20 4e6f 6e65 3a0a 2020  State | None:.  
+000476f0: 2020 2222 220a 2020 2020 4465 6369 6465    """.    Decide
+00047700: 2077 6869 6368 2077 6f72 6b65 7220 7368   which worker sh
+00047710: 6f75 6c64 2074 616b 6520 7461 736b 202a  ould take task *
+00047720: 7473 2a2e 0a0a 2020 2020 5765 2063 686f  ts*...    We cho
+00047730: 6f73 6520 7468 6520 776f 726b 6572 2074  ose the worker t
+00047740: 6861 7420 6861 7320 7468 6520 6461 7461  hat has the data
+00047750: 206f 6e20 7768 6963 6820 2a74 732a 2064   on which *ts* d
+00047760: 6570 656e 6473 2e0a 0a20 2020 2049 6620  epends...    If 
+00047770: 7365 7665 7261 6c20 776f 726b 6572 7320  several workers 
+00047780: 6861 7665 2064 6570 656e 6465 6e63 6965  have dependencie
+00047790: 7320 7468 656e 2077 6520 6368 6f6f 7365  s then we choose
+000477a0: 2074 6865 206c 6573 732d 6275 7379 2077   the less-busy w
+000477b0: 6f72 6b65 722e 0a0a 2020 2020 4f70 7469  orker...    Opti
+000477c0: 6f6e 616c 6c79 2070 726f 7669 6465 202a  onally provide *
+000477d0: 7661 6c69 645f 776f 726b 6572 732a 206f  valid_workers* o
+000477e0: 6620 7768 6572 6520 6a6f 6273 2061 7265  f where jobs are
+000477f0: 2061 6c6c 6f77 6564 2074 6f20 6f63 6375   allowed to occu
+00047800: 720a 2020 2020 2869 6620 616c 6c20 776f  r.    (if all wo
+00047810: 726b 6572 7320 6172 6520 616c 6c6f 7765  rkers are allowe
+00047820: 6420 746f 2074 616b 6520 7468 6520 7461  d to take the ta
+00047830: 736b 2c20 7061 7373 204e 6f6e 6520 696e  sk, pass None in
+00047840: 7374 6561 6429 2e0a 0a20 2020 2049 6620  stead)...    If 
+00047850: 7468 6520 7461 736b 2072 6571 7569 7265  the task require
+00047860: 7320 6461 7461 2063 6f6d 6d75 6e69 6361  s data communica
+00047870: 7469 6f6e 2062 6563 6175 7365 206e 6f20  tion because no 
+00047880: 656c 6967 6962 6c65 2077 6f72 6b65 7220  eligible worker 
+00047890: 6861 730a 2020 2020 616c 6c20 7468 6520  has.    all the 
+000478a0: 6465 7065 6e64 656e 6369 6573 2061 6c72  dependencies alr
+000478b0: 6561 6479 2c20 7468 656e 2077 6520 6368  eady, then we ch
+000478c0: 6f6f 7365 2074 6f20 6d69 6e69 6d69 7a65  oose to minimize
+000478d0: 2074 6865 206e 756d 6265 720a 2020 2020   the number.    
+000478e0: 6f66 2062 7974 6573 2073 656e 7420 6265  of bytes sent be
+000478f0: 7477 6565 6e20 776f 726b 6572 732e 2020  tween workers.  
+00047900: 5468 6973 2069 7320 6465 7465 726d 696e  This is determin
+00047910: 6564 2062 7920 6361 6c6c 696e 6720 7468  ed by calling th
+00047920: 650a 2020 2020 2a6f 626a 6563 7469 7665  e.    *objective
+00047930: 2a20 6675 6e63 7469 6f6e 2e0a 2020 2020  * function..    
+00047940: 2222 220a 2020 2020 6173 7365 7274 2061  """.    assert a
+00047950: 6c6c 2864 7473 2e77 686f 5f68 6173 2066  ll(dts.who_has f
+00047960: 6f72 2064 7473 2069 6e20 7473 2e64 6570  or dts in ts.dep
+00047970: 656e 6465 6e63 6965 7329 0a20 2020 2069  endencies).    i
+00047980: 6620 7473 2e61 6374 6f72 3a0a 2020 2020  f ts.actor:.    
+00047990: 2020 2020 6361 6e64 6964 6174 6573 203d      candidates =
+000479a0: 2073 6574 2861 6c6c 5f77 6f72 6b65 7273   set(all_workers
+000479b0: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
+000479c0: 2020 2020 6361 6e64 6964 6174 6573 203d      candidates =
+000479d0: 207b 7777 7320 666f 7220 6474 7320 696e   {wws for dts in
+000479e0: 2074 732e 6465 7065 6e64 656e 6369 6573   ts.dependencies
+000479f0: 2066 6f72 2077 7773 2069 6e20 6474 732e   for wws in dts.
+00047a00: 7768 6f5f 6861 737d 0a20 2020 2069 6620  who_has}.    if 
+00047a10: 7661 6c69 645f 776f 726b 6572 7320 6973  valid_workers is
+00047a20: 204e 6f6e 653a 0a20 2020 2020 2020 2069   None:.        i
+00047a30: 6620 6e6f 7420 6361 6e64 6964 6174 6573  f not candidates
+00047a40: 3a0a 2020 2020 2020 2020 2020 2020 6361  :.            ca
+00047a50: 6e64 6964 6174 6573 203d 2073 6574 2861  ndidates = set(a
+00047a60: 6c6c 5f77 6f72 6b65 7273 290a 2020 2020  ll_workers).    
+00047a70: 656c 7365 3a0a 2020 2020 2020 2020 6361  else:.        ca
+00047a80: 6e64 6964 6174 6573 2026 3d20 7661 6c69  ndidates &= vali
+00047a90: 645f 776f 726b 6572 730a 2020 2020 2020  d_workers.      
+00047aa0: 2020 6966 206e 6f74 2063 616e 6469 6461    if not candida
+00047ab0: 7465 733a 0a20 2020 2020 2020 2020 2020  tes:.           
+00047ac0: 2063 616e 6469 6461 7465 7320 3d20 7661   candidates = va
+00047ad0: 6c69 645f 776f 726b 6572 730a 2020 2020  lid_workers.    
+00047ae0: 2020 2020 2020 2020 6966 206e 6f74 2063          if not c
+00047af0: 616e 6469 6461 7465 733a 0a20 2020 2020  andidates:.     
+00047b00: 2020 2020 2020 2020 2020 2069 6620 7473             if ts
+00047b10: 2e6c 6f6f 7365 5f72 6573 7472 6963 7469  .loose_restricti
+00047b20: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
+00047b30: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00047b40: 6465 6369 6465 5f77 6f72 6b65 7228 7473  decide_worker(ts
+00047b50: 2c20 616c 6c5f 776f 726b 6572 732c 204e  , all_workers, N
+00047b60: 6f6e 652c 206f 626a 6563 7469 7665 290a  one, objective).
+00047b70: 0a20 2020 2069 6620 6e6f 7420 6361 6e64  .    if not cand
+00047b80: 6964 6174 6573 3a0a 2020 2020 2020 2020  idates:.        
+00047b90: 7265 7475 726e 204e 6f6e 650a 2020 2020  return None.    
+00047ba0: 656c 6966 206c 656e 2863 616e 6469 6461  elif len(candida
+00047bb0: 7465 7329 203d 3d20 313a 0a20 2020 2020  tes) == 1:.     
+00047bc0: 2020 2072 6574 7572 6e20 6e65 7874 2869     return next(i
+00047bd0: 7465 7228 6361 6e64 6964 6174 6573 2929  ter(candidates))
+00047be0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00047bf0: 2020 2072 6574 7572 6e20 6d69 6e28 6361     return min(ca
+00047c00: 6e64 6964 6174 6573 2c20 6b65 793d 6f62  ndidates, key=ob
+00047c10: 6a65 6374 6976 6529 0a0a 0a64 6566 2076  jective)...def v
+00047c20: 616c 6964 6174 655f 7461 736b 5f73 7461  alidate_task_sta
+00047c30: 7465 2874 733a 2054 6173 6b53 7461 7465  te(ts: TaskState
+00047c40: 2920 2d3e 204e 6f6e 653a 0a20 2020 2022  ) -> None:.    "
+00047c50: 2222 5661 6c69 6461 7465 2074 6865 2067  ""Validate the g
+00047c60: 6976 656e 2054 6173 6b53 7461 7465 2222  iven TaskState""
+00047c70: 220a 2020 2020 6173 7365 7274 2074 732e  ".    assert ts.
+00047c80: 7374 6174 6520 696e 2041 4c4c 5f54 4153  state in ALL_TAS
+00047c90: 4b5f 5354 4154 4553 2c20 7473 0a0a 2020  K_STATES, ts..  
+00047ca0: 2020 6966 2074 732e 7761 6974 696e 675f    if ts.waiting_
+00047cb0: 6f6e 3a0a 2020 2020 2020 2020 6173 7365  on:.        asse
+00047cc0: 7274 2074 732e 7761 6974 696e 675f 6f6e  rt ts.waiting_on
+00047cd0: 2e69 7373 7562 7365 7428 7473 2e64 6570  .issubset(ts.dep
+00047ce0: 656e 6465 6e63 6965 7329 2c20 280a 2020  endencies), (.  
+00047cf0: 2020 2020 2020 2020 2020 2277 6169 7469            "waiti
+00047d00: 6e67 206e 6f74 2073 7562 7365 7420 6f66  ng not subset of
+00047d10: 2064 6570 656e 6465 6e63 6965 7322 2c0a   dependencies",.
+00047d20: 2020 2020 2020 2020 2020 2020 7374 7228              str(
+00047d30: 7473 2e77 6169 7469 6e67 5f6f 6e29 2c0a  ts.waiting_on),.
+00047d40: 2020 2020 2020 2020 2020 2020 7374 7228              str(
+00047d50: 7473 2e64 6570 656e 6465 6e63 6965 7329  ts.dependencies)
+00047d60: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+00047d70: 6966 2074 732e 7761 6974 6572 733a 0a20  if ts.waiters:. 
+00047d80: 2020 2020 2020 2061 7373 6572 7420 7473         assert ts
+00047d90: 2e77 6169 7465 7273 2e69 7373 7562 7365  .waiters.issubse
+00047da0: 7428 7473 2e64 6570 656e 6465 6e74 7329  t(ts.dependents)
+00047db0: 2c20 280a 2020 2020 2020 2020 2020 2020  , (.            
+00047dc0: 2277 6169 7465 7273 206e 6f74 2073 7562  "waiters not sub
+00047dd0: 7365 7420 6f66 2064 6570 656e 6465 6e74  set of dependent
+00047de0: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+00047df0: 7374 7228 7473 2e77 6169 7465 7273 292c  str(ts.waiters),
+00047e00: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+00047e10: 2874 732e 6465 7065 6e64 656e 7473 292c  (ts.dependents),
+00047e20: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00047e30: 666f 7220 6474 7320 696e 2074 732e 7761  for dts in ts.wa
+00047e40: 6974 696e 675f 6f6e 3a0a 2020 2020 2020  iting_on:.      
+00047e50: 2020 6173 7365 7274 206e 6f74 2064 7473    assert not dts
+00047e60: 2e77 686f 5f68 6173 2c20 2822 7761 6974  .who_has, ("wait
+00047e70: 696e 6720 6f6e 2069 6e2d 6d65 6d6f 7279  ing on in-memory
+00047e80: 2064 6570 222c 2073 7472 2874 7329 2c20   dep", str(ts), 
+00047e90: 7374 7228 6474 7329 290a 2020 2020 2020  str(dts)).      
+00047ea0: 2020 6173 7365 7274 2064 7473 2e73 7461    assert dts.sta
+00047eb0: 7465 2021 3d20 2272 656c 6561 7365 6422  te != "released"
+00047ec0: 2c20 2822 7761 6974 696e 6720 6f6e 2072  , ("waiting on r
+00047ed0: 656c 6561 7365 6420 6465 7022 2c20 7374  eleased dep", st
+00047ee0: 7228 7473 292c 2073 7472 2864 7473 2929  r(ts), str(dts))
+00047ef0: 0a20 2020 2066 6f72 2064 7473 2069 6e20  .    for dts in 
+00047f00: 7473 2e64 6570 656e 6465 6e63 6965 733a  ts.dependencies:
+00047f10: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00047f20: 7473 2069 6e20 6474 732e 6465 7065 6e64  ts in dts.depend
+00047f30: 656e 7473 2c20 280a 2020 2020 2020 2020  ents, (.        
+00047f40: 2020 2020 226e 6f74 2069 6e20 6465 7065      "not in depe
+00047f50: 6e64 656e 6379 2773 2064 6570 656e 6465  ndency's depende
+00047f60: 6e74 7322 2c0a 2020 2020 2020 2020 2020  nts",.          
+00047f70: 2020 7374 7228 7473 292c 0a20 2020 2020    str(ts),.     
+00047f80: 2020 2020 2020 2073 7472 2864 7473 292c         str(dts),
+00047f90: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+00047fa0: 2864 7473 2e64 6570 656e 6465 6e74 7329  (dts.dependents)
+00047fb0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+00047fc0: 2020 2020 6966 2074 732e 7374 6174 6520      if ts.state 
+00047fd0: 696e 2028 2277 6169 7469 6e67 222c 2022  in ("waiting", "
+00047fe0: 7175 6575 6564 222c 2022 7072 6f63 6573  queued", "proces
+00047ff0: 7369 6e67 222c 2022 6e6f 2d77 6f72 6b65  sing", "no-worke
+00048000: 7222 293a 0a20 2020 2020 2020 2020 2020  r"):.           
+00048010: 2061 7373 6572 7420 6474 7320 696e 2074   assert dts in t
+00048020: 732e 7761 6974 696e 675f 6f6e 206f 7220  s.waiting_on or 
+00048030: 6474 732e 7768 6f5f 6861 732c 2028 0a20  dts.who_has, (. 
+00048040: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00048050: 6465 7020 6d69 7373 696e 6722 2c0a 2020  dep missing",.  
+00048060: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00048070: 7228 7473 292c 0a20 2020 2020 2020 2020  r(ts),.         
+00048080: 2020 2020 2020 2073 7472 2864 7473 292c         str(dts),
+00048090: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+000480a0: 2020 2020 2020 2061 7373 6572 7420 6474         assert dt
+000480b0: 732e 7374 6174 6520 213d 2022 666f 7267  s.state != "forg
+000480c0: 6f74 7465 6e22 0a0a 2020 2020 666f 7220  otten"..    for 
+000480d0: 6474 7320 696e 2074 732e 7761 6974 6572  dts in ts.waiter
+000480e0: 733a 0a20 2020 2020 2020 2061 7373 6572  s:.        asser
+000480f0: 7420 6474 732e 7374 6174 6520 696e 2028  t dts.state in (
+00048100: 2277 6169 7469 6e67 222c 2022 7175 6575  "waiting", "queu
+00048110: 6564 222c 2022 7072 6f63 6573 7369 6e67  ed", "processing
+00048120: 222c 2022 6e6f 2d77 6f72 6b65 7222 292c  ", "no-worker"),
+00048130: 2028 0a20 2020 2020 2020 2020 2020 2022   (.            "
+00048140: 7761 6974 6572 206e 6f74 2069 6e20 706c  waiter not in pl
+00048150: 6179 222c 0a20 2020 2020 2020 2020 2020  ay",.           
+00048160: 2073 7472 2874 7329 2c0a 2020 2020 2020   str(ts),.      
+00048170: 2020 2020 2020 7374 7228 6474 7329 2c0a        str(dts),.
+00048180: 2020 2020 2020 2020 290a 2020 2020 666f          ).    fo
+00048190: 7220 6474 7320 696e 2074 732e 6465 7065  r dts in ts.depe
+000481a0: 6e64 656e 7473 3a0a 2020 2020 2020 2020  ndents:.        
+000481b0: 6173 7365 7274 2074 7320 696e 2064 7473  assert ts in dts
+000481c0: 2e64 6570 656e 6465 6e63 6965 732c 2028  .dependencies, (
+000481d0: 0a20 2020 2020 2020 2020 2020 2022 6e6f  .            "no
+000481e0: 7420 696e 2064 6570 656e 6465 6e74 2773  t in dependent's
+000481f0: 2064 6570 656e 6465 6e63 6965 7322 2c0a   dependencies",.
+00048200: 2020 2020 2020 2020 2020 2020 7374 7228              str(
+00048210: 7473 292c 0a20 2020 2020 2020 2020 2020  ts),.           
+00048220: 2073 7472 2864 7473 292c 0a20 2020 2020   str(dts),.     
+00048230: 2020 2020 2020 2073 7472 2864 7473 2e64         str(dts.d
+00048240: 6570 656e 6465 6e63 6965 7329 2c0a 2020  ependencies),.  
+00048250: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00048260: 6173 7365 7274 2064 7473 2e73 7461 7465  assert dts.state
+00048270: 2021 3d20 2266 6f72 676f 7474 656e 220a   != "forgotten".
+00048280: 0a20 2020 2061 7373 6572 7420 2874 732e  .    assert (ts.
+00048290: 7072 6f63 6573 7369 6e67 5f6f 6e20 6973  processing_on is
+000482a0: 206e 6f74 204e 6f6e 6529 203d 3d20 2874   not None) == (t
+000482b0: 732e 7374 6174 6520 3d3d 2022 7072 6f63  s.state == "proc
+000482c0: 6573 7369 6e67 2229 0a20 2020 2061 7373  essing").    ass
+000482d0: 6572 7420 626f 6f6c 2874 732e 7768 6f5f  ert bool(ts.who_
+000482e0: 6861 7329 203d 3d20 2874 732e 7374 6174  has) == (ts.stat
+000482f0: 6520 3d3d 2022 6d65 6d6f 7279 2229 2c20  e == "memory"), 
+00048300: 2874 732c 2074 732e 7768 6f5f 6861 732c  (ts, ts.who_has,
+00048310: 2074 732e 7374 6174 6529 0a0a 2020 2020   ts.state)..    
+00048320: 6966 2074 732e 7374 6174 6520 3d3d 2022  if ts.state == "
+00048330: 7175 6575 6564 223a 0a20 2020 2020 2020  queued":.       
+00048340: 2061 7373 6572 7420 6e6f 7420 7473 2e70   assert not ts.p
+00048350: 726f 6365 7373 696e 675f 6f6e 0a20 2020  rocessing_on.   
+00048360: 2020 2020 2061 7373 6572 7420 6e6f 7420       assert not 
+00048370: 7473 2e77 686f 5f68 6173 0a20 2020 2020  ts.who_has.     
+00048380: 2020 2061 7373 6572 7420 616c 6c28 6474     assert all(dt
+00048390: 732e 7768 6f5f 6861 7320 666f 7220 6474  s.who_has for dt
+000483a0: 7320 696e 2074 732e 6465 7065 6e64 656e  s in ts.dependen
+000483b0: 6369 6573 292c 2028 0a20 2020 2020 2020  cies), (.       
+000483c0: 2020 2020 2022 7461 736b 2071 7565 7565       "task queue
+000483d0: 6420 7769 7468 6f75 7420 616c 6c20 6465  d without all de
+000483e0: 7073 222c 0a20 2020 2020 2020 2020 2020  ps",.           
+000483f0: 2073 7472 2874 7329 2c0a 2020 2020 2020   str(ts),.      
+00048400: 2020 2020 2020 7374 7228 7473 2e64 6570        str(ts.dep
+00048410: 656e 6465 6e63 6965 7329 2c0a 2020 2020  endencies),.    
+00048420: 2020 2020 290a 0a20 2020 2069 6620 7473      )..    if ts
+00048430: 2e73 7461 7465 203d 3d20 2270 726f 6365  .state == "proce
+00048440: 7373 696e 6722 3a0a 2020 2020 2020 2020  ssing":.        
+00048450: 6173 7365 7274 2061 6c6c 2864 7473 2e77  assert all(dts.w
+00048460: 686f 5f68 6173 2066 6f72 2064 7473 2069  ho_has for dts i
+00048470: 6e20 7473 2e64 6570 656e 6465 6e63 6965  n ts.dependencie
+00048480: 7329 2c20 280a 2020 2020 2020 2020 2020  s), (.          
+00048490: 2020 2274 6173 6b20 7072 6f63 6573 7369    "task processi
+000484a0: 6e67 2077 6974 686f 7574 2061 6c6c 2064  ng without all d
+000484b0: 6570 7322 2c0a 2020 2020 2020 2020 2020  eps",.          
+000484c0: 2020 7374 7228 7473 292c 0a20 2020 2020    str(ts),.     
+000484d0: 2020 2020 2020 2073 7472 2874 732e 6465         str(ts.de
+000484e0: 7065 6e64 656e 6369 6573 292c 0a20 2020  pendencies),.   
+000484f0: 2020 2020 2029 0a20 2020 2020 2020 2061       ).        a
+00048500: 7373 6572 7420 6e6f 7420 7473 2e77 6169  ssert not ts.wai
+00048510: 7469 6e67 5f6f 6e0a 0a20 2020 2069 6620  ting_on..    if 
+00048520: 7473 2e77 686f 5f68 6173 3a0a 2020 2020  ts.who_has:.    
+00048530: 2020 2020 6173 7365 7274 2074 732e 7761      assert ts.wa
+00048540: 6974 6572 7320 6f72 2074 732e 7768 6f5f  iters or ts.who_
+00048550: 7761 6e74 732c 2028 0a20 2020 2020 2020  wants, (.       
+00048560: 2020 2020 2022 756e 6e65 6564 6564 2074       "unneeded t
+00048570: 6173 6b20 696e 206d 656d 6f72 7922 2c0a  ask in memory",.
+00048580: 2020 2020 2020 2020 2020 2020 7374 7228              str(
+00048590: 7473 292c 0a20 2020 2020 2020 2020 2020  ts),.           
+000485a0: 2073 7472 2874 732e 7768 6f5f 6861 7329   str(ts.who_has)
+000485b0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+000485c0: 2020 2020 6966 2074 732e 7275 6e5f 7370      if ts.run_sp
+000485d0: 6563 3a20 2023 2077 6173 2063 6f6d 7075  ec:  # was compu
+000485e0: 7465 640a 2020 2020 2020 2020 2020 2020  ted.            
+000485f0: 6173 7365 7274 2074 732e 7479 7065 0a20  assert ts.type. 
+00048600: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+00048610: 7420 6973 696e 7374 616e 6365 2874 732e  t isinstance(ts.
+00048620: 7479 7065 2c20 7374 7229 0a20 2020 2020  type, str).     
+00048630: 2020 2061 7373 6572 7420 6e6f 7420 616e     assert not an
+00048640: 7928 5b74 7320 696e 2064 7473 2e77 6169  y([ts in dts.wai
+00048650: 7469 6e67 5f6f 6e20 666f 7220 6474 7320  ting_on for dts 
+00048660: 696e 2074 732e 6465 7065 6e64 656e 7473  in ts.dependents
+00048670: 5d29 0a20 2020 2020 2020 2066 6f72 2077  ]).        for w
+00048680: 7320 696e 2074 732e 7768 6f5f 6861 733a  s in ts.who_has:
+00048690: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
+000486a0: 6572 7420 7473 2069 6e20 7773 2e68 6173  ert ts in ws.has
+000486b0: 5f77 6861 742c 2028 0a20 2020 2020 2020  _what, (.       
+000486c0: 2020 2020 2020 2020 2022 6e6f 7420 696e           "not in
+000486d0: 2077 686f 5f68 6173 2720 6861 735f 7768   who_has' has_wh
+000486e0: 6174 222c 0a20 2020 2020 2020 2020 2020  at",.           
+000486f0: 2020 2020 2073 7472 2874 7329 2c0a 2020       str(ts),.  
+00048700: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00048710: 7228 7773 292c 0a20 2020 2020 2020 2020  r(ws),.         
+00048720: 2020 2020 2020 2073 7472 2877 732e 6861         str(ws.ha
+00048730: 735f 7768 6174 292c 0a20 2020 2020 2020  s_what),.       
+00048740: 2020 2020 2029 0a0a 2020 2020 666f 7220       )..    for 
+00048750: 6373 2069 6e20 7473 2e77 686f 5f77 616e  cs in ts.who_wan
+00048760: 7473 3a0a 2020 2020 2020 2020 6173 7365  ts:.        asse
+00048770: 7274 2074 7320 696e 2063 732e 7761 6e74  rt ts in cs.want
+00048780: 735f 7768 6174 2c20 280a 2020 2020 2020  s_what, (.      
+00048790: 2020 2020 2020 226e 6f74 2069 6e20 7768        "not in wh
+000487a0: 6f5f 7761 6e74 7327 2077 616e 7473 5f77  o_wants' wants_w
+000487b0: 6861 7422 2c0a 2020 2020 2020 2020 2020  hat",.          
+000487c0: 2020 7374 7228 7473 292c 0a20 2020 2020    str(ts),.     
+000487d0: 2020 2020 2020 2073 7472 2863 7329 2c0a         str(cs),.
+000487e0: 2020 2020 2020 2020 2020 2020 7374 7228              str(
+000487f0: 6373 2e77 616e 7473 5f77 6861 7429 2c0a  cs.wants_what),.
+00048800: 2020 2020 2020 2020 290a 0a20 2020 2069          )..    i
+00048810: 6620 7473 2e61 6374 6f72 3a0a 2020 2020  f ts.actor:.    
+00048820: 2020 2020 6966 2074 732e 7374 6174 6520      if ts.state 
+00048830: 3d3d 2022 6d65 6d6f 7279 223a 0a20 2020  == "memory":.   
+00048840: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+00048850: 7375 6d28 7473 2069 6e20 7773 2e61 6374  sum(ts in ws.act
+00048860: 6f72 7320 666f 7220 7773 2069 6e20 7473  ors for ws in ts
+00048870: 2e77 686f 5f68 6173 2920 3d3d 2031 0a20  .who_has) == 1. 
+00048880: 2020 2020 2020 2069 6620 7473 2e73 7461         if ts.sta
+00048890: 7465 203d 3d20 2270 726f 6365 7373 696e  te == "processin
+000488a0: 6722 3a0a 2020 2020 2020 2020 2020 2020  g":.            
+000488b0: 6173 7365 7274 2074 732e 7072 6f63 6573  assert ts.proces
+000488c0: 7369 6e67 5f6f 6e0a 2020 2020 2020 2020  sing_on.        
+000488d0: 2020 2020 6173 7365 7274 2074 7320 696e      assert ts in
+000488e0: 2074 732e 7072 6f63 6573 7369 6e67 5f6f   ts.processing_o
+000488f0: 6e2e 6163 746f 7273 0a20 2020 2020 2020  n.actors.       
+00048900: 2061 7373 6572 7420 7473 2e73 7461 7465   assert ts.state
+00048910: 2021 3d20 2271 7565 7565 6422 0a0a 0a64   != "queued"...d
+00048920: 6566 2076 616c 6964 6174 655f 776f 726b  ef validate_work
+00048930: 6572 5f73 7461 7465 2877 733a 2057 6f72  er_state(ws: Wor
+00048940: 6b65 7253 7461 7465 2920 2d3e 204e 6f6e  kerState) -> Non
+00048950: 653a 0a20 2020 2066 6f72 2074 7320 696e  e:.    for ts in
+00048960: 2077 732e 6861 735f 7768 6174 3a0a 2020   ws.has_what:.  
+00048970: 2020 2020 2020 6173 7365 7274 2077 7320        assert ws 
+00048980: 696e 2074 732e 7768 6f5f 6861 732c 2028  in ts.who_has, (
+00048990: 0a20 2020 2020 2020 2020 2020 2022 6e6f  .            "no
+000489a0: 7420 696e 2068 6173 5f77 6861 7427 2077  t in has_what' w
+000489b0: 686f 5f68 6173 222c 0a20 2020 2020 2020  ho_has",.       
+000489c0: 2020 2020 2073 7472 2877 7329 2c0a 2020       str(ws),.  
+000489d0: 2020 2020 2020 2020 2020 7374 7228 7473            str(ts
+000489e0: 292c 0a20 2020 2020 2020 2020 2020 2073  ),.            s
+000489f0: 7472 2874 732e 7768 6f5f 6861 7329 2c0a  tr(ts.who_has),.
+00048a00: 2020 2020 2020 2020 290a 0a20 2020 2066          )..    f
+00048a10: 6f72 2074 7320 696e 2077 732e 6163 746f  or ts in ws.acto
+00048a20: 7273 3a0a 2020 2020 2020 2020 6173 7365  rs:.        asse
+00048a30: 7274 2074 732e 7374 6174 6520 696e 2028  rt ts.state in (
+00048a40: 226d 656d 6f72 7922 2c20 2270 726f 6365  "memory", "proce
+00048a50: 7373 696e 6722 290a 0a0a 6465 6620 7661  ssing")...def va
+00048a60: 6c69 6461 7465 5f73 7461 7465 280a 2020  lidate_state(.  
+00048a70: 2020 7461 736b 733a 2064 6963 745b 7374    tasks: dict[st
+00048a80: 722c 2054 6173 6b53 7461 7465 5d2c 0a20  r, TaskState],. 
+00048a90: 2020 2077 6f72 6b65 7273 3a20 6469 6374     workers: dict
+00048aa0: 5b73 7472 2c20 576f 726b 6572 5374 6174  [str, WorkerStat
+00048ab0: 655d 2c0a 2020 2020 636c 6965 6e74 733a  e],.    clients:
+00048ac0: 2064 6963 745b 7374 722c 2043 6c69 656e   dict[str, Clien
+00048ad0: 7453 7461 7465 5d2c 0a29 202d 3e20 4e6f  tState],.) -> No
+00048ae0: 6e65 3a0a 2020 2020 2222 2256 616c 6964  ne:.    """Valid
+00048af0: 6174 6520 6120 6375 7272 656e 7420 7275  ate a current ru
+00048b00: 6e74 696d 6520 7374 6174 652e 0a0a 2020  ntime state...  
+00048b10: 2020 5468 6973 2070 6572 666f 726d 7320    This performs 
+00048b20: 6120 7365 7175 656e 6365 206f 6620 6368  a sequence of ch
+00048b30: 6563 6b73 206f 6e20 7468 6520 656e 7469  ecks on the enti
+00048b40: 7265 2067 7261 7068 2c20 7275 6e6e 696e  re graph, runnin
+00048b50: 6720 696e 2061 626f 7574 206c 696e 6561  g in about linea
+00048b60: 720a 2020 2020 7469 6d65 2e20 5468 6973  r.    time. This
+00048b70: 2072 6169 7365 7320 6173 7365 7274 2065   raises assert e
+00048b80: 7272 6f72 7320 6966 2061 6e79 7468 696e  rrors if anythin
+00048b90: 6720 646f 6573 6e27 7420 6368 6563 6b20  g doesn't check 
+00048ba0: 6f75 742e 0a20 2020 2022 2222 0a20 2020  out..    """.   
+00048bb0: 2066 6f72 2074 7320 696e 2074 6173 6b73   for ts in tasks
+00048bc0: 2e76 616c 7565 7328 293a 0a20 2020 2020  .values():.     
+00048bd0: 2020 2076 616c 6964 6174 655f 7461 736b     validate_task
+00048be0: 5f73 7461 7465 2874 7329 0a0a 2020 2020  _state(ts)..    
+00048bf0: 666f 7220 7773 2069 6e20 776f 726b 6572  for ws in worker
+00048c00: 732e 7661 6c75 6573 2829 3a0a 2020 2020  s.values():.    
+00048c10: 2020 2020 7661 6c69 6461 7465 5f77 6f72      validate_wor
+00048c20: 6b65 725f 7374 6174 6528 7773 290a 0a20  ker_state(ws).. 
+00048c30: 2020 2066 6f72 2063 7320 696e 2063 6c69     for cs in cli
+00048c40: 656e 7473 2e76 616c 7565 7328 293a 0a20  ents.values():. 
+00048c50: 2020 2020 2020 2066 6f72 2074 7320 696e         for ts in
+00048c60: 2063 732e 7761 6e74 735f 7768 6174 3a0a   cs.wants_what:.
+00048c70: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+00048c80: 7274 2063 7320 696e 2074 732e 7768 6f5f  rt cs in ts.who_
+00048c90: 7761 6e74 732c 2028 0a20 2020 2020 2020  wants, (.       
+00048ca0: 2020 2020 2020 2020 2022 6e6f 7420 696e           "not in
+00048cb0: 2077 616e 7473 5f77 6861 7427 2077 686f   wants_what' who
+00048cc0: 5f77 616e 7473 222c 0a20 2020 2020 2020  _wants",.       
+00048cd0: 2020 2020 2020 2020 2073 7472 2863 7329           str(cs)
+00048ce0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00048cf0: 2020 7374 7228 7473 292c 0a20 2020 2020    str(ts),.     
+00048d00: 2020 2020 2020 2020 2020 2073 7472 2874             str(t
+00048d10: 732e 7768 6f5f 7761 6e74 7329 2c0a 2020  s.who_wants),.  
+00048d20: 2020 2020 2020 2020 2020 290a 0a0a 6465            )...de
+00048d30: 6620 6865 6172 7462 6561 745f 696e 7465  f heartbeat_inte
+00048d40: 7276 616c 286e 3a20 696e 7429 202d 3e20  rval(n: int) -> 
+00048d50: 666c 6f61 743a 0a20 2020 2022 2222 496e  float:.    """In
+00048d60: 7465 7276 616c 2069 6e20 7365 636f 6e64  terval in second
+00048d70: 7320 7468 6174 2077 6520 6465 7369 7265  s that we desire
+00048d80: 2068 6561 7274 6265 6174 7320 6261 7365   heartbeats base
+00048d90: 6420 6f6e 206e 756d 6265 7220 6f66 2077  d on number of w
+00048da0: 6f72 6b65 7273 2222 220a 2020 2020 6966  orkers""".    if
+00048db0: 206e 203c 3d20 3130 3a0a 2020 2020 2020   n <= 10:.      
+00048dc0: 2020 7265 7475 726e 2030 2e35 0a20 2020    return 0.5.   
+00048dd0: 2065 6c69 6620 6e20 3c20 3530 3a0a 2020   elif n < 50:.  
+00048de0: 2020 2020 2020 7265 7475 726e 2031 0a20        return 1. 
+00048df0: 2020 2065 6c69 6620 6e20 3c20 3230 303a     elif n < 200:
+00048e00: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00048e10: 320a 2020 2020 656c 7365 3a0a 2020 2020  2.    else:.    
+00048e20: 2020 2020 2320 4e6f 206d 6f72 6520 7468      # No more th
+00048e30: 616e 2032 3030 2068 6561 7274 6265 6174  an 200 heartbeat
+00048e40: 7320 6120 7365 636f 6e64 2073 6361 6c65  s a second scale
+00048e50: 6420 6279 2077 6f72 6b65 7273 0a20 2020  d by workers.   
+00048e60: 2020 2020 2072 6574 7572 6e20 6e20 2f20       return n / 
+00048e70: 3230 3020 2b20 310a 0a0a 6465 6620 5f74  200 + 1...def _t
+00048e80: 6173 6b5f 736c 6f74 735f 6176 6169 6c61  ask_slots_availa
+00048e90: 626c 6528 7773 3a20 576f 726b 6572 5374  ble(ws: WorkerSt
+00048ea0: 6174 652c 2073 6174 7572 6174 696f 6e5f  ate, saturation_
+00048eb0: 6661 6374 6f72 3a20 666c 6f61 7429 202d  factor: float) -
+00048ec0: 3e20 696e 743a 0a20 2020 2022 2222 4e75  > int:.    """Nu
+00048ed0: 6d62 6572 206f 6620 7461 736b 7320 7468  mber of tasks th
+00048ee0: 6174 2063 616e 2062 6520 7365 6e74 2074  at can be sent t
+00048ef0: 6f20 7468 6973 2077 6f72 6b65 7220 7769  o this worker wi
+00048f00: 7468 6f75 7420 6f76 6572 7361 7475 7261  thout oversatura
+00048f10: 7469 6e67 2069 7422 2222 0a20 2020 2061  ting it""".    a
+00048f20: 7373 6572 7420 6e6f 7420 6d61 7468 2e69  ssert not math.i
+00048f30: 7369 6e66 2873 6174 7572 6174 696f 6e5f  sinf(saturation_
+00048f40: 6661 6374 6f72 290a 2020 2020 7265 7475  factor).    retu
+00048f50: 726e 206d 6178 286d 6174 682e 6365 696c  rn max(math.ceil
+00048f60: 2873 6174 7572 6174 696f 6e5f 6661 6374  (saturation_fact
+00048f70: 6f72 202a 2077 732e 6e74 6872 6561 6473  or * ws.nthreads
+00048f80: 292c 2031 2920 2d20 280a 2020 2020 2020  ), 1) - (.      
+00048f90: 2020 6c65 6e28 7773 2e70 726f 6365 7373    len(ws.process
+00048fa0: 696e 6729 202d 206c 656e 2877 732e 6c6f  ing) - len(ws.lo
+00048fb0: 6e67 5f72 756e 6e69 6e67 290a 2020 2020  ng_running).    
+00048fc0: 290a 0a0a 6465 6620 5f77 6f72 6b65 725f  )...def _worker_
+00048fd0: 6675 6c6c 2877 733a 2057 6f72 6b65 7253  full(ws: WorkerS
+00048fe0: 7461 7465 2c20 7361 7475 7261 7469 6f6e  tate, saturation
+00048ff0: 5f66 6163 746f 723a 2066 6c6f 6174 2920  _factor: float) 
+00049000: 2d3e 2062 6f6f 6c3a 0a20 2020 2069 6620  -> bool:.    if 
+00049010: 6d61 7468 2e69 7369 6e66 2873 6174 7572  math.isinf(satur
+00049020: 6174 696f 6e5f 6661 6374 6f72 293a 0a20  ation_factor):. 
+00049030: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00049040: 6c73 650a 2020 2020 7265 7475 726e 205f  lse.    return _
+00049050: 7461 736b 5f73 6c6f 7473 5f61 7661 696c  task_slots_avail
+00049060: 6162 6c65 2877 732c 2073 6174 7572 6174  able(ws, saturat
+00049070: 696f 6e5f 6661 6374 6f72 2920 3c3d 2030  ion_factor) <= 0
+00049080: 0a0a 0a63 6c61 7373 204b 696c 6c65 6457  ...class KilledW
+00049090: 6f72 6b65 7228 4578 6365 7074 696f 6e29  orker(Exception)
+000490a0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+000490b0: 5f5f 2873 656c 662c 2074 6173 6b3a 2073  __(self, task: s
+000490c0: 7472 2c20 6c61 7374 5f77 6f72 6b65 723a  tr, last_worker:
+000490d0: 2057 6f72 6b65 7253 7461 7465 2c20 616c   WorkerState, al
+000490e0: 6c6f 7765 645f 6661 696c 7572 6573 3a20  lowed_failures: 
+000490f0: 696e 7429 3a0a 2020 2020 2020 2020 7375  int):.        su
+00049100: 7065 7228 292e 5f5f 696e 6974 5f5f 2874  per().__init__(t
+00049110: 6173 6b2c 206c 6173 745f 776f 726b 6572  ask, last_worker
+00049120: 2c20 616c 6c6f 7765 645f 6661 696c 7572  , allowed_failur
+00049130: 6573 290a 0a20 2020 2040 7072 6f70 6572  es)..    @proper
+00049140: 7479 0a20 2020 2064 6566 2074 6173 6b28  ty.    def task(
+00049150: 7365 6c66 2920 2d3e 2073 7472 3a0a 2020  self) -> str:.  
+00049160: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00049170: 662e 6172 6773 5b30 5d0a 0a20 2020 2040  f.args[0]..    @
+00049180: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00049190: 206c 6173 745f 776f 726b 6572 2873 656c   last_worker(sel
+000491a0: 6629 202d 3e20 576f 726b 6572 5374 6174  f) -> WorkerStat
+000491b0: 653a 0a20 2020 2020 2020 2072 6574 7572  e:.        retur
+000491c0: 6e20 7365 6c66 2e61 7267 735b 315d 0a0a  n self.args[1]..
+000491d0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+000491e0: 2020 6465 6620 616c 6c6f 7765 645f 6661    def allowed_fa
+000491f0: 696c 7572 6573 2873 656c 6629 202d 3e20  ilures(self) -> 
+00049200: 696e 743a 0a20 2020 2020 2020 2072 6574  int:.        ret
+00049210: 7572 6e20 7365 6c66 2e61 7267 735b 325d  urn self.args[2]
+00049220: 0a0a 2020 2020 6465 6620 5f5f 7374 725f  ..    def __str_
+00049230: 5f28 7365 6c66 2920 2d3e 2073 7472 3a0a  _(self) -> str:.
+00049240: 2020 2020 2020 2020 7265 7475 726e 2028          return (
+00049250: 0a20 2020 2020 2020 2020 2020 2066 2241  .            f"A
+00049260: 7474 656d 7074 6564 2074 6f20 7275 6e20  ttempted to run 
+00049270: 7461 736b 207b 7365 6c66 2e74 6173 6b7d  task {self.task}
+00049280: 206f 6e20 7b73 656c 662e 616c 6c6f 7765   on {self.allowe
+00049290: 645f 6661 696c 7572 6573 7d20 6469 6666  d_failures} diff
+000492a0: 6572 656e 7420 220a 2020 2020 2020 2020  erent ".        
+000492b0: 2020 2020 2277 6f72 6b65 7273 2c20 6275      "workers, bu
+000492c0: 7420 616c 6c20 7468 6f73 6520 776f 726b  t all those work
+000492d0: 6572 7320 6469 6564 2077 6869 6c65 2072  ers died while r
+000492e0: 756e 6e69 6e67 2069 742e 2022 0a20 2020  unning it. ".   
+000492f0: 2020 2020 2020 2020 2066 2254 6865 206c           f"The l
+00049300: 6173 7420 776f 726b 6572 2074 6861 7420  ast worker that 
+00049310: 6174 7465 6d70 7420 746f 2072 756e 2074  attempt to run t
+00049320: 6865 2074 6173 6b20 7761 7320 7b73 656c  he task was {sel
+00049330: 662e 6c61 7374 5f77 6f72 6b65 722e 6164  f.last_worker.ad
+00049340: 6472 6573 737d 2e20 220a 2020 2020 2020  dress}. ".      
+00049350: 2020 2020 2020 2249 6e73 7065 6374 696e        "Inspectin
+00049360: 6720 776f 726b 6572 206c 6f67 7320 6973  g worker logs is
+00049370: 206f 6674 656e 2061 2067 6f6f 6420 6e65   often a good ne
+00049380: 7874 2073 7465 7020 746f 2064 6961 676e  xt step to diagn
+00049390: 6f73 6520 7768 6174 2077 656e 7420 7772  ose what went wr
+000493a0: 6f6e 672e 2022 0a20 2020 2020 2020 2020  ong. ".         
+000493b0: 2020 2022 466f 7220 6d6f 7265 2069 6e66     "For more inf
+000493c0: 6f72 6d61 7469 6f6e 2073 6565 2068 7474  ormation see htt
+000493d0: 7073 3a2f 2f64 6973 7472 6962 7574 6564  ps://distributed
+000493e0: 2e64 6173 6b2e 6f72 672f 656e 2f73 7461  .dask.org/en/sta
+000493f0: 626c 652f 6b69 6c6c 6564 2e68 746d 6c2e  ble/killed.html.
+00049400: 220a 2020 2020 2020 2020 290a 0a0a 636c  ".        )...cl
+00049410: 6173 7320 576f 726b 6572 5374 6174 7573  ass WorkerStatus
+00049420: 506c 7567 696e 2853 6368 6564 756c 6572  Plugin(Scheduler
+00049430: 506c 7567 696e 293a 0a20 2020 2022 2222  Plugin):.    """
+00049440: 4120 706c 7567 696e 2074 6f20 7368 6172  A plugin to shar
+00049450: 6520 776f 726b 6572 2073 7461 7475 7320  e worker status 
+00049460: 7769 7468 2061 2072 656d 6f74 6520 6f62  with a remote ob
+00049470: 7365 7276 6572 0a0a 2020 2020 5468 6973  server..    This
+00049480: 2069 7320 7573 6564 2069 6e20 636c 7573   is used in clus
+00049490: 7465 7220 6d61 6e61 6765 7273 2074 6f20  ter managers to 
+000494a0: 6b65 6570 2075 7064 6174 6564 2061 626f  keep updated abo
+000494b0: 7574 2074 6865 2073 7461 7475 7320 6f66  ut the status of
+000494c0: 2074 6865 2073 6368 6564 756c 6572 2e0a   the scheduler..
+000494d0: 2020 2020 2222 220a 0a20 2020 206e 616d      """..    nam
+000494e0: 653a 2043 6c61 7373 5661 725b 7374 725d  e: ClassVar[str]
+000494f0: 203d 2022 776f 726b 6572 2d73 7461 7475   = "worker-statu
+00049500: 7322 0a20 2020 2062 636f 6d6d 3a20 4261  s".    bcomm: Ba
+00049510: 7463 6865 6453 656e 640a 0a20 2020 2064  tchedSend..    d
+00049520: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00049530: 2c20 7363 6865 6475 6c65 723a 2053 6368  , scheduler: Sch
+00049540: 6564 756c 6572 2c20 636f 6d6d 3a20 436f  eduler, comm: Co
+00049550: 6d6d 293a 0a20 2020 2020 2020 2073 656c  mm):.        sel
+00049560: 662e 6263 6f6d 6d20 3d20 4261 7463 6865  f.bcomm = Batche
+00049570: 6453 656e 6428 696e 7465 7276 616c 3d22  dSend(interval="
+00049580: 356d 7322 290a 2020 2020 2020 2020 7365  5ms").        se
+00049590: 6c66 2e62 636f 6d6d 2e73 7461 7274 2863  lf.bcomm.start(c
+000495a0: 6f6d 6d29 0a20 2020 2020 2020 2073 6368  omm).        sch
+000495b0: 6564 756c 6572 2e61 6464 5f70 6c75 6769  eduler.add_plugi
+000495c0: 6e28 7365 6c66 290a 0a20 2020 2064 6566  n(self)..    def
+000495d0: 2061 6464 5f77 6f72 6b65 7228 7365 6c66   add_worker(self
+000495e0: 2c20 7363 6865 6475 6c65 723a 2053 6368  , scheduler: Sch
+000495f0: 6564 756c 6572 2c20 776f 726b 6572 3a20  eduler, worker: 
+00049600: 7374 7229 202d 3e20 4e6f 6e65 3a0a 2020  str) -> None:.  
+00049610: 2020 2020 2020 6964 656e 7420 3d20 7363        ident = sc
+00049620: 6865 6475 6c65 722e 776f 726b 6572 735b  heduler.workers[
+00049630: 776f 726b 6572 5d2e 6964 656e 7469 7479  worker].identity
+00049640: 2829 0a20 2020 2020 2020 2064 656c 2069  ().        del i
+00049650: 6465 6e74 5b22 6d65 7472 6963 7322 5d0a  dent["metrics"].
+00049660: 2020 2020 2020 2020 6465 6c20 6964 656e          del iden
+00049670: 745b 226c 6173 745f 7365 656e 225d 0a20  t["last_seen"]. 
+00049680: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00049690: 2020 2020 2020 2020 7365 6c66 2e62 636f          self.bco
+000496a0: 6d6d 2e73 656e 6428 5b22 6164 6422 2c20  mm.send(["add", 
+000496b0: 7b22 776f 726b 6572 7322 3a20 7b77 6f72  {"workers": {wor
+000496c0: 6b65 723a 2069 6465 6e74 7d7d 5d29 0a20  ker: ident}}]). 
+000496d0: 2020 2020 2020 2065 7863 6570 7420 436f         except Co
+000496e0: 6d6d 436c 6f73 6564 4572 726f 723a 0a20  mmClosedError:. 
+000496f0: 2020 2020 2020 2020 2020 2073 6368 6564             sched
+00049700: 756c 6572 2e72 656d 6f76 655f 706c 7567  uler.remove_plug
+00049710: 696e 286e 616d 653d 7365 6c66 2e6e 616d  in(name=self.nam
+00049720: 6529 0a0a 2020 2020 6465 6620 7265 6d6f  e)..    def remo
+00049730: 7665 5f77 6f72 6b65 7228 7365 6c66 2c20  ve_worker(self, 
+00049740: 7363 6865 6475 6c65 723a 2053 6368 6564  scheduler: Sched
+00049750: 756c 6572 2c20 776f 726b 6572 3a20 7374  uler, worker: st
+00049760: 7229 202d 3e20 4e6f 6e65 3a0a 2020 2020  r) -> None:.    
+00049770: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00049780: 2020 2020 2073 656c 662e 6263 6f6d 6d2e       self.bcomm.
+00049790: 7365 6e64 285b 2272 656d 6f76 6522 2c20  send(["remove", 
+000497a0: 776f 726b 6572 5d29 0a20 2020 2020 2020  worker]).       
+000497b0: 2065 7863 6570 7420 436f 6d6d 436c 6f73   except CommClos
+000497c0: 6564 4572 726f 723a 0a20 2020 2020 2020  edError:.       
+000497d0: 2020 2020 2073 6368 6564 756c 6572 2e72       scheduler.r
+000497e0: 656d 6f76 655f 706c 7567 696e 286e 616d  emove_plugin(nam
+000497f0: 653d 7365 6c66 2e6e 616d 6529 0a0a 2020  e=self.name)..  
+00049800: 2020 6465 6620 7465 6172 646f 776e 2873    def teardown(s
+00049810: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+00049820: 2020 2020 2020 7365 6c66 2e62 636f 6d6d        self.bcomm
+00049830: 2e63 6c6f 7365 2829 0a0a 0a63 6c61 7373  .close()...class
+00049840: 2043 6f6c 6c65 6374 5461 736b 4d65 7461   CollectTaskMeta
+00049850: 4461 7461 506c 7567 696e 2853 6368 6564  DataPlugin(Sched
+00049860: 756c 6572 506c 7567 696e 293a 0a20 2020  ulerPlugin):.   
+00049870: 2073 6368 6564 756c 6572 3a20 5363 6865   scheduler: Sche
+00049880: 6475 6c65 720a 2020 2020 6e61 6d65 3a20  duler.    name: 
+00049890: 7374 720a 2020 2020 6b65 7973 3a20 7365  str.    keys: se
+000498a0: 745b 7374 725d 0a20 2020 206d 6574 6164  t[str].    metad
+000498b0: 6174 613a 2064 6963 745b 7374 722c 2041  ata: dict[str, A
+000498c0: 6e79 5d0a 2020 2020 7374 6174 653a 2064  ny].    state: d
+000498d0: 6963 745b 7374 722c 2073 7472 5d0a 0a20  ict[str, str].. 
+000498e0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+000498f0: 7365 6c66 2c20 7363 6865 6475 6c65 723a  self, scheduler:
+00049900: 2053 6368 6564 756c 6572 2c20 6e61 6d65   Scheduler, name
+00049910: 3a20 7374 7229 3a0a 2020 2020 2020 2020  : str):.        
+00049920: 7365 6c66 2e73 6368 6564 756c 6572 203d  self.scheduler =
+00049930: 2073 6368 6564 756c 6572 0a20 2020 2020   scheduler.     
+00049940: 2020 2073 656c 662e 6e61 6d65 203d 206e     self.name = n
+00049950: 616d 650a 2020 2020 2020 2020 7365 6c66  ame.        self
+00049960: 2e6b 6579 7320 3d20 7365 7428 290a 2020  .keys = set().  
+00049970: 2020 2020 2020 7365 6c66 2e6d 6574 6164        self.metad
+00049980: 6174 6120 3d20 7b7d 0a20 2020 2020 2020  ata = {}.       
+00049990: 2073 656c 662e 7374 6174 6520 3d20 7b7d   self.state = {}
+000499a0: 0a0a 2020 2020 6465 6620 7570 6461 7465  ..    def update
+000499b0: 5f67 7261 7068 280a 2020 2020 2020 2020  _graph(.        
+000499c0: 7365 6c66 2c0a 2020 2020 2020 2020 7363  self,.        sc
+000499d0: 6865 6475 6c65 723a 2053 6368 6564 756c  heduler: Schedul
+000499e0: 6572 2c0a 2020 2020 2020 2020 2a2c 0a20  er,.        *,. 
+000499f0: 2020 2020 2020 206b 6579 733a 2073 6574         keys: set
+00049a00: 5b73 7472 5d2c 0a20 2020 2020 2020 202a  [str],.        *
+00049a10: 2a6b 7761 7267 733a 2041 6e79 2c0a 2020  *kwargs: Any,.  
+00049a20: 2020 2920 2d3e 204e 6f6e 653a 0a20 2020    ) -> None:.   
+00049a30: 2020 2020 2073 656c 662e 6b65 7973 2e75       self.keys.u
+00049a40: 7064 6174 6528 6b65 7973 290a 0a20 2020  pdate(keys)..   
+00049a50: 2064 6566 2074 7261 6e73 6974 696f 6e28   def transition(
+00049a60: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00049a70: 2020 2020 2020 206b 6579 3a20 7374 722c         key: str,
+00049a80: 0a20 2020 2020 2020 2073 7461 7274 3a20  .        start: 
+00049a90: 5461 736b 5374 6174 6553 7461 7465 2c0a  TaskStateState,.
+00049aa0: 2020 2020 2020 2020 6669 6e69 7368 3a20          finish: 
+00049ab0: 5461 736b 5374 6174 6553 7461 7465 2c0a  TaskStateState,.
+00049ac0: 2020 2020 2020 2020 2a61 7267 733a 2041          *args: A
+00049ad0: 6e79 2c0a 2020 2020 2020 2020 2a2a 6b77  ny,.        **kw
+00049ae0: 6172 6773 3a20 416e 792c 0a20 2020 2029  args: Any,.    )
+00049af0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00049b00: 2020 6966 2066 696e 6973 6820 696e 2028    if finish in (
+00049b10: 226d 656d 6f72 7922 2c20 2265 7272 6564  "memory", "erred
+00049b20: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+00049b30: 7473 203d 2073 656c 662e 7363 6865 6475  ts = self.schedu
+00049b40: 6c65 722e 7461 736b 732e 6765 7428 6b65  ler.tasks.get(ke
+00049b50: 7929 0a20 2020 2020 2020 2020 2020 2069  y).            i
+00049b60: 6620 7473 2069 7320 6e6f 7420 4e6f 6e65  f ts is not None
+00049b70: 2061 6e64 2074 732e 6b65 7920 696e 2073   and ts.key in s
+00049b80: 656c 662e 6b65 7973 3a0a 2020 2020 2020  elf.keys:.      
+00049b90: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00049ba0: 6574 6164 6174 615b 6b65 795d 203d 2074  etadata[key] = t
+00049bb0: 732e 6d65 7461 6461 7461 0a20 2020 2020  s.metadata.     
+00049bc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00049bd0: 7374 6174 655b 6b65 795d 203d 2066 696e  state[key] = fin
+00049be0: 6973 680a 2020 2020 2020 2020 2020 2020  ish.            
+00049bf0: 2020 2020 7365 6c66 2e6b 6579 732e 6469      self.keys.di
+00049c00: 7363 6172 6428 6b65 7929 0a              scard(key).
```

### Comparing `distributed-2023.4.1/distributed/security.py` & `distributed-2023.5.0/distributed/security.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/semaphore.py` & `distributed-2023.5.0/distributed/semaphore.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/shuffle/__init__.py` & `distributed-2023.5.0/distributed/shuffle/__init__.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/shuffle/_arrow.py` & `distributed-2023.5.0/distributed/shuffle/_arrow.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         column = meta_input[name]
         # FIXME: PyArrow does not support complex numbers: https://issues.apache.org/jira/browse/ARROW-638
         if pd.api.types.is_complex_dtype(column):
             raise TypeError(
                 f"p2p does not support data of type '{column.dtype}' found in column '{name}'."
             )
         # FIXME: PyArrow does not support sparse data: https://issues.apache.org/jira/browse/ARROW-8679
-        if pd.api.types.is_sparse(column):
+        if isinstance(column.dtype, pd.SparseDtype):
             raise TypeError("p2p does not support sparse data found in column '{name}'")
 
 
 def check_minimal_arrow_version() -> None:
     """Verify that the the correct version of pyarrow is installed to support
     the P2P extension.
```

### Comparing `distributed-2023.4.1/distributed/shuffle/_buffer.py` & `distributed-2023.5.0/distributed/shuffle/_buffer.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/shuffle/_comms.py` & `distributed-2023.5.0/distributed/shuffle/_comms.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/shuffle/_disk.py` & `distributed-2023.5.0/distributed/shuffle/_disk.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/shuffle/_limiter.py` & `distributed-2023.5.0/distributed/shuffle/_limiter.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/shuffle/_merge.py` & `distributed-2023.5.0/distributed/shuffle/_merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,21 +132,23 @@
 
 
 def merge_transfer(
     input: pd.DataFrame,
     id: ShuffleId,
     input_partition: int,
     npartitions: int,
+    parts_out: set[int],
 ):
     return shuffle_transfer(
         input=input,
         id=id,
         input_partition=input_partition,
         npartitions=npartitions,
         column=_HASH_COLUMN_NAME,
+        parts_out=parts_out,
     )
 
 
 def merge_unpack(
     shuffle_id_left: ShuffleId,
     shuffle_id_right: ShuffleId,
     output_partition: int,
@@ -336,23 +338,25 @@
             transfer_keys_left.append((name_left, i))
             dsk[(name_left, i)] = (
                 merge_transfer,
                 (self.name_input_left, i),
                 token_left,
                 i,
                 self.npartitions,
+                self.parts_out,
             )
         for i in range(self.n_partitions_right):
             transfer_keys_right.append((name_right, i))
             dsk[(name_right, i)] = (
                 merge_transfer,
                 (self.name_input_right, i),
                 token_right,
                 i,
                 self.npartitions,
+                self.parts_out,
             )
 
         _barrier_key_left = barrier_key(ShuffleId(token_left))
         _barrier_key_right = barrier_key(ShuffleId(token_right))
         dsk[_barrier_key_left] = (shuffle_barrier, token_left, transfer_keys_left)
         dsk[_barrier_key_right] = (shuffle_barrier, token_right, transfer_keys_right)
```

### Comparing `distributed-2023.4.1/distributed/shuffle/_rechunk.py` & `distributed-2023.5.0/distributed/shuffle/_rechunk.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from itertools import product
 from typing import TYPE_CHECKING, NamedTuple
 
 import dask
 from dask.base import tokenize
 from dask.highlevelgraph import HighLevelGraph, MaterializedLayer
 
+from distributed.exceptions import Reschedule
 from distributed.shuffle._shuffle import (
     ShuffleId,
     ShuffleType,
     _get_worker_extension,
     barrier_key,
     shuffle_barrier,
 )
@@ -53,33 +54,29 @@
 def rechunk_unpack(
     id: ShuffleId, output_chunk: NIndex, barrier_run_id: int
 ) -> np.ndarray:
     try:
         return _get_worker_extension().get_output_partition(
             id, barrier_run_id, output_chunk
         )
+    except Reschedule as e:
+        raise e
     except Exception as e:
         raise RuntimeError(f"rechunk_unpack failed during shuffle {id}") from e
 
 
 def rechunk_p2p(x: da.Array, chunks: ChunkedAxes) -> da.Array:
     import numpy as np
 
     import dask.array as da
 
     if x.size == 0:
         # Special case for empty array, as the algorithm below does not behave correctly
         return da.empty(x.shape, chunks=chunks, dtype=x.dtype)
 
-    if dask.config.get("optimization.fuse.active") is not False:
-        raise RuntimeError(
-            "P2P rechunking requires the fuse optimization to be turned off. "
-            "Set the 'optimization.fuse.active' config to False to deactivate."
-        )
-
     dsk: dict = {}
     token = tokenize(x, chunks)
     _barrier_key = barrier_key(ShuffleId(token))
     name = f"rechunk-transfer-{token}"
     transfer_keys = []
     for index in np.ndindex(tuple(len(dim) for dim in x.chunks)):
         transfer_keys.append((name,) + index)
```

### Comparing `distributed-2023.4.1/distributed/shuffle/_scheduler_extension.py` & `distributed-2023.5.0/distributed/shuffle/_scheduler_extension.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 import abc
 import contextlib
 import itertools
 import logging
 from collections import defaultdict
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, ClassVar
+from functools import partial
+from itertools import product
+from typing import TYPE_CHECKING, Any, Callable, ClassVar, Iterable, Sequence
 
 from distributed.diagnostics.plugin import SchedulerPlugin
 from distributed.shuffle._rechunk import ChunkedAxes, NIndex
 from distributed.shuffle._shuffle import (
     ShuffleId,
     ShuffleType,
     barrier_key,
@@ -101,14 +103,15 @@
     def __init__(self, scheduler: Scheduler):
         self.scheduler = scheduler
         self.scheduler.handlers.update(
             {
                 "shuffle_barrier": self.barrier,
                 "shuffle_get": self.get,
                 "shuffle_get_or_create": self.get_or_create,
+                "shuffle_restrict_task": self.restrict_task,
             }
         )
         self.heartbeats = defaultdict(lambda: defaultdict(dict))
         self.states = {}
         self.erred_shuffles = {}
         self.scheduler.add_plugin(self)
 
@@ -118,119 +121,182 @@
     async def barrier(self, id: ShuffleId, run_id: int) -> None:
         shuffle = self.states[id]
         msg = {"op": "shuffle_inputs_done", "shuffle_id": id, "run_id": run_id}
         await self.scheduler.broadcast(
             msg=msg, workers=list(shuffle.participating_workers)
         )
 
+    def restrict_task(self, id: ShuffleId, run_id: int, key: str, worker: str) -> dict:
+        shuffle = self.states[id]
+        if shuffle.run_id != run_id:
+            return {"status": "error", "message": "Stale shuffle"}
+        ts = self.scheduler.tasks[key]
+        self._set_restriction(ts, worker)
+        return {"status": "OK"}
+
     def heartbeat(self, ws: WorkerState, data: dict) -> None:
         for shuffle_id, d in data.items():
             if shuffle_id in self.shuffle_ids():
                 self.heartbeats[shuffle_id][ws.address].update(d)
 
     def get(self, id: ShuffleId, worker: str) -> dict[str, Any]:
         if exception := self.erred_shuffles.get(id):
-            return {"status": "ERROR", "message": str(exception)}
+            return {"status": "error", "message": str(exception)}
         state = self.states[id]
         state.participating_workers.add(worker)
         return state.to_msg()
 
     def get_or_create(
         self,
         id: ShuffleId,
         type: str,
         worker: str,
         spec: dict[str, Any],
     ) -> dict:
         try:
             return self.get(id, worker)
         except KeyError:
+            # FIXME: The current implementation relies on the barrier task to be
+            # known by its name. If the name has been mangled, we cannot guarantee
+            # that the shuffle works as intended and should fail instead.
+            self._raise_if_barrier_unknown(id)
+
             state: ShuffleState
             if type == ShuffleType.DATAFRAME:
                 state = self._create_dataframe_shuffle_state(id, spec)
             elif type == ShuffleType.ARRAY_RECHUNK:
                 state = self._create_array_rechunk_state(id, spec)
             else:  # pragma: no cover
                 raise TypeError(type)
             self.states[id] = state
             state.participating_workers.add(worker)
             return state.to_msg()
 
+    def _raise_if_barrier_unknown(self, id: ShuffleId) -> None:
+        key = barrier_key(id)
+        try:
+            self.scheduler.tasks[key]
+        except KeyError:
+            raise RuntimeError(
+                f"Barrier task with key {key!r} does not exist. This may be caused by "
+                "task fusion during graph generation. Please let us know that you ran "
+                "into this by leaving a comment at distributed#7816."
+            )
+
     def _create_dataframe_shuffle_state(
         self, id: ShuffleId, spec: dict[str, Any]
     ) -> DataFrameShuffleState:
         schema = spec["schema"]
         column = spec["column"]
         npartitions = spec["npartitions"]
+        parts_out = spec["parts_out"]
         assert schema is not None
         assert column is not None
         assert npartitions is not None
+        assert parts_out is not None
 
-        workers = list(self.scheduler.workers)
-        output_workers = set()
+        pick_worker = partial(get_worker_for_range_sharding, npartitions)
 
-        name = barrier_key(id)
-        mapping = {}
-
-        for ts in self.scheduler.tasks[name].dependents:
-            part = get_partition_id(ts)
-            if ts.worker_restrictions:
-                output_worker = list(ts.worker_restrictions)[0]
-            else:
-                output_worker = get_worker_for_range_sharding(
-                    part, workers, npartitions
-                )
-            mapping[part] = output_worker
-            output_workers.add(output_worker)
-            self.scheduler.set_restrictions({ts.key: {output_worker}})
+        mapping = self._pin_output_workers(id, parts_out, pick_worker)
+        output_workers = set(mapping.values())
 
         return DataFrameShuffleState(
             id=id,
             run_id=next(ShuffleState._run_id_iterator),
             worker_for=mapping,
             schema=schema,
             column=column,
             output_workers=output_workers,
             participating_workers=output_workers.copy(),
         )
 
+    def _pin_output_workers(
+        self,
+        id: ShuffleId,
+        output_partitions: Iterable[Any],
+        pick: Callable[[Any, Sequence[str]], str],
+    ) -> dict[Any, str]:
+        """Pin the outputs of a P2P shuffle to specific workers.
+
+        Parameters
+        ----------
+        id: ID of the shuffle to pin
+        output_partitions: Output partition IDs to pin
+        pick: Function that picks a worker given a partition ID and sequence of worker
+
+        .. note:
+            This function assumes that the barrier task and the output tasks share
+            the same worker restrictions.
+        """
+        mapping = {}
+        barrier = self.scheduler.tasks[barrier_key(id)]
+
+        if barrier.worker_restrictions:
+            workers = list(barrier.worker_restrictions)
+        else:
+            workers = list(self.scheduler.workers)
+
+        for partition in output_partitions:
+            worker = pick(partition, workers)
+            mapping[partition] = worker
+
+        for dt in barrier.dependents:
+            try:
+                partition = dt.annotations["shuffle"]
+            except KeyError:
+                continue
+
+            if dt.worker_restrictions:
+                worker = pick(partition, list(dt.worker_restrictions))
+                mapping[partition] = worker
+            else:
+                worker = mapping[partition]
+
+            self._set_restriction(dt, worker)
+
+        return mapping
+
     def _create_array_rechunk_state(
         self, id: ShuffleId, spec: dict[str, Any]
     ) -> ArrayRechunkState:
         old = spec["old"]
         new = spec["new"]
         assert old is not None
         assert new is not None
 
-        workers = list(self.scheduler.workers)
-        output_workers = set()
-
-        name = barrier_key(id)
-        mapping = {}
-
-        for ts in self.scheduler.tasks[name].dependents:
-            part = get_partition_id(ts)
-            if ts.worker_restrictions:
-                output_worker = list(ts.worker_restrictions)[0]
-            else:
-                output_worker = get_worker_for_hash_sharding(part, workers)
-            mapping[part] = output_worker
-            output_workers.add(output_worker)
-            self.scheduler.set_restrictions({ts.key: {output_worker}})
+        parts_out = product(*(range(len(c)) for c in new))
+        mapping = self._pin_output_workers(id, parts_out, get_worker_for_hash_sharding)
+        output_workers = set(mapping.values())
 
         return ArrayRechunkState(
             id=id,
             run_id=next(ShuffleState._run_id_iterator),
             worker_for=mapping,
             output_workers=output_workers,
             old=old,
             new=new,
             participating_workers=output_workers.copy(),
         )
 
+    def _set_restriction(self, ts: TaskState, worker: str) -> None:
+        if "shuffle_original_restrictions" in ts.annotations:
+            # This may occur if multiple barriers share the same output task,
+            # e.g. in a hash join.
+            return
+        ts.annotations["shuffle_original_restrictions"] = ts.worker_restrictions.copy()
+        self.scheduler.set_restrictions({ts.key: {worker}})
+
+    def _unset_restriction(self, ts: TaskState) -> None:
+        # shuffle_original_restrictions is only set if the task was first scheduled
+        # on the wrong worker
+        if "shuffle_original_restrictions" not in ts.annotations:
+            return
+        original_restrictions = ts.annotations.pop("shuffle_original_restrictions")
+        self.scheduler.set_restrictions({ts.key: original_restrictions})
+
     def remove_worker(self, scheduler: Scheduler, worker: str) -> None:
         from time import time
 
         stimulus_id = f"shuffle-failed-worker-left-{time()}"
 
         for shuffle_id, shuffle in self.states.items():
             if worker not in shuffle.participating_workers:
@@ -243,15 +309,15 @@
 
             barrier_task = self.scheduler.tasks[barrier_key(shuffle_id)]
             recs: Recs = {}
             if barrier_task.state == "memory":
                 for dt in barrier_task.dependents:
                     if worker not in dt.worker_restrictions:
                         continue
-                    dt.worker_restrictions.clear()
+                    self._unset_restriction(dt)
                     recs.update({dt.key: "waiting"})
                 # TODO: Do we need to handle other states?
 
             self.scheduler.transitions(recs, stimulus_id=stimulus_id)
 
     def transition(
         self,
@@ -289,38 +355,31 @@
 
     def _clean_on_scheduler(self, id: ShuffleId) -> None:
         del self.states[id]
         self.erred_shuffles.pop(id, None)
         with contextlib.suppress(KeyError):
             del self.heartbeats[id]
 
+        barrier_task = self.scheduler.tasks[barrier_key(id)]
+        for dt in barrier_task.dependents:
+            self._unset_restriction(dt)
+
     def restart(self, scheduler: Scheduler) -> None:
         self.states.clear()
         self.heartbeats.clear()
         self.erred_shuffles.clear()
 
 
-def get_partition_id(ts: TaskState) -> Any:
-    """Get the output partition ID of this task state."""
-    try:
-        return ts.annotations["shuffle"]
-    except KeyError:
-        raise RuntimeError(
-            f"{ts} has lost its ``shuffle`` annotation. This may be caused by "
-            "unintended optimization during graph generation. "
-            "Please report this problem on GitHub and link it to "
-            "the tracking issue at https://github.com/dask/distributed/issues/7716."
-        )
-
-
 def get_worker_for_range_sharding(
-    output_partition: int, workers: list[str], npartitions: int
+    npartitions: int, output_partition: int, workers: Sequence[str]
 ) -> str:
     """Get address of target worker for this output partition using range sharding"""
     i = len(workers) * output_partition // npartitions
     return workers[i]
 
 
-def get_worker_for_hash_sharding(output_partition: NIndex, workers: list[str]) -> str:
+def get_worker_for_hash_sharding(
+    output_partition: NIndex, workers: Sequence[str]
+) -> str:
     """Get address of target worker for this output partition using hash sharding"""
     i = hash(output_partition) % len(workers)
     return workers[i]
```

### Comparing `distributed-2023.4.1/distributed/shuffle/_shuffle.py` & `distributed-2023.5.0/distributed/shuffle/_shuffle.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 import logging
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Iterable, Iterator, NewType
 
-import dask
 from dask.base import tokenize
 from dask.highlevelgraph import HighLevelGraph
 from dask.layers import Layer
 
+from distributed.exceptions import Reschedule
 from distributed.shuffle._arrow import check_dtype_support, check_minimal_arrow_version
 
 logger = logging.getLogger("distributed.shuffle")
 if TYPE_CHECKING:
     import pandas as pd
 
     # TODO import from typing (requires Python >=3.10)
@@ -52,35 +52,39 @@
 
 def shuffle_transfer(
     input: pd.DataFrame,
     id: ShuffleId,
     input_partition: int,
     npartitions: int,
     column: str,
+    parts_out: set[int],
 ) -> int:
     try:
         return _get_worker_extension().add_partition(
             input,
             shuffle_id=id,
             type=ShuffleType.DATAFRAME,
             input_partition=input_partition,
             npartitions=npartitions,
             column=column,
+            parts_out=parts_out,
         )
     except Exception as e:
         raise RuntimeError(f"shuffle_transfer failed during shuffle {id}") from e
 
 
 def shuffle_unpack(
     id: ShuffleId, output_partition: int, barrier_run_id: int
 ) -> pd.DataFrame:
     try:
         return _get_worker_extension().get_output_partition(
             id, barrier_run_id, output_partition
         )
+    except Reschedule as e:
+        raise e
     except Exception as e:
         raise RuntimeError(f"shuffle_unpack failed during shuffle {id}") from e
 
 
 def shuffle_barrier(id: ShuffleId, run_ids: list[int]) -> int:
     try:
         return _get_worker_extension().barrier(id, run_ids)
@@ -91,20 +95,14 @@
 def rearrange_by_column_p2p(
     df: DataFrame,
     column: str,
     npartitions: int | None = None,
 ) -> DataFrame:
     from dask.dataframe import DataFrame
 
-    if dask.config.get("optimization.fuse.active"):
-        raise RuntimeError(
-            "P2P shuffling requires the fuse optimization to be turned off. "
-            "Set the 'optimization.fuse.active' config to False to deactivate."
-        )
-
     check_dtype_support(df._meta)
     npartitions = npartitions or df.npartitions
     token = tokenize(df, column, npartitions)
 
     empty = df._meta.copy()
     if any(not isinstance(c, str) for c in empty.columns):
         unsupported = {c: type(c) for c in empty.columns if not isinstance(c, str)}
@@ -141,25 +139,25 @@
         npartitions: int,
         npartitions_input: int,
         name_input: str,
         parts_out: Iterable | None = None,
         annotations: dict | None = None,
     ):
         check_minimal_arrow_version()
-        annotations = annotations or {}
-        annotations.update({"shuffle": lambda key: key[1]})
         self.name = name
         self.column = column
         self.npartitions = npartitions
         self.name_input = name_input
         if parts_out:
             self.parts_out = set(parts_out)
         else:
             self.parts_out = set(range(self.npartitions))
         self.npartitions_input = npartitions_input
+        annotations = annotations or {}
+        annotations.update({"shuffle": lambda key: key[1]})
         super().__init__(annotations=annotations)
 
     def __repr__(self) -> str:
         return (
             f"{type(self).__name__}<name='{self.name}', npartitions={self.npartitions}>"
         )
 
@@ -242,14 +240,15 @@
             dsk[(name, i)] = (
                 shuffle_transfer,
                 (self.name_input, i),
                 token,
                 i,
                 self.npartitions,
                 self.column,
+                self.parts_out,
             )
 
         dsk[_barrier_key] = (shuffle_barrier, token, transfer_keys)
 
         name = self.name
         for part_out in self.parts_out:
             dsk[(name, part_out)] = (shuffle_unpack, token, part_out, _barrier_key)
```

### Comparing `distributed-2023.4.1/distributed/shuffle/_worker_extension.py` & `distributed-2023.5.0/distributed/shuffle/_worker_extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 from collections.abc import Callable, Iterator
 from concurrent.futures import ThreadPoolExecutor
 from io import BytesIO
 from typing import TYPE_CHECKING, Any, Generic, TypeVar, overload
 
 import toolz
 
+from dask.context import thread_state
 from dask.utils import parse_bytes
 
 from distributed.core import PooledRPCCall
+from distributed.exceptions import Reschedule
 from distributed.protocol import to_serialize
 from distributed.shuffle._arrow import (
     convert_partition,
     deserialize_schema,
     list_of_buffers_to_table,
     serialize_table,
 )
@@ -201,26 +203,44 @@
         self.raise_if_closed()
         data: bytes = self._disk_buffer.read("_".join(str(i) for i in id))
         return data
 
     async def receive(self, data: list[tuple[T_transfer_shard_id, bytes]]) -> None:
         await self._receive(data)
 
+    async def _ensure_output_worker(self, i: T_partition_id, key: str) -> None:
+        assigned_worker = self._get_assigned_worker(i)
+
+        if assigned_worker != self.local_address:
+            result = await self.scheduler.shuffle_restrict_task(
+                id=self.id, run_id=self.run_id, key=key, worker=assigned_worker
+            )
+            if result["status"] == "error":
+                raise RuntimeError(result["message"])
+            assert result["status"] == "OK"
+            raise Reschedule()
+
+    @abc.abstractmethod
+    def _get_assigned_worker(self, i: T_partition_id) -> str:
+        """Get the address of the worker assigned to the output partition"""
+
     @abc.abstractmethod
     async def _receive(self, data: list[tuple[T_transfer_shard_id, bytes]]) -> None:
         """Receive shards belonging to output partitions of this shuffle run"""
 
     @abc.abstractmethod
     async def add_partition(
         self, data: T_partition_type, input_partition: T_partition_id
     ) -> int:
         """Add an input partition to the shuffle run"""
 
     @abc.abstractmethod
-    async def get_output_partition(self, i: T_partition_id) -> T_partition_type:
+    async def get_output_partition(
+        self, i: T_partition_id, key: str
+    ) -> T_partition_type:
         """Get an output partition to the shuffle run"""
 
 
 # TODO remove quotes on tuple (requires Python >=3.9)
 class ArrayRechunkRun(ShuffleRun[ArrayRechunkShardID, NIndex, "np.ndarray"]):
     """State for a single active rechunk execution
 
@@ -350,35 +370,33 @@
                 )
             return out
 
         out = await self.offload(_)
         await self._write_to_comm(out)
         return self.run_id
 
-    async def get_output_partition(self, i: NIndex) -> np.ndarray:
+    async def get_output_partition(self, i: NIndex, key: str) -> np.ndarray:
         self.raise_if_closed()
         assert self.transferred, "`get_output_partition` called before barrier task"
 
-        assert self.worker_for[i] == self.local_address, (
-            f"Output partition {i} belongs on {self.worker_for[i]}, "
-            f"not {self.local_address}. "
-        )
-        # ^ NOTE: this check isn't necessary, just a nice validation to prevent incorrect
-        # data in the case something has gone very wrong
+        await self._ensure_output_worker(i, key)
 
         await self.flush_receive()
 
         data = self._read_from_disk(i)
 
         def _() -> np.ndarray:
             subdims = tuple(len(self._old_to_new[dim][ix]) for dim, ix in enumerate(i))
             return convert_chunk(data, subdims)
 
         return await self.offload(_)
 
+    def _get_assigned_worker(self, i: NIndex) -> str:
+        return self.worker_for[i]
+
 
 class DataFrameShuffleRun(ShuffleRun[int, int, "pd.DataFrame"]):
     """State for a single active shuffle execution
 
     This object is responsible for splitting, sending, receiving and combining
     data shards.
 
@@ -503,38 +521,36 @@
             out = {k: [(input_partition, serialize_table(t))] for k, t in out.items()}
             return out
 
         out = await self.offload(_)
         await self._write_to_comm(out)
         return self.run_id
 
-    async def get_output_partition(self, i: int) -> pd.DataFrame:
+    async def get_output_partition(self, i: int, key: str) -> pd.DataFrame:
         self.raise_if_closed()
         assert self.transferred, "`get_output_partition` called before barrier task"
 
-        assert self.worker_for[i] == self.local_address, (
-            f"Output partition {i} belongs on {self.worker_for[i]}, "
-            f"not {self.local_address}. "
-        )
-        # ^ NOTE: this check isn't necessary, just a nice validation to prevent incorrect
-        # data in the case something has gone very wrong
+        await self._ensure_output_worker(i, key)
 
         await self.flush_receive()
         try:
             data = self._read_from_disk((i,))
 
             def _() -> pd.DataFrame:
                 df = convert_partition(data)
                 return df.to_pandas()
 
             out = await self.offload(_)
         except KeyError:
             out = self.schema.empty_table().to_pandas()
         return out
 
+    def _get_assigned_worker(self, i: int) -> str:
+        return self.worker_for[i]
+
 
 class ShuffleWorkerExtension:
     """Interface between a Worker and a Shuffle.
 
     This extension is responsible for
 
     - Lifecycle of Shuffle instances
@@ -759,28 +775,29 @@
                 type=type,
                 spec={
                     "schema": pa.Schema.from_pandas(kwargs["empty"])
                     .serialize()
                     .to_pybytes(),
                     "npartitions": kwargs["npartitions"],
                     "column": kwargs["column"],
+                    "parts_out": kwargs["parts_out"],
                 },
                 worker=self.worker.address,
             )
         elif type == ShuffleType.ARRAY_RECHUNK:
             assert kwargs is not None
             result = await self.worker.scheduler.shuffle_get_or_create(
                 id=shuffle_id,
                 type=type,
                 spec=kwargs,
                 worker=self.worker.address,
             )
         else:  # pragma: no cover
             raise TypeError(type)
-        if result["status"] == "ERROR":
+        if result["status"] == "error":
             raise RuntimeError(result["message"])
         assert result["status"] == "OK"
 
         if self.closed:
             raise ShuffleClosedError(
                 f"{self.__class__.__name__} already closed on {self.worker.address}"
             )
@@ -896,15 +913,18 @@
     ) -> Any:
         """
         Task: Retrieve a shuffled output partition from the ShuffleExtension.
 
         Calling this for a ``shuffle_id`` which is unknown or incomplete is an error.
         """
         shuffle = self.get_shuffle_run(shuffle_id, run_id)
-        return sync(self.worker.loop, shuffle.get_output_partition, output_partition)
+        key = thread_state.key
+        return sync(
+            self.worker.loop, shuffle.get_output_partition, output_partition, key
+        )
 
 
 def split_by_worker(
     df: pd.DataFrame,
     column: str,
     worker_for: pd.Series,
 ) -> dict[Any, pa.Table]:
```

### Comparing `distributed-2023.4.1/distributed/sizeof.py` & `distributed-2023.5.0/distributed/sizeof.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/spill.py` & `distributed-2023.5.0/distributed/spill.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
 import logging
 from collections import defaultdict
 from collections.abc import Hashable, Iterator, Mapping, Sized
 from contextlib import contextmanager
 from functools import partial
+from typing import Callable  # TODO import from collections.abc (requires Python >=3.9)
 from typing import Literal, NamedTuple, Protocol, cast
 
 import zict
 
 from distributed.metrics import context_meter
 from distributed.protocol import deserialize_bytes, serialize_bytelist
+from distributed.protocol.compression import get_compression_settings
 from distributed.sizeof import safe_sizeof
 from distributed.utils import RateLimiterFilter
 
 logger = logging.getLogger(__name__)
 logger.addFilter(RateLimiterFilter("Spill file on disk reached capacity"))
 logger.addFilter(RateLimiterFilter("Spill to disk failed"))
 
@@ -275,19 +277,28 @@
 
 class Slow(zict.Func[str, object, bytes]):
     max_weight: int | Literal[False]
     weight_by_key: dict[str, SpilledSize]
     total_weight: SpilledSize
 
     def __init__(self, spill_directory: str, max_weight: int | Literal[False] = False):
-        super().__init__(
-            partial(serialize_bytelist, on_error="raise"),
-            deserialize_bytes,
-            zict.File(spill_directory),
+        compression = get_compression_settings(
+            "distributed.worker.memory.spill-compression"
         )
+
+        # File is MutableMapping[str, bytes], but serialize_bytelist returns
+        # list[bytes | bytearray | memorymapping], which File.__setitem__ actually
+        # accepts despite its signature; File.__getitem__ actually returns
+        # bytearray. This headache is because MutableMapping doesn't allow for
+        # asymmetric VT in __getitem__ and __setitem__.
+        dump = cast(
+            Callable[[object], bytes],
+            partial(serialize_bytelist, compression=compression, on_error="raise"),
+        )
+        super().__init__(dump, deserialize_bytes, zict.File(spill_directory))
         self.max_weight = max_weight
         self.weight_by_key = {}
         self.total_weight = SpilledSize(0, 0)
 
     def __getitem__(self, key: str) -> object:
         with context_meter.meter("disk-read", "seconds"):
             pickled = self.d[key]
@@ -303,19 +314,15 @@
             # zict.LRU ensures that the key remains in fast if we raise.
             # Wrap the exception so that it's recognizable by SpillBuffer,
             # which will then unwrap it.
             raise PickleError(key, e)
 
         pickled_size = sum(
             frame.nbytes if isinstance(frame, memoryview) else len(frame)
-            # File is MutableMapping[str, bytes], but serialize_bytelist returns
-            # list[bytes | bytearray | memorymapping], which File.__setitem__ actually
-            # accepts despite its signature; File.__getitem__ actually returns
-            # bytearray. This headache is because MutableMapping doesn't allow for
-            # asymmetric VT in __getitem__ and __setitem__.
+            # See note in __init__ about serialize_bytelist
             for frame in cast(list, pickled)
         )
 
         # Thanks to Buffer.__setitem__, we never update existing
         # keys in slow, but always delete them and reinsert them.
         assert key not in self.d
         assert key not in self.weight_by_key
```

### Comparing `distributed-2023.4.1/distributed/stealing.py` & `distributed-2023.5.0/distributed/stealing.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/system.py` & `distributed-2023.5.0/distributed/system.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/system_monitor.py` & `distributed-2023.5.0/distributed/system_monitor.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/threadpoolexecutor.py` & `distributed-2023.5.0/distributed/threadpoolexecutor.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/utils.py` & `distributed-2023.5.0/distributed/utils.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/utils_comm.py` & `distributed-2023.5.0/distributed/utils_comm.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/utils_perf.py` & `distributed-2023.5.0/distributed/utils_perf.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/utils_test.py` & `distributed-2023.5.0/distributed/utils_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 from distributed.nanny import Nanny
 from distributed.node import ServerNode
 from distributed.proctitle import enable_proctitle_on_children
 from distributed.protocol import deserialize
 from distributed.scheduler import TaskState as SchedulerTaskState
 from distributed.security import Security
 from distributed.utils import (
+    Deadline,
     DequeHandler,
     _offload_executor,
     get_ip,
     get_ipv6,
     get_mp_context,
     iscoroutinefunction,
     log_errors,
@@ -108,14 +109,15 @@
     for name, logger in logging.root.manager.loggerDict.items()
     if isinstance(logger, logging.Logger)
 }
 
 _TEST_TIMEOUT = 30
 _offload_executor.submit(lambda: None).result()  # create thread during import
 
+
 # Dask configuration to completely disable the Active Memory Manager.
 # This is typically used with @gen_cluster(config=NO_AMM)
 # or @gen_cluster(config=merge(NO_AMM, {<more config options})).
 NO_AMM = {"distributed.scheduler.active-memory-manager.start": False}
 
 
 async def cleanup_global_workers():
@@ -911,40 +913,40 @@
 
     assert timeout, (
         "timeout should always be set and it should be smaller than the global one from"
         "pytest-timeout"
     )
     if is_debugging():
         timeout = 3600
-
     scheduler_kwargs = merge(
         dict(
             dashboard=False,
             dashboard_address=":0",
             transition_counter_max=50_000,
         ),
         scheduler_kwargs,
     )
     worker_kwargs = merge(
         dict(
             memory_limit=system.MEMORY_LIMIT,
-            death_timeout=15,
             transition_counter_max=50_000,
         ),
         worker_kwargs,
     )
 
     def _(func):
         if not iscoroutinefunction(func):
             raise RuntimeError("gen_cluster only works for coroutine functions.")
 
         @functools.wraps(func)
         @config_for_cluster_tests(**{"distributed.comm.timeouts.connect": "5s"})
         @clean(**clean_kwargs)
         def test_func(*outer_args, **kwargs):
+            deadline = Deadline.after(timeout)
+
             @contextlib.asynccontextmanager
             async def _client_factory(s):
                 if client:
                     async with Client(
                         s.address,
                         security=security,
                         asynchronous=True,
@@ -963,15 +965,18 @@
                         try:
                             s, ws = await start_cluster(
                                 nthreads,
                                 scheduler,
                                 security=security,
                                 Worker=Worker,
                                 scheduler_kwargs=scheduler_kwargs,
-                                worker_kwargs=worker_kwargs,
+                                worker_kwargs=merge(
+                                    {"death_timeout": min(15, int(deadline.remaining))},
+                                    worker_kwargs,
+                                ),
                             )
                         except Exception as e:
                             logger.error(
                                 "Failed to start gen_cluster: "
                                 f"{e.__class__.__name__}: {e}; retrying",
                                 exc_info=True,
                             )
@@ -995,20 +1000,23 @@
                     ) as c:
                         args = [s] + workers
                         if c is not None:
                             args = [c] + args
                         try:
                             coro = func(*args, *outer_args, **kwargs)
                             task = asyncio.create_task(coro)
-                            coro2 = utils_wait_for(asyncio.shield(task), timeout)
+                            coro2 = utils_wait_for(
+                                asyncio.shield(task), timeout=deadline.remaining
+                            )
                             result = await coro2
                             validate_state(s, *workers)
 
                         except asyncio.TimeoutError:
                             assert task
+                            elapsed = deadline.elapsed
                             buffer = io.StringIO()
                             # This stack indicates where the coro/test is suspended
                             task.print_stack(file=buffer)
 
                             if cluster_dump_directory:
                                 await dump_cluster_state(
                                     s=s,
@@ -1026,15 +1034,15 @@
                             # timeout
                             validate_state(s, *workers)
 
                             # Remove as much of the traceback as possible; it's
                             # uninteresting boilerplate from utils_test and asyncio
                             # and not from the code being tested.
                             raise asyncio.TimeoutError(
-                                f"Test timeout after {timeout}s.\n"
+                                f"Test timeout ({timeout}) hit after {elapsed}s.\n"
                                 "========== Test stack trace starts here ==========\n"
                                 f"{buffer.getvalue()}"
                             ) from None
 
                         except pytest.xfail.Exception:
                             raise
 
@@ -1059,16 +1067,15 @@
 
                     def get_unclosed():
                         return [c for c in Comm._instances if not c.closed()] + [
                             c for c in _global_clients.values() if c.status != "closed"
                         ]
 
                     try:
-                        start = time()
-                        while time() < start + 60:
+                        while deadline.remaining:
                             gc.collect()
                             if not get_unclosed():
                                 break
                             await asyncio.sleep(0.05)
                         else:
                             if allow_unclosed:
                                 print(f"Unclosed Comms: {get_unclosed()}")
```

### Comparing `distributed-2023.4.1/distributed/variable.py` & `distributed-2023.5.0/distributed/variable.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/versions.py` & `distributed-2023.5.0/distributed/versions.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/widgets/templates/client.html.j2` & `distributed-2023.5.0/distributed/widgets/templates/client.html.j2`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/widgets/templates/cluster.html.j2` & `distributed-2023.5.0/distributed/widgets/templates/cluster.html.j2`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/widgets/templates/computation.html.j2` & `distributed-2023.5.0/distributed/widgets/templates/computation.html.j2`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/widgets/templates/future.html.j2` & `distributed-2023.5.0/distributed/widgets/templates/future.html.j2`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/widgets/templates/has_what.html.j2` & `distributed-2023.5.0/distributed/widgets/templates/has_what.html.j2`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/widgets/templates/log.html.j2` & `distributed-2023.5.0/distributed/widgets/templates/log.html.j2`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/widgets/templates/process_interface.html.j2` & `distributed-2023.5.0/distributed/widgets/templates/process_interface.html.j2`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/widgets/templates/scheduler_info.html.j2` & `distributed-2023.5.0/distributed/widgets/templates/scheduler_info.html.j2`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/worker.py` & `distributed-2023.5.0/distributed/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import errno
 import logging
 import math
 import os
 import pathlib
 import random
 import sys
-import tempfile
 import threading
 import warnings
 import weakref
 from collections import defaultdict, deque
 from collections.abc import (
     Callable,
     Collection,
@@ -70,52 +69,53 @@
 from distributed.core import (
     ConnectionPool,
     PooledRPCCall,
     Status,
     coerce_to_address,
     context_meter_to_server_digest,
     error_message,
+    loads_function,
     pingpong,
 )
 from distributed.core import rpc as RPCType
 from distributed.core import send_recv
 from distributed.diagnostics import nvml, rmm
 from distributed.diagnostics.plugin import _get_plugin_name
-from distributed.diskutils import WorkDir, WorkSpace
+from distributed.diskutils import WorkSpace
+from distributed.exceptions import Reschedule
 from distributed.http import get_handlers
 from distributed.metrics import context_meter, thread_time, time
 from distributed.node import ServerNode
 from distributed.proctitle import setproctitle
 from distributed.protocol import pickle, to_serialize
+from distributed.protocol.serialize import _is_dumpable
 from distributed.pubsub import PubSubWorkerExtension
 from distributed.security import Security
 from distributed.shuffle import ShuffleWorkerExtension
 from distributed.sizeof import safe_sizeof as sizeof
 from distributed.threadpoolexecutor import ThreadPoolExecutor
 from distributed.threadpoolexecutor import secede as tpe_secede
 from distributed.utils import (
     TimeoutError,
     _maybe_complex,
     get_ip,
     has_arg,
-    import_file,
     in_async_call,
     is_python_shutting_down,
     iscoroutinefunction,
     json_load_robust,
     log_errors,
     offload,
     parse_ports,
     recursive_to_dict,
     run_in_executor_with_context,
     set_thread_state,
     silence_logging_cmgr,
     thread_state,
     wait_for,
-    warn_on_duration,
 )
 from distributed.utils_comm import gather_from_workers, pack_data, retry_operation
 from distributed.utils_perf import disable_gc_diagnosis, enable_gc_diagnosis
 from distributed.versions import get_versions
 from distributed.worker_memory import (
     DeprecatedMemoryManagerAttribute,
     DeprecatedMemoryMonitor,
@@ -430,16 +430,14 @@
     transfer_outgoing_bytes: int
     #: Current number of open data transfers to other workers
     transfer_outgoing_count: int
     bandwidth: float
     latency: float
     profile_cycle_interval: float
     workspace: WorkSpace
-    _workdir: WorkDir
-    local_directory: str
     _client: Client | None
     bandwidth_workers: defaultdict[str, tuple[float, int]]
     bandwidth_types: defaultdict[type, tuple[float, int]]
     preloads: list[preloading.Preload]
     contact_address: str | None
     _start_port: int | str | Collection[int] | None = None
     _start_host: str | None
@@ -594,71 +592,28 @@
         if profile_cycle_interval is None:
             profile_cycle_interval = dask.config.get("distributed.worker.profile.cycle")
         profile_cycle_interval = parse_timedelta(profile_cycle_interval, default="ms")
         assert profile_cycle_interval
 
         self._setup_logging(logger)
 
-        if not local_directory:
-            local_directory = (
-                dask.config.get("temporary-directory") or tempfile.gettempdir()
-            )
-        local_directory = os.path.join(local_directory, "dask-worker-space")
-
-        with warn_on_duration(
-            "1s",
-            "Creating scratch directories is taking a surprisingly long time. ({duration:.2f}s) "
-            "This is often due to running workers on a network file system. "
-            "Consider specifying a local-directory to point workers to write "
-            "scratch data to a local disk.",
-        ):
-            self._workspace = WorkSpace(local_directory)
-            self._workdir = self._workspace.new_work_dir(prefix="worker-")
-            self.local_directory = self._workdir.dir_path
-
-        if not preload:
-            preload = dask.config.get("distributed.worker.preload")
-        if not preload_argv:
-            preload_argv = dask.config.get("distributed.worker.preload-argv")
-        assert preload is not None
-        assert preload_argv is not None
-        self.preloads = preloading.process_preloads(
-            self, preload, preload_argv, file_dir=self.local_directory
-        )
-
         self.death_timeout = parse_timedelta(death_timeout)
-        if scheduler_file:
-            cfg = json_load_robust(scheduler_file, timeout=self.death_timeout)
-            scheduler_addr = cfg["address"]
-        elif scheduler_ip is None and dask.config.get("scheduler-address", None):
-            scheduler_addr = dask.config.get("scheduler-address")
-        elif scheduler_port is None:
-            scheduler_addr = coerce_to_address(scheduler_ip)
-        else:
-            scheduler_addr = coerce_to_address((scheduler_ip, scheduler_port))
         self.contact_address = contact_address
 
-        if protocol is None:
-            protocol_address = scheduler_addr.split("://")
-            if len(protocol_address) == 2:
-                protocol = protocol_address[0]
-            assert protocol
-
         self._start_port = port
         self._start_host = host
         if host:
             # Helpful error message if IPv6 specified incorrectly
             _, host_address = parse_address(host)
             if host_address.count(":") > 1 and not host_address.startswith("["):
                 raise ValueError(
                     "Host address with IPv6 must be bracketed like '[::1]'; "
                     f"got {host_address}"
                 )
         self._interface = interface
-        self._protocol = protocol
 
         nthreads = nthreads or CPU_COUNT
         if resources is None:
             resources = dask.config.get("distributed.worker.resources")
             assert isinstance(resources, dict)
 
         self.extensions = {}
@@ -698,17 +653,14 @@
             )
 
         self.batched_stream = BatchedSend(interval="2ms", loop=self.loop)
         self.name = name
         self.scheduler_delay = 0
         self.stream_comms = {}
 
-        if self.local_directory not in sys.path:
-            sys.path.insert(0, self.local_directory)
-
         self.plugins = {}
         self._pending_plugins = plugins
 
         self.services = {}
         self.service_specs = services or {}
 
         self._dashboard_address = dashboard_address
@@ -765,16 +717,46 @@
         }
 
         ServerNode.__init__(
             self,
             handlers=handlers,
             stream_handlers=stream_handlers,
             connection_args=self.connection_args,
+            local_directory=local_directory,
             **kwargs,
         )
+
+        if not preload:
+            preload = dask.config.get("distributed.worker.preload")
+        if not preload_argv:
+            preload_argv = dask.config.get("distributed.worker.preload-argv")
+        assert preload is not None
+        assert preload_argv is not None
+
+        self.preloads = preloading.process_preloads(
+            self, preload, preload_argv, file_dir=self.local_directory
+        )
+
+        if scheduler_file:
+            cfg = json_load_robust(scheduler_file, timeout=self.death_timeout)
+            scheduler_addr = cfg["address"]
+        elif scheduler_ip is None and dask.config.get("scheduler-address", None):
+            scheduler_addr = dask.config.get("scheduler-address")
+        elif scheduler_port is None:
+            scheduler_addr = coerce_to_address(scheduler_ip)
+        else:
+            scheduler_addr = coerce_to_address((scheduler_ip, scheduler_port))
+
+        if protocol is None:
+            protocol_address = scheduler_addr.split("://")
+            if len(protocol_address) == 2:
+                protocol = protocol_address[0]
+            assert protocol
+        self._protocol = protocol
+
         self.memory_manager = WorkerMemoryManager(
             self,
             data=data,
             nthreads=nthreads,
             memory_limit=memory_limit,
             memory_target_fraction=memory_target_fraction,
             memory_spill_fraction=memory_spill_fraction,
@@ -973,14 +955,32 @@
         )
 
     @property
     def logs(self):
         return self._deque_handler.deque
 
     def log_event(self, topic: str | Collection[str], msg: Any) -> None:
+        """Log an event under a given topic
+
+        Parameters
+        ----------
+        topic : str, list[str]
+            Name of the topic under which to log an event. To log the same
+            event under multiple topics, pass a list of topic names.
+        msg
+            Event message to log. Note this must be msgpack serializable.
+
+        See also
+        --------
+        Client.log_event
+        """
+        if not _is_dumpable(msg):
+            raise TypeError(
+                f"Message must be msgpack serializable. Got {type(msg)=} instead."
+            )
         full_msg = {
             "op": "log-event",
             "topic": topic,
             "msg": msg,
         }
         if self.thread_id == threading.get_ident():
             self.batched_send(full_msg)
@@ -1280,43 +1280,14 @@
     @fail_hard
     async def handle_scheduler(self, comm: Comm) -> None:
         try:
             await self.handle_stream(comm)
         finally:
             await self.close(reason="worker-handle-scheduler-connection-broken")
 
-    async def upload_file(
-        self, filename: str, data: str | bytes, load: bool = True
-    ) -> dict[str, Any]:
-        out_filename = os.path.join(self.local_directory, filename)
-
-        def func(data):
-            if isinstance(data, str):
-                data = data.encode()
-            with open(out_filename, "wb") as f:
-                f.write(data)
-                f.flush()
-                os.fsync(f.fileno())
-            return data
-
-        if len(data) < 10000:
-            data = func(data)
-        else:
-            data = await offload(func, data)
-
-        if load:
-            try:
-                import_file(out_filename)
-                cache_loads.data.clear()
-            except Exception as e:
-                logger.exception(e)
-                raise e
-
-        return {"status": "OK", "nbytes": len(data)}
-
     def keys(self) -> list[str]:
         return list(self.data)
 
     async def gather(self, who_has: dict[str, list[str]]) -> dict[str, Any]:
         who_has = {
             k: [coerce_to_address(addr) for addr in v]
             for k, v in who_has.items()
@@ -1594,15 +1565,14 @@
                     else:
                         # There is still the chance that even with us
                         # telling the client to be async, itself will decide
                         # otherwise
                         c.close()
 
         await self.scheduler.close_rpc()
-        self._workdir.release()
 
         self.stop_services()
 
         # Give some time for a UCX scheduler to complete closing endpoints
         # before closing self.batched_stream, otherwise the local endpoint
         # may be closed too early and errors be raised on the scheduler when
         # trying to send closing message.
@@ -2817,28 +2787,14 @@
             key=thread_state.key,
             compute_duration=duration,
             stimulus_id=f"secede-{time()}",
         ),
     )
 
 
-class Reschedule(Exception):
-    """Reschedule this task
-
-    Raising this exception will stop the current execution of the task and ask
-    the scheduler to reschedule this task, possibly on a different machine.
-
-    This does not guarantee that the task will move onto a different machine.
-    The scheduler will proceed through its normal heuristics to determine the
-    optimal machine to accept this task.  The machine will likely change if the
-    load across the cluster has significantly changed since first scheduling
-    the task.
-    """
-
-
 @overload
 async def get_data_from_worker(
     rpc: ConnectionPool,
     keys: Collection[str],
     worker: str,
     *,
     who: str | None = None,
@@ -2912,29 +2868,14 @@
     finally:
         rpc.reuse(worker, comm)
 
 
 job_counter = [0]
 
 
-cache_loads = LRU(maxsize=100)
-
-
-def loads_function(bytes_object):
-    """Load a function from bytes, cache bytes"""
-    if len(bytes_object) < 100000:
-        try:
-            result = cache_loads[bytes_object]
-        except KeyError:
-            result = pickle.loads(bytes_object)
-            cache_loads[bytes_object] = result
-        return result
-    return pickle.loads(bytes_object)
-
-
 @context_meter.meter("deserialize")
 def _deserialize(function=None, args=None, kwargs=None, task=NO_VALUE):
     """Deserialize task inputs and regularize to func, args, kwargs"""
     # Some objects require threadlocal state during deserialization, e.g. to
     # detect the current worker
     if function is not None:
         function = loads_function(function)
```

### Comparing `distributed-2023.4.1/distributed/worker_client.py` & `distributed-2023.5.0/distributed/worker_client.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/worker_memory.py` & `distributed-2023.5.0/distributed/worker_memory.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed/worker_state_machine.py` & `distributed-2023.5.0/distributed/worker_state_machine.py`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/distributed.egg-info/PKG-INFO` & `distributed-2023.5.0/distributed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distributed
-Version: 2023.4.1
+Version: 2023.5.0
 Summary: Distributed scheduler for Dask
 Maintainer-email: Matthew Rocklin <mrocklin@gmail.com>
 License: BSD
 Project-URL: Homepage, https://distributed.dask.org
 Project-URL: Source, https://github.com/dask/distributed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `distributed-2023.4.1/distributed.egg-info/SOURCES.txt` & `distributed-2023.5.0/distributed.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 distributed/config.py
 distributed/core.py
 distributed/counter.py
 distributed/diskutils.py
 distributed/distributed-schema.yaml
 distributed/distributed.yaml
 distributed/event.py
+distributed/exceptions.py
 distributed/lock.py
 distributed/metrics.py
 distributed/multi_lock.py
 distributed/nanny.py
 distributed/node.py
 distributed/objects.py
 distributed/preloading.py
@@ -93,14 +94,15 @@
 distributed/dashboard/worker.py
 distributed/dashboard/components/__init__.py
 distributed/dashboard/components/nvml.py
 distributed/dashboard/components/rmm.py
 distributed/dashboard/components/scheduler.py
 distributed/dashboard/components/shared.py
 distributed/dashboard/components/worker.py
+distributed/dashboard/templates/__init__.py
 distributed/dashboard/templates/performance_report.html
 distributed/deploy/__init__.py
 distributed/deploy/adaptive.py
 distributed/deploy/adaptive_core.py
 distributed/deploy/cluster.py
 distributed/deploy/local.py
 distributed/deploy/old_ssh.py
@@ -133,29 +135,34 @@
 distributed/http/scheduler/info.py
 distributed/http/scheduler/json.py
 distributed/http/scheduler/missing_bokeh.py
 distributed/http/scheduler/prometheus/__init__.py
 distributed/http/scheduler/prometheus/core.py
 distributed/http/scheduler/prometheus/semaphore.py
 distributed/http/scheduler/prometheus/stealing.py
+distributed/http/static/__init__.py
 distributed/http/static/individual-cluster-map.html
+distributed/http/static/css/__init__.py
 distributed/http/static/css/base.css
 distributed/http/static/css/gpu.css
 distributed/http/static/css/individual-cluster-map.css
 distributed/http/static/css/status.css
+distributed/http/static/images/__init__.py
 distributed/http/static/images/dask-logo.svg
 distributed/http/static/images/fa-bars.svg
 distributed/http/static/images/favicon.ico
 distributed/http/static/images/jupyter.svg
 distributed/http/static/images/numpy.png
 distributed/http/static/images/pandas.png
 distributed/http/static/images/python.png
+distributed/http/static/js/__init__.py
 distributed/http/static/js/anime.min.js
 distributed/http/static/js/individual-cluster-map.js
 distributed/http/static/js/reconnecting-websocket.min.js
+distributed/http/templates/__init__.py
 distributed/http/templates/base.html
 distributed/http/templates/call-stack.html
 distributed/http/templates/exceptions.html
 distributed/http/templates/gpu.html
 distributed/http/templates/json-index.html
 distributed/http/templates/logs.html
 distributed/http/templates/main.html
@@ -194,14 +201,15 @@
 distributed/shuffle/_limiter.py
 distributed/shuffle/_merge.py
 distributed/shuffle/_rechunk.py
 distributed/shuffle/_scheduler_extension.py
 distributed/shuffle/_shuffle.py
 distributed/shuffle/_worker_extension.py
 distributed/widgets/__init__.py
+distributed/widgets/templates/__init__.py
 distributed/widgets/templates/client.html.j2
 distributed/widgets/templates/cluster.html.j2
 distributed/widgets/templates/computation.html.j2
 distributed/widgets/templates/future.html.j2
 distributed/widgets/templates/has_what.html.j2
 distributed/widgets/templates/local_cluster.html.j2
 distributed/widgets/templates/log.html.j2
```

### Comparing `distributed-2023.4.1/docs/source/active_memory_manager.rst` & `distributed-2023.5.0/docs/source/active_memory_manager.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/actors.rst` & `distributed-2023.5.0/docs/source/actors.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/api.rst` & `distributed-2023.5.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/asynchronous.rst` & `distributed-2023.5.0/docs/source/asynchronous.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/changelog.rst` & `distributed-2023.5.0/docs/source/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,41 @@
 Changelog
 =========
 
+.. _v2023.5.0:
+
+2023.5.0
+--------
+
+Released on May 12, 2023
+
+Enhancements
+^^^^^^^^^^^^
+- ``Client.upload_file`` send to both Workers and Scheduler and rename scratch directory (:pr:`7802`) `Miles`_
+- Allow dashboard to be used with bokeh prereleases (:pr:`7814`) `James Bourbeau`_
+
+Bug Fixes
+^^^^^^^^^
+- Ensure log_event of non-msgpack serializable object do not kill servers (:pr:`7472`) `Florian Jetter`_
+- Fix ``test_nanny.py`` duplicated ``pytestmark`` definitions (:pr:`7819`) `Thomas Grainger`_
+- Fix flaky ``test_dask_worker.py::test_single_executable_deprecated`` (:pr:`7817`) `Thomas Grainger`_
+
+Maintenance
+^^^^^^^^^^^
+- Annotation-less P2P shuffling (:pr:`7801`) `Hendrik Makait`_
+- Fix docstring for ``batch_size`` in ``client.map`` (:pr:`7833`) `David Chudzicki`_
+- Refactor ``test_protocol.py`` (:pr:`7829`) `crusaderky`_
+- Lint #6496 (:pr:`7828`) `crusaderky`_
+- Remove hardcoded 60s timeout (:pr:`6496`) `Florian Jetter`_
+- Add ``__init__.py`` files to template and static directories (:pr:`7809`) `Thomas Grainger`_
+- Disable compression for fast comms (:pr:`7768`) `crusaderky`_
+- Avoid deprecated ``pd.api.types.is_sparse`` (:pr:`7813`) `James Bourbeau`_
+- Bump gpuCI ``PYTHON_VER`` from 3.8 to 3.9 (:pr:`7812`) `Charles Blackmon-Luca`_
+
+
 .. _v2023.4.1:
 
 2023.4.1
 --------
 
 Released on April 28, 2023
```

### Comparing `distributed-2023.4.1/docs/source/client.rst` & `distributed-2023.5.0/docs/source/client.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/communications.rst` & `distributed-2023.5.0/docs/source/communications.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/develop.rst` & `distributed-2023.5.0/docs/source/develop.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/diagnosing-performance.rst` & `distributed-2023.5.0/docs/source/diagnosing-performance.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/efficiency.rst` & `distributed-2023.5.0/docs/source/efficiency.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/examples/word-count.rst` & `distributed-2023.5.0/docs/source/examples/word-count.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/faq.rst` & `distributed-2023.5.0/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/foundations.rst` & `distributed-2023.5.0/docs/source/foundations.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/http_services.rst` & `distributed-2023.5.0/docs/source/http_services.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/index.rst` & `distributed-2023.5.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/install.rst` & `distributed-2023.5.0/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/journey.rst` & `distributed-2023.5.0/docs/source/journey.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/killed.rst` & `distributed-2023.5.0/docs/source/killed.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/limitations.rst` & `distributed-2023.5.0/docs/source/limitations.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/locality.rst` & `distributed-2023.5.0/docs/source/locality.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/logging.rst` & `distributed-2023.5.0/docs/source/logging.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/manage-computation.rst` & `distributed-2023.5.0/docs/source/manage-computation.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/memory.rst` & `distributed-2023.5.0/docs/source/memory.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/plugins.rst` & `distributed-2023.5.0/docs/source/plugins.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/priority.rst` & `distributed-2023.5.0/docs/source/priority.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/prometheus.rst` & `distributed-2023.5.0/docs/source/prometheus.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/protocol.rst` & `distributed-2023.5.0/docs/source/protocol.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/publish.rst` & `distributed-2023.5.0/docs/source/publish.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/quickstart.rst` & `distributed-2023.5.0/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/related-work.rst` & `distributed-2023.5.0/docs/source/related-work.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/resilience.rst` & `distributed-2023.5.0/docs/source/resilience.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/resources.rst` & `distributed-2023.5.0/docs/source/resources.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/scheduling-policies.rst` & `distributed-2023.5.0/docs/source/scheduling-policies.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/scheduling-state.rst` & `distributed-2023.5.0/docs/source/scheduling-state.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/serialization.rst` & `distributed-2023.5.0/docs/source/serialization.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/task-launch.rst` & `distributed-2023.5.0/docs/source/task-launch.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/tls.rst` & `distributed-2023.5.0/docs/source/tls.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/work-stealing.rst` & `distributed-2023.5.0/docs/source/work-stealing.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/worker-memory.rst` & `distributed-2023.5.0/docs/source/worker-memory.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/worker-state.rst` & `distributed-2023.5.0/docs/source/worker-state.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/docs/source/worker.rst` & `distributed-2023.5.0/docs/source/worker.rst`

 * *Files identical despite different names*

### Comparing `distributed-2023.4.1/pyproject.toml` & `distributed-2023.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "Topic :: System :: Distributed Computing",
 ]
 readme = "README.rst"
 requires-python = ">=3.8"
 dependencies = [
     "click >= 8.0",
     "cloudpickle >= 1.5.0",
-    "dask == 2023.4.1",
+    "dask == 2023.5.0",
     "jinja2 >= 2.10.3",
     "locket >= 1.0.0",
     "msgpack >= 1.0.0",
     "packaging >= 20.0",
     "psutil >= 5.7.0",
     "pyyaml >= 5.3.1",
     "sortedcontainers >= 2.0.5",
```


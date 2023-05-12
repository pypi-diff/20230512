# Comparing `tmp/adaptive_scheduler-1.8.0.tar.gz` & `tmp/adaptive_scheduler-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptive_scheduler-1.8.0.tar", last modified: Mon Apr 10 19:35:50 2023, max compression
+gzip compressed data, was "adaptive_scheduler-2.0.0.tar", last modified: Thu May 11 23:59:29 2023, max compression
```

## Comparing `adaptive_scheduler-1.8.0.tar` & `adaptive_scheduler-2.0.0.tar`

### file list

```diff
@@ -1,27 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:35:50.799599 adaptive_scheduler-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-04-10 19:35:50.799599 adaptive_scheduler-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:35:50.803598 adaptive_scheduler-1.8.0/adaptive_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/adaptive_scheduler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6835 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/adaptive_scheduler/_mock_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-10 19:35:50.803598 adaptive_scheduler-1.8.0/adaptive_scheduler/_static_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/adaptive_scheduler/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/adaptive_scheduler/client_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/adaptive_scheduler/run_script.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)    33523 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/adaptive_scheduler/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/adaptive_scheduler/sequence_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)    51548 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/adaptive_scheduler/server_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    27703 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/adaptive_scheduler/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/adaptive_scheduler/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:35:50.799599 adaptive_scheduler-1.8.0/adaptive_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-04-10 19:35:50.000000 adaptive_scheduler-1.8.0/adaptive_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-10 19:35:50.000000 adaptive_scheduler-1.8.0/adaptive_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:35:50.000000 adaptive_scheduler-1.8.0/adaptive_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-10 19:35:50.000000 adaptive_scheduler-1.8.0/adaptive_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-10 19:35:50.000000 adaptive_scheduler-1.8.0/adaptive_scheduler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-10 19:35:50.803598 adaptive_scheduler-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-10 19:35:40.000000 adaptive_scheduler-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:59:29.853717 adaptive_scheduler-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-11 23:59:29.853717 adaptive_scheduler-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:59:29.857717 adaptive_scheduler-2.0.0/adaptive_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7755 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_mock_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:59:29.845717 adaptive_scheduler-2.0.0/adaptive_scheduler/_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_scheduler/base_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_scheduler/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_scheduler/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_scheduler/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_scheduler/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:59:29.849717 adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/base_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13255 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/database_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/kill_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/parse_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/run_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/_server_support/slurm_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-11 23:59:29.857717 adaptive_scheduler-2.0.0/adaptive_scheduler/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/client_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/server_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35819 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32694 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/adaptive_scheduler/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:59:29.845717 adaptive_scheduler-2.0.0/adaptive_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-11 23:59:29.000000 adaptive_scheduler-2.0.0/adaptive_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-11 23:59:29.000000 adaptive_scheduler-2.0.0/adaptive_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 23:59:29.000000 adaptive_scheduler-2.0.0/adaptive_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-11 23:59:29.000000 adaptive_scheduler-2.0.0/adaptive_scheduler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-11 23:59:29.000000 adaptive_scheduler-2.0.0/adaptive_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 23:59:29.000000 adaptive_scheduler-2.0.0/adaptive_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-11 23:59:29.853717 adaptive_scheduler-2.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      523 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:59:29.853717 adaptive_scheduler-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_base_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_client_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13256 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_database_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_kill_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_log_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_log_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_run_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_server_support_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_slurm_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_slurm_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16970 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10801 2023-05-11 23:59:07.000000 adaptive_scheduler-2.0.0/tests/test_widgets.py
```

### Comparing `adaptive_scheduler-1.8.0/LICENSE` & `adaptive_scheduler-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-1.8.0/PKG-INFO` & `adaptive_scheduler-2.0.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,251 +1,203 @@
-Metadata-Version: 2.1
-Name: adaptive_scheduler
-Version: 1.8.0
-Summary: Run many `adaptive.Learner`s on many cores (>10k) using `mpi4py.futures`, `ipyparallel`, `dask-mpi`, or `process-pool`.
-Home-page: https://github.com/basnijholt/adaptive-scheduler
-Download-URL: https://pypi.python.org/pypi/adaptive_scheduler
-Maintainer: Bas Nijholt
-Maintainer-email: bas@nijho.lt
-License: BSD-3
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: System :: Distributed Computing
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-Provides-Extra: all
-License-File: LICENSE
-License-File: AUTHORS.md
+# Asynchronous Job Scheduler for Adaptive :rocket:
 
-An asynchronous job scheduler for `Adaptive <https://github.com/python-adaptive/adaptive/>`_
-============================================================================================
+[![PyPI](https://img.shields.io/pypi/v/adaptive-scheduler.svg)](https://pypi.python.org/pypi/adaptive-scheduler)
+[![Conda](https://img.shields.io/conda/v/conda-forge/adaptive-scheduler.svg?label=conda-forge)](https://anaconda.org/conda-forge/adaptive-scheduler)
+[![Downloads](https://anaconda.org/conda-forge/adaptive-scheduler/badges/downloads.svg)](https://anaconda.org/conda-forge/adaptive-scheduler)
+[![Build Status](https://github.com/basnijholt/adaptive-scheduler/actions/workflows/pytest.yml/badge.svg)](https://github.com/basnijholt/adaptive-scheduler/actions/workflows/pytest.yml)
+[![Documentation Status](https://readthedocs.org/projects/adaptive-scheduler/badge/?version=latest)](https://adaptive-scheduler.readthedocs.io/en/latest/?badge=latest)
+[![CodeCov](https://codecov.io/gh/basnijholt/adaptive-scheduler/branch/main/graph/badge.svg)](https://codecov.io/gh/basnijholt/adaptive-scheduler)
 
-|PyPI|  |Conda|  |Downloads|  |Build Status| |Documentation Status|
+This is an asynchronous job scheduler for [`Adaptive`](https://github.com/python-adaptive/adaptive/), designed to run many `adaptive.Learner`s on many cores (>***10k-100k***) using `mpi4py.futures`, `ipyparallel`, `loky`, `concurrent.futures.ProcessPoolExecutor`, or `dask.distributed`.
 
-Run many ``adaptive.Learner``\ s on many cores (>10k) using `mpi4py.futures`, `ipyparallel`, or `distributed`.
+<!-- toc-start -->
+## :books: Table of Contents
+<!-- START doctoc generated TOC please keep comment here to allow auto update -->
+<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
-What is this?
--------------
+- [:thinking: What is this?](#thinking-what-is-this)
+- [:dart: Design Goals](#dart-design-goals)
+- [:test_tube: How does it work?](#test_tube-how-does-it-work)
+- [:mag: But how does it *really* work?](#mag-but-how-does-it-really-work)
+- [:notebook: Jupyter Notebook Example](#notebook-jupyter-notebook-example)
+- [:computer: Installation](#computer-installation)
+- [:hammer_and_wrench: Development](#hammer_and_wrench-development)
+- [:warning: Limitations](#warning-limitations)
 
-The Adaptive scheduler solves the following problem, you need to run more learners than you can run with a single runner and/or can use >1k cores.
- 
-`ipyparallel` and `distributed` provide very powerful engines for interactive sessions. However, when you want to connect to >1k cores it starts to struggle. Besides that, on a shared cluster there is often the problem of starting an interactive session with ample space available.
+<!-- END doctoc generated TOC please keep comment here to allow auto update -->
+<!-- toc-end -->
 
-Our approach is to schedule a different job for each ``adaptive.Learner``. The creation and running of these jobs are managed by ``adaptive-scheduler``. This means that your calculation will definitely run, even though the cluster might be fully occupied at the moment. Because of this approach, there is almost no limit to how many cores you want to use. You can either use 10 nodes for 1 job (\ ``learner``\ ) or 1 core for 1 job (\ ``learner``\ ) while scheduling hundreds of jobs.
+## :thinking: What is this?
 
-Everything is written such that the computation is maximally local. This means that is one of the jobs crashes, there is no problem and it will automatically schedule a new one and continue the calculation where it left off (because of Adaptive's periodic saving functionality). Even if the central "job manager" dies, the jobs will continue to run (although no new jobs will be scheduled.)
+Adaptive Scheduler is designed to address the challenge of executing a large number of `adaptive.Learner`s in parallel, even when using more than **1k-100k cores**.
+Traditional engines like `ipyparallel` and `distributed` can struggle with such high core counts because there is a central process that communicates with each worker.
 
+This library schedules a separate job for each `adaptive.Learner`, and manages the creation and execution of these jobs.
+This ensures that your calculations will run even if the cluster is currently fully occupied (because job will just be put in the queue).
+The approach allows for nearly limitless core usage, whether you allocate 10 nodes for a single job or 1 core for a single job while scheduling hundreds of jobs.
 
-Design goals
-------------
+The computation is designed for maximum locality.
+If a job crashes, it will automatically reschedule a new one and continue the calculation from where it left off, thanks to Adaptive's periodic saving functionality.
+Even if the central "job manager" fails, the jobs will continue to run, although no new jobs will be scheduled.
 
-#. Needs to be able to run on efficiently >30k cores
-#. Works seamlessly with the Adaptive package
-#. Minimal load on the file system
-#. Removes all boilerplate of working with a scheduler
+## :dart: Design Goals
 
-   #. writes job script
-   #. (re)submits job scripts
+1. Needs to be able to run efficiently on >30k cores.
+2. Works seamlessly with the Adaptive package.
+3. Minimal load on the file system.
+4. Removes all boilerplate of working with a scheduler:
+   - Writes job script.
+   - (Re)submits job scripts.
+5. Handles random crashes (or node evictions) with minimal data loss.
+6. Preserves Python kernel and variables inside a job (in contrast to submitting jobs for every parameter).
+7. Separates the simulation definition code from the code that runs the simulation.
+8. Maximizes computation locality, jobs continue to run when the main process dies.
 
-#. Handles random crashes (or node evictions) with minimal data loss
-#. Preserves Python kernel and variables inside a job (in contrast to submitting jobs for every parameter)
-#. Separates the simulation definition code from the code that runs the simulation
-#. Maximizes computation locality, jobs continue to run when the main process dies
+## :test_tube: How does it work?
 
-How does it work?
------------------
+You create a bunch of `learners` and corresponding `fnames` so they can be loaded, like:
 
-You create a bunch of ``learners`` and corresponding ``fnames`` such that they can be loaded, like:
+```python
+import adaptive
+from functools import partial
 
-.. code-block:: python
+def h(x, pow, a):
+    return a * x**pow
 
-   import adaptive
-   from functools import partial
+combos = adaptive.utils.named_product(
+    pow=[0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
+    a=[0.1, 0.5],
+)  # returns list of dicts, cartesian product of all values
 
-   def h(x, pow, a):
-       return a * x**pow
+learners = [adaptive.Learner1D(partial(h, **combo),
+            bounds=(-1, 1)) for combo in combos]
+fnames = [f"data/{combo}" for combo in combos]
+```
 
-   combos = adaptive.utils.named_product(
-       pow=[0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
-       a=[0.1, 0.5],
-   )  # returns list of dicts, cartesian product of all values
+Then you start a process that creates and submits as many job-scripts as there are learners, like:
 
-   learners = [adaptive.Learner1D(partial(h, **combo),
-               bounds=(-1, 1)) for combo in combos]
-   fnames = [f"data/{combo}" for combo in combos]
+```python
+import adaptive_scheduler
 
+def goal(learner):
+    return learner.npoints > 200
 
-Then you start a process that creates and submits as many job-scripts as there are learners. Like:
+scheduler = adaptive_scheduler.scheduler.SLURM(cores=10)  # every learner gets this many cores
 
-.. code-block:: python
+run_manager = adaptive_scheduler.server_support.RunManager(
+    scheduler,
+    learners,
+    fnames,
+    goal=goal,
+    log_interval=30,  # write info such as npoints, cpu_usage, time, etc. to the job log file
+    save_interval=300,  # save the data every 300 seconds
+)
+run_manager.start()
+```
 
-   import adaptive_scheduler
+That's it! You can run `run_manager.info()` which will display an interactive `ipywidget` that shows the amount of running, pending, and finished jobs, buttons to cancel your job, and other useful information.
 
-   def goal(learner):
-       return learner.npoints > 200
+![Widget demo](https://user-images.githubusercontent.com/6897215/232347580-37f8faa9-53f0-45f5-a34b-856cd8e62b83.gif)
 
-   scheduler = adaptive_scheduler.scheduler.SLURM(cores=10)  # every learner get this many cores
+## :mag: But how does it *really* work?
 
-   run_manager = adaptive_scheduler.server_support.RunManager(
-       scheduler,
-       learners,
-       fnames,
-       goal=goal,
-       log_interval=30,  #  write info such as npoints, cpu_usage, time, etc. to the job log file
-       save_interval=300,  # save the data every 300 seconds
-   )
-   run_manager.start()
+The `adaptive_scheduler.server_support.RunManager` basically does the following:
 
+- *You* need to create `N` `learners` and `fnames` (like in the section above).
+- Then a "job manager" writes and submits `max(N, max_simultaneous_jobs)` job scripts but *doesn't know* which learner it is going to run!
+- This is the responsibility of the "database manager", which keeps a database of `job_id <--> learner`.
+- The job script starts a Python file `run_learner.py` in which the learner is run.
 
-That's it! You can run ``run_manager.info()`` which will display an interactive ``ipywidget`` that shows the amount of running, pending, and finished jobs, buttons to cancel your job, and other useful information.
+In a Jupyter notebook, you can start the "job manager" and the "database manager", and create the `run_learner.py` like:
 
-.. image:: http://files.nijho.lt/info.gif
-   :target: http://files.nijho.lt/info.gif
-   :alt: Widget demo
+```python
+import adaptive_scheduler
+from adaptive_scheduler import server_support
 
+# create a scheduler
+scheduler = adaptive_scheduler.scheduler.SLURM(cores=10)
 
+# create a new database that keeps track of job <-> learner
+db_fname = "running.json"
+url = (
+   server_support.get_allowed_url()
+)  # get a url where we can run the database_manager
+database_manager = server_support.DatabaseManager(
+   url, scheduler, db_fname, learners, fnames
+)
+database_manager.start()
 
-But how does it *really* work?
-------------------------------
+# create unique names for the jobs
+n_jobs = len(learners)
+job_names = [f"test-job-{i}" for i in range(n_jobs)]
 
-The `~adaptive_scheduler.server_support.RunManager` basically does the following.
-So, *you* need to create ``N`` ``learners`` and ``fnames`` (like in the section above).
-Then a "job manager" writes and submits ``max(N, max_simultaneous_jobs)`` job scripts but *doesn't know* which learner it is going to run!
-This is the responsibility of the "database manager", which keeps a database of ``job_id <--> learner``.
-The job script starts a Python file ``run_learner.py`` in which the learner is run.
+job_manager = server_support.JobManager(
+    job_names,
+    database_manager,
+    scheduler,
+    save_interval=300,
+    log_interval=30,
+    goal=0.01,
+)
+job_manager.start()
+```
 
+Then, when the jobs have been running for a while, you can check `server_support.parse_log_files(database_manager, scheduler)`.
 
-In a Jupyter notebook we can start the "job manager" and the "database manager", and create the ``run_learner.py`` like:
+And use `scheduler.cancel(job_names)` to cancel the jobs.
 
-.. code-block:: python
+You don't actually ever have to leave the Jupyter notebook; take a look at the [`example notebook`](https://github.com/basnijholt/adaptive-scheduler/blob/main/example.ipynb).
 
-   import adaptive_scheduler
-   from adaptive_scheduler import server_support
+## :notebook: Jupyter Notebook Example
 
-   # create a scheduler
-   scheduler = adaptive_scheduler.scheduler.SLURM(cores=10, run_script="run_learner.py",)
+See [`example.ipynb`](https://github.com/basnijholt/adaptive-scheduler/blob/main/example.ipynb).
 
-   # create a new database that keeps track of job <-> learner
-   db_fname = "running.json"
-   url = (
-      server_support.get_allowed_url()
-   )  # get a url where we can run the database_manager
-   database_manager = server_support.DatabaseManager(
-      url, scheduler, db_fname, learners, fnames
-   )
-   database_manager.start()
+## :computer: Installation
 
-   # create the Python script that runs a learner (run_learner.py)
-   server_support._make_default_run_script(
-      url=url,
-      save_interval=300,
-      log_interval=30,
-      goal=None,
-      executor_type=scheduler.executor_type,
-      run_script_fname=scheduler.run_script,
-   )
+Install the **latest stable** version from conda (recommended):
 
-   # create unique names for the jobs
-   n_jobs = len(learners)
-   job_names = [f"test-job-{i}" for i in range(n_jobs)]
+```bash
+conda install adaptive-scheduler
+```
 
-   job_manager = server_support.JobManager(job_names, database_manager, scheduler)
-   job_manager.start()
+or from PyPI:
 
+```bash
+pip install adaptive_scheduler
+```
 
-Then when the job have been running for a while you can check ``server_support.parse_log_files(job_names, database_manager, scheduler)``.
+or install **main** with:
 
-And use ``scheduler.cancel(job_names)`` to cancel the jobs.
+```bash
+pip install -U https://github.com/basnijholt/adaptive-scheduler/archive/main.zip
+```
 
-You don't actually ever have to leave the Jupter notebook, take a look at the `example notebook <https://github.com/basnijholt/adaptive-scheduler/blob/master/example.ipynb>`_.
+or clone the repository and do a dev install (recommended for dev):
 
-Jupyter notebook example
-------------------------
+```bash
+git clone git@github.com:basnijholt/adaptive-scheduler.git
+cd adaptive-scheduler
+pip install -e .
+```
 
-See `example.ipynb <https://github.com/basnijholt/adaptive-scheduler/blob/master/example.ipynb>`_.
+## :hammer_and_wrench: Development
 
-Installation
-------------
-
-**WARNING:** This is still the pre-alpha development stage.
-
-Install the **latest stable** version from conda with (recommended)
-
-.. code-block:: bash
-
-   conda install adaptive-scheduler
-
-
-or from PyPI with
-
-.. code-block:: bash
-
-   pip install adaptive_scheduler
-
-
-or install **master** with
-
-.. code-block:: bash
-
-   pip install -U https://github.com/basnijholt/adaptive-scheduler/archive/master.zip
-
-
-or clone the repository and do a dev install (recommended for dev)
-
-.. code-block:: bash
-
-   git clone git@github.com:basnijholt/adaptive-scheduler.git
-   cd adaptive-scheduler
-   pip install -e .
-
-
-Development
------------
-
-In order to not pollute the history with the output of the notebooks, please setup the git filter by executing
-
-.. code-block:: bash
-
-   python ipynb_filter.py
+In order not to pollute the history with the output of the notebooks, please set up the git filter by executing:
 
+```bash
+python ipynb_filter.py
+```
 
 in the repository.
 
-We also use `pre-commit <https://pre-commit.com>`_\ , so ``pip install pre_commit`` and run
-
-.. code-block:: bash
-
-   pre-commit install
+We also use `pre-commit`, so `pip install pre_commit` and run:
 
+```bash
+pre-commit install
+```
 
 in the repository.
 
-Limitations
------------
-
-Right now ``adaptive_scheduler`` is only working for SLURM and PBS, however only a class like `adaptive_scheduler/scheduler.py <https://github.com/basnijholt/adaptive-scheduler/blob/master/adaptive_scheduler/scheduler.py#L471>`_ would have to be implemented for another type of scheduler.
-Also there are **no tests** at all!
+## :warning: Limitations
 
-.. references-start
-.. |PyPI| image:: https://img.shields.io/pypi/v/adaptive-scheduler.svg
-   :target: https://pypi.python.org/pypi/adaptive-scheduler
-   :alt: PyPI
-.. |Conda| image:: https://anaconda.org/conda-forge/adaptive-scheduler/badges/installer/conda.svg
-   :target: https://anaconda.org/conda-forge/adaptive-scheduler
-   :alt: Conda
-.. |Downloads| image:: https://anaconda.org/conda-forge/adaptive-scheduler/badges/downloads.svg
-   :target: https://anaconda.org/conda-forge/adaptive-scheduler
-   :alt: Downloads
-.. |Build Status| image:: https://github.com/basnijholt/adaptive-scheduler/actions/workflows/pytest.yml/badge.svg
-   :target: https://github.com/basnijholt/adaptive-scheduler/actions/workflows/pytest.yml
-   :alt: Build Status
-.. |Documentation Status| image:: https://readthedocs.org/projects/adaptive-scheduler/badge/?version=latest
-   :target: https://adaptive-scheduler.readthedocs.io/en/latest/?badge=latest
-   :alt: Documentation Status
-.. references-end
+Currently, `adaptive_scheduler` only works for SLURM and PBS.
+However, only a class like [`adaptive_scheduler/scheduler.py`](https://github.com/basnijholt/adaptive-scheduler/blob/main/adaptive_scheduler/scheduler.py#L471) would have to be implemented for another type of scheduler.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `adaptive_scheduler-1.8.0/adaptive_scheduler/_mock_scheduler.py` & `adaptive_scheduler-2.0.0/adaptive_scheduler/_mock_scheduler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,41 @@
+#!/usr/bin/env python
 from __future__ import annotations
 
 import asyncio
 import datetime
 import logging
 import os
 import subprocess
-from typing import Coroutine
+from typing import TYPE_CHECKING, List, Tuple, Union
 
 import structlog
 import zmq
 import zmq.asyncio
 from toolz.dicttoolz import dissoc
 
+if TYPE_CHECKING:
+    from collections.abc import Coroutine
+    from typing import Any
+
 ctx = zmq.asyncio.Context()
 
 logger = logging.getLogger("adaptive_scheduler._mock_scheduler")
 logger.setLevel(logging.INFO)
 log = structlog.wrap_logger(logger)
 
 DEFAULT_URL = "tcp://127.0.0.1:60547"
 
+_RequestSubmitType = Tuple[str, str, Union[str, List[str]]]
+_RequestCancelType = Tuple[str, str]
+_RequestQueueType = Tuple[str]
+
 
 class MockScheduler:
-    f"""Emulates a HPC-like scheduler.
+    """Emulates a HPC-like scheduler.
 
     Start an instance of `MockScheduler` and then you are able to do
     ```
     python _mock_scheduler.py --queue
     python _mock_scheduler.py --submit JOB_NAME_HERE script_here.sh  # returns JOB_ID
     python _mock_scheduler.py --cancel JOB_ID
     ```
@@ -43,151 +52,162 @@
         ``bash`` executable.
     url : str, optional
         The URL of the socket. Defaults to {DEFAULT_URL}.
     """
 
     def __init__(
         self,
-        startup_delay=3,
-        max_running_jobs=4,
-        refresh_interval=0.1,
-        bash="bash",
-        url=None,
-    ):
-        self._current_queue = {}
+        *,
+        startup_delay: int = 3,
+        max_running_jobs: int = 4,
+        refresh_interval: float = 0.1,
+        bash: str = "bash",
+        url: str | None = None,
+    ) -> None:
+        self._current_queue: dict[str, dict[str, Any]] = {}
         self._job_id = 0
         self.max_running_jobs = max_running_jobs
         self.startup_delay = startup_delay
         self.refresh_interval = refresh_interval
         self.bash = bash
         self.ioloop = asyncio.get_event_loop()
         self.refresh_task = self.ioloop.create_task(self._refresh_coro())
         self.url = url or DEFAULT_URL
         self.command_listener_task = self.ioloop.create_task(self._command_listener())
 
-    def queue(self, only_me: bool = True):
-        # only_me doesn't do anything, but the argument is there
+    def queue(
+        self,
+        *,
+        me_only: bool = True,  # noqa: ARG002
+    ) -> dict[str, dict[str, Any]]:
+        """Return the current queue."""
+        # me_only doesn't do anything, but the argument is there
         # because it is in the other schedulers.
 
         # remove the "proc" entries because they aren't pickable
         return {
             job_id: dissoc(info, "proc") for job_id, info in self._current_queue.items()
         }
 
-    def _queue_is_full(self):
+    def _queue_is_full(self) -> bool:
         n_running = sum(info["state"] == "R" for info in self._current_queue.values())
         return n_running >= self.max_running_jobs
 
-    def _get_new_job_id(self):
+    def _get_new_job_id(self) -> str:
         job_id = self._job_id
         self._job_id += 1
         return str(job_id)
 
-    async def _submit_coro(self, job_id: str, fname: str):
+    async def _submit_coro(self, job_id: str, fname: str) -> None:
         await asyncio.sleep(self.startup_delay)
         while self._queue_is_full():
             await asyncio.sleep(self.refresh_interval)
         self._submit(job_id, fname)
 
-    def _submit(self, job_id: str, fname: str):
+    def _submit(self, job_id: str, fname: str) -> None:
         if job_id in self._current_queue:
             # job_id could be cancelled before it started
             cmd = f"{self.bash} {fname}"
             proc = subprocess.Popen(
-                cmd.split(), stdout=subprocess.PIPE, env=dict(os.environ, JOB_ID=job_id)
+                cmd.split(),
+                stdout=subprocess.PIPE,
+                env=dict(os.environ, JOB_ID=job_id),
             )
             info = self._current_queue[job_id]
             info["proc"] = proc
             info["state"] = "R"
 
-    def submit(self, job_name: str, fname: str):
+    def submit(self, job_name: str, fname: str) -> str:
         job_id = self._get_new_job_id()
         self._current_queue[job_id] = {
             "job_name": job_name,
             "proc": None,
             "state": "P",
-            "timestamp": str(datetime.datetime.now()),
+            "timestamp": str(datetime.datetime.now()),  # noqa: DTZ005
         }
         self.ioloop.create_task(self._submit_coro(job_id, fname))
         return job_id
 
-    def cancel(self, job_id: str):
+    def cancel(self, job_id: str) -> None:
         job_id = str(job_id)
         info = self._current_queue.pop(job_id)
         if info["proc"] is not None:
             info["proc"].kill()
 
-    async def _refresh_coro(self):
+    async def _refresh_coro(self) -> Coroutine[None, None, None]:
         while True:
             try:
                 await asyncio.sleep(self.refresh_interval)
                 self._refresh()
-            except Exception as e:
+            except Exception as e:  # noqa: BLE001
                 print(e)
 
-    def _refresh(self):
-        for job_id, info in self._current_queue.items():
+    def _refresh(self) -> None:
+        for _job_id, info in self._current_queue.items():
             if info["state"] == "R" and info["proc"].poll() is not None:
                 info["state"] = "F"
 
-    async def _command_listener(self) -> Coroutine:
+    async def _command_listener(self) -> Coroutine[None, None, None]:
         log.debug("started _command_listener")
         socket = ctx.socket(zmq.REP)
         socket.bind(self.url)
         try:
             while True:
                 request = await socket.recv_pyobj()
                 reply = self._dispatch(request)
                 await socket.send_pyobj(reply)
         finally:
             socket.close()
 
-    def _dispatch(self, request: tuple[str, ...]):
+    def _dispatch(
+        self,
+        request: _RequestSubmitType | _RequestCancelType | _RequestQueueType,
+    ) -> str | None | dict[str, dict[str, Any]] | Exception:
         log.debug("got a request", request=request)
         request_type, *request_arg = request
         try:
             if request_type == "submit":
                 job_name, fname = request_arg
                 log.debug("submitting a task", fname=fname, job_name=job_name)
-                job_id = self.submit(job_name, fname)
+                job_id = self.submit(job_name, fname)  # type: ignore[arg-type]
                 return job_id
-            elif request_type == "cancel":
-                job_id = request_arg[0]
+            if request_type == "cancel":
+                job_id = request_arg[0]  # type: ignore[assignment]
                 log.debug("got a cancel request", job_id=job_id)
                 self.cancel(job_id)
                 return None
-            elif request_type == "queue":
+            if request_type == "queue":
                 log.debug("got a queue request")
                 return self._current_queue
-            else:
-                log.debug("got unknown request")
-        except Exception as e:
+            log.debug("got unknown request")
+        except Exception as e:  # noqa: BLE001
             return e
+        msg = f"unknown request_type: {request_type}"
+        raise ValueError(msg)
 
 
-def _external_command(command: tuple[str, ...], url: str):
-    async def _coro(command, url) -> None:
+def _external_command(command: tuple[str, ...], url: str) -> Any:
+    async def _coro(command: tuple[str, ...], url: str) -> None:
         with ctx.socket(zmq.REQ) as socket:
             socket.setsockopt(zmq.RCVTIMEO, 2000)
             socket.connect(url)
             await socket.send_pyobj(command)
-            reply = await socket.recv_pyobj()
-            return reply
+            return await socket.recv_pyobj()
 
     coro = _coro(command, url)
     ioloop = asyncio.get_event_loop()
     task = ioloop.create_task(coro)
     return ioloop.run_until_complete(task)
 
 
-def queue(url: str = DEFAULT_URL):
+def queue(url: str = DEFAULT_URL) -> dict[str, dict[str, Any]]:
     return _external_command(("queue",), url)
 
 
-def submit(job_name: str, fname: str, url: str = DEFAULT_URL) -> None:
+def submit(job_name: str, fname: str, url: str = DEFAULT_URL) -> Any:
     return _external_command(("submit", job_name, fname), url)
 
 
 def cancel(job_id: str, url: str = DEFAULT_URL) -> None:
     return _external_command(("cancel", job_id), url)
```

### Comparing `adaptive_scheduler-1.8.0/adaptive_scheduler/client_support.py` & `adaptive_scheduler-2.0.0/adaptive_scheduler/client_support.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,65 @@
+"""Client support for Adaptive Scheduler."""
 from __future__ import annotations
 
-import asyncio
 import datetime
 import logging
 import socket
 from contextlib import suppress
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 import psutil
 import structlog
 import zmq
-from adaptive import AsyncRunner, BaseLearner
 
 from adaptive_scheduler.utils import (
     _deserialize,
     _get_npoints,
     _serialize,
     fname_to_learner,
     log_exception,
-    maybe_lst,
+    sleep_unless_task_is_done,
 )
 
+if TYPE_CHECKING:
+    import asyncio
+    from pathlib import Path
+
+    from adaptive import AsyncRunner, BaseLearner
+
+
 ctx = zmq.Context()
 logger = logging.getLogger("adaptive_scheduler.client")
 logger.setLevel(logging.INFO)
 log = structlog.wrap_logger(
     logger,
     processors=[
         structlog.processors.StackInfoRenderer(),
         structlog.processors.format_exc_info,
         structlog.processors.TimeStamper(fmt="%Y-%m-%d %H:%M.%S", utc=False),
         structlog.processors.JSONRenderer(),
     ],
 )
 
 
-def _add_log_file_handler(log_fname):
+def _add_log_file_handler(log_fname: str | Path) -> None:  # pragma: no cover
     fh = logging.FileHandler(log_fname)
     logger.addHandler(fh)
 
 
 def get_learner(
-    url: str, log_fname: str, job_id: str, job_name: str
+    url: str,
+    log_fname: str,
+    job_id: str,
+    job_name: str,
 ) -> tuple[BaseLearner, str | list[str]]:
-    """Get a learner from the database running at `url` and this learner's
-    process will be logged in `log_fname` and running under `job_id`.
+    """Get a learner from the database (running at `url`).
+
+    This learner's process will be logged in `log_fname`
+    and running under `job_id`.
 
     Parameters
     ----------
     url : str
         The url of the database manager running via
         (`adaptive_scheduler.server_support.manage_database`).
     log_fname : str
@@ -63,43 +74,45 @@
     learner : `adaptive.BaseLearner`
         Learner that is chosen.
     fname : str
         The filename of the learner that was chosen.
     """
     _add_log_file_handler(log_fname)
     log.info(
-        "trying to get learner", job_id=job_id, log_fname=log_fname, job_name=job_name
+        "trying to get learner",
+        job_id=job_id,
+        log_fname=log_fname,
+        job_name=job_name,
     )
     with ctx.socket(zmq.REQ) as socket:
         socket.setsockopt(zmq.LINGER, 0)
         socket.setsockopt(zmq.SNDTIMEO, 300_000)  # timeout after 300s
         socket.connect(url)
         socket.send_serialized(("start", job_id, log_fname, job_name), _serialize)
-        log.info("sent start signal, going to wait 60s for a reply.")
+        log.info("sent start signal, going to wait 300s for a reply.")
         socket.setsockopt(zmq.RCVTIMEO, 300_000)  # timeout after 300s
         reply = socket.recv_serialized(_deserialize)
         log.info("got reply", reply=str(reply))
         if reply is None:
             msg = "No learners to be run."
             exception = RuntimeError(msg)
             log_exception(log, msg, exception)
             raise exception
-        elif isinstance(reply, Exception):
+        if isinstance(reply, Exception):
             log_exception(log, "got an exception", exception=reply)
             raise reply
-        else:
-            fname = reply
-            learner = fname_to_learner(fname)
-            log.info("got fname and loaded learner")
+        fname = reply
+        learner = fname_to_learner(fname)
+        log.info("got fname and loaded learner")
 
     log.info("picked a learner")
-    return learner, maybe_lst(fname)
+    return learner, fname
 
 
-def tell_done(url: str, fname: str) -> None:
+def tell_done(url: str, fname: str | list[str]) -> None:
     """Tell the database that the learner has reached it's goal.
 
     Parameters
     ----------
     url : str
         The url of the database manager running via
         (`adaptive_scheduler.server_support.manage_database`).
@@ -116,55 +129,65 @@
         log.info("sent stop signal, going to wait 300s for a reply", fname=fname)
         socket.recv_serialized(_deserialize)  # Needed because of socket type
 
 
 def _get_log_entry(runner: AsyncRunner, npoints_start: int) -> dict[str, Any]:
     learner = runner.learner
     info: dict[str, int | float | str] = {}
-    Δt = datetime.timedelta(seconds=runner.elapsed_time())
+    Δt = datetime.timedelta(seconds=runner.elapsed_time())  # noqa: N806
     info["elapsed_time"] = str(Δt)
     info["overhead"] = runner.overhead()
     npoints = _get_npoints(learner)
     if npoints is not None:
-        info["npoints"] = _get_npoints(learner)
-        Δnpoints = npoints - npoints_start
+        info["npoints"] = npoints
+        Δnpoints = npoints - npoints_start  # noqa: N806
         with suppress(ZeroDivisionError):
             # Δt.seconds could be zero if the job is done when starting
             info["npoints/s"] = Δnpoints / Δt.seconds
     with suppress(Exception):
         info["latest_loss"] = learner._cache["loss"]
     with suppress(AttributeError):
         info["nlearners"] = len(learner.learners)
         if "npoints" in info:
-            info["npoints/learner"] = info["npoints"] / info["nlearners"]
+            info["npoints/learner"] = info["npoints"] / info["nlearners"]  # type: ignore[operator]
     info["cpu_usage"] = psutil.cpu_percent()
     info["mem_usage"] = psutil.virtual_memory().percent
+    for k, v in psutil.cpu_times()._asdict().items():
+        info[f"cputimes.{k}"] = v
     return info
 
 
-def log_info(runner: AsyncRunner, interval=300) -> asyncio.Task:
+def log_now(runner: AsyncRunner, npoints_start: int) -> None:
+    """Create a log message now."""
+    info = _get_log_entry(runner, npoints_start)
+    log.info("current status", **info)
+
+
+def log_info(runner: AsyncRunner, interval: int | float = 300) -> asyncio.Task:
     """Log info in the job's logfile, similar to `runner.live_info`.
 
     Parameters
     ----------
     runner : `adaptive.Runner` instance
-    interval : int, default: 300
+        Adaptive Runner instance.
+    interval : int | float, default: 300
         Time in seconds between log entries.
 
     Returns
     -------
     asyncio.Task
     """
 
-    async def coro(runner, interval):
-        log.info(f"started logger on hostname {socket.gethostname()}")
+    async def coro(runner: AsyncRunner, interval: int | float) -> None:
+        log.info(f"started logger on hostname {socket.gethostname()}")  # noqa: G004
         learner = runner.learner
         npoints_start = _get_npoints(learner)
+        assert npoints_start is not None
         log.info("npoints at start", npoints=npoints_start)
         while runner.status() == "running":
-            await asyncio.sleep(interval)
-            info = _get_log_entry(runner, npoints_start)
-            log.info("current status", **info)
+            if await sleep_unless_task_is_done(runner.task, interval):
+                break
+            log_now(runner, npoints_start)
         log.info("runner status changed", status=runner.status())
         log.info("current status", **_get_log_entry(runner, npoints_start))
 
     return runner.ioloop.create_task(coro(runner, interval))
```

### Comparing `adaptive_scheduler-1.8.0/adaptive_scheduler/scheduler.py` & `adaptive_scheduler-2.0.0/adaptive_scheduler/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,969 +1,1143 @@
+"""Utility functions for adaptive_scheduler."""
 from __future__ import annotations
 
-import abc
-import collections
-import getpass
+import asyncio
+import base64
+import functools
+import hashlib
+import inspect
 import math
 import os
-import os.path
-import re
-import subprocess
-import sys
-import textwrap
+import pickle
+import platform
+import random
+import shutil
+import tempfile
 import time
 import warnings
-from distutils.spawn import find_executable
-from functools import cached_property, lru_cache
-from typing import Literal
-
+from concurrent.futures import ThreadPoolExecutor
+from contextlib import suppress
+from datetime import datetime, timedelta, timezone
+from inspect import signature
+from multiprocessing import Manager
+from pathlib import Path
+from typing import TYPE_CHECKING, Any, Callable, List, Literal, Union
+
+import adaptive
+import cloudpickle
+import numpy as np
+import pandas as pd
+import toolz
+from adaptive.notebook_integration import in_ipynb
 from rich.console import Console
+from tqdm import tqdm, tqdm_notebook
 
-import adaptive_scheduler._mock_scheduler
-from adaptive_scheduler.utils import _progress, _RequireAttrsABCMeta
+if TYPE_CHECKING:
+    from collections.abc import Iterable, Sequence
+    from multiprocessing.managers import ListProxy
 
 console = Console()
 
+MAX_LINE_LENGTH = 100
+_NONE_RETURN_STR = "__ReturnsNone__"
+FnamesTypes = Union[List[str], List[Path], List[List[str]], List[List[Path]]]
+
+LOKY_START_METHODS = Literal[
+    "loky",
+    "loky_int_main",
+    "spawn",
+    "fork",
+    "forkserver",
+]
+
+EXECUTOR_TYPES = Literal["mpi4py", "ipyparallel", "dask-mpi", "process-pool", "loky"]
+GoalTypes = Union[
+    Callable[[adaptive.BaseLearner], bool],
+    int,
+    float,
+    datetime,
+    timedelta,
+    None,
+]
+
+
+def shuffle_list(*lists: list, seed: int | None = 0) -> zip | zip:
+    """Shuffle multiple lists in the same order."""
+    combined = list(zip(*lists))
+    random.Random(seed).shuffle(combined)
+    return zip(*combined)
+
+
+def hash_anything(x: Any) -> str:
+    """Hash anything."""
+    try:
+        return hashlib.md5(x).hexdigest()  # noqa: S324
+    except TypeError:
+        return hashlib.md5(pickle.dumps(x)).hexdigest()  # noqa: S324
 
-def _run_submit(cmd, name=None):
-    env = os.environ.copy()
-    if name is not None:
-        env["NAME"] = name
-    for _ in range(10):
-        proc = subprocess.run(cmd.split(), env=env, capture_output=True)
-        if proc.returncode == 0:
-            return
-        stderr = proc.stderr.decode()
-        if stderr != "":
-            console.log(f"Error: {stderr}")
-        time.sleep(0.5)
-
-
-class BaseScheduler(metaclass=_RequireAttrsABCMeta):
-    """Base object for a Scheduler.
+
+def split(seq: Iterable, n_parts: int) -> Iterable[tuple]:
+    """Split up a sequence into ``n_parts``.
 
     Parameters
     ----------
-    cores : int
-        Number of cores per job (so per learner.)
-    run_script : str
-        Filename of the script that is run on the nodes. Inside this script we
-        query the database and run the learner.
-    python_executable : str, default: `sys.executable`
-        The Python executable that should run the `run_script`. By default
-        it uses the same Python as where this function is called.
-    log_folder : str, default: ""
-        The folder in which to put the log-files.
-    mpiexec_executable : str, optional
-        ``mpiexec`` executable. By default `mpiexec` will be
-        used (so probably from ``conda``).
-    executor_type : str, default: "mpi4py"
-        The executor that is used, by default `mpi4py.futures.MPIPoolExecutor` is used.
-        One can use ``"ipyparallel"``, ``"dask-mpi"``, ``"mpi4py"``, or ``"process-pool"``.
-    num_threads : int, default 1
-        ``MKL_NUM_THREADS``, ``OPENBLAS_NUM_THREADS``, ``OMP_NUM_THREADS``, and
-        ``NUMEXPR_NUM_THREADS`` will be set to this number.
-    extra_scheduler : list, optional
-        Extra ``#SLURM`` (depending on scheduler type)
-        arguments, e.g. ``["--exclusive=user", "--time=1"]``.
-    extra_env_vars : list, optional
-        Extra environment variables that are exported in the job
-        script. e.g. ``["TMPDIR='/scratch'", "PYTHONPATH='my_dir:$PYTHONPATH'"]``.
-    extra_script : str, optional
-        Extra script that will be executed after any environment variables are set,
-        but before the main scheduler is run.
+    seq : sequence
+        A list or other iterable that has to be split up.
+    n_parts : int
+        The sequence will be split up in this many parts.
 
     Returns
     -------
-    `BaseScheduler` object.
+    iterable of tuples
     """
+    lst = list(seq)
+    n = math.ceil(len(lst) / n_parts)
+    return toolz.partition_all(n, lst)
 
-    required_attributes = ["_ext", "_submit_cmd", "_options_flag", "_cancel_cmd"]
 
-    def __init__(
-        self,
-        cores,
-        run_script,
-        python_executable,
-        log_folder,
-        mpiexec_executable,
-        executor_type: Literal["ipyparallel", "dask-mpi", "mpi4py", "process-pool"],
-        num_threads,
-        extra_scheduler,
-        extra_env_vars,
-        extra_script,
-    ):
-        self.cores = cores
-        self.run_script = run_script
-        self.python_executable = python_executable or sys.executable
-        self.log_folder = log_folder
-        self.mpiexec_executable = mpiexec_executable or "mpiexec"
-        self.executor_type = executor_type
-        self.num_threads = num_threads
-        self._extra_scheduler = extra_scheduler
-        self._extra_env_vars = extra_env_vars
-        self._extra_script = extra_script if extra_script is not None else ""
-        self._JOB_ID_VARIABLE = "${JOB_ID}"
-
-    @abc.abstractmethod
-    def queue(self, me_only: bool) -> dict[str, dict]:
-        """Get the current running and pending jobs.
+def split_in_balancing_learners(
+    learners: list[adaptive.BaseLearner],
+    fnames: list[str] | list[Path],
+    n_parts: int,
+    strategy: str = "npoints",
+) -> tuple[list[adaptive.BaseLearner], list[list[str]] | list[list[Path]]]:
+    r"""Split a list of learners and fnames into `adaptive.BalancingLearner`\s.
 
-        Parameters
-        ----------
-        me_only : bool, default: True
-            Only see your jobs.
+    Parameters
+    ----------
+    learners : list
+        List of learners.
+    fnames : list
+        List of filenames.
+    n_parts : int
+        Total number of `~adaptive.BalancingLearner`\s.
+    strategy : str
+        Learning strategy of the `~adaptive.BalancingLearner`.
 
-        Returns
-        -------
-        queue : dict
-            Mapping of ``job_id`` -> `dict` with ``name`` and ``state``, for
-            example ``{job_id: {"job_name": "TEST_JOB-1", "state": "R" or "Q"}}``.
-
-        Notes
-        -----
-        This function might return extra information about the job, however
-        this is not used elsewhere in this package.
-        """
+    Returns
+    -------
+    new_learners, new_fnames
+    """
+    new_learners = []
+    new_fnames = []
+    for x in split(zip(learners, fnames), n_parts):
+        learners_part, fnames_part = zip(*x)
+        learner = adaptive.BalancingLearner(learners_part, strategy=strategy)
+        new_learners.append(learner)
+        new_fnames.append(fnames_part)
+    return new_learners, new_fnames
+
+
+def split_sequence_learner(
+    big_learner: adaptive.SequenceLearner,
+    n_learners: int,
+    folder: str | Path = "",
+) -> tuple[list[adaptive.SequenceLearner], list[str]]:
+    r"""Split a sinlge `~adaptive.SequenceLearner` into many.
 
-    @property
-    def ext(self) -> str:
-        """The extension of the job script."""
-        return self._ext
+    Split into mutiple `adaptive.SequenceLearner`\s
+    (with the data loaded) and fnames.
 
-    @property
-    def submit_cmd(self) -> str:
-        """Command to start a job, e.g. ``qsub fname.batch`` or ``sbatch fname.sbatch``."""
-        return self._submit_cmd
-
-    @abc.abstractmethod
-    def job_script(self) -> str:
-        """Get a jobscript in string form.
+    See also `split_sequence_in_sequence_learners`.
 
-        Returns
-        -------
-        job_script : str
-            A job script that can be submitted to the scheduler.
-        """
+    Parameters
+    ----------
+    big_learner
+        A `~adaptive.SequenceLearner` instance
+    n_learners : int
+        Total number of `~adaptive.SequenceLearner`\s.
+    folder : pathlib.Path or str
+        Folder to prepend to fnames.
 
-    def batch_fname(self, name: str) -> str:
-        """The filename of the job script."""
-        return os.path.abspath(name + self.ext)
-
-    @staticmethod
-    def sanatize_job_id(job_id):
-        return job_id
+    Returns
+    -------
+    new_learners : List[adaptive.SequenceLearner]
+        List of `~adaptive.SequenceLearner`\s.
+    new_fnames : List[Path]
+        List of str based on a hash of the sequence.
+    """
+    new_learners, new_fnames = split_sequence_in_sequence_learners(
+        function=big_learner._original_function,
+        sequence=big_learner.sequence,
+        n_learners=n_learners,
+        folder=folder,
+    )
+    # Load the new learners with data
+    index_parts = split(range(len(big_learner.sequence)), n_learners)
+    for small_learner, part in zip(new_learners, index_parts):
+        for i_small, i_big in enumerate(part):
+            y = big_learner.data.get(i_big)
+            if y is None:
+                continue
+            x = i_small, big_learner.sequence[i_big]
+            small_learner.tell(x, y)
+
+    return new_learners, new_fnames
+
+
+def split_sequence_in_sequence_learners(
+    function: Callable[[Any], Any],
+    sequence: Sequence[Any],
+    n_learners: int,
+    folder: str | Path = "",
+) -> tuple[list[adaptive.SequenceLearner], list[str]]:
+    r"""Split a sequenceinto `adaptive.SequenceLearner`\s and fnames.
 
-    def cancel(
-        self, job_names: list[str], with_progress_bar: bool = True, max_tries: int = 5
-    ) -> None:
-        """Cancel all jobs in `job_names`.
+    Parameters
+    ----------
+    function : callable
+        Function for `adaptive.SequenceLearner`\s.
+    sequence : sequence
+        The sequence to split into ``n_learners``.
+    n_learners : int
+        Total number of `~adaptive.SequenceLearner`\s.
+    folder : pathlib.Path or str
+        Folder to prepend to fnames.
 
-        Parameters
-        ----------
-        job_names : list
-            List of job names.
-        with_progress_bar : bool, default: True
-            Display a progress bar using `tqdm`.
-        max_tries : int, default: 5
-            Maximum number of attempts to cancel a job.
-        """
+    Returns
+    -------
+    new_learners : List[adaptive.SequenceLearner]
+        List of `~adaptive.SequenceLearner`\s.
+    new_fnames : List[Path]
+        List of str based on a hash of the sequence.
+    """
+    folder = Path(folder)
+    new_learners = []
+    new_fnames = []
+    for sequence_part in split(sequence, n_learners):
+        learner = adaptive.SequenceLearner(function, sequence_part)
+        new_learners.append(learner)
+        hsh = hash_anything((sequence_part[0], len(sequence_part)))
+        fname = folder / f"{hsh}.pickle"
+        new_fnames.append(str(fname))
+    return new_learners, new_fnames
+
+
+def combine_sequence_learners(
+    learners: list[adaptive.SequenceLearner],
+    big_learner: adaptive.SequenceLearner | None = None,
+) -> adaptive.SequenceLearner:
+    r"""Combine several `~adaptive.SequenceLearner`\s into a single one.
 
-        def to_cancel(job_names):
-            return [
-                job_id
-                for job_id, info in self.queue().items()
-                if info["job_name"] in job_names
-            ]
-
-        def cancel_jobs(job_ids):
-            for job_id in _progress(job_ids, with_progress_bar, "Canceling jobs"):
-                cmd = f"{self._cancel_cmd} {job_id}".split()
-                returncode = subprocess.run(cmd, stderr=subprocess.PIPE).returncode
-                if returncode != 0:
-                    warnings.warn(f"Couldn't cancel '{job_id}'.", UserWarning)
-
-        job_names = set(job_names)
-        for _ in range(max_tries):
-            job_ids = to_cancel(job_names)
-            if not job_ids:
-                # no more running jobs
-                break
-            cancel_jobs(job_ids)
-            time.sleep(0.5)
-
-    def _mpi4py(self, name: str) -> str:
-        log_fname = self.log_fname(name)
-        return f"{self.mpiexec_executable} -n {self.cores} {self.python_executable} -m mpi4py.futures {self.run_script} --log-fname {log_fname} --job-id {self._JOB_ID_VARIABLE} --name {name}"
-
-    def _dask_mpi(self, name: str) -> str:
-        log_fname = self.log_fname(name)
-        return f"{self.mpiexec_executable} -n {self.cores} {self.python_executable} {self.run_script} --log-fname {log_fname} --job-id {self._JOB_ID_VARIABLE} --name {name}"
-
-    def _ipyparallel(self, name: str) -> str:
-        log_fname = self.log_fname(name)
-        job_id = self._JOB_ID_VARIABLE
-        profile = "${profile}"
-        return textwrap.dedent(
-            f"""\
-            profile=adaptive_scheduler_{job_id}
-
-            echo "Creating profile {profile}"
-            ipython profile create {profile}
-
-            echo "Launching controller"
-            ipcontroller --ip="*" --profile={profile} --log-to-file &
-            sleep 10
-
-            echo "Launching engines"
-            {self.mpiexec_executable} -n {self.cores-1} ipengine --profile={profile} --mpi --cluster-id='' --log-to-file &
-
-            echo "Starting the Python script"
-            {self.python_executable} {self.run_script} --profile {profile} --n {self.cores-1} --log-fname {log_fname} --job-id {job_id} --name {name}
-            """
-        )
+    Also copy over the data.
 
-    def _process_pool(self, name: str) -> str:
-        log_fname = self.log_fname(name)
-        return f"{self.python_executable} {self.run_script} --n {self.cores} --log-fname {log_fname} --job-id {self._JOB_ID_VARIABLE} --name {name}"
-
-    def _executor_specific(self, name: str) -> str:
-        if self.executor_type == "mpi4py":
-            return self._mpi4py(name)
-        elif self.executor_type == "dask-mpi":
-            return self._dask_mpi(name)
-        elif self.executor_type == "ipyparallel":
-            if self.cores <= 1:
-                raise ValueError(
-                    "`ipyparalllel` uses 1 cores of the `adaptive.Runner` and"
-                    " the rest of the cores for the engines, so use more than 1 core."
-                )
-            return self._ipyparallel(name)
-        elif self.executor_type == "process-pool":
-            return self._process_pool(name)
-        else:
-            raise NotImplementedError(
-                "Use 'ipyparallel', 'dask-mpi', 'mpi4py' or 'process-pool'."
-            )
+    Assumes that all ``learners`` take the same function.
 
-    def log_fname(self, name: str) -> str:
-        """The filename of the log."""
-        if self.log_folder:
-            os.makedirs(self.log_folder, exist_ok=True)
-        return os.path.join(self.log_folder, f"{name}-{self._JOB_ID_VARIABLE}.log")
-
-    def output_fnames(self, name: str) -> list[str]:
-        log_fname = self.log_fname(name)
-        return [log_fname.replace(".log", ".out")]
+    Parameters
+    ----------
+    learners : List[adaptive.SequenceLearner]
+        List of `~adaptive.SequenceLearner`\s.
+    big_learner : Optional[adaptive.SequenceLearner]
+        A learner to load, if None, a new learner will be generated.
 
-    @property
-    def extra_scheduler(self):
-        """Scheduler options that go in the job script."""
-        extra_scheduler = self._extra_scheduler or []
-        return "\n".join(f"#{self._options_flag} {arg}" for arg in extra_scheduler)
+    Returns
+    -------
+    adaptive.SequenceLearner
+        Big `~adaptive.SequenceLearner` with data from ``learners``.
+    """
+    if big_learner is None:
+        big_sequence: list[Any] = sum(
+            (list(learner.sequence) for learner in learners),
+            [],
+        )
+        big_learner = adaptive.SequenceLearner(
+            learners[0]._original_function,
+            sequence=big_sequence,
+        )
 
-    @property
-    def extra_env_vars(self):
-        """Environment variables that need to exist in the job script."""
-        extra_env_vars = self._extra_env_vars or []
-        return "\n".join(f"export {arg}" for arg in extra_env_vars)
+    cnt = 0
+    for learner in learners:
+        for i, key in enumerate(learner.sequence):
+            if i in learner.data:
+                x = cnt, key
+                y = learner.data[i]
+                big_learner.tell(x, y)
+            cnt += 1
+    return big_learner
+
+
+def copy_from_sequence_learner(
+    learner_from: adaptive.SequenceLearner,
+    learner_to: adaptive.SequenceLearner,
+) -> None:
+    """Copy the data from a `~adaptive.SequenceLearner` into a different one.
 
-    @property
-    def extra_script(self):
-        """Script that will be run before the main scheduler."""
-        return str(self._extra_script) or ""
-
-    def write_job_script(self, name: str) -> None:
-        with open(self.batch_fname(name), "w", encoding="utf-8") as f:
-            job_script = self.job_script()
-            f.write(job_script)
-
-    def start_job(self, name: str) -> None:
-        """Writes a job script and submits it to the scheduler."""
-        self.write_job_script(name)
-        submit_cmd = f"{self.submit_cmd} {self.batch_fname(name)}"
-        _run_submit(submit_cmd)
-
-    def __getstate__(self) -> dict:
-        return dict(
-            cores=self.cores,
-            run_script=self.run_script,
-            python_executable=self.python_executable,
-            log_folder=self.log_folder,
-            mpiexec_executable=self.mpiexec_executable,
-            executor_type=self.executor_type,
-            num_threads=self.num_threads,
-            extra_scheduler=self._extra_scheduler,
-            extra_env_vars=self._extra_env_vars,
-            extra_script=self._extra_script,
-        )
+    Parameters
+    ----------
+    learner_from : adaptive.SequenceLearner
+        Learner to take the data from.
+    learner_to : adaptive.SequenceLearner
+        Learner to tell the data to.
+    """
+    mapping = {
+        hash_anything(learner_from.sequence[i]): v for i, v in learner_from.data.items()
+    }
+    for i, key in enumerate(learner_to.sequence):
+        hsh = hash_anything(key)
+        if hsh in mapping:
+            v = mapping[hsh]
+            learner_to.tell((i, key), v)
+
+
+def _get_npoints(learner: adaptive.BaseLearner) -> int | None:
+    with suppress(AttributeError):
+        return learner.npoints
+    with suppress(AttributeError):
+        # If the Learner is a BalancingLearner
+        return sum(learner.npoints for learner in learner.learners)
+    return None
+
+
+def _progress(
+    seq: Iterable[Any],
+    with_progress_bar: bool = True,  # noqa: FBT001, FBT002
+    desc: str = "",
+) -> Iterable | tqdm:
+    if not with_progress_bar:
+        return seq
+    if in_ipynb():
+        return tqdm_notebook(list(seq), desc=desc)
+    return tqdm(list(seq), desc=desc)
+
+
+def combo_to_fname(
+    combo: dict[str, Any],
+    folder: str | Path | None = None,
+    ext: str = ".pickle",
+) -> Path:
+    """Converts a dict into a human readable filename."""
+    console.log(
+        "Use `adaptive_scheduler.utils.combo2fname` instead of `combo_to_fname`.",
+    )
+    fname = "__".join(f"{k}_{v}" for k, v in combo.items()) + ext
+    if folder is None:
+        return Path(fname)
+    return Path(folder) / fname
 
-    def __setstate__(self, state):
-        self.__init__(**state)
 
+def combo2fname(
+    combo: dict[str, Any],
+    folder: str | Path | None = None,
+    ext: str = ".pickle",
+    sig_figs: int = 8,
+) -> Path:
+    """Converts a dict into a human readable filename.
 
-class PBS(BaseScheduler):
-    def __init__(
-        self,
-        cores,
-        run_script="run_learner.py",
-        python_executable=None,
-        log_folder="",
-        mpiexec_executable=None,
-        executor_type: Literal[
-            "ipyparallel", "dask-mpi", "mpi4py", "process-pool"
-        ] = "mpi4py",
-        num_threads=1,
-        extra_scheduler=None,
-        extra_env_vars=None,
-        extra_script=None,
-        *,
-        cores_per_node=None,
-    ):
-        super().__init__(
-            cores,
-            run_script,
-            python_executable,
-            log_folder,
-            mpiexec_executable,
-            executor_type,
-            num_threads,
-            extra_scheduler,
-            extra_env_vars,
-            extra_script,
-        )
-        # Attributes that all schedulers need to have
-        self._ext = ".batch"
-        # the "-k oe" flags with "qsub" writes the log output to
-        # files directly instead of at the end of the job. The downside
-        # is that the logfiles are put in the homefolder.
-        self._submit_cmd = "qsub -k oe"
-        self._JOB_ID_VARIABLE = "${PBS_JOBID}"
-        self._options_flag = "PBS"
-        self._cancel_cmd = "qdel"
-
-        # PBS specific
-        self.cores_per_node = cores_per_node
-        self._calculate_nnodes()
-        if cores != self.cores:
-            warnings.warn(f"`self.cores` changed from {cores} to {self.cores}")
-
-    def __getstate__(self):
-        # PBS has one different argument from the BaseScheduler
-        return dict(**super().__getstate__(), cores_per_node=self.cores_per_node)
-
-    @staticmethod
-    def sanatize_job_id(job_id):
-        """Changes '91722.hpc05.hpc' into '91722'."""
-        return job_id.split(".")[0]
-
-    def _calculate_nnodes(self):
-        if self.cores_per_node is None:
-            partial_msg = "Use set `cores_per_node=...` before passing the scheduler."
-            try:
-                max_cores_per_node = self._guess_cores_per_node()
-                self.nnodes = math.ceil(self.cores / max_cores_per_node)
-                self.cores_per_node = round(self.cores / self.nnodes)
-                msg = (
-                    f"`#PBS -l nodes={self.nnodes}:ppn={self.cores_per_node}` is"
-                    f" guessed using the `qnodes` command, we set"
-                    f" `cores_per_node={self.cores_per_node}`."
-                    f" You might want to change this. {partial_msg}"
-                )
-                warnings.warn(msg)
-                self.cores = self.nnodes * self.cores_per_node
-            except Exception as e:
-                msg = (
-                    f"Got an error: {e}."
-                    " Couldn't guess `cores_per_node`, this argument is required"
-                    f" for PBS. {partial_msg}"
-                    " We set `cores_per_node=1`!"
-                )
-                warnings.warn(msg)
-                self.nnodes = self.cores
-                self.cores_per_nodes = 1
-        else:
-            self.nnodes = self.cores / self.cores_per_node
-            if not float(self.nnodes).is_integer():
-                raise ValueError("cores / cores_per_node must be an integer!")
-            else:
-                self.nnodes = int(self.nnodes)
+    Improved version of `combo_to_fname`.
+    """
+    name_parts = [f"{k}_{maybe_round(v, sig_figs)}" for k, v in sorted(combo.items())]
+    fname = Path("__".join(name_parts) + ext)
+    if folder is None:
+        return fname
+    return folder / fname
+
+
+def add_constant_to_fname(
+    combo: dict[str, Any],
+    constant: dict[str, Any],
+    *,
+    folder: str | Path | None = None,
+    ext: str = ".pickle",
+    sig_figs: int = 8,
+) -> tuple[Path, Path]:
+    """Construct old and new filename based on a combo.
 
-    def output_fnames(self, name: str) -> list[str]:
-        # The "-k oe" flags with "qsub" writes the log output to
-        # files directly instead of at the end of the job. The downside
-        # is that the logfiles are put in the homefolder.
-        home = os.path.expanduser("~/")
-        stdout, stderr = (
-            os.path.join(home, f"{name}.{x}{self._JOB_ID_VARIABLE}") for x in "oe"
-        )
-        return [stdout, stderr]
+    Assumes `combo2fname` has been used to construct the old filename.
+    Adds `constant` dict to the `combo` and returns the new filename too.
 
-    def job_script(self) -> str:
-        """Get a jobscript in string form.
+    Returns a tuple of ``old_fname`` and ``new_fname``.
+    """
+    for k in constant:
+        combo.pop(k, None)
+    old_fname = combo2fname(combo, folder, ext, sig_figs)
+    combo.update(constant)
+    new_fname = combo2fname(combo, folder, ext, sig_figs)
+    return old_fname, new_fname
+
+
+def maybe_round(x: Any, sig_figs: int) -> Any:
+    """Round to specified number of sigfigs if x is a float or complex."""
+    rnd = functools.partial(round_sigfigs, sig_figs=sig_figs)
+
+    def try_is_nan_inf(x: Any) -> bool:
+        try:
+            return np.isnan(x) or np.isinf(x)
+        except Exception:  # noqa: BLE001
+            return False
+
+    if try_is_nan_inf(x):
+        return x
+    if isinstance(x, float):
+        return rnd(x)
+    if isinstance(x, complex):
+        return complex(rnd(x.real), rnd(x.imag))
+    return x
 
-        Returns
-        -------
-        job_script : str
-            A job script that can be submitted to PBS.
-        """
 
-        job_script = textwrap.dedent(
-            f"""\
-            #!/bin/sh
-            #PBS -l nodes={self.nnodes}:ppn={self.cores_per_node}
-            #PBS -V
-            #PBS -o /tmp/placeholder
-            #PBS -e /tmp/placeholder
-            {{extra_scheduler}}
-
-            export MKL_NUM_THREADS={self.num_threads}
-            export OPENBLAS_NUM_THREADS={self.num_threads}
-            export OMP_NUM_THREADS={self.num_threads}
-            export NUMEXPR_NUM_THREADS={self.num_threads}
-            {{extra_env_vars}}
+def round_sigfigs(num: float, sig_figs: int) -> float:
+    """Round to specified number of sigfigs.
 
-            cd $PBS_O_WORKDIR
+    From
+    http://code.activestate.com/recipes/578114-round-number-to-specified-number-of-significant-di/
+    """
+    num = float(num)
+    if num != 0:
+        return round(num, -int(math.floor(math.log10(abs(num))) - (sig_figs - 1)))
+    return 0.0  # Can't take the log of 0
 
-            {{extra_script}}
 
-            {{executor_specific}}
-            """
-        )
+def _remove_or_move_files(
+    fnames: Sequence[str] | set[str] | Sequence[Path] | set[Path],
+    *,
+    with_progress_bar: bool = True,
+    move_to: str | Path | None = None,
+    desc: str | None = None,
+) -> None:
+    """Remove files by filename.
 
-        job_script = job_script.format(
-            extra_scheduler=self.extra_scheduler,
-            extra_env_vars=self.extra_env_vars,
-            extra_script=self.extra_script,
-            executor_specific=self._executor_specific("${NAME}"),
-            job_id_variable=self._JOB_ID_VARIABLE,
+    Parameters
+    ----------
+    fnames : list
+        List of filenames.
+    with_progress_bar : bool, default: True
+        Display a progress bar using `tqdm`.
+    move_to : str | Path, default None
+        Move the file to a different directory.
+        If None the file is removed.
+    desc : str, default: None
+        Description of the progressbar.
+    """
+    n_failed = 0
+    for fname in _progress(fnames, with_progress_bar, desc or "Removing files"):
+        fname = Path(fname)  # noqa: PLW2901
+        try:
+            if move_to is None:
+                fname.unlink()
+            else:
+                move_to = Path(move_to)
+                move_to.mkdir(parents=True, exist_ok=True)
+                src = fname.resolve()
+                dst = (move_to / src.name).resolve()
+                shutil.move(src, dst)  # overwrites old files
+        except Exception:  # noqa: BLE001
+            n_failed += 1
+
+    if n_failed:
+        warnings.warn(
+            f"Failed to remove (or move) {n_failed}/{len(fnames)} files.",
+            stacklevel=2,
         )
 
-        return job_script
 
-    def start_job(self, name: str) -> None:
-        """Writes a job script and submits it to the scheduler."""
-        name_prefix = name.rsplit("-", 1)[0]
-        self.write_job_script(name_prefix)
-        name_opt = f"-N {name}"
-        submit_cmd = f"{self.submit_cmd} {name_opt} {self.batch_fname(name_prefix)}"
-        _run_submit(submit_cmd, name)
-
-    @staticmethod
-    def _split_by_job(lines):
-        jobs = [[]]
-        for line in lines:
-            line = line.strip()
-            if line:
-                jobs[-1].append(line)
-            else:
-                jobs.append([])
-        return [j for j in jobs if j]
+def load_parallel(
+    learners: list[adaptive.BaseLearner],
+    fnames: list[str] | list[Path],
+    *,
+    with_progress_bar: bool = True,
+    max_workers: int | None = None,
+) -> None:
+    r"""Load a sequence of learners in parallel.
 
-    @staticmethod
-    def _fix_line_cuts(raw_info):
-        info = []
-        for line in raw_info:
-            if " = " in line:
-                info.append(line)
-            else:
-                info[-1] += line
-        return info
+    Parameters
+    ----------
+    learners : sequence of `adaptive.BaseLearner`\s
+        The learners to be loaded.
+    fnames : sequence of str
+        A list of filenames corresponding to `learners`.
+    with_progress_bar : bool, default True
+        Display a progress bar using `tqdm`.
+    max_workers : int, optional
+        The maximum number of parallel threads when loading the data.
+        If ``None``, use the maximum number of threads that is possible.
+    """
 
-    def queue(self, me_only: bool = True) -> dict[str, dict]:
-        cmd = ["qstat", "-f"]
+    def load(learner: adaptive.BaseLearner, fname: str) -> None:
+        learner.load(fname)
 
-        proc = subprocess.run(
-            cmd,
-            text=True,
-            capture_output=True,
-            env=dict(os.environ, SGE_LONG_QNAMES="1000"),
-        )
-        output = proc.stdout
+    with ThreadPoolExecutor(max_workers) as ex:
+        iterator = zip(learners, fnames)
+        pbar = _progress(iterator, with_progress_bar, "Submitting loading tasks")
+        futs = [ex.submit(load, *args) for args in pbar]
+        for fut in _progress(futs, with_progress_bar, "Finishing loading"):
+            fut.result()
+
+
+def save_parallel(
+    learners: list[adaptive.BaseLearner],
+    fnames: list[str] | list[Path],
+    *,
+    with_progress_bar: bool = True,
+) -> None:
+    r"""Save a sequence of learners in parallel.
+
+    Parameters
+    ----------
+    learners : sequence of `adaptive.BaseLearner`\s
+        The learners to be saved.
+    fnames : sequence of str
+        A list of filenames corresponding to `learners`.
+    with_progress_bar : bool, default True
+        Display a progress bar using `tqdm`.
+    """
 
-        if proc.returncode != 0:
-            raise RuntimeError("qstat is not responding.")
+    def save(learner: adaptive.BaseLearner, fname: str) -> None:
+        learner.save(fname)
 
-        jobs = self._split_by_job(output.replace("\n\t", "").split("\n"))
+    with ThreadPoolExecutor() as ex:
+        iterator = zip(learners, fnames)
+        pbar = _progress(iterator, with_progress_bar, "Submitting saving tasks")
+        futs = [ex.submit(save, *args) for args in pbar]
+        for fut in _progress(futs, with_progress_bar, "Finishing saving"):
+            fut.result()
+
+
+def _print_same_line(msg: str, *, new_line_end: bool = False) -> None:
+    msg = msg.strip()
+    global MAX_LINE_LENGTH
+    MAX_LINE_LENGTH = max(len(msg), MAX_LINE_LENGTH)
+    empty_space = max(MAX_LINE_LENGTH - len(msg), 0) * " "
+    print(msg + empty_space, end="\r" if not new_line_end else "\n")
+
+
+def _wait_for_successful_ipyparallel_client_start(
+    client: Any,
+    n: int,
+    timeout: int,
+) -> Any:
+    from ipyparallel.error import NoEnginesRegistered
+
+    n_engines_old = 0
+    for t in range(timeout):
+        n_engines = len(client)
+        with suppress(NoEnginesRegistered):
+            # This can happen, we just need to wait a little longer.
+            dview = client[:]
+        msg = f"Connected to {n_engines} out of {n} engines after {t} seconds."
+        _print_same_line(msg, new_line_end=(n_engines_old != n_engines))
+        if n_engines >= n:
+            return dview
+        n_engines_old = n_engines
+        time.sleep(1)
+    msg = f"Not all ({n_engines}/{n}) connected after {timeout} seconds."
+    raise Exception(msg)  # noqa: TRY002
+
+
+def connect_to_ipyparallel(
+    n: int,
+    profile: str,
+    timeout: int = 300,
+    folder: str | None = None,
+    client_kwargs: dict | None = None,
+) -> Any:
+    """Connect to an `ipcluster` on the cluster headnode.
 
-        running = {}
-        for header, *raw_info in jobs:
-            job_id = header.split("Job Id: ")[1]
-            info = dict([line.split(" = ") for line in self._fix_line_cuts(raw_info)])
-            if info["job_state"] in ["R", "Q"]:
-                info["job_name"] = info[
-                    "Job_Name"
-                ]  # used in `server_support.manage_jobs`
-                info["state"] = info["job_state"]  # used in `RunManager.live`
-                running[job_id] = info
-
-        if me_only:
-            # We do this because the "-u [username here]"  flag doesn't
-            # work with "-f" on some clusters.
-            username = getpass.getuser()
-            running = {
-                job_id: info
-                for job_id, info in running.items()
-                if username in info["Job_Owner"]
-            }
-
-        return running
-
-    def _qnodes(self):
-        proc = subprocess.run(["qnodes"], text=True, capture_output=True)
-        output = proc.stdout
-
-        if proc.returncode != 0:
-            raise RuntimeError("qnodes is not responding.")
-
-        jobs = self._split_by_job(output.replace("\n\t", "").split("\n"))
-
-        nodes = {
-            node: dict([line.split(" = ") for line in self._fix_line_cuts(raw_info)])
-            for node, *raw_info in jobs
-        }
-        return nodes
-
-    def _guess_cores_per_node(self):
-        nodes = self._qnodes()
-        cntr = collections.Counter([int(info["np"]) for info in nodes.values()])
-        ncores, freq = cntr.most_common(1)[0]
-        return ncores
-
-
-class SLURM(BaseScheduler):
-    """Base object for a Scheduler.
-
-    Parameters
-    ----------
-    cores : int | None
-        Number of cores per job (so per learner.)
-        Either use `cores` or `nodes` and `cores_per_node`.
-    nodes : int | None
-        Number of nodes per job (so per learner.)
-        Either `nodes` and `cores_per_node` or use `cores`.
-    cores_per_node: int | None
-        Number of cores per node.
-        Either `nodes` and `cores_per_node` or use `cores`.
-    partition: str | None
-        The SLURM partition to submit the job to.
-    exclusive : bool
-        Whether to use exclusive nodes (e.g., if SLURM it adds ``--exclusive`` as option).
-    run_script : str
-        Filename of the script that is run on the nodes. Inside this script we
-        query the database and run the learner.
-    python_executable : str, default: `sys.executable`
-        The Python executable that should run the `run_script`. By default
-        it uses the same Python as where this function is called.
-    log_folder : str, default: ""
-        The folder in which to put the log-files.
-    mpiexec_executable : str, optional
-        ``mpiexec`` executable. By default `mpiexec` will be
-        used (so probably from ``conda``).
-    executor_type : str, default: "mpi4py"
-        The executor that is used, by default `mpi4py.futures.MPIPoolExecutor` is used.
-        One can use ``"ipyparallel"``, ``"dask-mpi"``, ``"mpi4py"``, or ``"process-pool"``.
-    num_threads : int, default 1
-        ``MKL_NUM_THREADS``, ``OPENBLAS_NUM_THREADS``, ``OMP_NUM_THREADS``, and
-        ``NUMEXPR_NUM_THREADS`` will be set to this number.
-    extra_scheduler : list, optional
-        Extra ``#SLURM`` (depending on scheduler type)
-        arguments, e.g. ``["--exclusive=user", "--time=1"]``.
-    extra_env_vars : list, optional
-        Extra environment variables that are exported in the job
-        script. e.g. ``["TMPDIR='/scratch'", "PYTHONPATH='my_dir:$PYTHONPATH'"]``.
-    extra_script : str, optional
-        Extra script that will be executed after any environment variables are set,
-        but before the main scheduler is run.
+    Parameters
+    ----------
+    n : int
+        Number of engines to be started.
+    profile : str
+        Profile name of IPython profile.
+    timeout : int
+        Time for which we try to connect to get all the engines.
+    folder : str, optional
+        Folder that is added to the path of the engines, e.g. ``"~/Work/my_current_project"``.
+    client_kwargs
+        Keyword arguments passed to `ipyparallel.Client`.
+
+    Returns
+    -------
+    client : `ipyparallel.Client` object
+        An IPyparallel client.
+    """
+    from ipyparallel import Client
+
+    client = Client(profile=profile, **(client_kwargs or {}))
+    dview = _wait_for_successful_ipyparallel_client_start(client, n, timeout)
+    dview.use_dill()
+
+    if folder is not None:
+        console.print(f"Adding {folder} to path.")
+        cmd = f"import sys, os; sys.path.append(os.path.expanduser('{folder}'))"
+        dview.execute(cmd).result()
+
+    return client
+
+
+def _get_default_args(func: Callable) -> dict[str, str]:
+    signature = inspect.signature(func)
+    return {
+        k: v.default
+        for k, v in signature.parameters.items()
+        if v.default is not inspect.Parameter.empty
+    }
+
+
+def log_exception(log: Any, msg: str, exception: Exception) -> None:
+    """Log an exception with a message."""
+    try:
+        raise exception  # noqa: TRY301
+    except Exception:
+        log.exception(msg)
+
+
+def _serialize(msg: Any) -> list:
+    return [cloudpickle.dumps(msg)]
+
+
+def _deserialize(frames: list) -> Any:
+    try:
+        return cloudpickle.loads(frames[0])
+    except pickle.UnpicklingError as e:
+        if r"\x03" in str(e):
+            # Means that the frame is empty because it only contains an end of text char
+            # `\x03  ^C    (End of text)`
+            # TODO: Not sure why this happens.
+            console.log(
+                r"pickle.UnpicklingError in _deserialize: Received an empty frame (\x03).",
+            )
+            console.print_exception(show_locals=True)
+        raise
+
+
+class LRUCachedCallable:
+    """Wraps a function to become cached.
+
+    Parameters
+    ----------
+    function : Callable[..., Any]
+    max_size : int, optional
+        Cache size of the LRU cache, by default 128.
+    with_cloudpickle : bool
+        Use cloudpickle for storing the data in memory.
     """
 
     def __init__(
         self,
-        cores: int | None = None,
-        nodes: int | None = None,
-        cores_per_node: int | None = None,
-        partition: str | None = None,
-        exclusive: bool = True,
-        run_script="run_learner.py",
-        python_executable=None,
-        log_folder="",
-        mpiexec_executable=None,
-        executor_type: Literal[
-            "ipyparallel", "dask-mpi", "mpi4py", "process-pool"
-        ] = "mpi4py",
-        num_threads=1,
-        extra_scheduler=None,
-        extra_env_vars=None,
-        extra_script=None,
-    ):
-        self._cores = cores
-        self.nodes = nodes
-        self.cores_per_node = cores_per_node
-        self.partition = partition
-        self.exclusive = exclusive
-        self.__extra_scheduler = extra_scheduler
-
-        msg = "Specify either `nodes` and `cores_per_node`, or only `cores`, not both."
-        if cores is None:
-            if nodes is None or cores_per_node is None:
-                raise ValueError(msg)
+        function: Callable[..., Any],
+        *,
+        max_size: int = 128,
+        with_cloudpickle: bool = False,
+    ) -> None:
+        """Initialize the cache."""
+        self.max_size = max_size
+        self.function = function
+        self._with_cloudpickle = with_cloudpickle
+        self._signature = signature(self.function)
+        if max_size == 0:
+            return
+        manager = Manager()
+        self._cache_dict = manager.dict()
+        self._cache_queue = manager.list()
+        self._cache_lock = manager.Lock()
+
+    def _get_from_cache(self, key: str) -> tuple[bool, Any]:
+        """Get a value from the cache by key."""
+        if self.max_size == 0:
+            value = None
+        with self._cache_lock:
+            value = self._cache_dict.get(key)
+            if value is not None:  # Move key to back of queue
+                self._cache_queue.remove(key)
+                self._cache_queue.append(key)
+        if value is not None:
+            found = True
+            if value == _NONE_RETURN_STR:
+                value = None
+            elif self._with_cloudpickle:
+                value = cloudpickle.loads(value)
         else:
-            if nodes is not None or cores_per_node is not None:
-                raise ValueError(msg)
-
-        if extra_scheduler is None:
-            extra_scheduler = []
+            found = False
+        return found, value
 
-        if cores_per_node is not None:
-            extra_scheduler.append(f"--ntasks-per-node={cores_per_node}")
-            cores = nodes * cores_per_node
-
-        if partition is not None:
-            if partition not in self.partitions:
-                raise ValueError(
-                    f"Invalid partition: {partition}, only {self.partitions} are available."
-                )
-            extra_scheduler.append(f"--partition={partition}")
+    def _insert_into_cache(self, key: str, value: Any) -> ListProxy[Any]:
+        """Insert a key value pair into the cache."""
+        if value is None:
+            value = _NONE_RETURN_STR
+        elif self._with_cloudpickle:
+            value = cloudpickle.dumps(value)
+        with self._cache_lock:
+            cache_size = len(self._cache_queue)
+            self._cache_dict[key] = value
+            if cache_size < self.max_size:
+                self._cache_queue.append(key)
+            else:
+                key_to_evict = self._cache_queue.pop(0)
+                self._cache_dict.pop(key_to_evict)
+                self._cache_queue.append(key)
+            return self._cache_queue
 
-        if exclusive:
-            extra_scheduler.append("--exclusive")
+    @property
+    def cache_dict(self) -> dict:
+        """Returns a copy of the cache."""
+        return dict(self._cache_dict.items())
+
+    def __call__(self, *args: Any, **kwargs: Any) -> Any:
+        """Call the wrapped function and cache the result."""
+        bound_args = self._signature.bind(*args, **kwargs)
+        bound_args.apply_defaults()
+        if self.max_size == 0:
+            return self.function(*args, **kwargs)
+        key = str(bound_args.arguments)
+        found, value = self._get_from_cache(key)
+        if found:
+            return value
+        ret = self.function(*args, **kwargs)
+        self._insert_into_cache(key, ret)
+        return ret
+
+
+def shared_memory_cache(cache_size: int = 128) -> Callable:
+    """Create a cache similar to `functools.lru_cache`.
+
+    This will actually cache the return values of the function, whereas
+    `functools.lru_cache` will pickle the decorated function each time
+    with an empty cache.
+    """
 
-        super().__init__(
-            cores,
-            run_script,
-            python_executable,
-            log_folder,
-            mpiexec_executable,
-            executor_type,
-            num_threads,
-            extra_scheduler,
-            extra_env_vars,
-            extra_script,
-        )
-        # Attributes that all schedulers need to have
-        self._ext = ".sbatch"
-        self._submit_cmd = "sbatch"
-        self._JOB_ID_VARIABLE = "${SLURM_JOB_ID}"
-        self._options_flag = "SBATCH"
-        self._cancel_cmd = "scancel"
-
-        # SLURM specific
-        self.mpiexec_executable = mpiexec_executable or "srun --mpi=pmi2"
-
-    def __getstate__(self) -> dict:
-        state = super().__getstate__()
-        state["cores"] = self._cores
-        state["nodes"] = self.nodes
-        state["cores_per_node"] = self.cores_per_node
-        state["partition"] = self.partition
-        state["exclusive"] = self.exclusive
-        state["extra_scheduler"] = self.__extra_scheduler
-        return state
-
-    def __setstate__(self, state):
-        self.__init__(**state)
-
-    def _ipyparallel(self, name: str) -> str:
-        log_fname = self.log_fname(name)
-        job_id = self._JOB_ID_VARIABLE
-        profile = "${profile}"
-        cores = self.cores - 1
-        if self.nodes is not None and self.partition is not None and self.exclusive:
-            max_cores_per_node = self.partitions[self.partition]
-            tot_cores = self.nodes * max_cores_per_node
-            cores = min(self.cores, tot_cores - 1)
-        return textwrap.dedent(
-            f"""\
-            profile=adaptive_scheduler_{job_id}
-
-            echo "Creating profile {profile}"
-            ipython profile create {profile}
-
-            echo "Launching controller"
-            ipcontroller --ip="*" --profile={profile} --log-to-file &
-            sleep 10
-
-            echo "Launching engines"
-            srun --ntasks {cores} ipengine --profile={profile} --cluster-id='' --log-to-file &
-
-            echo "Starting the Python script"
-            srun --ntasks 1 {self.python_executable} {self.run_script} --profile {profile} --n {cores} --log-fname {log_fname} --job-id {job_id} --name {name}
-            """
+    def cache_decorator(function: Callable[..., Any]) -> Callable[..., Any]:
+        return functools.wraps(function)(
+            LRUCachedCallable(function, max_size=cache_size),
         )
 
-    def job_script(self) -> str:
-        """Get a jobscript in string form.
-
-        Returns
-        -------
-        job_script : str
-            A job script that can be submitted to SLURM.
-        """
-        job_script = textwrap.dedent(
-            f"""\
-            #!/bin/bash
-            #SBATCH --ntasks {self.cores}
-            #SBATCH --no-requeue
-            {{extra_scheduler}}
-
-            export MKL_NUM_THREADS={self.num_threads}
-            export OPENBLAS_NUM_THREADS={self.num_threads}
-            export OMP_NUM_THREADS={self.num_threads}
-            export NUMEXPR_NUM_THREADS={self.num_threads}
-            {{extra_env_vars}}
+    return cache_decorator
 
-            {{extra_script}}
 
-            {{executor_specific}}
-            """
-        )
+def _prefix(
+    fname: str | list[str] | Path | list[Path],
+) -> str:
+    if isinstance(fname, (tuple, list)):
+        return f".{len(fname):08}_learners."
+    if isinstance(fname, (str, Path)):
+        return ".learner."
+    msg = "Incorrect type for fname."
+    raise TypeError(msg)
+
+
+def fname_to_learner_fname(
+    fname: str | list[str] | Path | list[Path],
+) -> Path:
+    """Convert a learner filename (data) to a filename used to cloudpickle the learner."""
+    prefix = _prefix(fname)
+    if isinstance(fname, (tuple, list)):
+        fname = fname[0]
+    p = Path(fname)
+    new_name = f"{prefix}{p.stem}{p.suffix}"
+    return p.with_name(new_name)
+
+
+def fname_to_learner(
+    fname: str | list[str] | Path | list[Path],
+) -> adaptive.BaseLearner:
+    """Load a learner from a filename (based on cloudpickled learner)."""
+    learner_name = fname_to_learner_fname(fname)
+    with learner_name.open("rb") as f:
+        return cloudpickle.load(f)
+
+
+def _ensure_folder_exists(
+    fnames: FnamesTypes,
+) -> None:
+    if isinstance(fnames[0], (tuple, list)):
+        for _fnames in fnames:
+            assert isinstance(_fnames, (tuple, list))
+            _ensure_folder_exists(_fnames)
+    else:
+        assert isinstance(fnames[0], (str, Path))
+        folders = {Path(fname).parent for fname in fnames}  # type: ignore[arg-type]
+        for folder in folders:
+            folder.mkdir(parents=True, exist_ok=True)
+
+
+def cloudpickle_learners(
+    learners: list[adaptive.BaseLearner],
+    fnames: FnamesTypes,
+    *,
+    with_progress_bar: bool = False,
+    empty_copies: bool = True,
+) -> tuple[int, float]:
+    """Save a list of learners to disk using cloudpickle.
 
-        job_script = job_script.format(
-            extra_scheduler=self.extra_scheduler,
-            extra_env_vars=self.extra_env_vars,
-            extra_script=self.extra_script,
-            executor_specific=self._executor_specific("${NAME}"),
-        )
-        return job_script
+    Returns the total size of the saved files in bytes and the total time.
+    """
+    _ensure_folder_exists(fnames)
+    total_filesize = 0
+    t_start = time.time()
+    for learner, fname in _progress(
+        zip(learners, fnames),
+        with_progress_bar,
+        desc="Cloudpickling learners",
+    ):
+        fname_learner = fname_to_learner_fname(fname)
+        if empty_copies:
+            _at_least_adaptive_version("0.14.1", "empty_copies")
+            learner = learner.new()  # noqa: PLW2901
+        with fname_learner.open("wb") as f:
+            cloudpickle.dump(learner, f)
+        filesize = fname_learner.stat().st_size
+        total_filesize += filesize
+    total_time = time.time() - t_start
+    return total_filesize, total_time
+
+
+def fname_to_dataframe(
+    fname: str | list[str] | Path | list[Path],
+    format: str = "parquet",  # noqa: A002
+) -> Path:
+    """Convert a learner filename (data) to a filename is used to save the dataframe."""
+    if format == "excel":
+        format = "xlsx"  # noqa: A001
+    if isinstance(fname, (tuple, list)):
+        fname = fname[0]
+    p = Path(fname)
+    new_name = f"dataframe.{p.stem}.{format}"
+    return p.with_name(new_name)
+
+
+def save_dataframe(
+    fname: str | list[str],
+    *,
+    format: _DATAFRAME_FORMATS = "parquet",  # noqa: A002
+    save_kwargs: dict[str, Any] | None = None,
+    expand_dicts: bool = True,
+    **to_dataframe_kwargs: Any,
+) -> Callable[[adaptive.BaseLearner], None]:
+    """Save the learner's data to disk as pandas.DataFrame."""
+    save_kwargs = save_kwargs or {}
+
+    def save(learner: adaptive.BaseLearner) -> None:
+        df = learner.to_dataframe(**to_dataframe_kwargs)
+        if expand_dicts:
+            df = expand_dict_columns(df)
+        fname_df = fname_to_dataframe(fname, format=format)
+        if format == "parquet":
+            df.to_parquet(fname_df, **save_kwargs)
+        elif format == "csv":
+            df.to_csv(fname_df, **save_kwargs)
+        elif format == "hdf":
+            assert save_kwargs is not None  # for mypy
+            if "key" not in save_kwargs:
+                save_kwargs["key"] = "data"
+            df.to_hdf(fname_df, **save_kwargs)
+        elif format == "pickle":
+            df.to_pickle(fname_df, **save_kwargs)
+        elif format == "feather":
+            df.to_feather(fname_df, **save_kwargs)
+        elif format == "excel":
+            df.to_excel(fname_df, **save_kwargs)
+        elif format == "json":
+            df.to_json(fname_df, **save_kwargs)
+        else:
+            msg = f"Unknown format {format}."
+            raise ValueError(msg)
 
-    def start_job(self, name: str) -> None:
-        """Writes a job script and submits it to the scheduler."""
-        name_prefix = name.rsplit("-", 1)[0]
-        self.write_job_script(name_prefix)
-
-        output_fname = self.output_fnames(name)[0].replace(self._JOB_ID_VARIABLE, "%A")
-        output_opt = f"--output {output_fname}"
-        name_opt = f"--job-name {name}"
-        submit_cmd = (
-            f"{self.submit_cmd} {name_opt} {output_opt} {self.batch_fname(name_prefix)}"
-        )
-        _run_submit(submit_cmd, name)
+    return save
 
-    def queue(self, me_only: bool = True) -> dict[str, dict[str, str]]:
-        python_format = {
-            "jobid": 100,
-            "name": 100,
-            "state": 100,
-            "numnodes": 100,
-            "reasonlist": 4000,
-        }  # (key -> length) mapping
-
-        slurm_format = ",".join(f"{k}:{v}" for k, v in python_format.items())
-        cmd = [
-            "/usr/bin/squeue",
-            rf'--Format=",{slurm_format},"',
-            "--noheader",
-            "--array",
-        ]
-        if me_only:
-            username = getpass.getuser()
-            cmd.append(f"--user={username}")
-        proc = subprocess.run(cmd, text=True, capture_output=True)
-        output = proc.stdout
-
-        if (
-            "squeue: error" in output
-            or "slurm_load_jobs error" in output
-            or proc.returncode != 0
-        ):
-            raise RuntimeError("SLURM is not responding.")
-
-        def line_to_dict(line):
-            line = list(line)
-            info = {}
-            for k, v in python_format.items():
-                info[k] = "".join(line[:v]).strip()
-                line = line[v:]
-            return info
-
-        squeue = [line_to_dict(line) for line in output.split("\n")]
-        states = ("PENDING", "RUNNING", "CONFIGURING")
-        squeue = [info for info in squeue if info["state"] in states]
-        running = {info.pop("jobid"): info for info in squeue}
-        for info in running.values():
-            info["job_name"] = info.pop("name")
-        return running
-
-    @cached_property
-    def partitions(self):
-        return slurm_partitions()
 
+_DATAFRAME_FORMATS = Literal[
+    "parquet",
+    "csv",
+    "hdf",
+    "pickle",
+    "feather",
+    "excel",
+    "json",
+]
+
+
+def expand_dict_columns(df: pd.DataFrame) -> pd.DataFrame:
+    """Expand dict columns in a dataframe."""
+    if df.empty:
+        return df
+
+    for col, val in df.iloc[0].items():
+        if isinstance(val, dict):
+            prefix = f"{col}."
+            x = pd.json_normalize(df.pop(col)).add_prefix(prefix)  # type: ignore[arg-type]
+            x.index = df.index
+            for _col in x:
+                assert _col not in df, f"{_col=} already exists in df."
+            df = df.join(x)
+    return df
+
+
+def load_dataframes(  # noqa: PLR0912
+    fnames: list[str] | list[list[str]] | list[Path] | list[list[Path]],
+    *,
+    concat: bool = True,
+    read_kwargs: dict[str, Any] | None = None,
+    format: _DATAFRAME_FORMATS = "parquet",  # noqa: A002
+) -> pd.DataFrame | list[pd.DataFrame]:
+    """Load a list of dataframes from disk."""
+    read_kwargs = read_kwargs or {}
+    dfs = []
+    for fn in fnames:
+        fn_df = fname_to_dataframe(fn, format=format)
+        if not os.path.exists(fn_df):  # noqa: PTH110
+            continue
+        try:
+            if format == "parquet":
+                df = pd.read_parquet(fn_df, **read_kwargs)
+            elif format == "csv":
+                df = pd.read_csv(fn_df, **read_kwargs)
+            elif format == "hdf":
+                if "key" not in read_kwargs:
+                    read_kwargs["key"] = "data"
+                df = pd.read_hdf(fn_df, **read_kwargs)
+            elif format == "pickle":
+                df = pd.read_pickle(fn_df, **read_kwargs)  # noqa: S301
+            elif format == "feather":
+                df = pd.read_feather(fn_df, **read_kwargs)
+            elif format == "excel":
+                df = pd.read_excel(fn_df, **read_kwargs)
+            elif format == "json":
+                df = pd.read_json(fn_df, **read_kwargs)
+            else:
+                msg = f"Unknown format {format}."
+                raise ValueError(msg)  # noqa: TRY301
+        except Exception:  # noqa: BLE001
+            msg = f"`{fn}`'s DataFrame ({fn_df}) could not be read."
+            console.print(msg)
+            continue
+        df["fname"] = len(df) * [fn]
+        dfs.append(df)
+    if concat:
+        if dfs:
+            return pd.concat(dfs, axis=0)
+        return pd.DataFrame()
+    return dfs
+
+
+def _at_least_adaptive_version(
+    version: str,
+    name: str = "",
+    *,
+    raises: bool = True,
+) -> bool:
+    import pkg_resources
+
+    required = pkg_resources.parse_version(version)
+    v = adaptive.__version__
+    v_clean = ".".join(v.split(".")[:3])  # remove the dev0 or other suffix
+    current = pkg_resources.parse_version(v_clean)
+    if current < required:
+        if raises:
+            msg = (
+                f"`{name}` requires adaptive version "
+                f"of at least '{required}', currently using '{current}'.",
+            )
+            raise RuntimeError(msg)
+        return False
+    return True
+
+
+class _TimeGoal:
+    def __init__(self, dt: timedelta | datetime) -> None:
+        self.dt = dt
+        self.start_time: datetime | None = None
+
+    def __call__(self, learner: adaptive.BaseLearner) -> bool:  # noqa: ARG002
+        if isinstance(self.dt, timedelta):
+            if self.start_time is None:
+                self.start_time = datetime.now()  # noqa: DTZ005
+            return datetime.now() - self.start_time > self.dt  # noqa: DTZ005
+        if isinstance(self.dt, datetime):
+            return datetime.now() > self.dt  # noqa: DTZ005
+        msg = f"{self.dt=} is not a datetime or timedelta."
+        raise TypeError(msg)
+
+
+def smart_goal(
+    goal: GoalTypes,
+    learners: list[adaptive.BaseLearner],
+) -> Callable[[adaptive.BaseLearner], bool]:
+    """Extract a goal from the learners.
 
-class LocalMockScheduler(BaseScheduler):
-    """A scheduler that can be used for testing and runs locally.
+    Parameters
+    ----------
+    goal
+        Either a typical callable goal, or integer for number of points goal,
+        or float for loss goal, or None to automatically determine, or
+        `datetime.timedelta` for a time-based goal.
+    learners
+        List of learners.
 
-    CANCELLING DOESN'T WORK ATM, ALSO LEAVES ZOMBIE PROCESSES!
+    Returns
+    -------
+    Callable[[adaptive.BaseLearner], bool]
     """
-
-    def __init__(
-        self,
-        cores,
-        run_script="run_learner.py",
-        python_executable=None,
-        log_folder="",
-        mpiexec_executable=None,
-        executor_type="mpi4py",
-        num_threads=1,
-        extra_scheduler=None,
-        extra_env_vars=None,
-        extra_script=None,
-        *,
-        mock_scheduler_kwargs=None,
-    ):
-        warnings.warn("The LocalMockScheduler currently doesn't work!")
-        super().__init__(
-            cores,
-            run_script,
-            python_executable,
-            log_folder,
-            mpiexec_executable,
-            executor_type,
-            num_threads,
-            extra_scheduler,
-            extra_env_vars,
-            extra_script,
+    if callable(goal):
+        return goal
+    if isinstance(goal, int):
+        return lambda learner: learner.npoints >= goal
+    if isinstance(goal, float):
+        return lambda learner: learner.loss() <= goal
+    if isinstance(goal, (timedelta, datetime)):
+        return _TimeGoal(goal)
+    if goal is None:
+        learner_types = {type(learner) for learner in learners}
+        if len(learner_types) > 1:
+            msg = "Multiple learner types found."
+            raise TypeError(msg)
+        if isinstance(learners[0], adaptive.SequenceLearner):
+            return adaptive.SequenceLearner.done
+        warnings.warn(
+            "Goal is None which means the learners continue forever!",
+            stacklevel=2,
         )
-        # LocalMockScheduler specific
-        self.mock_scheduler_kwargs = mock_scheduler_kwargs or {}
-        self.mock_scheduler = adaptive_scheduler._mock_scheduler.MockScheduler(
-            **self.mock_scheduler_kwargs
-        )
-        mock_scheduler_file = adaptive_scheduler._mock_scheduler.__file__
-        self.base_cmd = f"{self.python_executable} {mock_scheduler_file}"
+        return lambda _: False
+    msg = "goal must be `callable | int | float | None`"
+    raise ValueError(msg)
 
-        # Attributes that all schedulers need to have
-        self._ext = ".batch"
-        self._submit_cmd = f"{self.base_cmd} --submit"
-        self._JOB_ID_VARIABLE = "${JOB_ID}"
-        self._cancel_cmd = f"{self.base_cmd} --cancel"
-
-    def __getstate__(self) -> dict:
-        # LocalMockScheduler has one different argument from the BaseScheduler
-        return dict(
-            **super().__getstate__(), mock_scheduler_kwargs=self.mock_scheduler_kwargs
-        )
 
-    def job_script(self) -> str:
-        """Get a jobscript in string form.
+def _serialize_to_b64(x: Any) -> str:
+    serialized_x = cloudpickle.dumps(x)
+    return base64.b64encode(serialized_x).decode("utf-8")
 
-        Returns
-        -------
-        job_script : str
-            A job script that can be submitted to PBS.
 
-        Notes
-        -----
-        Currently, there is a problem that this will not properly cleanup.
-        for example `ipengine ... &` will be detached and go on,
-        normally a scheduler will take care of this.
-        """
+def _deserialize_from_b64(x: str) -> Any:
+    bytes_ = base64.b64decode(x)
+    return cloudpickle.loads(bytes_)
 
-        job_script = textwrap.dedent(
-            f"""\
-            #!/bin/sh
-
-            export MKL_NUM_THREADS={self.num_threads}
-            export OPENBLAS_NUM_THREADS={self.num_threads}
-            export OMP_NUM_THREADS={self.num_threads}
-            export NUMEXPR_NUM_THREADS={self.num_threads}
-            {{extra_env_vars}}
 
-            {{extra_script}}
+_GLOBAL_CACHE = {}
 
-            {{executor_specific}}
-            """
-        )
 
-        job_script = job_script.format(
-            extra_env_vars=self.extra_env_vars,
-            executor_specific=self._executor_specific("${NAME}"),
-            extra_script=self.extra_script,
-            job_id_variable=self._JOB_ID_VARIABLE,
-        )
+class WrappedFunction:
+    """A wrapper to allow `cloudpickle.load`ed functions with `ProcessPoolExecutor`.
 
-        return job_script
+    A wrapper around a serialized function that handles deserialization and
+    caches the deserialized function in the worker process.
 
-    def queue(self, me_only: bool = True) -> dict[str, dict]:
-        return self.mock_scheduler.queue()
+    Parameters
+    ----------
+    function
+        The function to be serialized and wrapped.
+    mode
+        All of the options avoids sending the function to all workers.
+        If "random_id", store the serialized function only in the global cache.
+        If "file", save the serialized function to a file and store the path
+        to the file in the global cache. Only keep the path in this object.
+        If "memory", store the full serialized function in the object.
 
-    def start_job(self, name: str) -> None:
-        self.write_job_script(name)
-        submit_cmd = f"{self.submit_cmd} {name} {self.batch_fname(name)}"
-        _run_submit(submit_cmd, name)
+    Attributes
+    ----------
+    _cache_key : str
+        The key used to access the deserialized function in the global cache.
 
-    @property
-    def extra_scheduler(self):
-        raise NotImplementedError("extra_scheduler is not implemented.")
+    Examples
+    --------
+    >>> import cloudpickle
+    >>> def square(x):
+    ...     return x * x
+    >>> wrapped_function = WrappedFunction(square)
+    >>> wrapped_function(4)
+    16
+    """
 
+    def __init__(
+        self,
+        function: Callable[..., Any],
+        *,
+        mode: Literal["memory", "random_id", "file"] = "random_id",
+    ) -> None:
+        """Initialize WrappedFunction."""
+        serialized_function = cloudpickle.dumps(function)
+        self.mode = mode
+
+        if mode == "file":
+            with tempfile.NamedTemporaryFile(delete=False) as f:
+                f.write(serialized_function)
+                self._cache_key = f.name
+        elif mode == "memory":
+            self._cache_key = serialized_function
+        elif mode == "random_id":
+            assert platform.system() == "Linux"
+            name = function.__name__ if hasattr(function, "__name__") else "function"
+            self._cache_key = f"{name}_{os.urandom(16).hex()}"
+        else:
+            msg = f"mode={mode} is not valid."
+            raise ValueError(msg)
 
-def _get_default_scheduler():
-    """Determine which scheduler system is being used.
+        # This setting of the cache only works on Linux where the default start method
+        # is 'fork'. On MacOS it is 'spawn', so the cache can be populated in __call__.
+        global _GLOBAL_CACHE  # noqa: PLW0602
+        _GLOBAL_CACHE[self._cache_key] = function
 
-    It tries to determine it by running both PBS and SLURM commands.
+    def __call__(self, *args: Any, **kwargs: Any) -> Any:
+        """Call the wrapped function.
 
-    If both are available then one needs to set an environment variable
-    called 'SCHEDULER_SYSTEM' which is either 'PBS' or 'SLURM'.
+        Retrieves the deserialized function from the global cache and calls it
+        with the provided arguments and keyword arguments.
+
+        Parameters
+        ----------
+        *args : tuple
+            Positional arguments to pass to the deserialized function.
+        **kwargs : dict
+            Keyword arguments to pass to the deserialized function.
+
+        Returns
+        -------
+        Any
+            The result of calling the deserialized function with the provided
+            arguments and keyword arguments.
+        """
+        global _GLOBAL_CACHE  # noqa: PLW0602
 
-    For example add the following to your `.bashrc`
+        if self._cache_key not in _GLOBAL_CACHE:
+            if self.mode == "file":
+                with open(self._cache_key, "rb") as f:  # noqa: PTH123
+                    serialized_function = f.read()
+                deserialized_function = cloudpickle.loads(serialized_function)
+                _GLOBAL_CACHE[self._cache_key] = deserialized_function
+            elif self.mode == "memory":
+                _GLOBAL_CACHE[self._cache_key] = cloudpickle.loads(self._cache_key)
+            elif self.mode == "random_id":
+                msg = (
+                    "The function was not found in the global cache. "
+                    "This is likely because the default start method on "
+                    "your system is 'spawn' instead of 'fork'. "
+                    "Try setting `mode='file' or `mode='memory'`."
+                )
+                raise RuntimeError(msg)
 
-    ```bash
-    export SCHEDULER_SYSTEM="PBS"
-    ```
+        deserialized_function = _GLOBAL_CACHE[self._cache_key]
+        return deserialized_function(*args, **kwargs)
 
-    By default it is "SLURM".
-    """
 
-    has_pbs = bool(find_executable("qsub")) and bool(find_executable("qstat"))
-    has_slurm = bool(find_executable("sbatch")) and bool(find_executable("squeue"))
+def _now() -> str:
+    """Return the current time as a string."""
+    return datetime.now(tz=timezone.utc).isoformat()
 
-    DEFAULT = SLURM
-    default_msg = f"We set DefaultScheduler to '{DEFAULT}'."
-    scheduler_system = os.environ.get("SCHEDULER_SYSTEM", "").upper()
-    if scheduler_system:
-        if scheduler_system not in ("PBS", "SLURM"):
-            warnings.warn(
-                f"SCHEDULER_SYSTEM={scheduler_system} is not implemented."
-                f"Use SLURM or PBS. {default_msg}"
-            )
-            return DEFAULT
-        else:
-            return {"SLURM": SLURM, "PBS": PBS}[scheduler_system]
-    elif has_slurm and has_pbs:
-        msg = f"Both SLURM and PBS are detected. {default_msg}"
-        warnings.warn(msg)
-        return DEFAULT
-    elif has_pbs:
-        return PBS
-    elif has_slurm:
-        return SLURM
-    else:
-        msg = f"No scheduler system could be detected. {default_msg}"
-        warnings.warn(msg)
-        return DEFAULT
 
+def _from_datetime(dt: str) -> datetime:
+    """Return a string representation of a datetime object."""
+    return datetime.fromisoformat(dt)
 
-DefaultScheduler = _get_default_scheduler()
 
+def _time_between(start: str, end: str) -> float:
+    """Return the time between two strings representing datetimes."""
+    dt_start = _from_datetime(start)
+    dt_end = _from_datetime(end)
+    return (dt_end - dt_start).total_seconds()
 
-def _get_ncores(partition):
-    numbers = re.findall(r"\d+", partition)
-    return int(numbers[0])
 
+async def sleep_unless_task_is_done(
+    task: asyncio.Task,
+    sleep_duration: int | float,
+) -> bool:
+    """Sleep for an interval, unless the task is done before then."""
+    # Create the sleep task separately
+    sleep_task = asyncio.create_task(asyncio.sleep(sleep_duration))
 
-@lru_cache(maxsize=1)
-def slurm_partitions(
-    timeout: int = 5, with_ncores: bool = True
-) -> list[str] | dict[str, int]:
-    """Get the available slurm partitions, raises subprocess.TimeoutExpired after timeout."""
-    output = subprocess.run(
-        ["sinfo", "-ahO", "partition"], capture_output=True, timeout=timeout
+    # Await both the sleep_task and the passed task
+    done, pending = await asyncio.wait(
+        [sleep_task, task],
+        return_when=asyncio.FIRST_COMPLETED,
     )
-    lines = output.stdout.decode("utf-8").split("\n")
-    partitions = sorted(partition for line in lines if (partition := line.strip()))
-    # Sort partitions alphabetically, but put the default partition first
-    partitions = sorted(partitions, key=lambda s: ("*" not in s, s))
-    # Remove asterisk, which is used for default partition
-    partitions = [partition.replace("*", "") for partition in partitions]
-    if not with_ncores:
-        return partitions
-    else:
-        return {partition: _get_ncores(partition) for partition in partitions}
+
+    # Cancel only the sleep_task if it's pending
+    if sleep_task in pending:
+        sleep_task.cancel()
+        return True  # means that the task is done
+    return False
```


# Comparing `tmp/cubed-0.6.1.tar.gz` & `tmp/cubed-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubed-0.6.1.tar", last modified: Mon Mar 27 13:48:25 2023, max compression
+gzip compressed data, was "cubed-0.6.2.tar", last modified: Fri May 12 11:19:21 2023, max compression
```

## Comparing `cubed-0.6.1.tar` & `cubed-0.6.2.tar`

### file list

```diff
@@ -1,102 +1,103 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-27 13:48:25.348789 cubed-0.6.1/
--rw-r--r--   0 tom        (501) staff       (20)     1552 2023-03-27 13:48:25.348858 cubed-0.6.1/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      939 2023-02-21 09:42:15.000000 cubed-0.6.1/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-27 13:48:25.333749 cubed-0.6.1/cubed/
--rw-r--r--   0 tom        (501) staff       (20)      846 2023-02-17 17:56:56.000000 cubed-0.6.1/cubed/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-27 13:48:25.337870 cubed-0.6.1/cubed/array_api/
--rw-r--r--   0 tom        (501) staff       (20)     3578 2023-02-16 11:53:37.000000 cubed-0.6.1/cubed/array_api/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    12924 2023-02-16 11:53:37.000000 cubed-0.6.1/cubed/array_api/array_object.py
--rw-r--r--   0 tom        (501) staff       (20)       81 2022-10-17 16:19:52.000000 cubed-0.6.1/cubed/array_api/constants.py
--rw-r--r--   0 tom        (501) staff       (20)     8760 2023-03-21 10:44:51.000000 cubed-0.6.1/cubed/array_api/creation_functions.py
--rw-r--r--   0 tom        (501) staff       (20)      751 2022-10-17 16:19:52.000000 cubed-0.6.1/cubed/array_api/data_type_functions.py
--rw-r--r--   0 tom        (501) staff       (20)      471 2022-10-17 16:19:52.000000 cubed-0.6.1/cubed/array_api/dtypes.py
--rw-r--r--   0 tom        (501) staff       (20)    11395 2022-10-17 16:19:52.000000 cubed-0.6.1/cubed/array_api/elementwise_functions.py
--rw-r--r--   0 tom        (501) staff       (20)       83 2023-02-16 11:53:37.000000 cubed-0.6.1/cubed/array_api/indexing_functions.py
--rw-r--r--   0 tom        (501) staff       (20)     4016 2022-10-17 16:19:52.000000 cubed-0.6.1/cubed/array_api/linear_algebra_functions.py
--rw-r--r--   0 tom        (501) staff       (20)     9132 2023-03-21 10:44:51.000000 cubed-0.6.1/cubed/array_api/manipulation_functions.py
--rw-r--r--   0 tom        (501) staff       (20)     1010 2022-10-17 16:19:52.000000 cubed-0.6.1/cubed/array_api/searching_functions.py
--rw-r--r--   0 tom        (501) staff       (20)     3693 2023-03-17 17:46:35.000000 cubed-0.6.1/cubed/array_api/statistical_functions.py
--rw-r--r--   0 tom        (501) staff       (20)      479 2022-10-17 16:19:52.000000 cubed-0.6.1/cubed/array_api/utility_functions.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-27 13:48:25.339026 cubed-0.6.1/cubed/core/
--rw-r--r--   0 tom        (501) staff       (20)      431 2023-02-17 17:56:56.000000 cubed-0.6.1/cubed/core/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    11826 2023-03-21 10:44:51.000000 cubed-0.6.1/cubed/core/array.py
--rw-r--r--   0 tom        (501) staff       (20)     5531 2023-03-21 10:44:51.000000 cubed-0.6.1/cubed/core/gufunc.py
--rw-r--r--   0 tom        (501) staff       (20)    26650 2023-03-21 10:44:51.000000 cubed-0.6.1/cubed/core/ops.py
--rw-r--r--   0 tom        (501) staff       (20)    11573 2023-03-17 13:01:21.000000 cubed-0.6.1/cubed/core/plan.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-27 13:48:25.339972 cubed-0.6.1/cubed/extensions/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.1/cubed/extensions/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1164 2023-02-16 11:53:37.000000 cubed-0.6.1/cubed/extensions/history.py
--rw-r--r--   0 tom        (501) staff       (20)     2738 2022-10-17 16:19:52.000000 cubed-0.6.1/cubed/extensions/timeline.py
--rw-r--r--   0 tom        (501) staff       (20)     1439 2023-02-16 11:53:37.000000 cubed-0.6.1/cubed/extensions/tqdm.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-27 13:48:25.340699 cubed-0.6.1/cubed/primitive/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.1/cubed/primitive/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    10932 2023-03-21 10:44:51.000000 cubed-0.6.1/cubed/primitive/blockwise.py
--rw-r--r--   0 tom        (501) staff       (20)     1853 2023-03-17 13:01:21.000000 cubed-0.6.1/cubed/primitive/rechunk.py
--rw-r--r--   0 tom        (501) staff       (20)      355 2023-03-17 13:01:21.000000 cubed-0.6.1/cubed/primitive/types.py
--rw-r--r--   0 tom        (501) staff       (20)     1381 2023-03-21 10:44:51.000000 cubed-0.6.1/cubed/random.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-27 13:48:25.341676 cubed-0.6.1/cubed/runtime/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.1/cubed/runtime/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      953 2022-10-17 16:19:52.000000 cubed-0.6.1/cubed/runtime/backup.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-27 13:48:25.342817 cubed-0.6.1/cubed/runtime/executors/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.1/cubed/runtime/executors/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     8292 2023-03-17 13:01:21.000000 cubed-0.6.1/cubed/runtime/executors/beam.py
--rw-r--r--   0 tom        (501) staff       (20)     9228 2023-03-17 13:01:21.000000 cubed-0.6.1/cubed/runtime/executors/lithops.py
--rw-r--r--   0 tom        (501) staff       (20)     3460 2023-03-27 13:45:10.000000 cubed-0.6.1/cubed/runtime/executors/modal.py
--rw-r--r--   0 tom        (501) staff       (20)     6115 2023-03-27 13:45:10.000000 cubed-0.6.1/cubed/runtime/executors/modal_async.py
--rw-r--r--   0 tom        (501) staff       (20)     1279 2023-02-16 11:53:37.000000 cubed-0.6.1/cubed/runtime/executors/python.py
--rw-r--r--   0 tom        (501) staff       (20)     4187 2023-02-16 11:53:37.000000 cubed-0.6.1/cubed/runtime/executors/python_async.py
--rw-r--r--   0 tom        (501) staff       (20)     3620 2023-03-17 17:46:35.000000 cubed-0.6.1/cubed/runtime/pipeline.py
--rw-r--r--   0 tom        (501) staff       (20)      251 2023-03-17 13:01:21.000000 cubed-0.6.1/cubed/runtime/types.py
--rw-r--r--   0 tom        (501) staff       (20)      118 2022-10-17 16:19:52.000000 cubed-0.6.1/cubed/runtime/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-27 13:48:25.344687 cubed-0.6.1/cubed/tests/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.1/cubed/tests/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-27 13:48:25.345210 cubed-0.6.1/cubed/tests/primitive/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.1/cubed/tests/primitive/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     6308 2023-03-21 10:44:51.000000 cubed-0.6.1/cubed/tests/primitive/test_blockwise.py
--rw-r--r--   0 tom        (501) staff       (20)     2505 2023-03-17 13:01:21.000000 cubed-0.6.1/cubed/tests/primitive/test_rechunk.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-27 13:48:25.345972 cubed-0.6.1/cubed/tests/runtime/
--rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.1/cubed/tests/runtime/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      860 2022-10-17 16:19:52.000000 cubed-0.6.1/cubed/tests/runtime/test_backup.py
--rw-r--r--   0 tom        (501) staff       (20)     4014 2022-10-17 16:19:52.000000 cubed-0.6.1/cubed/tests/runtime/test_lithops.py
--rw-r--r--   0 tom        (501) staff       (20)     4691 2023-03-27 13:45:10.000000 cubed-0.6.1/cubed/tests/runtime/test_modal_async.py
--rw-r--r--   0 tom        (501) staff       (20)    16651 2023-02-16 11:53:37.000000 cubed-0.6.1/cubed/tests/test_array_api.py
--rw-r--r--   0 tom        (501) staff       (20)    14330 2023-02-16 11:53:37.000000 cubed-0.6.1/cubed/tests/test_core.py
--rw-r--r--   0 tom        (501) staff       (20)     3024 2023-02-21 09:41:17.000000 cubed-0.6.1/cubed/tests/test_gufunc.py
--rw-r--r--   0 tom        (501) staff       (20)     1450 2023-02-16 11:53:37.000000 cubed-0.6.1/cubed/tests/test_indexing.py
--rw-r--r--   0 tom        (501) staff       (20)     6778 2023-02-16 11:53:37.000000 cubed-0.6.1/cubed/tests/test_mem_utilization.py
--rw-r--r--   0 tom        (501) staff       (20)     2393 2023-02-16 11:53:37.000000 cubed-0.6.1/cubed/tests/test_optimization.py
--rw-r--r--   0 tom        (501) staff       (20)     1221 2022-10-17 16:19:52.000000 cubed-0.6.1/cubed/tests/test_random.py
--rw-r--r--   0 tom        (501) staff       (20)     2231 2023-02-16 11:53:37.000000 cubed-0.6.1/cubed/tests/test_utils.py
--rw-r--r--   0 tom        (501) staff       (20)     2703 2023-03-17 13:01:21.000000 cubed-0.6.1/cubed/tests/utils.py
--rw-r--r--   0 tom        (501) staff       (20)     4302 2023-03-21 10:44:51.000000 cubed-0.6.1/cubed/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-27 13:48:25.346099 cubed-0.6.1/cubed/vendor/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-17 13:01:21.000000 cubed-0.6.1/cubed/vendor/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-27 13:48:25.346843 cubed-0.6.1/cubed/vendor/dask/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-21 10:44:51.000000 cubed-0.6.1/cubed/vendor/dask/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-27 13:48:25.347701 cubed-0.6.1/cubed/vendor/dask/array/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-21 10:44:51.000000 cubed-0.6.1/cubed/vendor/dask/array/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    17366 2023-03-21 10:44:51.000000 cubed-0.6.1/cubed/vendor/dask/array/core.py
--rw-r--r--   0 tom        (501) staff       (20)     1685 2023-03-21 10:44:51.000000 cubed-0.6.1/cubed/vendor/dask/array/gufunc.py
--rw-r--r--   0 tom        (501) staff       (20)     4670 2023-03-21 10:44:51.000000 cubed-0.6.1/cubed/vendor/dask/array/reshape.py
--rw-r--r--   0 tom        (501) staff       (20)      543 2023-03-21 10:44:51.000000 cubed-0.6.1/cubed/vendor/dask/array/utils.py
--rw-r--r--   0 tom        (501) staff       (20)    14901 2023-03-21 10:44:51.000000 cubed-0.6.1/cubed/vendor/dask/blockwise.py
--rw-r--r--   0 tom        (501) staff       (20)      608 2023-03-21 10:44:51.000000 cubed-0.6.1/cubed/vendor/dask/core.py
--rw-r--r--   0 tom        (501) staff       (20)     2221 2023-03-21 10:44:51.000000 cubed-0.6.1/cubed/vendor/dask/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-27 13:48:25.348408 cubed-0.6.1/cubed/vendor/rechunker/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-17 13:01:21.000000 cubed-0.6.1/cubed/vendor/rechunker/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    13197 2023-03-17 13:01:21.000000 cubed-0.6.1/cubed/vendor/rechunker/algorithm.py
--rw-r--r--   0 tom        (501) staff       (20)    12312 2023-03-21 10:44:51.000000 cubed-0.6.1/cubed/vendor/rechunker/api.py
--rw-r--r--   0 tom        (501) staff       (20)      309 2023-03-17 13:01:21.000000 cubed-0.6.1/cubed/vendor/rechunker/compat.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-27 13:48:25.348668 cubed-0.6.1/cubed/vendor/rechunker/executors/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-17 13:01:21.000000 cubed-0.6.1/cubed/vendor/rechunker/executors/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      923 2023-03-17 13:01:21.000000 cubed-0.6.1/cubed/vendor/rechunker/executors/python.py
--rw-r--r--   0 tom        (501) staff       (20)     3421 2023-03-17 13:01:21.000000 cubed-0.6.1/cubed/vendor/rechunker/types.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-27 13:48:25.334617 cubed-0.6.1/cubed.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)     1552 2023-03-27 13:48:25.000000 cubed-0.6.1/cubed.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     2498 2023-03-27 13:48:25.000000 cubed-0.6.1/cubed.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-27 13:48:25.000000 cubed-0.6.1/cubed.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)       86 2023-03-27 13:48:25.000000 cubed-0.6.1/cubed.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)        6 2023-03-27 13:48:25.000000 cubed-0.6.1/cubed.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       81 2022-10-17 16:19:52.000000 cubed-0.6.1/pyproject.toml
--rw-r--r--   0 tom        (501) staff       (20)     1956 2023-03-27 13:48:25.349465 cubed-0.6.1/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)       91 2022-10-17 16:19:52.000000 cubed-0.6.1/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.078756 cubed-0.6.2/
+-rw-r--r--   0 tom        (501) staff       (20)    11358 2023-05-12 10:58:36.000000 cubed-0.6.2/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)     1868 2023-05-12 11:19:21.078886 cubed-0.6.2/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      939 2023-02-21 09:42:15.000000 cubed-0.6.2/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.062905 cubed-0.6.2/cubed/
+-rw-r--r--   0 tom        (501) staff       (20)      846 2023-05-05 10:22:49.000000 cubed-0.6.2/cubed/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.066460 cubed-0.6.2/cubed/array_api/
+-rw-r--r--   0 tom        (501) staff       (20)     3578 2023-02-16 11:53:37.000000 cubed-0.6.2/cubed/array_api/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    12924 2023-02-16 11:53:37.000000 cubed-0.6.2/cubed/array_api/array_object.py
+-rw-r--r--   0 tom        (501) staff       (20)       81 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/array_api/constants.py
+-rw-r--r--   0 tom        (501) staff       (20)     8760 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/array_api/creation_functions.py
+-rw-r--r--   0 tom        (501) staff       (20)      751 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/array_api/data_type_functions.py
+-rw-r--r--   0 tom        (501) staff       (20)      471 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/array_api/dtypes.py
+-rw-r--r--   0 tom        (501) staff       (20)    11395 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/array_api/elementwise_functions.py
+-rw-r--r--   0 tom        (501) staff       (20)       83 2023-02-16 11:53:37.000000 cubed-0.6.2/cubed/array_api/indexing_functions.py
+-rw-r--r--   0 tom        (501) staff       (20)     4016 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/array_api/linear_algebra_functions.py
+-rw-r--r--   0 tom        (501) staff       (20)     9132 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/array_api/manipulation_functions.py
+-rw-r--r--   0 tom        (501) staff       (20)     1010 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/array_api/searching_functions.py
+-rw-r--r--   0 tom        (501) staff       (20)     3693 2023-03-17 17:46:35.000000 cubed-0.6.2/cubed/array_api/statistical_functions.py
+-rw-r--r--   0 tom        (501) staff       (20)      479 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/array_api/utility_functions.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.067894 cubed-0.6.2/cubed/core/
+-rw-r--r--   0 tom        (501) staff       (20)      431 2023-02-17 17:56:56.000000 cubed-0.6.2/cubed/core/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    11826 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/core/array.py
+-rw-r--r--   0 tom        (501) staff       (20)     5531 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/core/gufunc.py
+-rw-r--r--   0 tom        (501) staff       (20)    26650 2023-05-11 13:34:35.000000 cubed-0.6.2/cubed/core/ops.py
+-rw-r--r--   0 tom        (501) staff       (20)    11573 2023-05-11 13:34:35.000000 cubed-0.6.2/cubed/core/plan.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.068648 cubed-0.6.2/cubed/extensions/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/extensions/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1164 2023-05-11 13:34:35.000000 cubed-0.6.2/cubed/extensions/history.py
+-rw-r--r--   0 tom        (501) staff       (20)     2738 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/extensions/timeline.py
+-rw-r--r--   0 tom        (501) staff       (20)     1439 2023-02-16 11:53:37.000000 cubed-0.6.2/cubed/extensions/tqdm.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.069469 cubed-0.6.2/cubed/primitive/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/primitive/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    10932 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/primitive/blockwise.py
+-rw-r--r--   0 tom        (501) staff       (20)     1853 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/primitive/rechunk.py
+-rw-r--r--   0 tom        (501) staff       (20)      355 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/primitive/types.py
+-rw-r--r--   0 tom        (501) staff       (20)     1381 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/random.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.070768 cubed-0.6.2/cubed/runtime/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/runtime/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      953 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/runtime/backup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.072337 cubed-0.6.2/cubed/runtime/executors/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/runtime/executors/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     8292 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/runtime/executors/beam.py
+-rw-r--r--   0 tom        (501) staff       (20)     9228 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/runtime/executors/lithops.py
+-rw-r--r--   0 tom        (501) staff       (20)     3460 2023-03-27 13:45:10.000000 cubed-0.6.2/cubed/runtime/executors/modal.py
+-rw-r--r--   0 tom        (501) staff       (20)     6115 2023-05-10 09:39:13.000000 cubed-0.6.2/cubed/runtime/executors/modal_async.py
+-rw-r--r--   0 tom        (501) staff       (20)     1279 2023-02-16 11:53:37.000000 cubed-0.6.2/cubed/runtime/executors/python.py
+-rw-r--r--   0 tom        (501) staff       (20)     4187 2023-05-10 09:39:13.000000 cubed-0.6.2/cubed/runtime/executors/python_async.py
+-rw-r--r--   0 tom        (501) staff       (20)     3620 2023-03-17 17:46:35.000000 cubed-0.6.2/cubed/runtime/pipeline.py
+-rw-r--r--   0 tom        (501) staff       (20)      251 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/runtime/types.py
+-rw-r--r--   0 tom        (501) staff       (20)      118 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/runtime/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.074620 cubed-0.6.2/cubed/tests/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/tests/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.075109 cubed-0.6.2/cubed/tests/primitive/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/tests/primitive/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     6308 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/tests/primitive/test_blockwise.py
+-rw-r--r--   0 tom        (501) staff       (20)     2505 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/tests/primitive/test_rechunk.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.075847 cubed-0.6.2/cubed/tests/runtime/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/tests/runtime/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      860 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/tests/runtime/test_backup.py
+-rw-r--r--   0 tom        (501) staff       (20)     4014 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/tests/runtime/test_lithops.py
+-rw-r--r--   0 tom        (501) staff       (20)     4691 2023-03-27 13:45:10.000000 cubed-0.6.2/cubed/tests/runtime/test_modal_async.py
+-rw-r--r--   0 tom        (501) staff       (20)    16651 2023-02-16 11:53:37.000000 cubed-0.6.2/cubed/tests/test_array_api.py
+-rw-r--r--   0 tom        (501) staff       (20)    14366 2023-05-11 10:25:04.000000 cubed-0.6.2/cubed/tests/test_core.py
+-rw-r--r--   0 tom        (501) staff       (20)     3024 2023-02-21 09:41:17.000000 cubed-0.6.2/cubed/tests/test_gufunc.py
+-rw-r--r--   0 tom        (501) staff       (20)     1450 2023-02-16 11:53:37.000000 cubed-0.6.2/cubed/tests/test_indexing.py
+-rw-r--r--   0 tom        (501) staff       (20)     6778 2023-05-11 13:34:35.000000 cubed-0.6.2/cubed/tests/test_mem_utilization.py
+-rw-r--r--   0 tom        (501) staff       (20)     2393 2023-02-16 11:53:37.000000 cubed-0.6.2/cubed/tests/test_optimization.py
+-rw-r--r--   0 tom        (501) staff       (20)     1221 2022-10-17 16:19:52.000000 cubed-0.6.2/cubed/tests/test_random.py
+-rw-r--r--   0 tom        (501) staff       (20)     2231 2023-02-16 11:53:37.000000 cubed-0.6.2/cubed/tests/test_utils.py
+-rw-r--r--   0 tom        (501) staff       (20)     2703 2023-05-11 08:51:38.000000 cubed-0.6.2/cubed/tests/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)     4302 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.076035 cubed-0.6.2/cubed/vendor/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/vendor/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.076763 cubed-0.6.2/cubed/vendor/dask/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/vendor/dask/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.077498 cubed-0.6.2/cubed/vendor/dask/array/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/vendor/dask/array/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    17366 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/vendor/dask/array/core.py
+-rw-r--r--   0 tom        (501) staff       (20)     1685 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/vendor/dask/array/gufunc.py
+-rw-r--r--   0 tom        (501) staff       (20)     4670 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/vendor/dask/array/reshape.py
+-rw-r--r--   0 tom        (501) staff       (20)      543 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/vendor/dask/array/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)    14901 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/vendor/dask/blockwise.py
+-rw-r--r--   0 tom        (501) staff       (20)      608 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/vendor/dask/core.py
+-rw-r--r--   0 tom        (501) staff       (20)     2221 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/vendor/dask/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.078336 cubed-0.6.2/cubed/vendor/rechunker/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/vendor/rechunker/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    13197 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/vendor/rechunker/algorithm.py
+-rw-r--r--   0 tom        (501) staff       (20)    12312 2023-03-21 10:44:51.000000 cubed-0.6.2/cubed/vendor/rechunker/api.py
+-rw-r--r--   0 tom        (501) staff       (20)      309 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/vendor/rechunker/compat.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.078612 cubed-0.6.2/cubed/vendor/rechunker/executors/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/vendor/rechunker/executors/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      923 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/vendor/rechunker/executors/python.py
+-rw-r--r--   0 tom        (501) staff       (20)     3421 2023-03-17 13:01:21.000000 cubed-0.6.2/cubed/vendor/rechunker/types.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-12 11:19:21.063696 cubed-0.6.2/cubed.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)     1868 2023-05-12 11:19:21.000000 cubed-0.6.2/cubed.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     2506 2023-05-12 11:19:21.000000 cubed-0.6.2/cubed.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-05-12 11:19:21.000000 cubed-0.6.2/cubed.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)      407 2023-05-12 11:19:21.000000 cubed-0.6.2/cubed.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)        6 2023-05-12 11:19:21.000000 cubed-0.6.2/cubed.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)     1652 2023-05-12 11:18:26.000000 cubed-0.6.2/pyproject.toml
+-rw-r--r--   0 tom        (501) staff       (20)     1195 2023-05-12 11:19:21.079544 cubed-0.6.2/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)      289 2023-05-12 07:47:27.000000 cubed-0.6.2/setup.py
```

### Comparing `cubed-0.6.1/PKG-INFO` & `cubed-0.6.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: cubed
-Version: 0.6.1
-Summary: Bounded-memory serverless distributed N-dimensional array processing
-Home-page: https://github.com/tomwhite/cubed
-Author: Tom White
-Author-email: tom.e.white@gmail.com
-License: Apache License 2.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # Cubed
 
 **_Note: this is a proof-of-concept, and many things are incomplete or don't work._**
 
 ## Bounded-memory serverless distributed N-dimensional array processing
 
 Cubed is a distributed N-dimensional array library implemented in Python using bounded-memory serverless processing and Zarr for storage.
```

### Comparing `cubed-0.6.1/cubed/__init__.py` & `cubed-0.6.2/cubed/__init__.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/array_api/__init__.py` & `cubed-0.6.2/cubed/array_api/__init__.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/array_api/array_object.py` & `cubed-0.6.2/cubed/array_api/array_object.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/array_api/creation_functions.py` & `cubed-0.6.2/cubed/array_api/creation_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/array_api/data_type_functions.py` & `cubed-0.6.2/cubed/array_api/data_type_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/array_api/elementwise_functions.py` & `cubed-0.6.2/cubed/array_api/elementwise_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/array_api/linear_algebra_functions.py` & `cubed-0.6.2/cubed/array_api/linear_algebra_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/array_api/manipulation_functions.py` & `cubed-0.6.2/cubed/array_api/manipulation_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/array_api/searching_functions.py` & `cubed-0.6.2/cubed/array_api/searching_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/array_api/statistical_functions.py` & `cubed-0.6.2/cubed/array_api/statistical_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/core/array.py` & `cubed-0.6.2/cubed/core/array.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/core/gufunc.py` & `cubed-0.6.2/cubed/core/gufunc.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/core/ops.py` & `cubed-0.6.2/cubed/core/ops.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/core/plan.py` & `cubed-0.6.2/cubed/core/plan.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/extensions/history.py` & `cubed-0.6.2/cubed/extensions/history.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/extensions/timeline.py` & `cubed-0.6.2/cubed/extensions/timeline.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/extensions/tqdm.py` & `cubed-0.6.2/cubed/extensions/tqdm.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/primitive/blockwise.py` & `cubed-0.6.2/cubed/primitive/blockwise.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/primitive/rechunk.py` & `cubed-0.6.2/cubed/primitive/rechunk.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/random.py` & `cubed-0.6.2/cubed/random.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/runtime/backup.py` & `cubed-0.6.2/cubed/runtime/backup.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/runtime/executors/beam.py` & `cubed-0.6.2/cubed/runtime/executors/beam.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/runtime/executors/lithops.py` & `cubed-0.6.2/cubed/runtime/executors/lithops.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/runtime/executors/modal.py` & `cubed-0.6.2/cubed/runtime/executors/modal.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/runtime/executors/modal_async.py` & `cubed-0.6.2/cubed/runtime/executors/modal_async.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/runtime/executors/python.py` & `cubed-0.6.2/cubed/runtime/executors/python.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/runtime/executors/python_async.py` & `cubed-0.6.2/cubed/runtime/executors/python_async.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/runtime/pipeline.py` & `cubed-0.6.2/cubed/runtime/pipeline.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/tests/primitive/test_blockwise.py` & `cubed-0.6.2/cubed/tests/primitive/test_blockwise.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/tests/primitive/test_rechunk.py` & `cubed-0.6.2/cubed/tests/primitive/test_rechunk.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/tests/runtime/test_backup.py` & `cubed-0.6.2/cubed/tests/runtime/test_backup.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/tests/runtime/test_lithops.py` & `cubed-0.6.2/cubed/tests/runtime/test_lithops.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/tests/runtime/test_modal_async.py` & `cubed-0.6.2/cubed/tests/runtime/test_modal_async.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/tests/test_array_api.py` & `cubed-0.6.2/cubed/tests/test_array_api.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/tests/test_core.py` & `cubed-0.6.2/cubed/tests/test_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -437,14 +437,16 @@
     # since c has already been computed, when computing d only 4 tasks are run, instead of 8
     task_counter = TaskCounter()
     d.compute(callbacks=[task_counter], optimize_graph=False)
     assert task_counter.value == 4
 
 
 def test_measure_reserved_memory(executor):
+    pytest.importorskip("lithops")
+
     from cubed.runtime.executors.lithops import LithopsDagExecutor
 
     if not isinstance(executor, LithopsDagExecutor):
         pytest.skip(f"{type(executor)} does not support measure_reserved_memory")
 
     reserved_memory = cubed.measure_reserved_memory(executor=executor)
     assert reserved_memory > 1_000_000  # over 1MB
```

### Comparing `cubed-0.6.1/cubed/tests/test_gufunc.py` & `cubed-0.6.2/cubed/tests/test_gufunc.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/tests/test_indexing.py` & `cubed-0.6.2/cubed/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/tests/test_mem_utilization.py` & `cubed-0.6.2/cubed/tests/test_mem_utilization.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/tests/test_optimization.py` & `cubed-0.6.2/cubed/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/tests/test_random.py` & `cubed-0.6.2/cubed/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/tests/test_utils.py` & `cubed-0.6.2/cubed/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/tests/utils.py` & `cubed-0.6.2/cubed/tests/utils.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/utils.py` & `cubed-0.6.2/cubed/utils.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/vendor/dask/array/core.py` & `cubed-0.6.2/cubed/vendor/dask/array/core.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/vendor/dask/array/gufunc.py` & `cubed-0.6.2/cubed/vendor/dask/array/gufunc.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/vendor/dask/array/reshape.py` & `cubed-0.6.2/cubed/vendor/dask/array/reshape.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/vendor/dask/array/utils.py` & `cubed-0.6.2/cubed/vendor/dask/array/utils.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/vendor/dask/blockwise.py` & `cubed-0.6.2/cubed/vendor/dask/blockwise.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/vendor/dask/core.py` & `cubed-0.6.2/cubed/vendor/dask/core.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/vendor/dask/utils.py` & `cubed-0.6.2/cubed/vendor/dask/utils.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/vendor/rechunker/algorithm.py` & `cubed-0.6.2/cubed/vendor/rechunker/algorithm.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/vendor/rechunker/api.py` & `cubed-0.6.2/cubed/vendor/rechunker/api.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/vendor/rechunker/executors/python.py` & `cubed-0.6.2/cubed/vendor/rechunker/executors/python.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed/vendor/rechunker/types.py` & `cubed-0.6.2/cubed/vendor/rechunker/types.py`

 * *Files identical despite different names*

### Comparing `cubed-0.6.1/cubed.egg-info/SOURCES.txt` & `cubed-0.6.2/cubed.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 cubed/__init__.py
 cubed/random.py
 cubed/utils.py
```


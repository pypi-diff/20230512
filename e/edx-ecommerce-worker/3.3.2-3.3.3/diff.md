# Comparing `tmp/edx-ecommerce-worker-3.3.2.tar.gz` & `tmp/edx-ecommerce-worker-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-ecommerce-worker-3.3.2.tar", last modified: Wed Jul  6 19:52:02 2022, max compression
+gzip compressed data, was "edx-ecommerce-worker-3.3.3.tar", last modified: Fri May 12 06:13:42 2023, max compression
```

## Comparing `edx-ecommerce-worker-3.3.2.tar` & `edx-ecommerce-worker-3.3.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 19:52:02.555090 edx-ecommerce-worker-3.3.2/
--rw-r--r--   0 runner    (1001) docker     (121)    35116 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5740 2022-07-06 19:52:02.555090 edx-ecommerce-worker-3.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4440 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 19:52:02.551090 edx-ecommerce-worker-3.3.2/ecommerce_worker/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1706 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/celery_app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 19:52:02.551090 edx-ecommerce-worker-3.3.2/ecommerce_worker/configuration/
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4154 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/configuration/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      932 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/configuration/devstack.py
--rw-r--r--   0 runner    (1001) docker     (121)      744 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/configuration/local.py
--rw-r--r--   0 runner    (1001) docker     (121)     3195 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/configuration/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/configuration/production.py
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/configuration/test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 19:52:02.551090 edx-ecommerce-worker-3.3.2/ecommerce_worker/email/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/email/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 19:52:02.555090 edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 19:52:02.555090 edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/braze/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/braze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20998 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/braze/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/braze/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    11061 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/braze/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 19:52:02.555090 edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/braze/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/braze/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17952 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/braze/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    16988 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/braze/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     6718 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 19:52:02.555090 edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     4305 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2406 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 19:52:02.555090 edx-ecommerce-worker-3.3.2/ecommerce_worker/fulfillment/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/fulfillment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 19:52:02.555090 edx-ecommerce-worker-3.3.2/ecommerce_worker/fulfillment/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/fulfillment/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2669 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/fulfillment/v1/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 19:52:02.555090 edx-ecommerce-worker-3.3.2/ecommerce_worker/fulfillment/v1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/fulfillment/v1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5752 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/fulfillment/v1/tests/test_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 19:52:02.555090 edx-ecommerce-worker-3.3.2/ecommerce_worker/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     2764 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2928 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/ecommerce_worker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 19:52:02.555090 edx-ecommerce-worker-3.3.2/edx_ecommerce_worker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5740 2022-07-06 19:52:02.000000 edx-ecommerce-worker-3.3.2/edx_ecommerce_worker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1892 2022-07-06 19:52:02.000000 edx-ecommerce-worker-3.3.2/edx_ecommerce_worker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-06 19:52:02.000000 edx-ecommerce-worker-3.3.2/edx_ecommerce_worker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-07-06 19:52:02.000000 edx-ecommerce-worker-3.3.2/edx_ecommerce_worker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-07-06 19:52:02.000000 edx-ecommerce-worker-3.3.2/edx_ecommerce_worker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 19:52:02.555090 edx-ecommerce-worker-3.3.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)     1382 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/requirements/common_constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/requirements/optional.txt
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/requirements/pip.txt
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/requirements/pip_tools.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2311 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/requirements/production.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4312 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (121)      640 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/requirements/tox.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-06 19:52:02.555090 edx-ecommerce-worker-3.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1733 2022-07-06 19:51:57.000000 edx-ecommerce-worker-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.619126 edx-ecommerce-worker-3.3.3/
+-rw-r--r--   0 runner    (1001) docker     (122)    35116 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      197 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5629 2023-05-12 06:13:42.619126 edx-ecommerce-worker-3.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4325 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.607126 edx-ecommerce-worker-3.3.3/ecommerce_worker/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1706 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/celery_app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.607126 edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/
+-rw-r--r--   0 runner    (1001) docker     (122)      512 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4154 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      932 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/devstack.py
+-rw-r--r--   0 runner    (1001) docker     (122)      744 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3195 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/production.py
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.611126 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.611126 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.611126 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20998 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11061 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.611126 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17952 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16988 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6718 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.615126 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      689 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4305 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2430 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.615126 edx-ecommerce-worker-3.3.3/ecommerce_worker/fulfillment/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/fulfillment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.615126 edx-ecommerce-worker-3.3.3/ecommerce_worker/fulfillment/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/fulfillment/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2693 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/fulfillment/v1/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.615126 edx-ecommerce-worker-3.3.3/ecommerce_worker/fulfillment/v1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/fulfillment/v1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5752 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/fulfillment/v1/tests/test_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.615126 edx-ecommerce-worker-3.3.3/ecommerce_worker/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2928 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/ecommerce_worker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.615126 edx-ecommerce-worker-3.3.3/edx_ecommerce_worker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5629 2023-05-12 06:13:42.000000 edx-ecommerce-worker-3.3.3/edx_ecommerce_worker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1892 2023-05-12 06:13:42.000000 edx-ecommerce-worker-3.3.3/edx_ecommerce_worker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-12 06:13:42.000000 edx-ecommerce-worker-3.3.3/edx_ecommerce_worker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       54 2023-05-12 06:13:42.000000 edx-ecommerce-worker-3.3.3/edx_ecommerce_worker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-12 06:13:42.000000 edx-ecommerce-worker-3.3.3/edx_ecommerce_worker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 06:13:42.619126 edx-ecommerce-worker-3.3.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1633 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1573 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/requirements/common_constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      817 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      166 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/requirements/optional.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      334 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/requirements/pip.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/requirements/pip_tools.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/requirements/production.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4691 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      589 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/requirements/tox.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-12 06:13:42.619126 edx-ecommerce-worker-3.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-05-12 06:13:36.000000 edx-ecommerce-worker-3.3.3/setup.py
```

### Comparing `edx-ecommerce-worker-3.3.2/LICENSE.txt` & `edx-ecommerce-worker-3.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.2/PKG-INFO` & `edx-ecommerce-worker-3.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 1.1
 Name: edx-ecommerce-worker
-Version: 3.3.2
+Version: 3.3.3
 Summary: Celery tasks supporting the operations of edX's ecommerce service
-Home-page: https://github.com/edx/ecommerce-worker
+Home-page: https://github.com/openedx/ecommerce-worker
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL
-Description: DEPRECATION WARNING 
+Description: DEPRECATION WARNING
         ====================
         This repository is deprecated and in maintainence-only operation while we work on a replacement, please see `this announcement <https://discuss.openedx.org/t/deprecation-removal-ecommerce-service-depr-22/6839>`__ for more information.
         -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
         
         Although we have stopped integrating new contributions, we always appreciate security disclosures and patches sent to `security@edx.org <mailto:security@edx.org>`__
         
         edX Ecommerce Worker  |Build|_ |Codecov|_
         =========================================
-        .. |Build| image:: https://github.com/edx/ecommerce-worker/workflows/Python%20CI/badge.svg?branch=master
-        .. _Build: https://github.com/edx/ecommerce-worker/actions?query=workflow%3A%22Python+CI%22
+        .. |Build| image:: https://github.com/openedx/ecommerce-worker/workflows/Python%20CI/badge.svg?branch=master
+        .. _Build: https://github.com/openedx/ecommerce-worker/actions?query=workflow%3A%22Python+CI%22
         
         .. |Codecov| image:: http://codecov.io/github/edx/ecommerce-worker/coverage.svg?branch=master
         .. _Codecov: http://codecov.io/github/edx/ecommerce-worker?branch=master
         
         The Celery tasks contained herein are used to implement asynchronous order fulfillment and other features requiring the asynchronous execution of many small, common operations.
         
         Prerequisites
@@ -28,15 +28,15 @@
         * Python 3.x
         * Celery 4.x
         * RabbitMQ 3.5.x
         
         Getting Started
         ---------------
         
-        Most commands necessary to develop and run this app can be found in the included Makefile. These instructions assume a working integration between the `edX ecommerce service <https://github.com/edx/ecommerce>`_ and the LMS, with asynchronous fulfillment configured on the ecommerce service.
+        Most commands necessary to develop and run this app can be found in the included Makefile. These instructions assume a working integration between the `edX ecommerce service <https://github.com/openedx/ecommerce>`_ and the LMS, with asynchronous fulfillment configured on the ecommerce service.
         
         To get started, create a new virtual environment and install the included requirements.
         
             $ make requirements
         
         This project uses `Celery <http://celery.readthedocs.org/en/latest/>`_ to asynchronously execute tasks, such as those required during order fulfillment. Celery requires a solution to send and receive messages which typically comes in the form of a separate service called a message broker. This project uses `RabbitMQ <http://www.rabbitmq.com/>`_ as a message broker. On OS X, use Homebrew to install it.
         
@@ -74,15 +74,15 @@
         The code in this repository is licensed under the AGPL unless otherwise noted. Please see ``LICENSE.txt`` for details.
         
         How To Contribute
         -----------------
         
         Anyone merging to this repository is expected to `release and monitor their changes <https://openedx.atlassian.net/wiki/spaces/RS/pages/1835106870/How+to+contribute+to+our+repositories>`__; if you are not able to do this DO NOT MERGE, please coordinate with someone who can to ensure that the changes are released.
         
-        Please also read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`__. Even though it was written with ``edx-platform`` in mind, these guidelines should be followed for Open edX code in general.
+        Please also read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`__.
         
         Reporting Security Issues
         -------------------------
         
         Please do not report security issues in public. Please email security@edx.org.
         
         Mailing List and IRC Channel
```

### Comparing `edx-ecommerce-worker-3.3.2/README.rst` & `edx-ecommerce-worker-3.3.3/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-DEPRECATION WARNING 
+DEPRECATION WARNING
 ====================
 This repository is deprecated and in maintainence-only operation while we work on a replacement, please see `this announcement <https://discuss.openedx.org/t/deprecation-removal-ecommerce-service-depr-22/6839>`__ for more information.
 -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 Although we have stopped integrating new contributions, we always appreciate security disclosures and patches sent to `security@edx.org <mailto:security@edx.org>`__
 
 edX Ecommerce Worker  |Build|_ |Codecov|_
 =========================================
-.. |Build| image:: https://github.com/edx/ecommerce-worker/workflows/Python%20CI/badge.svg?branch=master
-.. _Build: https://github.com/edx/ecommerce-worker/actions?query=workflow%3A%22Python+CI%22
+.. |Build| image:: https://github.com/openedx/ecommerce-worker/workflows/Python%20CI/badge.svg?branch=master
+.. _Build: https://github.com/openedx/ecommerce-worker/actions?query=workflow%3A%22Python+CI%22
 
 .. |Codecov| image:: http://codecov.io/github/edx/ecommerce-worker/coverage.svg?branch=master
 .. _Codecov: http://codecov.io/github/edx/ecommerce-worker?branch=master
 
 The Celery tasks contained herein are used to implement asynchronous order fulfillment and other features requiring the asynchronous execution of many small, common operations.
 
 Prerequisites
@@ -20,15 +20,15 @@
 * Python 3.x
 * Celery 4.x
 * RabbitMQ 3.5.x
 
 Getting Started
 ---------------
 
-Most commands necessary to develop and run this app can be found in the included Makefile. These instructions assume a working integration between the `edX ecommerce service <https://github.com/edx/ecommerce>`_ and the LMS, with asynchronous fulfillment configured on the ecommerce service.
+Most commands necessary to develop and run this app can be found in the included Makefile. These instructions assume a working integration between the `edX ecommerce service <https://github.com/openedx/ecommerce>`_ and the LMS, with asynchronous fulfillment configured on the ecommerce service.
 
 To get started, create a new virtual environment and install the included requirements.
 
     $ make requirements
 
 This project uses `Celery <http://celery.readthedocs.org/en/latest/>`_ to asynchronously execute tasks, such as those required during order fulfillment. Celery requires a solution to send and receive messages which typically comes in the form of a separate service called a message broker. This project uses `RabbitMQ <http://www.rabbitmq.com/>`_ as a message broker. On OS X, use Homebrew to install it.
 
@@ -66,15 +66,15 @@
 The code in this repository is licensed under the AGPL unless otherwise noted. Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Anyone merging to this repository is expected to `release and monitor their changes <https://openedx.atlassian.net/wiki/spaces/RS/pages/1835106870/How+to+contribute+to+our+repositories>`__; if you are not able to do this DO NOT MERGE, please coordinate with someone who can to ensure that the changes are released.
 
-Please also read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`__. Even though it was written with ``edx-platform`` in mind, these guidelines should be followed for Open edX code in general.
+Please also read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`__.
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Mailing List and IRC Channel
```

### Comparing `edx-ecommerce-worker-3.3.2/ecommerce_worker/cache.py` & `edx-ecommerce-worker-3.3.3/ecommerce_worker/cache.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.2/ecommerce_worker/configuration/__init__.py` & `edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.2/ecommerce_worker/configuration/base.py` & `edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/base.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.2/ecommerce_worker/configuration/devstack.py` & `edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/devstack.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.2/ecommerce_worker/configuration/local.py` & `edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/local.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.2/ecommerce_worker/configuration/logger.py` & `edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/logger.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.2/ecommerce_worker/configuration/production.py` & `edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/production.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.2/ecommerce_worker/configuration/test.py` & `edx-ecommerce-worker-3.3.3/ecommerce_worker/configuration/test.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/braze/client.py` & `edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/client.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/braze/exceptions.py` & `edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/exceptions.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/braze/tasks.py` & `edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/tasks.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/braze/tests/test_client.py` & `edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/braze/tests/test_tasks.py` & `edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/braze/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/tasks.py` & `edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/tasks.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/tests/test_api.py` & `edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/tests/test_utils.py` & `edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.2/ecommerce_worker/email/v1/utils.py` & `edx-ecommerce-worker-3.3.3/ecommerce_worker/email/v1/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,16 @@
             'offer_assignment_id': offer_assignment_id,
             'send_id': send_id,
             'status': status,
         }
         response = requests.post(
             api_url,
             data=post_data,
-            headers=headers
+            headers=headers,
+            timeout=10
         )
         response.raise_for_status()
         data = response.json()
     except (HTTPError, JSONDecodeError):
         return False
 
     return bool(data.get('status') == 'updated')
```

### Comparing `edx-ecommerce-worker-3.3.2/ecommerce_worker/fulfillment/v1/tasks.py` & `edx-ecommerce-worker-3.3.3/ecommerce_worker/fulfillment/v1/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,16 @@
     try:
         logger.info('Requesting fulfillment of order [%s].', order_number)
         headers = {'Authorization': f'JWT {get_access_token()}'}
         params = {'email_opt_in': email_opt_in}
         response = requests.put(
             api_url,
             params=params,
-            headers=headers
+            headers=headers,
+            timeout=10
         )
         response.raise_for_status()
 
     except HTTPError as exc:
         status_code = exc.response.status_code
         if status_code == 406:
             # The order is not fulfillable. Therefore, it must be complete.
```

### Comparing `edx-ecommerce-worker-3.3.2/ecommerce_worker/fulfillment/v1/tests/test_tasks.py` & `edx-ecommerce-worker-3.3.3/ecommerce_worker/fulfillment/v1/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.2/ecommerce_worker/tests/test_cache.py` & `edx-ecommerce-worker-3.3.3/ecommerce_worker/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.2/ecommerce_worker/tests/test_utils.py` & `edx-ecommerce-worker-3.3.3/ecommerce_worker/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.2/ecommerce_worker/utils.py` & `edx-ecommerce-worker-3.3.3/ecommerce_worker/utils.py`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.2/edx_ecommerce_worker.egg-info/PKG-INFO` & `edx-ecommerce-worker-3.3.3/edx_ecommerce_worker.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 1.1
 Name: edx-ecommerce-worker
-Version: 3.3.2
+Version: 3.3.3
 Summary: Celery tasks supporting the operations of edX's ecommerce service
-Home-page: https://github.com/edx/ecommerce-worker
+Home-page: https://github.com/openedx/ecommerce-worker
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL
-Description: DEPRECATION WARNING 
+Description: DEPRECATION WARNING
         ====================
         This repository is deprecated and in maintainence-only operation while we work on a replacement, please see `this announcement <https://discuss.openedx.org/t/deprecation-removal-ecommerce-service-depr-22/6839>`__ for more information.
         -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
         
         Although we have stopped integrating new contributions, we always appreciate security disclosures and patches sent to `security@edx.org <mailto:security@edx.org>`__
         
         edX Ecommerce Worker  |Build|_ |Codecov|_
         =========================================
-        .. |Build| image:: https://github.com/edx/ecommerce-worker/workflows/Python%20CI/badge.svg?branch=master
-        .. _Build: https://github.com/edx/ecommerce-worker/actions?query=workflow%3A%22Python+CI%22
+        .. |Build| image:: https://github.com/openedx/ecommerce-worker/workflows/Python%20CI/badge.svg?branch=master
+        .. _Build: https://github.com/openedx/ecommerce-worker/actions?query=workflow%3A%22Python+CI%22
         
         .. |Codecov| image:: http://codecov.io/github/edx/ecommerce-worker/coverage.svg?branch=master
         .. _Codecov: http://codecov.io/github/edx/ecommerce-worker?branch=master
         
         The Celery tasks contained herein are used to implement asynchronous order fulfillment and other features requiring the asynchronous execution of many small, common operations.
         
         Prerequisites
@@ -28,15 +28,15 @@
         * Python 3.x
         * Celery 4.x
         * RabbitMQ 3.5.x
         
         Getting Started
         ---------------
         
-        Most commands necessary to develop and run this app can be found in the included Makefile. These instructions assume a working integration between the `edX ecommerce service <https://github.com/edx/ecommerce>`_ and the LMS, with asynchronous fulfillment configured on the ecommerce service.
+        Most commands necessary to develop and run this app can be found in the included Makefile. These instructions assume a working integration between the `edX ecommerce service <https://github.com/openedx/ecommerce>`_ and the LMS, with asynchronous fulfillment configured on the ecommerce service.
         
         To get started, create a new virtual environment and install the included requirements.
         
             $ make requirements
         
         This project uses `Celery <http://celery.readthedocs.org/en/latest/>`_ to asynchronously execute tasks, such as those required during order fulfillment. Celery requires a solution to send and receive messages which typically comes in the form of a separate service called a message broker. This project uses `RabbitMQ <http://www.rabbitmq.com/>`_ as a message broker. On OS X, use Homebrew to install it.
         
@@ -74,15 +74,15 @@
         The code in this repository is licensed under the AGPL unless otherwise noted. Please see ``LICENSE.txt`` for details.
         
         How To Contribute
         -----------------
         
         Anyone merging to this repository is expected to `release and monitor their changes <https://openedx.atlassian.net/wiki/spaces/RS/pages/1835106870/How+to+contribute+to+our+repositories>`__; if you are not able to do this DO NOT MERGE, please coordinate with someone who can to ensure that the changes are released.
         
-        Please also read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`__. Even though it was written with ``edx-platform`` in mind, these guidelines should be followed for Open edX code in general.
+        Please also read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`__.
         
         Reporting Security Issues
         -------------------------
         
         Please do not report security issues in public. Please email security@edx.org.
         
         Mailing List and IRC Channel
```

### Comparing `edx-ecommerce-worker-3.3.2/edx_ecommerce_worker.egg-info/SOURCES.txt` & `edx-ecommerce-worker-3.3.3/edx_ecommerce_worker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-ecommerce-worker-3.3.2/requirements/base.txt` & `edx-ecommerce-worker-3.3.3/requirements/base.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,71 +1,82 @@
 #
-# This file is autogenerated by pip-compile
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    make upgrade
 #
 amqp==2.6.1
     # via kombu
-asgiref==3.4.1
+asgiref==3.6.0
     # via django
+async-timeout==4.0.2
+    # via redis
 billiard==3.6.4.0
     # via celery
 celery==4.4.7
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/base.in
-certifi==2021.5.30
+certifi==2022.12.7
     # via requests
-charset-normalizer==2.0.6
+cffi==1.15.1
+    # via pynacl
+charset-normalizer==3.1.0
     # via requests
-django-crum==0.7.9
-    # via edx-django-utils
-django-waffle==2.2.1
+click==8.1.3
     # via edx-django-utils
-django==3.2.8
+django==3.2.18
     # via
+    #   -c requirements/common_constraints.txt
     #   -c requirements/constraints.txt
     #   django-crum
     #   edx-django-utils
-edx-braze-client==0.1.4
+django-crum==0.7.9
+    # via edx-django-utils
+django-waffle==3.0.0
+    # via edx-django-utils
+edx-braze-client==0.1.6
     # via -r requirements/base.in
-edx-django-utils==4.4.0
+edx-django-utils==5.4.0
     # via edx-rest-api-client
-edx-rest-api-client==5.4.0
+edx-rest-api-client==5.5.0
     # via -r requirements/base.in
-idna==3.2
+idna==3.4
     # via requests
 kombu==4.6.11
     # via celery
-newrelic==7.0.0.166
+newrelic==8.8.0
     # via edx-django-utils
-pbr==5.6.0
+pbr==5.11.1
     # via stevedore
-psutil==5.8.0
+psutil==5.9.5
     # via edx-django-utils
-pyjwt==2.2.0
+pycparser==2.21
+    # via cffi
+pyjwt==2.6.0
     # via edx-rest-api-client
-pytz==2021.3
+pynacl==1.5.0
+    # via edx-django-utils
+pytz==2023.3
     # via
     #   celery
     #   django
-redis==3.5.3
+redis==4.5.4
     # via -r requirements/base.in
-requests==2.26.0
+requests==2.28.2
     # via
     #   edx-rest-api-client
     #   slumber
 six==1.16.0
     # via -r requirements/base.in
 slumber==0.7.1
     # via edx-rest-api-client
-sqlparse==0.4.2
+sqlparse==0.4.4
     # via django
-stevedore==3.4.0
+stevedore==5.0.0
     # via edx-django-utils
-urllib3==1.26.7
+urllib3==1.26.15
     # via requests
 vine==1.3.0
     # via
     #   amqp
     #   celery
```

### Comparing `edx-ecommerce-worker-3.3.2/requirements/common_constraints.txt` & `edx-ecommerce-worker-3.3.3/requirements/common_constraints.txt`

 * *Files 17% similar despite different names*

```diff
@@ -15,11 +15,18 @@
 # using LTS django version
 Django<4.0
 
 # elasticsearch>=7.14.0 includes breaking changes in it which caused issues in discovery upgrade process.
 # elastic search changelog: https://www.elastic.co/guide/en/enterprise-search/master/release-notes-7.14.0.html
 elasticsearch<7.14.0
 
-setuptools<60
-
 # django-simple-history>3.0.0 adds indexing and causes a lot of migrations to be affected
 django-simple-history==3.0.0
+
+# tox>4.0.0 isn't yet compatible with many tox plugins, causing CI failures in almost all repos.
+# Details can be found in this discussion: https://github.com/tox-dev/tox/discussions/1810
+tox<4.0.0
+
+# edx-sphinx-theme is not compatible with latest Sphinx==6.0.0 version 
+# Pinning Sphinx version unless the compatibility issue gets resolved
+# For details, see issue https://github.com/openedx/edx-sphinx-theme/issues/197
+sphinx<6.0.0
```

### Comparing `edx-ecommerce-worker-3.3.2/requirements/production.txt` & `edx-ecommerce-worker-3.3.3/requirements/production.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,112 +1,133 @@
 #
-# This file is autogenerated by pip-compile
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    make upgrade
 #
 amqp==2.6.1
     # via
     #   -r requirements/base.txt
     #   kombu
-asgiref==3.4.1
+asgiref==3.6.0
     # via
     #   -r requirements/base.txt
     #   django
+async-timeout==4.0.2
+    # via
+    #   -r requirements/base.txt
+    #   redis
 billiard==3.6.4.0
     # via
     #   -r requirements/base.txt
     #   celery
 celery==4.4.7
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/base.txt
-certifi==2021.5.30
+certifi==2022.12.7
     # via
     #   -r requirements/base.txt
     #   requests
-charset-normalizer==2.0.6
+cffi==1.15.1
     # via
     #   -r requirements/base.txt
-    #   requests
-django-crum==0.7.9
+    #   pynacl
+charset-normalizer==3.1.0
     # via
     #   -r requirements/base.txt
-    #   edx-django-utils
-django-waffle==2.2.1
+    #   requests
+click==8.1.3
     # via
     #   -r requirements/base.txt
     #   edx-django-utils
-django==3.2.8
+django==3.2.18
     # via
+    #   -c requirements/common_constraints.txt
     #   -c requirements/constraints.txt
     #   -r requirements/base.txt
     #   django-crum
     #   edx-django-utils
-edx-braze-client==0.1.4
+django-crum==0.7.9
+    # via
+    #   -r requirements/base.txt
+    #   edx-django-utils
+django-waffle==3.0.0
+    # via
+    #   -r requirements/base.txt
+    #   edx-django-utils
+edx-braze-client==0.1.6
     # via -r requirements/base.txt
-edx-django-utils==4.4.0
+edx-django-utils==5.4.0
     # via
     #   -r requirements/base.txt
     #   edx-rest-api-client
-edx-rest-api-client==5.4.0
+edx-rest-api-client==5.5.0
     # via -r requirements/base.txt
-idna==3.2
+idna==3.4
     # via
     #   -r requirements/base.txt
     #   requests
 kombu==4.6.11
     # via
     #   -r requirements/base.txt
     #   celery
-newrelic==7.0.0.166
+newrelic==8.8.0
     # via
     #   -r requirements/base.txt
     #   edx-django-utils
-pbr==5.6.0
+pbr==5.11.1
     # via
     #   -r requirements/base.txt
     #   stevedore
-psutil==5.8.0
+psutil==5.9.5
     # via
     #   -r requirements/base.txt
     #   edx-django-utils
-pyjwt==2.2.0
+pycparser==2.21
+    # via
+    #   -r requirements/base.txt
+    #   cffi
+pyjwt==2.6.0
     # via
     #   -r requirements/base.txt
     #   edx-rest-api-client
-pytz==2021.3
+pynacl==1.5.0
+    # via
+    #   -r requirements/base.txt
+    #   edx-django-utils
+pytz==2023.3
     # via
     #   -r requirements/base.txt
     #   celery
     #   django
-pyyaml==5.4.1
+pyyaml==6.0
     # via -r requirements/production.in
-redis==3.5.3
+redis==4.5.4
     # via -r requirements/base.txt
-requests==2.26.0
+requests==2.28.2
     # via
     #   -r requirements/base.txt
     #   edx-rest-api-client
     #   slumber
 six==1.16.0
     # via -r requirements/base.txt
 slumber==0.7.1
     # via
     #   -r requirements/base.txt
     #   edx-rest-api-client
-sqlparse==0.4.2
+sqlparse==0.4.4
     # via
     #   -r requirements/base.txt
     #   django
-stevedore==3.4.0
+stevedore==5.0.0
     # via
     #   -r requirements/base.txt
     #   edx-django-utils
-urllib3==1.26.7
+urllib3==1.26.15
     # via
     #   -r requirements/base.txt
     #   requests
 vine==1.3.0
     # via
     #   -r requirements/base.txt
     #   amqp
```

### Comparing `edx-ecommerce-worker-3.3.2/requirements/tox.txt` & `edx-ecommerce-worker-3.3.3/requirements/tox.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 #
-# This file is autogenerated by pip-compile
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    make upgrade
 #
-backports.entry-points-selectable==1.1.0
+distlib==0.3.6
     # via virtualenv
-distlib==0.3.3
-    # via virtualenv
-filelock==3.3.0
+filelock==3.12.0
     # via
     #   tox
     #   virtualenv
-packaging==21.0
+packaging==23.1
     # via tox
-platformdirs==2.4.0
+platformdirs==3.3.0
     # via virtualenv
 pluggy==1.0.0
     # via tox
-py==1.10.0
+py==1.11.0
     # via tox
-pyparsing==2.4.7
-    # via packaging
 six==1.16.0
-    # via
-    #   tox
-    #   virtualenv
-toml==0.10.2
     # via tox
-tox-battery==0.6.1
-    # via -r requirements/tox.in
-tox==3.24.4
+tomli==2.0.1
+    # via tox
+tox==3.28.0
     # via
+    #   -c requirements/common_constraints.txt
     #   -r requirements/tox.in
     #   tox-battery
-virtualenv==20.8.1
+tox-battery==0.6.1
+    # via -r requirements/tox.in
+virtualenv==20.22.0
     # via tox
```


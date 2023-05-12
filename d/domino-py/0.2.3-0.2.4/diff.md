# Comparing `tmp/domino-py-0.2.3.tar.gz` & `tmp/domino-py-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domino-py-0.2.3.tar", last modified: Wed May 10 21:43:23 2023, max compression
+gzip compressed data, was "domino-py-0.2.4.tar", last modified: Fri May 12 11:33:33 2023, max compression
```

## Comparing `domino-py-0.2.3.tar` & `domino-py-0.2.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:43:23.921459 domino-py-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-10 21:43:12.000000 domino-py-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10074 2023-05-10 21:43:23.921459 domino-py-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-10 21:43:12.000000 domino-py-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:43:23.917459 domino-py-0.2.3/domino/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14950 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/base_piece.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:43:23.917459 domino-py-0.2.3/domino/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:43:23.917459 domino-py-0.2.3/domino/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/cli/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17348 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/cli/utils/pieces_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    23722 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/cli/utils/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:43:23.917459 domino-py-0.2.3/domino/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/client/airflow_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/client/domino_backend_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/client/fs_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/client/github_rest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/client/local_files_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/client/s3_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:43:23.917459 domino-py-0.2.3/domino/custom_operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/custom_operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/custom_operators/docker_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/custom_operators/external_python_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17007 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/custom_operators/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/custom_operators/python_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:43:23.917459 domino-py-0.2.3/domino/custom_operators/sidecar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/custom_operators/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/custom_operators/sidecar/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/custom_operators/sidecar/mount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:43:23.917459 domino-py-0.2.3/domino/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/exceptions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:43:23.917459 domino-py-0.2.3/domino/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/schemas/container_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/schemas/deploy_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/schemas/from_upstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/schemas/piece_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/schemas/shared_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:43:23.921459 domino-py-0.2.3/domino/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/scripts/build_docker_images_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/scripts/create_docker_compose_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/scripts/docker_compose_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/scripts/docker_compose_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/scripts/load_piece.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/scripts/piece_dry_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/scripts/run_piece_bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/scripts/run_piece_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/scripts/run_piece_k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:43:23.921459 domino-py-0.2.3/domino/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/utils/metadata_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/utils/piece_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/utils/workflow_shared_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 21:43:13.000000 domino-py-0.2.3/domino/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:43:23.921459 domino-py-0.2.3/domino_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10074 2023-05-10 21:43:23.000000 domino-py-0.2.3/domino_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-10 21:43:23.000000 domino-py-0.2.3/domino_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 21:43:23.000000 domino-py-0.2.3/domino_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-10 21:43:23.000000 domino-py-0.2.3/domino_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-10 21:43:23.000000 domino-py-0.2.3/domino_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 21:43:23.000000 domino-py-0.2.3/domino_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 21:43:23.921459 domino-py-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-10 21:43:13.000000 domino-py-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:33:33.176880 domino-py-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-12 11:33:20.000000 domino-py-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10074 2023-05-12 11:33:33.176880 domino-py-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-12 11:33:20.000000 domino-py-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:33:33.168880 domino-py-0.2.4/domino/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14950 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/base_piece.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:33:33.168880 domino-py-0.2.4/domino/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:33:33.168880 domino-py-0.2.4/domino/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/cli/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17348 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/cli/utils/pieces_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24061 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/cli/utils/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:33:33.168880 domino-py-0.2.4/domino/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/client/airflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/client/domino_backend_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/client/fs_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/client/github_rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/client/local_files_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/client/s3_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:33:33.172880 domino-py-0.2.4/domino/custom_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/custom_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/custom_operators/docker_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/custom_operators/external_python_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17007 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/custom_operators/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/custom_operators/python_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:33:33.172880 domino-py-0.2.4/domino/custom_operators/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/custom_operators/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/custom_operators/sidecar/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/custom_operators/sidecar/mount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:33:33.172880 domino-py-0.2.4/domino/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/exceptions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:33:33.172880 domino-py-0.2.4/domino/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/schemas/container_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/schemas/deploy_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/schemas/from_upstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/schemas/piece_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/schemas/shared_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:33:33.172880 domino-py-0.2.4/domino/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/scripts/build_docker_images_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/scripts/create_docker_compose_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/scripts/docker_compose_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/scripts/docker_compose_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/scripts/load_piece.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/scripts/piece_dry_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/scripts/run_piece_bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/scripts/run_piece_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/scripts/run_piece_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:33:33.172880 domino-py-0.2.4/domino/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/utils/metadata_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/utils/piece_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/utils/workflow_shared_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-12 11:33:21.000000 domino-py-0.2.4/domino/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:33:33.176880 domino-py-0.2.4/domino_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10074 2023-05-12 11:33:32.000000 domino-py-0.2.4/domino_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-12 11:33:33.000000 domino-py-0.2.4/domino_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 11:33:32.000000 domino-py-0.2.4/domino_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 11:33:32.000000 domino-py-0.2.4/domino_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-12 11:33:32.000000 domino-py-0.2.4/domino_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 11:33:32.000000 domino-py-0.2.4/domino_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 11:33:33.176880 domino-py-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-12 11:33:21.000000 domino-py-0.2.4/setup.py
```

### Comparing `domino-py-0.2.3/LICENSE` & `domino-py-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/PKG-INFO` & `domino-py-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domino-py
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python package for the Domino platform
 Home-page: UNKNOWN
 Author: Luiz Tauffer and Vinicius Vaz
 Author-email: luiz@taufferconsulting.com
 License: UNKNOWN
 Description:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: domino-py Version: 0.2.3 Summary: Python package
+Metadata-Version: 2.1 Name: domino-py Version: 0.2.4 Summary: Python package
 for the Domino platform Home-page: UNKNOWN Author: Luiz Tauffer and Vinicius
 Vaz Author-email: luiz@taufferconsulting.com License: UNKNOWN Description:
    [https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/media/
                                    logo.png]
                     [https://img.shields.io/pypi/v/domino-
   py?color=%231BA331&label=PyPI&logo=python&logoColor=%23F7F991%20] [https://
  img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/domino]
```

### Comparing `domino-py-0.2.3/README.md` & `domino-py-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/base_piece.py` & `domino-py-0.2.4/domino/base_piece.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/cli/cli.py` & `domino-py-0.2.4/domino/cli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -166,17 +166,23 @@
 @click.command()
 @click.option(
     "--d",
     is_flag=True,
     help="Run in detached mode.",
     default=False
 )
-def cli_run_platform_compose(d):
+@click.option(
+    '--use-config-file',
+    is_flag=True,
+    help="Use config file to run platform.",
+    default=False
+)
+def cli_run_platform_compose(d, use_config_file):
     """Run Domino platform locally with docker compose. Do NOT use this in production."""
-    platform.run_platform_compose(detached=d)
+    platform.run_platform_compose(detached=d, use_config_file=use_config_file)
 
 
 @click.group()
 @click.pass_context
 def cli_platform(ctx):
     """Domino platform actions"""
     if ctx.invoked_subcommand == "prepare":
```

### Comparing `domino-py-0.2.3/domino/cli/utils/pieces_repository.py` & `domino-py-0.2.4/domino/cli/utils/pieces_repository.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/cli/utils/platform.py` & `domino-py-0.2.4/domino/cli/utils/platform.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,26 +64,24 @@
         config_dict = tomli.load(f)
     
     running_path = str(Path().cwd().resolve())
     config_dict["path"]["DOMINO_LOCAL_RUNNING_PATH"] = running_path
     config_dict["kind"]["DOMINO_KIND_CLUSTER_NAME"] = cluster_name
     config_dict['kind']['DOMINO_DEPLOY_MODE'] = deploy_mode
 
-    config_dict['local_pieces_repositories'] = {}
-    config_dict['local_domino_package'] = {"DOMINO_LOCAL_DOMINO_PACKAGE": ""}
     if deploy_mode == 'local-k8s-dev':
-        config_dict['local_domino_package']['DOMINO_LOCAL_DOMINO_PACKAGE'] = local_domino_path
+        config_dict['dev']['DOMINO_LOCAL_DOMINO_PACKAGE'] = local_domino_path
         for local_pieces_repository in local_pieces_repository_path:
             # Read repo config.toml to get repo name to map it to cluster path
             repo_config_file_path = Path(local_pieces_repository).resolve() / "config.toml"
             with open(str(repo_config_file_path), "rb") as f:
                 repo_toml = tomli.load(f)
             
             repo_name = repo_toml['repository']['REPOSITORY_NAME'] 
-            config_dict['local_pieces_repositories'][repo_name] = local_pieces_repository
+            config_dict['dev'][repo_name] = local_pieces_repository
 
     config_dict['github']['DOMINO_GITHUB_WORKFLOWS_REPOSITORY'] = workflows_repository.split("github.com/")[-1].strip('/')
 
     if not github_workflows_ssh_private_key:
         private_key, public_key = create_ssh_pair_key()
         config_dict["github"]["DOMINO_GITHUB_WORKFLOWS_SSH_PRIVATE_KEY"] = base64.b64encode(private_key).decode('utf-8')
         config_dict["github"]["DOMINO_GITHUB_WORKFLOWS_SSH_PUBLIC_KEY"] = public_key.decode("utf-8")
@@ -114,28 +112,31 @@
         nodeRegistration=dict(
             kubeletExtraArgs={
                 "node-labels": "ingress-ready=true"
             }
         )
     )
     extra_mounts_local_repositories = []
+
+    local_pieces_respositories = {key: value for key, value in platform_config['dev'].items() if key != "DOMINO_LOCAL_DOMINO_PACKAGE"}
     if platform_config['kind']['DOMINO_DEPLOY_MODE'] == 'local-k8s-dev':
-        for repo_name, repo_path in platform_config['local_pieces_repositories'].items():
+        #for repo_name, repo_path in platform_config['local_pieces_repositories'].items():
+        for repo_name, repo_path in local_pieces_respositories.items():
             extra_mounts_local_repositories.append(
                 dict(
                     hostPath=repo_path,
                     containerPath=f"/pieces_repositories/{repo_name}",
                     readOnly=True,
                     propagation='HostToContainer'
                 )
             )
-        if platform_config['local_domino_package'].get('DOMINO_LOCAL_DOMINO_PACKAGE'):
+        if platform_config['dev'].get('DOMINO_LOCAL_DOMINO_PACKAGE'):
             extra_mounts_local_repositories.append(
                 dict(
-                    hostPath=platform_config['local_domino_package']['DOMINO_LOCAL_DOMINO_PACKAGE'],
+                    hostPath=platform_config['dev']['DOMINO_LOCAL_DOMINO_PACKAGE'],
                     containerPath=f"/domino/domino_py",
                     readOnly=True,
                     propagation='HostToContainer'
                 )
             )
 
     kubeadm_parsed = AsLiteral(yaml.dump(kubeadm_config_patches))
@@ -241,15 +242,15 @@
     )
     airflow_ssh_config_parsed = AsLiteral(yaml.dump(airflow_ssh_config))
 
     workers_extra_volumes = []
     workers_extra_volumes_mounts = []
     workers = {}
     scheduler = {}
-    if platform_config['kind']["DOMINO_DEPLOY_MODE"] == 'local-k8s-dev' and platform_config['local_domino_package'].get('DOMINO_LOCAL_DOMINO_PACKAGE'):
+    if platform_config['kind']["DOMINO_DEPLOY_MODE"] == 'local-k8s-dev' and platform_config['dev'].get('DOMINO_LOCAL_DOMINO_PACKAGE'):
         workers_extra_volumes = [
             {
                 "name": "domino-dev-extra",
                 "persistentVolumeClaim": {
                     "claimName": "domino-dev-volume-claim"
                 }
             }
@@ -398,15 +399,15 @@
                 name="cluster-admin",
                 api_group="rbac.authorization.k8s.io"
             )
         )
         console.print('Creating RBAC Scheduler Authorization for local dev')
         v1.create_cluster_role_binding(cluster_role_binding_scheduler)
 
-        for project_name in platform_config["local_pieces_repositories"].keys():
+        for project_name in local_pieces_respositories.keys():
             console.log(f"Creating PV and PVC for {project_name}...")
             # Check if pv already exists
             persistent_volume_name = 'pv-{}'.format(str(project_name.lower().replace('_', '-')))
             persistent_volume_claim_name = 'pvc-{}'.format(str(project_name.lower().replace('_', '-')))
             pvc_exists = False
             try:
                 k8s_client.read_namespaced_persistent_volume_claim(name=persistent_volume_claim_name, namespace='default')
@@ -466,15 +467,15 @@
                                 ]
                             )
                         )
                     )
                 )
                 k8s_client.create_persistent_volume(body=pv)
         
-        if platform_config['local_domino_package'].get('DOMINO_LOCAL_DOMINO_PACKAGE'):
+        if platform_config['dev'].get('DOMINO_LOCAL_DOMINO_PACKAGE'):
             console.print("Creating PV's and PVC's for Local Domino Package...")
             # Create pv and pvc for local dev domino
             pvc = client.V1PersistentVolumeClaim(
                 metadata=client.V1ObjectMeta(name="domino-dev-volume-claim"),
                 spec=client.V1PersistentVolumeClaimSpec(
                     access_modes=["ReadWriteMany"],
                     volume_name="domino-dev-volume",
@@ -518,15 +519,22 @@
     console.print("")
     console.print("K8s resources created successfully!", style=f"bold {COLOR_PALETTE.get('success')}")
 
     console.print("You can now access the Domino frontend at: http://localhost/")
     console.print("and the Backend API at: http://localhost/api/")
 
 
-def run_platform_compose(detached: bool = False):
+def run_platform_compose(detached: bool = False, use_config_file: bool = False) -> None:
+    if use_config_file:
+        console.print("Using config file...")
+        with open("config-domino-local.toml", "rb") as f:
+            platform_config = tomli.load(f)
+        token_pieces = platform_config["github"].get("DOMINO_DEFAULT_PIECES_REPOSITORY_TOKEN")
+        os.environ['DOMINO_DEFAULT_PIECES_REPOSITORY_TOKEN'] = token_pieces
+
     # Create local directories
     local_path = Path(".").resolve()
     domino_dir = local_path / "domino_data"
     domino_dir.mkdir(parents=True, exist_ok=True)
     subprocess.run(["chmod", "-R", "777", "domino_data"])
     airflow_logs_dir = local_path / "airflow/logs"
     airflow_logs_dir.mkdir(parents=True, exist_ok=True)
```

### Comparing `domino-py-0.2.3/domino/client/airflow_client.py` & `domino-py-0.2.4/domino/client/airflow_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/client/domino_backend_client.py` & `domino-py-0.2.4/domino/client/domino_backend_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/client/fs_client.py` & `domino-py-0.2.4/domino/client/fs_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/client/github_rest_client.py` & `domino-py-0.2.4/domino/client/github_rest_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/client/local_files_client.py` & `domino-py-0.2.4/domino/client/local_files_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/client/s3_client.py` & `domino-py-0.2.4/domino/client/s3_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/custom_operators/docker_operator.py` & `domino-py-0.2.4/domino/custom_operators/docker_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/custom_operators/external_python_operator.py` & `domino-py-0.2.4/domino/custom_operators/external_python_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/custom_operators/k8s_operator.py` & `domino-py-0.2.4/domino/custom_operators/k8s_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/custom_operators/python_operator.py` & `domino-py-0.2.4/domino/custom_operators/python_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/custom_operators/sidecar/logger.py` & `domino-py-0.2.4/domino/custom_operators/sidecar/logger.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/custom_operators/sidecar/mount.py` & `domino-py-0.2.4/domino/custom_operators/sidecar/mount.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/exceptions/exceptions.py` & `domino-py-0.2.4/domino/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/logger.py` & `domino-py-0.2.4/domino/logger.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/schemas/piece_metadata.py` & `domino-py-0.2.4/domino/schemas/piece_metadata.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/schemas/shared_storage.py` & `domino-py-0.2.4/domino/schemas/shared_storage.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/scripts/build_docker_images_pieces.py` & `domino-py-0.2.4/domino/scripts/build_docker_images_pieces.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/scripts/create_docker_compose_file.py` & `domino-py-0.2.4/domino/scripts/create_docker_compose_file.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/scripts/docker_compose_constants.py` & `domino-py-0.2.4/domino/scripts/docker_compose_constants.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/scripts/docker_compose_scripts.py` & `domino-py-0.2.4/domino/scripts/docker_compose_scripts.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/scripts/load_piece.py` & `domino-py-0.2.4/domino/scripts/load_piece.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/scripts/piece_dry_run.py` & `domino-py-0.2.4/domino/scripts/piece_dry_run.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/scripts/run_piece_bash.py` & `domino-py-0.2.4/domino/scripts/run_piece_bash.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/scripts/run_piece_docker.py` & `domino-py-0.2.4/domino/scripts/run_piece_docker.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/scripts/run_piece_k8s.py` & `domino-py-0.2.4/domino/scripts/run_piece_k8s.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino/task.py` & `domino-py-0.2.4/domino/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,16 +195,16 @@
                 workflow_shared_storage=self.workflow_shared_storage,
                 namespace='default',  # TODO - separate namespace by User or Workspace?
                 image=self.piece["source_image"],
                 image_pull_policy='IfNotPresent',
                 task_id=self.task_id,
                 name=f"airflow-worker-pod-{self.task_id}",
                 startup_timeout_seconds=pod_startup_timeout_in_seconds,
-                # cmds=["python"],
-                # arguments=["-c", "'import time; time.sleep(10000)'"],
+                #cmds=["/bin/bash"],
+                #arguments=["-c", "sleep 120;"],
                 cmds=["domino"],
                 arguments=["run-piece-k8s"],
                 env_vars=container_env_vars,
                 do_xcom_push=True,
                 in_cluster=True,
                 volumes=all_volumes,
                 volume_mounts=all_volume_mounts,
```

### Comparing `domino-py-0.2.3/domino/utils/piece_generator.py` & `domino-py-0.2.4/domino/utils/piece_generator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/domino_py.egg-info/PKG-INFO` & `domino-py-0.2.4/domino_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domino-py
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python package for the Domino platform
 Home-page: UNKNOWN
 Author: Luiz Tauffer and Vinicius Vaz
 Author-email: luiz@taufferconsulting.com
 License: UNKNOWN
 Description:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: domino-py Version: 0.2.3 Summary: Python package
+Metadata-Version: 2.1 Name: domino-py Version: 0.2.4 Summary: Python package
 for the Domino platform Home-page: UNKNOWN Author: Luiz Tauffer and Vinicius
 Vaz Author-email: luiz@taufferconsulting.com License: UNKNOWN Description:
    [https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/media/
                                    logo.png]
                     [https://img.shields.io/pypi/v/domino-
   py?color=%231BA331&label=PyPI&logo=python&logoColor=%23F7F991%20] [https://
  img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/domino]
```

### Comparing `domino-py-0.2.3/domino_py.egg-info/SOURCES.txt` & `domino-py-0.2.4/domino_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.3/setup.py` & `domino-py-0.2.4/setup.py`

 * *Files identical despite different names*


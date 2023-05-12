# Comparing `tmp/quickmpc-0.3.7.tar.gz` & `tmp/quickmpc-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/QuickMPC/QuickMPC/packages/client/libclient-py/dist/.tmp-zuipom8n/quickmpc-0.3.7.tar", last modified: Mon Apr 24 10:55:36 2023, max compression
+gzip compressed data, was "/home/runner/work/QuickMPC/QuickMPC/packages/client/libclient-py/dist/.tmp-h0e_0g5r/quickmpc-0.3.8.tar", last modified: Fri May 12 10:42:14 2023, max compression
```

## Comparing `quickmpc-0.3.7.tar` & `quickmpc-0.3.8.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:55:36.000000 quickmpc-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-24 10:55:19.000000 quickmpc-0.3.7/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-24 10:55:19.000000 quickmpc-0.3.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-24 10:55:19.000000 quickmpc-0.3.7/.isort.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:55:36.000000 quickmpc-0.3.7/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-24 10:55:19.000000 quickmpc-0.3.7/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 10:55:19.000000 quickmpc-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-24 10:55:19.000000 quickmpc-0.3.7/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-24 10:55:36.000000 quickmpc-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-24 10:55:19.000000 quickmpc-0.3.7/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    38604 2023-04-24 10:55:19.000000 quickmpc-0.3.7/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-24 10:55:19.000000 quickmpc-0.3.7/README-ja.md
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-24 10:55:19.000000 quickmpc-0.3.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-24 10:55:19.000000 quickmpc-0.3.7/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-24 10:55:19.000000 quickmpc-0.3.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:55:36.000000 quickmpc-0.3.7/quickmpc/
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-04-24 10:55:19.000000 quickmpc-0.3.7/quickmpc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-24 10:55:19.000000 quickmpc-0.3.7/quickmpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 10:55:36.000000 quickmpc-0.3.7/quickmpc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-24 10:55:19.000000 quickmpc-0.3.7/quickmpc/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:55:36.000000 quickmpc-0.3.7/quickmpc/proto/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-24 10:55:19.000000 quickmpc-0.3.7/quickmpc/proto/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-24 10:55:19.000000 quickmpc-0.3.7/quickmpc/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:55:36.000000 quickmpc-0.3.7/quickmpc/proto/common_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:55:19.000000 quickmpc-0.3.7/quickmpc/proto/common_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-04-24 10:55:19.000000 quickmpc-0.3.7/quickmpc/proto/common_types/common_types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-04-24 10:55:19.000000 quickmpc-0.3.7/quickmpc/proto/common_types/common_types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12545 2023-04-24 10:55:19.000000 quickmpc-0.3.7/quickmpc/proto/libc_to_manage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13730 2023-04-24 10:55:19.000000 quickmpc-0.3.7/quickmpc/proto/libc_to_manage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-04-24 10:55:19.000000 quickmpc-0.3.7/quickmpc/proto/libc_to_manage_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-24 10:55:19.000000 quickmpc-0.3.7/quickmpc/proto/libc_to_manage_pb2_grpc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-04-24 10:55:19.000000 quickmpc-0.3.7/quickmpc/qmpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18252 2023-04-24 10:55:19.000000 quickmpc-0.3.7/quickmpc/qmpc_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-04-24 10:55:19.000000 quickmpc-0.3.7/quickmpc/share.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:55:36.000000 quickmpc-0.3.7/quickmpc/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:55:19.000000 quickmpc-0.3.7/quickmpc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-24 10:55:19.000000 quickmpc-0.3.7/quickmpc/utils/if_present.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-04-24 10:55:19.000000 quickmpc-0.3.7/quickmpc/utils/make_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-24 10:55:19.000000 quickmpc-0.3.7/quickmpc/utils/overload_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-04-24 10:55:19.000000 quickmpc-0.3.7/quickmpc/utils/parse_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-24 10:55:19.000000 quickmpc-0.3.7/quickmpc/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-24 10:55:19.000000 quickmpc-0.3.7/quickmpc/utils/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-24 10:55:19.000000 quickmpc-0.3.7/quickmpc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:55:36.000000 quickmpc-0.3.7/quickmpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-24 10:55:36.000000 quickmpc-0.3.7/quickmpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-24 10:55:36.000000 quickmpc-0.3.7/quickmpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 10:55:36.000000 quickmpc-0.3.7/quickmpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-24 10:55:36.000000 quickmpc-0.3.7/quickmpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-24 10:55:36.000000 quickmpc-0.3.7/quickmpc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-24 10:55:36.000000 quickmpc-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-24 10:55:19.000000 quickmpc-0.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:55:36.000000 quickmpc-0.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:55:36.000000 quickmpc-0.3.7/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:55:36.000000 quickmpc-0.3.7/tests/unit_tests/certificates/
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/certificates/server1.key
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/certificates/server1.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/certificates/server2.key
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/certificates/server2.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/certificates/server3.key
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/certificates/server3.pem
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/local_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:55:36.000000 quickmpc-0.3.7/tests/unit_tests/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/test_files/bitvector.csv
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/test_files/diff_col.csv
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/test_files/edge_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/test_files/empty.csv
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/test_files/none.csv
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/test_files/normal.csv
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/test_files/not_csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/test_files/over_number.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/test_files/string_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/test_make_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/test_over_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/test_qmpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/test_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/test_share_recons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tests/unit_tests/test_share_sharize.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-24 10:55:19.000000 quickmpc-0.3.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:42:14.000000 quickmpc-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-12 10:41:59.000000 quickmpc-0.3.8/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-12 10:41:59.000000 quickmpc-0.3.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-12 10:41:59.000000 quickmpc-0.3.8/.isort.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:42:14.000000 quickmpc-0.3.8/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-12 10:41:59.000000 quickmpc-0.3.8/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-12 10:41:59.000000 quickmpc-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-12 10:41:59.000000 quickmpc-0.3.8/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-12 10:42:14.000000 quickmpc-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-12 10:41:59.000000 quickmpc-0.3.8/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    38604 2023-05-12 10:41:59.000000 quickmpc-0.3.8/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-12 10:41:59.000000 quickmpc-0.3.8/README-ja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-12 10:41:59.000000 quickmpc-0.3.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-12 10:41:59.000000 quickmpc-0.3.8/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-12 10:41:59.000000 quickmpc-0.3.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:42:14.000000 quickmpc-0.3.8/quickmpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-05-12 10:41:59.000000 quickmpc-0.3.8/quickmpc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-12 10:41:59.000000 quickmpc-0.3.8/quickmpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-12 10:42:14.000000 quickmpc-0.3.8/quickmpc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-12 10:41:59.000000 quickmpc-0.3.8/quickmpc/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:42:14.000000 quickmpc-0.3.8/quickmpc/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-12 10:41:59.000000 quickmpc-0.3.8/quickmpc/proto/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-12 10:41:59.000000 quickmpc-0.3.8/quickmpc/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:42:14.000000 quickmpc-0.3.8/quickmpc/proto/common_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 10:41:59.000000 quickmpc-0.3.8/quickmpc/proto/common_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-05-12 10:41:59.000000 quickmpc-0.3.8/quickmpc/proto/common_types/common_types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-05-12 10:41:59.000000 quickmpc-0.3.8/quickmpc/proto/common_types/common_types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12545 2023-05-12 10:41:59.000000 quickmpc-0.3.8/quickmpc/proto/libc_to_manage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13730 2023-05-12 10:41:59.000000 quickmpc-0.3.8/quickmpc/proto/libc_to_manage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-05-12 10:41:59.000000 quickmpc-0.3.8/quickmpc/proto/libc_to_manage_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-05-12 10:41:59.000000 quickmpc-0.3.8/quickmpc/proto/libc_to_manage_pb2_grpc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-05-12 10:41:59.000000 quickmpc-0.3.8/quickmpc/qmpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18224 2023-05-12 10:41:59.000000 quickmpc-0.3.8/quickmpc/qmpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-05-12 10:41:59.000000 quickmpc-0.3.8/quickmpc/share.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:42:14.000000 quickmpc-0.3.8/quickmpc/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 10:41:59.000000 quickmpc-0.3.8/quickmpc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-12 10:41:59.000000 quickmpc-0.3.8/quickmpc/utils/if_present.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-12 10:41:59.000000 quickmpc-0.3.8/quickmpc/utils/make_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-12 10:41:59.000000 quickmpc-0.3.8/quickmpc/utils/overload_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-05-12 10:41:59.000000 quickmpc-0.3.8/quickmpc/utils/parse_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-12 10:41:59.000000 quickmpc-0.3.8/quickmpc/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-12 10:41:59.000000 quickmpc-0.3.8/quickmpc/utils/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-12 10:41:59.000000 quickmpc-0.3.8/quickmpc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:42:14.000000 quickmpc-0.3.8/quickmpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-12 10:42:14.000000 quickmpc-0.3.8/quickmpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-12 10:42:14.000000 quickmpc-0.3.8/quickmpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:42:14.000000 quickmpc-0.3.8/quickmpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-12 10:42:14.000000 quickmpc-0.3.8/quickmpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-12 10:42:14.000000 quickmpc-0.3.8/quickmpc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-12 10:42:14.000000 quickmpc-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-12 10:41:59.000000 quickmpc-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:42:14.000000 quickmpc-0.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:42:14.000000 quickmpc-0.3.8/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:42:14.000000 quickmpc-0.3.8/tests/unit_tests/certificates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/certificates/server1.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/certificates/server1.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/certificates/server2.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/certificates/server2.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/certificates/server3.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/certificates/server3.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/local_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:42:14.000000 quickmpc-0.3.8/tests/unit_tests/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/test_files/bitvector.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/test_files/diff_col.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/test_files/edge_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/test_files/empty.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/test_files/none.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/test_files/normal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/test_files/not_csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/test_files/over_number.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/test_files/string_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/test_make_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/test_over_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/test_qmpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/test_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/test_share_recons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tests/unit_tests/test_share_sharize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-12 10:41:59.000000 quickmpc-0.3.8/tox.ini
```

### Comparing `quickmpc-0.3.7/.vscode/settings.json` & `quickmpc-0.3.8/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/LICENSE` & `quickmpc-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/Pipfile.lock` & `quickmpc-0.3.8/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/README-ja.md` & `quickmpc-0.3.8/README-ja.md`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/README.md` & `quickmpc-0.3.8/README.md`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ## Install Package
+
 ### Develop
 ```console
 $ git clone https://github.com/acompany-develop/QuickMPC-libClient-py.git
 $ cd QuickMPC-libClient-py
 $ pipenv sync --dev
 ```
 
 ## unit_test
-
 ### Testing all cases
 ```console
 $ pipenv run tox
 ```
 Testing and syntax checking will be performed on Python 3.7, 3.8, and 3.9.
 
 ### Testing with Python 3.7
```

### Comparing `quickmpc-0.3.7/mypy.ini` & `quickmpc-0.3.8/mypy.ini`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/quickmpc/README.md` & `quickmpc-0.3.8/quickmpc/README.md`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/quickmpc/proto/common_types/common_types_pb2.py` & `quickmpc-0.3.8/quickmpc/proto/common_types/common_types_pb2.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/quickmpc/proto/common_types/common_types_pb2.pyi` & `quickmpc-0.3.8/quickmpc/proto/common_types/common_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/quickmpc/proto/libc_to_manage_pb2.py` & `quickmpc-0.3.8/quickmpc/proto/libc_to_manage_pb2.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/quickmpc/proto/libc_to_manage_pb2.pyi` & `quickmpc-0.3.8/quickmpc/proto/libc_to_manage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/quickmpc/proto/libc_to_manage_pb2_grpc.py` & `quickmpc-0.3.8/quickmpc/proto/libc_to_manage_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/quickmpc/proto/libc_to_manage_pb2_grpc.pyi` & `quickmpc-0.3.8/quickmpc/proto/libc_to_manage_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/quickmpc/qmpc.py` & `quickmpc-0.3.8/quickmpc/qmpc.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/quickmpc/qmpc_server.py` & `quickmpc-0.3.8/quickmpc/qmpc_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,33 +241,32 @@
             secrets, key=lambda row: row[matching_column - 1])
         # pieceに分けてシェア化
         pieces: list = MakePiece.make_pieces(
             sorted_secrets, int(piece_size / 10))
         data_id: str = hashlib.sha256(
             str(sorted_secrets).encode() + struct.pack('d', time.time())
         ).hexdigest()
-        shares = [Share.sharize(s, self.__party_size)
-                  for s in tqdm.tqdm(pieces, desc='sharize')]
-        sent_at = str(datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S'))
 
         # リクエストパラメータを設定して非同期にリクエスト送信
+        sent_at = str(datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S'))
+        futures: list = []
         with ThreadPoolExecutor() as executor:
-            futures = [executor.submit(self.__retry,
-                                       stub.SendShares,
-                                       SendSharesRequest(
-                                           data_id=data_id,
-                                           shares=json.dumps(s),
-                                           schema=typed_schema,
-                                           piece_id=piece_id,
-                                           sent_at=sent_at,
-                                           matching_column=matching_column,
-                                           token=self.token))
-                       for piece_id, share_piece in enumerate(shares)
-                       for stub, s in zip(self.__client_stubs, share_piece)
-                       ]
+            for piece_id, p in enumerate(tqdm.tqdm(pieces, desc='sharize')):
+                shares = Share.sharize(p, self.__party_size)
+                for stub, s in zip(self.__client_stubs, shares):
+                    req = SendSharesRequest(data_id=data_id,
+                                            shares=json.dumps(s),
+                                            schema=typed_schema,
+                                            piece_id=piece_id,
+                                            sent_at=sent_at,
+                                            matching_column=matching_column,
+                                            token=self.token)
+                    futures.append(executor.submit(self.__retry,
+                                                   stub.SendShares,
+                                                   req))
         is_ok, _ = QMPCServer.__futures_result(futures)
         return {"is_ok": is_ok, "data_id": data_id}
 
     def delete_share(self, data_ids: List[str]) -> Dict:
         """ Shareを削除 """
         req = DeleteSharesRequest(dataIds=data_ids, token=self.token)
         # 非同期にリクエスト送信
```

### Comparing `quickmpc-0.3.7/quickmpc/share.py` & `quickmpc-0.3.8/quickmpc/share.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/quickmpc/utils/make_pieces.py` & `quickmpc-0.3.8/quickmpc/utils/make_pieces.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/quickmpc/utils/overload_tools.py` & `quickmpc-0.3.8/quickmpc/utils/overload_tools.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/quickmpc/utils/parse_csv.py` & `quickmpc-0.3.8/quickmpc/utils/parse_csv.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import csv
 import logging
 from dataclasses import dataclass
 from hashlib import sha512
-from typing import Dict, List, Optional, Sequence, Tuple, Union
+from typing import Dict, Iterable, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 
 from ..exception import ArgumentError
 from ..proto.common_types.common_types_pb2 import Schema, ShareValueTypeEnum
 from .overload_tools import Dim1, methoddispatch
 
@@ -119,16 +119,15 @@
 
 
 def find_types(schema: List[str],
                data: List[List[str]],
                matching_column: Optional[int] = None
                ) -> List[ShareValueTypeEnum.ValueType]:
     # transpose to get column oriented list
-    transposed: List[List[str]] = np.array(
-        data, dtype=str).transpose().tolist()
+    transposed: Iterable[List[str]] = map(list, zip(*data))
     return [find_type(sch, col, idx == matching_column)
             for idx, (sch, col) in enumerate(zip(schema, transposed), start=1)]
 
 
 def convert(element: str,
             type_info: ShareValueTypeEnum.ValueType) -> ShareValueType:
     if type_info == ShareValueTypeEnum.Value('SHARE_VALUE_TYPE_FIXED_POINT'):
```

### Comparing `quickmpc-0.3.7/quickmpc/utils/random.py` & `quickmpc-0.3.8/quickmpc/utils/random.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/quickmpc/utils/restore.py` & `quickmpc-0.3.8/quickmpc/utils/restore.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/quickmpc.egg-info/SOURCES.txt` & `quickmpc-0.3.8/quickmpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/tests/unit_tests/certificates/server1.key` & `quickmpc-0.3.8/tests/unit_tests/certificates/server1.key`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/tests/unit_tests/certificates/server1.pem` & `quickmpc-0.3.8/tests/unit_tests/certificates/server1.pem`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/tests/unit_tests/certificates/server2.key` & `quickmpc-0.3.8/tests/unit_tests/certificates/server2.key`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/tests/unit_tests/certificates/server2.pem` & `quickmpc-0.3.8/tests/unit_tests/certificates/server2.pem`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/tests/unit_tests/certificates/server3.key` & `quickmpc-0.3.8/tests/unit_tests/certificates/server3.key`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/tests/unit_tests/certificates/server3.pem` & `quickmpc-0.3.8/tests/unit_tests/certificates/server3.pem`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/tests/unit_tests/conftest.py` & `quickmpc-0.3.8/tests/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/tests/unit_tests/local_server.py` & `quickmpc-0.3.8/tests/unit_tests/local_server.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/tests/unit_tests/test_files/edge_data.csv` & `quickmpc-0.3.8/tests/unit_tests/test_files/edge_data.csv`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/tests/unit_tests/test_files/string_data.csv` & `quickmpc-0.3.8/tests/unit_tests/test_files/string_data.csv`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/tests/unit_tests/test_make_pieces.py` & `quickmpc-0.3.8/tests/unit_tests/test_make_pieces.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/tests/unit_tests/test_over_load.py` & `quickmpc-0.3.8/tests/unit_tests/test_over_load.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/tests/unit_tests/test_parse.py` & `quickmpc-0.3.8/tests/unit_tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/tests/unit_tests/test_qmpc.py` & `quickmpc-0.3.8/tests/unit_tests/test_qmpc.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/tests/unit_tests/test_random.py` & `quickmpc-0.3.8/tests/unit_tests/test_random.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/tests/unit_tests/test_restore.py` & `quickmpc-0.3.8/tests/unit_tests/test_restore.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/tests/unit_tests/test_share_recons.py` & `quickmpc-0.3.8/tests/unit_tests/test_share_recons.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.7/tests/unit_tests/test_share_sharize.py` & `quickmpc-0.3.8/tests/unit_tests/test_share_sharize.py`

 * *Files identical despite different names*


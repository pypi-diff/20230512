# Comparing `tmp/hyperparameter-0.4.3.tar.gz` & `tmp/hyperparameter-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperparameter-0.4.3.tar", last modified: Wed Dec  7 07:10:31 2022, max compression
+gzip compressed data
```

## Comparing `hyperparameter-0.4.3.tar` & `hyperparameter-0.5.0.tar`

### file list

```diff
@@ -1,69 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 07:10:31.884719 hyperparameter-0.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 07:10:31.876719 hyperparameter-0.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 07:10:31.880719 hyperparameter-0.4.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 07:10:31.880719 hyperparameter-0.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/.github/workflows/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      845 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/.github/workflows/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      356 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2022-12-07 07:10:31.884719 hyperparameter-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/README.zh.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 07:10:31.880719 hyperparameter-0.4.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 07:10:31.880719 hyperparameter-0.4.3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/docs/examples/optimization.md
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/docs/examples/optimization.zh.md
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/docs/index.zh.md
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/docs/quick_start.md
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/docs/quick_start.zh.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/docs/reference.md
--rw-r--r--   0 runner    (1001) docker     (123)      110 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6738 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/docs/structured_parameter.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 07:10:31.876719 hyperparameter-0.4.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 07:10:31.880719 hyperparameter-0.4.3/examples/application/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/examples/application/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      789 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/examples/application/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/examples/application/cfg.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 07:10:31.880719 hyperparameter-0.4.3/examples/automl_optuna_mnist/
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/examples/automl_optuna_mnist/automl_mnist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 07:10:31.880719 hyperparameter-0.4.3/examples/mnist/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/examples/mnist/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/examples/mnist/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5899 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/examples/mnist/main_with_hp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/examples/mnist/main_with_hp_with_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/examples/mnist/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 07:10:31.880719 hyperparameter-0.4.3/examples/optuna/
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/examples/optuna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      230 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/examples/optuna/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/examples/optuna/example_hp.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/examples/optuna/example_hp_nested.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 07:10:31.884719 hyperparameter-0.4.3/examples/sparse_lr/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/examples/sparse_lr/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      581 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/examples/sparse_lr/example_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/examples/sparse_lr/example_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/examples/sparse_lr/example_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/examples/sparse_lr/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 07:10:31.884719 hyperparameter-0.4.3/hparam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/hparam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/hparam/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 07:10:31.884719 hyperparameter-0.4.3/hyperparameter/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/hyperparameter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15805 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/hyperparameter/hyperparameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/hyperparameter/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/hyperparameter/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/hyperparameter/tune.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 07:10:31.884719 hyperparameter-0.4.3/hyperparameter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2022-12-07 07:10:31.000000 hyperparameter-0.4.3/hyperparameter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2022-12-07 07:10:31.000000 hyperparameter-0.4.3/hyperparameter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 07:10:31.000000 hyperparameter-0.4.3/hyperparameter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-07 07:10:31.000000 hyperparameter-0.4.3/hyperparameter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      948 2022-12-07 07:10:18.000000 hyperparameter-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-07 07:10:31.884719 hyperparameter-0.4.3/setup.cfg
+-rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 hyperparameter-0.5.0/Cargo.toml
+-rw-r--r--   0     1001      123      834 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0     1001      123      126 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0     1001      123      595 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0     1001      123      706 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/.github/workflows/codecov.yml
+-rw-r--r--   0     1001      123      845 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/.github/workflows/mkdocs.yml
+-rw-r--r--   0     1001      123     1202 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/.github/workflows/python-publish.yml
+-rw-r--r--   0     1001      123     2001 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/.gitignore
+-rw-r--r--   0     1001      123      356 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123     5202 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      123     9722 2023-05-12 09:08:52.000000 hyperparameter-0.5.0/Cargo.lock
+-rw-r--r--   0     1001      123    11356 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/LICENSE
+-rw-r--r--   0     1001      123     3861 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/README.md
+-rw-r--r--   0     1001      123     3457 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/README.zh.md
+-rw-r--r--   0     1001      123     2846 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/docs/examples/optimization.md
+-rw-r--r--   0     1001      123     2868 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/docs/examples/optimization.zh.md
+-rw-r--r--   0     1001      123     3861 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/docs/index.md
+-rw-r--r--   0     1001      123     3457 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/docs/index.zh.md
+-rw-r--r--   0     1001      123     3000 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/docs/quick_start.md
+-rw-r--r--   0     1001      123     3000 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/docs/quick_start.zh.md
+-rw-r--r--   0     1001      123       48 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/docs/reference.md
+-rw-r--r--   0     1001      123      110 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/docs/requirements.txt
+-rw-r--r--   0     1001      123     6738 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/docs/structured_parameter.md
+-rw-r--r--   0     1001      123      337 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/application/README.md
+-rw-r--r--   0     1001      123      789 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/application/app.py
+-rw-r--r--   0     1001      123       46 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/application/cfg.json
+-rw-r--r--   0     1001      123     4733 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/automl_optuna_mnist/automl_mnist.py
+-rw-r--r--   0     1001      123     1382 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/cpp/cxx_test.cc
+-rw-r--r--   0     1001      123       96 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/cpp/cxx_test.py
+-rw-r--r--   0     1001      123      237 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/cpp/cxx_test.sh
+-rw-r--r--   0     1001      123      152 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/mnist/README.md
+-rw-r--r--   0     1001      123     5625 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/mnist/main.py
+-rw-r--r--   0     1001      123     5899 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/mnist/main_with_hp.py
+-rw-r--r--   0     1001      123     6202 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/mnist/main_with_hp_with_mlflow.py
+-rw-r--r--   0     1001      123       18 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/mnist/requirements.txt
+-rw-r--r--   0     1001      123     2846 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/optuna/README.md
+-rw-r--r--   0     1001      123      230 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/optuna/example.py
+-rw-r--r--   0     1001      123      527 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/optuna/example_hp.py
+-rw-r--r--   0     1001      123      727 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/optuna/example_hp_nested.py
+-rw-r--r--   0     1001      123     1650 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/sparse_lr/README.md
+-rw-r--r--   0     1001      123      581 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/sparse_lr/example_1.py
+-rw-r--r--   0     1001      123      934 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/sparse_lr/example_2.py
+-rw-r--r--   0     1001      123     1059 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/sparse_lr/example_mlflow.py
+-rw-r--r--   0     1001      123      867 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/sparse_lr/model.py
+-rw-r--r--   0     1001      123     1631 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/storage.rs
+-rw-r--r--   0     1001      123        0 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/hparam/__init__.py
+-rw-r--r--   0     1001      123     3710 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/hparam/__main__.py
+-rw-r--r--   0     1001      123      314 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/hyperparameter/__init__.py
+-rw-r--r--   0     1001      123    16064 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/hyperparameter/api.py
+-rw-r--r--   0     1001      123     7032 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/hyperparameter/hyperparameter.h
+-rw-r--r--   0     1001      123      828 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/hyperparameter/loader.py
+-rw-r--r--   0     1001      123     3854 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/hyperparameter/storage.py
+-rw-r--r--   0     1001      123     2223 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/hyperparameter/tune.py
+-rw-r--r--   0     1001      123     1249 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/mkdocs.yml
+-rw-r--r--   0     1001      123      938 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/pyproject.toml
+-rw-r--r--   0     1001      123     5802 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/src/entry.rs
+-rw-r--r--   0     1001      123     5132 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/src/ext.rs
+-rw-r--r--   0     1001      123     2038 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/src/ffi.rs
+-rw-r--r--   0     1001      123      106 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/src/lib.rs
+-rw-r--r--   0     1001      123     8872 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/src/storage.rs
+-rw-r--r--   0     1001      123     4528 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/src/xxh.rs
+-rwxr-xr-x   0     1001      123    40754 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/tests/a.out
+-rw-r--r--   0     1001      123     3769 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/tests/test_param_scope.py
+-rw-r--r--   0     1001      123      697 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/tests/test_param_scope_thread.py
+-rw-r--r--   0     1001      123     2988 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/tests/test_rust_backend.py
+-rw-r--r--   0        0        0     4210 1970-01-01 00:00:00.000000 hyperparameter-0.5.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `hyperparameter-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md` & `hyperparameter-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.4.3/.github/ISSUE_TEMPLATE/feature_request.md` & `hyperparameter-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.4.3/.github/workflows/codecov.yml` & `hyperparameter-0.5.0/.github/workflows/codecov.yml`

 * *Files 12% similar despite different names*

```diff
@@ -10,16 +10,18 @@
       run:
         working-directory: .
     steps:
     - uses: actions/checkout@v1
     - uses: actions/setup-python@v2
       with:
         python-version: '3.9'
+    - name: Install Rust toolchain
+      uses: dtolnay/rust-toolchain@stable
     - name: Install requirements
       run: |
-        pip install pytest pytest-cov
+        pip install pytest pytest-cov && pip install -e .
     - name: Run tests and collect coverage
       run: pytest --cov=./ --cov-report=xml
     - name: Upload coverage reports to Codecov with GitHub Action
       uses: codecov/codecov-action@v3
       with:
         token: ${{ secrets.CODECOV }}
```

### Comparing `hyperparameter-0.4.3/.github/workflows/mkdocs.yml` & `hyperparameter-0.5.0/.github/workflows/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.4.3/.github/workflows/python-publish.yml` & `hyperparameter-0.5.0/.github/workflows/python-publish.yml`

 * *Files 20% similar despite different names*

```diff
@@ -14,23 +14,27 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: '3.x'
+    - name: Install Rust toolchain
+      uses: dtolnay/rust-toolchain@stable
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install build
-    - name: Build package
-      run: python -m build
+        pip install build maturin
+    - uses: PyO3/maturin-action@v1
+      with:
+        command: build
+        args: --release --sdist -o dist
     - name: Publish package
       uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `hyperparameter-0.4.3/.gitignore` & `hyperparameter-0.5.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -128,7 +128,20 @@
 # Pyre type checker
 .pyre/
 examples/data/
 examples/mnist/mlruns/
 examples/sparse_lr/mlruns/
 .vscode/
 .DS_Store
+
+
+# Added by cargo
+
+/target
+
+
+# Added by cargo
+#
+# already existing elements were commented out
+
+#/target
+/Cargo.lock
```

### Comparing `hyperparameter-0.4.3/CODE_OF_CONDUCT.md` & `hyperparameter-0.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.4.3/LICENSE` & `hyperparameter-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.4.3/PKG-INFO` & `hyperparameter-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hyperparameter
-Version: 0.4.3
+Version: 0.5.0
+License-File: LICENSE
 Summary: A hyper-parameter library for researchers, data scientists and machine learning engineers.
 Author-email: Reiase <reiase@gmail.com>
 License: Apache License Version 2.0
 Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 **H**_yper_**P**_arameter_
 ===========================
 
 <h3 align="center">
   <p style="text-align: center;">
   <a href="README.md" target="_blank">ENGLISH</a> | <a href="README.zh.md">中文文档</a>
@@ -128,7 +128,8 @@
 ### [parameter tunning for researchers](examples/sparse_lr/README.md)
 
 This example shows how to use hyperparameter in your research projects, and make your experiments reproducible.
 
 ### [experiment tracing for data scientists](examples/mnist/README.md)
 
 This example shows experiment management with hyperparameter, and tracing the results with mlflow.tracing.
+
```

### Comparing `hyperparameter-0.4.3/README.md` & `hyperparameter-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.4.3/README.zh.md` & `hyperparameter-0.5.0/README.zh.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 <h3 align="center">
   <p style="text-align: center;">
   <a href="README.md" target="_blank">ENGLISH</a> | <a href="README.zh.md">中文文档</a>
   </p>
 </h3>
 
-HyperParameter 是轻量级python代码配置框架，用户仅需对代码添加标记即可实现配置化。特别适用于机器学习模型的参数管理，帮助开发者对接MLOps工具；也适用于大型Python应用的配置管理。
+HyperParameter 是轻量级python代码配置框架，用户仅需对代码添加标记即可实现配置化。特别适用于机器学习模型的参数管理，帮助开发者对接MLOps工具；也适用于大型Python应用的配置管理。=====
 
 ### 一个示例
 
 假设我们开发了一个MLP结构，并使用在某个模型中：
 
 ```python
 class MLP(nn.Module):
```

### Comparing `hyperparameter-0.4.3/docs/examples/optimization.md` & `hyperparameter-0.5.0/docs/examples/optimization.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.4.3/docs/examples/optimization.zh.md` & `hyperparameter-0.5.0/docs/examples/optimization.zh.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.4.3/docs/index.md` & `hyperparameter-0.5.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.4.3/docs/index.zh.md` & `hyperparameter-0.5.0/docs/index.zh.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 <h3 align="center">
   <p style="text-align: center;">
   <a href="README.md" target="_blank">ENGLISH</a> | <a href="README.zh.md">中文文档</a>
   </p>
 </h3>
 
-HyperParameter 是轻量级python代码配置框架，用户仅需对代码添加标记即可实现配置化。特别适用于机器学习模型的参数管理，帮助开发者对接MLOps工具；也适用于大型Python应用的配置管理。
+HyperParameter 是轻量级python代码配置框架，用户仅需对代码添加标记即可实现配置化。特别适用于机器学习模型的参数管理，帮助开发者对接MLOps工具；也适用于大型Python应用的配置管理。=====
 
 ### 一个示例
 
 假设我们开发了一个MLP结构，并使用在某个模型中：
 
 ```python
 class MLP(nn.Module):
```

### Comparing `hyperparameter-0.4.3/docs/quick_start.zh.md` & `hyperparameter-0.5.0/docs/quick_start.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 主要特性：
 
 1. `param_scope` 上下文，向 Python 应用提供线程安全的、可嵌套的参数管理上下文；提供对象化的树状参数管理，并支持默认值；
 
 ```python
 >>> from hyperparameter import param_scope
 >>> with param_scope(param1=1) as ps:
-...     print(f"param1={ps.param1}, param2={ps.param2('undefined')}")
+...     print(f"param1={ps.param1()}, param2={ps.param2('undefined')}")
 param1=1, param2=undefined
 
 ```
 
 2. `auto_param` 装饰器，自动将函数（或者 class）的默认参数转化为超参，并接受`param_scope`的参数控制；
 
 ```python
```

### Comparing `hyperparameter-0.4.3/docs/structured_parameter.md` & `hyperparameter-0.5.0/docs/structured_parameter.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.4.3/examples/application/app.py` & `hyperparameter-0.5.0/examples/application/app.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.4.3/examples/automl_optuna_mnist/automl_mnist.py` & `hyperparameter-0.5.0/examples/automl_optuna_mnist/automl_mnist.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.4.3/examples/mnist/main.py` & `hyperparameter-0.5.0/examples/mnist/main.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.4.3/examples/mnist/main_with_hp.py` & `hyperparameter-0.5.0/examples/mnist/main_with_hp.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.4.3/examples/mnist/main_with_hp_with_mlflow.py` & `hyperparameter-0.5.0/examples/mnist/main_with_hp_with_mlflow.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.4.3/examples/optuna/README.md` & `hyperparameter-0.5.0/examples/optuna/README.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.4.3/examples/optuna/example_hp.py` & `hyperparameter-0.5.0/examples/optuna/example_hp.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.4.3/examples/optuna/example_hp_nested.py` & `hyperparameter-0.5.0/examples/optuna/example_hp_nested.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.4.3/examples/sparse_lr/README.md` & `hyperparameter-0.5.0/examples/sparse_lr/README.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.4.3/examples/sparse_lr/example_1.py` & `hyperparameter-0.5.0/examples/sparse_lr/example_1.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.4.3/examples/sparse_lr/example_2.py` & `hyperparameter-0.5.0/examples/sparse_lr/example_2.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.4.3/examples/sparse_lr/example_mlflow.py` & `hyperparameter-0.5.0/examples/sparse_lr/example_mlflow.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.4.3/examples/sparse_lr/model.py` & `hyperparameter-0.5.0/examples/sparse_lr/model.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.4.3/hparam/__main__.py` & `hyperparameter-0.5.0/hparam/__main__.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.4.3/hyperparameter/loader.py` & `hyperparameter-0.5.0/hyperparameter/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,17 @@
     except Exception as e:
         warnings.warn(
             "package toml is required by hyperparameter, please install toml with `pip install toml`"
         )
         raise e
     return toml.loads(config)
 
+
 def dumps(config) -> str:
     try:
         import toml
     except Exception as e:
         warnings.warn(
             "package toml is required by hyperparameter, please install toml with `pip install toml`"
         )
         raise e
-    return toml.dumps(config)
+    return toml.dumps(config)
```

### Comparing `hyperparameter-0.4.3/hyperparameter/tune.py` & `hyperparameter-0.5.0/hyperparameter/tune.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     ...     def __init__(self, lst):
     ...         self._lst = lst
     ...         self._offset = 0
     ...     def __call__(self):
     ...         index, self._offset = self._offset % len(self._lst), self._offset + 1
     ...         return self._lst[index]
 
-    >>> from hyperparameter import param_scope, suggest_from
+    >>> from hyperparameter import param_scope
     >>> with param_scope(suggested = suggest_from(ValueWrapper([1,2,3]))) as ps:
     ...     ps().suggested()
     ...     ps().suggested()
     ...     ps().suggested()
     1
     2
     3
```

### Comparing `hyperparameter-0.4.3/mkdocs.yml` & `hyperparameter-0.5.0/mkdocs.yml`

 * *Files identical despite different names*


# Comparing `tmp/cliconfig-0.4.6.tar.gz` & `tmp/cliconfig-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliconfig-0.4.6.tar", last modified: Thu May 11 12:27:11 2023, max compression
+gzip compressed data, was "cliconfig-0.4.7.tar", last modified: Thu May 11 23:37:25 2023, max compression
```

## Comparing `cliconfig-0.4.6.tar` & `cliconfig-0.4.7.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:27:11.108993 cliconfig-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 12:26:50.000000 cliconfig-0.4.6/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:27:11.096992 cliconfig-0.4.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:27:11.100993 cliconfig-0.4.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-11 12:26:50.000000 cliconfig-0.4.6/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-11 12:26:50.000000 cliconfig-0.4.6/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-11 12:26:50.000000 cliconfig-0.4.6/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-11 12:26:50.000000 cliconfig-0.4.6/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-11 12:26:50.000000 cliconfig-0.4.6/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-11 12:26:50.000000 cliconfig-0.4.6/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-11 12:26:50.000000 cliconfig-0.4.6/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-11 12:26:50.000000 cliconfig-0.4.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-11 12:26:50.000000 cliconfig-0.4.6/.markdownlint.json
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-11 12:26:50.000000 cliconfig-0.4.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-11 12:26:50.000000 cliconfig-0.4.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-11 12:26:50.000000 cliconfig-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-05-11 12:27:11.108993 cliconfig-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-05-11 12:26:50.000000 cliconfig-0.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-05-11 12:26:50.000000 cliconfig-0.4.6/README_pypi.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:27:11.104993 cliconfig-0.4.6/cliconfig/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-11 12:26:50.000000 cliconfig-0.4.6/cliconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 12:27:10.000000 cliconfig-0.4.6/cliconfig/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-05-11 12:26:50.000000 cliconfig-0.4.6/cliconfig/build_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-11 12:26:50.000000 cliconfig-0.4.6/cliconfig/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    14687 2023-05-11 12:26:50.000000 cliconfig-0.4.6/cliconfig/dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-05-11 12:26:50.000000 cliconfig-0.4.6/cliconfig/process_routines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:27:11.104993 cliconfig-0.4.6/cliconfig/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-11 12:26:50.000000 cliconfig-0.4.6/cliconfig/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-11 12:26:50.000000 cliconfig-0.4.6/cliconfig/processing/_type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-11 12:26:50.000000 cliconfig-0.4.6/cliconfig/processing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16892 2023-05-11 12:26:50.000000 cliconfig-0.4.6/cliconfig/processing/builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-05-11 12:26:50.000000 cliconfig-0.4.6/cliconfig/processing/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-11 12:26:50.000000 cliconfig-0.4.6/cliconfig/tag_routines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:27:11.104993 cliconfig-0.4.6/cliconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-05-11 12:27:11.000000 cliconfig-0.4.6/cliconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-11 12:27:11.000000 cliconfig-0.4.6/cliconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 12:27:11.000000 cliconfig-0.4.6/cliconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 12:27:11.000000 cliconfig-0.4.6/cliconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 12:27:11.000000 cliconfig-0.4.6/cliconfig.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:27:11.104993 cliconfig-0.4.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-11 12:26:50.000000 cliconfig-0.4.6/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:27:11.104993 cliconfig-0.4.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-11 12:26:50.000000 cliconfig-0.4.6/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-11 12:26:50.000000 cliconfig-0.4.6/docs/_static/logo_extend.png
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-11 12:26:50.000000 cliconfig-0.4.6/docs/cliconfig.processing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-11 12:26:50.000000 cliconfig-0.4.6/docs/cliconfig_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-11 12:26:50.000000 cliconfig-0.4.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-11 12:26:50.000000 cliconfig-0.4.6/docs/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-11 12:26:50.000000 cliconfig-0.4.6/docs/edge_cases.md
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-11 12:26:50.000000 cliconfig-0.4.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-11 12:26:50.000000 cliconfig-0.4.6/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-11 12:26:50.000000 cliconfig-0.4.6/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-11 12:26:50.000000 cliconfig-0.4.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-05-11 12:26:50.000000 cliconfig-0.4.6/docs/processing.md
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-05-11 12:26:50.000000 cliconfig-0.4.6/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-11 12:26:50.000000 cliconfig-0.4.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:27:11.104993 cliconfig-0.4.6/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 12:26:50.000000 cliconfig-0.4.6/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-11 12:26:50.000000 cliconfig-0.4.6/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-11 12:26:50.000000 cliconfig-0.4.6/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-11 12:26:50.000000 cliconfig-0.4.6/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-11 12:26:50.000000 cliconfig-0.4.6/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:27:11.104993 cliconfig-0.4.6/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-11 12:26:50.000000 cliconfig-0.4.6/licenses_tier/FLATTEN_DICT_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-11 12:26:50.000000 cliconfig-0.4.6/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-11 12:26:50.000000 cliconfig-0.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-11 12:26:50.000000 cliconfig-0.4.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 12:26:50.000000 cliconfig-0.4.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 12:27:11.108993 cliconfig-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-11 12:26:50.000000 cliconfig-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:27:11.108993 cliconfig-0.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:27:11.108993 cliconfig-0.4.6/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/configs/config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/configs/config2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/configs/configtag1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/configs/configtag2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/configs/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/configs/default2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:27:11.108993 cliconfig-0.4.6/tests/configs/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/configs/integration/main.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/configs/integration/sub1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/configs/integration/sub2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:27:11.108993 cliconfig-0.4.6/tests/configs/merge/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/configs/merge/additional1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/configs/merge/additional2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/configs/merge/additional3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/configs/merge/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/configs/merge/default2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/configs/merge/default3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:27:11.108993 cliconfig-0.4.6/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/integration/test_inte_multiple_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:27:11.108993 cliconfig-0.4.6/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 12:27:11.108993 cliconfig-0.4.6/tests/unit/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/unit/processing/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/unit/processing/test_builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/unit/processing/test_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/unit/processing/test_type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/unit/test_build_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/unit/test_cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/unit/test_dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/unit/test_process_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-11 12:26:50.000000 cliconfig-0.4.6/tests/unit/test_tag_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:37:25.182442 cliconfig-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 23:37:05.000000 cliconfig-0.4.7/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:37:25.162442 cliconfig-0.4.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:37:25.170442 cliconfig-0.4.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-11 23:37:05.000000 cliconfig-0.4.7/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-11 23:37:05.000000 cliconfig-0.4.7/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-11 23:37:05.000000 cliconfig-0.4.7/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-11 23:37:05.000000 cliconfig-0.4.7/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-11 23:37:05.000000 cliconfig-0.4.7/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-11 23:37:05.000000 cliconfig-0.4.7/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-11 23:37:05.000000 cliconfig-0.4.7/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-11 23:37:05.000000 cliconfig-0.4.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-11 23:37:05.000000 cliconfig-0.4.7/.markdownlint.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-11 23:37:05.000000 cliconfig-0.4.7/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-11 23:37:05.000000 cliconfig-0.4.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-11 23:37:05.000000 cliconfig-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-05-11 23:37:25.182442 cliconfig-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-05-11 23:37:05.000000 cliconfig-0.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-05-11 23:37:05.000000 cliconfig-0.4.7/README_pypi.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:37:25.170442 cliconfig-0.4.7/cliconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-11 23:37:05.000000 cliconfig-0.4.7/cliconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 23:37:25.000000 cliconfig-0.4.7/cliconfig/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-05-11 23:37:05.000000 cliconfig-0.4.7/cliconfig/build_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-11 23:37:05.000000 cliconfig-0.4.7/cliconfig/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14687 2023-05-11 23:37:05.000000 cliconfig-0.4.7/cliconfig/dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-05-11 23:37:05.000000 cliconfig-0.4.7/cliconfig/process_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:37:25.174442 cliconfig-0.4.7/cliconfig/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-11 23:37:05.000000 cliconfig-0.4.7/cliconfig/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-11 23:37:05.000000 cliconfig-0.4.7/cliconfig/processing/_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-11 23:37:05.000000 cliconfig-0.4.7/cliconfig/processing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16892 2023-05-11 23:37:05.000000 cliconfig-0.4.7/cliconfig/processing/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-11 23:37:05.000000 cliconfig-0.4.7/cliconfig/processing/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-11 23:37:05.000000 cliconfig-0.4.7/cliconfig/tag_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:37:25.170442 cliconfig-0.4.7/cliconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-05-11 23:37:25.000000 cliconfig-0.4.7/cliconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-11 23:37:25.000000 cliconfig-0.4.7/cliconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 23:37:25.000000 cliconfig-0.4.7/cliconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 23:37:25.000000 cliconfig-0.4.7/cliconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 23:37:25.000000 cliconfig-0.4.7/cliconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:37:25.174442 cliconfig-0.4.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-11 23:37:05.000000 cliconfig-0.4.7/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:37:25.174442 cliconfig-0.4.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-11 23:37:05.000000 cliconfig-0.4.7/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-11 23:37:05.000000 cliconfig-0.4.7/docs/_static/logo_extend.png
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-11 23:37:05.000000 cliconfig-0.4.7/docs/cliconfig.processing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-11 23:37:05.000000 cliconfig-0.4.7/docs/cliconfig_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-11 23:37:05.000000 cliconfig-0.4.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-11 23:37:05.000000 cliconfig-0.4.7/docs/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-11 23:37:05.000000 cliconfig-0.4.7/docs/edge_cases.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-11 23:37:05.000000 cliconfig-0.4.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-11 23:37:05.000000 cliconfig-0.4.7/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-11 23:37:05.000000 cliconfig-0.4.7/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-11 23:37:05.000000 cliconfig-0.4.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-05-11 23:37:05.000000 cliconfig-0.4.7/docs/processing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-05-11 23:37:05.000000 cliconfig-0.4.7/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-11 23:37:05.000000 cliconfig-0.4.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:37:25.174442 cliconfig-0.4.7/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 23:37:05.000000 cliconfig-0.4.7/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-11 23:37:05.000000 cliconfig-0.4.7/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-11 23:37:05.000000 cliconfig-0.4.7/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-11 23:37:05.000000 cliconfig-0.4.7/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-11 23:37:05.000000 cliconfig-0.4.7/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:37:25.174442 cliconfig-0.4.7/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-11 23:37:05.000000 cliconfig-0.4.7/licenses_tier/FLATTEN_DICT_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-11 23:37:05.000000 cliconfig-0.4.7/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-11 23:37:05.000000 cliconfig-0.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-11 23:37:05.000000 cliconfig-0.4.7/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 23:37:05.000000 cliconfig-0.4.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 23:37:25.182442 cliconfig-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-11 23:37:05.000000 cliconfig-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:37:25.174442 cliconfig-0.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:37:25.178442 cliconfig-0.4.7/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/configs/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/configs/config2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/configs/configtag1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/configs/configtag2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/configs/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/configs/default2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:37:25.178442 cliconfig-0.4.7/tests/configs/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/configs/integration/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/configs/integration/sub1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/configs/integration/sub2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:37:25.178442 cliconfig-0.4.7/tests/configs/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/configs/merge/additional1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/configs/merge/additional2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/configs/merge/additional3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/configs/merge/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/configs/merge/default2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/configs/merge/default3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:37:25.178442 cliconfig-0.4.7/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/integration/test_inte_multiple_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:37:25.178442 cliconfig-0.4.7/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:37:25.178442 cliconfig-0.4.7/tests/unit/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/unit/processing/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/unit/processing/test_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/unit/processing/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/unit/processing/test_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/unit/test_build_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/unit/test_cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/unit/test_dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/unit/test_process_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-11 23:37:05.000000 cliconfig-0.4.7/tests/unit/test_tag_routines.py
```

### Comparing `cliconfig-0.4.6/.github/workflows/pipy_deployment.yaml` & `cliconfig-0.4.7/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/.github/workflows/pydocstyle.yaml` & `cliconfig-0.4.7/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/.github/workflows/pylint.yaml` & `cliconfig-0.4.7/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/.github/workflows/tests.yaml` & `cliconfig-0.4.7/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/.pylintrc` & `cliconfig-0.4.7/.pylintrc`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/CONTRIBUTING.md` & `cliconfig-0.4.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/LICENSE` & `cliconfig-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/PKG-INFO` & `cliconfig-0.4.7/README_pypi.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,21 @@
-Metadata-Version: 2.1
-Name: cliconfig
-Version: 0.4.6
-Summary: Merge your config files and set parameters from the command line in a simple way.
-Author-email: Valentin Goldite <valentin.goldite@gmail.com>
-Project-URL: Source, https://github.com/valentingol/cliconfig
-Keywords: logging,machine,learning
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CLI Config
 
 </p>
 <p align="center">
   <img src="https://raw.githubusercontent.com/valentingol/cliconfig/main/docs/_static/logo_extend.png" />
 </p>
 
 Lightweight library that provides routines to merge your configs (optionally nested)
-and set parameters from command line. It is also provide processing functions
-that can change the whole config before and after each config merge, before config
-saving and after config loading. It also contains many routines to manipulate
-the config as flatten or nested dicts.
+and set parameters from the command line. It also provides processing functions that
+can modify the entire config before and after each config merge, before config saving,
+and after config loading. Additionally, it contains many routines to manipulate the
+config, such as flattening or nesting dicts.
 
-## Documentation :memo: : [here](https://cliconfig.readthedocs.io/en/stable)
+## Documentation: [here](https://cliconfig.readthedocs.io/en/stable)
 
 [![Release](https://img.shields.io/github/v/tag/valentingol/cliconfig?label=Pypi&logo=pypi&logoColor=yellow)](https://pypi.org/project/cliconfig/)
 ![PythonVersion](https://img.shields.io/badge/Python-3.7%20%7E%203.11-informational)
 [![License](https://img.shields.io/github/license/valentingol/cliconfig?color=999)](https://stringfixer.com/fr/MIT_license)
 
 [![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -50,16 +38,16 @@
 pip install cliconfig
 ```
 
 This package is OS independent and supported on Linux, macOS and Windows.
 
 ## Quick start
 
-First create a default config that can be split in multiple files that will be merged
-(from left to right in `make_config` function). There is no limit of depth for the
+Create a default configuration that can be split across multiple files that will
+be merged in sequence. There is no depth limit for the
 configuration parameters.
 
 ```yaml
 ---  # default1.yaml
 param1: 1
 param2: 0
 letters:
@@ -68,145 +56,154 @@
 
 ---  # default2.yaml
 param1: 1
 param2: 2  # will override param2 from default1.yaml
 letters.letter3: c  # add a new parameter
 ```
 
-Now you can set up your program to use the config:
+Now you can write these following lines in your python program to use this config
+with `make_config`:
 
 ```python
 # main.py
-from cliconfig import make_config, show_config
+from cliconfig import make_config, show_dict
 
 config, _ = make_config('default1.yaml', 'default2.yaml')
-show_config(config)  # print the config to check it
+show_dict(config)  # print the config to check it
 ```
 
-Then add one or multiple additional config files that will be passed on command line
-and that will override the default values.
+Then you can add one or multiple additional config files that will be passed on
+command line and that will override the default values.
 
 ```yaml
 ---  # first.yaml
 letters:
   letter3: C
 
 ---  # second.yaml
 param1: -1
 letters.letter1: A
 ```
 
-**Be careful, the additional config files cannot add new parameters that are
-not in default configs**. It is intended to prevent typos in the config files
-that would not be detected. It also improves the readability of the config
-files and the retro-compatibility.
-
-Now you can launch the program with additional configurations and parameters.
-The additional configs will be merged to the default configs, then the parameters
-will be merged.
+**Please note that the additional config files must not introduce new parameters that
+are not in the default configs, as it will result in an error**. This
+restriction is in place to prevent potential typos in the config files from
+going unnoticed. It also enhances the readability of the default config files
+and ensures retro-compatibility.
+
+Now you can launch the program with additional configurations and also set
+individual parameters. The additional configs will be merged to the default
+configs, then the parameters will be merged.
 
 For example:
 
 ```bash
 python main.py --config first.yaml,second.yaml --param2=-2 --letters.letter2='B'
 ```
 
 *Note*: the additional configs are detected with `--config` followed by space
-and separated by a comma **without space**. It also possible to pass a list.
+and separated by comma(s) **without space**. It also possible to pass a list.
 The parameters are detected with the pattern `--<param>=<value>` without spaces.
 
-Will show:
+It will show:
 
 ```text
 [CONFIG] Merge 2 default configs, 2 additional configs and 2 CLI parameter(s).
 
 Config:
     param1: -1
     param2: -2
     letters:
         letter1: A
         letter2: B
         letter3: C
 ```
 
-Note that the configurations are native python dicts at each step of the process.
+Note that the configurations is a native python dict at each step of the process.
 
 ## Use tags
 
-By default, the package provides some "tags" that are strings starting with `@`
-and placed at the end of a key containing a parameter. It will change the way
-the configuration is processed.
-
-The default tags are:
-
-* `@merge_add`, `@merge_before` and `@merge_after` to merge the dict loaded
-  from the value (should be a yaml path!) to the current configuration.
-  `@merge_add` allow only new keys and is useful to split sub-configurations
-  in multiple files. `@merge_before` will merge the current dict on the loaded
-  one and `@merge_after` will merge the loaded dict on the current one. With
-  theses tags, you can dynamically merge configurations depending on the paths
-  you set as values.
-* `@copy` Copy a parameter from another key. The value should be a string containing
-  this flatten key
-* `@type:<my type>` To check if the key is of the type `<my type>` at each update
-  even if the tag is no longer present. It supports basic type (except tuple and
-  sets that are not handled by yaml) as well as union (with "Union" or "|"), optional,
-  lists and dicts.
+By default, the package provides some "tags" represented as strings that start with
+'@' and are placed at the end of a key containing a parameter. These tags change
+the way the configuration is processed.
+
+The default tags include:
+
+* `@merge_add`, `@merge_before`, and `@merge_after`: These tags merge the dictionary
+  loaded from the specified value (which should be a YAML path) into the current
+  configuration. `@merge_add` allows only the merging of new keys and is useful for
+  splitting different sub-configurations into multiple files. `@merge_before` merges
+  the current dictionary onto the loaded one, while `@merge_after` merges the loaded
+  dictionary onto the current one. These tags enable dynamic configuration merging
+  on the command line, depending on the specified paths. Note that when multiple
+  `@merge_before` or `@merge_after` tags merge the *same key*, the order of merging
+  is not guaranteed as it depends on the order of the tags in the configuration file.
+* `@copy`: This tag copies a parameter from another key. The value should be a string
+  that represents the flattened key. The copied value is then protected from further
+  updates but will be updated if the copied key change during a merge.
+* `@type:<my type>`: This tag checks if the key matches the specified type `<my type>`
+   after each update, even if the tag is no longer present. It supports basic types
+   (except for tuples and sets, which are not handled by YAML) as well as unions
+   (using "Union" or "|"), optional values, lists, and dictionaries.
 
-The tags are applied in this order: `@merge`, `@copy` then `@type`.
+The tags are applied in the following order: `@merge`, `@copy`, and then `@type`.
 
-Note that the tags are only used to trigger internal processing and will be
-automatically removed from the key after the processing.
+Please note that the tags serve as triggers for internal processing and will be
+automatically removed from the key after processing.
 
-You can also combine the tags, example:
+It is also possible to combine multiple tags. For example:
 
 ```yaml
 ---  # main.yaml
 path_1@merge_add: sub1.yaml
 path_2@merge_add: sub2.yaml
 --- # sub1.yaml
 config1:
-  param@copy@type:int: config1.param2
+  param@copy@type:int: config2.param2
   param2@type:int: 1
 --- # sub2.yaml
 config2.param@type:None|int: 2
 ```
 
 Here `main.yaml` is interpreted like:
 
 ```yaml
 path_1: sub1.yaml
 path_2: sub2.yaml
 config1:
-    param: 1
+    param: 2  # the value of config2.param2
     param2: 1
 config2:
     param: 2
 ```
 
-and now, all the parameters have a forced type.
+Now, all the parameters have a forced type and `config1.param2` will be
+update if `config2.param2` is updated during a merge. These side effects are not
+visible in the config but stored on processing classes. They are objects that
+catch the tags, remove them from config and apply a modification on the config.
+These processing are powerful tools that can be used to highly customize the
+configuration process.
 
-The point is that you can easily create your own processing associated to your
-own tags. They provide a large number of possibilities to customize the
-configuration process and are describe in the
+You can easily create your own processing (associated to a tag or not).
+The way to do it and a further explanation of them is available in the
 [*Processing*](https://cliconfig.readthedocs.io/en/latest/processing.html) section
 of the documentation.
 
 ## Edge cases
 
-**Be careful, tuples and sets are not supported by YAML and cannot be used in
-yaml files.**
-Use lists instead if possible.
-
-`None` is not recognized as a None object by YAML but as a string, you may use `null`
-or `Null` instead if you want to set a None object.
-
-Dicts are considered as sub-configs and so you may not be able to change
-the keys in the additional configs. If you want to modify or add dict keys, you should
-enclose it in a list.
+**Please note that YAML does not support tuples and sets**, and therefore they
+cannot be used in YAML files. If possible, consider using lists instead.
+
+Moreover, YAML does not recognize "None" as a None object, but interprets it as a
+string. If you wish to set a None object, you can use "null" or "Null" instead.
+
+In the context of this package, dictionaries are treated as sub-configurations,
+which means that modifying or adding keys directly in the additional configs may
+not be possible (because only the merge of default configuration allow adding new keys).
+If you need to modify or add keys within a dictionary, consider enclosing it in a list.
 
 For instance:
 
 ```yaml
 --- default.yaml
 logging:
   metrics: ['train loss', 'val loss']
```

### Comparing `cliconfig-0.4.6/README.md` & `cliconfig-0.4.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # CLI Config
 
 <p align="center">
   <img src="docs/_static/logo_extend.png" />
 </p>
 
 Lightweight library that provides routines to merge your configs (optionally nested)
-and set parameters from command line. It is also provide processing functions
-that can change the whole config before and after each config merge, before config
-saving and after config loading. It also contains many routines to manipulate
-the config as flatten or nested dicts.
+and set parameters from the command line. It also provides processing functions that
+can modify the entire config before and after each config merge, before config saving,
+and after config loading. Additionally, it contains many routines to manipulate the
+config, such as flattening or nesting dicts.
 
 ## Documentation :memo: [here](https://cliconfig.readthedocs.io/en/stable)
 
 [![Release](https://img.shields.io/github/v/tag/valentingol/cliconfig?label=Pypi&logo=pypi&logoColor=yellow)](https://pypi.org/project/cliconfig/)
 ![PythonVersion](https://img.shields.io/badge/Python-3.7%20%7E%203.11-informational)
 [![License](https://img.shields.io/github/license/valentingol/cliconfig?color=999)](https://stringfixer.com/fr/MIT_license)
 
@@ -37,17 +37,16 @@
 pip install cliconfig
 ```
 
 This package is OS independent and supported on Linux, macOS and Windows.
 
 ## Quick start
 
-First create a default config that can be split in multiple files that will be merged
-(from left to right in `make_config` function). There is no limit of depth for the
-configuration parameters.
+Create a default configuration that can be split across multiple files that will
+be merged in sequence. There is no depth limit for the configuration parameters.
 
 ```yaml
 ---  # default1.yaml
 param1: 1
 param2: 0
 letters:
   letter1: a
@@ -55,145 +54,154 @@
 
 ---  # default2.yaml
 param1: 1
 param2: 2  # will override param2 from default1.yaml
 letters.letter3: c  # add a new parameter
 ```
 
-Now you can set up your program to use the config:
+Now you can write these following lines in your python program to use this config
+with `make_config`:
 
 ```python
 # main.py
-from cliconfig import make_config, show_config
+from cliconfig import make_config, show_dict
 
 config, _ = make_config('default1.yaml', 'default2.yaml')
-show_config(config)  # print the config to check it
+show_dict(config)  # print the config to check it
 ```
 
-Then add one or multiple additional config files that will be passed on command line
-and that will override the default values.
+Then you can add one or multiple additional config files that will be passed on
+command line and that will override the default values.
 
 ```yaml
 ---  # first.yaml
 letters:
   letter3: C
 
 ---  # second.yaml
 param1: -1
 letters.letter1: A
 ```
 
-**Be careful, the additional config files cannot add new parameters that are
-not in default configs**. It is intended to prevent typos in the config files
-that would not be detected. It also improves the readability of the config
-files and the retro-compatibility.
-
-Now you can launch the program with additional configurations and parameters.
-The additional configs will be merged to the default configs, then the parameters
-will be merged.
+**Please note that the additional config files must not introduce new parameters that
+are not in the default configs, as it will result in an error**. This
+restriction is in place to prevent potential typos in the config files from
+going unnoticed. It also enhances the readability of the default config files
+and ensures retro-compatibility.
+
+Now you can launch the program with additional configurations and also set
+individual parameters. The additional configs will be merged to the default
+configs, then the parameters will be merged.
 
 For example:
 
 ```bash
 python main.py --config first.yaml,second.yaml --param2=-2 --letters.letter2='B'
 ```
 
 *Note*: the additional configs are detected with `--config` followed by space
-and separated by a comma **without space**. It also possible to pass a list.
+and separated by comma(s) **without space**. It also possible to pass a list.
 The parameters are detected with the pattern `--<param>=<value>` without spaces.
 
-Will show:
+It will show:
 
 ```text
 [CONFIG] Merge 2 default configs, 2 additional configs and 2 CLI parameter(s).
 
 Config:
     param1: -1
     param2: -2
     letters:
         letter1: A
         letter2: B
         letter3: C
 ```
 
-Note that the configurations are native python dicts at each step of the process.
+Note that the configurations is a native python dict at each step of the process.
 
 ## Use tags
 
-By default, the package provides some "tags" that are strings starting with `@`
-and placed at the end of a key containing a parameter. It will change the way
-the configuration is processed.
-
-The default tags are:
-
-* `@merge_add`, `@merge_before` and `@merge_after` to merge the dict loaded
-  from the value (should be a yaml path!) to the current configuration.
-  `@merge_add` allow only new keys and is useful to split sub-configurations
-  in multiple files. `@merge_before` will merge the current dict on the loaded
-  one and `@merge_after` will merge the loaded dict on the current one. With
-  theses tags, you can dynamically merge configurations depending on the paths
-  you set as values.
-* `@copy` Copy a parameter from another key. The value should be a string containing
-  this flatten key
-* `@type:<my type>` To check if the key is of the type `<my type>` at each update
-  even if the tag is no longer present. It supports basic type (except tuple and
-  sets that are not handled by yaml) as well as union (with "Union" or "|"), optional,
-  lists and dicts.
+By default, the package provides some "tags" represented as strings that start with
+'@' and are placed at the end of a key containing a parameter. These tags change
+the way the configuration is processed.
+
+The default tags include:
+
+* `@merge_add`, `@merge_before`, and `@merge_after`: These tags merge the dictionary
+  loaded from the specified value (which should be a YAML path) into the current
+  configuration. `@merge_add` allows only the merging of new keys and is useful for
+  splitting different sub-configurations into multiple files. `@merge_before` merges
+  the current dictionary onto the loaded one, while `@merge_after` merges the loaded
+  dictionary onto the current one. These tags enable dynamic configuration merging
+  on the command line, depending on the specified paths. Note that when multiple
+  `@merge_before` or `@merge_after` tags merge the *same key*, the order of merging
+  is not guaranteed as it depends on the order of the tags in the configuration file.
+* `@copy`: This tag copies a parameter from another key. The value should be a string
+  that represents the flattened key. The copied value is then protected from further
+  updates but will be updated if the copied key change during a merge.
+* `@type:<my type>`: This tag checks if the key matches the specified type `<my type>`
+   after each update, even if the tag is no longer present. It supports basic types
+   (except for tuples and sets, which are not handled by YAML) as well as unions
+   (using "Union" or "|"), optional values, lists, and dictionaries.
 
-The tags are applied in this order: `@merge`, `@copy` then `@type`.
+The tags are applied in the following order: `@merge`, `@copy`, and then `@type`.
 
-Note that the tags are only used to trigger internal processing and will be
-automatically removed from the key after the processing.
+Please note that the tags serve as triggers for internal processing and will be
+automatically removed from the key after processing.
 
-You can also combine the tags, example:
+It is also possible to combine multiple tags. For example:
 
 ```yaml
 ---  # main.yaml
 path_1@merge_add: sub1.yaml
 path_2@merge_add: sub2.yaml
 --- # sub1.yaml
 config1:
-  param@copy@type:int: config1.param2
+  param@copy@type:int: config2.param2
   param2@type:int: 1
 --- # sub2.yaml
 config2.param@type:None|int: 2
 ```
 
-Here `main.yaml` is interpreted like:
+Here `main.yaml` will be interpreted like:
 
 ```yaml
 path_1: sub1.yaml
 path_2: sub2.yaml
 config1:
-    param: 1
+    param: 2  # the value of config2.param2
     param2: 1
 config2:
     param: 2
 ```
 
-and now, all the parameters have a forced type.
+Now, all the parameters have a forced type and `config1.param2` will be
+update if `config2.param2` is updated during a merge. These side effects are not
+visible in the config but stored on processing classes. They are objects that
+catch the tags, remove them from config and apply a modification on the config.
+These processing are powerful tools that can be used to highly customize the
+configuration process.
 
-The point is that you can easily create your own processing associated to your
-own tags. They provide a large number of possibilities to customize the
-configuration process and are describe in the
+You can easily create your own processing (associated to a tag or not).
+The way to do it and a further explanation of them is available in the
 [*Processing*](https://cliconfig.readthedocs.io/en/latest/processing.html) section
 of the documentation.
 
 ## Edge cases
 
-**Be careful, tuples and sets are not supported by YAML and cannot be used in
-yaml files.**
-Use lists instead if possible.
-
-`None` is not recognized as a None object by YAML but as a string, you may use `null`
-or `Null` instead if you want to set a None object.
-
-Dicts are considered as sub-configs and so you may not be able to change
-the keys in the additional configs. If you want to modify or add dict keys, you should
-enclose it in a list.
+**Please note that YAML does not support tuples and sets**, and therefore they
+cannot be used in YAML files. If possible, consider using lists instead.
+
+Moreover, YAML does not recognize "None" as a None object, but interprets it as a
+string. If you wish to set a None object, you can use "null" or "Null" instead.
+
+In the context of this package, dictionaries are treated as sub-configurations,
+which means that modifying or adding keys directly in the additional configs may
+not be possible (because only the merge of default configuration allow adding new keys).
+If you need to modify or add keys within a dictionary, consider enclosing it in a list.
 
 For instance:
 
 ```yaml
 --- default.yaml
 logging:
   metrics: ['train loss', 'val loss']
```

### Comparing `cliconfig-0.4.6/README_pypi.md` & `cliconfig-0.4.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,33 @@
+Metadata-Version: 2.1
+Name: cliconfig
+Version: 0.4.7
+Summary: Merge your config files and set parameters from the command line in a simple way.
+Author-email: Valentin Goldite <valentin.goldite@gmail.com>
+Project-URL: Source, https://github.com/valentingol/cliconfig
+Keywords: logging,machine,learning
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # CLI Config
 
 </p>
 <p align="center">
   <img src="https://raw.githubusercontent.com/valentingol/cliconfig/main/docs/_static/logo_extend.png" />
 </p>
 
 Lightweight library that provides routines to merge your configs (optionally nested)
-and set parameters from command line. It is also provide processing functions
-that can change the whole config before and after each config merge, before config
-saving and after config loading. It also contains many routines to manipulate
-the config as flatten or nested dicts.
+and set parameters from the command line. It also provides processing functions that
+can modify the entire config before and after each config merge, before config saving,
+and after config loading. Additionally, it contains many routines to manipulate the
+config, such as flattening or nesting dicts.
 
-## Documentation :memo: : [here](https://cliconfig.readthedocs.io/en/stable)
+## Documentation: [here](https://cliconfig.readthedocs.io/en/stable)
 
 [![Release](https://img.shields.io/github/v/tag/valentingol/cliconfig?label=Pypi&logo=pypi&logoColor=yellow)](https://pypi.org/project/cliconfig/)
 ![PythonVersion](https://img.shields.io/badge/Python-3.7%20%7E%203.11-informational)
 [![License](https://img.shields.io/github/license/valentingol/cliconfig?color=999)](https://stringfixer.com/fr/MIT_license)
 
 [![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -38,16 +50,16 @@
 pip install cliconfig
 ```
 
 This package is OS independent and supported on Linux, macOS and Windows.
 
 ## Quick start
 
-First create a default config that can be split in multiple files that will be merged
-(from left to right in `make_config` function). There is no limit of depth for the
+Create a default configuration that can be split across multiple files that will
+be merged in sequence. There is no depth limit for the
 configuration parameters.
 
 ```yaml
 ---  # default1.yaml
 param1: 1
 param2: 0
 letters:
@@ -56,145 +68,154 @@
 
 ---  # default2.yaml
 param1: 1
 param2: 2  # will override param2 from default1.yaml
 letters.letter3: c  # add a new parameter
 ```
 
-Now you can set up your program to use the config:
+Now you can write these following lines in your python program to use this config
+with `make_config`:
 
 ```python
 # main.py
-from cliconfig import make_config, show_config
+from cliconfig import make_config, show_dict
 
 config, _ = make_config('default1.yaml', 'default2.yaml')
-show_config(config)  # print the config to check it
+show_dict(config)  # print the config to check it
 ```
 
-Then add one or multiple additional config files that will be passed on command line
-and that will override the default values.
+Then you can add one or multiple additional config files that will be passed on
+command line and that will override the default values.
 
 ```yaml
 ---  # first.yaml
 letters:
   letter3: C
 
 ---  # second.yaml
 param1: -1
 letters.letter1: A
 ```
 
-**Be careful, the additional config files cannot add new parameters that are
-not in default configs**. It is intended to prevent typos in the config files
-that would not be detected. It also improves the readability of the config
-files and the retro-compatibility.
-
-Now you can launch the program with additional configurations and parameters.
-The additional configs will be merged to the default configs, then the parameters
-will be merged.
+**Please note that the additional config files must not introduce new parameters that
+are not in the default configs, as it will result in an error**. This
+restriction is in place to prevent potential typos in the config files from
+going unnoticed. It also enhances the readability of the default config files
+and ensures retro-compatibility.
+
+Now you can launch the program with additional configurations and also set
+individual parameters. The additional configs will be merged to the default
+configs, then the parameters will be merged.
 
 For example:
 
 ```bash
 python main.py --config first.yaml,second.yaml --param2=-2 --letters.letter2='B'
 ```
 
 *Note*: the additional configs are detected with `--config` followed by space
-and separated by a comma **without space**. It also possible to pass a list.
+and separated by comma(s) **without space**. It also possible to pass a list.
 The parameters are detected with the pattern `--<param>=<value>` without spaces.
 
-Will show:
+It will show:
 
 ```text
 [CONFIG] Merge 2 default configs, 2 additional configs and 2 CLI parameter(s).
 
 Config:
     param1: -1
     param2: -2
     letters:
         letter1: A
         letter2: B
         letter3: C
 ```
 
-Note that the configurations are native python dicts at each step of the process.
+Note that the configurations is a native python dict at each step of the process.
 
 ## Use tags
 
-By default, the package provides some "tags" that are strings starting with `@`
-and placed at the end of a key containing a parameter. It will change the way
-the configuration is processed.
-
-The default tags are:
-
-* `@merge_add`, `@merge_before` and `@merge_after` to merge the dict loaded
-  from the value (should be a yaml path!) to the current configuration.
-  `@merge_add` allow only new keys and is useful to split sub-configurations
-  in multiple files. `@merge_before` will merge the current dict on the loaded
-  one and `@merge_after` will merge the loaded dict on the current one. With
-  theses tags, you can dynamically merge configurations depending on the paths
-  you set as values.
-* `@copy` Copy a parameter from another key. The value should be a string containing
-  this flatten key
-* `@type:<my type>` To check if the key is of the type `<my type>` at each update
-  even if the tag is no longer present. It supports basic type (except tuple and
-  sets that are not handled by yaml) as well as union (with "Union" or "|"), optional,
-  lists and dicts.
+By default, the package provides some "tags" represented as strings that start with
+'@' and are placed at the end of a key containing a parameter. These tags change
+the way the configuration is processed.
+
+The default tags include:
+
+* `@merge_add`, `@merge_before`, and `@merge_after`: These tags merge the dictionary
+  loaded from the specified value (which should be a YAML path) into the current
+  configuration. `@merge_add` allows only the merging of new keys and is useful for
+  splitting different sub-configurations into multiple files. `@merge_before` merges
+  the current dictionary onto the loaded one, while `@merge_after` merges the loaded
+  dictionary onto the current one. These tags enable dynamic configuration merging
+  on the command line, depending on the specified paths. Note that when multiple
+  `@merge_before` or `@merge_after` tags merge the *same key*, the order of merging
+  is not guaranteed as it depends on the order of the tags in the configuration file.
+* `@copy`: This tag copies a parameter from another key. The value should be a string
+  that represents the flattened key. The copied value is then protected from further
+  updates but will be updated if the copied key change during a merge.
+* `@type:<my type>`: This tag checks if the key matches the specified type `<my type>`
+   after each update, even if the tag is no longer present. It supports basic types
+   (except for tuples and sets, which are not handled by YAML) as well as unions
+   (using "Union" or "|"), optional values, lists, and dictionaries.
 
-The tags are applied in this order: `@merge`, `@copy` then `@type`.
+The tags are applied in the following order: `@merge`, `@copy`, and then `@type`.
 
-Note that the tags are only used to trigger internal processing and will be
-automatically removed from the key after the processing.
+Please note that the tags serve as triggers for internal processing and will be
+automatically removed from the key after processing.
 
-You can also combine the tags, example:
+It is also possible to combine multiple tags. For example:
 
 ```yaml
 ---  # main.yaml
 path_1@merge_add: sub1.yaml
 path_2@merge_add: sub2.yaml
 --- # sub1.yaml
 config1:
-  param@copy@type:int: config1.param2
+  param@copy@type:int: config2.param2
   param2@type:int: 1
 --- # sub2.yaml
 config2.param@type:None|int: 2
 ```
 
 Here `main.yaml` is interpreted like:
 
 ```yaml
 path_1: sub1.yaml
 path_2: sub2.yaml
 config1:
-    param: 1
+    param: 2  # the value of config2.param2
     param2: 1
 config2:
     param: 2
 ```
 
-and now, all the parameters have a forced type.
+Now, all the parameters have a forced type and `config1.param2` will be
+update if `config2.param2` is updated during a merge. These side effects are not
+visible in the config but stored on processing classes. They are objects that
+catch the tags, remove them from config and apply a modification on the config.
+These processing are powerful tools that can be used to highly customize the
+configuration process.
 
-The point is that you can easily create your own processing associated to your
-own tags. They provide a large number of possibilities to customize the
-configuration process and are describe in the
+You can easily create your own processing (associated to a tag or not).
+The way to do it and a further explanation of them is available in the
 [*Processing*](https://cliconfig.readthedocs.io/en/latest/processing.html) section
 of the documentation.
 
 ## Edge cases
 
-**Be careful, tuples and sets are not supported by YAML and cannot be used in
-yaml files.**
-Use lists instead if possible.
-
-`None` is not recognized as a None object by YAML but as a string, you may use `null`
-or `Null` instead if you want to set a None object.
-
-Dicts are considered as sub-configs and so you may not be able to change
-the keys in the additional configs. If you want to modify or add dict keys, you should
-enclose it in a list.
+**Please note that YAML does not support tuples and sets**, and therefore they
+cannot be used in YAML files. If possible, consider using lists instead.
+
+Moreover, YAML does not recognize "None" as a None object, but interprets it as a
+string. If you wish to set a None object, you can use "null" or "Null" instead.
+
+In the context of this package, dictionaries are treated as sub-configurations,
+which means that modifying or adding keys directly in the additional configs may
+not be possible (because only the merge of default configuration allow adding new keys).
+If you need to modify or add keys within a dictionary, consider enclosing it in a list.
 
 For instance:
 
 ```yaml
 --- default.yaml
 logging:
   metrics: ['train loss', 'val loss']
```

### Comparing `cliconfig-0.4.6/cliconfig/__init__.py` & `cliconfig-0.4.7/cliconfig/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     This project is free to use for COMMERCIAL USE, MODIFICATION,
     DISTRIBUTION and PRIVATE USE as long as the original license is
     include as well as this copy right notice.
 """
 from cliconfig._version import __version__, __version_tuple__
 from cliconfig.build_config import load_config, make_config
 from cliconfig.cli_parser import parse_cli
+from cliconfig.dict_routines import show_dict
 from cliconfig.process_routines import (
     merge_flat_paths_processing,
     merge_flat_processing,
     save_processing,
 )
 from cliconfig.processing.create import create_processing_value
 
@@ -26,9 +27,10 @@
     "__version_tuple__",
     "make_config",
     "parse_cli",
     "load_config",
     "merge_flat_paths_processing",
     "merge_flat_processing",
     "save_processing",
+    "show_dict",
     "create_processing_value",
 ]
```

### Comparing `cliconfig-0.4.6/cliconfig/build_config.py` & `cliconfig-0.4.7/cliconfig/build_config.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/cliconfig/cli_parser.py` & `cliconfig-0.4.7/cliconfig/cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/cliconfig/dict_routines.py` & `cliconfig-0.4.7/cliconfig/dict_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/cliconfig/process_routines.py` & `cliconfig-0.4.7/cliconfig/process_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/cliconfig/processing/_type_parser.py` & `cliconfig-0.4.7/cliconfig/processing/_type_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/cliconfig/processing/base.py` & `cliconfig-0.4.7/cliconfig/processing/base.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/cliconfig/processing/builtin.py` & `cliconfig-0.4.7/cliconfig/processing/builtin.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/cliconfig/processing/create.py` & `cliconfig-0.4.7/cliconfig/processing/create.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                 if self.tag_name:
                     del flat_dict[flat_key]
                     flat_key = clean_tag(flat_key, self.tag_name)
                 flat_dict[flat_key] = self.func(value)
         return flat_dict
 
 
-class ProcessingValuePersistent(Processing):
+class _ProcessingValuePersistent(Processing):
     """Processing class for make_processing_value. Persistent version."""
 
     def __init__(
         self,
         regex: str,
         tag_name: Optional[str],
         order: float,
@@ -146,9 +146,9 @@
             raise ValueError("You must provide a tag or a regex but not both.")
         regex = f'.*@{tag_name}.*'
     else:
         if regex is None:
             raise ValueError("You must provide a tag or a regex "
                              "(to trigger the value update).")
     if persistent:
-        return ProcessingValuePersistent(regex, tag_name, order, func)
+        return _ProcessingValuePersistent(regex, tag_name, order, func)
     return _ProcessingValue(regex, tag_name, order, func)
```

### Comparing `cliconfig-0.4.6/cliconfig/tag_routines.py` & `cliconfig-0.4.7/cliconfig/tag_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/cliconfig.egg-info/PKG-INFO` & `cliconfig-0.4.7/cliconfig.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 0.4.6
+Version: 0.4.7
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -14,20 +14,20 @@
 
 </p>
 <p align="center">
   <img src="https://raw.githubusercontent.com/valentingol/cliconfig/main/docs/_static/logo_extend.png" />
 </p>
 
 Lightweight library that provides routines to merge your configs (optionally nested)
-and set parameters from command line. It is also provide processing functions
-that can change the whole config before and after each config merge, before config
-saving and after config loading. It also contains many routines to manipulate
-the config as flatten or nested dicts.
+and set parameters from the command line. It also provides processing functions that
+can modify the entire config before and after each config merge, before config saving,
+and after config loading. Additionally, it contains many routines to manipulate the
+config, such as flattening or nesting dicts.
 
-## Documentation :memo: : [here](https://cliconfig.readthedocs.io/en/stable)
+## Documentation: [here](https://cliconfig.readthedocs.io/en/stable)
 
 [![Release](https://img.shields.io/github/v/tag/valentingol/cliconfig?label=Pypi&logo=pypi&logoColor=yellow)](https://pypi.org/project/cliconfig/)
 ![PythonVersion](https://img.shields.io/badge/Python-3.7%20%7E%203.11-informational)
 [![License](https://img.shields.io/github/license/valentingol/cliconfig?color=999)](https://stringfixer.com/fr/MIT_license)
 
 [![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
@@ -50,16 +50,16 @@
 pip install cliconfig
 ```
 
 This package is OS independent and supported on Linux, macOS and Windows.
 
 ## Quick start
 
-First create a default config that can be split in multiple files that will be merged
-(from left to right in `make_config` function). There is no limit of depth for the
+Create a default configuration that can be split across multiple files that will
+be merged in sequence. There is no depth limit for the
 configuration parameters.
 
 ```yaml
 ---  # default1.yaml
 param1: 1
 param2: 0
 letters:
@@ -68,145 +68,154 @@
 
 ---  # default2.yaml
 param1: 1
 param2: 2  # will override param2 from default1.yaml
 letters.letter3: c  # add a new parameter
 ```
 
-Now you can set up your program to use the config:
+Now you can write these following lines in your python program to use this config
+with `make_config`:
 
 ```python
 # main.py
-from cliconfig import make_config, show_config
+from cliconfig import make_config, show_dict
 
 config, _ = make_config('default1.yaml', 'default2.yaml')
-show_config(config)  # print the config to check it
+show_dict(config)  # print the config to check it
 ```
 
-Then add one or multiple additional config files that will be passed on command line
-and that will override the default values.
+Then you can add one or multiple additional config files that will be passed on
+command line and that will override the default values.
 
 ```yaml
 ---  # first.yaml
 letters:
   letter3: C
 
 ---  # second.yaml
 param1: -1
 letters.letter1: A
 ```
 
-**Be careful, the additional config files cannot add new parameters that are
-not in default configs**. It is intended to prevent typos in the config files
-that would not be detected. It also improves the readability of the config
-files and the retro-compatibility.
-
-Now you can launch the program with additional configurations and parameters.
-The additional configs will be merged to the default configs, then the parameters
-will be merged.
+**Please note that the additional config files must not introduce new parameters that
+are not in the default configs, as it will result in an error**. This
+restriction is in place to prevent potential typos in the config files from
+going unnoticed. It also enhances the readability of the default config files
+and ensures retro-compatibility.
+
+Now you can launch the program with additional configurations and also set
+individual parameters. The additional configs will be merged to the default
+configs, then the parameters will be merged.
 
 For example:
 
 ```bash
 python main.py --config first.yaml,second.yaml --param2=-2 --letters.letter2='B'
 ```
 
 *Note*: the additional configs are detected with `--config` followed by space
-and separated by a comma **without space**. It also possible to pass a list.
+and separated by comma(s) **without space**. It also possible to pass a list.
 The parameters are detected with the pattern `--<param>=<value>` without spaces.
 
-Will show:
+It will show:
 
 ```text
 [CONFIG] Merge 2 default configs, 2 additional configs and 2 CLI parameter(s).
 
 Config:
     param1: -1
     param2: -2
     letters:
         letter1: A
         letter2: B
         letter3: C
 ```
 
-Note that the configurations are native python dicts at each step of the process.
+Note that the configurations is a native python dict at each step of the process.
 
 ## Use tags
 
-By default, the package provides some "tags" that are strings starting with `@`
-and placed at the end of a key containing a parameter. It will change the way
-the configuration is processed.
-
-The default tags are:
-
-* `@merge_add`, `@merge_before` and `@merge_after` to merge the dict loaded
-  from the value (should be a yaml path!) to the current configuration.
-  `@merge_add` allow only new keys and is useful to split sub-configurations
-  in multiple files. `@merge_before` will merge the current dict on the loaded
-  one and `@merge_after` will merge the loaded dict on the current one. With
-  theses tags, you can dynamically merge configurations depending on the paths
-  you set as values.
-* `@copy` Copy a parameter from another key. The value should be a string containing
-  this flatten key
-* `@type:<my type>` To check if the key is of the type `<my type>` at each update
-  even if the tag is no longer present. It supports basic type (except tuple and
-  sets that are not handled by yaml) as well as union (with "Union" or "|"), optional,
-  lists and dicts.
+By default, the package provides some "tags" represented as strings that start with
+'@' and are placed at the end of a key containing a parameter. These tags change
+the way the configuration is processed.
+
+The default tags include:
+
+* `@merge_add`, `@merge_before`, and `@merge_after`: These tags merge the dictionary
+  loaded from the specified value (which should be a YAML path) into the current
+  configuration. `@merge_add` allows only the merging of new keys and is useful for
+  splitting different sub-configurations into multiple files. `@merge_before` merges
+  the current dictionary onto the loaded one, while `@merge_after` merges the loaded
+  dictionary onto the current one. These tags enable dynamic configuration merging
+  on the command line, depending on the specified paths. Note that when multiple
+  `@merge_before` or `@merge_after` tags merge the *same key*, the order of merging
+  is not guaranteed as it depends on the order of the tags in the configuration file.
+* `@copy`: This tag copies a parameter from another key. The value should be a string
+  that represents the flattened key. The copied value is then protected from further
+  updates but will be updated if the copied key change during a merge.
+* `@type:<my type>`: This tag checks if the key matches the specified type `<my type>`
+   after each update, even if the tag is no longer present. It supports basic types
+   (except for tuples and sets, which are not handled by YAML) as well as unions
+   (using "Union" or "|"), optional values, lists, and dictionaries.
 
-The tags are applied in this order: `@merge`, `@copy` then `@type`.
+The tags are applied in the following order: `@merge`, `@copy`, and then `@type`.
 
-Note that the tags are only used to trigger internal processing and will be
-automatically removed from the key after the processing.
+Please note that the tags serve as triggers for internal processing and will be
+automatically removed from the key after processing.
 
-You can also combine the tags, example:
+It is also possible to combine multiple tags. For example:
 
 ```yaml
 ---  # main.yaml
 path_1@merge_add: sub1.yaml
 path_2@merge_add: sub2.yaml
 --- # sub1.yaml
 config1:
-  param@copy@type:int: config1.param2
+  param@copy@type:int: config2.param2
   param2@type:int: 1
 --- # sub2.yaml
 config2.param@type:None|int: 2
 ```
 
 Here `main.yaml` is interpreted like:
 
 ```yaml
 path_1: sub1.yaml
 path_2: sub2.yaml
 config1:
-    param: 1
+    param: 2  # the value of config2.param2
     param2: 1
 config2:
     param: 2
 ```
 
-and now, all the parameters have a forced type.
+Now, all the parameters have a forced type and `config1.param2` will be
+update if `config2.param2` is updated during a merge. These side effects are not
+visible in the config but stored on processing classes. They are objects that
+catch the tags, remove them from config and apply a modification on the config.
+These processing are powerful tools that can be used to highly customize the
+configuration process.
 
-The point is that you can easily create your own processing associated to your
-own tags. They provide a large number of possibilities to customize the
-configuration process and are describe in the
+You can easily create your own processing (associated to a tag or not).
+The way to do it and a further explanation of them is available in the
 [*Processing*](https://cliconfig.readthedocs.io/en/latest/processing.html) section
 of the documentation.
 
 ## Edge cases
 
-**Be careful, tuples and sets are not supported by YAML and cannot be used in
-yaml files.**
-Use lists instead if possible.
-
-`None` is not recognized as a None object by YAML but as a string, you may use `null`
-or `Null` instead if you want to set a None object.
-
-Dicts are considered as sub-configs and so you may not be able to change
-the keys in the additional configs. If you want to modify or add dict keys, you should
-enclose it in a list.
+**Please note that YAML does not support tuples and sets**, and therefore they
+cannot be used in YAML files. If possible, consider using lists instead.
+
+Moreover, YAML does not recognize "None" as a None object, but interprets it as a
+string. If you wish to set a None object, you can use "null" or "Null" instead.
+
+In the context of this package, dictionaries are treated as sub-configurations,
+which means that modifying or adding keys directly in the additional configs may
+not be possible (because only the merge of default configuration allow adding new keys).
+If you need to modify or add keys within a dictionary, consider enclosing it in a list.
 
 For instance:
 
 ```yaml
 --- default.yaml
 logging:
   metrics: ['train loss', 'val loss']
```

### Comparing `cliconfig-0.4.6/cliconfig.egg-info/SOURCES.txt` & `cliconfig-0.4.7/cliconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/docs/Makefile` & `cliconfig-0.4.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/docs/_static/logo.png` & `cliconfig-0.4.7/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/docs/_static/logo_extend.png` & `cliconfig-0.4.7/docs/_static/logo_extend.png`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/docs/cliconfig_api.rst` & `cliconfig-0.4.7/docs/cliconfig_api.rst`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/docs/conf.py` & `cliconfig-0.4.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/docs/index.rst` & `cliconfig-0.4.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/docs/license.md` & `cliconfig-0.4.7/docs/license.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/docs/make.bat` & `cliconfig-0.4.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/docs/processing.md` & `cliconfig-0.4.7/docs/processing.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,134 +1,142 @@
 # Processing
 
-Processing are powerful tools to modify the config at each steps of the life of a
-configuration. More precisely, you can use processing to modify the full configuration
-before and after each merge, after loading and before saving the config.
+Processings are powerful tools to modify the config at each step of the lifecycle of
+a configuration. More precisely, you can use processings to modify the full
+configuration before and after each merge, after loading, and before saving the config.
 
 The processing are applied with a processing class that herits from
-`cliconfig.processing.Processing`. They implement premerge, postmerge, postload and
-presave methods. Each function have the signature:
+`cliconfig.processing.Processing`. They implement `premerge`, `postmerge`, `postload`
+and `presave` methods. Each function have the signature:
 
 ```python
 def premerge(self, flat_dict: Dict[str, Any], processing_list: List[Processing]) -> Dict[str, Any]:
     ...
 ```
 
-They takes a flat dict as input (a dict of depth 1 with dot-separated keys), the list
-of processing (not always needed but useful for more advanced processing,
-it is discussed in an advanced section below) and return the modified flat dict
-(and keep it flat). You can write your own processing objects and add them to the
-`processing_list` argument of `make_config` function to apply it automatically.
-You will see how they work and how to create them in this section.
+They take a flat dict as input (a dict of depth 1 with dot-separated keys), the list
+of processings (not always needed but useful for more advanced processing, as
+discussed in an advanced section below), and return the modified flat dict (while
+keeping it flat). You can write your own processing objects and add them to the
+`processing_list` argument of the `make_config` function to apply them automatically.
+In this section, you will learn how they work and how to create them.
 
 ## Why a flat dict?
 
-The idea is that is that when we build a config, we manipulate dict with both nested
-sub-dicts and flat keys in the same time.To simplify this, the dicts are flatten
-systematically before a merge. It make things mre simple and prevent from duplicated
-key in a same configuration like:
+The idea is that when we construct a config, we manipulate dictionaries that contain
+both nested sub-dicts and flat keys simultaneously. To simplify this process, the
+dictionaries are systematically flattened before merging. This approach makes things
+simpler and prevents duplicated keys within the same configuration, as shown in the
+example:
 
 ```python
 config = {'a': {'b': 1}, 'a.b': 2}
 ```
 
-More generally ALL config modifications are done with flat dicts during config building
-and so it is the case fot the processing too.
+More generally, all config modifications are performed using flat dictionaries
+during config construction, and the same applies to processings.
 
-Of course, after building your config, it will be unflattened to a normal nested config.
+However, it's important to note that after building your config,
+it will be unflattened to its normal nested configuration structure.
 
 ## Processing order
 
-The order of the processing to trigger is actually important because they modify
-the config and so the behavior of the the next processing. That is why
-the Processing classes have 4 float attributes that are the order of the 4 processing
-methods (premerge, postmerge, postload and presave).
+The order in which the processings are triggered is crucial because they modify
+the config and consequently affect the behavior of subsequent processings.
+To manage this order, the Processing classes have four float attributes representing
+the order of the four processing methods: premerge, postmerge, postload, and presave.
 
-An example to illustrate the importance of the order:
+Here's an example to illustrate the significance of the order:
 
 ```yaml
 --- # config.yaml
 param1@type:int@copy: 'param2'
 param2@type:int: 1
 ```
 
-Here, we decide to force the type of the parameters. The `param1` is also the copy
-of `param2` and naturally have the same type.
+In this example, we want to enforce the types of the parameters. Additionally, `param1`
+is intended to be a copy of `param2` and naturally should have the same type.
 
-On pre-merge, the processing will remove the tags and get the information of the
-forced types and the copy. Then, we make a merge (considering to simplify that none of
-our params are modified at this point), the the post-merge processing will be applied.
-
-What happen if the type processing triggers before copy processing? It will check the
-value, that is `"param2"` and raise an error because it is not an int. However, if
-the copy processing trigger before the type processing, it will copy the value of
-`param2` to `param1` (so `1`) and then the type processing not raises an error.
-
-Fortunately, the post-merge orders are `20.0` for the type processing and `10.0` for
-the copy processing so the copy triggers first. Take care of the order when you
-create your own processing!
+During the pre-merge processing, the tags are removed, and information about the
+enforced types and the copy operation is gathered. Then, a merge is performed (assuming
+no modifications to our parameters at this point), followed by the post-merge processing.
+
+Now, what happens if the type processing triggers before the copy processing? It will
+check the value, which is `"param2"`, and raise an error because it is not an integer.
+However, if the copy processing triggers before the type processing, it will copy the
+value of `param2` (which is `1`) to `param1`, and then the type processing will not
+encounter an error.
+
+Fortunately, the post-merge orders are set as follows: `20.0` for the type processing
+and `10.0` for the copy processing. As a result, the copy processing triggers first.
+Therefore, it is crucial to carefully manage the order when creating your own processings.
+
+Ensure you pay attention to the order of your processings to achieve the desired behavior.
 
 ## Create basic processing
 
 ### Pre-merge processing to pass a single value to a function and eventually modify it
 
-The pre-merge processing is kindly the most useful processing because it allows
-to modify the input config written bu the user to create the resulting python dict that
-store the config of your experiment. It is like the interface between the user config
+The pre-merge processing is particularly useful as it allows you to modify the input
+config provided by the user and create the resulting Python dictionary that stores the
+configuration for your experiment. It serves as the interface between the user config
 and the final config.
 
-To do so, you need sometimes to modify the parameters for which the key follows a
-pattern (i.e contains a tag or a particular prefix or suffix) depending on the
-current value.
-
-To do so, we provide the function `cliconfig.create_processing_value` to create such a
-processing quickly. It takes a regex or a tag name (in the latter case, the tag is
-removed after processing), the function to apply on the value to modify it
-and eventually the order of the processing. Finally, it takes a `persistent` bool
-parameter that indicates if encountering the tag (if you have a tag) once will trigger
-the process on all the following keys with the same name even if the tag is absent.
+In a lot of cases, you may need to modify parameters based on certain patterns in their
+keys, such as the presence of a specific tag, prefix, or suffix, depending on
+their current values.
+
+To simplify this process, we provide the `cliconfig.create_processing_value` function.
+This function allows you to quickly create a processing that matches a regular
+expression or a specific tag name (in which case the tag is removed after processing).
+You can specify the function to be applied on the value to modify it, and optionally,
+the order of the processing. Additionally, there is a persistent parameter, which is
+a boolean value indicating whether encountering the tag (if a tag is used) once will
+trigger the processing on all subsequent keys with the same name, even if the tag is
+absent.
 
-The function return a Processing class that can be directly used in your list
-of processing.
+The create_processing_value function returns a Processing class that can be directly
+used in your list of processings.
 
-For instance:
+Here's an example to illustrate:
 
 ```python
 proc = create_processing_value(lambda x: str(x), tag='convert_str', persistent=True)
 config, _ = make_config(default_config, processing_list=[proc])
 ```
 
-Now, parameters like `{"subconfig.param@convert_str": 1}` will be converted to:
-`{"subconfig.param": "1"}` and the keys `"subconfig.param"` will be converted
-to string forever before every merge.
-
-Note that you can also use function that make side effect without changing the value
-(to check if a condition is met for instance).
+In this example, parameters with keys like `{"subconfig.param@convert_str": 1}` will
+be converted to `{"subconfig.param": "1"}`. Moreover, the keys `"subconfig.param"`
+ will be permanently converted to strings before every merge.
+
+It's worth noting that you can also use functions that have side effects without
+necessarily changing the value itself. For example, you can use a function to
+check if a certain condition is met.
 
 ## Create your processing classes
 
-To create your own processing classes and unlock more possibilities, you simply need to
-overload the methods of the `Processing` class to modify the config on the timings
-you want. To do so, you often need to manipulate tags.
+To create your own processing classes and unlock more possibilities, you simply
+need to overload the methods of the Processing class to modify the config at the
+desired timings. To do so, you often need to manipulate tags.
 
 ### Manipulate the tags
 
-Tags are useful to trigger a processing as we have seen. However, we need to take care
-because tagging a key modify its name and can make conflicts when you use several
-in a same key. That is why we provide tags routines to manipulate the tags safely,
-available in `cliconfig.tag_routines`. There are:
+Tags are useful for triggering a processing, as we have seen. However, we need
+to be cautious because tagging a key modifies its name and can lead to conflicts
+when using multiple tags within the same key. To address this issue, we provide
+tag routines in `cliconfig.tag_routines`. These routines include:
 
-* `clean_tag` that remove a tag (with the exact name in input) from a key
-* `clean_all_tags` that remove all tags from a key. It is convenient to store the
+* `clean_tag`: Removes a specific tag (based on its exact name) from a key.
+* `clean_all_tags`: Removes all tags from a key. This is helpful for storing the
   actual key name to process it later.
-* `clean_dict_tags` that remove all tags from a dict and return the cleaned dict and
-  the list of keys containing tags.
+* `clean_dict_tags`: Removes all tags from a dictionary and returns the cleaned
+  dict along with a list of keys that contained tags.
 
-With these tools, we can write for instance a processing that look for a tag "@keep"
-and that restore the value of a parameter after the merge if it was updated.
+With these tools, we can write a processing, for example, that searches for the
+tag `"@keep"` and restores the value of a parameter after the merge if it was updated.
 
 ```python
 class ProcessKeep(Processing):
     """Prevent a value from being changed after the merge."""
 
     def __init__(self) -> None:
         super().__init__()
@@ -159,101 +167,106 @@
             # not necessarily contains all the same keys)
             if key in flat_dict:
                 if flat_dict[key] != value:
                     print(f"WARNING: protected key {key} was modified by the merge")
                 flat_dict[key] = value
         self.keep_vals = {}  # reset the values
         return flat_dict
+
+
+# Use it:
+config, _ = make_config("main.yaml", processing_list=[ProcessKeep()])
 ```
 
-If you not reset `self.keep_vals`, the internal state of the processing will be
-kept and you are able to protect a key forever if it is tagged with
-"@keep" once (in default config for instance). This can be an useful processing!
-
-**Note: Always clean the tag after (or before) using it! If some tags are still present
-after all pre-merge operations, it will trigger a security processing that raise
-an error (for security reasons).**
+If you don't reset `self.keep_vals`, the internal state of the processing will
+be retained, allowing you to protect a key indefinitely if it has been tagged with
+`"@keep"` before (for example, in the default config). This can be a useful processing!
+
+Note: Always remember to clean the tag after (or before) using it! If any tags
+remain present after all pre-merge operations, it will trigger a security processing
+that raises an error (for security reasons).
 
-### Manage the list of processing to create complex processing (Advanced)
+### Manage the list of processings to create complex processing (Advanced)
 
 The key concept is that the elementary operations on the config are not actually
-merge, save and load but actually:
+limited to merge, save, and load, but rather:
 
-* apply premerge processing on two configs, merge the two configs then apply
-  postmerge processing to the output
-* apply presave processing then save a config
-* load a config then apply postload processing
-
-Theses three operations are `cliconfig.merge_processing`, `cliconfig.save_processing`
-and `cliconfig.load_processing` and they naturally take the list of processing as
-input and return the modified list of processing (to keep the internal values
-of the processing).
+* Applying premerge processing, merging and postmerge processing to the output.
+* Applying presave processing and then saving a config.
+* Loading a config and then applying postload processing.
+
+These three operations are in `cliconfig.process_routines` and called
+`merge_processing`, `save_processing`, and `load_processing`, respectively. They take
+the list of processing as input and return the modified list of processing to
+maintain the internal values of the processing.
 
-Now the trick is that sometimes we want to apply these operations on processing
+Now, the trick is that sometimes we want to apply these operations to the processing
 themselves, particularly when we want to modify a part of the configuration instead
-of only one parameter (typically by merging two configurations). That is why we sometimes
-need the list of processing in input of the processing.
+of just a single parameter (such as merging two configurations). This is why we
+sometimes need the list of processing as input for the processing.
 
-An example with the tag "@merge_add", a processing that is triggered
-before merging and that merge the config loaded from a path (the value)
-to the current config. We want to see what happens if we merge a config that
-has also a "@merge_add" tag in it.
+For example, consider the tag "@merge_add," which triggers a processing before
+merging and merges the config loaded from a specified path (the value) into the
+current config. We may want to see what happens if we merge a config that also
+contains an "@merge_add" tag within it:
 
 ```yaml
 --- # main.yaml
 config_path1@merge_add: path1.yaml
 --- # path1.yaml
 param1: 1
 config_path2@merge_add: path2.yaml
 --- # path2.yaml
 param2: 2
 ```
 
-Now, considering that we want to merge the config `main.yaml` with another config.
-The pre-merge processing will be applied and find the tag `@merge_add`.
-It will remove the tag, merge the config found at `path1.yaml` to the config `main.yaml`.
-But it is not a simple merge, it is a merge *with processing*!
-So before merging `path1.yaml`, it will trigger the pre-merge processing on the config,
-find the key `config_path2@merge_add` and merge the config `path2.yaml` to `path1.yaml`.
-Then, it will merge `path1.yaml` to `main.yaml`. Finally, the configuration `main.yaml`
-is interpreted as:
+Now, let's consider we want to merge the config `main.yaml` with another config.
+During the pre-merge processing, we encounter the tag `@merge_add`. This tag is
+removed, and the config found at `path1.yaml` will be merged into the `main.yaml`
+config. However before this, it triggers the pre-merging.
+
+Therefore, before the merge `path1.yaml`, the processing discovers the key
+`config_path2@merge_add` and merges the config found at `path2.yaml` into `path1.yaml`.
+Then, `path1.yaml` is merged into `main.yaml`. Finally, the resulting configuration
+can be interpreted as follows:
 
 ```python
 {'param1': 1, 'param2': 2, 'config_path1': 'path1.yaml', 'config_path2': 'path2.yaml'}
 ```
 
-before being merged itself with another config. Note that is not only a processing that allows
-to organize the configuration on multiple files. In fact, it also allows you to choose a
-particular configuration among several ones by setting the path as value of the tagged
-key.
+before being merged itself with another config. Note that is not only a processing that
+allows to organize the configuration on multiple files. In fact, it also allows you to
+choose a particular configuration among several ones by setting the path as value of
+the tagged key.
 
 **Important:**
-To create a processing that merge, save or load a config, it is also necessary to
-update the list of processing after and before each operation to be sure that you use
-the good internal states of the processing. To pass the list of processing to other
-processing, simply make and update a `processing_list` attribute
-in your processing class. You have an example in `processing.builtin.ProcessMerge`.
+To create a processing that performs merging, saving, or loading of a config, it is
+necessary to update the list of processing before and after each operation. This
+ensures that the correct internal states of the processing are used. In order to pass
+the list of processing to other processing classes, you can create and update a
+processing_list attribute within your processing class. An example of this can be
+found in the `processing.builtin.ProcessMerge` class.
 
 ### Change processing list in processing (Still more advanced)
 
-Note that as the processing functions get the list of processing object at input
-and update it in attribute, it also possible to modify manually this list to
-change internal variables, add or remove processing. This allows you to make more
-complex things but this may have unwanted behavior if you do not know exactly what
-you are doing.
-
-A simple example of use is to make a processing that trigger only once and that adds
-a list of processing to the processing list to avoid passing the full list in
-`make_config`:
+Note that the processing functions receive the list of processing objects as an
+input and update as an attribute of the processing object. This means that it
+is possible to manually modify this list in processing functions to change internal
+variables, add or remove processing. While this flexibility allows for more complex
+operations, it can lead to unintended behavior if not done carefully.
+
+One simple example is creating a processing that triggers only once and adds a
+list of processing to the processing list. This avoids the need to pass the entire
+list in the make_config function.
 
 ```python
 class AddProcessList(Processing):
     def __init__(self):
         super().__init__()
         self.processing_list = self.processing_list.extend(
             [processing1, processing2, processing3, ...]
         )
 
-make_config("main.yaml", processing_list=[AddProcess()])
+config, _ = make_config("main.yaml", processing_list=[AddProcess()])
 ```
 
-You can then create named spaces of processing to organize them.
+This way you can then create named spaces of processing to organize them.
```

### Comparing `cliconfig-0.4.6/docs/quickstart.md` & `cliconfig-0.4.7/docs/quickstart.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Quick start
 
-First create a default config that can be split in multiple files that will be merged
-(from left to right in `make_config` function). There is no limit of depth for the
+Create a default configuration that can be split across multiple files that will
+be merged in sequence. There is no depth limit for the
 configuration parameters.
 
 ```yaml
 ---  # default1.yaml
 param1: 1
 param2: 0
 letters:
@@ -14,123 +14,134 @@
 
 ---  # default2.yaml
 param1: 1
 param2: 2  # will override param2 from default1.yaml
 letters.letter3: c  # add a new parameter
 ```
 
-Now you can set up your program to use the config:
+Now you can write these following lines in your python program to use this config
+with `make_config`:
 
 ```python
 # main.py
-from cliconfig import make_config, show_config
+from cliconfig import make_config, show_dict
 
 config, _ = make_config('default1.yaml', 'default2.yaml')
-show_config(config)  # print the config to check it
+show_dict(config)  # print the config to check it
 ```
 
-Then add one or multiple additional config files that will be passed on command line
-and that will override the default values.
+Then you can add one or multiple additional config files that will be passed on
+command line and that will override the default values.
 
 ```yaml
 ---  # first.yaml
 letters:
   letter3: C
 
 ---  # second.yaml
 param1: -1
 letters.letter1: A
 ```
 
-**Be careful, the additional config files cannot add new parameters that are
-not in default configs**. It is intended to prevent typos in the config files
-that would not be detected. It also improves the readability of the config
-files and the retro-compatibility.
-
-Now you can launch the program with additional configurations and parameters.
-The additional configs will be merged to the default configs, then the parameters
-will be merged.
+**Please note that the additional config files must not introduce new parameters that
+are not in the default configs, as it will result in an error**. This
+restriction is in place to prevent potential typos in the config files from
+going unnoticed. It also enhances the readability of the default config files
+and ensures retro-compatibility.
+
+Now you can launch the program with additional configurations and also set
+individual parameters. The additional configs will be merged to the default
+configs, then the parameters will be merged.
 
 For example:
 
 ```bash
 python main.py --config first.yaml,second.yaml --param2=-2 --letters.letter2='B'
 ```
 
 *Note*: the additional configs are detected with `--config` followed by space
-and separated by a comma **without space**. It also possible to pass a list.
+and separated by comma(s) **without space**. It also possible to pass a list.
 The parameters are detected with the pattern `--<param>=<value>` without spaces.
 
-Will show:
+It will show:
 
 ```text
 [CONFIG] Merge 2 default configs, 2 additional configs and 2 CLI parameter(s).
 
 Config:
     param1: -1
     param2: -2
     letters:
         letter1: A
         letter2: B
         letter3: C
 ```
 
-Note that the configurations are native python dicts at each step of the process.
+Note that the configurations is a native python dict at each step of the process.
 
 ## Use tags
 
-By default, the package provides some "tags" that are strings starting with `@`
-and placed at the end of a key containing a parameter. It will change the way
-the configuration is processed.
-
-The default tags are:
-
-* `@merge_add`, `@merge_before` and `@merge_after` to merge the dict loaded from the
-  value (should be a yaml path!) to the current configuration. `@merge_add` allow
-  only new keys and is useful to split sub-configurations in multiple files.
-  `@merge_before` will merge the current dict on the loaded one and `@merge_after`
-  will merge the loaded dict on the current one. With theses tags, you can dynamically
-  merge configurations depending on the paths you set as values.
-* `@copy` Copy a parameter from another key. The value should be a string containing
-  this flatten key
-* `@type:<my type>` To check if the key is of the type `<my type>` at each update
-  even if the tag is no longer present. It supports basic type (except tuple and sets
-  that are not handled by yaml) as well as union (with "Union" or "|"), optional,
-  lists and dicts.
+By default, the package provides some "tags" represented as strings that start with
+'@' and are placed at the end of a key containing a parameter. These tags change
+the way the configuration is processed.
+
+The default tags include:
+
+* `@merge_add`, `@merge_before`, and `@merge_after`: These tags merge the dictionary
+  loaded from the specified value (which should be a YAML path) into the current
+  configuration. `@merge_add` allows only the merging of new keys and is useful for
+  splitting different sub-configurations into multiple files. `@merge_before` merges
+  the current dictionary onto the loaded one, while `@merge_after` merges the loaded
+  dictionary onto the current one. These tags enable dynamic configuration merging
+  on the command line, depending on the specified paths. Note that when multiple
+  `@merge_before` or `@merge_after` tags merge the *same key*, the order of merging
+  is not guaranteed as it depends on the order of the tags in the configuration file.
+* `@copy`: This tag copies a parameter from another key. The value should be a string
+  that represents the flattened key. The copied value is then protected from further
+  updates but will be updated if the copied key change during a merge.
+* `@type:<my type>`: This tag checks if the key matches the specified type `<my type>`
+   after each update, even if the tag is no longer present. It supports basic types
+   (except for tuples and sets, which are not handled by YAML) as well as unions
+   (using "Union" or "|"), optional values, lists, and dictionaries.
 
-The tags are applied in this order: `@merge`, `@copy` then `@type`.
+The tags are applied in the following order: `@merge`, `@copy`, and then `@type`.
 
-Note that the tags are only used to trigger internal processing and will be
-automatically removed from the key after the processing.
+Please note that the tags serve as triggers for internal processing and will be
+automatically removed from the key after processing.
 
-You can also combine the tags, example:
+It is also possible to combine multiple tags. For example:
 
 ```yaml
 ---  # main.yaml
 path_1@merge_add: sub1.yaml
 path_2@merge_add: sub2.yaml
 --- # sub1.yaml
-config1.param@copy@type:int: config1.param2
-config1.param2@type:int: 1
+config1:
+  param@copy@type:int: config2.param2
+  param2@type:int: 1
 --- # sub2.yaml
 config2.param@type:None|int: 2
 ```
 
 Here `main.yaml` is interpreted like:
 
 ```yaml
 path_1: sub1.yaml
 path_2: sub2.yaml
 config1:
-    param: 1
+    param: 2  # the value of config2.param2
     param2: 1
 config2:
     param: 2
 ```
 
-and now, all the parameters have a forced type.
+Now, all the parameters have a forced type and `config1.param2` will be
+update if `config2.param2` is updated during a merge. These side effects are not
+visible in the config but stored on processing classes. They are objects that
+catch the tags, remove them from config and apply a modification on the config.
+These processing are powerful tools that can be used to highly customize the
+configuration process.
 
-The point is that you can easily create your own processing associated to your own tags.
-They provide a large number of possibilities to customize the configuration process
-and are describe in the
+You can easily create your own processing (associated to a tag or not).
+The way to do it and a further explanation of them is available in the
 [*Processing*](https://cliconfig.readthedocs.io/en/latest/processing.html) section
 of the documentation.
```

### Comparing `cliconfig-0.4.6/github_actions_utils/pydocstyle_manager.py` & `cliconfig-0.4.7/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/github_actions_utils/pylint_manager.py` & `cliconfig-0.4.7/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/github_actions_utils/pytest_manager.py` & `cliconfig-0.4.7/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/licenses_tier/FLATTEN_DICT_LICENSE` & `cliconfig-0.4.7/licenses_tier/FLATTEN_DICT_LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/pre-commit-checks.sh` & `cliconfig-0.4.7/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/pyproject.toml` & `cliconfig-0.4.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/tests/conftest.py` & `cliconfig-0.4.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/tests/integration/test_inte_multiple_tags.py` & `cliconfig-0.4.7/tests/integration/test_inte_multiple_tags.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/tests/unit/processing/test_base.py` & `cliconfig-0.4.7/tests/unit/processing/test_base.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/tests/unit/processing/test_builtin.py` & `cliconfig-0.4.7/tests/unit/processing/test_builtin.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/tests/unit/processing/test_create.py` & `cliconfig-0.4.7/tests/unit/processing/test_create.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/tests/unit/processing/test_type_parser.py` & `cliconfig-0.4.7/tests/unit/processing/test_type_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/tests/unit/test_build_config.py` & `cliconfig-0.4.7/tests/unit/test_build_config.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/tests/unit/test_cli_parser.py` & `cliconfig-0.4.7/tests/unit/test_cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/tests/unit/test_dict_routines.py` & `cliconfig-0.4.7/tests/unit/test_dict_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/tests/unit/test_process_routines.py` & `cliconfig-0.4.7/tests/unit/test_process_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.4.6/tests/unit/test_tag_routines.py` & `cliconfig-0.4.7/tests/unit/test_tag_routines.py`

 * *Files identical despite different names*


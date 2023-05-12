# Comparing `tmp/etils-1.2.0.tar.gz` & `tmp/etils-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etils-1.2.0.tar", last modified: Tue Apr  4 10:26:01 2023, max compression
+gzip compressed data, was "etils-1.3.0.tar", last modified: Fri May 12 12:49:54 2023, max compression
```

## Comparing `etils-1.2.0.tar` & `etils-1.3.0.tar`

### file list

```diff
@@ -1,76 +1,80 @@
--rw-r--r--   0        0        0    11357 2023-04-04 10:25:46.421010 etils-1.2.0/LICENSE
--rw-r--r--   0        0        0     2063 2023-04-04 10:25:46.421010 etils-1.2.0/README.md
--rw-r--r--   0        0        0      859 2023-04-04 10:25:46.421010 etils-1.2.0/etils/__init__.py
--rw-r--r--   0        0        0     1565 2023-04-04 10:25:46.421010 etils-1.2.0/etils/array_types/__init__.py
--rw-r--r--   0        0        0      720 2023-04-04 10:25:46.421010 etils-1.2.0/etils/eapp/__init__.py
--rw-r--r--   0        0        0     2740 2023-04-04 10:25:46.421010 etils-1.2.0/etils/eapp/dataclass_flags.py
--rw-r--r--   0        0        0     3770 2023-04-04 10:25:46.421010 etils-1.2.0/etils/eapp/logging_utils.py
--rw-r--r--   0        0        0     1333 2023-04-04 10:25:46.421010 etils-1.2.0/etils/ecolab/__init__.py
--rw-r--r--   0        0        0     6379 2023-04-04 10:25:46.421010 etils-1.2.0/etils/ecolab/array_as_img.py
--rw-r--r--   0        0        0     5297 2023-04-04 10:25:46.421010 etils-1.2.0/etils/ecolab/colab_utils.py
--rw-r--r--   0        0        0      583 2023-04-04 10:25:46.425010 etils-1.2.0/etils/ecolab/inspects/__init__.py
--rw-r--r--   0        0        0     1500 2023-04-04 10:25:46.425010 etils-1.2.0/etils/ecolab/inspects/attrs.py
--rw-r--r--   0        0        0     2630 2023-04-04 10:25:46.425010 etils-1.2.0/etils/ecolab/inspects/auto_utils.py
--rw-r--r--   0        0        0     2050 2023-04-04 10:25:46.425010 etils-1.2.0/etils/ecolab/inspects/core.py
--rw-r--r--   0        0        0     2047 2023-04-04 10:25:46.425010 etils-1.2.0/etils/ecolab/inspects/html_helper.py
--rw-r--r--   0        0        0    14441 2023-04-04 10:25:46.429010 etils-1.2.0/etils/ecolab/inspects/nodes.py
--rw-r--r--   0        0        0     1226 2023-04-04 10:25:46.429010 etils-1.2.0/etils/ecolab/inspects/resource_utils.py
--rw-r--r--   0        0        0      191 2023-04-04 10:25:46.429010 etils-1.2.0/etils/ecolab/inspects/static/auto_activate.css
--rw-r--r--   0        0        0     1500 2023-04-04 10:25:46.429010 etils-1.2.0/etils/ecolab/inspects/static/auto_activate.js
--rw-r--r--   0        0        0     2487 2023-04-04 10:25:46.429010 etils-1.2.0/etils/ecolab/inspects/static/main.js
--rw-r--r--   0        0        0     2557 2023-04-04 10:25:46.429010 etils-1.2.0/etils/ecolab/inspects/static/theme.css
--rw-r--r--   0        0        0    16275 2023-04-04 10:25:46.429010 etils-1.2.0/etils/ecolab/lazy_imports.py
--rw-r--r--   0        0        0     4563 2023-04-04 10:25:46.429010 etils-1.2.0/etils/ecolab/module_utils.py
--rw-r--r--   0        0        0     2441 2023-04-04 10:25:46.429010 etils-1.2.0/etils/ecolab/patch_utils.py
--rw-r--r--   0        0        0      756 2023-04-04 10:25:46.429010 etils-1.2.0/etils/ecolab/pyjs_com/__init__.py
--rw-r--r--   0        0        0     3031 2023-04-04 10:25:46.429010 etils-1.2.0/etils/ecolab/pyjs_com/py_js_com.js
--rw-r--r--   0        0        0     4428 2023-04-04 10:25:46.429010 etils-1.2.0/etils/ecolab/pyjs_com/py_js_com.py
--rw-r--r--   0        0        0     1282 2023-04-04 10:25:46.429010 etils-1.2.0/etils/ecolab/test_utils.py
--rw-r--r--   0        0        0      831 2023-04-04 10:25:46.429010 etils-1.2.0/etils/edc/__init__.py
--rw-r--r--   0        0        0     4083 2023-04-04 10:25:46.429010 etils-1.2.0/etils/edc/cast_utils.py
--rw-r--r--   0        0        0     7002 2023-04-04 10:25:46.429010 etils-1.2.0/etils/edc/dataclass_utils.py
--rw-r--r--   0        0        0     5405 2023-04-04 10:25:46.429010 etils-1.2.0/etils/edc/field_utils.py
--rw-r--r--   0        0        0     8161 2023-04-04 10:25:46.429010 etils-1.2.0/etils/edc/frozen_utils.py
--rw-r--r--   0        0        0     1919 2023-04-04 10:25:46.429010 etils-1.2.0/etils/enp/__init__.py
--rw-r--r--   0        0        0     3494 2023-04-04 10:25:46.429010 etils-1.2.0/etils/enp/array_spec.py
--rw-r--r--   0        0        0      603 2023-04-04 10:25:46.429010 etils-1.2.0/etils/enp/array_types/__init__.py
--rw-r--r--   0        0        0     7867 2023-04-04 10:25:46.429010 etils-1.2.0/etils/enp/array_types/dtypes.py
--rw-r--r--   0        0        0     3677 2023-04-04 10:25:46.429010 etils-1.2.0/etils/enp/array_types/typing.py
--rw-r--r--   0        0        0     9794 2023-04-04 10:25:46.429010 etils-1.2.0/etils/enp/checking.py
--rw-r--r--   0        0        0     4233 2023-04-04 10:25:46.429010 etils-1.2.0/etils/enp/compat.py
--rw-r--r--   0        0        0     2726 2023-04-04 10:25:46.429010 etils-1.2.0/etils/enp/geo_utils.py
--rw-r--r--   0        0        0     4128 2023-04-04 10:25:46.429010 etils-1.2.0/etils/enp/interp_utils.py
--rw-r--r--   0        0        0     1034 2023-04-04 10:25:46.429010 etils-1.2.0/etils/enp/linalg.py
--rw-r--r--   0        0        0    10814 2023-04-04 10:25:46.429010 etils-1.2.0/etils/enp/numpy_utils.py
--rw-r--r--   0        0        0     2804 2023-04-04 10:25:46.429010 etils-1.2.0/etils/enp/testing.py
--rw-r--r--   0        0        0     2086 2023-04-04 10:25:46.429010 etils-1.2.0/etils/enp/type_parsing.py
--rw-r--r--   0        0        0     2192 2023-04-04 10:25:46.429010 etils-1.2.0/etils/enp/typing.py
--rw-r--r--   0        0        0      995 2023-04-04 10:25:46.429010 etils-1.2.0/etils/epath/__init__.py
--rw-r--r--   0        0        0     6239 2023-04-04 10:25:46.429010 etils-1.2.0/etils/epath/abstract_path.py
--rw-r--r--   0        0        0     9084 2023-04-04 10:25:46.429010 etils-1.2.0/etils/epath/backend.py
--rw-r--r--   0        0        0     3159 2023-04-04 10:25:46.429010 etils-1.2.0/etils/epath/flags.py
--rw-r--r--   0        0        0     8951 2023-04-04 10:25:46.429010 etils-1.2.0/etils/epath/gpath.py
--rw-r--r--   0        0        0     3410 2023-04-04 10:25:46.429010 etils-1.2.0/etils/epath/register.py
--rw-r--r--   0        0        0     4766 2023-04-04 10:25:46.429010 etils-1.2.0/etils/epath/resource_utils.py
--rw-r--r--   0        0        0      922 2023-04-04 10:25:46.429010 etils-1.2.0/etils/epath/stat_utils.py
--rw-r--r--   0        0        0     4852 2023-04-04 10:25:46.429010 etils-1.2.0/etils/epath/testing.py
--rw-r--r--   0        0        0      940 2023-04-04 10:25:46.429010 etils-1.2.0/etils/epath/typing.py
--rw-r--r--   0        0        0     1467 2023-04-04 10:25:46.429010 etils-1.2.0/etils/epy/__init__.py
--rw-r--r--   0        0        0     1332 2023-04-04 10:25:46.429010 etils-1.2.0/etils/epy/_internal.py
--rw-r--r--   0        0        0     1629 2023-04-04 10:25:46.429010 etils-1.2.0/etils/epy/backports.py
--rw-r--r--   0        0        0     2173 2023-04-04 10:25:46.429010 etils-1.2.0/etils/epy/contextlib.py
--rw-r--r--   0        0        0     1097 2023-04-04 10:25:46.429010 etils-1.2.0/etils/epy/env_utils.py
--rw-r--r--   0        0        0     3777 2023-04-04 10:25:46.429010 etils-1.2.0/etils/epy/itertools.py
--rw-r--r--   0        0        0     4060 2023-04-04 10:25:46.429010 etils-1.2.0/etils/epy/py_utils.py
--rw-r--r--   0        0        0     4859 2023-04-04 10:25:46.429010 etils-1.2.0/etils/epy/reraise_utils.py
--rw-r--r--   0        0        0     2843 2023-04-04 10:25:46.429010 etils-1.2.0/etils/epy/testing.py
--rw-r--r--   0        0        0     4558 2023-04-04 10:25:46.429010 etils-1.2.0/etils/epy/text_utils.py
--rw-r--r--   0        0        0      642 2023-04-04 10:25:46.429010 etils-1.2.0/etils/etqdm/__init__.py
--rw-r--r--   0        0        0     1454 2023-04-04 10:25:46.429010 etils-1.2.0/etils/etqdm/tqdm_utils.py
--rw-r--r--   0        0        0     1195 2023-04-04 10:25:46.429010 etils-1.2.0/etils/etree/__init__.py
--rw-r--r--   0        0        0     7798 2023-04-04 10:25:46.433010 etils-1.2.0/etils/etree/backend.py
--rw-r--r--   0        0        0     4998 2023-04-04 10:25:46.433010 etils-1.2.0/etils/etree/tree_utils.py
--rw-r--r--   0        0        0      906 2023-04-04 10:25:46.433010 etils-1.2.0/etils/etree/typing.py
--rw-r--r--   0        0        0     1049 2023-04-04 10:25:46.433010 etils-1.2.0/etils/lazy_imports/__init__.py
--rw-r--r--   0        0        0     2769 2023-04-04 10:25:46.433010 etils-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5509 1970-01-01 00:00:00.000000 etils-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-12 12:49:33.017113 etils-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2063 2023-05-12 12:49:33.017113 etils-1.3.0/README.md
+-rw-r--r--   0        0        0      859 2023-05-12 12:49:33.017113 etils-1.3.0/etils/__init__.py
+-rw-r--r--   0        0        0     1565 2023-05-12 12:49:33.017113 etils-1.3.0/etils/array_types/__init__.py
+-rw-r--r--   0        0        0      720 2023-05-12 12:49:33.017113 etils-1.3.0/etils/eapp/__init__.py
+-rw-r--r--   0        0        0     2740 2023-05-12 12:49:33.017113 etils-1.3.0/etils/eapp/dataclass_flags.py
+-rw-r--r--   0        0        0     3770 2023-05-12 12:49:33.017113 etils-1.3.0/etils/eapp/logging_utils.py
+-rw-r--r--   0        0        0     1229 2023-05-12 12:49:33.017113 etils-1.3.0/etils/ecolab/__init__.py
+-rw-r--r--   0        0        0     6379 2023-05-12 12:49:33.017113 etils-1.3.0/etils/ecolab/array_as_img.py
+-rw-r--r--   0        0        0     6156 2023-05-12 12:49:33.017113 etils-1.3.0/etils/ecolab/colab_utils.py
+-rw-r--r--   0        0        0     1511 2023-05-12 12:49:33.025113 etils-1.3.0/etils/ecolab/highlight_util.py
+-rw-r--r--   0        0        0      583 2023-05-12 12:49:33.025113 etils-1.3.0/etils/ecolab/inspects/__init__.py
+-rw-r--r--   0        0        0     1500 2023-05-12 12:49:33.025113 etils-1.3.0/etils/ecolab/inspects/attrs.py
+-rw-r--r--   0        0        0     2630 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/inspects/auto_utils.py
+-rw-r--r--   0        0        0     2050 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/inspects/core.py
+-rw-r--r--   0        0        0     2047 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/inspects/html_helper.py
+-rw-r--r--   0        0        0    14441 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/inspects/nodes.py
+-rw-r--r--   0        0        0     1540 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/inspects/resource_utils.py
+-rw-r--r--   0        0        0      191 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/inspects/static/auto_activate.css
+-rw-r--r--   0        0        0     1500 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/inspects/static/auto_activate.js
+-rw-r--r--   0        0        0     2487 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/inspects/static/main.js
+-rw-r--r--   0        0        0     2557 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/inspects/static/theme.css
+-rw-r--r--   0        0        0    16290 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/lazy_imports.py
+-rw-r--r--   0        0        0     4563 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/module_utils.py
+-rw-r--r--   0        0        0     2441 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/patch_utils.py
+-rw-r--r--   0        0        0      756 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/pyjs_com/__init__.py
+-rw-r--r--   0        0        0     3031 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/pyjs_com/py_js_com.js
+-rw-r--r--   0        0        0     4460 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/pyjs_com/py_js_com.py
+-rw-r--r--   0        0        0     1074 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/static/highlight.css
+-rw-r--r--   0        0        0     1282 2023-05-12 12:49:33.029113 etils-1.3.0/etils/ecolab/test_utils.py
+-rw-r--r--   0        0        0      872 2023-05-12 12:49:33.029113 etils-1.3.0/etils/edc/__init__.py
+-rw-r--r--   0        0        0     1678 2023-05-12 12:49:33.029113 etils-1.3.0/etils/edc/cast_utils.py
+-rw-r--r--   0        0        0     2621 2023-05-12 12:49:33.029113 etils-1.3.0/etils/edc/context.py
+-rw-r--r--   0        0        0     8594 2023-05-12 12:49:33.029113 etils-1.3.0/etils/edc/dataclass_utils.py
+-rw-r--r--   0        0        0     5405 2023-05-12 12:49:33.029113 etils-1.3.0/etils/edc/field_utils.py
+-rw-r--r--   0        0        0     8161 2023-05-12 12:49:33.029113 etils-1.3.0/etils/edc/frozen_utils.py
+-rw-r--r--   0        0        0     5001 2023-05-12 12:49:33.029113 etils-1.3.0/etils/edc/helpers.py
+-rw-r--r--   0        0        0     1919 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/__init__.py
+-rw-r--r--   0        0        0     3680 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/array_spec.py
+-rw-r--r--   0        0        0      603 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/array_types/__init__.py
+-rw-r--r--   0        0        0     7867 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/array_types/dtypes.py
+-rw-r--r--   0        0        0     3677 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/array_types/typing.py
+-rw-r--r--   0        0        0     9794 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/checking.py
+-rw-r--r--   0        0        0     4233 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/compat.py
+-rw-r--r--   0        0        0     2726 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/geo_utils.py
+-rw-r--r--   0        0        0     4128 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/interp_utils.py
+-rw-r--r--   0        0        0     1034 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/linalg.py
+-rw-r--r--   0        0        0    10814 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/numpy_utils.py
+-rw-r--r--   0        0        0     2804 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/testing.py
+-rw-r--r--   0        0        0     2086 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/type_parsing.py
+-rw-r--r--   0        0        0     2192 2023-05-12 12:49:33.029113 etils-1.3.0/etils/enp/typing.py
+-rw-r--r--   0        0        0      995 2023-05-12 12:49:33.029113 etils-1.3.0/etils/epath/__init__.py
+-rw-r--r--   0        0        0     6239 2023-05-12 12:49:33.029113 etils-1.3.0/etils/epath/abstract_path.py
+-rw-r--r--   0        0        0     9084 2023-05-12 12:49:33.029113 etils-1.3.0/etils/epath/backend.py
+-rw-r--r--   0        0        0     3159 2023-05-12 12:49:33.029113 etils-1.3.0/etils/epath/flags.py
+-rw-r--r--   0        0        0     9026 2023-05-12 12:49:33.029113 etils-1.3.0/etils/epath/gpath.py
+-rw-r--r--   0        0        0     3410 2023-05-12 12:49:33.029113 etils-1.3.0/etils/epath/register.py
+-rw-r--r--   0        0        0     4937 2023-05-12 12:49:33.029113 etils-1.3.0/etils/epath/resource_utils.py
+-rw-r--r--   0        0        0      922 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epath/stat_utils.py
+-rw-r--r--   0        0        0     4927 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epath/testing.py
+-rw-r--r--   0        0        0      940 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epath/typing.py
+-rw-r--r--   0        0        0     1467 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epy/__init__.py
+-rw-r--r--   0        0        0     1332 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epy/_internal.py
+-rw-r--r--   0        0        0     1629 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epy/backports.py
+-rw-r--r--   0        0        0     2173 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epy/contextlib.py
+-rw-r--r--   0        0        0     1097 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epy/env_utils.py
+-rw-r--r--   0        0        0     3777 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epy/itertools.py
+-rw-r--r--   0        0        0     4060 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epy/py_utils.py
+-rw-r--r--   0        0        0     4859 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epy/reraise_utils.py
+-rw-r--r--   0        0        0     2843 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epy/testing.py
+-rw-r--r--   0        0        0     6165 2023-05-12 12:49:33.033113 etils-1.3.0/etils/epy/text_utils.py
+-rw-r--r--   0        0        0      642 2023-05-12 12:49:33.033113 etils-1.3.0/etils/etqdm/__init__.py
+-rw-r--r--   0        0        0     1454 2023-05-12 12:49:33.033113 etils-1.3.0/etils/etqdm/tqdm_utils.py
+-rw-r--r--   0        0        0     1195 2023-05-12 12:49:33.033113 etils-1.3.0/etils/etree/__init__.py
+-rw-r--r--   0        0        0     7798 2023-05-12 12:49:33.033113 etils-1.3.0/etils/etree/backend.py
+-rw-r--r--   0        0        0     4998 2023-05-12 12:49:33.033113 etils-1.3.0/etils/etree/tree_utils.py
+-rw-r--r--   0        0        0      906 2023-05-12 12:49:33.033113 etils-1.3.0/etils/etree/typing.py
+-rw-r--r--   0        0        0     1049 2023-05-12 12:49:33.033113 etils-1.3.0/etils/lazy_imports/__init__.py
+-rw-r--r--   0        0        0     2893 2023-05-12 12:49:33.033113 etils-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5459 1970-01-01 00:00:00.000000 etils-1.3.0/PKG-INFO
```

### Comparing `etils-1.2.0/LICENSE` & `etils-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/README.md` & `etils-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/__init__.py` & `etils-1.3.0/etils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Etils API."""
 
 # A new PyPI release will be pushed everytime `__version__` is increased
 # When changing this, also update the CHANGELOG.md
-__version__ = '1.2.0'
+__version__ = '1.3.0'
 
 # Do NOT add anything to this file. This is left empty on purpose.
 # Users should import subprojects directly.
```

### Comparing `etils-1.2.0/etils/array_types/__init__.py` & `etils-1.3.0/etils/array_types/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/eapp/__init__.py` & `etils-1.3.0/etils/eapp/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/eapp/dataclass_flags.py` & `etils-1.3.0/etils/eapp/dataclass_flags.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/eapp/logging_utils.py` & `etils-1.3.0/etils/eapp/logging_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/ecolab/__init__.py` & `etils-1.3.0/etils/ecolab/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,24 +14,15 @@
 
 """Colab public API."""
 
 from etils.ecolab.array_as_img import auto_plot_array
 from etils.ecolab.colab_utils import collapse
 from etils.ecolab.colab_utils import interruptible
 from etils.ecolab.colab_utils import json
+from etils.ecolab.highlight_util import highlight_html
 from etils.ecolab.inspects.auto_utils import auto_inspect
 from etils.ecolab.inspects.core import inspect
 from etils.ecolab.module_utils import clear_cached_modules
 from etils.ecolab.patch_utils import patch_graphviz
 from etils.ecolab.patch_utils import set_verbose
 from etils.ecolab.pyjs_com import js_import as pyjs_import
 from etils.ecolab.pyjs_com import register_js_fn
-
-__all__ = [
-    'auto_plot_array',
-    'collapse',
-    'clear_cached_modules',
-    'inspect',
-    'interruptible',
-    'patch_graphviz',
-    'set_verbose',
-]
```

### Comparing `etils-1.2.0/etils/ecolab/array_as_img.py` & `etils-1.3.0/etils/ecolab/array_as_img.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/ecolab/colab_utils.py` & `etils-1.3.0/etils/ecolab/colab_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,25 +59,55 @@
 def _redirect_stdall(new_target: io.StringIO) -> Iterator[None]:
   with contextlib.redirect_stderr(new_target):
     with contextlib.redirect_stdout(new_target):
       yield
 
 
 @contextlib.contextmanager
-def collapse(name: str = '') -> Iterator[None]:
+def collapse(name: str = '', *, widget: bool = False) -> Iterator[None]:
   """Capture stderr/stdout and display it in a collapsible block.
 
   Args:
     name: Name of the collapsible section.
+    widget: If True, use `ipywidgets` backend. Will become the default in the
+      future (output appear in real time, support HTML,...)
 
   Yields:
     None
   """
-  with _collapse_std(name=name, redirect_fn=_redirect_stdall):
-    yield
+  if widget:
+    with _collapse_widget(name):
+      yield
+  else:
+    with _collapse_std(name=name, redirect_fn=_redirect_stdall):
+      yield
+
+
+@contextlib.contextmanager
+def _collapse_widget(name: str = '') -> Iterator[None]:
+  """Widget implementation of Collapsible widget."""
+  import ipywidgets  # pylint: disable=g-import-not-at-top
+
+  out = ipywidgets.Output()
+  accordion = ipywidgets.Accordion(children=[out])
+  accordion.set_title(0, name)
+  accordion.selected_index = None
+  IPython.display.display(accordion)
+  with out:
+    try:
+      yield
+    except Exception as e:
+      # ipywidgets.Output erase exceptions, so we save it and reraise it after
+      # the scope.
+      exc = e
+      raise
+    else:
+      exc = None
+  if exc is not None:
+    raise exc
 
 
 def json(value: Json) -> None:
   """Display the Json `dict` / `list` interactivelly (with collapsible elems).
 
   Examples:
```

### Comparing `etils-1.2.0/etils/ecolab/inspects/__init__.py` & `etils-1.3.0/etils/ecolab/inspects/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/ecolab/inspects/attrs.py` & `etils-1.3.0/etils/ecolab/inspects/attrs.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/ecolab/inspects/auto_utils.py` & `etils-1.3.0/etils/ecolab/inspects/auto_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/ecolab/inspects/core.py` & `etils-1.3.0/etils/ecolab/inspects/core.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/ecolab/inspects/html_helper.py` & `etils-1.3.0/etils/ecolab/inspects/html_helper.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/ecolab/inspects/nodes.py` & `etils-1.3.0/etils/ecolab/inspects/nodes.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/ecolab/inspects/resource_utils.py` & `etils-1.3.0/etils/ecolab/highlight_util.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,31 +8,51 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Resource utils."""
+"""Syntax highlighting utils."""
 
-import functools
+from etils import epy
 
-from etils import epath
+from etils.ecolab.inspects import resource_utils
 
 
-def _static_path() -> epath.Path:
-  """Path to the static resources (`.js`, `.css`)."""
-  return epath.resource_path('etils') / 'ecolab' / 'inspects' / 'static'
-
-
-# TODO(epot): Use gstatic to serve those files.
-@functools.lru_cache()
-def resource_import(filename: str) -> str:
-  """Returns the `HTML` associated with the resource."""
-  path = _static_path().joinpath(filename)
-  content = path.read_text()
-  if path.suffix == '.css':
-    return f'<style>{content}</style>'
-  elif path.suffix == '.js':
-    return f'<script>{content}</script>'
-  else:
-    raise ValueError('')
+def highlight_html(code: str) -> str:
+  """Add Python syntax highlighting to a Python code string.
+
+  Usage:
+
+  Example:
+
+  ```python
+  @dataclasses.dataclass
+  class A:
+    x: int
+
+    def _repr_html_(self) -> str:
+      from etils import ecolab  # Lazy-import ecolab
+
+      return ecolab.highlight_html(repr(self))
+
+  ```
+
+  Args:
+    code: The string to wrap
+
+  Returns:
+    The HTML string representation
+  """
+  theme = resource_utils.resource_import(
+      'static/highlight.css', module='etils.ecolab'
+  )
+  html = """
+  {theme}
+  <script src="//cdnjs.cloudflare.com/ajax/libs/highlight.js/11.7.0/highlight.min.js"></script>
+  <script>hljs.highlightAll();</script>
+  <pre><code class="language-python">{code}</code></pre>
+  """
+  html = epy.dedent(html)
+  html = html.format(theme=theme, code=code)
+  return html
```

#### html2text {}

```diff
@@ -1,17 +1,19 @@
 # Copyright 2023 The etils Authors. # # Licensed under the Apache License,
 Version 2.0 (the "License"); # you may not use this file except in compliance
 with the License. # You may obtain a copy of the License at # # http://
 www.apache.org/licenses/LICENSE-2.0 # # Unless required by applicable law or
 agreed to in writing, software # distributed under the License is distributed
 on an "AS IS" BASIS, # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 express or implied. # See the License for the specific language governing
-permissions and # limitations under the License. """Resource utils.""" import
-functools from etils import epath def _static_path() -> epath.Path: """Path to
-the static resources (`.js`, `.css`).""" return epath.resource_path('etils') /
-'ecolab' / 'inspects' / 'static' # TODO(epot): Use gstatic to serve those
-files. @functools.lru_cache() def resource_import(filename: str) -> str:
-"""Returns the `HTML` associated with the resource.""" path = _static_path
-().joinpath(filename) content = path.read_text() if path.suffix == '.css':
-return f'
-' elif path.suffix == '.js': return f'
-' else: raise ValueError('')
+permissions and # limitations under the License. """Syntax highlighting
+utils.""" from etils import epy from etils.ecolab.inspects import
+resource_utils def highlight_html(code: str) -> str: """Add Python syntax
+highlighting to a Python code string. Usage: Example: ```python
+@dataclasses.dataclass class A: x: int def _repr_html_(self) -> str: from etils
+import ecolab # Lazy-import ecolab return ecolab.highlight_html(repr(self)) ```
+Args: code: The string to wrap Returns: The HTML string representation """
+theme = resource_utils.resource_import( 'static/highlight.css',
+module='etils.ecolab' ) html = """ {theme}
+{code}
+""" html = epy.dedent(html) html = html.format(theme=theme, code=code) return
+html
```

### Comparing `etils-1.2.0/etils/ecolab/inspects/static/auto_activate.js` & `etils-1.3.0/etils/ecolab/inspects/static/auto_activate.js`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/ecolab/inspects/static/main.js` & `etils-1.3.0/etils/ecolab/inspects/static/main.js`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/ecolab/inspects/static/theme.css` & `etils-1.3.0/etils/ecolab/inspects/static/theme.css`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/ecolab/lazy_imports.py` & `etils-1.3.0/etils/ecolab/lazy_imports.py`

 * *Files 0% similar despite different names*

```diff
@@ -510,14 +510,15 @@
   import matplotlib as mpl  # Standard alias
   from matplotlib import pyplot as plt
   import mediapy as media
   import ml_collections
   import networkx as nx
   import numpy as np
   import optax
+  import orbax
   import pandas as pd
   import PIL
   from PIL import Image  # Common alias
   import pycolmap
   import scipy
   import seaborn as sns
   import sklearn
```

### Comparing `etils-1.2.0/etils/ecolab/module_utils.py` & `etils-1.3.0/etils/ecolab/module_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/ecolab/patch_utils.py` & `etils-1.3.0/etils/ecolab/patch_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/ecolab/pyjs_com/__init__.py` & `etils-1.3.0/etils/ecolab/pyjs_com/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/ecolab/pyjs_com/py_js_com.js` & `etils-1.3.0/etils/ecolab/pyjs_com/py_js_com.js`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/ecolab/pyjs_com/py_js_com.py` & `etils-1.3.0/etils/ecolab/pyjs_com/py_js_com.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 class _Colab(_NotebookBackend):
   """Backend for Colab."""
 
   def wrap_output(self, out):
     return IPython.display.JSON(out)
 
   def register_fn(self, fn: _Fn) -> None:
-    from google.colab import output  # pylint: disable=g-import-not-at-top
+    from google.colab import output  # pylint: disable=g-import-not-at-top  # pytype: disable=import-error
 
     # TODO(epot): Fragile if multiple functions have the same name. How to
     # specify namespace ?
     output.register_callback(fn.__name__, fn)
 
 
 class _Jupyter(_NotebookBackend):
```

### Comparing `etils-1.2.0/etils/ecolab/test_utils.py` & `etils-1.3.0/etils/ecolab/test_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/edc/__init__.py` & `etils-1.3.0/etils/edc/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,10 +11,11 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Dataclasses utils."""
 
 from etils.edc.cast_utils import AutoCast
+from etils.edc.context import ContextVar
 from etils.edc.dataclass_utils import __repr__ as repr  # pylint: disable=redefined-builtin
 from etils.edc.dataclass_utils import dataclass
 from etils.edc.field_utils import field
```

### Comparing `etils-1.2.0/etils/edc/dataclass_utils.py` & `etils-1.3.0/etils/edc/dataclass_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,54 +21,59 @@
 import inspect
 import reprlib
 import typing
 from typing import Any, Callable, TypeVar
 
 from etils import epy
 from etils.edc import cast_utils
+from etils.edc import context
 from etils.edc import frozen_utils
+from etils.edc import helpers
 
 _Cls = Any
 _ClsT = TypeVar('_ClsT')
 _T = TypeVar('_T')
 
 
 @typing.overload
 def dataclass(
     cls: None = ...,
     *,
     kw_only: bool = ...,
     replace: bool = ...,  # pylint: disable=redefined-outer-name
     repr: bool = ...,  # pylint: disable=redefined-builtin
     auto_cast: bool = ...,
+    contextvars: bool = ...,
     allow_unfrozen: bool = ...,
 ) -> Callable[[_ClsT], _ClsT]:
   ...
 
 
 @typing.overload
 def dataclass(
     cls: _ClsT,
     *,
     kw_only: bool = ...,
     replace: bool = ...,  # pylint: disable=redefined-outer-name
     repr: bool = ...,  # pylint: disable=redefined-builtin
     auto_cast: bool = ...,
+    contextvars: bool = ...,
     allow_unfrozen: bool = ...,
 ) -> _ClsT:
   ...
 
 
 def dataclass(
     cls=None,
     *,
     kw_only=False,
     replace=True,  # pylint: disable=redefined-outer-name
     repr=True,  # pylint: disable=redefined-builtin
     auto_cast=True,
+    contextvars=True,
     allow_unfrozen=False,
 ):
   """Augment a dataclass with additional features.
 
   `auto_cast`: Auto-convert init assignements to the annotated class.
 
   ```python
@@ -141,22 +146,55 @@
     y = a.y
     a = a.frozen()
 
     y.x  # Raise error (created between the unfrozen/frozen call)
     a.y.x  # Work
     ```
 
+  `contextvars`: Fields annotated as `edc.ContextVar` are wrapped in
+  a `contextvars.ContextVar`. Afterward each thread / asyncio coroutine will
+  have its own version of the fields (similarly to `threading.local`).
+
+  The contextvars are lazily initialized at first usage.
+
+  Example:
+
+  ```python
+  @edc.dataclass
+  @dataclasses.dataclass
+  class Context:
+    thread_id: edc.ContextVar[int] = dataclasses.field(
+        default_factory=threading.get_native_id
+    )
+    stack: edc.ContextVar[list[str]] = dataclasses.field(default_factory=list)
+
+  # Global context object
+  context = Context(thread_id=0)
+
+  def worker():
+    # Inside each thread, the worker use its own context
+    assert context.thread_id != 0
+    context.stack.append(1)
+
+  with concurrent.futures.ThreadPoolExecutor(max_workers=5) as executor:
+    for _ in range(10):
+      executor.submit(worker)
+  ```
+
   Args:
     cls: The dataclass to decorate
     kw_only: If True, make the dataclass `__init__` keyword-only.
     replace: If `True`, add a `.replace(` alias of `dataclasses.replace`.
     repr: If `True`, the class `__repr__` will return a pretty-printed `str`
       (one attribute per line)
-    auto_cast: If `True`, field annotated as `x: edc.AutoCast[Cls]` will be
+    auto_cast: If `True`, fields annotated as `x: edc.AutoCast[Cls]` will be
       converted to `x: Cls = edc.field(validator=Cls)`.
+    contextvars: It `True`, fields annotated as `x: edc.AutoCast[T]` are
+      converted to `contextvars`. This allow to have a `threading.local`-like
+      API for contextvars.
     allow_unfrozen: If `True`, add `.frozen`, `.unfrozen` methods.
 
   Returns:
     Decorated class
   """
   # Return decorator
   if cls is None:
@@ -177,16 +215,32 @@
 
   if replace:
     cls = _add_replace(cls)
 
   if allow_unfrozen:
     cls = frozen_utils.add_unfrozen(cls)
 
+  descriptor_fns = []
   if auto_cast:
-    cls = cast_utils.apply_auto_cast_to_field(cls)
+    descriptor_fns.append(
+        helpers.DescriptorInfo(
+            annotation=cast_utils.AutoCast,
+            descriptor_fn=cast_utils.make_auto_cast_descriptor,
+        )
+    )
+
+  if contextvars:
+    descriptor_fns.append(
+        helpers.DescriptorInfo(
+            annotation=context.ContextVar,
+            descriptor_fn=context.make_contextvar_descriptor,
+        )
+    )
+
+  cls = helpers.wrap_new(cls, descriptor_fns)
 
   return cls
 
 
 def _make_kw_only(cls: _ClsT) -> _ClsT:
   """Replace the `__init__` by a keyword-only version."""
   # Use `cls.__dict__` and not `hasattr` to ignore parent classes
@@ -245,12 +299,12 @@
 def __repr__(self) -> str:  # pylint: disable=invalid-name
   """Pretty-print `repr`."""
   all_fields = dataclasses.fields(self)
 
   return epy.Lines.make_block(
       header=self.__class__.__name__,
       content={
-          field.name: repr(getattr(self, field.name))
+          field.name: getattr(self, field.name)
           for field in all_fields
           if field.repr
       },
   )
```

### Comparing `etils-1.2.0/etils/edc/field_utils.py` & `etils-1.3.0/etils/edc/field_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/edc/frozen_utils.py` & `etils-1.3.0/etils/edc/frozen_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/enp/__init__.py` & `etils-1.3.0/etils/enp/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/enp/array_spec.py` & `etils-1.3.0/etils/enp/array_spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """Array spec utils."""
 
 # Is there a way of merging this with array_types ?
 
 from __future__ import annotations
 
 import functools
+import sys
 from typing import Any, Optional
 
 from etils.enp import numpy_utils
 from etils.enp.array_types import typing as array_types
 from etils.enp.typing import Array
 import numpy as np
 
@@ -97,14 +98,19 @@
         array,
         (lazy.tf.TensorSpec, lazy.tf.Tensor),
     ):
       shape = array.shape
       dtype = array.dtype.as_numpy_dtype
     elif lazy.has_tf and isinstance(array, type(_get_none_spec())):
       return None  # Special case for `NoneTensorSpec()`
+    elif 'grain.tensorflow' in sys.modules and isinstance(
+        array, sys.modules['grain.tensorflow'].ArraySpec
+    ):
+      shape = array.shape
+      dtype = array.dtype
     elif isinstance(array, array_types.ArrayAliasMeta):
       try:
         shape = (int(s) for s in array.shape.split())
       except ValueError:
         raise UnknownArrayError(
             f'Not supported dynamic shape: {array}'
         ) from None
```

### Comparing `etils-1.2.0/etils/enp/array_types/__init__.py` & `etils-1.3.0/etils/enp/array_types/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/enp/array_types/dtypes.py` & `etils-1.3.0/etils/enp/array_types/dtypes.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/enp/array_types/typing.py` & `etils-1.3.0/etils/enp/array_types/typing.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/enp/checking.py` & `etils-1.3.0/etils/enp/checking.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/enp/compat.py` & `etils-1.3.0/etils/enp/compat.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/enp/geo_utils.py` & `etils-1.3.0/etils/enp/geo_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/enp/interp_utils.py` & `etils-1.3.0/etils/enp/interp_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/enp/linalg.py` & `etils-1.3.0/etils/enp/linalg.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/enp/numpy_utils.py` & `etils-1.3.0/etils/enp/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/enp/testing.py` & `etils-1.3.0/etils/enp/testing.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/enp/type_parsing.py` & `etils-1.3.0/etils/enp/type_parsing.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/enp/typing.py` & `etils-1.3.0/etils/enp/typing.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/epath/__init__.py` & `etils-1.3.0/etils/epath/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/epath/abstract_path.py` & `etils-1.3.0/etils/epath/abstract_path.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/epath/backend.py` & `etils-1.3.0/etils/epath/backend.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/epath/flags.py` & `etils-1.3.0/etils/epath/flags.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/epath/gpath.py` & `etils-1.3.0/etils/epath/gpath.py`

 * *Files 5% similar despite different names*

```diff
@@ -197,15 +197,15 @@
       self._backend.remove(self._path_str)
     except FileNotFoundError:
       if missing_ok:
         pass
       else:
         raise
 
-  def open(
+  def open(  # pytype: disable=signature-mismatch  # overriding-parameter-count-checks
       self,
       mode: str = 'r',
       *,
       encoding: Optional[str] = None,
       errors: Optional[str] = None,
       **kwargs: Any,
   ) -> typing.IO[Union[str, bytes]]:
```

### Comparing `etils-1.2.0/etils/epath/register.py` & `etils-1.3.0/etils/epath/register.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/epath/resource_utils.py` & `etils-1.3.0/etils/epath/resource_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 
 @register.register_path_cls
 class ResourcePath(zipfile.Path):
   """Wrapper around `zipfile.Path` compatible with `os.PathLike`.
 
   Note: Calling `os.fspath` on the path will extract the file so should be
   discouraged.
-
   """
 
   def __fspath__(self) -> str:
     """Path string for `os.path.join`, `open`,...
 
     compatibility.
 
@@ -72,14 +71,20 @@
 
     # Before 3.10, joinpath only accept a single arg
     def joinpath(self, *other):
       """Overwrite `joinpath` to be consistent with `pathlib.Path`."""
       next_ = posixpath.join(self.at, *other)  # pytype: disable=attribute-error
       return self._next(self.root.resolve_dir(next_))  # pytype: disable=attribute-error
 
+  if sys.version_info < (3, 11):
+
+    @property
+    def suffix(self):
+      return pathlib.Path(self.at).suffix or self.filename.suffix  # pytype: disable=attribute-error
+
 
 def resource_path(package: Union[str, types.ModuleType]) -> abstract_path.Path:
   """Returns read-only root directory path of the module.
 
   Used to access module resource files.
 
   Usage:
```

### Comparing `etils-1.2.0/etils/epath/stat_utils.py` & `etils-1.3.0/etils/epath/stat_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/epath/testing.py` & `etils-1.3.0/etils/epath/testing.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
   def rename(self, path: PathLike, dst: PathLike) -> None:
     return self._get_fn('rename')(path, dst)
 
   def replace(self, path: PathLike, dst: PathLike) -> None:
     return self._get_fn('replace')(path, dst)
 
-  def copy(self, path: PathLike, dst: PathLike, *, overwrite: bool) -> None:
+  def copy(self, path: PathLike, dst: PathLike, *, overwrite: bool) -> None:  # pytype: disable=signature-mismatch  # overriding-parameter-count-checks
     return self._get_fn('copy')(path, dst, overwrite=overwrite)
 
   def stat(self, path: PathLike) -> stat_utils.StatResult:
     return self._get_fn('stat')(path)
 
 
 @contextlib.contextmanager
```

### Comparing `etils-1.2.0/etils/epath/typing.py` & `etils-1.3.0/etils/epath/typing.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/epy/__init__.py` & `etils-1.3.0/etils/epy/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/epy/_internal.py` & `etils-1.3.0/etils/epy/_internal.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/epy/backports.py` & `etils-1.3.0/etils/epy/backports.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/epy/contextlib.py` & `etils-1.3.0/etils/epy/contextlib.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/epy/env_utils.py` & `etils-1.3.0/etils/epy/env_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/epy/itertools.py` & `etils-1.3.0/etils/epy/itertools.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/epy/py_utils.py` & `etils-1.3.0/etils/epy/py_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/epy/reraise_utils.py` & `etils-1.3.0/etils/epy/reraise_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/epy/testing.py` & `etils-1.3.0/etils/epy/testing.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/epy/text_utils.py` & `etils-1.3.0/etils/epy/text_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """Text utils."""
 
 from __future__ import annotations
 
 import contextlib
 import dataclasses
 import textwrap
-from typing import Iterable, Iterator, Union
+from typing import Any, Iterable, Iterator, Union
 
 _BRACE_TO_BRACES = {
     '(': ('(', ')'),
     '[': ('[', ']'),
     '{': ('{', '}'),
 }
 
@@ -126,18 +126,20 @@
     else:
       token = '\n'
     return token.join(lines)
 
   @classmethod
   def make_block(
       cls,
-      header: str,
-      content: dict[str, str],
+      header: str = '',
+      content: str | dict[str, Any] | list[Any] | tuple[Any, ...] = (),
       *,
       braces: Union[str, tuple[str, str]] = '(',
+      equal: str = '=',
+      limit: int = 20,
   ) -> str:
     """Util function to create a code block.
 
     Example:
 
     ```python
     epy.Lines.make_block('A', {}) == 'A()'
@@ -158,34 +160,85 @@
     ```
 
     Args:
       header: Prefix before the brace
       content: Dict of key to values. One line will be displayed per item if
         `len(content) > 1`. Otherwise the code is collapsed
       braces: Brace type (`(`, `[`, `{`), can be tuple for custom open/close.
+      equal: The separator (`=`, `: `)
+      limit: Strings smaller than this will be collapsed
 
     Returns:
       The block string
     """
-    collapse = len(content) <= 1
-    trailing = '' if collapse else ','
-
     if isinstance(braces, str):
       braces = _BRACE_TO_BRACES[braces]
     brace_start, brace_end = braces
 
+    if isinstance(content, str):
+      content = [content]
+
+    if isinstance(content, dict):
+      parts = [f'{k}{equal}{_repr_value(v)}' for k, v in content.items()]
+    elif isinstance(content, (list, tuple)):
+      parts = [f'{_repr_value(v)}' for v in content]
+    else:
+      raise TypeError(f'Invalid fields {type(content)}')
+
+    collapse = len(parts) <= 1
+    if any('\n' in p for p in parts):
+      collapse = False
+    # Also collapse string which are small
+    elif sum(len(p) for p in parts) <= limit:
+      collapse = True
+
     lines = cls()
     lines += f'{header}{brace_start}'
     with lines.indent():
-      for k, v in content.items():
-        lines += f'{k}={v}{trailing}'
+      if collapse:
+        lines += ', '.join(parts)
+      else:
+        for p in parts:
+          lines += f'{p},'
     lines += f'{brace_end}'
 
     return lines.join(collapse=collapse)
 
+  @classmethod
+  def repr(cls, obj: Any) -> str:
+    """Pretty print object."""
+    return _repr_value(obj)
+
+
+def _repr_value(obj: Any) -> str:
+  """Object representation, pretty-display for list, dict,..."""
+  from etils import edc  # pylint: disable=g-import-not-at-top
+
+  if isinstance(obj, str):
+    return repr(obj)
+  elif type(obj) in (list, tuple):  # Skip sub-class as could have custom repr
+    return Lines.make_block(
+        content=obj,
+        braces='[' if isinstance(obj, list) else '(',
+    )
+  elif type(obj) is dict:  # pylint: disable=unidiomatic-typecheck
+    return Lines.make_block(
+        content={repr(k): v for k, v in obj.items()},
+        braces='{',
+        equal=': ',
+    )
+  elif (
+      not isinstance(obj, type)
+      and dataclasses.is_dataclass(obj)
+      and edc.dataclass_utils.has_default_repr(type(obj))
+  ):
+    return edc.repr(obj)
+  else:
+    return repr(obj)
+
 
 def dedent(text: str) -> str:
   r"""Wrapper around `textwrap.dedent` which also `strip()` the content.
 
   Before:
 
   ```python
```

### Comparing `etils-1.2.0/etils/etqdm/__init__.py` & `etils-1.3.0/etils/etqdm/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/etqdm/tqdm_utils.py` & `etils-1.3.0/etils/etqdm/tqdm_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/etree/__init__.py` & `etils-1.3.0/etils/etree/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/etree/backend.py` & `etils-1.3.0/etils/etree/backend.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/etree/tree_utils.py` & `etils-1.3.0/etils/etree/tree_utils.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/etree/typing.py` & `etils-1.3.0/etils/etree/typing.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/etils/lazy_imports/__init__.py` & `etils-1.3.0/etils/lazy_imports/__init__.py`

 * *Files identical despite different names*

### Comparing `etils-1.2.0/pyproject.toml` & `etils-1.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     "jupyter",
     "numpy",
     "mediapy",
     "etils[enp]",
     "etils[epy]",
 ]
 edc = [
-    "typing_extensions",
+    # Do not add anything here. `edc` is an alias for `epy`
     "etils[epy]",
 ]
 enp = [
     "numpy",
     "etils[epy]",
 ]
 epath = [
@@ -109,15 +109,17 @@
 
 dev = [
     "pytest",
     "pytest-subtests",
     "pytest-xdist",
     "pyink",
     "pylint>=2.6.0",
+    # Lazy deps
     "chex",
+    # "grain",  # For `etree.spec_like`  # TODO(epot): Add once released
     "torch",
     "optree",  # For `etree.optree`
 ]
 
 [tool.flit.sdist]
 # Do not release tests, doc on PyPI
 exclude = [
```

### Comparing `etils-1.2.0/PKG-INFO` & `etils-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etils
-Version: 1.2.0
+Version: 1.3.0
 Summary: Collection of common python utils
 Keywords: utils,jax,tensorflow,tf,machine learning,deep learning
 Author-email: Conchylicultor <etils@google.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -37,15 +37,14 @@
 Requires-Dist: simple_parsing ; extra == "eapp"
 Requires-Dist: etils[epy] ; extra == "eapp"
 Requires-Dist: jupyter ; extra == "ecolab"
 Requires-Dist: numpy ; extra == "ecolab"
 Requires-Dist: mediapy ; extra == "ecolab"
 Requires-Dist: etils[enp] ; extra == "ecolab"
 Requires-Dist: etils[epy] ; extra == "ecolab"
-Requires-Dist: typing_extensions ; extra == "edc"
 Requires-Dist: etils[epy] ; extra == "edc"
 Requires-Dist: numpy ; extra == "enp"
 Requires-Dist: etils[epy] ; extra == "enp"
 Requires-Dist: importlib_resources ; extra == "epath"
 Requires-Dist: typing_extensions ; extra == "epath"
 Requires-Dist: zipp ; extra == "epath"
 Requires-Dist: etils[epy] ; extra == "epath"
```


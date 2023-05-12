# Comparing `tmp/cleanlab-studio-1.0.4.tar.gz` & `tmp/cleanlab-studio-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanlab-studio-1.0.4.tar", last modified: Thu May 11 00:02:06 2023, max compression
+gzip compressed data, was "cleanlab-studio-1.0.5.tar", last modified: Fri May 12 20:04:29 2023, max compression
```

## Comparing `cleanlab-studio-1.0.4.tar` & `cleanlab-studio-1.0.5.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.838179 cleanlab-studio-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-05-11 00:02:06.838179 cleanlab-studio-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.822179 cleanlab-studio-1.0.4/cleanlab_studio/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.826179 cleanlab-studio-1.0.4/cleanlab_studio/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11692 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/api_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.826179 cleanlab-studio-1.0.4/cleanlab_studio/cli/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/classes/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/classes/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/classes/excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/classes/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.826179 cleanlab-studio-1.0.4/cleanlab_studio/cli/cleanset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/cleanset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/cleanset/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/cleanset/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/cleanset/download_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/click_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.830179 cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/schema_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/schema_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    24955 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/upload_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.830179 cleanlab-studio-1.0.4/cleanlab_studio/cli/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/decorators/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/decorators/previous_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.830179 cleanlab-studio-1.0.4/cleanlab_studio/cli/login/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/login/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.830179 cleanlab-studio-1.0.4/cleanlab_studio/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.830179 cleanlab-studio-1.0.4/cleanlab_studio/internal/api/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.834179 cleanlab-studio-1.0.4/cleanlab_studio/internal/dataset_source/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/dataset_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/dataset_source/dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/internal/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.834179 cleanlab-studio-1.0.4/cleanlab_studio/studio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/studio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/studio/studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/studio/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/cleanlab_studio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.826179 cleanlab-studio-1.0.4/cleanlab_studio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-05-11 00:02:06.000000 cleanlab-studio-1.0.4/cleanlab_studio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-11 00:02:06.000000 cleanlab-studio-1.0.4/cleanlab_studio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 00:02:06.000000 cleanlab-studio-1.0.4/cleanlab_studio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-11 00:02:06.000000 cleanlab-studio-1.0.4/cleanlab_studio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-11 00:02:06.000000 cleanlab-studio-1.0.4/cleanlab_studio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-11 00:02:06.000000 cleanlab-studio-1.0.4/cleanlab_studio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 00:02:06.838179 cleanlab-studio-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.834179 cleanlab-studio-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/tests/bench.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 00:02:06.834179 cleanlab-studio-1.0.4/tests/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/tests/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/tests/datasets/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/tests/datasets/test_csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/tests/datasets/test_excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/tests/datasets/test_json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-11 00:01:38.000000 cleanlab-studio-1.0.4/tests/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.794393 cleanlab-studio-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-05-12 20:04:29.794393 cleanlab-studio-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.790393 cleanlab-studio-1.0.5/cleanlab_studio/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.790393 cleanlab-studio-1.0.5/cleanlab_studio/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11692 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/api_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.790393 cleanlab-studio-1.0.5/cleanlab_studio/cli/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/classes/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/classes/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/classes/excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/classes/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.790393 cleanlab-studio-1.0.5/cleanlab_studio/cli/cleanset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/cleanset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/cleanset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/cleanset/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/cleanset/download_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/click_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.790393 cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/schema_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/schema_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24955 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/upload_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.794393 cleanlab-studio-1.0.5/cleanlab_studio/cli/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/decorators/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/decorators/previous_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.794393 cleanlab-studio-1.0.5/cleanlab_studio/cli/login/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/login/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.794393 cleanlab-studio-1.0.5/cleanlab_studio/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.794393 cleanlab-studio-1.0.5/cleanlab_studio/internal/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.794393 cleanlab-studio-1.0.5/cleanlab_studio/internal/dataset_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/dataset_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/dataset_source/dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/internal/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.794393 cleanlab-studio-1.0.5/cleanlab_studio/studio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/studio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/studio/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/studio/studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/studio/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/cleanlab_studio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.790393 cleanlab-studio-1.0.5/cleanlab_studio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-05-12 20:04:29.000000 cleanlab-studio-1.0.5/cleanlab_studio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-12 20:04:29.000000 cleanlab-studio-1.0.5/cleanlab_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:04:29.000000 cleanlab-studio-1.0.5/cleanlab_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-12 20:04:29.000000 cleanlab-studio-1.0.5/cleanlab_studio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-12 20:04:29.000000 cleanlab-studio-1.0.5/cleanlab_studio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-12 20:04:29.000000 cleanlab-studio-1.0.5/cleanlab_studio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 20:04:29.794393 cleanlab-studio-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.794393 cleanlab-studio-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/tests/bench.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:29.794393 cleanlab-studio-1.0.5/tests/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/tests/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/tests/datasets/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/tests/datasets/test_csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/tests/datasets/test_excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/tests/datasets/test_json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-12 20:04:13.000000 cleanlab-studio-1.0.5/tests/datasets/utils.py
```

### Comparing `cleanlab-studio-1.0.4/LICENSE` & `cleanlab-studio-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/PKG-INFO` & `cleanlab-studio-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 1.0.4
+Version: 1.0.5
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
+Project-URL: Documentation, https://cleanlab-studio.readthedocs.io/en/latest/index.html
 Keywords: cleanlab
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Natural Language :: English
@@ -21,20 +22,23 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: docs
 License-File: LICENSE
 
-# cleanlab-studio [![Build Status](https://github.com/cleanlab/cleanlab-studio/workflows/CI/badge.svg)](https://github.com/cleanlab/cleanlab-studio/actions?query=workflow%3ACI) [![PyPI](https://img.shields.io/pypi/v/cleanlab-studio.svg)][PyPI]
+# cleanlab-studio [![Build Status](https://github.com/cleanlab/cleanlab-studio/workflows/CI/badge.svg)](https://github.com/cleanlab/cleanlab-studio/actions?query=workflow%3ACI) [![PyPI](https://img.shields.io/pypi/v/cleanlab-studio.svg)][PyPI] ![ReadTheDocs](https://readthedocs.org/projects/cleanlab-studio/badge/?version=latest)
 
 Command line and Python library interface to [Cleanlab Studio](https://cleanlab.ai/studio/). Upload datasets and download cleansets (cleaned datasets) from Cleanlab Studio in a single line of code!
 
+Comprehensive docs can be found [here](https://cleanlab-studio.readthedocs.io/en/latest/index.html).
+
 - [Installation](#installation)
 - [Quickstart](#quickstart)
 - [Advanced Usage](#advanced-usage)
 
 ## Installation
 
 You can install the Cleanlab Studio client [from PyPI][PyPI] with:
```

### Comparing `cleanlab-studio-1.0.4/README.md` & `cleanlab-studio-1.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-# cleanlab-studio [![Build Status](https://github.com/cleanlab/cleanlab-studio/workflows/CI/badge.svg)](https://github.com/cleanlab/cleanlab-studio/actions?query=workflow%3ACI) [![PyPI](https://img.shields.io/pypi/v/cleanlab-studio.svg)][PyPI]
+# cleanlab-studio [![Build Status](https://github.com/cleanlab/cleanlab-studio/workflows/CI/badge.svg)](https://github.com/cleanlab/cleanlab-studio/actions?query=workflow%3ACI) [![PyPI](https://img.shields.io/pypi/v/cleanlab-studio.svg)][PyPI] ![ReadTheDocs](https://readthedocs.org/projects/cleanlab-studio/badge/?version=latest)
 
 Command line and Python library interface to [Cleanlab Studio](https://cleanlab.ai/studio/). Upload datasets and download cleansets (cleaned datasets) from Cleanlab Studio in a single line of code!
 
+Comprehensive docs can be found [here](https://cleanlab-studio.readthedocs.io/en/latest/index.html).
+
 - [Installation](#installation)
 - [Quickstart](#quickstart)
 - [Advanced Usage](#advanced-usage)
 
 ## Installation
 
 You can install the Cleanlab Studio client [from PyPI][PyPI] with:
```

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/cli/api_service.py` & `cleanlab-studio-1.0.5/cleanlab_studio/cli/api_service.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/cli/classes/csv_dataset.py` & `cleanlab-studio-1.0.5/cleanlab_studio/cli/classes/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/cli/classes/dataset.py` & `cleanlab-studio-1.0.5/cleanlab_studio/cli/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/cli/classes/excel_dataset.py` & `cleanlab-studio-1.0.5/cleanlab_studio/cli/classes/excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/cli/classes/json_dataset.py` & `cleanlab-studio-1.0.5/cleanlab_studio/cli/classes/json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/cli/cleanset/download.py` & `cleanlab-studio-1.0.5/cleanlab_studio/cli/cleanset/download.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/cli/cleanset/download_helpers.py` & `cleanlab-studio-1.0.5/cleanlab_studio/cli/cleanset/download_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/cli/click_helpers.py` & `cleanlab-studio-1.0.5/cleanlab_studio/cli/click_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/helpers.py` & `cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/image_utils.py` & `cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/image_utils.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/schema_helpers.py` & `cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/schema_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/schema_types.py` & `cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/schema_types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/upload.py` & `cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/upload.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/upload_helpers.py` & `cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/cli/dataset/upload_types.py` & `cleanlab-studio-1.0.5/cleanlab_studio/cli/dataset/upload_types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/cli/decorators/auth_config.py` & `cleanlab-studio-1.0.5/cleanlab_studio/cli/decorators/auth_config.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/cli/decorators/previous_state.py` & `cleanlab-studio-1.0.5/cleanlab_studio/cli/decorators/previous_state.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/cli/login/login.py` & `cleanlab-studio-1.0.5/cleanlab_studio/cli/login/login.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/cli/main.py` & `cleanlab-studio-1.0.5/cleanlab_studio/cli/main.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/cli/types.py` & `cleanlab-studio-1.0.5/cleanlab_studio/cli/types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/cli/util.py` & `cleanlab-studio-1.0.5/cleanlab_studio/cli/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/errors.py` & `cleanlab-studio-1.0.5/cleanlab_studio/errors.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/internal/api/api.py` & `cleanlab-studio-1.0.5/cleanlab_studio/internal/api/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from cleanlab_studio.version import __version__
 
 base_url = os.environ.get("CLEANLAB_API_BASE_URL", "https://api.cleanlab.ai/api")
 cli_base_url = f"{base_url}/cli/v0"
 upload_base_url = f"{base_url}/upload/v0"
 dataset_base_url = f"{base_url}/datasets"
 project_base_url = f"{base_url}/projects"
+cleanset_base_url = f"{base_url}/cleansets"
 
 
 def _construct_headers(
     api_key: Optional[str], content_type: Optional[str] = "application/json"
 ) -> JSONDict:
     retval = dict()
     if api_key:
@@ -39,15 +40,17 @@
             raise APIError(res_json["description"])
     if res_json.get("error", None) is not None:
         raise APIError(res_json["error"])
 
 
 def validate_api_key(api_key: str) -> bool:
     res = requests.get(
-        cli_base_url + "/validate", json=dict(api_key=api_key), headers=_construct_headers(api_key)
+        cli_base_url + "/validate",
+        json=dict(api_key=api_key),
+        headers=_construct_headers(api_key),
     )
     handle_api_error(res)
     valid: bool = res.json()["valid"]
     return valid
 
 
 def is_valid_client_version() -> bool:
@@ -71,15 +74,17 @@
     presigned_posts: List[str] = res.json()["presigned_posts"]
     return upload_id, part_sizes, presigned_posts
 
 
 def complete_file_upload(api_key: str, upload_id: str, upload_parts: List[JSONDict]) -> None:
     request_json = dict(upload_id=upload_id, upload_parts=upload_parts)
     res = requests.post(
-        f"{upload_base_url}/complete", json=request_json, headers=_construct_headers(api_key)
+        f"{upload_base_url}/complete",
+        json=request_json,
+        headers=_construct_headers(api_key),
     )
     handle_api_error(res)
 
 
 def get_proposed_schema(api_key: str, upload_id: str) -> JSONDict:
     res = requests.get(
         f"{upload_base_url}/proposed_schema",
@@ -94,15 +99,17 @@
 def confirm_schema(
     api_key: str,
     schema: Optional[JSONDict],
     upload_id: str,
 ) -> None:
     request_json = dict(schema=schema, upload_id=upload_id)
     res = requests.post(
-        f"{upload_base_url}/confirm_schema", json=request_json, headers=_construct_headers(api_key)
+        f"{upload_base_url}/confirm_schema",
+        json=request_json,
+        headers=_construct_headers(api_key),
     )
     handle_api_error(res)
 
 
 def get_ingestion_status(api_key: str, upload_id: str) -> JSONDict:
     res = requests.get(
         f"{upload_base_url}/ingestion_status",
@@ -203,39 +210,61 @@
     return dataset_details
 
 
 def clean_dataset(
     api_key: str,
     dataset_id: str,
     project_name: str,
-    tasktype: str,
+    task_type: str,
     modality: str,
-    modeltype: str,
+    model_type: str,
     label_column: str,
     feature_columns: List[str],
     text_column: Optional[str],
 ) -> str:
     request_json = dict(
         name=project_name,
         dataset_id=dataset_id,
-        tasktype=tasktype,
+        tasktype=task_type,
         modality=modality,
-        model_type=modeltype,
+        model_type=model_type,
         label_column=label_column,
         feature_columns=feature_columns,
         text_column=text_column,
     )
     res = requests.post(
-        project_base_url + f"/clean", headers=_construct_headers(api_key), json=request_json
+        project_base_url + f"/clean",
+        headers=_construct_headers(api_key),
+        json=request_json,
     )
     handle_api_error(res)
     project_id = res.json()["project_id"]
     return str(project_id)
 
 
+def get_latest_cleanset_id(api_key: str, project_id: str) -> str:
+    res = requests.get(
+        cleanset_base_url + f"/project/{project_id}/latest_cleanset_id",
+        headers=_construct_headers(api_key),
+    )
+    handle_api_error(res)
+    cleanset_id = res.json()["cleanset_id"]
+    return str(cleanset_id)
+
+
+def get_cleanset_status(api_key: str, cleanset_id: str) -> JSONDict:
+    res = requests.get(
+        cleanset_base_url + f"/{cleanset_id}/status",
+        headers=_construct_headers(api_key),
+    )
+    handle_api_error(res)
+    status: JSONDict = res.json()
+    return status
+
+
 def poll_progress(
     progress_id: str, request_function: Callable[[str], JSONDict], description: str
 ) -> JSONDict:
     with tqdm(total=1, desc=description, bar_format="{desc}: {percentage:3.0f}%|{bar}|") as pbar:
         res = request_function(progress_id)
         while res["status"] != "complete":
             if res["status"] == "error":
```

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py` & `cleanlab-studio-1.0.5/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/internal/dataset_source/dataset_source.py` & `cleanlab-studio-1.0.5/cleanlab_studio/internal/dataset_source/dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py` & `cleanlab-studio-1.0.5/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py` & `cleanlab-studio-1.0.5/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/internal/settings.py` & `cleanlab-studio-1.0.5/cleanlab_studio/internal/settings.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/internal/upload_helpers.py` & `cleanlab-studio-1.0.5/cleanlab_studio/internal/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/internal/util.py` & `cleanlab-studio-1.0.5/cleanlab_studio/internal/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/studio/studio.py` & `cleanlab-studio-1.0.5/cleanlab_studio/studio/studio.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 try:
     import pyspark.sql
 
     pyspark_exists = True
 except ImportError:
     pyspark_exists = False
 
-from . import upload
+from . import clean, upload
 from cleanlab_studio.internal.api import api
 from cleanlab_studio.internal.util import init_dataset_source, as_numpy_type
 from cleanlab_studio.internal.settings import CleanlabSettings
 from cleanlab_studio.internal.types import FieldSchemaDict
 
 
 class Studio:
@@ -57,15 +57,19 @@
 
     def download_cleanlab_columns(self, cleanset_id: str) -> pd.DataFrame:
         project_id = api.get_project_of_cleanset(self._api_key, cleanset_id)
         label_column = api.get_label_column_of_project(self._api_key, project_id)
         return self._download_cleanlab_columns(cleanset_id, project_id, label_column)
 
     def _download_cleanlab_columns(
-        self, cleanset_id: str, project_id: str, label_column: str, include_action: bool = False
+        self,
+        cleanset_id: str,
+        project_id: str,
+        label_column: str,
+        include_action: bool = False,
     ) -> pd.DataFrame:
         rows = api.download_cleanlab_columns(self._api_key, cleanset_id, all=True)
         id_col = api.get_id_column(self._api_key, cleanset_id)
         # TODO actually get _all_ the columns incl e.g., cleanlab_top_labels
         # and have the API give the column headers rather than this library hard-coding it
         headers = [
             id_col,
@@ -150,28 +154,28 @@
 
     def create_project(
         self,
         dataset_id: str,
         project_name: str,
         modality: Literal["text", "tabular", "image"],
         *,
-        tasktype: Literal["multi-class", "multi-label"] = "multi-class",
-        modeltype: Literal["fast", "regular"] = "regular",
+        task_type: Literal["multi-class", "multi-label"] = "multi-class",
+        model_type: Literal["fast", "regular"] = "regular",
         label_column: Optional[str] = None,
         feature_columns: Optional[List[str]] = None,
         text_column: Optional[str] = None,
     ) -> str:
         """
         Creates a Cleanlab Studio project
 
         :param dataset_id: ID of dataset to create project for
         :param project_name: name for resulting project
         :param modality: modality of project (i.e. text, tabular, image)
-        :keyword tasktype: type of classification to perform (i.e. multi-class, multi-label)
-        :keyword modeltype: type of model to train (i.e. fast, regular)
+        :keyword task_type: type of classification to perform (i.e. multi-class, multi-label)
+        :keyword model_type: type of model to train (i.e. fast, regular)
         :keyword label_column: name of column in dataset containing labels (if not supplied, we'll make our best guess)
         :keyword feature_columns: list of columns to use as features when training tabular modality project (if not supplied and modality is "tabular" we'll use all valid feature columns)
         :keyword text_column: name of column containing the text to train text modality project on (if not supplied and modality is "text" we'll make our best guess)
 
         :return: ID of project
         """
         dataset_details = api.get_dataset_details(self._api_key, dataset_id)
@@ -206,14 +210,26 @@
             text_column = dataset_details["text_column_guess"]
             print(f"Text column not supplied. Using best guess {text_column}")
 
         return api.clean_dataset(
             api_key=self._api_key,
             dataset_id=dataset_id,
             project_name=project_name,
-            tasktype=tasktype,
+            task_type=task_type,
             modality=modality,
-            modeltype=modeltype,
+            model_type=model_type,
             label_column=label_column,
             feature_columns=feature_columns if feature_columns is not None else [],
             text_column=text_column,
         )
+
+    def poll_cleanset_status(self, cleanset_id: str, timeout: Optional[int] = None) -> bool:
+        """
+        Polls for cleanset status. Blocks until cleanset is ready, there is a cleanset error, or `timeout` is exceeded
+
+        :return: True if cleanset is ready, False otherwise
+        """
+        return clean.poll_cleanset_status(self._api_key, cleanset_id, timeout)
+
+    def get_latest_cleanset_id(self, project_id: str) -> str:
+        """Gets latest cleanset ID for a project"""
+        return api.get_latest_cleanset_id(self._api_key, project_id)
```

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio/studio/upload.py` & `cleanlab-studio-1.0.5/cleanlab_studio/studio/upload.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio.egg-info/PKG-INFO` & `cleanlab-studio-1.0.5/cleanlab_studio.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 1.0.4
+Version: 1.0.5
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
+Project-URL: Documentation, https://cleanlab-studio.readthedocs.io/en/latest/index.html
 Keywords: cleanlab
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Natural Language :: English
@@ -21,20 +22,23 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: docs
 License-File: LICENSE
 
-# cleanlab-studio [![Build Status](https://github.com/cleanlab/cleanlab-studio/workflows/CI/badge.svg)](https://github.com/cleanlab/cleanlab-studio/actions?query=workflow%3ACI) [![PyPI](https://img.shields.io/pypi/v/cleanlab-studio.svg)][PyPI]
+# cleanlab-studio [![Build Status](https://github.com/cleanlab/cleanlab-studio/workflows/CI/badge.svg)](https://github.com/cleanlab/cleanlab-studio/actions?query=workflow%3ACI) [![PyPI](https://img.shields.io/pypi/v/cleanlab-studio.svg)][PyPI] ![ReadTheDocs](https://readthedocs.org/projects/cleanlab-studio/badge/?version=latest)
 
 Command line and Python library interface to [Cleanlab Studio](https://cleanlab.ai/studio/). Upload datasets and download cleansets (cleaned datasets) from Cleanlab Studio in a single line of code!
 
+Comprehensive docs can be found [here](https://cleanlab-studio.readthedocs.io/en/latest/index.html).
+
 - [Installation](#installation)
 - [Quickstart](#quickstart)
 - [Advanced Usage](#advanced-usage)
 
 ## Installation
 
 You can install the Cleanlab Studio client [from PyPI][PyPI] with:
```

### Comparing `cleanlab-studio-1.0.4/cleanlab_studio.egg-info/SOURCES.txt` & `cleanlab-studio-1.0.5/cleanlab_studio.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 cleanlab_studio/internal/dataset_source/__init__.py
 cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
 cleanlab_studio/internal/dataset_source/dataset_source.py
 cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
 cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
 cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
 cleanlab_studio/studio/__init__.py
+cleanlab_studio/studio/clean.py
 cleanlab_studio/studio/studio.py
 cleanlab_studio/studio/upload.py
 tests/__init__.py
 tests/bench.py
 tests/datasets/__init__.py
 tests/datasets/constants.py
 tests/datasets/test_csv_dataset.py
```

### Comparing `cleanlab-studio-1.0.4/setup.py` & `cleanlab-studio-1.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     author_email="team@cleanlab.ai",
     description="Client interface for all things Cleanlab Studio",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cleanlab/cleanlab-studio",
     project_urls={
         "Bug Tracker": "https://github.com/cleanlab/cleanlab-studio/issues",
+        "Documentation": "https://cleanlab-studio.readthedocs.io/en/latest/index.html",
     },
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Information Technology",
@@ -56,12 +57,20 @@
         "ijson>=3.1.4",
         "jsonstreams>=0.6.0",
         "semver>=2.13.0,<3.0.0",
         "Pillow>=9.2.0",
         "openpyxl==3.0.10",
         "validators>=0.20.0",
     ],
+    extras_require={
+        "docs": [
+            "sphinx==6.2.1",
+            "sphinx_toolbox==3.4.0",
+            "furo==2022.12.07",
+            "nbsphinx==0.9.1",
+        ],
+    },
     entry_points="""
         [console_scripts]
         cleanlab=cleanlab_studio.cli:main
     """,
 )
```

### Comparing `cleanlab-studio-1.0.4/tests/bench.py` & `cleanlab-studio-1.0.5/tests/bench.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/tests/datasets/test_csv_dataset.py` & `cleanlab-studio-1.0.5/tests/datasets/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/tests/datasets/test_excel_dataset.py` & `cleanlab-studio-1.0.5/tests/datasets/test_excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/tests/datasets/test_json_dataset.py` & `cleanlab-studio-1.0.5/tests/datasets/test_json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.4/tests/datasets/utils.py` & `cleanlab-studio-1.0.5/tests/datasets/utils.py`

 * *Files identical despite different names*


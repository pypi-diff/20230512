# Comparing `tmp/astrohack-0.1.1.tar.gz` & `tmp/astrohack-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrohack-0.1.1.tar", last modified: Fri May  5 20:40:13 2023, max compression
+gzip compressed data, was "astrohack-0.1.2.tar", last modified: Fri May 12 20:00:47 2023, max compression
```

## Comparing `astrohack-0.1.1.tar` & `astrohack-0.1.2.tar`

### file list

```diff
@@ -1,98 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.371443 astrohack-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 20:39:54.000000 astrohack-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 20:39:54.000000 astrohack-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-05 20:40:13.371443 astrohack-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-05 20:39:54.000000 astrohack-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:39:54.000000 astrohack-0.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-05 20:39:54.000000 astrohack-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 20:40:13.371443 astrohack-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.359443 astrohack-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.363443 astrohack-0.1.1/src/astrohack/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.363443 astrohack-0.1.1/src/astrohack/_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    30781 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_classes/antenna_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20815 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_classes/base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_classes/polygon_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_classes/ring_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_classes/telescope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.367443 astrohack-0.1.1/src/astrohack/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.367443 astrohack-0.1.1/src/astrohack/_utils/_dask_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_dask_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    21572 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_extract_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    14344 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.367443 astrohack-0.1.1/src/astrohack/_utils/_logger/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5462 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_logger/_astrohack_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    31185 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.367443 astrohack-0.1.1/src/astrohack/_utils/_parm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_parm_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2158 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_parm_utils/_check_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25433 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/gaussfitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/astrohack_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/combine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.359443 astrohack-0.1.1/src/astrohack/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.367443 astrohack-0.1.1/src/astrohack/data/.file_meta_data/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after.json
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.json
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before.json
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.367443 astrohack-0.1.1/src/astrohack/data/telescopes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.367443 astrohack-0.1.1/src/astrohack/data/telescopes/aca_7m.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.367443 astrohack-0.1.1/src/astrohack/data/telescopes/alma_da.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.367443 astrohack-0.1.1/src/astrohack/data/telescopes/alma_dv.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.367443 astrohack-0.1.1/src/astrohack/data/telescopes/alma_tp.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.367443 astrohack-0.1.1/src/astrohack/data/telescopes/vla.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/vla.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/vla.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/vla.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.371443 astrohack-0.1.1/src/astrohack/data/telescopes/vlba.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/vlba.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/vlba.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
--rw-r--r--   0 runner    (1001) docker     (123)    16694 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    19791 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/gdown_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/holog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/locit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.371443 astrohack-0.1.1/src/astrohack/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/visualization/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.363443 astrohack-0.1.1/src/astrohack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-05 20:40:13.000000 astrohack-0.1.1/src/astrohack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-05 20:40:13.000000 astrohack-0.1.1/src/astrohack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 20:40:13.000000 astrohack-0.1.1/src/astrohack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-05 20:40:13.000000 astrohack-0.1.1/src/astrohack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 20:40:13.000000 astrohack-0.1.1/src/astrohack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.371443 astrohack-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-05-05 20:39:54.000000 astrohack-0.1.1/tests/test_class_antenna_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    19937 2023-05-05 20:39:54.000000 astrohack-0.1.1/tests/test_class_base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-05-05 20:39:54.000000 astrohack-0.1.1/tests/test_class_ring_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-05 20:39:54.000000 astrohack-0.1.1/tests/test_class_telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.466786 astrohack-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-12 20:00:28.000000 astrohack-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 20:00:28.000000 astrohack-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-12 20:00:47.466786 astrohack-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-12 20:00:28.000000 astrohack-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:28.000000 astrohack-0.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-12 20:00:28.000000 astrohack-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 20:00:47.470786 astrohack-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.454786 astrohack-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.458786 astrohack-0.1.2/src/astrohack/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.458786 astrohack-0.1.2/src/astrohack/_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    30692 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_classes/antenna_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20815 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_classes/base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_classes/polygon_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_classes/ring_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_classes/telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.462787 astrohack-0.1.2/src/astrohack/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.462787 astrohack-0.1.2/src/astrohack/_utils/_dask_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_dask_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21553 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_extract_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_gaussfitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15449 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.462787 astrohack-0.1.2/src/astrohack/_utils/_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5462 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_logger/_astrohack_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31185 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.462787 astrohack-0.1.2/src/astrohack/_utils/_parm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_parm_utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2158 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_parm_utils/_check_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/_utils/_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/astrohack_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/combine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.454786 astrohack-0.1.2/src/astrohack/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.462787 astrohack-0.1.2/src/astrohack/data/.file_meta_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.json
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before.json
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed.json
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.462787 astrohack-0.1.2/src/astrohack/data/telescopes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.466786 astrohack-0.1.2/src/astrohack/data/telescopes/aca_7m.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.466786 astrohack-0.1.2/src/astrohack/data/telescopes/alma_da.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.466786 astrohack-0.1.2/src/astrohack/data/telescopes/alma_dv.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.466786 astrohack-0.1.2/src/astrohack/data/telescopes/alma_tp.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.466786 astrohack-0.1.2/src/astrohack/data/telescopes/vla.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/vla.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/vla.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/vla.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.466786 astrohack-0.1.2/src/astrohack/data/telescopes/vlba.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/vlba.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/vlba.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
+-rw-r--r--   0 runner    (1001) docker     (123)    16694 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20249 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/gdown_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11291 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/locit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.466786 astrohack-0.1.2/src/astrohack/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-12 20:00:28.000000 astrohack-0.1.2/src/astrohack/visualization/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.458786 astrohack-0.1.2/src/astrohack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-12 20:00:47.000000 astrohack-0.1.2/src/astrohack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-12 20:00:47.000000 astrohack-0.1.2/src/astrohack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:00:47.000000 astrohack-0.1.2/src/astrohack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-12 20:00:47.000000 astrohack-0.1.2/src/astrohack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-12 20:00:47.000000 astrohack-0.1.2/src/astrohack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:00:47.466786 astrohack-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-05-12 20:00:28.000000 astrohack-0.1.2/tests/test_class_antenna_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19937 2023-05-12 20:00:28.000000 astrohack-0.1.2/tests/test_class_base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-05-12 20:00:28.000000 astrohack-0.1.2/tests/test_class_ring_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-12 20:00:28.000000 astrohack-0.1.2/tests/test_class_telescope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-05-12 20:00:28.000000 astrohack-0.1.2/tests/test_stakeholder.py
```

### Comparing `astrohack-0.1.1/LICENSE` & `astrohack-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/PKG-INFO` & `astrohack-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.1.1
+Version: 0.1.2
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `astrohack-0.1.1/README.md` & `astrohack-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/pyproject.toml` & `astrohack-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "astrohack"
-version = "0.1.1"
+version = "0.1.2"
 description = "Holography Antenna Commissioning Kit"
 authors = [
     {name = "Jan-Willem Steeb", email="jsteeb@nrao.edu"},
     {name = "Joshua Hoskins", email="jhoskins@nrao.edu"}, 
     {name = "Victor de Souza Magalhaes", email="vdesouza@nrao.edu"}
 ]
 license = {file = "LICENSE.txt"}
@@ -14,15 +14,15 @@
 dependencies = [
 'astropy==5.2.1',
 'click==8.1.3',
 'dask==2023.3.2',
 'dask_jobqueue==0.8.1',
 'distributed==2023.3.2',
 'gdown==4.7.1',
-'matplotlib==3.6.3',
+'matplotlib==3.7.1',
 'memory_profiler==0.61.0',
 'numba==0.56.3',
 'numpy==1.22.4',
 'param==1.13.0',
 'plotly==5.14.0',
 'prettytable==3.6.0',
 'psutil==5.9.4',
```

### Comparing `astrohack-0.1.1/src/astrohack/_classes/antenna_surface.py` & `astrohack-0.1.2/src/astrohack/_classes/antenna_surface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import numpy as np
 import xarray as xr
 from matplotlib import pyplot as plt
 from matplotlib import colormaps as cmaps
-from mpl_toolkits.axes_grid1 import make_axes_locatable
+
 from astrohack._classes.base_panel import panel_models, irigid
 from astrohack._classes.ring_panel import RingPanel
 from astrohack._utils._constants import *
 from astrohack._utils._conversion import _convert_to_db
 from astrohack._utils._conversion import _convert_unit
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
-from astrohack._utils._utils import _add_prefix
+from astrohack._utils._tools import _add_prefix, _well_positioned_colorbar
 
 lnbr = "\n"
 figsize = [5, 4]
 
 
 class AntennaSurface:
     def __init__(self, inputxds, telescope, cutoff=None, pmodel=None, crop=False, panel_margins=None, reread=False):
@@ -178,15 +178,15 @@
         Provide the correct panel label for VLA style panels
         Args:
             iring: Number of the ring the panel is in
             ipanel: Number of the panel in that ring clockwise from the top
         Returns:
             The proper label for the panel at iring, ipanel
         """
-        return '{0:d}-{1:2d}'.format(iring+1, ipanel+1)
+        return '{0:d}-{1:d}'.format(iring+1, ipanel+1)
 
     def _alma_panel_labeling(self, iring, ipanel):
         """
         Provide the correct panel label for ALMA style panels, which is more complicated than VLA panels due to the
         implementation of panel sectors
         Args:
             iring: Number of the ring the panel is in
@@ -537,27 +537,28 @@
 
     def _plot_map(self, filename, data, title, vmin, vmax, unit, screws=False, colormap=None, figuresize=None, dpi=300,
                   colorbar=True):
         if colormap is None:
             colormap = 'viridis'
         if figuresize is None:
             figuresize = figsize
-        fig, ax = plt.subplots(1, 1, figsize=figuresize)
+        if figuresize is None or figuresize == 'None':
+            fig, ax = plt.subplots(1, 1, figsize=figsize)
+        else:
+            fig, ax = plt.subplots(1, 1, figsize=figuresize)
         ax.set_title(title)
         # set the limits of the plot to the limits of the data
         xmin = np.min(self.u_axis)
         xmax = np.max(self.u_axis)
         ymin = np.min(self.v_axis)
         ymax = np.max(self.v_axis)
         im = ax.imshow(data, cmap=colormap, interpolation="nearest", extent=[xmin, xmax, ymin, ymax],
                        vmin=vmin, vmax=vmax,)
         if colorbar:
-            divider = make_axes_locatable(ax)
-            cax = divider.append_axes("right", size="5%", pad=0.05)
-            fig.colorbar(im, label="Z Scale [" + unit + "]", cax=cax)
+            _well_positioned_colorbar(ax, fig, im, "Z Scale [" + unit + "]")
         ax.set_xlabel("X axis [m]")
         ax.set_ylabel("Y axis [m]")
         for panel in self.panels:
             panel.plot(ax, screws=screws)
         fig.tight_layout()
         plt.savefig(filename, dpi=dpi)
         plt.close()
@@ -594,18 +595,16 @@
         # set the limits of the plot to the limits of the data
         xmin = np.min(self.u_axis)
         xmax = np.max(self.u_axis)
         ymin = np.min(self.v_axis)
         ymax = np.max(self.v_axis)
         im = ax.imshow(np.full_like(self.deviation, fill_value=np.nan), cmap=cmap, interpolation="nearest",
                        extent=[xmin, xmax, ymin, ymax], vmin=vmin, vmax=vmax)
-        divider = make_axes_locatable(ax)
-        cax = divider.append_axes("right", size="5%", pad=0.05)
-        colorbar = fig.colorbar(im, label="Screw adjustments [" + unit + "]", cax=cax)
-        if threshold>0:
+        colorbar = _well_positioned_colorbar(ax, fig, im, "Screw adjustments [" + unit + "]")
+        if threshold > 0:
             line = threshold
             while line < vmax:
                 colorbar.ax.axhline(y=line, color='black', linestyle='-', lw=0.2)
                 colorbar.ax.axhline(y=-line, color='black', linestyle='-', lw=0.2)
                 line += threshold
         ax.set_xlabel("X axis [m]")
         ax.set_ylabel("Y axis [m]")
@@ -637,20 +636,20 @@
     def export_screws(self, filename, unit="mm"):
         """
         Export screw adjustments for all panels onto an ASCII file
         Args:
             filename: ASCII file name/path
             unit: unit for panel screw adjustments ['mm','miliinches']
         """
-        outfile = "Screw adjustments for {0:s} {1:s} antenna\n".format(self.telescope.name, self.antenna_name)
-        outfile += "Adjustments are in " + unit + 2*lnbr
-        outfile += "Lower means away from subreflector" + lnbr
-        outfile += "Raise means toward the subreflector" + lnbr
-        outfile += "LOWER the panel if the number is POSITIVE" + lnbr
-        outfile += "RAISE the panel if the number is NEGATIVE" + lnbr
+        outfile =  "# Screw adjustments for {0:s} {1:s} antenna\n".format(self.telescope.name, self.antenna_name)
+        outfile += "# Adjustments are in " + unit + 2*lnbr
+        outfile += "# Lower means away from subreflector" + lnbr
+        outfile += "# Raise means toward the subreflector" + lnbr
+        outfile += "# LOWER the panel if the number is POSITIVE" + lnbr
+        outfile += "# RAISE the panel if the number is NEGATIVE" + lnbr
         outfile += 2 * lnbr
         outfile += "{0:16s}".format('Panel')
         nscrews = len(self.telescope.screw_description)
         for screw in self.telescope.screw_description:
             outfile += "{0:11s}".format(screw)
         outfile += lnbr
         fac = _convert_unit('m', unit, 'length')
```

### Comparing `astrohack-0.1.1/src/astrohack/_classes/base_panel.py` & `astrohack-0.1.2/src/astrohack/_classes/base_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/_classes/polygon_panel.py` & `astrohack-0.1.2/src/astrohack/_classes/polygon_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/_classes/ring_panel.py` & `astrohack-0.1.2/src/astrohack/_classes/ring_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/_classes/telescope.py` & `astrohack-0.1.2/src/astrohack/_classes/telescope.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/_utils/_algorithms.py` & `astrohack-0.1.2/src/astrohack/_utils/_algorithms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/_utils/_combine.py` & `astrohack-0.1.2/src/astrohack/_utils/_combine.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/_utils/_constants.py` & `astrohack-0.1.2/src/astrohack/_utils/_constants.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/_utils/_conversion.py` & `astrohack-0.1.2/src/astrohack/_utils/_conversion.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py` & `astrohack-0.1.2/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py` & `astrohack-0.1.2/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/_utils/_dio.py` & `astrohack-0.1.2/src/astrohack/_utils/_dio.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import numpy as np
+
 from astrohack._utils._io import _load_image_xds
 from prettytable import PrettyTable
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._io import _read_meta_data
 from astrohack._utils._io import _load_holog_file
 from astrohack._utils._io import _load_image_file
 from astrohack._utils._io import _load_panel_file
@@ -62,21 +63,22 @@
 
         if os.path.isdir(file_path):
             logger.info("Found {stem}.point.zarr directory ...".format(stem=file_stem))
             
             self._point_path = file_path
             self.point = AstrohackPointFile(file_path)
 
+
 class AstrohackImageFile(dict):
     """
         Data class for holography image data.
     """
     def __init__(self, file):
         super().__init__()
-
+        self._meta_data = None
         self.file = file
         self._open = False
 
     def __getitem__(self, key):
         return super().__getitem__(key)
     
     def __setitem__(self, key, value):
@@ -91,15 +93,17 @@
             file (str, optional): Path to holography file. Defaults to None.
         Returns:
             bool: bool describing whether the file was opened properly
         """
         logger = _get_astrohack_logger()
         if file is None:
             file = self.file
-        
+
+        self._meta_data = _read_meta_data(file, 'image')
+
         try:
             _load_image_file(file, image_dict=self)
 
             self._open = True
 
         except Exception as e:
             logger.error("[AstroHackImageFile.open()]: {}".format(e))
@@ -108,23 +112,27 @@
         return self._open
 
     def summary(self):
         """
            Prints summary table of holog image file. 
         """
 
+        print("Atributes:")
+        for key in self._meta_data.keys():
+            print(f'{key:26s}= {self._meta_data[key]}')
+
         table = PrettyTable()
         table.field_names = ["antenna", "ddi"]
         table.align = "l"
         
         for ant in self.keys():
             table.add_row([ant, list(self[ant].keys())])
-        
-        print(table)
 
+        print('\nContents:')
+        print(table)
 
     def select(self, ant=None, ddi=None, polar=False):
         """Select data on the basis of ddi, scan, ant. This is a convenience function.
         Args:
             ddi (int, optional): Data description ID. Defaults to None.
             ant (int, optional): Antenna ID. Defaults to None.
         Returns:
@@ -137,26 +145,26 @@
             return self
         else:
             if polar:
                 return self[ant][ddi].apply(np.absolute), self[ant][ddi].apply(np.angle, deg=True)
 
             return self[ant][ddi]
 
+
 class AstrohackHologFile(dict):
     """
         Data Class to interact ith holography imaging data.
     """
     def __init__(self, file):
         super().__init__()
         
         self.file = file
         self._meta_data = None
         self._open = False
 
-
     def __getitem__(self, key):
         return super().__getitem__(key)
     
     def __setitem__(self, key, value):
         return super().__setitem__(key, value)
 
     def is_open(self):
@@ -171,15 +179,15 @@
             bool: bool describing whether the file was opened properly
         """
         logger = _get_astrohack_logger()
 
         if file is None:
             file = self.file
 
-        self._meta_data = _read_meta_data(holog_file=file)
+        self._meta_data = _read_meta_data(file, 'holog')
 
         try:
             _load_holog_file(holog_file=file, dask_load=dask_load, load_pnt_dict=False, holog_dict=self)
             self._open = True
 
         except Exception as e:
             logger.error("[AstrohackHologFile]: {}".format(e))
@@ -187,23 +195,29 @@
         
         return self._open
 
     def summary(self):
         """
             Prints summary table of holog file.
         """
-
+        print("Atributes:")
+        for key in self._meta_data.keys():
+            if key == 'n_pix':
+                n_side = int(np.sqrt(self._meta_data[key]))
+                print(f'{key:26s}= {n_side:d} x {n_side:d}')
+            else:
+                print(f'{key:26s}= {self._meta_data[key]}')
         table = PrettyTable()
         table.field_names = ["ddi", "map", "antenna"]
         table.align = "l"
         
         for ddi in self.keys():
             for scan in self[ddi].keys():
                 table.add_row([ddi, scan, list(self[ddi][scan].keys())])
-        
+        print('\nContents:')
         print(table)
 
     def select(self, ddi=None, scan=None, ant=None):
         """ Select data on the basis of ddi, scan, ant. This is a convenience function.
         Args:
             ddi (int, optional): Data description ID. Defaults to None.
             scan (int, optional): Scan number. Defaults to None.
@@ -224,23 +238,25 @@
         """ Holog file meta data.
         Returns:
             JSON: JSON file of holography meta data.
         """
 
         return self._meta_data
 
+
 class AstrohackPanelFile(dict):
     """
         Data class for holography panel data.
     """
     def __init__(self, file):
         super().__init__()
 
         self.file = file
         self._open = False
+        self._meta_data = None
 
     def __getitem__(self, key):
         return super().__getitem__(key)
     
     def __setitem__(self, key, value):
         return super().__setitem__(key, value)
         
@@ -254,38 +270,43 @@
         Returns:
             bool: bool describing whether the file was opened properly
         """
         logger = _get_astrohack_logger()
 
         if file is None:
             file = self.file
-        
+
+        self._meta_data = _read_meta_data(file, 'panel')
+
         try:
             _load_panel_file(file, panel_dict=self)
-
             self._open = True
-
         except Exception as e:
             logger.error("[AstroHackPanelFile.open()]: {}".format(e))
             self._open = False
 
         return self._open
 
     def summary(self):
         """
            Prints summary table of panel image file.
         """
 
+        print("Atributes:")
+        for key in self._meta_data.keys():
+            print(f'{key:26s}= {self._meta_data[key]}')
+
         table = PrettyTable()
         table.field_names = ["antenna", "ddi"]
         table.align = "l"
         
         for ant in self.keys():
             table.add_row([ant, list(self[ant].keys())])
-        
+
+        print('\nContents:')
         print(table)
 
     def get_antenna(self, antenna, ddi):
         """
         Return an AntennaSurface object for interaction
         Args:
             antenna: Which antenna in to be used
@@ -306,15 +327,14 @@
     def __init__(self, file):
         super().__init__()
         
         self.file = file
         self._meta_data = None
         self._open = False
 
-
     def __getitem__(self, key):
         return super().__getitem__(key)
     
     def __setitem__(self, key, value):
         return super().__setitem__(key, value)
 
     def is_open(self):
@@ -329,30 +349,35 @@
             bool: bool describing whether the file was opened properly
         """
         logger = _get_astrohack_logger()
 
         if file is None:
             file = self.file
 
+        self._meta_data = _read_meta_data(file, 'point')
         try:
             _load_point_file(file=file, dask_load=dask_load, pnt_dict=self)
             self._open = True
 
         except Exception as e:
             logger.error("[AstrohackPointFile]: {}".format(e))
             self._open = False
         
         return self._open
 
     def summary(self):
         """
             Prints summary table of pointing file.
         """
+        print("Atributes:")
+        for key in self._meta_data.keys():
+            print(f'{key:26s}= {self._meta_data[key]}')
 
         table = PrettyTable()
         table.field_names = ["antenna"]
         table.align = "l"
         
         for ant in self.keys():
-            table.add_row(ant)
-        
+            table.add_row([ant])
+
+        print('\nContents:')
         print(table)
```

### Comparing `astrohack-0.1.1/src/astrohack/_utils/_extract_holog.py` & `astrohack-0.1.2/src/astrohack/_utils/_extract_holog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 import os
 import json
-import zarr
-import copy
 import numpy as np
 import xarray as xr
 import astropy
-from astropy.io import fits
-from scipy import spatial
 from numba import njit
 from numba.core import types
-from numba.typed import Dict
-import copy
 
 from casacore import tables as ctables
 from astrohack._utils._imaging import _calculate_parallactic_angle_chunk
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
-
+from astrohack._utils._io import _write_meta_data
 from astrohack._utils._algorithms import _get_grid_parms
 
 from astrohack._utils._io import _load_point_file
 
+
 def _extract_holog_chunk(extract_holog_params):
     """Perform data query on holography data chunk and get unique time and state_ids/
 
     Args:
         ms_name (str): Measurementset name
         data_col (str): Data column to extract.
         ddi (int): Data description id
@@ -136,15 +131,16 @@
     )
 
     logger.info(
         "Finished extracting holography chunk for ddi: {ddi} holog_map_key: {holog_map_key}".format(
             ddi=ddi, holog_map_key=holog_map_key
         )
     )
-    
+
+
 @njit(cache=False, nogil=True)
 def _extract_holog_chunk_jit(
     vis_data,
     weight,
     ant1,
     ant2,
     time_vis_row,
@@ -254,15 +250,14 @@
 
         if sum_of_sum_weight == 0:
             flagged_mapping_antennas.append(map_ant_id)
 
     return vis_map_dict, sum_weight_map_dict, flagged_mapping_antennas
 
 
-
 def _get_time_samples(time_vis):
     """Sample three values for time vis and cooresponding indicies. Values are sammpled as (first, middle, last)
 
     Args:
         time_vis (numpy.ndarray): a list of visibility times
 
     Returns:
@@ -385,14 +380,15 @@
 
         else:
             logger.warning(
                 "[FLAGGED DATA] mapping antenna index {index}".format(index=ant_names[map_ant_index]
                 )
             )
 
+
 def _create_holog_obs_dict(pnt_dict,baseline_average_distance,ant_names,ant_pos,ant_names_main):
     '''
     Generate holog_obs_dict.
     '''
 
     logger = _get_astrohack_logger()
     mapping_scans_dict = {}
@@ -454,15 +450,14 @@
                     holog_obs_dict[ddi][map_id]['ant'][map_ant_key] = np.array(list(ref_ant_set))
                 else:
                     del holog_obs_dict[ddi][map_id]['ant'][map_ant_key] #Don't want mapping antennas with no reference antennas.
                     logger.warning('DDI ' + str(ddi) + ' and mapping antenna ' + str(map_ant_key) + ' has no reference antennas.')
                      
     return holog_obs_dict
 
-    
 
 def _check_if_array_in_dict(array_dict,array):
     
     for key,val in array_dict.items():
         if np.array_equiv(val,array):
             return key
             
@@ -491,16 +486,15 @@
             pnt_ant_dict[antenna]
             .interp(time=time_vis, method="nearest")
         )
 
     return pnt_map_dict
 
 
-
-def _create_holog_meta_data(holog_file, holog_dict, holog_params):
+def _create_holog_meta_data(holog_file, holog_dict, input_params):
     """Save holog file meta information to json file with the transformation
         of the ordering (ddi, holog_map, ant) --> (ant, ddi, holog_map).
 
     Args:
         holog_name (str): holog file name.
         holog_dict (dict): Dictionary containing msdx data.
     """
@@ -523,42 +517,35 @@
                                 ant_holog_dict[ant][ddi] = {map:{}}
                     
                             ant_holog_dict[ant][ddi][map] = xds.to_dict(data=False)
                             cell_sizes.append(xds.attrs["grid_parms"]["cell_size"])
                             n_pixs.append(xds.attrs["grid_parms"]["n_pix"])
                             telescope_names.append(xds.attrs['telescope_name'])
 
-
     if not (len(set(cell_sizes)) == 1):
         logger.error('Cell size not consistant: ' + str(cell_sizes))
         raise
         
     if not (len(set(n_pixs)) == 1):
         logger.error('Number of pixels not consistant: ' + str(n_pixs))
         raise
         
     if not (len(set(telescope_names)) == 1):
         logger.error('Telescope name not consistant: ' + str(telescope_names))
         raise
-        
-    meta_data = {'cell_size':cell_sizes[0],'n_pix':n_pixs[0],'telescope_name':telescope_names[0]}
-
-    output_attr_file = "{name}/{ext}".format(name=holog_file, ext=".holog_attr")
-
-    try:
-        with open(output_attr_file, "w") as json_file:
-            json.dump(meta_data, json_file)
-
-    except Exception as error:
-        logger.error("[_create_holog_meta_data] {error}".format(error=error))
-    
-
-    
     output_meta_file = "{name}/{ext}".format(name=holog_file, ext=".holog_json")
-    
     try:
         with open(output_meta_file, "w") as json_file:
             json.dump(ant_holog_dict, json_file)
 
     except Exception as error:
         logger.error("[_create_holog_meta_data] {error}".format(error=error))
 
+    meta_data = {'cell_size': cell_sizes[0],
+                 'n_pix': n_pixs[0],
+                 'telescope_name': telescope_names[0]}
+    meta_data.update(input_params)
+    holog_attr_file = "{name}/{ext}".format(name=holog_file, ext=".holog_attr")
+    _write_meta_data('extract_holog', holog_attr_file, meta_data)
+    point_attr_file = "{name}/{ext}".format(name=input_params['point_name'], ext=".point_attr")
+    _write_meta_data('extract_holog', point_attr_file, input_params)
+
```

### Comparing `astrohack-0.1.1/src/astrohack/_utils/_extract_point.py` & `astrohack-0.1.2/src/astrohack/_utils/_extract_point.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/_utils/_holog.py` & `astrohack-0.1.2/src/astrohack/_utils/_holog.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,18 @@
-import os
-import dask
-import json
 import scipy
-
+import json
 import numpy as np
 import xarray as xr
 
 from scipy.interpolate import griddata
-from casacore import tables as ctables
 
 from astrohack._classes.telescope import Telescope
 
 from astrohack._utils._io import _load_holog_file
-from astrohack._utils._io import _read_meta_data
-from astrohack._utils._io import _load_point_file
+from astrohack._utils._io import _read_meta_data, _write_meta_data
 
 from astrohack._utils._panel import _phase_fitting_block
 
 from astrohack._utils._algorithms import _chunked_average
 from astrohack._utils._algorithms import _find_peak_beam_value
 from astrohack._utils._algorithms import _find_nearest
 from astrohack._utils._algorithms import _calc_coords
@@ -26,15 +21,14 @@
 
 from astrohack._utils._imaging import _parallactic_derotation
 from astrohack._utils._imaging import _mask_circular_disk
 from astrohack._utils._imaging import _calculate_aperture_pattern
 
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 
-from numba import njit
 
 def _holog_chunk(holog_chunk_params):
     """ Process chunk holography data along the antenna axis. Works with holography file to properly grid , normalize, average and correct data
         and returns the aperture pattern.
 
     Args:
         holog_chunk_params (dict): Dictionary containing holography parameters.
@@ -48,15 +42,15 @@
         holog_chunk_params["holog_file"],
         dask_load=False,
         load_pnt_dict=False,
         ant_id=holog_chunk_params["ant_id"],
         ddi_id=holog_chunk_params["ddi_id"]
     )
 
-    meta_data = _read_meta_data(holog_chunk_params["holog_file"])
+    meta_data = _read_meta_data(holog_chunk_params["holog_file"], 'holog')
 
     # Calculate lm coordinates
     l, m = _calc_coords(holog_chunk_params["grid_size"], holog_chunk_params["cell_size"])
     grid_l, grid_m = list(map(np.transpose, np.meshgrid(l, m)))
     
     to_stokes = holog_chunk_params["to_stokes"]
 
@@ -311,7 +305,17 @@
 
     cf_chan_map = np.zeros((n_chan,), dtype=int)
     for i in range(n_chan):
         cf_chan_map[i], _ = _find_nearest(pb_freq, freq_chan[i])
 
     return cf_chan_map, pb_freq
 
+
+def _create_image_meta_data(image_file, input_params):
+    """
+    Save image meta data to a json file
+    Args:
+        image_file: image file
+        input_params: holog input parameter dictionaire
+    """
+    output_attr_file = "{name}/{ext}".format(name=image_file, ext=".image_attr")
+    _write_meta_data('holog', output_attr_file, input_params)
```

### Comparing `astrohack-0.1.1/src/astrohack/_utils/_imaging.py` & `astrohack-0.1.2/src/astrohack/_utils/_imaging.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/_utils/_io.py` & `astrohack-0.1.2/src/astrohack/_utils/_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 import os
 import json
 import zarr
 import copy
 import numpy as np
 import xarray as xr
-import astropy
+
 from astropy.io import fits
-from numba import njit
-from numba.core import types
-from numba.typed import Dict
-
-from casacore import tables as ctables
-from astrohack._utils._imaging import _calculate_parallactic_angle_chunk
-from astrohack._utils._conversion import convert_dict_from_numba
+from astrohack import __version__ as code_version
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
+from astrohack._utils._tools import _numpy_to_json
 
 DIMENSION_KEY = "_ARRAY_DIMENSIONS"
 
 
 def check_if_file_exists(file):
     logger = _get_astrohack_logger()
 
@@ -299,35 +294,69 @@
             return xr.open_zarr(image_path)
         else:
             return _open_no_dask_zarr(image_path)
     else:
         raise FileNotFoundError("Image file: {} not found".format(image_path))
 
 
-def _read_meta_data(holog_file):
+def _read_meta_data(file_name, file_type):
     """Reads dimensional data from holog meta file.
 
     Args:
-        holog_file (str): holog file name.
+        file_name (str): astorhack file name.
+        file_type (str): astrohack file type
 
     Returns:
         dict: dictionary containing dimension data.
     """
     logger = _get_astrohack_logger()
     try:
-        with open("{name}/{file}".format(name=holog_file, file="/.holog_attr")) as json_file:
+        with open(f'{file_name}/.{file_type}_attr') as json_file:
             json_dict = json.load(json_file)
 
     except Exception as error:
         logger.error(str(error))
         raise
 
     return json_dict
 
 
+def _write_meta_data(origin, file_name, input_dict):
+    """
+    Creates a metadata dictionary that is compatible with JSON and writes it to a file
+    Args:
+        origin: Which function created the mds
+        file_name: Output json file name
+        input_dict: Dictionary to be included in the metadata
+    """
+    logger = _get_astrohack_logger()
+    metadata = {'version': code_version,
+                'origin': origin}
+    for key in input_dict.keys():
+        if type(input_dict[key]) == np.ndarray:
+            try:
+                for item in range(len(input_dict[key])):
+                    newkey = f'{key}_{item}'
+                    metadata[newkey] = _numpy_to_json(input_dict[key][item])
+            except TypeError:
+                if len(input_dict['grid_size'].shape) == 0:
+                    metadata[key] = "None"
+                else:
+                    metadata[key] = input_dict[key]
+        elif input_dict[key] is None:
+            metadata[key] = "None"
+        else:
+            metadata[key] = input_dict[key]
+    try:
+        with open(file_name, "w") as json_file:
+            json.dump(metadata, json_file)
+    except Exception as error:
+        logger.error("[_write_meta_data] {error}".format(error=error))
+
+
 def _read_data_from_holog_json(holog_file, holog_dict, ant_id, ddi_id=None):
     """Read holog file meta data and extract antenna based xds information for each (ddi, holog_map)
 
     Args:
         holog_file (str): holog file name.
         holog_dict (dict): holog file dictionary containing msxds data.
         ant_id (int): Antenna id
@@ -432,15 +461,14 @@
                     pnt_dict[ant] = xr.open_zarr(os.path.join(file, ant))
                 else:
                     pnt_dict[ant] = _open_no_dask_zarr(os.path.join(file, ant))
 
     return pnt_dict
 
 
-
 def _get_attrs(zarr_obj):
     """Get attributes of zarr obj (groups or arrays)
 
     Args:
         zarr_obj (zarr): a zarr_group object
 
     Returns:
```

### Comparing `astrohack-0.1.1/src/astrohack/_utils/_logger/_astrohack_logger.py` & `astrohack-0.1.2/src/astrohack/_utils/_logger/_astrohack_logger.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/_utils/_panel.py` & `astrohack-0.1.2/src/astrohack/_utils/_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/_utils/_parm_utils/_check_logger_parms.py` & `astrohack-0.1.2/src/astrohack/_utils/_parm_utils/_check_logger_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/_utils/_parm_utils/_check_parms.py` & `astrohack-0.1.2/src/astrohack/_utils/_parm_utils/_check_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/_utils/gaussfitter.py` & `astrohack-0.1.2/src/astrohack/_utils/_gaussfitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ===========
-gaussfitter
+_gaussfitter
 ===========
 .. codeauthor:: Adam Ginsburg <adam.g.ginsburg@gmail.com> 3/17/08
 
 Latest version available at <https://github.com/keflavich/gaussfitter>, where
 it was moved from google code on January 30, 2014
 
 """
```

### Comparing `astrohack-0.1.1/src/astrohack/astrohack_client.py` & `astrohack-0.1.2/src/astrohack/astrohack_client.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/combine.py` & `astrohack-0.1.2/src/astrohack/combine.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import dask
 import numpy as np
 
 from astrohack._utils._combine import _combine_chunk
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._parm_utils._check_parms import _check_parms
-from astrohack._utils._utils import _remove_suffix
-from astrohack._utils._io import check_if_file_will_be_overwritten, check_if_file_exists
+from astrohack._utils._tools import _remove_suffix
+from astrohack._utils._io import check_if_file_will_be_overwritten, check_if_file_exists, _write_meta_data
 from astrohack._utils._dio import AstrohackImageFile
 
 
 def combine_image_ddi(image_name, combine_name=None, ant_list=None, ddi_list=None, weighted=False, parallel=False,
                       overwrite=False):
     """Combine DDIs in a Holography image to increase SNR
 
@@ -48,14 +48,15 @@
             ⋮
             ant_n: …
         }
     """
     logger = _get_astrohack_logger()
 
     combine_params = _check_combine_parms(image_name, combine_name, ant_list, ddi_list, weighted, parallel,  overwrite)
+    input_params = combine_params.copy()
 
     check_if_file_exists(combine_params['image_file'])
     check_if_file_will_be_overwritten(combine_params['combine_file'], combine_params['overwrite'])
 
     if combine_params['ant_list'] == 'all':
         antennae = os.listdir(combine_params['image_file'])
     else:
@@ -70,14 +71,17 @@
             delayed_list.append(dask.delayed(_combine_chunk)(dask.delayed(combine_chunk_params)))
         else:
             _combine_chunk(combine_chunk_params)
 
     if parallel:
         dask.compute(delayed_list)
 
+    output_attr_file = "{name}/{ext}".format(name=combine_params['combine_file'], ext=".image_attr")
+    _write_meta_data('combine', output_attr_file, input_params)
+
     combine_mds = AstrohackImageFile(combine_chunk_params['combine_file'])
     combine_mds.open()
 
     return combine_mds
 
 
 def _check_combine_parms(image_name, combine_name, ant_list, ddi_list, weighted, parallel,  overwrite):
```

### Comparing `astrohack-0.1.1/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after.json` & `astrohack-0.1.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.json` & `astrohack-0.1.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before.json` & `astrohack-0.1.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed.json` & `astrohack-0.1.2/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs` & `astrohack-0.1.2/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata` & `astrohack-0.1.2/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/data/telescopes/alma_da.zarr/.zattrs` & `astrohack-0.1.2/src/astrohack/data/telescopes/alma_da.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata` & `astrohack-0.1.2/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs` & `astrohack-0.1.2/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata` & `astrohack-0.1.2/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs` & `astrohack-0.1.2/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata` & `astrohack-0.1.2/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/data/telescopes/vla.zarr/.zattrs` & `astrohack-0.1.2/src/astrohack/data/telescopes/vla.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/data/telescopes/vla.zarr/.zmetadata` & `astrohack-0.1.2/src/astrohack/data/telescopes/vla.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/data/telescopes/vlba.zarr/.zattrs` & `astrohack-0.1.2/src/astrohack/data/telescopes/vlba.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/data/telescopes/vlba.zarr/.zmetadata` & `astrohack-0.1.2/src/astrohack/data/telescopes/vlba.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/dio.py` & `astrohack-0.1.2/src/astrohack/dio.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from matplotlib import colormaps as cmaps
 
 from casacore import tables
 
 from astrohack._utils._constants import length_units, trigo_units, plot_types
 from astrohack._utils._parm_utils._check_parms import _check_parms
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
-from astrohack._utils._utils import _parm_to_list
+from astrohack._utils._tools import _parm_to_list
 
 from astrohack._utils._dio import AstrohackImageFile
 from astrohack._utils._dio import AstrohackHologFile
 from astrohack._utils._dio import AstrohackPanelFile
 from astrohack._utils._dio import AstrohackPointFile
 
 from astrohack._utils._panel import _plot_antenna_chunk
@@ -92,15 +92,15 @@
     for antenna in antennae:
         if 'ant' in antenna:
             ddis = _parm_to_list(parm_dict['ddi'], parm_dict['filename']+'/'+antenna)
             for ddi in ddis:
                 if 'ddi' in ddi:
                     export_name = parm_dict['destination']+f'/screws_{antenna}_{ddi}.'
                     surface = panel_mds.get_antenna(antenna, ddi)
-                    surface.export_screws(export_name+'txt', unit=unit)
+                    surface.export_screws(export_name+'csv', unit=unit)
                     if parm_dict['plot_map']:
                         surface.plot_screw_adjustments(export_name+'png', unit=unit, threshold=parm_dict['threshold'],
                                                        colormap=parm_dict['colormap'], figuresize=parm_dict['figuresize'],
                                                        dpi=parm_dict['dpi'])
 
 
 def plot_antenna(panel_mds_name, destination, ant_name=None, ddi=None, plot_type='deviation', plot_screws=False,
```

### Comparing `astrohack-0.1.1/src/astrohack/extract_holog.py` & `astrohack-0.1.2/src/astrohack/extract_holog.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import os
 import dask
 import sys
+import json
+import copy
 
 import xarray as xr
 import numpy as np
 import numbers
 
 from casacore import tables as ctables
 
@@ -18,22 +20,25 @@
 from astrohack._utils._extract_point import _extract_pointing
 
 from astrohack._utils._io import _load_point_file
 from astrohack._utils._io import _open_no_dask_zarr
 from astrohack._utils._io import _read_data_from_holog_json
 from astrohack._utils._io import _read_meta_data
 from astrohack._utils._io import _load_holog_file
-from astrohack._utils._io import  check_if_file_will_be_overwritten,check_if_file_exists
+from astrohack._utils._io import  check_if_file_will_be_overwritten, check_if_file_exists
+from astrohack._utils._io import _load_holog_file
 
 from astrohack._utils._extract_holog import _extract_holog_chunk
 
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._parm_utils._check_parms import _check_parms
-from astrohack._utils._utils import _remove_suffix
-from astrohack._utils._io import _load_holog_file
+
+from astrohack._utils._tools import _remove_suffix
+from astrohack._utils._tools import _jsonify
+from astrohack._utils._tools import _print_holog_obs_dict
 
 from astrohack._utils._dio import AstrohackHologFile
 
 def extract_holog(
     ms_name,
     holog_obs_dict=None,
     ddi_sel=None,
@@ -71,14 +76,17 @@
 
     :param parallel: Boolean for whether to process in parallel. Defaults to False
     :type parallel: bool, optional
     
     :param reuse_point_zarr: If true the point.zarr specified in point_name is reused.
     :type reuse_point_zarr: bool, optional
 
+    :param test_mode: Boolean for whether to writeholog dictionary to disk. This is solely for testing., defaults to False
+    :type overwrite: bool, optional
+
     :param overwrite: Boolean for whether to overwrite current holog.zarr and point.zarr files., defaults to False
     :type overwrite: bool, optional
 
     :return: Holography holog object.
     :rtype: AstrohackHologFile
 
     .. _Description:
@@ -151,14 +159,15 @@
                                 baseline_average_distance,
                                 holog_name,
                                 point_name,
                                 data_col,
                                 parallel,
                                 reuse_point_zarr,
                                 overwrite)
+    input_params = extract_holog_parms.copy()
     
     check_if_file_exists(extract_holog_parms['ms_name'])
     check_if_file_will_be_overwritten(extract_holog_parms['holog_name'],extract_holog_parms['overwrite'])
     check_if_file_will_be_overwritten(extract_holog_parms['point_name'],extract_holog_parms['overwrite'])
         
     ############# Exstract pointing infromation and save to point.zarr #############
     if extract_holog_parms["reuse_point_zarr"]:
@@ -230,16 +239,23 @@
                 holog_obs_dict_with_ddi['ddi_' + str(ddi_id)] = holog_obs_dict
         else:
             for ddi_id in ddi_sel:
                 holog_obs_dict_with_ddi['ddi_' + str(ddi_id)] = holog_obs_dict
         
         holog_obs_dict = holog_obs_dict_with_ddi
             
-    from pprint import pformat
-    logger.info("holog_obs_dict: \n%s", pformat(holog_obs_dict,indent=1,width=1))
+    _print_holog_obs_dict(holog_obs_dict)
+
+
+    outfile_obj = copy.deepcopy(holog_obs_dict)
+
+    _jsonify(outfile_obj)
+
+    with open(".holog_obs_dict.json", "w") as outfile:
+        json.dump(outfile_obj, outfile)
         
     ######## Get Scan and Subscan IDs ########
     # SDM Tables Short Description (https://drive.google.com/file/d/16a3g0GQxgcO7N_ZabfdtexQ8r2jRbYIS/view)
     # 2.54 ScanIntent (p. 150)
     # MAP ANTENNA SURFACE : Holography calibration scan
 
     # 2.61 SubscanIntent (p. 152)
@@ -383,15 +399,16 @@
 
     if parallel:
         dask.compute(delayed_list)    
 
     holog_dict = _load_holog_file(holog_file=extract_holog_parms["holog_name"], dask_load=True, load_pnt_dict=False)
 
     extract_holog_parms['telescope_name'] = telescope_name
-    _create_holog_meta_data(holog_file=extract_holog_parms['holog_name'], holog_dict=holog_dict, holog_params=extract_holog_parms)
+    _create_holog_meta_data(holog_file=extract_holog_parms['holog_name'], holog_dict=holog_dict,
+                            input_params=input_params)
     
     holog_mds = AstrohackHologFile(extract_holog_parms['holog_name'])
     holog_mds.open()
     
     return holog_mds
```

### Comparing `astrohack-0.1.1/src/astrohack/gdown_utils.py` & `astrohack-0.1.2/src/astrohack/gdown_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 from prettytable import PrettyTable
 from prettytable import DOUBLE_BORDER
 
 gdown_ids = {
     'ea25_cal_small_spw1_4_60_ea04_before.ms': '1-v1foZ4G-kHTOS2idylx-3S4snKgRHmM',
     'ea25_cal_small_spw1_4_60_ea04_after.ms': '1PmWvPA0rUtAfegVu9wOb4AGJXiQIp3Cp',
     'ea25_cal_small_spw1_4_60_ea04_before_fixed.ms': '1dV4e8FiVRdAw2NLNzSuPVvjwyqXPNXTf',
-    'ea25_cal_small_spw1_4_60_ea04_after_fixed.ms': '1Gn5GEJ3V43bl2vXxznHk6oXF5LtWOMzj'
+    'ea25_cal_small_spw1_4_60_ea04_after_fixed.ms': '1Gn5GEJ3V43bl2vXxznHk6oXF5LtWOMzj',
+    'ea25_cal_small_before_fixed.split.ms':'1oydlR7kA7F4n0i9KF9HgRc2jq1ziUslt',
+    'ea25_cal_small_after_fixed.split.ms':'1TATMxKTFYIEO-l9L3jdYj62lZ8TZex4T'
 }
 
 def check_download(name, folder, id):
     fullname = os.path.join(folder,name)
     if not os.path.exists(fullname):
         url = 'https://drive.google.com/u/0/uc?id='+id+'&export=download'
         gdown.download(url, fullname+'.zip')
```

### Comparing `astrohack-0.1.1/src/astrohack/holog.py` & `astrohack-0.1.2/src/astrohack/holog.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import os
 
 import dask
 import dask.distributed
 import numpy as np
 import numbers
 
-from astrohack._utils._holog import _holog_chunk
+from astrohack._utils._holog import _holog_chunk, _create_image_meta_data
 
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._parm_utils._check_parms import _check_parms
-from astrohack._utils._utils import _remove_suffix
+from astrohack._utils._tools import _remove_suffix
    
-from astrohack._utils._io import check_if_file_will_be_overwritten, check_if_file_exists
+from astrohack._utils._io import check_if_file_will_be_overwritten, check_if_file_exists, _read_meta_data
 from astrohack._utils._dio import AstrohackImageFile
 
 def holog(
     holog_name,
     grid_size=None,
     cell_size=None,
     image_name=None,
@@ -26,15 +26,16 @@
     chan_tolerance_factor=0.005,
     scan_average=True,
     ant_list=None,
     to_stokes=True,
     apply_mask=True,
     phase_fit=True,
     overwrite=False,
-    parallel=True):
+    parallel=True, 
+    ):
     """ Process holography data and derive aperture illumination pattern.
 
     :param holog_name: Name of holography .holog.zarr file to process.
     :type holog_name: str
 
     :param grid_size: Numpy array specifying the dimensions of the grid used in data gridding. If not specified grid_size is calculated using POINTING_OFFSET in pointing table.
     :type grid_size: numpy.ndarray, dtype int, optional
@@ -124,27 +125,23 @@
         scan_average,
         ant_list, 
         to_stokes, 
         apply_mask, 
         phase_fit,
         overwrite
     )
+    input_params = holog_params.copy()
     
     check_if_file_exists(holog_params['holog_file'])
     check_if_file_will_be_overwritten(holog_params['image_file'],holog_params['overwrite'])
 
     json_data = "/".join((holog_params['holog_file'], ".holog_json"))
-    meta_data = "/".join((holog_params['holog_file'], ".holog_attr"))
-    
     with open(json_data, "r") as json_file:
         holog_json = json.load(json_file)
-    
-    with open(meta_data, "r") as meta_file:
-        meta_data = json.load(meta_file)
-        image_name=None,
+    meta_data = _read_meta_data(holog_params['holog_file'], 'holog')
 
     if  holog_params['ant_list'] == 'all':
         holog_params['ant_list'] = list(holog_json.keys())
         
     logger.info('Mapping antennas ' + str(holog_params['ant_list']))
 
     
@@ -157,14 +154,22 @@
         holog_params["grid_size"] = grid_size
         
         logger.info("Cell size: " + str(cell_size) + " Grid size " + str(grid_size))
     else:
         holog_params["cell_size"] = cell_size
         holog_params["grid_size"] = grid_size
     
+    
+    json_data = {
+            "cell_size": list(map(float, cell_size)),
+            "grid_size": list(map(float, grid_size))
+    }
+
+    with open(".holog_diagnostic.json", "w") as out_file:
+        json.dump(json_data, out_file)
 
     
     holog_chunk_params =  holog_params
     delayed_list = []
     
     
     for ant_id in holog_chunk_params['ant_list']:
@@ -180,22 +185,23 @@
 
             else:
                 _holog_chunk(holog_chunk_params)
             
 
     if holog_chunk_params['parallel']:
         dask.compute(delayed_list)
+
+    _create_image_meta_data(holog_params['image_file'], input_params)
         
     image_mds = AstrohackImageFile(holog_chunk_params['image_file'])
     image_mds.open()
     
     return image_mds
 
 
-
 def _check_holog_parms(holog_name,grid_size,cell_size,image_name,
                       padding_factor,parallel,grid_interpolation_mode,
                       chan_average,chan_tolerance_factor,
                       scan_average,ant_list,to_stokes,apply_mask,phase_fit,overwrite):
 
     holog_params = {}
     holog_params["holog_file"] = holog_name
@@ -216,59 +222,41 @@
     
     #### Parameter Checking ####
     logger = _get_astrohack_logger()
     parms_passed = True
     
     parms_passed = parms_passed and _check_parms(holog_params, 'holog_file', [str],default=None)
 
-    parms_passed = parms_passed and _check_parms(holog_params, 'grid_size', [list,np.ndarray], list_acceptable_data_types=[np.int,np.int64], list_len=2, default='None',log_default_setting=False)
+    parms_passed = parms_passed and _check_parms(holog_params, 'grid_size', [list, np.ndarray], list_acceptable_data_types=[np.int64, np.int64], list_len=2, default='None',log_default_setting=False)
     if (isinstance(holog_params['grid_size'],str)) and (holog_params['grid_size'] == 'None'): holog_params['grid_size'] =  None
     holog_params['grid_size'] = np.array(holog_params['grid_size'])
 
     parms_passed = parms_passed and _check_parms(holog_params, 'cell_size', [list,np.ndarray], list_acceptable_data_types=[numbers.Number], list_len=2, default='None',log_default_setting=False)
     if (isinstance(holog_params['cell_size'],str)) and (holog_params['cell_size'] == 'None'): holog_params['cell_size'] =  None
     holog_params['cell_size'] = np.array(holog_params['cell_size'])
 
     
     base_name = _remove_suffix(holog_params['holog_file'],'.holog.zarr')
     parms_passed = parms_passed and _check_parms(holog_params,'image_file', [str],default=base_name+'.image.zarr')
-    
     parms_passed = parms_passed and _check_parms(holog_params, 'padding_factor', [int], default=50)
-  
-    
     parms_passed = parms_passed and _check_parms(holog_params, 'parallel', [bool],default=False)
-
-    
     parms_passed = parms_passed and _check_parms(holog_params,'grid_interpolation_mode', [str],acceptable_data=["nearest","linear","cubic"],default="nearest")
-   
-    
     parms_passed = parms_passed and _check_parms(holog_params, 'chan_average', [bool],default=True)
-
-    
     parms_passed = parms_passed and _check_parms(holog_params, 'chan_tolerance_factor', [float], acceptable_range=[0,1], default=0.005)
-   
-
     parms_passed = parms_passed and _check_parms(holog_params, 'scan_average', [bool],default=True)
-
     parms_passed = parms_passed and _check_parms(holog_params, 'ant_list', [list,np.ndarray], list_acceptable_data_types=[str], default='all')
- 
     parms_passed = parms_passed and _check_parms(holog_params, 'to_stokes', [bool],default=True)
-   
- 
+
     if isinstance(holog_params['phase_fit'],list) or isinstance(holog_params['phase_fit'],type(np.ndarray)):
         parms_passed = parms_passed and _check_parms(holog_params, 'phase_fit', [list,type(np.ndarray)], list_acceptable_data_types=[bool], list_len=5)
     else:
         parms_passed = parms_passed and _check_parms(holog_params, 'phase_fit', [bool], default=True)
-  
-   
+
     parms_passed = parms_passed and _check_parms(holog_params, 'apply_mask', [bool],default=True)
-    
     parms_passed = parms_passed and _check_parms(holog_params, 'overwrite', [bool],default=False)
 
     if not parms_passed:
         logger.error("extract_holog parameter checking failed.")
         raise Exception("extract_holog parameter checking failed.")
-    #### End Parameter Checking ####
-    
-    
+
     return holog_params
```

### Comparing `astrohack-0.1.1/src/astrohack/panel.py` & `astrohack-0.1.2/src/astrohack/panel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 import os
 import dask
 import shutil
 
 import numpy as np
-import xarray as xr
 
-from astrohack._classes.telescope import Telescope
 from astrohack._classes.base_panel import panel_models
-from astrohack._utils._io import _aips_holog_to_xds, check_if_file_will_be_overwritten, check_if_file_exists
-
+from astrohack._utils._io import _aips_holog_to_xds, check_if_file_will_be_overwritten, check_if_file_exists, _write_meta_data
 from astrohack._utils._panel import _panel_chunk
-
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._parm_utils._check_parms import _check_parms
-from astrohack._utils._utils import _remove_suffix
+from astrohack._utils._tools import _remove_suffix
 
 from astrohack._utils._dio import AstrohackPanelFile
 
 
 def panel(image_name, panel_name=None, cutoff=0.2, panel_model=None, panel_margins=0.2, parallel=False, sel_ddi=None, overwrite=False):
     """Analyze holography images to derive panel adjustments
 
@@ -92,14 +88,15 @@
 
     """
     
     logger = _get_astrohack_logger()
     
     panel_params = _check_panel_parms(image_name, panel_name, cutoff, panel_model, panel_margins, parallel, sel_ddi,
                                       overwrite)
+    input_params = panel_params.copy()
           
     check_if_file_exists(panel_params['image_name'])
     check_if_file_will_be_overwritten(panel_params['panel_name'], panel_params['overwrite'])
 
     if os.path.exists(panel_params['image_name']+'/.aips'):
         panel_params['origin'] = 'AIPS'
         _panel_chunk(panel_params)
@@ -128,21 +125,25 @@
                             _panel_chunk(panel_chunk_params)
                         count += 1
         if parallel:
             dask.compute(delayed_list)
 
         if count == 0:
             logger.warning("No data to process")
+            return None
         else:
             logger.info("Panel finished processing")
-            
+
+            output_attr_file = "{name}/{ext}".format(name=panel_chunk_params['panel_name'], ext=".panel_attr")
+            _write_meta_data('panel', output_attr_file, input_params)
             panel_mds = AstrohackPanelFile(panel_chunk_params['panel_name'])
             panel_mds.open()
             return panel_mds
 
+
 def aips_holog_to_astrohack(amp_image, dev_image, telescope_name, holog_name, overwrite=False):
     """
     Package AIPS HOLOG products in a .image.zarr file compatible with astrohack.panel.panel
 
     This function reads amplitude and deviation FITS files produced by AIPS's HOLOG task and transfers their data onto a
     .image.zarr file that can be read by panel.
     Most of the meta data can be inferred from the FITS headers, but it remains necessary to specify the telescope name
@@ -202,17 +203,15 @@
     base_name = _remove_suffix(panel_params['image_name'], '.image.zarr')
     base_name = _remove_suffix(base_name, '.combine.zarr')
     parms_passed = parms_passed and _check_parms(panel_params, 'panel_name', [str], default=base_name+'.panel.zarr')
     parms_passed = parms_passed and _check_parms(panel_params, 'cutoff', [float], acceptable_range=[0, 1], default=0.2)
     parms_passed = parms_passed and _check_parms(panel_params, 'panel_kind', [str], acceptable_data=panel_models, default="rigid")
     parms_passed = parms_passed and _check_parms(panel_params, 'panel_margins', [float], acceptable_range=[0, 0.5], default=0.2)
     parms_passed = parms_passed and _check_parms(panel_params, 'parallel', [bool], default=False)
-    parms_passed = parms_passed and _check_parms(panel_params, 'sel_ddi', [list, np.array], list_acceptable_data_types=[int, np.int], default='all')
+    parms_passed = parms_passed and _check_parms(panel_params, 'sel_ddi', [list, np.array], list_acceptable_data_types=[int, np.int64], default='all')
     parms_passed = parms_passed and _check_parms(panel_params, 'overwrite', [bool], default=False)
 
     if not parms_passed:
         logger.error("panel parameter checking failed.")
         raise Exception("panel parameter checking failed.")
     
-    return panel_params
-
-
+    return panel_params
```

### Comparing `astrohack-0.1.1/src/astrohack/profiling.py` & `astrohack-0.1.2/src/astrohack/profiling.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack/visualization/viewer.py` & `astrohack-0.1.2/src/astrohack/visualization/viewer.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/src/astrohack.egg-info/PKG-INFO` & `astrohack-0.1.2/src/astrohack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.1.1
+Version: 0.1.2
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `astrohack-0.1.1/src/astrohack.egg-info/SOURCES.txt` & `astrohack-0.1.2/src/astrohack.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -27,32 +27,34 @@
 src/astrohack/_utils/_algorithms.py
 src/astrohack/_utils/_combine.py
 src/astrohack/_utils/_constants.py
 src/astrohack/_utils/_conversion.py
 src/astrohack/_utils/_dio.py
 src/astrohack/_utils/_extract_holog.py
 src/astrohack/_utils/_extract_point.py
+src/astrohack/_utils/_gaussfitter.py
 src/astrohack/_utils/_holog.py
 src/astrohack/_utils/_imaging.py
 src/astrohack/_utils/_io.py
 src/astrohack/_utils/_panel.py
-src/astrohack/_utils/_utils.py
-src/astrohack/_utils/gaussfitter.py
+src/astrohack/_utils/_tools.py
 src/astrohack/_utils/_dask_plugins/__init__.py
 src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
 src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
 src/astrohack/_utils/_logger/__init__.py
 src/astrohack/_utils/_logger/_astrohack_logger.py
 src/astrohack/_utils/_parm_utils/__init__.py
 src/astrohack/_utils/_parm_utils/_check_logger_parms.py
 src/astrohack/_utils/_parm_utils/_check_parms.py
 src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after.json
 src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.json
+src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json
 src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before.json
 src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed.json
+src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json
 src/astrohack/data/telescopes/__init__.py
 src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
 src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
 src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
 src/astrohack/data/telescopes/alma_da.zarr/.zattrs
 src/astrohack/data/telescopes/alma_da.zarr/.zgroup
 src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
@@ -69,8 +71,9 @@
 src/astrohack/data/telescopes/vlba.zarr/.zgroup
 src/astrohack/data/telescopes/vlba.zarr/.zmetadata
 src/astrohack/visualization/__init__.py
 src/astrohack/visualization/viewer.py
 tests/test_class_antenna_surface.py
 tests/test_class_base_panel.py
 tests/test_class_ring_panel.py
-tests/test_class_telescope.py
+tests/test_class_telescope.py
+tests/test_stakeholder.py
```

### Comparing `astrohack-0.1.1/src/astrohack.egg-info/requires.txt` & `astrohack-0.1.2/src/astrohack.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 astropy==5.2.1
 click==8.1.3
 dask==2023.3.2
 dask_jobqueue==0.8.1
 distributed==2023.3.2
 gdown==4.7.1
-matplotlib==3.6.3
+matplotlib==3.7.1
 memory_profiler==0.61.0
 numba==0.56.3
 numpy==1.22.4
 param==1.13.0
 plotly==5.14.0
 prettytable==3.6.0
 psutil==5.9.4
```

### Comparing `astrohack-0.1.1/tests/test_class_antenna_surface.py` & `astrohack-0.1.2/tests/test_class_antenna_surface.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/tests/test_class_base_panel.py` & `astrohack-0.1.2/tests/test_class_base_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/tests/test_class_ring_panel.py` & `astrohack-0.1.2/tests/test_class_ring_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.1/tests/test_class_telescope.py` & `astrohack-0.1.2/tests/test_class_telescope.py`

 * *Files identical despite different names*


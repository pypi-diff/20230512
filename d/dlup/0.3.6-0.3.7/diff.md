# Comparing `tmp/dlup-0.3.6.tar.gz` & `tmp/dlup-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlup-0.3.6.tar", last modified: Sat Oct  1 13:16:41 2022, max compression
+gzip compressed data, was "dlup-0.3.7.tar", last modified: Sat Oct 22 10:26:03 2022, max compression
```

## Comparing `dlup-0.3.6.tar` & `dlup-0.3.7.tar`

### file list

```diff
@@ -1,91 +1,92 @@
-drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-01 13:16:41.255689 dlup-0.3.6/
--rw-r--r--   0 jteuwen    (501) staff       (20)     3579 2021-08-25 14:51:38.000000 dlup-0.3.6/CONTRIBUTING.rst
--rw-r--r--   0 jteuwen    (501) staff       (20)    11357 2021-08-25 14:51:38.000000 dlup-0.3.6/LICENSE
--rw-r--r--   0 jteuwen    (501) staff       (20)      226 2021-08-25 14:51:38.000000 dlup-0.3.6/MANIFEST.in
--rw-r--r--   0 jteuwen    (501) staff       (20)     2013 2022-10-01 13:16:41.255774 dlup-0.3.6/PKG-INFO
--rw-r--r--   0 jteuwen    (501) staff       (20)     1371 2022-09-19 11:44:11.000000 dlup-0.3.6/README.md
-drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-01 13:16:41.245071 dlup-0.3.6/dlup/
--rw-r--r--   0 jteuwen    (501) staff       (20)      390 2022-10-01 13:16:24.000000 dlup-0.3.6/dlup/__init__.py
--rw-r--r--   0 jteuwen    (501) staff       (20)      445 2022-09-19 11:44:11.000000 dlup-0.3.6/dlup/_exceptions.py
--rw-r--r--   0 jteuwen    (501) staff       (20)    12671 2022-10-01 13:16:04.000000 dlup-0.3.6/dlup/_image.py
--rw-r--r--   0 jteuwen    (501) staff       (20)     2722 2022-09-19 11:44:11.000000 dlup-0.3.6/dlup/_region.py
--rw-r--r--   0 jteuwen    (501) staff       (20)    26937 2022-10-01 13:14:00.000000 dlup-0.3.6/dlup/annotations.py
--rw-r--r--   0 jteuwen    (501) staff       (20)    10755 2022-09-19 11:44:11.000000 dlup-0.3.6/dlup/background.py
-drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-01 13:16:41.246370 dlup-0.3.6/dlup/cli/
--rw-r--r--   0 jteuwen    (501) staff       (20)      862 2022-01-22 12:00:51.000000 dlup-0.3.6/dlup/cli/__init__.py
--rw-r--r--   0 jteuwen    (501) staff       (20)     7630 2022-09-19 11:44:11.000000 dlup-0.3.6/dlup/cli/wsi.py
-drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-01 13:16:41.246999 dlup-0.3.6/dlup/data/
--rw-r--r--   0 jteuwen    (501) staff       (20)       49 2021-08-25 14:51:38.000000 dlup-0.3.6/dlup/data/__init__.py
--rw-r--r--   0 jteuwen    (501) staff       (20)    16579 2022-09-19 11:44:11.000000 dlup-0.3.6/dlup/data/dataset.py
-drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-01 13:16:41.247357 dlup-0.3.6/dlup/data/experimental/
--rw-r--r--   0 jteuwen    (501) staff       (20)       49 2022-09-19 11:44:11.000000 dlup-0.3.6/dlup/data/experimental/__init__.py
--rw-r--r--   0 jteuwen    (501) staff       (20)     5501 2022-09-19 11:44:11.000000 dlup-0.3.6/dlup/data/experimental/dataset.py
--rw-r--r--   0 jteuwen    (501) staff       (20)     7894 2022-10-01 13:14:00.000000 dlup-0.3.6/dlup/data/transforms.py
-drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-01 13:16:41.248185 dlup-0.3.6/dlup/experimental_backends/
--rw-r--r--   0 jteuwen    (501) staff       (20)     3921 2022-09-19 11:44:11.000000 dlup-0.3.6/dlup/experimental_backends/__init__.py
--rw-r--r--   0 jteuwen    (501) staff       (20)     5550 2022-09-19 11:44:11.000000 dlup-0.3.6/dlup/experimental_backends/common.py
--rw-r--r--   0 jteuwen    (501) staff       (20)     2192 2022-09-19 11:44:11.000000 dlup-0.3.6/dlup/experimental_backends/openslide_backend.py
--rw-r--r--   0 jteuwen    (501) staff       (20)     6201 2022-09-19 11:44:11.000000 dlup-0.3.6/dlup/experimental_backends/pyvips_backend.py
--rw-r--r--   0 jteuwen    (501) staff       (20)     4023 2022-09-19 11:44:11.000000 dlup-0.3.6/dlup/experimental_backends/tifffile_backend.py
--rw-r--r--   0 jteuwen    (501) staff       (20)     2602 2022-09-19 11:44:11.000000 dlup-0.3.6/dlup/logging.py
--rw-r--r--   0 jteuwen    (501) staff       (20)     5026 2022-09-19 11:44:11.000000 dlup-0.3.6/dlup/tiling.py
--rw-r--r--   0 jteuwen    (501) staff       (20)     1941 2021-11-04 11:38:08.000000 dlup-0.3.6/dlup/tools.py
--rw-r--r--   0 jteuwen    (501) staff       (20)      384 2022-09-29 20:11:24.000000 dlup-0.3.6/dlup/types.py
-drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-01 13:16:41.249297 dlup-0.3.6/dlup/utils/
--rw-r--r--   0 jteuwen    (501) staff       (20)      841 2022-09-19 11:44:11.000000 dlup-0.3.6/dlup/utils/__init__.py
--rw-r--r--   0 jteuwen    (501) staff       (20)      583 2022-09-19 11:44:11.000000 dlup-0.3.6/dlup/utils/image.py
--rw-r--r--   0 jteuwen    (501) staff       (20)      693 2022-09-19 11:44:11.000000 dlup-0.3.6/dlup/utils/imports.py
--rw-r--r--   0 jteuwen    (501) staff       (20)     1587 2022-09-19 11:44:11.000000 dlup-0.3.6/dlup/utils/pyvips_utils.py
--rw-r--r--   0 jteuwen    (501) staff       (20)     3889 2022-09-18 19:42:47.000000 dlup-0.3.6/dlup/utils/roi.py
--rw-r--r--   0 jteuwen    (501) staff       (20)     2927 2022-09-19 11:44:11.000000 dlup-0.3.6/dlup/utils/tifffile_utils.py
-drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-01 13:16:41.249642 dlup-0.3.6/dlup/viz/
--rw-r--r--   0 jteuwen    (501) staff       (20)       49 2021-08-25 14:51:38.000000 dlup-0.3.6/dlup/viz/__init__.py
--rw-r--r--   0 jteuwen    (501) staff       (20)     2319 2022-09-19 11:44:11.000000 dlup-0.3.6/dlup/viz/plotting.py
--rw-r--r--   0 jteuwen    (501) staff       (20)     9512 2022-09-19 11:44:11.000000 dlup-0.3.6/dlup/writers.py
-drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-01 13:16:41.245864 dlup-0.3.6/dlup.egg-info/
--rw-r--r--   0 jteuwen    (501) staff       (20)     2013 2022-10-01 13:16:41.000000 dlup-0.3.6/dlup.egg-info/PKG-INFO
--rw-r--r--   0 jteuwen    (501) staff       (20)     1690 2022-10-01 13:16:41.000000 dlup-0.3.6/dlup.egg-info/SOURCES.txt
--rw-r--r--   0 jteuwen    (501) staff       (20)        1 2022-10-01 13:16:41.000000 dlup-0.3.6/dlup.egg-info/dependency_links.txt
--rw-r--r--   0 jteuwen    (501) staff       (20)       39 2022-10-01 13:16:41.000000 dlup-0.3.6/dlup.egg-info/entry_points.txt
--rw-r--r--   0 jteuwen    (501) staff       (20)        1 2022-10-01 13:16:41.000000 dlup-0.3.6/dlup.egg-info/not-zip-safe
--rw-r--r--   0 jteuwen    (501) staff       (20)      245 2022-10-01 13:16:41.000000 dlup-0.3.6/dlup.egg-info/requires.txt
--rw-r--r--   0 jteuwen    (501) staff       (20)        5 2022-10-01 13:16:41.000000 dlup-0.3.6/dlup.egg-info/top_level.txt
-drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-01 13:16:41.252175 dlup-0.3.6/docs/
--rw-r--r--   0 jteuwen    (501) staff       (20)      605 2021-08-25 14:51:38.000000 dlup-0.3.6/docs/Makefile
--rw-r--r--   0 jteuwen    (501) staff       (20)     1633 2022-09-19 11:44:11.000000 dlup-0.3.6/docs/backends.rst
--rw-r--r--   0 jteuwen    (501) staff       (20)      659 2021-11-04 11:38:08.000000 dlup-0.3.6/docs/cli.rst
--rwxr-xr-x   0 jteuwen    (501) staff       (20)     7833 2021-08-25 14:51:38.000000 dlup-0.3.6/docs/conf.py
--rw-r--r--   0 jteuwen    (501) staff       (20)       33 2021-08-25 14:51:38.000000 dlup-0.3.6/docs/contributing.rst
-drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-01 13:16:41.252470 dlup-0.3.6/docs/examples/
--rw-r--r--   0 jteuwen    (501) staff       (20)     2570 2022-09-19 11:44:11.000000 dlup-0.3.6/docs/examples/dataset_examples.rst
--rw-r--r--   0 jteuwen    (501) staff       (20)     3881 2022-06-07 20:52:13.000000 dlup-0.3.6/docs/examples/tile_directory.rst
--rw-r--r--   0 jteuwen    (501) staff       (20)      185 2022-06-07 20:52:13.000000 dlup-0.3.6/docs/examples.rst
-drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-01 13:16:41.253865 dlup-0.3.6/docs/img/
--rw-r--r--   0 jteuwen    (501) staff       (20)   101659 2021-08-25 14:51:38.000000 dlup-0.3.6/docs/img/checkerboard.png
--rw-r--r--   0 jteuwen    (501) staff       (20)    88371 2021-09-04 10:15:10.000000 dlup-0.3.6/docs/img/dataset_example.png
--rw-r--r--   0 jteuwen    (501) staff       (20)    41387 2021-09-04 10:15:10.000000 dlup-0.3.6/docs/img/dataset_example2.png
--rw-r--r--   0 jteuwen    (501) staff       (20)    11077 2021-08-25 14:51:38.000000 dlup-0.3.6/docs/img/overflow.png
--rw-r--r--   0 jteuwen    (501) staff       (20)    10754 2021-08-25 14:51:38.000000 dlup-0.3.6/docs/img/skip.png
--rw-r--r--   0 jteuwen    (501) staff       (20)     1241 2022-09-19 11:44:11.000000 dlup-0.3.6/docs/index.rst
--rw-r--r--   0 jteuwen    (501) staff       (20)     3155 2022-09-19 11:44:11.000000 dlup-0.3.6/docs/installation.rst
--rw-r--r--   0 jteuwen    (501) staff       (20)      766 2021-08-25 14:51:38.000000 dlup-0.3.6/docs/make.bat
--rw-r--r--   0 jteuwen    (501) staff       (20)     4205 2021-11-04 11:38:08.000000 dlup-0.3.6/docs/quickstart.rst
--rw-r--r--   0 jteuwen    (501) staff       (20)      918 2022-09-19 11:44:11.000000 dlup-0.3.6/docs/tiling.rst
--rw-r--r--   0 jteuwen    (501) staff       (20)     4165 2022-09-19 11:44:11.000000 dlup-0.3.6/docs/writers.rst
--rw-r--r--   0 jteuwen    (501) staff       (20)     1191 2022-09-19 11:44:11.000000 dlup-0.3.6/pyproject.toml
--rw-r--r--   0 jteuwen    (501) staff       (20)      478 2022-10-01 13:16:41.256052 dlup-0.3.6/setup.cfg
--rw-r--r--   0 jteuwen    (501) staff       (20)     2187 2022-09-19 11:44:11.000000 dlup-0.3.6/setup.py
-drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-01 13:16:41.255164 dlup-0.3.6/tests/
--rw-r--r--   0 jteuwen    (501) staff       (20)        0 2022-09-19 11:44:11.000000 dlup-0.3.6/tests/__init__.py
--rw-r--r--   0 jteuwen    (501) staff       (20)     4399 2022-09-19 11:44:11.000000 dlup-0.3.6/tests/common.py
--rw-r--r--   0 jteuwen    (501) staff       (20)      554 2022-09-19 11:44:11.000000 dlup-0.3.6/tests/conftest.py
--rw-r--r--   0 jteuwen    (501) staff       (20)     4621 2022-09-19 11:44:11.000000 dlup-0.3.6/tests/test_annotations.py
--rw-r--r--   0 jteuwen    (501) staff       (20)      911 2022-09-19 11:44:11.000000 dlup-0.3.6/tests/test_dataset.py
--rw-r--r--   0 jteuwen    (501) staff       (20)     7090 2022-09-19 11:44:11.000000 dlup-0.3.6/tests/test_image.py
--rw-r--r--   0 jteuwen    (501) staff       (20)      918 2022-05-31 16:34:46.000000 dlup-0.3.6/tests/test_multiscale.py
--rw-r--r--   0 jteuwen    (501) staff       (20)     3355 2022-09-19 11:44:11.000000 dlup-0.3.6/tests/test_tiling.py
--rw-r--r--   0 jteuwen    (501) staff       (20)     1529 2022-09-22 12:38:29.000000 dlup-0.3.6/tests/test_writers.py
--rw-r--r--   0 jteuwen    (501) staff       (20)     1809 2022-08-27 10:13:06.000000 dlup-0.3.6/tests/transform_prelim..py
-drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-01 13:16:41.255523 dlup-0.3.6/tests/utils/
--rw-r--r--   0 jteuwen    (501) staff       (20)        0 2022-09-19 11:44:11.000000 dlup-0.3.6/tests/utils/__init__.py
--rw-r--r--   0 jteuwen    (501) staff       (20)      565 2022-09-19 11:44:11.000000 dlup-0.3.6/tests/utils/test_pyvips.py
+drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-22 10:26:03.229647 dlup-0.3.7/
+-rw-r--r--   0 jteuwen    (501) staff       (20)     3579 2021-08-25 14:51:38.000000 dlup-0.3.7/CONTRIBUTING.rst
+-rw-r--r--   0 jteuwen    (501) staff       (20)    11357 2021-08-25 14:51:38.000000 dlup-0.3.7/LICENSE
+-rw-r--r--   0 jteuwen    (501) staff       (20)      226 2021-08-25 14:51:38.000000 dlup-0.3.7/MANIFEST.in
+-rw-r--r--   0 jteuwen    (501) staff       (20)     2013 2022-10-22 10:26:03.229712 dlup-0.3.7/PKG-INFO
+-rw-r--r--   0 jteuwen    (501) staff       (20)     1371 2022-09-19 11:44:11.000000 dlup-0.3.7/README.md
+drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-22 10:26:03.219901 dlup-0.3.7/dlup/
+-rw-r--r--   0 jteuwen    (501) staff       (20)      390 2022-10-22 10:24:25.000000 dlup-0.3.7/dlup/__init__.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)      445 2022-09-19 11:44:11.000000 dlup-0.3.7/dlup/_exceptions.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)    12671 2022-10-20 14:15:56.000000 dlup-0.3.7/dlup/_image.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)     2722 2022-09-19 11:44:11.000000 dlup-0.3.7/dlup/_region.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)    27039 2022-10-12 08:35:30.000000 dlup-0.3.7/dlup/annotations.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)    10758 2022-10-20 14:15:59.000000 dlup-0.3.7/dlup/background.py
+drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-22 10:26:03.220857 dlup-0.3.7/dlup/cli/
+-rw-r--r--   0 jteuwen    (501) staff       (20)      862 2022-01-22 12:00:51.000000 dlup-0.3.7/dlup/cli/__init__.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)     7630 2022-09-19 11:44:11.000000 dlup-0.3.7/dlup/cli/wsi.py
+drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-22 10:26:03.221417 dlup-0.3.7/dlup/data/
+-rw-r--r--   0 jteuwen    (501) staff       (20)       49 2021-08-25 14:51:38.000000 dlup-0.3.7/dlup/data/__init__.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)    16579 2022-10-20 14:15:56.000000 dlup-0.3.7/dlup/data/dataset.py
+drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-22 10:26:03.221753 dlup-0.3.7/dlup/data/experimental/
+-rw-r--r--   0 jteuwen    (501) staff       (20)       49 2022-09-19 11:44:11.000000 dlup-0.3.7/dlup/data/experimental/__init__.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)     5501 2022-09-19 11:44:11.000000 dlup-0.3.7/dlup/data/experimental/dataset.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)     7894 2022-10-12 10:50:28.000000 dlup-0.3.7/dlup/data/transforms.py
+drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-22 10:26:03.222682 dlup-0.3.7/dlup/experimental_backends/
+-rw-r--r--   0 jteuwen    (501) staff       (20)     3921 2022-09-19 11:44:11.000000 dlup-0.3.7/dlup/experimental_backends/__init__.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)     5550 2022-10-20 14:15:56.000000 dlup-0.3.7/dlup/experimental_backends/common.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)     2192 2022-09-19 11:44:11.000000 dlup-0.3.7/dlup/experimental_backends/openslide_backend.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)     6201 2022-10-20 14:15:56.000000 dlup-0.3.7/dlup/experimental_backends/pyvips_backend.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)     4023 2022-09-19 11:44:11.000000 dlup-0.3.7/dlup/experimental_backends/tifffile_backend.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)     2602 2022-09-19 11:44:11.000000 dlup-0.3.7/dlup/logging.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)     5026 2022-09-19 11:44:11.000000 dlup-0.3.7/dlup/tiling.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)     1941 2021-11-04 11:38:08.000000 dlup-0.3.7/dlup/tools.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)      384 2022-10-22 10:24:35.000000 dlup-0.3.7/dlup/types.py
+drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-22 10:26:03.223518 dlup-0.3.7/dlup/utils/
+-rw-r--r--   0 jteuwen    (501) staff       (20)      841 2022-09-19 11:44:11.000000 dlup-0.3.7/dlup/utils/__init__.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)      583 2022-09-19 11:44:11.000000 dlup-0.3.7/dlup/utils/image.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)      693 2022-09-19 11:44:11.000000 dlup-0.3.7/dlup/utils/imports.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)     1587 2022-09-19 11:44:11.000000 dlup-0.3.7/dlup/utils/pyvips_utils.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)     3889 2022-09-18 19:42:47.000000 dlup-0.3.7/dlup/utils/roi.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)     2927 2022-09-19 11:44:11.000000 dlup-0.3.7/dlup/utils/tifffile_utils.py
+drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-22 10:26:03.223844 dlup-0.3.7/dlup/viz/
+-rw-r--r--   0 jteuwen    (501) staff       (20)       49 2021-08-25 14:51:38.000000 dlup-0.3.7/dlup/viz/__init__.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)     2319 2022-09-19 11:44:11.000000 dlup-0.3.7/dlup/viz/plotting.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)     9512 2022-09-19 11:44:11.000000 dlup-0.3.7/dlup/writers.py
+drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-22 10:26:03.220566 dlup-0.3.7/dlup.egg-info/
+-rw-r--r--   0 jteuwen    (501) staff       (20)     2013 2022-10-22 10:26:03.000000 dlup-0.3.7/dlup.egg-info/PKG-INFO
+-rw-r--r--   0 jteuwen    (501) staff       (20)     1710 2022-10-22 10:26:03.000000 dlup-0.3.7/dlup.egg-info/SOURCES.txt
+-rw-r--r--   0 jteuwen    (501) staff       (20)        1 2022-10-22 10:26:03.000000 dlup-0.3.7/dlup.egg-info/dependency_links.txt
+-rw-r--r--   0 jteuwen    (501) staff       (20)       39 2022-10-22 10:26:03.000000 dlup-0.3.7/dlup.egg-info/entry_points.txt
+-rw-r--r--   0 jteuwen    (501) staff       (20)        1 2022-10-22 10:26:03.000000 dlup-0.3.7/dlup.egg-info/not-zip-safe
+-rw-r--r--   0 jteuwen    (501) staff       (20)      245 2022-10-22 10:26:03.000000 dlup-0.3.7/dlup.egg-info/requires.txt
+-rw-r--r--   0 jteuwen    (501) staff       (20)        5 2022-10-22 10:26:03.000000 dlup-0.3.7/dlup.egg-info/top_level.txt
+drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-22 10:26:03.225990 dlup-0.3.7/docs/
+-rw-r--r--   0 jteuwen    (501) staff       (20)      605 2021-08-25 14:51:38.000000 dlup-0.3.7/docs/Makefile
+-rw-r--r--   0 jteuwen    (501) staff       (20)     1633 2022-09-19 11:44:11.000000 dlup-0.3.7/docs/backends.rst
+-rw-r--r--   0 jteuwen    (501) staff       (20)      659 2021-11-04 11:38:08.000000 dlup-0.3.7/docs/cli.rst
+-rwxr-xr-x   0 jteuwen    (501) staff       (20)     7833 2021-08-25 14:51:38.000000 dlup-0.3.7/docs/conf.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)       33 2021-08-25 14:51:38.000000 dlup-0.3.7/docs/contributing.rst
+drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-22 10:26:03.226251 dlup-0.3.7/docs/examples/
+-rw-r--r--   0 jteuwen    (501) staff       (20)     2570 2022-09-19 11:44:11.000000 dlup-0.3.7/docs/examples/dataset_examples.rst
+-rw-r--r--   0 jteuwen    (501) staff       (20)     3881 2022-06-07 20:52:13.000000 dlup-0.3.7/docs/examples/tile_directory.rst
+-rw-r--r--   0 jteuwen    (501) staff       (20)      185 2022-06-07 20:52:13.000000 dlup-0.3.7/docs/examples.rst
+drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-22 10:26:03.227762 dlup-0.3.7/docs/img/
+-rw-r--r--   0 jteuwen    (501) staff       (20)   101659 2021-08-25 14:51:38.000000 dlup-0.3.7/docs/img/checkerboard.png
+-rw-r--r--   0 jteuwen    (501) staff       (20)    88371 2021-09-04 10:15:10.000000 dlup-0.3.7/docs/img/dataset_example.png
+-rw-r--r--   0 jteuwen    (501) staff       (20)    41387 2021-09-04 10:15:10.000000 dlup-0.3.7/docs/img/dataset_example2.png
+-rw-r--r--   0 jteuwen    (501) staff       (20)    11077 2021-08-25 14:51:38.000000 dlup-0.3.7/docs/img/overflow.png
+-rw-r--r--   0 jteuwen    (501) staff       (20)    10754 2021-08-25 14:51:38.000000 dlup-0.3.7/docs/img/skip.png
+-rw-r--r--   0 jteuwen    (501) staff       (20)     1241 2022-09-19 11:44:11.000000 dlup-0.3.7/docs/index.rst
+-rw-r--r--   0 jteuwen    (501) staff       (20)     3155 2022-09-19 11:44:11.000000 dlup-0.3.7/docs/installation.rst
+-rw-r--r--   0 jteuwen    (501) staff       (20)      766 2021-08-25 14:51:38.000000 dlup-0.3.7/docs/make.bat
+-rw-r--r--   0 jteuwen    (501) staff       (20)     4205 2021-11-04 11:38:08.000000 dlup-0.3.7/docs/quickstart.rst
+-rw-r--r--   0 jteuwen    (501) staff       (20)      918 2022-09-19 11:44:11.000000 dlup-0.3.7/docs/tiling.rst
+-rw-r--r--   0 jteuwen    (501) staff       (20)     4165 2022-09-19 11:44:11.000000 dlup-0.3.7/docs/writers.rst
+-rw-r--r--   0 jteuwen    (501) staff       (20)     1191 2022-09-19 11:44:11.000000 dlup-0.3.7/pyproject.toml
+-rw-r--r--   0 jteuwen    (501) staff       (20)      478 2022-10-22 10:26:03.229963 dlup-0.3.7/setup.cfg
+-rw-r--r--   0 jteuwen    (501) staff       (20)     2187 2022-09-19 11:44:11.000000 dlup-0.3.7/setup.py
+drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-22 10:26:03.229251 dlup-0.3.7/tests/
+-rw-r--r--   0 jteuwen    (501) staff       (20)        0 2022-09-19 11:44:11.000000 dlup-0.3.7/tests/__init__.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)     4399 2022-09-19 11:44:11.000000 dlup-0.3.7/tests/common.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)      554 2022-09-19 11:44:11.000000 dlup-0.3.7/tests/conftest.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)      151 2022-10-10 16:44:17.000000 dlup-0.3.7/tests/leuke_test.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)     4621 2022-09-19 11:44:11.000000 dlup-0.3.7/tests/test_annotations.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)      911 2022-09-19 11:44:11.000000 dlup-0.3.7/tests/test_dataset.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)     7090 2022-09-19 11:44:11.000000 dlup-0.3.7/tests/test_image.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)      918 2022-05-31 16:34:46.000000 dlup-0.3.7/tests/test_multiscale.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)     3355 2022-09-19 11:44:11.000000 dlup-0.3.7/tests/test_tiling.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)     1529 2022-09-22 12:38:29.000000 dlup-0.3.7/tests/test_writers.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)     1809 2022-08-27 10:13:06.000000 dlup-0.3.7/tests/transform_prelim..py
+drwxr-xr-x   0 jteuwen    (501) staff       (20)        0 2022-10-22 10:26:03.229535 dlup-0.3.7/tests/utils/
+-rw-r--r--   0 jteuwen    (501) staff       (20)        0 2022-09-19 11:44:11.000000 dlup-0.3.7/tests/utils/__init__.py
+-rw-r--r--   0 jteuwen    (501) staff       (20)      565 2022-09-19 11:44:11.000000 dlup-0.3.7/tests/utils/test_pyvips.py
```

### Comparing `dlup-0.3.6/CONTRIBUTING.rst` & `dlup-0.3.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/LICENSE` & `dlup-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/PKG-INFO` & `dlup-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlup
-Version: 0.3.6
+Version: 0.3.7
 Home-page: https://github.com/NKI-AI/dlup
 Author: Jonas Teuwen
 Author-email: j.teuwen@nki.nl
 License: Apache Software License 2.0
 Keywords: dlup
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `dlup-0.3.6/README.md` & `dlup-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/dlup/_image.py` & `dlup-0.3.7/dlup/_image.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/dlup/_region.py` & `dlup-0.3.7/dlup/_region.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/dlup/annotations.py` & `dlup-0.3.7/dlup/annotations.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,22 +126,24 @@
         except KeyError as e:
             raise AttributeError(str(e)) from None
 
     def __str__(self) -> str:
         return f"{self.label}, {self.wkt}"
 
 
-def shape(coordinates, label):
+def shape(coordinates, label, multiplier: float = 1.0):
     geom_type = coordinates.get("type").lower()
     if geom_type == "point":
-        return [Point(coordinates["coordinates"], label=label)]
+        return [Point(np.asarray(coordinates["coordinates"]) * multiplier, label=label)]
     elif geom_type == "polygon":
-        return [Polygon(coordinates["coordinates"][0], label=label)]
+        return [Polygon(np.asarray(coordinates["coordinates"][0]) * multiplier, label=label)]
     elif geom_type == "multipolygon":
-        multi_polygon = shapely.geometry.MultiPolygon([[c[0], c[1:]] for c in coordinates["coordinates"]])
+        multi_polygon = shapely.geometry.MultiPolygon(
+            [[np.asarray(c[0]) * multiplier, np.asarray(c[1:]) * multiplier] for c in coordinates["coordinates"]]
+        )
         return [Polygon(_, label=label) for _ in multi_polygon.geoms]
     else:
         raise NotImplementedError(f"Not support geom_type {geom_type}")
 
 
 _POSTPROCESSORS = {
     AnnotationType.POINT: lambda x, region: x,
@@ -328,30 +330,30 @@
         -------
         WsiAnnotations
 
         """
         data = defaultdict(list)
         _remap_labels = {} if not remap_labels else remap_labels
         _scaling = 1.0 if not scaling else scaling
-        _geojsons = [geojsons] if not isinstance(geojsons, (tuple, list, Iterable)) else geojsons
+        if isinstance(geojsons, str):
+            _geojsons: Iterable[Any] = [pathlib.Path(geojsons)]
+
+        _geojsons = [geojsons] if not isinstance(geojsons, (tuple, list)) else geojsons
         for idx, path in enumerate(_geojsons):
             path = pathlib.Path(path)
             if not path.exists():
                 raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), str(path))
 
             with open(path, "r", encoding="utf-8") as annotation_file:
                 geojson_dict = json.load(annotation_file)["features"]
                 for x in geojson_dict:
-                    coordinates = np.asarray(x["geometry"]["coordinates"]) * _scaling
-                    x["geometry"]["coordinates"] = coordinates.tolist()
                     _label = x["properties"]["classification"]["name"]
-
                     if remap_labels and _label in _remap_labels:
                         _label = _remap_labels[_label]
-                    _geometry = shape(x["geometry"], label=_label)
+                    _geometry = shape(x["geometry"], label=_label, multiplier=_scaling)
                     for _ in _geometry:
                         data[_label].append(_)
 
         # It is assume that a specific label can only be one type (point or polygon)
         annotations: List[WsiSingleLabelAnnotation] = [
             WsiSingleLabelAnnotation(label=k, type=data[k][0].type, coordinates=data[k]) for k in data.keys()
         ]
```

### Comparing `dlup-0.3.6/dlup/background.py` & `dlup-0.3.7/dlup/background.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,15 @@
     x, y, w, h, mpp = region
 
     scaling = slide_image.get_scaling(mpp)
 
     polygon_region = background_mask.read_region((x, y), scaling, (w, h))
     total_area = sum([_.area for _ in polygon_region])
 
-    if total_area / (w * h) > threshold:
+    if total_area / (w * h) >= threshold:
         return True
 
     return False
 
 
 def is_foreground_wsiannotations(
     background_mask: SlideImage,
@@ -266,15 +266,15 @@
 
     # TODO: Let us read the mask at its native mpp for speed
     # Can do something as follows, but that is not exposed right now, so that waits for such an implementation.
     # best_level = background_mask._wsi.get_best_level_for_downsample(scaling)
     mask_region_view = background_mask.get_scaled_view(background_mask.get_scaling(mpp))
     mask = mask_region_view.read_region((x, y), (w, h)).convert("L")
 
-    return np.asarray(mask).mean() > threshold
+    return np.asarray(mask).mean() >= threshold
 
 
 def is_foreground_numpy(
     slide_image: SlideImage,
     background_mask: np.ndarray,
     region: Tuple[float, float, int, int, float],
     threshold: float = 1.0,
@@ -307,15 +307,15 @@
 
     if clipped_h == 0 or clipped_w == 0:
         return False
 
     mask_tile[:clipped_h, :clipped_w] = np.asarray(
         background_mask.resize((clipped_w, clipped_h), PIL.Image.BICUBIC, box=box), dtype=float  # type: ignore
     )
-    return mask_tile.mean() > threshold
+    return mask_tile.mean() >= threshold
 
 
 class AvailableMaskFunctions(Enum):
     """
     Class that maps strngs to the currently implemented mask functions as defined in dlup/background.py
 
     The method returns the function from a string input, e.g.
```

### Comparing `dlup-0.3.6/dlup/cli/__init__.py` & `dlup-0.3.7/dlup/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/dlup/cli/wsi.py` & `dlup-0.3.7/dlup/cli/wsi.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/dlup/data/dataset.py` & `dlup-0.3.7/dlup/data/dataset.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/dlup/data/experimental/dataset.py` & `dlup-0.3.7/dlup/data/experimental/dataset.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/dlup/data/transforms.py` & `dlup-0.3.7/dlup/data/transforms.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/dlup/experimental_backends/__init__.py` & `dlup-0.3.7/dlup/experimental_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/dlup/experimental_backends/common.py` & `dlup-0.3.7/dlup/experimental_backends/common.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/dlup/experimental_backends/openslide_backend.py` & `dlup-0.3.7/dlup/experimental_backends/openslide_backend.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/dlup/experimental_backends/pyvips_backend.py` & `dlup-0.3.7/dlup/experimental_backends/pyvips_backend.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/dlup/experimental_backends/tifffile_backend.py` & `dlup-0.3.7/dlup/experimental_backends/tifffile_backend.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/dlup/logging.py` & `dlup-0.3.7/dlup/logging.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/dlup/tiling.py` & `dlup-0.3.7/dlup/tiling.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/dlup/tools.py` & `dlup-0.3.7/dlup/tools.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/dlup/utils/__init__.py` & `dlup-0.3.7/dlup/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/dlup/utils/image.py` & `dlup-0.3.7/dlup/utils/image.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/dlup/utils/imports.py` & `dlup-0.3.7/dlup/utils/imports.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/dlup/utils/pyvips_utils.py` & `dlup-0.3.7/dlup/utils/pyvips_utils.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/dlup/utils/roi.py` & `dlup-0.3.7/dlup/utils/roi.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/dlup/utils/tifffile_utils.py` & `dlup-0.3.7/dlup/utils/tifffile_utils.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/dlup/viz/plotting.py` & `dlup-0.3.7/dlup/viz/plotting.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/dlup/writers.py` & `dlup-0.3.7/dlup/writers.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/dlup.egg-info/PKG-INFO` & `dlup-0.3.7/dlup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlup
-Version: 0.3.6
+Version: 0.3.7
 Home-page: https://github.com/NKI-AI/dlup
 Author: Jonas Teuwen
 Author-email: j.teuwen@nki.nl
 License: Apache Software License 2.0
 Keywords: dlup
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `dlup-0.3.6/dlup.egg-info/SOURCES.txt` & `dlup-0.3.7/dlup.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 docs/img/dataset_example.png
 docs/img/dataset_example2.png
 docs/img/overflow.png
 docs/img/skip.png
 tests/__init__.py
 tests/common.py
 tests/conftest.py
+tests/leuke_test.py
 tests/test_annotations.py
 tests/test_dataset.py
 tests/test_image.py
 tests/test_multiscale.py
 tests/test_tiling.py
 tests/test_writers.py
 tests/transform_prelim..py
```

### Comparing `dlup-0.3.6/docs/Makefile` & `dlup-0.3.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/docs/backends.rst` & `dlup-0.3.7/docs/backends.rst`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/docs/cli.rst` & `dlup-0.3.7/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/docs/conf.py` & `dlup-0.3.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/docs/examples/dataset_examples.rst` & `dlup-0.3.7/docs/examples/dataset_examples.rst`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/docs/examples/tile_directory.rst` & `dlup-0.3.7/docs/examples/tile_directory.rst`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/docs/img/checkerboard.png` & `dlup-0.3.7/docs/img/checkerboard.png`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/docs/img/dataset_example.png` & `dlup-0.3.7/docs/img/dataset_example.png`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/docs/img/dataset_example2.png` & `dlup-0.3.7/docs/img/dataset_example2.png`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/docs/img/overflow.png` & `dlup-0.3.7/docs/img/overflow.png`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/docs/img/skip.png` & `dlup-0.3.7/docs/img/skip.png`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/docs/index.rst` & `dlup-0.3.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/docs/installation.rst` & `dlup-0.3.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/docs/make.bat` & `dlup-0.3.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/docs/quickstart.rst` & `dlup-0.3.7/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/docs/tiling.rst` & `dlup-0.3.7/docs/tiling.rst`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/docs/writers.rst` & `dlup-0.3.7/docs/writers.rst`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/pyproject.toml` & `dlup-0.3.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/setup.py` & `dlup-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/tests/common.py` & `dlup-0.3.7/tests/common.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/tests/conftest.py` & `dlup-0.3.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/tests/test_annotations.py` & `dlup-0.3.7/tests/test_annotations.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/tests/test_dataset.py` & `dlup-0.3.7/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/tests/test_image.py` & `dlup-0.3.7/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/tests/test_multiscale.py` & `dlup-0.3.7/tests/test_multiscale.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/tests/test_tiling.py` & `dlup-0.3.7/tests/test_tiling.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/tests/test_writers.py` & `dlup-0.3.7/tests/test_writers.py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/tests/transform_prelim..py` & `dlup-0.3.7/tests/transform_prelim..py`

 * *Files identical despite different names*

### Comparing `dlup-0.3.6/tests/utils/test_pyvips.py` & `dlup-0.3.7/tests/utils/test_pyvips.py`

 * *Files identical despite different names*


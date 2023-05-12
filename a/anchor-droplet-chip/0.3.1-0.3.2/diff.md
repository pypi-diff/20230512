# Comparing `tmp/anchor_droplet_chip-0.3.1.tar.gz` & `tmp/anchor_droplet_chip-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anchor_droplet_chip-0.3.1.tar", last modified: Tue Apr  4 15:22:13 2023, max compression
+gzip compressed data, was "anchor_droplet_chip-0.3.2.tar", last modified: Fri May 12 10:06:12 2023, max compression
```

## Comparing `anchor_droplet_chip-0.3.1.tar` & `anchor_droplet_chip-0.3.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:22:13.420805 anchor_droplet_chip-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/-- SQLite.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:22:13.392805 anchor_droplet_chip-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:22:13.400805 anchor_droplet_chip-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-04-04 15:22:13.420805 anchor_droplet_chip-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/Snakefile
--rw-r--r--   0 runner    (1001) docker     (123)    75936 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   223486 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/find_all_big_nd2.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/logging.conf
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/runtime.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:22:13.400805 anchor_droplet_chip-0.3.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/scripts/merge_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/scripts/zarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-04 15:22:13.420805 anchor_droplet_chip-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:22:13.396805 anchor_droplet_chip-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:22:13.408805 anchor_droplet_chip-0.3.1/src/adc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/_align_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/_combine_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/_count_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/_manual_rois.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/_progress_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/_projection_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/_split_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/_sub_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-04 15:22:13.000000 anchor_droplet_chip-0.3.1/src/adc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/align.py
--rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:22:13.416805 anchor_droplet_chip-0.3.1/src/adc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/tests/test_count.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/tests/test_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/tests/test_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/tests/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/adc/tests/test_substack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:22:13.420805 anchor_droplet_chip-0.3.1/src/anchor_droplet_chip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-04-04 15:22:13.000000 anchor_droplet_chip-0.3.1/src/anchor_droplet_chip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-04 15:22:13.000000 anchor_droplet_chip-0.3.1/src/anchor_droplet_chip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 15:22:13.000000 anchor_droplet_chip-0.3.1/src/anchor_droplet_chip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-04 15:22:13.000000 anchor_droplet_chip-0.3.1/src/anchor_droplet_chip.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-04 15:22:13.000000 anchor_droplet_chip-0.3.1/src/anchor_droplet_chip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-04 15:22:13.000000 anchor_droplet_chip-0.3.1/src/anchor_droplet_chip.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:22:13.420805 anchor_droplet_chip-0.3.1/src/imreg_dft/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/imreg_dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26470 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/imreg_dft/imreg.py
--rw-r--r--   0 runner    (1001) docker     (123)    28749 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/src/imreg_dft/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/test_data_0h.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/test_data_24h.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)    17856 2023-04-04 15:21:46.000000 anchor_droplet_chip-0.3.1/zenodo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:06:12.830088 anchor_droplet_chip-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/-- SQLite.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:06:12.806088 anchor_droplet_chip-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:06:12.814088 anchor_droplet_chip-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-05-12 10:06:12.830088 anchor_droplet_chip-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (123)    75936 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   223486 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/find_all_big_nd2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/logging.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/runtime.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:06:12.818088 anchor_droplet_chip-0.3.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/scripts/merge_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/scripts/zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-12 10:06:12.830088 anchor_droplet_chip-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:06:12.810088 anchor_droplet_chip-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:06:12.822088 anchor_droplet_chip-0.3.2/src/adc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/_align_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/_combine_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/_count_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/_manual_rois.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/_progress_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/_projection_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/_split_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/_sub_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-12 10:06:12.000000 anchor_droplet_chip-0.3.2/src/adc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:06:12.826088 anchor_droplet_chip-0.3.2/src/adc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/tests/test_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/tests/test_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/tests/test_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/tests/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/adc/tests/test_substack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:06:12.830088 anchor_droplet_chip-0.3.2/src/anchor_droplet_chip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-05-12 10:06:12.000000 anchor_droplet_chip-0.3.2/src/anchor_droplet_chip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-12 10:06:12.000000 anchor_droplet_chip-0.3.2/src/anchor_droplet_chip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:06:12.000000 anchor_droplet_chip-0.3.2/src/anchor_droplet_chip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-12 10:06:12.000000 anchor_droplet_chip-0.3.2/src/anchor_droplet_chip.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-12 10:06:12.000000 anchor_droplet_chip-0.3.2/src/anchor_droplet_chip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-12 10:06:12.000000 anchor_droplet_chip-0.3.2/src/anchor_droplet_chip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:06:12.830088 anchor_droplet_chip-0.3.2/src/imreg_dft/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/imreg_dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26470 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/imreg_dft/imreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28749 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/src/imreg_dft/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/test_data_0h.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/test_data_24h.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    17856 2023-05-12 10:05:50.000000 anchor_droplet_chip-0.3.2/zenodo.ipynb
```

### Comparing `anchor_droplet_chip-0.3.1/.github/workflows/python-package.yml` & `anchor_droplet_chip-0.3.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/.gitignore` & `anchor_droplet_chip-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/.pre-commit-config.yaml` & `anchor_droplet_chip-0.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/LICENSE` & `anchor_droplet_chip-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/PKG-INFO` & `anchor_droplet_chip-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anchor_droplet_chip
-Version: 0.3.1
+Version: 0.3.2
 Summary: Segment organoids and measure intensities
 Home-page: https://github.com/BaroudLab/anchor-driplet-chip
 Author: Andrey Aristov
 Author-email: aaristov@pasteur.fr
 License: BSD-3-Clause
 Project-URL: Source Code, https://github.com/BaroudLab/anchor-droplet-chip
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `anchor_droplet_chip-0.3.1/README.md` & `anchor_droplet_chip-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/Snakefile` & `anchor_droplet_chip-0.3.2/Snakefile`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/example.ipynb` & `anchor_droplet_chip-0.3.2/example.ipynb`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/find_all_big_nd2.ipynb` & `anchor_droplet_chip-0.3.2/find_all_big_nd2.ipynb`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/scripts/zarr.py` & `anchor_droplet_chip-0.3.2/scripts/zarr.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/setup.cfg` & `anchor_droplet_chip-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/src/adc/_align_widget.py` & `anchor_droplet_chip-0.3.2/src/adc/_align_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,17 @@
         self.viewer.add_image(img[0], **img[1])
         self.viewer.add_points(centers[0], **centers[1])
         self.reset_choices()
 
     def _detect(self):
         logger.info("Start detecting")
         data_layer = self.viewer.layers[self.select_image.current_choice]
+
+        assert isinstance(path := get_path(data_layer), str)
+        logger.debug(f"data path: {path}")
         if data_layer.multiscale:
             n_scales = len(data_layer.data)
             assert (
                 n_scales >= 2
             ), "Weird multiscale, looking for 1/8 scale, or 1/4 at least"
             if isinstance(data_layer.data[n_scales - 1], da.Array):
                 try:
@@ -130,14 +133,23 @@
 
     def reset_choices(self, event=None):
         self.select_image.reset_choices(event)
         self.select_template.reset_choices(event)
         self.select_centers.reset_choices(event)
 
 
+def get_path(data_layer):
+    if (path := data_layer.source.path) is not None:
+        return path
+    elif (path := data_layer.metadata["path"]) is not None:
+        return path
+    else:
+        raise ValueError("Unable to get path of the dataset")
+
+
 def show_droplet_layer(viewer, data):
     return viewer.add_points(data, **DROPLETS_LAYER_PROPS)
 
 
 def add_new_dim(centers, value):
     return np.concatenate(
         (np.ones((len(centers), 1)) * value, centers), axis=1
```

### Comparing `anchor_droplet_chip-0.3.1/src/adc/_combine_widget.py` & `anchor_droplet_chip-0.3.2/src/adc/_combine_widget.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/src/adc/_count_widget.py` & `anchor_droplet_chip-0.3.2/src/adc/_count_widget.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/src/adc/_manual_rois.py` & `anchor_droplet_chip-0.3.2/src/adc/_manual_rois.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/src/adc/_progress_widget.py` & `anchor_droplet_chip-0.3.2/src/adc/_progress_widget.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/src/adc/_projection_stack.py` & `anchor_droplet_chip-0.3.2/src/adc/_projection_stack.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/src/adc/_reader.py` & `anchor_droplet_chip-0.3.2/src/adc/_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 
 def read_json(path):
     return json.load(path)
 
 
 def read_zarr(path):
     print(f"read_zarr {path}")
-
+    meta = {"path": path}
     try:
         attrs = json.load(open(os.path.join(path, ".zattrs")))
         info = attrs["multiscales"]["multiscales"][0]
         dataset_paths = [
             os.path.join(path, d["path"]) for d in info["datasets"]
         ]
         datasets = [da.from_zarr(p) for p in dataset_paths]
@@ -175,19 +175,21 @@
         logger.debug("no info found")
         colormap = None
 
     try:
         name = info["name"]
     except KeyError:
         print("name not found")
-        name = [os.path.basename(path)] * datasets[0].shape[channel_axis]
-    except Exception as e:
-        print("name exception", e.args)
         name = os.path.basename(path)
-    meta = {"path": path}
+
+    try:
+        pixel_size_um = info["pixel_size_um"]
+    except (UnboundLocalError, KeyError):
+        pixel_size_um = None
+    meta["pixel_size_um"] = pixel_size_um
 
     try:
         if "sizes" in info:
             meta["sizes"] = info["sizes"]
     except UnboundLocalError:
         pass
```

### Comparing `anchor_droplet_chip-0.3.1/src/adc/_sample_data.py` & `anchor_droplet_chip-0.3.2/src/adc/_sample_data.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/src/adc/_split_stack.py` & `anchor_droplet_chip-0.3.2/src/adc/_split_stack.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/src/adc/_sub_stack.py` & `anchor_droplet_chip-0.3.2/src/adc/_sub_stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             self.out_dask,
             name=f"{self.selected_layer.name}_{self.crop_coords}",
             channel_axis=channel_axis,
             metadata={
                 "pixel_size_um": self.pixel_size_um,
                 "sizes": self.out_sizes,
                 "substack_coords": self.crop_coords,
-                "source_path": self.path,
+                "path": self.path,
                 "dask_data": self.out_dask,
             },
         )
 
     def compute_substack(self):
         logger.debug("Compute substack")
         slices = []
```

### Comparing `anchor_droplet_chip-0.3.1/src/adc/align.py` & `anchor_droplet_chip-0.3.2/src/adc/align.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/src/adc/count.py` & `anchor_droplet_chip-0.3.2/src/adc/count.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/src/adc/fit.py` & `anchor_droplet_chip-0.3.2/src/adc/fit.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/src/adc/io.py` & `anchor_droplet_chip-0.3.2/src/adc/io.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/src/adc/merge.py` & `anchor_droplet_chip-0.3.2/src/adc/merge.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/src/adc/napari.yaml` & `anchor_droplet_chip-0.3.2/src/adc/napari.yaml`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/src/adc/plot.py` & `anchor_droplet_chip-0.3.2/src/adc/plot.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/src/adc/tests/test_align.py` & `anchor_droplet_chip-0.3.2/src/adc/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/src/adc/tests/test_count.py` & `anchor_droplet_chip-0.3.2/src/adc/tests/test_count.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/src/adc/tests/test_projection.py` & `anchor_droplet_chip-0.3.2/src/adc/tests/test_projection.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/src/adc/tests/test_reader.py` & `anchor_droplet_chip-0.3.2/src/adc/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/src/adc/tests/test_split.py` & `anchor_droplet_chip-0.3.2/src/adc/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/src/adc/tests/test_stack.py` & `anchor_droplet_chip-0.3.2/src/adc/tests/test_stack.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/src/adc/tests/test_substack.py` & `anchor_droplet_chip-0.3.2/src/adc/tests/test_substack.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/src/anchor_droplet_chip.egg-info/PKG-INFO` & `anchor_droplet_chip-0.3.2/src/anchor_droplet_chip.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anchor-droplet-chip
-Version: 0.3.1
+Version: 0.3.2
 Summary: Segment organoids and measure intensities
 Home-page: https://github.com/BaroudLab/anchor-driplet-chip
 Author: Andrey Aristov
 Author-email: aaristov@pasteur.fr
 License: BSD-3-Clause
 Project-URL: Source Code, https://github.com/BaroudLab/anchor-droplet-chip
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `anchor_droplet_chip-0.3.1/src/anchor_droplet_chip.egg-info/SOURCES.txt` & `anchor_droplet_chip-0.3.2/src/anchor_droplet_chip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/src/imreg_dft/imreg.py` & `anchor_droplet_chip-0.3.2/src/imreg_dft/imreg.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/src/imreg_dft/utils.py` & `anchor_droplet_chip-0.3.2/src/imreg_dft/utils.py`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/test_data_0h.yaml` & `anchor_droplet_chip-0.3.2/test_data_0h.yaml`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/test_data_24h.yaml` & `anchor_droplet_chip-0.3.2/test_data_24h.yaml`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/tox.ini` & `anchor_droplet_chip-0.3.2/tox.ini`

 * *Files identical despite different names*

### Comparing `anchor_droplet_chip-0.3.1/zenodo.ipynb` & `anchor_droplet_chip-0.3.2/zenodo.ipynb`

 * *Files identical despite different names*


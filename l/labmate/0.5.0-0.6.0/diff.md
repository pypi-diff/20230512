# Comparing `tmp/labmate-0.5.0.tar.gz` & `tmp/labmate-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labmate-0.5.0.tar", last modified: Fri Mar 17 16:55:25 2023, max compression
+gzip compressed data, was "labmate-0.6.0.tar", last modified: Fri May 12 13:19:49 2023, max compression
```

## Comparing `labmate-0.5.0.tar` & `labmate-0.6.0.tar`

### file list

```diff
@@ -1,70 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:55:25.401625 labmate-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-03-17 16:55:15.000000 labmate-0.5.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-17 16:55:15.000000 labmate-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-17 16:55:25.401625 labmate-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-17 16:55:15.000000 labmate-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:55:25.393625 labmate-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-17 16:55:15.000000 labmate-0.5.0/docs/acquisition_notebook.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:55:25.393625 labmate-0.5.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)   112640 2023-03-17 16:55:15.000000 labmate-0.5.0/docs/examples/acquisition_and_analysis_notebook.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:55:25.397625 labmate-0.5.0/docs/examples/files/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-17 16:55:15.000000 labmate-0.5.0/docs/examples/files/dummy_config1.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 16:55:15.000000 labmate-0.5.0/docs/examples/files/dummy_config2.txt
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-17 16:55:15.000000 labmate-0.5.0/docs/examples/files/init_analyse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:55:25.397625 labmate-0.5.0/docs/examples/more/
--rw-r--r--   0 runner    (1001) docker     (123)   111306 2023-03-17 16:55:15.000000 labmate-0.5.0/docs/examples/more/acquisition_and_analysis_notebook_with_magic.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-03-17 16:55:15.000000 labmate-0.5.0/docs/examples/more/h5nparray.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-03-17 16:55:15.000000 labmate-0.5.0/docs/examples/more/loop_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-17 16:55:15.000000 labmate-0.5.0/docs/examples/smart_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-03-17 16:55:15.000000 labmate-0.5.0/docs/h5nparray.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:55:25.397625 labmate-0.5.0/docs/releases/
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-03-17 16:55:15.000000 labmate-0.5.0/docs/releases/0.4.0.md
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-03-17 16:55:15.000000 labmate-0.5.0/docs/releases/0.5.0.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:55:25.397625 labmate-0.5.0/labmate/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:55:25.401625 labmate-0.5.0/labmate/acquisition/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/acquisition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/acquisition/acquisition_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11116 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/acquisition/acquisition_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/acquisition/acquisition_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11461 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/acquisition/analysis_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/acquisition/analysis_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/acquisition/lint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:55:25.401625 labmate-0.5.0/labmate/acquisition_notebook/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/acquisition_notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15227 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/acquisition_notebook/acquisition_analysis_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/acquisition_notebook/acquisition_magic_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:55:25.401625 labmate-0.5.0/labmate/attrdict/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/attrdict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/attrdict/attrdict_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/json_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:55:25.401625 labmate-0.5.0/labmate/path/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/path/path_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:55:25.401625 labmate-0.5.0/labmate/plot_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/plot_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/plot_utils/random_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/plt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:55:25.401625 labmate-0.5.0/labmate/syncdata/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/syncdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/syncdata/h5py_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20639 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/syncdata/syncdata_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:55:25.401625 labmate-0.5.0/labmate/syncdata_types/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/syncdata_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/syncdata_types/h5_np_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:55:25.401625 labmate-0.5.0/labmate/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/utils/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/utils/autoreload.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/utils/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-03-17 16:55:15.000000 labmate-0.5.0/labmate/utils/random_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 16:55:25.401625 labmate-0.5.0/labmate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-17 16:55:25.000000 labmate-0.5.0/labmate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-03-17 16:55:25.000000 labmate-0.5.0/labmate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 16:55:25.000000 labmate-0.5.0/labmate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-17 16:55:25.000000 labmate-0.5.0/labmate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-17 16:55:25.000000 labmate-0.5.0/labmate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-17 16:55:15.000000 labmate-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 16:55:25.401625 labmate-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-17 16:55:15.000000 labmate-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.060316 labmate-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-05-12 13:19:37.000000 labmate-0.6.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-12 13:19:37.000000 labmate-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-12 13:19:49.060316 labmate-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-12 13:19:37.000000 labmate-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.056316 labmate-0.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/acquisition_notebook.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.056316 labmate-0.6.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   112640 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/examples/acquisition_and_analysis_notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/examples/cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.056316 labmate-0.6.0/docs/examples/files/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/examples/files/dummy_config1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/examples/files/dummy_config2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/examples/files/dummy_config3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/examples/files/init_analyse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.056316 labmate-0.6.0/docs/examples/more/
+-rw-r--r--   0 runner    (1001) docker     (123)   111306 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/examples/more/acquisition_and_analysis_notebook_with_magic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/examples/more/h5nparray.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/examples/more/loop_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/examples/smart_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/h5nparray.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.056316 labmate-0.6.0/docs/releases/
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/releases/0.4.0.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/releases/0.5.0.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-12 13:19:37.000000 labmate-0.6.0/docs/releases/0.6.0.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.056316 labmate-0.6.0/labmate/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.060316 labmate-0.6.0/labmate/acquisition/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/acquisition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/acquisition/acquisition_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11078 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/acquisition/acquisition_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/acquisition/acquisition_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/acquisition/analysis_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/acquisition/analysis_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/acquisition/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.060316 labmate-0.6.0/labmate/acquisition_notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/acquisition_notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15313 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/acquisition_notebook/acquisition_analysis_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/acquisition_notebook/acquisition_magic_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.060316 labmate-0.6.0/labmate/attrdict/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/attrdict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/attrdict/attrdict_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.060316 labmate-0.6.0/labmate/json/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/json/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/json/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/json/open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/json_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.060316 labmate-0.6.0/labmate/path/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/path/path_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.060316 labmate-0.6.0/labmate/plot_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/plot_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/plot_utils/random_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/plt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.060316 labmate-0.6.0/labmate/syncdata/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/syncdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/syncdata/h5py_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20683 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/syncdata/syncdata_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.060316 labmate-0.6.0/labmate/syncdata_types/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/syncdata_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/syncdata_types/h5_np_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.060316 labmate-0.6.0/labmate/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/utils/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/utils/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/utils/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-12 13:19:37.000000 labmate-0.6.0/labmate/utils/random_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:19:49.060316 labmate-0.6.0/labmate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-12 13:19:49.000000 labmate-0.6.0/labmate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-12 13:19:49.000000 labmate-0.6.0/labmate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 13:19:49.000000 labmate-0.6.0/labmate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 13:19:49.000000 labmate-0.6.0/labmate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-12 13:19:49.000000 labmate-0.6.0/labmate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-12 13:19:37.000000 labmate-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 13:19:49.060316 labmate-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-12 13:19:37.000000 labmate-0.6.0/setup.py
```

### Comparing `labmate-0.5.0/LICENCE` & `labmate-0.6.0/LICENCE`

 * *Files identical despite different names*

### Comparing `labmate-0.5.0/PKG-INFO` & `labmate-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labmate
-Version: 0.5.0
+Version: 0.6.0
 Summary: Data management library to save data and plots to hdf5 files
 Home-page: https://github.com/kyrylo-gr/labmate
 Author: LKB-OMQ
 Author-email: cryo.paris.su@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `labmate-0.5.0/docs/examples/acquisition_and_analysis_notebook.ipynb` & `labmate-0.6.0/docs/examples/acquisition_and_analysis_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `labmate-0.5.0/docs/examples/files/init_analyse.py` & `labmate-0.6.0/docs/examples/files/init_analyse.py`

 * *Files identical despite different names*

### Comparing `labmate-0.5.0/docs/examples/more/acquisition_and_analysis_notebook_with_magic.ipynb` & `labmate-0.6.0/docs/examples/more/acquisition_and_analysis_notebook_with_magic.ipynb`

 * *Files identical despite different names*

### Comparing `labmate-0.5.0/docs/examples/more/h5nparray.ipynb` & `labmate-0.6.0/docs/examples/more/h5nparray.ipynb`

 * *Files identical despite different names*

### Comparing `labmate-0.5.0/docs/examples/more/loop_example.ipynb` & `labmate-0.6.0/docs/examples/more/loop_example.ipynb`

 * *Files identical despite different names*

### Comparing `labmate-0.5.0/docs/h5nparray.md` & `labmate-0.6.0/docs/h5nparray.md`

 * *Files identical despite different names*

### Comparing `labmate-0.5.0/docs/releases/0.4.0.md` & `labmate-0.6.0/docs/releases/0.4.0.md`

 * *Files identical despite different names*

### Comparing `labmate-0.5.0/docs/releases/0.5.0.md` & `labmate-0.6.0/docs/releases/0.5.0.md`

 * *Files identical despite different names*

### Comparing `labmate-0.5.0/labmate/acquisition/acquisition_data.py` & `labmate-0.6.0/labmate/acquisition/acquisition_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import os
 from typing import Dict, List, Optional, Union
 
 from ..syncdata import SyncData
-from ..utils.errors import MultiLineValueError
+from ..utils.parse import parse_str
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.WARNING)
 
 
 class NotebookAcquisitionData(SyncData):
     """It's a SyncData that has information about the configs file and the cell.
@@ -81,22 +81,51 @@
 
 
 def read_config_files(config_files: List[str]) -> Dict[str, str]:
     configs: Dict[str, str] = {}
     for config_file in config_files:
         config_file_name = os.path.basename(config_file)
         if config_file_name in configs:
-            raise MultiLineValueError(
-                """Some of the files have the same name. So it cannot
-                 be pushed into dictionary to preserve unique key""")
+            raise ValueError(
+                "Some of the files have the same name. So it cannot "
+                "be pushed into dictionary to preserve unique key")
         configs[config_file_name] = read_file(config_file)
     return configs
 
 
+def eval_config_files(configs: Dict[str, str], evals_modules: dict) -> Dict[str, str]:
+    # print(configs)
+    for file, module in evals_modules.items():
+        configs[file] = eval_config_file(configs[file], module)
+    return configs
+
+
+def eval_config_file(body, module):
+    variables = vars(module)
+    lines = body.split('\n')
+    for i, line in enumerate(lines):
+        for key, val in parse_str(line).items():
+            real_val = variables.get(key, "")
+            if (
+                    (isinstance(val, str) and
+                     isinstance(real_val, str) and
+                     real_val != val.strip('"\'')) or
+                    (isinstance(val, str) and
+                        isinstance(real_val, (float, int, complex)) and
+                        not isinstance(real_val, bool))
+            ):
+                lines[i] += f"  # value: {real_val}"
+
+                # print(f"{val}!={real_val}")
+                # print(f"{type(val)}!={type(real_val)}")
+
+    return "\n".join(lines)
+
+
 def read_file(file: str) -> str:
     if not os.path.isfile(file):
-        raise MultiLineValueError(
-            f"""Cannot read a file if it doesn't exist or it's not a file.
-             Path: {os.path.abspath(file)}""")
+        raise ValueError(
+            "Cannot read a file if it doesn't exist or it's not a file. "
+            f"Path: {os.path.abspath(file)}")
 
     with open(file, 'r', encoding="utf-8") as file_opened:
         return file_opened.read()
```

### Comparing `labmate-0.5.0/labmate/acquisition/acquisition_loop.py` & `labmate-0.6.0/labmate/acquisition/acquisition_loop.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 from typing import Any, Dict, Iterable, Iterator, List, Optional, Union, overload
 
 import numpy as np
 
 from ..syncdata import h5py_utils
 from ..syncdata_types.h5_np_array import SyncNp
 from ..syncdata.syncdata_class import SyncData
-from ..utils.errors import MultiLineValueError
 
 
 class AcquisitionLoop(SyncData):
     _level = 0
 
     def __init__(self) -> None:
         super().__init__()
         self._level = 0
         self._shape = []
         self._iteration = []
 
-    @ overload
+    @overload
     def __call__(self, **kwds) -> None:
-        """Saves the kwds.
-        Same as calling the function append_data(kwds)
-        """
+        """Save the kwds. Same as calling the function append_data(kwds)."""
 
-    @ overload
+    @overload
     def __call__(self, iterable: Iterable) -> Iterator:
-        """Given an iterable returns an iterator"""
+        """Return an iterator given an iterable."""
 
-    @ overload
+    @overload
     def __call__(self, stop: Union[int, float], /) -> Iterator:
-        """Given a stop value returns np.arange(stop)"""
+        """Return np.arange(stop) given a stop value."""
 
-    @ overload
+    @overload
     def __call__(self, start: Union[int, float], stop: Union[int, float], step: Union[int, float], /
                  ) -> Iterator:
-        """Given a start, stop and step returns np.arange(start, stop, step)"""
+        """Return np.arange(start, stop, step) given a start, stop and step."""
 
     def __call__(self, *args, iterable: Optional[Iterable] = None, **kwds) -> Optional[Iterator]:
-        """ If kwds are provided then is same as calling append_data(kwds),
-        otherwise returns iterator over iterable or np.arange(*args)
+        """Append_data or arange.
+
+        If kwds are provided then is same as calling append_data(kwds),
+        otherwise returns iterator over iterable or np.arange(*args).
         """
         if iterable is None and len(args) == 0:
             self.append(**kwds)
             return None
 
         if iterable is None:
             if isinstance(args[0], (int, float, np.int_, np.float_)):  # type: ignore
@@ -53,15 +52,15 @@
         if iterable is None:
             raise ValueError("You should provide an iterable")
 
         return self.iter(iterable)
 
     def append(self, level=None, **kwds):
         if len(kwds) == 0:
-            raise ValueError("You should provide keywords and values to save")
+            raise ValueError("You should provide keywords and values to save.")
 
         level = level if level is not None else self._level
         shape = tuple(self._shape[:self._level])
 
         iteration = tuple(self._iteration[:self._level])
         for key, value in kwds.items():
             if isinstance(value, (np.ndarray, )):
@@ -74,22 +73,22 @@
                 # print(self.data[key].shape, shape)
                 if self[key].shape == key_shape:
                     self[key][iteration] = value
                     # pass
                 else:
                     # print("app",list(i-j for i, j in zip(shape, self.data[key].shape)))
                     if len(key_shape) < len(self[key].shape):
-                        raise MultiLineValueError(
-                            f"""Object {key} hasn't the same shape as before. Now it's
-                             {key_shape[len(shape):]}, but before it was {self[key].shape[len(shape):]}""")
+                        raise ValueError(
+                            f"Object {key} hasn't the same shape as before. Now it's "
+                            f"{key_shape[len(shape):]}, but before it was {self[key].shape[len(shape):]}.")
 
                     elif len(key_shape) > len(self[key].shape):
-                        raise MultiLineValueError(
-                            f"""Object {key} cannot be save as the shape is not compatible. Before the shape was
-                            {self[key].shape}, but now it is {key_shape}""")
+                        raise ValueError(
+                            f"Object {key} cannot be save as the shape is not compatible. "
+                            f"Before the shape was {self[key].shape}, but now it is {key_shape}.")
 
                     # print(self[key].shape)
                     # print(f"{key_shape=}")
                     # print(tuple((0, i-j) for i, j in zip(
                     #             key_shape,
                     #             self[key].shape)))
                     self[key] = SyncNp(
@@ -141,15 +140,15 @@
             self._level -= 1
 
         return GenerToIter(
             loop_iter(iterable, level=level), length)
 
 
 class AcquisitionLoopOld:
-    """Acquisition loop alow to save data during for loops.
+    """Acquisition loop allow to save data during for loops.
 
     - Example 1 that saves list of squares till 10:
     ```
     sd.test_loop = loop = AcquisitionLoop()
     for i in loop(10):
         loop.append_data(x=i**2)
     ```
@@ -157,16 +156,16 @@
     - Example 2 with not direct manipulation:
     ```
     loop = AcquisitionLoop()
     for i in loop(10):
         loop.append_data(x=i**2)
     sd.update(test_loop = loop)
     ```
-
     """
+
     __filename__: Optional[str] = None
     __filekey__: Optional[str] = None
     __should_not_be_converted__ = True
     __save_on_edit__: bool = False
 
     def __init__(self):
         self.loop_shape: List[int] = []  # length of each loop level
@@ -174,35 +173,35 @@
         self.data_level = {}  # for each keyword, indicates at which loop_level it is scanned
         self._data_flatten = {}
 
     # @overload
     # def __call__(self, *arg) -> Iterator:
     #     ...
 
-    @ overload
+    @overload
     def __call__(self, **kwds) -> None:
-        """Saves the kwds.
-        Same as calling the function append_data(kwds)
-        """
+        """Save the kwds. Same as calling the function append_data(kwds)."""
 
-    @ overload
+    @overload
     def __call__(self, iterable: Iterable) -> Iterator:
-        """Given an iterable returns an iterator"""
+        """Given an iterable returns an iterator."""
 
-    @ overload
+    @overload
     def __call__(self, stop: Union[int, float], /) -> Iterator:
-        """Given a stop value returns np.arange(stop)"""
+        """Given a stop value returns np.arange(stop)."""
 
-    @ overload
+    @overload
     def __call__(self, start: Union[int, float], stop: Union[int, float], step: Union[int, float], /
                  ) -> Iterator:
-        """Given a start, stop and step returns np.arange(start, stop, step)"""
+        """Given a start, stop and step returns np.arange(start, stop, step)."""
 
     def __call__(self, *args, iterable: Optional[Iterable] = None, **kwds) -> Optional[Iterator]:
-        """ If kwds are provided then is same as calling append_data(kwds),
+        """Append_data or arange.
+
+        If kwds are provided then is same as calling append_data(kwds),
         otherwise returns iterator over iterable or np.arange(*args)
         """
         if iterable is None and len(args) == 0:
             self.append_data(**kwds)
             return None
 
         if iterable is None:
```

### Comparing `labmate-0.5.0/labmate/acquisition/acquisition_manager.py` & `labmate-0.6.0/labmate/acquisition/acquisition_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from __future__ import annotations
 import os
 
 from typing import Dict, List, NamedTuple, Optional, Union
 from ..path import Path
-# import logging
 
-from .acquisition_data import NotebookAcquisitionData, read_config_files, read_file
+from .acquisition_data import NotebookAcquisitionData, read_config_files, read_file, eval_config_files
 
 from ..utils import get_timestamp
-from ..json_utils import json_read, json_write
+from .. import json as jsn
 
 
 class AcquisitionTmpData(NamedTuple):
-    """Temporary data that stores inside temp.json"""
+    """Temporary data that stores inside temp.json."""
+
     experiment_name: str
     time_stamp: str
     configs: Dict[str, str] = {}
     directory: Optional[Union[str, Path]] = None
 
     def asdict(self):
         return self._asdict()  # pylint: disable=no-member
 
 
 class AcquisitionManager:
-    """AcquisitionManager"""
+    """AcquisitionManager."""
 
     _data_directory: Path
     config_files = []
+    config_files_eval = {}
 
     _current_acquisition = None
     _current_filepath = None
 
     _save_files = False
     _save_on_edit = True
     _init_code = None
@@ -79,66 +79,74 @@
         acquisition_tmp_data = self._acquisition_tmp_data or self.get_temp_data(self.temp_file_path)
         if acquisition_tmp_data is None:
             raise ValueError("You should create a new acquisition. It will create temp.json file.")
         return acquisition_tmp_data
 
     @acquisition_tmp_data.setter
     def acquisition_tmp_data(self, dic: AcquisitionTmpData) -> None:
-        json_write(self.temp_file_path, dic.asdict())
+        jsn.write(self.temp_file_path, dic.asdict())
         self._acquisition_tmp_data = dic
 
     def __setitem__(self, __key: str, __value) -> None:
         self.aq[__key] = __value
 
-    def set_config_file(self, filename: Union[str, List[str]]) -> AcquisitionManager:
+    def set_config_file(self, filename: Union[str, List[str]]) -> 'AcquisitionManager':
         """Set self.config_file to filename. Verify if exists.
         Only set config file for future acquisition and will not change current acquisition"""
         if isinstance(filename, str):
             filename = [filename]
 
         self.config_files = list(filename)
 
         for config_file in self.config_files:
             if not os.path.exists(config_file):
                 raise ValueError(f"Configuration file at {config_file} does not exist")
 
         return self
 
+    def set_config_evaluation_module(self, file, module):
+        if file not in self.config_files:
+            raise ValueError(
+                "Configuration file should be specified before with set_config_file function")
+        self.config_files_eval[os.path.basename(file)] = module
+
     def set_init_analyse_file(self, filename: Union[str, Path]) -> None:
         if not isinstance(filename, Path):
             filename = Path(filename)
         init = read_file(str(filename.absolute()))
         if init:
             self._init_code = init
 
-    def create_path_from_tmp_data(self, dic: AcquisitionTmpData) -> Path:
+    def create_path_from_tmp_data(self, dic: AcquisitionTmpData) -> 'Path':
         data_directory = dic.directory or self.data_directory
-        experiment_path = (Path(data_directory)/dic.experiment_name)
+        experiment_path = (Path(data_directory)/str(dic.experiment_name))
         if not experiment_path.exists():
             experiment_path.makedirs()
         if self._init_code and not os.path.exists(experiment_path/"init_analyse.py"):
             with open(experiment_path/"init_analyse.py", "w", encoding="utf-8") as file:
                 file.write(self._init_code)
         return experiment_path/f'{dic.time_stamp}__{dic.experiment_name}'
 
     @ staticmethod
     def get_temp_data(path: Path) -> Optional[AcquisitionTmpData]:
         if not os.path.exists(path):
             return None
-        return AcquisitionTmpData(**json_read(path))
+        return AcquisitionTmpData(**jsn.read(path))
 
     def new_acquisition(self,
                         name: str,
                         cell: Optional[str] = None,
                         save_on_edit: Optional[bool] = None
                         ) -> NotebookAcquisitionData:
-        """Creates a new acquisition with the given experiment name"""
+        """Create a new acquisition with the given experiment name."""
         self._current_acquisition = None
         self.cell = cell
         configs = read_config_files(self.config_files)
+        if self.config_files_eval:
+            configs = eval_config_files(configs, self.config_files_eval)
 
         dic = AcquisitionTmpData(experiment_name=name,
                                  time_stamp=get_timestamp(),
                                  configs=configs,
                                  directory=self.data_directory)
 
         self.acquisition_tmp_data = dic
@@ -184,15 +192,15 @@
             filepath=str(filepath),
             configs=configs,
             cell=cell,
             overwrite=replace,
             save_on_edit=save_on_edit,
             save_files=self._save_files)
 
-    def save_acquisition(self, **kwds) -> AcquisitionManager:
+    def save_acquisition(self, **kwds) -> 'AcquisitionManager':
         acq_data = self.current_acquisition
         if acq_data is None:
             raise ValueError("Cannot save data to acquisition as current acquisition is None. \n\
                 Possibly because you have never run `acquisition_cell(..)` or it's an old data""")
 
         acq_data.update(**kwds)
         acq_data.save_additional_info()
```

### Comparing `labmate-0.5.0/labmate/acquisition/analysis_data.py` & `labmate-0.6.0/labmate/acquisition/analysis_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 from .analysis_loop import AnalysisLoop
 
 from ..syncdata import SyncData
 from ..attrdict import AttrDict
 from ..path import Path
 from .. import utils
-from ..utils.errors import MultiLineValueError
 
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.WARNING)
 
 
 class FigureProtocol(Protocol):
     def savefig(self, fname, **kwds):
-        """Saves the figure to a file"""
+        """Save the figure to a file."""
 
 
 class AnalysisData(SyncData):
     """AnalysisManager is subclass of SyncData.
+
     It opens the filepath and immediately looks every existing keys.
     So that you can add and modify a new key, but cannot change old keys.
 
     Also if `cell` was provided, it will save it to h5 file and
     to _ANALYSIS_CELL.py file into the same directory.
 
     Use case are the same as for the SyncData except additional
@@ -34,16 +34,16 @@
 
     Example 1:
     ```
     data = AnalysisManager(filepath)
     print(data.x)
     data.fit_results = [1,2,3]
     ```
-
     """
+
     _figure_last_name = None
     _figure_saved = False
     _fig_index = 0
 
     def __init__(self,
                  filepath: Union[str, Path],
                  cell: Optional[str] = "none",
@@ -111,18 +111,19 @@
                 file.write(cell)
 
     def save_fig(self,
                  fig: Optional[FigureProtocol] = None,
                  name: Optional[Union[str, int]] = None,
                  tight_layout: bool = True,
                  **kwargs):
-        """saves the figure with the filename (...)_FIG_name
-          If name is None, use (...)_FIG1, (...)_FIG2.
-          pdf is used by default if no extension is provided in name"""
+        """Save the figure with the filename (...)_FIG_name.
 
+        If name is None, use (...)_FIG1, (...)_FIG2.
+        pdf is used by default if no extension is provided in name
+        """
         self._figure_last_name = str(name).lstrip('_') if name is not None else None
 
         fig_name = self.get_fig_name(name)
         full_fig_name = f'{self.filepath}_{fig_name}'
 
         if fig is not None:
             # if self._save_fig_inside_h5 and kwargs.get("pickle", True):
@@ -142,18 +143,20 @@
             if tight_layout:
                 plt.tight_layout()
             plt.savefig(full_fig_name, **kwargs)
 
         self._figure_saved = True
 
     def get_fig_name(self, name: Optional[Union[str, int]] = None) -> str:
-        """
+        """Get the name of the figure depending on the suffix.
+
         If name is not specified, suffix is `FIG1.pdf`, `FIG2.pdf`, etc.
         If name like `123`, the suffix is `FIG123.pdf`.
-        If name like `abc`, the suffix is `FIG_abc.pdf` """
+        If name like `abc`, the suffix is `FIG_abc.pdf`
+        """
         assert self.filepath, "You must set self.filepath before saving"
 
         if name is None:
             self._fig_index += 1
             name = f'{self._fig_index}.pdf'
         else:
             if not isinstance(name, str):
@@ -194,15 +197,19 @@
             config_files: Optional[Tuple[str, ...]] = None
     ) -> List[utils.parse.ValueForPrint]:
 
         config_data = self.parse_config(config_files=config_files)
         keys_with_values = []
         for key in keys:
             key_value, key_units, key_format = utils.parse.parse_get_format(key)
-            if key_value in config_data:
+            if key_value == "filename" or key_value == "file" or key_value == "f":
+                filename = os.path.split(self.filepath)[-1]
+                keys_with_values.append(utils.parse.ValueForPrint(
+                    key_value, filename, key_units, key_format))
+            elif key_value in config_data:
                 keys_with_values.append(utils.parse.ValueForPrint(
                     key_value, config_data[key_value], key_units, key_format))
             elif key_value in self:
                 keys_with_values.append(utils.parse.ValueForPrint(
                     key_value, self[key_value], key_units, key_format))
             else:
                 logger.warning("key %s not found and cannot be parsed", key_value)
@@ -211,16 +218,18 @@
 
     def parse_config_str(
             self,
             values: List[str],
             max_length: Optional[int] = None,
             config_files: Optional[Tuple[str, ...]] = None
     ) -> str:
-        """ Parse the configuration files.
-        Returns: key1=value1, key2=value2, ..."""
+        """Parse the configuration files.
+
+        Returns: key1=value1, key2=value2, ...
+        """
         keys_with_values = self.parse_config_values(values, config_files=config_files)
         return utils.parse.format_title(keys_with_values, max_length=max_length)
 
     def parse_config_file(self, config_file_name: str, /) -> AttrDict:
         if config_file_name in self._parsed_configs:
             return self._parsed_configs[config_file_name]
 
@@ -230,17 +239,17 @@
         if config_file_name not in self['configs']:
             original_config_name = config_file_name
             for possible_name in self['configs']:
                 if possible_name.startswith(config_file_name):
                     config_file_name = possible_name
                     break
             else:
-                raise MultiLineValueError(
-                    f"""Cannot find config with name '{config_file_name}'.
-                    Possible configs file are {tuple(self['configs'].keys())}""")
+                raise ValueError(
+                    f"Cannot find config with name '{config_file_name}'. "
+                    f"Possible configs file are {tuple(self['configs'].keys())}")
 
             if config_file_name in self._parsed_configs:
                 self._parsed_configs[original_config_name] = self._parsed_configs[config_file_name]
                 return self._parsed_configs[config_file_name]
 
         else:
             original_config_name = None
@@ -259,17 +268,17 @@
         self._default_config_files = (config_files, ) if isinstance(config_files, str) else tuple(config_files)
 
     def get_analysis_code(
             self, name: str = "default", /, update_code: bool = True) -> str:
 
         code: Optional[dict] = self.get('analysis_cells')
         if code is None:
-            raise MultiLineValueError(
-                f"""There is no field 'analysis_cells' inside the data file.
-                Possible keys are {tuple(self.keys())}""")
+            raise ValueError(
+                f"There is no field 'analysis_cells' inside the data file. "
+                f"Possible keys are {tuple(self.keys())}.")
 
         # if isinstance(code, bytes):
         #     code = code.decode()
         if name not in code:
             raise KeyError(f"Cannot get cell '{name}'. Possible cells are: {tuple(code.key())}")
 
         code_str: str = code[name]
```

### Comparing `labmate-0.5.0/labmate/acquisition/analysis_loop.py` & `labmate-0.6.0/labmate/acquisition/analysis_loop.py`

 * *Files identical despite different names*

### Comparing `labmate-0.5.0/labmate/acquisition/lint.py` & `labmate-0.6.0/labmate/acquisition/lint.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,84 @@
 import ast
-from typing import Optional, Tuple
+from typing import List, Optional, Tuple
+
+
+def get_args_from_list(args: List[ast.arg]):
+    return [arg.arg for arg in args]
 
 
 class NameVisitor(ast.NodeVisitor):
     parent = None
+    dont_parse = None
 
     def __init__(self, ignore_var: Optional[set] = None):
         self.local_vars = ignore_var.copy() if ignore_var else set()
         self.builtins = set(__builtins__.keys())
         self.external_vars = set()
         super().__init__()
 
-    def visit(self, node, parent=None):
+    def visit(self, node, parent=None, dont_parse=None):
         node.parent = parent  # type: ignore
-        # self.parent = parent
-        if isinstance(node, (ast.Import, ast.ImportFrom)):
+        node.dont_parse = dont_parse  # type: ignore
+
+        if (isinstance(node, ast.Call) and
+                isinstance(node.func, ast.Attribute) and
+                node.func.attr == "save_acquisition"):
+            node.dont_parse = []  # type: ignore
+            return
+
+        if isinstance(node, ast.FunctionDef):
+            variables = (
+                get_args_from_list(node.args.posonlyargs) +
+                get_args_from_list(node.args.args) +
+                get_args_from_list(node.args.kwonlyargs)
+            )
+            if node.args.kwarg:
+                variables += node.args.kwarg.arg
+            node.dont_parse = variables  # type: ignore
+
+        elif isinstance(node, (ast.Import, ast.ImportFrom)):
             for name in node.names:
                 var = name.asname or name.name
                 if var != "*":
                     self.local_vars.add(var)
-        if isinstance(node, ast.Name):
-            # print(node.id, node.ctx)
-            # print_node(child)
+
+        elif isinstance(node, ast.Name):
             if isinstance(node.ctx, ast.Store):
-                self.local_vars.add(node.id)
+                if node.dont_parse is None:  # type: ignore
+                    self.local_vars.add(node.id)
+                else:
+                    node.dont_parse.append(node.id)  # type: ignore
+
             if (isinstance(node.ctx, ast.Load) and
                     node.id not in self.local_vars and
                     node.id not in self.builtins):
-                if not (
-                    isinstance(node.parent, ast.keyword) and  # type: ignore
-                    isinstance(node.parent.parent, ast.Call) and  # type: ignore
-                    node.parent.parent.func.attr == "save_acquisition"  # type: ignore
-                ):
+                if (node.dont_parse is None) or (node.id not in node.dont_parse):  # type: ignore
                     self.external_vars.add(node.id)
-                # print(ast.dump(node.parent.parent, indent=4))
 
         self.generic_visit(node)
 
     def generic_visit(self, node):
         for _, value in ast.iter_fields(node):
             if isinstance(value, list):
                 for item in value:
                     if isinstance(item, ast.AST):
-                        self.visit(item, parent=node)
+                        self.visit(item, parent=node,
+                                   dont_parse=node.dont_parse)  # type: ignore
             elif isinstance(value, ast.AST):
-                self.visit(value, parent=node)
+                self.visit(value, parent=node,
+                           dont_parse=node.dont_parse)  # type: ignore
 
 
 def find_variables(node, ignore_var: Optional[set] = None) -> Tuple[set, set]:
-    """Walk through ast.node and find the variable that was never declared
-    inside this node, but used.
+    """Walk through ast.node and find the variable that was never declared inside this node, but used.
+
     Variables from ingore_var set is allowed external variables to use.
-    Returns (local_vars, external_vars)"""
+    Returns (local_vars, external_vars)
+    """
     visitor = NameVisitor(ignore_var)
     visitor.visit(node)
     return visitor.local_vars, visitor.external_vars
 
 
 def find_variables_from_code(code, ignore_var: Optional[set] = None) -> Tuple[set, set]:
     code = code.split("\n")
```

### Comparing `labmate-0.5.0/labmate/acquisition_notebook/acquisition_analysis_manager.py` & `labmate-0.6.0/labmate/acquisition_notebook/acquisition_analysis_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-from __future__ import annotations
-
+from typing import Any, Callable, Iterable, List, Literal, Optional, Tuple, Union, TYPE_CHECKING
 import os
 import logging
 import time
-from typing import Any, Callable, Iterable, List, Literal, Optional, Tuple, Union
-from ..utils import lstrip_int
-from ..acquisition import AcquisitionManager, AnalysisData, FigureProtocol
-from ..attrdict import AttrDict
+from ..acquisition import AcquisitionManager, AnalysisData
 from .. import utils
-from ..path import Path
-from ..utils.errors import MultiLineValueError
+if TYPE_CHECKING:
+    from ..acquisition import FigureProtocol
+    from ..attrdict import AttrDict
+    from ..path import Path
 
 # from ..syncdata import SyncData
 
 logging.basicConfig(format='%(levelname)s:%(message)s', level=logging.INFO)
 logger = logging.getLogger(__name__)
 handler = logging.StreamHandler()
 formatter = logging.Formatter('%(levelname)s:%(message)s')
@@ -22,16 +20,15 @@
 logger.setLevel(logging.INFO)
 logger.propagate = False
 
 _CallableWithNoArgs = Callable[[], Any]
 
 
 class AcquisitionAnalysisManager(AcquisitionManager):
-    """
-    AcquisitionAnalysisManager
+    """AcquisitionAnalysisManager.
 
     # Init:
     ```
     aqm = AcquisitionAnalysisManager("tmp_data/", use_magic=False, save_files=False)
     aqm.set_config_file("configuration.py")
     ```
     # acquisition_cell:
@@ -46,14 +43,15 @@
     aqm.analysis_cell()
     ...
     plt.plot(aqm.d.x, aqm.d.y)
     aqm.save_fig()
     ```
 
     """
+
     _analysis_data: Optional[AnalysisData] = None
     _analysis_cell_str = None
     _is_old_data = False
     _last_fig_name = None
     _default_config_files: Tuple[str, ...] = tuple()
     _acquisition_started = 0
     _linting_external_vars = None
@@ -132,17 +130,17 @@
 
     @property
     def d(self):  # pylint: disable=invalid-name
         return self.data
 
     def save_fig_only(
             self,
-            fig: Optional[FigureProtocol] = None,
+            fig: Optional['FigureProtocol'] = None,
             name: Optional[Union[str, int]] = None, **kwds
-    ) -> AcquisitionAnalysisManager:
+    ) -> 'AcquisitionAnalysisManager':
         """
         Save the fig as a file.
 
         Args:
             fig (Figure, optional): Figure that should be saved.
                 Figure could be any class with function save_fig implemented. Defaults to None.
 
@@ -157,106 +155,111 @@
         self.data.save_fig(fig=fig, name=name, **kwds)
         return self
 
     def save_analysis_cell(
             self,
             name: Optional[Union[str, int]] = None,
             cell: Optional[Union[str, Literal['none']]] = None
-    ) -> AcquisitionAnalysisManager:
+    ) -> 'AcquisitionAnalysisManager':
         if name is None:
             name = self.data.figure_last_name
 
         if name is not None:
             name = str(name)
 
         cell = cell or self._analysis_cell_str
 
         self.data.save_analysis_cell(cell=cell, cell_name=name)
 
         return self
 
     def save_fig(
             self,
-            fig: Optional[FigureProtocol] = None,
+            fig: Optional['FigureProtocol'] = None,
             name: Optional[Union[str, int]] = None,
             cell: Optional[str] = None,
             **kwds
-    ) -> AcquisitionAnalysisManager:
+    ) -> 'AcquisitionAnalysisManager':
 
         self.save_fig_only(fig=fig, name=name, **kwds)
         self.save_analysis_cell(name=name, cell=cell)
         return self
 
     def __setitem__(self, __key: str, __value: Any) -> None:
         if self._analysis_data is not None:
-            raise MultiLineValueError("This is the way to save acquisition data. But analysis data was loaded.\
-                So you possibly run it inside analysis_cell")
+            raise ValueError(
+                "This is the way to save acquisition data. But analysis data was loaded."
+                "So you possibly run it inside analysis_cell")
         acq_data = self.current_acquisition
         if acq_data is None:
-            raise MultiLineValueError("Cannot save data to acquisition as current acquisition is None.\
-                Possibly because you have never run `acquisition_cell(..)` or it's an old data""")
-        acq_data.update({__key: __value})
+            raise ValueError(
+                "Cannot save data to acquisition as current acquisition is None."
+                "Possibly because you have never run `acquisition_cell(..)` or it's an old data")
+        acq_data[__key] = __value
 
-    def save_acquisition(self, **kwds) -> AcquisitionAnalysisManager:
+    def save_acquisition(self, **kwds) -> 'AcquisitionAnalysisManager':
         acquisition_finished = time.time()
         kwds.update({"info": {"acquisition_duration": acquisition_finished-self._acquisition_started}})
         super().save_acquisition(**kwds)
         self.load_analysis_data()
         return self
 
     def load_analysis_data(self, filepath: Optional[str] = None):
         filepath = filepath or str(self.current_filepath)
 
         if not os.path.exists(filepath if filepath.endswith('.h5') else filepath + '.h5'):
-            raise MultiLineValueError(
-                f"""Cannot load data from {filepath}. As file does not exist.""")
+            raise ValueError(
+                f"Cannot load data from {filepath}. As file does not exist.")
 
         self._analysis_data = AnalysisData(
             filepath=filepath,
             save_files=self._save_files, save_on_edit=self._save_on_edit_analysis,
             save_fig_inside_h5=self._save_fig_inside_h5)
 
         self._analysis_data.unlock_data('useful').update(**{'useful': True}).lock_data('useful')
 
         if self._save_on_edit_analysis is False:
             self._analysis_data.save()
 
+        if self._default_config_files:
+            self._analysis_data.set_default_config_files(self._default_config_files)
+
         return self._analysis_data
 
     def acquisition_cell(
             self,
             name: str,
             cell: Optional[str] = None,
             prerun: Optional[Union[_CallableWithNoArgs, List[_CallableWithNoArgs]]] = None,
             save_on_edit: Optional[bool] = None
-    ) -> AcquisitionAnalysisManager:
+    ) -> 'AcquisitionAnalysisManager':
         self._analysis_cell_str = None
         self._analysis_data = None
         self._is_old_data = False
         self._acquisition_started = time.time()
 
         cell = cell or get_current_cell(self.shell)
 
         self.new_acquisition(name=name, cell=cell, save_on_edit=save_on_edit)
 
-        logger.info(os.path.basename(self.current_filepath))
+        logger.info(self.current_filepath.basename)
 
         utils.run_functions(self._acquisition_cell_prerun_hook)
         utils.run_functions(prerun)
 
         return self
 
     def analysis_cell(
             self,
-            filename: Optional[Union[str, Path]] = None, *,
+            filename: Optional[Union[str, 'Path']] = None, *,
             acquisition_name=None,
             cell: Optional[str] = None,
-            filepath: Optional[Union[str, Path]] = None,
+            filepath: Optional[Union[str, 'Path']] = None,
             prerun: Optional[Union[_CallableWithNoArgs, List[_CallableWithNoArgs]]] = None,
-    ) -> AcquisitionAnalysisManager:
+    ) -> 'AcquisitionAnalysisManager':
         # self.shell.get_local_scope(1)['result'].info.raw_cell  # type: ignore
 
         self._analysis_cell_str = cell or get_current_cell(self.shell)
         if filename or filepath:  # getting old data
             self._is_old_data = True
             if self.shell is not None:
                 try:
@@ -276,27 +279,27 @@
             if acquisition_name is not None:
                 import re
                 if (
                     len(acquisition_name) == 0 or
                     (acquisition_name[0] != r"^" and acquisition_name != self.current_experiment_name) or
                     (acquisition_name[0] == r"^" and re.match(acquisition_name, self.current_experiment_name) is None)
                 ):
-                    raise MultiLineValueError(
-                        f"""current acquisition ('{self.current_experiment_name}')
-                         isn't the one expected ('{acquisition_name}') for this analysis""")
+                    raise ValueError(
+                        f"Current acquisition ('{self.current_experiment_name}') "
+                        f"isn't the one expected ('{acquisition_name}') for this analysis")
 
             filename = str(self.current_filepath)  # without h5
         logger.info(os.path.basename(filename))
 
         if not self._is_old_data and self.shell is not None:
-            if ('acquisition_cell' in self.shell.last_execution_result.info.raw_cell and
+            if ('acquisition_cell(' in self.shell.last_execution_result.info.raw_cell and
                     not self.shell.last_execution_result.success):
                 raise ChildProcessError(
-                    """Last executed cell was probably an `acquisition_cell` and failed to run.
-                    Check if everything is ok and executive again""")
+                    "Last executed cell was probably an `acquisition_cell` and failed to run. "
+                    "Check if everything is ok and executive again")
 
         if os.path.exists(filename + '.h5'):
             self.load_analysis_data(filename)
         else:
             if self._is_old_data:
                 raise ValueError(f"Cannot load data from {filename}")
             self._analysis_data = None
@@ -329,30 +332,30 @@
 
     def get_full_filename(self, filename: str) -> str:
         if '/' in filename or '\\' in filename:
             return filename
 
         filename = (filename.rsplit('.h5', 1)[0]) if filename.endswith('.h5') else filename
 
-        name_with_prefix = lstrip_int(filename)
+        name_with_prefix = utils.lstrip_int(filename)
         if name_with_prefix:
             suffix = name_with_prefix[1]
             return os.path.join(self.data_directory, suffix, filename)
         return filename
 
-    def parse_config_file(self, config_file_name: str, /) -> AttrDict:
+    def parse_config_file(self, config_file_name: str, /) -> 'AttrDict':
         return self.data.parse_config_file(config_file_name)
 
     def parse_config(
             self,
-            config_files: Optional[Tuple[str, ...]] = None) -> AttrDict:
+            config_files: Optional[Tuple[str, ...]] = None) -> 'AttrDict':
         return self.data.parse_config(config_files=(config_files or self._default_config_files))
 
     @property
-    def cfg(self) -> AttrDict:
+    def cfg(self) -> 'AttrDict':
         return self.parse_config()
 
     def parse_config_str(
         self,
         values: List[str], /,
         max_length: Optional[int] = None,
     ) -> str:
```

### Comparing `labmate-0.5.0/labmate/acquisition_notebook/acquisition_magic_class.py` & `labmate-0.6.0/labmate/acquisition_notebook/acquisition_magic_class.py`

 * *Files identical despite different names*

### Comparing `labmate-0.5.0/labmate/json_utils.py` & `labmate-0.6.0/labmate/json_utils.py`

 * *Files identical despite different names*

### Comparing `labmate-0.5.0/labmate/plt.py` & `labmate-0.6.0/labmate/plt.py`

 * *Files identical despite different names*

### Comparing `labmate-0.5.0/labmate/syncdata/h5py_utils.py` & `labmate-0.6.0/labmate/syncdata/h5py_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import os
 import h5py
 from typing import Dict, Literal, Optional, Protocol, Set, Union
+from ..utils.errors import FileLockedError
 
 import numpy as np
 
 
 class ClassWithAsdict(Protocol):
     """Any class with predefined `_asdict` attribute.
     `_asdict` class should return a dictionary with only list and dict.
@@ -27,18 +28,14 @@
     """Any class with predefined `asarray` attribute.
     `asarray` class should return a np.ndarray."""
 
     def asarray(self) -> Union[np.ndarray, list]:
         ...
 
 
-class FileLockedError(Exception):
-    """Exception raised when a file is locked"""
-
-
 class LockFile:
     def __init__(self, filename):
         self.lock_filename = os.path.splitext(filename)[0] + ".lock"
 
     def __enter__(self):
         if os.path.exists(self.lock_filename):
             raise FileLockedError("File locked and cannot be opened in write mode")
@@ -194,15 +191,15 @@
     if additional_info:
         for key, value in additional_info.items():
             dict_str = dict_str.replace(f'"{key}":', f'"{key}"{value}:')
     return dict_str
 
 
 def dict_to_json_format_str(data: dict) -> str:
-    """" Outputs a dictionary structure """
+    """Output a dictionary structure."""
     return json.dumps(data, sort_keys=True, indent=4)
 
 
 def get_dict_structure(data: dict, level: int = 3) -> dict:
     structure = {}
 
     for k, v in data.items():
```

### Comparing `labmate-0.5.0/labmate/syncdata/syncdata_class.py` & `labmate-0.6.0/labmate/syncdata/syncdata_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+from typing import Any, Dict, Iterable, Optional, Set, TypeVar, Union, overload
 import logging
 import os
 from pathlib import Path
-from typing import Any, Dict, Iterable, Optional, Set, TypeVar, Union, overload
+from functools import wraps
 from . import h5py_utils
-from ..utils.errors import MultiLineValueError
-# from .h5_np_array import H5NpArray
 
 
 def editing(func):
-    """If a function changes the data it should be saved. It's a wrapper for such function"""
-
+    """If a function changes the data it should be saved.
+    It's a wrapper for such function.
+    """
+    @wraps(func)
     def run_func_and_clean_precalculated_results(self, *args, **kwargs):
         self._last_data_saved = False  # pylint: disable=W0212
         res = func(self, *args, **kwargs)
         self._clean_precalculated_results()  # pylint: disable=W0212
         if self._save_on_edit:  # pylint: disable=W0212
             self.save(just_update=True)
         return res
@@ -21,36 +22,38 @@
     return run_func_and_clean_precalculated_results
 
 
 _T = TypeVar("_T")
 
 
 class NotLoaded(object):
-    """Internal class for data that has not been loaded yet"""
+    """Internal class for data that has not been loaded yet."""
 
     def __init__(self):
         pass
 
     def __str__(self) -> str:
         return """This key is not loaded. If you see this message,
                 it means that you accessed the key not via SyncData object"""
 
     def __repr__(self) -> str:
         return """This key is not loaded"""
 
 
 class SyncData:
-    """
+    """Dict that is synchronized with .h5 file.
+
     This object is obtained by loading a dataset contained in a .h5 file.
     Datasets can be obtained as in a dictionary: e.g.
     data[freqs]
 
     This class should not contain any not local attributes.
     Look in __setattr__() to see why it would not work.
     """
+
     _repr: Optional[str] = None
     _default_attr = ['get', 'items', 'keys', 'pop', 'update', 'values', 'save']
     _last_data_saved: bool = False
     _filepath: Optional[str] = None
     _read_only: Union[bool, Set[str]]
     _raise_file_locked_error: bool = False
     _retry_on_file_locked_error: int = 5
@@ -63,15 +66,15 @@
                  filepath: Optional[Union[str, Path]] = None,
                  save_on_edit: bool = False,
                  read_only: Optional[Union[bool, Set[str]]] = None,
                  overwrite: Optional[bool] = None,
                  data: Optional[dict] = None,
                  open_on_init: Optional[bool] = None,
                  **kwds):
-        """_summary_
+        """SyncData.
 
         Args:
             filepath_or_data (str|dict, optional): either filepath, either data as dict.
             filepath (str|Path, optional): filepath to load. Defaults to None.
             save_on_edit (bool, optional): do you what to save file every time it edited. Defaults to False.
             read_only (bool, optional): opens file in read_only mode, i.e. it cannot be modified.
                 Defaults to (save_on_edit is False && overwrite is False) and filepath is set.
@@ -118,19 +121,18 @@
             filepath = filepath if filepath.endswith('.h5') else filepath + '.h5'
 
             if (overwrite or save_on_edit) and read_only:
                 raise ValueError("""Cannot open file in read_only mode and overwrite it.""")
 
             if os.path.exists(filepath):
                 if overwrite is None and not read_only:
-                    raise MultiLineValueError(
-                        """File with the same name already exists. So you
-                         should explicitly provide what to do with it. Set `overwrite=True`
-                         to replace file. Set `overwrite=False` if you want to open existing
-                         file and work with it.""")
+                    raise ValueError(
+                        "File with the same name already exists. So you should explicitly "
+                        "provide what to do with it. Set `overwrite=True` to replace file. "
+                        "Set `overwrite=False` if you want to open existing file and work with it.")
 
                 if overwrite and not read_only:
                     os.remove(filepath)
 
                 if read_only or (not read_only and not overwrite):
                     if self._open_on_init:
                         self._load_from_h5(filepath)
@@ -240,30 +242,30 @@
         # self.pull(auto=True)
         if key not in self._unopened_keys:
             self._data.pop(key)
             return self
 
     @overload
     def get_dict(self, __key: str) -> Optional[Any]:
-        """Default value by default is None"""
+        """Return element as a dict. Return None if not found."""
 
     @overload
     def get_dict(self, __key: str, __default: _T) -> Union[Any, _T]:
-        """With default value provided"""
+        """With default value provided."""
 
     def get_dict(self, key: str, default: Optional[Any] = None):
         return self.__get_data__(key, default)
 
     @overload
     def get(self, __key: str) -> Optional[Any]:
-        """Default value by default is None"""
+        """Return element as a SyncData class if it's dict. Return None if not found."""
 
     @overload
     def get(self, __key: str, __default: _T) -> Union[Any, _T]:
-        """With default value provided"""
+        """With default value provided."""
 
     def get(self, key: str, default: Optional[Any] = None):
         data = self.__get_data__(key, default)
         if isinstance(data, dict) and data:
             return SyncData(filepath=self._filepath, data=data, key_prefix=key)
         return data
 
@@ -287,27 +289,27 @@
         self.__add_key(__key)
         __value = h5py_utils.transform_to_possible_formats(__value)
 
         if self._read_only is not True:
             if hasattr(__value, "save"):
                 self._classes_should_be_saved_internally.add(__key)
 
-            if hasattr(__value, "__init__filepath__"):
+            if hasattr(__value, "__init__filepath__") and self._filepath:
                 if self._filepath is None:
                     raise ValueError("Cannot run __init__filepath__ with file unspecified")
                 key = __key if self._key_prefix is None else f"{self._key_prefix}/{__key}"
                 __value.__init__filepath__(  # type: ignore
                     filepath=self._filepath, filekey=key, save_on_edit=self._save_on_edit)
         self.__set_data__(__key, __value)
 
     def __delitem__(self, key: str):
         self.pop(key)
 
     def __getattr__(self, __name: str):
-        """Will be called if __getattribute__ does not work"""
+        """Call if __getattribute__ does not work."""
         if len(__name) > 1 and __name[0] == 'i' and \
                 __name[1:].isdigit() and __name not in self:
             __name = __name[1:]
         if __name in self:
             data = self.get(__name)
             # if isinstance(data, dict) and data:
             #     return SyncData(filepath=self._filepath, data=data, key_prefix=__name)
@@ -326,19 +328,19 @@
     def __delattr__(self, __name: str) -> None:
         if __name in self.keys():
             return self.__delitem__(__name)
         return object.__delattr__(self, __name)
 
     @overload
     def __get_data__(self, __key: str) -> Optional[None]:
-        """Return None if the data doesn't contain key"""
+        """Return None if the data doesn't contain key."""
 
     @overload
     def __get_data__(self, __key: str, __default: _T) -> Union[Any, _T]:
-        """Return default value if the data doesn't contain key"""
+        """Return default value if the data doesn't contain key."""
 
     def __get_data__(self, __key: str, __default: Optional[Any] = None):
         if __key in self._unopened_keys:
             self._load_from_h5(key=__key)
         data = self._data.get(__key, __default)
         if isinstance(data, NotLoaded):
             self._load_from_h5(key=__key)
@@ -471,16 +473,15 @@
                 async_utils.sleep(1)
 
         raise h5py_utils.FileLockedError(
             f"Even after {self._retry_on_file_locked_error} data was not saved")
 
     @staticmethod
     def _check_if_filepath_was_set(filepath: Optional[str], filepath2: Optional[str]) -> str:
-        """
-        Returns path to the file with filename, but without extension."""
+        """Return path to the file with filename, but without extension."""
         filepath = filepath or filepath2
         if filepath is None:
             raise ValueError("Should provide filepath or set self.filepath before saving")
         filepath = (filepath.rsplit('.h5', 1)[0]) if filepath.endswith('.h5') else filepath
         return filepath
 
     @property
```

### Comparing `labmate-0.5.0/labmate/syncdata_types/h5_np_array.py` & `labmate-0.6.0/labmate/syncdata_types/h5_np_array.py`

 * *Files identical despite different names*

### Comparing `labmate-0.5.0/labmate/utils/parse.py` & `labmate-0.6.0/labmate/utils/parse.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 from typing import Any, Dict, List, NamedTuple, Optional, Tuple, Union
 
 
 def parse_str(file: str, /) -> Dict[str, Union[str, int, float]]:
-    """Parsing a str.
+    """Parse strings.
     Return a dictionary of int or float if conversion is possible otherwise str"""
     parsed_values = {}
     for line in file.split('\n'):
         if len(line) == 0 or not line[0].isalpha() or '=' not in line:
             continue
         param, value = line.split('=')[:2]
-        value = value.split('#')[0].replace("_", "").strip()
+
+        if "# value: " in value:
+            value = value[value.find("# value: ") + 9:]
+
+        value = value.split('#')[0].strip()
+        value_without_underscores = value.replace("_", "")
+
         try:
-            if value.isdigit() or (value[0] == '-' and value[1:].isdigit()):
+            if len(value_without_underscores) == 0:
+                pass
+            elif value_without_underscores.isdigit() or \
+                    (value_without_underscores[0] == '-' and value[1:].isdigit()):
                 value = int(value)
-            elif value.replace('.', '').isdigit() or \
-                    (value[0] == '-' and value[1:].replace('.', '').isdigit()):
+            elif value_without_underscores.replace('.', '').isdigit() or \
+                    (value[0] == '-' and value_without_underscores[1:].replace('.', '').isdigit()):
                 value = float(value)
             elif (value[0].isdigit() or (value[0] == "-" and value[1].isdigit())) \
                     and value[-1].isdigit() and 'e' in value:
                 value = float(value)
         except ValueError:
             pass
```

### Comparing `labmate-0.5.0/labmate/utils/random_utils.py` & `labmate-0.6.0/labmate/utils/random_utils.py`

 * *Files identical despite different names*

### Comparing `labmate-0.5.0/labmate.egg-info/PKG-INFO` & `labmate-0.6.0/labmate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labmate
-Version: 0.5.0
+Version: 0.6.0
 Summary: Data management library to save data and plots to hdf5 files
 Home-page: https://github.com/kyrylo-gr/labmate
 Author: LKB-OMQ
 Author-email: cryo.paris.su@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `labmate-0.5.0/labmate.egg-info/SOURCES.txt` & `labmate-0.6.0/labmate.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 docs/acquisition_notebook.md
 docs/h5nparray.md
 docs/examples/acquisition_and_analysis_notebook.ipynb
+docs/examples/cfg.py
 docs/examples/smart_import.py
 docs/examples/files/dummy_config1.txt
 docs/examples/files/dummy_config2.txt
+docs/examples/files/dummy_config3.py
 docs/examples/files/init_analyse.py
 docs/examples/more/acquisition_and_analysis_notebook_with_magic.ipynb
 docs/examples/more/h5nparray.ipynb
 docs/examples/more/loop_example.ipynb
 docs/releases/0.4.0.md
 docs/releases/0.5.0.md
+docs/releases/0.6.0.md
 labmate/__init__.py
 labmate/json_utils.py
 labmate/plt.py
 labmate.egg-info/PKG-INFO
 labmate.egg-info/SOURCES.txt
 labmate.egg-info/dependency_links.txt
 labmate.egg-info/requires.txt
@@ -31,14 +34,18 @@
 labmate/acquisition/analysis_loop.py
 labmate/acquisition/lint.py
 labmate/acquisition_notebook/__init__.py
 labmate/acquisition_notebook/acquisition_analysis_manager.py
 labmate/acquisition_notebook/acquisition_magic_class.py
 labmate/attrdict/__init__.py
 labmate/attrdict/attrdict_class.py
+labmate/json/__init__.py
+labmate/json/decoders.py
+labmate/json/encoders.py
+labmate/json/open.py
 labmate/path/__init__.py
 labmate/path/path_class.py
 labmate/plot_utils/__init__.py
 labmate/plot_utils/random_utils.py
 labmate/syncdata/__init__.py
 labmate/syncdata/h5py_utils.py
 labmate/syncdata/syncdata_class.py
```

### Comparing `labmate-0.5.0/setup.py` & `labmate-0.6.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+"""Import Labmate."""
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='labmate',
-    version="0.5.0",
+    version="0.6.0",
     author="LKB-OMQ",
     author_email="cryo.paris.su@gmail.com",
     description="Data management library to save data and plots to hdf5 files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kyrylo-gr/labmate",
     packages=setuptools.find_packages(exclude=['tests', 'tests.*']),
```


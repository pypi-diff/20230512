# Comparing `tmp/glue-astronomy-0.7.0.tar.gz` & `tmp/glue-astronomy-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue-astronomy-0.7.0.tar", last modified: Thu Mar  2 13:24:47 2023, max compression
+gzip compressed data, was "glue-astronomy-0.8.0.tar", last modified: Thu May 11 21:54:47 2023, max compression
```

## Comparing `glue-astronomy-0.7.0.tar` & `glue-astronomy-0.8.0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:24:47.069899 glue-astronomy-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:24:47.061899 glue-astronomy-0.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:24:47.061899 glue-astronomy-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/.github/workflows/update-changelog.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-03-02 13:24:47.069899 glue-astronomy-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/RELEASE.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:24:47.061899 glue-astronomy-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/docs/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/docs/data_loaders.rst
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/docs/translators.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:24:47.065899 glue-astronomy-0.7.0/glue_astronomy/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:24:47.065899 glue-astronomy-0.7.0/glue_astronomy/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:24:47.065899 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/spectral_cube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:24:47.065899 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:24:47.065899 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:24:47.065899 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:24:47.065899 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/table.dat
--rw-r--r--   0 runner    (1001) docker     (123)    98816 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/table.f0
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/table.info
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/table.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:24:47.069899 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/table.dat
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/table.f0
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/table.f0_TSM0
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/table.info
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/table.lock
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/table.dat
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/table.f0
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/table.f0_TSM0
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/table.info
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/table.lock
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_4d.fits
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_4d_fullstokes.fits
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/test_spectral_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/spectral_coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:24:47.069899 glue-astronomy-0.7.0/glue_astronomy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/tests/test_spectral_coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:24:47.069899 glue-astronomy-0.7.0/glue_astronomy/translators/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/translators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/translators/nddata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/translators/regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/translators/spectral_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/translators/spectrum1d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:24:47.069899 glue-astronomy-0.7.0/glue_astronomy/translators/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/translators/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/translators/tests/test_nddata.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/translators/tests/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/translators/tests/test_spectral_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/translators/tests/test_spectrum1d.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/translators/tests/test_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/glue_astronomy/translators/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-02 13:24:46.000000 glue-astronomy-0.7.0/glue_astronomy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:24:47.065899 glue-astronomy-0.7.0/glue_astronomy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-03-02 13:24:47.000000 glue-astronomy-0.7.0/glue_astronomy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-03-02 13:24:47.000000 glue-astronomy-0.7.0/glue_astronomy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 13:24:47.000000 glue-astronomy-0.7.0/glue_astronomy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-02 13:24:47.000000 glue-astronomy-0.7.0/glue_astronomy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 13:24:47.000000 glue-astronomy-0.7.0/glue_astronomy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-02 13:24:47.000000 glue-astronomy-0.7.0/glue_astronomy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-02 13:24:47.000000 glue-astronomy-0.7.0/glue_astronomy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-03-02 13:24:47.069899 glue-astronomy-0.7.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-03-02 13:24:28.000000 glue-astronomy-0.7.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.744903 glue-astronomy-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.740903 glue-astronomy-0.8.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.740903 glue-astronomy-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/.github/workflows/update-changelog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-11 21:54:47.744903 glue-astronomy-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/RELEASE.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.740903 glue-astronomy-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/docs/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/docs/data_loaders.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/docs/translators.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.740903 glue-astronomy-0.8.0/glue_astronomy/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.740903 glue-astronomy-0.8.0/glue_astronomy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.740903 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/spectral_cube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.740903 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.740903 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.740903 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.744903 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/table.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    98816 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/table.f0
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/table.info
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/table.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.744903 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/table.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/table.f0
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/table.f0_TSM0
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/table.info
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/table.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/table.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/table.f0
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/table.f0_TSM0
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/table.info
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/table.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_4d.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_4d_fullstokes.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/test_spectral_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/spectral_coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.744903 glue-astronomy-0.8.0/glue_astronomy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/tests/test_spectral_coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.744903 glue-astronomy-0.8.0/glue_astronomy/translators/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/translators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/translators/nddata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/translators/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/translators/spectral_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/translators/spectrum1d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.744903 glue-astronomy-0.8.0/glue_astronomy/translators/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/translators/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/translators/tests/test_nddata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21270 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/translators/tests/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/translators/tests/test_spectral_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/translators/tests/test_spectrum1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/translators/tests/test_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/glue_astronomy/translators/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-11 21:54:47.000000 glue-astronomy-0.8.0/glue_astronomy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:54:47.740903 glue-astronomy-0.8.0/glue_astronomy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-11 21:54:47.000000 glue-astronomy-0.8.0/glue_astronomy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-11 21:54:47.000000 glue-astronomy-0.8.0/glue_astronomy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 21:54:47.000000 glue-astronomy-0.8.0/glue_astronomy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-11 21:54:47.000000 glue-astronomy-0.8.0/glue_astronomy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 21:54:47.000000 glue-astronomy-0.8.0/glue_astronomy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-11 21:54:47.000000 glue-astronomy-0.8.0/glue_astronomy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 21:54:47.000000 glue-astronomy-0.8.0/glue_astronomy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-11 21:54:47.744903 glue-astronomy-0.8.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-11 21:54:30.000000 glue-astronomy-0.8.0/tox.ini
```

### Comparing `glue-astronomy-0.7.0/.github/workflows/main.yml` & `glue-astronomy-0.8.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/.github/workflows/update-changelog.yaml` & `glue-astronomy-0.8.0/.github/workflows/update-changelog.yaml`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/.gitignore` & `glue-astronomy-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/CHANGES.md` & `glue-astronomy-0.8.0/CHANGES.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 # Full changelog
 
+## v0.7.0 - 2023-03-02
+
+<!-- Release notes generated using configuration in .github/release.yml at main -->
+### What's Changed
+
+#### New Features
+
+- Adding support for uncertainty extraction to NDDataArray by @bmorris3 in https://github.com/glue-viz/glue-astronomy/pull/86
+
+#### Bug Fixes
+
+- Fix world_axis_units for SpectralCoordinates by @astrofrog in https://github.com/glue-viz/glue-astronomy/pull/87
+
+**Full Changelog**: https://github.com/glue-viz/glue-astronomy/compare/v0.6.1...v0.7.0
+
 ## v0.6.1 - 2023-01-31
 
 <!-- Release notes generated using configuration in .github/release.yml at main -->
 ### What's Changed
 
 #### Bug Fixes
```

### Comparing `glue-astronomy-0.7.0/LICENSE` & `glue-astronomy-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/PKG-INFO` & `glue-astronomy-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-astronomy
-Version: 0.7.0
+Version: 0.8.0
 Summary: Astronomy-specific plugins for glue
 Home-page: https://github.com/glue-viz/glue-astronomy
 Author: Thomas Robitaille
 Author-email: glue.viz@gmail.com
 License: BSD 3-Clause License
 Provides: glue_astronomy
 Requires-Python: >=3.8
```

### Comparing `glue-astronomy-0.7.0/README.rst` & `glue-astronomy-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/RELEASE.rst` & `glue-astronomy-0.8.0/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/docs/Makefile` & `glue-astronomy-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/docs/conf.py` & `glue-astronomy-0.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/docs/data_loaders.rst` & `glue-astronomy-0.8.0/docs/data_loaders.rst`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/docs/translators.rst` & `glue-astronomy-0.8.0/docs/translators.rst`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/spectral_cube.py` & `glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/spectral_cube.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.fits` & `glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.fits`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/table.dat` & `glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/table.dat`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/table.f0` & `glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/logtable/table.f0`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/table.dat` & `glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/mask0/table.dat`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/table.dat` & `glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_3d.image/table.dat`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_4d.fits` & `glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_4d.fits`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/data/cube_4d_fullstokes.fits` & `glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/data/cube_4d_fullstokes.fits`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/glue_astronomy/io/spectral_cube/tests/test_spectral_cube.py` & `glue-astronomy-0.8.0/glue_astronomy/io/spectral_cube/tests/test_spectral_cube.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/glue_astronomy/spectral_coordinates.py` & `glue-astronomy-0.8.0/glue_astronomy/spectral_coordinates.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/glue_astronomy/tests/test_spectral_coordinates.py` & `glue-astronomy-0.8.0/glue_astronomy/tests/test_spectral_coordinates.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/glue_astronomy/translators/nddata.py` & `glue-astronomy-0.8.0/glue_astronomy/translators/nddata.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/glue_astronomy/translators/spectral_cube.py` & `glue-astronomy-0.8.0/glue_astronomy/translators/spectral_cube.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/glue_astronomy/translators/spectrum1d.py` & `glue-astronomy-0.8.0/glue_astronomy/translators/spectrum1d.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/glue_astronomy/translators/tests/test_nddata.py` & `glue-astronomy-0.8.0/glue_astronomy/translators/tests/test_nddata.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/glue_astronomy/translators/tests/test_regions.py` & `glue-astronomy-0.8.0/glue_astronomy/translators/tests/test_regions.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,31 +2,34 @@
 import numpy as np
 from astropy import units as u
 from astropy.tests.helper import assert_quantity_allclose
 from numpy.testing import assert_allclose, assert_array_equal, assert_equal
 from packaging.version import Version
 
 from regions import (RectanglePixelRegion, PolygonPixelRegion, CirclePixelRegion,
-                     EllipsePixelRegion, PointPixelRegion, CompoundPixelRegion, PixCoord)
+                     EllipsePixelRegion, PointPixelRegion, CompoundPixelRegion,
+                     CircleAnnulusPixelRegion, PixCoord)
 
 from glue.core import Data, DataCollection
 from glue.core.roi import (RectangularROI, PolygonalROI, CircularROI, EllipticalROI,
                            PointROI, XRangeROI, YRangeROI, AbstractMplRoi)
 
 from glue.core.subset import (RoiSubsetState, RangeSubsetState, OrState,
                               AndState, XorState, MultiOrState, MultiRangeSubsetState)
 
 from glue.viewers.image.pixel_selection_subset_state import PixelSubsetState
 from glue import __version__ as glue_version
 
+from glue_astronomy.translators.regions import _annulus_to_subset_state
+
 
 class TestAstropyRegions:
 
     def setup_method(self, method):
-        self.data = Data(flux=np.ones((128, 256)))
+        self.data = Data(flux=np.ones((128, 256)))  # ny, nx
         self.dc = DataCollection([self.data])
 
     def test_rectangular_roi(self):
 
         subset_state = RoiSubsetState(self.data.pixel_component_ids[1],
                                       self.data.pixel_component_ids[0],
                                       RectangularROI(1, 3.5, -0.2, 3.3))
@@ -300,14 +303,28 @@
         assert isinstance(reg.region2, CirclePixelRegion)
 
         assert reg.contains(PixCoord(4.5, 5.5))
         assert not reg.contains(PixCoord(3, 4))
         assert not reg.contains(PixCoord(5.1, 6.1))
         assert not reg.contains(PixCoord(11, 12))
 
+    def test_circular_annulus(self):
+        reg_orig = CircleAnnulusPixelRegion(
+            center=PixCoord(x=50, y=25), inner_radius=7, outer_radius=13)
+        subset_state = _annulus_to_subset_state(reg_orig, self.data)
+        self.dc.new_subset_group(subset_state=subset_state, label='annulus_1')
+        reg = self.data.get_selection_definition(subset_id='annulus_1', format='astropy-regions')
+
+        # Would round-trip if translator worked correctly.
+        assert isinstance(reg, CircleAnnulusPixelRegion)
+        assert reg.center.x == reg_orig.center.x
+        assert reg.center.y == reg_orig.center.y
+        assert reg.outer_radius == reg_orig.outer_radius
+        assert reg.inner_radius == reg_orig.inner_radius
+
     def test_or_region(self):
         subset_state1 = RoiSubsetState(self.data.pixel_component_ids[1],
                                        self.data.pixel_component_ids[0],
                                        RectangularROI(1, 5, 2, 6))
         subset_state2 = RoiSubsetState(self.data.pixel_component_ids[1],
                                        self.data.pixel_component_ids[0],
                                        CircularROI(4.75, 5.75, 0.5))
@@ -390,15 +407,15 @@
 
         and_region = self.data.get_selection_definition(subset_id='and', format='astropy-regions')
         or_region = self.data.get_selection_definition(subset_id='or', format='astropy-regions')
         xor_region = self.data.get_selection_definition(subset_id='xor', format='astropy-regions')
         multior_region = self.data.get_selection_definition(subset_id='multior',
                                                             format='astropy-regions')
 
-        for reg in and_region, or_region, xor_region, multior_region:
+        for reg in (and_region, or_region, xor_region, multior_region):
             assert isinstance(reg, CompoundPixelRegion)
             assert isinstance(reg.region1, RectanglePixelRegion)
             assert isinstance(reg.region2, CirclePixelRegion)
 
     def test_reordered_pixel_components(self):
         self.data._pixel_component_ids = self.data._pixel_component_ids[::-1]
         range_state = RangeSubsetState(105.5, 107.7, self.data.pixel_component_ids[1])
@@ -432,28 +449,28 @@
 
         subset_state = RoiSubsetState(self.data.pixel_component_ids[1],
                                       self.data.pixel_component_ids[0],
                                       RectangularROI(1, 3.5, -0.2, 3.3))
 
         self.dc.new_subset_group(subset_state=subset_state, label='rectangular')
 
-        for subset_id in [None, 0, 'rectangular']:
+        for subset_id in (None, 0, 'rectangular'):
             reg = self.data.get_selection_definition(format='astropy-regions',
                                                      subset_id=subset_id)
             assert isinstance(reg, RectanglePixelRegion)
             assert_allclose(reg.center.x, 2.25)
             assert_allclose(reg.center.y, 1.55)
             assert_allclose(reg.width, 2.5)
             assert_allclose(reg.height, 3.5)
 
-        with pytest.raises(ValueError) as exc:
+        with pytest.raises(ValueError, match="No subset found with the label 'circular'"):
             self.data.get_selection_definition(format='astropy-regions',
                                                subset_id='circular')
-        assert exc.value.args[0] == "No subset found with the label 'circular'"
 
     def test_unsupported(self):
         self.dc.new_subset_group(subset_state=self.data.id['flux'] > 0.5,
                                  label='Flux-based selection')
-        with pytest.raises(NotImplementedError) as exc:
+        with pytest.raises(
+                NotImplementedError,
+                match='Subset states of type InequalitySubsetState are not supported'):
             self.data.get_selection_definition(format='astropy-regions',
                                                subset_id='Flux-based selection')
-        assert exc.value.args[0] == 'Subset states of type InequalitySubsetState are not supported'
```

### Comparing `glue-astronomy-0.7.0/glue_astronomy/translators/tests/test_spectral_cube.py` & `glue-astronomy-0.8.0/glue_astronomy/translators/tests/test_spectral_cube.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/glue_astronomy/translators/tests/test_spectrum1d.py` & `glue-astronomy-0.8.0/glue_astronomy/translators/tests/test_spectrum1d.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/glue_astronomy/translators/tests/test_trace.py` & `glue-astronomy-0.8.0/glue_astronomy/translators/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/glue_astronomy/translators/trace.py` & `glue-astronomy-0.8.0/glue_astronomy/translators/trace.py`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/glue_astronomy.egg-info/PKG-INFO` & `glue-astronomy-0.8.0/glue_astronomy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-astronomy
-Version: 0.7.0
+Version: 0.8.0
 Summary: Astronomy-specific plugins for glue
 Home-page: https://github.com/glue-viz/glue-astronomy
 Author: Thomas Robitaille
 Author-email: glue.viz@gmail.com
 License: BSD 3-Clause License
 Provides: glue_astronomy
 Requires-Python: >=3.8
```

### Comparing `glue-astronomy-0.7.0/glue_astronomy.egg-info/SOURCES.txt` & `glue-astronomy-0.8.0/glue_astronomy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/setup.cfg` & `glue-astronomy-0.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `glue-astronomy-0.7.0/tox.ini` & `glue-astronomy-0.8.0/tox.ini`

 * *Files identical despite different names*


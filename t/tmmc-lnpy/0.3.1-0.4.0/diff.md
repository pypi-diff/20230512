# Comparing `tmp/tmmc-lnpy-0.3.1.tar.gz` & `tmp/tmmc-lnpy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmmc-lnpy-0.3.1.tar", last modified: Thu May  4 19:23:43 2023, max compression
+gzip compressed data, was "tmmc-lnpy-0.4.0.tar", last modified: Fri May 12 20:08:59 2023, max compression
```

## Comparing `tmmc-lnpy-0.3.1.tar` & `tmmc-lnpy-0.4.0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.829684 tmmc-lnpy-0.3.1/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1489 2023-05-04 19:22:49.000000 tmmc-lnpy-0.3.1/.cruft.json
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      540 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/.editorconfig
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1324 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/.gitignore
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/.markdownlint.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3681 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/.prettierrc.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      684 2023-05-04 19:22:49.000000 tmmc-lnpy-0.3.1/.recipe-append.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      122 2023-04-24 16:21:31.000000 tmmc-lnpy-0.3.1/AUTHORS.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1834 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/CHANGELOG.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9663 2023-05-04 19:22:49.000000 tmmc-lnpy-0.3.1/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1645 2023-04-13 20:07:49.000000 tmmc-lnpy-0.3.1/LICENSE
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      285 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/MANIFEST.in
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    11319 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/Makefile
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     7674 2023-05-04 19:23:43.829048 tmmc-lnpy-0.3.1/PKG-INFO
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3245 2023-05-04 19:22:49.000000 tmmc-lnpy-0.3.1/README.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.789692 tmmc-lnpy-0.3.1/changelog.d/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/changelog.d/README.txt
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.790416 tmmc-lnpy-0.3.1/changelog.d/templates/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.791513 tmmc-lnpy-0.3.1/changelog.d/templates/auto-changelog/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      213 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/changelog.d/templates/auto-changelog/macros.jinja2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      774 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/changelog.d/templates/auto-changelog/template.jinja2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      269 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/changelog.d/templates/new_fragment.md.j2
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.797149 tmmc-lnpy-0.3.1/environment/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      961 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/environment/dev-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      317 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/environment/dev.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      108 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       79 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      670 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/environment/docs-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      523 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/environment/docs.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       53 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/environment/lint-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      207 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/environment/lint.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       25 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      198 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/environment/test.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      299 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/environment/tools.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      187 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/environment.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6102 2023-05-04 19:22:49.000000 tmmc-lnpy-0.3.1/pyproject.toml
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.801244 tmmc-lnpy-0.3.1/scripts/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      840 2023-05-04 19:22:49.000000 tmmc-lnpy-0.3.1/scripts/dist-conda.mk
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      312 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/scripts/dist-pypi.mk
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1099 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/scripts/docs-examples-symlinks.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      266 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/scripts/lint.mk
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      598 2023-05-04 19:22:49.000000 tmmc-lnpy-0.3.1/scripts/recipe-append.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       91 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/scripts/run-prettier.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      489 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/scripts/tox-ipykernel-display-name.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       38 2023-05-04 19:23:43.829922 tmmc-lnpy-0.3.1/setup.cfg
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.781344 tmmc-lnpy-0.3.1/src/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.802922 tmmc-lnpy-0.3.1/src/lnPi/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      815 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.1/src/lnPi/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      111 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.1/src/lnPi/collectionlnpiutils.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       90 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.1/src/lnPi/stability.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.810538 tmmc-lnpy-0.3.1/src/lnpy/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1744 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.1/src/lnpy/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2664 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.1/src/lnpy/bracket.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.813876 tmmc-lnpy-0.3.1/src/lnpy/data/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)   243309 2022-09-28 17:20:41.000000 tmmc-lnpy-0.3.1/src/lnpy/data/hsmix_example.json.gz
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    38953 2023-04-14 22:51:35.000000 tmmc-lnpy-0.3.1/src/lnpy/data/lj_sub_example.json
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    38751 2023-04-14 22:51:35.000000 tmmc-lnpy-0.3.1/src/lnpy/data/lj_sup_example.json
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)   450917 2022-09-28 17:20:41.000000 tmmc-lnpy-0.3.1/src/lnpy/data/ljmix_sup_example.json.gz
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    61595 2023-04-14 22:51:35.000000 tmmc-lnpy-0.3.1/src/lnpy/data/watermof_example.json
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2270 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/src/lnpy/docstrings.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    34518 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/src/lnpy/ensembles.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4997 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.1/src/lnpy/examples.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13203 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/src/lnpy/extensions.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18031 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.1/src/lnpy/lnpicollectionutils.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18795 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/src/lnpy/lnpidata.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    22908 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/src/lnpy/lnpienergy.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    26234 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/src/lnpy/lnpiseries.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    15148 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/src/lnpy/maskedlnpi_legacy.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6050 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.1/src/lnpy/molfrac.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3127 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/src/lnpy/options.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    20437 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/src/lnpy/segment.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    26446 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/src/lnpy/stability.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14481 2023-04-04 21:54:21.000000 tmmc-lnpy-0.3.1/src/lnpy/utils.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.817842 tmmc-lnpy-0.3.1/src/tmmc_lnpy.egg-info/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     7674 2023-05-04 19:23:43.000000 tmmc-lnpy-0.3.1/src/tmmc_lnpy.egg-info/PKG-INFO
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2083 2023-05-04 19:23:43.000000 tmmc-lnpy-0.3.1/src/tmmc_lnpy.egg-info/SOURCES.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-05-04 19:23:43.000000 tmmc-lnpy-0.3.1/src/tmmc_lnpy.egg-info/dependency_links.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      112 2023-05-04 19:23:43.000000 tmmc-lnpy-0.3.1/src/tmmc_lnpy.egg-info/requires.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       10 2023-05-04 19:23:43.000000 tmmc-lnpy-0.3.1/src/tmmc_lnpy.egg-info/top_level.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-05-04 19:23:42.000000 tmmc-lnpy-0.3.1/src/tmmc_lnpy.egg-info/zip-safe
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.822594 tmmc-lnpy-0.3.1/tests/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2540 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/tests/test_hs_mix.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       24 2023-04-05 21:34:36.000000 tmmc-lnpy-0.3.1/tests/test_import.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1852 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/tests/test_lj_mix_0.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5240 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/tests/test_lnPi.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5843 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/tests/test_single_comp_sub.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5081 2023-05-03 03:04:44.000000 tmmc-lnpy-0.3.1/tests/test_single_comp_super.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2801 2023-04-15 00:15:07.000000 tmmc-lnpy-0.3.1/tests/test_water_cluster.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-04 19:23:43.828035 tmmc-lnpy-0.3.1/tests/water_cluster/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      559 2022-09-14 17:15:37.000000 tmmc-lnpy-0.3.1/tests/water_cluster/data_0.csv
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      116 2022-09-14 17:15:37.000000 tmmc-lnpy-0.3.1/tests/water_cluster/data_0_dw.csv
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3953 2022-09-14 17:15:37.000000 tmmc-lnpy-0.3.1/tests/water_cluster/data_1.csv
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4784 2022-09-14 17:15:37.000000 tmmc-lnpy-0.3.1/tests/water_cluster/data_1_dw.csv
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      367 2023-04-14 22:51:35.000000 tmmc-lnpy-0.3.1/tests/water_cluster/water_MOF_ensemble.json
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    29453 2022-09-14 17:15:37.000000 tmmc-lnpy-0.3.1/tests/water_cluster/water_MOF_example.csv
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3947 2023-05-04 19:22:49.000000 tmmc-lnpy-0.3.1/tox.ini
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.759583 tmmc-lnpy-0.4.0/
+-rw-r--r--   0 wpk      (42033)    36681     1492 2023-05-12 20:08:22.000000 tmmc-lnpy-0.4.0/.cruft.json
+-rw-r--r--   0 wpk      (42033)    36681      540 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/.editorconfig
+-rw-r--r--   0 wpk      (42033)    36681     1347 2023-05-12 20:08:22.000000 tmmc-lnpy-0.4.0/.gitignore
+-rw-r--r--   0 wpk      (42033)    36681      161 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033)    36681     3683 2023-05-12 20:08:22.000000 tmmc-lnpy-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033)    36681       20 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033)    36681      684 2023-05-04 19:22:49.000000 tmmc-lnpy-0.4.0/.recipe-append.yaml
+-rw-r--r--   0 wpk      (42033)    36681      122 2023-04-24 16:21:31.000000 tmmc-lnpy-0.4.0/AUTHORS.md
+-rw-r--r--   0 wpk      (42033)    36681     2087 2023-05-12 20:08:22.000000 tmmc-lnpy-0.4.0/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033)    36681     9663 2023-05-04 19:22:49.000000 tmmc-lnpy-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033)    36681     1645 2023-04-13 20:07:49.000000 tmmc-lnpy-0.4.0/LICENSE
+-rw-r--r--   0 wpk      (42033)    36681      285 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/MANIFEST.in
+-rw-r--r--   0 wpk      (42033)    36681    11436 2023-05-12 20:08:22.000000 tmmc-lnpy-0.4.0/Makefile
+-rw-r--r--   0 wpk      (42033)    36681     9142 2023-05-12 20:08:59.759097 tmmc-lnpy-0.4.0/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681     4460 2023-05-12 20:08:22.000000 tmmc-lnpy-0.4.0/README.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.726364 tmmc-lnpy-0.4.0/changelog.d/
+-rw-r--r--   0 wpk      (42033)    36681       64 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.726737 tmmc-lnpy-0.4.0/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.728287 tmmc-lnpy-0.4.0/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033)    36681      213 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      774 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      269 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/changelog.d/templates/new_fragment.md.j2
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.734166 tmmc-lnpy-0.4.0/environment/
+-rw-r--r--   0 wpk      (42033)    36681      979 2023-05-12 20:08:22.000000 tmmc-lnpy-0.4.0/environment/dev-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      356 2023-05-12 20:08:22.000000 tmmc-lnpy-0.4.0/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033)    36681      108 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033)    36681       79 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033)    36681      670 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/environment/docs-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      523 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/environment/docs.yaml
+-rw-r--r--   0 wpk      (42033)    36681       53 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/environment/lint-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      207 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/environment/lint.yaml
+-rw-r--r--   0 wpk      (42033)    36681       25 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      198 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/environment/test.yaml
+-rw-r--r--   0 wpk      (42033)    36681      299 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/environment/tools.yaml
+-rw-r--r--   0 wpk      (42033)    36681      187 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/environment.yaml
+-rw-r--r--   0 wpk      (42033)    36681     6155 2023-05-12 20:08:22.000000 tmmc-lnpy-0.4.0/pyproject.toml
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.738529 tmmc-lnpy-0.4.0/scripts/
+-rw-r--r--   0 wpk      (42033)    36681      840 2023-05-04 19:22:49.000000 tmmc-lnpy-0.4.0/scripts/dist-conda.mk
+-rw-r--r--   0 wpk      (42033)    36681      312 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/scripts/dist-pypi.mk
+-rw-r--r--   0 wpk      (42033)    36681     1099 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/scripts/docs-examples-symlinks.sh
+-rw-r--r--   0 wpk      (42033)    36681      266 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/scripts/lint.mk
+-rw-r--r--   0 wpk      (42033)    36681      598 2023-05-04 19:22:49.000000 tmmc-lnpy-0.4.0/scripts/recipe-append.sh
+-rw-r--r--   0 wpk      (42033)    36681       91 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/scripts/run-prettier.sh
+-rw-r--r--   0 wpk      (42033)    36681      489 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/scripts/tox-ipykernel-display-name.sh
+-rw-r--r--   0 wpk      (42033)    36681       38 2023-05-12 20:08:59.759688 tmmc-lnpy-0.4.0/setup.cfg
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.714485 tmmc-lnpy-0.4.0/src/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.739950 tmmc-lnpy-0.4.0/src/lnPi/
+-rw-r--r--   0 wpk      (42033)    36681      815 2023-04-04 21:54:21.000000 tmmc-lnpy-0.4.0/src/lnPi/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681      111 2023-04-04 21:54:21.000000 tmmc-lnpy-0.4.0/src/lnPi/collectionlnpiutils.py
+-rw-r--r--   0 wpk      (42033)    36681       90 2023-04-04 21:54:21.000000 tmmc-lnpy-0.4.0/src/lnPi/stability.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.746514 tmmc-lnpy-0.4.0/src/lnpy/
+-rw-r--r--   0 wpk      (42033)    36681     1744 2023-04-04 21:54:21.000000 tmmc-lnpy-0.4.0/src/lnpy/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681     2664 2023-04-04 21:54:21.000000 tmmc-lnpy-0.4.0/src/lnpy/bracket.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.750374 tmmc-lnpy-0.4.0/src/lnpy/data/
+-rw-r--r--   0 wpk      (42033)    36681   243309 2022-09-28 17:20:41.000000 tmmc-lnpy-0.4.0/src/lnpy/data/hsmix_example.json.gz
+-rw-r--r--   0 wpk      (42033)    36681    38953 2023-04-14 22:51:35.000000 tmmc-lnpy-0.4.0/src/lnpy/data/lj_sub_example.json
+-rw-r--r--   0 wpk      (42033)    36681    38751 2023-04-14 22:51:35.000000 tmmc-lnpy-0.4.0/src/lnpy/data/lj_sup_example.json
+-rw-r--r--   0 wpk      (42033)    36681   450917 2022-09-28 17:20:41.000000 tmmc-lnpy-0.4.0/src/lnpy/data/ljmix_sup_example.json.gz
+-rw-r--r--   0 wpk      (42033)    36681    61595 2023-04-14 22:51:35.000000 tmmc-lnpy-0.4.0/src/lnpy/data/watermof_example.json
+-rw-r--r--   0 wpk      (42033)    36681     2270 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/src/lnpy/docstrings.py
+-rw-r--r--   0 wpk      (42033)    36681    34518 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/src/lnpy/ensembles.py
+-rw-r--r--   0 wpk      (42033)    36681     5004 2023-05-12 20:08:22.000000 tmmc-lnpy-0.4.0/src/lnpy/examples.py
+-rw-r--r--   0 wpk      (42033)    36681    13203 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/src/lnpy/extensions.py
+-rw-r--r--   0 wpk      (42033)    36681    18031 2023-04-04 21:54:21.000000 tmmc-lnpy-0.4.0/src/lnpy/lnpicollectionutils.py
+-rw-r--r--   0 wpk      (42033)    36681    18795 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/src/lnpy/lnpidata.py
+-rw-r--r--   0 wpk      (42033)    36681    22908 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/src/lnpy/lnpienergy.py
+-rw-r--r--   0 wpk      (42033)    36681    26234 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/src/lnpy/lnpiseries.py
+-rw-r--r--   0 wpk      (42033)    36681    15148 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/src/lnpy/maskedlnpi_legacy.py
+-rw-r--r--   0 wpk      (42033)    36681     6050 2023-04-04 21:54:21.000000 tmmc-lnpy-0.4.0/src/lnpy/molfrac.py
+-rw-r--r--   0 wpk      (42033)    36681     3127 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/src/lnpy/options.py
+-rw-r--r--   0 wpk      (42033)    36681    20437 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/src/lnpy/segment.py
+-rw-r--r--   0 wpk      (42033)    36681    26446 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/src/lnpy/stability.py
+-rw-r--r--   0 wpk      (42033)    36681    14481 2023-04-04 21:54:21.000000 tmmc-lnpy-0.4.0/src/lnpy/utils.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.752957 tmmc-lnpy-0.4.0/src/tmmc_lnpy.egg-info/
+-rw-r--r--   0 wpk      (42033)    36681     9142 2023-05-12 20:08:59.000000 tmmc-lnpy-0.4.0/src/tmmc_lnpy.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681     2083 2023-05-12 20:08:59.000000 tmmc-lnpy-0.4.0/src/tmmc_lnpy.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-05-12 20:08:59.000000 tmmc-lnpy-0.4.0/src/tmmc_lnpy.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033)    36681      112 2023-05-12 20:08:59.000000 tmmc-lnpy-0.4.0/src/tmmc_lnpy.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033)    36681       10 2023-05-12 20:08:59.000000 tmmc-lnpy-0.4.0/src/tmmc_lnpy.egg-info/top_level.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-05-04 19:23:42.000000 tmmc-lnpy-0.4.0/src/tmmc_lnpy.egg-info/zip-safe
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.756067 tmmc-lnpy-0.4.0/tests/
+-rw-r--r--   0 wpk      (42033)    36681     2540 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/tests/test_hs_mix.py
+-rw-r--r--   0 wpk      (42033)    36681       24 2023-04-05 21:34:36.000000 tmmc-lnpy-0.4.0/tests/test_import.py
+-rw-r--r--   0 wpk      (42033)    36681     1852 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/tests/test_lj_mix_0.py
+-rw-r--r--   0 wpk      (42033)    36681     5240 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/tests/test_lnPi.py
+-rw-r--r--   0 wpk      (42033)    36681     5843 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/tests/test_single_comp_sub.py
+-rw-r--r--   0 wpk      (42033)    36681     5081 2023-05-03 03:04:44.000000 tmmc-lnpy-0.4.0/tests/test_single_comp_super.py
+-rw-r--r--   0 wpk      (42033)    36681     2802 2023-05-12 20:08:22.000000 tmmc-lnpy-0.4.0/tests/test_water_cluster.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-12 20:08:59.758416 tmmc-lnpy-0.4.0/tests/water_cluster/
+-rw-r--r--   0 wpk      (42033)    36681      559 2022-09-14 17:15:37.000000 tmmc-lnpy-0.4.0/tests/water_cluster/data_0.csv
+-rw-r--r--   0 wpk      (42033)    36681      116 2022-09-14 17:15:37.000000 tmmc-lnpy-0.4.0/tests/water_cluster/data_0_dw.csv
+-rw-r--r--   0 wpk      (42033)    36681     3953 2022-09-14 17:15:37.000000 tmmc-lnpy-0.4.0/tests/water_cluster/data_1.csv
+-rw-r--r--   0 wpk      (42033)    36681     4784 2022-09-14 17:15:37.000000 tmmc-lnpy-0.4.0/tests/water_cluster/data_1_dw.csv
+-rw-r--r--   0 wpk      (42033)    36681      367 2023-04-14 22:51:35.000000 tmmc-lnpy-0.4.0/tests/water_cluster/water_MOF_ensemble.json
+-rw-r--r--   0 wpk      (42033)    36681    29453 2022-09-14 17:15:37.000000 tmmc-lnpy-0.4.0/tests/water_cluster/water_MOF_example.csv
+-rw-r--r--   0 wpk      (42033)    36681     4088 2023-05-12 20:08:22.000000 tmmc-lnpy-0.4.0/tox.ini
```

### Comparing `tmmc-lnpy-0.3.1/.cruft.json` & `tmmc-lnpy-0.4.0/.cruft.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9155701754385964%*

 * *Differences: {"'commit'": "'a0209ae199aa6f953364fc929e50d41d58082173'",*

 * * "'context'": "{'cookiecutter': {'conda_channel': 'conda-forge'}}"}*

```diff
@@ -1,25 +1,25 @@
 {
     "checkout": "feature/markdown",
-    "commit": "10a9fe1a4f0b341184e41953433c344020f92c72",
+    "commit": "a0209ae199aa6f953364fc929e50d41d58082173",
     "context": {
         "cookiecutter": {
             "_copy_without_render": [
                 "*.html",
                 "docs/_templates/*.rst",
                 "docs/_templates/autosummary/*.rst",
                 "docs/_templates/autodocsumm/*.rst",
                 "docs/_static/css/*",
                 "docs/_static/js/*",
                 "changelog.d/templates/*.j2",
                 "changelog.d/templates/auto-changelog/*.jinja2"
             ],
             "_template": "https://github.com/wpk-nist-gov/cookiecutter-pypackage.git",
             "command_line_interface": "No command-line interface",
-            "conda_channel": "wpk-nist",
+            "conda_channel": "conda-forge",
             "create_author_file": "y",
             "email": "wpk@nist.gov",
             "full_name": "William P. Krekelberg",
             "github_username": "usnistgov",
             "open_source_license": "NIST license",
             "project_name": "tmmc-lnpy",
             "project_short_description": "Analysis of lnPi results from TMMC simulation",
```

### Comparing `tmmc-lnpy-0.3.1/.editorconfig` & `tmmc-lnpy-0.4.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/.gitignore` & `tmmc-lnpy-0.4.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -106,7 +106,8 @@
 pyrightconfig.json
 .autoenv.zsh
 .autoenv_leave.zsh
 /docs/**/generated/
 /monkeytype.sqlite3
 /dist-conda/*
 !/dist-conda/Makefile
+/tmmc-lnpy-feedstock*/
```

### Comparing `tmmc-lnpy-0.3.1/.pre-commit-config.yaml` & `tmmc-lnpy-0.4.0/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
       - id: black
   - repo: https://github.com/adamchainz/blacken-docs
     rev: "1.13.0"
     hooks:
       - id: blacken-docs
         additional_dependencies:
           - black==23.3.0
-        exclude: ^README.md
+        # exclude: ^README.md
   - repo: https://github.com/nbQA-dev/nbQA
     rev: 1.7.0
     hooks:
       - id: nbqa-ruff
         additional_dependencies: [ruff]
         exclude: ^examples/archived/
       - id: nbqa-black
```

### Comparing `tmmc-lnpy-0.3.1/.recipe-append.yaml` & `tmmc-lnpy-0.4.0/.recipe-append.yaml`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/CHANGELOG.md` & `tmmc-lnpy-0.4.0/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,30 @@
+<!-- markdownlint-disable MD024 -->
+
 # Changelog
 
 Changelog for `lnpy`
 
 ## Unreleased
 
 See the fragment files in [changelog.d](https://github.com/usnistgov/tmmc-lnpy)
 
 <!-- scriv-insert-here -->
 
+## v0.4.0 — 2023-05-12
+
+### Added
+
+- Package now available on conda-forge
+
+### Changed
+
+- Changed `examples.load_example_maskddata` to
+  `examples.load_example_lnpimasked` for consistency with other method names.
+
 ## v0.3.0 — 2023-05-02
 
 ### Added
 
 - Added support for python3.11
 
 - Moved `_docstrings` -> `docstrings` to make available
```

### Comparing `tmmc-lnpy-0.3.1/CONTRIBUTING.md` & `tmmc-lnpy-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/LICENSE` & `tmmc-lnpy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/Makefile` & `tmmc-lnpy-0.4.0/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,17 @@
 ################################################################################
 # Testing
 ################################################################################
 .PHONY: test coverage
 test: ## run tests quickly with the default Python
 	pytest -x -v
 
+test-accept: ## run tests and accept doctest results. (using pytest-accept)
+	DOCFILLER_SUB=False pytest -v --accept
+
 coverage: ## check code coverage quickly with the default Python
 	coverage run --source lnpy -m pytest
 	coverage report -m
 	coverage html
 	$(BROWSER) htmlcov/index.html
```

### Comparing `tmmc-lnpy-0.3.1/PKG-INFO` & `tmmc-lnpy-0.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmmc-lnpy
-Version: 0.3.1
+Version: 0.4.0
 Summary: Analysis of lnPi results from TMMC simulation
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST-PD
 Project-URL: homepage, https://github.com/usnistgov/tmmc-lnpy
 Project-URL: documentation, https://pages.nist.gov/tmmc-lnpy/
 Keywords: tmmc-lnpy
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -42,16 +42,16 @@
 [black-link]: https://github.com/psf/black
 [pypi-badge]: https://img.shields.io/pypi/v/tmmc-lnpy
 [pypi-link]: https://pypi.org/project/tmmc-lnpy
 [docs-badge]: https://img.shields.io/badge/docs-sphinx-informational
 [docs-link]: https://pages.nist.gov/tmmc-lnpy/
 [repo-badge]: https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff
 [repo-link]: https://github.com/usnistgov/tmmc-lnpy
-[conda-badge]: https://img.shields.io/conda/v/wpk-nist/tmmc-lnpy
-[conda-link]: https://anaconda.org/wpk-nist/tmmc-lnpy
+[conda-badge]: https://img.shields.io/conda/v/conda-forge/tmmc-lnpy
+[conda-link]: https://anaconda.org/conda-forge/tmmc-lnpy
 [license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
 [license-link]: https://github.com/usnistgov/tmmc-lnpy/blob/main/LICENSE
 
 <!-- other links -->
 
 # `tmmc-lnpy`
 
@@ -87,27 +87,71 @@
 ```bash
 pip install tmmc-lnpy
 ```
 
 or
 
 ```bash
-conda install -c wpk-nist tmmc-lnpy
+conda install -c conda-forge tmmc-lnpy
 ```
 
 ## Example usage
 
 Note that the distribution name `tmmc-lnpy` is different than the import name
 `lnpy` due to name clashing on pypi.
 
-```python
-import lnpy
-import lnpy.examples
+```pycon
+>>> import numpy as np
+>>> import lnpy
+>>> import lnpy.examples
+
+>>> ref = lnpy.examples.load_example_lnpimasked("lj_sub")
+
+>>> phase_creator = lnpy.PhaseCreator(nmax=1, ref=ref)
+>>> build_phases = phase_creator.build_phases_mu([None])
+>>> collection = lnpy.lnPiCollection.from_builder(
+...     lnzs=np.linspace(-10, 3, 5), build_phases=build_phases
+... )
+
+
+# Collections are like pandas.Series
+>>> collection
+<class lnPiCollection>
+lnz_0   phase
+-10.00  0        [-10.0]
+-6.75   0        [-6.75]
+-3.50   0         [-3.5]
+-0.25   0        [-0.25]
+ 3.00   0          [3.0]
+dtype: object
+
+
+# Access xarray backend for Grand Canonical properties with `xge` accessor
+>>> collection.xge.betaOmega()
+<xarray.DataArray 'betaOmega' (lnz_0: 5, phase: 1)>
+array([[-2.32445630e-02],
+       [-6.03695807e-01],
+       [-1.85523371e+02],
+       [-1.54471391e+03],
+       [-2.95801694e+03]])
+Coordinates:
+  * lnz_0    (lnz_0) float64 -10.0 -6.75 -3.5 -0.25 3.0
+  * phase    (phase) int64 0
+    beta     float64 1.372
+    volume   float64 512.0
+Attributes:
+    dims_n:         ['n_0']
+    dims_lnz:       ['lnz_0']
+    dims_comp:      ['component']
+    dims_state:     ['lnz_0', 'beta', 'volume']
+    dims_rec:       ['sample']
+    standard_name:  grand_potential
+    long_name:      $\beta \Omega(\mu,V,T)$
+
 
-ref = lnpy.examples.load_example_maskddata('lj_sub')
 ```
 
 <!-- end-docs -->
 
 ## Documentation
 
 See the [documentation][docs-link] for a look at `tmmc-lnpy` in action.
@@ -130,24 +174,37 @@
 
 This package was created with
 [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
 [wpk-nist-gov/cookiecutter-pypackage](https://github.com/wpk-nist-gov/cookiecutter-pypackage)
 Project template forked from
 [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).
 
+<!-- markdownlint-disable MD024 -->
+
 # Changelog
 
 Changelog for `lnpy`
 
 ## Unreleased
 
 See the fragment files in [changelog.d](https://github.com/usnistgov/tmmc-lnpy)
 
 <!-- scriv-insert-here -->
 
+## v0.4.0 — 2023-05-12
+
+### Added
+
+- Package now available on conda-forge
+
+### Changed
+
+- Changed `examples.load_example_maskddata` to
+  `examples.load_example_lnpimasked` for consistency with other method names.
+
 ## v0.3.0 — 2023-05-02
 
 ### Added
 
 - Added support for python3.11
 
 - Moved `_docstrings` -> `docstrings` to make available
```

### Comparing `tmmc-lnpy-0.3.1/changelog.d/templates/auto-changelog/template.jinja2` & `tmmc-lnpy-0.4.0/changelog.d/templates/auto-changelog/template.jinja2`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/environment/dev-extras.yaml` & `tmmc-lnpy-0.4.0/environment/dev-extras.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -43,15 +43,16 @@
   # - pyls-black
   # - pyls-isort
   # mypy
   # - mypy
   # - pytest-mypy
   # # Monkeytype: autocreate type hints
   # - MonkeyType
-  # - pip
-  # - pip:
+  - pip
+  - pip:
+      - pytest-accept
   # - mypy-extensions
   # - pytest-monkeytype
   # - flake8-mypy
   # - attr-utils
   # spelling?
   # - pyenchant
```

### Comparing `tmmc-lnpy-0.3.1/environment/docs-extras.yaml` & `tmmc-lnpy-0.4.0/environment/docs-extras.yaml`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/environment/docs.yaml` & `tmmc-lnpy-0.4.0/environment/docs.yaml`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/pyproject.toml` & `tmmc-lnpy-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -69,16 +69,16 @@
 [tool.setuptools_scm]
 fallback_version = "999"
 
 [tool.aliases]
 test = "pytest"
 
 [tool.pytest.ini_options]
-addopts = "--verbose"
-testpaths = ["tests"]
+addopts = "--verbose --doctest-modules --doctest-glob='*.md'"
+testpaths = ["README.md", "tests"]
 
 [tool.isort]
 profile = "black"
 skip_gitignore = true
 known_first_party = ["lnpy"]
 
 [tool.ruff]
```

### Comparing `tmmc-lnpy-0.3.1/scripts/dist-conda.mk` & `tmmc-lnpy-0.4.0/scripts/dist-conda.mk`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/scripts/docs-examples-symlinks.sh` & `tmmc-lnpy-0.4.0/scripts/docs-examples-symlinks.sh`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/scripts/recipe-append.sh` & `tmmc-lnpy-0.4.0/scripts/recipe-append.sh`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/src/lnPi/__init__.py` & `tmmc-lnpy-0.4.0/src/lnPi/__init__.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/src/lnpy/__init__.py` & `tmmc-lnpy-0.4.0/src/lnpy/__init__.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/src/lnpy/bracket.py` & `tmmc-lnpy-0.4.0/src/lnpy/bracket.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/src/lnpy/data/hsmix_example.json.gz` & `tmmc-lnpy-0.4.0/src/lnpy/data/hsmix_example.json.gz`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/src/lnpy/data/lj_sub_example.json` & `tmmc-lnpy-0.4.0/src/lnpy/data/lj_sub_example.json`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/src/lnpy/data/lj_sup_example.json` & `tmmc-lnpy-0.4.0/src/lnpy/data/lj_sup_example.json`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/src/lnpy/data/ljmix_sup_example.json.gz` & `tmmc-lnpy-0.4.0/src/lnpy/data/ljmix_sup_example.json.gz`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/src/lnpy/data/watermof_example.json` & `tmmc-lnpy-0.4.0/src/lnpy/data/watermof_example.json`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/src/lnpy/docstrings.py` & `tmmc-lnpy-0.4.0/src/lnpy/docstrings.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/src/lnpy/ensembles.py` & `tmmc-lnpy-0.4.0/src/lnpy/ensembles.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/src/lnpy/examples.py` & `tmmc-lnpy-0.4.0/src/lnpy/examples.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,26 +56,26 @@
     Load a dictionary of data
 
     Parameters
     ----------
     name : {'lj_sub', 'lj_sup', 'ljmix_sup', 'hsmix', 'watermof}
     """
 
-    ref = load_example_maskddata(name)
+    ref = load_example_lnpimasked(name)
 
     return {
         "lnPi_data": ref.data,
         "lnPi_mask": ref.mask,
         "state_kws": ref.state_kws,
         "extra_kws": ref.extra_kws,
         "lnz": ref.lnz,
     }
 
 
-def load_example_maskddata(name):
+def load_example_lnpimasked(name):
     """
     Load an example file
 
     Parameters
     ----------
     name : {'lj_sub', 'lj_sup', 'ljmix_sup', 'hsmix', 'watermof}
     """
@@ -119,15 +119,15 @@
         if keys is None:
             keys = ["ref", "phase_creator", "build_phases"]
         return (getattr(self, k) for k in keys)
 
 
 def lj_sup_example():
     """Create an :class:`Example` instance for a Lennard-Jones fluid (subcritical)"""
-    ref = load_example_maskddata("lj_sup")
+    ref = load_example_lnpimasked("lj_sup")
 
     phase_creator = PhaseCreator(
         nmax=1,
         nmax_peak=1,
         ref=ref,
         merge_kws={"efac": 0.8},
         tag_phases=None,
@@ -143,15 +143,15 @@
         raise ValueError("bad tag function")
     argmax0 = np.array([xx.local_argmax()[0] for xx in x])
     return np.where(argmax0 <= x[0].shape[0] / 2, 0, 1)
 
 
 def lj_sub_example():
     """Create an :class:`Example` instance for a Lennard-Jones fluid (subcritical)"""
-    ref = load_example_maskddata("lj_sub")
+    ref = load_example_lnpimasked("lj_sub")
 
     phase_creator = PhaseCreator(
         nmax=2,
         nmax_peak=4,
         ref=ref,
         merge_kws={"efac": 0.8},
         tag_phases=tag_phases_single_comp_simple,
@@ -160,15 +160,15 @@
     build_phases = phase_creator.build_phases_mu([None])
 
     return Example(ref=ref, phase_creator=phase_creator, build_phases=build_phases)
 
 
 def ljmix_sup_example():
     """Create an :class:`Example` instance for a Lennard-Jones mixture (supercritical)."""
-    ref = load_example_maskddata("ljmix_sup")
+    ref = load_example_lnpimasked("ljmix_sup")
 
     phase_creator = PhaseCreator(
         nmax=1,
         ref=ref,
     )
 
     build_phases = phase_creator.build_phases
@@ -180,15 +180,15 @@
 
     def tag_phases(x):
         if len(x) > 2:
             raise ValueError("bad tag function")
         argmax0 = np.array([xx.local_argmax()[0] for xx in x])
         return np.where(argmax0 <= x[0].shape[0] / 2, 0, 1)
 
-    ref = load_example_maskddata("hsmix")
+    ref = load_example_lnpimasked("hsmix")
 
     phase_creator = PhaseCreator(
         nmax=2, nmax_peak=4, ref=ref, tag_phases=tag_phases, merge_kws={"efac": 0.8}
     )
 
     return Example(ref=ref, phase_creator=phase_creator, build_phases=None)
 
@@ -196,15 +196,15 @@
 # def watermof_example():
 #     def tag_phases(x):
 #         if len(x) > 2:
 #             raise ValueError("bad tag function")
 #         argmax0 = np.array([xx.local_argmax()[0] for xx in x])
 #         return np.where(argmax0 <= x[0].shape[0] / 2, 0, 1)
 
-#     ref = load_example_maskddata('watermof')
+#     ref = load_example_lnpimasked('watermof')
 
 #     phase_creator = PhaseCreator(
 #         nmax=2,
 #         nmax_peak=10,
 #         merge_kws={'efac': 0.8}
 
 #     )
```

### Comparing `tmmc-lnpy-0.3.1/src/lnpy/extensions.py` & `tmmc-lnpy-0.4.0/src/lnpy/extensions.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/src/lnpy/lnpicollectionutils.py` & `tmmc-lnpy-0.4.0/src/lnpy/lnpicollectionutils.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/src/lnpy/lnpidata.py` & `tmmc-lnpy-0.4.0/src/lnpy/lnpidata.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/src/lnpy/lnpienergy.py` & `tmmc-lnpy-0.4.0/src/lnpy/lnpienergy.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/src/lnpy/lnpiseries.py` & `tmmc-lnpy-0.4.0/src/lnpy/lnpiseries.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/src/lnpy/maskedlnpi_legacy.py` & `tmmc-lnpy-0.4.0/src/lnpy/maskedlnpi_legacy.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/src/lnpy/molfrac.py` & `tmmc-lnpy-0.4.0/src/lnpy/molfrac.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/src/lnpy/options.py` & `tmmc-lnpy-0.4.0/src/lnpy/options.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/src/lnpy/segment.py` & `tmmc-lnpy-0.4.0/src/lnpy/segment.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/src/lnpy/stability.py` & `tmmc-lnpy-0.4.0/src/lnpy/stability.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/src/lnpy/utils.py` & `tmmc-lnpy-0.4.0/src/lnpy/utils.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/src/tmmc_lnpy.egg-info/PKG-INFO` & `tmmc-lnpy-0.4.0/src/tmmc_lnpy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmmc-lnpy
-Version: 0.3.1
+Version: 0.4.0
 Summary: Analysis of lnPi results from TMMC simulation
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST-PD
 Project-URL: homepage, https://github.com/usnistgov/tmmc-lnpy
 Project-URL: documentation, https://pages.nist.gov/tmmc-lnpy/
 Keywords: tmmc-lnpy
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -42,16 +42,16 @@
 [black-link]: https://github.com/psf/black
 [pypi-badge]: https://img.shields.io/pypi/v/tmmc-lnpy
 [pypi-link]: https://pypi.org/project/tmmc-lnpy
 [docs-badge]: https://img.shields.io/badge/docs-sphinx-informational
 [docs-link]: https://pages.nist.gov/tmmc-lnpy/
 [repo-badge]: https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff
 [repo-link]: https://github.com/usnistgov/tmmc-lnpy
-[conda-badge]: https://img.shields.io/conda/v/wpk-nist/tmmc-lnpy
-[conda-link]: https://anaconda.org/wpk-nist/tmmc-lnpy
+[conda-badge]: https://img.shields.io/conda/v/conda-forge/tmmc-lnpy
+[conda-link]: https://anaconda.org/conda-forge/tmmc-lnpy
 [license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
 [license-link]: https://github.com/usnistgov/tmmc-lnpy/blob/main/LICENSE
 
 <!-- other links -->
 
 # `tmmc-lnpy`
 
@@ -87,27 +87,71 @@
 ```bash
 pip install tmmc-lnpy
 ```
 
 or
 
 ```bash
-conda install -c wpk-nist tmmc-lnpy
+conda install -c conda-forge tmmc-lnpy
 ```
 
 ## Example usage
 
 Note that the distribution name `tmmc-lnpy` is different than the import name
 `lnpy` due to name clashing on pypi.
 
-```python
-import lnpy
-import lnpy.examples
+```pycon
+>>> import numpy as np
+>>> import lnpy
+>>> import lnpy.examples
+
+>>> ref = lnpy.examples.load_example_lnpimasked("lj_sub")
+
+>>> phase_creator = lnpy.PhaseCreator(nmax=1, ref=ref)
+>>> build_phases = phase_creator.build_phases_mu([None])
+>>> collection = lnpy.lnPiCollection.from_builder(
+...     lnzs=np.linspace(-10, 3, 5), build_phases=build_phases
+... )
+
+
+# Collections are like pandas.Series
+>>> collection
+<class lnPiCollection>
+lnz_0   phase
+-10.00  0        [-10.0]
+-6.75   0        [-6.75]
+-3.50   0         [-3.5]
+-0.25   0        [-0.25]
+ 3.00   0          [3.0]
+dtype: object
+
+
+# Access xarray backend for Grand Canonical properties with `xge` accessor
+>>> collection.xge.betaOmega()
+<xarray.DataArray 'betaOmega' (lnz_0: 5, phase: 1)>
+array([[-2.32445630e-02],
+       [-6.03695807e-01],
+       [-1.85523371e+02],
+       [-1.54471391e+03],
+       [-2.95801694e+03]])
+Coordinates:
+  * lnz_0    (lnz_0) float64 -10.0 -6.75 -3.5 -0.25 3.0
+  * phase    (phase) int64 0
+    beta     float64 1.372
+    volume   float64 512.0
+Attributes:
+    dims_n:         ['n_0']
+    dims_lnz:       ['lnz_0']
+    dims_comp:      ['component']
+    dims_state:     ['lnz_0', 'beta', 'volume']
+    dims_rec:       ['sample']
+    standard_name:  grand_potential
+    long_name:      $\beta \Omega(\mu,V,T)$
+
 
-ref = lnpy.examples.load_example_maskddata('lj_sub')
 ```
 
 <!-- end-docs -->
 
 ## Documentation
 
 See the [documentation][docs-link] for a look at `tmmc-lnpy` in action.
@@ -130,24 +174,37 @@
 
 This package was created with
 [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
 [wpk-nist-gov/cookiecutter-pypackage](https://github.com/wpk-nist-gov/cookiecutter-pypackage)
 Project template forked from
 [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).
 
+<!-- markdownlint-disable MD024 -->
+
 # Changelog
 
 Changelog for `lnpy`
 
 ## Unreleased
 
 See the fragment files in [changelog.d](https://github.com/usnistgov/tmmc-lnpy)
 
 <!-- scriv-insert-here -->
 
+## v0.4.0 — 2023-05-12
+
+### Added
+
+- Package now available on conda-forge
+
+### Changed
+
+- Changed `examples.load_example_maskddata` to
+  `examples.load_example_lnpimasked` for consistency with other method names.
+
 ## v0.3.0 — 2023-05-02
 
 ### Added
 
 - Added support for python3.11
 
 - Moved `_docstrings` -> `docstrings` to make available
```

### Comparing `tmmc-lnpy-0.3.1/src/tmmc_lnpy.egg-info/SOURCES.txt` & `tmmc-lnpy-0.4.0/src/tmmc_lnpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/tests/test_hs_mix.py` & `tmmc-lnpy-0.4.0/tests/test_hs_mix.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/tests/test_lj_mix_0.py` & `tmmc-lnpy-0.4.0/tests/test_lj_mix_0.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/tests/test_lnPi.py` & `tmmc-lnpy-0.4.0/tests/test_lnPi.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/tests/test_single_comp_sub.py` & `tmmc-lnpy-0.4.0/tests/test_single_comp_sub.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/tests/test_single_comp_super.py` & `tmmc-lnpy-0.4.0/tests/test_single_comp_super.py`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/tests/test_water_cluster.py` & `tmmc-lnpy-0.4.0/tests/test_water_cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 @pytest.fixture(params=[0, 1])
 def ref(request):
     if request.param == 0:
         return load_ref()
     else:
         import lnpy.examples
 
-        return lnpy.examples.load_example_maskddata("watermof")
+        return lnpy.examples.load_example_lnpimasked("watermof")
 
 
 def get_test_table(o, ref):
     return (
         o.xge.table(
             keys=[
                 "betaOmega",
```

### Comparing `tmmc-lnpy-0.3.1/tests/water_cluster/data_0.csv` & `tmmc-lnpy-0.4.0/tests/water_cluster/data_0.csv`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/tests/water_cluster/data_1.csv` & `tmmc-lnpy-0.4.0/tests/water_cluster/data_1.csv`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/tests/water_cluster/data_1_dw.csv` & `tmmc-lnpy-0.4.0/tests/water_cluster/data_1_dw.csv`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/tests/water_cluster/water_MOF_example.csv` & `tmmc-lnpy-0.4.0/tests/water_cluster/water_MOF_example.csv`

 * *Files identical despite different names*

### Comparing `tmmc-lnpy-0.3.1/tox.ini` & `tmmc-lnpy-0.4.0/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -100,30 +100,32 @@
 envdir       = {toxworkdir}/dist-conda
 basepython   = {[base]build_python}
 conda_env    = {[base]conda_env_dist_conda}
 changedir    = {toxinidir}
 commands     =
     make -f {toxinidir}/scripts/dist-conda.mk {posargs} project_name={env:project_name:{[base]package_name}}
 
-[testenv:testdist-{pypi, conda}-{local,remote}-py3{8, 9, 10, 11}]
+[testenv:testdist-{pypi, conda, condaforge}-{local,remote}-py3{8, 9, 10, 11}]
 conda_channels =
-    {[base]conda_channels}
+    conda: {[base]conda_channels}
+    condaforge: conda-forge
 description =
     Test install from
     pypi: pypi
-    conda: conda
+    conda: conda (user channel)
+    condaforge: conda (conda-forge channel)
     using either
     local: local
     remote: remote
     versions.
 skip_install = True
 conda_env    = {toxinidir}/environment/test-extras.yaml
 conda_deps =
-    conda-remote: {[base]package_name}{env:TEST_VERSION:''}
-    conda-local: {posargs}
+    conda-remote,condaforge-remote: {[base]package_name}{env:TEST_VERSION:''}
+    conda-local,condaforge-local: {posargs}
 deps =
     pypi-remote: {[base]package_name}{env:TEST_VERSION:''}
     pypi-local: {posargs}
 
 [testenv:testpip-py3{8, 9, 10, 11}]
 description  =
     Test package against pip installed packages
```


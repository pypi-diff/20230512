# Comparing `tmp/dtfabric-20221218.tar.gz` & `tmp/dtfabric-20230512.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtfabric-20221218.tar", last modified: Sun Dec 18 11:17:37 2022, max compression
+gzip compressed data, was "dtfabric-20230512.tar", last modified: Fri May 12 04:07:16 2023, max compression
```

## Comparing `dtfabric-20221218.tar` & `dtfabric-20230512.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 11:17:37.689771 dtfabric-20221218/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 11:17:37.661770 dtfabric-20221218/.github/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 11:17:37.676771 dtfabric-20221218/.github/workflows/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2519 2022-12-18 07:48:07.000000 dtfabric-20221218/.github/workflows/test_docker.yml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1356 2022-12-18 07:48:07.000000 dtfabric-20221218/.github/workflows/test_docs.yml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1656 2022-12-18 07:48:07.000000 dtfabric-20221218/.github/workflows/test_tox.yml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    21003 2022-12-18 07:48:07.000000 dtfabric-20221218/.pylintrc
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      149 2022-07-10 04:44:41.000000 dtfabric-20221218/.yamllint.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       92 2022-01-24 07:36:34.000000 dtfabric-20221218/ACKNOWLEDGEMENTS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      265 2018-07-03 18:38:13.000000 dtfabric-20221218/AUTHORS
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2016-09-25 06:41:25.000000 dtfabric-20221218/LICENSE
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      592 2021-08-22 05:30:09.000000 dtfabric-20221218/MANIFEST.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      602 2022-12-18 11:17:37.689771 dtfabric-20221218/PKG-INFO
--rw-r-----   0 lordyesta  (1000) lordyesta  (1000)      195 2020-06-21 05:38:03.000000 dtfabric-20221218/README
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2022-12-18 07:48:07.000000 dtfabric-20221218/appveyor.yml
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 11:17:37.661770 dtfabric-20221218/config/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 11:17:37.677770 dtfabric-20221218/config/appveyor/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      763 2022-12-18 07:48:07.000000 dtfabric-20221218/config/appveyor/install.ps1
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2022-12-18 07:48:07.000000 dtfabric-20221218/config/appveyor/install.sh
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2022-12-18 07:48:07.000000 dtfabric-20221218/config/appveyor/runtests.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 11:17:37.678771 dtfabric-20221218/config/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2022-12-18 07:48:59.000000 dtfabric-20221218/config/dpkg/changelog
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       38 2017-05-26 07:25:10.000000 dtfabric-20221218/config/dpkg/clean
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        2 2022-12-18 07:48:07.000000 dtfabric-20221218/config/dpkg/compat
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      786 2022-12-18 07:48:07.000000 dtfabric-20221218/config/dpkg/control
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      884 2017-04-14 13:14:48.000000 dtfabric-20221218/config/dpkg/copyright
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       20 2017-04-14 13:31:35.000000 dtfabric-20221218/config/dpkg/dtfabric-data.dirs
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       26 2017-04-14 13:32:40.000000 dtfabric-20221218/config/dpkg/dtfabric-data.install
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      144 2017-05-26 07:25:20.000000 dtfabric-20221218/config/dpkg/python-dtfabric.install
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      144 2017-05-26 07:25:27.000000 dtfabric-20221218/config/dpkg/python3-dtfabric.install
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2022-12-18 07:48:07.000000 dtfabric-20221218/config/dpkg/rules
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 11:17:37.678771 dtfabric-20221218/config/dpkg/source/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2017-04-14 13:14:48.000000 dtfabric-20221218/config/dpkg/source/format
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 11:17:37.678771 dtfabric-20221218/config/pylint/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      362 2020-06-21 09:14:13.000000 dtfabric-20221218/config/pylint/spelling-private-dict
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      151 2020-01-19 18:45:05.000000 dtfabric-20221218/dependencies.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 11:17:37.679771 dtfabric-20221218/docs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5061 2022-12-18 07:48:16.000000 dtfabric-20221218/docs/conf.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      566 2021-07-30 06:46:25.000000 dtfabric-20221218/docs/index.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      105 2022-12-18 07:48:16.000000 dtfabric-20221218/docs/requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 11:17:37.679771 dtfabric-20221218/docs/sources/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    15554 2022-07-10 05:53:49.000000 dtfabric-20221218/docs/sources/Format-specification.md
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 11:17:37.679771 dtfabric-20221218/docs/sources/api/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1097 2022-02-19 13:55:33.000000 dtfabric-20221218/docs/sources/api/dtfabric.rst
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      869 2021-07-30 06:46:25.000000 dtfabric-20221218/docs/sources/api/dtfabric.runtime.rst
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       61 2021-07-30 06:37:51.000000 dtfabric-20221218/docs/sources/api/modules.rst
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 11:17:37.680770 dtfabric-20221218/docs/sources/user/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1633 2021-12-28 03:59:54.000000 dtfabric-20221218/docs/sources/user/Installation-instructions.md
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      288 2021-07-30 06:37:51.000000 dtfabric-20221218/docs/sources/user/index.rst
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 11:17:37.681771 dtfabric-20221218/dtfabric/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       74 2022-12-18 07:48:59.000000 dtfabric-20221218/dtfabric/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31346 2022-09-25 13:56:37.000000 dtfabric-20221218/dtfabric/data_types.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      710 2022-09-18 09:38:10.000000 dtfabric-20221218/dtfabric/decorators.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1502 2021-07-30 10:44:15.000000 dtfabric-20221218/dtfabric/definitions.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1016 2021-07-30 06:46:25.000000 dtfabric-20221218/dtfabric/errors.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    53117 2022-09-18 09:39:14.000000 dtfabric-20221218/dtfabric/reader.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3192 2022-09-18 09:35:13.000000 dtfabric-20221218/dtfabric/registry.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 11:17:37.682771 dtfabric-20221218/dtfabric/runtime/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-03-18 06:58:01.000000 dtfabric-20221218/dtfabric/runtime/__init__.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2523 2022-09-18 09:36:04.000000 dtfabric-20221218/dtfabric/runtime/byte_operations.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    71655 2022-09-25 14:31:31.000000 dtfabric-20221218/dtfabric/runtime/data_maps.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2022-01-27 14:27:48.000000 dtfabric-20221218/dtfabric/runtime/fabric.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6233 2022-09-18 09:46:53.000000 dtfabric-20221218/dtfabric/runtime/runtime.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 11:17:37.681771 dtfabric-20221218/dtfabric.egg-info/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      602 2022-12-18 11:17:35.000000 dtfabric-20221218/dtfabric.egg-info/PKG-INFO
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2835 2022-12-18 11:17:37.000000 dtfabric-20221218/dtfabric.egg-info/SOURCES.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2022-12-18 11:17:35.000000 dtfabric-20221218/dtfabric.egg-info/dependency_links.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2022-12-18 11:17:35.000000 dtfabric-20221218/dtfabric.egg-info/requires.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        9 2022-12-18 11:17:35.000000 dtfabric-20221218/dtfabric.egg-info/top_level.txt
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      395 2019-02-03 12:58:57.000000 dtfabric-20221218/dtfabric.ini
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       28 2022-12-18 07:48:07.000000 dtfabric-20221218/requirements.txt
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      777 2022-09-18 09:32:38.000000 dtfabric-20221218/run_tests.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 11:17:37.682771 dtfabric-20221218/scripts/
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     3218 2022-09-18 08:56:58.000000 dtfabric-20221218/scripts/validate-definitions.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      302 2022-12-18 11:17:37.689771 dtfabric-20221218/setup.cfg
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     6782 2022-12-18 07:48:07.000000 dtfabric-20221218/setup.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 11:17:37.686771 dtfabric-20221218/test_data/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1426 2017-05-01 13:58:49.000000 dtfabric-20221218/test_data/Notepad.lnk
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       99 2022-07-10 05:55:10.000000 dtfabric-20221218/test_data/boolean.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      101 2022-07-10 05:55:12.000000 dtfabric-20221218/test_data/character.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      284 2022-07-10 05:55:13.000000 dtfabric-20221218/test_data/constant.yaml
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 11:17:37.687770 dtfabric-20221218/test_data/definitions/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      524 2022-07-10 05:54:56.000000 dtfabric-20221218/test_data/definitions/booleans.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      453 2022-07-10 05:54:58.000000 dtfabric-20221218/test_data/definitions/characters.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      405 2022-07-10 05:55:00.000000 dtfabric-20221218/test_data/definitions/floating-points.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1364 2022-07-10 05:55:01.000000 dtfabric-20221218/test_data/definitions/integers.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      812 2022-07-10 05:55:15.000000 dtfabric-20221218/test_data/enumeration.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      218 2022-07-10 05:55:16.000000 dtfabric-20221218/test_data/floating-point.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      555 2022-07-10 05:55:18.000000 dtfabric-20221218/test_data/format.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      399 2022-07-10 05:55:19.000000 dtfabric-20221218/test_data/integer.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       83 2022-07-10 05:55:23.000000 dtfabric-20221218/test_data/padding.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      457 2022-07-10 05:55:28.000000 dtfabric-20221218/test_data/sequence.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      572 2022-07-10 05:55:25.000000 dtfabric-20221218/test_data/sequence_with_context.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      433 2022-07-10 05:55:26.000000 dtfabric-20221218/test_data/sequence_with_structure.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      657 2022-07-10 05:55:29.000000 dtfabric-20221218/test_data/stream.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      707 2022-07-10 05:55:32.000000 dtfabric-20221218/test_data/string.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      818 2022-07-10 05:55:30.000000 dtfabric-20221218/test_data/string_array.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1059 2022-07-10 05:55:50.000000 dtfabric-20221218/test_data/structure.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2022-07-10 05:55:34.000000 dtfabric-20221218/test_data/structure_family.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1576 2022-07-10 05:55:35.000000 dtfabric-20221218/test_data/structure_group.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      651 2022-07-10 05:55:36.000000 dtfabric-20221218/test_data/structure_with_condition.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      496 2022-07-10 05:55:38.000000 dtfabric-20221218/test_data/structure_with_context.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      712 2022-07-10 05:57:13.000000 dtfabric-20221218/test_data/structure_with_padding.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      322 2022-07-10 05:55:41.000000 dtfabric-20221218/test_data/structure_with_section.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      468 2022-07-10 05:55:43.000000 dtfabric-20221218/test_data/structure_with_sequence.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      466 2022-07-10 05:55:44.000000 dtfabric-20221218/test_data/structure_with_stream.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      446 2022-07-10 05:55:45.000000 dtfabric-20221218/test_data/structure_with_string.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      370 2022-07-10 05:55:47.000000 dtfabric-20221218/test_data/structure_with_union.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      700 2022-07-10 05:55:49.000000 dtfabric-20221218/test_data/structure_with_values.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      383 2022-07-10 05:55:53.000000 dtfabric-20221218/test_data/union.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      380 2022-07-10 05:55:51.000000 dtfabric-20221218/test_data/union_with_condition.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      200 2022-07-10 05:55:54.000000 dtfabric-20221218/test_data/uuid.yaml
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      107 2022-12-18 07:46:44.000000 dtfabric-20221218/test_dependencies.ini
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       14 2022-12-18 07:48:07.000000 dtfabric-20221218/test_requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 11:17:37.687770 dtfabric-20221218/tests/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-03-18 06:58:01.000000 dtfabric-20221218/tests/__init__.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    19685 2022-02-13 10:09:16.000000 dtfabric-20221218/tests/data_types.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    62062 2022-07-10 05:53:49.000000 dtfabric-20221218/tests/reader.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3002 2021-07-30 06:46:25.000000 dtfabric-20221218/tests/registry.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 11:17:37.688771 dtfabric-20221218/tests/runtime/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-03-18 06:58:01.000000 dtfabric-20221218/tests/runtime/__init__.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1645 2021-07-30 09:04:50.000000 dtfabric-20221218/tests/runtime/byte_operations.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    83501 2022-09-25 13:56:56.000000 dtfabric-20221218/tests/runtime/data_maps.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      662 2021-07-30 06:46:25.000000 dtfabric-20221218/tests/runtime/fabric.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2494 2021-07-30 06:46:25.000000 dtfabric-20221218/tests/runtime/runtime.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2272 2022-09-18 09:32:59.000000 dtfabric-20221218/tests/test_lib.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1469 2022-12-18 07:48:35.000000 dtfabric-20221218/tox.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2022-12-18 11:17:37.689771 dtfabric-20221218/utils/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       70 2018-03-18 06:58:04.000000 dtfabric-20221218/utils/__init__.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2022-12-18 07:48:07.000000 dtfabric-20221218/utils/check_dependencies.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2022-12-18 07:48:07.000000 dtfabric-20221218/utils/dependencies.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      616 2021-12-28 04:01:20.000000 dtfabric-20221218/utils/update_release.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.685438 dtfabric-20230512/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.332437 dtfabric-20230512/.github/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.384437 dtfabric-20230512/.github/workflows/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2541 2023-05-08 04:44:50.000000 dtfabric-20230512/.github/workflows/test_docker.yml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1378 2023-05-08 04:44:50.000000 dtfabric-20230512/.github/workflows/test_docs.yml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4107 2023-05-08 04:44:50.000000 dtfabric-20230512/.github/workflows/test_tox.yml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    21911 2023-05-08 04:44:50.000000 dtfabric-20230512/.pylintrc
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      149 2022-07-10 04:44:41.000000 dtfabric-20230512/.yamllint.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       92 2022-01-24 07:36:34.000000 dtfabric-20230512/ACKNOWLEDGEMENTS
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      265 2018-07-03 18:38:13.000000 dtfabric-20230512/AUTHORS
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2016-09-25 06:41:25.000000 dtfabric-20230512/LICENSE
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      592 2021-08-22 05:30:09.000000 dtfabric-20230512/MANIFEST.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      583 2023-05-12 04:07:16.685438 dtfabric-20230512/PKG-INFO
+-rw-r-----   0 lordyesta  (1000) lordyesta  (1000)      195 2020-06-21 05:38:03.000000 dtfabric-20230512/README
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-05-08 04:44:50.000000 dtfabric-20230512/appveyor.yml
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.332437 dtfabric-20230512/config/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.384437 dtfabric-20230512/config/appveyor/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      839 2023-05-08 04:44:50.000000 dtfabric-20230512/config/appveyor/install.ps1
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2023-05-08 04:44:50.000000 dtfabric-20230512/config/appveyor/install.sh
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2023-05-08 04:44:50.000000 dtfabric-20230512/config/appveyor/runtests.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.437437 dtfabric-20230512/config/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2023-05-12 03:57:04.000000 dtfabric-20230512/config/dpkg/changelog
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       38 2017-05-26 07:25:10.000000 dtfabric-20230512/config/dpkg/clean
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        2 2023-05-08 04:44:51.000000 dtfabric-20230512/config/dpkg/compat
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      786 2023-05-08 04:44:51.000000 dtfabric-20230512/config/dpkg/control
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      884 2017-04-14 13:14:48.000000 dtfabric-20230512/config/dpkg/copyright
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       20 2017-04-14 13:31:35.000000 dtfabric-20230512/config/dpkg/dtfabric-data.dirs
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       26 2017-04-14 13:32:40.000000 dtfabric-20230512/config/dpkg/dtfabric-data.install
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      144 2017-05-26 07:25:20.000000 dtfabric-20230512/config/dpkg/python-dtfabric.install
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      144 2017-05-26 07:25:27.000000 dtfabric-20230512/config/dpkg/python3-dtfabric.install
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2023-05-08 04:44:51.000000 dtfabric-20230512/config/dpkg/rules
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.437437 dtfabric-20230512/config/dpkg/source/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2017-04-14 13:14:48.000000 dtfabric-20230512/config/dpkg/source/format
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.438437 dtfabric-20230512/config/pylint/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      362 2020-06-21 09:14:13.000000 dtfabric-20230512/config/pylint/spelling-private-dict
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      151 2020-01-19 18:45:05.000000 dtfabric-20230512/dependencies.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.454437 dtfabric-20230512/docs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5061 2023-05-08 04:44:51.000000 dtfabric-20230512/docs/conf.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      566 2021-07-30 06:46:25.000000 dtfabric-20230512/docs/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      105 2023-05-08 04:45:00.000000 dtfabric-20230512/docs/requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.454437 dtfabric-20230512/docs/sources/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    15554 2022-07-10 05:53:49.000000 dtfabric-20230512/docs/sources/Format-specification.md
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.455437 dtfabric-20230512/docs/sources/api/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1097 2022-02-19 13:55:33.000000 dtfabric-20230512/docs/sources/api/dtfabric.rst
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      869 2021-07-30 06:46:25.000000 dtfabric-20230512/docs/sources/api/dtfabric.runtime.rst
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       61 2021-07-30 06:37:51.000000 dtfabric-20230512/docs/sources/api/modules.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.455437 dtfabric-20230512/docs/sources/user/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1633 2021-12-28 03:59:54.000000 dtfabric-20230512/docs/sources/user/Installation-instructions.md
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      288 2021-07-30 06:37:51.000000 dtfabric-20230512/docs/sources/user/index.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.457437 dtfabric-20230512/dtfabric/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       74 2023-05-12 03:57:04.000000 dtfabric-20230512/dtfabric/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31346 2022-09-25 13:56:37.000000 dtfabric-20230512/dtfabric/data_types.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      710 2022-09-18 09:38:10.000000 dtfabric-20230512/dtfabric/decorators.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1502 2021-07-30 10:44:15.000000 dtfabric-20230512/dtfabric/definitions.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1016 2021-07-30 06:46:25.000000 dtfabric-20230512/dtfabric/errors.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    53227 2023-05-12 03:56:53.000000 dtfabric-20230512/dtfabric/reader.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3192 2022-09-18 09:35:13.000000 dtfabric-20230512/dtfabric/registry.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.461437 dtfabric-20230512/dtfabric/runtime/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-03-18 06:58:01.000000 dtfabric-20230512/dtfabric/runtime/__init__.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2523 2022-09-18 09:36:04.000000 dtfabric-20230512/dtfabric/runtime/byte_operations.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    71655 2022-09-25 14:31:31.000000 dtfabric-20230512/dtfabric/runtime/data_maps.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2022-01-27 14:27:48.000000 dtfabric-20230512/dtfabric/runtime/fabric.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6233 2022-09-18 09:46:53.000000 dtfabric-20230512/dtfabric/runtime/runtime.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.459437 dtfabric-20230512/dtfabric.egg-info/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      583 2023-05-12 04:07:14.000000 dtfabric-20230512/dtfabric.egg-info/PKG-INFO
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2835 2023-05-12 04:07:16.000000 dtfabric-20230512/dtfabric.egg-info/SOURCES.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        1 2023-05-12 04:07:14.000000 dtfabric-20230512/dtfabric.egg-info/dependency_links.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-05-12 04:07:14.000000 dtfabric-20230512/dtfabric.egg-info/requires.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        9 2023-05-12 04:07:14.000000 dtfabric-20230512/dtfabric.egg-info/top_level.txt
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      395 2019-02-03 12:58:57.000000 dtfabric-20230512/dtfabric.ini
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       28 2023-05-08 04:44:50.000000 dtfabric-20230512/requirements.txt
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      777 2022-09-18 09:32:38.000000 dtfabric-20230512/run_tests.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.461437 dtfabric-20230512/scripts/
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     3218 2022-09-18 08:56:58.000000 dtfabric-20230512/scripts/validate-definitions.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      302 2023-05-12 04:07:16.686437 dtfabric-20230512/setup.cfg
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     6782 2023-05-08 04:44:50.000000 dtfabric-20230512/setup.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.486437 dtfabric-20230512/test_data/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1426 2017-05-01 13:58:49.000000 dtfabric-20230512/test_data/Notepad.lnk
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       99 2022-07-10 05:55:10.000000 dtfabric-20230512/test_data/boolean.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      101 2022-07-10 05:55:12.000000 dtfabric-20230512/test_data/character.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      284 2022-07-10 05:55:13.000000 dtfabric-20230512/test_data/constant.yaml
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.487437 dtfabric-20230512/test_data/definitions/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      524 2022-07-10 05:54:56.000000 dtfabric-20230512/test_data/definitions/booleans.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      453 2022-07-10 05:54:58.000000 dtfabric-20230512/test_data/definitions/characters.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      405 2022-07-10 05:55:00.000000 dtfabric-20230512/test_data/definitions/floating-points.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1364 2022-07-10 05:55:01.000000 dtfabric-20230512/test_data/definitions/integers.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      812 2022-07-10 05:55:15.000000 dtfabric-20230512/test_data/enumeration.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      218 2022-07-10 05:55:16.000000 dtfabric-20230512/test_data/floating-point.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      555 2022-07-10 05:55:18.000000 dtfabric-20230512/test_data/format.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      399 2022-07-10 05:55:19.000000 dtfabric-20230512/test_data/integer.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       83 2022-07-10 05:55:23.000000 dtfabric-20230512/test_data/padding.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      457 2022-07-10 05:55:28.000000 dtfabric-20230512/test_data/sequence.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      572 2022-07-10 05:55:25.000000 dtfabric-20230512/test_data/sequence_with_context.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      433 2022-07-10 05:55:26.000000 dtfabric-20230512/test_data/sequence_with_structure.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      657 2022-07-10 05:55:29.000000 dtfabric-20230512/test_data/stream.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      707 2022-07-10 05:55:32.000000 dtfabric-20230512/test_data/string.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      818 2022-07-10 05:55:30.000000 dtfabric-20230512/test_data/string_array.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1059 2022-07-10 05:55:50.000000 dtfabric-20230512/test_data/structure.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2022-07-10 05:55:34.000000 dtfabric-20230512/test_data/structure_family.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1576 2022-07-10 05:55:35.000000 dtfabric-20230512/test_data/structure_group.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      651 2022-07-10 05:55:36.000000 dtfabric-20230512/test_data/structure_with_condition.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      496 2022-07-10 05:55:38.000000 dtfabric-20230512/test_data/structure_with_context.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      712 2022-07-10 05:57:13.000000 dtfabric-20230512/test_data/structure_with_padding.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      322 2022-07-10 05:55:41.000000 dtfabric-20230512/test_data/structure_with_section.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      468 2022-07-10 05:55:43.000000 dtfabric-20230512/test_data/structure_with_sequence.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      466 2022-07-10 05:55:44.000000 dtfabric-20230512/test_data/structure_with_stream.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      446 2022-07-10 05:55:45.000000 dtfabric-20230512/test_data/structure_with_string.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      370 2022-07-10 05:55:47.000000 dtfabric-20230512/test_data/structure_with_union.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      700 2022-07-10 05:55:49.000000 dtfabric-20230512/test_data/structure_with_values.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      383 2022-07-10 05:55:53.000000 dtfabric-20230512/test_data/union.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      380 2022-07-10 05:55:51.000000 dtfabric-20230512/test_data/union_with_condition.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      200 2022-07-10 05:55:54.000000 dtfabric-20230512/test_data/uuid.yaml
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      107 2022-12-18 07:46:44.000000 dtfabric-20230512/test_dependencies.ini
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       14 2023-05-08 04:44:50.000000 dtfabric-20230512/test_requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.618437 dtfabric-20230512/tests/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-03-18 06:58:01.000000 dtfabric-20230512/tests/__init__.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    19685 2022-02-13 10:09:16.000000 dtfabric-20230512/tests/data_types.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    62062 2022-07-10 05:53:49.000000 dtfabric-20230512/tests/reader.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3002 2021-07-30 06:46:25.000000 dtfabric-20230512/tests/registry.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.683438 dtfabric-20230512/tests/runtime/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       24 2018-03-18 06:58:01.000000 dtfabric-20230512/tests/runtime/__init__.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1645 2021-07-30 09:04:50.000000 dtfabric-20230512/tests/runtime/byte_operations.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    83501 2022-09-25 13:56:56.000000 dtfabric-20230512/tests/runtime/data_maps.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      662 2021-07-30 06:46:25.000000 dtfabric-20230512/tests/runtime/fabric.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2494 2021-07-30 06:46:25.000000 dtfabric-20230512/tests/runtime/runtime.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2272 2022-09-18 09:32:59.000000 dtfabric-20230512/tests/test_lib.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1252 2023-05-08 04:44:51.000000 dtfabric-20230512/tox.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-12 04:07:16.684438 dtfabric-20230512/utils/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       70 2018-03-18 06:58:04.000000 dtfabric-20230512/utils/__init__.py
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2023-05-08 04:44:50.000000 dtfabric-20230512/utils/check_dependencies.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2023-05-08 04:44:51.000000 dtfabric-20230512/utils/dependencies.py
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)      616 2021-12-28 04:01:20.000000 dtfabric-20230512/utils/update_release.sh
```

### Comparing `dtfabric-20221218/.github/workflows/test_docker.yml` & `dtfabric-20230512/.github/workflows/test_docker.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Run tests on Fedora and Ubuntu Docker images using GIFT CORP and GIFT PPA on commit
 name: test_docker
 on: [push]
+permissions: read-all
 jobs:
   test_fedora:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        version: ['36']
+        version: ['38']
     container:
       image: registry.fedoraproject.org/fedora:${{ matrix.version }}
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up container
       run: |
         dnf install -y dnf-plugins-core langpacks-en
     - name: Install dependencies
       run: |
         dnf copr -y enable @gift/dev
         dnf install -y @development-tools python3 python3-devel python3-mock python3-pyyaml python3-setuptools
@@ -40,15 +41,15 @@
     runs-on: ubuntu-latest
     strategy:
       matrix:
         version: ['22.04']
     container:
       image: ubuntu:${{ matrix.version }}
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
```

### Comparing `dtfabric-20221218/.github/workflows/test_docs.yml` & `dtfabric-20230512/.github/workflows/test_docs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 on:
   pull_request:
     branches:
     - main
   push:
     branches:
     - main
+permissions: read-all
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         include:
         - python-version: '3.8'
           toxenv: 'docs'
     container:
       image: ubuntu:22.04
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
```

### Comparing `dtfabric-20221218/.pylintrc` & `dtfabric-20230512/.pylintrc`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,30 @@
-# Pylint 2.10.x configuration file
+# Pylint 2.14.x configuration file
 #
 # This file is generated by l2tdevtools update-dependencies.py, any dependency
 # related changes should be made in dependencies.ini.
-[MASTER]
+[MAIN]
+
+# Analyse import fallback blocks. This can be used to support both Python 2 and
+# 3 compatible code, which means that the block might have code that exists
+# only in one or another interpreter, leading to false positives when analysed.
+analyse-fallback-blocks=no
+
+# Load and enable all available extensions. Use --list-extensions to see a list
+# all available extensions.
+#enable-all-extensions=
+
+# In error mode, messages with a category besides ERROR or FATAL are
+# suppressed, and no reports are done by default. Error mode is compatible with
+# disabling specific errors.
+#errors-only=
+
+# Always return a 0 (non-error) status code, even if lint errors are found.
+# This is primarily useful in continuous integration scripts.
+#exit-zero=
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
 # run arbitrary code.
 extension-pkg-allow-list=
 
 # A comma-separated list of package or module names from where C extensions may
@@ -17,70 +35,116 @@
 
 # Return non-zero exit code if any of these messages/categories are detected,
 # even if score is above --fail-under value. Syntax same as enable. Messages
 # specified are enabled, while categories only check already-enabled messages.
 fail-on=
 
 # Specify a score threshold to be exceeded before program exits with error.
-fail-under=10.0
+fail-under=10
+
+# Interpret the stdin as a python script, whose filename needs to be passed as
+# the module_or_package argument.
+#from-stdin=
 
 # Files or directories to be skipped. They should be base names, not paths.
 ignore=CVS
 
 # Add files or directories matching the regex patterns to the ignore-list. The
 # regex matches against paths and can be in Posix or Windows format.
 ignore-paths=
 
 # Files or directories matching the regex patterns are skipped. The regex
-# matches against base names, not paths. The default value ignores emacs file
+# matches against base names, not paths. The default value ignores Emacs file
 # locks
 ignore-patterns=^\.#
 
+# List of module names for which member attributes should not be checked
+# (useful for modules/projects where namespaces are manipulated during runtime
+# and thus existing member attributes cannot be deduced by static analysis). It
+# supports qualified module names, as well as Unix pattern matching.
+ignored-modules=
+
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
 #init-hook=
 
 # Use multiple processes to speed up Pylint. Specifying 0 will auto-detect the
-# number of processors available to use.
+# number of processors available to use, and will cap the count on Windows to
+# avoid hangs.
 jobs=1
 
 # Control the amount of potential inferred values when inferring a single
 # object. This can help the performance when dealing with large functions or
 # complex, nested conditions.
 limit-inference-results=100
 
 # List of plugins (as comma separated values of python module names) to load,
 # usually to register additional checkers.
+# load-plugins=
 load-plugins=pylint.extensions.docparams
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Minimum Python version to use for version dependent checks. Will default to
 # the version used to run pylint.
-py-version=3.10
+py-version=3.11
 
 # Discover python modules and packages in the file system subtree.
+# recursive=no
 recursive=yes
 
 # When enabled, pylint would attempt to guess common misconfiguration and emit
 # user-friendly hints instead of false-positive error messages.
 suggestion-mode=yes
 
 # Allow loading of arbitrary C extensions. Extensions are imported into the
 # active Python interpreter and may run arbitrary code.
 unsafe-load-any-extension=no
 
+# In verbose mode, extra non-checker-related info will be displayed.
+#verbose=
+
+
+[REPORTS]
+
+# Python expression which should return a score less than or equal to 10. You
+# have access to the variables 'fatal', 'error', 'warning', 'refactor',
+# 'convention', and 'info' which contain the number of messages in each
+# category, as well as 'statement' which is the total number of statements
+# analyzed. This score is used by the global evaluation report (RP0004).
+evaluation=max(0, 0 if fatal else 10.0 - ((float(5 * error + warning + refactor + convention) / statement) * 10))
+
+# Template used to display messages. This is a python new-style format string
+# used to format the message information. See doc for all details.
+msg-template=
+
+# Set the output format. Available formats are text, parseable, colorized, json
+# and msvs (visual studio). You can also give a reporter class, e.g.
+# mypackage.mymodule.MyReporterClass.
+#output-format=
+
+# Tells whether to display a full report or only the messages.
+reports=no
+
+# Activate the evaluation score.
+# score=yes
+score=no
+
 
 [MESSAGES CONTROL]
 
 # Only show warnings with the listed confidence levels. Leave empty to show
 # all. Valid levels: HIGH, CONTROL_FLOW, INFERENCE, INFERENCE_FAILURE,
 # UNDEFINED.
-confidence=
+confidence=HIGH,
+           CONTROL_FLOW,
+           INFERENCE,
+           INFERENCE_FAILURE,
+           UNDEFINED
 
 # Disable the message, report, category or checker with the given id(s). You
 # can either give multiple identifiers separated by comma (,) or put this
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once). You can also use "--disable=all" to
 # disable everything first and then re-enable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
@@ -88,26 +152,20 @@
 # no Warning level messages displayed, use "--disable=all --enable=classes
 # --disable=W".
 disable=assignment-from-none,
         bad-inline-option,
         consider-using-f-string,
         deprecated-pragma,
         duplicate-code,
-        eq-without-hash,
         file-ignored,
         fixme,
         locally-disabled,
-        locally-enabled,
         logging-format-interpolation,
         logging-fstring-interpolation,
-        metaclass-assignment,
         missing-param-doc,
-        no-absolute-import,
-        no-self-use,
-        parameter-unpacking,
         raise-missing-from,
         raw-checker-failed,
         super-with-arguments,
         suppressed-message,
         too-few-public-methods,
         too-many-ancestors,
         too-many-boolean-expressions,
@@ -126,51 +184,14 @@
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=c-extension-no-member
 
 
-[REPORTS]
-
-# Python expression which should return a score less than or equal to 10. You
-# have access to the variables 'fatal', 'error', 'warning', 'refactor',
-# 'convention', and 'info' which contain the number of messages in each
-# category, as well as 'statement' which is the total number of statements
-# analyzed. This score is used by the global evaluation report (RP0004).
-evaluation=max(0, 0 if fatal else 10.0 - ((float(5 * error + warning + refactor + convention) / statement) * 10))
-
-# Template used to display messages. This is a python new-style format string
-# used to format the message information. See doc for all details.
-#msg-template=
-
-# Set the output format. Available formats are text, parseable, colorized, json
-# and msvs (visual studio). You can also give a reporter class, e.g.
-# mypackage.mymodule.MyReporterClass.
-output-format=text
-
-# Tells whether to display a full report or only the messages.
-reports=no
-
-# Activate the evaluation score.
-score=no
-
-
-[REFACTORING]
-
-# Maximum number of nested blocks for function / method body
-max-nested-blocks=5
-
-# Complete name of functions that never returns. When checking for
-# inconsistent-return-statements if a never returning function is called then
-# it will be considered as an explicit return statement and no message will be
-# printed.
-never-returning-functions=sys.exit,argparse.parse_error
-
-
 [VARIABLES]
 
 # List of additional names supposed to be defined in builtins. Remember that
 # you should avoid defining new builtins when possible.
 additional-builtins=
 
 # Tells whether unused global variables should be treated as a violation.
@@ -208,55 +229,50 @@
 contextmanager-decorators=contextlib.contextmanager
 
 # List of members which are set dynamically and missed by pylint inference
 # system, and so shouldn't trigger E1101 when accessed. Python regular
 # expressions are accepted.
 generated-members=
 
-# Tells whether missing members accessed in mixin class should be ignored. A
-# class is considered mixin if its name matches the mixin-class-rgx option.
-ignore-mixin-members=yes
-
 # Tells whether to warn about missing members when the owner of the attribute
 # is inferred to be None.
 ignore-none=yes
 
 # This flag controls whether pylint should warn about no-member and similar
 # checks whenever an opaque object is returned when inferring. The inference
 # can return multiple potential results while evaluating a Python object, but
 # some branches might not be evaluated, which results in partial inference. In
 # that case, it might be useful to still emit no-member and other checks for
 # the rest of the inferred objects.
 ignore-on-opaque-inference=yes
 
+# List of symbolic message names to ignore for Mixin members.
+ignored-checks-for-mixins=no-member,
+                          not-async-context-manager,
+                          not-context-manager,
+                          attribute-defined-outside-init
+
 # List of class names for which member attributes should not be checked (useful
 # for classes with dynamically set attributes). This supports the use of
 # qualified names.
-ignored-classes=optparse.Values,thread._local,_thread._local
-
-# List of module names for which member attributes should not be checked
-# (useful for modules/projects where namespaces are manipulated during runtime
-# and thus existing member attributes cannot be deduced by static analysis). It
-# supports qualified module names, as well as Unix pattern matching.
-ignored-modules=
+ignored-classes=optparse.Values,thread._local,_thread._local,argparse.Namespace
 
 # Show a hint with possible names when a member name was not found. The aspect
 # of finding the hint is based on edit distance.
 missing-member-hint=yes
 
 # The minimum edit distance a name should have in order to be considered a
 # similar match for a missing member name.
 missing-member-hint-distance=1
 
 # The total number of similar names that should be taken in consideration when
 # showing a hint for a missing member.
 missing-member-max-choices=1
 
-# Regex pattern to define which classes are considered mixins ignore-mixin-
-# members is set to 'yes'
+# Regex pattern to define which classes are considered mixins.
 mixin-class-rgx=.*[Mm]ixin
 
 # List of decorators that change the signature of a decorated function.
 signature-mutators=
 
 
 [LOGGING]
@@ -266,30 +282,74 @@
 logging-format-style=old
 
 # Logging modules to check that the string format arguments are in logging
 # function parameter format.
 logging-modules=logging
 
 
+[DESIGN]
+
+# List of regular expressions of class ancestor names to ignore when counting
+# public methods (see R0903)
+exclude-too-few-public-methods=
+
+# List of qualified class names to ignore when counting class parents (see
+# R0901)
+ignored-parents=
+
+# Maximum number of arguments for function / method.
+# max-args=5
+max-args=10
+
+# Maximum number of attributes for a class (see R0902).
+max-attributes=7
+
+# Maximum number of boolean expressions in an if statement (see R0916).
+max-bool-expr=5
+
+# Maximum number of branch for function / method body.
+max-branches=12
+
+# Maximum number of locals for function / method body.
+max-locals=15
+
+# Maximum number of parents for a class (see R0901).
+max-parents=7
+
+# Maximum number of public methods for a class (see R0904).
+max-public-methods=20
+
+# Maximum number of return / yield for function / method body.
+max-returns=6
+
+# Maximum number of statements in function / method body.
+max-statements=50
+
+# Minimum number of public methods for a class (see R0903).
+min-public-methods=2
+
+
 [BASIC]
 
 # Naming style matching correct argument names.
 argument-naming-style=snake_case
 
 # Regular expression matching correct argument names. Overrides argument-
 # naming-style. If left empty, argument names will be checked with the set
 # naming style.
+#argument-rgx=
 argument-rgx=(([a-z][a-z0-9_]*)|(_[a-z0-9_]*))$
 
 # Naming style matching correct attribute names.
 attr-naming-style=snake_case
 
 # Regular expression matching correct attribute names. Overrides attr-naming-
 # style. If left empty, attribute names will be checked with the set naming
 # style.
+#attr-rgx=
 attr-rgx=(([a-z][a-z0-9_]*)|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma.
 bad-names=foo,
           bar,
           baz,
           toto,
@@ -302,14 +362,15 @@
 
 # Naming style matching correct class attribute names.
 class-attribute-naming-style=any
 
 # Regular expression matching correct class attribute names. Overrides class-
 # attribute-naming-style. If left empty, class attribute names will be checked
 # with the set naming style.
+#class-attribute-rgx=
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]*|(__.*__))$
 
 # Naming style matching correct class constant names.
 class-const-naming-style=UPPER_CASE
 
 # Regular expression matching correct class constant names. Overrides class-
 # const-naming-style. If left empty, class constant names will be checked with
@@ -317,34 +378,37 @@
 #class-const-rgx=
 
 # Naming style matching correct class names.
 class-naming-style=PascalCase
 
 # Regular expression matching correct class names. Overrides class-naming-
 # style. If left empty, class names will be checked with the set naming style.
+#class-rgx=
 class-rgx=[A-Z_][a-zA-Z0-9]+$
 
 # Naming style matching correct constant names.
 const-naming-style=UPPER_CASE
 
 # Regular expression matching correct constant names. Overrides const-naming-
 # style. If left empty, constant names will be checked with the set naming
 # style.
+#const-rgx=
 const-rgx=(([a-zA-Z_][a-zA-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
 # Naming style matching correct function names.
 function-naming-style=snake_case
 
 # Regular expression matching correct function names. Overrides function-
 # naming-style. If left empty, function names will be checked with the set
 # naming style.
+#function-rgx=
 function-rgx=[A-Z_][a-zA-Z0-9_]*$
 
 # Good variable names which should always be accepted, separated by a comma.
 good-names=i,
            j,
            k,
            ex,
@@ -360,28 +424,31 @@
 
 # Naming style matching correct inline iteration names.
 inlinevar-naming-style=any
 
 # Regular expression matching correct inline iteration names. Overrides
 # inlinevar-naming-style. If left empty, inline iteration names will be checked
 # with the set naming style.
+#inlinevar-rgx=
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
 # Naming style matching correct method names.
 method-naming-style=snake_case
 
 # Regular expression matching correct method names. Overrides method-naming-
 # style. If left empty, method names will be checked with the set naming style.
+#method-rgx=
 method-rgx=(test|[A-Z_])[a-zA-Z0-9_]*$
 
 # Naming style matching correct module names.
 module-naming-style=snake_case
 
 # Regular expression matching correct module names. Overrides module-naming-
 # style. If left empty, module names will be checked with the set naming style.
+#module-rgx=
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
 # Regular expression which should only match function or class names that do
@@ -399,26 +466,60 @@
 
 # Naming style matching correct variable names.
 variable-naming-style=snake_case
 
 # Regular expression matching correct variable names. Overrides variable-
 # naming-style. If left empty, variable names will be checked with the set
 # naming style.
+#variable-rgx=
 variable-rgx=(([a-z][a-z0-9_]*)|(_[a-z0-9_]*))$
 
 
+[EXCEPTIONS]
+
+# Exceptions that will emit a warning when caught.
+overgeneral-exceptions=BaseException,
+                       Exception
+
+
+[CLASSES]
+
+# Warn about protected attribute access inside special methods
+check-protected-access-in-special-methods=no
+
+# List of method names used to declare (i.e. assign) instance attributes.
+defining-attr-methods=__init__,
+                      __new__,
+                      setUp,
+                      __post_init__
+
+# List of member names, which should be excluded from the protected access
+# warning.
+exclude-protected=_asdict,
+                  _fields,
+                  _replace,
+                  _source,
+                  _make
+
+# List of valid names for the first argument in a class method.
+valid-classmethod-first-arg=cls
+
+# List of valid names for the first argument in a metaclass class method.
+valid-metaclass-classmethod-first-arg=cls
+
+
 [MISCELLANEOUS]
 
 # List of note tags to take in consideration, separated by a comma.
 notes=FIXME,
       XXX,
       TODO
 
 # Regular expression of note tags to take in consideration.
-#notes-rgx=
+notes-rgx=
 
 
 [FORMAT]
 
 # Expected format of line ending, e.g. empty (any line ending), LF or CRLF.
 expected-line-ending-format=
 
@@ -426,17 +527,19 @@
 ignore-long-lines=^\s*(# )?<?https?://\S+>?$
 
 # Number of spaces of indent required inside a hanging or continued line.
 indent-after-paren=4
 
 # String used as indentation unit. This is usually "    " (4 spaces) or "\t" (1
 # tab).
+# indent-string='    '
 indent-string='  '
 
 # Maximum number of characters on a single line.
+# max-line-length=100
 max-line-length=80
 
 # Maximum number of lines in a module.
 max-module-lines=1000
 
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
@@ -458,15 +561,15 @@
 # (hunspell), en_IE (hunspell), en_IN (hunspell), en_JM (hunspell), en_MW
 # (hunspell), en_NA (hunspell), en_NG (hunspell), en_NZ (hunspell), en_PH
 # (hunspell), en_SG (hunspell), en_TT (hunspell), en_US (hunspell), en_ZA
 # (hunspell), en_ZM (hunspell), en_ZW (hunspell).
 spelling-dict=
 
 # List of comma separated words that should be considered directives if they
-# appear and the beginning of a comment and should not be checked.
+# appear at the beginning of a comment and should not be checked.
 spelling-ignore-comment-directives=fmt: on,fmt: off,noqa:,noqa,nosec,isort:skip,mypy:
 
 # List of comma separated words that should not be checked.
 spelling-ignore-words=
 
 # A path to a file that contains the private dictionary; one word per line.
 spelling-private-dict-file=
@@ -481,18 +584,18 @@
 # Comments are removed from the similarity computation
 ignore-comments=yes
 
 # Docstrings are removed from the similarity computation
 ignore-docstrings=yes
 
 # Imports are removed from the similarity computation
-ignore-imports=no
+ignore-imports=yes
 
 # Signatures are removed from the similarity computation
-ignore-signatures=no
+ignore-signatures=yes
 
 # Minimum lines number of a similarity.
 min-similarity-lines=4
 
 
 [STRING]
 
@@ -501,97 +604,25 @@
 check-quote-consistency=no
 
 # This flag controls whether the implicit-str-concat should generate a warning
 # on implicit string concatenation in sequences defined over several lines.
 check-str-concat-over-line-jumps=no
 
 
-[DESIGN]
-
-# List of regular expressions of class ancestor names to ignore when counting
-# public methods (see R0903)
-exclude-too-few-public-methods=
-
-# List of qualified class names to ignore when counting class parents (see
-# R0901)
-ignored-parents=
-
-# Maximum number of arguments for function / method.
-max-args=10
-
-# Maximum number of attributes for a class (see R0902).
-max-attributes=7
-
-# Maximum number of boolean expressions in an if statement (see R0916).
-max-bool-expr=5
-
-# Maximum number of branch for function / method body.
-max-branches=12
-
-# Maximum number of locals for function / method body.
-max-locals=15
-
-# Maximum number of parents for a class (see R0901).
-max-parents=7
-
-# Maximum number of public methods for a class (see R0904).
-max-public-methods=20
-
-# Maximum number of return / yield for function / method body.
-max-returns=6
-
-# Maximum number of statements in function / method body.
-max-statements=50
-
-# Minimum number of public methods for a class (see R0903).
-min-public-methods=2
-
-
-[CLASSES]
-
-# Warn about protected attribute access inside special methods
-check-protected-access-in-special-methods=no
-
-# List of method names used to declare (i.e. assign) instance attributes.
-defining-attr-methods=__init__,
-                      __new__,
-                      setUp,
-                      __post_init__
-
-# List of member names, which should be excluded from the protected access
-# warning.
-exclude-protected=_asdict,
-                  _fields,
-                  _replace,
-                  _source,
-                  _make
-
-# List of valid names for the first argument in a class method.
-valid-classmethod-first-arg=cls
-
-# List of valid names for the first argument in a metaclass class method.
-valid-metaclass-classmethod-first-arg=cls
-
-
 [IMPORTS]
 
 # List of modules that can be imported at any level, not just the top level
 # one.
 allow-any-import-level=
 
 # Allow wildcard imports from modules that define __all__.
 allow-wildcard-with-all=no
 
-# Analyse import fallback blocks. This can be used to support both Python 2 and
-# 3 compatible code, which means that the block might have code that exists
-# only in one or another interpreter, leading to false positives when analysed.
-analyse-fallback-blocks=no
-
 # Deprecated modules which should not be used, separated by a comma.
-deprecated-modules=optparse,tkinter.tix
+deprecated-modules=
 
 # Output a graph (.gv or any supported image format) of external dependencies
 # to the given file (report RP0402 must not be disabled).
 ext-import-graph=
 
 # Output a graph (.gv or any supported image format) of all (i.e. internal and
 # external) dependencies to the given file (report RP0402 must not be
@@ -609,13 +640,17 @@
 # Force import order to recognize a module as part of a third party library.
 known-third-party=enchant
 
 # Couples of modules and preferred modules, separated by a comma.
 preferred-modules=
 
 
-[EXCEPTIONS]
+[REFACTORING]
 
-# Exceptions that will emit a warning when being caught. Defaults to
-# "BaseException, Exception".
-overgeneral-exceptions=BaseException,
-                       Exception
+# Maximum number of nested blocks for function / method body
+max-nested-blocks=5
+
+# Complete name of functions that never returns. When checking for
+# inconsistent-return-statements if a never returning function is called then
+# it will be considered as an explicit return statement and no message will be
+# printed.
+never-returning-functions=sys.exit,argparse.parse_error
```

### Comparing `dtfabric-20221218/LICENSE` & `dtfabric-20230512/LICENSE`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/MANIFEST.in` & `dtfabric-20230512/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/PKG-INFO` & `dtfabric-20230512/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: dtfabric
-Version: 20221218
+Version: 20230512
 Summary: Data type fabric (dtfabric)
 Home-page: https://github.com/libyal/dtfabric
 Maintainer: Joachim Metz
 Maintainer-email: joachim.metz@gmail.com
 License: Apache License, Version 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/plain
 License-File: LICENSE
 
 dtFabric, or data type fabric, is a project to manage data types and structures, as used in the libyal projects.
-
```

### Comparing `dtfabric-20221218/appveyor.yml` & `dtfabric-20230512/appveyor.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 environment:
   matrix:
-  - DESCRIPTION: "Windows with 32-bit Python 3.10"
+  - DESCRIPTION: "Windows with 32-bit Python 3.11"
     MACHINE_TYPE: "x86"
-    APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2019
-    PYTHON: "C:\\Python310"
-    PYTHON_VERSION: "3.10"
+    APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2022
+    PYTHON: "C:\\Python311"
+    PYTHON_VERSION: "3.11"
     L2TBINARIES_TRACK: "dev"
-  - DESCRIPTION: "Windows with 64-bit Python 3.10"
+  - DESCRIPTION: "Windows with 64-bit Python 3.11"
     MACHINE_TYPE: "amd64"
-    APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2019
-    PYTHON: "C:\\Python310-x64"
-    PYTHON_VERSION: "3.10"
+    APPVEYOR_BUILD_WORKER_IMAGE: Visual Studio 2022
+    PYTHON: "C:\\Python311-x64"
+    PYTHON_VERSION: "3.11"
     L2TBINARIES_TRACK: "dev"
   - DESCRIPTION: "Mac OS with Python 3.11"
     APPVEYOR_BUILD_WORKER_IMAGE: macos-monterey
     HOMEBREW_NO_INSTALL_CLEANUP: 1
 
 install:
 - cmd: "%PYTHON%\\python.exe -m pip install -U pip setuptools twine wheel"
```

### Comparing `dtfabric-20221218/config/appveyor/install.ps1` & `dtfabric-20230512/config/appveyor/install.ps1`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # Script to set up tests on AppVeyor Windows.
 
 $Dependencies = "PyYAML mock"
-$Dependencies = ${Dependencies} -split " "
 
-$Output = Invoke-Expression -Command "git clone https://github.com/log2timeline/l2tdevtools.git ..\l2tdevtools 2>&1"
-Write-Host (${Output} | Out-String)
-
-If ($env:APPVEYOR_REPO_BRANCH -eq "main")
-{
-	$Track = "stable"
-}
-Else
+If ($Dependencies.Length -gt 0)
 {
-	$Track = $env:APPVEYOR_REPO_BRANCH
-}
-New-Item -ItemType "directory" -Name "dependencies"
+	$Dependencies = ${Dependencies} -split " "
 
-$env:PYTHONPATH = "..\l2tdevtools"
+	$Output = Invoke-Expression -Command "git clone https://github.com/log2timeline/l2tdevtools.git ..\l2tdevtools 2>&1" | %{ "$_" }
+	Write-Host (${Output} | Out-String)
 
-$Output = Invoke-Expression -Command "& '${env:PYTHON}\python.exe' ..\l2tdevtools\tools\update.py --download-directory dependencies --machine-type ${env:MACHINE_TYPE} --msi-targetdir ${env:PYTHON} --track ${env:L2TBINARIES_TRACK} ${Dependencies} 2>&1"
-Write-Host (${Output} | Out-String)
+	If ($env:APPVEYOR_REPO_BRANCH -eq "main")
+	{
+		$Track = "stable"
+	}
+	Else
+	{
+		$Track = $env:APPVEYOR_REPO_BRANCH
+	}
+	New-Item -ItemType "directory" -Name "dependencies"
+
+	$env:PYTHONPATH = "..\l2tdevtools"
+
+	$Output = Invoke-Expression -Command "& '${env:PYTHON}\python.exe' ..\l2tdevtools\tools\update.py --download-directory dependencies --machine-type ${env:MACHINE_TYPE} --msi-targetdir ${env:PYTHON} --track ${env:L2TBINARIES_TRACK} ${Dependencies} 2>&1" | %{ "$_" }
+	Write-Host (${Output} | Out-String)
+}
```

### Comparing `dtfabric-20221218/config/appveyor/runtests.sh` & `dtfabric-20230512/config/appveyor/runtests.sh`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/config/dpkg/control` & `dtfabric-20230512/config/dpkg/control`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/config/dpkg/copyright` & `dtfabric-20230512/config/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/docs/conf.py` & `dtfabric-20230512/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/docs/index.rst` & `dtfabric-20230512/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/docs/sources/Format-specification.md` & `dtfabric-20230512/docs/sources/Format-specification.md`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/docs/sources/api/dtfabric.rst` & `dtfabric-20230512/docs/sources/api/dtfabric.rst`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/docs/sources/api/dtfabric.runtime.rst` & `dtfabric-20230512/docs/sources/api/dtfabric.runtime.rst`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/docs/sources/user/Installation-instructions.md` & `dtfabric-20230512/docs/sources/user/Installation-instructions.md`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/dtfabric/data_types.py` & `dtfabric-20230512/dtfabric/data_types.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/dtfabric/decorators.py` & `dtfabric-20230512/dtfabric/decorators.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/dtfabric/definitions.py` & `dtfabric-20230512/dtfabric/definitions.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/dtfabric/errors.py` & `dtfabric-20230512/dtfabric/errors.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/dtfabric/reader.py` & `dtfabric-20230512/dtfabric/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -734,15 +734,17 @@
       values = [value]
 
     supported_values = None
     if values:
       supported_values = []
       for value in values:
         if isinstance(value, str):
-          value = value.encode('ascii')
+          # Note that latin1 is used here since the ascii encoding is limited
+          # to 127 characters.
+          value = value.encode('latin1')
 
         supported_values.append(value)
 
     if type_indicator is not None:
       data_type_callback = self._DATA_TYPE_CALLBACKS.get(type_indicator, None)
       if data_type_callback:
         data_type_callback = getattr(self, data_type_callback, None)
```

### Comparing `dtfabric-20221218/dtfabric/registry.py` & `dtfabric-20230512/dtfabric/registry.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/dtfabric/runtime/byte_operations.py` & `dtfabric-20230512/dtfabric/runtime/byte_operations.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/dtfabric/runtime/data_maps.py` & `dtfabric-20230512/dtfabric/runtime/data_maps.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/dtfabric/runtime/fabric.py` & `dtfabric-20230512/dtfabric/runtime/fabric.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/dtfabric/runtime/runtime.py` & `dtfabric-20230512/dtfabric/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/dtfabric.egg-info/PKG-INFO` & `dtfabric-20230512/dtfabric.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: dtfabric
-Version: 20221218
+Version: 20230512
 Summary: Data type fabric (dtfabric)
 Home-page: https://github.com/libyal/dtfabric
 Maintainer: Joachim Metz
 Maintainer-email: joachim.metz@gmail.com
 License: Apache License, Version 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/plain
 License-File: LICENSE
 
 dtFabric, or data type fabric, is a project to manage data types and structures, as used in the libyal projects.
-
```

### Comparing `dtfabric-20221218/dtfabric.egg-info/SOURCES.txt` & `dtfabric-20230512/dtfabric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/run_tests.py` & `dtfabric-20230512/run_tests.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/scripts/validate-definitions.py` & `dtfabric-20230512/scripts/validate-definitions.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/setup.py` & `dtfabric-20230512/setup.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/test_data/Notepad.lnk` & `dtfabric-20230512/test_data/Notepad.lnk`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/test_data/definitions/booleans.yaml` & `dtfabric-20230512/test_data/definitions/booleans.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/test_data/definitions/integers.yaml` & `dtfabric-20230512/test_data/definitions/integers.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/test_data/enumeration.yaml` & `dtfabric-20230512/test_data/enumeration.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/test_data/format.yaml` & `dtfabric-20230512/test_data/format.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/test_data/sequence_with_context.yaml` & `dtfabric-20230512/test_data/sequence_with_context.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/test_data/stream.yaml` & `dtfabric-20230512/test_data/stream.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/test_data/string.yaml` & `dtfabric-20230512/test_data/string.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/test_data/string_array.yaml` & `dtfabric-20230512/test_data/string_array.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/test_data/structure.yaml` & `dtfabric-20230512/test_data/structure.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/test_data/structure_family.yaml` & `dtfabric-20230512/test_data/structure_family.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/test_data/structure_group.yaml` & `dtfabric-20230512/test_data/structure_group.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/test_data/structure_with_condition.yaml` & `dtfabric-20230512/test_data/structure_with_condition.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/test_data/structure_with_padding.yaml` & `dtfabric-20230512/test_data/structure_with_padding.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/test_data/structure_with_values.yaml` & `dtfabric-20230512/test_data/structure_with_values.yaml`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/tests/data_types.py` & `dtfabric-20230512/tests/data_types.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/tests/reader.py` & `dtfabric-20230512/tests/reader.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/tests/registry.py` & `dtfabric-20230512/tests/registry.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/tests/runtime/byte_operations.py` & `dtfabric-20230512/tests/runtime/byte_operations.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/tests/runtime/data_maps.py` & `dtfabric-20230512/tests/runtime/data_maps.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/tests/runtime/fabric.py` & `dtfabric-20230512/tests/runtime/fabric.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/tests/runtime/runtime.py` & `dtfabric-20230512/tests/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/tests/test_lib.py` & `dtfabric-20230512/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/utils/dependencies.py` & `dtfabric-20230512/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `dtfabric-20221218/utils/update_release.sh` & `dtfabric-20230512/utils/update_release.sh`

 * *Files identical despite different names*


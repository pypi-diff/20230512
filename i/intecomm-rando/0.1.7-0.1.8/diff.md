# Comparing `tmp/intecomm-rando-0.1.7.tar.gz` & `tmp/intecomm-rando-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intecomm-rando-0.1.7.tar", last modified: Thu May  4 03:04:45 2023, max compression
+gzip compressed data, was "intecomm-rando-0.1.8.tar", last modified: Fri May 12 04:22:54 2023, max compression
```

## Comparing `intecomm-rando-0.1.7.tar` & `intecomm-rando-0.1.8.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-04 03:04:45.838839 intecomm-rando-0.1.7/
--rw-r--r--   0 erikvw     (501) staff       (20)       64 2022-11-18 01:20:32.000000 intecomm-rando-0.1.7/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-18 01:20:32.000000 intecomm-rando-0.1.7/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-04 03:04:45.822990 intecomm-rando-0.1.7/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-04 03:04:45.828479 intecomm-rando-0.1.7/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1645 2023-03-31 00:48:41.000000 intecomm-rando-0.1.7/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1842 2022-11-20 14:10:06.000000 intecomm-rando-0.1.7/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1173 2023-04-22 18:11:43.000000 intecomm-rando-0.1.7/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-18 01:20:32.000000 intecomm-rando-0.1.7/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)      243 2022-11-18 01:20:32.000000 intecomm-rando-0.1.7/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       29 2022-11-18 01:20:32.000000 intecomm-rando-0.1.7/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-18 00:53:59.000000 intecomm-rando-0.1.7/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      189 2022-11-18 01:20:32.000000 intecomm-rando-0.1.7/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1685 2023-05-04 03:04:45.838947 intecomm-rando-0.1.7/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      825 2022-11-18 01:20:32.000000 intecomm-rando-0.1.7/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-11-18 01:20:32.000000 intecomm-rando-0.1.7/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-04 03:04:45.830843 intecomm-rando-0.1.7/intecomm_rando/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-01-23 15:17:21.000000 intecomm-rando-0.1.7/intecomm_rando/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      161 2022-11-18 01:20:32.000000 intecomm-rando-0.1.7/intecomm_rando/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)       72 2023-01-25 03:01:52.000000 intecomm-rando-0.1.7/intecomm_rando/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)      103 2022-11-23 01:14:40.000000 intecomm-rando-0.1.7/intecomm_rando/exceptions.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2749 2023-03-31 00:48:41.000000 intecomm-rando-0.1.7/intecomm_rando/group_eligibility.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1116 2022-11-20 02:31:32.000000 intecomm-rando-0.1.7/intecomm_rando/group_identifier.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-04 03:04:45.834064 intecomm-rando-0.1.7/intecomm_rando/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    24521 2023-03-31 00:48:41.000000 intecomm-rando-0.1.7/intecomm_rando/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3304 2023-03-31 00:48:41.000000 intecomm-rando-0.1.7/intecomm_rando/migrations/0002_alter_historicalregisteredgroup_group_identifier_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:31:32.000000 intecomm-rando-0.1.7/intecomm_rando/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-04 03:04:45.834920 intecomm-rando-0.1.7/intecomm_rando/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      154 2023-05-03 01:50:00.000000 intecomm-rando-0.1.7/intecomm_rando/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      524 2023-03-31 00:48:41.000000 intecomm-rando-0.1.7/intecomm_rando/models/randomization_list.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1849 2023-03-31 00:48:41.000000 intecomm-rando-0.1.7/intecomm_rando/models/registered_group.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3116 2023-05-04 03:04:38.000000 intecomm-rando-0.1.7/intecomm_rando/models/signals.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4962 2023-05-04 03:04:38.000000 intecomm-rando-0.1.7/intecomm_rando/randomize_group.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1320 2023-01-25 03:01:52.000000 intecomm-rando-0.1.7/intecomm_rando/randomizers.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-04 03:04:45.835475 intecomm-rando-0.1.7/intecomm_rando/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-01-23 15:16:20.000000 intecomm-rando-0.1.7/intecomm_rando/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-04 03:04:45.838213 intecomm-rando-0.1.7/intecomm_rando/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      391 2023-01-25 03:01:52.000000 intecomm-rando-0.1.7/intecomm_rando/tests/etc/randomization_list.csv
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.7/intecomm_rando/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.7/intecomm_rando/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-11-20 14:10:06.000000 intecomm-rando-0.1.7/intecomm_rando/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-20 14:10:06.000000 intecomm-rando-0.1.7/intecomm_rando/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-20 14:10:06.000000 intecomm-rando-0.1.7/intecomm_rando/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-20 14:10:06.000000 intecomm-rando-0.1.7/intecomm_rando/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.7/intecomm_rando/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.7/intecomm_rando/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      303 2023-03-31 00:48:41.000000 intecomm-rando-0.1.7/intecomm_rando/tests/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)      294 2022-11-20 02:31:32.000000 intecomm-rando-0.1.7/intecomm_rando/tests/sites.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-04 03:04:45.838565 intecomm-rando-0.1.7/intecomm_rando/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-23 01:14:40.000000 intecomm-rando-0.1.7/intecomm_rando/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)    12293 2023-05-04 03:04:20.000000 intecomm-rando-0.1.7/intecomm_rando/tests/tests/test_rando_group.py
--rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-18 01:20:32.000000 intecomm-rando-0.1.7/intecomm_rando/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-04 03:04:45.831966 intecomm-rando-0.1.7/intecomm_rando.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1685 2023-05-04 03:04:45.000000 intecomm-rando-0.1.7/intecomm_rando.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1605 2023-05-04 03:04:45.000000 intecomm-rando-0.1.7/intecomm_rando.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-04 03:04:45.000000 intecomm-rando-0.1.7/intecomm_rando.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-18 01:20:40.000000 intecomm-rando-0.1.7/intecomm_rando.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       15 2023-05-04 03:04:45.000000 intecomm-rando-0.1.7/intecomm_rando.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1753 2023-03-31 00:48:41.000000 intecomm-rando-0.1.7/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1711 2023-03-31 00:48:41.000000 intecomm-rando-0.1.7/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1159 2023-05-04 03:04:45.839497 intecomm-rando-0.1.7/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:22:54.860658 intecomm-rando-0.1.8/
+-rw-r--r--   0 erikvw     (501) staff       (20)       64 2022-11-18 01:20:32.000000 intecomm-rando-0.1.8/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-18 01:20:32.000000 intecomm-rando-0.1.8/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:22:54.850397 intecomm-rando-0.1.8/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:22:54.854064 intecomm-rando-0.1.8/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1645 2023-03-31 00:48:41.000000 intecomm-rando-0.1.8/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1842 2022-11-20 14:10:06.000000 intecomm-rando-0.1.8/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1173 2023-04-22 18:11:43.000000 intecomm-rando-0.1.8/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-18 01:20:32.000000 intecomm-rando-0.1.8/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)      243 2022-11-18 01:20:32.000000 intecomm-rando-0.1.8/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)       29 2022-11-18 01:20:32.000000 intecomm-rando-0.1.8/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-18 00:53:59.000000 intecomm-rando-0.1.8/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      189 2022-11-18 01:20:32.000000 intecomm-rando-0.1.8/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1685 2023-05-12 04:22:54.860742 intecomm-rando-0.1.8/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      825 2022-11-18 01:20:32.000000 intecomm-rando-0.1.8/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-11-18 01:20:32.000000 intecomm-rando-0.1.8/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:22:54.855952 intecomm-rando-0.1.8/intecomm_rando/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-01-23 15:17:21.000000 intecomm-rando-0.1.8/intecomm_rando/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      161 2022-11-18 01:20:32.000000 intecomm-rando-0.1.8/intecomm_rando/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       72 2023-01-25 03:01:52.000000 intecomm-rando-0.1.8/intecomm_rando/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      103 2022-11-23 01:14:40.000000 intecomm-rando-0.1.8/intecomm_rando/exceptions.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2749 2023-03-31 00:48:41.000000 intecomm-rando-0.1.8/intecomm_rando/group_eligibility.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1116 2022-11-20 02:31:32.000000 intecomm-rando-0.1.8/intecomm_rando/group_identifier.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:22:54.857303 intecomm-rando-0.1.8/intecomm_rando/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    24521 2023-03-31 00:48:41.000000 intecomm-rando-0.1.8/intecomm_rando/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3304 2023-03-31 00:48:41.000000 intecomm-rando-0.1.8/intecomm_rando/migrations/0002_alter_historicalregisteredgroup_group_identifier_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-20 02:31:32.000000 intecomm-rando-0.1.8/intecomm_rando/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:22:54.857969 intecomm-rando-0.1.8/intecomm_rando/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      154 2023-05-03 01:50:00.000000 intecomm-rando-0.1.8/intecomm_rando/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      524 2023-03-31 00:48:41.000000 intecomm-rando-0.1.8/intecomm_rando/models/randomization_list.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1849 2023-03-31 00:48:41.000000 intecomm-rando-0.1.8/intecomm_rando/models/registered_group.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3153 2023-05-12 04:22:47.000000 intecomm-rando-0.1.8/intecomm_rando/models/signals.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4962 2023-05-04 03:04:38.000000 intecomm-rando-0.1.8/intecomm_rando/randomize_group.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1328 2023-05-12 04:22:47.000000 intecomm-rando-0.1.8/intecomm_rando/randomizers.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:22:54.858356 intecomm-rando-0.1.8/intecomm_rando/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-01-23 15:16:20.000000 intecomm-rando-0.1.8/intecomm_rando/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:22:54.860145 intecomm-rando-0.1.8/intecomm_rando/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      391 2023-01-25 03:01:52.000000 intecomm-rando-0.1.8/intecomm_rando/tests/etc/randomization_list.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.8/intecomm_rando/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.8/intecomm_rando/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-11-20 14:10:06.000000 intecomm-rando-0.1.8/intecomm_rando/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-20 14:10:06.000000 intecomm-rando-0.1.8/intecomm_rando/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-20 14:10:06.000000 intecomm-rando-0.1.8/intecomm_rando/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-20 14:10:06.000000 intecomm-rando-0.1.8/intecomm_rando/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.8/intecomm_rando/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-20 14:10:06.000000 intecomm-rando-0.1.8/intecomm_rando/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      303 2023-03-31 00:48:41.000000 intecomm-rando-0.1.8/intecomm_rando/tests/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      294 2022-11-20 02:31:32.000000 intecomm-rando-0.1.8/intecomm_rando/tests/sites.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:22:54.860404 intecomm-rando-0.1.8/intecomm_rando/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-23 01:14:40.000000 intecomm-rando-0.1.8/intecomm_rando/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    12293 2023-05-04 03:04:20.000000 intecomm-rando-0.1.8/intecomm_rando/tests/tests/test_rando_group.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      118 2022-11-18 01:20:32.000000 intecomm-rando-0.1.8/intecomm_rando/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 04:22:54.856801 intecomm-rando-0.1.8/intecomm_rando.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1685 2023-05-12 04:22:54.000000 intecomm-rando-0.1.8/intecomm_rando.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1605 2023-05-12 04:22:54.000000 intecomm-rando-0.1.8/intecomm_rando.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-12 04:22:54.000000 intecomm-rando-0.1.8/intecomm_rando.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-18 01:20:40.000000 intecomm-rando-0.1.8/intecomm_rando.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       15 2023-05-12 04:22:54.000000 intecomm-rando-0.1.8/intecomm_rando.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1753 2023-03-31 00:48:41.000000 intecomm-rando-0.1.8/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1711 2023-03-31 00:48:41.000000 intecomm-rando-0.1.8/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1159 2023-05-12 04:22:54.861053 intecomm-rando-0.1.8/setup.cfg
```

### Comparing `intecomm-rando-0.1.7/.github/workflows/build.yml` & `intecomm-rando-0.1.8/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.7/.gitignore` & `intecomm-rando-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.7/.pre-commit-config.yaml` & `intecomm-rando-0.1.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.7/LICENSE` & `intecomm-rando-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.7/PKG-INFO` & `intecomm-rando-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intecomm-rando
-Version: 0.1.7
+Version: 0.1.8
 Summary: INTECOMM EDC randomization
 Home-page: https://github.com/intecomm-trial/intecomm-rando
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc INTECOMM EDC randomization,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `intecomm-rando-0.1.7/README.rst` & `intecomm-rando-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.7/intecomm_rando/group_eligibility.py` & `intecomm-rando-0.1.8/intecomm_rando/group_eligibility.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.7/intecomm_rando/group_identifier.py` & `intecomm-rando-0.1.8/intecomm_rando/group_identifier.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.7/intecomm_rando/migrations/0001_initial.py` & `intecomm-rando-0.1.8/intecomm_rando/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.7/intecomm_rando/migrations/0002_alter_historicalregisteredgroup_group_identifier_and_more.py` & `intecomm-rando-0.1.8/intecomm_rando/migrations/0002_alter_historicalregisteredgroup_group_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.7/intecomm_rando/models/randomization_list.py` & `intecomm-rando-0.1.8/intecomm_rando/models/randomization_list.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.7/intecomm_rando/models/registered_group.py` & `intecomm-rando-0.1.8/intecomm_rando/models/registered_group.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.7/intecomm_rando/models/signals.py` & `intecomm-rando-0.1.8/intecomm_rando/models/signals.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,19 @@
     dispatch_uid="randomize_group_on_post_save",
 )
 def randomize_patient_group_on_post_save(sender, instance, raw, **kwargs):
     """Randomize a patient group if ready and not already randomized.
 
     Note: may be called by the model or its proxy.
     """
-    if not raw and instance and instance._meta.label_lower.split(".")[1] == "patientgroup":
+    if (
+        not raw
+        and instance
+        and instance._meta.label_lower.split(".")[1] == "patientgrouprando"
+    ):
         if (
             not instance.randomized
             and instance.randomize_now == YES
             and instance.confirm_randomize_now == "RANDOMIZE"
             and instance.status == COMPLETE
         ):
             if not re.match(UUID_PATTERN, str(instance.group_identifier)):
```

### Comparing `intecomm-rando-0.1.7/intecomm_rando/randomize_group.py` & `intecomm-rando-0.1.8/intecomm_rando/randomize_group.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.7/intecomm_rando/randomizers.py` & `intecomm-rando-0.1.8/intecomm_rando/randomizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
     Intervention: Integrated Community-based care
     Control: Integrated clinic-based care
     """
 
     assignment_map = {COMM_INTERVENTION: 1, CLINIC_CONTROL: 2}
     assignment_description_map = {
-        COMM_INTERVENTION: "Integrated Community Care",
-        CLINIC_CONTROL: "Integrated Clinic-based care",
+        COMM_INTERVENTION: "Integrated community-based care",
+        CLINIC_CONTROL: "Integrated facility-based care",
     }
     trial_is_blinded = False
     model: str = "intecomm_rando.randomizationlist"
 
     extra_csv_fieldnames = ["description", "facility_type", "country", "version"]
 
     def __init__(self, **kwargs):
```

### Comparing `intecomm-rando-0.1.7/intecomm_rando/tests/etc/user-rsa-local-private.pem` & `intecomm-rando-0.1.8/intecomm_rando/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.7/intecomm_rando/tests/etc/user-rsa-restricted-private.pem` & `intecomm-rando-0.1.8/intecomm_rando/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.7/intecomm_rando/tests/tests/test_rando_group.py` & `intecomm-rando-0.1.8/intecomm_rando/tests/tests/test_rando_group.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.7/intecomm_rando.egg-info/PKG-INFO` & `intecomm-rando-0.1.8/intecomm_rando.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intecomm-rando
-Version: 0.1.7
+Version: 0.1.8
 Summary: INTECOMM EDC randomization
 Home-page: https://github.com/intecomm-trial/intecomm-rando
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc INTECOMM EDC randomization,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `intecomm-rando-0.1.7/intecomm_rando.egg-info/SOURCES.txt` & `intecomm-rando-0.1.8/intecomm_rando.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.7/pyproject.toml` & `intecomm-rando-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.7/runtests.py` & `intecomm-rando-0.1.8/runtests.py`

 * *Files identical despite different names*

### Comparing `intecomm-rando-0.1.7/setup.cfg` & `intecomm-rando-0.1.8/setup.cfg`

 * *Files identical despite different names*


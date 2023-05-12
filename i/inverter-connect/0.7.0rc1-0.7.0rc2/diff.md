# Comparing `tmp/inverter-connect-0.7.0rc1.tar.gz` & `tmp/inverter-connect-0.7.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inverter-connect-0.7.0rc1.tar", last modified: Tue May  9 16:28:33 2023, max compression
+gzip compressed data, was "inverter-connect-0.7.0rc2.tar", last modified: Fri May 12 07:39:07 2023, max compression
```

## Comparing `inverter-connect-0.7.0rc1.tar` & `inverter-connect-0.7.0rc2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-13 15:18:51.000000 inverter-connect-0.7.0rc1/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-13 15:18:51.000000 inverter-connect-0.7.0rc1/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1570 2023-05-09 16:20:44.000000 inverter-connect-0.7.0rc1/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-13 15:18:51.000000 inverter-connect-0.7.0rc1/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)    17208 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)    16791 2023-05-09 16:26:48.000000 inverter-connect-0.7.0rc1/README.md
--rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:23:42.000000 inverter-connect-0.7.0rc1/cli.py
--rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:24:01.000000 inverter-connect-0.7.0rc1/dev-cli.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/inverter/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-17 13:29:40.000000 inverter-connect-0.7.0rc1/inverter/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-17 13:29:40.000000 inverter-connect-0.7.0rc1/inverter/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/inverter/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/inverter/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-17 13:29:40.000000 inverter-connect-0.7.0rc1/inverter/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-17 13:29:40.000000 inverter-connect-0.7.0rc1/inverter/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)      151 2023-05-08 20:06:40.000000 inverter-connect-0.7.0rc1/inverter/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      186 2023-04-20 19:23:05.000000 inverter-connect-0.7.0rc1/inverter/__main__.py
--rw-rw-r--   0 jens      (1000) users      (100)     4860 2023-05-08 19:17:03.000000 inverter-connect-0.7.0rc1/inverter/api.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/inverter/cli/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 13:29:40.000000 inverter-connect-0.7.0rc1/inverter/cli/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)    14946 2023-05-09 06:54:43.000000 inverter-connect-0.7.0rc1/inverter/cli/cli_app.py
--rw-rw-r--   0 jens      (1000) users      (100)     8894 2023-05-09 16:16:52.000000 inverter-connect-0.7.0rc1/inverter/cli/dev.py
--rw-rw-r--   0 jens      (1000) users      (100)    10495 2023-05-08 19:17:03.000000 inverter-connect-0.7.0rc1/inverter/connection.py
--rw-rw-r--   0 jens      (1000) users      (100)      361 2023-05-08 16:20:47.000000 inverter-connect-0.7.0rc1/inverter/constants.py
--rw-rw-r--   0 jens      (1000) users      (100)     1768 2023-05-06 10:26:14.000000 inverter-connect-0.7.0rc1/inverter/daily_reset.py
--rw-rw-r--   0 jens      (1000) users      (100)     3795 2023-05-09 06:54:47.000000 inverter-connect-0.7.0rc1/inverter/data_types.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/inverter/definitions/
--rw-rw-r--   0 jens      (1000) users      (100)     2918 2023-04-23 17:07:32.000000 inverter-connect-0.7.0rc1/inverter/definitions/deye_2mppt.yaml
--rw-rw-r--   0 jens      (1000) users      (100)      213 2023-05-06 09:30:48.000000 inverter-connect-0.7.0rc1/inverter/definitions/deye_2mppt_validations.yaml
--rw-rw-r--   0 jens      (1000) users      (100)     2260 2023-05-06 10:26:15.000000 inverter-connect-0.7.0rc1/inverter/definitions.py
--rw-rw-r--   0 jens      (1000) users      (100)      538 2023-05-06 10:11:26.000000 inverter-connect-0.7.0rc1/inverter/exceptions.py
--rw-rw-r--   0 jens      (1000) users      (100)     3350 2023-05-09 07:31:07.000000 inverter-connect-0.7.0rc1/inverter/publish_loop.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/inverter/tests/
--rw-rw-r--   0 jens      (1000) users      (100)      256 2023-05-08 19:20:13.000000 inverter-connect-0.7.0rc1/inverter/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      548 2023-05-08 19:29:24.000000 inverter-connect-0.7.0rc1/inverter/tests/fixtures.py
--rw-rw-r--   0 jens      (1000) users      (100)     3293 2023-05-06 10:24:09.000000 inverter-connect-0.7.0rc1/inverter/tests/test_api.py
--rw-rw-r--   0 jens      (1000) users      (100)     1412 2023-05-09 07:33:09.000000 inverter-connect-0.7.0rc1/inverter/tests/test_cli.py
--rw-rw-r--   0 jens      (1000) users      (100)      826 2023-05-06 10:26:14.000000 inverter-connect-0.7.0rc1/inverter/tests/test_connect.py
--rw-rw-r--   0 jens      (1000) users      (100)     5888 2023-05-08 19:33:47.000000 inverter-connect-0.7.0rc1/inverter/tests/test_daily_reset.py
--rw-rw-r--   0 jens      (1000) users      (100)     1563 2023-05-08 19:29:30.000000 inverter-connect-0.7.0rc1/inverter/tests/test_definitions.py
--rw-rw-r--   0 jens      (1000) users      (100)      211 2023-04-17 13:29:40.000000 inverter-connect-0.7.0rc1/inverter/tests/test_doctests.py
--rw-rw-r--   0 jens      (1000) users      (100)     2641 2023-05-03 17:38:17.000000 inverter-connect-0.7.0rc1/inverter/tests/test_project_setup.py
--rw-rw-r--   0 jens      (1000) users      (100)     5436 2023-05-09 06:29:28.000000 inverter-connect-0.7.0rc1/inverter/tests/test_readme.py
--rw-rw-r--   0 jens      (1000) users      (100)     1975 2023-05-08 17:44:09.000000 inverter-connect-0.7.0rc1/inverter/tests/test_user_settings.py
--rw-rw-r--   0 jens      (1000) users      (100)      537 2023-05-09 07:37:24.000000 inverter-connect-0.7.0rc1/inverter/tests/test_user_settings_migrate_old_settings_1.snapshot.toml
--rw-rw-r--   0 jens      (1000) users      (100)     2114 2023-05-08 19:34:46.000000 inverter-connect-0.7.0rc1/inverter/tests/test_validators.py
--rw-rw-r--   0 jens      (1000) users      (100)     2682 2023-05-09 07:37:21.000000 inverter-connect-0.7.0rc1/inverter/user_settings.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/inverter/utilities/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 17:34:28.000000 inverter-connect-0.7.0rc1/inverter/utilities/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     3242 2023-05-09 07:31:16.000000 inverter-connect-0.7.0rc1/inverter/utilities/cli.py
--rw-rw-r--   0 jens      (1000) users      (100)     2187 2023-04-24 08:58:03.000000 inverter-connect-0.7.0rc1/inverter/utilities/modbus_converter.py
--rw-rw-r--   0 jens      (1000) users      (100)     1562 2023-05-06 10:34:37.000000 inverter-connect-0.7.0rc1/inverter/validators.py
--rw-rw-r--   0 jens      (1000) users      (100)      732 2023-05-08 19:17:53.000000 inverter-connect-0.7.0rc1/inverter/verbosity.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/inverter_connect.egg-info/
--rw-rw-r--   0 jens      (1000) users      (100)    17208 2023-05-09 16:28:33.000000 inverter-connect-0.7.0rc1/inverter_connect.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)     1474 2023-05-09 16:28:33.000000 inverter-connect-0.7.0rc1/inverter_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1000) users      (100)        1 2023-05-09 16:28:33.000000 inverter-connect-0.7.0rc1/inverter_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1000) users      (100)       93 2023-05-09 16:28:33.000000 inverter-connect-0.7.0rc1/inverter_connect.egg-info/entry_points.txt
--rw-rw-r--   0 jens      (1000) users      (100)      289 2023-05-09 16:28:33.000000 inverter-connect-0.7.0rc1/inverter_connect.egg-info/requires.txt
--rw-rw-r--   0 jens      (1000) users      (100)        9 2023-05-09 16:28:33.000000 inverter-connect-0.7.0rc1/inverter_connect.egg-info/top_level.txt
--rw-rw-r--   0 jens      (1000) users      (100)     4940 2023-05-08 16:12:10.000000 inverter-connect-0.7.0rc1/pyproject.toml
--rw-rw-r--   0 jens      (1000) users      (100)    53766 2023-05-08 16:13:00.000000 inverter-connect-0.7.0rc1/requirements.dev.txt
--rw-rw-r--   0 jens      (1000) users      (100)     8423 2023-05-08 16:12:42.000000 inverter-connect-0.7.0rc1/requirements.txt
--rw-rw-r--   0 jens      (1000) users      (100)       38 2023-05-09 16:28:33.766603 inverter-connect-0.7.0rc1/setup.cfg
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-12 07:39:07.635541 inverter-connect-0.7.0rc2/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-13 15:18:51.000000 inverter-connect-0.7.0rc2/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-13 15:18:51.000000 inverter-connect-0.7.0rc2/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-12 07:39:07.631541 inverter-connect-0.7.0rc2/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-12 07:39:07.631541 inverter-connect-0.7.0rc2/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1570 2023-05-09 16:20:44.000000 inverter-connect-0.7.0rc2/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-13 15:18:51.000000 inverter-connect-0.7.0rc2/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)    17176 2023-05-12 07:39:07.635541 inverter-connect-0.7.0rc2/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)    16759 2023-05-12 07:14:18.000000 inverter-connect-0.7.0rc2/README.md
+-rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:23:42.000000 inverter-connect-0.7.0rc2/cli.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:24:01.000000 inverter-connect-0.7.0rc2/dev-cli.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-12 07:39:07.635541 inverter-connect-0.7.0rc2/inverter/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-17 13:29:40.000000 inverter-connect-0.7.0rc2/inverter/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-17 13:29:40.000000 inverter-connect-0.7.0rc2/inverter/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-12 07:39:07.631541 inverter-connect-0.7.0rc2/inverter/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-12 07:39:07.635541 inverter-connect-0.7.0rc2/inverter/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-17 13:29:40.000000 inverter-connect-0.7.0rc2/inverter/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-17 13:29:40.000000 inverter-connect-0.7.0rc2/inverter/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)      151 2023-05-12 06:41:05.000000 inverter-connect-0.7.0rc2/inverter/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      186 2023-04-20 19:23:05.000000 inverter-connect-0.7.0rc2/inverter/__main__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4860 2023-05-08 19:17:03.000000 inverter-connect-0.7.0rc2/inverter/api.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-12 07:39:07.635541 inverter-connect-0.7.0rc2/inverter/cli/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 13:29:40.000000 inverter-connect-0.7.0rc2/inverter/cli/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)    14050 2023-05-12 06:40:16.000000 inverter-connect-0.7.0rc2/inverter/cli/cli_app.py
+-rw-rw-r--   0 jens      (1000) users      (100)     9380 2023-05-12 07:19:04.000000 inverter-connect-0.7.0rc2/inverter/cli/dev.py
+-rw-rw-r--   0 jens      (1000) users      (100)    10495 2023-05-08 19:17:03.000000 inverter-connect-0.7.0rc2/inverter/connection.py
+-rw-rw-r--   0 jens      (1000) users      (100)      392 2023-05-12 06:12:26.000000 inverter-connect-0.7.0rc2/inverter/constants.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1768 2023-05-06 10:26:14.000000 inverter-connect-0.7.0rc2/inverter/daily_reset.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3795 2023-05-09 06:54:47.000000 inverter-connect-0.7.0rc2/inverter/data_types.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-12 07:39:07.635541 inverter-connect-0.7.0rc2/inverter/definitions/
+-rw-rw-r--   0 jens      (1000) users      (100)     2918 2023-04-23 17:07:32.000000 inverter-connect-0.7.0rc2/inverter/definitions/deye_2mppt.yaml
+-rw-rw-r--   0 jens      (1000) users      (100)      379 2023-05-12 07:21:52.000000 inverter-connect-0.7.0rc2/inverter/definitions/deye_2mppt_validations.yaml
+-rw-rw-r--   0 jens      (1000) users      (100)     2260 2023-05-06 10:26:15.000000 inverter-connect-0.7.0rc2/inverter/definitions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      538 2023-05-06 10:11:26.000000 inverter-connect-0.7.0rc2/inverter/exceptions.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3350 2023-05-09 07:31:07.000000 inverter-connect-0.7.0rc2/inverter/publish_loop.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-12 07:39:07.635541 inverter-connect-0.7.0rc2/inverter/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)      256 2023-05-08 19:20:13.000000 inverter-connect-0.7.0rc2/inverter/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3390 2023-05-12 07:35:44.000000 inverter-connect-0.7.0rc2/inverter/tests/fixtures.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3293 2023-05-06 10:24:09.000000 inverter-connect-0.7.0rc2/inverter/tests/test_api.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1412 2023-05-09 07:33:09.000000 inverter-connect-0.7.0rc2/inverter/tests/test_cli.py
+-rw-rw-r--   0 jens      (1000) users      (100)      826 2023-05-06 10:26:14.000000 inverter-connect-0.7.0rc2/inverter/tests/test_connect.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5888 2023-05-08 19:33:47.000000 inverter-connect-0.7.0rc2/inverter/tests/test_daily_reset.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1563 2023-05-08 19:29:30.000000 inverter-connect-0.7.0rc2/inverter/tests/test_definitions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      293 2023-05-12 07:35:44.000000 inverter-connect-0.7.0rc2/inverter/tests/test_doctests.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2641 2023-05-03 17:38:17.000000 inverter-connect-0.7.0rc2/inverter/tests/test_project_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5334 2023-05-12 07:37:22.000000 inverter-connect-0.7.0rc2/inverter/tests/test_readme.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3456 2023-05-12 06:33:31.000000 inverter-connect-0.7.0rc2/inverter/tests/test_user_settings.py
+-rw-rw-r--   0 jens      (1000) users      (100)      537 2023-05-09 07:37:24.000000 inverter-connect-0.7.0rc2/inverter/tests/test_user_settings_migrate_old_settings_1.snapshot.toml
+-rw-rw-r--   0 jens      (1000) users      (100)     2114 2023-05-08 19:34:46.000000 inverter-connect-0.7.0rc2/inverter/tests/test_validators.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3549 2023-05-12 07:10:22.000000 inverter-connect-0.7.0rc2/inverter/user_settings.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-12 07:39:07.635541 inverter-connect-0.7.0rc2/inverter/utilities/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 17:34:28.000000 inverter-connect-0.7.0rc2/inverter/utilities/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3242 2023-05-09 07:31:16.000000 inverter-connect-0.7.0rc2/inverter/utilities/cli.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2187 2023-04-24 08:58:03.000000 inverter-connect-0.7.0rc2/inverter/utilities/modbus_converter.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1562 2023-05-06 10:34:37.000000 inverter-connect-0.7.0rc2/inverter/validators.py
+-rw-rw-r--   0 jens      (1000) users      (100)      732 2023-05-08 19:17:53.000000 inverter-connect-0.7.0rc2/inverter/verbosity.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-12 07:39:07.635541 inverter-connect-0.7.0rc2/inverter_connect.egg-info/
+-rw-rw-r--   0 jens      (1000) users      (100)    17176 2023-05-12 07:39:07.000000 inverter-connect-0.7.0rc2/inverter_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     1474 2023-05-12 07:39:07.000000 inverter-connect-0.7.0rc2/inverter_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        1 2023-05-12 07:39:07.000000 inverter-connect-0.7.0rc2/inverter_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       93 2023-05-12 07:39:07.000000 inverter-connect-0.7.0rc2/inverter_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      299 2023-05-12 07:39:07.000000 inverter-connect-0.7.0rc2/inverter_connect.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        9 2023-05-12 07:39:07.000000 inverter-connect-0.7.0rc2/inverter_connect.egg-info/top_level.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     4950 2023-05-12 06:03:54.000000 inverter-connect-0.7.0rc2/pyproject.toml
+-rw-rw-r--   0 jens      (1000) users      (100)    53797 2023-05-12 06:04:25.000000 inverter-connect-0.7.0rc2/requirements.dev.txt
+-rw-rw-r--   0 jens      (1000) users      (100)    22472 2023-05-12 06:04:08.000000 inverter-connect-0.7.0rc2/requirements.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       38 2023-05-12 07:39:07.635541 inverter-connect-0.7.0rc2/setup.cfg
```

### Comparing `inverter-connect-0.7.0rc1/.github/workflows/tests.yml` & `inverter-connect-0.7.0rc2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.7.0rc1/PKG-INFO` & `inverter-connect-0.7.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inverter-connect
-Version: 0.7.0rc1
+Version: 0.7.0rc2
 Summary: Get information from Deye Microinverter
 Author-email: Jens Diemer <inverter-connect@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/inverter-connect
 Project-URL: Source, https://github.com/jedie/inverter-connect
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
@@ -182,17 +182,17 @@
 
 [comment]: <> (✂✂✂ auto generated read-register help start ✂✂✂)
 ```
 Usage: ./cli.py read-register [OPTIONS] REGISTER LENGTH
 
  Read register(s) from the inverter
  e.g.: read 3 registers starting from 0x16:
- .../inverter-connect$ ./cli.py read-register 192.168.123.456 0x16 3
+ .../inverter-connect$ ./cli.py read-register 0x16 3
  e.g.: read the first 32 registers:
- .../inverter-connect$ ./cli.py read-register 192.168.123.456 0 32
+ .../inverter-connect$ ./cli.py read-register 0 32
  The start address can be pass as decimal number or as hex string, e.g.: 0x123
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ *  --ip             TEXT                     IP address of your inverter [required]              │
 │ *  --port           INTEGER                  Port of inverter services [default: 48899]          │
 │                                              [required]                                          │
 │    --verbosity  -v  INTEGER RANGE [0<=x<=3]  Verbosity level; Accepts integer value e.g.:        │
```

### Comparing `inverter-connect-0.7.0rc1/README.md` & `inverter-connect-0.7.0rc2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -170,17 +170,17 @@
 
 [comment]: <> (✂✂✂ auto generated read-register help start ✂✂✂)
 ```
 Usage: ./cli.py read-register [OPTIONS] REGISTER LENGTH
 
  Read register(s) from the inverter
  e.g.: read 3 registers starting from 0x16:
- .../inverter-connect$ ./cli.py read-register 192.168.123.456 0x16 3
+ .../inverter-connect$ ./cli.py read-register 0x16 3
  e.g.: read the first 32 registers:
- .../inverter-connect$ ./cli.py read-register 192.168.123.456 0 32
+ .../inverter-connect$ ./cli.py read-register 0 32
  The start address can be pass as decimal number or as hex string, e.g.: 0x123
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ *  --ip             TEXT                     IP address of your inverter [required]              │
 │ *  --port           INTEGER                  Port of inverter services [default: 48899]          │
 │                                              [required]                                          │
 │    --verbosity  -v  INTEGER RANGE [0<=x<=3]  Verbosity level; Accepts integer value e.g.:        │
```

### Comparing `inverter-connect-0.7.0rc1/cli.py` & `inverter-connect-0.7.0rc2/cli.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.7.0rc1/dev-cli.py` & `inverter-connect-0.7.0rc2/dev-cli.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.7.0rc1/inverter/.github/workflows/tests.yml` & `inverter-connect-0.7.0rc2/inverter/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.7.0rc1/inverter/api.py` & `inverter-connect-0.7.0rc2/inverter/api.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.7.0rc1/inverter/cli/cli_app.py` & `inverter-connect-0.7.0rc2/inverter/cli/cli_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,30 @@
 """
 
 import logging
 import sys
 import time
 from pathlib import Path
 
+import rich_click
 import rich_click as click
 from bx_py_utils.path import assert_is_file
 from ha_services.mqtt4homeassistant.mqtt import get_connected_client
-from ha_services.toml_settings.api import debug_print_user_settings, edit_user_settings, get_user_settings
+from ha_services.toml_settings.api import TomlSettings
 from ha_services.toml_settings.exceptions import UserSettingsNotFound
 from rich import print  # noqa
+from rich.console import Console
+from rich.traceback import install as rich_traceback_install
 from rich_click import RichGroup
 
 import inverter
 from inverter import constants
 from inverter.api import Inverter, set_current_time
 from inverter.connection import InverterSock
-from inverter.constants import ERROR_STR_NO_DATA, USER_SETTINGS_PATH
+from inverter.constants import ERROR_STR_NO_DATA, SETTINGS_DIR_NAME, SETTINGS_FILE_NAME
 from inverter.data_types import Parameter, ValueType
 from inverter.exceptions import ReadInverterError
 from inverter.publish_loop import publish_forever
 from inverter.user_settings import UserSettings, make_config, migrate_old_settings
 from inverter.utilities.cli import convert_address_option, print_register
 from inverter.verbosity import OPTION_KWARGS_VERBOSE, setup_logging
 
@@ -80,23 +83,24 @@
 
 cli.add_command(version)
 
 
 ######################################################################################################
 # User settings
 
-
-migrate_old_settings()  # TODO: Remove in the Future
+toml_settings = TomlSettings(
+    dir_name=SETTINGS_DIR_NAME,
+    file_name=SETTINGS_FILE_NAME,
+    settings_dataclass=UserSettings(),
+)
+migrate_old_settings(toml_settings)  # TODO: Remove in the Future
 
 try:
-    user_settings: UserSettings = get_user_settings(user_settings=UserSettings(), settings_path=USER_SETTINGS_PATH)
+    user_settings: UserSettings = toml_settings.get_user_settings(debug=True)
 except UserSettingsNotFound:
-    print(f'[red]No settings file found: [yellow]{USER_SETTINGS_PATH}')
-    input('Press any key, to create it')
-    edit_user_settings(user_settings=UserSettings(), settings_path=USER_SETTINGS_PATH)
     sys.exit(1)
 
 
 option_kwargs_ip = dict(
     required=True,
     type=str,
     help='IP address of your inverter',
@@ -122,31 +126,28 @@
 @click.command()
 @click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
 def edit_settings(verbosity: int):
     """
     Edit the settings file. On first call: Create the default one.
     """
     setup_logging(verbosity=verbosity)
-    edit_user_settings(user_settings=UserSettings(), settings_path=USER_SETTINGS_PATH)
+    toml_settings.open_in_editor()
 
 
 cli.add_command(edit_settings)
 
 
 @click.command()
 @click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
 def debug_settings(verbosity: int):
     """
     Display (anonymized) MQTT server username and password
     """
     setup_logging(verbosity=verbosity)
-    try:
-        debug_print_user_settings(user_settings=UserSettings(), settings_path=USER_SETTINGS_PATH)
-    except UserSettingsNotFound as err:
-        print(f'[yellow]No settings created yet[/yellow]: {err} [green](Hint: call "edit-settings" first!)')
+    toml_settings.print_settings()
 
 
 cli.add_command(debug_settings)
 
 
 ######################################################################################################
 
@@ -158,18 +159,14 @@
 @click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
 def print_values(ip, port, inverter, verbosity: int):
     """
     Print all known register values from Inverter, e.g.:
 
     .../inverter-connect$ ./cli.py print-values 192.168.123.456
     """
-    if user_settings is None:
-        print('[yellow]No settings created yet! [green]Call "edit-settings" first!')
-        return
-
     setup_logging(verbosity=verbosity)
 
     print()
 
     config = make_config(
         user_settings=user_settings,
         verbosity=verbosity,
@@ -235,18 +232,14 @@
 
     wait a while and request the current date time:
 
     .../inverter-connect$ ./cli.py print-at-commands 192.168.123.456 NTPTM
 
     (Note: The prefix "AT+" will be added to every command)
     """
-    if user_settings is None:
-        print('[yellow]No settings created yet! [green]Call "edit-settings" first!')
-        return
-
     setup_logging(verbosity=verbosity)
 
     if not commands:
         commands = (
             # 'KEY',  # Set/Get Device Password
             'VER',
             'BVER',  # bootloader version
@@ -324,18 +317,14 @@
     Set current date time in the inverter device.
 
     Default start address is 0x16, so that this will be filled:
         0x16 - year + month
         0x17 - day + hour
         0x18 - minute + second
     """
-    if user_settings is None:
-        print('[yellow]No settings created yet! [green]Call "edit-settings" first!')
-        return
-
     setup_logging(verbosity=verbosity)
 
     address = convert_address_option(raw_address=register, debug=bool(verbosity))
 
     config = make_config(
         user_settings=user_settings,
         verbosity=verbosity,
@@ -374,25 +363,22 @@
 @click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
 def read_register(ip, port, register, length, verbosity: int):
     """
     Read register(s) from the inverter
 
     e.g.: read 3 registers starting from 0x16:
 
-        .../inverter-connect$ ./cli.py read-register 192.168.123.456 0x16 3
+        .../inverter-connect$ ./cli.py read-register 0x16 3
 
     e.g.: read the first 32 registers:
 
-    .../inverter-connect$ ./cli.py read-register 192.168.123.456 0 32
+    .../inverter-connect$ ./cli.py read-register 0 32
 
     The start address can be pass as decimal number or as hex string, e.g.: 0x123
     """
-    if user_settings is None:
-        print('[yellow]No settings created yet! [green]Call "edit-settings" first!')
-        return
 
     setup_logging(verbosity=verbosity)
 
     print(f'Read {length} register(s) from {register=!r} ({ip}:{port})')
     address = convert_address_option(raw_address=register, debug=bool(verbosity))
 
     config = make_config(
@@ -422,17 +408,14 @@
 
 @click.command()
 @click.option('-v', '--verbosity', **OPTION_KWARGS_VERBOSE)
 def test_mqtt_connection(verbosity: int):
     """
     Test connection to MQTT Server
     """
-    if user_settings is None:
-        print('[yellow]No settings created yet! [green]Call "edit-settings" first!')
-        return
 
     setup_logging(verbosity=verbosity)
 
     mqttc = get_connected_client(settings=user_settings.mqtt, verbose=True)
     mqttc.loop_start()
     mqttc.loop_stop()
     mqttc.disconnect()
@@ -450,17 +433,14 @@
 def publish_loop(ip, port, inverter, verbosity: int):
     """
     Publish current data via MQTT for Home Assistant (endless loop)
 
     The "Daily Production" count will be cleared in the night,
     by set the current date time via AT-command.
     """
-    if user_settings is None:
-        print('[yellow]No settings created yet! [green]Call "edit-settings" first!')
-        return
 
     setup_logging(verbosity=verbosity)
 
     config = make_config(
         user_settings=user_settings,
         verbosity=verbosity,
         ip=ip,
@@ -475,10 +455,18 @@
 
 cli.add_command(publish_loop)
 
 
 def main():
     print(f'[bold][green]{inverter.__name__}[/green] v[cyan]{inverter.__version__}')
 
+    console = Console()
+    rich_traceback_install(
+        width=console.size.width,  # full terminal width
+        show_locals=True,
+        suppress=[click, rich_click],
+        max_frames=2,
+    )
+
     # Execute Click CLI:
     cli.name = './cli.py'
     cli()
```

### Comparing `inverter-connect-0.7.0rc1/inverter/cli/dev.py` & `inverter-connect-0.7.0rc2/inverter/cli/dev.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """
     CLI for development
 """
 import logging
+import os
 import sys
 from pathlib import Path
 
 import rich_click as click
 import tomlkit
 from bx_py_utils.path import assert_is_file
+from ha_services.toml_settings.api import TomlSettings
 from ha_services.toml_settings.serialize import dataclass2toml
 from manageprojects.utilities import code_style
 from manageprojects.utilities.publish import publish_package
 from manageprojects.utilities.subprocess_utils import verbose_check_call
 from manageprojects.utilities.version_info import print_version
 from rich import print  # noqa; noqa
 from rich_click import RichGroup
 from tomlkit import TOMLDocument
 
 import inverter
 from inverter import constants
-from inverter.constants import USER_SETTINGS_PATH
+from inverter.constants import SETTINGS_DIR_NAME, SETTINGS_FILE_NAME
 from inverter.user_settings import UserSettings
 
 
 logger = logging.getLogger(__name__)
 
 
 PACKAGE_ROOT = Path(inverter.__file__).parent.parent
@@ -305,24 +307,36 @@
 
 
 cli.add_command(version)
 
 
 ######################################################################################################
 @click.command()
-def create_default_settings():
+@click.option('--force', **OPTION_ARGS_DEFAULT_FALSE)
+def create_default_settings(force):
     """
     Create a default user settings file. (Used by CI pipeline ;)
     """
-    settings_path = Path(USER_SETTINGS_PATH).expanduser()
+    if not force and 'CI' not in os.environ:
+        print('We are not running in CI pipeline and "--force" not used -> Abort.')
+        sys.exit(-1)
+
+    settings_dataclass = UserSettings()
+    toml_settings = TomlSettings(
+        dir_name=SETTINGS_DIR_NAME,
+        file_name=SETTINGS_FILE_NAME,
+        settings_dataclass=settings_dataclass,
+    )
+
+    settings_path = toml_settings.file_path
     if settings_path.is_file():
         print(f'[green]Use settings file already exists here: {settings_path}')
         return
 
-    document: TOMLDocument = dataclass2toml(instance=UserSettings())
+    document: TOMLDocument = dataclass2toml(instance=settings_dataclass)
     doc_str = tomlkit.dumps(document, sort_keys=False)
 
     settings_path.write_text(doc_str, encoding='UTF-8')
     print(f'[green]Default settings file created here: {settings_path}')
 
 
 cli.add_command(create_default_settings)
```

### Comparing `inverter-connect-0.7.0rc1/inverter/connection.py` & `inverter-connect-0.7.0rc2/inverter/connection.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.7.0rc1/inverter/daily_reset.py` & `inverter-connect-0.7.0rc2/inverter/daily_reset.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.7.0rc1/inverter/data_types.py` & `inverter-connect-0.7.0rc2/inverter/data_types.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.7.0rc1/inverter/definitions/deye_2mppt.yaml` & `inverter-connect-0.7.0rc2/inverter/definitions/deye_2mppt.yaml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.7.0rc1/inverter/definitions.py` & `inverter-connect-0.7.0rc2/inverter/definitions.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.7.0rc1/inverter/exceptions.py` & `inverter-connect-0.7.0rc2/inverter/exceptions.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.7.0rc1/inverter/publish_loop.py` & `inverter-connect-0.7.0rc2/inverter/publish_loop.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.7.0rc1/inverter/tests/test_api.py` & `inverter-connect-0.7.0rc2/inverter/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.7.0rc1/inverter/tests/test_cli.py` & `inverter-connect-0.7.0rc2/inverter/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.7.0rc1/inverter/tests/test_connect.py` & `inverter-connect-0.7.0rc2/inverter/tests/test_connect.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.7.0rc1/inverter/tests/test_daily_reset.py` & `inverter-connect-0.7.0rc2/inverter/tests/test_daily_reset.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.7.0rc1/inverter/tests/test_definitions.py` & `inverter-connect-0.7.0rc2/inverter/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.7.0rc1/inverter/tests/test_project_setup.py` & `inverter-connect-0.7.0rc2/inverter/tests/test_project_setup.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.7.0rc1/inverter/tests/test_readme.py` & `inverter-connect-0.7.0rc2/inverter/tests/test_readme.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 import tempfile
 from pathlib import Path
 
-import tomlkit
 from bx_py_utils.auto_doc import assert_readme_block
-from bx_py_utils.environ import OverrideEnviron
 from bx_py_utils.path import assert_is_file
-from click._compat import strip_ansi
-from ha_services.toml_settings.serialize import dataclass2toml
 from manageprojects.test_utils.click_cli_utils import subprocess_cli
 from manageprojects.tests.base import BaseTestCase
-from tomlkit import TOMLDocument
 
 from inverter import constants
 from inverter.cli.cli_app import PACKAGE_ROOT
-from inverter.constants import USER_SETTINGS_PATH
+from inverter.tests.fixtures import MockedUserSetting
 from inverter.user_settings import UserSettings
 
 
 def assert_cli_help_in_readme(text_block: str, marker: str):
     README_PATH = PACKAGE_ROOT / 'README.md'
     assert_is_file(README_PATH)
 
@@ -38,24 +33,26 @@
         So we can't directly invoke_click() here, because user settings are read and
         used on module level!
         So we must use subprocess and use a default settings file!
         """
         with tempfile.TemporaryDirectory(prefix='test-inverter-connect') as temp_dir:
             temp_path = Path(temp_dir)
 
-            with OverrideEnviron(HOME=temp_dir, TERM='dump', PYTHONUNBUFFERED='1'):
+            with MockedUserSetting(
+                temp_path=temp_path, settings_dataclass=UserSettings, COLUMNS='120', TERM='dump', NO_COLOR='1'
+            ) as user_settings_mock:
                 assert Path('~').expanduser() == temp_path
 
-                document: TOMLDocument = dataclass2toml(instance=UserSettings())
-                doc_str = tomlkit.dumps(document, sort_keys=False)
-                Path(USER_SETTINGS_PATH).expanduser().write_text(doc_str, encoding='UTF-8')
+                toml_file_path = temp_path / '.config' / 'inverter-connect' / 'inverter-connect.toml'
+                assert user_settings_mock.settings_file_path == toml_file_path
+                assert_is_file(toml_file_path)
 
                 stdout = subprocess_cli(cli_bin=cli_bin, args=args)
 
-                stdout = strip_ansi(stdout)  # FIXME
+                # stdout = strip_ansi(stdout)  # FIXME
 
                 # Skip header stuff:
                 lines = stdout.splitlines()
                 for pos, line in enumerate(lines):
                     if line.lstrip().startswith('Usage: ./'):
                         stdout = '\n'.join(lines[pos:])
                         break
```

### Comparing `inverter-connect-0.7.0rc1/inverter/tests/test_user_settings.py` & `inverter-connect-0.7.0rc2/inverter/tests/test_user_settings.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,50 +2,80 @@
 import tempfile
 from pathlib import Path
 from unittest import TestCase
 
 from bx_py_utils.environ import OverrideEnviron
 from bx_py_utils.path import assert_is_file
 from bx_py_utils.test_utils.snapshot import assert_text_snapshot
+from ha_services.toml_settings.api import TomlSettings
 
-from inverter.user_settings import migrate_old_settings
+from inverter.user_settings import UserSettings, migrate_old_settings
 
 
 class UserSettingsTestCase(TestCase):
     def test_migrate_old_settings(self):
         with tempfile.TemporaryDirectory(prefix='test-inverter-connect') as temp_dir:
             temp_path = Path(temp_dir)
             with OverrideEnviron(HOME=temp_dir):
                 assert Path('~').expanduser() == temp_path
+                Path(temp_path / '.config').mkdir()
 
+                toml_settings = TomlSettings(
+                    dir_name='test_dir_name',
+                    file_name='test_file_name',
+                    settings_dataclass=UserSettings(),
+                )
+
+                # Test convert the old, old settings file:
                 old_settings_path = temp_path / '.inverter-connect'
                 old_settings_path.write_text(
                     json.dumps(
                         dict(
                             host='my-mosquitto.tld',
                             port=1883,
                             user_name='test-user',
                             password='NoSecurePassword',
                         )
                     )
                 )
 
+                # Test: '~/.inverter-connect' -> '~/config/inverter-connect/inverter-connect.toml'
+                with self.assertLogs(logger=None) as logs:
+                    migrate_old_settings(toml_settings)
+
+                self.assertEqual(
+                    logs.output,
+                    [
+                        f'INFO:root:Migrate v1 settings from: {temp_dir}/.inverter-connect',
+                        f'INFO:root:Migrate settings to: {temp_dir}/.config/test_dir_name/test_file_name.toml',
+                    ],
+                )
+                self.assertFalse(Path(f'{temp_dir}/.inverter-connect').exists())
+
+                # Test: '~/.inverter-connect.toml' -> '~/config/inverter-connect/inverter-connect.toml'
+                Path(f'{temp_dir}/.config/test_dir_name/test_file_name.toml').rename(
+                    Path(f'{temp_dir}/.inverter-connect.toml')
+                )
+                Path(f'{temp_dir}/.config/test_dir_name/').rmdir()
                 with self.assertLogs(logger=None) as logs:
-                    migrate_old_settings()
+                    migrate_old_settings(toml_settings)
 
                 self.assertEqual(
                     logs.output,
                     [
-                        f'INFO:root:Migrate old settings from: {temp_dir}/.inverter-connect',
-                        f'INFO:root:Migrate settings to: {temp_dir}/.inverter-connect.toml',
+                        (
+                            'INFO:root:Move settings file '
+                            f'{temp_dir}/.inverter-connect.toml to '
+                            f'{temp_dir}/.config/test_dir_name/test_file_name.toml'
+                        ),
                     ],
                 )
 
             self.assertFalse(old_settings_path.is_file())
-            new_settings_path = temp_path / '.inverter-connect.toml'
+            new_settings_path = Path(f'{temp_dir}/.config/test_dir_name/test_file_name.toml')
             assert_is_file(new_settings_path)
             new_settings_str = new_settings_path.read_text()
 
         self.assertIn('[mqtt]', new_settings_str)
         self.assertIn('host = "my-mosquitto.tld"', new_settings_str)
         self.assertIn('password = "NoSecurePassword"', new_settings_str)
```

### Comparing `inverter-connect-0.7.0rc1/inverter/tests/test_user_settings_migrate_old_settings_1.snapshot.toml` & `inverter-connect-0.7.0rc2/inverter/tests/test_user_settings_migrate_old_settings_1.snapshot.toml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.7.0rc1/inverter/tests/test_validators.py` & `inverter-connect-0.7.0rc2/inverter/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.7.0rc1/inverter/user_settings.py` & `inverter-connect-0.7.0rc2/inverter/user_settings.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 import json
 import logging
 import socket
 from pathlib import Path
 
 import tomlkit
 from ha_services.mqtt4homeassistant.data_classes import MqttSettings as OriginMqttSettings
+from ha_services.toml_settings.api import TomlSettings
 from ha_services.toml_settings.serialize import dataclass2toml
 from rich import print  # noqa
 from tomlkit import TOMLDocument
 
-from inverter.constants import USER_SETTINGS_PATH
 from inverter.data_types import Config
 from inverter.utilities.cli import exit_with_human_error
 
 
 @dataclasses.dataclass
 class MqttSettings(OriginMqttSettings):
     """
@@ -45,38 +45,51 @@
     User settings for inverter-connect
     """
 
     mqtt: dataclasses = dataclasses.field(default_factory=MqttSettings)
     inverter: dataclasses = dataclasses.field(default_factory=Inverter)
 
 
-def migrate_old_settings():  # TODO: Remove in the Future
-    new_settings_path = Path(USER_SETTINGS_PATH).expanduser()
-    if new_settings_path.is_file():
+def migrate_old_settings(toml_settings: TomlSettings):  # TODO: Remove in the Future
+    file_path = toml_settings.file_path  # '~/config/inverter-connect/inverter-connect.toml'
+    if file_path.is_file():
+        logging.debug('v2 settings file exists: %s -> no migration needed', file_path)
         return
+    else:
+        logging.debug('v2 settings not exists: %s -> try migration', file_path)
 
-    old_settings_path = Path('~/.inverter-connect').expanduser()
-    if not old_settings_path.is_file():
-        return
-
-    logging.info('Migrate old settings from: %s', old_settings_path)
-    settings_str = old_settings_path.read_text(encoding='UTF-8')
-    data = json.loads(settings_str)
-    mqtt = MqttSettings(**data)
-    user_settings = UserSettings()
-    user_settings.mqtt = mqtt
-
-    document: TOMLDocument = dataclass2toml(instance=user_settings)
-    doc_str = tomlkit.dumps(document, sort_keys=False)
-
-    new_settings_path.write_text(doc_str, encoding='UTF-8')
-
-    logging.info('Migrate settings to: %s', new_settings_path)
-
-    old_settings_path.unlink()
+    # '~/.inverter-connect' -> '~/config/inverter-connect/inverter-connect.toml'
+    v1_settings_path = Path('~/.inverter-connect').expanduser()
+    if v1_settings_path.is_file():
+        logging.info('Migrate v1 settings from: %s', v1_settings_path)
+        settings_str = v1_settings_path.read_text(encoding='UTF-8')
+        assert settings_str, f'Empty file: {v1_settings_path} (Please remove it!)'
+        data = json.loads(settings_str)
+        mqtt = MqttSettings(**data)
+        user_settings = UserSettings()
+        user_settings.mqtt = mqtt
+
+        document: TOMLDocument = dataclass2toml(instance=user_settings)
+        doc_str = tomlkit.dumps(document, sort_keys=False)
+
+        file_path.write_text(doc_str, encoding='UTF-8')
+
+        logging.info('Migrate settings to: %s', file_path)
+
+        v1_settings_path.unlink()
+    else:
+        logging.debug('No v1 settings file: %s', v1_settings_path)
+
+        v2_settings_path = Path('~/.inverter-connect.toml').expanduser()
+        if v2_settings_path.is_file():
+            logging.info('Move settings file %s to %s', v2_settings_path, file_path)
+            file_path.parent.mkdir(exist_ok=True)
+            v2_settings_path.rename(file_path)
+        else:
+            logging.debug('No old settings file found here: %s', v2_settings_path)
 
 
 def make_config(*, user_settings: UserSettings, ip, port, verbosity, inverter=None) -> Config:
     # "Validate" ip address:
     try:
         result = socket.gethostbyname(ip)
     except socket.gaierror as err:
```

### Comparing `inverter-connect-0.7.0rc1/inverter/utilities/cli.py` & `inverter-connect-0.7.0rc2/inverter/utilities/cli.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.7.0rc1/inverter/utilities/modbus_converter.py` & `inverter-connect-0.7.0rc2/inverter/utilities/modbus_converter.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.7.0rc1/inverter/validators.py` & `inverter-connect-0.7.0rc2/inverter/validators.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.7.0rc1/inverter/verbosity.py` & `inverter-connect-0.7.0rc2/inverter/verbosity.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.7.0rc1/inverter_connect.egg-info/PKG-INFO` & `inverter-connect-0.7.0rc2/inverter_connect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inverter-connect
-Version: 0.7.0rc1
+Version: 0.7.0rc2
 Summary: Get information from Deye Microinverter
 Author-email: Jens Diemer <inverter-connect@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/inverter-connect
 Project-URL: Source, https://github.com/jedie/inverter-connect
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
@@ -182,17 +182,17 @@
 
 [comment]: <> (✂✂✂ auto generated read-register help start ✂✂✂)
 ```
 Usage: ./cli.py read-register [OPTIONS] REGISTER LENGTH
 
  Read register(s) from the inverter
  e.g.: read 3 registers starting from 0x16:
- .../inverter-connect$ ./cli.py read-register 192.168.123.456 0x16 3
+ .../inverter-connect$ ./cli.py read-register 0x16 3
  e.g.: read the first 32 registers:
- .../inverter-connect$ ./cli.py read-register 192.168.123.456 0 32
+ .../inverter-connect$ ./cli.py read-register 0 32
  The start address can be pass as decimal number or as hex string, e.g.: 0x123
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ *  --ip             TEXT                     IP address of your inverter [required]              │
 │ *  --port           INTEGER                  Port of inverter services [default: 48899]          │
 │                                              [required]                                          │
 │    --verbosity  -v  INTEGER RANGE [0<=x<=3]  Verbosity level; Accepts integer value e.g.:        │
```

### Comparing `inverter-connect-0.7.0rc1/inverter_connect.egg-info/SOURCES.txt` & `inverter-connect-0.7.0rc2/inverter_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.7.0rc1/pyproject.toml` & `inverter-connect-0.7.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 license = {text = "GPL-3.0-or-later"}
 readme = "README.md"
 authors = [
     {name = 'Jens Diemer', email = 'inverter-connect@jensdiemer.de'}
 ]
 requires-python = ">=3.9,<4"
 dependencies = [
-    "ha-services", # https://github.com/jedie/ha-services
+    "ha-services>=0.2.0rc0", # https://github.com/jedie/ha-services
     "paho-mqtt",  # https://pypi.org/project/paho-mqtt/
     "msgspec",  # https://github.com/jcrist/msgspec
     "pyyaml",  # https://github.com/yaml/pyyaml
     "bx_py_utils",  # https://github.com/boxine/bx_py_utils
     "click",  # https://github.com/pallets/click/
     "rich-click",  # https://github.com/ewels/rich-click
     "rich",  # https://github.com/Textualize/rich
```

### Comparing `inverter-connect-0.7.0rc1/requirements.dev.txt` & `inverter-connect-0.7.0rc2/requirements.dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -321,17 +321,17 @@
     --hash=sha256:cf4173be4ad2982e5b2ebab7e08bd0d27173f2459ec1b1cf66aec9290da80cce \
     --hash=sha256:d72126418194871aeaf1e8aa620ad06edc5472848bef71c4d393c22b65571878
     # via inverter-connect (pyproject.toml)
 distlib==0.3.6 \
     --hash=sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46 \
     --hash=sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e
     # via virtualenv
-docutils==0.19 \
-    --hash=sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6 \
-    --hash=sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc
+docutils==0.20 \
+    --hash=sha256:a428f10de4de4774389734c986a01b4af2d802d26717108b0f1b9356862937c5 \
+    --hash=sha256:f75a5a52fbcacd81b47e42888ad2b380748aaccfb3f13af0fe69deb759f01eb6
     # via readme-renderer
 dparse==0.6.2 \
     --hash=sha256:8097076f1dd26c377f30d4745e6ec18fef42f3bf493933b842ac5bafad8c345f \
     --hash=sha256:d45255bda21f998bc7ddf2afd5e62505ba6134756ba2d42a84c56b0826614dfe
     # via safety
 editorconfig==0.12.3 \
     --hash=sha256:57f8ce78afcba15c8b18d46b5170848c88d56fd38f05c2ec60dbbfcb8996e89e \
@@ -351,17 +351,17 @@
     --hash=sha256:2863ac8ec19d6ec8d29e760546e6ced644baf6dff3c7cdc77e03abbd29b80f14 \
     --hash=sha256:2bd1b37043ad88a3f3c3c34a76fc0b64d24e5f03d36ea6b48cb69cc642bff17e
     # via darker
 freezegun==1.2.2 \
     --hash=sha256:cd22d1ba06941384410cd967d8a99d5ae2442f57dfafeff2fda5de8dc5c05446 \
     --hash=sha256:ea1b963b993cb9ea195adbd893a48d573fda951b0da64f60883d7e988b606c9f
     # via inverter-connect (pyproject.toml)
-ha-services==0.0.1 \
-    --hash=sha256:9ab060d3afed22ab83176179dc2808ad8b30b7df34b9940897e0ffc5face92ec \
-    --hash=sha256:eeb6a6c30988338ef8aec49bd7f5bf42b764d38452f5051603d7e0b21ed0426c
+ha-services==0.2.0rc0 \
+    --hash=sha256:1e118fd6c6054250a3856c60ae82eb8ad6c3f025f44fa825815aa10d8739cdf4 \
+    --hash=sha256:4c61dcf62918ec5ee1656756aa4cb15aa1c9fe6c57894fcf015e6d8659968d44
     # via inverter-connect (pyproject.toml)
 idna==3.4 \
     --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
     --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
     # via requests
 importlib-metadata==6.6.0 \
     --hash=sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed \
@@ -393,18 +393,20 @@
     --hash=sha256:d14eaa4d315e7688daa4969f616f226614350c48730bfa1692d2caebd8c90d40 \
     --hash=sha256:d3eab6605e3ec8b7a0863df09cc1d23714908fa61aa6986a845c20ba488b4efa
     # via cookiecutter
 keyring==23.13.1 \
     --hash=sha256:771ed2a91909389ed6148631de678f82ddc73737d85a927f382a8a1b157898cd \
     --hash=sha256:ba2e15a9b35e21908d0aaf4e0a47acc52d6ae33444df0da2b49d41a46ef6d678
     # via twine
-manageprojects==0.9.10 \
-    --hash=sha256:5f6aac8e660cc8bc72548afbc300be8d3096f4afd715e1549a4bebedba105c75 \
-    --hash=sha256:be59603525d1f27519bd65717d5dcfe4d81eb75c34df71bb86a3fc4fbe15f0b5
-    # via inverter-connect (pyproject.toml)
+manageprojects==0.10.0 \
+    --hash=sha256:939d9cf9c629be755c2ab6f8ccd4019dfa1c7e39564c25f6087ec2f63867133a \
+    --hash=sha256:db457b77e52a73e3ec5fd4889e056df01926ec0c9b1476ab28c79db254d0465f
+    # via
+    #   ha-services
+    #   inverter-connect (pyproject.toml)
 markdown-it-py==2.2.0 \
     --hash=sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30 \
     --hash=sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1
     # via rich
 markupsafe==2.1.2 \
     --hash=sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed \
     --hash=sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc \
@@ -465,74 +467,74 @@
     --hash=sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8 \
     --hash=sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba
     # via markdown-it-py
 more-itertools==9.1.0 \
     --hash=sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d \
     --hash=sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3
     # via jaraco-classes
-msgspec==0.14.2 \
-    --hash=sha256:03ddc8c518afbea4fb89afb587d77f11d00909f003966d437f31fb8fffdfac28 \
-    --hash=sha256:1c8f7e631fad9d5a33fcfb0f2a27eb86dc0390e91d6b51c95a604b7ccbc264f1 \
-    --hash=sha256:1fc99f0929fa91cc53fa35f59be366d67f116c2b7f0f3b29dc60e3179f6fb205 \
-    --hash=sha256:2039451b22813af2fd5cbe99eaecfc318d64fcee5af0ce5b3d5cce12427d24cd \
-    --hash=sha256:26bcb3a69b348be2757ab19e86038e586920522a99d49d358c12890fbcfb6aa8 \
-    --hash=sha256:3288b65ee7c78d08f32003a8b5ca72fff12c6a7400bd35f9d65630c9d58efce2 \
-    --hash=sha256:4f13e47803aedbb32c9375317fedbd20af3397dc024d311eebdc635c07f6f908 \
-    --hash=sha256:57a79cfa306fda2c66f4fc7eb72836c0f78fd9a6d748d028960b387797f0381b \
-    --hash=sha256:580464c7ca5c47a1422973c853301bbfd3d1a4184bdb6bddb73b5df094d8fc55 \
-    --hash=sha256:587371a65798a0f0182d0a7a4b7c4b87a5f46e25e8821c6474b3f717dcfcad14 \
-    --hash=sha256:59491de3566c7789bdb0a152f305e150a6ba3e825af471680b05a029a664a89a \
-    --hash=sha256:78361dadef4b993b8c4a887d3d267b89b0ea0846259eadf2fe993659e4dbf9c8 \
-    --hash=sha256:7e50885274e2041e49ec5d7cce8e59768f599c27dfb4c046edaf9ab25b1fddc2 \
-    --hash=sha256:87c4cd1bb197be11f89ad779038c8989d6ffcb8b360705107f034e4d2783c0a6 \
-    --hash=sha256:8927efaf506e5a8f9ffe76602e08d30a80c19b38d50a7e783887c317573ecd80 \
-    --hash=sha256:8b8a766b9f3e7f87946965a8ffc6e72f7a3ec8d031b3168df16762bfd3d03205 \
-    --hash=sha256:8ed61cad6b20f0218a8d239294c4b30b4e82854871ba0434cf0d54497043bffe \
-    --hash=sha256:907ed4305a97b50248e6b86e79ddc8edcf9b718eab0c93a6b46d673c5edbe3a4 \
-    --hash=sha256:94fc3d9a8835f18c18b48fdf49f7d445184061bfbc457a6623a4eb1f74ebe806 \
-    --hash=sha256:a0a3908309581e4e632457fac1938fec7fd84121396ddab6ddca37784e6db068 \
-    --hash=sha256:a12e704786256431d559c2027d6135a64f2339f009118d97906709cd8409e7ac \
-    --hash=sha256:b965c14851f146537f1b732cd2ed16c38e0c59662f23b72d396aee21e81aed4f \
-    --hash=sha256:d03861f0d271b696faefb1a885ea0c7dc7db70baaa05c7f18086f2b9085d1cb8 \
-    --hash=sha256:d469aede5d986223d6ec9a8d0713156f96fd6b427b12e14f81d26627a47687b9 \
-    --hash=sha256:d85e9bfd1441216010c084626d968e96a3d88d762959c5eb430de62076cd7fe9 \
-    --hash=sha256:decd1d2015d340ebfd58f29ed2916e118ca255b6a94fc1787a236a2654dfd8ff \
-    --hash=sha256:eee59e73982ca0d730f8d4e8fb5f01da9fa466490dea43ea1bcfa23b8a8bbc0d \
-    --hash=sha256:f97006b9c9e24e9677fb84f43586fb4d03a72eb426199656a1c24775c62b9fe4 \
-    --hash=sha256:ff7c987330e2be62eb8811bc2da33507e8edeb761f4fd343f2fa5fdafce4f989
+msgspec==0.15.0 \
+    --hash=sha256:05fc603508e0c8021249d3e531fa4bb72d167bdfa76d869d48f96a5b8f9b50bf \
+    --hash=sha256:07ee1d1a15e3b319dcd7326470216928a7b58d47460b253577ccd0ab5dcf5c3c \
+    --hash=sha256:0c75fd847709e30265f050375c408fec1c07797694162834aa86ab3b3cf055da \
+    --hash=sha256:1b5b7c1b69416eab3ab2ad1c9593b749226b80555532292fae5fe9d154794089 \
+    --hash=sha256:20bf8018bff6bb85f5315ba6fd47b2f9373ab67e8bb59b0d7a7def22bbbf9f70 \
+    --hash=sha256:22713a1f618b4094c0268c6fbeef530397e5f3fa5292e4afd51caddad645843f \
+    --hash=sha256:2b57b6869ef1717c0343465198e19284d1e6aa5f292af2726284e4dfedfedeef \
+    --hash=sha256:346960762d648a6512b51f30be7c1267630e0bbc6fd65e8b23a3f54e5f562656 \
+    --hash=sha256:381c7a891adcc741e617956ba987912bc21864f9dd27b8cfb03bfb0aded5e1fd \
+    --hash=sha256:415519f68cd3f1a224f87ed415459ac3b86e4f6e82815a036e4238c62006f696 \
+    --hash=sha256:42c2f9fe0b58dc6f2b15720490c67554b5ba0007d3ee94340ca4448bda917287 \
+    --hash=sha256:490c88d76d573cce16653434ace3d9a8a8675ef6e350f114752fe60e69b6a232 \
+    --hash=sha256:4d3cde786110a92f764666b9f963b4389d5d1798bf1aca2422a59931d8d1f694 \
+    --hash=sha256:550b359c49562d52849103b87b4f7381fbc0adf958afa316599befb9a3e3379e \
+    --hash=sha256:8a46a9818570362d4022161684cdb97ecd102953043059ee4902862940f48f8d \
+    --hash=sha256:8b7e0354c37b742e1c02fe0cd3ced97db516c8da62ac5a408609e9f5858aaf24 \
+    --hash=sha256:8cee590163788fce21c5998d09198ef08ec06c1ca68ef50f2d5ed9e54d308538 \
+    --hash=sha256:9178a7550a5516295c682e6e5c143782503719b4c816496349a4a0f1b62397ef \
+    --hash=sha256:9d61de44b248feef82c8979a1e9912c923527cfb1d01c93b7bb5d6ca93ed09d6 \
+    --hash=sha256:beb3789519253b22338cca48053ba5ac8b442633e3af8f58e264d776a98ff6d0 \
+    --hash=sha256:bf3ab3f8d5752dbe68babc77d21b42575b916793515442e3890aef680e212154 \
+    --hash=sha256:c4c7e0abfac3a67f3e1d51e1d1313fd4205528e17663ff264b1945c3370b18bd \
+    --hash=sha256:cc253e4ad51d360590358ab2cee5a6139f04ad994e0fcbff52e7f61fca475c3e \
+    --hash=sha256:cd198ed4445914ebc25a24b6cc6020902bb6b888fc9b39500ef4500841b1b437 \
+    --hash=sha256:d760ff747165d84965791bfcd14588f61f111708036d80f1980387e3760035e7 \
+    --hash=sha256:ddef8fdc06676dd1bec9fe67b3128f84079469ee6424384cbb29a90c9033b559 \
+    --hash=sha256:f77cc91d3cb8a7bccfba28fe4aec537178384509bfce222f8eca287b7e5d0214 \
+    --hash=sha256:ff80bd40469915cc61686086a2503b901e17040f8a191099d8ccaa45dc72df8c \
+    --hash=sha256:fffa7ec85f27577f7f5471b390bf902d58ccd89b3612cf40bfb92f4ba75e6c95
     # via
     #   ha-services
     #   inverter-connect (pyproject.toml)
-mypy==1.2.0 \
-    --hash=sha256:023fe9e618182ca6317ae89833ba422c411469156b690fde6a315ad10695a521 \
-    --hash=sha256:031fc69c9a7e12bcc5660b74122ed84b3f1c505e762cc4296884096c6d8ee140 \
-    --hash=sha256:2de7babe398cb7a85ac7f1fd5c42f396c215ab3eff731b4d761d68d0f6a80f48 \
-    --hash=sha256:2e93a8a553e0394b26c4ca683923b85a69f7ccdc0139e6acd1354cc884fe0128 \
-    --hash=sha256:390bc685ec209ada4e9d35068ac6988c60160b2b703072d2850457b62499e336 \
-    --hash=sha256:3a2d219775a120581a0ae8ca392b31f238d452729adbcb6892fa89688cb8306a \
-    --hash=sha256:3efde4af6f2d3ccf58ae825495dbb8d74abd6d176ee686ce2ab19bd025273f41 \
-    --hash=sha256:4a99fe1768925e4a139aace8f3fb66db3576ee1c30b9c0f70f744ead7e329c9f \
-    --hash=sha256:4b41412df69ec06ab141808d12e0bf2823717b1c363bd77b4c0820feaa37249e \
-    --hash=sha256:4c8d8c6b80aa4a1689f2a179d31d86ae1367ea4a12855cc13aa3ba24bb36b2d8 \
-    --hash=sha256:4d19f1a239d59f10fdc31263d48b7937c585810288376671eaf75380b074f238 \
-    --hash=sha256:4e4a682b3f2489d218751981639cffc4e281d548f9d517addfd5a2917ac78119 \
-    --hash=sha256:695c45cea7e8abb6f088a34a6034b1d273122e5530aeebb9c09626cea6dca4cb \
-    --hash=sha256:701189408b460a2ff42b984e6bd45c3f41f0ac9f5f58b8873bbedc511900086d \
-    --hash=sha256:70894c5345bea98321a2fe84df35f43ee7bb0feec117a71420c60459fc3e1eed \
-    --hash=sha256:8293a216e902ac12779eb7a08f2bc39ec6c878d7c6025aa59464e0c4c16f7eb9 \
-    --hash=sha256:8d26b513225ffd3eacece727f4387bdce6469192ef029ca9dd469940158bc89e \
-    --hash=sha256:a197ad3a774f8e74f21e428f0de7f60ad26a8d23437b69638aac2764d1e06a6a \
-    --hash=sha256:bea55fc25b96c53affab852ad94bf111a3083bc1d8b0c76a61dd101d8a388cf5 \
-    --hash=sha256:c9a084bce1061e55cdc0493a2ad890375af359c766b8ac311ac8120d3a472950 \
-    --hash=sha256:d0e9464a0af6715852267bf29c9553e4555b61f5904a4fc538547a4d67617937 \
-    --hash=sha256:d8e9187bfcd5ffedbe87403195e1fc340189a68463903c39e2b63307c9fa0394 \
-    --hash=sha256:eaeaa0888b7f3ccb7bcd40b50497ca30923dba14f385bde4af78fac713d6d6f6 \
-    --hash=sha256:f46af8d162f3d470d8ffc997aaf7a269996d205f9d746124a179d3abe05ac602 \
-    --hash=sha256:f70a40410d774ae23fcb4afbbeca652905a04de7948eaf0b1789c8d1426b72d1 \
-    --hash=sha256:fe91be1c51c90e2afe6827601ca14353bbf3953f343c2129fa1e247d55fd95ba
+mypy==1.3.0 \
+    --hash=sha256:1c4c42c60a8103ead4c1c060ac3cdd3ff01e18fddce6f1016e08939647a0e703 \
+    --hash=sha256:44797d031a41516fcf5cbfa652265bb994e53e51994c1bd649ffcd0c3a7eccbf \
+    --hash=sha256:473117e310febe632ddf10e745a355714e771ffe534f06db40702775056614c4 \
+    --hash=sha256:4c99c3ecf223cf2952638da9cd82793d8f3c0c5fa8b6ae2b2d9ed1e1ff51ba85 \
+    --hash=sha256:550a8b3a19bb6589679a7c3c31f64312e7ff482a816c96e0cecec9ad3a7564dd \
+    --hash=sha256:658fe7b674769a0770d4b26cb4d6f005e88a442fe82446f020be8e5f5efb2fae \
+    --hash=sha256:6e33bb8b2613614a33dff70565f4c803f889ebd2f859466e42b46e1df76018dd \
+    --hash=sha256:6e42d29e324cdda61daaec2336c42512e59c7c375340bd202efa1fe0f7b8f8ca \
+    --hash=sha256:74bc9b6e0e79808bf8678d7678b2ae3736ea72d56eede3820bd3849823e7f305 \
+    --hash=sha256:76ec771e2342f1b558c36d49900dfe81d140361dd0d2df6cd71b3db1be155409 \
+    --hash=sha256:7d23370d2a6b7a71dc65d1266f9a34e4cde9e8e21511322415db4b26f46f6b8c \
+    --hash=sha256:87df44954c31d86df96c8bd6e80dfcd773473e877ac6176a8e29898bfb3501cb \
+    --hash=sha256:8c5979d0deb27e0f4479bee18ea0f83732a893e81b78e62e2dda3e7e518c92ee \
+    --hash=sha256:95d8d31a7713510685b05fbb18d6ac287a56c8f6554d88c19e73f724a445448a \
+    --hash=sha256:a22435632710a4fcf8acf86cbd0d69f68ac389a3892cb23fbad176d1cddaf228 \
+    --hash=sha256:a8763e72d5d9574d45ce5881962bc8e9046bf7b375b0abf031f3e6811732a897 \
+    --hash=sha256:c1eb485cea53f4f5284e5baf92902cd0088b24984f4209e25981cc359d64448d \
+    --hash=sha256:c5d2cc54175bab47011b09688b418db71403aefad07cbcd62d44010543fc143f \
+    --hash=sha256:cbc07246253b9e3d7d74c9ff948cd0fd7a71afcc2b77c7f0a59c26e9395cb152 \
+    --hash=sha256:d0b6c62206e04061e27009481cb0ec966f7d6172b5b936f3ead3d74f29fe3dcf \
+    --hash=sha256:ddae0f39ca146972ff6bb4399f3b2943884a774b8771ea0a8f50e971f5ea5ba8 \
+    --hash=sha256:e1f4d16e296f5135624b34e8fb741eb0eadedca90862405b1f1fde2040b9bd11 \
+    --hash=sha256:e86c2c6852f62f8f2b24cb7a613ebe8e0c7dc1402c61d36a609174f63e0ff017 \
+    --hash=sha256:ebc95f8386314272bbc817026f8ce8f4f0d2ef7ae44f947c4664efac9adec929 \
+    --hash=sha256:f9dca1e257d4cc129517779226753dbefb4f2266c4eaad610fc15c6a7e14283e \
+    --hash=sha256:faff86aa10c1aa4a10e1a301de160f3d8fc8703b88c7e98de46b531ff1276a9a
     # via inverter-connect (pyproject.toml)
 mypy-extensions==1.0.0 \
     --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
     --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
     # via
     #   black
     #   mypy
@@ -559,17 +561,17 @@
     --hash=sha256:50943f151d87e752abddec8158622c34ad7f292e193836e90e30d87da60b19d9 \
     --hash=sha256:61d46bd2eb8016ed4a924e196e6e5b0a268cd3babd79e593048720db23522bb1
     # via inverter-connect (pyproject.toml)
 pkginfo==1.9.6 \
     --hash=sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546 \
     --hash=sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046
     # via twine
-platformdirs==3.5.0 \
-    --hash=sha256:47692bc24c1958e8b0f13dd727307cff1db103fca36399f457da8e05f222fdc4 \
-    --hash=sha256:7954a68d0ba23558d753f73437c55f89027cf8f5108c19844d4b82e5af396335
+platformdirs==3.5.1 \
+    --hash=sha256:412dae91f52a6f84830f39a8078cecd0e866cb72294a5c66808e74d5e88d251f \
+    --hash=sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5
     # via
     #   black
     #   tox
     #   virtualenv
 pluggy==1.0.0 \
     --hash=sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159 \
     --hash=sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3
@@ -695,17 +697,17 @@
 rich-click==1.6.1 \
     --hash=sha256:0fcf4d1a09029d79322dd814ab0b2e66ac183633037561881d45abae8a161d95 \
     --hash=sha256:f8ff96693ec6e261d1544e9f7d9a5811c5ef5d74c8adb4978430fc0dac16777e
     # via
     #   ha-services
     #   inverter-connect (pyproject.toml)
     #   manageprojects
-ruamel-yaml==0.17.24 \
-    --hash=sha256:90e398ee24524ebe20fc48cd1861cedd25520457b9a36cfb548613e57fde30a0 \
-    --hash=sha256:f251bd9096207af604af69d6495c3c650a3338d0493d27b04bc55477d7a884ed
+ruamel-yaml==0.17.26 \
+    --hash=sha256:25d0ee82a0a9a6f44683dcf8c282340def4074a4562f3a24f55695bb254c1693 \
+    --hash=sha256:baa2d0a5aad2034826c439ce61c142c07082b76f4791d54145e131206e998059
     # via safety
 ruamel-yaml-clib==0.2.7 \
     --hash=sha256:045e0626baf1c52e5527bd5db361bc83180faaba2ff586e763d3d5982a876a9e \
     --hash=sha256:15910ef4f3e537eea7fe45f8a5d19997479940d9196f357152a09031c5be59f3 \
     --hash=sha256:184faeaec61dbaa3cace407cffc5819f7b977e75360e8d5ca19461cd851a5fc5 \
     --hash=sha256:1f08fd5a2bea9c4180db71678e850b995d2a5f4537be0e94557668cf0f5f9497 \
     --hash=sha256:2aa261c29a5545adfef9296b7e33941f46aa5bbd21164228e833412af4c9c75f \
```


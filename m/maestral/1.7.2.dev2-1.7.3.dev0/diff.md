# Comparing `tmp/maestral-1.7.2.dev2.tar.gz` & `tmp/maestral-1.7.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maestral-1.7.2.dev2.tar", last modified: Sun Apr 30 12:47:14 2023, max compression
+gzip compressed data, was "maestral-1.7.3.dev0.tar", last modified: Fri May 12 20:30:57 2023, max compression
```

## Comparing `maestral-1.7.2.dev2.tar` & `maestral-1.7.3.dev0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:14.431205 maestral-1.7.2.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-04-30 12:47:14.431205 maestral-1.7.2.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 12:47:14.431205 maestral-1.7.2.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:14.423205 maestral-1.7.2.dev2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:14.427205 maestral-1.7.2.dev2/src/maestral/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/autostart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:14.427205 maestral-1.7.2.dev2/src/maestral/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14787 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/cli/cli_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10518 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/cli/cli_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1925 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/cli/cli_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    15396 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/cli/cli_maintenance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/cli/cli_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/cli/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/cli/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/cli/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/cli/output.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    69523 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:14.431205 maestral-1.7.2.dev2/src/maestral/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/config/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/config/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    21989 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/daemon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:14.431205 maestral-1.7.2.dev2/src/maestral/database/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/database/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    17525 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/database/orm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/database/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/database/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    33650 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/errorhandling.py
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:14.431205 maestral-1.7.2.dev2/src/maestral/fsevents/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/fsevents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/fsevents/polling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    63172 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    29677 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    17790 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/notify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:14.431205 maestral-1.7.2.dev2/src/maestral/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   137001 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/resources/maestral.png
--rw-r--r--   0 runner    (1001) docker     (123)   147935 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:14.431205 maestral-1.7.2.dev2/src/maestral/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/utils/appdirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/utils/caches.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/utils/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/utils/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    18734 2023-04-30 12:46:54.000000 maestral-1.7.2.dev2/src/maestral/utils/path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:47:14.427205 maestral-1.7.2.dev2/src/maestral.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-04-30 12:47:14.000000 maestral-1.7.2.dev2/src/maestral.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-30 12:47:14.000000 maestral-1.7.2.dev2/src/maestral.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:47:14.000000 maestral-1.7.2.dev2/src/maestral.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-30 12:47:14.000000 maestral-1.7.2.dev2/src/maestral.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-30 12:47:14.000000 maestral-1.7.2.dev2/src/maestral.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-30 12:47:14.000000 maestral-1.7.2.dev2/src/maestral.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:30:57.798431 maestral-1.7.3.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-05-12 20:30:57.794431 maestral-1.7.3.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 20:30:57.798431 maestral-1.7.3.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:30:57.790431 maestral-1.7.3.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:30:57.790431 maestral-1.7.3.dev0/src/maestral/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/autostart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:30:57.794431 maestral-1.7.3.dev0/src/maestral/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14787 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/cli/cli_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10518 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/cli/cli_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1925 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/cli/cli_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15396 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/cli/cli_maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/cli/cli_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/cli/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/cli/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/cli/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69578 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:30:57.794431 maestral-1.7.3.dev0/src/maestral/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/config/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/config/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21989 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/daemon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:30:57.794431 maestral-1.7.3.dev0/src/maestral/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/database/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17525 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/database/orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/database/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/database/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33650 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/errorhandling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:30:57.794431 maestral-1.7.3.dev0/src/maestral/fsevents/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/fsevents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/fsevents/polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63172 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29677 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17790 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/notify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:30:57.794431 maestral-1.7.3.dev0/src/maestral/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   137001 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/resources/maestral.png
+-rw-r--r--   0 runner    (1001) docker     (123)   147935 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:30:57.794431 maestral-1.7.3.dev0/src/maestral/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/utils/appdirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/utils/caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/utils/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/utils/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18734 2023-05-12 20:30:40.000000 maestral-1.7.3.dev0/src/maestral/utils/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:30:57.794431 maestral-1.7.3.dev0/src/maestral.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-05-12 20:30:57.000000 maestral-1.7.3.dev0/src/maestral.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-12 20:30:57.000000 maestral-1.7.3.dev0/src/maestral.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:30:57.000000 maestral-1.7.3.dev0/src/maestral.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 20:30:57.000000 maestral-1.7.3.dev0/src/maestral.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-12 20:30:57.000000 maestral-1.7.3.dev0/src/maestral.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 20:30:57.000000 maestral-1.7.3.dev0/src/maestral.egg-info/top_level.txt
```

### Comparing `maestral-1.7.2.dev2/LICENSE.txt` & `maestral-1.7.3.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/PKG-INFO` & `maestral-1.7.3.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestral
-Version: 1.7.2.dev2
+Version: 1.7.3.dev0
 Summary: Open-source Dropbox client for macOS and Linux.
 Author-email: Sam Schott <sam.schott@outlook.com>
 License: MIT
 Project-URL: Homepage, https://maestral.app
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
```

### Comparing `maestral-1.7.2.dev2/README.md` & `maestral-1.7.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/pyproject.toml` & `maestral-1.7.3.dev0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2", "build"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "maestral"
-version = "1.7.2.dev2"
+version = "1.7.3.dev0"
 authors = [{name = "Sam Schott", email = "sam.schott@outlook.com"}]
 license = {text = "MIT"}
 description = "Open-source Dropbox client for macOS and Linux."
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: Unix",
     "Programming Language :: Python",
@@ -45,16 +45,16 @@
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.optional-dependencies]
 gui = [
-    "maestral-qt>=1.7.1;sys_platform=='linux'",
-    "maestral-cocoa>=1.7.1;sys_platform=='darwin'",
+    "maestral-qt>=1.7.3.dev0;sys_platform=='linux'",
+    "maestral-cocoa>=1.7.3.dev0;sys_platform=='darwin'",
 ]
 syslog = ["systemd-python"]
 lint = [
     "black",
     "flake8",
     "flake8-pyproject",
     "mypy",
@@ -67,16 +67,16 @@
     "pytest-benchmark",
     "pytest-cov",
     "pytest-rerunfailures",
 ]
 docs = [
     "sphinx",
     "sphinxext-opengraph",
-    "m2r2",
     "sphinx-autoapi",
+    "sphinx-mdinclude",
     "sphinx_rtd_theme",
 ]
 dev = [
     "bump2version",
     "maestral[lint,test]",
 ]
```

### Comparing `maestral-1.7.2.dev2/src/maestral/autostart.py` & `maestral-1.7.3.dev0/src/maestral/autostart.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,27 +17,28 @@
 import re
 import shutil
 import stat
 import subprocess
 import shlex
 import plistlib
 import configparser
+import sys
 from pathlib import Path
 from enum import Enum
 from typing import Any
 
 try:
     from importlib.metadata import files, PackageNotFoundError
 except ImportError:  # Python 3.7 and lower
     from importlib_metadata import files, PackageNotFoundError
 
 # local imports
 from .utils.appdirs import get_home_dir, get_conf_path, get_data_path
 from .utils.integration import cat
-from .constants import BUNDLE_ID, ENV, IS_LINUX, IS_MACOS
+from .constants import BUNDLE_ID, ENV, IS_LINUX, IS_MACOS, FROZEN
 from .exceptions import MaestralApiError
 
 
 class SupportedImplementations(Enum):
     """Enumeration of supported implementations"""
 
     systemd = "systemd"
@@ -250,44 +251,47 @@
     if IS_LINUX:
         init_command = cat(Path("/proc/1/comm"))
         if init_command is not None and b"systemd" in init_command:
             return SupportedImplementations.systemd
     return None
 
 
-def get_maestral_command_path() -> str:
+def get_command_path(dist: str, command: str) -> str:
     """
-    Returns the path to the maestral executable. May be an empty string if the
-    executable cannot be found.
+    Returns the path to a command line script. Tries to check dist_files first, falls
+    back to :meth:`shutil.which` otherwise.
+
+    :param dist: The distribution which installed the command line script.
+    :param command: The command.
     """
     try:
-        dist_files = files("maestral")
+        dist_files = files(dist)
     except PackageNotFoundError:
         # we may have had installation issues
         dist_files = []
 
     path: os.PathLike[str] | None
 
     if dist_files:
         try:
-            rel_path = next(p for p in dist_files if p.match("**/bin/maestral"))
+            rel_path = next(p for p in dist_files if p.match(f"**/bin/{command}"))
             path = rel_path.locate()
         except StopIteration:
             path = None
     else:
         path = None
 
     if isinstance(path, Path):
         # resolve any symlinks and “..” components
         path = path.resolve()
 
     if path and osp.isfile(path):
         return str(path)
     else:
-        return shutil.which("maestral") or ""
+        return shutil.which(command) or ""
 
 
 class AutoStart:
     """Starts Maestral on user log-in
 
     Creates auto-start files in the appropriate system location to automatically start
     Maestral when the user logs in. Different backends are used depending on the
@@ -295,43 +299,64 @@
 
     :param config_name: Name of Maestral config.
     """
 
     _impl: AutoStartBase
 
     def __init__(self, config_name: str) -> None:
-        self.maestral_path = get_maestral_command_path()
         self.implementation = get_available_implementation()
 
-        start_cmd = f"{self.maestral_path} start -f -c {config_name}"
-        launchd_id = f"{BUNDLE_ID}-daemon.{config_name}"
+        # When using systemd, infer the config name from service name.
+        if self.implementation == SupportedImplementations.systemd:
+            config_name = "%i"
+
+        if FROZEN:
+            start_cmd = [
+                sys.executable,
+                "--cli",
+                "start",
+                "--foreground",
+                "--config-name",
+                config_name,
+            ]
+            stop_cmd = [sys.executable, "--cli", "stop", "--config-name", config_name]
+        else:
+            command_location = get_command_path("maestral", "maestral")
+            start_cmd = [
+                command_location,
+                "start",
+                "--foreground",
+                "--config-name",
+                config_name,
+            ]
+            stop_cmd = [command_location, "stop", "--config-name", config_name]
 
         if self.implementation == SupportedImplementations.launchd:
             self._impl = AutoStartLaunchd(
-                launchd_id,
-                start_cmd,
+                f"{BUNDLE_ID}-daemon.{config_name}",
+                " ".join(start_cmd),
                 EnvironmentVariables=ENV,
                 AssociatedBundleIdentifiers=BUNDLE_ID,
             )
 
         elif self.implementation == SupportedImplementations.systemd:
             notify_failure = (
                 "if [ ${SERVICE_RESULT} != success ]; "
                 "then notify-send Maestral 'Daemon failed: ${SERVICE_RESULT}'; "
                 "fi"
             )
 
             self._impl = AutoStartSystemd(
                 service_name=f"maestral-daemon@{config_name}.service",
-                start_cmd=f"{self.maestral_path} start -f -c %i",
+                start_cmd=" ".join(start_cmd),
                 unit_dict={"Description": "Maestral daemon for the config %i"},
                 service_dict={
                     "Type": "notify",
                     "WatchdogSec": "30",
-                    "ExecStop": f"{self.maestral_path} stop -c %i",
+                    "ExecStop": " ".join(stop_cmd),
                     "ExecStopPost": f'/usr/bin/env bash -c "{notify_failure}"',
                     "Environment": " ".join(f"{k}={v}" for k, v in ENV.items()),
                 },
             )
 
         else:
             self._impl = AutoStartBase()
@@ -353,19 +378,14 @@
         """Toggles autostart on or off."""
         self.enabled = not self.enabled
 
     def enable(self) -> None:
         """Enable autostart."""
         if self.enabled:
             return
-
-        if self.maestral_path:
-            self._impl.enable()
-        else:
-            raise OSError("Could not find path of maestral executable")
+        self._impl.enable()
 
     def disable(self) -> None:
         """Disable autostart."""
         if not self.enabled:
             return
-
         self._impl.disable()
```

### Comparing `maestral-1.7.2.dev2/src/maestral/cli/cli_core.py` & `maestral-1.7.3.dev0/src/maestral/cli/cli_core.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/cli/cli_info.py` & `maestral-1.7.3.dev0/src/maestral/cli/cli_info.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/cli/cli_main.py` & `maestral-1.7.3.dev0/src/maestral/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/cli/cli_maintenance.py` & `maestral-1.7.3.dev0/src/maestral/cli/cli_maintenance.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/cli/cli_settings.py` & `maestral-1.7.3.dev0/src/maestral/cli/cli_settings.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/cli/common.py` & `maestral-1.7.3.dev0/src/maestral/cli/common.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/cli/core.py` & `maestral-1.7.3.dev0/src/maestral/cli/core.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/cli/dialogs.py` & `maestral-1.7.3.dev0/src/maestral/cli/dialogs.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/cli/output.py` & `maestral-1.7.3.dev0/src/maestral/cli/output.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/client.py` & `maestral-1.7.3.dev0/src/maestral/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,18 +415,18 @@
         :param refresh_token: Optionally, instead of an authorization code, directly
             provide a refresh token.
         :param access_token: Optionally, instead of an authorization code or a refresh
             token, directly provide an access token. Note that access tokens are
             short-lived.
         :returns: 0 on success, 1 for an invalid token and 2 for connection errors.
         """
-        if not (code or access_token or refresh_token):
+        if code is None and access_token is None and refresh_token is None:
             raise RuntimeError("No auth code, refresh token or access token provided.")
 
-        if code:
+        if code is not None:
             if not self._auth_flow:
                 raise RuntimeError("Please start auth flow with 'get_auth_url' first")
 
             try:
                 res = self._auth_flow.finish(code)
             except requests.exceptions.HTTPError:
                 return 1
@@ -478,20 +478,20 @@
 
         :param refresh_token: Long-lived refresh-token for the SDK.
         :param access_token: Short-lived access-token for the SDK.
         :raises RuntimeError: if token is not available from storage and no token is
             passed as an argument.
         """
         refresh_token = refresh_token or self._cred_storage.token
-        if not (refresh_token or access_token):
+        if refresh_token is None and access_token is None:
             raise NotLinkedError(
                 "No auth token set", "Please link a Dropbox account first."
             )
 
-        if refresh_token:
+        if refresh_token is not None:
             # Initialise Dropbox SDK.
             self._dbx_base = _DropboxSDK(
                 oauth2_refresh_token=refresh_token,
                 app_key=DROPBOX_APP_KEY,
                 session=self._session,
                 user_agent=USER_AGENT,
                 timeout=self._timeout,
```

### Comparing `maestral-1.7.2.dev2/src/maestral/config/__init__.py` & `maestral-1.7.3.dev0/src/maestral/config/__init__.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/config/main.py` & `maestral-1.7.3.dev0/src/maestral/config/main.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/config/user.py` & `maestral-1.7.3.dev0/src/maestral/config/user.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/constants.py` & `maestral-1.7.3.dev0/src/maestral/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 """
 This module provides constants used throughout the maestral, the GUI and CLI. It should
 be kept free of memory heavy imports.
 """
 
 # system imports
+import sys
+import sys
 import platform
 import pathlib
 from enum import Enum
+from importlib_metadata import metadata
 from typing import ContextManager
 
 try:
     from importlib.resources import as_file, files  # type: ignore
 
     def resource_path(package: str, resource: str) -> ContextManager[pathlib.Path]:
         return as_file(files(package) / resource)
 
 except ImportError:
     from importlib.resources import path as resource_path
 
 
 # app
+FROZEN = "Briefcase-Version" in metadata(__package__) or getattr(sys, "frozen", False)
 APP_NAME = "Maestral"
 BUNDLE_ID = "com.samschott.maestral"
 APP_ICON_PATH = resource_path("maestral.resources", "maestral.png").__enter__()
 ENV = {"PYTHONOPTIMIZE": "2", "LC_CTYPE": "UTF-8"}
 DEFAULT_CONFIG_NAME = "maestral"
 
 # sync
```

### Comparing `maestral-1.7.2.dev2/src/maestral/core.py` & `maestral-1.7.3.dev0/src/maestral/core.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/daemon.py` & `maestral-1.7.3.dev0/src/maestral/daemon.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/database/core.py` & `maestral-1.7.3.dev0/src/maestral/database/core.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/database/orm.py` & `maestral-1.7.3.dev0/src/maestral/database/orm.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/database/query.py` & `maestral-1.7.3.dev0/src/maestral/database/query.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/database/types.py` & `maestral-1.7.3.dev0/src/maestral/database/types.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/errorhandling.py` & `maestral-1.7.3.dev0/src/maestral/errorhandling.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/exceptions.py` & `maestral-1.7.3.dev0/src/maestral/exceptions.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/fsevents/__init__.py` & `maestral-1.7.3.dev0/src/maestral/fsevents/__init__.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/fsevents/polling.py` & `maestral-1.7.3.dev0/src/maestral/fsevents/polling.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/keyring.py` & `maestral-1.7.3.dev0/src/maestral/keyring.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/logging.py` & `maestral-1.7.3.dev0/src/maestral/logging.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/main.py` & `maestral-1.7.3.dev0/src/maestral/main.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/manager.py` & `maestral-1.7.3.dev0/src/maestral/manager.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/models.py` & `maestral-1.7.3.dev0/src/maestral/models.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/notify.py` & `maestral-1.7.3.dev0/src/maestral/notify.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/resources/maestral.png` & `maestral-1.7.3.dev0/src/maestral/resources/maestral.png`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/sync.py` & `maestral-1.7.3.dev0/src/maestral/sync.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/utils/__init__.py` & `maestral-1.7.3.dev0/src/maestral/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/utils/appdirs.py` & `maestral-1.7.3.dev0/src/maestral/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/utils/caches.py` & `maestral-1.7.3.dev0/src/maestral/utils/caches.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/utils/hashing.py` & `maestral-1.7.3.dev0/src/maestral/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/utils/integration.py` & `maestral-1.7.3.dev0/src/maestral/utils/integration.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral/utils/path.py` & `maestral-1.7.3.dev0/src/maestral/utils/path.py`

 * *Files identical despite different names*

### Comparing `maestral-1.7.2.dev2/src/maestral.egg-info/PKG-INFO` & `maestral-1.7.3.dev0/src/maestral.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestral
-Version: 1.7.2.dev2
+Version: 1.7.3.dev0
 Summary: Open-source Dropbox client for macOS and Linux.
 Author-email: Sam Schott <sam.schott@outlook.com>
 License: MIT
 Project-URL: Homepage, https://maestral.app
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
```

### Comparing `maestral-1.7.2.dev2/src/maestral.egg-info/SOURCES.txt` & `maestral-1.7.3.dev0/src/maestral.egg-info/SOURCES.txt`

 * *Files identical despite different names*


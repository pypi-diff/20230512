# Comparing `tmp/sugar_shell-0.2.4.tar.gz` & `tmp/sugar_shell-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sugar_shell-0.2.4.tar", last modified: Fri Apr 14 06:36:53 2023, max compression
+gzip compressed data, was "sugar_shell-0.2.5.tar", last modified: Fri May 12 09:14:30 2023, max compression
```

## Comparing `sugar_shell-0.2.4.tar` & `sugar_shell-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:36:53.392594 sugar_shell-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 06:36:50.000000 sugar_shell-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-14 06:36:53.392594 sugar_shell-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-14 06:36:50.000000 sugar_shell-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 06:36:53.392594 sugar_shell-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-14 06:36:50.000000 sugar_shell-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:36:53.388594 sugar_shell-0.2.4/sugar_shell/
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-14 06:36:50.000000 sugar_shell-0.2.4/sugar_shell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:36:53.392594 sugar_shell-0.2.4/sugar_shell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-14 06:36:53.000000 sugar_shell-0.2.4/sugar_shell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-14 06:36:53.000000 sugar_shell-0.2.4/sugar_shell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 06:36:53.000000 sugar_shell-0.2.4/sugar_shell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 06:36:53.000000 sugar_shell-0.2.4/sugar_shell.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 06:36:53.000000 sugar_shell-0.2.4/sugar_shell.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:14:30.811361 sugar_shell-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-12 09:14:26.000000 sugar_shell-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-12 09:14:30.807361 sugar_shell-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-12 09:14:26.000000 sugar_shell-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 09:14:30.811361 sugar_shell-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-12 09:14:26.000000 sugar_shell-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:14:30.807361 sugar_shell-0.2.5/sugar_shell/
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-05-12 09:14:26.000000 sugar_shell-0.2.5/sugar_shell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:14:30.807361 sugar_shell-0.2.5/sugar_shell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-12 09:14:30.000000 sugar_shell-0.2.5/sugar_shell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-12 09:14:30.000000 sugar_shell-0.2.5/sugar_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 09:14:30.000000 sugar_shell-0.2.5/sugar_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 09:14:30.000000 sugar_shell-0.2.5/sugar_shell.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-12 09:14:30.000000 sugar_shell-0.2.5/sugar_shell.egg-info/top_level.txt
```

### Comparing `sugar_shell-0.2.4/LICENSE` & `sugar_shell-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sugar_shell-0.2.4/README.md` & `sugar_shell-0.2.5/README.md`

 * *Files identical despite different names*


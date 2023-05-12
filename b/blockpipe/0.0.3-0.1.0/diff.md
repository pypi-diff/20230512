# Comparing `tmp/blockpipe-0.0.3.tar.gz` & `tmp/blockpipe-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockpipe-0.0.3.tar", last modified: Fri Jul 22 10:38:41 2022, max compression
+gzip compressed data, was "blockpipe-0.1.0.tar", max compression
```

## Comparing `blockpipe-0.0.3.tar` & `blockpipe-0.1.0.tar`

### file list

```diff
@@ -1,33 +1,5 @@
-drwxr-xr-x   0 wormtail   (502) staff       (20)        0 2022-07-22 10:38:41.072801 blockpipe-0.0.3/
--rw-r--r--   0 wormtail   (502) staff       (20)      337 2022-07-22 10:38:41.072431 blockpipe-0.0.3/PKG-INFO
--rw-r--r--   0 wormtail   (502) staff       (20)       12 2022-07-19 09:39:30.000000 blockpipe-0.0.3/README.md
-drwxr-xr-x   0 wormtail   (502) staff       (20)        0 2022-07-22 10:38:41.061895 blockpipe-0.0.3/blockpipe/
-drwxr-xr-x   0 wormtail   (502) staff       (20)        0 2022-07-22 10:38:41.064556 blockpipe-0.0.3/blockpipe/db/
--rw-r--r--   0 wormtail   (502) staff       (20)        0 2022-07-21 06:49:50.000000 blockpipe-0.0.3/blockpipe/db/__init__.py
-drwxr-xr-x   0 wormtail   (502) staff       (20)        0 2022-07-22 10:38:41.065289 blockpipe-0.0.3/blockpipe/faucet/
--rw-r--r--   0 wormtail   (502) staff       (20)        0 2022-07-21 06:45:56.000000 blockpipe-0.0.3/blockpipe/faucet/__init__.py
--rw-r--r--   0 wormtail   (502) staff       (20)       23 2022-07-22 08:28:44.000000 blockpipe-0.0.3/blockpipe/faucet/faucet.py
--rw-r--r--   0 wormtail   (502) staff       (20)        0 2022-07-21 06:45:52.000000 blockpipe-0.0.3/blockpipe/faucet/path.py
-drwxr-xr-x   0 wormtail   (502) staff       (20)        0 2022-07-22 10:38:41.065567 blockpipe-0.0.3/blockpipe/handler/
--rw-r--r--   0 wormtail   (502) staff       (20)        0 2022-07-21 06:49:55.000000 blockpipe-0.0.3/blockpipe/handler/__init__.py
-drwxr-xr-x   0 wormtail   (502) staff       (20)        0 2022-07-22 10:38:41.066603 blockpipe-0.0.3/blockpipe/script/
--rw-r--r--   0 wormtail   (502) staff       (20)       50 2022-07-22 09:02:15.000000 blockpipe-0.0.3/blockpipe/script/__init__.py
--rw-r--r--   0 wormtail   (502) staff       (20)     1663 2022-07-22 10:38:28.000000 blockpipe-0.0.3/blockpipe/script/app.py
-drwxr-xr-x   0 wormtail   (502) staff       (20)        0 2022-07-22 10:38:41.071695 blockpipe-0.0.3/blockpipe/types/
--rw-r--r--   0 wormtail   (502) staff       (20)      440 2022-07-21 06:38:16.000000 blockpipe-0.0.3/blockpipe/types/__init__.py
--rw-r--r--   0 wormtail   (502) staff       (20)     2488 2022-07-22 09:19:10.000000 blockpipe-0.0.3/blockpipe/types/abi.py
--rw-r--r--   0 wormtail   (502) staff       (20)        0 2022-07-21 06:38:35.000000 blockpipe-0.0.3/blockpipe/types/abi_test.py
--rw-r--r--   0 wormtail   (502) staff       (20)      212 2022-07-19 10:14:31.000000 blockpipe-0.0.3/blockpipe/types/alias.py
--rw-r--r--   0 wormtail   (502) staff       (20)      202 2022-07-19 10:14:27.000000 blockpipe-0.0.3/blockpipe/types/alias_test.py
--rw-r--r--   0 wormtail   (502) staff       (20)     2941 2022-07-22 09:23:12.000000 blockpipe-0.0.3/blockpipe/types/log.py
--rw-r--r--   0 wormtail   (502) staff       (20)     2471 2022-07-22 04:21:48.000000 blockpipe-0.0.3/blockpipe/types/types.py
--rw-r--r--   0 wormtail   (502) staff       (20)      334 2022-07-21 06:28:17.000000 blockpipe-0.0.3/blockpipe/types/types_test.py
-drwxr-xr-x   0 wormtail   (502) staff       (20)        0 2022-07-22 10:38:41.064099 blockpipe-0.0.3/blockpipe.egg-info/
--rw-r--r--   0 wormtail   (502) staff       (20)      337 2022-07-22 10:38:41.000000 blockpipe-0.0.3/blockpipe.egg-info/PKG-INFO
--rw-r--r--   0 wormtail   (502) staff       (20)      598 2022-07-22 10:38:41.000000 blockpipe-0.0.3/blockpipe.egg-info/SOURCES.txt
--rw-r--r--   0 wormtail   (502) staff       (20)        1 2022-07-22 10:38:41.000000 blockpipe-0.0.3/blockpipe.egg-info/dependency_links.txt
--rw-r--r--   0 wormtail   (502) staff       (20)       71 2022-07-22 10:38:41.000000 blockpipe-0.0.3/blockpipe.egg-info/requires.txt
--rw-r--r--   0 wormtail   (502) staff       (20)       10 2022-07-22 10:38:41.000000 blockpipe-0.0.3/blockpipe.egg-info/top_level.txt
--rw-r--r--   0 wormtail   (502) staff       (20)      593 2022-07-22 10:38:32.000000 blockpipe-0.0.3/pyproject.toml
--rw-r--r--   0 wormtail   (502) staff       (20)       38 2022-07-22 10:38:41.072907 blockpipe-0.0.3/setup.cfg
--rw-r--r--   0 wormtail   (502) staff       (20)       38 2022-07-22 10:13:34.000000 blockpipe-0.0.3/setup.py
+-rw-r--r--   0        0        0    10935 2023-05-12 16:42:57.356759 blockpipe-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1746 2023-05-12 16:42:30.627520 blockpipe-0.1.0/README.md
+-rw-r--r--   0        0        0      756 2023-05-12 16:37:47.361664 blockpipe-0.1.0/blockpipe/__init__.py
+-rw-r--r--   0        0        0      331 2023-05-12 16:43:16.489708 blockpipe-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2081 1970-01-01 00:00:00.000000 blockpipe-0.1.0/PKG-INFO
```


# Comparing `tmp/gen3_util-0.0.1.tar.gz` & `tmp/gen3_util-0.0.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3_util-0.0.1.tar", last modified: Thu May  4 23:14:14 2023, max compression
+gzip compressed data, was "gen3_util-0.0.2rc1.tar", last modified: Fri May 12 13:39:40 2023, max compression
```

## Comparing `gen3_util-0.0.1.tar` & `gen3_util-0.0.2rc1.tar`

### file list

```diff
@@ -1,55 +1,71 @@
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-04 23:14:14.715089 gen3_util-0.0.1/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_util-0.0.1/LICENSE
--rw-r--r--   0 walsbr   (320923486) 1971611142     1802 2023-05-04 23:14:14.714860 gen3_util-0.0.1/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     1120 2023-05-04 22:44:42.000000 gen3_util-0.0.1/README.md
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-04 23:14:14.696750 gen3_util-0.0.1/gen3_util/
--rw-r--r--   0 walsbr   (320923486) 1971611142       71 2023-05-04 21:27:52.000000 gen3_util-0.0.1/gen3_util/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-04 23:14:14.703979 gen3_util-0.0.1/gen3_util/cli/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-04 22:01:58.000000 gen3_util-0.0.1/gen3_util/cli/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1250 2023-05-04 22:50:51.000000 gen3_util-0.0.1/gen3_util/cli/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2041 2023-05-04 21:46:37.000000 gen3_util-0.0.1/gen3_util/cli/common.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-04 23:14:14.705026 gen3_util-0.0.1/gen3_util/config/
--rw-r--r--   0 walsbr   (320923486) 1971611142      603 2023-05-04 21:27:22.000000 gen3_util-0.0.1/gen3_util/config/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      495 2023-05-04 22:39:30.000000 gen3_util-0.0.1/gen3_util/config/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      502 2023-05-04 21:30:42.000000 gen3_util-0.0.1/gen3_util/config/config.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-04 23:14:14.707014 gen3_util-0.0.1/gen3_util/files/
--rw-r--r--   0 walsbr   (320923486) 1971611142      197 2023-05-04 15:14:41.000000 gen3_util-0.0.1/gen3_util/files/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      755 2023-05-04 22:02:35.000000 gen3_util-0.0.1/gen3_util/files/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      211 2023-05-04 21:19:30.000000 gen3_util-0.0.1/gen3_util/files/downloader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      190 2023-05-04 21:17:36.000000 gen3_util-0.0.1/gen3_util/files/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      200 2023-05-04 21:17:40.000000 gen3_util-0.0.1/gen3_util/files/remover.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      207 2023-05-04 21:17:43.000000 gen3_util-0.0.1/gen3_util/files/uploader.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-04 23:14:14.709296 gen3_util-0.0.1/gen3_util/meta/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-04 14:46:33.000000 gen3_util-0.0.1/gen3_util/meta/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      947 2023-05-04 22:02:45.000000 gen3_util-0.0.1/gen3_util/meta/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      210 2023-05-04 21:24:52.000000 gen3_util-0.0.1/gen3_util/meta/downloader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      189 2023-05-04 21:23:29.000000 gen3_util-0.0.1/gen3_util/meta/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      199 2023-05-04 21:23:39.000000 gen3_util-0.0.1/gen3_util/meta/remover.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      206 2023-05-04 21:23:47.000000 gen3_util-0.0.1/gen3_util/meta/uploader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      199 2023-05-04 21:18:49.000000 gen3_util-0.0.1/gen3_util/meta/validator.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-04 23:14:14.711771 gen3_util-0.0.1/gen3_util/projects/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-04 14:47:16.000000 gen3_util-0.0.1/gen3_util/projects/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      764 2023-05-04 22:02:53.000000 gen3_util-0.0.1/gen3_util/projects/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      202 2023-05-04 21:16:26.000000 gen3_util-0.0.1/gen3_util/projects/creator.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      196 2023-05-04 21:16:36.000000 gen3_util-0.0.1/gen3_util/projects/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      205 2023-05-04 21:25:19.000000 gen3_util-0.0.1/gen3_util/projects/remover.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      533 2023-05-04 22:39:34.000000 gen3_util-0.0.1/gen3_util/util.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-04 23:14:14.703055 gen3_util-0.0.1/gen3_util.egg-info/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1802 2023-05-04 23:14:14.000000 gen3_util-0.0.1/gen3_util.egg-info/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     1102 2023-05-04 23:14:14.000000 gen3_util-0.0.1/gen3_util.egg-info/SOURCES.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142        1 2023-05-04 23:14:14.000000 gen3_util-0.0.1/gen3_util.egg-info/dependency_links.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       53 2023-05-04 23:14:14.000000 gen3_util-0.0.1/gen3_util.egg-info/entry_points.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142      118 2023-05-04 23:14:14.000000 gen3_util-0.0.1/gen3_util.egg-info/requires.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       16 2023-05-04 23:14:14.000000 gen3_util-0.0.1/gen3_util.egg-info/top_level.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       38 2023-05-04 23:14:14.715152 gen3_util-0.0.1/setup.cfg
--rw-r--r--   0 walsbr   (320923486) 1971611142     5576 2023-05-04 23:14:01.000000 gen3_util-0.0.1/setup.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-04 23:14:14.687625 gen3_util-0.0.1/tests/
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-04 23:14:14.712522 gen3_util-0.0.1/tests/integration/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-04 14:34:18.000000 gen3_util-0.0.1/tests/integration/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      108 2023-05-04 14:34:18.000000 gen3_util-0.0.1/tests/integration/conftest.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-04 23:14:14.714436 gen3_util-0.0.1/tests/unit/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-04 14:34:18.000000 gen3_util-0.0.1/tests/unit/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      322 2023-05-04 15:50:19.000000 gen3_util-0.0.1/tests/unit/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2912 2023-05-04 22:40:24.000000 gen3_util-0.0.1/tests/unit/test_cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-04 14:34:18.000000 gen3_util-0.0.1/tests/unit/test_coding_conventions.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      551 2023-05-04 22:39:13.000000 gen3_util-0.0.1/tests/unit/test_config.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.906822 gen3_util-0.0.2rc1/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_util-0.0.2rc1/LICENSE
+-rw-r--r--   0 walsbr   (320923486) 1971611142     8996 2023-05-12 13:39:40.906468 gen3_util-0.0.2rc1/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     8311 2023-05-12 13:39:21.000000 gen3_util-0.0.2rc1/README.md
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.860794 gen3_util-0.0.2rc1/gen3_util/
+-rw-r--r--   0 walsbr   (320923486) 1971611142       71 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc1/gen3_util/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.868334 gen3_util-0.0.2rc1/gen3_util/access/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1819 2023-05-12 00:08:03.000000 gen3_util-0.0.2rc1/gen3_util/access/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1948 2023-05-12 00:08:03.000000 gen3_util-0.0.2rc1/gen3_util/access/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1869 2023-05-11 17:49:58.000000 gen3_util-0.0.2rc1/gen3_util/access/requestor.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.875286 gen3_util-0.0.2rc1/gen3_util/buckets/
+-rw-r--r--   0 walsbr   (320923486) 1971611142      803 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/buckets/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      628 2023-05-12 12:59:15.000000 gen3_util-0.0.2rc1/gen3_util/buckets/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      474 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/buckets/lister.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.878738 gen3_util-0.0.2rc1/gen3_util/cli/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3932 2023-05-11 00:12:51.000000 gen3_util-0.0.2rc1/gen3_util/cli/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1667 2023-05-10 23:46:59.000000 gen3_util-0.0.2rc1/gen3_util/cli/cli.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.880004 gen3_util-0.0.2rc1/gen3_util/common/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4102 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/common/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.885279 gen3_util-0.0.2rc1/gen3_util/config/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2425 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/config/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      485 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/config/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      503 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/config/config.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.889141 gen3_util-0.0.2rc1/gen3_util/files/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1270 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/files/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2246 2023-05-12 13:00:59.000000 gen3_util-0.0.2rc1/gen3_util/files/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      920 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/files/downloader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      192 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/files/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      202 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/files/remover.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    13289 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/files/uploader.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.900799 gen3_util-0.0.2rc1/gen3_util/meta/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4117 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/meta/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1291 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/meta/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      210 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc1/gen3_util/meta/downloader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5483 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/meta/importer.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      191 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/meta/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      201 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/meta/remover.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      208 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/meta/uploader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3248 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/meta/validator.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.902047 gen3_util-0.0.2rc1/gen3_util/projects/
+-rw-r--r--   0 walsbr   (320923486) 1971611142      329 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/projects/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1152 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/projects/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      204 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/projects/creator.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      553 2023-05-12 13:11:53.000000 gen3_util-0.0.2rc1/gen3_util/projects/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      207 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/gen3_util/projects/remover.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.866330 gen3_util-0.0.2rc1/gen3_util.egg-info/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     8996 2023-05-12 13:39:40.000000 gen3_util-0.0.2rc1/gen3_util.egg-info/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1502 2023-05-12 13:39:40.000000 gen3_util-0.0.2rc1/gen3_util.egg-info/SOURCES.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142        1 2023-05-12 13:39:40.000000 gen3_util-0.0.2rc1/gen3_util.egg-info/dependency_links.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       53 2023-05-12 13:39:40.000000 gen3_util-0.0.2rc1/gen3_util.egg-info/entry_points.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142      128 2023-05-12 13:39:40.000000 gen3_util-0.0.2rc1/gen3_util.egg-info/requires.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       16 2023-05-12 13:39:40.000000 gen3_util-0.0.2rc1/gen3_util.egg-info/top_level.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       38 2023-05-12 13:39:40.906894 gen3_util-0.0.2rc1/setup.cfg
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5580 2023-05-12 13:37:11.000000 gen3_util-0.0.2rc1/setup.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.857640 gen3_util-0.0.2rc1/tests/
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.903804 gen3_util-0.0.2rc1/tests/integration/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc1/tests/integration/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      108 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc1/tests/integration/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2941 2023-05-12 13:32:44.000000 gen3_util-0.0.2rc1/tests/integration/test_access.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      433 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/tests/integration/test_buckets.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2047 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/tests/integration/test_files.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1225 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/tests/integration/test_project.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-05-12 13:39:40.906114 gen3_util-0.0.2rc1/tests/unit/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc1/tests/unit/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      322 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc1/tests/unit/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3222 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/tests/unit/test_cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc1/tests/unit/test_coding_conventions.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      551 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc1/tests/unit/test_config.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1760 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/tests/unit/test_files.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      867 2023-05-11 22:42:33.000000 gen3_util-0.0.2rc1/tests/unit/test_meta.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1546 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc1/tests/unit/test_validate_directory.py
```

### Comparing `gen3_util-0.0.1/LICENSE` & `gen3_util-0.0.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.1/gen3_util/cli/cli.py` & `gen3_util-0.0.2rc1/gen3_util/cli/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,59 @@
 import logging
+import pathlib
 
 import click
+import pkg_resources  # part of setuptools
 
 import gen3_util
-from gen3_util.util import print_formatted
-from gen3_util.cli.common import StdNaturalOrderGroup
+from gen3_util.access.cli import access_group
+from gen3_util.cli import StdNaturalOrderGroup
+from gen3_util.config.cli import config_group
 from gen3_util.files.cli import file_group
 from gen3_util.meta.cli import meta_group
 from gen3_util.projects.cli import project_group
-from gen3_util.config.cli import config_group
-
-import pkg_resources  # part of setuptools
+from gen3_util.buckets.cli import bucket_group
+from gen3_util.common import print_formatted
 
 
 @click.group(cls=StdNaturalOrderGroup, invoke_without_command=True)
 @click.pass_context
-def cli(ctx, config, output_format):
+def cli(ctx, config, output_format, cred, state_dir):
     """Gen3 Management Utilities"""
 
     config__ = gen3_util.default_config
+    logging.basicConfig(format=config__.log.format, level=config__.log.level)
 
     if config:
         config__ = gen3_util.config.custom(config)
 
     if output_format:
         config__.output.format = output_format
 
-    # print(("cli group stdout", config, config_))
-    logging.basicConfig(format=config__.log.format, level=config__.log.level)
+    if cred:
+        config__.gen3.refresh_file = pathlib.Path(cred).expanduser()
 
-    # ensure that ctx.obj exists and is a dict
+    if state_dir:
+        _ = pathlib.Path(state_dir).expanduser()
+        _.mkdir(parents=True, exist_ok=True)
+        config__.state_dir = _
+
+    # ensure that ctx.obj exists
     ctx.obj = config__
     logging.getLogger(__name__).debug(("config", ctx.obj))
 
-    version = pkg_resources.require("gen3_util")[0].version
-
-    print_formatted(config__, {'msg': f'Version {version}'})
+    # called with no arguments
+    if ctx.invoked_subcommand is None:
+        version = pkg_resources.require("gen3_util")[0].version
+        print_formatted(config__, {'msg': f'Version {version}'})
 
 
 cli.add_command(project_group)
+cli.add_command(bucket_group)
 cli.add_command(meta_group)
 cli.add_command(file_group)
+cli.add_command(access_group)
 cli.add_command(config_group)
 
 
 if __name__ == '__main__':
     cli()
```

### Comparing `gen3_util-0.0.1/gen3_util/meta/cli.py` & `gen3_util-0.0.2rc1/gen3_util/meta/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import click
 
-from gen3_util.cli.common import NaturalOrderGroup
+from gen3_util.cli import NaturalOrderGroup, CLIOutput
 from gen3_util.config import Config
 from gen3_util.meta.lister import ls
 from gen3_util.meta.remover import rm
 from gen3_util.meta.uploader import cp
 from gen3_util.meta.validator import validate
 
+from gen3_util.meta.importer import cli as importer_cli
+
 
 @click.group(name='meta', cls=NaturalOrderGroup)
 @click.pass_obj
 def meta_group(config):
     """Manage meta data."""
     pass
 
@@ -18,26 +20,38 @@
 @meta_group.command(name="ls")
 @click.pass_obj
 def meta_ls(config: Config):
     """List meta in a project."""
     ls(config)
 
 
-@meta_group.command(name="validate")
-@click.pass_obj
-def meta_validate(config: Config):
-    """Copy meta to/from the project bucket."""
-    validate(config)
-
-
 @meta_group.command(name="cp")
 @click.pass_obj
 def meta_cp(config: Config):
     """Copy meta to/from the project bucket."""
     cp(config)
 
 
 @meta_group.command(name="rm")
 @click.pass_obj
 def meta_rm(config: Config):
     """Remove meta from a project."""
     rm(config)
+
+
+@meta_group.group(name="import")
+@click.pass_obj
+def meta_import(config: Config):
+    """Import study from directory listing."""
+    pass
+
+
+meta_import.add_command(importer_cli)
+
+
+@meta_group.command(name="validate")
+@click.argument('directory')
+@click.pass_obj
+def meta_validate(config: Config, directory):
+    """Validate FHIR data in DIRECTORY."""
+    with CLIOutput(config) as output:
+        output.update(validate(config, directory))
```

### Comparing `gen3_util-0.0.1/setup.py` & `gen3_util-0.0.2rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name='gen3_util',  # Required
 
     # Versions should comply with PEP 440:
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.1',  # Required
+    version='0.0.2-rc1',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Commons utilities',
     # Optional
```

### Comparing `gen3_util-0.0.1/tests/unit/test_cli.py` & `gen3_util-0.0.2rc1/tests/unit/test_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 from click.testing import CliRunner
 from gen3_util.cli.cli import cli
 
 
 def test_default_command(caplog):
-    """Ensure it prints version"""
+    """Ensure it prints version if no other command"""
     runner = CliRunner()
-    result = runner.invoke(cli)  # , ['--config', 'tests/fixtures/custom_config/config.yaml'])
+    result = runner.invoke(cli)
     assert result.exit_code == 0
-    expected_strings = ['Version']
-    for expected_string in expected_strings:
-        assert expected_string in result.output, f"Should have printed {expected_string}"
+    expected = ['Version']
+    for _ in expected:
+        assert _ in result.output, f"Should have printed expected={_} actual={result.output}"
+
+
+def test_any_command(caplog):
+    """Ensure it does not print version if command provided"""
+    runner = CliRunner()
+    result = runner.invoke(cli, ['config'])
+    assert result.exit_code == 0
+    un_expected_strings = ['Version']
+    for expected_string in un_expected_strings:
+        assert expected_string not in result.output, "only print version if nothing else to do"
 
 
 def test_help(caplog):
     """Ensure it prints command groups"""
     runner = CliRunner()
     result = runner.invoke(cli, ['--help'])
     assert result.exit_code == 0
```

### Comparing `gen3_util-0.0.1/tests/unit/test_coding_conventions.py` & `gen3_util-0.0.2rc1/tests/unit/test_coding_conventions.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.1/tests/unit/test_config.py` & `gen3_util-0.0.2rc1/tests/unit/test_config.py`

 * *Files identical despite different names*


# Comparing `tmp/shadow-scholar-0.5.0.tar.gz` & `tmp/shadow-scholar-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shadow-scholar-0.5.0.tar", last modified: Fri Mar 24 01:01:32 2023, max compression
+gzip compressed data, was "shadow-scholar-0.6.0.tar", last modified: Thu May 11 23:17:06 2023, max compression
```

## Comparing `shadow-scholar-0.5.0.tar` & `shadow-scholar-0.6.0.tar`

### file list

```diff
@@ -1,79 +1,84 @@
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-03-24 01:01:32.512869 shadow-scholar-0.5.0/
--rw-r--r--   0 lucas      (502) staff       (20)    11357 2023-01-30 22:02:35.000000 shadow-scholar-0.5.0/LICENSE
--rw-r--r--   0 lucas      (502) staff       (20)      100 2023-03-09 19:05:25.000000 shadow-scholar-0.5.0/MANIFEST.in
--rw-r--r--   0 lucas      (502) staff       (20)     5436 2023-03-24 01:01:32.512713 shadow-scholar-0.5.0/PKG-INFO
--rw-r--r--   0 lucas      (502) staff       (20)     4824 2023-03-10 17:37:54.000000 shadow-scholar-0.5.0/README.md
--rw-r--r--   0 lucas      (502) staff       (20)     2028 2023-03-24 01:00:50.000000 shadow-scholar-0.5.0/pyproject.toml
--rw-r--r--   0 lucas      (502) staff       (20)       38 2023-03-24 01:01:32.512915 shadow-scholar-0.5.0/setup.cfg
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-03-24 01:01:32.492459 shadow-scholar-0.5.0/src/
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-03-24 01:01:32.494976 shadow-scholar-0.5.0/src/shadow_scholar/
--rw-r--r--   0 lucas      (502) staff       (20)      516 2023-03-21 21:22:41.000000 shadow-scholar-0.5.0/src/shadow_scholar/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)       59 2023-03-03 22:16:56.000000 shadow-scholar-0.5.0/src/shadow_scholar/__main__.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-03-24 01:01:32.496090 shadow-scholar-0.5.0/src/shadow_scholar/app/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-02-14 02:56:52.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/__init__.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-03-24 01:01:32.497213 shadow-scholar-0.5.0/src/shadow_scholar/app/chat_s2/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-03-02 18:48:43.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/chat_s2/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)    12939 2023-03-24 00:59:46.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/chat_s2/_old.py
--rw-r--r--   0 lucas      (502) staff       (20)     6062 2023-03-24 00:59:46.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/chat_s2/library.py
--rw-r--r--   0 lucas      (502) staff       (20)     5220 2023-03-24 00:59:46.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/chat_s2/llm.py
--rw-r--r--   0 lucas      (502) staff       (20)    15972 2023-03-24 00:59:46.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/chat_s2/main.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-03-24 01:01:32.497377 shadow-scholar-0.5.0/src/shadow_scholar/app/chat_s2/res/
--rw-r--r--   0 lucas      (502) staff       (20)      801 2023-03-24 00:59:46.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/chat_s2/res/style.css
--rw-r--r--   0 lucas      (502) staff       (20)     3858 2023-03-24 00:59:46.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/chat_s2/search.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-03-24 01:01:32.503452 shadow-scholar-0.5.0/src/shadow_scholar/app/galactica/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-02-23 21:23:12.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/galactica/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)     8596 2023-02-23 21:23:12.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/galactica/_old.py
--rw-r--r--   0 lucas      (502) staff       (20)     9251 2023-02-23 21:23:12.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/galactica/constants.py
--rw-r--r--   0 lucas      (502) staff       (20)     8755 2023-03-03 21:48:10.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/galactica/convert_to_int8.py
--rw-r--r--   0 lucas      (502) staff       (20)  1290127 2023-02-23 21:23:12.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/galactica/example.png
--rw-r--r--   0 lucas      (502) staff       (20)    16518 2023-03-24 00:59:46.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/galactica/galai_model.py
--rw-r--r--   0 lucas      (502) staff       (20)     1490 2023-02-23 21:23:12.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/galactica/galai_parallel_policy.py
--rw-r--r--   0 lucas      (502) staff       (20)     5433 2023-02-23 21:23:12.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/galactica/galai_utils.py
--rw-r--r--   0 lucas      (502) staff       (20)     9211 2023-03-24 00:59:46.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/galactica/main.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-03-24 01:01:32.504336 shadow-scholar-0.5.0/src/shadow_scholar/app/hello_world/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-03-03 22:16:55.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/hello_world/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-03-09 19:05:25.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/hello_world/gradio.css
--rw-r--r--   0 lucas      (502) staff       (20)     1673 2023-03-24 00:59:46.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/hello_world/main.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-03-24 01:01:32.505420 shadow-scholar-0.5.0/src/shadow_scholar/app/hello_world/res/
--rw-r--r--   0 lucas      (502) staff       (20)   151710 2023-03-09 19:05:25.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/hello_world/res/logo.png
--rw-r--r--   0 lucas      (502) staff       (20)      252 2023-03-24 00:59:46.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/hello_world/res/style.css
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-03-24 01:01:32.505969 shadow-scholar-0.5.0/src/shadow_scholar/app/llama/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-03-02 18:48:43.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/llama/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)    11621 2023-03-24 00:59:46.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/llama/main.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-03-24 01:01:32.508923 shadow-scholar-0.5.0/src/shadow_scholar/app/pdod/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-02-14 02:56:52.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/pdod/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)     1050 2023-03-24 00:59:46.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/pdod/caches.py
--rw-r--r--   0 lucas      (502) staff       (20)     5099 2023-02-23 21:23:12.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/pdod/datasets.py
--rw-r--r--   0 lucas      (502) staff       (20)     5524 2023-03-10 05:36:31.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/pdod/main.py
--rw-r--r--   0 lucas      (502) staff       (20)     2454 2023-02-23 21:23:12.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/pdod/mmda_utils.py
--rw-r--r--   0 lucas      (502) staff       (20)     7874 2023-02-23 21:23:12.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/pdod/rankers.py
--rw-r--r--   0 lucas      (502) staff       (20)     1342 2023-02-16 07:04:20.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/pdod/reg_utils.py
--rw-r--r--   0 lucas      (502) staff       (20)     2804 2023-03-10 05:35:40.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/pdod/slicers.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-03-24 01:01:32.509608 shadow-scholar-0.5.0/src/shadow_scholar/app/qa/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-02-14 02:56:52.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/qa/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)     7112 2023-03-10 05:35:40.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/qa/data.py
--rw-r--r--   0 lucas      (502) staff       (20)     7014 2023-03-21 21:27:24.000000 shadow-scholar-0.5.0/src/shadow_scholar/app/qa/main.py
--rw-r--r--   0 lucas      (502) staff       (20)    14042 2023-03-10 05:36:31.000000 shadow-scholar-0.5.0/src/shadow_scholar/cli.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-03-24 01:01:32.510000 shadow-scholar-0.5.0/src/shadow_scholar/collections/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-02-14 02:56:52.000000 shadow-scholar-0.5.0/src/shadow_scholar/collections/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)     5238 2023-03-03 22:37:47.000000 shadow-scholar-0.5.0/src/shadow_scholar/collections/athena.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-03-24 01:01:32.512224 shadow-scholar-0.5.0/src/shadow_scholar/collections/queries/
--rw-r--r--   0 lucas      (502) staff       (20)     1177 2023-03-24 00:59:46.000000 shadow-scholar-0.5.0/src/shadow_scholar/collections/queries/acl_anthology.sql
--rw-r--r--   0 lucas      (502) staff       (20)     3419 2023-02-14 02:56:52.000000 shadow-scholar-0.5.0/src/shadow_scholar/collections/queries/s2ag_abstracts.sql
--rw-r--r--   0 lucas      (502) staff       (20)      980 2023-02-14 02:56:52.000000 shadow-scholar-0.5.0/src/shadow_scholar/collections/queries/s2ag_authors.sql
--rw-r--r--   0 lucas      (502) staff       (20)      690 2023-02-14 02:56:52.000000 shadow-scholar-0.5.0/src/shadow_scholar/collections/queries/s2ag_citations.sql
--rw-r--r--   0 lucas      (502) staff       (20)      348 2023-02-14 02:56:52.000000 shadow-scholar-0.5.0/src/shadow_scholar/collections/queries/s2ag_embeddings.sql
--rw-r--r--   0 lucas      (502) staff       (20)      239 2023-02-14 02:56:52.000000 shadow-scholar-0.5.0/src/shadow_scholar/collections/queries/s2ag_paper_ids.sql
--rw-r--r--   0 lucas      (502) staff       (20)     3256 2023-02-14 02:56:52.000000 shadow-scholar-0.5.0/src/shadow_scholar/collections/queries/s2ag_papers.sql
--rw-r--r--   0 lucas      (502) staff       (20)      431 2023-02-14 02:56:52.000000 shadow-scholar-0.5.0/src/shadow_scholar/collections/queries/s2ag_publication_venues.sql
--rw-r--r--   0 lucas      (502) staff       (20)     4581 2023-02-14 02:56:52.000000 shadow-scholar-0.5.0/src/shadow_scholar/collections/queries/s2ag_s2orc.sql
--rw-r--r--   0 lucas      (502) staff       (20)      203 2023-02-14 02:56:52.000000 shadow-scholar-0.5.0/src/shadow_scholar/collections/queries/s2ag_tldrs.sql
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-03-24 01:01:32.495954 shadow-scholar-0.5.0/src/shadow_scholar.egg-info/
--rw-r--r--   0 lucas      (502) staff       (20)     5436 2023-03-24 01:01:32.000000 shadow-scholar-0.5.0/src/shadow_scholar.egg-info/PKG-INFO
--rw-r--r--   0 lucas      (502) staff       (20)     2546 2023-03-24 01:01:32.000000 shadow-scholar-0.5.0/src/shadow_scholar.egg-info/SOURCES.txt
--rw-r--r--   0 lucas      (502) staff       (20)        1 2023-03-24 01:01:32.000000 shadow-scholar-0.5.0/src/shadow_scholar.egg-info/dependency_links.txt
--rw-r--r--   0 lucas      (502) staff       (20)       50 2023-03-24 01:01:32.000000 shadow-scholar-0.5.0/src/shadow_scholar.egg-info/entry_points.txt
--rw-r--r--   0 lucas      (502) staff       (20)      238 2023-03-24 01:01:32.000000 shadow-scholar-0.5.0/src/shadow_scholar.egg-info/requires.txt
--rw-r--r--   0 lucas      (502) staff       (20)       15 2023-03-24 01:01:32.000000 shadow-scholar-0.5.0/src/shadow_scholar.egg-info/top_level.txt
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-03-24 01:01:32.512459 shadow-scholar-0.5.0/tests/
--rw-r--r--   0 lucas      (502) staff       (20)      354 2023-02-14 02:56:52.000000 shadow-scholar-0.5.0/tests/test_imports.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.767712 shadow-scholar-0.6.0/
+-rw-r--r--   0 lucas      (502) staff       (20)    11357 2023-01-30 22:02:35.000000 shadow-scholar-0.6.0/LICENSE
+-rw-r--r--   0 lucas      (502) staff       (20)      106 2023-04-11 19:13:05.000000 shadow-scholar-0.6.0/MANIFEST.in
+-rw-r--r--   0 lucas      (502) staff       (20)     6263 2023-05-11 23:17:06.767545 shadow-scholar-0.6.0/PKG-INFO
+-rw-r--r--   0 lucas      (502) staff       (20)     5651 2023-05-11 23:16:57.000000 shadow-scholar-0.6.0/README.md
+-rw-r--r--   0 lucas      (502) staff       (20)     2028 2023-05-11 23:16:57.000000 shadow-scholar-0.6.0/pyproject.toml
+-rw-r--r--   0 lucas      (502) staff       (20)       38 2023-05-11 23:17:06.767762 shadow-scholar-0.6.0/setup.cfg
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.749837 shadow-scholar-0.6.0/src/
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.752549 shadow-scholar-0.6.0/src/shadow_scholar/
+-rw-r--r--   0 lucas      (502) staff       (20)      604 2023-05-11 23:16:57.000000 shadow-scholar-0.6.0/src/shadow_scholar/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)       59 2023-03-03 22:16:56.000000 shadow-scholar-0.6.0/src/shadow_scholar/__main__.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.753511 shadow-scholar-0.6.0/src/shadow_scholar/app/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/__init__.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.754315 shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-03-02 18:48:43.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     8837 2023-05-11 23:15:29.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/library.py
+-rw-r--r--   0 lucas      (502) staff       (20)     6656 2023-05-11 22:13:47.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/llm.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1995 2023-04-11 19:13:05.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/logging.py
+-rw-r--r--   0 lucas      (502) staff       (20)    19018 2023-05-11 22:13:47.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/main.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.754599 shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/res/
+-rw-r--r--   0 lucas      (502) staff       (20)     4871 2023-03-24 00:59:46.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/res/logo.svg
+-rw-r--r--   0 lucas      (502) staff       (20)      960 2023-04-11 19:13:05.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/res/style.css
+-rw-r--r--   0 lucas      (502) staff       (20)     6153 2023-05-11 22:13:47.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/search.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.757995 shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-02-23 21:23:12.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     8596 2023-02-23 21:23:12.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/_old.py
+-rw-r--r--   0 lucas      (502) staff       (20)     9251 2023-02-23 21:23:12.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/constants.py
+-rw-r--r--   0 lucas      (502) staff       (20)     8755 2023-03-03 21:48:10.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/convert_to_int8.py
+-rw-r--r--   0 lucas      (502) staff       (20)  1290127 2023-02-23 21:23:12.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/example.png
+-rw-r--r--   0 lucas      (502) staff       (20)    16518 2023-04-03 06:48:20.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/galai_model.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1490 2023-02-23 21:23:12.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/galai_parallel_policy.py
+-rw-r--r--   0 lucas      (502) staff       (20)     5433 2023-02-23 21:23:12.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/galai_utils.py
+-rw-r--r--   0 lucas      (502) staff       (20)     9211 2023-03-24 00:59:46.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/main.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.758401 shadow-scholar-0.6.0/src/shadow_scholar/app/hello_world/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-03-03 22:16:55.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/hello_world/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-03-09 19:05:25.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/hello_world/gradio.css
+-rw-r--r--   0 lucas      (502) staff       (20)     1622 2023-05-11 23:16:57.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/hello_world/main.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.759810 shadow-scholar-0.6.0/src/shadow_scholar/app/hello_world/res/
+-rw-r--r--   0 lucas      (502) staff       (20)   151710 2023-03-09 19:05:25.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/hello_world/res/logo.png
+-rw-r--r--   0 lucas      (502) staff       (20)      252 2023-03-24 00:59:46.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/hello_world/res/style.css
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.760510 shadow-scholar-0.6.0/src/shadow_scholar/app/llama/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-03-02 18:48:43.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/llama/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)    11621 2023-03-24 00:59:46.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/llama/main.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.761786 shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-04-17 02:25:19.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1051 2023-05-11 23:16:57.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/caches.py
+-rw-r--r--   0 lucas      (502) staff       (20)     5099 2023-04-17 02:25:19.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/datasets.py
+-rw-r--r--   0 lucas      (502) staff       (20)     5524 2023-04-17 02:25:19.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/main.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2454 2023-04-17 02:25:19.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/mmda_utils.py
+-rw-r--r--   0 lucas      (502) staff       (20)     7874 2023-04-17 02:25:19.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/rankers.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1342 2023-04-17 02:25:19.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/reg_utils.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2804 2023-04-17 02:25:19.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/slicers.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.762188 shadow-scholar-0.6.0/src/shadow_scholar/app/qa/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/qa/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     7112 2023-04-03 06:48:20.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/qa/data.py
+-rw-r--r--   0 lucas      (502) staff       (20)     7014 2023-03-21 21:27:24.000000 shadow-scholar-0.6.0/src/shadow_scholar/app/qa/main.py
+-rw-r--r--   0 lucas      (502) staff       (20)    16138 2023-05-11 23:16:57.000000 shadow-scholar-0.6.0/src/shadow_scholar/cli.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.762458 shadow-scholar-0.6.0/src/shadow_scholar/collections/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/src/shadow_scholar/collections/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     5254 2023-05-11 23:16:57.000000 shadow-scholar-0.6.0/src/shadow_scholar/collections/athena.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.766291 shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/
+-rw-r--r--   0 lucas      (502) staff       (20)     1177 2023-03-24 00:59:46.000000 shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/acl_anthology.sql
+-rw-r--r--   0 lucas      (502) staff       (20)     3419 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_abstracts.sql
+-rw-r--r--   0 lucas      (502) staff       (20)      980 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_authors.sql
+-rw-r--r--   0 lucas      (502) staff       (20)      690 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_citations.sql
+-rw-r--r--   0 lucas      (502) staff       (20)      348 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_embeddings.sql
+-rw-r--r--   0 lucas      (502) staff       (20)      239 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_paper_ids.sql
+-rw-r--r--   0 lucas      (502) staff       (20)     3256 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_papers.sql
+-rw-r--r--   0 lucas      (502) staff       (20)      431 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_publication_venues.sql
+-rw-r--r--   0 lucas      (502) staff       (20)     4581 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_s2orc.sql
+-rw-r--r--   0 lucas      (502) staff       (20)      203 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_tldrs.sql
+-rw-r--r--   0 lucas      (502) staff       (20)      637 2023-05-11 23:16:57.000000 shadow-scholar-0.6.0/src/shadow_scholar/hello_world.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.766929 shadow-scholar-0.6.0/src/shadow_scholar/util/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-05-11 23:16:57.000000 shadow-scholar-0.6.0/src/shadow_scholar/util/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1134 2023-05-11 23:16:57.000000 shadow-scholar-0.6.0/src/shadow_scholar/util/s2_api.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.753371 shadow-scholar-0.6.0/src/shadow_scholar.egg-info/
+-rw-r--r--   0 lucas      (502) staff       (20)     6263 2023-05-11 23:17:06.000000 shadow-scholar-0.6.0/src/shadow_scholar.egg-info/PKG-INFO
+-rw-r--r--   0 lucas      (502) staff       (20)     2697 2023-05-11 23:17:06.000000 shadow-scholar-0.6.0/src/shadow_scholar.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas      (502) staff       (20)        1 2023-05-11 23:17:06.000000 shadow-scholar-0.6.0/src/shadow_scholar.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas      (502) staff       (20)       50 2023-05-11 23:17:06.000000 shadow-scholar-0.6.0/src/shadow_scholar.egg-info/entry_points.txt
+-rw-r--r--   0 lucas      (502) staff       (20)      238 2023-05-11 23:17:06.000000 shadow-scholar-0.6.0/src/shadow_scholar.egg-info/requires.txt
+-rw-r--r--   0 lucas      (502) staff       (20)       15 2023-05-11 23:17:06.000000 shadow-scholar-0.6.0/src/shadow_scholar.egg-info/top_level.txt
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-05-11 23:17:06.767254 shadow-scholar-0.6.0/tests/
+-rw-r--r--   0 lucas      (502) staff       (20)      354 2023-02-14 02:56:52.000000 shadow-scholar-0.6.0/tests/test_imports.py
```

### Comparing `shadow-scholar-0.5.0/LICENSE` & `shadow-scholar-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.5.0/PKG-INFO` & `shadow-scholar-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,19 @@
-Metadata-Version: 2.1
-Name: shadow-scholar
-Version: 0.5.0
-Summary: 🎓🕶️ A collection of utilities and demos from the Semantic Scholar Research Team 🕶️🎓
-Author-email: Luca Soldaini <lucas@allenai.org>
-License: Apache-2.0
-Project-URL: Homepage, https://github.com/allenai/shadow-scholar
-Project-URL: Source, https://github.com/allenai/shadow-scholar
-Project-URL: Tracker, https://github.com/allenai/shadow-scholar/issues
-Classifier: Development Status :: 3 - Alpha
-Classifier: Typing :: Typed
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 <h1 align="center">Shadow Scholar</h1>
 <p align="center">
     <img src="https://raw.githubusercontent.com/allenai/shadow-scholar/main/res/shadow-scholar.png" width="400" height="400" align="center" />
 </p>
 
+**Table of Contents**
+- [Installation](#installation)
+- [Available Scripts](#available-scripts)
+- [Getting Access to AWS services](#getting-access-to-aws-services)
+- [Adding Your Own Script](#adding-your-own-script-application-entry-point)
+- [Adding A New Module](#adding-a-new-module-available-to-all-scriptsas-a-dependency)
+
 ## Installation
 
 To install from PyPI, simply run:
 
 ```bash
 pip install shadow-scholar
 ```
@@ -39,15 +30,15 @@
 
 - [Athena](https://aws.amazon.com/athena/)
 - [S3](https://aws.amazon.com/s3/)
 
 The best way to do so is to obtain AWS credentials (access key and secret key) and set them as environment variables.
 
 
-## Writing your own script
+## Adding Your Own Script (Application Entry Point)
 
 To write your own script for Shadow Scholar, follow these steps:
 
 **Step 1**: Choose where to add your code in Shadow Scholar. It can either be
 in an existing module, such as `shadow_scholar.collections.athena`, or in a
 new module.
 
@@ -200,7 +191,26 @@
 **Step 7**: Import the function in the `__init__.py` file of the module. For
 example, if you added your script to `shadow_scholar/examples.py`, you would
 add the following to `shadow_scholar/__init__.py`:
 
 ```python
 from shadow_scholar.examples import my_script
 ```
+
+
+## Adding A New Module (Available to All Scripts/as a Dependency)
+
+Adding a module to Shadow Scholar is as easy as adding a script, but,
+instead of decorating the main entry-point function with `cli`, you need
+to use the `@require` decorator. For example:
+
+```python
+from shadow_scholar.cli import require, safe_import
+
+with safe_import():
+    import requests
+
+@require(["requests>=2.0.0"])
+def module_function():
+    # Do something with requests
+    requests.get(...)
+```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `shadow-scholar-0.5.0/pyproject.toml` & `shadow-scholar-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "shadow-scholar"
-version = "0.5.0"
+version = "0.6.0"
 description = "🎓🕶️ A collection of utilities and demos from the Semantic Scholar Research Team 🕶️🎓"
 authors = [
     {name = "Luca Soldaini", email = "lucas@allenai.org" }
 ]
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
-    "necessary>=0.4.1",
+    "necessary>=0.4.2",
     "typing_extensions>=4.0.0",
     "platformdirs>=2.4.0",
     "cachetools>=4.2.4"
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Typing :: Typed",
```

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/app/chat_s2/library.py` & `shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/library.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,74 +1,130 @@
-import logging
 import os
 import re
 from dataclasses import dataclass, field
+from logging import Logger
 from time import time
-from typing import Dict, Iterable, List, Optional, Union, cast
+from typing import Dict, Iterable, List, Optional, Union
 
+import edlib
 import requests
 
 API_FIELDS = [
     "title",
     "abstract",
     "venue",
     "fieldsOfStudy",
     "authors",
     "isOpenAccess",
     "year",
     "corpusId",
+    "externalIds",
 ]
 
 S2_API_KEY = os.environ.get("S2_API_KEY", "")
 
 
-LOGGER = logging.getLogger(__name__)
+def clean_html(raw_html: Optional[str] = None) -> str:
+    if not (raw_html := (raw_html or "").strip()):
+        return raw_html
+
+    return re.sub(
+        r"<.*?>|&([a-z0-9]+|#[0-9]{1,6}|#x[0-9a-f]{1,6});", "", raw_html
+    )
+
+
+def get_s2_metadata_single(
+    paper: "Paper",
+    s2_api_key: str = S2_API_KEY,
+    logger: Optional[Logger] = None,
+):
+    url = (
+        "https://api.semanticscholar.org/graph/v1/paper/"
+        f"{paper.id}?fields={','.join(API_FIELDS)}"
+    )
+    header = {"x-api-key": s2_api_key}
+    response = requests.get(url, headers=header)
+    paper.metadata.update(response.json())
 
 
 def get_s2_metadata(
-    papers: Union["Paper", Iterable["Paper"]],
+    papers: Iterable["Paper"],
     s2_api_key: str = S2_API_KEY,
+    logger: Optional[Logger] = None,
 ):
     start = time()
 
     url = (
         "https://api.semanticscholar.org/graph/v1/paper/batch?"
         f"fields={','.join(API_FIELDS)}"
     )
     header = {"x-api-key": s2_api_key}
 
-    papers = [papers] if isinstance(papers, Paper) else papers
-    missing = [p for p in papers if p.missing]
+    papers_with_missing_metadata = [p for p in papers if p.missing]
 
-    if not missing:
+    if not papers_with_missing_metadata:
         # nothing new to fetch metadata for
         return
 
-    data = {"ids": [p.id for p in missing]}
+    data = {"ids": [p.id for p in papers_with_missing_metadata]}
     response = requests.post(url, headers=header, json=data)
     results = response.json()
 
-    delta = time() - start
-    LOGGER.warn(f"S2 Metadata :: {delta:.2f}s :: {len(results)} items.")
+    if (
+        isinstance(results, dict)
+        and results.get("message") == "Internal Server Error"
+    ):
+        for paper in papers_with_missing_metadata:
+            get_s2_metadata_single(paper, s2_api_key, logger)
+        return
 
-    for paper, paper_metadata in zip(missing, results):
-        if paper_metadata:
-            try:
-                paper.metadata.update(cast(dict, paper_metadata))
-            except Exception as e:
-                LOGGER.error(f"Failed to update metadata for {paper.id}: {e}")
-                continue
+    # responses might not in order of request, so we need to match them up;
+    # we do this by calculating similarity
+    for paper in papers_with_missing_metadata:
+        distance: List[int] = []
+        for result in results:
+            if (
+                paper.id == result.get("paperId", None)
+                or paper.id == result.get("corpusId", None)
+                or str(paper.id).split(":", 1)[-1]
+                in result.get("externalIds", {}).values()
+            ):
+                distance.append(0)
+                break
+
+            elif "title" in result and "title" in paper.metadata:
+                distance.append(
+                    edlib.align(paper.metadata["title"], result["title"])[
+                        "editDistance"
+                    ]
+                )
+            else:
+                distance.append(1000)
+
+        if len(distance) > 0 and (best_guess := min(distance)) < 1000:
+            location = distance.index(best_guess)
+            metadata = results.pop(location)
+            paper.metadata.update(metadata)
+
+    delta = time() - start
+    logger.info(
+        {
+            "url": url,
+            "data": data,
+            "elapsed": delta,
+            "response": results,
+            "action": "get_s2_metadata",
+        }
+    ) if logger else None
 
 
 @dataclass
 class Paper:
     id: str
     metadata: dict = field(default_factory=dict)
-    score: float = -1.0
-    short_id: Optional[int] = None
 
     def __str__(self) -> str:
         return f"Paper({self.id})"
 
     @classmethod
     def id_from_s2_url(cls, url: str) -> Union[str, None]:
         is_valid_url = re.match(
@@ -88,19 +144,29 @@
 
         arxiv_id = is_valid_url.group(2)
         return f"arxiv:{arxiv_id}"
 
     @classmethod
     def from_url(cls, url: str, **attrs) -> Optional["Paper"]:
         id_ = cls.id_from_s2_url(url) or cls.id_from_arxiv_url(url)
-        return cls(id_, **attrs) if id_ else None
+        return cls(id_, metadata=attrs) if id_ else None
+
+    @property
+    def short_id(self) -> Optional[int]:
+        if short_id := self.metadata.get("short_id", None):
+            short_id = int(short_id)
+        return short_id
+
+    @property
+    def score(self) -> float:
+        return self.metadata.get("score", -1.0)
 
     @property
     def missing(self) -> bool:
-        return len(self.metadata) == 0
+        return self.metadata.get("corpusId", None) is None
 
     @property
     def authors(self) -> List[str]:
         return [author["name"] for author in self.metadata.get("authors", [])]
 
     @property
     def url(self) -> str:
@@ -110,19 +176,19 @@
     def year(self) -> Union[int, None]:
         if (year := self.metadata.get("year")) is not None:
             year = int(year)
         return year
 
     @property
     def title(self) -> str:
-        return self.metadata.get("title", "")
+        return clean_html(self.metadata.get("title", ""))
 
     @property
     def abstract(self) -> str:
-        return self.metadata.get("abstract", "")
+        return clean_html(self.metadata.get("abstract", ""))
 
     @property
     def is_open_access(self) -> bool:
         return self.metadata.get("isOpenAccess", False)
 
     @property
     def venue(self) -> str:
@@ -133,19 +199,22 @@
         return self.metadata.get("corpusId", "")
 
     def _truncate(self, text: str, cols: int = 70) -> str:
         if len(text) > (cols - 3):
             return text[:cols] + "..."
         return text
 
-    def html_format_paper(self) -> str:
-        title = (
-            f'<p><a href="{self.url}" target="_blank">'
-            f"<b>{self._truncate(self.title)}</b></a> ({self.year})</p>"
+    def html_format_title(self) -> str:
+        return (
+            f'<a href="{self.url}" target="_blank">'
+            f"<b>{self._truncate(self.title)}</b></a> ({self.year})"
         )
+
+    def html_format_paper(self) -> str:
+        title = self.html_format_title()
         authors = f'<p><i>{self._truncate(", ".join(self.authors))}</i></p>'
         abstract = f'<p>{self._truncate(self.abstract or "")}</p>'
         return "\n".join([title, authors, abstract])
 
     def html_format_id(self) -> str:
         short_id = (
             f'<span class="span-major">[{self.short_id}]</span>'
@@ -163,36 +232,52 @@
         return (
             '<div id="id-score-table-container">'
             f"<p>{short_id}</p><p>{title_id}</p>"
             f'<p id="score-para">{score}</p>'
             "</div>"
         )
 
+    def to_json(self):
+        return {
+            "id": self.id,
+            "metadata": self.metadata,
+            "short_id": self.short_id,
+        }
+
+    @classmethod
+    def from_json(cls, data):
+        return cls(**data)
+
 
 @dataclass
 class Stack:
     papers: Dict[str, Paper] = field(default_factory=dict)
     s2_api_key: str = S2_API_KEY
 
+    def _compute_short_ids(self):
+        for i, p in enumerate(self.papers.values(), start=1):
+            if p.short_id is None:
+                p.metadata["short_id"] = i
+
     def append(self, paper: Paper):
         if paper.id not in self.papers:
             self.papers[paper.id] = paper
-            paper.short_id = len(self.papers)
-        elif paper.score > self.papers[paper.id].score:
-            self.papers[paper.id].score = paper.score
+            self._compute_short_ids()
 
     def extend(self, papers: Iterable[Paper]):
         for paper in papers:
             self.append(paper)
 
     def fetch(self):
         get_s2_metadata(self.papers.values(), s2_api_key=self.s2_api_key)
-        for p in list(self.papers.keys()):
-            if self.papers[p].missing:
-                self.papers.pop(p)
+        for pid in list(self.papers):
+            # remove papers that are not found
+            if self.papers[pid].missing:
+                del self.papers[pid]
+        self._compute_short_ids()
 
     @property
     def sorted(self) -> List[Paper]:
         return sorted(self.papers.values(), key=lambda p: -p.score)
 
     def __len__(self):
         return len(self.papers)
@@ -212,9 +297,19 @@
 
     def table(self) -> List[List[str]]:
         if len(self) == 0:
             # we need to return something otherwise UI will break
             return [["", ""]]
 
         return [
-            [p.html_format_id(), p.html_format_paper()] for p in self.sorted
+            [p.html_format_id(), p.html_format_paper()]
+            for p in sorted(
+                self.sorted, key=lambda p: (p.short_id or -p.score)
+            )
         ]
+
+    def to_json(self):
+        return [p.to_json() for p in self.papers.values()]
+
+    @classmethod
+    def from_json(cls, data):
+        return cls(papers={p["id"]: Paper.from_json(p) for p in data})
```

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/app/chat_s2/llm.py` & `shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/llm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import json
-import logging
 import os
 from dataclasses import dataclass, field
 from typing import (
     Any,
     Dict,
     Iterable,
     List,
@@ -13,26 +11,25 @@
     Tuple,
     Union,
 )
 
 import openai
 from jinja2 import Template
 
-from .library import Paper
+from .library import Paper, clean_html
+from .logging import get_logger
 
 OPENAI_API_KEY = os.environ.get("OPENAI_API_KEY", None)
 
-LOGGER = logging.getLogger(__name__)
-
 
 class ChatMessage(NamedTuple):
     role: Literal["user", "system", "assistant"]
     content: Template
 
-    def json(self, content: Optional[dict] = None) -> Dict[str, str]:
+    def to_json(self, content: Optional[dict] = None) -> Dict[str, str]:
         return {
             "role": self.role,
             "content": self.content.render(**(content or {})),
         }
 
 
 class OpenAiPrompt:
@@ -59,53 +56,60 @@
             ChatMessage(role=role, content=Template(content))  # type: ignore
             for role, content in prompt
         ]
 
         self.temperature = temperature
         self.max_tokens = max_tokens
 
-        self._cache: Dict[str, Any] = {}
+        self.logger = get_logger(__name__, disable_cloudwatch="yes")
+
+    def to_json(self) -> Dict[str, Any]:
+        return {
+            "model": self.model,
+            "mode": self.mode,
+            "prompt": [message.to_json() for message in self.prompt],
+            "temperature": self.temperature,
+            "max_tokens": self.max_tokens,
+        }
 
     def completion(self, content: dict, params: Optional[dict] = None) -> str:
         request = {
             "model": self.model,
             "prompt": self.prompt[0].content.render(**content),
             "temperature": self.temperature,
             "max_tokens": self.max_tokens,
             **(params or {}),
         }
         response = openai.Completion.create(**request)
-        LOGGER.warn(
-            json.dumps(
-                {
-                    "request": request,
-                    "response": response,
-                    "endpoint": "Completion",
-                }
-            )
+        self.logger.info(
+            {
+                "request": request,
+                "response": response,
+                "endpoint": "Completion",
+                "action": "completion_openai_llm",
+            }
         )
         return response.choices[0].text  # pyright: ignore
 
     def chat(self, content: dict, params: Optional[dict] = None) -> str:
         request = {
             "model": self.model,
-            "messages": [message.json(content) for message in self.prompt],
+            "messages": [message.to_json(content) for message in self.prompt],
             "temperature": self.temperature,
             "max_tokens": self.max_tokens,
             **(params or {}),
         }
         response = openai.ChatCompletion.create(**request)
-        LOGGER.warn(
-            json.dumps(
-                {
-                    "request": request,
-                    "response": response,
-                    "endpoint": "ChatCompletion",
-                }
-            )
+        self.logger.info(
+            {
+                "request": request,
+                "response": response,
+                "endpoint": "ChatCompletion",
+                "action": "chat_openai_llm",
+            }
         )
         return response.choices[0].message.content  # pyright: ignore
 
     def __call__(self, **content: Any) -> str:
         if self.mode == "chat":
             return self.chat(content)
         elif self.mode == "completion":
@@ -127,19 +131,36 @@
     def id(self) -> str:
         return self.paper.id
 
     def html_format_id(self) -> str:
         return self.paper.html_format_id()
 
     def html_format_summary(self) -> str:
-        return "".join([f"<p>{line}</p>" for line in self.summary.split("\n")])
+        body = "".join([f"<p>{line}</p>" for line in self.summary.split("\n")])
+        title = self.paper.html_format_title()
+        return f"{title}{body}"
 
     def format_relevant(self) -> str:
         return "✅" if self.relevant else "❌"
 
+    def to_json(self) -> Dict[str, Any]:
+        return {
+            "summary": self.summary,
+            "score": self.score,
+            "paper": self.paper.to_json(),
+        }
+
+    @classmethod
+    def from_json(cls, data: Dict[str, Any]) -> "Summary":
+        return cls(
+            summary=data["summary"],
+            score=data["score"],
+            paper=Paper.from_json(data["paper"]),
+        )
+
 
 @dataclass
 class Summaries:
     summaries: Dict[Tuple[str, str], Summary] = field(default_factory=dict)
 
     def __contains__(self, id_: str) -> bool:
         return id_ in self.summaries
@@ -155,15 +176,17 @@
         prompt: str = "",
         score: Optional[float] = None,
         paper: Optional[Paper] = None,
     ):
         if isinstance(summary, str):
             if score is None or paper is None:
                 raise ValueError("Must provide score/paper if summary is str")
-            summary = Summary(summary=summary, score=score, paper=paper)
+            summary = Summary(
+                summary=clean_html(summary), score=score, paper=paper
+            )
 
         self.summaries[(summary.id, prompt)] = summary
 
     def filter(self):
         for id_ in list(self.summaries):
             if not self.summaries[id_].relevant:
                 del self.summaries[id_]
@@ -171,9 +194,28 @@
     def table(self, prompt: Optional[str] = None) -> List[List[str]]:
         if len(self.summaries) == 0:
             # must return empty list to avoid error
             return [["", "", ""]]
 
         return [
             [s.html_format_id(), s.html_format_summary(), s.format_relevant()]
-            for s in sorted(self.iter(prompt), key=lambda s: -s.paper.score)
+            for s in sorted(
+                list(self.iter(prompt)),
+                key=lambda s: s.paper.short_id or -s.paper.score,
+            )
         ]
+
+    def to_json(self) -> Dict[str, Any]:
+        return {
+            "summaries": {
+                f"{id_}|||{prompt}": summary.to_json()
+                for (id_, prompt), summary in self.summaries.items()
+            }
+        }
+
+    @classmethod
+    def from_json(cls, data: Dict[str, Any]) -> "Summaries":
+        summaries = {}
+        for key, value in data["summaries"].items():
+            id_, prompt = key.split("|||", 1)
+            summaries[(id_, prompt)] = Summary.from_json(value)
+        return cls(summaries=summaries)
```

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/app/chat_s2/main.py` & `shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,67 +1,70 @@
 import os
 import re
+from dataclasses import dataclass
 from functools import partial
 from pathlib import Path
-from typing import List, NamedTuple, Tuple, Union
+from typing import List, Tuple, Union
 
 from shadow_scholar.cli import Argument, cli, safe_import
 
 with safe_import():
     import gradio as gr
 
     from .library import Paper, Stack
     from .llm import OpenAiPrompt, Summaries
+    from .logging import get_logger
     from .search import BaseSearchEndpoint, GoogleSearchEndpoint, Queries
 
 
 ConversationType = List[Tuple[Union[str, None], Union[str, None]]]
 
 
 SEARCH_URI = "https://api.semanticscholar.org/graph/v1/paper/search/"
 CSS_URI = Path(__file__).parent / "res" / "style.css"
 LOGO_URI = Path(__file__).parent / "res" / "logo.svg"
 JAVASCRIPT_URI = Path(__file__).parent / "res" / "script.js"
 
-
 DESCRIPTION = """\
 <div id="description">
     <div id="description-header">
         <h1>
             <span id="header-logo">{svg_logo}</span>
             <span id="header-text">Talk to Shadow Scholar</span>
         </h1>
     </div>
     <p>
         This is a demo of a chatbot that uses the <a target="_blank" \
         href="https://semanticscholar.org/">Semantic Scholar</a> API to \
-        API to answer questions about scientific papers.You can either \
-        provide it a list of papers to use, or ask the virtual scholar \
-        to search papers for you.
+        answer questions about scientific papers.You can either provide \
+        it a list of papers to use, or ask the virtual scholar to search \
+        papers for you.
     </p>
     <p>
         This virtual scholar is powered by the <a target="_blank" \
         href="https://platform.openai.com/docs/models/gpt-3">OpenAI API \
         </a> and uses the <code>{model}</code> model. It is intended as a \
         research prototype, <b>do not use it to power any user-facing \
         applications</b>.
     </p>
 </div>
 """
 
 
 QUERY_EXTRACTION_TEMPLATE = """\
-I need to find academic papers about the following prompt.
-
-"{{ prompt }}"
+I need help finding academic papers about the following topic: "{{ prompt }}".
 
 I have access to an intelligent search engine that can find papers on the \
-topic above. Could you suggest one or more queries to use? Write them as a \
-list, starting with "-". Fewer queries is better; suggest at most {{ cnt }} \
-queries. Avoid repetitive queries. Shorter queries is better.
+topic above. Could you suggest one or more queries to use? A few rules:
+- Write them as a list, starting with "-".
+- Suggest at most {% if cnt > 1 %}{{ cnt }} queries\
+{% else %}one query{% endif %}.
+- Avoid repetitive queries.
+- Shorter queries are better.
+- Do not use boolean operators, such as AND, OR, NOT, in the queries.
 """
 
 
 ANSWER_FORMULATION_TEMPLATE = """\
 I am interested in learning more about the following question: "{{ prompt }}".
 
 Using the following evidence summaries I have summarized from papers:
@@ -70,72 +73,97 @@
 {% endfor %}\
 
 Could you answer the question? A few rules:
 - Please cite the relevant snippet(s) using the format [n] \
 (for example, [{{ summaries[0].paper.short_id }}] for the first snippet).
 - Do not write a claim unless it appears in one of the snippets.
 - If a snippet is not relevant, do not use it.
-- Please be as brief and concise as possible.
-- Please explain your reasoning.
+- You must be as brief and concise as possible; do not write more than \
+five sentences.
+- You must explain your reasoning.
 - If none of the snippets contain a good answer, say that you can't answer \
 the question.
 """
 
 RESULTS_SUMMARIZATION_TEMPLATE = """\
 I am interested in learning more about the following topic: \
 "{{ prompt }}".
 
 Does the following text contain any relevant information on the topic?
 
-{{ paper.title }}
+{{ paper.title }} ({{ paper.year }})
+{{ " ".join(paper.authors) }}
 {{ paper.abstract }}
 
-If it does contain relevant information, write down one or two short \
-sentences explaining why; do not start with "relevant". \
-If the passage is not relevant, respond with "not relevant".
+If it does contain relevant information, write down one short sentences \
+explaining why; do not start with "relevant". If the passage is not relevant, \
+respond with "not relevant".
 """
 
 
 def search_and_table(
     state: "State",
     max_results: Union[int, float],
     endpoint: "BaseSearchEndpoint",
 ) -> Tuple[List[List[str]], "State"]:
-
-    for query in state.queries.use():
-        results = endpoint(query, max_results=int(max_results))
+    searches = []
+    max_results = int(max_results)
+    for query in state.queries.use(max_results):
+        results = endpoint(query, max_results=max_results)
         state.stack.extend(results)
+        searches.append({"query": query, "results": [p.id for p in results]})
 
     state.stack.fetch()
 
+    state.logger.info(
+        {
+            "searches": searches,
+            "action": "search_and_table",
+            "endpoint": endpoint.to_json(),
+        }
+    )
+
     return state.stack.table(), state
 
 
 def add_user_paper_to_chatbot(
     paper_id: str, state: "State"
 ) -> Tuple[str, List[List[str]], "State"]:
-
     paper = (
         Paper.from_url(url=paper_id)
         if paper_id.startswith("http")
         else Paper(id=paper_id)
     )
     if paper is not None:
         state.stack.append(paper)
         state.stack.fetch()
 
+    state.logger.info(
+        {
+            "action": "add_user_paper_to_chatbot",
+            "paper_id": paper_id,
+            "paper": paper.id if paper is not None else None,
+        }
+    )
+
     return "", state.stack.table(), state
 
 
 def add_user_query_to_chatbot(
     query: str, state: "State"
 ) -> Tuple[str, ConversationType, "State"]:
-
     if query := query.strip():
         state.queries.add([(query, None)])
+
+    state.logger.info(
+        {
+            "action": "add_user_query_to_chatbot",
+            "query": query,
+        }
+    )
     return "", state.queries.list(), state
 
 
 def make_queries_from_prompt(
     user_prompt: str,
     cnt_query: Union[int, float],
     state: "State",
@@ -146,14 +174,22 @@
 
     completion = model(prompt=user_prompt, cnt=int(cnt_query))
     extracted_queries = [
         strip_and_remove_quotes(q) for q in completion.split("\n") if q.strip()
     ]
     state.queries.add([(None, q) for q in extracted_queries])
 
+    state.logger.info(
+        {
+            "action": "make_queries_from_prompt",
+            "user_prompt": user_prompt,
+            "cnt_query": cnt_query,
+            "queries": extracted_queries,
+        }
+    )
     return state.queries.list(), state
 
 
 def strip_and_remove_quotes(text: str) -> str:
     text = re.sub(r"^\-\s*", "", text)
     text = re.sub(r"[\"\']+", "", text)
     text = re.sub(r"(^\s+|\s+$)", "", text)
@@ -177,14 +213,24 @@
         summary = re.sub(
             r"(^relevant.*?)([a-zA-Z])", r"\2", summary, flags=re.I
         )
         state.summaries.append(
             summary=summary, prompt=prompt, score=score, paper=paper
         )
 
+    state.logger.info(
+        {
+            "action": "summarize_results",
+            "prompt": prompt,
+            "summaries": [
+                {"paper": s.id, "summary": s.summary}
+                for s in state.summaries.iter(prompt)
+            ],
+        }
+    )
     return state.summaries.table(), state
 
 
 def compute_answer_from_summaries(
     prompt: str,
     state: "State",
     model: "OpenAiPrompt",
@@ -196,27 +242,38 @@
         s for s in state.summaries.iter(prompt) if s.relevant
     ]
 
     if not relevant_summaries:
         return "No relevant summaries found", state
 
     answer = model(prompt=prompt, summaries=relevant_summaries)
+
+    state.logger.info(
+        {
+            "action": "compute_answer_from_summaries",
+            "prompt": prompt,
+            "answer": answer,
+        }
+    )
+
     return answer, state
 
 
 def run_all_fn(
     prompt: str,
     cnt_query: int,
     max_results: int,
     state: "State",
     search_endpoint: "BaseSearchEndpoint",
     query_prompt_model: "OpenAiPrompt",
     answer_prompt_model: "OpenAiPrompt",
     results_summarization: "OpenAiPrompt",
 ):
+    state = State.new()
+
     # make queries from prompt
     queries, state = make_queries_from_prompt(
         user_prompt=prompt,
         cnt_query=cnt_query,
         state=state,
         model=query_prompt_model,
     )
@@ -243,25 +300,63 @@
     )
 
     return [queries, results, summaries, output, state]
 
 
 def clear_all():
     state = State.new()
-    return "", "", state.queries.list(), state.stack.table(), state
+    return (
+        "",
+        "",
+        state.queries.list(),
+        state.stack.table(),
+        state.summaries.table(),
+        state,
+    )
+
+
+def rate_feedback(prompt: str, output: str, state: "State", score: int):
+    state.logger.warn(
+        {
+            "action": "rate_feedback_interaction",
+            "prompt": prompt,
+            "output": output,
+            "score": score,
+            "state": state.to_json(),
+        }
+    )
 
 
-class State(NamedTuple):
+@dataclass
+class State:
     stack: "Stack"
     queries: "Queries"
     summaries: "Summaries"
 
+    def __post_init__(self):
+        self.logger = get_logger(__name__)
+
     @classmethod
     def new(cls) -> "State":
-        return cls(stack=Stack(), queries=Queries(), summaries=Summaries())
+        return State(stack=Stack(), queries=Queries(), summaries=Summaries())
+
+    def to_json(self):
+        return {
+            "stack": self.stack.to_json(),
+            "queries": self.queries.to_json(),
+            "summaries": self.summaries.to_json(),
+        }
+
+    @classmethod
+    def from_json(cls, json):
+        return cls(
+            stack=Stack.from_json(json["stack"]),
+            queries=Queries.from_json(json["queries"]),
+            summaries=Summaries.from_json(json["summaries"]),
+        )
 
 
 @cli(
     "app.chat_s2",
     arguments=[
         Argument(
             "-sp",
@@ -297,17 +392,20 @@
             "-gk",
             "--google-custom-search-key",
             default=os.environ.get("GOOGLE_CUSTOM_SEARCH_API_KEY"),
         ),
     ],
     requirements=[
         "requests",
-        "transformers",
         "openai",
         "jinja2",
+        "gradio>=3.23.0",
+        "watchtower",
+        "logging_json",
+        "edlib",
     ],
 )
 def run_v2_demo(
     server_port: int,
     server_name: str,
     openai_key: str,
     llm_model: str,
@@ -332,38 +430,44 @@
         title="Talk to Shadow Scholar ",
         css=css_gradio,
         analytics_enabled=False,
     ) as demo:
         gr.HTML(DESCRIPTION.format(svg_logo=svg_logo, model=llm_model))
         state = gr.State(State.new)  # pyright: ignore
 
-        with gr.Row():
-            with gr.Column(scale=1):
+        with gr.Row(variant="panel"):
+            with gr.Column(scale=3):
                 run_all = gr.Button(
                     "Run End-to-End",
                     variant="primary",
                     elem_id="run-end-to-end",
                 )
                 prompt = gr.Textbox(
                     interactive=True,
                     label="Prompt",
                     lines=5,
                     max_lines=5,
                     placeholder="What would you like to know about?",
                 )
 
-            with gr.Column(scale=1):
+            with gr.Column(scale=3):
                 clear = gr.Button("Clear All", variant="stop")
                 output = gr.Textbox(
                     interactive=False,
                     label="Output",
                     lines=5,
                     placeholder="Provide a prompt to get started",
                 )
 
+            with gr.Column(min_width=50):
+                gr.HTML('<div id="rate-text">Rate Output</div>')
+                with gr.Row(variant="compact"):
+                    feedback_positive = gr.Button("👍")
+                    feedback_negative = gr.Button("👎")
+
         gr.Markdown("## 1️⃣ Search Pipeline")
         with gr.Row(variant="panel"):
             with gr.Column(scale=1, min_width=200):
                 with gr.Row():
                     with gr.Column(min_width=100):
                         make_queries = gr.Button(
                             "Get Queries",
@@ -501,29 +605,36 @@
             [prompt, state],
             [output, state],
         )
 
         clear.click(
             clear_all,
             [],
-            [prompt, output, queries, results, state],
+            [prompt, output, queries, results, summaries, state],
         )
 
         run_all.click(
             partial(
                 run_all_fn,
                 search_endpoint=search_endpoint,
                 query_prompt_model=query_prompt_model,
                 answer_prompt_model=answer_prompt_model,
                 results_summarization=results_summarization,
             ),
             [prompt, cnt_query, max_results, state],
             [queries, results, summaries, output, state],
         )
 
+        feedback_positive.click(
+            partial(rate_feedback, score=1), [prompt, output, state]
+        )
+        feedback_negative.click(
+            partial(rate_feedback, score=-1), [prompt, output, state]
+        )
+
     try:
         demo.launch(
             server_name=server_name,
             server_port=server_port,
             show_api=False,
         )
     except Exception as e:
```

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/app/chat_s2/res/style.css` & `shadow-scholar-0.6.0/src/shadow_scholar/app/chat_s2/res/style.css`

 * *Files 10% similar despite different names*

```diff
@@ -40,14 +40,23 @@
     font-weight: bold;
 }
 
 button.match-height{
     height: 100%;
 }
 
+div#rate-text {
+    margin-top: 0.5em;
+    margin-bottom: 2em;
+    margin-left: auto;
+    margin-right: auto;
+    text-align: center;
+    font-size: 1.5em;
+}
+
 div#description{
     max-width: 640px;
     margin: 0em auto 2em auto;
     display: grid;
 }
 
 .paper_row {
```

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/app/galactica/_old.py` & `shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/_old.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/app/galactica/constants.py` & `shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/constants.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/app/galactica/convert_to_int8.py` & `shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/convert_to_int8.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/app/galactica/example.png` & `shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/example.png`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/app/galactica/galai_model.py` & `shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/galai_model.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/app/galactica/galai_parallel_policy.py` & `shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/galai_parallel_policy.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/app/galactica/galai_utils.py` & `shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/galai_utils.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/app/galactica/main.py` & `shadow-scholar-0.6.0/src/shadow_scholar/app/galactica/main.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/app/hello_world/main.py` & `shadow-scholar-0.6.0/src/shadow_scholar/app/hello_world/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,56 @@
-from typing import Callable, List, Union
 from pathlib import Path
 
 from shadow_scholar.cli import Argument, cli, safe_import
 
 with safe_import():
     import gradio as gr
+
     # from fastapi import FastAPI
     # import uvicorn
 
 
 S2R_URL = "https://www.semanticscholar.org/research/research-team"
 SWS_URL = "https://github.com/allenai/shadow-scholar"
 CSS_URI = Path(__file__).parent / "res" / "style.css"
 IMG_URI = Path(__file__).parent / "res" / "logo.png"
 
 
 @cli(
     "app.hello_world",
     arguments=[
-        Argument("--host", default='localhost', help="Host to bind to"),
+        Argument("--host", default="localhost", help="Host to bind to"),
         Argument("--port", default=7860, type=int, help="Port to bind to"),
     ],
     requirements=["gradio"],
 )
 def run_hello_world(
     host: str,
     port: int,
 ):
     with open(CSS_URI, "r") as f:
         css = f.read()
 
     with gr.Blocks(title="Shadow Scholar", css=css) as app:
-        gr.Markdown(
-            "# 🕶️ 🎓 Shadow Scholar 🎓 🕶️",
-            elem_id="center"
-        )
+        gr.Markdown("# 🕶️ 🎓 Shadow Scholar 🎓 🕶️", elem_id="center")
         gr.Image(
             str(IMG_URI),
             elem_id="logo",
             shape=(400, 400),
             show_label=False,
             interactive=False,
         )
         gr.Markdown(
             "Shadow Scholar is a collection of tools and applications "
             f"from the [S2 Research Team]({S2R_URL}). To learn more about "
             f"this project, please visit our [GitHub repository]({SWS_URL}). "
             f"To install shadow scholar, run `pip install shadow-scholar`.",
-            elem_id="center"
+            elem_id="center",
         )
 
     try:
-        app.launch(server_name=host, server_port=port, show_api=False, inline=True)
+        app.launch(
+            server_name=host, server_port=port, show_api=False, inline=True
+        )
     except Exception as e:
         app.close()
         raise e
```

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/app/hello_world/res/logo.png` & `shadow-scholar-0.6.0/src/shadow_scholar/app/hello_world/res/logo.png`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/app/llama/main.py` & `shadow-scholar-0.6.0/src/shadow_scholar/app/llama/main.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/app/pdod/caches.py` & `shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/caches.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from abc import ABC, abstractmethod, abstractproperty
 from enum import IntEnum
 from typing import Any, Dict, Literal, Sequence, Union
+
 from shadow_scholar.cli import safe_import
 
 with safe_import():
-    from unqlite import UnQLite
-    import torch
     import numpy as np
+    import torch
+    from unqlite import UnQLite
 
 
 TensorType = Union[torch.Tensor, np.ndarray]
 
 
 class CacheMode(IntEnum):
     READ_ONLY = 1
```

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/app/pdod/datasets.py` & `shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/datasets.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/app/pdod/main.py` & `shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/main.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/app/pdod/mmda_utils.py` & `shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/mmda_utils.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/app/pdod/rankers.py` & `shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/rankers.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/app/pdod/reg_utils.py` & `shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/reg_utils.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/app/pdod/slicers.py` & `shadow-scholar-0.6.0/src/shadow_scholar/app/pdod/slicers.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/app/qa/data.py` & `shadow-scholar-0.6.0/src/shadow_scholar/app/qa/data.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/app/qa/main.py` & `shadow-scholar-0.6.0/src/shadow_scholar/app/qa/main.py`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/cli.py` & `shadow-scholar-0.6.0/src/shadow_scholar/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,40 +15,46 @@
     List,
     NamedTuple,
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
+    cast,
 )
 
 from necessary import necessary
-from typing_extensions import ParamSpec
+from typing_extensions import ParamSpec, TypeAlias
 
 # parameter spec
 PS = ParamSpec("PS")
 
 # return type
 RT = TypeVar("RT")
 
 # generic type
 T = TypeVar("T")
 
-# sentinel value
-M = object()
+# type alias for a requirement
+RequirementType: TypeAlias = Union[str, Tuple[str, str], "NamedRequirement"]
 
 
 # sentinel value for missing arguments
 class _M:
     ...  # noqa: E701
 
 
 M = _M()  # noqa: E305
 
 
+class ShadowModuleNotFoundError(ModuleNotFoundError):
+    # make easier to track when this error is raised
+    ...
+
+
 class Argument:
     """Holds parameters for argparse.ArgumentParser.add_argument."""
 
     args: Tuple[str, ...]
     kwargs: Dict[str, Any]
 
     def __init__(
@@ -87,15 +93,17 @@
 
 
 class NamedRequirement(NamedTuple):
     name: str
     package: str
 
     @classmethod
-    def parse(cls, elem: Union[str, Tuple[str, str]]) -> "NamedRequirement":
+    def parse(cls, elem: RequirementType) -> "NamedRequirement":
+        if isinstance(elem, cls):
+            return elem
         if isinstance(elem, str):
             return cls(elem, elem)
         elif isinstance(elem, tuple):
             return cls(*elem)
         else:
             raise TypeError(f"Expected str or 2-tuple, got {type(elem)}")
 
@@ -108,15 +116,15 @@
 
 class EntryPoint(Generic[PS, RT]):
     def __init__(
         self,
         name: str,
         func: Callable[PS, RT],
         args: List[Argument],
-        reqs: List[Union[str, Tuple[str, str]]],
+        reqs: List[RequirementType],
     ):
         self.name = name
         self.func = func
         self.args = args
 
         # if receiving a tuple, the first element is the name of the
         # package and the second is the name of the module to import
@@ -137,18 +145,16 @@
         """
         return SpecTuple(self.name, self.func.__name__, self.func.__module__)
 
     def __call__(self, *args: PS.args, **kwargs: PS.kwargs) -> RT:
         """Run the function."""
 
         if self.missing_reqs:
-            raise ModuleNotFoundError(
-                f"Missing requirements: {' '.join(self.missing_reqs)}; "
-                f"run `shadow -r {self.name}` to list all requirements for "
-                "this entrypoint."
+            raise ShadowModuleNotFoundError(
+                f"Missing requirements: {' '.join(self.missing_reqs)}"
             )
         return self.func(*args, **kwargs)
 
     def cli(
         self,
         args: Optional[List[str]] = None,
         file_config: Optional[Dict[str, Any]] = None,
@@ -183,15 +189,16 @@
 
     @classmethod
     def decorate(
         cls,
         func: Callable[PS, RT],
         name: Optional[str] = None,
         arguments: Optional[List[Argument]] = None,
-        requirements: Optional[List[Union[str, Tuple[str, str]]]] = None,
+        requirements: Optional[List[RequirementType]] = None,
+        registry: Optional["Registry"] = None,
     ) -> "EntryPoint[PS, RT]":
         """Decorator designed to add function to a registry alongside
         all its arguments and requirements.
 
         We add the requirement for future parsing, rather than
         building a ArgumentParser here, for two reasons:
         1. We want to be able for all decorated functions to be able to
@@ -206,14 +213,16 @@
                 function name is used. Defaults to None.
             arguments (List[Argument], optional): A list of Argument objects
                 to be passed to the ArgumentParser. The available options
                 are the same as those for argparse.ArgumentParser.add_argument.
                 Defaults to None.
             requirements (Optional[List[str]], optional): A list of required
                 packages for the function to run. Defaults to None.
+            registry (Registry, optional): The registry to add the function
+                to. If none is provided, the entrypoint is not registered.
         """
 
         name = name or func.__name__
         arguments = arguments or []
         func_requirements = requirements or []
 
         # create the entry point by wrapping the function
@@ -221,15 +230,15 @@
             name=name,
             func=func,
             args=arguments,
             reqs=func_requirements,
         )
 
         # add the function to the registry
-        Registry().add(entry_point)
+        registry.add(entry_point) if registry else None
 
         return entry_point
 
 
 class Registry:
     """A registry to hold all the functions decorated with @cli."""
 
@@ -257,35 +266,43 @@
 
         self._registry[entry_point.name] = entry_point
 
     def cli(
         self,
         name: Optional[str] = None,
         arguments: Optional[List[Argument]] = None,
-        requirements: Optional[List[Union[str, Tuple[str, str]]]] = None,
+        requirements: Optional[List[RequirementType]] = None,
     ) -> Callable[[Callable[PS, RT]], "EntryPoint[PS, RT]"]:
         """A decorator to add a function to the registry.
 
         Args:
             name (str, optional): Name to use for the function
                 when it is called from the command line. If none is provided,
                 the function name is used. Defaults to None.
             arguments (List[Argument], optional): A list of Argument objects
                 to be passed to the ArgumentParser. The available options
                 are the same as those for argparse.ArgumentParser.add_argument.
                 Defaults to None.
-            requirements (Optional[List[str]], optional): A list of required
+            requirements: A list of requirements for the function. Can
+                be either a list of strings (e.g., ["spacy"]), a list that
+                includes the minimum versions (e.g., ["spacy>=3.0.0"]), or a
+                list of tuples (e.g., [("scikit-learn>=0.24.0", "sklearn"),
+                "spacy"]) for cases where the package name is different from
+                the import name.
         """
         decorated = partial(
-            EntryPoint.decorate,  # type: ignore
+            # need to make types more permissive here because otherwise
+            # mypy complains about the partial not being a callable
+            cast(Callable[..., EntryPoint[PS, RT]], EntryPoint.decorate),
             name=name,
             arguments=arguments,
             requirements=requirements,
+            registry=self,
         )
-        return decorated  # type: ignore
+        return decorated  # pyright: ignore
 
     def _formatted_entrypoints(self, sep="   ") -> str:
         term_width = shutil.get_terminal_size().columns
 
         l_col, r_col = zip(
             *(
                 (e.spec.name, f"{e.spec.module}.{e.spec.func}")
@@ -401,34 +418,65 @@
             sys.exit(0)
 
         config = {}
         if opts.config_path:
             with open(opts.config_path) as f:
                 config = json.load(f)
 
-        entrypoint.cli(args=post_args, file_config=config)
+        try:
+            entrypoint.cli(args=post_args, file_config=config)
+        except ShadowModuleNotFoundError as e:
+            e.msg += (
+                f"; run `shadow -r {entry_name}` to list all requirements "
+                "for this entrypoint."
+            )
+            raise e
+
+    def require(
+        self, requirements: List[RequirementType]
+    ) -> Callable[[Callable[PS, RT]], EntryPoint[PS, RT]]:
+        """Specifies a list of requirements for a function.
+
+        Args:
+            requirements: A list of requirements for the function. Can
+                be either a list of strings (e.g., ["spacy"]), a list that
+                includes the minimum versions (e.g., ["spacy>=3.0.0"]), or a
+                list of tuples (e.g., [("scikit-learn>=0.24.0", "sklearn"),
+                "spacy"]) for cases where the package name is different from
+                the import name.
+        """
+
+        decorated = partial(
+            cast(Callable[..., EntryPoint[PS, RT]], EntryPoint.decorate),
+            requirements=requirements,
+        )
+        return decorated  # type: ignore
 
 
 @contextmanager
 def safe_import():
-    """Context manager to safely import a package.
-
-    Args:
-        package (str): Name of the package to import.
-    """
+    """Context manager to safely import a package."""
     try:
         yield
     except (ModuleNotFoundError, ImportError):
         pass
 
 
 def load_kwargs(path_or_json: str) -> Dict[str, Any]:
+    """Load a json file containing a config, or a json string."""
+
     if Path(path_or_json).exists():
         with open(path_or_json) as f:
             path_or_json = f.read()
-    return json.loads(path_or_json)
+
+    try:
+        return json.loads(path_or_json)
+    except json.JSONDecodeError as e:
+        err = ValueError(f"Could not parse json {path_or_json}.")
+        raise err from e
 
 
 run = Registry().run
 cli = Registry().cli
+require = Registry().require
 
-__all__ = ["run", "cli", "Argument", "safe_import", "load_kwargs"]
+__all__ = ["run", "cli", "Argument", "safe_import", "load_kwargs", "require"]
```

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/collections/athena.py` & `shadow-scholar-0.6.0/src/shadow_scholar/collections/athena.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
             "--abstract",
             default=None,
             type=str,
             help="text to search in the abstract",
         ),
         *run_athena_query_and_get_result.args,
     ],
-    requirements=run_athena_query_and_get_result.reqs,
+    requirements=run_athena_query_and_get_result.reqs,  # type: ignore
 )
 def get_s2ag_abstracts(
     database: str,
     release: str,
     limit: int,
     output_location: str,
     s3_staging: str,
```

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/collections/queries/acl_anthology.sql` & `shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/acl_anthology.sql`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/collections/queries/s2ag_abstracts.sql` & `shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_abstracts.sql`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/collections/queries/s2ag_authors.sql` & `shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_authors.sql`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/collections/queries/s2ag_citations.sql` & `shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_citations.sql`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/collections/queries/s2ag_papers.sql` & `shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_papers.sql`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar/collections/queries/s2ag_s2orc.sql` & `shadow-scholar-0.6.0/src/shadow_scholar/collections/queries/s2ag_s2orc.sql`

 * *Files identical despite different names*

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar.egg-info/PKG-INFO` & `shadow-scholar-0.6.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadow-scholar
-Version: 0.5.0
+Version: 0.6.0
 Summary: 🎓🕶️ A collection of utilities and demos from the Semantic Scholar Research Team 🕶️🎓
 Author-email: Luca Soldaini <lucas@allenai.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/allenai/shadow-scholar
 Project-URL: Source, https://github.com/allenai/shadow-scholar
 Project-URL: Tracker, https://github.com/allenai/shadow-scholar/issues
 Classifier: Development Status :: 3 - Alpha
@@ -15,14 +15,21 @@
 License-File: LICENSE
 
 <h1 align="center">Shadow Scholar</h1>
 <p align="center">
     <img src="https://raw.githubusercontent.com/allenai/shadow-scholar/main/res/shadow-scholar.png" width="400" height="400" align="center" />
 </p>
 
+**Table of Contents**
+- [Installation](#installation)
+- [Available Scripts](#available-scripts)
+- [Getting Access to AWS services](#getting-access-to-aws-services)
+- [Adding Your Own Script](#adding-your-own-script-application-entry-point)
+- [Adding A New Module](#adding-a-new-module-available-to-all-scriptsas-a-dependency)
+
 ## Installation
 
 To install from PyPI, simply run:
 
 ```bash
 pip install shadow-scholar
 ```
@@ -39,15 +46,15 @@
 
 - [Athena](https://aws.amazon.com/athena/)
 - [S3](https://aws.amazon.com/s3/)
 
 The best way to do so is to obtain AWS credentials (access key and secret key) and set them as environment variables.
 
 
-## Writing your own script
+## Adding Your Own Script (Application Entry Point)
 
 To write your own script for Shadow Scholar, follow these steps:
 
 **Step 1**: Choose where to add your code in Shadow Scholar. It can either be
 in an existing module, such as `shadow_scholar.collections.athena`, or in a
 new module.
 
@@ -200,7 +207,26 @@
 **Step 7**: Import the function in the `__init__.py` file of the module. For
 example, if you added your script to `shadow_scholar/examples.py`, you would
 add the following to `shadow_scholar/__init__.py`:
 
 ```python
 from shadow_scholar.examples import my_script
 ```
+
+
+## Adding A New Module (Available to All Scripts/as a Dependency)
+
+Adding a module to Shadow Scholar is as easy as adding a script, but,
+instead of decorating the main entry-point function with `cli`, you need
+to use the `@require` decorator. For example:
+
+```python
+from shadow_scholar.cli import require, safe_import
+
+with safe_import():
+    import requests
+
+@require(["requests>=2.0.0"])
+def module_function():
+    # Do something with requests
+    requests.get(...)
+```
```

### Comparing `shadow-scholar-0.5.0/src/shadow_scholar.egg-info/SOURCES.txt` & `shadow-scholar-0.6.0/src/shadow_scholar.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 src/shadow_scholar/__init__.py
 src/shadow_scholar/__main__.py
 src/shadow_scholar/cli.py
+src/shadow_scholar/hello_world.py
 src/shadow_scholar.egg-info/PKG-INFO
 src/shadow_scholar.egg-info/SOURCES.txt
 src/shadow_scholar.egg-info/dependency_links.txt
 src/shadow_scholar.egg-info/entry_points.txt
 src/shadow_scholar.egg-info/requires.txt
 src/shadow_scholar.egg-info/top_level.txt
 src/shadow_scholar/app/__init__.py
 src/shadow_scholar/app/chat_s2/__init__.py
-src/shadow_scholar/app/chat_s2/_old.py
 src/shadow_scholar/app/chat_s2/library.py
 src/shadow_scholar/app/chat_s2/llm.py
+src/shadow_scholar/app/chat_s2/logging.py
 src/shadow_scholar/app/chat_s2/main.py
 src/shadow_scholar/app/chat_s2/search.py
+src/shadow_scholar/app/chat_s2/res/logo.svg
 src/shadow_scholar/app/chat_s2/res/style.css
 src/shadow_scholar/app/galactica/__init__.py
 src/shadow_scholar/app/galactica/_old.py
 src/shadow_scholar/app/galactica/constants.py
 src/shadow_scholar/app/galactica/convert_to_int8.py
 src/shadow_scholar/app/galactica/example.png
 src/shadow_scholar/app/galactica/galai_model.py
@@ -54,8 +56,10 @@
 src/shadow_scholar/collections/queries/s2ag_citations.sql
 src/shadow_scholar/collections/queries/s2ag_embeddings.sql
 src/shadow_scholar/collections/queries/s2ag_paper_ids.sql
 src/shadow_scholar/collections/queries/s2ag_papers.sql
 src/shadow_scholar/collections/queries/s2ag_publication_venues.sql
 src/shadow_scholar/collections/queries/s2ag_s2orc.sql
 src/shadow_scholar/collections/queries/s2ag_tldrs.sql
+src/shadow_scholar/util/__init__.py
+src/shadow_scholar/util/s2_api.py
 tests/test_imports.py
```


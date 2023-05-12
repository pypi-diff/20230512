# Comparing `tmp/mcrit-1.0.0.tar.gz` & `tmp/mcrit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcrit-1.0.0.tar", last modified: Mon Apr 10 16:38:50 2023, max compression
+gzip compressed data, was "mcrit-1.0.1.tar", last modified: Fri May 12 14:54:29 2023, max compression
```

## Comparing `mcrit-1.0.0.tar` & `mcrit-1.0.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-04-10 16:38:50.104970 mcrit-1.0.0/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    35149 2022-05-13 09:44:28.000000 mcrit-1.0.0/LICENSE
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    12656 2023-04-10 16:38:50.104970 mcrit-1.0.0/PKG-INFO
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    10327 2023-04-10 16:33:01.000000 mcrit-1.0.0/README.md
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-04-10 16:38:50.100970 mcrit-1.0.0/mcrit/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    21415 2022-12-14 11:14:13.000000 mcrit-1.0.0/mcrit/Worker.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/__init__.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1838 2023-03-21 09:06:40.000000 mcrit-1.0.0/mcrit/__main__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-04-10 16:38:50.100970 mcrit-1.0.0/mcrit/client/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    28146 2023-03-24 15:01:21.000000 mcrit-1.0.0/mcrit/client/McritClient.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    17638 2023-04-10 16:19:48.000000 mcrit-1.0.0/mcrit/client/McritConsole.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/client/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-04-10 16:38:50.100970 mcrit-1.0.0/mcrit/config/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      855 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/config/ConfigInterface.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      960 2023-04-10 15:55:00.000000 mcrit-1.0.0/mcrit/config/McritConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2148 2023-04-10 15:53:10.000000 mcrit-1.0.0/mcrit/config/MinHashConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      821 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/config/QueueConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1974 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/config/ShinglerConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1775 2022-07-29 10:29:16.000000 mcrit-1.0.0/mcrit/config/StorageConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/config/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-04-10 16:38:50.100970 mcrit-1.0.0/mcrit/index/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    29049 2023-04-10 15:53:10.000000 mcrit-1.0.0/mcrit/index/MinHashIndex.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3890 2022-08-08 11:41:38.000000 mcrit-1.0.0/mcrit/index/SearchCursor.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6210 2022-08-08 11:41:38.000000 mcrit-1.0.0/mcrit/index/SearchQueryParser.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6366 2022-08-08 11:41:38.000000 mcrit-1.0.0/mcrit/index/SearchQueryTree.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/index/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-04-10 16:38:50.100970 mcrit-1.0.0/mcrit/libs/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/libs/__init__.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    16784 2022-08-23 11:53:24.000000 mcrit-1.0.0/mcrit/libs/mongoqueue.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    14152 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/libs/pymmh3.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2028 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/libs/utility.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-04-10 16:38:50.100970 mcrit-1.0.0/mcrit/matchers/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6378 2022-08-31 07:13:17.000000 mcrit-1.0.0/mcrit/matchers/MatcherCross.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    28260 2023-04-10 15:53:10.000000 mcrit-1.0.0/mcrit/matchers/MatcherInterface.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3014 2022-11-25 14:50:57.000000 mcrit-1.0.0/mcrit/matchers/MatcherQuery.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3097 2023-04-10 15:53:10.000000 mcrit-1.0.0/mcrit/matchers/MatcherQueryFunction.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      751 2022-09-28 13:53:00.000000 mcrit-1.0.0/mcrit/matchers/MatcherSample.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2429 2022-12-14 11:14:13.000000 mcrit-1.0.0/mcrit/matchers/MatcherVs.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-08-29 06:59:30.000000 mcrit-1.0.0/mcrit/matchers/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-04-10 16:38:50.100970 mcrit-1.0.0/mcrit/minhash/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3662 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/minhash/MinHash.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    10547 2022-11-11 10:02:06.000000 mcrit-1.0.0/mcrit/minhash/MinHasher.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3212 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/minhash/ShingleLoader.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/minhash/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-04-10 16:38:50.104970 mcrit-1.0.0/mcrit/queue/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    10980 2022-08-31 07:13:17.000000 mcrit-1.0.0/mcrit/queue/LocalQueue.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1308 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/queue/QueueFactory.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    14987 2022-10-12 12:19:42.000000 mcrit-1.0.0/mcrit/queue/QueueRemoteCalls.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-08-29 06:36:44.000000 mcrit-1.0.0/mcrit/queue/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-04-10 16:38:50.104970 mcrit-1.0.0/mcrit/server/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1297 2023-03-21 14:19:34.000000 mcrit-1.0.0/mcrit/server/BlocksResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6004 2023-03-21 14:19:34.000000 mcrit-1.0.0/mcrit/server/FamilyResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3486 2023-03-21 14:19:34.000000 mcrit-1.0.0/mcrit/server/FunctionResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     4609 2023-03-21 14:19:34.000000 mcrit-1.0.0/mcrit/server/JobResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3551 2023-03-21 14:19:34.000000 mcrit-1.0.0/mcrit/server/MatchResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     7608 2023-03-22 15:50:20.000000 mcrit-1.0.0/mcrit/server/QueryResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    11793 2023-03-21 14:19:34.000000 mcrit-1.0.0/mcrit/server/SampleResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     5159 2023-03-21 14:19:34.000000 mcrit-1.0.0/mcrit/server/StatusResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/server/__init__.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     5887 2023-03-17 17:07:42.000000 mcrit-1.0.0/mcrit/server/application_routes.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1868 2023-03-21 14:19:34.000000 mcrit-1.0.0/mcrit/server/utils.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)       69 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/server/wsgi.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-04-10 16:38:50.104970 mcrit-1.0.0/mcrit/storage/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2077 2022-08-03 10:24:19.000000 mcrit-1.0.0/mcrit/storage/FamilyEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6415 2023-03-21 14:19:34.000000 mcrit-1.0.0/mcrit/storage/FunctionEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1661 2023-03-21 14:19:34.000000 mcrit-1.0.0/mcrit/storage/FunctionLabelEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2764 2023-02-27 12:31:29.000000 mcrit-1.0.0/mcrit/storage/MatchedFunctionEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6617 2023-02-14 15:17:18.000000 mcrit-1.0.0/mcrit/storage/MatchedSampleEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1389 2023-04-10 15:53:10.000000 mcrit-1.0.0/mcrit/storage/MatchingCache.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    21812 2023-03-14 13:04:24.000000 mcrit-1.0.0/mcrit/storage/MatchingResult.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    44811 2023-03-24 15:01:21.000000 mcrit-1.0.0/mcrit/storage/MemoryStorage.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    59588 2023-03-24 15:01:21.000000 mcrit-1.0.0/mcrit/storage/MongoDbStorage.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     4932 2023-03-17 17:07:42.000000 mcrit-1.0.0/mcrit/storage/SampleEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      735 2022-11-13 10:29:45.000000 mcrit-1.0.0/mcrit/storage/StorageFactory.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    25158 2023-03-21 14:19:34.000000 mcrit-1.0.0/mcrit/storage/StorageInterface.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.0/mcrit/storage/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-04-10 16:38:50.100970 mcrit-1.0.0/mcrit.egg-info/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    12656 2023-04-10 16:38:49.000000 mcrit-1.0.0/mcrit.egg-info/PKG-INFO
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1950 2023-04-10 16:38:49.000000 mcrit-1.0.0/mcrit.egg-info/SOURCES.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        1 2023-04-10 16:38:49.000000 mcrit-1.0.0/mcrit.egg-info/dependency_links.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      135 2023-04-10 16:38:49.000000 mcrit-1.0.0/mcrit.egg-info/requires.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        6 2023-04-10 16:38:49.000000 mcrit-1.0.0/mcrit.egg-info/top_level.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)       38 2023-04-10 16:38:50.104970 mcrit-1.0.0/setup.cfg
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1355 2023-04-10 16:10:06.000000 mcrit-1.0.0/setup.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-05-12 14:54:29.865078 mcrit-1.0.1/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    35149 2022-05-13 09:44:28.000000 mcrit-1.0.1/LICENSE
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    12788 2023-05-12 14:54:29.865078 mcrit-1.0.1/PKG-INFO
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    10451 2023-05-12 14:53:49.000000 mcrit-1.0.1/README.md
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-05-12 14:54:29.857078 mcrit-1.0.1/mcrit/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    21415 2022-12-14 11:14:13.000000 mcrit-1.0.1/mcrit/Worker.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/__init__.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1838 2023-03-21 09:06:40.000000 mcrit-1.0.1/mcrit/__main__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-05-12 14:54:29.857078 mcrit-1.0.1/mcrit/client/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    28489 2023-05-12 13:29:52.000000 mcrit-1.0.1/mcrit/client/McritClient.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    17638 2023-04-10 16:19:48.000000 mcrit-1.0.1/mcrit/client/McritConsole.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/client/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-05-12 14:54:29.861078 mcrit-1.0.1/mcrit/config/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      855 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/config/ConfigInterface.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      960 2023-05-12 14:54:03.000000 mcrit-1.0.1/mcrit/config/McritConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2148 2023-04-10 15:53:10.000000 mcrit-1.0.1/mcrit/config/MinHashConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      821 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/config/QueueConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1974 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/config/ShinglerConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1775 2022-07-29 10:29:16.000000 mcrit-1.0.1/mcrit/config/StorageConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/config/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-05-12 14:54:29.861078 mcrit-1.0.1/mcrit/index/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    29120 2023-04-26 15:34:26.000000 mcrit-1.0.1/mcrit/index/MinHashIndex.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3890 2022-08-08 11:41:38.000000 mcrit-1.0.1/mcrit/index/SearchCursor.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6210 2022-08-08 11:41:38.000000 mcrit-1.0.1/mcrit/index/SearchQueryParser.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6366 2022-08-08 11:41:38.000000 mcrit-1.0.1/mcrit/index/SearchQueryTree.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/index/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-05-12 14:54:29.861078 mcrit-1.0.1/mcrit/libs/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/libs/__init__.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    16784 2022-08-23 11:53:24.000000 mcrit-1.0.1/mcrit/libs/mongoqueue.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    14152 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/libs/pymmh3.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2028 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/libs/utility.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-05-12 14:54:29.861078 mcrit-1.0.1/mcrit/matchers/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6378 2022-08-31 07:13:17.000000 mcrit-1.0.1/mcrit/matchers/MatcherCross.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    28260 2023-04-10 15:53:10.000000 mcrit-1.0.1/mcrit/matchers/MatcherInterface.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3014 2022-11-25 14:50:57.000000 mcrit-1.0.1/mcrit/matchers/MatcherQuery.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3097 2023-04-10 15:53:10.000000 mcrit-1.0.1/mcrit/matchers/MatcherQueryFunction.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      751 2022-09-28 13:53:00.000000 mcrit-1.0.1/mcrit/matchers/MatcherSample.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2429 2022-12-14 11:14:13.000000 mcrit-1.0.1/mcrit/matchers/MatcherVs.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-08-29 06:59:30.000000 mcrit-1.0.1/mcrit/matchers/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-05-12 14:54:29.865078 mcrit-1.0.1/mcrit/minhash/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3662 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/minhash/MinHash.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    10547 2022-11-11 10:02:06.000000 mcrit-1.0.1/mcrit/minhash/MinHasher.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3212 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/minhash/ShingleLoader.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/minhash/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-05-12 14:54:29.865078 mcrit-1.0.1/mcrit/queue/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    10980 2022-08-31 07:13:17.000000 mcrit-1.0.1/mcrit/queue/LocalQueue.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1308 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/queue/QueueFactory.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    14987 2022-10-12 12:19:42.000000 mcrit-1.0.1/mcrit/queue/QueueRemoteCalls.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-08-29 06:36:44.000000 mcrit-1.0.1/mcrit/queue/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-05-12 14:54:29.865078 mcrit-1.0.1/mcrit/server/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1297 2023-03-21 14:19:34.000000 mcrit-1.0.1/mcrit/server/BlocksResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6004 2023-03-21 14:19:34.000000 mcrit-1.0.1/mcrit/server/FamilyResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3764 2023-05-12 13:35:06.000000 mcrit-1.0.1/mcrit/server/FunctionResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     4609 2023-03-21 14:19:34.000000 mcrit-1.0.1/mcrit/server/JobResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3551 2023-03-21 14:19:34.000000 mcrit-1.0.1/mcrit/server/MatchResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     7608 2023-03-22 15:50:20.000000 mcrit-1.0.1/mcrit/server/QueryResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    11793 2023-03-21 14:19:34.000000 mcrit-1.0.1/mcrit/server/SampleResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     5159 2023-03-21 14:19:34.000000 mcrit-1.0.1/mcrit/server/StatusResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/server/__init__.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     5887 2023-03-17 17:07:42.000000 mcrit-1.0.1/mcrit/server/application_routes.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1868 2023-03-21 14:19:34.000000 mcrit-1.0.1/mcrit/server/utils.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)       69 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/server/wsgi.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-05-12 14:54:29.865078 mcrit-1.0.1/mcrit/storage/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2077 2022-08-03 10:24:19.000000 mcrit-1.0.1/mcrit/storage/FamilyEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6415 2023-03-21 14:19:34.000000 mcrit-1.0.1/mcrit/storage/FunctionEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1661 2023-03-21 14:19:34.000000 mcrit-1.0.1/mcrit/storage/FunctionLabelEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2764 2023-02-27 12:31:29.000000 mcrit-1.0.1/mcrit/storage/MatchedFunctionEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6617 2023-02-14 15:17:18.000000 mcrit-1.0.1/mcrit/storage/MatchedSampleEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1389 2023-04-10 15:53:10.000000 mcrit-1.0.1/mcrit/storage/MatchingCache.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    21812 2023-05-08 07:42:59.000000 mcrit-1.0.1/mcrit/storage/MatchingResult.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    44811 2023-03-24 15:01:21.000000 mcrit-1.0.1/mcrit/storage/MemoryStorage.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    59597 2023-04-26 15:32:48.000000 mcrit-1.0.1/mcrit/storage/MongoDbStorage.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     4932 2023-03-17 17:07:42.000000 mcrit-1.0.1/mcrit/storage/SampleEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      735 2022-11-13 10:29:45.000000 mcrit-1.0.1/mcrit/storage/StorageFactory.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    25158 2023-03-21 14:19:34.000000 mcrit-1.0.1/mcrit/storage/StorageInterface.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.1/mcrit/storage/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-05-12 14:54:29.857078 mcrit-1.0.1/mcrit.egg-info/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    12788 2023-05-12 14:54:29.000000 mcrit-1.0.1/mcrit.egg-info/PKG-INFO
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1950 2023-05-12 14:54:29.000000 mcrit-1.0.1/mcrit.egg-info/SOURCES.txt
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        1 2023-05-12 14:54:29.000000 mcrit-1.0.1/mcrit.egg-info/dependency_links.txt
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      135 2023-05-12 14:54:29.000000 mcrit-1.0.1/mcrit.egg-info/requires.txt
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        6 2023-05-12 14:54:29.000000 mcrit-1.0.1/mcrit.egg-info/top_level.txt
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)       38 2023-05-12 14:54:29.865078 mcrit-1.0.1/setup.cfg
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1355 2023-05-12 14:53:08.000000 mcrit-1.0.1/setup.py
```

### Comparing `mcrit-1.0.0/LICENSE` & `mcrit-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/PKG-INFO` & `mcrit-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcrit
-Version: 1.0.0
+Version: 1.0.1
 Summary: MCRIT is a framework created for simplified application of the MinHash algorithm to code similarity.
 Home-page: https://github.com/danielplohmann/mcrit
 Author: Daniel Plohmann, Manuel Blatt, Steffen Enders, Paul Hordiienko
 Author-email: daniel.plohmann@fkie.fraunhofer.de
 License: NU General Public License v3 (GPLv3)
 Description: # MinHash-based Code Relationship & Investigation Toolkit (MCRIT)
         [![Test](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml/badge.svg)](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml)
@@ -119,14 +119,15 @@
         ./plugins/ida/ida_mcrit.py
         ```
         
         in IDA.
         
         
         ## Version History
+         * 2023-05-12 v1.0.1: Some progress on label import for the IDA plugin. Reflected API extension of MCRITweb in McritClient.
          * 2023-04-10 v1.0.0: Milestone release for Botconf 2023.
          * 2023-04-10 v0.25.0: IDA plugin can now do function queries for the currently viewed function.
          * 2023-03-24 v0.24.2: McritClient can forward username/apitoken, addJsonReport is now forwardable.
          * 2023-03-21 v0.24.0: FunctionEntries now can store additional FunctionLabelEntries, along submitting user/date.
          * 2023-03-17 v0.23.0: It is now possible to query matches for single SmdaFunctions (synchronously).
          * 2023-03-15 v0.22.0: McritClient now supports apitokens and raw responses for a subset of functionality.
          * 2023-03-14 v0.21.0: Backend support for more fine grained filtering.
```

### Comparing `mcrit-1.0.0/README.md` & `mcrit-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 ./plugins/ida/ida_mcrit.py
 ```
 
 in IDA.
 
 
 ## Version History
+ * 2023-05-12 v1.0.1: Some progress on label import for the IDA plugin. Reflected API extension of MCRITweb in McritClient.
  * 2023-04-10 v1.0.0: Milestone release for Botconf 2023.
  * 2023-04-10 v0.25.0: IDA plugin can now do function queries for the currently viewed function.
  * 2023-03-24 v0.24.2: McritClient can forward username/apitoken, addJsonReport is now forwardable.
  * 2023-03-21 v0.24.0: FunctionEntries now can store additional FunctionLabelEntries, along submitting user/date.
  * 2023-03-17 v0.23.0: It is now possible to query matches for single SmdaFunctions (synchronously).
  * 2023-03-15 v0.22.0: McritClient now supports apitokens and raw responses for a subset of functionality.
  * 2023-03-14 v0.21.0: Backend support for more fine grained filtering.
```

### Comparing `mcrit-1.0.0/mcrit/Worker.py` & `mcrit-1.0.1/mcrit/Worker.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/__main__.py` & `mcrit-1.0.1/mcrit/__main__.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/client/McritClient.py` & `mcrit-1.0.1/mcrit/client/McritClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,21 +276,22 @@
         response = requests.get(f"{self.mcrit_server}/functions{query_string}", headers=self.headers)
         if self.raw:
             return response
         data = handle_response(response)
         if data is not None:
             return {int(k): FunctionEntry.fromDict(v) for k, v in data.items()}
         
-    def getFunctionsByIds(self, function_ids:list):
+    def getFunctionsByIds(self, function_ids:list, with_label_only=False):
         """
         Get all FunctionEntries identified by the provided list of function_ids
         Supported by mcritweb API pass-through
         """
+        query_with_label_only = "?with_label_only=True" if with_label_only else ""
         function_id_string = ",".join(["%d" % fid for fid in function_ids])
-        response = requests.post(f"{self.mcrit_server}/functions", data=function_id_string, headers=self.headers)
+        response = requests.post(f"{self.mcrit_server}/functions{query_with_label_only}", data=function_id_string, headers=self.headers)
         if self.raw:
             return response
         data = handle_response(response)
         if data is not None:
             return {int(k): FunctionEntry.fromDict(v) for k, v in data.items()}
         return {}
 
@@ -410,30 +411,34 @@
         pichash_size=None,
         band_matches_required=None,
         force_recalculation=False,
     ) -> None:
         params = self._getMatchingRequestParams(
             minhash_threshold, pichash_size, force_recalculation, band_matches_required
         )
-        response = requests.get(f"{self.mcrit_server}/matches/sample/{sample_id}", params=params)
+        response = requests.get(f"{self.mcrit_server}/matches/sample/{sample_id}", headers=self.headers, params=params)
+        if self.raw:
+            return response
         return handle_response(response)
 
     def requestMatchesForSampleVs(
         self,
         sample_id,
         other_sample_id,
         minhash_threshold=None,
         pichash_size=None,
         band_matches_required=None,
         force_recalculation=False,
     ) -> str:
         params = self._getMatchingRequestParams(
             minhash_threshold, pichash_size, force_recalculation, band_matches_required
         )
-        response = requests.get(f"{self.mcrit_server}/matches/sample/{sample_id}/{other_sample_id}",params=params)
+        response = requests.get(f"{self.mcrit_server}/matches/sample/{sample_id}/{other_sample_id}", headers=self.headers, params=params)
+        if self.raw:
+            return response
         return handle_response(response)
 
     def requestMatchesCross(
         self,
         sample_ids,
         minhash_threshold=None,
         pichash_size=None,
@@ -450,15 +455,17 @@
         return handle_response(response)
 
     def getMatchFunctionVs(
         self,
         function_id_a:int,
         function_id_b:int
     ) -> None:
-        response = requests.get(f"{self.mcrit_server}/matches/function/{function_id_a}/{function_id_b}")
+        response = requests.get(f"{self.mcrit_server}/matches/function/{function_id_a}/{function_id_b}", headers=self.headers)
+        if self.raw:
+            return response
         return handle_response(response)
 
 
     def getMatchesForSmdaFunction(self, smda_report, minhash_threshold=None, pichash_size=None, force_recalculation=None, band_matches_required=None, exclude_self_matches=False):
         """
         Get all matches for a SmdaReport with a single SmdaFunction
         Supported by mcritweb API pass-through
```

### Comparing `mcrit-1.0.0/mcrit/client/McritConsole.py` & `mcrit-1.0.1/mcrit/client/McritConsole.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/config/ConfigInterface.py` & `mcrit-1.0.1/mcrit/config/ConfigInterface.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/config/McritConfig.py` & `mcrit-1.0.1/mcrit/config/McritConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .ShinglerConfig import ShinglerConfig
 from .StorageConfig import StorageConfig
 
 
 class McritConfig(object):
 
     # NOTE to self: always change this in setup.py as well!
-    VERSION = "1.0.0"
+    VERSION = "1.0.1"
     CONFIG_FILE_PATH = str(os.path.abspath(__file__))
     PROJECT_ROOT = str(os.path.abspath(os.sep.join([CONFIG_FILE_PATH, "..", ".."])))
 
     ### global logging-config setup
     # Only do basicConfig if no handlers have been configured
     LOG_PATH = "./"
     LOG_LEVEL = logging.INFO
```

### Comparing `mcrit-1.0.0/mcrit/config/MinHashConfig.py` & `mcrit-1.0.1/mcrit/config/MinHashConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/config/QueueConfig.py` & `mcrit-1.0.1/mcrit/config/QueueConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/config/ShinglerConfig.py` & `mcrit-1.0.1/mcrit/config/ShinglerConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/config/StorageConfig.py` & `mcrit-1.0.1/mcrit/config/StorageConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/index/MinHashIndex.py` & `mcrit-1.0.1/mcrit/index/MinHashIndex.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,14 +259,15 @@
         if sample_entry:
             self._storage.updateFunctionLabels(smda_report, username)
             return {"existed": True, "sample_info": sample_entry.toDict()}
         sample_entry = self._storage.addSmdaReport(smda_report)
         if not sample_entry:
             return None
         LOGGER.info("Added %s", sample_entry)
+        # ensure that original function_names are also added as labels
         self._storage.updateFunctionLabels(smda_report, username)
         function_entries = self._storage.getFunctionsBySampleId(sample_entry.sample_id)
         LOGGER.info("Added %d function entries.", len(function_entries))
         job_id = None
         if calculate_hashes:
             job_id = self.updateMinHashesForSample(sample_entry.sample_id)
         return {"existed": False, "sample_info": sample_entry.toDict(), "job_id": job_id}
```

### Comparing `mcrit-1.0.0/mcrit/index/SearchCursor.py` & `mcrit-1.0.1/mcrit/index/SearchCursor.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/index/SearchQueryParser.py` & `mcrit-1.0.1/mcrit/index/SearchQueryParser.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/index/SearchQueryTree.py` & `mcrit-1.0.1/mcrit/index/SearchQueryTree.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/libs/mongoqueue.py` & `mcrit-1.0.1/mcrit/libs/mongoqueue.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/libs/pymmh3.py` & `mcrit-1.0.1/mcrit/libs/pymmh3.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/libs/utility.py` & `mcrit-1.0.1/mcrit/libs/utility.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/matchers/MatcherCross.py` & `mcrit-1.0.1/mcrit/matchers/MatcherCross.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/matchers/MatcherInterface.py` & `mcrit-1.0.1/mcrit/matchers/MatcherInterface.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/matchers/MatcherQuery.py` & `mcrit-1.0.1/mcrit/matchers/MatcherQuery.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/matchers/MatcherQueryFunction.py` & `mcrit-1.0.1/mcrit/matchers/MatcherQueryFunction.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/matchers/MatcherSample.py` & `mcrit-1.0.1/mcrit/matchers/MatcherSample.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/matchers/MatcherVs.py` & `mcrit-1.0.1/mcrit/matchers/MatcherVs.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/minhash/MinHash.py` & `mcrit-1.0.1/mcrit/minhash/MinHash.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/minhash/MinHasher.py` & `mcrit-1.0.1/mcrit/minhash/MinHasher.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/minhash/ShingleLoader.py` & `mcrit-1.0.1/mcrit/minhash/ShingleLoader.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/queue/LocalQueue.py` & `mcrit-1.0.1/mcrit/queue/LocalQueue.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/queue/QueueFactory.py` & `mcrit-1.0.1/mcrit/queue/QueueFactory.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/queue/QueueRemoteCalls.py` & `mcrit-1.0.1/mcrit/queue/QueueRemoteCalls.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/server/BlocksResource.py` & `mcrit-1.0.1/mcrit/server/BlocksResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/server/FamilyResource.py` & `mcrit-1.0.1/mcrit/server/FamilyResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/server/FunctionResource.py` & `mcrit-1.0.1/mcrit/server/FunctionResource.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,22 +44,27 @@
                     "status": "failed",
                     "data": {"message": "POST request without body can't be processed."},
                 }
             )
             resp.status = falcon.HTTP_400
             db_log_msg(self.index, req, f"FunctionResource.on_post - failed - no POST body.")
             return
+        with_label_only = False 
+        if "with_label_only" in req.params:
+            with_label_only = req.params["with_label_only"].lower().strip() == "true"
         # assume the POST body consists of comma separated function_ids
         post_body = req.stream.read()
         if re.match(b"^\d+(?:[\s]*,[\s]*\d+)*$", post_body):
             target_function_ids = [int(function_id) for function_id in post_body.split(b",")]
             function_entries = {}
             for function_id in target_function_ids:
                 function_entry = self.index.getFunctionById(function_id, with_xcfg=False).toDict()
                 if function_entry:
+                    if with_label_only and not function_entry["function_labels"]:
+                        continue
                     function_entries[function_id] = function_entry
             resp.data = jsonify({"status": "successful", "data": function_entries})
             resp.status = falcon.HTTP_200
             db_log_msg(self.index, req, f"FunctionResource.on_post - success.")
             return
         resp.status = falcon.HTTP_400
         db_log_msg(self.index, req, f"FunctionResource.on_post - failed - invalid body format.")
```

### Comparing `mcrit-1.0.0/mcrit/server/JobResource.py` & `mcrit-1.0.1/mcrit/server/JobResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/server/MatchResource.py` & `mcrit-1.0.1/mcrit/server/MatchResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/server/QueryResource.py` & `mcrit-1.0.1/mcrit/server/QueryResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/server/SampleResource.py` & `mcrit-1.0.1/mcrit/server/SampleResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/server/StatusResource.py` & `mcrit-1.0.1/mcrit/server/StatusResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/server/application_routes.py` & `mcrit-1.0.1/mcrit/server/application_routes.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/server/utils.py` & `mcrit-1.0.1/mcrit/server/utils.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/storage/FamilyEntry.py` & `mcrit-1.0.1/mcrit/storage/FamilyEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/storage/FunctionEntry.py` & `mcrit-1.0.1/mcrit/storage/FunctionEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/storage/FunctionLabelEntry.py` & `mcrit-1.0.1/mcrit/storage/FunctionLabelEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/storage/MatchedFunctionEntry.py` & `mcrit-1.0.1/mcrit/storage/MatchedFunctionEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/storage/MatchedSampleEntry.py` & `mcrit-1.0.1/mcrit/storage/MatchedSampleEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/storage/MatchingCache.py` & `mcrit-1.0.1/mcrit/storage/MatchingCache.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/storage/MatchingResult.py` & `mcrit-1.0.1/mcrit/storage/MatchingResult.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/storage/MemoryStorage.py` & `mcrit-1.0.1/mcrit/storage/MemoryStorage.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/storage/MongoDbStorage.py` & `mcrit-1.0.1/mcrit/storage/MongoDbStorage.py`

 * *Files 1% similar despite different names*

```diff
@@ -535,25 +535,25 @@
         return None
 
     def updateFunctionLabels(self, smda_report: "SmdaReport", username) -> Optional["SampleEntry"]:
         sample_entry = self.getSampleBySha256(smda_report.sha256)
         if not sample_entry:
             return False
         # check which functions in the SmdaReport have suitable function_names
-        extracted_labels = {}
+        submitted_labels = {}
         for smda_function in smda_report.getFunctions():
             function_name = smda_function.function_name
             if function_name and not re.match("sub_[a-fA-F0-9]{1,16}", function_name):
-                extracted_labels[smda_function.offset] = function_name
+                submitted_labels[smda_function.offset] = function_name
         # get the respective FunctionEntries and check if the label is novel
         sample_function_entries = {entry.offset: entry for entry in self.getFunctionsBySampleId(sample_entry.sample_id)}
         label_updates = []
-        for label_offset, extracted_label in extracted_labels.items():
+        for label_offset, extracted_label in submitted_labels.items():
             is_new_label = False
-            # we can only ever update labels if they exist in our DB
+            # we can only ever update labels if their offset exists in our DB
             if label_offset in sample_function_entries:
                 is_new_label = True
                 existing_labels = sample_function_entries[label_offset].function_labels
                 for existing_label in existing_labels:
                     if existing_label.username == username and existing_label.function_label == extracted_label:
                         is_new_label = False
             # match by function_id or offset and add the label if it had not existed before.
```

### Comparing `mcrit-1.0.0/mcrit/storage/SampleEntry.py` & `mcrit-1.0.1/mcrit/storage/SampleEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/storage/StorageFactory.py` & `mcrit-1.0.1/mcrit/storage/StorageFactory.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit/storage/StorageInterface.py` & `mcrit-1.0.1/mcrit/storage/StorageInterface.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/mcrit.egg-info/PKG-INFO` & `mcrit-1.0.1/mcrit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcrit
-Version: 1.0.0
+Version: 1.0.1
 Summary: MCRIT is a framework created for simplified application of the MinHash algorithm to code similarity.
 Home-page: https://github.com/danielplohmann/mcrit
 Author: Daniel Plohmann, Manuel Blatt, Steffen Enders, Paul Hordiienko
 Author-email: daniel.plohmann@fkie.fraunhofer.de
 License: NU General Public License v3 (GPLv3)
 Description: # MinHash-based Code Relationship & Investigation Toolkit (MCRIT)
         [![Test](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml/badge.svg)](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml)
@@ -119,14 +119,15 @@
         ./plugins/ida/ida_mcrit.py
         ```
         
         in IDA.
         
         
         ## Version History
+         * 2023-05-12 v1.0.1: Some progress on label import for the IDA plugin. Reflected API extension of MCRITweb in McritClient.
          * 2023-04-10 v1.0.0: Milestone release for Botconf 2023.
          * 2023-04-10 v0.25.0: IDA plugin can now do function queries for the currently viewed function.
          * 2023-03-24 v0.24.2: McritClient can forward username/apitoken, addJsonReport is now forwardable.
          * 2023-03-21 v0.24.0: FunctionEntries now can store additional FunctionLabelEntries, along submitting user/date.
          * 2023-03-17 v0.23.0: It is now possible to query matches for single SmdaFunctions (synchronously).
          * 2023-03-15 v0.22.0: McritClient now supports apitokens and raw responses for a subset of functionality.
          * 2023-03-14 v0.21.0: Backend support for more fine grained filtering.
```

### Comparing `mcrit-1.0.0/mcrit.egg-info/SOURCES.txt` & `mcrit-1.0.1/mcrit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.0/setup.py` & `mcrit-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "smda>=1.3.0",
     "tqdm",
     "waitress",
 ]
 
 setup(
     name='mcrit',
-    version="1.0.0",
+    version="1.0.1",
     description='MCRIT is a framework created for simplified application of the MinHash algorithm to code similarity.',
     long_description_content_type="text/markdown",
     long_description=README,
     author='Daniel Plohmann, Manuel Blatt, Steffen Enders, Paul Hordiienko',
     author_email='daniel.plohmann@fkie.fraunhofer.de',
     url='https://github.com/danielplohmann/mcrit',
     license="NU General Public License v3 (GPLv3)",
```

